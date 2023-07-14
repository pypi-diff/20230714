# Comparing `tmp/ansys_meshing_prime-0.4.0.dev9.tar.gz` & `tmp/ansys_meshing_prime-0.5.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_meshing_prime-0.4.0.dev9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_meshing_prime-0.5.0.dev2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_meshing_prime-0.4.0.dev9.tar` & `ansys_meshing_prime-0.5.0.dev2.tar`

### file list

```diff
@@ -1,119 +1,120 @@
--rw-r--r--   0        0        0     1090 2023-07-11 22:39:33.441578 ansys_meshing_prime-0.4.0.dev9/LICENSE
--rw-r--r--   0        0        0     3062 2023-07-11 22:39:33.441578 ansys_meshing_prime-0.4.0.dev9/README.md
--rw-r--r--   0        0        0     2366 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/pyproject.toml
--rw-r--r--   0        0        0     6032 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/__init__.py
--rw-r--r--   0        0        0     2650 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/automesh.py
--rw-r--r--   0        0        0    59522 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/automeshstructs.py
--rw-r--r--   0        0        0     6111 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py
--rw-r--r--   0        0        0     3847 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/collapsetool.py
--rw-r--r--   0        0        0    14701 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/collapsetoolstructs.py
--rw-r--r--   0        0        0    15524 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/commonstructs.py
--rw-r--r--   0        0        0     3875 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/commontypes.py
--rw-r--r--   0        0        0     9883 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/connect.py
--rw-r--r--   0        0        0    39669 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/connectstructs.py
--rw-r--r--   0        0        0    10456 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/controldata.py
--rw-r--r--   0        0        0    55335 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/controlstructs.py
--rw-r--r--   0        0        0      714 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/coreobject.py
--rw-r--r--   0        0        0     3427 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/deletetool.py
--rw-r--r--   0        0        0    13990 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/deletetoolstructs.py
--rw-r--r--   0        0        0     5573 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/featureextraction.py
--rw-r--r--   0        0        0    33896 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/featureextractionstructs.py
--rw-r--r--   0        0        0    24627 2023-07-11 22:39:33.525583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/fileio.py
--rw-r--r--   0        0        0   112910 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/fileiostructs.py
--rw-r--r--   0        0        0    50117 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/igastructs.py
--rw-r--r--   0        0        0     4093 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/materialpointmanager.py
--rw-r--r--   0        0        0    16296 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py
--rw-r--r--   0        0        0     4858 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/meshinfo.py
--rw-r--r--   0        0        0    60035 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/meshinfostructs.py
--rw-r--r--   0        0        0    16491 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/model.py
--rw-r--r--   0        0        0    27227 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/modelstructs.py
--rw-r--r--   0        0        0     3793 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/morpher.py
--rw-r--r--   0        0        0     7831 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/morpherbcsstructs.py
--rw-r--r--   0        0        0    24059 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/morpherstructs.py
--rw-r--r--   0        0        0    58131 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/part.py
--rw-r--r--   0        0        0   167481 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/partstructs.py
--rw-r--r--   0        0        0     7502 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/periodiccontrol.py
--rw-r--r--   0        0        0    13315 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py
--rw-r--r--   0        0        0    28641 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/primeconfig.py
--rw-r--r--   0        0        0     5727 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/prismcontrol.py
--rw-r--r--   0        0        0    14563 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/prismcontrolstructs.py
--rw-r--r--   0        0        0     7237 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/scaffolder.py
--rw-r--r--   0        0        0    29265 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/scaffolderstructs.py
--rw-r--r--   0        0        0    18382 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/sizecontrol.py
--rw-r--r--   0        0        0    52720 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/sizecontrolstructs.py
--rw-r--r--   0        0        0     2790 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/sizefield.py
--rw-r--r--   0        0        0    18893 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/sizefieldstructs.py
--rw-r--r--   0        0        0     4241 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/splittoolstructs.py
--rw-r--r--   0        0        0    19710 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surfacesearch.py
--rw-r--r--   0        0        0   117867 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surfacesearchstructs.py
--rw-r--r--   0        0        0    22036 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surfaceutilities.py
--rw-r--r--   0        0        0   144388 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py
--rw-r--r--   0        0        0     7182 2023-07-11 22:39:33.529583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surfer.py
--rw-r--r--   0        0        0    44962 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surferstructs.py
--rw-r--r--   0        0        0     4448 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/thinvolumecontrol.py
--rw-r--r--   0        0        0     4250 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/thinvolumecontrolstructs.py
--rw-r--r--   0        0        0     8477 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/topodata.py
--rw-r--r--   0        0        0     2646 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/topoutilities.py
--rw-r--r--   0        0        0    13167 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/topoutilitystructs.py
--rw-r--r--   0        0        0     2960 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/transform.py
--rw-r--r--   0        0        0     8727 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/transformstructs.py
--rw-r--r--   0        0        0     5980 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumecontrol.py
--rw-r--r--   0        0        0     6259 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumecontrolstructs.py
--rw-r--r--   0        0        0     4893 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumemeshtool.py
--rw-r--r--   0        0        0    29508 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py
--rw-r--r--   0        0        0     2761 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumesearch.py
--rw-r--r--   0        0        0    25492 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumesearchstructs.py
--rw-r--r--   0        0        0     4886 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumesweeper.py
--rw-r--r--   0        0        0    25535 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumesweeperstructs.py
--rw-r--r--   0        0        0     5426 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/wrapper.py
--rw-r--r--   0        0        0    10816 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/wrappercontrol.py
--rw-r--r--   0        0        0    61895 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/wrapperstructs.py
--rw-r--r--   0        0        0    13896 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/controldata.py
--rw-r--r--   0        0        0    17050 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/fileio.py
--rw-r--r--   0        0        0    11033 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/model.py
--rw-r--r--   0        0        0     4181 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/part.py
--rw-r--r--   0        0        0     2287 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/periodiccontrol.py
--rw-r--r--   0        0        0     2208 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/sizecontrol.py
--rw-r--r--   0        0        0     4069 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/surfaceutilities.py
--rw-r--r--   0        0        0     4664 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/surfer.py
--rw-r--r--   0        0        0     2309 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/volumecontrol.py
--rw-r--r--   0        0        0     3064 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/volumesweeper.py
--rw-r--r--   0        0        0     5981 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/wrapper.py
--rw-r--r--   0        0        0     2115 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/wrappercontrol.py
--rw-r--r--   0        0        0      817 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/examples/__init__.py
--rw-r--r--   0        0        0     4566 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/examples/download_utilities.py
--rw-r--r--   0        0        0    31534 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/examples/examples.py
--rw-r--r--   0        0        0     1514 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/examples/unit_test_examples.py
--rw-r--r--   0        0        0       59 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/__init__.py
--rw-r--r--   0        0        0    41937 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/graphics.py
--rw-r--r--   0        0        0     2234 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/bin.png
--rw-r--r--   0        0        0     1708 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/invert_visibility.png
--rw-r--r--   0        0        0     2510 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/parts.png
--rw-r--r--   0        0        0     1297 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/selectioninfo.png
--rw-r--r--   0        0        0     2440 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/show_edges.png
--rw-r--r--   0        0        0      203 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/show_ruler.png
--rw-r--r--   0        0        0     1547 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/surface_body.png
--rw-r--r--   0        0        0     1612 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/trame_gui.py
--rw-r--r--   0        0        0     5393 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/client.py
--rw-r--r--   0        0        0      626 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/comm_manager.py
--rw-r--r--   0        0        0     1881 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/communicator.py
--rw-r--r--   0        0        0     4664 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/config.py
--rw-r--r--   0        0        0     3080 2023-07-11 22:39:33.533583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/defaults.py
--rw-r--r--   0        0        0    36123 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/error_handling.py
--rw-r--r--   0        0        0     8285 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/grpc_communicator.py
--rw-r--r--   0        0        0      652 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/grpc_utils.py
--rw-r--r--   0        0        0     2319 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/json_utils.py
--rw-r--r--   0        0        0     8044 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/launcher.py
--rw-r--r--   0        0        0     2084 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/logger.py
--rw-r--r--   0        0        0     2815 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/prime_communicator.py
--rw-r--r--   0        0        0    11476 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/utils.py
--rw-r--r--   0        0        0      143 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/lucid/__init__.py
--rw-r--r--   0        0        0    69132 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/lucid/mesh_util.py
--rw-r--r--   0        0        0     7532 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/lucid/scope.py
--rw-r--r--   0        0        0     1493 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/lucid/utils.py
--rw-r--r--   0        0        0     2104 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/params/primestructs.py
--rw-r--r--   0        0        0     4369 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/relaxed_json/__init__.py
--rw-r--r--   0        0        0    13490 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/relaxed_json/decoder.py
--rw-r--r--   0        0        0    13168 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/relaxed_json/encoder.py
--rw-r--r--   0        0        0     3024 2023-07-11 22:39:33.537583 ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/relaxed_json/scanner.py
--rw-r--r--   0        0        0     4990 1970-01-01 00:00:00.000000 ansys_meshing_prime-0.4.0.dev9/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-07-14 20:29:54.808248 ansys_meshing_prime-0.5.0.dev2/LICENSE
+-rw-r--r--   0        0        0     3062 2023-07-14 20:29:54.808248 ansys_meshing_prime-0.5.0.dev2/README.md
+-rw-r--r--   0        0        0     2366 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0     6055 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/__init__.py
+-rw-r--r--   0        0        0     2650 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/automesh.py
+-rw-r--r--   0        0        0    59522 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/automeshstructs.py
+-rw-r--r--   0        0        0     6111 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py
+-rw-r--r--   0        0        0     3847 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/collapsetool.py
+-rw-r--r--   0        0        0    14701 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/collapsetoolstructs.py
+-rw-r--r--   0        0        0    15524 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/commonstructs.py
+-rw-r--r--   0        0        0     3875 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/commontypes.py
+-rw-r--r--   0        0        0     9883 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/connect.py
+-rw-r--r--   0        0        0    50784 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/connectstructs.py
+-rw-r--r--   0        0        0    10456 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/controldata.py
+-rw-r--r--   0        0        0    55335 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/controlstructs.py
+-rw-r--r--   0        0        0      714 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/coreobject.py
+-rw-r--r--   0        0        0     3427 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/deletetool.py
+-rw-r--r--   0        0        0    13990 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/deletetoolstructs.py
+-rw-r--r--   0        0        0     5573 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/featureextraction.py
+-rw-r--r--   0        0        0    33896 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/featureextractionstructs.py
+-rw-r--r--   0        0        0    24627 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/fileio.py
+-rw-r--r--   0        0        0   114169 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/fileiostructs.py
+-rw-r--r--   0        0        0    64474 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/igastructs.py
+-rw-r--r--   0        0        0     4093 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/materialpointmanager.py
+-rw-r--r--   0        0        0    16296 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py
+-rw-r--r--   0        0        0     4858 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/meshinfo.py
+-rw-r--r--   0        0        0    60035 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/meshinfostructs.py
+-rw-r--r--   0        0        0    16491 2023-07-14 20:29:54.900254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/model.py
+-rw-r--r--   0        0        0    27227 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/modelstructs.py
+-rw-r--r--   0        0        0     3793 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/morpher.py
+-rw-r--r--   0        0        0     7831 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/morpherbcsstructs.py
+-rw-r--r--   0        0        0    24059 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/morpherstructs.py
+-rw-r--r--   0        0        0    58189 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/part.py
+-rw-r--r--   0        0        0   167481 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/partstructs.py
+-rw-r--r--   0        0        0     7502 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/periodiccontrol.py
+-rw-r--r--   0        0        0    13315 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py
+-rw-r--r--   0        0        0    28915 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/primeconfig.py
+-rw-r--r--   0        0        0     5727 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/prismcontrol.py
+-rw-r--r--   0        0        0    14563 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/prismcontrolstructs.py
+-rw-r--r--   0        0        0     3773 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/quadtospline.py
+-rw-r--r--   0        0        0     7237 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/scaffolder.py
+-rw-r--r--   0        0        0    29265 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/scaffolderstructs.py
+-rw-r--r--   0        0        0    18382 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/sizecontrol.py
+-rw-r--r--   0        0        0    52720 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/sizecontrolstructs.py
+-rw-r--r--   0        0        0     2790 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/sizefield.py
+-rw-r--r--   0        0        0    18893 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/sizefieldstructs.py
+-rw-r--r--   0        0        0     4241 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/splittoolstructs.py
+-rw-r--r--   0        0        0    19710 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/surfacesearch.py
+-rw-r--r--   0        0        0   117867 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/surfacesearchstructs.py
+-rw-r--r--   0        0        0    22036 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/surfaceutilities.py
+-rw-r--r--   0        0        0   144419 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py
+-rw-r--r--   0        0        0     7182 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/surfer.py
+-rw-r--r--   0        0        0    44962 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/surferstructs.py
+-rw-r--r--   0        0        0     4448 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/thinvolumecontrol.py
+-rw-r--r--   0        0        0     6689 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/thinvolumecontrolstructs.py
+-rw-r--r--   0        0        0     8477 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/topodata.py
+-rw-r--r--   0        0        0     2646 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/topoutilities.py
+-rw-r--r--   0        0        0    13167 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/topoutilitystructs.py
+-rw-r--r--   0        0        0     2960 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/transform.py
+-rw-r--r--   0        0        0     8727 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/transformstructs.py
+-rw-r--r--   0        0        0     5980 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/volumecontrol.py
+-rw-r--r--   0        0        0     6259 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/volumecontrolstructs.py
+-rw-r--r--   0        0        0     4893 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/volumemeshtool.py
+-rw-r--r--   0        0        0    29508 2023-07-14 20:29:54.904254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py
+-rw-r--r--   0        0        0     2761 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/volumesearch.py
+-rw-r--r--   0        0        0    25492 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/volumesearchstructs.py
+-rw-r--r--   0        0        0     4886 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/volumesweeper.py
+-rw-r--r--   0        0        0    25535 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/volumesweeperstructs.py
+-rw-r--r--   0        0        0     5426 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/wrapper.py
+-rw-r--r--   0        0        0    10816 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/wrappercontrol.py
+-rw-r--r--   0        0        0    63122 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/wrapperstructs.py
+-rw-r--r--   0        0        0    13896 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/controldata.py
+-rw-r--r--   0        0        0    17050 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/fileio.py
+-rw-r--r--   0        0        0    11033 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/model.py
+-rw-r--r--   0        0        0     4181 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/part.py
+-rw-r--r--   0        0        0     2287 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/periodiccontrol.py
+-rw-r--r--   0        0        0     2208 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/sizecontrol.py
+-rw-r--r--   0        0        0     4069 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/surfaceutilities.py
+-rw-r--r--   0        0        0     4664 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/surfer.py
+-rw-r--r--   0        0        0     2309 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/volumecontrol.py
+-rw-r--r--   0        0        0     3064 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/volumesweeper.py
+-rw-r--r--   0        0        0     5981 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/wrapper.py
+-rw-r--r--   0        0        0     2115 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/wrappercontrol.py
+-rw-r--r--   0        0        0      949 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/examples/__init__.py
+-rw-r--r--   0        0        0     4566 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/examples/download_utilities.py
+-rw-r--r--   0        0        0    36650 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/examples/examples.py
+-rw-r--r--   0        0        0     1514 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/examples/unit_test_examples.py
+-rw-r--r--   0        0        0       59 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/graphics/__init__.py
+-rw-r--r--   0        0        0    41937 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/graphics/graphics.py
+-rw-r--r--   0        0        0     2234 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/graphics/images/bin.png
+-rw-r--r--   0        0        0     1708 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/graphics/images/invert_visibility.png
+-rw-r--r--   0        0        0     2510 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/graphics/images/parts.png
+-rw-r--r--   0        0        0     1297 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/graphics/images/selectioninfo.png
+-rw-r--r--   0        0        0     2440 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/graphics/images/show_edges.png
+-rw-r--r--   0        0        0      203 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/graphics/images/show_ruler.png
+-rw-r--r--   0        0        0     1547 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/graphics/images/surface_body.png
+-rw-r--r--   0        0        0     1612 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/graphics/trame_gui.py
+-rw-r--r--   0        0        0     5393 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/client.py
+-rw-r--r--   0        0        0      626 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/comm_manager.py
+-rw-r--r--   0        0        0     1881 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/communicator.py
+-rw-r--r--   0        0        0     5045 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/config.py
+-rw-r--r--   0        0        0     3121 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/defaults.py
+-rw-r--r--   0        0        0    36123 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/error_handling.py
+-rw-r--r--   0        0        0     8285 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/grpc_communicator.py
+-rw-r--r--   0        0        0      652 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/grpc_utils.py
+-rw-r--r--   0        0        0     2319 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/json_utils.py
+-rw-r--r--   0        0        0     8044 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/launcher.py
+-rw-r--r--   0        0        0     2380 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/logger.py
+-rw-r--r--   0        0        0     2815 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/prime_communicator.py
+-rw-r--r--   0        0        0    11476 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/utils.py
+-rw-r--r--   0        0        0      143 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/lucid/__init__.py
+-rw-r--r--   0        0        0    69132 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/lucid/mesh_util.py
+-rw-r--r--   0        0        0     7532 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/lucid/scope.py
+-rw-r--r--   0        0        0     1493 2023-07-14 20:29:54.908254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/lucid/utils.py
+-rw-r--r--   0        0        0     2104 2023-07-14 20:29:54.912254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/params/primestructs.py
+-rw-r--r--   0        0        0     4369 2023-07-14 20:29:54.912254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/relaxed_json/__init__.py
+-rw-r--r--   0        0        0    13490 2023-07-14 20:29:54.912254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/relaxed_json/decoder.py
+-rw-r--r--   0        0        0    13168 2023-07-14 20:29:54.912254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/relaxed_json/encoder.py
+-rw-r--r--   0        0        0     3024 2023-07-14 20:29:54.912254 ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/relaxed_json/scanner.py
+-rw-r--r--   0        0        0     4990 1970-01-01 00:00:00.000000 ansys_meshing_prime-0.5.0.dev2/PKG-INFO
```

### Comparing `ansys_meshing_prime-0.4.0.dev9/LICENSE` & `ansys_meshing_prime-0.5.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/README.md` & `ansys_meshing_prime-0.5.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/pyproject.toml` & `ansys_meshing_prime-0.5.0.dev2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-meshing-prime"
-version = "0.4.0.dev9"
+version = "0.5.0.dev2"
 description = "PyPrimeMesh is a Python client to Ansys Prime Server, which delivers core Ansys meshing technology."
 readme = "README.md"
 requires-python = ">=3.8,<4"
 license = {file = "LICENSE"}
 authors = [{name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"}]
 maintainers =  [{name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"}]
 classifiers = [
@@ -39,15 +39,15 @@
   "pyvista[trame]==0.40.0"
 ]
 doc = [
   "ansys-sphinx-theme==0.9.9",
   "jupyter-sphinx==0.4.0",
   "numpydoc==1.5.0",
   "Sphinx==7.0.1",
-  "pyvista==0.39.1",
+  "pyvista==0.40.1",
   "sphinx-autodoc-typehints==1.23.3",
   "sphinx-copybutton==0.5.2",
   "sphinx-gallery==0.13.0",
   "sphinx-notfound-page==0.8.3",
   "sphinxemoji==0.2.0",
 ]
 all = [
```

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/__init__.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 from ansys.meshing.prime.internals.launcher import *
 from ansys.meshing.prime.internals.config import (
     is_optimizing_numpy_arrays,
     enable_optimizing_numpy_arrays,
     disable_optimizing_numpy_arrays,
     numpy_array_optimization_enabled,
     numpy_array_optimization_disabled,
+    enable_log_output,
 )
 
 import ansys.meshing.prime.examples as examples
 import ansys.meshing.prime.lucid as lucid
 
 # Version
 # ------------------------------------------------------------------------------
```

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/automesh.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/automesh.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/automeshstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/automeshstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/collapsetool.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/collapsetool.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/collapsetoolstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/collapsetoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/commonstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/commonstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/commontypes.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/commontypes.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/connect.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/connect.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/connectstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/connectstructs.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,14 +32,285 @@
     NONE = 0
     """No action to be taken for matched mesh."""
     TRIMONESIDE = 3
     """Delete matched faces on one side and merge matched nodes at middle locations (works only within a single part)."""
     TRIMTWOSIDES = 4
     """Delete matched faces on both sides and merge matched nodes at middle locations (works only within a single part)."""
 
+class OverlapPairs(CoreObject):
+    """Provides ids of a pair of overlapping face zonelets.
+    """
+    _default_params = {}
+
+    def __initialize(
+            self,
+            zone_id0: int,
+            zone_id1: int):
+        self._zone_id0 = zone_id0
+        self._zone_id1 = zone_id1
+
+    def __init__(
+            self,
+            model: CommunicationManager=None,
+            zone_id0: int = None,
+            zone_id1: int = None,
+            json_data : dict = None,
+             **kwargs):
+        """Initializes the OverlapPairs.
+
+        Parameters
+        ----------
+        model: Model
+            Model to create a OverlapPairs object with default parameters.
+        zone_id0: int, optional
+            Id of one overlapping face zonelet.
+        zone_id1: int, optional
+            Id of other overlapping face zonelet.
+        json_data: dict, optional
+            JSON dictionary to create a OverlapPairs object with provided parameters.
+
+        Examples
+        --------
+        >>> overlap_pairs = prime.OverlapPairs(model = model)
+        """
+        if json_data:
+            self.__initialize(
+                json_data["zoneId0"] if "zoneId0" in json_data else None,
+                json_data["zoneId1"] if "zoneId1" in json_data else None)
+        else:
+            all_field_specified = all(arg is not None for arg in [zone_id0, zone_id1])
+            if all_field_specified:
+                self.__initialize(
+                    zone_id0,
+                    zone_id1)
+            else:
+                if model is None:
+                    raise ValueError("Invalid assignment. Either pass model or specify all properties")
+                else:
+                    param_json = model._communicator.initialize_params(model, "OverlapPairs")
+                    json_data = param_json["OverlapPairs"] if "OverlapPairs" in param_json else {}
+                    self.__initialize(
+                        zone_id0 if zone_id0 is not None else ( OverlapPairs._default_params["zone_id0"] if "zone_id0" in OverlapPairs._default_params else (json_data["zoneId0"] if "zoneId0" in json_data else None)),
+                        zone_id1 if zone_id1 is not None else ( OverlapPairs._default_params["zone_id1"] if "zone_id1" in OverlapPairs._default_params else (json_data["zoneId1"] if "zoneId1" in json_data else None)))
+        self._custom_params = kwargs
+        if model is not None:
+            [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
+        [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
+        lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
+        self._freeze()
+
+    @staticmethod
+    def set_default(
+            zone_id0: int = None,
+            zone_id1: int = None):
+        """Set the default values of OverlapPairs.
+
+        Parameters
+        ----------
+        zone_id0: int, optional
+            Id of one overlapping face zonelet.
+        zone_id1: int, optional
+            Id of other overlapping face zonelet.
+        """
+        args = locals()
+        [OverlapPairs._default_params.update({ key: value }) for key, value in args.items() if value is not None]
+
+    @staticmethod
+    def print_default():
+        """Print the default values of OverlapPairs.
+
+        Examples
+        --------
+        >>> OverlapPairs.print_default()
+        """
+        message = ""
+        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in OverlapPairs._default_params.items())
+        print(message)
+
+    def _jsonify(self) -> Dict[str, Any]:
+        json_data = {}
+        if self._zone_id0 is not None:
+            json_data["zoneId0"] = self._zone_id0
+        if self._zone_id1 is not None:
+            json_data["zoneId1"] = self._zone_id1
+        [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
+        return json_data
+
+    def __str__(self) -> str:
+        message = "zone_id0 :  %s\nzone_id1 :  %s" % (self._zone_id0, self._zone_id1)
+        message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
+        return message
+
+    @property
+    def zone_id0(self) -> int:
+        """Id of one overlapping face zonelet.
+        """
+        return self._zone_id0
+
+    @zone_id0.setter
+    def zone_id0(self, value: int):
+        self._zone_id0 = value
+
+    @property
+    def zone_id1(self) -> int:
+        """Id of other overlapping face zonelet.
+        """
+        return self._zone_id1
+
+    @zone_id1.setter
+    def zone_id1(self, value: int):
+        self._zone_id1 = value
+
+class OverlapSearchResults(CoreObject):
+    """Provides ids of a pair of overlapping face zonelets.
+    """
+    _default_params = {}
+
+    def __initialize(
+            self,
+            n_pairs: int,
+            overlap_pairs: List[OverlapPairs],
+            error_code: ErrorCode):
+        self._n_pairs = n_pairs
+        self._overlap_pairs = overlap_pairs
+        self._error_code = ErrorCode(error_code)
+
+    def __init__(
+            self,
+            model: CommunicationManager=None,
+            n_pairs: int = None,
+            overlap_pairs: List[OverlapPairs] = None,
+            error_code: ErrorCode = None,
+            json_data : dict = None,
+             **kwargs):
+        """Initializes the OverlapSearchResults.
+
+        Parameters
+        ----------
+        model: Model
+            Model to create a OverlapSearchResults object with default parameters.
+        n_pairs: int, optional
+            Number of pairs.
+        overlap_pairs: List[OverlapPairs], optional
+            Ids corresponding to pairs of overlapping face zonelets.
+        error_code: ErrorCode, optional
+            Error Code associated with failure of operation.
+        json_data: dict, optional
+            JSON dictionary to create a OverlapSearchResults object with provided parameters.
+
+        Examples
+        --------
+        >>> overlap_search_results = prime.OverlapSearchResults(model = model)
+        """
+        if json_data:
+            self.__initialize(
+                json_data["nPairs"] if "nPairs" in json_data else None,
+                [OverlapPairs(model = model, json_data = data) for data in json_data["overlapPairs"]] if "overlapPairs" in json_data else None,
+                ErrorCode(json_data["errorCode"] if "errorCode" in json_data else None))
+        else:
+            all_field_specified = all(arg is not None for arg in [n_pairs, overlap_pairs, error_code])
+            if all_field_specified:
+                self.__initialize(
+                    n_pairs,
+                    overlap_pairs,
+                    error_code)
+            else:
+                if model is None:
+                    raise ValueError("Invalid assignment. Either pass model or specify all properties")
+                else:
+                    param_json = model._communicator.initialize_params(model, "OverlapSearchResults")
+                    json_data = param_json["OverlapSearchResults"] if "OverlapSearchResults" in param_json else {}
+                    self.__initialize(
+                        n_pairs if n_pairs is not None else ( OverlapSearchResults._default_params["n_pairs"] if "n_pairs" in OverlapSearchResults._default_params else (json_data["nPairs"] if "nPairs" in json_data else None)),
+                        overlap_pairs if overlap_pairs is not None else ( OverlapSearchResults._default_params["overlap_pairs"] if "overlap_pairs" in OverlapSearchResults._default_params else [OverlapPairs(model = model, json_data = data) for data in (json_data["overlapPairs"] if "overlapPairs" in json_data else None)]),
+                        error_code if error_code is not None else ( OverlapSearchResults._default_params["error_code"] if "error_code" in OverlapSearchResults._default_params else ErrorCode(json_data["errorCode"] if "errorCode" in json_data else None)))
+        self._custom_params = kwargs
+        if model is not None:
+            [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
+        [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
+        lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
+        self._freeze()
+
+    @staticmethod
+    def set_default(
+            n_pairs: int = None,
+            overlap_pairs: List[OverlapPairs] = None,
+            error_code: ErrorCode = None):
+        """Set the default values of OverlapSearchResults.
+
+        Parameters
+        ----------
+        n_pairs: int, optional
+            Number of pairs.
+        overlap_pairs: List[OverlapPairs], optional
+            Ids corresponding to pairs of overlapping face zonelets.
+        error_code: ErrorCode, optional
+            Error Code associated with failure of operation.
+        """
+        args = locals()
+        [OverlapSearchResults._default_params.update({ key: value }) for key, value in args.items() if value is not None]
+
+    @staticmethod
+    def print_default():
+        """Print the default values of OverlapSearchResults.
+
+        Examples
+        --------
+        >>> OverlapSearchResults.print_default()
+        """
+        message = ""
+        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in OverlapSearchResults._default_params.items())
+        print(message)
+
+    def _jsonify(self) -> Dict[str, Any]:
+        json_data = {}
+        if self._n_pairs is not None:
+            json_data["nPairs"] = self._n_pairs
+        if self._overlap_pairs is not None:
+            json_data["overlapPairs"] = [data._jsonify() for data in self._overlap_pairs]
+        if self._error_code is not None:
+            json_data["errorCode"] = self._error_code
+        [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
+        return json_data
+
+    def __str__(self) -> str:
+        message = "n_pairs :  %s\noverlap_pairs :  %s\nerror_code :  %s" % (self._n_pairs, '[' + ''.join('\n' + str(data) for data in self._overlap_pairs) + ']', self._error_code)
+        message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
+        return message
+
+    @property
+    def n_pairs(self) -> int:
+        """Number of pairs.
+        """
+        return self._n_pairs
+
+    @n_pairs.setter
+    def n_pairs(self, value: int):
+        self._n_pairs = value
+
+    @property
+    def overlap_pairs(self) -> List[OverlapPairs]:
+        """Ids corresponding to pairs of overlapping face zonelets.
+        """
+        return self._overlap_pairs
+
+    @overlap_pairs.setter
+    def overlap_pairs(self, value: List[OverlapPairs]):
+        self._overlap_pairs = value
+
+    @property
+    def error_code(self) -> ErrorCode:
+        """Error Code associated with failure of operation.
+        """
+        return self._error_code
+
+    @error_code.setter
+    def error_code(self, value: ErrorCode):
+        self._error_code = value
+
 class ConnectResults(CoreObject):
     """Results associated with the connection operations.
     """
     _default_params = {}
 
     def __initialize(
             self,
```

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/controldata.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/controldata.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/controlstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/controlstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/coreobject.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/coreobject.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/deletetool.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/deletetool.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/deletetoolstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/deletetoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/featureextraction.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/featureextraction.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/featureextractionstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/featureextractionstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/fileio.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/fileio.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/fileiostructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/fileiostructs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1261,36 +1261,39 @@
     """Parameters to control CAD import settings.
     """
     _default_params = {}
 
     def __initialize(
             self,
             append: bool,
+            ansys_release: str,
             cad_reader_route: CadReaderRoute,
             part_creation_type: PartCreationType,
             geometry_transfer: bool,
             length_unit: LengthUnit,
             refacet: bool,
             cad_refaceting_params: CadRefacetingParams,
             stitch_tolerance: float,
             cad_update_parameters: Dict[str, Union[str, int, float, bool]]):
         self._append = append
+        self._ansys_release = ansys_release
         self._cad_reader_route = CadReaderRoute(cad_reader_route)
         self._part_creation_type = PartCreationType(part_creation_type)
         self._geometry_transfer = geometry_transfer
         self._length_unit = LengthUnit(length_unit)
         self._refacet = refacet
         self._cad_refaceting_params = cad_refaceting_params
         self._stitch_tolerance = stitch_tolerance
         self._cad_update_parameters = cad_update_parameters
 
     def __init__(
             self,
             model: CommunicationManager=None,
             append: bool = None,
+            ansys_release: str = None,
             cad_reader_route: CadReaderRoute = None,
             part_creation_type: PartCreationType = None,
             geometry_transfer: bool = None,
             length_unit: LengthUnit = None,
             refacet: bool = None,
             cad_refaceting_params: CadRefacetingParams = None,
             stitch_tolerance: float = None,
@@ -1301,14 +1304,16 @@
 
         Parameters
         ----------
         model: Model
             Model to create a ImportCadParams object with default parameters.
         append: bool, optional
             Append imported CAD into existing model when true.
+        ansys_release: str, optional
+            Configures the Ansys release to be used for loading CAD data through non Native route.
         cad_reader_route: CadReaderRoute, optional
             Specify the available CAD reader routes. The available CAD reader routes are ProgramControlled, Native, WorkBench, SpaceClaim.
         part_creation_type: PartCreationType, optional
             Create a part per CAD Model, Assembly, Part, Body.
         geometry_transfer: bool, optional
             Option to enable transfer of geometry data (NURBS).
         length_unit: LengthUnit, optional
@@ -1327,27 +1332,29 @@
         Examples
         --------
         >>> import_cad_params = prime.ImportCadParams(model = model)
         """
         if json_data:
             self.__initialize(
                 json_data["append"] if "append" in json_data else None,
+                json_data["ansysRelease"] if "ansysRelease" in json_data else None,
                 CadReaderRoute(json_data["cadReaderRoute"] if "cadReaderRoute" in json_data else None),
                 PartCreationType(json_data["partCreationType"] if "partCreationType" in json_data else None),
                 json_data["geometryTransfer"] if "geometryTransfer" in json_data else None,
                 LengthUnit(json_data["lengthUnit"] if "lengthUnit" in json_data else None),
                 json_data["refacet"] if "refacet" in json_data else None,
                 CadRefacetingParams(model = model, json_data = json_data["cadRefacetingParams"] if "cadRefacetingParams" in json_data else None),
                 json_data["stitchTolerance"] if "stitchTolerance" in json_data else None,
                 json_data["cadUpdateParameters"] if "cadUpdateParameters" in json_data else None)
         else:
-            all_field_specified = all(arg is not None for arg in [append, cad_reader_route, part_creation_type, geometry_transfer, length_unit, refacet, cad_refaceting_params, stitch_tolerance, cad_update_parameters])
+            all_field_specified = all(arg is not None for arg in [append, ansys_release, cad_reader_route, part_creation_type, geometry_transfer, length_unit, refacet, cad_refaceting_params, stitch_tolerance, cad_update_parameters])
             if all_field_specified:
                 self.__initialize(
                     append,
+                    ansys_release,
                     cad_reader_route,
                     part_creation_type,
                     geometry_transfer,
                     length_unit,
                     refacet,
                     cad_refaceting_params,
                     stitch_tolerance,
@@ -1356,14 +1363,15 @@
                 if model is None:
                     raise ValueError("Invalid assignment. Either pass model or specify all properties")
                 else:
                     param_json = model._communicator.initialize_params(model, "ImportCadParams")
                     json_data = param_json["ImportCadParams"] if "ImportCadParams" in param_json else {}
                     self.__initialize(
                         append if append is not None else ( ImportCadParams._default_params["append"] if "append" in ImportCadParams._default_params else (json_data["append"] if "append" in json_data else None)),
+                        ansys_release if ansys_release is not None else ( ImportCadParams._default_params["ansys_release"] if "ansys_release" in ImportCadParams._default_params else (json_data["ansysRelease"] if "ansysRelease" in json_data else None)),
                         cad_reader_route if cad_reader_route is not None else ( ImportCadParams._default_params["cad_reader_route"] if "cad_reader_route" in ImportCadParams._default_params else CadReaderRoute(json_data["cadReaderRoute"] if "cadReaderRoute" in json_data else None)),
                         part_creation_type if part_creation_type is not None else ( ImportCadParams._default_params["part_creation_type"] if "part_creation_type" in ImportCadParams._default_params else PartCreationType(json_data["partCreationType"] if "partCreationType" in json_data else None)),
                         geometry_transfer if geometry_transfer is not None else ( ImportCadParams._default_params["geometry_transfer"] if "geometry_transfer" in ImportCadParams._default_params else (json_data["geometryTransfer"] if "geometryTransfer" in json_data else None)),
                         length_unit if length_unit is not None else ( ImportCadParams._default_params["length_unit"] if "length_unit" in ImportCadParams._default_params else LengthUnit(json_data["lengthUnit"] if "lengthUnit" in json_data else None)),
                         refacet if refacet is not None else ( ImportCadParams._default_params["refacet"] if "refacet" in ImportCadParams._default_params else (json_data["refacet"] if "refacet" in json_data else None)),
                         cad_refaceting_params if cad_refaceting_params is not None else ( ImportCadParams._default_params["cad_refaceting_params"] if "cad_refaceting_params" in ImportCadParams._default_params else CadRefacetingParams(model = model, json_data = (json_data["cadRefacetingParams"] if "cadRefacetingParams" in json_data else None))),
                         stitch_tolerance if stitch_tolerance is not None else ( ImportCadParams._default_params["stitch_tolerance"] if "stitch_tolerance" in ImportCadParams._default_params else (json_data["stitchTolerance"] if "stitchTolerance" in json_data else None)),
@@ -1374,28 +1382,31 @@
         [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
         lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
         self._freeze()
 
     @staticmethod
     def set_default(
             append: bool = None,
+            ansys_release: str = None,
             cad_reader_route: CadReaderRoute = None,
             part_creation_type: PartCreationType = None,
             geometry_transfer: bool = None,
             length_unit: LengthUnit = None,
             refacet: bool = None,
             cad_refaceting_params: CadRefacetingParams = None,
             stitch_tolerance: float = None,
             cad_update_parameters: Dict[str, Union[str, int, float, bool]] = None):
         """Set the default values of ImportCadParams.
 
         Parameters
         ----------
         append: bool, optional
             Append imported CAD into existing model when true.
+        ansys_release: str, optional
+            Configures the Ansys release to be used for loading CAD data through non Native route.
         cad_reader_route: CadReaderRoute, optional
             Specify the available CAD reader routes. The available CAD reader routes are ProgramControlled, Native, WorkBench, SpaceClaim.
         part_creation_type: PartCreationType, optional
             Create a part per CAD Model, Assembly, Part, Body.
         geometry_transfer: bool, optional
             Option to enable transfer of geometry data (NURBS).
         length_unit: LengthUnit, optional
@@ -1424,14 +1435,16 @@
         message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in ImportCadParams._default_params.items())
         print(message)
 
     def _jsonify(self) -> Dict[str, Any]:
         json_data = {}
         if self._append is not None:
             json_data["append"] = self._append
+        if self._ansys_release is not None:
+            json_data["ansysRelease"] = self._ansys_release
         if self._cad_reader_route is not None:
             json_data["cadReaderRoute"] = self._cad_reader_route
         if self._part_creation_type is not None:
             json_data["partCreationType"] = self._part_creation_type
         if self._geometry_transfer is not None:
             json_data["geometryTransfer"] = self._geometry_transfer
         if self._length_unit is not None:
@@ -1444,29 +1457,39 @@
             json_data["stitchTolerance"] = self._stitch_tolerance
         if self._cad_update_parameters is not None:
             json_data["cadUpdateParameters"] = self._cad_update_parameters
         [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
         return json_data
 
     def __str__(self) -> str:
-        message = "append :  %s\ncad_reader_route :  %s\npart_creation_type :  %s\ngeometry_transfer :  %s\nlength_unit :  %s\nrefacet :  %s\ncad_refaceting_params :  %s\nstitch_tolerance :  %s\ncad_update_parameters :  %s" % (self._append, self._cad_reader_route, self._part_creation_type, self._geometry_transfer, self._length_unit, self._refacet, '{ ' + str(self._cad_refaceting_params) + ' }', self._stitch_tolerance, self._cad_update_parameters)
+        message = "append :  %s\nansys_release :  %s\ncad_reader_route :  %s\npart_creation_type :  %s\ngeometry_transfer :  %s\nlength_unit :  %s\nrefacet :  %s\ncad_refaceting_params :  %s\nstitch_tolerance :  %s\ncad_update_parameters :  %s" % (self._append, self._ansys_release, self._cad_reader_route, self._part_creation_type, self._geometry_transfer, self._length_unit, self._refacet, '{ ' + str(self._cad_refaceting_params) + ' }', self._stitch_tolerance, self._cad_update_parameters)
         message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
         return message
 
     @property
     def append(self) -> bool:
         """Append imported CAD into existing model when true.
         """
         return self._append
 
     @append.setter
     def append(self, value: bool):
         self._append = value
 
     @property
+    def ansys_release(self) -> str:
+        """Configures the Ansys release to be used for loading CAD data through non Native route.
+        """
+        return self._ansys_release
+
+    @ansys_release.setter
+    def ansys_release(self, value: str):
+        self._ansys_release = value
+
+    @property
     def cad_reader_route(self) -> CadReaderRoute:
         """Specify the available CAD reader routes. The available CAD reader routes are ProgramControlled, Native, WorkBench, SpaceClaim.
         """
         return self._cad_reader_route
 
     @cad_reader_route.setter
     def cad_reader_route(self, value: CadReaderRoute):
```

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/materialpointmanager.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/materialpointmanager.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/meshinfo.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/meshinfo.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/meshinfostructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/meshinfostructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/model.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/model.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/modelstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/modelstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/morpher.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/morpher.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/morpherbcsstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/morpherbcsstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/morpherstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/morpherstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/part.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/part.py`

 * *Files 1% similar despite different names*

```diff
@@ -1436,35 +1436,35 @@
         args = {}
         command_name = "PrimeMesh::Part/GetSplines"
         self._model._print_logs_before_command("get_splines", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("get_splines")
         return result
 
-    def get_uspline_surface(self) -> IGAUSplineSurf:
+    def get_unstructured_spline_surface(self) -> IGAUSplineSurf:
         """ Gets the unstructured surface spline for the part.
 
 
         Returns
         -------
         IGAUSplineSurf
             Returns the surface spline structure.
 
 
         Examples
         --------
         >>> from ansys.meshing.prime import Part
-        >>> spline = part.GetUSplineSurface()
+        >>> spline = part.GetUnstructuredSplineSurface()
 
         """
         args = {}
-        command_name = "PrimeMesh::Part/GetUSplineSurface"
-        self._model._print_logs_before_command("get_uspline_surface", args)
+        command_name = "PrimeMesh::Part/GetUnstructuredSplineSurface"
+        self._model._print_logs_before_command("get_unstructured_spline_surface", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("get_uspline_surface", IGAUSplineSurf(model = self._model, json_data = result))
+        self._model._print_logs_after_command("get_unstructured_spline_surface", IGAUSplineSurf(model = self._model, json_data = result))
         return IGAUSplineSurf(model = self._model, json_data = result)
 
     def get_summary(self, params : PartSummaryParams) -> PartSummaryResults:
         """ Get the part summary.
 
         Provides the part summary for the given parameters.
```

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/partstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/partstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/periodiccontrol.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/periodiccontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/primeconfig.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/primeconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -574,14 +574,18 @@
     """Invalid number of layers provided for thin volume control."""
     THINVOLUMECONTROLTOPOLOGYNOTSUPPORTED = 12108
     """Thin volume mesh controls not supported for part with topology data."""
     THINVOLUMECONTROLINVALIDVOLUMESCOPE = 12109
     """Invalid volume scope provided for thin volume control."""
     THINVOLUMECONTROLINVALIDCONTROL = 12110
     """Same face scope is set as target for multiple thin volume controls."""
+    THINVOLUMECONTROLSAMESOURCEFORMORETHANTWOCONTROL = 12111
+    """Same face scope is set as source for more than two thin volume controls."""
+    THINVOLUMEMESHNOTSUPPORTEDWITHFACEBASEDDATABASE = 12112
+    """Thin volume mesh is not supported with face based database."""
     MICROSTRUCTUREINVALIDELEMENTTYPE = 13000
     """Invalid input provided. Invalid Element Type."""
 
 class WarningCode(enum.IntEnum):
     """Warning codes associated with the PyPrimeMesh operation.
     """
     NOWARNING = 0
```

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/prismcontrol.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/prismcontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/prismcontrolstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/prismcontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/scaffolder.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/scaffolder.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/scaffolderstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/scaffolderstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/sizecontrol.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/sizecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/sizecontrolstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/sizecontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/sizefield.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/sizefield.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/sizefieldstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/sizefieldstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/splittoolstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/splittoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surfacesearch.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/surfacesearch.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surfacesearchstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/surfacesearchstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surfaceutilities.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/surfaceutilities.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,15 +289,15 @@
         return self._error_code
 
     @error_code.setter
     def error_code(self, value: ErrorCode):
         self._error_code = value
 
 class CopyZoneletsParams(CoreObject):
-    """Parameters to copy zonelets.
+    """Parameters to copy zonelets. This is for internal use only.
     """
     _default_params = {}
 
     def __initialize(
             self):
         pass
```

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surfer.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/surfer.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/surferstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/surferstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/thinvolumecontrol.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/thinvolumecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/topodata.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/topodata.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/topoutilities.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/topoutilities.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/topoutilitystructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/topoutilitystructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/transform.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/transform.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/transformstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/transformstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumecontrol.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/volumecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumecontrolstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/volumecontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumemeshtool.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/volumemeshtool.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumesearch.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/volumesearch.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumesearchstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/volumesearchstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumesweeper.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/volumesweeper.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/volumesweeperstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/volumesweeperstructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/wrapper.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/wrapper.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/wrappercontrol.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/wrappercontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/autogen/wrapperstructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/autogen/wrapperstructs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1005,29 +1005,32 @@
 
     def __initialize(
             self,
             target: ScopeDefinition,
             gap_size: float,
             material_point_name: str,
             suggested_part_name: str,
-            number_of_threads: int):
+            number_of_threads: int,
+            merge_to_geom: bool):
         self._target = target
         self._gap_size = gap_size
         self._material_point_name = material_point_name
         self._suggested_part_name = suggested_part_name
         self._number_of_threads = number_of_threads
+        self._merge_to_geom = merge_to_geom
 
     def __init__(
             self,
             model: CommunicationManager=None,
             target: ScopeDefinition = None,
             gap_size: float = None,
             material_point_name: str = None,
             suggested_part_name: str = None,
             number_of_threads: int = None,
+            merge_to_geom: bool = None,
             json_data : dict = None,
              **kwargs):
         """Initializes the WrapperCloseGapsParams.
 
         Parameters
         ----------
         model: Model
@@ -1038,77 +1041,85 @@
             Maximum gap size to be closed.
         material_point_name: str, optional
             Material point name near the gaps to be closed.
         suggested_part_name: str, optional
             Suggested part name for created patching surfaces.
         number_of_threads: int, optional
             Number of threads for multithreading.
+        merge_to_geom: bool, optional
+            Merges the created gap closure elements to the nearest input geometry.
         json_data: dict, optional
             JSON dictionary to create a WrapperCloseGapsParams object with provided parameters.
 
         Examples
         --------
         >>> wrapper_close_gaps_params = prime.WrapperCloseGapsParams(model = model)
         """
         if json_data:
             self.__initialize(
                 ScopeDefinition(model = model, json_data = json_data["target"] if "target" in json_data else None),
                 json_data["gapSize"] if "gapSize" in json_data else None,
                 json_data["materialPointName"] if "materialPointName" in json_data else None,
                 json_data["suggestedPartName"] if "suggestedPartName" in json_data else None,
-                json_data["numberOfThreads"] if "numberOfThreads" in json_data else None)
+                json_data["numberOfThreads"] if "numberOfThreads" in json_data else None,
+                json_data["mergeToGeom"] if "mergeToGeom" in json_data else None)
         else:
-            all_field_specified = all(arg is not None for arg in [target, gap_size, material_point_name, suggested_part_name, number_of_threads])
+            all_field_specified = all(arg is not None for arg in [target, gap_size, material_point_name, suggested_part_name, number_of_threads, merge_to_geom])
             if all_field_specified:
                 self.__initialize(
                     target,
                     gap_size,
                     material_point_name,
                     suggested_part_name,
-                    number_of_threads)
+                    number_of_threads,
+                    merge_to_geom)
             else:
                 if model is None:
                     raise ValueError("Invalid assignment. Either pass model or specify all properties")
                 else:
                     param_json = model._communicator.initialize_params(model, "WrapperCloseGapsParams")
                     json_data = param_json["WrapperCloseGapsParams"] if "WrapperCloseGapsParams" in param_json else {}
                     self.__initialize(
                         target if target is not None else ( WrapperCloseGapsParams._default_params["target"] if "target" in WrapperCloseGapsParams._default_params else ScopeDefinition(model = model, json_data = (json_data["target"] if "target" in json_data else None))),
                         gap_size if gap_size is not None else ( WrapperCloseGapsParams._default_params["gap_size"] if "gap_size" in WrapperCloseGapsParams._default_params else (json_data["gapSize"] if "gapSize" in json_data else None)),
                         material_point_name if material_point_name is not None else ( WrapperCloseGapsParams._default_params["material_point_name"] if "material_point_name" in WrapperCloseGapsParams._default_params else (json_data["materialPointName"] if "materialPointName" in json_data else None)),
                         suggested_part_name if suggested_part_name is not None else ( WrapperCloseGapsParams._default_params["suggested_part_name"] if "suggested_part_name" in WrapperCloseGapsParams._default_params else (json_data["suggestedPartName"] if "suggestedPartName" in json_data else None)),
-                        number_of_threads if number_of_threads is not None else ( WrapperCloseGapsParams._default_params["number_of_threads"] if "number_of_threads" in WrapperCloseGapsParams._default_params else (json_data["numberOfThreads"] if "numberOfThreads" in json_data else None)))
+                        number_of_threads if number_of_threads is not None else ( WrapperCloseGapsParams._default_params["number_of_threads"] if "number_of_threads" in WrapperCloseGapsParams._default_params else (json_data["numberOfThreads"] if "numberOfThreads" in json_data else None)),
+                        merge_to_geom if merge_to_geom is not None else ( WrapperCloseGapsParams._default_params["merge_to_geom"] if "merge_to_geom" in WrapperCloseGapsParams._default_params else (json_data["mergeToGeom"] if "mergeToGeom" in json_data else None)))
         self._custom_params = kwargs
         if model is not None:
             [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
         [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
         lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
         self._freeze()
 
     @staticmethod
     def set_default(
             target: ScopeDefinition = None,
             gap_size: float = None,
             material_point_name: str = None,
             suggested_part_name: str = None,
-            number_of_threads: int = None):
+            number_of_threads: int = None,
+            merge_to_geom: bool = None):
         """Set the default values of WrapperCloseGapsParams.
 
         Parameters
         ----------
         target: ScopeDefinition, optional
             Scope of target face zonelets to patch gaps between scope and target. If empty scope is provided, CloseGaps patch gaps within scope.
         gap_size: float, optional
             Maximum gap size to be closed.
         material_point_name: str, optional
             Material point name near the gaps to be closed.
         suggested_part_name: str, optional
             Suggested part name for created patching surfaces.
         number_of_threads: int, optional
             Number of threads for multithreading.
+        merge_to_geom: bool, optional
+            Merges the created gap closure elements to the nearest input geometry.
         """
         args = locals()
         [WrapperCloseGapsParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
 
     @staticmethod
     def print_default():
         """Print the default values of WrapperCloseGapsParams.
@@ -1129,19 +1140,21 @@
             json_data["gapSize"] = self._gap_size
         if self._material_point_name is not None:
             json_data["materialPointName"] = self._material_point_name
         if self._suggested_part_name is not None:
             json_data["suggestedPartName"] = self._suggested_part_name
         if self._number_of_threads is not None:
             json_data["numberOfThreads"] = self._number_of_threads
+        if self._merge_to_geom is not None:
+            json_data["mergeToGeom"] = self._merge_to_geom
         [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
         return json_data
 
     def __str__(self) -> str:
-        message = "target :  %s\ngap_size :  %s\nmaterial_point_name :  %s\nsuggested_part_name :  %s\nnumber_of_threads :  %s" % ('{ ' + str(self._target) + ' }', self._gap_size, self._material_point_name, self._suggested_part_name, self._number_of_threads)
+        message = "target :  %s\ngap_size :  %s\nmaterial_point_name :  %s\nsuggested_part_name :  %s\nnumber_of_threads :  %s\nmerge_to_geom :  %s" % ('{ ' + str(self._target) + ' }', self._gap_size, self._material_point_name, self._suggested_part_name, self._number_of_threads, self._merge_to_geom)
         message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
         return message
 
     @property
     def target(self) -> ScopeDefinition:
         """Scope of target face zonelets to patch gaps between scope and target. If empty scope is provided, CloseGaps patch gaps within scope.
         """
@@ -1187,14 +1200,24 @@
         """
         return self._number_of_threads
 
     @number_of_threads.setter
     def number_of_threads(self, value: int):
         self._number_of_threads = value
 
+    @property
+    def merge_to_geom(self) -> bool:
+        """Merges the created gap closure elements to the nearest input geometry.
+        """
+        return self._merge_to_geom
+
+    @merge_to_geom.setter
+    def merge_to_geom(self, value: bool):
+        self._merge_to_geom = value
+
 class WrapperCloseGapsResult(CoreObject):
     """Result structure associated with close gaps operation.
     """
     _default_params = {}
 
     def __initialize(
             self,
```

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/controldata.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/controldata.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/fileio.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/fileio.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/model.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/model.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/part.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/part.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/periodiccontrol.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/periodiccontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/sizecontrol.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/sizecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/surfaceutilities.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/surfaceutilities.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/surfer.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/surfer.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/volumecontrol.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/volumecontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/volumesweeper.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/volumesweeper.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/wrapper.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/core/wrappercontrol.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/core/wrappercontrol.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/examples/download_utilities.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/examples/download_utilities.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/examples/examples.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/examples/examples.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,18 @@
     "download_pipe_tee_dsco",
     "download_turbine_blade_cdb",
     "download_pcb_pmdat",
     "download_pcb_scdoc",
     "download_saddle_bracket_fmd",
     "download_saddle_bracket_scdoc",
     "download_saddle_bracket_dsco",
+    "download_f1_rw_drs_stl",
+    "download_f1_rw_enclosure_stl",
+    "download_f1_rw_end_plates_stl",
+    "download_f1_rw_main_plane_stl",
 ]
 
 
 class Examples(Enum):
     """Contains the PyPrimeMesh examples available for download."""
 
     ELBOW_PMDAT = {"filename": "mixing_elbow.pmdat", "git_folder": "mixing_elbow"}
@@ -58,14 +62,18 @@
     DEFORMED_BLADE_DSCO = {"filename": "blade_deformed.dsco", "git_folder": "turbine_blade"}
     TURBINE_BLADE_CDB = {"filename": "blade.cdb", "git_folder": "turbine_blade"}
     PCB_PMDAT = {"filename": "pcb_stacker.pmdat", "git_folder": "pcb"}
     PCB_SCDOC = {"filename": "pcb_stacker.scdoc", "git_folder": "pcb"}
     SADDLE_BRACKET_FMD = {"filename": "saddle_bracket.fmd", "git_folder": "saddle_bracket"}
     SADDLE_BRACKET_SCDOC = {"filename": "saddle_bracket.scdoc", "git_folder": "saddle_bracket"}
     SADDLE_BRACKET_DSCO = {"filename": "saddle_bracket.dsco", "git_folder": "saddle_bracket"}
+    F1_RW_DRS_STL = {"filename": "f1_rw_drs.stl", "git_folder": "f1_rear_wing"}
+    F1_RW_END_PLATES_STL = {"filename": "f1_rw_enclosure.stl", "git_folder": "f1_rear_wing"}
+    F1_RW_ENCLOSURE_STL = {"filename": "f1_rw_end_plates.stl", "git_folder": "f1_rear_wing"}
+    F1_RW_MAIN_PLANE_STL = {"filename": "f1_rw_main_plane.stl", "git_folder": "f1_rear_wing"}
 
 
 _DOWNLOADS = []
 
 
 def get_file(
     example: Examples,
@@ -73,21 +81,21 @@
     force: bool = False,
 ) -> Union[str, os.PathLike]:
     """Download a PyPrimeMesh example file from the GitHub repository.
 
     Parameters
     ----------
     example : Examples
-        Name of the example file to download.
+        Name of the example file to be downloaded.
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -115,19 +123,19 @@
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download the PMDAT file for the mixing elbow example.
 
     Parameters
     ----------
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -151,19 +159,19 @@
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download the FMD file for the mixing elbow example.
 
     Parameters
     ----------
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -188,19 +196,19 @@
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download the SCDOC file for the mixing elbow example.
 
     Parameters
     ----------
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -224,19 +232,19 @@
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download the DSCO file for the mixing elbow example.
 
     Parameters
     ----------
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -260,19 +268,19 @@
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download the FMD file for the bracket scaffold example.
 
     Parameters
     ----------
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -296,19 +304,19 @@
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download the SCDOC file for the bracket scaffold example.
 
     Parameters
     ----------
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -332,19 +340,19 @@
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download the DSCO file for the bracket scaffold example.
 
     Parameters
     ----------
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -368,19 +376,19 @@
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download the PMDAT file for the toy car example.
 
     Parameters
     ----------
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -404,19 +412,19 @@
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download the FMD file for the toy car example.
 
     Parameters
     ----------
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -440,19 +448,19 @@
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download the SCDOC file for the toy car example.
 
     Parameters
     ----------
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -476,19 +484,19 @@
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download the DSCO file for the toy car example.
 
     Parameters
     ----------
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -512,19 +520,19 @@
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download the PMDAT file for the pipe tee example.
 
     Parameters
     ----------
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -548,19 +556,19 @@
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download the FMD file for the pipe tee example.
 
     Parameters
     ----------
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to  download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -584,19 +592,19 @@
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download the SCDOC file for the pipe tee example.
 
     Parameters
     ----------
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -620,19 +628,19 @@
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download the DSCO file for the pipe tee example.
 
     Parameters
     ----------
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -656,19 +664,19 @@
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download the FMD file for the turbine blade example.
 
     Parameters
     ----------
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -692,19 +700,19 @@
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download the SCDOC file for the turbine blade example.
 
     Parameters
     ----------
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -728,19 +736,19 @@
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download the DSCO file for the turbine blade example.
 
     Parameters
     ----------
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -762,19 +770,19 @@
 
 def download_turbine_blade_cdb(
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download the CDB file for the turbine blade example.
 
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -801,19 +809,19 @@
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download the PMDAT file for the PCB example.
 
     Parameters
     ----------
     destination : str, optional
-        Path to download the example file to. The default
+        Path to which you download the example file. The default
         is ``None``, in which case the default path for app data
         is used.
     force : bool, optional
-        Whether to always download the example file. The default is
+        Option to download the example file. The default is
         ``False``, in which case if the example file is cached, it
         is reused.
 
     Returns
     -------
     str
         Local path to the downloaded example file.
@@ -832,29 +840,30 @@
     """
     return get_file(Examples.PCB_PMDAT, destination, force)
 
 
 def download_pcb_scdoc(
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
-    """Download SCDOC file for the pcb example
+    """Download SCDOC file for the pcb example.
 
     Parameters
     ----------
     destination: Optional[str]
         Destination for the file to be downloaded.
-        If nothing is provided, the default path in app data is used
+        If nothing is provided, the default path in app data is used.
     force: bool
+        Option to download the file.
         If true, the file is always downloaded.
-        If false, an existing file in the cache may be re-used.
+        If false, an existing file in the cache may be reused.
 
     Returns
     -------
     str
-        Local path to the downloaded file
+        Local path to the downloaded file.
 
     Examples
     --------
     >>> import ansys.meshing.prime as prime
     >>> import ansys.meshing.prime.examples as prime_examples
     >>> with prime.launch_prime() as session:
     >>>     model = session.model
@@ -872,23 +881,24 @@
 ) -> Union[str, os.PathLike]:
     """Download FMD file for the saddle bracket example
 
     Parameters
     ----------
     destination: Optional[str]
         Destination for the file to be downloaded.
-        If nothing is provided, the default path in app data is used
+        If nothing is provided, the default path in app data is used.
     force: bool
+        Option to download the file.
         If true, the file is always downloaded.
-        If false, an existing file in the cache may be re-used.
+        If false, an existing file in the cache may be reused.
 
     Returns
     -------
     str
-        Local path to the downloaded file
+        Local path to the downloaded file.
 
     Examples
     --------
     >>> import ansys.meshing.prime as prime
     >>> import ansys.meshing.prime.examples as prime_examples
     >>> with prime.launch_prime() as session:
     >>>     model = session.model
@@ -901,29 +911,30 @@
 
     return get_file(Examples.SADDLE_BRACKET_FMD, destination, force)
 
 
 def download_saddle_bracket_scdoc(
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
-    """Download SCDOC file for the saddle bracket example
+    """Download SCDOC file for the saddle bracket example.
 
     Parameters
     ----------
     destination: Optional[str]
         Destination for the file to be downloaded.
-        If nothing is provided, the default path in app data is used
+        If nothing is provided, the default path in app data is used.
     force: bool
+        Option to download the file.
         If true, the file is always downloaded.
-        If false, an existing file in the cache may be re-used.
+        If false, an existing file in the cache may be reused.
 
     Returns
     -------
     str
-        Local path to the downloaded file
+        Local path to the downloaded file.
 
     Examples
     --------
     >>> import ansys.meshing.prime as prime
     >>> import ansys.meshing.prime.examples as prime_examples
     >>> with prime.launch_prime() as session:
     >>>     model = session.model
@@ -935,36 +946,177 @@
     """
     return get_file(Examples.SADDLE_BRACKET_SCDOC, destination, force)
 
 
 def download_saddle_bracket_dsco(
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
-    """Download DSCO file for the saddle bracket example
+    """Download DSCO file for the saddle bracket example.
 
     Parameters
     ----------
     destination: Optional[str]
         Destination for the file to be downloaded.
-        If nothing is provided, the default path in app data is used
+        If nothing is provided, the default path in app data is used.
     force: bool
+        Option to download the file.
         If true, the file is always downloaded.
-        If false, an existing file in the cache may be re-used.
+        If false, an existing file in the cache may be reused.
 
     Returns
     -------
     str
-        Local path to the downloaded file
+        Local path to the downloaded file.
 
     Examples
     --------
     >>> import ansys.meshing.prime as prime
     >>> import ansys.meshing.prime.examples as prime_examples
     >>> with prime.launch_prime() as session:
     >>>     model = session.model
     >>>     saddle_bracket = prime_examples.download_saddle_bracket_dsco()
     >>>     with prime.FileIO(model) as io:
     >>>         _ = io.import_cad(saddle_bracket, params=prime.ImportCADParams(model))
     >>>     print(model)
 
     """
     return get_file(Examples.SADDLE_BRACKET_DSCO, destination, force)
+
+
+def download_f1_rw_drs_stl(
+    destination: Optional[str] = None, force: bool = False
+) -> Union[str, os.PathLike]:
+    """Download STL file for the generic f1 rear wing example.
+
+    Parameters
+    ----------
+    destination: Optional[str]
+        Destination for the file to be downloaded.
+        If nothing is provided, the default path in app data is used.
+    force: bool
+        Option to download the file.
+        If true, the file is always downloaded.
+        If false, an existing file in the cache may be reused.
+
+    Returns
+    -------
+    str
+        Local path to the downloaded file.
+
+    Examples
+    --------
+    >>> import ansys.meshing.prime as prime
+    >>> import ansys.meshing.prime.examples as prime_examples
+    >>> with prime.launch_prime() as session:
+    >>>     model = session.model
+    >>>     f1_rw_drs = prime_examples.download_f1_rw_drs_stl()
+    >>>     with prime.FileIO(model) as io:
+    >>>         _ = io.read_pmdat(pcb, params=prime.FileReadParams(model))
+    >>>     print(model)
+
+    """
+    return get_file(Examples.F1_RW_DRS_STL, destination, force)
+
+
+def download_f1_rw_enclosure_stl(
+    destination: Optional[str] = None, force: bool = False
+) -> Union[str, os.PathLike]:
+    """Download STL file for the generic f1 rear wing example.
+
+    Parameters
+    ----------
+    destination: Optional[str]
+        Destination for the file to be downloaded.
+        If nothing is provided, the default path in app data is used.
+    force: bool
+        Option to download the file.
+        If true, the file is always downloaded.
+        If false, an existing file in the cache may be reused.
+
+    Returns
+    -------
+    str
+        Local path to the downloaded file.
+
+    Examples
+    --------
+    >>> import ansys.meshing.prime as prime
+    >>> import ansys.meshing.prime.examples as prime_examples
+    >>> with prime.launch_prime() as session:
+    >>>     model = session.model
+    >>>     f1_rw_enclosure = prime_examples.download_f1_rw_enclosure_stl()
+    >>>     with prime.FileIO(model) as io:
+    >>>         _ = io.read_pmdat(pcb, params=prime.FileReadParams(model))
+    >>>     print(model)
+
+    """
+    return get_file(Examples.F1_RW_ENCLOSURE_STL, destination, force)
+
+
+def download_f1_rw_end_plates_stl(
+    destination: Optional[str] = None, force: bool = False
+) -> Union[str, os.PathLike]:
+    """Download STL file for the generic f1 rear wing example.
+
+    Parameters
+    ----------
+    destination: Optional[str]
+        Destination for the file to be downloaded.
+        If nothing is provided, the default path in app data is used.
+    force: bool
+        Option to download the file.
+        If true, the file is always downloaded.
+        If false, an existing file in the cache may be reused.
+
+    Returns
+    -------
+    str
+        Local path to the downloaded file.
+
+    Examples
+    --------
+    >>> import ansys.meshing.prime as prime
+    >>> import ansys.meshing.prime.examples as prime_examples
+    >>> with prime.launch_prime() as session:
+    >>>     model = session.model
+    >>>     f1_rw_end_plates = prime_examples.download_f1_rw_end_plates_stl()
+    >>>     with prime.FileIO(model) as io:
+    >>>         _ = io.read_pmdat(pcb, params=prime.FileReadParams(model))
+    >>>     print(model)
+
+    """
+    return get_file(Examples.F1_RW_END_PLATES_STL, destination, force)
+
+
+def download_f1_rw_main_plane_stl(
+    destination: Optional[str] = None, force: bool = False
+) -> Union[str, os.PathLike]:
+    """Download STL file for the generic f1 rear wing example.
+
+    Parameters
+    ----------
+    destination: Optional[str]
+        Destination for the file to be downloaded.
+        If nothing is provided, the default path in app data is used.
+    force: bool
+        Option to download the file.
+        If true, the file is always downloaded.
+        If false, an existing file in the cache may be reused.
+
+    Returns
+    -------
+    str
+        Local path to the downloaded file.
+
+    Examples
+    --------
+    >>> import ansys.meshing.prime as prime
+    >>> import ansys.meshing.prime.examples as prime_examples
+    >>> with prime.launch_prime() as session:
+    >>>     model = session.model
+    >>>     f1_rw_main_plane = prime_examples.download_f1_rw_main_plane_stl()
+    >>>     with prime.FileIO(model) as io:
+    >>>         _ = io.read_pmdat(pcb, params=prime.FileReadParams(model))
+    >>>     print(model)
+
+    """
+    return get_file(Examples.F1_RW_MAIN_PLANE_STL, destination, force)
```

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/examples/unit_test_examples.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/examples/unit_test_examples.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/graphics.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/graphics/graphics.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/bin.png` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/graphics/images/bin.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/invert_visibility.png` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/graphics/images/invert_visibility.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/parts.png` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/graphics/images/parts.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/selectioninfo.png` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/graphics/images/selectioninfo.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/show_edges.png` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/graphics/images/show_edges.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/images/surface_body.png` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/graphics/images/surface_body.png`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/graphics/trame_gui.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/graphics/trame_gui.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/client.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/client.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/comm_manager.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/comm_manager.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/communicator.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/communicator.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/config.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,24 @@
     'is_optimizing_numpy_arrays',
     'numpy_array_optimization_enabled',
     'numpy_array_optimization_disabled',
     'set_using_container',
     'using_container',
     'set_has_pim',
     'has_pim',
+    'enable_log_output',
 ]
 
 __DEFAULT_USE_BINARY = False
 __USING_CONTAINER = False
 __HAS_PIM = False
 __FILE_CHECK = True
 
+from ansys.meshing.prime.internals.logger import PrimeLogger
+
 
 def _optimize_vectors():
     """Get the value of the flag for optimizing vectors."""
     return __DEFAULT_USE_BINARY
 
 
 def _set_optimize_vectors(optimize_vectors: bool):
@@ -186,7 +189,20 @@
     -------
     bool
         Option to check if files exist before reading them.
     """
     global __FILE_CHECK
     __FILE_CHECK = value
     return __FILE_CHECK
+
+
+def enable_log_output(stream=None):
+    """Enable logger output to given stream.
+
+    If stream is not specified, sys.stderr is used.
+
+    Parameters
+    ----------
+    stream: TextIO, optional
+        Stream to output the log output to stream
+    """
+    PrimeLogger().enable_output(stream)
```

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/defaults.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/defaults.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 
 import os
 
 try:
     import appdirs
 
     USER_DATA_PATH = os.getenv(
-        'PYPRIMEMESH_USER_DATA',
-        appdirs.user_data_dir(appname='ansys_meshing_prime', appauthor='Ansys'),
+        'PYPRIMEMESH_USER_DATA', appdirs.user_data_dir(appname='pyprimemesh', appauthor=False)
     )
 except ModuleNotFoundError:
     # If appdirs is not installed, then try with tempfile.
     # NOTE: This only occurs for ADO ARM Test runs
     import tempfile
 
+    USER_NAME = os.getenv('USERNAME', os.getenv('USER', 'pyprimemesh'))
     USER_DATA_PATH = os.getenv(
-        'PYPRIMEMESH_USER_DATA', os.path.join(tempfile.gettempdir(), 'ansys_meshing_prime')
+        'PYPRIMEMESH_USER_DATA', os.path.join(tempfile.gettempdir(), USER_NAME)
     )
 
 if not os.path.exists(USER_DATA_PATH):  # pragma: no cover
     os.makedirs(USER_DATA_PATH)
 
 EXAMPLES_PATH = os.path.join(USER_DATA_PATH, 'examples')
 if not os.path.exists(EXAMPLES_PATH):  # pragma: no cover
```

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/error_handling.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/error_handling.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/grpc_communicator.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/grpc_communicator.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/grpc_utils.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/grpc_utils.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/json_utils.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/json_utils.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/launcher.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/launcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except ModuleNotFoundError:
     pass
 
 __all__ = ['launch_prime', 'launch_server_process']
 
 
 def get_install_locations():
-    supported_versions = ['232']
+    supported_versions = ['241']
     awp_roots = {ver: os.environ.get(f'AWP_ROOT{ver}', '') for ver in supported_versions}
     installed_versions = {
         ver: os.path.join(path, 'meshing', 'Prime')
         for ver, path in awp_roots.items()
         if path and os.path.isdir(path)
     }
     installed_versions = {
```

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/logger.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,42 +29,53 @@
 
     _logger = None
 
     def __init__(self, logger_name: str = "PyPrimeMesh"):
         """Logger initializer."""
         self._logger = logging.getLogger(logger_name)
         self._logger.setLevel(logging.DEBUG)
-        self.formatter = logging.Formatter(
+        self._formatter = logging.Formatter(
             '%(asctime)s \t [%(levelname)s | %(filename)s:%(lineno)s] > %(message)s'
         )
-        # stdout
-        stream_handler = logging.StreamHandler()
-        stream_handler.setFormatter(self.formatter)
-        self._logger.addHandler(stream_handler)
 
     def get_logger(self):
         """Get the logger.
 
         Returns
         -------
         Logger
             Logger.
         """
         return self._logger
 
+    def enable_output(self, stream=None):
+        """Enable logger output to given stream.
+
+        If stream is not specified, sys.stderr is used.
+
+        Parameters
+        ----------
+        stream: TextIO, optional
+            Stream to output the log output to stream
+        """
+        # stdout
+        stream_handler = logging.StreamHandler(stream)
+        stream_handler.setFormatter(self._formatter)
+        self._logger.addHandler(stream_handler)
+
     def add_file_handler(self, logs_dir: str = "./.log"):
         """Save logs to a file in addition to printing them to stdout.
 
         Parameters
         ----------
         logs_dir : str, optional
             Directory of the logs. The default is ``"./.log"``.
         """
         now = datetime.datetime.now()
         if not os.path.isdir(logs_dir):
             os.mkdir(logs_dir)
         file_handler = logging.FileHandler(logs_dir + "/log_" + now.strftime("%Y-%m-%d") + ".log")
-        file_handler.setFormatter(self.formatter)
+        file_handler.setFormatter(self._formatter)
         self._logger.addHandler(file_handler)
 
 
 LOG = PrimeLogger().get_logger()
```

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/prime_communicator.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/prime_communicator.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/internals/utils.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/internals/utils.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/lucid/mesh_util.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/lucid/mesh_util.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/lucid/scope.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/lucid/scope.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/lucid/utils.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/lucid/utils.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/params/primestructs.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/params/primestructs.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/relaxed_json/__init__.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/relaxed_json/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/relaxed_json/decoder.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/relaxed_json/decoder.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/relaxed_json/encoder.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/relaxed_json/encoder.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/src/ansys/meshing/prime/relaxed_json/scanner.py` & `ansys_meshing_prime-0.5.0.dev2/src/ansys/meshing/prime/relaxed_json/scanner.py`

 * *Files identical despite different names*

### Comparing `ansys_meshing_prime-0.4.0.dev9/PKG-INFO` & `ansys_meshing_prime-0.5.0.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-meshing-prime
-Version: 0.4.0.dev9
+Version: 0.5.0.dev2
 Summary: PyPrimeMesh is a Python client to Ansys Prime Server, which delivers core Ansys meshing technology.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 Requires-Dist: appdirs>=1.4.0
 Requires-Dist: importlib-metadata>=4.0,<5; python_version<='3.8'
 Requires-Dist: pyvista>=0.32.0 ; extra == "all"
 Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
 Requires-Dist: jupyter-sphinx==0.4.0 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: Sphinx==7.0.1 ; extra == "doc"
-Requires-Dist: pyvista==0.39.1 ; extra == "doc"
+Requires-Dist: pyvista==0.40.1 ; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints==1.23.3 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxemoji==0.2.0 ; extra == "doc"
 Requires-Dist: pyvista>=0.32.0 ; extra == "graphics"
 Requires-Dist: pytest==7.4.0 ; extra == "tests"
```

