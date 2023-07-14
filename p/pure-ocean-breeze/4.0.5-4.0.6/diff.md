# Comparing `tmp/pure_ocean_breeze-4.0.5.tar.gz` & `tmp/pure_ocean_breeze-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_ocean_breeze-4.0.5.tar", last modified: Fri Jul  7 02:35:15 2023, max compression
+gzip compressed data, was "pure_ocean_breeze-4.0.6.tar", last modified: Fri Jul 14 07:14:28 2023, max compression
```

## Comparing `pure_ocean_breeze-4.0.5.tar` & `pure_ocean_breeze-4.0.6.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.221577 pure_ocean_breeze-4.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-07 02:35:15.221577 pure_ocean_breeze-4.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.181577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.185577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31919 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    34891 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    66719 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    53733 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.185577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.189577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.189577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   268539 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.189577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.193577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.193577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1p10/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1p10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1p10/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.193577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v2/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.197577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.197577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.201577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.201577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.201577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.201577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.205577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.205577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.205577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.209577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.213577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.213577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.213577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.217577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/mail/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.217577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/state/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.217577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.217577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.221577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.221577 pure_ocean_breeze-4.0.5/pure_ocean_breeze/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:35:15.181577 pure_ocean_breeze-4.0.5/pure_ocean_breeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-07 02:35:15.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-07 02:35:15.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 02:35:15.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-07 02:35:15.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 02:35:15.000000 pure_ocean_breeze-4.0.5/pure_ocean_breeze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 02:35:15.221577 pure_ocean_breeze-4.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-07 02:35:02.000000 pure_ocean_breeze-4.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.041613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.041613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31919 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34891 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66752 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53733 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.041613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.045613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.045613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   268911 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.045613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.045613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.045613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1p10/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1p10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1p10/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.045613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v2/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.045613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.049613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.049613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.049613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.049613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.049613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.049613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.049613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.049613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.049613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.049613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/pure_ocean_breeze/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:14:28.041613 pure_ocean_breeze-4.0.6/pure_ocean_breeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-14 07:14:28.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-14 07:14:28.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 07:14:28.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-14 07:14:28.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 07:14:28.000000 pure_ocean_breeze-4.0.6/pure_ocean_breeze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 07:14:28.053613 pure_ocean_breeze-4.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-14 07:14:15.000000 pure_ocean_breeze-4.0.6/setup.py
```

### Comparing `pure_ocean_breeze-4.0.5/LICENSE` & `pure_ocean_breeze-4.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/PKG-INFO` & `pure_ocean_breeze-4.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure_ocean_breeze
-Version: 4.0.5
+Version: 4.0.6
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-4.0.5/README.md` & `pure_ocean_breeze-4.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/__init__.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 一个量化多因子研究的框架，包含数据、回测、因子加工等方面的功能
 """
 
-__updated__ = "2023-07-04 16:16:50"
-__version__ = "4.0.5"
+__updated__ = "2023-07-13 08:36:22"
+__version__ = "4.0.6"
 __author__ = "chenzongwei"
 __author_email__ = "winterwinter999@163.com"
 __url__ = "https://github.com/chen-001/pure_ocean_breeze"
 __all__ = [
     "data",
     "labor",
     "state",
```

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/database.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/dicts.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/read_data.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/tools.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 针对一些不常见的文件格式，读取数据文件的一些工具函数，以及其他数据工具
 """
 
-__updated__ = "2023-07-07 10:32:50"
+__updated__ = "2023-07-10 12:46:10"
 
 import os
 import pandas as pd
 import tqdm.auto
 import datetime
 import scipy.io as scio
 import numpy as np
@@ -533,14 +533,15 @@
         res = []
         if history_file is not None:
             if os.path.exists(homeplace.update_data_file + history_file):
                 old = pd.read_parquet(homeplace.update_data_file + history_file)
                 old_date = old.index.max()
                 if old_date == self.fac.date.max():
                     logger.info(f"本地文件已经是最新的了，无需计算")
+                    self.fac=old
                 else:
                     try:
                         new_date = self.find_begin(
                             self.tradedays, old_date, self.backsee
                         )
                         fac = self.fac[self.fac.date > new_date]
                         iter_item = [i for i in iter_item if i > new_date]
```

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/data/write_data.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/data/write_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-07-02 02:35:59"
+__updated__ = "2023-07-14 15:11:40"
 
 import time
 
 try:
     import rqdatac
 
     rqdatac.init()
```

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/future_version/half_way.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/initialize/initialize.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/labor/comment.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/labor/process.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/labor/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-07-07 10:21:18"
+__updated__ = "2023-07-13 12:17:42"
 
 import warnings
 
 warnings.filterwarnings("ignore")
 import numpy as np
 import pandas as pd
 import knockknock as kk
@@ -3413,15 +3413,20 @@
                 return df
 
             if n_jobs > 1:
                 with concurrent.futures.ThreadPoolExecutor(
                     max_workers=n_jobs
                 ) as executor:
                     factor_new_more = list(
-                        tqdm.auto.tqdm(executor.map(cal_one, cuts), total=len(cuts))
+                        tqdm.auto.tqdm(
+                            executor.map(
+                                cal_one, cut_points[:-many_days], cut_points[many_days:]
+                            ),
+                            total=len(cut_points[many_days:]),
+                        )
                     )
                 factor_new = factor_new + factor_new_more
             else:
                 # 开始计算因子值
                 for date1, date2 in tqdm.auto.tqdm(cuts, desc="不知乘月几人归，落月摇情满江树。"):
                     df = cal_one(date1, date2)
                     factor_new.append(df)
@@ -3464,15 +3469,20 @@
             pairs = self.forward_dates(dates, many_days=many_days)
             cuts2 = tuple(zip(pairs, dates))
             if n_jobs > 1:
                 with concurrent.futures.ThreadPoolExecutor(
                     max_workers=n_jobs
                 ) as executor:
                     factor_new_more = list(
-                        tqdm.auto.tqdm(executor.map(cal_two, cuts2), total=len(cuts2))
+                        tqdm.auto.tqdm(
+                            executor.map(
+                                cal_two, pairs, dates
+                            ),
+                            total=len(pairs),
+                        )
                     )
                 factor_new = factor_new + factor_new_more
             else:
                 # 开始计算因子值
                 for date1, date2 in tqdm.auto.tqdm(cuts2, desc="知不可乎骤得，托遗响于悲风。"):
                     df = cal_two(date1, date2)
                     factor_new.append(df)
@@ -5642,15 +5652,15 @@
             else:
                 # raise NotImplementedError(f"{date}这一期的优化失败，请检查")
                 logger.warning(f"{name}在{date}这一期的优化失败，请检查")
                 return None
         else:
             return None
 
-    def optimize_many_days(self, startdate: int = 20130101):
+    def optimize_many_days(self, startdate: int = STATES['START']):
         dates = [i for i in self.facs.index if i >= pd.Timestamp(str(startdate))]
         for date in tqdm.auto.tqdm(dates):
             fac = self.facs[self.facs.index == date].T.dropna()
             total_cap = self.total_caps[self.total_caps.index == date].T.dropna()
             indu_dummy = self.indu_dummys[self.indu_dummys.date <= date]
             indu_dummy = (
                 indu_dummy[indu_dummy.date == indu_dummy.date.max()]
@@ -5688,15 +5698,15 @@
         rets = pd.concat([ret, index, abret], axis=1).dropna()
         rets.columns = [f"{name}增强组合净值", f"{name}指数净值", f"{name}增强组合超额净值"]
         rets = (rets + 1).cumprod()
         rets = rets.apply(lambda x: x / x.iloc[0])
         comments = comments_on_twins(rets[f"{name}增强组合超额净值"], abret.dropna())
         return comments, rets
 
-    def run(self, startdate: int = 20130101) -> pd.DataFrame:
+    def run(self, startdate: int = STATES['START']) -> pd.DataFrame:
         """运行规划求解
 
         Parameters
         ----------
         startdate : int, optional
             起始日期, by default 20130101
```

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1/initialize.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1p10/initialize.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1p10/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v2/initialize.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v2/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/__init__.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/database.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/tools.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/labor/process.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/mail/email.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/__init__.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/database.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/tools.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/labor/process.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/mail/email.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/state/states.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/mail/email.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/state/decorators.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/state/homeplace.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/state/states.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/state/states.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 一些默认的参数
 """
 
-__updated__ = "2022-11-04 14:41:09"
+__updated__ = "2023-07-13 12:18:16"
 
 STATES = {
     "NO_LOG": False,
     "NO_COMMENT": False,
     "NO_SAVE": True,
     "NO_PLOT": False,
-    "START": 20130101,
+    "START": 20140101,
     "db_host": "127.0.0.1",
     "db_port": 3306,
     "db_user": "root",
     "db_password": "Kingwila98",
 }
 
 COMMENTS_WRITER=None
```

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze/withs/requires.py` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze.egg-info/PKG-INFO` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-ocean-breeze
-Version: 4.0.5
+Version: 4.0.6
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-4.0.5/pure_ocean_breeze.egg-info/SOURCES.txt` & `pure_ocean_breeze-4.0.6/pure_ocean_breeze.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-4.0.5/setup.py` & `pure_ocean_breeze-4.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-07-03 01:28:50"
+__updated__ = "2023-07-14 15:12:11"
 
 from setuptools import setup
 import setuptools
 import re
 import os
 import sys
 
@@ -11,15 +11,16 @@
 
 
 def get_version(package):
     """Return package version as listed in `__version__` in `init.py`."""
     init_py = open(os.path.join(package, "__init__.py")).read()
     return re.search("__version__ = ['\"]([^'\"]+)['\"]", init_py).group(1)
 
-install_requires=[
+
+install_requires = [
     # "numpy",
     "pandas<=1.5.3",
     "scipy",
     "statsmodels",
     "plotly",
     # "matplotlib",
     "pyarrow",
@@ -39,19 +40,24 @@
     "xpinyin",
     "cufflinks",
     "clickhouse_sqlalchemy",
     "tradetime",
     "deprecation",
     "questdb",
     "mpire",
+    "py7zr",
+    "unrar",
+    "rarfile",
+    "zipfile",
+    "chardet",
 ]
-if sys.platform.startswith('win'):
-    install_requires=install_requires+['psycopg2']
+if sys.platform.startswith("win"):
+    install_requires = install_requires + ["psycopg2"]
 else:
-    install_requires=install_requires+['psycopg2-binary']
+    install_requires = install_requires + ["psycopg2-binary"]
 
 setup(
     name="pure_ocean_breeze",
     version=get_version("pure_ocean_breeze"),
     description="stock factor test",
     # long_description="详见homepage\nhttps://github.com/chen-001/pure_ocean_breeze.git",
     long_description=long_description,
@@ -61,9 +67,13 @@
     url="https://github.com/chen-001/pure_ocean_breeze.git",
     project_urls={"Documentation": "https://chen-001.github.io/pure_ocean_breeze/"},
     install_requires=install_requires,
     python_requires=">=3",
     license="MIT",
     packages=setuptools.find_packages(),
     requires=[],
-    extras_require={'windows':['psycopg2'],'macos':['psycopg2-binary'],'linux':['psycopg2-binary']}
+    extras_require={
+        "windows": ["psycopg2"],
+        "macos": ["psycopg2-binary"],
+        "linux": ["psycopg2-binary"],
+    },
 )
```

