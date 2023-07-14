# Comparing `tmp/osc-1.1.4.tar.gz` & `tmp/osc-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osc-1.1.4.tar", last modified: Wed May 24 07:04:25 2023, max compression
+gzip compressed data, was "osc-1.2.0.tar", last modified: Fri Jul 14 09:12:07 2023, max compression
```

## Comparing `osc-1.1.4.tar` & `osc-1.2.0.tar`

### file list

```diff
@@ -1,87 +1,98 @@
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-24 07:04:25.964644 osc-1.1.4/
--rw-r--r--   0 dmach     (1000) dmach     (1000)      480 2023-05-24 07:04:23.000000 osc-1.1.4/AUTHORS
--rw-r--r--   0 dmach     (1000) dmach     (1000)    18092 2023-05-24 07:04:23.000000 osc-1.1.4/COPYING
--rw-r--r--   0 dmach     (1000) dmach     (1000)       63 2023-05-24 07:04:23.000000 osc-1.1.4/MANIFEST.in
--rw-r--r--   0 dmach     (1000) dmach     (1000)     7756 2023-05-24 07:04:23.000000 osc-1.1.4/NEWS
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1420 2023-05-24 07:04:25.964644 osc-1.1.4/PKG-INFO
--rw-r--r--   0 dmach     (1000) dmach     (1000)     5632 2023-05-24 07:04:23.000000 osc-1.1.4/README.md
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-24 07:04:25.960644 osc-1.1.4/osc/
--rw-r--r--   0 dmach     (1000) dmach     (1000)    13406 2023-05-24 07:04:23.000000 osc-1.1.4/osc/OscConfigParser.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      259 2023-05-24 07:04:23.000000 osc-1.1.4/osc/__init__.py
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-24 07:04:25.960644 osc-1.1.4/osc/_private/
--rw-r--r--   0 dmach     (1000) dmach     (1000)      692 2023-05-24 07:04:23.000000 osc-1.1.4/osc/_private/__init__.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     5770 2023-05-24 07:04:23.000000 osc-1.1.4/osc/_private/api.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     2338 2023-05-24 07:04:23.000000 osc-1.1.4/osc/_private/api_build.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      381 2023-05-24 07:04:23.000000 osc-1.1.4/osc/_private/api_configuration.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3347 2023-05-24 07:04:23.000000 osc-1.1.4/osc/_private/api_source.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1525 2023-05-24 07:04:23.000000 osc-1.1.4/osc/_private/common.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3623 2023-05-24 07:04:23.000000 osc-1.1.4/osc/_private/package.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1207 2023-05-24 07:04:23.000000 osc-1.1.4/osc/_private/request.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     8977 2023-05-24 07:04:23.000000 osc-1.1.4/osc/babysitter.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    63492 2023-05-24 07:04:23.000000 osc-1.1.4/osc/build.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3211 2023-05-24 07:04:23.000000 osc-1.1.4/osc/checker.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    10121 2023-05-24 07:04:23.000000 osc-1.1.4/osc/cmdln.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)   440457 2023-05-24 07:04:23.000000 osc-1.1.4/osc/commandline.py
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-24 07:04:25.960644 osc-1.1.4/osc/commands/
--rw-r--r--   0 dmach     (1000) dmach     (1000)        0 2023-05-24 07:04:23.000000 osc-1.1.4/osc/commands/__init__.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    40770 2023-05-24 07:04:23.000000 osc-1.1.4/osc/conf.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    25246 2023-05-24 07:04:23.000000 osc-1.1.4/osc/connection.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)   332241 2023-05-24 07:04:23.000000 osc-1.1.4/osc/core.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    11240 2023-05-24 07:04:23.000000 osc-1.1.4/osc/credentials.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    17821 2023-05-24 07:04:23.000000 osc-1.1.4/osc/fetch.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1611 2023-05-24 07:04:23.000000 osc-1.1.4/osc/grabber.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     2076 2023-05-24 07:04:23.000000 osc-1.1.4/osc/meter.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     5923 2023-05-24 07:04:23.000000 osc-1.1.4/osc/oscerr.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     6840 2023-05-24 07:04:23.000000 osc-1.1.4/osc/oscssl.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)        0 2023-05-24 07:04:23.000000 osc-1.1.4/osc/py.typed
--rw-r--r--   0 dmach     (1000) dmach     (1000)     9989 2023-05-24 07:04:23.000000 osc-1.1.4/osc/store.py
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-24 07:04:25.960644 osc-1.1.4/osc/util/
--rw-r--r--   0 dmach     (1000) dmach     (1000)       79 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/__init__.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     7084 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/ar.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     7225 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/archquery.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     8208 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/cpio.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     9258 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/debquery.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     2728 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/git_version.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1886 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/helper.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     5499 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/packagequery.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     6788 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/repodata.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    13167 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/rpmquery.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      809 2023-05-24 07:04:23.000000 osc-1.1.4/osc/util/safewriter.py
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-24 07:04:25.960644 osc-1.1.4/osc.egg-info/
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1420 2023-05-24 07:04:25.000000 osc-1.1.4/osc.egg-info/PKG-INFO
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1635 2023-05-24 07:04:25.000000 osc-1.1.4/osc.egg-info/SOURCES.txt
--rw-r--r--   0 dmach     (1000) dmach     (1000)        1 2023-05-24 07:04:25.000000 osc-1.1.4/osc.egg-info/dependency_links.txt
--rw-r--r--   0 dmach     (1000) dmach     (1000)       44 2023-05-24 07:04:25.000000 osc-1.1.4/osc.egg-info/entry_points.txt
--rw-r--r--   0 dmach     (1000) dmach     (1000)       52 2023-05-24 07:04:25.000000 osc-1.1.4/osc.egg-info/requires.txt
--rw-r--r--   0 dmach     (1000) dmach     (1000)        4 2023-05-24 07:04:25.000000 osc-1.1.4/osc.egg-info/top_level.txt
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1574 2023-05-24 07:04:25.964644 osc-1.1.4/setup.cfg
--rwxr-xr-x   0 dmach     (1000) dmach     (1000)       95 2023-05-24 07:04:23.000000 osc-1.1.4/setup.py
-drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-05-24 07:04:25.964644 osc-1.1.4/tests/
--rw-r--r--   0 dmach     (1000) dmach     (1000)      788 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test__private_api.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     4912 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test__private_package.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3168 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_addfiles.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1416 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_build.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    29754 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_commandline.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    21957 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_commit.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1451 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_conf.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      578 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_config_parser.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     1783 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_core.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     8446 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_core_package.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      877 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_core_request.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     8656 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_deletefiles.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    11258 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_difffiles.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     2320 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_doc_plugins.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      856 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_grabber.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)      926 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_helpers.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     4605 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_init_package.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3431 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_init_project.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3094 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_package_status.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     8779 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_prdiff.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     5829 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_project_status.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    10407 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_repairwc.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    24512 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_request.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     2307 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_results.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     3277 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_revertfiles.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     4891 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_setlinkrev.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)     8298 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_store.py
--rw-r--r--   0 dmach     (1000) dmach     (1000)    15545 2023-05-24 07:04:23.000000 osc-1.1.4/tests/test_update.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-07-14 09:12:07.901594 osc-1.2.0/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      480 2023-07-14 08:59:10.000000 osc-1.2.0/AUTHORS
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    18092 2023-07-14 08:59:10.000000 osc-1.2.0/COPYING
+-rw-r--r--   0 dmach     (1000) dmach     (1000)       63 2023-07-14 08:59:10.000000 osc-1.2.0/MANIFEST.in
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8577 2023-07-14 09:07:45.000000 osc-1.2.0/NEWS
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1420 2023-07-14 09:12:07.901594 osc-1.2.0/PKG-INFO
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5632 2023-07-14 08:59:10.000000 osc-1.2.0/README.md
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-07-14 09:12:07.893593 osc-1.2.0/osc/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    13406 2023-07-14 08:59:10.000000 osc-1.2.0/osc/OscConfigParser.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      259 2023-07-14 08:59:27.000000 osc-1.2.0/osc/__init__.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-07-14 09:12:07.897593 osc-1.2.0/osc/_private/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      692 2023-07-14 08:59:10.000000 osc-1.2.0/osc/_private/__init__.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     7063 2023-07-14 08:59:10.000000 osc-1.2.0/osc/_private/api.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2338 2023-07-14 08:59:10.000000 osc-1.2.0/osc/_private/api_build.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      381 2023-07-14 08:59:10.000000 osc-1.2.0/osc/_private/api_configuration.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3347 2023-07-14 08:59:10.000000 osc-1.2.0/osc/_private/api_source.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1525 2023-07-14 08:59:10.000000 osc-1.2.0/osc/_private/common.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3623 2023-07-14 08:59:10.000000 osc-1.2.0/osc/_private/package.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5741 2023-07-14 08:59:10.000000 osc-1.2.0/osc/_private/project.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1207 2023-07-14 08:59:10.000000 osc-1.2.0/osc/_private/request.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8977 2023-07-14 08:59:10.000000 osc-1.2.0/osc/babysitter.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    63507 2023-07-14 08:59:10.000000 osc-1.2.0/osc/build.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3211 2023-07-14 08:59:10.000000 osc-1.2.0/osc/checker.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    10121 2023-07-14 08:59:10.000000 osc-1.2.0/osc/cmdln.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)   441251 2023-07-14 08:59:10.000000 osc-1.2.0/osc/commandline.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-07-14 09:12:07.897593 osc-1.2.0/osc/commands/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)        0 2023-07-14 08:59:10.000000 osc-1.2.0/osc/commands/__init__.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      185 2023-07-14 08:59:10.000000 osc-1.2.0/osc/commands/repo.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2518 2023-07-14 08:59:10.000000 osc-1.2.0/osc/commands/repo_add.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1781 2023-07-14 08:59:10.000000 osc-1.2.0/osc/commands/repo_list.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1569 2023-07-14 08:59:10.000000 osc-1.2.0/osc/commands/repo_remove.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    40770 2023-07-14 08:59:10.000000 osc-1.2.0/osc/conf.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    25922 2023-07-14 08:59:10.000000 osc-1.2.0/osc/connection.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)   332358 2023-07-14 08:59:10.000000 osc-1.2.0/osc/core.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    11418 2023-07-14 08:59:10.000000 osc-1.2.0/osc/credentials.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    17821 2023-07-14 08:59:10.000000 osc-1.2.0/osc/fetch.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1611 2023-07-14 08:59:10.000000 osc-1.2.0/osc/grabber.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2076 2023-07-14 08:59:10.000000 osc-1.2.0/osc/meter.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5923 2023-07-14 08:59:10.000000 osc-1.2.0/osc/oscerr.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     6840 2023-07-14 08:59:10.000000 osc-1.2.0/osc/oscssl.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-07-14 09:12:07.897593 osc-1.2.0/osc/output/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      131 2023-07-14 08:59:10.000000 osc-1.2.0/osc/output/__init__.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2519 2023-07-14 08:59:10.000000 osc-1.2.0/osc/output/key_value_table.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      746 2023-07-14 08:59:10.000000 osc-1.2.0/osc/output/tty.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      450 2023-07-14 08:59:10.000000 osc-1.2.0/osc/output/widechar.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)        0 2023-07-14 08:59:10.000000 osc-1.2.0/osc/py.typed
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     9989 2023-07-14 08:59:10.000000 osc-1.2.0/osc/store.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-07-14 09:12:07.897593 osc-1.2.0/osc/util/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)       79 2023-07-14 08:59:10.000000 osc-1.2.0/osc/util/__init__.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     7084 2023-07-14 08:59:10.000000 osc-1.2.0/osc/util/ar.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     7225 2023-07-14 08:59:10.000000 osc-1.2.0/osc/util/archquery.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8208 2023-07-14 08:59:10.000000 osc-1.2.0/osc/util/cpio.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     9258 2023-07-14 08:59:10.000000 osc-1.2.0/osc/util/debquery.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2728 2023-07-14 08:59:10.000000 osc-1.2.0/osc/util/git_version.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1886 2023-07-14 08:59:10.000000 osc-1.2.0/osc/util/helper.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5499 2023-07-14 08:59:10.000000 osc-1.2.0/osc/util/packagequery.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     6788 2023-07-14 08:59:10.000000 osc-1.2.0/osc/util/repodata.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    13167 2023-07-14 08:59:10.000000 osc-1.2.0/osc/util/rpmquery.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      809 2023-07-14 08:59:10.000000 osc-1.2.0/osc/util/safewriter.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-07-14 09:12:07.893593 osc-1.2.0/osc.egg-info/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1420 2023-07-14 09:12:07.000000 osc-1.2.0/osc.egg-info/PKG-INFO
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1874 2023-07-14 09:12:07.000000 osc-1.2.0/osc.egg-info/SOURCES.txt
+-rw-r--r--   0 dmach     (1000) dmach     (1000)        1 2023-07-14 09:12:07.000000 osc-1.2.0/osc.egg-info/dependency_links.txt
+-rw-r--r--   0 dmach     (1000) dmach     (1000)       44 2023-07-14 09:12:07.000000 osc-1.2.0/osc.egg-info/entry_points.txt
+-rw-r--r--   0 dmach     (1000) dmach     (1000)       52 2023-07-14 09:12:07.000000 osc-1.2.0/osc.egg-info/requires.txt
+-rw-r--r--   0 dmach     (1000) dmach     (1000)        4 2023-07-14 09:12:07.000000 osc-1.2.0/osc.egg-info/top_level.txt
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1586 2023-07-14 09:12:07.901594 osc-1.2.0/setup.cfg
+-rwxr-xr-x   0 dmach     (1000) dmach     (1000)       95 2023-07-14 08:59:10.000000 osc-1.2.0/setup.py
+drwxr-xr-x   0 dmach     (1000) dmach     (1000)        0 2023-07-14 09:12:07.901594 osc-1.2.0/tests/
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      788 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test__private_api.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     4912 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test__private_package.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3168 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_addfiles.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1416 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_build.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    29754 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_commandline.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    21957 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_commit.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1451 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_conf.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      578 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_config_parser.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1783 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_core.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8446 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_core_package.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      877 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_core_request.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8656 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_deletefiles.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    11258 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_difffiles.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2320 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_doc_plugins.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      856 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_grabber.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)      926 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_helpers.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     4605 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_init_package.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3431 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_init_project.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     1462 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_output.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3094 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_package_status.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8779 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_prdiff.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     5829 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_project_status.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    10407 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_repairwc.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    24512 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_request.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     2307 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_results.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     3277 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_revertfiles.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     4891 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_setlinkrev.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)     8298 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_store.py
+-rw-r--r--   0 dmach     (1000) dmach     (1000)    15545 2023-07-14 08:59:10.000000 osc-1.2.0/tests/test_update.py
```

### Comparing `osc-1.1.4/COPYING` & `osc-1.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/NEWS` & `osc-1.2.0/NEWS`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+- 1.2.0
+  - Command-line:
+    - Add 'repo' command and subcommands for managing repositories in project meta
+    - Extend 'browse' command to open requests in a web browser
+    - Add highlighting for 'osc diff' and similar commands
+    - Fix 'api' command to stream output to avoid running out of memory
+    - Fix printing utf-8 characters to stdout
+  - Connection:
+    - Fix ValueError: Cannot set verify_mode to CERT_NONE when check_hostname is enabled
+  - Authentication:
+    - Correctly handle passwords with utf-8 characters
+  - Library:
+    - Fix crash when submiting a SCM package which has no _link
+    - Fix local service execution of scmsync packages
+    - Detect target package by its full name, instead of assuming its origin is identical to the source package type
+  - Other:
+    - Spell openSUSE correctly
+
 - 1.1.4
   - Command-line:
     - Change 'review list' command to display open requests (state: new, review, declined)
     - Fix running osc in an AppImage by switching to the correct working directory
     - Handle ProtocolError exception
   - Library:
     - Add 'req_states' parameter to osc.core.get_review_list()
```

### Comparing `osc-1.1.4/PKG-INFO` & `osc-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osc
-Version: 1.1.4
+Version: 1.2.0
 Summary: openSUSE commander
 Home-page: http://en.opensuse.org/openSUSE:OSC
 Download-URL: https://github.com/openSUSE/osc
 Author: openSUSE project
 Author-email: opensuse-buildservice@opensuse.org
 License: GPLv2+
 Keywords: openSUSE,SUSE,RPM,build,buildservice,command-line
```

### Comparing `osc-1.1.4/README.md` & `osc-1.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![codecov](https://codecov.io/gh/openSUSE/osc/branch/master/graph/badge.svg)](https://codecov.io/gh/openSUSE/osc)
 [![code climate](https://github.com/openSUSE/osc/actions/workflows/codeql.yml/badge.svg)](https://github.com/openSUSE/osc/actions/workflows/codeql.yml)
 [![contributors](https://img.shields.io/github/contributors/openSUSE/osc.svg)](https://github.com/openSUSE/osc/graphs/contributors)
 
 
 # openSUSE Commander
 
-OpenSUSE Commander (osc) is a command-line interface to the
+openSUSE Commander (osc) is a command-line interface to the
 [Open Build Service (OBS)](https://github.com/openSUSE/open-build-service/).
 
 
 ## Installation
 
 RPM packages are available in the [openSUSE:Tools](http://download.opensuse.org/repositories/openSUSE:/Tools/) repository.
```

### Comparing `osc-1.1.4/osc/OscConfigParser.py` & `osc-1.2.0/osc/OscConfigParser.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/_private/__init__.py` & `osc-1.2.0/osc/_private/__init__.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/_private/api.py` & `osc-1.2.0/osc/_private/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -60,14 +60,42 @@
 
     url = osc_core.makeurl(apiurl, path, query)
     with osc_connection.http_POST(url) as f:
         root = ET.parse(f).getroot()
     return root
 
 
+def put(apiurl, path, query=None, data=None):
+    """
+    Send a PUT request to OBS.
+
+    :param apiurl: OBS apiurl.
+    :type  apiurl: str
+    :param path: URL path segments.
+    :type  path: list(str)
+    :param query: URL query values.
+    :type  query: dict(str, str)
+    :returns: Parsed XML root.
+    :rtype:   xml.etree.ElementTree.Element
+    """
+    from osc import connection as osc_connection
+    from osc import core as osc_core
+
+    assert apiurl
+    assert path
+
+    if not isinstance(path, (list, tuple)):
+        raise TypeError("Argument `path` expects a list of strings")
+
+    url = osc_core.makeurl(apiurl, path, query)
+    with osc_connection.http_PUT(url, data=data) as f:
+        root = osc_core.ET.parse(f).getroot()
+    return root
+
+
 def _to_xpath(*args):
     """
     Convert strings and dictionaries to xpath:
         string gets translated to a node name
         dictionary gets translated to [@key='value'] predicate
 
     All values are properly escaped.
@@ -135,14 +163,38 @@
     assert root.tag == root_name
     if not args:
         # only verify the root tag
         return root
     return root.find(_to_xpath(*args))
 
 
+def group_child_nodes(node):
+    nodes = node[:]
+    result = []
+
+    while nodes:
+        # look at the tag of the first node
+        tag = nodes[0].tag
+
+        # collect all nodes with the same tag and append them to the result
+        # then repeat the step for the next tag(s)
+        matches = []
+        others = []
+        for i in nodes:
+            if i.tag == tag:
+                matches.append(i)
+            else:
+                others.append(i)
+
+        result += matches
+        nodes = others
+
+    node[:] = result
+
+
 def write_xml_node_to_file(node, path, indent=True):
     """
     Write a XML node to a file.
 
     :param node: Node to write.
     :type  node: xml.etree.ElementTree.Element
     :param path: Path to a file that will be written to.
```

### Comparing `osc-1.1.4/osc/_private/api_build.py` & `osc-1.2.0/osc/_private/api_build.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/_private/api_source.py` & `osc-1.2.0/osc/_private/api_source.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/_private/common.py` & `osc-1.2.0/osc/_private/common.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/_private/package.py` & `osc-1.2.0/osc/_private/package.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/_private/request.py` & `osc-1.2.0/osc/_private/request.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/babysitter.py` & `osc-1.2.0/osc/babysitter.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/build.py` & `osc-1.2.0/osc/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -1363,15 +1363,15 @@
         else:
             print('WARNING: deb packages get not verified, they can compromise your system !')
     else:
         print('WARNING: unknown packages get not verified, they can compromise your system !')
 
     for i in bi.deps:
         if i.hdrmd5:
-            if not i.name.startswith('container:') and i.pacsuffix != 'rpm':
+            if not i.name.startswith('container:') and not i.fullfilename.endswith(".rpm"):
                 continue
             if i.name.startswith('container:'):
                 hdrmd5 = dgst(i.fullfilename)
             else:
                 hdrmd5 = packagequery.PackageQuery.queryhdrmd5(i.fullfilename)
             if not hdrmd5:
                 print("Error: cannot get hdrmd5 for %s" % i.fullfilename)
```

### Comparing `osc-1.1.4/osc/checker.py` & `osc-1.2.0/osc/checker.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/cmdln.py` & `osc-1.2.0/osc/cmdln.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/commandline.py` & `osc-1.2.0/osc/commandline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1679,18 +1679,18 @@
             if len(args) > 1:
                 query['project'] = args[0]
                 query['package'] = args[1]
 
             url = makeurl(apiurl, url_path, query)
             f = http_POST(url)
             while True:
-                buf = f.read(16384)
-                if not buf:
+                data = f.read(16384)
+                if not data:
                     break
-                sys.stdout.write(decode_it(buf))
+                sys.stdout.buffer.write(data)
 
         elif opts.delete:
             print("Delete token")
             url_path.append(opts.delete)
             url = makeurl(apiurl, url_path)
             http_DELETE(url)
         elif opts.trigger:
@@ -1709,15 +1709,15 @@
             print(decode_it(fd.read()))
         else:
             if args and args[0] in ['create', 'delete', 'trigger']:
                 raise oscerr.WrongArgs("Did you mean --" + args[0] + "?")
             # just list token
             url = makeurl(apiurl, url_path)
             for data in streamfile(url, http_GET):
-                sys.stdout.write(decode_it(data))
+                sys.stdout.buffer.write(data)
 
     @cmdln.option('-a', '--attribute', metavar='ATTRIBUTE',
                         help='affect only a given attribute')
     @cmdln.option('--attribute-defaults', action='store_true',
                   help='include defined attribute defaults')
     @cmdln.option('--attribute-project', action='store_true',
                   help='include project values, if missing in packages ')
@@ -1981,15 +1981,15 @@
             if opts.set:
                 for i in opts.set.split(','):
                     values += '<value>%s</value>' % _private.api.xml_escape(i)
 
             d = '<attributes><attribute namespace=\'%s\' name=\'%s\' >%s</attribute></attributes>' % (aname[0], aname[1], values)
             url = makeurl(apiurl, attributepath)
             for data in streamfile(url, http_POST, data=d):
-                sys.stdout.write(decode_it(data))
+                sys.stdout.buffer.write(data)
 
         # upload file
         if opts.file:
 
             if opts.file == '-':
                 f = sys.stdin.read()
             else:
@@ -2048,15 +2048,15 @@
                 http_DELETE(u)
             elif cmd == 'attribute':
                 if not opts.attribute:
                     raise oscerr.WrongOptions('no attribute given to create')
                 attributepath.append(opts.attribute)
                 u = makeurl(apiurl, attributepath)
                 for data in streamfile(u, http_DELETE):
-                    sys.stdout.write(decode_it(data))
+                    sys.stdout.buffer.write(data)
             else:
                 raise oscerr.WrongOptions('The --delete switch is only for pattern metadata or attributes.')
 
     # TODO: rewrite and consolidate the current submitrequest/createrequest "mess"
 
     @cmdln.option('-m', '--message', metavar='TEXT',
                   help='specify message TEXT')
@@ -2336,15 +2336,15 @@
                 rdiff += server_diff(apiurl,
                                      dst_project, dst_package, None,
                                      src_project, src_package, rev, True)
             except:
                 rdiff = b''
 
         if opts.diff:
-            run_pager(rdiff)
+            run_pager(highlight_diff(rdiff))
             return
         if rdiff is not None:
             rdiff = decode_it(rdiff)
 
         supersede_existing = False
         reqs = []
         if not opts.supersede:
@@ -3395,15 +3395,15 @@
                     if not r.get_actions('submit') and not r.get_actions('maintenance_incident') and not r.get_actions('maintenance_release'):
                         raise oscerr.WrongOptions('\'--diff\' not possible (request has no supported actions)')
                     for action in sr_actions:
                         diff += b'old: %s/%s\nnew: %s/%s\n' % (action.src_project.encode(), action.src_package.encode(),
                                                                action.tgt_project.encode(), action.tgt_package.encode())
                         diff += submit_action_diff(apiurl, action)
                         diff += b'\n\n'
-                run_pager(diff, tmp_suffix='')
+                run_pager(highlight_diff(diff), tmp_suffix="")
 
         # checkout
         elif cmd in ('checkout', 'co'):
             r = get_request(apiurl, reqid)
             sr_actions = r.get_actions('submit', 'maintenance_release')
             if not sr_actions:
                 raise oscerr.WrongArgs('\'checkout\' not possible (request has no \'submit\' actions)')
@@ -4616,16 +4616,29 @@
                 raise oscerr.APIError('package is not a source link')
             baserev = linkinfo.get('baserev')
             opts.revision = baserev
             if pacs:
                 print("diff working copy against last committed version\n")
             else:
                 print("diff committed package against linked revision %s\n" % baserev)
-                run_pager(server_diff(self.get_api_url(), linkinfo.get('project'), linkinfo.get('package'), baserev,
-                                      args[0], args[1], linkinfo.get('lsrcmd5'), not opts.plain, opts.missingok))
+                run_pager(
+                    highlight_diff(
+                        server_diff(
+                            self.get_api_url(),
+                            linkinfo.get("project"),
+                            linkinfo.get("package"),
+                            baserev,
+                            args[0],
+                            args[1],
+                            linkinfo.get("lsrcmd5"),
+                            not opts.plain,
+                            opts.missingok,
+                        )
+                    )
+                )
                 return
 
         if opts.change:
             try:
                 rev = int(opts.change)
                 if rev > 0:
                     rev1 = rev - 1
@@ -4651,15 +4664,15 @@
                     # "." is illegal filename that causes server to return 400
                     files = None
                 else:
                     files = args
                 diff += server_diff_noex(pac.apiurl, pac.prjname, pac.name, rev1,
                                          pac.prjname, pac.name, rev2,
                                          not opts.plain, opts.missingok, opts.meta, not opts.unexpand, files=files)
-        run_pager(diff)
+        run_pager(highlight_diff(diff))
 
     @cmdln.option('--issues-only', action='store_true',
                   help='show only issues in diff')
     @cmdln.option('-M', '--meta', action='store_true',
                         help='diff meta data')
     @cmdln.option('-r', '--revision', metavar='N[:M]',
                   help='revision id, where N = old revision and M = new revision')
@@ -4742,15 +4755,15 @@
                                  meta=opts.meta,
                                  expand=not opts.unexpand,
                                  onlyissues=opts.issues_only,
                                  xml=opts.xml)
         if opts.issues_only:
             print(decode_it(rdiff))
         else:
-            run_pager(rdiff)
+            run_pager(highlight_diff(rdiff))
 
     def _pdiff_raise_non_existing_package(self, project, package, msg=None):
         raise oscerr.PackageMissing(project, package, msg or '%s/%s does not exist.' % (project, package))
 
     def _pdiff_package_exists(self, apiurl, project, package):
         try:
             show_package_meta(apiurl, project, package)
@@ -4889,15 +4902,15 @@
             self._pdiff_raise_non_existing_package(parent_project, parent_package,
                                                    msg='Parent for %s/%s (%s/%s) does not exist.' %
                                                    (project, package, parent_project, parent_package))
 
         rdiff = server_diff(apiurl, parent_project, parent_package, None, project,
                             package, None, unified=unified, missingok=noparentok)
 
-        run_pager(rdiff)
+        run_pager(highlight_diff(rdiff))
 
     def _get_branch_parent(self, prj):
         m = re.match('^home:[^:]+:branches:(.+)', prj)
         # OBS_Maintained is a special case
         if m and prj.find(':branches:OBS_Maintained:') == -1:
             return m.group(1)
         return None
@@ -5095,28 +5108,33 @@
 
     def do_browse(self, subcmd, opts, *args):
         """
         Opens browser
 
         usage:
            osc browse [PROJECT [PACKAGE]]
+           osc browse [REQUEST_ID]
         """
-        apiurl = self.get_api_url()
-
         args = list(args)
-        project, package = pop_project_package_from_args(
-            args, default_project=".", default_package=".", package_is_optional=True
-        )
-        ensure_no_remaining_args(args)
-
+        apiurl = self.get_api_url()
         obs_url = _private.get_configuration_value(apiurl, "obs_url")
-        if package:
-            url = f"{obs_url}/package/show/{project}/{package}"
+
+        if len(args) == 1 and args[0].isnumeric():
+            reqid = args.pop(0)
+            url = f"{obs_url}/request/show/{reqid}"
         else:
-            url = f"{obs_url}/project/show/{project}"
+            project, package = pop_project_package_from_args(
+                args, default_project=".", default_package=".", package_is_optional=True
+            )
+            if package:
+                url = f"{obs_url}/package/show/{project}/{package}"
+            else:
+                url = f"{obs_url}/project/show/{project}"
+
+        ensure_no_remaining_args(args)
 
         run_external('xdg-open', url)
 
     @cmdln.option('-r', '--revision', metavar='rev',
                         help='checkout the specified revision. '
                              'NOTE: if you checkout the complete project '
                              'this option is ignored!')
@@ -6370,19 +6388,19 @@
             offset = int(opts.offset)
         logfile = os.path.join(buildroot, '.build.log')
         if not os.path.isfile(logfile):
             raise oscerr.OscIOError(None, 'logfile \'%s\' does not exist' % logfile)
         f = open(logfile, 'rb')
         f.seek(offset)
         data = f.read(BUFSIZE)
-        data = decode_it(data)
         while len(data):
             if opts.strip_time or conf.config['buildlog_strip_time']:
+                # FIXME: this is not working when the time is split between 2 chunks
                 data = buildlog_strip_time(data)
-            sys.stdout.write(decode_it(data))
+            sys.stdout.buffer.write(data)
             data = f.read(BUFSIZE)
         f.close()
 
     @cmdln.option('-M', '--multibuild-package', metavar='FLAVOR', help=HELP_MULTIBUILD_ONE)
     @cmdln.alias('tr')
     def do_triggerreason(self, subcmd, opts, *args):
         """
@@ -8691,28 +8709,30 @@
             opts.headers = dict(opts.headers)
 
         r = http_request(opts.method,
                          url,
                          data=opts.data,
                          file=opts.file,
                          headers=opts.headers)
-        out = r.read()
 
         if opts.edit:
+            # to edit the output, we need to read all of it
+            # it's going to run ouf of memory if the data is too big
+            out = r.read()
             text = edit_text(out)
             r = http_request("PUT",
                              url,
                              data=text,
                              headers=opts.headers)
-            out = r.read()
 
-        if isinstance(out, str):
-            sys.stdout.write(out)
-        else:
-            sys.stdout.buffer.write(out)
+        while True:
+            data = r.read(8192)
+            if not data:
+                break
+            sys.stdout.buffer.write(data)
 
     @cmdln.option('-b', '--bugowner-only', action='store_true',
                   help='Show only the bugowner')
     @cmdln.option('-B', '--bugowner', action='store_true',
                   help='Show only the bugowner if defined, or maintainer otherwise')
     @cmdln.option('-e', '--email', action='store_true',
                   help='show email addresses instead of user names')
@@ -9550,18 +9570,18 @@
                         if not opts.notraverse and len(l) > 1 and l[0] and l[1] and e.code == 404:
                             print('%s has no key, trying %s' % (prj, l[0]))
                             prj = l[0]
                         else:
                             raise
 
         while True:
-            buf = f.read(16384)
-            if not buf:
+            data = f.read(16384)
+            if not data:
                 break
-            sys.stdout.write(decode_it(buf))
+            sys.stdout.buffer.write(data)
 
     @cmdln.option('-m', '--message',
                   help='add MESSAGE to changes (do not open an editor)')
     @cmdln.option('-F', '--file', metavar='FILE',
                   help='read changes message from FILE (do not open an editor)')
     @cmdln.option('-e', '--just-edit', action='store_true', default=False,
                   help='just open changes (cannot be used with -m)')
```

### Comparing `osc-1.1.4/osc/conf.py` & `osc-1.2.0/osc/conf.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/connection.py` & `osc-1.2.0/osc/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,18 +100,22 @@
     # rebuild proxy url in order to remove auth because ProxyManager would fail on it
     if proxy_purl.port:
         proxy_url = f"{proxy_purl.scheme}://{proxy_purl.host}:{proxy_purl.port}"
     else:
         proxy_url = f"{proxy_purl.scheme}://{proxy_purl.host}"
 
     proxy_headers = urllib3.make_headers(
-        proxy_basic_auth=proxy_purl.auth,
         user_agent=f"osc/{__version__}",
     )
 
+    proxy_basic_auth = urllib.parse.unquote(proxy_purl.auth)
+    proxy_basic_auth = proxy_basic_auth.encode("utf-8")
+    proxy_basic_auth = base64.b64encode(proxy_basic_auth).decode()
+    proxy_headers["Proxy-Authorization"] = f"Basic {proxy_basic_auth:s}"
+
     manager = urllib3.ProxyManager(proxy_url, proxy_headers=proxy_headers)
     return manager
 
 
 # Instantiate on first use in `http_request()`.
 # Each `apiurl` requires a differently configured pool
 # (incl. trusted keys for example).
@@ -248,17 +252,27 @@
             raise_on_status=False,
             **retries_kwargs,
         )
 
         if purl.scheme == "https":
             ssl_context = oscssl.create_ssl_context()
             ssl_context.load_default_certs()
+            pool_kwargs["ssl_context"] = ssl_context
             # turn cert verification off if sslcertck = 0
+
+            # urllib3 v1
             pool_kwargs["cert_reqs"] = "CERT_REQUIRED" if options["sslcertck"] else "CERT_NONE"
-            pool_kwargs["ssl_context"] = ssl_context
+
+            # urllib3 v2
+            if options["sslcertck"]:
+                ssl_context.check_hostname = True
+                ssl_context.verify_mode = ssl.CERT_REQUIRED
+            else:
+                ssl_context.check_hostname = False
+                ssl_context.verify_mode = ssl.CERT_NONE
 
         if purl.scheme == "http" and HTTP_PROXY_MANAGER and not urllib.request.proxy_bypass(url):
             # connection through HTTP proxy
             pool = HTTP_PROXY_MANAGER.connection_from_host(
                 host=purl.host,
                 port=purl.port,
                 scheme=purl.scheme,
@@ -535,15 +549,20 @@
 
     def set_request_headers_after_401(self, url, request_headers, response):
         auth_schemes = self._get_auth_schemes(response)
         if "basic" not in auth_schemes:
             return False
         if not self.user or not self.password:
             return False
-        request_headers.update(urllib3.make_headers(basic_auth=f"{self.user}:{self.password}"))
+
+        basic_auth = f"{self.user:s}:{self.password:s}"
+        basic_auth = basic_auth.encode("utf-8")
+        basic_auth = base64.b64encode(basic_auth).decode()
+        request_headers["Authorization"] = f"Basic {basic_auth:s}"
+
         return True
 
     def process_response(self, url, request_headers, response):
         pass
 
 
 class SignatureAuthHandler(AuthHandlerBase):
```

### Comparing `osc-1.1.4/osc/core.py` & `osc-1.2.0/osc/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1933,16 +1933,16 @@
             self.skipped = []
             self.to_be_added = []
             self.to_be_deleted = []
             self.in_conflict = []
             self.linkrepair = None
             self.rev = None
             self.srcmd5 = None
-            self.linkinfo = None
-            self.serviceinfo = None
+            self.linkinfo = Linkinfo()
+            self.serviceinfo = DirectoryServiceinfo()
             self.size_limit = None
             self.meta = None
             self.excluded = []
             self.filenamelist_unvers = []
             return
 
         files_tree = read_filemeta(self.dir)
@@ -2626,22 +2626,21 @@
     def run_source_services(self, mode=None, singleservice=None, verbose=None):
         if self.name.startswith("_"):
             return 0
         curdir = os.getcwd()
         os.chdir(self.absdir)  # e.g. /usr/lib/obs/service/verify_file fails if not inside the project dir.
         si = Serviceinfo()
         if os.path.exists('_service'):
-            if self.filenamelist.count('_service') or self.filenamelist_unvers.count('_service'):
-                try:
-                    service = ET.parse(os.path.join(self.absdir, '_service')).getroot()
-                except ET.ParseError as v:
-                    line, column = v.position
-                    print('XML error in _service file on line %s, column %s' % (line, column))
-                    sys.exit(1)
-                si.read(service)
+            try:
+                service = ET.parse(os.path.join(self.absdir, '_service')).getroot()
+            except ET.ParseError as v:
+                line, column = v.position
+                print('XML error in _service file on line %s, column %s' % (line, column))
+                sys.exit(1)
+            si.read(service)
         si.getProjectGlobalServices(self.apiurl, self.prjname, self.name)
         r = si.execute(self.absdir, mode, singleservice, verbose)
         os.chdir(curdir)
         return r
 
     def revert(self, filename):
         if filename not in self.filenamelist and filename not in self.to_be_added:
@@ -4365,14 +4364,32 @@
         dist = _get_linux_distro()
         if dist == 'debian':
             return 'pager'
         return 'less'
     return 'more'
 
 
+def format_diff_line(line):
+    if line.startswith(b"+++") or line.startswith(b"---") or line.startswith(b"Index:"):
+        line = b"\x1b[1m" + line + b"\x1b[0m"
+    elif line.startswith(b"+"):
+        line = b"\x1b[32m" + line + b"\x1b[0m"
+    elif line.startswith(b"-"):
+        line = b"\x1b[31m" + line + b"\x1b[0m"
+    elif line.startswith(b"@"):
+        line = b"\x1b[96m" + line + b"\x1b[0m"
+    return line
+
+
+def highlight_diff(diff):
+    if sys.stdout.isatty():
+        diff = b"\n".join((format_diff_line(line) for line in diff.split(b"\n")))
+    return diff
+
+
 def run_pager(message, tmp_suffix=''):
     if not message:
         return
 
     if not sys.stdout.isatty():
         if isinstance(message, str):
             print(message)
@@ -6921,21 +6938,15 @@
     lastsucceeded=False,
 ):
     """prints out the buildlog on stdout"""
 
     def print_data(data, strip_time=False):
         if strip_time:
             data = buildlog_strip_time(data)
-        # hmm calling decode_it is a bit problematic because data might begin
-        # or end with an, for instance, incomplete utf-8 sequence
-        sys.stdout.write(decode_it(data.translate(all_bytes, remove_bytes)))
-
-    # to protect us against control characters
-    all_bytes = bytes.maketrans(b'', b'')
-    remove_bytes = all_bytes[:8] + all_bytes[14:32]  # accept tabs and newlines
+        sys.stdout.buffer.write(data)
 
     query = {'nostream': '1', 'start': '%s' % offset}
     if last:
         query['last'] = 1
     if lastsucceeded:
         query['lastsucceeded'] = 1
     retry_count = 0
```

### Comparing `osc-1.1.4/osc/credentials.py` & `osc-1.2.0/osc/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,19 @@
                       file=sys.stderr)
                 password = password()
             if password is None:
                 raise oscerr.OscIOError(None, 'Unable to retrieve password')
             self._password = password
         return self._password
 
+    def __format__(self, format_spec):
+        if format_spec.endswith("s"):
+            return f"{self.__str__():{format_spec}}"
+        return super().__format__(format_spec)
+
     def __len__(self):
         return len(str(self))
 
     def __add__(self, other):
         return str(self) + other
 
     def __radd__(self, other):
```

### Comparing `osc-1.1.4/osc/fetch.py` & `osc-1.2.0/osc/fetch.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/grabber.py` & `osc-1.2.0/osc/grabber.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/meter.py` & `osc-1.2.0/osc/meter.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/oscerr.py` & `osc-1.2.0/osc/oscerr.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/oscssl.py` & `osc-1.2.0/osc/oscssl.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/store.py` & `osc-1.2.0/osc/store.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/util/ar.py` & `osc-1.2.0/osc/util/ar.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/util/archquery.py` & `osc-1.2.0/osc/util/archquery.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/util/cpio.py` & `osc-1.2.0/osc/util/cpio.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/util/debquery.py` & `osc-1.2.0/osc/util/debquery.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/util/git_version.py` & `osc-1.2.0/osc/util/git_version.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/util/helper.py` & `osc-1.2.0/osc/util/helper.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/util/packagequery.py` & `osc-1.2.0/osc/util/packagequery.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/util/repodata.py` & `osc-1.2.0/osc/util/repodata.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/util/rpmquery.py` & `osc-1.2.0/osc/util/rpmquery.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc/util/safewriter.py` & `osc-1.2.0/osc/util/safewriter.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/osc.egg-info/PKG-INFO` & `osc-1.2.0/osc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osc
-Version: 1.1.4
+Version: 1.2.0
 Summary: openSUSE commander
 Home-page: http://en.opensuse.org/openSUSE:OSC
 Download-URL: https://github.com/openSUSE/osc
 Author: openSUSE project
 Author-email: opensuse-buildservice@opensuse.org
 License: GPLv2+
 Keywords: openSUSE,SUSE,RPM,build,buildservice,command-line
```

### Comparing `osc-1.1.4/osc.egg-info/SOURCES.txt` & `osc-1.2.0/osc.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -32,16 +32,25 @@
 osc/_private/__init__.py
 osc/_private/api.py
 osc/_private/api_build.py
 osc/_private/api_configuration.py
 osc/_private/api_source.py
 osc/_private/common.py
 osc/_private/package.py
+osc/_private/project.py
 osc/_private/request.py
 osc/commands/__init__.py
+osc/commands/repo.py
+osc/commands/repo_add.py
+osc/commands/repo_list.py
+osc/commands/repo_remove.py
+osc/output/__init__.py
+osc/output/key_value_table.py
+osc/output/tty.py
+osc/output/widechar.py
 osc/util/__init__.py
 osc/util/ar.py
 osc/util/archquery.py
 osc/util/cpio.py
 osc/util/debquery.py
 osc/util/git_version.py
 osc/util/helper.py
@@ -63,14 +72,15 @@
 tests/test_deletefiles.py
 tests/test_difffiles.py
 tests/test_doc_plugins.py
 tests/test_grabber.py
 tests/test_helpers.py
 tests/test_init_package.py
 tests/test_init_project.py
+tests/test_output.py
 tests/test_package_status.py
 tests/test_prdiff.py
 tests/test_project_status.py
 tests/test_repairwc.py
 tests/test_request.py
 tests/test_results.py
 tests/test_revertfiles.py
```

### Comparing `osc-1.1.4/setup.cfg` & `osc-1.2.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 	Topic :: System :: Archiving :: Packaging
 
 [options]
 packages = 
 	osc
 	osc._private
 	osc.commands
+	osc.output
 	osc.util
 install_requires = 
 	cryptography
 	rpm
 	urllib3
 
 [options.extras_require]
```

### Comparing `osc-1.1.4/tests/test__private_api.py` & `osc-1.2.0/tests/test__private_api.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test__private_package.py` & `osc-1.2.0/tests/test__private_package.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_addfiles.py` & `osc-1.2.0/tests/test_addfiles.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_build.py` & `osc-1.2.0/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_commandline.py` & `osc-1.2.0/tests/test_commandline.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_commit.py` & `osc-1.2.0/tests/test_commit.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_conf.py` & `osc-1.2.0/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_config_parser.py` & `osc-1.2.0/tests/test_config_parser.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_core.py` & `osc-1.2.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_core_package.py` & `osc-1.2.0/tests/test_core_package.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_core_request.py` & `osc-1.2.0/tests/test_core_request.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_deletefiles.py` & `osc-1.2.0/tests/test_deletefiles.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_difffiles.py` & `osc-1.2.0/tests/test_difffiles.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_doc_plugins.py` & `osc-1.2.0/tests/test_doc_plugins.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_grabber.py` & `osc-1.2.0/tests/test_grabber.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_helpers.py` & `osc-1.2.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_init_package.py` & `osc-1.2.0/tests/test_init_package.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_init_project.py` & `osc-1.2.0/tests/test_init_project.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_package_status.py` & `osc-1.2.0/tests/test_package_status.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_prdiff.py` & `osc-1.2.0/tests/test_prdiff.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_project_status.py` & `osc-1.2.0/tests/test_project_status.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_repairwc.py` & `osc-1.2.0/tests/test_repairwc.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_request.py` & `osc-1.2.0/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_results.py` & `osc-1.2.0/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_revertfiles.py` & `osc-1.2.0/tests/test_revertfiles.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_setlinkrev.py` & `osc-1.2.0/tests/test_setlinkrev.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_store.py` & `osc-1.2.0/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `osc-1.1.4/tests/test_update.py` & `osc-1.2.0/tests/test_update.py`

 * *Files identical despite different names*

