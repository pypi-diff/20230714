# Comparing `tmp/dkist_processing_visp-2.5.1.tar.gz` & `tmp/dkist_processing_visp-2.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_processing_visp-2.5.1.tar", last modified: Tue Jul 11 22:22:17 2023, max compression
+gzip compressed data, was "dkist_processing_visp-2.6.0rc1.tar", last modified: Fri Jul 14 00:14:39 2023, max compression
```

## Comparing `dkist_processing_visp-2.5.1.tar` & `dkist_processing_visp-2.6.0rc1.tar`

### file list

```diff
@@ -1,114 +1,116 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:22:17.987091 dkist_processing_visp-2.5.1/
--rw-rw-rw-   0 root         (0) root         (0)     2461 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    21632 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     6213 2023-07-11 22:22:17.987091 dkist_processing_visp-2.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5645 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3652 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/SCIENCE_CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     3428 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:22:17.979091 dkist_processing_visp-2.5.1/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:22:17.979091 dkist_processing_visp-2.5.1/dkist_processing_visp/
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:22:17.979091 dkist_processing_visp-2.5.1/dkist_processing_visp/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/fonts/Lato-Regular.ttf
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:22:17.979091 dkist_processing_visp-2.5.1/dkist_processing_visp/models/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3440 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    11306 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/models/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:22:17.979091 dkist_processing_visp-2.5.1/dkist_processing_visp/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5370 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/parsers/map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/parsers/polarimeter_mode.py
--rw-rw-rw-   0 root         (0) root         (0)     2913 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/parsers/raster_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/parsers/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1869 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/parsers/visp_l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/parsers/visp_l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      843 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/parsers/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:22:17.983091 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3296 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    14744 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     4137 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/dark.py
--rw-rw-rw-   0 root         (0) root         (0)    41082 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    20368 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)      395 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5343 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     7068 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/make_movie_frames.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:22:17.983091 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5656 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/mixin/corrections.py
--rw-rw-rw-   0 root         (0) root         (0)     1343 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/mixin/downsample.py
--rw-rw-rw-   0 root         (0) root         (0)     7112 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)    10506 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     4604 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     7944 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    28173 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/science.py
--rw-rw-rw-   0 root         (0) root         (0)    28801 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6846 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:22:17.983091 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16409 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:22:17.983091 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/local_trial_workflows/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/local_trial_workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18994 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py
--rw-rw-rw-   0 root         (0) root         (0)     8247 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2514 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    18443 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     1171 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_build_quality_report.py
--rw-rw-rw-   0 root         (0) root         (0)     5272 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_dark.py
--rw-rw-rw-   0 root         (0) root         (0)     2173 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_downsample.py
--rw-rw-rw-   0 root         (0) root         (0)    14009 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    12613 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)     5651 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     4021 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    11818 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    16234 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_parse.py
--rw-rw-rw-   0 root         (0) root         (0)     4383 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    19734 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_science.py
--rw-rw-rw-   0 root         (0) root         (0)     9883 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_submit_quality.py
--rw-rw-rw-   0 root         (0) root         (0)     5340 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5091 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_visp_constants.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     5752 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:22:17.987091 dkist_processing_visp-2.5.1/dkist_processing_visp/workflows/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3280 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/workflows/l0_processing.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/workflows/single_task_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     3391 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/dkist_processing_visp/workflows/trial_workflows.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:22:17.979091 dkist_processing_visp-2.5.1/dkist_processing_visp.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6213 2023-07-11 22:22:17.000000 dkist_processing_visp-2.5.1/dkist_processing_visp.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3873 2023-07-11 22:22:17.000000 dkist_processing_visp-2.5.1/dkist_processing_visp.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-11 22:22:17.000000 dkist_processing_visp-2.5.1/dkist_processing_visp.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-07-11 22:22:17.000000 dkist_processing_visp-2.5.1/dkist_processing_visp.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-11 22:22:17.000000 dkist_processing_visp-2.5.1/dkist_processing_visp.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:22:17.987091 dkist_processing_visp-2.5.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     4844 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/docs/background_light.rst
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     2028 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     6427 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/docs/gain_correction.rst
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/docs/l0_to_l1_visp.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     4995 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/docs/polarization_calibration.rst
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/docs/requirements_table.rst
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/docs/science_calibration.rst
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/docs/scientific_changelog.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 22:22:17.987091 dkist_processing_visp-2.5.1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       60 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/science_towncrier.sh
--rw-rw-rw-   0 root         (0) root         (0)     1687 2023-07-11 22:22:17.987091 dkist_processing_visp-2.5.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      422 2023-07-11 22:22:10.000000 dkist_processing_visp-2.5.1/towncrier_science.toml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.055791 dkist_processing_visp-2.6.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     2461 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    21632 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6216 2023-07-14 00:14:39.055791 dkist_processing_visp-2.6.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5645 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3652 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/SCIENCE_CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3428 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.047791 dkist_processing_visp-2.6.0rc1/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/changelog/121.feature.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.047791 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.047791 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/fonts/Lato-Regular.ttf
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.047791 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/models/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3440 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    11306 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/models/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.047791 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5370 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     3005 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/modulator_states.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/polarimeter_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/raster_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/visp_l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/visp_l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      843 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.051792 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3296 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    14744 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     4137 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/dark.py
+-rw-rw-rw-   0 root         (0) root         (0)    41082 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    20368 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5343 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7068 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/make_movie_frames.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.051792 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5642 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/mixin/corrections.py
+-rw-rw-rw-   0 root         (0) root         (0)     1343 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/mixin/downsample.py
+-rw-rw-rw-   0 root         (0) root         (0)     7112 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)    10506 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4329 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     7944 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    28173 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/science.py
+-rw-rw-rw-   0 root         (0) root         (0)    28801 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6846 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.055791 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16409 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.055791 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/local_trial_workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/local_trial_workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18994 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py
+-rw-rw-rw-   0 root         (0) root         (0)     8247 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2514 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    18443 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_build_quality_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     5272 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     2173 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_downsample.py
+-rw-rw-rw-   0 root         (0) root         (0)    14009 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    12613 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)     5651 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)    11818 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    20093 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    19734 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     9883 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_submit_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     5340 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5091 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_visp_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     5752 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.055791 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3280 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/workflows/l0_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/workflows/single_task_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     3314 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/workflows/trial_workflows.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.047791 dkist_processing_visp-2.6.0rc1/dkist_processing_visp.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6216 2023-07-14 00:14:38.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3949 2023-07-14 00:14:39.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-14 00:14:38.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-07-14 00:14:38.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-14 00:14:38.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.055791 dkist_processing_visp-2.6.0rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     4844 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/background_light.rst
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6427 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/gain_correction.rst
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/l0_to_l1_visp.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     4995 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/polarization_calibration.rst
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/requirements_table.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/science_calibration.rst
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/scientific_changelog.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.055791 dkist_processing_visp-2.6.0rc1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       60 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/science_towncrier.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1687 2023-07-14 00:14:39.055791 dkist_processing_visp-2.6.0rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      422 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/towncrier_science.toml
```

### Comparing `dkist_processing_visp-2.5.1/.gitignore` & `dkist_processing_visp-2.6.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/.pre-commit-config.yaml` & `dkist_processing_visp-2.6.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/CHANGELOG.rst` & `dkist_processing_visp-2.6.0rc1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/PKG-INFO` & `dkist_processing_visp-2.6.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_processing_visp
-Version: 2.5.1
+Version: 2.6.0rc1
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_visp-2.5.1/README.rst` & `dkist_processing_visp-2.6.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/SCIENCE_CHANGELOG.rst` & `dkist_processing_visp-2.6.0rc1/SCIENCE_CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/bitbucket-pipelines.yml` & `dkist_processing_visp-2.6.0rc1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/check_changelog_updated.sh` & `dkist_processing_visp-2.6.0rc1/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/fonts/Lato-Regular.ttf` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/models/constants.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/models/parameters.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/models/tags.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/parsers/map_repeats.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/parsers/polarimeter_mode.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/polarimeter_mode.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/parsers/raster_step.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/raster_step.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/parsers/task.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/task.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/parsers/time.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/parsers/visp_l0_fits_access.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/visp_l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/parsers/visp_l1_fits_access.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/visp_l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/parsers/wavelength.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/assemble_movie.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/background_light.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/background_light.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/dark.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/geometric.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/geometric.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/instrument_polarization.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/instrument_polarization.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/lamp.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/lamp.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/make_movie_frames.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/mixin/corrections.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/mixin/corrections.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         """
         arrays = [arrays] if isinstance(arrays, np.ndarray) else arrays
         for array in arrays:
             numy = array.shape[1]
             array_output = np.zeros(array.shape)
             for j in range(numy):
-                array_output[:, j] = spnd.interpolation.shift(
+                array_output[:, j] = spnd.shift(
                     array[:, j], -spec_shift[j], mode="constant", cval=np.nanmedian(array[:, j])
                 )
             yield array_output
 
     def corrections_mask_hairlines(self, array: np.ndarray) -> np.ndarray:
         """
         Mask hairlines from an array.
```

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/mixin/downsample.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/mixin/downsample.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/mixin/input_frame_loaders.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/mixin/input_frame_loaders.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/parse.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 """ViSP parse task."""
 from typing import TypeVar
 
-from dkist_processing_common.models.constants import BudName
 from dkist_processing_common.models.flower_pot import Stem
 from dkist_processing_common.parsers.cs_step import CSStepFlower
 from dkist_processing_common.parsers.cs_step import NumCSStepBud
-from dkist_processing_common.parsers.single_value_single_key_flower import (
-    SingleValueSingleKeyFlower,
-)
 from dkist_processing_common.parsers.time import ExposureTimeFlower
 from dkist_processing_common.parsers.unique_bud import UniqueBud
 from dkist_processing_common.tasks import ParseL0InputDataBase
 from dkist_processing_common.tasks.mixin.input_dataset import InputDatasetMixin
 
 from dkist_processing_visp.models.constants import VispBudName
 from dkist_processing_visp.models.parameters import VispParameters
-from dkist_processing_visp.models.tags import VispStemName
 from dkist_processing_visp.parsers.map_repeats import MapScanFlower
 from dkist_processing_visp.parsers.map_repeats import NumMapScansBud
+from dkist_processing_visp.parsers.modulator_states import ModulatorStateFlower
+from dkist_processing_visp.parsers.modulator_states import NumberModulatorStatesBud
 from dkist_processing_visp.parsers.polarimeter_mode import PolarimeterModeBud
 from dkist_processing_visp.parsers.raster_step import RasterScanStepFlower
 from dkist_processing_visp.parsers.raster_step import TotalRasterStepsBud
 from dkist_processing_visp.parsers.task import VispTaskTypeFlower
 from dkist_processing_visp.parsers.time import ObsIpStartTimeBud
 from dkist_processing_visp.parsers.time import VispTaskExposureTimesBud
 from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
@@ -67,17 +64,15 @@
     def constant_buds(self) -> list[S]:
         """Add ViSP specific constants to common constants."""
         return super().constant_buds + [
             NumMapScansBud(),
             TotalRasterStepsBud(),
             NumCSStepBud(self.parameters.max_cs_step_time_sec),
             ObsIpStartTimeBud(),
-            UniqueBud(
-                constant_name=BudName.num_modstates.value, metadata_key="number_of_modulator_states"
-            ),
+            NumberModulatorStatesBud(),
             ObserveWavelengthBud(),
             PolarimeterModeBud(),
             VispTaskExposureTimesBud(
                 stem_name=VispBudName.lamp_exposure_times.value, ip_task_type="LAMP_GAIN"
             ),
             VispTaskExposureTimesBud(
                 stem_name=VispBudName.solar_exposure_times.value, ip_task_type="SOLAR_GAIN"
@@ -97,12 +92,10 @@
     def tag_flowers(self) -> list[S]:
         """Add ViSP specific tags to common tags."""
         return super().tag_flowers + [
             CSStepFlower(max_cs_step_time_sec=self.parameters.max_cs_step_time_sec),
             MapScanFlower(),
             VispTaskTypeFlower(),
             RasterScanStepFlower(),
-            SingleValueSingleKeyFlower(
-                tag_stem_name=VispStemName.modstate.value, metadata_key="modulator_state"
-            ),
+            ModulatorStateFlower(),
             ExposureTimeFlower(),
         ]
```

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/quality_metrics.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/science.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/solar.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/solar.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/trial_output_data.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/visp_base.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/visp_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tasks/write_l1.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/conftest.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_assemble_movie.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_background_light.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_background_light.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_build_quality_report.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_build_quality_report.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_dark.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_downsample.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_geometric.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_geometric.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_instrument_polarization.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_instrument_polarization.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_lamp.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_lamp.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_make_movie_frames.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_map_repeats.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_map_repeats.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 @pytest.fixture(scope="session")
 def complete_map_headers():
     num_steps = 5
     num_modstates = 4
     num_maps = 3
-    start_time = Time("1946-11-20T12:00:00")
+    start_time = Time("2020-11-20T12:00:00")
     dt = TimeDelta(10, format="sec")
     i = 0
     header_list = []
     map_number_list = []
     for map_scan in range(1, num_maps + 1):
         for step_num in range(0, num_steps):
             for modstate in range(1, num_modstates + 1):
@@ -59,15 +59,15 @@
 
 
 @pytest.fixture(scope="session")
 def map_headers_with_missing_steps():
     num_steps = 2
     num_modstates = 2
     num_maps = 3
-    start_time = Time("1946-11-20T12:00:00")
+    start_time = Time("2020-11-20T12:00:00")
     dt = TimeDelta(10, format="sec")
     i = 0
     header_list = []
     map_number_list = []
     for map_scan in range(1, num_maps + 1):
         for step_num in range(0, num_steps):
             if step_num == 0 and map_scan == 1:
```

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_parameters.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_parse.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_parse.py`

 * *Files 18% similar despite different names*

```diff
@@ -254,14 +254,76 @@
         except:
             raise
         finally:
             task.scratch.purge()
             task.constants._purge()
 
 
+@pytest.fixture
+def parse_task_with_intensity_observes_and_polarmetric_cals(
+    tmp_path, recipe_run_id, assign_input_dataset_doc_to_task
+):
+    num_maps = 1
+    num_observe_modstates = 1
+    num_calibration_modstates = 2
+    num_raster_steps = 3
+    with ParseL0VispInputData(
+        recipe_run_id=recipe_run_id,
+        workflow_name="parse_visp_input_data",
+        workflow_version="VX.Y",
+    ) as task:
+        try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
+            task._scratch = WorkflowFileSystem(
+                scratch_base_path=tmp_path, recipe_run_id=recipe_run_id
+            )
+            assign_input_dataset_doc_to_task(task, VispTestingParameters())
+            for map_scan in range(num_maps + 1):
+                for raster_step in range(num_raster_steps + 1):
+                    for observe_modstate in range(1, num_observe_modstates + 1):
+                        ds = VispHeadersValidObserveFrames(
+                            dataset_shape=(2, 2, 2),
+                            array_shape=(1, 2, 2),
+                            time_delta=10,
+                            num_modstates=num_observe_modstates,
+                            modstate=observe_modstate,
+                            num_raster_steps=num_raster_steps,
+                            raster_step=raster_step,
+                            polarimeter_mode="observe_intensity",
+                        )
+                        header = next(ds).header()
+                        translated_header = translate_spec122_to_spec214_l0(header)
+                        hdu = fits.PrimaryHDU(
+                            data=np.ones((1, 2, 2)), header=fits.Header(translated_header)
+                        )
+                        hdul = fits.HDUList([hdu])
+                        task.fits_data_write(hdu_list=hdul, tags=[Tag.input(), Tag.frame()])
+                    for calibration_modstate in range(1, num_calibration_modstates + 1):
+                        ds = VispHeadersValidLampGainFrames(
+                            dataset_shape=(2, 2, 2),
+                            array_shape=(1, 2, 2),
+                            time_delta=10,
+                            num_modstates=num_calibration_modstates,
+                            modstate=calibration_modstate,
+                            polarimeter_mode="dark_polarimetric",
+                        )
+                        header = next(ds).header()
+                        translated_header = translate_spec122_to_spec214_l0(header)
+                        hdu = fits.PrimaryHDU(
+                            data=np.ones((1, 2, 2)), header=fits.Header(translated_header)
+                        )
+                        hdul = fits.HDUList([hdu])
+                        task.fits_data_write(hdu_list=hdul, tags=[Tag.input(), Tag.frame()])
+            yield task
+        except:
+            raise
+        finally:
+            task.scratch.purge()
+            task.constants._purge()
+
+
 def test_parse_visp_input_data(parse_inputs_valid_task, mocker):
     """
     Given: A ParseVispInputData task
     When: Calling the task instance
     Then: All tagged files exist and individual task tags are applied
     """
     mocker.patch(
@@ -359,7 +421,27 @@
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
     task, num_steps, num_map_scans = parse_task_with_incomplete_final_map
     task()
     assert task.constants._db_dict["NUM_RASTER_STEPS"] == num_steps
     assert task.constants._db_dict["NUM_MAP_SCANS"] == num_map_scans - 1
+
+
+def test_intensity_observes_and_polarmetric_cals(
+    parse_task_with_intensity_observes_and_polarmetric_cals, mocker
+):
+    """
+    :Given: Data where the observe frames are in intensity mode and the calibration frames are in polarimetric mode
+    :When: Parsing the data
+    :Then: All modulator state keys generated for all frames are in the first modulator state
+    """
+    mocker.patch(
+        "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
+    )
+    task = parse_task_with_intensity_observes_and_polarmetric_cals
+    task()
+    assert task.constants._db_dict["NUM_MODSTATES"] == 1
+    assert task.constants._db_dict["POLARIMETER_MODE"] == "observe_intensity"
+    files = list(task.read(tags=[Tag.input(), Tag.frame()]))
+    for file in files:
+        assert "MODSTATE_1" in task.scratch.tags(file)
```

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_quality.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_science.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_solar.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_solar.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_submit_quality.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_submit_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_trial_output_data.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_visp_base.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_visp_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_visp_constants.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_visp_constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/tests/test_write_l1.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/workflows/l0_processing.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/workflows/l0_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp/workflows/trial_workflows.py` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/workflows/trial_workflows.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from dkist_processing_visp.tasks.background_light import BackgroundLightCalibration
 from dkist_processing_visp.tasks.dark import DarkCalibration
 from dkist_processing_visp.tasks.geometric import GeometricCalibration
 from dkist_processing_visp.tasks.instrument_polarization import InstrumentPolarizationCalibration
 from dkist_processing_visp.tasks.lamp import LampCalibration
 from dkist_processing_visp.tasks.parse import ParseL0VispInputData
-from dkist_processing_visp.tasks.quality_metrics import VispL0QualityMetrics
 from dkist_processing_visp.tasks.science import ScienceCalibration
 from dkist_processing_visp.tasks.solar import SolarCalibration
 from dkist_processing_visp.tasks.trial_output_data import TransferVispTrialData
 from dkist_processing_visp.tasks.write_l1 import VispWriteL1Frame
 
 non_science_trial_pipeline = Workflow(
     category="visp",
```

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp.egg-info/PKG-INFO` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-visp
-Version: 2.5.1
+Version: 2.6.0rc1
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp.egg-info/SOURCES.txt` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 check_changelog_updated.sh
 pyproject.toml
 science_towncrier.sh
 setup.cfg
 setup.py
 towncrier_science.toml
 changelog/.gitempty
+changelog/121.feature.rst
 dkist_processing_visp/__init__.py
 dkist_processing_visp.egg-info/PKG-INFO
 dkist_processing_visp.egg-info/SOURCES.txt
 dkist_processing_visp.egg-info/dependency_links.txt
 dkist_processing_visp.egg-info/requires.txt
 dkist_processing_visp.egg-info/top_level.txt
 dkist_processing_visp/fonts/Lato-Regular.ttf
 dkist_processing_visp/models/__init__.py
 dkist_processing_visp/models/constants.py
 dkist_processing_visp/models/parameters.py
 dkist_processing_visp/models/tags.py
 dkist_processing_visp/parsers/__init__.py
 dkist_processing_visp/parsers/map_repeats.py
+dkist_processing_visp/parsers/modulator_states.py
 dkist_processing_visp/parsers/polarimeter_mode.py
 dkist_processing_visp/parsers/raster_step.py
 dkist_processing_visp/parsers/task.py
 dkist_processing_visp/parsers/time.py
 dkist_processing_visp/parsers/visp_l0_fits_access.py
 dkist_processing_visp/parsers/visp_l1_fits_access.py
 dkist_processing_visp/parsers/wavelength.py
```

### Comparing `dkist_processing_visp-2.5.1/dkist_processing_visp.egg-info/requires.txt` & `dkist_processing_visp-2.6.0rc1/dkist_processing_visp.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/docs/Makefile` & `dkist_processing_visp-2.6.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/docs/background_light.rst` & `dkist_processing_visp-2.6.0rc1/docs/background_light.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/docs/conf.py` & `dkist_processing_visp-2.6.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/docs/gain_correction.rst` & `dkist_processing_visp-2.6.0rc1/docs/gain_correction.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/docs/l0_to_l1_visp.rst` & `dkist_processing_visp-2.6.0rc1/docs/l0_to_l1_visp.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/docs/make.bat` & `dkist_processing_visp-2.6.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/docs/polarization_calibration.rst` & `dkist_processing_visp-2.6.0rc1/docs/polarization_calibration.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/docs/science_calibration.rst` & `dkist_processing_visp-2.6.0rc1/docs/science_calibration.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/licenses/LICENSE.rst` & `dkist_processing_visp-2.6.0rc1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/pyproject.toml` & `dkist_processing_visp-2.6.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.5.1/setup.cfg` & `dkist_processing_visp-2.6.0rc1/setup.cfg`

 * *Files identical despite different names*

