# Comparing `tmp/clover-energy-5.0.7b2.tar.gz` & `tmp/clover-energy-5.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clover-energy-5.0.7b2.tar", last modified: Tue Feb 14 09:56:25 2023, max compression
+gzip compressed data, was "/home/bewinche/modelling/CLOVER/dist/.tmp-1d4azq4f/clover-energy-5.0.8.tar", last modified: Fri Jul 14 14:29:36 2023, max compression
```

## Comparing `clover-energy-5.0.7b2.tar` & `clover-energy-5.0.8.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.992073 clover-energy-5.0.7b2/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1080 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/LICENSE
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)       47 2022-11-11 16:23:59.000000 clover-energy-5.0.7b2/MANIFEST.in
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    16575 2023-02-14 09:56:25.993074 clover-energy-5.0.7b2/PKG-INFO
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    15933 2023-02-12 13:03:31.000000 clover-energy-5.0.7b2/README.md
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      103 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/pyproject.toml
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1298 2023-02-14 09:56:25.993074 clover-energy-5.0.7b2/setup.cfg
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.896025 clover-energy-5.0.7b2/src/
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.908031 clover-energy-5.0.7b2/src/clover/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    45444 2023-02-14 09:55:34.000000 clover-energy-5.0.7b2/src/clover/__main__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    93443 2023-02-14 09:55:34.000000 clover-energy-5.0.7b2/src/clover/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    36337 2023-02-12 13:03:31.000000 clover-energy-5.0.7b2/src/clover/analysis.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     8337 2023-01-27 11:10:45.000000 clover-energy-5.0.7b2/src/clover/argparser.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.909032 clover-energy-5.0.7b2/src/clover/conversion/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/conversion/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    26993 2023-02-12 13:03:31.000000 clover-energy-5.0.7b2/src/clover/conversion/conversion.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.909032 clover-energy-5.0.7b2/src/clover/conversion/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/conversion/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.910032 clover-energy-5.0.7b2/src/clover/conversion/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/conversion/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)   103637 2023-02-12 13:03:31.000000 clover-energy-5.0.7b2/src/clover/fileparser.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.915035 clover-energy-5.0.7b2/src/clover/generation/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/generation/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    19640 2022-07-26 17:20:23.000000 clover-energy-5.0.7b2/src/clover/generation/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    19468 2023-02-12 13:03:31.000000 clover-energy-5.0.7b2/src/clover/generation/solar.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.916035 clover-energy-5.0.7b2/src/clover/generation/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/generation/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.916035 clover-energy-5.0.7b2/src/clover/generation/tests/component/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/generation/tests/component/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.917036 clover-energy-5.0.7b2/src/clover/generation/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/generation/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4505 2023-01-27 11:10:45.000000 clover-energy-5.0.7b2/src/clover/generation/weather.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3514 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/generation/wind.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.920037 clover-energy-5.0.7b2/src/clover/impact/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/impact/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4199 2023-02-12 13:03:31.000000 clover-energy-5.0.7b2/src/clover/impact/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    44081 2023-02-14 09:55:34.000000 clover-energy-5.0.7b2/src/clover/impact/finance.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    30814 2023-02-12 13:03:31.000000 clover-energy-5.0.7b2/src/clover/impact/ghgs.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.923039 clover-energy-5.0.7b2/src/clover/impact/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/impact/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.924039 clover-energy-5.0.7b2/src/clover/impact/tests/component/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/impact/tests/component/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.926040 clover-energy-5.0.7b2/src/clover/impact/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/impact/tests/unit/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.934044 clover-energy-5.0.7b2/src/clover/load/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/load/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    39767 2023-02-12 13:03:31.000000 clover-energy-5.0.7b2/src/clover/load/load.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.935045 clover-energy-5.0.7b2/src/clover/load/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/load/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.935045 clover-energy-5.0.7b2/src/clover/load/tests/component/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/load/tests/component/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.936045 clover-energy-5.0.7b2/src/clover/mains_supply/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/mains_supply/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4473 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/mains_supply/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4578 2022-07-26 17:20:24.000000 clover-energy-5.0.7b2/src/clover/mains_supply/grid.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.937046 clover-energy-5.0.7b2/src/clover/mains_supply/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/mains_supply/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.937046 clover-energy-5.0.7b2/src/clover/mains_supply/tests/component/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/mains_supply/tests/component/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.937046 clover-energy-5.0.7b2/src/clover/mains_supply/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/mains_supply/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    11741 2022-07-26 17:20:24.000000 clover-energy-5.0.7b2/src/clover/mains_supply/water_source.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.939047 clover-energy-5.0.7b2/src/clover/optimisation/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/optimisation/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    42697 2023-02-12 13:06:10.000000 clover-energy-5.0.7b2/src/clover/optimisation/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    29242 2023-02-12 13:03:31.000000 clover-energy-5.0.7b2/src/clover/optimisation/appraisal.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    64522 2023-02-12 13:02:56.000000 clover-energy-5.0.7b2/src/clover/optimisation/optimisation.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    43497 2023-02-06 16:42:03.000000 clover-energy-5.0.7b2/src/clover/optimisation/single_line_simulation.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.944049 clover-energy-5.0.7b2/src/clover/optimisation/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/optimisation/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.945050 clover-energy-5.0.7b2/src/clover/optimisation/tests/component/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/optimisation/tests/component/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.946050 clover-energy-5.0.7b2/src/clover/optimisation/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/optimisation/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     8395 2023-01-27 11:10:45.000000 clover-energy-5.0.7b2/src/clover/printer.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.967061 clover-energy-5.0.7b2/src/clover/scripts/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/scripts/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1309 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/scripts/clover.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1202 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/scripts/clover_hpc_clover.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1298 2023-02-03 12:49:50.000000 clover-energy-5.0.7b2/src/clover/scripts/clover_hpc_outbox_assembly.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1138 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/scripts/clover_new_location.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1360 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/scripts/clover_update_api_token.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     6656 2023-02-12 13:02:56.000000 clover-energy-5.0.7b2/src/clover/scripts/hpc.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    10191 2022-12-06 16:49:38.000000 clover-energy-5.0.7b2/src/clover/scripts/hpc_clover.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4894 2023-02-03 12:49:50.000000 clover-energy-5.0.7b2/src/clover/scripts/hpc_outbox_assembly.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    21830 2023-02-12 13:02:56.000000 clover-energy-5.0.7b2/src/clover/scripts/hpc_utils.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    11904 2022-07-26 17:20:26.000000 clover-energy-5.0.7b2/src/clover/scripts/new_location.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.967061 clover-energy-5.0.7b2/src/clover/scripts/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/scripts/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.967061 clover-energy-5.0.7b2/src/clover/scripts/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/scripts/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3638 2022-07-26 17:20:26.000000 clover-energy-5.0.7b2/src/clover/scripts/update_api_token.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.973064 clover-energy-5.0.7b2/src/clover/simulation/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/simulation/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    20348 2023-02-12 13:03:31.000000 clover-energy-5.0.7b2/src/clover/simulation/__utils__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    12992 2023-02-12 13:03:31.000000 clover-energy-5.0.7b2/src/clover/simulation/diesel.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    88163 2023-02-14 09:55:34.000000 clover-energy-5.0.7b2/src/clover/simulation/energy_system.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     2450 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/simulation/exchanger.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    24234 2023-02-12 13:03:31.000000 clover-energy-5.0.7b2/src/clover/simulation/solar.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    30736 2023-02-12 13:03:31.000000 clover-energy-5.0.7b2/src/clover/simulation/storage.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    19002 2022-11-11 16:23:59.000000 clover-energy-5.0.7b2/src/clover/simulation/storage_utils.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.974064 clover-energy-5.0.7b2/src/clover/simulation/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/simulation/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.974064 clover-energy-5.0.7b2/src/clover/simulation/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/simulation/tests/unit/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     5411 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/simulation/transmission.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.977066 clover-energy-5.0.7b2/src/clover/src/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/src/__init__.py
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    56900 2023-02-14 09:55:34.000000 clover-energy-5.0.7b2/src/clover/src/new_location.yaml
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.979067 clover-energy-5.0.7b2/src/clover/tests/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/tests/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.980067 clover-energy-5.0.7b2/src/clover/tests/integration/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/tests/integration/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.980067 clover-energy-5.0.7b2/src/clover/tests/unit/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2022-07-26 16:30:02.000000 clover-energy-5.0.7b2/src/clover/tests/unit/__init__.py
-drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-02-14 09:56:25.992073 clover-energy-5.0.7b2/src/clover_energy.egg-info/
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)    16575 2023-02-14 09:56:25.000000 clover-energy-5.0.7b2/src/clover_energy.egg-info/PKG-INFO
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3003 2023-02-14 09:56:25.000000 clover-energy-5.0.7b2/src/clover_energy.egg-info/SOURCES.txt
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)        1 2023-02-14 09:56:25.000000 clover-energy-5.0.7b2/src/clover_energy.egg-info/dependency_links.txt
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      299 2023-02-14 09:56:25.000000 clover-energy-5.0.7b2/src/clover_energy.egg-info/entry_points.txt
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)      119 2023-02-14 09:56:25.000000 clover-energy-5.0.7b2/src/clover_energy.egg-info/requires.txt
--rw-r--r--   0 bewinche  (1000) bewinche  (1000)        7 2023-02-14 09:56:25.000000 clover-energy-5.0.7b2/src/clover_energy.egg-info/top_level.txt
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1080 2023-06-30 07:49:00.000000 clover-energy-5.0.8/LICENSE
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)       47 2023-06-30 07:49:00.000000 clover-energy-5.0.8/MANIFEST.in
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    16573 2023-07-14 14:29:36.000000 clover-energy-5.0.8/PKG-INFO
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    15933 2023-06-30 07:49:00.000000 clover-energy-5.0.8/README.md
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      103 2023-06-30 07:49:00.000000 clover-energy-5.0.8/pyproject.toml
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1296 2023-07-14 14:29:36.000000 clover-energy-5.0.8/setup.cfg
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     2049 2023-07-13 13:38:08.000000 clover-energy-5.0.8/src/clover/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    45472 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/__main__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    93443 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    36337 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/analysis.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     8337 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/argparser.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/conversion/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      710 2023-07-13 13:38:08.000000 clover-energy-5.0.8/src/clover/conversion/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    26993 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/conversion/conversion.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/conversion/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/conversion/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/conversion/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/conversion/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)   103637 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/fileparser.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/generation/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/generation/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    19640 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/generation/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    19468 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/generation/solar.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/generation/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/generation/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/generation/tests/component/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/generation/tests/component/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/generation/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/generation/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4505 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/generation/weather.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3514 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/generation/wind.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/impact/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1141 2023-07-13 13:38:08.000000 clover-energy-5.0.8/src/clover/impact/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4199 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/impact/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    44081 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/impact/finance.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    30818 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/impact/ghgs.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/impact/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/impact/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/impact/tests/component/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/impact/tests/component/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/impact/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/impact/tests/unit/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/load/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      931 2023-07-13 13:38:08.000000 clover-energy-5.0.8/src/clover/load/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    39767 2023-07-11 16:32:53.000000 clover-energy-5.0.8/src/clover/load/load.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/load/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/load/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/load/tests/component/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/load/tests/component/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/mains_supply/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      774 2023-07-13 13:38:08.000000 clover-energy-5.0.8/src/clover/mains_supply/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4473 2023-07-11 16:32:53.000000 clover-energy-5.0.8/src/clover/mains_supply/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4578 2023-07-11 16:32:53.000000 clover-energy-5.0.8/src/clover/mains_supply/grid.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/mains_supply/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/mains_supply/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/mains_supply/tests/component/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/mains_supply/tests/component/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/mains_supply/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/mains_supply/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    11741 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/mains_supply/water_source.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/optimisation/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1069 2023-07-13 13:38:08.000000 clover-energy-5.0.8/src/clover/optimisation/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    43289 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/optimisation/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    29242 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/optimisation/appraisal.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    64522 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/optimisation/optimisation.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    43497 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/optimisation/single_line_simulation.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/optimisation/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/optimisation/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/optimisation/tests/component/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/optimisation/tests/component/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/optimisation/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/optimisation/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     8395 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/printer.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/scripts/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1309 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/clover.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1202 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/clover_hpc_clover.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1298 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/clover_hpc_outbox_assembly.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1138 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/clover_new_location.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1360 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/clover_update_api_token.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     6682 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/hpc.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    10191 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/hpc_clover.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     4894 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/hpc_outbox_assembly.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    22944 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/hpc_utils.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    11904 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/new_location.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/scripts/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/scripts/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3638 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/scripts/update_api_token.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/simulation/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     1199 2023-07-13 13:38:08.000000 clover-energy-5.0.8/src/clover/simulation/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    20348 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/simulation/__utils__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    12992 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/simulation/diesel.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    88163 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/simulation/energy_system.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     2450 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/simulation/exchanger.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    24234 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/simulation/solar.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    30736 2023-07-14 14:26:32.000000 clover-energy-5.0.8/src/clover/simulation/storage.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    19002 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/simulation/storage_utils.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/simulation/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/simulation/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/simulation/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/simulation/tests/unit/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     5411 2023-07-11 16:48:20.000000 clover-energy-5.0.8/src/clover/simulation/transmission.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/src/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/src/__init__.py
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    56900 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/src/new_location.yaml
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/tests/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/tests/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/tests/integration/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:48:00.000000 clover-energy-5.0.8/src/clover/tests/integration/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover/tests/unit/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      372 2023-06-30 07:49:00.000000 clover-energy-5.0.8/src/clover/tests/unit/__init__.py
+drwxr-xr-x   0 bewinche  (1000) bewinche  (1000)        0 2023-07-14 14:29:36.000000 clover-energy-5.0.8/src/clover_energy.egg-info/
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)    16573 2023-07-14 14:29:35.000000 clover-energy-5.0.8/src/clover_energy.egg-info/PKG-INFO
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)     3003 2023-07-14 14:29:35.000000 clover-energy-5.0.8/src/clover_energy.egg-info/SOURCES.txt
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)        1 2023-07-14 14:29:35.000000 clover-energy-5.0.8/src/clover_energy.egg-info/dependency_links.txt
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      299 2023-07-14 14:29:35.000000 clover-energy-5.0.8/src/clover_energy.egg-info/entry_points.txt
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)      119 2023-07-14 14:29:35.000000 clover-energy-5.0.8/src/clover_energy.egg-info/requires.txt
+-rw-r--r--   0 bewinche  (1000) bewinche  (1000)        7 2023-07-14 14:29:35.000000 clover-energy-5.0.8/src/clover_energy.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `clover-energy-5.0.7b2/LICENSE` & `clover-energy-5.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/PKG-INFO` & `clover-energy-5.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: clover-energy
-Version: 5.0.7b2
+Version: 5.0.8
 Summary: Continuous Lifetime Optimisation of Variable Electricity Resources
-Home-page: https://github.com/phil-sandwell/CLOVER
+Home-page: https://github.com/CLOVER-energy/CLOVER
 Author: Phil Sandwell, Ben Winchester and Hamish Beath
 Author-email: philip.sandwell@gmail.com,benedict.winchester@gmail.com,hamishbeath@outlook.com
 Project-URL: Bug Tracker, https://github.com/CLOVER-energy/CLOVER/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `clover-energy-5.0.7b2/README.md` & `clover-energy-5.0.8/README.md`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/setup.cfg` & `clover-energy-5.0.8/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = clover-energy
-version = 5.0.7b2
+version = 5.0.8
 author = Phil Sandwell, Ben Winchester and Hamish Beath
 author_email = philip.sandwell@gmail.com,benedict.winchester@gmail.com,hamishbeath@outlook.com
 description = Continuous Lifetime Optimisation of Variable Electricity Resources
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/phil-sandwell/CLOVER
+url = https://github.com/CLOVER-energy/CLOVER
 project_urls = 
 	Bug Tracker = https://github.com/CLOVER-energy/CLOVER/issues
 classifiers = 
 	Programming Language :: Python :: 3.7
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
```

### Comparing `clover-energy-5.0.7b2/src/clover/__main__.py` & `clover-energy-5.0.8/src/clover/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 CLOVER (Continuous Lifetime Optimisation of Variable Electricity Resources) can evaluate
 and optimise minigrid systems, determining whether a demand is met whilst minimising
 environmental and economic impacts. The main flow of CLOVER can be executed by running
 the clover module from the command-line interface.
 
 """
 
-__version__ = "5.0.7b2"
+__version__ = "5.0.8"
 
 import datetime
 import logging
 import math
 import os
 import sys
 
@@ -1227,14 +1227,15 @@
             for appraisal in optimisation_results:
                 appraisal.system_details.file_information = input_file_info
 
             # Save the optimisation output.
             save_optimisation(
                 disable_tqdm,
                 logger,
+                optimisation,
                 optimisation_inputs,
                 optimisation_number,
                 output,
                 optimisation_output_directory,
                 optimisation.scenario,
                 optimisation_results,
             )
```

### Comparing `clover-energy-5.0.7b2/src/clover/__utils__.py` & `clover-energy-5.0.8/src/clover/__utils__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/analysis.py` & `clover-energy-5.0.8/src/clover/analysis.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/argparser.py` & `clover-energy-5.0.8/src/clover/argparser.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/conversion/conversion.py` & `clover-energy-5.0.8/src/clover/conversion/conversion.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/fileparser.py` & `clover-energy-5.0.8/src/clover/fileparser.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/generation/__utils__.py` & `clover-energy-5.0.8/src/clover/generation/__utils__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/generation/solar.py` & `clover-energy-5.0.8/src/clover/generation/solar.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/generation/weather.py` & `clover-energy-5.0.8/src/clover/generation/weather.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/generation/wind.py` & `clover-energy-5.0.8/src/clover/generation/wind.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/impact/__utils__.py` & `clover-energy-5.0.8/src/clover/impact/__utils__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/impact/finance.py` & `clover-energy-5.0.8/src/clover/impact/finance.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/impact/ghgs.py` & `clover-energy-5.0.8/src/clover/impact/ghgs.py`

 * *Files 0% similar despite different names*

```diff
@@ -920,15 +920,15 @@
             )
             for converter, size in converters.items()
         )
     else:
         logger.debug("No converters installed so no converter OM GHGs to calcualte.")
 
     diesel_om_ghgs = calculate_om_ghgs(
-        diesel_size, ghg_inputs, ImpactingComponent.PV.value, start_year, end_year
+        diesel_size, ghg_inputs, ImpactingComponent.DIESEL.value, start_year, end_year
     )
 
     general_om_ghgs = calculate_om_ghgs(
         1, ghg_inputs, ImpactingComponent.GENERAL.value, start_year, end_year
     )
 
     if (
```

### Comparing `clover-energy-5.0.7b2/src/clover/load/load.py` & `clover-energy-5.0.8/src/clover/load/load.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/mains_supply/__utils__.py` & `clover-energy-5.0.8/src/clover/mains_supply/__utils__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/mains_supply/grid.py` & `clover-energy-5.0.8/src/clover/mains_supply/grid.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/mains_supply/water_source.py` & `clover-energy-5.0.8/src/clover/mains_supply/water_source.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/optimisation/__utils__.py` & `clover-energy-5.0.8/src/clover/optimisation/__utils__.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     "Optimisation",
     "OptimisationParameters",
     "recursive_iteration",
     "save_optimisation",
     "SolarSystemSize",
     "StorageSystemSize",
     "TankSize",
+    "THRESHOLD_CRITERIA",
     "ThresholdMode",
 )
 
 # Converter name string:
 #   The name used for parsing the converter name group.
 #   NOTE: This name is not updated within the regex and needs to be updated separately.
 CONVERTER_NAME_STRING: str = "name"
@@ -78,18 +79,26 @@
 # Converter size regex:
 #   Regular expression used for parsing the size of various converters for
 # optimisations.
 #   NOTE: The name of the group is not updated automatically in accordance with the
 # above string and needs to be udpated separately.
 CONVERTER_SIZE_REGEX: Pattern[str] = re.compile(r"(?P<name>.*)_size")
 
+# Optimisation criteria:
+#   Keyword used for parsing the optimisation criteria.
+OPTIMISATION_CRITERIA: str = "optimisation_criteria"
+
 # Scenario:
 #   Keyword used for parsing the scenario to use for a given optimisation.
 SCENARIO: str = "scenario"
 
+# Threshold criteria:
+#   Keyword used for parsing the threshold criteria.
+THRESHOLD_CRITERIA: str = "threshold_criteria"
+
 
 def converters_from_sizing(converter_sizes: Dict[Converter, int]) -> List[Converter]:
     """
     Generates a `list` of available converters based on the number of each available.
 
     As the system is optimised, it becomes necessary to generate a `list` containing the
     available converters, with duplicates allowed to indiciate multiple instances of a
@@ -256,30 +265,30 @@
             - A :class:`Optimisation` instance based on the input data.
 
         """
 
         try:
             optimisation_criteria = {
                 Criterion(key): CriterionMode(value)
-                for entry in optimisation_data["optimisation_criteria"]
+                for entry in optimisation_data[OPTIMISATION_CRITERIA]
                 for key, value in entry.items()
             }
         except KeyError as e:
             logger.error(
                 "%sError processing optimisation criteria, missing entry: %s%s",
                 BColours.fail,
                 str(e),
                 BColours.endc,
             )
             raise
 
         try:
             threshold_criteria = {
                 Criterion(key): value
-                for entry in optimisation_data["threshold_criteria"]
+                for entry in optimisation_data[THRESHOLD_CRITERIA]
                 for key, value in entry.items()
             }
         except KeyError as e:
             logger.error(
                 "%sError processing threshold criteria, missing entry: %s%s",
                 BColours.fail,
                 str(e),
@@ -344,17 +353,17 @@
         }
         threshold_criteria = {
             str(key.value): float(value)
             for key, value in self.threshold_criteria.items()
         }
 
         return {
-            "optimisation_criteria": optimisation_criteria,
+            OPTIMISATION_CRITERIA: optimisation_criteria,
             "scenario": self.scenario.to_dict(),
-            "threshold_criteria": threshold_criteria,
+            THRESHOLD_CRITERIA: threshold_criteria,
         }
 
 
 @dataclasses.dataclass
 class OptimisationComponent(enum.Enum):
     """
     Contains information about the components which are variable in an optimisation.
@@ -1154,14 +1163,15 @@
     # Return the sufficient appraisals that were found at this resolution.
     return sufficient_appraisals
 
 
 def save_optimisation(
     disable_tqdm: bool,
     logger: Logger,
+    optimisation: Optimisation,
     optimisation_inputs: OptimisationParameters,
     optimisation_number: int,
     output: str,
     output_directory: str,
     scenario: Scenario,
     system_appraisals: List[SystemAppraisal],
 ) -> None:
@@ -1203,14 +1213,21 @@
         f"iteration_{index}": appraisal.to_dict()
         for index, appraisal in enumerate(system_appraisals)
     }
 
     # Add the optimisation parameter information.
     output_dict = {
         "optimisation_inputs": optimisation_inputs.to_dict(),
+        "optimisation_criteria": {
+            key.value: value.value
+            for key, value in optimisation.optimisation_criteria.items()
+        },
+        "threshold_criteria": {
+            key.value: value for key, value in optimisation.threshold_criteria.items()
+        },
         "scenario": scenario.to_dict(),
         "system_appraisals": system_appraisals_dict,
     }
 
     with tqdm(
         total=1,
         desc="saving output files",
```

### Comparing `clover-energy-5.0.7b2/src/clover/optimisation/appraisal.py` & `clover-energy-5.0.8/src/clover/optimisation/appraisal.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/optimisation/optimisation.py` & `clover-energy-5.0.8/src/clover/optimisation/optimisation.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/optimisation/single_line_simulation.py` & `clover-energy-5.0.8/src/clover/optimisation/single_line_simulation.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/printer.py` & `clover-energy-5.0.8/src/clover/printer.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/scripts/clover.py` & `clover-energy-5.0.8/src/clover/scripts/clover.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/scripts/clover_hpc_clover.py` & `clover-energy-5.0.8/src/clover/scripts/clover_hpc_clover.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/scripts/clover_hpc_outbox_assembly.py` & `clover-energy-5.0.8/src/clover/scripts/clover_hpc_outbox_assembly.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/scripts/clover_new_location.py` & `clover-energy-5.0.8/src/clover/scripts/clover_new_location.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/scripts/clover_update_api_token.py` & `clover-energy-5.0.8/src/clover/scripts/clover_update_api_token.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/scripts/hpc.py` & `clover-energy-5.0.8/src/clover/scripts/hpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     logger.info("Run successfully determined: %s", str(hpc_run))
 
     # Setup the arguments to pass to CLOVER.
     clover_arguments = [
         "--location",
         hpc_run.location,
         "--output",
-        hpc_run.output,
+        f"{hpc_run.output}_hpc_run_{run_number}",
     ]
 
     if hpc_run.total_load:
         if hpc_run.total_load_file is None:
             logger.error(
                 "%sRun %s was processed as having a total-load file but an internal "
                 "error occurred determining the total-load file name.%s",
```

### Comparing `clover-energy-5.0.7b2/src/clover/scripts/hpc_clover.py` & `clover-energy-5.0.8/src/clover/scripts/hpc_clover.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/scripts/hpc_outbox_assembly.py` & `clover-energy-5.0.8/src/clover/scripts/hpc_outbox_assembly.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/scripts/hpc_utils.py` & `clover-energy-5.0.8/src/clover/scripts/hpc_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     BColours,
     DEFAULT_SCENARIO,
     InputFileError,
     LOCATIONS_FOLDER_NAME,
     read_yaml,
 )
 from ..fileparser import INPUTS_DIRECTORY, OPTIMISATION_INPUTS_FILE, OPTIMISATIONS
-
+from ..optimisation.__utils__ import OPTIMISATION_CRITERIA, THRESHOLD_CRITERIA
 
 __all__ = (
     "HpcRunType",
     "HpcOptimisation",
     "HpcSimulation",
     "parse_args_and_hpc_input_file",
     "temporary_optimisations_file",
@@ -128,15 +128,15 @@
                 Whether a total-load file should be used.
             - total_load_file:
                 If being used, the name of the total-load file.
 
         """
 
         self.location = location
-        self.output = output
+        self._output = output
         self.total_load = total_load
         self.total_load_file = total_load_file
 
     def __init_subclass__(cls, run_type: HpcRunType) -> None:
         """
         Method run when instantiating a :class:`_BaseHpcRun` child.
 
@@ -166,14 +166,26 @@
                 f", total_load_file={self.total_load_file}"
                 if self.total_load_file is not None
                 else ""
             )
             + ")"
         )
 
+    @property
+    def output(self) -> str:
+        """
+        Return an output name for the class.
+
+        Outputs:
+            An output name for the run.
+
+        """
+
+        return self._output
+
 
 class HpcOptimisation(
     _BaseHpcRun, run_type=HpcRunType.OPTIMISATION
 ):  # pylint: disable=too-few-public-methods
     """
     Represents an optimisation to be carried out on the HPC.
 
@@ -276,14 +288,43 @@
 
         if OPTIMISATIONS in self.optimisation_inputs_data:
             return self.optimisation_inputs_data
 
         self.optimisation_inputs_data[OPTIMISATIONS] = self.optimisation
         return self.optimisation_inputs_data
 
+    @property
+    def output(self) -> str:
+        """
+        Return an output name for the class based on the optimisation criterion etc.
+
+        Outputs:
+            An output name for the run.
+
+        """
+
+        output_name: str = f"{self._output}_"
+
+        # Add the optimisation criteria information
+        for entry in self.optimisation[0][OPTIMISATION_CRITERIA]:
+            output_name += "_".join([f"{key}_{value}" for key, value in entry.items()])
+
+        output_name += "_"
+
+        # Add the threshold-criteria information
+        for entry in self.optimisation[0][THRESHOLD_CRITERIA]:
+            output_name += "_".join(
+                [
+                    f"{key}_{str(value).replace('.', '_')}"
+                    for key, value in entry.items()
+                ]
+            )
+
+        return output_name
+
 
 class HpcSimulation(
     _BaseHpcRun, run_type=HpcRunType.SIMULATION
 ):  # pylint: disable=too-few-public-methods
     """
     Representst a simulation, or multiple simulations, to be carried out on the HPC.
```

### Comparing `clover-energy-5.0.7b2/src/clover/scripts/new_location.py` & `clover-energy-5.0.8/src/clover/scripts/new_location.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/scripts/update_api_token.py` & `clover-energy-5.0.8/src/clover/scripts/update_api_token.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/simulation/__utils__.py` & `clover-energy-5.0.8/src/clover/simulation/__utils__.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/simulation/diesel.py` & `clover-energy-5.0.8/src/clover/simulation/diesel.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/simulation/energy_system.py` & `clover-energy-5.0.8/src/clover/simulation/energy_system.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/simulation/exchanger.py` & `clover-energy-5.0.8/src/clover/simulation/exchanger.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/simulation/solar.py` & `clover-energy-5.0.8/src/clover/simulation/solar.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/simulation/storage.py` & `clover-energy-5.0.8/src/clover/simulation/storage.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/simulation/storage_utils.py` & `clover-energy-5.0.8/src/clover/simulation/storage_utils.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/simulation/transmission.py` & `clover-energy-5.0.8/src/clover/simulation/transmission.py`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover/src/new_location.yaml` & `clover-energy-5.0.8/src/clover/src/new_location.yaml`

 * *Files identical despite different names*

### Comparing `clover-energy-5.0.7b2/src/clover_energy.egg-info/PKG-INFO` & `clover-energy-5.0.8/src/clover_energy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: clover-energy
-Version: 5.0.7b2
+Version: 5.0.8
 Summary: Continuous Lifetime Optimisation of Variable Electricity Resources
-Home-page: https://github.com/phil-sandwell/CLOVER
+Home-page: https://github.com/CLOVER-energy/CLOVER
 Author: Phil Sandwell, Ben Winchester and Hamish Beath
 Author-email: philip.sandwell@gmail.com,benedict.winchester@gmail.com,hamishbeath@outlook.com
 Project-URL: Bug Tracker, https://github.com/CLOVER-energy/CLOVER/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `clover-energy-5.0.7b2/src/clover_energy.egg-info/SOURCES.txt` & `clover-energy-5.0.8/src/clover_energy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

