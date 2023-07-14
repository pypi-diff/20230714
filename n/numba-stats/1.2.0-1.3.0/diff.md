# Comparing `tmp/numba-stats-1.2.0.tar.gz` & `tmp/numba-stats-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numba-stats-1.2.0.tar", last modified: Tue May  9 11:25:45 2023, max compression
+gzip compressed data, was "numba-stats-1.3.0.tar", last modified: Fri Jul 14 09:19:25 2023, max compression
```

## Comparing `numba-stats-1.2.0.tar` & `numba-stats-1.3.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:45.130054 numba-stats-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:45.114054 numba-stats-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:45.118054 numba-stats-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-09 11:25:14.000000 numba-stats-1.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-09 11:25:14.000000 numba-stats-1.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-09 11:25:14.000000 numba-stats-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-09 11:25:14.000000 numba-stats-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-09 11:25:14.000000 numba-stats-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-09 11:25:14.000000 numba-stats-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-09 11:25:45.130054 numba-stats-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-09 11:25:14.000000 numba-stats-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:45.118054 numba-stats-1.2.0/bench/
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-09 11:25:14.000000 numba-stats-1.2.0/bench/plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-05-09 11:25:14.000000 numba-stats-1.2.0/bench/test_stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-05-09 11:25:14.000000 numba-stats-1.2.0/coverage.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:45.114054 numba-stats-1.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:45.122054 numba-stats-1.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    70602 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/bernstein.density.svg
--rw-r--r--   0 runner    (1001) docker     (123)    58277 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/expon.cdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    57880 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/expon.pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    58675 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/expon.ppf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    58022 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/norm.cdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    58418 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/norm.pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    58822 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/norm.ppf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    59429 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/t.cdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    61026 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/t.pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    57399 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/t.ppf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    58746 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/truncexpon.cdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    59714 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/truncexpon.pdf.plus.norm.pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    58950 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/truncexpon.pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    58745 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/truncexpon.ppf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    62491 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/truncnorm.cdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    59095 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/truncnorm.pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    61300 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/truncnorm.ppf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    58793 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/uniform.cdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    58392 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/uniform.pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    58792 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/uniform.ppf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    60274 2023-05-09 11:25:14.000000 numba-stats-1.2.0/docs/_static/voigt.pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-09 11:25:14.000000 numba-stats-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-09 11:25:45.130054 numba-stats-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-09 11:25:14.000000 numba-stats-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:45.114054 numba-stats-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:45.126054 numba-stats-1.2.0/src/numba_stats/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/_special.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-09 11:25:30.000000 numba-stats-1.2.0/src/numba_stats/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/bernstein.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/cpoisson.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/cruijff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/crystalball.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/crystalball_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/expon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/lognorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/poisson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/qgaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/t.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/truncexpon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/truncnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/tsallis.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-09 11:25:14.000000 numba-stats-1.2.0/src/numba_stats/voigt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:45.126054 numba-stats-1.2.0/src/numba_stats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-09 11:25:44.000000 numba-stats-1.2.0/src/numba_stats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-09 11:25:44.000000 numba-stats-1.2.0/src/numba_stats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:25:44.000000 numba-stats-1.2.0/src/numba_stats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-09 11:25:44.000000 numba-stats-1.2.0/src/numba_stats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 11:25:44.000000 numba-stats-1.2.0/src/numba_stats.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:45.130054 numba-stats-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_bernstein.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_cpoisson.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_cruijff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_crystalball.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_crystalball_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_expon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_lognorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_poisson.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_qgaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_t.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_truncexpon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_truncnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_tsallis.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-09 11:25:14.000000 numba-stats-1.2.0/tests/test_voigt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:19:25.192346 numba-stats-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:19:25.184346 numba-stats-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:19:25.184346 numba-stats-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 09:19:01.000000 numba-stats-1.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-14 09:19:01.000000 numba-stats-1.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-14 09:19:01.000000 numba-stats-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-14 09:19:01.000000 numba-stats-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-14 09:19:01.000000 numba-stats-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 09:19:01.000000 numba-stats-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-07-14 09:19:25.192346 numba-stats-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-07-14 09:19:01.000000 numba-stats-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:19:25.184346 numba-stats-1.3.0/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-14 09:19:01.000000 numba-stats-1.3.0/bench/plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-14 09:19:01.000000 numba-stats-1.3.0/bench/test_stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-07-14 09:19:01.000000 numba-stats-1.3.0/coverage.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:19:25.184346 numba-stats-1.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:19:25.188346 numba-stats-1.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    70602 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/bernstein.density.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58277 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/expon.cdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    57880 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/expon.pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58675 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/expon.ppf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58022 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/norm.cdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58418 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/norm.pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58822 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/norm.ppf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    59429 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/t.cdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    61026 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/t.pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    57399 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/t.ppf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58746 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/truncexpon.cdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    59714 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/truncexpon.pdf.plus.norm.pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58950 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/truncexpon.pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58745 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/truncexpon.ppf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    62491 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/truncnorm.cdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    59095 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/truncnorm.pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    61300 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/truncnorm.ppf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58793 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/uniform.cdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58392 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/uniform.pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    58792 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/uniform.ppf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    60274 2023-07-14 09:19:01.000000 numba-stats-1.3.0/docs/_static/voigt.pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-14 09:19:01.000000 numba-stats-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-14 09:19:25.192346 numba-stats-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-14 09:19:01.000000 numba-stats-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:19:25.184346 numba-stats-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:19:25.192346 numba-stats-1.3.0/src/numba_stats/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 09:19:01.000000 numba-stats-1.3.0/src/numba_stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-14 09:19:01.000000 numba-stats-1.3.0/src/numba_stats/_special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-14 09:19:01.000000 numba-stats-1.3.0/src/numba_stats/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 09:19:13.000000 numba-stats-1.3.0/src/numba_stats/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-07-14 09:19:01.000000 numba-stats-1.3.0/src/numba_stats/bernstein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-14 09:19:01.000000 numba-stats-1.3.0/src/numba_stats/cpoisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-14 09:19:01.000000 numba-stats-1.3.0/src/numba_stats/cruijff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-14 09:19:01.000000 numba-stats-1.3.0/src/numba_stats/crystalball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-14 09:19:01.000000 numba-stats-1.3.0/src/numba_stats/crystalball_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-14 09:19:01.000000 numba-stats-1.3.0/src/numba_stats/expon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-14 09:19:01.000000 numba-stats-1.3.0/src/numba_stats/lognorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-14 09:19:01.000000 numba-stats-1.3.0/src/numba_stats/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-14 09:19:01.000000 numba-stats-1.3.0/src/numba_stats/poisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-14 09:19:01.000000 numba-stats-1.3.0/src/numba_stats/qgaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-14 09:19:01.000000 numba-stats-1.3.0/src/numba_stats/t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-14 09:19:01.000000 numba-stats-1.3.0/src/numba_stats/truncexpon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-14 09:19:01.000000 numba-stats-1.3.0/src/numba_stats/truncnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-14 09:19:01.000000 numba-stats-1.3.0/src/numba_stats/tsallis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-14 09:19:01.000000 numba-stats-1.3.0/src/numba_stats/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-14 09:19:01.000000 numba-stats-1.3.0/src/numba_stats/voigt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:19:25.192346 numba-stats-1.3.0/src/numba_stats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-07-14 09:19:25.000000 numba-stats-1.3.0/src/numba_stats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-14 09:19:25.000000 numba-stats-1.3.0/src/numba_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:19:25.000000 numba-stats-1.3.0/src/numba_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-14 09:19:25.000000 numba-stats-1.3.0/src/numba_stats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 09:19:25.000000 numba-stats-1.3.0/src/numba_stats.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:19:25.192346 numba-stats-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:19:01.000000 numba-stats-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-14 09:19:01.000000 numba-stats-1.3.0/tests/test_bernstein.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-14 09:19:01.000000 numba-stats-1.3.0/tests/test_cpoisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-14 09:19:01.000000 numba-stats-1.3.0/tests/test_cruijff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-07-14 09:19:01.000000 numba-stats-1.3.0/tests/test_crystalball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-14 09:19:01.000000 numba-stats-1.3.0/tests/test_crystalball_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-14 09:19:01.000000 numba-stats-1.3.0/tests/test_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-14 09:19:01.000000 numba-stats-1.3.0/tests/test_expon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-14 09:19:01.000000 numba-stats-1.3.0/tests/test_lognorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-14 09:19:01.000000 numba-stats-1.3.0/tests/test_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-14 09:19:01.000000 numba-stats-1.3.0/tests/test_poisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-14 09:19:01.000000 numba-stats-1.3.0/tests/test_qgaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-14 09:19:01.000000 numba-stats-1.3.0/tests/test_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-14 09:19:01.000000 numba-stats-1.3.0/tests/test_truncexpon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-14 09:19:01.000000 numba-stats-1.3.0/tests/test_truncnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-14 09:19:01.000000 numba-stats-1.3.0/tests/test_tsallis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-14 09:19:01.000000 numba-stats-1.3.0/tests/test_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-14 09:19:01.000000 numba-stats-1.3.0/tests/test_voigt.py
```

### Comparing `numba-stats-1.2.0/.github/workflows/release.yml` & `numba-stats-1.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/.pre-commit-config.yaml` & `numba-stats-1.3.0/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -43,10 +43,10 @@
   hooks:
   - id: pydocstyle
     args: ["--convention=numpy"]
     files: src/numba_stats/[^_].*\.py
 
 # Python formatting
 - repo: https://github.com/psf/black
-  rev: 23.3.0
+  rev: 23.7.0
   hooks:
   - id: black
```

### Comparing `numba-stats-1.2.0/LICENSE` & `numba-stats-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/PKG-INFO` & `numba-stats-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numba-stats
-Version: 1.2.0
+Version: 1.3.0
 Summary: Numba-accelerated implementations of common probability distributions
 Home-page: UNKNOWN
 Author: Hans Dembinski
 Author-email: hans.dembinski@gmail.com
 License: "MIT"
 Project-URL: Bug Tracker, https://github.com/hdembinski/numba-stats/issues
 Platform: UNKNOWN
@@ -101,15 +101,14 @@
 ![](docs/_static/truncnorm.cdf.svg)
 ![](docs/_static/truncnorm.ppf.svg)
 ![](docs/_static/truncexpon.pdf.svg)
 ![](docs/_static/truncexpon.cdf.svg)
 ![](docs/_static/truncexpon.ppf.svg)
 ![](docs/_static/voigt.pdf.svg)
 ![](docs/_static/bernstein.density.svg)
-![](docs/_static/bernstein.density.svg)
 ![](docs/_static/truncexpon.pdf.plus.norm.pdf.svg)
 
 ## Documentation
 
 To get documentation, please use `help()` in the Python interpreter.
 
 Functions with equivalents in `scipy.stats` follow the `scipy` calling conventions exactly, except for distributions starting with `trunc...`, which follow a different convention, since the `scipy` behavior is very impractical. Even so, note that the `scipy` conventions are sometimes a bit unusual, particular in case of the exponential, the log-normal, and the uniform distribution. See the `scipy` docs for details.
```

### Comparing `numba-stats-1.2.0/README.md` & `numba-stats-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,14 @@
 ![](docs/_static/truncnorm.cdf.svg)
 ![](docs/_static/truncnorm.ppf.svg)
 ![](docs/_static/truncexpon.pdf.svg)
 ![](docs/_static/truncexpon.cdf.svg)
 ![](docs/_static/truncexpon.ppf.svg)
 ![](docs/_static/voigt.pdf.svg)
 ![](docs/_static/bernstein.density.svg)
-![](docs/_static/bernstein.density.svg)
 ![](docs/_static/truncexpon.pdf.plus.norm.pdf.svg)
 
 ## Documentation
 
 To get documentation, please use `help()` in the Python interpreter.
 
 Functions with equivalents in `scipy.stats` follow the `scipy` calling conventions exactly, except for distributions starting with `trunc...`, which follow a different convention, since the `scipy` behavior is very impractical. Even so, note that the `scipy` conventions are sometimes a bit unusual, particular in case of the exponential, the log-normal, and the uniform distribution. See the `scipy` docs for details.
```

### Comparing `numba-stats-1.2.0/bench/plot.ipynb` & `numba-stats-1.3.0/bench/plot.ipynb`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/bench/test_stats.py` & `numba-stats-1.3.0/bench/test_stats.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/bernstein.density.svg` & `numba-stats-1.3.0/docs/_static/bernstein.density.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/expon.cdf.svg` & `numba-stats-1.3.0/docs/_static/expon.cdf.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/expon.pdf.svg` & `numba-stats-1.3.0/docs/_static/expon.pdf.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/expon.ppf.svg` & `numba-stats-1.3.0/docs/_static/expon.ppf.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/norm.cdf.svg` & `numba-stats-1.3.0/docs/_static/norm.cdf.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/norm.pdf.svg` & `numba-stats-1.3.0/docs/_static/norm.pdf.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/norm.ppf.svg` & `numba-stats-1.3.0/docs/_static/norm.ppf.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/t.cdf.svg` & `numba-stats-1.3.0/docs/_static/t.cdf.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/t.pdf.svg` & `numba-stats-1.3.0/docs/_static/t.pdf.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/t.ppf.svg` & `numba-stats-1.3.0/docs/_static/t.ppf.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/truncexpon.cdf.svg` & `numba-stats-1.3.0/docs/_static/truncexpon.cdf.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/truncexpon.pdf.plus.norm.pdf.svg` & `numba-stats-1.3.0/docs/_static/truncexpon.pdf.plus.norm.pdf.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/truncexpon.pdf.svg` & `numba-stats-1.3.0/docs/_static/truncexpon.pdf.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/truncexpon.ppf.svg` & `numba-stats-1.3.0/docs/_static/truncexpon.ppf.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/truncnorm.cdf.svg` & `numba-stats-1.3.0/docs/_static/truncnorm.cdf.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/truncnorm.pdf.svg` & `numba-stats-1.3.0/docs/_static/truncnorm.pdf.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/truncnorm.ppf.svg` & `numba-stats-1.3.0/docs/_static/truncnorm.ppf.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/uniform.cdf.svg` & `numba-stats-1.3.0/docs/_static/uniform.cdf.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/uniform.pdf.svg` & `numba-stats-1.3.0/docs/_static/uniform.pdf.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/uniform.ppf.svg` & `numba-stats-1.3.0/docs/_static/uniform.ppf.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/docs/_static/voigt.pdf.svg` & `numba-stats-1.3.0/docs/_static/voigt.pdf.svg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/setup.cfg` & `numba-stats-1.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/src/numba_stats/_special.py` & `numba-stats-1.3.0/src/numba_stats/_special.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/src/numba_stats/_util.py` & `numba-stats-1.3.0/src/numba_stats/_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,18 @@
     return Array(T, 1, "A", readonly=True)
 
 
 def _jit(arg, cache=True):
     """
     Wrapper for numba.njit to reduce boilerplate code.
 
-    We want to build jitted functions with explicit signatures to restrict
-    the argument types which are used in the implemnetation to float32 or
-    float64. We also want to pass specific options consistently
-    (e.g. error_model='numpy').
+    We want to build jitted functions with explicit signatures to restrict the argument
+    types which are used in the implemnetation to float32 or float64. We also want to
+    pass specific options consistently: error_model='numpy' and inline='always'. The
+    latter is important to profit from auto-parallelization of surrounding code.
 
     Parameters
     ----------
     arg : int
         Number of arguments. If negative, all arguments of this function are scalars
         and -arg is the number of arguments. If positive, the first argument is
         an array, the others are scalars and arg is the number of scalar arguments.
```

### Comparing `numba-stats-1.2.0/src/numba_stats/bernstein.py` & `numba-stats-1.3.0/src/numba_stats/bernstein.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/src/numba_stats/cpoisson.py` & `numba-stats-1.3.0/src/numba_stats/cpoisson.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/src/numba_stats/cruijff.py` & `numba-stats-1.3.0/src/numba_stats/cruijff.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 scale_left : float
     Left width parameter.
 scale_right: float
     Right width parameter.
 """
 
 
-@_jit(6)
-def _density(x, ymax, beta_left, beta_right, loc, scale_left, scale_right):
+@_jit(5)
+def _density(x, beta_left, beta_right, loc, scale_left, scale_right):
     r = np.empty_like(x)
     for i in _prange(len(x)):
         if x[i] < loc:
             scale = scale_left
             beta = beta_left
         else:
             scale = scale_right
             beta = beta_right
         z = (x[i] - loc) / scale
         r[i] = -0.5 * z**2 / (1 + beta * z**2)
-    return ymax * np.exp(r)
+    return np.exp(r)
 
 
 _generate_wrappers(globals())
```

### Comparing `numba-stats-1.2.0/src/numba_stats/crystalball.py` & `numba-stats-1.3.0/src/numba_stats/crystalball.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/src/numba_stats/crystalball_ex.py` & `numba-stats-1.3.0/src/numba_stats/crystalball_ex.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/src/numba_stats/expon.py` & `numba-stats-1.3.0/src/numba_stats/expon.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/src/numba_stats/lognorm.py` & `numba-stats-1.3.0/src/numba_stats/lognorm.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/src/numba_stats/norm.py` & `numba-stats-1.3.0/src/numba_stats/norm.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/src/numba_stats/poisson.py` & `numba-stats-1.3.0/src/numba_stats/poisson.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/src/numba_stats/qgaussian.py` & `numba-stats-1.3.0/src/numba_stats/qgaussian.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/src/numba_stats/t.py` & `numba-stats-1.3.0/src/numba_stats/t.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/src/numba_stats/truncexpon.py` & `numba-stats-1.3.0/src/numba_stats/truncexpon.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/src/numba_stats/truncnorm.py` & `numba-stats-1.3.0/src/numba_stats/truncnorm.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/src/numba_stats/tsallis.py` & `numba-stats-1.3.0/src/numba_stats/tsallis.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/src/numba_stats/uniform.py` & `numba-stats-1.3.0/src/numba_stats/uniform.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/src/numba_stats/voigt.py` & `numba-stats-1.3.0/src/numba_stats/voigt.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/src/numba_stats.egg-info/PKG-INFO` & `numba-stats-1.3.0/src/numba_stats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numba-stats
-Version: 1.2.0
+Version: 1.3.0
 Summary: Numba-accelerated implementations of common probability distributions
 Home-page: UNKNOWN
 Author: Hans Dembinski
 Author-email: hans.dembinski@gmail.com
 License: "MIT"
 Project-URL: Bug Tracker, https://github.com/hdembinski/numba-stats/issues
 Platform: UNKNOWN
@@ -101,15 +101,14 @@
 ![](docs/_static/truncnorm.cdf.svg)
 ![](docs/_static/truncnorm.ppf.svg)
 ![](docs/_static/truncexpon.pdf.svg)
 ![](docs/_static/truncexpon.cdf.svg)
 ![](docs/_static/truncexpon.ppf.svg)
 ![](docs/_static/voigt.pdf.svg)
 ![](docs/_static/bernstein.density.svg)
-![](docs/_static/bernstein.density.svg)
 ![](docs/_static/truncexpon.pdf.plus.norm.pdf.svg)
 
 ## Documentation
 
 To get documentation, please use `help()` in the Python interpreter.
 
 Functions with equivalents in `scipy.stats` follow the `scipy` calling conventions exactly, except for distributions starting with `trunc...`, which follow a different convention, since the `scipy` behavior is very impractical. Even so, note that the `scipy` conventions are sometimes a bit unusual, particular in case of the exponential, the log-normal, and the uniform distribution. See the `scipy` docs for details.
```

### Comparing `numba-stats-1.2.0/src/numba_stats.egg-info/SOURCES.txt` & `numba-stats-1.3.0/src/numba_stats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/tests/test_bernstein.py` & `numba-stats-1.3.0/tests/test_bernstein.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/tests/test_cruijff.py` & `numba-stats-1.3.0/tests/test_cruijff.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 import numpy as np
 from scipy.stats import norm
 from numpy.testing import assert_allclose
 
 
 def test_density_1():
     x = np.linspace(-5, 5, 100)
-    got = cruijff.density(x, 1 / np.sqrt(2 * np.pi), 0, 0, 0, 1, 1)
+    got = cruijff.density(x, 0, 0, 0, 1, 1) / np.sqrt(2 * np.pi)
     expected = norm().pdf(x)
     assert_allclose(got, expected)
 
 
 def test_density_2():
     x = np.linspace(-5, 5, 100)
-    got = cruijff.density(x, 1, 0.1, 0.2, 1.5, 2.1, 2.1)
-    expected = cruijff.density((x - 1.5) / 2.1, 1, 0.1, 0.2, 0, 1, 1)
+    got = cruijff.density(x, 0.1, 0.2, 1.5, 2.1, 2.1)
+    expected = cruijff.density((x - 1.5) / 2.1, 0.1, 0.2, 0, 1, 1)
     assert_allclose(got, expected)
 
 
 def test_density_3():
     x = np.linspace(-5, 5, 100)
-    y = cruijff.density(x, 1, 0.2, 0.3, 0, 1.1, 1.2)
+    y = cruijff.density(x, 0.2, 0.3, 0, 1.1, 1.2)
     dy = np.diff(y, 1)
     # density should be smooth
     assert_allclose(dy, 0, atol=0.05)
     # function rises up to x = 0
     assert np.all(dy[x[1:] < 0] > 0)
     # function falls after x = 0
     assert np.all(dy[x[1:] > 0.1] < 0)
```

### Comparing `numba-stats-1.2.0/tests/test_crystalball.py` & `numba-stats-1.3.0/tests/test_crystalball.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/tests/test_crystalball_ex.py` & `numba-stats-1.3.0/tests/test_crystalball_ex.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/tests/test_doc.py` & `numba-stats-1.3.0/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/tests/test_expon.py` & `numba-stats-1.3.0/tests/test_expon.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/tests/test_lognorm.py` & `numba-stats-1.3.0/tests/test_lognorm.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/tests/test_norm.py` & `numba-stats-1.3.0/tests/test_norm.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/tests/test_qgaussian.py` & `numba-stats-1.3.0/tests/test_qgaussian.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/tests/test_t.py` & `numba-stats-1.3.0/tests/test_t.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/tests/test_truncexpon.py` & `numba-stats-1.3.0/tests/test_truncexpon.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/tests/test_truncnorm.py` & `numba-stats-1.3.0/tests/test_truncnorm.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/tests/test_tsallis.py` & `numba-stats-1.3.0/tests/test_tsallis.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.2.0/tests/test_uniform.py` & `numba-stats-1.3.0/tests/test_uniform.py`

 * *Files identical despite different names*

