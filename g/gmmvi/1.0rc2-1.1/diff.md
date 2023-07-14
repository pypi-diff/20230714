# Comparing `tmp/gmmvi-1.0rc2.tar.gz` & `tmp/gmmvi-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmmvi-1.0rc2.tar", last modified: Thu Jul 13 15:18:55 2023, max compression
+gzip compressed data, was "gmmvi-1.1.tar", last modified: Fri Jul 14 09:07:42 2023, max compression
```

## Comparing `gmmvi-1.0rc2.tar` & `gmmvi-1.1.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.818601 gmmvi-1.0rc2/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     4854 2023-07-13 09:10:01.000000 gmmvi-1.0rc2/.gitignore
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      663 2023-07-13 15:09:10.000000 gmmvi-1.0rc2/.readthedocs.yaml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1049 2023-07-13 13:59:44.000000 gmmvi-1.0rc2/LICENSE
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      619 2023-07-13 15:18:55.818601 gmmvi-1.0rc2/PKG-INFO
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      215 2023-02-09 15:57:08.000000 gmmvi-1.0rc2/README.rst
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.414598 gmmvi-1.0rc2/docs/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      638 2022-10-27 09:21:30.000000 gmmvi-1.0rc2/docs/Makefile
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      799 2022-10-27 09:21:30.000000 gmmvi-1.0rc2/docs/make.bat
--rwxrw-r-x   0 oleg      (1000) oleg      (1000)       48 2023-02-09 15:58:28.000000 gmmvi-1.0rc2/docs/make_docs.sh
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1855 2023-07-13 13:23:28.000000 gmmvi-1.0rc2/docs/requirements.txt
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.414598 gmmvi-1.0rc2/docs/source/
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.414598 gmmvi-1.0rc2/docs/source/_extensions/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1167 2023-07-13 14:21:08.000000 gmmvi-1.0rc2/docs/source/_extensions/autolink.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.414598 gmmvi-1.0rc2/docs/source/_templates/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      616 2023-07-13 14:21:08.000000 gmmvi-1.0rc2/docs/source/_templates/custom-class-template.rst
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1210 2023-07-13 14:21:08.000000 gmmvi-1.0rc2/docs/source/_templates/custom-module-template.rst
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     7136 2023-02-09 16:09:12.000000 gmmvi-1.0rc2/docs/source/about.rst
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      286 2023-02-07 10:23:01.000000 gmmvi-1.0rc2/docs/source/api.rst
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     6001 2023-07-13 15:04:56.000000 gmmvi-1.0rc2/docs/source/conf.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.414598 gmmvi-1.0rc2/docs/source/distributions/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      475 2023-02-02 13:58:05.000000 gmmvi-1.0rc2/docs/source/distributions/classes.rst
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.414598 gmmvi-1.0rc2/docs/source/experiments/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      175 2023-02-07 10:23:01.000000 gmmvi-1.0rc2/docs/source/experiments/classes.rst
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.414598 gmmvi-1.0rc2/docs/source/experiments/evaluation/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       88 2023-02-01 16:04:57.000000 gmmvi-1.0rc2/docs/source/experiments/evaluation/classes.rst
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.414598 gmmvi-1.0rc2/docs/source/experiments/target_distributions/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1507 2023-07-13 08:48:54.000000 gmmvi-1.0rc2/docs/source/experiments/target_distributions/classes.rst
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     4001 2023-07-13 08:48:51.000000 gmmvi-1.0rc2/docs/source/get_started.rst
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      725 2023-02-01 16:29:46.000000 gmmvi-1.0rc2/docs/source/index.rst
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.414598 gmmvi-1.0rc2/docs/source/optimization/
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.414598 gmmvi-1.0rc2/docs/source/optimization/Least_Squares/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      264 2023-02-07 10:23:01.000000 gmmvi-1.0rc2/docs/source/optimization/Least_Squares/classes.rst
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.414598 gmmvi-1.0rc2/docs/source/optimization/Modules/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      273 2023-02-09 08:06:41.000000 gmmvi-1.0rc2/docs/source/optimization/Modules/classes.rst
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.414598 gmmvi-1.0rc2/docs/source/optimization/Modules/component_adaptation/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      839 2023-02-09 15:12:08.000000 gmmvi-1.0rc2/docs/source/optimization/Modules/component_adaptation/classes.rst
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.414598 gmmvi-1.0rc2/docs/source/optimization/Modules/component_stepsize_adaptation/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1435 2023-02-09 15:19:17.000000 gmmvi-1.0rc2/docs/source/optimization/Modules/component_stepsize_adaptation/classes.rst
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.414598 gmmvi-1.0rc2/docs/source/optimization/Modules/ng_based_component_updater/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1304 2023-02-09 15:19:17.000000 gmmvi-1.0rc2/docs/source/optimization/Modules/ng_based_component_updater/classes.rst
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.414598 gmmvi-1.0rc2/docs/source/optimization/Modules/ng_estimator/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      721 2023-02-09 15:18:19.000000 gmmvi-1.0rc2/docs/source/optimization/Modules/ng_estimator/classes.rst
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.414598 gmmvi-1.0rc2/docs/source/optimization/Modules/sample_selector/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      732 2023-02-09 15:19:17.000000 gmmvi-1.0rc2/docs/source/optimization/Modules/sample_selector/classes.rst
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.414598 gmmvi-1.0rc2/docs/source/optimization/Modules/weight_stepsize_adaptation/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1366 2023-02-09 15:19:17.000000 gmmvi-1.0rc2/docs/source/optimization/Modules/weight_stepsize_adaptation/classes.rst
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.418598 gmmvi-1.0rc2/docs/source/optimization/Modules/weight_updater/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      832 2023-02-09 15:19:17.000000 gmmvi-1.0rc2/docs/source/optimization/Modules/weight_updater/classes.rst
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      317 2023-02-07 10:23:01.000000 gmmvi-1.0rc2/docs/source/optimization/classes.rst
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       80 2023-02-01 16:28:51.000000 gmmvi-1.0rc2/docs/source/references.rst
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     6276 2023-02-02 17:11:19.000000 gmmvi-1.0rc2/docs/source/refs.bib
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.442598 gmmvi-1.0rc2/examples/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     2321 2023-02-09 13:34:12.000000 gmmvi-1.0rc2/examples/1_directly_using_gmmvi.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      322 2023-02-09 13:15:07.000000 gmmvi-1.0rc2/examples/2_using_the_gmmvi_runner.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1870 2023-02-09 16:19:49.000000 gmmvi-1.0rc2/examples/3_gmmvi_runner_with_default_configs.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     3461 2023-02-09 13:44:37.000000 gmmvi-1.0rc2/examples/4_gmmvi_runner_with_custom_environments.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1900 2023-05-16 08:50:38.000000 gmmvi-1.0rc2/examples/5_samtron_20D_student-T.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     2704 2023-05-16 08:50:38.000000 gmmvi-1.0rc2/examples/6_samtron_planar4.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     2039 2023-07-13 07:54:13.000000 gmmvi-1.0rc2/examples/example_config.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1144 2023-07-13 14:59:41.000000 gmmvi-1.0rc2/pyproject.toml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       38 2023-07-13 15:18:55.818601 gmmvi-1.0rc2/setup.cfg
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.450598 gmmvi-1.0rc2/src/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2022-10-27 13:32:44.000000 gmmvi-1.0rc2/src/__init__.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.450598 gmmvi-1.0rc2/src/gmmvi/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2022-10-27 09:28:11.000000 gmmvi-1.0rc2/src/gmmvi/__init__.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.450598 gmmvi-1.0rc2/src/gmmvi/configs/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     2877 2023-02-07 10:23:01.000000 gmmvi-1.0rc2/src/gmmvi/configs/__init__.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.498599 gmmvi-1.0rc2/src/gmmvi/configs/experiment_configs/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      468 2023-07-13 08:47:49.000000 gmmvi-1.0rc2/src/gmmvi/configs/experiment_configs/breast_cancer.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      543 2023-07-13 08:47:49.000000 gmmvi-1.0rc2/src/gmmvi/configs/experiment_configs/breast_cancer_mb.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      501 2023-07-13 08:47:49.000000 gmmvi-1.0rc2/src/gmmvi/configs/experiment_configs/german_credit.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      576 2023-07-13 08:47:49.000000 gmmvi-1.0rc2/src/gmmvi/configs/experiment_configs/german_credit_mb.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      364 2022-12-30 07:56:40.000000 gmmvi-1.0rc2/src/gmmvi/configs/experiment_configs/gmm100.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      358 2022-12-30 07:56:40.000000 gmmvi-1.0rc2/src/gmmvi/configs/experiment_configs/gmm20.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      604 2023-07-13 08:47:49.000000 gmmvi-1.0rc2/src/gmmvi/configs/experiment_configs/planar_robot_4.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      412 2023-01-05 09:52:04.000000 gmmvi-1.0rc2/src/gmmvi/configs/experiment_configs/stm20.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      407 2022-12-30 07:56:40.000000 gmmvi-1.0rc2/src/gmmvi/configs/experiment_configs/stm300.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      364 2023-02-01 15:34:21.000000 gmmvi-1.0rc2/src/gmmvi/configs/experiment_configs/talos.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      391 2022-12-30 07:56:40.000000 gmmvi-1.0rc2/src/gmmvi/configs/experiment_configs/wine.yml
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.410598 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.510599 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/component_adaptation/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      295 2023-02-09 09:24:43.000000 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/component_adaptation/adaptive.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       69 2022-11-22 09:24:32.000000 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/component_adaptation/fixed.yml
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.522599 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/component_stepsize_adaptation/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      129 2022-11-22 09:24:32.000000 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/component_stepsize_adaptation/decaying.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      103 2022-11-22 09:24:32.000000 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/component_stepsize_adaptation/fixed.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      209 2022-11-22 09:24:32.000000 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/component_stepsize_adaptation/improvement-based.yml
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.530599 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/ng_based_component_updater/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       61 2022-11-22 09:24:32.000000 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/ng_based_component_updater/direct.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       60 2022-11-22 09:24:32.000000 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/ng_based_component_updater/iBLR.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       68 2022-11-22 09:24:32.000000 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/ng_based_component_updater/trust-region.yml
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.538599 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/ng_estimator/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      165 2022-11-29 18:34:52.000000 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/ng_estimator/MORE.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      124 2022-11-29 18:34:52.000000 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/ng_estimator/Stein.yml
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.538599 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/sample_selector/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      139 2023-07-13 07:54:13.000000 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/sample_selector/component-based.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      137 2023-07-13 07:54:13.000000 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/sample_selector/mixture-based.yml
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.538599 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/weight_stepsize_adaptation/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      125 2022-11-22 09:24:32.000000 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/weight_stepsize_adaptation/decaying.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       95 2022-11-22 09:24:32.000000 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/weight_stepsize_adaptation/fixed.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      206 2022-12-27 15:34:48.000000 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/weight_stepsize_adaptation/improvement-based.yml
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.554599 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/weight_updater/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      102 2022-11-27 09:47:54.000000 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/weight_updater/direct.yml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      108 2022-11-27 09:47:54.000000 gmmvi-1.0rc2/src/gmmvi/configs/module_configs/weight_updater/trust-region.yml
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.566599 gmmvi-1.0rc2/src/gmmvi/experiments/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2022-10-27 09:28:11.000000 gmmvi-1.0rc2/src/gmmvi/experiments/__init__.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.566599 gmmvi-1.0rc2/src/gmmvi/experiments/evaluation/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2022-10-27 13:32:44.000000 gmmvi-1.0rc2/src/gmmvi/experiments/evaluation/__init__.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     3456 2023-02-09 16:40:03.000000 gmmvi-1.0rc2/src/gmmvi/experiments/evaluation/mmd.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     6349 2023-05-16 08:50:38.000000 gmmvi-1.0rc2/src/gmmvi/experiments/evaluation/visualize_planar_robot.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     7031 2023-07-13 08:47:49.000000 gmmvi-1.0rc2/src/gmmvi/experiments/setup_experiment.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.566599 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2022-10-27 09:28:11.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/__init__.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)    21433 2023-02-07 10:23:01.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/bnn.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.590599 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)   124103 2022-10-27 09:28:11.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/breast_cancer.data
--rw-rw-r--   0 oleg      (1000) oleg      (1000)   102000 2022-10-27 09:28:11.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/german.data-numeric
--rw-rw-r--   0 oleg      (1000) oleg      (1000)   109543 2022-10-27 09:28:11.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/talos_reduced.urdf
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.790601 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)   236666 2022-10-27 09:28:11.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_0.npz
--rw-rw-r--   0 oleg      (1000) oleg      (1000)   236666 2022-10-27 09:28:11.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_1.npz
--rw-rw-r--   0 oleg      (1000) oleg      (1000)   236666 2022-10-27 09:28:11.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_2.npz
--rw-rw-r--   0 oleg      (1000) oleg      (1000)   236666 2022-10-27 09:28:11.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_3.npz
--rw-rw-r--   0 oleg      (1000) oleg      (1000)   236666 2022-10-27 09:28:11.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_4.npz
--rw-rw-r--   0 oleg      (1000) oleg      (1000)   236666 2022-10-27 09:28:11.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_5.npz
--rw-rw-r--   0 oleg      (1000) oleg      (1000)   236666 2022-10-27 09:28:11.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_6.npz
--rw-rw-r--   0 oleg      (1000) oleg      (1000)   236666 2022-10-27 09:28:11.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_7.npz
--rw-rw-r--   0 oleg      (1000) oleg      (1000)   236666 2022-10-27 09:28:11.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_8.npz
--rw-rw-r--   0 oleg      (1000) oleg      (1000)   236666 2022-10-27 09:28:11.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_9.npz
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1555 2022-11-29 18:34:52.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/diag_gmm.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     9140 2023-07-13 08:48:54.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/gmm.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     5352 2023-07-13 08:48:54.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/lnpdf.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     8194 2023-07-13 08:47:49.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/logistic_regression.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     6264 2023-07-13 11:40:20.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/planar_robot.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     9383 2023-05-16 08:50:38.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/student_t_mixture.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     9028 2023-07-13 08:48:56.000000 gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/talos_ik.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     8467 2023-02-14 08:32:14.000000 gmmvi-1.0rc2/src/gmmvi/gmmvi_runner.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.814601 gmmvi-1.0rc2/src/gmmvi/models/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2022-10-27 09:28:11.000000 gmmvi-1.0rc2/src/gmmvi/models/__init__.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     2970 2023-07-13 07:54:13.000000 gmmvi-1.0rc2/src/gmmvi/models/diagonal_gmm.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     3758 2023-07-13 07:54:13.000000 gmmvi-1.0rc2/src/gmmvi/models/full_cov_gmm.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)    18140 2023-07-13 07:54:13.000000 gmmvi-1.0rc2/src/gmmvi/models/gmm.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)    10520 2023-02-09 13:55:58.000000 gmmvi-1.0rc2/src/gmmvi/models/gmm_wrapper.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.814601 gmmvi-1.0rc2/src/gmmvi/optimization/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2022-10-27 09:28:11.000000 gmmvi-1.0rc2/src/gmmvi/optimization/__init__.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)    10285 2023-02-14 09:01:56.000000 gmmvi-1.0rc2/src/gmmvi/optimization/gmmvi.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.818601 gmmvi-1.0rc2/src/gmmvi/optimization/gmmvi_modules/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2022-10-27 09:28:11.000000 gmmvi-1.0rc2/src/gmmvi/optimization/gmmvi_modules/__init__.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)    15715 2023-02-09 08:06:41.000000 gmmvi-1.0rc2/src/gmmvi/optimization/gmmvi_modules/component_adaptation.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     8375 2023-02-09 08:06:41.000000 gmmvi-1.0rc2/src/gmmvi/optimization/gmmvi_modules/component_stepsize_adaptation.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)    25916 2023-02-14 14:43:59.000000 gmmvi-1.0rc2/src/gmmvi/optimization/gmmvi_modules/ng_based_component_updater.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)    22201 2023-05-30 11:51:36.000000 gmmvi-1.0rc2/src/gmmvi/optimization/gmmvi_modules/ng_estimator.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)    17985 2023-07-13 07:54:13.000000 gmmvi-1.0rc2/src/gmmvi/optimization/gmmvi_modules/sample_selector.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     6578 2023-02-09 10:02:23.000000 gmmvi-1.0rc2/src/gmmvi/optimization/gmmvi_modules/weight_stepsize_adaptation.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)    14301 2023-02-09 08:06:41.000000 gmmvi-1.0rc2/src/gmmvi/optimization/gmmvi_modules/weight_updater.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     6905 2023-07-13 08:47:49.000000 gmmvi-1.0rc2/src/gmmvi/optimization/least_squares.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)    11095 2023-02-07 10:23:01.000000 gmmvi-1.0rc2/src/gmmvi/optimization/sample_db.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-13 15:18:55.450598 gmmvi-1.0rc2/src/gmmvi.egg-info/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      619 2023-07-13 15:18:55.000000 gmmvi-1.0rc2/src/gmmvi.egg-info/PKG-INFO
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     5909 2023-07-13 15:18:55.000000 gmmvi-1.0rc2/src/gmmvi.egg-info/SOURCES.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        1 2023-07-13 15:18:55.000000 gmmvi-1.0rc2/src/gmmvi.egg-info/dependency_links.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      244 2023-07-13 15:18:55.000000 gmmvi-1.0rc2/src/gmmvi.egg-info/requires.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       15 2023-07-13 15:18:55.000000 gmmvi-1.0rc2/src/gmmvi.egg-info/top_level.txt
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.283436 gmmvi-1.1/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     4854 2023-07-14 07:50:52.000000 gmmvi-1.1/.gitignore
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      738 2023-07-14 09:05:06.000000 gmmvi-1.1/.readthedocs.yaml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1049 2023-07-14 07:50:52.000000 gmmvi-1.1/LICENSE
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      665 2023-07-14 09:07:42.283436 gmmvi-1.1/PKG-INFO
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      264 2023-07-14 09:05:06.000000 gmmvi-1.1/README.rst
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.275436 gmmvi-1.1/docs/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      638 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/Makefile
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      799 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/make.bat
+-rwxrwxr-x   0 oleg      (1000) oleg      (1000)       48 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/make_docs.sh
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1855 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/requirements.txt
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.275436 gmmvi-1.1/docs/source/
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.275436 gmmvi-1.1/docs/source/_extensions/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1162 2023-07-14 09:05:06.000000 gmmvi-1.1/docs/source/_extensions/autolink.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.275436 gmmvi-1.1/docs/source/_templates/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      616 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/source/_templates/custom-class-template.rst
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1210 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/source/_templates/custom-module-template.rst
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     7395 2023-07-14 09:05:06.000000 gmmvi-1.1/docs/source/about.rst
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      286 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/source/api.rst
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     6001 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/source/conf.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.275436 gmmvi-1.1/docs/source/distributions/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      475 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/source/distributions/classes.rst
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.275436 gmmvi-1.1/docs/source/experiments/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      175 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/source/experiments/classes.rst
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.275436 gmmvi-1.1/docs/source/experiments/evaluation/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       88 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/source/experiments/evaluation/classes.rst
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.275436 gmmvi-1.1/docs/source/experiments/target_distributions/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1507 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/source/experiments/target_distributions/classes.rst
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     4001 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/source/get_started.rst
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      720 2023-07-14 09:05:06.000000 gmmvi-1.1/docs/source/index.rst
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.275436 gmmvi-1.1/docs/source/optimization/
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.275436 gmmvi-1.1/docs/source/optimization/Least_Squares/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      264 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/source/optimization/Least_Squares/classes.rst
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.275436 gmmvi-1.1/docs/source/optimization/Modules/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      273 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/source/optimization/Modules/classes.rst
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.275436 gmmvi-1.1/docs/source/optimization/Modules/component_adaptation/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      839 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/source/optimization/Modules/component_adaptation/classes.rst
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.275436 gmmvi-1.1/docs/source/optimization/Modules/component_stepsize_adaptation/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1435 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/source/optimization/Modules/component_stepsize_adaptation/classes.rst
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.275436 gmmvi-1.1/docs/source/optimization/Modules/ng_based_component_updater/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1304 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/source/optimization/Modules/ng_based_component_updater/classes.rst
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.275436 gmmvi-1.1/docs/source/optimization/Modules/ng_estimator/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      721 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/source/optimization/Modules/ng_estimator/classes.rst
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.275436 gmmvi-1.1/docs/source/optimization/Modules/sample_selector/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      732 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/source/optimization/Modules/sample_selector/classes.rst
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.275436 gmmvi-1.1/docs/source/optimization/Modules/weight_stepsize_adaptation/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1366 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/source/optimization/Modules/weight_stepsize_adaptation/classes.rst
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.279436 gmmvi-1.1/docs/source/optimization/Modules/weight_updater/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      832 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/source/optimization/Modules/weight_updater/classes.rst
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      317 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/source/optimization/classes.rst
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       80 2023-07-14 07:50:52.000000 gmmvi-1.1/docs/source/references.rst
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     6608 2023-07-14 09:05:06.000000 gmmvi-1.1/docs/source/refs.bib
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.279436 gmmvi-1.1/examples/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2321 2023-07-14 07:50:52.000000 gmmvi-1.1/examples/1_directly_using_gmmvi.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      322 2023-07-14 07:50:52.000000 gmmvi-1.1/examples/2_using_the_gmmvi_runner.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1870 2023-07-14 07:50:52.000000 gmmvi-1.1/examples/3_gmmvi_runner_with_default_configs.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     3461 2023-07-14 07:50:52.000000 gmmvi-1.1/examples/4_gmmvi_runner_with_custom_environments.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1900 2023-07-14 07:50:52.000000 gmmvi-1.1/examples/5_samtron_20D_student-T.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2704 2023-07-14 07:50:52.000000 gmmvi-1.1/examples/6_samtron_planar4.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2039 2023-07-14 07:50:52.000000 gmmvi-1.1/examples/example_config.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1144 2023-07-14 07:50:52.000000 gmmvi-1.1/pyproject.toml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       38 2023-07-14 09:07:42.283436 gmmvi-1.1/setup.cfg
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.279436 gmmvi-1.1/src/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2023-07-14 07:50:52.000000 gmmvi-1.1/src/__init__.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.279436 gmmvi-1.1/src/gmmvi/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/__init__.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.279436 gmmvi-1.1/src/gmmvi/configs/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2877 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/__init__.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.279436 gmmvi-1.1/src/gmmvi/configs/experiment_configs/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      468 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/experiment_configs/breast_cancer.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      543 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/experiment_configs/breast_cancer_mb.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      501 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/experiment_configs/german_credit.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      576 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/experiment_configs/german_credit_mb.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      364 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/experiment_configs/gmm100.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      358 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/experiment_configs/gmm20.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      604 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/experiment_configs/planar_robot_4.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      412 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/experiment_configs/stm20.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      407 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/experiment_configs/stm300.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      364 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/experiment_configs/talos.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      391 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/experiment_configs/wine.yml
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.275436 gmmvi-1.1/src/gmmvi/configs/module_configs/
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.279436 gmmvi-1.1/src/gmmvi/configs/module_configs/component_adaptation/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      295 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/module_configs/component_adaptation/adaptive.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       69 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/module_configs/component_adaptation/fixed.yml
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.279436 gmmvi-1.1/src/gmmvi/configs/module_configs/component_stepsize_adaptation/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      129 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/module_configs/component_stepsize_adaptation/decaying.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      103 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/module_configs/component_stepsize_adaptation/fixed.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      209 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/module_configs/component_stepsize_adaptation/improvement-based.yml
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.279436 gmmvi-1.1/src/gmmvi/configs/module_configs/ng_based_component_updater/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       61 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/module_configs/ng_based_component_updater/direct.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       60 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/module_configs/ng_based_component_updater/iBLR.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       68 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/module_configs/ng_based_component_updater/trust-region.yml
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.279436 gmmvi-1.1/src/gmmvi/configs/module_configs/ng_estimator/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      165 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/module_configs/ng_estimator/MORE.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      124 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/module_configs/ng_estimator/Stein.yml
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.279436 gmmvi-1.1/src/gmmvi/configs/module_configs/sample_selector/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      139 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/module_configs/sample_selector/component-based.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      137 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/module_configs/sample_selector/mixture-based.yml
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.279436 gmmvi-1.1/src/gmmvi/configs/module_configs/weight_stepsize_adaptation/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      125 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/module_configs/weight_stepsize_adaptation/decaying.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       95 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/module_configs/weight_stepsize_adaptation/fixed.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      206 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/module_configs/weight_stepsize_adaptation/improvement-based.yml
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.279436 gmmvi-1.1/src/gmmvi/configs/module_configs/weight_updater/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      102 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/module_configs/weight_updater/direct.yml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      108 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/configs/module_configs/weight_updater/trust-region.yml
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.279436 gmmvi-1.1/src/gmmvi/experiments/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/__init__.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.279436 gmmvi-1.1/src/gmmvi/experiments/evaluation/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/evaluation/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     3456 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/evaluation/mmd.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     6349 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/evaluation/visualize_planar_robot.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     7031 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/setup_experiment.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.279436 gmmvi-1.1/src/gmmvi/experiments/target_distributions/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)    21433 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/bnn.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.279436 gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)   124103 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/breast_cancer.data
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)   102000 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/german.data-numeric
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)   109543 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/talos_reduced.urdf
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.283436 gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)   236666 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_0.npz
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)   236666 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_1.npz
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)   236666 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_2.npz
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)   236666 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_3.npz
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)   236666 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_4.npz
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)   236666 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_5.npz
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)   236666 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_6.npz
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)   236666 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_7.npz
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)   236666 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_8.npz
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)   236666 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_9.npz
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1555 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/diag_gmm.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     9140 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/gmm.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5352 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/lnpdf.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     8194 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/logistic_regression.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     6264 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/planar_robot.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     9383 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/student_t_mixture.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     9161 2023-07-14 09:05:06.000000 gmmvi-1.1/src/gmmvi/experiments/target_distributions/talos_ik.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     8467 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/gmmvi_runner.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.283436 gmmvi-1.1/src/gmmvi/models/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/models/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2970 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/models/diagonal_gmm.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     3758 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/models/full_cov_gmm.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)    18140 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/models/gmm.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)    10520 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/models/gmm_wrapper.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.283436 gmmvi-1.1/src/gmmvi/optimization/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/optimization/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)    10285 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/optimization/gmmvi.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.283436 gmmvi-1.1/src/gmmvi/optimization/gmmvi_modules/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        0 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/optimization/gmmvi_modules/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)    15715 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/optimization/gmmvi_modules/component_adaptation.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     8375 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/optimization/gmmvi_modules/component_stepsize_adaptation.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)    25916 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/optimization/gmmvi_modules/ng_based_component_updater.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)    22201 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/optimization/gmmvi_modules/ng_estimator.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)    17985 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/optimization/gmmvi_modules/sample_selector.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     6578 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/optimization/gmmvi_modules/weight_stepsize_adaptation.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)    14301 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/optimization/gmmvi_modules/weight_updater.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     6905 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/optimization/least_squares.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)    11095 2023-07-14 07:50:52.000000 gmmvi-1.1/src/gmmvi/optimization/sample_db.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-07-14 09:07:42.279436 gmmvi-1.1/src/gmmvi.egg-info/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      665 2023-07-14 09:07:42.000000 gmmvi-1.1/src/gmmvi.egg-info/PKG-INFO
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     5909 2023-07-14 09:07:42.000000 gmmvi-1.1/src/gmmvi.egg-info/SOURCES.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        1 2023-07-14 09:07:42.000000 gmmvi-1.1/src/gmmvi.egg-info/dependency_links.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      244 2023-07-14 09:07:42.000000 gmmvi-1.1/src/gmmvi.egg-info/requires.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       15 2023-07-14 09:07:42.000000 gmmvi-1.1/src/gmmvi.egg-info/top_level.txt
```

### Comparing `gmmvi-1.0rc2/.gitignore` & `gmmvi-1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/.readthedocs.yaml` & `gmmvi-1.1/.readthedocs.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
   tools:
     python: "3.10"
   apt_packages:
     - graphviz
   jobs:
     post_install:
       - pip install .[doc]
+      - pip install git+https://github.com/OlegArenz/tf_robot_learning.git
 
 # Build documentation in the docs/ directory with Sphinx
 sphinx:
   configuration: docs/source/conf.py
 
 # We recommend specifying your dependencies to enable reproducible builds:
 # https://docs.readthedocs.io/en/stable/guides/reproducible-builds.html
```

### Comparing `gmmvi-1.0rc2/LICENSE` & `gmmvi-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/PKG-INFO` & `gmmvi-1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: gmmvi
-Version: 1.0rc2
+Version: 1.1
 Summary: A library for learning Gaussian mixture models for variational inference
 Author: Oleg Arenz
 Author-email: oleg@holistic-robotics.de
 License: MIT
 Keywords: variational inference,machine learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: doc
 License-File: LICENSE
 
 GMMVI: Gaussian Mixture Model Variational Inference
 ===================================================
 
-The documentation is provided as `html <docs/build/html/index.html>`_ or `pdf <docs/build/latex/gmmvi.pdf>`_.
+A framework for optimizing Gaussian mixture models for variational inference.
+Please refer to the `online documentation <https://gmmvi.rtfd.io>`_ for details.
```

### Comparing `gmmvi-1.0rc2/docs/Makefile` & `gmmvi-1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/docs/make.bat` & `gmmvi-1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/docs/requirements.txt` & `gmmvi-1.1/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/docs/source/_extensions/autolink.py` & `gmmvi-1.1/docs/source/_extensions/autolink.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     if len(tag):
         print('Git tag: ', tag)
         path = tag
     return path
 
 
 def setup(app):
-    baseurl = 'https://github.com/OlegArenz/gmmvi_test'
+    baseurl = 'https://github.com/OlegArenz/gmmvi'
     rev = get_github_rev()
     app.add_role('gitlink', autolink('{}/tree/{}/%s'.format(baseurl, rev)))
     app.add_role('example', autolink('{}/tree/{}/examples/%s'.format(baseurl, rev)))
     app.add_role('example_file', autolink('{}/blob/{}/examples/%s'.format(baseurl, rev)))
     app.add_role('example_raw', autolink('{}/raw/{}/examples/%s'.format(baseurl, rev)))
```

### Comparing `gmmvi-1.0rc2/docs/source/_templates/custom-class-template.rst` & `gmmvi-1.1/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/docs/source/_templates/custom-module-template.rst` & `gmmvi-1.1/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/docs/source/about.rst` & `gmmvi-1.1/docs/source/about.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 About
 =====
 
-GMMVI (Gaussian Mixture Model Variational Inference) is a framework for optimizing a Gaussian mixture model
+GMMVI (Gaussian Mixture Model Variational Inference) is a framework for learning GMMS for variational inference,
+that was released along with the article :cite:p:`Arenz2023`.
+
+Formally, we aim to optimize a GMM
 :math:`q(\mathbf{x})` with Gaussian components :math:`q(\mathbf{x}|o)` and weights :math:`q(o)`,
 
 .. math::
     q(\mathbf{x}) = \sum_o q(o) q(\mathbf{x}|o),
 
 with respect to the optimization problem,
 
@@ -26,16 +29,17 @@
 ------
 The optimization is performed iteratively, where at every iteration an independent natural gradient descent step is
 performed to the categorical distribution over weights, :math:`q(o)`, and to each individual component
 :math:`q(\mathbf{x}|o)`. This procedure was concurrently proposed by :cite:t:`Arenz2018` and :cite:t:`Lin2019`.
 However, both approaches differ quite significantly in several design choices (e.g. how the natural gradients are
 estimated) and derived the procedure from different perspectives with different theoretical guarantees, and therefore
 the equivalence of both approaches was initially not understand. This framework is published along with the article
-that first established the close connection between both approaches, and was used to systematically evaluate the
-effects of the different design choices.
+:cite:p:`Arenz2023` that first established the close connection between both approaches, and was used to systematically evaluate the
+effects of the different design choices. For reproducing these experiments, please refer to our
+`reproducibility package <https://github.com/OlegArenz/gmmvi-reproducibility>`_.
 
 .. _design choices:
 
 Design Choices
 --------------
 We distinguish design choices for seven different :ref:`modules <gmmvi-modules>` corresponding to the abstract classes,
 where for each design choice, there are two to three option implemented as concrete classes.
```

### Comparing `gmmvi-1.0rc2/docs/source/conf.py` & `gmmvi-1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/docs/source/experiments/target_distributions/classes.rst` & `gmmvi-1.1/docs/source/experiments/target_distributions/classes.rst`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/docs/source/get_started.rst` & `gmmvi-1.1/docs/source/get_started.rst`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/docs/source/index.rst` & `gmmvi-1.1/docs/source/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 If you don't quite know how you ended up here,
 check out the :doc:`about` page, for more details on the problem setting and the underlying algorithms.
 
 Just wanna know how do :ref:`install<installation>` and :ref:`use<usage>` the framework? :doc:`Get Started<get_started>`!
 
 For a look under the hood, you can check the :doc:`api` or directly dig into the source on the
-`Github page <https://github.com/OlegArenz/gmmvi_test>`_.
+`Github page <https://github.com/OlegArenz/gmmvi>`_.
 
 .. toctree::
    about
    get_started
    api
    references
    :hidden:
```

### Comparing `gmmvi-1.0rc2/docs/source/optimization/Modules/component_adaptation/classes.rst` & `gmmvi-1.1/docs/source/optimization/Modules/component_adaptation/classes.rst`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/docs/source/optimization/Modules/component_stepsize_adaptation/classes.rst` & `gmmvi-1.1/docs/source/optimization/Modules/component_stepsize_adaptation/classes.rst`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/docs/source/optimization/Modules/ng_based_component_updater/classes.rst` & `gmmvi-1.1/docs/source/optimization/Modules/ng_based_component_updater/classes.rst`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/docs/source/optimization/Modules/ng_estimator/classes.rst` & `gmmvi-1.1/docs/source/optimization/Modules/ng_estimator/classes.rst`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/docs/source/optimization/Modules/sample_selector/classes.rst` & `gmmvi-1.1/docs/source/optimization/Modules/sample_selector/classes.rst`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/docs/source/optimization/Modules/weight_stepsize_adaptation/classes.rst` & `gmmvi-1.1/docs/source/optimization/Modules/weight_stepsize_adaptation/classes.rst`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/docs/source/optimization/Modules/weight_updater/classes.rst` & `gmmvi-1.1/docs/source/optimization/Modules/weight_updater/classes.rst`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/docs/source/refs.bib` & `gmmvi-1.1/docs/source/refs.bib`

 * *Files 3% similar despite different names*

```diff
@@ -116,8 +116,16 @@
   organization={PMLR}
 }
 @InProceedings{Arenz2018,
   title = 	 {Efficient Gradient-Free Variational Inference using Policy Search},
   author = 	 {Arenz, O. and Zhong, M. and Neumann, G.},
   booktitle = 	 {International Conference on Machine Learning (ICML)},
   year = 	 {2018},
+}
+@article{
+  Arenz2023,
+  title={A Unified Perspective on Natural Gradient Variational Inference with Gaussian Mixture Models},
+  author={Arenz, O. and Dahlinger, P. and Ye, Z. and Volpp, M. and Neumann, G.},
+  journal={Transactions on Machine Learning Research},
+  year={2023},
+  url={https://openreview.net/forum?id=tLBjsX4tjs},
 }
```

### Comparing `gmmvi-1.0rc2/examples/1_directly_using_gmmvi.py` & `gmmvi-1.1/examples/1_directly_using_gmmvi.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/examples/3_gmmvi_runner_with_default_configs.py` & `gmmvi-1.1/examples/3_gmmvi_runner_with_default_configs.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/examples/4_gmmvi_runner_with_custom_environments.py` & `gmmvi-1.1/examples/4_gmmvi_runner_with_custom_environments.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/examples/5_samtron_20D_student-T.py` & `gmmvi-1.1/examples/5_samtron_20D_student-T.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/examples/6_samtron_planar4.py` & `gmmvi-1.1/examples/6_samtron_planar4.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/examples/example_config.yml` & `gmmvi-1.1/examples/example_config.yml`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/pyproject.toml` & `gmmvi-1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/configs/__init__.py` & `gmmvi-1.1/src/gmmvi/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/configs/experiment_configs/breast_cancer_mb.yml` & `gmmvi-1.1/src/gmmvi/configs/experiment_configs/breast_cancer_mb.yml`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/configs/experiment_configs/german_credit_mb.yml` & `gmmvi-1.1/src/gmmvi/configs/experiment_configs/german_credit_mb.yml`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/configs/experiment_configs/planar_robot_4.yml` & `gmmvi-1.1/src/gmmvi/configs/experiment_configs/planar_robot_4.yml`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/evaluation/mmd.py` & `gmmvi-1.1/src/gmmvi/experiments/evaluation/mmd.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/evaluation/visualize_planar_robot.py` & `gmmvi-1.1/src/gmmvi/experiments/evaluation/visualize_planar_robot.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/setup_experiment.py` & `gmmvi-1.1/src/gmmvi/experiments/setup_experiment.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/bnn.py` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/bnn.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/breast_cancer.data` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/breast_cancer.data`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/german.data-numeric` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/german.data-numeric`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/talos_reduced.urdf` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/talos_reduced.urdf`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_0.npz` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_0.npz`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_1.npz` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_1.npz`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_2.npz` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_2.npz`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_3.npz` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_3.npz`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_4.npz` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_4.npz`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_5.npz` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_5.npz`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_6.npz` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_6.npz`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_7.npz` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_7.npz`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_8.npz` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_8.npz`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_9.npz` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/datasets/wine/wine_seed_9.npz`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/diag_gmm.py` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/diag_gmm.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/gmm.py` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/gmm.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/lnpdf.py` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/lnpdf.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/logistic_regression.py` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/planar_robot.py` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/planar_robot.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/student_t_mixture.py` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/student_t_mixture.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/experiments/target_distributions/talos_ik.py` & `gmmvi-1.1/src/gmmvi/experiments/target_distributions/talos_ik.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 
 class Talos(LNPDF):
     """
     The target distribution for the humanoid inverse kinematik problem. The unnormalized target distribution is given
     by a mixture of experts, that penalize the task space error of the left endeffector, joint-limit violations,
     unstable configurations, etc.
 
+    This class requires a fork of tf_robot_learning that can be found
+    `here <https://github.com/OlegArenz/tf_robot_learning>`_.
+
     Parameters:
         context: list[float]
             A list of three floats, specifying the desired x, y, z coordinates of the left endeffector.
     """
 
     def __init__(self, context):
         super().__init__(use_log_density_and_grad=True, safe_for_tf_graph=False)
```

### Comparing `gmmvi-1.0rc2/src/gmmvi/gmmvi_runner.py` & `gmmvi-1.1/src/gmmvi/gmmvi_runner.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/models/diagonal_gmm.py` & `gmmvi-1.1/src/gmmvi/models/diagonal_gmm.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/models/full_cov_gmm.py` & `gmmvi-1.1/src/gmmvi/models/full_cov_gmm.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/models/gmm.py` & `gmmvi-1.1/src/gmmvi/models/gmm.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/models/gmm_wrapper.py` & `gmmvi-1.1/src/gmmvi/models/gmm_wrapper.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/optimization/gmmvi.py` & `gmmvi-1.1/src/gmmvi/optimization/gmmvi.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/optimization/gmmvi_modules/component_adaptation.py` & `gmmvi-1.1/src/gmmvi/optimization/gmmvi_modules/component_adaptation.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/optimization/gmmvi_modules/component_stepsize_adaptation.py` & `gmmvi-1.1/src/gmmvi/optimization/gmmvi_modules/component_stepsize_adaptation.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/optimization/gmmvi_modules/ng_based_component_updater.py` & `gmmvi-1.1/src/gmmvi/optimization/gmmvi_modules/ng_based_component_updater.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/optimization/gmmvi_modules/ng_estimator.py` & `gmmvi-1.1/src/gmmvi/optimization/gmmvi_modules/ng_estimator.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/optimization/gmmvi_modules/sample_selector.py` & `gmmvi-1.1/src/gmmvi/optimization/gmmvi_modules/sample_selector.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/optimization/gmmvi_modules/weight_stepsize_adaptation.py` & `gmmvi-1.1/src/gmmvi/optimization/gmmvi_modules/weight_stepsize_adaptation.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/optimization/gmmvi_modules/weight_updater.py` & `gmmvi-1.1/src/gmmvi/optimization/gmmvi_modules/weight_updater.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/optimization/least_squares.py` & `gmmvi-1.1/src/gmmvi/optimization/least_squares.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi/optimization/sample_db.py` & `gmmvi-1.1/src/gmmvi/optimization/sample_db.py`

 * *Files identical despite different names*

### Comparing `gmmvi-1.0rc2/src/gmmvi.egg-info/PKG-INFO` & `gmmvi-1.1/src/gmmvi.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: gmmvi
-Version: 1.0rc2
+Version: 1.1
 Summary: A library for learning Gaussian mixture models for variational inference
 Author: Oleg Arenz
 Author-email: oleg@holistic-robotics.de
 License: MIT
 Keywords: variational inference,machine learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: doc
 License-File: LICENSE
 
 GMMVI: Gaussian Mixture Model Variational Inference
 ===================================================
 
-The documentation is provided as `html <docs/build/html/index.html>`_ or `pdf <docs/build/latex/gmmvi.pdf>`_.
+A framework for optimizing Gaussian mixture models for variational inference.
+Please refer to the `online documentation <https://gmmvi.rtfd.io>`_ for details.
```

### Comparing `gmmvi-1.0rc2/src/gmmvi.egg-info/SOURCES.txt` & `gmmvi-1.1/src/gmmvi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

