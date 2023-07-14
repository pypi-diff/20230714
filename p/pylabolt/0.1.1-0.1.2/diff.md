# Comparing `tmp/pylabolt-0.1.1.tar.gz` & `tmp/pylabolt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylabolt-0.1.1.tar", last modified: Sat May  6 13:48:25 2023, max compression
+gzip compressed data, was "pylabolt-0.1.2.tar", last modified: Fri Jul 14 08:40:47 2023, max compression
```

## Comparing `pylabolt-0.1.1.tar` & `pylabolt-0.1.2.tar`

### file list

```diff
@@ -1,54 +1,60 @@
-drwxrwxr-x   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-06 13:48:25.893729 pylabolt-0.1.1/
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)    35149 2023-04-30 13:48:57.000000 pylabolt-0.1.1/LICENSE
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)      625 2023-05-06 13:48:25.893729 pylabolt-0.1.1/PKG-INFO
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)       83 2023-05-06 13:40:14.000000 pylabolt-0.1.1/README.rst
-drwxrwxr-x   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-06 13:48:25.893729 pylabolt-0.1.1/pylabolt/
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-01 14:08:59.000000 pylabolt-0.1.1/pylabolt/__init__.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)      102 2023-05-01 14:08:59.000000 pylabolt-0.1.1/pylabolt/__main__.py
-drwxrwxr-x   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-06 13:48:25.893729 pylabolt-0.1.1/pylabolt/base/
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-01 14:08:59.000000 pylabolt-0.1.1/pylabolt/base/__init__.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)    10958 2023-05-06 13:28:52.000000 pylabolt-0.1.1/pylabolt/base/baseAlgorithm.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)    10145 2023-05-06 13:29:10.000000 pylabolt-0.1.1/pylabolt/base/boundary.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     3122 2023-05-01 14:08:59.000000 pylabolt-0.1.1/pylabolt/base/boundaryConditions.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)    10938 2023-05-06 13:34:26.000000 pylabolt-0.1.1/pylabolt/base/createSim.py
-drwxrwxr-x   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-06 13:48:25.893729 pylabolt-0.1.1/pylabolt/base/cuda/
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-01 14:08:59.000000 pylabolt-0.1.1/pylabolt/base/cuda/__init__.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     3942 2023-05-01 14:08:59.000000 pylabolt-0.1.1/pylabolt/base/cuda/boundaryConditions_cuda.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     1514 2023-05-01 14:08:59.000000 pylabolt-0.1.1/pylabolt/base/cuda/deviceFields.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     3565 2023-05-06 13:28:01.000000 pylabolt-0.1.1/pylabolt/base/cuda/kernels.py
-drwxrwxr-x   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-06 13:48:25.893729 pylabolt-0.1.1/pylabolt/base/cuda/models/
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-01 14:08:59.000000 pylabolt-0.1.1/pylabolt/base/cuda/models/__init__.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)      168 2023-05-01 14:08:59.000000 pylabolt-0.1.1/pylabolt/base/cuda/models/collisionModels_cuda.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)      566 2023-05-01 14:08:59.000000 pylabolt-0.1.1/pylabolt/base/cuda/models/equilibriumModels_cuda.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     4061 2023-05-05 16:34:11.000000 pylabolt-0.1.1/pylabolt/base/fields.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     1097 2023-05-01 14:08:59.000000 pylabolt-0.1.1/pylabolt/base/lattice.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)      963 2023-05-02 15:07:17.000000 pylabolt-0.1.1/pylabolt/base/mesh.py
-drwxrwxr-x   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-06 13:48:25.893729 pylabolt-0.1.1/pylabolt/base/models/
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-01 14:08:59.000000 pylabolt-0.1.1/pylabolt/base/models/__init__.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)      147 2023-05-01 14:08:59.000000 pylabolt-0.1.1/pylabolt/base/models/collisionModels.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)      528 2023-05-01 14:08:59.000000 pylabolt-0.1.1/pylabolt/base/models/equilibriumModels.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     2613 2023-05-06 13:35:27.000000 pylabolt-0.1.1/pylabolt/base/schemeLB.py
-drwxrwxr-x   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-06 13:48:25.893729 pylabolt-0.1.1/pylabolt/parallel/
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     6728 2023-05-05 16:52:58.000000 pylabolt-0.1.1/pylabolt/parallel/MPI_comm.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     8506 2023-05-06 12:24:33.000000 pylabolt-0.1.1/pylabolt/parallel/MPI_decompose.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     9860 2023-05-06 13:35:28.000000 pylabolt-0.1.1/pylabolt/parallel/MPI_reconstruct.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-01 14:08:59.000000 pylabolt-0.1.1/pylabolt/parallel/__init__.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     5377 2023-05-06 13:33:27.000000 pylabolt-0.1.1/pylabolt/parallel/parallelSetup.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     2303 2023-05-06 13:31:17.000000 pylabolt-0.1.1/pylabolt/pylabolt.py
-drwxrwxr-x   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-06 13:48:25.893729 pylabolt-0.1.1/pylabolt/solvers/
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-01 14:08:59.000000 pylabolt-0.1.1/pylabolt/solvers/__init__.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     1685 2023-05-06 13:30:58.000000 pylabolt-0.1.1/pylabolt/solvers/fluidLB.py
-drwxrwxr-x   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-06 13:48:25.893729 pylabolt-0.1.1/pylabolt/utils/
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-01 14:08:59.000000 pylabolt-0.1.1/pylabolt/utils/__init__.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     3000 2023-05-05 16:05:52.000000 pylabolt-0.1.1/pylabolt/utils/inputOutput.py
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     5092 2023-05-06 10:30:10.000000 pylabolt-0.1.1/pylabolt/utils/vtkconvert.py
-drwxrwxr-x   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-06 13:48:25.893729 pylabolt-0.1.1/pylabolt.egg-info/
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)      625 2023-05-06 13:48:25.000000 pylabolt-0.1.1/pylabolt.egg-info/PKG-INFO
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     1277 2023-05-06 13:48:25.000000 pylabolt-0.1.1/pylabolt.egg-info/SOURCES.txt
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        1 2023-05-06 13:48:25.000000 pylabolt-0.1.1/pylabolt.egg-info/dependency_links.txt
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)       52 2023-05-06 13:48:25.000000 pylabolt-0.1.1/pylabolt.egg-info/entry_points.txt
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)       94 2023-05-06 13:48:25.000000 pylabolt-0.1.1/pylabolt.egg-info/requires.txt
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        9 2023-05-06 13:48:25.000000 pylabolt-0.1.1/pylabolt.egg-info/top_level.txt
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        1 2023-05-06 13:38:43.000000 pylabolt-0.1.1/pylabolt.egg-info/zip-safe
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)       85 2023-04-30 13:48:57.000000 pylabolt-0.1.1/pyproject.toml
--rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     1018 2023-05-06 13:48:25.893729 pylabolt-0.1.1/setup.cfg
+drwxrwxr-x   0 malyadeep  (1001) malyadeep  (1001)        0 2023-07-14 08:40:47.606513 pylabolt-0.1.2/
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)    35149 2023-05-06 14:53:11.000000 pylabolt-0.1.2/LICENSE
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     7099 2023-07-14 08:40:47.606513 pylabolt-0.1.2/PKG-INFO
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     6528 2023-06-17 06:27:51.000000 pylabolt-0.1.2/README.rst
+drwxrwxr-x   0 malyadeep  (1001) malyadeep  (1001)        0 2023-07-14 08:40:47.602513 pylabolt-0.1.2/pylabolt/
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-06 14:53:11.000000 pylabolt-0.1.2/pylabolt/__init__.py
+drwxrwxr-x   0 malyadeep  (1001) malyadeep  (1001)        0 2023-07-14 08:40:47.602513 pylabolt-0.1.2/pylabolt/base/
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-06 14:53:11.000000 pylabolt-0.1.2/pylabolt/base/__init__.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)    12942 2023-06-17 14:42:52.000000 pylabolt-0.1.2/pylabolt/base/boundary.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     4237 2023-06-17 14:35:08.000000 pylabolt-0.1.2/pylabolt/base/boundaryConditions.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     3289 2023-07-06 11:18:35.000000 pylabolt-0.1.2/pylabolt/base/boundaryConditions_cuda.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     1097 2023-05-06 14:53:11.000000 pylabolt-0.1.2/pylabolt/base/lattice.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)      963 2023-05-06 14:53:11.000000 pylabolt-0.1.2/pylabolt/base/mesh.py
+drwxrwxr-x   0 malyadeep  (1001) malyadeep  (1001)        0 2023-07-14 08:40:47.602513 pylabolt-0.1.2/pylabolt/base/models/
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     1231 2023-06-21 03:20:53.000000 pylabolt-0.1.2/pylabolt/base/models/MRT_params.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-06 14:53:11.000000 pylabolt-0.1.2/pylabolt/base/models/__init__.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)      664 2023-06-21 05:38:31.000000 pylabolt-0.1.2/pylabolt/base/models/collisionModels.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)      690 2023-06-21 06:48:01.000000 pylabolt-0.1.2/pylabolt/base/models/collisionModels_cuda.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     1357 2023-06-03 09:27:22.000000 pylabolt-0.1.2/pylabolt/base/models/equilibriumModels.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     1411 2023-06-05 04:57:16.000000 pylabolt-0.1.2/pylabolt/base/models/equilibriumModels_cuda.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)      501 2023-06-20 13:58:05.000000 pylabolt-0.1.2/pylabolt/base/models/forcingModels.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)      533 2023-06-21 06:45:50.000000 pylabolt-0.1.2/pylabolt/base/models/forcingModels_cuda.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)    32504 2023-07-01 09:41:17.000000 pylabolt-0.1.2/pylabolt/base/obstacle.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     4608 2023-06-28 11:13:51.000000 pylabolt-0.1.2/pylabolt/base/obstacleTypes.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)    10244 2023-06-21 05:37:35.000000 pylabolt-0.1.2/pylabolt/base/schemeLB.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     2167 2023-05-31 10:55:30.000000 pylabolt-0.1.2/pylabolt/base/setRegionFields.py
+drwxrwxr-x   0 malyadeep  (1001) malyadeep  (1001)        0 2023-07-14 08:40:47.606513 pylabolt-0.1.2/pylabolt/parallel/
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)    11004 2023-06-29 09:43:16.000000 pylabolt-0.1.2/pylabolt/parallel/MPI_comm.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)    23361 2023-07-01 09:42:02.000000 pylabolt-0.1.2/pylabolt/parallel/MPI_decompose.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)    10161 2023-06-28 12:13:26.000000 pylabolt-0.1.2/pylabolt/parallel/MPI_reconstruct.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-06 14:53:11.000000 pylabolt-0.1.2/pylabolt/parallel/__init__.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     3508 2023-07-06 11:37:50.000000 pylabolt-0.1.2/pylabolt/parallel/cudaReduce.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     7924 2023-07-05 14:35:44.000000 pylabolt-0.1.2/pylabolt/parallel/parallelSetup.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     2311 2023-06-17 08:49:53.000000 pylabolt-0.1.2/pylabolt/pylabolt.py
+drwxrwxr-x   0 malyadeep  (1001) malyadeep  (1001)        0 2023-07-14 08:40:47.606513 pylabolt-0.1.2/pylabolt/solvers/
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-06 14:53:11.000000 pylabolt-0.1.2/pylabolt/solvers/__init__.py
+drwxrwxr-x   0 malyadeep  (1001) malyadeep  (1001)        0 2023-07-14 08:40:47.606513 pylabolt-0.1.2/pylabolt/solvers/fluidLB/
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        0 2023-06-19 04:54:47.000000 pylabolt-0.1.2/pylabolt/solvers/fluidLB/__init__.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)    22225 2023-07-06 10:28:01.000000 pylabolt-0.1.2/pylabolt/solvers/fluidLB/baseAlgorithm.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)    14671 2023-07-01 09:36:57.000000 pylabolt-0.1.2/pylabolt/solvers/fluidLB/createSim.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     3313 2023-07-03 14:36:14.000000 pylabolt-0.1.2/pylabolt/solvers/fluidLB/deviceFields.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     1658 2023-06-20 10:54:30.000000 pylabolt-0.1.2/pylabolt/solvers/fluidLB/fields.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     2851 2023-06-28 12:07:23.000000 pylabolt-0.1.2/pylabolt/solvers/fluidLB/fluidLB.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     2400 2023-05-31 10:26:17.000000 pylabolt-0.1.2/pylabolt/solvers/fluidLB/initFields.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     5037 2023-07-06 10:42:51.000000 pylabolt-0.1.2/pylabolt/solvers/fluidLB/kernels.py
+drwxrwxr-x   0 malyadeep  (1001) malyadeep  (1001)        0 2023-07-14 08:40:47.606513 pylabolt-0.1.2/pylabolt/utils/
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        0 2023-05-06 14:53:11.000000 pylabolt-0.1.2/pylabolt/utils/__init__.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     3142 2023-06-16 04:52:42.000000 pylabolt-0.1.2/pylabolt/utils/inputOutput.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)    17369 2023-07-06 10:49:08.000000 pylabolt-0.1.2/pylabolt/utils/options.py
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     4942 2023-06-15 18:02:52.000000 pylabolt-0.1.2/pylabolt/utils/vtkconvert.py
+drwxrwxr-x   0 malyadeep  (1001) malyadeep  (1001)        0 2023-07-14 08:40:47.602513 pylabolt-0.1.2/pylabolt.egg-info/
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     7099 2023-07-14 08:40:47.000000 pylabolt-0.1.2/pylabolt.egg-info/PKG-INFO
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     1565 2023-07-14 08:40:47.000000 pylabolt-0.1.2/pylabolt.egg-info/SOURCES.txt
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        1 2023-07-14 08:40:47.000000 pylabolt-0.1.2/pylabolt.egg-info/dependency_links.txt
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)       52 2023-07-14 08:40:47.000000 pylabolt-0.1.2/pylabolt.egg-info/entry_points.txt
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)       94 2023-07-14 08:40:47.000000 pylabolt-0.1.2/pylabolt.egg-info/requires.txt
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        9 2023-07-14 08:40:47.000000 pylabolt-0.1.2/pylabolt.egg-info/top_level.txt
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)        1 2023-07-14 08:40:47.000000 pylabolt-0.1.2/pylabolt.egg-info/zip-safe
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)       85 2023-05-06 14:53:11.000000 pylabolt-0.1.2/pyproject.toml
+-rw-rw-r--   0 malyadeep  (1001) malyadeep  (1001)     1068 2023-07-14 08:40:47.606513 pylabolt-0.1.2/setup.cfg
```

### Comparing `pylabolt-0.1.1/LICENSE` & `pylabolt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylabolt-0.1.1/pylabolt/base/boundaryConditions.py` & `pylabolt-0.1.2/pylabolt/base/boundaryConditions_cuda.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,70 +1,91 @@
-from numba import prange
+from numba import cuda
 import numpy as np
 
 
+@cuda.jit
 def fixedU(f, f_new, rho, u, faceList, outDirections, invDirections,
            boundaryVector, boundaryScalar, c, w, cs, Nx, Ny):
-    cs_2 = 1/(cs * cs)
-    for ind in prange(faceList.shape[0]):
-        rhoWall = rho[faceList[ind]]
+    itr = cuda.grid(1)
+    if itr < faceList.shape[0]:
+        cs_2 = 1/(cs * cs)
+        ind = faceList[itr]
+        rhoWall = rho[ind]
         for dir in range(invDirections.shape[0]):
             preFactor = 2 * w[outDirections[dir]] * rhoWall *\
                 ((c[outDirections[dir], 0] * boundaryVector[0] +
-                  c[outDirections[dir], 1] * boundaryVector[1])) * cs_2
-            f_new[faceList[ind], invDirections[dir]] = \
-                f[faceList[ind], outDirections[dir]] - preFactor
+                    c[outDirections[dir], 1] * boundaryVector[1])) * cs_2
+            f_new[ind, invDirections[dir]] = \
+                f[ind, outDirections[dir]] - preFactor
+    else:
+        return
 
 
+@cuda.jit
 def fixedPressure(f, f_new, rho, u, faceList, outDirections, invDirections,
                   boundaryVector, boundaryScalar, c, w, cs, Nx, Ny):
-    cs_2 = 1/(cs * cs)
-    cs_4 = cs_2 * cs_2
-    for ind in prange(faceList.shape[0]):
-        i, j = int(faceList[ind] / Ny), int(faceList[ind] % Ny)
+    itr = cuda.grid(1)
+    if itr < faceList.shape[0]:
+        cs_2 = 1/(cs * cs)
+        cs_4 = cs_2 * cs_2
+        ind = faceList[itr]
+        i, j = int(ind / Ny), int(ind % Ny)
         for direction in invDirections:
             c_mag = int(np.ceil((c[direction, 0] * c[direction, 0]
                         + c[direction, 1] * c[direction, 1])))
             if c_mag == 1:
                 i_nb = int(i + c[direction, 0])
                 j_nb = int(j + c[direction, 1])
                 ind_nb = int(i_nb * Ny + j_nb)
                 break
-        u_nb = u[faceList[ind], :] + 0.5 * (u[faceList[ind], :] -
-                                            u[ind_nb, :])
+        u_nb = u[ind, :] + 0.5 * (u[ind, :] - u[ind_nb, :])
         u_nb_2 = u_nb[0] * u_nb[0] + u_nb[1] * u_nb[1]
         for dir in range(invDirections.shape[0]):
             c_dot_u = (c[outDirections[dir], 0] * u_nb[0] +
                        c[outDirections[dir], 1] * u_nb[1])
-            preFactor = 2 * w[outDirections[dir]] * boundaryScalar * cs_2 *\
-                (1. + c_dot_u * c_dot_u * 0.5 * cs_4 - u_nb_2 * 0.5 * cs_2)
-            f_new[faceList[ind], invDirections[dir]] = \
-                - f[faceList[ind], outDirections[dir]] + preFactor
+            preFactor = 2 * w[outDirections[dir]] * boundaryScalar * \
+                cs_2 * (1. + c_dot_u * c_dot_u * 0.5 * cs_4 - u_nb_2
+                        * 0.5 * cs_2)
+            f_new[ind, invDirections[dir]] = \
+                - f[ind, outDirections[dir]] + preFactor
+    else:
+        return
 
 
+@cuda.jit
 def bounceBack(f, f_new, rho, u, faceList, outDirections, invDirections,
                boundaryVector, boundaryScalar, c, w, cs, Nx, Ny):
-    for ind in prange(faceList.shape[0]):
+    itr = cuda.grid(1)
+    if itr < faceList.shape[0]:
+        ind = faceList[itr]
         for dir in range(invDirections.shape[0]):
-            f_new[faceList[ind], invDirections[dir]] = \
-                f[faceList[ind], outDirections[dir]]
+            f_new[ind, invDirections[dir]] = \
+                f[ind, outDirections[dir]]
+    else:
+        return
 
 
+@cuda.jit
 def zeroGradient(f, f_new, rho, u, faceList, outDirections, invDirections,
                  boundaryVector, boundaryScalar, c, w, cs, Nx, Ny):
-    for ind in prange(faceList.shape[0]):
-        i, j = int(faceList[ind] / Ny), int(faceList[ind] % Ny)
+    itr = cuda.grid(1)
+    if itr < faceList.shape[0]:
+        ind = faceList[itr]
+        i, j = int(ind / Ny), int(ind % Ny)
         for direction in invDirections:
             c_mag = int(np.ceil((c[direction, 0] * c[direction, 0]
                         + c[direction, 1] * c[direction, 1])))
             if c_mag == 1:
                 i_nb = int(i + c[direction, 0])
                 j_nb = int(j + c[direction, 1])
                 ind_nb = int(i_nb * Ny + j_nb)
                 break
         for k in range(f.shape[1]):
-            f[faceList[ind], k] = f[ind_nb, k]
+            f[ind, k] = f[ind_nb, k]
+    else:
+        return
 
 
+@cuda.jit
 def periodic(f, f_new, rho, u, faceList, outDirections, invDirections,
              boundaryVector, boundaryScalar, c, w, cs, Nx, Ny):
     pass
```

### Comparing `pylabolt-0.1.1/pylabolt/base/createSim.py` & `pylabolt-0.1.2/pylabolt/solvers/fluidLB/createSim.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import os
 import sys
 import numpy as np
 import numba
+from copy import deepcopy
 
 
-from pylabolt.base import mesh, lattice, boundary, schemeLB, fields
-from pylabolt.parallel.MPI_decompose import decompose, distributeSolid_mpi
+from pylabolt.base import (mesh, lattice, boundary, schemeLB,
+                           obstacle)
+from pylabolt.solvers.fluidLB import (initFields, fields)
+from pylabolt.parallel.MPI_decompose import (decompose, distributeSolid_mpi,
+                                             distributeInitialFields_mpi)
+from pylabolt.utils.options import options
 
 
 @numba.njit
 def initializePopulations(Nx, Ny, f_eq, f, f_new, u, rho,
                           noOfDirections, equilibriumFunc,
                           equilibriumArgs, procBoundary):
     for ind in range(Nx * Ny):
@@ -27,16 +32,15 @@
         self.size = size
         if rank == 0:
             print('Reading simulation parameters...\n', flush=True)
         try:
             workingDir = os.getcwd()
             sys.path.append(workingDir)
             from simulation import (controlDict, boundaryDict, collisionDict,
-                                    latticeDict, meshDict, obstacle,
-                                    internalFields)
+                                    latticeDict, meshDict, internalFields)
         except ImportError as e:
             print('FATAL ERROR!')
             print(str(e))
             print('Aborting....')
             os._exit(1)
 
         if rank == 0:
@@ -60,96 +64,159 @@
         except KeyError as e:
             if rank == 0:
                 print('ERROR! Keyword ' + str(e) + ' missing in controlDict')
             os._exit(1)
         if rank == 0:
             self.writeControlLog()
             print('Setting control parameters done!\n', flush=True)
-        try:
-            self.u_initial = internalFields['u']
-            self.v_initial = internalFields['v']
-            self.U_initial = np.array([self.u_initial, self.v_initial],
-                                      dtype=self.precision)
-            self.rho_initial = np.float64(internalFields['rho'])
-        except KeyError as e:
-            if rank == 0:
-                print('ERROR! Keyword ' + str(e) +
-                      ' missing in internalFields')
 
         if rank == 0:
             print('Reading mesh info and creating mesh...', flush=True)
         self.mesh = mesh.createMesh(meshDict, self.precision)
         if rank == 0:
             print('Reading mesh info and creating mesh done!\n', flush=True)
-        if size > 1:
-            self.mpiParams = decompose(self.mesh, self.rank, self.size, comm)
+
         if rank == 0:
             print('Setting lattice structure...', flush=True)
         self.lattice = lattice.createLattice(latticeDict, self.precision)
         if rank == 0:
             print('Setting lattice structure done!\n', flush=True)
             print('Setting collision scheme and equilibrium model...',
                   flush=True)
         self.collisionScheme = schemeLB.collisionScheme(self.lattice,
                                                         collisionDict,
-                                                        parallelization)
+                                                        parallelization,
+                                                        self.rank,
+                                                        self.precision)
         if rank == 0:
-            self.schemeLog()
             print('Setting collision scheme and equilibrium model done!\n',
                   flush=True)
+
+        if rank == 0:
+            print('Setting forcing scheme...', flush=True)
+        self.forcingScheme = schemeLB.forcingScheme(self.precision,
+                                                    self.lattice)
+        self.forcingScheme.setForcingScheme(self.lattice,
+                                            self.collisionScheme,
+                                            self.rank,
+                                            self.precision)
+        if rank == 0:
+            self.schemeLog()
+            print('Setting forcing scheme done!\n', flush=True)
+
+        if size > 1:
+            if rank == 0:
+                print('Decomposing domain...', flush=True)
+            self.mpiParams = decompose(self.mesh, self.rank, self.size, comm)
+            if rank == 0:
+                print('Domain decomposition done!\n', flush=True)
+
+        if rank == 0:
+            print('Reading options...', flush=True)
+        self.options = options(self.rank, self.precision, self.mesh)
+
+        if rank == 0:
+            print('Reading option done!\n', flush=True)
+
+        if rank == 0:
             print('Initializing fields...', flush=True)
-        self.fields = fields.fields(self.mesh, self.lattice,
-                                    self.U_initial, self.rho_initial,
-                                    self.precision, size)
-        solid = fields.setObstacle(obstacle, self.mesh)
-        if size == 1:
-            fields.solid = solid
+
+        initialFields_temp = initFields.initFields(internalFields, self.mesh,
+                                                   self.precision, self.rank,
+                                                   comm)
+
+        self.initialFields = initFields.initialFields(self.mesh.Nx,
+                                                      self.mesh.Ny,
+                                                      self.precision)
+        self.obstacle = obstacle.obstacleSetup(size, self.mesh, self.precision)
+        solid = self.obstacle.setObstacle(self.mesh, self.precision,
+                                          self.options, initialFields_temp,
+                                          self.rank, size)
+        comm.Barrier()
+        if size > 1:
+            distributeInitialFields_mpi(initialFields_temp, self.initialFields,
+                                        self.mpiParams, self.mesh, self.rank,
+                                        self.size, comm, self.precision)
         else:
-            distributeSolid_mpi(solid, self.fields, self.mpiParams, self.mesh,
-                                self.rank, self.size, comm)
+            self.initialFields = initialFields_temp
+        self.fields = fields.fields(self.mesh, self.lattice,
+                                    self.initialFields,
+                                    self.precision, size, rank)
+        if (self.options.computeForces is True or self.options.computeTorque
+                is True and rank == 0):
+            self.obstacle.computeFluidNb(solid, self.mesh, self.lattice,
+                                         self.size)
+        # if rank == 0:
+        #     self.obstacle.details()
+        obstacleTemp = deepcopy(self.obstacle)
+        if size == 1 and solid is not None:
+            self.fields.solid = solid
+        elif size > 1 and solid is not None:
+            distributeSolid_mpi(solid, self.obstacle,
+                                self.fields, self.mpiParams, self.mesh,
+                                self.precision, self.rank, self.size, comm)
+        if rank == 0:
+            print('Initializing fields done!\n', flush=True)
+
         if rank == 0:
-            print('Initializing fields done!\n')
-            print('Reading boundary conditions...')
+            print('Reading boundary conditions...', flush=True)
         self.boundary = boundary.boundary(boundaryDict)
         if rank == 0:
-            self.boundary.readBoundaryDict()
+            self.boundary.readBoundaryDict(self.rank)
             self.boundary.initializeBoundary(self.lattice, self.mesh,
-                                             self.fields)
+                                             self.fields, self.precision)
             # self.boundary.details()
         if rank == 0:
             self.writeDomainLog(meshDict)
-            print('Reading boundary conditions done...\n')
-
+            print('Reading boundary conditions done...\n', flush=True)
+        if (self.options.computeForces is True or self.options.computeTorque
+                is True):
+            if rank == 0:
+                self.options.gatherObstacleNodes(obstacleTemp)
+                self.options.gatherBoundaryNodes(self.boundary)
+                # self.options.details(self.rank, self.mesh, self.fields.solid,
+                #                      self.fields.u, flag='all')
+        # if rank == 3:
+        #     self.obstacle.details()
+        #     obstacleTemp.details()
+        del obstacleTemp, solid
         # initialize functions
         self.equilibriumFunc = self.collisionScheme.equilibriumFunc
         self.equilibriumArgs = self.collisionScheme.equilibriumArgs
         self.collisionFunc = self.collisionScheme.collisionFunc
         self.setBoundaryFunc = self.boundary.setBoundary
 
         # Prepare function arguments
         self.collisionArgs = (
             self.mesh.Nx, self.mesh.Ny, self.fields.f_eq,
             self.fields.f, self.fields.f_new, self.fields.u, self.fields.rho,
             self.fields.solid, self.collisionFunc, self.equilibriumFunc,
-            self.collisionScheme.preFactor,
-            self.collisionScheme.equilibriumArgs,
-            self.fields.procBoundary
+            self.collisionScheme.preFactor, self.collisionScheme.
+            equilibriumArgs, self.fields.procBoundary, self.forcingScheme.
+            forceFunc_force, self.forcingScheme.forceArgs_force,
+            self.forcingScheme.forcingPreFactor,
+            self.lattice.noOfDirections, self.precision
         )
 
         self.streamArgs = (
             self.mesh.Nx, self.mesh.Ny, self.fields.f, self.fields.f_new,
-            self.lattice.c, self.lattice.noOfDirections,
-            self.lattice.invList, self.fields.solid, self.size
+            self.fields.solid, self.fields.rho, self.fields.u,
+            self.fields.procBoundary, self.lattice.c, self.lattice.w,
+            self.lattice.noOfDirections, self.collisionScheme.cs_2,
+            self.lattice.invList, self.size
         )
 
         self.computeFieldsArgs = (
             self.mesh.Nx, self.mesh.Ny, self.fields.f_new,
             self.fields.u, self.fields.rho, self.fields.solid,
             self.lattice.c, self.lattice.noOfDirections,
-            self.fields.procBoundary, self.size
+            self.fields.procBoundary, self.size,
+            self.forcingScheme.forceFunc_vel,
+            self.forcingScheme.forceArgs_vel,
+            self.fields.f_eq, self.precision
         )
 
         if size > 1:
             self.gatherArgs = (self.fields.u, self.fields.rho,
                                self.fields.solid, self.rank,
                                self.mpiParams.nProc_x,
                                self.mpiParams.nProc_y,
@@ -221,18 +288,26 @@
 
     def schemeLog(self):
         schemeFile = open('log_scheme', 'w')
         schemeFile.write('Scheme Information...\n')
         schemeFile.write('\tcollision scheme : ' +
                          str(self.collisionScheme.collisionModel) + '\n')
         schemeFile.write('\trelaxation time : ' +
-                         str(self.collisionScheme.tau) + '\n')
+                         str(self.collisionScheme.nu) + '\n')
         schemeFile.write('\tcollision scheme : ' +
                          str(self.collisionScheme.equilibriumModel) + '\n')
         schemeFile.write('\nLattice Information...\n')
         schemeFile.write('\tLattice : ' +
                          str(self.lattice.latticeType) + '\n')
         schemeFile.write('\tdeltaX in lattice units : ' +
                          str(self.lattice.deltaX) + '\n')
         schemeFile.write('\tdeltaT in lattice units : ' +
                          str(self.lattice.deltaT) + '\n')
+        schemeFile.write('\nForcing Information...\n')
+        try:
+            schemeFile.write('\tModel : ' + self.forcingScheme.
+                             forcingModel + '\n')
+            schemeFile.write('\tValue : ' + str(self.forcingScheme.
+                             forcingValue) + '\n')
+        except AttributeError:
+            schemeFile.write('\tNo Forcing scheme selected\n')
         schemeFile.close()
```

### Comparing `pylabolt-0.1.1/pylabolt/base/cuda/kernels.py` & `pylabolt-0.1.2/pylabolt/solvers/fluidLB/kernels.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,128 @@
 import numpy as np
 from numba import cuda
-from pylabolt.base.cuda.models.equilibriumModels_cuda import (firstOrder,
-                                                              secondOrder)
-from pylabolt.base.cuda.models.collisionModels_cuda import BGK
+from pylabolt.base.models.equilibriumModels_cuda import (stokesLinear,
+                                                         secondOrder,
+                                                         incompressible,
+                                                         oseen)
+from pylabolt.base.models.collisionModels_cuda import (BGK, MRT)
+from pylabolt.base.models.forcingModels_cuda import (Guo_force, Guo_vel)
+import pylabolt.parallel.cudaReduce as cudaReduce
 
 
 @cuda.jit
 def equilibriumRelaxation_cuda(Nx, Ny, f_eq, f, f_new, u, rho, solid,
-                               preFactor, cs_2, cs_4, c, w, equilibriumType,
-                               collisionType):
+                               preFactor, rho_0, U_0, cs_2, cs_4, c, w,
+                               source, noOfDirections, F, equilibriumType,
+                               collisionType, forcingType, forcingPreFactor):
     ind = cuda.grid(1)
     if ind < Nx * Ny:
-        if solid[ind] != 1:
+        if solid[ind, 0] != 1:
             if equilibriumType == 1:
-                firstOrder(f_eq[ind, :], u[ind, :],
-                           rho[ind], cs_2, cs_4, c, w)
+                stokesLinear(f_eq[ind, :], u[ind, :],
+                             rho[ind], rho_0, cs_2, c, w)
             elif equilibriumType == 2:
                 secondOrder(f_eq[ind, :], u[ind, :],
                             rho[ind], cs_2, cs_4, c, w)
+            elif equilibriumType == 3:
+                incompressible(f_eq[ind, :], u[ind, :],
+                               rho[ind], rho_0, cs_2, cs_4, c, w)
+            elif equilibriumType == 4:
+                oseen(f_eq[ind, :], u[ind, :],
+                      rho[ind], rho_0, U_0, cs_2, cs_4, c, w)
+
+            if forcingType == 1:
+                force = True
+                Guo_force(u[ind, :], source[ind, :], F, c, w,
+                          noOfDirections, cs_2, cs_4)
 
             if collisionType == 1:
                 BGK(f[ind, :], f_new[ind, :],
-                    f_eq[ind, :], preFactor)
+                    f_eq[ind, :], preFactor, forcingPreFactor,
+                    source[ind, :], force)
+            elif collisionType == 2:
+                MRT(f[ind, :], f_new[ind, :],
+                    f_eq[ind, :], preFactor, forcingPreFactor,
+                    source[ind, :], force)
     else:
         return
 
 
-@cuda.reduce
-def residueReduce(a, b):
-    return a + b
-
-
-def computeResiduals_cuda(u_sq, u_err_sq, rho_sq, rho_err_sq):
-    resU = np.sqrt(residueReduce(u_err_sq[:, 0])/(residueReduce(u_sq[:, 0])
-                   + 1e-9))
-    resV = np.sqrt(residueReduce(u_err_sq[:, 1])/(residueReduce(u_sq[:, 1])
-                   + 1e-9))
-    resRho = np.sqrt(residueReduce(rho_err_sq)/(residueReduce(rho_sq)
-                     + 1e-9))
-    # resU = np.sqrt(np.sum(u_err_sq[:, 0])/(np.sum(u_sq[:, 0])
-    #                + 1e-9))
-    # resV = np.sqrt(np.sum(u_err_sq[:, 1])/(np.sum(u_sq[:, 1])
-    #                + 1e-9))
-    # resRho = np.sqrt(np.sum(rho_err_sq)/(np.sum(rho_sq)
-    #                  + 1e-9))
+def computeResiduals_cuda(residues, noOfResidues, blocks,
+                          n_threads, blockSize):
+    cudaReduce.arrayShape = 6
+    cudaReduce.cudaSum(blocks, n_threads, blockSize, residues)
+    resU_num = residues[0, 0]
+    resU_den = residues[0, 1]
+    resV_num = residues[0, 2]
+    resV_den = residues[0, 3]
+    resRho_num = residues[0, 4]
+    resRho_den = residues[0, 5]
+    if np.isclose(resU_den, 0, rtol=1e-10):
+        resU_den += 1e-10
+    if np.isclose(resV_den, 0, rtol=1e-10):
+        resV_den += 1e-10
+    if np.isclose(resRho_den, 0, rtol=1e-10):
+        resRho_den += 1e-10
+    resU = np.sqrt(resU_num/resU_den)
+    resV = np.sqrt(resV_num/resV_den)
+    resRho = np.sqrt(resRho_num/resRho_den)
     return resU, resV, resRho
 
 
 @cuda.jit
 def computeFields_cuda(Nx, Ny, f_new, u, rho, solid, c,
-                       noOfDirections, u_old, rho_old, u_sq,
-                       u_err_sq, rho_sq, rho_err_sq):
+                       noOfDirections, forcingType, F, A, u_old,
+                       rho_old, residues, noOfResidues):
     ind = cuda.grid(1)
     if ind < Nx * Ny:
-        if solid[ind] != 1:
+        if solid[ind, 0] != 1:
             rhoSum = 0.
             uSum = 0.
             vSum = 0.
             for k in range(noOfDirections):
                 rhoSum += f_new[ind, k]
                 uSum += c[k, 0] * f_new[ind, k]
                 vSum += c[k, 1] * f_new[ind, k]
             rho[ind] = rhoSum
-            u[ind, 0] = uSum/(rho[ind] + 1e-9)
-            u[ind, 1] = vSum/(rho[ind] + 1e-9)
+            u[ind, 0] = uSum/(rho[ind])
+            u[ind, 1] = vSum/(rho[ind])
 
-            u_err_sq[ind, 0] = (u[ind, 0] - u_old[ind, 0]) * \
-                (u[ind, 0] - u_old[ind, 0])
-            u_sq[ind, 0] = u_old[ind, 0] * u_old[ind, 0]
-            u_err_sq[ind, 1] = (u[ind, 1] - u_old[ind, 1]) * \
-                (u[ind, 1] - u_old[ind, 1])
-            u_sq[ind, 1] = u_old[ind, 1] * u_old[ind, 1]
-            rho_err_sq[ind] = (rho[ind] - rho_old[ind]) * \
-                (rho[ind] - rho_old[ind])
-            rho_sq[ind] = rho_old[ind] * rho_old[ind]
-            u_old[ind, 0] = u[ind, 0]
-            u_old[ind, 1] = u[ind, 1]
-            rho_old[ind] = rho[ind]
+            if forcingType == 1:
+                Guo_vel(u[ind, :], rho[ind], F, A)
+
+        residues[ind, 0] = (u[ind, 0] - u_old[ind, 0]) * \
+            (u[ind, 0] - u_old[ind, 0])
+        residues[ind, 1] = u_old[ind, 0] * u_old[ind, 0]
+        residues[ind, 2] = (u[ind, 1] - u_old[ind, 1]) * \
+            (u[ind, 1] - u_old[ind, 1])
+        residues[ind, 3] = u_old[ind, 1] * u_old[ind, 1]
+        residues[ind, 4] = (rho[ind] - rho_old[ind]) * \
+            (rho[ind] - rho_old[ind])
+        residues[ind, 5] = rho_old[ind] * rho_old[ind]
+        u_old[ind, 0] = u[ind, 0]
+        u_old[ind, 1] = u[ind, 1]
+        rho_old[ind] = rho[ind]
     else:
         return
 
 
 @cuda.jit
-def stream_cuda(Nx, Ny, f, f_new, c, noOfDirections, invList, solid):
+def stream_cuda(Nx, Ny, f, f_new, solid, rho, u, c, w,
+                noOfDirections, cs_2, invList):
     ind = cuda.grid(1)
     if ind < Nx * Ny:
-        i, j = np.int32(ind / Ny), np.int32(ind % Ny)
-        for k in range(noOfDirections):
-            i_old = (i - np.int32(c[k, 0])
-                     + Nx) % Nx
-            j_old = (j - np.int32(c[k, 1])
-                     + Ny) % Ny
-            if solid[i_old * Ny + j_old] != 1:
-                f_new[ind, k] = f[i_old * Ny + j_old, k]
-            elif solid[i_old * Ny + j_old] == 1:
-                f_new[ind, k] = f[ind, invList[k]]
+        if solid[ind, 0] != 1:
+            i, j = np.int64(ind / Ny), np.int64(ind % Ny)
+            for k in range(noOfDirections):
+                i_old = (i - np.int64(c[k, 0]) + Nx) % Nx
+                j_old = (j - np.int64(c[k, 1]) + Ny) % Ny
+                if solid[i_old * Ny + j_old, 0] != 1:
+                    f_new[ind, k] = f[i_old * Ny + j_old, k]
+                elif solid[i_old * Ny + j_old, 0] == 1:
+                    ind_old = i_old * Ny + j_old
+                    preFactor = 2 * w[invList[k]] * rho[ind] * \
+                        (c[invList[k], 0] * u[ind_old, 0] +
+                         c[invList[k], 1] * u[ind_old, 1]) * cs_2
+                    f_new[ind, k] = f[ind, invList[k]] - preFactor
     else:
         return
```

### Comparing `pylabolt-0.1.1/pylabolt/base/lattice.py` & `pylabolt-0.1.2/pylabolt/base/lattice.py`

 * *Files identical despite different names*

### Comparing `pylabolt-0.1.1/pylabolt/base/mesh.py` & `pylabolt-0.1.2/pylabolt/base/mesh.py`

 * *Files identical despite different names*

### Comparing `pylabolt-0.1.1/pylabolt/base/models/equilibriumModels.py` & `pylabolt-0.1.2/pylabolt/base/models/equilibriumModels.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,11 +8,33 @@
         cu = c[k, 0] * u[0] + c[k, 1] * u[1]
         f_eq[k] = w[k] * rho * (1 + cs_2 * cu +
                                 0.5 * cs_4 * cu * cu -
                                 0.5 * cs_2 * u_2)
 
 
 @numba.njit
-def firstOrder(f_eq, u, rho, cs_2, c, w):
+def stokesLinear(f_eq, u, rho, rho_0, cs_2, c, w):
     for k in range(f_eq.shape[0]):
         cu = c[k, 0] * u[0] + c[k, 1] * u[1]
-        f_eq[k] = w[k] * rho * (1 + cu * cs_2)
+        f_eq[k] = w[k] * (rho + rho_0 * cu * cs_2)
+
+
+@numba.njit
+def incompressible(f_eq, u, rho, rho_0, cs_2, cs_4, c, w):
+    u_2 = u[0] * u[0] + u[1] * u[1]
+    for k in range(f_eq.shape[0]):
+        cu = c[k, 0] * u[0] + c[k, 1] * u[1]
+        f_eq[k] = w[k] * rho + w[k] * rho_0 * (cs_2 * cu +
+                                               0.5 * cs_4 * cu * cu -
+                                               0.5 * cs_2 * u_2)
+
+
+@numba.njit
+def oseen(f_eq, u, rho, rho_0, U_0, cs_2, cs_4, c, w):
+    uU = u[0] * U_0[0] + u[1] * U_0[1]
+    UU = U_0[0] * U_0[0] + U_0[1] * U_0[1]
+    for k in range(f_eq.shape[0]):
+        cu = c[k, 0] * u[0] + c[k, 1] * u[1]
+        cU = c[k, 0] * U_0[0] + c[k, 1] * U_0[1]
+        f_eq[k] = w[k] * rho + w[k] * rho_0 * \
+            (cs_2 * cu + (2 * cu * cU - cU * cU) * 0.5 * cs_4
+             - 0.5 * cs_2 * (2 * uU - UU))
```

### Comparing `pylabolt-0.1.1/pylabolt/parallel/MPI_reconstruct.py` & `pylabolt-0.1.2/pylabolt/parallel/MPI_reconstruct.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import numpy as np
 import os
 import sys
 import numba
 from mpi4py import MPI
+from time import perf_counter
+
 from pylabolt.base.mesh import createMesh
 
 
 def reconstructMesh(comm, precision):
     try:
         from simulation import meshDict
     except ImportError as e:
@@ -204,19 +206,21 @@
             print('Aborting....')
             comm.Abort(1)
         except FileNotFoundError as e:
             print('FATAL ERROR!')
             print(str(e))
             print('Aborting....')
             comm.Abort(1)
+        start = perf_counter()
         if rank == 0:
             print('Reconstructing fields --> time = ' + str(time))
         x, y, u, rho, solid = gather(rank, time, comm)
         if rank == 0:
             writeData(time, x, y, u, rho, solid)
+        runTime = perf_counter() - start
     elif options == 'all':
         try:
             from simulation import controlDict
             if int(controlDict['endTime']) < int(controlDict['saveInterval']):
                 raise Warning("'endTime' in controlDict is greater than" +
                               " 'saveInterval'! Execution may fail or" +
                               " produce no output at all!")
@@ -234,22 +238,27 @@
             print('Aborting....')
             comm.Abort(1)
         except FileNotFoundError as e:
             print('FATAL ERROR!')
             print(str(e))
             print('Aborting....')
             comm.Abort(1)
+        start = perf_counter()
         for time in range(startTime, endTime + 1, interval):
             if rank == 0:
                 print('Reconstructing fields --> time = ' + str(time))
             x, y, u, rho, solid = gather(rank, time, comm)
             if rank == 0:
                 writeData(time, x, y, u, rho, solid)
+        runTime = perf_counter() - start
     elif options == 'time':
+        start = perf_counter()
         if rank == 0:
             print('Reconstructing fields --> time = ' + str(time))
         x, y, u, rho, solid = gather(rank, time, comm)
         if rank == 0:
             writeData(time, x, y, u, rho, solid)
+        runTime = perf_counter() - start
     if rank == 0:
-        print('\nReconstruction of Fields done!\n')
+        print('\nReconstruction of Fields done!')
+        print('\nRun time = ' + str(runTime) + ' s \n')
     MPI.Finalize()
```

### Comparing `pylabolt-0.1.1/pylabolt/pylabolt.py` & `pylabolt-0.1.2/pylabolt/pylabolt.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     if args.cuda is True and args.parallel is True:
         raise RuntimeError("ERROR! set a single backend for parallelization!")
         os._exit(1)
     elif args.parallel is False and args.cuda is False:
         parallelization = None
 
     if args.solver == 'fluidLB':
-        from pylabolt.solvers import fluidLB
+        from pylabolt.solvers.fluidLB import fluidLB
         fluidLB.main(parallelization, n_threads=args.n_threads)
 
     if args.reconstruct is not None:
         from pylabolt.parallel.MPI_reconstruct import reconstruct
         reconstruct(args.reconstruct, args.time)
 
     if args.toVTK is not None:
```

### Comparing `pylabolt-0.1.1/pylabolt/utils/inputOutput.py` & `pylabolt-0.1.2/pylabolt/utils/inputOutput.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import os
 import pickle
+import numpy as np
 
 
 def writeFields(timeStep, fields, mesh):
     if not os.path.isdir('output'):
         os.makedirs('output')
     if not os.path.isdir('output/' + str(timeStep)):
         os.makedirs('output/' + str(timeStep))
     writeFile = open('output/' + str(timeStep) + '/fields.dat', 'w')
     for ind in range(fields.u.shape[0]):
-        writeFile.write(str(round(ind, 10)).ljust(12) + '\t' +
-                        str(round(mesh.x[ind], 10)).ljust(12) + '\t' +
-                        str(round(mesh.y[ind], 10)).ljust(12) + '\t' +
-                        str(round(fields.rho[ind], 10)).ljust(12) + '\t' +
-                        str(round(fields.u[ind, 0], 10)).ljust(12) + '\t' +
-                        str(round(fields.u[ind, 1], 10)).ljust(12) + '\t' +
-                        str(round(fields.solid[ind], 10)).ljust(12) + '\n')
+        writeFile.write(str(np.round(ind, 10)).ljust(12) + '\t' +
+                        str(np.round(mesh.x[ind], 10)).ljust(12) + '\t' +
+                        str(np.round(mesh.y[ind], 10)).ljust(12) + '\t' +
+                        str(np.round(fields.rho[ind], 10)).ljust(12) + '\t' +
+                        str(np.round(fields.u[ind, 0], 10)).ljust(12) + '\t' +
+                        str(np.round(fields.u[ind, 1], 10)).ljust(12) + '\t' +
+                        str(np.round(fields.solid[ind, 0], 10)).ljust(12) +
+                        '\n')
     writeFile.close()
 
 
 def saveState(timeStep, simulation):
     if not os.path.isdir('states'):
         os.makedirs('states')
     if not os.path.isdir('states/' + str(timeStep)):
@@ -62,13 +64,15 @@
     if not os.path.isdir('procs/proc_' + str(rank) + '/' + str(timeStep)):
         os.makedirs('procs/proc_' + str(rank) + '/' + str(timeStep))
     writeFile = open('procs/proc_' + str(rank) + '/' +
                      str(timeStep) + '/fields.dat', 'w')
     for i in range(mesh.Nx):
         for j in range(mesh.Ny):
             ind = i * mesh.Ny + j
-            writeFile.write(str(round(ind, 10)).ljust(12) + '\t' +
-                            str(round(fields.rho[ind], 10)).ljust(12) + '\t' +
-                            str(round(fields.u[ind, 0], 10)).ljust(12) + '\t' +
-                            str(round(fields.u[ind, 1], 10)).ljust(12) + '\t' +
-                            str(round(fields.solid[ind], 10)).ljust(12) + '\n')
+            writeFile.write(str(np.round(ind, 10)).ljust(12) + '\t' +
+                            str(np.round(fields.rho[ind], 10)).ljust(12) + '\t'
+                            + str(np.round(fields.u[ind, 0], 10)).ljust(12) +
+                            '\t' + str(np.round(fields.u[ind, 1], 10)).
+                            ljust(12) + '\t' +
+                            str(np.round(fields.solid[ind, 0], 10)).ljust(12)
+                            + '\n')
     writeFile.close()
```

### Comparing `pylabolt-0.1.1/pylabolt.egg-info/SOURCES.txt` & `pylabolt-0.1.2/pylabolt.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 LICENSE
 README.rst
 pyproject.toml
 setup.cfg
 pylabolt/__init__.py
-pylabolt/__main__.py
 pylabolt/pylabolt.py
 pylabolt.egg-info/PKG-INFO
 pylabolt.egg-info/SOURCES.txt
 pylabolt.egg-info/dependency_links.txt
 pylabolt.egg-info/entry_points.txt
 pylabolt.egg-info/requires.txt
 pylabolt.egg-info/top_level.txt
 pylabolt.egg-info/zip-safe
 pylabolt/base/__init__.py
-pylabolt/base/baseAlgorithm.py
 pylabolt/base/boundary.py
 pylabolt/base/boundaryConditions.py
-pylabolt/base/createSim.py
-pylabolt/base/fields.py
+pylabolt/base/boundaryConditions_cuda.py
 pylabolt/base/lattice.py
 pylabolt/base/mesh.py
+pylabolt/base/obstacle.py
+pylabolt/base/obstacleTypes.py
 pylabolt/base/schemeLB.py
-pylabolt/base/cuda/__init__.py
-pylabolt/base/cuda/boundaryConditions_cuda.py
-pylabolt/base/cuda/deviceFields.py
-pylabolt/base/cuda/kernels.py
-pylabolt/base/cuda/models/__init__.py
-pylabolt/base/cuda/models/collisionModels_cuda.py
-pylabolt/base/cuda/models/equilibriumModels_cuda.py
+pylabolt/base/setRegionFields.py
+pylabolt/base/models/MRT_params.py
 pylabolt/base/models/__init__.py
 pylabolt/base/models/collisionModels.py
+pylabolt/base/models/collisionModels_cuda.py
 pylabolt/base/models/equilibriumModels.py
+pylabolt/base/models/equilibriumModels_cuda.py
+pylabolt/base/models/forcingModels.py
+pylabolt/base/models/forcingModels_cuda.py
 pylabolt/parallel/MPI_comm.py
 pylabolt/parallel/MPI_decompose.py
 pylabolt/parallel/MPI_reconstruct.py
 pylabolt/parallel/__init__.py
+pylabolt/parallel/cudaReduce.py
 pylabolt/parallel/parallelSetup.py
 pylabolt/solvers/__init__.py
-pylabolt/solvers/fluidLB.py
+pylabolt/solvers/fluidLB/__init__.py
+pylabolt/solvers/fluidLB/baseAlgorithm.py
+pylabolt/solvers/fluidLB/createSim.py
+pylabolt/solvers/fluidLB/deviceFields.py
+pylabolt/solvers/fluidLB/fields.py
+pylabolt/solvers/fluidLB/fluidLB.py
+pylabolt/solvers/fluidLB/initFields.py
+pylabolt/solvers/fluidLB/kernels.py
 pylabolt/utils/__init__.py
 pylabolt/utils/inputOutput.py
+pylabolt/utils/options.py
 pylabolt/utils/vtkconvert.py
```

### Comparing `pylabolt-0.1.1/setup.cfg` & `pylabolt-0.1.2/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
 name = pylabolt
-version = 0.1.1
+version = 0.1.2
 author = Malyadeep Bhattacharya, Mithun M Nair
 author_email = malyadeep1999@gmail.com
-url = https://github.com/Malyadeep/LBpy
+url = https://github.com/Malyadeep/pylabolt/tree/stable
 description = A single phase 2D lattice Boltzmann solver
 long_description = file: README.rst
-long_description_content_type = text/markdown
-keywords = lattice Boltzmann
+long_description_content_type = text/x-rst
+keywords = lattice Boltzmann, fluid flow, CFD
 license = GNU GENERAL PUBLIC LICENSE 3.0
 classifiers = 
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Programming Language :: Python :: 3
 
 [options]
 packages = find:
@@ -32,14 +32,14 @@
 example = README.rst, docs/, tests/
 
 [options.entry_points]
 console_scripts = 
 	pylabolt = pylabolt.pylabolt:main
 
 [project.urls]
-"Homepage" = https://github.com/Malyadeep/LBpy
-"Bug Tracker" = https://github.com/Malyadeep/LBpy/issues
+"Homepage" = https://github.com/Malyadeep/pylabolt/tree/stable
+"Bug Tracker" = https://github.com/Malyadeep/pylabolt/issues
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

