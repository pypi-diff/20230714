# Comparing `tmp/tidy3d-2.3.0rc1.tar.gz` & `tmp/tidy3d-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidy3d-2.3.0rc1.tar", last modified: Mon Jun  5 20:08:20 2023, max compression
+gzip compressed data, was "tidy3d-2.3.1.tar", last modified: Fri Jul 14 19:13:34 2023, max compression
```

## Comparing `tidy3d-2.3.0rc1.tar` & `tidy3d-2.3.1.tar`

### file list

```diff
@@ -1,195 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.304961 tidy3d-2.3.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-06-05 20:08:20.304961 tidy3d-2.3.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.288961 tidy3d-2.3.0rc1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/requirements/basic.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/requirements/gdspy.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/requirements/gdstk.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/requirements/jax.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/requirements/trimesh.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/requirements/web.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 20:08:20.304961 tidy3d-2.3.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.288961 tidy3d-2.3.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.288961 tidy3d-2.3.0rc1/tests/_test_local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/_test_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/_test_local/_test_adjoint_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/_test_local/_test_data_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/_test_local/_test_fit_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/_test_local/_test_plugins_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/_test_local/_test_web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.292961 tidy3d-2.3.0rc1/tests/test_components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_IO.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_boundaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    32452 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_field_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_grid_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_medium.py
--rw-r--r--   0 runner    (1001) docker     (123)    23843 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_meshgenerate.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21134 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_sidewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    53649 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_components/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.292961 tidy3d-2.3.0rc1/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_data/test_data_arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)    19395 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_data/test_monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_data/test_sim_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.292961 tidy3d-2.3.0rc1/tests/test_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_package/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_package/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_package/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_package/test_make_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_package/test_material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_package/test_parametric_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.292961 tidy3d-2.3.0rc1/tests/test_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41852 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_plugins/test_adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_plugins/test_component_modeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_plugins/test_dispersion_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_plugins/test_mode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_plugins/test_polyslab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_plugins/test_resonance_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_plugins/test_waveguide.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.292961 tidy3d-2.3.0rc1/tests/test_web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_web/mock_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_web/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_web/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_web/test_material_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_web/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_web/test_tidy3d_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_web/test_tidy3d_material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_web/test_tidy3d_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/test_web/test_webapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.296961 tidy3d-2.3.0rc1/tidy3d/
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.296961 tidy3d-2.3.0rc1/tidy3d/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)    26944 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/boundary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.296961 tidy3d-2.3.0rc1/tidy3d/components/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14272 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/data/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    78767 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/data/monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    28054 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/data/sim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/field_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)   146898 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.300961 tidy3d-2.3.0rc1/tidy3d/components/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14955 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/grid/grid_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    47556 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/grid/mesher.py
--rw-r--r--   0 runner    (1001) docker     (123)   114593 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    29507 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)   119586 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    32775 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/components/viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.300961 tidy3d-2.3.0rc1/tidy3d/material_library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/material_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62029 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/material_library/material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/material_library/material_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/material_library/parametric_materials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.300961 tidy3d-2.3.0rc1/tidy3d/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.300961 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.300961 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.300961 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/data/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/data/monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/data/sim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23786 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    20217 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)    17771 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    30051 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.300961 tidy3d-2.3.0rc1/tidy3d/plugins/dispersion/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/dispersion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21590 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/dispersion/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/dispersion/fit_web.py
--rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/dispersion/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.300961 tidy3d-2.3.0rc1/tidy3d/plugins/mode/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/mode/derivatives.py
--rw-r--r--   0 runner    (1001) docker     (123)    25720 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/mode/mode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    27752 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/mode/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/mode/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.300961 tidy3d-2.3.0rc1/tidy3d/plugins/polyslab/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/polyslab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/polyslab/polyslab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.304961 tidy3d-2.3.0rc1/tidy3d/plugins/resonance/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/resonance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/resonance/resonance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.304961 tidy3d-2.3.0rc1/tidy3d/plugins/smatrix/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/smatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/smatrix/smatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.304961 tidy3d-2.3.0rc1/tidy3d/plugins/waveguide/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/waveguide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35573 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/plugins/waveguide/rectangular_dielectric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/updater.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.304961 tidy3d-2.3.0rc1/tidy3d/web/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)   275233 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.304961 tidy3d-2.3.0rc1/tidy3d/web/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/cli/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20751 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/http_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/httputils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/material_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/material_libray.py
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/s3utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16498 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/simulation_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    24457 2023-06-05 20:08:04.000000 tidy3d-2.3.0rc1/tidy3d/web/webapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:08:20.296961 tidy3d-2.3.0rc1/tidy3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-06-05 20:08:20.000000 tidy3d-2.3.0rc1/tidy3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-06-05 20:08:20.000000 tidy3d-2.3.0rc1/tidy3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:08:20.000000 tidy3d-2.3.0rc1/tidy3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-05 20:08:20.000000 tidy3d-2.3.0rc1/tidy3d.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-05 20:08:20.000000 tidy3d-2.3.0rc1/tidy3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 20:08:20.000000 tidy3d-2.3.0rc1/tidy3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:34.001042 tidy3d-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-14 19:13:15.000000 tidy3d-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-14 19:13:15.000000 tidy3d-2.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-07-14 19:13:34.001042 tidy3d-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-14 19:13:15.000000 tidy3d-2.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-14 19:13:15.000000 tidy3d-2.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.981041 tidy3d-2.3.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-14 19:13:15.000000 tidy3d-2.3.1/requirements/basic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-14 19:13:15.000000 tidy3d-2.3.1/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-14 19:13:15.000000 tidy3d-2.3.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 19:13:15.000000 tidy3d-2.3.1/requirements/gdspy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 19:13:15.000000 tidy3d-2.3.1/requirements/gdstk.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-14 19:13:15.000000 tidy3d-2.3.1/requirements/jax.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-14 19:13:15.000000 tidy3d-2.3.1/requirements/trimesh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-14 19:13:15.000000 tidy3d-2.3.1/requirements/web.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-14 19:13:15.000000 tidy3d-2.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 19:13:34.001042 tidy3d-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-14 19:13:15.000000 tidy3d-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.981041 tidy3d-2.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.981041 tidy3d-2.3.1/tests/_test_local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/_test_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/_test_local/_test_adjoint_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/_test_local/_test_data_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/_test_local/_test_fit_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/_test_local/_test_plugins_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/_test_local/_test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.985041 tidy3d-2.3.1/tests/test_components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35660 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_field_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_grid_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14648 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23843 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_meshgenerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21134 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_sidewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54875 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8394 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_components/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.985041 tidy3d-2.3.1/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_data/test_data_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20413 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_data/test_monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_data/test_sim_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.985041 tidy3d-2.3.1/tests/test_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_package/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_package/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_package/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_package/test_make_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_package/test_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_package/test_parametric_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.985041 tidy3d-2.3.1/tests/test_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47180 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_plugins/test_adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_plugins/test_component_modeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_plugins/test_dispersion_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_plugins/test_mode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_plugins/test_polyslab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_plugins/test_resonance_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_plugins/test_waveguide.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.989041 tidy3d-2.3.1/tests/test_web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_web/mock_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_web/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_web/test_material_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_web/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_web/test_tidy3d_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_web/test_tidy3d_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9391 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_web/test_tidy3d_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/test_web/test_webapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21275 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.989041 tidy3d-2.3.1/tidy3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.993041 tidy3d-2.3.1/tidy3d/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26944 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/boundary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.993041 tidy3d-2.3.1/tidy3d/components/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/data/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14518 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84194 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/data/monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28740 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/data/sim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/field_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   147649 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.993041 tidy3d-2.3.1/tidy3d/components/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18769 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/grid/grid_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47562 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/grid/mesher.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124300 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34086 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121570 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33009 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/components/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.993041 tidy3d-2.3.1/tidy3d/material_library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/material_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62878 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/material_library/material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/material_library/material_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/material_library/parametric_materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.993041 tidy3d-2.3.1/tidy3d/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.993041 tidy3d-2.3.1/tidy3d/plugins/adjoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.997041 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.997041 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17841 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/data/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/data/monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/data/sim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29109 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21387 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22900 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/components/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29884 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/adjoint/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.997041 tidy3d-2.3.1/tidy3d/plugins/dispersion/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/dispersion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/dispersion/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/dispersion/fit_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/dispersion/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.997041 tidy3d-2.3.1/tidy3d/plugins/mode/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/mode/derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26106 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/mode/mode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30578 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/mode/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/mode/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16290 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/mode/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.997041 tidy3d-2.3.1/tidy3d/plugins/polyslab/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/polyslab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/polyslab/polyslab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.997041 tidy3d-2.3.1/tidy3d/plugins/resonance/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/resonance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/resonance/resonance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.997041 tidy3d-2.3.1/tidy3d/plugins/smatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/smatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19900 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/smatrix/smatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.997041 tidy3d-2.3.1/tidy3d/plugins/waveguide/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/waveguide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35912 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/plugins/waveguide/rectangular_dielectric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:34.001042 tidy3d-2.3.1/tidy3d/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)   275233 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:34.001042 tidy3d-2.3.1/tidy3d/web/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/cli/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22414 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/http_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/httputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/material_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/material_libray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/s3utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16788 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/simulation_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26567 2023-07-14 19:13:15.000000 tidy3d-2.3.1/tidy3d/web/webapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:33.989041 tidy3d-2.3.1/tidy3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-07-14 19:13:33.000000 tidy3d-2.3.1/tidy3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-14 19:13:33.000000 tidy3d-2.3.1/tidy3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:13:33.000000 tidy3d-2.3.1/tidy3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 19:13:33.000000 tidy3d-2.3.1/tidy3d.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-14 19:13:33.000000 tidy3d-2.3.1/tidy3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 19:13:33.000000 tidy3d-2.3.1/tidy3d.egg-info/top_level.txt
```

### Comparing `tidy3d-2.3.0rc1/LICENSE` & `tidy3d-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/PKG-INFO` & `tidy3d-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.3.0rc1
+Version: 2.3.1
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Project-URL: Bug Tracker, https://github.com/flexcompute/tidy3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy3d-2.3.0rc1/README.md` & `tidy3d-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/setup.py` & `tidy3d-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/_test_local/_test_adjoint_performance.py` & `tidy3d-2.3.1/tests/_test_local/_test_adjoint_performance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/_test_local/_test_data_performance.py` & `tidy3d-2.3.1/tests/_test_local/_test_data_performance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/_test_local/_test_fit_web.py` & `tidy3d-2.3.1/tests/_test_local/_test_fit_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/_test_local/_test_plugins_web.py` & `tidy3d-2.3.1/tests/_test_local/_test_plugins_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/_test_local/_test_web.py` & `tidy3d-2.3.1/tests/_test_local/_test_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_components/test_IO.py` & `tidy3d-2.3.1/tests/test_components/test_IO.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,21 @@
         if src["type"] == "CustomFieldSource":
             src["field_dataset"] = None
         elif src["type"] == "CustomCurrentSource":
             src["current_dataset"] = None
     for structure in sim_dict["structures"]:
         if structure["geometry"]["type"] == "TriangleMesh":
             structure["geometry"]["mesh_dataset"] = None
+        if "Custom" in structure["medium"]["type"]:
+            if structure["medium"]["type"] == "CustomMedium":
+                structure["medium"]["eps_dataset"] = None
+            elif structure["medium"]["type"] == "CustomPoleResidue":
+                structure["medium"]["poles"] = []
+            else:
+                structure["medium"]["coeffs"] = []
     return td.Simulation.parse_obj(sim_dict)
 
 
 @clear_tmp
 def test_simulation_load_export():
 
     major, minor, patch = __version__.split(".")
```

### Comparing `tidy3d-2.3.0rc1/tests/test_components/test_apodization.py` & `tidy3d-2.3.1/tests/test_components/test_apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_components/test_base.py` & `tidy3d-2.3.1/tests/test_components/test_base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_components/test_boundaries.py` & `tidy3d-2.3.1/tests/test_components/test_boundaries.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_components/test_custom.py` & `tidy3d-2.3.1/tests/test_components/test_custom.py`

 * *Files 14% similar despite different names*

```diff
@@ -235,31 +235,31 @@
 
 def test_medium_interp():
     """Test if the interp works."""
     coord_interp = Coords(**{ax: np.linspace(-2, 2, 20 + ind) for ind, ax in enumerate("xyz")})
 
     # more than one entries per each axis
     orig_data = make_scalar_data()
-    data_fit_nearest = CustomMedium._interp(orig_data, coord_interp, "nearest")
-    data_fit_linear = CustomMedium._interp(orig_data, coord_interp, "linear")
+    data_fit_nearest = coord_interp.spatial_interp(orig_data, "nearest")
+    data_fit_linear = coord_interp.spatial_interp(orig_data, "linear")
     assert np.allclose(data_fit_nearest.shape[:3], [len(f) for f in coord_interp.to_list])
     assert np.allclose(data_fit_linear.shape[:3], [len(f) for f in coord_interp.to_list])
     # maximal or minimal values shouldn't exceed that in the supplied data
     assert max(data_fit_linear.values.ravel()) <= max(orig_data.values.ravel())
     assert min(data_fit_linear.values.ravel()) >= min(orig_data.values.ravel())
     assert max(data_fit_nearest.values.ravel()) <= max(orig_data.values.ravel())
     assert min(data_fit_nearest.values.ravel()) >= min(orig_data.values.ravel())
 
     # single entry along some axis
     Nx = 1
     X = [1.1]
     data = np.random.random((Nx, Ny, Nz, 1))
     orig_data = ScalarFieldDataArray(data, coords=dict(x=X, y=Y, z=Z, f=freqs))
-    data_fit_nearest = CustomMedium._interp(orig_data, coord_interp, "nearest")
-    data_fit_linear = CustomMedium._interp(orig_data, coord_interp, "linear")
+    data_fit_nearest = coord_interp.spatial_interp(orig_data, "nearest")
+    data_fit_linear = coord_interp.spatial_interp(orig_data, "linear")
     assert np.allclose(data_fit_nearest.shape[:3], [len(f) for f in coord_interp.to_list])
     assert np.allclose(data_fit_linear.shape[:3], [len(f) for f in coord_interp.to_list])
     # maximal or minimal values shouldn't exceed that in the supplied data
     assert max(data_fit_linear.values.ravel()) <= max(orig_data.values.ravel())
     assert min(data_fit_linear.values.ravel()) >= min(orig_data.values.ravel())
     assert max(data_fit_nearest.values.ravel()) <= max(orig_data.values.ravel())
     assert min(data_fit_nearest.values.ravel()) >= min(orig_data.values.ravel())
@@ -311,14 +311,23 @@
     meds = CustomMedium.from_nk(n=ns)
     assert med.eps_model(1e14) == meds.eps_model(1e14)
     # lossy
     med = CustomMedium.from_nk(n=n, k=k)
     meds = CustomMedium.from_nk(n=ns, k=ks, freq=freqs[0])
     assert med.eps_model(1e14) == meds.eps_model(1e14)
 
+    # gain
+    with pytest.raises(pydantic.ValidationError):
+        med = CustomMedium.from_nk(n=n, k=-k)
+    with pytest.raises(pydantic.ValidationError):
+        meds = CustomMedium.from_nk(n=ns, k=-ks, freq=freqs[0])
+    med = CustomMedium.from_nk(n=n, k=-k, allow_gain=True)
+    meds = CustomMedium.from_nk(n=ns, k=-ks, freq=freqs[0], allow_gain=True)
+    assert med.eps_model(1e14) == meds.eps_model(1e14)
+
     # inconsistent freq
     with pytest.raises(SetupError):
         med = CustomMedium.from_nk(n=n, k=k, freq=freqs[0] * 1.1)
 
     # missing freq
     with pytest.raises(SetupError):
         med = CustomMedium.from_nk(n=ns, k=ks)
@@ -439,19 +448,19 @@
     with pytest.raises(pydantic.ValidationError):
         sigmatmp = SpatialDataArray(
             np.random.random((Nx, Ny, Nz)) + 0.1j, coords=dict(x=X, y=Y, z=Z)
         )
         mat = CustomMedium(permittivity=permittivity, conductivity=sigmatmp)
 
     # some terms in conductivity are negative
+    sigmatmp = SpatialDataArray(np.random.random((Nx, Ny, Nz)) - 0.5, coords=dict(x=X, y=Y, z=Z))
     with pytest.raises(pydantic.ValidationError):
-        sigmatmp = SpatialDataArray(
-            np.random.random((Nx, Ny, Nz)) - 0.5, coords=dict(x=X, y=Y, z=Z)
-        )
         mat = CustomMedium(permittivity=permittivity, conductivity=sigmatmp)
+    mat = CustomMedium(permittivity=permittivity, conductivity=sigmatmp, allow_gain=True)
+    verify_custom_medium_methods(mat)
 
     # inconsistent coords
     with pytest.raises(pydantic.ValidationError):
         sigmatmp = SpatialDataArray(np.random.random((Nx, Ny, Nz)), coords=dict(x=X + 1, y=Y, z=Z))
         mat = CustomMedium(permittivity=permittivity, conductivity=sigmatmp)
 
     mat = CustomMedium(permittivity=permittivity, conductivity=conductivity)
@@ -487,15 +496,15 @@
     for (a, c) in poles_interp:
         assert a.shape == coord_shape
         assert c.shape == coord_shape
 
 
 def test_custom_pole_residue():
     """Custom pole residue medium."""
-    a = SpatialDataArray(np.random.random((Nx, Ny, Nz)), coords=dict(x=X, y=Y, z=Z))
+    a = SpatialDataArray(-np.random.random((Nx, Ny, Nz)), coords=dict(x=X, y=Y, z=Z))
     c = SpatialDataArray(np.random.random((Nx, Ny, Nz)) * 1j, coords=dict(x=X, y=Y, z=Z))
 
     # some terms in eps_inf are negative
     with pytest.raises(pydantic.ValidationError):
         eps_inf = SpatialDataArray(np.random.random((Nx, Ny, Nz)) - 0.5, coords=dict(x=X, y=Y, z=Z))
         mat = CustomPoleResidue(eps_inf=eps_inf, poles=((a, c),))
 
@@ -509,19 +518,43 @@
     # inconsistent coords of eps_inf with a,c
     with pytest.raises(pydantic.ValidationError):
         eps_inf = SpatialDataArray(
             np.random.random((Nx, Ny, Nz)) + 1, coords=dict(x=X + 1, y=Y, z=Z)
         )
         mat = CustomPoleResidue(eps_inf=eps_inf, poles=((a, c),))
 
+    # break causality
+    with pytest.raises(pydantic.ValidationError):
+        atmp = SpatialDataArray(np.random.random((Nx, Ny, Nz)), coords=dict(x=X, y=Y, z=Z))
+        mat = CustomPoleResidue(eps_inf=xr.ones_like(a), poles=((atmp, c),))
+
     eps_inf = SpatialDataArray(np.random.random((Nx, Ny, Nz)) + 1, coords=dict(x=X, y=Y, z=Z))
     mat = CustomPoleResidue(eps_inf=eps_inf, poles=((a, c),))
     verify_custom_dispersive_medium_methods(mat)
     assert mat.n_cfl > 1
 
+    # to custom non-dispersive medium
+    # dispersive failure
+    with pytest.raises(ValidationError):
+        mat_medium = mat.to_medium()
+    # non-dispersive but gain
+    a = xr.zeros_like(c)
+    mat = CustomPoleResidue(eps_inf=eps_inf, poles=((a, c - 0.1),))
+    with pytest.raises(pydantic.ValidationError):
+        mat_medium = mat.to_medium()
+    mat = CustomPoleResidue(eps_inf=eps_inf, poles=((a, c - 0.1),), allow_gain=True)
+    mat_medium = mat.to_medium()
+    verify_custom_medium_methods(mat_medium)
+    assert mat_medium.n_cfl > 1
+
+    # custom medium to pole residue
+    mat = CustomPoleResidue.from_medium(mat_medium)
+    verify_custom_dispersive_medium_methods(mat)
+    assert mat.n_cfl > 1
+
 
 def test_custom_sellmeier():
     """Custom Sellmeier medium."""
     b1 = SpatialDataArray(np.random.random((Nx, Ny, Nz)), coords=dict(x=X, y=Y, z=Z))
     c1 = SpatialDataArray(np.random.random((Nx, Ny, Nz)), coords=dict(x=X, y=Y, z=Z))
 
     b2 = SpatialDataArray(np.random.random((Nx, Ny, Nz)), coords=dict(x=X, y=Y, z=Z))
@@ -538,14 +571,21 @@
         mat = CustomSellmeier(coeffs=((b1, c1), (b2, ctmp)))
 
     # negative c
     with pytest.raises(pydantic.ValidationError):
         ctmp = SpatialDataArray(np.random.random((Nx, Ny, Nz)) - 0.5, coords=dict(x=X, y=Y, z=Z))
         mat = CustomSellmeier(coeffs=((b1, c1), (b2, ctmp)))
 
+    # negative b
+    btmp = SpatialDataArray(np.random.random((Nx, Ny, Nz)) - 0.5, coords=dict(x=X, y=Y, z=Z))
+    with pytest.raises(pydantic.ValidationError):
+        mat = CustomSellmeier(coeffs=((b1, c1), (btmp, c2)))
+    mat = CustomSellmeier(coeffs=((b1, c1), (btmp, c2)), allow_gain=True)
+    assert mat.pole_residue.allow_gain
+
     # inconsistent coord
     with pytest.raises(pydantic.ValidationError):
         btmp = SpatialDataArray(np.random.random((Nx, Ny, Nz)), coords=dict(x=X + 1, y=Y, z=Z))
         mat = CustomSellmeier(coeffs=((b1, c2), (btmp, c2)))
 
     mat = CustomSellmeier(coeffs=((b1, c1), (b2, c2)))
     verify_custom_dispersive_medium_methods(mat)
@@ -582,17 +622,37 @@
         mat = CustomLorentz(eps_inf=eps_inf, coeffs=((de1, f1, delta1), (de2, f2, deltatmp)))
 
     # inconsistent coords
     with pytest.raises(pydantic.ValidationError):
         ftmp = SpatialDataArray(1 + np.random.random((Nx, Ny, Nz)), coords=dict(x=X + 1, y=Y, z=Z))
         mat = CustomLorentz(eps_inf=eps_inf, coeffs=((de1, f1, delta1), (de2, ftmp, delta2)))
 
-    mat = CustomLorentz(eps_inf=eps_inf, coeffs=((de1, f1, delta1), (de2, f2, delta2)))
+    # break causality with negative delta
+    with pytest.raises(pydantic.ValidationError):
+        deltatmp = SpatialDataArray(
+            np.random.random((Nx, Ny, Nz)) - 0.5, coords=dict(x=X, y=Y, z=Z)
+        )
+        mat = CustomLorentz(eps_inf=eps_inf, coeffs=((de1, f1, delta1), (de2, f2, deltatmp)))
+
+    # gain medium with negative delta epsilon
+    with pytest.raises(pydantic.ValidationError):
+        detmp = SpatialDataArray(np.random.random((Nx, Ny, Nz)) - 0.5, coords=dict(x=X, y=Y, z=Z))
+        mat = CustomLorentz(eps_inf=eps_inf, coeffs=((de1, f1, delta1), (detmp, f2, delta2)))
+    mat = CustomLorentz(
+        eps_inf=eps_inf, coeffs=((de1, f1, delta1), (detmp, f2, delta2)), allow_gain=True
+    )
+    verify_custom_dispersive_medium_methods(mat)
+    assert mat.n_cfl > 1
+
+    mat = CustomLorentz(
+        eps_inf=eps_inf, coeffs=((de1, f1, delta1), (de2, f2, delta2)), subpixel=True
+    )
     verify_custom_dispersive_medium_methods(mat)
     assert mat.n_cfl > 1
+    assert mat.pole_residue.subpixel
 
 
 def test_custom_drude():
     """Custom Drude medium."""
     eps_inf = SpatialDataArray(np.random.random((Nx, Ny, Nz)) + 1, coords=dict(x=X, y=Y, z=Z))
 
     f1 = SpatialDataArray(1 + np.random.random((Nx, Ny, Nz)), coords=dict(x=X, y=Y, z=Z))
@@ -651,20 +711,28 @@
         mat = CustomDebye(eps_inf=eps_inf, coeffs=((eps1, tau1), (eps2, tautmp)))
 
     # inconsistent coords
     with pytest.raises(pydantic.ValidationError):
         epstmp = SpatialDataArray(np.random.random((Nx, Ny, Nz)), coords=dict(x=X + 1, y=Y, z=Z))
         mat = CustomDebye(eps_inf=eps_inf, coeffs=((eps1, tau1), (epstmp, tau2)))
 
+    # negative delta epsilon
+    with pytest.raises(pydantic.ValidationError):
+        epstmp = SpatialDataArray(np.random.random((Nx, Ny, Nz)) - 0.5, coords=dict(x=X, y=Y, z=Z))
+        mat = CustomDebye(eps_inf=eps_inf, coeffs=((eps1, tau1), (epstmp, tau2)))
+    mat = CustomDebye(eps_inf=eps_inf, coeffs=((eps1, tau1), (epstmp, tau2)), allow_gain=True)
+    verify_custom_dispersive_medium_methods(mat)
+    assert mat.n_cfl > 1
+
     mat = CustomDebye(eps_inf=eps_inf, coeffs=((eps1, tau1), (eps2, tau2)))
     verify_custom_dispersive_medium_methods(mat)
     assert mat.n_cfl > 1
 
 
-def test_custom_anisotropic_medium():
+def test_custom_anisotropic_medium(log_capture):
     """Custom anisotropic medium."""
 
     # xx
     permittivity = SpatialDataArray(1 + np.random.random((Nx, Ny, Nz)), coords=dict(x=X, y=Y, z=Z))
     conductivity = SpatialDataArray(np.random.random((Nx, Ny, Nz)), coords=dict(x=X, y=Y, z=Z))
     mat_xx = CustomMedium(permittivity=permittivity, conductivity=conductivity)
 
@@ -684,14 +752,17 @@
     delta2 = SpatialDataArray(np.random.random((Nx, Ny, Nz)), coords=dict(x=X, y=Y, z=Z))
     mat_zz = CustomDrude(eps_inf=eps_inf, coeffs=((f1, delta1), (f2, delta2)))
 
     # anisotropic
     mat = CustomAnisotropicMedium(xx=mat_xx, yy=mat_yy, zz=mat_zz)
     verify_custom_medium_methods(mat)
 
+    mat = CustomAnisotropicMedium(xx=mat_xx, yy=mat_yy, zz=mat_zz, subpixel=True)
+    assert_log_level(log_capture, "WARNING")
+
     ## interpolation method verification for "xx" component
     # 1) xx-component is using `interp_method = nearest`, and mat using `None`;
     # so that xx-component is using "nearest"
     freq = 2e14
     dist_coeff = 0.6
     coord_test = Coords(x=[X[0] * dist_coeff + X[1] * (1 - dist_coeff)], y=Y[0], z=Z[0])
     eps_nearest = mat.eps_sigma_to_eps_complex(
```

### Comparing `tidy3d-2.3.0rc1/tests/test_components/test_field_projection.py` & `tidy3d-2.3.1/tests/test_components/test_field_projection.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         Ephi=scalar_field_u,
         Hr=scalar_field_u,
         Htheta=scalar_field_u,
         Hphi=scalar_field_u,
     )
 
     sim = td.Simulation(
-        size=(7, 7, 7),
+        size=(7, 7, 9),
         grid_spec=td.GridSpec.auto(wavelength=5.0),
         monitors=[monitor_xy, monitor_u, monitor_tp],
         run_time=1e-12,
     )
 
     sim_data = td.SimulationData(simulation=sim, data=(data_xy, data_u, data_tp))
     sim_data[monitor_xy.name]
```

### Comparing `tidy3d-2.3.0rc1/tests/test_components/test_geometry.py` & `tidy3d-2.3.1/tests/test_components/test_geometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -411,14 +411,42 @@
     polyslabs_gap = make_polyslabs(gap_size=0.3)
     assert len(polyslabs_gap) == 2, "untouching polylsabs were merged incorrectly."
 
     polyslabs_touching = make_polyslabs(gap_size=0)
     assert len(polyslabs_touching) == 1, "polyslabs didnt merge correctly."
 
 
+def test_polyslab_side_plot_merge():
+    """In side plot, make sure splitted polygons merge."""
+    x0 = 2
+    y0 = 4
+    z0 = 1
+    R = 5
+    wg_width = 0.5
+    wg_thickness = 0.22
+    sidewall_angle = 15 * np.pi / 180
+
+    cell = gdstk.Cell("bottom")
+    path_bottom = gdstk.RobustPath(
+        (x0 + R, y0), wg_width - wg_thickness * np.tan(np.abs(sidewall_angle)), layer=1, datatype=0
+    )
+
+    path_bottom.arc(R, 0, -np.pi)
+    cell.add(path_bottom)
+    ring_bottom_geo = td.PolySlab.from_gds(
+        cell,
+        gds_layer=1,
+        axis=2,
+        slab_bounds=(z0 - wg_thickness / 2, z0 + wg_thickness / 2),
+        sidewall_angle=sidewall_angle,
+        reference_plane="top",
+    )
+    assert len(ring_bottom_geo[0].intersections_plane(x=2)) == 1
+
+
 @pytest.mark.parametrize("axis", [0, 1, 2])
 def test_polyslab_axis(axis):
     ps = td.PolySlab(slab_bounds=(-1, 1), vertices=((-5, -5), (-5, 5), (5, 5), (5, -5)), axis=axis)
 
     # bound test
     bounds_ideal = [-5, -5]
     bounds_ideal.insert(axis, -1)
```

### Comparing `tidy3d-2.3.0rc1/tests/test_components/test_grid.py` & `tidy3d-2.3.1/tests/test_components/test_grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_components/test_grid_spec.py` & `tidy3d-2.3.1/tests/test_components/test_grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_components/test_medium.py` & `tidy3d-2.3.1/tests/test_components/test_medium.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Tests mediums."""
 import numpy as np
 import pytest
 import pydantic
 import matplotlib.pylab as plt
 import tidy3d as td
 from tidy3d.exceptions import ValidationError
+from ..utils import assert_log_level, log_capture
 from typing import Dict
 
 MEDIUM = td.Medium()
 ANIS_MEDIUM = td.AnisotropicMedium(xx=MEDIUM, yy=MEDIUM, zz=MEDIUM)
 PEC = td.PECMedium()
-PR = td.PoleResidue(poles=[(1 + 1j, 2 + 2j)])
+PR = td.PoleResidue(poles=[(-1 + 1j, 2 + 2j)])
 SM = td.Sellmeier(coeffs=[(1, 2)])
 LZ = td.Lorentz(coeffs=[(1, 2, 3)])
 DR = td.Drude(coeffs=[(1, 2)])
 DB = td.Debye(coeffs=[(1, 2)])
 MEDIUMS = [MEDIUM, ANIS_MEDIUM, PEC, PR, SM, LZ, DR, DB]
 
 f, AX = plt.subplots()
@@ -83,15 +84,15 @@
 
     struct = td.Structure(geometry=td.Box(size=(1, 1, 1)), medium=td.PEC)
 
 
 def test_medium_dispersion():
 
     # construct media
-    m_PR = td.PoleResidue(eps_inf=1.0, poles=[((1 + 2j), (1 + 3j)), ((2 + 4j), (1 + 5j))])
+    m_PR = td.PoleResidue(eps_inf=1.0, poles=[((-1 + 2j), (1 + 3j)), ((-2 + 4j), (1 + 5j))])
     m_SM = td.Sellmeier(coeffs=[(2, 3), (2, 4)])
     m_LZ = td.Lorentz(eps_inf=1.0, coeffs=[(1, 3, 2), (2, 4, 1)])
     m_LZ2 = td.Lorentz(eps_inf=1.0, coeffs=[(1, 2, 3), (2, 1, 4)])
     m_DR = td.Drude(eps_inf=1.0, coeffs=[(1, 3), (2, 4)])
     m_DB = td.Debye(eps_inf=1.0, coeffs=[(1, 3), (2, 4)])
 
     with pytest.raises(pydantic.ValidationError) as e_info:
@@ -110,15 +111,15 @@
     for medium in [m_SM, m_LZ, m_LZ2, m_DR, m_DB]:
         eps_c = medium.eps_model(freqs)
         assert np.all(eps_c.imag >= 0)
 
 
 def test_medium_dispersion_conversion():
 
-    m_PR = td.PoleResidue(eps_inf=1.0, poles=[((1 + 2j), (1 + 3j)), ((2 + 4j), (1 + 5j))])
+    m_PR = td.PoleResidue(eps_inf=1.0, poles=[((-1 + 2j), (1 + 3j)), ((-2 + 4j), (1 + 5j))])
     m_SM = td.Sellmeier(coeffs=[(2, 3), (2, 4)])
     m_LZ = td.Lorentz(eps_inf=1.0, coeffs=[(1, 3, 2), (2, 4, 1)])
     m_LZ2 = td.Lorentz(eps_inf=1.0, coeffs=[(1, 2, 3), (2, 1, 4)])
     m_DR = td.Drude(eps_inf=1.0, coeffs=[(1, 3), (2, 4)])
     m_DB = td.Debye(eps_inf=1.0, coeffs=[(1, 3), (2, 4)])
 
     freqs = np.linspace(0.01, 1, 1001)
@@ -126,15 +127,15 @@
         eps_model = medium.eps_model(freqs)
         eps_pr = medium.pole_residue.eps_model(freqs)
         np.testing.assert_allclose(eps_model, eps_pr)
 
 
 def test_medium_dispersion_create():
 
-    m_PR = td.PoleResidue(eps_inf=1.0, poles=[((1 + 2j), (1 + 3j)), ((2 + 4j), (1 + 5j))])
+    m_PR = td.PoleResidue(eps_inf=1.0, poles=[((-1 + 2j), (1 + 3j)), ((-2 + 4j), (1 + 5j))])
     m_SM = td.Sellmeier(coeffs=[(2, 3), (2, 4)])
     m_LZ = td.Lorentz(eps_inf=1.0, coeffs=[(1, 3, 2), (2, 4, 1)])
     m_LZ2 = td.Lorentz(eps_inf=1.0, coeffs=[(1, 2, 3), (2, 1, 4)])
     m_DR = td.Drude(eps_inf=1.0, coeffs=[(1, 3), (2, 4)])
     m_DB = td.Debye(eps_inf=1.0, coeffs=[(1, 3), (2, 4)])
 
     for medium in [m_PR, m_SM, m_DB, m_LZ, m_DR, m_LZ2]:
@@ -252,25 +253,68 @@
     assert material.n_cfl == 2
     # PEC
     assert PEC.n_cfl == 1
     # anisotropic
     material = td.AnisotropicMedium(xx=MEDIUM, yy=td.Medium(permittivity=4), zz=MEDIUM)
     assert material.n_cfl == 1
     # dispersive
-    material = td.PoleResidue(eps_inf=0.16, poles=[(1 + 1j, 2 + 2j)])
+    material = td.PoleResidue(eps_inf=0.16, poles=[(-1 + 1j, 2 + 2j)])
     assert material.n_cfl == 0.4
     assert SM.n_cfl == 1
     material = td.Lorentz(eps_inf=0.04, coeffs=[(1, 2, 3)])
     assert material.n_cfl == 0.2
     material = td.Drude(eps_inf=4, coeffs=[(1, 2)])
     assert material.n_cfl == 2
     material = td.Debye(eps_inf=4, coeffs=[(1, 2)])
     assert material.n_cfl == 2
 
 
+def test_gain_medium(log_capture):
+    """Test passive and gain medium validations."""
+    # non-dispersive
+    with pytest.raises(pydantic.ValidationError) as e_info:
+        m = td.Medium(conductivity=-0.1)
+    with pytest.raises(pydantic.ValidationError) as e_info:
+        m = td.Medium(conductivity=-1.0, allow_gain=False)
+    mM = td.Medium(conductivity=-1.0, allow_gain=True)
+
+    # pole residue, causality
+    with pytest.raises(pydantic.ValidationError) as e_info:
+        m = td.PoleResidue(eps_inf=0.16, poles=[(1 + 1j, 2 + 2j)])
+
+    # Sellmeier
+    with pytest.raises(pydantic.ValidationError) as e_info:
+        m = td.Sellmeier(coeffs=((-1, 1),))
+    mS = td.Sellmeier(coeffs=((-1, 1),), allow_gain=True)
+
+    # Lorentz
+    # causality, negative gamma
+    with pytest.raises(pydantic.ValidationError) as e_info:
+        m = td.Lorentz(eps_inf=0.04, coeffs=[(1, 2, -3)])
+    # gain, negative Delta epsilon
+    with pytest.raises(pydantic.ValidationError) as e_info:
+        m = td.Lorentz(eps_inf=0.04, coeffs=[(-1, 2, 3)])
+    mL = td.Lorentz(eps_inf=0.04, coeffs=[(-1, 2, 3)], allow_gain=True)
+    assert mL.pole_residue.allow_gain
+
+    # f_i can take whatever sign
+    m = td.Lorentz(eps_inf=0.04, coeffs=[(1, -2, 3)])
+
+    # Drude, only causality constraint
+    with pytest.raises(pydantic.ValidationError) as e_info:
+        m = td.Drude(eps_inf=0.04, coeffs=[(1, -2)])
+
+    # anisotropic medium, warn allow_gain is ignored
+    m = td.AnisotropicMedium(xx=td.Medium(), yy=mL, zz=mS, allow_gain=True)
+    assert_log_level(log_capture, "WARNING")
+
+    m = td.AnisotropicMedium(xx=td.Medium(), yy=mL, zz=mS, allow_gain=False)
+    assert_log_level(log_capture, "WARNING")
+
+
 def test_medium2d():
     sigma = 0.45
     thickness = 0.01
     cond_med = td.Medium(conductivity=sigma)
     medium = td.Medium2D.from_medium(cond_med, thickness=thickness)
 
     _ = medium.plot(freqs=[2e14, 3e14], ax=AX)
@@ -337,14 +381,15 @@
         td.FullyAnisotropicMedium(permittivity=[3, 4, 2])
 
     # check that permittivity >= 1 and conductivity >= 0
     with pytest.raises(pydantic.ValidationError):
         td.FullyAnisotropicMedium(permittivity=[[3, 0, 0], [0, 0.5, 0], [0, 0, 1]])
     with pytest.raises(pydantic.ValidationError):
         td.FullyAnisotropicMedium(conductivity=[[-3, 0, 0], [0, 0.5, 0], [0, 0, 1]])
+    td.FullyAnisotropicMedium(conductivity=[[-3, 0, 0], [0, 0.5, 0], [0, 0, 1]], allow_gain=True)
 
     # check that permittivity needs to be symmetric
     with pytest.raises(pydantic.ValidationError):
         td.FullyAnisotropicMedium(permittivity=[[3, 0.1, 0], [0.2, 2, 0], [0, 0, 1]])
 
     # check that differently oriented permittivity and conductivity are not accepted
     with pytest.raises(pydantic.ValidationError):
```

### Comparing `tidy3d-2.3.0rc1/tests/test_components/test_meshgenerate.py` & `tidy3d-2.3.1/tests/test_components/test_meshgenerate.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_components/test_mode.py` & `tidy3d-2.3.1/tests/test_components/test_mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_components/test_monitor.py` & `tidy3d-2.3.1/tests/test_components/test_monitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,20 @@
 
 def test_excluded_surfaces_flat():
 
     with pytest.raises(pydantic.ValidationError):
         M = td.FluxMonitor(size=(1, 1, 0), name="f", freqs=[1e12], exclude_surfaces=("x-",))
 
 
+def test_fld_mnt_freqs_none():
+    """Test that validation errors if freqs=[None]."""
+    with pytest.raises(pydantic.ValidationError):
+        td.FieldMonitor(center=(0, 0, 0), size=(0, 0, 0), freqs=[None], name="test")
+
+
 def test_integration_surfaces():
     # test that integration surfaces are extracted correctly for surface and volume
     # integration monitors
 
     # surface monitor
     surfaces = td.FieldProjectionAngleMonitor(
         size=(2, 0, 2), theta=[1, 2], phi=[0], name="f", freqs=[2e12]
@@ -108,14 +114,34 @@
 
     M = td.FieldProjectionAngleMonitor(
         size=(2, 2, 2), theta=[1], phi=[0], name="f", freqs=[2e12], exclude_surfaces=["x-", "y+"]
     ).projection_surfaces
     assert len(M) == 4
 
 
+def test_fieldproj_surfaces_in_simulaiton():
+    # test error if a projection surfaces is outside the simulation domain
+    M = td.FieldProjectionAngleMonitor(size=(1, 3, 3), theta=[1], phi=[0], name="f", freqs=[2e12])
+    with pytest.raises(pydantic.ValidationError):
+        sim = td.Simulation(
+            size=(2, 2, 2),
+            run_time=1e-12,
+            monitors=[M],
+            grid_spec=td.GridSpec.uniform(0.1),
+        )
+    # no error when outside surfaces are excluded
+    M = M.updated_copy(exclude_surfaces=["y-", "y+", "z-", "z+"])
+    sim = td.Simulation(
+        size=(2, 2, 2),
+        run_time=1e-12,
+        monitors=[M],
+        grid_spec=td.GridSpec.uniform(0.1),
+    )
+
+
 def test_fieldproj_kspace_range():
     # make sure ux, uy are in [-1, 1] for k-space projection monitors
     with pytest.raises(pydantic.ValidationError):
         M = td.FieldProjectionKSpaceMonitor(
             size=(2, 0, 2), ux=[0.1, 2], uy=[0], name="f", freqs=[2e12], proj_axis=1
         )
     with pytest.raises(pydantic.ValidationError):
@@ -206,14 +232,15 @@
     with pytest.raises(pydantic.ValidationError) as e_info:
         sim = td.Simulation(
             size=(2, 2, 2),
             run_time=1e-12,
             structures=[td.Structure(geometry=td.Box(size=(1, 1, 1)), medium=td.Medium())],
             boundary_spec=boundary_spec,
             monitors=[td.DiffractionMonitor(size=[td.inf, td.inf, 0], freqs=[1e12], name="de")],
+            grid_spec=td.GridSpec.uniform(dl=0.1),
         )
 
     # ensure error if monitor isn't infinite in two directions
     with pytest.raises(pydantic.ValidationError) as e_info:
         monitor = td.DiffractionMonitor(size=[td.inf, 4, 0], freqs=[1e12], name="de")
 
 
@@ -227,15 +254,20 @@
     m2 = td.FieldTimeMonitor(size=size, center=center, name="test_mon")
     m3 = td.FluxMonitor(size=(1, 1, 0), center=center, freqs=[1, 2, 3], name="test_mon")
     m4 = td.FluxTimeMonitor(size=(1, 1, 0), center=center, name="test_mon")
     m5 = td.ModeMonitor(
         size=(1, 1, 0), center=center, mode_spec=td.ModeSpec(), freqs=[1, 2, 3], name="test_mon"
     )
     m6 = td.ModeSolverMonitor(
-        size=(1, 1, 0), center=center, mode_spec=td.ModeSpec(), freqs=[1, 2, 3], name="test_mon"
+        size=(1, 1, 0),
+        center=center,
+        mode_spec=td.ModeSpec(),
+        freqs=[1, 2, 3],
+        name="test_mon",
+        direction="-",
     )
     m7 = td.PermittivityMonitor(size=size, center=center, freqs=[1, 2, 3], name="perm")
 
     tmesh = np.linspace(0, 1, 10)
 
     for m in [m1, m2, m3, m4, m5, m6, m7]:
         # m.plot(y=2)
```

### Comparing `tidy3d-2.3.0rc1/tests/test_components/test_sidewall.py` & `tidy3d-2.3.1/tests/test_components/test_sidewall.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_components/test_simulation.py` & `tidy3d-2.3.1/tests/test_components/test_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,57 +107,59 @@
                 source_time=td.GaussianPulse(freq0=2e14, fwidth=1e14),
             )
         ],
     )
     assert_log_level(log_capture, None)
 
 
-def test_sim_bounds():
+@pytest.mark.parametrize("shift_amount, log_level", ((1, None), (2, "WARNING")))
+def test_sim_bounds(shift_amount, log_level, log_capture):
     """make sure bounds are working correctly"""
 
     # make sure all things are shifted to this central location
     CENTER_SHIFT = (-1.0, 1.0, 100.0)
 
     def place_box(center_offset):
 
         shifted_center = tuple(c + s for (c, s) in zip(center_offset, CENTER_SHIFT))
 
         sim = td.Simulation(
-            size=(1, 1, 1),
+            size=(1.5, 1.5, 1.5),
             center=CENTER_SHIFT,
             grid_spec=td.GridSpec(wavelength=1.0),
             run_time=1e-12,
             structures=[
                 td.Structure(
                     geometry=td.Box(size=(1, 1, 1), center=shifted_center), medium=td.Medium()
                 )
             ],
             boundary_spec=td.BoundarySpec.all_sides(boundary=td.Periodic()),
+            sources=[
+                td.PointDipole(
+                    center=CENTER_SHIFT,
+                    polarization="Ex",
+                    source_time=td.GaussianPulse(freq0=td.C_0, fwidth=td.C_0),
+                )
+            ],
         )
 
     # create all permutations of squares being shifted 1, -1, or zero in all three directions
     bin_strings = [list(format(i, "03b")) for i in range(8)]
     bin_ints = [[int(b) for b in bin_string] for bin_string in bin_strings]
     bin_ints = np.array(bin_ints)
     bin_signs = 2 * (bin_ints - 0.5)
 
     # test all cases where box is shifted +/- 1 in x,y,z and still intersects
     for amp in bin_ints:
         for sign in bin_signs:
-            center = amp * sign
-            place_box(tuple(center))
-
-    # test all cases where box is shifted +/- 2 in x,y,z and no longer intersects
-    for amp in bin_ints:
-        for sign in bin_signs:
-            center = 2 * amp * sign
+            center = shift_amount * amp * sign
             if np.sum(center) < 1e-12:
                 continue
-            with pytest.raises(pydantic.ValidationError) as e_info:
-                place_box(tuple(center))
+            place_box(tuple(center))
+    assert_log_level(log_capture, log_level)
 
 
 def test_sim_size():
 
     # note dl may need to change if we change the maximum allowed number of cells
     mesh1d = td.UniformGrid(dl=2e-4)
     grid_spec = td.GridSpec(grid_x=mesh1d, grid_y=mesh1d, grid_z=mesh1d)
@@ -1457,15 +1459,15 @@
         grid_spec=td.GridSpec.uniform(dl=0.1),
     )
     dt = sim.dt
 
     # simulation with eps_inf < 1
     structure = td.Structure(
         geometry=td.Box(size=(1, 1, 1), center=(-1, 0, 0)),
-        medium=td.PoleResidue(eps_inf=0.16, poles=[(1 + 1j, 2 + 2j)]),
+        medium=td.PoleResidue(eps_inf=0.16, poles=[(-1 + 1j, 2 + 2j)]),
     )
     sim_new = sim.copy(update=dict(structures=[structure]))
     assert sim_new.dt == 0.4 * dt
 
 
 @clear_tmp
 def test_sim_volumetric_structures():
@@ -1648,7 +1650,38 @@
         boundary_spec=td.BoundarySpec.pml(**pml_on_kwargs),
     )
 
     pml_boxes = sim2d._make_pml_boxes(normal_axis=normal_axis)
 
     for pml_box in pml_boxes:
         assert pml_box.size[normal_axis] > 0, "PML box has size of 0 in normal direction of 2D sim."
+
+
+def test_allow_gain():
+    """Test if simulation allows gain."""
+
+    medium = td.Medium(permittivity=2.0)
+    medium_gain = td.Medium(permittivity=2.0, allow_gain=True)
+    medium_ani = td.AnisotropicMedium(xx=medium, yy=medium, zz=medium)
+    medium_gain_ani = td.AnisotropicMedium(xx=medium, yy=medium_gain, zz=medium)
+
+    # Test simulation medium
+    sim = td.Simulation(
+        size=(10, 10, 10), run_time=1e-12, medium=medium, grid_spec=td.GridSpec.uniform(dl=0.1)
+    )
+    assert not sim.allow_gain
+    sim = sim.updated_copy(medium=medium_gain)
+    assert sim.allow_gain
+
+    # Test structure with anisotropic gain medium
+    struct = td.Structure(geometry=td.Box(center=(0, 0, 0), size=(1, 1, 1)), medium=medium_ani)
+    struct_gain = struct.updated_copy(medium=medium_gain_ani)
+    sim = td.Simulation(
+        size=(1, 1, 1),
+        run_time=1e-12,
+        medium=medium,
+        grid_spec=td.GridSpec.uniform(dl=0.1),
+        structures=[struct],
+    )
+    assert not sim.allow_gain
+    sim = sim.updated_copy(structures=[struct_gain])
+    assert sim.allow_gain
```

### Comparing `tidy3d-2.3.0rc1/tests/test_components/test_source.py` & `tidy3d-2.3.1/tests/test_components/test_source.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,15 +37,18 @@
 
 
 def test_UniformCurrentSource():
 
     g = td.GaussianPulse(freq0=1, fwidth=0.1)
 
     # test we can make generic UniformCurrentSource
-    s = td.UniformCurrentSource(size=(1, 1, 1), source_time=g, polarization="Ez")
+    s1 = td.UniformCurrentSource(
+        size=(1, 1, 1), source_time=g, polarization="Ez", interpolate=False
+    )
+    s2 = td.UniformCurrentSource(size=(1, 1, 1), source_time=g, polarization="Ez", interpolate=True)
 
 
 def test_source_times():
 
     # test we can make gaussian pulse
     g = td.GaussianPulse(freq0=1, fwidth=0.1)
     ts = np.linspace(0, 30, 1001)
@@ -59,15 +62,16 @@
     ts = np.linspace(0, 30, 1001)
     c.amp_time(ts)
 
 
 def test_dipole():
 
     g = td.GaussianPulse(freq0=1, fwidth=0.1)
-    p = td.PointDipole(center=(1, 2, 3), source_time=g, polarization="Ex")
+    p1 = td.PointDipole(center=(1, 2, 3), source_time=g, polarization="Ex", interpolate=True)
+    p2 = td.PointDipole(center=(1, 2, 3), source_time=g, polarization="Ex", interpolate=False)
     # p.plot(y=2)
 
     with pytest.raises(pydantic.ValidationError) as e_info:
         p = td.PointDipole(size=(1, 1, 1), source_time=g, center=(1, 2, 3), polarization="Ex")
 
 
 def test_FieldSource():
```

### Comparing `tidy3d-2.3.0rc1/tests/test_components/test_types.py` & `tidy3d-2.3.1/tests/test_components/test_types.py`

 * *Files 19% similar despite different names*

```diff
@@ -59,14 +59,38 @@
     assert np.all(my_obj.b == [1.0, 2.0])  # numpy arrays converted tolist()
     assert np.all(my_obj.c == [1.0, 3.0])  # converted to float
     assert np.all(my_obj.d == [1.0 + 0.0j])  # converted to complex
 
     my_obj.json()
 
 
+def test_array_like_field_name():
+    class MyClass(Tidy3dBaseModel):
+
+        a: ArrayLike  # can be any array-like thing
+        b: constrained_array(ndim=2)  # must be 2D
+        c: constrained_array(dtype=float)  # must be float-like
+        d: constrained_array(ndim=1, dtype=complex)  # 1D complex
+        e: constrained_array(ndim=3, shape=(1, 2, 3))  # must have certain shape
+        f: ArrayLike = None
+
+    fields = MyClass.__fields__
+
+    def correct_field_display(field_name, display_name):
+        """Make sure the field has the expected name."""
+        assert fields[field_name]._type_display() == display_name
+
+    correct_field_display("a", "ArrayLike")
+    correct_field_display("b", "ArrayLike[ndim=2]")
+    correct_field_display("c", "ArrayLike[dtype=float]")
+    correct_field_display("d", "ArrayLike[dtype=complex, ndim=1]")
+    correct_field_display("e", "ArrayLike[ndim=3, shape=(1, 2, 3)]")
+    correct_field_display("f", "Optional[ArrayLike]")
+
+
 def test_hash():
     class MyClass(Tidy3dBaseModel):
 
         a: ArrayLike
         b: constrained_array(ndim=1)
         c: Tuple[ArrayLike, ...]
```

### Comparing `tidy3d-2.3.0rc1/tests/test_data/test_data_arrays.py` & `tidy3d-2.3.1/tests/test_data/test_data_arrays.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_data/test_monitor_data.py` & `tidy3d-2.3.1/tests/test_data/test_monitor_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -248,14 +248,28 @@
     fields = field_data.field_components.items()
     fields_single_f = {key: val.isel(f=[0]).assign_coords(f=[freq]) for key, val in fields}
     field_data = field_data.copy(update=fields_single_f)
     dot = data.dot(field_data)
     # Check that broadcasting worked
     assert data.Ex.f == dot.f
     assert data.Ex.mode_index == dot.mode_index
+    # Check eps_spec validator
+    num_freqs = len(data.monitor.freqs)
+    data_eps_spec = data.updated_copy(eps_spec=["diagonal"] * num_freqs)
+    data_eps_spec = data.updated_copy(eps_spec=["tensorial_real"] * num_freqs)
+    data_eps_spec = data.updated_copy(eps_spec=["tensorial_complex"] * num_freqs)
+    # wrong keyword
+    with pytest.raises(pydantic.ValidationError):
+        data_eps_spec = data.updated_copy(eps_spec=["tensorial"] * num_freqs)
+    # wrong number
+    with pytest.raises(pydantic.ValidationError):
+        data_eps_spec = data.updated_copy(eps_spec=["diagonal"] * (num_freqs + 1))
+    # check monitor direction changes upon time reversal
+    data_reversed = data.time_reversed_copy
+    assert data_reversed.monitor.direction == "-"
 
 
 def test_permittivity_data():
     data = make_permittivity_data()
     for comp in "xyz":
         _ = getattr(data, "eps_" + comp + comp)
 
@@ -506,7 +520,16 @@
     tan_fields = mode_data._tangential_fields
     # Check that data is only slightly different
     for comp, field in mode_data.field_components.items():
         if comp in tan_fields.keys():
             max_diff = np.amax(np.abs(np.abs(field) - np.abs(tan_fields[comp])))
             max_diff /= np.amax(np.abs(field))
             assert 0.1 > max_diff > 0
+
+
+def test_outer_dot():
+    mode_data = make_mode_solver_data()
+    field_data = make_field_data_2d()
+    _ = mode_data.outer_dot(mode_data)
+    _ = field_data.outer_dot(mode_data)
+    _ = mode_data.outer_dot(field_data)
+    _ = field_data.outer_dot(field_data)
```

### Comparing `tidy3d-2.3.0rc1/tests/test_data/test_sim_data.py` & `tidy3d-2.3.1/tests/test_data/test_sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_package/test_config.py` & `tidy3d-2.3.1/tests/test_package/test_config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_package/test_log.py` & `tidy3d-2.3.1/tests/test_package/test_log.py`

 * *Files 13% similar despite different names*

```diff
@@ -63,28 +63,27 @@
     wavelength = 1
     f0 = td.C_0 / wavelength
     fwidth = f0 / 10.0
     source_time = td.GaussianPulse(freq0=f0, fwidth=fwidth)
     run_time = 10 / fwidth
     freqs = np.linspace(f0 - fwidth, f0 + fwidth, 11)
 
-    # 1 warning: "group_index_step" with single precision
     mode_mnt = td.ModeMonitor(
         center=(0, 0, 0),
         size=(domain_size, 0, domain_size),
         freqs=list(freqs),
-        mode_spec=td.ModeSpec(num_modes=3, group_index_step=1),
+        mode_spec=td.ModeSpec(num_modes=3),
         name="mode",
     )
 
-    # 2 warnings: "group_index_step" with single precision, too high num_freqs
+    # 1 warning: too high num_freqs
     mode_source = td.ModeSource(
         size=(domain_size, 0, domain_size),
         source_time=source_time,
-        mode_spec=td.ModeSpec(num_modes=2, group_index_step=1, precision="single"),
+        mode_spec=td.ModeSpec(num_modes=2, precision="single"),
         mode_index=1,
         num_freqs=50,
         direction="-",
     )
 
     # 1 warning: ignoring "normal_dir"
     monitor_flux = td.FluxMonitor(
@@ -126,9 +125,9 @@
 
     # parse the entire simulation at once to capture warnings hierarchically
     sim_json = sim.json()
 
     td.log.set_capture(True)
     sim = td.Simulation.parse_raw(sim_json)
     warning_list = td.log.captured_warnings()
-    assert len(warning_list) == 17
+    assert len(warning_list) == 15
     td.log.set_capture(False)
```

### Comparing `tidy3d-2.3.0rc1/tests/test_package/test_make_script.py` & `tidy3d-2.3.1/tests/test_package/test_make_script.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_package/test_material_library.py` & `tidy3d-2.3.1/tests/test_package/test_material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_plugins/test_adjoint.py` & `tidy3d-2.3.1/tests/test_plugins/test_adjoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,33 +15,37 @@
 
 import tidy3d as td
 from typing import Tuple, Any, List
 
 from tidy3d.exceptions import DataError, Tidy3dKeyError, AdjointError
 from tidy3d.plugins.adjoint.components.base import JaxObject
 from tidy3d.plugins.adjoint.components.geometry import JaxBox, JaxPolySlab, MAX_NUM_VERTICES
+from tidy3d.plugins.adjoint.components.geometry import JaxGeometryGroup
 from tidy3d.plugins.adjoint.components.medium import JaxMedium, JaxAnisotropicMedium
 from tidy3d.plugins.adjoint.components.medium import JaxCustomMedium, MAX_NUM_CELLS_CUSTOM_MEDIUM
 from tidy3d.plugins.adjoint.components.structure import JaxStructure
 from tidy3d.plugins.adjoint.components.simulation import JaxSimulation, JaxInfo
+from tidy3d.plugins.adjoint.components.simulation import MAX_NUM_INPUT_STRUCTURES
 from tidy3d.plugins.adjoint.components.data.sim_data import JaxSimulationData
 from tidy3d.plugins.adjoint.components.data.monitor_data import JaxModeData, JaxDiffractionData
 from tidy3d.plugins.adjoint.components.data.data_array import JaxDataArray, JAX_DATA_ARRAY_TAG
 from tidy3d.plugins.adjoint.components.data.dataset import JaxPermittivityDataset
 from tidy3d.plugins.adjoint.web import run, run_async
 from tidy3d.plugins.adjoint.web import run_local, run_async_local
 from tidy3d.plugins.adjoint.components.data.data_array import VALUE_FILTER_THRESHOLD
 from tidy3d.web.container import BatchData
+from tidy3d.web import run as run_regular
 
 from ..utils import run_emulated, assert_log_level, log_capture, run_async_emulated
 from ..utils import SIM_DATA_PATH, SIM_FULL, TMP_DIR
 
 FWD_SIM_DATA_FILE = TMP_DIR + "adjoint_grad_data_fwd.hdf5"
 SIM_VJP_FILE = TMP_DIR + "adjoint_sim_vjp_file.hdf5"
 RUN_PATH = TMP_DIR + "simulation.hdf5"
+NUM_PROC_PARALLEL = 2
 
 EPS = 2.0
 SIZE = (1.0, 2.0, 3.0)
 CENTER = (2.0, -1.0, 1.0)
 VERTICES = ((-1.0, -1.0), (0.0, 0.0), (-1.0, 0.0))
 POLYSLAB_AXIS = 2
 FREQ0 = 2e14
@@ -90,14 +94,15 @@
     sim_adj: td.Simulation,
     jax_info_adj: JaxInfo,
     fwd_task_id: str,
     task_name: str,
     folder_name: str,
     callback_url: str,
     verbose: bool,
+    num_proc: int = NUM_PROC_PARALLEL,
 ) -> JaxSimulation:
     """Runs adjoint simulation on our servers, grabs the gradient data from fwd for processing."""
 
     # Forward data
     sim_data_fwd = JaxSimulationData.from_file(FWD_SIM_DATA_FILE)
     grad_data_fwd = sim_data_fwd.grad_data_symmetry
     grad_eps_data_fwd = sim_data_fwd.grad_eps_data_symmetry
@@ -109,15 +114,17 @@
         path=RUN_PATH,
     )
 
     jax_sim_data_adj = JaxSimulationData.from_sim_data(sim_data_adj, jax_info_adj)
     grad_data_adj = jax_sim_data_adj.grad_data_symmetry
 
     # get gradient and insert into the resulting simulation structure medium
-    sim_vjp = jax_sim_data_adj.simulation.store_vjp(grad_data_fwd, grad_data_adj, grad_eps_data_fwd)
+    sim_vjp = jax_sim_data_adj.simulation.store_vjp(
+        grad_data_fwd, grad_data_adj, grad_eps_data_fwd, num_proc=num_proc
+    )
 
     # write VJP sim to and from file to emulate webapi download and loading
     sim_vjp.to_file(SIM_VJP_FILE)
     sim_vjp = JaxSimulation.from_file(SIM_VJP_FILE)
 
     return sim_vjp
 
@@ -170,14 +177,15 @@
             sim_adj=sim,
             jax_info_adj=jax_info,
             fwd_task_id="test",
             task_name=str(i),
             folder_name=folder_name,
             callback_url=callback_url,
             verbose=verbose,
+            num_proc=NUM_PROC_PARALLEL,
         )
         sim_vjps_orig.append(sim_vjp)
 
     return sim_vjps_orig
 
 
 def make_sim(
@@ -189,15 +197,15 @@
     med = td.Medium(permittivity=2.0)
     extraneous_structure = td.Structure(geometry=box, medium=med)
 
     # NOTE: Any new input structures should be added below as they are made
 
     # JaxBox
     jax_box1 = JaxBox(size=size, center=(1, 0, 2))
-    jax_med1 = JaxMedium(permittivity=permittivity)
+    jax_med1 = JaxMedium(permittivity=permittivity, conductivity=permittivity * 0.1)
     jax_struct1 = JaxStructure(geometry=jax_box1, medium=jax_med1)
 
     jax_box2 = JaxBox(size=size, center=(-1, 0, -3))
     jax_med2 = JaxAnisotropicMedium(
         xx=JaxMedium(permittivity=permittivity),
         yy=JaxMedium(permittivity=permittivity + 2),
         zz=JaxMedium(permittivity=permittivity * 2),
@@ -215,20 +223,27 @@
         y=np.linspace(ymin, ymax, Ny).tolist(),
         z=np.linspace(zmin, zmax, Nz).tolist(),
         f=[FREQ0],
     )
 
     jax_box_custom = JaxBox(size=size, center=(1, 0, 2))
     values = base_eps_val + np.random.random((Nx, Ny, Nz, 1))
+
+    # adding this line breaks things without enforcing that the vjp for custom medium is complex
+    values = (1 + 1j) * values
+    values = values + (1 + 1j) * values / 0.5
+
     eps_ii = JaxDataArray(values=values, coords=coords)
     field_components = {f"eps_{dim}{dim}": eps_ii for dim in "xyz"}
     jax_eps_dataset = JaxPermittivityDataset(**field_components)
     jax_med_custom = JaxCustomMedium(eps_dataset=jax_eps_dataset)
     jax_struct_custom = JaxStructure(geometry=jax_box_custom, medium=jax_med_custom)
 
+    jax_geo_group = JaxGeometryGroup(geometries=[jax_polyslab1, jax_polyslab1])
+    jax_struct_group = JaxStructure(geometry=jax_geo_group, medium=jax_med1)
     # TODO: Add new geometries as they are created.
 
     # NOTE: Any new output monitors should be added below as they are made
 
     # ModeMonitors
     output_mnt1 = td.ModeMonitor(
         size=(10, 10, 0),
@@ -243,68 +258,163 @@
         size=(td.inf, td.inf, 0),
         normal_dir="+",
         freqs=[FREQ0],
         name=MNT_NAME + "2",
     )
 
     output_mnt3 = td.FieldMonitor(
-        size=(10, 2, 0),
+        size=(2, 0, 2),
         freqs=[FREQ0],
         name=MNT_NAME + "3",
     )
 
+    output_mnt4 = td.FieldMonitor(
+        size=(0, 0, 0),
+        freqs=[FREQ0],
+        name=MNT_NAME + "4",
+    )
+
     extraneous_field_monitor = td.FieldMonitor(
         size=(10, 10, 0),
         freqs=[1e14, 2e14],
         name="field",
     )
 
     sim = JaxSimulation(
         size=(10, 10, 10),
         run_time=1e-12,
-        grid_spec=td.GridSpec(wavelength=1.0),
+        grid_spec=td.GridSpec(wavelength=4.0),
         monitors=(extraneous_field_monitor,),
         structures=(extraneous_structure,),
-        output_monitors=(output_mnt1, output_mnt2),  # , output_mnt3),
-        input_structures=(jax_struct1, jax_struct2, jax_struct_custom, jax_struct3),
+        input_structures=(
+            jax_struct1,
+            jax_struct2,
+            jax_struct_custom,
+            jax_struct3,
+            jax_struct_group,
+        ),
+        output_monitors=(output_mnt1, output_mnt2, output_mnt3, output_mnt4),
         boundary_spec=td.BoundarySpec.pml(x=False, y=False, z=False),
+        symmetry=(0, 1, -1),
     )
 
     return sim
 
 
 def objective(amp: complex) -> float:
     """Objective function as a function of the complex amplitude."""
     return abs(amp) ** 2
 
 
+def test_run_flux(use_emulated_run):
+    td.config.logging_level = "ERROR"
+
+    def make_components(eps, size, vertices, base_eps_val):
+        sim = make_sim(permittivity=eps, size=size, vertices=vertices, base_eps_val=base_eps_val)
+        # sim = sim.to_simulation()[0]
+        td.config.logging_level = "WARNING"
+        sim = sim.updated_copy(
+            sources=[
+                td.PointDipole(
+                    center=(0, 0, 0),
+                    polarization="Ex",
+                    source_time=td.GaussianPulse(freq0=2e14, fwidth=1e15),
+                )
+            ]
+        )
+        sim_data = run_local(sim, task_name="test", path=RUN_PATH)
+        mnt_data = sim_data[MNT_NAME + "3"]
+        flat_components = {}
+        for key, fld in mnt_data.field_components.items():
+            values = jnp.array(jax.lax.stop_gradient(fld.values))[:, 1, ...]
+            values = values[:, None, ...]
+            coords = dict(fld.coords).copy()
+            coords["y"] = [0.0]
+            if isinstance(fld, td.ScalarFieldDataArray):
+                flat_components[key] = td.ScalarFieldDataArray(values, coords=coords)
+            else:
+                flat_components[key] = fld.updated_copy(values=values, coords=coords)
+        return mnt_data.updated_copy(**flat_components)
+
+    mnt_data = make_components(EPS, SIZE, VERTICES, BASE_EPS_VAL)
+
+    # whether to run the flux pipeline through jax (True) or regular tidy3d (False)
+    use_jax = True
+    if not use_jax:
+
+        td_field_components = {}
+        for fld, jax_data_array in mnt_data.field_components.items():
+            data_array = td.ScalarFieldDataArray(
+                np.array(jax_data_array.values), coords=jax_data_array.coords
+            )
+            td_field_components[fld] = data_array
+
+        mnt_data = td.FieldData(monitor=mnt_data.monitor, **td_field_components)
+
+    def get_flux(x):
+
+        fld_components = {}
+        for fld, fld_component in mnt_data.field_components.items():
+            new_values = x * fld_component.values
+            if isinstance(fld_component, td.ScalarFieldDataArray):
+                fld_data = td.ScalarFieldDataArray(new_values, coords=fld_component.coords)
+            else:
+                fld_data = fld_component.updated_copy(values=new_values)
+            fld_components[fld] = fld_data
+
+        mnt_data2 = mnt_data.updated_copy(**fld_components)
+
+        return jnp.sum(mnt_data2.flux)
+
+    f = get_flux(1.0)
+
+    if use_jax:
+        get_flux_grad = jax.grad(get_flux)
+        g = get_flux_grad(1.0)
+
+
 def extract_amp(sim_data: td.SimulationData) -> complex:
     """get the amplitude from a simulation data object."""
 
     ret_value = 0.0
 
     # ModeData
     mnt_name = MNT_NAME + "1"
-    mnt_data = sim_data.output_monitor_data[mnt_name]
+    mnt_data = sim_data[mnt_name]
     amps = mnt_data.amps
     ret_value += amps.sel(direction="+", f=2e14, mode_index=0)
     ret_value += amps.isel(direction=0, f=0, mode_index=0)
     ret_value += amps.sel(direction="-", f=2e14, mode_index=1)
     ret_value += amps.sel(mode_index=1, f=2e14, direction="-")
     ret_value += amps.sel(direction="-", f=2e14).isel(mode_index=1)
 
     # DiffractionData
     mnt_name = MNT_NAME + "2"
-    mnt_data = sim_data.output_monitor_data[mnt_name]
+    mnt_data = sim_data[mnt_name]
     ret_value += mnt_data.amps.sel(orders_x=0, orders_y=0, f=2e14, polarization="p")
     ret_value += mnt_data.amps.sel(orders_x=-1, orders_y=1, f=2e14, polarization="p")
     ret_value += mnt_data.amps.isel(orders_x=0, orders_y=1, f=0, polarization=0)
     ret_value += mnt_data.Er.isel(orders_x=0, orders_y=1, f=0)
     ret_value += mnt_data.power.sel(orders_x=-1, orders_y=1, f=2e14)
 
+    # FieldData
+    mnt_name = MNT_NAME + "3"
+    mnt_data = sim_data[mnt_name]
+    ret_value += jnp.sum(jnp.array(mnt_data.Ex.values))
+    ret_value += jnp.sum(jnp.array(mnt_data.Ex.interp(z=0).values))
+
+    # this should work when we figure out a jax version of xr.DataArray
+    sim_data.get_intensity(mnt_name)
+    # ret_value += jnp.sum(jnp.array(mnt_data.flux().values))
+
+    # FieldData (dipole)
+    mnt_name = MNT_NAME + "4"
+    mnt_data = sim_data[mnt_name]
+    ret_value += jnp.sum(jnp.array(mnt_data.Ex.values))
+
     return ret_value
 
 
 @pytest.fixture
 def use_emulated_run(monkeypatch):
     """If this fixture is used, the `tests.utils.run_emulated` function is used for simulation."""
     import tidy3d.plugins.adjoint.web as adjoint_web
@@ -600,14 +710,18 @@
 
     # creation
     da = JaxDataArray(values=values, coords=coords)
     _ = da.real
     _ = da.imag
     _ = da.as_list
 
+    # isel multi
+    z = da.isel(a=1, b=[0, 1], c=0)
+    assert z.shape == (2,)
+
     # isel
     z = da.isel(a=1, b=1, c=0)
     z = da.isel(c=0, b=1, a=1)
 
     # sel
     z = da.sel(a=1, b=2, c=4)
     z = da.sel(c=4, b=2, a=1)
@@ -625,16 +739,25 @@
         da.isel(c=1)
     with pytest.raises(DataError):
         da.isel(c=-1)
     with pytest.raises(DataError):
         da.sel(c=5)
 
     # not implemented
-    with pytest.raises(NotImplementedError):
-        da.interp(b=2.5)
+    # with pytest.raises(NotImplementedError):
+    da.interp(b=2.5)
+
+    assert np.isclose(da.interp(a=2, b=3, c=4), values[1, 1, 0])
+    assert np.isclose(da.interp(a=1, b=2, c=4), values[0, 0, 0])
+
+    with pytest.raises(Tidy3dKeyError):
+        da.interp(d=3)
+
+    da1d = JaxDataArray(values=[0.0, 1.0, 2.0, 3.0], coords=dict(x=[0, 1, 2, 3]))
+    assert np.isclose(da1d.interp(x=0.5), 0.5)
 
 
 def test_jax_sim_data(use_emulated_run):
     """Test mechanics of the JaxSimulationData."""
 
     sim = make_sim(permittivity=EPS, size=SIZE, vertices=VERTICES, base_eps_val=BASE_EPS_VAL)
     sim_data = run(sim, task_name="test", path=RUN_PATH)
@@ -892,20 +1015,32 @@
             center=(0, 4, 0),
             size=(td.inf, 0, td.inf),
             normal_dir="+",
             freqs=[2e14],
             name=MNT_NAME + "2",
         )
 
+        output_mnt3 = td.FieldMonitor(
+            size=(2, 0, 2),
+            freqs=[FREQ0],
+            name=MNT_NAME + "3",
+        )
+
+        output_mnt4 = td.FieldMonitor(
+            size=(0, 0, 0),
+            freqs=[FREQ0],
+            name=MNT_NAME + "4",
+        )
+
         sim = JaxSimulation(
             size=(10, 10, sim_size_axis),
             run_time=1e-12,
             grid_spec=td.GridSpec(wavelength=1.0),
             boundary_spec=td.BoundarySpec.all_sides(boundary=td.Periodic()),
-            output_monitors=(output_mnt1, output_mnt2),
+            output_monitors=(output_mnt1, output_mnt2, output_mnt3, output_mnt4),
             input_structures=(jax_struct,),
             sources=[
                 td.PointDipole(
                     source_time=td.GaussianPulse(freq0=1e14, fwidth=1e14),
                     center=(0, 0, 0),
                     polarization="Ex",
                 )
@@ -1145,16 +1280,17 @@
     vertices = np.random.rand(MAX_NUM_VERTICES, 2)
     poly = JaxPolySlab(vertices=vertices, slab_bounds=(-1, 1))
     vertices = np.random.rand(MAX_NUM_VERTICES + 1, 2)
     with pytest.raises(pydantic.ValidationError):
         poly = JaxPolySlab(vertices=vertices, slab_bounds=(-1, 1))
 
 
-def test_custom_medium_3D(use_emulated_run):
+def _test_custom_medium_3D(use_emulated_run):
     """Ensure custom medium fails if 3D pixelated grid."""
+    # NOTE: turned off since we relaxed this restriction
 
     jax_box = JaxBox(size=(1, 1, 1), center=(0, 0, 0))
 
     def make_custom_medium(Nx: int, Ny: int, Nz: int) -> JaxCustomMedium:
 
         # custom medium
         (xmin, ymin, zmin), (xmax, ymax, zmax) = jax_box.bounds
@@ -1255,7 +1391,22 @@
         assert "input_structures" in f.keys()
         json_string = str(f["JSON_STRING"][()])
         assert JAX_DATA_ARRAY_TAG in json_string
 
     sim2 = JaxSimulation.from_file(fname)
 
     assert sim == sim2
+
+
+def test_num_input_structures():
+    """Assert proper error is raised if number of input structures is too large."""
+
+    def make_sim_(num_input_structures: int) -> JaxSimulation:
+
+        sim = make_sim(permittivity=EPS, size=SIZE, vertices=VERTICES, base_eps_val=BASE_EPS_VAL)
+        struct = sim.input_structures[0]
+        return sim.updated_copy(input_structures=num_input_structures * [struct])
+
+    sim = make_sim_(num_input_structures=MAX_NUM_INPUT_STRUCTURES)
+
+    with pytest.raises(pydantic.ValidationError):
+        sim = make_sim_(num_input_structures=MAX_NUM_INPUT_STRUCTURES + 1)
```

### Comparing `tidy3d-2.3.0rc1/tests/test_plugins/test_component_modeler.py` & `tidy3d-2.3.1/tests/test_plugins/test_component_modeler.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,28 +182,28 @@
 def make_component_modeler(**kwargs):
     """Tests S matrix loading."""
 
     sim = make_coupler()
     ports = make_ports()
     batch_empty = Batch(simulations={}, folder_name="None")
     return ComponentModeler(
-        simulation=sim, ports=ports, freqs=sim.monitors[0].freqs, batch=batch_empty, **kwargs
+        simulation=sim, ports=ports, freqs=sim.monitors[0].freqs, path_dir=PATH_DIR, **kwargs
     )
 
 
 def run_component_modeler(monkeypatch, modeler: ComponentModeler):
 
     values = dict(
         simulation=modeler.simulation,
         ports=modeler.ports,
         freqs=modeler.freqs,
         run_only=modeler.run_only,
         element_mappings=modeler.element_mappings,
     )
-    sim_dict = modeler.make_sim_dict(values)
+    sim_dict = modeler.sim_dict
     batch_data = {task_name: run_emulated(sim) for task_name, sim in sim_dict.items()}
     monkeypatch.setattr(ComponentModeler, "_run_sims", lambda self, path_dir: batch_data)
     s_matrix = modeler.run(path_dir=PATH_DIR)
     return s_matrix
 
 
 def test_validate_no_sources():
@@ -214,22 +214,23 @@
     sim_w_source = modeler.simulation.copy(update=dict(sources=(source,)))
     with pytest.raises(pydantic.ValidationError):
         modeler_w_source = modeler.copy(update=dict(simulation=sim_w_source))
 
 
 def test_element_mappings_none():
     modeler = make_component_modeler()
-    modeler.matrix_indices_run_sim(ports=[], element_mappings=None)
+    modeler = modeler.updated_copy(ports=[], element_mappings=())
+    modeler.matrix_indices_run_sim
 
 
 def test_no_port():
     modeler = make_component_modeler()
     ports = modeler.ports
     with pytest.raises(Tidy3dKeyError):
-        modeler.get_port_by_name(ports=ports, port_name="NOT_A_PORT")
+        modeler.get_port_by_name(port_name="NOT_A_PORT")
 
 
 def test_ports_too_close_boundary():
     modeler = make_component_modeler()
     grid_boundaries = modeler.simulation.grid.boundaries.to_list[0]
     way_outside = grid_boundaries[0] - 1000
     xmin = grid_boundaries[1]
@@ -238,21 +239,23 @@
         port_at_edge = modeler.ports[0].copy()
         port_center_at_edge = list(port_at_edge.center)
         port_center_at_edge[0] = edge_val
         port_at_edge = port_at_edge.copy(
             update=dict(center=port_center_at_edge, direction=port_dir)
         )
         with pytest.raises(SetupError):
-            modeler._shift_value_signed(simulation=modeler.simulation, port=port_at_edge)
+            modeler._shift_value_signed(port=port_at_edge)
 
 
 def test_validate_batch_supplied():
 
     sim = make_coupler()
-    modeler = ComponentModeler(simulation=sim, ports=[], freqs=sim.monitors[0].freqs, batch=None)
+    modeler = ComponentModeler(
+        simulation=sim, ports=[], freqs=sim.monitors[0].freqs, path_dir=PATH_DIR
+    )
 
 
 def test_plot_sim():
     modeler = make_component_modeler()
     modeler.plot_sim(z=0)
 
 
@@ -368,14 +371,12 @@
 
     # add the self-self coupling element to complete row
     mapping = ((("right_bot", 1), ("right_bot", 1)), (EXCLUDE_INDEX, EXCLUDE_INDEX), +1)
     element_mappings.append(mapping)
 
     modeler = make_component_modeler(element_mappings=element_mappings)
 
-    run_sim_indices = modeler.matrix_indices_run_sim(
-        ports=modeler.ports, run_only=modeler.run_only, element_mappings=modeler.element_mappings
-    )
+    run_sim_indices = modeler.matrix_indices_run_sim
     assert EXCLUDE_INDEX not in run_sim_indices, "mapping didnt exclude row properly"
 
     s_matrix = run_component_modeler(monkeypatch, modeler)
     _test_mappings(element_mappings, s_matrix)
```

### Comparing `tidy3d-2.3.0rc1/tests/test_plugins/test_dispersion_fitter.py` & `tidy3d-2.3.1/tests/test_plugins/test_dispersion_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_plugins/test_polyslab.py` & `tidy3d-2.3.1/tests/test_plugins/test_polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_plugins/test_resonance_finder.py` & `tidy3d-2.3.1/tests/test_plugins/test_resonance_finder.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_plugins/test_waveguide.py` & `tidy3d-2.3.1/tests/test_plugins/test_waveguide.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_web/test_cli.py` & `tidy3d-2.3.1/tests/test_web/test_cli.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_web/test_material_fitter.py` & `tidy3d-2.3.1/tests/test_web/test_material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_web/test_tidy3d_folder.py` & `tidy3d-2.3.1/tests/test_web/test_tidy3d_folder.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_web/test_tidy3d_material_library.py` & `tidy3d-2.3.1/tests/test_web/test_tidy3d_material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tests/test_web/test_tidy3d_task.py` & `tidy3d-2.3.1/tests/test_web/test_tidy3d_task.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import pytest
 import os
 import tempfile
 
 import responses
 from responses import matchers
 
+from tidy3d.web import monitor
 from tidy3d.web.environment import Env, EnvironmentConfig
 from tidy3d.web.simulation_task import Folder, SimulationTask
 from tidy3d.version import __version__
 
 test_env = EnvironmentConfig(
     name="test",
+    s3_region="test",
     web_api_endpoint="https://test",
     website_endpoint="https://test",
 )
 
 Env.set_current(test_env)
 
 
@@ -141,15 +143,15 @@
     responses.add(
         responses.POST,
         f"{Env.current.web_api_endpoint}/tidy3d/projects/1234/tasks",
         match=[
             matchers.json_params_matcher(
                 {
                     "taskName": "test task",
-                    "call_back_url": None,
+                    "callbackUrl": None,
                     "simulationType": "tidy3d",
                     "parentTasks": None,
                 }
             )
         ],
         json={
             "data": {
@@ -162,73 +164,107 @@
     )
     task = SimulationTask.create(None, "test task", "test folder2")
     assert task.task_id == "1234"
 
 
 @responses.activate
 def test_submit(set_api_key):
+    project_id = "1234"
+    task_id = "1234"
+    task_name = "test task"
     responses.add(
         responses.GET,
         f"{Env.current.web_api_endpoint}/tidy3d/project",
         match=[matchers.query_param_matcher({"projectName": "test folder1"})],
-        json={"data": {"projectId": "1234", "projectName": "test folder1"}},
+        json={"data": {"projectId": project_id, "projectName": "test folder1"}},
         status=200,
     )
     responses.add(
         responses.POST,
-        f"{Env.current.web_api_endpoint}/tidy3d/projects/1234/tasks",
+        f"{Env.current.web_api_endpoint}/tidy3d/projects/{project_id}/tasks",
         match=[
             matchers.json_params_matcher(
                 {
-                    "taskName": "test task",
-                    "call_back_url": None,
+                    "taskName": task_name,
+                    "callbackUrl": None,
                     "simulationType": "tidy3d",
                     "parentTasks": None,
                 }
             )
         ],
         json={
             "data": {
-                "taskId": "1234",
-                "taskName": "test task",
+                "taskId": task_id,
+                "taskName": task_name,
                 "createdAt": "2022-01-01T00:00:00.000Z",
             }
         },
         status=200,
     )
     responses.add(
         responses.POST,
-        f"{Env.current.web_api_endpoint}/tidy3d/tasks/1234/submit",
+        f"{Env.current.web_api_endpoint}/tidy3d/tasks/{task_id}/submit",
         match=[
             matchers.json_params_matcher(
                 {"solverVersion": None, "workerGroup": None, "protocolVersion": __version__}
             )
         ],
         json={
             "data": {
-                "taskId": "1234",
-                "taskName": "test task",
+                "taskId": task_id,
+                "taskName": task_name,
                 "createdAt": "2022-01-01T00:00:00.000Z",
+                "taskBlockInfo": {
+                    "chargeType": "free",
+                    "maxFreeCount": 20,
+                    "maxGridPoints": 1000,
+                    "maxTimeSteps": 1000,
+                },
             }
         },
         status=200,
     )
-    task = SimulationTask.create(None, "test task", "test folder1")
+    responses.add(
+        responses.GET,
+        f"{Env.current.web_api_endpoint}/tidy3d/tasks/{task_id}/detail",
+        json={
+            "taskId": task_id,
+            "taskName": task_name,
+            "createdAt": "2022-01-01T00:00:00.000Z",
+            "status": "running",
+            "taskBlockInfo": {
+                "chargeType": "free",
+                "maxFreeCount": 20,
+                "maxGridPoints": 1000,
+                "maxTimeSteps": 1000,
+            },
+        },
+        status=200,
+    )
+    task = SimulationTask.create(None, task_name, "test folder1")
     task.submit()
+    # test DE need to open the comment
+    # monitor(task_id, True)
 
 
 @responses.activate
 def test_estimate_cost(set_api_key):
     responses.add(
         responses.GET,
         f"{Env.current.web_api_endpoint}/tidy3d/tasks/3eb06d16-208b-487b-864b-e9b1d3e010a7/detail",
         json={
             "data": {
                 "taskId": "3eb06d16-208b-487b-864b-e9b1d3e010a7",
                 "createdAt": "2022-01-01T00:00:00.000Z",
+                "taskBlockInfo": {
+                    "chargeType": "free",
+                    "maxFreeCount": 20,
+                    "maxGridPoints": 1000,
+                    "maxTimeSteps": 1000,
+                },
             }
         },
         status=200,
     )
 
     responses.add(
         responses.POST,
```

### Comparing `tidy3d-2.3.0rc1/tests/test_web/test_webapi.py` & `tidy3d-2.3.1/tests/test_web/test_webapi.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,70 @@
 # Tests webapi and things that depend on it
 import tempfile
 import pytest
 import responses
+from _pytest import monkeypatch
+import os
+
 import tidy3d as td
 import tidy3d.web as web
 
 from responses import matchers
 
-from tidy3d import Simulation
+from tidy3d.exceptions import SetupError
 from tidy3d.web.environment import Env
 from tidy3d.web.webapi import delete, delete_old, download, download_json, run
 from tidy3d.web.webapi import download_log, estimate_cost, get_info, get_run_info, get_tasks
 from tidy3d.web.webapi import load, load_simulation, start, upload, monitor, real_cost
 from tidy3d.web.container import Job, Batch
 from tidy3d.web.task import TaskInfo
 from tidy3d.web.asynchronous import run_async
 
 from tidy3d.__main__ import main
 
+from ..utils import TMP_DIR
+
 # variables used below
-FNAME_TMP = "tests/tmp/web_test_tmp.json"
+FNAME_TMP = os.path.join(TMP_DIR, "web_test_tmp.json")
+
 TASK_NAME = "task_name_test"
 TASK_ID = "1234"
 CREATED_AT = "2022-01-01T00:00:00.000Z"
 PROJECT_NAME = "default"
 FLEX_UNIT = 1.0
+EST_FLEX_UNIT = 11.11
+
+# make the TMP directory if it doesnt exist
+if not os.path.exists(TMP_DIR):
+    os.mkdir(TMP_DIR)
 
 
 def make_sim():
     """Makes a simulation."""
-    return td.Simulation(size=(1, 1, 1), grid_spec=td.GridSpec.auto(wavelength=1.0), run_time=1e-12)
+    pulse = td.GaussianPulse(freq0=200e12, fwidth=20e12)
+    pt_dipole = td.PointDipole(source_time=pulse, polarization="Ex")
+    return td.Simulation(
+        size=(1, 1, 1),
+        grid_spec=td.GridSpec.auto(wavelength=1.0),
+        run_time=1e-12,
+        sources=[pt_dipole],
+    )
 
 
 @pytest.fixture
 def set_api_key(monkeypatch):
     """Set the api key."""
     import tidy3d.web.http_management as http_module
 
     monkeypatch.setattr(http_module, "api_key", lambda: "apikey")
 
 
 @pytest.fixture
 def mock_upload(monkeypatch, set_api_key):
-    """Mocks webapi.uupload."""
+    """Mocks webapi.upload."""
 
     responses.add(
         responses.GET,
         f"{Env.current.web_api_endpoint}/tidy3d/project",
         match=[matchers.query_param_matcher({"projectName": PROJECT_NAME})],
         json={"data": {"projectId": TASK_ID, "projectName": PROJECT_NAME}},
         status=200,
@@ -55,15 +73,15 @@
     responses.add(
         responses.POST,
         f"{Env.current.web_api_endpoint}/tidy3d/projects/{TASK_ID}/tasks",
         match=[
             matchers.json_params_matcher(
                 {
                     "taskName": TASK_NAME,
-                    "call_back_url": None,
+                    "callbackUrl": None,
                     "simulationType": "tidy3d",
                     "parentTasks": None,
                 }
             )
         ],
         json={
             "data": {
@@ -87,38 +105,32 @@
 
     responses.add(
         responses.GET,
         f"{Env.current.web_api_endpoint}/tidy3d/tasks/{TASK_ID}/detail",
         json={
             "data": {
                 "taskId": TASK_ID,
+                "taskName": TASK_NAME,
                 "createdAt": CREATED_AT,
                 "realFlexUnit": FLEX_UNIT,
+                "estFlexUnit": EST_FLEX_UNIT,
+                "metadataStatus": "processed",
+                "status": "success",
+                "s3Storage": 1.0,
             }
         },
         status=200,
     )
 
 
 @pytest.fixture
-def mock_start(monkeypatch, set_api_key):
+def mock_start(monkeypatch, set_api_key, mock_get_info):
     """Mocks webapi.start."""
 
     responses.add(
-        responses.GET,
-        f"{Env.current.web_api_endpoint}/tidy3d/tasks/{TASK_ID}/detail",
-        json={
-            "data": {
-                "taskId": TASK_ID,
-                "createdAt": CREATED_AT,
-            }
-        },
-        status=200,
-    )
-    responses.add(
         responses.POST,
         f"{Env.current.web_api_endpoint}/tidy3d/tasks/{TASK_ID}/submit",
         match=[
             matchers.json_params_matcher(
                 {
                     "solverVersion": None,
                     "workerGroup": None,
@@ -139,110 +151,77 @@
 
 @pytest.fixture
 def mock_monitor(monkeypatch):
 
     status_count = [0]
     statuses = ("upload", "running", "running", "running", "running", "running", "success")
 
-    def mock_get_info(task_id):
+    def mock_get_status(task_id):
 
         current_count = min(status_count[0], len(statuses) - 1)
         current_status = statuses[current_count]
         status_count[0] += 1
-        return TaskInfo(status=current_status, taskName=TASK_NAME, taskId=task_id, realFlexUnit=1.0)
+        return current_status
+        # return TaskInfo(status=current_status, taskName=TASK_NAME, taskId=task_id, realFlexUnit=1.0)
 
     run_count = [0]
     perc_dones = (1, 10, 20, 30, 100)
 
     def mock_get_run_info(task_id):
         current_count = min(run_count[0], len(perc_dones) - 1)
         perc_done = perc_dones[current_count]
         run_count[0] += 1
         return perc_done, 1
 
     monkeypatch.setattr("tidy3d.web.webapi.REFRESH_TIME", 0.00001)
     monkeypatch.setattr("tidy3d.web.webapi.RUN_REFRESH_TIME", 0.00001)
-    monkeypatch.setattr("tidy3d.web.webapi.get_info", mock_get_info)
+    monkeypatch.setattr("tidy3d.web.webapi.get_status", mock_get_status)
     monkeypatch.setattr("tidy3d.web.webapi.get_run_info", mock_get_run_info)
 
 
 @pytest.fixture
-def mock_download(monkeypatch, set_api_key):
+def mock_download(monkeypatch, set_api_key, mock_get_info):
     """Mocks webapi.download."""
-    responses.add(
-        responses.GET,
-        f"{Env.current.web_api_endpoint}/tidy3d/tasks/{TASK_ID}/detail",
-        json={
-            "data": {
-                "taskId": TASK_ID,
-                "createdAt": CREATED_AT,
-            }
-        },
-        status=200,
-    )
 
     def _mock_download(*args, **kwargs):
         file_path = kwargs["to_file"]
         with open(file_path, "w") as f:
             f.write("0.3,5.7")
 
     monkeypatch.setattr("tidy3d.web.simulation_task.download_file", _mock_download)
     download(TASK_ID, FNAME_TMP)
     with open(FNAME_TMP, "r") as f:
         assert f.read() == "0.3,5.7"
 
 
 @pytest.fixture
-def mock_load(monkeypatch, set_api_key):
+def mock_load(monkeypatch, set_api_key, mock_get_info):
     """Mocks webapi.load"""
 
-    responses.add(
-        responses.GET,
-        f"{Env.current.web_api_endpoint}/tidy3d/tasks/{TASK_ID}/detail",
-        json={
-            "data": {
-                "taskId": TASK_ID,
-                "createdAt": CREATED_AT,
-            }
-        },
-        status=200,
-    )
-
     def _mock_download(*args, **kwargs):
         pass
 
     monkeypatch.setattr("tidy3d.web.simulation_task.download_file", _mock_download)
 
-    # estimate cost
+
+@pytest.fixture
+def mock_metadata(monkeypatch, set_api_key):
+    """Mocks call to metadata api"""
     responses.add(
-        responses.GET,
-        f"{Env.current.web_api_endpoint}/tidy3d/tasks/{TASK_ID}/detail",
+        responses.POST,
+        f"{Env.current.web_api_endpoint}/tidy3d/tasks/{TASK_ID}/metadata",
         json={
             "data": {
-                "taskId": TASK_ID,
                 "createdAt": CREATED_AT,
             }
         },
         status=200,
     )
 
 
-responses.add(
-    responses.POST,
-    f"{Env.current.web_api_endpoint}/tidy3d/tasks/{TASK_ID}/metadata",
-    json={
-        "data": {
-            "flex_unit": 11.11,
-            "createdAt": CREATED_AT,
-        }
-    },
-    status=200,
-)
-
-
 @pytest.fixture
 def mock_get_run_info(monkeypatch, set_api_key):
     """Mocks webapi.get_run_info"""
     responses.add(
         responses.GET,
         f"{Env.current.web_api_endpoint}/tidy3d/tasks/{TASK_ID}/progress",
         json={
@@ -252,19 +231,29 @@
             }
         },
         status=200,
     )
 
 
 @pytest.fixture
-def mock_webapi(mock_upload, mock_get_info, mock_start, mock_monitor, mock_download, mock_load):
+def mock_webapi(
+    mock_upload, mock_metadata, mock_get_info, mock_start, mock_monitor, mock_download, mock_load
+):
     """Mocks all webapi operation."""
 
 
 @responses.activate
+def test_source_validation(mock_upload):
+    sim = make_sim().copy(update={"sources": []})
+    assert upload(sim, TASK_NAME, PROJECT_NAME, source_required=False)
+    with pytest.raises(SetupError):
+        upload(sim, TASK_NAME, PROJECT_NAME)
+
+
+@responses.activate
 def test_upload(mock_upload):
     sim = make_sim()
     assert upload(sim, TASK_NAME, PROJECT_NAME)
 
 
 @responses.activate
 def test_get_info(mock_get_info):
@@ -285,47 +274,24 @@
 def test_download(mock_download):
     download(TASK_ID, FNAME_TMP)
     with open(FNAME_TMP, "r") as f:
         assert f.read() == "0.3,5.7"
 
 
 @responses.activate
-def _test_load(mock_load):
-    responses.add(
-        responses.GET,
-        f"{Env.current.web_api_endpoint}/tidy3d/tasks/{TASK_ID}/detail",
-        json={
-            "data": {
-                "taskId": TASK_ID,
-                "createdAt": CREATED_AT,
-            }
-        },
-        status=200,
-    )
-
+def _test_load(mock_load, mock_get_info):
     def mock_download(*args, **kwargs):
         pass
 
     monkeypatch.setattr("tidy3d.web.simulation_task.download_file", mock_download)
     load(TASK_ID, "tmp/monitor_data.hdf5")
 
 
 @responses.activate
-def test_delete(set_api_key):
-    responses.add(
-        responses.GET,
-        f"{Env.current.web_api_endpoint}/tidy3d/tasks/{TASK_ID}/detail",
-        json={
-            "data": {
-                "taskId": TASK_ID,
-                "createdAt": CREATED_AT,
-            }
-        },
-        status=200,
-    )
+def test_delete(set_api_key, mock_get_info):
 
     responses.add(
         responses.DELETE,
         f"{Env.current.web_api_endpoint}/tidy3d/tasks/{TASK_ID}",
         json={
             "data": {
                 "taskId": TASK_ID,
@@ -335,104 +301,46 @@
         status=200,
     )
 
     assert delete(TASK_ID).taskId == TASK_ID
 
 
 @responses.activate
-def test_estimate_cost(set_api_key):
-    responses.add(
-        responses.GET,
-        f"{Env.current.web_api_endpoint}/tidy3d/tasks/{TASK_ID}/detail",
-        json={
-            "data": {
-                "taskId": TASK_ID,
-                "createdAt": CREATED_AT,
-            }
-        },
-        status=200,
-    )
-    responses.add(
-        responses.POST,
-        f"{Env.current.web_api_endpoint}/tidy3d/tasks/{TASK_ID}/metadata",
-        json={
-            "data": {
-                "flex_unit": 11.11,
-                "createdAt": CREATED_AT,
-            }
-        },
-        status=200,
-    )
-    assert estimate_cost(TASK_ID) == 11.11
+def test_estimate_cost(set_api_key, mock_get_info, mock_metadata):
+    assert estimate_cost(TASK_ID) == EST_FLEX_UNIT
 
 
 @responses.activate
-def test_download_json(monkeypatch):
-    responses.add(
-        responses.GET,
-        f"{Env.current.web_api_endpoint}/tidy3d/tasks/{TASK_ID}/detail",
-        json={
-            "data": {
-                "taskId": TASK_ID,
-                "createdAt": CREATED_AT,
-            }
-        },
-        status=200,
-    )
-
+def test_download_json(monkeypatch, mock_get_info):
     def mock_download(*args, **kwargs):
         file_path = kwargs["to_file"]
         with open(file_path, "w") as f:
             f.write("0.3,5.7")
 
     monkeypatch.setattr("tidy3d.web.simulation_task.download_file", mock_download)
 
     download_json(TASK_ID, FNAME_TMP)
     with open(FNAME_TMP, "r") as f:
         assert f.read() == "0.3,5.7"
 
 
 @responses.activate
-def test_load_simulation(monkeypatch):
-    responses.add(
-        responses.GET,
-        f"{Env.current.web_api_endpoint}/tidy3d/tasks/{TASK_ID}/detail",
-        json={
-            "data": {
-                "taskId": TASK_ID,
-                "createdAt": CREATED_AT,
-            }
-        },
-        status=200,
-    )
-
+def test_load_simulation(monkeypatch, mock_get_info):
     def mock_download(*args, **kwargs):
         make_sim().to_file(args[1])
 
     monkeypatch.setattr(
         "tidy3d.web.simulation_task.SimulationTask.get_simulation_json", mock_download
     )
 
     assert load_simulation(TASK_ID, FNAME_TMP + ".json")
 
 
 @responses.activate
-def test_download_log(monkeypatch):
-    responses.add(
-        responses.GET,
-        f"{Env.current.web_api_endpoint}/tidy3d/tasks/{TASK_ID}/detail",
-        json={
-            "data": {
-                "taskId": TASK_ID,
-                "createdAt": CREATED_AT,
-            }
-        },
-        status=200,
-    )
-
+def test_download_log(monkeypatch, mock_get_info):
     def mock(*args, **kwargs):
         file_path = kwargs["to_file"]
         with open(file_path, "w") as f:
             f.write("0.3,5.7")
 
     monkeypatch.setattr("tidy3d.web.simulation_task.download_file", mock)
 
@@ -496,15 +404,15 @@
 def test_run(mock_webapi, monkeypatch):
     sim = make_sim()
     monkeypatch.setattr("tidy3d.web.webapi.load", lambda *args, **kwargs: True)
     assert run(sim, task_name=TASK_NAME, folder_name=PROJECT_NAME, path=FNAME_TMP)
 
 
 @responses.activate
-def test_monitor(mock_monitor):
+def test_monitor(mock_get_info, mock_monitor):
     monitor(TASK_ID, verbose=True)
     monitor(TASK_ID, verbose=False)
 
 
 @responses.activate
 def test_real_cost(mock_get_info):
     assert real_cost(TASK_ID) == FLEX_UNIT
@@ -518,15 +426,15 @@
 
     monkeypatch.setattr("tidy3d.web.container.Job.load", lambda *args, **kwargs: True)
     sim = make_sim()
     j = Job(simulation=sim, task_name=TASK_NAME, folder_name=PROJECT_NAME)
 
     sim_data = j.run(path=FNAME_TMP)
     j.status
-    j.get_info()
+    j.estimate_cost()
     # j.download
     j.delete
     assert j.real_cost() == FLEX_UNIT
 
 
 @pytest.fixture
 def mock_job_status(monkeypatch):
@@ -538,14 +446,15 @@
 def test_batch(mock_webapi, mock_job_status):
 
     # monkeypatch.setattr("tidy3d.web.container.Batch.monitor", lambda self: time.sleep(0.1))
     # monkeypatch.setattr("tidy3d.web.container.Job.status", property(lambda self: "success"))
 
     sims = {TASK_NAME: make_sim()}
     b = Batch(simulations=sims, folder_name=PROJECT_NAME)
+    b.estimate_cost()
     batch_data = b.run(path_dir="tests/tmp/")
     assert b.real_cost() == FLEX_UNIT * len(sims)
 
 
 """ Async """
 
 
@@ -563,28 +472,17 @@
 @responses.activate
 def test_main(mock_webapi, monkeypatch, mock_job_status):
 
     # sims = {TASK_NAME: make_sim()}
     # batch_data = run_async(sims, folder_name=PROJECT_NAME)
 
     def save_sim_to_path(path: str) -> None:
-        sim = Simulation(size=(1, 1, 1), grid_spec=td.GridSpec.auto(wavelength=1.0), run_time=1e-12)
+        sim = make_sim()
         sim.to_file(path)
 
-    def mock_get_info(task_id):
-        return TaskInfo(
-            status="success",
-            taskName=TASK_NAME,
-            taskId=TASK_ID,
-            realFlexUnit=1.0,
-            s3Storage=1.0,
-            estFlexUnit=1.0,
-        )
-
-    monkeypatch.setattr("tidy3d.web.webapi.get_info", mock_get_info)
     monkeypatch.setattr("builtins.input", lambda _: "Y")
 
     path = f"tests/tmp/sim.json"
     save_sim_to_path(path)
     main(
         [
             path,
```

### Comparing `tidy3d-2.3.0rc1/tests/utils.py` & `tidy3d-2.3.1/tests/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import os
 from pathlib import Path
 from typing import Dict, Tuple
 import pydantic as pd
+import trimesh
 
 import pytest
 import numpy as np
 from tidy3d import *
 import tidy3d as td
 from tidy3d.log import _get_level_int
 from tidy3d.web import BatchData
 from tidy3d.components.base import Tidy3dBaseModel
 
 """ utilities shared between all tests """
+np.random.seed(4)
 
 
 def clear_dir(path: str):
     """clears a dir"""
     for f in os.listdir(path):
         full_path = os.path.join(path, f)
         if not os.path.isdir(full_path):
@@ -59,14 +61,76 @@
             mode_spec=ModeSpec(num_modes=3),
             name="mode",
         ),
     ],
     boundary_spec=BoundarySpec.all_sides(boundary=Periodic()),
 )
 
+# STL geometry
+VERTICES = np.array([[-1.5, -0.5, -0.5], [-0.5, -0.5, -0.5], [-1.5, 0.5, -0.5], [-1.5, -0.5, 0.5]])
+FACES = np.array([[1, 2, 3], [0, 3, 2], [0, 1, 3], [0, 2, 1]])
+STL_GEO = TriangleMesh.from_trimesh(trimesh.Trimesh(VERTICES, FACES))
+
+# custom medium
+COORDS = dict(x=[-1.5, -0.5], y=[0, 1], z=[0, 1])
+custom_medium = CustomMedium(
+    permittivity=td.SpatialDataArray(
+        1 + np.random.random((2, 2, 2)),
+        coords=COORDS,
+    ),
+)
+custom_poleresidue = CustomPoleResidue(
+    eps_inf=td.SpatialDataArray(1 + np.random.random((2, 2, 2)), coords=COORDS),
+    poles=(
+        (
+            td.SpatialDataArray(-1 + np.random.random((2, 2, 2)), coords=COORDS),
+            td.SpatialDataArray(1 + np.random.random((2, 2, 2)), coords=COORDS),
+        ),
+    ),
+)
+custom_debye = CustomDebye(
+    eps_inf=td.SpatialDataArray(1 + np.random.random((2, 2, 2)), coords=COORDS),
+    coeffs=(
+        (
+            td.SpatialDataArray(1 + np.random.random((2, 2, 2)), coords=COORDS),
+            td.SpatialDataArray(1 + np.random.random((2, 2, 2)), coords=COORDS),
+        ),
+    ),
+)
+
+custom_drude = CustomDrude(
+    eps_inf=td.SpatialDataArray(1 + np.random.random((2, 2, 2)), coords=COORDS),
+    coeffs=(
+        (
+            td.SpatialDataArray(1 + np.random.random((2, 2, 2)), coords=COORDS),
+            td.SpatialDataArray(1 + np.random.random((2, 2, 2)), coords=COORDS),
+        ),
+    ),
+)
+
+custom_lorentz = CustomLorentz(
+    eps_inf=td.SpatialDataArray(1 + np.random.random((2, 2, 2)), coords=COORDS),
+    coeffs=(
+        (
+            td.SpatialDataArray(1 + np.random.random((2, 2, 2)), coords=COORDS),
+            td.SpatialDataArray(10 + np.random.random((2, 2, 2)), coords=COORDS),
+            td.SpatialDataArray(1 + np.random.random((2, 2, 2)), coords=COORDS),
+        ),
+    ),
+)
+
+custom_sellmeier = CustomSellmeier(
+    coeffs=(
+        (
+            td.SpatialDataArray(0.1 + np.random.random((2, 2, 2)), coords=COORDS),
+            td.SpatialDataArray(10 + np.random.random((2, 2, 2)), coords=COORDS),
+        ),
+    ),
+)
+
 SIM_FULL = Simulation(
     size=(8.0, 8.0, 8.0),
     run_time=1e-12,
     structures=[
         Structure(
             geometry=Box(size=(1, 1, 1), center=(-1, 0, 0)),
             medium=Medium(permittivity=2.0),
@@ -84,14 +148,18 @@
             medium=Lorentz(eps_inf=2.0, coeffs=[(1, 2, 3)]),
         ),
         Structure(
             geometry=Box(size=(1, 1, 1), center=(-1, 0, 0)),
             medium=Debye(eps_inf=2.0, coeffs=[(1, 3)]),
         ),
         Structure(
+            geometry=STL_GEO,
+            medium=Debye(eps_inf=2.0, coeffs=[(1, 3)]),
+        ),
+        Structure(
             geometry=Box(size=(1, 1, 1), center=(-1, 0, 0)),
             medium=Drude(eps_inf=2.0, coeffs=[(1, 3)]),
         ),
         Structure(
             geometry=Box(size=(1, 0, 1), center=(-1, 0, 0)),
             medium=Medium2D.from_medium(Medium(conductivity=0.45), thickness=0.01),
         ),
@@ -109,14 +177,62 @@
         ),
         Structure(
             geometry=PolySlab(
                 vertices=[(-1.5, -1.5), (-0.5, -1.5), (-0.5, -0.5)], slab_bounds=[-1, 1]
             ),
             medium=PoleResidue(eps_inf=1.0, poles=((6206417594288582j, (-3.311074436985222e16j)),)),
         ),
+        Structure(
+            geometry=Box(
+                size=(1, 1, 1),
+                center=(-1.0, 0.5, 0.5),
+            ),
+            medium=custom_medium,
+        ),
+        Structure(
+            geometry=Box(
+                size=(1, 1, 1),
+                center=(-1.0, 0.5, 0.5),
+            ),
+            medium=custom_drude,
+        ),
+        Structure(
+            geometry=Box(
+                size=(1, 1, 1),
+                center=(-1.0, 0.5, 0.5),
+            ),
+            medium=custom_lorentz,
+        ),
+        Structure(
+            geometry=Box(
+                size=(1, 1, 1),
+                center=(-1.0, 0.5, 0.5),
+            ),
+            medium=custom_debye,
+        ),
+        Structure(
+            geometry=Box(
+                size=(1, 1, 1),
+                center=(-1.0, 0.5, 0.5),
+            ),
+            medium=custom_poleresidue,
+        ),
+        Structure(
+            geometry=Box(
+                size=(1, 1, 1),
+                center=(-1.0, 0.5, 0.5),
+            ),
+            medium=custom_sellmeier,
+        ),
+        Structure(
+            geometry=PolySlab(
+                vertices=[(-1.5, -1.5), (-0.5, -1.5), (-0.5, -0.5)], slab_bounds=[-1, 1]
+            ),
+            medium=PoleResidue(eps_inf=1.0, poles=((6206417594288582j, (-3.311074436985222e16j)),)),
+        ),
         Structure(
             geometry=TriangleMesh.from_triangles(
                 np.array(
                     [
                         [[1, 0, 0], [0, 1, 0], [0, 0, 1]],
                         [[0, 0, 0], [0, 0, 1], [0, 1, 0]],
                         [[0, 0, 0], [1, 0, 0], [0, 0, 1]],
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/__init__.py` & `tidy3d-2.3.1/tidy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/__main__.py` & `tidy3d-2.3.1/tidy3d/__main__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/apodization.py` & `tidy3d-2.3.1/tidy3d/components/apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/base.py` & `tidy3d-2.3.1/tidy3d/components/base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/boundary.py` & `tidy3d-2.3.1/tidy3d/components/boundary.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/data/data_array.py` & `tidy3d-2.3.1/tidy3d/components/data/data_array.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Storing tidy3d data at it's most fundamental level as xr.DataArray objects"""
 from __future__ import annotations
-from typing import Dict
+from typing import Dict, List
 
 import xarray as xr
 import numpy as np
 import dask
 import h5py
 
 from ...constants import HERTZ, SECOND, MICROMETER, RADIAN
@@ -110,15 +110,15 @@
     @classmethod
     def _json_encoder(cls, val):  # pylint:disable=unused-argument
         """What function to call when writing a DataArray to json."""
         return type(val).__name__
 
     def __eq__(self, other) -> bool:
         """Whether two data array objects are equal."""
-        if not np.all(self.data == other.data):
+        if not self.data.shape == other.data.shape or not np.all(self.data == other.data):
             return False
         for key, val in self.coords.items():
             if not np.all(np.array(val) == np.array(other.coords[key])):
                 return False
         return True
 
     @property
@@ -160,14 +160,20 @@
         return cls.from_hdf5(fname=fname, group_path=group_path)
 
     def __hash__(self) -> int:
         """Generate hash value for a :class:.`DataArray` instance, needed for custom components."""
         token_str = dask.base.tokenize(self)
         return hash(token_str)
 
+    def multiply_at(self, value: complex, coord_name: str, indices: List[int]) -> DataArray:
+        """Multiply self by value at indices into ."""
+        self_mult = self.copy()
+        self_mult[{coord_name: indices}] *= value
+        return self_mult
+
 
 class FreqDataArray(DataArray):
     """Frequency-domain array.
 
     Example
     -------
     >>> f = [2e14, 3e14]
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/data/dataset.py` & `tidy3d-2.3.1/tidy3d/components/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Collections of DataArrays."""
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Union, Dict, Callable
+from typing import Union, Dict, Callable, Any
 
 import xarray as xr
 import numpy as np
 import pydantic as pd
 
 from .data_array import DataArray
 from .data_array import ScalarFieldDataArray, ScalarFieldTimeDataArray, ScalarModeFieldDataArray
@@ -36,14 +36,18 @@
         """Maps field components to the string key of their grid locations on the yee lattice."""
 
     @property
     @abstractmethod
     def symmetry_eigenvalues(self) -> Dict[str, Callable[[Axis], float]]:
         """Maps field components to their (positive) symmetry eigenvalues."""
 
+    def package_colocate_results(self, centered_fields: Dict[str, ScalarFieldDataArray]) -> Any:
+        """How to package the dictionary of fields computed via self.colocate()."""
+        return xr.Dataset(centered_fields)
+
     def colocate(self, x=None, y=None, z=None) -> xr.Dataset:
         """colocate all of the data at a set of x, y, z coordinates.
 
         Parameters
         ----------
         x : Optional[array-like] = None
             x coordinates of locations.
@@ -75,29 +79,29 @@
         centered_fields = {}
 
         # loop through field components
         for field_name, field_data in self.field_components.items():
 
             # loop through x, y, z dimensions and raise an error if only one element along dim
             for coord_name, coords_supplied in supplied_coord_map.items():
-                coord_data = field_data.coords[coord_name]
+                coord_data = np.array(field_data.coords[coord_name])
                 if coord_data.size == 1:
                     raise DataError(
                         f"colocate given {coord_name}={coords_supplied}, but "
-                        f"data only has one coordinate at {coord_name}={coord_data.values[0]}. "
+                        f"data only has one coordinate at {coord_name}={coord_data[0]}. "
                         "Therefore, can't colocate along this dimension. "
                         f"supply {coord_name}=None to skip it."
                     )
 
             centered_fields[field_name] = field_data.interp(
                 **supplied_coord_map, kwargs={"bounds_error": True}
             )
 
         # combine all centered fields in a dataset
-        return xr.Dataset(centered_fields)
+        return self.package_colocate_results(centered_fields)
 
 
 EMScalarFieldType = Union[ScalarFieldDataArray, ScalarFieldTimeDataArray, ScalarModeFieldDataArray]
 
 
 class ElectromagneticFieldDataset(AbstractFieldDataset, ABC):
     """Stores a collection of E and H fields with x, y, z components."""
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/data/monitor_data.py` & `tidy3d-2.3.1/tidy3d/components/data/monitor_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pylint:disable=too-many-lines
 """ Monitor Level Data, store the DataArrays associated with a single monitor."""
 from __future__ import annotations
 
 from abc import ABC
-from typing import Union, Tuple, Callable, Dict, List
+from typing import Union, Tuple, Callable, Dict, List, Any
 import warnings
 
 import xarray as xr
 import numpy as np
 import pydantic as pd
 
 from .data_array import FluxTimeDataArray, FluxDataArray
@@ -17,24 +17,25 @@
 from .data_array import DataArray, DiffractionDataArray
 from .data_array import ScalarFieldDataArray, ScalarFieldTimeDataArray
 from .data_array import FreqDataArray, TimeDataArray, FreqModeDataArray
 from .dataset import Dataset, AbstractFieldDataset, ElectromagneticFieldDataset
 from .dataset import FieldDataset, FieldTimeDataset, ModeSolverDataset, PermittivityDataset
 from ..base import TYPE_TAG_STR, cached_property
 from ..types import Coordinate, Symmetry, ArrayFloat1D, ArrayFloat2D, Size, Numpy, TrackFreq
+from ..types import EpsSpecType
 from ..grid.grid import Grid, Coords
 from ..validators import enforce_monitor_fields_present, required_if_symmetry_present
 from ..monitor import MonitorType, FieldMonitor, FieldTimeMonitor, ModeSolverMonitor
 from ..monitor import ModeMonitor, FluxMonitor, FluxTimeMonitor, PermittivityMonitor
 from ..monitor import FieldProjectionAngleMonitor, FieldProjectionCartesianMonitor
 from ..monitor import FieldProjectionKSpaceMonitor, FieldProjectionSurface
 from ..monitor import DiffractionMonitor
 from ..source import SourceTimeType, CustomFieldSource
 from ..medium import Medium, MediumType
-from ...exceptions import SetupError, DataError, Tidy3dNotImplementedError
+from ...exceptions import SetupError, DataError, Tidy3dNotImplementedError, ValidationError
 from ...constants import ETA_0, C_0, MICROMETER
 from ...log import log
 
 
 Coords1D = ArrayFloat1D
 
 
@@ -100,15 +101,14 @@
             A data object with the symmetry expanded fields.
         """
 
         if all(sym == 0 for sym in self.symmetry):
             return self.copy()
 
         update_dict = {}
-
         for field_name, scalar_data in self.field_components.items():
 
             eigenval_fn = self.symmetry_eigenvalues[field_name]
 
             # get grid locations for this field component on the expanded grid
             field_coords = self._expanded_grid_field_coords(field_name)
 
@@ -134,15 +134,17 @@
                 # when handling modes, in which case they should be at the boundary and close to 0.
                 scalar_data = scalar_data.sel({dim_name: coords_interp}, method="nearest")
                 scalar_data = scalar_data.assign_coords({dim_name: coords})
 
                 # apply the symmetry eigenvalue (if defined) to the flipped values
                 if eigenval_fn is not None:
                     sym_eigenvalue = eigenval_fn(sym_dim)
-                    scalar_data[{dim_name: flip_inds}] *= sym_val * sym_eigenvalue
+                    scalar_data = scalar_data.multiply_at(
+                        value=sym_val * sym_eigenvalue, coord_name=dim_name, indices=flip_inds
+                    )
 
             # assign the final scalar data to the update_dict
             update_dict[field_name] = scalar_data
 
         update_dict.update({"symmetry": (0, 0, 0), "symmetry_center": None})
         return self.copy(update=update_dict)
 
@@ -191,28 +193,24 @@
             raise DataError("Data must be 2D to get tangential dimensions.")
         tangential_dims = ["x", "y", "z"]
         tangential_dims.pop(self.monitor.zero_dims[0])
 
         return tangential_dims
 
     @property
-    def _grid_corrected_fields(self) -> Dict[str, DataArray]:
+    def _in_plane(self) -> Dict[str, DataArray]:
         """Dictionary of field components with finite grid correction factors applied and symmetry
         expanded."""
         if len(self.monitor.zero_dims) != 1:
             raise DataError("Data must be 2D to apply grid corrections.")
+
         normal_dim = "xyz"[self.monitor.zero_dims[0]]
         fields = {}
-        for field_name, field in self.symmetry_expanded_copy.field_components.items():
-            eig_val = self.symmetry_eigenvalues[field_name](normal_dim)
-            if eig_val < 0:
-                fields[field_name] = field * self.grid_dual_correction
-            else:
-                fields[field_name] = field * self.grid_primal_correction
-            fields[field_name] = fields[field_name].squeeze(dim=normal_dim, drop=True)
+        for field_name, field in self.grid_corrected_copy.field_components.items():
+            fields[field_name] = field.squeeze(dim=normal_dim, drop=True)
         return fields
 
     @property
     def _plane_grid_boundaries(self) -> Tuple[Coords1D, Coords1D]:
         """For a 2D monitor data, return the boundaries of the in-plane grid to be used to compute
         differential area and to colocate fields to grid centers if needed."""
         if np.any(np.array(self.monitor.interval_space) > 1):
@@ -229,16 +227,16 @@
             plane_bounds1 = np.unique(self.grid_expanded.boundaries.to_dict[dim1])
             plane_bounds2 = np.unique(self.grid_expanded.boundaries.to_dict[dim2])
         else:
             # Last pixel missing compared to sim.discretize(self.monitor, extend=True).
             # This is because we cannot colocate the fields to the center of that pixel.
             # However, the monitor should be completely outside of this last pixel.
             fields = self.symmetry_expanded_copy.field_components
-            plane_bounds1 = fields["E" + dim2].coords[dim1].values
-            plane_bounds2 = fields["E" + dim1].coords[dim2].values
+            plane_bounds1 = np.array(fields["E" + dim2].coords[dim1])
+            plane_bounds2 = np.array(fields["E" + dim1].coords[dim2])
 
         return plane_bounds1, plane_bounds2
 
     @property
     def _plane_grid_centers(self) -> Tuple[Coords1D, Coords1D]:
         """For 2D monitor data, return the centers of the in-plane grid"""
         return [(bs[1:] + bs[:-1]) / 2 for bs in self._plane_grid_boundaries]
@@ -301,27 +299,28 @@
         are oriented such that the third component would be the normal axis. This just means that
         the H field gets an extra minus sign if the normal axis is ``"y"``.
 
         Note
         ----
             The finite grid correction factors are applied and symmetry is expanded.
         """
-        return self._tangential_corrected(self._grid_corrected_fields)
+        return self._tangential_corrected(self._in_plane)
 
     @property
     def _centered_fields(self) -> Dict[str, DataArray]:
         """For a 2D monitor data, get all E and H fields colocated to the cell centers in the 2D
         plane grid.
 
         Note
         ----
             The finite grid correction factors are applied and symmetry is expanded.
         """
 
-        field_components = self._grid_corrected_fields
+        field_components = self._in_plane
+
         if self.monitor.colocate:
             return field_components
 
         # Interpolate field components to cell centers
         interp_dict = {"assume_sorted": True}
         for dim, cents in zip(self._tangential_dims, self._plane_grid_centers):
             if cents.size > 0:
@@ -341,14 +340,32 @@
         Note
         ----
             The finite grid correction factors are applied and symmetry is expanded.
         """
         return self._tangential_corrected(self._centered_fields)
 
     @property
+    def grid_corrected_copy(self) -> ElectromagneticFieldData:
+        """Return a copy of self with grid correction factors applied (if necessary) and symmetry
+        expanded."""
+        field_data = self.symmetry_expanded_copy
+        if len(self.monitor.zero_dims) != 1:
+            return field_data
+
+        normal_dim = "xyz"[self.monitor.zero_dims[0]]
+        update = {"grid_primal_correction": 1.0, "grid_dual_correction": 1.0}
+        for field_name, field in field_data.field_components.items():
+            eig_val = self.symmetry_eigenvalues[field_name](normal_dim)
+            if eig_val < 0:
+                update[field_name] = field * self.grid_dual_correction
+            else:
+                update[field_name] = field * self.grid_primal_correction
+        return field_data.copy(update=update)
+
+    @property
     def intensity(self) -> ScalarFieldDataArray:
         """Return the sum of the squared absolute electric field components."""
         fields = self._centered_fields
         components = ("Ex", "Ey", "Ez")
         if any(cmp not in fields for cmp in components):
             raise KeyError("Can't compute intensity, all E field components must be present.")
         return sum(fields[cmp].abs ** 2 for cmp in components)
@@ -357,26 +374,36 @@
     def poynting(self) -> ScalarFieldDataArray:
         """Time-averaged Poynting vector for frequency-domain data associated to a 2D monitor,
         projected to the direction normal to the monitor plane."""
 
         # Tangential fields are ordered as E1, E2, H1, H2
         tan_fields = self._centered_tangential_fields
         dim1, dim2 = self._tangential_dims
+
         e_x_h_star = tan_fields["E" + dim1] * tan_fields["H" + dim2].conj()
         e_x_h_star -= tan_fields["E" + dim2] * tan_fields["H" + dim1].conj()
         poynting = 0.5 * np.real(e_x_h_star)
         return poynting
 
+    def package_flux_results(self, flux_values: xr.DataArray) -> Any:
+        """How to package flux"""
+        return FluxDataArray(flux_values)
+
     @cached_property
     def flux(self) -> FluxDataArray:
         """Flux for data corresponding to a 2D monitor."""
 
         # Compute flux by integrating Poynting vector in-plane
         d_area = self._diff_area
-        return FluxDataArray((self.poynting * d_area).sum(dim=d_area.dims))
+        poynting = self.poynting
+
+        flux_values = poynting * d_area
+        flux_values = flux_values.sum(dim=d_area.dims)
+
+        return self.package_flux_results(flux_values)
 
     @cached_property
     def mode_area(self) -> FreqModeDataArray:
         """Effective mode area corresponding to a 2D monitor.
 
         Effective mode area is calculated as: (∫|E|²dA)² / (∫|E|⁴dA)
         """
@@ -411,17 +438,17 @@
 
         Note
         ----
             The dot product with and without conjugation is equivalent (up to a phase) for
             modes in lossless waveguides but differs for modes in lossy materials. In that case,
             the conjugated dot product can be interpreted as the fraction of the power of the first
             mode carried by the second, but modes are not orthogonal with respect to that product
-            and the sum of carried power fractions exceed 1. In the non-conjugated definition,
-            orthogonal modes can be defined, but the interpretation of modal overlap as power
-            carried by a given mode is no longer valid.
+            and the sum of carried power fractions may be different from the total flux.
+            In the non-conjugated definition, modes are orthogonal, but the interpretation of the
+            dot product power carried by a given mode is no longer valid.
         """
 
         # Tangential fields for current and other field data
         fields_self = self._centered_tangential_fields
         # pylint:disable=protected-access
         fields_other = field_data._centered_tangential_fields
         if conjugate:
@@ -472,29 +499,30 @@
         self, field_data: Union[FieldData, ModeSolverData], conjugate: bool = True
     ) -> MixedModeDataArray:
         """Dot product (modal overlap) with another :class:`.FieldData` object.
 
         The tangential fields from ``field_data`` are interpolated to this object's grid, so the
         data arrays don't need to have the same discretization.  The calculation is performed for
         all common frequencies between data arrays.  In the output, ``mode_index_0`` and
-        ``mode_index_1`` are the mode indices from this object and ``field_data``, respectively.
+        ``mode_index_1`` are the mode indices from this object and ``field_data``, respectively, if
+        they are instances of ``ModeSolverData``.
 
         Parameters
         ----------
         field_data : :class:`ElectromagneticFieldData`
             A data instance to compute the dot product with.
         conjugate : bool = True
             If ``True`` (default), the dot product is defined as ``1 / 4`` times the integral of
             ``E_self* x H_other - H_self* x E_other``, where ``x`` is the cross product and ``*`` is
             complex conjugation. If ``False``, the complex conjugation is skipped.
 
         Returns
         -------
-        :class:`.MixedModeDataArray`
-            Dataset with the complex-valued modal overlaps between the two mode data.
+        :class:`xarray.DataArray`
+            Data array with the complex-valued modal overlaps between the two mode data.
 
         See also
         --------
         :member:`dot`
         """
 
         tan_dims = self._tangential_dims
@@ -518,52 +546,73 @@
         e_2 = "E" + dim2
         h_1 = "H" + dim1
         h_2 = "H" + dim2
 
         # Prepare array with proper dimensions for the dot product data
         arrays = (fields_self[e_1], fields_other[e_1])
         coords = (arrays[0].coords, arrays[1].coords)
+
         # Common frequencies to both data arrays
         f = np.array(sorted(set(coords[0]["f"].values).intersection(coords[1]["f"].values)))
-        mode_index_0 = coords[0]["mode_index"].values
-        mode_index_1 = coords[1]["mode_index"].values
+
+        # Mode indices, if available
+        modes_in_self = "mode_index" in coords[0]
+        mode_index_0 = coords[0]["mode_index"].values if modes_in_self else np.zeros(1, dtype=int)
+        modes_in_other = "mode_index" in coords[1]
+        mode_index_1 = coords[1]["mode_index"].values if modes_in_other else np.zeros(1, dtype=int)
+
         dtype = np.promote_types(arrays[0].dtype, arrays[1].dtype)
         dot = np.empty((f.size, mode_index_0.size, mode_index_1.size), dtype=dtype)
 
         # Calculate overlap for each common frequency and each mode pair
         for i, freq in enumerate(f):
+            indexer_self = {"f": freq}
+            indexer_other = {"f": freq}
             for mi0 in mode_index_0:
-                e_self_1 = fields_self[e_1].sel(f=freq, mode_index=mi0, drop=True)
-                e_self_2 = fields_self[e_2].sel(f=freq, mode_index=mi0, drop=True)
-                h_self_1 = fields_self[h_1].sel(f=freq, mode_index=mi0, drop=True)
-                h_self_2 = fields_self[h_2].sel(f=freq, mode_index=mi0, drop=True)
+                if modes_in_self:
+                    indexer_self["mode_index"] = mi0
+                e_self_1 = fields_self[e_1].sel(indexer_self, drop=True)
+                e_self_2 = fields_self[e_2].sel(indexer_self, drop=True)
+                h_self_1 = fields_self[h_1].sel(indexer_self, drop=True)
+                h_self_2 = fields_self[h_2].sel(indexer_self, drop=True)
 
                 for mi1 in mode_index_1:
-                    e_other_1 = fields_other[e_1].sel(f=freq, mode_index=mi1, drop=True)
-                    e_other_2 = fields_other[e_2].sel(f=freq, mode_index=mi1, drop=True)
-                    h_other_1 = fields_other[h_1].sel(f=freq, mode_index=mi1, drop=True)
-                    h_other_2 = fields_other[h_2].sel(f=freq, mode_index=mi1, drop=True)
+                    if modes_in_other:
+                        indexer_other["mode_index"] = mi1
+                    e_other_1 = fields_other[e_1].sel(indexer_other, drop=True)
+                    e_other_2 = fields_other[e_2].sel(indexer_other, drop=True)
+                    h_other_1 = fields_other[h_1].sel(indexer_other, drop=True)
+                    h_other_2 = fields_other[h_2].sel(indexer_other, drop=True)
 
                     # Cross products of fields
                     e_self_x_h_other = e_self_1 * h_other_2 - e_self_2 * h_other_1
                     h_self_x_e_other = h_self_1 * e_other_2 - h_self_2 * e_other_1
 
                     # Integrate over plane
                     d_area = self._diff_area
                     integrand = (e_self_x_h_other - h_self_x_e_other) * d_area
                     dot[i, mi0, mi1] = 0.25 * integrand.sum(dim=d_area.dims)
 
         coords = {"f": f, "mode_index_0": mode_index_0, "mode_index_1": mode_index_1}
-        return MixedModeDataArray(dot, coords=coords)
+        result = xr.DataArray(dot, coords=coords)
+
+        # Remove mode index coordinate if the input did not have it
+        if not modes_in_self:
+            result = result.isel(mode_index_0=0, drop=True)
+        if not modes_in_other:
+            result = result.isel(mode_index_1=0, drop=True)
+
+        return result
 
     @property
     def time_reversed_copy(self) -> FieldData:
         """Make a copy of the data with time-reversed fields."""
 
-        # Time reversal for frequency-domain fields; overwritten in :class:`FieldTimeData`.
+        # Time reversal for frequency-domain fields; overwritten in :class:`FieldTimeData`
+        # and :class:`ModeSolverData`.
         new_data = {}
         for comp, field in self.field_components.items():
             if comp[0] == "H":
                 new_data[comp] = -np.conj(field)
             else:
                 new_data[comp] = np.conj(field)
         return self.copy(update=new_data)
@@ -738,14 +787,32 @@
     ... )
     """
 
     monitor: ModeSolverMonitor = pd.Field(
         ..., title="Monitor", description="Mode solver monitor associated with the data."
     )
 
+    eps_spec: List[EpsSpecType] = pd.Field(
+        None,
+        title="Permettivity Specification",
+        description="Characterization of the permittivity profile on the plane where modes are "
+        "computed. Possible values are 'diagonal', 'tensorial_real', 'tensorial_complex'.",
+    )
+
+    @pd.validator("eps_spec", always=True)
+    def eps_spec_match_mode_spec(cls, val, values):
+        """Raise validation error if frequencies in eps_spec does not match frequency list"""
+        if val:
+            mode_data_freqs = values["monitor"].freqs
+            if len(val) != len(mode_data_freqs):
+                raise ValidationError(
+                    "eps_spec must be provided at the same frequencies as mode solver data."
+                )
+        return val
+
     # pylint:disable=too-many-locals
     def overlap_sort(
         self,
         track_freq: TrackFreq,
         overlap_thresh: float = 0.9,
     ) -> ModeSolverData:
         """Starting from the base frequency defined by parameter ``track_freq``, sort modes at each
@@ -846,14 +913,16 @@
         """Find new ordering of modes in data_to_sort based on their similarity to own modes."""
 
         num_modes = self.n_complex.sizes["mode_index"]
 
         # Current pairs and their overlaps
         pairs = np.arange(num_modes)
         complex_amps = self.dot(data_to_sort).data.ravel()
+        if self.monitor.direction == "-":
+            complex_amps *= -1
 
         # Check whether modes already match
         modes_to_sort = np.where(np.abs(complex_amps) < overlap_thresh)[0]
         num_modes_to_sort = len(modes_to_sort)
         if num_modes_to_sort <= 1:
             return pairs, complex_amps
 
@@ -867,14 +936,16 @@
 
             # Get one mode from data_to_sort
             # pylint:disable=protected-access
             one_mode = data_to_sort._isel(mode_index=[mode_index])
 
             # Project to all modes of interest from data_template
             amps_reduced[:, i] = data_template_reduced.dot(one_mode).data.ravel()
+            if self.monitor.direction == "-":
+                amps_reduced[:, i] *= -1
 
         # Find the most similar modes and corresponding overlap values
         pairs_reduced, amps_reduced = self._find_closest_pairs(amps_reduced)
 
         # Insert new sorting and overlap values into arrays with all data
         complex_amps[modes_to_sort] = amps_reduced
         pairs[modes_to_sort] = modes_to_sort[pairs_reduced]
@@ -941,14 +1012,85 @@
 
         # Update mode_spec in the monitor
         mode_spec = self.monitor.mode_spec.copy(update=dict(track_freq=track_freq))
         update_dict["monitor"] = self.monitor.copy(update=dict(mode_spec=mode_spec))
 
         return self.copy(update=update_dict)
 
+    def _group_index_post_process(self, frequency_step: float) -> ModeSolverData:
+        """Calculate group index and remove added frequencies used only for this calculation.
+
+        Parameters
+        ----------
+        frequency_step: float
+            Fractional frequency step used to calculate the group index.
+
+        Returns
+        -------
+        :class:`.ModeSolverData`
+            Filtered data with calulated group index.
+        """
+
+        freqs = self.n_complex.coords["f"].values
+        num_freqs = freqs.size
+        back = slice(0, num_freqs, 3)
+        center = slice(1, num_freqs, 3)
+        fwd = slice(2, num_freqs, 3)
+
+        # calculate group index
+        n_center = self.n_eff.isel(f=center).values
+        n_backward = self.n_eff.isel(f=back).values
+        n_forward = self.n_eff.isel(f=fwd).values
+
+        n_group_data = n_center + (n_forward - n_backward) / (2 * frequency_step)
+        n_group = ModeIndexDataArray(
+            n_group_data,
+            coords={
+                "f": list(freqs[center]),
+                "mode_index": list(self.n_complex.coords["mode_index"].values),
+            },
+            attrs={"long name": "Group index"},
+        )
+
+        # remove data corresponding to frequencies used only for group index calculation
+        update_dict = {"n_complex": self.n_complex.isel(f=center), "n_group": n_group}
+
+        for key, field in self.field_components.items():
+            update_dict[key] = field.isel(f=center)
+
+        # pylint: disable=protected-access
+        for key, data in self._grid_correction_dict.items():
+            update_dict[key] = data.isel(f=center)
+
+        if self.eps_spec:
+            update_dict["eps_spec"] = self.eps_spec[center]
+
+        update_dict["monitor"] = self.monitor.updated_copy(freqs=freqs[center])
+
+        return self.copy(update=update_dict)
+
+    @property
+    def time_reversed_copy(self) -> FieldData:
+        """Make a copy of the data with direction-reversed fields. In lossy or gyrotropic systems,
+        the time-reversed fields will not be the same as the backward-propagating modes."""
+
+        # Time reversal
+        new_data = {}
+        for comp, field in self.field_components.items():
+            if comp[0] == "H":
+                new_data[comp] = -np.conj(field)
+            else:
+                new_data[comp] = np.conj(field)
+
+        # switch direction in the monitor
+        mnt = self.monitor
+        new_direction = "+" if mnt.direction == "-" else "-"
+        new_data["monitor"] = mnt.updated_copy(direction=new_direction)
+        return self.copy(update=new_data)
+
 
 class PermittivityData(PermittivityDataset, AbstractFieldData):
     """Data for a :class:`.PermittivityMonitor`: diagonal components of the permittivity tensor.
 
     Example
     -------
     >>> from tidy3d import ScalarFieldDataArray
@@ -1000,14 +1142,20 @@
 
     n_complex: ModeIndexDataArray = pd.Field(
         ...,
         title="Propagation Index",
         description="Complex-valued effective propagation constants associated with the mode.",
     )
 
+    n_group: ModeIndexDataArray = pd.Field(
+        None,
+        title="Group Index",
+        description="Index associated with group velocity of the mode.",
+    )
+
     @property
     def n_eff(self):
         """Real part of the propagation index."""
         return self.n_complex.real
 
     @property
     def k_eff(self):
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/data/sim_data.py` & `tidy3d-2.3.1/tidy3d/components/data/sim_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,16 +212,31 @@
         Returns
         -------
         xarray.Dataset
             Dataset containing all of the fields in the data
             interpolated to center locations on Yee grid.
         """
 
-        # get the data
-        monitor_data = self.load_field_monitor(field_monitor_name)
+        return self._at_centers(self.load_field_monitor(field_monitor_name))
+
+    def _at_centers(self, monitor_data: xr.Dataset) -> xr.Dataset:
+        """return xarray.Dataset representation of field monitor data
+        co-located at Yee cell centers.
+
+        Parameters
+        ----------
+        monitor_data : xr.Dataset
+            Monitor data to be co-located.
+
+        Returns
+        -------
+        xarray.Dataset
+            Dataset containing all of the fields in the data
+            interpolated to center locations on Yee grid.
+        """
 
         # discretize the monitor and get center locations
         sub_grid = self.simulation.discretize(monitor_data.monitor, extend=False)
         centers = sub_grid.centers
 
         # pass coords if each of the scalar field data have more than one coordinate along a dim
         xyz_kwargs = {}
@@ -229,14 +244,15 @@
             scalar_data = list(monitor_data.field_components.values())
             coord_lens = [len(data.coords[dim]) for data in scalar_data]
             if all(ncoords > 1 for ncoords in coord_lens):
                 xyz_kwargs[dim] = centers
 
         return monitor_data.colocate(**xyz_kwargs)
 
+    # pylint: disable=too-many-locals
     def get_poynting_vector(self, field_monitor_name: str) -> xr.Dataset:
         """return ``xarray.Dataset`` of the Poynting vector at Yee cell centers.
 
         Calculated values represent the instantaneous Poynting vector for time-domain fields and the
         complex vector for frequency-domain: ``S = 1/2 E × conj(H)``.
 
         Only the available components are returned, e.g., if the indicated monitor doesn't include
@@ -249,16 +265,17 @@
 
         Returns
         -------
         xarray.DataArray
             DataArray containing the Poynting vector calculated based on the field components
             colocated at the center locations of the Yee grid.
         """
-
-        field_dataset = self.at_centers(field_monitor_name)
+        # Fields from 2D monitors need a correction factor
+        mon_data = self.load_field_monitor(field_monitor_name).grid_corrected_copy
+        field_dataset = self._at_centers(mon_data)
 
         time_domain = isinstance(self.monitor_data[field_monitor_name], FieldTimeData)
 
         poynting_components = {}
 
         dims = "xyz"
         for axis, dim in enumerate(dims):
@@ -365,20 +382,21 @@
                 derived_data.name = f"|Re{{{field_name}}}|"
 
             elif val == "imag":
                 derived_data = sum(f.imag**2 for f in field_components) ** 0.5
                 derived_data.name = f"|Im{{{field_name}}}|"
 
             elif val == "abs":
-                derived_data = sum(np.abs(f) ** 2 for f in field_components) ** 0.5
+                derived_data = sum(abs(f) ** 2 for f in field_components) ** 0.5
                 derived_data.name = f"|{field_name}|"
 
             elif val == "abs^2":
-                derived_data = sum(np.abs(f) ** 2 for f in field_components)
-                derived_data.name = f"|{field_name}|²"
+                derived_data = sum(abs(f) ** 2 for f in field_components)
+                if hasattr(derived_data, "name"):
+                    derived_data.name = f"|{field_name}|²"
 
             elif val == "phase":
                 raise Tidy3dKeyError(f"Phase is not defined for complex vector {field_name}")
 
             return derived_data
 
         raise Tidy3dKeyError(
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/field_projection.py` & `tidy3d-2.3.1/tidy3d/components/field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/geometry.py` & `tidy3d-2.3.1/tidy3d/components/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import List, Tuple, Union, Any, Callable, Optional
 from math import isclose
 import functools
 
 import pydantic
 import numpy as np
 from matplotlib import patches, path
+from shapely import unary_union
 from shapely.geometry import Point, Polygon, box, MultiPolygon, LineString
 from shapely.validation import make_valid
 
 from .base import Tidy3dBaseModel, cached_property
 from .types import Bound, Size, Coordinate, Axis, Coordinate2D, ArrayFloat3D, PlanePosition
 from .types import Vertices, Ax, Shapely, annotate_type
 from .viz import add_ax_if_none, equal_aspect
@@ -46,14 +47,16 @@
 # non self-intersecting during the entire dilation process
 _N_SAMPLE_POLYGON_INTERSECT = 5
 # for sampling conical frustum in visualization
 _N_SAMPLE_CURVE_SHAPELY = 40
 _IS_CLOSE_RTOL = np.finfo(float).eps
 # for shapely circular shapes discretization in visualization
 _N_SHAPELY_QUAD_SEGS = 200
+# polygon merge
+POLY_GRID_SIZE = 1e-12
 
 
 Points = ArrayFloat3D
 
 
 # pylint:disable=too-many-public-methods
 class Geometry(Tidy3dBaseModel, ABC):
@@ -420,14 +423,16 @@
 
     def plot_shape(self, shape: Shapely, plot_params: PlotParams, ax: Ax) -> Ax:
         """Defines how a shape is plotted on a matplotlib axes."""
         _shape = self.evaluate_inf_shape(shape)
         if isinstance(_shape, LineString):
             xs, ys = zip(*_shape.coords)
             ax.plot(xs, ys, color=plot_params.edgecolor)
+        elif isinstance(_shape, Point):
+            ax.scatter(shape.x, shape.y, color=plot_params.facecolor)
         else:
             patch = polygon_patch(_shape, **plot_params.to_kwargs())
             ax.add_artist(patch)
         return ax
 
     @classmethod
     def strip_coords(
@@ -1268,14 +1273,15 @@
         """
         exclude_surfaces = kwargs.pop("exclude_surfaces", None)
         surfaces = cls.surfaces(size=size, center=center, **kwargs)
         if "name" in cls.__dict__["__fields__"] and exclude_surfaces:
             surfaces = [surf for surf in surfaces if surf.name[-2:] not in exclude_surfaces]
         return surfaces
 
+    # pylint:disable=too-many-locals
     def intersections_plane(self, x: float = None, y: float = None, z: float = None):
         """Returns shapely geometry at plane specified by one non None value of x,y,z.
 
         Parameters
         ----------
         x : float = None
             Position of plane in x direction, only one of x,y,z can be specified to define plane.
@@ -1295,15 +1301,25 @@
         if not self.intersects_axis_position(axis, position):
             return []
         z0, (x0, y0) = self.pop_axis(self.center, axis=axis)
         Lz, (Lx, Ly) = self.pop_axis(self.size, axis=axis)
         dz = np.abs(z0 - position)
         if dz > Lz / 2 + fp_eps:
             return []
-        return [box(minx=x0 - Lx / 2, miny=y0 - Ly / 2, maxx=x0 + Lx / 2, maxy=y0 + Ly / 2)]
+
+        minx = x0 - Lx / 2
+        miny = y0 - Ly / 2
+        maxx = x0 + Lx / 2
+        maxy = y0 + Ly / 2
+
+        # handle case where the box vertices are identical
+        if isclose(minx, maxx) and isclose(miny, maxy):
+            return [Point(minx, miny)]
+
+        return [box(minx=minx, miny=miny, maxx=maxx, maxy=maxy)]
 
     def inside(
         self, x: np.ndarray[float], y: np.ndarray[float], z: np.ndarray[float]
     ) -> np.ndarray[bool]:
         """For input arrays ``x``, ``y``, ``z`` of arbitrary but identical shape, return an array
         with the same shape which is ``True`` for every point in zip(x, y, z) that is inside the
         volume of the :class:`Geometry`, and ``False`` otherwise.
@@ -2302,18 +2318,16 @@
             )
 
         all_vertices = gds_loader_fn(
             gds_cell=gds_cell, gds_layer=gds_layer, gds_dtype=gds_dtype, gds_scale=gds_scale
         )
 
         # convert vertices into polyslabs
-        polygons = (Polygon(vertices) for vertices in all_vertices)
-        polys_union = functools.reduce(
-            lambda poly1, poly2: poly1.union(poly2, grid_size=1e-12), polygons
-        )
+        polygons = [Polygon(vertices).buffer(0) for vertices in all_vertices]
+        polys_union = unary_union(polygons, grid_size=POLY_GRID_SIZE)
 
         if isinstance(polys_union, Polygon):
             all_vertices = [PolySlab.strip_coords(polys_union)[0]]
         elif isinstance(polys_union, MultiPolygon):
             all_vertices = [PolySlab.strip_coords(polygon)[0] for polygon in polys_union.geoms]
         return all_vertices
 
@@ -2689,18 +2703,25 @@
                     x3, y3 = self._order_by_axis(
                         plane_val=y_max - dy_max, axis_val=z_max, axis=axis
                     )
                     x4, y4 = self._order_by_axis(
                         plane_val=y_min + dy_min, axis_val=z_max, axis=axis
                     )
                     vertices = ((x1, y1), (x2, y2), (x3, y3), (x4, y4))
-                    polys.append(Polygon(vertices))
+                    polys.append(Polygon(vertices).buffer(0))
             # update the base coordinate for the next subsection
             h_base = h_top
 
+        # merge touching polygons
+        polys_union = unary_union(polys, grid_size=POLY_GRID_SIZE)
+        if isinstance(polys_union, Polygon):
+            return [polys_union]
+        if isinstance(polys_union, MultiPolygon):
+            return polys_union.geoms
+        # in other cases, just return the original unmerged polygons
         return polys
 
     def _find_intersecting_height(self, position: float, axis: int) -> np.ndarray:
         """Found a list of height where the plane will intersect with the vertices;
         For vertical sidewall, just return np.array([]).
         Assumes axis is handles so this function works on xy plane.
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/grid/grid.py` & `tidy3d-2.3.1/tidy3d/components/grid/grid.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Defines the FDTD grid."""
-
-from typing import Tuple, List
+from __future__ import annotations
+from typing import Tuple, List, Union
 
 import numpy as np
 import pydantic as pd
 
 from ..base import Tidy3dBaseModel, cached_property
-from ..types import ArrayFloat1D, Axis, TYPE_TAG_STR
+from ..data.data_array import DataArray, SpatialDataArray, ScalarFieldDataArray
+from ..types import ArrayFloat1D, Axis, TYPE_TAG_STR, InterpMethod, Literal
 from ..geometry import Box
 
 from ...exceptions import SetupError
 
 # data type of one dimensional coordinate array.
 Coords1D = ArrayFloat1D
 
@@ -44,14 +45,104 @@
         return {key: np.array(value) for key, value in self.dict(exclude={TYPE_TAG_STR}).items()}
 
     @cached_property
     def to_list(self):
         """Return a list of the three Coord1D objects as numpy arrays."""
         return list(self.to_dict.values())
 
+    def spatial_interp(
+        self,
+        array: Union[SpatialDataArray, ScalarFieldDataArray],
+        interp_method: InterpMethod,
+        fill_value: Union[Literal["extrapolate"], float] = "extrapolate",
+    ) -> Union[SpatialDataArray, ScalarFieldDataArray]:
+        """
+        Similar to ``xarrray.DataArray.interp`` with 2 enhancements:
+
+            1) Check if the coordinate of the supplied data are in monotonically increasing order.
+            If they are, apply the faster ``assume_sorted=True``.
+
+            2) For axes of single entry, instead of error, apply ``isel()`` along the axis.
+
+        Parameters
+        ----------
+        array : Union[:class:`.SpatialDataArray`, :class:`.ScalarFieldDataArray`]
+            Supplied scalar dataset
+        interp_method : :class:`.InterpMethod`
+            Interpolation method.
+        fill_value : Union[Literal['extrapolate'], float] = "extrapolate"
+            Value used to fill in for points outside the data range. If set to 'extrapolate',
+            values will be extrapolated into those regions using the "nearest" method.
+
+        Returns
+        -------
+        Union[:class:`.SpatialDataArray`, :class:`.ScalarFieldDataArray`]
+            The interpolated spatial dataset.
+
+        Note
+        ----
+        This method is called from a :class:`Coords` instance with the array to be interpolated as
+        an argument, not the other way around.
+        """
+
+        # Check for empty dimensions
+        result_coords = dict(self.to_dict)
+        if any(len(v) == 0 for v in result_coords.values()):
+            for c in array.coords:
+                if c not in result_coords:
+                    result_coords[c] = array.coords[c].values
+            result_shape = tuple(len(v) for v in result_coords.values())
+            result = DataArray(np.empty(result_shape, dtype=array.dtype), coords=result_coords)
+            return result
+
+        # Check wich axes need interpolation or selection
+        interp_ax = []
+        isel_ax = []
+        for ax in "xyz":
+            if array.sizes[ax] == 1:
+                isel_ax.append(ax)
+            else:
+                interp_ax.append(ax)
+
+        # apply iselection for the axis containing single entry
+        if len(isel_ax) > 0:
+            array = array.isel({ax: [0] * len(self.to_dict[ax]) for ax in isel_ax})
+            array = array.assign_coords({ax: self.to_dict[ax] for ax in isel_ax})
+            if len(interp_ax) == 0:
+                return array
+
+        # Apply interp for the rest
+        is_sorted = all((np.all(np.diff(array.coords[f]) > 0) for f in interp_ax))
+        interp_param = {
+            "method": interp_method,
+            "assume_sorted": is_sorted,
+            "kwargs": {
+                "bounds_error": False,
+                "fill_value": fill_value,
+            },
+        }
+
+        # Mark extrapolated points with nan's to fill in later
+        if fill_value == "extrapolate" and interp_method != "nearest":
+            interp_param["kwargs"]["fill_value"] = np.nan
+
+        # interpolation
+        interp_array = array.interp({ax: self.to_dict[ax] for ax in interp_ax}, **interp_param)
+
+        # Fill in nan's with nearest values
+        if fill_value == "extrapolate" and interp_method != "nearest":
+            interp_param["method"] = "nearest"
+            interp_param["kwargs"]["fill_value"] = "extrapolate"
+            nearest_array = array.interp({ax: self.to_dict[ax] for ax in interp_ax}, **interp_param)
+            interp_array.values[:] = np.where(
+                np.isnan(interp_array.values), nearest_array.values, interp_array.values
+            )
+
+        return interp_array
+
 
 class FieldGrid(Tidy3dBaseModel):
     """Holds the grid data for a single field.
 
     Example
     -------
     >>> x = np.linspace(-1, 1, 10)
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/grid/grid_spec.py` & `tidy3d-2.3.1/tidy3d/components/grid/grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/grid/mesher.py` & `tidy3d-2.3.1/tidy3d/components/grid/mesher.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 
             # Handle insertion of the current structure bounds in the intervals
             intervals = self.insert_bbox(intervals, str_ind, bbox, bbox_contained_2d, min_step)
 
         # Truncate intervals to domain bounds
         coords = np.array(intervals["coords"])
         num_ints = len(intervals["structs"])
-        in_domain = np.argwhere((coords >= domain_bounds[0]) * (coords <= domain_bounds[1]))
+        in_domain = np.nonzero((coords >= domain_bounds[0]) * (coords <= domain_bounds[1]))[0]
         intervals["coords"] = [intervals["coords"][int(i)] for i in in_domain]
         intervals["structs"] = [intervals["structs"][int(i)] for i in in_domain if i < num_ints]
 
         # Compute the maximum allowed step size in each interval
         max_steps = []
         for coord_ind, _ in enumerate(intervals["coords"][:-1]):
             # if there are any enforced structure in the interval, use the last structure
@@ -232,15 +232,15 @@
         """
 
         coords = intervals["coords"]
         structs = intervals["structs"]
 
         # Left structure bound
         bound_coord = str_bbox[0, 2]
-        indsmin = np.argwhere(bound_coord <= coords)
+        indsmin = np.nonzero(bound_coord <= coords)[0]
         indmin = int(indsmin[0])  # coordinate is in interval index ``indmin - 1````
         is_close_l = self.is_close(bound_coord, coords, indmin - 1, min_step)
         is_close_r = self.is_close(bound_coord, coords, indmin, min_step)
         is_contained = self.is_contained(bound_coord, bbox_contained_2d)
 
         # Decide on whether coordinate should be inserted or indmin modified
         if is_close_l:
@@ -251,15 +251,15 @@
             coords.insert(indmin, bound_coord)
             # Copy the structure containment list to the newly created interval
             struct_list = structs[max(0, indmin - 1)]
             structs.insert(indmin, struct_list.copy())
 
         # Right structure bound
         bound_coord = str_bbox[1, 2]
-        indsmax = np.argwhere(bound_coord >= coords)
+        indsmax = np.nonzero(bound_coord >= coords)[0]
         indmax = int(indsmax[-1])  # coordinate is in interval index ``indmax``
         is_close_l = self.is_close(bound_coord, coords, indmax, min_step)
         is_close_r = self.is_close(bound_coord, coords, indmax + 1, min_step)
         is_contained = self.is_contained(bound_coord, bbox_contained_2d)
 
         # Decide on whether coordinate should be inserted or indmax modified
         if is_close_r:
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/medium.py` & `tidy3d-2.3.1/tidy3d/components/medium.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import xarray as xr
 
 from .base import Tidy3dBaseModel, cached_property
 from .grid.grid import Coords, Grid
 from .types import PoleAndResidue, Ax, FreqBound, TYPE_TAG_STR, InterpMethod, Bound, ArrayComplex3D
 from .types import Axis, TensorReal
 from .data.dataset import PermittivityDataset
-from .data.data_array import SpatialDataArray, ScalarFieldDataArray
+from .data.data_array import SpatialDataArray, ScalarFieldDataArray, DATA_ARRAY_MAP
 from .viz import add_ax_if_none
 from .geometry import Geometry
 from .validators import validate_name_str
 from ..constants import C_0, pec_val, EPSILON_0, LARGE_NUMBER, fp_eps
 from ..constants import HERTZ, CONDUCTIVITY, PERMITTIVITY, RADPERSEC, MICROMETER, SECOND
 from ..exceptions import ValidationError, SetupError
 from ..log import log
@@ -78,14 +78,24 @@
     frequency_range: FreqBound = pd.Field(
         None,
         title="Frequency Range",
         description="Optional range of validity for the medium.",
         units=(HERTZ, HERTZ),
     )
 
+    allow_gain: bool = pd.Field(
+        False,
+        title="Allow gain medium",
+        description="Allow the medium to be active. Caution: "
+        "simulations with gain medium are unstable, and are likely to diverge."
+        "Simulations where 'allow_gain' is set to 'True' will still be charged even if "
+        "diverged. Monitor data up to the divergence point will still be returned and can be "
+        "useful in some cases.",
+    )
+
     _name_validator = validate_name_str()
 
     @abstractmethod
     def eps_model(self, frequency: float) -> complex:
         """Complex-valued permittivity as a function of frequency.
 
         Parameters
@@ -341,14 +351,23 @@
         description="Interpolation method to obtain permittivity values "
         "that are not supplied at the Yee grids; For grids outside the range "
         "of the supplied data, extrapolation will be applied. When the extrapolated "
         "value is smaller (greater) than the minimal (maximal) of the supplied data, "
         "the extrapolated value will take the minimal (maximal) of the supplied data.",
     )
 
+    subpixel: bool = pd.Field(
+        False,
+        title="Subpixel averaging",
+        description="If ``True`` and simulation's ``subpixel`` is also ``True``, "
+        "applies subpixel averaging of the permittivity "
+        "on the interface of the structure, including exterior boundary and "
+        "intersection interfaces with other structures.",
+    )
+
     @cached_property
     @abstractmethod
     def is_isotropic(self) -> bool:
         """The medium is isotropic or anisotropic."""
 
     def _interp_method(self, comp: Axis) -> InterpMethod:  # pylint:disable=unused-argument
         """Interpolation method applied to comp."""
@@ -390,18 +409,18 @@
         -------
         Tuple[ArrayComplex3D, ArrayComplex3D, ArrayComplex3D]
             The complex-valued permittivity tensor at ``frequency`` interpolated
             at the supplied coordinate.
         """
         eps_spatial = self.eps_dataarray_freq(frequency)
         if self.is_isotropic:
-            eps_interp = self._interp(eps_spatial[0], coords, self._interp_method(0)).values
+            eps_interp = coords.spatial_interp(eps_spatial[0], self._interp_method(0)).values
             return (eps_interp, eps_interp, eps_interp)
         return tuple(
-            self._interp(eps_comp, coords, self._interp_method(comp)).values
+            coords.spatial_interp(eps_comp, self._interp_method(comp)).values
             for comp, eps_comp in enumerate(eps_spatial)
         )
 
     def eps_comp_on_grid(
         self,
         row: Axis,
         col: Axis,
@@ -462,98 +481,28 @@
         return np.all(np.isreal(dataarray.values))
 
     @staticmethod
     def _validate_isreal_dataarray_tuple(dataarray_tuple: Tuple[SpatialDataArray, ...]) -> bool:
         """Validate that the dataarray is real"""
         return np.all([AbstractCustomMedium._validate_isreal_dataarray(f) for f in dataarray_tuple])
 
-    @staticmethod
-    def _interp(
-        spatial_dataarray: Union[SpatialDataArray, ScalarFieldDataArray],
-        coord_interp: Coords,
-        interp_method: InterpMethod,
-    ) -> Union[SpatialDataArray, ScalarFieldDataArray]:
-        """
-        Enhance xarray's ``.interp`` in two ways:
-            1) Check if the coordinate of the supplied data are in monotically increasing order.
-            If they are, apply the faster ``assume_sorted=True``.
-
-            2) For axes of single entry, instead of error, apply ``isel()`` along the axis.
-
-            3) When linear interp is applied, in the extrapolated region, filter values smaller
-            or larger than the original data's min(max) will be replaced with the original min(max).
-
-        Parameters
-        ----------
-        spatial_dataarray: Union[:class:`.SpatialDataArray`, :class:`.ScalarFieldDataArray`]
-            Supplied scalar dataset
-        coord_interp : :class:`.Coords`
-            The grid point coordinates over which interpolation is performed.
-        interp_method : :class:`.InterpMethod`
-            Interpolation method.
-
-        Returns
-        -------
-        Union[:class:`.SpatialDataArray`, :class:`.ScalarFieldDataArray`]
-            The interpolated spatial dataset.
-        """
-
-        all_coords = "xyz"
-        is_single_entry = [spatial_dataarray.sizes[ax] == 1 for ax in all_coords]
-        interp_ax = [
-            ax for (ax, single_entry) in zip(all_coords, is_single_entry) if not single_entry
-        ]
-        isel_ax = [ax for ax in all_coords if ax not in interp_ax]
-
-        # apply isel for the axis containing single entry
-        if len(isel_ax) > 0:
-            spatial_dataarray = spatial_dataarray.isel(
-                {ax: [0] * len(coord_interp.to_dict[ax]) for ax in isel_ax}
-            )
-            spatial_dataarray = spatial_dataarray.assign_coords(
-                {ax: coord_interp.to_dict[ax] for ax in isel_ax}
-            )
-            if len(interp_ax) == 0:
-                return spatial_dataarray
-
-        # Apply interp for the rest
-        #   first check if it's sorted
-        is_sorted = all((np.all(np.diff(spatial_dataarray.coords[f]) > 0) for f in interp_ax))
-        interp_param = dict(
-            kwargs={"fill_value": FILL_VALUE},
-            assume_sorted=is_sorted,
-            method=interp_method,
-        )
-        #   interpolation
-        interp_dataarray = spatial_dataarray.interp(
-            {ax: coord_interp.to_dict[ax] for ax in interp_ax},
-            **interp_param,
-        )
-
-        # filter any values larger/smaller than the original data's max/min.
-        max_val = max(spatial_dataarray.values.ravel())
-        min_val = min(spatial_dataarray.values.ravel())
-        interp_dataarray = interp_dataarray.where(interp_dataarray >= min_val, min_val)
-        interp_dataarray = interp_dataarray.where(interp_dataarray <= max_val, max_val)
-        return interp_dataarray
-
 
 """ Dispersionless Medium """
 
+
 # PEC keyword
 class PECMedium(AbstractMedium):
     """Perfect electrical conductor class.
 
     Note
     ----
     To avoid confusion from duplicate PECs, must import ``tidy3d.PEC`` instance directly.
     """
 
     def eps_model(self, frequency: float) -> complex:
-
         # return something like frequency with value of pec_val + 0j
         return 0j * frequency + pec_val
 
     @cached_property
     def n_cfl(self):
         """This property computes the index of refraction related to CFL condition, so that
         the FDTD with this medium is stable when the time step size that doesn't take
@@ -577,21 +526,31 @@
 
     permittivity: float = pd.Field(
         1.0, ge=1.0, title="Permittivity", description="Relative permittivity.", units=PERMITTIVITY
     )
 
     conductivity: float = pd.Field(
         0.0,
-        ge=0.0,
         title="Conductivity",
         description="Electric conductivity. Defined such that the imaginary part of the complex "
         "permittivity at angular frequency omega is given by conductivity/omega.",
         units=CONDUCTIVITY,
     )
 
+    @pd.validator("conductivity", always=True)
+    def _passivity_validation(cls, val, values):
+        """Assert passive medium if `allow_gain` is False."""
+        if not values.get("allow_gain") and val < 0:
+            raise ValidationError(
+                "For passive medium, 'conductivity' must be non-negative. "
+                "To simulate gain medium, please set 'allow_gain=True'. "
+                "Caution: simulations with gain medium are unstable, and are likely to diverge."
+            )
+        return val
+
     @cached_property
     def n_cfl(self):
         """This property computes the index of refraction related to CFL condition, so that
         the FDTD with this medium is stable when the time step size that doesn't take
         material factor into account is multiplied by ``n_cfl``.
 
         For dispersiveless medium, it equals ``sqrt(permittivity)``.
@@ -669,33 +628,43 @@
 
         if np.any(val.values < 1):
             raise SetupError("'permittivity' must be no less than one.")
 
         return val
 
     @pd.validator("conductivity", always=True)
-    def _conductivity_non_negative_correct_shape(cls, val, values):
-        """Assert conductivity>=0"""
+    def _conductivity_real_and_correct_shape(cls, val, values):
+        """Assert conductivity is real and of right shape."""
 
         if val is None:
             return val
 
         if values.get("permittivity") is None:
             raise ValidationError("'permittivity' failed validation.")
 
         if not CustomIsotropicMedium._validate_isreal_dataarray(val):
             raise SetupError("'conductivity' must be real.")
 
-        if np.any(val.values < 0):
-            raise SetupError("'conductivity' must be non-negative.")
-
         if values["permittivity"].coords != val.coords:
             raise SetupError("'permittivity' and 'conductivity' must have the same coordinates.")
         return val
 
+    @pd.validator("conductivity", always=True)
+    def _passivity_validation(cls, val, values):
+        """Assert passive medium if `allow_gain` is False."""
+        if val is None:
+            return val
+        if not values.get("allow_gain") and np.any(val.values < 0):
+            raise ValidationError(
+                "For passive medium, 'conductivity' must be non-negative. "
+                "To simulate gain medium, please set 'allow_gain=True'. "
+                "Caution: simulations with gain medium are unstable, and are likely to diverge."
+            )
+        return val
+
     @cached_property
     def n_cfl(self):
         """This property computes the index of refraction related to CFL condition, so that
         the FDTD with this medium is stable when the time step size that doesn't take
         material factor into account is multiplied by ``n_cfl``.
 
         For dispersiveless medium, it equals ``sqrt(permittivity)``.
@@ -766,14 +735,42 @@
         title="Permittivity Dataset",
         description="[To be deprecated] User-supplied dataset containing complex-valued "
         "permittivity as a function of space. Permittivity distribution over the Yee-grid "
         "will be interpolated based on ``interp_method``.",
     )
 
     @pd.root_validator(pre=True)
+    def _warn_if_none(cls, values):
+        """Warn if the data array fails to load, and return a vacuum medium."""
+        eps_dataset = values.get("eps_dataset")
+        permittivity = values.get("permittivity")
+        conductivity = values.get("conductivity")
+        fail_load = False
+        if isinstance(permittivity, str) and permittivity in DATA_ARRAY_MAP.keys():
+            log.warning(
+                "Loading 'permittivity' without data; constructing a vacuum medium instead."
+            )
+            fail_load = True
+        if isinstance(conductivity, str) and conductivity in DATA_ARRAY_MAP.keys():
+            log.warning(
+                "Loading 'conductivity' without data; constructing a vacuum medium instead."
+            )
+            fail_load = True
+        if isinstance(eps_dataset, dict):
+            if any((v in DATA_ARRAY_MAP for _, v in eps_dataset.items() if isinstance(v, str))):
+                log.warning(
+                    "Loading 'eps_dataset' without data; constructing a vacuum medium instead."
+                )
+                fail_load = True
+        if fail_load:
+            eps_real = SpatialDataArray(np.ones((1, 1, 1)), coords=dict(x=[0], y=[0], z=[0]))
+            return dict(permittivity=eps_real)
+        return values
+
+    @pd.root_validator(pre=True)
     def _deprecation_dataset(cls, values):
         """Raise deprecation warning if dataset supplied and convert to dataset."""
 
         eps_dataset = values.get("eps_dataset")
         permittivity = values.get("permittivity")
         conductivity = values.get("conductivity")
 
@@ -830,32 +827,34 @@
                 raise SetupError(
                     f"'eps_dataset.{name}' must have a single frequency, "
                     f"but it contains {len(freqs)} frequencies."
                 )
         return val
 
     @pd.validator("eps_dataset", always=True)
-    def _eps_dataset_eps_inf_greater_no_less_than_one_sigma_positive(cls, val):
+    def _eps_dataset_eps_inf_greater_no_less_than_one_sigma_positive(cls, val, values):
         """Assert any eps_inf must be >=1"""
         if val is None:
             return val
 
         for comp in ["eps_xx", "eps_yy", "eps_zz"]:
             eps_real, sigma = CustomMedium.eps_complex_to_eps_sigma(
                 val.field_components[comp], val.field_components[comp].f
             )
             if np.any(eps_real.values < 1):
                 raise SetupError(
                     "Permittivity at infinite frequency at any spatial point "
                     "must be no less than one."
                 )
-            if np.any(sigma.values < 0):
-                raise SetupError(
-                    "Negative imaginary part of refrative index leads to a gain medium, "
-                    "which is not supported."
+            if not values.get("allow_gain") and np.any(sigma.values < 0):
+                raise ValidationError(
+                    "For passive medium, imaginary part of permittivity must be non-negative. "
+                    "To simulate gain medium, please set 'allow_gain=True'. "
+                    "Caution: simulations with gain medium are unstable, "
+                    "and are likely to diverge."
                 )
         return val
 
     @pd.validator("permittivity", always=True)
     def _eps_inf_greater_no_less_than_one(cls, val):
         """Assert any eps_inf must be >=1"""
         if val is None:
@@ -878,16 +877,21 @@
 
         if values.get("permittivity") is None:
             raise ValidationError("'permittivity' failed validation.")
 
         if not CustomMedium._validate_isreal_dataarray(val):
             raise SetupError("'conductivity' must be real.")
 
-        if np.any(val.values < 0):
-            raise SetupError("'conductivity' must be non-negative.")
+        if not values.get("allow_gain") and np.any(val.values < 0):
+            raise ValidationError(
+                "For passive medium, 'conductivity' must be non-negative. "
+                "To simulate gain medium, please set 'allow_gain=True'. "
+                "Caution: simulations with gain medium are unstable, "
+                "and are likely to diverge."
+            )
 
         if values["permittivity"].coords != val.coords:
             raise SetupError("'permittivity' and 'conductivity' must have the same coordinates.")
         return val
 
     @cached_property
     def is_isotropic(self) -> bool:
@@ -915,52 +919,45 @@
         )
 
     @cached_property
     def _medium(self):
         """Internal representation in the form of
         either `CustomIsotropicMedium` or `CustomAnisotropicMedium`.
         """
+        self_dict = self.dict(exclude={"type", "eps_dataset"})
         # isotropic
         if self.eps_dataset is None:
-            return CustomIsotropicMedium(
-                permittivity=self.permittivity,
-                conductivity=self.conductivity,
-                interp_method=self.interp_method,
-            )
+            self_dict.update({"permittivity": self.permittivity, "conductivity": self.conductivity})
+            return CustomIsotropicMedium.parse_obj(self_dict)
+
         # isotropic, but with `eps_dataset`
         if self.is_isotropic:
             eps_real, sigma = CustomMedium.eps_complex_to_eps_sigma(
                 np.array(self.eps_dataset.eps_xx.values), self.freqs[0]
             )
             coords = self.eps_dataset.eps_xx.coords
             eps_real = ScalarFieldDataArray(eps_real, coords=coords)
             sigma = ScalarFieldDataArray(sigma, coords=coords)
             eps_real = SpatialDataArray(eps_real.squeeze(dim="f", drop=True))
             sigma = SpatialDataArray(sigma.squeeze(dim="f", drop=True))
-            return CustomIsotropicMedium(
-                permittivity=eps_real,
-                conductivity=sigma,
-                interp_method=self.interp_method,
-            )
+            self_dict.update({"permittivity": eps_real, "conductivity": sigma})
+            return CustomIsotropicMedium.parse_obj(self_dict)
+
         # anisotropic
         eps_field_components = self.eps_dataset.field_components
         mat_comp = {"interp_method": self.interp_method}
         for comp in ["xx", "yy", "zz"]:
             eps_real, sigma = CustomMedium.eps_complex_to_eps_sigma(
                 eps_field_components["eps_" + comp], eps_field_components["eps_" + comp].coords["f"]
             )
             eps_real = SpatialDataArray(eps_real.squeeze(dim="f", drop=True))
             sigma = SpatialDataArray(sigma.squeeze(dim="f", drop=True))
-            mat_comp.update(
-                {
-                    comp: CustomIsotropicMedium(
-                        permittivity=eps_real, conductivity=sigma, interp_method=self.interp_method
-                    )
-                }
-            )
+            comp_dict = self_dict.copy()
+            comp_dict.update({"permittivity": eps_real, "conductivity": sigma})
+            mat_comp.update({comp: CustomIsotropicMedium.parse_obj(comp_dict)})
         return CustomAnisotropicMediumInternal(**mat_comp)
 
     def _interp_method(self, comp: Axis) -> InterpMethod:
         """Interpolation method applied to comp."""
         return self._medium._interp_method(comp)  # pylint:disable=protected-access
 
     @cached_property
@@ -1031,14 +1028,15 @@
 
     @classmethod
     def from_eps_raw(
         cls,
         eps: Union[ScalarFieldDataArray, SpatialDataArray],
         freq: float = None,
         interp_method: InterpMethod = "nearest",
+        **kwargs,
     ) -> CustomMedium:
         """Construct a :class:`.CustomMedium` from datasets containing raw permittivity values.
 
         Parameters
         ----------
         eps : Union[:class:`.SpatialDataArray`, :class:`.ScalarFieldDataArray`]
             Dataset containing complex-valued permittivity as a function of space.
@@ -1061,45 +1059,48 @@
         -------
         :class:`.CustomMedium`
             Medium containing the spatially varying permittivity data.
         """
         if isinstance(eps, SpatialDataArray):
             # purely real, not need to know `freq`
             if CustomMedium._validate_isreal_dataarray(eps):
-                return cls(permittivity=eps, interp_method=interp_method)
+                return cls(permittivity=eps, interp_method=interp_method, **kwargs)
             # complex permittivity, needs to know `freq`
             if freq is None:
                 raise SetupError(
                     "For a complex 'eps', 'freq' at which 'eps' is defined must be supplied",
                 )
             eps_real, sigma = CustomMedium.eps_complex_to_eps_sigma(eps, freq)
-            return cls(permittivity=eps_real, conductivity=sigma, interp_method=interp_method)
+            return cls(
+                permittivity=eps_real, conductivity=sigma, interp_method=interp_method, **kwargs
+            )
 
         # eps is ScalarFieldDataArray
         # contradictory definition of frequency
         freq_data = eps.coords["f"].data[0]
         if freq is not None and not isclose(freq, freq_data):
             raise SetupError(
                 "'freq' value is inconsistent with the coordinate 'f'"
                 "in 'eps' DataArray. It's unclear at which frequency 'eps' "
                 "is defined. Please leave 'freq=None' to use the frequency "
                 "value in the DataArray."
             )
         eps_real, sigma = CustomMedium.eps_complex_to_eps_sigma(eps, freq_data)
         eps_real = SpatialDataArray(eps_real.squeeze(dim="f", drop=True))
         sigma = SpatialDataArray(sigma.squeeze(dim="f", drop=True))
-        return cls(permittivity=eps_real, conductivity=sigma, interp_method=interp_method)
+        return cls(permittivity=eps_real, conductivity=sigma, interp_method=interp_method, **kwargs)
 
     @classmethod
     def from_nk(
         cls,
         n: Union[ScalarFieldDataArray, SpatialDataArray],
         k: Optional[Union[ScalarFieldDataArray, SpatialDataArray]] = None,
         freq: float = None,
         interp_method: InterpMethod = "nearest",
+        **kwargs,
     ) -> CustomMedium:
         """Construct a :class:`.CustomMedium` from datasets containing n and k values.
 
         Parameters
         ----------
         n : Union[:class:`.SpatialDataArray`, :class:`.ScalarFieldDataArray`]
             Real part of refractive index.
@@ -1127,15 +1128,15 @@
         """
         # lossless
         if k is None:
             if isinstance(n, ScalarFieldDataArray):
                 n = SpatialDataArray(n.squeeze(dim="f", drop=True))
             freq = 0  # dummy value
             eps_real, _ = CustomMedium.nk_to_eps_sigma(n, 0 * n, freq)
-            return cls(permittivity=eps_real, interp_method=interp_method)
+            return cls(permittivity=eps_real, interp_method=interp_method, **kwargs)
 
         # lossy case
         if n.coords.keys() != k.coords.keys():
             raise SetupError("'n' and 'k' must be of the same type.")
         if n.coords != k.coords:
             raise SetupError("'n' and 'k' must have same coordinates.")
 
@@ -1143,30 +1144,32 @@
         if isinstance(k, SpatialDataArray):
             if freq is None:
                 raise SetupError(
                     "For a lossy medium, must supply 'freq' at which to convert 'n' "
                     "and 'k' to a complex valued permittivity."
                 )
             eps_real, sigma = CustomMedium.nk_to_eps_sigma(n, k, freq)
-            return cls(permittivity=eps_real, conductivity=sigma, interp_method=interp_method)
+            return cls(
+                permittivity=eps_real, conductivity=sigma, interp_method=interp_method, **kwargs
+            )
 
         # k is a ScalarFieldDataArray
         freq_data = k.coords["f"].data[0]
         if freq is not None and not isclose(freq, freq_data):
             raise SetupError(
                 "'freq' value is inconsistent with the coordinate 'f'"
                 "in 'k' DataArray. It's unclear at which frequency 'k' "
                 "is defined. Please leave 'freq=None' to use the frequency "
                 "value in the DataArray."
             )
 
         eps_real, sigma = CustomMedium.nk_to_eps_sigma(n, k, freq_data)
         eps_real = SpatialDataArray(eps_real.squeeze(dim="f", drop=True))
         sigma = SpatialDataArray(sigma.squeeze(dim="f", drop=True))
-        return cls(permittivity=eps_real, conductivity=sigma, interp_method=interp_method)
+        return cls(permittivity=eps_real, conductivity=sigma, interp_method=interp_method, **kwargs)
 
     def grids(self, bounds: Bound) -> Dict[str, Grid]:
         """Make a :class:`.Grid` corresponding to the data in each ``eps_ii`` component.
         The min and max coordinates along each dimension are bounded by ``bounds``."""
 
         rmin, rmax = bounds
         pt_mins = dict(zip("xyz", rmin))
@@ -1201,15 +1204,14 @@
 
             # construct grid
             boundaries = Coords(**bound_coords)
             return Grid(boundaries=boundaries)
 
         grids = {}
         for field_name in ("eps_xx", "eps_yy", "eps_zz"):
-
             # grab user supplied data long this dimension
             scalar_field = self.eps_dataset.field_components[field_name]
 
             # feed it to make_grid
             grids[field_name] = make_grid(scalar_field)
 
         return grids
@@ -1224,15 +1226,15 @@
     @abstractmethod
     def _pole_residue_dict(self) -> Dict:
         """Dict representation of Medium as a pole-residue model."""
 
     @cached_property
     def pole_residue(self):
         """Representation of Medium as a pole-residue model."""
-        return PoleResidue(**self._pole_residue_dict())
+        return PoleResidue(**self._pole_residue_dict(), allow_gain=self.allow_gain)
 
     @cached_property
     def n_cfl(self):
         """This property computes the index of refraction related to CFL condition, so that
         the FDTD with this medium is stable when the time step size that doesn't take
         material factor into account is multiplied by ``n_cfl``.
 
@@ -1273,15 +1275,57 @@
     def is_isotropic(self):
         """Whether the medium is isotropic."""
         return True
 
     @cached_property
     def pole_residue(self):
         """Representation of Medium as a pole-residue model."""
-        return CustomPoleResidue(**self._pole_residue_dict(), interp_method=self.interp_method)
+        return CustomPoleResidue(
+            **self._pole_residue_dict(),
+            interp_method=self.interp_method,
+            allow_gain=self.allow_gain,
+            subpixel=self.subpixel,
+        )
+
+    @staticmethod
+    def _warn_if_data_none(nested_tuple_field: str):
+        """Warn if any of `eps_inf` and nested_tuple_field are not loaded,
+        and return a vacuum with eps_inf = 1.
+        """
+
+        @pd.root_validator(pre=True, allow_reuse=True)
+        def _warn_if_none(cls, values):  # pylint:disable=unused-argument
+            """Warn if any of `eps_inf` and nested_tuple_field are not load."""
+            eps_inf = values.get("eps_inf")
+            coeffs = values.get(nested_tuple_field)
+            fail_load = False
+
+            if isinstance(eps_inf, str) and eps_inf in DATA_ARRAY_MAP.keys():
+                log.warning("Loading 'eps_inf' without data; constructing a vacuum medium instead.")
+                fail_load = True
+            for coeff in coeffs:
+                if fail_load:
+                    break
+                for coeff_i in coeff:
+                    if isinstance(coeff_i, str) and coeff_i in DATA_ARRAY_MAP.keys():
+                        log.warning(
+                            "Loading '{nested_tuple_field}' without data; "
+                            "constructing a vacuum medium instead."
+                        )
+                        fail_load = True
+                        break
+
+            if fail_load and eps_inf is None:
+                return {nested_tuple_field: ()}
+            if fail_load:
+                eps_inf = SpatialDataArray(np.ones((1, 1, 1)), coords=dict(x=[0], y=[0], z=[0]))
+                return {"eps_inf": eps_inf, nested_tuple_field: ()}
+            return values
+
+        return _warn_if_none
 
 
 class PoleResidue(DispersiveMedium):
     """A dispersive medium described by the pole-residue pair model.
     The frequency-dependence of the complex-valued permittivity is described by:
 
     Note
@@ -1290,15 +1334,15 @@
 
         \\epsilon(\\omega) = \\epsilon_\\infty - \\sum_i
         \\left[\\frac{c_i}{j \\omega + a_i} +
         \\frac{c_i^*}{j \\omega + a_i^*}\\right]
 
     Example
     -------
-    >>> pole_res = PoleResidue(eps_inf=2.0, poles=[((1+2j), (3+4j)), ((5+6j), (7+8j))])
+    >>> pole_res = PoleResidue(eps_inf=2.0, poles=[((-1+2j), (3+4j)), ((-5+6j), (7+8j))])
     >>> eps = pole_res.eps_model(200e12)
     """
 
     eps_inf: pd.PositiveFloat = pd.Field(
         1.0,
         title="Epsilon at Infinity",
         description="Relative permittivity at infinite frequency (:math:`\\epsilon_\\infty`).",
@@ -1308,21 +1352,29 @@
     poles: Tuple[PoleAndResidue, ...] = pd.Field(
         (),
         title="Poles",
         description="Tuple of complex-valued (:math:`a_i, c_i`) poles for the model.",
         units=(RADPERSEC, RADPERSEC),
     )
 
+    @pd.validator("poles", always=True)
+    def _causality_validation(cls, val):
+        """Assert causal medium."""
+        for a, _ in val:
+            if np.any(np.real(a) > 0):
+                raise SetupError("For stable medium, 'Re(a_i)' must be non-positive.")
+        return val
+
     @ensure_freq_in_range
     def eps_model(self, frequency: float) -> complex:
         """Complex-valued permittivity as a function of frequency."""
 
         omega = 2 * np.pi * frequency
         eps = self.eps_inf + np.zeros_like(frequency) + 0.0j
-        for (a, c) in self.poles:
+        for a, c in self.poles:
             a_cc = np.conj(a)
             c_cc = np.conj(c)
             eps -= c / (1j * omega + a)
             eps -= c_cc / (1j * omega + a_cc)
         return eps
 
     def _pole_residue_dict(self) -> Dict:
@@ -1370,15 +1422,15 @@
 
         Returns
         -------
         :class:`.Medium`
             The non-dispersive equivalent with constant permittivity and conductivity.
         """
         res = 0
-        for (a, c) in self.poles:
+        for a, c in self.poles:
             if abs(a) > fp_eps:
                 raise ValidationError("Cannot convert dispersive 'PoleResidue' to 'Medium'.")
             res += (c + np.conj(c)) / 2
         sigma = res * 2 * EPSILON_0
         return Medium(
             permittivity=self.eps_inf,
             conductivity=np.real(sigma),
@@ -1401,17 +1453,17 @@
     Example
     -------
     >>> x = np.linspace(-1, 1, 5)
     >>> y = np.linspace(-1, 1, 6)
     >>> z = np.linspace(-1, 1, 7)
     >>> coords = dict(x=x, y=y, z=z)
     >>> eps_inf = SpatialDataArray(np.ones((5, 6, 7)), coords=coords)
-    >>> a1 = SpatialDataArray(np.random.random((5, 6, 7)), coords=coords)
+    >>> a1 = SpatialDataArray(-np.random.random((5, 6, 7)), coords=coords)
     >>> c1 = SpatialDataArray(np.random.random((5, 6, 7)), coords=coords)
-    >>> a2 = SpatialDataArray(np.random.random((5, 6, 7)), coords=coords)
+    >>> a2 = SpatialDataArray(-np.random.random((5, 6, 7)), coords=coords)
     >>> c2 = SpatialDataArray(np.random.random((5, 6, 7)), coords=coords)
     >>> pole_res = CustomPoleResidue(eps_inf=eps_inf, poles=[(a1, c1), (a2, c2)])
     >>> eps = pole_res.eps_model(200e12)
     """
 
     eps_inf: SpatialDataArray = pd.Field(
         ...,
@@ -1423,14 +1475,16 @@
     poles: Tuple[Tuple[SpatialDataArray, SpatialDataArray], ...] = pd.Field(
         (),
         title="Poles",
         description="Tuple of complex-valued (:math:`a_i, c_i`) poles for the model.",
         units=(RADPERSEC, RADPERSEC),
     )
 
+    _warn_if_none = CustomDispersiveMedium._warn_if_data_none("poles")
+
     @pd.validator("eps_inf", always=True)
     def _eps_inf_positive(cls, val):
         """eps_inf must be positive"""
         if not CustomDispersiveMedium._validate_isreal_dataarray(val):
             raise SetupError("'eps_inf' must be real.")
         if np.any(val < 0):
             raise SetupError("'eps_inf' must be positive.")
@@ -1481,15 +1535,15 @@
         Returns
         -------
         Tuple[Tuple[ArrayComplex3D, ArrayComplex3D], ...]
             The poles interpolated at the supplied coordinate.
         """
 
         def fun_interp(input_data: SpatialDataArray) -> ArrayComplex3D:
-            return self._interp(input_data, coords, self.interp_method).values
+            return coords.spatial_interp(input_data, self.interp_method).values
 
         return tuple((fun_interp(a), fun_interp(c)) for (a, c) in self.poles)
 
     @classmethod
     def from_medium(cls, medium: CustomMedium) -> "CustomPoleResidue":
         """Convert a :class:`.CustomMedium` to a pole residue model.
 
@@ -1499,40 +1553,41 @@
             The medium with permittivity and conductivity to convert.
 
         Returns
         -------
         :class:`.CustomPoleResidue`
             The pole residue equivalent.
         """
-        poles = [(0, medium.conductivity / (2 * EPSILON_0))]
-        return CustomPoleResidue(
-            eps_inf=medium.permittivity, poles=poles, frequency_range=medium.frequency_range
-        )
+        poles = [(xr.zeros_like(medium.conductivity), medium.conductivity / (2 * EPSILON_0))]
+        medium_dict = medium.dict(exclude={"type", "eps_dataset", "permittivity", "conductivity"})
+        medium_dict.update({"eps_inf": medium.permittivity, "poles": poles})
+        return CustomPoleResidue.parse_obj(medium_dict)
 
     def to_medium(self) -> CustomMedium:
         """Convert to a :class:`.CustomMedium`.
         Requires the pole residue model to only have a pole at 0 frequency,
         corresponding to a constant conductivity term.
 
         Returns
         -------
         :class:`.CustomMedium`
             The non-dispersive equivalent with constant permittivity and conductivity.
         """
         res = 0
-        for (a, c) in self.poles:
-            if abs(a) > fp_eps:
-                raise ValidationError("Cannot convert dispersive 'PoleResidue' to 'Medium'.")
+        for a, c in self.poles:
+            if np.any(abs(a.values) > fp_eps):
+                raise ValidationError(
+                    "Cannot convert dispersive 'CustomPoleResidue' to 'CustomMedium'."
+                )
             res += (c + np.conj(c)) / 2
         sigma = res * 2 * EPSILON_0
-        return CustomMedium(
-            permittivity=self.eps_inf,
-            conductivity=np.real(sigma),
-            frequency_range=self.frequency_range,
-        )
+
+        self_dict = self.dict(exclude={"type", "eps_inf", "poles"})
+        self_dict.update({"permittivity": self.eps_inf, "conductivity": np.real(sigma)})
+        return CustomMedium.parse_obj(self_dict)
 
 
 class Sellmeier(DispersiveMedium):
     """A dispersive medium described by the Sellmeier model.
     The frequency-dependence of the refractive index is described by:
 
     Note
@@ -1549,35 +1604,50 @@
 
     coeffs: Tuple[Tuple[float, pd.PositiveFloat], ...] = pd.Field(
         title="Coefficients",
         description="List of Sellmeier (:math:`B_i, C_i`) coefficients.",
         units=(None, MICROMETER + "^2"),
     )
 
+    @pd.validator("coeffs", always=True)
+    def _passivity_validation(cls, val, values):
+        """Assert passive medium if `allow_gain` is False."""
+        if values.get("allow_gain"):
+            return val
+        for B, _ in val:
+            if B < 0:
+                raise ValidationError(
+                    "For passive medium, 'B_i' must be non-negative. "
+                    "To simulate gain medium, please set 'allow_gain=True'. "
+                    "Caution: simulations with gain medium are unstable, "
+                    "and are likely to diverge."
+                )
+        return val
+
     def _n_model(self, frequency: float) -> complex:
         """Complex-valued refractive index as a function of frequency."""
 
         wvl = C_0 / np.array(frequency)
         wvl2 = wvl**2
         n_squared = 1.0
-        for (B, C) in self.coeffs:
+        for B, C in self.coeffs:
             n_squared += B * wvl2 / (wvl2 - C)
         return np.sqrt(n_squared)
 
     @ensure_freq_in_range
     def eps_model(self, frequency: float) -> complex:
         """Complex-valued permittivity as a function of frequency."""
 
         n = self._n_model(frequency)
         return AbstractMedium.nk_to_eps_complex(n)
 
     def _pole_residue_dict(self) -> Dict:
         """Dict representation of Medium as a pole-residue model"""
         poles = []
-        for (B, C) in self.coeffs:
+        for B, C in self.coeffs:
             beta = 2 * np.pi * C_0 / np.sqrt(C)
             alpha = -0.5 * beta * B
             a = 1j * beta
             c = 1j * alpha
             poles.append((a, c))
         return dict(eps_inf=1, poles=poles, frequency_range=self.frequency_range, name=self.name)
 
@@ -1637,36 +1707,57 @@
     >>> b1 = SpatialDataArray(np.random.random((5, 6, 7)), coords=coords)
     >>> c1 = SpatialDataArray(np.random.random((5, 6, 7)), coords=coords)
     >>> sellmeier_medium = CustomSellmeier(coeffs=[(b1,c1),])
     >>> eps = sellmeier_medium.eps_model(200e12)
     """
 
     coeffs: Tuple[Tuple[SpatialDataArray, SpatialDataArray], ...] = pd.Field(
+        ...,
         title="Coefficients",
         description="List of Sellmeier (:math:`B_i, C_i`) coefficients.",
         units=(None, MICROMETER + "^2"),
     )
 
+    _warn_if_none = CustomDispersiveMedium._warn_if_data_none("coeffs")
+
     @pd.validator("coeffs", always=True)
     def _correct_shape_and_sign(cls, val):
         """every term in coeffs must have the same shape, and B>=0 and C>0."""
+        if len(val) == 0:
+            return val
         expected_coords = val[0][0].coords
-        for (B, C) in val:
+        for B, C in val:
             if B.coords != expected_coords or C.coords != expected_coords:
                 raise SetupError("Every term in 'coeffs' must have the same coordinates.")
             if not CustomDispersiveMedium._validate_isreal_dataarray_tuple((B, C)):
                 raise SetupError("'B' and 'C' must be real.")
             if np.any(C <= 0):
                 raise SetupError("'C' must be positive.")
         return val
 
+    @pd.validator("coeffs", always=True)
+    def _passivity_validation(cls, val, values):
+        """Assert passive medium if `allow_gain` is False."""
+        if values.get("allow_gain"):
+            return val
+        for B, _ in val:
+            if np.any(B < 0):
+                raise ValidationError(
+                    "For passive medium, 'B_i' must be non-negative. "
+                    "To simulate gain medium, please set 'allow_gain=True'. "
+                    "Caution: simulations with gain medium are unstable, "
+                    "and are likely to diverge."
+                )
+        return val
+
     def _pole_residue_dict(self) -> Dict:
         """Dict representation of Medium as a pole-residue model."""
         poles_dict = Sellmeier._pole_residue_dict(self)
-        poles_dict.update({"eps_inf": xr.ones_like(self.coeffs[0][0])})
+        if len(self.coeffs) > 0:
+            poles_dict.update({"eps_inf": xr.ones_like(self.coeffs[0][0])})
         return poles_dict
 
     def eps_dataarray_freq(
         self, frequency: float
     ) -> Tuple[SpatialDataArray, SpatialDataArray, SpatialDataArray]:
         """Permittivity array at ``frequency``.
 
@@ -1677,14 +1768,18 @@
 
         Returns
         -------
         Tuple[:class:`.SpatialDataArray`, :class:`.SpatialDataArray`, :class:`.SpatialDataArray`]
             The permittivity evaluated at ``frequency``.
         """
         eps = Sellmeier.eps_model(self, frequency)
+        # if `eps` is simply a float, convert it to a SpatialDataArray ; this is possible when
+        # `coeffs` is empty.
+        if isinstance(eps, (int, float, complex)):
+            eps = SpatialDataArray(eps * np.ones((1, 1, 1)), coords=dict(x=[0], y=[0], z=[0]))
         return (eps, eps, eps)
 
     @classmethod
     def from_dispersion(
         cls,
         n: SpatialDataArray,
         freq: float,
@@ -1747,48 +1842,62 @@
     eps_inf: pd.PositiveFloat = pd.Field(
         1.0,
         title="Epsilon at Infinity",
         description="Relative permittivity at infinite frequency (:math:`\\epsilon_\\infty`).",
         units=PERMITTIVITY,
     )
 
-    coeffs: Tuple[Tuple[float, float, float], ...] = pd.Field(
+    coeffs: Tuple[Tuple[float, float, pd.NonNegativeFloat], ...] = pd.Field(
         ...,
         title="Coefficients",
         description="List of (:math:`\\Delta\\epsilon_i, f_i, \\delta_i`) values for model.",
         units=(PERMITTIVITY, HERTZ, HERTZ),
     )
 
     @pd.validator("coeffs", always=True)
     def _coeffs_unequal_f_delta(cls, val):
-        """f and delta cannot be exactly the same."""
-        for (_, f, delta) in val:
-            if f == delta:
+        """f**2 and delta**2 cannot be exactly the same."""
+        for _, f, delta in val:
+            if f**2 == delta**2:
                 raise SetupError("'f' and 'delta' cannot take equal values.")
         return val
 
+    @pd.validator("coeffs", always=True)
+    def _passivity_validation(cls, val, values):
+        """Assert passive medium if `allow_gain` is False."""
+        if values.get("allow_gain"):
+            return val
+        for del_ep, _, _ in val:
+            if del_ep < 0:
+                raise ValidationError(
+                    "For passive medium, 'Delta epsilon_i' must be non-negative. "
+                    "To simulate gain medium, please set 'allow_gain=True'. "
+                    "Caution: simulations with gain medium are unstable, "
+                    "and are likely to diverge."
+                )
+        return val
+
     @ensure_freq_in_range
     def eps_model(self, frequency: float) -> complex:
         """Complex-valued permittivity as a function of frequency."""
 
         eps = self.eps_inf + 0.0j
-        for (de, f, delta) in self.coeffs:
+        for de, f, delta in self.coeffs:
             eps += (de * f**2) / (f**2 - 2j * frequency * delta - frequency**2)
         return eps
 
     def _pole_residue_dict(self) -> Dict:
         """Dict representation of Medium as a pole-residue model."""
 
         poles = []
-        for (de, f, delta) in self.coeffs:
-
+        for de, f, delta in self.coeffs:
             w = 2 * np.pi * f
             d = 2 * np.pi * delta
 
-            if self._all_larger(d, w):
+            if self._all_larger(d**2, w**2):
                 r = np.sqrt(d * d - w * w) + 0j
                 a0 = -d + r
                 c0 = de * w**2 / 4 / r
                 a1 = -d - r
                 c1 = -c0
                 poles.extend(((a0, c0), (a1, c1)))
             else:
@@ -1847,14 +1956,16 @@
     coeffs: Tuple[Tuple[SpatialDataArray, SpatialDataArray, SpatialDataArray], ...] = pd.Field(
         ...,
         title="Coefficients",
         description="List of (:math:`\\Delta\\epsilon_i, f_i, \\delta_i`) values for model.",
         units=(PERMITTIVITY, HERTZ, HERTZ),
     )
 
+    _warn_if_none = CustomDispersiveMedium._warn_if_data_none("coeffs")
+
     @pd.validator("eps_inf", always=True)
     def _eps_inf_positive(cls, val):
         """eps_inf must be positive"""
         if not CustomDispersiveMedium._validate_isreal_dataarray(val):
             raise SetupError("'eps_inf' must be real.")
         if np.any(val < 0):
             raise SetupError("'eps_inf' must be positive.")
@@ -1865,21 +1976,21 @@
         """f and delta cannot be exactly the same.
         Not needed for now because we have a more strict
         validator `_coeffs_delta_all_smaller_or_larger_than_fi`.
         """
         return val
 
     @pd.validator("coeffs", always=True)
-    def _coeffs_correct_shape_and_sign(cls, val, values):
-        """coeffs must have consistent shape and sign."""
+    def _coeffs_correct_shape(cls, val, values):
+        """coeffs must have consistent shape."""
         if values.get("eps_inf") is None:
             raise ValidationError("'eps_inf' failed validation.")
 
         expected_coords = values["eps_inf"].coords
-        for (de, f, delta) in val:
+        for de, f, delta in val:
             if (
                 de.coords != expected_coords
                 or f.coords != expected_coords
                 or delta.coords != expected_coords
             ):
                 raise SetupError(
                     "All terms in 'coeffs' must have the same coordinates; "
@@ -1887,20 +1998,38 @@
                 )
             if not CustomDispersiveMedium._validate_isreal_dataarray_tuple((de, f, delta)):
                 raise SetupError("All terms in 'coeffs' must be real.")
         return val
 
     @pd.validator("coeffs", always=True)
     def _coeffs_delta_all_smaller_or_larger_than_fi(cls, val):
-        """We restrict either all f>delta or all f<delta for now."""
-        for (_, f, delta) in val:
-            if not (Lorentz._all_larger(f, delta) or Lorentz._all_larger(delta, f)):
+        """We restrict either all f**2>delta**2 or all f**2<delta**2 for now."""
+        for _, f, delta in val:
+            f2 = f**2
+            delta2 = delta**2
+            if not (Lorentz._all_larger(f2, delta2) or Lorentz._all_larger(delta2, f2)):
                 raise SetupError(
                     "Coefficients in 'coeffs' are restricted to have "
-                    "either all 'delta'<'f' or all 'delta'>'f'."
+                    "either all 'delta**2'<'f**2' or all 'delta**2'>'f**2'."
+                )
+        return val
+
+    @pd.validator("coeffs", always=True)
+    def _passivity_validation(cls, val, values):
+        """Assert passive medium if `allow_gain` is False."""
+        allow_gain = values.get("allow_gain")
+        for del_ep, _, delta in val:
+            if np.any(delta < 0):
+                raise ValidationError("For stable medium, 'delta_i' must be non-negative.")
+            if not allow_gain and np.any(del_ep < 0):
+                raise ValidationError(
+                    "For passive medium, 'Delta epsilon_i' must be non-negative. "
+                    "To simulate gain medium, please set 'allow_gain=True'. "
+                    "Caution: simulations with gain medium are unstable, "
+                    "and are likely to diverge."
                 )
         return val
 
     def eps_dataarray_freq(
         self, frequency: float
     ) -> Tuple[SpatialDataArray, SpatialDataArray, SpatialDataArray]:
         """Permittivity array at ``frequency``.
@@ -1951,25 +2080,24 @@
     )
 
     @ensure_freq_in_range
     def eps_model(self, frequency: float) -> complex:
         """Complex-valued permittivity as a function of frequency."""
 
         eps = self.eps_inf + 0.0j
-        for (f, delta) in self.coeffs:
+        for f, delta in self.coeffs:
             eps -= (f**2) / (frequency**2 + 1j * frequency * delta)
         return eps
 
     def _pole_residue_dict(self) -> Dict:
         """Dict representation of Medium as a pole-residue model."""
 
         poles = []
 
-        for (f, delta) in self.coeffs:
-
+        for f, delta in self.coeffs:
             w = 2 * np.pi * f
             d = 2 * np.pi * delta
 
             c0 = (w**2) / 2 / d + 0j
             c1 = -c0
             a1 = -d + 0j
 
@@ -2022,14 +2150,16 @@
     coeffs: Tuple[Tuple[SpatialDataArray, SpatialDataArray], ...] = pd.Field(
         ...,
         title="Coefficients",
         description="List of (:math:`f_i, \\delta_i`) values for model.",
         units=(HERTZ, HERTZ),
     )
 
+    _warn_if_none = CustomDispersiveMedium._warn_if_data_none("coeffs")
+
     @pd.validator("eps_inf", always=True)
     def _eps_inf_positive(cls, val):
         """eps_inf must be positive"""
         if not CustomDispersiveMedium._validate_isreal_dataarray(val):
             raise SetupError("'eps_inf' must be real.")
         if np.any(val < 0):
             raise SetupError("'eps_inf' must be positive.")
@@ -2038,24 +2168,24 @@
     @pd.validator("coeffs", always=True)
     def _coeffs_correct_shape_and_sign(cls, val, values):
         """coeffs must have consistent shape and sign."""
         if values.get("eps_inf") is None:
             raise ValidationError("'eps_inf' failed validation.")
 
         expected_coords = values["eps_inf"].coords
-        for (f, delta) in val:
+        for f, delta in val:
             if f.coords != expected_coords or delta.coords != expected_coords:
                 raise SetupError(
                     "All terms in 'coeffs' must have the same coordinates; "
                     "The coordinates must also be consistent with 'eps_inf'."
                 )
             if not CustomDispersiveMedium._validate_isreal_dataarray_tuple((f, delta)):
                 raise SetupError("All terms in 'coeffs' must be real.")
-            if np.any(delta < 0):
-                raise SetupError("'delta' must be non-negative.")
+            if np.any(delta <= 0):
+                raise SetupError("For stable medium, 'delta' must be positive.")
         return val
 
     def eps_dataarray_freq(
         self, frequency: float
     ) -> Tuple[SpatialDataArray, SpatialDataArray, SpatialDataArray]:
         """Permittivity array at ``frequency``.
 
@@ -2100,28 +2230,43 @@
     coeffs: Tuple[Tuple[float, pd.PositiveFloat], ...] = pd.Field(
         ...,
         title="Coefficients",
         description="List of (:math:`\\Delta\\epsilon_i, \\tau_i`) values for model.",
         units=(PERMITTIVITY, SECOND),
     )
 
+    @pd.validator("coeffs", always=True)
+    def _passivity_validation(cls, val, values):
+        """Assert passive medium if `allow_gain` is False."""
+        if values.get("allow_gain"):
+            return val
+        for del_ep, _ in val:
+            if del_ep < 0:
+                raise ValidationError(
+                    "For passive medium, 'Delta epsilon_i' must be non-negative. "
+                    "To simulate gain medium, please set 'allow_gain=True'. "
+                    "Caution: simulations with gain medium are unstable, "
+                    "and are likely to diverge."
+                )
+        return val
+
     @ensure_freq_in_range
     def eps_model(self, frequency: float) -> complex:
         """Complex-valued permittivity as a function of frequency."""
 
         eps = self.eps_inf + 0.0j
-        for (de, tau) in self.coeffs:
+        for de, tau in self.coeffs:
             eps += de / (1 - 1j * frequency * tau)
         return eps
 
     def _pole_residue_dict(self):
         """Dict representation of Medium as a pole-residue model."""
 
         poles = []
-        for (de, tau) in self.coeffs:
+        for de, tau in self.coeffs:
             a = -2 * np.pi / tau + 0j
             c = -0.5 * de * a
 
             poles.append((a, c))
 
         return dict(
             eps_inf=self.eps_inf,
@@ -2165,40 +2310,56 @@
     coeffs: Tuple[Tuple[SpatialDataArray, SpatialDataArray], ...] = pd.Field(
         ...,
         title="Coefficients",
         description="List of (:math:`\\Delta\\epsilon_i, \\tau_i`) values for model.",
         units=(PERMITTIVITY, SECOND),
     )
 
+    _warn_if_none = CustomDispersiveMedium._warn_if_data_none("coeffs")
+
     @pd.validator("eps_inf", always=True)
     def _eps_inf_positive(cls, val):
         """eps_inf must be positive"""
         if not CustomDispersiveMedium._validate_isreal_dataarray(val):
             raise SetupError("'eps_inf' must be real.")
         if np.any(val < 0):
             raise SetupError("'eps_inf' must be positive.")
         return val
 
     @pd.validator("coeffs", always=True)
-    def _coeffs_correct_shape_and_sign(cls, val, values):
-        """coeffs must have consistent shape and sign."""
+    def _coeffs_correct_shape(cls, val, values):
+        """coeffs must have consistent shape."""
         if values.get("eps_inf") is None:
             raise ValidationError("'eps_inf' failed validation.")
 
         expected_coords = values["eps_inf"].coords
-        for (de, tau) in val:
+        for de, tau in val:
             if de.coords != expected_coords or tau.coords != expected_coords:
                 raise SetupError(
                     "All terms in 'coeffs' must have the same coordinates; "
                     "The coordinates must also be consistent with 'eps_inf'."
                 )
             if not CustomDispersiveMedium._validate_isreal_dataarray_tuple((de, tau)):
                 raise SetupError("All terms in 'coeffs' must be real.")
+        return val
+
+    @pd.validator("coeffs", always=True)
+    def _passivity_validation(cls, val, values):
+        """Assert passive medium if `allow_gain` is False."""
+        allow_gain = values.get("allow_gain")
+        for del_ep, tau in val:
             if np.any(tau <= 0):
-                raise SetupError("'tau' must be positive.")
+                raise SetupError("For stable medium, 'tau_i' must be positive.")
+            if not allow_gain and np.any(del_ep < 0):
+                raise ValidationError(
+                    "For passive medium, 'Delta epsilon_i' must be non-negative. "
+                    "To simulate gain medium, please set 'allow_gain=True'. "
+                    "Caution: simulations with gain medium are unstable, "
+                    "and are likely to diverge."
+                )
         return val
 
     def eps_dataarray_freq(
         self, frequency: float
     ) -> Tuple[SpatialDataArray, SpatialDataArray, SpatialDataArray]:
         """Permittivity array at ``frequency``.
 
@@ -2260,14 +2421,29 @@
     zz: IsotropicUniformMediumType = pd.Field(
         ...,
         title="ZZ Component",
         description="Medium describing the zz-component of the diagonal permittivity tensor.",
         discriminator=TYPE_TAG_STR,
     )
 
+    allow_gain: bool = pd.Field(
+        None,
+        title="Allow gain medium",
+        description="This field is ignored. Please set ``allow_gain`` in each component",
+    )
+
+    @pd.root_validator(pre=True)
+    def _ignored_fields(cls, values):
+        """The field is ignored."""
+        if values.get("xx") is not None and values.get("allow_gain") is not None:
+            log.warning(
+                "The field 'allow_gain' is ignored. Please set 'allow_gain' in each component."
+            )
+        return values
+
     @cached_property
     def components(self) -> Dict[str, Medium]:
         """Dictionary of diagonal medium components."""
         return dict(xx=self.xx, yy=self.yy, zz=self.zz)
 
     @cached_property
     def n_cfl(self):
@@ -2322,15 +2498,14 @@
     def plot(self, freqs: float, ax: Ax = None) -> Ax:
         """Plot n, k of a :class:`.Medium` as a function of frequency."""
 
         freqs = np.array(freqs)
         freqs_thz = freqs / 1e12
 
         for label, medium_component in self.elements.items():
-
             eps_complex = medium_component.eps_model(freqs)
             n, k = AbstractMedium.eps_complex_to_nk(eps_complex)
             ax.plot(freqs_thz, n, label=f"n, eps_{label}")
             ax.plot(freqs_thz, k, label=f"k, eps_{label}")
 
         ax.set_xlabel("frequency (THz)")
         ax.set_title("medium dispersion")
@@ -2391,31 +2566,44 @@
 
         if np.any(np.linalg.eigvals(val) < 1 - fp_eps):
             raise ValidationError("Main diagonal of provided permittivity tensor is not >= 1.")
 
         return val
 
     @pd.validator("conductivity", always=True)
-    def conductivity_ge_zero_and_commutes(cls, val, values):
+    def conductivity_commutes(cls, val, values):
         """Check that the symmetric part of conductivity tensor commutes with permittivity tensor
-        (that is, simultaneously diagonalizable) with eigenvalues >= 0.
+        (that is, simultaneously diagonalizable).
         """
 
         perm = values.get("permittivity")
         cond_sym = 0.5 * (val + val.T)
         comm_diff = np.abs(np.matmul(perm, cond_sym) - np.matmul(cond_sym, perm))
 
         if not np.allclose(comm_diff, 0, atol=fp_eps):
             raise ValidationError(
                 "Main directions of conductivity and permittivity tensor do not coincide."
             )
 
-        if np.any(np.linalg.eigvals(cond_sym) < -fp_eps):
-            raise ValidationError("Main diagonal of provided conductivity tensor is not >= 0.")
+        return val
 
+    @pd.validator("conductivity", always=True)
+    def _passivity_validation(cls, val, values):
+        """Assert passive medium if `allow_gain` is False."""
+        if values.get("allow_gain"):
+            return val
+
+        cond_sym = 0.5 * (val + val.T)
+        if np.any(np.linalg.eigvals(cond_sym) < -fp_eps):
+            raise ValidationError(
+                "For passive medium, main diagonal of provided conductivity tensor "
+                "must be non-negative. "
+                "To simulate gain medium, please set 'allow_gain=True'. "
+                "Caution: simulations with gain medium are unstable, and are likely to diverge."
+            )
         return val
 
     @classmethod
     def from_diagonal(cls, xx: Medium, yy: Medium, zz: Medium, rotation: RotationType):
         """Construct a fully anisotropic medium by rotating a diagonally ansisotropic medium.
 
         Parameters
@@ -2596,14 +2784,26 @@
         None,
         title="Interpolation method",
         description="When the value is 'None', each component will follow its own "
         "interpolation method. When the value is other than 'None', the interpolation "
         "method specified by this field will override the one in each component.",
     )
 
+    allow_gain: bool = pd.Field(
+        None,
+        title="Allow gain medium",
+        description="This field is ignored. Please set ``allow_gain`` in each component",
+    )
+
+    subpixel: bool = pd.Field(
+        None,
+        title="Subpixel averaging",
+        description="This field is ignored. Please set ``subpixel`` in each component",
+    )
+
     @pd.validator("xx", always=True)
     def _isotropic_xx(cls, val):
         """If it's `CustomMedium`, make sure it's isotropic."""
         if isinstance(val, CustomMedium) and not val.is_isotropic:
             raise SetupError("The xx-component medium type is not isotropic.")
         return val
 
@@ -2617,14 +2817,28 @@
     @pd.validator("zz", always=True)
     def _isotropic_zz(cls, val):
         """If it's `CustomMedium`, make sure it's isotropic."""
         if isinstance(val, CustomMedium) and not val.is_isotropic:
             raise SetupError("The zz-component medium type is not isotropic.")
         return val
 
+    @pd.root_validator(pre=True)
+    def _ignored_fields(cls, values):
+        """The field is ignored."""
+        if values.get("xx") is not None:
+            if values.get("allow_gain") is not None:
+                log.warning(
+                    "The field 'allow_gain' is ignored. Please set 'allow_gain' in each component."
+                )
+            if values.get("subpixel") is not None:
+                log.warning(
+                    "The field 'subpixel' is ignored. Please set 'subpixel' in each component."
+                )
+        return values
+
     @cached_property
     def n_cfl(self):
         """This property computes the index of refraction related to CFL condition, so that
         the FDTD with this medium is stable when the time step size that doesn't take
         material factor into account is multiplied by ``n_cfl``.
 
         For this medium, it takes the minimal of ``n_clf`` in all components.
@@ -2774,15 +2988,15 @@
     @classmethod
     def _weighted_avg(
         cls, meds: List[IsotropicUniformMediumType], weights: List[float]
     ) -> PoleResidue:
         """Average ``meds`` with weights ``weights``."""
         eps_inf = 1
         poles = []
-        for (med, weight) in zip(meds, weights):
+        for med, weight in zip(meds, weights):
             if isinstance(med, DispersiveMedium):
                 pole_res = med.pole_residue
                 eps_inf += weight * (med.pole_residue.eps_inf - 1)
             elif isinstance(med, Medium):
                 pole_res = PoleResidue.from_medium(med)
                 eps_inf += weight * (med.eps_model(np.inf) - 1)
             elif isinstance(med, PECMedium):
@@ -3014,15 +3228,14 @@
             "to obtain the physical refractive index."
         )
 
         freqs = np.array(freqs)
         freqs_thz = freqs / 1e12
 
         for label, medium_component in self.elements.items():
-
             eps_complex = medium_component.eps_model(freqs)
             n, k = AbstractMedium.eps_complex_to_nk(eps_complex)
             ax.plot(freqs_thz, n, label=f"n, eps_{label}")
             ax.plot(freqs_thz, k, label=f"k, eps_{label}")
 
         ax.set_xlabel("frequency (THz)")
         ax.set_title("medium dispersion")
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/mode.py` & `tidy3d-2.3.1/tidy3d/components/mode.py`

 * *Files 8% similar despite different names*

```diff
@@ -144,13 +144,8 @@
         """Verify critical ModeSpec settings for group index calculation."""
         if values["group_index_step"] > 0:
             if values["track_freq"] is None:
                 log.warning(
                     "Group index calculation without mode tracking can lead to incorrect results "
                     "around mode crossings. Consider setting 'track_freq' to 'central'."
                 )
-            if values["precision"] != "double":
-                log.warning(
-                    "Group index calculation should be performed with double precision for better "
-                    "accuracy. Consider setting 'precision' to 'double'."
-                )
         return values
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/monitor.py` & `tidy3d-2.3.1/tidy3d/components/monitor.py`

 * *Files 11% similar despite different names*

```diff
@@ -144,15 +144,15 @@
             tend = np.nonzero(tmesh <= t_stop)[0]
             if tend.size > 0:
                 tind_end = int(tend[-1] + 1)
 
         # Step to compare to in order to handle t_start = t_stop
         dt = 1e-20 if np.array(tmesh).size < 2 else tmesh[1] - tmesh[0]
         # If equal start and stopping time, record one time step
-        if np.abs(self.start - t_stop) < dt:
+        if np.abs(self.start - t_stop) < dt and self.start <= tmesh[-1]:
             tind_beg = max(tind_end - 1, 0)
         else:
             tbeg = np.nonzero(tmesh[:tind_end] >= self.start)[0]
             tind_beg = tbeg[0] if tbeg.size > 0 else tind_end
         return (tind_beg, tind_end)
 
     def num_steps(self, tmesh: ArrayFloat1D) -> int:
@@ -452,14 +452,19 @@
         # stores 1 real number per time step
         num_steps = self.num_steps(tmesh)
         return BYTES_REAL * num_steps
 
 
 class ModeMonitor(AbstractModeMonitor):
     """:class:`Monitor` that records amplitudes from modal decomposition of fields on plane.
+    The amplitudes are defined as
+    ``mode_solver_data.dot(recorded_field) / mode_solver_data.dot(mode_solver_data)``, where
+    ``recorded_field`` is the field data recorded in the FDTD simulation at the monitor frequencies,
+    and ``mode_solver_data`` is the mode data from the mode solver at the monitor plane.
+    This gives the power amplitude of ``recorded_field`` carried by each mode.
 
     Example
     -------
     >>> mode_spec = ModeSpec(num_modes=3)
     >>> monitor = ModeMonitor(
     ...     center=(1,2,3),
     ...     size=(2,2,0),
@@ -485,14 +490,21 @@
     ...     center=(1,2,3),
     ...     size=(2,2,0),
     ...     freqs=[200e12, 210e12],
     ...     mode_spec=mode_spec,
     ...     name='mode_monitor')
     """
 
+    direction: Direction = pydantic.Field(
+        "+",
+        title="Propagation direction",
+        description="Direction of waveguide mode propagation along the axis defined by its normal "
+        "dimension.",
+    )
+
     def storage_size(self, num_cells: int, tmesh: int) -> int:
         """Size of monitor storage given the number of points after discretization."""
         return 6 * BYTES_COMPLEX * num_cells * len(self.freqs) * self.mode_spec.num_modes
 
     @property
     def interval_space(self):
         """No downsampling is applied to the stored fields."""
@@ -548,15 +560,19 @@
         "monitor's center.",
         units=MICROMETER,
     )
 
     far_field_approx: bool = pydantic.Field(
         True,
         title="Far field approximation",
-        description="Whether to enable the far field approximation when projecting fields.",
+        description="Whether to enable the far field approximation when projecting fields. "
+        "If ``True``, terms that decay as O(1/r^2) are ignored, as are the radial components "
+        "of fields. Typically, this should be set to ``True`` only when the projection distance "
+        "is much larger than the size of the device being modeled, and the projected points are "
+        "in the far field of the device.",
     )
 
     @property
     def projection_surfaces(self) -> Tuple[FieldProjectionSurface, ...]:
         """Surfaces of the monitor where near fields will be recorded for subsequent projection."""
         surfaces = self.integration_surfaces
         return [
@@ -575,15 +591,27 @@
         if self.custom_origin is None:
             return self.center
         return self.custom_origin
 
 
 class FieldProjectionAngleMonitor(AbstractFieldProjectionMonitor):
     """:class:`Monitor` that samples electromagnetic near fields in the frequency domain
-    and projects them at given observation angles.
+    and projects them at given observation angles. The ``center`` and ``size`` fields define
+    where the monitor will be placed in order to record near fields, typically very close
+    to the structure of interest. The near fields are then projected
+    to far-field locations defined by ``phi``, ``theta``, and ``proj_distance``, relative
+    to the ``custom_origin``. If the distance between the near and far field locations is
+    much larger than the size of the device, one can typically set ``far_field_approx`` to
+    ``True``, which will make use of the far-field approximation to speed up calculations.
+    If the projection distance is comparable to the size of the device, we recommend setting
+    ``far_field_approx`` to ``False``, so that the approximations are not used, and the
+    projection is accurate even just a few wavelengths away from the near field locations.
+    For applications where the monitor is an open surface rather than a box that
+    encloses the device, it is advisable to pick the size of the monitor such that the
+    recorded near fields decay to negligible values near the edges of the monitor.
 
     Example
     -------
     >>> monitor = FieldProjectionAngleMonitor(
     ...     center=(1,2,3),
     ...     size=(2,2,2),
     ...     freqs=[250e12, 300e12],
@@ -622,15 +650,29 @@
         # stores 1 complex number per pair of angles, per frequency,
         # for Er, Etheta, Ephi, Hr, Htheta, and Hphi (6 components)
         return BYTES_COMPLEX * len(self.theta) * len(self.phi) * len(self.freqs) * 6
 
 
 class FieldProjectionCartesianMonitor(AbstractFieldProjectionMonitor):
     """:class:`Monitor` that samples electromagnetic near fields in the frequency domain
-    and projects them on a Cartesian observation plane.
+    and projects them on a Cartesian observation plane. The ``center`` and ``size`` fields define
+    where the monitor will be placed in order to record near fields, typically very close
+    to the structure of interest. The near fields are then projected
+    to far-field locations defined by ``x``, ``y``, and ``proj_distance``, relative
+    to the ``custom_origin``. Here, ``x`` and ``y`` correspond to a local coordinate system
+    where the local z axis is defined by ``proj_axis``: which is the axis normal to this monitor.
+    If the distance between the near and far field locations is much larger than the size of the
+    device, one can typically set ``far_field_approx`` to ``True``, which will make use of the
+    far-field approximation to speed up calculations. If the projection distance is comparable
+    to the size of the device, we recommend setting ``far_field_approx`` to ``False``,
+    so that the approximations are not used, and the projection is accurate even just a few
+    wavelengths away from the near field locations.
+    For applications where the monitor is an open surface rather than a box that
+    encloses the device, it is advisable to pick the size of the monitor such that the
+    recorded near fields decay to negligible values near the edges of the monitor.
 
     Example
     -------
     >>> monitor = FieldProjectionCartesianMonitor(
     ...     center=(1,2,3),
     ...     size=(2,2,2),
     ...     freqs=[250e12, 300e12],
@@ -682,15 +724,29 @@
         # stores 1 complex number per pair of grid points, per frequency,
         # for Er, Etheta, Ephi, Hr, Htheta, and Hphi (6 components)
         return BYTES_COMPLEX * len(self.x) * len(self.y) * len(self.freqs) * 6
 
 
 class FieldProjectionKSpaceMonitor(AbstractFieldProjectionMonitor):
     """:class:`Monitor` that samples electromagnetic near fields in the frequency domain
-    and projects them on an observation plane defined in k-space.
+    and projects them on an observation plane defined in k-space. The ``center`` and ``size``
+    fields define where the monitor will be placed in order to record near fields, typically
+    very close to the structure of interest. The near fields are then
+    projected to far-field locations defined in k-space by ``ux``, ``uy``, and ``proj_distance``,
+    relative to the ``custom_origin``. Here, ``ux`` and ``uy`` are associated with a local
+    coordinate system where the local 'z' axis is defined by ``proj_axis``: which is the axis
+    normal to this monitor. If the distance between the near and far field locations is much
+    larger than the size of the device, one can typically set ``far_field_approx`` to ``True``,
+    which will make use of the far-field approximation to speed up calculations. If the
+    projection distance is comparable to the size of the device, we recommend setting
+    ``far_field_approx`` to ``False``, so that the approximations are not used, and the
+    projection is accurate even just a few wavelengths away from the near field locations.
+    For applications where the monitor is an open surface rather than a box that
+    encloses the device, it is advisable to pick the size of the monitor such that the
+    recorded near fields decay to negligible values near the edges of the monitor.
 
     Example
     -------
     >>> monitor = FieldProjectionKSpaceMonitor(
     ...     center=(1,2,3),
     ...     size=(2,2,2),
     ...     freqs=[250e12, 300e12],
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/simulation.py` & `tidy3d-2.3.1/tidy3d/components/simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from .medium import AnisotropicMedium, FullyAnisotropicMedium
 from .boundary import BoundarySpec, BlochBoundary, PECBoundary, PMCBoundary, Periodic
 from .boundary import PML, StablePML, Absorber, AbsorberSpec
 from .structure import Structure
 from .source import SourceType, PlaneWave, GaussianBeam, AstigmaticGaussianBeam, CustomFieldSource
 from .source import CustomCurrentSource
 from .source import TFSF, Source
-from .monitor import MonitorType, Monitor, FreqMonitor
+from .monitor import MonitorType, Monitor, FreqMonitor, SurfaceIntegrationMonitor
 from .monitor import AbstractFieldMonitor, DiffractionMonitor, AbstractFieldProjectionMonitor
 from .data.dataset import Dataset
 from .viz import add_ax_if_none, equal_aspect
 
 from .viz import MEDIUM_CMAP, STRUCTURE_EPS_CMAP, PlotParams, plot_params_symmetry, polygon_path
 from .viz import plot_params_structure, plot_params_pml, plot_params_override_structures
 from .viz import plot_params_pec, plot_params_pmc, plot_params_bloch, plot_sim_3d
@@ -46,15 +46,16 @@
 # minimum number of grid points allowed per central wavelength in a medium
 MIN_GRIDS_PER_WVL = 6.0
 
 # maximum number of mediums supported
 MAX_NUM_MEDIUMS = 65530
 
 # maximum numbers of simulation parameters
-MAX_TIME_STEPS = 1e8
+MAX_TIME_STEPS = 1e7
+WARN_TIME_STEPS = 1e6
 MAX_GRID_CELLS = 20e9
 MAX_CELLS_TIMES_STEPS = 1e16
 WARN_MONITOR_DATA_SIZE_GB = 10
 MAX_SIMULATION_DATA_SIZE_GB = 50
 
 # number of grid cells at which we warn about slow Simulation.epsilon()
 NUM_CELLS_WARN_EPSILON = 100_000_000
@@ -239,15 +240,15 @@
     @pydantic.validator("grid_spec", always=True)
     def _validate_auto_grid_wavelength(cls, val, values):
         """Check that wavelength can be defined if there is auto grid spec."""
         if val.wavelength is None and val.auto_grid_used:
             _ = val.wavelength_from_sources(sources=values.get("sources"))
         return val
 
-    _structures_in_bounds = assert_objects_in_sim_bounds("structures")
+    _structures_in_bounds = assert_objects_in_sim_bounds("structures", error=False)
     _sources_in_bounds = assert_objects_in_sim_bounds("sources")
     _monitors_in_bounds = assert_objects_in_sim_bounds("monitors")
     _mode_sources_symmetries = validate_mode_objects_symmetry("sources")
     _mode_monitors_symmetries = validate_mode_objects_symmetry("monitors")
 
     # make sure all names are unique
     _unique_structure_names = assert_unique_names("structures")
@@ -574,15 +575,15 @@
             raise ValidationError(
                 "could not validate `_warn_monitor_simulation_frequency_range` "
                 "as `sources` failed validation"
             )
 
         source_ranges = [source.source_time.frequency_range() for source in values["sources"]]
         if not source_ranges:
-            log.warning("No sources in simulation.")
+            log.info("No sources in simulation.")
             return val
 
         freq_min = min((freq_range[0] for freq_range in source_ranges), default=0.0)
         freq_max = max((freq_range[1] for freq_range in source_ranges), default=0.0)
 
         with log as consolidated_logger:
             for monitor_index, monitor in enumerate(val):
@@ -651,14 +652,36 @@
                         f"{len(mediums)} different mediums detected on plane "
                         f"intersecting a {monitor.type}. Plane must be homogeneous."
                     )
 
         return val
 
     @pydantic.validator("monitors", always=True)
+    def _integration_surfaces_in_bounds(cls, val, values):
+        """Error if any of the integration surfaces are outside of the simulation domain."""
+
+        if val is None:
+            return val
+
+        sim_center = values.get("center")
+        sim_size = values.get("size")
+        sim_box = Box(size=sim_size, center=sim_center)
+
+        for mnt in (mnt for mnt in val if isinstance(mnt, SurfaceIntegrationMonitor)):
+            for surface in mnt.integration_surfaces:
+                if not sim_box.intersects(surface):
+                    raise SetupError(
+                        f"Integration surface '{surface.name}' of monitor "
+                        f"'{mnt.name}' is outside of the simulation bounds. Modify monitor "
+                        "geometry or use 'exclude_surfaces' to exclude that surface."
+                    )
+
+        return val
+
+    @pydantic.validator("monitors", always=True)
     def _projection_monitors_distance(cls, val, values):
         """Warn if the projection distance is large for exact projections."""
 
         if val is None:
             return val
 
         sim_size = values.get("size")
@@ -885,22 +908,30 @@
                             f"source '{source.name}'. For best results, we recommended ensuring a "
                             "uniform grid in both directions tangential to the TFSF injection "
                             f"axis, '{'xyz'[source.injection_axis]}'."
                         )
 
     """ Pre submit validation (before web.upload()) """
 
-    def validate_pre_upload(self) -> None:
-        """Validate the fully initialized simulation is ok for upload to our servers."""
+    def validate_pre_upload(self, source_required: bool = True) -> None:
+        """Validate the fully initialized simulation is ok for upload to our servers.
+
+        Parameters
+        ----------
+        source_required: bool = True
+            If ``True``, validation will fail in case no sources are found in the simulation.
+        """
         self._validate_size()
         self._validate_monitor_size()
         self._validate_datasets_not_none()
         self._validate_tfsf_structure_intersections()
         # self._validate_run_time()
         _ = self.volumetric_structures
+        if source_required and len(self.sources) == 0:
+            raise SetupError("No sources in simulation.")
 
     def _validate_size(self) -> None:
         """Ensures the simulation is within size limits before simulation is uploaded."""
 
         num_comp_cells = self.num_cells / 2 ** (np.sum(np.abs(self.symmetry)))
         if num_comp_cells > MAX_GRID_CELLS:
             raise SetupError(
@@ -910,14 +941,19 @@
 
         num_time_steps = self.num_time_steps
         if num_time_steps > MAX_TIME_STEPS:
             raise SetupError(
                 f"Simulation has {num_time_steps:.2e} time steps, "
                 f"a maximum of {MAX_TIME_STEPS:.2e} are allowed."
             )
+        if num_time_steps > WARN_TIME_STEPS:
+            log.warning(
+                f"Simulation has {num_time_steps:.2e} time steps. The 'run_time' may be "
+                "unnecessarily large, unless there are very long-lived resonances."
+            )
 
         num_cells_times_steps = num_time_steps * num_comp_cells
         if num_cells_times_steps > MAX_CELLS_TIMES_STEPS:
             raise SetupError(
                 f"Simulation has {num_cells_times_steps:.2e} grid cells * time steps, "
                 f"a maximum of {MAX_CELLS_TIMES_STEPS:.2e} are allowed."
             )
@@ -2765,7 +2801,19 @@
         return tuple(new_structures)
 
     @cached_property
     def volumetric_structures(self) -> Tuple[Structure]:
         """Generate a tuple of structures wherein any 2D materials are converted to 3D
         volumetric equivalents."""
         return self._volumetric_structures_grid(self.grid)
+
+    @cached_property
+    def allow_gain(self) -> bool:
+        """``True`` if any of the mediums in the simulation allows gain."""
+
+        for medium in self.mediums:
+            if isinstance(medium, AnisotropicMedium):
+                if np.any([med.allow_gain for med in [medium.xx, medium.yy, medium.zz]]):
+                    return True
+            elif medium.allow_gain:
+                return True
+        return False
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/source.py` & `tidy3d-2.3.1/tidy3d/components/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -406,25 +406,38 @@
         component = self.polarization[-1]  # 'x' 'y' or 'z'
         pol_axis = "xyz".index(component)
         pol_vec = [0, 0, 0]
         pol_vec[pol_axis] = 1
         return pol_vec
 
 
-class UniformCurrentSource(CurrentSource):
+class ReverseInterpolatedSource(Source):
+    """Abstract source that allows reverse-interpolation along zero-sized dimensions."""
+
+    interpolate: bool = pydantic.Field(
+        True,
+        title="Enable Interpolation",
+        description="Handles reverse-interpolation of zero-size dimensions of the source. "
+        "If ``False``, the source data is snapped to the nearest Yee grid point. If ``True``, "
+        "equivalent source data is applied on the surrounding Yee grid points to emulate "
+        "placement at the specified location using linear interpolation.",
+    )
+
+
+class UniformCurrentSource(CurrentSource, ReverseInterpolatedSource):
     """Source in a rectangular volume with uniform time dependence. size=(0,0,0) gives point source.
 
     Example
     -------
     >>> pulse = GaussianPulse(freq0=200e12, fwidth=20e12)
     >>> pt_source = UniformCurrentSource(size=(0,0,0), source_time=pulse, polarization='Ex')
     """
 
 
-class PointDipole(CurrentSource):
+class PointDipole(CurrentSource, ReverseInterpolatedSource):
     """Uniform current source with a zero size.
 
     Example
     -------
     >>> pulse = GaussianPulse(freq0=200e12, fwidth=20e12)
     >>> pt_dipole = PointDipole(center=(1,2,3), source_time=pulse, polarization='Ex')
     """
@@ -432,32 +445,23 @@
     size: Tuple[Literal[0], Literal[0], Literal[0]] = pydantic.Field(
         (0, 0, 0),
         title="Size",
         description="Size in x, y, and z directions, constrained to ``(0, 0, 0)``.",
         units=MICROMETER,
     )
 
-    interpolate: bool = pydantic.Field(
-        True,
-        title="Enable Interpolation",
-        description="If ``False``, the dipole is placed at the nearest Yee grid point "
-        "based on the chosen ``polarization``. If ``True``, uses linear interpolation "
-        "so that effectively the dipole is placed at the exact position requested.",
-    )
-
 
-class CustomCurrentSource(Source):
+class CustomCurrentSource(ReverseInterpolatedSource):
     """Implements a source corresponding to an input dataset containing ``E`` and ``H`` fields.
     Injects the specified components of the ``E`` and ``H`` dataset directly as ``J`` and ``M``
     current distributions in the FDTD solver.
 
     Note
     ----
-        If only the ``E`` or only the ``H`` fields are provided, the source will not be directional,
-        but will inject equal power in both directions instead.
+        The coordinates of all provided fields are assumed to be relative to the source center.
 
     Example
     -------
     >>> from tidy3d import ScalarFieldDataArray
     >>> pulse = GaussianPulse(freq0=200e12, fwidth=20e12)
     >>> x = np.linspace(-1, 1, 101)
     >>> y = np.linspace(-1, 1, 101)
@@ -578,24 +582,27 @@
         return val
 
 
 """ Source current profiles determined by user-supplied data on a plane."""
 
 
 class CustomFieldSource(FieldSource, PlanarSource):
-    """Implements a source corresponding to an input dataset containing ``E`` and ``H`` fields.
-    For the injection to work as expected, the fields must decay by the edges of the source plane,
-    or the source plane must span the entire simulation domain and the fields must match the
-    simulation boundary conditions. The equivalent source currents are fully defined by the field
-    components tangential to the source plane. The normal components (e.g. ``Ez`` and ``Hz``) can be
-    provided but will have no effect on the results, in accordance with the equivalence principle.
-    At least one of the tangential components has to be defined. For example, for a ``z``-normal
-    source, at least one of ``Ex``, ``Ey``, ``Hx``, and ``Hy`` has to be present in the provided
-    dataset. The coordinates of all provided fields are assumed to be relative to the source
-    center. Each provided field component must also span the size of the source.
+    """Implements a source corresponding to an input dataset containing ``E`` and ``H`` fields,
+    using the equivalence principle to define the actual injected currents. For the injection to
+    work as expected (i.e. to reproduce the required ``E`` and ``H`` fields), the field data must
+    decay by the edges of the source plane, or the source plane must span the entire simulation
+    domain and the fields must match the simulation boundary conditions.
+    The equivalent source currents are fully defined by the field components tangential to the
+    source plane. For e.g. source normal along ``z``, the normal components (``Ez`` and ``Hz``)
+    can be provided but will have no effect on the results, and at least one of the tangential
+    components has to be in the dataset, i.e. at least one of ``Ex``, ``Ey``, ``Hx``, and ``Hy``.
+
+    Note
+    ----
+        The coordinates of all provided fields are assumed to be relative to the source center.
 
     Note
     ----
         If only the ``E`` or only the ``H`` fields are provided, the source will not be directional,
         but will inject equal power in both directions instead.
 
     Example
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/structure.py` & `tidy3d-2.3.1/tidy3d/components/structure.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/transformation.py` & `tidy3d-2.3.1/tidy3d/components/transformation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/types.py` & `tidy3d-2.3.1/tidy3d/components/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
     @classmethod
     def __get_validators__(cls):
         yield cls.load_complex
         yield cls.convert_to_numpy
         yield cls.check_dims
         yield cls.check_shape
+        yield cls.assert_non_null
 
     @classmethod
     def load_complex(cls, val):
         """Special handling to load a complex-valued np.ndarray saved to file."""
         if not isinstance(val, dict):
             return val
         if "real" not in val or "imag" not in val:
@@ -82,37 +83,47 @@
     def check_shape(cls, val):
         """Make sure the shape is correct."""
         if cls.shape and val.shape != cls.shape:
             raise ValidationError(f"Expected shape {cls.shape} for ArrayLike, got {val.shape}.")
         return val
 
     @classmethod
+    def assert_non_null(cls, val):
+        """Make sure array is not None."""
+        if np.any(np.isnan(val)):
+            raise ValidationError("'ArrayLike' field contained None or nan values.")
+        return val
+
+    @classmethod
     def __modify_schema__(cls, field_schema):
         """Sets the schema of DataArray object."""
 
         schema = dict(
-            title="ArrayLike",
             type="ArrayLike",
         )
         field_schema.update(schema)
 
 
 def constrained_array(
     dtype: type = None, ndim: int = None, shape: Tuple[pydantic.NonNegativeInt, ...] = None
 ) -> type:
     """Generate an ArrayLike sub-type with constraints built in."""
 
     # note, a unique name is required for each subclass of ArrayLike with constraints
     type_name = "ArrayLike"
+
+    meta_args = []
     if dtype is not None:
-        type_name += f"_dtype={dtype}"
+        meta_args.append(f"dtype={dtype.__name__}")
     if ndim is not None:
-        type_name += f"_ndim={ndim}"
+        meta_args.append(f"ndim={ndim}")
     if shape is not None:
-        type_name += f"_shape={shape}"
+        meta_args.append(f"shape={shape}")
+    type_name += "[" + ", ".join(meta_args) + "]"
+
     return type(type_name, (ArrayLike,), dict(dtype=dtype, ndim=ndim, shape=shape))
 
 
 # pre-define a set of commonly used array like instances for import and use in type hints
 ArrayFloat1D = constrained_array(dtype=float, ndim=1)
 ArrayFloat2D = constrained_array(dtype=float, ndim=2)
 ArrayFloat3D = constrained_array(dtype=float, ndim=3)
@@ -216,11 +227,12 @@
 FieldVal = Literal["real", "imag", "abs", "abs^2", "phase"]
 PlotScale = Literal["lin", "dB"]
 ColormapType = Literal["divergent", "sequential", "cyclic"]
 
 """ mode solver """
 
 ModeSolverType = Literal["tensorial", "diagonal"]
+EpsSpecType = Literal["diagonal", "tensorial_real", "tensorial_complex"]
 
 """ mode tracking """
 
 TrackFreq = Literal["central", "lowest", "highest"]
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/validators.py` & `tidy3d-2.3.1/tidy3d/components/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,32 +149,36 @@
         if len(unique_names) != len(field_names):
             raise SetupError(f"'{field_name}' names are not unique, given {field_names}.")
         return val
 
     return field_has_unique_names
 
 
-def assert_objects_in_sim_bounds(field_name: str):
+def assert_objects_in_sim_bounds(field_name: str, error: bool = True):
     """Makes sure all objects in field are at least partially inside of simulation bounds."""
 
     @pydantic.validator(field_name, allow_reuse=True, always=True)
     def objects_in_sim_bounds(cls, val, values):
         """check for intersection of each structure with simulation bounds."""
         sim_center = values.get("center")
         sim_size = values.get("size")
         sim_box = Box(size=sim_size, center=sim_center)
 
         for position_index, geometric_object in enumerate(val):
             if not sim_box.intersects(geometric_object.geometry):
-                raise SetupError(
-                    f"'{geometric_object}' "
-                    f"(at `simulation.{field_name}[{position_index}]`) "
+
+                message = (
+                    f"'{geometric_object}' (at `simulation.{field_name}[{position_index}]`) "
                     "is completely outside of simulation domain."
                 )
 
+                if error:
+                    raise SetupError(message)
+                log.warning(message)
+
         return val
 
     return objects_in_sim_bounds
 
 
 def enforce_monitor_fields_present():
     """Make sure all of the fields in the monitor are present in the correponding data."""
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/components/viz.py` & `tidy3d-2.3.1/tidy3d/components/viz.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/config.py` & `tidy3d-2.3.1/tidy3d/config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/constants.py` & `tidy3d-2.3.1/tidy3d/constants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/exceptions.py` & `tidy3d-2.3.1/tidy3d/exceptions.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/log.py` & `tidy3d-2.3.1/tidy3d/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,22 @@
     "CRITICAL": 50,
 }
 
 _level_name = {v: k for k, v in _level_value.items()}
 
 DEFAULT_LEVEL = "WARNING"
 
+DEFAULT_LOG_STYLES = {
+    "DEBUG": None,
+    "INFO": None,
+    "WARNING": "red",
+    "ERROR": "red bold",
+    "CRITICAL": "red bold",
+}
+
 
 def _get_level_int(level: LogValue) -> int:
     """Get the integer corresponding to the level string."""
     if isinstance(level, int):
         return level
 
     if level not in _level_value:
@@ -50,15 +58,21 @@
         """Output log messages depending on log level"""
         if level >= self.level:
             stack = inspect.stack()
             offset = 4
             if stack[offset - 1].filename.endswith("exceptions.py"):
                 # We want the calling site for exceptions.py
                 offset += 1
-            self.console.log(level_name, message, sep=": ", _stack_offset=offset)
+            self.console.log(
+                level_name,
+                message,
+                sep=": ",
+                style=DEFAULT_LOG_STYLES[level_name],
+                _stack_offset=offset,
+            )
 
 
 class Logger:
     """Custom logger to avoid the complexities of the logging module
 
     The logger can be used in a context manager to avoid the emission of multiple messages. In this
     case, the first message in the context is emitted normally, but any others are discarded. When
@@ -306,16 +320,17 @@
         raise ValueError("filemode must be either 'w' or 'a'")
 
     # Close previous handler, if any
     if "file" in log.handlers:
         try:
             log.handlers["file"].file.close()
         except:  # pylint: disable=bare-except
-            del log.handlers["file"]
             log.warning("Log file could not be closed")
+        finally:
+            del log.handlers["file"]
 
     try:
         # pylint: disable=consider-using-with
         file = open(fname, filemode)
     except:  # pylint: disable=bare-except
         log.error(f"File {fname} could not be opened")
         return
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/material_library/material_library.py` & `tidy3d-2.3.1/tidy3d/material_library/material_library.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,15 +134,16 @@
                 (-76642436669493.88 + 1j * 123745349008080.44),
                 (129838572187083.62 - 1j * 2.1821880909947117e17),
             ),
         ],
         frequency_range=(24179892422719.273, 1208994621135963.5),
     ),
     reference=[material_refs["Rakic1998"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Ag/Rakic-BB.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Ag/Rakic-BB.yml",
 )
 
 Ag_RakicLorentzDrude1998 = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=(
             ((-800062663506.125 + 0j), (1.1099533667426209e18 + 0j)),
@@ -153,15 +154,16 @@
             ((-49376192059874.14 - 1.2435106032980426e16j), 82876469878486.64j),
             ((-695824491182226.4 - 1.3781951983423364e16j), 5710269496109004j),
             ((-1837553978351315.8 - 3.0771118889340676e16j), 1.7190386342847058e16j),
         ),
         frequency_range=(24179892422719.273, 1208994621135963.5),
     ),
     reference=[material_refs["Rakic1998"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Ag/Rakic-LD.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Ag/Rakic-LD.yml",
 )
 
 Ag_JohnsonChristy1972 = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0000740219977509,
         poles=(
             ((-1306213662214179.8 - 6200791340906446j), (5316579866298263 + 770314552771784.5j)),
@@ -173,15 +175,16 @@
                 (-1414117800340546 - 841892406600516.1j),
                 (-3015811271404633.5 - 1.627264404485923e16j),
             ),
         ),
         frequency_range=(154771532566312.25, 1595489401708072.2),
     ),
     reference=[material_refs["JohnsonChristy1972"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Ag/Johnson.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Ag/Johnson.yml",
 )
 
 Ag_Yang2015Drude = VariantItem(
     medium=PoleResidue(
         eps_inf=5.0,
         poles=(
             (
@@ -192,15 +195,16 @@
                 (-58823530000000 + 0j),
                 (-1.5540587685959158e18 - 0j),
             ),
         ),
         frequency_range=(154771532566312.25, 1595489401708072.2),
     ),
     reference=[material_refs["Yang2015"]],
-    data_url="https://refractiveindex.info/database/data/main/Ag/Yang.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Ag/Yang.yml",
 )
 
 Al_Rakic1995 = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=[
             (
@@ -220,15 +224,16 @@
                 (-1.0180997365823526e16 - 1j * 5542555481403632.0),
                 (-1.6978040336362288e16 - 1j * 1.4140848316870884e16),
             ),
         ],
         frequency_range=(151926744799612.75, 1.5192674479961274e16),
     ),
     reference=[material_refs["Rakic1995"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Al/Rakic.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Al/Rakic.yml",
 )
 
 Al_RakicLorentzDrude1998 = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=(
             ((-16956600687280.727 + 0j), (3.6126085572070707e18 + 0j)),
@@ -238,15 +243,16 @@
             ((-237005721887395.88 - 2333745139453868j), 5548539400655874j),
             ((-1026265161121384.1 - 2547917843202809j), 1.6872706975652858e16j),
             ((-2569081254561451.5 - 4608729293067524j), 1685784870483934.5j),
         ),
         frequency_range=(1208994621135.9636, 4835978484543854.0),
     ),
     reference=[material_refs["Rakic1998"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Al/Rakic-LD.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Al/Rakic-LD.yml",
 )
 
 Al2O3_Horiba = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=[((-0.0 - 1j * 1.856240967961668e16), (0.0 + 1j * 1.4107431356508676e16))],
         frequency_range=(145079354536315.6, 1450793545363156.0),
@@ -271,15 +277,16 @@
         poles=[
             ((0.0 + 1j * 6674881541314847.0), (-0.0 - 1j * 2.0304989648679764e16)),
             ((0.0 + 1j * 68198825885555.74), (-0.0 - 1j * 64788884591277.95)),
         ],
         frequency_range=(136269299354975.81, 535343676037405.0),
     ),
     reference=[material_refs["FernOnton1971"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/AlAs/Fern.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/AlAs/Fern.yml",
 )
 
 AlGaN_Horiba = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=[
             ((-96473482947754.08 - 1j * 1.0968686723518324e16), (0.0 + 1j * 1.974516343551917e16))
@@ -328,15 +335,16 @@
                 (-56597670698540.76 - 8080114483410.944j),
                 (895004078070708.5 + 5.346045584373232e18j),
             ),
         ),
         frequency_range=(12025369359446.29, 999308193769986.8),
     ),
     reference=[material_refs["Olmon2012"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Au/Olmon-ev.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Au/Olmon-ev.yml",
 )
 
 Au_Olmon2012stripped = VariantItem(
     medium=PoleResidue(
         eps_inf=1.8661249761826162,
         poles=(
             (
@@ -348,15 +356,16 @@
                 (-102715947550852.86 - 10649989484.773024j),
                 (-6.333331223161453e17 + 5.199295820846523e18j),
             ),
         ),
         frequency_range=(12025369359446.29, 999308193769986.8),
     ),
     reference=[material_refs["Olmon2012"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Au/Olmon-ts.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Au/Olmon-ts.yml",
 )
 
 Au_Olmon2012crystal = VariantItem(
     medium=PoleResidue(
         eps_inf=2.093707117588658,
         poles=(
             (
@@ -371,15 +380,16 @@
                 (-112863245755655.73 - 1485493875832.8145j),
                 (-3.854564084910335e17 + 4.175729670090279e18j),
             ),
         ),
         frequency_range=(12025369359446.29, 999308193769986.8),
     ),
     reference=[material_refs["Olmon2012"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Au/Olmon-sc.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Au/Olmon-sc.yml",
 )
 
 Au_Olmon2012Drude = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=(
             (
@@ -390,15 +400,16 @@
                 (-71428570000000 + 0j),
                 (-1.153665672616558e18 - 0j),
             ),
         ),
         frequency_range=(12025369359446.29, 241798930000000),
     ),
     reference=[material_refs["Olmon2012"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Au/Olmon-sc.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Au/Olmon-sc.yml",
 )
 
 Au_JohnsonChristy1972 = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=[
             (
@@ -425,15 +436,16 @@
                 (-258129278193.38495 + 1j * 126209156799910.83),
                 (972898514880373.2 - 1j * 2.6164309961808477e17),
             ),
         ],
         frequency_range=(154751311505403.34, 1595872899899471.8),
     ),
     reference=[material_refs["JohnsonChristy1972"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Au/Johnson.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Au/Johnson.yml",
 )
 
 Au_RakicLorentzDrude1998 = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=[
             ((-1146636944.7421875 + 0j), (8.88238982652701e17 + 0j)),
@@ -443,15 +455,16 @@
             ((-660881339878315.4 - 4462028230599516j), 1497407504712811j),
             ((-1894526507651171.2 - 6258461223088549j), 9036929133946472j),
             ((-1681829064931713 - 2.0166634496554556e16j), 2.0457430700884664e16j),
         ],
         frequency_range=(4.83598623e13, 1.20898681e15),
     ),
     reference=[material_refs["Rakic1998"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Au/Rakic-LD.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Au/Rakic-LD.yml",
 )
 
 BK7_Zemax = VariantItem(
     medium=PoleResidue(
         eps_inf=1,
         poles=[
             ((0.0 + 1j * 2.431642149296798e16), (-0.0 - 1j * 1.2639823249559002e16)),
@@ -484,15 +497,16 @@
                 (-21593264136101.0 + 1j * 15791763527.314959),
                 (10898385976899.773 - 1j * 1.844312751315413e21),
             ),
         ],
         frequency_range=(4835978484543.8545, 1208994621135963.5),
     ),
     reference=[material_refs["Rakic1998"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Be/Rakic-BB.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Be/Rakic-BB.yml",
 )
 
 Be_RakicLorentzDrude1998 = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=(
             ((-1108290667017.4727 + 0j), (6.51808619662519e17 + 0j)),
@@ -503,15 +517,16 @@
             ((-4626578610293440 + 0j), (-1.351759826496727e16 - 0j)),
             ((-3383408606687375.5 - 3455109465888045.5j), 6.06548265916751e16j),
             ((-1368859970644510.8 - 6859457195810405j), 7493848504616175j),
         ),
         frequency_range=(4835978484543.8545, 1208994621135963.5),
     ),
     reference=[material_refs["Rakic1998"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Be/Rakic-LD.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Be/Rakic-LD.yml",
 )
 
 CaF2_Horiba = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=[((-0.0 - 1j * 2.376134288665943e16), (0.0 + 1j * 1.2308375615289586e16))],
         frequency_range=(181349193170394.5, 1148544890079165.2),
@@ -550,15 +565,16 @@
                 (-14969882528204.193 + 1j * 2792246309026.462),
                 (1365296575589394.2 - 1j * 3.587733271017399e18),
             ),
         ],
         frequency_range=(4835362227919.29, 1208840556979822.5),
     ),
     reference=[material_refs["Rakic1998"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Cr/Rakic-BB.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Cr/Rakic-BB.yml",
 )
 
 Cr_RakicLorentzDrude1998 = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=(
             ((-817479822341.9102 + 0j), (3.211383394563691e17 + 0j)),
@@ -569,15 +585,16 @@
             ((-1541009790006751.5 + 0j), (-1.8197032850966144e16 - 0j)),
             ((-2032779845418818.5 - 2196724138579424.2j), 6.975894511603244e16j),
             ((-1014111021537414.9 - 1.3292945008240806e16j), 8277289379024513j),
         ),
         frequency_range=(4835978484543.8545, 1208994621135963.5),
     ),
     reference=[material_refs["Rakic1998"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Cr/Rakic-LD.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Cr/Rakic-LD.yml",
 )
 
 Cu_JohnsonChristy1972 = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0717963962915042,
         poles=(
             (
@@ -597,15 +614,16 @@
                 (-1518719353508992.2 + 4.4544685629246894e18j),
             ),
             ((-1292418447472384 - 3584018186373431j), (2786681303341121.5 + 2.134483285446143e16j)),
         ),
         frequency_range=(154771532266391.3, 1595489398616285.2),
     ),
     reference=[material_refs["JohnsonChristy1972"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Cu/Johnson.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Cu/Johnson.yml",
 )
 
 Cu_RakicLorentzDrude1998 = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=(
             ((-506299046.578125 + 0j), (1.7077228480506522e18 + 0j)),
@@ -614,76 +632,82 @@
             ((-802173212541955.2 - 4420275938629775j), 3184779293720060j),
             ((-2440703155205778.5 - 7673302022556904j), 1.275414610754998e16j),
             ((-3270223181811664 - 1.6667627171842064e16j), 5181342297925362j),
         ),
         frequency_range=(2.41768111e13, 1.44827274e15),
     ),
     reference=[material_refs["Rakic1998"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Cu/Rakic-LD.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Cu/Rakic-LD.yml",
 )
 
 FusedSilica_Zemax = VariantItem(
     medium=PoleResidue(
         eps_inf=1,
         poles=[
             ((0.0 + 1j * 2.7537034527932452e16), (-0.0 - 1j * 9585177720141492.0)),
             ((0.0 + 1j * 1.620465316968868e16), (-0.0 - 1j * 3305284173070520.5)),
             ((0.0 + 1j * 190341645710801.38), (-0.0 - 1j * 85413852993771.3)),
         ],
         frequency_range=(44745143071783.1, 1427583136099746.8),
     ),
     reference=[material_refs["Malitson1965"], material_refs["Tan1998"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/SiO2/Malitson.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/SiO2/Malitson.yml",
 )
 
 FusedSilica_Zemax_Visible_PMLStable = VariantItem(
     medium=PoleResidue(
         eps_inf=1,
         poles=((-2.0054061849947e16j, 1.1008717135056432e16j),),
         frequency_range=(382925607524582.94, 739315556426623.9),
     ),
     reference=[material_refs["Malitson1965"], material_refs["Tan1998"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/SiO2/Malitson.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/SiO2/Malitson.yml",
 )
 
 FusedSilica_Zemax_PMLStable = VariantItem(
     medium=PoleResidue(
         eps_inf=1,
         poles=((-1.7312422399228024e16j, 9389865424501702j),),
         frequency_range=(150347270878132.4, 739315556426623.9),
     ),
     reference=[material_refs["Malitson1965"], material_refs["Tan1998"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/SiO2/Malitson.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/SiO2/Malitson.yml",
 )
 
 GaAs_Skauli2003 = VariantItem(
     medium=PoleResidue(
         eps_inf=5.372514,
         poles=[
             ((0.0 + 1j * 4250781024557878.5), (-0.0 - 1j * 1.1618961579876792e16)),
             ((0.0 + 1j * 2153617667595138.0), (-0.0 - 1j * 26166023937747.41)),
             ((0.0 + 1j * 51024513930292.87), (-0.0 - 1j * 49940804278927.375)),
         ],
         frequency_range=(17634850504761.58, 309064390289635.9),
     ),
     reference=[material_refs["Skauli2003"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/GaAs/Skauli.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/GaAs/Skauli.yml",
 )
 
 Ge_Icenogle1976 = VariantItem(
     medium=PoleResidue(
         eps_inf=1,
         poles=[
             ((0.0 + 1j * 2836329349380603.5), (-0.0 - 1j * 9542546463056102.0)),
             ((0.0 + 1j * 30278857121656.766), (-0.0 - 1j * 3225758043455.7036)),
         ],
         frequency_range=(24982704881745.566, 119916983432378.72),
     ),
     reference=[material_refs["Icenogle1976"], material_refs["Barnes1979"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Ge/Icenogle.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Ge/Icenogle.yml",
 )
 
 GeOx_Horiba = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=[
             ((-351710414211103.44 - 1j * 2.4646085673376252e16), (0.0 + 1j * 2.02755336442934e16))
@@ -745,15 +769,16 @@
         frequency_range=(29979245858094.68, 315571009032575.6),
     ),
     reference=[
         material_refs["Pettit1965"],
         material_refs["Pikhtin1978"],
         material_refs["HandbookOptics"],
     ],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/InP/Pettit.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/InP/Pettit.yml",
 )
 
 MgF2_Horiba = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=[((-0.0 - 1j * 2.5358092974503356e16), (0.0 + 1j * 1.1398462792039258e16))],
         frequency_range=(193439139381754.16, 918835912063332.1),
@@ -777,15 +802,16 @@
                 (-982824644.4296285 - 1j * 4252237346494.8228),
                 (338287950556.00256 + 1j * 4386571425642974.0),
             ),
         ],
         frequency_range=(55517121959434.59, 832756829391519.0),
     ),
     reference=[material_refs["StephensMalitson1952"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/MgO/Stephens.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/MgO/Stephens.yml",
 )
 
 MoS2_Li2014 = VariantItem2D(
     medium=Medium2D.from_dispersive_medium(
         PoleResidue(
             eps_inf=7,
             poles=(
@@ -839,15 +865,16 @@
                 (-3956384974540.076 - 12646403210723.701j),
                 (8260543758347535 + 3.3147262955373885e18j),
             ),
         ),
         frequency_range=(154771532266391.3, 1594640734042553.2),
     ),
     reference=[material_refs["JohnsonChristy1972"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Ni/Johnson.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Ni/Johnson.yml",
 )
 
 Ni_RakicLorentzDrude1998 = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=(
             ((-800062663506.125 + 0j), (3.936912856387643e17 + 0j)),
@@ -858,15 +885,16 @@
             ((-1508373859996014.5 + 0j), (-3.988443595266845e16 - 0j)),
             ((-1654482250867782.5 - 1774676068987181.8j), 1.7470742743872056e16j),
             ((-4779615391395816 - 7920412739409055j), 2.6921813490544444e16j),
         ),
         frequency_range=(48359784845438.55, 1208994621135963.5),
     ),
     reference=[material_refs["Rakic1998"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Ni/Rakic-LD.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Ni/Rakic-LD.yml",
 )
 
 PEI_Horiba = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=[((-0.0 - 1j * 1.8231209375953524e16), (0.0 + 1j * 9936009109894670.0))],
         frequency_range=(181349193170394.5, 1148544890079165.2),
@@ -950,15 +978,16 @@
                 (-1.0165311890218712e16 - 1j * 6195195244753680.0),
                 (-8682197716799510.0 - 1j * 2496615613677907.5),
             ),
         ],
         frequency_range=(154751311505403.34, 1595872899899471.8),
     ),
     reference=[material_refs["JohnsonChristy1972"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Pd/Johnson.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Pd/Johnson.yml",
 )
 
 Pd_RakicLorentzDrude1998 = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=(
             ((-6077069791984.51 - 4557802343988.38j), 7.894587671231656e18j),
@@ -968,15 +997,16 @@
             ((-1067065603800966.5 + 0j), (1.4236470639056928e16 + 0j)),
             ((-5953469273389138 + 0j), (-1.4236470639056928e16 - 0j)),
             ((-2458174730857734 - 8327373750489667j), 5931453695969745j),
         ),
         frequency_range=(24179892422719.273, 1208994621135963.5),
     ),
     reference=[material_refs["Rakic1998"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Pd/Rakic-LD.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Pd/Rakic-LD.yml",
 )
 
 Polycarbonate_Horiba = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=[((-0.0 - 1j * 1.8240324980641504e16), (0.0 + 1j * 1.3716724385442412e16))],
         frequency_range=(362698386340789.0, 967195696908770.8),
@@ -1030,15 +1060,16 @@
                 (-9967323231923196.0 - 1j * 4041974141709040.5),
                 (-501748269346742.7 + 1j * 6.883385112306915e16),
             ),
         ],
         frequency_range=(120884055879414.03, 2997924585809468.0),
     ),
     reference=[material_refs["Werner2009"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Pt/Werner.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Pt/Werner.yml",
 )
 
 Pt_RakicLorentzDrude1998 = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=(
             ((-476640283942.46875 + 0j), (2.9309972445197843e17 + 0j)),
@@ -1047,15 +1078,16 @@
             ((-1396206784708441 - 1426846131279794.5j), 4.9021202075413656e16j),
             ((-2786336499624897.5 - 3874079860313212j), 1.498630066235504e16j),
             ((-6469800427291508 - 1.2473655652689588e16j), 3.042842289267071e16j),
         ),
         frequency_range=(24179892422719.273, 1208994621135963.5),
     ),
     reference=[material_refs["Rakic1998"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Pt/Rakic-LD.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Pt/Rakic-LD.yml",
 )
 
 Sapphire_Horiba = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=[((-0.0 - 1j * 2.0143967092980652e16), (0.0 + 1j * 2.105044561216478e16))],
         frequency_range=(362698386340789.0, 1329894083249559.8),
@@ -1080,35 +1112,38 @@
         poles=[
             ((0.0 + 1j * 1.391786035350109e16), (-0.0 - 1j * 2.1050067891652724e16)),
             ((0.0 + 1j * 1519267431623.5857), (-0.0 - 1j * 3.0623873619236616e16)),
         ],
         frequency_range=(54468106573573.19, 967072447035312.2),
     ),
     reference=[material_refs["Luke2015"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Si3N4/Luke.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Si3N4/Luke.yml",
 )
 
 Si3N4_Luke2015_PMLStable = VariantItem(
     medium=PoleResidue(
         eps_inf=3.031225983820944,
         poles=((-7534484687295489j, 3530332266482328j), (-4550924050946271j, 7233481618.869821j)),
         frequency_range=(152024573088740.38, 724311326723836.8),
     ),
     reference=[material_refs["Luke2015"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Si3N4/Luke.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Si3N4/Luke.yml",
 )
 
 Si3N4_Philipp1973 = VariantItem(
     medium=PoleResidue(
         eps_inf=1,
         poles=[((0.0 + 1j * 1.348644355236665e16), (-0.0 - 1j * 1.9514209498096924e16))],
         frequency_range=(241768111758828.06, 1448272746767859.0),
     ),
     reference=[material_refs["Philipp1973"], material_refs["Baak1982"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Si3N4/Philipp.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Si3N4/Philipp.yml",
 )
 
 SiC_Horiba = VariantItem(
     medium=PoleResidue(
         eps_inf=3.0,
         poles=[((-0.0 - 1j * 1.2154139583969018e16), (0.0 + 1j * 2.3092865209541132e16))],
         frequency_range=(145079354536315.6, 967195696908770.8),
@@ -1165,15 +1200,16 @@
             ((-2919746613155850.5 - 1j * 7.211858151732786e16), (0.0 + 1j * 744301222539582.0)),
             ((-4635394958195360.0 - 1j * 5.622429893839941e16), (0.0 + 1j * 2101343798471838.0)),
             ((-9774364062177540.0 - 1j * 4844300045008988.0), (0.0 + 1j * 7.377824793744533e16)),
         ],
         frequency_range=(120884055879414.03, 2997924585809468.0),
     ),
     reference=[material_refs["Werner2009"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Ti/Werner.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Ti/Werner.yml",
 )
 
 Ti_RakicLorentzDrude1998 = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=(
             ((-464807447764.2969 + 0j), (7.341080927693171e16 + 0j)),
@@ -1183,15 +1219,16 @@
             ((-1912757717027124.2 - 1360524146154420.5j), 1.7716577274303782e16j),
             ((-1263270883008780 - 3596426881658456.5j), 3189068866500566j),
             ((-1338474621684588.2 - 2.9489006173628724e16j), 2079856587113.8086j),
         ),
         frequency_range=(9.67072446e12, 1.20884056e15),
     ),
     reference=[material_refs["Rakic1998"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Ti/Rakic-LD.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Ti/Rakic-LD.yml",
 )
 
 TiOx_Horiba = VariantItem(
     medium=PoleResidue(
         eps_inf=0.29,
         poles=[((-0.0 - 1j * 9875238411974826.0), (0.0 + 1j * 1.7429795797135566e16))],
         frequency_range=(145079354536315.6, 725396772681578.0),
@@ -1235,15 +1272,16 @@
                 (-3989296857299139.0 - 1j * 3986090497375137.0),
                 (-352374832782093.06 + 1j * 6.323677441887342e16),
             ),
         ],
         frequency_range=(120884055879414.03, 2997924585809468.0),
     ),
     reference=[material_refs["Werner2009"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/W/Werner.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/W/Werner.yml",
 )
 
 W_RakicLorentzDrude1998 = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=(
             ((-596977842693.5781 + 0j), (4.3263359766348934e17 + 0j)),
@@ -1252,15 +1290,16 @@
             ((-973090800441519.6 - 2745063931489722j), 1.219711179953004e16j),
             ((-2531099568361548 - 4814146946972908j), 2.9579221430831028e16j),
             ((-4433222413252700 - 1.0493429699239636e16j), 4.978330061510859e16j),
         ),
         frequency_range=(2.41768111e13, 1.20884056e15),
     ),
     reference=[material_refs["Rakic1998"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/W/Rakic-LD.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/W/Rakic-LD.yml",
 )
 
 WS2_Li2014 = VariantItem2D(
     medium=Medium2D.from_dispersive_medium(
         PoleResidue(
             eps_inf=6.18,
             poles=(
@@ -1309,28 +1348,30 @@
         poles=[
             ((0.0 + 1j * 1.3580761146063806e16), (-0.0 - 1j * 1.7505601117276244e16)),
             ((0.0 + 1j * 82126420080181.8), (-0.0 - 1j * 161583731507757.7)),
         ],
         frequency_range=(31228381102181.96, 1199169834323787.2),
     ),
     reference=[material_refs["Nigara1968"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Y2O3/Nigara.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Y2O3/Nigara.yml",
 )
 
 YAG_Zelmon1998 = VariantItem(
     medium=PoleResidue(
         eps_inf=1,
         poles=[
             ((0.0 + 1j * 1.7303796419562446e16), (-0.0 - 1j * 1.974363171472075e16)),
             ((0.0 + 1j * 112024123195387.16), (-0.0 - 1j * 183520159101147.16)),
         ],
         frequency_range=(59958491716189.36, 749481146452367.0),
     ),
     reference=[material_refs["Zelmon1998"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Y3Al5O12/Zelmon.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Y3Al5O12/Zelmon.yml",
 )
 
 ZrO2_Horiba = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=[
             ((-97233116671752.14 - 1j * 1.446765717253359e16), (0.0 + 1j * 2.0465425413547396e16))
@@ -1354,25 +1395,27 @@
 cSi_SalzbergVilla1957 = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=[((0.0 + 1j * 6206417594288582.0), (-0.0 - 1j * 3.311074436985222e16))],
         frequency_range=(27253859870995.164, 220435631309519.7),
     ),
     reference=[material_refs["SalzbergVilla1957"], material_refs["Tatian1984"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Si/Salzberg.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Si/Salzberg.yml",
 )
 
 cSi_Li1993_293K = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=[((0.0 + 1j * 6241549589084091.0), (0.0 - 1j * 3.3254308736142404e16))],
         frequency_range=(21413747041496.2, 249827048817455.7),
     ),
     reference=[material_refs["Li1993_293K"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Si/Li-293K.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Si/Li-293K.yml",
 )
 
 cSi_Green2008 = VariantItem(
     medium=PoleResidue(
         eps_inf=1.0,
         poles=[
             (
@@ -1391,15 +1434,16 @@
                 (-379444981070553.4 + 1j * 5656363945615038.0),
                 (1105733518717537.1 - 1j * 8204725853411607.0),
             ),
         ],
         frequency_range=(206753419710997.8, 1199169834323787.2),
     ),
     reference=[material_refs["Green2008"]],
-    data_url="https://refractiveindex.info/data_csv.php?datafile=data/main/Si/Green-2008.yml",
+    data_url="https://refractiveindex.info/data_csv.php?datafile=database/data-nk/"
+    "main/Si/Green-2008.yml",
 )
 
 
 material_library = dict(
     Ag=MaterialItem(
         name="Silver",
         variants=dict(
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/material_library/material_reference.py` & `tidy3d-2.3.1/tidy3d/material_library/material_reference.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/material_library/parametric_materials.py` & `tidy3d-2.3.1/tidy3d/material_library/parametric_materials.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 """Parametric material models."""
 from abc import ABC, abstractmethod
 from typing import List, Tuple
+import warnings
 import pydantic as pd
 import numpy as np
 
 from ..components.medium import PoleResidue, Medium2D, Drude
 from ..components.base import Tidy3dBaseModel
 from ..constants import EPSILON_0, Q_e, HBAR, K_B, ELECTRON_VOLT, KELVIN
+from ..log import log
 
 try:
     from scipy import integrate
 
     INTEGRATE_AVAILABLE = True
 except ImportError:
     INTEGRATE_AVAILABLE = False
 
-
 # default values of the physical parameters for graphene
 # scattering rate in eV
 GRAPHENE_DEF_GAMMA = 0.00041
 # chemical potential in eV
 GRAPHENE_DEF_MU_C = 0
 # temperature in K
 GRAPHENE_DEF_TEMP = 300
 
 # constants controlling the numerical integration of the interband term in graphene
 # frequency limits of integration
-GRAPHENE_INT_MIN = 0
+GRAPHENE_INT_MIN = 1e10
 GRAPHENE_INT_MAX = 1e16
 # integration absolute tolerance
 GRAPHENE_INT_TOL = 1e-20
 
 # constants controlling the Pade approximation of the interband term in graphene
 # frequency range for fitting
 GRAPHENE_FIT_FREQ_MIN = 1e12
 GRAPHENE_FIT_FREQ_MAX = 1e15
-# the fitting for the interband feature has this width relative to the absorption threshold
-GRAPHENE_FIT_REL_WIDTH = 1.1
+GRAPHENE_FIT_NUM_FREQS = 100
+GRAPHENE_FIT_ATOL = 2e-5
+# parameters controlling node placement
+GRAPHENE_FIT_LARGE_MULTIPLIER = 10
+GRAPHENE_FIT_SMALL_MULTIPLIER = 0.25
 # number of optimization iterations for fitting
 GRAPHENE_FIT_NUM_ITERS = 100
 
 
 class ParametricVariantItem2D(ABC, Tidy3dBaseModel):
     """A variant of a 2D material depending on parameters, that must be initialized in order to
     generate the material model."""
@@ -112,37 +116,28 @@
         GRAPHENE_FIT_NUM_ITERS,
         title="Interband fitting number of iterations",
         description="Number of iterations for optimizing each Pade approximant when "
         "fitting the interband term. Making this larger might give a better fit "
         "at the cost of decreased stability in the fitting algorithm.",
     )
 
-    @pd.validator("interband_fit_freq_nodes", always=True)
-    def _calculate_freq_nodes(cls, val, values):
-        """Calculate the default frequency nodes if none are provided."""
-        if val is None:
-            mu_c = values["mu_c"] / (2 * np.pi * HBAR)
-            temp = values["temp"] * K_B / (2 * np.pi * HBAR)
-            center = max(np.sqrt(abs(mu_c**2 - temp**2)), GRAPHENE_FIT_FREQ_MIN * 1e-5)
-            return [
-                (GRAPHENE_FIT_FREQ_MIN, GRAPHENE_FIT_FREQ_MAX),
-                (2 * center, 2 * (center + temp) * GRAPHENE_FIT_REL_WIDTH),
-            ]
-        return val
-
     @property
     def medium(self) -> Medium2D:
         """Surface conductivity model for graphene."""
         intraband = self.intraband_drude
         if self.include_interband:
             interband = self.interband_pole_residue
             intraband_poles = intraband.pole_residue.poles
             interband_poles = interband.pole_residue.poles
             poles = intraband_poles + interband_poles
-            pole_residue = self._filter_poles(PoleResidue(poles=poles))
+            pole_residue = self._filter_poles(
+                PoleResidue(
+                    poles=poles, frequency_range=(GRAPHENE_FIT_FREQ_MIN, GRAPHENE_FIT_FREQ_MAX)
+                )
+            )
             return Medium2D(ss=pole_residue, tt=pole_residue)
         return Medium2D(ss=intraband, tt=intraband)
 
     @property
     def intraband_drude(self) -> Drude:
         """A Drude-type model for the intraband term of graphene.
 
@@ -166,22 +161,46 @@
         include the intraband term, which is added in separately.
 
         Returns
         -------
         :class:`.PoleResidue`
             A pole-residue model for the interband term of graphene.
         """
-
+        mu_c = self.mu_c / (2 * np.pi * HBAR)
+        temp = self.temp * K_B / (2 * np.pi * HBAR)
+        resonance = max(np.sqrt(abs(mu_c**2 - temp**2)), GRAPHENE_FIT_FREQ_MIN * 1e-5)
+        freqs = np.linspace(
+            resonance / GRAPHENE_FIT_LARGE_MULTIPLIER,
+            resonance * GRAPHENE_FIT_LARGE_MULTIPLIER,
+            GRAPHENE_FIT_NUM_FREQS,
+        )
+        sigma = self.interband_conductivity(freqs)
         nodes = self.interband_fit_freq_nodes
+        if nodes is None:
+            fcenter = freqs[np.argmin(np.imag(sigma))]
+            fwidth = (
+                fcenter - freqs[np.nonzero(np.imag(sigma) < 0.5 * np.amin(np.imag(sigma)))[0][0]]
+            )
+            nodes = [
+                (fcenter / GRAPHENE_FIT_LARGE_MULTIPLIER, fcenter * GRAPHENE_FIT_LARGE_MULTIPLIER),
+                (fcenter, fcenter + fwidth * GRAPHENE_FIT_SMALL_MULTIPLIER),
+            ]
+
         flattened_freqs = [freq for pair in nodes for freq in pair]
-        sigma = self.interband_conductivity(flattened_freqs)
+        sigma_inds = self.interband_conductivity(flattened_freqs)
         inds = [(2 * i, 2 * i + 1) for i in range(len(nodes))]
 
-        pole_residue = self._fit_interband_conductivity(flattened_freqs, sigma, inds)
-        return self._filter_poles(pole_residue)
+        pole_residue = self._fit_interband_conductivity(flattened_freqs, sigma_inds, inds)
+        pole_residue_filtered = self._filter_poles(pole_residue)
+        sigma_fit = pole_residue_filtered.sigma_model(freqs)
+        if not np.allclose(sigma, sigma_fit, rtol=0, atol=GRAPHENE_FIT_ATOL):
+            log.warning(
+                "Graphene fit may not be good. Try changing the physical or fitting parameters."
+            )
+        return pole_residue_filtered
 
     def numerical_conductivity(self, freqs: List[float]) -> List[complex]:
         """Numerically calculate the conductivity. If this differs from the
         conductivity of the :class:`.Medium2D`, it is due to error while
         fitting the interband term, and you may try values of ``interband_fit_freq_nodes``
         different from its default (calculated) value.
 
@@ -211,15 +230,18 @@
         -------
         List[complex]
             The list of corresponding interband conductivities, in S.
         """
 
         def fermi(E: float) -> float:
             """Fermi distribution."""
-            return 1 / (np.exp((E - self.mu_c) / (K_B * self.temp)) + 1)
+            # catch overflow warning
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")
+                return 1 / (np.exp((E - self.mu_c) / (K_B * self.temp)) + 1)
 
         def fermi_g(E: float) -> float:
             """Difference of fermi distributions."""
             return fermi(-E) - fermi(E)
 
         def integrand(E: float, omega: float) -> float:
             """Integrand for interband term."""
@@ -336,15 +358,23 @@
 
                 if disc > 0:
                     for (root, res) in zip([root1, root2], [res1, res2]):
                         poles.append((root, res / 2))
                 else:
                     poles.append((root1, res1))
 
-            return PoleResidue(poles=poles)
+            flipped_poles = []
+            for (a, c) in poles:
+                if np.real(a) > 0:
+                    flipped_poles += [(-1j * np.conj(1j * a), c)]
+                else:
+                    flipped_poles += [(a, c)]
+            return PoleResidue(
+                poles=flipped_poles, frequency_range=(GRAPHENE_FIT_FREQ_MIN, GRAPHENE_FIT_FREQ_MAX)
+            )
 
         # fitting works better with normalized quantities (THz and uS)
         omega_thz = 2 * np.pi * np.array(freqs) * 1e-12
         sigma_us = np.array(sigma) * 1e6
         coeffslist = []
         for inds in indslist:
             res = np.array(sigma_us) - evaluate_coeffslist(omega_thz, coeffslist)
@@ -352,31 +382,26 @@
 
         coeffslist = optimize(omega_thz, sigma_us, indslist, coeffslist)
 
         pole_res = get_pole_residue(coeffslist)
         # unnormalize, and convert from conductivity to permittivity
         poles = [(a * 1e12, -c / (a * EPSILON_0 * 1e6)) for (a, c) in pole_res.poles]
 
-        flipped_poles = []
-        for (a, c) in poles:
-            if np.real(a) > 0:
-                flipped_poles += [(-1j * np.conj(1j * a), c)]
-            else:
-                flipped_poles += [(a, c)]
-
-        # residue at omega = 0
-        zero_res = -np.sum([c for (_, c) in flipped_poles])
-
-        return PoleResidue(poles=flipped_poles + [(0, zero_res)])
+        return PoleResidue(
+            poles=poles, frequency_range=(GRAPHENE_FIT_FREQ_MIN, GRAPHENE_FIT_FREQ_MAX)
+        )
 
     def _filter_poles(self, medium: PoleResidue) -> PoleResidue:
         """Clean up poles, merging poles at zero frequency."""
         zero_res = 0
         poles = []
         for (a, c) in medium.poles:
             if a == 0:
                 zero_res += c
             elif abs(a) > 1e17:
                 continue
             else:
                 poles += [(a, c)]
-        return PoleResidue(poles=poles + [(0, zero_res)])
+        return PoleResidue(
+            poles=poles + [(0, zero_res)],
+            frequency_range=(GRAPHENE_FIT_FREQ_MIN, GRAPHENE_FIT_FREQ_MAX),
+        )
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/__init__.py` & `tidy3d-2.3.1/tidy3d/plugins/adjoint/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Imports for adjoint plugin."""
 
 # import the jax version of tidy3d components
 try:
-    from .components.geometry import JaxBox, JaxPolySlab
+    from .components.geometry import JaxBox, JaxPolySlab, JaxGeometryGroup
     from .components.medium import JaxMedium, JaxAnisotropicMedium, JaxCustomMedium
     from .components.structure import JaxStructure
     from .components.simulation import JaxSimulation
     from .components.data.sim_data import JaxSimulationData
     from .components.data.monitor_data import JaxModeData
     from .components.data.dataset import JaxPermittivityDataset
     from .components.data.data_array import JaxDataArray
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/base.py` & `tidy3d-2.3.1/tidy3d/plugins/adjoint/components/base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/data/dataset.py` & `tidy3d-2.3.1/tidy3d/plugins/adjoint/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/data/sim_data.py` & `tidy3d-2.3.1/tidy3d/plugins/adjoint/components/data/sim_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,17 +110,26 @@
         # construct JaxSimulationData with no data (yet)
         self_dict["simulation"] = jax_sim
         self_dict["data"] = ()
 
         data_dict = cls.split_data(mnt_data=sim_data.data, jax_info=jax_info)
 
         # convert the output data to the proper jax type
-        data_dict["output_data"] = [
-            JAX_MONITOR_DATA_MAP[type(x)].from_monitor_data(x) for x in data_dict["output_data"]
-        ]
+        output_data_list = []
+        for mnt_data in data_dict["output_data"]:
+            mnt_data_type_str = type(mnt_data)
+            if mnt_data_type_str not in JAX_MONITOR_DATA_MAP:
+                raise KeyError(
+                    f"MonitorData type '{mnt_data_type_str}' "
+                    "not currently supported by adjoint plugin."
+                )
+            mnt_data_type = JAX_MONITOR_DATA_MAP[mnt_data_type_str]
+            jax_mnt_data = mnt_data_type.from_monitor_data(mnt_data)
+            output_data_list.append(jax_mnt_data)
+            data_dict["output_data"] = output_data_list
 
         self_dict.update(data_dict)
         self_dict.update(dict(task_id=task_id))
 
         return cls.parse_obj(self_dict)
 
     @classmethod
@@ -162,10 +171,11 @@
                 adj_srcs.append(adj_source)
 
         update_dict = dict(boundary_spec=bc_adj, sources=adj_srcs, monitors=(), output_monitors=())
         update_dict.update(
             self.simulation.get_grad_monitors(
                 input_structures=self.simulation.input_structures,
                 freq_adjoint=self.simulation.freq_adjoint,
+                include_eps_mnts=False,
             )
         )
         return self.simulation.updated_copy(**update_dict)
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/geometry.py` & `tidy3d-2.3.1/tidy3d/plugins/adjoint/components/geometry.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # pylint: disable=invalid-name
 """Defines jax-compatible geometries and their conversion to grad monitors."""
 from __future__ import annotations
 
-import os
 from abc import ABC
 from typing import Tuple, Union, Dict
 from multiprocessing import Pool
 
 import pydantic as pd
 import numpy as np
 import xarray as xr
 import jax.numpy as jnp
 from jax.tree_util import register_pytree_node_class
 import jax
 
 from ....components.base import cached_property
-from ....components.types import Bound, Coordinate2D
-from ....components.geometry import Geometry, Box, PolySlab
+from ....components.types import Bound, Coordinate2D  # , annotate_type
+from ....components.geometry import Geometry, Box, PolySlab, GeometryGroup
 from ....components.data.monitor_data import FieldData, PermittivityData
 from ....components.data.data_array import ScalarFieldDataArray
 from ....components.monitor import FieldMonitor, PermittivityMonitor
 from ....constants import fp_eps, MICROMETER
 from ....exceptions import AdjointError
 
 from .base import JaxObject
@@ -157,14 +156,15 @@
         grad_data_fwd: FieldData,
         grad_data_adj: FieldData,
         grad_data_eps: PermittivityData,
         sim_bounds: Bound,
         wvl_mat: float,
         eps_out: complex,
         eps_in: complex,
+        num_proc: int = 1,
     ) -> JaxBox:
         """Stores the gradient of the box parameters given forward and adjoint field data."""
 
         # multiply the E and D field components together for fwd and adj
         e_mult_xyz, d_mult_xyz = self.compute_dotted_e_d_fields(
             grad_data_fwd=grad_data_fwd, grad_data_adj=grad_data_adj, grad_data_eps=grad_data_eps
         )
@@ -544,43 +544,198 @@
         grad_data_fwd: FieldData,
         grad_data_adj: FieldData,
         grad_data_eps: PermittivityData,
         sim_bounds: Bound,
         wvl_mat: float,
         eps_out: complex,
         eps_in: complex,
+        num_proc: int = 1,
     ) -> JaxPolySlab:
         """Stores the gradient of the vertices given forward and adjoint field data."""
 
         # multiply the E and D field components together for fwd and adj
         e_mult_xyz, d_mult_xyz = self.compute_dotted_e_d_fields(
             grad_data_fwd=grad_data_fwd, grad_data_adj=grad_data_adj, grad_data_eps=grad_data_eps
         )
 
-        # Construct arguments to pass to the parallel vertices_vjp computation
+        if num_proc is not None and num_proc > 1:
+            return self.store_vjp_parallel(
+                e_mult_xyz=e_mult_xyz,
+                d_mult_xyz=d_mult_xyz,
+                sim_bounds=sim_bounds,
+                wvl_mat=wvl_mat,
+                eps_out=eps_out,
+                eps_in=eps_in,
+                num_proc=num_proc,
+            )
+
+        return self.store_vjp_sequential(
+            e_mult_xyz=e_mult_xyz,
+            d_mult_xyz=d_mult_xyz,
+            sim_bounds=sim_bounds,
+            wvl_mat=wvl_mat,
+            eps_out=eps_out,
+            eps_in=eps_in,
+        )
+
+    def _make_vertex_args(
+        self,
+        e_mult_xyz: FieldData,
+        d_mult_xyz: FieldData,
+        sim_bounds: Bound,
+        wvl_mat: float,
+        eps_out: complex,
+        eps_in: complex,
+    ) -> tuple:
+        """Generate arguments for `vertex_vjp`."""
+
         num_verts = len(self.vertices)
         args = [range(num_verts)]
+
         # append all of the arguments that are the same for each call
         constant_args = [e_mult_xyz, d_mult_xyz, sim_bounds, wvl_mat, eps_out, eps_in]
         args += [[arg] * num_verts for arg in constant_args]
+        return args
+
+    def store_vjp_sequential(
+        self,
+        e_mult_xyz: FieldData,
+        d_mult_xyz: FieldData,
+        sim_bounds: Bound,
+        wvl_mat: float,
+        eps_out: complex,
+        eps_in: complex,
+    ) -> JaxPolySlab:
+        """Stores the gradient of the vertices given forward and adjoint field data."""
+        # Construct arguments to pass to the parallel vertices_vjp computation
 
-        try:
-            # Try to use multiprocessing over polygon vertices.
-            # Use only half of the available cpus in case there is something else running.
-            num_proc = max(1, os.cpu_count() // 2)
-            with Pool(num_proc) as p:
-                vertices_vjp = p.starmap(self.vertex_vjp, zip(*args))
-        except Exception:  # pylint:disable=broad-except
-            # Compute without parallel pool
-            vertices_vjp = list(map(self.vertex_vjp, *args))
+        args = self._make_vertex_args(e_mult_xyz, d_mult_xyz, sim_bounds, wvl_mat, eps_out, eps_in)
+        vertices_vjp = list(map(self.vertex_vjp, *args))
+        return self.copy(update=dict(vertices=vertices_vjp))
+
+    def store_vjp_parallel(
+        self,
+        e_mult_xyz: FieldData,
+        d_mult_xyz: FieldData,
+        sim_bounds: Bound,
+        wvl_mat: float,
+        eps_out: complex,
+        eps_in: complex,
+        num_proc: int = 1,
+    ) -> JaxPolySlab:
+        """Stores the gradient of the vertices given forward and adjoint field data."""
 
-        # return copy of the polyslab with the vertices storing the
+        args = self._make_vertex_args(e_mult_xyz, d_mult_xyz, sim_bounds, wvl_mat, eps_out, eps_in)
+        with Pool(num_proc) as pool:
+            vertices_vjp = pool.starmap(self.vertex_vjp, zip(*args))
         return self.copy(update=dict(vertices=vertices_vjp))
 
 
-JaxGeometryType = Union[JaxBox, JaxPolySlab]
+JaxSingleGeometryType = Union[JaxBox, JaxPolySlab]
+
+
+@register_pytree_node_class
+class JaxGeometryGroup(JaxGeometry, GeometryGroup, JaxObject):
+    """A collection of Geometry objects that can be called as a single geometry object."""
+
+    geometries: Tuple[JaxPolySlab, ...] = pd.Field(
+        ...,
+        title="Geometries",
+        description="Tuple of jax geometries in a single grouping. "
+        "Can provide significant performance enhancement in ``JaxStructure`` when all geometries "
+        "are assigned the same ``JaxMedium``. Note: at this moment, only ``JaxPolySlab`` "
+        "is supported.",
+        jax_field=True,
+    )
+
+    def to_tidy3d(self) -> GeometryGroup:
+        """Convert :class:`.JaxGeometryGroup` instance to :class:`.GeometryGroup`"""
+        self_dict = self.dict(exclude={"type"})
+        self_dict["geometries"] = [geo.to_tidy3d() for geo in self.geometries]
+        map_reverse = {v: k for k, v in JAX_GEOMETRY_MAP.items()}
+        tidy3d_type = map_reverse[type(self)]
+        return tidy3d_type.parse_obj(self_dict)
+
+    @classmethod
+    def from_tidy3d(cls, tidy3d_obj: GeometryGroup) -> JaxGeometryGroup:
+        """Convert :class:`.GeometryGroup` instance to :class:`.GeometryGroup`"""
+        obj_dict = tidy3d_obj.dict(exclude={"type"})
+        jax_geometries = []
+
+        tidy3d_type_map = {k.__name__: k for k, v in JAX_GEOMETRY_MAP.items()}
+        jax_type_map = {k.__name__: v for k, v in JAX_GEOMETRY_MAP.items()}
+
+        for geo in obj_dict["geometries"]:
+            type_str = geo["type"]
+            tidy3d_type = tidy3d_type_map[type_str]
+            jax_type = jax_type_map[type_str]
+            geo_tidy3d = tidy3d_type.parse_obj(geo)
+            geo_jax = jax_type.from_tidy3d(geo_tidy3d)
+            jax_geometries.append(geo_jax)
+        obj_dict["geometries"] = jax_geometries
+        return cls.parse_obj(obj_dict)
+
+    # pylint: disable=too-many-arguments
+    @staticmethod
+    def _store_vjp_geometry(
+        geometry: JaxSingleGeometryType,
+        grad_data_fwd: FieldData,
+        grad_data_adj: FieldData,
+        grad_data_eps: PermittivityData,
+        sim_bounds: Bound,
+        wvl_mat: float,
+        eps_out: complex,
+        eps_in: complex,
+    ) -> JaxSingleGeometryType:
+        """Function to store a single vjp for a single geometry."""
+        return geometry.store_vjp(
+            grad_data_fwd=grad_data_fwd,
+            grad_data_adj=grad_data_adj,
+            grad_data_eps=grad_data_eps,
+            sim_bounds=sim_bounds,
+            wvl_mat=wvl_mat,
+            eps_out=eps_out,
+            eps_in=eps_in,
+        )
+
+    # pylint: disable=too-many-arguments
+    def store_vjp(
+        self,
+        grad_data_fwd: FieldData,
+        grad_data_adj: FieldData,
+        grad_data_eps: PermittivityData,
+        sim_bounds: Bound,
+        wvl_mat: float,
+        eps_out: complex,
+        eps_in: complex,
+        num_proc: int = 1,
+    ) -> JaxGeometryGroup:
+        """Returns a `JaxGeometryGroup` where the `.geometries` store the gradient info."""
+
+        map_args = (
+            self.geometries,
+            [grad_data_fwd] * len(self.geometries),
+            [grad_data_adj] * len(self.geometries),
+            [grad_data_eps] * len(self.geometries),
+            [sim_bounds] * len(self.geometries),
+            [wvl_mat] * len(self.geometries),
+            [eps_out] * len(self.geometries),
+            [eps_in] * len(self.geometries),
+        )
+
+        if num_proc == 1:
+            geometries_vjp = tuple(map(self._store_vjp_geometry, *map_args))
+        else:
+            with Pool(num_proc) as pool:
+                geometries_vjp = tuple(pool.starmap(self._store_vjp_geometry, zip(*map_args)))
+
+        return self.updated_copy(geometries=geometries_vjp)
+
+
+JaxGeometryType = Union[JaxSingleGeometryType, JaxGeometryGroup]
 
 # pylint: disable=unhashable-member
 JAX_GEOMETRY_MAP = {
     Box: JaxBox,
     PolySlab: JaxPolySlab,
+    GeometryGroup: JaxGeometryGroup,
 }
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/medium.py` & `tidy3d-2.3.1/tidy3d/plugins/adjoint/components/medium.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from __future__ import annotations
 
 from typing import Dict, Tuple, Union, Callable, Optional
 from abc import ABC
 
 import pydantic as pd
 import numpy as np
-import jax.numpy as jnp
 from jax.tree_util import register_pytree_node_class
 import xarray as xr
 
 from ....components.types import Bound, Literal
 from ....components.medium import Medium, AnisotropicMedium, CustomMedium
 from ....components.geometry import Geometry
 from ....components.data.monitor_data import FieldData
 from ....components.data.dataset import PermittivityDataset
 from ....components.data.data_array import ScalarFieldDataArray
 from ....exceptions import SetupError
+from ....constants import CONDUCTIVITY
 
 from .base import JaxObject
 from .types import JaxFloat, validate_jax_float
 from .data.data_array import JaxDataArray
 from .data.dataset import JaxPermittivityDataset
 
 
@@ -88,26 +88,26 @@
         inside_fn: Callable,
     ) -> xr.DataArray:
         """Get the E_fwd * E_adj * dV field distribution inside of the discretized volume."""
 
         e_fwd = grad_data_fwd.field_components[field]
         e_adj = grad_data_adj.field_components[field]
 
-        e_dotted = (e_fwd * e_adj).real
+        e_dotted = e_fwd * e_adj
 
         inside_mask = self.make_inside_mask(vol_coords=vol_coords, inside_fn=inside_fn)
 
         isel_kwargs = {
             key: [0]
             for key, value in vol_coords.items()
             if isinstance(value, float) or len(value) <= 1
         }
         interp_kwargs = {key: value for key, value in vol_coords.items() if key not in isel_kwargs}
 
-        fields_eval = e_dotted.isel(f=0, **isel_kwargs).interp(**interp_kwargs, assume_sorted=True)
+        fields_eval = e_dotted.isel(**isel_kwargs).interp(**interp_kwargs, assume_sorted=True)
         inside_mask = inside_mask.isel(**isel_kwargs)
 
         return inside_mask * d_vol * fields_eval
 
     def d_eps_map(
         self,
         grad_data_fwd: FieldData,
@@ -144,15 +144,30 @@
     permittivity: JaxFloat = pd.Field(
         1.0,
         title="Permittivity",
         description="Relative permittivity of the medium. May be a ``jax`` ``DeviceArray``.",
         jax_field=True,
     )
 
+    conductivity: JaxFloat = pd.Field(
+        0.0,
+        title="Conductivity",
+        description="Electric conductivity. Defined such that the imaginary part of the complex "
+        "permittivity at angular frequency omega is given by conductivity/omega.",
+        units=CONDUCTIVITY,
+        jax_field=True,
+    )
+
+    @pd.validator("conductivity", always=True)
+    def _passivity_validation(cls, val, values):
+        """Override of inherited validator."""
+        return val
+
     _sanitize_permittivity = validate_jax_float("permittivity")
+    _sanitize_conductivity = validate_jax_float("conductivity")
 
     def to_medium(self) -> Medium:
         """Convert :class:`.JaxMedium` instance to :class:`.Medium`"""
         self_dict = self.dict(exclude={"type"})
         return Medium.parse_obj(self_dict)
 
     # pylint:disable=too-many-locals, too-many-arguments
@@ -171,16 +186,25 @@
             grad_data_fwd=grad_data_fwd,
             grad_data_adj=grad_data_adj,
             sim_bounds=sim_bounds,
             wvl_mat=wvl_mat,
             inside_fn=inside_fn,
         )
 
-        vjp_permittivty = jnp.sum(d_eps_map.values)
-        return self.copy(update=dict(permittivity=vjp_permittivty))
+        vjp_eps_complex = np.sum(d_eps_map.values)
+
+        freq = d_eps_map.coords["f"][0]
+        vjp_eps, vjp_sigma = self.eps_complex_to_eps_sigma(vjp_eps_complex, freq)
+
+        return self.copy(
+            update=dict(
+                permittivity=vjp_eps,
+                conductivity=vjp_sigma,
+            )
+        )
 
 
 @register_pytree_node_class
 class JaxAnisotropicMedium(AnisotropicMedium, AbstractJaxMedium):
     """A :class:`.Medium` registered with jax."""
 
     xx: JaxMedium = pd.Field(
@@ -246,16 +270,22 @@
                 grad_data_fwd=grad_data_fwd,
                 grad_data_adj=grad_data_adj,
                 vol_coords=vol_coords,
                 d_vol=d_vol,
                 inside_fn=inside_fn,
             )
 
-            vjp_ii = jnp.sum(e_mult_dim.real.values)
-            vjp_fields[component_name] = JaxMedium(permittivity=vjp_ii)
+            vjp_eps_complex_ii = np.sum(e_mult_dim.values)
+            freq = e_mult_dim.coords["f"][0]
+            vjp_eps_ii, vjp_sigma_ii = self.eps_complex_to_eps_sigma(vjp_eps_complex_ii, freq)
+
+            vjp_fields[component_name] = JaxMedium(
+                permittivity=vjp_eps_ii,
+                conductivity=vjp_sigma_ii,
+            )
 
         return self.copy(update=vjp_fields)
 
 
 @register_pytree_node_class
 class JaxCustomMedium(CustomMedium, AbstractJaxMedium):
     """A :class:`.CustomMedium` registered with ``jax``.
@@ -299,31 +329,30 @@
         return values
 
     @pd.root_validator(pre=True)
     def _deprecation_dataset(cls, values):
         """Raise deprecation warning if dataset supplied and convert to dataset."""
         return values
 
-    @pd.validator("eps_dataset", always=True)
-    def _is_not_3d(cls, val):
-        """Ensure the custom medium pixels contain at least one dimension with only pixel thick."""
+    # @pd.validator("eps_dataset", always=True)
+    # def _is_not_3d(cls, val):
+    #     """Ensure the custom medium pixels contain at least one dimension with one pixel thick."""
+    #     for field_dim in "xyz":
+    #         field_name = f"eps_{field_dim}{field_dim}"
+    #         data_array = val.field_components[field_name]
+    #         coord_lens = [len(data_array.coords[key]) for key in "xyz"]
+    #         dims_len1 = [val == 1 for val in coord_lens]
+    #         if sum(dims_len1) == 0:
+    #             raise SetupError(
+    #                 "For adjoint plugin, the 'JaxCustomMedium' is restricted to a 1D or 2D "
+    #                 "pixellated grid. It may not contain multiple pixels along all 3 dimensions. "
+    #                 f"Detected 3D pixelated grid in '{field_name}' component of 'eps_dataset'."
+    #             )
 
-        for field_dim in "xyz":
-            field_name = f"eps_{field_dim}{field_dim}"
-            data_array = val.field_components[field_name]
-            coord_lens = [len(data_array.coords[key]) for key in "xyz"]
-            dims_len1 = [val == 1 for val in coord_lens]
-            if sum(dims_len1) == 0:
-                raise SetupError(
-                    "For adjoint plugin, the 'JaxCustomMedium' is restricted to a 1D or 2D "
-                    "pixellated grid. It may not contain multiple pixels along all 3 dimensions. "
-                    f"Detected 3D pixelated grid in '{field_name}' component of 'eps_dataset'."
-                )
-
-        return val
+    #     return val
 
     @pd.validator("eps_dataset", always=True)
     def _is_not_too_large(cls, val):
         """Ensure number of pixels doesnt surpass a set amount."""
 
         for field_dim in "xyz":
             field_name = f"eps_{field_dim}{field_dim}"
@@ -341,26 +370,26 @@
 
     @pd.validator("eps_dataset", always=True)
     def _eps_dataset_single_frequency(cls, val):
         """Override of inherited validator."""
         return val
 
     @pd.validator("eps_dataset", always=True)
-    def _eps_dataset_eps_inf_greater_no_less_than_one_sigma_positive(cls, val):
+    def _eps_dataset_eps_inf_greater_no_less_than_one_sigma_positive(cls, val, values):
         """Override of inherited validator."""
         return val
 
     @pd.validator("permittivity", always=True)
     def _eps_inf_greater_no_less_than_one(cls, val):
-        """Assert any eps_inf must be >=1"""
+        """Override of inherited validator."""
         return val
 
     @pd.validator("conductivity", always=True)
     def _conductivity_non_negative_correct_shape(cls, val, values):
-        """Assert conductivity>=0"""
+        """Override of inherited validator."""
         return val
 
     def eps_dataarray_freq(self, frequency: float):
         """ "Permittivity array at ``frequency``"""
         as_custom_medium = self.to_medium()
         return as_custom_medium.eps_dataarray_freq(frequency)
 
@@ -488,20 +517,24 @@
                 grad_data_fwd=grad_data_fwd,
                 grad_data_adj=grad_data_adj,
                 vol_coords=interp_coords,
                 d_vol=d_vols,
                 inside_fn=inside_fn,
             ).sum(sum_axes)
 
-            # if np.any(np.isnan(e_dotted)) or np.isclose(np.sum(e_dotted), 0):
-            #     import pdb; pdb.set_trace()
-
             # reshape values to the expected vjp shape to be more safe
             vjp_shape = tuple(len(coord) for _, coord in coords.items())
-            vjp_values = e_dotted.real.values.reshape(vjp_shape)
+
+            # make sure this has the same dtype as the original
+            dtype_orig = np.array(orig_data_array.values).dtype
+
+            vjp_values = e_dotted.values.reshape(vjp_shape)
+            if dtype_orig.kind == "f":
+                vjp_values = vjp_values.real
+            vjp_values = vjp_values.astype(dtype_orig)
 
             # construct a DataArray storing the vjp
             vjp_data_array = JaxDataArray(values=vjp_values, coords=coords)
             vjp_field_components[eps_field_name] = vjp_data_array
 
         # package everything into dataset
         vjp_eps_dataset = JaxPermittivityDataset(**vjp_field_components)
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/simulation.py` & `tidy3d-2.3.1/tidy3d/plugins/adjoint/components/simulation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Defines a jax-compatible simulation."""
 from __future__ import annotations
 
 from typing import Tuple, Union, List, Dict
+from multiprocessing import Pool
 
 import pydantic as pd
 import numpy as np
 
 from jax.tree_util import register_pytree_node_class
 
 from ....log import log
@@ -17,15 +18,25 @@
 from ....components.structure import Structure
 from ....components.types import Ax, annotate_type
 from ....constants import HERTZ
 from ....exceptions import AdjointError
 
 from .base import JaxObject
 from .structure import JaxStructure
-from .geometry import JaxPolySlab
+from .geometry import JaxPolySlab, JaxGeometryGroup
+
+
+# bandwidth of adjoint source in units of freq0 if no sources and no `fwidth_adjoint` specified
+FWIDTH_FACTOR = 1.0 / 10
+
+# how many processors to use for server and client side adjoint
+NUM_PROC_LOCAL = 1
+
+# number of input structures before it errors
+MAX_NUM_INPUT_STRUCTURES = 400
 
 
 class JaxInfo(Tidy3dBaseModel):
     """Class to store information when converting between jax and tidy3d."""
 
     num_input_structures: pd.NonNegativeInt = pd.Field(
         ...,
@@ -55,18 +66,14 @@
         None,
         title="Adjoint Frequency Width",
         description="Custom frequency width of the original JaxSimulation.",
         units=HERTZ,
     )
 
 
-# bandwidth of adjoint source in units of freq0 if no sources and no `fwidth_adjoint` specified
-FWIDTH_FACTOR = 1.0 / 10
-
-
 @register_pytree_node_class
 class JaxSimulation(Simulation, JaxObject):
     """A :class:`.Simulation` registered with jax."""
 
     input_structures: Tuple[JaxStructure, ...] = pd.Field(
         (),
         title="Input Structures",
@@ -130,14 +137,26 @@
     def _subpixel_is_on(cls, val):
         """Assert subpixel is on."""
         if not val:
             raise AdjointError("'JaxSimulation.subpixel' must be 'True' to use adjoint plugin.")
         return val
 
     @pd.validator("input_structures", always=True)
+    def _restrict_input_structures(cls, val):
+        """Restrict number of input structures."""
+        num_input_structures = len(val)
+        if num_input_structures > MAX_NUM_INPUT_STRUCTURES:
+            raise AdjointError(
+                "For performance, adjoint plugin restricts the number of input structures to "
+                f"{MAX_NUM_INPUT_STRUCTURES}. Found {num_input_structures}."
+            )
+
+        return val
+
+    @pd.validator("input_structures", always=True)
     def _warn_overlap(cls, val, values):
         """Print appropriate warning if structures intersect in ways that cause gradient error."""
 
         input_structures = list(val)
         structures = list(values.get("structures"))
 
         # if the center and size of all structure geometries do not contain all numbers, skip check
@@ -172,14 +191,28 @@
                             f"intersects with 'JaxSimulation.structures[{j}]'. Note that in this "
                             "version of the adjoint plugin, there may be errors in the gradient "
                             "when 'JaxPolySlab' intersects with background structures."
                         )
 
         return val
 
+    @pd.validator("output_monitors", always=True)
+    def _warn_if_colocate(cls, val):
+        """warn if any colocate=True in output FieldMonitors."""
+        for index, mnt in enumerate(val):
+            if isinstance(mnt, FieldMonitor):
+                if mnt.colocate:
+                    log.warning(
+                        f"'FieldMonitor' at 'JaxSimulation.output_monitors[{index}]' "
+                        "has 'colocate=True', "
+                        "this may lead to decreased accuracy in adjoint gradient."
+                    )
+                    return val
+        return val
+
     @staticmethod
     def get_freq_adjoint(output_monitors: List[Monitor]) -> float:
         """Return the single adjoint frequency stripped from the output monitors."""
 
         if len(output_monitors) == 0:
             raise AdjointError("Can't get adjoint frequency as no output monitors present.")
 
@@ -407,52 +440,140 @@
     def to_simulation_fwd(self) -> Tuple[Simulation, JaxInfo, JaxInfo]:
         """Like ``to_simulation()`` but the gradient monitors are included."""
         simulation, jax_info = self.to_simulation()
         sim_fwd, jax_info_fwd = self.make_sim_fwd(simulation=simulation, jax_info=jax_info)
         return sim_fwd, jax_info_fwd, jax_info
 
     @staticmethod
-    def get_grad_monitors(input_structures: List[Structure], freq_adjoint: float) -> dict:
+    def get_grad_monitors(
+        input_structures: List[Structure], freq_adjoint: float, include_eps_mnts: bool = True
+    ) -> dict:
         """Return dictionary of gradient monitors for simulation."""
         grad_mnts = []
         grad_eps_mnts = []
         for index, structure in enumerate(input_structures):
             grad_mnt, grad_eps_mnt = structure.make_grad_monitors(
                 freq=freq_adjoint, name=f"grad_mnt_{index}"
             )
             grad_mnts.append(grad_mnt)
-            grad_eps_mnts.append(grad_eps_mnt)
+            if include_eps_mnts:
+                grad_eps_mnts.append(grad_eps_mnt)
         return dict(grad_monitors=grad_mnts, grad_eps_monitors=grad_eps_mnts)
 
+    def _store_vjp_structure(
+        self,
+        structure: JaxStructure,
+        fld_fwd: FieldData,
+        fld_adj: FieldData,
+        eps_data: PermittivityData,
+        num_proc: int = NUM_PROC_LOCAL,
+    ) -> JaxStructure:
+        """Store the vjp for a single structure."""
+
+        freq = float(eps_data.eps_xx.coords["f"])
+        eps_out = self.medium.eps_model(frequency=freq)
+        return structure.store_vjp(
+            grad_data_fwd=fld_fwd,
+            grad_data_adj=fld_adj,
+            grad_data_eps=eps_data,
+            sim_bounds=self.bounds,
+            eps_out=eps_out,
+            num_proc=num_proc,
+        )
+
     def store_vjp(
         self,
         grad_data_fwd: Tuple[FieldData],
         grad_data_adj: Tuple[FieldData],
         grad_eps_data: Tuple[PermittivityData],
+        num_proc: int = NUM_PROC_LOCAL,
     ) -> JaxSimulation:
         """Store the vjp w.r.t. each input_structure as a sim using fwd and adj grad_data."""
 
-        input_structures_vjp = []
-        adjoint_info = zip(self.input_structures, grad_data_fwd, grad_data_adj, grad_eps_data)
+        # if num_proc supplied and greater than 1, run parallel
+        if num_proc is not None and num_proc > 1:
+            return self.store_vjp_parallel(
+                grad_data_fwd=grad_data_fwd,
+                grad_data_adj=grad_data_adj,
+                grad_eps_data=grad_eps_data,
+                num_proc=num_proc,
+            )
+
+        # otherwise, call regular sequential one
+        return self.store_vjp_sequential(
+            grad_data_fwd=grad_data_fwd, grad_data_adj=grad_data_adj, grad_eps_data=grad_eps_data
+        )
 
-        for in_struct, fld_fwd, fld_adj, eps_data in adjoint_info:
+    def store_vjp_sequential(
+        self,
+        grad_data_fwd: Tuple[FieldData],
+        grad_data_adj: Tuple[FieldData],
+        grad_eps_data: Tuple[PermittivityData],
+    ) -> JaxSimulation:
+        """Store the vjp w.r.t. each input_structure without multiprocessing."""
+        map_args = [self.input_structures, grad_data_fwd, grad_data_adj, grad_eps_data]
+        input_structures_vjp = list(map(self._store_vjp_structure, *map_args))
+
+        return self.copy(
+            update=dict(
+                input_structures=input_structures_vjp, grad_monitors=(), grad_eps_monitors=()
+            )
+        )
+
+    def store_vjp_parallel(
+        self,
+        grad_data_fwd: Tuple[FieldData],
+        grad_data_adj: Tuple[FieldData],
+        grad_eps_data: Tuple[PermittivityData],
+        num_proc: int,
+    ) -> JaxSimulation:
+        """Store the vjp w.r.t. each input_structure as a sim using fwd and adj grad_data, and
+        parallel processing over ``num_proc`` processes."""
 
-            freq = float(eps_data.eps_xx.coords["f"])
-            eps_out = self.medium.eps_model(frequency=freq)
-            eps_in = in_struct.medium.eps_model(frequency=freq)
-
-            input_structure_vjp = in_struct.store_vjp(
-                grad_data_fwd=fld_fwd,
-                grad_data_adj=fld_adj,
-                grad_data_eps=eps_data,
-                sim_bounds=self.bounds,
-                eps_out=eps_out,
-                eps_in=eps_in,
+        # Indexing into structures which use internal parallelization, and those which don't.
+        # For the latter, simple parallelization over the list will be used.
+        internal_par_structs = [JaxGeometryGroup]
+
+        # Parallelize polyslabs internally or externally depending on total number
+        polyslabs = [struct for struct in self.input_structures if isinstance(struct, JaxPolySlab)]
+        if len(polyslabs) < num_proc:
+            internal_par_structs += [JaxPolySlab]
+
+        inds_par_internal, inds_par_external = [], []
+        for index, structure in enumerate(self.input_structures):
+            if isinstance(structure.geometry, tuple(internal_par_structs)):
+                inds_par_internal.append(index)
+            else:
+                inds_par_external.append(index)
+
+        def make_args(indexes, num_proc_internal):
+            """Make the arguments to map over selecting over a set of structure ``indexes``."""
+            structures = [self.input_structures[index] for index in indexes]
+            data_fwd = [grad_data_fwd[index] for index in indexes]
+            data_bwd = [grad_data_adj[index] for index in indexes]
+            eps_data = [grad_eps_data[index] for index in indexes]
+            num_proc = [num_proc_internal] * len(indexes)
+
+            return (structures, data_fwd, data_bwd, eps_data, num_proc)
+
+        # Get vjps for structures that parallelize internally using simple map
+        args_par_internal = make_args(inds_par_internal, num_proc_internal=num_proc)
+        vjps_par_internal = list(map(self._store_vjp_structure, *args_par_internal))
+
+        # Get vjps for structures where we parallelize directly here
+        args_par_external = make_args(inds_par_external, num_proc_internal=NUM_PROC_LOCAL)
+        with Pool(num_proc) as pool:
+            vjps_par_external = list(
+                pool.starmap(self._store_vjp_structure, zip(*args_par_external))
             )
 
-            input_structures_vjp.append(input_structure_vjp)
+        # Reshuffle the two lists back in the correct order
+        vjps_all = list(vjps_par_internal) + list(vjps_par_external)
+        input_structures_vjp = [None] * len(self.input_structures)
+        for index, vjp in zip(inds_par_internal + inds_par_external, vjps_all):
+            input_structures_vjp[index] = vjp
 
         return self.copy(
             update=dict(
                 input_structures=input_structures_vjp, grad_monitors=(), grad_eps_monitors=()
             )
         )
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/structure.py` & `tidy3d-2.3.1/tidy3d/plugins/adjoint/components/structure.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,32 +60,34 @@
     def store_vjp(
         self,
         grad_data_fwd: FieldData,
         grad_data_adj: FieldData,
         grad_data_eps: PermittivityData,
         sim_bounds: Bound,
         eps_out: complex,
-        eps_in: complex,
+        num_proc: int = 1,
     ) -> JaxStructure:
         """Returns the gradient of the structure parameters given forward and adjoint field data."""
 
         # compute wavelength in material (to use for determining integration points)
         freq = float(grad_data_eps.eps_xx.f)
         wvl_free_space = C_0 / freq
-        ref_ind = np.sqrt(np.max(np.real(self.medium.eps_model(freq))))
+        eps_in = self.medium.eps_model(frequency=freq)
+        ref_ind = np.sqrt(np.max(np.real(eps_in)))
         wvl_mat = wvl_free_space / ref_ind
 
         geo_vjp = self.geometry.store_vjp(
             grad_data_fwd=grad_data_fwd,
             grad_data_adj=grad_data_adj,
             grad_data_eps=grad_data_eps,
             sim_bounds=sim_bounds,
             wvl_mat=wvl_mat,
             eps_out=eps_out,
             eps_in=eps_in,
+            num_proc=num_proc,
         )
 
         medium_vjp = self.medium.store_vjp(
             grad_data_fwd=grad_data_fwd,
             grad_data_adj=grad_data_adj,
             sim_bounds=sim_bounds,
             wvl_mat=wvl_mat,
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/components/types.py` & `tidy3d-2.3.1/tidy3d/plugins/adjoint/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/plugins/adjoint/web.py` & `tidy3d-2.3.1/tidy3d/plugins/adjoint/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 from ...components.types import Literal
 
 from .components.base import JaxObject
 from .components.simulation import JaxSimulation, JaxInfo
 from .components.data.sim_data import JaxSimulationData
 
 
-# TODO: confused about these paths, they aren't local but rather wherre the jax info and sim_vjp get
-# stored on the server? maybe add a comment for each?
-# when i changed them, adjoint runs errored on the solver.
+# file names and paths for server side adjoint
 SIM_VJP_FILE = "output/jax_sim_vjp.hdf5"
 JAX_INFO_FILE = "jax_info.json"
 
 
 @register_pytree_node_class
 class RunResidual(JaxObject):
     """Class to store extra data needed to pass between the forward and backward adjoint run."""
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/plugins/dispersion/fit.py` & `tidy3d-2.3.1/tidy3d/plugins/dispersion/fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from ...log import log
 from ...components.base import Tidy3dBaseModel, cached_property
 from ...components.medium import PoleResidue, AbstractMedium
 from ...components.viz import add_ax_if_none
 from ...components.types import Ax, ArrayFloat1D
 from ...constants import C_0, HBAR, MICROMETER
 from ...exceptions import ValidationError, WebError, SetupError
-from ...web.config import DEFAULT_CONFIG as Config
+from ...web.environment import Env
 
 
 class DispersionFitter(Tidy3dBaseModel):
     """Tool for fitting refractive index data to get a
     dispersive medium described by :class:`.PoleResidue` model."""
 
     wvl_um: ArrayFloat1D = Field(
@@ -582,16 +582,15 @@
             Ignore the k data if they are present, so the fitted material is lossless.
 
         Returns
         -------
         :class:`DispersionFitter`
             A :class:`DispersionFitter` instance.
         """
-
-        resp = requests.get(url_file, verify=Config.ssl_verify)
+        resp = requests.get(url_file, verify=Env.current.ssl_verify)
 
         try:
             resp.raise_for_status()
         except Exception as e:  # pylint:disable=broad-except
             raise WebError("Connection to the website failed. Please provide a valid URL.") from e
 
         data_url = list(
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/plugins/dispersion/web.py` & `tidy3d-2.3.1/tidy3d/plugins/dispersion/web.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from ...log import log
 from ...components.base import Tidy3dBaseModel
 from ...components.types import Literal
 from ...components.medium import PoleResidue
 from ...constants import MICROMETER, HERTZ
 from ...exceptions import WebError, Tidy3dError, SetupError
 from ...web.httputils import get_headers
-from ...web.config import DEFAULT_CONFIG
+from ...web.environment import Env
 
 from .fit import DispersionFitter
 
 
 BOUND_MAX_FACTOR = 10
 
 URL_ENV = {
@@ -225,35 +225,35 @@
         ----------
         config_env : Literal["default", "dev", "prod", "local"], optional
             Service environment to pick from
         """
 
         _env = config_env
         if _env == "default":
-            _env = "dev" if "dev" in DEFAULT_CONFIG.web_api_endpoint else "prod"
+            _env = "dev" if "dev" in Env.current.web_api_endpoint else "prod"
         return URL_ENV[_env]
 
     @staticmethod
     def _setup_server(url_server: str):
         """set up web server access
 
         Parameters
         ----------
         url_server : str
             URL for the server
         """
 
         try:
             # test connection
-            resp = requests.get(f"{url_server}/health", verify=DEFAULT_CONFIG.ssl_verify)
+            resp = requests.get(f"{url_server}/health", verify=Env.current.ssl_verify)
             resp.raise_for_status()
         except (requests.exceptions.SSLError, ssl.SSLError):
             log.info("Retrying with SSL verification disabled.")
-            DEFAULT_CONFIG.ssl_verify = False
-            resp = requests.get(f"{url_server}/health", verify=DEFAULT_CONFIG.ssl_verify)
+            Env.current.ssl_verify = False
+            resp = requests.get(f"{url_server}/health", verify=Env.current.ssl_verify)
         except Exception as e:
             raise WebError("Connection to the server failed. Please try again.") from e
 
         return get_headers()
 
     def run(self) -> Tuple[PoleResidue, float]:
         """Execute the data fit using the stable fitter in the server.
@@ -267,15 +267,15 @@
         url_server = self._set_url("default")
         headers = self._setup_server(url_server)
 
         resp = requests.post(
             f"{url_server}/dispersion/fit",
             headers=headers,
             data=self.json(),
-            verify=DEFAULT_CONFIG.ssl_verify,
+            verify=Env.current.ssl_verify,
         )
 
         try:
             resp.raise_for_status()
         except Exception as e:
             if resp.status_code == ExceptionCodes.GATEWAY_TIMEOUT.value:
                 msg = (
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/plugins/mode/derivatives.py` & `tidy3d-2.3.1/tidy3d/plugins/mode/derivatives.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,32 +135,34 @@
     if direction == "b":
         return create_sfactor_b(omega, dls, N, n_pml, dmin_pml)
 
     raise ValueError(f"Direction value {direction} not recognized")
 
 
 def create_sfactor_f(omega, dls, N, n_pml, dmin_pml):
-    """S-factor profile for forward derivative matrix"""
+    """S-factor profile applied after forward derivative matrix, i.e. applied to H-field
+    locations."""
     sfactor_array = np.ones(N, dtype=np.complex128)
     for i in range(N):
-        if i <= n_pml and dmin_pml:
-            sfactor_array[i] = s_value(dls[0], (n_pml - i + 0.5) / n_pml, omega)
-        elif i > N - n_pml:
-            sfactor_array[i] = s_value(dls[-1], (i - (N - n_pml) - 0.5) / n_pml, omega)
+        if i <= n_pml - 1 and dmin_pml:
+            sfactor_array[i] = s_value(dls[0], (n_pml - i - 0.5) / n_pml, omega)
+        elif i >= N - n_pml:
+            sfactor_array[i] = s_value(dls[-1], (i - (N - n_pml) + 0.5) / n_pml, omega)
     return sfactor_array
 
 
 def create_sfactor_b(omega, dls, N, n_pml, dmin_pml):
-    """S-factor profile for backward derivative matrix"""
+    """S-factor profile applied after backward derivative matrix, i.e. applied to E-field
+    locations."""
     sfactor_array = np.ones(N, dtype=np.complex128)
     for i in range(N):
-        if i <= n_pml and dmin_pml:
-            sfactor_array[i] = s_value(dls[0], (n_pml - i + 1) / n_pml, omega)
+        if i < n_pml and dmin_pml:
+            sfactor_array[i] = s_value(dls[0], (n_pml - i) / n_pml, omega)
         elif i > N - n_pml:
-            sfactor_array[i] = s_value(dls[-1], (i - (N - n_pml) - 1) / n_pml, omega)
+            sfactor_array[i] = s_value(dls[-1], (i - (N - n_pml)) / n_pml, omega)
     return sfactor_array
 
 
 def sig_w(dl, step, sorder=3):
     """Fictional conductivity, note that these values might need tuning"""
     sig_max = 0.8 * (sorder + 1) / (ETA_0 * dl)
     return sig_max * step**sorder
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/plugins/mode/mode_solver.py` & `tidy3d-2.3.1/tidy3d/plugins/mode/mode_solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Solve for modes in a 2D cross-sectional plane in a simulation, assuming translational
 invariance along a given propagation axis.
 """
 
+from __future__ import annotations
 from typing import List, Tuple, Dict
 
 import numpy as np
 import pydantic
 import xarray as xr
 
 from ...log import log
@@ -13,15 +14,15 @@
 from ...components.geometry import Box
 from ...components.simulation import Simulation
 from ...components.grid.grid import Grid
 from ...components.mode import ModeSpec
 from ...components.monitor import ModeSolverMonitor, ModeMonitor
 from ...components.source import ModeSource, SourceTime
 from ...components.types import Direction, FreqArray, Ax, Literal, Axis, Symmetry, PlotScale
-from ...components.types import ArrayComplex3D, ArrayComplex4D, ArrayFloat1D
+from ...components.types import ArrayComplex3D, ArrayComplex4D, ArrayFloat1D, EpsSpecType
 from ...components.data.data_array import ModeIndexDataArray, ScalarModeFieldDataArray
 from ...components.data.data_array import FreqModeDataArray
 from ...components.data.sim_data import SimulationData
 from ...components.data.monitor_data import ModeSolverData
 from ...exceptions import ValidationError
 from ...constants import C_0
 from .solver import compute_modes
@@ -53,14 +54,21 @@
         description="Container with specifications about the modes to be solved for.",
     )
 
     freqs: FreqArray = pydantic.Field(
         ..., title="Frequencies", description="A list of frequencies at which to solve."
     )
 
+    direction: Direction = pydantic.Field(
+        "+",
+        title="Propagation direction",
+        description="Direction of waveguide mode propagation along the axis defined by its normal "
+        "dimension.",
+    )
+
     @pydantic.validator("plane", always=True)
     def is_plane(cls, val):
         """Raise validation error if not planar."""
         if val.size.count(0.0) != 1:
             raise ValidationError(f"ModeSolver plane must be planar, given size={val}")
         return val
 
@@ -110,69 +118,57 @@
         """:class:`.ModeSolverData` containing the field and effective index data.
 
         Returns
         -------
         ModeSolverData
             :class:`.ModeSolverData` object containing the effective index and mode fields.
         """
+        log.warning(
+            "Use the remote mode solver with subpixel averaging for better accuracy through "
+            "'tidy3d.plugins.mode.web.run(...)'.",
+            log_once=True,
+        )
         return self.data
 
-    # pylint: disable=too-many-locals
+    def _freqs_for_group_index(self) -> FreqArray:
+        """Get frequencies used to compute group index."""
+        f_step = self.mode_spec.group_index_step
+        fractional_steps = (1 - f_step, 1, 1 + f_step)
+        return np.outer(self.freqs, fractional_steps).flatten()
+
+    def _remove_freqs_for_group_index(self) -> FreqArray:
+        """Remove frequencies used to compute group index.
+
+        Returns
+        -------
+        FreqArray
+            Filtered frequency array with only original values.
+        """
+        return np.array(self.freqs[1 : len(self.freqs) : 3])
+
     def _get_data_with_group_index(self) -> ModeSolverData:
         """:class:`.ModeSolverData` with fields, effective and group indices on unexpanded grid.
 
         Returns
         -------
         ModeSolverData
             :class:`.ModeSolverData` object containing the effective and group indices, and mode
             fields.
         """
 
-        # insert extra frequency steps into original array
-        f_step = self.mode_spec.group_index_step
-        fractional_steps = (1 - f_step, 1, 1 + f_step)
-        freqs = np.outer(self.freqs, fractional_steps).flatten()
-
         # create a copy with the required frequencies for numerical differentiation
         mode_spec = self.mode_spec.copy(update={"group_index_step": False})
-        mode_solver = self.copy(update={"freqs": freqs, "mode_spec": mode_spec})
-        mode_solver_data = mode_solver.data_raw
-
-        # calculate group index
-        num_freqs = freqs.size
-        original_slice = slice(1, num_freqs, 3)
-        n_center = mode_solver_data.n_eff.isel(f=original_slice).values
-        n_backward = mode_solver_data.n_eff.isel(f=slice(0, num_freqs, 3)).values
-        n_forward = mode_solver_data.n_eff.isel(f=slice(2, num_freqs, 3)).values
-
-        n_group_data = n_center + (n_forward - n_backward) / (2 * f_step)
-        n_group = ModeIndexDataArray(
-            n_group_data,
-            coords={
-                "f": list(self.freqs),
-                "mode_index": np.arange(self.mode_spec.num_modes),
-            },
-            attrs={"long name": "Group index"},
-        )
-
-        # remove data corresponding to frequencies used only for group index calculation
-        update_dict = {
-            "n_complex": mode_solver_data.n_complex.isel(f=original_slice),
-            "n_group": n_group,
-        }
-
-        for key, field in mode_solver_data.field_components.items():
-            update_dict[key] = field.isel(f=original_slice)
-
-        # pylint: disable=protected-access
-        for key, data in mode_solver_data._grid_correction_dict.items():
-            update_dict[key] = data.isel(f=original_slice)
+        mode_solver = self.copy(
+            update={"freqs": self._freqs_for_group_index(), "mode_spec": mode_spec}
+        )
 
-        return mode_solver_data.copy(update=update_dict)
+        # pylint:disable=protected-access
+        return mode_solver.data_raw._group_index_post_process(self.mode_spec.group_index_step)
 
+    # pylint:disable=too-many-locals
     @cached_property
     def data_raw(self) -> ModeSolverData:
         """:class:`.ModeSolverData` containing the field and effective index on unexpanded grid.
 
         Returns
         -------
         ModeSolverData
@@ -183,15 +179,15 @@
             return self._get_data_with_group_index()
 
         _, _solver_coords = self.plane.pop_axis(
             self._solver_grid.boundaries.to_list, axis=self.normal_axis
         )
 
         # Compute and store the modes at all frequencies
-        n_complex, fields = self._solve_all_freqs(
+        n_complex, fields, eps_spec = self._solve_all_freqs(
             coords=_solver_coords, symmetry=self.solver_symmetry
         )
 
         # start a dictionary storing the data arrays for the ModeSolverData
         index_data = ModeIndexDataArray(
             np.stack(n_complex, axis=0),
             coords=dict(
@@ -222,25 +218,32 @@
                     f=list(self.freqs),
                     mode_index=np.arange(self.mode_spec.num_modes),
                 ),
             )
             data_dict[field_name] = scalar_field_data
 
         # finite grid corrections
-        grid_factors = self._grid_correction(index_data)
+        grid_factors = self._grid_correction(
+            simulation=self.simulation,
+            plane=self.plane,
+            mode_spec=self.mode_spec,
+            n_complex=index_data,
+            direction=self.direction,
+        )
 
         # make mode solver data
         mode_solver_monitor = self.to_mode_solver_monitor(name=MODE_MONITOR_NAME)
         mode_solver_data = ModeSolverData(
             monitor=mode_solver_monitor,
             symmetry=self.simulation.symmetry,
             symmetry_center=self.simulation.center,
             grid_expanded=self.simulation.discretize(self.plane, extend=True),
             grid_primal_correction=grid_factors[0],
             grid_dual_correction=grid_factors[1],
+            eps_spec=eps_spec,
             **data_dict,
         )
         self._field_decay_warning(mode_solver_data.symmetry_expanded_copy)
 
         # normalize modes
         scaling = np.sqrt(np.abs(mode_solver_data.flux))
         mode_solver_data = mode_solver_data.copy(
@@ -286,16 +289,15 @@
         eps_keys = ["Ex", "Exy", "Exz", "Eyx", "Ey", "Eyz", "Ezx", "Ezy", "Ez"]
         eps_tensor = [
             self.simulation.epsilon_on_grid(self._solver_grid, key, freq) for key in eps_keys
         ]
         return np.stack(eps_tensor, axis=0)
 
     def _solver_eps(self, freq: float) -> ArrayComplex4D:
-        """Get the permittivity tensor in the shape needed to be supplied to the sovler, with the
-        normal axis rotated to z."""
+        """Diagonal permittivity in the shape needed by solver, with normal axis rotated to z."""
 
         # Get diagonal epsilon components in the plane
         eps_tensor = self._get_epsilon(freq)
 
         # get rid of normal axis
         eps_tensor = np.take(eps_tensor, indices=[0], axis=1 + self.normal_axis)
         eps_tensor = np.squeeze(eps_tensor, axis=1 + self.normal_axis)
@@ -321,45 +323,50 @@
         # construct eps to feed to mode solver
         return eps_tensor
 
     def _solve_all_freqs(
         self,
         coords: Tuple[ArrayFloat1D, ArrayFloat1D],
         symmetry: Tuple[Symmetry, Symmetry],
-    ) -> Tuple[List[float], List[Dict[str, ArrayComplex4D]]]:
+    ) -> Tuple[List[float], List[Dict[str, ArrayComplex4D]], List[EpsSpecType]]:
         """Call the mode solver at all requested frequencies."""
 
         fields = []
         n_complex = []
+        eps_spec = []
         for freq in self.freqs:
-            n_freq, fields_freq = self._solve_single_freq(
+            # pylint: disable=unbalanced-tuple-unpacking
+            n_freq, fields_freq, eps_spec_freq = self._solve_single_freq(
                 freq=freq, coords=coords, symmetry=symmetry
             )
             fields.append(fields_freq)
             n_complex.append(n_freq)
+            eps_spec.append(eps_spec_freq)
 
-        return n_complex, fields
+        return n_complex, fields, eps_spec
 
     # pylint:disable=too-many-locals
     def _solve_single_freq(
         self,
         freq: float,
         coords: Tuple[ArrayFloat1D, ArrayFloat1D],
         symmetry: Tuple[Symmetry, Symmetry],
-    ) -> Tuple[float, Dict[str, ArrayComplex4D]]:
+    ) -> Tuple[float, Dict[str, ArrayComplex4D], EpsSpecType]:
         """Call the mode solver at a single frequency.
+
         The fields are rotated from propagation coordinates back to global coordinates.
         """
 
-        solver_fields, n_complex = compute_modes(
+        solver_fields, n_complex, eps_spec = compute_modes(
             eps_cross=self._solver_eps(freq),
             coords=coords,
             freq=freq,
             mode_spec=self.mode_spec,
             symmetry=symmetry,
+            direction=self.direction,
         )
 
         fields = {key: [] for key in ("Ex", "Ey", "Ez", "Hx", "Hy", "Hz")}
         for mode_index in range(self.mode_spec.num_modes):
             # Get E and H fields at the current mode_index
             ((Ex, Ey, Ez), (Hx, Hy, Hz)) = self._process_fields(solver_fields, mode_index)
 
@@ -367,15 +374,15 @@
             fields_mode = {"Ex": Ex, "Ey": Ey, "Ez": Ez, "Hx": Hx, "Hy": Hy, "Hz": Hz}
             for field_name, field in fields_mode.items():
                 fields[field_name].append(field)
 
         for field_name, field in fields.items():
             fields[field_name] = np.stack(field, axis=-1)
 
-        return n_complex, fields
+        return n_complex, fields, eps_spec
 
     def _rotate_field_coords(self, field: FIELD) -> FIELD:
         """Move the propagation axis=z to the proper order in the array."""
         f_x, f_y, f_z = np.moveaxis(field, source=3, destination=1 + self.normal_axis)
         return np.stack(self.plane.unpop_axis(f_z, (f_x, f_y), axis=self.normal_axis), axis=0)
 
     def _process_fields(
@@ -426,18 +433,25 @@
                 # Warn if needed
                 if e_edge / e_norm > FIELD_DECAY_CUTOFF:
                     log.warning(
                         f"Mode field at frequency index {freq_index}, mode index {mode_index} does "
                         "not decay at the plane boundaries."
                     )
 
+    @staticmethod
     def _grid_correction(
-        self, n_complex: ModeIndexDataArray
+        simulation: Simulation,
+        plane: Box,
+        mode_spec: ModeSpec,
+        n_complex: ModeIndexDataArray,
+        direction: Direction,
     ) -> [FreqModeDataArray, FreqModeDataArray]:
-        """Return a copy of the :class:`.ModeSolverData` with the fields renormalized to account
+        """Correct the fields due to propagation on the grid.
+
+        Return a copy of the :class:`.ModeSolverData` with the fields renormalized to account
         for propagation on a finite grid along the propagation direction. The fields are assumed to
         have ``E exp(1j k r)`` dependence on the finite grid and are then resampled using linear
         interpolation to the exact position of the mode plane. This is needed to correctly compute
         overlap with fields that come from a :class:`.FieldMonitor` placed in the same grid.
 
         Parameters
         ----------
@@ -445,30 +459,33 @@
             Numerical grid on which the modes are assumed to propagate.
 
         Returns
         -------
         :class:`.ModeSolverData`
             Copy of the data with renormalized fields.
         """
-        normal_pos = self.plane.center[self.normal_axis]
-        normal_dim = "xyz"[self.normal_axis]
+        normal_axis = plane.size.index(0.0)
+        normal_pos = plane.center[normal_axis]
+        normal_dim = "xyz"[normal_axis]
 
         # Primal and dual grid along the normal direction,
         # i.e. locations of the tangential E-field and H-field components, respectively
-        grid = self.simulation.grid
-        normal_primal = grid.boundaries.to_list[self.normal_axis]
+        grid = simulation.grid
+        normal_primal = grid.boundaries.to_list[normal_axis]
         normal_primal = xr.DataArray(normal_primal, coords={normal_dim: normal_primal})
-        normal_dual = grid.centers.to_list[self.normal_axis]
+        normal_dual = grid.centers.to_list[normal_axis]
         normal_dual = xr.DataArray(normal_dual, coords={normal_dim: normal_dual})
 
         # Propagation phase at the primal and dual locations. The k-vector is along the propagation
         # direction, so angle_theta has to be taken into account. The distance along the propagation
         # direction is the distance along the normal direction over cosine(theta).
-        cos_theta = np.cos(self.mode_spec.angle_theta)
+        cos_theta = np.cos(mode_spec.angle_theta)
         k_vec = 2 * np.pi * n_complex * n_complex.f / C_0 / cos_theta
+        if direction == "-":
+            k_vec *= -1
         phase_primal = np.exp(1j * k_vec * (normal_primal - normal_pos))
         phase_dual = np.exp(1j * k_vec * (normal_dual - normal_pos))
 
         # Fields are modified by a linear interpolation to the exact monitor position
         if normal_primal.size > 1:
             phase_primal = phase_primal.interp(**{normal_dim: normal_pos})
         else:
@@ -482,15 +499,15 @@
 
     def to_source(
         self,
         source_time: SourceTime,
         direction: Direction,
         mode_index: pydantic.NonNegativeInt = 0,
     ) -> ModeSource:
-        """Creates :class:`.ModeSource` from a :class:`.ModeSolver` instance plus additional
+        """Creates :class:`.ModeSource` from a :class:`ModeSolver` instance plus additional
         specifications.
 
         Parameters
         ----------
         source_time: :class:`.SourceTime`
             Specification of the source time-dependence.
         direction : Direction
@@ -511,15 +528,15 @@
             source_time=source_time,
             mode_spec=self.mode_spec,
             mode_index=mode_index,
             direction=direction,
         )
 
     def to_monitor(self, freqs: List[float], name: str) -> ModeMonitor:
-        """Creates :class:`ModeMonitor` from a :class:`.ModeSolver` instance plus additional
+        """Creates :class:`ModeMonitor` from a :class:`ModeSolver` instance plus additional
         specifications.
 
         Parameters
         ----------
         freqs : List[float]
             Frequencies to include in Monitor (Hz).
         name : str
@@ -537,15 +554,15 @@
             size=self.plane.size,
             freqs=freqs,
             mode_spec=self.mode_spec,
             name=name,
         )
 
     def to_mode_solver_monitor(self, name: str) -> ModeSolverMonitor:
-        """Creates :class:`ModeSolverMonitor` from a :class:`.ModeSolver` instance.
+        """Creates :class:`ModeSolverMonitor` from a :class:`ModeSolver` instance.
 
         Parameters
         ----------
         name : str
             Name of the monitor.
 
         Returns
@@ -554,14 +571,15 @@
             Mode monitor with specifications taken from the ModeSolver instance and ``name``.
         """
         return ModeSolverMonitor(
             size=self.plane.size,
             center=self.plane.center,
             mode_spec=self.mode_spec,
             freqs=self.freqs,
+            direction=self.direction,
             name=name,
         )
 
     # pylint:disable=too-many-arguments
     def plot_field(
         self,
         field_name: str,
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/plugins/mode/solver.py` & `tidy3d-2.3.1/tidy3d/plugins/mode/solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Mode solver for propagating EM modes."""
 from typing import Tuple
 
 import numpy as np
 import scipy.sparse as sp
 import scipy.sparse.linalg as spl
 
-from ...components.types import Numpy, ModeSolverType
+from ...components.types import Numpy, ModeSolverType, EpsSpecType
 from ...components.base import Tidy3dBaseModel
 from ...constants import ETA_0, C_0, fp_eps, pec_val
 from .derivatives import create_d_matrices as d_mats
 from .derivatives import create_s_matrices as s_mats
 from .transforms import radial_transform, angled_transform
 
 # Consider vec to be complex if norm(vec.imag)/norm(vec) > TOL_COMPLEX
@@ -30,15 +30,16 @@
     def compute_modes(  # pylint:disable=too-many-arguments
         cls,
         eps_cross,
         coords,
         freq,
         mode_spec,
         symmetry=(0, 0),
-    ) -> Tuple[Numpy, Numpy]:
+        direction="+",
+    ) -> Tuple[Numpy, Numpy, EpsSpecType]:
         """Solve for the modes of a waveguide cross section.
 
         Parameters
         ----------
         eps_cross : array_like or tuple of array_like
             Either a single 2D array defining the relative permittivity in the cross-section,
             or nine 2D arrays defining the permittivity at the Ex, Ey, and Ez locations
@@ -47,20 +48,23 @@
             Two 1D arrays with each with size one larger than the corresponding axis of
             ``eps_cross``.
             Defines a (potentially non-uniform) Cartesian grid on which the modes are computed.
         freq : float
             (Hertz) Frequency at which the eigenmodes are computed.
         mode_spec : ModeSpec
             ``ModeSpec`` object containing specifications of the mode solver.
+        direction : Union["+", "-"]
+            Direction of mode propagation.
 
         Returns
         -------
-        Tuple[Numpy, Numpy]
-            The first array gives the E and H fields for all modes, the second one give sthe complex
-            effective index.
+        Tuple[Numpy, Numpy, str]
+            The first array gives the E and H fields for all modes, the second one gives the complex
+            effective index. The last variable describes permittivity characterization on the mode
+            solver's plane ("diagonal", "tensorial_real", or "tensorial_complex").
         """
 
         # freq += 0.0001j
         num_modes = mode_spec.num_modes
         bend_radius = mode_spec.bend_radius
         bend_axis = mode_spec.bend_axis
         angle_theta = mode_spec.angle_theta
@@ -162,23 +166,24 @@
             n_max = np.sqrt(np.max(np.abs(eps_physical)))
             target = n_max
         else:
             target = mode_spec.target_neff
         target_neff_p = target / np.linalg.norm(kp_to_k) + fp_eps
 
         # Solve for the modes
-        E, H, neff, keff = cls.solver_em(
+        E, H, neff, keff, eps_spec = cls.solver_em(
             Nx,
             Ny,
             eps_tensor,
             mu_tensor,
             der_mats,
             num_modes,
             target_neff_p,
             mode_spec.precision,
+            direction,
         )
 
         # Filter polarization if needed
         if mode_spec.filter_pol is not None:
             te_int = np.sum(np.abs(E[0]) ** 2, axis=0) / np.sum(np.abs(E[:2]) ** 2, axis=(0, 1))
             if mode_spec.filter_pol == "te":
                 sort_inds = np.concatenate(
@@ -195,22 +200,32 @@
 
         # Transform back to original axes, E = J^T E'
         E = np.sum(jac_e[..., None] * E[:, None, ...], axis=0)
         E = E.reshape((3, Nx, Ny, 1, num_modes))
         H = np.sum(jac_h[..., None] * H[:, None, ...], axis=0)
         H = H.reshape((3, Nx, Ny, 1, num_modes))
         neff = neff * np.linalg.norm(kp_to_k)
+        keff = keff * np.linalg.norm(kp_to_k)
 
         fields = np.stack((E, H), axis=0)
 
-        return fields, neff + 1j * keff
+        return fields, neff + 1j * keff, eps_spec
 
     @classmethod
     def solver_em(
-        cls, Nx, Ny, eps_tensor, mu_tensor, der_mats, num_modes, neff_guess, mat_precision
+        cls,
+        Nx,
+        Ny,
+        eps_tensor,
+        mu_tensor,
+        der_mats,
+        num_modes,
+        neff_guess,
+        mat_precision,
+        direction,
     ):  # pylint:disable=too-many-arguments
         """Solve for the electromagnetic modes of a system defined by in-plane permittivity and
         permeability and assuming translational invariance in the normal direction.
 
         Parameters
         ----------
         Nx : int
@@ -225,25 +240,29 @@
             The sparce derivative matrices dxf, dxb, dyf, dyb, including the PML.
         num_modes : int
             Number of modes to solve for.
         neff_guess : float
             Initial guess for the effective index.
         mat_precision : Union['single', 'double']
             Single or double-point precision in eigensolver.
+        direction : Union["+", "-"]
+            Direction of mode propagation.
 
         Returns
         -------
         E : np.ndarray
             Electric field of the eigenmodes, shape (3, N, num_modes).
         H : np.ndarray
             Magnetic field of the eigenmodes, shape (3, N, num_modes).
         neff : np.ndarray
             Real part of the effective index, shape (num_modes, ).
         keff : np.ndarray
             Imaginary part of the effective index, shape (num_modes, ).
+        eps_spec : Union["diagonal", "tensorial_real", "tensorial_complex"]
+            Permittivity characterization on the mode solver's plane.
         """
 
         # use a high-conductivity model for locations associated with a PEC
         def conductivity_model_for_pec(eps, threshold=0.9 * pec_val):
             """PEC entries associated with 'eps' are converted to a high-conductivity model."""
             eps = eps.astype(complex)
             eps[eps <= threshold] = 1 + 1j * np.abs(pec_val)
@@ -251,62 +270,94 @@
 
         eps_tensor = conductivity_model_for_pec(eps_tensor)
 
         # Determine if ``eps`` and ``mu`` are diagonal or tensorial
         off_diagonals = (np.ones((3, 3)) - np.eye(3)).astype(bool)
         eps_offd = np.abs(eps_tensor[off_diagonals])
         mu_offd = np.abs(mu_tensor[off_diagonals])
-        is_tensorial = False
-        if np.any(eps_offd > TOL_TENSORIAL) or np.any(mu_offd > TOL_TENSORIAL):
-            is_tensorial = True
+        is_tensorial = np.any(eps_offd > TOL_TENSORIAL) or np.any(mu_offd > TOL_TENSORIAL)
+
+        # initial vector for eigensolver in correct data type
+        vec_init = cls.set_initial_vec(Nx, Ny, is_tensorial=is_tensorial)
+
+        # call solver
+        kwargs = {
+            "eps": eps_tensor,
+            "mu": mu_tensor,
+            "der_mats": der_mats,
+            "num_modes": num_modes,
+            "neff_guess": neff_guess,
+            "vec_init": vec_init,
+            "mat_precision": mat_precision,
+        }
+
+        is_eps_complex = cls.isinstance_complex(eps_tensor)
+
+        if not is_tensorial:
+
+            eps_spec = "diagonal"
+            E, H, neff, keff = cls.solver_diagonal(**kwargs)
+            if direction == "-":
+                H[0] *= -1
+                H[1] *= -1
+                E[2] *= -1
+
+        elif not is_eps_complex:
+
+            eps_spec = "tensorial_real"
+            E, H, neff, keff = cls.solver_tensorial(**kwargs, direction="+")
+            if direction == "-":
+                E = np.conj(E)
+                H = -np.conj(H)
+
+        else:
+
+            eps_spec = "tensorial_complex"
+            E, H, neff, keff = cls.solver_tensorial(**kwargs, direction=direction)
 
-        # Determine data types
+        return E, H, neff, keff, eps_spec
+
+    # pylint:disable=too-many-arguments
+    @classmethod
+    def matrix_data_type(cls, eps, mu, der_mats, mat_precision, is_tensorial):
+        """Determine data type that should be used for the matrix for diagonalization."""
         mat_dtype = np.float32
         # In tensorial case, even though the matrix can be real, the
         # expected eigenvalue is purely imaginary. So for now we enforce
         # the matrix to be complex type so that it will look for the right eigenvalues.
         if is_tensorial:
             mat_dtype = np.complex128 if mat_precision == "double" else np.complex64
         else:
             # 1) check if complex or not
-            complex_solver = False
-            if (
-                cls.isinstance_complex(eps_tensor)
-                or cls.isinstance_complex(mu_tensor)
+            complex_solver = (
+                cls.isinstance_complex(eps)
+                or cls.isinstance_complex(mu)
                 or np.any([cls.isinstance_complex(f) for f in der_mats])
-            ):
-                complex_solver = True
+            )
             # 2) determine precision
             if complex_solver:
                 mat_dtype = np.complex128 if mat_precision == "double" else np.complex64
             else:
                 if mat_precision == "double":
                     mat_dtype = np.float64
 
-        # data type conversion
-        eps_tensor = cls.type_conversion(eps_tensor, mat_dtype)
-        mu_tensor = cls.type_conversion(mu_tensor, mat_dtype)
-        der_mats = [cls.type_conversion(f, mat_dtype) for f in der_mats]
-        neff_guess = cls.type_conversion(np.array([neff_guess]), mat_dtype)[0]
-
-        # initial vector for eigensolver
-        vec_init = cls.set_initial_vec(Nx, Ny, mat_dtype=mat_dtype, is_tensorial=is_tensorial)
-
-        # call solver
-        if is_tensorial:
-            return cls.solver_tensorial(
-                eps_tensor, mu_tensor, der_mats, num_modes, vec_init, neff_guess
-            )
+        return mat_dtype
 
-        return cls.solver_diagonal(eps_tensor, mu_tensor, der_mats, num_modes, vec_init, neff_guess)
+    @classmethod
+    def trim_small_values(cls, mat: sp.csr_matrix, tol: float) -> sp.csr_matrix:
+        """Eliminate elements of matrix ``mat`` for which ``abs(element) / abs(max_element) < tol``,
+        or ``np.abs(mat_data) < tol``. This operates in-place on mat so there is no return.
+        """
+        max_element = np.amax(np.abs(mat))
+        mat.data *= np.logical_or(np.abs(mat.data) / max_element > tol, np.abs(mat.data) > tol)
+        mat.eliminate_zeros()
 
+    # pylint:disable=too-many-arguments
     @classmethod
-    def solver_diagonal(
-        cls, eps, mu, der_mats, num_modes, vec_init, neff_guess
-    ):  # pylint:disable=too-many-arguments
+    def solver_diagonal(cls, eps, mu, der_mats, num_modes, neff_guess, vec_init, mat_precision):
         """EM eigenmode solver assuming ``eps`` and ``mu`` are diagonal everywhere."""
 
         # code associated with these options is included below in case it's useful in the future
         enable_incidence_matrices = False
         enable_preconditioner = False
         analyze_conditioning = False
 
@@ -355,17 +406,30 @@
         q11 = -dxb.dot(inv_mu_zz).dot(dyf)
         q12 = dxb.dot(inv_mu_zz).dot(dxf) + sp.spdiags(eps_yy, [0], N, N)
         q21 = -dyb.dot(inv_mu_zz).dot(dyf) - sp.spdiags(eps_xx, [0], N, N)
         q22 = dyb.dot(inv_mu_zz).dot(dxf)
 
         pmat = sp.bmat([[p11, p12], [p21, p22]])
         qmat = sp.bmat([[q11, q12], [q21, q22]])
-
         mat = pmat.dot(qmat)
 
+        # Cast matrix to target data type
+        mat_dtype = cls.matrix_data_type(eps, mu, der_mats, mat_precision, is_tensorial=False)
+        mat = cls.type_conversion(mat, mat_dtype)
+
+        # Trim small values in single precision case
+        if mat_precision == "single":
+            cls.trim_small_values(mat, tol=fp_eps)
+
+        # Casting starting vector to target data type
+        vec_init = cls.type_conversion(vec_init, mat_dtype)
+
+        # Starting eigenvalue guess in target data type
+        eig_guess = cls.type_conversion(np.array([-(neff_guess**2)]), mat_dtype)[0]
+
         if enable_incidence_matrices:
             mat = dnz * mat * dnz.T  # pylint: disable=used-before-assignment
             vec_init = dnz * vec_init  # pylint: disable=used-before-assignment
 
         if enable_preconditioner:
             precon = sp.diags(1 / mat.diagonal())
             mat = mat * precon
@@ -380,15 +444,15 @@
             print(spl.norm(diff, ord="fro"), spl.norm(aca, ord="fro"), spl.norm(aac, ord="fro"))
 
         # Call the eigensolver. The eigenvalues are -(neff + 1j * keff)**2
         vals, vecs = cls.solver_eigs(
             mat,
             num_modes,
             vec_init,
-            guess_value=-(neff_guess**2),
+            guess_value=eig_guess,
             mode_solver_type=mode_solver_type,
             M=precon,
         )
 
         if enable_preconditioner:
             vecs = precon * vecs
 
@@ -419,18 +483,19 @@
         H = np.stack((Hx, Hy, Hz), axis=0)
 
         # Return to standard H field units (see CEM notes for H normalization used in solver)
         H *= -1j / ETA_0
 
         return E, H, neff, keff
 
+    # pylint:disable=too-many-arguments
     @classmethod
     def solver_tensorial(
-        cls, eps, mu, der_mats, num_modes, vec_init, neff_guess
-    ):  # pylint:disable=too-many-arguments
+        cls, eps, mu, der_mats, num_modes, neff_guess, vec_init, mat_precision, direction
+    ):
         """EM eigenmode solver assuming ``eps`` or ``mu`` have off-diagonal elements."""
 
         mode_solver_type = "tensorial"
         N = eps.shape[-1]
         dxf, dxb, dyf, dyb = der_mats
 
         # Compute all blocks of the matrix for diagonalization
@@ -490,21 +555,42 @@
                 [axax, axay, axbx, axby],
                 [ayax, ayay, aybx, ayby],
                 [bxax, bxay, bxbx, bxby],
                 [byax, byay, bybx, byby],
             ]
         )
 
-        # Call the eigensolver. The eigenvalues are 1j * (neff + 1j * keff)
-        # Now multiply the matrix by -1j, so that eigenvalues are (neff + 1j * keff)
+        # The eigenvalues for the matrix above are 1j * (neff + 1j * keff)
+        # Multiply the matrix by -1j, so that eigenvalues are (neff + 1j * keff)
+        mat *= -1j
+
+        # change matrix sign for backward direction
+        if direction == "-":
+            mat *= -1
+
+        # Cast matrix to target data type
+        mat_dtype = cls.matrix_data_type(eps, mu, der_mats, mat_precision, is_tensorial=True)
+        mat = cls.type_conversion(mat, mat_dtype)
+
+        # Trim small values in single precision case
+        if mat_precision == "single":
+            cls.trim_small_values(mat, tol=fp_eps)
+
+        # Casting starting vector to target data type
+        vec_init = cls.type_conversion(vec_init, mat_dtype)
+
+        # Starting eigenvalue guess in target data type
+        eig_guess = cls.type_conversion(np.array([neff_guess]), mat_dtype)[0]
+
+        # Call the eigensolver.
         vals, vecs = cls.solver_eigs(
-            -1j * mat,
+            mat,
             num_modes,
             vec_init,
-            guess_value=neff_guess,
+            guess_value=eig_guess,
             mode_solver_type=mode_solver_type,
         )
         neff, keff = cls.eigs_to_effective_index(vals, mode_solver_type)
         # Sort by descending real part
         sort_inds = np.argsort(neff)[::-1]
         neff = neff[sort_inds]
         keff = keff[sort_inds]
@@ -592,43 +678,40 @@
         if new_dtype in {np.float64, np.float32}:
             converted_vec_or_mat = vec_or_mat.real
             return converted_vec_or_mat.astype(new_dtype)
 
         raise RuntimeError("Unsupported new_type.")
 
     @classmethod
-    def set_initial_vec(cls, Nx, Ny, mat_dtype=np.complex128, is_tensorial=False):
+    def set_initial_vec(cls, Nx, Ny, is_tensorial=False):
         """Set initial vector for eigs:
         1) The field at x=0 and y=0 boundaries are set to 0. This should be
         the case for PEC boundaries, but wouldn't hurt for non-PEC boundary;
         2) The vector is np.complex128 by default, and will be converted to
         approriate type afterwards.
 
         Parameters
         ----------
         Nx : int
             Number of grids along x-direction.
         Ny : int
             Number of grids along y-direction.
-        mat_dtype : Union[np.complex128, np.complex64, np.float64, np.float32]
-            The type of returned vector.
         is_tensorial : bool
             diagonal or tensorial eigenvalue problem.
         """
 
         # The size of the vector is len_multiplier * Nx * Ny
         len_multiplier = 2
         if is_tensorial:
             len_multiplier *= 2
 
         # Initialize the vector
         size = (Nx, Ny, len_multiplier)
         rng = np.random.default_rng(0)
         vec_init = rng.random(size) + 1j * rng.random(size)
-        vec_init = cls.type_conversion(vec_init, mat_dtype)
 
         # Set values at the boundary to be 0
         if Nx > 1:
             vec_init[0, :, :] = 0
         if Ny > 1:
             vec_init[:, 0, :] = 0
 
@@ -666,10 +749,10 @@
             neff = np.sqrt(vre / 2 + np.sqrt(vre**2 + vim**2) / 2)
             keff = vim / 2 / (neff + 1e-10)
             return neff, keff
 
         raise RuntimeError(f"Unidentified 'mode_solver_type={mode_solver_type}'.")
 
 
-def compute_modes(*args, **kwargs) -> Tuple[Numpy, Numpy]:
+def compute_modes(*args, **kwargs) -> Tuple[Numpy, Numpy, str]:
     """A wrapper around ``EigSolver.compute_modes``, which is used in ``ModeSolver``."""
     return EigSolver.compute_modes(*args, **kwargs)
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/plugins/mode/transforms.py` & `tidy3d-2.3.1/tidy3d/plugins/mode/transforms.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/plugins/polyslab/polyslab.py` & `tidy3d-2.3.1/tidy3d/plugins/polyslab/polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/plugins/resonance/resonance.py` & `tidy3d-2.3.1/tidy3d/plugins/resonance/resonance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/plugins/smatrix/smatrix.py` & `tidy3d-2.3.1/tidy3d/plugins/smatrix/smatrix.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 """Tools for generating an S matrix automatically from tidy3d simulation and port definitions."""
+from __future__ import annotations
 
-from typing import List, Tuple, Optional, Callable, Dict
+from typing import List, Tuple, Optional, Dict
+import os
 
 import pydantic as pd
 import numpy as np
 
 from ...constants import HERTZ, C_0
 from ...components.simulation import Simulation
 from ...components.geometry import Box
 from ...components.mode import ModeSpec
 from ...components.monitor import ModeMonitor
 from ...components.source import ModeSource, GaussianPulse
 from ...components.data.sim_data import SimulationData
 from ...components.data.data_array import DataArray
 from ...components.types import Direction, Ax, Complex
 from ...components.viz import add_ax_if_none, equal_aspect
-from ...components.base import Tidy3dBaseModel
+from ...components.base import Tidy3dBaseModel, cached_property
 from ...exceptions import SetupError, Tidy3dKeyError
-from ...web.container import Batch, BatchData
-
+from ...log import log
+from ...web.container import BatchData, Batch
 
 # fwidth of gaussian pulse in units of central frequency
 FWIDTH_FRAC = 1.0 / 10
-DEFAULT_DATA_DIR = "data"
+DEFAULT_DATA_DIR = "."
 
 
 class Port(Box):
     """Specifies a port in the scattering matrix."""
 
     direction: Direction = pd.Field(
         ...,
@@ -122,169 +124,135 @@
         "the data corresponding to other inputs will be missing in the resulting matrix.",
     )
     verbose: bool = pd.Field(
         False,
         title="Verbosity",
         description="Whether the :class:`.ComponentModeler` should print status and progressbars.",
     )
-    batch: Optional[Batch] = pd.Field(
+    callback_url: str = pd.Field(
         None,
-        title="Batch",
-        description="Batch of generated simulations needed for each row of the scattering matrix."
-        "Should be left ``None`` in almost all cases, which will generate the proper batch "
-        "internally and store it as ``ComponentModeler.batch``.",
+        title="Callback URL",
+        description="Http PUT url to receive simulation finish event. "
+        "The body content is a json file with fields "
+        "``{'id', 'status', 'name', 'workUnit', 'solverVersion'}``.",
+    )
+    path_dir: str = pd.Field(
+        DEFAULT_DATA_DIR,
+        title="Directory Path",
+        description="Base directory where data and batch will be downloaded.",
     )
 
     @pd.validator("simulation", always=True)
     def _sim_has_no_sources(cls, val):
         """Make sure simulation has no sources as they interfere with tool."""
         if len(val.sources) > 0:
             raise SetupError("'ComponentModeler.simulation' must not have any sources.")
         return val
 
-    @pd.validator("batch", always=True)
-    def _set_batch(cls, val, values):
-        """Initialize the batch if not supplied."""
-
-        # if supplied, return it
-        if val is not None:
-            return val
-
-        # otherwise, generate all sims and make a new batch
-        sim_dict = cls.make_sim_dict(values=values)
-        return Batch(
-            simulations=sim_dict,
-            folder_name=values.get("folder_name"),
-            verbose=values.get("verbose"),
-        )
-
-    @classmethod
-    def make_sim_dict(cls, values: dict) -> Dict[str, Simulation]:
+    @cached_property
+    def sim_dict(self) -> Dict[str, Simulation]:
         """Generate all the :class:`Simulation` objects for the S matrix calculation."""
 
         sim_dict = {}
-        ports = values.get("ports")
-        simulation = values.get("simulation")
-        freqs = values.get("freqs")
-
-        mode_monitors = [
-            cls._to_monitor(port=port, freqs=freqs) for port in ports
-        ]  # pylint:disable=protected-access
-
-        for (port_name, mode_index) in cls.matrix_indices_run_sim(
-            ports=ports,
-            run_only=values.get("run_only"),
-            element_mappings=values.get("element_mappings"),
-        ):
-
-            port = cls.get_port_by_name(port_name=port_name, ports=ports)
-
-            port_source = cls._shift_port(
-                simulation=simulation, port=port
-            )  # pylint:disable=protected-access
-            mode_source = cls._to_source(
-                port=port_source, mode_index=mode_index, freqs=freqs
-            )  # pylint:disable=protected-access
-
-            new_mnts = list(simulation.monitors) + mode_monitors
-            sim_copy = simulation.copy(update=dict(sources=[mode_source], monitors=new_mnts))
-            task_name = cls._task_name(port=port, mode_index=mode_index)
+        mode_monitors = [self.to_monitor(port=port) for port in self.ports]
+
+        for (port_name, mode_index) in self.matrix_indices_run_sim:
+
+            port = self.get_port_by_name(port_name=port_name)
+
+            port_source = self.shift_port(port=port)
+            mode_source = self.to_source(port=port_source, mode_index=mode_index)
+
+            new_mnts = list(self.simulation.monitors) + mode_monitors
+            sim_copy = self.simulation.copy(update=dict(sources=[mode_source], monitors=new_mnts))
+            task_name = self._task_name(port=port, mode_index=mode_index)
             sim_dict[task_name] = sim_copy
         return sim_dict
 
-    @classmethod
-    def matrix_indices_monitor(cls, ports: Tuple[Port, ...]) -> Tuple[MatrixIndex, ...]:
+    @cached_property
+    def matrix_indices_monitor(self) -> Tuple[MatrixIndex, ...]:
         """Tuple of all the possible matrix indices (port, mode_index) in the Component Modeler."""
         matrix_indices = []
-        for port in ports:
+        for port in self.ports:
             for mode_index in range(port.mode_spec.num_modes):
                 matrix_indices.append((port.name, mode_index))
         return tuple(matrix_indices)
 
-    @classmethod
-    def matrix_indices_source(
-        cls, ports: Tuple[Port, ...], run_only: Tuple[MatrixIndex, ...] = None
-    ) -> Tuple[MatrixIndex, ...]:
+    @cached_property
+    def matrix_indices_source(self) -> Tuple[MatrixIndex, ...]:
         """Tuple of all the source matrix indices (port, mode_index) in the Component Modeler."""
-        return run_only if run_only is not None else cls.matrix_indices_monitor(ports=ports)
+        if self.run_only is not None:
+            return self.run_only
+        return self.matrix_indices_monitor
 
-    @classmethod
-    def matrix_indices_run_sim(
-        cls,
-        ports: Tuple[Port, ...],
-        element_mappings: Dict[Element, Dict[Element, Callable[[complex], complex]]] = None,
-        run_only: Tuple[MatrixIndex, ...] = None,
-    ) -> Tuple[MatrixIndex, ...]:
+    @cached_property
+    def matrix_indices_run_sim(self) -> Tuple[MatrixIndex, ...]:
         """Tuple of all the source matrix indices (port, mode_index) in the Component Modeler."""
 
-        if element_mappings is None or element_mappings == {}:
-            return cls.matrix_indices_source(ports=ports, run_only=run_only)
+        if self.element_mappings is None or self.element_mappings == {}:
+            return self.matrix_indices_source
 
         # all the (i, j) pairs in `S_ij` that are tagged as covered by `element_mappings`
-        elements_determined_by_map = [element_out for (_, element_out, _) in element_mappings]
+        elements_determined_by_map = [element_out for (_, element_out, _) in self.element_mappings]
 
         # loop through rows of the full s matrix and record rows that still need running.
         source_indices_needed = []
-        for col_index in cls.matrix_indices_source(ports=ports, run_only=run_only):
+        for col_index in self.matrix_indices_source:
 
             # loop through columns and keep track of whether each element is covered by mapping.
             matrix_elements_covered = []
-            for row_index in cls.matrix_indices_monitor(ports=ports):
+            for row_index in self.matrix_indices_monitor:
                 element = (row_index, col_index)
                 element_covered_by_map = element in elements_determined_by_map
                 matrix_elements_covered.append(element_covered_by_map)
 
             # if any matrix elements in row still not covered by map, a source is needed for row.
             if not all(matrix_elements_covered):
                 source_indices_needed.append(col_index)
 
         return source_indices_needed
 
-    @staticmethod
-    def get_port_by_name(ports: Tuple[Port, ...], port_name: str) -> Port:
+    def get_port_by_name(self, port_name: str) -> Port:
         """Get the port from the name."""
-        ports = [port for port in ports if port.name == port_name]
+        ports = [port for port in self.ports if port.name == port_name]
         if len(ports) == 0:
             raise Tidy3dKeyError(f'Port "{port_name}" not found.')
         return ports[0]
 
-    @staticmethod
-    def _to_monitor(port: Port, freqs: List[float]) -> ModeMonitor:
+    def to_monitor(self, port: Port) -> ModeMonitor:
         """Creates a mode monitor from a given port."""
         return ModeMonitor(
             center=port.center,
             size=port.size,
-            freqs=freqs,
+            freqs=self.freqs,
             mode_spec=port.mode_spec,
             name=port.name,
         )
 
-    @staticmethod
-    def _to_source(port: Port, mode_index: int, freqs: List[float]) -> List[ModeSource]:
+    def to_source(self, port: Port, mode_index: int) -> List[ModeSource]:
         """Creates a list of mode sources from a given port."""
-        freq0 = np.mean(freqs)
-        fdiff = max(freqs) - min(freqs)
+        freq0 = np.mean(self.freqs)
+        fdiff = max(self.freqs) - min(self.freqs)
         fwidth = max(fdiff, freq0 * FWIDTH_FRAC)
         return ModeSource(
             center=port.center,
             size=port.size,
             source_time=GaussianPulse(freq0=freq0, fwidth=fwidth),
             mode_spec=port.mode_spec,
             mode_index=mode_index,
             direction=port.direction,
             name=port.name,
         )
 
-    @staticmethod
-    def _shift_value_signed(simulation: Simulation, port: Port) -> float:
+    def _shift_value_signed(self, port: Port) -> float:
         """How far (signed) to shift the source from the monitor."""
 
         # get the grid boundaries and sizes along port normal from the simulation
         normal_axis = port.size.index(0.0)
-        grid = simulation.grid
+        grid = self.simulation.grid
         grid_boundaries = grid.boundaries.to_list[normal_axis]
         grid_centers = grid.centers.to_list[normal_axis]
 
         # get the index of the grid cell where the port lies
         port_position = port.center[normal_axis]
         port_pos_gt_grid_bounds = np.argwhere(port_position > grid_boundaries)
 
@@ -310,19 +278,18 @@
                     f"Port {port.name} normal is too close to boundary "
                     f"on +{'xyz'[normal_axis]} side."
                 )
 
         new_pos = grid_centers[shifted_index]
         return new_pos - port_position
 
-    @classmethod
-    def _shift_port(cls, simulation: Simulation, port: Port) -> Port:
+    def shift_port(self, port: Port) -> Port:
         """Generate a new port shifted by the shift amount in normal direction."""
 
-        shift_value = cls._shift_value_signed(simulation=simulation, port=port)
+        shift_value = self._shift_value_signed(port=port)
         center_shifted = list(port.center)
         center_shifted[port.size.index(0.0)] += shift_value
         port_shifted = port.copy(update=dict(center=center_shifted))
         return port_shifted
 
     @staticmethod
     def _task_name(port: Port, mode_index: int) -> str:
@@ -332,24 +299,68 @@
     @equal_aspect
     @add_ax_if_none
     def plot_sim(self, x: float = None, y: float = None, z: float = None, ax: Ax = None) -> Ax:
         """Plot a :class:`Simulation` with all sources added for each port, for troubleshooting."""
 
         plot_sources = []
         for port_source in self.ports:
-            mode_source_0 = self._to_source(port=port_source, freqs=self.freqs, mode_index=0)
+            mode_source_0 = self.to_source(port=port_source, mode_index=0)
             plot_sources.append(mode_source_0)
         sim_plot = self.simulation.copy(update=dict(sources=plot_sources))
         return sim_plot.plot(x=x, y=y, z=z, ax=ax)
 
-    def _run_sims(self, path_dir: str) -> BatchData:
+    @cached_property
+    def batch(self) -> Batch:
+        """Batch associated with this component modeler."""
+
+        # first try loading the batch from file, if it exists
+        batch_path = self._batch_path
+        if os.path.exists(batch_path):
+            return Batch.from_file(fname=batch_path)
+
+        return Batch(
+            simulations=self.sim_dict,
+            folder_name=self.folder_name,
+            callback_url=self.callback_url,
+            verbose=self.verbose,
+        )
+
+    @cached_property
+    def batch_path(self) -> str:
+        """Path to the batch saved to file."""
+        # pylint: disable=protected-access
+        return self.batch._batch_path(path_dir=DEFAULT_DATA_DIR)
+
+    def get_path_dir(self, path_dir: str) -> None:
+        """Check whether the supplied 'path_dir' matches the internal field value."""
+
+        if path_dir not in (DEFAULT_DATA_DIR, self.path_dir):
+            log.warning(
+                f"'ComponentModeler' method was supplied a 'path_dir' of '{path_dir}' "
+                f"when its internal 'path_dir' field was set to '{self.path_dir}'. "
+                "The passed value will be deprecated in later versions. "
+                "Please set the internal 'path_dir' field to the desired value and "
+                "remove the 'path_dir' from the method argument. "
+                f"Using supplied '{path_dir}'."
+            )
+            return path_dir
+
+        return self.path_dir
+
+    @cached_property
+    def _batch_path(self) -> str:
+        """Where we store the batch for this ComponentModeler instance after the run."""
+        return os.path.join(self.path_dir, "batch" + str(hash(self)) + ".json")
+
+    def _run_sims(self, path_dir: str = DEFAULT_DATA_DIR) -> BatchData:
         """Run :class:`Simulations` for each port and return the batch after saving."""
-        self.batch.start()
-        self.batch.monitor()
-        return self.batch.load(path_dir=path_dir)
+        batch = self.batch
+        batch_data = batch.run(path_dir=path_dir)
+        batch.to_file(self._batch_path)
+        return batch_data
 
     def _normalization_factor(self, port_source: Port, sim_data: SimulationData) -> complex:
         """Compute the normalization amplitude based on the measured input mode amplitude."""
 
         port_monitor_data = sim_data[port_source.name]
         mode_index = sim_data.simulation.sources[0].mode_index
 
@@ -359,57 +370,50 @@
             mode_index=mode_index,
         ).values
 
         normalize_n_eff = port_monitor_data.n_eff.sel(f=self.freqs, mode_index=mode_index).values
 
         k0s = 2 * np.pi * C_0 / np.array(self.freqs)
         k_effs = k0s * normalize_n_eff
-        shift_value = self._shift_value_signed(simulation=self.simulation, port=port_source)
+        shift_value = self._shift_value_signed(port=port_source)
         return normalize_amps * np.exp(1j * k_effs * shift_value)
 
-    @property
+    @cached_property
     def max_mode_index(self) -> Tuple[int, int]:
         """maximum mode indices for the smatrix dataset for the in and out ports, respectively."""
 
         def get_max_mode_indices(matrix_elements: Tuple[str, int]) -> int:
             """Get the maximum mode index for a list of (port name, mode index)."""
             return max(mode_index for _, mode_index in matrix_elements)
 
-        matrix_elements_out = self.matrix_indices_monitor(ports=self.ports)
-        matrix_elements_in = self.matrix_indices_source(ports=self.ports, run_only=self.run_only)
-
-        max_mode_index_out = get_max_mode_indices(matrix_elements_out)
-        max_mode_index_in = get_max_mode_indices(matrix_elements_in)
+        max_mode_index_out = get_max_mode_indices(self.matrix_indices_monitor)
+        max_mode_index_in = get_max_mode_indices(self.matrix_indices_source)
 
         return max_mode_index_out, max_mode_index_in
 
-    @property
+    @cached_property
     def port_names(self) -> Tuple[List[str], List[str]]:
         """List of port names for inputs and outputs, respectively."""
 
         def get_port_names(matrix_elements: Tuple[str, int]) -> List[str]:
             """Get the port names from a list of (port name, mode index)."""
             port_names = []
             for port_name, _ in matrix_elements:
                 if port_name not in port_names:
                     port_names.append(port_name)
             return port_names
 
-        matrix_elements_in = self.matrix_indices_source(ports=self.ports, run_only=self.run_only)
-        matrix_elements_out = self.matrix_indices_monitor(ports=self.ports)
-
-        port_names_in = get_port_names(matrix_elements_in)
-        port_names_out = get_port_names(matrix_elements_out)
+        port_names_in = get_port_names(self.matrix_indices_source)
+        port_names_out = get_port_names(self.matrix_indices_monitor)
 
         return port_names_out, port_names_in
 
-    def _construct_smatrix(  # pylint:disable=too-many-locals
-        self, batch_data: BatchData
-    ) -> SMatrixDataArray:
-        """Post process batch to generate scattering matrix."""
+    # pylint:disable=too-many-locals
+    def _construct_smatrix(self, batch_data: BatchData) -> SMatrixDataArray:
+        """Post process `BatchData` to generate scattering matrix."""
 
         max_mode_index_out, max_mode_index_in = self.max_mode_index
         num_modes_out = max_mode_index_out + 1
         num_modes_in = max_mode_index_in + 1
         port_names_out, port_names_in = self.port_names
 
         values = np.zeros(
@@ -423,27 +427,25 @@
             mode_index_in=range(num_modes_in),
             f=self.freqs,
         )
 
         s_matrix = SMatrixDataArray(values, coords=coords)
 
         # loop through source ports
-        for col_index in self.matrix_indices_run_sim(
-            ports=self.ports, run_only=self.run_only, element_mappings=self.element_mappings
-        ):
+        for col_index in self.matrix_indices_run_sim:
 
             port_name_in, mode_index_in = col_index
-            port_in = self.get_port_by_name(port_name=port_name_in, ports=self.ports)
+            port_in = self.get_port_by_name(port_name=port_name_in)
 
             sim_data = batch_data[self._task_name(port=port_in, mode_index=mode_index_in)]
 
-            for row_index in self.matrix_indices_monitor(ports=self.ports):
+            for row_index in self.matrix_indices_monitor:
 
                 port_name_out, mode_index_out = row_index
-                port_out = self.get_port_by_name(port_name=port_name_out, ports=self.ports)
+                port_out = self.get_port_by_name(port_name=port_name_out)
 
                 # directly compute the element
                 mode_amps_data = sim_data[port_out.name].copy().amps
                 dir_out = "-" if port_out.direction == "+" else "+"
                 amp = mode_amps_data.sel(f=self.freqs, direction=dir_out, mode_index=mode_index_out)
                 source_norm = self._normalization_factor(port_in, sim_data)
                 s_matrix_elements = np.array(amp.data) / np.array(source_norm)
@@ -478,18 +480,18 @@
             )
             s_matrix.loc[coords_to] = mult_by * s_matrix.loc[coords_from].values
 
         return s_matrix
 
     def run(self, path_dir: str = DEFAULT_DATA_DIR) -> SMatrixDataArray:
         """Solves for the scattering matrix of the system."""
+        path_dir = self.get_path_dir(path_dir)
 
         batch_data = self._run_sims(path_dir=path_dir)
         return self._construct_smatrix(batch_data=batch_data)
 
     def load(self, path_dir: str = DEFAULT_DATA_DIR) -> SMatrixDataArray:
-        """Load an Smatrix from saved BatchData object."""
+        """Load a scattering matrix from saved `BatchData` object."""
+        path_dir = self.get_path_dir(path_dir)
 
-        if self.batch is None:
-            raise SetupError("Component modeler has no batch saved. Run .run() to generate.")
-        batch_data = self.batch.load(path_dir=path_dir)
+        batch_data = BatchData.load(path_dir=path_dir)
         return self._construct_smatrix(batch_data=batch_data)
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/plugins/waveguide/rectangular_dielectric.py` & `tidy3d-2.3.1/tidy3d/plugins/waveguide/rectangular_dielectric.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 from ...components.boundary import BoundarySpec, Periodic
 from ...components.data.data_array import ModeIndexDataArray, FreqModeDataArray
 from ...components.geometry import Box, PolySlab
 from ...components.grid.grid_spec import GridSpec
 from ...components.medium import Medium, MediumType
 from ...components.mode import ModeSpec
 from ...components.simulation import Simulation
+
 from ...components.source import ModeSource, GaussianPulse
 from ...components.structure import Structure
 from ...components.types import ArrayFloat1D, Ax, Axis, Coordinate, Literal, Size1D, Union
+from ...components.types import TYPE_TAG_STR
 from ...constants import C_0, inf, MICROMETER, RADIAN
 from ...exceptions import Tidy3dError, ValidationError
 from ...log import log
 
 from ..mode.mode_solver import ModeSolver
 
 
@@ -56,26 +58,29 @@
         units=MICROMETER,
     )
 
     core_medium: MediumType = pydantic.Field(
         ...,
         title="Core Medium",
         description="Medium associated with the core layer.",
+        discriminator=TYPE_TAG_STR,
     )
 
     clad_medium: MediumType = pydantic.Field(
         ...,
         title="Clad Medium",
         description="Medium associated with the upper cladding layer.",
+        discriminator=TYPE_TAG_STR,
     )
 
     box_medium: MediumType = pydantic.Field(
         None,
         title="Box Medium",
         description="Medium associated with the lower cladding layer.",
+        discriminator=TYPE_TAG_STR,
     )
 
     slab_thickness: Size1D = pydantic.Field(
         0.0,
         title="Slab Thickness",
         description="Thickness of the slab for rib geometry.",
         units=MICROMETER,
@@ -126,28 +131,30 @@
         units=MICROMETER,
     )
 
     sidewall_medium: MediumType = pydantic.Field(
         None,
         title="Sidewall medium",
         description="Medium associated with the sidewall layer to model sidewall losses.",
+        discriminator=TYPE_TAG_STR,
     )
 
     surface_thickness: Size1D = pydantic.Field(
         0.0,
         title="Surface Thickness",
         description="Thickness of the surface layers defined on the top of the waveguide and  "
         "slab regions (if any).",
         units=MICROMETER,
     )
 
     surface_medium: MediumType = pydantic.Field(
         None,
         title="Surface Medium",
         description="Medium associated with the surface layer to model surface losses.",
+        discriminator=TYPE_TAG_STR,
     )
 
     origin: Coordinate = pydantic.Field(
         (0, 0, 0),
         title="Origin",
         description="Center of the waveguide geometry.  This coordinate represents the base "
         "of the waveguides (substrate surface) in the normal axis, and center of the geometry "
@@ -171,15 +178,15 @@
     normal_axis: Axis = pydantic.Field(
         2,
         title="Normal Axis",
         description="Axis normal to the substrate surface",
     )
 
     mode_spec: ModeSpec = pydantic.Field(
-        ModeSpec(num_modes=2, precision="double"),
+        ModeSpec(num_modes=2),
         title="Mode Specification",
         description=":class:`ModeSpec` defining waveguide mode properties.",
     )
 
     grid_resolution: int = pydantic.Field(
         15,
         title="Grid Resolution",
@@ -626,25 +633,29 @@
         ... )
         >>> mode_data = wg.mode_solver.solve()
         >>> mode_data.n_eff.values
         array([[2.4536054 1.7850305]], dtype=float32)
 
         """
         freqs = C_0 / self.wavelength
+        f_max = freqs.max()
+        f_min = freqs.min()
+        freq0 = 0.5 * (f_max + f_min)
+        fwidth = max(0.1 * freq0, f_max - f_min)
 
         plane = Box(
             center=self._translate(0, 0.5 * self.height - self.box_thickness, 0),
             size=self._swap_axis(self.width, self.height, 0),
         )
 
         # Source used only to silence warnings
         mode_source = ModeSource(
             center=plane.center,
             size=plane.size,
-            source_time=GaussianPulse(freq0=freqs[0], fwidth=freqs[0] / 10),
+            source_time=GaussianPulse(freq0=freq0, fwidth=fwidth),
             direction="+",
             mode_spec=self.mode_spec,
         )
 
         simulation = Simulation(
             center=plane.center,
             size=plane.size,
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/updater.py` & `tidy3d-2.3.1/tidy3d/updater.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/web/asynchronous.py` & `tidy3d-2.3.1/tidy3d/web/asynchronous.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/web/cacert.pem` & `tidy3d-2.3.1/tidy3d/web/cacert.pem`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/web/cli/app.py` & `tidy3d-2.3.1/tidy3d/web/cli/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 Commandline interface for tidy3d.
 """
 import json
 import os.path
+import ssl
 
 import click
 import requests
 import toml
 
 from tidy3d.web.cli.constants import TIDY3D_DIR, CONFIG_FILE, CREDENTIAL_FILE
 from tidy3d.web.cli.migrate import migrate
-from tidy3d.web.config import DEFAULT_CONFIG
+from tidy3d.web.environment import Env
 
 if not os.path.exists(TIDY3D_DIR):
     os.mkdir(TIDY3D_DIR)
 
 
 def get_description():
     """Get the description for the config command.
@@ -86,15 +87,21 @@
                 return
 
     if not apikey:
         current_apikey = get_description()
         message = f"Current API key: [{current_apikey}]\n" if current_apikey else ""
         apikey = click.prompt(f"{message}Please enter your api key", type=str)
 
-    resp = requests.get(f"{DEFAULT_CONFIG.web_api_endpoint}/apikey", auth=auth, verify=False)
+    try:
+        resp = requests.get(
+            f"{Env.current.web_api_endpoint}/apikey", auth=auth, verify=Env.current.ssl_verify
+        )
+    except (requests.exceptions.SSLError, ssl.SSLError):
+        resp = requests.get(f"{Env.current.web_api_endpoint}/apikey", auth=auth, verify=False)
+
     if resp.status_code == 200:
         click.echo("Configured successfully.")
         with open(CONFIG_FILE, "w+", encoding="utf-8") as config_file:
             toml_config = toml.loads(config_file.read())
             toml_config.update({"apikey": apikey})
             config_file.write(toml.dumps(toml_config))
     else:
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/web/cli/migrate.py` & `tidy3d-2.3.1/tidy3d/web/cli/migrate.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 import click
 import requests
 import toml
 
 from tidy3d.web.cli.constants import CONFIG_FILE, CREDENTIAL_FILE, TIDY3D_DIR
-from tidy3d.web.config import DEFAULT_CONFIG
+from tidy3d.web.environment import Env
 
 
 # disable pylint for this file
 # pylint: disable-all
 
 
 def migrate() -> bool:
@@ -31,37 +31,35 @@
                 "workings of Tidy3D will remain the same.",
                 type=bool,
                 default=True,
             )
             if is_migrate:
                 headers = {"Application": "TIDY3D"}
                 resp = requests.get(
-                    f"{DEFAULT_CONFIG.auth_api_endpoint}/auth",
+                    f"{Env.current.auth_api_endpoint}/auth",
                     headers=headers,
                     auth=(email, password),
                 )
                 if resp.status_code != 200:
                     click.echo(f"Migrate to api key failed: {resp.text}")
                     return False
                 else:
                     # click.echo(json.dumps(resp.json(), indent=4))
                     access_token = resp.json()["data"]["auth"]["accessToken"]
                     headers["Authorization"] = f"Bearer {access_token}"
-                    resp = requests.get(
-                        f"{DEFAULT_CONFIG.web_api_endpoint}/apikey", headers=headers
-                    )
+                    resp = requests.get(f"{Env.current.web_api_endpoint}/apikey", headers=headers)
                     if resp.status_code != 200:
                         click.echo(f"Migrate to api key failed: {resp.text}")
                         return False
                     else:
                         click.echo(json.dumps(resp.json(), indent=4))
                         apikey = resp.json()["data"]
                         if not apikey:
                             resp = requests.post(
-                                f"{DEFAULT_CONFIG.web_api_endpoint}/apikey", headers=headers
+                                f"{Env.current.web_api_endpoint}/apikey", headers=headers
                             )
                             if resp.status_code != 200:
                                 click.echo(f"Migrate to api key failed: {resp.text}")
                                 return False
                             else:
                                 apikey = resp.json()["data"]
                         if not os.path.exists(TIDY3D_DIR):
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/web/container.py` & `tidy3d-2.3.1/tidy3d/web/container.py`

 * *Files 4% similar despite different names*

```diff
@@ -191,22 +191,42 @@
         Returns
         -------
         :class:`.SimulationData`
             Object containing data about simulation.
         """
         return web.load(task_id=self.task_id, path=path, verbose=self.verbose)
 
-    def delete(self):
+    def delete(self) -> None:
         """Delete server-side data associated with :class:`Job`."""
         web.delete(self.task_id)
 
-    def real_cost(self):
+    def real_cost(self) -> float:
         """Get the billed cost for the task associated with this job."""
         return web.real_cost(self.task_id)
 
+    def estimate_cost(self) -> float:
+        """Compute the maximum FlexCredit charge for a given :class:`.Job`.
+
+        Returns
+        -------
+        float
+            Estimated maximum cost for :class:`.Simulation` associated with given ``Job``.
+
+        Note
+        ----
+        Cost is calculated assuming the simulation runs for
+        the full ``run_time``. If early shut-off is triggered, the cost is adjusted proporionately.
+
+        Returns
+        -------
+        float
+            Estimated cost of the task in FlexCredits.
+        """
+        return web.estimate_cost(self.task_id)
+
 
 class BatchData(Tidy3dBaseModel):
     """Holds a collection of :class:`.SimulationData` returned by :class:`.Batch`."""
 
     task_paths: Dict[TaskName, str] = pd.Field(
         ...,
         title="Data Paths",
@@ -452,14 +472,22 @@
         ]
         end_statuses = ("success", "error", "errored", "diverged", "diverge", "deleted", "draft")
 
         if self.verbose:
             console = Console()
             console.log("Started working on Batch.")
 
+            est_flex_unit = self.estimate_cost()
+            if est_flex_unit is not None and est_flex_unit > 0:
+                console.log(
+                    f"Maximum FlexCredit cost: {est_flex_unit:1.3f} for the whole batch. "
+                    "Use 'Batch.real_cost()' to "
+                    "get the billed FlexCredit cost after the Batch has completed."
+                )
+
             with Progress(console=console) as progress:
 
                 # create progressbars
                 pbar_tasks = {}
                 for task_name, job in self.jobs.items():
                     status = job.status
                     description = pbar_description(task_name, status)
@@ -594,20 +622,40 @@
                 continue
 
             task_paths[task_name] = self._job_data_path(task_id=job.task_id, path_dir=path_dir)
             task_ids[task_name] = self.jobs[task_name].task_id
 
         return BatchData(task_paths=task_paths, task_ids=task_ids, verbose=self.verbose)
 
-    def delete(self):
+    def delete(self) -> None:
         """Delete server-side data associated with each task in the batch."""
         for _, job in self.jobs.items():
             job.delete()
 
-    def real_cost(self):
+    def real_cost(self) -> float:
         """Get the sum of billed costs for each task associated with this batch."""
         real_cost_sum = 0.0
         for _, job in self.jobs.items():
             cost_job = job.real_cost()
             if cost_job is not None:
                 real_cost_sum += cost_job
         return real_cost_sum or None
+
+    def estimate_cost(self) -> float:
+        """Compute the maximum FlexCredit charge for a given :class:`.Batch`.
+
+        Returns
+        -------
+        float
+            Estimated maximum cost for each :class:`.Simulation` associated with given ``Batch``.
+
+        Note
+        ----
+        Cost is calculated assuming the simulation runs for
+        the full ``run_time``. If early shut-off is triggered, the cost is adjusted proporionately.
+
+        Returns
+        -------
+        float
+            Estimated total cost of the tasks in FlexCredits.
+        """
+        return sum(job.estimate_cost() for _, job in self.jobs.items())
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/web/http_management.py` & `tidy3d-2.3.1/tidy3d/web/http_management.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/web/httputils.py` & `tidy3d-2.3.1/tidy3d/web/httputils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import jwt
 import toml
 from requests import Session
 import requests
 
 from .cli.constants import CONFIG_FILE
-from .config import DEFAULT_CONFIG as Config
+from .environment import Env
 from ..exceptions import WebError
 from ..version import __version__
 
 SIMCLOUD_APIKEY = "SIMCLOUD_APIKEY"
 
 
 def api_key():
@@ -64,15 +64,15 @@
         "API key not found, please set it by commandline or environment,"
         " eg: tidy3d configure or export "
         "SIMCLOUD_APIKEY=xxx"
     )
 
 
 session = Session()
-session.verify = Config.ssl_verify
+session.verify = Env.current.ssl_verify
 session.auth = auth
 
 
 class ResponseCodes(Enum):
     """HTTP response codes to handle individually."""
 
     UNAUTHORIZED = 401
@@ -125,15 +125,15 @@
         Method name.
 
     Returns
     -------
     str
         The full query url
     """
-    return f"{Config.web_api_endpoint}/{method}"
+    return f"{Env.current.web_api_endpoint}/{method}"
 
 
 def need_token_refresh(token: str) -> bool:
     """Check whether to refresh token or not.
 
     Parameters
     ----------
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/web/material_fitter.py` & `tidy3d-2.3.1/tidy3d/web/material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/web/material_libray.py` & `tidy3d-2.3.1/tidy3d/web/material_libray.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/web/s3utils.py` & `tidy3d-2.3.1/tidy3d/web/s3utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # pylint:disable=unused-argument
-"""handles filesystem, storage 
+"""handles filesystem, storage
 """
 import io
-import os
+import pathlib
 import urllib
 from datetime import datetime
 from enum import Enum
-from typing import Callable
+from typing import Callable, Mapping
 
 import boto3
 from boto3.s3.transfer import TransferConfig
 from pydantic import BaseModel, Field
 from rich.progress import TextColumn, Progress, BarColumn, DownloadColumn
 from rich.progress import TransferSpeedColumn, TimeRemainingColumn
 
 from . import httputils as http
-from .config import DEFAULT_CONFIG
+from .environment import Env
 
 
 class _UserCredential(BaseModel):
     """Stores information about user credentials."""
 
     access_key_id: str = Field(alias="accessKeyId")
     expiration: datetime
@@ -46,19 +46,19 @@
         return r.path[1:]
 
     def get_client(self) -> boto3.client:
         """Get the boto client for this token."""
 
         return boto3.client(
             "s3",
-            region_name=DEFAULT_CONFIG.s3_region,
+            region_name=Env.current.s3_region,
             aws_access_key_id=self.user_credential.access_key_id,
             aws_secret_access_key=self.user_credential.secret_access_key,
             aws_session_token=self.user_credential.session_token,
-            verify=DEFAULT_CONFIG.ssl_verify,
+            verify=Env.current.ssl_verify,
         )
 
     def is_expired(self) -> bool:
         """True if token is expired."""
 
         return (
             self.user_credential.expiration
@@ -169,44 +169,52 @@
     multipart_chunksize=1024 * 25,
     use_threads=True,
 )
 
 _s3_sts_tokens: [str, _S3STSToken] = {}
 
 
-def get_s3_sts_token(resource_id: str, file_name: str) -> _S3STSToken:
+def get_s3_sts_token(
+    resource_id: str, file_name: str, extra_arguments: Mapping[str, str] = None
+) -> _S3STSToken:
     """Get s3 sts token for the given resource id and file name.
 
     Parameters
     ----------
     resource_id : str
         The resource id, e.g. task id.
     file_name : str
         The remote file name on S3.
+    extra_arguments : Mapping[str, str]
+        Additional arguments for the query url.
 
     Returns
     -------
     _S3STSToken
         The S3 STS token.
     """
     cache_key = f"{resource_id}:{file_name}"
     if cache_key not in _s3_sts_tokens or _s3_sts_tokens[cache_key].is_expired():
-        method = f"tidy3d/tasks/{resource_id}/file?filename={file_name}"
+        method = f"tidy3d/py/tasks/{resource_id}/file?filename={file_name}"
+        if extra_arguments is not None:
+            method += "&" + "&".join(f"{k}={v}" for k, v in extra_arguments.items())
         resp = http.get(method)
         token = _S3STSToken.parse_obj(resp)
         _s3_sts_tokens[cache_key] = token
     return _s3_sts_tokens[cache_key]
 
 
+# pylint: disable=too-many-arguments
 def upload_string(
     resource_id: str,
     content: str,
     remote_filename: str,
     verbose: bool = True,
     progress_callback: Callable[[float], None] = None,
+    extra_arguments: Mapping[str, str] = None,
 ):
     """Upload a string to a file on S3.
 
     Parameters
     ----------
     resource_id : str
         The resource id, e.g. task id.
@@ -214,17 +222,19 @@
         The content of the file
     remote_filename : str
         The remote file name on S3 relative to the resource context root path.
     verbose : bool = True
         Whether to display a progressbar for the upload.
     progress_callback : Callable[[float], None] = None
         User-supplied callback function with ``bytes_in_chunk`` as argument.
+    extra_arguments : Mapping[str, str]
+        Additional arguments used to specify the upload bucket.
     """
 
-    token = get_s3_sts_token(resource_id, remote_filename)
+    token = get_s3_sts_token(resource_id, remote_filename, extra_arguments)
 
     def _upload(_callback: Callable) -> None:
         """Perform the upload with a callback fn
 
         Parameters
         ----------
         _callback : Callable[[float], None]
@@ -252,20 +262,22 @@
                 _upload(_callback)
                 progress.update(task_id, completed=total_size, refresh=True)
 
         elif progress_callback is None:
             _upload(lambda bytes_in_chunk: None)
 
 
+# pylint: disable=too-many-arguments
 def upload_file(
     resource_id: str,
     path: str,
     remote_filename: str,
     verbose: bool = True,
     progress_callback: Callable[[float], None] = None,
+    extra_arguments: Mapping[str, str] = None,
 ):
     """Upload a file to S3.
 
     Parameters
     ----------
     resource_id : str
         The resource id, e.g. task id.
@@ -273,17 +285,19 @@
         Path to the file to upload.
     remote_filename : str
         The remote file name on S3 relative to the resource context root path.
     verbose : bool = True
         Whether to display a progressbar for the upload.
     progress_callback : Callable[[float], None] = None
         User-supplied callback function with ``bytes_in_chunk`` as argument.
+    extra_arguments : Mapping[str, str]
+        Additional arguments used to specify the upload bucket.
     """
 
-    token = get_s3_sts_token(resource_id, remote_filename)
+    token = get_s3_sts_token(resource_id, remote_filename, extra_arguments)
 
     def _upload(_callback: Callable) -> None:
         """Perform the upload with a callback function.
 
         Parameters
         ----------
         _callback : Callable[[float], None]
@@ -300,15 +314,15 @@
             )
 
     if progress_callback is not None:
         _upload(progress_callback)
     else:
         if verbose:
             with _get_progress(_S3Action.UPLOADING) as progress:
-                total_size = os.path.getsize(path)
+                total_size = pathlib.Path(path).stat().st_size
                 task_id = progress.add_task("upload", filename=remote_filename, total=total_size)
 
                 def _callback(bytes_in_chunk):
                     progress.update(task_id, advance=bytes_in_chunk)
 
                 _upload(_callback)
 
@@ -320,15 +334,15 @@
 
 def download_file(
     resource_id: str,
     remote_filename: str,
     to_file: str = None,
     verbose: bool = True,
     progress_callback: Callable[[float], None] = None,
-):
+) -> pathlib.Path:
     """Download file from S3.
 
     Parameters
     ----------
     resource_id : str
         The resource id, e.g. task id.
     content : str
@@ -341,51 +355,56 @@
         User-supplied callback function with ``bytes_in_chunk`` as argument.
     """
 
     token = get_s3_sts_token(resource_id, remote_filename)
     client = token.get_client()
     meta_data = client.head_object(Bucket=token.get_bucket(), Key=token.get_s3_key())
 
+    # Get only last part of the remote file name
+    remote_basename = pathlib.Path(remote_filename).name
+
+    # set to_file if None
     if not to_file:
-        os.makedirs(resource_id, exist_ok=True)
-        to_file = os.path.join(resource_id, os.path.basename(remote_filename))
+        path = pathlib.Path(resource_id)
+        to_file = path / remote_basename
+    else:
+        to_file = pathlib.Path(to_file)
 
-    # make the leading directories in the 'to_file', if specified.
-    base_dir, _ = os.path.split(to_file)
-    if base_dir and not os.path.exists(base_dir):
-        os.makedirs(base_dir, exist_ok=True)
+    # make the leading directories in the 'to_file', if any
+    to_file.parent.mkdir(parents=True, exist_ok=True)
 
     def _download(_callback: Callable) -> None:
         """Perform the download with a callback function.
 
         Parameters
         ----------
         _callback : Callable[[float], None]
             Callback function for download, accepts ``bytes_in_chunk``
         """
 
         client.download_file(
-            Bucket=token.get_bucket(), Filename=to_file, Key=token.get_s3_key(), Callback=_callback
+            Bucket=token.get_bucket(),
+            Filename=str(to_file),
+            Key=token.get_s3_key(),
+            Callback=_callback,
         )
 
     if progress_callback is not None:
         _download(progress_callback)
     else:
         if verbose:
             with _get_progress(_S3Action.DOWNLOADING) as progress:
                 total_size = meta_data.get("ContentLength", 0)
                 progress.start()
-                task_id = progress.add_task(
-                    "download",
-                    filename=os.path.basename(remote_filename),
-                    total=total_size,
-                )
+                task_id = progress.add_task("download", filename=remote_basename, total=total_size)
 
                 def _callback(bytes_in_chunk):
                     progress.update(task_id, advance=bytes_in_chunk)
 
                 _download(_callback)
 
                 progress.update(task_id, completed=total_size, refresh=True)
 
         else:
             _download(lambda bytes_in_chunk: None)
+
+    return to_file
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/web/simulation_task.py` & `tidy3d-2.3.1/tidy3d/web/simulation_task.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Tidy3d webapi types."""
 from __future__ import annotations
 
-import os.path
+import os
+import pathlib
 import tempfile
 from datetime import datetime
 from typing import List, Optional, Callable, Tuple
 import pydantic as pd
 from pydantic import Extra, Field, parse_obj_as
 
 from tidy3d import Simulation
@@ -16,15 +17,15 @@
 from .s3utils import download_file, upload_file, upload_string
 from .types import Queryable, ResourceLifecycle, Submittable
 from .types import Tidy3DResource
 
 SIMULATION_JSON = "simulation.json"
 SIMULATION_HDF5 = "output/monitor_data.hdf5"
 RUNNING_INFO = "output/solver_progress.csv"
-LOG_FILE = "output/tidy3d.log"
+SIM_LOG_FILE = "output/tidy3d.log"
 SIM_FILE_HDF5 = "simulation.hdf5"
 
 
 class Folder(Tidy3DResource, Queryable, extra=Extra.allow):
     """Tidy3D Folder."""
 
     folder_id: str = Field(..., title="Folder id", description="folder id", alias="projectId")
@@ -50,49 +51,55 @@
             )
             if resp
             else None
         )
 
     # pylint: disable=arguments-differ
     @classmethod
-    def get(cls, folder_name: str):
+    def get(cls, folder_name: str, create: bool = False):
         """Get folder by name.
 
         Parameters
         ----------
         folder_name : str
             Name of the folder.
+        create : str
+            If the folder doesn't exist, create it.
 
         Returns
         -------
         folder : Folder
         """
-        resp = http.get(f"tidy3d/project?projectName={folder_name}")
-        return Folder(**resp) if resp else None
+        folder = FOLDER_CACHE.get(folder_name)
+        if not folder:
+            resp = http.get(f"tidy3d/project?projectName={folder_name}")
+            if resp:
+                folder = Folder(**resp)
+        if create and not folder:
+            resp = http.post("tidy3d/projects", {"projectName": folder_name})
+            if resp:
+                folder = Folder(**resp)
+        FOLDER_CACHE[folder_name] = folder
+        return folder
 
     # pylint: disable=arguments-differ
     @classmethod
     def create(cls, folder_name: str):
         """Create a folder, return existing folder if there is one has the same name.
 
         Parameters
         ----------
-        ----------
         folder_name : str
             Name of the folder.
 
         Returns
         -------
         folder : Folder
         """
-        folder = Folder.get(folder_name)
-        if folder:
-            return folder
-        resp = http.post("tidy3d/projects", {"projectName": folder_name})
-        return Folder(**resp) if resp else None
+        return Folder.get(folder_name, True)
 
     def delete(self):
         """Remove this folder."""
 
         http.delete(f"tidy3d/projects/{self.folder_id}")
 
     def list_tasks(self) -> List[Tidy3DResource]:
@@ -182,27 +189,27 @@
 
     # pylint: disable=arguments-differ,too-many-arguments
     @classmethod
     def create(
         cls,
         simulation: Simulation,
         task_name: str,
-        folder_name="default",
-        call_back_url=None,
+        folder_name: str = "default",
+        callback_url: str = None,
         simulation_type: str = "tidy3d",
         parent_tasks: List[str] = None,
     ) -> SimulationTask:
         """Create a new task on the server.
 
         Parameters
         ----------
         simulation: :class".Simulation"
             The :class:`.Simulation` will be uploaded to server in the submitting phase.
             If Simulation is too large to fit into memory, pass None to this parameter
-            and use :meth:`.simulationTask.upload_file` instead.
+            and use :meth:`.SimulationTask.upload_file` instead.
         task_name: str
             The name of the task.
         folder_name: str,
             The name of the folder to store the task. Default is "default".
         callback_url: str
             Http PUT url to receive simulation finish event. The body content is a json file with
             fields ``{'id', 'status', 'name', 'workUnit', 'solverVersion'}``.
@@ -211,28 +218,22 @@
         parent_tasks : List[str]
             List of related task ids.
 
         Returns
         -------
         :class:`SimulationTask`
             :class:`SimulationTask` object containing info about status, size,
-             credits of task and others.
+            credits of task and others.
         """
-        folder = FOLDER_CACHE.get(folder_name)
-        if not folder:
-            folder = Folder.get(folder_name)
-        if not folder:
-            folder = Folder.create(folder_name)
-        FOLDER_CACHE[folder_name] = folder
-
+        folder = Folder.get(folder_name, create=True)
         resp = http.post(
             f"tidy3d/projects/{folder.folder_id}/tasks",
             {
                 "taskName": task_name,
-                "call_back_url": call_back_url,
+                "callbackUrl": callback_url,
                 "simulationType": simulation_type,
                 "parentTasks": parent_tasks,
             },
         )
 
         return SimulationTask(**resp, simulation=simulation, folder=folder)
 
@@ -255,18 +256,14 @@
         resp = http.get(f"tidy3d/tasks/{task_id}/detail")
         return SimulationTask(**resp) if resp else None
 
     @classmethod
     def get_running_tasks(cls) -> List[SimulationTask]:
         """Get a list of running tasks from the server"
 
-
-        Parameters
-        ----------
-
         Returns
         -------
         List[:class:`.SimulationTask`]
             :class:`.SimulationTask` object containing info about status,
              size, credits of task and others.
         """
         resp = http.get("tidy3d/py/tasks")
@@ -283,42 +280,47 @@
     def get_simulation(self) -> Optional[Simulation]:
         """Download simulation from server.
 
         Returns
         -------
         :class:`.Simulation`
             :class:`.Simulation` object containing info about status, size,
-             credits of task and others.
+            credits of task and others.
         """
         if self.simulation:
             return self.simulation
 
         with tempfile.NamedTemporaryFile(suffix=".json") as temp:
             self.get_simulation_json(temp.name)
-            if os.path.exists(temp.name):
+            if pathlib.Path(temp.name).exists():
                 self.simulation = Simulation.from_file(temp.name)
                 return self.simulation
         return None
 
     def get_simulation_json(
         self, to_file: str, verbose: bool = True, progress_callback: Callable[[float], None] = None
-    ) -> None:
+    ) -> pathlib.Path:
         """Get json file for a :class:`.Simulation` from server.
 
         Parameters
         ----------
         to_file: str
             save file to path.
         verbose: bool = True
-            Whether to display progressbars.
+            Whether to display progress bars.
         progress_callback : Callable[[float], None] = None
-            Optional callback function called when uploading file.
+            Optional callback function called while downloading the data.
+
+        Returns
+        -------
+        path: pathlib.Path
+            Path to saved file.
         """
         assert self.task_id
-        download_file(
+        return download_file(
             self.task_id,
             SIMULATION_JSON,
             to_file=to_file,
             verbose=verbose,
             progress_callback=progress_callback,
         )
 
@@ -326,41 +328,42 @@
         self, verbose: bool = True, progress_callback: Callable[[float], None] = None
     ) -> None:
         """Upload :class:`.Simulation` object to Server.
 
         Parameters
         ----------
         verbose: bool = True
-            Whether to display progressbars.
+            Whether to display progress bars.
         progress_callback : Callable[[float], None] = None
-            Optional callback function called when uploading file.
+            Optional callback function called while uploading the data.
         """
         assert self.task_id
         assert self.simulation
         upload_string(
             self.task_id,
             self.simulation._json_string,  # pylint: disable=protected-access
             SIMULATION_JSON,
             verbose=verbose,
             progress_callback=progress_callback,
         )
         if len(self.simulation.custom_datasets) > 0:
             # Also upload hdf5 containing all data.
-            # The temp file will be re-opened in `to_hdf5` which can cause an error on some systems
-            # so we explicitly close it first.
-            data_file = tempfile.NamedTemporaryFile()  # pylint:disable=consider-using-with
-            data_file.close()
-            self.simulation.to_hdf5(data_file.name)
-            upload_file(
-                self.task_id,
-                data_file.name,
-                SIM_FILE_HDF5,
-                verbose=verbose,
-                progress_callback=progress_callback,
-            )
+            file, file_name = tempfile.mkstemp()
+            os.close(file)
+            self.simulation.to_hdf5(file_name)
+            try:
+                upload_file(
+                    self.task_id,
+                    file_name,
+                    SIM_FILE_HDF5,
+                    verbose=verbose,
+                    progress_callback=progress_callback,
+                )
+            finally:
+                os.unlink(file_name)
 
     def upload_file(
         self,
         local_file: str,
         remote_filename: str,
         verbose: bool = True,
         progress_callback: Callable[[float], None] = None,
@@ -371,17 +374,17 @@
         Parameters
         ----------
         local_file: str
             local file path.
         remote_filename: str
             file name on the server
         verbose: bool = True
-            Whether to display progressbars.
+            Whether to display progress bars.
         progress_callback : Callable[[float], None] = None
-            Optional callback function called when uploading file.
+            Optional callback function called while uploading the data.
         """
         assert self.task_id
 
         upload_file(
             self.task_id,
             local_file,
             remote_filename,
@@ -390,19 +393,19 @@
         )
 
     def submit(
         self,
         solver_version: str = None,
         worker_group: str = None,
     ):
-        """Kick off this task. If this task instance contain a :class:`.Simulation`,
-         it will be uploaded to server first,
-        then kick off the task. Otherwise, this method makes assumption that
-         the Simulation has been uploaded by the
-        upload_file function, so the task will be kicked off directly.
+        """Kick off this task.
+
+        If this task instance contain a :class:`.Simulation`, it will be uploaded to server before
+        starting the task. Otherwise, this method assumes that the Simulation has been uploaded by
+        the upload_file function, so the task will be kicked off directly.
 
         Parameters
         ----------
         solver_version: str = None
             target solver version.
         worker_group: str = None
             worker group
@@ -457,28 +460,33 @@
                 "protocolVersion": protocol_version,
             },
         )
         return resp
 
     def get_simulation_hdf5(
         self, to_file: str, verbose: bool = True, progress_callback: Callable[[float], None] = None
-    ) -> None:
+    ) -> pathlib.Path:
         """Get hdf5 file from Server.
 
         Parameters
         ----------
         to_file: str
             save file to path.
         verbose: bool = True
-            Whether to display progressbars.
+            Whether to display progress bars.
         progress_callback : Callable[[float], None] = None
-            Optional callback function called when uploading file.
+            Optional callback function called while downloading the data.
+
+        Returns
+        -------
+        path: pathlib.Path
+            Path to saved file.
         """
         assert self.task_id
-        download_file(
+        return download_file(
             self.task_id,
             SIMULATION_HDF5,
             to_file=to_file,
             verbose=verbose,
             progress_callback=progress_callback,
         )
 
@@ -487,40 +495,45 @@
 
         Returns
         -------
         perc_done : float
             Percentage of run done (in terms of max number of time steps).
             Is ``None`` if run info not available.
         field_decay : float
-            Average field intensity normlized to max value (1.0).
+            Average field intensity normalized to max value (1.0).
             Is ``None`` if run info not available.
         """
         assert self.task_id
 
         resp = http.get(f"tidy3d/tasks/{self.task_id}/progress")
         perc_done = resp.get("perc_done")
         field_decay = resp.get("field_decay")
         return perc_done, field_decay
 
     def get_log(
         self, to_file: str, verbose: bool = True, progress_callback: Callable[[float], None] = None
-    ) -> None:
+    ) -> pathlib.Path:
         """Get log file from Server.
 
         Parameters
         ----------
         to_file: str
             save file to path.
         verbose: bool = True
-            Whether to display progressbars.
+            Whether to display progress bars.
         progress_callback : Callable[[float], None] = None
-            Optional callback function called when uploading file.
+            Optional callback function called while downloading the data.
+
+        Returns
+        -------
+        path: pathlib.Path
+            Path to saved file.
         """
 
         assert self.task_id
-        download_file(
+        return download_file(
             self.task_id,
-            LOG_FILE,
+            SIM_LOG_FILE,
             to_file=to_file,
             verbose=verbose,
             progress_callback=progress_callback,
         )
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/web/task.py` & `tidy3d-2.3.1/tidy3d/web/task.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,14 +31,31 @@
 # type of the task_id
 TaskId = str
 
 # type of task_name
 TaskName = str
 
 
+class ChargeType(str, Enum):
+    """The payment method of task."""
+
+    FREE = "free"
+    PAID = "paid"
+
+
+class TaskBlockInfo(TaskBase):
+    """The block info that task will be blocked by all three features of DE,
+    User limit and Insufficient balance"""
+
+    chargeType: ChargeType = None
+    maxFreeCount: int = None
+    maxGridPoints: int = None
+    maxTimeSteps: int = None
+
+
 class TaskInfo(TaskBase):
     """General information about task."""
 
     taskId: str
     taskName: str = None
     nodeSize: int = None
     completedAt: Optional[datetime] = None
@@ -53,14 +70,16 @@
     estFlexUnit: float = None
     s3Storage: float = None
     startSolverTime: Optional[datetime] = None
     finishSolverTime: Optional[datetime] = None
     totalSolverTime: int = None
     callbackUrl: str = None
     taskType: str = None
+    metadataStatus: str = None
+    taskBlockInfo: TaskBlockInfo = None
 
 
 class RunInfo(TaskBase):
     """Information about the run."""
 
     perc_done: pydantic.confloat(ge=0.0, le=100.0)
     field_decay: pydantic.confloat(ge=0.0, le=1.0)
```

### Comparing `tidy3d-2.3.0rc1/tidy3d/web/types.py` & `tidy3d-2.3.1/tidy3d/web/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.3.0rc1/tidy3d/web/webapi.py` & `tidy3d-2.3.1/tidy3d/web/webapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,22 +13,21 @@
 
 import pytz
 from rich.console import Console
 from rich.progress import Progress
 
 from .environment import Env
 from .simulation_task import SimulationTask, SIM_FILE_HDF5, Folder
-from .task import TaskId, TaskInfo
+from .task import TaskId, TaskInfo, ChargeType
 from ..components.data.sim_data import SimulationData
 from ..components.simulation import Simulation
 from ..components.types import Literal
 from ..log import log
 from ..exceptions import WebError
 
-
 # time between checking task status
 REFRESH_TIME = 0.3
 
 # time between checking run status
 RUN_REFRESH_TIME = 1.0
 
 # file names when uploading to S3
@@ -87,18 +86,18 @@
 
     Parameters
     ----------
     simulation : :class:`.Simulation`
         Simulation to upload to server.
     task_name : str
         Name of task.
-    path : str = "simulation_data.hdf5"
-        Path to download results file (.hdf5), including filename.
     folder_name : str = "default"
         Name of folder to store task on web UI.
+    path : str = "simulation_data.hdf5"
+        Path to download results file (.hdf5), including filename.
     callback_url : str = None
         Http PUT url to receive simulation finish event. The body content is a json file with
         fields ``{'id', 'status', 'name', 'workUnit', 'solverVersion'}``.
     verbose : bool = True
         If `True`, will print progressbars and status, otherwise, will run silently.
     progress_callback_upload : Callable[[float], None] = None
         Optional callback function called when uploading file with ``bytes_in_chunk`` as argument.
@@ -139,14 +138,15 @@
     task_name: str,
     folder_name: str = "default",
     callback_url: str = None,
     verbose: bool = True,
     progress_callback: Callable[[float], None] = None,
     simulation_type: str = "tidy3d",
     parent_tasks: List[str] = None,
+    source_required: bool = True,
 ) -> TaskId:
     """Upload simulation to server, but do not start running :class:`.Simulation`.
 
     Parameters
     ----------
     simulation : :class:`.Simulation`
         Simulation to upload to server.
@@ -161,26 +161,28 @@
         If `True`, will print progressbars and status, otherwise, will run silently.
     progress_callback : Callable[[float], None] = None
         Optional callback function called when uploading file with ``bytes_in_chunk`` as argument.
     simulation_type : str
         Type of simulation being uploaded.
     parent_tasks : List[str]
         List of related task ids.
+    source_required: bool = True
+        If ``True``, simulations without sources will raise an error before being uploaded.
 
     Returns
     -------
     str
         Unique identifier of task on server.
 
     Note
     ----
     To start the simulation running, must call :meth:`start` after uploaded.
     """
 
-    simulation.validate_pre_upload()
+    simulation.validate_pre_upload(source_required=source_required)
     log.debug("Creating task.")
 
     task = SimulationTask.create(
         simulation, task_name, folder_name, callback_url, simulation_type, parent_tasks
     )
     if verbose:
         console = Console()
@@ -262,14 +264,31 @@
         Average field intensity normlized to max value (1.0).
         Is ``None`` if run info not available.
     """
     task = SimulationTask(taskId=task_id)
     return task.get_running_info()
 
 
+def get_status(task_id) -> str:
+    """Get the status of a task. Raises an error if status is "error".
+
+    Parameters
+    ----------
+    task_id : str
+        Unique identifier of task on server.  Returned by :meth:`upload`.
+    """
+    task_info = get_info(task_id)
+    status = task_info.status
+    if status == "visualize":
+        return "success"
+    if status == "error":
+        raise WebError("Error running task!")
+    return status
+
+
 # pylint: disable=too-many-statements, too-many-locals, too-many-branches
 def monitor(task_id: TaskId, verbose: bool = True) -> None:
     # pylint:disable=too-many-statements
     """Print the real time task progress until completion.
 
     Parameters
     ----------
@@ -286,41 +305,63 @@
     task_info = get_info(task_id)
     task_name = task_info.taskName
 
     break_statuses = ("success", "error", "diverged", "deleted", "draft")
 
     console = Console() if verbose else None
 
-    def get_status() -> str:
-        """Get status for this task."""
-        task_info = get_info(task_id)
-        status = task_info.status
-        if status == "visualize":
-            return "success"
-        if status == "error":
-            raise WebError("Error running task!")
-        return status
-
     def get_estimated_cost() -> float:
         """Get estimated cost, if None, is not ready."""
         task_info = get_info(task_id)
-        return task_info.estFlexUnit
+        block_info = task_info.taskBlockInfo
+        if block_info and block_info.chargeType == ChargeType.FREE:
+            est_flex_unit = 0
+            grid_points = block_info.maxGridPoints
+            time_steps = block_info.maxTimeSteps
+            if grid_points < 1000:
+                grid_points_str = f"{grid_points}"
+            elif 1000 <= grid_points < 1000 * 1000:
+                grid_points_str = f"{grid_points / 1000}K"
+            else:
+                grid_points_str = f"{grid_points / 1000 / 1000}M"
+
+            if time_steps < 1000:
+                time_steps_str = f"{time_steps}"
+            elif 1000 <= grid_points < 1000 * 1000:
+                time_steps_str = f"{time_steps / 1000}K"
+            else:
+                time_steps_str = f"{time_steps / 1000 / 1000}M"
+
+            console.log(
+                f"You are running this simulation for FREE. Your current plan allows"
+                f" up to {block_info.maxFreeCount} free non-concurrent simulations per"
+                f" day (under {grid_points_str} grid points and {time_steps_str}"
+                f" time steps)"
+            )
+        else:
+            est_flex_unit = task_info.estFlexUnit
+            if est_flex_unit is not None and est_flex_unit > 0:
+                console.log(
+                    f"Maximum FlexCredit cost: {est_flex_unit:1.3f}. Use 'web.real_cost(task_id)'"
+                    f" to get the billed FlexCredit cost after a simulation run."
+                )
+        return est_flex_unit
 
     def monitor_preprocess() -> None:
         """Periodically check the status."""
-        status = get_status()
+        status = get_status(task_id)
         while status not in break_statuses and status != "running":
-            new_status = get_status()
+            new_status = get_status(task_id)
             if new_status != status:
                 status = new_status
                 if verbose and status != "running":
                     console.log(f"status = {status}")
             time.sleep(REFRESH_TIME)
 
-    status = get_status()
+    status = get_status(task_id)
 
     if verbose:
         console.log(f"status = {status}")
 
     # already done
     if status in break_statuses:
         return
@@ -330,37 +371,36 @@
         with console.status(f"[bold green]Starting '{task_name}'...", spinner="runner"):
             monitor_preprocess()
     else:
         monitor_preprocess()
 
     # if the estimated cost is ready, print it
     if verbose:
-        est_flex_unit = get_estimated_cost()
-        if est_flex_unit is not None and est_flex_unit > 0:
-            console.log(
-                f"Maximum FlexCredit cost: {est_flex_unit:1.3f}. Use 'web.real_cost(task_id)' to "
-                "get the billed FlexCredit cost after a simulation run."
-            )
+        get_estimated_cost()
         console.log("starting up solver")
 
     # while running but before the percentage done is available, keep waiting
-    while get_run_info(task_id)[0] is None and get_status() == "running":
+    while get_run_info(task_id)[0] is None and get_status(task_id) == "running":
         time.sleep(REFRESH_TIME)
 
     # while running but percentage done is available
     if verbose:
 
         # verbose case, update progressbar
         console.log("running solver")
+        console.log(
+            "To cancel the simulation, use 'web.delete(task_id)' or delete the task in the web"
+            " UI. Terminating the Python script will not stop the job running on the cloud."
+        )
         with Progress(console=console) as progress:
 
             pbar_pd = progress.add_task("% done", total=100)
             perc_done, _ = get_run_info(task_id)
 
-            while perc_done is not None and perc_done < 100 and get_status() == "running":
+            while perc_done is not None and perc_done < 100 and get_status(task_id) == "running":
                 perc_done, field_decay = get_run_info(task_id)
                 new_description = f"solver progress (field decay = {field_decay:.2e})"
                 progress.update(pbar_pd, completed=perc_done, description=new_description)
                 time.sleep(RUN_REFRESH_TIME)
 
             perc_done, field_decay = get_run_info(task_id)
             if perc_done is not None and perc_done < 100 and field_decay > 0:
@@ -368,34 +408,34 @@
 
             progress.update(pbar_pd, completed=100, refresh=True)
 
     else:
 
         # non-verbose case, just keep checking until status is not running or perc_done >= 100
         perc_done, _ = get_run_info(task_id)
-        while perc_done is not None and perc_done < 100 and get_status() == "running":
+        while perc_done is not None and perc_done < 100 and get_status(task_id) == "running":
             perc_done, field_decay = get_run_info(task_id)
             time.sleep(1.0)
 
     # post processing
     if verbose:
 
-        status = get_status()
+        status = get_status(task_id)
         if status != "running":
             console.log(f"status = {status}")
 
         with console.status(f"[bold green]Finishing '{task_name}'...", spinner="runner"):
             while status not in break_statuses:
-                new_status = get_status()
+                new_status = get_status(task_id)
                 if new_status != status:
                     status = new_status
                     console.log(f"status = {status}")
                 time.sleep(REFRESH_TIME)
     else:
-        while get_status() not in break_statuses:
+        while get_status(task_id) not in break_statuses:
             time.sleep(REFRESH_TIME)
 
 
 @wait_for_connection
 def download(
     task_id: TaskId,
     path: str = "simulation_data.hdf5",
@@ -682,15 +722,15 @@
     -------
     float
         Estimated maximum cost for :class:`.Simulation` associated with given ``task_id``..
 
     Note
     ----
     Cost is calculated assuming the simulation runs for
-    the full ``run_time``. If early shut-off is triggered, the cost is adjusted proporionately.
+    the full ``run_time``. If early shut-off is triggered, the cost is adjusted proportionately.
 
     Parameters
     ----------
     task_id : str
         Unique identifier of task on server.  Returned by :meth:`upload`.
 
     Returns
@@ -698,22 +738,33 @@
     float
         Estimated cost of the task in FlexCredits.
     """
 
     task = SimulationTask.get(task_id)
     if not task:
         raise ValueError("Task not found.")
-    resp = task.estimate_cost()
-    flex_unit = resp.get("flex_unit")
-    if not flex_unit:
-        log.warning(
-            "Could not get estimated cost! It will be reported in preprocessing upon "
-            "simulation run."
-        )
-    return flex_unit
+
+    task.estimate_cost()
+    task_info = get_info(task_id)
+    status = task_info.metadataStatus
+
+    # Wait for a termination status
+    while status not in ["processed", "success", "error", "failed"]:
+        time.sleep(REFRESH_TIME)
+        task_info = get_info(task_id)
+        status = task_info.metadataStatus
+
+    if status in ["processed", "success"]:
+        return task_info.estFlexUnit
+
+    log.warning(
+        "Could not get estimated cost! It will be reported during a simulation run in the "
+        "preprocessing step."
+    )
+    return None
 
 
 @wait_for_connection
 def real_cost(task_id: str) -> float:
     """Get the billed cost for given task after it has been run.
 
     Note
```

### Comparing `tidy3d-2.3.0rc1/tidy3d.egg-info/PKG-INFO` & `tidy3d-2.3.1/tidy3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.3.0rc1
+Version: 2.3.1
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Project-URL: Bug Tracker, https://github.com/flexcompute/tidy3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy3d-2.3.0rc1/tidy3d.egg-info/SOURCES.txt` & `tidy3d-2.3.1/tidy3d.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 tests/test_plugins/test_dispersion_fitter.py
 tests/test_plugins/test_mode_solver.py
 tests/test_plugins/test_polyslab.py
 tests/test_plugins/test_resonance_finder.py
 tests/test_plugins/test_waveguide.py
 tests/test_web/__init__.py
 tests/test_web/mock_web.py
-tests/test_web/test_auth.py
 tests/test_web/test_cli.py
 tests/test_web/test_material_fitter.py
 tests/test_web/test_task.py
 tests/test_web/test_tidy3d_folder.py
 tests/test_web/test_tidy3d_material_library.py
 tests/test_web/test_tidy3d_task.py
 tests/test_web/test_webapi.py
@@ -131,28 +130,27 @@
 tidy3d/plugins/dispersion/fit_web.py
 tidy3d/plugins/dispersion/web.py
 tidy3d/plugins/mode/__init__.py
 tidy3d/plugins/mode/derivatives.py
 tidy3d/plugins/mode/mode_solver.py
 tidy3d/plugins/mode/solver.py
 tidy3d/plugins/mode/transforms.py
+tidy3d/plugins/mode/web.py
 tidy3d/plugins/polyslab/__init__.py
 tidy3d/plugins/polyslab/polyslab.py
 tidy3d/plugins/resonance/__init__.py
 tidy3d/plugins/resonance/resonance.py
 tidy3d/plugins/smatrix/__init__.py
 tidy3d/plugins/smatrix/smatrix.py
 tidy3d/plugins/waveguide/__init__.py
 tidy3d/plugins/waveguide/rectangular_dielectric.py
 tidy3d/web/__init__.py
 tidy3d/web/asynchronous.py
-tidy3d/web/auth.py
 tidy3d/web/cacert.pem
 tidy3d/web/cache.py
-tidy3d/web/config.py
 tidy3d/web/container.py
 tidy3d/web/environment.py
 tidy3d/web/http_management.py
 tidy3d/web/httputils.py
 tidy3d/web/material_fitter.py
 tidy3d/web/material_libray.py
 tidy3d/web/s3utils.py
```

### Comparing `tidy3d-2.3.0rc1/tidy3d.egg-info/requires.txt` & `tidy3d-2.3.1/tidy3d.egg-info/requires.txt`

 * *Files identical despite different names*

