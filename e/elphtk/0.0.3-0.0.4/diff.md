# Comparing `tmp/elphtk-0.0.3.tar.gz` & `tmp/elphtk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elphtk-0.0.3.tar", last modified: Fri Jul 14 15:44:38 2023, max compression
+gzip compressed data, was "elphtk-0.0.4.tar", last modified: Fri Jul 14 15:51:49 2023, max compression
```

## Comparing `elphtk-0.0.3.tar` & `elphtk-0.0.4.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:44:38.042288 elphtk-0.0.3/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:44:37.578282 elphtk-0.0.3/Examples/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      973 2023-07-12 08:22:30.000000 elphtk-0.0.3/Examples/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:44:37.686283 elphtk-0.0.3/Examples/example1/
--rw-r--r--   0 zsh       (1000) zsh       (1000)    11162 2023-06-17 09:08:46.000000 elphtk-0.0.3/Examples/example1/FORCE_SETS
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      104 2023-07-12 08:24:25.000000 elphtk-0.0.3/Examples/example1/README
--rw-r--r--   0 zsh       (1000) zsh       (1000)      124 2023-06-17 09:08:46.000000 elphtk-0.0.3/Examples/example1/band.conf
--rw-r--r--   0 zsh       (1000) zsh       (1000)   105801 2023-06-17 09:09:17.000000 elphtk-0.0.3/Examples/example1/band.yaml
--rw-r--r--   0 zsh       (1000) zsh       (1000)    29529 2023-07-12 08:23:11.000000 elphtk-0.0.3/Examples/example1/phonopy.freq.gp
--rw-r--r--   0 zsh       (1000) zsh       (1000)     9381 2023-06-17 09:09:22.000000 elphtk-0.0.3/Examples/example1/phonopy.yaml
--rw-r--r--   0 zsh       (1000) zsh       (1000)     9576 2023-06-17 09:08:46.000000 elphtk-0.0.3/Examples/example1/phonopy_disp.yaml
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:44:37.750284 elphtk-0.0.3/Examples/example2/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      110 2023-07-12 08:25:32.000000 elphtk-0.0.3/Examples/example2/README
--rw-r--r--   0 zsh       (1000) zsh       (1000)      237 2023-06-17 10:19:20.000000 elphtk-0.0.3/Examples/example2/ZrN.dyn0
--rw-r--r--   0 zsh       (1000) zsh       (1000)     8701 2023-06-17 10:19:20.000000 elphtk-0.0.3/Examples/example2/ZrN.dyn1
--rw-r--r--   0 zsh       (1000) zsh       (1000)    20620 2023-06-17 10:19:21.000000 elphtk-0.0.3/Examples/example2/ZrN.dyn2
--rw-r--r--   0 zsh       (1000) zsh       (1000)    20620 2023-06-17 10:19:21.000000 elphtk-0.0.3/Examples/example2/ZrN.dyn3
--rw-r--r--   0 zsh       (1000) zsh       (1000)    45660 2023-06-17 10:19:21.000000 elphtk-0.0.3/Examples/example2/ZrN.fc
--rw-r--r--   0 zsh       (1000) zsh       (1000)    14862 2023-06-17 10:19:21.000000 elphtk-0.0.3/Examples/example2/ZrN.freq
--rw-r--r--   0 zsh       (1000) zsh       (1000)    12194 2023-06-17 10:19:21.000000 elphtk-0.0.3/Examples/example2/ZrN.freq.gp
--rw-r--r--   0 zsh       (1000) zsh       (1000)      260 2023-06-17 11:04:38.000000 elphtk-0.0.3/Examples/example2/matdyn.in
--rw-r--r--   0 zsh       (1000) zsh       (1000)      193 2023-06-17 10:19:19.000000 elphtk-0.0.3/Examples/example2/ph.in
--rw-r--r--   0 zsh       (1000) zsh       (1000)   141685 2023-06-17 10:19:20.000000 elphtk-0.0.3/Examples/example2/ph.out
--rw-r--r--   0 zsh       (1000) zsh       (1000)       75 2023-06-17 10:19:19.000000 elphtk-0.0.3/Examples/example2/q2r.in
--rw-r--r--   0 zsh       (1000) zsh       (1000)      702 2023-06-17 10:19:19.000000 elphtk-0.0.3/Examples/example2/scf.in
--rw-r--r--   0 zsh       (1000) zsh       (1000)    19082 2023-06-17 10:19:20.000000 elphtk-0.0.3/Examples/example2/scf.out
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:44:37.862286 elphtk-0.0.3/Examples/example3/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      245 2023-07-12 08:47:33.000000 elphtk-0.0.3/Examples/example3/README
--rw-r--r--   0 zsh       (1000) zsh       (1000)    66919 2023-06-17 10:51:28.000000 elphtk-0.0.3/Examples/example3/ZrN.a2f
--rw-r--r--   0 zsh       (1000) zsh       (1000)    66919 2023-06-17 10:51:28.000000 elphtk-0.0.3/Examples/example3/ZrN.a2f.01
--rw-r--r--   0 zsh       (1000) zsh       (1000)    84566 2023-06-17 10:51:29.000000 elphtk-0.0.3/Examples/example3/ZrN.a2f_iso
--rw-r--r--   0 zsh       (1000) zsh       (1000)    66919 2023-06-17 10:51:30.000000 elphtk-0.0.3/Examples/example3/ZrN.a2f_tr.01
--rw-r--r--   0 zsh       (1000) zsh       (1000)     1539 2023-06-17 10:52:20.000000 elphtk-0.0.3/Examples/example3/ZrN.kmap
--rw-r--r--   0 zsh       (1000) zsh       (1000)    52726 2023-06-17 12:30:29.000000 elphtk-0.0.3/Examples/example3/ZrN.lambda_FS
--rw-r--r--   0 zsh       (1000) zsh       (1000)     3483 2023-06-17 10:52:21.000000 elphtk-0.0.3/Examples/example3/ZrN.lambda_k_pairs
--rw-r--r--   0 zsh       (1000) zsh       (1000)    19565 2023-06-17 10:52:35.000000 elphtk-0.0.3/Examples/example3/ZrN.nnkp
--rw-r--r--   0 zsh       (1000) zsh       (1000)    81500 2023-06-17 11:00:13.000000 elphtk-0.0.3/Examples/example3/ZrN.phdos
--rw-r--r--   0 zsh       (1000) zsh       (1000)    66500 2023-06-17 10:52:35.000000 elphtk-0.0.3/Examples/example3/ZrN.phdos.01
--rw-r--r--   0 zsh       (1000) zsh       (1000)   104000 2023-06-17 10:59:04.000000 elphtk-0.0.3/Examples/example3/ZrN.phdos_proj
--rw-r--r--   0 zsh       (1000) zsh       (1000)    13131 2023-06-17 12:31:01.000000 elphtk-0.0.3/Examples/example3/ZrN.res.01
--rw-r--r--   0 zsh       (1000) zsh       (1000)     2324 2023-06-17 10:52:40.000000 elphtk-0.0.3/Examples/example3/ZrN.win
--rw-r--r--   0 zsh       (1000) zsh       (1000)     2144 2023-06-17 14:20:25.000000 elphtk-0.0.3/Examples/example3/epw.in
--rw-r--r--   0 zsh       (1000) zsh       (1000)     4947 2023-06-17 10:49:58.000000 elphtk-0.0.3/Examples/example3/nscf.in
--rw-r--r--   0 zsh       (1000) zsh       (1000)    70036 2023-06-17 10:50:00.000000 elphtk-0.0.3/Examples/example3/nscf.out
--rw-r--r--   0 zsh       (1000) zsh       (1000)      720 2023-06-17 10:49:58.000000 elphtk-0.0.3/Examples/example3/scf.in
--rw-r--r--   0 zsh       (1000) zsh       (1000)    19082 2023-06-17 10:50:00.000000 elphtk-0.0.3/Examples/example3/scf.out
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:44:37.874286 elphtk-0.0.3/Examples/example4/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      118 2023-07-12 09:06:35.000000 elphtk-0.0.3/Examples/example4/README
--rw-rw-r--   0 zsh       (1000) zsh       (1000)    23760 2023-07-12 09:21:26.000000 elphtk-0.0.3/Examples/example4/freq.txt
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:44:37.946287 elphtk-0.0.3/Examples/example4/tmp/
--rw-r--r--   0 zsh       (1000) zsh       (1000)    48744 2023-06-17 11:02:44.000000 elphtk-0.0.3/Examples/example4/tmp/ZrN.egnv
--rw-r--r--   0 zsh       (1000) zsh       (1000)   179728 2023-06-17 13:11:51.000000 elphtk-0.0.3/Examples/example4/tmp/ZrN.ephmat1
--rw-r--r--   0 zsh       (1000) zsh       (1000)    32272 2023-06-17 11:02:44.000000 elphtk-0.0.3/Examples/example4/tmp/ZrN.freq
--rw-r--r--   0 zsh       (1000) zsh       (1000)    15564 2023-06-17 13:25:15.000000 elphtk-0.0.3/Examples/example4/tmp/ZrN.ikmap
--rw-r--r--   0 zsh       (1000) zsh       (1000)     1058 2023-06-17 07:04:09.000000 elphtk-0.0.3/LICENSE.txt
--rw-r--r--   0 zsh       (1000) zsh       (1000)      161 2023-06-17 14:16:37.000000 elphtk-0.0.3/MANIFEST.in
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      285 2023-07-14 15:44:38.042288 elphtk-0.0.3/PKG-INFO
--rw-r--r--   0 zsh       (1000) zsh       (1000)     1881 2023-06-17 16:00:40.000000 elphtk-0.0.3/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:44:38.018288 elphtk-0.0.3/elphtk/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      299 2023-07-12 11:58:22.000000 elphtk-0.0.3/elphtk/__init__.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)    14279 2023-07-12 08:41:38.000000 elphtk-0.0.3/elphtk/arguments.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)    14600 2023-07-12 11:58:08.000000 elphtk-0.0.3/elphtk/epw_binary.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)    26823 2023-07-12 11:57:39.000000 elphtk-0.0.3/elphtk/epw_tool.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)     7603 2023-07-14 15:42:22.000000 elphtk-0.0.3/elphtk/phonon_plot.py
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     1571 2023-07-14 15:43:22.000000 elphtk-0.0.3/elphtk/phonopy_phonon.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)      404 2023-06-18 05:08:44.000000 elphtk-0.0.3/elphtk/pkg_info.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)     9906 2023-07-12 08:39:33.000000 elphtk-0.0.3/elphtk/qe_phonon.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)     3922 2023-07-12 08:39:49.000000 elphtk-0.0.3/elphtk/wgauss.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:44:38.022288 elphtk-0.0.3/elphtk.egg-info/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      285 2023-07-14 15:44:37.000000 elphtk-0.0.3/elphtk.egg-info/PKG-INFO
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     1767 2023-07-14 15:44:37.000000 elphtk-0.0.3/elphtk.egg-info/SOURCES.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-07-14 15:44:37.000000 elphtk-0.0.3/elphtk.egg-info/dependency_links.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-07-14 15:44:37.000000 elphtk-0.0.3/elphtk.egg-info/requires.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)        7 2023-07-14 15:44:37.000000 elphtk-0.0.3/elphtk.egg-info/top_level.txt
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:44:38.038288 elphtk-0.0.3/scripts/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3066 2023-07-14 15:43:49.000000 elphtk-0.0.3/scripts/phplot
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7181 2023-07-12 11:54:15.000000 elphtk-0.0.3/scripts/post_epw
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    10991 2023-07-12 09:02:25.000000 elphtk-0.0.3/scripts/qe2epw
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13693 2023-07-12 08:39:06.000000 elphtk-0.0.3/scripts/qe_lambda
--rw-r--r--   0 zsh       (1000) zsh       (1000)      574 2023-07-14 15:44:38.042288 elphtk-0.0.3/setup.cfg
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2626 2023-07-14 15:44:21.000000 elphtk-0.0.3/setup.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:51:49.963554 elphtk-0.0.4/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:51:49.947554 elphtk-0.0.4/Examples/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      973 2023-07-12 08:22:30.000000 elphtk-0.0.4/Examples/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:51:49.951554 elphtk-0.0.4/Examples/example1/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    11162 2023-06-17 09:08:46.000000 elphtk-0.0.4/Examples/example1/FORCE_SETS
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      104 2023-07-12 08:24:25.000000 elphtk-0.0.4/Examples/example1/README
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      124 2023-06-17 09:08:46.000000 elphtk-0.0.4/Examples/example1/band.conf
+-rw-r--r--   0 zsh       (1000) zsh       (1000)   105801 2023-06-17 09:09:17.000000 elphtk-0.0.4/Examples/example1/band.yaml
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    29529 2023-07-12 08:23:11.000000 elphtk-0.0.4/Examples/example1/phonopy.freq.gp
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     9381 2023-06-17 09:09:22.000000 elphtk-0.0.4/Examples/example1/phonopy.yaml
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     9576 2023-06-17 09:08:46.000000 elphtk-0.0.4/Examples/example1/phonopy_disp.yaml
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:51:49.951554 elphtk-0.0.4/Examples/example2/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      110 2023-07-12 08:25:32.000000 elphtk-0.0.4/Examples/example2/README
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      237 2023-06-17 10:19:20.000000 elphtk-0.0.4/Examples/example2/ZrN.dyn0
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     8701 2023-06-17 10:19:20.000000 elphtk-0.0.4/Examples/example2/ZrN.dyn1
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    20620 2023-06-17 10:19:21.000000 elphtk-0.0.4/Examples/example2/ZrN.dyn2
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    20620 2023-06-17 10:19:21.000000 elphtk-0.0.4/Examples/example2/ZrN.dyn3
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    45660 2023-06-17 10:19:21.000000 elphtk-0.0.4/Examples/example2/ZrN.fc
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    14862 2023-06-17 10:19:21.000000 elphtk-0.0.4/Examples/example2/ZrN.freq
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    12194 2023-06-17 10:19:21.000000 elphtk-0.0.4/Examples/example2/ZrN.freq.gp
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      260 2023-06-17 11:04:38.000000 elphtk-0.0.4/Examples/example2/matdyn.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      193 2023-06-17 10:19:19.000000 elphtk-0.0.4/Examples/example2/ph.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)   141685 2023-06-17 10:19:20.000000 elphtk-0.0.4/Examples/example2/ph.out
+-rw-r--r--   0 zsh       (1000) zsh       (1000)       75 2023-06-17 10:19:19.000000 elphtk-0.0.4/Examples/example2/q2r.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      702 2023-06-17 10:19:19.000000 elphtk-0.0.4/Examples/example2/scf.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    19082 2023-06-17 10:19:20.000000 elphtk-0.0.4/Examples/example2/scf.out
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:51:49.955554 elphtk-0.0.4/Examples/example3/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      245 2023-07-12 08:47:33.000000 elphtk-0.0.4/Examples/example3/README
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    66919 2023-06-17 10:51:28.000000 elphtk-0.0.4/Examples/example3/ZrN.a2f
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    66919 2023-06-17 10:51:28.000000 elphtk-0.0.4/Examples/example3/ZrN.a2f.01
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    84566 2023-06-17 10:51:29.000000 elphtk-0.0.4/Examples/example3/ZrN.a2f_iso
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    66919 2023-06-17 10:51:30.000000 elphtk-0.0.4/Examples/example3/ZrN.a2f_tr.01
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     1539 2023-06-17 10:52:20.000000 elphtk-0.0.4/Examples/example3/ZrN.kmap
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    52726 2023-06-17 12:30:29.000000 elphtk-0.0.4/Examples/example3/ZrN.lambda_FS
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     3483 2023-06-17 10:52:21.000000 elphtk-0.0.4/Examples/example3/ZrN.lambda_k_pairs
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    19565 2023-06-17 10:52:35.000000 elphtk-0.0.4/Examples/example3/ZrN.nnkp
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    81500 2023-06-17 11:00:13.000000 elphtk-0.0.4/Examples/example3/ZrN.phdos
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    66500 2023-06-17 10:52:35.000000 elphtk-0.0.4/Examples/example3/ZrN.phdos.01
+-rw-r--r--   0 zsh       (1000) zsh       (1000)   104000 2023-06-17 10:59:04.000000 elphtk-0.0.4/Examples/example3/ZrN.phdos_proj
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    13131 2023-06-17 12:31:01.000000 elphtk-0.0.4/Examples/example3/ZrN.res.01
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     2324 2023-06-17 10:52:40.000000 elphtk-0.0.4/Examples/example3/ZrN.win
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     2144 2023-06-17 14:20:25.000000 elphtk-0.0.4/Examples/example3/epw.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     4947 2023-06-17 10:49:58.000000 elphtk-0.0.4/Examples/example3/nscf.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    70036 2023-06-17 10:50:00.000000 elphtk-0.0.4/Examples/example3/nscf.out
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      720 2023-06-17 10:49:58.000000 elphtk-0.0.4/Examples/example3/scf.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    19082 2023-06-17 10:50:00.000000 elphtk-0.0.4/Examples/example3/scf.out
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:51:49.959554 elphtk-0.0.4/Examples/example4/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      118 2023-07-12 09:06:35.000000 elphtk-0.0.4/Examples/example4/README
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)    23760 2023-07-12 09:21:26.000000 elphtk-0.0.4/Examples/example4/freq.txt
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:51:49.959554 elphtk-0.0.4/Examples/example4/tmp/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    48744 2023-06-17 11:02:44.000000 elphtk-0.0.4/Examples/example4/tmp/ZrN.egnv
+-rw-r--r--   0 zsh       (1000) zsh       (1000)   179728 2023-06-17 13:11:51.000000 elphtk-0.0.4/Examples/example4/tmp/ZrN.ephmat1
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    32272 2023-06-17 11:02:44.000000 elphtk-0.0.4/Examples/example4/tmp/ZrN.freq
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    15564 2023-06-17 13:25:15.000000 elphtk-0.0.4/Examples/example4/tmp/ZrN.ikmap
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     1058 2023-06-17 07:04:09.000000 elphtk-0.0.4/LICENSE.txt
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      161 2023-06-17 14:16:37.000000 elphtk-0.0.4/MANIFEST.in
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      285 2023-07-14 15:51:49.963554 elphtk-0.0.4/PKG-INFO
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     1881 2023-06-17 16:00:40.000000 elphtk-0.0.4/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:51:49.959554 elphtk-0.0.4/elphtk/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      299 2023-07-14 15:49:55.000000 elphtk-0.0.4/elphtk/__init__.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    14279 2023-07-12 08:41:38.000000 elphtk-0.0.4/elphtk/arguments.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    14600 2023-07-12 11:58:08.000000 elphtk-0.0.4/elphtk/epw_binary.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    26823 2023-07-12 11:57:39.000000 elphtk-0.0.4/elphtk/epw_tool.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     7603 2023-07-14 15:42:22.000000 elphtk-0.0.4/elphtk/phonon_plot.py
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     2681 2023-07-14 15:49:48.000000 elphtk-0.0.4/elphtk/phonopy_phonon.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      404 2023-06-18 05:08:44.000000 elphtk-0.0.4/elphtk/pkg_info.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     9906 2023-07-12 08:39:33.000000 elphtk-0.0.4/elphtk/qe_phonon.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     3922 2023-07-12 08:39:49.000000 elphtk-0.0.4/elphtk/wgauss.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:51:49.963554 elphtk-0.0.4/elphtk.egg-info/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      285 2023-07-14 15:51:49.000000 elphtk-0.0.4/elphtk.egg-info/PKG-INFO
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     1767 2023-07-14 15:51:49.000000 elphtk-0.0.4/elphtk.egg-info/SOURCES.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-07-14 15:51:49.000000 elphtk-0.0.4/elphtk.egg-info/dependency_links.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-07-14 15:51:49.000000 elphtk-0.0.4/elphtk.egg-info/requires.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)        7 2023-07-14 15:51:49.000000 elphtk-0.0.4/elphtk.egg-info/top_level.txt
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-14 15:51:49.963554 elphtk-0.0.4/scripts/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3066 2023-07-14 15:43:49.000000 elphtk-0.0.4/scripts/phplot
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7181 2023-07-12 11:54:15.000000 elphtk-0.0.4/scripts/post_epw
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    10991 2023-07-12 09:02:25.000000 elphtk-0.0.4/scripts/qe2epw
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13693 2023-07-12 08:39:06.000000 elphtk-0.0.4/scripts/qe_lambda
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      574 2023-07-14 15:51:49.963554 elphtk-0.0.4/setup.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2626 2023-07-14 15:51:43.000000 elphtk-0.0.4/setup.py
```

### Comparing `elphtk-0.0.3/Examples/README.md` & `elphtk-0.0.4/Examples/README.md`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example1/FORCE_SETS` & `elphtk-0.0.4/Examples/example1/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example1/band.yaml` & `elphtk-0.0.4/Examples/example1/band.yaml`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example1/phonopy.freq.gp` & `elphtk-0.0.4/Examples/example1/phonopy.freq.gp`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example1/phonopy.yaml` & `elphtk-0.0.4/Examples/example1/phonopy.yaml`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example1/phonopy_disp.yaml` & `elphtk-0.0.4/Examples/example1/phonopy_disp.yaml`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example2/ZrN.dyn1` & `elphtk-0.0.4/Examples/example2/ZrN.dyn1`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example2/ZrN.dyn2` & `elphtk-0.0.4/Examples/example2/ZrN.dyn2`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example2/ZrN.dyn3` & `elphtk-0.0.4/Examples/example2/ZrN.dyn3`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example2/ZrN.fc` & `elphtk-0.0.4/Examples/example2/ZrN.fc`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example2/ZrN.freq` & `elphtk-0.0.4/Examples/example2/ZrN.freq`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example2/ZrN.freq.gp` & `elphtk-0.0.4/Examples/example2/ZrN.freq.gp`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example2/ph.out` & `elphtk-0.0.4/Examples/example2/ph.out`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example2/scf.in` & `elphtk-0.0.4/Examples/example2/scf.in`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example2/scf.out` & `elphtk-0.0.4/Examples/example2/scf.out`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example3/ZrN.a2f` & `elphtk-0.0.4/Examples/example3/ZrN.a2f`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example3/ZrN.a2f.01` & `elphtk-0.0.4/Examples/example3/ZrN.a2f.01`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example3/ZrN.a2f_iso` & `elphtk-0.0.4/Examples/example3/ZrN.a2f_iso`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example3/ZrN.a2f_tr.01` & `elphtk-0.0.4/Examples/example3/ZrN.a2f_tr.01`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example3/ZrN.kmap` & `elphtk-0.0.4/Examples/example3/ZrN.kmap`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example3/ZrN.lambda_FS` & `elphtk-0.0.4/Examples/example3/ZrN.lambda_FS`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example3/ZrN.lambda_k_pairs` & `elphtk-0.0.4/Examples/example3/ZrN.lambda_k_pairs`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example3/ZrN.nnkp` & `elphtk-0.0.4/Examples/example3/ZrN.nnkp`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example3/ZrN.phdos` & `elphtk-0.0.4/Examples/example3/ZrN.phdos`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example3/ZrN.phdos.01` & `elphtk-0.0.4/Examples/example3/ZrN.phdos.01`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example3/ZrN.phdos_proj` & `elphtk-0.0.4/Examples/example3/ZrN.phdos_proj`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example3/ZrN.res.01` & `elphtk-0.0.4/Examples/example3/ZrN.res.01`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example3/ZrN.win` & `elphtk-0.0.4/Examples/example3/ZrN.win`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example3/epw.in` & `elphtk-0.0.4/Examples/example3/epw.in`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example3/nscf.in` & `elphtk-0.0.4/Examples/example3/nscf.in`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example3/nscf.out` & `elphtk-0.0.4/Examples/example3/nscf.out`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example3/scf.in` & `elphtk-0.0.4/Examples/example3/scf.in`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example3/scf.out` & `elphtk-0.0.4/Examples/example3/scf.out`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example4/freq.txt` & `elphtk-0.0.4/Examples/example4/freq.txt`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example4/tmp/ZrN.egnv` & `elphtk-0.0.4/Examples/example4/tmp/ZrN.egnv`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example4/tmp/ZrN.ephmat1` & `elphtk-0.0.4/Examples/example4/tmp/ZrN.ephmat1`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example4/tmp/ZrN.freq` & `elphtk-0.0.4/Examples/example4/tmp/ZrN.freq`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/Examples/example4/tmp/ZrN.ikmap` & `elphtk-0.0.4/Examples/example4/tmp/ZrN.ikmap`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/LICENSE.txt` & `elphtk-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/README.md` & `elphtk-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/elphtk/arguments.py` & `elphtk-0.0.4/elphtk/arguments.py`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/elphtk/epw_binary.py` & `elphtk-0.0.4/elphtk/epw_binary.py`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/elphtk/epw_tool.py` & `elphtk-0.0.4/elphtk/epw_tool.py`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/elphtk/phonon_plot.py` & `elphtk-0.0.4/elphtk/phonon_plot.py`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/elphtk/qe_phonon.py` & `elphtk-0.0.4/elphtk/qe_phonon.py`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/elphtk/wgauss.py` & `elphtk-0.0.4/elphtk/wgauss.py`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/elphtk.egg-info/SOURCES.txt` & `elphtk-0.0.4/elphtk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/scripts/phplot` & `elphtk-0.0.4/scripts/phplot`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/scripts/post_epw` & `elphtk-0.0.4/scripts/post_epw`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/scripts/qe2epw` & `elphtk-0.0.4/scripts/qe2epw`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/scripts/qe_lambda` & `elphtk-0.0.4/scripts/qe_lambda`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.3/setup.cfg` & `elphtk-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = elphtk
-version = 0.0.3
+version = 0.0.4
 author = Shunhong Zhang
 author_email = zhangshunhong.pku@gmail.com
 keywords = [Python,Phonon,Electron-phonon]
 py_modules = core_modules
 license = MIT License
 description = Python library for (electron)-phonon-related analysis
 long_desc = An open-source Python library for phonon-related data processing
```

### Comparing `elphtk-0.0.3/setup.py` & `elphtk-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 scripts_pysupercell = glob.glob('scripts/*')
 
 long_desc="An open-source Python library for phonon-related data processing"
 
 
 kwargs_setup=dict(
 name='elphtk',
-version='0.0.3',
+version='0.0.4',
 author='Shunhong Zhang',
 author_email='zhangshunhong.pku@gmail.com',
 url='https://pypi.org/project/elphtk',
 download_url='https://pypi.org/project/elphtk',
 keywords=['Python','Phonon','Electron-phonon'],
 py_modules=core_modules,
 license="MIT License",
```

