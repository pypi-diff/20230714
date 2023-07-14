# Comparing `tmp/ansys_meshing_prime-0.4.0.dev8.tar.gz` & `tmp/ansys_meshing_prime-0.4.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_meshing_prime-0.4.0.dev8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_meshing_prime-0.4.0.dev9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_meshing_prime-0.4.0.dev8.tar` & `ansys_meshing_prime-0.4.0.dev9.tar`

### file list

```diff
@@ -1,119 +1,119 @@
--rw-r--r--   0        0        0     1090 2023-05-19 16:26:35.466403 ansys_meshing_prime-0.4.0.dev8/LICENSE
--rw-r--r--   0        0        0     3036 2023-05-19 16:26:35.466403 ansys_meshing_prime-0.4.0.dev8/README.md
--rw-r--r--   0        0        0     2029 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/pyproject.toml
--rw-r--r--   0        0        0     6098 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/__init__.py
--rw-r--r--   0        0        0     2650 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/automesh.py
--rw-r--r--   0        0        0    59522 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/automeshstructs.py
--rw-r--r--   0        0        0     6111 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py
--rw-r--r--   0        0        0     3847 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/collapsetool.py
--rw-r--r--   0        0        0    14701 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/collapsetoolstructs.py
--rw-r--r--   0        0        0    15524 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/commonstructs.py
--rw-r--r--   0        0        0     3875 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/commontypes.py
--rw-r--r--   0        0        0     9883 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/connect.py
--rw-r--r--   0        0        0    39669 2023-05-19 16:26:35.542402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/connectstructs.py
--rw-r--r--   0        0        0    10456 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/controldata.py
--rw-r--r--   0        0        0    55335 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/controlstructs.py
--rw-r--r--   0        0        0      714 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/coreobject.py
--rw-r--r--   0        0        0     3427 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/deletetool.py
--rw-r--r--   0        0        0    13990 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/deletetoolstructs.py
--rw-r--r--   0        0        0     5573 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/featureextraction.py
--rw-r--r--   0        0        0    33896 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/featureextractionstructs.py
--rw-r--r--   0        0        0    24627 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/fileio.py
--rw-r--r--   0        0        0   112910 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/fileiostructs.py
--rw-r--r--   0        0        0    60431 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/igastructs.py
--rw-r--r--   0        0        0     4093 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/materialpointmanager.py
--rw-r--r--   0        0        0    16296 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py
--rw-r--r--   0        0        0     4858 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/meshinfo.py
--rw-r--r--   0        0        0    60035 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/meshinfostructs.py
--rw-r--r--   0        0        0    16491 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/model.py
--rw-r--r--   0        0        0    27227 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/modelstructs.py
--rw-r--r--   0        0        0     3793 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/morpher.py
--rw-r--r--   0        0        0     7831 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/morpherbcsstructs.py
--rw-r--r--   0        0        0    24059 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/morpherstructs.py
--rw-r--r--   0        0        0    58131 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/part.py
--rw-r--r--   0        0        0   167481 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/partstructs.py
--rw-r--r--   0        0        0     7502 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/periodiccontrol.py
--rw-r--r--   0        0        0    13315 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py
--rw-r--r--   0        0        0    28641 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/primeconfig.py
--rw-r--r--   0        0        0     5727 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/prismcontrol.py
--rw-r--r--   0        0        0    14563 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/prismcontrolstructs.py
--rw-r--r--   0        0        0     3773 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/quadtospline.py
--rw-r--r--   0        0        0     7237 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/scaffolder.py
--rw-r--r--   0        0        0    29265 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/scaffolderstructs.py
--rw-r--r--   0        0        0    18382 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/sizecontrol.py
--rw-r--r--   0        0        0    52720 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/sizecontrolstructs.py
--rw-r--r--   0        0        0     2790 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/sizefield.py
--rw-r--r--   0        0        0    18893 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/sizefieldstructs.py
--rw-r--r--   0        0        0     4241 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/splittoolstructs.py
--rw-r--r--   0        0        0    19710 2023-05-19 16:26:35.546402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surfacesearch.py
--rw-r--r--   0        0        0   117867 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surfacesearchstructs.py
--rw-r--r--   0        0        0    22036 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surfaceutilities.py
--rw-r--r--   0        0        0   144419 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py
--rw-r--r--   0        0        0     7182 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surfer.py
--rw-r--r--   0        0        0    44962 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surferstructs.py
--rw-r--r--   0        0        0     4448 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/thinvolumecontrol.py
--rw-r--r--   0        0        0     6689 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/thinvolumecontrolstructs.py
--rw-r--r--   0        0        0     8477 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/topodata.py
--rw-r--r--   0        0        0     2646 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/topoutilities.py
--rw-r--r--   0        0        0    13167 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/topoutilitystructs.py
--rw-r--r--   0        0        0     2960 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/transform.py
--rw-r--r--   0        0        0     8727 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/transformstructs.py
--rw-r--r--   0        0        0     5980 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumecontrol.py
--rw-r--r--   0        0        0     6259 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumecontrolstructs.py
--rw-r--r--   0        0        0     4893 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumemeshtool.py
--rw-r--r--   0        0        0    29508 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py
--rw-r--r--   0        0        0     2761 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumesearch.py
--rw-r--r--   0        0        0    25492 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumesearchstructs.py
--rw-r--r--   0        0        0     4886 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumesweeper.py
--rw-r--r--   0        0        0    25535 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumesweeperstructs.py
--rw-r--r--   0        0        0     5426 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/wrapper.py
--rw-r--r--   0        0        0    10816 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/wrappercontrol.py
--rw-r--r--   0        0        0    61895 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/wrapperstructs.py
--rw-r--r--   0        0        0    13848 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/controldata.py
--rw-r--r--   0        0        0    17135 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/fileio.py
--rw-r--r--   0        0        0    10887 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/model.py
--rw-r--r--   0        0        0     4207 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/part.py
--rw-r--r--   0        0        0     2314 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/periodiccontrol.py
--rw-r--r--   0        0        0     2193 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/sizecontrol.py
--rw-r--r--   0        0        0     4091 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/surfaceutilities.py
--rw-r--r--   0        0        0     4400 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/surfer.py
--rw-r--r--   0        0        0     2308 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/volumecontrol.py
--rw-r--r--   0        0        0     2823 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/volumesweeper.py
--rw-r--r--   0        0        0     5692 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/wrapper.py
--rw-r--r--   0        0        0     2141 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/wrappercontrol.py
--rw-r--r--   0        0        0      691 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/examples/__init__.py
--rw-r--r--   0        0        0     4227 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/examples/download_utilities.py
--rw-r--r--   0        0        0    24869 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/examples/examples.py
--rw-r--r--   0        0        0     1392 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/examples/unit_test_examples.py
--rw-r--r--   0        0        0       59 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/__init__.py
--rw-r--r--   0        0        0    35690 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/graphics.py
--rw-r--r--   0        0        0     2234 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/bin.png
--rw-r--r--   0        0        0     1708 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/invert_visibility.png
--rw-r--r--   0        0        0     2510 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/parts.png
--rw-r--r--   0        0        0     1297 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/selectioninfo.png
--rw-r--r--   0        0        0     2440 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/show_edges.png
--rw-r--r--   0        0        0      203 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/show_ruler.png
--rw-r--r--   0        0        0     1547 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/surface_body.png
--rw-r--r--   0        0        0     1600 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/trame_gui.py
--rw-r--r--   0        0        0     4550 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/client.py
--rw-r--r--   0        0        0      238 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/comm_manager.py
--rw-r--r--   0        0        0      506 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/communicator.py
--rw-r--r--   0        0        0     2960 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/config.py
--rw-r--r--   0        0        0     3077 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/defaults.py
--rw-r--r--   0        0        0    34238 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/error_handling.py
--rw-r--r--   0        0        0     6130 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/grpc_communicator.py
--rw-r--r--   0        0        0      492 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/grpc_utils.py
--rw-r--r--   0        0        0     1444 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/json_utils.py
--rw-r--r--   0        0        0     8029 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/launcher.py
--rw-r--r--   0        0        0     1720 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/prime_communicator.py
--rw-r--r--   0        0        0     7632 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/utils.py
--rw-r--r--   0        0        0      143 2023-05-19 16:26:35.550402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/lucid/__init__.py
--rw-r--r--   0        0        0    68591 2023-05-19 16:26:35.554402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/lucid/mesh_util.py
--rw-r--r--   0        0        0     7399 2023-05-19 16:26:35.554402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/lucid/scope.py
--rw-r--r--   0        0        0     1493 2023-05-19 16:26:35.554402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/lucid/utils.py
--rw-r--r--   0        0        0     2059 2023-05-19 16:26:35.554402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/params/primestructs.py
--rw-r--r--   0        0        0     4345 2023-05-19 16:26:35.554402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/relaxed_json/__init__.py
--rw-r--r--   0        0        0    10039 2023-05-19 16:26:35.554402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/relaxed_json/decoder.py
--rw-r--r--   0        0        0    12256 2023-05-19 16:26:35.554402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/relaxed_json/encoder.py
--rw-r--r--   0        0        0     2623 2023-05-19 16:26:35.554402 ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/relaxed_json/scanner.py
--rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 ansys_meshing_prime-0.4.0.dev8/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-07-11 22:39:33.441578 ansys_meshing_prime-0.4.0.dev9/LICENSE
+-rw-r--r--   0        0        0     3062 2023-07-11 22:39:33.441578 ansys_meshing_prime-0.4.0.dev9/README.md
+-rw-r--r--   0        0        0     2366 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/pyproject.toml
+-rw-r--r--   0        0        0     6032 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/__init__.py
+-rw-r--r--   0        0        0     2650 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/automesh.py
+-rw-r--r--   0        0        0    59522 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/automeshstructs.py
+-rw-r--r--   0        0        0     6111 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py
+-rw-r--r--   0        0        0     3847 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/collapsetool.py
+-rw-r--r--   0        0        0    14701 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/collapsetoolstructs.py
+-rw-r--r--   0        0        0    15524 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/commonstructs.py
+-rw-r--r--   0        0        0     3875 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/commontypes.py
+-rw-r--r--   0        0        0     9883 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/connect.py
+-rw-r--r--   0        0        0    39669 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/connectstructs.py
+-rw-r--r--   0        0        0    10456 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/controldata.py
+-rw-r--r--   0        0        0    55335 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/controlstructs.py
+-rw-r--r--   0        0        0      714 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/coreobject.py
+-rw-r--r--   0        0        0     3427 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/deletetool.py
+-rw-r--r--   0        0        0    13990 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/deletetoolstructs.py
+-rw-r--r--   0        0        0     5573 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/featureextraction.py
+-rw-r--r--   0        0        0    33896 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/featureextractionstructs.py
+-rw-r--r--   0        0        0    24627 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/fileio.py
+-rw-r--r--   0        0        0   112910 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/fileiostructs.py
+-rw-r--r--   0        0        0    50117 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/igastructs.py
+-rw-r--r--   0        0        0     4093 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/materialpointmanager.py
+-rw-r--r--   0        0        0    16296 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py
+-rw-r--r--   0        0        0     4858 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/meshinfo.py
+-rw-r--r--   0        0        0    60035 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/meshinfostructs.py
+-rw-r--r--   0        0        0    16491 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/model.py
+-rw-r--r--   0        0        0    27227 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/modelstructs.py
+-rw-r--r--   0        0        0     3793 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/morpher.py
+-rw-r--r--   0        0        0     7831 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/morpherbcsstructs.py
+-rw-r--r--   0        0        0    24059 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/morpherstructs.py
+-rw-r--r--   0        0        0    58131 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/part.py
+-rw-r--r--   0        0        0   167481 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/partstructs.py
+-rw-r--r--   0        0        0     7502 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/periodiccontrol.py
+-rw-r--r--   0        0        0    13315 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py
+-rw-r--r--   0        0        0    28641 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/primeconfig.py
+-rw-r--r--   0        0        0     5727 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/prismcontrol.py
+-rw-r--r--   0        0        0    14563 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/prismcontrolstructs.py
+-rw-r--r--   0        0        0     7237 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/scaffolder.py
+-rw-r--r--   0        0        0    29265 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/scaffolderstructs.py
+-rw-r--r--   0        0        0    18382 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/sizecontrol.py
+-rw-r--r--   0        0        0    52720 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/sizecontrolstructs.py
+-rw-r--r--   0        0        0     2790 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/sizefield.py
+-rw-r--r--   0        0        0    18893 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/sizefieldstructs.py
+-rw-r--r--   0        0        0     4241 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/splittoolstructs.py
+-rw-r--r--   0        0        0    19710 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surfacesearch.py
+-rw-r--r--   0        0        0   117867 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surfacesearchstructs.py
+-rw-r--r--   0        0        0    22036 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surfaceutilities.py
+-rw-r--r--   0        0        0   144388 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py
+-rw-r--r--   0        0        0     7182 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surfer.py
+-rw-r--r--   0        0        0    44962 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surferstructs.py
+-rw-r--r--   0        0        0     4448 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/thinvolumecontrol.py
+-rw-r--r--   0        0        0     4250 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/thinvolumecontrolstructs.py
+-rw-r--r--   0        0        0     8477 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/topodata.py
+-rw-r--r--   0        0        0     2646 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/topoutilities.py
+-rw-r--r--   0        0        0    13167 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/topoutilitystructs.py
+-rw-r--r--   0        0        0     2960 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/transform.py
+-rw-r--r--   0        0        0     8727 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/transformstructs.py
+-rw-r--r--   0        0        0     5980 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumecontrol.py
+-rw-r--r--   0        0        0     6259 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumecontrolstructs.py
+-rw-r--r--   0        0        0     4893 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumemeshtool.py
+-rw-r--r--   0        0        0    29508 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py
+-rw-r--r--   0        0        0     2761 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumesearch.py
+-rw-r--r--   0        0        0    25492 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumesearchstructs.py
+-rw-r--r--   0        0        0     4886 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumesweeper.py
+-rw-r--r--   0        0        0    25535 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumesweeperstructs.py
+-rw-r--r--   0        0        0     5426 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/wrapper.py
+-rw-r--r--   0        0        0    10816 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/wrappercontrol.py
+-rw-r--r--   0        0        0    61895 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/wrapperstructs.py
+-rw-r--r--   0        0        0    13896 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/controldata.py
+-rw-r--r--   0        0        0    17050 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/fileio.py
+-rw-r--r--   0        0        0    11033 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/model.py
+-rw-r--r--   0        0        0     4181 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/part.py
+-rw-r--r--   0        0        0     2287 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/periodiccontrol.py
+-rw-r--r--   0        0        0     2208 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/sizecontrol.py
+-rw-r--r--   0        0        0     4069 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/surfaceutilities.py
+-rw-r--r--   0        0        0     4664 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/surfer.py
+-rw-r--r--   0        0        0     2309 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/volumecontrol.py
+-rw-r--r--   0        0        0     3064 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/volumesweeper.py
+-rw-r--r--   0        0        0     5981 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/wrapper.py
+-rw-r--r--   0        0        0     2115 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/wrappercontrol.py
+-rw-r--r--   0        0        0      817 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/examples/__init__.py
+-rw-r--r--   0        0        0     4566 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/examples/download_utilities.py
+-rw-r--r--   0        0        0    31534 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/examples/examples.py
+-rw-r--r--   0        0        0     1514 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/examples/unit_test_examples.py
+-rw-r--r--   0        0        0       59 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/__init__.py
+-rw-r--r--   0        0        0    41937 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/graphics.py
+-rw-r--r--   0        0        0     2234 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/bin.png
+-rw-r--r--   0        0        0     1708 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/invert_visibility.png
+-rw-r--r--   0        0        0     2510 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/parts.png
+-rw-r--r--   0        0        0     1297 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/selectioninfo.png
+-rw-r--r--   0        0        0     2440 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/show_edges.png
+-rw-r--r--   0        0        0      203 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/show_ruler.png
+-rw-r--r--   0        0        0     1547 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/surface_body.png
+-rw-r--r--   0        0        0     1612 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/trame_gui.py
+-rw-r--r--   0        0        0     5393 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/client.py
+-rw-r--r--   0        0        0      626 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/comm_manager.py
+-rw-r--r--   0        0        0     1881 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/communicator.py
+-rw-r--r--   0        0        0     4664 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/config.py
+-rw-r--r--   0        0        0     3080 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/defaults.py
+-rw-r--r--   0        0        0    36123 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/error_handling.py
+-rw-r--r--   0        0        0     8285 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/grpc_communicator.py
+-rw-r--r--   0        0        0      652 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/grpc_utils.py
+-rw-r--r--   0        0        0     2319 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/json_utils.py
+-rw-r--r--   0        0        0     8044 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/launcher.py
+-rw-r--r--   0        0        0     2084 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/logger.py
+-rw-r--r--   0        0        0     2815 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/prime_communicator.py
+-rw-r--r--   0        0        0    11476 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/utils.py
+-rw-r--r--   0        0        0      143 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/lucid/__init__.py
+-rw-r--r--   0        0        0    69132 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/lucid/mesh_util.py
+-rw-r--r--   0        0        0     7532 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/lucid/scope.py
+-rw-r--r--   0        0        0     1493 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/lucid/utils.py
+-rw-r--r--   0        0        0     2104 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/params/primestructs.py
+-rw-r--r--   0        0        0     4369 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/relaxed_json/__init__.py
+-rw-r--r--   0        0        0    13490 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/relaxed_json/decoder.py
+-rw-r--r--   0        0        0    13168 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/relaxed_json/encoder.py
+-rw-r--r--   0        0        0     3024 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/relaxed_json/scanner.py
+-rw-r--r--   0        0        0     4990 1970-01-01 00:00:00.000000 ansys_meshing_prime-0.4.0.dev9/PKG-INFO
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/LICENSE` & `ansys_meshing_prime-0.4.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/README.md` & `ansys_meshing_prime-0.4.0.dev9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 ## Overview
 
 PyPrimeMesh is a Python client to Ansys Prime Server, which
 delivers core Ansys meshing technology.
 
 ## Documentation and Issues
 
-For information on PyPrimeMesh, refer to the latest [documentation](
-https://prime.docs.pyansys.com).
+For information on PyPrimeMesh, refer to the [documentation](
+https://prime.docs.pyansys.com) for the latest stable version.
 
 For queries related to PyPrimeMesh, post on the [PyPrimeMesh Discussions](
 https://github.com/ansys/pyprimemesh/discussions) page. 
 
 For bugs or enhancement requests, post an issue on the [PyPrimeMesh Issues](
 https://github.com/ansys/pyprimemesh/issues) page. 
 
@@ -75,8 +75,8 @@
 ## License and Acknowledgments
 
 PyPrimeMesh is licensed under the MIT license.
 
 PyPrimeMesh makes no commercial claim over Ansys whatsoever. This library extends the functionality of
 Ansys Prime Server by adding a Python interface without changing the core behavior or license
 of the original software. The use of Ansys Prime Server requires a legally licensed copy of Ansys
-2023 or later.
+2023 R1 or later.
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/pyproject.toml` & `ansys_meshing_prime-0.4.0.dev9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-meshing-prime"
-version = "0.4.0.dev8"
+version = "0.4.0.dev9"
 description = "PyPrimeMesh is a Python client to Ansys Prime Server, which delivers core Ansys meshing technology."
 readme = "README.md"
 requires-python = ">=3.8,<4"
 license = {file = "LICENSE"}
 authors = [{name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"}]
 maintainers =  [{name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"}]
 classifiers = [
@@ -29,26 +29,26 @@
 ]
 
 [project.optional-dependencies]
 graphics = [
   "pyvista>=0.32.0",
 ]
 tests = [
-  "pytest==7.3.1",
-  "pytest-cov==4.0.0",
+  "pytest==7.4.0",
+  "pytest-cov==4.1.0",
   "pytest-pyvista==0.1.8",
-  "pyvista[trame]==0.38.6"
+  "pyvista[trame]==0.40.0"
 ]
 doc = [
-  "ansys-sphinx-theme==0.9.8",
+  "ansys-sphinx-theme==0.9.9",
   "jupyter-sphinx==0.4.0",
   "numpydoc==1.5.0",
-  "Sphinx==6.2.0",
-  "pyvista==0.38.6",
-  "sphinx-autodoc-typehints==1.23.0",
+  "Sphinx==7.0.1",
+  "pyvista==0.39.1",
+  "sphinx-autodoc-typehints==1.23.3",
   "sphinx-copybutton==0.5.2",
   "sphinx-gallery==0.13.0",
   "sphinx-notfound-page==0.8.3",
   "sphinxemoji==0.2.0",
 ]
 all = [
   "pyvista>=0.32.0",
@@ -83,7 +83,14 @@
   | tests
   | profiling
   | src/ansys/meshing/prime/autogen
   | .md
   | doc
 )/
 '''
+[tool.pytest.ini_options]
+minversion = "7.1"
+addopts = "-ra --cov=ansys.meshing.prime.core --cov=ansys.meshing.prime.internals --cov=ansys.meshing.prime.lucid --cov=ansys.meshing.prime.graphics --cov-report=term --cov-report=html:.cov/html --image_cache_dir tests/graphics/image_cache --add_missing_images"
+testpaths = [
+    "tests",
+]
+
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/__init__.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from ansys.meshing.prime.core.volumecontrol import VolumeControl
 
 from ansys.meshing.prime.autogen.surfaceutilitystructs import *
 from ansys.meshing.prime.autogen.wrapperstructs import *
 from ansys.meshing.prime.autogen.scaffolder import Scaffolder
 from ansys.meshing.prime.autogen.automesh import AutoMesh
 from ansys.meshing.prime.autogen.boundaryfittednurbs import BoundaryFittedSpline
-from ansys.meshing.prime.autogen.quadtospline import QuadToSpline
 from ansys.meshing.prime.autogen.sizefield import SizeField
 from ansys.meshing.prime.autogen.meshinfo import MeshInfo
 from ansys.meshing.prime.autogen.transform import Transform
 from ansys.meshing.prime.autogen.connect import Connect
 from ansys.meshing.prime.autogen.deletetool import DeleteTool
 from ansys.meshing.prime.autogen.collapsetool import CollapseTool
 from ansys.meshing.prime.autogen.volumemeshtool import VolumeMeshTool
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/automesh.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/automesh.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/automeshstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/automeshstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/collapsetool.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/collapsetool.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/collapsetoolstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/collapsetoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/commonstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/commonstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/commontypes.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/commontypes.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/connect.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/connect.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/connectstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/connectstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/controldata.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/controldata.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/controlstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/controlstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/coreobject.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/coreobject.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/deletetool.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/deletetool.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/deletetoolstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/deletetoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/featureextraction.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/featureextraction.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/featureextractionstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/featureextractionstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/fileio.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/fileio.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/fileiostructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/fileiostructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/igastructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/igastructs.py`

 * *Files 16% similar despite different names*

```diff
@@ -875,253 +875,14 @@
         """
         return self._control_point_selection_type
 
     @control_point_selection_type.setter
     def control_point_selection_type(self, value: ControlPointSelection):
         self._control_point_selection_type = value
 
-class QuadToSplineParams(CoreObject):
-    """Parameters to control conversion quadrilateral to spline.
-    """
-    _default_params = {}
-
-    def __initialize(
-            self,
-            keep_feature: bool,
-            feature_mode: bool,
-            feature_angle: float,
-            corner_angle: float,
-            pillow: bool,
-            shell_thickness: float,
-            solid_shell: bool):
-        self._keep_feature = keep_feature
-        self._feature_mode = feature_mode
-        self._feature_angle = feature_angle
-        self._corner_angle = corner_angle
-        self._pillow = pillow
-        self._shell_thickness = shell_thickness
-        self._solid_shell = solid_shell
-
-    def __init__(
-            self,
-            model: CommunicationManager=None,
-            keep_feature: bool = None,
-            feature_mode: bool = None,
-            feature_angle: float = None,
-            corner_angle: float = None,
-            pillow: bool = None,
-            shell_thickness: float = None,
-            solid_shell: bool = None,
-            json_data : dict = None,
-             **kwargs):
-        """Initializes the QuadToSplineParams.
-
-        Parameters
-        ----------
-        model: Model
-            Model to create a QuadToSplineParams object with default parameters.
-        keep_feature: bool, optional
-            Option to turn on or off feature capture.
-        feature_mode: bool, optional
-            Feature extract options.
-        feature_angle: float, optional
-            Angle to capture the feature.
-        corner_angle: float, optional
-            Corner angle of the feature.
-        pillow: bool, optional
-            Option to turn on or off pillow feature.
-        shell_thickness: float, optional
-            Thickness of shell.
-        solid_shell: bool, optional
-            Solid shell option.
-        json_data: dict, optional
-            JSON dictionary to create a QuadToSplineParams object with provided parameters.
-
-        Examples
-        --------
-        >>> quad_to_spline_params = prime.QuadToSplineParams(model = model)
-        """
-        if json_data:
-            self.__initialize(
-                json_data["keepFeature"] if "keepFeature" in json_data else None,
-                json_data["featureMode"] if "featureMode" in json_data else None,
-                json_data["featureAngle"] if "featureAngle" in json_data else None,
-                json_data["cornerAngle"] if "cornerAngle" in json_data else None,
-                json_data["pillow"] if "pillow" in json_data else None,
-                json_data["shellThickness"] if "shellThickness" in json_data else None,
-                json_data["solidShell"] if "solidShell" in json_data else None)
-        else:
-            all_field_specified = all(arg is not None for arg in [keep_feature, feature_mode, feature_angle, corner_angle, pillow, shell_thickness, solid_shell])
-            if all_field_specified:
-                self.__initialize(
-                    keep_feature,
-                    feature_mode,
-                    feature_angle,
-                    corner_angle,
-                    pillow,
-                    shell_thickness,
-                    solid_shell)
-            else:
-                if model is None:
-                    raise ValueError("Invalid assignment. Either pass model or specify all properties")
-                else:
-                    param_json = model._communicator.initialize_params(model, "QuadToSplineParams")
-                    json_data = param_json["QuadToSplineParams"] if "QuadToSplineParams" in param_json else {}
-                    self.__initialize(
-                        keep_feature if keep_feature is not None else ( QuadToSplineParams._default_params["keep_feature"] if "keep_feature" in QuadToSplineParams._default_params else (json_data["keepFeature"] if "keepFeature" in json_data else None)),
-                        feature_mode if feature_mode is not None else ( QuadToSplineParams._default_params["feature_mode"] if "feature_mode" in QuadToSplineParams._default_params else (json_data["featureMode"] if "featureMode" in json_data else None)),
-                        feature_angle if feature_angle is not None else ( QuadToSplineParams._default_params["feature_angle"] if "feature_angle" in QuadToSplineParams._default_params else (json_data["featureAngle"] if "featureAngle" in json_data else None)),
-                        corner_angle if corner_angle is not None else ( QuadToSplineParams._default_params["corner_angle"] if "corner_angle" in QuadToSplineParams._default_params else (json_data["cornerAngle"] if "cornerAngle" in json_data else None)),
-                        pillow if pillow is not None else ( QuadToSplineParams._default_params["pillow"] if "pillow" in QuadToSplineParams._default_params else (json_data["pillow"] if "pillow" in json_data else None)),
-                        shell_thickness if shell_thickness is not None else ( QuadToSplineParams._default_params["shell_thickness"] if "shell_thickness" in QuadToSplineParams._default_params else (json_data["shellThickness"] if "shellThickness" in json_data else None)),
-                        solid_shell if solid_shell is not None else ( QuadToSplineParams._default_params["solid_shell"] if "solid_shell" in QuadToSplineParams._default_params else (json_data["solidShell"] if "solidShell" in json_data else None)))
-        self._custom_params = kwargs
-        if model is not None:
-            [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
-        [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
-        lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
-        self._freeze()
-
-    @staticmethod
-    def set_default(
-            keep_feature: bool = None,
-            feature_mode: bool = None,
-            feature_angle: float = None,
-            corner_angle: float = None,
-            pillow: bool = None,
-            shell_thickness: float = None,
-            solid_shell: bool = None):
-        """Set the default values of QuadToSplineParams.
-
-        Parameters
-        ----------
-        keep_feature: bool, optional
-            Option to turn on or off feature capture.
-        feature_mode: bool, optional
-            Feature extract options.
-        feature_angle: float, optional
-            Angle to capture the feature.
-        corner_angle: float, optional
-            Corner angle of the feature.
-        pillow: bool, optional
-            Option to turn on or off pillow feature.
-        shell_thickness: float, optional
-            Thickness of shell.
-        solid_shell: bool, optional
-            Solid shell option.
-        """
-        args = locals()
-        [QuadToSplineParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
-
-    @staticmethod
-    def print_default():
-        """Print the default values of QuadToSplineParams.
-
-        Examples
-        --------
-        >>> QuadToSplineParams.print_default()
-        """
-        message = ""
-        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in QuadToSplineParams._default_params.items())
-        print(message)
-
-    def _jsonify(self) -> Dict[str, Any]:
-        json_data = {}
-        if self._keep_feature is not None:
-            json_data["keepFeature"] = self._keep_feature
-        if self._feature_mode is not None:
-            json_data["featureMode"] = self._feature_mode
-        if self._feature_angle is not None:
-            json_data["featureAngle"] = self._feature_angle
-        if self._corner_angle is not None:
-            json_data["cornerAngle"] = self._corner_angle
-        if self._pillow is not None:
-            json_data["pillow"] = self._pillow
-        if self._shell_thickness is not None:
-            json_data["shellThickness"] = self._shell_thickness
-        if self._solid_shell is not None:
-            json_data["solidShell"] = self._solid_shell
-        [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
-        return json_data
-
-    def __str__(self) -> str:
-        message = "keep_feature :  %s\nfeature_mode :  %s\nfeature_angle :  %s\ncorner_angle :  %s\npillow :  %s\nshell_thickness :  %s\nsolid_shell :  %s" % (self._keep_feature, self._feature_mode, self._feature_angle, self._corner_angle, self._pillow, self._shell_thickness, self._solid_shell)
-        message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
-        return message
-
-    @property
-    def keep_feature(self) -> bool:
-        """Option to turn on or off feature capture.
-        """
-        return self._keep_feature
-
-    @keep_feature.setter
-    def keep_feature(self, value: bool):
-        self._keep_feature = value
-
-    @property
-    def feature_mode(self) -> bool:
-        """Feature extract options.
-        """
-        return self._feature_mode
-
-    @feature_mode.setter
-    def feature_mode(self, value: bool):
-        self._feature_mode = value
-
-    @property
-    def feature_angle(self) -> float:
-        """Angle to capture the feature.
-        """
-        return self._feature_angle
-
-    @feature_angle.setter
-    def feature_angle(self, value: float):
-        self._feature_angle = value
-
-    @property
-    def corner_angle(self) -> float:
-        """Corner angle of the feature.
-        """
-        return self._corner_angle
-
-    @corner_angle.setter
-    def corner_angle(self, value: float):
-        self._corner_angle = value
-
-    @property
-    def pillow(self) -> bool:
-        """Option to turn on or off pillow feature.
-        """
-        return self._pillow
-
-    @pillow.setter
-    def pillow(self, value: bool):
-        self._pillow = value
-
-    @property
-    def shell_thickness(self) -> float:
-        """Thickness of shell.
-        """
-        return self._shell_thickness
-
-    @shell_thickness.setter
-    def shell_thickness(self, value: float):
-        self._shell_thickness = value
-
-    @property
-    def solid_shell(self) -> bool:
-        """Solid shell option.
-        """
-        return self._solid_shell
-
-    @solid_shell.setter
-    def solid_shell(self, value: bool):
-        self._solid_shell = value
-
 class RefineSplineParams(CoreObject):
     """Spline refinement parameters.
     """
     _default_params = {}
 
     def __initialize(
             self,
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/materialpointmanager.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/materialpointmanager.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/meshinfo.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/meshinfo.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/meshinfostructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/meshinfostructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/model.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/model.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/modelstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/modelstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/morpher.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/morpher.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/morpherbcsstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/morpherbcsstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/morpherstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/morpherstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/part.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/part.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/partstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/partstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/periodiccontrol.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/periodiccontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/primeconfig.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/primeconfig.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/prismcontrol.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/prismcontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/prismcontrolstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/prismcontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/scaffolder.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/scaffolder.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/scaffolderstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/scaffolderstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/sizecontrol.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/sizecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/sizecontrolstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/sizecontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/sizefield.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/sizefield.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/sizefieldstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/sizefieldstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/splittoolstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/splittoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surfacesearch.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surfacesearch.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surfacesearchstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surfacesearchstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surfaceutilities.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surfaceutilities.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,15 +289,15 @@
         return self._error_code
 
     @error_code.setter
     def error_code(self, value: ErrorCode):
         self._error_code = value
 
 class CopyZoneletsParams(CoreObject):
-    """Parameters to copy zonelets. This is for internal use only.
+    """Parameters to copy zonelets.
     """
     _default_params = {}
 
     def __initialize(
             self):
         pass
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surfer.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surfer.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/surferstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surferstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/thinvolumecontrol.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/thinvolumecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/topodata.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/topodata.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/topoutilities.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/topoutilities.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/topoutilitystructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/topoutilitystructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/transform.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/transform.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/transformstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/transformstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumecontrol.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumecontrolstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumecontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumemeshtool.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumemeshtool.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumesearch.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumesearch.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumesearchstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumesearchstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumesweeper.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumesweeper.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/volumesweeperstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumesweeperstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/wrapper.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/wrapper.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/wrappercontrol.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/wrappercontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/autogen/wrapperstructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/wrapperstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/controldata.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/controldata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Module for control data."""
 from typing import Iterable, List
 
 # isort: split
 from ansys.meshing.prime.autogen.controldata import ControlData as _ControlData
 
 # isort: split
 from ansys.meshing.prime.autogen.commonstructs import DeleteResults
@@ -13,231 +14,234 @@
 from ansys.meshing.prime.core.volumecontrol import VolumeControl
 from ansys.meshing.prime.core.wrappercontrol import WrapperControl
 from ansys.meshing.prime.internals.comm_manager import CommunicationManager
 from ansys.meshing.prime.params.primestructs import SizingType
 
 
 class ControlData(_ControlData):
-    """ControlData acts as a container for all controls (size controls, prism controls,
-    wrapper controls, etc).
+    """Contains all controls.
+
+    This class contains all controls, including size controls, prism controls,
+    and wrapper controls.
+
+    Parameters
+    ----------
+    model : CommunicationManager
+        Communicator with the server.
+    id : int
+        ID of the model.
+    object_id : int
+        ID of the object.
+    name : str
+        Name of the control.
 
     """
 
     def __init__(self, model: CommunicationManager, id: int, object_id: int, name: str):
-        """Initializes ControlData"""
+        """Initialize the ``ControlData`` class."""
         self._model = model
         self._wrapper_controls = []
         self._size_controls = []
         self._prism_controls = []
         self._thin_volume_controls = []
         self._volume_controls = []
         self._periodic_controls = []
         _ControlData.__init__(self, model, id, object_id, name)
 
     def get_wrapper_control_by_name(self, name) -> WrapperControl:
-        """Gets the wrapper control by name.
-
+        """Get the wrapper control by name.
 
         Parameters
         ----------
         name : str
             Name of the wrapper control.
 
         Returns
         -------
         WrapperControl
-            Returns the wrapper control.
+            Wrapper control.
 
         Examples
         --------
         >>> wrapper_control = model.control_data.get_wrapper_control_by_name("wrappercontrol-1")
 
         """
         for wc in self._wrapper_controls:
             if wc.name == name:
                 return wc
         return None
 
     def create_size_control(self, sizing_type: SizingType) -> SizeControl:
-        """Creates size control for the given sizing type.
-
+        """Create a size control for a sizing type.
 
         Parameters
         ----------
         type : SizingType
-            Sizing type used to create a size control.
+            Sizing type for creating the size control.
 
         Returns
         -------
         SizeControl
-            Returns the size control.
+            Size control.
 
         Notes
         -----
-        An empty size control is created on calling this API.
+        An empty size control is created on calling this method.
 
         Examples
         --------
         >>> size_control = model.control_data.create_size_control(SizingType.Curvature)
 
         """
         res = _ControlData.create_size_control(self, sizing_type)
         new_size_control = SizeControl(self._model, res[0], res[1], res[2])
         self._size_controls.append(new_size_control)
         return new_size_control
 
     def create_prism_control(self) -> PrismControl:
-        """Creates a PrismControl.
-
+        """Create a prism control.
 
         Returns
         -------
         PrismControl
-            Returns PrismControl.
+            Prism control.
 
 
         Examples
         --------
         >>> prism_control = model.control_data.create_prism_control()
 
         """
         res = _ControlData.create_prism_control(self)
         new_prism_control = PrismControl(self._model, res[0], res[1], res[2])
         self._prism_controls.append(new_prism_control)
         return new_prism_control
 
     def create_thin_volume_control(self) -> ThinVolumeControl:
-        """Creates a ThinVolumeControl.
-
+        """Create a thin volume control.
 
         Returns
         -------
         ThinVolumeControl
-            Returns ThinVolumeControl.
-
+            Thin volume control.
 
         Examples
         --------
         >>> thin_volume_control = model.control_data.create_thin_volume_control()
 
         """
         res = _ControlData.create_thin_volume_control(self)
         new_thin_volume_control = ThinVolumeControl(self._model, res[0], res[1], res[2])
         self._thin_volume_controls.append(new_thin_volume_control)
         return new_thin_volume_control
 
     def create_wrapper_control(self) -> WrapperControl:
-        """Creates wrapper control with defaults.
-
+        """Create a wrapper control with default values.
 
         Returns
         -------
         WrapperControl
-            Returns the wrapper control.
+            Wrapper control.
 
         Notes
         -----
-        A wrapper control with defaults is created on calling this API.
+        A wrapper control with default values is created on calling this method.
 
         Examples
         --------
         >>> wrapper_control = model.control_data.create_wrapper_control()
 
         """
         res = _ControlData.create_wrapper_control(self)
         new_control = WrapperControl(self._model, res[0], res[1], res[2])
         self._wrapper_controls.append(new_control)
         return new_control
 
     def get_size_control_by_name(self, name: str) -> SizeControl:
-        """Gets the size control by name.
-
+        """Get a size control by name.
 
         Parameters
         ----------
         name : str
             Name of the size control.
 
         Returns
         -------
         SizeControl
-            Returns the size control.
+            Size control.
 
         Examples
         --------
         >>> size_control = model.control_data.get_size_control_by_name("SizeControl-1")
 
         """
         for size_control in self._size_controls:
             if size_control.name == name:
                 return size_control
         return None
 
     def get_prism_control_by_name(self, name: str) -> PrismControl:
-        """Gets the prism control by name.
-
+        """Get a prism control by name.
 
         Parameters
         ----------
         name : str
             Name of the prism control.
 
         Returns
         -------
         PrismControl
-            Returns the prism control.
+            Prism control.
 
         Examples
         --------
         >>> prism_control = model.control_data.get_prism_control_by_name("PrismControl-1")
 
         """
         for prism_control in self._prism_controls:
             if prism_control.name == name:
                 return prism_control
         return None
 
     def get_thin_volume_control_by_name(self, name: str) -> ThinVolumeControl:
-        """Gets the thin volume control with the given name.
-
+        """Get a thin volume control by name.
 
         Parameters
         ----------
         name : str
             Name of the thin volume control.
 
         Returns
         -------
         ThinVolumeControl
-            Returns the thin volume control.
+            Thin volume control.
 
         Examples
         --------
         >>> contorl_data = model.control_data
         >>> thin_volume_control = control_data.get_thin_volume_control_by_name(
                                                      "ThinVolumeControl-1")
         """
         for thin_volume_control in self._thin_volume_controls:
             if thin_volume_control.name == name:
                 return thin_volume_control
         return None
 
     def delete_controls(self, control_ids: Iterable[int]) -> DeleteResults:
-        """Deletes the control for the given id.
-
+        """Delete the control for one or more IDs.
 
         Parameters
         ----------
         control_ids : Iterable[int]
-            List of control ids.
+            List of control IDs.
 
         Returns
         -------
         DeleteResults
-            Returns the DeleteResults.
+            Delete results.
 
         Examples
         --------
         >>> results = model.control_data.delete_controls([size_control.id, volume_control.id])
 
         """
         res = _ControlData.delete_controls(self, control_ids=control_ids)
@@ -286,44 +290,43 @@
 
     def _update_thin_volume_controls(self, c_data: List):
         self._thin_volume_controls = [
             ThinVolumeControl(self._model, c[0], c[1], c[2]) for c in c_data
         ]
 
     def create_volume_control(self) -> VolumeControl:
-        """Creates the volume control.
+        """Create a volume control.
 
         Returns
         -------
         VolumeControl
-            Returns the volume control.
+            Volume control.
 
         Examples
         --------
         >>> volume_control = model.control_data.create_volume_control()
 
         """
         res = _ControlData.create_volume_control(self)
         new_control = VolumeControl(self._model, res[0], res[1], res[2])
         self._volume_controls.append(new_control)
         return new_control
 
     def get_volume_control_by_name(self, name: str) -> VolumeControl:
-        """Gets the volume control by name.
-
+        """Get a volume control by name.
 
         Parameters
         ----------
         name : str
             Name of the volume control.
 
         Returns
         -------
         VolumeControl
-            Returns the volume control.
+            Volume control.
 
         Examples
         --------
         >>> volume_control = model.control_data.get_volume_control_by_name("VolumeControl-1")
 
         """
         for volume_control in self._volume_controls:
@@ -334,45 +337,45 @@
     @property
     def size_controls(self) -> List[SizeControl]:
         """Get the size controls.
 
         Returns
         -------
         List[SizeControl]
-            Returns the list of size controls.
+            List of size controls.
 
         Examples
         --------
             >>> size_controls = model.control_data.size_controls
         """
         return self._size_controls
 
     @property
     def volume_controls(self) -> List[VolumeControl]:
         """Get the volume controls.
 
         Returns
         -------
         List[VolumeControl]
-            Returns the list of volume controls.
+            List of volume controls.
 
         Examples
         --------
             >>> volume_controls = model.control_data.volume_controls
         """
         return self._volume_controls
 
     @property
     def prism_controls(self) -> List[PrismControl]:
         """Get the prism controls.
 
         Returns
         -------
         List[PrismControl]
-            Returns the list of prism controls.
+            List of prism controls.
 
         Examples
         --------
         >>> prism_control = model.control_data.prism_controls
 
         """
         return self._prism_controls
@@ -380,15 +383,15 @@
     @property
     def thin_volume_controls(self) -> List[ThinVolumeControl]:
         """Get the thin volume controls.
 
         Returns
         -------
         List[ThinVolumeControl]
-            Returns the list of thin volume controls.
+            List of thin volume controls.
 
         Examples
         --------
         >>> thin_volume_control = model.control_data.thin_volume_controls
 
         """
         return self._thin_volume_controls
@@ -396,54 +399,53 @@
     @property
     def wrapper_controls(self) -> List[WrapperControl]:
         """Get the wrapper controls.
 
         Returns
         -------
         List[WrapperControl]
-            Returns the list of wrapper controls.
+            List of wrapper controls.
 
         Examples
         --------
         >>> wrapper_control = model.control_data.wrapper_controls
 
         """
         return self._wrapper_controls
 
     def create_periodic_control(self) -> PeriodicControl:
-        """Creates the periodic control.
+        """Create a periodic control.
 
         Returns
         -------
         PeriodicControl
-            Returns the periodic control.
+            Periodic control.
 
         Examples
         --------
         >>> periodic_control = model.control_data.create_periodic_control()
 
         """
         res = _ControlData.create_periodic_control(self)
         new_control = PeriodicControl(self._model, res[0], res[1], res[2])
         self._periodic_controls.append(new_control)
         return new_control
 
     def get_periodic_control_by_name(self, name: str) -> PeriodicControl:
-        """Gets the periodic control by name.
-
+        """Get a periodic control by name.
 
         Parameters
         ----------
         name : str
             Name of the periodic control.
 
         Returns
         -------
         PeriodicControl
-            Returns the periodic control.
+            Periodic control.
 
         Examples
         --------
         >>> periodic_control = model.control_data.get_periodic_control_by_name("PeriodicControl-1")
 
         """
         for periodic_control in self._periodic_controls:
@@ -454,14 +456,14 @@
     @property
     def periodic_controls(self) -> List[PeriodicControl]:
         """Get the periodic controls.
 
         Returns
         -------
         List[PeriodicControl]
-            Returns the list of periodic controls.
+            List of periodic controls.
 
         Examples
         --------
             >>> periodic_controls = model.control_data.periodic_controls
         """
         return self._periodic_controls
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/fileio.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/fileio.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Module containing file input and output related classes and methods."""
+"""Module for mangaging file inputs and outputs."""
 from typing import List
 
 # isort: split
 from ansys.meshing.prime.autogen.fileio import FileIO as _FileIO
 
 # isort: split
 import ansys.meshing.prime.internals.utils as utils
@@ -30,49 +30,47 @@
     WriteSizeFieldParams,
 )
 from ansys.meshing.prime.core.model import Model
 from ansys.meshing.prime.params.primestructs import ErrorCode
 
 
 class FileIO(_FileIO):
-    """Input and output managing class.
+    """Manages file inputs and outputs.
 
     Parameters
     ----------
     model : Model
-        Server model where to create and modify WrapperControls from.
+        Server model from which to create and modify wrapper controls.
     """
 
     __doc__ = _FileIO.__doc__
 
     def __init__(self, model: Model):
         """Initialize model and parent class."""
         self._model = model
         super().__init__(model)
 
     def read_pmdat(self, file_name: str, file_read_params: FileReadParams) -> FileReadResults:
-        """Read PyPrimeMesh data file.
-
-        PyPrimeMesh data files have pmdat extension.
+        """Read a PyPrimeMesh data (PMDAT) file.
 
         Parameters
         ----------
         file_name : str
-            Path to file on disk.
+            Path to the data file on disk.
         file_read_params : FileReadParams
-            Parameter to read a file.
+            Parameters for reading the data file.
 
         Returns
         -------
         FileReadResults
-            Return FileReadResults.
+            Results from reading the data file.
 
         Notes
         -----
-        This API does not support Unicode paths now.
+        This method does not support Unicode paths.
 
         Examples
         --------
         >>> import ansys.meshing.prime as prime
         >>> #connect client to server and get model from it
         >>> client = prime.Client(ip="localhost", port=50060)
         >>> model = client.model
@@ -84,147 +82,143 @@
         with utils.file_read_context(self._model, file_name) as temp_file_name:
             result = super().read_pmdat(temp_file_name, file_read_params)
             if result.error_code == ErrorCode.NOERROR:
                 self._model._sync_up_model()
         return result
 
     def write_pmdat(self, file_name: str, file_write_params: FileWriteParams) -> FileWriteResults:
-        """Write PyPrimeMesh data file. PyPrimeMesh data files have .pmdat extension.
+        """Write a PyPrimeMesh data (PMDAT) file.
 
         Parameters
         ----------
         file_name : str
-            Path to write file on disk.
+            Path for writing the data file on disk.
         file_write_params : FileWriteParams
-            Parameters to write PyPrimeMesh data file.
+            Parameters for writing the data file.
 
         Returns
         -------
         FileWriteResults
-            Return the FileWriteResults structure.
+            Results from writing the data file.
 
         Examples
         --------
         >>> results = file_io.write_pmdat("/tmp/prime_mesh_data.pmdat",
                                           prime.FileWriteParams(model=model))
         """
         with utils.file_write_context(self._model, file_name) as temp_file_name:
             result = super().write_pmdat(temp_file_name, file_write_params)
         return result
 
     def import_fluent_meshing_size_field(self, file_name: str) -> SizeFieldFileReadResults:
-        """Import Fluent Meshing sizefield file from disk.
-
-        Fluent Meshing sizefield files have sf and sf.gz extension.
+        """Import a Fluent Meshing size field (SF and SF.GZ) file from disk.
 
         Parameters
         ----------
         file_name : str
-            Path to file on disk
+            Path to the size field file on disk.
 
         Returns
         -------
         SizeFieldFileReadResults
-            Return the SizeFieldFileReadResults.
+            Results from reading the size field file.
 
         Notes
         -----
-        This API does not support Unicode paths now.
+        This method does not support Unicode paths.
 
         Examples
         --------
         >>> file_io = prime.FileIO(model=model)
         >>> results = file_io.import_fluent_meshing_size_field("/tmp/my_sizefield.sf")
         """
         with utils.file_read_context(self._model, file_name) as temp_file_name:
             result = super().import_fluent_meshing_size_field(temp_file_name)
         return result
 
     def read_size_field(
         self, file_name: str, params: ReadSizeFieldParams
     ) -> SizeFieldFileReadResults:
-        """Read PyPrimeMesh sizefield file from disk.
-
-        PyPrimeMesh sizefield files have psf and psf.gz extension.
+        """Read a PyPrimeMesh size field (PSF and PSF.GZ) file from disk.
 
         Parameters
         ----------
         file_name : str
-            Path to file on disk.
+            Path to the size field file on disk.
         params : ReadSizeFieldParams
-            Parameters to read size field file.
+            Parameters for reading size field file.
 
         Returns
         -------
         SizeFieldFileReadResults
-            Return the SizeFieldFileReadResults.
+            Results from reading the size field file.
 
         Notes
         -----
-        This API does not support Unicode paths now.
+        This method does not support Unicode paths.
 
         Examples
         --------
         >>> file_io = prime.FileIO(model=model)
         >>> params = prime.ReadSizeFieldParams(model=model)
         >>> results = file_io.read_size_field("/tmp/my_prime_sizefield.psf", params)
         """
         with utils.file_read_context(self._model, file_name) as temp_file_name:
             result = super().read_size_field(temp_file_name, params)
         return result
 
     def write_size_field(self, file_name: str, params: WriteSizeFieldParams) -> FileWriteResults:
-        """Write PyPrimeMesh sizefield (.psf) to file.
+        """Write a PyPrimeMesh size field (PSF) file to a file on disk.
 
         Parameters
         ----------
         file_name : str
-            Path to file on disk.
+            Path to the size field file on disk.
         params : WriteSizeFieldParams
-            Parameters to write size field file.
+            Parameters for writing the size field file.
 
         Returns
         -------
         FileWriteResults
-            Return the FileWriteResults.
+            Results from writing the size field file.
 
         Notes
         -----
-        This API does not support Unicode paths now.
+        This method does not support Unicode paths.
 
         Examples
         --------
         >>> file_io = prime.FileIO(model=model)
         >>> params = prime.WriteSizeFieldParams(model=model)
         >>> results = file_io.write_size_field("/tmp/my_prime_sizefield.psf", params)
         """
         with utils.file_write_context(self._model, file_name) as temp_file_name:
             result = super().write_size_field(temp_file_name, params)
         return result
 
     def import_mapdl_cdb(
         self, file_name: str, params: ImportMapdlCdbParams
     ) -> ImportMapdlCdbResults:
-        """Open MAPDL CDB file(cdb).
+        """Import an MAPDL CDB file.
 
         Parameters
         ----------
         file_name : str
-            Path to file on disk.
+            Path to the CDB file on disk.
         params : ImportMapdlCdbParams
-            Parameter to import a CDB file.
+            Parameters for importing the CDB file.
 
         Returns
         -------
         ImportMapdlCdbResults
-            Return ImportMapdlCdbResults.
+            Results from importing the CDB file.
 
         Notes
         -----
-        This API does not support Unicode paths now.
+        This method does not support Unicode paths.
 
         Examples
         --------
         >>> import ansys.meshing.prime as prime
         >>> # connect client to server and get model from it
         >>> client = prime.Client(ip="localhost", port=50060)
         >>> model = client.model
@@ -237,31 +231,31 @@
             if result.error_code == ErrorCode.NOERROR:
                 self._model._sync_up_model()
         return result
 
     def export_mapdl_cdb(
         self, file_name: str, params: ExportMapdlCdbParams
     ) -> ExportMapdlCdbResults:
-        """Export MAPDL CDB file(cdb).
+        """Export an MAPDL CDB file.
 
         Parameters
         ----------
         file_name : str
-            Path to file on disk.
+            Path to the CDB file on disk.
         params : ExportMapdlCdbParams
-            Parameter to export a CDB file.
+            Parameters for exporting the CDB file.
 
         Returns
         -------
         ExportMapdlCdbResults
-            Return ExportMapdlCdbResults.
+            Results from exporting the CDB file.
 
         Notes
         -----
-        This API does not support Unicode paths now.
+        This method does not support Unicode paths.
 
         Examples
         --------
         >>> import ansys.meshing.prime as prime
         >>> #connect client to server and get model from it
         >>> client = prime.Client(ip="localhost", port=50060)
         >>> model = client.model
@@ -274,34 +268,32 @@
         return result
 
     def import_fluent_meshing_meshes(
         self,
         file_names: List[str],
         import_fluent_meshing_mesh_params: ImportFluentMeshingMeshParams,
     ) -> ImportFluentMeshingMeshResults:
-        """Import Fluent Meshing meshes of given files on disk.
-
-        Fluent Meshing mesh files have msh and msh.gz extension.
+        """Import Fluent Meshing's mesh (MS and MSH.GZ) files from disk.
 
         Parameters
         ----------
         file_names : List[str]
-            Full path of files to be imported.
+            List of full path for the mesh files to import.
         import_fluent_meshing_mesh_params : ImportFluentMeshingMeshParams
-            Parameters to import Fluent Meshing mesh.
+            Parameters for importing the mesh files.
 
         Returns
         -------
         ImportFluentMeshingMeshResults
-            Return the FileReadResults.
+            Results from importing the mesh files.
 
 
         Notes
         -----
-        This API does not support Unicode paths now.
+        This method does not support Unicode paths.
 
         Examples
         --------
         >>> file_io = prime.FileIO(model=model)
         >>> params = prime.ImportFluentMeshingMeshParams(model=model)
         >>> results = file_io.import_fluent_meshing_meshes(
                         ["/tmp/mesh.msh", "/tmp/mesh1.msh"],
@@ -315,34 +307,32 @@
         if result.error_code == ErrorCode.NOERROR:
             self._model._sync_up_model()
         return result
 
     def import_fluent_case(
         self, file_name: str, import_fluent_case_params: ImportFluentCaseParams
     ) -> ImportFluentCaseResults:
-        """Import Fluent case file on disk.
-
-        Fluent case files have cas extension.
+        """Import a Fluent case (CAS) file from disk.
 
         Parameters
         ----------
         file_name : str
-            Path to file on disk.
+            Path to the case file on disk.
         import_fluent_case_params : ImportFluentCaseParams
-            Parameters to import fluent case file.
+            Parameters for importing the case file.
 
         Returns
         -------
         ImportFluentCaseResults
-            Return the ImportFluentCaseResults.
+            Results from importing the case file.
 
 
         Notes
         -----
-        This API does not support Unicode paths now.
+        This method does not support Unicode paths.
 
         Examples
         --------
         >>> file_io = prime.FileIO(model=model)
         >>> params = prime.ImportFluentCaseParams(model=model)
         >>> results = file_io.import_fluent_case("/tmp/fluent.cas", params)
 
@@ -352,27 +342,27 @@
             if result.error_code == ErrorCode.NOERROR:
                 self._model._sync_up_model()
         return result
 
     def export_fluent_case(
         self, file_name: str, export_fluent_case_params: ExportFluentCaseParams
     ) -> FileWriteResults:
-        """Export Fluent case file. Fluent case files have cas extension.
+        """Export a Fluent case (CAS) file.
 
         Parameters
         ----------
         file_name : str
-            Path to file on disk.
+            Path to the case file on disk.
         export_fluent_case_params : ExportFluentCaseParams
-            Parameters to export fluent case file.
+            Parameters for exporting the case file.
 
         Returns
         -------
         FileWriteResults
-            Return the FileWriteResults structure.
+            Results from exporting the case file.
 
         Examples
         --------
         >>> file_io = FileIO(model=model)
         >>> results = file_io.export_fluent_case(
                         "/tmp/fluent.cas",
                         prime.ExportFluentCaseParams(model=model))
@@ -380,97 +370,95 @@
         with utils.file_write_context(self._model, file_name) as temp_file_name:
             result = super().export_fluent_case(temp_file_name, export_fluent_case_params)
         return result
 
     def export_fluent_meshing_mesh(
         self, file_name: str, export_fluent_mesh_params: ExportFluentMeshingMeshParams
     ) -> FileWriteResults:
-        """Export Fluent Meshing mesh file. Fluent Meshing mesh files have .msh extension.
+        """Export a Fluent Meshing mesh (MSH) file.
 
         Parameters
         ----------
         file_name : str
-            Path to file on disk.
+            Path to the mesh file on disk.
         export_fluent_mesh_params : ExportFluentMeshingMeshParams
-            Parameters to export Fluent Meshing mesh file.
+            Parameters for exporting the mesh file.
 
         Returns
         -------
         FileWriteResults
-            Return the FileWriteResults structure.
+            Results from exporting the mesh file.
 
         Examples
         --------
         >>> results = file_io.export_fluent_meshing_mesh(
                         "/tmp/fluent_meshing.msh",
                         ExportFluentMeshingMeshParams(model=model))
         """
         with utils.file_write_context(self._model, file_name) as temp_file_name:
             result = super().export_fluent_meshing_mesh(temp_file_name, export_fluent_mesh_params)
         return result
 
     def export_boundary_fitted_spline_kfile(
         self, file_name: str, export_params: ExportBoundaryFittedSplineParams
     ) -> FileWriteResults:
-        """Export IGA LS-DYNA Keyword file for boundary fitted spline.
+        """Export the IGA LS-DYNA keyword file for a boundary fitted spline.
 
         Parameters
         ----------
         file_name : str
-            Name of the file.
+            Name of the keyword file.
         export_params : ExportBoundaryFittedSplineParams
-            Parameters for IGA LS-DYNA Keyword file export.
+            Parameters for exporting the keyword file.
 
         Returns
         -------
         FileWriteResults
-            Return FileWriteResults.
+            Results from exporting the keyword file.
 
         Examples
         --------
         >>> results = file_io.export_boundary_fitted_spline_k_file(
                         file_name,
                         ExportBoundaryFittedSplineParams(model=model))
         """
         with utils.file_write_context(self._model, file_name) as temp_file_name:
             result = super().export_boundary_fitted_spline_kfile(temp_file_name, export_params)
         return result
 
     def import_cad(self, file_name: str, params: ImportCadParams) -> ImportCadResults:
-        r"""Open CAD file.
-
-        Import CAD file from disk.
+        r"""Import a CAD file from disk.
 
-        Supported formats on Windows are:
+        Supported CAD file formats on Windows are:
 
         \*.scdoc \*.fmd \*.agdb \*.pmdb \*.meshdat \*.mechdat \*.dsdb \*.cmdb \*.sat \*.sab
         \*.dwg \*.dxf \*.model \*.exp \*.CATPart \*.CATProduct \*.cgr \*.3dxml \*.prt\* \*.asm\*
         \*.iges \*.igs \*.ipt \*.iam \*.jt \*.prt \*.x_t \*.x_b \*.par \*.psm \*.asm \*.sldprt
         \*.sldasm \*.step \*.stp \*.stl \*.plmxml \*.tgf
 
-        Supported formats on Linux are:
+        Supported CAD file formats on Linux are:
 
         \*.fmd \*.agdb \*.pmdb \*.meshdat \*.mechdat \*.dsdb \*.cmdb \*.sat \*.sab
         \*.CATPart \*.CATProduct \*.iges \*.igs \*.jt \*.x_t \*.x_b \*.step \*.stp
         \*.stl \*.plmxml \*.tgf
 
-        Refer documentation for detailed list of supported formats.
+        See the documentation for a comprehensive list of supported formats.
 
         Parameters
         ----------
         file_name : str
-             Path to file on disk.
+            Path to the CAD file on disk.
 
         params : ImportCadParams
-             Parameters to control CAD import options
+            Parameters for importing the CAD file.
 
         Returns
         -------
         ImportCadResults
-             Return ImportCadResults.
+            Results from importing the CAD file.
 
         Examples
         --------
         >>> import ansys.meshing.prime as prime
         >>> # connect client to server and get model from it
         >>> client = prime.Client(ip="localhost", port=50060)
         >>> model = client.model
@@ -483,33 +471,31 @@
         with utils.file_read_context(self._model, file_name) as temp_file_name:
             import_result = super().import_cad(temp_file_name, params)
             if import_result.error_code == ErrorCode.NOERROR:
                 self._model._sync_up_model()
         return import_result
 
     def export_stl(self, file_name: str, params: ExportSTLParams) -> FileWriteResults:
-        """Export STL file.
-
+        """Export an STL file.
 
         Parameters
         ----------
         file_name : str
-            Path to file on disk.
+            Path to the STL file on disk.
         params : ExportSTLParams
-            Parameters for writing the file.
+            Parameters for exporting the STL file.
 
         Returns
         -------
         FileWriteResults
-            Returns the FileWriteResults.
-
+            Results from exporting the STL file.
 
         Notes
         -----
-        This API does not support Unicode paths now.
+        This method does not support Unicode paths.
 
         Examples
         --------
         >>> import ansys.meshing.prime as prime
         >>> model = prime.local_model()
         >>> fileio = prime.FileIO(model=model)
         >>> out_file_path = r"/tmp/output.stl"
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/model.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Module containing managing logic of the Prime Model."""
+"""Module containing the managing logic of the Prime model."""
 from typing import Iterable, List
 
 # isort: split
 from ansys.meshing.prime.autogen.model import Model as _Model
 
 # isort: split
 import ansys.meshing.prime.internals.json_utils as json
@@ -15,27 +15,29 @@
 )
 from ansys.meshing.prime.autogen.primeconfig import ErrorCode
 from ansys.meshing.prime.autogen.topodata import TopoData
 from ansys.meshing.prime.core.controldata import ControlData
 from ansys.meshing.prime.core.part import Part
 from ansys.meshing.prime.internals.communicator import Communicator
 from ansys.meshing.prime.internals.error_handling import PrimeRuntimeError
+from ansys.meshing.prime.internals.logger import LOG
 
 
 class Model(_Model):
-    """Model is the nucleus of Prime.
+    """Contains all information about Ansys Prime Server.
 
-    Model forms the base and contains all the information about Prime.
-    You can access any information in Prime only through Model.
-    Model allows you to query TopoData, ControlData, Parts, SizeFields and more.
+    This class provides the nucleus of Ansys meshing technology. You can access
+    any information in Ansys Prime Server only through the ``Model`` class.
+    Using this class, you can query topo data, control data, parts, size fields,
+    and more.
 
     Parameters
     ----------
     comm : Communicator
-        Communicator to connect with the server.
+        Communicator to connect with the Ansys Prime server.
     id : int
         ID of the model.
     object_id : int
         Object ID of the model.
     name : str
         Name of the model.
     """
@@ -50,17 +52,18 @@
         self._default_part = None
         self._topo_data = None
         self._control_data = None
         self._material_point_data = None
         self._freeze()
 
     def _sync_up_model(self):
-        """Synchronize client model with the server model.
+        """Synchronize the client model with the server model.
 
-        Updates proxy child objects of the client model with the child objects of the server model.
+        This method Updates proxy child objects of the client model with the
+        child objects of the server model.
 
         Examples
         --------
         >>> from ansys.meshing.prime import Model
         >>> model = client.model
         >>> model._sync_up_model()
         """
@@ -87,20 +90,20 @@
         self._control_data._update_volume_controls(vc_data)
         self._topo_data = TopoData(self, -1, res["TopoData"], "")
         if "PeriodicControl" in res:
             self._control_data._update_periodic_controls(percon_data)
         self._material_point_data = MaterialPointManager(self, -1, res["MaterialPointData"], "")
 
     def _add_part(self, id: int):
-        """Add a part that is present on server.
+        """Add a part that is present on the server.
 
         Parameters
         ----------
         id : int
-            ID of the part
+            ID of the part.
 
         Raises
         ------
         PrimeRuntimeError
             Raise if unable to create the part.
         """
         res = json.loads(
@@ -113,75 +116,75 @@
                 new_part = Part(self, part[0], part[1], part[2])
                 self._parts.append(new_part)
                 break
         if new_part == None:
             raise PrimeRuntimeError("Unable to create part", ErrorCode.PARTNOTFOUND)
 
     def get_part_by_name(self, name: str) -> Part:
-        """Get the part by name. Returns None if part doesn't exist for the given name.
+        """Get the part by name.
 
         Parameters
         ----------
         name : str
             Name of the part.
 
         Returns
         -------
         Part
-            Returns the part.
+            Part or ``None`` if the given part name doesn't exist.
 
         Examples
         --------
             >>> from ansys.meshing.prime import Model
             >>> model = client.model
             >>> part = model.get_part_by_name("part.1")
         """
         for part in self._parts:
             if part.name == name:
                 return part
         return None
 
     def get_part(self, id: int) -> Part:
-        """Get the part by id. Returns None if part doesn't exist for the given id.
+        """Get the part by ID.
 
         Parameters
         ----------
         id : int
-            Id of the part.
+            ID of the part.
 
         Returns
         -------
         Part
-            Return the part.
+            Part or ``None`` if the given part ID doesn't exist.
 
         Examples
         --------
             >>> from ansys.meshing.prime import Model
             >>> model = client.model
             >>> part = model.get_part(2)
         """
         for part in self._parts:
             if part.id == id:
                 return part
         return None
 
     def merge_parts(self, part_ids: Iterable[int], params: MergePartsParams) -> MergePartsResults:
-        """Merge given parts into one.
+        """Merge multiple parts into a single part.
 
         Parameters
         ----------
         part_ids : Iterable[int]
-            Ids of parts to be merged.
+            IDs of the parts to merge.
         params : MergePartsParams
-            Parameters to merge parts.
+            Parameters for merging parts.
 
         Returns
         -------
         MergePartsResults
-            Return the MergePartsResults.
+            Results for merging the parts into a single part.
 
 
         Examples
         --------
         >>> params = prime.MergePartsParams(model = model)
         >>> results = model.merge_parts(part_ids, params)
 
@@ -194,25 +197,25 @@
             for id in part_ids:
                 part = self.get_part(id)
                 if part.id != merged_part.id:
                     self._parts.remove(part)
         return res
 
     def delete_parts(self, part_ids: Iterable[int]) -> DeleteResults:
-        """Delete the parts and its contents.
+        """Delete parts and their contents.
 
         Parameters
         ----------
         part_ids : Iterable[int]
-            Ids of parts to be deleted.
+            IDs of parts to delete.
 
         Returns
         -------
         DeleteResults
-            Return DeleteResults.
+            Results from deleting parts and their contents.
 
 
         Examples
         --------
         >>> results = model.delete_parts(part_ids)
 
         """
@@ -221,38 +224,36 @@
             for id in part_ids:
                 for part in list(self._parts):
                     if part.id == id:
                         self._parts.remove(part)
         return res
 
     def get_global_sizing_params(self) -> GlobalSizingParams:
-        """Get the GlobalSizingParams.
+        """Get global sizing parameters.
 
         Returns
         -------
         GlobalSizingParams
-            Return the GlobalSizingParams.
+            Global sizing parameters.
 
         Examples
         --------
             >>> model = client.model
             >>> sf_params = model.get_global_sizing_params()
         """
         return self._global_sf_params
 
     def set_global_sizing_params(self, params: GlobalSizingParams):
-        """Set the global sizing parameters.
-
-        Set the global sizing params to initialize surfer parameters and various size control
-        parameters.
+        """Set global sizing parameters.
 
         Parameters
         ----------
         params : GlobalSizingParams
-             Global sizing parameters.
+            Global sizing parameters for initializing surfer parameters and
+            various size control parameters.
 
         Examples
         --------
         >>> model = client.model
         >>> model.set_global_sizing_params(GlobalSizingParams(model=model,
         ...                                          min=0.1,
         ...                                          max=1.0,
@@ -263,15 +264,15 @@
 
     def __str__(self):
         """Print the summary of the model.
 
         Returns
         -------
         str
-            Return the summary of the model.
+            Summary of the model.
 
         Examples
         --------
         >>> from ansys.meshing.prime import Model
         >>> model = client.model
         >>> print(model)
         """
@@ -279,93 +280,93 @@
         result += "Part Summary:\n"
         for part in self._parts:
             result += part.__str__() + "\n"
         return result
 
     @property
     def parts(self) -> List[Part]:
-        """Get the list of parts of a model.
+        """Get the list of parts for the model.
 
         Returns
         -------
         List[Part]
-            Return the list of parts.
+            List of parts for the model.
 
         Examples
         --------
             >>> from ansys.meshing.prime import Model
             >>> model = client.model
             >>> parts = model.parts
         """
         return self._parts
 
     @property
     def topo_data(self) -> TopoData:
-        """Gets the topodata of a model.
+        """Get the TopoData for the model.
 
         Returns
         -------
         TopoData
-            Returns the topodata.
+            TopoData for the model.
 
         Examples
         --------
             >>> topo_data=model.topo_data
         """
         return self._topo_data
 
     @property
     def control_data(self) -> ControlData:
-        """Get the control data of a model.
+        """Get the control data for the model.
 
         Returns
         -------
         ControlData
-            Return the control data.
+            Control data for the model.
 
         Examples
         --------
             >>> control_data = model.control_data
         """
         if self._control_data is None:
             self._sync_up_model()
         return self._control_data
 
     @property
     def material_point_data(self) -> MaterialPointManager:
-        """Get Material Point Data.
+        """Get material point data for the model.
 
-        MaterialPointManager is used to create, delete and manage material points.
+        The Material Point Manager is used to create, delete, and manage material points.
 
         Returns
         -------
         MaterialPointManager
-            Return the material point manager.
+            Material Point Manager.
 
         Examples
         --------
             >>> mpt_data = model.material_point_data
         """
         if self._material_point_data is None:
             self._sync_up_model()
         return self._material_point_data
 
     @property
     def python_logger(self):
-        """Get PyPrimeMesh's Logger instance.
+        """Get PyPrimeMesh's logger instance.
 
-        PyPrimeMesh's Logger instance can be used to control the verbosity
+        PyPrimeMesh's logger instance can be used to control the verbosity
         of messages printed by PyPrimeMesh.
 
         Returns
         -------
-        Logger
-             Return logging.Logger instance.
+        logging.Logger
+            PyPrimeMesh's logger instance.
 
         Examples
         --------
         Set log level to debug.
 
         >>> model.python_logger.setLevel(logging.DEBUG)
 
         """
-        return self._logger
+        return LOG
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/part.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/part.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Module containing Part class."""
+"""Module containing the ``Part`` class."""
 from typing import Any
 
 # isort: split
 from ansys.meshing.prime.autogen.part import Part as _Part
 
 # isort: split
 from ansys.meshing.prime.autogen.commonstructs import SetNameResults as SetNameResults
@@ -12,50 +12,51 @@
 class Part(_Part):
     """
     Defines and modifies the parts of a model.
 
     Parameters
     ----------
     model: ansys.meshing.prime.Model
-        Model in which part is created
+        Model in which the part is created.
     id: int
-        Id of the part provided by server
+        ID of the part provided by the server.
     object_id: int
-        Object id provided by the server
+        Object ID provided by the server.
     name: str
-        Part name
+        Part name.
     """
 
     __doc__ = _Part.__doc__
 
     def __init__(self, model, id: int, object_id: int, name: str):
         """Initialize Part."""
         self._model = model
         self._print_mesh = False
         self._print_id = False
         _Part.__init__(self, model, id, object_id, name)
 
     def __call__(self, *args: Any, **kwds: Any) -> str:
-        """Callable interface of the Part.
+        """Get a summary of the part.
 
-        Gets summary of the part using supported keyword arguments as given below.
+        This method provides a callable interface of the part for getting a part summary
+        using supported keyword arguments.
 
         Parameters
         ----------
         print_mesh : bool, optional
-            Passing True will get the mesh summary along with part summary.
-            The default is False.
-        peint_id : bool, optional
-            Passing True will get id's of topo entities/zonelets along with part summary.
-            The default is False.
+            Whether to get the mesh summary along with the part summary. The default is
+            ``False``.
+        print_id : bool, optional
+            Whether to get IDs of TopEntities or zonelets along with the part summary.
+            The default is ``False``.
 
         Returns
         -------
         str
-            Returns the summary of part.
+            Summary of the part.
 
         Examples
         --------
         >>> from ansys.meshing.prime import Model
         >>> model = client.model
         >>> part = model.get_part_by_name("Part.1")
         >>> print(part(print_mesh=True, print_id=True))
@@ -71,20 +72,21 @@
                 params.print_id = value
         result = _Part.get_summary(self, params)
         return result.message
 
     def __str__(self) -> str:
         """Print the summary of a part.
 
-        Uses print_mesh and print_id properties to control the the summary of a part.
+        This method uses the ``print_mesh`` and ``print_id`` properties
+        to control the summary of a part.
 
         Returns
         -------
         str
-            Return the summary of a part.
+            Summary of the part.
 
         Examples
         --------
         >>> from ansys.meshing.prime import Model
         >>> model = client.model
         >>> part = model.get_part_by_name("Part.1")
         >>> print(part)
@@ -92,57 +94,53 @@
         params = PartSummaryParams(model=self._model)
         params.print_mesh = self._print_mesh
         params.print_id = self._print_id
         result = _Part.get_summary(self, params)
         return result.message
 
     def set_suggested_name(self, name: str) -> SetNameResults:
-        """Set the unique name for the part based on the given suggested name.
+        """Set the unique name for the part to a suggested name.
 
         Parameters
         ----------
         name : str
             Suggested name for the part.
 
         Returns
         -------
         SetNameResults
-            Return the results with assigned name of the part.
+            Newly suggested name for the part.
 
 
         Examples
         --------
         >>> part.set_suggested_name("part1")
 
         """
         result = _Part.set_suggested_name(self, name)
         self._name = result.assigned_name
         return result
 
     @property
     def print_mesh(self) -> bool:
-        """When True, prints the mesh summary along with part summary. The default is False."""
+        """Whether the mesh summary is set to print along with the part summary."""
         return self._print_mesh
 
     @print_mesh.setter
     def print_mesh(self, value: bool):
         """Print the mesh of the part.
 
         Parameters
         ----------
         value : bool
-            _description_
+            Whether to print the mesh.
         """
         self._print_mesh = value
 
     @property
     def print_id(self) -> bool:
-        """Print the id's of topoentities.
-
-        When True, prints the id's of topoentities or zonelets along with part summary.
-        The default is False.
-        """
+        """Whether IDs of TopoEntities or zonelets are set to print along with the part summary."""
         return self._print_id
 
     @print_id.setter
     def print_id(self, value: bool):
         self._print_id = value
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/periodiccontrol.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/periodiccontrol.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-"""Module containing PeriodicControl related classes and methods."""
+"""Module containing classes and methods related to periodic control."""
 
 from ansys.meshing.prime.autogen.periodiccontrol import (
     PeriodicControl as _PeriodicControl,
 )
 
 # isort: split
 from ansys.meshing.prime.autogen.commonstructs import SetNameResults
 from ansys.meshing.prime.autogen.periodiccontrolstructs import PeriodicControlParams
 
 
 class PeriodicControl(_PeriodicControl):
-    """Periodic control is used to define the scope and transformation for periodic surfaces.
+    """Defines the scope and transformation for periodic surfaces.
 
     Parameters
     ----------
     model : CommunicationManager
-        Server model where to create and modify PeriodicControls from.
+        Server model to create and modify periodic controls from.
     id : int
         ID of the control.
     object_id : int
         Object ID of the control.
     name : str
-        Name of the PeriodicControl
+        Name of the periodic control.
     local : bool, optional
-        Unused, by default False
+        Unused. The default is ``False``.
     """
 
     def __init__(self, model, id, object_id, name, local=False):
-        """Initialize class variables and superclass."""
+        """Initialize class variables and the superclass."""
         _PeriodicControl.__init__(self, model, id, object_id, name)
         self._model = model
         self._name = name
 
     def __str__(self) -> str:
-        """Representation of the class in string format.
+        """Get a representation of the class in string format.
 
         Returns
         -------
         str
             Class data in string format.
         """
         params = PeriodicControlParams(model=self._model)
         result = _PeriodicControl.get_summary(self, params)
         return result.message
 
     def set_suggested_name(self, name: str) -> SetNameResults:
-        """Set the unique name for the periodic control based on the given suggested name.
+        """Set the unique name for the periodic control to a suggested name.
 
         Parameters
         ----------
         name : str
             Suggested name for the periodic control.
 
         Returns
         -------
         SetNameResults
-            Returns a name of the periodic control.
+            Newly suggested name of the periodic control.
 
         Examples
         --------
         >>> periodic_control.set_suggested_name("control1")
 
         """
         result = _PeriodicControl.set_suggested_name(self, name)
@@ -69,15 +69,15 @@
     @property
     def name(self):
         """Get the name of the periodic control.
 
         Returns
         -------
         str
-            Returns the name of the periodic control.
+            Name of the periodic control.
 
         Examples
         --------
         >>> print(periodic_control.name)
 
         """
         return self._name
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/sizecontrol.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/sizecontrol.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,60 +3,60 @@
 
 # isort: split
 from ansys.meshing.prime.autogen.commonstructs import SetNameResults
 from ansys.meshing.prime.autogen.sizecontrolstructs import SizeControlSummaryParams
 
 
 class SizeControl(_SizeControl):
-    """Compute size field for volumetric surface meshing.
+    """Compute the size field for a volumetric surface meshing.
 
     Parameters
     ----------
     model : CommunicationManager
-        Server model where to create and modify SizeControls from.
+        Server model to create and modify size controls from.
     id : int
-        ID of the control.
+        ID of the size control.
     object_id : int
-        Object ID of the control.
+        Object ID of the size control.
     name : str
-        Name of the SizeControl
+        Name of the size control.
     local : bool, optional
-        Unused, by default False
+        Unused. The default is ``False``.
     """
 
     def __init__(self, model, id, object_id, name, local=False):
-        """Initialize class variables and superclass."""
+        """Initialize class variables and the superclass."""
         _SizeControl.__init__(self, model, id, object_id, name)
         self._model = model
         self._name = name
 
     def __str__(self) -> str:
-        """Representation of the class in string format.
+        """Get a representation of the class in string format.
 
         Returns
         -------
         str
             Class data in string format.
         """
         params = SizeControlSummaryParams(model=self._model)
         result = _SizeControl.get_summary(self, params)
         return result.message
 
     def set_suggested_name(self, name: str) -> SetNameResults:
-        """Set the unique name for the size control based on the given suggested name.
+        """Set the unique name for the size control to a suggested name.
 
         Parameters
         ----------
         name : str
             Suggested name for the size control.
 
         Returns
         -------
         SetNameResults
-            Returns a name of the size control.
+            Newly suggested name for the size control.
 
 
         Examples
         --------
         >>> size_control.set_suggested_name("control1")
 
         """
@@ -67,15 +67,15 @@
     @property
     def name(self):
         """Get the name of size control.
 
         Returns
         -------
         str
-            Returns a name of the size control.
+            Name of the size control.
 
         Examples
         --------
         >>> print(size_control.name)
 
         """
         return self._name
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/surfaceutilities.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/surfaceutilities.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,43 +25,43 @@
     CreateContactPatchResults as CreateContactPatchResults,
 )
 from ansys.meshing.prime.core.model import Model
 from ansys.meshing.prime.params.primestructs import ErrorCode as ErrorCode
 
 
 class SurfaceUtilities(_SurfaceUtilities):
-    """Performs various general surface utilities algorithms. For example, add thickness.
+    """Performs various general surface utilities algorithms, such as adding thickness.
 
     Parameters
     ----------
     model : Model
-        Server model in which to perform the operations.
+        Server model in which to perform operations.
     """
 
     def __init__(self, model: Model):
-        """Initialize the superclass and Model variable."""
+        """Initialize the superclass and ``model`` variable."""
         _SurfaceUtilities.__init__(self, model)
         self._model = model
 
     def add_thickness(
         self, zonelets: Iterable[int], params: AddThicknessParams
     ) -> AddThicknessResults:
-        """Thickens the selected list of face zonelet ids.
+        """Add thicknesss to input face zonelets.
 
         Parameters
         ----------
         zonelets : Iterable[int]
-            List of input face zonelet ids.
+            List of input face zonelet IDs.
         params : AddThicknessParams
-            Parameters to control the add thickness operation.
+            Parameters for controlling the addition of thickness.
 
         Returns
         -------
         AddThicknessResults
-            Returns the AddThicknessResults.
+            Results for adding thickness.
 
 
         Examples
         --------
         >>> result = surf_utils.add_thickness(zonelets, params)
 
         """
@@ -69,28 +69,27 @@
         if result.error_code == ErrorCode.NOERROR:
             self._model._sync_up_model()
         return result
 
     def create_boi(
         self, face_zonelet_ids: Iterable[int], params: CreateBOIParams
     ) -> CreateBOIResults:
-        """Creates BOI to the selected list of face zonelet ids.
-
+        """Create BOI to input face zonelets.
 
         Parameters
         ----------
         face_zonelet_ids : Iterable[int]
-            List of input face zonelet ids.
+            List of input face zonelet IDs.
         params : CreateBOIParams
-            Parameters to control the BOI creation operation.
+            Parameters for controlling BOI creation.
 
         Returns
         -------
         CreateBOIResults
-            Returns the BOIResults.
+            Results from creating BOI.
 
 
         Examples
         --------
         >>> result = surf_utils.create_boi(zonelets, params)
 
         """
@@ -101,30 +100,29 @@
 
     def create_contact_patch(
         self,
         source_zonelets: Iterable[int],
         target_zonelets: Iterable[int],
         params: CreateContactPatchParams,
     ) -> CreateContactPatchResults:
-        """Creates contact patch by offsetting the target zonelets.
-
+        """Create a contact patch by offsetting the target zonelets.
 
         Parameters
         ----------
         source_zonelets : Iterable[int]
-            Source face zonelet ids.
+            IDS for the source face zonelets.
         target_zonelets : Iterable[int]
-            Target face zonelet ids.
+            IDs for the target face zonelets.
         params : CreateContactPatchParams
-            Parameters to control the contact patch creation operation.
+            Parameters for controlling the contact patch creation.
 
         Returns
         -------
         CreateContactPatchResults
-            Returns the CreateContactPatchResults.
+            Results from creating the contact patch.
 
 
         Examples
         --------
         >>> result = surf_utils.create_contact_patch(zonelets, params)
 
         """
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/surfer.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/surfer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Module for surfer data."""
 from typing import Iterable
 
 # isort: split
 from ansys.meshing.prime.autogen.surfer import Surfer as _Surfer
 
 # isort: split
 from ansys.meshing.prime.autogen.coreobject import CoreObject
@@ -11,38 +12,46 @@
     SurferParams,
     SurferResults,
 )
 from ansys.meshing.prime.core.model import Model
 
 
 class Surfer(CoreObject):
+    """Provides surfer operations.
+
+    Parameters
+    ----------
+    model : Model
+        Model to operate in.
+    """
+
     __doc__ = _Surfer.__doc__
 
     def __init__(self, model: Model):
-        """__init__(Surfer self, Model model)"""
+        """Initialize a surfer instance."""
         self._model = model
 
     def mesh_topo_faces(
         self, part_id: int, topo_faces: Iterable[int], params: SurferParams
     ) -> SurferResults:
-        """Performs meshing on the given topofaces with provided parameters.
+        """Perform meshing on TopoFaces with given parameters.
 
         Parameters
         ----------
         part_id : int
-            Id of part.
+            ID of part.
         topo_faces : Iterable[int]
-            Ids of topofaces.
+            IDs of the TopoFaces.
         params : SurferParams
-            Surfer Parameters.
+            Surfer parameters.
 
         Returns
         -------
         SurferResults
-            Returns the SurferResults.
+            Results from performing meshing on the TopoFaces.
 
         Examples
         --------
         >>> surfer = prime.Surfer(model)
         >>> surfer_params = prime.SurferParams(model)
         >>> results = surfer.mesh_topo_faces(part_id, topo_faces, surfer_params)
 
@@ -53,31 +62,31 @@
     def remesh_face_zonelets_locally(
         self,
         part_id: int,
         face_zonelets: Iterable[int],
         register_id: int,
         local_surfer_params: LocalSurferParams,
     ) -> LocalSurferResults:
-        """Remesh the given face zonelets locally at the registered faces with provided parameters.
+        """Remesh face zonelets locally at the registered faces with given parameters.
 
         Parameters
         ----------
         part_id : int
-            Id of part.
+            ID of part.
         face_zonelets : Iterable[int]
-            Ids of face zonelets.
+            IDs of the face zonelets.
         register_id : int
-            Register id of the target faces.
+            Register ID of the target faces.
         local_surfer_params : LocalSurferParams
-            Local surfer Parameters.
+            Local surfer parameters.
 
         Returns
         -------
         LocalSurferResults
-            Returns the LocalSurferResults.
+            Results from remeshing the face zonelets.
 
         Examples
         --------
         >>> surfer = prime.Surfer(model)
         >>> local_surfer_params = prime.LocalSurferParams(model)
         >>> results = surfer.remesh_face_zonelets_locally(part_id,
                         face_zonelets, register_id, local_surfer_params)
@@ -91,59 +100,60 @@
     def remesh_face_zonelets(
         self,
         part_id: int,
         face_zonelets: Iterable[int],
         edge_zonelets: Iterable[int],
         params: SurferParams,
     ) -> SurferResults:
-        """Performs meshing on the given face zonelets with provided parameters.
+        """Perform meshing on face zonelets with given parameters.
 
         Parameters
         ----------
         part_id : int
-            Id of part.
+            ID of part.
         face_zonelets : Iterable[int]
-            Ids of face zonelets.
+            IDs of the face zonelets.
         edge_zonelets : Iterable[int]
-            Ids of edge zonelets.
+            IDs of the edge zonelets.
         params : SurferParams
             Surfer parameters.
 
         Returns
         -------
         SurferResults
-            Returns the SurferResults.
+            Results from meshing the face zonelets.
 
         Examples
         --------
         >>> surfer = prime.Surfer(model)
         >>> surfer_params = prime.SurferParams(model)
         >>> results = surfer.remesh_face_zonelets(part_id,
                         face_zonelets, edge_zonelets, surfer_params)
 
         """
         with _Surfer(model=self._model, part_id=part_id) as surfer:
             return surfer.remesh_face_zonelets(face_zonelets, edge_zonelets, params)
 
     def initialize_surfer_params_for_wrapper(self) -> SurferParams:
-        """Initialize surfer parameters to mesh surfaces generated by wrapper.
-
+        """Initialize surfer parameters to mesh surfaces generated by the wrapper.
 
         Returns
         -------
         SurferParams
-            Returns the SurferParams initialized for wrapper inputs.
+            Surfer parameters initialized for wrapper inputs.
 
         Examples
         --------
         >>> surfer = prime.Surfer(model)
         >>> surfer_params = surfer.initialize_surfer_params_for_wrapper()
 
         """
         with _Surfer(model=self._model, part_id=-1) as surfer:
             return surfer.initialize_surfer_params_for_wrapper()
 
     def __enter__(self):
+        """Run initializing context manager."""
         return self
 
     def __exit__(self, type, value, traceback):
+        """Run when closing the context manager."""
         pass
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/volumecontrol.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/volumecontrol.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,80 +3,80 @@
 
 # isort: split
 from ansys.meshing.prime.autogen.commonstructs import SetNameResults
 from ansys.meshing.prime.autogen.volumecontrolstructs import VolumeControlParams
 
 
 class VolumeControl(_VolumeControl):
-    """Volume control is used to define the scope and type of volume mesh to be generated.
+    """Defines the scope and type of volume mesh to generate.
 
     Parameters
     ----------
     model : CommunicationManager
-        Server model where to create and modify VolumeControls from.
+        Server model to create and modify volume controls from.
     id : int
-        ID of the control.
+        ID of the volume control.
     object_id : int
-        Object ID of the control.
+        Object ID of the volume control.
     name : str
-        Name of the VolumeControl
+        Name of the volume control.
     local : bool, optional
-        Unused, by default False
+        Unused. The default is ``False``.
     """
 
     def __init__(self, model, id, object_id, name, local=False):
-        """Initialize the superclass and Model variable."""
+        """Initialize the superclass and the ``model`` variable."""
         _VolumeControl.__init__(self, model, id, object_id, name)
         self._model = model
         self._name = name
 
     def __str__(self) -> str:
-        """Representation of the class in string format.
+        """Get a representation of the class in string format.
 
         Returns
         -------
         str
             Class data in string format.
         """
         params = VolumeControlParams(model=self._model)
         # TODO: function get_summary() not implemented
         result = _VolumeControl.get_summary(self, params)
         return result.message
 
     def set_suggested_name(self, name: str) -> SetNameResults:
-        """Set the unique name for the volume control based on the given suggested name.
+        """Set the unique name for the volume control based on a suggested name.
 
         Parameters
         ----------
         name : str
             Suggested name for the volume control.
 
         Returns
         -------
         SetNameResults
-            Returns a name of the volume control.
+            Newly suggested name of the volume control.
 
 
         Examples
         --------
         >>> volume_control.set_suggested_name("control1")
 
         """
         result = _VolumeControl.set_suggested_name(self, name)
         self._name = result.assigned_name
         return result
 
     @property
     def name(self):
-        """Get the name of volume control.
+        """Get the name of the volume control.
 
         Returns
         -------
         str
-            Returns a name of volume control.
+            Name of the volume control.
 
         Examples
         --------
         >>> print(volume_control.name)
 
         """
         return self._name
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/volumesweeper.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/volumesweeper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,61 @@
+"""Module for volume sweeper operations."""
 from ansys.meshing.prime.autogen.volumesweeper import VolumeSweeper as _Sweeper
 
 # isort: split
 from typing import Iterable
 
 from ansys.meshing.prime.autogen.volumesweeperstructs import (
     MeshStackerParams,
     MeshStackerResults,
 )
 from ansys.meshing.prime.core.model import Model
 
 
 class VolumeSweeper(_Sweeper):
+    """Provides operations to generate volume meshes using stacker technology.
 
-    """VolumeSweeper class provide functions to volume mesh a given set of topovolumes by sweeping
-    or stacking a set of face and edge zonelets.
-    Provide operations to generate volume mesh using stacker technology."""
+    TopoVolumes are volume meshed by sweeping or stacking a set of face
+    and edge zonelets.
+
+    Parameters
+    ----------
+    model : Model
+        Model to apply the operations to.
+    """
 
     __doc__ = _Sweeper.__doc__
 
     def __init__(self, model: Model):
-        """__init__(Sweeper self, Model model)"""
+        """Initialize the model in the volume sweeper."""
         self._model = model
 
     def create_base_face(
         self, part_id: int, topo_volume_ids: Iterable[int], params: MeshStackerParams
     ) -> MeshStackerResults:
-        """Creates a face at the specified origin and perpendicular to the specified direction.
-        Also, imprint model edges on the face, make necessary edge repairs, and duplicate relevant
-        size controls on the base face.
+        """Create a face at the specified origin.
+
+        This method creates a face at the specified origin and perpendicular to the
+        specified direction. Also, it imprints model edges on the face, makes necessary
+        edge repairs, and duplicates relevant size controls on the base face.
 
 
         Parameters
         ----------
         part_id : int
-            Id of part.
+            ID of part.
         topo_volume_ids : Iterable[int]
-            Ids of volumes that need to be meshed.
+            IDs of the volumes to mesh.
         params : MeshStackerParams
             Mesh stacker parameters.
 
         Returns
         -------
         MeshStackerResults
-            Returns the MeshStackerResults.
+            Results from creating the face.
 
 
         Examples
         --------
         >>> results = volumesweeper.create_base_face(part_id, topo_volume_ids, params)
 
         """
@@ -56,33 +65,36 @@
     def stack_base_face(
         self,
         part_id: int,
         base_face_ids: Iterable[int],
         topo_volume_ids: Iterable[int],
         params: MeshStackerParams,
     ) -> MeshStackerResults:
-        """Generate volume mesh stacking a meshed face, layer by layer, along the given
-        direction. Calculates the stack layers using size controls and global size parameters.
+        """Generate volume mesh by stacking a meshed face.
+
+        This method generates volume mesh by stacking a meshed face, layer by layer, along
+        the given direction. It calculates the stack layers using size controls and global
+        size parameters.
 
 
         Parameters
         ----------
         part_id : int
-            Id of part.
+            ID of the part.
         base_face_ids: Iterable[int]
-            Ids of base faces to be stacked.
+            IDs of the base faces to stack.
         topo_volume_ids : Iterable[int]
-            Ids of volumes that need to be meshed.
+            IDs of the volumes to mesh.
         params : MeshStackerParams
             Mesh stacker parameters.
 
         Returns
         -------
         MeshStackerResults
-            Returns the MeshStackerResults.
+            Results from generating the volume mesh.
 
 
         Examples
         --------
         >>> results = volumesweeper.stack_base_face(part_id, base_face_ids, topo_volume_ids, params)
 
         """
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/wrapper.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/wrapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Module for the wrapper class."""
 from typing import List
 
 import numpy as np
 
 # isort: split
 from ansys.meshing.prime.autogen.wrapper import Wrapper as _Wrapper
 
@@ -23,37 +24,45 @@
 from ansys.meshing.prime.autogen.wrapperstructs import WrapResult as WrapResult
 from ansys.meshing.prime.core.model import Model
 from ansys.meshing.prime.core.part import Part
 from ansys.meshing.prime.params.primestructs import ErrorCode as ErrorCode
 
 
 class Wrapper(_Wrapper):
-    """Provides operations to generate surface mesh using wrapper technology."""
+    """Provides operations for generating a surface mesh using wrapper technology.
+
+    Parameters
+    ----------
+    model : Model
+        Model to apply wrapping to.
+    """
 
     def __init__(self, model: Model):
-        """__init__(Model self, int id, int object_id, char* name)"""
+        """Initialize the wrapper and model."""
         _Wrapper.__init__(self, model)
         self._model = model
 
     def wrap(self, wrapper_control_id: int, params: WrapParams) -> WrapResult:
-        """Performs wrapping with specified controls in wrapper control and with provided
-            parameters.
+        """Perform wrapping with specified controls and given parameters.
+
+        This method performs wrapping with specified controls in the wrapper control
+        and with given parameters.
 
 
         Parameters
         ----------
         wrapper_control_id : int
-            Id of wrapper control.
+            ID of the wrapper control.
         params : WrapParams
-            Wrap Parameters.
+            Wrap parameters.
 
         Returns
         -------
         WrapResult
-            Returns the Wrap Results.
+            Wrap results.
 
 
         Examples
         --------
         >>> results = wrapper.wrap(wrapper_control_id, params)
 
         """
@@ -65,28 +74,30 @@
     def connect(
         self,
         wrapper_part: Part,
         target_labels: List[str],
         source_parts: List[Part],
         source_labels: List[str],
     ):
-        """Performs label controlled connection of wrapper part face zonelets to face zonelets of
-            source parts.
+        """Perform a label-controlled connection.
+
+        This method performs a label-controlled connection of wrapper part face zonelets to
+        face zonelets of source parts.
 
 
         Parameters
         ----------
         wrapper_part : Part
-            wrapper part.
+            Wrapper part.
         target_labels : List[str]
-            target zonelet labels to be connected.
+            List of target zonelet labels to connect.
         source_parts : List[Part]
-           source parts to be connected with.
+           List of source parts to connect with.
         source_labels : List[Part]
-           source zonelet labels to be connected.
+           List of source zonelet labels to connect.
 
 
         Examples
         --------
         >>> wrapper.connect(wrapper_part, target_labels, source_parts, source_labels)
 
         """
@@ -136,29 +147,31 @@
         surf_utils.resolve_intersections(
             face_zonelet_ids=modified_zonelets, params=ResolveIntersectionsParams(model=self._model)
         )
 
     def close_gaps(
         self, scope: ScopeDefinition, params: WrapperCloseGapsParams
     ) -> WrapperCloseGapsResult:
-        """Close gaps create patching surfaces within the face zonelets specified
-            by scope using gap size.
+        """Close gaps.
+
+        Closing gaps creates patching surfaces within the face zonelets specified
+        by scope using gap size.
 
 
         Parameters
         ----------
         scope : ScopeDefinition
-            Scope definition of face zonelets.
+            Scope definition of the face zonelets.
         params : WrapperCloseGapsParams
-            Wrapper close gaps parameters.
+            Wrapper providing close gap parameters.
 
         Returns
         -------
         WrapperCloseGapsResult
-            Returns the WrapperCloseGapsResult.
+            Results from the wrapper for closing gaps.
 
 
         Examples
         --------
         >>> result = wrapper.close_gaps(scope, params)
 
         """
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/core/wrappercontrol.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/wrappercontrol.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,74 +3,74 @@
 
 # isort: split
 from ansys.meshing.prime.autogen.commonstructs import SetNameResults as SetNameResults
 from ansys.meshing.prime.internals.comm_manager import CommunicationManager
 
 
 class WrapperControl(_WrapperControl):
-    """Wrapper Control to describe all parameters and controls used for wrapping.
+    """Provides all parameters and controls used for wrapping.
 
     Parameters
     ----------
     model : CommunicationManager
-        Server model where to create and modify WrapperControls from.
+        Server model to create and modify wrapper controls from.
     id : int
-        ID of the control.
+        ID of the wrapper control.
     object_id : int
-        Object ID of the control.
+        Object ID of the wrapper control.
     name : str
-        Name of the WrapperControl
+        Name of the wrapper control
     """
 
     def __init__(self, model: CommunicationManager, id: int, object_id: int, name: str):
-        """Initialize the superclass and Model variable."""
+        """Initialize the superclass and the ''Model'' variable."""
         self._model = model
         _WrapperControl.__init__(self, model, id, object_id, name)
 
     def __str__(self) -> str:
-        """Representation of the class in string format.
+        """Get a representation of the class in string format.
 
         Returns
         -------
         str
             Class data in string format.
         """
         return "Not implemented yet"
 
     def set_suggested_name(self, name: str) -> SetNameResults:
-        """Set the unique name for the wrapper control based on the given suggested name.
+        """Set the unique name for the wrapper control based on a suggested name.
 
         Parameters
         ----------
         name : str
             Suggested name for the wrapper control.
 
         Returns
         -------
         SetNameResults
-            Returns the results with assigned name of the wrapper control.
+            Newly assigned name of the wrapper control.
 
 
         Examples
         --------
         >>> wrapper_control.set_suggested_name("wrapper_control1")
 
         """
         result = _WrapperControl.set_suggested_name(self, name)
         self._name = result.assigned_name
         return result
 
     @property
     def name(self):
-        """Get the name of wrapper control.
+        """Get the name of the wrapper control.
 
         Returns
         -------
         str
-            Returns a name of the wrapper control.
+            Name of the wrapper control.
 
         Examples
         --------
         >>> print(wrapper_control.name)
 
         """
         return self._name
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/examples/__init__.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/examples/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,18 +7,22 @@
     download_deformed_blade_fmd,
     download_deformed_blade_scdoc,
     download_elbow_dsco,
     download_elbow_fmd,
     download_elbow_pmdat,
     download_elbow_scdoc,
     download_pcb_pmdat,
+    download_pcb_scdoc,
     download_pipe_tee_dsco,
     download_pipe_tee_fmd,
     download_pipe_tee_pmdat,
     download_pipe_tee_scdoc,
+    download_saddle_bracket_dsco,
+    download_saddle_bracket_fmd,
+    download_saddle_bracket_scdoc,
     download_toy_car_dsco,
     download_toy_car_fmd,
     download_toy_car_pmdat,
     download_toy_car_scdoc,
     download_turbine_blade_cdb,
 )
 from .unit_test_examples import download_test_examples
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/examples/download_utilities.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/examples/download_utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,80 +7,88 @@
 import ansys.meshing.prime.internals.defaults as defaults
 
 __all__ = ['DownloadManager']
 
 
 class DownloadManagerMeta(type):
     """
-    This is a thread-safe implementation of Singleton, from
-    https://refactoring.guru/design-patterns/singleton/python/example#example-1
+    Provides a thread-safe implementation of ``Singleton`` from
+    https://refactoring.guru/design-patterns/singleton/python/example#example-1.
     """
 
     _instances = {}
     _lock: Lock = Lock()
 
     def __call__(cls, *args, **kwargs):
         """
-        Possible changes to the value of the `__init__` argument do not affect
+        Possible changes to the value of the ``__init__`` argument do not affect
         the returned instance.
         """
         with cls._lock:
             if cls not in cls._instances:
                 instance = super().__call__(*args, **kwargs)
                 cls._instances[cls] = instance
         return cls._instances[cls]
 
 
 class DownloadManager(metaclass=DownloadManagerMeta):
-    """Singleton class to manage the file downloads of the module.
-    Local paths are saved in this class so we can do a global cleanup when
-    closing the client.
+    """Manages downloads of example files.
+
+    Local paths are saved in this class so that a global cleanup
+    of example files can be performed when the client is closed.
     """
 
     def __init__(self):
         self.downloads_list = []
 
     def add_file(self, file_path: str):
-        """Adds downloaded file path to a list to keep track of where the downloaded
-        files are. This will be used for cleaning up the downloads.
+        """Add the path for a downloaded example file to a list.
+
+        This list keeps track of where example files are
+        downloaded so that a global cleanup of these files can be
+        performed when the client is closed.
 
         Parameters
         ----------
         file_path : str
-            Local path of the downloaded file.
+            Local path of the downloaded example file.
         """
         self.downloads_list.append(file_path)
 
     def clear_download_cache(self):
-        """Removes the downloaded files from the local."""
+        """Remove downloaded example files from the local path."""
         for file in self.downloads_list:
             os.remove(file)
         self.downloads_list.clear()
 
     def download_file(
         self, filename: str, *directory: str, destination: Optional[str] = None, force: bool = False
     ) -> str:
-        """Download a file from PyAnsys examples Github repo
+        """Download an example file from the PyPrimeMesh repository.
 
         Parameters
         ----------
-        filename: str
-            Name of the file to download
-        destination: Optional[str]
-            Optional destination to download the directory to
-        force: bool
-            Flag to force download even if the file exists in cache
-        directory: tuple[str]
-            Path under the PyAnsys Github examples repo
+        filename : str
+            Name of the example file to download.
+        destination : str, optional
+            Path to download the example file to. The default
+            is ``None``, in which case the default path for app data
+            is used.
+        force : bool, optional
+            Whether to always download the example file. The default is
+            ``False``, in which case if the example file is cached, it
+            is reused.
+        directory : tuple[str]
+            Path under the PyAnsys Github examples repository.
 
         Returns
         -------
-        Tuple[str, str]
-            Tuple containing filepath to be used and the local filepath of the downloaded directory
-            The two are different in case of containers.
+        tuple[str, str]
+            Tuple containing the filepath to use and the local filepath of the downloaded
+            directory. The two are different in case of containers.
 
         """
         # if destination is not a dir create it
         if destination is not None and not os.path.isdir(destination):
             os.mkdir(destination)
 
         # check if it was able to create the dir
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/examples/unit_test_examples.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/examples/unit_test_examples.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,29 +15,31 @@
     "hex.msh",
 ]
 
 
 def download_test_examples(
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
-    """Download files necessary for unit testing.
+    """Download the example files necessary for unit testing.
 
     Parameters
     ----------
-    destination: Optional[str]
-        Destination for the file to be downloaded.
-        If nothing is provided, the default path in app data is used
-    force: bool
-        If true, the file is always downloaded.
-        If false, an existing file in the cache may be re-used.
+    destination : str, optional
+        Path to download the test example files to. The default
+        is ``None``, in which case the default path for app data
+        is used.
+    force : bool, optional
+        Whether to always download the test example files. The default is
+        ``False``, in which case if the test example files are cached, they
+        are reused.
 
     Returns
     -------
     List[str]
-        Local paths to the downloaded files
+        Local paths to the downloaded test example files.
 
     Examples
     --------
     >>> import ansys.meshing.prime as prime
     >>> import ansys.meshing.prime.examples as prime_examples
     >>> with prime.launch_prime() as session:
     >>>     model = session.model
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/graphics.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/graphics.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,36 @@
+"""Module for graphics-related implementations."""
 import enum
 import os
+from typing import List
 
 import numpy as np
 import pyvista as pv
 import vtk
 from pyvista.plotting.plotting import Plotter
 
 import ansys.meshing.prime as prime
 from ansys.meshing.prime.graphics.trame_gui import _HAS_TRAME, TrameVisualizer
 from ansys.meshing.prime.internals import defaults
 
 
-def compute_face_list_from_structured_nodes(nodes, dim):
+# TODO: nodes parameter is unused.
+def compute_face_list_from_structured_nodes(dim):
+    """Compute the distances from the nodes.
+
+    Parameters
+    ----------
+    dim : List[int]
+        List with the number of elements in each dimension.
+
+    Returns
+    -------
+    List
+        List with the faces.
+    """
     flist = []
     for w in range(dim[2]):
         for u in range(dim[0] - 1):
             for v in range(dim[1] - 1):
                 flist.append(4)
                 flist.append(u + v * dim[0] + w * dim[0] * dim[1])
                 flist.append(u + 1 + v * dim[0] + w * dim[0] * dim[1])
@@ -39,23 +54,27 @@
                 flist.append(u + (v + 1) * dim[0] + w * dim[0] * dim[1])
                 flist.append(u + (v + 1) * dim[0] + (w + 1) * dim[0] * dim[1])
                 flist.append(u + v * dim[0] + (w + 1) * dim[0] * dim[1])
     return flist
 
 
 class DisplayMeshType(enum.IntEnum):
+    """Contains the mesh types to display."""
+
     TOPOFACE = 0
     TOPOEDGE = 1
     FACEZONELET = 2
     EDGEZONELET = 3
     SPLINECONTROLPOINTS = 4
     SPLINESURFACE = 5
 
 
 class ColorByType(enum.IntEnum):
+    """Contains the zone types to display."""
+
     ZONE = 0
     ZONELET = 1
     PART = 2
 
 
 ''' bright color palette '''
 '''color_matrix = np.array([
@@ -109,40 +128,60 @@
         [215, 208, 198],
         [196, 235, 145],
     ]
 )
 
 
 def compute_distance(point1, point2):
+    """Compute the distance between two points."""
     dist = np.linalg.norm(np.array(point2) - np.array(point1))
     return dist
 
 
 class Picker:
-    def __init__(self, plotter, graphics):
+    """Contains the items that can be selected from the display with the mouse.
+
+    Parameters
+    ----------
+    plotter : Plotter
+        PyVista plotter to manipulate.
+    graphics : Graphics
+        Class for providing callbacks.
+    """
+
+    def __init__(self, plotter: pv.Plotter, graphics):
+        """Initialize the picker."""
         self.plotter = plotter
         self._graphics = graphics
         self._selected_disp_mesh: list[_DisplayMesh] = []
         self._points = []
         self._ignore = False
 
     @property
     def selections(self):
-        """To access all the selected disp mesh when done."""
+        """All selected meshes in the display."""
         return self._selected_disp_mesh
 
     def clear_selection(self):
-        """ """
+        """Clear all picked selections in the display."""
         [disp_mesh.deselect() for disp_mesh in self._selected_disp_mesh]
         self._selected_disp_mesh.clear()
 
     def ignore(self, ignore_pick):
+        """Setter for ignore_pick.
+
+        Parameters
+        ----------
+        ignore_pick : Any
+            Picked selection to ignore.
+        """
         self._ignore = ignore_pick
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args, **kwargs):  # pragma: no cover
+        """Call the code to run when something is clicked in the display."""
         if self._ignore:
             return
         picked_pt = np.array(self.plotter.pick_mouse_position())
         direction = picked_pt - self.plotter.camera_position[0]
         direction = direction / np.linalg.norm(direction)
         start = picked_pt - 1000 * direction
         end = picked_pt + 10000 * direction
@@ -164,18 +203,26 @@
         if closest_disp_mesh is not None:
             self._selected_disp_mesh.append(closest_disp_mesh)
         [disp_mesh.select() for disp_mesh in self._selected_disp_mesh]
         return
 
 
 class Graphics(object):
-    """ """
+    """Manages graphics in PyPrime.
+
+    Parameters
+    ----------
+    model : prime.Model
+        Model to show.
+    use_trame : bool, optional
+        Whether to use the Trame visualizer. The default is ``False``.
+    """
 
     def __init__(self, model: prime.Model, use_trame: bool = False):
-        """ """
+        """Initialize graphics."""
         self._model = model
         self._display_data = {}
         self._display_spline_data = {}
         self._plotter = None
         self._picker = None
         self._color_by_type = ColorByType.ZONE
         self._parts = None
@@ -187,27 +234,27 @@
         self._hideBt: vtk.vtkButtonWidget = None
         self._showEdgeBt: vtk.vtkButtonWidget = None
         self._printInfoBt: vtk.vtkButtonWidget = None
         self._showRulerBt: vtk.vtkButtonWidget = None
         self._sphinx_build = defaults.get_sphinx_build()
         self._use_trame = use_trame
 
-        if self._use_trame and not _HAS_TRAME:
+        if self._use_trame and not _HAS_TRAME:  # pragma: no cover
             warn_msg = (
                 "'use_trame' is active but Trame dependencies are not installed."
                 "Consider installing 'pyvista[trame]' to use this functionality."
             )
             self._model._logger.warning(warn_msg)
-        if os.getenv('PRIME_APP_RUN'):
+        if os.getenv('PRIME_APP_RUN'):  # pragma: no cover
             self._app = __import__('PrimeApp')
         else:
             self.__update_display_data()
 
     def __update_display_data(self):
-        """ """
+        """Update the objects displayed in the visualizer."""
         part_ids = [part.id for part in self._model.parts]
         mesh_info = prime.MeshInfo(self._model)
         self._display_data.clear()
         with prime.numpy_array_optimization_enabled():
             self._facet_result = mesh_info.get_face_and_edge_connectivity(
                 part_ids, prime.FaceAndEdgeConnectivityParams(model=self._model)
             )
@@ -238,19 +285,33 @@
             if len(disp_ctrl_point_data) > 0:
                 data["ctrlpts"] = disp_ctrl_point_data
             if len(disp_spline_surf_data) > 0:
                 data["splinesurf"] = disp_spline_surf_data
             self._display_data[part_id] = data
 
     def __get_ctrl_point_display_mesh_object(self, part_id, spline_id):
+        """Calculate the control points in a display.
+
+        Parameters
+        ----------
+        part_id : int
+            ID of the part to show the edges on.
+        spline_id : prime.EdgeConnectivityResults
+            Results of the face connectivity.
+
+        Returns
+        -------
+        _DisplayMesh
+            Displayed mesh.
+        """
         part = self._model.get_part(part_id)
         spline = part.get_spline(spline_id)
         dim = spline.control_points_count
         nodes = spline.control_points
-        face_list = compute_face_list_from_structured_nodes(nodes, dim)
+        face_list = compute_face_list_from_structured_nodes(dim)
         display_mesh_type = DisplayMeshType.SPLINECONTROLPOINTS
         id = spline.id
         disp_mesh = _DisplayMesh(
             display_mesh_type,
             id,
             part_id,
             self,
@@ -261,19 +322,33 @@
             zone_id=-1,
             zone_name="",
             part_name=part.name,
         )
         return disp_mesh
 
     def __get_spline_surf_display_mesh_object(self, part_id, spline_id):
+        """Calculate the splines in a display.
+
+        Parameters
+        ----------
+        part_id : int
+            ID of the part to show the edges on.
+        spline_id : prime.EdgeConnectivityResults
+            Results of the face connectivity.
+
+        Returns
+        -------
+        _DisplayMesh
+            Displayed mesh.
+        """
         part = self._model.get_part(part_id)
         spline = part.get_spline(spline_id)
         dim = spline.spline_points_count
         nodes = spline.spline_points
-        face_list = compute_face_list_from_structured_nodes(nodes, dim)
+        face_list = compute_face_list_from_structured_nodes(dim)
         display_mesh_type = DisplayMeshType.SPLINESURFACE
         id = spline.id
         disp_mesh = _DisplayMesh(
             display_mesh_type,
             id,
             part_id,
             self,
@@ -286,15 +361,30 @@
             part_name=part.name,
         )
         return disp_mesh
 
     def __get_face_display_mesh_object(
         self, part_id: int, face_facet_res: prime.FaceConnectivityResults, index: int
     ):
-        """ """
+        """Display the faces in an object.
+
+        Parameters
+        ----------
+        part_id : int
+            ID of the part to show the edges on.
+        face_facet_res : prime.EdgeConnectivityResults
+            Results of the face connectivity.
+        index : int
+            Index of the TopoEdges list.
+
+        Returns
+        -------
+        _DisplayMesh
+            Displayed mesh.
+        """
         part = self._model.get_part(part_id)
         node_start = 3 * np.sum(face_facet_res.num_nodes_per_face_zonelet[0:index])
         num_node_coords = 3 * face_facet_res.num_nodes_per_face_zonelet[index]
         face_list_start = np.sum(face_facet_res.num_face_list_per_face_zonelet[0:index])
         num_face_list = face_facet_res.num_face_list_per_face_zonelet[index]
         has_mesh = True
         if face_facet_res.topo_face_ids[index] > 0:
@@ -318,15 +408,30 @@
             part_name=part.name,
         )
         return disp_mesh
 
     def __get_edge_display_mesh_object(
         self, part_id: int, edge_facet_res: prime.EdgeConnectivityResults, index: int
     ):
-        """ """
+        """Display the edges in an object.
+
+        Parameters
+        ----------
+        part_id : int
+            ID of the part with the edges to display.
+        edge_facet_res : prime.EdgeConnectivityResults
+            Results of the edge connectivity.
+        index : int
+            Index of the TopoEdges list.
+
+        Returns
+        -------
+        _DisplayMesh
+            displayed mesh.
+        """
         part = self._model.get_part(part_id)
         node_start = 3 * np.sum(edge_facet_res.num_nodes_per_edge_zonelet[0:index])
         num_node_coords = 3 * edge_facet_res.num_nodes_per_edge_zonelet[index]
         edge_list_start = np.sum(edge_facet_res.num_edge_list_per_edge_zonelet[0:index])
         num_edge_list = edge_facet_res.num_edge_list_per_edge_zonelet[index]
         has_mesh = True
         if edge_facet_res.topo_edge_ids[index] > 0:
@@ -347,29 +452,44 @@
             has_mesh,
             part_name=part.name,
             topo_edge_type=edge_facet_res.topo_edge_types[index],
             number_of_edges=edge_facet_res.num_edges_per_edge_zonelet[index],
         )
         return disp_mesh
 
-    def __call__(self, parts=None, update=True, spline=False, scope: prime.ScopeDefinition = None):
-        """ """
+    def __call__(
+        self,
+        parts: List = None,
+        update: bool = True,
+        spline: bool = False,
+        scope: prime.ScopeDefinition = None,
+    ):
+        """Show the appropriate display based on parameters.
+
+        Parameters
+        ----------
+        parts : Any, optional
+            Parts to show. The default is ``None``.
+        update : bool, optional
+            Whether to update the display. The default is ``True``.
+        spline : bool, optional
+            Whether to use splines. The default is ``False``.
+        scope : prime.ScopeDefinition, optional
+            Scope of the parts. The default is ``None``.
+        """
         self._parts = parts
-        # if(spline):
-        #     self.__draw_spline(update)
-        # el
         if scope != None:
             self.__draw_scope_parts(update, scope)
         elif parts != None:
             self.__draw_parts(parts, update, spline)
         else:
             self.show(update)
 
-    def __color_by_type_callback(self, flag):
-        """ """
+    def __color_by_type_callback(self):  # pragma: no cover
+        """Determine the color of a type in the callback."""
         vr = self._colorByTypeBt.GetRepresentation()
         state = vr.GetState()
         self._color_by_type = ColorByType(state)
         r = vtk.vtkPNGReader()
         color_by_type_icon_file = ""
         if self._color_by_type == ColorByType.ZONELET:
             color_by_type_icon_file = os.path.join(
@@ -386,42 +506,42 @@
         [
             disp_mesh.set_color_by_type(self._color_by_type)
             for part_id, data in self._display_data.items()
             if data.get("faces") != None
             for disp_mesh in data["faces"]
         ]
 
-    def __hide_unhide_selection(self, flag):
-        """ """
+    def __hide_unhide_selection(self):  # pragma: no cover
+        """Hide or unhide the clicked component."""
         sel_disp_mesh = self._picker.selections
         if len(sel_disp_mesh) > 0:
             [disp_mesh.hide(self._plotter) for disp_mesh in sel_disp_mesh]
             self._picker.clear_selection()
         else:
             [
                 disp_mesh.unhide(self._plotter)
                 for part_id, data in self._display_data.items()
                 if data.get("faces") != None
                 for disp_mesh in data["faces"]
             ]
 
-    def __show_edges_callback(self, flag):
+    def __show_edges_callback(self, flag):  # pragma: no cover
         [
             disp_mesh.show_edges(flag)
             for part_id, data in self._display_data.items()
             if data.get("faces") != None
             for disp_mesh in data["faces"]
         ]
 
-    def __print_callback(self, flag):
+    def __print_callback(self, flag):  # pragma: no cover
         sel_disp_mesh = self._picker.selections
         [print(disp_mesh) for disp_mesh in sel_disp_mesh]
 
-    def __show_ruler_callback(self, flag):
-        """This function shows ruler on UI when clicked on ruler button"""
+    def __show_ruler_callback(self, flag):  # pragma: no cover
+        """Show a ruler on the UI when ruler button is clicked."""
         if self._plotter is not None:
             if self._ruler_visible and self._ruler_actor is not None:
                 self._plotter.remove_actor(self._ruler_actor)
                 self._ruler_visible = False
             else:
                 self._ruler_actor = self._plotter.show_bounds(
                     grid='front',
@@ -430,36 +550,48 @@
                     show_xaxis=True,
                     show_yaxis=True,
                     show_zaxis=True,
                 )
                 self._ruler_visible = True
 
     def get_face_mesh_data(self):
-        """ """
+        """Get the mesh data from a face.
+
+        Returns
+        -------
+        List
+            Mesh data for the face.
+        """
         face_mesh_data = [
             disp_mesh
             for part_id, data in self._display_data.items()
             if data.get("faces") != None
             for disp_mesh in data["faces"]
         ]
         return face_mesh_data
 
     def show(self, update=False):
-        """ """
-        if os.getenv('PRIME_APP_RUN') and self._app is not None:
+        """Show the current set display.
+
+        Parameters
+        ----------
+        update : bool, optional
+            Whether to update the display. The default is ``False``.
+        """
+        if os.getenv('PRIME_APP_RUN') and self._app is not None:  # pragma: no cover
             app_g = self._app.Graphics().Get()
             app_g.DisplayModel()
             app_g.FitToScreen()
             return
         if update == True:
             self.__update_display_data()
 
         # if we use trame, activate OFF_SCREEN before initializing plotter
         pv_off_screen_original = None
-        if self._use_trame:
+        if self._use_trame:  # pragma: no cover
             pv_off_screen_original = pv.OFF_SCREEN
             pv.OFF_SCREEN = True
         self._plotter = pv.Plotter()
         self._plotter.show_axes()
         [
             disp_mesh.add_to_plotter(self._plotter)
             for part_id, data in self._display_data.items()
@@ -490,29 +622,39 @@
                 self.__show_ruler_callback, position=(10, 500), size=30, border_size=3
             )
         self._picker = Picker(self._plotter, self)
         self._plotter.track_click_position(self._picker, side='left')
         if self._sphinx_build == False:
             self.__update_bt_icons()
         self._show_selector()
-        if self._use_trame:
+        if self._use_trame:  # pragma: no cover
             pv.OFF_SCREEN = pv_off_screen_original
 
     def _show_selector(self):
         """Chooses between using Trame or Python visualizer."""
-        if self._use_trame:
+        if self._use_trame:  # pragma: no cover
             visualizer = TrameVisualizer()
             visualizer.set_scene(self._plotter)
             visualizer.show()
         else:
             self._plotter.show()
 
-    def __draw_parts(self, parts=[], update=False, spline=False):
-        """ """
-        if os.getenv('PRIME_APP_RUN') and self._app is not None:
+    def __draw_parts(self, parts: List = [], update: bool = False, spline: bool = False):
+        """Draw parts in the display.
+
+        Parameters
+        ----------
+        parts : list, optional
+            List of parts to display. The default is ``[]``.
+        update : bool, optional
+             Whether to update the display. The default is ``False``.
+        spline : bool, optional
+            Whether to use splines. The default is ``False``.
+        """
+        if os.getenv('PRIME_APP_RUN') and self._app is not None:  # pragma: no cover
             app_g = self._app.Graphics().Get()
             app_g.Clear()
             [app_g.DrawPart(part) for part in parts]
             app_g.FitToScreen()
             return
         if update == True:
             self.__update_display_data()
@@ -565,18 +707,26 @@
         self._plotter.track_click_position(self._picker, side='left')
         # self._plotter.window_size = [1920, 1017]
         if self._sphinx_build == False:
             self.__update_bt_icons()
         self._show_selector()
 
     def __draw_scope_parts(self, update=False, scope: prime.ScopeDefinition = None):
-        """ """
+        """Draws the scope of the parts.
+
+        Parameters
+        ----------
+        update : bool, optional
+            Whether to update the display. The default is ``False``.
+        scope : prime.ScopeDefinition, optional
+            Definition of the scopes. The default is ``None``.
+        """
         self._plotter = pv.Plotter()
         self._plotter.show_axes()
-        if os.getenv('PRIME_APP_RUN') and self._app is not None:
+        if os.getenv('PRIME_APP_RUN') and self._app is not None:  # pragma: no cover
             app_g = self._app.Graphics().Get()
             app_g.Clear()
         elif update == True:
             self.__update_display_data()
 
         parts = self._model.control_data.get_scope_parts(scope)
         scope_def = scope
@@ -625,14 +775,15 @@
         self._plotter.track_click_position(self._picker, side='left')
         # self._plotter.window_size = [1920, 1017]
         if self._sphinx_build == False:
             self.__update_bt_icons()
         self._show_selector()
 
     def __update_bt_icons(self):
+        """Update the icons on display."""
         vr = self._colorByTypeBt.GetRepresentation()
         vr.SetNumberOfStates(3)
         r = vtk.vtkPNGReader()
         color_by_zone_icon_file = os.path.join(os.path.dirname(__file__), 'images', 'bin.png')
         r.SetFileName(color_by_zone_icon_file)
         r.Update()
         image_1 = r.GetOutput()
@@ -671,20 +822,56 @@
         show_ruler_r.SetFileName(show_ruler_icon_file)
         show_ruler_r.Update()
         image_5 = show_ruler_r.GetOutput()
         show_ruler_vr.SetButtonTexture(0, image_5)
         show_ruler_vr.SetButtonTexture(1, image_5)
 
     def get_color_by_type(self) -> ColorByType:
-        """ """
+        """Get the color by zone type.
+
+        Returns
+        -------
+        ColorByType
+            Color by zone type.
+        """
         return self._color_by_type
 
 
-class _DisplayMesh(object):
-    """ """
+class _DisplayMesh(object):  # pragma: no cover
+    """Provides a helper class for displaying meshes in the plotter.
+
+    Parameters
+    ----------
+    type : DisplayMeshType
+        Type of the mesh.
+    id : int
+        ID of the mesh.
+    part_id : int
+        ID of the part to mesh.
+    graphics : Graphics
+        Instance of the ``Graphics`` class.
+    model : prime.Model
+        Model to show.
+    vertices : np.array
+        Vertices of the mesh.
+    facet_list : np.array
+        List of faces of the model.
+    has_mesh : bool
+        Whether the model is meshed.
+    zone_id : int, optional
+        ID of the zone. The default is ``0``.
+    zone_name : str, optional
+        Name of the zone. The default is ``""``.
+    part_name : str, optional
+        Name of the part. The default is ``""``.
+    topo_edge_type : int, optional
+        Type of the TopoEdge. The default is ``0``.
+    number_of_edges : int, optional
+        Number of edges in the model. The default is ``0``.
+    """
 
     def __init__(
         self,
         type: DisplayMeshType,
         id: int,
         part_id: int,
         graphics: Graphics,
@@ -694,15 +881,15 @@
         has_mesh: bool,
         zone_id: int = 0,
         zone_name: str = "",
         part_name: str = "",
         topo_edge_type: int = 0,
         number_of_edges: int = 0,
     ):
-        """ """
+        """Initialize the parameters to display."""
         self._type = type
         self._id = id
         self._part_id = part_id
         self._geom_id = None
         self._mesh_id = None
         self._graphics = graphics
         self._model = model
@@ -736,15 +923,21 @@
             msg += str(self._id)
         msg += ", in Part Id : " + str(self._part_id) + ", Part Name : " + self._part_name + "\n"
         if self._zone_id > 0:
             msg += "Zone Id : " + str(self._zone_id) + ", Zone Name : " + self._zone_name
         return msg
 
     def add_to_plotter(self, plotter: Plotter):
-        """ """
+        """Add elements to the plotter.
+
+        Parameters
+        ----------
+        plotter : Plotter
+            Elements of another plotter to add.
+        """
         if self._type == DisplayMeshType.TOPOFACE or self._type == DisplayMeshType.FACEZONELET:
             if self._poly_data == None:
                 surf = pv.PolyData(self._vertices, self._facet_list)
                 fcolor = np.array(self.get_face_color())
                 colors = np.tile(fcolor, (surf.n_faces, 1))
                 surf["colors"] = colors
                 surf.disp_mesh = self
@@ -809,26 +1002,38 @@
                 self._poly_data = surf
             if self._poly_data.n_points > 0:
                 self._actor = plotter.add_mesh(
                     self._poly_data, show_edges=False, scalars="colors", rgb=True, pickable=False
                 )
 
     def get_face_color(self):
-        """ """
+        """Get the colors of faces.
+
+        Returns
+        -------
+        List
+            List of colors for faces.
+        """
         type = self._graphics.get_color_by_type()
         num_colors = int(color_matrix.size / 3)
         if type == ColorByType.ZONELET:
             return color_matrix[self._id % num_colors].tolist()
         elif type == ColorByType.PART:
             return color_matrix[self._part_id % num_colors].tolist()
         else:
             return color_matrix[self._zone_id % num_colors].tolist()
 
     def get_edge_color(self):
-        """ """
+        """Get the colors of edges.
+
+        Returns
+        -------
+        List
+            List of colors for edges.
+        """
         num_colors = int(color_matrix.size / 3)
         if self._type == DisplayMeshType.EDGEZONELET:
             return color_matrix[self._id % num_colors].tolist()
         elif self._type == DisplayMeshType.TOPOEDGE:
             if self._topo_edge_type == 1:
                 return [255, 0, 0]
             elif self._topo_edge_type == 2:
@@ -881,15 +1086,21 @@
     def show_edges(self, show: bool):
         if self._actor is not None and self._has_mesh:
             prop = self._actor.GetProperty()
             self._show_edges = not prop.GetEdgeVisibility()
             prop.SetEdgeVisibility(not prop.GetEdgeVisibility())
 
     def set_color_by_type(self, type: ColorByType):
-        """ """
+        """Set the color based on the zone type.
+
+        Parameters
+        ----------
+        type : ColorByType
+            Color by zone type.
+        """
         if self._type == DisplayMeshType.TOPOFACE or self._type == DisplayMeshType.FACEZONELET:
             if self._poly_data != None:
                 fcolor = np.array(self.get_face_color())
                 colors = np.tile(fcolor, (self._poly_data.n_faces, 1))
                 self._poly_data["colors"] = colors
 
     @property
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/bin.png` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/bin.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/invert_visibility.png` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/invert_visibility.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/parts.png` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/parts.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/selectioninfo.png` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/selectioninfo.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/show_edges.png` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/show_edges.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/images/surface_body.png` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/surface_body.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/graphics/trame_gui.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/trame_gui.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,34 +7,35 @@
     _HAS_TRAME = True
 
 except ModuleNotFoundError:  # pragma: no cover
     _HAS_TRAME = False
 
 
 class TrameVisualizer:
-    """Trame visualizer class. It will define how the trame view layout will be."""
+    """Defines the view layout for the Trame visualizer."""
 
     def __init__(self) -> None:
-        """Inits server and server related variables."""
+        """Initialize the server and server-related variables."""
         if not _HAS_TRAME:  # pragma: no cover
             raise ModuleNotFoundError(
                 "The package 'pyvista[trame]' is required to use this function."
             )
 
         self.server = get_server()
         self.state, self.ctrl = self.server.state, self.server.controller
 
     def set_scene(self, plotter):
-        """Sets the trame layout view and the mesh to show
-        through the pyvista plotter.
+        """Set the view layout for the Trame visualizer.
+
+        This method also sets the mesh to show by the PyVista plotter.
 
         Parameters
         ----------
         plotter : pv.Plotter
-            PyVista plotter with the mesh rendered.
+            PyVista plotter to render the mesh.
         """
         self.state.trame__title = "PyPrime Viewer"
 
         with SinglePageLayout(self.server) as layout:
             layout.icon.click = self.ctrl.view_reset_camera
             layout.title.set_text("PyPrime")
 
@@ -43,9 +44,9 @@
                 view = plotter_ui(plotter)
                 self.ctrl.view_update = view.update
 
             # hide footer with trame watermark
             layout.footer.hide()
 
     def show(self):
-        """Starts the server and shows the mesh."""
+        """Start the server and show the mesh."""
         self.server.start()
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/client.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,55 @@
+"""Module for client communication implementations."""
+
 import logging
 import os
 
 import ansys.meshing.prime.examples as examples
 import ansys.meshing.prime.internals.config as config
 import ansys.meshing.prime.internals.defaults as defaults
 import ansys.meshing.prime.internals.utils as utils
 from ansys.meshing.prime.core.model import Model
 from ansys.meshing.prime.internals.utils import terminate_process
 
 __all__ = ['Client']
 
 
 class Client(object):
-    '''Client class for PyPrimeMesh.'''
+    """Provides the ``Client`` class for PyPrimeMesh.
+
+    Parameters
+    ----------
+    server_process : Any, optional
+        Server process in the system. The default is ``None``.
+    ip : str, optional
+        IP address where the server is located. The default is ``defaults.ip()``.
+    port : int, optional
+        Port where the server is deployed. The default is ``defaults.port()``.
+    timeout : float, optional
+        Maximum time to wait for connection. The default is ``defaults.connection_timeout()``.
+    credentials : Any, optional
+        Credentials to connect to the server. The default is ``None``.
+
+    Raises
+    ------
+    ValueError
+        Failed to load the communicator.
+    """
 
     def __init__(
         self,
         *,
         server_process=None,
         ip: str = defaults.ip(),
         port: int = defaults.port(),
         timeout: float = defaults.connection_timeout(),
         credentials=None,
         **kwargs,
     ):
+        """Initialize the client."""
         self._default_model: Model = None
         local = kwargs.get('local', False)
         if local and server_process is not None:
             raise ValueError('Local client cannot be instantiated with a server process')
         self._local = local
         self._process = server_process
         self._comm = None
@@ -65,49 +87,48 @@
             except ImportError as err:
                 logging.getLogger('PyPrimeMesh').error(
                     f'Failed to load prime_communicator with message: {err.msg}'
                 )
 
     @property
     def model(self):
-        '''Gets model associated with the client.'''
+        """Get the model associated with the client."""
         if self._default_model is None:
             # This assumes that the Model is always object id 1....
             self._default_model = Model(self._comm, 1, 1, "Default")
         return self._default_model
 
     def run_on_server(self, recipe: str):
-        '''Run a recipe on server.
+        """Run a recipe on the server.
 
         Parameters
         ----------
         recipe: str
-            Recipe to run on the server. This needs to be a valid
-            python script.
-        '''
+            Recipe to run. This must be a valid Python script.
+        """
         if self._comm is not None:
             result = self._comm.run_on_server(recipe)
             return result['Results']
 
     def exit(self):
-        '''Close the connection with the server.
+        """Close the connection with the server.
 
-        If the client had launched the server, then this will also
-        kill the server process.
+        If the client has launched the server, this method also
+        kills the server process.
 
         Examples
         --------
         >>> import ansys.meshing.prime as prime
-        >>> prime_client = prime.launch_prime() # This will launch a server process
+        >>> prime_client = prime.launch_prime() # This launches a server process.
         >>> model = prime_client.model
         >>> fileio = prime.FileIO(model)
         >>> result = fileio.read_pmdat('example.pmdat', prime.FileReadParams(model=model))
         >>> print(result)
-        >>> prime_client.exit() # Sever connection with server and kill server
-        '''
+        >>> prime_client.exit() # Sever connection with server and kill the server.
+        """
         if self._comm is not None:
             self._comm.close()
             self._comm = None
         if self._process is not None:
             assert self._local == False
             terminate_process(self._process)
             self._process = None
@@ -121,11 +142,13 @@
 
         clear_examples = bool(int(os.environ.get('PYPRIMEMESH_CLEAR_EXAMPLES', '1')))
         if clear_examples:
             download_manager = examples.DownloadManager()
             download_manager.clear_download_cache()
 
     def __enter__(self):
+        """Open client."""
         return self
 
     def __exit__(self, type, value, traceback):
+        """Close communication with the server when deleting the instance."""
         self.exit()
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/defaults.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/defaults.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-'''The default configuration for the PyPrimeMesh library.
-'''
+"""Default configuration for PyPrimeMesh."""
 
 __all__ = [
     'ip',
     'port',
     'connection_timeout',
     'print_communicator_stats',
     'max_message_length',
@@ -15,23 +14,24 @@
 
 import os
 
 try:
     import appdirs
 
     USER_DATA_PATH = os.getenv(
-        'PYPRIMEMESH_USER_DATA', appdirs.user_data_dir(appname='pyprimemesh', appauthor=False)
+        'PYPRIMEMESH_USER_DATA',
+        appdirs.user_data_dir(appname='ansys_meshing_prime', appauthor='Ansys'),
     )
 except ModuleNotFoundError:
     # If appdirs is not installed, then try with tempfile.
     # NOTE: This only occurs for ADO ARM Test runs
     import tempfile
 
     USER_DATA_PATH = os.getenv(
-        'PYPRIMEMESH_USER_DATA', os.path.join(tempfile.gettempdir(), 'pyprimemesh')
+        'PYPRIMEMESH_USER_DATA', os.path.join(tempfile.gettempdir(), 'ansys_meshing_prime')
     )
 
 if not os.path.exists(USER_DATA_PATH):  # pragma: no cover
     os.makedirs(USER_DATA_PATH)
 
 EXAMPLES_PATH = os.path.join(USER_DATA_PATH, 'examples')
 if not os.path.exists(EXAMPLES_PATH):  # pragma: no cover
@@ -43,75 +43,75 @@
 
 CONTAINER_USER_DATA = '/data'
 CONTAINER_EXAMPLES = os.path.join(CONTAINER_USER_DATA, 'examples')
 CONTAINER_OUTDIR = os.path.join(CONTAINER_USER_DATA, 'output')
 
 __DEFAULT_IP = '127.0.0.1'
 __DEFAULT_PORT = 50055
-__DEFAULT_CONNECTION_TIMEOUT = 10.0
+__DEFAULT_CONNECTION_TIMEOUT = 20.0
 __DEFAULT_COMM_LOG = False
 __MAX_MESSAGE_LENGTH = 4194310
 
 SPHINX_BUILD = bool(int(os.getenv('PYPRIMEMESH_SPHINX_BUILD', 0)))
 
 
 def ip():
-    '''Gets the default ip address used throughout the library.'''
+    """Get the default IP address used throughout the library."""
     return __DEFAULT_IP
 
 
 def port():
-    '''Gets the default port used throughout the library.'''
+    """Get the default port used throughout the library."""
     return __DEFAULT_PORT
 
 
 def connection_timeout():
-    '''Gets the default connection timeout used throughout the library.'''
+    """Get the default connection timeout used throughout the library."""
     return __DEFAULT_CONNECTION_TIMEOUT
 
 
 def print_communicator_stats():
-    '''INTERNAL ONLY: Gets the flag to decide whether to print communicator stats.'''
+    """Get the flag to decide whether to print communicator stats(INTERNAL ONLY)."""
     return __DEFAULT_COMM_LOG
 
 
 def max_message_length():
-    '''Gets the maximum message length for a grpc channel'''
+    """Get the maximum message length for a grpc channel."""
     return __MAX_MESSAGE_LENGTH
 
 
 def get_examples_path():
-    '''Gets the client side default container path'''
+    """Get the client-side default container path."""
     return EXAMPLES_PATH
 
 
 def get_user_data_path():
-    '''Gets the client side default user data path'''
+    """Get the client-side default user data path."""
     return USER_DATA_PATH
 
 
 def get_user_data_path_for_containers():
-    '''Gets the user data path for containers'''
+    """Get the user data path for containers."""
     return CONTAINER_USER_DATA
 
 
 def get_examples_path_for_containers():
-    '''Gets the server side default container path in case of containers
+    """Get the server-side default container path in case of containers.
 
-    In case of a container, the user data directory is mounted within on the container image.
-    '''
+    In case of a container, the user data directory is mounted within the container image.
+    """
     return CONTAINER_EXAMPLES
 
 
 def get_output_path():
-    '''Gets the client side output directory used by containers'''
+    """Get the client-side output directory used by containers."""
     return LOCAL_OUTDIR
 
 
 def get_output_path_for_containers():
-    '''Gets the server side output directory used by containers'''
+    """Get the server-side output directory used by containers."""
     return CONTAINER_OUTDIR
 
 
 def get_sphinx_build():
-    '''Gets the flag for if sphinx build is being used'''
+    """Get the flag for if sphinx build is being used."""
     return SPHINX_BUILD
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/error_handling.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/error_handling.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Module for error handling in PyPrimeMesh."""
 import re
 from functools import wraps
 
 from ansys.meshing.prime.autogen.primeconfig import ErrorCode, WarningCode
 
 prime_error_messages = {
     ErrorCode.NOERROR: "Success.",
@@ -322,26 +323,50 @@
     WarningCode.MESHHASLEFTHANDEDNESSFACES: "Mesh has left handed faces.",
     WarningCode.FACEZONELETSWITHOUTVOLUMES: "Face zonelets have no volume associated to them.",
     WarningCode.JOINEDZONELETSFROMMULTIPLEVOLUMES: "Joined zonelets from more than two volumes. The volumes are not auto updated on the zonelets.",
 }
 
 
 class PrimeRuntimeError(Exception):
-    '''Runtime error for PyPrimeMesh.'''
+    """Provides runtime errors for PyPrimeMesh.
 
-    def __init__(self, message, error_code: ErrorCode = None, error_locations=None):
+    Parameters
+    ----------
+    message : str
+        Error message to show.
+    error_code : ErrorCode, optional
+        ID of the error. The default is ``None``.
+    error_locations : Any, optional
+        Location of the error. The default is ``None``.
+    """
+
+    def __init__(self, message: str, error_code: ErrorCode = None, error_locations=None):
+        """Initialize the error message."""
         super().__init__()
         self._message = self.__process_message(message)
         self._error_code = error_code
         self._error_locations = error_locations
 
     def __str__(self) -> str:
+        """Transform the message to a string."""
         return self._message
 
     def __process_message(self, message: str):
+        """Process the message to be digested by the error class.
+
+        Parameters
+        ----------
+        message : str
+            Message to process.
+
+        Returns
+        -------
+        str
+            Processed message.
+        """
         output_message = message
         if "Invalid Parameter Type: " in message:
             param_names = message[len("Invalid Parameter Type: ") :].split(".")
             output_message = "Invalid Parameter Type: " + param_names[0]
             if len(param_names) > 1:
                 for name in param_names[1:]:
                     output_message += "." + re.sub(r'(?<!^)(?=[A-Z])', '_', name).lower()
@@ -360,38 +385,64 @@
     @property
     def error_locations(self) -> list:
         """Locations associated with the error."""
         return self._error_locations
 
 
 class PrimeRuntimeWarning(UserWarning):
-    '''Runtime warning for PyPrimeMesh.'''
+    """Provides the runtime warning for PyPrimeMesh.
+
+    Parameters
+    ----------
+    message : str
+        Message to show.
+    """
 
     def __init__(self, message):
+        """Initialize the warning message."""
         super().__init__()
         self._message = message
 
     def __str__(self) -> str:
+        """Transform the message to a string."""
         return self._message
 
     @property
     def message(self):
         """Warning message to be reported."""
         return self._message
 
 
 def communicator_error_handler(
     _func=None,
     *,
-    expected_token='Results',
-    server_error_token='ServerError',
-    info_token='info_msg',
-    warning_token='warning_msg',
-    error_token='err_msg',
+    expected_token="Results",
+    server_error_token="ServerError",
+    info_token="info_msg",
+    warning_token="warning_msg",
+    error_token="err_msg",
 ):
+    """Create a decorator to use in error handling.
+
+    Parameters
+    ----------
+    _func : Func, optional
+        Function to use as decorator. The default is ``None``.
+    expected_token : str, optional
+        Token to expect in the response result. The default is ""Results"".
+    server_error_token : str, optional
+        Token from the server error. The default is ``"ServerError"``.
+    info_token : str, optional
+        Information message. The default is ``"info_msg"``.
+    warning_token : str, optional
+        Warning message. The default is ``"warning_msg"``.
+    error_token : str, optional
+        Error message. The default is ``"err_msg"``.
+    """
+
     def decorator_handle_errors(func):
         @wraps(func)
         def wrapper_handle_errors(*args, **kwargs):
             func_result = func(*args, **kwargs)
             if func_result is None:
                 return func_result
             server_error = func_result.get(server_error_token, None)
@@ -420,14 +471,22 @@
     if _func is None:
         return decorator_handle_errors
     else:
         return decorator_handle_errors(_func)
 
 
 def error_code_handler(_func=None):
+    """Decode errors from the server.
+
+    Parameters
+    ----------
+    _func : Func, optional
+        Decorator to apply to the error code. The default is ``None``.
+    """
+
     def decorator_error_code(func):
         @wraps(func)
         def wrapper_error_code(*args, **kwargs):
             try:
                 result = func(*args, **kwargs)
             except RuntimeError as err:
                 import logging
@@ -492,13 +551,23 @@
     if _func is None:
         return decorator_error_code
     else:
         return decorator_error_code(_func)
 
 
 def apply_if(decorator, condition):
+    """Apply a function based on a condition.
+
+    Parameters
+    ----------
+    decorator : Func
+        Function to apply.
+    condition : bool
+        Condition to check.
+    """
+
     def decorator_apply_if(func):
         if not condition:
             return func
         return decorator(func)
 
     return decorator_apply_if
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/grpc_communicator.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/grpc_communicator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+"""Module for communications with the gRPC server."""
 __all__ = ['GRPCCommunicator']
 from typing import Optional
 
 import grpc
 from ansys.api.meshing.prime.v1 import prime_pb2, prime_pb2_grpc
 
 import ansys.meshing.prime.internals.config as config
 import ansys.meshing.prime.internals.defaults as defaults
 import ansys.meshing.prime.internals.grpc_utils as grpc_utils
 import ansys.meshing.prime.internals.json_utils as json
+from ansys.meshing.prime.core.model import Model
 from ansys.meshing.prime.internals.communicator import Communicator
 from ansys.meshing.prime.internals.error_handling import (
     communicator_error_handler,
     error_code_handler,
 )
 
 # Keep some buffer for gRPC metadata that it may want to send
@@ -40,42 +42,81 @@
 
 
 def get_response(response_iterator, separator):
     return separator.join(response.data for response in get_response_messages(response_iterator))
 
 
 class GRPCCommunicator(Communicator):
+    """Manages communication with the gRPC server.
+
+    Parameters
+    ----------
+    ip : Optional[str], optional
+        IP address where the server is located. The default is ``None``.
+    port : Optional[int], optional
+        Port where the server is deployed. The default is ``None``.
+    timeout : float, optional
+        Maximum time to wait for connection. The default is ``10.0``.
+    credentials : Any, optional
+        Credentials for connecting to the server. The default is ``None``.
+
+    Raises
+    ------
+    ConnectionError
+        Could not connect to server.
+    """
+
     def __init__(
         self,
         ip: Optional[str] = None,
         port: Optional[int] = None,
         timeout: float = 10.0,
         credentials=None,
         **kwargs,
     ):
+        """Initialize the server connection."""
         self._channel = kwargs.get('channel', None)
         if self._channel is None:
             ip_addr = f"{ip}:{port}"
             channel_options = grpc_utils.get_default_channel_args()
             if credentials is None:
                 self._channel = grpc.insecure_channel(ip_addr, options=channel_options)
             else:
                 self._channel = grpc.secure_channel(ip_addr, credentials, options=channel_options)
         try:
             grpc.channel_ready_future(self._channel).result(timeout=timeout)
         except grpc.FutureTimeoutError as err:
             raise ConnectionError(
-                'Failed to connect to Server in given timeout of 10 secs'
+                f'Failed to connect to Server in given timeout of {timeout} secs'
             ) from err
 
         self._stub = prime_pb2_grpc.PrimeStub(self._channel)
 
     @error_code_handler
     @communicator_error_handler
-    def serve(self, model, command, *args, **kwargs) -> dict:
+    def serve(self, model: Model, command: str, *args, **kwargs) -> dict:
+        """Serve model and send a command to the server.
+
+        Parameters
+        ----------
+        model : Model
+            Model to serve.
+        command : str
+            Command to send.
+
+        Returns
+        -------
+        dict
+            Response from the server.
+
+        Raises
+        ------
+        RuntimeError
+            Can not connect to server.
+        """
         if self._stub is not None:
             command = {"Command": command}
             if len(args) > 0:
                 command.update({"ObjectID": args[0]})
             if kwargs is not None:
                 if "args" in kwargs:
                     command.update({"Args": kwargs["args"]})
@@ -110,15 +151,34 @@
                 logging.getLogger("PyPrimeMesh").info(
                     f'Data Transfer: Received {len(message)} bytes'
                 )
             return json.loads(message)
         else:
             raise RuntimeError("No connection with server")
 
-    def initialize_params(self, model, param_name: str, *args) -> dict:
+    def initialize_params(self, model: Model, param_name: str, *args) -> dict:
+        """Initialize parameters on the server side.
+
+        Parameters
+        ----------
+        model : Model
+            Model to initialize parameters on.
+        param_name : str
+            Parameter to initialize.
+
+        Returns
+        -------
+        dict
+            Response from the server.
+
+        Raises
+        ------
+        RuntimeError
+            Can not connect to server.
+        """
         if self._stub is not None:
             command = {"ParamName": param_name}
             with config.numpy_array_optimization_disabled():
                 response = self._stub.GetParamDefaultJson(
                     request_iterator(
                         model._object_id,
                         json.dumps(command),
@@ -130,15 +190,38 @@
                 )
                 message = get_response(response, '')
                 result = json.loads(message)
             return result
         else:
             raise RuntimeError("No connection with server")
 
-    def run_on_server(self, model, recipe: str) -> dict:
+    def run_on_server(self, model: Model, recipe: str) -> dict:
+        """Run commands on the server.
+
+        Run commands on a model on the server.
+
+        Parameters
+        ----------
+        model : core.Model
+            Model to run commands on.
+        recipe : str
+            Commands to run.
+
+        Returns
+        -------
+        dict
+            Result from the server side.
+
+        Raises
+        ------
+        RuntimeError
+            Bad response from server.
+        RuntimeError
+            Can not connect to server.
+        """
         if self._stub is not None:
             commands = recipe
             response = self._stub.RunOnServer(
                 request_iterator(
                     model._object_id,
                     commands,
                     prime_pb2.StringMessage,
@@ -153,14 +236,16 @@
             if "Error" in result:
                 raise RuntimeError(result['Error'])
             return result
         else:
             raise RuntimeError("No connection with server")
 
     def close(self):
+        """Close opened channels."""
         self._stub = None
         if self._channel is not None:
             self._channel.close()
             self._channel = None
 
     def __del__(self):
+        """Close communication when deleting the instance."""
         self.close()
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/json_utils.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/json_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,49 @@
+"""Module for JSON utility functions."""
 import json
 from typing import Union
 
 import numpy as np
 
 import ansys.meshing.prime.internals.config as config
 import ansys.meshing.prime.relaxed_json as relaxed_json
 
 __all__ = ['loads', 'dumps']
 
 
 def try_process_as_iterable(obj):
+    """Try if an object is an iterable and return its list.
+
+    Parameters
+    ----------
+    obj : Any
+        Object to test.
+
+    Returns
+    -------
+    List
+        List of the object.
+    """
     iterable = iter(obj)
     return list(iterable)
 
 
 def try_process_numpy_array(obj):
+    """Try if an object is a numpy array and return its list.
+
+    Parameters
+    ----------
+    obj : Any
+        Object to test.
+
+    Returns
+    -------
+    bool, list
+        Whether the object is a numpy array and the list of the object.
+    """
     if isinstance(obj, np.ndarray):
         return True, obj.tolist()
     return False, obj
 
 
 class _CustomJSONEncoder(json.JSONEncoder):
     def default(self, obj):
@@ -41,19 +66,43 @@
         except TypeError:
             pass
 
         return super().default(obj)
 
 
 def loads(s: Union[str, bytes, bytearray], *args, **kwargs):
+    """Load JSON from an input string.
+
+    Parameters
+    ----------
+    s : Union[str, bytes, bytearray]
+        Input string.
+
+    Returns
+    -------
+    json
+        Object converted to JSON.
+    """
     if config.is_optimizing_numpy_arrays():
         return relaxed_json.loads(s, *args, **kwargs)
     return json.loads(s, *args, **kwargs)
 
 
 def dumps(obj, *args, **kwargs):
+    """Dump JSON to an object.
+
+    Parameters
+    ----------
+    obj : Any
+        Input object.
+
+    Returns
+    -------
+    Object
+        JSON converted to an object.
+    """
     if config.is_optimizing_numpy_arrays():
         kwargs.setdefault('cls', _CustomBinaryJSONEncoder)
         return relaxed_json.dumps(obj, *args, **kwargs)
 
     kwargs.setdefault('cls', _CustomJSONEncoder)
     return json.dumps(obj, *args, **kwargs)
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/launcher.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/launcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Helper module for launching the server."""
 import logging
 import os
 import subprocess
 import sys
 from typing import Optional
 
 import ansys.meshing.prime.internals.config as config
@@ -48,40 +49,40 @@
 def launch_server_process(
     prime_root: Optional[str] = None,
     ip: str = defaults.ip(),
     port: int = defaults.port(),
     n_procs: Optional[int] = None,
     **kw,
 ) -> subprocess.Popen:
-    '''Launch a server process for Ansys Prime Server.
+    """Launch a server process for Ansys Prime Server.
 
     Parameters
     ----------
-    prime_root: Optional[str]
-        Root directory which contains the Ansys Prime Server.
+    prime_root : str, optional
+        Root directory for Ansys Prime Server.
     ip: str
-        IP address to start the server at.  The default IP address is 127.0.0.1.
+        IP address to start the server at. The default is ``127.0.0.1``.
     port: int
-        Port at which the server is started. The default port is 50055.
+        Port at which the server is started. The default is ``50055``.
     n_procs: Optional[int]
-        When running in distributed mode, specify the number of distributed
-        processes to spawn. Process marked as Node 0 will host the GRPC
-        server. If None is specified, server will be launched as the only
-        process (normal mode).
+        When running in distributed mode, the number of distributed
+        processes to spawn. The default is ``None``, in which case
+        the server is launched as the only process (normal mode). The
+        process marked as ``Node 0`` hosts the gRPC server.
 
     Returns
     -------
     subprocess.Popen
-        The instance of the subprocess that is launched.
+        Instance of the subprocess that is launched.
 
     Raises
     ------
     FileNotFoundError
         When there is an error in the file paths used to launch the server.
-    '''
+    """
     if prime_root is None:
         prime_root = get_ansys_prime_server_root()
         if prime_root is None:
             raise FileNotFoundError('No valid Ansys Prime Server found to launch.')
     else:  # verify if the file exists
         if not os.path.isdir(prime_root):
             raise FileNotFoundError('Invalid exec_file path.')
@@ -138,19 +139,19 @@
     server = subprocess.Popen(server_args, **kwargs)
     return server
 
 
 def launch_remote_prime(
     version: Optional[str] = None, timeout: float = defaults.connection_timeout()
 ):
-    '''Create a remote instance of Prime server using PyPIM
+    """Create a remote instance of Ansys Prime Server using PyPIM.
 
-    This method is used in case of Ansys Labs to create a remote instance of prime.
-    This method also creates a file transfer service that is available on Ansys Labs
-    '''
+    This method is used if Ansys Lab creates a remote instance of Ansys Prime Server.
+    This method creates a file transfer service that is available on Ansys Lab.
+    """
     if version is None:
         version = 'latest'
 
     pim = pypim.connect()
     instance = pim.create_instance(product_name='prime', product_version=version)
     instance.wait_for_ready()
 
@@ -183,45 +184,45 @@
     ip: str = defaults.ip(),
     port: int = defaults.port(),
     timeout: float = defaults.connection_timeout(),
     n_procs: Optional[int] = None,
     version: Optional[str] = None,
     **kwargs,
 ):
-    '''Launch an instance of Ansys Prime Server and get a client for it.
+    """Launch an instance of Ansys Prime Server and get a client for it.
 
     Parameters
     ----------
     prime_root: Optional[str]
-        Root directory which contains the Ansys Prime Server.
+        Root directory for Ansys Prime Server.
     ip: str
-        IP address to start the server at.  The default IP address is 127.0.0.1.
+        IP address to start the server at. The default is ``127.0.0.1``.
     port: int
-        Port at which the server is started.  The default port is 50055.
+        Port at which the server is started. The default is ``50055``.
     timeout: float
         Maximum time in seconds to wait for the client to connect to the server.
-        The default is 10.0 seconds
+        The default is ``20.0``.
     n_procs: Optional[int]
-        When running in distributed mode, specify the number of distributed
-        processes to spawn. Process marked as Node 0 will host the GRPC
-        server. If None is specified, server will be launched as the only
-        process (normal mode).
+        When running in distributed mode, the number of distributed
+        processes to spawn. The default is ``None``, in which case
+        the server is launched as the only process (normal mode). The
+        process marked as ``Node 0`` hosts the gRPC server.
 
     Returns
     -------
     Client
-        The instance of the client that is connected to the launched server.
+        Instance of the client that is connected to the launched server.
 
     Raises
     ------
     FileNotFoundError
         When there is an error in file paths used to launch the server.
     ConnectionError
-        When there is an error in connecting to the GRPC server.
-    '''
+        When there is an error in connecting to the gRPC server.
+    """
     if config.has_pim():
         return launch_remote_prime(version=version, timeout=timeout)
 
     # Check for port availability on local host
     if ip == defaults.ip():
         port = utils.get_available_local_port(port)
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/internals/utils.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,53 @@
+"""Module for general utilities of the project."""
 import logging
 import os
 import shutil
 import subprocess
 from contextlib import contextmanager
-from typing import Optional
+from typing import List, Optional
 
 import ansys.meshing.prime.internals.config as config
 import ansys.meshing.prime.internals.defaults as defaults
 
 _LOCAL_PORTS = []
 
 
 def to_camel_case(snake_str):
+    """Transform snake_case string to camelCase.
+
+    Parameters
+    ----------
+    snake_str : str
+        snake_case string.
+
+    Returns
+    -------
+    str
+        String converted to camelCase.
+    """
     components = snake_str.split('_')
     # We capitalize the first letter of each component except the first one
     # with the 'title' method and join them together.
     return components[0] + ''.join(x.title() for x in components[1:])
 
 
 def get_child_processes(process):
+    """Get child processes of a process.
+
+    Parameters
+    ----------
+    process : int
+        Process ID of the parent process.
+
+    Returns
+    -------
+    List
+        Process IDs of the processes.
+    """
     children = []
     cmd = subprocess.Popen("pgrep -P %d" % process, shell=True, stdout=subprocess.PIPE)
     out = cmd.stdout.read().decode("utf-8")
     cmd.wait()
     for pid in out.split("\n")[:1]:
         if pid.strip() == '':
             break
@@ -35,15 +60,22 @@
         if "AnsysPrimeServer" in cmd_name:
             children.append(int(pid))
         else:
             children += get_child_processes(int(pid))
     return children
 
 
-def terminate_process(process):
+def terminate_process(process: subprocess):
+    """Terminates a process.
+
+    Parameters
+    ----------
+    process : subprocess
+        Process to terminate.
+    """
     import signal
     import sys
 
     if sys.platform.startswith('win32'):
         # process.send_signal(signal.CTRL_C_EVENT)
         process.send_signal(signal.CTRL_BREAK_EVENT)
     else:
@@ -57,14 +89,25 @@
     if process.stderr is not None:
         process.stderr.close()
     process.terminate()
     process.wait()
 
 
 def print_logs_before_command(logger: logging.Logger, command: str, args):
+    """Print logs before running a command.
+
+    Parameters
+    ----------
+    logger : logging.Logger
+        Logger to print to.
+    command : str
+        Command to run.
+    args : str
+        Arguments of the command.
+    """
     logger.info("Executing " + command)
     if logger.isEnabledFor(logging.DEBUG):
         logger.debug("Command: " + command)
         logger.debug("Args:")
         for key in args:
             logger.debug("    " + key + ":")
             val = args[key]
@@ -77,14 +120,25 @@
                 printable_str = str(val)
             for line in printable_str.splitlines():
                 logger.debug("        " + line)
         logger.debug("")
 
 
 def print_logs_after_command(logger: logging.Logger, command: str, ret):
+    """Print logs after running a command.
+
+    Parameters
+    ----------
+    logger : logging.Logger
+        Logger to print to.
+    command : str
+        Command to run.
+    ret : str
+        Return type of the command.
+    """
     logger.info("Finished " + command)
     if logger.isEnabledFor(logging.DEBUG):
         logger.debug("Return: ")
         printable_str = ""
         if hasattr(ret, '__str__'):
             printable_str = ret.__str__()
         elif type(ret) == 'str':
@@ -96,17 +150,38 @@
         logger.debug("")
 
 
 def launch_prime_github_container(
     mount_host: str = defaults.get_user_data_path(),
     mount_image: str = defaults.get_user_data_path_for_containers(),
     port: int = defaults.port(),
-    name: str = 'ansys-prime-server',
+    name: str = "ansys-prime-server",
     version: Optional[str] = None,
 ):
+    """Launch a container.
+
+    Parameters
+    ----------
+    mount_host : str, optional
+        IP address for the container to mount. The default is ``defaults.get_user_data_path()``.
+    mount_image : str, optional
+        Name of the path to the container to mount. The default is
+        ``defaults.get_user_data_path_for_containers()``.
+    port : int, optional
+        Port to expose. The default is ``defaults.port()``.
+    name : str, optional
+        Name of the container. The default is ``"ansys-prime-server"``.
+    version : str, optional
+        Version of the container to retrieve. The default is ``None``.
+
+    Raises
+    ------
+    ValueError
+        License is not available.
+    """
     license_file = os.environ.get('ANSYSLMD_LICENSE_FILE', None)
     image_name = os.environ.get('PYPRIMEMESH_IMAGE_NAME', 'ghcr.io/ansys/prime')
     if license_file is None:
         raise ValueError('Licensing information to launch container not found')
     if version is None:
         version = os.environ.get('PYPRIMEMESH_IMAGE_TAG', 'latest')
     docker_command = [
@@ -126,19 +201,44 @@
         '--port',
         f'{port}',
     ]
     subprocess.run(docker_command, stdout=subprocess.DEVNULL)
 
 
 def stop_prime_github_container(name):
+    """Stop a running container.
+
+    Parameters
+    ----------
+    name : str
+        Name of the container.
+    """
     subprocess.run(['docker', 'stop', f'{name}'], stdout=subprocess.DEVNULL)
 
 
 @contextmanager
-def file_read_context(model, file_name):
+def file_read_context(model, file_name: str):
+    """Upload context.
+
+    Upload context to a model.
+
+    Parameters
+    ----------
+    model : Model
+        Model to upload the context to.
+    file_name : str
+        Name of the file containing the context.
+
+    Yields
+    ------
+    str
+        File name of the context.
+    """
+    if config.file_existence_check_enabled() and not os.path.exists(file_name):
+        raise FileNotFoundError(f'Given file name "{file_name}" is not found on local disk')
     if config.using_container():
         base_file_name = os.path.basename(file_name)
         temp_file_name = os.path.join(defaults.get_examples_path(), base_file_name)
         is_copy: bool = file_name != temp_file_name
         if is_copy:
             shutil.copyfile(file_name, temp_file_name)
         container_file_name = os.path.join(
@@ -153,41 +253,88 @@
         model.file_service.upload_file(file_name)
         yield temp_file_name
     else:
         yield file_name
 
 
 def port_in_use(port, host=defaults.ip()):
-    """Returns True when a port is in use at the given host.
-    Must actually "bind" the address.  Just checking if we can create
-    a socket is insufficient as it's possible to run into permission
-    errors like:
+    """Check if a port is in use on a given host.
+
+    This method must actually check is is a "bind" of the port to the
+    address. Just checking if a socket can be created is insufficient
+    because it's possible to run into permission errors like this one:
+
     - An attempt was made to access a socket in a way forbidden by its
       access permissions.
+
+    Parameters
+    ----------
+    port : int
+        Port to check.
+    host : str, optional
+        IP address to check. The default is ``defaults.ip()``.
+
+    Returns
+    -------
+    bool
+        ``True`` if the port is in use, ``False`` if the port is available.
     """
     import socket
 
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
         try:
             sock.bind((host, port))
             return False
         except:
             return True
 
 
 def get_available_local_port(init_port: int = defaults.port()):
+    """Get which ports are available and return the first one.
+
+    Parameters
+    ----------
+    init_port : int, optional
+        Port to start the search from. The default is ``defaults.port()```.
+
+    Returns
+    -------
+    int
+        First available port.
+    """
     port = init_port
     while port_in_use(port) or port in _LOCAL_PORTS:
         port += 1
     _LOCAL_PORTS.append(port)
     return port
 
 
 @contextmanager
-def file_read_context_list(model, file_names):
+def file_read_context_list(model, file_names: List[str]):
+    """Upload context.
+
+    Upload context to a model.
+
+    Parameters
+    ----------
+    model : Model
+        Model to upload context to.
+    file_names : List[str]
+        List of files with the context.
+
+    Yields
+    ------
+    List[str]
+        List of context files.
+    """
+    if config.file_existence_check_enabled():
+        for file in file_names:
+            if not os.path.exists(file):
+                error_msg = f"File {file} given for read is missing from local disk."
+                raise FileNotFoundError(error_msg)
     if config.using_container():
         base_names = [os.path.basename(file) for file in file_names]
         temp_names = [os.path.join(defaults.get_examples_path(), base) for base in base_names]
         for file, temp in zip(file_names, temp_names):
             shutil.copyfile(file, temp)
         container_files = [
             os.path.join(defaults.get_examples_path_for_containers(), base) for base in base_names
@@ -202,15 +349,31 @@
             model.file_service.upload_file(file)
         yield temp_files
     else:
         yield file_names
 
 
 @contextmanager
-def file_write_context(model, file_name):
+def file_write_context(model, file_name: str):
+    """Download context.
+
+    Download context from a model and write it to a local file.
+
+    Parameters
+    ----------
+    model : Model
+        Model to download context from.
+    file_name : str
+        Name of the file to write the context to.
+
+    Yields
+    ------
+    str
+        Name of the file to which context has been written.
+    """
     if config.using_container():
         base_file_name = os.path.basename(file_name)
         temp_file_name = os.path.join(defaults.get_output_path_for_containers(), base_file_name)
         temp_file_name = temp_file_name.replace(os.path.sep, '/')
         if not os.path.exists(defaults.get_output_path()):
             os.makedirs(defaults.get_output_path())
         yield temp_file_name
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/lucid/mesh_util.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/lucid/mesh_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,75 +1,78 @@
+"""Module for meshing utility functions."""
 import enum
 import os
 from typing import Iterable, List
 
 import ansys.meshing.prime as prime
 
 from .scope import SurfaceScope, VolumeScope
 from .utils import check_name_pattern
 
 
 class LabelToZoneMethod(enum.IntEnum):
-    """Method to create zones from labels."""
+    """Provides for creating zones from labels."""
 
     SIMPLE = 0
     """
-    Simple method to create zones from labels.
-    Entities are queried using labels and zones created.
+    Simple method for creating zones from labels.
+
+    Entities are queried using labels, and zones are created.
     """
 
 
 class Mesh:
-    """Mesh is one of the classes in Lucid API.
+    """Provides methods for users who are new to meshing.
+
+    This class also serves as a tutorial for commonly used meshing workflows.
+
+    The ``Mesh`` class provides these functionalities:
 
-    This class is meant for beginners to meshing.
-    It also serves as a tutorial for commonly used meshing workflows.
+    * Surface meshing with constant and variable sizing with triangle
+      or quad dominant mesh
+    * Volume meshing with prism, tetrahedral, and polyhedral elements
+    * Surface wrapping
+    * Helper method for creating zones from labels
+    * Helper methods for reading and writing files
 
-    The following functionalities are provided by this class:
-    * Surface meshing with constant and variable sizing with triangle or quad dominant mesh.
-    * Volume meshing with prism, tetrahedral and polyhedral elements.
-    * Surface wrapping.
-    * Helper method to create zones from labels.
-    * Helper methods for reading and writing files.
     """
 
     def __init__(self, model: prime.Model):
-        """Initialize mesher using model.
+        """Initialize the mesher using a model.
 
         Parameters
         ----------
         model : prime.Model
-            Model on which the methods work.
+            Model that the methods are to work on.
         """
         self._model = model
         self._logger = model.python_logger
 
     def read(
         self, file_name: str, append: bool = False, cad_reader_route: prime.CadReaderRoute = None
     ):
-        """Read or import files of different formats based on file extension.
+        """Read or import files of different formats based on file extensions.
 
-        PyPrimeMesh's native file format has extension pmdat.
-        The method supports the following:
-        * Reading PyPrimeMesh's native file format.
-        * Importing various CAD Formats.
-        * Importing Fluent Meshing's msh file.
-        * Importing Fluent cas file.
-        * Importing MAPDL cdb files.
+        This method supports reading and importing these file formats:
+
+        * Reading PyPrimeMesh's native PMDAT files
+        * Importing various types of CAD files
+        * Importing Fluent Meshing's MSH files
+        * Importing Fluent's CAS files
+        * Importing MAPDL's CDB files
 
         Parameters
         ----------
         file_name : str
-            Path to file to be read or imported.
-
-        append : bool
-            Set it to True to append instead of overwrite.
-
-        cad_reader_route : prime.CadReaderRoute
-            Route of CadReader.
+            Path to the file to read or import.
+        append : bool, optional
+            Whether to append to the file. The default is ``False``, in which case
+             the file is overwritten.
+        cad_reader_route : prime.CadReaderRoute, optional
+            Route of the CAD reader. The default is ``None``.
 
         """
         filename, fileext = os.path.splitext(file_name)
         if fileext == ".msh" or file_name[-7:] == ".msh.gz":
             prime.FileIO(self._model).import_fluent_meshing_meshes(
                 [file_name], prime.ImportFluentMeshingMeshParams(self._model, append=append)
             )
@@ -90,27 +93,27 @@
                 file_name,
                 prime.ImportCadParams(
                     self._model, append=append, cad_reader_route=cad_reader_route
                 ),
             )
 
     def write(self, file_name: str):
-        """Write or export files of different formats based on file extension.
+        """Write or export files of different formats based on file extensions.
+
+        This method supports writing and exporting these file formats:
 
-        PyPrimeMesh's native file format has extension pmdat.
-        The method supports the following:
-        * Writing PyPrimeMesh's native file format.
-        * Exporting Fluent Meshing's msh file.
-        * Exporting Fluent cas file.
-        * Exporting MAPDL cdb files.
+        * Writing PyPrimeMesh's native PMDAT files
+        * Exporting Fluent Meshing's MSH files
+        * Exporting Fluent's CAS files
+        * Exporting MAPDL's CDB files.
 
         Parameters
         ----------
         file_name : str
-            Path of file to be written or exported.
+            Path of the file to write or export.
 
         """
         filename, fileext = os.path.splitext(file_name)
         if fileext == ".cdb":
             prime.FileIO(self._model).export_mapdl_cdb(
                 file_name, prime.ExportMapdlCdbParams(self._model)
             )
@@ -132,39 +135,39 @@
     ):
         """Create zones from labels.
 
         When exporting to various solvers, zones play a very important role.
         Zones are where material properties and boundary conditions
         can be set in respective solvers.
 
-        Zones allow downstream setting of
-        boundary conditions or material properties.
+        Zones allow downstream setting of boundary conditions or material properties.
 
-        Zone names in PyPrimeMesh are translated into equivalent concepts in solver.
-        Currently, only one method is available to convert zone to label.
-        Currently, only face zones are created.
-
-        The method finds the entities by labels and then adds them to the
-        zone with the same name as label.
-
-        If no label_expression is provided then all labels will be flattened to
-        create zones.  Label names will be combined if overlaps occur and
-        separate zones created.
-
-        For example, if "LabelA" and "LabelB" had overlapping TopoFaces then
-        the following three zones would be created;
-        "LabelA", "LabelB" and "LabelA_LabelB" for the overlap.
+        Zone names in PyPrimeMesh are translated into equivalent concepts in the solver.
+        Currently, only one method is available to convert a zone to a label, and
+        only face zones are created.
+
+        The ``create_zones_from_labels`` method finds the entities by labels
+        and then adds them to zones with the same names as the labels.
+
+        If the ``label_expression`` parameter is not provided, all labels are
+        flattened to create zones. If overlaps occur, label names are combined, and
+        separate zones are created.
+
+        For example, if "LabelA" and "LabelB" have overlapping TopoFaces,
+        these zones are created: ``"LabelA"``, ``"LabelB"``, and
+        ``"LabelA_LabelB"`` for the overlap.
 
         Parameters
         ----------
-        label_expression : str
-            Expression for labels to be converted to zones.
-
-        conversion_method : LabelToZoneMethod
-            Method used to convert label to zones.
+        label_expression : str, optional
+            Expression for the labels to convert to zones. The
+            default is ``None``.
+        conversion_method : LabelToZoneMethod, optional
+            Method for converting the labels to zones. The default
+            is ``LabelToZoneMethod.SIMPLE``.
 
         Examples
         --------
         >>> from ansys.meshing.prime import lucid
         >>> mesh_util = lucid.Mesh(model)
         >>> mesh_util.create_zones_from_labels()
 
@@ -260,55 +263,35 @@
                         elif face not in all_topo and face in part.get_face_zonelets():
                             part.add_zonelets_to_zone(
                                 zonelets=[face],
                                 zone_id=self._model.get_zone_by_name(zone_name=zone_name),
                             )
 
     def merge_parts(self, parts_expression: str = "*", new_name: str = "merged_part"):
-        """Merges given parts into one.
+        """Merge multiple parts into a single part.
 
         Parameters
         ----------
-        parts_expression : str
-            Expression of parts to be merged.
-        new_name : str
-            New part name for the merged part.
+        parts_expression : str, optional
+            Expression of the parts to merge. The default is ``"*"``.
+        new_name : str, optional
+            Name of the new part that is created from the merged parts.
+            The default is ``"merged_part"``.
 
         """
         part_ids = []
         for part in self._model.parts:
             if check_name_pattern(parts_expression, part.get_name()):
                 part_ids.append(part.id)
 
         self._model.merge_parts(
             part_ids=part_ids,
             params=prime.MergePartsParams(self._model, merged_part_suggested_name=new_name),
         )
 
-    def delete_topology(self, parts_expression: str = "*", delete_edges: bool = True):
-        """Delete topoentities of part.
-
-        Parameters
-        ----------
-        parts_expression : str
-            Expression of parts whose topology needs to be deleted.
-        delete_edges : bool
-            Check whether to delete the edges or not.
-
-        """
-        for part in self._model.parts:
-            if check_name_pattern(parts_expression, part.get_name()):
-                part.delete_topo_entities(
-                    prime.DeleteTopoEntitiesParams(
-                        self._model, delete_geom_zonelets=True, delete_mesh_zonelets=False
-                    )
-                )
-                if delete_edges:
-                    part.delete_zonelets(part.get_edge_zonelets())
-
     def __surface_mesh_on_active_sf(self, generate_quads: bool, scope: SurfaceScope):
         part_ids = scope.get_parts(self._model)
         for part_id in part_ids:
             topofaces = scope.get_topo_faces(self._model, part_id)
             surfer = prime.Surfer(self._model)
             params = prime.SurferParams(
                 self._model,
@@ -413,42 +396,39 @@
     def surface_mesh(
         self,
         min_size: float = None,
         max_size: float = None,
         generate_quads: bool = False,
         scope: SurfaceScope = SurfaceScope(),
     ):
-        """Generate Surface mesh on the given scope.
+        """Generate a surface mesh on a scope.
 
-        This method generates surface mesh on the given scope.
-        The method is used to generate constant or variable size surface mesh.
-        The method supports generating quad dominant or triangular elements.
+        This method is used to generate a surface mesh of a constant or variable
+        size. It supports generating quad dominant or triangular elements.
 
-        If min size and max size are provided, variable size mesh is generated
-        between min size and max size by applying sizes based on curvature.
+        If minimum and maximum sizes are provided, a variable size mesh is generated
+        between the minimum size and maximum size by applying sizes based on curvature.
 
-        If either of min size or max size is provided, constant size mesh
-        will be generated with the provided size.
+        If only the minimum size or maximum size is provided, a constant size mesh
+        is generated with the provided size.
 
-        If neither of min size or max size is provided, global max setting is used to
-        generate a constant size mesh.
+        If neither minimum size or maximum size is provided, the global maximum setting
+        is used to generate a constant size mesh.
 
         Parameters
         ----------
-        min_size : float
-            Minimum edge length of the mesh.
-
-        max_size : float
-            Maximum edge length of the mesh.
-
-        generate_quads : bool
-            Generate quad dominant mesh or all triangular mesh.
-
+        min_size : float, optional
+            Minimum edge length of the mesh. The default is ``None``.
+        max_size : float, optional
+            Maximum edge length of the mesh. The default is ``None``.
+        generate_quads : bool, optional
+            Whether to generate a quad dominant mesh. The default is
+            ``False``, in which case a triangular mesh is generated.
         scope : SurfaceScope
-            Scope for generating surface mesh.
+            Scope for generating the surface mesh.
 
         """
         if min_size == None and max_size == None:
             global_sizing = self._model.get_global_sizing_params()
             self._logger.warning(
                 "Min and Max size not provided. Using max global size "
                 + str(global_sizing.max)
@@ -477,28 +457,24 @@
 
     def create_constant_size_control(
         self,
         control_name: str = "size_control",
         size: float = 1.0,
         scope: SurfaceScope = SurfaceScope(),
     ):
-        """Generate constant size control on the given scope.
-
-        This method generates constant size control on the given scope.
+        """Generate constant size control on a scope.
 
         Parameters
         ----------
         control_name : str
             Name of the control.
-
-        size : float
-            Constant edge length of the mesh.
-
+        size : float, optional
+            Constant edge length of the mesh. The default is ``1.0``.
         scope : SurfaceScope
-            Scope for creating size control.
+            Scope for creating the size control.
 
         """
         global_sizes = self._model.get_global_sizing_params()
         if global_sizes.max < size:
             global_sizes.max = size
         if global_sizes.min > size or global_sizes.min <= 0:
             global_sizes.min = size
@@ -515,31 +491,26 @@
     def create_curvature_size_control(
         self,
         control_name: str = "size_control",
         min: float = 1.0,
         max: float = 2.0,
         scope: SurfaceScope = SurfaceScope(),
     ):
-        """Generate curvature size control on the given scope.
-
-        This method generates curvature size control on the given scope.
+        """Generate a curvature size control on a scope.
 
         Parameters
         ----------
-        control_name : str
-            Name of the control.
-
-        min : float
-            Min edge length of the mesh.
-
+        control_name : str, optional
+            Name of the control. The default is ``"size_control"``.
+        min : float, optional
+            Minimum edge length of the mesh. The default is ``1.0``.
         max : float
-            Max edge length of the mesh.
-
+            Maximum edge length of the mesh. The default is ``2.0``.
         scope : SurfaceScope
-            Scope for creating size control.
+            Scope for creating the size control.
 
         """
         global_sizes = self._model.get_global_sizing_params()
         if max < min:
             t = max
             max = min
             min = t
@@ -559,30 +530,27 @@
 
     def surface_mesh_with_size_controls(
         self,
         size_control_names: str = "*",
         generate_quads: bool = False,
         scope: SurfaceScope = SurfaceScope(),
     ):
-        """Generate Surface mesh on the given scope with the given size controls.
+        """Generate a surface mesh on a scope using the given size controls.
 
-        This method generates surface mesh on the given scope.
-        The method is used to generate surface mesh using the given size controls.
-        The method supports generating quad dominant or triangular elements.
+        This method supports generating quad dominant or triangular elements.
 
         Parameters
         ----------
-        size_control_names : str
-            Name pattern for the size controls.
-
-        generate_quads : bool
-            Generate quad dominant mesh or all triangular mesh.
-
+        size_control_names : str, optional
+            Name pattern for the size controls. The default is ``"*"``.
+        generate_quads : bool, optional
+            Whether to generate a quad dominant mesh. The default is
+            ``False``, in which case a triangular mesh is generated.
         scope : SurfaceScope
-            Scope for generating surface mesh.
+            Scope for generating the surface mesh.
 
         """
         sizefield = prime.SizeField(model=self._model)
         s_control_ids = []
         s_controls = self._model.control_data.size_controls
         for control in s_controls:
             if check_name_pattern(size_control_names, control.name):
@@ -600,30 +568,33 @@
     def connect_faces(
         self,
         part_expression: str = "*",
         face_labels: str = "*",
         target_face_labels: str = "*",
         tolerance: float = 0.05,
     ):
-        """Connect face zonelets with given label name pattern within the given tolerance.
+        """Connect face zonelets with a label name pattern within a given tolerance.
 
-        This method is used to connect face zonelets of given label name pattern to the
-        face zonelets given by target face labels within a given tolerance. Connect happens within
-        part. Face zonelets of a part are connected with face zonelets of the same part only.
+        This method connects face zonelets with a label name pattern to
+        face zonelets with target face labels within a given tolerance. The connection
+        happens within the part. Face zonelets of a part are connected with face zonelets
+        of the same part only.
 
         Parameters
         ----------
-        part_expression: str
-            Name pattern of parts used for connecting.
-        face_labels: str
-            Name pattern of face labels used for connecting.
-        target_face_labels: str
-            Name pattern of face labels with which you want to connect.
-        tolerance: float
-            Tolerance used for connection.
+        part_expression : str, optional
+            Name pattern of the parts to use for connecting the face zonelets. The
+            default is ``"*"``.
+        face_labels : str, optional
+            Name pattern of the face labels used for connecting the face zonelets.
+            The default is ``"*"``.
+        target_face_labels : str, optional
+            Name pattern of the face labels to connect. The default is ``"*"``.
+        tolerance: float, optional
+            Tolerance for the connection. The default is ``0.05``.
 
         """
         name_pattern_param = prime.NamePatternParams(self._model)
         connect = prime.Connect(self._model)
         for part in self._model.parts:
             if check_name_pattern(part_expression, part.name):
                 join_faces_source = part.get_face_zonelets_of_label_name_pattern(
@@ -643,51 +614,47 @@
                         part.id,
                         face_zonelet_ids=join_faces_source,
                         with_face_zonelet_ids=join_faces_target,
                         params=prime.JoinParams(self._model, tolerance=tolerance),
                     )
 
     def compute_volumes(self, part_expression: str = "*", create_zones_per_volume: bool = True):
-        """
-        Computes volumes in the parts defined by the part expression
+        """Compute volumes in the parts defined by the part expression.
 
         Parameters
         ----------
-        part_expression : str
-            Expression of parts where topology needs to be deleted.
-
-        create_zones_per_volume : bool
-            Creates volume zones for each volume when True.
+        part_expression : str, optional
+            Expression of the parts where the topology must be deleted.
+            The default is ``"*"``.
+        create_zones_per_volume : bool, optional
+            Whether to create volume zones for each volume. The default
+            is ``True``.
 
         """
         create_zones_type = prime.CreateVolumeZonesType.NONE
         if create_zones_per_volume:
             create_zones_type = prime.CreateVolumeZonesType.PERVOLUME
         params = prime.ComputeVolumesParams(model=self._model, create_zones_type=create_zones_type)
         for part in self._model.parts:
             if check_name_pattern(part_expression, part.name):
                 if len(part.get_topo_faces()) > 0:
                     part.compute_topo_volumes(params=params)
                 else:
                     part.compute_closed_volumes(params=params)
 
     def delete_topology(self, part_expression: str = "*", delete_edges: bool = True):
-        """
-        Deletes topology in the given part.
-
-        This method can be used to delete topology in the parts defined by the part expression.
-        If delete_edges is set to True, edge zonelets will be deleted.
+        """Delete topology in one or more parts.
 
         Parameters
         ----------
-        part_expression : str
-            Expression of parts where topology needs to be deleted.
-
-        delete_edges : bool
-            Edge zonelets are deleted when true.
+        part_expression : str, optional
+            Expression of the parts where the topology must be deleted.
+            The default is ``"*"``.
+        delete_edges : bool, optional
+            Whether to delete edge zonelets. The default is ``True``.
 
         """
         for part in self._model.parts:
             if check_name_pattern(part_expression, part.name):
                 part.delete_topo_entities(
                     prime.DeleteTopoEntitiesParams(
                         model=self._model, delete_geom_zonelets=True, delete_mesh_zonelets=False
@@ -714,24 +681,24 @@
                 model=self._model, create_zone=True, suggested_zone_name=flow_volume_zone_name
             )
             res = part.extract_volumes(face_zonelets=face_zonelets, params=params)
 
     def create_flow_volume(
         self, flow_volume_zone_name: str = "flow_volume", cap_scope: SurfaceScope = SurfaceScope()
     ):
-        """Create flow volume by the given face labels defining the boundary of the volume.
-
-        This method creates flow volumes for the given faces defining the boundary of the volume.
+        """Create flow volume by the face labels defining the boundary of the volume.
 
         Parameters
         ----------
-        flow_volume_zone_name: str
-            Suggested name for the volume zone of the created flow volume.
-        cap_scope: SurfaceScope
-            Scope defining the face zonelets where cap for flow volume needs to be created.
+        flow_volume_zone_name : str, optional
+            Name for the volume zone of the created flow volume. The default is
+            ``"flow_volume"``.
+        cap_scope : SurfaceScope
+            Scope defining the face zonelets where the cap for flow volume must
+            be created.
 
         """
         parts = cap_scope.get_parts(self._model)
         for part in parts:
             caps = self.__create_cap(part, cap_scope.get_face_zonelets(self._model, part))
             if len(caps) > 0:
                 self.__compute_flow_volume(part, caps, flow_volume_zone_name)
@@ -791,45 +758,39 @@
         quadratic: bool = False,
         prism_layers: int = None,
         prism_surface_expression: str = "*",
         prism_volume_expression: str = "*",
         growth_rate: float = 1.2,
         scope: VolumeScope = VolumeScope(),
     ):
-        """Generate Volume mesh on the model.
-
-        This method can be used to generate volume mesh on the entire model.
-        If prism layers parameter is set, prism layers are generated.
+        """Generate a volume mesh on the model.
 
         Parameters
         ----------
         volume_fill_type : prime.VolumeFillType
-            Type of volume elements to be generated.
-
-        quadratic : bool
-            Option to generate quadratic mesh. It is not supported with parallel meshing.
-            It is only supported with pure tetrahedral mesh.
-
-        prism_layers : int
-            Number of prism layers to grow.
-
-        prism_surface_expression : str
-            Facezonelets or topofaces from which prisms are grown.
-            Default is to grow from all surfaces.
-
-        prism_volume_expression : str
-            Volumes or topovolumes into which prisms are grown.
-            The expression evaluates to zone names and volumes
-            or topovolumes are queried based on zones evaluated.
-
-        growth_rate : float
-            Prism growth rate.
-
+            Type of volume elements to generate.
+        quadratic : bool, optional
+            Whether to generate a quadratic mesh. The default is ``False``.
+            A quadratic mesh is not supported with parallel meshing.
+            It is only supported with a pure tetrahedral mesh.
+        prism_layers : int, optional
+            Number of prism layers to grow. The default is ``None``.
+            If a value for prism layers is specified, prism layers are generated.
+        prism_surface_expression : str, optional
+            Face zones or TopoFaces to grow prisms from. The default is ``"*"``,
+            in which case prisms are grown from all surfaces.
+        prism_volume_expression : str, optional
+            Volumes or TopoVolumes to grow prisms in.
+            The default is ``"*"``. This expression evaluates
+            to zone names and volumes, or TopoVolumes are queried
+            based on the zones evaluated.
+        growth_rate : float, optional
+            Prism growth rate. The default is ``1.2``.
         scope : VolumeScope
-            Scope of volumes to be meshed.
+            Scope of volumes to mesh.
 
         """
         automesh_params = prime.AutoMeshParams(model=self._model)
         automesh_params.volume_fill_type = volume_fill_type
         if quadratic:
             automesh_params.tet = prime.TetParams(self._model, True)
         automesh = prime.AutoMesh(self._model)
@@ -999,17 +960,15 @@
                 )
                 const_size_control.set_scope(scope)
                 geodesic_global_size_controls.append(const_size_control)
 
         return min_size, max_size
 
     def __is_size_field_type_geodesic(self, controls: List[prime.SizeControl]):
-        """
-        Checks if the size field type is geodesic.
-        """
+        """Check if the size field type is geodesic."""
         geodesic = True
         geodesic_types = ["Curvature", "Soft"]
         self._logger.info("Size controls: " + str([control.name for control in controls]))
         for control in controls:
             result = control.get_summary(prime.SizeControlSummaryParams(self._model))
             message = str(result.message)
             ctrl_type = message.split("Type : ")[1]
@@ -1020,28 +979,24 @@
                 self._logger.info("Note: VOLUMETRIC method used.")
                 return geodesic
         return geodesic
 
     def __compute_size_field(
         self, size_controls: List[prime.SizeControl], field: prime.SizeField
     ) -> int:
-        """
-        Helper method to compute size field.
-        """
+        """Compute size field using the helper method."""
         self._model.delete_volumetric_size_fields(self._model.get_volumetric_size_fields())
         result = field.compute_volumetric(
             [size_control.id for size_control in size_controls],
             prime.VolumetricSizeFieldComputeParams(model=self._model, enable_multi_threading=False),
         )
         return result.size_field_id
 
     def __remesh_after_wrap(self, part: prime.Part):
-        """
-        Surface mesh after wrapping.
-        """
+        """Surface mesh after wrapping."""
         surfer = prime.Surfer(self._model)
         feature_edges = part.get_edge_zonelets_of_label_name_pattern(
             label_name_pattern="___wrapper_feature_path___",
             name_pattern_params=prime.NamePatternParams(model=self._model),
         )
         surf_params = surfer.initialize_surfer_params_for_wrapper()
         surf_params.size_field_type = prime.SizeFieldType.VOLUMETRIC
@@ -1059,16 +1014,17 @@
         min_size: float,
         max_size: float,
         growth_rate: float,
         geodesic_global_size_controls: List,
         scope: str,
     ):
         """
-        Creates contact prevention controls for all parts.
-        Proximity size control created for remeshing.
+        Create contact prevention controls for all parts.
+
+        A proximity size control is created for remeshing.
         """
         all_parts_labels = len(self._model.parts)
         all_parts_labels += sum([len(part.get_labels()) for part in self._model.parts])
         if contact_prevention_size < min_size:
             prime.PrimeRuntimeError("Contact_prevention_size is less than min_size.")
             return
         self._logger.info(
@@ -1344,125 +1300,95 @@
         size_fields: List[prime.SizeField] = None,
         wrap_size_controls: List[prime.SizeControl] = None,
         remesh_size_controls: List[prime.SizeControl] = None,
         feature_recovery_params: List[prime.FeatureRecoveryParams] = None,
         contact_prevention_params: List[prime.ContactPreventionParams] = None,
         leak_prevention_params: List[prime.LeakPreventionParams] = None,
     ):
-        """Wrap and remesh input.
+        """Wrap and remesh the input.
 
-        Default behaviour is to perform an external wrap of all parts in the model
-        using curvature sizing and extracting features.
-        The wrap is then remeshed to give a surface mesh for the extracted region.
+        The default behavior is to perform an external wrap of all parts in the model
+        using curvature sizing and extracting features. The wrap is then remeshed
+        to provide a surface mesh for the extracted region.
 
-        Geodesic sizing is used if only soft and curvature controls are set.
-        If contact prevention size is set and geodesic sizing is available then contact detection
-        is used globally.
+        Geodesic sizing is used only if soft and curvature controls are set.
+        If contact prevention size is set and geodesic sizing is available, contact
+        detection is used globally.
 
-        If min_size and max_size is provided, variable size mesh is generated
-        between min_size and max_size by applying sizes based on curvature.
+        If minimum and maximum sizes are provided, variable size mesh is generated
+        between the minimum size and maximum size by applying sizes based on curvature.
 
-        If either of min_size or max_size is provided, constant size mesh
-        will be generated with the provided size.
-
-        If neither of min_size or max_size is provided, global min and max settings are used to
-        generate a variable size mesh based on curvature.
+        If either minimum size or maximum size is provided, constant size mesh
+        is generated with the provided size.
 
+        If neither minimum size or maximum size is provided, global minimum and
+        maximum settings are used to generate a variable size mesh based on curvature.
 
         Parameters
         ----------
-        input_parts : str
-            Parts to be wrapped.
-            Default = "*"
-
+        min_size : float, optional
+            Minimum edge length of the mesh. The default is ``None``.
+        max_size : float, optional
+            Maximum edge length of the mesh. The default is ``None``.
+        growth_rate : float, optional
+            Growth rate. The default is ``1.2``.
+        elements_per_gap : float, optional
+            Global proximity size control elements per gap with self proximity.
+            The default is ``None``.
+        normal_angle : float, optional
+            Global curvature size control normal angle. The default is ``18.0``.
+        input_parts : str, optional
+            Parts to wrap. The default is ``"*"``.
         input_labels : str
-            Labels to be wrapped.
-            Default = "*"
-
-        keep_inputs : bool
-            Retain inputs.
-            Default = False
-
+            Labels to wrap. The default is ``"*"``.
+        keep_inputs : bool, optional
+            Whether to retain inputs. The default is ``False``.
         region_extract : prime.WrapRegion
-            Set region to wrap.
-            Default = prime.WrapRegion.EXTERNAL
-
+            Region to wrap. The default is ``prime.WrapRegion.EXTERNAL``.
         material_point : List[float], optional
-            Material point needed if region extraction method set to material point.
-
-        min_size: float, optional
-            Minimum edge length of the mesh.
-
-        max_size: float, optional
-            Maximum edge length of the mesh.
-
-        growth_rate : float
-            Default = 1.2
-
-        elements_per_gap : float, optional
-            Global proximity size control elements per gap with self proximity.
-
-        normal_angle : float
-            Global curvature size control normal angle.
-            Default = 18.0
-
-        create_intersection_loops: bool
-            Create intersection loops between all parts.
-            Default = False
-
-        use_existing_features: bool
-            Maintain existing features on parts.
-            Default = False
-
-        extract_features: bool
-            Extract feature edges using feature angle.
-            Default = True
-
-        feature_angle: float
-            Angle used to extract features.
-            Default = 40.0
-
-        enable_feature_octree_refinement: bool
-            Apply refinement to feature edges during wrap.
-            Default = True
-
-        contact_prevention_size: float, optional
+            Material point if the region extraction method is set to
+            material point. The default is ``None``.
+        extract_features : bool, optional
+            Whether to extract feature edges using the feature angle. The
+            default is ``True``.
+        create_intersection_loops : bool, optional
+            Whether to create intersection loops between all parts.
+            The default is ``False``.
+        use_existing_features : bool, optional
+            Whether to maintain existing features on parts. The
+            default is ``False``.
+        enable_feature_octree_refinement: bool, optional
+            Whether to apply refinement to feature edges during the wrap.
+            The default is ``True``.
+        feature_angle : float, optional
+            Angle to use for extracting features. The default is ``40.0``.
+        contact_prevention_size : float, optional
             Global proximity size controls between all parts.
-
-        number_of_threads: int, optional
-
-        remesh_postwrap : bool
-            Remesh wrap.
-            Default = True
-
-        recompute_remesh_sizes : bool
-            Recompute sizes from global controls using the wrap surface.
-            Default = False
-
-        use_existing_size_fields : bool
-            Use precomputed size fields.
-            Default = False
-
+            The default is ``None``.
+        number_of_threads : int, optional
+            Number of threads. The default is ``None``.
+        remesh_postwrap : bool, optional
+            Whether to remesh the wrap. The default is ``True``.
+        recompute_remesh_sizes : bool, optional
+            Whether to recompute sizes from global controls using
+            the wrap surface. The default is ``False``.
+        use_existing_size_fields : bool, optional
+            Whether to use precomputed size fields. The default is ``False``.
         size_fields : List[prime.SizeField], optional
-            Set size fields to use.
-
+            List of size fields to use. The default is ``None``.
         wrap_size_controls : List[prime.SizeControl], optional
-            Set wrap size controls to use.
-
+            List of wrap size controls to use. The default is ``None``.
         remesh_size_controls : List[prime.SizeControl], optional
-            Set remesh size controls to use.
-
+            List of remesh size controls to use. The default is ``None``.
         feature_recovery_params : List[prime.FeatureRecoveryParams], optional
-            Set feature recovery parameters to use.
-
+            List of feature recovery parameters to use. The default is ``None``.
         contact_prevention_params : List[prime.ContactPreventionParams], optional
-            Set contact prevention parameters to use.
-
+            List of contact prevention parameters to use. The default is ``None``.
         leak_prevention_params : List[prime.LeakPreventionParams], optional
-            Set leak prevention parameters to use.
+            List of leak prevention parameters to use.  The default is ``None``.
 
         Returns
         -------
         Wrapped part
                 Returns Part.
 
         Examples
@@ -1495,15 +1421,15 @@
         scope = prime.ScopeDefinition(
             model=self._model,
             part_expression=input_parts,
             label_expression=input_labels,
             entity_type=prime.ScopeEntity.FACEANDEDGEZONELETS,
         )
 
-        # Delete topology and work only only on zonelets for now
+        # Delete topology and work only on zonelets for now
         for part in self._model.parts:
             if len(part.get_topo_faces()) > 0:
                 part.delete_topo_entities(
                     prime.DeleteTopoEntitiesParams(
                         self._model, delete_geom_zonelets=False, delete_mesh_zonelets=True
                     )
                 )
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/lucid/scope.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/lucid/scope.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Module for Lucid Scope for operation on surfaces functionality."""
 from typing import Iterable
 
 from ansys.meshing.prime.autogen.controlstructs import (
     ScopeDefinition,
     ScopeEntity,
     ScopeEvaluationType,
 )
@@ -31,15 +32,15 @@
                 self._entity_expression,
                 str(int(self._evaluation_type)),
                 str(int(self._entity_type)),
             ]
         )
 
     def get_scope_definition(self, model: Model) -> ScopeDefinition:
-        """Gets the scope definition of the scope.
+        """Get the scope definition of the scope.
 
         Parameters
         ----------
         model : Model
             PyPrimeMesh model.
 
         Returns
@@ -76,15 +77,17 @@
 
     def __init__(
         self,
         part_expression: str = "*",
         entity_expression: str = "*",
         scope_evaluation_type: ScopeEvaluationType = ScopeEvaluationType.LABELS,
     ):
-        """Initialize SurfaceScope with the given part expression,
+        """Initialize SurfaceScope.
+
+        Initialize SurfaceScope with the given part expression,
         entity expression and scope evaluation type.
 
         Parameters
         ----------
         part_expression : str
             Part expression to scope parts while evaluating scope.
         entity_expression : str
@@ -98,15 +101,15 @@
             part_expression,
             entity_expression,
             scope_evaluation_type,
             ScopeEntity.FACEZONELETS,
         )
 
     def get_parts(self, model: Model) -> Iterable[int]:
-        """Gets the list of part ids in the scope.
+        """Get the list of part ids in the scope.
 
         Parameters
         ----------
         model : Model
             PyPrimeMesh model.
 
         Returns
@@ -125,15 +128,15 @@
         sel_parts: Iterable[int] = []
         for part in model.parts:
             if check_name_pattern(self._part_expression, part.name):
                 sel_parts.append(part.id)
         return sel_parts
 
     def get_face_zonelets(self, model: Model, part_id: int) -> Iterable[int]:
-        """Gets the list of face zonelets for the given part in the scope.
+        """Get the list of face zonelets for the given part in the scope.
 
         Parameters
         ----------
         model : Model
             PyPrimeMesh model.
         part_id : int
             Id of the part.
@@ -161,15 +164,15 @@
             else:
                 face_zonelets = part.get_face_zonelets_of_zone_name_pattern(
                     self._entity_expression, NamePatternParams(model)
                 )
         return face_zonelets
 
     def get_topo_faces(self, model: Model, part_id: int) -> Iterable[int]:
-        """Gets the list of topofaces for the given part in the scope.
+        """Get the list of topofaces for the given part in the scope.
 
         Parameters
         ----------
         model : Model
             PyPrimeMesh model.
         part_id : int
             Id of the part.
@@ -211,15 +214,17 @@
 
     def __init__(
         self,
         part_expression: str = "*",
         entity_expression: str = "*",
         scope_evaluation_type: ScopeEvaluationType = ScopeEvaluationType.ZONES,
     ):
-        """Initialize VolumeScope with the given part expression, entity expression and scope
+        """Initialize VolumeScope.
+
+        Initialize VolumeScope with the given part expression, entity expression and scope
         evaluation type.
 
         Parameters
         ----------
         part_expression : str
             Part expression to scope parts while evaluating scope.
         entity_expression : str
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/lucid/utils.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/lucid/utils.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/params/primestructs.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/params/primestructs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Module for imports of autogen modules."""
 # isort: off
 from ansys.meshing.prime.autogen.primeconfig import *
 from ansys.meshing.prime.autogen.commontypes import *
 from ansys.meshing.prime.autogen.commonstructs import *
 
 # isort: on
 from ansys.meshing.prime.autogen.automeshstructs import *
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/relaxed_json/__init__.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/relaxed_json/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,47 +26,48 @@
     allow_nan=True,
     cls=None,
     separators=None,
     default=None,
     sort_keys=False,
     **kw,
 ):
-    """Serialize ``obj`` to a JSON formatted ``str``.
+    """Serialize an object to a JSON-formatted string.
 
-    If ``skipkeys`` is true then ``dict`` keys that are not basic types
-    (``str``, ``int``, ``float``, ``bool``, ``None``) will be skipped
+    If ``skipkeys`` is ``True``, ``dict`` keys that are not basic types
+    (``str``, ``int``, ``float``, ``bool``, and ``None``) are skipped
     instead of raising a ``TypeError``.
 
-    If ``ensure_ascii`` is false, then the return value can contain non-ASCII
-    characters if they appear in strings contained in ``obj``. Otherwise, all
+    If ``ensure_ascii`` is ``False``, the return value can contain non-ASCII
+    characters if they appear in strings contained in the object. Otherwise, all
     such characters are escaped in JSON strings.
 
-    If ``check_circular`` is false, then the circular reference check
-    for container types will be skipped and a circular reference will
-    result in an ``RecursionError`` (or worse).
+    If ``check_circular`` is ``False``, the circular reference check
+    for container types is skipped and a circular reference
+    results in an ``RecursionError`` (or worse).
 
-    If ``allow_nan`` is false, then it will be a ``ValueError`` to
-    serialize out of range ``float`` values (``nan``, ``inf``, ``-inf``) in
+    If ``allow_nan`` is ``False``, it is a ``ValueError`` to
+    serialize out-of-range float values (``nan``, ``inf``, and ``-inf``) in
     strict compliance of the JSON specification, instead of using the
-    JavaScript equivalents (``NaN``, ``Infinity``, ``-Infinity``).
+    JavaScript equivalents (``NaN``, ``Infinity``, and ``-Infinity``).
 
     If specified, ``separators`` should be an ``(item_separator, key_separator)``
-    tuple.  The default is ``(', ', ': ')`` if *indent* is ``None`` and
-    ``(',', ': ')`` otherwise.  To get the most compact JSON representation,
+    tuple. The default is ``(', ', ': ')`` if *indent* is ``None`` and
+    ``(',', ': ')`` otherwise. To get the most compact JSON representation,
     you should specify ``(',', ':')`` to eliminate whitespace.
 
     ``default(obj)`` is a function that should return a serializable version
-    of obj or raise TypeError. The default simply raises TypeError.
+    of the object or raise a ``TypeError``. The default simply raises a
+    ``TypeError``.
 
-    If *sort_keys* is true (default: ``False``), then the output of
-    dictionaries will be sorted by key.
+    If ``sort_keys`` is ``True`` rather than the default of ``False``, the
+    output of the dictionaries are sorted by key.
 
-    To use a custom ``JSONEncoder`` subclass (e.g. one that overrides the
+    To use a custom ``JSONEncoder`` subclass (one that overrides the
     ``.default()`` method to serialize additional types), specify it with
-    the ``cls`` kwarg; otherwise ``JSONEncoder`` is used.
+    the ``cls`` kwarg. Otherwise ``JSONEncoder`` is used.
 
     """
     # cached encoder
     if (
         not skipkeys
         and ensure_ascii
         and check_circular
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/src/ansys/meshing/prime/relaxed_json/encoder.py` & `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/relaxed_json/encoder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-'''Implementation of JSOnEncoder that can handle byte arrays
-'''
+"""Implementation of JSOnEncoder that can handle byte arrays."""
 import re
 
 import numpy as np
 
 ESCAPE = re.compile(r'[\x00-\x1f\\"\b\f\n\r\t]')
 ESCAPE_ASCII = re.compile(r'([\\"]|[^\ -~])')
 HAS_UTF8 = re.compile(b'[\x80-\xff]')
@@ -58,44 +57,44 @@
     elif np.issubdtype(current_dtype, np.float64):
         return np.float64
     else:
         raise ValueError(f'Unsupported dtype {current_dtype}for ' f'numpy array optimizaation')
 
 
 def _check_if_byteorder_needs_to_change(dtype_: np.dtype):
-    '''Check if we need to change the byteorder of a numpy array
+    """Check if we need to change the byteorder of a numpy array.
 
     The wire format for numpy arrays is always in bigendian to ensure
     cross-platform compatibility. Hence, this check ensures that we switch the
     dtype of an ndarray only when the existing dtype does not have a byteorder
     defined or if the defined byteorder is little-endian.
-    '''
+    """
     import sys
 
     if dtype_.byteorder == '<' or dtype_.byteorder == '|':
         return True
     if dtype_.byteorder == '=' and sys.byteorder == 'little':
         return True
     return False
 
 
 def py_encode_basestring(s):
-    """Return a bytearray JSON representation of a Python string"""
+    """Return a bytearray JSON representation of a Python string."""
 
     def replace(match):
         return ESCAPE_DCT[match.group(0)]
 
     return str('"' + ESCAPE.sub(replace, s) + '"').encode('utf-8')
 
 
 encode_basestring = py_encode_basestring
 
 
 def py_encode_basestring_ascii(s):
-    """Return an ASCII-only bytearray JSON representation of a Python string"""
+    """Return an ASCII-only bytearray JSON representation of a Python string."""
 
     def replace(match):
         s = match.group(0)
         try:
             return ESCAPE_DCT[s]
         except KeyError:
             n = ord(s)
@@ -112,63 +111,95 @@
     return str('"' + ESCAPE_ASCII.sub(replace, s) + '"').encode('utf-8')
 
 
 encode_basestring_ascii = py_encode_basestring_ascii
 
 
 class JSONEncoder:
+    """Class to encode Object to JSON format.
+
+    Parameters
+    ----------
+    skipkeys : bool, optional
+        Skip keys, by default False.
+    ensure_ascii : bool, optional
+        Ensure that we use ASCII characters, by default True.
+    check_circular : bool, optional
+        Check circular loops, by default True.
+    allow_nan : bool, optional
+        Allow not number values, by default True.
+    sort_keys : bool, optional
+        Order the keys, by default False.
+    separators : Any, optional
+        String separators, by default None.
+    default : Any, optional
+        Default error message, by default None.
+    """
+
     item_separator = b','
     key_separator = b':'
 
     def __init__(
         self,
         *,
         skipkeys=False,
         ensure_ascii=True,
         check_circular=True,
         allow_nan=True,
         sort_keys=False,
         separators=None,
         default=None,
     ):
-        '''Constructor of JSON Encoder'''
+        """Initialize of JSON Encoder."""
         self.skipkeys = skipkeys
         self.ensure_ascii = ensure_ascii
         self.check_circular = check_circular
         self.allow_nan = allow_nan
         self.sort_keys = sort_keys
         if separators is not None:
             self.item_separator, self.key_separator = separators
         if default is not None:
             self.default = default
 
     def default(self, obj):
+        """Raise default error.
+
+        Parameters
+        ----------
+        obj : Any
+            Object that is not serializable.
+
+        Raises
+        ------
+        TypeError
+            Raise the error with the proper type
+        """
         raise TypeError(f'Object of type {type(obj)} is not JSON serializable')
 
     def encode(self, obj):
-        '''Return a bytearray containing JSON representation of
-        Python Data structure, with the vector extension
-        '''
+        """Return a bytearray containing JSON.
+
+        Return a bytearray containing JSON representation of Python Data
+        structure, with the vector extension
+        """
         # This is for extremely simple cases and benchmarks.
         if isinstance(obj, str):
             if self.ensure_ascii:
                 return encode_basestring_ascii(obj)
             else:
                 return encode_basestring(obj)
 
         chunks = self.iterencode(obj)
         if not isinstance(chunks, (list, tuple)):
             chunks = list(chunks)
 
         return b''.join(chunks)
 
     def iterencode(self, obj):
-        '''Encode the given object and yield the bytearray representation
-        as available
-        '''
+        """Encode the given object and yield the bytearray representationas available."""
         if self.check_circular:
             markers = {}
         else:
             markers = None
         if self.ensure_ascii:
             _encoder = encode_basestring_ascii
         else:
```

### Comparing `ansys_meshing_prime-0.4.0.dev8/PKG-INFO` & `ansys_meshing_prime-0.4.0.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-meshing-prime
-Version: 0.4.0.dev8
+Version: 0.4.0.dev9
 Summary: PyPrimeMesh is a Python client to Ansys Prime Server, which delivers core Ansys meshing technology.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -14,29 +14,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ansys-api-meshing-prime==0.1.1
 Requires-Dist: numpy>=1.14.0
 Requires-Dist: appdirs>=1.4.0
 Requires-Dist: importlib-metadata>=4.0,<5; python_version<='3.8'
 Requires-Dist: pyvista>=0.32.0 ; extra == "all"
-Requires-Dist: ansys-sphinx-theme==0.9.8 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
 Requires-Dist: jupyter-sphinx==0.4.0 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
-Requires-Dist: Sphinx==6.2.0 ; extra == "doc"
-Requires-Dist: pyvista==0.38.6 ; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints==1.23.0 ; extra == "doc"
+Requires-Dist: Sphinx==7.0.1 ; extra == "doc"
+Requires-Dist: pyvista==0.39.1 ; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints==1.23.3 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxemoji==0.2.0 ; extra == "doc"
 Requires-Dist: pyvista>=0.32.0 ; extra == "graphics"
-Requires-Dist: pytest==7.3.1 ; extra == "tests"
-Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
+Requires-Dist: pytest==7.4.0 ; extra == "tests"
+Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
 Requires-Dist: pytest-pyvista==0.1.8 ; extra == "tests"
-Requires-Dist: pyvista[trame]==0.38.6 ; extra == "tests"
+Requires-Dist: pyvista[trame]==0.40.0 ; extra == "tests"
 Project-URL: Documentation, https://prime.docs.pyansys.com
 Project-URL: Source, https://github.com/ansys/pyprimemesh
 Provides-Extra: all
 Provides-Extra: doc
 Provides-Extra: graphics
 Provides-Extra: tests
 
@@ -50,16 +50,16 @@
 ## Overview
 
 PyPrimeMesh is a Python client to Ansys Prime Server, which
 delivers core Ansys meshing technology.
 
 ## Documentation and Issues
 
-For information on PyPrimeMesh, refer to the latest [documentation](
-https://prime.docs.pyansys.com).
+For information on PyPrimeMesh, refer to the [documentation](
+https://prime.docs.pyansys.com) for the latest stable version.
 
 For queries related to PyPrimeMesh, post on the [PyPrimeMesh Discussions](
 https://github.com/ansys/pyprimemesh/discussions) page. 
 
 For bugs or enhancement requests, post an issue on the [PyPrimeMesh Issues](
 https://github.com/ansys/pyprimemesh/issues) page. 
 
@@ -117,9 +117,9 @@
 ## License and Acknowledgments
 
 PyPrimeMesh is licensed under the MIT license.
 
 PyPrimeMesh makes no commercial claim over Ansys whatsoever. This library extends the functionality of
 Ansys Prime Server by adding a Python interface without changing the core behavior or license
 of the original software. The use of Ansys Prime Server requires a legally licensed copy of Ansys
-2023 or later.
+2023 R1 or later.
```

