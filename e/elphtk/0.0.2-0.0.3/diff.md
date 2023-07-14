# Comparing `tmp/elphtk-0.0.2.tar.gz` & `tmp/elphtk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elphtk-0.0.2.tar", last modified: Wed Jul 12 09:18:57 2023, max compression
+gzip compressed data, was "elphtk-0.0.3.tar", last modified: Fri Jul 14 15:44:38 2023, max compression
```

## Comparing `elphtk-0.0.2.tar` & `elphtk-0.0.3.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-12 09:18:57.142871 elphtk-0.0.2/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-12 09:18:57.122871 elphtk-0.0.2/Examples/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      973 2023-07-12 08:22:30.000000 elphtk-0.0.2/Examples/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-12 09:18:57.126871 elphtk-0.0.2/Examples/example1/
--rw-r--r--   0 zsh       (1000) zsh       (1000)    11162 2023-06-17 09:08:46.000000 elphtk-0.0.2/Examples/example1/FORCE_SETS
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      104 2023-07-12 08:24:25.000000 elphtk-0.0.2/Examples/example1/README
--rw-r--r--   0 zsh       (1000) zsh       (1000)      124 2023-06-17 09:08:46.000000 elphtk-0.0.2/Examples/example1/band.conf
--rw-r--r--   0 zsh       (1000) zsh       (1000)   105801 2023-06-17 09:09:17.000000 elphtk-0.0.2/Examples/example1/band.yaml
--rw-r--r--   0 zsh       (1000) zsh       (1000)    29529 2023-07-12 08:23:11.000000 elphtk-0.0.2/Examples/example1/phonopy.freq.gp
--rw-r--r--   0 zsh       (1000) zsh       (1000)     9381 2023-06-17 09:09:22.000000 elphtk-0.0.2/Examples/example1/phonopy.yaml
--rw-r--r--   0 zsh       (1000) zsh       (1000)     9576 2023-06-17 09:08:46.000000 elphtk-0.0.2/Examples/example1/phonopy_disp.yaml
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-12 09:18:57.130871 elphtk-0.0.2/Examples/example2/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      110 2023-07-12 08:25:32.000000 elphtk-0.0.2/Examples/example2/README
--rw-r--r--   0 zsh       (1000) zsh       (1000)      237 2023-06-17 10:19:20.000000 elphtk-0.0.2/Examples/example2/ZrN.dyn0
--rw-r--r--   0 zsh       (1000) zsh       (1000)     8701 2023-06-17 10:19:20.000000 elphtk-0.0.2/Examples/example2/ZrN.dyn1
--rw-r--r--   0 zsh       (1000) zsh       (1000)    20620 2023-06-17 10:19:21.000000 elphtk-0.0.2/Examples/example2/ZrN.dyn2
--rw-r--r--   0 zsh       (1000) zsh       (1000)    20620 2023-06-17 10:19:21.000000 elphtk-0.0.2/Examples/example2/ZrN.dyn3
--rw-r--r--   0 zsh       (1000) zsh       (1000)    45660 2023-06-17 10:19:21.000000 elphtk-0.0.2/Examples/example2/ZrN.fc
--rw-r--r--   0 zsh       (1000) zsh       (1000)    14862 2023-06-17 10:19:21.000000 elphtk-0.0.2/Examples/example2/ZrN.freq
--rw-r--r--   0 zsh       (1000) zsh       (1000)    12194 2023-06-17 10:19:21.000000 elphtk-0.0.2/Examples/example2/ZrN.freq.gp
--rw-r--r--   0 zsh       (1000) zsh       (1000)      260 2023-06-17 11:04:38.000000 elphtk-0.0.2/Examples/example2/matdyn.in
--rw-r--r--   0 zsh       (1000) zsh       (1000)      193 2023-06-17 10:19:19.000000 elphtk-0.0.2/Examples/example2/ph.in
--rw-r--r--   0 zsh       (1000) zsh       (1000)   141685 2023-06-17 10:19:20.000000 elphtk-0.0.2/Examples/example2/ph.out
--rw-r--r--   0 zsh       (1000) zsh       (1000)       75 2023-06-17 10:19:19.000000 elphtk-0.0.2/Examples/example2/q2r.in
--rw-r--r--   0 zsh       (1000) zsh       (1000)      702 2023-06-17 10:19:19.000000 elphtk-0.0.2/Examples/example2/scf.in
--rw-r--r--   0 zsh       (1000) zsh       (1000)    19082 2023-06-17 10:19:20.000000 elphtk-0.0.2/Examples/example2/scf.out
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-12 09:18:57.138871 elphtk-0.0.2/Examples/example3/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      245 2023-07-12 08:47:33.000000 elphtk-0.0.2/Examples/example3/README
--rw-r--r--   0 zsh       (1000) zsh       (1000)    66919 2023-06-17 10:51:28.000000 elphtk-0.0.2/Examples/example3/ZrN.a2f
--rw-r--r--   0 zsh       (1000) zsh       (1000)    66919 2023-06-17 10:51:28.000000 elphtk-0.0.2/Examples/example3/ZrN.a2f.01
--rw-r--r--   0 zsh       (1000) zsh       (1000)    84566 2023-06-17 10:51:29.000000 elphtk-0.0.2/Examples/example3/ZrN.a2f_iso
--rw-r--r--   0 zsh       (1000) zsh       (1000)    66919 2023-06-17 10:51:30.000000 elphtk-0.0.2/Examples/example3/ZrN.a2f_tr.01
--rw-r--r--   0 zsh       (1000) zsh       (1000)     1539 2023-06-17 10:52:20.000000 elphtk-0.0.2/Examples/example3/ZrN.kmap
--rw-r--r--   0 zsh       (1000) zsh       (1000)    52726 2023-06-17 12:30:29.000000 elphtk-0.0.2/Examples/example3/ZrN.lambda_FS
--rw-r--r--   0 zsh       (1000) zsh       (1000)     3483 2023-06-17 10:52:21.000000 elphtk-0.0.2/Examples/example3/ZrN.lambda_k_pairs
--rw-r--r--   0 zsh       (1000) zsh       (1000)    19565 2023-06-17 10:52:35.000000 elphtk-0.0.2/Examples/example3/ZrN.nnkp
--rw-r--r--   0 zsh       (1000) zsh       (1000)    81500 2023-06-17 11:00:13.000000 elphtk-0.0.2/Examples/example3/ZrN.phdos
--rw-r--r--   0 zsh       (1000) zsh       (1000)    66500 2023-06-17 10:52:35.000000 elphtk-0.0.2/Examples/example3/ZrN.phdos.01
--rw-r--r--   0 zsh       (1000) zsh       (1000)   104000 2023-06-17 10:59:04.000000 elphtk-0.0.2/Examples/example3/ZrN.phdos_proj
--rw-r--r--   0 zsh       (1000) zsh       (1000)    13131 2023-06-17 12:31:01.000000 elphtk-0.0.2/Examples/example3/ZrN.res.01
--rw-r--r--   0 zsh       (1000) zsh       (1000)     2324 2023-06-17 10:52:40.000000 elphtk-0.0.2/Examples/example3/ZrN.win
--rw-r--r--   0 zsh       (1000) zsh       (1000)     2144 2023-06-17 14:20:25.000000 elphtk-0.0.2/Examples/example3/epw.in
--rw-r--r--   0 zsh       (1000) zsh       (1000)     4947 2023-06-17 10:49:58.000000 elphtk-0.0.2/Examples/example3/nscf.in
--rw-r--r--   0 zsh       (1000) zsh       (1000)    70036 2023-06-17 10:50:00.000000 elphtk-0.0.2/Examples/example3/nscf.out
--rw-r--r--   0 zsh       (1000) zsh       (1000)      720 2023-06-17 10:49:58.000000 elphtk-0.0.2/Examples/example3/scf.in
--rw-r--r--   0 zsh       (1000) zsh       (1000)    19082 2023-06-17 10:50:00.000000 elphtk-0.0.2/Examples/example3/scf.out
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-12 09:18:57.138871 elphtk-0.0.2/Examples/example4/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      118 2023-07-12 09:06:35.000000 elphtk-0.0.2/Examples/example4/README
--rw-rw-r--   0 zsh       (1000) zsh       (1000)    23760 2023-07-12 09:06:43.000000 elphtk-0.0.2/Examples/example4/freq.txt
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-12 09:18:57.138871 elphtk-0.0.2/Examples/example4/tmp/
--rw-r--r--   0 zsh       (1000) zsh       (1000)    48744 2023-06-17 11:02:44.000000 elphtk-0.0.2/Examples/example4/tmp/ZrN.egnv
--rw-r--r--   0 zsh       (1000) zsh       (1000)   179728 2023-06-17 13:11:51.000000 elphtk-0.0.2/Examples/example4/tmp/ZrN.ephmat1
--rw-r--r--   0 zsh       (1000) zsh       (1000)    32272 2023-06-17 11:02:44.000000 elphtk-0.0.2/Examples/example4/tmp/ZrN.freq
--rw-r--r--   0 zsh       (1000) zsh       (1000)    15564 2023-06-17 13:25:15.000000 elphtk-0.0.2/Examples/example4/tmp/ZrN.ikmap
--rw-r--r--   0 zsh       (1000) zsh       (1000)     1058 2023-06-17 07:04:09.000000 elphtk-0.0.2/LICENSE.txt
--rw-r--r--   0 zsh       (1000) zsh       (1000)      161 2023-06-17 14:16:37.000000 elphtk-0.0.2/MANIFEST.in
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      285 2023-07-12 09:18:57.142871 elphtk-0.0.2/PKG-INFO
--rw-r--r--   0 zsh       (1000) zsh       (1000)     1881 2023-06-17 16:00:40.000000 elphtk-0.0.2/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-12 09:18:57.142871 elphtk-0.0.2/elphtk/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      299 2023-07-12 09:18:30.000000 elphtk-0.0.2/elphtk/__init__.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)    14279 2023-07-12 08:41:38.000000 elphtk-0.0.2/elphtk/arguments.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)    14325 2023-07-12 09:05:50.000000 elphtk-0.0.2/elphtk/epw_binary.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)    26012 2023-07-12 08:55:02.000000 elphtk-0.0.2/elphtk/epw_tool.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)     7603 2023-06-17 15:57:41.000000 elphtk-0.0.2/elphtk/phonon_plot.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)      404 2023-06-18 05:08:44.000000 elphtk-0.0.2/elphtk/pkg_info.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)     9906 2023-07-12 08:39:33.000000 elphtk-0.0.2/elphtk/qe_phonon.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)     3922 2023-07-12 08:39:49.000000 elphtk-0.0.2/elphtk/wgauss.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-12 09:18:57.142871 elphtk-0.0.2/elphtk.egg-info/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      285 2023-07-12 09:18:56.000000 elphtk-0.0.2/elphtk.egg-info/PKG-INFO
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     1742 2023-07-12 09:18:57.000000 elphtk-0.0.2/elphtk.egg-info/SOURCES.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-07-12 09:18:56.000000 elphtk-0.0.2/elphtk.egg-info/dependency_links.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-07-12 09:18:56.000000 elphtk-0.0.2/elphtk.egg-info/requires.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)        7 2023-07-12 09:18:56.000000 elphtk-0.0.2/elphtk.egg-info/top_level.txt
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-12 09:18:57.142871 elphtk-0.0.2/scripts/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5655 2023-07-12 08:39:15.000000 elphtk-0.0.2/scripts/phplot
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6960 2023-07-12 09:05:46.000000 elphtk-0.0.2/scripts/post_epw
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    10991 2023-07-12 09:02:25.000000 elphtk-0.0.2/scripts/qe2epw
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13693 2023-07-12 08:39:06.000000 elphtk-0.0.2/scripts/qe_lambda
--rw-r--r--   0 zsh       (1000) zsh       (1000)      574 2023-07-12 09:18:57.146871 elphtk-0.0.2/setup.cfg
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2608 2023-07-12 09:16:39.000000 elphtk-0.0.2/setup.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:44:38.042288 elphtk-0.0.3/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:44:37.578282 elphtk-0.0.3/Examples/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      973 2023-07-12 08:22:30.000000 elphtk-0.0.3/Examples/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:44:37.686283 elphtk-0.0.3/Examples/example1/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    11162 2023-06-17 09:08:46.000000 elphtk-0.0.3/Examples/example1/FORCE_SETS
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      104 2023-07-12 08:24:25.000000 elphtk-0.0.3/Examples/example1/README
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      124 2023-06-17 09:08:46.000000 elphtk-0.0.3/Examples/example1/band.conf
+-rw-r--r--   0 zsh       (1000) zsh       (1000)   105801 2023-06-17 09:09:17.000000 elphtk-0.0.3/Examples/example1/band.yaml
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    29529 2023-07-12 08:23:11.000000 elphtk-0.0.3/Examples/example1/phonopy.freq.gp
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     9381 2023-06-17 09:09:22.000000 elphtk-0.0.3/Examples/example1/phonopy.yaml
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     9576 2023-06-17 09:08:46.000000 elphtk-0.0.3/Examples/example1/phonopy_disp.yaml
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:44:37.750284 elphtk-0.0.3/Examples/example2/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      110 2023-07-12 08:25:32.000000 elphtk-0.0.3/Examples/example2/README
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      237 2023-06-17 10:19:20.000000 elphtk-0.0.3/Examples/example2/ZrN.dyn0
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     8701 2023-06-17 10:19:20.000000 elphtk-0.0.3/Examples/example2/ZrN.dyn1
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    20620 2023-06-17 10:19:21.000000 elphtk-0.0.3/Examples/example2/ZrN.dyn2
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    20620 2023-06-17 10:19:21.000000 elphtk-0.0.3/Examples/example2/ZrN.dyn3
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    45660 2023-06-17 10:19:21.000000 elphtk-0.0.3/Examples/example2/ZrN.fc
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    14862 2023-06-17 10:19:21.000000 elphtk-0.0.3/Examples/example2/ZrN.freq
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    12194 2023-06-17 10:19:21.000000 elphtk-0.0.3/Examples/example2/ZrN.freq.gp
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      260 2023-06-17 11:04:38.000000 elphtk-0.0.3/Examples/example2/matdyn.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      193 2023-06-17 10:19:19.000000 elphtk-0.0.3/Examples/example2/ph.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)   141685 2023-06-17 10:19:20.000000 elphtk-0.0.3/Examples/example2/ph.out
+-rw-r--r--   0 zsh       (1000) zsh       (1000)       75 2023-06-17 10:19:19.000000 elphtk-0.0.3/Examples/example2/q2r.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      702 2023-06-17 10:19:19.000000 elphtk-0.0.3/Examples/example2/scf.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    19082 2023-06-17 10:19:20.000000 elphtk-0.0.3/Examples/example2/scf.out
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:44:37.862286 elphtk-0.0.3/Examples/example3/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      245 2023-07-12 08:47:33.000000 elphtk-0.0.3/Examples/example3/README
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    66919 2023-06-17 10:51:28.000000 elphtk-0.0.3/Examples/example3/ZrN.a2f
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    66919 2023-06-17 10:51:28.000000 elphtk-0.0.3/Examples/example3/ZrN.a2f.01
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    84566 2023-06-17 10:51:29.000000 elphtk-0.0.3/Examples/example3/ZrN.a2f_iso
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    66919 2023-06-17 10:51:30.000000 elphtk-0.0.3/Examples/example3/ZrN.a2f_tr.01
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     1539 2023-06-17 10:52:20.000000 elphtk-0.0.3/Examples/example3/ZrN.kmap
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    52726 2023-06-17 12:30:29.000000 elphtk-0.0.3/Examples/example3/ZrN.lambda_FS
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     3483 2023-06-17 10:52:21.000000 elphtk-0.0.3/Examples/example3/ZrN.lambda_k_pairs
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    19565 2023-06-17 10:52:35.000000 elphtk-0.0.3/Examples/example3/ZrN.nnkp
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    81500 2023-06-17 11:00:13.000000 elphtk-0.0.3/Examples/example3/ZrN.phdos
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    66500 2023-06-17 10:52:35.000000 elphtk-0.0.3/Examples/example3/ZrN.phdos.01
+-rw-r--r--   0 zsh       (1000) zsh       (1000)   104000 2023-06-17 10:59:04.000000 elphtk-0.0.3/Examples/example3/ZrN.phdos_proj
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    13131 2023-06-17 12:31:01.000000 elphtk-0.0.3/Examples/example3/ZrN.res.01
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     2324 2023-06-17 10:52:40.000000 elphtk-0.0.3/Examples/example3/ZrN.win
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     2144 2023-06-17 14:20:25.000000 elphtk-0.0.3/Examples/example3/epw.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     4947 2023-06-17 10:49:58.000000 elphtk-0.0.3/Examples/example3/nscf.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    70036 2023-06-17 10:50:00.000000 elphtk-0.0.3/Examples/example3/nscf.out
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      720 2023-06-17 10:49:58.000000 elphtk-0.0.3/Examples/example3/scf.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    19082 2023-06-17 10:50:00.000000 elphtk-0.0.3/Examples/example3/scf.out
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:44:37.874286 elphtk-0.0.3/Examples/example4/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      118 2023-07-12 09:06:35.000000 elphtk-0.0.3/Examples/example4/README
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)    23760 2023-07-12 09:21:26.000000 elphtk-0.0.3/Examples/example4/freq.txt
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:44:37.946287 elphtk-0.0.3/Examples/example4/tmp/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    48744 2023-06-17 11:02:44.000000 elphtk-0.0.3/Examples/example4/tmp/ZrN.egnv
+-rw-r--r--   0 zsh       (1000) zsh       (1000)   179728 2023-06-17 13:11:51.000000 elphtk-0.0.3/Examples/example4/tmp/ZrN.ephmat1
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    32272 2023-06-17 11:02:44.000000 elphtk-0.0.3/Examples/example4/tmp/ZrN.freq
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    15564 2023-06-17 13:25:15.000000 elphtk-0.0.3/Examples/example4/tmp/ZrN.ikmap
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     1058 2023-06-17 07:04:09.000000 elphtk-0.0.3/LICENSE.txt
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      161 2023-06-17 14:16:37.000000 elphtk-0.0.3/MANIFEST.in
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      285 2023-07-14 15:44:38.042288 elphtk-0.0.3/PKG-INFO
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     1881 2023-06-17 16:00:40.000000 elphtk-0.0.3/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:44:38.018288 elphtk-0.0.3/elphtk/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      299 2023-07-12 11:58:22.000000 elphtk-0.0.3/elphtk/__init__.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    14279 2023-07-12 08:41:38.000000 elphtk-0.0.3/elphtk/arguments.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    14600 2023-07-12 11:58:08.000000 elphtk-0.0.3/elphtk/epw_binary.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    26823 2023-07-12 11:57:39.000000 elphtk-0.0.3/elphtk/epw_tool.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     7603 2023-07-14 15:42:22.000000 elphtk-0.0.3/elphtk/phonon_plot.py
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     1571 2023-07-14 15:43:22.000000 elphtk-0.0.3/elphtk/phonopy_phonon.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      404 2023-06-18 05:08:44.000000 elphtk-0.0.3/elphtk/pkg_info.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     9906 2023-07-12 08:39:33.000000 elphtk-0.0.3/elphtk/qe_phonon.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     3922 2023-07-12 08:39:49.000000 elphtk-0.0.3/elphtk/wgauss.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:44:38.022288 elphtk-0.0.3/elphtk.egg-info/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      285 2023-07-14 15:44:37.000000 elphtk-0.0.3/elphtk.egg-info/PKG-INFO
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     1767 2023-07-14 15:44:37.000000 elphtk-0.0.3/elphtk.egg-info/SOURCES.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-07-14 15:44:37.000000 elphtk-0.0.3/elphtk.egg-info/dependency_links.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-07-14 15:44:37.000000 elphtk-0.0.3/elphtk.egg-info/requires.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)        7 2023-07-14 15:44:37.000000 elphtk-0.0.3/elphtk.egg-info/top_level.txt
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:44:38.038288 elphtk-0.0.3/scripts/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3066 2023-07-14 15:43:49.000000 elphtk-0.0.3/scripts/phplot
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7181 2023-07-12 11:54:15.000000 elphtk-0.0.3/scripts/post_epw
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    10991 2023-07-12 09:02:25.000000 elphtk-0.0.3/scripts/qe2epw
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13693 2023-07-12 08:39:06.000000 elphtk-0.0.3/scripts/qe_lambda
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      574 2023-07-14 15:44:38.042288 elphtk-0.0.3/setup.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2626 2023-07-14 15:44:21.000000 elphtk-0.0.3/setup.py
```

### Comparing `elphtk-0.0.2/Examples/README.md` & `elphtk-0.0.3/Examples/README.md`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example1/FORCE_SETS` & `elphtk-0.0.3/Examples/example1/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example1/band.yaml` & `elphtk-0.0.3/Examples/example1/band.yaml`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example1/phonopy.freq.gp` & `elphtk-0.0.3/Examples/example1/phonopy.freq.gp`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example1/phonopy.yaml` & `elphtk-0.0.3/Examples/example1/phonopy.yaml`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example1/phonopy_disp.yaml` & `elphtk-0.0.3/Examples/example1/phonopy_disp.yaml`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example2/ZrN.dyn1` & `elphtk-0.0.3/Examples/example2/ZrN.dyn1`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example2/ZrN.dyn2` & `elphtk-0.0.3/Examples/example2/ZrN.dyn2`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example2/ZrN.dyn3` & `elphtk-0.0.3/Examples/example2/ZrN.dyn3`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example2/ZrN.fc` & `elphtk-0.0.3/Examples/example2/ZrN.fc`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example2/ZrN.freq` & `elphtk-0.0.3/Examples/example2/ZrN.freq`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example2/ZrN.freq.gp` & `elphtk-0.0.3/Examples/example2/ZrN.freq.gp`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example2/ph.out` & `elphtk-0.0.3/Examples/example2/ph.out`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example2/scf.in` & `elphtk-0.0.3/Examples/example2/scf.in`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example2/scf.out` & `elphtk-0.0.3/Examples/example2/scf.out`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example3/ZrN.a2f` & `elphtk-0.0.3/Examples/example3/ZrN.a2f`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example3/ZrN.a2f.01` & `elphtk-0.0.3/Examples/example3/ZrN.a2f.01`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example3/ZrN.a2f_iso` & `elphtk-0.0.3/Examples/example3/ZrN.a2f_iso`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example3/ZrN.a2f_tr.01` & `elphtk-0.0.3/Examples/example3/ZrN.a2f_tr.01`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example3/ZrN.kmap` & `elphtk-0.0.3/Examples/example3/ZrN.kmap`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example3/ZrN.lambda_FS` & `elphtk-0.0.3/Examples/example3/ZrN.lambda_FS`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example3/ZrN.lambda_k_pairs` & `elphtk-0.0.3/Examples/example3/ZrN.lambda_k_pairs`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example3/ZrN.nnkp` & `elphtk-0.0.3/Examples/example3/ZrN.nnkp`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example3/ZrN.phdos` & `elphtk-0.0.3/Examples/example3/ZrN.phdos`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example3/ZrN.phdos.01` & `elphtk-0.0.3/Examples/example3/ZrN.phdos.01`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example3/ZrN.phdos_proj` & `elphtk-0.0.3/Examples/example3/ZrN.phdos_proj`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example3/ZrN.res.01` & `elphtk-0.0.3/Examples/example3/ZrN.res.01`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example3/ZrN.win` & `elphtk-0.0.3/Examples/example3/ZrN.win`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example3/epw.in` & `elphtk-0.0.3/Examples/example3/epw.in`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example3/nscf.in` & `elphtk-0.0.3/Examples/example3/nscf.in`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example3/nscf.out` & `elphtk-0.0.3/Examples/example3/nscf.out`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example3/scf.in` & `elphtk-0.0.3/Examples/example3/scf.in`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example3/scf.out` & `elphtk-0.0.3/Examples/example3/scf.out`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example4/freq.txt` & `elphtk-0.0.3/Examples/example4/freq.txt`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example4/tmp/ZrN.egnv` & `elphtk-0.0.3/Examples/example4/tmp/ZrN.egnv`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example4/tmp/ZrN.ephmat1` & `elphtk-0.0.3/Examples/example4/tmp/ZrN.ephmat1`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example4/tmp/ZrN.freq` & `elphtk-0.0.3/Examples/example4/tmp/ZrN.freq`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/Examples/example4/tmp/ZrN.ikmap` & `elphtk-0.0.3/Examples/example4/tmp/ZrN.ikmap`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/LICENSE.txt` & `elphtk-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/README.md` & `elphtk-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/elphtk/arguments.py` & `elphtk-0.0.3/elphtk/arguments.py`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/elphtk/epw_binary.py` & `elphtk-0.0.3/elphtk/epw_binary.py`

 * *Files 9% similar despite different names*

```diff
@@ -96,14 +96,35 @@
         ekfs[ik,:len(idx)]=ekf_[ik][idx]
     print ('ef  ={:15.8f} eV\nef0 ={:15.8f} eV'.format(ef,ef0))
     print ('min eigenval = {:10.5f}\nmax eigenval = {:10.5f} eV'.format(np.min(ekf_),np.max(ekf_)))
     grid_params = (nkftot,nkf1,nkf2,nkf3,nkfs,nbndfs)
     en_params = (ef,ef0,dosef,degaussw,fsthick)
     return grid_params,en_params,wkfs,xkfs,ekfs
 
+
+
+def write_grid_params(grid_params,file=None):
+    nkftot,nkf1,nkf2,nkf3,nkfs,nbndfs = grid_params
+    print ('# nkftot = {:4d}'.format(nkftot),file=file)
+    print ('# nkf1 = {:4d}'.format(nkf1),file=file)
+    print ('# nkf2 = {:4d}'.format(nkf2),file=file)
+    print ('# nkf3 = {:4d}'.format(nkf3),file=file)
+    print ('# nkfs = {:4d}'.format(nkfs),file=file)
+    print ('# nbndfs = {:4d}'.format(nbndfs),file=file)
+
+
+def write_en_params(en_params,file=None):
+    ef,ef0,dosef,degaussw,fsthick = en_params
+    print ('# Ef = {:10.5f}'.format(ef),file=file)
+    print ('# Ef0 = {:10.5f}'.format(ef0),file=file)
+    print ('# DOS_Ef = {:10.5f}'.format(dosef),file=file)
+    print ('# DeGaussW = {:10.5f}'.format(degaussw),file=file)
+    print ('# FS_thick = {:10.5f}'.format(fsthick),file=file)
+ 
+
     
 def gen_xkff(nkf1,nkf2,nkf3):
     xx=np.linspace(0,1,nkf1,endpoint=False)
     yy=np.linspace(0,1,nkf2,endpoint=False)
     zz=np.linspace(0,1,nkf3,endpoint=False)
     y,z,x = np.meshgrid(yy,zz,xx)
     nkftot=np.prod([nkf1,nkf2,nkf3])
@@ -117,31 +138,14 @@
         nkf_mesh = int(nkf_mesh)
         ixkf=np.zeros(nkf_mesh,int)
         for ik in range(nkf_mesh):
             ixkf[ik]=f.read_record('i4')
     return ixkf
 
 
-def plot_nkfs(nkf1,nkf2,nkf3,ixkf,ekfs):
-    # only works for 2D systems
-    idx=np.where(ixkf!=0)[0]
-    nkfs=len(idx)
-    xkff=gen_xkff(nkf1,nkf2,nkf3)
-    import matplotlib.pyplot as plt
-    colors=['r','g','b','c','m','orange']
-    nbnd=ekfs.shape[1]
-    fig,ax=plt.subplots(1,nbnd,figsize=(4*nbnd,4))
-    for i in range(ekfs.shape[1]):
-        ax[i].scatter(xkff[idx][:,0],xkff[idx][:,1],s=30,facecolor=colors[i],edgecolor='none')
-    fig.tight_layout()
-    plt.show()
-    fig.savefig('nkfs',dpi=500)
-    return fig,ax
-
-
 def read_nks(outdir='tmp',prefix='wannier90',seedname='wannier90'):
     get_ephmat = glob.glob('{}/{}.ephmat*'.format(outdir,seedname))
     npool = len(get_ephmat)
     nks=np.zeros(npool,int)
     for ipool in range(npool):
         with fortio.FortranFile('{0}/{1}.ephmat{2}'.format(outdir,seedname,ipool+1)) as f:
             pool_id,nks[ipool] = f.read_record('i4',shape=2)
@@ -377,7 +381,8 @@
     nlines = get_ephmat_lines(outdir=outdir,prefix=prefix,seedname=seedname)
     if rank==0: print('\nReading ephmat: {:5d} pools'.format(npool))
     start,last=assign_task(npool,size,rank)
     for ii,i in enumerate(range(start,last)):
         read_ephmat_one_pool(i+1,nks,ef0,fsthick,ekfs,ixkqf,nqfs,nbndfs,nnq,nlines,
         outdir=outdir,seedname=seedname,prefix=prefix,eps_acustic=eps_acustic)
     comm.barrier()
+
```

### Comparing `elphtk-0.0.2/elphtk/epw_tool.py` & `elphtk-0.0.3/elphtk/epw_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -665,7 +665,33 @@
         if i==ax.shape[0]-1:    ax[i,j].set_xlabel('$\omega\ \mathrm{(meV)}$')
         if j==0:    ax[i,j].set_ylabel('$\Delta\ \mathrm{(meV)}$')
     fig.tight_layout()
     fig.savefig('gap_freq',dpi=args.dpi)
     if args.show_plot: plt.show()
     return fig
 
+
+def gen_xkff(nkf1,nkf2,nkf3):
+    xx=np.linspace(0,1,nkf1,endpoint=False)
+    yy=np.linspace(0,1,nkf2,endpoint=False)
+    zz=np.linspace(0,1,nkf3,endpoint=False)
+    y,z,x = np.meshgrid(yy,zz,xx)
+    nkftot=np.prod([nkf1,nkf2,nkf3])
+    xkff=np.array([x.T,y.T,z.T]).reshape(3,nkftot).T
+    return xkff
+
+
+def plot_nkfs(nkf1,nkf2,nkf3,ixkf,ekfs,show=False):
+    # only works for 2D systems
+    idx=np.where(ixkf!=0)[0]
+    nkfs=len(idx)
+    xkff=gen_xkff(nkf1,nkf2,nkf3)
+
+    colors=['r','g','b','c','m','orange']
+    nbnd=ekfs.shape[1]
+    fig,ax=plt.subplots(1,nbnd,figsize=(4*nbnd,4))
+    for i in range(ekfs.shape[1]):
+        ax[i].scatter(xkff[idx][:,0],xkff[idx][:,1],s=30,facecolor=colors[i],edgecolor='none')
+    fig.tight_layout()
+    fig.savefig('nkfs',dpi=500)
+    if show: plt.show()
+    return fig
```

### Comparing `elphtk-0.0.2/elphtk/phonon_plot.py` & `elphtk-0.0.3/elphtk/phonon_plot.py`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/elphtk/qe_phonon.py` & `elphtk-0.0.3/elphtk/qe_phonon.py`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/elphtk/wgauss.py` & `elphtk-0.0.3/elphtk/wgauss.py`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/elphtk.egg-info/SOURCES.txt` & `elphtk-0.0.3/elphtk.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 Examples/example4/tmp/ZrN.freq
 Examples/example4/tmp/ZrN.ikmap
 elphtk/__init__.py
 elphtk/arguments.py
 elphtk/epw_binary.py
 elphtk/epw_tool.py
 elphtk/phonon_plot.py
+elphtk/phonopy_phonon.py
 elphtk/pkg_info.py
 elphtk/qe_phonon.py
 elphtk/wgauss.py
 elphtk.egg-info/PKG-INFO
 elphtk.egg-info/SOURCES.txt
 elphtk.egg-info/dependency_links.txt
 elphtk.egg-info/requires.txt
```

### Comparing `elphtk-0.0.2/scripts/post_epw` & `elphtk-0.0.3/scripts/post_epw`

 * *Files 11% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 'mpi_elph',
 'freq',
 'kqmap_demo',
 None,
 ]
 
 
-def main():
+def main(kws):
     print ('{0}\n'.format(desc_str))
     print_task_list(task_list)
     print ('task=',args.task)
     if   args.task==None:               dryrun()
     elif args.task=='a2f':              plot_a2f(args)
     elif args.task=='wan_band':         plot_wan_band(args)
     elif args.task=='gap':              plot_gap(args)
@@ -156,14 +156,18 @@
     elif args.task=='lambda.phself':    plot_lambda.phself(args)
     elif args.task=='specfun':          plot_specfun(args)
     elif args.task=='specfun_sup':      plot_specfun_sup(args)
     elif args.task=='phdos':            plot_phdos(args)
     elif args.task=='kqmap_demo':       test_kpmq()
     elif args.task=='elph':             read_elph(**kws)
     elif args.task=='mpi_elph':         mpi_read_elph(**kws)
+    elif args.task=='engv':             
+        grid_params,en_params,wkfs,xkfs,ekfs = read_egnv(outdir=args.outdir,seedname=args.seedname)
+        write_grid_params(grid_params)
+        write_en_params(en_params)
     elif args.task=='freq':
         qpts,freqs = read_freq_scipy(**kws)
         qpts,freqs = read_freq(**kws)
         write_freq(qpts,freqs)
     else: exit('Unavaialble taks {} specified!'.format(args.task))
 
 
@@ -181,8 +185,8 @@
 if __name__=='__main__':
     from elphtk import __version__
     from elphtk.pkg_info import verbose_pkg_info
     verbose_pkg_info(__version__)
     print (__note__)
     print ('nqf1,nqf2,nqf3 = {},{},{}'.format(nqf1,nqf2,nqf3))
     print ('Change them if necessary')
-    main()
+    main(kws)
```

### Comparing `elphtk-0.0.2/scripts/qe2epw` & `elphtk-0.0.3/scripts/qe2epw`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/scripts/qe_lambda` & `elphtk-0.0.3/scripts/qe_lambda`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.2/setup.cfg` & `elphtk-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = elphtk
-version = 0.0.2
+version = 0.0.3
 author = Shunhong Zhang
 author_email = zhangshunhong.pku@gmail.com
 keywords = [Python,Phonon,Electron-phonon]
 py_modules = core_modules
 license = MIT License
 description = Python library for (electron)-phonon-related analysis
 long_desc = An open-source Python library for phonon-related data processing
```

### Comparing `elphtk-0.0.2/setup.py` & `elphtk-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,28 +48,29 @@
 
 core_modules=[
 'arguments',
 'epw_binary',
 'epw_tool',
 'wgauss',
 'qe_phonon',
+'phonopy_phonon',
 'phonon_plot',
 'pkg_info',
 '__init__',
 ]
 
 core_modules = ['elphtk/{}'.format(item) for item in core_modules]
 scripts_pysupercell = glob.glob('scripts/*')
 
 long_desc="An open-source Python library for phonon-related data processing"
 
 
 kwargs_setup=dict(
 name='elphtk',
-version='0.0.2',
+version='0.0.3',
 author='Shunhong Zhang',
 author_email='zhangshunhong.pku@gmail.com',
 url='https://pypi.org/project/elphtk',
 download_url='https://pypi.org/project/elphtk',
 keywords=['Python','Phonon','Electron-phonon'],
 py_modules=core_modules,
 license="MIT License",
```

