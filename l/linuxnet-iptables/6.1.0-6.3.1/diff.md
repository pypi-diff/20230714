# Comparing `tmp/linuxnet-iptables-6.1.0.tar.gz` & `tmp/linuxnet-iptables-6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linuxnet-iptables-6.1.0.tar", last modified: Sun Jul  9 21:00:05 2023, max compression
+gzip compressed data, was "linuxnet-iptables-6.3.1.tar", last modified: Fri Jul 14 00:04:28 2023, max compression
```

## Comparing `linuxnet-iptables-6.1.0.tar` & `linuxnet-iptables-6.3.1.tar`

### file list

```diff
@@ -1,103 +1,105 @@
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-09 21:00:05.601427 linuxnet-iptables-6.1.0/
--rw-r--r--   0 panos     (1001) users      (100)    18810 2023-01-01 01:13:07.000000 linuxnet-iptables-6.1.0/.pylintrc
--rw-r--r--   0 panos     (1001) users      (100)     3549 2023-07-09 20:53:09.000000 linuxnet-iptables-6.1.0/CHANGELOG.md
--rw-r--r--   0 panos     (1001) users      (100)    32387 2023-01-01 01:13:10.000000 linuxnet-iptables-6.1.0/LICENSE
--rw-r--r--   0 panos     (1001) users      (100)      284 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/MANIFEST.in
--rw-r--r--   0 panos     (1001) users      (100)     5164 2023-01-01 01:13:07.000000 linuxnet-iptables-6.1.0/Makefile
--rw-r--r--   0 panos     (1001) users      (100)     4132 2023-07-09 21:00:05.601427 linuxnet-iptables-6.1.0/PKG-INFO
--rw-r--r--   0 panos     (1001) users      (100)     3237 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/README.md
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-09 21:00:05.589427 linuxnet-iptables-6.1.0/docs/
--rw-r--r--   0 panos     (1001) users      (100)      905 2023-01-01 01:13:06.000000 linuxnet-iptables-6.1.0/docs/Makefile
--rw-r--r--   0 panos     (1001) users      (100)     1491 2023-03-01 20:08:53.000000 linuxnet-iptables-6.1.0/docs/chain.rst
--rw-r--r--   0 panos     (1001) users      (100)     2850 2023-01-27 18:52:21.000000 linuxnet-iptables-6.1.0/docs/conf.py
--rw-r--r--   0 panos     (1001) users      (100)     1061 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/exception.rst
--rw-r--r--   0 panos     (1001) users      (100)     7952 2023-07-09 20:01:50.000000 linuxnet-iptables-6.1.0/docs/extensibility.rst
--rw-r--r--   0 panos     (1001) users      (100)     3319 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/index.rst
--rw-r--r--   0 panos     (1001) users      (100)     3187 2023-03-01 20:08:53.000000 linuxnet-iptables-6.1.0/docs/iptables_api.rst
--rw-r--r--   0 panos     (1001) users      (100)     3047 2023-07-09 20:01:50.000000 linuxnet-iptables-6.1.0/docs/match-example.py
--rw-r--r--   0 panos     (1001) users      (100)     2258 2023-02-08 00:19:00.000000 linuxnet-iptables-6.1.0/docs/match.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-09 21:00:05.591427 linuxnet-iptables-6.1.0/docs/matches/
--rw-r--r--   0 panos     (1001) users      (100)     1335 2023-06-19 04:02:28.000000 linuxnet-iptables-6.1.0/docs/matches/addrtypematch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1431 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/matches/commentmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)      990 2023-02-05 23:48:23.000000 linuxnet-iptables-6.1.0/docs/matches/connmarkmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1583 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/matches/conntrackmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1899 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/matches/icmpmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1861 2023-02-20 17:08:37.000000 linuxnet-iptables-6.1.0/docs/matches/limitmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1439 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/matches/markmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1965 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/matches/ownermatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     2447 2023-02-08 00:19:00.000000 linuxnet-iptables-6.1.0/docs/matches/packetmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1511 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/matches/packettypematch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1312 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/matches/statematch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1746 2023-07-09 20:01:50.000000 linuxnet-iptables-6.1.0/docs/matches/tcpmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1382 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/matches/tcpmssmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1521 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/matches/ttlmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)     1280 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/matches/udpmatch.rst
--rw-r--r--   0 panos     (1001) users      (100)      873 2023-03-01 20:08:53.000000 linuxnet-iptables-6.1.0/docs/rule.rst
--rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-05 23:48:29.000000 linuxnet-iptables-6.1.0/docs/table.rst
--rw-r--r--   0 panos     (1001) users      (100)     1129 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/target-example.py
--rw-r--r--   0 panos     (1001) users      (100)     1201 2023-02-08 00:19:00.000000 linuxnet-iptables-6.1.0/docs/target.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-09 21:00:05.593427 linuxnet-iptables-6.1.0/docs/targets/
--rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/targets/chaintarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/targets/connmarktarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/targets/dnattarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/targets/logtarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/targets/marktarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/targets/masqueradetarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      902 2023-06-04 01:25:41.000000 linuxnet-iptables-6.1.0/docs/targets/notracktarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      906 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/targets/rejecttarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/targets/snattarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      896 2023-06-04 01:25:41.000000 linuxnet-iptables-6.1.0/docs/targets/tracetarget.rst
--rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/docs/targets/ttltarget.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-09 21:00:05.593427 linuxnet-iptables-6.1.0/linuxnet/
--rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-6.1.0/linuxnet/__init__.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-09 21:00:05.594427 linuxnet-iptables-6.1.0/linuxnet/iptables/
--rw-r--r--   0 panos     (1001) users      (100)     1170 2023-03-01 20:08:53.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)    27815 2023-07-09 20:01:50.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/chain.py
--rw-r--r--   0 panos     (1001) users      (100)      854 2023-02-20 17:08:37.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/deps.py
--rw-r--r--   0 panos     (1001) users      (100)     1825 2023-02-05 23:48:20.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/exceptions.py
--rw-r--r--   0 panos     (1001) users      (100)     1340 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/extension.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-09 21:00:05.598427 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/
--rw-r--r--   0 panos     (1001) users      (100)     1339 2023-06-19 04:02:28.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)     4978 2023-07-09 20:01:49.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/addrtypematch.py
--rw-r--r--   0 panos     (1001) users      (100)     2879 2023-07-09 20:01:48.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/commentmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2285 2023-07-09 20:01:48.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/connmarkmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     5113 2023-07-09 20:01:48.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/conntrackmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     9761 2023-07-09 20:01:48.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/icmpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     4559 2023-07-09 20:01:48.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/limitmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     3872 2023-07-09 20:01:48.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/markmatch.py
--rw-r--r--   0 panos     (1001) users      (100)    16427 2023-07-09 20:01:48.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/match.py
--rw-r--r--   0 panos     (1001) users      (100)     7640 2023-07-09 20:01:48.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/ownermatch.py
--rw-r--r--   0 panos     (1001) users      (100)     7077 2023-07-09 20:01:48.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/packetmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2827 2023-07-09 20:01:48.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/packettypematch.py
--rw-r--r--   0 panos     (1001) users      (100)     3167 2023-07-09 20:01:49.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/statematch.py
--rw-r--r--   0 panos     (1001) users      (100)    11625 2023-07-09 20:01:49.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/tcpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     3776 2023-07-09 20:01:49.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/tcpmssmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     4317 2023-07-09 20:01:49.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/ttlmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     2597 2023-07-09 20:01:49.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/udpmatch.py
--rw-r--r--   0 panos     (1001) users      (100)     5782 2023-06-19 04:02:28.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/matches/util.py
--rw-r--r--   0 panos     (1001) users      (100)      918 2023-07-09 20:01:50.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/metadata.py
--rw-r--r--   0 panos     (1001) users      (100)     7810 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/parsing.py
--rw-r--r--   0 panos     (1001) users      (100)    17490 2023-07-09 20:01:49.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/rule.py
--rw-r--r--   0 panos     (1001) users      (100)    29276 2023-07-09 20:01:50.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/table.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-09 21:00:05.600427 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/
--rw-r--r--   0 panos     (1001) users      (100)     1165 2023-06-04 01:25:41.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)     7386 2023-03-05 20:39:10.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/connmarktarget.py
--rw-r--r--   0 panos     (1001) users      (100)     6518 2023-02-08 00:19:00.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/logtarget.py
--rw-r--r--   0 panos     (1001) users      (100)     6551 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/marktarget.py
--rw-r--r--   0 panos     (1001) users      (100)     4133 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/masqueradetarget.py
--rw-r--r--   0 panos     (1001) users      (100)     8146 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/nattarget.py
--rw-r--r--   0 panos     (1001) users      (100)     1405 2023-06-19 04:02:28.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/notracktarget.py
--rw-r--r--   0 panos     (1001) users      (100)     2124 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/rejecttarget.py
--rw-r--r--   0 panos     (1001) users      (100)    10896 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/target.py
--rw-r--r--   0 panos     (1001) users      (100)     1387 2023-06-19 04:02:28.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/tracetarget.py
--rw-r--r--   0 panos     (1001) users      (100)     4873 2023-02-06 17:07:04.000000 linuxnet-iptables-6.1.0/linuxnet/iptables/targets/ttltarget.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-09 21:00:05.600427 linuxnet-iptables-6.1.0/linuxnet_iptables.egg-info/
--rw-r--r--   0 panos     (1001) users      (100)     4132 2023-07-09 21:00:05.000000 linuxnet-iptables-6.1.0/linuxnet_iptables.egg-info/PKG-INFO
--rw-r--r--   0 panos     (1001) users      (100)     2699 2023-07-09 21:00:05.000000 linuxnet-iptables-6.1.0/linuxnet_iptables.egg-info/SOURCES.txt
--rw-r--r--   0 panos     (1001) users      (100)        1 2023-07-09 21:00:05.000000 linuxnet-iptables-6.1.0/linuxnet_iptables.egg-info/dependency_links.txt
--rw-r--r--   0 panos     (1001) users      (100)        9 2023-07-09 21:00:05.000000 linuxnet-iptables-6.1.0/linuxnet_iptables.egg-info/top_level.txt
--rw-r--r--   0 panos     (1001) users      (100)       38 2023-07-09 21:00:05.601427 linuxnet-iptables-6.1.0/setup.cfg
--rw-r--r--   0 panos     (1001) users      (100)     6662 2023-06-05 00:27:39.000000 linuxnet-iptables-6.1.0/setup.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-09 21:00:05.601427 linuxnet-iptables-6.1.0/tests/
--rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-6.1.0/tests/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)    65961 2023-07-09 20:01:50.000000 linuxnet-iptables-6.1.0/tests/iptables_test.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-14 00:04:28.825236 linuxnet-iptables-6.3.1/
+-rw-r--r--   0 panos     (1001) users      (100)    18810 2023-01-01 01:13:07.000000 linuxnet-iptables-6.3.1/.pylintrc
+-rw-r--r--   0 panos     (1001) users      (100)     3742 2023-07-13 23:59:57.000000 linuxnet-iptables-6.3.1/CHANGELOG.md
+-rw-r--r--   0 panos     (1001) users      (100)    32387 2023-01-01 01:13:10.000000 linuxnet-iptables-6.3.1/LICENSE
+-rw-r--r--   0 panos     (1001) users      (100)      284 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/MANIFEST.in
+-rw-r--r--   0 panos     (1001) users      (100)     5164 2023-01-01 01:13:07.000000 linuxnet-iptables-6.3.1/Makefile
+-rw-r--r--   0 panos     (1001) users      (100)     4108 2023-07-14 00:04:28.825236 linuxnet-iptables-6.3.1/PKG-INFO
+-rw-r--r--   0 panos     (1001) users      (100)     3213 2023-07-12 15:09:37.000000 linuxnet-iptables-6.3.1/README.md
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-14 00:04:28.814235 linuxnet-iptables-6.3.1/docs/
+-rw-r--r--   0 panos     (1001) users      (100)      905 2023-01-01 01:13:06.000000 linuxnet-iptables-6.3.1/docs/Makefile
+-rw-r--r--   0 panos     (1001) users      (100)     1491 2023-03-01 20:08:53.000000 linuxnet-iptables-6.3.1/docs/chain.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2850 2023-01-27 18:52:21.000000 linuxnet-iptables-6.3.1/docs/conf.py
+-rw-r--r--   0 panos     (1001) users      (100)     1061 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/exception.rst
+-rw-r--r--   0 panos     (1001) users      (100)     8110 2023-07-13 23:47:21.000000 linuxnet-iptables-6.3.1/docs/extensibility.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3319 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/index.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3187 2023-03-01 20:08:53.000000 linuxnet-iptables-6.3.1/docs/iptables_api.rst
+-rw-r--r--   0 panos     (1001) users      (100)     3047 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/docs/match-example.py
+-rw-r--r--   0 panos     (1001) users      (100)     2258 2023-02-08 00:19:00.000000 linuxnet-iptables-6.3.1/docs/match.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-14 00:04:28.817235 linuxnet-iptables-6.3.1/docs/matches/
+-rw-r--r--   0 panos     (1001) users      (100)     1335 2023-06-19 04:02:28.000000 linuxnet-iptables-6.3.1/docs/matches/addrtypematch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1431 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/matches/commentmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1268 2023-07-13 23:47:20.000000 linuxnet-iptables-6.3.1/docs/matches/connmarkmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1583 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/matches/conntrackmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1899 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/matches/icmpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1861 2023-02-20 17:08:37.000000 linuxnet-iptables-6.3.1/docs/matches/limitmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1438 2023-07-13 23:47:21.000000 linuxnet-iptables-6.3.1/docs/matches/markmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1965 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/matches/ownermatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2447 2023-02-08 00:19:00.000000 linuxnet-iptables-6.3.1/docs/matches/packetmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1511 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/matches/packettypematch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2248 2023-07-13 23:47:22.000000 linuxnet-iptables-6.3.1/docs/matches/recentmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1312 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/matches/statematch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2302 2023-07-13 23:47:21.000000 linuxnet-iptables-6.3.1/docs/matches/tcpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1382 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/matches/tcpmssmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1521 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/matches/ttlmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1280 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/matches/udpmatch.rst
+-rw-r--r--   0 panos     (1001) users      (100)      873 2023-03-01 20:08:53.000000 linuxnet-iptables-6.3.1/docs/rule.rst
+-rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-05 23:48:29.000000 linuxnet-iptables-6.3.1/docs/table.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1129 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/target-example.py
+-rw-r--r--   0 panos     (1001) users      (100)     1201 2023-02-08 00:19:00.000000 linuxnet-iptables-6.3.1/docs/target.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-14 00:04:28.818235 linuxnet-iptables-6.3.1/docs/targets/
+-rw-r--r--   0 panos     (1001) users      (100)      903 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/targets/chaintarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/targets/connmarktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/targets/dnattarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/targets/logtarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/targets/marktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      912 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/targets/masqueradetarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      902 2023-06-04 01:25:41.000000 linuxnet-iptables-6.3.1/docs/targets/notracktarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      906 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/targets/rejecttarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      900 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/targets/snattarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      896 2023-06-04 01:25:41.000000 linuxnet-iptables-6.3.1/docs/targets/tracetarget.rst
+-rw-r--r--   0 panos     (1001) users      (100)      897 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/docs/targets/ttltarget.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-14 00:04:28.818235 linuxnet-iptables-6.3.1/linuxnet/
+-rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-6.3.1/linuxnet/__init__.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-14 00:04:28.820236 linuxnet-iptables-6.3.1/linuxnet/iptables/
+-rw-r--r--   0 panos     (1001) users      (100)     1170 2023-03-01 20:08:53.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)    27956 2023-07-13 23:47:20.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/chain.py
+-rw-r--r--   0 panos     (1001) users      (100)      854 2023-02-20 17:08:37.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/deps.py
+-rw-r--r--   0 panos     (1001) users      (100)     1825 2023-02-05 23:48:20.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/exceptions.py
+-rw-r--r--   0 panos     (1001) users      (100)     1467 2023-07-13 23:47:20.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/extension.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-14 00:04:28.822236 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/
+-rw-r--r--   0 panos     (1001) users      (100)     1376 2023-07-13 23:47:19.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)     4978 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/addrtypematch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2879 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/commentmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2285 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/connmarkmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     5113 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/conntrackmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     9761 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/icmpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     4559 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/limitmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3872 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/markmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)    16568 2023-07-13 23:47:19.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/match.py
+-rw-r--r--   0 panos     (1001) users      (100)     7640 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/ownermatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     7077 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/packetmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2827 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/packettypematch.py
+-rw-r--r--   0 panos     (1001) users      (100)     9287 2023-07-13 23:47:21.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/recentmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3049 2023-07-13 23:47:19.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/statematch.py
+-rw-r--r--   0 panos     (1001) users      (100)    11676 2023-07-13 23:47:20.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/tcpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     3776 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/tcpmssmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     4317 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/ttlmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     2597 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/udpmatch.py
+-rw-r--r--   0 panos     (1001) users      (100)     6190 2023-07-13 23:47:19.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/matches/util.py
+-rw-r--r--   0 panos     (1001) users      (100)      918 2023-07-13 23:47:20.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/metadata.py
+-rw-r--r--   0 panos     (1001) users      (100)     8386 2023-07-13 23:47:20.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/parsing.py
+-rw-r--r--   0 panos     (1001) users      (100)    18505 2023-07-13 23:47:20.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/rule.py
+-rw-r--r--   0 panos     (1001) users      (100)    29276 2023-07-09 21:05:25.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/table.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-14 00:04:28.824236 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/
+-rw-r--r--   0 panos     (1001) users      (100)     1165 2023-06-04 01:25:41.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)     7386 2023-03-05 20:39:10.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/connmarktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     6518 2023-02-08 00:19:00.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/logtarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     6551 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/marktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     4133 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/masqueradetarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     8146 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/nattarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     1405 2023-06-19 04:02:28.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/notracktarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     2124 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/rejecttarget.py
+-rw-r--r--   0 panos     (1001) users      (100)    10896 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/target.py
+-rw-r--r--   0 panos     (1001) users      (100)     1387 2023-06-19 04:02:28.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/tracetarget.py
+-rw-r--r--   0 panos     (1001) users      (100)     4873 2023-02-06 17:07:04.000000 linuxnet-iptables-6.3.1/linuxnet/iptables/targets/ttltarget.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-14 00:04:28.824236 linuxnet-iptables-6.3.1/linuxnet_iptables.egg-info/
+-rw-r--r--   0 panos     (1001) users      (100)     4108 2023-07-14 00:04:28.000000 linuxnet-iptables-6.3.1/linuxnet_iptables.egg-info/PKG-INFO
+-rw-r--r--   0 panos     (1001) users      (100)     2769 2023-07-14 00:04:28.000000 linuxnet-iptables-6.3.1/linuxnet_iptables.egg-info/SOURCES.txt
+-rw-r--r--   0 panos     (1001) users      (100)        1 2023-07-14 00:04:28.000000 linuxnet-iptables-6.3.1/linuxnet_iptables.egg-info/dependency_links.txt
+-rw-r--r--   0 panos     (1001) users      (100)        9 2023-07-14 00:04:28.000000 linuxnet-iptables-6.3.1/linuxnet_iptables.egg-info/top_level.txt
+-rw-r--r--   0 panos     (1001) users      (100)       38 2023-07-14 00:04:28.825236 linuxnet-iptables-6.3.1/setup.cfg
+-rw-r--r--   0 panos     (1001) users      (100)     6662 2023-06-05 00:27:39.000000 linuxnet-iptables-6.3.1/setup.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-07-14 00:04:28.825236 linuxnet-iptables-6.3.1/tests/
+-rw-r--r--   0 panos     (1001) users      (100)        0 2023-01-01 01:13:07.000000 linuxnet-iptables-6.3.1/tests/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)    70348 2023-07-13 23:47:20.000000 linuxnet-iptables-6.3.1/tests/iptables_test.py
```

### Comparing `linuxnet-iptables-6.1.0/.pylintrc` & `linuxnet-iptables-6.3.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/CHANGELOG.md` & `linuxnet-iptables-6.3.1/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Change Log
 ==========
 
+6.3.1 (2023-07-13)
+------------------
+
+- added RecentMatch class
+- added ChainRule.iter_matches()
+- added GenericPositiveCriterion class for criteria that do
+  not support inequality comparisons
+
+
 6.1.0 (2023-07-09)
 ------------------
 
 - this version maintains user API backwards-compatibility;
   however the major version was changed because the Match/Criterion
   implementation was updated in a way that breaks
   backwards-compatibility with out-of-tree Match subclasses
-
 - the Chain and ChainRule classes are now iterable
-
 - added ability to zero the packet/byte counters of individual rules
-
 - the Chain.iter_rules() can now return rules that match a number of
   conditions: have a chain as a target, have a specific match, etc.
-
 - added support for TCP option matching (--tcp-option) to TcpMatch
 
 
 5.4.0 (2023-06-18)
 ------------------
 
 - added AddressTypeMatch class to support the 'addrtype' match
```

### Comparing `linuxnet-iptables-6.1.0/LICENSE` & `linuxnet-iptables-6.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/Makefile` & `linuxnet-iptables-6.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/PKG-INFO` & `linuxnet-iptables-6.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxnet-iptables
-Version: 6.1.0
+Version: 6.3.1
 Summary: programmatic access to Linux iptables
 Home-page: https://gitlab.com/panos-tools/linuxnet-iptables
 Author: Panagiotis (Panos) Tsirigotis
 Author-email: ptsirigotis01@gmail.com
 License: AGPLv3
 Project-URL: Source, https://gitlab.com/panos-tools/linuxnet-iptables
 Project-URL: Documentation, https://linuxnet-iptables.readthedocs.io/en/latest/index.html
@@ -31,15 +31,15 @@
 For the following examples, Python3 (3.6 or later) is required.
 
 ```python
 >>> from linuxnet.iptables import IptablesPacketFilterTable
 >>> table = IptablesPacketFilterTable('filter')
 >>> table.read_system_config()
 >>> input_chain = table.get_chain('INPUT')
->>> for rule in input_chain.get_rules():
+>>> for rule in input_chain:
 ...    print(' '.join(rule.to_iptables_args()))
 ...
 -j prod_bad_traffic
 -m state --state RELATED,ESTABLISHED -j ACCEPT
 -j prod_ingress
 -j prod_INPUT_ldrop
 >>>
@@ -66,15 +66,15 @@
 ...    output = f.read()
 ...
 >>> from linuxnet.iptables import IptablesPacketFilterTable
 >>> table = IptablesPacketFilterTable('filter')
 >>> table.init_from_output(output)
 True
 >>> input_chain = table.get_chain('INPUT')
->>> for rule in input_chain.get_rules():
+>>> for rule in input_chain:
 ...     print(' '.join(rule.to_iptables_args()))
 ...
 -j prod_bad_traffic
 -m state --state RELATED,ESTABLISHED -j ACCEPT
 -j prod_ingress
 -j prod_INPUT_ldrop
 >>>
```

### Comparing `linuxnet-iptables-6.1.0/README.md` & `linuxnet-iptables-6.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 For the following examples, Python3 (3.6 or later) is required.
 
 ```python
 >>> from linuxnet.iptables import IptablesPacketFilterTable
 >>> table = IptablesPacketFilterTable('filter')
 >>> table.read_system_config()
 >>> input_chain = table.get_chain('INPUT')
->>> for rule in input_chain.get_rules():
+>>> for rule in input_chain:
 ...    print(' '.join(rule.to_iptables_args()))
 ...
 -j prod_bad_traffic
 -m state --state RELATED,ESTABLISHED -j ACCEPT
 -j prod_ingress
 -j prod_INPUT_ldrop
 >>>
@@ -45,15 +45,15 @@
 ...    output = f.read()
 ...
 >>> from linuxnet.iptables import IptablesPacketFilterTable
 >>> table = IptablesPacketFilterTable('filter')
 >>> table.init_from_output(output)
 True
 >>> input_chain = table.get_chain('INPUT')
->>> for rule in input_chain.get_rules():
+>>> for rule in input_chain:
 ...     print(' '.join(rule.to_iptables_args()))
 ...
 -j prod_bad_traffic
 -m state --state RELATED,ESTABLISHED -j ACCEPT
 -j prod_ingress
 -j prod_INPUT_ldrop
 >>>
```

### Comparing `linuxnet-iptables-6.1.0/docs/Makefile` & `linuxnet-iptables-6.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/chain.rst` & `linuxnet-iptables-6.3.1/docs/chain.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/conf.py` & `linuxnet-iptables-6.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/exception.rst` & `linuxnet-iptables-6.3.1/docs/exception.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/extensibility.rst` & `linuxnet-iptables-6.3.1/docs/extensibility.rst`

 * *Files 2% similar despite different names*

```diff
@@ -266,7 +266,16 @@
 GenericCriterion
 ~~~~~~~~~~~~~~~~
 
 .. autoclass:: GenericCriterion
     :members:
     :member-order: bysource
     :show-inheritance:
+
+
+GenericPositiveCriterion
+~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. autoclass:: GenericPositiveCriterion
+    :members:
+    :member-order: bysource
+    :show-inheritance:
```

### Comparing `linuxnet-iptables-6.1.0/docs/index.rst` & `linuxnet-iptables-6.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/iptables_api.rst` & `linuxnet-iptables-6.3.1/docs/iptables_api.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/match-example.py` & `linuxnet-iptables-6.3.1/docs/match-example.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/match.rst` & `linuxnet-iptables-6.3.1/docs/match.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/matches/addrtypematch.rst` & `linuxnet-iptables-6.3.1/docs/matches/addrtypematch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/matches/commentmatch.rst` & `linuxnet-iptables-6.3.1/docs/matches/commentmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/matches/connmarkmatch.rst` & `linuxnet-iptables-6.3.1/docs/targets/notracktarget.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ..
-    Copyright (c) 2022, 2023, Panagiotis Tsirigotis
+    Copyright (c) 2023, Panagiotis Tsirigotis
     
     This file is part of linuxnet-iptables.
     
     linuxnet-iptables is free software: you can redistribute it and/or
     modify it under the terms of version 3 of the GNU Affero General Public
     License as published by the Free Software Foundation.
     
@@ -14,17 +14,14 @@
     
     You should have received a copy of the GNU Affero General
     Public License along with linuxnet-iptables. If not, see
     <https://www.gnu.org/licenses/>.
 
 .. currentmodule:: linuxnet.iptables
 
-ConnmarkMatch
+NoTrackTarget
 -------------
 
-The :class:`ConnmarkMatch` class uses the same :ref:`mark_criterion` as
-the :class:`MarkMatch` class.
-
-.. autoclass:: ConnmarkMatch
+.. autoclass:: NoTrackTarget
     :members:
-    :inherited-members: Match
-
+    :inherited-members:
+    :member-order: bysource
```

### Comparing `linuxnet-iptables-6.1.0/docs/matches/conntrackmatch.rst` & `linuxnet-iptables-6.3.1/docs/matches/conntrackmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/matches/icmpmatch.rst` & `linuxnet-iptables-6.3.1/docs/matches/icmpmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/matches/limitmatch.rst` & `linuxnet-iptables-6.3.1/docs/matches/limitmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/matches/markmatch.rst` & `linuxnet-iptables-6.3.1/docs/matches/markmatch.rst`

 * *Files 0% similar despite different names*

```diff
@@ -47,8 +47,7 @@
 MarkCriterion
 ~~~~~~~~~~~~~
 
 .. autoclass:: MarkCriterion
     :class-doc-from: class
     :member-order: bysource
     :inherited-members:
-
```

### Comparing `linuxnet-iptables-6.1.0/docs/matches/ownermatch.rst` & `linuxnet-iptables-6.3.1/docs/matches/ownermatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/matches/packetmatch.rst` & `linuxnet-iptables-6.3.1/docs/matches/packetmatch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/matches/packettypematch.rst` & `linuxnet-iptables-6.3.1/docs/matches/packettypematch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/matches/statematch.rst` & `linuxnet-iptables-6.3.1/docs/matches/statematch.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/matches/tcpmatch.rst` & `linuxnet-iptables-6.3.1/docs/matches/tcpmssmatch.rst`

 * *Files 24% similar despite different names*

```diff
@@ -14,65 +14,36 @@
     
     You should have received a copy of the GNU Affero General
     Public License along with linuxnet-iptables. If not, see
     <https://www.gnu.org/licenses/>.
 
 .. currentmodule:: linuxnet.iptables
 
-TcpMatch
---------
+TcpmssMatch
+-----------
 
-.. autoclass:: TcpMatch
-    :members:
-    :inherited-members: Match
-    :member-order: bysource
+Example::
 
--------
+    >>> from linuxnet.iptables import TcpmssMatch
+    >>> m = TcpmssMatch()
+    >>> m.mss().equals(500,600)
+    <linuxnet.iptables.matches.tcpmssmatch.TcpmssMatch object at 0x7f4a19799240>
+    >>> m.to_iptables_args()
+    ['-m', 'tcpmss', '--mss', '500:600']
 
-.. currentmodule:: linuxnet.iptables.matches.tcpmatch
 
-TcpFlagsCriterion
-~~~~~~~~~~~~~~~~~
-
-.. autoclass:: TcpFlagsCriterion
-    :class-doc-from: class
-    :inherited-members:
-    :member-order: bysource
-
-.. autoclass:: TcpFlag
-    :class-doc-from: class
+.. autoclass:: TcpmssMatch
     :members:
+    :inherited-members: Match
     :member-order: bysource
 
 -------
 
-.. _source_port_criterion:
-
-SourcePortCriterion
-~~~~~~~~~~~~~~~~~~~
-
-.. autoclass:: SourcePortCriterion
-    :class-doc-from: class
-    :inherited-members:
-    :member-order: bysource
-
--------
-
-.. _dest_port_criterion:
-
-DestPortCriterion
-~~~~~~~~~~~~~~~~~
-
-.. autoclass:: DestPortCriterion
-    :class-doc-from: class
-    :inherited-members:
-    :member-order: bysource
-
--------
+.. currentmodule:: linuxnet.iptables.matches.tcpmssmatch
 
-TcpOptionCriterion
-~~~~~~~~~~~~~~~~~~
+MssCriterion
+~~~~~~~~~~~~
 
-.. autoclass:: TcpOptionCriterion
+.. autoclass:: MssCriterion
     :class-doc-from: class
     :inherited-members:
     :member-order: bysource
```

### Comparing `linuxnet-iptables-6.1.0/docs/matches/tcpmssmatch.rst` & `linuxnet-iptables-6.3.1/docs/matches/ttlmatch.rst`

 * *Files 20% similar despite different names*

```diff
@@ -14,36 +14,41 @@
     
     You should have received a copy of the GNU Affero General
     Public License along with linuxnet-iptables. If not, see
     <https://www.gnu.org/licenses/>.
 
 .. currentmodule:: linuxnet.iptables
 
-TcpmssMatch
------------
+TtlMatch
+--------
 
 Example::
 
-    >>> from linuxnet.iptables import TcpmssMatch
-    >>> m = TcpmssMatch()
-    >>> m.mss().equals(500,600)
-    <linuxnet.iptables.matches.tcpmssmatch.TcpmssMatch object at 0x7f4a19799240>
+    m linuxnet.iptables import TtlMatch
+    >>> m = TtlMatch()
+    >>> m.ttl().not_equals(32)
+    <linuxnet.iptables.match.TtlMatch object at 0x7ff96e466f60>
     >>> m.to_iptables_args()
-    ['-m', 'tcpmss', '--mss', '500:600']
+    ['-m', 'ttl', '!', '--ttl-eq', '32']
+    >>> m = TtlMatch()
+    >>> m.ttl().less_than(32)
+    <linuxnet.iptables.match.TtlMatch object at 0x7ff96e466fd0>
+    >>> m.to_iptables_args()
+    ['-m', 'ttl', '--ttl-lt', '32']
 
 
-.. autoclass:: TcpmssMatch
+.. autoclass:: TtlMatch
     :members:
     :inherited-members: Match
     :member-order: bysource
 
 -------
 
-.. currentmodule:: linuxnet.iptables.matches.tcpmssmatch
+.. currentmodule:: linuxnet.iptables.matches.ttlmatch
 
-MssCriterion
+TtlCriterion
 ~~~~~~~~~~~~
 
-.. autoclass:: MssCriterion
+.. autoclass:: TtlCriterion
     :class-doc-from: class
     :inherited-members:
     :member-order: bysource
```

### Comparing `linuxnet-iptables-6.1.0/docs/matches/ttlmatch.rst` & `linuxnet-iptables-6.3.1/docs/matches/udpmatch.rst`

 * *Files 15% similar despite different names*

```diff
@@ -14,41 +14,31 @@
     
     You should have received a copy of the GNU Affero General
     Public License along with linuxnet-iptables. If not, see
     <https://www.gnu.org/licenses/>.
 
 .. currentmodule:: linuxnet.iptables
 
-TtlMatch
+UdpMatch
 --------
 
+The :class:`UdpMatch` class uses the same
+:ref:`source_port_criterion`
+and 
+:ref:`dest_port_criterion`
+as the :class:`TcpMatch` class.
+
 Example::
 
-    m linuxnet.iptables import TtlMatch
-    >>> m = TtlMatch()
-    >>> m.ttl().not_equals(32)
-    <linuxnet.iptables.match.TtlMatch object at 0x7ff96e466f60>
-    >>> m.to_iptables_args()
-    ['-m', 'ttl', '!', '--ttl-eq', '32']
-    >>> m = TtlMatch()
-    >>> m.ttl().less_than(32)
-    <linuxnet.iptables.match.TtlMatch object at 0x7ff96e466fd0>
+    >>> from linuxnet.iptables import UdpMatch
+    >>> m = UdpMatch()
+    >>> m.dest_port().equals(53)
+    <linuxnet.iptables.match.UdpMatch object at 0x7ff96e466f98>
     >>> m.to_iptables_args()
-    ['-m', 'ttl', '--ttl-lt', '32']
+    ['-m', 'udp', '--dport', '53']
 
 
-.. autoclass:: TtlMatch
+.. autoclass:: UdpMatch
     :members:
     :inherited-members: Match
     :member-order: bysource
 
--------
-
-.. currentmodule:: linuxnet.iptables.matches.ttlmatch
-
-TtlCriterion
-~~~~~~~~~~~~
-
-.. autoclass:: TtlCriterion
-    :class-doc-from: class
-    :inherited-members:
-    :member-order: bysource
```

### Comparing `linuxnet-iptables-6.1.0/docs/matches/udpmatch.rst` & `linuxnet-iptables-6.3.1/docs/target.rst`

 * *Files 20% similar despite different names*

```diff
@@ -12,33 +12,35 @@
     or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General Public
     License for more details.
     
     You should have received a copy of the GNU Affero General
     Public License along with linuxnet-iptables. If not, see
     <https://www.gnu.org/licenses/>.
 
+.. _target:
+
+.. currentmodule:: linuxnet.iptables.extension
+
+Targets
+=======
+
+All target-related classes are derived from the :class:`Target` class.
+The following subclasses are available:
+
 .. currentmodule:: linuxnet.iptables
 
-UdpMatch
---------
+.. toctree::
+    :maxdepth: 1
+    :glob:
+
+    targets/*
+
+-------
 
-The :class:`UdpMatch` class uses the same
-:ref:`source_port_criterion`
-and 
-:ref:`dest_port_criterion`
-as the :class:`TcpMatch` class.
-
-Example::
-
-    >>> from linuxnet.iptables import UdpMatch
-    >>> m = UdpMatch()
-    >>> m.dest_port().equals(53)
-    <linuxnet.iptables.match.UdpMatch object at 0x7ff96e466f98>
-    >>> m.to_iptables_args()
-    ['-m', 'udp', '--dport', '53']
+The helper class :class:`Targets` provides access to the special 
+targets (e.g. ``ACCEPT``).
 
 
-.. autoclass:: UdpMatch
+.. autoclass:: Targets
     :members:
-    :inherited-members: Match
     :member-order: bysource
```

### Comparing `linuxnet-iptables-6.1.0/docs/rule.rst` & `linuxnet-iptables-6.3.1/docs/rule.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/table.rst` & `linuxnet-iptables-6.3.1/docs/table.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/target-example.py` & `linuxnet-iptables-6.3.1/docs/target-example.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/targets/chaintarget.rst` & `linuxnet-iptables-6.3.1/docs/targets/chaintarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/targets/connmarktarget.rst` & `linuxnet-iptables-6.3.1/docs/targets/connmarktarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/targets/dnattarget.rst` & `linuxnet-iptables-6.3.1/docs/targets/dnattarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/targets/logtarget.rst` & `linuxnet-iptables-6.3.1/docs/targets/logtarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/targets/marktarget.rst` & `linuxnet-iptables-6.3.1/docs/targets/marktarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/targets/masqueradetarget.rst` & `linuxnet-iptables-6.3.1/docs/targets/masqueradetarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/targets/notracktarget.rst` & `linuxnet-iptables-6.3.1/docs/targets/rejecttarget.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ..
-    Copyright (c) 2023, Panagiotis Tsirigotis
+    Copyright (c) 2022, 2023, Panagiotis Tsirigotis
     
     This file is part of linuxnet-iptables.
     
     linuxnet-iptables is free software: you can redistribute it and/or
     modify it under the terms of version 3 of the GNU Affero General Public
     License as published by the Free Software Foundation.
     
@@ -14,14 +14,15 @@
     
     You should have received a copy of the GNU Affero General
     Public License along with linuxnet-iptables. If not, see
     <https://www.gnu.org/licenses/>.
 
 .. currentmodule:: linuxnet.iptables
 
-NoTrackTarget
--------------
+RejectTarget
+------------
 
-.. autoclass:: NoTrackTarget
+.. autoclass:: RejectTarget
     :members:
     :inherited-members:
     :member-order: bysource
+
```

### Comparing `linuxnet-iptables-6.1.0/docs/targets/rejecttarget.rst` & `linuxnet-iptables-6.3.1/docs/targets/snattarget.rst`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     
     You should have received a copy of the GNU Affero General
     Public License along with linuxnet-iptables. If not, see
     <https://www.gnu.org/licenses/>.
 
 .. currentmodule:: linuxnet.iptables
 
-RejectTarget
-------------
+SnatTarget
+----------
 
-.. autoclass:: RejectTarget
+.. autoclass:: SnatTarget
     :members:
     :inherited-members:
     :member-order: bysource
```

### Comparing `linuxnet-iptables-6.1.0/docs/targets/snattarget.rst` & `linuxnet-iptables-6.3.1/docs/targets/ttltarget.rst`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     
     You should have received a copy of the GNU Affero General
     Public License along with linuxnet-iptables. If not, see
     <https://www.gnu.org/licenses/>.
 
 .. currentmodule:: linuxnet.iptables
 
-SnatTarget
-----------
+TtlTarget
+---------
 
-.. autoclass:: SnatTarget
+.. autoclass:: TtlTarget
     :members:
     :inherited-members:
     :member-order: bysource
```

### Comparing `linuxnet-iptables-6.1.0/docs/targets/tracetarget.rst` & `linuxnet-iptables-6.3.1/docs/targets/tracetarget.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/docs/targets/ttltarget.rst` & `linuxnet-iptables-6.3.1/linuxnet/iptables/deps.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-..
-    Copyright (c) 2022, 2023, Panagiotis Tsirigotis
-    
-    This file is part of linuxnet-iptables.
-    
-    linuxnet-iptables is free software: you can redistribute it and/or
-    modify it under the terms of version 3 of the GNU Affero General Public
-    License as published by the Free Software Foundation.
-    
-    linuxnet-iptables is distributed in the hope that it will be useful, but
-    WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
-    or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General Public
-    License for more details.
-    
-    You should have received a copy of the GNU Affero General
-    Public License along with linuxnet-iptables. If not, see
-    <https://www.gnu.org/licenses/>.
+# Copyright (c) 2022, Panagiotis Tsirigotis
 
-.. currentmodule:: linuxnet.iptables
+# This file is part of linuxnet-iptables.
+#
+# linuxnet-iptables is free software: you can redistribute it and/or
+# modify it under the terms of version 3 of the GNU Affero General Public
+# License as published by the Free Software Foundation.
+#
+# linuxnet-iptables is distributed in the hope that it will be useful, but
+# WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
+# or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General Public
+# License for more details.
+#
+# You should have received a copy of the GNU Affero General
+# Public License along with linuxnet-iptables. If not, see
+# <https://www.gnu.org/licenses/>.
 
-TtlTarget
----------
+"""Compatibility module to hide the dependency on the progutil package.
+"""
 
-.. autoclass:: TtlTarget
-    :members:
-    :inherited-members:
-    :member-order: bysource
+# pylint: disable=unused-import
 
+from logging import getLogger as get_logger
```

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/__init__.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/chain.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,17 @@
 
         :param chain_target: if ``True``, return rules where the target
             is a chain
         :param uses_goto: if ``True``, return rules that use goto
         :param match_count: if not ``None``, return rules that have that
             number of matches
         :param match: if not ``None``, return rules that have a matching
-            :class:`Match` in their match list
+            :class:`Match` in their match list; if the ``match`` has
+            no criteria set, it will match any :class:``Match``
+            instance of the **same** class
         """
         if (chain_target or uses_goto or match_count is not None or
                                                 match is not None):
             match_klass = type(None)
             if match:
                 # Perform a match class comparison
                 match_klass = type(match)
@@ -652,17 +654,18 @@
         """
         super().__init__(chain_name)
         self.__policy = policy
         self.__policy_packet_count = packet_count
         self.__policy_byte_count = byte_count
 
     def __str__(self):
-        return f'BuiltinChain({self.__real_chain_name})'
+        return f'BuiltinChain({self.get_real_name()})'
 
-    def is_builtin(self) -> bool:
+    @staticmethod
+    def is_builtin() -> bool:
         """
         :rtype: always returns ``True``
         """
         return True
 
     def get_policy(self) -> Target:
         """Returns the policy target of this builtin chain
```

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/deps.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/metadata.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, Panagiotis Tsirigotis
+# Copyright (c) 2022, 2023, Panagiotis Tsirigotis
 
 # This file is part of linuxnet-iptables.
 #
 # linuxnet-iptables is free software: you can redistribute it and/or
 # modify it under the terms of version 3 of the GNU Affero General Public
 # License as published by the Free Software Foundation.
 #
@@ -11,13 +11,17 @@
 # or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General Public
 # License for more details.
 #
 # You should have received a copy of the GNU Affero General
 # Public License along with linuxnet-iptables. If not, see
 # <https://www.gnu.org/licenses/>.
 
-"""Compatibility module to hide the dependency on the progutil package.
+"""
+Metadata information intended to be used by setup.py and the
+Sphinx conf.py
 """
 
-# pylint: disable=unused-import
+# pylint: disable=invalid-name
 
-from logging import getLogger as get_logger
+_version_ = "6.3.1"
+_author_ = "Panagiotis (Panos) Tsirigotis"
+_package_ = "linuxnet.iptables"
```

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/exceptions.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/exceptions.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/extension.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/extension.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,10 +26,14 @@
 from .exceptions import IptablesError, IptablesParsingError
 from .matches.match import (
                         Match,
                         MatchParser,
                         Criterion,
                         CriteriaExhaustedError,
                         )
-from .matches.util import BooleanCriterion, GenericCriterion
+from .matches.util import (
+                        BooleanCriterion,
+                        GenericCriterion,
+                        GenericPositiveCriterion,
+                        )
 from .parsing import LookaheadIterator, RuleFieldIterator
 from .targets.target import Target, TargetParser
```

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/__init__.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,12 +26,13 @@
 from .conntrackmatch import ConntrackMatch
 from .icmpmatch import IcmpMatch
 from .limitmatch import LimitMatch
 from .markmatch import MarkMatch
 from .ownermatch import OwnerMatch
 from .packetmatch import PacketMatch
 from .packettypematch import PacketTypeMatch
+from .recentmatch import RecentMatch
 from .statematch import StateMatch
 from .tcpmatch import TcpMatch, TcpFlag
 from .ttlmatch import TtlMatch
 from .tcpmssmatch import TcpmssMatch
 from .udpmatch import UdpMatch
```

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/addrtypematch.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/addrtypematch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/commentmatch.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/commentmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/connmarkmatch.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/connmarkmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/conntrackmatch.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/conntrackmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/icmpmatch.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/icmpmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/limitmatch.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/limitmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/markmatch.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/markmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/match.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/match.py`

 * *Files 1% similar despite different names*

```diff
@@ -422,14 +422,17 @@
                 #
                 # Newer iptables versions have the '!' as a standalone field
                 # instead of as a prefix of the value.
                 #
                 if token == '!':
                     self.__negation = token
                     self.__match_name = next(self.__iter)
+                elif token.startswith('!'):
+                    self.__negation = token[0]
+                    self.__match_name = token[1:]
                 else:
                     self.__match_name = token
                 match = None
                 klass = self._match_class_map.get(self.__match_name)
                 if klass is not None:
                     try:
                         match = klass.parse(self)
```

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/ownermatch.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/ownermatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/packetmatch.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/packetmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/packettypematch.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/packettypematch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/statematch.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/statematch.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,37 +15,30 @@
 # Public License along with linuxnet-iptables. If not, see
 # <https://www.gnu.org/licenses/>.
 
 """
 This module provides matching against the connection tracking state
 """
 
-
 from typing import Iterable
 
 from ..deps import get_logger
 
 from .match import Match, MatchParser
 from .util import GenericCriterion
 
 _logger = get_logger('linuxnet.iptables.matches.statematch')
 
 
-#
-#######################################################################
-#
-# Matching against connection tracking state
-#
-
 class StateCriterion(GenericCriterion):
     """Compare with the connection tracking state
 
     The comparison value is a string.
     """
-    def __init__(self, match):
+    def __init__(self, match: Match):
         super().__init__(match, '--state')
 
 
 class StateMatch(Match):
     """Match against the connection tracking state
 
     This match is accessed via the **state** module, but it is not clear
```

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/tcpmatch.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/tcpmatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,20 +223,22 @@
         self.__flags_crit = None
         self.__src_port_crit = None
         self.__dest_port_crit = None
         self.__tcp_option_crit = None
 
     @staticmethod
     def get_match_name() -> str:
-        """Returns the **iptables(8)** match extension name
+        """Returns the **iptables(8)** match extension name,
+        in this case, ``tcp``
         """
         return 'tcp'
 
     def get_criteria(self) -> Iterable['Criterion']:
-        """Returns the TCP match criteria: flags, source-port, dest-port
+        """Returns the TCP match criteria: flags, source-port, dest-port,
+        tcp-option
         """
         return (self.__flags_crit, self.__src_port_crit,
                         self.__dest_port_crit, self.__tcp_option_crit)
 
     def syn(self) -> TcpFlagsCriterion:
         """Criterion for matching against a SYN packet
         """
```

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/tcpmssmatch.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/tcpmssmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/ttlmatch.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/ttlmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/udpmatch.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/udpmatch.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/matches/util.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/matches/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,14 +60,26 @@
 
     def _crit_iptables_args(self) -> List[str]:
         """Convert to **iptables(8)** arguments
         """
         return [self.__option, str(self.__value)]
 
 
+class GenericPositiveCriterion(GenericCriterion):
+    """A subclass of :class:`GenericCriterion` for criteria that do
+    not support negation.
+    """
+    def not_equals(self, *args, **kwargs):
+        """Indicates that negation is not supported by raising
+        an :exc:`IptablesError`
+        """
+        raise IptablesError(
+                f'{self.get_iptables_option()} does not support negation')
+
+
 class BooleanCriterion(Criterion):
     """Helper class for criteria that test single bits.
     """
 
     def __init__(self, match: Match, iptables_option: str,
                                         supports_negation=True):
         """
```

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/metadata.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/tracetarget.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, 2023, Panagiotis Tsirigotis
+# Copyright (c) 2023, Panagiotis Tsirigotis
 
 # This file is part of linuxnet-iptables.
 #
 # linuxnet-iptables is free software: you can redistribute it and/or
 # modify it under the terms of version 3 of the GNU Affero General Public
 # License as published by the Free Software Foundation.
 #
@@ -12,16 +12,36 @@
 # License for more details.
 #
 # You should have received a copy of the GNU Affero General
 # Public License along with linuxnet-iptables. If not, see
 # <https://www.gnu.org/licenses/>.
 
 """
-Metadata information intended to be used by setup.py and the
-Sphinx conf.py
+This module provides the TraceTarget class which provides access to
+the iptables TRACE target.
 """
 
-# pylint: disable=invalid-name
+from ..deps import get_logger
 
-_version_ = "6.1.0"
-_author_ = "Panagiotis (Panos) Tsirigotis"
-_package_ = "linuxnet.iptables"
+from .target import Target, TargetParser
+
+_logger = get_logger("linuxnet.iptables.target.notracktarget")
+
+
+class TraceTarget(Target):
+    """This class provides access to the ``TRACE`` target
+    """
+    def __init__(self):
+        """The :meth:`__init__` method expects no arguments.
+        """
+        super().__init__('TRACE', terminates=False)
+
+    @classmethod
+    def parse(cls, _) -> Target:
+        """Parse the TRACE target
+
+        :meta private:
+        """
+        return TraceTarget()
+
+
+TargetParser.register_target('TRACE', TraceTarget)
```

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/parsing.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/parsing.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,24 +83,35 @@
         try:
             token = self.__next__()
             self.put_back(token)
             return token
         except StopIteration:
             return None
 
-    def put_back(self, token: str) -> None:
-        """Put back the specified token. This must be a token previously
-        returned by the iterator (identity is checked, not equality)
+    def put_back(self, token: str, *, replace_token=False) -> None:
+        """This method puts the previously returned token back to the
+        iterator, so that the token can be returned again.
+
+        :param token: the token to put back to the iterator; when
+            ``replace_token`` is ``False``, this must be **the** token
+            previously returned by the iterator: identity is checked,
+            not equality
+        :param replace_token: if ``True``, it allows ``token`` to be different
+            than then one previously returned by the iterator
         """
         if self.__cursor == len(self.__tokens):
             # Either there are no consumed tokens, or this is an attempt to
             # put back one more tokens than those already consumed.
             raise ValueError('not a consumed token')
         if token is not self.__tokens[self.__cursor]:
-            raise ValueError('wrong token')
+            if not replace_token:
+                raise ValueError(
+                    f'wrong token: expected={self.__tokens[self.__cursor]}, '
+                    f'putback={token}')
+            self.__tokens[self.__cursor] = token
         self.__cursor += 1
 
     def rewind(self, step=1) -> 'LookaheadIterator':
         """Put back last ``step`` tokens
 
         A :exc:`ValueError` will be raised if there are not enough
         tokens to put back.
```

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/rule.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -197,17 +197,38 @@
         """
         if self.__owner_chain is not None:
             raise IptablesError('attempt to replace target of active rule')
         self.__target = target
 
     def iter_match_list(self) -> Iterator[Match]:
         """Returns an iterator for the matches of this rule.
+
+        **This method is deprecated and will be removed at a future version.**
         """
         return iter(self.__match_list)
 
+    def iter_matches(self, lookfor: Optional[Match] =None) -> Iterator[Match]:
+        """Returns an iterator for the matches of this rule.
+        If ``lookfor`` is not ``None``, the iterator will return
+        :class:`Match` instances with criteria that compare equal to those of
+        the ``lookfor`` :class:`Match`; if ``lookfor`` has no criteria
+        defined, the iterator will return :class:`Match` instances of
+        the **same** type as the ``lookfor`` :class:`Match`.
+        """
+        if lookfor is None:
+            return iter(self.__match_list)
+        lookfor_klass = type(lookfor)
+        for crit in lookfor.get_criteria():
+            if crit is not None and crit.is_set():
+                # Perform a match value comparison
+                lookfor_klass = type(None)
+                break
+        return filter(lambda m: lookfor_klass is type(m) or m == lookfor,
+                        self.__match_list)
+
     def get_match_count(self) -> int:
         """Returns the number of matches.
         """
         return len(self.__match_list)
 
     def get_match_list(self) -> List[Match]:
         """Returns the match list of this rule.
```

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/table.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/table.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/__init__.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/connmarktarget.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/connmarktarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/logtarget.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/logtarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/marktarget.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/marktarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/masqueradetarget.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/masqueradetarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/nattarget.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/nattarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/notracktarget.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/notracktarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/rejecttarget.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/rejecttarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/target.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/target.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet/iptables/targets/ttltarget.py` & `linuxnet-iptables-6.3.1/linuxnet/iptables/targets/ttltarget.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/linuxnet_iptables.egg-info/PKG-INFO` & `linuxnet-iptables-6.3.1/linuxnet_iptables.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxnet-iptables
-Version: 6.1.0
+Version: 6.3.1
 Summary: programmatic access to Linux iptables
 Home-page: https://gitlab.com/panos-tools/linuxnet-iptables
 Author: Panagiotis (Panos) Tsirigotis
 Author-email: ptsirigotis01@gmail.com
 License: AGPLv3
 Project-URL: Source, https://gitlab.com/panos-tools/linuxnet-iptables
 Project-URL: Documentation, https://linuxnet-iptables.readthedocs.io/en/latest/index.html
@@ -31,15 +31,15 @@
 For the following examples, Python3 (3.6 or later) is required.
 
 ```python
 >>> from linuxnet.iptables import IptablesPacketFilterTable
 >>> table = IptablesPacketFilterTable('filter')
 >>> table.read_system_config()
 >>> input_chain = table.get_chain('INPUT')
->>> for rule in input_chain.get_rules():
+>>> for rule in input_chain:
 ...    print(' '.join(rule.to_iptables_args()))
 ...
 -j prod_bad_traffic
 -m state --state RELATED,ESTABLISHED -j ACCEPT
 -j prod_ingress
 -j prod_INPUT_ldrop
 >>>
@@ -66,15 +66,15 @@
 ...    output = f.read()
 ...
 >>> from linuxnet.iptables import IptablesPacketFilterTable
 >>> table = IptablesPacketFilterTable('filter')
 >>> table.init_from_output(output)
 True
 >>> input_chain = table.get_chain('INPUT')
->>> for rule in input_chain.get_rules():
+>>> for rule in input_chain:
 ...     print(' '.join(rule.to_iptables_args()))
 ...
 -j prod_bad_traffic
 -m state --state RELATED,ESTABLISHED -j ACCEPT
 -j prod_ingress
 -j prod_INPUT_ldrop
 >>>
```

### Comparing `linuxnet-iptables-6.1.0/linuxnet_iptables.egg-info/SOURCES.txt` & `linuxnet-iptables-6.3.1/linuxnet_iptables.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 docs/matches/conntrackmatch.rst
 docs/matches/icmpmatch.rst
 docs/matches/limitmatch.rst
 docs/matches/markmatch.rst
 docs/matches/ownermatch.rst
 docs/matches/packetmatch.rst
 docs/matches/packettypematch.rst
+docs/matches/recentmatch.rst
 docs/matches/statematch.rst
 docs/matches/tcpmatch.rst
 docs/matches/tcpmssmatch.rst
 docs/matches/ttlmatch.rst
 docs/matches/udpmatch.rst
 docs/targets/chaintarget.rst
 docs/targets/connmarktarget.rst
@@ -62,14 +63,15 @@
 linuxnet/iptables/matches/icmpmatch.py
 linuxnet/iptables/matches/limitmatch.py
 linuxnet/iptables/matches/markmatch.py
 linuxnet/iptables/matches/match.py
 linuxnet/iptables/matches/ownermatch.py
 linuxnet/iptables/matches/packetmatch.py
 linuxnet/iptables/matches/packettypematch.py
+linuxnet/iptables/matches/recentmatch.py
 linuxnet/iptables/matches/statematch.py
 linuxnet/iptables/matches/tcpmatch.py
 linuxnet/iptables/matches/tcpmssmatch.py
 linuxnet/iptables/matches/ttlmatch.py
 linuxnet/iptables/matches/udpmatch.py
 linuxnet/iptables/matches/util.py
 linuxnet/iptables/targets/__init__.py
```

### Comparing `linuxnet-iptables-6.1.0/setup.py` & `linuxnet-iptables-6.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `linuxnet-iptables-6.1.0/tests/iptables_test.py` & `linuxnet-iptables-6.3.1/tests/iptables_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,15 @@
                 TcpmssMatch, TcpMatch,
                 UdpMatch, IcmpMatch,
                 PacketTypeMatch,
                 ConnmarkMatch,
                 LimitMatch,
                 OwnerMatch,
                 PacketMatch,
+                RecentMatch,
                 MatchNone,
                 )
 
 root_logger = logging.getLogger()
 root_logger.addHandler(logging.FileHandler('test.log', 'w'))
 root_logger.setLevel(logging.INFO)
 
@@ -372,14 +373,89 @@
                 self.assertEqual(len(match_list), 2)
                 match = match_list[-1]
                 self.assertTrue(isinstance(match, IcmpMatch))
                 icmp_type = match.icmp_type()
                 self.assertTrue(icmp_type.is_positive() and
                                 icmp_type.get_type_value() == 3)
 
+
+    def test_parsing_recent_match(self):
+        """Parse output that uses recent match
+        """
+        output = """\
+Chain INPUT (policy DROP 0 packets, 0 bytes)
+    pkts      bytes target     prot opt in     out     source               destination
+       0        0 LOG        all  --  *      *       0.0.0.0/0            0.0.0.0/0           recent: CHECK TTL-Match name: foobar side: source LOG flags 0 level 4
+       0        0 LOG        all  --  *      *       0.0.0.0/0            0.0.0.0/0           !recent: SET name: foobar side: source LOG flags 0 level 4
+       0        0 MARK       all  --  *      *       0.0.0.0/0            0.0.0.0/0           recent: REMOVE name: foobar side: destMARK set 0xa
+       0        0            all  --  *      *       0.0.0.0/0            0.0.0.0/0           !recent: UPDATE seconds: 4 hit_count: 3 name: foobar side: source
+       0        0 LOG        all  --  *      *       0.0.0.0/0            0.0.0.0/0           recent: REMOVE name: foobar side: dest/* silly */ LOG flags 0 level 4
+""" + '\n' + self.EMPTY_FORWARD + '\n' + self.EMPTY_OUTPUT
+        pft = IptablesPacketFilterTable('filter')
+        self.assertTrue(pft.init_from_output(output))
+        input_chain = pft.get_builtin_chain('INPUT')
+        self.assertEqual(input_chain.get_rule_count(), 5)
+        for rule in input_chain:
+            rulenum = rule.get_rulenum()
+            if rulenum == 1:
+                match = next(iter(rule))
+                self.assertTrue(isinstance(match, RecentMatch))
+                action = match.action()
+                self.assertTrue(action.is_positive() and
+                    action.get_value() == RecentMatch.CHECK)
+                self.assertTrue(match.same_ttl().is_positive())
+                self.assertTrue(match.name().get_value() == 'foobar')
+                self.assertTrue(
+                        match.address_selection().get_value() ==
+                                        RecentMatch.SOURCE_ADDRESS)
+            elif rulenum == 2:
+                match = next(iter(rule))
+                self.assertTrue(isinstance(match, RecentMatch))
+                action = match.action()
+                self.assertTrue(not action.is_positive() and
+                    action.get_value() == RecentMatch.SET)
+                self.assertTrue(match.name().get_value() == 'foobar')
+                self.assertTrue(
+                        match.address_selection().get_value() ==
+                                        RecentMatch.SOURCE_ADDRESS)
+            elif rulenum == 3:
+                match = next(iter(rule))
+                self.assertTrue(isinstance(match, RecentMatch))
+                action = match.action()
+                self.assertTrue(action.is_positive() and
+                    action.get_value() == RecentMatch.REMOVE)
+                self.assertTrue(match.name().get_value() == 'foobar')
+                self.assertTrue(
+                        match.address_selection().get_value() ==
+                                        RecentMatch.DEST_ADDRESS)
+                self.assertTrue(
+                    rule.get_target().get_target_name() == 'MARK')
+            elif rulenum == 4:
+                match = next(iter(rule))
+                self.assertTrue(isinstance(match, RecentMatch))
+                action = match.action()
+                self.assertTrue(not action.is_positive() and
+                    action.get_value() == RecentMatch.UPDATE)
+                self.assertTrue(match.name().get_value() == 'foobar')
+                self.assertTrue(match.seconds().get_value() == 4)
+                self.assertTrue(match.hitcount().get_value() == 3)
+                self.assertTrue(
+                        match.address_selection().get_value() ==
+                                        RecentMatch.SOURCE_ADDRESS)
+            elif rulenum == 5:
+                self.assertEqual(rule.get_match_count(), 2)
+                match_list = rule.get_match_list()
+                match = match_list[0]
+                self.assertTrue(isinstance(match, RecentMatch))
+                action = match.action()
+                self.assertTrue(action.is_positive() and
+                    action.get_value() == RecentMatch.REMOVE)
+                self.assertTrue(match.name().get_value() == 'foobar')
+                self.assertTrue(isinstance(match_list[1], CommentMatch))
+
     def test_parsing_owner_match(self):
         """Parse output with match related to UID/GID
         """
         output = self.EMPTY_INPUT + '\n' + self.EMPTY_FORWARD + '\n' + \
 """\
 Chain OUTPUT (policy DROP 0 packets, 0 bytes)
     pkts      bytes target     prot opt in     out     source               destination
```

