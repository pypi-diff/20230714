# Comparing `tmp/petl_retouched_version-0.1.1.tar.gz` & `tmp/petl_retouched_version-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petl_retouched_version-0.1.1.tar", last modified: Tue Jun  6 13:24:40 2023, max compression
+gzip compressed data, was "petl_retouched_version-0.1.2.tar", last modified: Fri Jul 14 11:31:00 2023, max compression
```

## Comparing `petl_retouched_version-0.1.1.tar` & `petl_retouched_version-0.1.2.tar`

### file list

```diff
@@ -1,251 +1,251 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:40.623942 petl_retouched_version-0.1.1/
--rw-rw-rw-   0        0        0       91 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/.coveragerc
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:38.334374 petl_retouched_version-0.1.1/.github/
--rw-rw-rw-   0        0        0      170 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/.github/CONTRIBUTING.md
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:38.384118 petl_retouched_version-0.1.1/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0     1454 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-rw-   0        0        0     1105 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-rw-   0        0        0     1428 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:38.467666 petl_retouched_version-0.1.1/.github/workflows/
--rw-rw-rw-   0        0        0     2314 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/.github/workflows/codacy-analysis.yml
--rw-rw-rw-   0        0        0     2430 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/.github/workflows/codeql-analysis.yml
--rw-rw-rw-   0        0        0      889 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/.github/workflows/publish-release.yml
--rw-rw-rw-   0        0        0     6575 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/.github/workflows/test-changes.yml
--rw-rw-rw-   0        0        0     3440 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/.gitignore
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:38.533070 petl_retouched_version-0.1.1/.vscode/
--rw-rw-rw-   0        0        0      428 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/.vscode/launch.json
--rw-rw-rw-   0        0        0     4486 2023-05-24 16:48:57.000000 petl_retouched_version-0.1.1/.vscode/settings.json
--rw-rw-rw-   0        0        0     1383 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/.vscode/tasks.json
--rw-rw-rw-   0        0        0     1087 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       47 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2309 2023-06-06 13:24:40.614287 petl_retouched_version-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1738 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/README.rst
--rw-rw-rw-   0        0        0      933 2023-05-27 19:11:07.000000 petl_retouched_version-0.1.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:38.552129 petl_retouched_version-0.1.1/bin/
--rw-rw-rw-   0        0        0      761 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/bin/petl
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:38.774186 petl_retouched_version-0.1.1/docs/
--rw-rw-rw-   0        0        0     4712 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/docs/Makefile
--rw-rw-rw-   0        0        0     2836 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/docs/acknowledgments.rst
--rw-rw-rw-   0        0        0    25474 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/docs/changes.rst
--rw-rw-rw-   0        0        0     7701 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/docs/conf.py
--rw-rw-rw-   0        0        0       96 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.1/docs/config.rst
--rw-rw-rw-   0        0        0     4764 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/docs/contributing.rst
--rw-rw-rw-   0        0        0     1895 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/docs/index.rst
--rw-rw-rw-   0        0        0     2572 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/docs/install.rst
--rw-rw-rw-   0        0        0    13271 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/docs/intro.rst
--rw-rw-rw-   0        0        0    13307 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/docs/io.rst
--rwxrwxrwx   0        0        0     4257 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/docs/make.bat
--rw-rw-rw-   0        0        0   154638 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/docs/petl-architecture.png
--rw-rw-rw-   0        0        0     9685 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/docs/related_work.rst
--rw-rw-rw-   0        0        0     9141 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/docs/transform.rst
--rw-rw-rw-   0        0        0     3149 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/docs/util.rst
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:38.814553 petl_retouched_version-0.1.1/examples/
--rw-rw-rw-   0        0        0      368 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/comparison.py
--rw-rw-rw-   0        0        0      891 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/intro.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:39.148545 petl_retouched_version-0.1.1/examples/io/
--rw-rw-rw-   0        0        0      670 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/io/csv.py
--rw-rw-rw-   0        0        0      305 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/io/html.py
--rw-rw-rw-   0        0        0     1018 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/io/json.py
--rw-rw-rw-   0        0        0      993 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/io/numpy.py
--rw-rw-rw-   0        0        0      548 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/io/pandas.py
--rw-rw-rw-   0        0        0      676 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/io/pickle.py
--rw-rw-rw-   0        0        0     2708 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/io/pytables.py
--rw-rw-rw-   0        0        0     1005 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/io/sqlite3.py
--rw-rw-rw-   0        0        0      758 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/io/text.py
--rw-rw-rw-   0        0        0     2595 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/io/whoosh.py
--rw-rw-rw-   0        0        0     1465 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/io/xml.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:39.567288 petl_retouched_version-0.1.1/examples/notes/
--rw-rw-rw-   0        0        0       15 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/notes/.gitignore
--rw-rw-rw-   0        0        0    13376 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/notes/20140424_example.ipynb
--rw-rw-rw-   0        0        0     1573 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/notes/20140424_example.py
--rw-rw-rw-   0        0        0     4268 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/notes/20141022_example.ipynb
--rw-rw-rw-   0        0        0     7825 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/notes/20141110_example.ipynb
--rw-rw-rw-   0        0        0    11359 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/notes/20150319 resolve conflicts.ipynb
--rw-rw-rw-   0        0        0     3335 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/notes/20150331 split null.ipynb
--rw-rw-rw-   0        0        0    55658 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/notes/case_study_1.ipynb
--rw-rw-rw-   0        0        0    13673 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/notes/issue_219.ipynb
--rw-rw-rw-   0        0        0     2119 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/notes/issue_219.py
--rw-rw-rw-   0        0        0     6135 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/notes/issue_256.ipynb
--rw-rw-rw-   0        0        0      905 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/notes/issue_256.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:39.875104 petl_retouched_version-0.1.1/examples/transform/
--rw-rw-rw-   0        0        0     4542 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/transform/basics.py
--rw-rw-rw-   0        0        0     1813 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/transform/conversions.py
--rw-rw-rw-   0        0        0     1392 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/transform/dedup.py
--rw-rw-rw-   0        0        0     1175 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/transform/fills.py
--rw-rw-rw-   0        0        0     1191 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/transform/headers.py
--rw-rw-rw-   0        0        0     3869 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/transform/intervals.py
--rw-rw-rw-   0        0        0     3677 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/transform/joins.py
--rw-rw-rw-   0        0        0     2179 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/transform/maps.py
--rw-rw-rw-   0        0        0     2502 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/transform/reductions.py
--rw-rw-rw-   0        0        0     1738 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/transform/regex.py
--rw-rw-rw-   0        0        0     3993 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/transform/reshape.py
--rw-rw-rw-   0        0        0     1811 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/transform/selects.py
--rw-rw-rw-   0        0        0     1973 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/transform/setops.py
--rw-rw-rw-   0        0        0     1169 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/transform/sorts.py
--rw-rw-rw-   0        0        0      550 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/transform/unpacks.py
--rw-rw-rw-   0        0        0      929 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/transform/validation.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:40.137884 petl_retouched_version-0.1.1/examples/util/
--rw-rw-rw-   0        0        0     1905 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/util/base.py
--rw-rw-rw-   0        0        0     2828 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.1/examples/util/counting.py
--rw-rw-rw-   0        0        0     3972 2023-05-23 16:57:38.000000 petl_retouched_version-0.1.1/examples/util/lookups.py
--rw-rw-rw-   0        0        0      449 2023-05-23 16:57:38.000000 petl_retouched_version-0.1.1/examples/util/materialise.py
--rw-rw-rw-   0        0        0     1009 2023-05-23 16:57:38.000000 petl_retouched_version-0.1.1/examples/util/misc.py
--rw-rw-rw-   0        0        0     1126 2023-05-23 16:57:38.000000 petl_retouched_version-0.1.1/examples/util/parsers.py
--rw-rw-rw-   0        0        0      607 2023-05-23 16:57:38.000000 petl_retouched_version-0.1.1/examples/util/random.py
--rw-rw-rw-   0        0        0      475 2023-05-23 16:57:38.000000 petl_retouched_version-0.1.1/examples/util/statistics.py
--rw-rw-rw-   0        0        0      583 2023-05-23 16:57:38.000000 petl_retouched_version-0.1.1/examples/util/timing.py
--rw-rw-rw-   0        0        0      590 2023-05-23 16:57:38.000000 petl_retouched_version-0.1.1/examples/util/vis.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:35.788641 petl_retouched_version-0.1.1/petl/
--rw-rw-rw-   0        0        0      415 2023-05-30 14:22:22.000000 petl_retouched_version-0.1.1/petl/__init__.py
--rw-rw-rw-   0        0        0     3888 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/comparison.py
--rw-rw-rw-   0        0        0     1802 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/compat.py
--rw-rw-rw-   0        0        0      793 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/config.py
--rw-rw-rw-   0        0        0      631 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/errors.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:36.360715 petl_retouched_version-0.1.1/petl/io/
--rw-rw-rw-   0        0        0     1485 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/__init__.py
--rw-rw-rw-   0        0        0    20835 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/avro.py
--rw-rw-rw-   0        0        0     1946 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/base.py
--rw-rw-rw-   0        0        0     6282 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/bcolz.py
--rw-rw-rw-   0        0        0     6258 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/csv.py
--rw-rw-rw-   0        0        0     5433 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/csv_py2.py
--rw-rw-rw-   0        0        0     2995 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/csv_py3.py
--rw-rw-rw-   0        0        0    30462 2023-06-06 10:27:02.000000 petl_retouched_version-0.1.1/petl/io/db.py
--rw-rw-rw-   0        0        0    11440 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/db_create.py
--rw-rw-rw-   0        0        0     3117 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/db_utils.py
--rw-rw-rw-   0        0        0     8266 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/gsheet.py
--rw-rw-rw-   0        0        0     8683 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/html.py
--rw-rw-rw-   0        0        0    14004 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/json.py
--rw-rw-rw-   0        0        0     5434 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/numpy.py
--rw-rw-rw-   0        0        0     2689 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/pandas.py
--rw-rw-rw-   0        0        0     4547 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/pickle.py
--rw-rw-rw-   0        0        0    12977 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/pytables.py
--rw-rw-rw-   0        0        0     8731 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/remotes.py
--rw-rw-rw-   0        0        0    13121 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/sources.py
--rw-rw-rw-   0        0        0     8278 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/text.py
--rw-rw-rw-   0        0        0    17839 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/whoosh.py
--rw-rw-rw-   0        0        0     3541 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/xls.py
--rw-rw-rw-   0        0        0     6914 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/xlsx.py
--rw-rw-rw-   0        0        0     4545 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/xlutils_view.py
--rw-rw-rw-   0        0        0    16130 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/io/xml.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:36.530550 petl_retouched_version-0.1.1/petl/test/
--rw-rw-rw-   0        0        0        0 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/__init__.py
--rw-rw-rw-   0        0        0      205 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/conftest.py
--rw-rw-rw-   0        0        0     3685 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/failonerror.py
--rw-rw-rw-   0        0        0     2569 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:37.199990 petl_retouched_version-0.1.1/petl/test/io/
--rw-rw-rw-   0        0        0       66 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/__init__.py
--rw-rw-rw-   0        0        0    11773 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_avro.py
--rw-rw-rw-   0        0        0     6373 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_avro_schemas.py
--rw-rw-rw-   0        0        0     2198 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_bcolz.py
--rw-rw-rw-   0        0        0     7929 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_csv.py
--rw-rw-rw-   0        0        0     4334 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_csv_unicode.py
--rw-rw-rw-   0        0        0     6855 2023-05-27 19:17:16.000000 petl_retouched_version-0.1.1/petl/test/io/test_db.py
--rw-rw-rw-   0        0        0     7980 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_db_create.py
--rw-rw-rw-   0        0        0    11239 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_db_server.py
--rw-rw-rw-   0        0        0     8878 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_gsheet.py
--rw-rw-rw-   0        0        0     3296 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_html.py
--rw-rw-rw-   0        0        0     1499 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_html_unicode.py
--rw-rw-rw-   0        0        0     8129 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_json.py
--rw-rw-rw-   0        0        0      775 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_json_unicode.py
--rw-rw-rw-   0        0        0     3043 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_jsonl.py
--rw-rw-rw-   0        0        0     6186 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_numpy.py
--rw-rw-rw-   0        0        0     1348 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_pandas.py
--rw-rw-rw-   0        0        0     1635 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_pickle.py
--rw-rw-rw-   0        0        0     7076 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_pytables.py
--rw-rw-rw-   0        0        0     6383 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_remotes.py
--rw-rw-rw-   0        0        0     4186 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_sources.py
--rw-rw-rw-   0        0        0     4999 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_sqlite3.py
--rw-rw-rw-   0        0        0     6686 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_tees.py
--rw-rw-rw-   0        0        0     3985 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_text.py
--rw-rw-rw-   0        0        0     2126 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_text_unicode.py
--rw-rw-rw-   0        0        0     8598 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_whoosh.py
--rw-rw-rw-   0        0        0     3880 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_xls.py
--rw-rw-rw-   0        0        0     6710 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.1/petl/test/io/test_xlsx.py
--rw-rw-rw-   0        0        0    15051 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/io/test_xml.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:40.411877 petl_retouched_version-0.1.1/petl/test/resources/
--rw-rw-rw-   0        0        0    21504 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/resources/test.xls
--rw-rw-rw-   0        0        0     9596 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/resources/test.xlsx
--rw-rw-rw-   0        0        0      424 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/resources/test.xml
--rw-rw-rw-   0        0        0     4837 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/test_comparison.py
--rw-rw-rw-   0        0        0     3093 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/test_fluent.py
--rw-rw-rw-   0        0        0     1294 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/test_helpers.py
--rw-rw-rw-   0        0        0     1780 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/test_interactive.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:37.575973 petl_retouched_version-0.1.1/petl/test/transform/
--rw-rw-rw-   0        0        0       66 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/transform/__init__.py
--rw-rw-rw-   0        0        0    20074 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/transform/test_basics.py
--rw-rw-rw-   0        0        0    11234 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/transform/test_conversions.py
--rw-rw-rw-   0        0        0     7317 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/transform/test_dedup.py
--rw-rw-rw-   0        0        0     2695 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/transform/test_fills.py
--rw-rw-rw-   0        0        0     7236 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/transform/test_headers.py
--rw-rw-rw-   0        0        0    33773 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/transform/test_intervals.py
--rw-rw-rw-   0        0        0    44856 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/transform/test_joins.py
--rw-rw-rw-   0        0        0    11199 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/transform/test_maps.py
--rw-rw-rw-   0        0        0    15028 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/transform/test_reductions.py
--rw-rw-rw-   0        0        0     9008 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/transform/test_regex.py
--rw-rw-rw-   0        0        0    13261 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/transform/test_reshape.py
--rw-rw-rw-   0        0        0     9256 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/transform/test_selects.py
--rw-rw-rw-   0        0        0    10534 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/transform/test_setops.py
--rw-rw-rw-   0        0        0    14265 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/transform/test_sorts.py
--rw-rw-rw-   0        0        0     4112 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/transform/test_unpacks.py
--rw-rw-rw-   0        0        0     3649 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/transform/test_validation.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:37.836966 petl_retouched_version-0.1.1/petl/test/util/
--rw-rw-rw-   0        0        0       64 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/util/__init__.py
--rw-rw-rw-   0        0        0     6650 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/util/test_base.py
--rw-rw-rw-   0        0        0     5059 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/util/test_counting.py
--rw-rw-rw-   0        0        0     5732 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/util/test_lookups.py
--rw-rw-rw-   0        0        0      744 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/util/test_materialise.py
--rw-rw-rw-   0        0        0     1139 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/util/test_misc.py
--rw-rw-rw-   0        0        0     1481 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.1/petl/test/util/test_parsers.py
--rw-rw-rw-   0        0        0      627 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.1/petl/test/util/test_statistics.py
--rw-rw-rw-   0        0        0      621 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.1/petl/test/util/test_timing.py
--rw-rw-rw-   0        0        0     3907 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.1/petl/test/util/test_vis.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:38.134171 petl_retouched_version-0.1.1/petl/transform/
--rw-rw-rw-   0        0        0     2523 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.1/petl/transform/__init__.py
--rw-rw-rw-   0        0        0    33801 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.1/petl/transform/basics.py
--rw-rw-rw-   0        0        0    17269 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.1/petl/transform/conversions.py
--rw-rw-rw-   0        0        0    15700 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.1/petl/transform/dedup.py
--rw-rw-rw-   0        0        0     7208 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.1/petl/transform/fills.py
--rw-rw-rw-   0        0        0    15771 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.1/petl/transform/hashjoins.py
--rw-rw-rw-   0        0        0     9624 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.1/petl/transform/headers.py
--rw-rw-rw-   0        0        0    36364 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.1/petl/transform/intervals.py
--rw-rw-rw-   0        0        0    32965 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.1/petl/transform/joins.py
--rw-rw-rw-   0        0        0    13758 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.1/petl/transform/maps.py
--rw-rw-rw-   0        0        0    26510 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.1/petl/transform/reductions.py
--rw-rw-rw-   0        0        0    15856 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/petl/transform/regex.py
--rw-rw-rw-   0        0        0    22804 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/petl/transform/reshape.py
--rw-rw-rw-   0        0        0    15788 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/petl/transform/selects.py
--rw-rw-rw-   0        0        0    16097 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/petl/transform/setops.py
--rw-rw-rw-   0        0        0    18880 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/petl/transform/sorts.py
--rw-rw-rw-   0        0        0     6226 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/petl/transform/unpacks.py
--rw-rw-rw-   0        0        0     7384 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/petl/transform/validation.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:38.296527 petl_retouched_version-0.1.1/petl/util/
--rw-rw-rw-   0        0        0     1083 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/petl/util/__init__.py
--rw-rw-rw-   0        0        0    20876 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/petl/util/base.py
--rw-rw-rw-   0        0        0    14764 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/petl/util/counting.py
--rw-rw-rw-   0        0        0    11605 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/petl/util/lookups.py
--rw-rw-rw-   0        0        0     4019 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/petl/util/materialise.py
--rw-rw-rw-   0        0        0     3471 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/petl/util/misc.py
--rw-rw-rw-   0        0        0     5702 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/petl/util/parsers.py
--rw-rw-rw-   0        0        0     6812 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/petl/util/random.py
--rw-rw-rw-   0        0        0     2613 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/petl/util/statistics.py
--rw-rw-rw-   0        0        0     9933 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/petl/util/timing.py
--rw-rw-rw-   0        0        0    17122 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/petl/util/vis.py
--rw-rw-rw-   0        0        0      193 2023-05-30 15:49:12.000000 petl_retouched_version-0.1.1/petl/version.py
-drwxrwxrwx   0        0        0        0 2023-06-06 13:24:40.601498 petl_retouched_version-0.1.1/petl_retouched_version.egg-info/
--rw-rw-rw-   0        0        0     2309 2023-06-06 13:24:34.000000 petl_retouched_version-0.1.1/petl_retouched_version.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9179 2023-06-06 13:24:35.000000 petl_retouched_version-0.1.1/petl_retouched_version.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 13:24:34.000000 petl_retouched_version-0.1.1/petl_retouched_version.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      393 2023-06-06 13:24:34.000000 petl_retouched_version-0.1.1/petl_retouched_version.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-06 13:24:34.000000 petl_retouched_version-0.1.1/petl_retouched_version.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       70 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      147 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/pytest.ini
--rw-rw-rw-   0        0        0    22767 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/repr_html.ipynb
--rw-rw-rw-   0        0        0      134 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/requirements-database.txt
--rw-rw-rw-   0        0        0       57 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/requirements-docs.txt
--rw-rw-rw-   0        0        0      340 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/requirements-formats.txt
--rw-rw-rw-   0        0        0      412 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/requirements-optional.txt
--rw-rw-rw-   0        0        0      281 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/requirements-remote.txt
--rw-rw-rw-   0        0        0      131 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/requirements-tests.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 13:24:40.625309 petl_retouched_version-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2401 2023-06-06 13:23:39.000000 petl_retouched_version-0.1.1/setup.py
--rw-rw-rw-   0        0        0     2504 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.1/tox.ini
+drwxrwxrwx   0        0        0        0 2023-07-14 11:31:00.539836 petl_retouched_version-0.1.2/
+-rw-rw-rw-   0        0        0       91 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/.coveragerc
+drwxrwxrwx   0        0        0        0 2023-07-14 11:30:58.236945 petl_retouched_version-0.1.2/.github/
+-rw-rw-rw-   0        0        0      170 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/.github/CONTRIBUTING.md
+drwxrwxrwx   0        0        0        0 2023-07-14 11:30:58.271834 petl_retouched_version-0.1.2/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0     1454 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-rw-   0        0        0     1105 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-rw-   0        0        0     1428 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/.github/PULL_REQUEST_TEMPLATE.md
+drwxrwxrwx   0        0        0        0 2023-07-14 11:30:58.360434 petl_retouched_version-0.1.2/.github/workflows/
+-rw-rw-rw-   0        0        0     2314 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/.github/workflows/codacy-analysis.yml
+-rw-rw-rw-   0        0        0     2430 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/.github/workflows/codeql-analysis.yml
+-rw-rw-rw-   0        0        0      889 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/.github/workflows/publish-release.yml
+-rw-rw-rw-   0        0        0     6575 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/.github/workflows/test-changes.yml
+-rw-rw-rw-   0        0        0     3440 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/.gitignore
+drwxrwxrwx   0        0        0        0 2023-07-14 11:30:58.429299 petl_retouched_version-0.1.2/.vscode/
+-rw-rw-rw-   0        0        0      428 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/.vscode/launch.json
+-rw-rw-rw-   0        0        0     4486 2023-05-24 16:48:57.000000 petl_retouched_version-0.1.2/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1383 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/.vscode/tasks.json
+-rw-rw-rw-   0        0        0     1087 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       47 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2309 2023-07-14 11:31:00.526567 petl_retouched_version-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1738 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/README.rst
+-rw-rw-rw-   0        0        0      933 2023-05-27 19:11:07.000000 petl_retouched_version-0.1.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 11:30:58.458791 petl_retouched_version-0.1.2/bin/
+-rw-rw-rw-   0        0        0      761 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/bin/petl
+drwxrwxrwx   0        0        0        0 2023-07-14 11:30:58.825450 petl_retouched_version-0.1.2/docs/
+-rw-rw-rw-   0        0        0     4712 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/docs/Makefile
+-rw-rw-rw-   0        0        0     2836 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/docs/acknowledgments.rst
+-rw-rw-rw-   0        0        0    25474 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/docs/changes.rst
+-rw-rw-rw-   0        0        0     7701 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/docs/conf.py
+-rw-rw-rw-   0        0        0       96 2023-05-23 16:57:36.000000 petl_retouched_version-0.1.2/docs/config.rst
+-rw-rw-rw-   0        0        0     4764 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/docs/contributing.rst
+-rw-rw-rw-   0        0        0     1895 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/docs/index.rst
+-rw-rw-rw-   0        0        0     2572 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/docs/install.rst
+-rw-rw-rw-   0        0        0    13271 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/docs/intro.rst
+-rw-rw-rw-   0        0        0    13307 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/docs/io.rst
+-rwxrwxrwx   0        0        0     4257 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/docs/make.bat
+-rw-rw-rw-   0        0        0   154638 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/docs/petl-architecture.png
+-rw-rw-rw-   0        0        0     9685 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/docs/related_work.rst
+-rw-rw-rw-   0        0        0     9141 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/docs/transform.rst
+-rw-rw-rw-   0        0        0     3149 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/docs/util.rst
+drwxrwxrwx   0        0        0        0 2023-07-14 11:30:58.875730 petl_retouched_version-0.1.2/examples/
+-rw-rw-rw-   0        0        0      368 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/comparison.py
+-rw-rw-rw-   0        0        0      891 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/intro.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:30:59.109107 petl_retouched_version-0.1.2/examples/io/
+-rw-rw-rw-   0        0        0      670 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/io/csv.py
+-rw-rw-rw-   0        0        0      305 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/io/html.py
+-rw-rw-rw-   0        0        0     1018 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/io/json.py
+-rw-rw-rw-   0        0        0      993 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/io/numpy.py
+-rw-rw-rw-   0        0        0      548 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/io/pandas.py
+-rw-rw-rw-   0        0        0      676 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/io/pickle.py
+-rw-rw-rw-   0        0        0     2708 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/io/pytables.py
+-rw-rw-rw-   0        0        0     1005 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/io/sqlite3.py
+-rw-rw-rw-   0        0        0      758 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/io/text.py
+-rw-rw-rw-   0        0        0     2595 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/io/whoosh.py
+-rw-rw-rw-   0        0        0     1465 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/io/xml.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:30:59.472552 petl_retouched_version-0.1.2/examples/notes/
+-rw-rw-rw-   0        0        0       15 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/notes/.gitignore
+-rw-rw-rw-   0        0        0    13376 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/notes/20140424_example.ipynb
+-rw-rw-rw-   0        0        0     1573 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/notes/20140424_example.py
+-rw-rw-rw-   0        0        0     4268 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/notes/20141022_example.ipynb
+-rw-rw-rw-   0        0        0     7825 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/notes/20141110_example.ipynb
+-rw-rw-rw-   0        0        0    11359 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/notes/20150319 resolve conflicts.ipynb
+-rw-rw-rw-   0        0        0     3335 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/notes/20150331 split null.ipynb
+-rw-rw-rw-   0        0        0    55658 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/notes/case_study_1.ipynb
+-rw-rw-rw-   0        0        0    13673 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/notes/issue_219.ipynb
+-rw-rw-rw-   0        0        0     2119 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/notes/issue_219.py
+-rw-rw-rw-   0        0        0     6135 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/notes/issue_256.ipynb
+-rw-rw-rw-   0        0        0      905 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/notes/issue_256.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:30:59.865357 petl_retouched_version-0.1.2/examples/transform/
+-rw-rw-rw-   0        0        0     4542 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/transform/basics.py
+-rw-rw-rw-   0        0        0     1813 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/transform/conversions.py
+-rw-rw-rw-   0        0        0     1392 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/transform/dedup.py
+-rw-rw-rw-   0        0        0     1175 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/transform/fills.py
+-rw-rw-rw-   0        0        0     1191 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/transform/headers.py
+-rw-rw-rw-   0        0        0     3869 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/transform/intervals.py
+-rw-rw-rw-   0        0        0     3677 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/transform/joins.py
+-rw-rw-rw-   0        0        0     2179 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/transform/maps.py
+-rw-rw-rw-   0        0        0     2502 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/transform/reductions.py
+-rw-rw-rw-   0        0        0     1738 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/transform/regex.py
+-rw-rw-rw-   0        0        0     3993 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/transform/reshape.py
+-rw-rw-rw-   0        0        0     1811 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/transform/selects.py
+-rw-rw-rw-   0        0        0     1973 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/transform/setops.py
+-rw-rw-rw-   0        0        0     1169 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/transform/sorts.py
+-rw-rw-rw-   0        0        0      550 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/transform/unpacks.py
+-rw-rw-rw-   0        0        0      929 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/transform/validation.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:31:00.065700 petl_retouched_version-0.1.2/examples/util/
+-rw-rw-rw-   0        0        0     1905 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/util/base.py
+-rw-rw-rw-   0        0        0     2828 2023-05-23 16:57:37.000000 petl_retouched_version-0.1.2/examples/util/counting.py
+-rw-rw-rw-   0        0        0     3972 2023-05-23 16:57:38.000000 petl_retouched_version-0.1.2/examples/util/lookups.py
+-rw-rw-rw-   0        0        0      449 2023-05-23 16:57:38.000000 petl_retouched_version-0.1.2/examples/util/materialise.py
+-rw-rw-rw-   0        0        0     1009 2023-05-23 16:57:38.000000 petl_retouched_version-0.1.2/examples/util/misc.py
+-rw-rw-rw-   0        0        0     1126 2023-05-23 16:57:38.000000 petl_retouched_version-0.1.2/examples/util/parsers.py
+-rw-rw-rw-   0        0        0      607 2023-05-23 16:57:38.000000 petl_retouched_version-0.1.2/examples/util/random.py
+-rw-rw-rw-   0        0        0      475 2023-05-23 16:57:38.000000 petl_retouched_version-0.1.2/examples/util/statistics.py
+-rw-rw-rw-   0        0        0      583 2023-05-23 16:57:38.000000 petl_retouched_version-0.1.2/examples/util/timing.py
+-rw-rw-rw-   0        0        0      590 2023-05-23 16:57:38.000000 petl_retouched_version-0.1.2/examples/util/vis.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:30:55.903707 petl_retouched_version-0.1.2/petl/
+-rw-rw-rw-   0        0        0      415 2023-05-30 14:22:22.000000 petl_retouched_version-0.1.2/petl/__init__.py
+-rw-rw-rw-   0        0        0     3888 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/comparison.py
+-rw-rw-rw-   0        0        0     1802 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/compat.py
+-rw-rw-rw-   0        0        0      793 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/config.py
+-rw-rw-rw-   0        0        0      631 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:30:56.284573 petl_retouched_version-0.1.2/petl/io/
+-rw-rw-rw-   0        0        0     1485 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/__init__.py
+-rw-rw-rw-   0        0        0    20835 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/avro.py
+-rw-rw-rw-   0        0        0     1946 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/base.py
+-rw-rw-rw-   0        0        0     6282 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/bcolz.py
+-rw-rw-rw-   0        0        0     6258 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/csv.py
+-rw-rw-rw-   0        0        0     5433 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/csv_py2.py
+-rw-rw-rw-   0        0        0     2995 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/csv_py3.py
+-rw-rw-rw-   0        0        0    30463 2023-07-14 11:11:56.000000 petl_retouched_version-0.1.2/petl/io/db.py
+-rw-rw-rw-   0        0        0    11440 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/db_create.py
+-rw-rw-rw-   0        0        0     3117 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/db_utils.py
+-rw-rw-rw-   0        0        0     8266 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/gsheet.py
+-rw-rw-rw-   0        0        0     8683 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/html.py
+-rw-rw-rw-   0        0        0    14004 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/json.py
+-rw-rw-rw-   0        0        0     5434 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/numpy.py
+-rw-rw-rw-   0        0        0     2689 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/pandas.py
+-rw-rw-rw-   0        0        0     4547 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/pickle.py
+-rw-rw-rw-   0        0        0    12977 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/pytables.py
+-rw-rw-rw-   0        0        0     8731 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/remotes.py
+-rw-rw-rw-   0        0        0    13121 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/sources.py
+-rw-rw-rw-   0        0        0     8278 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/text.py
+-rw-rw-rw-   0        0        0    17839 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/whoosh.py
+-rw-rw-rw-   0        0        0     3541 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/xls.py
+-rw-rw-rw-   0        0        0     6914 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/xlsx.py
+-rw-rw-rw-   0        0        0     4545 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/xlutils_view.py
+-rw-rw-rw-   0        0        0    16130 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/io/xml.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:30:56.388031 petl_retouched_version-0.1.2/petl/test/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/__init__.py
+-rw-rw-rw-   0        0        0      205 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/conftest.py
+-rw-rw-rw-   0        0        0     3685 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/failonerror.py
+-rw-rw-rw-   0        0        0     2569 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:30:56.981504 petl_retouched_version-0.1.2/petl/test/io/
+-rw-rw-rw-   0        0        0       66 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/__init__.py
+-rw-rw-rw-   0        0        0    11773 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_avro.py
+-rw-rw-rw-   0        0        0     6373 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_avro_schemas.py
+-rw-rw-rw-   0        0        0     2198 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_bcolz.py
+-rw-rw-rw-   0        0        0     7929 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_csv.py
+-rw-rw-rw-   0        0        0     4334 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_csv_unicode.py
+-rw-rw-rw-   0        0        0     6855 2023-05-27 19:17:16.000000 petl_retouched_version-0.1.2/petl/test/io/test_db.py
+-rw-rw-rw-   0        0        0     7980 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_db_create.py
+-rw-rw-rw-   0        0        0    11239 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_db_server.py
+-rw-rw-rw-   0        0        0     8878 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_gsheet.py
+-rw-rw-rw-   0        0        0     3296 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_html.py
+-rw-rw-rw-   0        0        0     1499 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_html_unicode.py
+-rw-rw-rw-   0        0        0     8129 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_json.py
+-rw-rw-rw-   0        0        0      775 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_json_unicode.py
+-rw-rw-rw-   0        0        0     3043 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_jsonl.py
+-rw-rw-rw-   0        0        0     6186 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_numpy.py
+-rw-rw-rw-   0        0        0     1348 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_pandas.py
+-rw-rw-rw-   0        0        0     1635 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_pickle.py
+-rw-rw-rw-   0        0        0     7076 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_pytables.py
+-rw-rw-rw-   0        0        0     6383 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_remotes.py
+-rw-rw-rw-   0        0        0     4186 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_sources.py
+-rw-rw-rw-   0        0        0     4999 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_sqlite3.py
+-rw-rw-rw-   0        0        0     6686 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_tees.py
+-rw-rw-rw-   0        0        0     3985 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_text.py
+-rw-rw-rw-   0        0        0     2126 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_text_unicode.py
+-rw-rw-rw-   0        0        0     8598 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_whoosh.py
+-rw-rw-rw-   0        0        0     3880 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_xls.py
+-rw-rw-rw-   0        0        0     6710 2023-05-23 16:57:40.000000 petl_retouched_version-0.1.2/petl/test/io/test_xlsx.py
+-rw-rw-rw-   0        0        0    15051 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/io/test_xml.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:31:00.312898 petl_retouched_version-0.1.2/petl/test/resources/
+-rw-rw-rw-   0        0        0    21504 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/resources/test.xls
+-rw-rw-rw-   0        0        0     9596 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/resources/test.xlsx
+-rw-rw-rw-   0        0        0      424 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/resources/test.xml
+-rw-rw-rw-   0        0        0     4837 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/test_comparison.py
+-rw-rw-rw-   0        0        0     3093 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/test_fluent.py
+-rw-rw-rw-   0        0        0     1294 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/test_helpers.py
+-rw-rw-rw-   0        0        0     1780 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/test_interactive.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:30:57.368951 petl_retouched_version-0.1.2/petl/test/transform/
+-rw-rw-rw-   0        0        0       66 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/transform/__init__.py
+-rw-rw-rw-   0        0        0    20074 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/transform/test_basics.py
+-rw-rw-rw-   0        0        0    11234 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/transform/test_conversions.py
+-rw-rw-rw-   0        0        0     7317 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/transform/test_dedup.py
+-rw-rw-rw-   0        0        0     2695 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/transform/test_fills.py
+-rw-rw-rw-   0        0        0     7236 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/transform/test_headers.py
+-rw-rw-rw-   0        0        0    33773 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/transform/test_intervals.py
+-rw-rw-rw-   0        0        0    44856 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/transform/test_joins.py
+-rw-rw-rw-   0        0        0    11199 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/transform/test_maps.py
+-rw-rw-rw-   0        0        0    15028 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/transform/test_reductions.py
+-rw-rw-rw-   0        0        0     9008 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/transform/test_regex.py
+-rw-rw-rw-   0        0        0    13261 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/transform/test_reshape.py
+-rw-rw-rw-   0        0        0     9256 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/transform/test_selects.py
+-rw-rw-rw-   0        0        0    10534 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/transform/test_setops.py
+-rw-rw-rw-   0        0        0    14265 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/transform/test_sorts.py
+-rw-rw-rw-   0        0        0     4112 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/transform/test_unpacks.py
+-rw-rw-rw-   0        0        0     3649 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/transform/test_validation.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:30:57.607314 petl_retouched_version-0.1.2/petl/test/util/
+-rw-rw-rw-   0        0        0       64 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/util/__init__.py
+-rw-rw-rw-   0        0        0     6650 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/util/test_base.py
+-rw-rw-rw-   0        0        0     5059 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/util/test_counting.py
+-rw-rw-rw-   0        0        0     5732 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/util/test_lookups.py
+-rw-rw-rw-   0        0        0      744 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/util/test_materialise.py
+-rw-rw-rw-   0        0        0     1139 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/util/test_misc.py
+-rw-rw-rw-   0        0        0     1481 2023-05-23 16:57:41.000000 petl_retouched_version-0.1.2/petl/test/util/test_parsers.py
+-rw-rw-rw-   0        0        0      627 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.2/petl/test/util/test_statistics.py
+-rw-rw-rw-   0        0        0      621 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.2/petl/test/util/test_timing.py
+-rw-rw-rw-   0        0        0     3907 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.2/petl/test/util/test_vis.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:30:58.017176 petl_retouched_version-0.1.2/petl/transform/
+-rw-rw-rw-   0        0        0     2523 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.2/petl/transform/__init__.py
+-rw-rw-rw-   0        0        0    33801 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.2/petl/transform/basics.py
+-rw-rw-rw-   0        0        0    17269 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.2/petl/transform/conversions.py
+-rw-rw-rw-   0        0        0    15700 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.2/petl/transform/dedup.py
+-rw-rw-rw-   0        0        0     7208 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.2/petl/transform/fills.py
+-rw-rw-rw-   0        0        0    15771 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.2/petl/transform/hashjoins.py
+-rw-rw-rw-   0        0        0     9624 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.2/petl/transform/headers.py
+-rw-rw-rw-   0        0        0    36364 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.2/petl/transform/intervals.py
+-rw-rw-rw-   0        0        0    32965 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.2/petl/transform/joins.py
+-rw-rw-rw-   0        0        0    13758 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.2/petl/transform/maps.py
+-rw-rw-rw-   0        0        0    26510 2023-05-23 16:57:42.000000 petl_retouched_version-0.1.2/petl/transform/reductions.py
+-rw-rw-rw-   0        0        0    15856 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/petl/transform/regex.py
+-rw-rw-rw-   0        0        0    22804 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/petl/transform/reshape.py
+-rw-rw-rw-   0        0        0    15788 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/petl/transform/selects.py
+-rw-rw-rw-   0        0        0    16097 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/petl/transform/setops.py
+-rw-rw-rw-   0        0        0    18880 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/petl/transform/sorts.py
+-rw-rw-rw-   0        0        0     6226 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/petl/transform/unpacks.py
+-rw-rw-rw-   0        0        0     7384 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/petl/transform/validation.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:30:58.190582 petl_retouched_version-0.1.2/petl/util/
+-rw-rw-rw-   0        0        0     1083 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/petl/util/__init__.py
+-rw-rw-rw-   0        0        0    20876 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/petl/util/base.py
+-rw-rw-rw-   0        0        0    14764 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/petl/util/counting.py
+-rw-rw-rw-   0        0        0    11605 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/petl/util/lookups.py
+-rw-rw-rw-   0        0        0     4019 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/petl/util/materialise.py
+-rw-rw-rw-   0        0        0     3471 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/petl/util/misc.py
+-rw-rw-rw-   0        0        0     5702 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/petl/util/parsers.py
+-rw-rw-rw-   0        0        0     6812 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/petl/util/random.py
+-rw-rw-rw-   0        0        0     2613 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/petl/util/statistics.py
+-rw-rw-rw-   0        0        0     9933 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/petl/util/timing.py
+-rw-rw-rw-   0        0        0    17122 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/petl/util/vis.py
+-rw-rw-rw-   0        0        0      193 2023-05-30 15:49:12.000000 petl_retouched_version-0.1.2/petl/version.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:31:00.505955 petl_retouched_version-0.1.2/petl_retouched_version.egg-info/
+-rw-rw-rw-   0        0        0     2309 2023-07-14 11:30:54.000000 petl_retouched_version-0.1.2/petl_retouched_version.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9179 2023-07-14 11:30:55.000000 petl_retouched_version-0.1.2/petl_retouched_version.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 11:30:54.000000 petl_retouched_version-0.1.2/petl_retouched_version.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      393 2023-07-14 11:30:54.000000 petl_retouched_version-0.1.2/petl_retouched_version.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-14 11:30:54.000000 petl_retouched_version-0.1.2/petl_retouched_version.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       70 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      147 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/pytest.ini
+-rw-rw-rw-   0        0        0    22767 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/repr_html.ipynb
+-rw-rw-rw-   0        0        0      134 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/requirements-database.txt
+-rw-rw-rw-   0        0        0       57 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/requirements-docs.txt
+-rw-rw-rw-   0        0        0      340 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/requirements-formats.txt
+-rw-rw-rw-   0        0        0      412 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/requirements-optional.txt
+-rw-rw-rw-   0        0        0      281 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/requirements-remote.txt
+-rw-rw-rw-   0        0        0      131 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/requirements-tests.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 11:31:00.540835 petl_retouched_version-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2401 2023-07-14 11:14:53.000000 petl_retouched_version-0.1.2/setup.py
+-rw-rw-rw-   0        0        0     2504 2023-05-23 16:57:43.000000 petl_retouched_version-0.1.2/tox.ini
```

### Comparing `petl_retouched_version-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `petl_retouched_version-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md` & `petl_retouched_version-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/.github/PULL_REQUEST_TEMPLATE.md` & `petl_retouched_version-0.1.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/.github/workflows/codacy-analysis.yml` & `petl_retouched_version-0.1.2/.github/workflows/codacy-analysis.yml`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/.github/workflows/codeql-analysis.yml` & `petl_retouched_version-0.1.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/.github/workflows/publish-release.yml` & `petl_retouched_version-0.1.2/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/.github/workflows/test-changes.yml` & `petl_retouched_version-0.1.2/.github/workflows/test-changes.yml`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/.gitignore` & `petl_retouched_version-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/.vscode/settings.json` & `petl_retouched_version-0.1.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/.vscode/tasks.json` & `petl_retouched_version-0.1.2/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/LICENSE.txt` & `petl_retouched_version-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/PKG-INFO` & `petl_retouched_version-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petl_retouched_version
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for extracting, transforming and loading tables of data. Modified from Original Petl Lib
 Author: Alistair Miles
 Author-email: alimanfoo@googlemail.com
 Maintainer: Winston David
 Maintainer-email: winstondavid96@gmail.com
 License: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `petl_retouched_version-0.1.1/README.rst` & `petl_retouched_version-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/README.txt` & `petl_retouched_version-0.1.2/README.txt`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/bin/petl` & `petl_retouched_version-0.1.2/bin/petl`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/docs/Makefile` & `petl_retouched_version-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/docs/acknowledgments.rst` & `petl_retouched_version-0.1.2/docs/acknowledgments.rst`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/docs/changes.rst` & `petl_retouched_version-0.1.2/docs/changes.rst`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/docs/conf.py` & `petl_retouched_version-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/docs/contributing.rst` & `petl_retouched_version-0.1.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/docs/index.rst` & `petl_retouched_version-0.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/docs/install.rst` & `petl_retouched_version-0.1.2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/docs/intro.rst` & `petl_retouched_version-0.1.2/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/docs/io.rst` & `petl_retouched_version-0.1.2/docs/io.rst`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/docs/make.bat` & `petl_retouched_version-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/docs/petl-architecture.png` & `petl_retouched_version-0.1.2/docs/petl-architecture.png`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/docs/related_work.rst` & `petl_retouched_version-0.1.2/docs/related_work.rst`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/docs/transform.rst` & `petl_retouched_version-0.1.2/docs/transform.rst`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/docs/util.rst` & `petl_retouched_version-0.1.2/docs/util.rst`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/intro.py` & `petl_retouched_version-0.1.2/examples/intro.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/io/csv.py` & `petl_retouched_version-0.1.2/examples/io/csv.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/io/json.py` & `petl_retouched_version-0.1.2/examples/io/json.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/io/numpy.py` & `petl_retouched_version-0.1.2/examples/io/numpy.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/io/pandas.py` & `petl_retouched_version-0.1.2/examples/io/pandas.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/io/pickle.py` & `petl_retouched_version-0.1.2/examples/io/pickle.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/io/pytables.py` & `petl_retouched_version-0.1.2/examples/io/pytables.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/io/sqlite3.py` & `petl_retouched_version-0.1.2/examples/io/sqlite3.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/io/text.py` & `petl_retouched_version-0.1.2/examples/io/text.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/io/whoosh.py` & `petl_retouched_version-0.1.2/examples/io/whoosh.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/io/xml.py` & `petl_retouched_version-0.1.2/examples/io/xml.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/notes/20140424_example.ipynb` & `petl_retouched_version-0.1.2/examples/notes/20140424_example.ipynb`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/notes/20140424_example.py` & `petl_retouched_version-0.1.2/examples/notes/20140424_example.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/notes/20141022_example.ipynb` & `petl_retouched_version-0.1.2/examples/notes/20141022_example.ipynb`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/notes/20141110_example.ipynb` & `petl_retouched_version-0.1.2/examples/notes/20141110_example.ipynb`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/notes/20150319 resolve conflicts.ipynb` & `petl_retouched_version-0.1.2/examples/notes/20150319 resolve conflicts.ipynb`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/notes/20150331 split null.ipynb` & `petl_retouched_version-0.1.2/examples/notes/20150331 split null.ipynb`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/notes/case_study_1.ipynb` & `petl_retouched_version-0.1.2/examples/notes/case_study_1.ipynb`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/notes/issue_219.ipynb` & `petl_retouched_version-0.1.2/examples/notes/issue_219.ipynb`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/notes/issue_219.py` & `petl_retouched_version-0.1.2/examples/notes/issue_219.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/notes/issue_256.ipynb` & `petl_retouched_version-0.1.2/examples/notes/issue_256.ipynb`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/notes/issue_256.py` & `petl_retouched_version-0.1.2/examples/notes/issue_256.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/transform/basics.py` & `petl_retouched_version-0.1.2/examples/transform/basics.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/transform/conversions.py` & `petl_retouched_version-0.1.2/examples/transform/conversions.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/transform/dedup.py` & `petl_retouched_version-0.1.2/examples/transform/dedup.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/transform/fills.py` & `petl_retouched_version-0.1.2/examples/transform/fills.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/transform/headers.py` & `petl_retouched_version-0.1.2/examples/transform/headers.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/transform/intervals.py` & `petl_retouched_version-0.1.2/examples/transform/intervals.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/transform/joins.py` & `petl_retouched_version-0.1.2/examples/transform/joins.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/transform/maps.py` & `petl_retouched_version-0.1.2/examples/transform/maps.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/transform/reductions.py` & `petl_retouched_version-0.1.2/examples/transform/reductions.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/transform/regex.py` & `petl_retouched_version-0.1.2/examples/transform/regex.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/transform/reshape.py` & `petl_retouched_version-0.1.2/examples/transform/reshape.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/transform/selects.py` & `petl_retouched_version-0.1.2/examples/transform/selects.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/transform/setops.py` & `petl_retouched_version-0.1.2/examples/transform/setops.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/transform/sorts.py` & `petl_retouched_version-0.1.2/examples/transform/sorts.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/transform/unpacks.py` & `petl_retouched_version-0.1.2/examples/transform/unpacks.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/transform/validation.py` & `petl_retouched_version-0.1.2/examples/transform/validation.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/util/base.py` & `petl_retouched_version-0.1.2/examples/util/base.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/util/counting.py` & `petl_retouched_version-0.1.2/examples/util/counting.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/util/lookups.py` & `petl_retouched_version-0.1.2/examples/util/lookups.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/util/misc.py` & `petl_retouched_version-0.1.2/examples/util/misc.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/util/parsers.py` & `petl_retouched_version-0.1.2/examples/util/parsers.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/util/random.py` & `petl_retouched_version-0.1.2/examples/util/random.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/util/timing.py` & `petl_retouched_version-0.1.2/examples/util/timing.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/examples/util/vis.py` & `petl_retouched_version-0.1.2/examples/util/vis.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/comparison.py` & `petl_retouched_version-0.1.2/petl/comparison.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/compat.py` & `petl_retouched_version-0.1.2/petl/compat.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/config.py` & `petl_retouched_version-0.1.2/petl/config.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/errors.py` & `petl_retouched_version-0.1.2/petl/errors.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/__init__.py` & `petl_retouched_version-0.1.2/petl/io/__init__.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/avro.py` & `petl_retouched_version-0.1.2/petl/io/avro.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/base.py` & `petl_retouched_version-0.1.2/petl/io/base.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/bcolz.py` & `petl_retouched_version-0.1.2/petl/io/bcolz.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/csv.py` & `petl_retouched_version-0.1.2/petl/io/csv.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/csv_py2.py` & `petl_retouched_version-0.1.2/petl/io/csv_py2.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/csv_py3.py` & `petl_retouched_version-0.1.2/petl/io/csv_py3.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/db.py` & `petl_retouched_version-0.1.2/petl/io/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 def clean_csv_value(value: Optional[Any]) -> str:
     # print(value)
     if value is None:
         # return r'\N' 
         return 'NULL'
     cleaned_value = str(value).replace('\n', '\\n')
     cleaned_value = cleaned_value.replace('\r', '\\r')
-    cleaned_value = re.sub(r'[^A-Za-z0-9\- .:+]', '', cleaned_value)
+    cleaned_value = re.sub(r'[^A-Za-z0-9\- .:+,]', '', cleaned_value)
     # print(value)
     return cleaned_value
 
 
 class StringIteratorIO(stdlib_io.TextIOBase):
 
     def __init__(self, iterator: Iterator[str]):
```

### Comparing `petl_retouched_version-0.1.1/petl/io/db_create.py` & `petl_retouched_version-0.1.2/petl/io/db_create.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/db_utils.py` & `petl_retouched_version-0.1.2/petl/io/db_utils.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/gsheet.py` & `petl_retouched_version-0.1.2/petl/io/gsheet.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/html.py` & `petl_retouched_version-0.1.2/petl/io/html.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/json.py` & `petl_retouched_version-0.1.2/petl/io/json.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/numpy.py` & `petl_retouched_version-0.1.2/petl/io/numpy.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/pandas.py` & `petl_retouched_version-0.1.2/petl/io/pandas.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/pickle.py` & `petl_retouched_version-0.1.2/petl/io/pickle.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/pytables.py` & `petl_retouched_version-0.1.2/petl/io/pytables.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/remotes.py` & `petl_retouched_version-0.1.2/petl/io/remotes.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/sources.py` & `petl_retouched_version-0.1.2/petl/io/sources.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/text.py` & `petl_retouched_version-0.1.2/petl/io/text.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/whoosh.py` & `petl_retouched_version-0.1.2/petl/io/whoosh.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/xls.py` & `petl_retouched_version-0.1.2/petl/io/xls.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/xlsx.py` & `petl_retouched_version-0.1.2/petl/io/xlsx.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/xlutils_view.py` & `petl_retouched_version-0.1.2/petl/io/xlutils_view.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/io/xml.py` & `petl_retouched_version-0.1.2/petl/io/xml.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/failonerror.py` & `petl_retouched_version-0.1.2/petl/test/failonerror.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/helpers.py` & `petl_retouched_version-0.1.2/petl/test/helpers.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_avro.py` & `petl_retouched_version-0.1.2/petl/test/io/test_avro.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_avro_schemas.py` & `petl_retouched_version-0.1.2/petl/test/io/test_avro_schemas.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_bcolz.py` & `petl_retouched_version-0.1.2/petl/test/io/test_bcolz.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_csv.py` & `petl_retouched_version-0.1.2/petl/test/io/test_csv.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_csv_unicode.py` & `petl_retouched_version-0.1.2/petl/test/io/test_csv_unicode.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_db.py` & `petl_retouched_version-0.1.2/petl/test/io/test_db.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_db_create.py` & `petl_retouched_version-0.1.2/petl/test/io/test_db_create.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_db_server.py` & `petl_retouched_version-0.1.2/petl/test/io/test_db_server.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_gsheet.py` & `petl_retouched_version-0.1.2/petl/test/io/test_gsheet.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_html.py` & `petl_retouched_version-0.1.2/petl/test/io/test_html.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_html_unicode.py` & `petl_retouched_version-0.1.2/petl/test/io/test_html_unicode.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_json.py` & `petl_retouched_version-0.1.2/petl/test/io/test_json.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_json_unicode.py` & `petl_retouched_version-0.1.2/petl/test/io/test_json_unicode.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_jsonl.py` & `petl_retouched_version-0.1.2/petl/test/io/test_jsonl.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_numpy.py` & `petl_retouched_version-0.1.2/petl/test/io/test_numpy.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_pandas.py` & `petl_retouched_version-0.1.2/petl/test/io/test_pandas.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_pickle.py` & `petl_retouched_version-0.1.2/petl/test/io/test_pickle.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_pytables.py` & `petl_retouched_version-0.1.2/petl/test/io/test_pytables.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_remotes.py` & `petl_retouched_version-0.1.2/petl/test/io/test_remotes.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_sources.py` & `petl_retouched_version-0.1.2/petl/test/io/test_sources.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_sqlite3.py` & `petl_retouched_version-0.1.2/petl/test/io/test_sqlite3.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_tees.py` & `petl_retouched_version-0.1.2/petl/test/io/test_tees.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_text.py` & `petl_retouched_version-0.1.2/petl/test/io/test_text.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_text_unicode.py` & `petl_retouched_version-0.1.2/petl/test/io/test_text_unicode.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_whoosh.py` & `petl_retouched_version-0.1.2/petl/test/io/test_whoosh.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_xls.py` & `petl_retouched_version-0.1.2/petl/test/io/test_xls.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_xlsx.py` & `petl_retouched_version-0.1.2/petl/test/io/test_xlsx.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/io/test_xml.py` & `petl_retouched_version-0.1.2/petl/test/io/test_xml.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/resources/test.xls` & `petl_retouched_version-0.1.2/petl/test/resources/test.xls`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/resources/test.xlsx` & `petl_retouched_version-0.1.2/petl/test/resources/test.xlsx`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/test_comparison.py` & `petl_retouched_version-0.1.2/petl/test/test_comparison.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/test_fluent.py` & `petl_retouched_version-0.1.2/petl/test/test_fluent.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/test_helpers.py` & `petl_retouched_version-0.1.2/petl/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/test_interactive.py` & `petl_retouched_version-0.1.2/petl/test/test_interactive.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/transform/test_basics.py` & `petl_retouched_version-0.1.2/petl/test/transform/test_basics.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/transform/test_conversions.py` & `petl_retouched_version-0.1.2/petl/test/transform/test_conversions.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/transform/test_dedup.py` & `petl_retouched_version-0.1.2/petl/test/transform/test_dedup.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/transform/test_fills.py` & `petl_retouched_version-0.1.2/petl/test/transform/test_fills.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/transform/test_headers.py` & `petl_retouched_version-0.1.2/petl/test/transform/test_headers.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/transform/test_intervals.py` & `petl_retouched_version-0.1.2/petl/test/transform/test_intervals.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/transform/test_joins.py` & `petl_retouched_version-0.1.2/petl/test/transform/test_joins.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/transform/test_maps.py` & `petl_retouched_version-0.1.2/petl/test/transform/test_maps.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/transform/test_reductions.py` & `petl_retouched_version-0.1.2/petl/test/transform/test_reductions.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/transform/test_regex.py` & `petl_retouched_version-0.1.2/petl/test/transform/test_regex.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/transform/test_reshape.py` & `petl_retouched_version-0.1.2/petl/test/transform/test_reshape.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/transform/test_selects.py` & `petl_retouched_version-0.1.2/petl/test/transform/test_selects.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/transform/test_setops.py` & `petl_retouched_version-0.1.2/petl/test/transform/test_setops.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/transform/test_sorts.py` & `petl_retouched_version-0.1.2/petl/test/transform/test_sorts.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/transform/test_unpacks.py` & `petl_retouched_version-0.1.2/petl/test/transform/test_unpacks.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/transform/test_validation.py` & `petl_retouched_version-0.1.2/petl/test/transform/test_validation.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/util/test_base.py` & `petl_retouched_version-0.1.2/petl/test/util/test_base.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/util/test_counting.py` & `petl_retouched_version-0.1.2/petl/test/util/test_counting.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/util/test_lookups.py` & `petl_retouched_version-0.1.2/petl/test/util/test_lookups.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/util/test_materialise.py` & `petl_retouched_version-0.1.2/petl/test/util/test_materialise.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/util/test_misc.py` & `petl_retouched_version-0.1.2/petl/test/util/test_misc.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/util/test_parsers.py` & `petl_retouched_version-0.1.2/petl/test/util/test_parsers.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/util/test_statistics.py` & `petl_retouched_version-0.1.2/petl/test/util/test_statistics.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/util/test_timing.py` & `petl_retouched_version-0.1.2/petl/test/util/test_timing.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/test/util/test_vis.py` & `petl_retouched_version-0.1.2/petl/test/util/test_vis.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/transform/__init__.py` & `petl_retouched_version-0.1.2/petl/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/transform/basics.py` & `petl_retouched_version-0.1.2/petl/transform/basics.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/transform/conversions.py` & `petl_retouched_version-0.1.2/petl/transform/conversions.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/transform/dedup.py` & `petl_retouched_version-0.1.2/petl/transform/dedup.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/transform/fills.py` & `petl_retouched_version-0.1.2/petl/transform/fills.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/transform/hashjoins.py` & `petl_retouched_version-0.1.2/petl/transform/hashjoins.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/transform/headers.py` & `petl_retouched_version-0.1.2/petl/transform/headers.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/transform/intervals.py` & `petl_retouched_version-0.1.2/petl/transform/intervals.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/transform/joins.py` & `petl_retouched_version-0.1.2/petl/transform/joins.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/transform/maps.py` & `petl_retouched_version-0.1.2/petl/transform/maps.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/transform/reductions.py` & `petl_retouched_version-0.1.2/petl/transform/reductions.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/transform/regex.py` & `petl_retouched_version-0.1.2/petl/transform/regex.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/transform/reshape.py` & `petl_retouched_version-0.1.2/petl/transform/reshape.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/transform/selects.py` & `petl_retouched_version-0.1.2/petl/transform/selects.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/transform/setops.py` & `petl_retouched_version-0.1.2/petl/transform/setops.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/transform/sorts.py` & `petl_retouched_version-0.1.2/petl/transform/sorts.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/transform/unpacks.py` & `petl_retouched_version-0.1.2/petl/transform/unpacks.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/transform/validation.py` & `petl_retouched_version-0.1.2/petl/transform/validation.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/util/__init__.py` & `petl_retouched_version-0.1.2/petl/util/__init__.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/util/base.py` & `petl_retouched_version-0.1.2/petl/util/base.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/util/counting.py` & `petl_retouched_version-0.1.2/petl/util/counting.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/util/lookups.py` & `petl_retouched_version-0.1.2/petl/util/lookups.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/util/materialise.py` & `petl_retouched_version-0.1.2/petl/util/materialise.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/util/misc.py` & `petl_retouched_version-0.1.2/petl/util/misc.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/util/parsers.py` & `petl_retouched_version-0.1.2/petl/util/parsers.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/util/random.py` & `petl_retouched_version-0.1.2/petl/util/random.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/util/statistics.py` & `petl_retouched_version-0.1.2/petl/util/statistics.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/util/timing.py` & `petl_retouched_version-0.1.2/petl/util/timing.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl/util/vis.py` & `petl_retouched_version-0.1.2/petl/util/vis.py`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/petl_retouched_version.egg-info/PKG-INFO` & `petl_retouched_version-0.1.2/petl_retouched_version.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petl-retouched-version
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for extracting, transforming and loading tables of data. Modified from Original Petl Lib
 Author: Alistair Miles
 Author-email: alimanfoo@googlemail.com
 Maintainer: Winston David
 Maintainer-email: winstondavid96@gmail.com
 License: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `petl_retouched_version-0.1.1/petl_retouched_version.egg-info/SOURCES.txt` & `petl_retouched_version-0.1.2/petl_retouched_version.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/repr_html.ipynb` & `petl_retouched_version-0.1.2/repr_html.ipynb`

 * *Files identical despite different names*

### Comparing `petl_retouched_version-0.1.1/setup.py` & `petl_retouched_version-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         'whoosh': ['whoosh'],
     },
     # use_scm_version={
     #     "version_scheme": "guess-next-dev",
     #     "local_scheme": "dirty-tag",
     #     "write_to": "petl/version.py",
     # },
-    version= '0.1.1',
+    version= '0.1.2',
     classifiers=['Intended Audience :: Developers',
                  'License :: OSI Approved :: MIT License',
                  'Programming Language :: Python :: 2',
                  'Programming Language :: Python :: 2.7',
                  'Programming Language :: Python :: 3',
                  'Programming Language :: Python :: 3.6',
                  'Programming Language :: Python :: 3.7',
```

### Comparing `petl_retouched_version-0.1.1/tox.ini` & `petl_retouched_version-0.1.2/tox.ini`

 * *Files identical despite different names*

