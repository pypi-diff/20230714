# Comparing `tmp/quickstats-0.6.8.8.tar.gz` & `tmp/quickstats-0.6.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstats-0.6.8.8.tar", last modified: Sat Jul  8 17:04:23 2023, max compression
+gzip compressed data, was "quickstats-0.6.8.9.tar", last modified: Fri Jul 14 09:26:18 2023, max compression
```

## Comparing `quickstats-0.6.8.8.tar` & `quickstats-0.6.8.9.tar`

### file list

```diff
@@ -1,242 +1,242 @@
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2023-01-04 09:02:54.000000 quickstats-0.6.8.8/README.md
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/bin/
--rwxr-xr-x   0 chlcheng (124202) zp        (1307)     1651 2023-05-11 20:22:22.000000 quickstats-0.6.8.8/bin/quickstats
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/quickstats/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      626 2023-05-31 15:23:38.000000 quickstats-0.6.8.8/quickstats/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)       24 2023-07-08 04:42:44.000000 quickstats-0.6.8.8/quickstats/_version.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/quickstats/analysis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2023-02-08 03:42:01.000000 quickstats-0.6.8.8/quickstats/analysis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-02-08 08:27:54.000000 quickstats-0.6.8.8/quickstats/analysis/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4191 2023-02-08 05:24:19.000000 quickstats-0.6.8.8/quickstats/analysis/analysis_path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22807 2023-03-14 14:12:10.000000 quickstats-0.6.8.8/quickstats/analysis/config_format_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    41649 2023-05-20 03:33:19.000000 quickstats-0.6.8.8/quickstats/analysis/data_loading.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1303 2023-01-04 09:02:54.000000 quickstats-0.6.8.8/quickstats/analysis/data_preprocessing.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    85935 2023-05-20 03:34:59.000000 quickstats-0.6.8.8/quickstats/analysis/event_categorization.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8060 2023-01-04 09:02:54.000000 quickstats-0.6.8.8/quickstats/analysis/multi_class_boundary_tree.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9286 2023-05-20 03:35:21.000000 quickstats-0.6.8.8/quickstats/analysis/ntuple_conversion_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    32121 2023-07-07 22:03:31.000000 quickstats-0.6.8.8/quickstats/analysis/ntuple_process_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8897 2023-06-07 14:20:37.000000 quickstats-0.6.8.8/quickstats/analysis/sample_poly_param_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/quickstats/analysis/systematics/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2023-03-07 22:17:53.000000 quickstats-0.6.8.8/quickstats/analysis/systematics/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29560 2023-07-07 22:04:35.000000 quickstats-0.6.8.8/quickstats/analysis/systematics/base_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9774 2023-04-03 12:27:59.000000 quickstats-0.6.8.8/quickstats/analysis/systematics/gaussian_shape_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6796 2023-03-14 18:47:57.000000 quickstats-0.6.8.8/quickstats/analysis/systematics/normalization_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11869 2023-07-07 22:04:22.000000 quickstats-0.6.8.8/quickstats/analysis/systematics/systematics_evaluation_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/clis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-05-17 11:53:22.000000 quickstats-0.6.8.8/quickstats/clis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    35406 2023-06-08 10:16:18.000000 quickstats-0.6.8.8/quickstats/clis/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2174 2023-02-14 22:30:46.000000 quickstats-0.6.8.8/quickstats/clis/inspect_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2023-02-14 22:27:47.000000 quickstats-0.6.8.8/quickstats/clis/inspect_ws.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16785 2023-06-05 09:37:42.000000 quickstats-0.6.8.8/quickstats/clis/likelihood_fit.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7980 2023-06-26 09:38:29.000000 quickstats-0.6.8.8/quickstats/clis/likelihood_scan.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8575 2023-01-04 09:02:54.000000 quickstats-0.6.8.8/quickstats/clis/limit_setting.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1512 2023-06-13 21:11:53.000000 quickstats-0.6.8.8/quickstats/clis/processor_cli.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15259 2023-06-13 03:13:49.000000 quickstats-0.6.8.8/quickstats/clis/workspace_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/components/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      849 2023-05-30 19:49:31.000000 quickstats-0.6.8.8/quickstats/components/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3152 2023-05-27 07:22:07.000000 quickstats-0.6.8.8/quickstats/components/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13357 2023-07-07 21:51:04.000000 quickstats-0.6.8.8/quickstats/components/analysis_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7333 2023-06-08 10:12:47.000000 quickstats-0.6.8.8/quickstats/components/asimov_generator.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    30804 2023-05-20 02:55:29.000000 quickstats-0.6.8.8/quickstats/components/asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2464 2023-01-04 09:02:54.000000 quickstats-0.6.8.8/quickstats/components/basics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    31916 2023-06-07 11:32:50.000000 quickstats-0.6.8.8/quickstats/components/extended_minimizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)   102824 2023-07-08 04:44:50.000000 quickstats-0.6.8.8/quickstats/components/extended_model.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5542 2023-07-07 21:58:36.000000 quickstats-0.6.8.8/quickstats/components/extended_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14934 2023-07-04 00:19:59.000000 quickstats-0.6.8.8/quickstats/components/likelihood.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/components/modelling/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.6.8.8/quickstats/components/modelling/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2520 2022-09-18 05:43:28.000000 quickstats-0.6.8.8/quickstats/components/modelling/component_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20157 2023-05-20 03:06:27.000000 quickstats-0.6.8.8/quickstats/components/modelling/data_modelling.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      767 2022-09-18 12:07:18.000000 quickstats-0.6.8.8/quickstats/components/modelling/model_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4562 2022-09-18 16:32:35.000000 quickstats-0.6.8.8/quickstats/components/modelling/parameter_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5578 2023-05-20 03:07:18.000000 quickstats-0.6.8.8/quickstats/components/modelling/pdf_fit_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3532 2023-05-20 03:07:28.000000 quickstats-0.6.8.8/quickstats/components/modelling/tree_data_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10888 2023-07-03 21:42:51.000000 quickstats-0.6.8.8/quickstats/components/nuisance_parameter_harmonizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    17463 2023-07-07 22:11:31.000000 quickstats-0.6.8.8/quickstats/components/nuisance_parameter_pull.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12396 2023-07-07 22:07:20.000000 quickstats-0.6.8.8/quickstats/components/nuisance_parameter_ranking.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/components/processors/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      205 2022-07-19 21:07:01.000000 quickstats-0.6.8.8/quickstats/components/processors/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2066 2023-05-19 15:52:58.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2022-07-21 18:27:25.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/auxiliary.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1072 2023-03-05 12:07:49.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1082 2022-07-19 21:51:30.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_as_numpy.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2666 2023-07-07 21:51:37.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_base_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      784 2023-05-21 22:53:11.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_declare.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      870 2023-05-23 18:53:54.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1154 2023-06-03 14:06:41.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_export.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1164 2022-07-21 15:20:21.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_filter.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1250 2023-06-13 21:07:45.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_global_variables.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_helper_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_hybrid_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      697 2022-07-21 18:29:41.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_if_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      704 2022-07-21 18:48:13.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_if_not_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-19 21:50:41.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_load_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1121 2023-05-21 22:55:55.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_load_macro.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:20.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_max.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      142 2022-07-19 20:41:10.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_mean.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:51.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_min.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_nested_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_rdf_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2022-07-19 20:28:28.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_redefine.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1677 2023-05-22 21:51:19.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_report.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1382 2023-03-05 12:11:04.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_safe_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      454 2022-07-19 20:28:24.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_safe_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2129 2023-06-03 16:04:25.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_save.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      645 2023-06-03 14:13:00.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_save_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1194 2022-07-19 21:50:00.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_stat.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:39:49.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_sum.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      523 2022-07-19 21:54:23.000000 quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_treename.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9969 2023-06-05 23:09:50.000000 quickstats-0.6.8.8/quickstats/components/processors/builtin_methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6504 2023-05-21 22:51:45.000000 quickstats-0.6.8.8/quickstats/components/processors/roo_config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6788 2023-07-07 21:53:01.000000 quickstats-0.6.8.8/quickstats/components/processors/roo_processor.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5397 2021-09-16 21:06:55.000000 quickstats-0.6.8.8/quickstats/components/pvalue_toys.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3551 2023-07-07 21:53:49.000000 quickstats-0.6.8.8/quickstats/components/roo_inspector.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3083 2023-05-20 03:04:47.000000 quickstats-0.6.8.8/quickstats/components/root_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21336 2023-05-20 03:06:10.000000 quickstats-0.6.8.8/quickstats/components/toy_limit_calculator.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/components/workspaces/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2023-05-11 12:58:08.000000 quickstats-0.6.8.8/quickstats/components/workspaces/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2023-05-20 03:10:01.000000 quickstats-0.6.8.8/quickstats/components/workspaces/asimov_handler.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2023-05-20 03:10:09.000000 quickstats-0.6.8.8/quickstats/components/workspaces/core_argument_sets.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2023-01-09 17:03:21.000000 quickstats-0.6.8.8/quickstats/components/workspaces/sample.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2023-03-11 17:09:50.000000 quickstats-0.6.8.8/quickstats/components/workspaces/settings.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8295 2023-05-20 03:10:27.000000 quickstats-0.6.8.8/quickstats/components/workspaces/systematic.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2023-01-08 18:43:45.000000 quickstats-0.6.8.8/quickstats/components/workspaces/systematics_domain.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    53162 2023-06-06 14:20:25.000000 quickstats-0.6.8.8/quickstats/components/workspaces/ws_comparer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8837 2023-05-20 03:11:35.000000 quickstats-0.6.8.8/quickstats/components/workspaces/ws_decomposer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1756 2022-04-20 13:20:42.000000 quickstats-0.6.8.8/quickstats/components/workspaces/ws_modifier_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10859 2023-05-20 03:12:06.000000 quickstats-0.6.8.8/quickstats/components/workspaces/xml_ws_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    87030 2023-05-20 03:16:06.000000 quickstats-0.6.8.8/quickstats/components/workspaces/xml_ws_builder_v1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    76213 2023-05-20 03:19:36.000000 quickstats-0.6.8.8/quickstats/components/workspaces/xml_ws_builder_v2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    45869 2023-07-07 21:58:59.000000 quickstats-0.6.8.8/quickstats/components/workspaces/xml_ws_combiner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    49268 2023-07-08 04:44:49.000000 quickstats-0.6.8.8/quickstats/components/workspaces/xml_ws_modifier.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/concurrent/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      306 2023-05-31 15:27:50.000000 quickstats-0.6.8.8/quickstats/concurrent/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3379 2023-06-26 09:41:33.000000 quickstats-0.6.8.8/quickstats/concurrent/abstract_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.6.8.8/quickstats/concurrent/logging.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5239 2023-05-31 16:02:49.000000 quickstats-0.6.8.8/quickstats/concurrent/nuisance_parameter_ranking_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5891 2023-06-10 22:16:28.000000 quickstats-0.6.8.8/quickstats/concurrent/parameterised_asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10758 2023-06-28 16:38:35.000000 quickstats-0.6.8.8/quickstats/concurrent/parameterised_likelihood.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3963 2023-05-31 15:27:15.000000 quickstats-0.6.8.8/quickstats/concurrent/parameterised_runner.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/core/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2023-01-04 09:02:55.000000 quickstats-0.6.8.8/quickstats/core/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      811 2023-01-04 09:02:55.000000 quickstats-0.6.8.8/quickstats/core/abstract_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20587 2023-05-20 03:28:17.000000 quickstats-0.6.8.8/quickstats/core/configs.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2198 2023-01-04 09:02:55.000000 quickstats-0.6.8.8/quickstats/core/configurable_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      541 2023-01-04 09:02:55.000000 quickstats-0.6.8.8/quickstats/core/dataclass_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      971 2023-05-20 03:27:42.000000 quickstats-0.6.8.8/quickstats/core/decorators.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2296 2023-05-23 21:10:32.000000 quickstats-0.6.8.8/quickstats/core/enums.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6651 2023-02-14 22:36:19.000000 quickstats-0.6.8.8/quickstats/core/methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9057 2023-02-08 05:24:13.000000 quickstats-0.6.8.8/quickstats/core/path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2952 2022-07-21 15:05:33.000000 quickstats-0.6.8.8/quickstats/core/virtual_trees.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/interface/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       66 2023-05-31 15:27:05.000000 quickstats-0.6.8.8/quickstats/interface/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/interface/cppyy/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2023-05-31 20:08:24.000000 quickstats-0.6.8.8/quickstats/interface/cppyy/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2022-01-31 03:37:54.000000 quickstats-0.6.8.8/quickstats/interface/cppyy/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12546 2023-05-28 20:56:33.000000 quickstats-0.6.8.8/quickstats/interface/cppyy/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4433 2023-01-04 09:02:55.000000 quickstats-0.6.8.8/quickstats/interface/cppyy/vectorize.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/interface/root/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.6.8.8/quickstats/interface/root/RooAbsData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9855 2023-05-20 12:12:25.000000 quickstats-0.6.8.8/quickstats/interface/root/RooAbsPdf.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      420 2022-08-23 02:59:13.000000 quickstats-0.6.8.8/quickstats/interface/root/RooArgSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2023-03-12 16:17:52.000000 quickstats-0.6.8.8/quickstats/interface/root/RooCategory.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    44679 2023-05-20 12:08:58.000000 quickstats-0.6.8.8/quickstats/interface/root/RooDataSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.6.8.8/quickstats/interface/root/RooMsgService.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5451 2023-05-11 15:17:32.000000 quickstats-0.6.8.8/quickstats/interface/root/RooRealVar.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.6.8.8/quickstats/interface/root/TArrayData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2023-01-04 09:02:55.000000 quickstats-0.6.8.8/quickstats/interface/root/TF1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1995 2023-02-28 09:57:47.000000 quickstats-0.6.8.8/quickstats/interface/root/TFile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2023-05-20 12:06:46.000000 quickstats-0.6.8.8/quickstats/interface/root/TH1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5707 2023-05-03 13:36:36.000000 quickstats-0.6.8.8/quickstats/interface/root/TH2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      571 2022-08-23 03:14:20.000000 quickstats-0.6.8.8/quickstats/interface/root/TObject.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      856 2023-03-12 13:27:02.000000 quickstats-0.6.8.8/quickstats/interface/root/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.6.8.8/quickstats/interface/root/helper.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-03-24 19:40:20.000000 quickstats-0.6.8.8/quickstats/interface/root/inspection.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.6.8.8/quickstats/interface/root/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    19576 2023-05-11 13:39:17.000000 quickstats-0.6.8.8/quickstats/interface/root/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5637 2023-05-27 06:13:47.000000 quickstats-0.6.8.8/quickstats/interface/root/roofit_extension.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/quickstats/macros/
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/macros/AsymptoticCLsTool/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7083 2021-08-19 17:39:48.000000 quickstats-0.6.8.8/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1511 2021-06-11 19:36:10.000000 quickstats-0.6.8.8/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/macros/FlexibleInterpVarMkII/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.6.8.8/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.6.8.8/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/macros/QuickStatsCore/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1231 2022-05-07 02:55:05.000000 quickstats-0.6.8.8/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10322 2022-05-11 00:00:32.000000 quickstats-0.6.8.8/quickstats/macros/QuickStatsCore/RooFitExt.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3429 2022-05-10 23:59:25.000000 quickstats-0.6.8.8/quickstats/macros/QuickStatsCore/RooFitExt.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/macros/ResponseFunction/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13755 2023-04-25 19:09:18.000000 quickstats-0.6.8.8/quickstats/macros/ResponseFunction/ResponseFunction.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.6.8.8/quickstats/macros/ResponseFunction/ResponseFunction.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/macros/RooTwoSidedCBShape/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.6.8.8/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.6.8.8/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/maths/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.6.8.8/quickstats/maths/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2093 2023-06-21 12:10:05.000000 quickstats-0.6.8.8/quickstats/maths/interpolation.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5548 2023-03-30 08:30:53.000000 quickstats-0.6.8.8/quickstats/maths/numerics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    28267 2023-07-08 04:40:34.000000 quickstats-0.6.8.8/quickstats/maths/statistics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2023-05-15 01:04:06.000000 quickstats-0.6.8.8/quickstats/maths/statistics_jitted.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.6.8.8/quickstats/maths/symbolics.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/parsers/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      113 2022-04-20 10:58:59.000000 quickstats-0.6.8.8/quickstats/parsers/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.6.8.8/quickstats/parsers/config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15916 2023-07-07 22:02:29.000000 quickstats-0.6.8.8/quickstats/parsers/param_parser.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/plots/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1441 2023-03-29 12:38:13.000000 quickstats-0.6.8.8/quickstats/plots/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14389 2023-06-21 01:49:40.000000 quickstats-0.6.8.8/quickstats/plots/abstract_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14145 2023-03-29 14:21:34.000000 quickstats-0.6.8.8/quickstats/plots/bidirectional_bar_chart.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.6.8.8/quickstats/plots/collective_data_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2750 2023-04-01 10:15:48.000000 quickstats-0.6.8.8/quickstats/plots/color_schemes.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5180 2023-05-17 15:59:58.000000 quickstats-0.6.8.8/quickstats/plots/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4007 2023-05-17 16:00:48.000000 quickstats-0.6.8.8/quickstats/plots/correlation_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6018 2023-07-03 18:31:57.000000 quickstats-0.6.8.8/quickstats/plots/general_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22775 2022-09-07 07:18:02.000000 quickstats-0.6.8.8/quickstats/plots/general_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3731 2022-09-09 08:30:51.000000 quickstats-0.6.8.8/quickstats/plots/histo_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6100 2023-03-21 16:34:42.000000 quickstats-0.6.8.8/quickstats/plots/hypotest_inverter_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8917 2023-07-04 13:41:54.000000 quickstats-0.6.8.8/quickstats/plots/likelihood_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14929 2023-07-08 03:46:17.000000 quickstats-0.6.8.8/quickstats/plots/likelihood_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      219 2021-04-19 13:56:55.000000 quickstats-0.6.8.8/quickstats/plots/likelihood_scan_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29009 2023-05-31 19:45:49.000000 quickstats-0.6.8.8/quickstats/plots/np_ranking_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    25696 2023-04-18 01:26:39.000000 quickstats-0.6.8.8/quickstats/plots/pdf_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5059 2023-02-06 09:15:46.000000 quickstats-0.6.8.8/quickstats/plots/sample_purity_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10293 2023-03-27 13:06:51.000000 quickstats-0.6.8.8/quickstats/plots/score_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4123 2023-01-04 09:02:56.000000 quickstats-0.6.8.8/quickstats/plots/stat_plot_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18642 2023-04-02 13:33:12.000000 quickstats-0.6.8.8/quickstats/plots/template.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13688 2022-07-29 18:50:11.000000 quickstats-0.6.8.8/quickstats/plots/test_statistic_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11061 2023-01-04 09:02:56.000000 quickstats-0.6.8.8/quickstats/plots/upper_limit_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    17787 2023-06-21 01:00:28.000000 quickstats-0.6.8.8/quickstats/plots/upper_limit_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12201 2023-06-19 12:52:28.000000 quickstats-0.6.8.8/quickstats/plots/upper_limit_2D_plot_deprecated.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13186 2022-08-18 13:35:04.000000 quickstats-0.6.8.8/quickstats/plots/upper_limit_3D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16450 2023-06-21 14:06:12.000000 quickstats-0.6.8.8/quickstats/plots/upper_limit_benchmark_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29707 2023-06-27 09:55:20.000000 quickstats-0.6.8.8/quickstats/plots/variable_distribution_plot.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/resources/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2023-03-20 15:25:27.000000 quickstats-0.6.8.8/quickstats/resources/default_workspace_extensions.json
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-04-08 03:20:04.000000 quickstats-0.6.8.8/quickstats/root_checker.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/stylesheets/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2021-10-20 08:52:20.000000 quickstats-0.6.8.8/quickstats/stylesheets/quick_default.mplstyle
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/quickstats/utils/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.6.8.8/quickstats/utils/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11009 2023-07-07 22:00:44.000000 quickstats-0.6.8.8/quickstats/utils/common_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.6.8.8/quickstats/utils/condor_tasks.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    17089 2023-06-04 03:39:00.000000 quickstats-0.6.8.8/quickstats/utils/data_conversion.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.6.8.8/quickstats/utils/hep_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6812 2023-05-31 13:27:25.000000 quickstats-0.6.8.8/quickstats/utils/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      335 2021-05-17 13:11:29.000000 quickstats-0.6.8.8/quickstats/utils/process_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    26262 2023-06-07 15:13:35.000000 quickstats-0.6.8.8/quickstats/utils/roofit_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9267 2021-11-23 21:10:48.000000 quickstats-0.6.8.8/quickstats/utils/roostats_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12379 2023-07-07 22:00:16.000000 quickstats-0.6.8.8/quickstats/utils/root_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1448 2023-07-08 03:51:23.000000 quickstats-0.6.8.8/quickstats/utils/string_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15023 2023-07-07 22:01:35.000000 quickstats-0.6.8.8/quickstats/utils/xml_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/quickstats.egg-info/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/quickstats.egg-info/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9130 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/quickstats.egg-info/SOURCES.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/quickstats.egg-info/dependency_links.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/quickstats.egg-info/requires.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2023-07-08 17:04:22.000000 quickstats-0.6.8.8/quickstats.egg-info/top_level.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2023-07-08 17:04:23.000000 quickstats-0.6.8.8/setup.cfg
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1687 2023-01-04 09:02:56.000000 quickstats-0.6.8.8/setup.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:18.000000 quickstats-0.6.8.9/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-07-14 09:26:18.000000 quickstats-0.6.8.9/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2023-01-04 09:02:54.000000 quickstats-0.6.8.9/README.md
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:12.000000 quickstats-0.6.8.9/bin/
+-rwxr-xr-x   0 chlcheng (124202) zp        (1307)     1651 2023-05-11 20:22:22.000000 quickstats-0.6.8.9/bin/quickstats
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:12.000000 quickstats-0.6.8.9/quickstats/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      626 2023-05-31 15:23:38.000000 quickstats-0.6.8.9/quickstats/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       24 2023-07-13 23:45:35.000000 quickstats-0.6.8.9/quickstats/_version.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:12.000000 quickstats-0.6.8.9/quickstats/analysis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2023-02-08 03:42:01.000000 quickstats-0.6.8.9/quickstats/analysis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-02-08 08:27:54.000000 quickstats-0.6.8.9/quickstats/analysis/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4191 2023-02-08 05:24:19.000000 quickstats-0.6.8.9/quickstats/analysis/analysis_path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22807 2023-03-14 14:12:10.000000 quickstats-0.6.8.9/quickstats/analysis/config_format_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    41649 2023-05-20 03:33:19.000000 quickstats-0.6.8.9/quickstats/analysis/data_loading.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1303 2023-01-04 09:02:54.000000 quickstats-0.6.8.9/quickstats/analysis/data_preprocessing.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    85935 2023-05-20 03:34:59.000000 quickstats-0.6.8.9/quickstats/analysis/event_categorization.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8060 2023-01-04 09:02:54.000000 quickstats-0.6.8.9/quickstats/analysis/multi_class_boundary_tree.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9286 2023-05-20 03:35:21.000000 quickstats-0.6.8.9/quickstats/analysis/ntuple_conversion_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    32121 2023-07-07 22:03:31.000000 quickstats-0.6.8.9/quickstats/analysis/ntuple_process_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8897 2023-06-07 14:20:37.000000 quickstats-0.6.8.9/quickstats/analysis/sample_poly_param_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:12.000000 quickstats-0.6.8.9/quickstats/analysis/systematics/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2023-03-07 22:17:53.000000 quickstats-0.6.8.9/quickstats/analysis/systematics/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29560 2023-07-07 22:04:35.000000 quickstats-0.6.8.9/quickstats/analysis/systematics/base_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9774 2023-04-03 12:27:59.000000 quickstats-0.6.8.9/quickstats/analysis/systematics/gaussian_shape_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6796 2023-03-14 18:47:57.000000 quickstats-0.6.8.9/quickstats/analysis/systematics/normalization_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11869 2023-07-07 22:04:22.000000 quickstats-0.6.8.9/quickstats/analysis/systematics/systematics_evaluation_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:13.000000 quickstats-0.6.8.9/quickstats/clis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-05-17 11:53:22.000000 quickstats-0.6.8.9/quickstats/clis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    35538 2023-07-13 11:58:34.000000 quickstats-0.6.8.9/quickstats/clis/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2174 2023-02-14 22:30:46.000000 quickstats-0.6.8.9/quickstats/clis/inspect_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2023-02-14 22:27:47.000000 quickstats-0.6.8.9/quickstats/clis/inspect_ws.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16785 2023-06-05 09:37:42.000000 quickstats-0.6.8.9/quickstats/clis/likelihood_fit.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7980 2023-06-26 09:38:29.000000 quickstats-0.6.8.9/quickstats/clis/likelihood_scan.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8575 2023-01-04 09:02:54.000000 quickstats-0.6.8.9/quickstats/clis/limit_setting.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1512 2023-06-13 21:11:53.000000 quickstats-0.6.8.9/quickstats/clis/processor_cli.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15259 2023-06-13 03:13:49.000000 quickstats-0.6.8.9/quickstats/clis/workspace_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:13.000000 quickstats-0.6.8.9/quickstats/components/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      849 2023-05-30 19:49:31.000000 quickstats-0.6.8.9/quickstats/components/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3152 2023-05-27 07:22:07.000000 quickstats-0.6.8.9/quickstats/components/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13357 2023-07-07 21:51:04.000000 quickstats-0.6.8.9/quickstats/components/analysis_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7333 2023-06-08 10:12:47.000000 quickstats-0.6.8.9/quickstats/components/asimov_generator.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    30804 2023-05-20 02:55:29.000000 quickstats-0.6.8.9/quickstats/components/asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2464 2023-01-04 09:02:54.000000 quickstats-0.6.8.9/quickstats/components/basics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    31916 2023-06-07 11:32:50.000000 quickstats-0.6.8.9/quickstats/components/extended_minimizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)   102824 2023-07-08 04:44:50.000000 quickstats-0.6.8.9/quickstats/components/extended_model.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5542 2023-07-07 21:58:36.000000 quickstats-0.6.8.9/quickstats/components/extended_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13996 2023-07-12 12:32:58.000000 quickstats-0.6.8.9/quickstats/components/likelihood.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:13.000000 quickstats-0.6.8.9/quickstats/components/modelling/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.6.8.9/quickstats/components/modelling/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2520 2022-09-18 05:43:28.000000 quickstats-0.6.8.9/quickstats/components/modelling/component_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20157 2023-05-20 03:06:27.000000 quickstats-0.6.8.9/quickstats/components/modelling/data_modelling.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      767 2022-09-18 12:07:18.000000 quickstats-0.6.8.9/quickstats/components/modelling/model_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4562 2022-09-18 16:32:35.000000 quickstats-0.6.8.9/quickstats/components/modelling/parameter_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5578 2023-05-20 03:07:18.000000 quickstats-0.6.8.9/quickstats/components/modelling/pdf_fit_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3532 2023-05-20 03:07:28.000000 quickstats-0.6.8.9/quickstats/components/modelling/tree_data_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10888 2023-07-03 21:42:51.000000 quickstats-0.6.8.9/quickstats/components/nuisance_parameter_harmonizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17463 2023-07-07 22:11:31.000000 quickstats-0.6.8.9/quickstats/components/nuisance_parameter_pull.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12396 2023-07-07 22:07:20.000000 quickstats-0.6.8.9/quickstats/components/nuisance_parameter_ranking.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:13.000000 quickstats-0.6.8.9/quickstats/components/processors/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      205 2022-07-19 21:07:01.000000 quickstats-0.6.8.9/quickstats/components/processors/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:14.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2066 2023-05-19 15:52:58.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2022-07-21 18:27:25.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/auxiliary.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1072 2023-03-05 12:07:49.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1082 2022-07-19 21:51:30.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_as_numpy.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2666 2023-07-07 21:51:37.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_base_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      784 2023-05-21 22:53:11.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_declare.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      870 2023-05-23 18:53:54.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1154 2023-06-03 14:06:41.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_export.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1164 2022-07-21 15:20:21.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_filter.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1250 2023-06-13 21:07:45.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_global_variables.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_helper_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_hybrid_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      697 2022-07-21 18:29:41.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_if_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      704 2022-07-21 18:48:13.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_if_not_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-19 21:50:41.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_load_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1121 2023-05-21 22:55:55.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_load_macro.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:20.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_max.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      142 2022-07-19 20:41:10.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_mean.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:51.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_min.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_nested_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_rdf_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2022-07-19 20:28:28.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_redefine.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1677 2023-05-22 21:51:19.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_report.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1382 2023-03-05 12:11:04.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_safe_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      454 2022-07-19 20:28:24.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_safe_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2129 2023-06-03 16:04:25.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_save.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      645 2023-06-03 14:13:00.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_save_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1194 2022-07-19 21:50:00.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_stat.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:39:49.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_sum.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      523 2022-07-19 21:54:23.000000 quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_treename.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9969 2023-06-05 23:09:50.000000 quickstats-0.6.8.9/quickstats/components/processors/builtin_methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6504 2023-05-21 22:51:45.000000 quickstats-0.6.8.9/quickstats/components/processors/roo_config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6792 2023-07-12 23:26:18.000000 quickstats-0.6.8.9/quickstats/components/processors/roo_processor.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5397 2021-09-16 21:06:55.000000 quickstats-0.6.8.9/quickstats/components/pvalue_toys.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3551 2023-07-07 21:53:49.000000 quickstats-0.6.8.9/quickstats/components/roo_inspector.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3083 2023-05-20 03:04:47.000000 quickstats-0.6.8.9/quickstats/components/root_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21336 2023-05-20 03:06:10.000000 quickstats-0.6.8.9/quickstats/components/toy_limit_calculator.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:14.000000 quickstats-0.6.8.9/quickstats/components/workspaces/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2023-05-11 12:58:08.000000 quickstats-0.6.8.9/quickstats/components/workspaces/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2023-05-20 03:10:01.000000 quickstats-0.6.8.9/quickstats/components/workspaces/asimov_handler.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2023-05-20 03:10:09.000000 quickstats-0.6.8.9/quickstats/components/workspaces/core_argument_sets.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2023-01-09 17:03:21.000000 quickstats-0.6.8.9/quickstats/components/workspaces/sample.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2023-03-11 17:09:50.000000 quickstats-0.6.8.9/quickstats/components/workspaces/settings.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8295 2023-05-20 03:10:27.000000 quickstats-0.6.8.9/quickstats/components/workspaces/systematic.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2023-01-08 18:43:45.000000 quickstats-0.6.8.9/quickstats/components/workspaces/systematics_domain.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    53162 2023-06-06 14:20:25.000000 quickstats-0.6.8.9/quickstats/components/workspaces/ws_comparer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8837 2023-05-20 03:11:35.000000 quickstats-0.6.8.9/quickstats/components/workspaces/ws_decomposer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1756 2022-04-20 13:20:42.000000 quickstats-0.6.8.9/quickstats/components/workspaces/ws_modifier_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10859 2023-05-20 03:12:06.000000 quickstats-0.6.8.9/quickstats/components/workspaces/xml_ws_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    87030 2023-05-20 03:16:06.000000 quickstats-0.6.8.9/quickstats/components/workspaces/xml_ws_builder_v1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    76213 2023-05-20 03:19:36.000000 quickstats-0.6.8.9/quickstats/components/workspaces/xml_ws_builder_v2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    45869 2023-07-07 21:58:59.000000 quickstats-0.6.8.9/quickstats/components/workspaces/xml_ws_combiner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    49268 2023-07-08 04:44:49.000000 quickstats-0.6.8.9/quickstats/components/workspaces/xml_ws_modifier.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:15.000000 quickstats-0.6.8.9/quickstats/concurrent/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      306 2023-05-31 15:27:50.000000 quickstats-0.6.8.9/quickstats/concurrent/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3379 2023-06-26 09:41:33.000000 quickstats-0.6.8.9/quickstats/concurrent/abstract_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.6.8.9/quickstats/concurrent/logging.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5239 2023-05-31 16:02:49.000000 quickstats-0.6.8.9/quickstats/concurrent/nuisance_parameter_ranking_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5891 2023-06-10 22:16:28.000000 quickstats-0.6.8.9/quickstats/concurrent/parameterised_asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10758 2023-06-28 16:38:35.000000 quickstats-0.6.8.9/quickstats/concurrent/parameterised_likelihood.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3963 2023-05-31 15:27:15.000000 quickstats-0.6.8.9/quickstats/concurrent/parameterised_runner.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:15.000000 quickstats-0.6.8.9/quickstats/core/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2023-01-04 09:02:55.000000 quickstats-0.6.8.9/quickstats/core/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      811 2023-01-04 09:02:55.000000 quickstats-0.6.8.9/quickstats/core/abstract_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20587 2023-05-20 03:28:17.000000 quickstats-0.6.8.9/quickstats/core/configs.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2198 2023-01-04 09:02:55.000000 quickstats-0.6.8.9/quickstats/core/configurable_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      541 2023-01-04 09:02:55.000000 quickstats-0.6.8.9/quickstats/core/dataclass_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      971 2023-05-20 03:27:42.000000 quickstats-0.6.8.9/quickstats/core/decorators.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2296 2023-05-23 21:10:32.000000 quickstats-0.6.8.9/quickstats/core/enums.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6651 2023-02-14 22:36:19.000000 quickstats-0.6.8.9/quickstats/core/methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9057 2023-02-08 05:24:13.000000 quickstats-0.6.8.9/quickstats/core/path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2952 2022-07-21 15:05:33.000000 quickstats-0.6.8.9/quickstats/core/virtual_trees.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:15.000000 quickstats-0.6.8.9/quickstats/interface/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       66 2023-05-31 15:27:05.000000 quickstats-0.6.8.9/quickstats/interface/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:15.000000 quickstats-0.6.8.9/quickstats/interface/cppyy/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2023-05-31 20:08:24.000000 quickstats-0.6.8.9/quickstats/interface/cppyy/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2022-01-31 03:37:54.000000 quickstats-0.6.8.9/quickstats/interface/cppyy/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12794 2023-07-12 23:07:57.000000 quickstats-0.6.8.9/quickstats/interface/cppyy/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4433 2023-01-04 09:02:55.000000 quickstats-0.6.8.9/quickstats/interface/cppyy/vectorize.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:15.000000 quickstats-0.6.8.9/quickstats/interface/root/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.6.8.9/quickstats/interface/root/RooAbsData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9855 2023-05-20 12:12:25.000000 quickstats-0.6.8.9/quickstats/interface/root/RooAbsPdf.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      420 2022-08-23 02:59:13.000000 quickstats-0.6.8.9/quickstats/interface/root/RooArgSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2023-03-12 16:17:52.000000 quickstats-0.6.8.9/quickstats/interface/root/RooCategory.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    44679 2023-05-20 12:08:58.000000 quickstats-0.6.8.9/quickstats/interface/root/RooDataSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.6.8.9/quickstats/interface/root/RooMsgService.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5451 2023-05-11 15:17:32.000000 quickstats-0.6.8.9/quickstats/interface/root/RooRealVar.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.6.8.9/quickstats/interface/root/TArrayData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2023-01-04 09:02:55.000000 quickstats-0.6.8.9/quickstats/interface/root/TF1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1995 2023-02-28 09:57:47.000000 quickstats-0.6.8.9/quickstats/interface/root/TFile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2023-05-20 12:06:46.000000 quickstats-0.6.8.9/quickstats/interface/root/TH1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5707 2023-05-03 13:36:36.000000 quickstats-0.6.8.9/quickstats/interface/root/TH2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      571 2022-08-23 03:14:20.000000 quickstats-0.6.8.9/quickstats/interface/root/TObject.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      856 2023-03-12 13:27:02.000000 quickstats-0.6.8.9/quickstats/interface/root/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.6.8.9/quickstats/interface/root/helper.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-03-24 19:40:20.000000 quickstats-0.6.8.9/quickstats/interface/root/inspection.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.6.8.9/quickstats/interface/root/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19576 2023-05-11 13:39:17.000000 quickstats-0.6.8.9/quickstats/interface/root/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5637 2023-05-27 06:13:47.000000 quickstats-0.6.8.9/quickstats/interface/root/roofit_extension.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:12.000000 quickstats-0.6.8.9/quickstats/macros/
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:15.000000 quickstats-0.6.8.9/quickstats/macros/AsymptoticCLsTool/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7083 2021-08-19 17:39:48.000000 quickstats-0.6.8.9/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1511 2021-06-11 19:36:10.000000 quickstats-0.6.8.9/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:16.000000 quickstats-0.6.8.9/quickstats/macros/FlexibleInterpVarMkII/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.6.8.9/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.6.8.9/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:16.000000 quickstats-0.6.8.9/quickstats/macros/QuickStatsCore/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1231 2022-05-07 02:55:05.000000 quickstats-0.6.8.9/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10322 2022-05-11 00:00:32.000000 quickstats-0.6.8.9/quickstats/macros/QuickStatsCore/RooFitExt.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3429 2022-05-10 23:59:25.000000 quickstats-0.6.8.9/quickstats/macros/QuickStatsCore/RooFitExt.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:16.000000 quickstats-0.6.8.9/quickstats/macros/ResponseFunction/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13755 2023-04-25 19:09:18.000000 quickstats-0.6.8.9/quickstats/macros/ResponseFunction/ResponseFunction.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.6.8.9/quickstats/macros/ResponseFunction/ResponseFunction.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:16.000000 quickstats-0.6.8.9/quickstats/macros/RooTwoSidedCBShape/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.6.8.9/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.6.8.9/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:16.000000 quickstats-0.6.8.9/quickstats/maths/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.6.8.9/quickstats/maths/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2093 2023-06-21 12:10:05.000000 quickstats-0.6.8.9/quickstats/maths/interpolation.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5548 2023-03-30 08:30:53.000000 quickstats-0.6.8.9/quickstats/maths/numerics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    28267 2023-07-08 04:40:34.000000 quickstats-0.6.8.9/quickstats/maths/statistics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2023-05-15 01:04:06.000000 quickstats-0.6.8.9/quickstats/maths/statistics_jitted.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.6.8.9/quickstats/maths/symbolics.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:16.000000 quickstats-0.6.8.9/quickstats/parsers/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      113 2022-04-20 10:58:59.000000 quickstats-0.6.8.9/quickstats/parsers/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.6.8.9/quickstats/parsers/config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15974 2023-07-13 23:36:20.000000 quickstats-0.6.8.9/quickstats/parsers/param_parser.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:17.000000 quickstats-0.6.8.9/quickstats/plots/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1441 2023-03-29 12:38:13.000000 quickstats-0.6.8.9/quickstats/plots/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14389 2023-06-21 01:49:40.000000 quickstats-0.6.8.9/quickstats/plots/abstract_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14145 2023-03-29 14:21:34.000000 quickstats-0.6.8.9/quickstats/plots/bidirectional_bar_chart.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.6.8.9/quickstats/plots/collective_data_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2750 2023-04-01 10:15:48.000000 quickstats-0.6.8.9/quickstats/plots/color_schemes.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5180 2023-05-17 15:59:58.000000 quickstats-0.6.8.9/quickstats/plots/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4007 2023-05-17 16:00:48.000000 quickstats-0.6.8.9/quickstats/plots/correlation_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6018 2023-07-03 18:31:57.000000 quickstats-0.6.8.9/quickstats/plots/general_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22775 2022-09-07 07:18:02.000000 quickstats-0.6.8.9/quickstats/plots/general_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3731 2022-09-09 08:30:51.000000 quickstats-0.6.8.9/quickstats/plots/histo_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6100 2023-03-21 16:34:42.000000 quickstats-0.6.8.9/quickstats/plots/hypotest_inverter_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8917 2023-07-04 13:41:54.000000 quickstats-0.6.8.9/quickstats/plots/likelihood_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15974 2023-07-10 11:46:54.000000 quickstats-0.6.8.9/quickstats/plots/likelihood_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      219 2021-04-19 13:56:55.000000 quickstats-0.6.8.9/quickstats/plots/likelihood_scan_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29141 2023-07-13 12:02:23.000000 quickstats-0.6.8.9/quickstats/plots/np_ranking_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    25696 2023-04-18 01:26:39.000000 quickstats-0.6.8.9/quickstats/plots/pdf_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5059 2023-02-06 09:15:46.000000 quickstats-0.6.8.9/quickstats/plots/sample_purity_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10293 2023-03-27 13:06:51.000000 quickstats-0.6.8.9/quickstats/plots/score_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4123 2023-01-04 09:02:56.000000 quickstats-0.6.8.9/quickstats/plots/stat_plot_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18642 2023-07-12 22:40:24.000000 quickstats-0.6.8.9/quickstats/plots/template.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13688 2022-07-29 18:50:11.000000 quickstats-0.6.8.9/quickstats/plots/test_statistic_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11061 2023-01-04 09:02:56.000000 quickstats-0.6.8.9/quickstats/plots/upper_limit_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18278 2023-07-12 22:35:07.000000 quickstats-0.6.8.9/quickstats/plots/upper_limit_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12201 2023-06-19 12:52:28.000000 quickstats-0.6.8.9/quickstats/plots/upper_limit_2D_plot_deprecated.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13186 2022-08-18 13:35:04.000000 quickstats-0.6.8.9/quickstats/plots/upper_limit_3D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17108 2023-07-10 22:33:48.000000 quickstats-0.6.8.9/quickstats/plots/upper_limit_benchmark_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29707 2023-06-27 09:55:20.000000 quickstats-0.6.8.9/quickstats/plots/variable_distribution_plot.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:17.000000 quickstats-0.6.8.9/quickstats/resources/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2023-03-20 15:25:27.000000 quickstats-0.6.8.9/quickstats/resources/default_workspace_extensions.json
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-04-08 03:20:04.000000 quickstats-0.6.8.9/quickstats/root_checker.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:17.000000 quickstats-0.6.8.9/quickstats/stylesheets/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2021-10-20 08:52:20.000000 quickstats-0.6.8.9/quickstats/stylesheets/quick_default.mplstyle
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:18.000000 quickstats-0.6.8.9/quickstats/utils/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.6.8.9/quickstats/utils/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11009 2023-07-07 22:00:44.000000 quickstats-0.6.8.9/quickstats/utils/common_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.6.8.9/quickstats/utils/condor_tasks.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17089 2023-06-04 03:39:00.000000 quickstats-0.6.8.9/quickstats/utils/data_conversion.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.6.8.9/quickstats/utils/hep_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6812 2023-05-31 13:27:25.000000 quickstats-0.6.8.9/quickstats/utils/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      335 2021-05-17 13:11:29.000000 quickstats-0.6.8.9/quickstats/utils/process_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    26262 2023-06-07 15:13:35.000000 quickstats-0.6.8.9/quickstats/utils/roofit_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9267 2021-11-23 21:10:48.000000 quickstats-0.6.8.9/quickstats/utils/roostats_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12379 2023-07-07 22:00:16.000000 quickstats-0.6.8.9/quickstats/utils/root_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1448 2023-07-08 03:51:23.000000 quickstats-0.6.8.9/quickstats/utils/string_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15023 2023-07-07 22:01:35.000000 quickstats-0.6.8.9/quickstats/utils/xml_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-07-14 09:26:12.000000 quickstats-0.6.8.9/quickstats.egg-info/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-07-14 09:26:08.000000 quickstats-0.6.8.9/quickstats.egg-info/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9130 2023-07-14 09:26:10.000000 quickstats-0.6.8.9/quickstats.egg-info/SOURCES.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2023-07-14 09:26:08.000000 quickstats-0.6.8.9/quickstats.egg-info/dependency_links.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2023-07-14 09:26:08.000000 quickstats-0.6.8.9/quickstats.egg-info/requires.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2023-07-14 09:26:08.000000 quickstats-0.6.8.9/quickstats.egg-info/top_level.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2023-07-14 09:26:18.000000 quickstats-0.6.8.9/setup.cfg
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1687 2023-01-04 09:02:56.000000 quickstats-0.6.8.9/setup.py
```

### Comparing `quickstats-0.6.8.8/PKG-INFO` & `quickstats-0.6.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.6.8.8
+Version: 0.6.8.9
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.6.8.8/README.md` & `quickstats-0.6.8.9/README.md`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/bin/quickstats` & `quickstats-0.6.8.9/bin/quickstats`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/__init__.py` & `quickstats-0.6.8.9/quickstats/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/analysis/analysis_base.py` & `quickstats-0.6.8.9/quickstats/analysis/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/analysis/analysis_path_manager.py` & `quickstats-0.6.8.9/quickstats/analysis/analysis_path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/analysis/config_format_templates.py` & `quickstats-0.6.8.9/quickstats/analysis/config_format_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/analysis/data_loading.py` & `quickstats-0.6.8.9/quickstats/analysis/data_loading.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/analysis/data_preprocessing.py` & `quickstats-0.6.8.9/quickstats/analysis/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/analysis/event_categorization.py` & `quickstats-0.6.8.9/quickstats/analysis/event_categorization.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/analysis/multi_class_boundary_tree.py` & `quickstats-0.6.8.9/quickstats/analysis/multi_class_boundary_tree.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/analysis/ntuple_conversion_tool.py` & `quickstats-0.6.8.9/quickstats/analysis/ntuple_conversion_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/analysis/ntuple_process_tool.py` & `quickstats-0.6.8.9/quickstats/analysis/ntuple_process_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/analysis/sample_poly_param_tool.py` & `quickstats-0.6.8.9/quickstats/analysis/sample_poly_param_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/analysis/systematics/base_systematics.py` & `quickstats-0.6.8.9/quickstats/analysis/systematics/base_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/analysis/systematics/gaussian_shape_systematics.py` & `quickstats-0.6.8.9/quickstats/analysis/systematics/gaussian_shape_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/analysis/systematics/normalization_systematics.py` & `quickstats-0.6.8.9/quickstats/analysis/systematics/normalization_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/analysis/systematics/systematics_evaluation_tool.py` & `quickstats-0.6.8.9/quickstats/analysis/systematics/systematics_evaluation_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/clis/core.py` & `quickstats-0.6.8.9/quickstats/clis/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,16 @@
               help='Pull range')
 @click.option('-y', '--padding', type=int, default=7, show_default=True,
               help='Padding below plot for texts and legends. NP column height is 1 unit.')
 @click.option('-h', '--height', type=float, default=1.0, show_default=True,
               help='NP column height')
 @click.option('-s', '--spacing', type=float, default=0., show_default=True,
               help='Spacing between impact box')
+@click.option('--label-fontsize', type=float, default=20., show_default=True,
+              help='Fontsize of analysis label text')
 @click.option('-d', '--display_poi', default=r"$\mu$", show_default=True,
               help='POI name to be shown in the plot')
 @click.option('-t', '--extra_text', default=None, help='Extra texts below the ATLAS label. '+\
                                                        'Use "//" as newline delimiter')
 @click.option('--elumi_label/--no_elumi_label', default=True, show_default=True,
               help='Show energy and luminosity labels')
 @click.option('--ranking_label/--no_ranking_label', default=True, show_default=True,
```

### Comparing `quickstats-0.6.8.8/quickstats/clis/inspect_rfile.py` & `quickstats-0.6.8.9/quickstats/clis/inspect_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/clis/inspect_ws.py` & `quickstats-0.6.8.9/quickstats/clis/inspect_ws.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/clis/likelihood_fit.py` & `quickstats-0.6.8.9/quickstats/clis/likelihood_fit.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/clis/likelihood_scan.py` & `quickstats-0.6.8.9/quickstats/clis/likelihood_scan.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/clis/limit_setting.py` & `quickstats-0.6.8.9/quickstats/clis/limit_setting.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/clis/processor_cli.py` & `quickstats-0.6.8.9/quickstats/clis/processor_cli.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/clis/workspace_tools.py` & `quickstats-0.6.8.9/quickstats/clis/workspace_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/__init__.py` & `quickstats-0.6.8.9/quickstats/components/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/analysis_base.py` & `quickstats-0.6.8.9/quickstats/components/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/analysis_object.py` & `quickstats-0.6.8.9/quickstats/components/analysis_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/asimov_generator.py` & `quickstats-0.6.8.9/quickstats/components/asimov_generator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/asymptotic_cls.py` & `quickstats-0.6.8.9/quickstats/components/asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/basics.py` & `quickstats-0.6.8.9/quickstats/components/basics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/extended_minimizer.py` & `quickstats-0.6.8.9/quickstats/components/extended_minimizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/extended_model.py` & `quickstats-0.6.8.9/quickstats/components/extended_model.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/extended_rfile.py` & `quickstats-0.6.8.9/quickstats/components/extended_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/likelihood.py` & `quickstats-0.6.8.9/quickstats/components/likelihood.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,21 +49,25 @@
         poi_val = cond_fit_result['mu']
         if (qmu >= 0):
             ndof = len(poi_val)
             if ndof == 1:
                 # ndof = 1 case
                 poi_name = list(poi_val)[0]
                 x0 = poi_val[poi_name]
-                significance = math.sqrt(qmu)
+                if x0 == 0:
+                    sign = np.sign(uncond_fit_result['muhat'][poi_name])
+                    significance = sign * math.sqrt(qmu)
+                else:
+                    significance = math.sqrt(qmu)
                 pvalue = 1 - ROOT.Math.normal_cdf(significance, 1, x0)
             else:
                 x0 = list(set(poi_val.values()))
                 if len(x0) > 1:
-                    combined_fit_result['significance'] = None
-                    combined_fit_result['pvalue'] = None
+                    pvalue = None
+                    significance = None
                 else:
                     pvalue = ROOT.Math.chisquared_cdf_c(qmu, ndof, x0[0])
                     significance = ROOT.RooStats.PValueToSignificance(pvalue)
             combined_fit_result['significance'] = significance
             combined_fit_result['pvalue'] = pvalue
         else:
             combined_fit_result['significance'] = None
@@ -229,41 +233,16 @@
                 'muhat': muhat,
                 'nll': nll_cond,
                 'status': fit_status_cond,
                 'time': fit_time_cond
             }
             
         if mode == FitMode.HYBRID:
-            pnll = nll_cond - nll_uncond
-            qmu  = 2*pnll
-            self.stdout.info("PNLL = ".rjust(15) + "{:.5f}".format(nll_cond - nll_uncond), bare=True)
-            fit_result['pnll'] = pnll
-            fit_result['qmu']  = qmu
-            
-            if (qmu >= 0):
-                ndof = len(pois)
-                if ndof == 1:
-                    # ndof = 1 case
-                    poi_name = pois.first().GetName()
-                    x0 = poi_val[poi_name]
-                    significance = math.sqrt(qmu)
-                    pvalue = 1 - ROOT.Math.normal_cdf(significance, 1, x0)
-                else:
-                    x0 = list(set(poi_val.values()))
-                    if len(x0) > 1:
-                        fit_result['significance'] = None
-                        fit_result['pvalue'] = None
-                    else:
-                        pvalue = ROOT.Math.chisquared_cdf_c(qmu, ndof, x0[0])
-                        significance = ROOT.RooStats.PValueToSignificance(pvalue)
-                fit_result['significance'] = significance
-                fit_result['pvalue'] = pvalue
-            else:
-                fit_result['significance'] = None
-                fit_result['pvalue'] = None
+            hybrid_result = self.get_combined_fit_result(fit_result['uncond_fit'], fit_result['cond_fit'])
+            fit_result.update(hybrid_result)
                 
         if mode != FitMode.NOMINAL:
             self.stdout.info("time = ".rjust(15) + \
                              "(uncond_fit) {:.3f}, (cond_fit) {:.3f}".format(fit_time_uncond, fit_time_cond), bare=True)
             fit_result['total_time'] = fit_time_uncond + fit_time_cond
         else:
             self.stdout.info("prefit NLL = ".rjust(18) + f"{prefit_nll:.5f}", bare=True)
```

### Comparing `quickstats-0.6.8.8/quickstats/components/modelling/component_source.py` & `quickstats-0.6.8.9/quickstats/components/modelling/component_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/modelling/data_modelling.py` & `quickstats-0.6.8.9/quickstats/components/modelling/data_modelling.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/modelling/model_source.py` & `quickstats-0.6.8.9/quickstats/components/modelling/model_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/modelling/parameter_templates.py` & `quickstats-0.6.8.9/quickstats/components/modelling/parameter_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/modelling/pdf_fit_tool.py` & `quickstats-0.6.8.9/quickstats/components/modelling/pdf_fit_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/modelling/tree_data_source.py` & `quickstats-0.6.8.9/quickstats/components/modelling/tree_data_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/nuisance_parameter_harmonizer.py` & `quickstats-0.6.8.9/quickstats/components/nuisance_parameter_harmonizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/nuisance_parameter_pull.py` & `quickstats-0.6.8.9/quickstats/components/nuisance_parameter_pull.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/nuisance_parameter_ranking.py` & `quickstats-0.6.8.9/quickstats/components/nuisance_parameter_ranking.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/__init__.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_alias.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_as_numpy.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_as_numpy.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_base_action.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_base_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_declare.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_declare.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_define.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_define.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_export.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_export.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_filter.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_filter.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_global_variables.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_global_variables.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_hybrid_action.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_hybrid_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_if_defined.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_if_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_if_not_defined.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_if_not_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_load_frame.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_load_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_load_macro.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_load_macro.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_nested_action.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_nested_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_report.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_report.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_safe_alias.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_safe_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_save.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_save.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_save_frame.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_save_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_stat.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_stat.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/actions/rooproc_treename.py` & `quickstats-0.6.8.9/quickstats/components/processors/actions/rooproc_treename.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/builtin_methods.py` & `quickstats-0.6.8.9/quickstats/components/processors/builtin_methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/roo_config_parser.py` & `quickstats-0.6.8.9/quickstats/components/processors/roo_config_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/processors/roo_processor.py` & `quickstats-0.6.8.9/quickstats/components/processors/roo_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,17 +84,17 @@
     def cleanup(self):
         close_all_root_files()
         self.rdf_frames = {}
         self.rdf = None
         
     def _get_all_files(self, filenames:Union[List[str], str]):
         all_files = []
-        if isinstance(filename, str):
-            filename = [filename]
-        if not isinstance(filename, list):
+        if isinstance(filenames, str):
+            filenames = [filenames]
+        if not isinstance(filenames, list):
             raise ValueError("filename must be either string or list of strings")
         for filename in filenames:
             if os.path.isdir(filename):
                 all_files += glob.glob(os.path.join(filename, "*.root"))
             else:
                 all_files += glob.glob(filename)
         if not all_files:
```

### Comparing `quickstats-0.6.8.8/quickstats/components/pvalue_toys.py` & `quickstats-0.6.8.9/quickstats/components/pvalue_toys.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/roo_inspector.py` & `quickstats-0.6.8.9/quickstats/components/roo_inspector.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/root_object.py` & `quickstats-0.6.8.9/quickstats/components/root_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/toy_limit_calculator.py` & `quickstats-0.6.8.9/quickstats/components/toy_limit_calculator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/workspaces/__init__.py` & `quickstats-0.6.8.9/quickstats/components/workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/workspaces/asimov_handler.py` & `quickstats-0.6.8.9/quickstats/components/workspaces/asimov_handler.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/workspaces/core_argument_sets.py` & `quickstats-0.6.8.9/quickstats/components/workspaces/core_argument_sets.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/workspaces/sample.py` & `quickstats-0.6.8.9/quickstats/components/workspaces/sample.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/workspaces/settings.py` & `quickstats-0.6.8.9/quickstats/components/workspaces/settings.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/workspaces/systematic.py` & `quickstats-0.6.8.9/quickstats/components/workspaces/systematic.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/workspaces/systematics_domain.py` & `quickstats-0.6.8.9/quickstats/components/workspaces/systematics_domain.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/workspaces/ws_comparer.py` & `quickstats-0.6.8.9/quickstats/components/workspaces/ws_comparer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/workspaces/ws_decomposer.py` & `quickstats-0.6.8.9/quickstats/components/workspaces/ws_decomposer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/workspaces/ws_modifier_config.py` & `quickstats-0.6.8.9/quickstats/components/workspaces/ws_modifier_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/workspaces/xml_ws_base.py` & `quickstats-0.6.8.9/quickstats/components/workspaces/xml_ws_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/workspaces/xml_ws_builder_v1.py` & `quickstats-0.6.8.9/quickstats/components/workspaces/xml_ws_builder_v1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/workspaces/xml_ws_builder_v2.py` & `quickstats-0.6.8.9/quickstats/components/workspaces/xml_ws_builder_v2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/workspaces/xml_ws_combiner.py` & `quickstats-0.6.8.9/quickstats/components/workspaces/xml_ws_combiner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/components/workspaces/xml_ws_modifier.py` & `quickstats-0.6.8.9/quickstats/components/workspaces/xml_ws_modifier.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/concurrent/abstract_runner.py` & `quickstats-0.6.8.9/quickstats/concurrent/abstract_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/concurrent/logging.py` & `quickstats-0.6.8.9/quickstats/concurrent/logging.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/concurrent/nuisance_parameter_ranking_runner.py` & `quickstats-0.6.8.9/quickstats/concurrent/nuisance_parameter_ranking_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/concurrent/parameterised_asymptotic_cls.py` & `quickstats-0.6.8.9/quickstats/concurrent/parameterised_asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/concurrent/parameterised_likelihood.py` & `quickstats-0.6.8.9/quickstats/concurrent/parameterised_likelihood.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/concurrent/parameterised_runner.py` & `quickstats-0.6.8.9/quickstats/concurrent/parameterised_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/core/abstract_object.py` & `quickstats-0.6.8.9/quickstats/core/abstract_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/core/configs.py` & `quickstats-0.6.8.9/quickstats/core/configs.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/core/configurable_object.py` & `quickstats-0.6.8.9/quickstats/core/configurable_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/core/dataclass_object.py` & `quickstats-0.6.8.9/quickstats/core/dataclass_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/core/decorators.py` & `quickstats-0.6.8.9/quickstats/core/decorators.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/core/enums.py` & `quickstats-0.6.8.9/quickstats/core/enums.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/core/methods.py` & `quickstats-0.6.8.9/quickstats/core/methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/core/path_manager.py` & `quickstats-0.6.8.9/quickstats/core/path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/core/virtual_trees.py` & `quickstats-0.6.8.9/quickstats/core/virtual_trees.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/interface/cppyy/core.py` & `quickstats-0.6.8.9/quickstats/interface/cppyy/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/interface/cppyy/macros.py` & `quickstats-0.6.8.9/quickstats/interface/cppyy/macros.py`

 * *Files 3% similar despite different names*

```diff
@@ -180,51 +180,52 @@
                         XGBoosterGetAttr(*m_booster.get(), "best_iteration", &out, &success);
                         m_bst_ntree_limit = atoi(out);
                     }
                     else
                         m_bst_ntree_limit = 0;
                 }
                 
-                std::vector<float> getWeightsFromDMatrix(std::vector<float> &vars, const int &size=1){
+                std::vector<float> getWeightsFromDMatrix(std::vector<float> &vars, const int &size=1, int option_mask=0){
                     const int nvars = vars.size();
-                    std::vector<float> weights = getWeightsFromDMatrix(vars.data(), nvars, size);
+                    std::vector<float> weights = getWeightsFromDMatrix(vars.data(), nvars, size, option_mask);
                     return weights;
                 }
                 
-                std::vector<float> getWeightsFromDMatrix(float* vars, const int nvars, const int &size=1){
+                std::vector<float> getWeightsFromDMatrix(float* vars, const int nvars, const int &size=1, int option_mask=0){
                     DMatrixHandle dmat;
                     XGDMatrixCreateFromMat(vars, size, nvars, -1, &dmat);
                     bst_ulong out_len;
                     const float *f;
-                    XGBoosterPredict(*m_booster.get(), dmat, 0, m_bst_ntree_limit, 0, &out_len, &f);
+                    XGBoosterPredict(*m_booster.get(), dmat, option_mask, m_bst_ntree_limit, 0, &out_len, &f);
                     XGDMatrixFree(dmat);
                     std::vector<float> weights(size);
                     weights.assign(f, f + size);
                     return weights;
                 }
                 
-                std::vector<float> getWeightsFromDense(std::vector<float> &vars, const int &size=1){
+                std::vector<float> getWeightsFromDense(std::vector<float> &vars, const int &size=1, int option_mask=0){
                     const int nvars = vars.size();
-                    std::vector<float> weights = getWeightsFromDense(vars.data(), nvars, size);
+                    std::vector<float> weights = getWeightsFromDense(vars.data(), nvars, size, option_mask);
                     return weights;
                 }
 
-                std::vector<float> getWeightsFromDense(float* vars, const int nvars, const int &size=1){
+                std::vector<float> getWeightsFromDense(float* vars, const int nvars, const int &size=1, int option_mask=0){
                     const char str_format[] = "{\\"data\\": [%lu, true], \\"shape\\": [%lu, %lu], "
                                               "\\"typestr\\": \\"<f4\\", \\"version\\": 3}";
-                    const char config[] = "{\\"type\\": 0, \\"training\\": false, \\"iteration_begin\\": 0, "
-                                          "\\"iteration_end\\": 0, \\"strict_shape\\": true, \\"cache_id\\": 0"
-                                          ", \\"missing\\": NaN}";
+                    std::string config = (std::string)("{\\"type\\": " + std::to_string(option_mask) + 
+                                                       ", \\"training\\": false, \\"iteration_begin\\": 0,"
+                                                       "\\"iteration_end\\": 0, \\"strict_shape\\": true,"
+                                                       "\\"cache_id\\": 0, \\"missing\\": NaN}");
                     char array_interface[256];
                     memset(array_interface, '\\0', sizeof(array_interface));
                     sprintf(array_interface, str_format, (size_t) vars, (size_t)size, (size_t)nvars);
                     const float *f;
                     bst_ulong out_len;
                     uint64_t const *out_shape;
-                    XGBoosterPredictFromDense(*m_booster.get(), array_interface, config, NULL,
+                    XGBoosterPredictFromDense(*m_booster.get(), array_interface, config.c_str(), NULL,
                                               &out_shape, &out_len, &f);
                     std::vector<float> weights(size);
                     weights.assign(f, f + size);
                     return weights;
                 }
             private:
                 std::unique_ptr<BoosterHandle> m_booster;
```

### Comparing `quickstats-0.6.8.8/quickstats/interface/cppyy/vectorize.py` & `quickstats-0.6.8.9/quickstats/interface/cppyy/vectorize.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/interface/root/RooAbsData.py` & `quickstats-0.6.8.9/quickstats/interface/root/RooAbsData.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/interface/root/RooAbsPdf.py` & `quickstats-0.6.8.9/quickstats/interface/root/RooAbsPdf.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/interface/root/RooCategory.py` & `quickstats-0.6.8.9/quickstats/interface/root/RooCategory.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/interface/root/RooDataSet.py` & `quickstats-0.6.8.9/quickstats/interface/root/RooDataSet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/interface/root/RooMsgService.py` & `quickstats-0.6.8.9/quickstats/interface/root/RooMsgService.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/interface/root/RooRealVar.py` & `quickstats-0.6.8.9/quickstats/interface/root/RooRealVar.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/interface/root/TF1.py` & `quickstats-0.6.8.9/quickstats/interface/root/TF1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/interface/root/TFile.py` & `quickstats-0.6.8.9/quickstats/interface/root/TFile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/interface/root/TH1.py` & `quickstats-0.6.8.9/quickstats/interface/root/TH1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/interface/root/TH2.py` & `quickstats-0.6.8.9/quickstats/interface/root/TH2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/interface/root/TObject.py` & `quickstats-0.6.8.9/quickstats/interface/root/TObject.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/interface/root/__init__.py` & `quickstats-0.6.8.9/quickstats/interface/root/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/interface/root/helper.py` & `quickstats-0.6.8.9/quickstats/interface/root/helper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/interface/root/inspection.py` & `quickstats-0.6.8.9/quickstats/interface/root/inspection.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/interface/root/macros.py` & `quickstats-0.6.8.9/quickstats/interface/root/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/interface/root/roofit_extension.py` & `quickstats-0.6.8.9/quickstats/interface/root/roofit_extension.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx` & `quickstats-0.6.8.9/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h` & `quickstats-0.6.8.9/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx` & `quickstats-0.6.8.9/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h` & `quickstats-0.6.8.9/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx` & `quickstats-0.6.8.9/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/macros/QuickStatsCore/RooFitExt.cxx` & `quickstats-0.6.8.9/quickstats/macros/QuickStatsCore/RooFitExt.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/macros/QuickStatsCore/RooFitExt.h` & `quickstats-0.6.8.9/quickstats/macros/QuickStatsCore/RooFitExt.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/macros/ResponseFunction/ResponseFunction.cxx` & `quickstats-0.6.8.9/quickstats/macros/ResponseFunction/ResponseFunction.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/macros/ResponseFunction/ResponseFunction.h` & `quickstats-0.6.8.9/quickstats/macros/ResponseFunction/ResponseFunction.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx` & `quickstats-0.6.8.9/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h` & `quickstats-0.6.8.9/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/maths/interpolation.py` & `quickstats-0.6.8.9/quickstats/maths/interpolation.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/maths/numerics.py` & `quickstats-0.6.8.9/quickstats/maths/numerics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/maths/statistics.py` & `quickstats-0.6.8.9/quickstats/maths/statistics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/maths/statistics_jitted.py` & `quickstats-0.6.8.9/quickstats/maths/statistics_jitted.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/maths/symbolics.py` & `quickstats-0.6.8.9/quickstats/maths/symbolics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/parsers/param_parser.py` & `quickstats-0.6.8.9/quickstats/parsers/param_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,16 +259,19 @@
             filenames = glob.glob(dirname)
         param_points = []
         for filename in filenames:
             basename = os.path.basename(filename)
             match = self.filename_regex.match(basename)
             if not match:
                 continue
-            point = {'filename': filename, 'parameters':{}}
-            point['basename'] = basename.split('.')[0]
+            point = {
+                'filename'   : filename,
+                'basename'   : os.path.splitext(basename)[0],
+                'parameters' : {}
+            }
             for key, value in match.groupdict().items():
                 parser = self.attribute_parser[key]
                 point['parameters'][key] = parser(value)
             param_points.append(point)
         attributes = list(self.attribute_parser)
         param_points = self.sort_param_points(param_points, attributes)
         selected_param_points = self.select_param_points(param_points, filter_expr,
```

### Comparing `quickstats-0.6.8.8/quickstats/plots/__init__.py` & `quickstats-0.6.8.9/quickstats/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/abstract_plot.py` & `quickstats-0.6.8.9/quickstats/plots/abstract_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/bidirectional_bar_chart.py` & `quickstats-0.6.8.9/quickstats/plots/bidirectional_bar_chart.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/collective_data_plot.py` & `quickstats-0.6.8.9/quickstats/plots/collective_data_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/color_schemes.py` & `quickstats-0.6.8.9/quickstats/plots/color_schemes.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/core.py` & `quickstats-0.6.8.9/quickstats/plots/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/correlation_plot.py` & `quickstats-0.6.8.9/quickstats/plots/correlation_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/general_1D_plot.py` & `quickstats-0.6.8.9/quickstats/plots/general_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/general_distribution_plot.py` & `quickstats-0.6.8.9/quickstats/plots/general_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/histo_1D_plot.py` & `quickstats-0.6.8.9/quickstats/plots/histo_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/hypotest_inverter_plot.py` & `quickstats-0.6.8.9/quickstats/plots/hypotest_inverter_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/likelihood_1D_plot.py` & `quickstats-0.6.8.9/quickstats/plots/likelihood_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/likelihood_2D_plot.py` & `quickstats-0.6.8.9/quickstats/plots/likelihood_2D_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,20 +177,34 @@
             nan_shapes = self.get_nan_shapes(data, xattrib, yattrib, zattrib)
         else:
             nan_shapes = None
         if (remove_nan_points_within_distance is not None) and (len(nan_shapes) > 0):
             if len(nan_shapes) > 0:
                 from shapely import Point
                 XY = np.column_stack((X.ravel(), Y.ravel()))
-                mask = np.ones(Z.shape)
                 d = remove_nan_points_within_distance
                 for shape in nan_shapes:
-                    new_mask = np.array([shape.exterior.distance(Point(xy)) > d for xy in XY])
-                    mask = np.logical_and(mask, new_mask.reshape(mask.shape))
-                Z[~mask] = np.nan
+                    x_ext, y_ext = shape.exterior.coords.xy
+                    min_x_cutoff, max_x_cutoff = np.min(x_ext) - d, np.max(x_ext) + d
+                    min_y_cutoff, max_y_cutoff = np.min(y_ext) - d, np.max(y_ext) + d
+                    # only focus on points within the largest box formed by the convex hull + distance
+                    box_mask = (((XY[:, 0] > min_x_cutoff) & (XY[:, 0] < max_x_cutoff)) & 
+                                ((XY[:, 1] > min_y_cutoff) & (XY[:, 1] < max_y_cutoff)))
+                    mask = np.full(box_mask.shape, False)
+                    XY_box = XY[box_mask]
+                    # remove points inside the polygon
+                    mask_int = np.array([shape.contains(Point(xy)) for xy in XY_box])
+                    XY_box_ext = XY_box[~mask_int]
+                    # remove points within distance d of the polygon
+                    mask_int_d = np.array([shape.exterior.distance(Point(xy)) < d for xy in XY_box_ext])
+                    slice_int = np.arange(mask.shape[0])[box_mask][mask_int]
+                    slice_int_d = np.arange(mask.shape[0])[box_mask][~mask_int][mask_int_d]
+                    mask[slice_int] = True
+                    mask[slice_int_d] = True
+                    Z[mask.reshape(Z.shape)] = np.nan
         if draw_colormesh:
             cmap = config['cmap']
             im = ax.pcolormesh(X, Y, Z, cmap=cmap, shading='auto')
             import matplotlib.pyplot as plt
             self.cbar = plt.colorbar(im, ax=ax, **config['colorbar'])
             self.cbar.set_label(**config['colorbar_label'])
```

### Comparing `quickstats-0.6.8.8/quickstats/plots/np_ranking_plot.py` & `quickstats-0.6.8.9/quickstats/plots/np_ranking_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -582,19 +582,21 @@
             ax2.get_xaxis().set_visible(False)
         return fig
     
     def plot(self, show_sigma:bool=True, show_prefit:bool=True, show_postfit:bool=True, sigma_bands:bool=False,
              sigma_lines:bool=True, shade:bool=True, correlation:bool=True, onesided:bool=True, relative:bool=False,
              theta_max:float=2, padding:int=7, height:float=1, spacing:float=0, display_poi:str=r"$\mu$", 
              extra_text:str=None, elumi_label:bool=True, ranking_label:bool=True, energy:str=r"13 TeV", 
-             lumi:str=r"139 fb$^{-1}$",
+             lumi:str=r"139 fb$^{-1}$", label_fontsize:Optional[float]=None,
              status:str='int', n_rank=None, rank_per_plot=20, combine_pdf=True, threshold=0, ranking=True, 
              fix_axis_scale=True, outdir="ranking_plots", outname:str='ranking', style:Union[str, Dict]=DEFAULT_STYLE):
         if isinstance(style, str):
             style = self.parse_style(style)
+        if label_fontsize is not None:
+            style['label']['fontsize'] = label_fontsize
         if self.data is None:
             raise ValueError("no data to process")
         has_impact = any('impact' in i for i in self.data)
         if not has_impact:
             ranking, threshold, show_prefit, show_postfit = False, False, False, False           
         processed_data = self.get_processed_data(self.data, num=n_rank, threshold=threshold, ranking=ranking)
         num_data = len(processed_data)
```

### Comparing `quickstats-0.6.8.8/quickstats/plots/pdf_distribution_plot.py` & `quickstats-0.6.8.9/quickstats/plots/pdf_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/sample_purity_plot.py` & `quickstats-0.6.8.9/quickstats/plots/sample_purity_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/score_distribution_plot.py` & `quickstats-0.6.8.9/quickstats/plots/score_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/stat_plot_config.py` & `quickstats-0.6.8.9/quickstats/plots/stat_plot_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/template.py` & `quickstats-0.6.8.9/quickstats/plots/template.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/test_statistic_distribution_plot.py` & `quickstats-0.6.8.9/quickstats/plots/test_statistic_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/upper_limit_1D_plot.py` & `quickstats-0.6.8.9/quickstats/plots/upper_limit_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/upper_limit_2D_plot.py` & `quickstats-0.6.8.9/quickstats/plots/upper_limit_2D_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,31 +207,37 @@
         if styles is None:
             styles = self.config['highlight_styles']
         x, y, label = option['x'], option['y'], option['label']
         handle = ax.plot(x, y, label=label, **styles)
         self.update_legend_handles({'highlight': handle[0]}, idx=0)
         
     def draw_single_data(self, ax, data:pd.DataFrame,
+                         column:Optional[str]=None,
                          scale_theory:bool=False,
-                         log:bool=False,
+                         logx:bool=False,
+                         logy:bool=False,
                          draw_expected:bool=True,
                          draw_observed:bool=True,
                          color_pallete:Optional[Dict]=None,
                          labels:Optional[Dict]=None,
                          sigma_band_hatch:Optional[str]=None,
                          draw_errorband:bool=True,
                          idx:int=0):
         
         if color_pallete is None:
             color_pallete = self.color_pallete
             
         if labels is None:
             labels = self.labels
-   
-        x = data.index.astype(float).values
+       
+        if column is None:
+            x = data.index.astype(float).values
+        else:
+            x = data[column].values
+            
         if (not scale_theory) or (self.theory_func is None):
             scale_factor = 1.0
         else:
             _, scale_factor, _, _ = self.get_theory_prediction(x)
 
         handles_map = {}
         
@@ -250,18 +256,22 @@
                                             facecolor=color_pallete['1sigma'],
                                             label=labels['1sigma'],
                                             hatch=sigma_band_hatch,
                                             **self.config["errorband_plot_styles"])
             handles_map['1sigma'] = handle_1sigma
             handles_map['2sigma'] = handle_2sigma
         
-        if log:
+        if (not logx) and (not logy):
+            draw_fn = ax.plot
+        elif logy and (not logx):
             draw_fn = ax.semilogy
+        elif logx and (not logy):
+            draw_fn = ax.semilogx
         else:
-            draw_fn = ax.plot
+            draw_fn = ax.loglog
  
         if draw_observed:
             y_obs = data['obs'].values * scale_factor
             handle_observed = draw_fn(x, y_obs, color=color_pallete['observed'], 
                                       label=labels['observed'], 
                                       **self.config["observed_plot_styles"])
             handles_map['observed'] = handle_observed[0]
@@ -336,16 +346,16 @@
                         **self.styles['annotation'])
     
     def _get_candidate_columns(self, data:pd.DataFrame):
         cols = [col for col in data.columns if col not in ['-2', '-1', '0', '1', '2', 'obs', 'inj']]
         return cols
     
     def draw(self, column:Optional[str]=None, xlabel:str="", ylabel:str="",
-             ylim=None, xlim=None, scale_theory:bool=False, log:bool=False,
-             draw_expected:bool=True, draw_observed:bool=True,
+             ylim=None, xlim=None, scale_theory:bool=False, logx:bool=False,
+             logy:bool=False, draw_expected:bool=True, draw_observed:bool=True,
              draw_errorband:bool=True, draw_hatch:bool=True,
              draw_theory_curve:bool=False, draw_interval:bool=False,
              draw_length:bool=False):
         
         ax = self.draw_frame()
         
         if len(self.additional_data) > 0:
@@ -353,16 +363,17 @@
                 sigma_band_hatch = self.config['secondary_hatch']
                 alpha = self.config['secondary_alpha']
             else:
                 sigma_band_hatch = None
                 alpha = 1.
             for idx, config in enumerate(self.additional_data):
                 data_i = config["data"].copy().sort_index()
-                self.draw_single_data(ax, data_i,
-                                      log=log, scale_theory=scale_theory,
+                self.draw_single_data(ax, data_i, column=column,
+                                      logx=logx, logy=logy,
+                                      scale_theory=scale_theory,
                                       draw_expected=config["draw_expected"],
                                       draw_observed=config["draw_observed"],
                                       color_pallete=config["color_pallete"],
                                       labels=config["labels"],
                                       sigma_band_hatch=sigma_band_hatch,
                                       draw_errorband=config["draw_errorband"],
                                       idx=idx + 1)
@@ -372,16 +383,17 @@
             else:
                 sigma_band_hatch = None
                 alpha = 1.
         else:
             sigma_band_hatch = None
             alpha = 1.
             
-        self.draw_single_data(ax, self.data,
-                              log=log, scale_theory=scale_theory,
+        self.draw_single_data(ax, self.data, column=column,
+                              logx=logx, logy=logy,
+                              scale_theory=scale_theory,
                               draw_expected=draw_expected,
                               draw_observed=draw_observed,
                               color_pallete=self.color_pallete,
                               labels=self.labels,
                               sigma_band_hatch=sigma_band_hatch,
                               draw_errorband=draw_errorband,
                               idx=0)
```

### Comparing `quickstats-0.6.8.8/quickstats/plots/upper_limit_2D_plot_deprecated.py` & `quickstats-0.6.8.9/quickstats/plots/upper_limit_2D_plot_deprecated.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/upper_limit_3D_plot.py` & `quickstats-0.6.8.9/quickstats/plots/upper_limit_3D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/plots/upper_limit_benchmark_plot.py` & `quickstats-0.6.8.9/quickstats/plots/upper_limit_benchmark_plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -277,15 +277,36 @@
             target_cols.extend(['-2', '-1', '1', '2'])
         y = comparison_data[target_cols].values
         ylim = list(ax.get_ylim())
         if ylim[0] > np.min(y):
             ylim[0] = np.min(y)
         if ylim[1] < np.max(y):
             ylim[1] = np.max(y)
-        ax.set_ylim(ylim)      
+        ax.set_ylim(ylim)
+        
+    def get_theory_scale(self, df:Optional[pd.DataFrame]=None,
+                         iloc:Optional[List[int]]=None, target:Optional[str]=None):
+        if df is None:
+            df = self.get_target_df(iloc=iloc, target=target)
+        nbenchmark = len(df.index)
+        nlevel = df.index.nlevels 
+        values = np.array(sum(df.index.values, ())).reshape(nbenchmark, nlevel).T
+        theory_scale = self.get_theory_prediction(*values)[-3]
+        df_theory = df.drop(columns=df.columns)
+        df_theory['theory_scale'] = theory_scale
+        return df_theory
+    
+    def get_target_df(self, iloc:Optional[List[int]]=None, target:Optional[str]=None):
+        if target is None:
+            df = self.data.copy()
+        else:
+            df = self.alt_data[target].copy()
+        if iloc is not None:
+            df = df[iloc]
+        return df
     
     def draw(self, iloc:Optional[List[int]]=None, xticklabels:Optional[List[str]]=None,
              logy:bool=False, xlabel:str="", ylabel:str="", ylim=None,
              scale_theory:bool=False, draw_expected:bool=True,
              draw_observed:bool=True, draw_errorband:bool=True,
              alt_draw_options:Optional[Dict]=None,
              comparison_options:Optional[Dict]=None):
@@ -293,44 +314,39 @@
         targets = [None]
         if alt_draw_options is not None:
             targets.extend(list(alt_draw_options.keys()))
         target_kwargs = {}
         nbenchmark = None
         for target in targets:
             target_kwargs[target] = {}
+            df = self.get_target_df(iloc=iloc, target=target)
             if target is None:
-                df = self.data.copy()
                 target_kwargs[target]['color_pallete'] = self.color_pallete
                 target_kwargs[target]['labels'] = self.labels
                 target_kwargs[target]['custom_styles'] = self.custom_styles
                 target_kwargs[target]['draw_expected'] = draw_expected
                 target_kwargs[target]['draw_observed'] = draw_observed
                 target_kwargs[target]['draw_errorband'] = draw_errorband
                 target_scale_theory = scale_theory
             else:
-                df = self.alt_data[target].copy()
                 draw_options = alt_draw_options[target]
                 target_kwargs[target]['color_pallete'] = self.alt_color_pallete[target]
                 target_kwargs[target]['labels'] = self.alt_labels[target]
                 target_kwargs[target]['custom_styles'] = self.alt_custom_styles[target] 
                 target_kwargs[target]['draw_expected'] = draw_options.get('draw_expected', draw_expected)
                 target_kwargs[target]['draw_observed'] = draw_options.get('draw_observed', draw_observed)
                 target_kwargs[target]['draw_errorband'] = draw_options.get('draw_errorband', draw_errorband)
                 target_scale_theory = draw_options.get('scale_theory', scale_theory)
-            if iloc is not None:
-                df = df[iloc]
             if nbenchmark is None:
                 nbenchmark = len(df.index)
             elif len(df.index) != nbenchmark:
                 RuntimeError(f'main and alternative data ("{target}") have different number of benchmark points')
             if target_scale_theory:
-                nlevel = df.index.nlevels 
-                values = np.array(sum(df.index.values, ())).reshape(nbenchmark, nlevel).T
-                scale_factor = self.get_theory_prediction(*values)[-3]
-                df['scale'] = scale_factor
+                df_theory = self.get_theory_scale(df=df)
+                df.loc[df_theory.index, ['scale']] = df_theory['theory_scale']
                 cols = ['-2', '-1', '0', '1', '2', 'obs']
                 df.loc[:, cols] = df.loc[:, cols].multiply(df.loc[:, 'scale'], axis="index")
             target_kwargs[target]['data'] = df
             
         if xticklabels is None:
             xticklabels = [str(i) for i in range(nbenchmark)]
         elif len(xticklabels) != nbenchmark:
```

### Comparing `quickstats-0.6.8.8/quickstats/plots/variable_distribution_plot.py` & `quickstats-0.6.8.9/quickstats/plots/variable_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/root_checker.py` & `quickstats-0.6.8.9/quickstats/root_checker.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/utils/common_utils.py` & `quickstats-0.6.8.9/quickstats/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/utils/data_conversion.py` & `quickstats-0.6.8.9/quickstats/utils/data_conversion.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/utils/hep_utils.py` & `quickstats-0.6.8.9/quickstats/utils/hep_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/utils/io.py` & `quickstats-0.6.8.9/quickstats/utils/io.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/utils/roofit_utils.py` & `quickstats-0.6.8.9/quickstats/utils/roofit_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/utils/roostats_utils.py` & `quickstats-0.6.8.9/quickstats/utils/roostats_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/utils/root_utils.py` & `quickstats-0.6.8.9/quickstats/utils/root_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/utils/string_utils.py` & `quickstats-0.6.8.9/quickstats/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats/utils/xml_tools.py` & `quickstats-0.6.8.9/quickstats/utils/xml_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/quickstats.egg-info/PKG-INFO` & `quickstats-0.6.8.9/quickstats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.6.8.8
+Version: 0.6.8.9
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.6.8.8/quickstats.egg-info/SOURCES.txt` & `quickstats-0.6.8.9/quickstats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.8/setup.py` & `quickstats-0.6.8.9/setup.py`

 * *Files identical despite different names*

