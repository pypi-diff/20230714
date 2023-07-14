# Comparing `tmp/pyblp-1.0.0.tar.gz` & `tmp/pyblp-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyblp-1.0.0.tar", last modified: Wed Apr 19 16:31:37 2023, max compression
+gzip compressed data, was "dist\pyblp-1.1.0.tar", last modified: Fri Jul 14 20:26:35 2023, max compression
```

## Comparing `pyblp-1.0.0.tar` & `pyblp-1.1.0.tar`

### file list

```diff
@@ -1,141 +1,144 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 16:31:37.000000 pyblp-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-04-19 16:31:37.000000 pyblp-1.0.0/docs/
--rw-rw-rw-   0        0        0    11617 2022-08-01 20:06:35.000000 pyblp-1.0.0/docs/api.rst
--rw-rw-rw-   0        0        0    27034 2023-04-18 19:22:14.000000 pyblp-1.0.0/docs/background.rst
--rw-rw-rw-   0        0        0     7077 2023-04-19 16:18:14.000000 pyblp-1.0.0/docs/conf.py
--rw-rw-rw-   0        0        0      347 2023-01-25 21:32:43.000000 pyblp-1.0.0/docs/contributing.rst
--rw-rw-rw-   0        0        0      670 2021-06-11 17:07:44.000000 pyblp-1.0.0/docs/index.rst
--rw-rw-rw-   0        0        0       87 2023-04-18 19:16:57.000000 pyblp-1.0.0/docs/introduction.rst
--rw-rw-rw-   0        0        0       45 2021-06-11 17:07:44.000000 pyblp-1.0.0/docs/legal.rst
--rw-rw-rw-   0        0        0    12162 2022-06-08 19:22:02.000000 pyblp-1.0.0/docs/notation.rst
-drwxrwxrwx   0        0        0        0 2023-04-19 16:31:37.000000 pyblp-1.0.0/docs/notebooks/
-drwxrwxrwx   0        0        0        0 2023-04-19 16:31:37.000000 pyblp-1.0.0/docs/notebooks/api/
-drwxrwxrwx   0        0        0        0 2023-04-19 16:31:37.000000 pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0    31385 2023-04-18 19:29:13.000000 pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/build_blp_instruments-checkpoint.ipynb
--rw-rw-rw-   0        0        0    29293 2023-04-18 19:30:07.000000 pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/build_differentiation_instruments-checkpoint.ipynb
--rw-rw-rw-   0        0        0     1891 2023-04-18 19:30:10.000000 pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/build_id_data-checkpoint.ipynb
--rw-rw-rw-   0        0        0     3232 2023-04-18 19:30:11.000000 pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/build_integration-checkpoint.ipynb
--rw-rw-rw-   0        0        0    12117 2023-04-18 19:30:13.000000 pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/build_matrix-checkpoint.ipynb
--rw-rw-rw-   0        0        0     5439 2023-04-18 19:30:15.000000 pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/build_ownership-checkpoint.ipynb
--rw-rw-rw-   0        0        0    14521 2023-04-18 19:30:17.000000 pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/data-checkpoint.ipynb
--rw-rw-rw-   0        0        0    20517 2023-04-18 19:30:19.000000 pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/data_to_dict-checkpoint.ipynb
--rw-rw-rw-   0        0        0     3514 2023-04-18 19:30:20.000000 pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/formulation-checkpoint.ipynb
--rw-rw-rw-   0        0        0     2478 2023-04-18 19:30:22.000000 pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/integration-checkpoint.ipynb
--rw-rw-rw-   0        0        0     3467 2023-04-18 19:30:24.000000 pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/iteration-checkpoint.ipynb
--rw-rw-rw-   0        0        0     4060 2023-01-12 23:16:23.000000 pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/micro_dataset-checkpoint.ipynb
--rw-rw-rw-   0        0        0     3405 2023-01-12 23:16:20.000000 pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/micro_part-checkpoint.ipynb
--rw-rw-rw-   0        0        0     3106 2023-04-18 19:30:26.000000 pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/optimization-checkpoint.ipynb
--rw-rw-rw-   0        0        0     3926 2023-04-18 19:30:27.000000 pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/parallel-checkpoint.ipynb
--rw-rw-rw-   0        0        0    31385 2023-04-18 19:29:13.000000 pyblp-1.0.0/docs/notebooks/api/build_blp_instruments.ipynb
--rw-rw-rw-   0        0        0    29293 2023-04-18 19:30:07.000000 pyblp-1.0.0/docs/notebooks/api/build_differentiation_instruments.ipynb
--rw-rw-rw-   0        0        0     1891 2023-04-18 19:30:10.000000 pyblp-1.0.0/docs/notebooks/api/build_id_data.ipynb
--rw-rw-rw-   0        0        0     3232 2023-04-18 19:30:11.000000 pyblp-1.0.0/docs/notebooks/api/build_integration.ipynb
--rw-rw-rw-   0        0        0    12117 2023-04-18 19:30:13.000000 pyblp-1.0.0/docs/notebooks/api/build_matrix.ipynb
--rw-rw-rw-   0        0        0     5439 2023-04-18 19:30:15.000000 pyblp-1.0.0/docs/notebooks/api/build_ownership.ipynb
--rw-rw-rw-   0        0        0    14521 2023-04-18 19:30:17.000000 pyblp-1.0.0/docs/notebooks/api/data.ipynb
--rw-rw-rw-   0        0        0    20517 2023-04-18 19:30:19.000000 pyblp-1.0.0/docs/notebooks/api/data_to_dict.ipynb
--rw-rw-rw-   0        0        0     3514 2023-04-18 19:30:20.000000 pyblp-1.0.0/docs/notebooks/api/formulation.ipynb
--rw-rw-rw-   0        0        0     2478 2023-04-18 19:30:22.000000 pyblp-1.0.0/docs/notebooks/api/integration.ipynb
--rw-rw-rw-   0        0        0     3467 2023-04-18 19:30:24.000000 pyblp-1.0.0/docs/notebooks/api/iteration.ipynb
--rw-rw-rw-   0        0        0     3106 2023-04-18 19:30:26.000000 pyblp-1.0.0/docs/notebooks/api/optimization.ipynb
--rw-rw-rw-   0        0        0     3926 2023-04-18 19:30:27.000000 pyblp-1.0.0/docs/notebooks/api/parallel.ipynb
-drwxrwxrwx   0        0        0        0 2023-04-19 16:31:37.000000 pyblp-1.0.0/docs/notebooks/tutorial/
-drwxrwxrwx   0        0        0        0 2023-04-19 16:31:37.000000 pyblp-1.0.0/docs/notebooks/tutorial/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0    29637 2023-04-18 19:34:47.000000 pyblp-1.0.0/docs/notebooks/tutorial/.ipynb_checkpoints/blp-checkpoint.ipynb
--rw-rw-rw-   0        0        0    34724 2023-04-18 19:31:05.000000 pyblp-1.0.0/docs/notebooks/tutorial/.ipynb_checkpoints/logit_nested-checkpoint.ipynb
--rw-rw-rw-   0        0        0    59665 2023-04-18 19:48:10.000000 pyblp-1.0.0/docs/notebooks/tutorial/.ipynb_checkpoints/nevo-checkpoint.ipynb
--rw-rw-rw-   0        0        0    59766 2023-04-18 20:05:52.000000 pyblp-1.0.0/docs/notebooks/tutorial/.ipynb_checkpoints/petrin-checkpoint.ipynb
--rw-rw-rw-   0        0        0   199510 2023-04-18 19:35:02.000000 pyblp-1.0.0/docs/notebooks/tutorial/.ipynb_checkpoints/post_estimation-checkpoint.ipynb
--rw-rw-rw-   0        0        0    14403 2023-04-18 19:32:11.000000 pyblp-1.0.0/docs/notebooks/tutorial/.ipynb_checkpoints/simulation-checkpoint.ipynb
--rw-rw-rw-   0        0        0    29637 2023-04-18 19:34:47.000000 pyblp-1.0.0/docs/notebooks/tutorial/blp.ipynb
--rw-rw-rw-   0        0        0    34724 2023-04-18 19:31:05.000000 pyblp-1.0.0/docs/notebooks/tutorial/logit_nested.ipynb
--rw-rw-rw-   0        0        0    59665 2023-04-18 19:48:10.000000 pyblp-1.0.0/docs/notebooks/tutorial/nevo.ipynb
--rw-rw-rw-   0        0        0    59766 2023-04-18 20:05:52.000000 pyblp-1.0.0/docs/notebooks/tutorial/petrin.ipynb
--rw-rw-rw-   0        0        0   199510 2023-04-18 19:35:02.000000 pyblp-1.0.0/docs/notebooks/tutorial/post_estimation.ipynb
--rw-rw-rw-   0        0        0    14403 2023-04-18 19:32:11.000000 pyblp-1.0.0/docs/notebooks/tutorial/simulation.ipynb
--rw-rw-rw-   0        0        0    11051 2023-04-18 19:21:19.000000 pyblp-1.0.0/docs/references.rst
-drwxrwxrwx   0        0        0        0 2023-04-19 16:31:37.000000 pyblp-1.0.0/docs/static/
--rw-rw-rw-   0        0        0     1343 2021-06-11 17:07:44.000000 pyblp-1.0.0/docs/static/override.css
--rw-rw-rw-   0        0        0      245 2021-06-11 17:07:44.000000 pyblp-1.0.0/docs/static/override.js
--rw-rw-rw-   0        0        0      299 2021-06-11 17:07:44.000000 pyblp-1.0.0/docs/static/preamble.tex
-drwxrwxrwx   0        0        0        0 2023-04-19 16:31:37.000000 pyblp-1.0.0/docs/templates/
--rw-rw-rw-   0        0        0      101 2021-06-11 17:07:44.000000 pyblp-1.0.0/docs/templates/breadcrumbs.html
--rw-rw-rw-   0        0        0      103 2021-06-11 17:07:44.000000 pyblp-1.0.0/docs/templates/class_without_methods.rst
--rw-rw-rw-   0        0        0      105 2021-06-11 17:07:44.000000 pyblp-1.0.0/docs/templates/class_without_methods_or_signature.rst
--rw-rw-rw-   0        0        0      378 2021-06-11 17:07:44.000000 pyblp-1.0.0/docs/templates/class_without_signature.rst
--rw-rw-rw-   0        0        0      373 2021-06-11 17:07:44.000000 pyblp-1.0.0/docs/templates/class_with_signature.rst
--rw-rw-rw-   0        0        0       38 2021-06-11 17:07:44.000000 pyblp-1.0.0/docs/templates/nbsphinx_epilog.rst
--rw-rw-rw-   0        0        0      484 2021-06-11 17:07:44.000000 pyblp-1.0.0/docs/templates/nbsphinx_prolog.rst
--rw-rw-rw-   0        0        0     3613 2023-04-19 16:19:47.000000 pyblp-1.0.0/docs/testing.rst
--rw-rw-rw-   0        0        0      549 2023-01-13 01:37:52.000000 pyblp-1.0.0/docs/tutorial.rst
--rw-rw-rw-   0        0        0     4489 2023-04-18 19:28:39.000000 pyblp-1.0.0/docs/versions.rst
--rw-rw-rw-   0        0        0     1084 2021-06-11 17:07:44.000000 pyblp-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      238 2021-06-11 17:07:44.000000 pyblp-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7769 2023-04-19 16:31:37.000000 pyblp-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-19 16:31:37.000000 pyblp-1.0.0/pyblp/
-drwxrwxrwx   0        0        0        0 2023-04-19 16:31:37.000000 pyblp-1.0.0/pyblp/configurations/
--rw-rw-rw-   0        0        0    28826 2023-03-21 22:25:06.000000 pyblp-1.0.0/pyblp/configurations/formulation.py
--rw-rw-rw-   0        0        0    46683 2021-11-13 19:48:09.000000 pyblp-1.0.0/pyblp/configurations/integration.py
--rw-rw-rw-   0        0        0    22392 2022-05-21 13:14:05.000000 pyblp-1.0.0/pyblp/configurations/iteration.py
--rw-rw-rw-   0        0        0    23921 2022-08-15 13:04:07.000000 pyblp-1.0.0/pyblp/configurations/optimization.py
--rw-rw-rw-   0        0        0       30 2021-06-11 17:07:44.000000 pyblp-1.0.0/pyblp/configurations/__init__.py
--rw-rw-rw-   0        0        0    25523 2023-04-10 22:11:10.000000 pyblp-1.0.0/pyblp/construction.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:31:37.000000 pyblp-1.0.0/pyblp/data/
--rw-rw-rw-   0        0        0   501476 2021-06-11 17:07:44.000000 pyblp-1.0.0/pyblp/data/blp_agents.csv
--rw-rw-rw-   0        0        0   765587 2021-06-11 17:07:44.000000 pyblp-1.0.0/pyblp/data/blp_products.csv
--rw-rw-rw-   0        0        0   327112 2021-06-11 17:07:44.000000 pyblp-1.0.0/pyblp/data/nevo_agents.csv
--rw-rw-rw-   0        0        0   642162 2021-06-11 17:07:44.000000 pyblp-1.0.0/pyblp/data/nevo_products.csv
--rw-rw-rw-   0        0        0  2203389 2022-07-26 21:45:21.000000 pyblp-1.0.0/pyblp/data/petrin_agents.csv
--rw-rw-rw-   0        0        0     2376 2022-05-16 13:19:23.000000 pyblp-1.0.0/pyblp/data/petrin_covariances.csv
--rw-rw-rw-   0        0        0  1078568 2022-07-26 21:40:51.000000 pyblp-1.0.0/pyblp/data/petrin_products.csv
--rw-rw-rw-   0        0        0      193 2022-07-26 22:03:23.000000 pyblp-1.0.0/pyblp/data/petrin_values.csv
--rw-rw-rw-   0        0        0     4000 2022-07-27 18:25:54.000000 pyblp-1.0.0/pyblp/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:31:37.000000 pyblp-1.0.0/pyblp/economies/
--rw-rw-rw-   0        0        0    18874 2023-02-24 21:29:19.000000 pyblp-1.0.0/pyblp/economies/economy.py
--rw-rw-rw-   0        0        0   112388 2023-02-24 21:22:13.000000 pyblp-1.0.0/pyblp/economies/problem.py
--rw-rw-rw-   0        0        0    53947 2023-02-24 21:22:29.000000 pyblp-1.0.0/pyblp/economies/simulation.py
--rw-rw-rw-   0        0        0       43 2021-06-11 17:07:44.000000 pyblp-1.0.0/pyblp/economies/__init__.py
--rw-rw-rw-   0        0        0    12954 2022-12-16 21:01:23.000000 pyblp-1.0.0/pyblp/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:31:37.000000 pyblp-1.0.0/pyblp/markets/
--rw-rw-rw-   0        0        0    27785 2023-04-10 22:16:27.000000 pyblp-1.0.0/pyblp/markets/economy_results_market.py
--rw-rw-rw-   0        0        0    98930 2023-04-10 22:16:00.000000 pyblp-1.0.0/pyblp/markets/market.py
--rw-rw-rw-   0        0        0    12282 2022-12-16 21:01:23.000000 pyblp-1.0.0/pyblp/markets/problem_market.py
--rw-rw-rw-   0        0        0     6334 2022-12-13 19:38:21.000000 pyblp-1.0.0/pyblp/markets/simulation_market.py
--rw-rw-rw-   0        0        0       52 2021-06-11 17:07:44.000000 pyblp-1.0.0/pyblp/markets/__init__.py
--rw-rw-rw-   0        0        0    23057 2023-04-18 19:23:42.000000 pyblp-1.0.0/pyblp/micro.py
--rw-rw-rw-   0        0        0     9356 2023-03-10 23:34:55.000000 pyblp-1.0.0/pyblp/options.py
--rw-rw-rw-   0        0        0    29455 2022-12-13 19:38:21.000000 pyblp-1.0.0/pyblp/parameters.py
--rw-rw-rw-   0        0        0    28301 2023-03-21 22:21:26.000000 pyblp-1.0.0/pyblp/primitives.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:31:37.000000 pyblp-1.0.0/pyblp/results/
--rw-rw-rw-   0        0        0    16753 2022-06-18 19:40:25.000000 pyblp-1.0.0/pyblp/results/bootstrapped_results.py
--rw-rw-rw-   0        0        0    90409 2023-02-24 21:32:29.000000 pyblp-1.0.0/pyblp/results/economy_results.py
--rw-rw-rw-   0        0        0     6637 2023-04-10 22:26:20.000000 pyblp-1.0.0/pyblp/results/importance_sampling_results.py
--rw-rw-rw-   0        0        0    22114 2022-12-13 19:38:21.000000 pyblp-1.0.0/pyblp/results/optimal_instrument_results.py
--rw-rw-rw-   0        0        0    79894 2023-04-10 22:21:46.000000 pyblp-1.0.0/pyblp/results/problem_results.py
--rw-rw-rw-   0        0        0    19108 2022-06-19 20:46:43.000000 pyblp-1.0.0/pyblp/results/simulation_results.py
--rw-rw-rw-   0        0        0       35 2021-06-11 17:07:44.000000 pyblp-1.0.0/pyblp/results/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:31:37.000000 pyblp-1.0.0/pyblp/utilities/
--rw-rw-rw-   0        0        0     8071 2022-05-20 13:22:47.000000 pyblp-1.0.0/pyblp/utilities/algebra.py
--rw-rw-rw-   0        0        0    24837 2023-04-11 17:10:01.000000 pyblp-1.0.0/pyblp/utilities/basics.py
--rw-rw-rw-   0        0        0     6021 2021-06-11 17:07:44.000000 pyblp-1.0.0/pyblp/utilities/statistics.py
--rw-rw-rw-   0        0        0       30 2021-06-11 17:07:44.000000 pyblp-1.0.0/pyblp/utilities/__init__.py
--rw-rw-rw-   0        0        0       57 2023-04-18 19:23:55.000000 pyblp-1.0.0/pyblp/version.py
--rw-rw-rw-   0        0        0     1738 2022-08-01 20:05:54.000000 pyblp-1.0.0/pyblp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:31:37.000000 pyblp-1.0.0/pyblp.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-19 16:31:37.000000 pyblp-1.0.0/pyblp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     7769 2023-04-19 16:31:37.000000 pyblp-1.0.0/pyblp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-04-19 16:31:37.000000 pyblp-1.0.0/pyblp.egg-info/requires.txt
--rw-rw-rw-   0        0        0     4361 2023-04-19 16:31:37.000000 pyblp-1.0.0/pyblp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       12 2023-04-19 16:31:37.000000 pyblp-1.0.0/pyblp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7490 2023-04-19 16:15:23.000000 pyblp-1.0.0/README.rst
--rw-rw-rw-   0        0        0       72 2021-06-11 17:07:44.000000 pyblp-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0      283 2023-04-19 16:31:37.000000 pyblp-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1976 2022-06-07 14:45:18.000000 pyblp-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:31:37.000000 pyblp-1.0.0/tests/
--rw-rw-rw-   0        0        0    32845 2023-04-18 20:38:33.000000 pyblp-1.0.0/tests/conftest.py
--rw-rw-rw-   0        0        0    90359 2023-04-18 20:35:25.000000 pyblp-1.0.0/tests/test_blp.py
--rw-rw-rw-   0        0        0     9323 2021-11-10 16:56:28.000000 pyblp-1.0.0/tests/test_formulation.py
--rw-rw-rw-   0        0        0     5544 2021-06-11 17:07:44.000000 pyblp-1.0.0/tests/test_integration.py
--rw-rw-rw-   0        0        0     5420 2022-05-21 13:16:47.000000 pyblp-1.0.0/tests/test_iteration.py
--rw-rw-rw-   0        0        0     4154 2022-08-15 13:04:30.000000 pyblp-1.0.0/tests/test_optimization.py
--rw-rw-rw-   0        0        0       22 2021-06-11 17:07:44.000000 pyblp-1.0.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:26:35.000000 pyblp-1.1.0/
+-rw-rw-rw-   0        0        0      710 2021-06-11 17:07:44.000000 pyblp-1.1.0/.gitignore
+drwxrwxrwx   0        0        0        0 2023-07-14 20:26:34.000000 pyblp-1.1.0/docs/
+-rw-rw-rw-   0        0        0    11617 2022-08-01 20:06:35.000000 pyblp-1.1.0/docs/api.rst
+-rw-rw-rw-   0        0        0    27047 2023-07-06 15:42:48.000000 pyblp-1.1.0/docs/background.rst
+-rw-rw-rw-   0        0        0     7190 2023-07-14 20:23:31.000000 pyblp-1.1.0/docs/conf.py
+-rw-rw-rw-   0        0        0      347 2023-01-25 21:32:43.000000 pyblp-1.1.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0      670 2021-06-11 17:07:44.000000 pyblp-1.1.0/docs/index.rst
+-rw-rw-rw-   0        0        0       87 2023-04-18 19:16:57.000000 pyblp-1.1.0/docs/introduction.rst
+-rw-rw-rw-   0        0        0       45 2021-06-11 17:07:44.000000 pyblp-1.1.0/docs/legal.rst
+-rw-rw-rw-   0        0        0    13032 2023-07-12 20:00:24.000000 pyblp-1.1.0/docs/notation.rst
+drwxrwxrwx   0        0        0        0 2023-07-14 20:26:34.000000 pyblp-1.1.0/docs/notebooks/
+drwxrwxrwx   0        0        0        0 2023-07-14 20:26:34.000000 pyblp-1.1.0/docs/notebooks/api/
+drwxrwxrwx   0        0        0        0 2023-07-14 20:26:34.000000 pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0    31385 2023-07-14 16:29:01.000000 pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/build_blp_instruments-checkpoint.ipynb
+-rw-rw-rw-   0        0        0    29293 2023-07-14 16:29:02.000000 pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/build_differentiation_instruments-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     1891 2023-07-14 16:29:03.000000 pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/build_id_data-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     3232 2023-07-14 16:29:04.000000 pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/build_integration-checkpoint.ipynb
+-rw-rw-rw-   0        0        0    12117 2023-07-14 16:29:07.000000 pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/build_matrix-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     5439 2023-07-14 16:29:11.000000 pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/build_ownership-checkpoint.ipynb
+-rw-rw-rw-   0        0        0    14521 2023-07-14 16:29:13.000000 pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/data-checkpoint.ipynb
+-rw-rw-rw-   0        0        0    20562 2023-07-14 16:29:14.000000 pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/data_to_dict-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     3514 2023-07-14 16:29:17.000000 pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/formulation-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     2478 2023-07-14 16:29:18.000000 pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/integration-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     3467 2023-07-14 16:29:19.000000 pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/iteration-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     4060 2023-01-12 23:16:23.000000 pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/micro_dataset-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     3405 2023-01-12 23:16:20.000000 pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/micro_part-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     3106 2023-07-14 16:29:20.000000 pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/optimization-checkpoint.ipynb
+-rw-rw-rw-   0        0        0     3926 2023-07-14 16:29:23.000000 pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/parallel-checkpoint.ipynb
+-rw-rw-rw-   0        0        0    31385 2023-07-14 16:29:01.000000 pyblp-1.1.0/docs/notebooks/api/build_blp_instruments.ipynb
+-rw-rw-rw-   0        0        0    29293 2023-07-14 16:29:02.000000 pyblp-1.1.0/docs/notebooks/api/build_differentiation_instruments.ipynb
+-rw-rw-rw-   0        0        0     1891 2023-07-14 16:29:03.000000 pyblp-1.1.0/docs/notebooks/api/build_id_data.ipynb
+-rw-rw-rw-   0        0        0     3232 2023-07-14 16:29:04.000000 pyblp-1.1.0/docs/notebooks/api/build_integration.ipynb
+-rw-rw-rw-   0        0        0    12117 2023-07-14 16:29:07.000000 pyblp-1.1.0/docs/notebooks/api/build_matrix.ipynb
+-rw-rw-rw-   0        0        0     5439 2023-07-14 16:29:11.000000 pyblp-1.1.0/docs/notebooks/api/build_ownership.ipynb
+-rw-rw-rw-   0        0        0    14521 2023-07-14 16:29:13.000000 pyblp-1.1.0/docs/notebooks/api/data.ipynb
+-rw-rw-rw-   0        0        0    20562 2023-07-14 16:29:14.000000 pyblp-1.1.0/docs/notebooks/api/data_to_dict.ipynb
+-rw-rw-rw-   0        0        0     3514 2023-07-14 16:29:17.000000 pyblp-1.1.0/docs/notebooks/api/formulation.ipynb
+-rw-rw-rw-   0        0        0     2478 2023-07-14 16:29:18.000000 pyblp-1.1.0/docs/notebooks/api/integration.ipynb
+-rw-rw-rw-   0        0        0     3467 2023-07-14 16:29:19.000000 pyblp-1.1.0/docs/notebooks/api/iteration.ipynb
+-rw-rw-rw-   0        0        0     3106 2023-07-14 16:29:20.000000 pyblp-1.1.0/docs/notebooks/api/optimization.ipynb
+-rw-rw-rw-   0        0        0     3926 2023-07-14 16:29:23.000000 pyblp-1.1.0/docs/notebooks/api/parallel.ipynb
+drwxrwxrwx   0        0        0        0 2023-07-14 20:26:34.000000 pyblp-1.1.0/docs/notebooks/tutorial/
+drwxrwxrwx   0        0        0        0 2023-07-14 20:26:34.000000 pyblp-1.1.0/docs/notebooks/tutorial/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0    29637 2023-07-14 16:42:15.000000 pyblp-1.1.0/docs/notebooks/tutorial/.ipynb_checkpoints/blp-checkpoint.ipynb
+-rw-rw-rw-   0        0        0    34724 2023-07-14 16:30:01.000000 pyblp-1.1.0/docs/notebooks/tutorial/.ipynb_checkpoints/logit_nested-checkpoint.ipynb
+-rw-rw-rw-   0        0        0    59665 2023-07-14 16:42:18.000000 pyblp-1.1.0/docs/notebooks/tutorial/.ipynb_checkpoints/nevo-checkpoint.ipynb
+-rw-rw-rw-   0        0        0    59760 2023-07-14 17:11:04.000000 pyblp-1.1.0/docs/notebooks/tutorial/.ipynb_checkpoints/petrin-checkpoint.ipynb
+-rw-rw-rw-   0        0        0   199510 2023-07-14 16:37:42.000000 pyblp-1.1.0/docs/notebooks/tutorial/.ipynb_checkpoints/post_estimation-checkpoint.ipynb
+-rw-rw-rw-   0        0        0    14403 2023-07-14 16:30:15.000000 pyblp-1.1.0/docs/notebooks/tutorial/.ipynb_checkpoints/simulation-checkpoint.ipynb
+-rw-rw-rw-   0        0        0    29637 2023-07-14 16:42:15.000000 pyblp-1.1.0/docs/notebooks/tutorial/blp.ipynb
+-rw-rw-rw-   0        0        0    34724 2023-07-14 16:30:01.000000 pyblp-1.1.0/docs/notebooks/tutorial/logit_nested.ipynb
+-rw-rw-rw-   0        0        0    59665 2023-07-14 16:42:18.000000 pyblp-1.1.0/docs/notebooks/tutorial/nevo.ipynb
+-rw-rw-rw-   0        0        0    59760 2023-07-14 17:11:04.000000 pyblp-1.1.0/docs/notebooks/tutorial/petrin.ipynb
+-rw-rw-rw-   0        0        0   199510 2023-07-14 16:37:42.000000 pyblp-1.1.0/docs/notebooks/tutorial/post_estimation.ipynb
+-rw-rw-rw-   0        0        0    14403 2023-07-14 16:30:15.000000 pyblp-1.1.0/docs/notebooks/tutorial/simulation.ipynb
+-rw-rw-rw-   0        0        0    11320 2023-05-22 14:48:50.000000 pyblp-1.1.0/docs/references.rst
+drwxrwxrwx   0        0        0        0 2023-07-14 20:26:34.000000 pyblp-1.1.0/docs/static/
+-rw-rw-rw-   0        0        0     1343 2021-06-11 17:07:44.000000 pyblp-1.1.0/docs/static/override.css
+-rw-rw-rw-   0        0        0      245 2021-06-11 17:07:44.000000 pyblp-1.1.0/docs/static/override.js
+-rw-rw-rw-   0        0        0      299 2021-06-11 17:07:44.000000 pyblp-1.1.0/docs/static/preamble.tex
+drwxrwxrwx   0        0        0        0 2023-07-14 20:26:34.000000 pyblp-1.1.0/docs/templates/
+-rw-rw-rw-   0        0        0      101 2021-06-11 17:07:44.000000 pyblp-1.1.0/docs/templates/breadcrumbs.html
+-rw-rw-rw-   0        0        0      103 2021-06-11 17:07:44.000000 pyblp-1.1.0/docs/templates/class_without_methods.rst
+-rw-rw-rw-   0        0        0      105 2021-06-11 17:07:44.000000 pyblp-1.1.0/docs/templates/class_without_methods_or_signature.rst
+-rw-rw-rw-   0        0        0      378 2021-06-11 17:07:44.000000 pyblp-1.1.0/docs/templates/class_without_signature.rst
+-rw-rw-rw-   0        0        0      373 2021-06-11 17:07:44.000000 pyblp-1.1.0/docs/templates/class_with_signature.rst
+-rw-rw-rw-   0        0        0       38 2021-06-11 17:07:44.000000 pyblp-1.1.0/docs/templates/nbsphinx_epilog.rst
+-rw-rw-rw-   0        0        0      484 2021-06-11 17:07:44.000000 pyblp-1.1.0/docs/templates/nbsphinx_prolog.rst
+-rw-rw-rw-   0        0        0     3613 2023-04-19 16:19:47.000000 pyblp-1.1.0/docs/testing.rst
+-rw-rw-rw-   0        0        0      549 2023-01-13 01:37:52.000000 pyblp-1.1.0/docs/tutorial.rst
+-rw-rw-rw-   0        0        0     4575 2023-07-14 16:27:15.000000 pyblp-1.1.0/docs/versions.rst
+-rw-rw-rw-   0        0        0     1084 2021-06-11 17:07:44.000000 pyblp-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      238 2021-06-11 17:07:44.000000 pyblp-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7838 2023-07-14 20:26:35.000000 pyblp-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 20:26:34.000000 pyblp-1.1.0/pyblp/
+drwxrwxrwx   0        0        0        0 2023-07-14 20:26:34.000000 pyblp-1.1.0/pyblp/configurations/
+-rw-rw-rw-   0        0        0    28826 2023-03-21 22:25:06.000000 pyblp-1.1.0/pyblp/configurations/formulation.py
+-rw-rw-rw-   0        0        0    46683 2021-11-13 19:48:09.000000 pyblp-1.1.0/pyblp/configurations/integration.py
+-rw-rw-rw-   0        0        0    22392 2022-05-21 13:14:05.000000 pyblp-1.1.0/pyblp/configurations/iteration.py
+-rw-rw-rw-   0        0        0    23921 2022-08-15 13:04:07.000000 pyblp-1.1.0/pyblp/configurations/optimization.py
+-rw-rw-rw-   0        0        0       30 2021-06-11 17:07:44.000000 pyblp-1.1.0/pyblp/configurations/__init__.py
+-rw-rw-rw-   0        0        0    25523 2023-04-10 22:11:10.000000 pyblp-1.1.0/pyblp/construction.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:26:34.000000 pyblp-1.1.0/pyblp/data/
+-rw-rw-rw-   0        0        0   501476 2021-06-11 17:07:44.000000 pyblp-1.1.0/pyblp/data/blp_agents.csv
+-rw-rw-rw-   0        0        0   765587 2021-06-11 17:07:44.000000 pyblp-1.1.0/pyblp/data/blp_products.csv
+-rw-rw-rw-   0        0        0   327112 2021-06-11 17:07:44.000000 pyblp-1.1.0/pyblp/data/nevo_agents.csv
+-rw-rw-rw-   0        0        0   642162 2021-06-11 17:07:44.000000 pyblp-1.1.0/pyblp/data/nevo_products.csv
+-rw-rw-rw-   0        0        0  2203389 2022-07-26 21:45:21.000000 pyblp-1.1.0/pyblp/data/petrin_agents.csv
+-rw-rw-rw-   0        0        0     2376 2022-05-16 13:19:23.000000 pyblp-1.1.0/pyblp/data/petrin_covariances.csv
+-rw-rw-rw-   0        0        0  1078568 2022-07-26 21:40:51.000000 pyblp-1.1.0/pyblp/data/petrin_products.csv
+-rw-rw-rw-   0        0        0      193 2022-07-26 22:03:23.000000 pyblp-1.1.0/pyblp/data/petrin_values.csv
+-rw-rw-rw-   0        0        0     4000 2022-07-27 18:25:54.000000 pyblp-1.1.0/pyblp/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:26:34.000000 pyblp-1.1.0/pyblp/economies/
+-rw-rw-rw-   0        0        0    19014 2023-05-22 14:59:19.000000 pyblp-1.1.0/pyblp/economies/economy.py
+-rw-rw-rw-   0        0        0   118288 2023-07-14 16:23:43.000000 pyblp-1.1.0/pyblp/economies/problem.py
+-rw-rw-rw-   0        0        0    55629 2023-06-27 20:19:24.000000 pyblp-1.1.0/pyblp/economies/simulation.py
+-rw-rw-rw-   0        0        0       43 2021-06-11 17:07:44.000000 pyblp-1.1.0/pyblp/economies/__init__.py
+-rw-rw-rw-   0        0        0    12954 2022-12-16 21:01:23.000000 pyblp-1.1.0/pyblp/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:26:35.000000 pyblp-1.1.0/pyblp/markets/
+-rw-rw-rw-   0        0        0    27960 2023-06-27 20:17:51.000000 pyblp-1.1.0/pyblp/markets/economy_results_market.py
+-rw-rw-rw-   0        0        0   100283 2023-07-06 15:34:27.000000 pyblp-1.1.0/pyblp/markets/market.py
+-rw-rw-rw-   0        0        0    12282 2023-06-15 22:01:39.000000 pyblp-1.1.0/pyblp/markets/problem_market.py
+-rw-rw-rw-   0        0        0     6334 2022-12-13 19:38:21.000000 pyblp-1.1.0/pyblp/markets/simulation_market.py
+-rw-rw-rw-   0        0        0       52 2021-06-11 17:07:44.000000 pyblp-1.1.0/pyblp/markets/__init__.py
+-rw-rw-rw-   0        0        0    23485 2023-06-26 16:05:12.000000 pyblp-1.1.0/pyblp/micro.py
+-rw-rw-rw-   0        0        0     9356 2023-03-10 23:34:55.000000 pyblp-1.1.0/pyblp/options.py
+-rw-rw-rw-   0        0        0    29455 2022-12-13 19:38:21.000000 pyblp-1.1.0/pyblp/parameters.py
+-rw-rw-rw-   0        0        0    30238 2023-06-27 20:14:43.000000 pyblp-1.1.0/pyblp/primitives.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:26:35.000000 pyblp-1.1.0/pyblp/results/
+-rw-rw-rw-   0        0        0    16753 2022-06-18 19:40:25.000000 pyblp-1.1.0/pyblp/results/bootstrapped_results.py
+-rw-rw-rw-   0        0        0    90543 2023-06-27 18:23:21.000000 pyblp-1.1.0/pyblp/results/economy_results.py
+-rw-rw-rw-   0        0        0     6637 2023-04-10 22:26:20.000000 pyblp-1.1.0/pyblp/results/importance_sampling_results.py
+-rw-rw-rw-   0        0        0    22114 2022-12-13 19:38:21.000000 pyblp-1.1.0/pyblp/results/optimal_instrument_results.py
+-rw-rw-rw-   0        0        0    81099 2023-05-31 16:30:21.000000 pyblp-1.1.0/pyblp/results/problem_results.py
+-rw-rw-rw-   0        0        0    19108 2022-06-19 20:46:43.000000 pyblp-1.1.0/pyblp/results/simulation_results.py
+-rw-rw-rw-   0        0        0       35 2021-06-11 17:07:44.000000 pyblp-1.1.0/pyblp/results/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:26:35.000000 pyblp-1.1.0/pyblp/utilities/
+-rw-rw-rw-   0        0        0     8071 2022-05-20 13:22:47.000000 pyblp-1.1.0/pyblp/utilities/algebra.py
+-rw-rw-rw-   0        0        0    26343 2023-06-16 18:52:40.000000 pyblp-1.1.0/pyblp/utilities/basics.py
+-rw-rw-rw-   0        0        0     6073 2023-05-31 16:37:27.000000 pyblp-1.1.0/pyblp/utilities/statistics.py
+-rw-rw-rw-   0        0        0       30 2021-06-11 17:07:44.000000 pyblp-1.1.0/pyblp/utilities/__init__.py
+-rw-rw-rw-   0        0        0       57 2023-07-14 16:27:02.000000 pyblp-1.1.0/pyblp/version.py
+-rw-rw-rw-   0        0        0     1738 2022-08-01 20:05:54.000000 pyblp-1.1.0/pyblp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:26:34.000000 pyblp-1.1.0/pyblp.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-14 20:26:34.000000 pyblp-1.1.0/pyblp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     7838 2023-07-14 20:26:34.000000 pyblp-1.1.0/pyblp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-07-14 20:26:34.000000 pyblp-1.1.0/pyblp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     4396 2023-07-14 20:26:34.000000 pyblp-1.1.0/pyblp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2023-07-14 20:26:34.000000 pyblp-1.1.0/pyblp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7559 2023-06-27 20:23:40.000000 pyblp-1.1.0/README.rst
+-rw-rw-rw-   0        0        0      158 2021-06-11 17:07:44.000000 pyblp-1.1.0/readthedocs.yml
+-rw-rw-rw-   0        0        0       72 2021-06-11 17:07:44.000000 pyblp-1.1.0/requirements.txt
+-rw-rw-rw-   0        0        0      283 2023-07-14 20:26:35.000000 pyblp-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1976 2022-06-07 14:45:18.000000 pyblp-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:26:35.000000 pyblp-1.1.0/tests/
+-rw-rw-rw-   0        0        0    34701 2023-07-06 15:34:57.000000 pyblp-1.1.0/tests/conftest.py
+-rw-rw-rw-   0        0        0    94076 2023-07-06 15:37:41.000000 pyblp-1.1.0/tests/test_blp.py
+-rw-rw-rw-   0        0        0     9323 2021-11-10 16:56:28.000000 pyblp-1.1.0/tests/test_formulation.py
+-rw-rw-rw-   0        0        0     5544 2021-06-11 17:07:44.000000 pyblp-1.1.0/tests/test_integration.py
+-rw-rw-rw-   0        0        0     5420 2022-05-21 13:16:47.000000 pyblp-1.1.0/tests/test_iteration.py
+-rw-rw-rw-   0        0        0     4154 2022-08-15 13:04:30.000000 pyblp-1.1.0/tests/test_optimization.py
+-rw-rw-rw-   0        0        0       22 2021-06-11 17:07:44.000000 pyblp-1.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     3742 2022-06-07 15:05:03.000000 pyblp-1.1.0/tox.ini
```

### Comparing `pyblp-1.0.0/docs/api.rst` & `pyblp-1.1.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/docs/background.rst` & `pyblp-1.1.0/docs/background.rst`

 * *Files 0% similar despite different names*

```diff
@@ -60,17 +60,17 @@
 .. math:: \pi_{ft} = \sum_{j \in J_{ft}} (p_{jt} - c_{jt})s_{jt}.
 
 In a single market, the corresponding multi-product differentiated Bertrand first order conditions are, in vector-matrix form,
 
 .. math:: p - c = \underbrace{\Delta^{-1}s}_{\eta},
    :label: eta
 
-where the multi-product Bertrand markup :math:`\eta` depends on :math:`\Delta`, a :math:`J_t \times J_t` matrix of intra-firm (negative) demand derivatives:
+where the multi-product Bertrand markup :math:`\eta` depends on :math:`\Delta`, a :math:`J_t \times J_t` matrix of intra-firm (negative, transposed) demand derivatives:
 
-.. math:: \Delta = -\mathscr{H} \odot \frac{\partial s}{\partial p}.
+.. math:: \Delta = -\mathscr{H} \odot \frac{\partial s}{\partial p}'.
 
 Here, :math:`\mathscr{H}` denotes the market-level ownership or product holdings matrix in the market, where :math:`\mathscr{H}_{jk}` is typically :math:`1` if the same firm produces products :math:`j` and :math:`k`, and :math:`0` otherwise.
 
 To include a supply side, we must specify a functional form for marginal costs:
 
 .. math:: \tilde{c} = f(c) = X_3\gamma + \omega.
    :label: costs
```

### Comparing `pyblp-1.0.0/docs/conf.py` & `pyblp-1.1.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 autosummary_generate = True
 numpydoc_show_class_members = False
 autosectionlabel_prefix_document = True
 nbsphinx_prolog = read('templates/nbsphinx_prolog.rst')
 nbsphinx_epilog = read('templates/nbsphinx_epilog.rst')
 linkcheck_ignore = [
     'https://www.anaconda.com/download',  # 403 forbidden, but fine in browser
+    'https://www.tandfonline.com/doi/abs/10.1080/01621459.1963.10480682',  # 403 forbidden, but fine in browser
 ]
 
 # configure HTML information
 html_theme = 'sphinx_rtd_theme'
 
 # configure LaTeX information
 latex_elements = {
```

### Comparing `pyblp-1.0.0/docs/index.rst` & `pyblp-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/docs/notation.rst` & `pyblp-1.1.0/docs/notation.rst`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 :math:`K_2`            Demand-side nonlinear product characteristics
 :math:`K_3`            Supply-side product characteristics
 :math:`K_3^\text{ex}`  Exogenous supply-side product characteristics
 :math:`K_3^\text{en}`  Endogenous supply-side product characteristics
 :math:`D`              Demographic variables
 :math:`M_D`            Demand-side instruments
 :math:`M_S`            Supply-side instruments
+:math:`M_C`            Covariance instruments
 :math:`M_M`            Micro moments
 :math:`T_m`            Markets over which micro moment :math:`m` is averaged
 :math:`T_{mn}`         Markets over which micro moments :math:`m` and :math:`n` are both averaged
 :math:`N_m`            Observations underlying observed micro moment value :math:`m`.
 :math:`M`              All moments
 :math:`E_D`            Absorbed dimensions of demand-side fixed effects
 :math:`E_S`            Absorbed dimensions of supply-side fixed effects
@@ -57,78 +58,82 @@
 :math:`J_{ct}`         Products in cluster :math:`c` and market :math:`t`
 =====================  ==========================================================================
 
 
 Matrices, Vectors, and Scalars
 ------------------------------
 
-=====================================================  ==============================  ====================================================================================
-Symbol                                                 Dimensions                      Description
-=====================================================  ==============================  ====================================================================================
-:math:`X_1`                                            :math:`N \times K_1`            Demand-side linear product characteristics
-:math:`X_1^\text{ex}`                                  :math:`N \times K_1^\text{ex}`  Exogenous demand-side linear product characteristics
-:math:`X_1^\text{en}`                                  :math:`N \times K_1^\text{en}`  Endogenous demand-side linear product characteristics
-:math:`X_2`                                            :math:`N \times K_2`            Demand-side Nonlinear product characteristics
-:math:`X_3`                                            :math:`N \times K_3`            Supply-side product characteristics
-:math:`X_3^\text{ex}`                                  :math:`N \times K_3^\text{ex}`  Exogenous supply-side product characteristics
-:math:`X_3^\text{en}`                                  :math:`N \times K_3^\text{en}`  Endogenous supply-side product characteristics
-:math:`\xi`                                            :math:`N \times 1`              Unobserved demand-side product characteristics
-:math:`\omega`                                         :math:`N \times 1`              Unobserved supply-side product characteristics
-:math:`p`                                              :math:`N \times 1`              Prices
-:math:`s` (:math:`s_{jt}`)                             :math:`N \times 1`              Market shares
-:math:`s` (:math:`s_{ht}`)                             :math:`H \times 1`              Group shares in a market :math:`t`
-:math:`s` (:math:`s_{ijt}`)                            :math:`N \times I_t`            Choice probabilities in a market :math:`t`
-:math:`c`                                              :math:`N \times 1`              Marginal costs
-:math:`\tilde{c}`                                      :math:`N \times 1`              Linear or log-linear marginal costs, :math:`c` or :math:`\log c` 
-:math:`\eta`                                           :math:`N \times 1`              Markup term from the BLP-markup equation
-:math:`\zeta`                                          :math:`N \times 1`              Markup term from the :math:`\zeta`-markup equation
-:math:`\mathscr{H}`                                    :math:`J_t \times J_t`          Ownership or product holdings matrix in market :math:`t`
-:math:`\kappa`                                         :math:`F_t \times F_t`          Cooperation matrix in market :math:`t`
-:math:`\Delta`                                         :math:`J_t \times J_t`          Intra-firm matrix of (negative) demand derivatives in market :math:`t`
-:math:`\Lambda`                                        :math:`J_t \times J_t`          Diagonal matrix used to decompose :math:`\eta` and :math:`\zeta` in market :math:`t`
-:math:`\Gamma`                                         :math:`J_t \times J_t`          Another matrix used to decompose :math:`\eta` and :math:`\zeta` in market :math:`t`
-:math:`d`                                              :math:`I_t \times D`            Observed agent characteristics called demographics in market :math:`t`
-:math:`\nu`                                            :math:`I_t \times K_2`          Unobserved agent characteristics called integration nodes in market :math:`t`
-:math:`w`                                              :math:`I_t \times 1`            Integration weights in market :math:`t`
-:math:`\delta`                                         :math:`N \times 1`              Mean utility
-:math:`\mu`                                            :math:`J_t \times I_t`          Agent-specific portion of utility in market :math:`t`
-:math:`\epsilon`                                       :math:`N \times 1`              Type I Extreme Value idiosyncratic preferences
-:math:`\bar{\epsilon}` (:math:`\bar{\epsilon}_{ijt}`)  :math:`N \times 1`              Type I Extreme Value term used to decompose :math:`\epsilon`
-:math:`\bar{\epsilon}` (:math:`\bar{\epsilon}_{iht}`)  :math:`N \times 1`              Group-specific term used to decompose :math:`\epsilon`
-:math:`U`                                              :math:`J_t \times I_t`          Indirect utilities
-:math:`V` (:math:`V_{ijt}`)                            :math:`J_t \times I_t`          Indirect utilities minus :math:`\epsilon`
-:math:`V` (:math:`V_{iht}`)                            :math:`J_t \times I_t`          Inclusive value of a nesting group
-:math:`\pi` (:math:`\pi_{jt}`)                         :math:`N \times 1`              Population-normalized gross expected profits
-:math:`\pi` (:math:`\pi_{ft}`)                         :math:`F_t \times 1`            Population-normalized gross expected profits of a firm in market :math:`t`
-:math:`\beta`                                          :math:`K_1 \times 1`            Demand-side linear parameters
-:math:`\beta^\text{ex}`                                :math:`K_1^\text{ex} \times 1`  Parameters in :math:`\beta` on exogenous product characteristics
-:math:`\alpha`                                         :math:`K_1^\text{en} \times 1`  Parameters in :math:`\beta` on endogenous product characteristics
-:math:`\Sigma`                                         :math:`K_2 \times K_2`          Cholesky root of the covariance matrix for unobserved taste heterogeneity
-:math:`\Pi`                                            :math:`K_2 \times D`            Parameters that measures how agent tastes vary with demographics
-:math:`\rho`                                           :math:`H \times 1`              Parameters that measures within nesting group correlation
-:math:`\gamma`                                         :math:`K_3 \times 1`            Supply-side linear parameters
-:math:`\gamma^\text{ex}`                               :math:`K_3^\text{ex} \times 1`  Parameters in :math:`\gamma` on exogenous product characteristics
-:math:`\gamma^\text{en}`                               :math:`K_3^\text{en} \times 1`  Parameters in :math:`\gamma` on endogenous product characteristics
-:math:`\theta`                                         :math:`P \times 1`              Parameters
-:math:`Z_D`                                            :math:`N \times M_D`            Demand-side instruments
-:math:`Z_S`                                            :math:`N \times M_S`            Supply-side instruments
-:math:`W`                                              :math:`M \times M`              Weighting matrix
-:math:`S`                                              :math:`M \times M`              Moment covariances
-:math:`q`                                              :math:`1 \times 1`              Objective value
-:math:`g_D`                                            :math:`N \times M_D`            Demand-side moments
-:math:`g_S`                                            :math:`N \times M_S`            Supply-side moments
-:math:`g_M`                                            :math:`I \times M_M`            Micro moments
-:math:`g` (:math:`g_{jt}`)                             :math:`N \times (M_D + M_S)`    Demand- and supply-side moments
-:math:`g` (:math:`g_c`)                                :math:`C \times (M_D + M_S)`    Clustered demand- and supply-side moments
-:math:`\bar{g}_D`                                      :math:`M_D \times 1`            Averaged demand-side moments
-:math:`\bar{g}_S`                                      :math:`M_S \times 1`            Averaged supply-side moments
-:math:`\bar{g}_M`                                      :math:`M_M \times 1`            Averaged micro moments
-:math:`\bar{g}`                                        :math:`M \times 1`              Averaged moments
-:math:`\bar{G}`                                        :math:`M \times P`              Jacobian of the averaged moments with respect to :math:`\theta`
-:math:`\varepsilon`                                    :math:`J_t \times J_t`          Elasticities of demand in market :math:`t`
-:math:`\mathscr{D}`                                    :math:`J_t \times J_t`          Diversion ratios in market :math:`t`
-:math:`\bar{\mathscr{D}}`                              :math:`J_t \times J_t`          Long-run diversion ratios in market :math:`t`
-:math:`\mathscr{M}`                                    :math:`N \times 1`              Markups
-:math:`\mathscr{E}`                                    :math:`1 \times 1`              Aggregate elasticity of demand of a market
-:math:`\text{CS}`                                      :math:`1 \times 1`              Population-normalized consumer surplus of a market
-:math:`\text{HHI}`                                     :math:`1 \times 1`              Herfindahl-Hirschman Index of a market
-=====================================================  ==============================  ====================================================================================
+=====================================================  ==================================  ====================================================================================
+Symbol                                                 Dimensions                          Description
+=====================================================  ==================================  ====================================================================================
+:math:`X_1`                                            :math:`N \times K_1`                Demand-side linear product characteristics
+:math:`X_1^\text{ex}`                                  :math:`N \times K_1^\text{ex}`      Exogenous demand-side linear product characteristics
+:math:`X_1^\text{en}`                                  :math:`N \times K_1^\text{en}`      Endogenous demand-side linear product characteristics
+:math:`X_2`                                            :math:`N \times K_2`                Demand-side Nonlinear product characteristics
+:math:`X_3`                                            :math:`N \times K_3`                Supply-side product characteristics
+:math:`X_3^\text{ex}`                                  :math:`N \times K_3^\text{ex}`      Exogenous supply-side product characteristics
+:math:`X_3^\text{en}`                                  :math:`N \times K_3^\text{en}`      Endogenous supply-side product characteristics
+:math:`\xi`                                            :math:`N \times 1`                  Unobserved demand-side product characteristics
+:math:`\omega`                                         :math:`N \times 1`                  Unobserved supply-side product characteristics
+:math:`p`                                              :math:`N \times 1`                  Prices
+:math:`s` (:math:`s_{jt}`)                             :math:`N \times 1`                  Market shares
+:math:`s` (:math:`s_{ht}`)                             :math:`H \times 1`                  Group shares in a market :math:`t`
+:math:`s` (:math:`s_{ijt}`)                            :math:`N \times I_t`                Choice probabilities in a market :math:`t`
+:math:`c`                                              :math:`N \times 1`                  Marginal costs
+:math:`\tilde{c}`                                      :math:`N \times 1`                  Linear or log-linear marginal costs, :math:`c` or :math:`\log c`
+:math:`\eta`                                           :math:`N \times 1`                  Markup term from the BLP-markup equation
+:math:`\zeta`                                          :math:`N \times 1`                  Markup term from the :math:`\zeta`-markup equation
+:math:`\mathscr{H}`                                    :math:`J_t \times J_t`              Ownership or product holdings matrix in market :math:`t`
+:math:`\kappa`                                         :math:`F_t \times F_t`              Cooperation matrix in market :math:`t`
+:math:`\Delta`                                         :math:`J_t \times J_t`              Intra-firm matrix of (negative, transposed) demand derivatives in market :math:`t`
+:math:`\Lambda`                                        :math:`J_t \times J_t`              Diagonal matrix used to decompose :math:`\eta` and :math:`\zeta` in market :math:`t`
+:math:`\Gamma`                                         :math:`J_t \times J_t`              Another matrix used to decompose :math:`\eta` and :math:`\zeta` in market :math:`t`
+:math:`d`                                              :math:`I_t \times D`                Observed agent characteristics called demographics in market :math:`t`
+:math:`\nu`                                            :math:`I_t \times K_2`              Unobserved agent characteristics called integration nodes in market :math:`t`
+:math:`a`                                              :math:`I_t \times J_t`              Agent-specific product availability in market :math:`t`
+:math:`w`                                              :math:`I_t \times 1`                Integration weights in market :math:`t`
+:math:`\delta`                                         :math:`N \times 1`                  Mean utility
+:math:`\mu`                                            :math:`J_t \times I_t`              Agent-specific portion of utility in market :math:`t`
+:math:`\epsilon`                                       :math:`N \times 1`                  Type I Extreme Value idiosyncratic preferences
+:math:`\bar{\epsilon}` (:math:`\bar{\epsilon}_{ijt}`)  :math:`N \times 1`                  Type I Extreme Value term used to decompose :math:`\epsilon`
+:math:`\bar{\epsilon}` (:math:`\bar{\epsilon}_{iht}`)  :math:`N \times 1`                  Group-specific term used to decompose :math:`\epsilon`
+:math:`U`                                              :math:`J_t \times I_t`              Indirect utilities
+:math:`V` (:math:`V_{ijt}`)                            :math:`J_t \times I_t`              Indirect utilities minus :math:`\epsilon`
+:math:`V` (:math:`V_{iht}`)                            :math:`J_t \times I_t`              Inclusive value of a nesting group
+:math:`\pi` (:math:`\pi_{jt}`)                         :math:`N \times 1`                  Population-normalized gross expected profits
+:math:`\pi` (:math:`\pi_{ft}`)                         :math:`F_t \times 1`                Population-normalized gross expected profits of a firm in market :math:`t`
+:math:`\beta`                                          :math:`K_1 \times 1`                Demand-side linear parameters
+:math:`\beta^\text{ex}`                                :math:`K_1^\text{ex} \times 1`      Parameters in :math:`\beta` on exogenous product characteristics
+:math:`\alpha`                                         :math:`K_1^\text{en} \times 1`      Parameters in :math:`\beta` on endogenous product characteristics
+:math:`\Sigma`                                         :math:`K_2 \times K_2`              Cholesky root of the covariance matrix for unobserved taste heterogeneity
+:math:`\Pi`                                            :math:`K_2 \times D`                Parameters that measures how agent tastes vary with demographics
+:math:`\rho`                                           :math:`H \times 1`                  Parameters that measures within nesting group correlation
+:math:`\gamma`                                         :math:`K_3 \times 1`                Supply-side linear parameters
+:math:`\gamma^\text{ex}`                               :math:`K_3^\text{ex} \times 1`      Parameters in :math:`\gamma` on exogenous product characteristics
+:math:`\gamma^\text{en}`                               :math:`K_3^\text{en} \times 1`      Parameters in :math:`\gamma` on endogenous product characteristics
+:math:`\theta`                                         :math:`P \times 1`                  Parameters
+:math:`Z_D`                                            :math:`N \times M_D`                Demand-side instruments
+:math:`Z_S`                                            :math:`N \times M_S`                Supply-side instruments
+:math:`Z_C`                                            :math:`N \times M_C`                Covariance instruments
+:math:`W`                                              :math:`M \times M`                  Weighting matrix
+:math:`S`                                              :math:`M \times M`                  Moment covariances
+:math:`q`                                              :math:`1 \times 1`                  Objective value
+:math:`g_D`                                            :math:`N \times M_D`                Demand-side moments
+:math:`g_S`                                            :math:`N \times M_S`                Supply-side moments
+:math:`g_C`                                            :math:`N \times M_C`                Covariance moments
+:math:`g_M`                                            :math:`I \times M_M`                Micro moments
+:math:`g` (:math:`g_{jt}`)                             :math:`N \times (M_D + M_S + M_C)`  Demand-side, supply-side, and covariance moments
+:math:`g` (:math:`g_c`)                                :math:`C \times (M_D + M_S + M_C)`  Clustered demand-side, supply-side, and covariance moments
+:math:`\bar{g}_D`                                      :math:`M_D \times 1`                Averaged demand-side moments
+:math:`\bar{g}_S`                                      :math:`M_S \times 1`                Averaged supply-side moments
+:math:`\bar{g}_C`                                      :math:`M_C \times 1`                Averaged covariance moments
+:math:`\bar{g}_M`                                      :math:`M_M \times 1`                Averaged micro moments
+:math:`\bar{g}`                                        :math:`M \times 1`                  Averaged moments
+:math:`\bar{G}`                                        :math:`M \times P`                  Jacobian of the averaged moments with respect to :math:`\theta`
+:math:`\varepsilon`                                    :math:`J_t \times J_t`              Elasticities of demand in market :math:`t`
+:math:`\mathscr{D}`                                    :math:`J_t \times J_t`              Diversion ratios in market :math:`t`
+:math:`\bar{\mathscr{D}}`                              :math:`J_t \times J_t`              Long-run diversion ratios in market :math:`t`
+:math:`\mathscr{M}`                                    :math:`N \times 1`                  Markups
+:math:`\mathscr{E}`                                    :math:`1 \times 1`                  Aggregate elasticity of demand of a market
+:math:`\text{CS}`                                      :math:`1 \times 1`                  Population-normalized consumer surplus of a market
+:math:`\text{HHI}`                                     :math:`1 \times 1`                  Herfindahl-Hirschman Index of a market
+=====================================================  ==================================  ====================================================================================
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/build_blp_instruments-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/build_blp_instruments-checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999218750000001%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/build_differentiation_instruments-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/build_differentiation_instruments-checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999348958333334%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/build_id_data-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/build_id_data-checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998046875%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/build_integration-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/build_integration-checkpoint.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99990234375%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/build_matrix-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/build_matrix-checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999131944444444%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/build_ownership-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/build_ownership-checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999289772727273%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/data-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/data-checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999218750000001%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/data_to_dict-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/data_to_dict-checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998111979166666%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}, 5: {\'outputs\': '*

 * *            '{0: {\'data\': {\'text/plain\': {insert: [(0, "rec.array([([\'C01Q1\'], [1], '*

 * *            "['F1B04'], [], [], ['F1B04'], [], [], [0.], [-2.5e-01,  4.1e-02, -1.6e+00, -2.7e-01, "*

 * *            '-1.0e-02,  6.9e-03, -9.2e-01,  5.1e-03,  1.3e-01,  2.8e-01,  2.0e-01,  2.5e-01, '*

 * *            '-4.1e-03, -3.6e-02,  7.1e-02,  1.2e-02,  1.7e-02, -1.5e-02,  8.1e-02, -1.6e-02], [], '*

 * *            '[], [-0.],  […]*

```diff
@@ -13,15 +13,15 @@
             "metadata": {
                 "scrolled": true
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -91,22 +91,22 @@
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "rec.array([(['C01Q1'], [1], ['F1B04'], [], [], ['F1B04'], [], [], [0.], [-2.5e-01,  4.1e-02, -1.6e+00, -2.7e-01, -1.0e-02,  6.9e-03, -9.2e-01,  5.1e-03,  1.3e-01,  2.8e-01,  2.0e-01,  2.5e-01, -4.1e-03, -3.6e-02,  7.1e-02,  1.2e-02,  1.7e-02, -1.5e-02,  8.1e-02, -1.6e-02], [], [-0.], [], [], [0.1]),\n",
-                            "           (['C01Q1'], [1], ['F1B06'], [], [], ['F1B06'], [], [], [0.], [-2.1e-01,  5.7e-02, -1.0e+01,  1.5e-01,  4.0e-02,  6.1e-03,  1.1e+00,  8.6e-02,  1.1e-01, -2.7e-02, -1.2e+00, -1.3e-01,  2.6e-03, -6.8e-03, -4.5e-02,  6.7e-05,  3.1e-02,  5.8e-03, -3.2e-02, -1.1e-02], [], [-0.], [], [], [0.1]),\n",
-                            "           (['C01Q1'], [1], ['F1B07'], [], [], ['F1B07'], [], [], [0.], [-2.1e-01,  4.6e-02, -2.3e+00, -3.0e-02,  2.4e-03, -1.3e-02,  3.3e-01, -1.7e-01, -2.3e-01,  3.1e-01,  1.0e+00,  2.0e-01,  9.9e-04,  1.8e-02,  8.2e-02,  3.5e-02,  2.8e-02,  1.3e-02,  4.7e-02,  2.7e-02], [], [ 0.], [], [], [0.1]),\n",
+                            "rec.array([(['C01Q1'], [1], ['F1B04'], [], [], ['F1B04'], [], [], [0.], [-2.5e-01,  4.1e-02, -1.6e+00, -2.7e-01, -1.0e-02,  6.9e-03, -9.2e-01,  5.1e-03,  1.3e-01,  2.8e-01,  2.0e-01,  2.5e-01, -4.1e-03, -3.6e-02,  7.1e-02,  1.2e-02,  1.7e-02, -1.5e-02,  8.1e-02, -1.6e-02], [], [], [-0.], [], [], [0.1]),\n",
+                            "           (['C01Q1'], [1], ['F1B06'], [], [], ['F1B06'], [], [], [0.], [-2.1e-01,  5.7e-02, -1.0e+01,  1.5e-01,  4.0e-02,  6.1e-03,  1.1e+00,  8.6e-02,  1.1e-01, -2.7e-02, -1.2e+00, -1.3e-01,  2.6e-03, -6.8e-03, -4.5e-02,  6.7e-05,  3.1e-02,  5.8e-03, -3.2e-02, -1.1e-02], [], [], [-0.], [], [], [0.1]),\n",
+                            "           (['C01Q1'], [1], ['F1B07'], [], [], ['F1B07'], [], [], [0.], [-2.1e-01,  4.6e-02, -2.3e+00, -3.0e-02,  2.4e-03, -1.3e-02,  3.3e-01, -1.7e-01, -2.3e-01,  3.1e-01,  1.0e+00,  2.0e-01,  9.9e-04,  1.8e-02,  8.2e-02,  3.5e-02,  2.8e-02,  1.3e-02,  4.7e-02,  2.7e-02], [], [], [ 0.], [], [], [0.1]),\n",
                             "           ...,\n",
-                            "           (['C65Q2'], [4], ['F4B10'], [], [], ['F4B10'], [], [], [0.], [-1.2e-01, -3.2e-04, -1.1e+00,  1.8e-01,  3.6e-02, -1.9e-02,  2.4e-01,  5.4e-02, -3.2e-01,  8.7e-02,  2.7e+00,  1.6e-01,  8.8e-04,  3.8e-02,  1.9e-02, -5.2e-02, -1.8e-02,  3.7e-02, -5.8e-02,  3.6e-02], [], [ 0.], [], [], [0.1]),\n",
-                            "           (['C65Q2'], [4], ['F4B12'], [], [], ['F4B12'], [], [], [0.], [-2.0e-01,  3.3e-04, -5.1e-01, -4.5e-03,  3.2e-02,  6.1e-03,  5.7e-01,  2.3e-02,  1.1e-01,  1.9e-01,  2.1e+00,  1.3e-01, -8.1e-03, -1.2e-02, -3.6e-02, -4.3e-03, -1.7e-02, -6.6e-03,  7.2e-03, -1.5e-02], [], [-0.], [], [], [0.1]),\n",
-                            "           (['C65Q2'], [6], ['F6B18'], [], [], ['F6B18'], [], [], [0.], [-1.4e-01,  3.5e-03, -2.9e-01,  2.9e-01,  3.9e-02,  2.0e-02, -1.9e+00, -4.0e-02,  3.8e-01,  1.1e-01,  3.4e+00,  1.1e-01, -6.1e-03, -1.2e-03, -4.7e-02, -2.4e-02, -2.1e-02, -2.9e-02, -2.6e-02, -2.5e-02], [], [-0.], [], [], [0.1])],\n",
-                            "          dtype=[('market_ids', 'O', (1,)), ('firm_ids', 'O', (1,)), ('demand_ids', 'O', (1,)), ('supply_ids', 'O', (0,)), ('nesting_ids', 'O', (0,)), ('product_ids', 'O', (1,)), ('clustering_ids', 'O', (0,)), ('ownership', '<f8', (0,)), ('shares', '<f8', (1,)), ('ZD', '<f8', (20,)), ('ZS', '<f8', (0,)), (((prices,), 'X1'), '<f8', (1,)), (((), 'X2'), '<f8', (0,)), (((), 'X3'), '<f8', (0,)), ('prices', '<f8', (1,))])"
+                            "           (['C65Q2'], [4], ['F4B10'], [], [], ['F4B10'], [], [], [0.], [-1.2e-01, -3.2e-04, -1.1e+00,  1.8e-01,  3.6e-02, -1.9e-02,  2.4e-01,  5.4e-02, -3.2e-01,  8.7e-02,  2.7e+00,  1.6e-01,  8.8e-04,  3.8e-02,  1.9e-02, -5.2e-02, -1.8e-02,  3.7e-02, -5.8e-02,  3.6e-02], [], [], [ 0.], [], [], [0.1]),\n",
+                            "           (['C65Q2'], [4], ['F4B12'], [], [], ['F4B12'], [], [], [0.], [-2.0e-01,  3.3e-04, -5.1e-01, -4.5e-03,  3.2e-02,  6.1e-03,  5.7e-01,  2.3e-02,  1.1e-01,  1.9e-01,  2.1e+00,  1.3e-01, -8.1e-03, -1.2e-02, -3.6e-02, -4.3e-03, -1.7e-02, -6.6e-03,  7.2e-03, -1.5e-02], [], [], [-0.], [], [], [0.1]),\n",
+                            "           (['C65Q2'], [6], ['F6B18'], [], [], ['F6B18'], [], [], [0.], [-1.4e-01,  3.5e-03, -2.9e-01,  2.9e-01,  3.9e-02,  2.0e-02, -1.9e+00, -4.0e-02,  3.8e-01,  1.1e-01,  3.4e+00,  1.1e-01, -6.1e-03, -1.2e-03, -4.7e-02, -2.4e-02, -2.1e-02, -2.9e-02, -2.6e-02, -2.5e-02], [], [], [-0.], [], [], [0.1])],\n",
+                            "          dtype=[('market_ids', 'O', (1,)), ('firm_ids', 'O', (1,)), ('demand_ids', 'O', (1,)), ('supply_ids', 'O', (0,)), ('nesting_ids', 'O', (0,)), ('product_ids', 'O', (1,)), ('clustering_ids', 'O', (0,)), ('ownership', '<f8', (0,)), ('shares', '<f8', (1,)), ('ZD', '<f8', (20,)), ('ZS', '<f8', (0,)), ('ZC', '<f8', (0,)), (((prices,), 'X1'), '<f8', (1,)), (((), 'X2'), '<f8', (0,)), (((), 'X3'), '<f8', (0,)), ('prices', '<f8', (1,))])"
                         ]
                     },
                     "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/formulation-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/formulation-checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999131944444444%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/integration-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/integration-checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998697916666667%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/iteration-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/iteration-checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99990234375%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/micro_dataset-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/micro_dataset-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/micro_part-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/micro_part-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/optimization-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/optimization-checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99990234375%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/.ipynb_checkpoints/parallel-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/api/.ipynb_checkpoints/parallel-checkpoint.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997829861111112%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}, 4: {\'outputs\': '*

 * *            "{0: {'text': {insert: [(3, 'Finished after 00:00:03.\\n')], delete: [3]}}}}}"}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -95,15 +95,15 @@
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Starting a pool of 2 processes ...\n",
                         "Started the process pool after 00:00:00.\n",
                         "Computing elasticities with respect to prices ...\n",
-                        "Finished after 00:00:02.\n",
+                        "Finished after 00:00:03.\n",
                         "\n",
                         "Terminating the pool of 2 processes ...\n",
                         "Terminated the process pool after 00:00:00.\n"
                     ]
                 }
             ],
             "source": [
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/build_blp_instruments.ipynb` & `pyblp-1.1.0/docs/notebooks/api/build_blp_instruments.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999218750000001%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/build_differentiation_instruments.ipynb` & `pyblp-1.1.0/docs/notebooks/api/build_differentiation_instruments.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999348958333334%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/build_id_data.ipynb` & `pyblp-1.1.0/docs/notebooks/api/build_id_data.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998046875%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/build_integration.ipynb` & `pyblp-1.1.0/docs/notebooks/api/build_integration.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99990234375%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/build_matrix.ipynb` & `pyblp-1.1.0/docs/notebooks/api/build_matrix.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999131944444444%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/build_ownership.ipynb` & `pyblp-1.1.0/docs/notebooks/api/build_ownership.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999289772727273%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/data.ipynb` & `pyblp-1.1.0/docs/notebooks/api/data.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999218750000001%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/data_to_dict.ipynb` & `pyblp-1.1.0/docs/notebooks/api/data_to_dict.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998111979166666%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}, 5: {\'outputs\': '*

 * *            '{0: {\'data\': {\'text/plain\': {insert: [(0, "rec.array([([\'C01Q1\'], [1], '*

 * *            "['F1B04'], [], [], ['F1B04'], [], [], [0.], [-2.5e-01,  4.1e-02, -1.6e+00, -2.7e-01, "*

 * *            '-1.0e-02,  6.9e-03, -9.2e-01,  5.1e-03,  1.3e-01,  2.8e-01,  2.0e-01,  2.5e-01, '*

 * *            '-4.1e-03, -3.6e-02,  7.1e-02,  1.2e-02,  1.7e-02, -1.5e-02,  8.1e-02, -1.6e-02], [], '*

 * *            '[], [-0.],  […]*

```diff
@@ -13,15 +13,15 @@
             "metadata": {
                 "scrolled": true
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -91,22 +91,22 @@
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "rec.array([(['C01Q1'], [1], ['F1B04'], [], [], ['F1B04'], [], [], [0.], [-2.5e-01,  4.1e-02, -1.6e+00, -2.7e-01, -1.0e-02,  6.9e-03, -9.2e-01,  5.1e-03,  1.3e-01,  2.8e-01,  2.0e-01,  2.5e-01, -4.1e-03, -3.6e-02,  7.1e-02,  1.2e-02,  1.7e-02, -1.5e-02,  8.1e-02, -1.6e-02], [], [-0.], [], [], [0.1]),\n",
-                            "           (['C01Q1'], [1], ['F1B06'], [], [], ['F1B06'], [], [], [0.], [-2.1e-01,  5.7e-02, -1.0e+01,  1.5e-01,  4.0e-02,  6.1e-03,  1.1e+00,  8.6e-02,  1.1e-01, -2.7e-02, -1.2e+00, -1.3e-01,  2.6e-03, -6.8e-03, -4.5e-02,  6.7e-05,  3.1e-02,  5.8e-03, -3.2e-02, -1.1e-02], [], [-0.], [], [], [0.1]),\n",
-                            "           (['C01Q1'], [1], ['F1B07'], [], [], ['F1B07'], [], [], [0.], [-2.1e-01,  4.6e-02, -2.3e+00, -3.0e-02,  2.4e-03, -1.3e-02,  3.3e-01, -1.7e-01, -2.3e-01,  3.1e-01,  1.0e+00,  2.0e-01,  9.9e-04,  1.8e-02,  8.2e-02,  3.5e-02,  2.8e-02,  1.3e-02,  4.7e-02,  2.7e-02], [], [ 0.], [], [], [0.1]),\n",
+                            "rec.array([(['C01Q1'], [1], ['F1B04'], [], [], ['F1B04'], [], [], [0.], [-2.5e-01,  4.1e-02, -1.6e+00, -2.7e-01, -1.0e-02,  6.9e-03, -9.2e-01,  5.1e-03,  1.3e-01,  2.8e-01,  2.0e-01,  2.5e-01, -4.1e-03, -3.6e-02,  7.1e-02,  1.2e-02,  1.7e-02, -1.5e-02,  8.1e-02, -1.6e-02], [], [], [-0.], [], [], [0.1]),\n",
+                            "           (['C01Q1'], [1], ['F1B06'], [], [], ['F1B06'], [], [], [0.], [-2.1e-01,  5.7e-02, -1.0e+01,  1.5e-01,  4.0e-02,  6.1e-03,  1.1e+00,  8.6e-02,  1.1e-01, -2.7e-02, -1.2e+00, -1.3e-01,  2.6e-03, -6.8e-03, -4.5e-02,  6.7e-05,  3.1e-02,  5.8e-03, -3.2e-02, -1.1e-02], [], [], [-0.], [], [], [0.1]),\n",
+                            "           (['C01Q1'], [1], ['F1B07'], [], [], ['F1B07'], [], [], [0.], [-2.1e-01,  4.6e-02, -2.3e+00, -3.0e-02,  2.4e-03, -1.3e-02,  3.3e-01, -1.7e-01, -2.3e-01,  3.1e-01,  1.0e+00,  2.0e-01,  9.9e-04,  1.8e-02,  8.2e-02,  3.5e-02,  2.8e-02,  1.3e-02,  4.7e-02,  2.7e-02], [], [], [ 0.], [], [], [0.1]),\n",
                             "           ...,\n",
-                            "           (['C65Q2'], [4], ['F4B10'], [], [], ['F4B10'], [], [], [0.], [-1.2e-01, -3.2e-04, -1.1e+00,  1.8e-01,  3.6e-02, -1.9e-02,  2.4e-01,  5.4e-02, -3.2e-01,  8.7e-02,  2.7e+00,  1.6e-01,  8.8e-04,  3.8e-02,  1.9e-02, -5.2e-02, -1.8e-02,  3.7e-02, -5.8e-02,  3.6e-02], [], [ 0.], [], [], [0.1]),\n",
-                            "           (['C65Q2'], [4], ['F4B12'], [], [], ['F4B12'], [], [], [0.], [-2.0e-01,  3.3e-04, -5.1e-01, -4.5e-03,  3.2e-02,  6.1e-03,  5.7e-01,  2.3e-02,  1.1e-01,  1.9e-01,  2.1e+00,  1.3e-01, -8.1e-03, -1.2e-02, -3.6e-02, -4.3e-03, -1.7e-02, -6.6e-03,  7.2e-03, -1.5e-02], [], [-0.], [], [], [0.1]),\n",
-                            "           (['C65Q2'], [6], ['F6B18'], [], [], ['F6B18'], [], [], [0.], [-1.4e-01,  3.5e-03, -2.9e-01,  2.9e-01,  3.9e-02,  2.0e-02, -1.9e+00, -4.0e-02,  3.8e-01,  1.1e-01,  3.4e+00,  1.1e-01, -6.1e-03, -1.2e-03, -4.7e-02, -2.4e-02, -2.1e-02, -2.9e-02, -2.6e-02, -2.5e-02], [], [-0.], [], [], [0.1])],\n",
-                            "          dtype=[('market_ids', 'O', (1,)), ('firm_ids', 'O', (1,)), ('demand_ids', 'O', (1,)), ('supply_ids', 'O', (0,)), ('nesting_ids', 'O', (0,)), ('product_ids', 'O', (1,)), ('clustering_ids', 'O', (0,)), ('ownership', '<f8', (0,)), ('shares', '<f8', (1,)), ('ZD', '<f8', (20,)), ('ZS', '<f8', (0,)), (((prices,), 'X1'), '<f8', (1,)), (((), 'X2'), '<f8', (0,)), (((), 'X3'), '<f8', (0,)), ('prices', '<f8', (1,))])"
+                            "           (['C65Q2'], [4], ['F4B10'], [], [], ['F4B10'], [], [], [0.], [-1.2e-01, -3.2e-04, -1.1e+00,  1.8e-01,  3.6e-02, -1.9e-02,  2.4e-01,  5.4e-02, -3.2e-01,  8.7e-02,  2.7e+00,  1.6e-01,  8.8e-04,  3.8e-02,  1.9e-02, -5.2e-02, -1.8e-02,  3.7e-02, -5.8e-02,  3.6e-02], [], [], [ 0.], [], [], [0.1]),\n",
+                            "           (['C65Q2'], [4], ['F4B12'], [], [], ['F4B12'], [], [], [0.], [-2.0e-01,  3.3e-04, -5.1e-01, -4.5e-03,  3.2e-02,  6.1e-03,  5.7e-01,  2.3e-02,  1.1e-01,  1.9e-01,  2.1e+00,  1.3e-01, -8.1e-03, -1.2e-02, -3.6e-02, -4.3e-03, -1.7e-02, -6.6e-03,  7.2e-03, -1.5e-02], [], [], [-0.], [], [], [0.1]),\n",
+                            "           (['C65Q2'], [6], ['F6B18'], [], [], ['F6B18'], [], [], [0.], [-1.4e-01,  3.5e-03, -2.9e-01,  2.9e-01,  3.9e-02,  2.0e-02, -1.9e+00, -4.0e-02,  3.8e-01,  1.1e-01,  3.4e+00,  1.1e-01, -6.1e-03, -1.2e-03, -4.7e-02, -2.4e-02, -2.1e-02, -2.9e-02, -2.6e-02, -2.5e-02], [], [], [-0.], [], [], [0.1])],\n",
+                            "          dtype=[('market_ids', 'O', (1,)), ('firm_ids', 'O', (1,)), ('demand_ids', 'O', (1,)), ('supply_ids', 'O', (0,)), ('nesting_ids', 'O', (0,)), ('product_ids', 'O', (1,)), ('clustering_ids', 'O', (0,)), ('ownership', '<f8', (0,)), ('shares', '<f8', (1,)), ('ZD', '<f8', (20,)), ('ZS', '<f8', (0,)), ('ZC', '<f8', (0,)), (((prices,), 'X1'), '<f8', (1,)), (((), 'X2'), '<f8', (0,)), (((), 'X3'), '<f8', (0,)), ('prices', '<f8', (1,))])"
                         ]
                     },
                     "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/formulation.ipynb` & `pyblp-1.1.0/docs/notebooks/api/formulation.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999131944444444%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/integration.ipynb` & `pyblp-1.1.0/docs/notebooks/api/integration.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998697916666667%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/iteration.ipynb` & `pyblp-1.1.0/docs/notebooks/api/iteration.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99990234375%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/optimization.ipynb` & `pyblp-1.1.0/docs/notebooks/api/optimization.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99990234375%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}}'}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/api/parallel.ipynb` & `pyblp-1.1.0/docs/notebooks/api/parallel.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997829861111112%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}, 4: {\'outputs\': '*

 * *            "{0: {'text': {insert: [(3, 'Finished after 00:00:03.\\n')], delete: [3]}}}}}"}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -95,15 +95,15 @@
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Starting a pool of 2 processes ...\n",
                         "Started the process pool after 00:00:00.\n",
                         "Computing elasticities with respect to prices ...\n",
-                        "Finished after 00:00:02.\n",
+                        "Finished after 00:00:03.\n",
                         "\n",
                         "Terminating the pool of 2 processes ...\n",
                         "Terminated the process pool after 00:00:00.\n"
                     ]
                 }
             ],
             "source": [
```

### Comparing `pyblp-1.0.0/docs/notebooks/tutorial/.ipynb_checkpoints/blp-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/tutorial/.ipynb_checkpoints/blp-checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999559445488722%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}, 17: '*

 * *            "{'outputs': {0: {'data': {'text/plain': {insert: [(5, ' 2    +5.0E+02     "*

 * *            '+1.1E-08        +4.9E-01         +5.1E+02         0        0         '*

 * *            "+4.2E+09          +3.8E+08     \\n'), (13, ' 00:10:14       No           58           "*

 * *            "126         36807       112905   \\n')], delete: [13, 5]}}}}}}"}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -606,23 +606,23 @@
                     "data": {
                         "text/plain": [
                             "Problem Results Summary:\n",
                             "=======================================================================================================================\n",
                             "GMM   Objective    Projected    Reduced Hessian  Reduced Hessian  Clipped  Clipped  Weighting Matrix  Covariance Matrix\n",
                             "Step    Value    Gradient Norm  Min Eigenvalue   Max Eigenvalue   Shares    Costs   Condition Number  Condition Number \n",
                             "----  ---------  -------------  ---------------  ---------------  -------  -------  ----------------  -----------------\n",
-                            " 2    +5.0E+02     +4.1E-08        +4.9E-01         +5.1E+02         0        0         +4.2E+09          +3.8E+08     \n",
+                            " 2    +5.0E+02     +1.1E-08        +4.9E-01         +5.1E+02         0        0         +4.2E+09          +3.8E+08     \n",
                             "=======================================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:03:29       No           55           112         34229       104904   \n",
+                            " 00:10:14       No           58           126         36807       112905   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs Adjusted for 999 Clusters in Parentheses):\n",
                             "===================================================================================================\n",
                             "Sigma:      1        prices      hpwt        air         mpd        space     |   Pi:    1*1/income\n",
                             "------  ----------  --------  ----------  ----------  ----------  ----------  |  ------  ----------\n",
                             "  1      +2.0E+00                                                             |    1      +0.0E+00 \n",
```

### Comparing `pyblp-1.0.0/docs/notebooks/tutorial/.ipynb_checkpoints/logit_nested-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/tutorial/.ipynb_checkpoints/logit_nested-checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999714516488414%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}, 17: '*

 * *            "{'outputs': {0: {'data': {'text/plain': {insert: [(5, ' 2    +2.0E+02     "*

 * *            "+1.2E-09     +1.1E+04     0         +2.0E+09          +3.0E+04     \\n'), (13, ' "*

 * *            "00:00:04       Yes          3             8     \\n')], delete: [13, 5]}}}}}, 21: "*

 * *            "{'outputs': {0: {'data': {'text/plain': {insert: [(5, ' 2    +6.9E+02     "*

 * *            "+3.0E-10     +5.6E+03     0         +5.1 […]*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -559,23 +559,23 @@
                     "data": {
                         "text/plain": [
                             "Problem Results Summary:\n",
                             "======================================================================================\n",
                             "GMM   Objective    Projected    Reduced   Clipped  Weighting Matrix  Covariance Matrix\n",
                             "Step    Value    Gradient Norm  Hessian   Shares   Condition Number  Condition Number \n",
                             "----  ---------  -------------  --------  -------  ----------------  -----------------\n",
-                            " 2    +2.0E+02     +3.0E-09     +1.1E+04     0         +2.0E+09          +3.0E+04     \n",
+                            " 2    +2.0E+02     +1.2E-09     +1.1E+04     0         +2.0E+09          +3.0E+04     \n",
                             "======================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "=================================================\n",
                             "Computation  Optimizer  Optimization   Objective \n",
                             "   Time      Converged   Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------\n",
-                            " 00:00:02       Yes          3             8     \n",
+                            " 00:00:04       Yes          3             8     \n",
                             "=================================================\n",
                             "\n",
                             "Rho Estimates (Robust SEs in Parentheses):\n",
                             "==========\n",
                             "All Groups\n",
                             "----------\n",
                             " +9.8E-01 \n",
@@ -658,23 +658,23 @@
                     "data": {
                         "text/plain": [
                             "Problem Results Summary:\n",
                             "======================================================================================\n",
                             "GMM   Objective    Projected    Reduced   Clipped  Weighting Matrix  Covariance Matrix\n",
                             "Step    Value    Gradient Norm  Hessian   Shares   Condition Number  Condition Number \n",
                             "----  ---------  -------------  --------  -------  ----------------  -----------------\n",
-                            " 2    +6.9E+02     +5.5E-09     +5.6E+03     0         +5.1E+08          +2.0E+04     \n",
+                            " 2    +6.9E+02     +3.0E-10     +5.6E+03     0         +5.1E+08          +2.0E+04     \n",
                             "======================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "=================================================\n",
                             "Computation  Optimizer  Optimization   Objective \n",
                             "   Time      Converged   Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------\n",
-                            " 00:00:02       Yes          3             8     \n",
+                            " 00:00:03       Yes          3             8     \n",
                             "=================================================\n",
                             "\n",
                             "Rho Estimates (Robust SEs in Parentheses):\n",
                             "==========\n",
                             "All Groups\n",
                             "----------\n",
                             " +8.9E-01 \n",
```

### Comparing `pyblp-1.0.0/docs/notebooks/tutorial/.ipynb_checkpoints/nevo-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/tutorial/.ipynb_checkpoints/nevo-checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999633168392696%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}, 18: '*

 * *            "{'outputs': {0: {'data': {'text/plain': {insert: [(13, ' 00:01:48       Yes          "*

 * *            "58           75          82256       252902   \\n')], delete: [13]}}}}}, 19: "*

 * *            "{'outputs': {0: {'data': {'text/plain': {insert: [(5, ' 2    +1.6E+02   +1.1E-05     "*

 * *            "+1.6E-02        +5.3E+03        0         +5.3E+07          +5.0E+20     \\n'), (13, "*

 * *            "' 00:04:57       No […]*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -585,15 +585,15 @@
                             "=======================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:01:37       Yes          58           75          83853       257686   \n",
+                            " 00:01:48       Yes          58           75          82256       252902   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs in Parentheses):\n",
                             "=========================================================================================================================\n",
                             "Sigma:      1         prices      sugar       mushy     |  Sigma Squared:      1         prices      sugar       mushy   \n",
                             "------  ----------  ----------  ----------  ----------  |  --------------  ----------  ----------  ----------  ----------\n",
                             "  1      +1.2E+00                                       |        1          +1.5E+00    -1.4E+01    +7.3E-02    -7.1E-01 \n",
@@ -637,48 +637,48 @@
                     "data": {
                         "text/plain": [
                             "Problem Results Summary:\n",
                             "=======================================================================================================\n",
                             "GMM   Objective  Gradient      Hessian         Hessian     Clipped  Weighting Matrix  Covariance Matrix\n",
                             "Step    Value      Norm    Min Eigenvalue  Max Eigenvalue  Shares   Condition Number  Condition Number \n",
                             "----  ---------  --------  --------------  --------------  -------  ----------------  -----------------\n",
-                            " 2    +1.6E+02   +3.2E-05     +1.6E-02        +5.3E+03        0         +5.3E+07          +1.2E+21     \n",
+                            " 2    +1.6E+02   +1.1E-05     +1.6E-02        +5.3E+03        0         +5.3E+07          +5.0E+20     \n",
                             "=======================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:03:02       Yes          64           78          68670       212085   \n",
+                            " 00:04:57       No           63           130         96884       301280   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs in Parentheses):\n",
                             "=========================================================================================================================\n",
                             "Sigma:      1         prices      sugar       mushy     |  Sigma Squared:      1         prices      sugar       mushy   \n",
                             "------  ----------  ----------  ----------  ----------  |  --------------  ----------  ----------  ----------  ----------\n",
                             "  1      -7.4E-01                                       |        1          +5.5E-01    -9.4E+00    +8.3E-02    -1.1E-01 \n",
-                            "        (+2.1E+00)                                      |                  (+3.1E+00)  (+3.2E+01)  (+1.7E-01)  (+6.3E-01)\n",
+                            "        (+2.3E+00)                                      |                  (+3.4E+00)  (+3.5E+01)  (+1.6E-01)  (+6.4E-01)\n",
                             "                                                        |                                                                \n",
-                            "prices   +1.3E+01    -8.8E-06                           |      prices       -9.4E+00    +1.6E+02    -1.4E+00    +1.9E+00 \n",
-                            "        (+7.7E+00)  (+2.3E+03)                          |                  (+3.2E+01)  (+2.0E+02)  (+7.8E-01)  (+8.8E+00)\n",
+                            "prices   +1.3E+01    +6.6E-06                           |      prices       -9.4E+00    +1.6E+02    -1.4E+00    +1.9E+00 \n",
+                            "        (+7.5E+00)  (+2.7E+03)                          |                  (+3.5E+01)  (+1.9E+02)  (+8.0E-01)  (+8.9E+00)\n",
                             "                                                        |                                                                \n",
-                            "sugar    -1.1E-01    +1.1E-07    -3.0E-09               |      sugar        +8.3E-02    -1.4E+00    +1.2E-02    -1.7E-02 \n",
-                            "        (+2.1E-01)  (+1.9E+05)  (+7.3E+02)              |                  (+1.7E-01)  (+7.8E-01)  (+2.1E-02)  (+1.5E-01)\n",
+                            "sugar    -1.1E-01    -7.4E-08    -8.9E-09               |      sugar        +8.3E-02    -1.4E+00    +1.2E-02    -1.7E-02 \n",
+                            "        (+2.0E-01)  (+2.2E+05)  (+5.2E+04)              |                  (+1.6E-01)  (+8.0E-01)  (+2.2E-02)  (+1.6E-01)\n",
                             "                                                        |                                                                \n",
-                            "mushy    +1.5E-01    +4.6E-07    +1.9E-08    -1.3E-08   |      mushy        -1.1E-01    +1.9E+00    -1.7E-02    +2.2E-02 \n",
-                            "        (+6.8E-01)  (+3.5E+03)  (+6.3E+02)  (+1.8E+02)  |                  (+6.3E-01)  (+8.8E+00)  (+1.5E-01)  (+2.0E-01)\n",
+                            "mushy    +1.5E-01    -4.3E-07    +1.6E-07    +4.7E-08   |      mushy        -1.1E-01    +1.9E+00    -1.7E-02    +2.2E-02 \n",
+                            "        (+6.8E-01)  (+5.0E+03)  (+7.0E+02)  (+4.3E+02)  |                  (+6.4E-01)  (+8.9E+00)  (+1.6E-01)  (+2.0E-01)\n",
                             "=========================================================================================================================\n",
                             "\n",
                             "Beta Estimates (Robust SEs in Parentheses):\n",
                             "==========\n",
                             "  prices  \n",
                             "----------\n",
                             " -3.1E+01 \n",
-                            "(+4.4E+00)\n",
+                            "(+4.0E+00)\n",
                             "=========="
                         ]
                     },
                     "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -705,15 +705,15 @@
                             "=======================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:00:23       Yes          16           24          19540        60462   \n",
+                            " 00:00:28       Yes          16           24          19529        60447   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs in Parentheses):\n",
                             "======================================================\n",
                             "Sigma:      1         prices      sugar       mushy   \n",
                             "------  ----------  ----------  ----------  ----------\n",
                             "  1      +5.2E-02                                     \n",
@@ -1017,23 +1017,23 @@
                     "data": {
                         "text/plain": [
                             "Problem Results Summary:\n",
                             "=======================================================================================================\n",
                             "GMM   Objective  Gradient      Hessian         Hessian     Clipped  Weighting Matrix  Covariance Matrix\n",
                             "Step    Value      Norm    Min Eigenvalue  Max Eigenvalue  Shares   Condition Number  Condition Number \n",
                             "----  ---------  --------  --------------  --------------  -------  ----------------  -----------------\n",
-                            " 1    +4.6E+00   +6.9E-06     +3.2E-05        +1.6E+04        0         +6.9E+07          +8.4E+08     \n",
+                            " 1    +4.6E+00   +6.9E-06     +3.3E-05        +1.6E+04        0         +6.9E+07          +8.4E+08     \n",
                             "=======================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:01:00       Yes          51           57          46386       143970   \n",
+                            " 00:01:12       Yes          51           57          46389       143977   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs in Parentheses):\n",
                             "=====================================================================================================================\n",
                             "Sigma:      1         prices      sugar       mushy     |   Pi:      income    income_squared     age        child   \n",
                             "------  ----------  ----------  ----------  ----------  |  ------  ----------  --------------  ----------  ----------\n",
                             "  1      +5.6E-01                                       |    1      +2.3E+00      +0.0E+00      +1.3E+00    +0.0E+00 \n",
@@ -1121,15 +1121,15 @@
                             "=======================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:00:45       Yes          34           40          34392       106492   \n",
+                            " 00:00:53       Yes          34           40          34390       106492   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs in Parentheses):\n",
                             "=====================================================================================================================\n",
                             "Sigma:      1         prices      sugar       mushy     |   Pi:      income    income_squared     age        child   \n",
                             "------  ----------  ----------  ----------  ----------  |  ------  ----------  --------------  ----------  ----------\n",
                             "  1      +3.7E-01                                       |    1      +3.1E+00      +0.0E+00      +1.2E+00    +0.0E+00 \n",
@@ -1194,15 +1194,15 @@
                             "=======================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:00:45       Yes          34           40          34403       106539   \n",
+                            " 00:00:55       Yes          34           40          34371       106443   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs in Parentheses):\n",
                             "=====================================================================================================\n",
                             "Sigma:      1         prices      sugar       mushy     |   Pi:      income       age        child   \n",
                             "------  ----------  ----------  ----------  ----------  |  ------  ----------  ----------  ----------\n",
                             "  1      +3.7E-01                                       |    1      +3.1E+00    +1.2E+00    +0.0E+00 \n",
```

### Comparing `pyblp-1.0.0/docs/notebooks/tutorial/.ipynb_checkpoints/petrin-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/tutorial/.ipynb_checkpoints/petrin-checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998521013592292%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {1: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}, 16: {\'source\': '*

 * *            "{insert: [(2, 'By using $1 + J_t$ instead of $J_t$, we are specifying that the micro "*

 * *            'dataset contains observations of the outside option $j = 0$. If we instead specified '*

 * *            'a matrix of shape $I_t \\\\times J_t$, this would be the same as setting the first '*

 * *            "column equal to all zeros, so that outside choices are not sampled from.\\n')], "*

 * *            "delet […]*

```diff
@@ -25,15 +25,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -653,15 +653,15 @@
         {
             "cell_type": "markdown",
             "id": "2b95e675",
             "metadata": {},
             "source": [
                 "We called the dataset \"CEX\", defined the number of observations in it, and also defined a lambda function for computing survey weights in a market. The `compute_weights` function has three arguments: the current market's ID $t$, the $J_t$ :class:`Products` inside the market, and the $I_t$ :class:`Agents` inside the market. In this case, we are assuming that each product and agent/consumer type are sampled with equal probability, so we simply return a matrix of ones of shape $I_t \\times (1 + J_t)$. This sets each $w_{dijt} = 1$.\n",
                 "\n",
-                "By using $1 + J_t$ instead of $J_t$, we are specifying that the micro dataset contains observations of the outside option $j = 0$. If we instead specified a matrix of shape $I_t \\times (1 + J_t)$, this would be the same as setting the first column equal to all zeros, so that outside choices are not sampled from.\n",
+                "By using $1 + J_t$ instead of $J_t$, we are specifying that the micro dataset contains observations of the outside option $j = 0$. If we instead specified a matrix of shape $I_t \\times J_t$, this would be the same as setting the first column equal to all zeros, so that outside choices are not sampled from.\n",
                 "\n",
                 "We will be matching a few different statistics that were computed from this survey. For convenience, they are packaged in a data file with pyblp.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
@@ -1057,23 +1057,23 @@
                     "data": {
                         "text/plain": [
                             "Problem Results Summary:\n",
                             "=======================================================================================================\n",
                             "GMM   Objective  Gradient      Hessian         Hessian     Clipped  Weighting Matrix  Covariance Matrix\n",
                             "Step    Value      Norm    Min Eigenvalue  Max Eigenvalue  Shares   Condition Number  Condition Number \n",
                             "----  ---------  --------  --------------  --------------  -------  ----------------  -----------------\n",
-                            " 2    +1.8E+02   +4.4E-05     +4.3E-01        +1.3E+03        0         +2.8E+11          +8.1E+07     \n",
+                            " 2    +1.8E+02   +4.3E-05     +3.8E-01        +1.3E+03        0         +2.8E+11          +8.1E+07     \n",
                             "=======================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:26:42       Yes          72           87          10899        33588   \n",
+                            " 00:34:10       Yes          72           87          10905        33592   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs Adjusted for 898 Clusters in Parentheses):\n",
                             "================================================================================================================================================================================================================================================\n",
                             "Sigma:       1       -prices      hpwt       space        air         mpd         fwd         mi        sw        su        pv     |    Pi:       1      low/income  mid/income  high/income  fv*log(fs)    age        fs       mid       high  \n",
                             "-------  ----------  --------  ----------  ----------  ----------  ----------  ----------  --------  --------  --------  --------  |  -------  --------  ----------  ----------  -----------  ----------  --------  --------  --------  --------\n",
                             "   1      +3.0E-02                                                                                                                 |     1     +0.0E+00   +0.0E+00    +0.0E+00    +0.0E+00     +0.0E+00   +0.0E+00  +0.0E+00  +0.0E+00  +0.0E+00\n",
@@ -1263,15 +1263,15 @@
             "execution_count": 19,
             "id": "b4d00395",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "array([[425.90823299]])"
+                            "array([[425.90824856]])"
                         ]
                     },
                     "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/tutorial/.ipynb_checkpoints/post_estimation-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/tutorial/.ipynb_checkpoints/post_estimation-checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999827226283909%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}, 5: {\'outputs\': '*

 * *            "{0: {'data': {'text/plain': {insert: [(5, ' 1    +4.6E+00   +6.9E-06     "*

 * *            "+3.3E-05        +1.6E+04        0         +6.9E+07          +8.4E+08     \\n'), (13, "*

 * *            "' 00:01:16       Yes          51           57          46389       143977   \\n')], "*

 * *            "delete: [13, 5]}}}}}, 37: {'outputs': {0: {'data': {'text/plain': {insert: [(5, ' "*

 * *            "00:00:09       […]*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -113,23 +113,23 @@
                     "data": {
                         "text/plain": [
                             "Problem Results Summary:\n",
                             "=======================================================================================================\n",
                             "GMM   Objective  Gradient      Hessian         Hessian     Clipped  Weighting Matrix  Covariance Matrix\n",
                             "Step    Value      Norm    Min Eigenvalue  Max Eigenvalue  Shares   Condition Number  Condition Number \n",
                             "----  ---------  --------  --------------  --------------  -------  ----------------  -----------------\n",
-                            " 1    +4.6E+00   +6.9E-06     +3.2E-05        +1.6E+04        0         +6.9E+07          +8.4E+08     \n",
+                            " 1    +4.6E+00   +6.9E-06     +3.3E-05        +1.6E+04        0         +6.9E+07          +8.4E+08     \n",
                             "=======================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:01:05       Yes          51           57          46386       143970   \n",
+                            " 00:01:16       Yes          51           57          46389       143977   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs in Parentheses):\n",
                             "=====================================================================================================================\n",
                             "Sigma:      1         prices      sugar       mushy     |   Pi:      income    income_squared     age        child   \n",
                             "------  ----------  ----------  ----------  ----------  |  ------  ----------  --------------  ----------  ----------\n",
                             "  1      +5.6E-01                                       |    1      +2.3E+00      +0.0E+00      +1.3E+00    +0.0E+00 \n",
@@ -605,15 +605,15 @@
                     "data": {
                         "text/plain": [
                             "Bootstrapped Results Summary:\n",
                             "======================\n",
                             "Computation  Bootstrap\n",
                             "   Time        Draws  \n",
                             "-----------  ---------\n",
-                            " 00:00:08       100   \n",
+                            " 00:00:09       100   \n",
                             "======================"
                         ]
                     },
                     "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -823,15 +823,15 @@
                             "=======================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:01:03       Yes          42           50          45892       142159   \n",
+                            " 00:01:05       Yes          42           50          45902       142164   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs in Parentheses):\n",
                             "=====================================================================================================================\n",
                             "Sigma:      1         prices      sugar       mushy     |   Pi:      income    income_squared     age        child   \n",
                             "------  ----------  ----------  ----------  ----------  |  ------  ----------  --------------  ----------  ----------\n",
                             "  1      +2.1E-01                                       |    1      +6.0E+00      +0.0E+00      +1.6E-01    +0.0E+00 \n",
@@ -1446,23 +1446,23 @@
                     "data": {
                         "text/plain": [
                             "Problem Results Summary:\n",
                             "=======================================================================================================\n",
                             "GMM   Objective  Gradient      Hessian         Hessian     Clipped  Weighting Matrix  Covariance Matrix\n",
                             "Step    Value      Norm    Min Eigenvalue  Max Eigenvalue  Shares   Condition Number  Condition Number \n",
                             "----  ---------  --------  --------------  --------------  -------  ----------------  -----------------\n",
-                            " 1    +1.1E+02   +3.8E-06     +3.0E-03        +8.3E+04        0         +2.2E+08          +4.1E+07     \n",
+                            " 1    +1.1E+02   +8.8E-06     +2.3E-03        +8.3E+04        0         +2.2E+08          +4.1E+07     \n",
                             "=======================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:00:59       Yes          34           42          33337       103774   \n",
+                            " 00:01:26       Yes          34           55          42977       133908   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs in Parentheses):\n",
                             "=====================================================================================================================\n",
                             "Sigma:      1         prices      sugar       mushy     |   Pi:      income    income_squared     age        child   \n",
                             "------  ----------  ----------  ----------  ----------  |  ------  ----------  --------------  ----------  ----------\n",
                             "  1      +4.6E-01                                       |    1      +4.8E+00      +0.0E+00      +6.5E-01    +0.0E+00 \n",
```

### Comparing `pyblp-1.0.0/docs/notebooks/tutorial/.ipynb_checkpoints/simulation-checkpoint.ipynb` & `pyblp-1.1.0/docs/notebooks/tutorial/.ipynb_checkpoints/simulation-checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999568256578948%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}, 13: '*

 * *            "{'outputs': {0: {'data': {'text/plain': {insert: [(13, ' 00:00:16       Yes          "*

 * *            "23           30          8295         26312   \\n')], delete: [13]}}}}}}"}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -265,15 +265,15 @@
                             "==============================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:00:13       Yes          23           30          8295         26314   \n",
+                            " 00:00:16       Yes          23           30          8295         26312   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs in Parentheses):\n",
                             "==================\n",
                             "Sigma:      x     \n",
                             "------  ----------\n",
                             "  x      +7.8E-01 \n",
```

### Comparing `pyblp-1.0.0/docs/notebooks/tutorial/blp.ipynb` & `pyblp-1.1.0/docs/notebooks/tutorial/blp.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999559445488722%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}, 17: '*

 * *            "{'outputs': {0: {'data': {'text/plain': {insert: [(5, ' 2    +5.0E+02     "*

 * *            '+1.1E-08        +4.9E-01         +5.1E+02         0        0         '*

 * *            "+4.2E+09          +3.8E+08     \\n'), (13, ' 00:10:14       No           58           "*

 * *            "126         36807       112905   \\n')], delete: [13, 5]}}}}}}"}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -606,23 +606,23 @@
                     "data": {
                         "text/plain": [
                             "Problem Results Summary:\n",
                             "=======================================================================================================================\n",
                             "GMM   Objective    Projected    Reduced Hessian  Reduced Hessian  Clipped  Clipped  Weighting Matrix  Covariance Matrix\n",
                             "Step    Value    Gradient Norm  Min Eigenvalue   Max Eigenvalue   Shares    Costs   Condition Number  Condition Number \n",
                             "----  ---------  -------------  ---------------  ---------------  -------  -------  ----------------  -----------------\n",
-                            " 2    +5.0E+02     +4.1E-08        +4.9E-01         +5.1E+02         0        0         +4.2E+09          +3.8E+08     \n",
+                            " 2    +5.0E+02     +1.1E-08        +4.9E-01         +5.1E+02         0        0         +4.2E+09          +3.8E+08     \n",
                             "=======================================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:03:29       No           55           112         34229       104904   \n",
+                            " 00:10:14       No           58           126         36807       112905   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs Adjusted for 999 Clusters in Parentheses):\n",
                             "===================================================================================================\n",
                             "Sigma:      1        prices      hpwt        air         mpd        space     |   Pi:    1*1/income\n",
                             "------  ----------  --------  ----------  ----------  ----------  ----------  |  ------  ----------\n",
                             "  1      +2.0E+00                                                             |    1      +0.0E+00 \n",
```

### Comparing `pyblp-1.0.0/docs/notebooks/tutorial/logit_nested.ipynb` & `pyblp-1.1.0/docs/notebooks/tutorial/logit_nested.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999714516488414%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}, 17: '*

 * *            "{'outputs': {0: {'data': {'text/plain': {insert: [(5, ' 2    +2.0E+02     "*

 * *            "+1.2E-09     +1.1E+04     0         +2.0E+09          +3.0E+04     \\n'), (13, ' "*

 * *            "00:00:04       Yes          3             8     \\n')], delete: [13, 5]}}}}}, 21: "*

 * *            "{'outputs': {0: {'data': {'text/plain': {insert: [(5, ' 2    +6.9E+02     "*

 * *            "+3.0E-10     +5.6E+03     0         +5.1 […]*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -559,23 +559,23 @@
                     "data": {
                         "text/plain": [
                             "Problem Results Summary:\n",
                             "======================================================================================\n",
                             "GMM   Objective    Projected    Reduced   Clipped  Weighting Matrix  Covariance Matrix\n",
                             "Step    Value    Gradient Norm  Hessian   Shares   Condition Number  Condition Number \n",
                             "----  ---------  -------------  --------  -------  ----------------  -----------------\n",
-                            " 2    +2.0E+02     +3.0E-09     +1.1E+04     0         +2.0E+09          +3.0E+04     \n",
+                            " 2    +2.0E+02     +1.2E-09     +1.1E+04     0         +2.0E+09          +3.0E+04     \n",
                             "======================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "=================================================\n",
                             "Computation  Optimizer  Optimization   Objective \n",
                             "   Time      Converged   Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------\n",
-                            " 00:00:02       Yes          3             8     \n",
+                            " 00:00:04       Yes          3             8     \n",
                             "=================================================\n",
                             "\n",
                             "Rho Estimates (Robust SEs in Parentheses):\n",
                             "==========\n",
                             "All Groups\n",
                             "----------\n",
                             " +9.8E-01 \n",
@@ -658,23 +658,23 @@
                     "data": {
                         "text/plain": [
                             "Problem Results Summary:\n",
                             "======================================================================================\n",
                             "GMM   Objective    Projected    Reduced   Clipped  Weighting Matrix  Covariance Matrix\n",
                             "Step    Value    Gradient Norm  Hessian   Shares   Condition Number  Condition Number \n",
                             "----  ---------  -------------  --------  -------  ----------------  -----------------\n",
-                            " 2    +6.9E+02     +5.5E-09     +5.6E+03     0         +5.1E+08          +2.0E+04     \n",
+                            " 2    +6.9E+02     +3.0E-10     +5.6E+03     0         +5.1E+08          +2.0E+04     \n",
                             "======================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "=================================================\n",
                             "Computation  Optimizer  Optimization   Objective \n",
                             "   Time      Converged   Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------\n",
-                            " 00:00:02       Yes          3             8     \n",
+                            " 00:00:03       Yes          3             8     \n",
                             "=================================================\n",
                             "\n",
                             "Rho Estimates (Robust SEs in Parentheses):\n",
                             "==========\n",
                             "All Groups\n",
                             "----------\n",
                             " +8.9E-01 \n",
```

### Comparing `pyblp-1.0.0/docs/notebooks/tutorial/nevo.ipynb` & `pyblp-1.1.0/docs/notebooks/tutorial/nevo.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999633168392696%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}, 18: '*

 * *            "{'outputs': {0: {'data': {'text/plain': {insert: [(13, ' 00:01:48       Yes          "*

 * *            "58           75          82256       252902   \\n')], delete: [13]}}}}}, 19: "*

 * *            "{'outputs': {0: {'data': {'text/plain': {insert: [(5, ' 2    +1.6E+02   +1.1E-05     "*

 * *            "+1.6E-02        +5.3E+03        0         +5.3E+07          +5.0E+20     \\n'), (13, "*

 * *            "' 00:04:57       No […]*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -585,15 +585,15 @@
                             "=======================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:01:37       Yes          58           75          83853       257686   \n",
+                            " 00:01:48       Yes          58           75          82256       252902   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs in Parentheses):\n",
                             "=========================================================================================================================\n",
                             "Sigma:      1         prices      sugar       mushy     |  Sigma Squared:      1         prices      sugar       mushy   \n",
                             "------  ----------  ----------  ----------  ----------  |  --------------  ----------  ----------  ----------  ----------\n",
                             "  1      +1.2E+00                                       |        1          +1.5E+00    -1.4E+01    +7.3E-02    -7.1E-01 \n",
@@ -637,48 +637,48 @@
                     "data": {
                         "text/plain": [
                             "Problem Results Summary:\n",
                             "=======================================================================================================\n",
                             "GMM   Objective  Gradient      Hessian         Hessian     Clipped  Weighting Matrix  Covariance Matrix\n",
                             "Step    Value      Norm    Min Eigenvalue  Max Eigenvalue  Shares   Condition Number  Condition Number \n",
                             "----  ---------  --------  --------------  --------------  -------  ----------------  -----------------\n",
-                            " 2    +1.6E+02   +3.2E-05     +1.6E-02        +5.3E+03        0         +5.3E+07          +1.2E+21     \n",
+                            " 2    +1.6E+02   +1.1E-05     +1.6E-02        +5.3E+03        0         +5.3E+07          +5.0E+20     \n",
                             "=======================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:03:02       Yes          64           78          68670       212085   \n",
+                            " 00:04:57       No           63           130         96884       301280   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs in Parentheses):\n",
                             "=========================================================================================================================\n",
                             "Sigma:      1         prices      sugar       mushy     |  Sigma Squared:      1         prices      sugar       mushy   \n",
                             "------  ----------  ----------  ----------  ----------  |  --------------  ----------  ----------  ----------  ----------\n",
                             "  1      -7.4E-01                                       |        1          +5.5E-01    -9.4E+00    +8.3E-02    -1.1E-01 \n",
-                            "        (+2.1E+00)                                      |                  (+3.1E+00)  (+3.2E+01)  (+1.7E-01)  (+6.3E-01)\n",
+                            "        (+2.3E+00)                                      |                  (+3.4E+00)  (+3.5E+01)  (+1.6E-01)  (+6.4E-01)\n",
                             "                                                        |                                                                \n",
-                            "prices   +1.3E+01    -8.8E-06                           |      prices       -9.4E+00    +1.6E+02    -1.4E+00    +1.9E+00 \n",
-                            "        (+7.7E+00)  (+2.3E+03)                          |                  (+3.2E+01)  (+2.0E+02)  (+7.8E-01)  (+8.8E+00)\n",
+                            "prices   +1.3E+01    +6.6E-06                           |      prices       -9.4E+00    +1.6E+02    -1.4E+00    +1.9E+00 \n",
+                            "        (+7.5E+00)  (+2.7E+03)                          |                  (+3.5E+01)  (+1.9E+02)  (+8.0E-01)  (+8.9E+00)\n",
                             "                                                        |                                                                \n",
-                            "sugar    -1.1E-01    +1.1E-07    -3.0E-09               |      sugar        +8.3E-02    -1.4E+00    +1.2E-02    -1.7E-02 \n",
-                            "        (+2.1E-01)  (+1.9E+05)  (+7.3E+02)              |                  (+1.7E-01)  (+7.8E-01)  (+2.1E-02)  (+1.5E-01)\n",
+                            "sugar    -1.1E-01    -7.4E-08    -8.9E-09               |      sugar        +8.3E-02    -1.4E+00    +1.2E-02    -1.7E-02 \n",
+                            "        (+2.0E-01)  (+2.2E+05)  (+5.2E+04)              |                  (+1.6E-01)  (+8.0E-01)  (+2.2E-02)  (+1.6E-01)\n",
                             "                                                        |                                                                \n",
-                            "mushy    +1.5E-01    +4.6E-07    +1.9E-08    -1.3E-08   |      mushy        -1.1E-01    +1.9E+00    -1.7E-02    +2.2E-02 \n",
-                            "        (+6.8E-01)  (+3.5E+03)  (+6.3E+02)  (+1.8E+02)  |                  (+6.3E-01)  (+8.8E+00)  (+1.5E-01)  (+2.0E-01)\n",
+                            "mushy    +1.5E-01    -4.3E-07    +1.6E-07    +4.7E-08   |      mushy        -1.1E-01    +1.9E+00    -1.7E-02    +2.2E-02 \n",
+                            "        (+6.8E-01)  (+5.0E+03)  (+7.0E+02)  (+4.3E+02)  |                  (+6.4E-01)  (+8.9E+00)  (+1.6E-01)  (+2.0E-01)\n",
                             "=========================================================================================================================\n",
                             "\n",
                             "Beta Estimates (Robust SEs in Parentheses):\n",
                             "==========\n",
                             "  prices  \n",
                             "----------\n",
                             " -3.1E+01 \n",
-                            "(+4.4E+00)\n",
+                            "(+4.0E+00)\n",
                             "=========="
                         ]
                     },
                     "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -705,15 +705,15 @@
                             "=======================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:00:23       Yes          16           24          19540        60462   \n",
+                            " 00:00:28       Yes          16           24          19529        60447   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs in Parentheses):\n",
                             "======================================================\n",
                             "Sigma:      1         prices      sugar       mushy   \n",
                             "------  ----------  ----------  ----------  ----------\n",
                             "  1      +5.2E-02                                     \n",
@@ -1017,23 +1017,23 @@
                     "data": {
                         "text/plain": [
                             "Problem Results Summary:\n",
                             "=======================================================================================================\n",
                             "GMM   Objective  Gradient      Hessian         Hessian     Clipped  Weighting Matrix  Covariance Matrix\n",
                             "Step    Value      Norm    Min Eigenvalue  Max Eigenvalue  Shares   Condition Number  Condition Number \n",
                             "----  ---------  --------  --------------  --------------  -------  ----------------  -----------------\n",
-                            " 1    +4.6E+00   +6.9E-06     +3.2E-05        +1.6E+04        0         +6.9E+07          +8.4E+08     \n",
+                            " 1    +4.6E+00   +6.9E-06     +3.3E-05        +1.6E+04        0         +6.9E+07          +8.4E+08     \n",
                             "=======================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:01:00       Yes          51           57          46386       143970   \n",
+                            " 00:01:12       Yes          51           57          46389       143977   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs in Parentheses):\n",
                             "=====================================================================================================================\n",
                             "Sigma:      1         prices      sugar       mushy     |   Pi:      income    income_squared     age        child   \n",
                             "------  ----------  ----------  ----------  ----------  |  ------  ----------  --------------  ----------  ----------\n",
                             "  1      +5.6E-01                                       |    1      +2.3E+00      +0.0E+00      +1.3E+00    +0.0E+00 \n",
@@ -1121,15 +1121,15 @@
                             "=======================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:00:45       Yes          34           40          34392       106492   \n",
+                            " 00:00:53       Yes          34           40          34390       106492   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs in Parentheses):\n",
                             "=====================================================================================================================\n",
                             "Sigma:      1         prices      sugar       mushy     |   Pi:      income    income_squared     age        child   \n",
                             "------  ----------  ----------  ----------  ----------  |  ------  ----------  --------------  ----------  ----------\n",
                             "  1      +3.7E-01                                       |    1      +3.1E+00      +0.0E+00      +1.2E+00    +0.0E+00 \n",
@@ -1194,15 +1194,15 @@
                             "=======================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:00:45       Yes          34           40          34403       106539   \n",
+                            " 00:00:55       Yes          34           40          34371       106443   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs in Parentheses):\n",
                             "=====================================================================================================\n",
                             "Sigma:      1         prices      sugar       mushy     |   Pi:      income       age        child   \n",
                             "------  ----------  ----------  ----------  ----------  |  ------  ----------  ----------  ----------\n",
                             "  1      +3.7E-01                                       |    1      +3.1E+00    +1.2E+00    +0.0E+00 \n",
```

### Comparing `pyblp-1.0.0/docs/notebooks/tutorial/petrin.ipynb` & `pyblp-1.1.0/docs/notebooks/tutorial/petrin.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998521013592292%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {1: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}, 16: {\'source\': '*

 * *            "{insert: [(2, 'By using $1 + J_t$ instead of $J_t$, we are specifying that the micro "*

 * *            'dataset contains observations of the outside option $j = 0$. If we instead specified '*

 * *            'a matrix of shape $I_t \\\\times J_t$, this would be the same as setting the first '*

 * *            "column equal to all zeros, so that outside choices are not sampled from.\\n')], "*

 * *            "delet […]*

```diff
@@ -25,15 +25,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -653,15 +653,15 @@
         {
             "cell_type": "markdown",
             "id": "2b95e675",
             "metadata": {},
             "source": [
                 "We called the dataset \"CEX\", defined the number of observations in it, and also defined a lambda function for computing survey weights in a market. The `compute_weights` function has three arguments: the current market's ID $t$, the $J_t$ :class:`Products` inside the market, and the $I_t$ :class:`Agents` inside the market. In this case, we are assuming that each product and agent/consumer type are sampled with equal probability, so we simply return a matrix of ones of shape $I_t \\times (1 + J_t)$. This sets each $w_{dijt} = 1$.\n",
                 "\n",
-                "By using $1 + J_t$ instead of $J_t$, we are specifying that the micro dataset contains observations of the outside option $j = 0$. If we instead specified a matrix of shape $I_t \\times (1 + J_t)$, this would be the same as setting the first column equal to all zeros, so that outside choices are not sampled from.\n",
+                "By using $1 + J_t$ instead of $J_t$, we are specifying that the micro dataset contains observations of the outside option $j = 0$. If we instead specified a matrix of shape $I_t \\times J_t$, this would be the same as setting the first column equal to all zeros, so that outside choices are not sampled from.\n",
                 "\n",
                 "We will be matching a few different statistics that were computed from this survey. For convenience, they are packaged in a data file with pyblp.\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
@@ -1057,23 +1057,23 @@
                     "data": {
                         "text/plain": [
                             "Problem Results Summary:\n",
                             "=======================================================================================================\n",
                             "GMM   Objective  Gradient      Hessian         Hessian     Clipped  Weighting Matrix  Covariance Matrix\n",
                             "Step    Value      Norm    Min Eigenvalue  Max Eigenvalue  Shares   Condition Number  Condition Number \n",
                             "----  ---------  --------  --------------  --------------  -------  ----------------  -----------------\n",
-                            " 2    +1.8E+02   +4.4E-05     +4.3E-01        +1.3E+03        0         +2.8E+11          +8.1E+07     \n",
+                            " 2    +1.8E+02   +4.3E-05     +3.8E-01        +1.3E+03        0         +2.8E+11          +8.1E+07     \n",
                             "=======================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:26:42       Yes          72           87          10899        33588   \n",
+                            " 00:34:10       Yes          72           87          10905        33592   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs Adjusted for 898 Clusters in Parentheses):\n",
                             "================================================================================================================================================================================================================================================\n",
                             "Sigma:       1       -prices      hpwt       space        air         mpd         fwd         mi        sw        su        pv     |    Pi:       1      low/income  mid/income  high/income  fv*log(fs)    age        fs       mid       high  \n",
                             "-------  ----------  --------  ----------  ----------  ----------  ----------  ----------  --------  --------  --------  --------  |  -------  --------  ----------  ----------  -----------  ----------  --------  --------  --------  --------\n",
                             "   1      +3.0E-02                                                                                                                 |     1     +0.0E+00   +0.0E+00    +0.0E+00    +0.0E+00     +0.0E+00   +0.0E+00  +0.0E+00  +0.0E+00  +0.0E+00\n",
@@ -1263,15 +1263,15 @@
             "execution_count": 19,
             "id": "b4d00395",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "array([[425.90823299]])"
+                            "array([[425.90824856]])"
                         ]
                     },
                     "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
```

### Comparing `pyblp-1.0.0/docs/notebooks/tutorial/post_estimation.ipynb` & `pyblp-1.1.0/docs/notebooks/tutorial/post_estimation.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999827226283909%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}, 5: {\'outputs\': '*

 * *            "{0: {'data': {'text/plain': {insert: [(5, ' 1    +4.6E+00   +6.9E-06     "*

 * *            "+3.3E-05        +1.6E+04        0         +6.9E+07          +8.4E+08     \\n'), (13, "*

 * *            "' 00:01:16       Yes          51           57          46389       143977   \\n')], "*

 * *            "delete: [13, 5]}}}}}, 37: {'outputs': {0: {'data': {'text/plain': {insert: [(5, ' "*

 * *            "00:00:09       […]*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -113,23 +113,23 @@
                     "data": {
                         "text/plain": [
                             "Problem Results Summary:\n",
                             "=======================================================================================================\n",
                             "GMM   Objective  Gradient      Hessian         Hessian     Clipped  Weighting Matrix  Covariance Matrix\n",
                             "Step    Value      Norm    Min Eigenvalue  Max Eigenvalue  Shares   Condition Number  Condition Number \n",
                             "----  ---------  --------  --------------  --------------  -------  ----------------  -----------------\n",
-                            " 1    +4.6E+00   +6.9E-06     +3.2E-05        +1.6E+04        0         +6.9E+07          +8.4E+08     \n",
+                            " 1    +4.6E+00   +6.9E-06     +3.3E-05        +1.6E+04        0         +6.9E+07          +8.4E+08     \n",
                             "=======================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:01:05       Yes          51           57          46386       143970   \n",
+                            " 00:01:16       Yes          51           57          46389       143977   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs in Parentheses):\n",
                             "=====================================================================================================================\n",
                             "Sigma:      1         prices      sugar       mushy     |   Pi:      income    income_squared     age        child   \n",
                             "------  ----------  ----------  ----------  ----------  |  ------  ----------  --------------  ----------  ----------\n",
                             "  1      +5.6E-01                                       |    1      +2.3E+00      +0.0E+00      +1.3E+00    +0.0E+00 \n",
@@ -605,15 +605,15 @@
                     "data": {
                         "text/plain": [
                             "Bootstrapped Results Summary:\n",
                             "======================\n",
                             "Computation  Bootstrap\n",
                             "   Time        Draws  \n",
                             "-----------  ---------\n",
-                            " 00:00:08       100   \n",
+                            " 00:00:09       100   \n",
                             "======================"
                         ]
                     },
                     "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -823,15 +823,15 @@
                             "=======================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:01:03       Yes          42           50          45892       142159   \n",
+                            " 00:01:05       Yes          42           50          45902       142164   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs in Parentheses):\n",
                             "=====================================================================================================================\n",
                             "Sigma:      1         prices      sugar       mushy     |   Pi:      income    income_squared     age        child   \n",
                             "------  ----------  ----------  ----------  ----------  |  ------  ----------  --------------  ----------  ----------\n",
                             "  1      +2.1E-01                                       |    1      +6.0E+00      +0.0E+00      +1.6E-01    +0.0E+00 \n",
@@ -1446,23 +1446,23 @@
                     "data": {
                         "text/plain": [
                             "Problem Results Summary:\n",
                             "=======================================================================================================\n",
                             "GMM   Objective  Gradient      Hessian         Hessian     Clipped  Weighting Matrix  Covariance Matrix\n",
                             "Step    Value      Norm    Min Eigenvalue  Max Eigenvalue  Shares   Condition Number  Condition Number \n",
                             "----  ---------  --------  --------------  --------------  -------  ----------------  -----------------\n",
-                            " 1    +1.1E+02   +3.8E-06     +3.0E-03        +8.3E+04        0         +2.2E+08          +4.1E+07     \n",
+                            " 1    +1.1E+02   +8.8E-06     +2.3E-03        +8.3E+04        0         +2.2E+08          +4.1E+07     \n",
                             "=======================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:00:59       Yes          34           42          33337       103774   \n",
+                            " 00:01:26       Yes          34           55          42977       133908   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs in Parentheses):\n",
                             "=====================================================================================================================\n",
                             "Sigma:      1         prices      sugar       mushy     |   Pi:      income    income_squared     age        child   \n",
                             "------  ----------  ----------  ----------  ----------  |  ------  ----------  --------------  ----------  ----------\n",
                             "  1      +4.6E-01                                       |    1      +4.8E+00      +0.0E+00      +6.5E-01    +0.0E+00 \n",
```

### Comparing `pyblp-1.0.0/docs/notebooks/tutorial/simulation.ipynb` & `pyblp-1.1.0/docs/notebooks/tutorial/simulation.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999568256578948%*

 * *Differences: {"'cells'": '{1: {\'outputs\': {0: {\'data\': {\'text/plain\': ["\'1.1.0\'"]}}}}, 13: '*

 * *            "{'outputs': {0: {'data': {'text/plain': {insert: [(13, ' 00:00:16       Yes          "*

 * *            "23           30          8295         26312   \\n')], delete: [13]}}}}}}"}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'1.0.0'"
+                            "'1.1.0'"
                         ]
                     },
                     "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -265,15 +265,15 @@
                             "==============================================================================================================\n",
                             "\n",
                             "Cumulative Statistics:\n",
                             "===========================================================================\n",
                             "Computation  Optimizer  Optimization   Objective   Fixed Point  Contraction\n",
                             "   Time      Converged   Iterations   Evaluations  Iterations   Evaluations\n",
                             "-----------  ---------  ------------  -----------  -----------  -----------\n",
-                            " 00:00:13       Yes          23           30          8295         26314   \n",
+                            " 00:00:16       Yes          23           30          8295         26312   \n",
                             "===========================================================================\n",
                             "\n",
                             "Nonlinear Coefficient Estimates (Robust SEs in Parentheses):\n",
                             "==================\n",
                             "Sigma:      x     \n",
                             "------  ----------\n",
                             "  x      +7.8E-01 \n",
```

### Comparing `pyblp-1.0.0/docs/references.rst` & `pyblp-1.1.0/docs/references.rst`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,20 @@
 
 Lovell (1963)
 ~~~~~~~~~~~~~
 
 Lovell, Michael C. (1963). `Seasonal adjustment of economic time series and multiple regression analysis <https://www.tandfonline.com/doi/abs/10.1080/01621459.1963.10480682>`_. *Journal of the American Statistical Association, 58* (304), 993-1010.
 
 
+MacKay and Miller (2023)
+~~~~~~~~~~~~~~~~~~~~~~~~
+
+MacKay, Alexander and Nathan Miller (2023). `Estimating models of supply and demand: Instruments and covariance restrictions <https://www.hbs.edu/faculty/Pages/item.aspx?num=55227>`_. HBS working paper 19-051.
+
+
 Morrow and Skerlos (2011)
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Morrow, W. Ross, and Steven J. Skerlos (2011). `Fixed-point approaches to computing Bertrand-Nash equilibrium prices under mixed-logit demand <https://ideas.repec.org/a/inm/oropre/v59y2011i2p328-345.html>`_. *Operations Research, 59* (2), 328-345.
 
 
 Nevo (2000a)
```

### Comparing `pyblp-1.0.0/docs/static/override.css` & `pyblp-1.1.0/docs/static/override.css`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/docs/testing.rst` & `pyblp-1.1.0/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/docs/tutorial.rst` & `pyblp-1.1.0/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/docs/versions.rst` & `pyblp-1.1.0/docs/versions.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Version Notes
 =============
 
 These notes will only include major changes.
 
 
+1.1
+---
+- Covariance restrictions
+- Demographic-specific product availability
+
+
 1.0
 ---
 
 - Support matching smooth functions of micro means
 - Optimal micro moments
 - Support elimination of groups of products for second choices
 - Micro data simulation
```

### Comparing `pyblp-1.0.0/LICENSE.txt` & `pyblp-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/PKG-INFO` & `pyblp-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyblp
-Version: 1.0.0
+Version: 1.1.0
 Summary: BLP demand estimation with Python 3
 Home-page: https://github.com/jeffgortmaker/pyblp
 Author: Jeff Gortmaker, Christopher Conlon
 Author-email: jeff@jeffgortmaker.com
 License: MIT
 Project-URL: Documentation, http://pyblp.readthedocs.io/en/latest
 Project-URL: Tracker, https://github.com/jeffgortmaker/pyblp/issues
@@ -118,14 +118,15 @@
 --------
 
 - R-style formula interface
 - Bertrand-Nash supply-side moments
 - Multiple equation GMM
 - Demographic interactions
 - Product-specific demographics
+- Consumer-specific product availability
 - Flexible micro moments that can match statistics based on survey data
 - Support for micro moments based on second choice data
 - Support for optimal micro moments that match micro data scores
 - Fixed effect absorption
 - Nonlinear functions of product characteristics
 - Concentrating out linear parameters
 - Flexible random coefficient distributions
@@ -133,14 +134,15 @@
 - Random coefficients nested logit (RCNL)
 - Approximation to the pure characteristics model
 - Varying nesting parameters across groups
 - Logit and nested logit benchmarks
 - Classic BLP instruments
 - Differentiation instruments
 - Optimal instruments
+- Covariance restrictions
 - Adjustments for simulation error
 - Tests of overidentifying and model restrictions
 - Parametric boostrapping post-estimation outputs
 - Elasticities and diversion ratios
 - Marginal costs and markups
 - Passthrough calculations
 - Profits and consumer surplus
```

### Comparing `pyblp-1.0.0/pyblp/configurations/formulation.py` & `pyblp-1.1.0/pyblp/configurations/formulation.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/configurations/integration.py` & `pyblp-1.1.0/pyblp/configurations/integration.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/configurations/iteration.py` & `pyblp-1.1.0/pyblp/configurations/iteration.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/configurations/optimization.py` & `pyblp-1.1.0/pyblp/configurations/optimization.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/construction.py` & `pyblp-1.1.0/pyblp/construction.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/data/blp_agents.csv` & `pyblp-1.1.0/pyblp/data/blp_agents.csv`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/data/blp_products.csv` & `pyblp-1.1.0/pyblp/data/blp_products.csv`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/data/nevo_agents.csv` & `pyblp-1.1.0/pyblp/data/nevo_agents.csv`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/data/nevo_products.csv` & `pyblp-1.1.0/pyblp/data/nevo_products.csv`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/data/petrin_agents.csv` & `pyblp-1.1.0/pyblp/data/petrin_agents.csv`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/data/petrin_covariances.csv` & `pyblp-1.1.0/pyblp/data/petrin_covariances.csv`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/data/petrin_products.csv` & `pyblp-1.1.0/pyblp/data/petrin_products.csv`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/data/__init__.py` & `pyblp-1.1.0/pyblp/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/economies/economy.py` & `pyblp-1.1.0/pyblp/economies/economy.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     I: int
     K1: int
     K2: int
     K3: int
     D: int
     MD: int
     MS: int
+    MC: int
     ED: int
     ES: int
     H: int
     _market_indices: Dict[Hashable, int]
     _product_market_indices: Dict[Hashable, Array]
     _agent_market_indices: Dict[Hashable, Array]
     _max_J: int
@@ -76,14 +77,15 @@
         self.I = self.agents.shape[0] if self.products.X2.shape[1] > 0 else 0
         self.K1 = self.products.X1.shape[1]
         self.K2 = self.products.X2.shape[1]
         self.K3 = self.products.X3.shape[1]
         self.D = self.agents.demographics.shape[1]
         self.MD = self.products.ZD.shape[1]
         self.MS = self.products.ZS.shape[1]
+        self.MC = self.products.ZC.shape[1]
         self.ED = self.products.demand_ids.shape[1]
         self.ES = self.products.supply_ids.shape[1]
         self.H = self.unique_nesting_ids.size
 
         # identify market indices
         self._market_indices = {t: i for i, t in enumerate(self.unique_market_ids)}
         self._product_market_indices = get_indices(self.products.market_ids)
@@ -130,15 +132,15 @@
         """Format economy information as a string."""
         return "\n\n".join([self._format_dimensions(), self._format_formulations()])
 
     def _format_dimensions(self) -> str:
         """Format information about the nonzero dimensions of the economy as a string."""
         header: List[str] = []
         values: List[str] = []
-        for key in ['T', 'N', 'F', 'I', 'K1', 'K2', 'K3', 'D', 'MD', 'MS', 'ED', 'ES', 'H']:
+        for key in ['T', 'N', 'F', 'I', 'K1', 'K2', 'K3', 'D', 'MD', 'MS', 'MC', 'ED', 'ES', 'H']:
             value = getattr(self, key)
             if value > 0:
                 header.append(f" {key} ")
                 values.append(str(value))
 
         return format_table(header, values, title="Dimensions")
 
@@ -176,15 +178,16 @@
             'X2': [str(f) for f in self._X2_formulations],
             'X3': [str(f) for f in self._X3_formulations],
             'ZD': [str(f) for f in self._X1_formulations if 'prices' not in f.names] if added_exogenous else [],
             'ZS': [str(f) for f in self._X3_formulations if 'shares' not in f.names] if added_exogenous else [],
         }
         matrix_labels.update({
             'ZD': [f'demand_instruments{i}' for i in range(self.MD - len(matrix_labels['ZD']))] + matrix_labels['ZD'],
-            'ZS': [f'demand_instruments{i}' for i in range(self.MS - len(matrix_labels['ZS']))] + matrix_labels['ZS']
+            'ZS': [f'supply_instruments{i}' for i in range(self.MS - len(matrix_labels['ZS']))] + matrix_labels['ZS'],
+            'ZC': [f'covariance_instruments{i}' for i in range(self.MC)],
         })
 
         # check each matrix for collinearity
         for name, labels in matrix_labels.items():
             collinear, successful = precisely_identify_collinearity(self.products[name])
             common_message = "To disable collinearity checks, set options.collinear_atol = options.collinear_rtol = 0."
             if (self.ED > 0 and name in {'X1', 'ZD'}) or (self.ES > 0 and name in {'X3', 'ZS'}):
```

### Comparing `pyblp-1.0.0/pyblp/economies/problem.py` & `pyblp-1.1.0/pyblp/economies/problem.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,17 +47,17 @@
             beta_bounds: Optional[Tuple[Any, Any]] = None, gamma_bounds: Optional[Tuple[Any, Any]] = None,
             delta: Optional[Any] = None, method: str = '2s', initial_update: Optional[bool] = None,
             optimization: Optional[Optimization] = None, scale_objective: bool = True, check_optimality: str = 'both',
             finite_differences: bool = False, error_behavior: str = 'revert', error_punishment: float = 1,
             delta_behavior: str = 'first', iteration: Optional[Iteration] = None, fp_type: str = 'safe_linear',
             shares_bounds: Optional[Tuple[Any, Any]] = (1e-300, None), costs_bounds: Optional[Tuple[Any, Any]] = None,
             W: Optional[Any] = None, center_moments: bool = True, W_type: str = 'robust', se_type: str = 'robust',
-            micro_moments: Sequence[MicroMoment] = (), micro_sample_covariances: Optional[Any] = None,
-            resample_agent_data: Optional[Callable[[int], Optional[Mapping]]] = None) -> (
-            ProblemResults):
+            covariance_moments_mean: float = 0, micro_moments: Sequence[MicroMoment] = (),
+            micro_sample_covariances: Optional[Any] = None,
+            resample_agent_data: Optional[Callable[[int], Optional[Mapping]]] = None) -> ProblemResults:
         r"""Solve the problem.
 
         The problem is solved in one or more GMM steps. During each step, any parameters in :math:`\theta` are optimized
         to minimize the GMM objective value, giving the estimated :math:`\hat{\theta}`. If there are no parameters in
         :math:`\theta` (for example, in the logit model there are no nonlinear parameters and all linear parameters can
         be concentrated out), the objective is evaluated once during the step.
 
@@ -417,14 +417,19 @@
                   computed under the assumption that the weighting matrix is optimal.
 
             This only affects the standard demand- and supply-side block of the matrix of averaged moment covariances.
             If there are micro moments, the :math:`S` matrix defined in the expressions referenced above will be
             block-diagonal with a micro moment block equal to the scaled covariance matrix defined in
             :eq:`scaled_micro_moment_covariances`.
 
+        covariance_moments_mean : `float, optional`
+            If ``covariance_instruments`` were specified in ``product_data``, this can be used to choose a
+            :math:`m \neq 0` in covariance moments :math:`E[g_{C,jt}] = E[(\xi_{jt}\omega_{jt} - m)Z_{C,jt}] = 0` where
+            :math:`m` is by default zero. This can be used for sensitivity testing to see how different covariances
+            may affect estimates.
         micro_moments : `sequence of MicroMoment, optional`
             Configurations for the :math:`M_M` :class:`MicroMoment` instances that will be added to the standard set of
             moments. By default, no micro moments are used, so :math:`M_M = 0`.
 
             When micro moments are specified, unless an initial weighting matrix ``W`` is specified as well (with a
             lower right micro moment block that reflects micro moment covariances), an ``initial_update`` will be used
             to update starting values :math:`W` and the mean utility :math:`\delta` at the initial parameter values
@@ -494,14 +499,16 @@
         if se_type not in {'robust', 'unadjusted', 'clustered'}:
             raise ValueError("se_type must be 'robust', 'unadjusted', or 'clustered'.")
         if 'clustered' in {W_type, se_type}:
             if 'clustering_ids' not in self.products.dtype.names or self.products.clustering_ids.size == 0:
                 raise ValueError(
                     "W_type or se_type is 'clustered' but clustering_ids were not specified in product_data."
                 )
+        if not isinstance(covariance_moments_mean, (int, float)):
+            raise ValueError("covariance_moments_mean must be a float.")
 
         # configure or validate bounds on shares and costs
         shares_bounds = self._coerce_optional_bounds(shares_bounds, 'shares_bounds')
         costs_bounds = self._coerce_optional_bounds(costs_bounds, 'costs_bounds')
 
         # validate and structure micro moments before outputting related information
         moments = Moments(micro_moments, self)
@@ -546,26 +553,37 @@
             if parameters.fixed or optimization._supports_bounds:
                 output("")
                 output(parameters.format_lower_bounds("Lower Bounds"))
                 output("")
                 output(parameters.format_upper_bounds("Upper Bounds"))
                 output("")
 
+        # warn if it seems like the model is under-identified
+        M = self.MD + self.MS + self.MC + moments.MM
+        P_total = len(parameters.unfixed) + len(parameters.eliminated)
+        if P_total > M:
+            warn(
+                f"The model may be under-identified. The total number of unfixed parameters is {P_total}, which is "
+                f"more than the total number of moments, {M}. Consider checking whether instruments were properly "
+                f"specified when initializing the problem, and whether parameters were properly configured when "
+                f"solving the problem."
+            )
+
         # load or compute the weighting matrix
         if W is not None:
             W = np.c_[np.asarray(W, options.dtype)]
-            M = self.MD + self.MS + moments.MM
             if W.shape != (M, M):
                 raise ValueError(f"W must be a square {M} by {M} matrix.")
             self._require_psd(W, "W")
             self._detect_singularity(W, "W")
         else:
             S = scipy.linalg.block_diag(
                 self.products.ZD.T @ self.products.ZD / self.N,
                 self.products.ZS.T @ self.products.ZS / self.N,
+                self.products.ZC.T @ self.products.ZC / self.N,
             )
             self._detect_singularity(S, "the 2SLS weighting matrix")
             W, successful = precisely_invert(S)
             if not successful:
                 raise ValueError("Failed to compute the 2SLS weighting matrix. There may be instrument collinearity.")
 
             # an initial update will be used when there are micro moments, so this initial block does not matter
@@ -621,15 +639,16 @@
             # initialize an IV model for linear parameter estimation
             iv = IV(X_list, Z_list, W[:self.MD + self.MS, :self.MD + self.MS])
             self._handle_errors(iv.errors, error_behavior)
 
             # wrap computation of progress information with step-specific information
             compute_step_progress = functools.partial(
                 self._compute_progress, parameters, moments, iv, W, scale_objective, error_behavior, error_punishment,
-                delta_behavior, iteration, fp_type, shares_bounds, costs_bounds, finite_differences, resample_agent_data
+                delta_behavior, iteration, fp_type, shares_bounds, costs_bounds, finite_differences,
+                covariance_moments_mean, resample_agent_data
             )
 
             # initialize optimization progress
             iteration_stats: List[Dict[Hashable, SolverStats]] = []
             smallest_objective = np.inf
             progress = InitialProgress(
                 self, parameters, moments, W, theta, objective, gradient, hessian, delta, delta, tilde_costs, micro,
@@ -699,15 +718,15 @@
             )
             iteration_stats.append(final_progress.iteration_stats)
             optimization_stats.evaluations += 1
             detect_micro_collinearity = False
             results = ProblemResults(
                 final_progress, last_results, step, last_step, step_start_time, optimization_start_time,
                 optimization_end_time, optimization_stats, iteration_stats, scale_objective, shares_bounds,
-                costs_bounds, micro_moment_covariances, center_moments, W_type, se_type
+                costs_bounds, micro_moment_covariances, center_moments, W_type, se_type, covariance_moments_mean
             )
             self._handle_errors(results._errors, error_behavior)
             output(f"Computed results after {format_seconds(results.total_time - results.optimization_time)}.")
 
             # store the last results and return results from the final step
             last_results = results
             output("")
@@ -726,15 +745,15 @@
             W = results.updated_W
             step += 1
             step_start_time = time.time()
 
     def _compute_progress(
             self, parameters: Parameters, moments: Moments, iv: IV, W: Array, scale_objective: bool,
             error_behavior: str, error_punishment: float, delta_behavior: str, iteration: Iteration, fp_type: str,
-            shares_bounds: Bounds, costs_bounds: Bounds, finite_differences: bool,
+            shares_bounds: Bounds, costs_bounds: Bounds, finite_differences: bool, covariance_moments_mean: float,
             resample_agent_data: Optional[Callable[[int], Optional[Mapping]]], theta: Array,
             progress: 'InitialProgress', compute_gradient: bool, compute_hessian: bool,
             compute_micro_covariances: bool, detect_micro_collinearity: bool,
             compute_simulation_covariances: bool, agents_override: Optional[RecArray] = None) -> 'Progress':
         """Compute demand- and supply-side contributions before recovering the linear parameters and structural error
         terms. Then, form the GMM objective value and its gradient. Finally, handle any errors that were encountered
         before structuring relevant progress information.
@@ -1010,18 +1029,18 @@
 
         # optionally compute Jacobians with central finite differences
         if compute_gradient and finite_differences and parameters.P > 0:
             def compute_perturbed_stack(perturbed_theta: Array) -> Array:
                 """Evaluate a stack of xi, micro moments, and omega at a perturbed parameter vector."""
                 perturbed_progress = self._compute_progress(
                     parameters, moments, iv, W, scale_objective, error_behavior, error_punishment, delta_behavior,
-                    iteration, fp_type, shares_bounds, costs_bounds, finite_differences=False, resample_agent_data=None,
-                    theta=perturbed_theta, progress=progress, compute_gradient=False, compute_hessian=False,
-                    compute_micro_covariances=False, detect_micro_collinearity=False,
-                    compute_simulation_covariances=False,
+                    iteration, fp_type, shares_bounds, costs_bounds, finite_differences=False,
+                    covariance_moments_mean=covariance_moments_mean, resample_agent_data=None, theta=perturbed_theta,
+                    progress=progress, compute_gradient=False, compute_hessian=False, compute_micro_covariances=False,
+                    detect_micro_collinearity=False, compute_simulation_covariances=False,
                 )
                 perturbed_stack = perturbed_progress.iv_delta
                 if moments.MM > 0:
                     perturbed_stack = np.r_[perturbed_stack, perturbed_progress.micro]
                 if self.K3 > 0:
                     perturbed_stack = np.r_[perturbed_stack, perturbed_progress.iv_tilde_costs]
                 return perturbed_stack
@@ -1040,57 +1059,75 @@
         if not parameters.eliminated_beta_index.all():
             theta_beta = np.c_[beta[~parameters.eliminated_beta_index]]
             iv_delta -= self._compute_true_X1(index=~parameters.eliminated_beta_index.flatten()) @ theta_beta
         if not parameters.eliminated_gamma_index.all():
             theta_gamma = np.c_[gamma[~parameters.eliminated_gamma_index]]
             iv_tilde_costs -= self._compute_true_X3(index=~parameters.eliminated_gamma_index.flatten()) @ theta_gamma
 
+        # check whether delta and tilde cost Jacobians need to be explicitly converted into xi and omega Jacobians to
+        #   account for concentrating out linear parameters (without covariance moments, it turns out that convenient
+        #   orthogonality conditions makes this unnecessary, which cuts down significantly on additional computation)
+        convert_jacobians = self.MC > 0 and (compute_gradient or finite_differences) and parameters.P > 0
+
         # absorb any fixed effects
         if self._absorb_demand_ids is not None:
             iv_delta, demand_absorption_errors = self._absorb_demand_ids(iv_delta)
             errors.extend(demand_absorption_errors)
+            if convert_jacobians:
+                xi_jacobian, demand_jacobian_absorption_errors = self._absorb_demand_ids(xi_jacobian)
+                errors.extend(demand_jacobian_absorption_errors)
         if self._absorb_supply_ids is not None:
             iv_tilde_costs, supply_absorption_errors = self._absorb_supply_ids(iv_tilde_costs)
             errors.extend(supply_absorption_errors)
+            if convert_jacobians:
+                omega_jacobian, supply_jacobian_absorption_errors = self._absorb_supply_ids(omega_jacobian)
+                errors.extend(supply_jacobian_absorption_errors)
 
         # collect inputs into GMM estimation
         X_list = [self.products.X1[:, parameters.eliminated_beta_index.flat]]
         Z_list = [self.products.ZD]
         y_list = [iv_delta]
         jacobian_list = [xi_jacobian]
         if self.K3 > 0:
             X_list.append(self.products.X3[:, parameters.eliminated_gamma_index.flat])
             Z_list.append(self.products.ZS)
             y_list.append(iv_tilde_costs)
             jacobian_list.append(omega_jacobian)
 
         # recover the linear parameters and structural error terms
-        parameters_list, u_list = iv.estimate(X_list, Z_list, W[:self.MD + self.MS, :self.MD + self.MS], y_list)
+        parameters_list, u_list, jacobian_list = iv.estimate(
+            X_list, Z_list, W[:self.MD + self.MS, :self.MD + self.MS], y_list, jacobian_list, convert_jacobians
+        )
         beta[parameters.eliminated_beta_index] = parameters_list[0].flat
-        xi = u_list[0]
         if self.K3 == 0:
+            xi = u_list[0]
             omega = np.full((self.N, 0), np.nan, options.dtype)
+            xi_jacobian = jacobian_list[0]
         else:
             gamma[parameters.eliminated_gamma_index] = parameters_list[1].flat
-            omega = u_list[1]
+            xi, omega = u_list
+            xi_jacobian, omega_jacobian = jacobian_list
+
+            # add any covariance moments
+            if self.MC > 0:
+                u_list.append(xi * omega - covariance_moments_mean)
+                Z_list.append(self.products.ZC)
+                jacobian_list.append(xi_jacobian * omega + xi * omega_jacobian)
 
         # compute the objective value and replace it with its last value if computation failed
         with np.errstate(all='ignore'):
             mean_g = np.r_[compute_gmm_moments_mean(u_list, Z_list), micro]
             objective = mean_g.T @ W @ mean_g
             if scale_objective:
                 objective *= self.N
         if not np.isfinite(np.squeeze(objective)):
             objective = progress.objective
             errors.append(exceptions.ObjectiveReversionError())
 
-        # compute the gradient and replace any invalid elements with their last values (even if we concentrate out
-        #   linear parameters, it turns out that one can use orthogonality conditions to show that treating the linear
-        #   parameters as fixed is fine, so that we can treat xi and omega Jacobians as equal to delta and transformed
-        #   marginal cost Jacobians when computing the gradient)
+        # compute the gradient and replace any invalid elements with their last values
         gradient = np.full_like(progress.gradient, np.nan)
         if compute_gradient:
             with np.errstate(all='ignore'):
                 mean_G = np.r_[compute_gmm_moments_jacobian_mean(jacobian_list, Z_list), micro_jacobian]
                 gradient = 2 * (mean_G.T @ W @ mean_g)
                 if scale_objective:
                     gradient *= self.N
@@ -1120,16 +1157,16 @@
         # optionally compute the Hessian with central finite differences
         hessian = np.full_like(progress.hessian, np.nan)
         if compute_hessian:
             def compute_perturbed_gradient(perturbed_theta: Array) -> Array:
                 """Evaluate the gradient at a perturbed parameter vector."""
                 perturbed_progress = self._compute_progress(
                     parameters, moments, iv, W, scale_objective, error_behavior, error_punishment, delta_behavior,
-                    iteration, fp_type, shares_bounds, costs_bounds, finite_differences, resample_agent_data,
-                    perturbed_theta, progress, compute_gradient=True, compute_hessian=False,
+                    iteration, fp_type, shares_bounds, costs_bounds, finite_differences, covariance_moments_mean,
+                    resample_agent_data, perturbed_theta, progress, compute_gradient=True, compute_hessian=False,
                     compute_micro_covariances=False, detect_micro_collinearity=False,
                     compute_simulation_covariances=False,
                 )
                 return perturbed_progress.gradient
 
             # compute the Hessian, enforcing shape and symmetry
             hessian = compute_finite_differences(compute_perturbed_gradient, theta)
@@ -1150,18 +1187,18 @@
                 try:
                     resampled_agents = Agents(self.products, self.agent_formulation, resampled_agent_data)
                 except Exception as exception:
                     raise RuntimeError("Failed to use resampled agents because of the above exception.") from exception
 
                 resampled_progress = self._compute_progress(
                     parameters, moments, iv, W, scale_objective, error_behavior, error_punishment, delta_behavior,
-                    iteration, fp_type, shares_bounds, costs_bounds, finite_differences, resample_agent_data, theta,
-                    progress, compute_gradient=False, compute_hessian=False, compute_micro_covariances=False,
-                    detect_micro_collinearity=False, compute_simulation_covariances=False,
-                    agents_override=resampled_agents,
+                    iteration, fp_type, shares_bounds, costs_bounds, finite_differences, covariance_moments_mean,
+                    resample_agent_data, theta, progress, compute_gradient=False, compute_hessian=False,
+                    compute_micro_covariances=False, detect_micro_collinearity=False,
+                    compute_simulation_covariances=False, agents_override=resampled_agents,
                 )
                 mean_g_samples.append(resampled_progress.mean_g.flatten())
 
             if len(mean_g_samples) < 2:
                 raise ValueError(
                     "There must be at least 2 resampled sets of agent data to estimate the contribution of simulation "
                     "error to moment covariances."
@@ -1244,14 +1281,42 @@
               ``add_exogenous`` to ``False``.
 
             - **supply_instruments** : (`numeric, optional`) - Excluded supply-side instruments, which, together with
               the formulated exogenous supply-side characteristics, :math:`X_3^\text{ex}`, constitute the full set of
               supply-side instruments, :math:`Z_S`. To instead specify the full matrix :math:`Z_S`, set
               ``add_exogenous`` to ``False``.
 
+            - **covariance_instruments** : (`numeric, optional`) - Covariance instruments :math:`Z_C`. If specified,
+              additional moments :math:`E[g_{C,jt}] = E[\xi_{jt}\omega_{jt}Z_{C,jt}] = 0` will be added, as in
+              :ref:`references:MacKay and Miller (2023)`.
+
+              If any fixed effects are absorbed, :math:`\xi_{jt}` and :math:`\omega_{jt}` in these new covariance
+              moments are replaced with :math:`\Delta\xi_{jt}` and/or :math:`\Delta\omega_{jt}` in :eq:`fe`. The default
+              2SLS weighting matrix will have an additional :math:`(Z_C'Z_C / N)^{-1}` block after the first two.
+
+              .. warning::
+
+                 Covariance restrictions are still an experimental feature. The way in which they are implemented and
+                 used may change somewhat in future releases.
+
+              .. note::
+
+                 Using covariance restrictions to identify a parameter on price can sometimes yield two solutions, where
+                 the "upper" solution may be positive (i.e., implying upward-sloping demand). See
+                 :ref:`references:MacKay and Miller (2023)` for more discussion of this point. In these cases when the
+                 "lower" root is the correct solution, consider bounding the parameter on price from below using
+                 ``beta_bounds`` (if the parameter is in ``beta``) or replacing it with a lognormal coefficient on
+                 price via the ``rc_type`` argument to :class:`Problem`.
+
+              .. note::
+
+                 In the current implementation, these covariance restrictions only affect the nonlinear parameters. The
+                 linear parameters are estimated using other moments. In the case of overidentification, the estimator
+                 may not be fully efficient because of this implementation decision.
+
         The recommendation in :ref:`references:Conlon and Gortmaker (2020)` is to start with differentiation instruments
         of :ref:`references:Gandhi and Houde (2017)`, which can be built with :func:`build_differentiation_instruments`,
         and then compute feasible optimal instruments with :func:`ProblemResults.compute_optimal_instruments` in the
         second stage.
 
         For guidance on how to construct instruments and add them to product data, refer to the examples in the
         documentation for the :func:`build_blp_instruments` and :func:`build_differentiation_instruments` functions.
@@ -1330,26 +1395,45 @@
 
         It may be convenient to define IDs for different agents:
 
             - **agent_ids** (`object, optional`) - IDs that identify agents within markets. There can be multiple of the
               same ID within a market.
 
         Along with ``market_ids`` and ``agent_ids``, the names of any additional fields can be typically be used as
-        variables in ``agent_formulation``. The exception is the name ``'demographics'``, which is reserved for use by
-        :class:`Agents`.
+        variables in ``agent_formulation``. Exceptions are the names ``'demographics'`` and ``'availability'``, which
+        are reserved for use by :class:`Agents`.
 
         In addition to standard demographic variables :math:`d_{it}`, it is also possible to specify product-specific
         demographics :math:`d_{ijt}`. A typical example is geographic distance of agent :math:`i` from product
         :math:`j`. If ``agent_formulation`` has, for example, ``'distance'``, instead of including a single
         ``'distance'`` field in ``agent_data``, one should instead include ``'distance0'``, ``'distance1'``,
         ``'distance2'`` and so on, where the index corresponds to the order in which products appear within market in
         ``product_data``. For example, ``'distance5'`` should measure the distance of agents to the fifth product within
         the market, as ordered in ``product_data``. The last index should be the number of products in the largest
         market, minus one. For markets with fewer products than this maximum number, latter columns will be ignored.
 
+        Finally, by default each agent :math:`i` in market :math:`t` is faced with the same choice set of product
+        :math:`j`, but it is possible to specify agent-specific availability :math:`a_{ijt}` much in the same way that
+        product-specific demographics are specified. To do so, the following field can be specified:
+
+            - **availability** : (`numeric, optional`) - Agent-specific product availability, :math:`a`. Choice
+              probabilities in :eq:`probabilities` are modified according to
+
+              .. math:: s_{ijt} = \frac{a_{ijt} \exp V_{ijt}}{1 + \sum_{k \in J_t} a_{ijt} \exp V_{ikt}},
+
+              and similarly for the nested logit model and consumer surplus calculations. By default, all
+              :math:`a_{ijt} = 1`. To have a product :math:`j` be unavailable to agent :math:`i`, set
+              :math:`a_{ijt} = 0`.
+
+              Agent-specific availability is specified in the same way that product-specific demographics are specified.
+              In ``agent_data``, one can include ``'availability0'``, ``'availability1'``, ``'availability2'``, and so
+              on, where the index corresponds to the order in which products appear within market in ``product_data``.
+              The last index should be the number of products in the largest market, minus one. For markets with fewer
+              products than this maximum number, latter columns will be ignored.
+
     integration : `Integration, optional`
         :class:`Integration` configuration for how to build nodes and weights for integration over agent choice
         probabilities, which will replace any ``nodes`` and ``weights`` fields in ``agent_data``. This configuration is
         required if ``nodes`` and ``weights`` in ``agent_data`` are not specified. It should not be specified if
         :math:`X_2` is not formulated in ``product_formulations``.
 
         If this configuration is specified, :math:`K_2` columns of nodes (the number of demand-side nonlinear product
@@ -1486,14 +1570,16 @@
         Number of demographic variables, :math:`D`.
     MD : `int`
         Number of demand-side instruments, :math:`M_D`, which is typically the number of excluded demand-side
         instruments plus the number of exogenous demand-side linear product characteristics, :math:`K_1^\text{ex}`.
     MS : `int`
         Number of supply-side instruments, :math:`M_S`, which is typically the number of excluded supply-side
         instruments plus the number of exogenous supply-side linear product characteristics, :math:`K_3^\text{ex}`.
+    MC : `int`
+        Number of covariance instruments, :math:`M_C`.
     ED : `int`
         Number of absorbed dimensions of demand-side fixed effects, :math:`E_D`.
     ES : `int`
         Number of absorbed dimensions of supply-side fixed effects, :math:`E_S`.
     H : `int`
         Number of nesting groups, :math:`H`.
```

### Comparing `pyblp-1.0.0/pyblp/economies/simulation.py` & `pyblp-1.1.0/pyblp/economies/simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,33 @@
         :math:`j`. If ``agent_formulation`` has, for example, ``'distance'``, instead of including a single
         ``'distance'`` field in ``agent_data``, one should instead include ``'distance0'``, ``'distance1'``,
         ``'distance2'`` and so on, where the index corresponds to the order in which products appear within market in
         ``product_data``. For example, ``'distance5'`` should measure the distance of agents to the fifth product within
         the market, as ordered in ``product_data``. The last index should be the number of products in the largest
         market, minus one. For markets with fewer products than this maximum number, latter columns will be ignored.
 
+        Finally, by default each agent :math:`i` in market :math:`t` is faced with the same choice set of product
+        :math:`j`, but it is possible to specify agent-specific availability :math:`a_{ijt}` much in the same way that
+        product-specific demographics are specified. To do so, the following field can be specified:
+
+            - **availability** : (`numeric, optional`) - Agent-specific product availability, :math:`a`. Choice
+              probabilities in :eq:`probabilities` are modified according to
+
+              .. math:: s_{ijt} = \frac{a_{ijt} \exp V_{ijt}}{1 + \sum_{k \in J_t} a_{ijt} \exp V_{ikt}},
+
+              and similarly for the nested logit model and consumer surplus calculations. By default, all
+              :math:`a_{ijt} = 1`. To have a product :math:`j` be unavailable to agent :math:`i`, set
+              :math:`a_{ijt} = 0`.
+
+              Agent-specific availability is specified in the same way that product-specific demographics are specified.
+              In ``agent_data``, one can include ``'availability0'``, ``'availability1'``, ``'availability2'``, and so
+              on, where the index corresponds to the order in which products appear within market in ``product_data``.
+              The last index should be the number of products in the largest market, minus one. For markets with fewer
+              products than this maximum number, latter columns will be ignored.
+
     integration : `Integration, optional`
         :class:`Integration` configuration for how to build nodes and weights for integration over agent choice
         probabilities, which will replace any ``nodes`` and ``weights`` fields in ``agent_data``. This configuration is
         required if ``nodes`` and ``weights`` in ``agent_data`` are not specified. It should not be specified if
         :math:`X_2` is not formulated in ``product_formulations``.
 
         If this configuration is specified, :math:`K_2` columns of nodes (the number of demand-side nonlinear product
@@ -331,14 +350,16 @@
         Number of demographic variables, :math:`D`.
     MD : `int`
         Number of demand-side instruments, :math:`M_D`, which is always zero because instruments are added or
         constructed in :meth:`SimulationResults.to_problem`.
     MS : `int`
         Number of supply-side instruments, :math:`M_S`, which is always zero because  instruments are added or
         constructed in :meth:`SimulationResults.to_problem`.
+    MC : `int`
+        Number of covariance instruments, :math:`M_C`.
     ED : `int`
         Number of absorbed dimensions of demand-side fixed effects, :math:`E_D`, which is always zero because
         simulations do not support fixed effect absorption.
     ES : `int`
         Number of absorbed dimensions of supply-side fixed effects, :math:`E_S`, which is always zero because
         simulations do not support fixed effect absorption.
     H : `int`
@@ -453,29 +474,31 @@
         agent_mapping = None
         if products.X2.shape[1] > 0:
             # determine the number of agents by loading market IDs or by building them along with nodes and weights
             if integration is not None:
                 if not isinstance(integration, Integration):
                     raise ValueError("integration must be None or an Integration instance.")
                 agent_market_ids, nodes, weights = integration._build_many(products.X2.shape[1], np.unique(market_ids))
-                agent_ids = None
+                agent_ids = availability = None
             elif agent_data is not None:
                 agent_market_ids = extract_matrix(agent_data, 'market_ids')
                 agent_ids = extract_matrix(agent_data, 'agent_ids')
                 nodes = extract_matrix(agent_data, 'nodes')
                 weights = extract_matrix(agent_data, 'weights')
+                availability = extract_matrix(agent_data, 'availability')
             else:
                 raise ValueError("At least one of agent_data or integration must be specified.")
 
             # load or simulate agent variables in sorted order so that a seed always gives the same draws
             agent_mapping = {
                 'market_ids': (agent_market_ids, np.object_),
                 'agent_ids': (agent_ids, np.object_),
                 'nodes': (nodes, options.dtype),
-                'weights': (weights, options.dtype)
+                'weights': (weights, options.dtype),
+                'availability': (availability, options.dtype),
             }
             if agent_formulation is not None:
                 for name in sorted(agent_formulation._names - set(agent_mapping)):
                     matrix = extract_matrix(agent_data, name) if agent_data is not None else None
                     if matrix is None:
                         agent_mapping[name] = (state.uniform(size=agent_market_ids.size), options.dtype)
                     else:
```

### Comparing `pyblp-1.0.0/pyblp/exceptions.py` & `pyblp-1.1.0/pyblp/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/markets/economy_results_market.py` & `pyblp-1.1.0/pyblp/markets/economy_results_market.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,14 +373,18 @@
         utilities = delta + mu
         if self.H > 0:
             utilities /= 1 - self.rho
         utility_reduction = np.clip(utilities.max(axis=0, keepdims=True), 0, None)
         exp_utilities = np.exp(utilities - utility_reduction)
         scale_weights = 1
 
+        # optionally adjust for agent-specific product availability
+        if self.agents.availability.size > 0:
+            exp_utilities *= self.agents.availability.T
+
         # eliminate any products from the choice set
         if eliminate_product_ids is not None:
             for j, product_id in enumerate(self.products.product_ids[:, product_ids_index]):
                 if product_id in eliminate_product_ids:
                     exp_utilities[j] = 0
 
         # handle nesting
```

### Comparing `pyblp-1.0.0/pyblp/markets/market.py` & `pyblp-1.1.0/pyblp/markets/market.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,23 +72,26 @@
         if options.drop_product_fields:
             products_update_mapping = {}
             for key in ['demand_ids', 'supply_ids', 'clustering_ids', 'X1', 'X3', 'ZD', 'ZS', 'ownership']:
                 products_update_mapping[key] = (None, self.products[key].dtype)
             self.products = update_matrices(self.products, products_update_mapping)
 
         # fill missing columns of integration nodes (associated with zeros in sigma) with zeros and drop extra
-        #   product-specific demographic values for product indices not in this market
+        #   product-specific demographic/agent-specific product availability values for products not in this market
         agents_update_mapping: Dict[str, Tuple[Optional[Array], Any]] = {}
         if self.agents.nodes.shape[1] != economy.K2 and not parameters.nonzero_sigma_index.all():
             nodes = np.zeros((self.agents.shape[0], economy.K2), self.agents.nodes.dtype)
             nodes[:, parameters.nonzero_sigma_index] = self.agents.nodes[:, :parameters.nonzero_sigma_index.sum()]
             agents_update_mapping['nodes'] = (nodes, nodes.dtype)
         if len(self.agents.demographics.shape) == 3:
             demographics = self.agents.demographics[..., :self.products.size]
             agents_update_mapping['demographics'] = (demographics, demographics.dtype)
+        if self.agents.availability.size > 0:
+            availability = self.agents.availability[..., :self.products.size]
+            agents_update_mapping['availability'] = (availability, availability.dtype)
         if agents_update_mapping:
             self.agents = update_matrices(self.agents, agents_update_mapping)
 
         # create nesting groups but keep all nesting IDs for associating parameters with groups
         self.groups = Groups(self.products.nesting_ids)
         self.unique_nesting_ids = economy.unique_nesting_ids
 
@@ -327,16 +330,16 @@
 
         return derivatives
 
     def compute_probabilities(
             self, delta: Array = None, mu: Optional[Array] = None, linear: bool = True, safe: bool = True,
             utility_reduction: Optional[Array] = None, numerator: Optional[Array] = None,
             eliminate_outside: bool = False, eliminate_product: Optional[int] = None,
-            eliminate_product_id: Optional[Any] = None, product_ids_index: Optional[int] = None) -> (
-            Tuple[Array, Optional[Array]]):
+            eliminate_product_id: Optional[Any] = None, product_ids_index: Optional[int] = None,
+            availability: Optional[Array] = None) -> Tuple[Array, Optional[Array]]:
         """Compute choice probabilities. By default, use unchanged delta and mu values. If linear is False, delta and mu
         must be specified and already be exponentiated. If safe is True, scale the logit equation by the exponential of
         negative the maximum utility for each agent, and if utility_reduction is specified, it should be values that
         have already been subtracted from the specified utility for each agent. If the numerator is specified, it will
         be used as the numerator in the non-nested logit expression. If any products are eliminated, eliminate the
         outside option, an inside product, a group of products with the same product ID, or any of these from the
         choice set.
@@ -380,14 +383,20 @@
                 if self.rho_size > 1:
                     scale_weights = np.exp(-utility_reduction[None] * (self.group_rho.T - self.group_rho)[..., None])
 
         # optionally eliminate the outside option from the choice set
         if eliminate_outside:
             scale = 0
 
+        # optionally adjust for agent-specific product availability
+        if availability is None and self.agents.availability.size > 0:
+            availability = self.agents.availability
+        if availability is not None:
+            exp_utilities *= availability.T
+
         # optionally eliminate a product from the choice set
         if eliminate_product is not None:
             exp_utilities[eliminate_product] = 0
 
         # optionally eliminate all products with the same product ID from the choice set
         if eliminate_product_id is not None:
             exp_utilities[self.products.product_ids[:, product_ids_index] == eliminate_product_id] = 0
@@ -651,14 +660,15 @@
 
         utility_derivatives = self.compute_utility_derivatives('prices')
         probability_utility_derivatives = probabilities * utility_derivatives
         capital_lamda_diagonal, capital_delta = self.compute_capital_lamda_gamma(
             probability_utility_derivatives, probabilities, conditionals
         )
         np.einsum('jj->j', capital_delta)[...] -= capital_lamda_diagonal
+        capital_delta = capital_delta.T
         capital_delta *= ownership
 
         # use solve if not keeping the inverse of capital delta
         if not keep_capital_delta_inverse:
             capital_delta_inverse = None
             eta, replacement = approximately_solve(capital_delta, self.products.shares)
             if replacement:
@@ -1019,19 +1029,29 @@
             # handle any groups of eliminated products
             if eliminate_product_id is not None:
                 utilities[self.products.product_ids[:, product_ids_index] == eliminate_product_id] = -np.inf
 
             # compute the tangent of marginal probabilities with respect to the parameter (re-scale for robustness)
             utility_reduction = np.clip(utilities.max(axis=0, keepdims=True), 0, None)
             with np.errstate(divide='ignore', invalid='ignore'):
+                exp_utilities = np.exp(utilities - utility_reduction)
+
+                # hand agent-specific product availability
+                if self.agents.availability.size > 0:
+                    availability = self.agents.availability
+                    if agent_indices is not None:
+                        availability = availability[agent_indices]
+                    exp_utilities *= availability.T
+
                 B = marginals * (
                     A_sums * (1 - self.group_rho) -
-                    (np.log(self.groups.sum(np.exp(utilities - utility_reduction))) + utility_reduction)
+                    (np.log(self.groups.sum(exp_utilities)) + utility_reduction)
                 )
                 marginals_tangent = group_associations * B - marginals * (group_associations.T @ B)
+
             marginals_tangent[~np.isfinite(marginals_tangent)] = 0
 
         else:
             assert isinstance(parameter, GammaParameter)
             conditionals_tangent = np.zeros_like(conditionals)
             marginals_tangent = np.zeros_like(marginals)
 
@@ -1305,14 +1325,15 @@
             capital_lamda_diagonal_tangent, capital_delta_tangent = (
                 self.compute_capital_lamda_gamma_by_parameter_tangent(
                     parameter, probability_utility_derivatives, probability_utility_derivatives_tangent, probabilities,
                     probabilities_tangent_mapping[p], conditionals, conditionals_tangent_mapping[p]
                 )
             )
             np.einsum('jj->j', capital_delta_tangent)[...] -= capital_lamda_diagonal_tangent
+            capital_delta_tangent = capital_delta_tangent.T
             capital_delta_tangent *= ownership
 
             # subtract this parameter's contribution
             eta_jacobian[:, [p]] = -(capital_delta_inverse @ capital_delta_tangent @ eta)
 
         return eta_jacobian
 
@@ -1417,16 +1438,19 @@
             ]):
         """Compute contributions of micro datasets to micro moments."""
         if delta is None:
             assert self.delta is not None
             delta = self.delta
 
         mu = None
+        availability = None
         if agent_indices is not None:
             mu = self.mu[:, agent_indices]
+            if self.agents.availability.size > 0:
+                availability = self.agents.availability[agent_indices]
 
         # pre-compute and validate micro dataset weights, multiplying these with probabilities and using these to
         #   compute micro value denominators
         weights_mapping: Dict[MicroDataset, Array] = {}
         denominator_mapping: Dict[MicroDataset, Array] = {}
         outside_probabilities = None
         eliminated_probabilities: Dict[Optional[int], Array] = {}
@@ -1450,15 +1474,15 @@
                 product_groups = Groups(product_ids)
 
             # compute and validate weights
             weights = self.compute_micro_weights(dataset, agent_indices)
 
             # pre-compute probabilities
             if probabilities is None:
-                probabilities, _ = self.compute_probabilities(delta, mu)
+                probabilities, _ = self.compute_probabilities(delta, mu, availability=availability)
 
             # pre-compute outside probabilities
             need_outside_probabilities = len(weights.shape) == 2 and weights.shape[1] == 1 + self.J
             need_outside_probabilities |= len(weights.shape) == 3 and weights.shape[2] == 1 + self.J
             if need_outside_probabilities and outside_probabilities is None:
                 outside_probabilities = 1 - probabilities.sum(axis=0)
 
@@ -1481,15 +1505,15 @@
                             with np.errstate(all='ignore'):
                                 eliminated_probabilities_j = probabilities / (1 - probabilities[j][None])
                                 eliminated_probabilities_j[j] = 0
 
                         # re-compute probabilities if there is nesting or there was a numerical error
                         if eliminated_probabilities_j is None or not np.isfinite(eliminated_probabilities_j).all():
                             eliminated_probabilities_j, eliminated_conditionals_j = self.compute_probabilities(
-                                delta, mu, eliminate_product=j
+                                delta, mu, eliminate_product=j, availability=availability
                             )
 
                         eliminated_probabilities_list.append(eliminated_probabilities_j)
                         eliminated_conditionals_list.append(eliminated_conditionals_j)
 
                     eliminated_probabilities[ids_index] = np.stack(eliminated_probabilities_list)
                 else:
@@ -1506,15 +1530,16 @@
                                     probabilities / (1 - probabilities[product_id_index].sum(axis=0, keepdims=True))
                                 )
                                 eliminated_probabilities_j[product_id_index] = 0
 
                         # re-compute probabilities if there is nesting or there was a numerical error
                         if eliminated_probabilities_j is None or not np.isfinite(eliminated_probabilities_j).all():
                             eliminated_probabilities_j, eliminated_conditionals_j = self.compute_probabilities(
-                                delta, mu, eliminate_product_id=product_id, product_ids_index=ids_index
+                                delta, mu, eliminate_product_id=product_id, product_ids_index=ids_index,
+                                availability=availability
                             )
 
                         eliminated_probabilities_list.append(eliminated_probabilities_j)
                         eliminated_conditionals_list.append(eliminated_conditionals_j)
 
                     eliminated_probabilities[ids_index] = np.stack(
                         [eliminated_probabilities_list[i] for i in product_groups.codes]
@@ -1598,15 +1623,15 @@
                 if self.H == 0:
                     with np.errstate(all='ignore'):
                         outside_eliminated_probabilities = probabilities / probabilities.sum(axis=0, keepdims=True)
 
                 # re-compute probabilities if there is nesting or there was a numerical error
                 if outside_eliminated_probabilities is None or not np.isfinite(outside_eliminated_probabilities).all():
                     outside_eliminated_probabilities, outside_eliminated_conditionals = self.compute_probabilities(
-                        delta, mu, eliminate_outside=True
+                        delta, mu, eliminate_outside=True, availability=availability
                     )
 
                 if compute_jacobians:
                     # use a fast analytic trick when possible
                     if self.H == 0:
                         with np.errstate(all='ignore'):
                             outside_eliminated_ratio = outside_eliminated_probabilities / probabilities
```

### Comparing `pyblp-1.0.0/pyblp/markets/problem_market.py` & `pyblp-1.1.0/pyblp/markets/problem_market.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/markets/simulation_market.py` & `pyblp-1.1.0/pyblp/markets/simulation_market.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/micro.py` & `pyblp-1.1.0/pyblp/micro.py`

 * *Files 3% similar despite different names*

```diff
@@ -320,17 +320,17 @@
             raise TypeError("value must be a float.")
         if not np.isfinite(value):
             raise ValueError("value must be a finite number.")
 
         if isinstance(parts, MicroPart):
             parts = [parts]
             if compute_value is None:
-                compute_value = lambda v: float(v)
+                compute_value = default_compute_value
             if compute_gradient is None:
-                compute_gradient = lambda v: np.ones_like(v)
+                compute_gradient = default_compute_gradient
         else:
             if not isinstance(parts, collections.abc.Sequence) or len(parts) < 1:
                 raise TypeError("parts must be a MicroPart instance or a sequence of instances.")
             if compute_value is None:
                 raise TypeError("Since parts is a sequence of MicroPart instances, compute_value must be specified.")
             if compute_gradient is None:
                 raise TypeError("Since parts is a sequence of MicroPart instances, compute_gradient must be specified.")
@@ -360,14 +360,26 @@
 
     def __str__(self) -> str:
         """Format information about the moment as a string."""
         parts_string = str(self.parts) if isinstance(self.parts, MicroPart) else "; ".join(str(p) for p in self.parts)
         return f"{self.name}: {format_number(self.value)} ({parts_string})"
 
 
+def default_compute_value(part_values: Array) -> float:
+    """Define the default micro value computation function for a single micro part. This needs to be at the module
+    level to allow for standard multiprocessing to work.
+    """
+    return float(part_values)
+
+
+def default_compute_gradient(part_values: Array) -> Array:
+    """Define the same but for the gradient."""
+    return np.ones_like(part_values)
+
+
 class Moments(object):
     """Information about a sequence of micro moments."""
 
     micro_moments: Sequence[MicroMoment]
     micro_parts: Sequence[MicroPart]
     values: Array
     MM: int
```

### Comparing `pyblp-1.0.0/pyblp/options.py` & `pyblp-1.1.0/pyblp/options.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/parameters.py` & `pyblp-1.1.0/pyblp/parameters.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/primitives.py` & `pyblp-1.1.0/pyblp/primitives.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,16 @@
         Full set of demand-side instruments, :math:`Z_D`, which typically consists of excluded demand-side instruments
         and :math:`X_1^\text{ex}`. If there are any demand-side fixed effects, these instruments will be residualized
         with respect to these fixed effects.
     ZS : `ndarray`
         Full set of supply-side instruments, :math:`Z_S`, which typically consists of excluded supply-side instruments
         and :math:`X_3^\text{ex}`. If there are any supply-side fixed effects, these instruments will be residualized
         with respect to these fixed effects.
+    ZC : `ndarray`
+        Covariance instruments, :math:`Z_C`, as in :ref:`references:MacKay and Miller (2023)`.
     X1 : `ndarray`
         Demand-side linear product characteristics, :math:`X_1`. If there are any demand-side fixed effects, these
         characteristics will be residualized with respect to these fixed effects.
     X2 : `ndarray`
         Demand-side nonlinear product characteristics, :math:`X_2`.
     X3 : `ndarray`
         Supply-side product characteristics, :math:`X_3`. If there are any supply-side fixed effects, these
@@ -68,14 +70,15 @@
     product_ids: Array
     clustering_ids: Array
     ownership: Array
     shares: Array
     prices: Array
     ZD: Array
     ZS: Array
+    ZC: Array
     X1: Array
     X2: Array
     X3: Array
 
     def __new__(
             cls, product_formulations: Sequence[Optional[Formulation]], product_data: Mapping,
             instruments: bool = True, add_exogenous: bool = True) -> RecArray:
@@ -140,14 +143,21 @@
             if ZS is not None and not np.isfinite(ZS).all():
                 raise ValueError("The supply_instruments field of product_data should not have NaNs or infinities.")
             if add_exogenous:
                 for index, formulation in enumerate(X3_formulations):
                     if 'shares' not in formulation.names:
                         ZS = X3[:, [index]] if ZS is None else np.c_[ZS, X3[:, [index]]]
 
+        # load covariance instruments
+        ZC = None
+        if instruments and X3 is not None:
+            ZC = extract_matrix(product_data, 'covariance_instruments')
+            if ZC is not None and not np.isfinite(ZC).all():
+                raise ValueError("The covariance_instruments field of product_data should not have NaNs or infinities.")
+
         # load fixed effect IDs
         demand_ids = None
         supply_ids = None
         if product_formulations[0]._absorbed_terms:
             demand_ids = product_formulations[0]._build_ids(product_data)
         if product_formulations[2] is not None and product_formulations[2]._absorbed_terms:
             supply_ids = product_formulations[2]._build_ids(product_data)
@@ -213,20 +223,21 @@
             'supply_ids': (supply_ids, np.object_),
             'nesting_ids': (nesting_ids, np.object_),
             'product_ids': (product_ids, np.object_),
             'clustering_ids': (clustering_ids, np.object_),
             'ownership': (ownership, options.dtype),
             'shares': (shares, options.dtype),
             'ZD': (ZD, options.dtype),
-            'ZS': (ZS, options.dtype)
+            'ZS': (ZS, options.dtype),
+            'ZC': (ZC, options.dtype),
         })
         product_mapping.update({
             (tuple(X1_formulations), 'X1'): (X1, options.dtype),
             (tuple(X2_formulations), 'X2'): (X2, options.dtype),
-            (tuple(X3_formulations), 'X3'): (X3, options.dtype)
+            (tuple(X3_formulations), 'X3'): (X3, options.dtype),
         })
 
         # structure and validate variables underlying X1, X2, and X3
         underlying_data = {k: (v, options.dtype) for k, v in {**X1_data, **X2_data, **X3_data}.items() if k != 'shares'}
         invalid_names = set(underlying_data) & {k if isinstance(k, str) else k[1] for k in product_mapping}
         if invalid_names:
             raise NameError(f"These reserved names in product_formulations are invalid: {list(invalid_names)}.")
@@ -245,36 +256,40 @@
         IDs that identify agents within markets.
     weights : `ndarray`
         Integration weights, :math:`w`.
     nodes : `ndarray`
         Unobserved agent characteristics called integration nodes, :math:`\nu`.
     demographics : `ndarray`
         Observed agent characteristics, :math:`d`.
+    availability : `ndarray`
+        Agent-specific product availability, :math:`a`.
 
     """
 
     market_ids: Array
     agent_ids: Array
     weights: Array
     nodes: Array
     demographics: Array
+    availability: Array
 
     def __new__(
             cls, products: RecArray, agent_formulation: Optional[Formulation] = None,
             agent_data: Optional[Mapping] = None, integration: Optional[Integration] = None,
             check_weights: bool = True) -> RecArray:
         """Structure agent data."""
 
         # data structures may be empty
         market_ids = None
         agent_ids = None
         weights = None
         nodes = None
         demographics = None
         demographics_formulations: List[ColumnFormulation] = []
+        availability = None
 
         # if there are only linear characteristics, build a trivial set of agents
         K2 = products.X2.shape[1]
         if K2 == 0:
             if agent_formulation is not None or agent_data is not None or integration is not None:
                 raise ValueError(
                     "Since X2 is not formulated, none of agent_formulation, agent_data, and integration should be "
@@ -294,26 +309,34 @@
                 demographics, demographics_formulations = build_demographics(products, agent_data, agent_formulation)
                 assert demographics is not None
                 if len(demographics.shape) == 2 and not np.isfinite(demographics).all():
                     raise ValueError(
                         "Variables in agent_data that contribute to demographics should not have NaNs or infinities."
                     )
 
-            # load IDs
+            # load IDs and any availability
             if agent_data is not None:
                 market_ids = extract_matrix(agent_data, 'market_ids')
                 agent_ids = extract_matrix(agent_data, 'agent_ids')
+                availability = extract_matrix(agent_data, 'availability')
                 if market_ids is None:
                     raise KeyError("agent_data must have a market_ids field.")
                 if market_ids.shape[1] > 1:
                     raise ValueError("The market_ids field of agent_data must be one-dimensional.")
                 if set(np.unique(products.market_ids)) != set(np.unique(market_ids)):
                     raise ValueError("The market_ids field of agent_data must have the same IDs as product data.")
                 if agent_ids is not None and agent_ids.shape[1] > 1:
                     raise ValueError("The agent_ids field of agent_data must be one-dimensional.")
+                if availability is not None:
+                    max_J = max(i.size for i in get_indices(products.market_ids).values())
+                    if availability.shape[1] < max_J:
+                        raise ValueError(
+                            f"The availability field of agent_data must have at least {max_J} columns, which is the "
+                            f"number of products in the market with the most products."
+                        )
 
             # build nodes and weights
             if integration is not None:
                 if not isinstance(integration, Integration):
                     raise ValueError("integration must be None or an Integration instance.")
                 loaded_market_ids = market_ids
                 market_ids, nodes, weights = integration._build_many(K2, np.unique(products.market_ids))
@@ -368,52 +391,62 @@
             )
 
         return structure_matrices({
             'market_ids': (market_ids, np.object_),
             'agent_ids': (agent_ids, np.object_),
             'weights': (weights, options.dtype),
             'nodes': (nodes, options.dtype),
-            (tuple(demographics_formulations), 'demographics'): (demographics, options.dtype)
+            (tuple(demographics_formulations), 'demographics'): (demographics, options.dtype),
+            'availability': (availability, options.dtype),
         })
 
 
 class MicroAgents(object):
     """Micro agent data structured as a record array."""
 
     micro_ids: Array
     market_ids: Array
     agent_ids: Array
     weights: Array
     nodes: Array
     demographics: Array
+    availability: Array
     choice_indices: Array
     second_choice_indices: Array
 
     def __new__(
             cls, products: RecArray, parameters: Parameters, micro_data: Mapping, demographics: Optional[Array] = None,
             demographics_formulations: Sequence[ColumnFormulation] = (),
             integration: Optional[Integration] = None) -> RecArray:
         """Structure agent data."""
         K2 = products.X2.shape[1]
         if K2 == 0:
             raise ValueError("X2 is not formulated.")
 
-        # load IDs and indices
+        # load IDs, availability, and indices
         market_ids = extract_matrix(micro_data, 'market_ids')
         agent_ids = extract_matrix(micro_data, 'agent_ids')
+        availability = extract_matrix(micro_data, 'availability')
         choice_indices = extract_matrix(micro_data, 'choice_indices')
         second_choice_indices = extract_matrix(micro_data, 'second_choice_indices')
         if market_ids is None:
             raise KeyError("micro_data must have a market_ids field.")
         if market_ids.shape[1] > 1:
             raise ValueError("The market_ids field of micro_data must be one-dimensional.")
         if set(np.unique(market_ids)) - set(np.unique(products.market_ids)):
             raise ValueError("The market_ids field of micro_data must not have IDs that are not in product data.")
         if agent_ids is not None and agent_ids.shape[1] > 1:
             raise ValueError("The agent_ids field of micro_data must be one-dimensional.")
+        if availability is not None:
+            max_J = max(i.size for i in get_indices(products.market_ids).values())
+            if availability.shape[1] < max_J:
+                raise ValueError(
+                    f"The availability field of micro_data must have at least {max_J} columns, which is the number of "
+                    f"products in the market with the most products."
+                )
         if choice_indices is not None and choice_indices.shape[1] > 1:
             raise ValueError("The choice_indices field of micro_data must be one-dimensional.")
         if second_choice_indices is not None and second_choice_indices.shape[1] > 1:
             raise ValueError("The second_choice_indices field of micro_data must be one-dimensional.")
 
         # either load micro IDs, nodes, and weights, or build them
         if integration is None:
@@ -465,14 +498,15 @@
             # duplicate observations by as many rows as there are built nodes
             micro_ids, nodes, weights = integration._build_many(
                 parameters.nonzero_sigma_index.sum(), np.arange(market_ids.size)
             )
             repeats = np.bincount(micro_ids)
             duplicate = lambda x: np.repeat(x, repeats, axis=0) if x is not None else None
             demographics = duplicate(demographics)
+            availability = duplicate(availability)
             market_ids = duplicate(market_ids)
             agent_ids = duplicate(agent_ids)
             choice_indices = duplicate(choice_indices)
             second_choice_indices = duplicate(second_choice_indices)
 
         # output a warning if weights do not sum to one for each observation
         micro_groups = Groups(micro_ids)
@@ -488,14 +522,15 @@
         return structure_matrices({
             'micro_ids': (micro_ids, np.object_),
             'market_ids': (market_ids, np.object_),
             'agent_ids': (agent_ids, np.object_),
             'weights': (weights, options.dtype),
             'nodes': (nodes, options.dtype),
             (tuple(demographics_formulations), 'demographics'): (demographics, options.dtype),
+            'availability': (availability, options.dtype),
             'choice_indices': (choice_indices, np.int64),
             'second_choice_indices': (second_choice_indices, np.int64),
         })
 
 
 def build_demographics(
         products: RecArray, data: Mapping, agent_formulation: Optional[Formulation]) -> (
```

### Comparing `pyblp-1.0.0/pyblp/results/bootstrapped_results.py` & `pyblp-1.1.0/pyblp/results/bootstrapped_results.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/results/economy_results.py` & `pyblp-1.1.0/pyblp/results/economy_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1263,15 +1263,16 @@
         ----------
         dataset : `MicroDataset`
             The :class:`MicroDataset` for which scores will be computed. The ``compute_weights`` function is called
             separately for each observation :math:`n`.
         micro_data : `structured array-like`
             Each row corresponds either to an observation :math:`n` or if there are multiple rows per observation, to
             an :math:`i \in I_n` that integrates over unobserved heterogeneity. In addition to the names of any
-            demographics used in the ``agent_formulation``, the following fields are required:
+            demographics used in the ``agent_formulation`` and any specification of agent-specific product
+            ``'availability'``, the following fields are required:
 
                 - **market_ids** : (`object`) - Market IDs :math:`t_n` for each observation :math:`n`.
 
                 - **choice_indices** : (`int`) - Within-market indices of choices :math:`j_n`. If ``compute_weights``
                   passed to the ``dataset`` returns an array with :math:`J_t` elements in its second axis, then choice
                   indices take on values from :math:`0` to :math:`J_t - 1` where :math:`0` corresponds to the first
                   inside good. If it returns an array with :math:`1 + J_t` elements in its second axis, then choice
@@ -1453,14 +1454,15 @@
             demographics_formulations = agents.dtype.fields['demographics'][2]
             micro_data = {
                 'micro_ids': np.arange(agents.size),
                 'market_ids': agents.market_ids,
                 'agent_ids': agents.agent_ids,
                 'nodes': agents.nodes,
                 'weights': np.ones(agents.size),
+                'availability': agents.availability,
             }
             micro_agents = MicroAgents(
                 self._economy.products, self._parameters, micro_data, demographics, demographics_formulations,
                 integration
             )
 
         # compute the contributions
```

### Comparing `pyblp-1.0.0/pyblp/results/importance_sampling_results.py` & `pyblp-1.1.0/pyblp/results/importance_sampling_results.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/results/optimal_instrument_results.py` & `pyblp-1.1.0/pyblp/results/optimal_instrument_results.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/results/problem_results.py` & `pyblp-1.1.0/pyblp/results/problem_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,15 +315,16 @@
     _errors: List[Error]
 
     def __init__(
             self, progress: 'Progress', last_results: Optional['ProblemResults'], step: int, last_step: bool,
             step_start_time: float, optimization_start_time: float, optimization_end_time: float,
             optimization_stats: SolverStats, iteration_stats: Sequence[Dict[Hashable, SolverStats]],
             scaled_objective: bool, shares_bounds: Bounds, costs_bounds: Bounds,
-            micro_moment_covariances: Optional[Array], center_moments: bool, W_type: str, se_type: str) -> None:
+            micro_moment_covariances: Optional[Array], center_moments: bool, W_type: str, se_type: str,
+            covariance_moments_mean: float) -> None:
         """Compute cumulative progress statistics, update weighting matrices, and estimate standard errors."""
         self.sigma, self.pi, self.rho, _, _ = progress.parameters.expand(progress.theta)
         self._errors = progress.errors
         self.problem = progress.problem
         self.W = progress.W
         self.theta = progress.theta
         self.delta = progress.delta
@@ -437,27 +438,27 @@
         self.beta_labels = self._parameters.beta_labels
         self.gamma_labels = self._parameters.gamma_labels
         self.theta_labels = self._parameters.theta_labels
 
         # ignore computational errors when updating the weighting matrix and computing covariances
         with np.errstate(all='ignore'):
             # update the weighting matrix
-            S_for_weights = self._compute_S(progress.moments, W_type, center_moments)
+            S_for_weights = self._compute_S(progress.moments, W_type, covariance_moments_mean, center_moments)
             self.updated_W, W_errors = compute_gmm_weights(S_for_weights)
             self._errors.extend(W_errors)
 
             # only compute parameter covariances and standard errors if this is the last step
             self.moments_jacobian = np.full((self.moments.size, self.parameters.size), np.nan, options.dtype)
             self.parameter_covariances = np.full((self.parameters.size, self.parameters.size), np.nan, options.dtype)
             se = np.full((self.parameters.size, 1), np.nan, options.dtype)
             sigma_squared_vector_se = np.full((self.problem.K2 * (self.problem.K2 + 1) // 2, 1), np.nan, options.dtype)
             if last_step:
                 S_for_covariances = S_for_weights
                 if se_type != W_type or center_moments:
-                    S_for_covariances = self._compute_S(progress.moments, se_type)
+                    S_for_covariances = self._compute_S(progress.moments, se_type, covariance_moments_mean)
 
                 # if this is the first step, an unadjusted weighting matrix needs to be used when computing unadjusted
                 #   covariances so that they are scaled properly
                 W_for_covariances = self.W
                 if se_type == 'unadjusted' and self.step == 1:
                     W_for_covariances, W_for_covariances_errors = compute_gmm_weights(S_for_covariances)
                     self._errors.extend(W_for_covariances_errors)
@@ -530,31 +531,42 @@
         if self.problem.K3 > 0:
             Z_list.append(self.problem.products.ZS)
             jacobian_list.append(np.c_[
                 self.omega_by_theta_jacobian,
                 np.zeros_like(self.problem.products.X1[:, self._parameters.eliminated_beta_index.flat]),
                 -self.problem.products.X3[:, self._parameters.eliminated_gamma_index.flat]
             ])
+            if self.problem.MC > 0:
+                Z_list.append(self.problem.products.ZC)
+                jacobian_list.append(np.c_[
+                    self.xi_by_theta_jacobian * self.omega + self.xi * self.omega_by_theta_jacobian,
+                    -self.problem.products.X1[:, self._parameters.eliminated_beta_index.flat] * self.omega,
+                    self.xi * -self.problem.products.X3[:, self._parameters.eliminated_gamma_index.flat]
+                ])
         mean_G = np.r_[
             compute_gmm_moments_jacobian_mean(jacobian_list, Z_list),
             np.c_[
                 self.micro_by_theta_jacobian,
                 np.zeros((moments.MM, self._parameters.eliminated_beta_index.sum()), options.dtype),
                 np.zeros((moments.MM, self._parameters.eliminated_gamma_index.sum()), options.dtype)
             ]
         ]
         return mean_G
 
-    def _compute_S(self, moments: Moments, S_type: str, center_moments: bool = False) -> Array:
+    def _compute_S(
+            self, moments: Moments, S_type: str, covariance_moments_mean: float, center_moments: bool = False) -> Array:
         """Compute moment covariances."""
         u_list = [self.xi]
         Z_list = [self.problem.products.ZD]
         if self.problem.K3 > 0:
             u_list.append(self.omega)
             Z_list.append(self.problem.products.ZS)
+            if self.problem.MC > 0:
+                u_list.append(self.xi * self.omega - covariance_moments_mean)
+                Z_list.append(self.problem.products.ZC)
 
         S = compute_gmm_moment_covariances(u_list, Z_list, S_type, self.problem.products.clustering_ids, center_moments)
         self.problem._detect_singularity(S, "the estimated covariance matrix of aggregate GMM moments")
         if moments.MM > 0:
             S = scipy.linalg.block_diag(S, self.problem.N * self.micro_covariances)
 
         S += self.simulation_covariances
@@ -1062,14 +1074,21 @@
 
            When both a supply and demand side are estimated, there are usually collinear rows in
            :eq:`optimal_instruments` because of overlapping product characteristics in :math:`X_1` and :math:`X_3`. The
            expression can be corrected by multiplying it with a conformable matrix of ones and zeros that remove the
            collinearity problem. The question of which rows to exclude is addressed in
            :meth:`OptimalInstrumentResults.to_problem`.
 
+        .. warning::
+
+           Currently, only optimal instruments for the standard demand- and supply-side moments are supported. If
+           ``covariance_instruments`` were specified in ``product_data``, the computed optimal instruments will only be
+           optimal with respect to the demand- and supply-side moments, not with respect to the addition of any
+           covariance moments as well.
+
         Parameters
         ----------
         method : `str, optional`
             The method by which the integral over the joint density of :math:`\xi` and :math:`\omega` is approximated.
             The following methods are supported:
 
                 - ``'approximate'`` (default) - Evaluate the Jacobians at the expected value of the error terms: zero
```

### Comparing `pyblp-1.0.0/pyblp/results/simulation_results.py` & `pyblp-1.1.0/pyblp/results/simulation_results.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/utilities/algebra.py` & `pyblp-1.1.0/pyblp/utilities/algebra.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp/utilities/basics.py` & `pyblp-1.1.0/pyblp/utilities/basics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Basic functionality."""
 
 import contextlib
 import copyreg
 import functools
 import inspect
 import multiprocessing.pool
+import pickle
 import re
 import sys
 import time
 import traceback
 from typing import (
     Any, Callable, Container, Dict, Hashable, Iterable, Iterator, List, Mapping, Optional, Set, Sequence, Type, Tuple,
     Union
@@ -47,15 +48,19 @@
 
     Arguments
     ---------
     processes : `int`
         Number of Python processes that will be created and used by any method that supports parallel processing.
     use_pathos : `bool, optional`
         Whether to use `pathos <https://pathos.readthedocs.io/en/latest/>`_ (which will need to be installed) instead of
-        the default, built-in :mod:`multiprocessing` module.
+        the default, built-in :mod:`multiprocessing` module. Since pathos uses
+        `dill <https://dill.readthedocs.io/en/latest/>`_ to pickle and pass objects between processes, it can support
+        more objects than the default `multiprocessing <https://docs.python.org/3/library/multiprocessing.html>`_
+        module, which uses the default `pickle <https://docs.python.org/3/library/pickle.html>`_ module. However, dill
+        can be much slower, so using pathos can further increase overhead of passing data between processes.
 
     Examples
     --------
     .. raw:: latex
 
        \begin{examplenotebook}
 
@@ -89,71 +94,79 @@
 
     # start the process pool, wait for work to be done, and then terminate it
     output(f"Starting a pool of {processes} processes ...")
     start_time = time.time()
     global pool
     if use_pathos:
         try:
-            from pathos.multiprocessing import ProcessPool
+            import pathos
         except ImportError as exception:
             if "pathos" not in str(exception):
                 raise
             raise ImportError("pathos must be installed when use_pathos is True.") from exception
+
+        # enable pathos' pickling library's recursion feature, which is necessary in particular because SymPy is a
+        #   dependency that automatically uses gmpy2 when installed, which has some classes that need this feature to
+        #   be pickled
+        try:
+            import dill
+            default_dill_recurse = dill.settings['recurse']
+            dill.settings['recurse'] = True
+        except ImportError as exception:
+            if "dill" not in str(exception):
+                raise
+            raise ImportError("dill must be installed when use_pathos is True.") from exception
+
+        # revert to standard pickling of NumPy record arrays because dill's approach is very slow
+        @dill.register(np.recarray)
+        def pickle_recarray(pickler: dill.Pickler, x: RecArray) -> Any:
+            """Revert to standard pickling."""
+            pickler.save_reduce(pickle.loads, (pickle.dumps(x),), obj=x)
+
         try:
-            pool = ProcessPool(nodes=processes)
-            output(f"Started the process pool after {format_seconds(time.time() - start_time)}.")
-            yield
+            with pathos.multiprocessing.Pool(processes) as pool:
+                output(f"Started the process pool after {format_seconds(time.time() - start_time)}.")
+                yield
+                output(f"Terminating the pool of {processes} processes ...")
+                terminate_time = time.time()
         finally:
-            output(f"Terminating the pool of {processes} processes ...")
-            terminate_time = time.time()
-            try:
-                pool.close()
-            except Exception:
-                pass
-            try:
-                pool.join()
-            except Exception:
-                pass
-            try:
-                pool.clear()
-            except Exception:
-                pass
             pool = None
+            dill.settings['recurse'] = default_dill_recurse
     else:
         try:
             with multiprocessing.pool.Pool(processes) as pool:
                 output(f"Started the process pool after {format_seconds(time.time() - start_time)}.")
                 yield
                 output(f"Terminating the pool of {processes} processes ...")
                 terminate_time = time.time()
         except AttributeError as exception:
-            if "Can't pickle local object" not in str(exception) or "<lambda>" not in str(exception):
+            if "Can't pickle local object" not in str(exception):
                 raise
-            pathos_message = (
-                "The built-in multiprocessing module does not support lambda functions. Consider setting "
-                "the use_pathos of parallel to True."
+            object_message = "lambda functions" if '<lambda>' in str(exception) else "some objects"
+            pickling_message = (
+                f"The built-in multiprocessing module does not support {object_message}, such as the one referenced in "
+                f"the above exception. Consider setting the use_pathos argument of parallel to True, which will use "
+                f"the dill package for multiprocessing, which supports more objects. If using pathos results in large "
+                f"slow downs, consider applying a custom picking patch to the above object's class with the copyreg "
+                f"module (for standard multiprocessing and pickling) or with dill.register (for pathos and dill)."
             )
-            raise RuntimeError(pathos_message) from exception
+            raise RuntimeError(pickling_message) from exception
         finally:
             pool = None
     output(f"Terminated the process pool after {format_seconds(time.time() - terminate_time)}.")
 
 
 def generate_items(keys: Iterable, factory: Callable[[Any], tuple], method: Callable) -> Iterator:
     """Generate (key, method(*factory(key))) tuples for each key. The first element returned by factory is an instance
     of the class to which method is attached. If a process pool has been initialized, use multiprocessing; otherwise,
     use serial processing.
     """
     if pool is None:
         return (generate_items_worker((k, factory(k), method)) for k in keys)
-    try:
-        return pool.imap_unordered(generate_items_worker, ((k, factory(k), method) for k in keys))
-    except AttributeError:
-        # a pathos ProcessPool uses uimap instead of imap_unordered
-        return pool.uimap(generate_items_worker, ((k, factory(k), method) for k in keys))
+    return pool.imap_unordered(generate_items_worker, ((k, factory(k), method) for k in keys))
 
 
 def generate_items_worker(args: Tuple[Any, tuple, Callable]) -> Tuple[Any, Any]:
     """Call the specified method of a class instance with any additional arguments. Return the associated key along with
     the returned object.
     """
     key, (instance, *method_args), method = args
```

### Comparing `pyblp-1.0.0/pyblp/utilities/statistics.py` & `pyblp-1.1.0/pyblp/utilities/statistics.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,31 +30,38 @@
 
         # store any errors
         self.errors: List[Error] = []
         if replacement:
             self.errors.append(exceptions.LinearParameterCovariancesInversionError(covariances_inverse, replacement))
 
     def estimate(
-            self, X_list: List[Array], Z_list: List[Array], W: Array, y_list: List[Array]) -> (
-            Tuple[List[Array], List[Array]]):
-        """Estimate parameters and compute residuals."""
+            self, X_list: List[Array], Z_list: List[Array], W: Array, y_list: List[Array], jacobian_list: List[Array],
+            convert_jacobians: bool) -> Tuple[List[Array], List[Array], List[Array]]:
+        """Estimate parameters and compute residuals. Optionally convert Jacobians of y into Jacobians of residuals."""
 
         # stack matrices
         X = scipy.linalg.block_diag(*X_list)
         Z = scipy.linalg.block_diag(*Z_list)
         y = np.vstack(y_list)
 
         # estimate the model
-        parameters = self.covariances @ (X.T @ Z) @ W @ (Z.T @ y)
+        XZ = X.T @ Z
+        parameters = self.covariances @ XZ @ W @ (Z.T @ y)
         residuals = y - X @ parameters
 
         # split the parameters and residuals into lists
         parameters_list = np.split(parameters, [x.shape[1] for x in X_list[:-1]], axis=0)
         residuals_list = np.split(residuals, len(X_list), axis=0)
-        return parameters_list, residuals_list
+
+        # optionally convert Jacobians
+        if convert_jacobians:
+            jacobian = (np.eye(y.size) - X @ self.covariances @ XZ @ W @ Z.T) @ np.vstack(jacobian_list)
+            jacobian_list = np.split(jacobian, len(jacobian_list), axis=0)
+
+        return parameters_list, residuals_list, jacobian_list
 
 
 def compute_gmm_weights(S: Array) -> Tuple[Array, List[Error]]:
     """Compute a GMM weighting matrix."""
     errors: List[Error] = []
 
     # invert the matrix and handle any errors
@@ -124,24 +131,15 @@
 def compute_gmm_moments_mean(u_list: List[Array], Z_list: List[Array]) -> Array:
     """Compute GMM moments, averaged across observations."""
     return np.c_[compute_gmm_moments(u_list, Z_list).mean(axis=0)]
 
 
 def compute_gmm_moments_jacobian_mean(jacobian_list: List[Array], Z_list: List[Array]) -> Array:
     """Compute the Jacobian of GMM moments with respect to parameters, averaged across observations."""
-
-    # tensors or loops are not needed when there is only one equation
-    if len(jacobian_list) == 1:
-        N = Z_list[0].shape[0]
-        return Z_list[0].T @ jacobian_list[0] / N
-
-    # tensors are faster than loops for more than one equation
-    Z_transpose_stack = np.dstack(np.split(scipy.linalg.block_diag(*Z_list), len(jacobian_list)))
-    jacobian_stack = np.dstack(jacobian_list).swapaxes(1, 2)
-    return (Z_transpose_stack @ jacobian_stack).mean(axis=0)
+    return np.concatenate([j[:, None] * Z[:, :, None] for j, Z in zip(jacobian_list, Z_list)], axis=1).mean(axis=0)
 
 
 def compute_sigma_squared_vector_covariances(sigma: Array, sigma_vector_covariances: Array) -> Array:
     """Use the delta method to transform the asymptotic covariance matrix of vech(sigma) into the asymptotic covariance
     matrix of vech(sigma * sigma') where sigma is a lower triangular Cholesky root of parameters. See Section 10.5.4 in
     the Handbook of Matrices (Lutkepohl and Lutkepohl).
     """
```

### Comparing `pyblp-1.0.0/pyblp/__init__.py` & `pyblp-1.1.0/pyblp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/pyblp.egg-info/PKG-INFO` & `pyblp-1.1.0/pyblp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyblp
-Version: 1.0.0
+Version: 1.1.0
 Summary: BLP demand estimation with Python 3
 Home-page: https://github.com/jeffgortmaker/pyblp
 Author: Jeff Gortmaker, Christopher Conlon
 Author-email: jeff@jeffgortmaker.com
 License: MIT
 Project-URL: Documentation, http://pyblp.readthedocs.io/en/latest
 Project-URL: Tracker, https://github.com/jeffgortmaker/pyblp/issues
@@ -118,14 +118,15 @@
 --------
 
 - R-style formula interface
 - Bertrand-Nash supply-side moments
 - Multiple equation GMM
 - Demographic interactions
 - Product-specific demographics
+- Consumer-specific product availability
 - Flexible micro moments that can match statistics based on survey data
 - Support for micro moments based on second choice data
 - Support for optimal micro moments that match micro data scores
 - Fixed effect absorption
 - Nonlinear functions of product characteristics
 - Concentrating out linear parameters
 - Flexible random coefficient distributions
@@ -133,14 +134,15 @@
 - Random coefficients nested logit (RCNL)
 - Approximation to the pure characteristics model
 - Varying nesting parameters across groups
 - Logit and nested logit benchmarks
 - Classic BLP instruments
 - Differentiation instruments
 - Optimal instruments
+- Covariance restrictions
 - Adjustments for simulation error
 - Tests of overidentifying and model restrictions
 - Parametric boostrapping post-estimation outputs
 - Elasticities and diversion ratios
 - Marginal costs and markups
 - Passthrough calculations
 - Profits and consumer surplus
```

### Comparing `pyblp-1.0.0/pyblp.egg-info/SOURCES.txt` & `pyblp-1.1.0/pyblp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+.gitignore
 LICENSE.txt
 MANIFEST.in
 README.rst
+readthedocs.yml
 requirements.txt
 setup.cfg
 setup.py
+tox.ini
 docs/api.rst
 docs/background.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
 docs/introduction.rst
 docs/legal.rst
```

### Comparing `pyblp-1.0.0/README.rst` & `pyblp-1.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,15 @@
 --------
 
 - R-style formula interface
 - Bertrand-Nash supply-side moments
 - Multiple equation GMM
 - Demographic interactions
 - Product-specific demographics
+- Consumer-specific product availability
 - Flexible micro moments that can match statistics based on survey data
 - Support for micro moments based on second choice data
 - Support for optimal micro moments that match micro data scores
 - Fixed effect absorption
 - Nonlinear functions of product characteristics
 - Concentrating out linear parameters
 - Flexible random coefficient distributions
@@ -128,14 +129,15 @@
 - Random coefficients nested logit (RCNL)
 - Approximation to the pure characteristics model
 - Varying nesting parameters across groups
 - Logit and nested logit benchmarks
 - Classic BLP instruments
 - Differentiation instruments
 - Optimal instruments
+- Covariance restrictions
 - Adjustments for simulation error
 - Tests of overidentifying and model restrictions
 - Parametric boostrapping post-estimation outputs
 - Elasticities and diversion ratios
 - Marginal costs and markups
 - Passthrough calculations
 - Profits and consumer surplus
```

### Comparing `pyblp-1.0.0/setup.py` & `pyblp-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/tests/conftest.py` & `pyblp-1.1.0/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,20 +115,28 @@
             'firm_ids': id_data.firm_ids,
             'clustering_ids': np.random.RandomState(2).choice(range(30), id_data.size)
         },
         beta=[1, -6, 1, 2, 3],
         gamma=[0.1, 0.2, 0.3, -0.2],
         xi_variance=0.00001,
         omega_variance=0.00001,
-        correlation=0.1,
+        correlation=0,
         costs_type='log',
         seed=2
     )
     simulation_results = simulation.replace_endogenous(constant_costs=False)
-    return simulation, simulation_results, {}, []
+
+    demand_instruments, supply_instruments = simulation_results._compute_default_instruments()
+    simulated_data_override = {
+        'demand_instruments': demand_instruments,
+        'supply_instruments': supply_instruments,
+        'covariance_instruments': np.ones(simulation.N),
+    }
+
+    return simulation, simulation_results, simulated_data_override, []
 
 
 @pytest.fixture(scope='session')
 def small_nested_logit_simulation() -> SimulationFixture:
     """Solve a simulation with four markets, linear prices, two linear characteristics, two cost characteristics, and
     two nesting groups with different nesting parameters.
     """
@@ -222,14 +230,29 @@
 @pytest.fixture(scope='session')
 def medium_blp_simulation() -> SimulationFixture:
     """Solve a simulation with four markets, linear/nonlinear/cost constants, two linear characteristics, two cost
     characteristics, a demographic interacted with second-degree prices, an alternative ownership structure, and a
     scaled epsilon.
     """
     id_data = build_id_data(T=10, J=25, F=6)
+
+    integration = Integration('product', 4)
+    agent_data = build_integration(integration, 2)
+    unique_market_ids = np.unique(id_data.market_ids)
+    max_J = max(i.size for i in get_indices(id_data.market_ids).values())
+
+    state = np.random.RandomState(2)
+    availability = {}
+    for j in range(max_J):
+        availability[f'availability{j}'] = state.choice(
+            [0, 0.5, 1],
+            p=[0.05, 0.05, 0.9],
+            size=unique_market_ids.size * agent_data.weights.size,
+        )
+
     simulation = Simulation(
         product_formulations=(
             Formulation('1 + x + prices'),
             Formulation('1 + I(prices**2)'),
             Formulation('1 + a + b')
         ),
         product_data={
@@ -245,23 +268,36 @@
         ],
         pi=[
             [+0.0],
             [-0.1]
         ],
         gamma=[1, 1, 2],
         agent_formulation=Formulation('0 + f'),
-        integration=Integration('product', 4),
+        agent_data={
+            'market_ids': np.repeat(unique_market_ids, agent_data.weights.size),
+            'agent_ids': np.tile(np.arange(agent_data.weights.size), unique_market_ids.size),
+            'weights': np.tile(agent_data.weights.flat, unique_market_ids.size),
+            'nodes': np.tile(agent_data.nodes, (unique_market_ids.size, 1)),
+            **availability,
+        },
         xi_variance=0.00001,
         omega_variance=0.00001,
         correlation=0.8,
         epsilon_scale=0.7,
         seed=1,
     )
     simulation_results = simulation.replace_endogenous()
 
+    demand_instruments, supply_instruments = simulation_results._compute_default_instruments()
+    simulated_data_override = {
+        'demand_instruments': demand_instruments,
+        'supply_instruments': supply_instruments,
+        'covariance_instruments': build_matrix(Formulation('0 + x + a'), simulation.product_data),
+    }
+
     simulated_micro_moments = replace_micro_moment_values(simulation_results, [MicroMoment(
         name="demographic interaction",
         value=0,
         parts=MicroPart(
             name="demographic interaction",
             dataset=MicroDataset(
                 name="inside",
@@ -269,15 +305,15 @@
                 compute_weights=lambda _, p, a: np.ones((a.size, p.size)),
                 market_ids=[simulation.unique_market_ids[2]],
             ),
             compute_values=lambda _, p, a: p.X2[:, [0]].T * a.demographics[:, [0]],
         ),
     )])
 
-    return simulation, simulation_results, {}, simulated_micro_moments
+    return simulation, simulation_results, simulated_data_override, simulated_micro_moments
 
 
 @pytest.fixture(scope='session')
 def large_blp_simulation() -> SimulationFixture:
     """Solve a simulation with 20 markets, varying numbers of products per market, a linear constant, log-linear
     coefficients on prices, a linear/nonlinear/cost characteristic, another three linear characteristics, another two
     cost characteristics, demographics interacted with prices and the linear/nonlinear/cost characteristic, dense
@@ -519,14 +555,24 @@
 
     integration = Integration('product', 4)
     agent_data = build_integration(integration, 2)
     unique_market_ids = np.unique(id_data.market_ids)
     max_J = max(i.size for i in get_indices(id_data.market_ids).values())
 
     state = np.random.RandomState(2)
+    demographics = {}
+    availability = {}
+    for j in range(max_J):
+        demographics[f'g{j}'] = state.uniform(size=unique_market_ids.size * agent_data.weights.size)
+        availability[f'availability{j}'] = state.choice(
+            [0.5, 1],
+            p=[0.2, 0.8],
+            size=unique_market_ids.size * agent_data.weights.size,
+        )
+
     simulation = Simulation(
         product_formulations=(
             Formulation('1 + x + y + z + q'),
             Formulation('0 + I(-prices) + x'),
             Formulation('0 + log(x) + log(a) + log(b)')
         ),
         product_data={
@@ -537,15 +583,16 @@
             'clustering_ids': state.choice(range(30), id_data.size),
         },
         agent_data={
             'market_ids': np.repeat(unique_market_ids, agent_data.weights.size),
             'agent_ids': np.tile(np.arange(agent_data.weights.size), unique_market_ids.size),
             'weights': np.tile(agent_data.weights.flat, unique_market_ids.size),
             'nodes': np.tile(agent_data.nodes, (unique_market_ids.size, 1)),
-            **{f'g{j}': state.uniform(size=unique_market_ids.size * agent_data.weights.size) for j in range(max_J)},
+            **demographics,
+            **availability,
         },
         beta=[1, 1, 2, 3, 1],
         sigma=[
             [0.5, 0],
             [0.0, 2]
         ],
         pi=[
```

### Comparing `pyblp-1.0.0/tests/test_blp.py` & `pyblp-1.1.0/tests/test_blp.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from .conftest import SimulatedProblemFixture
 
 
 @pytest.mark.usefixtures('simulated_problem')
 @pytest.mark.parametrize('solve_options_update', [
     pytest.param({'method': '2s'}, id="two-step"),
     pytest.param({'scale_objective': True}, id="scaled objective"),
+    pytest.param({'covariance_moments_mean': 1e-14}, id="tiny covariance moments mean"),
     pytest.param({'center_moments': False, 'W_type': 'unadjusted', 'se_type': 'clustered'}, id="complex covariances"),
     pytest.param({'delta_behavior': 'last'}, id="faster starting delta values"),
     pytest.param({'delta_behavior': 'logit'}, id="logit starting delta values"),
     pytest.param({'fp_type': 'linear'}, id="non-safe linear fixed point"),
     pytest.param({'fp_type': 'safe_nonlinear'}, id="nonlinear fixed point"),
     pytest.param({'fp_type': 'nonlinear'}, id="non-safe nonlinear fixed point"),
     pytest.param(
@@ -51,14 +52,18 @@
 
     # skip different iteration configurations when they won't matter
     if simulation.K2 == 0 and {'delta_behavior', 'fp_type', 'iteration'} & set(solve_options_update):
         return pytest.skip("A different iteration configuration has no impact when there is no heterogeneity.")
     if simulation.epsilon_scale != 1 and 'nonlinear' in solve_options_update.get('fp_type', 'safe_linear'):
         return pytest.skip("Nonlinear fixed point configurations are not supported when epsilon is scaled.")
 
+    # skip the covariance moments value difference when it doesn't matter
+    if 'covariance_moments_mean' in solve_options_update and (problem.K3 == 0 or problem.MC == 0):
+        return pytest.skip("There is nothing to test with the covariance moments mean with no covariance moments.")
+
     # update the default options and solve the problem
     updated_solve_options = copy.deepcopy(solve_options)
     updated_solve_options.update(solve_options_update)
     updated_solve_options.update({k: 0.5 * solve_options[k] for k in ['sigma', 'pi', 'rho', 'beta']})
     results = problem.solve(**updated_solve_options)
 
     # test the accuracy of the estimated parameters
@@ -396,15 +401,16 @@
     solve_options = copy.deepcopy(solve_options)
     solve_options['optimization'] = Optimization('l-bfgs-b', {'maxfun': 3})
 
     # make product data mutable and add instruments
     product_data = {k: simulation_results.product_data[k] for k in simulation_results.product_data.dtype.names}
     product_data.update({
         'demand_instruments': problem.products.ZD[:, :-problem.K1],
-        'supply_instruments': problem.products.ZS[:, :-problem.K3]
+        'supply_instruments': problem.products.ZS[:, :-problem.K3],
+        'covariance_instruments': problem.products.ZC,
     })
 
     # remove constants and delete associated elements in the initial beta
     product_formulations = list(problem.product_formulations).copy()
     if ED > 0:
         assert product_formulations[0] is not None
         constant_indices = [i for i, e in enumerate(product_formulations[0]._expressions) if not e.free_symbols]
@@ -453,14 +459,15 @@
         product_formulations1, product_data, problem.agent_formulation, simulation.agent_data,
         rc_types=simulation.rc_types, epsilon_scale=simulation.epsilon_scale, costs_type=simulation.costs_type
     )
     if solve_options1['micro_moments']:
         solve_options1['W'] = scipy.linalg.pinv(scipy.linalg.block_diag(
             problem1.products.ZD.T @ problem1.products.ZD,
             problem1.products.ZS.T @ problem1.products.ZS,
+            problem1.products.ZC.T @ problem1.products.ZC,
             np.eye(len(solve_options1['micro_moments'])),
         ))
     problem_results1 = problem1.solve(**solve_options1)
 
     # solve the first stage of a problem in which fixed effects are included as indicator variables
     solve_options2 = copy.deepcopy(solve_options)
     product_formulations2 = product_formulations.copy()
@@ -478,14 +485,15 @@
         solve_options2['beta'],
         np.full((problem2.K1 - solve_options2['beta'].size, 1), np.nan)
     ]
     if solve_options2['micro_moments']:
         solve_options2['W'] = scipy.linalg.pinv(scipy.linalg.block_diag(
             problem2.products.ZD.T @ problem2.products.ZD,
             problem2.products.ZS.T @ problem2.products.ZS,
+            problem2.products.ZC.T @ problem2.products.ZC,
             np.eye(len(solve_options2['micro_moments'])),
         ))
     problem_results2 = problem2.solve(**solve_options2)
 
     # solve the first stage of a problem in which some fixed effects are absorbed and some are included as indicators
     if ED == ES == 0:
         problem_results3 = problem_results2
@@ -510,14 +518,15 @@
             solve_options3['beta'],
             np.full((problem3.K1 - solve_options3['beta'].size, 1), np.nan)
         ]
         if solve_options3['micro_moments']:
             solve_options3['W'] = scipy.linalg.pinv(scipy.linalg.block_diag(
                 problem3.products.ZD.T @ problem3.products.ZD,
                 problem3.products.ZS.T @ problem3.products.ZS,
+                problem3.products.ZC.T @ problem3.products.ZC,
                 np.eye(len(solve_options3['micro_moments'])),
             ))
         problem_results3 = problem3.solve(**solve_options3)
 
     # compute optimal instruments (use only two draws for speed; accuracy is not a concern here)
     Z_results1 = problem_results1.compute_optimal_instruments(draws=2, seed=0)
     Z_results2 = problem_results2.compute_optimal_instruments(draws=2, seed=0)
@@ -619,15 +628,15 @@
 
     # test single product ownership matrices
     single_ownership = build_ownership(simulation_results.product_data, 'single')
     assert np.nansum(single_ownership) == simulation.N
 
 
 @pytest.mark.usefixtures('simulated_problem')
-def test_costs(simulated_problem: SimulatedProblemFixture) -> None:
+def test_specified_ownership(simulated_problem: SimulatedProblemFixture) -> None:
     """Test that marginal costs computed under specified firm IDs and ownership are the same as costs computed when
     firm IDs and ownership are left unspecified.
     """
     _, simulation_results, _, _, results = simulated_problem
 
     # compute costs in the simplest way possible
     costs1 = results.compute_costs()
@@ -642,14 +651,24 @@
     costs2 = results.compute_costs(firm_ids=simulation_results.product_data.firm_ids)
     costs3 = results.compute_costs(ownership=build_ownership(simulation_results.product_data))
     np.testing.assert_equal(costs1, costs2)
     np.testing.assert_equal(costs1, costs3)
 
 
 @pytest.mark.usefixtures('simulated_problem')
+def test_costs(simulated_problem: SimulatedProblemFixture) -> None:
+    """Test that true marginal costs can be recovered after estimation at the true parameter values. This is essentially
+    a joint test of the zeta-markup approach to computing equilibrium prices and the eta-markup expression.
+    """
+    _, simulation_results, _, _, _ = simulated_problem
+    costs = simulation_results.compute_costs()
+    np.testing.assert_allclose(costs, simulation_results.costs, atol=1e-10, rtol=1e-10)
+
+
+@pytest.mark.usefixtures('simulated_problem')
 @pytest.mark.parametrize('iteration', [
     pytest.param(Iteration('simple', {'atol': 1e-12}, universal_display=True), id="simple"),
     pytest.param(Iteration('hybr', {'xtol': 1e-12, 'ftol': 0}, compute_jacobian=True), id="Powell/LM"),
 ])
 def test_prices(simulated_problem: SimulatedProblemFixture, iteration: Iteration) -> None:
     """Test that equilibrium prices computed with different methods are approximate the same.
     """
@@ -1315,14 +1334,18 @@
     """
     simulation, simulation_results, problem, _, _ = simulated_problem
 
     # skip problems with supply since this test will be the same
     if problem.K3 > 0:
         return pytest.skip("Configurations with supply give the same test.")
 
+    # skip problems with differing product availability
+    if problem.agents.availability.size > 0:
+        return pytest.skip("This test is not supported for differing product availability.")
+
     # select only a few products (if there's nesting, select two from each of two nests)
     J = 4
     small_product_data = simulation_results.product_data[:J].copy()
     small_product_data.shares[:] = np.c_[[0.1, 0.2, 0.3, 0.15]]
     small_product_data.market_ids[:] = simulation.unique_market_ids[0]
     if small_product_data.ownership.size > 0:
         small_product_data = update_matrices(small_product_data, {
@@ -1492,15 +1515,15 @@
 
                 values_list.append(values[tuple(indices)])
 
             part_values.append(np.concatenate(values_list).mean())
 
         # compute the micro values
         value = moment.compute_value(np.array(part_values))
-        np.testing.assert_allclose(moment.value, value, atol=0, rtol=0.01, err_msg=moment)
+        np.testing.assert_allclose(moment.value, value, atol=0, rtol=0.015, err_msg=moment)
 
 
 @pytest.mark.usefixtures('simulated_problem')
 def test_micro_scores(simulated_problem: SimulatedProblemFixture) -> None:
     """Test that true micro scores without any unobserved heterogeneity are zero, and that micro scores with unobserved
     heterogeneity based on micro data are of the same order of magnitude as the truth.
     """
@@ -1581,66 +1604,114 @@
         scores = results.compute_micro_scores(dataset, data, integration)
         means = np.array(scores).mean(axis=1)
         np.testing.assert_allclose(means, true_means, atol=1e-13, rtol=10, err_msg=f'{name}: {dataset}')
 
 
 @pytest.mark.usefixtures('simulated_problem')
 @pytest.mark.parametrize('eliminate', [
-    pytest.param(True, id="linear parameters eliminated"),
-    pytest.param(False, id="linear parameters not eliminated")
+    pytest.param('all', id="all possible linear parameters eliminated"),
+    pytest.param('some', id="some linear parameters eliminated"),
+    pytest.param('no', id="no linear parameters eliminated")
+])
+@pytest.mark.parametrize('fe', [
+    pytest.param(False, id="no FE"),
+    pytest.param(True, id="FE"),
 ])
 @pytest.mark.parametrize('demand', [
     pytest.param(True, id="demand"),
     pytest.param(False, id="no demand")
 ])
 @pytest.mark.parametrize('supply', [
     pytest.param(True, id="supply"),
     pytest.param(False, id="no supply")
 ])
+@pytest.mark.parametrize('covariance', [
+    pytest.param(True, id="covariance"),
+    pytest.param(False, id="no covariance")
+])
 @pytest.mark.parametrize('micro', [
     pytest.param(True, id="micro"),
     pytest.param(False, id="no micro")
 ])
 def test_objective_gradient(
-        simulated_problem: SimulatedProblemFixture, eliminate: bool, demand: bool, supply: bool, micro: bool) -> None:
+        simulated_problem: SimulatedProblemFixture, eliminate: str, fe: bool, demand: bool, supply: bool,
+        covariance: bool, micro: bool) -> None:
     """Implement central finite differences in a custom optimization routine to test that analytic gradient values
     are close to estimated values.
     """
-    simulation, _, problem, solve_options, problem_results = simulated_problem
+    simulation, simulation_results, problem, solve_options, problem_results = simulated_problem
 
     # skip some redundant tests
     if supply and problem.K3 == 0:
         return pytest.skip("The problem does not have supply-side moments to test.")
+    if covariance and (problem.K3 == 0 or problem.MC == 0):
+        return pytest.skip("The problem does not have covariance moments to test.")
     if micro and not solve_options['micro_moments']:
         return pytest.skip("The problem does not have micro moments to test.")
-    if not demand and not supply and not micro:
+    if not demand and not supply and not covariance and not micro:
         return pytest.skip("There are no moments to test.")
 
     # configure the options used to solve the problem
     updated_solve_options = copy.deepcopy(solve_options)
     updated_solve_options.update({k: 0.9 * solve_options[k] for k in ['sigma', 'pi', 'rho', 'beta']})
 
     # optionally include linear parameters in theta
-    if not eliminate:
+    if eliminate == 'no':
+        if problem.K1 > 0:
+            updated_solve_options['beta'] = 0.9 * simulation.beta
+        if problem.K3 > 0:
+            updated_solve_options['gamma'] = 0.9 * simulation.gamma
+    elif eliminate == 'some':
         if problem.K1 > 0:
             updated_solve_options['beta'][-1] = 0.9 * simulation.beta[-1]
         if problem.K3 > 0:
             updated_solve_options['gamma'] = np.full_like(simulation.gamma, np.nan)
             updated_solve_options['gamma'][-1] = 0.9 * simulation.gamma[-1]
+    else:
+        assert eliminate == 'all'
+
+    # optionally add a fixed effect
+    if fe:
+        # make product data mutable and add instruments
+        product_data = {k: simulation_results.product_data[k] for k in simulation_results.product_data.dtype.names}
+        product_data.update({
+            'demand_instruments': problem.products.ZD[:, :-problem.K1],
+            'supply_instruments': problem.products.ZS[:, :-problem.K3],
+            'covariance_instruments': problem.products.ZC,
+        })
+
+        # remove constants and delete associated elements in the initial beta
+        product_formulations = list(problem.product_formulations).copy()
+        assert product_formulations[0] is not None
+        constant_indices = [i for i, e in enumerate(product_formulations[0]._expressions) if not e.free_symbols]
+        updated_solve_options['beta'] = np.delete(updated_solve_options['beta'], constant_indices, axis=0)
+
+        # add fixed effect IDs to the data
+        state = np.random.RandomState(seed=0)
+        ids = state.choice(['a', 'b', 'c'], problem.N)
+        product_data['demand_ids'] = ids
+
+        # update the problem
+        product_formulations[0] = Formulation(f'{product_formulations[0]._formula} - 1', absorb='demand_ids')
+        problem = Problem(
+            product_formulations, product_data, problem.agent_formulation, simulation.agent_data,
+            rc_types=simulation.rc_types, epsilon_scale=simulation.epsilon_scale, costs_type=simulation.costs_type
+        )
 
     # zero out weighting matrix blocks to only test individual contributions of the gradient
-    updated_solve_options['W'] = copy.deepcopy(problem_results.W)
-    if micro:
-        MM = len(updated_solve_options['micro_moments'])
-        updated_solve_options['W'][-MM:, -MM:] = np.eye(MM)
-    updated_solve_options['W'] = np.eye(problem_results.W.shape[0])
+    updated_solve_options['W'] = np.eye(problem.MD + problem.MS + problem.MC + len(solve_options['micro_moments']))
     if not demand:
         updated_solve_options['W'][:problem.MD, :problem.MD] = 0
     if not supply and problem.K3 > 0:
-        updated_solve_options['W'][problem.MD:problem.MD + problem.MS, problem.MD:problem.MD + problem.MS] = 0
+        MDS = problem.MD + problem.MS
+        updated_solve_options['W'][problem.MD:MDS, problem.MD:MDS] = 0
+    if not covariance and problem.K3 > 0:
+        MDS = problem.MD + problem.MS
+        MDSC = MDS + problem.MC
+        updated_solve_options['W'][MDS:MDSC, MDS:MDSC] = 0
     if not micro and updated_solve_options['micro_moments']:
         MM = len(updated_solve_options['micro_moments'])
         updated_solve_options['W'][-MM:, -MM:] = 0
 
     # use a restrictive iteration tolerance
     updated_solve_options['iteration'] = Iteration('squarem', {'atol': 1e-14})
```

### Comparing `pyblp-1.0.0/tests/test_formulation.py` & `pyblp-1.1.0/tests/test_formulation.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/tests/test_integration.py` & `pyblp-1.1.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/tests/test_iteration.py` & `pyblp-1.1.0/tests/test_iteration.py`

 * *Files identical despite different names*

### Comparing `pyblp-1.0.0/tests/test_optimization.py` & `pyblp-1.1.0/tests/test_optimization.py`

 * *Files identical despite different names*

