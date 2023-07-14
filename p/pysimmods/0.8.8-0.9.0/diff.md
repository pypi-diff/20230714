# Comparing `tmp/pysimmods-0.8.8.tar.gz` & `tmp/pysimmods-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysimmods-0.8.8.tar", last modified: Thu Nov 10 10:52:48 2022, max compression
+gzip compressed data, was "pysimmods-0.9.0.tar", last modified: Fri Jul 14 14:27:32 2023, max compression
```

## Comparing `pysimmods-0.8.8.tar` & `pysimmods-0.9.0.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.355517 pysimmods-0.8.8/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     7648 2022-04-06 06:55:56.000000 pysimmods-0.8.8/LICENSE
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       91 2022-04-06 06:55:56.000000 pysimmods-0.8.8/MANIFEST.in
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     2172 2022-11-10 10:52:48.355517 pysimmods-0.8.8/PKG-INFO
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1139 2022-06-21 08:49:04.000000 pysimmods-0.8.8/README.md
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        5 2022-11-10 10:52:21.000000 pysimmods-0.8.8/VERSION
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       38 2022-11-10 10:52:48.355517 pysimmods-0.8.8/setup.cfg
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1826 2022-06-08 06:10:12.000000 pysimmods-0.8.8/setup.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.345516 pysimmods-0.8.8/src/
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.345516 pysimmods-0.8.8/src/pysimmods/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/__init__.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.345516 pysimmods-0.8.8/src/pysimmods/buffer/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/buffer/__init__.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.345516 pysimmods-0.8.8/src/pysimmods/buffer/batterysim/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       29 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/buffer/batterysim/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     5630 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/buffer/batterysim/battery.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     2352 2022-06-15 11:10:38.000000 pysimmods-0.8.8/src/pysimmods/buffer/batterysim/config.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      354 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/buffer/batterysim/inputs.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      514 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/buffer/batterysim/presets.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1532 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/buffer/batterysim/state.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.345516 pysimmods-0.8.8/src/pysimmods/consumer/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/consumer/__init__.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.345516 pysimmods-0.8.8/src/pysimmods/consumer/hvacsim/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       74 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/consumer/hvacsim/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     3040 2022-04-06 07:13:10.000000 pysimmods-0.8.8/src/pysimmods/consumer/hvacsim/config.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     4485 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/consumer/hvacsim/hvac.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      559 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/consumer/hvacsim/inputs.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     7187 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/consumer/hvacsim/presets.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1391 2022-04-06 07:13:10.000000 pysimmods-0.8.8/src/pysimmods/consumer/hvacsim/state.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.345516 pysimmods-0.8.8/src/pysimmods/generator/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/generator/__init__.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.345516 pysimmods-0.8.8/src/pysimmods/generator/biogassim/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       86 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/generator/biogassim/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     9428 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/generator/biogassim/biogas.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     3277 2022-06-16 11:18:24.000000 pysimmods-0.8.8/src/pysimmods/generator/biogassim/config.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      301 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/generator/biogassim/inputs.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)    22582 2022-06-16 11:18:24.000000 pysimmods-0.8.8/src/pysimmods/generator/biogassim/presets.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1727 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/generator/biogassim/state.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.345516 pysimmods-0.8.8/src/pysimmods/generator/chpcngsim/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       79 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/generator/chpcngsim/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     6118 2022-04-06 07:13:10.000000 pysimmods-0.8.8/src/pysimmods/generator/chpcngsim/chpcng.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1709 2022-04-06 07:13:10.000000 pysimmods-0.8.8/src/pysimmods/generator/chpcngsim/config.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      797 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/generator/chpcngsim/inputs.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      994 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/generator/chpcngsim/state.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.345516 pysimmods-0.8.8/src/pysimmods/generator/chplpgsim/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       81 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/generator/chplpgsim/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     6453 2022-06-16 11:18:21.000000 pysimmods-0.8.8/src/pysimmods/generator/chplpgsim/chplpg.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     2359 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/generator/chplpgsim/config.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      591 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/generator/chplpgsim/inputs.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1132 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/generator/chplpgsim/state.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.345516 pysimmods-0.8.8/src/pysimmods/generator/chplpgsystemsim/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      135 2022-04-06 07:32:42.000000 pysimmods-0.8.8/src/pysimmods/generator/chplpgsystemsim/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     4431 2022-07-07 17:02:55.000000 pysimmods-0.8.8/src/pysimmods/generator/chplpgsystemsim/chplpg_system.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1004 2022-07-07 17:02:55.000000 pysimmods-0.8.8/src/pysimmods/generator/chplpgsystemsim/config.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      535 2022-07-07 17:02:55.000000 pysimmods-0.8.8/src/pysimmods/generator/chplpgsystemsim/inputs.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     4237 2022-07-07 17:02:55.000000 pysimmods-0.8.8/src/pysimmods/generator/chplpgsystemsim/presets.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      682 2022-06-16 11:18:21.000000 pysimmods-0.8.8/src/pysimmods/generator/chplpgsystemsim/state.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.355517 pysimmods-0.8.8/src/pysimmods/generator/dieselsim/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       90 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/generator/dieselsim/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1239 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/generator/dieselsim/config.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1712 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/generator/dieselsim/dieselgen.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      385 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/generator/dieselsim/inputs.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      337 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/generator/dieselsim/presets.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      122 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/generator/dieselsim/state.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.355517 pysimmods-0.8.8/src/pysimmods/generator/pvsim/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       91 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/generator/pvsim/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     4785 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/generator/pvsim/config.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1181 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/generator/pvsim/inputs.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     8198 2022-11-10 10:50:35.000000 pysimmods-0.8.8/src/pysimmods/generator/pvsim/pvp.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      662 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/generator/pvsim/state.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.355517 pysimmods-0.8.8/src/pysimmods/generator/pvsystemsim/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      101 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/generator/pvsystemsim/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     4257 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/generator/pvsystemsim/config.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      956 2022-04-06 07:21:35.000000 pysimmods-0.8.8/src/pysimmods/generator/pvsystemsim/inputs.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1677 2022-11-10 07:54:10.000000 pysimmods-0.8.8/src/pysimmods/generator/pvsystemsim/presets.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     2690 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/generator/pvsystemsim/pvpsystem.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      670 2022-04-06 07:13:10.000000 pysimmods-0.8.8/src/pysimmods/generator/pvsystemsim/state.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.355517 pysimmods-0.8.8/src/pysimmods/model/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       50 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/model/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     6931 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/model/buffer.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     3094 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/model/config.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      774 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/model/consumer.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      483 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/model/generator.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1116 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/model/inputs.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)    11069 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/model/model.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     5811 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/model/qgenerator.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1090 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/model/state.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.355517 pysimmods-0.8.8/src/pysimmods/mosaik/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       50 2022-05-09 08:15:00.000000 pysimmods-0.8.8/src/pysimmods/mosaik/__init__.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.355517 pysimmods-0.8.8/src/pysimmods/mosaik/analysis/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2022-05-04 07:28:24.000000 pysimmods-0.8.8/src/pysimmods/mosaik/analysis/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     2751 2022-05-04 07:32:50.000000 pysimmods-0.8.8/src/pysimmods/mosaik/analysis/analysis.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     3960 2022-06-21 08:49:24.000000 pysimmods-0.8.8/src/pysimmods/mosaik/analysis/power.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)    11438 2022-08-11 10:41:48.000000 pysimmods-0.8.8/src/pysimmods/mosaik/flex_mosaik.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     2182 2022-07-07 17:02:55.000000 pysimmods-0.8.8/src/pysimmods/mosaik/meta.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)    21850 2022-11-10 10:48:27.000000 pysimmods-0.8.8/src/pysimmods/mosaik/midas_module.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     8764 2022-09-19 07:21:45.000000 pysimmods-0.8.8/src/pysimmods/mosaik/pysim_mosaik.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.355517 pysimmods-0.8.8/src/pysimmods/other/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       50 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/other/__init__.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.355517 pysimmods-0.8.8/src/pysimmods/other/dummy/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/other/dummy/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1384 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/other/dummy/buffer.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1166 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/other/dummy/consumer.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1065 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/other/dummy/generator.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     2018 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/other/dummy/model.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1670 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/other/dummy/qgenerator.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.355517 pysimmods-0.8.8/src/pysimmods/other/flexibility/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       65 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/other/flexibility/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     3780 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/other/flexibility/flexibility_model.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     5983 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/other/flexibility/forecast_model.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     8644 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/other/flexibility/schedule.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     6045 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/other/flexibility/schedule_model.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.355517 pysimmods-0.8.8/src/pysimmods/other/heatdemandsim/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      317 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/other/heatdemandsim/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      803 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/other/heatdemandsim/config.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     7216 2022-04-06 07:13:10.000000 pysimmods-0.8.8/src/pysimmods/other/heatdemandsim/heatdemand.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      258 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/other/heatdemandsim/inputs.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      712 2022-04-06 07:13:10.000000 pysimmods-0.8.8/src/pysimmods/other/heatdemandsim/state.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.355517 pysimmods-0.8.8/src/pysimmods/other/heatdemandsim/util/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/other/heatdemandsim/util/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)    11136 2022-04-06 07:32:42.000000 pysimmods-0.8.8/src/pysimmods/other/heatdemandsim/util/hprofiles.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.355517 pysimmods-0.8.8/src/pysimmods/other/heatstoragesim/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/other/heatstoragesim/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     3223 2022-06-16 11:18:21.000000 pysimmods-0.8.8/src/pysimmods/other/heatstoragesim/heatstorage.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.355517 pysimmods-0.8.8/src/pysimmods/other/invertersim/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       94 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/other/invertersim/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1573 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/other/invertersim/config.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1809 2022-04-06 07:21:35.000000 pysimmods-0.8.8/src/pysimmods/other/invertersim/inputs.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     8339 2022-06-14 07:31:43.000000 pysimmods-0.8.8/src/pysimmods/other/invertersim/inverter.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      808 2022-04-06 07:21:35.000000 pysimmods-0.8.8/src/pysimmods/other/invertersim/state.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.355517 pysimmods-0.8.8/src/pysimmods/util/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2022-04-06 06:55:56.000000 pysimmods-0.8.8/src/pysimmods/util/__init__.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      467 2022-04-06 07:13:10.000000 pysimmods-0.8.8/src/pysimmods/util/date_util.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     3383 2022-04-06 07:13:10.000000 pysimmods-0.8.8/src/pysimmods/util/irradiance.py
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     4425 2022-04-06 07:13:10.000000 pysimmods-0.8.8/src/pysimmods/util/solargeometry.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2022-11-10 10:52:48.345516 pysimmods-0.8.8/src/pysimmods.egg-info/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     2172 2022-11-10 10:52:48.000000 pysimmods-0.8.8/src/pysimmods.egg-info/PKG-INFO
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     4477 2022-11-10 10:52:48.000000 pysimmods-0.8.8/src/pysimmods.egg-info/SOURCES.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        1 2022-11-10 10:52:48.000000 pysimmods-0.8.8/src/pysimmods.egg-info/dependency_links.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      136 2022-11-10 10:52:48.000000 pysimmods-0.8.8/src/pysimmods.egg-info/requires.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       10 2022-11-10 10:52:48.000000 pysimmods-0.8.8/src/pysimmods.egg-info/top_level.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      431 2022-04-06 06:55:56.000000 pysimmods-0.8.8/tox.ini
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.662357 pysimmods-0.9.0/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     7648 2023-07-12 12:35:29.000000 pysimmods-0.9.0/LICENSE
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       91 2023-07-12 12:35:29.000000 pysimmods-0.9.0/MANIFEST.in
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     2136 2023-07-14 14:27:32.662357 pysimmods-0.9.0/PKG-INFO
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1139 2023-07-12 12:35:29.000000 pysimmods-0.9.0/README.md
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        5 2023-07-14 14:17:50.000000 pysimmods-0.9.0/VERSION
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1309 2023-07-14 14:27:24.000000 pysimmods-0.9.0/pyproject.toml
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       38 2023-07-14 14:27:32.662357 pysimmods-0.9.0/setup.cfg
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.649023 pysimmods-0.9.0/src/
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.652356 pysimmods-0.9.0/src/pysimmods/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/__init__.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.652356 pysimmods-0.9.0/src/pysimmods/buffer/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/buffer/__init__.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.652356 pysimmods-0.9.0/src/pysimmods/buffer/batterysim/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       29 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/buffer/batterysim/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     5580 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/buffer/batterysim/battery.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     2352 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/buffer/batterysim/config.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      354 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/buffer/batterysim/inputs.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      513 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/buffer/batterysim/presets.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1532 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/buffer/batterysim/state.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.652356 pysimmods-0.9.0/src/pysimmods/consumer/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/consumer/__init__.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.655690 pysimmods-0.9.0/src/pysimmods/consumer/hvacsim/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       74 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/consumer/hvacsim/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     3040 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/consumer/hvacsim/config.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     4484 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/consumer/hvacsim/hvac.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      559 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/consumer/hvacsim/inputs.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     7185 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/consumer/hvacsim/presets.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1391 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/consumer/hvacsim/state.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.655690 pysimmods-0.9.0/src/pysimmods/generator/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/__init__.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.655690 pysimmods-0.9.0/src/pysimmods/generator/biogassim/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       86 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/biogassim/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     9426 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/biogassim/biogas.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     3277 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/biogassim/config.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      301 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/biogassim/inputs.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)    22582 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/biogassim/presets.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1727 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/biogassim/state.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.655690 pysimmods-0.9.0/src/pysimmods/generator/chpcngsim/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       79 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/chpcngsim/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     6117 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/chpcngsim/chpcng.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1709 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/chpcngsim/config.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      797 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/chpcngsim/inputs.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      994 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/chpcngsim/state.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.655690 pysimmods-0.9.0/src/pysimmods/generator/chplpgsim/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       81 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/chplpgsim/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     6628 2023-07-14 11:05:27.000000 pysimmods-0.9.0/src/pysimmods/generator/chplpgsim/chplpg.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     2359 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/chplpgsim/config.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      591 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/chplpgsim/inputs.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1132 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/chplpgsim/state.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.655690 pysimmods-0.9.0/src/pysimmods/generator/chplpgsystemsim/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      135 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/chplpgsystemsim/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     4430 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/chplpgsystemsim/chplpg_system.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1003 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/chplpgsystemsim/config.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      535 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/chplpgsystemsim/inputs.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     4237 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/chplpgsystemsim/presets.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      682 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/chplpgsystemsim/state.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.655690 pysimmods-0.9.0/src/pysimmods/generator/dieselsim/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       90 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/dieselsim/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1239 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/dieselsim/config.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1712 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/dieselsim/dieselgen.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      385 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/dieselsim/inputs.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      337 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/dieselsim/presets.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      122 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/dieselsim/state.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.659023 pysimmods-0.9.0/src/pysimmods/generator/pvsim/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       91 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/pvsim/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     4785 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/pvsim/config.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1181 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/pvsim/inputs.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     8198 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/pvsim/pvp.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      662 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/pvsim/state.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.659023 pysimmods-0.9.0/src/pysimmods/generator/pvsystemsim/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      101 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/pvsystemsim/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     4257 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/pvsystemsim/config.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      956 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/pvsystemsim/inputs.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1677 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/pvsystemsim/presets.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     2748 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/pvsystemsim/pvpsystem.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      801 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/generator/pvsystemsim/state.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.659023 pysimmods-0.9.0/src/pysimmods/model/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       50 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/model/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     7047 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/model/buffer.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     3093 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/model/config.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      774 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/model/consumer.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      599 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/model/generator.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1116 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/model/inputs.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)    11069 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/model/model.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     5811 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/model/qgenerator.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1090 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/model/state.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.659023 pysimmods-0.9.0/src/pysimmods/mosaik/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       50 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/mosaik/__init__.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.659023 pysimmods-0.9.0/src/pysimmods/mosaik/analysis/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/mosaik/analysis/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     2751 2023-07-14 11:05:27.000000 pysimmods-0.9.0/src/pysimmods/mosaik/analysis/analysis.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     3960 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/mosaik/analysis/power.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)    11537 2023-07-14 14:05:19.000000 pysimmods-0.9.0/src/pysimmods/mosaik/flex_mosaik.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     2200 2023-07-14 13:12:04.000000 pysimmods-0.9.0/src/pysimmods/mosaik/meta.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)    23043 2023-07-14 11:05:27.000000 pysimmods-0.9.0/src/pysimmods/mosaik/midas_module.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)    10362 2023-07-14 14:18:20.000000 pysimmods-0.9.0/src/pysimmods/mosaik/pysim_mosaik.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.659023 pysimmods-0.9.0/src/pysimmods/other/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       50 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/__init__.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.662357 pysimmods-0.9.0/src/pysimmods/other/dummy/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/dummy/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1384 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/dummy/buffer.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1166 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/dummy/consumer.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1065 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/dummy/generator.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     2285 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/dummy/model.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1670 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/dummy/qgenerator.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.662357 pysimmods-0.9.0/src/pysimmods/other/flexibility/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       65 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/flexibility/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      918 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/flexibility/flexibilities.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     4391 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/flexibility/flexibility_model.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     5983 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/flexibility/forecast_model.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)    11661 2023-07-14 11:25:56.000000 pysimmods-0.9.0/src/pysimmods/other/flexibility/schedule.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     6043 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/flexibility/schedule_model.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.662357 pysimmods-0.9.0/src/pysimmods/other/heatdemandsim/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      317 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/heatdemandsim/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      803 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/heatdemandsim/config.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     7216 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/heatdemandsim/heatdemand.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      258 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/heatdemandsim/inputs.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      711 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/heatdemandsim/state.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.662357 pysimmods-0.9.0/src/pysimmods/other/heatdemandsim/util/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/heatdemandsim/util/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)    11136 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/heatdemandsim/util/hprofiles.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.662357 pysimmods-0.9.0/src/pysimmods/other/heatstoragesim/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/heatstoragesim/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     3286 2023-07-14 11:05:27.000000 pysimmods-0.9.0/src/pysimmods/other/heatstoragesim/heatstorage.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.662357 pysimmods-0.9.0/src/pysimmods/other/invertersim/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       94 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/invertersim/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1573 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/invertersim/config.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1809 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/invertersim/inputs.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     8339 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/invertersim/inverter.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      808 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/other/invertersim/state.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.662357 pysimmods-0.9.0/src/pysimmods/util/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        0 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/util/__init__.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      467 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/util/date_util.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     3383 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/util/irradiance.py
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     4425 2023-07-12 12:35:29.000000 pysimmods-0.9.0/src/pysimmods/util/solargeometry.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-07-14 14:27:32.652356 pysimmods-0.9.0/src/pysimmods.egg-info/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     2136 2023-07-14 14:27:32.000000 pysimmods-0.9.0/src/pysimmods.egg-info/PKG-INFO
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     4524 2023-07-14 14:27:32.000000 pysimmods-0.9.0/src/pysimmods.egg-info/SOURCES.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        1 2023-07-14 14:27:32.000000 pysimmods-0.9.0/src/pysimmods.egg-info/dependency_links.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      127 2023-07-14 14:27:32.000000 pysimmods-0.9.0/src/pysimmods.egg-info/requires.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       10 2023-07-14 14:27:32.000000 pysimmods-0.9.0/src/pysimmods.egg-info/top_level.txt
```

### Comparing `pysimmods-0.8.8/LICENSE` & `pysimmods-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/PKG-INFO` & `pysimmods-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: pysimmods
-Version: 0.8.8
+Version: 0.9.0
 Summary: A set of simulation models representing different distributed consumer or generator units.
-Home-page: https://gitlab.com/midas-mosaik/pysimmods
-Author: Stephan Balduin
-Author-email: stephan.balduin@offis.de
-License: LGPL
-Platform: UNKNOWN
+Author-email: Stephan Balduin <stephan.balduin@offis.de>
+Project-URL: Homepage, https://midas-mosaik.gitlab.io/pysimmods
+Project-URL: Bug Tracker, https://gitlab.com/midas-mosaik/pysimmods/-/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -47,8 +44,7 @@
 
     >>> pip install -e .
 
 ## Documentation
 
 You will find a still growing documentation at https://midas-mosaik.gitlab.io/pysimmods.
 Please create an issue if you find any errors or if you think that something should be explained more explicitly.
-
```

### Comparing `pysimmods-0.8.8/README.md` & `pysimmods-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/setup.py` & `pysimmods-0.9.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,50 @@
-#!/usr/bin/env python3
-"""Setup file for pysimmods package."""
-import setuptools
-
-with open("VERSION") as freader:
-    VERSION = freader.readline().strip()
-
-
-with open("README.md") as freader:
-    README = freader.read()
-
-install_requirements = [
-    "numpy",
-    "pandas",
+[build-system]
+requires = ["setuptools", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "pysimmods"
+version = "0.9.0"
+authors = [{name="Stephan Balduin", email="stephan.balduin@offis.de"}]
+description = "A set of simulation models representing different distributed consumer or generator units."
+readme = "README.md"
+requires-python = ">=3.8"
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Science/Research",
+    "Natural Language :: English",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Topic :: Scientific/Engineering",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+]
+dependencies = [
     "mosaik_api",
+    "midas-util>=1.0.4",
+    "pandas",
+    "numpy",
 ]
-development_requirements = {
-    "tox",
+
+[project.optional-dependencies]
+dev = [
     "pytest",
     "flake8",
-    "rope",
     "twine",
     "black==22.3.0",
     "coverage",
     "sphinx",
     "pytest-cov",
     "matplotlib",
     "wheel",
-    "midas-util>=1.0.0",
-}
+]
 
-extras = {"dev": development_requirements}
+[project.urls]
+"Homepage" = "https://midas-mosaik.gitlab.io/pysimmods"
+"Bug Tracker" = "https://gitlab.com/midas-mosaik/pysimmods/-/issues"
 
-setuptools.setup(
-    name="pysimmods",
-    version=VERSION,
-    author="Stephan Balduin",
-    author_email="stephan.balduin@offis.de",
-    description="A set of simulation models representing different "
-    "distributed consumer or generator units.",
-    long_description=README,
-    long_description_content_type="text/markdown",
-    url="https://gitlab.com/midas-mosaik/pysimmods",
-    packages=setuptools.find_packages(where="src"),
-    package_dir={"": "src"},
-    include_package_data=True,
-    install_requires=install_requirements,
-    extras_require=extras,
-    license="LGPL",
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: "
-        "GNU Lesser General Public License v2 (LGPLv2)",
-        "Natural Language :: English",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Topic :: Scientific/Engineering",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-    ],
-    python_requires=">=3.8",
-)
+[tool.black]
+line-length = 79
```

### Comparing `pysimmods-0.8.8/src/pysimmods/buffer/batterysim/battery.py` & `pysimmods-0.9.0/src/pysimmods/buffer/batterysim/battery.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,31 +127,29 @@
 
         if theoretical_energy_kwh > abs(delta_energy_kwh):
             # Won't be fully discharged in this step
             nstate._energy_kwh += delta_energy_kwh
         else:
             # Will be fully discharged in this step
             nstate.p_kw = theoretical_energy_kwh / (
-                self.inputs.step_size / 3600
+                self.inputs.step_size / 3600 / nstate.eta_percent * -100
             )
             nstate._energy_kwh = (
                 self.config.soc_min_percent / 100 * self.config.cap_kwh
             )
-            nstate.p_kw *= nstate.eta_percent / -100
 
     def _charge(self, nstate: BatteryState):
         delta_energy_kwh = (
             nstate.p_kw
             * (nstate.eta_percent / 100)
             * (self.inputs.step_size / 3600)
         )
 
         if (self.config.cap_kwh - nstate._energy_kwh) > delta_energy_kwh:
             # Won't be fully charged in this step
             nstate._energy_kwh += delta_energy_kwh
         else:
             # Will be fully charged in this step
             nstate.p_kw = (self.config.cap_kwh - nstate._energy_kwh) / (
-                self.inputs.step_size / 3600
+                self.inputs.step_size / 3600 * nstate.eta_percent / 100
             )
             nstate._energy_kwh = self.config.cap_kwh
-            nstate.p_kw /= nstate.eta_percent * 100
```

### Comparing `pysimmods-0.8.8/src/pysimmods/buffer/batterysim/config.py` & `pysimmods-0.9.0/src/pysimmods/buffer/batterysim/config.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/buffer/batterysim/presets.py` & `pysimmods-0.9.0/src/pysimmods/buffer/batterysim/presets.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Presets for the battery model."""
 
 
 def battery_preset(pn_max_kw, **kwargs):
-
     params = _get_dict(pn_max_kw, cap_kwh=kwargs.get("cap_kwh", pn_max_kw * 5))
     inits = {"soc_percent": kwargs.get("soc_percent", 50.0)}
 
     return params, inits
 
 
 def _get_dict(pn_max_kw, cap_kwh):
```

### Comparing `pysimmods-0.8.8/src/pysimmods/buffer/batterysim/state.py` & `pysimmods-0.9.0/src/pysimmods/buffer/batterysim/state.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/consumer/hvacsim/config.py` & `pysimmods-0.9.0/src/pysimmods/consumer/hvacsim/config.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/consumer/hvacsim/hvac.py` & `pysimmods-0.9.0/src/pysimmods/consumer/hvacsim/hvac.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,14 @@
         )
 
     def set_percent(self, percentage: float) -> None:
         if percentage is not None and ~np.isnan(percentage):
             return super().set_percent(percentage)
 
     def get_default_setpoint(self, hour: int) -> float:
-
         test_state = deepcopy(self.state)
         self._check_constraints(test_state)
         return self._get_percent(
             test_state.p_kw,
             self.get_pn_min_kw(),
             self.get_pn_max_kw(),
         )
```

### Comparing `pysimmods-0.8.8/src/pysimmods/consumer/hvacsim/inputs.py` & `pysimmods-0.9.0/src/pysimmods/consumer/hvacsim/inputs.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/consumer/hvacsim/presets.py` & `pysimmods-0.9.0/src/pysimmods/consumer/hvacsim/presets.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,21 @@
 
 """
 
 import sys
 
 
 def hvac_preset(pn_max_kw, **kwargs):
-
     params = _get_dict(pn_max_kw, "params")
     inits = _get_dict(pn_max_kw, "init")
 
     return params, inits
 
 
 def _get_dict(p_kw, dicttype):
-
     thismodule = sys.modules[__name__]
 
     if p_kw in (0.08,):
         method = "hvac_{}w_{}".format(int(p_kw * 1000), dicttype)
     elif p_kw in (2, 60, 100, 230, 343, 1279):
         method = "hvac_{}kw_{}".format(int(p_kw), dicttype)
     else:
```

### Comparing `pysimmods-0.8.8/src/pysimmods/consumer/hvacsim/state.py` & `pysimmods-0.9.0/src/pysimmods/consumer/hvacsim/state.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/biogassim/biogas.py` & `pysimmods-0.9.0/src/pysimmods/generator/biogassim/biogas.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,14 @@
         for chp, p_set_kw in zip(self.chps, best_combi):
             self._set_chp_inputs(next_state)
             # TODO: Adapt available gas
             chp.inputs.p_set_kw = p_set_kw
             chp.step()
 
     def _generate_feasible_combis(self, next_state, p_combis):
-
         feasibles = dict()
         for combi in p_combis:
             states = list()
             for chp, p_set_kw in zip(self.chps, combi):
                 self._set_chp_inputs(next_state)
                 chp.inputs.p_set_kw = p_set_kw
                 states.append(chp.step(pretend=True))
@@ -255,15 +254,14 @@
             next_state.gas_critical = True
 
         if next_state.gas_fill_percent > self.config.gas_fill_max_percent:
             next_state.burn_gas = True
             next_state.gas_critical = True
 
     def get_state(self):
-
         state = {"state": copy.deepcopy(self.state.__dict__)}
         for idx, chp in enumerate(self.chps):
             state[f"chp-{idx}"] = chp.get_state()
         return state
 
     def set_state(self, state):
         for attr, value in state["state"].items():
```

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/biogassim/config.py` & `pysimmods-0.9.0/src/pysimmods/generator/biogassim/config.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/biogassim/presets.py` & `pysimmods-0.9.0/src/pysimmods/generator/biogassim/presets.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/biogassim/state.py` & `pysimmods-0.9.0/src/pysimmods/generator/biogassim/state.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/chpcngsim/chpcng.py` & `pysimmods-0.9.0/src/pysimmods/generator/chpcngsim/chpcng.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,14 @@
             setpoint = self.config.p_min_kw + (
                 (self.config.p_max_kw - self.config.p_min_kw) * default / 100
             )
 
         return abs(setpoint)
 
     def _check_constraints(self, next_state):
-
         if not self.inputs.gas_critical:
             self._check_daily_incative_time(next_state)
             self._check_restarts(next_state)
             self._check_daily_active_time(next_state)
 
         self._check_gas_demand(next_state)
```

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/chpcngsim/config.py` & `pysimmods-0.9.0/src/pysimmods/generator/chpcngsim/config.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/chpcngsim/inputs.py` & `pysimmods-0.9.0/src/pysimmods/generator/chpcngsim/inputs.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/chpcngsim/state.py` & `pysimmods-0.9.0/src/pysimmods/generator/chpcngsim/state.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/chplpgsim/chplpg.py` & `pysimmods-0.9.0/src/pysimmods/generator/chplpgsim/chplpg.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,23 +22,25 @@
     inputs : CHPLPGInputs
 
     """
 
     def __init__(self, params, inits):
         self.config = CHPLPGConfig(params)
         self.state = CHPLPGState(inits)
-        self.inputs = CHPLPGInputs()
+        self.inputs: CHPLPGInputs = CHPLPGInputs()
 
         self._storage = HeatStorage(params, inits)
 
     def step(self):
         """Perform a simulation step."""
         next_state = copy(self.state)
         next_state.p_kw = self._get_setpoint()
 
+        self._check_inputs()
+
         # Operating state constraint is checked first to prevent
         # invalid user inputs. However, this has least priority and
         # changes due to other constraints are possible.
         self._check_operating_state(next_state)
 
         self._check_performance_limit(next_state)
         self._check_lubricant(next_state)
@@ -57,14 +59,19 @@
             next_state.lubricant_l = self.config.lubricant_max_l
 
         next_state.q_kvar = 0
 
         self.state = next_state
         self.inputs.reset()
 
+    def _check_inputs(self):
+
+        if self.inputs.e_th_demand_set_kwh is None:
+            self.inputs.e_th_demand_set_kwh = 0
+
     def _get_setpoint(self):
         setpoint = self.inputs.p_set_kw
 
         if setpoint is not None:
             return abs(setpoint)
 
         hour = self.inputs.now_dt.hour
```

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/chplpgsim/config.py` & `pysimmods-0.9.0/src/pysimmods/generator/chplpgsim/config.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/chplpgsim/inputs.py` & `pysimmods-0.9.0/src/pysimmods/generator/chplpgsim/inputs.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/chplpgsim/state.py` & `pysimmods-0.9.0/src/pysimmods/generator/chplpgsim/state.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/chplpgsystemsim/chplpg_system.py` & `pysimmods-0.9.0/src/pysimmods/generator/chplpgsystemsim/chplpg_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 LOG = logging.getLogger(__name__)
 
 
 class CHPLPGSystem(Generator):
     """CHP system with CHP and household"""
 
     def __init__(self, params, inits):
-
         # First, create the chp
         params["chp"]["sign_convention"] = params.get(
             "sign_convention", "passive"
         )
         self.chp = CHPLPG(params["chp"], inits["chp"])
 
         # Get the thermal capabilities of the chp
```

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/chplpgsystemsim/config.py` & `pysimmods-0.9.0/src/pysimmods/generator/chplpgsystemsim/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
         self.e_th_demand_sign = 1.0
         if params.get("flip_e_th_demand_sign", False):
             self.e_th_demand_sign = -1.0
         self.default_schedule = self.chp.default_schedule
 
     @property
     def p_min_kw(self):
-
         return self.chp.p_min_kw
 
     @property
     def p_max_kw(self):
         return self.chp.p_max_kw
 
     @property
```

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/chplpgsystemsim/inputs.py` & `pysimmods-0.9.0/src/pysimmods/generator/chplpgsystemsim/inputs.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/chplpgsystemsim/presets.py` & `pysimmods-0.9.0/src/pysimmods/generator/chplpgsystemsim/presets.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/chplpgsystemsim/state.py` & `pysimmods-0.9.0/src/pysimmods/generator/chplpgsystemsim/state.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/dieselsim/config.py` & `pysimmods-0.9.0/src/pysimmods/generator/dieselsim/config.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/dieselsim/dieselgen.py` & `pysimmods-0.9.0/src/pysimmods/generator/dieselsim/dieselgen.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/pvsim/config.py` & `pysimmods-0.9.0/src/pysimmods/generator/pvsim/config.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/pvsim/inputs.py` & `pysimmods-0.9.0/src/pysimmods/generator/pvsim/inputs.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/pvsim/pvp.py` & `pysimmods-0.9.0/src/pysimmods/generator/pvsim/pvp.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/pvsim/state.py` & `pysimmods-0.9.0/src/pysimmods/generator/pvsim/state.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/pvsystemsim/config.py` & `pysimmods-0.9.0/src/pysimmods/generator/pvsystemsim/config.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/pvsystemsim/inputs.py` & `pysimmods-0.9.0/src/pysimmods/generator/pvsystemsim/inputs.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/pvsystemsim/presets.py` & `pysimmods-0.9.0/src/pysimmods/generator/pvsystemsim/presets.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/generator/pvsystemsim/pvpsystem.py` & `pysimmods-0.9.0/src/pysimmods/generator/pvsystemsim/pvpsystem.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         self.inverter.inputs.inductive = self.inputs.inverter_inductive
 
         self.inverter.step()
 
         # Update state
         self.state.t_module_deg_celsius = self.pv.state.t_module_deg_celsius
         self.state.p_kw = self.inverter.state.p_kw
+        self.state.p_possible_max_kw = self.pv.state.p_kw
         self.state.q_kvar = self.inverter.state.q_kvar
         self.state.cos_phi = self.inverter.state.cos_phi
         self.state.inverter_inductive = self.inverter.state.inductive
 
         self.inputs.reset()
 
     def get_state(self):
```

### Comparing `pysimmods-0.8.8/src/pysimmods/model/buffer.py` & `pysimmods-0.9.0/src/pysimmods/model/buffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,7 +187,13 @@
             self.inputs.p_set_kw = max(p_min, min(p_max, p_kw))
 
     def set_q_kvar(self, q_kvar) -> None:
         self.inputs.q_set_kvar = q_kvar
 
     def get_p_kw(self) -> float:
         return self.state.p_kw * self.config.lsign
+
+    def get_qn_min_kvar(self) -> float:
+        return 0
+
+    def get_qn_max_kvar(self) -> float:
+        return 0
```

### Comparing `pysimmods-0.8.8/src/pysimmods/model/config.py` & `pysimmods-0.9.0/src/pysimmods/model/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
         The minimal nominal apparent power output of the model.
     s_max_kva: float
         The maximal nominal apparent power output of the model.
 
     """
 
     def __init__(self, params: dict) -> None:
-
         self.sign_convention = params.get("sign_convention", "passive")
         assert self.sign_convention in ["active", "passive"]
 
         self.psc = self.sign_convention == "passive"
         self.asc = self.sign_convention == "active"
 
         if self.sign_convention == "active":
```

### Comparing `pysimmods-0.8.8/src/pysimmods/model/consumer.py` & `pysimmods-0.9.0/src/pysimmods/model/consumer.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/model/inputs.py` & `pysimmods-0.9.0/src/pysimmods/model/inputs.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/model/model.py` & `pysimmods-0.9.0/src/pysimmods/model/model.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/model/qgenerator.py` & `pysimmods-0.9.0/src/pysimmods/model/qgenerator.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/model/state.py` & `pysimmods-0.9.0/src/pysimmods/model/state.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/mosaik/analysis/analysis.py` & `pysimmods-0.9.0/src/pysimmods/mosaik/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/mosaik/analysis/power.py` & `pysimmods-0.9.0/src/pysimmods/mosaik/analysis/power.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/mosaik/flex_mosaik.py` & `pysimmods-0.9.0/src/pysimmods/mosaik/flex_mosaik.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """This module contains a :class:`mosaik_api.Simulator` for the
 flexiblity model, which is a wrapper for all models of the
 pysimmods package.
 
 """
 from __future__ import annotations
-import json
 
-import sys
+import json
 from datetime import datetime, timedelta, timezone
 from typing import Any, Dict, List, Union
 
 import mosaik_api
 import numpy as np
 import pandas as pd
+
 from midas.util.dict_util import tobool
 from midas.util.logging import set_and_init_logger
 from midas.util.runtime_config import RuntimeConfig
 from pysimmods.mosaik import LOG
 from pysimmods.other.flexibility.flexibility_model import FlexibilityModel
 from pysimmods.other.flexibility.forecast_model import ForecastModel
 from pysimmods.other.flexibility.schedule_model import ScheduleModel
@@ -160,26 +160,20 @@
         params.setdefault("use_decimal_percent", self.use_decimal_percent)
         self.num_models.setdefault(model, 0)
 
         for _ in range(num):
             eid = f"{model}-{self.num_models[model]}"
 
             if self.provide_flexibilities:
-                # FIXME
                 self.models[eid] = FlexibilityModel(
                     MODELS[model](params, inits),
-                    self.now_dt,
-                    step_size=self.step_size,
-                    forecast_horizon_hours=self.forecast_horizon_hours,
-                    flexibility_horizon_hours=self.flexibility_horizon_hours,
-                    num_schedules=self.num_schedules,
-                    seed=self.rng.randint(sys.maxsize),
                     unit=self.unit,
-                    use_decimal_percent=self.use_decimal_percent,
-                    priorize_schedule=self.prioritize_setpoint,
+                    prioritize_setpoint=self.prioritize_setpoint,
+                    forecast_horizon_hours=self.forecast_horizon_hours,
+                    seed=self.rng.randint(2**32 - 1),
                 )
 
             elif self.provide_forecasts:
                 self.models[eid] = ForecastModel(
                     MODELS[model](params, inits),
                     unit=self.unit,
                     prioritize_setpoint=self.prioritize_setpoint,
@@ -257,15 +251,16 @@
                 "id": f"{self.sid}_{eid}",
                 "name": eid,
                 "type": eid.split("-")[0],
             }
 
             for attr in attrs:
                 if attr == "flexibilities":
-                    value = self.models[eid].flexibilities
+                    value = self._get_attr_flexibilities(eid)
+                    log_msg[attr] = json.loads(value)
 
                 elif attr == "schedule":
                     value = self._get_attr_schedule(eid)
                     log_msg[attr] = json.loads(value)
 
                 else:
                     value = self._get_remaining_attrs(eid, attr)
@@ -274,14 +269,16 @@
                 data.setdefault(eid, dict())[attr] = value
 
             if self.key_value_logs:
                 LOG.info(json.dumps(log_msg))
 
         if not self.key_value_logs:
             LOG.debug("Gathered outputs: %s.", data)
+        else:
+            LOG.debug(data)
 
         return data
 
     def _update_meta(self):
         for model in self.meta["models"].keys():
             self.meta["models"][model]["attrs"].extend(
                 ["flexibilities", "schedule", "target"]
@@ -321,19 +318,27 @@
             self.now_dt
             + timedelta(hours=self.forecast_horizon_hours)
             - timedelta(seconds=self.step_size),
         )
 
         return value
 
+    def _get_attr_flexibilities(self, eid: str) -> str:
+        dict_of_json = self.models[eid].flexibilities.to_json()
+        # value = json.dumps(dict_of_json)
+        return dict_of_json
+
     def _generate_flexibilities(self):
         if self.provide_flexibilities:
             for model in self.models.values():
                 model.generate_schedules(
-                    self.now_dt.strftime(GER),
+                    (
+                        self.now_dt
+                        + timedelta(hours=self.planning_horizon_hours)
+                    ).strftime(GER),
                     self.flexibility_horizon_hours,
                     self.num_schedules,
                 )
 
 
 def deserialize_schedule(
     schedule: Union[pd.DataFrame, Dict[str, Any], str]
```

### Comparing `pysimmods-0.8.8/src/pysimmods/mosaik/meta.py` & `pysimmods-0.9.0/src/pysimmods/mosaik/meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from pysimmods.consumer.hvacsim import HVAC
 from pysimmods.generator.biogassim import BiogasPlant
 from pysimmods.generator.chplpgsystemsim import CHPLPGSystem
 from pysimmods.generator.dieselsim import DieselGenerator
 from pysimmods.generator.pvsystemsim import PVPlantSystem
 
 _SHARED_ATTRS = [
-    "set_percent",
     "p_set_mw",
     "p_set_kw",
     "p_mw",
     "p_kw",
     "q_mvar",
     "q_kvar",
     "local_time",
@@ -36,14 +35,15 @@
                 "q_set_kvar",
                 "t_air_deg_celsius",
                 "t_module_deg_celsius",
                 "bh_w_per_m2",
                 "dh_w_per_m2",
                 "s_module_w_per_m2",
                 "inverter_inductive",
+                "p_possible_max_mw",
             ]
             + _SHARED_ATTRS,
         },
         "CHP": {
             "public": True,
             "params": ["params", "inits"],
             "attrs": [
```

### Comparing `pysimmods-0.8.8/src/pysimmods/mosaik/midas_module.py` & `pysimmods-0.9.0/src/pysimmods/mosaik/midas_module.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,20 @@
             "%(python)s -m pysimmods.mosaik.flex_mosaik %(addr)s"
         )
         self.models = {
             "PV": (
                 "Photovoltaic",
                 "sgen",
                 ["bh_w_per_m2", "dh_w_per_m2", "t_air_deg_celsius"],
-                ["p_mw", "q_mvar", "t_module_deg_celsius"],
+                [
+                    "p_mw",
+                    "q_mvar",
+                    "t_module_deg_celsius",
+                    "p_possible_max_mw",
+                ],
             ),
             "HVAC": (
                 "HVAC",
                 "load",
                 ["t_air_deg_celsius"],
                 ["p_mw", "q_mvar"],
             ),
@@ -104,28 +109,33 @@
         module_params.setdefault("prioritize_setpoint", False)
         module_params.setdefault(
             "provide_forecasts", module_params["provide_flexibilities"]
         )
         module_params.setdefault(
             "enable_schedules", module_params["provide_forecasts"]
         )
+        module_params.setdefault("pv_send_p_possible_max_mw_to_grid", False)
 
     def check_sim_params(self, module_params, **kwargs):
         """Check the params for a certain simulator instance."""
         self.sim_params.setdefault("grid_name", self.scope_name)
         self.sim_params.setdefault("start_date", module_params["start_date"])
         self.sim_params.setdefault("cos_phi", module_params["cos_phi"])
         self.sim_params.setdefault("q_control", module_params["q_control"])
         self.sim_params.setdefault(
             "inverter_mode", module_params["inverter_mode"]
         )
         self.sim_params.setdefault(
             "pv_is_static_t_module", module_params["pv_is_static_t_module"]
         )
         self.sim_params.setdefault(
+            "pv_send_p_possible_max_mw_to_grid",
+            module_params["pv_send_p_possible_max_mw_to_grid"],
+        )
+        self.sim_params.setdefault(
             "forecast_horizon_hours",
             module_params["forecast_horizon_hours"],
         )
         self.sim_params.setdefault(
             "provide_flexibilities",
             module_params["provide_flexibilities"],
         )
@@ -194,14 +204,23 @@
         if not self.sim_params[mapping_key]:
             # No mapping configured
             return
 
         eid_mapping = self.scenario.create_shared_mapping(
             self, self.sim_params["grid_name"], "eid"
         )
+        try:
+            pg_mapping = self.scenario.get_powergrid_mappings(
+                self.sim_params["grid_name"]
+            )
+        except Exception:
+            LOG.exception(
+                "Please update midas-mosaik or powergrid mapping will not work."
+            )
+            pg_mapping = {}
         high = "1.0" if self.sim_params["use_decimal_percent"] else "100.0"
         model_ctrs = {}
 
         for model, info in self.models.items():
             for bus, entities in self.sim_params[mapping_key].items():
                 for name, p_peak_mw in entities:
                     if model != name:
@@ -221,14 +240,20 @@
 
                     eid_mapping[full_id] = {
                         "p_mw": p_peak_mw,
                         "bus": bus,
                         "type": info[1],
                         "sn_mva": sn_mva,
                     }
+                    bus_mapping = pg_mapping.setdefault(bus, {})
+                    module_mapping = bus_mapping.setdefault(
+                        self.module_name, {}
+                    )
+                    model_mapping = module_mapping.setdefault(model, [])
+                    model_mapping.append(model_key)
                     if p_min != p_max:
                         self.actuators.append(
                             create_actuator(full_id, "p_set_mw", p_min, p_max)
                         )
                     if q_min != q_max:
                         self.actuators.append(
                             create_actuator(
@@ -305,20 +330,24 @@
                 if model != name:
                     continue
 
                 model_ctrs.setdefault(model, 0)
                 model_key = self.scenario.generate_model_key(
                     self, model.lower(), bus, model_ctrs[model]
                 )
+                attrs = info[3][:2]
+                if (
+                    self.sim_params["pv_send_p_possible_max_mw_to_grid"]
+                    and model.lower() == "pv"
+                ):
+                    attrs.append(("p_possible_max_mw", "max_p_mw"))
                 grid_entity_key = None
                 try:
                     grid_entity_key = self.get_grid_entity(info[1], bus)
-                    self.connect_entities(
-                        model_key, grid_entity_key, info[3][:2]
-                    )
+                    self.connect_entities(model_key, grid_entity_key, attrs)
                 except ScenarioError as e:
                     LOG.warning(
                         "Encountered scenario error while connecting %s"
                         "to grid entity %s: %s",
                         model_key,
                         grid_entity_key,
                         e,
@@ -344,15 +373,14 @@
     def connect_to_db(self):
         """Connect the models to db."""
         mapping_key = "peak_mapping"
         db_key = self.scenario.find_first_model("store", "database")[0]
 
         model_ctrs = dict()
         for model, info in self.models.items():
-
             for bus, entities in self.sim_params[mapping_key].items():
                 for name, _ in entities:
                     if model != name:
                         continue
 
                     model_ctrs.setdefault(model, 0)
                     model_key = self.scenario.generate_model_key(
@@ -414,15 +442,15 @@
                         break
 
                 except KeyError:
                     pass
 
         wpmapping = dict()
         for models in self.sim_params["mapping"].values():
-            for (model, _) in models:
+            for model, _ in models:
                 wpmapping.setdefault(model, dict())
                 wpmapping[model].setdefault(wprovider, list())
                 wpmapping[model][wprovider].append(0)
 
         return wpmapping
 
     def get_weather_model(self, model, idx, forecast=False):
```

### Comparing `pysimmods-0.8.8/src/pysimmods/mosaik/pysim_mosaik.py` & `pysimmods-0.9.0/src/pysimmods/mosaik/pysim_mosaik.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """This module contains a :class:`mosaik_api.Simulator` for all models
 of the pysimmods package.
 
 """
 import json
 import logging
 import pprint
-from datetime import datetime, timedelta, timezone
-from typing import Any, Dict
 import warnings
+from datetime import datetime, timedelta, timezone
+from typing import Any, Dict, List, Optional
 
 import mosaik_api
 import numpy as np
+
 from midas.util.dict_util import strtobool
 from midas.util.logging import set_and_init_logger
 from midas.util.runtime_config import RuntimeConfig
 from pysimmods.model.model import Model
 from pysimmods.mosaik import LOG
 from pysimmods.util.date_util import GER
 
@@ -25,109 +26,122 @@
 
 class PysimmodsSimulator(mosaik_api.Simulator):
     """The Pysimmods simulator."""
 
     def __init__(self):
         super().__init__(META)
         self.sid: str
-        self.models: Dict[str, Model] = {}
-        self.num_models: Dict[str, int] = {}
-
         self.step_size: int
         self.now_dt: datetime
-        self.percent_factor: float = 1.0
         self.key_value_logs: bool
 
-    def init(self, sid, **sim_params):
+        self.models: Dict[str, Model] = {}
+        self.num_models: Dict[str, int] = {}
+
+    def init(
+        self,
+        sid: str,
+        start_date: str,
+        step_size: int = 900,
+        key_value_logs: Optional[bool] = None,
+        time_resolution: float = 1.0,
+    ):
         """Called exactly ones after the simulator has been started.
 
         Parameters
         ----------
         sid : str
             Simulator ID for this simulator.
         start_date : str
             The start date as UTC ISO 8601 date string.
         step_size : int, optional
             Step size for this simulator. Defaults to 900.
+        key_value_logs: bool, optional
+            If set to True, a different, json-based logging format will
+            be used. Default is False.
+        time_resolution: float, optional
+            Something new from mosaik 3.
 
         Returns
         -------
         dict
             The meta dict (set by *mosaik_api.Simulator*).
 
         """
         self.sid = sid
-        if "step_size" not in sim_params:
-            LOG.debug(
-                "Param *step_size* not provided. "
-                "Using default step size of 900."
-            )
-        self.step_size = sim_params.get("step_size", 900)
-        self.now_dt = datetime.strptime(
-            sim_params["start_date"], GER
-        ).astimezone(timezone.utc)
-
-        use_decimal_percent = sim_params.get("use_decimal_percent", False)
-        if not isinstance(use_decimal_percent, bool):
-            try:
-                use_decimal_percent = strtobool(use_decimal_percent)
-            except ValueError:
-                use_decimal_percent = False
+        self.step_size = step_size
+        self.now_dt = datetime.strptime(start_date, GER).astimezone(
+            timezone.utc
+        )
 
-        if use_decimal_percent:
-            self.percent_factor = 0.01
-        else:
-            self.percent_factor = 1.0
+        self.key_value_logs = key_value_logs
+        if self.key_value_logs is None:
+            self.key_value_logs = RuntimeConfig().misc.get(
+                "key_value_logs", False
+            )
 
-        self.key_value_logs = sim_params.get(
-            "key_value_logs", RuntimeConfig().misc.get("key_value_logs", False)
-        )
         return self.meta
 
-    def create(self, num, model, **model_params):
+    def create(
+        self,
+        num: int,
+        model: str,
+        params: Dict[str, Any],
+        inits: Dict[str, Any],
+    ):
         """Initialize the simulation model instance (entity).
 
         Parameters
         ----------
-        num : int
+        num: int
             The number of models to create.
-        model : str
+        model: str
             The name of the models to create. Must be present inside
             the simulator's meta.
+        params: Dict[str, Any]
+            The dictionary with parameters for the model to be created.
+            Must be provided but can be empty.
+        inits: Dict[str, Any]
+            The dictionary with initial values for the state of the
+            model to be created. Must be provided but can be empty.
 
         Returns
         -------
         list
             A list with information on the created entity.
 
         """
-        entities = list()
-        params = model_params["params"]
-        inits = model_params["inits"]
+        entities = []
         self.num_models.setdefault(model, 0)
 
         for _ in range(num):
-
             eid = f"{model}-{self.num_models[model]}"
             self.models[eid] = MODELS[model](params, inits)
             self.num_models[model] += 1
             entities.append({"eid": eid, "type": model})
 
         return entities
 
-    def step(self, time, inputs, max_advance=0):
+    def step(
+        self,
+        time: int,
+        inputs: Dict[str, Dict[str, Dict[str, Any]]],
+        max_advance: int = 0,
+    ):
         """Perform a simulation step.
 
         Parameters
         ----------
         time : int
             The current simulation step (by convention in seconds since
             simulation start.
         inputs : dict
             A *dict* containing inputs for entities of this simulator.
+        max_advance: int,
+            Required for mosaik>=3 but not explicitly supported yet.
 
         Returns
         -------
         int
             The next step this simulator wants to be stepped.
 
         """
@@ -139,14 +153,16 @@
             )
 
         self._set_default_inputs()
 
         # Set inputs from other simulators
         for eid, attrs in inputs.items():
             for attr, src_ids in attrs.items():
+                if self.key_value_logs:
+                    self._log_input(eid, attr, src_ids)
 
                 # Use time information from time generator
                 if attr == "local_time":
                     self._set_attr_local_time(eid, src_ids)
                     continue
 
                 attr_sum = self._aggregate_attr(src_ids)
@@ -157,44 +173,39 @@
             model.step()
 
         # Update time for the next step
         self.now_dt += timedelta(seconds=self.step_size)
 
         return time + self.step_size
 
-    def get_data(self, outputs):
+    def get_data(
+        self, outputs: Dict[str, List[str]]
+    ) -> Dict[str, Dict[str, Any]]:
         """Return the requested output (if feasible).
 
         Parameters
         ----------
         outputs : dict
             A *dict* containing requested outputs of each entity.
 
         Returns
         -------
         dict
             A *dict* containing the values of the requested outputs.
 
         """
 
-        data = dict()
+        data = {}
         for eid, attrs in outputs.items():
-            log_msg = {
-                "id": f"{self.sid}_{eid}",
-                "name": eid,
-                "type": eid.split("-")[0],
-            }
-
             for attr in attrs:
                 value = self._get_remaining_attrs(eid, attr)
                 data.setdefault(eid, dict())[attr] = value
-                log_msg[attr] = value
 
-            if self.key_value_logs:
-                LOG.info(json.dumps(log_msg))
+                if self.key_value_logs:
+                    self._log_output(eid, attr, value)
 
         if not self.key_value_logs:
             LOG.debug("Gathered outputs: %s.", pprint.pformat(data))
 
         return data
 
     def _set_default_inputs(self):
@@ -203,14 +214,51 @@
             self.step_size,
             self.now_dt,
         )
         for _, model in self.models.items():
             model.set_step_size(self.step_size)
             model.set_now_dt(self.now_dt)
 
+    def _log_input(self, eid: str, attr: str, src_ids: Dict[str, Any]):
+        for src_id, val in src_ids.items():
+            if isinstance(val, np.ndarray):
+                val = val.tolist()
+            elif isinstance(val, np.integer):
+                val = int(val)
+            elif isinstance(val, (np.float32, np.floating)):
+                val = float(val)
+
+            LOG.debug(
+                json.dumps(
+                    {
+                        "id": f"{self.sid}_{eid}",
+                        "name": eid,
+                        "model": eid.split("-")[0],
+                        "type": "input",
+                        "attribute": attr,
+                        "source": src_id,
+                        "value": val,
+                    }
+                )
+            )
+
+    def _log_output(self, eid: str, attr: str, value: Any):
+        LOG.debug(
+            json.dumps(
+                {
+                    "id": f"{self.sid}_{eid}",
+                    "name": eid,
+                    "model": eid.split("-")[0],
+                    "type": "output",
+                    "attribute": attr,
+                    "value": value,
+                }
+            )
+        )
+
     def _set_attr_local_time(self, eid: str, src_ids: Dict[str, Any]) -> bool:
         for val in src_ids.values():
             self.models[eid].set_now_dt(val)
             self.now_dt = datetime.strptime(val, GER).astimezone(timezone.utc)
             return True
 
         return False
@@ -229,20 +277,20 @@
                 # This should only happen if palaestrAI is used
                 val = val[0]
             attr_sum += val
         attr_sum /= len(src_ids)
 
         return float(attr_sum)
 
-    def _set_percent_power(self, eid: str, attr_sum: float):
-        attr_sum /= self.percent_factor
-        attr_sum = self.models[eid].get_pn_min_kw() + attr_sum * (
-            self.models[eid].get_pn_max_kw() - self.models[eid].get_pn_min_kw()
-        )
-        self.models[eid].set_p_kw(attr_sum)
+    # def _set_percent_power(self, eid: str, attr_sum: float):
+    #     attr_sum /= self.percent_factor
+    #     attr_sum = self.models[eid].get_pn_min_kw() + attr_sum * (
+    #         self.models[eid].get_pn_max_kw() - self.models[eid].get_pn_min_kw()
+    #     )
+    #     self.models[eid].set_p_kw(attr_sum)
 
     def _set_remaining_attrs(self, eid: str, attr: str, attr_sum: float):
         # Apply corrections
         if attr in ("p_set_mw", "p_th_set_mw", "q_set_mvar"):
             attr = attr.replace("m", "k")
             attr_sum *= 1e3
 
@@ -260,26 +308,28 @@
         else:
             setattr(self.models[eid].inputs, attr, attr_sum)
 
     def _get_remaining_attrs(self, eid: str, attr: str) -> float:
         # Apply correction of the attr if necessary
         if attr in ("p_mw", "p_th_mw", "q_mvar"):
             true_attr = attr.replace("m", "k")
+        elif attr == "p_possible_max_mw":
+            true_attr = "p_possible_max_kw"
         else:
             true_attr = attr
 
         if true_attr == "p_kw":
             value = self.models[eid].get_p_kw()
         elif true_attr == "q_kvar":
             value = self.models[eid].get_q_kvar()
         else:
             value = getattr(self.models[eid].state, true_attr)
 
         # Apply correction of the value if necessary
-        if attr in ("p_mw", "p_th_mw", "q_mvar"):
+        if attr in ("p_mw", "p_th_mw", "q_mvar", "p_possible_max_mw"):
             value *= 1e-3
 
         return value
 
 
 if __name__ == "__main__":
     set_and_init_logger(
```

### Comparing `pysimmods-0.8.8/src/pysimmods/other/dummy/buffer.py` & `pysimmods-0.9.0/src/pysimmods/other/dummy/buffer.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/other/dummy/consumer.py` & `pysimmods-0.9.0/src/pysimmods/other/dummy/consumer.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/other/dummy/generator.py` & `pysimmods-0.9.0/src/pysimmods/other/dummy/generator.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/other/dummy/model.py` & `pysimmods-0.9.0/src/pysimmods/other/dummy/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 class DummyConfig(ModelConfig):
     def __init__(self, params: Dict[str, Any]):
         super().__init__(params)
 
         self.p_max_kw: float = params.get("p_max_kw", 500)
         self.p_min_kw: float = params.get("p_min_kw", 250)
+        self.q_min_kvar: float = params.get("q_min_kvar", -550)
+        self.q_max_kvar: float = params.get("q_max_kvar", 550)
         self.default_p_schedule = [375.0] * 24
         self.default_q_schedule = [125.0] * 24
 
 
 class DummyState(ModelState):
     pass
 
@@ -46,14 +48,20 @@
 
     def get_pn_max_kw(self):
         return self.config.p_max_kw
 
     def get_pn_min_kw(self):
         return self.config.p_min_kw
 
+    def get_qn_max_kvar(self):
+        return self.config.q_max_kvar
+
+    def get_qn_min_kvar(self):
+        return self.config.q_min_kvar
+
     def set_p_kw(self, p_kw: float) -> None:
         self.inputs.p_set_kw = p_kw
 
     def get_p_kw(self):
         return self.state.p_kw
 
     def set_q_kvar(self, q_kvar: float) -> None:
```

### Comparing `pysimmods-0.8.8/src/pysimmods/other/dummy/qgenerator.py` & `pysimmods-0.9.0/src/pysimmods/other/dummy/qgenerator.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/other/flexibility/flexibility_model.py` & `pysimmods-0.9.0/src/pysimmods/other/flexibility/flexibility_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 """This module contains the flexibility model."""
+import logging
 from datetime import datetime, timedelta
 from typing import Optional
 
 import numpy as np
 import pandas as pd
-from pysimmods.util.date_util import GER, TZ
 
-from . import LOG
+from pysimmods.util.date_util import GER
+
+from .flexibilities import Flexibilities
 from .forecast_model import ForecastModel
+from .schedule import Schedule
+
+LOG = logging.getLogger(__name__)
 
 
 class FlexibilityModel(ForecastModel):
     """The flexibility model for all pysimmods."""
 
     def __init__(
         self,
         model,
         unit="kw",
-        priorize_setpoint=False,
+        prioritize_setpoint: bool = False,
         step_size: Optional[int] = None,
         now_dt: Optional[datetime] = None,
         forecast_horizon_hours=1,
         seed=None,
+        store_min_and_max: bool = False,
     ):
         super().__init__(
             model,
             unit,
-            priorize_setpoint,
+            prioritize_setpoint,
             step_size,
             now_dt,
             forecast_horizon_hours,
         )
 
+        self._store_min_and_max = store_min_and_max
+
         if seed is not None:
             self._rng = np.random.RandomState(seed)
         else:
             self._rng = np.random.RandomState()
 
     def generate_schedules(
         self, start, flexibility_horizon_hours, num_schedules
@@ -64,57 +72,69 @@
         periods = flexibility_horizon_hours * 3_600 / step_size
 
         # Fast forward to the planning interval
         while start_dt > now_dt:
             try:
                 self._calculate_step(
                     now_dt,
-                    self.schedule.get(now_dt, "target") / self._percent_factor,
+                    self.schedule.get(now_dt, self._psetname),
+                    self.schedule.get(now_dt, self._qsetname),
                 )
                 now_dt += timedelta(seconds=step_size)
             except KeyError as err:
                 # raise err
                 LOG.info("Could not create flexibilities: %s", err)
-                return dict()
+                return {}
 
         index = pd.date_range(start_dt, end_dt, periods=periods)
 
-        self.flexibilities = dict()
+        self.flexibilities = Flexibilities()
 
         for schedule_id in range(num_schedules):
-            schedule = self._generate_schedule(
-                pd.DataFrame(
-                    columns=["target", self._pname, self._qname],
-                    index=index,
-                )
-            )
-
-            self.flexibilities[schedule_id] = schedule.tz_convert(tz=TZ)
+            self.flexibilities.add_schedule(schedule_id, self.sample(index))
 
         self._model.set_state(state_backup)
         return self.flexibilities
 
-    def _generate_schedule(self, dataframe):
-        num_steps = len(dataframe.index)
-        dataframe["target"] = self._rng.uniform(size=num_steps) / (
-            0.01 / self._percent_factor
+    def sample(self, index):
+        dataframe = pd.DataFrame(
+            columns=[
+                self._psetname,
+                self._qsetname,
+                self._pname,
+                self._qname,
+            ],
+            index=index,
+        )
+        dataframe[self._psetname] = self._rng.uniform(
+            low=self.get_pn_min_kw(),
+            high=self.get_pn_max_kw(),
+            size=len(index),
+        )
+        dataframe[self._qsetname] = self._rng.uniform(
+            low=self.get_qn_min_kvar(),
+            high=self.get_qn_max_kvar(),
+            size=len(index),
         )
 
         state_backup = self._model.get_state()
         for index, row in dataframe.iterrows():
             try:
-                self._calculate_step(index, row["target"])
+                self._calculate_step(
+                    index, row[self._psetname], row[self._qsetname]
+                )
                 dataframe.loc[index, self._pname] = (
                     self._model.get_p_kw() * self._unit_factor
                 )
                 dataframe.loc[index, self._qname] = (
                     self._model.get_q_kvar() * self._unit_factor
                 )
 
             except KeyError:
                 # Forecast is missing
                 dataframe.loc[index, self._pname] = np.nan
                 dataframe.loc[index, self._qname] = np.nan
-                dataframe.loc[index, "target"] = np.nan
+                dataframe.loc[index, self._psetname] = np.nan
+                dataframe.loc[index, self._qsetname] = np.nan
         self._model.set_state(state_backup)
 
-        return dataframe
+        return Schedule().from_dataframe(dataframe)
```

### Comparing `pysimmods-0.8.8/src/pysimmods/other/flexibility/forecast_model.py` & `pysimmods-0.9.0/src/pysimmods/other/flexibility/forecast_model.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/other/flexibility/schedule.py` & `pysimmods-0.9.0/src/pysimmods/other/flexibility/schedule.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """This module contains the :class:`.Schedule` that is used by the
 :class:`.ForecastModel` and :class:`.FlexibilityModel`.
 
 """
+from __future__ import annotations
+
 import logging
 from datetime import datetime, timedelta, timezone
-from typing import Optional
+from typing import Dict, Optional
 
 import numpy as np
 import pandas as pd
-from pysimmods.util.date_util import GER
+
+from pysimmods.util.date_util import GER, TZ
 
 LOG = logging.getLogger(__name__)
 
 
 class Schedule:
     """Schedule class for the :class:`.ScheduleModel`.
 
@@ -33,25 +36,32 @@
         step_size: int = 1,
         horizon_hours: float = 1,
         start_date: Optional[datetime] = None,
         p_name: str = "p_kw",
         q_name: str = "q_kvar",
         p_set_name: Optional[str] = None,
         q_set_name: Optional[str] = None,
+        store_min_and_max: bool = False,
     ):
         self._data: pd.DataFrame
 
         self.step_size = step_size
         self.horizon_hours = horizon_hours
         self.now_dt = start_date
 
         self.p_name = p_name
         self.q_name = q_name
         self.p_set_name = p_set_name
         self.q_set_name = q_set_name
+        self.p_min_name = "p_min"
+        self.p_max_name = "p_max"
+        self.q_min_name = "q_min"
+        self.q_max_name = "q_max"
+
+        self.store_min_and_max = store_min_and_max
 
     def init(self):
         """Initialize the schedule data frame.
 
         After initialization, the schedule's data frame should have
         three columns *target*, *p_kw*, and *q_kvar* and a number of
         rows, each value initialized with np.nan.
@@ -62,14 +72,24 @@
 
         """
         LOG.debug(
             "Creating new schedule dataframe (and wiping any existing data)."
         )
         columns = [self.p_name, self.q_name]
 
+        if self.store_min_and_max:
+            columns.extend(
+                [
+                    self.p_min_name,
+                    self.p_max_name,
+                    self.q_min_name,
+                    self.q_max_name,
+                ]
+            )
+
         if self.p_set_name is None:
             unit = self.p_name.rsplit("_", 1)[1]
             self.p_set_name = f"p_set_{unit}"
         if self.q_set_name is None:
             unit = self.q_name.rsplit("_", 1)[1]
             self.q_set_name = f"q_set_{unit}"
 
@@ -126,33 +146,48 @@
     def update_row(
         self,
         index: datetime,
         p_set: float,
         q_set: Optional[float],
         p_val: float,
         q_val: float,
+        p_min: float = 0,
+        p_max: float = 0,
+        q_min: float = 0,
+        q_max: float = 0,
     ):
-
         if index in self._data.index:
-            self._data.loc[index][self.p_set_name] = p_set
-            self._data.loc[index][self.q_set_name] = q_set
-            self._data.loc[index][self.p_name] = p_val
-            self._data.loc[index][self.q_name] = q_val
+            self._data.loc[index, self.p_set_name] = p_set
+            self._data.loc[index, self.q_set_name] = q_set
+            self._data.loc[index, self.p_name] = p_val
+            self._data.loc[index, self.q_name] = q_val
+
+            if self.store_min_and_max:
+                self._data.loc[index, self.p_min_name] = p_min
+                self._data.loc[index, self.p_max_name] = p_max
+                self._data.loc[index, self.q_min_name] = q_min
+                self._data.loc[index, self.q_max_name] = q_max
 
         else:
             tmp_df = pd.DataFrame(
                 data={
                     self.p_set_name: p_set,
                     self.q_set_name: q_set,
                     self.p_name: p_val,
                     self.q_name: q_val,
                 },
                 index=[index],
             )
 
+            if self.store_min_and_max:
+                self._data.loc[index, self.p_min_name] = p_min
+                self._data.loc[index, self.p_max_name] = p_max
+                self._data.loc[index, self.q_min_name] = q_min
+                self._data.loc[index, self.q_max_name] = q_max
+
             self._data = pd.concat([self._data, tmp_df])
 
         self._data.sort_index(inplace=True)
         self._data.index = pd.to_datetime(self._data.index)
         self._data = self._data.fillna(value=np.nan)
 
     def update_entry(self, index, col, val):
@@ -161,15 +196,15 @@
                 f"Invalid column '{col}'. Supported columns are "
                 f"{self._data.columns}."
             )
         if index not in self._data.index:
             self._data = pd.concat(
                 [self._data, pd.DataFrame({col: val}, index=[index])]
             )
-        self._data.loc[index][col] = val
+        self._data.loc[index, col] = val
         self._data.sort_index(inplace=True)
         self._data = self._data.fillna(value=np.nan)
 
     def has_index(self, index):
         return index in self._data.index
 
     def reschedule_required(self):
@@ -195,14 +230,23 @@
                 return True
             if self.get(now, self.q_set_name) is None:
                 return True
             if self.get(now, self.p_name) is None:
                 return True
             elif self.get(now, self.q_name) is None:
                 return True
+            if self.store_min_and_max:
+                if self.get(now, self.p_min_name) is None:
+                    return True
+                if self.get(now, self.p_max_name) is None:
+                    return True
+                if self.get(now, self.q_min_name) is None:
+                    return True
+                if self.get(now, self.q_max_name) is None:
+                    return True
 
             now += timedelta(seconds=self.step_size)
 
         return False
 
     def prune(self):
         self._data = self._data.loc[self.now_dt :]
@@ -229,64 +273,108 @@
         val = self._data.loc[now][col]
 
         if np.isnan(val):
             return None
         else:
             return val
 
+    def to_dict(
+        self,
+        start_dt: Optional[datetime] = None,
+        end_dt: Optional[datetime] = None,
+        keep_datetime: bool = False,
+    ) -> Dict[str, str]:
+        if start_dt is None:
+            start_dt = self._data.index[0]
+
+        if end_dt is None:
+            end_dt = self._data.index[-1]
+
+        partition = self._data.loc[start_dt:end_dt]
+
+        if not keep_datetime:
+            partition.index = partition.index.astype(np.int64)
+
+        return partition.to_dict()
+
+    def from_dict(self, dict_of_schedules: Dict[str, str]) -> Schedule:
+        df = pd.DataFrame(dict_of_schedules)
+        df.index = pd.to_datetime(
+            df.index.astype(np.int64), utc=True, origin="unix"
+        )
+        self.from_dataframe(df)
+
+        return self
+
     def to_json(
         self,
         start_dt: Optional[datetime] = None,
         end_dt: Optional[datetime] = None,
     ) -> str:
         if start_dt is None:
             start_dt = self._data.index[0]
 
         if end_dt is None:
             end_dt = self._data.index[-1]
 
         return self._data.loc[start_dt:end_dt].to_json()
 
-    def from_json(self, schedule_json):
+    def from_json(self, schedule_json) -> Schedule:
         schedule_df = pd.read_json(schedule_json).tz_localize("UTC")
         self.from_dataframe(schedule_df)
 
     def __call__(self):
         return self._data
 
     def from_dataframe(self, dataframe: pd.DataFrame):
         self._data = dataframe
-        self._data.index = pd.to_datetime(self._data.index)
+        self._data.index = pd.to_datetime(self._data.index).tz_convert(TZ)
         if "target" in self._data.columns:
             self.use_absolute_setpoints = False
             self.p_set_name = None
             self.q_set_name = None
         else:
             self.use_absolute_setpoints = True
 
         for col in self._data.columns:
             if "p_set" in col:
                 self.p_set_name = col
             elif "q_set" in col:
                 self.q_set_name = col
+            elif "p_min" in col:
+                self.p_min_name = col
+                self.store_min_and_max = True
+            elif "p_max" in col:
+                self.p_max_name = col
+                self.store_min_and_max = True
+            elif "q_min" in col:
+                self.q_min_name = col
+                self.store_min_and_max = True
+            elif "q_max" in col:
+                self.q_max_name = col
+                self.store_min_and_max = True
             elif "p_" in col:
                 self.p_name = col
             elif "q_" in col:
                 self.q_name = col
 
         self.now_dt = self._data.index[0].to_pydatetime()
         self.step_size = max(
             1,
             int(
                 (self._data.index[-1] - self._data.index[0]).total_seconds()
                 / (len(self._data.index) - 1)
             ),
         )
+        return self
 
     def __repr__(self):
         return self._data.__repr__()
 
     def is_empty(self):
         if not hasattr(self, "_data"):
             return True
 
         return self._data.empty
+
+    def compare(self, other: Schedule):
+        return self._data.compare(other._data)
```

### Comparing `pysimmods-0.8.8/src/pysimmods/other/flexibility/schedule_model.py` & `pysimmods-0.9.0/src/pysimmods/other/flexibility/schedule_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
         self,
         model: Model,
         unit: str = "kw",
         prioritize_setpoint: bool = False,
         step_size: Optional[int] = None,
         now_dt: Optional[datetime] = None,
     ):
-
         self._model = model
         self._prioritize_setpoint = prioritize_setpoint
 
         if unit == "mw":
             self._unit_factor = 1e-3
             unit_str = "m"
 
@@ -87,15 +86,14 @@
             self._model.get_p_kw() * self._unit_factor,
             self._model.get_q_kvar() * self._unit_factor,
         )
         self.schedule.now_dt = self._now_dt
         self.schedule.prune()
 
     def _check_inputs(self) -> None:
-
         # Check if model has a different step size
         if (
             self._model.inputs.step_size is not None
             and self._model.inputs.step_size != self._step_size
         ):
             self._step_size = self._model.inputs.step_size
```

### Comparing `pysimmods-0.8.8/src/pysimmods/other/heatdemandsim/config.py` & `pysimmods-0.9.0/src/pysimmods/other/heatdemandsim/config.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/other/heatdemandsim/heatdemand.py` & `pysimmods-0.9.0/src/pysimmods/other/heatdemandsim/heatdemand.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/other/heatdemandsim/util/hprofiles.py` & `pysimmods-0.9.0/src/pysimmods/other/heatdemandsim/util/hprofiles.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/other/heatstoragesim/heatstorage.py` & `pysimmods-0.9.0/src/pysimmods/other/heatstoragesim/heatstorage.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         Current temperature of the environment in [°C]. The storage
         is assumed to be placed indoor and, therefore, defaults to
         19.0 °C.
 
     """
 
     def __init__(self, params, inits):
-
         # Config
         self.cap_l = params["storage_cap_l"]
         self.consumption_kwh_per_day = params[
             "storage_consumption_kwh_per_day"
         ]
         self.t_min_c = params["storage_t_min_c"]
         self.t_max_c = params["storage_t_max_c"]
@@ -99,15 +98,15 @@
         e_th_in_min_kwh = (
             C_WATER * self.cap_l * max(0, self.t_c - self.t_min_c) / 3_600
         )
 
         return e_th_in_min_kwh
 
     def absorb_energy(self, e_th_prod, e_th_demand):
-
         # 1 kWh = 3600 kJ
+        # One and only one of prod and demand has to be negative
         e_th_delta_kj = (e_th_prod + e_th_demand) * 3_600
 
         t_chilled = self._calculate_chilled_t()
         t_new = e_th_delta_kj / (C_WATER * self.cap_l) + t_chilled
 
         self.t_c = max(t_new, self.env_t_c)
```

### Comparing `pysimmods-0.8.8/src/pysimmods/other/invertersim/config.py` & `pysimmods-0.9.0/src/pysimmods/other/invertersim/config.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/other/invertersim/inputs.py` & `pysimmods-0.9.0/src/pysimmods/other/invertersim/inputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """This module contains the input model for the inverter."""
 
 
-from distutils.util import strtobool
+from midas.util.dict_util import tobool
 
 
 class InverterInputs:
     """Inverter inputs.
 
     This model does not inherit from the :class:`~.ModelInputs`,
     because those inputs are not required for the inverter.
@@ -51,12 +51,12 @@
             return 0
 
     @inductive.setter
     def inductive(self, val):
         if val is None or isinstance(val, bool):
             self._inductive = val
         elif isinstance(val, str):
-            self._inductive = strtobool(val)
+            self._inductive = tobool(val)
         elif val != 0:
             self._inductive = True
         else:
             self._inductive = False
```

### Comparing `pysimmods-0.8.8/src/pysimmods/other/invertersim/inverter.py` & `pysimmods-0.9.0/src/pysimmods/other/invertersim/inverter.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/other/invertersim/state.py` & `pysimmods-0.9.0/src/pysimmods/other/invertersim/state.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/util/irradiance.py` & `pysimmods-0.9.0/src/pysimmods/util/irradiance.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods/util/solargeometry.py` & `pysimmods-0.9.0/src/pysimmods/util/solargeometry.py`

 * *Files identical despite different names*

### Comparing `pysimmods-0.8.8/src/pysimmods.egg-info/PKG-INFO` & `pysimmods-0.9.0/src/pysimmods.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: pysimmods
-Version: 0.8.8
+Version: 0.9.0
 Summary: A set of simulation models representing different distributed consumer or generator units.
-Home-page: https://gitlab.com/midas-mosaik/pysimmods
-Author: Stephan Balduin
-Author-email: stephan.balduin@offis.de
-License: LGPL
-Platform: UNKNOWN
+Author-email: Stephan Balduin <stephan.balduin@offis.de>
+Project-URL: Homepage, https://midas-mosaik.gitlab.io/pysimmods
+Project-URL: Bug Tracker, https://gitlab.com/midas-mosaik/pysimmods/-/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -47,8 +44,7 @@
 
     >>> pip install -e .
 
 ## Documentation
 
 You will find a still growing documentation at https://midas-mosaik.gitlab.io/pysimmods.
 Please create an issue if you find any errors or if you think that something should be explained more explicitly.
-
```

### Comparing `pysimmods-0.8.8/src/pysimmods.egg-info/SOURCES.txt` & `pysimmods-0.9.0/src/pysimmods.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 VERSION
-setup.py
-tox.ini
+pyproject.toml
 src/pysimmods/__init__.py
 src/pysimmods.egg-info/PKG-INFO
 src/pysimmods.egg-info/SOURCES.txt
 src/pysimmods.egg-info/dependency_links.txt
 src/pysimmods.egg-info/requires.txt
 src/pysimmods.egg-info/top_level.txt
 src/pysimmods/buffer/__init__.py
@@ -85,14 +84,15 @@
 src/pysimmods/other/dummy/__init__.py
 src/pysimmods/other/dummy/buffer.py
 src/pysimmods/other/dummy/consumer.py
 src/pysimmods/other/dummy/generator.py
 src/pysimmods/other/dummy/model.py
 src/pysimmods/other/dummy/qgenerator.py
 src/pysimmods/other/flexibility/__init__.py
+src/pysimmods/other/flexibility/flexibilities.py
 src/pysimmods/other/flexibility/flexibility_model.py
 src/pysimmods/other/flexibility/forecast_model.py
 src/pysimmods/other/flexibility/schedule.py
 src/pysimmods/other/flexibility/schedule_model.py
 src/pysimmods/other/heatdemandsim/__init__.py
 src/pysimmods/other/heatdemandsim/config.py
 src/pysimmods/other/heatdemandsim/heatdemand.py
```

