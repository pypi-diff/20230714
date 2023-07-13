# Comparing `tmp/prog_models-1.5.1.tar.gz` & `tmp/prog_models-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prog_models-1.5.1.tar", last modified: Thu Jul 13 03:45:36 2023, max compression
+gzip compressed data, was "prog_models-1.5.2.tar", last modified: Thu Jul 13 22:33:57 2023, max compression
```

## Comparing `prog_models-1.5.1.tar` & `prog_models-1.5.2.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.557369 prog_models-1.5.1/
--rw-r--r--   0 cteubert   (507) staff       (20)     7013 2023-07-13 03:45:36.557201 prog_models-1.5.1/PKG-INFO
--rw-r--r--   0 cteubert   (507) staff       (20)     5153 2023-07-10 14:41:28.000000 prog_models-1.5.1/README.md
--rw-r--r--   0 cteubert   (507) staff       (20)       38 2023-07-13 03:45:36.557416 prog_models-1.5.1/setup.cfg
--rw-r--r--   0 cteubert   (507) staff       (20)     2928 2023-07-13 03:44:24.000000 prog_models-1.5.1/setup.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.527922 prog_models-1.5.1/src/
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.531760 prog_models-1.5.1/src/prog_models/
--rw-r--r--   0 cteubert   (507) staff       (20)      464 2023-07-13 03:44:13.000000 prog_models-1.5.1/src/prog_models/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)    12776 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/composite_model.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.534362 prog_models-1.5.1/src/prog_models/data_models/
--rw-r--r--   0 cteubert   (507) staff       (20)      476 2023-07-05 23:05:00.000000 prog_models-1.5.1/src/prog_models/data_models/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     8208 2023-07-13 03:43:42.000000 prog_models-1.5.1/src/prog_models/data_models/data_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)    22276 2023-07-13 03:43:42.000000 prog_models-1.5.1/src/prog_models/data_models/dmd.py
--rw-r--r--   0 cteubert   (507) staff       (20)    35216 2023-07-13 03:43:42.000000 prog_models-1.5.1/src/prog_models/data_models/lstm_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)     8465 2023-07-13 03:43:42.000000 prog_models-1.5.1/src/prog_models/data_models/pce.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.534829 prog_models-1.5.1/src/prog_models/datasets/
--rw-r--r--   0 cteubert   (507) staff       (20)      157 2023-06-20 18:44:15.000000 prog_models-1.5.1/src/prog_models/datasets/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6185 2023-07-05 23:05:00.000000 prog_models-1.5.1/src/prog_models/datasets/nasa_battery.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6170 2023-07-05 23:05:00.000000 prog_models-1.5.1/src/prog_models/datasets/nasa_cmapss.py
--rw-r--r--   0 cteubert   (507) staff       (20)     5558 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/ensemble_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)      543 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/exceptions.py
--rw-r--r--   0 cteubert   (507) staff       (20)     9133 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/linear_model.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.536622 prog_models-1.5.1/src/prog_models/loading/
--rw-r--r--   0 cteubert   (507) staff       (20)      347 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/loading/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)    15484 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/loading/controllers.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1495 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/loading/gaussian_wrapper.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2102 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/loading/moving_average.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1772 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/loading/piecewise.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.540054 prog_models-1.5.1/src/prog_models/models/
--rw-r--r--   0 cteubert   (507) staff       (20)      918 2023-07-05 23:05:00.000000 prog_models-1.5.1/src/prog_models/models/__init__.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.541365 prog_models-1.5.1/src/prog_models/models/aircraft_model/
--rw-r--r--   0 cteubert   (507) staff       (20)      242 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/aircraft_model/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)      335 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/aircraft_model/aircraft.py
--rw-r--r--   0 cteubert   (507) staff       (20)    19213 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/aircraft_model/small_rotorcraft.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.542558 prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/
--rw-r--r--   0 cteubert   (507) staff       (20)      159 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/__init__.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.543479 prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/aero/
--rw-r--r--   0 cteubert   (507) staff       (20)      159 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/aero/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1387 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/aero/aerodynamics.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.543937 prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/control/
--rw-r--r--   0 cteubert   (507) staff       (20)      159 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/control/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2583 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/control/allocation_functions.py
--rw-r--r--   0 cteubert   (507) staff       (20)    12709 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/vehicles.py
--rw-r--r--   0 cteubert   (507) staff       (20)     7882 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/battery_circuit.py
--rw-r--r--   0 cteubert   (507) staff       (20)    32566 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/battery_electrochem.py
--rw-r--r--   0 cteubert   (507) staff       (20)    12741 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/centrifugal_pump.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6530 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/dcmotor.py
--rw-r--r--   0 cteubert   (507) staff       (20)     5649 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/dcmotor_singlephase.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4653 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/esc.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.545257 prog_models-1.5.1/src/prog_models/models/experimental/
--rw-r--r--   0 cteubert   (507) staff       (20)      158 2023-06-20 20:08:13.000000 prog_models-1.5.1/src/prog_models/models/experimental/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2949 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/experimental/paris_law.py
--rw-r--r--   0 cteubert   (507) staff       (20)    17214 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/pneumatic_valve.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6555 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/powertrain.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1428 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/propeller_load.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.547681 prog_models-1.5.1/src/prog_models/models/test_models/
--rw-r--r--   0 cteubert   (507) staff       (20)      249 2023-07-05 23:05:00.000000 prog_models-1.5.1/src/prog_models/models/test_models/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4384 2023-07-05 23:05:00.000000 prog_models-1.5.1/src/prog_models/models/test_models/linear_models.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4050 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/test_models/linear_thrown_object.py
--rw-r--r--   0 cteubert   (507) staff       (20)     5714 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/models/thrown_object.py
--rw-r--r--   0 cteubert   (507) staff       (20)    68654 2023-07-13 03:43:42.000000 prog_models-1.5.1/src/prog_models/prognostics_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)    17189 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/sim_result.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.549997 prog_models-1.5.1/src/prog_models/utils/
--rw-r--r--   0 cteubert   (507) staff       (20)      198 2023-06-20 18:44:15.000000 prog_models-1.5.1/src/prog_models/utils/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)    21583 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/utils/calc_error.py
--rw-r--r--   0 cteubert   (507) staff       (20)     8984 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/utils/containers.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1014 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/utils/input_validation.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4382 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/utils/next_state.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2242 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/utils/noise_functions.py
--rw-r--r--   0 cteubert   (507) staff       (20)    10374 2023-07-05 23:05:00.000000 prog_models-1.5.1/src/prog_models/utils/parameters.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1173 2023-07-05 23:05:00.000000 prog_models-1.5.1/src/prog_models/utils/progress_bar.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1859 2023-07-05 23:05:00.000000 prog_models-1.5.1/src/prog_models/utils/serialization.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2484 2023-07-05 23:05:00.000000 prog_models-1.5.1/src/prog_models/utils/size.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.551333 prog_models-1.5.1/src/prog_models/utils/traj_gen/
--rw-r--r--   0 cteubert   (507) staff       (20)      221 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/utils/traj_gen/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)    24434 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/utils/traj_gen/geometry.py
--rw-r--r--   0 cteubert   (507) staff       (20)    16044 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/utils/traj_gen/nurbs.py
--rw-r--r--   0 cteubert   (507) staff       (20)    33968 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/utils/traj_gen/trajectory.py
--rw-r--r--   0 cteubert   (507) staff       (20)    27416 2023-07-10 14:41:28.000000 prog_models-1.5.1/src/prog_models/visualize.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.532951 prog_models-1.5.1/src/prog_models.egg-info/
--rw-r--r--   0 cteubert   (507) staff       (20)     7013 2023-07-13 03:45:36.000000 prog_models-1.5.1/src/prog_models.egg-info/PKG-INFO
--rw-r--r--   0 cteubert   (507) staff       (20)     3302 2023-07-13 03:45:36.000000 prog_models-1.5.1/src/prog_models.egg-info/SOURCES.txt
--rw-r--r--   0 cteubert   (507) staff       (20)        1 2023-07-13 03:45:36.000000 prog_models-1.5.1/src/prog_models.egg-info/dependency_links.txt
--rw-r--r--   0 cteubert   (507) staff       (20)      204 2023-07-13 03:45:36.000000 prog_models-1.5.1/src/prog_models.egg-info/requires.txt
--rw-r--r--   0 cteubert   (507) staff       (20)       12 2023-07-13 03:45:36.000000 prog_models-1.5.1/src/prog_models.egg-info/top_level.txt
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-07-13 03:45:36.556962 prog_models-1.5.1/tests/
--rw-r--r--   0 cteubert   (507) staff       (20)    56896 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_base_models.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2652 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_battery.py
--rw-r--r--   0 cteubert   (507) staff       (20)    18087 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_calc_error.py
--rw-r--r--   0 cteubert   (507) staff       (20)     8122 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_centrifugal_pump.py
--rw-r--r--   0 cteubert   (507) staff       (20)    14085 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_composite.py
--rw-r--r--   0 cteubert   (507) staff       (20)    13250 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_data_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1872 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_datasets.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4177 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_dict_like_matrix_wrapper.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4622 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_direct.py
--rw-r--r--   0 cteubert   (507) staff       (20)     7537 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_ensemble.py
--rw-r--r--   0 cteubert   (507) staff       (20)    55549 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_estimate_params.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1627 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_examples.py
--rw-r--r--   0 cteubert   (507) staff       (20)    18578 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_linear_model.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6686 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_manual.py
--rw-r--r--   0 cteubert   (507) staff       (20)    12907 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_pneumatic_valve.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2435 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_powertrain.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4267 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_serialization.py
--rw-r--r--   0 cteubert   (507) staff       (20)    35373 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_sim_result.py
--rw-r--r--   0 cteubert   (507) staff       (20)    32855 2023-07-13 03:43:36.000000 prog_models-1.5.1/tests/test_surrogates.py
--rw-r--r--   0 cteubert   (507) staff       (20)      918 2023-07-10 14:41:28.000000 prog_models-1.5.1/tests/test_tutorials.py
--rw-r--r--   0 cteubert   (507) staff       (20)    15453 2023-07-13 03:43:36.000000 prog_models-1.5.1/tests/test_uav_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:33:57.222330 prog_models-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-07-13 22:33:57.222330 prog_models-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-13 22:33:47.000000 prog_models-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 22:33:57.222330 prog_models-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-13 22:33:47.000000 prog_models-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:33:57.210330 prog_models-1.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:33:57.210330 prog_models-1.5.2/src/prog_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/composite_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:33:57.214330 prog_models-1.5.2/src/prog_models/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/data_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/data_models/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22276 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/data_models/dmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35060 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/data_models/lstm_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/data_models/pce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:33:57.214330 prog_models-1.5.2/src/prog_models/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/datasets/nasa_battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/datasets/nasa_cmapss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/linear_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:33:57.214330 prog_models-1.5.2/src/prog_models/loading/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/loading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15484 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/loading/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/loading/gaussian_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/loading/moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/loading/piecewise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:33:57.214330 prog_models-1.5.2/src/prog_models/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:33:57.214330 prog_models-1.5.2/src/prog_models/models/aircraft_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/aircraft_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/aircraft_model/aircraft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19213 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/aircraft_model/small_rotorcraft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:33:57.214330 prog_models-1.5.2/src/prog_models/models/aircraft_model/vehicles/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/aircraft_model/vehicles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:33:57.214330 prog_models-1.5.2/src/prog_models/models/aircraft_model/vehicles/aero/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/aircraft_model/vehicles/aero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/aircraft_model/vehicles/aero/aerodynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:33:57.218330 prog_models-1.5.2/src/prog_models/models/aircraft_model/vehicles/control/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/aircraft_model/vehicles/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/aircraft_model/vehicles/control/allocation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12709 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/aircraft_model/vehicles/vehicles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/battery_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32566 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/battery_electrochem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/centrifugal_pump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/dcmotor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/dcmotor_singlephase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/esc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:33:57.218330 prog_models-1.5.2/src/prog_models/models/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/experimental/paris_law.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17214 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/pneumatic_valve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/powertrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/propeller_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:33:57.218330 prog_models-1.5.2/src/prog_models/models/test_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/test_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/test_models/linear_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/test_models/linear_thrown_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/models/thrown_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68654 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/prognostics_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17189 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/sim_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:33:57.218330 prog_models-1.5.2/src/prog_models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21583 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/utils/calc_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/utils/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/utils/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/utils/next_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/utils/noise_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/utils/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/utils/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/utils/size.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:33:57.218330 prog_models-1.5.2/src/prog_models/utils/traj_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/utils/traj_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24434 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/utils/traj_gen/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16044 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/utils/traj_gen/nurbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33968 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/utils/traj_gen/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27416 2023-07-13 22:33:47.000000 prog_models-1.5.2/src/prog_models/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:33:57.214330 prog_models-1.5.2/src/prog_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-07-13 22:33:57.000000 prog_models-1.5.2/src/prog_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-13 22:33:57.000000 prog_models-1.5.2/src/prog_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 22:33:57.000000 prog_models-1.5.2/src/prog_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 22:33:57.000000 prog_models-1.5.2/src/prog_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 22:33:57.000000 prog_models-1.5.2/src/prog_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:33:57.222330 prog_models-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    56896 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_base_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18087 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_calc_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_centrifugal_pump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_dict_like_matrix_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55549 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_estimate_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_linear_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_pneumatic_valve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_powertrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35373 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_sim_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32855 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_surrogates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_tutorials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-07-13 22:33:47.000000 prog_models-1.5.2/tests/test_uav_model.py
```

### Comparing `prog_models-1.5.1/PKG-INFO` & `prog_models-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prog_models
-Version: 1.5.1
+Version: 1.5.2
 Summary: The NASA Prognostic Model Package is a python modeling framework focused on defining and building models for prognostics (computation of remaining useful life) of engineering systems, and provides a set of prognostics models for select components developed within this framework, suitable for use in prognostics applications for these components.
 Home-page: https://nasa.github.io/progpy/prog_models_guide.html
 Author: Christopher Teubert
 Author-email: christopher.a.teubert@nasa.gov
 License: NOSA
 Project-URL: Bug Reports, https://github.com/nasa/prog_models/issues
 Project-URL: Docs, https://nasa.github.io/progpy/prog_models_guide.html
```

### Comparing `prog_models-1.5.1/README.md` & `prog_models-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/setup.py` & `prog_models-1.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         'fastdtw',  # For DTW error calculation
         "tensorflow; platform_system!='Darwin' or platform_machine!='arm64'",
         "tensorflow-macos; platform_system=='Darwin' and platform_machine=='arm64'",
     ]
 
 setup(
     name='prog_models',
-    version='1.5.1',
+    version='1.5.2',
     description='The NASA Prognostic Model Package is a python modeling framework focused on defining and building models for prognostics (computation of remaining useful life) of engineering systems, and provides a set of prognostics models for select components developed within this framework, suitable for use in prognostics applications for these components.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://nasa.github.io/progpy/prog_models_guide.html',
     author='Christopher Teubert',
     author_email='christopher.a.teubert@nasa.gov',
     classifiers=[
```

### Comparing `prog_models-1.5.1/src/prog_models/composite_model.py` & `prog_models-1.5.2/src/prog_models/composite_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/data_models/data_model.py` & `prog_models-1.5.2/src/prog_models/data_models/data_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/data_models/dmd.py` & `prog_models-1.5.2/src/prog_models/data_models/dmd.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/data_models/lstm_model.py` & `prog_models-1.5.2/src/prog_models/data_models/lstm_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -533,18 +533,15 @@
             # so we need to transpose them to a column vector
             params['normalization'] = (z_mean, z_std)
 
         # Tensorflow is imported here to avoid importing it if not needed
         from tensorflow import keras
 
         # Build model
-        callbacks = [
-            keras.callbacks.ModelCheckpoint("best_model.keras", save_best_only=True)
-        ]
-
+        callbacks = []
         if params['early_stop']:
             callbacks.append(keras.callbacks.EarlyStopping(**params['early_stop.cfg']))
 
         inputs = keras.Input(shape=u_all.shape[1:])
         x = inputs
         if params['normalize']:
             x = keras.layers.Normalization(mean = u_mean, variance = u_std**2)(inputs)
@@ -588,16 +585,14 @@
             output_data,
             epochs=params['epochs'],
             callbacks=callbacks,
             validation_split=params['validation_split'],
             workers=params['workers'],
             use_multiprocessing=(params['workers'] > 1))
 
-        model = keras.models.load_model("best_model.keras")
-
         # Split model into separate models
         n_state_layers = params['layers'] + 1 + (params['dropout'] > 0) + (params['normalize'])
         output_layer_input = keras.layers.Input(model.layers[n_state_layers-1].output.shape[1:])
         output_layer = model.get_layer('output')(output_layer_input)
         state_model = keras.Model(model.input, model.layers[n_state_layers-1].output)
         output_model = keras.Model(output_layer_input, output_layer)
         if event_states is None:
```

### Comparing `prog_models-1.5.1/src/prog_models/data_models/pce.py` & `prog_models-1.5.2/src/prog_models/data_models/pce.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/datasets/nasa_battery.py` & `prog_models-1.5.2/src/prog_models/datasets/nasa_battery.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/datasets/nasa_cmapss.py` & `prog_models-1.5.2/src/prog_models/datasets/nasa_cmapss.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/ensemble_model.py` & `prog_models-1.5.2/src/prog_models/ensemble_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/exceptions.py` & `prog_models-1.5.2/src/prog_models/exceptions.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/linear_model.py` & `prog_models-1.5.2/src/prog_models/linear_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/loading/controllers.py` & `prog_models-1.5.2/src/prog_models/loading/controllers.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/loading/gaussian_wrapper.py` & `prog_models-1.5.2/src/prog_models/loading/gaussian_wrapper.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/loading/moving_average.py` & `prog_models-1.5.2/src/prog_models/loading/moving_average.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/loading/piecewise.py` & `prog_models-1.5.2/src/prog_models/loading/piecewise.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/models/__init__.py` & `prog_models-1.5.2/src/prog_models/models/__init__.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/models/aircraft_model/small_rotorcraft.py` & `prog_models-1.5.2/src/prog_models/models/aircraft_model/small_rotorcraft.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/aero/aerodynamics.py` & `prog_models-1.5.2/src/prog_models/models/aircraft_model/vehicles/aero/aerodynamics.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/control/allocation_functions.py` & `prog_models-1.5.2/src/prog_models/models/aircraft_model/vehicles/control/allocation_functions.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/models/aircraft_model/vehicles/vehicles.py` & `prog_models-1.5.2/src/prog_models/models/aircraft_model/vehicles/vehicles.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/models/battery_circuit.py` & `prog_models-1.5.2/src/prog_models/models/battery_circuit.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/models/battery_electrochem.py` & `prog_models-1.5.2/src/prog_models/models/battery_electrochem.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/models/centrifugal_pump.py` & `prog_models-1.5.2/src/prog_models/models/centrifugal_pump.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/models/dcmotor.py` & `prog_models-1.5.2/src/prog_models/models/dcmotor.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/models/dcmotor_singlephase.py` & `prog_models-1.5.2/src/prog_models/models/dcmotor_singlephase.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/models/esc.py` & `prog_models-1.5.2/src/prog_models/models/esc.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/models/experimental/paris_law.py` & `prog_models-1.5.2/src/prog_models/models/experimental/paris_law.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/models/pneumatic_valve.py` & `prog_models-1.5.2/src/prog_models/models/pneumatic_valve.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/models/powertrain.py` & `prog_models-1.5.2/src/prog_models/models/powertrain.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/models/propeller_load.py` & `prog_models-1.5.2/src/prog_models/models/propeller_load.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/models/test_models/linear_models.py` & `prog_models-1.5.2/src/prog_models/models/test_models/linear_models.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/models/test_models/linear_thrown_object.py` & `prog_models-1.5.2/src/prog_models/models/test_models/linear_thrown_object.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/models/thrown_object.py` & `prog_models-1.5.2/src/prog_models/models/thrown_object.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/prognostics_model.py` & `prog_models-1.5.2/src/prog_models/prognostics_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/sim_result.py` & `prog_models-1.5.2/src/prog_models/sim_result.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/utils/calc_error.py` & `prog_models-1.5.2/src/prog_models/utils/calc_error.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/utils/containers.py` & `prog_models-1.5.2/src/prog_models/utils/containers.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/utils/input_validation.py` & `prog_models-1.5.2/src/prog_models/utils/input_validation.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/utils/next_state.py` & `prog_models-1.5.2/src/prog_models/utils/next_state.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/utils/noise_functions.py` & `prog_models-1.5.2/src/prog_models/utils/noise_functions.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/utils/parameters.py` & `prog_models-1.5.2/src/prog_models/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/utils/progress_bar.py` & `prog_models-1.5.2/src/prog_models/utils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/utils/serialization.py` & `prog_models-1.5.2/src/prog_models/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/utils/size.py` & `prog_models-1.5.2/src/prog_models/utils/size.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/utils/traj_gen/geometry.py` & `prog_models-1.5.2/src/prog_models/utils/traj_gen/geometry.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/utils/traj_gen/nurbs.py` & `prog_models-1.5.2/src/prog_models/utils/traj_gen/nurbs.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/utils/traj_gen/trajectory.py` & `prog_models-1.5.2/src/prog_models/utils/traj_gen/trajectory.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models/visualize.py` & `prog_models-1.5.2/src/prog_models/visualize.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/src/prog_models.egg-info/PKG-INFO` & `prog_models-1.5.2/src/prog_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prog-models
-Version: 1.5.1
+Version: 1.5.2
 Summary: The NASA Prognostic Model Package is a python modeling framework focused on defining and building models for prognostics (computation of remaining useful life) of engineering systems, and provides a set of prognostics models for select components developed within this framework, suitable for use in prognostics applications for these components.
 Home-page: https://nasa.github.io/progpy/prog_models_guide.html
 Author: Christopher Teubert
 Author-email: christopher.a.teubert@nasa.gov
 License: NOSA
 Project-URL: Bug Reports, https://github.com/nasa/prog_models/issues
 Project-URL: Docs, https://nasa.github.io/progpy/prog_models_guide.html
```

### Comparing `prog_models-1.5.1/src/prog_models.egg-info/SOURCES.txt` & `prog_models-1.5.2/src/prog_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_base_models.py` & `prog_models-1.5.2/tests/test_base_models.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_battery.py` & `prog_models-1.5.2/tests/test_battery.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_calc_error.py` & `prog_models-1.5.2/tests/test_calc_error.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_centrifugal_pump.py` & `prog_models-1.5.2/tests/test_centrifugal_pump.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_composite.py` & `prog_models-1.5.2/tests/test_composite.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_data_model.py` & `prog_models-1.5.2/tests/test_data_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_datasets.py` & `prog_models-1.5.2/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_dict_like_matrix_wrapper.py` & `prog_models-1.5.2/tests/test_dict_like_matrix_wrapper.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_direct.py` & `prog_models-1.5.2/tests/test_direct.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_ensemble.py` & `prog_models-1.5.2/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_estimate_params.py` & `prog_models-1.5.2/tests/test_estimate_params.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_examples.py` & `prog_models-1.5.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_linear_model.py` & `prog_models-1.5.2/tests/test_linear_model.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_manual.py` & `prog_models-1.5.2/tests/test_manual.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_pneumatic_valve.py` & `prog_models-1.5.2/tests/test_pneumatic_valve.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_powertrain.py` & `prog_models-1.5.2/tests/test_powertrain.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_serialization.py` & `prog_models-1.5.2/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_sim_result.py` & `prog_models-1.5.2/tests/test_sim_result.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_surrogates.py` & `prog_models-1.5.2/tests/test_surrogates.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_tutorials.py` & `prog_models-1.5.2/tests/test_tutorials.py`

 * *Files identical despite different names*

### Comparing `prog_models-1.5.1/tests/test_uav_model.py` & `prog_models-1.5.2/tests/test_uav_model.py`

 * *Files identical despite different names*

