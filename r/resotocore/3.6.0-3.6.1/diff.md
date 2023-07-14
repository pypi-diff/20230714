# Comparing `tmp/resotocore-3.6.0.tar.gz` & `tmp/resotocore-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotocore-3.6.0.tar", last modified: Fri Jun 30 19:29:18 2023, max compression
+gzip compressed data, was "resotocore-3.6.1.tar", last modified: Fri Jul 14 17:01:36 2023, max compression
```

## Comparing `resotocore-3.6.0.tar` & `resotocore-3.6.1.tar`

### file list

```diff
@@ -1,804 +1,806 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.584757 resotocore-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-30 19:24:13.000000 resotocore-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-30 19:24:13.000000 resotocore-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17709 2023-06-30 19:29:18.584757 resotocore-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-30 19:24:13.000000 resotocore-3.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-30 19:24:13.000000 resotocore-3.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.392756 resotocore-3.6.0/resotocore/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12630 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.392756 resotocore-3.6.0/resotocore/action_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/action_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/action_handlers/merge_outer_edge_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.396756 resotocore-3.6.0/resotocore/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/analytics/posthog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/analytics/recurrent_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/async_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.396756 resotocore-3.6.0/resotocore/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31065 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)   242365 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/cli/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)    26704 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/cli/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/cli/tip_of_the_day.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.396756 resotocore-3.6.0/resotocore/config/
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/config/config_handler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/config/config_override_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/config/core_config_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/console_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    33686 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/core_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.400756 resotocore-3.6.0/resotocore/db/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32054 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/arango_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/arangodb_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/arangodb_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21148 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/async_arangodb.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/configdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    14240 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/db_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/deferred_edge_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/entitydb.py
--rw-r--r--   0 runner    (1001) docker     (123)    64492 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/graphdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/jobdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/modeldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/packagedb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/runningtaskdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/subscriberdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/system_data_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/db/templatedb.py
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.400756 resotocore-3.6.0/resotocore/graph_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/graph_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/graph_manager/graph_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/ids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.404756 resotocore-3.6.0/resotocore/infra_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/infra_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/infra_apps/local_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/infra_apps/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/infra_apps/package_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/infra_apps/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.404756 resotocore-3.6.0/resotocore/jupyterlite/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.376756 resotocore-3.6.0/resotocore/jupyterlite/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.404756 resotocore-3.6.0/resotocore/jupyterlite/api/contents/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-30 19:29:13.000000 resotocore-3.6.0/resotocore/jupyterlite/api/contents/all.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.404756 resotocore-3.6.0/resotocore/jupyterlite/api/translations/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-30 19:29:13.000000 resotocore-3.6.0/resotocore/jupyterlite/api/translations/all.json
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-30 19:29:13.000000 resotocore-3.6.0/resotocore/jupyterlite/api/translations/en.json
--rw-r--r--   0 runner    (1001) docker     (123)     3223 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/bootstrap.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.504756 resotocore-3.6.0/resotocore/jupyterlite/build/
--rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1037.51967a2.js
--rw-r--r--   0 runner    (1001) docker     (123)    21710 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1079.cdbaf67.js
--rw-r--r--   0 runner    (1001) docker     (123)     9647 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1084.4cd1c89.js
--rw-r--r--   0 runner    (1001) docker     (123)     1950 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1113.23c9417.js
--rw-r--r--   0 runner    (1001) docker     (123)     9736 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1125.129d070.js
--rw-r--r--   0 runner    (1001) docker     (123)     9342 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1163.ac28297.js
--rw-r--r--   0 runner    (1001) docker     (123)    74541 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1221.c51249a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1245.be46619.js
--rw-r--r--   0 runner    (1001) docker     (123)     9525 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1261.199fc1d.js
--rw-r--r--   0 runner    (1001) docker     (123)    10027 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1272.f334098.js
--rw-r--r--   0 runner    (1001) docker     (123)    14792 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1278.0524a4a.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1290.3981211.js
--rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1295.46e72b8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3404 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1310.23bbe67.js
--rw-r--r--   0 runner    (1001) docker     (123)    10986 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1320.21effe3.js
--rw-r--r--   0 runner    (1001) docker     (123)     6216 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1325.f76267c.js
--rw-r--r--   0 runner    (1001) docker     (123)     7061 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1408.7461890.js
--rw-r--r--   0 runner    (1001) docker     (123)     2273 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1440.a9e7ea1.js
--rw-r--r--   0 runner    (1001) docker     (123)    23820 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1483.616d9ab.js
--rw-r--r--   0 runner    (1001) docker     (123)    47542 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1489.e50b6d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     2605 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1507.5705605.js
--rw-r--r--   0 runner    (1001) docker     (123)      624 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/152.525d460.js
--rw-r--r--   0 runner    (1001) docker     (123)    36869 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1520.4e2eb21.js
--rw-r--r--   0 runner    (1001) docker     (123)     1533 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1555.e188f3f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8584 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1559.7c89925.js
--rw-r--r--   0 runner    (1001) docker     (123)     9056 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/160.5f28731.js
--rw-r--r--   0 runner    (1001) docker     (123)   478144 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1603.370a2a6.js
--rw-r--r--   0 runner    (1001) docker     (123)    22415 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1644.0e49167.js
--rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1667.f0afb2b.js
--rw-r--r--   0 runner    (1001) docker     (123)    17330 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1687.27f1ad6.js
--rw-r--r--   0 runner    (1001) docker     (123)   272197 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1725.f151c33.js
--rw-r--r--   0 runner    (1001) docker     (123)    25316 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1767.c8c2f26.js
--rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1806.1aaf66b.js
--rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1838.1202b16.js
--rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1909.28a2def.js
--rw-r--r--   0 runner    (1001) docker     (123)     9485 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/1989.88d258f.js
--rw-r--r--   0 runner    (1001) docker     (123)    89976 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2030.1562cc6.js
--rw-r--r--   0 runner    (1001) docker     (123)     6343 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2047.baed97b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2099.f4b6fcd.js
--rw-r--r--   0 runner    (1001) docker     (123)     6160 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2118.5b65f70.js
--rw-r--r--   0 runner    (1001) docker     (123)     3149 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/213.5769e57.js
--rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2161.dcb27b8.js
--rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2169.635c88e.js
--rw-r--r--   0 runner    (1001) docker     (123)    17630 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/217.90d10e2.js
--rw-r--r--   0 runner    (1001) docker     (123)    35022 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2212.72be094.js
--rw-r--r--   0 runner    (1001) docker     (123)   123689 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2287.997c38e.js
--rw-r--r--   0 runner    (1001) docker     (123)      545 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2303.9ff8710.js
--rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2319.6b4cbb7.js
--rw-r--r--   0 runner    (1001) docker     (123)     2648 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2329.4c5ca6d.js
--rw-r--r--   0 runner    (1001) docker     (123)     8667 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2351.fbd96d8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2358.d5cf7c8.js
--rw-r--r--   0 runner    (1001) docker     (123)     7913 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2359.6451c3e.js
--rw-r--r--   0 runner    (1001) docker     (123)     9289 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/237.f765e77.js
--rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2384.71782be.js
--rw-r--r--   0 runner    (1001) docker     (123)     4763 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/240.cddc46b.js
--rw-r--r--   0 runner    (1001) docker     (123)    15476 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2431.648d237.js
--rw-r--r--   0 runner    (1001) docker     (123)    12395 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2546.1f48267.js
--rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2557.75e9da2.js
--rw-r--r--   0 runner    (1001) docker     (123)     4176 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/261.5f53c0e.js
--rw-r--r--   0 runner    (1001) docker     (123)     8923 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2629.c0e1cd6.js
--rw-r--r--   0 runner    (1001) docker     (123)     2328 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2788.46acc8a.js
--rw-r--r--   0 runner    (1001) docker     (123)     8591 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2834.942acc6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2887.47ba752.js
--rw-r--r--   0 runner    (1001) docker     (123)     8870 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2956.8880209.js
--rw-r--r--   0 runner    (1001) docker     (123)     4300 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/2973.2a51dc4.js
--rw-r--r--   0 runner    (1001) docker     (123)     8060 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3004.255e79c.js
--rw-r--r--   0 runner    (1001) docker     (123)    17042 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/302.8bcc38f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8560 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3037.70ee38d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3042.7cfad84.js
--rw-r--r--   0 runner    (1001) docker     (123)    10136 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3051.34fac68.js
--rw-r--r--   0 runner    (1001) docker     (123)     9664 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3122.2289fca.js
--rw-r--r--   0 runner    (1001) docker     (123)     2550 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3151.10ef4de.js
--rw-r--r--   0 runner    (1001) docker     (123)    15850 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/316.c850a76.js
--rw-r--r--   0 runner    (1001) docker     (123)    20975 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3196.4e35a17.js
--rw-r--r--   0 runner    (1001) docker     (123)    16159 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3265.a80440a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3277.9c04e75.js
--rw-r--r--   0 runner    (1001) docker     (123)     8847 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/330.126fa98.js
--rw-r--r--   0 runner    (1001) docker     (123)    14007 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3392.29fe6b9.js
--rw-r--r--   0 runner    (1001) docker     (123)    80815 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3413.480a49d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3444.47d5ea1.js
--rw-r--r--   0 runner    (1001) docker     (123)     1863 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3469.7d14d0b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9554 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3546.fee1bd7.js
--rw-r--r--   0 runner    (1001) docker     (123)     5145 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/362.6716970.js
--rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3708.410d087.js
--rw-r--r--   0 runner    (1001) docker     (123)      170 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3752.8735345.js
--rw-r--r--   0 runner    (1001) docker     (123)    16215 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3850.903abc2.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3433 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3880.bd39dce.js
--rw-r--r--   0 runner    (1001) docker     (123)    10216 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3970.236586f.js
--rw-r--r--   0 runner    (1001) docker     (123)   897822 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3976.58893b9.js
--rw-r--r--   0 runner    (1001) docker     (123)     2025 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16446 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/3979.385527e.js
--rw-r--r--   0 runner    (1001) docker     (123)    11331 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/400.d72234b.js
--rw-r--r--   0 runner    (1001) docker     (123)    11916 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4018.1a35967.js
--rw-r--r--   0 runner    (1001) docker     (123)     9851 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/406.9b7af92.js
--rw-r--r--   0 runner    (1001) docker     (123)    11111 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4117.a8107fd.js
--rw-r--r--   0 runner    (1001) docker     (123)    10886 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4182.e2430f9.js
--rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4191.02bbea8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4197.53ab10b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9224 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4206.a5f8bb0.js
--rw-r--r--   0 runner    (1001) docker     (123)     8525 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4207.0d0580b.js
--rw-r--r--   0 runner    (1001) docker     (123)    10616 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4262.bb73457.js
--rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4298.5ee510c.js
--rw-r--r--   0 runner    (1001) docker     (123)    83844 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/44.0cfa785.js
--rw-r--r--   0 runner    (1001) docker     (123)     1021 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4410.e4a25d3.js
--rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4466.64d23d1.js
--rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4507.8b41ef4.js
--rw-r--r--   0 runner    (1001) docker     (123)     7852 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/451.d9683ad.js
--rw-r--r--   0 runner    (1001) docker     (123)     2977 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4535.34b060a.js
--rw-r--r--   0 runner    (1001) docker     (123)    20495 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4565.43bdb91.js
--rw-r--r--   0 runner    (1001) docker     (123)    22220 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4569.f374f9d.js
--rw-r--r--   0 runner    (1001) docker     (123)    91604 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4615.eb5d40a.js
--rw-r--r--   0 runner    (1001) docker     (123)   119541 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4658.090d4a9.js
--rw-r--r--   0 runner    (1001) docker     (123)       95 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4658.090d4a9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4665.aa19a41.js
--rw-r--r--   0 runner    (1001) docker     (123)      142 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4668.f65690b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4695 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4690.3dd4096.js
--rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4715.e7690b9.js
--rw-r--r--   0 runner    (1001) docker     (123)    10282 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4749.46ebbb2.js
--rw-r--r--   0 runner    (1001) docker     (123)     9653 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4750.56c06ab.js
--rw-r--r--   0 runner    (1001) docker     (123)    17648 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4856.2d7415f.js
--rw-r--r--   0 runner    (1001) docker     (123)    41909 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4875.375150e.js
--rw-r--r--   0 runner    (1001) docker     (123)     6350 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/489.b981dea.js
--rw-r--r--   0 runner    (1001) docker     (123)     2209 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/490.c2624d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     2796 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4905.667bf33.js
--rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4931.430433b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/4942.b96c164.js
--rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5016.dd2fe83.js
--rw-r--r--   0 runner    (1001) docker     (123)     5766 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5072.733a1b5.js
--rw-r--r--   0 runner    (1001) docker     (123)     2604 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/509.6448878.js
--rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5096.8ed0d8e.js
--rw-r--r--   0 runner    (1001) docker     (123)     4581 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5126.eecad7a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5129.1ba4763.js
--rw-r--r--   0 runner    (1001) docker     (123)     6272 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5153.763d8fa.js
--rw-r--r--   0 runner    (1001) docker     (123)      618 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5155.06b4ea9.js
--rw-r--r--   0 runner    (1001) docker     (123)    32726 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5193.e9f6866.js
--rw-r--r--   0 runner    (1001) docker     (123)     9808 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5213.3e1a360.js
--rw-r--r--   0 runner    (1001) docker     (123)     8503 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5227.8c8acd8.js
--rw-r--r--   0 runner    (1001) docker     (123)    11129 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5238.1751cc3.js
--rw-r--r--   0 runner    (1001) docker     (123)     5579 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/528.2262cb0.js
--rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5292.79d4aba.js
--rw-r--r--   0 runner    (1001) docker     (123)     7706 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5437.31236f7.js
--rw-r--r--   0 runner    (1001) docker     (123)    10580 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5489.848a8cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     5146 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5508.317fca3.js
--rw-r--r--   0 runner    (1001) docker     (123)     9068 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/554.ac98303.js
--rw-r--r--   0 runner    (1001) docker     (123)     2549 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/555.2cd31dd.js
--rw-r--r--   0 runner    (1001) docker     (123)    16702 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5573.ebcdb93.js
--rw-r--r--   0 runner    (1001) docker     (123)   171864 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5666.c5e5324.js
--rw-r--r--   0 runner    (1001) docker     (123)     8628 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5710.70d0b1d.js
--rw-r--r--   0 runner    (1001) docker     (123)   172015 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5747.94ad626.js
--rw-r--r--   0 runner    (1001) docker     (123)    14074 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/582.21b8e7d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5823.5045bdb.js
--rw-r--r--   0 runner    (1001) docker     (123)     2543 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5851.30b7b2a.js
--rw-r--r--   0 runner    (1001) docker     (123)   257877 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5878.32d92fa.js
--rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5880.68f975b.js
--rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5955.88508f7.js
--rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/5971.88c5642.js
--rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6080.aa0ff24.js
--rw-r--r--   0 runner    (1001) docker     (123)    28010 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/61.2808a0d.js
--rw-r--r--   0 runner    (1001) docker     (123)    18045 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6136.b8ba2b2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1343 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6141.9831d58.js
--rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6475.6037fbb.js
--rw-r--r--   0 runner    (1001) docker     (123)     7434 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6493.d796aa5.js
--rw-r--r--   0 runner    (1001) docker     (123)     4963 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6556.b3d9293.js
--rw-r--r--   0 runner    (1001) docker     (123)     5803 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6571.2c8884e.js
--rw-r--r--   0 runner    (1001) docker     (123)    10586 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6576.3ea568e.js
--rw-r--r--   0 runner    (1001) docker     (123)    83397 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6591.94ed352.js
--rw-r--r--   0 runner    (1001) docker     (123)     7388 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6612.1632879.js
--rw-r--r--   0 runner    (1001) docker     (123)   246379 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6623.ae3b3cc.js
--rw-r--r--   0 runner    (1001) docker     (123)      160 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6623.ae3b3cc.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16150 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6664.2160109.js
--rw-r--r--   0 runner    (1001) docker     (123)     9611 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6747.47be7f5.js
--rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6748.be68f5f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8961 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6870.7940288.js
--rw-r--r--   0 runner    (1001) docker     (123)    11058 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6879.c8367a5.js
--rw-r--r--   0 runner    (1001) docker     (123)    16507 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6898.9bbc12a.js
--rw-r--r--   0 runner    (1001) docker     (123)    10256 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6952.f68b818.js
--rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6985.321ad92.js
--rw-r--r--   0 runner    (1001) docker     (123)    10925 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6993.32cf9a6.js
--rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/6997.b06fe71.js
--rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7041.d4f561e.js
--rw-r--r--   0 runner    (1001) docker     (123)    10338 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7058.805c88e.js
--rw-r--r--   0 runner    (1001) docker     (123)       51 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7058.805c88e.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7174.6c45206.js
--rw-r--r--   0 runner    (1001) docker     (123)    35260 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7334.8859b1b.js
--rw-r--r--   0 runner    (1001) docker     (123)     8497 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7359.6ee65ec.js
--rw-r--r--   0 runner    (1001) docker     (123)     3555 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7364.195178b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9117 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7380.58a4413.js
--rw-r--r--   0 runner    (1001) docker     (123)     7126 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7427.f9c2017.js
--rw-r--r--   0 runner    (1001) docker     (123)      294 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7427.f9c2017.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14994 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7463.18fd278.js
--rw-r--r--   0 runner    (1001) docker     (123)    10358 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7509.1e0189e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7526.1a303e5.js
--rw-r--r--   0 runner    (1001) docker     (123)    31492 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7537.1323a15.js
--rw-r--r--   0 runner    (1001) docker     (123)    10078 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7692.33d5169.js
--rw-r--r--   0 runner    (1001) docker     (123)      595 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7746.5908d29.js
--rw-r--r--   0 runner    (1001) docker     (123)    10754 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7808.1d582a2.js
--rw-r--r--   0 runner    (1001) docker     (123)     4962 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/783.c156751.js
--rw-r--r--   0 runner    (1001) docker     (123)     9192 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7858.2386e4d.js
--rw-r--r--   0 runner    (1001) docker     (123)    31628 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/7941.01ea680.js
--rw-r--r--   0 runner    (1001) docker     (123)     5753 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8005.c5ad7b2.js
--rw-r--r--   0 runner    (1001) docker     (123)     7966 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8028.39e2fa1.js
--rw-r--r--   0 runner    (1001) docker     (123)     9977 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8061.cc62561.js
--rw-r--r--   0 runner    (1001) docker     (123)   317511 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8101.cf46d02.js
--rw-r--r--   0 runner    (1001) docker     (123)       50 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8101.cf46d02.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7965 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/812.9b0e86e.js
--rw-r--r--   0 runner    (1001) docker     (123)      855 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/816.c8050f2.js
--rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8165.b2c3285.js
--rw-r--r--   0 runner    (1001) docker     (123)     3150 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8232.a578bf9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1142 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/824.8678196.js
--rw-r--r--   0 runner    (1001) docker     (123)    15838 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8270.89fe7e1.js
--rw-r--r--   0 runner    (1001) docker     (123)     2327 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/833.9cc6653.js
--rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8370.8f855e5.js
--rw-r--r--   0 runner    (1001) docker     (123)    10481 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8373.96b0b3a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2921 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8389.ffe031f.js
--rw-r--r--   0 runner    (1001) docker     (123)     6825 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8412.1528057.js
--rw-r--r--   0 runner    (1001) docker     (123)     9361 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8427.4923f43.js
--rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8542.027afdc.js
--rw-r--r--   0 runner    (1001) docker     (123)     8843 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8594.0112f03.js
--rw-r--r--   0 runner    (1001) docker     (123)    30005 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8656.d5b8e92.js
--rw-r--r--   0 runner    (1001) docker     (123)    12065 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8685.d78bdab.js
--rw-r--r--   0 runner    (1001) docker     (123)   114157 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8698.9817d75.js
--rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8732.9320f73.js
--rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8741.b138cb8.js
--rw-r--r--   0 runner    (1001) docker     (123)     2572 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8785.cf4fe95.js
--rw-r--r--   0 runner    (1001) docker     (123)    27799 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8828.77c71d0.js
--rw-r--r--   0 runner    (1001) docker     (123)     2950 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8883.80c7b63.js
--rw-r--r--   0 runner    (1001) docker     (123)     9758 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8976.3816942.js
--rw-r--r--   0 runner    (1001) docker     (123)      432 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8981.99a4275.js
--rw-r--r--   0 runner    (1001) docker     (123)     1931 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/8990.2a453cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9035.1e45c1b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4177 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9053.45b77fc.js
--rw-r--r--   0 runner    (1001) docker     (123)     9689 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9077.fefb6ca.js
--rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9128.b8fa6f0.js
--rw-r--r--   0 runner    (1001) docker     (123)     9225 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9156.0cefbd3.js
--rw-r--r--   0 runner    (1001) docker     (123)     2790 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9170.0023587.js
--rw-r--r--   0 runner    (1001) docker     (123)    10649 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9196.315f9f9.js
--rw-r--r--   0 runner    (1001) docker     (123)    28388 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9198.9971d70.js
--rw-r--r--   0 runner    (1001) docker     (123)   131443 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/920.d15c177.js
--rw-r--r--   0 runner    (1001) docker     (123)     4000 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9253.0b31caa.js
--rw-r--r--   0 runner    (1001) docker     (123)     8378 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9266.bacd0dd.js
--rw-r--r--   0 runner    (1001) docker     (123)      591 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9307.c3a00ed.js
--rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9321.869e413.js
--rw-r--r--   0 runner    (1001) docker     (123)  1188430 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9344.ba0abcf.js
--rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9382.9014799.js
--rw-r--r--   0 runner    (1001) docker     (123)    29226 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9440.1b10b8f.js
--rw-r--r--   0 runner    (1001) docker     (123)      163 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9440.1b10b8f.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9464.79e6ac5.js
--rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9502.9a24831.js
--rw-r--r--   0 runner    (1001) docker     (123)    32420 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9507.1e6cc5d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9206 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9602.62bf0f1.js
--rw-r--r--   0 runner    (1001) docker     (123)     9381 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9621.e2e8b5d.js
--rw-r--r--   0 runner    (1001) docker     (123)      625 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9622.ccab065.js
--rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9626.a178bd0.js
--rw-r--r--   0 runner    (1001) docker     (123)    10559 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9647.ed91993.js
--rw-r--r--   0 runner    (1001) docker     (123)   432928 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9657.bc5c60e.js
--rw-r--r--   0 runner    (1001) docker     (123)     9073 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/97.ad126b0.js
--rw-r--r--   0 runner    (1001) docker     (123)     2515 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9712.796a0a1.js
--rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9733.a3b2a7f.js
--rw-r--r--   0 runner    (1001) docker     (123)    36791 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9737.7dc8f98.js
--rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9777.0b8a504.js
--rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9793.6d63a85.js
--rw-r--r--   0 runner    (1001) docker     (123)    17595 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9806.652c162.js
--rw-r--r--   0 runner    (1001) docker     (123)   179318 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9865.2e3db6f.js
--rw-r--r--   0 runner    (1001) docker     (123)      246 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9865.2e3db6f.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4299 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/989.bcca86a.js
--rw-r--r--   0 runner    (1001) docker     (123)    14270 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9943.f3f35c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    18136 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9958.25c8c06.js
--rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/9960.64cd61e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1131 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/add-above.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1210 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/add-below.svg
--rw-r--r--   0 runner    (1001) docker     (123)      227 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/add.svg
--rw-r--r--   0 runner    (1001) docker     (123)      942 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/bug-dot.svg
--rw-r--r--   0 runner    (1001) docker     (123)      585 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/bug.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2481 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/build.svg
--rw-r--r--   0 runner    (1001) docker     (123)      301 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/caret-down-empty-thin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/caret-down-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/caret-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/caret-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      262 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/caret-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/caret-up-empty-thin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/caret-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1143 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/case-sensitive.svg
--rw-r--r--   0 runner    (1001) docker     (123)      260 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/check.svg
--rw-r--r--   0 runner    (1001) docker     (123)      316 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/circle-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)      209 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/circle.svg
--rw-r--r--   0 runner    (1001) docker     (123)      452 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/clear.svg
--rw-r--r--   0 runner    (1001) docker     (123)      562 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/close.svg
--rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/code.svg
--rw-r--r--   0 runner    (1001) docker     (123)      423 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/console.svg
--rw-r--r--   0 runner    (1001) docker     (123)      391 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/copy.svg
--rw-r--r--   0 runner    (1001) docker     (123)      623 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/copyright.svg
--rw-r--r--   0 runner    (1001) docker     (123)      602 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/cut.svg
--rw-r--r--   0 runner    (1001) docker     (123)      312 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/delete.svg
--rw-r--r--   0 runner    (1001) docker     (123)      233 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/download.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1384 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/duplicate.svg
--rw-r--r--   0 runner    (1001) docker     (123)      341 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/edit.svg
--rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/ellipses.svg
--rw-r--r--   0 runner    (1001) docker     (123)      484 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/extension.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76736 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13224 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78268 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      243 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/fast-forward.svg
--rw-r--r--   0 runner    (1001) docker     (123)      229 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/file-upload.svg
--rw-r--r--   0 runner    (1001) docker     (123)      461 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/file.svg
--rw-r--r--   0 runner    (1001) docker     (123)      238 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/filter-list.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/folder-favorite.svg
--rw-r--r--   0 runner    (1001) docker     (123)      285 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/home.svg
--rw-r--r--   0 runner    (1001) docker     (123)      891 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/html5.svg
--rw-r--r--   0 runner    (1001) docker     (123)      454 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/image.svg
--rw-r--r--   0 runner    (1001) docker     (123)      322 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/inspector.svg
--rw-r--r--   0 runner    (1001) docker     (123)      923 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/json.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/julia.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1151 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/jupyter-favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2765 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/jupyter.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4156 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/jupyterlab-wordmark.svg
--rw-r--r--   0 runner    (1001) docker     (123)      368 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/kernel.svg
--rw-r--r--   0 runner    (1001) docker     (123)      434 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/keyboard.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.508756 resotocore-3.6.0/resotocore/jupyterlite/build/lab/
--rw-r--r--   0 runner    (1001) docker     (123)    54484 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/lab/bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)      411 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/launch.svg
--rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/launcher.svg
--rw-r--r--   0 runner    (1001) docker     (123)      200 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/line-form.svg
--rw-r--r--   0 runner    (1001) docker     (123)      403 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/link.svg
--rw-r--r--   0 runner    (1001) docker     (123)      371 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/list.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1674 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/listings-info.svg
--rw-r--r--   0 runner    (1001) docker     (123)      428 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/markdown.svg
--rw-r--r--   0 runner    (1001) docker     (123)      600 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/move-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      610 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/move-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/new-folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      899 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/not-trusted.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/notebook.svg
--rw-r--r--   0 runner    (1001) docker     (123)      355 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/numbering.svg
--rw-r--r--   0 runner    (1001) docker     (123)      330 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/offline-bolt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/palette.svg
--rw-r--r--   0 runner    (1001) docker     (123)      404 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/paste.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1893 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/python.svg
--rw-r--r--   0 runner    (1001) docker     (123)      473 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/r-kernel.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2734 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/react.svg
--rw-r--r--   0 runner    (1001) docker     (123)      388 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/redo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/refresh.svg
--rw-r--r--   0 runner    (1001) docker     (123)      620 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/regex.svg
--rw-r--r--   0 runner    (1001) docker     (123)      217 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/run.svg
--rw-r--r--   0 runner    (1001) docker     (123)      364 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/running.svg
--rw-r--r--   0 runner    (1001) docker     (123)      346 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/save.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.508756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.380756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.508756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2971 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json
--rw-r--r--   0 runner    (1001) docker     (123)     3219 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json
--rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json
--rw-r--r--   0 runner    (1001) docker     (123)      763 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.508756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      746 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json
--rw-r--r--   0 runner    (1001) docker     (123)      563 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json
--rw-r--r--   0 runner    (1001) docker     (123)     3717 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json
--rw-r--r--   0 runner    (1001) docker     (123)      457 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/workspaces.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.508756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.508756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     6730 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.512756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      343 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/files.json
--rw-r--r--   0 runner    (1001) docker     (123)      348 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.512756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      365 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/foreign.json
--rw-r--r--   0 runner    (1001) docker     (123)     6167 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.512756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json
--rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.512756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      465 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/download.json
--rw-r--r--   0 runner    (1001) docker     (123)     3587 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.516756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.516756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     5970 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json
--rw-r--r--   0 runner    (1001) docker     (123)      513 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json
--rw-r--r--   0 runner    (1001) docker     (123)      385 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
--rw-r--r--   0 runner    (1001) docker     (123)      477 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-with.json
--rw-r--r--   0 runner    (1001) docker     (123)     2310 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.516756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     8578 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.516756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      422 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/about.json
--rw-r--r--   0 runner    (1001) docker     (123)      456 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/jupyter-forum.json
--rw-r--r--   0 runner    (1001) docker     (123)      466 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/launch-classic.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.516756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.516756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.520756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      332 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      655 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json
--rw-r--r--   0 runner    (1001) docker     (123)      319 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.520756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.520756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.520756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     9894 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.520756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2325 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.520756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      672 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json
--rw-r--r--   0 runner    (1001) docker     (123)     2932 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json
--rw-r--r--   0 runner    (1001) docker     (123)    24989 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.520756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      389 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/form-ui.json
--rw-r--r--   0 runner    (1001) docker     (123)      440 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.520756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.520756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.520756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.524757 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      551 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      402 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/files.json
--rw-r--r--   0 runner    (1001) docker     (123)      572 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.524757 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.380756 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@retrolab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.524757 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      463 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/menus.json
--rw-r--r--   0 runner    (1001) docker     (123)      443 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/top.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.524757 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      491 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/scroll-output.json
--rw-r--r--   0 runner    (1001) docker     (123)    79291 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/schemas/all.json
--rw-r--r--   0 runner    (1001) docker     (123)      439 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/search.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/service-worker-b2fb40a.js
--rw-r--r--   0 runner    (1001) docker     (123)      860 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/settings.svg
--rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/spreadsheet.svg
--rw-r--r--   0 runner    (1001) docker     (123)      259 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/stop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/tab.svg
--rw-r--r--   0 runner    (1001) docker     (123)      297 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/table-rows.svg
--rw-r--r--   0 runner    (1001) docker     (123)      825 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/tag.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2552 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/terminal.svg
--rw-r--r--   0 runner    (1001) docker     (123)      270 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/text-editor.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.380756 resotocore-3.6.0/resotocore/jupyterlite/build/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.380756 resotocore-3.6.0/resotocore/jupyterlite/build/themes/@jupyterlab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.524757 resotocore-3.6.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/
--rw-r--r--   0 runner    (1001) docker     (123)    16232 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.524757 resotocore-3.6.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/
--rw-r--r--   0 runner    (1001) docker     (123)    15136 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.js
--rw-r--r--   0 runner    (1001) docker     (123)   310614 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)      538 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/toc.svg
--rw-r--r--   0 runner    (1001) docker     (123)      300 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/tree-view.svg
--rw-r--r--   0 runner    (1001) docker     (123)      828 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/trusted.svg
--rw-r--r--   0 runner    (1001) docker     (123)      334 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/undo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      382 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/vega.svg
--rw-r--r--   0 runner    (1001) docker     (123)      426 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/build/yaml.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7192 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/config-utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.380756 resotocore-3.6.0/resotocore/jupyterlite/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.524757 resotocore-3.6.0/resotocore/jupyterlite/doc/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      295 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/doc/workspaces/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.384756 resotocore-3.6.0/resotocore/jupyterlite/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.380756 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.524757 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2562 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.528756 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)     8738 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    27007 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      621 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     4825 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     8374 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    15897 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.528756 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/
--rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/install.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     2633 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.532756 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)     8195 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js
--rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     6063 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js
--rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     2532 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js
--rw-rw-rw-   0 runner    (1001) docker     (123)   165727 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.532756 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/
--rw-rw-rw-   0 runner    (1001) docker     (123)     4270 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     6512 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     6720 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     8221 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     7915 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.536756 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/
--rw-rw-rw-   0 runner    (1001) docker     (123)     1081 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     2657 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json
--rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    14685 2023-06-30 19:29:09.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.536756 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2732 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.544757 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2643 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     8368 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js
--rw-rw-rw-   0 runner    (1001) docker     (123)  3578814 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     1110 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)    70520 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      336 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     2360 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    14737 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     7706 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     5802 2023-06-30 19:28:56.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.544757 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/
--rw-rw-rw-   0 runner    (1001) docker     (123)      199 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/install.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     3508 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.544757 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)      224 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/568.1e2faa2ba0bbe59c4780.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     7753 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     3889 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      162 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     2452 2023-06-30 19:29:05.000000 resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.544757 resotocore-3.6.0/resotocore/jupyterlite/files/
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/jupyterlite/files/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4609 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (123)    20954 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/icon-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)     2513 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/jupyter-lite.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-30 19:29:13.000000 resotocore-3.6.0/resotocore/jupyterlite/jupyter-lite.json
--rw-r--r--   0 runner    (1001) docker     (123)    11794 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/jupyterlite.schema.v0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.544757 resotocore-3.6.0/resotocore/jupyterlite/kernelspecs/
--rw-r--r--   0 runner    (1001) docker     (123)      777 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/kernelspecs/javascript.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.548756 resotocore-3.6.0/resotocore/jupyterlite/lab/
--rw-r--r--   0 runner    (1001) docker     (123)   324251 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/lab/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      993 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/lab/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/lab/jupyter-lite.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      144 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/lab/jupyter-lite.json
--rw-r--r--   0 runner    (1001) docker     (123)    10101 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/lab/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.548756 resotocore-3.6.0/resotocore/jupyterlite/lab/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      290 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/lab/tree/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.548756 resotocore-3.6.0/resotocore/jupyterlite/lab/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/lab/workspaces/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      690 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/manifest.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)     1307 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/service-worker-b2fb40a.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.548756 resotocore-3.6.0/resotocore/jupyterlite/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      304 1985-10-26 08:15:00.000000 resotocore-3.6.0/resotocore/jupyterlite/tree/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/message_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.552757 resotocore-3.6.0/resotocore/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/model/adjust_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/model/db_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    26304 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/model/graph_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/model/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    58079 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/model/model_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/model/resolve_in_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/model/transform_kind_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/model/typed_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.552757 resotocore-3.6.0/resotocore/query/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48513 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/query/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/query/query_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/query/template_expander.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/query/template_expander_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.552757 resotocore-3.6.0/resotocore/report/
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/report/benchmark_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/report/inspector_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/report/report_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.556757 resotocore-3.6.0/resotocore/static/
--rw-r--r--   0 runner    (1001) docker     (123)   129588 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/api-doc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/ck-unicode-truecolor.ans
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.556757 resotocore-3.6.0/resotocore/static/report/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.384756 resotocore-3.6.0/resotocore/static/report/benchmark/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.556757 resotocore-3.6.0/resotocore/static/report/benchmark/aws/
--rw-r--r--   0 runner    (1001) docker     (123)    43058 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/benchmark/aws/aws_cis_1_5.json
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/benchmark_template.json
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/check_template.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.384756 resotocore-3.6.0/resotocore/static/report/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.560757 resotocore-3.6.0/resotocore/static/report/checks/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/checks/aws/aws_apigateway.json
--rw-r--r--   0 runner    (1001) docker     (123)    33970 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/checks/aws/aws_cloudtrail.json
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/checks/aws/aws_config.json
--rw-r--r--   0 runner    (1001) docker     (123)    46657 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/checks/aws/aws_ec2.json
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/checks/aws/aws_efs.json
--rw-r--r--   0 runner    (1001) docker     (123)    24445 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/checks/aws/aws_iam.json
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/checks/aws/aws_kms.json
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/checks/aws/aws_lambda.json
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/checks/aws/aws_rds.json
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/report/checks/aws/aws_s3.json
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/resoto.css
--rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/static/resoto_logo_and_text.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.560757 resotocore-3.6.0/resotocore/task/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/task/job_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/task/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/task/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/task/start_workflow_on_first_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/task/subscribers.py
--rw-r--r--   0 runner    (1001) docker     (123)    30956 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/task/task_description.py
--rw-r--r--   0 runner    (1001) docker     (123)    28462 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/task/task_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.564756 resotocore-3.6.0/resotocore/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/templates/create_first_user.html
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.564756 resotocore-3.6.0/resotocore/user/
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/user/user_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.564756 resotocore-3.6.0/resotocore/web/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66253 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/web/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/web/certificate_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/web/content_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/web/directives.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/web/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/web/tsdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-06-30 19:24:13.000000 resotocore-3.6.0/resotocore/worker_task_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.392756 resotocore-3.6.0/resotocore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17709 2023-06-30 19:29:18.000000 resotocore-3.6.0/resotocore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34481 2023-06-30 19:29:18.000000 resotocore-3.6.0/resotocore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:29:18.000000 resotocore-3.6.0/resotocore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 19:29:18.000000 resotocore-3.6.0/resotocore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:29:17.000000 resotocore-3.6.0/resotocore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-30 19:29:18.000000 resotocore-3.6.0/resotocore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-30 19:29:18.000000 resotocore-3.6.0/resotocore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-30 19:29:18.584757 resotocore-3.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.564756 resotocore-3.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.568757 resotocore-3.6.0/tests/resotocore/
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.568757 resotocore-3.6.0/tests/resotocore/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/analytics/posthog_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/analytics/recurrent_events_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.568757 resotocore-3.6.0/tests/resotocore/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/cli/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    59377 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/cli/command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/cli/model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.572757 resotocore-3.6.0/tests/resotocore/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12759 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/config/config_handler_service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/config/config_override_service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/config/core_config_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27737 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/console_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/core_config_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.576757 resotocore-3.6.0/tests/resotocore/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/arango_query_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/arangodb_functions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/async_arangodb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/configdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/db_access_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/entitydb.py
--rw-r--r--   0 runner    (1001) docker     (123)    29413 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/graphdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/jobdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/modeldb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/runningtaskdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/subscriberdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/system_data_db_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/db/templatedb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/dependencies_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.576757 resotocore-3.6.0/tests/resotocore/graph_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/graph_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/graph_manager/graph_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/hypothesis_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.576757 resotocore-3.6.0/tests/resotocore/infra_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/infra_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/infra_apps/local_runtime_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/infra_apps/package_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/message_bus_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.580757 resotocore-3.6.0/tests/resotocore/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/model/adjust_node_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/model/db_updater_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16464 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/model/graph_access_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/model/json_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/model/model_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    24923 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/model/model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/model/resolve_in_graph_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/model/typed_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.580757 resotocore-3.6.0/tests/resotocore/query/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/query/model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/query/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/query/template_expander_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.580757 resotocore-3.6.0/tests/resotocore/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/report/benchnmark_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/report/inspector_service_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.584757 resotocore-3.6.0/tests/resotocore/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/task/job_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/task/start_workflow_on_first_subscriber_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/task/subscribers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/task/task_description_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/task/task_handler_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.584757 resotocore-3.6.0/tests/resotocore/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/user/user_management_service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/util_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/validator_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:29:18.584757 resotocore-3.6.0/tests/resotocore/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/web/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/web/api_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/web/certificate_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/web/content_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-30 19:24:13.000000 resotocore-3.6.0/tests/resotocore/worker_task_queue_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.377378 resotocore-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 16:55:53.000000 resotocore-3.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-14 16:55:53.000000 resotocore-3.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17709 2023-07-14 17:01:36.377378 resotocore-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-14 16:55:53.000000 resotocore-3.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-14 16:55:53.000000 resotocore-3.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.149377 resotocore-3.6.1/resotocore/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.153377 resotocore-3.6.1/resotocore/action_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/action_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/action_handlers/merge_outer_edge_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.153377 resotocore-3.6.1/resotocore/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/analytics/posthog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/analytics/recurrent_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/async_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.153377 resotocore-3.6.1/resotocore/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31097 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)   241878 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/cli/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/cli/tip_of_the_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.157377 resotocore-3.6.1/resotocore/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/config/config_handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/config/config_override_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/config/core_config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/console_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33844 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/core_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.161377 resotocore-3.6.1/resotocore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34739 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/arango_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/arangodb_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/arangodb_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20693 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/async_arangodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/configdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13991 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/db_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/deferred_edge_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/entitydb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65689 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/graphdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/jobdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/modeldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/packagedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/runningtaskdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/subscriberdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/system_data_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/templatedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/db/usagedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.161377 resotocore-3.6.1/resotocore/graph_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/graph_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/graph_manager/graph_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.161377 resotocore-3.6.1/resotocore/infra_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/infra_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/infra_apps/local_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/infra_apps/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/infra_apps/package_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/infra_apps/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.165377 resotocore-3.6.1/resotocore/jupyterlite/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.133377 resotocore-3.6.1/resotocore/jupyterlite/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.165377 resotocore-3.6.1/resotocore/jupyterlite/api/contents/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-14 17:01:30.000000 resotocore-3.6.1/resotocore/jupyterlite/api/contents/all.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.165377 resotocore-3.6.1/resotocore/jupyterlite/api/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-14 17:01:30.000000 resotocore-3.6.1/resotocore/jupyterlite/api/translations/all.json
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 17:01:30.000000 resotocore-3.6.1/resotocore/jupyterlite/api/translations/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/bootstrap.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.285378 resotocore-3.6.1/resotocore/jupyterlite/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1037.51967a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21710 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1079.cdbaf67.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1084.4cd1c89.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1113.23c9417.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9736 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1125.129d070.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1163.ac28297.js
+-rw-r--r--   0 runner    (1001) docker     (123)    74541 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1221.c51249a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1245.be46619.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9525 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1261.199fc1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1272.f334098.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14792 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1278.0524a4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1290.3981211.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1295.46e72b8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1310.23bbe67.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1320.21effe3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1325.f76267c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1408.7461890.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1440.a9e7ea1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23820 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1483.616d9ab.js
+-rw-r--r--   0 runner    (1001) docker     (123)    47542 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1489.e50b6d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1507.5705605.js
+-rw-r--r--   0 runner    (1001) docker     (123)      624 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/152.525d460.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36869 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1520.4e2eb21.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1555.e188f3f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1559.7c89925.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/160.5f28731.js
+-rw-r--r--   0 runner    (1001) docker     (123)   478144 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1603.370a2a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22415 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1644.0e49167.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1667.f0afb2b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17330 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1687.27f1ad6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   272197 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1725.f151c33.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25316 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1767.c8c2f26.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1806.1aaf66b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1838.1202b16.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1909.28a2def.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/1989.88d258f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89976 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2030.1562cc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2047.baed97b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2099.f4b6fcd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2118.5b65f70.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/213.5769e57.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2161.dcb27b8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2169.635c88e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17630 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/217.90d10e2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35022 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2212.72be094.js
+-rw-r--r--   0 runner    (1001) docker     (123)   123689 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2287.997c38e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      545 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2303.9ff8710.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2319.6b4cbb7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2329.4c5ca6d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2351.fbd96d8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2358.d5cf7c8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7913 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2359.6451c3e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/237.f765e77.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2384.71782be.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/240.cddc46b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15476 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2431.648d237.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2546.1f48267.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2557.75e9da2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/261.5f53c0e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2629.c0e1cd6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2788.46acc8a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2834.942acc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2887.47ba752.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2956.8880209.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/2973.2a51dc4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3004.255e79c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17042 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/302.8bcc38f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3037.70ee38d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3042.7cfad84.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10136 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3051.34fac68.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3122.2289fca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3151.10ef4de.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15850 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/316.c850a76.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20975 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3196.4e35a17.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16159 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3265.a80440a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3277.9c04e75.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8847 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/330.126fa98.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14007 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3392.29fe6b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    80815 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3413.480a49d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3444.47d5ea1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3469.7d14d0b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3546.fee1bd7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/362.6716970.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3708.410d087.js
+-rw-r--r--   0 runner    (1001) docker     (123)      170 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3752.8735345.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16215 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3850.903abc2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3880.bd39dce.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3970.236586f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   897822 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3976.58893b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16446 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/3979.385527e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11331 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/400.d72234b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11916 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4018.1a35967.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/406.9b7af92.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11111 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4117.a8107fd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10886 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4182.e2430f9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4191.02bbea8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4197.53ab10b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4206.a5f8bb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4207.0d0580b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4262.bb73457.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4298.5ee510c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    83844 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/44.0cfa785.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4410.e4a25d3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4466.64d23d1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4507.8b41ef4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/451.d9683ad.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4535.34b060a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20495 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4565.43bdb91.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22220 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4569.f374f9d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91604 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4615.eb5d40a.js
+-rw-r--r--   0 runner    (1001) docker     (123)   119541 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4658.090d4a9.js
+-rw-r--r--   0 runner    (1001) docker     (123)       95 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4658.090d4a9.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4665.aa19a41.js
+-rw-r--r--   0 runner    (1001) docker     (123)      142 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4668.f65690b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4690.3dd4096.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4715.e7690b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4749.46ebbb2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9653 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4750.56c06ab.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17648 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4856.2d7415f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41909 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4875.375150e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/489.b981dea.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/490.c2624d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4905.667bf33.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4931.430433b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/4942.b96c164.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5016.dd2fe83.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5072.733a1b5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/509.6448878.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5096.8ed0d8e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5126.eecad7a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5129.1ba4763.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5153.763d8fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)      618 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5155.06b4ea9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32726 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5193.e9f6866.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9808 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5213.3e1a360.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5227.8c8acd8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5238.1751cc3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/528.2262cb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5292.79d4aba.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7706 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5437.31236f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5489.848a8cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5508.317fca3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9068 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/554.ac98303.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/555.2cd31dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16702 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5573.ebcdb93.js
+-rw-r--r--   0 runner    (1001) docker     (123)   171864 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5666.c5e5324.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5710.70d0b1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)   172015 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5747.94ad626.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14074 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/582.21b8e7d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5823.5045bdb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5851.30b7b2a.js
+-rw-r--r--   0 runner    (1001) docker     (123)   257877 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5878.32d92fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5880.68f975b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5955.88508f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/5971.88c5642.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6080.aa0ff24.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28010 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/61.2808a0d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18045 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6136.b8ba2b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6141.9831d58.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6475.6037fbb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6493.d796aa5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6556.b3d9293.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6571.2c8884e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6576.3ea568e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    83397 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6591.94ed352.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6612.1632879.js
+-rw-r--r--   0 runner    (1001) docker     (123)   246379 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6623.ae3b3cc.js
+-rw-r--r--   0 runner    (1001) docker     (123)      160 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6623.ae3b3cc.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16150 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6664.2160109.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6747.47be7f5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6748.be68f5f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6870.7940288.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11058 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6879.c8367a5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16507 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6898.9bbc12a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6952.f68b818.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6985.321ad92.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6993.32cf9a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/6997.b06fe71.js
+-rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7041.d4f561e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10338 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7058.805c88e.js
+-rw-r--r--   0 runner    (1001) docker     (123)       51 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7058.805c88e.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7174.6c45206.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35260 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7334.8859b1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7359.6ee65ec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7364.195178b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7380.58a4413.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7427.f9c2017.js
+-rw-r--r--   0 runner    (1001) docker     (123)      294 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7427.f9c2017.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14994 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7463.18fd278.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10358 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7509.1e0189e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7526.1a303e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31492 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7537.1323a15.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7692.33d5169.js
+-rw-r--r--   0 runner    (1001) docker     (123)      595 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7746.5908d29.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7808.1d582a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/783.c156751.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9192 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7858.2386e4d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31628 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/7941.01ea680.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8005.c5ad7b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8028.39e2fa1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9977 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8061.cc62561.js
+-rw-r--r--   0 runner    (1001) docker     (123)   317511 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8101.cf46d02.js
+-rw-r--r--   0 runner    (1001) docker     (123)       50 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8101.cf46d02.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/812.9b0e86e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      855 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/816.c8050f2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8165.b2c3285.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8232.a578bf9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/824.8678196.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15838 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8270.89fe7e1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/833.9cc6653.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8370.8f855e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8373.96b0b3a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8389.ffe031f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8412.1528057.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8427.4923f43.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8542.027afdc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8843 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8594.0112f03.js
+-rw-r--r--   0 runner    (1001) docker     (123)    30005 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8656.d5b8e92.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8685.d78bdab.js
+-rw-r--r--   0 runner    (1001) docker     (123)   114157 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8698.9817d75.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8732.9320f73.js
+-rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8741.b138cb8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8785.cf4fe95.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27799 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8828.77c71d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8883.80c7b63.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8976.3816942.js
+-rw-r--r--   0 runner    (1001) docker     (123)      432 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8981.99a4275.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/8990.2a453cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9035.1e45c1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9053.45b77fc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9077.fefb6ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9128.b8fa6f0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9225 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9156.0cefbd3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9170.0023587.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9196.315f9f9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28388 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9198.9971d70.js
+-rw-r--r--   0 runner    (1001) docker     (123)   131443 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/920.d15c177.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9253.0b31caa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9266.bacd0dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      591 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9307.c3a00ed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9321.869e413.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1188430 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9344.ba0abcf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9382.9014799.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29226 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9440.1b10b8f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      163 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9440.1b10b8f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9464.79e6ac5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9502.9a24831.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32420 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9507.1e6cc5d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9602.62bf0f1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9621.e2e8b5d.js
+-rw-r--r--   0 runner    (1001) docker     (123)      625 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9622.ccab065.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9626.a178bd0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10559 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9647.ed91993.js
+-rw-r--r--   0 runner    (1001) docker     (123)   432928 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9657.bc5c60e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9073 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/97.ad126b0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9712.796a0a1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9733.a3b2a7f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36791 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9737.7dc8f98.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9777.0b8a504.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9793.6d63a85.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17595 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9806.652c162.js
+-rw-r--r--   0 runner    (1001) docker     (123)   179318 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9865.2e3db6f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      246 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9865.2e3db6f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/989.bcca86a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14270 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9943.f3f35c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9958.25c8c06.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/9960.64cd61e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/add-above.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/add-below.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      227 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/add.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      942 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/bug-dot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      585 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/bug.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/build.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      301 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/caret-down-empty-thin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/caret-down-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/caret-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/caret-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      262 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/caret-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/caret-up-empty-thin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/caret-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/case-sensitive.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      260 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/check.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      316 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/circle-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      209 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/circle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      452 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/clear.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      562 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/console.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      391 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/copy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      623 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/copyright.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      602 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/cut.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      233 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/duplicate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      341 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/edit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/ellipses.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      484 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/extension.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76736 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13224 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78268 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      243 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/fast-forward.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      229 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/file-upload.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      461 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      238 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/filter-list.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/folder-favorite.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      285 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      891 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/html5.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      454 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/image.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      322 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/inspector.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/json.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/julia.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/jupyter-favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/jupyter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/jupyterlab-wordmark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      368 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/kernel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      434 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/keyboard.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.289378 resotocore-3.6.1/resotocore/jupyterlite/build/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)    54484 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/lab/bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)      411 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/launch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/launcher.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      200 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/line-form.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      403 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      371 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/list.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/listings-info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      428 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/markdown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/move-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      610 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/move-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/new-folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      899 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/not-trusted.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/notebook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      355 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/numbering.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      330 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/offline-bolt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/palette.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      404 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/paste.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/python.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      473 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/r-kernel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/react.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      388 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/redo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/refresh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      620 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/regex.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      217 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/run.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      364 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/running.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      346 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/save.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.289378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.137377 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.289378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json
+-rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)      763 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.289378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json
+-rw-r--r--   0 runner    (1001) docker     (123)      563 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      457 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/workspaces.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.289378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.293378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.293378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)      348 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.293378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/foreign.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.293378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.293378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/download.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.293378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.297378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json
+-rw-r--r--   0 runner    (1001) docker     (123)      513 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      477 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-with.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.297378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.297378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/about.json
+-rw-r--r--   0 runner    (1001) docker     (123)      456 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/jupyter-forum.json
+-rw-r--r--   0 runner    (1001) docker     (123)      466 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/launch-classic.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.301378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.301378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.301378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      655 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json
+-rw-r--r--   0 runner    (1001) docker     (123)      319 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.301378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.301378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.301378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.301378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.305378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24989 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.305378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/form-ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)      440 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.305378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.305378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.305378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.305378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      402 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)      572 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.305378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.137377 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@retrolab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.305378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/menus.json
+-rw-r--r--   0 runner    (1001) docker     (123)      443 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/top.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.309378 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/scroll-output.json
+-rw-r--r--   0 runner    (1001) docker     (123)    79291 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/schemas/all.json
+-rw-r--r--   0 runner    (1001) docker     (123)      439 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/search.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/service-worker-b2fb40a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      860 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/spreadsheet.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      259 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/stop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      297 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/table-rows.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/tag.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/terminal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      270 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/text-editor.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.137377 resotocore-3.6.1/resotocore/jupyterlite/build/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.137377 resotocore-3.6.1/resotocore/jupyterlite/build/themes/@jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.309378 resotocore-3.6.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)    16232 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.309378 resotocore-3.6.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)    15136 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)   310614 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)      538 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/toc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      300 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/tree-view.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      828 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/trusted.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      334 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      382 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/vega.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      426 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/build/yaml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/config-utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.141377 resotocore-3.6.1/resotocore/jupyterlite/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.309378 resotocore-3.6.1/resotocore/jupyterlite/doc/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/doc/workspaces/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.141377 resotocore-3.6.1/resotocore/jupyterlite/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.141377 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.309378 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2562 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.313378 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8738 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    27007 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      621 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4825 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8374 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    15897 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.313378 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/install.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2633 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.317378 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8195 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6063 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2532 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)   165727 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.317378 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4270 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6512 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6720 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8221 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     7915 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.321378 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1081 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2657 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14685 2023-07-14 17:01:26.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.321378 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2732 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.329378 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2643 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8368 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)  3578814 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1110 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)    70520 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      336 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2360 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14737 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     7706 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5802 2023-07-14 17:01:13.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.329378 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      199 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/install.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3508 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.329378 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      224 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/568.1e2faa2ba0bbe59c4780.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     7753 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3889 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      162 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2452 2023-07-14 17:01:21.000000 resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.333378 resotocore-3.6.1/resotocore/jupyterlite/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/jupyterlite/files/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20954 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/icon-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/jupyter-lite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-14 17:01:30.000000 resotocore-3.6.1/resotocore/jupyterlite/jupyter-lite.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11794 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/jupyterlite.schema.v0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.333378 resotocore-3.6.1/resotocore/jupyterlite/kernelspecs/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/kernelspecs/javascript.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.333378 resotocore-3.6.1/resotocore/jupyterlite/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)   324251 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/lab/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      993 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/lab/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/lab/jupyter-lite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      144 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/lab/jupyter-lite.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/lab/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.333378 resotocore-3.6.1/resotocore/jupyterlite/lab/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/lab/tree/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.333378 resotocore-3.6.1/resotocore/jupyterlite/lab/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/lab/workspaces/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      690 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/manifest.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/service-worker-b2fb40a.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.333378 resotocore-3.6.1/resotocore/jupyterlite/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 1985-10-26 08:15:00.000000 resotocore-3.6.1/resotocore/jupyterlite/tree/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.337378 resotocore-3.6.1/resotocore/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/model/adjust_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16479 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/model/db_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27281 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/model/graph_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/model/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58798 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/model/model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/model/resolve_in_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/model/transform_kind_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/model/typed_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.341378 resotocore-3.6.1/resotocore/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50309 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/query/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15393 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/query/query_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/query/template_expander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/query/template_expander_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.341378 resotocore-3.6.1/resotocore/report/
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/report/benchmark_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18010 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/report/inspector_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/report/report_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.341378 resotocore-3.6.1/resotocore/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   130266 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/api-doc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/ck-unicode-truecolor.ans
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.341378 resotocore-3.6.1/resotocore/static/report/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.141377 resotocore-3.6.1/resotocore/static/report/benchmark/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.345378 resotocore-3.6.1/resotocore/static/report/benchmark/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)    43058 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/benchmark/aws/aws_cis_1_5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/benchmark_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/check_template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.145377 resotocore-3.6.1/resotocore/static/report/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.345378 resotocore-3.6.1/resotocore/static/report/checks/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/checks/aws/aws_apigateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33970 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/checks/aws/aws_cloudtrail.json
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/checks/aws/aws_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46657 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/checks/aws/aws_ec2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/checks/aws/aws_efs.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24445 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/checks/aws/aws_iam.json
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/checks/aws/aws_kms.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/checks/aws/aws_lambda.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/checks/aws/aws_rds.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/report/checks/aws/aws_s3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/resoto.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/static/resoto_logo_and_text.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/system_start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.349378 resotocore-3.6.1/resotocore/task/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/task/job_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/task/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/task/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/task/start_workflow_on_first_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/task/subscribers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/task/task_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32516 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/task/task_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29621 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/task/task_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.349378 resotocore-3.6.1/resotocore/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/templates/create_first_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.349378 resotocore-3.6.1/resotocore/user/
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/user/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15532 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.353378 resotocore-3.6.1/resotocore/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65625 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/web/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/web/certificate_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/web/content_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/web/directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/web/tsdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-07-14 16:55:53.000000 resotocore-3.6.1/resotocore/worker_task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.153377 resotocore-3.6.1/resotocore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17709 2023-07-14 17:01:36.000000 resotocore-3.6.1/resotocore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34535 2023-07-14 17:01:36.000000 resotocore-3.6.1/resotocore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:01:36.000000 resotocore-3.6.1/resotocore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-14 17:01:36.000000 resotocore-3.6.1/resotocore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:01:35.000000 resotocore-3.6.1/resotocore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-14 17:01:36.000000 resotocore-3.6.1/resotocore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 17:01:36.000000 resotocore-3.6.1/resotocore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-14 17:01:36.377378 resotocore-3.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.353378 resotocore-3.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.357378 resotocore-3.6.1/tests/resotocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.357378 resotocore-3.6.1/tests/resotocore/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/analytics/posthog_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/analytics/recurrent_events_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.357378 resotocore-3.6.1/tests/resotocore/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/cli/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59406 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/cli/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/cli/model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.361378 resotocore-3.6.1/tests/resotocore/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12759 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/config/config_handler_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/config/config_override_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/config/core_config_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29325 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/console_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/core_config_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.365378 resotocore-3.6.1/tests/resotocore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/arango_query_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/arangodb_functions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/async_arangodb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/configdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/db_access_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/entitydb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31108 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/graphdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/jobdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/modeldb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/runningtaskdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/subscriberdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/system_data_db_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/db/templatedb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/dependencies_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.365378 resotocore-3.6.1/tests/resotocore/graph_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/graph_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/graph_manager/graph_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/hypothesis_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.369378 resotocore-3.6.1/tests/resotocore/infra_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/infra_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/infra_apps/local_runtime_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/infra_apps/package_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/message_bus_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.369378 resotocore-3.6.1/tests/resotocore/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/model/adjust_node_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/model/db_updater_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16522 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/model/graph_access_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/model/json_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/model/model_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24923 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/model/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/model/resolve_in_graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/model/typed_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.373378 resotocore-3.6.1/tests/resotocore/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15231 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/query/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/query/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/query/template_expander_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.373378 resotocore-3.6.1/tests/resotocore/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/report/benchnmark_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/report/inspector_service_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.373378 resotocore-3.6.1/tests/resotocore/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/task/job_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/task/start_workflow_on_first_subscriber_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/task/subscribers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10787 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/task/task_description_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/task/task_handler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.373378 resotocore-3.6.1/tests/resotocore/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/user/user_management_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/util_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/validator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:01:36.377378 resotocore-3.6.1/tests/resotocore/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/web/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21447 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/web/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/web/certificate_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/web/content_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-14 16:55:53.000000 resotocore-3.6.1/tests/resotocore/worker_task_queue_test.py
```

### Comparing `resotocore-3.6.0/LICENSE` & `resotocore-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/PKG-INFO` & `resotocore-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotocore
-Version: 3.6.0
+Version: 3.6.1
 Summary: Keeps all the things.
 Author: Some Engineering Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `resotocore-3.6.0/README.md` & `resotocore-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/pyproject.toml` & `resotocore-3.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resotocore"
-version = "3.6.0"
+version = "3.6.1"
 authors = [{name="Some Engineering Inc."}]
 description = "Keeps all the things."
 license = {file="LICENSE"}
 urls = {"Homepage" = "https://resoto.com"}
 requires-python = ">=3.9"
 classifiers = [ "Programming Language :: Python :: 3" ]
 readme = {file="README.md", content-type="text/markdown"}
```

### Comparing `resotocore-3.6.0/resotocore/__main__.py` & `resotocore-3.6.1/resotocore/config/config_handler_service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,315 +1,287 @@
 import asyncio
-import logging
-import platform
-import sys
-import traceback
-import warnings
-from argparse import Namespace
-from asyncio import Queue
-from contextlib import suppress
+
 from datetime import timedelta
-from functools import partial
-from pathlib import Path
-from tempfile import TemporaryDirectory
-from typing import AsyncIterator, List, Union
-
-from aiohttp.web_app import Application
-from arango.database import StandardDatabase
-from attrs import evolve
-from urllib3.exceptions import HTTPWarning
-
-from resotocore import version
-from resotocore.action_handlers.merge_outer_edge_handler import MergeOuterEdgesHandler
-from resotocore.analytics import CoreEvent, NoEventSender
-from resotocore.analytics.posthog import PostHogEventSender
-from resotocore.analytics.recurrent_events import emit_recurrent_events
-from resotocore.cli.cli import CLIService
-from resotocore.cli.command import alias_names, all_commands
-from resotocore.cli.dependencies import CLIDependencies
-from resotocore.config.config_handler_service import ConfigHandlerService
-from resotocore.config.config_override_service import ConfigOverrideService, model_from_db, override_config_for_startup
-from resotocore.config.core_config_handler import CoreConfigHandler
-from resotocore.core_config import (
-    config_from_db,
-    CoreConfig,
-    RunConfig,
-    inside_docker,
-    inside_kubernetes,
-    helm_installation,
-    ResotoCoreConfigId,
-)
-from resotocore.db import SystemData
-from resotocore.db.db_access import DbAccess
-from resotocore.dependencies import db_access, setup_process, parse_args, system_info, reconfigure_logging
-from resotocore.error import RestartService
-from resotocore.message_bus import MessageBus
-from resotocore.model.model_handler import ModelHandlerDB
-from resotocore.model.typed_model import to_json, class_fqn
-from resotocore.query.template_expander_service import TemplateExpanderService
-from resotocore.report.inspector_service import InspectorService
-from resotocore.task.scheduler import Scheduler
-from resotocore.task.subscribers import SubscriptionHandler
-from resotocore.task.task_handler import TaskHandlerService
-from resotocore.user.user_management import UserManagementService
-from resotocore.util import shutdown_process, utc
-from resotocore.web.api import Api
-from resotocore.web.certificate_handler import CertificateHandler
-from resotocore.worker_task_queue import WorkerTaskQueue
-from resotocore.infra_apps.local_runtime import LocalResotocoreAppRuntime
-from resotocore.infra_apps.package_manager import PackageManager
-from resotocore.graph_manager.graph_manager import GraphManager
-from resotolib.asynchronous.web import runner
-
-log = logging.getLogger("resotocore")
-
-
-def main() -> None:
-    """
-    Application entrypoint - no arguments are allowed.
-    """
-    try:
-        run(sys.argv[1:])
-        log.info("Process finished.")
-    except (KeyboardInterrupt, SystemExit):
-        log.info("Stopping resoto graph core.")
-        shutdown_process(0)
-    except Exception as ex:
-        if "--debug" in sys.argv:
-            print(traceback.format_exc())
-        print(f"resotocore stopped. Reason {class_fqn(ex)}: {ex}", file=sys.stderr)
-        shutdown_process(1)
-
-
-def run(arguments: List[str]) -> None:
-    """
-    Run application. When this method returns, the process is done.
-    :param arguments: the arguments provided to this process.
-                 Note: this method is used in tests to specify arbitrary arguments.
-    """
-    args = parse_args(arguments)
-    setup_process(args)
-
-    # after setup, logging is possible
-    info = system_info()
-    log.info(
-        f"Starting up version={info.version} on system with cpus={info.cpus}, "
-        f"available_mem={info.mem_available}, total_mem={info.mem_total}"
-    )
-
-    # The loop is here to restart the process in case of RestartService exceptions.
-    while True:
-        try:
-            run_process(args)
-            break  # This line should never be reached. In case it does, break the loop.
-        except RestartService as ex:
-            message = f"Restarting Service. Reason: {ex.reason}"
-            line = "-" * len(message)
-            print(f"\n{line}\n{message}\n{line}\n")
-
-
-def run_process(args: Namespace) -> None:
-    with TemporaryDirectory() as temp_name:
-        temp = Path(temp_name)
-        with warnings.catch_warnings():  # ignore ssl errors during setup
-            warnings.simplefilter("ignore", HTTPWarning)
-            # wait here for an initial connection to the database before we continue. blocking!
-            created, system_data, sdb = DbAccess.connect(args, timedelta(seconds=120), verify=False)
-            # only to be used for CoreConfig creation
-            core_config_override_service = asyncio.run(override_config_for_startup(args.config_override_path))
-            config = config_from_db(args, sdb, lambda: core_config_override_service.get_override(ResotoCoreConfigId))
-            cert_handler = CertificateHandler.lookup(config, sdb, temp)
-            verify: Union[bool, str] = False if args.graphdb_no_ssl_verify else str(cert_handler.ca_bundle)
-            config = evolve(config, run=RunConfig(temp, verify))
-        # in case of tls: connect again with the correct certificate settings
-        use_tls = args.graphdb_server.startswith("https://")
-        db_client = DbAccess.connect(args, timedelta(seconds=30), verify=verify)[2] if use_tls else sdb
-        with_config(created, system_data, db_client, cert_handler, config, args.config_override_path)
-
-
-def with_config(
-    created: bool,
-    system_data: SystemData,
-    sdb: StandardDatabase,
-    cert_handler: CertificateHandler,
-    config: CoreConfig,
-    config_overrides_paths: List[Path],
-) -> None:
-    reconfigure_logging(config)  # based on the config, logging might have changed
-    # only lg the editable config - to not log any passwords
-    log.debug(f"Starting with config: {config.editable}")
-    info = system_info()
-    event_sender = PostHogEventSender(system_data) if config.runtime.usage_metrics else NoEventSender()
-    db = db_access(config, sdb, event_sender)
-    message_bus = MessageBus()
-    scheduler = Scheduler()
-    worker_task_queue = WorkerTaskQueue()
-    model = ModelHandlerDB(db, config.runtime.plantuml_server)
-    # a "real" config override service, unlike the one used for core config
-    config_override_service = ConfigOverrideService(config_overrides_paths, partial(model_from_db, db.configs_model_db))
-    config_handler = ConfigHandlerService(
-        db.config_entity_db,
-        db.config_validation_entity_db,
-        db.configs_model_db,
-        worker_task_queue,
-        message_bus,
-        event_sender,
-        config,
-        config_override_service,
-    )
-    user_management = UserManagementService(db, config_handler, event_sender)
-    cli_deps = CLIDependencies(
-        message_bus=message_bus,
-        event_sender=event_sender,
-        db_access=db,
-        model_handler=model,
-        worker_task_queue=worker_task_queue,
-        config=config,
-        config_handler=config_handler,
-        cert_handler=cert_handler,
-        user_management=user_management,
-    )
-    default_env = {"graph": config.cli.default_graph, "section": config.cli.default_section}
-    cli = CLIService(cli_deps, all_commands(cli_deps), default_env, alias_names())
-    template_expander = TemplateExpanderService(db.template_entity_db, cli)
-    cli_deps.extend(template_expander=template_expander)
-    inspector = InspectorService(cli)
-    subscriptions = SubscriptionHandler(db.subscribers_db, message_bus)
-    task_handler = TaskHandlerService(
-        db.running_task_db, db.job_db, message_bus, event_sender, subscriptions, scheduler, cli, config
-    )
-    core_config_handler = CoreConfigHandler(
-        config, message_bus, worker_task_queue, config_handler, event_sender, inspector
-    )
-    merge_outer_edges_handler = MergeOuterEdgesHandler(message_bus, subscriptions, task_handler, db, model)
-    cli_deps.extend(task_handler=task_handler, inspector=inspector)
-    infra_apps_runtime = LocalResotocoreAppRuntime(cli)
-    cli_deps.extend(infra_apps_runtime=infra_apps_runtime)
-    infra_apps_package_manager = PackageManager(
-        db.package_entity_db, config_handler, cli.register_infra_app_alias, cli.unregister_infra_app_alias
-    )
-    cli_deps.extend(infra_apps_package_manager=infra_apps_package_manager)
-    graph_manager = GraphManager(db, config.snapshots, core_config_handler, task_handler)
-    cli_deps.extend(graph_manager=graph_manager)
-    api = Api(
-        db,
-        model,
-        subscriptions,
-        task_handler,
-        message_bus,
-        event_sender,
-        worker_task_queue,
-        cert_handler,
-        config_handler,
-        inspector,
-        cli,
-        template_expander,
-        config,
-        user_management,
-        config_override_service.get_override,
-        graph_manager,
-    )
-    event_emitter = emit_recurrent_events(
-        event_sender, model, subscriptions, worker_task_queue, message_bus, timedelta(hours=1), timedelta(hours=1)
-    )
-
-    async def on_start() -> None:
-        # queue must be created inside an async function!
-        cli_deps.extend(forked_tasks=Queue())
-        await db.start()
-        await event_sender.start()
-        await subscriptions.start()
-        await scheduler.start()
-        await worker_task_queue.start()
-        await event_emitter.start()
-        await cli.start()
-        await inspector.start()
-        await task_handler.start()
-        await config_override_service.start()
-        await config_handler.start()
-        await core_config_handler.start()
-        await merge_outer_edges_handler.start()
-        await cert_handler.start()
-        await api.start()
-        await infra_apps_package_manager.start()
-        await graph_manager.start()
-        if created:
-            docker = inside_docker()
-            kubernetes = inside_kubernetes()
-            helm = helm_installation()
-            await event_sender.core_event(
-                CoreEvent.SystemInstalled,
-                {
-                    "docker_install": docker,
-                    "k8s_install": kubernetes,
-                    "helm_install": helm,
-                    "pip_install": not (docker or kubernetes or helm),
-                },
-            )
-        await event_sender.core_event(
-            CoreEvent.SystemStarted,
-            {
-                "version": version(),
-                "created_at": to_json(system_data.created_at),
-                "system": platform.system(),
-                "platform": platform.platform(),
-                "inside_docker": info.inside_docker,
-            },
-            cpu_count=info.cpus,
-            mem_total=info.mem_total,
-            mem_available=info.mem_available,
+from typing import Optional, AsyncIterator, List, Dict, Any, cast
+import attrs
+import yaml
+import os
+from deepdiff import DeepDiff
+import hashlib
+
+from resotocore.analytics import AnalyticsEventSender, CoreEvent
+from resotocore.config import ConfigHandler, ConfigEntity, ConfigValidation, ConfigOverride
+from resotocore.db.configdb import ConfigEntityDb, ConfigValidationEntityDb
+from resotocore.db.modeldb import ModelDb
+from resotocore.message_bus import MessageBus, CoreMessage
+from resotocore.model.model import Model, Kind, ComplexKind
+from resotocore.service import Service
+from resotocore.types import Json, JsonElement
+from resotocore.util import uuid_str, deep_merge, first
+from resotocore.worker_task_queue import WorkerTaskQueue, WorkerTask, WorkerTaskName
+from resotocore.ids import TaskId, ConfigId
+from resotocore.core_config import CoreConfig
+from resotolib.utils import merge_json_elements
+
+from resotolib.utils import replace_env_vars
+
+
+class ConfigHandlerService(ConfigHandler, Service):
+    def __init__(
+        self,
+        cfg_db: ConfigEntityDb,
+        validation_db: ConfigValidationEntityDb,
+        model_db: ModelDb,
+        task_queue: WorkerTaskQueue,
+        message_bus: MessageBus,
+        event_sender: AnalyticsEventSender,
+        core_config: CoreConfig,
+        override_service: ConfigOverride,
+    ) -> None:
+        self.cfg_db = cfg_db
+        self.validation_db = validation_db
+        self.model_db = model_db
+        self.task_queue = task_queue
+        self.message_bus = message_bus
+        self.event_sender = event_sender
+        self.core_config = core_config
+        self.override_service = override_service
+        self.old_overrides: Dict[ConfigId, Json] = {}
+
+    async def coerce_and_check_model(self, cfg_id: ConfigId, config: Json, validate: bool = True) -> Json:
+        model = await self.get_configs_model()
+        # filter config roots to match top level entries in config
+        config_roots = {kind.fqn: kind for kind in model.complex_kinds() if kind.aggregate_root}
+
+        final_config = {}
+        if validate:
+            for key, value in config.items():
+                if key in config_roots:
+                    try:
+                        value_kind = config_roots[key]
+                        coerced = value_kind.check_valid(value, normalize=False, config_context=True)
+                        final_config[key] = value_kind.sort_json(coerced or value)
+                    except Exception as ex:
+                        raise AttributeError(f"Error validating section {key}: {ex}") from ex
+                else:
+                    final_config[key] = value
+        else:
+            final_config = config
+
+        # If an external entity needs to approve this change.
+        # Method throws if config is not valid according to external approval.
+        keys = {key async for key in self.validation_db.keys()}
+        parts = cfg_id.split(".")
+        # A config with key foo.bla.bar can be validated by foo.bla.bar, foo.bla and foo
+        # The longest key is the most specific validator and is used.
+        validator = first(lambda x: x in keys, (".".join(parts[0:i]) for i in range(len(parts), 0, -1)))
+        if validator:
+            validation = await self.validation_db.get(validator)
+            if validation and validation.external_validation and validate:
+                await self.acknowledge_config_change(validator, final_config)
+
+        # If we come here, everything is fine
+        return final_config
+
+    async def coerce_config(self, config: Json) -> Json:
+        model = await self.get_configs_model()
+
+        final_config = {}
+        for key, value in config.items():
+            if key in model:
+                value_kind = model[key]
+                coerced = value_kind.coerce(value)
+                sorted_conf = value_kind.sort_json(coerced) if isinstance(coerced, dict) else coerced
+                final_config[key] = sorted_conf
+            else:
+                final_config[key] = value
+        return final_config
+
+    def list_config_ids(self) -> AsyncIterator[ConfigId]:
+        return self.cfg_db.keys()
+
+    async def get_config(
+        self, cfg_id: ConfigId, apply_overrides: bool = True, resolve_env_vars: bool = True
+    ) -> Optional[ConfigEntity]:
+        conf = await self.cfg_db.get(cfg_id)
+        if conf is None:
+            return None
+
+        # apply overrides if they exist and we do not opt out
+        # we do not want to apply overrides if the config is to be shown during editing
+        overrides = self.override_service.get_override(cfg_id)
+        updated_conf = cast(
+            Json, merge_json_elements(conf.config, overrides) if overrides and apply_overrides else conf.config
+        )
+
+        # reslove env vars
+        # we do not want to resolve env vars if the config is to be shown to the user when editing,
+        # otherwise sensitive data might be exposed
+        if resolve_env_vars:
+            resolved_conf = {k: replace_env_vars(v, os.environ) for k, v in updated_conf.items()}
+            coerced_conf = await self.coerce_config(resolved_conf)
+            updated_conf = coerced_conf
+
+        return attrs.evolve(conf, config=updated_conf)
+
+    async def put_config(self, cfg: ConfigEntity, *, validate: bool = True, dry_run: bool = False) -> ConfigEntity:
+        coerced = await self.coerce_and_check_model(cfg.id, cfg.config, validate)
+        existing = await self.cfg_db.get(cfg.id)
+        if not dry_run and (not existing or existing.config != cfg.config):
+            result = await self.cfg_db.update(ConfigEntity(cfg.id, coerced, cfg.revision))
+            await self.message_bus.emit_event(CoreMessage.ConfigUpdated, dict(id=result.id, revision=result.revision))
+            await self.event_sender.core_event(CoreEvent.SystemConfigurationChanged, result.analytics())
+            return result
+        else:
+            return cfg
+
+    async def patch_config(self, cfg: ConfigEntity, *, validate: bool = True, dry_run: bool = False) -> ConfigEntity:
+        current = await self.cfg_db.get(cfg.id)
+        current_config = current.config if current else {}
+        coerced = await self.coerce_and_check_model(cfg.id, deep_merge(current_config, cfg.config), validate)
+        if not dry_run and (not current or current_config != coerced):
+            result = await self.cfg_db.update(ConfigEntity(cfg.id, coerced, current.revision if current else None))
+            await self.message_bus.emit_event(CoreMessage.ConfigUpdated, dict(id=result.id, revision=result.revision))
+            await self.event_sender.core_event(CoreEvent.SystemConfigurationChanged, result.analytics())
+            return result
+        else:
+            return cfg
+
+    async def delete_config(self, cfg_id: ConfigId) -> None:
+        await self.cfg_db.delete(cfg_id)
+        await self.validation_db.delete(cfg_id)
+        await self.message_bus.emit_event(CoreMessage.ConfigDeleted, dict(id=cfg_id))
+        await self.event_sender.core_event(CoreEvent.SystemConfigurationDeleted)
+
+    async def copy_config(self, from_cfg_id: ConfigId, to_cfg_id: ConfigId) -> Optional[ConfigEntity]:
+        old = await self.cfg_db.get(from_cfg_id)
+        if old is None:
+            return None
+        if await self.cfg_db.get(to_cfg_id) is not None:
+            raise ValueError(f"Config with id {to_cfg_id} already exists")
+        result = await self.cfg_db.update(ConfigEntity(to_cfg_id, old.config, old.revision))
+        await self.message_bus.emit_event(
+            CoreMessage.ConfigUpdated, dict(old=old.id, new=result.id, revision=result.revision)
         )
+        await self.event_sender.core_event(CoreEvent.SystemConfigurationChanged, result.analytics())
+        return result
 
-    async def on_stop() -> None:
-        duration = utc() - info.started_at
-        await graph_manager.stop()
-        await infra_apps_package_manager.stop()
-        await api.stop()
-        await cert_handler.stop()
-        await config_override_service.stop()
-        await core_config_handler.stop()
-        await merge_outer_edges_handler.stop()
-        await task_handler.stop()
-        await inspector.stop()
-        await cli.stop()
-        await event_sender.core_event(CoreEvent.SystemStopped, total_seconds=int(duration.total_seconds()))
-        await event_emitter.stop()
-        await worker_task_queue.stop()
-        await scheduler.stop()
-        await subscriptions.stop()
-        await db.stop()
-        await event_sender.stop()
-
-    async def async_initializer() -> Application:
-        async def clean_all_tasks() -> None:
-            log.info("Clean up all running tasks.")
-            for task in asyncio.all_tasks():
-                with suppress(asyncio.CancelledError):
-                    if not task.done() or not task.cancelled():
-                        task.cancel()
-                    log.debug(f"Wait for task: {task}")
-                    await task
-
-        async def on_start_stop(_: Application) -> AsyncIterator[None]:
-            await on_start()
-            log.info("Initialization done. Starting API.")
-            yield
-            log.info("Shutdown initiated. Stop all tasks.")
-            await on_stop()
-            await clean_all_tasks()
-
-        api.app.cleanup_ctx.append(on_start_stop)
-        return api.app
-
-    runner.run_app(
-        async_initializer(),
-        api.stop,
-        host=config.api.web_hosts,
-        https_port=config.api.https_port,
-        http_port=config.api.http_port,
-        default_port=8900,
-        ssl_context=cert_handler.host_context,
-    )
+    def list_config_validation_ids(self) -> AsyncIterator[str]:
+        return self.validation_db.keys()
+
+    async def get_config_validation(self, cfg_id: str) -> Optional[ConfigValidation]:
+        return await self.validation_db.get(cfg_id)
+
+    async def put_config_validation(self, validation: ConfigValidation) -> ConfigValidation:
+        return await self.validation_db.update(validation)
+
+    async def get_configs_model(self) -> Model:
+        kinds = [kind async for kind in self.model_db.all()]
+        return Model.from_kinds(list(kinds))
+
+    async def update_configs_model(self, kinds: List[Kind]) -> Model:
+        # load existing model
+        model = await self.get_configs_model()
+        # make sure the update is valid, but ignore overlapping property paths, so the same name can
+        # have different types in different sections
+        updated = model.update_kinds(kinds, check_overlap=False)
+        # store all updated kinds
+        await self.model_db.update_many(kinds)
+        return updated
+
+    async def config_yaml(self, cfg_id: ConfigId, revision: bool = False) -> Optional[str]:
+        config = await self.get_config(cfg_id, apply_overrides=False, resolve_env_vars=False)
+        if config:
+            model = await self.get_configs_model()
+
+            # returns the overridden config with comments about the changes
+            def overridden_parts(existing: JsonElement, update: JsonElement) -> JsonElement:
+                if isinstance(update, dict):
+                    return {
+                        key: overridden_parts(
+                            existing.get(key) if isinstance(existing, dict) else existing, update[key]
+                        )
+                        for key in set(update.keys())
+                    }
+                else:
+
+                    def mkstr(val: Any) -> str:
+                        if isinstance(val, list):
+                            return f'[{", ".join(val)}]'
+                        return str(val)
+
+                    return mkstr(update)
+
+            yaml_str = ""
+
+            overrides = overridden_parts(config.config, self.override_service.get_override(cfg_id) or {})
+            overrides_json = overrides if isinstance(overrides, dict) else {}
+
+            for num, (key, value) in enumerate(config.config.items()):
+                maybe_kind = model.get(key)
+                if isinstance(maybe_kind, ComplexKind):
+                    part = maybe_kind.create_yaml(value, initial_level=1, overrides=overrides_json.get(key) or {})
+                    if num > 0:
+                        yaml_str += "\n"
+                    yaml_str += key + ":" + part
+                else:
+                    yaml_str += yaml.dump({key: value}, sort_keys=False, allow_unicode=True)
+
+            # mix the revision into the yaml document
+            if revision and config.revision:
+                yaml_str += (
+                    "\n\n# This property is not part of the configuration but defines the revision "
+                    "of this document.\n# Please leave it here to avoid conflicting writes.\n"
+                    f'_revision: "{config.revision}"'
+                )
+
+            return yaml_str
+        else:
+            return None
+
+    async def acknowledge_config_change(self, cfg_id: str, config: Json) -> None:
+        """
+        In case an external entity should acknowledge this config change.
+        This method either return, which signals success or throws an exception.
+        """
+        future = asyncio.get_event_loop().create_future()
+        task = WorkerTask(
+            TaskId(uuid_str()),
+            WorkerTaskName.validate_config,
+            {"config_id": cfg_id},
+            {"task": WorkerTaskName.validate_config, "config": config},
+            future,
+            timedelta(seconds=30),
+        )
+        # add task to queue - do not retry
+        await self.task_queue.add_task(task)
+        # In case the config is not valid or no worker is available
+        # this future will throw an exception.
+        # Do not handle it here and let the error bubble up.
+        await future
+
+    async def start(self) -> None:
+        async def on_override_change(new_overrides: Dict[ConfigId, Json]) -> None:
+            def updated_revision(conf: Json, override: Json) -> str:
+                m = hashlib.sha1(usedforsecurity=False)
+                m.update(yaml.dump(conf).encode("utf-8"))
+                m.update(yaml.dump(override).encode("utf-8"))
+                return m.hexdigest()
+
+            diff = DeepDiff(self.old_overrides, new_overrides, ignore_order=True)
+            if diff.affected_root_keys:
+                affected_configs = diff.affected_root_keys
+
+                for config_id in affected_configs:
+                    # the new and updated version, since the override is already applied
+                    config = await self.get_config(config_id)
+                    if config:
+                        new_revision = updated_revision(config.config, new_overrides.get(config_id) or {})
+                        await self.message_bus.emit_event(
+                            CoreMessage.ConfigUpdated, dict(id=config.id, revision=new_revision)
+                        )
+                        await self.event_sender.core_event(CoreEvent.SystemConfigurationChanged, config.analytics())
 
+                self.old_overrides = new_overrides
 
-if __name__ == "__main__":
-    main()
+        self.old_overrides = self.override_service.get_all_overrides()
+        self.override_service.add_override_change_hook(on_override_change)
```

### Comparing `resotocore-3.6.0/resotocore/action_handlers/merge_outer_edge_handler.py` & `resotocore-3.6.1/resotocore/action_handlers/merge_outer_edge_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 import asyncio
 from asyncio import Task, Future
 from typing import Optional, Tuple, List
 from contextlib import suppress
 from datetime import timedelta
 from resotocore.model.graph_access import ByNodeId, NodeSelector
+from resotocore.service import Service
 from resotocore.task.model import Subscriber
 from resotocore.ids import NodeId, SubscriberId
 from resotocore.task.task_handler import TaskHandlerService
 from resotocore.ids import TaskId
 from resotocore.task.subscribers import SubscriptionHandler
 from resotocore.db.db_access import DbAccess
 from resotocore.model.model_handler import ModelHandler
@@ -19,15 +20,15 @@
 
 log = logging.getLogger(__name__)
 
 subscriber_id = SubscriberId("resotocore")
 merge_outer_edges = "merge_outer_edges"
 
 
-class MergeOuterEdgesHandler:
+class MergeOuterEdgesHandler(Service):
     def __init__(
         self,
         message_bus: MessageBus,
         subscription_handler: SubscriptionHandler,
         task_handler_service: TaskHandlerService,
         db_access: DbAccess,
         model_handler: ModelHandler,
```

### Comparing `resotocore-3.6.0/resotocore/analytics/__init__.py` & `resotocore-3.6.1/resotocore/analytics/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 from abc import ABC, abstractmethod
 from attrs import define
 from datetime import datetime
 from typing import Optional, Mapping, List, Union
 
+from resotocore.service import Service
 from resotocore.types import JsonElement
 from resotocore.util import utc
 
 log = logging.getLogger(__name__)
 
 
 class CoreEvent:
@@ -51,15 +52,15 @@
     system: str  # e.g. creator of the event: resotocore, resotoui, resotosh, etc.
     kind: str  # kind of the event. Every kind has a specific set of data and context vars
     context: Mapping[str, JsonElement]  # context properties
     counters: Mapping[str, Union[int, float]]  # all counters of this event
     at: datetime  # time, when this event has been created
 
 
-class AnalyticsEventSender(ABC):
+class AnalyticsEventSender(Service, ABC):
     async def core_event(
         self, kind: str, context: Optional[Mapping[str, JsonElement]] = None, **counters: Union[int, float]
     ) -> AnalyticsEvent:
         event = AnalyticsEvent("resotocore", kind, context if context else {}, counters, utc())
         await self.capture([event])
         return event
```

### Comparing `resotocore-3.6.0/resotocore/analytics/posthog.py` & `resotocore-3.6.1/resotocore/analytics/posthog.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/analytics/recurrent_events.py` & `resotocore-3.6.1/resotocore/analytics/recurrent_events.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/async_extensions.py` & `resotocore-3.6.1/resotocore/async_extensions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/cli/__init__.py` & `resotocore-3.6.1/resotocore/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/cli/cli.py` & `resotocore-3.6.1/resotocore/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     WelcomeCommand,
     SortPart,
     LimitPart,
     HistoryPart,
     ReportCommand,
     WriteCommand,
 )
-from resotocore.cli.dependencies import CLIDependencies
+from resotocore.dependencies import Dependencies
 from resotocore.cli.model import (
     ParsedCommand,
     ParsedCommands,
     ExecutableCommand,
     ParsedCommandLine,
     CLICommand,
     InternalPart,
@@ -72,14 +72,15 @@
     AggregateVariableName,
     AggregateFunction,
     PathRoot,
     Limit,
     Sort,
 )
 from resotocore.query.query_parser import aggregate_parameter_parser, sort_args_p, limit_parser_direct
+from resotocore.service import Service
 from resotocore.types import JsonElement
 from resotocore.util import group_by
 from resotolib.parse_util import make_parser, pipe_p, semicolon_p
 
 log = logging.getLogger(__name__)
 
 
@@ -113,15 +114,15 @@
         command [optional]: if given shows the help for a specific command
 
     Show help text for a command or general help information.
     """
 
     def __init__(
         self,
-        dependencies: CLIDependencies,
+        dependencies: Dependencies,
         parts: List[CLICommand],
         alias_names: Dict[str, str],
         alias_templates: Dict[str, AliasTemplate],
         infra_app_aliases: Dict[str, InfraAppAlias],
     ):
         super().__init__(dependencies, "misc", True)
         self.all_parts = {p.name: p for p in parts + [self]}
@@ -214,22 +215,22 @@
 CLIArg = Tuple[CLICommand, Optional[str]]
 # If no sort is defined in the part, we use this default sort order
 DefaultSort = [Sort("/reported.kind"), Sort("/reported.name"), Sort("/reported.id")]
 # Default sort order for history searches
 HistorySort = [Sort("/changed_at"), Sort("/reported.kind"), Sort("/reported.name"), Sort("/reported.id")]
 
 
-class CLIService(CLI):
+class CLIService(CLI, Service):
     """
     The CLI has a defined set of dependencies and knows a list if commands.
     A string can be parsed into a command line that can be executed based on the list of available commands.
     """
 
     def __init__(
-        self, dependencies: CLIDependencies, parts: List[CLICommand], env: Dict[str, Any], alias_names: Dict[str, str]
+        self, dependencies: Dependencies, parts: List[CLICommand], env: Dict[str, Any], alias_names: Dict[str, str]
     ):
         dependencies.extend(cli=self)
         alias_templates_list = [AliasTemplate.from_config(cmd) for cmd in dependencies.config.custom_commands.commands]
         alias_templates = {a.name: a for a in alias_templates_list}
         infra_app_aliases: Dict[str, InfraAppAlias] = {}
         help_cmd = HelpCommand(
             dependencies,
@@ -263,15 +264,15 @@
         return self.__commands
 
     @property
     def env(self) -> Dict[str, Any]:
         return self.cli_env
 
     @property
-    def dependencies(self) -> CLIDependencies:
+    def dependencies(self) -> Dependencies:
         return self.__dependencies
 
     @property
     def alias_templates(self) -> Dict[str, AliasTemplate]:
         return self.__alias_templates
 
     @property
```

### Comparing `resotocore-3.6.0/resotocore/cli/command.py` & `resotocore-3.6.1/resotocore/cli/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     js_value_at,
     js_value_get,
     key_values_parser,
     parse_time_or_delta,
     strip_quotes,
     key_value_parser,
 )
-from resotocore.cli.dependencies import CLIDependencies
+from resotocore.dependencies import Dependencies
 from resotocore.cli.model import (
     CLICommand,
     CLIContext,
     EmptyContext,
     CLIAction,
     CLISource,
     CLIFlow,
@@ -98,15 +98,15 @@
 )
 from resotocore.cli.tip_of_the_day import SuggestionPolicy, SuggestionStrategy, get_suggestion_strategy
 from resotocore.config import ConfigEntity
 from resotocore.db.async_arangodb import AsyncCursor
 from resotocore.db.graphdb import HistoryChange, GraphDB
 from resotocore.db.model import QueryModel
 from resotocore.db.runningtaskdb import RunningTaskData
-from resotocore.dependencies import system_info
+from resotocore.system_start import system_info
 from resotocore.error import CLIParseError, ClientError, CLIExecutionError
 from resotocore.ids import ConfigId, TaskId, InfraAppName, TaskDescriptorId, GraphName, Email, Password
 from resotocore.infra_apps.manifest import AppManifest
 from resotocore.infra_apps.package_manager import Failure
 from resotocore.model.graph_access import Section, EdgeTypes
 from resotocore.model.model import (
     Model,
@@ -178,18 +178,14 @@
 )
 from resotolib.utils import safe_members_in_tarfile, get_local_tzinfo
 from resotolib.x509 import write_cert_to_file, write_key_to_file
 
 log = logging.getLogger(__name__)
 
 
-def deps(command: CLICommand) -> CLIDependencies:
-    return cast(CLIDependencies, command.dependencies)
-
-
 # A SearchCLIPart is a command that can be used on the command line.
 # Such a part is not executed, but builds a search, which is executed.
 # Therefore, the parse method is implemented in a dummy fashion here.
 # The real interpretation happens in CLI.create_query.
 class SearchCLIPart(CLICommand, EntityProvider, ABC):
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
         return CLISource.empty()
@@ -1420,20 +1416,18 @@
         history: bool = parsed.get("history", False)
         at: Optional[datetime] = parse_at(parsed.get("at", None))
 
         # all templates are expanded at this point, so we can call the parser directly.
         query = parse_query(rest, **ctx.env)
 
         async def get_db(at: Optional[datetime], graph_name: GraphName) -> Tuple[GraphDB, GraphName]:
-            db_access = cast(CLIDependencies, self.dependencies).db_access
+            db_access = self.dependencies.db_access
             if at:
                 # if we search at some specific time: find a snapshot at that time
-                snapshot_name = await cast(CLIDependencies, self.dependencies).graph_manager.snapshot_at(
-                    time=at, graph_name=graph_name
-                )
+                snapshot_name = await self.dependencies.graph_manager.snapshot_at(time=at, graph_name=graph_name)
                 if not snapshot_name:
                     raise CLIParseError(f"No graph snapshot at {at} found for graph {graph_name}.")
 
                 return db_access.get_graph_db(snapshot_name), snapshot_name
 
             return db_access.get_graph_db(graph_name), graph_name
 
@@ -1954,15 +1948,15 @@
         func = partial(self.set_desired, arg, ctx.graph_name, self.patch(arg, ctx))
         return CLIFlow(lambda in_stream: stream.flatmap(stream.chunks(in_stream, buffer_size), func))
 
     async def set_desired(
         self, arg: Optional[str], graph_name: GraphName, patch: Json, items: List[Json]
     ) -> AsyncIterator[JsonElement]:
         model = await self.dependencies.model_handler.load_model(graph_name)
-        db = cast(CLIDependencies, self.dependencies).db_access.get_graph_db(graph_name)
+        db = self.dependencies.db_access.get_graph_db(graph_name)
         node_ids = []
         for item in items:
             if "id" in item:
                 node_ids.append(item["id"])
             elif isinstance(item, str):
                 node_ids.append(item)
         async for update in db.update_nodes_desired(model, patch, node_ids):
@@ -2088,15 +2082,15 @@
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIFlow:
         buffer_size = 1000
         func = partial(self.set_metadata, ctx.graph_name, self.patch(arg, ctx))
         return CLIFlow(lambda in_stream: stream.flatmap(stream.chunks(in_stream, buffer_size), func))
 
     async def set_metadata(self, graph_name: GraphName, patch: Json, items: List[Json]) -> AsyncIterator[JsonElement]:
         model = await self.dependencies.model_handler.load_model(graph_name)
-        db = cast(CLIDependencies, self.dependencies).db_access.get_graph_db(graph_name)
+        db = self.dependencies.db_access.get_graph_db(graph_name)
         node_ids = []
         for item in items:
             if "id" in item:
                 node_ids.append(item["id"])
             elif isinstance(item, str):
                 node_ids.append(item)
         async for update in db.update_nodes_metadata(model, patch, node_ids):
@@ -3066,15 +3060,15 @@
 
     def update_node_in_graphdb(self, model: Model, **env: str) -> Callable[[WorkerTask, Future[Json]], Awaitable[Json]]:
         async def to_result(task: WorkerTask, future_result: Future[Json]) -> Json:
             nid = js_value_at(task.data, ["node", "id"])
             try:
                 result = await future_result
                 if is_node(result):
-                    db = cast(CLIDependencies, self.dependencies).db_access.get_graph_db(GraphName(env["graph"]))
+                    db = self.dependencies.db_access.get_graph_db(GraphName(env["graph"]))
                     try:
                         updated: Json = await db.update_node(model, result["id"], result, True, None)
                         return updated
                     except ClientError as ex:
                         # if the change could not be reflected in database, show success
                         log.warning(
                             f"Update not reflected in db. Wait until next collector run. Reason: {str(ex)}",
@@ -3200,15 +3194,15 @@
             def with_dependencies(model: Model) -> Stream:
                 load = self.load_by_id_merged(model, in_stream, variables, allowed_on_kind, **ctx.env)
                 handler = self.update_node_in_graphdb(model, **ctx.env) if expect_node_result else self.no_update
                 return self.send_to_queue_stream(stream.map(load, fn), handler, True)
 
             # dependencies are not resolved directly (no async function is allowed here)
             async def load_model() -> Model:
-                return await cast(CLIDependencies, self.dependencies).model_handler.load_model(ctx.graph_name)
+                return await self.dependencies.model_handler.load_model(ctx.graph_name)
 
             dependencies = stream.call(load_model)
             return stream.flatmap(dependencies, with_dependencies)
 
         def setup_source() -> Stream:
             arg = {"args": args_parts_unquoted_parser.parse(formatter({}))}
             return self.send_to_queue_stream(stream.just((command_name, {}, arg)), self.no_update, True)
@@ -3323,15 +3317,15 @@
         def setup_stream(in_stream: Stream) -> Stream:
             def with_dependencies(model: Model) -> Stream:
                 load = self.load_by_id_merged(model, in_stream, variables, **ctx.env)
                 result_handler = self.update_node_in_graphdb(model, **ctx.env)
                 return self.send_to_queue_stream(stream.map(load, fn), result_handler, not ns.nowait)
 
             async def load_model() -> Model:
-                return await cast(CLIDependencies, self.dependencies).model_handler.load_model(ctx.graph_name)
+                return await self.dependencies.model_handler.load_model(ctx.graph_name)
 
             # dependencies are not resolved directly (no async function is allowed here)
             dependencies = stream.call(load_model)
             return stream.flatmap(dependencies, with_dependencies)
 
         return CLIFlow(setup_stream)
 
@@ -3480,15 +3474,15 @@
             "info": [],
         }
 
     async def create_backup(self, arg: Optional[str]) -> AsyncIterator[JsonElement]:
         maybe_proc: Optional[Process] = None
         async with TemporaryDirectory() as temp_dir:
             try:
-                db_config = cast(CLIDependencies, self.dependencies).config.db
+                db_config = self.dependencies.config.db
                 if not shutil.which("arangodump"):
                     raise CLIParseError("db_backup expects the executable `arangodump` to be in path!")
                 # fmt: off
                 process = await asyncio.create_subprocess_exec(
                     "arangodump",
                     "--progress", "false",  # do not show progress
                     "--include-system-collections", "true",  # graphs are considered a system collection
@@ -3543,15 +3537,15 @@
             maybe_proc: Optional[Process] = None
             try:
                 # extract tar file
                 with tarfile.open(backup_file, "r") as tar:
                     tar.extractall(temp_dir, members=safe_members_in_tarfile(tar))
 
                 # fmt: off
-                db_conf = cast(CLIDependencies, self.dependencies).config.db
+                db_conf = self.dependencies.config.db
                 process = await asyncio.create_subprocess_exec(
                     "arangorestore",
                     "--progress", "false",  # do not show progress
                     "--include-system-collections", "true",  # graphs are considered a system collection
                     "--threads", "8",  # default is 2
                     "--log.level", "error",  # only print error messages
                     "--input-directory", temp_dir,  # directory to write to
@@ -3772,17 +3766,15 @@
         async def list_templates() -> Tuple[Optional[int], AsyncIterator[Json]]:
             templates = await self.dependencies.template_expander.list_templates()
             return len(templates), stream.iterate(template_str(t) for t in templates)
 
         async def put_template(name: str, template_query: str) -> AsyncIterator[str]:
             # try to render_console the template with dummy values and see if the search can be parsed
             try:
-                rendered_query = cast(CLIDependencies, self.dependencies).template_expander.render(
-                    template_query, defaultdict(lambda: True)
-                )
+                rendered_query = self.dependencies.template_expander.render(template_query, defaultdict(lambda: True))
                 parse_query(rendered_query, **ctx.env)
             except Exception as ex:
                 raise CLIParseError(f"Given template does not define a valid search: {template_query}") from ex
             await self.dependencies.template_expander.put_template(Template(name, template_query))
             yield f"Template {name} added to the search library.\n{template_query}"
 
         async def delete_template(name: str) -> AsyncIterator[str]:
@@ -3976,15 +3968,15 @@
 
         async def perform_request(e: JsonElement) -> int:
             nonlocal retries_left
             data = None if template.no_body else (JsonPayload(e) if isinstance(e, (dict, list)) else e)
             authuser, authpass = template.auth.split(":", 1) if template.auth else (None, None)
             log.debug(f"Perform request with this template={template} and data={data}")
             try:
-                async with cast(CLIDependencies, self.dependencies).http_session.request(
+                async with self.dependencies.http_session.request(
                     template.method,
                     template.url,
                     headers=template.headers,
                     params=template.params,
                     data=data,
                     compress=template.compress,
                     timeout=template.timeout,
@@ -4677,15 +4669,15 @@
             ]
         }
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
         async def create_certificate(
             common_name: str, dns_names: List[str], ip_addresses: List[str], days_valid: int
         ) -> AsyncIterator[str]:
-            key, cert = cast(CLIDependencies, self.dependencies).cert_handler.create_key_and_cert(
+            key, cert = self.dependencies.cert_handler.create_key_and_cert(
                 common_name, dns_names, ip_addresses, days_valid
             )
             async with TemporaryDirectory() as tmpdir:
                 key_file = os.path.join(tmpdir, f"{common_name}.key")
                 cert_file = os.path.join(tmpdir, f"{common_name}.crt")
                 write_cert_to_file(cert, cert_file, rename=False)
                 write_key_to_file(key, key_file, rename=False)
@@ -5051,15 +5043,15 @@
         async def apps_list() -> AsyncIterator[JsonElement]:
             async for app in self.dependencies.infra_apps_package_manager.list():
                 yield app
 
         async def app_run(
             in_stream: JsGen, app_name: InfraAppName, dry_run: bool, config: Optional[str], argv: List[str]
         ) -> AsyncIterator[JsonElement]:
-            runtime = cast(CLIDependencies, self.dependencies).infra_apps_runtime
+            runtime = self.dependencies.infra_apps_runtime
             manifest = await self.dependencies.infra_apps_package_manager.get_manifest(app_name)
             if not manifest:
                 raise ValueError(f"App {app_name} is not installed.")
             app_config = None
             config = config or f"resoto.apps.{app_name}"
             ce = await self.dependencies.config_handler.get_config(ConfigId(config))
             if ce:
@@ -5476,15 +5468,15 @@
                     async for line in export_lines:
                         await f.write(line + "\n")
                 yield FilePath.user_local(file_name, path).json()
 
         async def graph_export(graph_name: Optional[GraphName], file_name: str) -> AsyncIterator[JsonElement]:
             if not graph_name:
                 graph_name = ctx.graph_name
-            lines = cast(CLIDependencies, self.dependencies).graph_manager.export_graph(graph_name)
+            lines = self.dependencies.graph_manager.export_graph(graph_name)
             return write_result_to_file(lines, file_name)
 
         async def graph_import(
             graph_name: Optional[GraphName], file_name: str, force: bool
         ) -> AsyncIterator[JsonElement]:
             if not graph_name:
                 graph_name = ctx.graph_name
@@ -5651,15 +5643,15 @@
         return "Synchronizes data to an SQL database."
 
     async def list_kinds_of_query(
         self, query: Optional[Query], graph_name: GraphName, model: Model
     ) -> List[ComplexKind]:
         assert query is not None, "No query provided, not sure what to synchronize?"
         assert query.aggregate is None, "Aggregates are not supported for synchronization"
-        db = deps(self).db_access.get_graph_db(graph_name)
+        db = self.dependencies.db_access.get_graph_db(graph_name)
         aggregate_by_kind = Aggregate(
             [AggregateVariable(AggregateVariableName("reported.kind"), "kind")],
             [AggregateFunction("sum", 1)],
         )
         query = evolve(query, aggregate=aggregate_by_kind)
         async with await db.search_aggregation(QueryModel(query, model)) as cursor:
             return [
@@ -5696,32 +5688,32 @@
                 db_string += "?" + "&".join([f"{k}={v}" for pl in p.arg for k, v in pl])
                 db_config = EngineConfig(db_string, p.batch_size)
 
                 sync_fn = partial(database_synchronize, db_config, p.complete_schema, p.drop_existing_tables)
                 if maybe_stream is not None:  # search | db sync
                     await sync_fn(query=ctx.query, in_stream=maybe_stream)
                 else:
-                    resoto_model = await deps(self).model_handler.load_model(ctx.graph_name)
+                    resoto_model = await self.dependencies.model_handler.load_model(ctx.graph_name)
                     query = Query(parts=[Part(term=IsTerm(["graph_root"]), navigation=NavigateUntilLeaf)])
-                    graph_db = deps(self).db_access.get_graph_db(ctx.graph_name)
+                    graph_db = self.dependencies.db_access.get_graph_db(ctx.graph_name)
                     async with await graph_db.search_graph_gen(
                         QueryModel(query, resoto_model), timeout=timedelta(weeks=200000)
                     ) as cursor:
                         await sync_fn(query=query, in_stream=stream.iterate(cursor))
 
                 yield FilePath.user_local(p.database, file_output).json() if file_output else "Database synchronized."
 
         async def database_synchronize(
             engine_config: EngineConfig,
             complete_model: bool,
             drop_existing_tables: bool,
             query: Optional[Query],
             in_stream: Stream,
         ) -> None:
-            resoto_model = await deps(self).model_handler.load_model(ctx.graph_name)
+            resoto_model = await self.dependencies.model_handler.load_model(ctx.graph_name)
 
             if complete_model:
                 complex_kinds = resoto_model.complex_kinds()
                 kinds = list(resoto_model.kinds.values())
             else:
                 # only export the kinds that are exported by this query
                 complex_kinds = await self.list_kinds_of_query(query, ctx.graph_name, resoto_model)
@@ -5795,15 +5787,15 @@
                     envelope={CLIEnvelope.no_history: "yes"},
                     produces=produces,
                 )
         else:
             return CLISource.single(lambda: stream.just(self.rendered_help(ctx)))
 
 
-def all_commands(d: CLIDependencies) -> List[CLICommand]:
+def all_commands(d: Dependencies) -> List[CLICommand]:
     commands = [
         AggregateCommand(d, "search"),
         AggregateToCountCommand(d, "search"),
         AncestorsPart(d, "search"),
         CertificateCommand(d, "setup", allowed_in_source_position=True),
         ChunkCommand(d, "misc"),
         CleanCommand(d, "action"),
```

### Comparing `resotocore-3.6.0/resotocore/cli/model.py` & `resotocore-3.6.1/resotocore/cli/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,29 @@
 from abc import ABC, abstractmethod
 from asyncio import iscoroutine
 from datetime import timedelta
 from enum import Enum
 from functools import reduce
 from pathlib import Path
 from textwrap import dedent
-from typing import Optional, List, Any, Dict, Tuple, Callable, Union, Awaitable, Type, cast, Set, AsyncIterator
+from typing import (
+    Optional,
+    List,
+    Any,
+    Dict,
+    Tuple,
+    Callable,
+    Union,
+    Awaitable,
+    Type,
+    cast,
+    Set,
+    AsyncIterator,
+    TYPE_CHECKING,
+)
 
 from aiostream import stream
 from aiostream.core import Stream
 from attrs import define, field
 from parsy import test_char, string
 from rich.jupyter import JupyterMixin
 
@@ -26,14 +40,17 @@
 from resotocore.query.model import Query, variable_to_absolute, PathRoot
 from resotocore.query.template_expander import render_template
 from resotocore.types import Json, JsonElement
 from resotocore.util import AccessJson, uuid_str, from_utc, utc, utc_str
 from resotolib.parse_util import l_curly_dp, r_curly_dp
 from resotolib.utils import get_local_tzinfo
 
+if TYPE_CHECKING:
+    from resotocore.dependencies import Dependencies
+
 
 class MediaType(Enum):
     Json = 1
     FilePath = 2
     Markdown = 3
     String = 4
 
@@ -315,15 +332,17 @@
     """
     The CLIPart is the base for all participants of the cli execution.
     Source: generates a stream of objects
     Flow: transforms the elements in a stream of objects
     Sink: takes a stream of objects and creates a result
     """
 
-    def __init__(self, dependencies: Any, category: str = "misc", allowed_in_source_position: bool = False) -> None:
+    def __init__(
+        self, dependencies: Dependencies, category: str = "misc", allowed_in_source_position: bool = False
+    ) -> None:
         self.dependencies = dependencies
         self.category = category
         self.allowed_in_source_position = allowed_in_source_position
 
     @property
     @abstractmethod
     def name(self) -> str:
```

### Comparing `resotocore-3.6.0/resotocore/cli/tip_of_the_day.py` & `resotocore-3.6.1/resotocore/cli/tip_of_the_day.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/config/__init__.py` & `resotocore-3.6.1/resotocore/config/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/config/config_override_service.py` & `resotocore-3.6.1/resotocore/config/config_override_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pathlib import Path
 import yaml
 import logging
 from datetime import timedelta
 
 from resotocore.core_config import config_model
 from resotocore.model.typed_model import from_js
+from resotocore.service import Service
 from resotocore.types import Json
 from resotocore.ids import ConfigId
 from resotocore.util import Periodic
 from resotocore.config import ConfigOverride
 from resotocore.db.modeldb import ModelDb
 from resotocore.model.model import Model, Kind
 from resotolib.utils import merge_json_elements
@@ -22,15 +23,15 @@
 
 
 async def model_from_db(model_db: ModelDb) -> Model:
     kinds = [kind async for kind in model_db.all()]
     return Model.from_kinds(list(kinds))
 
 
-class ConfigOverrideService(ConfigOverride):
+class ConfigOverrideService(ConfigOverride, Service):
     def __init__(
         self, override_paths: List[Path], get_configs_model: Callable[[], Awaitable[Model]], sleep_time: float = 10.0
     ):
         self.override_paths = override_paths
         self._get_configs_model = get_configs_model
 
         self.overrides: Dict[ConfigId, Json] = {}
```

### Comparing `resotocore-3.6.0/resotocore/config/core_config_handler.py` & `resotocore-3.6.1/resotocore/config/core_config_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,30 +21,31 @@
     ResotoCoreSnapshotsRoot,
     SnapshotsScheduleConfig,
     CustomCommandsConfig,
     migrate_core_config,
     config_model as core_config_model,
     migrate_command_config,
 )
-from resotocore.dependencies import empty_config
+from resotocore.system_start import empty_config
 from resotocore.ids import SubscriberId, WorkerId, ConfigId
 from resotocore.message_bus import MessageBus, CoreMessage
 from resotocore.model.model import Kind
 from resotocore.model.typed_model import from_js
 from resotocore.report import ResotoReportBenchmark, ResotoReportCheck, Inspector, BenchmarkConfigRoot, CheckConfigRoot
 from resotocore.report.report_config import config_model as report_config_model
+from resotocore.service import Service
 from resotocore.types import Json
 from resotocore.user import config_model as user_config_model, UsersConfigId, ResotoUsersConfig
 from resotocore.util import deep_merge, restart_service, value_in_path, value_in_path_get
 from resotocore.worker_task_queue import WorkerTaskQueue, WorkerTaskDescription, WorkerTaskName, WorkerTask
 
 log = logging.getLogger(__name__)
 
 
-class CoreConfigHandler:
+class CoreConfigHandler(Service):
     def __init__(
         self,
         config: CoreConfig,
         message_bus: MessageBus,
         worker_task_queue: WorkerTaskQueue,
         config_handler: ConfigHandler,
         event_sender: AnalyticsEventSender,
```

### Comparing `resotocore-3.6.0/resotocore/console_renderer.py` & `resotocore-3.6.1/resotocore/console_renderer.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/constants.py` & `resotocore-3.6.1/resotocore/constants.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/core_config.py` & `resotocore-3.6.1/resotocore/core_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -493,14 +493,18 @@
         default=4 * 3600,
         metadata={"description": "If a graph update takes longer than this duration, the update is aborted."},
     )
     keep_history: bool = field(
         default=True,
         metadata={"description": "If true, changes of the graph are stored and are available via history."},
     )
+    parallel_imports: int = field(
+        default=5,
+        metadata={"description": "Number of parallel graph merge requests handled in parallel."},
+    )
 
     def merge_max_wait_time(self) -> timedelta:
         return timedelta(seconds=self.merge_max_wait_time_seconds)
 
     def abort_after(self) -> timedelta:
         return timedelta(seconds=self.abort_after_seconds)
```

### Comparing `resotocore-3.6.0/resotocore/db/__init__.py` & `resotocore-3.6.1/resotocore/db/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/db/arango_query.py` & `resotocore-3.6.1/resotocore/db/arango_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import logging
 import re
 from collections import defaultdict
-from attrs import evolve
+from textwrap import dedent
 from typing import Union, List, Tuple, Any, Optional, Dict, Set
 
 from arango.typings import Json
+from attrs import evolve
 
 from resotocore.constants import less_greater_then_operations as lgt_ops, arangodb_matches_null_ops
 from resotocore.db import EstimatedSearchCost, EstimatedQueryCostRating as Rating
 from resotocore.db.arangodb_functions import as_arangodb_function
 from resotocore.db.model import QueryModel
 from resotocore.model.graph_access import Section, Direction
 from resotocore.model.model import SyntheticProperty, ResolvedProperty
@@ -34,16 +35,18 @@
     MergeTerm,
     MergeQuery,
     Query,
     SortOrder,
     FulltextTerm,
     Limit,
     ContextTerm,
+    WithUsage,
 )
-from resotocore.util import first, set_value_in_path, exist
+from resotocore.util import first, set_value_in_path, exist, utc_str
+from resotolib.durations import duration_str
 
 log = logging.getLogger(__name__)
 
 # Those words are keywords in aql and need to be "escaped"
 escape_aql_parts = {
     "collect",
     "filter",
@@ -396,14 +399,59 @@
                 for_stmt = f"{for_stmt}{sort_by}{limited}"
             f_res = f'MERGE({crsr}, {{metadata:MERGE({md}, {{"query_tag": "{p.tag}"}})}})' if p.tag else crsr
             return_stmt = f"RETURN {f_res}"
             reverse = "REVERSE" if p.reverse_result else ""
             query_part += f"LET {filtered_out} = {reverse}({for_stmt}{return_stmt})"
             return filtered_out
 
+        def with_usage(in_crsr: str, usage: WithUsage, term: Term, limit: Optional[Limit]) -> str:
+            nonlocal query_part
+
+            # split the term and create a filter statement for everything before the usage predicates
+            before_term, after_term = term.split_by_usage()
+
+            # the limit is applied here, when the after term does not filter at all
+            after_filter_cursor = filter_statement(in_crsr, before_term, limit=limit if after_term.is_all else None)
+
+            # add the usage predicates
+            usage_crs = next_crs("with_usage")
+            start = next_bind_var_name()
+            end = next_bind_var_name()
+            start_s = next_bind_var_name()
+            duration = next_bind_var_name()
+            start_time = usage.start_from_now()
+            end_time = usage.end_from_now()
+            bind_vars[start] = start_time.timestamp()
+            bind_vars[end] = end_time.timestamp()
+            bind_vars[start_s] = utc_str(start_time)
+            bind_vars[duration] = duration_str(end_time - start_time)
+            avgs = []
+            merges = []
+            for mn in usage.metrics:
+                avgs.append(f"{mn}_min = MIN(m.v.{mn}.min), {mn}_avg = AVG(m.v.{mn}.avg), {mn}_max = MAX(m.v.{mn}.max)")
+                merges.append(f"{mn}: {{min: {mn}_min, avg: {mn}_avg, max: {mn}_max}}")
+            query_part += dedent(
+                f"""
+                let {usage_crs} = (
+                    for r in {after_filter_cursor}
+                        let resource=r
+                        let resource_usage = first(
+                            for m in {db.usage_db.collection_name}
+                            filter m.at>=@{start} and m.at<=@{end} and m.id==r._key
+                            collect aggregate {", ".join(avgs)}, count = sum(1)
+                            return {{usage:{{{",".join(merges)},entries:count,start:@{start_s},duration:@{duration}}}}}
+                        )
+                        return resource_usage.usage.entries ? merge(resource, resource_usage) : resource
+                )
+                """
+            )
+
+            # finally apply the filter that includes the usage predicates
+            return filter_statement(usage_crs, after_term, limit)
+
         def with_clause(in_crsr: str, clause: WithClause, limit: Optional[Limit]) -> str:
             nonlocal query_part
             # this is the general structure of the with_clause that is created
             #
             # FOR cloud in foo FILTER @0 in cloud.kinds
             #    FOR account IN 0..1 OUTBOUND cloud foo_default
             #    OPTIONS { bfs: true, uniqueVertices: 'global' }
@@ -524,24 +572,30 @@
                 all_walks_combined = ",".join(all_walks)
                 query_part += f"LET {nav_crsr} = UNION_DISTINCT({all_walks_combined})"
                 return nav_crsr
 
         # apply the limit in the filter statement only, when no with clause is present
         # otherwise the limit is applied in the with clause
         filter_limit = p.limit if p.with_clause is None else None
+        cursor = in_cursor
+        part_term = p.term
         if isinstance(p.term, MergeTerm):
-            # do not allow a limit in the prefilter
-            filter_cursor = filter_statement(in_cursor, p.term.pre_filter, None)
+            # only allow a limit in the prefilter, if there is no post filter
+            pre_limit = filter_limit if (p.term.post_filter is None or p.term.post_filter.is_all) else None
+            filter_cursor = filter_statement(cursor, p.term.pre_filter, pre_limit)
             cursor, merge_part = merge(filter_cursor, p.term.merge)
             query_part += merge_part
-            post = p.term.post_filter if p.term.post_filter else AllTerm()
             # always do the post filter in case of sort or limit
-            cursor = filter_statement(cursor, post, filter_limit)
+            part_term = p.term.post_filter if p.term.post_filter else AllTerm()
+        if p.with_usage and len(p.with_usage.metrics) > 0:
+            # filter is applied in the with usage
+            cursor = with_usage(cursor, p.with_usage, part_term, filter_limit)
         else:
-            cursor = filter_statement(in_cursor, p.term, filter_limit)
+            cursor = filter_statement(cursor, part_term, filter_limit)
+
         cursor = with_clause(cursor, p.with_clause, p.limit) if p.with_clause else cursor
         cursor = navigation(cursor, p.navigation) if p.navigation else cursor
         return p, cursor, filtered_out, query_part
 
     def sort(cursor: str, so: List[Sort]) -> str:
         def single_sort(single: Sort) -> str:
             prop_name, resolved, _ = prop_name_kind(single.name)
```

### Comparing `resotocore-3.6.0/resotocore/db/arangodb_extensions.py` & `resotocore-3.6.1/resotocore/db/arangodb_extensions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/db/arangodb_functions.py` & `resotocore-3.6.1/resotocore/db/arangodb_functions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/db/async_arangodb.py` & `resotocore-3.6.1/resotocore/db/async_arangodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from arango.cursor import Cursor
 from arango.database import StandardDatabase, Database, TransactionDatabase
 from arango.graph import Graph
 from arango.typings import Json, Jsons
 
 from resotocore.async_extensions import run_async
 from resotocore.error import QueryTookToLongError
-from resotocore.metrics import timed
 from resotocore.util import identity
 from resotocore.ids import GraphName
 
 log = logging.getLogger(__name__)
 
 
 class AsyncCursor(AsyncIterator[Any]):
@@ -154,15 +153,14 @@
         self.cursor.close()
 
 
 class AsyncArangoDBBase:
     def __init__(self, db: Database):
         self.db = db
 
-    @timed("arango", "aql")
     async def aql_cursor(
         self,
         query: str,
         trafo: Optional[Callable[[Json], Optional[Any]]] = None,
         count: bool = False,
         batch_size: Optional[int] = None,
         ttl: Optional[Number] = None,
@@ -204,15 +202,14 @@
             satellite_sync_wait,
             stream,
             skip_inaccessible_cols,
             max_runtime,
         )
         return AsyncCursorContext(cursor, trafo)
 
-    @timed("arango", "aql")
     async def aql(
         self,
         query: str,
         count: bool = False,
         batch_size: Optional[int] = None,
         ttl: Optional[Number] = None,
         bind_vars: Optional[Dict[str, Any]] = None,
@@ -252,26 +249,24 @@
             intermediate_commit_size,
             satellite_sync_wait,
             stream,
             skip_inaccessible_cols,
             max_runtime,
         )
 
-    @timed("arango", "explain")
     async def explain(
         self,
         query: str,
         all_plans: bool = False,
         max_plans: Optional[int] = None,
         opt_rules: Optional[Sequence[str]] = None,
         bind_vars: Optional[MutableMapping[str, str]] = None,
     ) -> Union[Json, Jsons]:
         return await run_async(self.db.aql.explain, query, all_plans, max_plans, opt_rules, bind_vars)  # type: ignore
 
-    @timed("arango", "execute_transaction")
     async def execute_transaction(
         self,
         command: str,
         params: Optional[Json] = None,
         read: Optional[Sequence[str]] = None,
         write: Optional[Sequence[str]] = None,
         sync: Optional[bool] = None,
@@ -291,25 +286,23 @@
             timeout,
             max_size,
             allow_implicit,
             intermediate_commit_count,
             intermediate_commit_size,
         )
 
-    @timed("arango", "get")
     async def get(
         self,
         collection: str,
         document: Union[str, Json],
         rev: Optional[str] = None,
         check_rev: bool = True,
     ) -> Optional[Json]:
         return await run_async(self.db.collection(collection).get, document, rev, check_rev)  # type: ignore
 
-    @timed("arango", "insert")
     async def insert(
         self,
         collection: str,
         document: Json,
         return_new: bool = False,
         sync: Optional[bool] = None,
         silent: bool = False,
@@ -329,15 +322,14 @@
             overwrite,
             return_old,
             overwrite_mode,
             keep_none,
             merge,
         )
 
-    @timed("arango", "update")
     async def update(
         self,
         collection: str,
         document: Json,
         check_rev: bool = True,
         merge: bool = True,
         keep_none: bool = True,
@@ -354,15 +346,14 @@
             keep_none,
             return_new,
             return_old,
             sync,
             silent,
         )
 
-    @timed("arango", "delete")
     async def delete(
         self,
         collection: str,
         document: Union[str, Json],
         rev: Optional[str] = None,
         check_rev: bool = True,
         ignore_missing: bool = False,
@@ -377,40 +368,36 @@
             check_rev,
             ignore_missing,
             return_old,
             sync,
             silent,
         )
 
-    @timed("arango", "all")
     async def all(self, collection: str, skip: Optional[int] = None, limit: Optional[int] = None) -> Cursor:
         return await run_async(self.db.collection(collection).all, skip, limit)  # type: ignore
 
-    @timed("arango", "keys")
     async def keys(self, collection: str) -> Cursor:
         return await run_async(self.db.collection(collection).keys)  # type: ignore
 
     async def count(self, collection: str) -> int:
         return await run_async(self.db.collection(collection).count)  # type: ignore
 
-    @timed("arango", "insert_many")
     async def insert_many(
         self,
         collection: str,
         documents: Sequence[Json],
         return_new: bool = False,
         sync: Optional[bool] = None,
         silent: bool = False,
         overwrite: bool = False,
         return_old: bool = False,
     ) -> Union[bool, List[Union[Json, ArangoServerError]]]:
         fn = self.db.collection(collection).insert_many
         return await run_async(fn, documents, return_new, sync, silent, overwrite, return_old)  # type: ignore
 
-    @timed("arango", "update_many")
     async def update_many(
         self,
         collection: str,
         documents: Sequence[Json],
         check_rev: bool = True,
         merge: bool = True,
         keep_none: bool = True,
@@ -420,15 +407,14 @@
         silent: bool = False,
     ) -> Union[bool, List[Union[Json, ArangoServerError]]]:
         fn = self.db.collection(collection).update_many
         return await run_async(
             fn, documents, check_rev, merge, keep_none, return_new, return_old, sync, silent  # type: ignore
         )
 
-    @timed("arango", "delete_many")
     async def delete_many(
         self,
         collection: str,
         documents: Sequence[Json],
         return_old: bool = False,
         check_rev: bool = True,
         sync: Optional[bool] = None,
```

### Comparing `resotocore-3.6.0/resotocore/db/configdb.py` & `resotocore-3.6.1/resotocore/db/configdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/db/db_access.py` & `resotocore-3.6.1/resotocore/db/db_access.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,72 +1,69 @@
 import logging
-from abc import ABC
 from argparse import Namespace
 from datetime import datetime, timezone, timedelta
 from time import sleep
 from typing import Dict, List, Tuple, Union, cast, Optional
 
 from arango import ArangoServerError
 from arango.client import ArangoClient
 from arango.database import StandardDatabase
 from dateutil.parser import parse
 from requests.exceptions import RequestException
 
-
 from resotocore.analytics import AnalyticsEventSender
 from resotocore.async_extensions import run_async
 from resotocore.core_config import CoreConfig
 from resotocore.db import SystemData
 from resotocore.db.arangodb_extensions import ArangoHTTPClient
 from resotocore.db.async_arangodb import AsyncArangoDB
 from resotocore.db.configdb import config_entity_db, config_validation_entity_db
+from resotocore.db.deferred_edge_db import pending_deferred_edge_db
 from resotocore.db.entitydb import EventEntityDb
 from resotocore.db.graphdb import ArangoGraphDB, GraphDB, EventGraphDB
 from resotocore.db.jobdb import job_db
 from resotocore.db.modeldb import ModelDb, model_db
-from resotocore.db.deferred_edge_db import pending_deferred_edge_db
+from resotocore.db.packagedb import app_package_entity_db
 from resotocore.db.runningtaskdb import running_task_db
 from resotocore.db.subscriberdb import subscriber_db
 from resotocore.db.system_data_db import SystemDataDb
 from resotocore.db.templatedb import template_entity_db
-from resotocore.db.packagedb import app_package_entity_db
 from resotocore.error import NoSuchGraph, RequiredDependencyMissingError
+from resotocore.ids import GraphName
 from resotocore.model.adjust_node import AdjustNode
-from resotocore.model.typed_model import from_js, to_js
 from resotocore.model.graph_access import EdgeTypes
+from resotocore.model.typed_model import from_js, to_js
+from resotocore.service import Service
 from resotocore.types import Json
-from resotocore.ids import GraphName
 from resotocore.util import Periodic, utc, shutdown_process, uuid_str, check_graph_name
 
 log = logging.getLogger(__name__)
 
 
-class DbAccess(ABC):
+class DbAccess(Service):
     def __init__(
         self,
         arango_database: StandardDatabase,
         event_sender: AnalyticsEventSender,
         adjust_node: AdjustNode,
         config: CoreConfig,
-        model_name: str = "model",
         subscriber_name: str = "subscribers",
         running_task_name: str = "running_tasks",
         job_name: str = "jobs",
         deferred_edge_name: str = "deferred_outer_edges",
         config_entity: str = "configs",
         config_validation_entity: str = "config_validation",
         configs_model: str = "configs_model",
         template_entity: str = "templates",
         infra_app_packages: str = "infra_app_packages",
     ):
         self.event_sender = event_sender
         self.database = arango_database
         self.db = AsyncArangoDB(arango_database)
         self.adjust_node = adjust_node
-        self.model_db = EventEntityDb(model_db(self.db, model_name), event_sender, model_name)
         self.graph_model_dbs: Dict[GraphName, ModelDb] = {}
         self.subscribers_db = EventEntityDb(subscriber_db(self.db, subscriber_name), event_sender, subscriber_name)
         self.system_data_db = SystemDataDb(self.db)
         self.running_task_db = running_task_db(self.db, running_task_name)
         self.pending_deferred_edge_db = pending_deferred_edge_db(self.db, deferred_edge_name)
         self.job_db = job_db(self.db, job_name)
         self.config_entity_db = config_entity_db(self.db, config_entity)
@@ -75,15 +72,14 @@
         self.template_entity_db = template_entity_db(self.db, template_entity)
         self.package_entity_db = app_package_entity_db(self.db, infra_app_packages)
         self.graph_dbs: Dict[str, GraphDB] = {}
         self.config = config
         self.cleaner = Periodic("outdated_updates_cleaner", self.check_outdated_updates, timedelta(seconds=60))
 
     async def start(self) -> None:
-        await self.model_db.create_update_schema()
         await self.subscribers_db.create_update_schema()
         await self.running_task_db.create_update_schema()
         await self.job_db.create_update_schema()
         await self.config_entity_db.create_update_schema()
         await self.config_validation_entity_db.create_update_schema()
         await self.configs_model_db.create_update_schema()
         await self.template_entity_db.create_update_schema()
@@ -114,15 +110,15 @@
             check_graph_name(name)
 
         db = self.get_graph_db(name, no_check=True)
         await db.create_update_schema()
         return db
 
     async def delete_graph(self, name: GraphName) -> None:
-        def delete(name: GraphName) -> None:
+        def delete() -> None:
             db = self.database
             if db.has_graph(name):
                 # delete arrangodb graph
                 db.delete_graph(name, drop_collections=True, ignore_missing=True)
                 # delete vertex collections just in case
                 db.delete_collection(name, ignore_missing=True)
                 # delete edge collections
@@ -133,15 +129,15 @@
                 db.delete_view(f"search_{name}", ignore_missing=True)
                 # remove all temp collection names
                 for coll in cast(List[Json], db.collections()):
                     if coll["name"].startswith(f"{name}_temp_"):
                         db.delete_collection(coll["name"], ignore_missing=True)
                 self.graph_dbs.pop(name, None)
 
-        return await run_async(delete, name)
+        return await run_async(delete)
 
     async def delete_graph_model(self, graph_name: GraphName) -> None:
         await self.db.delete_collection(self.graph_model_name(graph_name), ignore_missing=True)
         self.graph_model_dbs.pop(graph_name, None)
 
     async def list_graphs(self) -> List[GraphName]:
         return [a["name"] for a in cast(List[Json], self.database.graphs()) if not a["name"].endswith("_hs")]
@@ -153,17 +149,14 @@
             if not no_check and not self.database.has_graph(name):
                 raise NoSuchGraph(name)
             graph_db = ArangoGraphDB(self.db, name, self.adjust_node, self.config.graph_update)
             event_db = EventGraphDB(graph_db, self.event_sender)
             self.graph_dbs[name] = event_db
             return event_db
 
-    def get_model_db(self) -> ModelDb:
-        return self.model_db
-
     async def get_graph_model_db(self, graph_name: GraphName) -> ModelDb:
         if db := self.graph_model_dbs.get(graph_name):
             return db
         else:
             model_name = self.graph_model_name(graph_name)
             db = EventEntityDb(model_db(self.db, model_name), self.event_sender, model_name)
             await db.create_update_schema()
```

### Comparing `resotocore-3.6.0/resotocore/db/deferred_edge_db.py` & `resotocore-3.6.1/resotocore/db/deferred_edge_db.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/db/entitydb.py` & `resotocore-3.6.1/resotocore/db/entitydb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/db/graphdb.py` & `resotocore-3.6.1/resotocore/db/graphdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,27 @@
 
 from resotocore.analytics import CoreEvent, AnalyticsEventSender
 from resotocore.core_config import GraphUpdateConfig
 from resotocore.db import arango_query, EstimatedSearchCost
 from resotocore.db.arango_query import fulltext_delimiter
 from resotocore.db.async_arangodb import AsyncArangoDB, AsyncArangoTransactionDB, AsyncArangoDBBase, AsyncCursorContext
 from resotocore.db.model import GraphUpdate, QueryModel
+from resotocore.db.usagedb import resource_usage_db
 from resotocore.error import InvalidBatchUpdate, ConflictingChangeInProgress, NoSuchChangeError, OptimisticLockingFailed
 from resotocore.ids import NodeId, GraphName
 from resotocore.model.adjust_node import AdjustNode
 from resotocore.model.graph_access import GraphAccess, GraphBuilder, EdgeTypes, Section
-from resotocore.model.model import Model, ComplexKind, TransformKind, ResolvedProperty, synthetic_metadata_kinds
+from resotocore.model.model import (
+    Model,
+    ComplexKind,
+    TransformKind,
+    ResolvedProperty,
+    UsageDatapoint,
+    synthetic_metadata_kinds,
+)
 from resotocore.model.resolve_in_graph import NodePath, GraphResolver
 from resotocore.query.model import Query, FulltextTerm, MergeTerm, P
 from resotocore.types import JsonElement, EdgeType
 from resotocore.util import first, value_in_path_get, utc_str, uuid_str, value_in_path, json_hash, set_value_in_path
 
 log = logging.getLogger(__name__)
 
@@ -85,15 +93,19 @@
 
     @abstractmethod
     async def delete_node(self, node_id: NodeId) -> None:
         pass
 
     @abstractmethod
     async def merge_graph(
-        self, graph_to_merge: MultiDiGraph, model: Model, maybe_change_id: Optional[str] = None, is_batch: bool = False
+        self,
+        graph_to_merge: MultiDiGraph,
+        model: Model,
+        maybe_change_id: Optional[str] = None,
+        is_batch: bool = False,
     ) -> Tuple[List[str], GraphUpdate]:
         pass
 
     @abstractmethod
     async def list_in_progress_updates(self) -> List[Json]:
         pass
 
@@ -154,23 +166,28 @@
     async def create_update_schema(self) -> None:
         pass
 
     @abstractmethod
     async def copy_graph(self, to_graph: GraphName, to_snapshot: bool = False) -> "GraphDB":
         pass
 
+    @abstractmethod
+    async def insert_usage_data(self, data: List[UsageDatapoint]) -> None:
+        pass
+
 
 class ArangoGraphDB(GraphDB):
     def __init__(self, db: AsyncArangoDB, name: GraphName, adjust_node: AdjustNode, config: GraphUpdateConfig) -> None:
         super().__init__()
         self._name = name
         self.node_adjuster = adjust_node
         self.vertex_name = name
         self.in_progress = f"{name}_in_progress"
         self.node_history = f"{name}_node_history"
+        self.usage_db = resource_usage_db(db, f"{name}_usage")
         self.db = db
         self.config = config
 
     @property
     def name(self) -> GraphName:
         return self._name
 
@@ -178,15 +195,15 @@
         return f"{self.name}_{edge_type}"
 
     async def get_node(self, model: Model, node_id: NodeId) -> Optional[Json]:
         node = await self.by_id(node_id)
         return self.document_to_instance_fn(model)(node) if node is not None else None
 
     async def create_node(self, model: Model, node_id: NodeId, data: Json, under_node_id: NodeId) -> Json:
-        graph = GraphBuilder(model)
+        graph = GraphBuilder(model, uuid_str())
         graph.add_node(node_id, data)
         graph.add_edge(under_node_id, node_id, EdgeTypes.default)
         access = GraphAccess(graph.graph, node_id, {under_node_id})
         _, node_inserts, _, _ = self.prepare_nodes(access, [], model)
         _, edge_inserts, _ = self.prepare_edges(access, [], EdgeTypes.default)
         assert len(node_inserts) == 1
         assert len(edge_inserts) == 1
@@ -572,33 +589,37 @@
             for a in EdgeTypes.all
         ]
         history_updates = [
             f'for e in {temp_name} filter e.action=="node_created" insert MERGE({{change: e.action, changed_at: e.data.created}}, UNSET(e.data, "_key", "flat", "hash")) in {self.node_history}',  # noqa: E501
             f'for e in {temp_name} filter e.action=="node_updated" insert MERGE({{change: e.action, changed_at: e.data.updated}}, UNSET(e.data, "_key", "flat", "hash")) in {self.node_history}',  # noqa: E501
             f'for e in {temp_name} filter e.action=="node_deleted" let node = Document(CONCAT("{self.vertex_name}/", e.data._key)) insert MERGE({{change: "node_deleted", deleted: e.data.deleted, changed_at: e.data.deleted}}, UNSET(node, "_key", "_id", "_rev", "flat", "hash")) in {self.node_history}',  # noqa: E501
         ]
+        usage_updates = [
+            f'for u in {self.usage_db.collection_name} filter u.change_id=="{change_id}" update {{_key: u.id}} with {{ usage: MERGE(u.v, {{ start: DATE_ISO8601(u.at*1000), duration: "1h" }}) }} in {self.vertex_name} options {{ mergeObjects: false }}'  # noqa: E501
+        ]
         updates = ";\n".join(
             map(
                 lambda aql: f"db._createStatement({{ query: `{aql}` }}).execute()",
                 (history_updates if self.config.keep_history else [])
                 + [
                     f'for e in {temp_name} filter e.action=="node_created" insert e.data in {self.vertex_name}'
                     ' OPTIONS{overwriteMode: "replace"}',
                     f'for e in {temp_name} filter e.action=="node_updated" update e.data in {self.vertex_name}'
                     " OPTIONS {mergeObjects: false}",
                     f'for e in {temp_name} filter e.action=="node_deleted" remove e.data in {self.vertex_name}',
                 ]
                 + edge_inserts
                 + edge_deletes
+                + usage_updates
                 + [f'remove {{_key: "{change_key}"}} in {self.in_progress}'],
             )
         )
         await self.db.execute_transaction(
             f'function () {{\nvar db=require("@arangodb").db;\n{updates}\n}}',
-            read=[temp_name],
+            read=[temp_name, self.usage_db.collection_name],
             write=[self.edge_collection(a) for a in EdgeTypes.all]
             + [self.vertex_name, self.in_progress, self.node_history],
         )
         log.info(f"Move temp->proper data: change_id={change_id} done.")
 
     async def mark_update(
         self, root_node_ids: List[str], parent_node_ids: List[str], change_id: str, is_batch: bool
@@ -731,15 +752,19 @@
 
         for edge_from, edge_to in access.not_visited_edges(edge_type):
             insert_edge(edge_from, edge_to)
 
         return info, edges_inserts, edges_deletes
 
     async def merge_graph(
-        self, graph_to_merge: MultiDiGraph, model: Model, maybe_change_id: Optional[str] = None, is_batch: bool = False
+        self,
+        graph_to_merge: MultiDiGraph,
+        model: Model,
+        maybe_change_id: Optional[str] = None,
+        is_batch: bool = False,
     ) -> Tuple[List[str], GraphUpdate]:
         change_id = maybe_change_id if maybe_change_id else uuid_str()
 
         async def prepare_graph(
             sub: GraphAccess, node_query: Tuple[str, Json], edge_query: Callable[[EdgeType], Tuple[str, Json]]
         ) -> Tuple[
             GraphUpdate, List[Json], List[Json], List[Json], Dict[EdgeType, List[Json]], Dict[EdgeType, List[Json]]
@@ -1036,14 +1061,15 @@
             # we only create the indexes on the vertex collection
             create_node_indexes(vertex)
         else:
             in_progress = await create_collection(self.in_progress)
             node_history_collection = await create_collection(self.node_history)
             create_node_indexes(vertex)
             create_update_collection_indexes(in_progress, node_history_collection)
+            await self.usage_db.create_update_schema()
 
         for edge_type in EdgeTypes.all:
             edge_collection = db.graph(self.name).edge_collection(self.edge_collection(edge_type))
             create_update_edge_indexes(edge_collection)
 
         await create_update_views(vertex)
         if init_with_data:
@@ -1118,14 +1144,19 @@
             )
 
         await create_new_collections(new_graph_db, to_snapshot=to_snapshot)
         await copy_data()
 
         return cast(GraphDB, new_graph_db)
 
+    async def insert_usage_data(self, data: List[UsageDatapoint]) -> None:
+        if self.name.startswith("snapshot"):
+            raise ValueError("Cannot insert usage data into a snapshot graph")
+        await self.usage_db.update_many(data)
+
     @staticmethod
     def db_edge_key(from_node: str, to_node: str) -> str:
         return str(uuid.uuid5(uuid.NAMESPACE_DNS, f"{from_node}:{to_node}"))
 
     # parameter: rid
     # return: the complete document
     def query_node_by_id(self) -> str:
@@ -1196,29 +1227,29 @@
         RETURN length
         """
 
     def query_active_updates(self) -> str:
         return f"""
         FOR c IN `{self.in_progress}`
         RETURN {{id: c.change, created: c.created, affected_nodes: c.root_node_ids, is_batch: c.is_batch}}
-        """
+        """  # noqa: E501
 
     def query_active_change(self) -> str:
         return f"""
         FOR change IN `{self.in_progress}`
         FILTER @root_node_ids any in change.parent_node_ids OR @root_node_ids any in change.root_node_ids
         RETURN change
         """
 
     def update_active_change(self) -> str:
         return f"""
         FOR d in `{self.in_progress}`
         FILTER d.change == @change
         UPDATE d WITH {{created: DATE_ISO8601(DATE_NOW())}} in `{self.in_progress}`
-        """
+        """  # noqa: E501
 
 
 class EventGraphDB(GraphDB):
     def __init__(self, real: ArangoGraphDB, event_sender: AnalyticsEventSender):
         self.real = real
         self.event_sender = event_sender
         self.graph_name = real.name
@@ -1273,15 +1304,19 @@
         await self.event_sender.core_event(
             CoreEvent.NodesMetadataUpdated, {"graph": self.graph_name}, updated=len(node_ids)
         )
         async for a in result:
             yield a
 
     async def merge_graph(
-        self, graph_to_merge: MultiDiGraph, model: Model, maybe_change_id: Optional[str] = None, is_batch: bool = False
+        self,
+        graph_to_merge: MultiDiGraph,
+        model: Model,
+        maybe_change_id: Optional[str] = None,
+        is_batch: bool = False,
     ) -> Tuple[List[str], GraphUpdate]:
         roots, info = await self.real.merge_graph(graph_to_merge, model, maybe_change_id, is_batch)
         root_counter: Dict[str, int] = {}
         for root in roots:
             root_node = graph_to_merge.nodes[root]
             rep_id = value_in_path_get(root_node, NodePath.reported_id, root)
             root_counter[f"node_count_{rep_id}.total"] = value_in_path_get(root_node, NodePath.descendant_count, 0)
@@ -1373,7 +1408,10 @@
 
     async def copy_graph(self, to_graph: GraphName, to_snapshot: bool = False) -> GraphDB:
         await self.event_sender.core_event(
             CoreEvent.GraphCopied,
             {"graph": self.graph_name, "to_graph": to_graph},
         )
         return await self.real.copy_graph(to_graph, to_snapshot=to_snapshot)
+
+    async def insert_usage_data(self, data: List[UsageDatapoint]) -> None:
+        await self.real.insert_usage_data(data)
```

### Comparing `resotocore-3.6.0/resotocore/db/model.py` & `resotocore-3.6.1/resotocore/db/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/db/packagedb.py` & `resotocore-3.6.1/resotocore/db/packagedb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/db/runningtaskdb.py` & `resotocore-3.6.1/resotocore/db/runningtaskdb.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from resotocore.ids import TaskId, TaskDescriptorId
 from resotocore.message_bus import Message, ActionInfo, ActionError
 from resotocore.model.typed_model import to_js, from_js
 from resotocore.task.task_description import RunningTask
 from resotocore.types import Json, JsonElement
 from resotocore.util import utc, utc_str
 from resotolib.durations import duration_str
+from resotolib.utils import freeze
 
 log = logging.getLogger(__name__)
 
 
 @define(order=True, hash=True, frozen=True)
 class RunningTaskStepInfo:
     step_name: str
@@ -62,14 +63,16 @@
     task_duration: Optional[timedelta] = None
     # indicates if this task is still active
     done: bool = False
     # indicates if this task had warnings
     has_info: bool = False
     # indicates if this task had errors
     has_error: bool = False
+    # metadata about the task, such as last stage creation tims
+    metadata: Json = field(factory=dict)
 
     def info_messages(self) -> List[Union[ActionInfo, ActionError]]:
         return [m for m in iter(self.received_messages) if isinstance(m, (ActionInfo, ActionError))]
 
     @staticmethod
     def data(wi: RunningTask) -> RunningTaskData:
         return RunningTaskData(
@@ -86,14 +89,15 @@
             not wi.is_active,
             any(True for msg in wi.info_messages if isinstance(msg, ActionInfo) and msg.level == "info"),
             any(
                 True
                 for msg in wi.info_messages
                 if (isinstance(msg, ActionInfo) and msg.level == "error") or isinstance(msg, ActionError)
             ),
+            freeze(wi.metadata),
         )
 
 
 class RunningTaskDb(EntityDb[str, RunningTaskData]):
     @abstractmethod
     def all_running(self) -> AsyncGenerator[RunningTaskData, None]:
         pass
@@ -120,14 +124,22 @@
         started_before: Optional[datetime] = None,
         with_info: Optional[bool] = None,
         with_error: Optional[bool] = None,
         limit: Optional[int] = None,
     ) -> AsyncCursorContext:
         pass
 
+    @abstractmethod
+    async def last(
+        self,
+        *,
+        descriptor_id: Optional[TaskDescriptorId] = None,
+    ) -> Optional[RunningTaskData]:
+        pass
+
 
 class ArangoRunningTaskDb(ArangoEntityDb[str, RunningTaskData], RunningTaskDb):
     def __init__(self, db: AsyncArangoDB, collection: str):
         super().__init__(db, collection, RunningTaskData, lambda k: k.id)
 
     async def create_update_schema(self) -> None:
         await super().create_update_schema()
@@ -190,14 +202,39 @@
         with await self.db.aql(aql) as crsr:
             for elem in crsr:
                 name = elem.pop("name")
                 elem["average_duration"] = duration_str(timedelta(seconds=elem["average_duration"]), precision=2)
                 result[name] = elem
         return result
 
+    async def last(
+        self,
+        *,
+        descriptor_id: Optional[TaskDescriptorId] = None,
+    ) -> Optional[RunningTaskData]:
+        if descriptor_id:
+            descriptor_clause = "AND rt.task_descriptor_id == @descriptor_id"
+            bind_vars = {"descriptor_id": descriptor_id}
+        else:
+            descriptor_clause = ""
+            bind_vars = None
+
+        aql = f"""
+        FOR rt in {self.collection_name}
+        FILTER rt.done == true {descriptor_clause}
+        SORT rt.task_started_at DESC
+        LIMIT 1
+        RETURN rt
+        """
+
+        async with await self.db.aql_cursor(aql, bind_vars=bind_vars) as crsr:
+            async for elem in crsr:
+                return from_js(elem, RunningTaskData)
+        return None
+
     async def filtered(
         self,
         *,
         task_id: Optional[TaskId] = None,
         descriptor_id: Optional[str] = None,
         started_after: Optional[datetime] = None,
         started_before: Optional[datetime] = None,
```

### Comparing `resotocore-3.6.0/resotocore/db/system_data_db.py` & `resotocore-3.6.1/resotocore/db/system_data_db.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/dependencies.py` & `resotocore-3.6.1/resotocore/system_start.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/error.py` & `resotocore-3.6.1/resotocore/error.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/graph_manager/graph_manager.py` & `resotocore-3.6.1/resotocore/graph_manager/graph_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import logging
 
 from resotocore.db.db_access import DbAccess
 from resotocore.db.graphdb import EventGraphDB
 from resotocore.util import utc_str, UTC_Date_Format_short, utc
 from resotocore.ids import GraphName, TaskDescriptorId
-from resotocore.web.service import Service
+from resotocore.service import Service
 from resotocore.util import check_graph_name, Periodic
 from resotocore.types import Json
 from resotocore.model.model import Kind
 from resotocore.model.typed_model import from_js, to_js_str
 from resotocore.model.graph_access import EdgeTypes
 from resotocore.db.async_arangodb import AsyncCursor
 from resotocore.config.core_config_handler import CoreConfigHandler
```

### Comparing `resotocore-3.6.0/resotocore/infra_apps/local_runtime.py` & `resotocore-3.6.1/resotocore/infra_apps/local_runtime.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import List, AsyncIterator, Type, Optional, Any
 from resotocore.infra_apps.runtime import Runtime
 from resotocore.infra_apps.manifest import AppManifest
+from resotocore.service import Service
 from resotocore.types import Json, JsonElement
 from resotocore.ids import GraphName
 from resotocore.db.model import QueryModel
 from resotocore.cli.model import CLI, CLIContext
 from resotocore.cli import NoExitArgumentParser
 from jinja2 import Environment
 import logging
@@ -15,15 +16,15 @@
 from resotolib.asynchronous.utils import async_lines
 from pydoc import locate
 
 
 log = logging.getLogger(__name__)
 
 
-class LocalResotocoreAppRuntime(Runtime):
+class LocalResotocoreAppRuntime(Runtime, Service):
     """
     Runtime implementation that runs the Infrastructure Apps directly on the resotocore.
     Currently, only the Jinja2 language is supported.
     """
 
     def __init__(self, cli: CLI) -> None:
         self.cli = cli
```

### Comparing `resotocore-3.6.0/resotocore/infra_apps/manifest.py` & `resotocore-3.6.1/resotocore/infra_apps/manifest.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/infra_apps/package_manager.py` & `resotocore-3.6.1/resotocore/infra_apps/package_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from resotocore.config import ConfigEntity
 from resotocore.ids import InfraAppName, ConfigId
 from resotocore.model.model import Kind, ComplexKind
 from resotocore.types import Json
 from resotocore.model.typed_model import from_js
 from resotocore.cli.model import InfraAppAlias, InfraAppAliasParameter
 from logging import getLogger
-from resotocore.web.service import Service
+from resotocore.service import Service
 
 logger = getLogger(__name__)
 
 
 def config_id(name: InfraAppName) -> ConfigId:
     return ConfigId(f"resoto.apps.{name}")
```

### Comparing `resotocore-3.6.0/resotocore/infra_apps/runtime.py` & `resotocore-3.6.1/resotocore/infra_apps/runtime.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/bootstrap.js` & `resotocore-3.6.1/resotocore/jupyterlite/bootstrap.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1037.51967a2.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1037.51967a2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1079.cdbaf67.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1079.cdbaf67.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1084.4cd1c89.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1084.4cd1c89.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1113.23c9417.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1113.23c9417.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1125.129d070.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1125.129d070.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1163.ac28297.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1163.ac28297.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1221.c51249a.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1221.c51249a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1245.be46619.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1245.be46619.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1261.199fc1d.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1261.199fc1d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1272.f334098.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1272.f334098.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1278.0524a4a.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1278.0524a4a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt` & `resotocore-3.6.1/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1290.3981211.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1290.3981211.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1295.46e72b8.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1295.46e72b8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1310.23bbe67.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1310.23bbe67.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1320.21effe3.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1320.21effe3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1325.f76267c.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1325.f76267c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1408.7461890.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1408.7461890.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1440.a9e7ea1.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1440.a9e7ea1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1483.616d9ab.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1483.616d9ab.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1489.e50b6d4.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1489.e50b6d4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1507.5705605.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1507.5705605.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/152.525d460.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/152.525d460.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1520.4e2eb21.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1520.4e2eb21.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1555.e188f3f.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1555.e188f3f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1559.7c89925.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1559.7c89925.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/160.5f28731.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/160.5f28731.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1603.370a2a6.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1603.370a2a6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1644.0e49167.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1644.0e49167.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1667.f0afb2b.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1667.f0afb2b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1687.27f1ad6.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1687.27f1ad6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1725.f151c33.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1725.f151c33.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1767.c8c2f26.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1767.c8c2f26.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1806.1aaf66b.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1806.1aaf66b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1838.1202b16.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1838.1202b16.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1909.28a2def.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1909.28a2def.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/1989.88d258f.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/1989.88d258f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2030.1562cc6.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2030.1562cc6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2047.baed97b.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2047.baed97b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2099.f4b6fcd.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2099.f4b6fcd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2118.5b65f70.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2118.5b65f70.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/213.5769e57.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/213.5769e57.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2161.dcb27b8.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2161.dcb27b8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2169.635c88e.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2169.635c88e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/217.90d10e2.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/217.90d10e2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2212.72be094.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2212.72be094.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2287.997c38e.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2287.997c38e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt` & `resotocore-3.6.1/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2303.9ff8710.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2303.9ff8710.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2319.6b4cbb7.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2319.6b4cbb7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2329.4c5ca6d.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2329.4c5ca6d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2351.fbd96d8.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2351.fbd96d8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2358.d5cf7c8.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2358.d5cf7c8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2359.6451c3e.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2359.6451c3e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/237.f765e77.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/237.f765e77.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2384.71782be.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2384.71782be.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/240.cddc46b.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/240.cddc46b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2431.648d237.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2431.648d237.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2546.1f48267.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2546.1f48267.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2557.75e9da2.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2557.75e9da2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/261.5f53c0e.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/261.5f53c0e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2629.c0e1cd6.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2629.c0e1cd6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2788.46acc8a.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2788.46acc8a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2834.942acc6.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2834.942acc6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2887.47ba752.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2887.47ba752.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2956.8880209.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2956.8880209.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/2973.2a51dc4.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/2973.2a51dc4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3004.255e79c.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/3004.255e79c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/302.8bcc38f.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/302.8bcc38f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3037.70ee38d.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/3037.70ee38d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3042.7cfad84.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/3042.7cfad84.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3051.34fac68.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/3051.34fac68.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3122.2289fca.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/3122.2289fca.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3151.10ef4de.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/3151.10ef4de.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/316.c850a76.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/316.c850a76.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3196.4e35a17.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/3196.4e35a17.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3265.a80440a.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/3265.a80440a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3277.9c04e75.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/3277.9c04e75.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/330.126fa98.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/330.126fa98.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3392.29fe6b9.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/3392.29fe6b9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3413.480a49d.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/3413.480a49d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3444.47d5ea1.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/3444.47d5ea1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3469.7d14d0b.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/3469.7d14d0b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3546.fee1bd7.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/3546.fee1bd7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/362.6716970.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/362.6716970.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3708.410d087.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/3708.410d087.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3850.903abc2.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/3850.903abc2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt` & `resotocore-3.6.1/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3880.bd39dce.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/3880.bd39dce.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3970.236586f.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/3970.236586f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3976.58893b9.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/3976.58893b9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt` & `resotocore-3.6.1/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/3979.385527e.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/3979.385527e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/400.d72234b.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/400.d72234b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4018.1a35967.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4018.1a35967.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/406.9b7af92.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/406.9b7af92.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4117.a8107fd.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4117.a8107fd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4182.e2430f9.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4182.e2430f9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4191.02bbea8.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4191.02bbea8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4197.53ab10b.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4197.53ab10b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4206.a5f8bb0.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4206.a5f8bb0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4207.0d0580b.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4207.0d0580b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4262.bb73457.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4262.bb73457.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4298.5ee510c.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4298.5ee510c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/44.0cfa785.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/44.0cfa785.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt` & `resotocore-3.6.1/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4410.e4a25d3.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4410.e4a25d3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4466.64d23d1.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4466.64d23d1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/451.d9683ad.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/451.d9683ad.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4535.34b060a.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4535.34b060a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4565.43bdb91.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4565.43bdb91.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4569.f374f9d.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4569.f374f9d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4615.eb5d40a.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4615.eb5d40a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4658.090d4a9.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4658.090d4a9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4690.3dd4096.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4690.3dd4096.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4715.e7690b9.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4715.e7690b9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4749.46ebbb2.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4749.46ebbb2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4750.56c06ab.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4750.56c06ab.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4856.2d7415f.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4856.2d7415f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4875.375150e.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4875.375150e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/489.b981dea.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/489.b981dea.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/490.c2624d4.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/490.c2624d4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4905.667bf33.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4905.667bf33.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4931.430433b.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4931.430433b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/4942.b96c164.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/4942.b96c164.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5016.dd2fe83.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5016.dd2fe83.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5072.733a1b5.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5072.733a1b5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/509.6448878.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/509.6448878.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5096.8ed0d8e.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5096.8ed0d8e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5126.eecad7a.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5126.eecad7a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5129.1ba4763.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5129.1ba4763.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5153.763d8fa.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5153.763d8fa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5155.06b4ea9.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5155.06b4ea9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5193.e9f6866.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5193.e9f6866.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5213.3e1a360.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5213.3e1a360.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5227.8c8acd8.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5227.8c8acd8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5238.1751cc3.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5238.1751cc3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/528.2262cb0.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/528.2262cb0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5292.79d4aba.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5292.79d4aba.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5437.31236f7.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5437.31236f7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5489.848a8cf.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5489.848a8cf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5508.317fca3.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5508.317fca3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/554.ac98303.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/554.ac98303.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/555.2cd31dd.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/555.2cd31dd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5573.ebcdb93.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5573.ebcdb93.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5666.c5e5324.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5666.c5e5324.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5710.70d0b1d.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5710.70d0b1d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5747.94ad626.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5747.94ad626.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/582.21b8e7d.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/582.21b8e7d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5823.5045bdb.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5823.5045bdb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5851.30b7b2a.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5851.30b7b2a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5878.32d92fa.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5878.32d92fa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5880.68f975b.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5880.68f975b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5955.88508f7.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5955.88508f7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/5971.88c5642.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/5971.88c5642.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6080.aa0ff24.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6080.aa0ff24.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/61.2808a0d.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/61.2808a0d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6136.b8ba2b2.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6136.b8ba2b2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6141.9831d58.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6141.9831d58.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6475.6037fbb.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6475.6037fbb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6493.d796aa5.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6493.d796aa5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6556.b3d9293.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6556.b3d9293.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6571.2c8884e.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6571.2c8884e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6576.3ea568e.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6576.3ea568e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6591.94ed352.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6591.94ed352.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6612.1632879.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6612.1632879.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6623.ae3b3cc.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6623.ae3b3cc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6664.2160109.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6664.2160109.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6747.47be7f5.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6747.47be7f5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6748.be68f5f.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6748.be68f5f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6870.7940288.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6870.7940288.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6879.c8367a5.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6879.c8367a5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6898.9bbc12a.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6898.9bbc12a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6952.f68b818.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6952.f68b818.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6985.321ad92.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6985.321ad92.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6993.32cf9a6.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6993.32cf9a6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/6997.b06fe71.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/6997.b06fe71.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/7041.d4f561e.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/7041.d4f561e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/7058.805c88e.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/7058.805c88e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/7174.6c45206.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/7174.6c45206.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/7334.8859b1b.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/7334.8859b1b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/7359.6ee65ec.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/7359.6ee65ec.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/7364.195178b.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/7364.195178b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/7380.58a4413.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/7380.58a4413.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/7427.f9c2017.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/7427.f9c2017.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/7463.18fd278.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/7463.18fd278.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/7509.1e0189e.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/7509.1e0189e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/7526.1a303e5.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/7526.1a303e5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/7537.1323a15.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/7537.1323a15.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/7692.33d5169.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/7692.33d5169.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/7746.5908d29.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/7746.5908d29.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/7808.1d582a2.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/7808.1d582a2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/783.c156751.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/783.c156751.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/7858.2386e4d.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/7858.2386e4d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/7941.01ea680.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/7941.01ea680.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8005.c5ad7b2.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8005.c5ad7b2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8028.39e2fa1.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8028.39e2fa1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8061.cc62561.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8061.cc62561.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8101.cf46d02.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8101.cf46d02.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/812.9b0e86e.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/812.9b0e86e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/816.c8050f2.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/816.c8050f2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8165.b2c3285.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8165.b2c3285.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8232.a578bf9.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8232.a578bf9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/824.8678196.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/824.8678196.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8270.89fe7e1.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8270.89fe7e1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/833.9cc6653.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/833.9cc6653.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8370.8f855e5.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8370.8f855e5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8373.96b0b3a.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8373.96b0b3a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8389.ffe031f.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8389.ffe031f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8412.1528057.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8412.1528057.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8427.4923f43.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8427.4923f43.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8542.027afdc.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8542.027afdc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8594.0112f03.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8594.0112f03.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8656.d5b8e92.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8656.d5b8e92.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8685.d78bdab.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8685.d78bdab.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8698.9817d75.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8698.9817d75.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8732.9320f73.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8732.9320f73.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8785.cf4fe95.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8785.cf4fe95.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8828.77c71d0.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8828.77c71d0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8883.80c7b63.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8883.80c7b63.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8976.3816942.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8976.3816942.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/8990.2a453cf.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/8990.2a453cf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9035.1e45c1b.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9035.1e45c1b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9053.45b77fc.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9053.45b77fc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9077.fefb6ca.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9077.fefb6ca.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9128.b8fa6f0.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9128.b8fa6f0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9156.0cefbd3.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9156.0cefbd3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9170.0023587.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9170.0023587.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9196.315f9f9.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9196.315f9f9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9198.9971d70.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9198.9971d70.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/920.d15c177.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/920.d15c177.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9253.0b31caa.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9253.0b31caa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9266.bacd0dd.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9266.bacd0dd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9307.c3a00ed.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9307.c3a00ed.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9321.869e413.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9321.869e413.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9344.ba0abcf.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9344.ba0abcf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9382.9014799.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9382.9014799.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9440.1b10b8f.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9440.1b10b8f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9464.79e6ac5.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9464.79e6ac5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9502.9a24831.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9502.9a24831.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9507.1e6cc5d.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9507.1e6cc5d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9602.62bf0f1.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9602.62bf0f1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9621.e2e8b5d.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9621.e2e8b5d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9622.ccab065.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9622.ccab065.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9626.a178bd0.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9626.a178bd0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9647.ed91993.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9647.ed91993.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9657.bc5c60e.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9657.bc5c60e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/97.ad126b0.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/97.ad126b0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9712.796a0a1.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9712.796a0a1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9737.7dc8f98.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9737.7dc8f98.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9777.0b8a504.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9777.0b8a504.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9793.6d63a85.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9793.6d63a85.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9806.652c162.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9806.652c162.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9865.2e3db6f.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9865.2e3db6f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/989.bcca86a.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/989.bcca86a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9943.f3f35c7.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9943.f3f35c7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9958.25c8c06.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9958.25c8c06.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/9960.64cd61e.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/9960.64cd61e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/add-above.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/add-above.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/add-below.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/add-below.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/bug-dot.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/bug-dot.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/bug.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/bug.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/build.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/build.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/case-sensitive.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/case-sensitive.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/close.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/close.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/copyright.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/copyright.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/cut.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/cut.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/duplicate.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/duplicate.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/fa-brands-400.woff2` & `resotocore-3.6.1/resotocore/jupyterlite/build/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/fa-regular-400.woff2` & `resotocore-3.6.1/resotocore/jupyterlite/build/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/fa-solid-900.woff2` & `resotocore-3.6.1/resotocore/jupyterlite/build/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/html5.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/html5.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/json.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/json.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/julia.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/julia.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/jupyter-favicon.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/jupyter-favicon.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/jupyter.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/jupyter.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/jupyterlab-wordmark.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/jupyterlab-wordmark.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/lab/bundle.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/lab/bundle.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/listings-info.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/listings-info.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/move-down.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/move-down.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/move-up.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/move-up.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/not-trusted.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/not-trusted.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/palette.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/palette.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/pdf.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/pdf.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/python.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/python.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/react.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/react.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/regex.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/regex.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/schemas/all.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/schemas/all.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/service-worker-b2fb40a.js` & `resotocore-3.6.1/resotocore/jupyterlite/build/service-worker-b2fb40a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/settings.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/settings.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/tag.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/tag.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/terminal.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/terminal.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css` & `resotocore-3.6.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css` & `resotocore-3.6.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/third-party-licenses.json` & `resotocore-3.6.1/resotocore/jupyterlite/build/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/toc.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/toc.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/build/trusted.svg` & `resotocore-3.6.1/resotocore/jupyterlite/build/trusted.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/config-utils.js` & `resotocore-3.6.1/resotocore/jupyterlite/config-utils.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json` & `resotocore-3.6.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/files/example.ipynb` & `resotocore-3.6.1/resotocore/jupyterlite/files/example.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/icon-120x120.png` & `resotocore-3.6.1/resotocore/jupyterlite/icon-120x120.png`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/icon-512x512.png` & `resotocore-3.6.1/resotocore/jupyterlite/icon-512x512.png`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/index.html` & `resotocore-3.6.1/resotocore/jupyterlite/index.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/jupyter-lite.ipynb` & `resotocore-3.6.1/resotocore/jupyterlite/jupyter-lite.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/jupyter-lite.json` & `resotocore-3.6.1/resotocore/jupyterlite/jupyter-lite.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/jupyterlite.schema.v0.json` & `resotocore-3.6.1/resotocore/jupyterlite/jupyterlite.schema.v0.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/kernelspecs/javascript.svg` & `resotocore-3.6.1/resotocore/jupyterlite/kernelspecs/javascript.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/lab/favicon.ico` & `resotocore-3.6.1/resotocore/jupyterlite/lab/favicon.ico`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/lab/index.html` & `resotocore-3.6.1/resotocore/jupyterlite/lab/index.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/lab/jupyter-lite.ipynb` & `resotocore-3.6.1/resotocore/jupyterlite/lab/jupyter-lite.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/lab/package.json` & `resotocore-3.6.1/resotocore/jupyterlite/lab/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/manifest.webmanifest` & `resotocore-3.6.1/resotocore/jupyterlite/manifest.webmanifest`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/package.json` & `resotocore-3.6.1/resotocore/jupyterlite/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/jupyterlite/service-worker-b2fb40a.js` & `resotocore-3.6.1/resotocore/jupyterlite/service-worker-b2fb40a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/message_bus.py` & `resotocore-3.6.1/resotocore/message_bus.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from contextlib import asynccontextmanager
 from datetime import datetime
 from typing import Any, Optional, Dict, List, AsyncGenerator
 
 from frozendict import frozendict
 from jsons import set_deserializer, set_serializer
 from resotocore.ids import TaskId
+from resotocore.service import Service
 
 from resotocore.types import Json
 from resotocore.util import pop_keys, utc_str, from_utc
 from resotocore.ids import SubscriberId
 from resotolib.core.progress import Progress
 
 log = logging.getLogger(__name__)
@@ -23,14 +24,15 @@
     Connected = "message-listener-connected"
     Disconnected = "message-listener-disconnected"
     ConfigUpdated = "config-updated"
     ConfigCopied = "config-copied"
     ConfigDeleted = "config-deleted"
     ErrorMessage = "error"
     ProgressMessage = "progress"
+    GraphMergeCompleted = "graph-merge-completed"
 
 
 class Message(ABC):
     """
     Json representation of a message is always:
     { "kind": "xxx", "message_type": "yyy", "data": { ... }}
 
@@ -220,15 +222,15 @@
         self.subscriber_id = subscriber_id
         self.error = error
 
     def info(self) -> str:
         return f"Fatal: could not perform action {self.step_name}. Reason: {self.error}"
 
 
-class MessageBus:
+class MessageBus(Service):
     """
     This class implements a simple event bus.
     Every subscriber is context managed and gets its own queue of events.
     """
 
     def __init__(self) -> None:
         # key is the channel name, value is the list of queues
@@ -287,14 +289,18 @@
             self.active_listener.pop(subscriber_id, None)
             await self.emit_event(CoreMessage.Disconnected, {"subscriber_id": subscriber_id, "channels": channels})
 
     async def emit_event(self, event_type: str, data: Json) -> None:
         return await self.emit(Event(event_type, data))
 
     async def emit(self, message: Message) -> None:
+        log.debug(
+            "Emitting message %s: %s", message.message_type, ", ".join(f"{k}={v}" for k, v in message.data.items())
+        )
+
         async def emit_by(name: str) -> None:
             for listener in self.listeners.get(name, []):
                 await listener.put(message)
 
         await emit_by(message.message_type)  # inform specific listener
         await emit_by("*")  # inform "all" event listener
```

### Comparing `resotocore-3.6.0/resotocore/metrics.py` & `resotocore-3.6.1/resotocore/metrics.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import time
 from functools import wraps
 from typing import Callable, Any, TypeVar, cast
 
 from prometheus_client import Histogram, Counter, Gauge
 
 # All exported metrics are listed here
@@ -11,14 +12,16 @@
 RequestLatency = Histogram(f"{Prefix}request_latency_seconds", "Request latency", ["endpoint"])
 RequestInProgress = Gauge(f"{Prefix}requests_in_progress_total", "Requests in progress", ["endpoint", "method"])
 
 # Create a type that is bound to the underlying wrapped function
 # This way all signature information is preserved!
 DecoratedFn = TypeVar("DecoratedFn", bound=Callable[..., Any])
 
+log = logging.getLogger(__name__)
+
 
 def perf_now() -> float:
     return time.perf_counter()
 
 
 def timed(module: str, name: str, is_async: bool = True) -> Callable[[DecoratedFn], DecoratedFn]:
     """
@@ -34,24 +37,28 @@
         @wraps(fn)
         def async_time_decorated(*args: Any, **kwargs: Any) -> Any:
             start_time = perf_now()
             try:
                 rv = fn(*args, **kwargs)
                 return rv
             finally:
-                metric.observe(perf_now() - start_time)
+                duration = perf_now() - start_time
+                log.debug(f"Duration of {module}::{name}: {duration}")
+                metric.observe(duration)
 
         return cast(DecoratedFn, async_time_decorated)
 
     def async_time_wrapper(fn: DecoratedFn) -> DecoratedFn:
         @wraps(fn)
         async def async_time_decorated(*args: Any, **kwargs: Any) -> Any:
             start_time = perf_now()
             try:
                 rv = await fn(*args, **kwargs)
                 return rv
             finally:
-                metric.observe(perf_now() - start_time)
+                duration = round((perf_now() - start_time) * 1000)
+                log.debug(f"Duration of {module}::{name}: {duration} millis")
+                metric.observe(duration)
 
         return cast(DecoratedFn, async_time_decorated)
 
     return async_time_wrapper if is_async else sync_time_wrapper
```

### Comparing `resotocore-3.6.0/resotocore/model/adjust_node.py` & `resotocore-3.6.1/resotocore/model/adjust_node.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/model/db_updater.py` & `resotocore-3.6.1/resotocore/model/db_updater.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,73 @@
 from __future__ import annotations
+
 import asyncio
 import json
 import logging
+import shutil
+import tempfile
 from abc import ABC
-from asyncio import Task
+from asyncio import Task, CancelledError
+from collections import defaultdict
 from contextlib import suppress
-from attrs import define
-from datetime import timedelta
+from datetime import timedelta, datetime
 from multiprocessing import Process, Queue
+from pathlib import Path
 from queue import Empty
-from typing import Optional, Union, AsyncGenerator, Any, Generator, List
+from typing import Optional, Union, Any, Generator, List, AsyncIterator, Dict
 
+import aiofiles
 from aiostream import stream
 from aiostream.core import Stream
+from attrs import define
 
 from resotocore.analytics import AnalyticsEventSender, InMemoryEventSender, AnalyticsEvent
 from resotocore.async_extensions import run_async
 from resotocore.core_config import CoreConfig
 from resotocore.db.db_access import DbAccess
+from resotocore.db.deferred_edge_db import PendingDeferredEdges
 from resotocore.db.graphdb import GraphDB
 from resotocore.db.model import GraphUpdate
-from resotocore.db.deferred_edge_db import PendingDeferredEdges
-from resotocore.dependencies import db_access, setup_process, reset_process_start_method
 from resotocore.error import ImportAborted
+from resotocore.ids import TaskId, GraphName
+from resotocore.message_bus import MessageBus, CoreMessage
 from resotocore.model.graph_access import GraphBuilder
-from resotocore.model.model import Model
 from resotocore.model.model_handler import ModelHandlerDB, ModelHandler
+from resotocore.service import Service
+from resotocore.system_start import db_access, setup_process, reset_process_start_method
 from resotocore.types import Json
-from resotocore.ids import TaskId, GraphName
 from resotocore.util import utc, uuid_str, shutdown_process
 
 log = logging.getLogger(__name__)
 
 
 class ProcessAction(ABC):
     """
     Base class to exchange commands between processes.
     Important: all messages must be serializable in order to get pickled/unpickled.
     """
 
 
 @define
+class ReadFile(ProcessAction):
+    """
+    Read a file from disk.
+    """
+
+    path: Path
+    task_id: Optional[str]
+
+    def jsons(self) -> Generator[Json, Any, None]:
+        with open(self.path, "r", encoding="utf-8") as f:
+            for line in f:
+                if line.strip():
+                    yield json.loads(line)
+
+
+@define
 class ReadElement(ProcessAction):
     """
     Read an incoming element:
     - either a line of text or
     - a complete json element
     Parent -> Child: for every incoming data line.
     """
@@ -112,48 +135,63 @@
     Once the MergeGraph action is received, the graph gets imported.
     From here the parent expects result messages from the child.
     All events happen in the child are forwarded to the parent via EmitEvent.
     Once the graph update is done, a result is send.
     The result is either an exception in case of failure or a graph update in success case.
     """
 
-    def __init__(self, read_queue: Queue[ProcessAction], write_queue: Queue[ProcessAction], config: CoreConfig) -> None:
+    def __init__(
+        self,
+        read_queue: Queue[ProcessAction],
+        write_queue: Queue[ProcessAction],
+        config: CoreConfig,
+        graph_name: GraphName,
+        change_id: str,
+    ) -> None:
         super().__init__(name="merge_update")
         self.read_queue = read_queue
         self.write_queue = write_queue
         self.config = config
+        self.change_id = change_id
+        self.graph_name = graph_name
 
     def next_action(self) -> ProcessAction:
         try:
             # graph is read into memory. If the sender does not send data in a given amount of time,
             # we raise an exception and abort the update.
             return self.read_queue.get(True, 90)
         except Empty as ex:
             raise ImportAborted("Merge process did not receive any data for more than 90 seconds. Abort.") from ex
 
     async def merge_graph(self, db: DbAccess) -> GraphUpdate:  # type: ignore
-        model = Model.from_kinds([kind async for kind in db.model_db.all()])
-        builder = GraphBuilder(model)
+        model_handler = ModelHandlerDB(db)
+        model = await model_handler.load_model(self.graph_name)
+        builder = GraphBuilder(model, self.change_id)
         nxt = self.next_action()
-        while isinstance(nxt, ReadElement):
+        if isinstance(nxt, ReadFile):
             for element in nxt.jsons():
                 builder.add_from_json(element)
-            log.debug(f"Read {int(BatchSize / 1000)}K elements in process")
             nxt = self.next_action()
+        elif isinstance(nxt, ReadElement):
+            while isinstance(nxt, ReadElement):
+                for element in nxt.jsons():
+                    builder.add_from_json(element)
+                log.debug(f"Read {int(BatchSize / 1000)}K elements in process")
+                nxt = self.next_action()
         if isinstance(nxt, PoisonPill):
             log.debug("Got poison pill - going to die.")
             shutdown_process(0)
         elif isinstance(nxt, MergeGraph):
             log.debug("Graph read into memory")
             builder.check_complete()
             graphdb = db.get_graph_db(nxt.graph)
             outer_edge_db = db.pending_deferred_edge_db
+            await graphdb.insert_usage_data(builder.usage)
             _, result = await graphdb.merge_graph(builder.graph, model, nxt.change_id, nxt.is_batch)
             # sizes of model entries have been adjusted during the merge. Update the model in the db.
-            model_handler = ModelHandlerDB(db, "")
             await model_handler.update_model(graphdb.name, list(model.kinds.values()))
             if nxt.task_id and builder.deferred_edges:
                 await outer_edge_db.update(PendingDeferredEdges(nxt.task_id, utc(), nxt.graph, builder.deferred_edges))
                 log.debug(f"Updated {len(builder.deferred_edges)} pending outer edges for collect task {nxt.task_id}")
             return result
 
     async def setup_and_merge(self) -> GraphUpdate:
@@ -177,92 +215,195 @@
         except Exception as ex:
             # not all exceptions can be pickled. Use string representation.
             self.write_queue.put(Result(repr(ex)))
             log.error(f"Update process interrupted. Preemptive Exit. {ex}", exc_info=ex)
             shutdown_process(1)
 
 
-async def merge_graph_process(
-    db: GraphDB,
-    model_handler: ModelHandler,
-    event_sender: AnalyticsEventSender,
-    config: CoreConfig,
-    content: AsyncGenerator[Union[bytes, Json], None],
-    max_wait: timedelta,
-    maybe_batch: Optional[str],
-    task_id: Optional[TaskId],
-) -> GraphUpdate:
-    change_id = maybe_batch if maybe_batch else uuid_str()
-    write: Queue[ProcessAction] = Queue()
-    read: Queue[ProcessAction] = Queue()
-    updater = DbUpdaterProcess(write, read, config)  # the process reads from our write queue and vice versa
-    stale = timedelta(seconds=5).total_seconds()  # consider dead communication after this amount of time
-    deadline = utc() + max_wait
-    dead_adjusted = False
-
-    async def send_to_child(pa: ProcessAction) -> bool:
-        alive = updater.is_alive()
-        if alive:
-            await run_async(write.put, pa, True, stale)
-        return alive
-
-    def read_results() -> Task[GraphUpdate]:
-        async def read_forever() -> GraphUpdate:
-            nonlocal deadline
-            nonlocal dead_adjusted
-            while utc() < deadline:
-                # After exit of updater: adjust the deadline once
-                if not updater.is_alive() and not dead_adjusted:
-                    log.debug("Import process done or dead. Adjust deadline.")
-                    deadline = utc() + timedelta(seconds=30)
-                    dead_adjusted = True
-                try:
-                    action = await run_async(read.get, True, stale)
-                    if isinstance(action, EmitAnalyticsEvent):
-                        await event_sender.capture([action.event])
-                    elif isinstance(action, Result):
-                        return action.get_value()
-                except Empty:
-                    # empty is fine
-                    pass
-            raise ImportAborted(f"Import process died. (ExitCode: {updater.exitcode})")
-
-        return asyncio.create_task(read_forever())
-
-    task: Optional[Task[GraphUpdate]] = None
-    result: Optional[GraphUpdate] = None
-    try:
-        reset_process_start_method()  # other libraries might have tampered the value in the mean time
-        updater.start()
-        task = read_results()  # concurrently read result queue
-        chunked: Stream = stream.chunks(content, BatchSize)
-        async with chunked.stream() as streamer:
-            async for lines in streamer:
-                if not await send_to_child(ReadElement(lines, task_id)):
-                    # in case the child is dead, we should stop
-                    break
-        await send_to_child(MergeGraph(db.name, change_id, maybe_batch is not None, task_id))
-        result = await task  # wait for final result
-        await model_handler.load_model(db.name, force=True)  # reload model to get the latest changes
-        return result
-    finally:
-        if task is not None and not task.done():
-            task.cancel()
-        if not result:
-            # make sure the change is aborted in case of transaction
-            log.info(f"Abort update manually: {change_id}")
-            await db.abort_update(change_id)
-        await send_to_child(PoisonPill())
-        await run_async(updater.join, stale)
-        if updater.is_alive():
-            log.warning(f"Process is still alive after poison pill. Terminate process {updater.pid}")
-            with suppress(Exception):
-                updater.terminate()
-            await asyncio.sleep(3)
-        if updater.is_alive():
-            log.warning(f"Process is still alive after terminate. Kill process {updater.pid}")
-            with suppress(Exception):
-                updater.kill()
-            await run_async(updater.join)
-        if not updater.is_alive():
+@define
+class GraphUpdateTask:
+    """
+    This class represents a graph update task that is queued for processing.
+    The update is written to a temporary file.
+    """
+
+    db: GraphDB
+    path: Path
+    deadline: datetime
+    maybe_batch: Optional[str]
+    task_id: Optional[TaskId]
+
+    def cleanup(self) -> None:
+        shutil.rmtree(self.path.parent)
+
+
+class GraphMerger(Service):
+    def __init__(
+        self,
+        model_handler: ModelHandler,
+        event_sender: AnalyticsEventSender,
+        config: CoreConfig,
+        message_bus: MessageBus,
+    ) -> None:
+        self.model_handler = model_handler
+        self.event_sender = event_sender
+        self.config = config
+        self.message_bus = message_bus
+        self.run_lock = asyncio.Lock()
+        self.running_imports: Dict[TaskId, int] = defaultdict(int)
+        self.update_queue: asyncio.Queue[GraphUpdateTask] = asyncio.Queue()
+        self.concurrent_updates = asyncio.Semaphore(self.config.graph_update.parallel_imports)
+        self.handler_task: Optional[Task[Any]] = None
+
+    async def __process_item(self, item: GraphUpdateTask) -> Union[GraphUpdate, Exception]:
+        log.info(f"Start processing graph merge from queue: {item}")
+        try:
+            return await self.__merge_graph_process(item.db, item.path, item.deadline, item.maybe_batch, item.task_id)
+        except Exception as ex:
+            log.error(f"Failed to process graph merge: {item}", exc_info=ex)
+            return ex
+        finally:
+            item.cleanup()
+
+    async def start(self) -> None:
+        async def wait_for_update() -> None:
+            log.info("Start waiting for graph updates")
+            cl = stream.cycle(stream.call(self.update_queue.get))
+            fl = stream.map(cl, self.__process_item, task_limit=self.config.graph_update.parallel_imports)
+            with suppress(CancelledError):
+                async with fl.stream() as streamer:
+                    async for update in streamer:
+                        if isinstance(update, GraphUpdate):
+                            log.info(f"Finished spawned graph merge: {update}")
+
+        self.handler_task = asyncio.create_task(wait_for_update())
+
+    async def stop(self) -> None:
+        if self.handler_task:
+            self.handler_task.cancel()
             with suppress(Exception):
-                updater.close()
+                await self.handler_task
+        # cleanup all queued entries
+        while not self.update_queue.empty():
+            self.update_queue.get_nowait().cleanup()
+
+    async def merge_graph(
+        self,
+        db: GraphDB,
+        content: AsyncIterator[Union[bytes, Json]],
+        max_wait: timedelta,
+        maybe_batch: Optional[str],
+        task_id: Optional[TaskId],
+        wait_for_result: bool = False,
+    ) -> Optional[GraphUpdate]:
+        # increment count
+        if task_id:
+            async with self.run_lock:
+                self.running_imports[task_id] += 1
+
+        deadline = utc() + max_wait
+        if wait_for_result:
+            return await self.__merge_graph_process(db, content, deadline, maybe_batch, task_id)
+        else:
+            td = Path(tempfile.mkdtemp()) / "graph"
+            log.debug(f"Do not merge directly. Write to temp file: {td}")
+            async with aiofiles.open(td, "wb") as f:
+                async for line in content:
+                    await f.write(line if isinstance(line, bytes) else (json.dumps(line) + "\n").encode("utf-8"))
+            await self.update_queue.put(GraphUpdateTask(db, td, deadline, maybe_batch, task_id))
+            log.debug("GraphMerge operation queued.")
+            return None
+
+    async def __merge_graph_process(
+        self,
+        db: GraphDB,
+        content: Union[AsyncIterator[Union[bytes, Json]], Path],
+        deadline: datetime,
+        maybe_batch: Optional[str],
+        task_id: Optional[TaskId],
+    ) -> GraphUpdate:
+        async with self.concurrent_updates:
+            change_id = maybe_batch if maybe_batch else uuid_str()
+            write: Queue[ProcessAction] = Queue()
+            read: Queue[ProcessAction] = Queue()
+            updater = DbUpdaterProcess(write, read, self.config, db.name, change_id)  # the process communication queue
+            stale = timedelta(seconds=5).total_seconds()  # consider dead communication after this amount of time
+            dead_adjusted = False
+
+            async def send_to_child(pa: ProcessAction) -> bool:
+                alive = updater.is_alive()
+                if alive:
+                    await run_async(write.put, pa, True, stale)
+                return alive
+
+            def read_results() -> Task[GraphUpdate]:
+                async def read_forever() -> GraphUpdate:
+                    nonlocal deadline
+                    nonlocal dead_adjusted
+                    while utc() < deadline:
+                        # After exit of updater: adjust the deadline once
+                        if not updater.is_alive() and not dead_adjusted:
+                            log.debug("Import process done or dead. Adjust deadline.")
+                            deadline = utc() + timedelta(seconds=30)
+                            dead_adjusted = True
+                        try:
+                            action = await run_async(read.get, True, stale)
+                            if isinstance(action, EmitAnalyticsEvent):
+                                await self.event_sender.capture([action.event])
+                            elif isinstance(action, Result):
+                                return action.get_value()
+                        except Empty:
+                            # empty is fine
+                            pass
+                    raise ImportAborted(f"Import process died or deadline exceeded. (ExitCode: {updater.exitcode})")
+
+                return asyncio.create_task(read_forever())
+
+            task: Optional[Task[GraphUpdate]] = None
+            result: Optional[GraphUpdate] = None
+            try:
+                reset_process_start_method()  # other libraries might have tampered the value in the mean time
+                updater.start()
+                task = read_results()  # concurrently read result queue
+                # Either send a file or stream the content directly
+                if isinstance(content, Path):
+                    await send_to_child(ReadFile(content, task_id))
+                else:
+                    chunked: Stream = stream.chunks(content, BatchSize)
+                    async with chunked.stream() as streamer:
+                        async for lines in streamer:
+                            if not await send_to_child(ReadElement(lines, task_id)):
+                                # in case the child is dead, we should stop
+                                break
+                await send_to_child(MergeGraph(db.name, change_id, maybe_batch is not None, task_id))
+                result = await task  # wait for final result
+                await self.model_handler.load_model(db.name, force=True)  # reload model to get the latest changes
+                return result
+            finally:
+                # update running imports and send event if completed
+                if task_id:
+                    async with self.run_lock:
+                        self.running_imports[task_id] -= 1
+                        if self.running_imports[task_id] == 0:
+                            del self.running_imports[task_id]
+                            await self.message_bus.emit_event(CoreMessage.GraphMergeCompleted, dict(task_id=task_id))
+                if task is not None and not task.done():
+                    task.cancel()
+                if not result:
+                    # make sure the change is aborted in case of transaction
+                    log.info(f"Abort update manually: {change_id}")
+                    await db.abort_update(change_id)
+                await send_to_child(PoisonPill())
+                await run_async(updater.join, stale)
+                if updater.is_alive():
+                    log.warning(f"Process is still alive after poison pill. Terminate process {updater.pid}")
+                    with suppress(Exception):
+                        updater.terminate()
+                    await asyncio.sleep(3)
+                if updater.is_alive():
+                    log.warning(f"Process is still alive after terminate. Kill process {updater.pid}")
+                    with suppress(Exception):
+                        updater.kill()
+                    await run_async(updater.join)
+                if not updater.is_alive():
+                    with suppress(Exception):
+                        updater.close()
```

### Comparing `resotocore-3.6.0/resotocore/model/graph_access.py` & `resotocore-3.6.1/resotocore/model/graph_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     DateTimeKind,
     DictionaryKind,
     StringKind,
     Property,
     SimpleKind,
     DateKind,
     DurationKind,
+    UsageDatapoint,
+    UsageMetricValues,
 )
 from resotocore.model.resolve_in_graph import GraphResolver, NodePath, ResolveProp
 from resotocore.model.typed_model import from_js
 from resotocore.types import Json, EdgeType, JsonElement
 from resotocore.util import utc, utc_str, value_in_path, set_value_in_path, value_in_path_get
 
 log = logging.getLogger(__name__)
@@ -63,20 +65,23 @@
     # All resolved ancestors are written to this section.
     ancestors = "ancestors"
 
     # Resolved descendants would be written to this section.
     # Only here for completeness - currently not used.
     descendants = "descendants"
 
+    # Usage of the resource
+    usage = "usage"
+
     # The set of all content sections
     content_ordered = [reported, desired, metadata]
     content = set(content_ordered)
 
     # The list of all lookup sections
-    lookup_sections_ordered = [ancestors, descendants]
+    lookup_sections_ordered = [ancestors, descendants, usage]
 
     # The list of all sections
     all_ordered = [*content_ordered, *lookup_sections_ordered]
     all = set(all_ordered)
 
     # remove the section plus dot if it exists in the string: reported.foo => foo
     __no_section = re.compile("^/?(" + "|".join(f"({s})" for s in content_ordered) + ")[.]")
@@ -133,31 +138,53 @@
 class DeferredEdge:
     from_node: NodeSelector
     to_node: NodeSelector
     edge_type: str
 
 
 class GraphBuilder:
-    def __init__(self, model: Model):
+    def __init__(self, model: Model, change_id: str):
         self.model = model
         self.graph = MultiDiGraph()
         self.nodes = 0
         self.edges = 0
         self.deferred_edges: List[DeferredEdge] = []
+        self.usage: List[UsageDatapoint] = []
+        self.at = int(utc().timestamp())
+        self.change_id = change_id
 
     def add_from_json(self, js: Json) -> None:
         if "id" in js and Section.reported in js:
+            usage_json = js.get(Section.usage, {})
+            if len(usage_json) == 0:
+                usage_json = None
             self.add_node(
-                js["id"],
-                js[Section.reported],
-                js.get(Section.desired, None),
-                js.get(Section.metadata, None),
-                js.get("search", None),
-                js.get("replace", False) is True,
+                node_id=js["id"],
+                reported=js[Section.reported],
+                desired=js.get(Section.desired, None),
+                metadata=js.get(Section.metadata, None),
+                search=js.get("search", None),
+                replace=js.get("replace", False) is True,
             )
+            if usage_json:
+                values = {
+                    k: UsageMetricValues(
+                        min=v.get("min", v["avg"]),
+                        avg=v["avg"],
+                        max=v.get("max", v["avg"]),
+                    )
+                    for k, v in usage_json.items()
+                }
+                usage = UsageDatapoint(
+                    id=js["id"],
+                    change_id=self.change_id,
+                    at=self.at,
+                    v=values,
+                )
+                self.usage.append(usage)
         elif "from" in js and "to" in js:
             self.add_edge(js["from"], js["to"], js.get("edge_type", EdgeTypes.default))
         elif "from_selector" in js and "to_selector" in js:
 
             def parse_selector(js: Json) -> NodeSelector:
                 if "node_id" in js:
                     return ByNodeId(NodeId(from_js(js["node_id"], str)))
```

### Comparing `resotocore-3.6.0/resotocore/model/json_schema.py` & `resotocore-3.6.1/resotocore/model/json_schema.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/model/model.py` & `resotocore-3.6.1/resotocore/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,33 @@
 import re
 import sys
 import textwrap
 from abc import ABC, abstractmethod
 from datetime import datetime, timezone, date
 from functools import lru_cache
 from json import JSONDecodeError
-from typing import Union, Any, Optional, Callable, Type, Sequence, Dict, List, Set, cast, Tuple, Iterable, TypeVar
+from typing import (
+    Union,
+    Any,
+    Optional,
+    Callable,
+    Type,
+    Sequence,
+    Dict,
+    List,
+    Set,
+    cast,
+    Tuple,
+    Iterable,
+    TypeVar,
+    NamedTuple,
+)
 
 import yaml
-from attrs import define
+from attrs import define, frozen
 from dateutil.parser import parse
 from jsons import set_deserializer, set_serializer
 from networkx import MultiDiGraph
 from parsy import regex, string, Parser
 
 from resotocore.compat import remove_suffix
 from resotocore.model.transform_kind_convert import converters
@@ -1198,14 +1213,15 @@
             Property("last_access", "trafo.duration_to_datetime", False, SyntheticProperty(["atime"])),
             # Resource tags might define expiration time. Translate durations to absolute times.
             Property("expires", "datetime", False, None, "datetime when the node expires."),
             # Account defines the time when the data was collected in the metadata section
             Property("exported_at", "datetime", False, None, "datetime when the account was exported."),
             Property("exported_age", "trafo.duration_to_datetime", False, SyntheticProperty(["exported_at"])),
         ],
+        metadata={"dynamic": True},
     ),
 ]
 predefined_kinds_by_name = {k.fqn: k for k in predefined_kinds}
 
 allowed_simple_type_changes: List[Tuple[Optional[str], Optional[str]]] = [
     ("string", "duration"),
     ("string", "date"),
@@ -1440,10 +1456,39 @@
                     )
                 )
             else:
                 result.append(kind)
         return result
 
 
+class UsageMetricValues(NamedTuple):
+    min: float
+    avg: float
+    max: float
+
+
+@frozen
+class UsageDatapoint:
+    """
+    A single datapoint of resource usage.
+
+    id: `str`
+        Identifier of the resource as named by the cloud.
+    at: `int`
+        Timestamp of the datapoint in seconds since epoch.
+        Name of the metric.
+    change_id: `str`
+        Id of the import
+    v: `Dict[str, List[float]]]`
+        Dictionary of metric names to lists of values. The values are `min`, `avg` and `max`.
+
+    """
+
+    id: str
+    at: int
+    change_id: str
+    v: Dict[str, UsageMetricValues]
+
+
 # register serializer for this class
 set_deserializer(Kind.from_json, Kind)
 set_serializer(SimpleKind.to_json, SimpleKind)
```

### Comparing `resotocore-3.6.0/resotocore/model/model_handler.py` & `resotocore-3.6.1/resotocore/model/model_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from plantuml import PlantUML
 
 from resotocore.async_extensions import run_async
 from resotocore.db.db_access import DbAccess
 from resotocore.ids import GraphName
 from resotocore.model.model import Model, Kind, ComplexKind, Property
+from resotocore.service import Service
 from resotocore.types import EdgeType
 from resotocore.util import exist
 
 log = logging.getLogger(__name__)
 
 
 class ModelHandler(ABC):
@@ -86,33 +87,27 @@
     "skinparam RoundCorner 5\n"
     "skinparam Shadowing false\n"
     "skinparam stereotypeCBackgroundColor #e98df7\n"
     "skinparam stereotypeIBackgroundColor #e98df7\n"
 )
 
 
-class ModelHandlerDB(ModelHandler):
-    def __init__(self, db_access: DbAccess, plantuml_server: str):
+class ModelHandlerDB(ModelHandler, Service):
+    def __init__(self, db_access: DbAccess, plantuml_server: str = "https://plantuml.resoto.org"):
         self.db_access = db_access
         self.plantuml_server = plantuml_server
         self.__loaded_model: Dict[GraphName, Model] = {}
         self.default_legacy_graph_name = GraphName("resoto")
 
     async def load_model(self, graph_name: GraphName, *, force: bool = False) -> Model:
         if not force and (model := self.__loaded_model.get(graph_name)) is not None:
             return model
         else:
             graph_model_db = await self.db_access.get_graph_model_db(graph_name)
-            model_db = self.db_access.get_model_db()
-            # check the new implementation for the kinds
-            model_kinds = [kind async for kind in graph_model_db.all()]
-            # if nothing found and the graph is the legacy default one, look in the legacy implementation
-            if not model_kinds and graph_name == self.default_legacy_graph_name:
-                model_kinds = [kind async for kind in model_db.all()]
-            model = Model.from_kinds(model_kinds)
+            model = Model.from_kinds([kind async for kind in graph_model_db.all()])
             self.__loaded_model[graph_name] = model
             return model
 
     async def uml_image(
         self,
         graph_name: GraphName,
         output: str = "svg",
@@ -233,12 +228,10 @@
         # load existing model
         model = await self.load_model(graph_name)
         # make sure the update is valid
         updated = model.update_kinds(kinds)
         # store all updated kinds
         db = await self.db_access.get_graph_model_db(graph_name)
         await db.update_many(kinds)
-        if graph_name == self.default_legacy_graph_name:
-            await self.db_access.get_model_db().update_many(kinds)
         # unset loaded model
         self.__loaded_model[graph_name] = updated
         return updated
```

### Comparing `resotocore-3.6.0/resotocore/model/resolve_in_graph.py` & `resotocore-3.6.1/resotocore/model/resolve_in_graph.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/model/transform_kind_convert.py` & `resotocore-3.6.1/resotocore/model/transform_kind_convert.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/model/typed_model.py` & `resotocore-3.6.1/resotocore/model/typed_model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/query/__init__.py` & `resotocore-3.6.1/resotocore/query/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/query/model.py` & `resotocore-3.6.1/resotocore/query/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 
 import abc
 from collections import defaultdict
+from datetime import datetime, timedelta
+
 from attrs import define, field, evolve
 from functools import reduce, partial, cached_property
 from itertools import chain
 from typing import Mapping, Union, Optional, Any, ClassVar, Dict, List, Tuple, Callable, Set, Iterable
 
 from jsons import set_deserializer
 
 from resotocore.model.graph_access import EdgeTypes, Direction
 from resotocore.model.resolve_in_graph import GraphResolver
 from resotocore.model.typed_model import to_js_str
 from resotocore.types import Json, JsonElement, EdgeType
-from resotocore.util import combine_optional
+from resotocore.util import combine_optional, utc_str, utc
+from resotolib.durations import duration_str
 
 PathRoot = "/"
 
 
 def variable_to_absolute(section: Optional[str], name: str) -> str:
     if name.startswith(PathRoot):
         return name[1:]
@@ -205,14 +208,18 @@
         if op == "or":
             return self.or_term(other)
         elif op == "and":
             return self.and_term(other)
         else:
             raise AttributeError(f"Don't know how to combine with {op}")
 
+    @property
+    def is_all(self) -> bool:
+        return isinstance(self, AllTerm)
+
     def or_term(self, other: Term) -> Term:
         if isinstance(self, AllTerm):  # all or x == all
             return self
         elif isinstance(other, AllTerm):  # x or all == all
             return other
         elif isinstance(self, MergeTerm):  # combining a merge term needs special handling
             return self.or_merge_term(other)
@@ -296,14 +303,61 @@
             return result
         else:
             return []
 
     def contains_term_type(self, clazz: type) -> bool:
         return self.find_term(lambda x: isinstance(x, clazz)) is not None
 
+    def split_term_by(self, check_fn: Callable[[Term], bool]) -> Tuple[Term, Term]:
+        before_merge: Term = AllTerm()
+        after_merge: Term = AllTerm()
+
+        def walk_term(term: Term) -> None:
+            # precondition: this method is only called with a term that has ancestor/descendant
+            nonlocal before_merge
+            nonlocal after_merge
+            if isinstance(term, CombinedTerm):
+                left_has_ad = check_fn(term.left)
+                right_has_ad = check_fn(term.right)
+                if term.op == "or":
+                    after_merge = after_merge & term
+                elif left_has_ad and right_has_ad:
+                    walk_term(term.left)
+                    walk_term(term.right)
+                elif left_has_ad:
+                    before_merge = before_merge & term.right
+                    walk_term(term.left)
+                elif right_has_ad:
+                    before_merge = before_merge & term.left
+                    walk_term(term.right)
+                else:
+                    raise NotImplementedError("Logic unsound. This case should not happen!")
+            elif isinstance(term, MergeTerm):
+                # in case pre- and post- filter are defined, handle it as AND combined term
+                # background: pre- and post- filter will be applied on the result
+                #             that effectively reflects an and combination.
+                #             The merge part only merges data to the existing values.
+                if term.post_filter:
+                    walk_term(CombinedTerm(term.pre_filter, "and", term.post_filter))
+                else:
+                    walk_term(term.pre_filter)
+            else:
+                after_merge = after_merge & term
+
+        if check_fn(self):
+            walk_term(self)
+            return before_merge, after_merge
+        else:
+            return self, AllTerm()
+
+    def split_by_usage(self) -> Tuple[Term, Term]:
+        return self.split_term_by(
+            lambda x: x.find_term(lambda t: isinstance(t, Predicate) and t.name.startswith("usage")) is not None
+        )
+
     # noinspection PyUnusedLocal
     @staticmethod
     def from_json(js: Dict[str, Any], _: type = object, **kwargs: Any) -> Term:
         if isinstance(js.get("left"), dict) and isinstance(js.get("right"), dict) and isinstance(js.get("op"), str):
             left = Term.from_json(js["left"])
             right = Term.from_json(js["right"])
             return CombinedTerm(left, js["op"], right)
@@ -555,41 +609,66 @@
     def __str__(self) -> str:
         term = " " + str(self.term) if self.term else ""
         with_clause = " " + str(self.with_clause) if self.with_clause else ""
         return f"with({self.with_filter}, {self.navigation}{term}{with_clause})"
 
 
 @define(order=True, hash=True, frozen=True)
+class WithUsage:
+    start: Union[datetime, timedelta]
+    end: Union[datetime, timedelta, None]
+    metrics: List[str]
+
+    def __str__(self) -> str:
+        def dd_str(d: Union[datetime, timedelta]) -> str:
+            return duration_str(d) if isinstance(d, timedelta) else utc_str(d)
+
+        end = f"::{dd_str(self.end)}" if self.end else ""
+        return f'with_usage({dd_str(self.start)}{end}, [{",".join(self.metrics)}])'
+
+    def start_from_now(self) -> datetime:
+        return self.start if isinstance(self.start, datetime) else utc() - self.start
+
+    def end_from_now(self) -> datetime:
+        if self.end:
+            return self.end if isinstance(self.end, datetime) else utc() - self.end
+        else:
+            return utc()
+
+
+@define(order=True, hash=True, frozen=True)
 class Limit:
     offset: int
     length: int
 
     def __str__(self) -> str:
         return f" limit {self.length}" if self.offset == 0 else f" limit {self.offset}, {self.length}"
 
 
 # pylint: disable=not-an-iterable
 @define(order=True, hash=True, frozen=True)
 class Part:
     term: Term
     tag: Optional[str] = None
     with_clause: Optional[WithClause] = None
+    with_usage: Optional[WithUsage] = None
     sort: List[Sort] = field(factory=list)
     limit: Optional[Limit] = None
     navigation: Optional[Navigation] = None
     reverse_result: bool = False
 
     def __str__(self) -> str:
+        with_usage = f"{self.with_usage} " if self.with_usage is not None else ""
         with_clause = f" {self.with_clause}" if self.with_clause is not None else ""
         tag = f"#{self.tag}" if self.tag else ""
         sort = " sort " + (", ".join(f"{a.name} {a.order}" for a in self.sort)) if self.sort else ""
         limit = str(self.limit) if self.limit else ""
         nav = f" {self.navigation}" if self.navigation is not None else ""
         reverse = " reversed " if self.reverse_result else ""
-        return f"{self.term}{with_clause}{tag}{sort}{limit}{reverse}{nav}"
+        return f"{with_usage}{self.term}{with_clause}{tag}{sort}{limit}{reverse}{nav}"
 
     def change_variable(self, fn: Callable[[str], str]) -> Part:
         return evolve(
             self,
             term=self.term.change_variable(fn),
             with_clause=self.with_clause.change_variable(fn) if self.with_clause else None,
             sort=[sort.change_variable(fn) for sort in self.sort],
@@ -634,57 +713,24 @@
         The query is rewritten in order to create a prefilter with all terms that do not depend on the merge.
         A MergeTerm is either created if not existent or the existing one will be extended with all merge query
         additions. All merge relevant parts will be performed as merge term post filter.
         Even if the query is rewritten, the logic of the query is not changed and stays the same.
 
         :return: the rewritten part with resolved merge parts if ancestor or descendant predicates are found.
         """
-        before_merge: Term = AllTerm()
-        after_merge: Term = AllTerm()
 
         def has_ancestor_descendant(t: Term) -> bool:
             return t.find_term(lambda trm: isinstance(trm, Predicate) and is_ancestor_descendant(trm.name)) is not None
 
         def ancestor_descendant_predicates(t: Term) -> List[Predicate]:
             return t.find_terms(lambda t: isinstance(t, Predicate) and is_ancestor_descendant(t.name), in_context_term=False)  # type: ignore # noqa: E501
 
-        def walk_term(term: Term) -> None:
-            # precondition: this method is only called with a term that has ancestor/descendant
-            nonlocal before_merge
-            nonlocal after_merge
-            if isinstance(term, CombinedTerm):
-                left_has_ad = has_ancestor_descendant(term.left)
-                right_has_ad = has_ancestor_descendant(term.right)
-                if term.op == "or":
-                    after_merge = after_merge & term
-                elif left_has_ad and right_has_ad:
-                    walk_term(term.left)
-                    walk_term(term.right)
-                elif left_has_ad:
-                    before_merge = before_merge & term.right
-                    walk_term(term.left)
-                elif right_has_ad:
-                    before_merge = before_merge & term.left
-                    walk_term(term.right)
-                else:
-                    raise NotImplementedError("Logic unsound. This case should not happen!")
-            elif isinstance(term, MergeTerm):
-                # in case pre- and post- filter are defined, handle it as AND combined term
-                # background: pre- and post- filter will be applied on the result
-                #             that effectively reflects an and combination.
-                #             The merge part only merges data to the existing values.
-                if term.post_filter:
-                    walk_term(CombinedTerm(term.pre_filter, "and", term.post_filter))
-                else:
-                    walk_term(term.pre_filter)
-            else:
-                after_merge = after_merge & term
-
         if has_ancestor_descendant(self.term):
-            walk_term(self.term)
+            # create a filter term that is independent of the merge and execute it before the merge
+            before_merge, after_merge = self.term.split_term_by(has_ancestor_descendant)
             # Create a dict here instead of a set only to ensure ordering (dict remembers order, set is not)'b
             queries = self.merge_queries_for({p.name: 1 for p in ancestor_descendant_predicates(after_merge)})
             return evolve(self, term=MergeTerm(before_merge, queries, after_merge))
         else:
             return self
 
     @property
@@ -1000,17 +1046,18 @@
             if left_last.with_clause and right_first.with_clause:
                 raise AttributeError("Can not combine 2 with clauses!")
             term = left_last.term & right_first.term
             if left_last.tag and right_first.tag:
                 raise AttributeError("Can not combine 2 tag clauses!")
             tag = left_last.tag if left_last.tag else right_first.tag
             with_clause = left_last.with_clause if left_last.with_clause else right_first.with_clause
+            with_usage = left_last.with_usage if left_last.with_usage else right_first.with_usage
             sort = combine_optional(left_last.sort, right_first.sort, lambda m, r: m + r)
             limit = combine_optional(left_last.limit, right_first.limit, combine_limit)
-            combined = Part(term, tag, with_clause, sort if sort else [], limit, right_first.navigation)
+            combined = Part(term, tag, with_clause, with_usage, sort if sort else [], limit, right_first.navigation)
             parts = [*other.parts[0:-1], combined, *self.parts[1:]]
         return Query(parts, preamble, aggregate)
 
     @property
     def visible_predicates(self) -> List[Predicate]:
         """
         Returns a list of all predicates in this query.
```

### Comparing `resotocore-3.6.0/resotocore/query/query_parser.py` & `resotocore-3.6.1/resotocore/query/query_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import timedelta
 from functools import reduce
 from typing import List
 
 import parsy
 from attrs import evolve
 from parsy import string, Parser, regex
 
@@ -28,16 +29,18 @@
     AggregateVariableCombined,
     NotTerm,
     MergeTerm,
     MergeQuery,
     FulltextTerm,
     Limit,
     ContextTerm,
+    WithUsage,
 )
 from resotocore.types import EdgeType
+from resotolib.durations import duration_parser
 from resotolib.parse_util import (
     lparen_p,
     lexeme,
     rparen_p,
     l_bracket_p,
     r_bracket_p,
     colon_p,
@@ -67,14 +70,15 @@
     json_object_p,
     true_dp,
     false_dp,
     null_dp,
     double_quoted_string_dp,
     float_dp,
     dot_p,
+    iso_date_time_utc_parser,
 )
 
 operation_p = (
     reduce(
         lambda x, y: x | y,
         [lexeme(string(a)) for a in ["<=", ">=", ">", "<", "==", "!=", "=~", "!~"]],
     )
@@ -261,28 +265,45 @@
 in_out_p = lexeme(string("<-") >> two_directional_edge_definition_parser << string("->")).map(
     lambda nav: Navigation(nav[0], nav[1], nav[2], Direction.any, nav[3])
 )
 navigation_parser = in_out_p | out_p | in_p
 
 tag_parser = lexeme(string("#") >> literal_p).optional()
 with_p = lexeme(string("with"))
+with_usage_p = lexeme(string("with_usage"))
 count_p = lexeme(string("count"))
 
 len_empty = lexeme(string("empty")).result(WithClauseFilter("==", 0))
 len_any = lexeme(string("any")).result(WithClauseFilter(">", 0))
 
 
 @make_parser
 def with_count_parser() -> Parser:
     yield count_p
     op = yield operation_p
     num = yield integer_p
     return WithClauseFilter(op, num)
 
 
+timedelta_parser = duration_parser.map(lambda ds: timedelta(seconds=ds))
+duration_or_datetime_parser = timedelta_parser | iso_date_time_utc_parser
+
+
+@make_parser
+def with_usage_parser() -> Parser:
+    yield with_usage_p
+    yield lparen_p
+    start = yield duration_or_datetime_parser
+    end = yield ((whitespace + colon_p + colon_p) >> duration_or_datetime_parser).optional()
+    yield comma_p
+    metrics = yield literal_list_optional_brackets
+    yield rparen_p
+    return WithUsage(start, end, metrics)
+
+
 @make_parser
 def with_clause_parser() -> Parser:
     yield with_p
     yield lparen_p
     with_filter = yield len_empty | len_any | with_count_parser
     yield comma_p
     nav = yield navigation_parser
@@ -329,24 +350,26 @@
 
 
 limit_parser = limit_p >> space_dp >> limit_parser_direct
 
 
 @make_parser
 def part_parser() -> Parser:
+    with_usage = yield with_usage_parser.optional()
     term = yield term_parser.optional()
     yield whitespace
     with_clause = yield with_clause_parser.optional()
     tag = yield tag_parser
     sort = yield sort_parser.optional()
     limit = yield limit_parser.optional()
     reverse = yield reversed_p
-    nav = yield navigation_parser.optional() if term or sort or limit else navigation_parser
+    part_def = bool(with_usage or term or with_clause or tag or sort or limit or reverse)
+    nav = yield navigation_parser.optional() if part_def else navigation_parser
     term = term if term else AllTerm()
-    return Part(term, tag, with_clause, sort if sort else [], limit, nav, reverse)
+    return Part(term, tag, with_clause, with_usage, sort if sort else [], limit, nav, reverse)
 
 
 @make_parser
 def key_value_preamble_parser() -> Parser:
     key = yield preamble_prop_p
     yield equals_p
     value = yield quoted_string_p | true_p | false_p | float_p | integer_p | literal_p
@@ -359,15 +382,17 @@
     key_values = yield key_value_preamble_parser.sep_by(comma_p)
     yield rparen_p
     return dict(key_values)
 
 
 as_p = lexeme(string("as"))
 aggregate_p = lexeme(string("aggregate"))
-aggregate_func_p = reduce(lambda x, y: x | y, [lexeme(string(a)) for a in ["sum", "count", "min", "max", "avg"]])
+aggregate_func_p = reduce(
+    lambda x, y: x | y, [lexeme(string(a)) for a in ["sum", "count", "min", "max", "avg", "stddev", "variance"]]
+)
 match_p = lexeme(string("match"))
 aggregate_variable_name_p = variable_p.map(AggregateVariableName)
 no_curly_dp = regex(r'[^{"]+')
 var_in_curly = (l_curly_dp >> variable_p << r_curly_dp).map(AggregateVariableName)
 aggregate_group_variable_name_combined_p = (
     double_quote_dp >> (no_curly_dp | var_in_curly).at_least(1).map(AggregateVariableCombined) << double_quote_dp
 )
@@ -428,14 +453,15 @@
     yield colon_p if maybe_aggregate or maybe_preamble else colon_p.optional()
     return maybe_aggregate, preamble
 
 
 @make_parser
 def query_parser() -> Parser:
     maybe_aggregate, preamble = yield preamble_parser
+    # noinspection PyTypeChecker
     parts: List[Part] = yield part_parser.at_least(1)
     # Make sure the parts are connected via traversals (is not enforced by the parser)
     for p in parts[0:-1]:
         if not p.navigation:
             raise ParseError(f"Query can not be executed. Navigation traversal missing after: {p}")
     return Query(parts[::-1], preamble, maybe_aggregate)
```

### Comparing `resotocore-3.6.0/resotocore/query/template_expander.py` & `resotocore-3.6.1/resotocore/query/template_expander.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import functools
 import json
+import re
 from abc import abstractmethod
 from typing import Any, Union, Iterable, Tuple, List, Optional, cast
 
 from parsy import string, Parser, regex, any_char
 from ustache import default_getter, default_virtuals, render, PropertyGetter, TagsTuple, default_tags
 
 from resotocore.error import NoSuchTemplateError
@@ -87,31 +88,56 @@
     async def list_templates(self) -> List[Template]:
         """
         List all available templates in the system.
         :return: all templates in the system.
         """
 
 
+# Replace abbreviated predicate names with actual names
+PredicateNameAdditions = {
+    # shortcut for selecting any attribute on cloud/account/region/zone: cloud.id=123
+    "(cloud[.]).*": "/ancestors.cloud.reported.",
+    "(account[.]).*": "/ancestors.account.reported.",
+    "(region[.]).*": "/ancestors.region.reported.",
+    "(zone[.]).*": "/ancestors.zone.reported.",
+    "(usage[.]).*": "/usage.",
+    # shortcut for selecting by name on cloud/account/region/zone: cloud=aws
+    "(cloud)": "/ancestors.cloud.reported.name",
+    "(account)": "/ancestors.account.reported.name",
+    "(region)": "/ancestors.region.reported.name",
+    "(zone)": "/ancestors.zone.reported.name",
+}
+
+
 class TemplateExpanderBase(TemplateExpander):
     """
     Base expander functionality which implements the expanding functionality
     and leaves the storage functionality to the subsequent classes.
     """
 
+    @staticmethod
+    def change_well_known_names(name: str) -> str:
+        for pattern, addition in PredicateNameAdditions.items():
+            if match := re.fullmatch(pattern, name):
+                res = addition + name[len(match.group(1)) :]
+                return res
+        return name
+
     async def parse_query(
         self, to_parse: str, on_section: Optional[str], *, omit_section_expansion: bool = False, **env: str
     ) -> Query:
         # if the query starts with the term "search " then we parse it as command line
         if to_parse.strip().startswith("search "):
             in_section = PathRoot if omit_section_expansion else on_section or PathRoot
             to_parse = await self.parse_query_from_command_line(to_parse, in_section, **env)
             omit_section_expansion = True  # already done
         rendered = self.render(to_parse, env) if env else to_parse
         expanded, _ = await self.expand(rendered)
         result = query_parser.parse_query(expanded, **env)
+        result = result.change_variable(self.change_well_known_names)
         return result if omit_section_expansion else result.on_section(on_section)
 
     async def expand(self, maybe_expandable: str) -> Tuple[str, List[Expandable]]:
         parts = string_with_expands.parse(maybe_expandable)
         expands = [exp for exp in parts if isinstance(exp, Expandable)]
         if expands:
             result = ""
```

### Comparing `resotocore-3.6.0/resotocore/query/template_expander_service.py` & `resotocore-3.6.1/resotocore/query/template_expander_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Optional, List
 
 from resotocore.cli import strip_quotes
 from resotocore.cli.model import CLI, CLIContext
 from resotocore.db.templatedb import TemplateEntityDb
 from resotocore.query.model import Template
 from resotocore.query.template_expander import TemplateExpanderBase
+from resotocore.service import Service
 from resotocore.types import Json
 
 
-class TemplateExpanderService(TemplateExpanderBase):
+class TemplateExpanderService(TemplateExpanderBase, Service):
     """
     Template expander, which maintains the templates in the database.
     """
 
     def __init__(self, db: TemplateEntityDb, cli: CLI) -> None:
         self.db = db
         self.cli = cli
```

### Comparing `resotocore-3.6.0/resotocore/report/__init__.py` & `resotocore-3.6.1/resotocore/report/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/report/benchmark_renderer.py` & `resotocore-3.6.1/resotocore/report/benchmark_renderer.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/report/inspector_service.py` & `resotocore-3.6.1/resotocore/report/inspector_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     ResotoReportCheck,
     ReportSeverity,
     ReportSeverityPriority,
 )
 from resotocore.report.report_config import ReportCheckCollectionConfig, BenchmarkConfig
 from resotocore.types import Json
 from resotocore.util import value_in_path
-from resotocore.web.service import Service
+from resotocore.service import Service
 
 log = logging.getLogger(__name__)
 
 CountByAccount = Dict[str, int]
 
 
 def benchmark_id(name: str) -> ConfigId:
```

### Comparing `resotocore-3.6.0/resotocore/report/report_config.py` & `resotocore-3.6.1/resotocore/report/report_config.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/static/api-doc.yaml` & `resotocore-3.6.1/resotocore/static/api-doc.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -444,14 +444,22 @@
         - name: graph_id
           in: path
           description: "The identifier of the graph"
           example: resoto
           required: true
           schema:
             type: string
+        - name: wait_for_result
+          in: query
+          description: >
+            If this parameter is set, the request will block until the batch update is finished.
+            The response will contain the batch identifier and the result of the batch update.
+          schema:
+            default: true
+            type: boolean
       requestBody:
         description:
           "The graph is sent as newline delimited json, where each line holds a document, which is either a node or an edge."
         required: true
         content:
           application/x-ndjson:
             schema:
@@ -496,14 +504,22 @@
             A batch identifier is a string that uniquely identifies the batch update.
             If this parameter is omitted, a new batch identifier is created automatically.
             The resulting batch identifier can be retrieved via the response message.
           required: false
           schema:
             default: null
             type: string
+        - name: wait_for_result
+          in: query
+          description: >
+            If this parameter is set, the request will block until the batch update is finished.
+            The response will contain the batch identifier and the result of the batch update.
+          schema:
+            default: true
+            type: boolean
       requestBody:
         description:
           "The graph is sent as newline delimited json, where each line holds a document, which is either a node or an edge."
         required: true
         content:
           application/x-ndjson:
             schema:
```

### Comparing `resotocore-3.6.0/resotocore/static/ck-unicode-truecolor.ans` & `resotocore-3.6.1/resotocore/static/ck-unicode-truecolor.ans`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/static/report/benchmark/aws/aws_cis_1_5.json` & `resotocore-3.6.1/resotocore/static/report/benchmark/aws/aws_cis_1_5.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/static/report/check_template.json` & `resotocore-3.6.1/resotocore/static/report/check_template.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/static/report/checks/aws/aws_apigateway.json` & `resotocore-3.6.1/resotocore/static/report/checks/aws/aws_apigateway.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/static/report/checks/aws/aws_cloudtrail.json` & `resotocore-3.6.1/resotocore/static/report/checks/aws/aws_cloudtrail.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/static/report/checks/aws/aws_config.json` & `resotocore-3.6.1/resotocore/static/report/checks/aws/aws_config.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/static/report/checks/aws/aws_ec2.json` & `resotocore-3.6.1/resotocore/static/report/checks/aws/aws_ec2.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/static/report/checks/aws/aws_efs.json` & `resotocore-3.6.1/resotocore/static/report/checks/aws/aws_efs.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/static/report/checks/aws/aws_iam.json` & `resotocore-3.6.1/resotocore/static/report/checks/aws/aws_iam.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/static/report/checks/aws/aws_kms.json` & `resotocore-3.6.1/resotocore/static/report/checks/aws/aws_kms.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/static/report/checks/aws/aws_lambda.json` & `resotocore-3.6.1/resotocore/static/report/checks/aws/aws_lambda.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/static/report/checks/aws/aws_rds.json` & `resotocore-3.6.1/resotocore/static/report/checks/aws/aws_rds.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/static/report/checks/aws/aws_s3.json` & `resotocore-3.6.1/resotocore/static/report/checks/aws/aws_s3.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/static/resoto_logo_and_text.svg` & `resotocore-3.6.1/resotocore/static/resoto_logo_and_text.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/task/__init__.py` & `resotocore-3.6.1/resotocore/task/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/task/model.py` & `resotocore-3.6.1/resotocore/task/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/task/scheduler.py` & `resotocore-3.6.1/resotocore/task/scheduler.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 
 from apscheduler.executors.asyncio import AsyncIOExecutor
 from apscheduler.job import Job
 from apscheduler.jobstores.memory import MemoryJobStore
 from apscheduler.schedulers.asyncio import AsyncIOScheduler
 from apscheduler.triggers.cron import CronTrigger
 
+from resotocore.service import Service
 from resotolib.utils import get_local_tzinfo
 
 
 warnings.filterwarnings(
     "ignore",
     message="The localize method is no longer necessary, as this time zone supports the fold attribute",
 )
 
 
-class Scheduler:
+class Scheduler(Service):
     def __init__(self) -> None:
         self.scheduler = AsyncIOScheduler(
             jobstores={"default": MemoryJobStore()},
             executors={"default": AsyncIOExecutor()},
             # coalesce: run once instead of many times if the job should be run more than once in succession
             # max_instances: allowed parallel instances for one job
             # misfire_grace_time: seconds after the designated runtime that the job is still allowed to be run
```

### Comparing `resotocore-3.6.0/resotocore/task/start_workflow_on_first_subscriber.py` & `resotocore-3.6.1/resotocore/task/start_workflow_on_first_subscriber.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/task/subscribers.py` & `resotocore-3.6.1/resotocore/task/subscribers.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Optional, Iterable, Dict, List
 
 from resotocore.db.subscriberdb import SubscriberDb
 from resotocore.message_bus import MessageBus
 from resotocore.util import utc, Periodic
 from resotocore.task.model import Subscriber, Subscription
 from resotocore.ids import SubscriberId
-from resotocore.web.service import Service
+from resotocore.service import Service
 
 log = logging.getLogger(__name__)
 
 
 class SubscriptionHandler(Service):
     """
     SubscriptionHandler maintains all subscriptions in memory and syncs its internal state with the underlying db.
```

### Comparing `resotocore-3.6.0/resotocore/task/task_description.py` & `resotocore-3.6.1/resotocore/task/task_description.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,29 +3,42 @@
 import logging
 import uuid
 from abc import ABC
 from asyncio import Task
 from contextlib import suppress
 from datetime import timedelta, datetime
 from enum import Enum
-from typing import Optional, Any, Sequence, MutableSequence, Callable, Dict, List, Set, Tuple, Union
+from typing import Optional, Any, Sequence, MutableSequence, Dict, List, Set, Tuple, Union, TYPE_CHECKING
 
 from apscheduler.triggers.cron import CronTrigger
 from attrs import define
 from frozendict import frozendict
 from jsons import set_deserializer, set_serializer
 from transitions import Machine, State, MachineError
 
 from resotocore.ids import SubscriberId, TaskDescriptorId, TaskId
-from resotocore.message_bus import Event, Action, ActionDone, Message, ActionError, ActionInfo, ActionProgress
+from resotocore.message_bus import (
+    Event,
+    Action,
+    ActionDone,
+    Message,
+    ActionError,
+    ActionInfo,
+    ActionProgress,
+    CoreMessage,
+)
 from resotocore.model.typed_model import to_json, from_js, to_js
 from resotocore.task.model import Subscriber
 from resotocore.types import Json
 from resotocore.util import first, interleave, empty, exist, identity, utc, utc_str
 from resotolib.core.progress import ProgressTree, Progress, ProgressDone
+from resotolib.utils import freeze
+
+if TYPE_CHECKING:  # avoid circular dependency
+    from resotocore.task.task_dependencies import TaskDependencies
 
 log = logging.getLogger(__name__)
 
 
 class StepErrorBehaviour(Enum):
     """
     This enumeration defines the behaviour of steps in case of an error:
@@ -101,14 +114,19 @@
 class WaitForEvent(StepAction):
     # Wait for this event to arrive
     wait_for_message_type: str
     filter_data: Optional[Json] = None
 
 
 @define(order=True, hash=True, frozen=True)
+class WaitForCollectDone(StepAction):
+    pass
+
+
+@define(order=True, hash=True, frozen=True)
 class ExecuteCommand(RestartAgainStepAction):
     # Execute this command in the command interpreter.
     command: str
 
 
 # endregion
 
@@ -399,14 +417,16 @@
         """
         if isinstance(step.action, PerformAction):
             return PerformActionState(step.action, step, instance)
         elif isinstance(step.action, EmitEvent):
             return EmitEventState(step.action, step, instance)
         elif isinstance(step.action, WaitForEvent):
             return WaitForEventState(step.action, step, instance)
+        elif isinstance(step.action, WaitForCollectDone):
+            return WaitForCollectDoneState(step, instance)
         elif isinstance(step.action, ExecuteCommand):
             return ExecuteCommandState(step.action, step, instance)
         else:
             raise AttributeError(f"No mapping for {type(step.action).__name__}")
 
     def step_started(self) -> None:
         """
@@ -446,18 +466,20 @@
     This state emits an action when started and then waits for all actors to respond with a done message.
     State is done, when all subscribers with expected answer send a done message.
     """
 
     def __init__(self, perform: PerformAction, step: Step, instance: RunningTask):
         super().__init__(step, instance)
         self.perform = perform
-        self._wait_for: List[Subscriber] = self.instance.subscribers_by_event().get(perform.message_type, [])
+        self._wait_for: List[Subscriber] = self.instance.dependencies.subscribers_by_event().get(
+            perform.message_type, []
+        )
 
     def wait_for(self) -> List[Subscriber]:
-        existing = {s.id for s in self.instance.subscribers_by_event().get(self.perform.message_type, [])}
+        existing = {s.id for s in self.instance.dependencies.subscribers_by_event().get(self.perform.message_type, [])}
         return [s for s in self._wait_for if s.id in existing]
 
     def current_step_done(self) -> bool:
         """
         This state is done, when we received an ack or an error from every subscriber.
         The step behavior defines how to deal in case of an error.
         """
@@ -483,26 +505,29 @@
             max_timeout = max_timeout if not subscription.wait_for_completion or max_timeout > to else to
         return max_timeout
 
     def commands_to_execute(self) -> Sequence[TaskCommand]:
         """
         When the state is entered, emit the action message and inform all actors.
         """
-        return [SendMessage(Action(self.perform.message_type, self.instance.id, self.step.name))]
+        data = freeze(self.instance.metadata)
+        return [SendMessage(Action(self.perform.message_type, self.instance.id, self.step.name, data))]
 
     def step_started(self) -> None:
         super().step_started()
         # refresh the list of subscribers when the step has started
-        self._wait_for = self.instance.subscribers_by_event().get(self.perform.message_type, [])
+        self._wait_for = self.instance.dependencies.subscribers_by_event().get(self.perform.message_type, [])
 
     def export_state(self) -> Json:
         return {"wait_for": [a.id for a in self._wait_for]}
 
     def import_state(self, js: Json) -> None:
-        existing = {s.id: s for s in self.instance.subscribers_by_event().get(self.perform.message_type, [])}
+        existing = {
+            s.id: s for s in self.instance.dependencies.subscribers_by_event().get(self.perform.message_type, [])
+        }
         wait_for = js.get("wait_for", [])
         # filter all existing subscriber from the list of subscribers to wait_for
         self._wait_for = list(filter(identity, (existing.get(sid) for sid in wait_for)))  # type: ignore
 
     def initial_progress(self, progress: ProgressTree) -> None:
         super().initial_progress(progress)
         if self.wait_for():
@@ -538,14 +563,39 @@
 
         if event.message_type == self.perform.wait_for_message_type and filter_applies():
             self.instance.received_messages.append(event)
             return True
         return False
 
 
+class WaitForCollectDoneState(StepState):
+    def __init__(self, step: Step, instance: RunningTask):
+        super().__init__(step, instance)
+        self.collection_done = False
+
+    def current_step_done(self) -> bool:
+        running = self.instance.dependencies.graph_merger.running_imports.get(self.instance.id)
+        if running is None or running == 0:  # no running imports for this task
+            self.collection_done = True
+
+        # either no collect or event is already received
+        return self.collection_done
+
+    def handle_event(self, event: Event) -> bool:
+        if (
+            not self.collection_done
+            and event.message_type == CoreMessage.GraphMergeCompleted
+            and event.data.get("task_id") == self.instance.id
+        ):
+            self.instance.received_messages.append(event)
+            self.collection_done = True
+            return True
+        return False
+
+
 class ExecuteCommandState(StepState):
     def __init__(self, execute: ExecuteCommand, step: Step, instance: RunningTask):
         super().__init__(step, instance)
         self.execute = execute
         self.execution_done = False
 
     def commands_to_execute(self) -> Sequence[TaskCommand]:
@@ -607,34 +657,41 @@
         super().step_started()
         self.instance.task_duration = utc() - self.instance.task_started_at
 
 
 class RunningTask:
     @staticmethod
     def empty(
-        descriptor: TaskDescription, subscriber_by_event: Callable[[], Dict[str, List[Subscriber]]]
+        descriptor: TaskDescription,
+        dependencies: TaskDependencies,
+        metadata: Optional[Json] = None,
     ) -> Tuple[RunningTask, Sequence[TaskCommand]]:
         assert len(descriptor.steps) > 0, "TaskDescription needs at least one step!"
         uid = TaskId(str(uuid.uuid1()))
-        task = RunningTask(uid, descriptor, subscriber_by_event)
+        task = RunningTask(uid, descriptor, dependencies, metadata)
         messages = [SendMessage(Event("task_started", data={"task": descriptor.name})), *task.move_to_next_state()]
         return task, messages
 
     def __init__(
-        self, uid: TaskId, descriptor: TaskDescription, subscribers_by_event: Callable[[], Dict[str, List[Subscriber]]]
+        self,
+        uid: TaskId,
+        descriptor: TaskDescription,
+        dependencies: TaskDependencies,
+        metadata: Optional[Json] = None,
     ):
         self.id = uid
         self.is_error = False
         self.descriptor = descriptor
         self.received_messages: MutableSequence[Message] = []
-        self.subscribers_by_event = subscribers_by_event
+        self.dependencies = dependencies
         self.task_started_at = utc()
         self.task_duration: Optional[timedelta] = None
         self.update_task: Optional[Task[None]] = None
         self.descriptor_alive = True
+        self.metadata = metadata or {}
         self.info_messages: List[Union[ActionInfo, ActionError]] = []
         self.__progress: ProgressTree = ProgressTree(self.descriptor.name)
         self.__progress_updated_at: datetime = utc()
         self.__progress_emitted_at: Optional[datetime] = None
 
         steps = []
         for step in descriptor.steps:
```

### Comparing `resotocore-3.6.0/resotocore/task/task_handler.py` & `resotocore-3.6.1/resotocore/task/task_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 from __future__ import annotations
 
 import asyncio
 import logging
+import re
 from asyncio import Task, CancelledError
 from contextlib import suppress
 from copy import copy
-from attrs import evolve
 from datetime import timedelta
 from typing import Optional, Any, Callable, Union, Sequence, Dict, List, Tuple
-
 from aiostream import stream
+from attrs import evolve
 
 from resotocore.analytics import AnalyticsEventSender, CoreEvent
 from resotocore.cli.model import CLIContext, CLI
 from resotocore.core_config import CoreConfig
 from resotocore.db.jobdb import JobDb
 from resotocore.db.runningtaskdb import RunningTaskData, RunningTaskDb
+from resotocore.ids import SubscriberId, TaskDescriptorId
 from resotocore.message_bus import (
     MessageBus,
     Event,
     Action,
     ActionDone,
     Message,
     ActionError,
     ActionInfo,
     ActionProgress,
     CoreMessage,
 )
-from resotocore.ids import SubscriberId, TaskDescriptorId
+from resotocore.model.db_updater import GraphMerger
+from resotocore.service import Service
 from resotocore.task import TaskHandler, RunningTaskInfo
 from resotocore.task.model import Subscriber
 from resotocore.task.scheduler import Scheduler
 from resotocore.task.start_workflow_on_first_subscriber import wait_and_start
 from resotocore.task.subscribers import SubscriptionHandler
+from resotocore.task.task_dependencies import TaskDependencies
 from resotocore.task.task_description import (
     Workflow,
     RunningTask,
     EventTrigger,
     TimeTrigger,
     TaskSurpassBehaviour,
     PerformAction,
@@ -46,31 +49,33 @@
     ExecuteCommand,
     TaskCommand,
     SendMessage,
     ExecuteOnCLI,
     StepErrorBehaviour,
     RestartAgainStepAction,
     Trigger,
+    WaitForCollectDone,
 )
 from resotocore.util import first, Periodic, group_by, utc_str, utc, partition_by
-import re
+from resotocore.types import Json
 
 log = logging.getLogger(__name__)
 
 
-class TaskHandlerService(TaskHandler):
+class TaskHandlerService(TaskHandler, Service):
     # region init
 
     def __init__(
         self,
         running_task_db: RunningTaskDb,
         job_db: JobDb,
         message_bus: MessageBus,
         event_sender: AnalyticsEventSender,
         subscription_handler: SubscriptionHandler,
+        graph_merger: GraphMerger,
         scheduler: Scheduler,
         cli: CLI,
         config: CoreConfig,
     ):
         self.running_task_db = running_task_db
         self.job_db = job_db
         self.message_bus = message_bus
@@ -87,14 +92,15 @@
         self.task_descriptions: Sequence[TaskDescription] = [*self.known_workflows(config), *self.known_jobs()]
         self.tasks: Dict[str, RunningTask] = {}
         self.message_bus_watcher: Optional[Task[None]] = None
         self.initial_start_workflow_task: Optional[Task[None]] = None
         self.timeout_watcher = Periodic("task_watcher", self.check_running_tasks, timedelta(seconds=10))
         self.registered_event_trigger: List[Tuple[EventTrigger, TaskDescription]] = []
         self.registered_event_trigger_by_message_type: Dict[str, List[Tuple[EventTrigger, TaskDescription]]] = {}
+        self.task_dependencies = TaskDependencies(graph_merger, subscription_handler.subscribers_by_event)
 
     # endregion
 
     # region startup and teardown
 
     async def update_trigger(self, desc: TaskDescription, register: bool = True) -> None:
         # safeguard: unregister all event trigger of this task
@@ -129,17 +135,35 @@
             else:
                 return step
 
         updated = copy(descriptor)
         updated.steps = [evaluate(step) for step in descriptor.steps]
         return updated
 
+    async def fetch_task_metadata(self, descriptor_id: TaskDescriptorId) -> Json:
+        timing: Dict[str, Dict[str, int]] = {}
+        if last_workflow_run := await self.running_task_db.last(descriptor_id=descriptor_id):
+            timing = {
+                s.step_name: {
+                    "started_at": int(s.started_at.timestamp()),
+                    "finished_at": int(s.finished_at.timestamp()),
+                }
+                for s in last_workflow_run.step_states
+                if s.finished_at and s.started_at
+            }
+        return {
+            "timing": timing,
+        }
+
     async def start_task_directly(self, desc: TaskDescription, reason: str) -> RunningTask:
         updated = self.evaluate_task_definition(desc)
-        task, commands = RunningTask.empty(updated, self.subscription_handler.subscribers_by_event)
+
+        metadata = await self.fetch_task_metadata(desc.id)
+        task, commands = RunningTask.empty(updated, self.task_dependencies, metadata=metadata)
+
         log.info(f"Start new task: {updated.name} with id {task.id}")
         # store initial state in database
         await self.running_task_db.insert(task)
         self.tasks[task.id] = task
         await self.execute_task_commands(task, commands)
         await self.event_sender.core_event(
             CoreEvent.TaskStarted,
@@ -203,15 +227,15 @@
 
         instances: List[RunningTask] = []
         async for data in self.running_task_db.all_running():
             descriptor = descriptions.get(data.task_descriptor_id)
             if descriptor:
                 # we have captured the timestamp when the task has been started
                 updated = self.evaluate_task_definition(descriptor, now=utc_str(data.task_started_at))
-                rt = RunningTask(data.id, updated, self.subscription_handler.subscribers_by_event)
+                rt = RunningTask(data.id, updated, self.task_dependencies)
                 instance = reset_state(rt, data)
                 if isinstance(instance.current_step.action, RestartAgainStepAction):
                     log.info(f"Restart interrupted action: {instance.current_step.action}")
                     await self.execute_task_commands(instance, instance.current_state.commands_to_execute())
                 instances.append(instance)
 
             else:
@@ -464,14 +488,15 @@
                     elif isinstance(command, ExecuteOnCLI):
                         ctx = evolve(self.cli_context, env={**command.env, **wi.descriptor.environment})
                         result = await self.cli.execute_cli_command(command.command, stream.list, ctx)
                         results[command] = result
                     else:
                         raise AttributeError(f"Does not understand this command: {wi.descriptor.name}:  {command}")
                 except Exception as ex:
+                    log.info(f"Error executing command: {command} {ex}")
                     results[command] = ex
 
             # The descriptor might be removed in the meantime. If this is the case stop execution.
             if wi.descriptor_alive:
                 active_before_result = wi.is_active
                 # before we move on, we need to store the current state of the task (or delete if it is done)
                 await self.store_running_task_state(wi, origin_message)
@@ -576,14 +601,15 @@
             if wf_config:
                 trigger.append(TimeTrigger(wf_config.schedule))
             return Workflow(uid=name, name=name, steps=steps, triggers=trigger, on_surpass=TaskSurpassBehaviour.Wait)
 
         collect_steps = [
             Step("pre_collect", PerformAction("pre_collect"), timedelta(seconds=10)),
             Step("collect", PerformAction("collect"), timedelta(seconds=10)),
+            Step("wait_for_graph_merged", WaitForCollectDone(), timedelta(minutes=10)),
             Step("merge_outer_edges", PerformAction("merge_outer_edges"), timedelta(seconds=10)),
             Step("post_collect", PerformAction("post_collect"), timedelta(seconds=10)),
         ]
         cleanup_steps = [
             Step("pre_cleanup_plan", PerformAction("pre_cleanup_plan"), timedelta(seconds=10)),
             Step("cleanup_plan", PerformAction("cleanup_plan"), timedelta(seconds=10)),
             Step("post_cleanup_plan", PerformAction("post_cleanup_plan"), timedelta(seconds=10)),
```

### Comparing `resotocore-3.6.0/resotocore/templates/base.html` & `resotocore-3.6.1/resotocore/templates/base.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/templates/create_first_user.html` & `resotocore-3.6.1/resotocore/templates/create_first_user.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/templates/login.html` & `resotocore-3.6.1/resotocore/templates/login.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/types.py` & `resotocore-3.6.1/resotocore/types.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/user/__init__.py` & `resotocore-3.6.1/resotocore/user/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Dict, List, ClassVar, Optional, Type, Set, Any
 
 from attr import define, field
 
 from resotocore.ids import ConfigId, Email, Password
 from resotocore.model.typed_model import to_js
 from resotocore.types import Json
-from resotocore.web.service import Service
+from resotocore.service import Service
 from resotolib.core.model_export import dataclasses_to_resotocore_model
 
 UsersConfigRoot = "resoto_users"
 UsersConfigId = ConfigId("resoto.users")
 
 
 ValidRoles = {"admin", "readwrite", "readonly"}
```

### Comparing `resotocore-3.6.0/resotocore/user/user_management.py` & `resotocore-3.6.1/resotocore/user/user_management.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/util.py` & `resotocore-3.6.1/resotocore/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 import asyncio
 import hashlib
 import json
 import logging
 import random
+import re
 import string
 import sys
 import uuid
-from asyncio import Future
+from asyncio import Future, AbstractEventLoop, Task
 from collections import defaultdict
 from collections.abc import Iterable
 from contextlib import suppress
 from datetime import timedelta, datetime, timezone
 from typing import (
     Any,
     Callable,
@@ -23,31 +24,81 @@
     Dict,
     List,
     Tuple,
     AsyncIterator,
     Iterator,
     Union,
     Sequence,
+    Awaitable,
 )
-import re
 
 from dateutil.parser import isoparse, parse as parse_date
-from resotolib.asynchronous import periodic
 
-from resotolib.durations import parse_duration
 from resotocore.error import RestartService
+from resotocore.service import Service
 from resotocore.types import JsonElement, Json
+from resotolib.durations import parse_duration
 
 log = logging.getLogger(__name__)
 
 AnyT = TypeVar("AnyT")
 AnyR = TypeVar("AnyR")
 
-# moved to resotolib. define it here to have stable references
-Periodic = periodic.Periodic
+
+class Periodic(Service):
+    """
+    Periodic execution of a function based on a defined frequency that can be started and stopped.
+    """
+
+    def __init__(
+        self,
+        name: str,
+        func: Callable[[], Any],
+        frequency: timedelta,
+        first_run: Optional[timedelta] = None,
+        loop: Optional[AbstractEventLoop] = None,
+    ):
+        self.name = name
+        self.func = func
+        self.frequency = frequency
+        self.first_run = first_run if first_run else frequency
+        self._task: Optional[Task[None]] = None
+        self._loop = loop
+
+    @property
+    def started(self) -> bool:
+        return self._task is not None
+
+    async def start(self) -> None:
+        if self._task is None:
+            # Start task to call func periodically:
+            self._task = asyncio.ensure_future(self._run(), loop=self._loop)
+            log.debug(f"Periodic task {self.name} has been started.")
+
+    async def stop(self) -> None:
+        # Stop task and await it stopped:
+        if self._task is not None:
+            self._task.cancel()
+            with suppress(asyncio.CancelledError):
+                await self._task
+
+    async def _run(self) -> None:
+        await asyncio.sleep(self.first_run.total_seconds())
+        while True:
+            log.debug(f"Execute periodic task {self.name}.")
+            try:
+                result = self.func()
+                if isinstance(result, Awaitable):
+                    await result
+            except Exception as ex:
+                log.error(
+                    f"Periodic function {self.name} caught an exception: {ex}",
+                    exc_info=ex,
+                )
+            await asyncio.sleep(self.frequency.total_seconds())
 
 
 # noinspection PyUnusedLocal
 async def async_noop(*args: Any, **kwargs: Any) -> None:
     pass
 
 
@@ -85,35 +136,35 @@
 def utc() -> datetime:
     return datetime.now(timezone.utc)
 
 
 def utc_str(dt: Optional[datetime] = None, date_format: str = UTC_Date_Format) -> str:
     if dt is None:
         dt = utc()
-    if dt.tzinfo is not None and dt.tzname() != "UTC":
-        offset = dt.tzinfo.utcoffset(dt)
-        if offset is not None and offset.total_seconds() != 0:
-            dt = (dt - offset).replace(tzinfo=timezone.utc)
+    if dt.tzinfo is None:
+        dt = dt.replace(tzinfo=timezone.utc)
+    elif dt.tzinfo == timezone.utc:
+        pass
+    else:
+        dt = dt.astimezone(timezone.utc)
     return dt.strftime(date_format)
 
 
 def from_utc(date_string: str) -> datetime:
     return isoparse(date_string)
 
 
 def parse_utc(date_string: str) -> datetime:
     try:
         dt = datetime.fromisoformat(date_string)
     except Exception:
         dt = parse_date(date_string)
-    if (
-        not dt.tzinfo
-        or dt.tzinfo.utcoffset(None) is None
-        or dt.tzinfo.utcoffset(None).total_seconds() != 0  # type: ignore
-    ):
+    if dt.tzinfo is None:
+        dt = dt.replace(tzinfo=timezone.utc)
+    elif dt.tzinfo == timezone.utc:
         dt = dt.astimezone(timezone.utc)
     return dt
 
 
 def duration(d: str) -> timedelta:
     return parse_duration(d)
```

### Comparing `resotocore-3.6.0/resotocore/validator.py` & `resotocore-3.6.1/resotocore/validator.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/web/api.py` & `resotocore-3.6.1/resotocore/web/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,74 +48,64 @@
 from aiohttp.web import Request, StreamResponse, WebSocketResponse
 from aiohttp.web_exceptions import HTTPNotFound, HTTPNoContent, HTTPOk, HTTPNotAcceptable, HTTPSeeOther
 from aiohttp.web_fileresponse import FileResponse
 from aiohttp.web_response import json_response
 from aiohttp_swagger3 import SwaggerFile, SwaggerUiSettings
 from aiostream import stream
 from attrs import evolve
+from dateutil import parser as date_parser
 from networkx.readwrite import cytoscape_data
 from resotoui import ui_path
-from dateutil import parser as date_parser
 
-from resotocore.analytics import AnalyticsEventSender, AnalyticsEvent
+from resotocore.analytics import AnalyticsEvent
 from resotocore.cli.command import alias_names
+from resotocore.dependencies import Dependencies
 from resotocore.cli.model import (
     ParsedCommandLine,
     CLIContext,
     CLICommand,
     InternalPart,
     WorkerCustomCommand,
-    CLI,
     AliasTemplate,
     InfraAppAlias,
     FilePath,
 )
-from resotocore.config import ConfigHandler, ConfigValidation, ConfigEntity
+from resotocore.config import ConfigValidation, ConfigEntity
 from resotocore.console_renderer import ConsoleColorSystem, ConsoleRenderer
-from resotocore.core_config import CoreConfig
-from resotocore.db.db_access import DbAccess
 from resotocore.db.graphdb import GraphDB, HistoryChange
 from resotocore.db.model import QueryModel
 from resotocore.error import NotFoundError
-from resotocore.graph_manager.graph_manager import GraphManager
 from resotocore.ids import TaskId, ConfigId, NodeId, SubscriberId, WorkerId, GraphName, Email, Password
-from resotocore.message_bus import MessageBus, Message, ActionDone, Action, ActionError, ActionInfo, ActionProgress
-from resotocore.model.db_updater import merge_graph_process
+from resotocore.message_bus import Message, ActionDone, Action, ActionError, ActionInfo, ActionProgress
+from resotocore.metrics import timed
 from resotocore.model.graph_access import Section
 from resotocore.model.json_schema import json_schema
 from resotocore.model.model import Kind, Model
-from resotocore.model.model_handler import ModelHandler
 from resotocore.model.typed_model import to_json, from_js, to_js_str, to_js
-from resotocore.query import QueryParser
-from resotocore.report import Inspector
+from resotocore.service import Service
 from resotocore.task.model import Subscription
-from resotocore.task.subscribers import SubscriptionHandler
-from resotocore.task.task_handler import TaskHandlerService
 from resotocore.types import Json, JsonElement
-from resotocore.user import UserManagement
 from resotocore.util import uuid_str, force_gen, rnd_str, if_set, duration, utc_str, parse_utc, async_noop, utc
-from resotocore.web.certificate_handler import CertificateHandler
+from resotocore.web.auth import raw_jwt_from_auth_message, AuthorizedUser, AuthHandler
 from resotocore.web.content_renderer import result_binary_gen, single_result
 from resotocore.web.directives import (
     metrics_handler,
     error_handler,
     on_response_prepare,
     cors_handler,
     enable_compression,
     default_middleware,
 )
 from resotocore.web.tsdb import tsdb
 from resotocore.worker_task_queue import (
     WorkerTaskDescription,
-    WorkerTaskQueue,
     WorkerTask,
     WorkerTaskResult,
     WorkerTaskInProgress,
 )
-from resotocore.web.auth import raw_jwt_from_auth_message, AuthorizedUser, AuthHandler
 from resotolib.asynchronous.web.ws_handler import accept_websocket, clean_ws_handler
 from resotolib.jwt import encode_jwt
 from resotolib.x509 import cert_to_bytes
 
 log = logging.getLogger(__name__)
 
 
@@ -142,68 +132,37 @@
     "/notebook/.*",
     "/debug/.*",
 }
 # Authorization is not required, but implemented as part of the request handler
 DeferredCheck = {"/events", "/work/queue"}
 
 
-class Api:
-    def __init__(
-        self,
-        db: DbAccess,
-        model_handler: ModelHandler,
-        subscription_handler: SubscriptionHandler,
-        workflow_handler: TaskHandlerService,
-        message_bus: MessageBus,
-        event_sender: AnalyticsEventSender,
-        worker_task_queue: WorkerTaskQueue,
-        cert_handler: CertificateHandler,
-        config_handler: ConfigHandler,
-        inspector: Inspector,
-        cli: CLI,
-        query_parser: QueryParser,
-        config: CoreConfig,
-        user_management: UserManagement,
-        get_override: Callable[[ConfigId], Optional[Json]],
-        graph_manager: GraphManager,
-    ):
-        self.db = db
-        self.model_handler = model_handler
-        self.subscription_handler = subscription_handler
-        self.workflow_handler = workflow_handler
-        self.message_bus = message_bus
-        self.event_sender = event_sender
-        self.worker_task_queue = worker_task_queue
-        self.cert_handler = cert_handler
-        self.config_handler = config_handler
-        self.inspector = inspector
-        self.cli = cli
-        self.query_parser = query_parser
-        self.config = config
-        self.user_management = user_management
-        self.get_override = get_override
-        self.auth_handler = AuthHandler(db.system_data_db, config, cert_handler, AlwaysAllowed | DeferredCheck)
-        self.graph_manager = graph_manager
+class Api(Service):
+    def __init__(self, deps: Dependencies):
+        self.deps = deps
+        self.auth_handler = AuthHandler(
+            deps.db_access.system_data_db, deps.config, deps.cert_handler, AlwaysAllowed | DeferredCheck
+        )
 
         self.app = web.Application(
-            client_max_size=config.api.max_request_size or 1024**2,
+            client_max_size=self.deps.config.api.max_request_size or 1024**2,
             # note on order: the middleware is passed in the order provided.
             middlewares=[
                 metrics_handler,
                 self.auth_handler.middleware(),
                 cors_handler,
-                error_handler(config, event_sender),
+                error_handler(deps.config, deps.event_sender),
                 default_middleware(self),
             ],
         )
         self.app.on_response_prepare.append(on_response_prepare)
         self._session: Optional[ClientSession] = None
         self.in_shutdown = False
         self.websocket_handler: Dict[str, Tuple[Future[Any], WebSocketResponse]] = {}
-        path_part = config.api.web_path.strip().strip("/").strip()
+        path_part = deps.config.api.web_path.strip().strip("/").strip()
         web_path = "" if path_part == "" else f"/{path_part}"
         self.__add_routes(web_path)
         aiohttp_jinja2.setup(
             self.app, loader=jinja2.FileSystemLoader(os.path.abspath(os.path.dirname(__file__) + "/../templates"))
         )
 
     @property
@@ -321,15 +280,15 @@
                 web.get(prefix + "/authorization/user", self.get_authorized_user),
                 web.get(prefix + "/authorization/renew", self.renew_authorization),
                 # tsdb operations
                 web.route(METH_ANY, prefix + "/tsdb/{tail:.+}", tsdb(self)),
                 web.static(f"{prefix}/ui/", ui_path),
             ]
         )
-        if self.config.runtime.debug:
+        if self.deps.config.runtime.debug:
             self.app.add_routes([web.get(prefix + "/debug/ui/{commit}/{path:.+}", self.serve_debug_ui)])
         SwaggerFile(
             self.app,
             spec_file=f"{static_path}/api-doc.yaml",
             swagger_ui_settings=SwaggerUiSettings(path=prefix + "/api-doc", layout="BaseLayout", docExpansion="none"),
         )
 
@@ -367,15 +326,15 @@
     async def ready(_: Request) -> StreamResponse:
         return web.HTTPOk(text="ok")
 
     async def jwks(self, _: Request) -> StreamResponse:
         return web.json_response(self.auth_handler.signing_key_jwk)
 
     async def login_page(self, request: Request) -> StreamResponse:
-        template = "login.html" if await self.user_management.has_users() else "create_first_user.html"
+        template = "login.html" if await self.deps.user_management.has_users() else "create_first_user.html"
         return aiohttp_jinja2.render_template(template, request, context=request.query)
 
     async def create_first_user(self, request: Request) -> StreamResponse:
         post_data = await request.post()
         errors = []
         try:
             email = Email(str(post_data.get("email", "")).strip())
@@ -390,31 +349,31 @@
             if not company:
                 errors.append("Company name is required")
             if not fullname:
                 errors.append("Full name is required")
             if password != password_repeat:
                 errors.append("Passwords do not match")
             if not errors:
-                await self.user_management.create_first_user(company, fullname, email, password)
+                await self.deps.user_management.create_first_user(company, fullname, email, password)
                 return await self.authenticate(request)
         except Exception as e:
             errors.append(str(e))
         error_string = ". ".join(errors)
         return aiohttp_jinja2.render_template(
             "create_first_user.html", request, context={**post_data, "error": error_string}
         )
 
     async def authenticate(self, request: Request) -> StreamResponse:
         post_data = await request.post()
         email = Email(str(post_data.get("email", "")))
         password = Password(str(post_data.get("password", "")))
         redirect = str(post_data.get("redirect", ""))
-        if email and password and (user := await self.user_management.login(email, password)):
+        if email and password and (user := await self.deps.user_management.login(email, password)):
             params: Dict[str, List[str]] = {}
-            if self.config.args.psk:
+            if self.deps.config.args.psk:
                 code = await self.auth_handler.add_authorized_user(AuthorizedUser(email, user.roles, utc()))
                 params["code"] = [code]
             if redirect:
                 if params:
                     parsed = urlparse(redirect)
                     query_params = parse_qs(parsed.query)
                     query_params.update(params)
@@ -441,22 +400,22 @@
             user = AuthorizedUser(jwt_raw["email"], set(jwt_raw["roles"].split(",")), exp)
             renewed, data = self.auth_handler.user_jwt(user)
             return web.json_response(data, headers={"Authorization": f"Bearer {renewed}"})
         else:
             return HTTPNoContent()  # no psk, no renewal
 
     async def list_configs(self, request: Request) -> StreamResponse:
-        return await self.stream_response_from_gen(request, self.config_handler.list_config_ids())
+        return await self.stream_response_from_gen(request, self.deps.config_handler.list_config_ids())
 
     async def get_config(self, request: Request) -> StreamResponse:
         config_id = ConfigId(request.match_info["config_id"])
         accept = request.headers.get("accept", "application/json")
         not_found = HTTPNotFound(text="No config with this id")
         if accept == "application/yaml":
-            yml = await self.config_handler.config_yaml(config_id)
+            yml = await self.deps.config_handler.config_yaml(config_id)
             return web.Response(body=yml.encode("utf-8"), content_type="application/yaml") if yml else not_found
         else:
 
             def get_query_param_bool(name: str, default: bool) -> bool:
                 return request.query.get(name, "true" if default else "false").lower() == "true"
 
             # do we want the config with overrides/env_vars applied in-place or in a separate object?
@@ -473,21 +432,21 @@
                 # if we request a single object with overrides applied,
                 # we apply overrides and resolve env vars by default
                 apply_overrides = get_query_param_bool("apply_overrides", default=True)
                 resolve_env_vars = get_query_param_bool("resolve_env_vars", default=True)
                 # ignored in case of a single config object requested
                 include_raw_config = False
 
-            config = await self.config_handler.get_config(config_id, apply_overrides, resolve_env_vars)
+            config = await self.deps.config_handler.get_config(config_id, apply_overrides, resolve_env_vars)
             if config:
                 headers = {"Resoto-Config-Revision": config.revision}
                 if separate_overrides:
-                    payload = {"config": config.config, "overrides": self.get_override(config_id)}
+                    payload = {"config": config.config, "overrides": self.deps.config_override.get_override(config_id)}
                     if include_raw_config:
-                        raw_config = await self.config_handler.get_config(
+                        raw_config = await self.deps.config_handler.get_config(
                             config_id, apply_overrides=False, resolve_env_vars=False
                         )
                         payload["raw_config"] = raw_config.config if raw_config else None
                 else:
                     payload = config.config
 
                 return await single_result(request, payload, headers)
@@ -495,186 +454,192 @@
                 return not_found
 
     async def put_config(self, request: Request) -> StreamResponse:
         config_id = ConfigId(request.match_info["config_id"])
         validate = request.query.get("validate", "true").lower() != "false"
         dry_run = request.query.get("dry_run", "false").lower() == "true"
         config = await self.json_from_request(request)
-        result = await self.config_handler.put_config(
+        result = await self.deps.config_handler.put_config(
             ConfigEntity(config_id, config), validate=validate, dry_run=dry_run
         )
         headers = {"Resoto-Config-Revision": result.revision}
         return await single_result(request, result.config, headers)
 
     async def patch_config(self, request: Request) -> StreamResponse:
         config_id = ConfigId(request.match_info["config_id"])
         validate = request.query.get("validate", "true").lower() != "false"
         dry_run = request.query.get("dry_run", "false").lower() == "true"
         patch = await self.json_from_request(request)
-        updated = await self.config_handler.patch_config(
+        updated = await self.deps.config_handler.patch_config(
             ConfigEntity(config_id, patch), validate=validate, dry_run=dry_run
         )
         headers = {"Resoto-Config-Revision": updated.revision}
         return await single_result(request, updated.config, headers)
 
     async def delete_config(self, request: Request) -> StreamResponse:
         config_id = ConfigId(request.match_info["config_id"])
-        await self.config_handler.delete_config(config_id)
+        await self.deps.config_handler.delete_config(config_id)
         return HTTPNoContent()
 
     async def list_config_models(self, request: Request) -> StreamResponse:
-        return await self.stream_response_from_gen(request, self.config_handler.list_config_validation_ids())
+        return await self.stream_response_from_gen(request, self.deps.config_handler.list_config_validation_ids())
 
     async def get_config_validation(self, request: Request) -> StreamResponse:
         config_id = request.match_info["config_id"]
-        model = await self.config_handler.get_config_validation(config_id)
+        model = await self.deps.config_handler.get_config_validation(config_id)
         return await single_result(request, to_js(model)) if model else HTTPNotFound(text="No model for this config.")
 
     async def get_configs_model(self, request: Request) -> StreamResponse:
-        model = await self.config_handler.get_configs_model()
+        model = await self.deps.config_handler.get_configs_model()
         if request.query.get("flat", "false") == "true":
             model = Model.from_kinds(model.flat_kinds())
         return await single_result(request, to_js(model, strip_nulls=True))
 
     async def update_configs_model(self, request: Request) -> StreamResponse:
         js = await self.json_from_request(request)
         kinds: List[Kind] = from_js(js, List[Kind])
-        model = await self.config_handler.update_configs_model(kinds)
+        model = await self.deps.config_handler.update_configs_model(kinds)
         return await single_result(request, to_js(model))
 
     async def put_config_validation(self, request: Request) -> StreamResponse:
         config_id = request.match_info["config_id"]
         js = await self.json_from_request(request)
         js["id"] = config_id
         config_model = from_js(js, ConfigValidation)
-        model = await self.config_handler.put_config_validation(config_model)
+        model = await self.deps.config_handler.put_config_validation(config_model)
         return await single_result(request, to_js(model))
 
     async def certificate(self, _: Request) -> StreamResponse:
-        cert, fingerprint = self.cert_handler.authority_certificate
+        cert, fingerprint = self.deps.cert_handler.authority_certificate
         headers = {
             "SHA256-Fingerprint": fingerprint,
             "Content-Disposition": 'attachment; filename="resoto_root_ca.pem"',
         }
-        if self.config.args.psk:
-            headers["Authorization"] = "Bearer " + encode_jwt({"sha256_fingerprint": fingerprint}, self.config.args.psk)
+        if self.deps.config.args.psk:
+            headers["Authorization"] = "Bearer " + encode_jwt(
+                {"sha256_fingerprint": fingerprint}, self.deps.config.args.psk
+            )
         return HTTPOk(headers=headers, body=cert, content_type="application/x-pem-file")
 
     async def sign_certificate(self, request: Request) -> StreamResponse:
         csr_bytes = await request.content.read()
-        cert, fingerprint = self.cert_handler.sign(csr_bytes)
+        cert, fingerprint = self.deps.cert_handler.sign(csr_bytes)
         headers = {"SHA256-Fingerprint": fingerprint}
         return HTTPOk(headers=headers, body=cert_to_bytes(cert), content_type="application/x-pem-file")
 
     @staticmethod
     async def metrics(_: Request) -> StreamResponse:
         resp = web.Response(body=prometheus_client.generate_latest())
         resp.content_type = prometheus_client.CONTENT_TYPE_LATEST
         return resp
 
     async def list_all_subscriptions(self, request: Request) -> StreamResponse:
-        subscribers = await self.subscription_handler.all_subscribers()
+        subscribers = await self.deps.subscription_handler.all_subscribers()
         return await single_result(request, to_json(subscribers))
 
     async def get_subscriber(self, request: Request) -> StreamResponse:
         subscriber_id = SubscriberId(request.match_info["subscriber_id"])
-        subscriber = await self.subscription_handler.get_subscriber(subscriber_id)
+        subscriber = await self.deps.subscription_handler.get_subscriber(subscriber_id)
         return self.optional_json(subscriber, f"No subscriber with id {subscriber_id}")
 
     async def list_subscription_for_event(self, request: Request) -> StreamResponse:
         event_type = request.match_info["event_type"]
-        subscribers = await self.subscription_handler.list_subscriber_for(event_type)
+        subscribers = await self.deps.subscription_handler.list_subscriber_for(event_type)
         return await single_result(request, to_json(subscribers))
 
     async def update_subscriber(self, request: Request) -> StreamResponse:
         subscriber_id = SubscriberId(request.match_info["subscriber_id"])
         body = await self.json_from_request(request)
         subscriptions = from_js(body, List[Subscription])
-        sub = await self.subscription_handler.update_subscriptions(subscriber_id, subscriptions)
+        sub = await self.deps.subscription_handler.update_subscriptions(subscriber_id, subscriptions)
         return await single_result(request, to_json(sub))
 
     async def delete_subscriber(self, request: Request) -> StreamResponse:
         subscriber_id = SubscriberId(request.match_info["subscriber_id"])
-        await self.subscription_handler.remove_subscriber(subscriber_id)
+        await self.deps.subscription_handler.remove_subscriber(subscriber_id)
         return web.HTTPNoContent()
 
     async def add_subscription(self, request: Request) -> StreamResponse:
         subscriber_id = SubscriberId(request.match_info["subscriber_id"])
         event_type = request.match_info["event_type"]
         timeout = timedelta(seconds=int(request.query.get("timeout", "60")))
         wait_for_completion = request.query.get("wait_for_completion", "true").lower() != "false"
-        sub = await self.subscription_handler.add_subscription(subscriber_id, event_type, wait_for_completion, timeout)
+        sub = await self.deps.subscription_handler.add_subscription(
+            subscriber_id, event_type, wait_for_completion, timeout
+        )
         return await single_result(request, to_js(sub))
 
     async def delete_subscription(self, request: Request) -> StreamResponse:
         subscriber_id = SubscriberId(request.match_info["subscriber_id"])
         event_type = request.match_info["event_type"]
-        sub = await self.subscription_handler.remove_subscription(subscriber_id, event_type)
+        sub = await self.deps.subscription_handler.remove_subscription(subscriber_id, event_type)
         return await single_result(request, to_js(sub))
 
     async def handle_subscribed(self, request: Request) -> StreamResponse:
         subscriber_id = SubscriberId(request.match_info["subscriber_id"])
-        subscriber = await self.subscription_handler.get_subscriber(subscriber_id)
-        if subscriber_id in self.message_bus.active_listener:
+        subscriber = await self.deps.subscription_handler.get_subscriber(subscriber_id)
+        if subscriber_id in self.deps.message_bus.active_listener:
             log.info(f"There is already a listener for subscriber: {subscriber_id}. Reject.")
             return web.HTTPTooManyRequests(text="Only one connection per subscriber is allowed!")
         elif subscriber and subscriber.subscriptions:
-            pending = await self.workflow_handler.list_all_pending_actions_for(subscriber)
+            pending = await self.deps.task_handler.list_all_pending_actions_for(subscriber)
             return await self.listen_to_events(request, subscriber_id, list(subscriber.subscriptions.keys()), pending)
         else:
             return web.HTTPNotFound(text=f"No subscriber with this id: {subscriber_id} or no subscriptions")
 
     async def perform_benchmark_on_checks(self, request: Request) -> StreamResponse:
         graph = GraphName(request.match_info["graph_id"])
         provider = request.query.get("provider")
         service = request.query.get("service")
         category = request.query.get("category")
         kind = request.query.get("kind")
         acc = request.query.get("accounts")
         accounts = [a.strip() for a in acc.split(",")] if acc else None
-        result = await self.inspector.perform_checks(
+        result = await self.deps.inspector.perform_checks(
             graph, provider=provider, service=service, category=category, kind=kind, accounts=accounts
         )
         return await single_result(request, to_js(result))
 
     async def perform_benchmark(self, request: Request) -> StreamResponse:
         benchmark = request.match_info["benchmark"]
         graph = GraphName(request.match_info["graph_id"])
         acc = request.query.get("accounts")
         accounts = [a.strip() for a in acc.split(",")] if acc else None
-        result = await self.inspector.perform_benchmark(graph, benchmark, accounts=accounts)
+        result = await self.deps.inspector.perform_benchmark(graph, benchmark, accounts=accounts)
         result_graph = result.to_graph()
         async with stream.iterate(result_graph).stream() as streamer:
             await self.stream_response_from_gen(request, streamer, len(result_graph))
         return await single_result(request, to_js(result))
 
     async def inspection_checks(self, request: Request) -> StreamResponse:
         provider = request.query.get("provider")
         service = request.query.get("service")
         category = request.query.get("category")
         kind = request.query.get("kind")
-        inspections = await self.inspector.list_checks(provider=provider, service=service, category=category, kind=kind)
+        inspections = await self.deps.inspector.list_checks(
+            provider=provider, service=service, category=category, kind=kind
+        )
         return await single_result(request, to_js(inspections))
 
     async def inspection_results(self, request: Request) -> StreamResponse:
         graph = GraphName(request.match_info["graph_id"])
         check_id = request.match_info["check_id"]
         acc = request.query.get("accounts")
         accounts = [a.strip() for a in acc.split(",")] if acc else None
-        inspections = await self.inspector.list_failing_resources(graph, check_id, accounts)
+        inspections = await self.deps.inspector.list_failing_resources(graph, check_id, accounts)
         return await self.stream_response_from_gen(request, inspections)
 
     async def handle_events(self, request: Request) -> StreamResponse:
         show = request.query["show"].split(",") if "show" in request.query else ["*"]
         return await self.listen_to_events(request, SubscriberId(str(uuid.uuid1())), show)
 
     async def send_analytics_events(self, request: Request) -> StreamResponse:
         events_json = await self.json_from_request(request)
         events = from_js(events_json, List[AnalyticsEvent])
-        await self.event_sender.capture(events)
+        await self.deps.event_sender.capture(events)
         return web.HTTPNoContent()
 
     async def listen_to_events(
         self,
         request: Request,
         listener_id: SubscriberId,
         event_types: List[str],
@@ -694,29 +659,29 @@
             if "data" in js:
                 js["data"]["subscriber_id"] = listener_id
                 js["data"]["received_at"] = utc_str()
             message: Message = from_js(js, Message)
             if isinstance(message, Action):
                 raise AttributeError("Actors should not emit action messages. ")
             elif isinstance(message, ActionInfo):
-                await self.workflow_handler.handle_action_info(message)
+                await self.deps.task_handler.handle_action_info(message)
             elif isinstance(message, ActionProgress):
-                await self.workflow_handler.handle_action_progress(message)
+                await self.deps.task_handler.handle_action_progress(message)
             elif isinstance(message, ActionDone):
-                await self.workflow_handler.handle_action_done(message)
+                await self.deps.task_handler.handle_action_done(message)
             elif isinstance(message, ActionError):
-                await self.workflow_handler.handle_action_error(message)
+                await self.deps.task_handler.handle_action_error(message)
             else:
-                await self.message_bus.emit(message)
+                await self.deps.message_bus.emit(message)
 
         handler = authorize_request if request.get("authorized", False) is False else handle_message
         return await accept_websocket(
             request,
             handle_incoming=lambda x: handler(x),  # pylint: disable=unnecessary-lambda # it is required!
-            outgoing_context=partial(self.message_bus.subscribe, listener_id, event_types),
+            outgoing_context=partial(self.deps.message_bus.subscribe, listener_id, event_types),
             websocket_handler=self.websocket_handler,
             initial_messages=initial_messages,
         )
 
     async def handle_work_tasks(self, request: Request) -> WebSocketResponse:
         worker_id = WorkerId(uuid_str())
         worker_descriptions: Future[List[WorkerTaskDescription]] = asyncio.get_event_loop().create_future()
@@ -733,37 +698,37 @@
             nonlocal handler
             cmds = from_js(json.loads(msg), List[WorkerCustomCommand])
             description = [WorkerTaskDescription(cmd.name, cmd.filter) for cmd in cmds]
             # set the future and allow attaching the worker to the task queue
             worker_descriptions.set_result(description)
             # register the descriptions as custom command on the CLI
             for cmd in cmds:
-                self.cli.register_alias_template(cmd.to_template())
+                self.deps.cli.register_alias_template(cmd.to_template())
             # the connect process is done, define the final handler
             handler = handle_message
 
         async def handle_message(msg: str) -> None:
             tr = from_js(json.loads(msg), WorkerTaskResult)
             if tr.result == "error":
                 error = tr.error if tr.error else "worker signalled error without detailed error message"
-                await self.worker_task_queue.error_task(worker_id, tr.task_id, error)
+                await self.deps.worker_task_queue.error_task(worker_id, tr.task_id, error)
             elif tr.result == "done":
-                await self.worker_task_queue.acknowledge_task(worker_id, tr.task_id, tr.data)
+                await self.deps.worker_task_queue.acknowledge_task(worker_id, tr.task_id, tr.data)
             else:
                 log.info(f"Do not understand this message: {msg}")
 
         def task_json(task: WorkerTask) -> str:
             return to_js_str(task.to_json())
 
         @asynccontextmanager
         async def connect_to_task_queue() -> AsyncIterator[Queue[WorkerTask]]:
             # we need to wait for the worker to send the list of commands it can handle
             # before we can attach to the worker task queue
             descriptions = await worker_descriptions
-            async with self.worker_task_queue.attach(worker_id, descriptions) as queue:
+            async with self.deps.worker_task_queue.attach(worker_id, descriptions) as queue:
                 yield queue
 
         handler = authorize_request if request.get("authorized", False) is False else handle_connect
         # noinspection PyTypeChecker
         return await accept_websocket(
             request,
             handle_incoming=lambda x: handler(x),  # pylint: disable=unnecessary-lambda # it is required!
@@ -777,15 +742,15 @@
             return {
                 "task": ip.task.to_json(),
                 "worker": ip.worker.worker_id,
                 "retry_counter": ip.retry_counter,
                 "deadline": to_json(ip.deadline),
             }
 
-        return web.json_response([wt_to_js(ot) for ot in self.worker_task_queue.outstanding_tasks.values()])
+        return web.json_response([wt_to_js(ot) for ot in self.deps.worker_task_queue.outstanding_tasks.values()])
 
     async def model_uml(self, request: Request) -> StreamResponse:
         output = request.query.get("output", "svg")
         graph_id = GraphName(request.match_info.get("graph_id", "resoto"))
         show = request.query["show"].split(",") if "show" in request.query else None
         hide = request.query["hide"].split(",") if "hide" in request.query else None
         with_inheritance = request.query.get("with_inheritance", "true") != "false"
@@ -794,15 +759,15 @@
         dependency = set(request.query["dependency"].split(",")) if "dependency" in request.query else None
         with_predecessors = request.query.get("with_predecessors", "false") != "false"
         with_successors = request.query.get("with_successors", "false") != "false"
         with_properties = request.query.get("with_properties", "true") != "false"
         aggregate_roots = request.query.get("aggregate_roots", "true") != "false"
         link_classes = request.query.get("link_classes", "false") != "false"
         sort_props = request.query.get("sort_props", "true") != "false"
-        result = await self.model_handler.uml_image(
+        result = await self.deps.model_handler.uml_image(
             graph_name=graph_id,
             output=output,
             show_packages=show,
             hide_packages=hide,
             with_inheritance=with_inheritance,
             with_base_classes=with_base_classes,
             with_subclasses=with_subclasses,
@@ -819,69 +784,69 @@
         response.headers["Content-Type"] = mt[output]
         await response.prepare(request)
         await response.write_eof(result)
         return response
 
     async def get_model(self, request: Request) -> StreamResponse:
         graph_id = GraphName(request.match_info.get("graph_id", "resoto"))
-        md = await self.model_handler.load_model(graph_id)
+        md = await self.deps.model_handler.load_model(graph_id)
         # default to internal model format, but allow to request json schema format
         if request.headers.get("accept") == "application/schema+json":
             return json_response(json_schema(md), content_type="application/schema+json")
         kinds: Iterable[Kind]
         if request.query.get("flat", "false") == "true":
             kinds = md.flat_kinds()
         else:
             kinds = md.kinds.values()
         return await single_result(request, to_js(kinds, strip_nulls=True))
 
     async def update_model(self, request: Request) -> StreamResponse:
         graph_id = GraphName(request.match_info.get("graph_id", "resoto"))
         js = await self.json_from_request(request)
         kinds: List[Kind] = from_js(js, List[Kind])
-        model = await self.model_handler.update_model(graph_id, kinds)
+        model = await self.deps.model_handler.update_model(graph_id, kinds)
         return await single_result(request, to_js(model, strip_nulls=True))
 
     async def get_node(self, request: Request) -> StreamResponse:
         graph_id = GraphName(request.match_info.get("graph_id", "resoto"))
         node_id = NodeId(request.match_info.get("node_id", "root"))
-        graph = self.db.get_graph_db(graph_id)
-        model = await self.model_handler.load_model(graph_id)
+        graph = self.deps.db_access.get_graph_db(graph_id)
+        model = await self.deps.model_handler.load_model(graph_id)
         node = await graph.get_node(model, node_id)
         if node is None:
             return web.HTTPNotFound(text=f"No such node with id {node_id} in graph {graph_id}")
         else:
             return await single_result(request, node)
 
     async def create_node(self, request: Request) -> StreamResponse:
         graph_id = GraphName(request.match_info.get("graph_id", "resoto"))
         node_id = NodeId(request.match_info.get("node_id", "some_existing"))
         parent_node_id = NodeId(request.match_info.get("parent_node_id", "root"))
-        graph = self.db.get_graph_db(graph_id)
+        graph = self.deps.db_access.get_graph_db(graph_id)
         item = await self.json_from_request(request)
-        md = await self.model_handler.load_model(graph_id)
+        md = await self.deps.model_handler.load_model(graph_id)
         node = await graph.create_node(md, node_id, item, parent_node_id)
         return await single_result(request, node)
 
     async def update_node(self, request: Request) -> StreamResponse:
         graph_id = GraphName(request.match_info.get("graph_id", "resoto"))
         node_id = NodeId(request.match_info.get("node_id", "some_existing"))
         section = section_of(request)
-        graph = self.db.get_graph_db(graph_id)
+        graph = self.deps.db_access.get_graph_db(graph_id)
         patch = await self.json_from_request(request)
-        md = await self.model_handler.load_model(graph_id)
+        md = await self.deps.model_handler.load_model(graph_id)
         node = await graph.update_node(md, node_id, patch, False, section)
         return await single_result(request, node)
 
     async def delete_node(self, request: Request) -> StreamResponse:
         graph_id = GraphName(request.match_info.get("graph_id", "resoto"))
         node_id = NodeId(request.match_info.get("node_id", "some_existing"))
         if node_id == "root":
             raise AttributeError("Root node can not be deleted!")
-        graph = self.db.get_graph_db(graph_id)
+        graph = self.deps.db_access.get_graph_db(graph_id)
         await graph.delete_node(node_id)
         return web.HTTPNoContent()
 
     async def update_nodes(self, request: Request) -> StreamResponse:
         graph_name = GraphName(request.match_info.get("graph_id", "resoto"))
         allowed = {*Section.content, "id", "revision"}
         updates: Dict[NodeId, Json] = {}
@@ -890,97 +855,100 @@
             assert keys.issubset(allowed), f"Invalid json. Allowed keys are: {allowed}"
             assert "id" in elem, f"No id given for element {elem}"
             assert keys.intersection(Section.content), f"No update provided for element {elem}"
             uid = elem["id"]
             assert uid not in updates, f"Only one update allowed per id! {elem}"
             del elem["id"]
             updates[uid] = elem
-        db = self.db.get_graph_db(graph_name)
-        model = await self.model_handler.load_model(graph_name)
+        db = self.deps.db_access.get_graph_db(graph_name)
+        model = await self.deps.model_handler.load_model(graph_name)
         result_gen = db.update_nodes(model, updates)
         return await self.stream_response_from_gen(request, result_gen)
 
     async def list_graphs(self, request: Request) -> StreamResponse:
-        graphs = await self.db.list_graphs()
+        graphs = await self.deps.db_access.list_graphs()
         return await single_result(request, graphs)
 
     async def create_graph(self, request: Request) -> StreamResponse:
         graph_id = request.match_info.get("graph_id", "resoto")
         if "_" in graph_id:
             raise AttributeError("Graph name should not have underscores!")
         graph_name = GraphName(graph_id)
-        graph = await self.db.create_graph(graph_name)
-        model = await self.model_handler.load_model(graph_name)
+        graph = await self.deps.db_access.create_graph(graph_name)
+        model = await self.deps.model_handler.load_model(graph_name)
         root = await graph.get_node(model, NodeId("root"))
         return web.json_response(root)
 
     async def merge_graph(self, request: Request) -> StreamResponse:
-        log.info("Received merge_graph request")
         graph_id = GraphName(request.match_info.get("graph_id", "resoto"))
+        wait_for_result = request.query.get("wait_for_result", "true").lower() == "true"
         task_id: Optional[TaskId] = None
         if tid := request.headers.get("Resoto-Worker-Task-Id"):
             task_id = TaskId(tid)
-        db = self.db.get_graph_db(graph_id)
+        log.info(
+            f"Received merge_graph request for graph {graph_id}, wait_for_result={wait_for_result}, task_id={task_id}"
+        )
+        db = self.deps.db_access.get_graph_db(graph_id)
         it = self.to_line_generator(request)
-        mh = self.model_handler
-        max_wait = self.config.graph_update.merge_max_wait_time()
-        info = await merge_graph_process(db, mh, self.event_sender, self.config, it, max_wait, None, task_id)
-        return web.json_response(to_js(info))
+        max_wait = self.deps.config.graph_update.merge_max_wait_time()
+        info = await self.deps.graph_merger.merge_graph(db, it, max_wait, None, task_id, wait_for_result)
+        return web.json_response(to_js(info)) if info else web.HTTPNoContent()
 
     async def update_merge_graph_batch(self, request: Request) -> StreamResponse:
-        log.info("Received put_sub_graph_batch request")
         graph_id = GraphName(request.match_info.get("graph_id", "resoto"))
+        wait_for_result = request.query.get("wait_for_result", "true").lower() == "true"
         task_id: Optional[TaskId] = None
         if tid := request.headers.get("Resoto-Worker-Task-Id"):
             task_id = TaskId(tid)
-        db = self.db.get_graph_db(graph_id)
+        log.info(f"Received put_sub_graph_batch request for graph {graph_id}, wait_for_result={wait_for_result}")
+        db = self.deps.db_access.get_graph_db(graph_id)
         rnd = "".join(SystemRandom().choice(string.ascii_letters) for _ in range(12))
         batch_id = request.query.get("batch_id", rnd)
         it = self.to_line_generator(request)
-        mh = self.model_handler
-        max_wait = self.config.graph_update.merge_max_wait_time()
-        info = await merge_graph_process(db, mh, self.event_sender, self.config, it, max_wait, batch_id, task_id)
-        return web.json_response(to_json(info), headers={"BatchId": batch_id})
+        max_wait = self.deps.config.graph_update.merge_max_wait_time()
+        info = await self.deps.graph_merger.merge_graph(db, it, max_wait, batch_id, task_id, wait_for_result)
+        headers = {"BatchId": batch_id}
+        return web.json_response(to_json(info), headers=headers) if info else web.HTTPNoContent(headers=headers)
 
     async def list_batches(self, request: Request) -> StreamResponse:
-        graph_db = self.db.get_graph_db(GraphName(request.match_info.get("graph_id", "resoto")))
+        graph_db = self.deps.db_access.get_graph_db(GraphName(request.match_info.get("graph_id", "resoto")))
         batch_updates = await graph_db.list_in_progress_updates()
         return web.json_response([b for b in batch_updates if b.get("is_batch")])
 
     async def commit_batch(self, request: Request) -> StreamResponse:
-        graph_db = self.db.get_graph_db(GraphName(request.match_info.get("graph_id", "resoto")))
+        graph_db = self.deps.db_access.get_graph_db(GraphName(request.match_info.get("graph_id", "resoto")))
         batch_id = request.match_info.get("batch_id", "some_existing")
         await graph_db.commit_batch_update(batch_id)
         return web.HTTPOk(body="Batch committed.")
 
     async def abort_batch(self, request: Request) -> StreamResponse:
-        graph_db = self.db.get_graph_db(GraphName(request.match_info.get("graph_id", "resoto")))
+        graph_db = self.deps.db_access.get_graph_db(GraphName(request.match_info.get("graph_id", "resoto")))
         batch_id = request.match_info.get("batch_id", "some_existing")
         await graph_db.abort_update(batch_id)
         return web.HTTPOk(body="Batch aborted.")
 
     async def graph_query_model_from_request(self, request: Request) -> Tuple[GraphDB, QueryModel]:
         section = section_of(request)
         query_string = await request.text()
         graph_name = GraphName(request.match_info.get("graph_id", "resoto"))
         raw_at = request.query.get("at")
         at = date_parser.parse(raw_at) if raw_at else None
 
         snapshot_name = None
 
         if at:
-            snapshot_name = await self.graph_manager.snapshot_at(time=at, graph_name=graph_name)
+            snapshot_name = await self.deps.graph_manager.snapshot_at(time=at, graph_name=graph_name)
             if not snapshot_name:
                 raise ValueError(f"No snapshot found for {graph_name} at {at}")
 
         graph_name = snapshot_name or graph_name
 
-        graph_db = self.db.get_graph_db(graph_name)
-        q = await self.query_parser.parse_query(query_string, section, **request.query)
-        m = await self.model_handler.load_model(graph_name)
+        graph_db = self.deps.db_access.get_graph_db(graph_name)
+        q = await self.deps.template_expander.parse_query(query_string, section, **request.query)
+        m = await self.deps.model_handler.load_model(graph_name)
         return graph_db, QueryModel(q, m)
 
     async def raw(self, request: Request) -> StreamResponse:
         graph_db, query_model = await self.graph_query_model_from_request(request)
         with_edges = request.query.get("edges") is not None
         query, bind_vars = await graph_db.to_query(query_model, with_edges)
         return web.json_response({"query": query, "bind_vars": bind_vars})
@@ -1035,15 +1003,15 @@
     async def serve_debug_ui(self, request: Request) -> FileResponse:
         """
         This is only for testing different versions of the UI during development.
         """
         commit = request.match_info.get("commit", "default")
         commit = commit[0:6] if len(commit) == 40 else commit  # shorten commit hash
         path = request.match_info.get("path", "index.html")
-        dir_path = self.config.run.temp_dir / "ui" / commit
+        dir_path = self.deps.config.run.temp_dir / "ui" / commit
         if not dir_path.exists():
             dir_path.mkdir(parents=True)
             async with self.session.get(f"https://cdn.some.engineering/resoto-ui/commits/{commit}.zip") as resp:
                 if resp.status != 200:
                     raise NotFoundError(f"Commit not found: {commit}")
                 body = await resp.read()
                 with zipfile.ZipFile(BytesIO(body)) as zip_ref:
@@ -1052,18 +1020,18 @@
         if not file.exists():
             raise NotFoundError(f"File not found: {path}")
         return FileResponse(file)
 
     async def wipe(self, request: Request) -> StreamResponse:
         graph_id = GraphName(request.match_info.get("graph_id", "resoto"))
         if "truncate" in request.query:
-            await self.db.get_graph_db(graph_id).wipe()
+            await self.deps.db_access.get_graph_db(graph_id).wipe()
             return web.HTTPOk(body="Graph truncated.")
         else:
-            await self.db.delete_graph(graph_id)
+            await self.deps.db_access.delete_graph(graph_id)
             return web.HTTPOk(body="Graph deleted.")
 
     async def cli_info(self, _: Request) -> StreamResponse:
         def cmd_json(cmd: CLICommand) -> Json:
             return {
                 "name": cmd.name,
                 "info": cmd.info(),
@@ -1086,23 +1054,27 @@
                 "name": cmd.name,
                 "info": cmd.description,
                 "help": cmd.readme,
                 "args": to_js(cmd.parameters, force_dict=True),
                 "source": True,
             }
 
-        commands = [cmd_json(cmd) for cmd in self.cli.direct_commands.values() if not isinstance(cmd, InternalPart)]
-        replacements = self.cli.replacements()
+        commands = [
+            cmd_json(cmd) for cmd in self.deps.cli.direct_commands.values() if not isinstance(cmd, InternalPart)
+        ]
+        replacements = self.deps.cli.replacements()
         return web.json_response(
             {
                 "commands": commands,
                 "replacements": replacements,
                 "alias_names": alias_names(),
-                "alias_templates": [alias_json(alias) for alias in self.cli.alias_templates.values()],
-                "infra_app_aliases": [infra_app_alias_json(alias) for alias in self.cli.infra_app_aliases.values()],
+                "alias_templates": [alias_json(alias) for alias in self.deps.cli.alias_templates.values()],
+                "infra_app_aliases": [
+                    infra_app_alias_json(alias) for alias in self.deps.cli.infra_app_aliases.values()
+                ],
             }
         )
 
     @staticmethod
     def cli_context_from_request(request: Request) -> CLIContext:
         try:
             columns = int(request.headers.get("Resoto-Shell-Columns", "120"))
@@ -1116,23 +1088,24 @@
             return CLIContext(
                 env=dict(request.query), console_renderer=ConsoleRenderer.default_renderer(), source="api"
             )
 
     async def evaluate(self, request: Request) -> StreamResponse:
         ctx = self.cli_context_from_request(request)
         command = await request.text()
-        parsed = await self.cli.evaluate_cli_command(command, ctx)
+        parsed = await self.deps.cli.evaluate_cli_command(command, ctx)
 
         def line_to_js(line: ParsedCommandLine) -> Json:
             parsed_commands = to_json(line.parsed_commands.commands)
             execute_commands = [{"cmd": part.command.name, "arg": part.arg} for part in line.executable_commands]
             return {"parsed": parsed_commands, "execute": execute_commands, "env": line.parsed_commands.env}
 
         return web.json_response([line_to_js(line) for line in parsed])
 
+    @timed("api", "execute")
     async def execute(self, request: Request) -> StreamResponse:
         temp_dir: Optional[str] = None
         try:
             ctx = self.cli_context_from_request(request)
             if request.content_type.startswith("text"):
                 command = (await request.text()).strip()
             elif request.content_type.startswith("multipart"):
@@ -1151,15 +1124,15 @@
                         while not part.at_eof():
                             writer.write(await part.read_chunk())
                 ctx = evolve(ctx, uploaded_files=files)
             else:
                 raise AttributeError(f"Not able to handle: {request.content_type}")
 
             # we want to eagerly evaluate the command, so that parse exceptions will throw directly here
-            parsed = await self.cli.evaluate_cli_command(command, ctx)
+            parsed = await self.deps.cli.evaluate_cli_command(command, ctx)
             return await self.execute_parsed(request, command, parsed, ctx)
         finally:
             if temp_dir:
                 shutil.rmtree(temp_dir)
 
     async def execute_parsed(
         self, request: Request, command: str, parsed: List[ParsedCommandLine], ctx: CLIContext
```

### Comparing `resotocore-3.6.0/resotocore/web/auth.py` & `resotocore-3.6.1/resotocore/web/auth.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/web/certificate_handler.py` & `resotocore-3.6.1/resotocore/web/certificate_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import Tuple, Optional, List, Union, Dict
 
 from arango.database import StandardDatabase
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey
 from cryptography.x509 import Certificate, CertificateSigningRequest
 
 from resotocore.core_config import CoreConfig, CertificateConfig
+from resotocore.service import Service
 from resotocore.types import Json
 from resotocore.util import Periodic
 from resotolib.utils import get_local_ip_addresses, get_local_hostnames
 from resotolib.x509 import (
     bootstrap_ca,
     gen_rsa_key,
     gen_csr,
@@ -32,15 +33,15 @@
     load_cert_from_file,
     write_ca_bundle,
 )
 
 log = logging.getLogger(__name__)
 
 
-class CertificateHandler:
+class CertificateHandler(Service):
     def __init__(self, config: CoreConfig, ca_key: RSAPrivateKey, ca_cert: Certificate, temp_dir: Path) -> None:
         self.config = config
         self._ca_key = ca_key
         self._ca_cert = ca_cert
         self._ca_cert_bytes = cert_to_bytes(ca_cert)
         self._ca_cert_fingerprint = cert_fingerprint(ca_cert)
         self._host_key, self._host_cert = self.__create_host_certificate(config.api.host_certificate, ca_key, ca_cert)
```

### Comparing `resotocore-3.6.0/resotocore/web/content_renderer.py` & `resotocore-3.6.1/resotocore/web/content_renderer.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/web/directives.py` & `resotocore-3.6.1/resotocore/web/directives.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/resotocore/web/tsdb.py` & `resotocore-3.6.1/resotocore/web/tsdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,29 +42,29 @@
             return True
         elif response.status >= 500:
             return True
         else:
             return False
 
     async def proxy_request(request: Request) -> StreamResponse:
-        if api_handler.config.api.tsdb_proxy_url:
+        if api_handler.deps.config.api.tsdb_proxy_url:
             in_headers = request.headers.copy()
             drop_request_specific_headers(in_headers)
-            url = f'{api_handler.config.api.tsdb_proxy_url}/{request.match_info["tail"]}'
+            url = f'{api_handler.deps.config.api.tsdb_proxy_url}/{request.match_info["tail"]}'
             max_retries = 5
 
             async def do_request(attempts_left: int) -> StreamResponse:
                 async with api_handler.session.request(
                     request.method,
                     url,
                     params=request.query,
                     headers=in_headers,
                     compress="deflate",
                     data=request.content,
-                    ssl=api_handler.cert_handler.client_context,
+                    ssl=api_handler.deps.cert_handler.client_context,
                 ) as cr:
                     try:
                         # in case of error: do we need to retry?
                         if cr.status >= 400 and attempts_left > 0 and should_be_retried(cr):
                             req_header = ", ".join(f"{k}={v}" for k, v in in_headers.items())
                             req_params = ", ".join(f"{k}={v}" for k, v in request.query.items())
                             req_body = await request.content.read()
```

### Comparing `resotocore-3.6.0/resotocore/worker_task_queue.py` & `resotocore-3.6.1/resotocore/worker_task_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from collections import defaultdict
 from contextlib import asynccontextmanager
 from attrs import define, field
 from datetime import timedelta, datetime
 from functools import reduce
 from typing import Any, Optional, AsyncGenerator, Dict, List
 
+from resotocore.service import Service
 from resotocore.types import Json, JsonElement
 from resotocore.util import utc, Periodic, set_future_result
 from resotocore.ids import TaskId, WorkerId
 
 log = logging.getLogger(__name__)
 
 
@@ -76,15 +77,15 @@
     task: WorkerTaskDescription
     queue: Queue[WorkerTask]
 
     def __len__(self) -> int:
         return self.queue.qsize()
 
 
-class WorkerTaskQueue:
+class WorkerTaskQueue(Service):
     """
     This class implements a simple task queue.
     """
 
     def __init__(self) -> None:
         # key is the task_name, value is the list of worker subscriptions
         self.worker_by_task_name: Dict[str, List[WorkerTaskSubscription]] = defaultdict(list)
```

### Comparing `resotocore-3.6.0/resotocore.egg-info/PKG-INFO` & `resotocore-3.6.1/resotocore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotocore
-Version: 3.6.0
+Version: 3.6.1
 Summary: Keeps all the things.
 Author: Some Engineering Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `resotocore-3.6.0/resotocore.egg-info/SOURCES.txt` & `resotocore-3.6.1/resotocore.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 resotocore/constants.py
 resotocore/core_config.py
 resotocore/dependencies.py
 resotocore/error.py
 resotocore/ids.py
 resotocore/message_bus.py
 resotocore/metrics.py
+resotocore/service.py
+resotocore/system_start.py
 resotocore/types.py
 resotocore/util.py
 resotocore/validator.py
 resotocore/worker_task_queue.py
 resotocore.egg-info/PKG-INFO
 resotocore.egg-info/SOURCES.txt
 resotocore.egg-info/dependency_links.txt
@@ -30,15 +32,14 @@
 resotocore/action_handlers/merge_outer_edge_handler.py
 resotocore/analytics/__init__.py
 resotocore/analytics/posthog.py
 resotocore/analytics/recurrent_events.py
 resotocore/cli/__init__.py
 resotocore/cli/cli.py
 resotocore/cli/command.py
-resotocore/cli/dependencies.py
 resotocore/cli/model.py
 resotocore/cli/tip_of_the_day.py
 resotocore/config/__init__.py
 resotocore/config/config_handler_service.py
 resotocore/config/config_override_service.py
 resotocore/config/core_config_handler.py
 resotocore/db/__init__.py
@@ -55,14 +56,15 @@
 resotocore/db/model.py
 resotocore/db/modeldb.py
 resotocore/db/packagedb.py
 resotocore/db/runningtaskdb.py
 resotocore/db/subscriberdb.py
 resotocore/db/system_data_db.py
 resotocore/db/templatedb.py
+resotocore/db/usagedb.py
 resotocore/graph_manager/__init__.py
 resotocore/graph_manager/graph_manager.py
 resotocore/infra_apps/__init__.py
 resotocore/infra_apps/local_runtime.py
 resotocore/infra_apps/manifest.py
 resotocore/infra_apps/package_manager.py
 resotocore/infra_apps/runtime.py
@@ -614,28 +616,28 @@
 resotocore/static/report/checks/aws/aws_s3.json
 resotocore/task/__init__.py
 resotocore/task/job_handler.py
 resotocore/task/model.py
 resotocore/task/scheduler.py
 resotocore/task/start_workflow_on_first_subscriber.py
 resotocore/task/subscribers.py
+resotocore/task/task_dependencies.py
 resotocore/task/task_description.py
 resotocore/task/task_handler.py
 resotocore/templates/base.html
 resotocore/templates/create_first_user.html
 resotocore/templates/login.html
 resotocore/user/__init__.py
 resotocore/user/user_management.py
 resotocore/web/__init__.py
 resotocore/web/api.py
 resotocore/web/auth.py
 resotocore/web/certificate_handler.py
 resotocore/web/content_renderer.py
 resotocore/web/directives.py
-resotocore/web/service.py
 resotocore/web/tsdb.py
 tests/__init__.py
 tests/resotocore/__init__.py
 tests/resotocore/conftest.py
 tests/resotocore/console_renderer_test.py
 tests/resotocore/core_config_test.py
 tests/resotocore/dependencies_test.py
```

### Comparing `resotocore-3.6.0/tests/resotocore/__init__.py` & `resotocore-3.6.1/tests/resotocore/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/analytics/posthog_test.py` & `resotocore-3.6.1/tests/resotocore/analytics/posthog_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/analytics/recurrent_events_test.py` & `resotocore-3.6.1/tests/resotocore/analytics/recurrent_events_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/cli/cli_test.py` & `resotocore-3.6.1/tests/resotocore/cli/cli_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/cli/command_test.py` & `resotocore-3.6.1/tests/resotocore/cli/command_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from attrs import evolve
 from pytest import fixture
 
 from resotocore import version
 from resotocore.cli import is_node
 from resotocore.cli.cli import CLIService
 from resotocore.cli.command import HttpCommand, JqCommand, AggregateCommand, all_commands
-from resotocore.cli.dependencies import CLIDependencies
+from resotocore.dependencies import Dependencies
 from resotocore.cli.model import CLIContext, WorkerCustomCommand, CLI, FilePath
 from resotocore.cli.tip_of_the_day import generic_tips
 from resotocore.console_renderer import ConsoleRenderer, ConsoleColorSystem
 from resotocore.db.graphdb import ArangoGraphDB
 from resotocore.db.jobdb import JobDb
 from resotocore.error import CLIParseError
 from resotocore.graph_manager.graph_manager import GraphManager
@@ -48,17 +48,17 @@
 
 @fixture
 def json_source() -> str:
     nums = ",".join([f'{{ "num": {a}, "inner": {{"num": {a%10}}}}}' for a in range(0, 100)])
     return "json [" + nums + "," + nums + "]"
 
 
-def test_known_category(cli_deps: CLIDependencies) -> None:
+def test_known_category(dependencies: Dependencies) -> None:
     allowed_categories = {"search", "format", "action", "setup", "misc"}
-    for cmd in all_commands(cli_deps):
+    for cmd in all_commands(dependencies):
         assert cmd.category in allowed_categories, f"Unknown category {cmd.category} for command {cmd.name}"
 
 
 @pytest.mark.asyncio
 async def test_echo_source(cli: CLI) -> None:
     # no arg passed to json
     result = await cli.execute_cli_command("echo", stream.list)
@@ -263,15 +263,15 @@
     result = await cli.execute_cli_command('search is("foo") | protect | dump', stream.list)
     assert len(result[0]) == 11
     for elem in result[0]:
         assert {"protected": True}.items() <= elem["metadata"].items()
 
 
 @pytest.mark.asyncio
-async def test_list_sink(cli: CLI, cli_deps: CLIDependencies) -> None:
+async def test_list_sink(cli: CLI, dependencies: Dependencies) -> None:
     result = await cli.execute_cli_command("json [1,2,3] | dump", stream.list)
     assert result == [[1, 2, 3]]
 
 
 @pytest.mark.asyncio
 async def test_flat_sink(cli: CLI) -> None:
     parsed = await cli.evaluate_cli_command("json [1,2,3] | dump; json [4,5,6] | dump; json [7,8,9] | dump")
@@ -310,15 +310,15 @@
 
 @pytest.mark.asyncio
 async def test_workflows_command(cli: CLIService, task_handler: TaskHandlerService, test_workflow: Workflow) -> None:
     async def execute(cmd: str) -> List[JsonElement]:
         ctx = CLIContext(cli.cli_env)
         return (await cli.execute_cli_command(cmd, stream.list, ctx))[0]  # type: ignore
 
-    assert await execute("workflows list") == ["sleep_workflow", "test_workflow"]
+    assert await execute("workflows list") == ["sleep_workflow", "wait_for_collect_done", "test_workflow"]
     assert await execute("workflows show test_workflow") == [to_js(test_workflow)]
     wf = await execute("workflows run test_workflow")
     assert wf[0].startswith("Workflow test_workflow started with id")  # type: ignore
     assert len(await execute("workflows running")) == 1
 
     # executing an already running workflow will give a specific message
     await execute("workflows run sleep_workflow")
@@ -984,21 +984,21 @@
     assert await history_count(f"history --change node_deleted") == 0
     assert await history_count(f"history is(foo)") == 11
     # combine all selectors
     assert await history_count(f"history --after 5m --before {five_min_later} --change node_created is(foo)") == 11
 
 
 @pytest.mark.asyncio
-async def test_aggregate(cli_deps: CLIDependencies) -> None:
+async def test_aggregate(dependencies: Dependencies) -> None:
     in_stream = stream.iterate(
         [{"a": 1, "b": 1, "c": 1}, {"a": 2, "b": 1, "c": 1}, {"a": 3, "b": 2, "c": 1}, {"a": 4, "b": 2, "c": 1}]
     )
 
     async def aggregate(agg_str: str) -> List[Json]:
-        res = AggregateCommand(cli_deps).parse(agg_str)
+        res = AggregateCommand(dependencies).parse(agg_str)
         async with (await res.flow(in_stream)).stream() as flow:
             return [s async for s in flow]
 
     assert await aggregate("b as bla, c, r.d.f.name: sum(1) as count, min(a) as min, max(a) as max") == [
         {"group": {"bla": 1, "c": 1, "r.d.f.name": None}, "count": 2, "min": 1, "max": 2},
         {"group": {"bla": 2, "c": 1, "r.d.f.name": None}, "count": 2, "min": 3, "max": 4},
     ]
```

### Comparing `resotocore-3.6.0/tests/resotocore/cli/model_test.py` & `resotocore-3.6.1/tests/resotocore/cli/model_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/config/config_handler_service_test.py` & `resotocore-3.6.1/tests/resotocore/config/config_handler_service_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/config/config_override_service_test.py` & `resotocore-3.6.1/tests/resotocore/config/config_override_service_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/config/core_config_handler_test.py` & `resotocore-3.6.1/tests/resotocore/config/core_config_handler_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 from resotocore.core_config import (
     ResotoCoreConfigId,
     ResotoCoreRoot,
     ResotoCoreCommandsRoot,
     CustomCommandsConfig,
     ResotoCoreSnapshotsRoot,
 )
-from resotocore.dependencies import empty_config
+from resotocore.system_start import empty_config
 from resotocore.message_bus import MessageBus, CoreMessage
 from resotocore.ids import ConfigId
-from resotocore.types import Json
 
 
 @mark.asyncio
 async def test_model_updated_on_start(core_config_handler: CoreConfigHandler, config_handler: ConfigHandler) -> None:
     try:
         default_model = await config_handler.get_configs_model()
         await core_config_handler.start()
```

### Comparing `resotocore-3.6.0/tests/resotocore/conftest.py` & `resotocore-3.6.1/tests/resotocore/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,35 +4,36 @@
 from asyncio import Queue
 from collections import defaultdict
 from contextlib import suppress
 from datetime import timedelta
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from types import SimpleNamespace
-from typing import AsyncGenerator, Iterator, Dict, Any, Generator
+from typing import AsyncGenerator, Iterator, Dict, Any, Generator, Callable
 from typing import List, Optional
 from typing import Tuple, AsyncIterator, cast
 
 from aiohttp import ClientSession
 from aiohttp.hdrs import METH_ANY
 from aiohttp.test_utils import TestServer
 from aiohttp.web import Request, Response, Application, route
 from arango.client import ArangoClient
 from arango.database import StandardDatabase
+from attr import evolve
 from pytest import fixture
 from rich.console import Console
 
 from resotocore.action_handlers.merge_outer_edge_handler import MergeOuterEdgesHandler
 from resotocore.analytics import AnalyticsEventSender, InMemoryEventSender, NoEventSender
 from resotocore.cli.cli import CLIService
 from resotocore.cli.command import (
     alias_names,
     all_commands,
 )
-from resotocore.cli.dependencies import CLIDependencies
+from resotocore.dependencies import Dependencies
 from resotocore.config import ConfigHandler, ConfigEntity, ConfigValidation, ConfigOverride
 from resotocore.config.config_handler_service import ConfigHandlerService
 from resotocore.config.core_config_handler import CoreConfigHandler
 from resotocore.console_renderer import ConsoleRenderer, ConsoleColorSystem
 from resotocore.core_config import (
     GraphUpdateConfig,
     CoreConfig,
@@ -48,35 +49,37 @@
 from resotocore.db.db_access import DbAccess
 from resotocore.db.graphdb import ArangoGraphDB, EventGraphDB
 from resotocore.db.jobdb import JobDb
 from resotocore.db.packagedb import PackageEntityDb, app_package_entity_db
 from resotocore.db.runningtaskdb import RunningTaskDb
 from resotocore.db.system_data_db import SystemDataDb
 from resotocore.graph_manager.graph_manager import GraphManager
-from resotocore.dependencies import empty_config, parse_args
+from resotocore.system_start import empty_config, parse_args
 from resotocore.ids import SubscriberId, WorkerId, TaskDescriptorId, ConfigId, GraphName
 from resotocore.infra_apps.local_runtime import LocalResotocoreAppRuntime
 from resotocore.infra_apps.package_manager import PackageManager
 from resotocore.message_bus import (
     MessageBus,
     Message,
     Event,
     Action,
     ActionDone,
 )
 from resotocore.model.adjust_node import NoAdjust
+from resotocore.model.db_updater import GraphMerger
 from resotocore.model.graph_access import EdgeTypes, Section
 from resotocore.model.model import Model, Kind, ComplexKind, Property, SyntheticProperty, StringKind
 from resotocore.model.resolve_in_graph import GraphResolver
 from resotocore.model.resolve_in_graph import NodePath
 from resotocore.model.typed_model import to_js
 from resotocore.query.template_expander import TemplateExpander
 from resotocore.report import BenchmarkConfigPrefix, CheckConfigPrefix, Benchmark
 from resotocore.report.inspector_service import InspectorService
 from resotocore.report.report_config import BenchmarkConfig
+from resotocore.task.task_dependencies import TaskDependencies
 from resotocore.task.model import Subscriber, Subscription
 from resotocore.task.scheduler import Scheduler
 from resotocore.task.subscribers import SubscriptionHandler
 from resotocore.task.task_description import (
     Step,
     PerformAction,
     WaitForEvent,
@@ -85,14 +88,15 @@
     EventTrigger,
     RunningTask,
     ExecuteCommand,
     TaskSurpassBehaviour,
     Job,
     Workflow,
     TimeTrigger,
+    WaitForCollectDone,
 )
 from resotocore.task.task_handler import TaskHandlerService
 from resotocore.types import Json
 from resotocore.user import UserManagement
 from resotocore.user.user_management import UserManagementService
 from resotocore.util import value_in_path, uuid_str, utc
 from resotocore.web.certificate_handler import CertificateHandler
@@ -479,30 +483,30 @@
 async def core_config_handler_started(core_config_handler: CoreConfigHandler) -> AsyncIterator[CoreConfigHandler]:
     await core_config_handler.start()
     yield core_config_handler
     await core_config_handler.stop()
 
 
 @fixture
-async def cli_deps(
+async def dependencies(
     filled_graph_db: ArangoGraphDB,
     message_bus: MessageBus,
     event_sender: InMemoryEventSender,
     foo_model: Model,
     task_queue: WorkerTaskQueue,
     worker: Tuple[WorkerTaskDescription, WorkerTaskDescription, WorkerTaskDescription],
     expander: TemplateExpander,
     config_handler: ConfigHandler,
     cert_handler: CertificateHandler,
     user_management: UserManagement,
-) -> AsyncIterator[CLIDependencies]:
+) -> AsyncIterator[Dependencies]:
     db_access = DbAccess(filled_graph_db.db.db, event_sender, NoAdjust(), empty_config())
     model_handler = ModelHandlerStatic(foo_model)
     config = empty_config(["--graphdb-database", "test", "--graphdb-username", "test", "--graphdb-password", "test"])
-    deps = CLIDependencies(
+    deps = Dependencies(
         message_bus=message_bus,
         event_sender=event_sender,
         db_access=db_access,
         model_handler=model_handler,
         worker_task_queue=task_queue,
         config=config,
         template_expander=expander,
@@ -514,17 +518,30 @@
     await db_access.start()
     yield deps
     await db_access.stop()
     await deps.stop()
 
 
 @fixture
-def cli(cli_deps: CLIDependencies) -> CLIService:
+async def graph_merger(
+    foo_model: Model, event_sender: AnalyticsEventSender, default_config: CoreConfig, message_bus: MessageBus
+) -> GraphMerger:
+    model_handler = ModelHandlerStatic(foo_model)
+    return GraphMerger(model_handler, event_sender, default_config, message_bus)
+
+
+@fixture
+async def task_dependencies(graph_merger: GraphMerger, subscription_handler: SubscriptionHandler) -> TaskDependencies:
+    return TaskDependencies(graph_merger, subscription_handler.subscribers_by_event)
+
+
+@fixture
+def cli(dependencies: Dependencies) -> CLIService:
     env = {"graph": "ns", "section": "reported"}
-    return CLIService(cli_deps, all_commands(cli_deps), env, alias_names())
+    return CLIService(dependencies, all_commands(dependencies), env, alias_names())
 
 
 @fixture
 async def inspector_service(cli: CLIService) -> InspectorService:
     async with InspectorService(cli) as service:
         cli.dependencies.lookup["inspector"] = service
         return service
@@ -636,15 +653,25 @@
     return [
         Workflow(
             TaskDescriptorId("sleep_workflow"),
             "Speakable name of workflow",
             [Step("sleep", ExecuteCommand("sleep 0.1"), timedelta(seconds=10))],
             triggers=[],
             on_surpass=TaskSurpassBehaviour.Wait,
-        )
+        ),
+        Workflow(
+            TaskDescriptorId("wait_for_collect_done"),
+            "Wait for collect",
+            [
+                Step("wait", WaitForEvent("collected", {}), timedelta(seconds=10)),
+                Step("wait_for_collect_done", WaitForCollectDone(), timedelta(seconds=10)),
+            ],
+            triggers=[],
+            on_surpass=TaskSurpassBehaviour.Wait,
+        ),
     ]
 
 
 @fixture
 def test_wait_workflow() -> Workflow:
     return Workflow(
         TaskDescriptorId("test_workflow"),
@@ -658,24 +685,25 @@
         ],
         [EventTrigger("start me up")],
     )
 
 
 @fixture
 def workflow_instance(
+    task_dependencies: TaskDependencies,
     test_wait_workflow: Workflow,
 ) -> Tuple[RunningTask, Subscriber, Subscriber, Dict[str, List[Subscriber]]]:
     td = timedelta(seconds=100)
     sub1 = Subscription("start_collect", True, td)
     sub2 = Subscription("collect", True, td)
     sub3 = Subscription("collect_done", True, td)
     s1 = Subscriber.from_list(SubscriberId("s1"), [sub1, sub2, sub3])
     s2 = Subscriber.from_list(SubscriberId("s2"), [sub2, sub3])
     subscriptions = {"start_collect": [s1], "collect": [s1, s2], "collect_done": [s1, s2]}
-    w, _ = RunningTask.empty(test_wait_workflow, lambda: subscriptions)
+    w, _ = RunningTask.empty(test_wait_workflow, evolve(task_dependencies, subscribers_by_event=lambda: subscriptions))
     w.received_messages = [
         Action("start_collect", w.id, "start"),
         ActionDone("start_collect", w.id, "start", s1.id),
         ActionDone("start_collect", w.id, "start", s2.id),
         Event("godot", {"a": 1, "b": 2}),
         Action("collect", w.id, "collect"),
         ActionDone("collect", w.id, "collect", s1.id),
@@ -694,21 +722,22 @@
 @fixture
 async def task_handler(
     running_task_db: RunningTaskDb,
     job_db: JobDb,
     message_bus: MessageBus,
     event_sender: AnalyticsEventSender,
     subscription_handler: SubscriptionHandler,
+    graph_merger: GraphMerger,
     cli: CLIService,
     test_workflow: Workflow,
     additional_workflows: List[Workflow],
 ) -> AsyncGenerator[TaskHandlerService, None]:
     config = empty_config()
     task_handler = TaskHandlerService(
-        running_task_db, job_db, message_bus, event_sender, subscription_handler, Scheduler(), cli, config
+        running_task_db, job_db, message_bus, event_sender, subscription_handler, graph_merger, Scheduler(), cli, config
     )
     task_handler.task_descriptions = additional_workflows + [test_workflow]
     cli.dependencies.lookup["task_handler"] = task_handler
     async with task_handler:
         yield task_handler
 
 
@@ -776,7 +805,19 @@
     with suppress(Exception):
         test_db.insert_document(
             "system_data", {"_key": "ca", "key": "private_key", "certificate": "some cert"}, overwrite=False
         )
     async_db = AsyncArangoDB(test_db)
     yield SystemDataDb(async_db)
     test_db.collection("system_data").delete({"_key": "ca"})
+
+
+async def eventually(
+    predicate: Callable[[], bool],
+    timeout: timedelta = timedelta(seconds=5),
+    interval: timedelta = timedelta(seconds=0.1),
+) -> None:
+    async def wait_for_condition() -> None:
+        while not predicate():
+            await asyncio.sleep(interval.total_seconds())
+
+    await asyncio.wait_for(wait_for_condition(), timeout.total_seconds())
```

### Comparing `resotocore-3.6.0/tests/resotocore/console_renderer_test.py` & `resotocore-3.6.1/tests/resotocore/console_renderer_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/core_config_test.py` & `resotocore-3.6.1/tests/resotocore/core_config_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     migrate_core_config,
     migrate_command_config,
     CustomCommandsConfig,
     alias_templates,
     ResotoCoreCommandsRoot,
     ResotoCoreConfigId,
 )
-from resotocore.dependencies import parse_args
+from resotocore.system_start import parse_args
 from resotocore.model.typed_model import to_js, from_js
 from resotocore.types import Json
 from resotocore.util import value_in_path
 
 
 def test_parse_empty(default_config: CoreConfig) -> None:
     result = parse_config(parse_args(["--analytics-opt-out"]), {}, lambda: None)
@@ -200,15 +200,20 @@
                         "info": "Test command",
                         "name": "test",
                         "parameters": [{"name": "test", "default": "test argument", "description": "easy"}],
                         "template": "do something",
                     }
                 ],
             },
-            "graph_update": {"abort_after_seconds": 1234, "merge_max_wait_time_seconds": 4321, "keep_history": True},
+            "graph_update": {
+                "abort_after_seconds": 1234,
+                "merge_max_wait_time_seconds": 4321,
+                "keep_history": True,
+                "parallel_imports": 5,
+            },
             "runtime": {
                 "usage_metrics": False,
                 "debug": True,
                 "log_level": "WARN",
                 "plantuml_server": "https://foo",
                 "start_collect_on_subscriber_connect": True,
             },
```

### Comparing `resotocore-3.6.0/tests/resotocore/db/arango_query_test.py` & `resotocore-3.6.1/tests/resotocore/db/arango_query_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -121,7 +121,26 @@
     query = "is(foo) and inner[1].{name=true and inner[0].name==true}"
     aql, bind_vars = to_query(graph_db, QueryModel(parse_query(query).on_section("reported"), foo_model))
     assert aql == (
         "LET filter0 = (FOR m0 in `ns` FILTER (@b0 IN m0.kinds) and "
         "((m0.reported.inner[1].name == @b1) and (m0.reported.inner[1].inner[0].name == @b2))  RETURN m0) "
         'FOR result in filter0 RETURN UNSET(result, ["flat"])'
     )
+
+
+def test_usage(foo_model: Model, graph_db: GraphDB) -> None:
+    q, b = to_query(graph_db, QueryModel(parse_query("with_usage(3w, cpu, mem) is(foo)"), foo_model))
+    assert q == (
+        "LET filter0 = (FOR m0 in `ns` FILTER @b0 IN m0.kinds  RETURN m0)\n"
+        "let with_usage0 = (\n"
+        "    for r in filter0\n"
+        "        let resource=r\n"
+        "        let resource_usage = first(\n"
+        "            for m in ns_usage\n"
+        "            filter m.at>=@b1 and m.at<=@b2 and m.id==r._key\n"
+        "            collect aggregate cpu_min = MIN(m.v.cpu.min), cpu_avg = AVG(m.v.cpu.avg), cpu_max = MAX(m.v.cpu.max), mem_min = MIN(m.v.mem.min), mem_avg = AVG(m.v.mem.avg), mem_max = MAX(m.v.mem.max), count = sum(1)\n"  # noqa: E501
+        "            return {usage:{cpu: {min: cpu_min, avg: cpu_avg, max: cpu_max},mem: {min: mem_min, avg: mem_avg, max: mem_max},entries:count,start:@b3,duration:@b4}}\n"  # noqa: E501
+        "        )\n"
+        "        return resource_usage.usage.entries ? merge(resource, resource_usage) : resource\n"
+        ")\n"
+        ' FOR result in with_usage0 RETURN UNSET(result, ["flat"])'
+    )
```

### Comparing `resotocore-3.6.0/tests/resotocore/db/arangodb_functions_test.py` & `resotocore-3.6.1/tests/resotocore/db/arangodb_functions_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/db/async_arangodb_test.py` & `resotocore-3.6.1/tests/resotocore/db/async_arangodb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/db/configdb_test.py` & `resotocore-3.6.1/tests/resotocore/db/configdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/db/db_access_test.py` & `resotocore-3.6.1/tests/resotocore/db/db_access_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import timedelta
 
 from arango.client import ArangoClient
 from arango.database import StandardDatabase
 
 from resotocore.analytics import NoEventSender
 from resotocore.db.db_access import DbAccess
-from resotocore.dependencies import parse_args, empty_config
+from resotocore.system_start import parse_args, empty_config
 from resotocore.model.adjust_node import NoAdjust
 from resotocore.ids import GraphName
 
 import pytest
 
 
 def test_already_existing(test_db: StandardDatabase) -> None:
```

### Comparing `resotocore-3.6.0/tests/resotocore/db/entitydb.py` & `resotocore-3.6.1/tests/resotocore/db/entitydb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/db/graphdb_test.py` & `resotocore-3.6.1/tests/resotocore/db/graphdb_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from resotocore.analytics import CoreEvent, InMemoryEventSender
 from resotocore.db.graphdb import ArangoGraphDB, GraphDB, EventGraphDB, HistoryChange
 from resotocore.db.model import QueryModel, GraphUpdate
 from resotocore.db.db_access import DbAccess
 from resotocore.error import ConflictingChangeInProgress, NoSuchChangeError, InvalidBatchUpdate
 from resotocore.ids import NodeId, GraphName
 from resotocore.model.graph_access import GraphAccess, EdgeTypes, Section
-from resotocore.model.model import Model
+from resotocore.model.model import Model, UsageDatapoint, UsageMetricValues
 from resotocore.model.typed_model import from_js, to_js
 from resotocore.query.model import Query, P, Navigation
 from resotocore.query.query_parser import parse_query
 from resotocore.types import JsonElement, EdgeType
 from resotocore.util import AccessJson, utc, value_in_path, AccessNone
 
 
@@ -175,46 +175,69 @@
 
 @mark.asyncio
 async def test_update_merge_batched(graph_db: ArangoGraphDB, foo_model: Model, test_db: StandardDatabase) -> None:
     md = foo_model
     await graph_db.wipe()
     batch_id = "".join(SystemRandom().choice(string.ascii_letters) for _ in range(12))
     g = create_graph("yes or no")
+    await graph_db.insert_usage_data(
+        [
+            UsageDatapoint("0", at=100, v={"cpu": UsageMetricValues(42, 42, 42)}, change_id=batch_id),
+            UsageDatapoint("0", at=101, v={"cpu": UsageMetricValues(43, 43, 43)}, change_id="foo"),
+        ]
+    )
 
     # empty database: all changes are written to a temp table
     assert await graph_db.merge_graph(g, foo_model, batch_id, True) == (
         ["collector"],
         GraphUpdate(112, 1, 0, 212, 0, 0),
     )
     assert len((await load_graph(graph_db, md)).nodes) == 0
     # not allowed to commit an unknown batch
     with raises(NoSuchChangeError):
         await graph_db.commit_batch_update("does_not_exist")
     # commit the batch and see the changes reflected in the database
     await graph_db.commit_batch_update(batch_id)
-    assert len((await load_graph(graph_db, md)).nodes) == 111
+    updated_graph = await load_graph(graph_db, md)
+    assert len(updated_graph.nodes) == 111
     # ensure that all temp tables are removed
     assert len(list(filter(lambda c: c["name"].startswith("temp_"), cast(List[Json], test_db.collections())))) == 0
+    # ensure the usage is there
+    n = await graph_db.get_node(foo_model, NodeId("0")) or {}
+    assert n.get("usage", {}).get("cpu") == {"min": 42, "avg": 42, "max": 42}
     # create a new batch that gets aborted: make sure all temp tables are gone
     batch_id = "will_be_aborted"
     await graph_db.merge_graph(g, foo_model, batch_id, True)
     await graph_db.abort_update(batch_id)
     assert len(list(filter(lambda c: c["name"].startswith("temp_"), cast(List[Json], test_db.collections())))) == 0
 
 
 @mark.asyncio
 async def test_merge_graph(graph_db: ArangoGraphDB, foo_model: Model) -> None:
     await graph_db.wipe()
 
     def create(txt: str, width: int = 10) -> MultiDiGraph:
         return create_graph(txt, width=width)
 
+    await graph_db.insert_usage_data(
+        [
+            UsageDatapoint("0", at=100, v={"cpu": UsageMetricValues(42, 42, 42)}, change_id="foo"),
+            UsageDatapoint("0", at=101, v={"cpu": UsageMetricValues(43, 43, 43)}, change_id="bar"),
+        ]
+    )
+
     p = ["collector"]
     # empty database: all nodes and all edges have to be inserted, the root node is updated and the link to root added
-    assert await graph_db.merge_graph(create("yes or no"), foo_model) == (p, GraphUpdate(112, 1, 0, 212, 0, 0))
+    assert await graph_db.merge_graph(create("yes or no"), foo_model, maybe_change_id="foo") == (
+        p,
+        GraphUpdate(112, 1, 0, 212, 0, 0),
+    )
+    # check the usage
+    n = await graph_db.get_node(foo_model, NodeId("0")) or {}
+    assert n.get("usage", {}).get("cpu") == {"min": 42, "avg": 42, "max": 42}
     # exactly the same graph is updated: expect no changes
     assert await graph_db.merge_graph(create("yes or no"), foo_model) == (p, GraphUpdate(0, 0, 0, 0, 0, 0))
     # all bla entries have different content: expect 100 node updates, but no inserts or deletions
     assert await graph_db.merge_graph(create("maybe"), foo_model) == (p, GraphUpdate(0, 100, 0, 0, 0, 0))
     # the width of the graph is reduced: expect nodes and edges to be removed
     assert await graph_db.merge_graph(create("maybe", width=5), foo_model) == (p, GraphUpdate(0, 0, 80, 0, 0, 155))
     # going back to the previous graph: the same amount of nodes and edges is inserted
@@ -619,19 +642,41 @@
         existing_delete_edge_ids = {a["_key"] for a in await db.all(f"{original_db_name}_delete")}
         copy_delete_edge_ids = {a["_key"] for a in await db.all(f"{copy_db_name}_delete")}
         assert existing_delete_edge_ids == copy_delete_edge_ids
 
     await validate(graph_db.name, copy_db.name)
 
     # check snapshots
-    snapshot_db_name = GraphName("snapshot_" + graph_db.name)
+    snapshot_db_name = GraphName("snapshot-" + graph_db.name)
     snapshot_db = await graph_db.copy_graph(snapshot_db_name, to_snapshot=True)
     assert snapshot_db.name == snapshot_db_name
     await validate(graph_db.name, snapshot_db.name)
 
+    # clean up
+    await snapshot_db.wipe()
+
+
+@mark.asyncio
+async def test_no_snapshot_usage(graph_db: ArangoGraphDB, foo_model: Model, db_access: DbAccess) -> None:
+    await graph_db.wipe()
+    await db_access.delete_graph(GraphName("snapshot-" + graph_db.name))
+
+    snapshot_db_name = GraphName("snapshot-" + graph_db.name)
+    snapshot_db = await graph_db.copy_graph(snapshot_db_name, to_snapshot=True)
+
+    with raises(ValueError) as ex:
+        await snapshot_db.insert_usage_data(
+            [UsageDatapoint("foo", 42, "foo", {"cpu": UsageMetricValues(0.42, 0.42, 0.42)})]
+        )
+
+    assert str(ex.value) == "Cannot insert usage data into a snapshot graph"
+
+    # clean up
+    await snapshot_db.wipe()
+
 
 def test_render_metadata_section(foo_model: Model) -> None:
     printer = ArangoGraphDB.document_to_instance_fn(foo_model)
     out = printer({"_key": "1", "reported": {"kind": "foo"}, "metadata": {"exported_at": "2023-03-06T19:37:51Z"}})
     assert "exported_age" in out["metadata"]  # exported_age is not part of the document, but should be added
```

### Comparing `resotocore-3.6.0/tests/resotocore/db/jobdb_test.py` & `resotocore-3.6.1/tests/resotocore/db/jobdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/db/modeldb_test.py` & `resotocore-3.6.1/tests/resotocore/db/modeldb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/db/runningtaskdb_test.py` & `resotocore-3.6.1/tests/resotocore/db/runningtaskdb_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,28 @@
 async def test_load_running(running_task_db: RunningTaskDb, instances: List[RunningTaskData]) -> None:
     await running_task_db.update_many(instances)
     not_done = list(filter(lambda x: not x.done, instances))
     assert not_done.sort() == [sub async for sub in running_task_db.all_running()].sort()
 
 
 @mark.asyncio
+async def test_last(running_task_db: RunningTaskDb, instances: List[RunningTaskData]) -> None:
+    await running_task_db.update_many(instances)
+    running_tasks = list(filter(lambda x: x.done, instances))
+    running_tasks.sort(key=lambda x: x.task_started_at, reverse=True)
+    done_task = next(iter(running_tasks), None)
+    assert done_task
+    last_done = await running_task_db.last(descriptor_id=done_task.task_descriptor_id)
+    assert last_done
+    assert done_task.id == last_done.id
+
+    assert await running_task_db.last()
+
+
+@mark.asyncio
 async def test_load(running_task_db: RunningTaskDb, instances: List[RunningTaskData]) -> None:
     await running_task_db.update_many(instances)
     loaded = [sub async for sub in running_task_db.all()]
     assert instances.sort() == loaded.sort()
 
 
 @mark.asyncio
```

### Comparing `resotocore-3.6.0/tests/resotocore/db/subscriberdb_test.py` & `resotocore-3.6.1/tests/resotocore/db/subscriberdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/db/system_data_db_test.py` & `resotocore-3.6.1/tests/resotocore/db/system_data_db_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/db/templatedb_test.py` & `resotocore-3.6.1/tests/resotocore/db/templatedb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/dependencies_test.py` & `resotocore-3.6.1/tests/resotocore/dependencies_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Tuple, List
 
-from resotocore.dependencies import parse_args
+from resotocore.system_start import parse_args
 from resotocore.types import JsonElement
 
 
 def test_parse_override() -> None:
     def parse(args: str) -> List[Tuple[str, JsonElement]]:
         return parse_args(args.split()).config_override  # type: ignore
```

### Comparing `resotocore-3.6.0/tests/resotocore/graph_manager/graph_manager_test.py` & `resotocore-3.6.1/tests/resotocore/graph_manager/graph_manager_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/hypothesis_extension.py` & `resotocore-3.6.1/tests/resotocore/hypothesis_extension.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import string
+from datetime import datetime
 from typing import TypeVar, Callable, Any, cast, Optional, List, Generator
 
 from aiostream import stream
 from aiostream.core import Stream
 from hypothesis.strategies import (
     SearchStrategy,
     just,
@@ -42,14 +43,16 @@
         return self.draw(optional(st))
 
 
 any_ws_digits_string = text(alphabet=string.ascii_letters + string.whitespace + string.digits, min_size=0, max_size=10)
 any_string = text(alphabet=string.ascii_letters, min_size=3, max_size=10)
 kind_gen = sampled_from(["volume", "instance", "load_balancer", "volume_type"])
 
+any_datetime = integers(min_value=0, max_value=1688108028).map(lambda x: datetime.fromtimestamp(x))
+
 
 @composite
 def json_element_gen(ud: UD) -> JsonElement:
     return cast(JsonElement, ud(json_object_gen | json_simple_element_gen | json_array_gen))
 
 
 json_simple_element_gen = any_ws_digits_string | booleans() | integers(min_value=0, max_value=100000) | just(None)
```

### Comparing `resotocore-3.6.0/tests/resotocore/infra_apps/local_runtime_test.py` & `resotocore-3.6.1/tests/resotocore/infra_apps/local_runtime_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/infra_apps/package_manager_test.py` & `resotocore-3.6.1/tests/resotocore/infra_apps/package_manager_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/message_bus_test.py` & `resotocore-3.6.1/tests/resotocore/message_bus_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/model/__init__.py` & `resotocore-3.6.1/tests/resotocore/model/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/model/adjust_node_test.py` & `resotocore-3.6.1/tests/resotocore/model/adjust_node_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/model/db_updater_test.py` & `resotocore-3.6.1/tests/resotocore/model/db_updater_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,82 @@
+import asyncio
 import json
 from datetime import timedelta
 from multiprocessing import set_start_method
-from typing import List, AsyncGenerator
+from typing import List, AsyncGenerator, Any
 
 import pytest
 
 from resotocore.analytics import AnalyticsEventSender
 from resotocore.db.deferred_edge_db import pending_deferred_edge_db
 from resotocore.db.graphdb import ArangoGraphDB
 from resotocore.db.model import GraphUpdate
-from resotocore.dependencies import empty_config
+from resotocore.system_start import empty_config
 from resotocore.ids import TaskId
-from resotocore.model.db_updater import merge_graph_process
+from resotocore.message_bus import MessageBus
+from resotocore.model.db_updater import GraphMerger
 from resotocore.model.model import Kind, Model
 from resotocore.model.typed_model import to_js
 from resotocore.types import Json
 from tests.resotocore.db.graphdb_test import create_graph
 from tests.resotocore.model import ModelHandlerStatic
 
 
 @pytest.mark.asyncio
 async def test_merge_process(
-    event_sender: AnalyticsEventSender, graph_db: ArangoGraphDB, foo_kinds: List[Kind]
+    event_sender: AnalyticsEventSender, graph_db: ArangoGraphDB, foo_kinds: List[Kind], message_bus: MessageBus
 ) -> None:
     # set explicitly (is done in main explicitly as well)
     set_start_method("spawn")
 
     # wipe any existing data
     await graph_db.wipe()
     # store the model in db, so it can be loaded by the sub process
-    graph_db.db.collection("model").insert_many([to_js(a) for a in foo_kinds])
+    graph_db.db.collection(f"{graph_db.name}_model").insert_many([to_js(a) for a in foo_kinds])
     # define args to parse for the sub process
     config = empty_config(["--graphdb-username", "test", "--graphdb-password", "test", "--graphdb-database", "test"])
     # create sample graph data to insert
     graph = create_graph("test")
 
     await pending_deferred_edge_db(graph_db.db, "deferred_outer_edges").create_update_schema()
 
     async def iterator() -> AsyncGenerator[bytes, None]:
+        def to_b(a: Any) -> bytes:
+            return bytes(json.dumps(a) + "\n", "utf-8")
+
         for node in graph.nodes():
-            yield bytes(json.dumps(graph.nodes[node]), "utf-8")
+            yield to_b(graph.nodes[node])
         for from_node, to_node, data in graph.edges(data=True):
-            yield bytes(json.dumps({"from": from_node, "to": to_node, "edge_type": data["edge_type"]}), "utf-8")
-        yield bytes(
-            json.dumps(
-                {"from_selector": {"node_id": "id_123"}, "to_selector": {"node_id": "id_456"}, "edge_type": "delete"}
-            ),
-            "utf-8",
+            yield to_b({"from": from_node, "to": to_node, "edge_type": data["edge_type"]})
+        yield to_b(
+            {"from_selector": {"node_id": "id_123"}, "to_selector": {"node_id": "id_456"}, "edge_type": "delete"}
         )
 
     model_handler = ModelHandlerStatic(Model.from_kinds(foo_kinds))
-    result = await merge_graph_process(
-        graph_db, model_handler, event_sender, config, iterator(), timedelta(seconds=30), None, TaskId("test_task_123")
-    )
-    assert result == GraphUpdate(112, 1, 0, 212, 0, 0)
-    elem: Json = graph_db.db.collection("deferred_outer_edges").get("test_task_123")  # type: ignore
-    assert elem["_key"] == "test_task_123"
-    assert elem["task_id"] == "test_task_123"
-    assert elem["edges"][0] == {"from_node": {"value": "id_123"}, "to_node": {"value": "id_456"}, "edge_type": "delete"}
+    async with GraphMerger(model_handler, event_sender, config, message_bus) as merger:
+        result = await merger.merge_graph(
+            graph_db, iterator(), timedelta(seconds=30), None, TaskId("test_task_123"), wait_for_result=True
+        )
+        assert result == GraphUpdate(112, 1, 0, 212, 0, 0)
+        elem: Json = graph_db.db.collection("deferred_outer_edges").get("test_task_123")  # type: ignore
+        assert elem["_key"] == "test_task_123"
+        assert elem["task_id"] == "test_task_123"
+        assert elem["edges"][0] == {
+            "from_node": {"value": "id_123"},
+            "to_node": {"value": "id_456"},
+            "edge_type": "delete",
+        }
+
+        # make another update without wait
+        current_count = graph_db.db.collection("ns").count()
+        graph = create_graph("test2", width=1)
+        no_result = await merger.merge_graph(
+            graph_db, iterator(), timedelta(seconds=30), None, TaskId("test_task_124"), wait_for_result=False
+        )
+        assert no_result is None
+
+        async def wait_for_result() -> None:
+            while graph_db.db.collection("ns").count() == current_count:
+                await asyncio.sleep(0.01)
+
+        # make sure that the update is processed in the background
+        await asyncio.wait_for(wait_for_result(), timeout=5)
```

### Comparing `resotocore-3.6.0/tests/resotocore/model/graph_access_test.py` & `resotocore-3.6.1/tests/resotocore/model/graph_access_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pytest import fixture
 
 from resotocore.ids import NodeId
 from resotocore.model.graph_access import GraphAccess, GraphBuilder, EdgeTypes, EdgeKey
 from resotocore.model.model import Model, AnyKind, ComplexKind
 from resotocore.model.typed_model import to_json
 from resotocore.types import Json, EdgeType
-from resotocore.util import AccessJson, AccessNone
+from resotocore.util import AccessJson, AccessNone, uuid_str
 from tests.resotocore.db.graphdb_test import Foo
 
 FooTuple = collections.namedtuple(
     "FooTuple",
     ["a", "b", "c", "d", "e", "f", "g", "kind"],
     defaults=["", 0, [], "foo", {"a": 12, "b": 32}, date.fromisoformat("2021-03-29"), 1.234567, "foo"],
 )
@@ -133,15 +133,15 @@
         return res
     else:
         raise AttributeError(f"Expected {node_id} to be defined!")
 
 
 def test_builder(person_model: Model) -> None:
     max_m = {"id": "max", "kind": "Person", "name": "Max"}
-    builder = GraphBuilder(person_model)
+    builder = GraphBuilder(person_model, uuid_str())
     builder.add_from_json({"id": "root", "reported": max_m})
     builder.add_from_json({"from": "root", "to": "2"})
     with pytest.raises(AssertionError) as no_node:
         builder.check_complete()
     assert str(no_node.value) == "2 was used in an edge definition but not provided as vertex!"
     builder.add_from_json({"id": "2", "reported": max_m})
     builder.add_from_json({"id": "3", "reported": max_m})
@@ -150,28 +150,28 @@
     assert str(no_node.value) == "Given subgraph has more than one root: ['root', '3']"
     builder.add_from_json({"from": "root", "to": "3"})
     builder.check_complete()
 
 
 def test_reassign_root(person_model: Model) -> None:
     max_m = {"id": "max", "kind": "Person", "name": "Max"}
-    builder = GraphBuilder(person_model)
+    builder = GraphBuilder(person_model, uuid_str())
     builder.add_from_json({"id": "should_be_root", "reported": {"kind": "graph_root"}})
     builder.add_from_json({"id": "2", "reported": max_m})
     builder.add_from_json({"id": "3", "reported": max_m})
     builder.add_from_json({"from": "should_be_root", "to": "2"})
     builder.add_from_json({"from": "should_be_root", "to": "3"})
     builder.check_complete()
     access = GraphAccess(builder.graph)
     assert access.root() == "root"
     assert set(access.successors(NodeId("root"), EdgeTypes.default)) == {"2", "3"}
 
 
 def test_replace_nodes(person_model: Model) -> None:
-    builder = GraphBuilder(person_model)
+    builder = GraphBuilder(person_model, uuid_str())
     meta = {"metadata": {"replace": True}}
     builder.add_from_json({"id": "root", "reported": {"kind": "graph_root"}})
     builder.add_from_json({"id": "cloud", "reported": {"id": "cloud", "kind": "cloud"}, **meta})
     # also mark account and region as replace node -> the flags should be ignored!
     builder.add_from_json({"id": "account", "reported": {"id": "account", "kind": "account"}, **meta})
     builder.add_from_json({"id": "region", "reported": {"id": "region", "kind": "region"}, **meta})
     builder.add_from_json({"from": "root", "to": "cloud"})
@@ -357,15 +357,15 @@
     assert r2.metadata.descendant_count == 60
     r3 = AccessJson(graph.node("cloud_gcp"))  # type: ignore
     assert r3.metadata.descendant_summary == {"child": 162, "region": 18, "account": 3}
     assert r3.metadata.descendant_count == 183
 
 
 def test_model_size(person_model: Model) -> None:
-    builder = GraphBuilder(person_model)
+    builder = GraphBuilder(person_model, uuid_str())
     tags1 = {"foo": "bar", "bla": "blub" * 22}
     a1 = {"kind": "Address", "id": "a1", "zip": "s1", "city": "c1", "list": ["ccc"]}
     a2 = {"kind": "Address", "id": "aa2", "zip": "s2", "city": "gotham", "tags": tags1}
     p1 = dict(kind="Person", id="pp1", name="pp1", address=a1, list=["a", "bb"], tags=tags1)
     p2 = dict(kind="Person", id="p2", name="ppp2", addresses=[a1, a2], other_addresses=dict(home=a1, work=a2))
     builder.add_node(NodeId("p1"), p1)
     builder.add_node(NodeId("p2"), p2)
```

### Comparing `resotocore-3.6.0/tests/resotocore/model/json_schema_test.py` & `resotocore-3.6.1/tests/resotocore/model/json_schema_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/model/model_handler_test.py` & `resotocore-3.6.1/tests/resotocore/model/model_handler_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/model/model_test.py` & `resotocore-3.6.1/tests/resotocore/model/model_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/model/typed_model_test.py` & `resotocore-3.6.1/tests/resotocore/model/typed_model_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/query/__init__.py` & `resotocore-3.6.1/tests/resotocore/query/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     just,
     integers,
     booleans,
     tuples,
 )
 
 from resotocore.model.graph_access import EdgeTypes, Direction
-from tests.resotocore.hypothesis_extension import Drawer, optional, UD, any_string
+from tests.resotocore.hypothesis_extension import Drawer, optional, UD, any_string, any_datetime
 from resotocore.query.model import (
     IsTerm,
     Predicate,
     Term,
     Part,
     Query,
     CombinedTerm,
@@ -29,14 +29,15 @@
     AllTerm,
     Aggregate,
     AggregateVariableName,
     AggregateVariableCombined,
     AggregateVariable,
     AggregateFunction,
     Limit,
+    WithUsage,
 )
 
 
 query_property = sampled_from(["reported.name", "reported.cpu_count"])
 kind = sampled_from(["bucket", "volume", "certificate", "cloud", "database", "endpoint"])
 query_operations = sampled_from(["==", ">=", "<=", ">", "<"])
 query_values = sampled_from(["test", 23, True, False, None])
@@ -88,25 +89,37 @@
     num = d.draw(integers(min_value=0))
     nav = d.draw(navigation())
     trm = d.optional(term)
     wc = d.optional(with_clause())
     return WithClause(WithClauseFilter(op, num), nav, trm, wc)
 
 
+@composite
+def with_usage(ud: UD) -> WithUsage:
+    d = Drawer(ud)
+    start = d.draw(any_datetime)
+    end = d.optional(any_datetime)
+    metrics = d.draw(lists(any_string, min_size=1, max_size=3))
+    return WithUsage(start, end, metrics)
+
+
 part = builds(
     Part,
     term | merge_term(),
     optional(any_string),
     with_clause(),
+    with_usage(),
     lists(sort, min_size=0, max_size=3),
     optional(limit_gen),
     navigation(),
 )
 
-only_filter_part = builds(Part, term, just(None), just(None), lists(sort, min_size=0, max_size=1), optional(limit_gen))
+only_filter_part = builds(
+    Part, term, just(None), just(None), just(None), lists(sort, min_size=0, max_size=1), optional(limit_gen)
+)
 
 
 @composite
 def merge_query_query(ud: UD) -> Query:
     d = Drawer(ud)
     nav = d.draw(navigation())
     trm = d.draw(term)
```

### Comparing `resotocore-3.6.0/tests/resotocore/query/model_test.py` & `resotocore-3.6.1/tests/resotocore/query/model_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,14 +151,28 @@
     assert str(with_section_r.relative_to_section("r")) == str(query)
     # a query on section root does not change the query
     assert str(with_section_r.on_section(PathRoot)) == on_section
     # a query relative to section root does not change the query
     assert str(with_section_r.relative_to_section(PathRoot)) == on_section
 
 
+def test_rewrite_usage() -> None:
+    def check(query_str: str, expect_before: str, expect_after: str) -> None:
+        before, after = parse_query(query_str).current_part.term.split_by_usage()
+        assert str(before) == expect_before
+        assert str(after) == expect_after
+
+    # filter on a,b,c before the usage is evaluated
+    check("usage.cpu.max>3 and ((a<1 and b>1) or c==3)", "((a < 1 and b > 1) or c == 3)", "usage.cpu.max > 3")
+    # same query, but different order
+    check("((a<1 and b>1) or c==3) and usage.cpu.max>3", "((a < 1 and b > 1) or c == 3)", "usage.cpu.max > 3")
+    # usage on top level in combination with or can not be optimized
+    check("usage.cpu.max>3 or ((a<1 and b>1) or c==3)", "all", "(usage.cpu.max > 3 or ((a < 1 and b > 1) or c == 3))")
+
+
 def test_rewrite_ancestors_descendants() -> None:
     # a query without ancestor/descendants is not changed
     assert str(parse_query("(a<1 and b>1) or c==3")) == "((a < 1 and b > 1) or c == 3)"
     # a query with resolved ancestor is not changed
     assert (
         str(parse_query('a<1 and ancestors.cloud.reported.name=="test"').on_section())
         == '(a < 1 and ancestors.cloud.reported.name == "test")'
```

### Comparing `resotocore-3.6.0/tests/resotocore/query/query_parser_test.py` & `resotocore-3.6.1/tests/resotocore/query/query_parser_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from datetime import datetime, timedelta
 from functools import partial
-from typing import Callable, Optional, Any
+from typing import Callable, Optional, Any, List
 
 import pytest
 from attrs import evolve
 from deepdiff import DeepDiff
 from hypothesis import given, settings, HealthCheck
 from parsy import Parser, ParseError
+from pytest import approx
 
 from resotocore import error
 from resotocore.model.graph_access import EdgeTypes, Direction
 from resotocore.query.model import (
     Navigation,
     Part,
     Query,
@@ -28,14 +30,15 @@
     MergeTerm,
     MergeQuery,
     FulltextTerm,
     CombinedTerm,
     Predicate,
     Limit,
     NotTerm,
+    WithUsage,
 )
 from resotocore.query.query_parser import (
     predicate_term,
     is_term,
     function_term,
     combined_term,
     navigation_parser,
@@ -50,15 +53,17 @@
     sort_parser,
     limit_parser,
     with_clause_parser,
     not_term,
     term_parser,
     parse_query,
     context_term,
+    with_usage_parser,
 )
+from resotocore.util import utc, parse_utc
 from tests.resotocore.query import query
 
 
 def test_parse_is_term() -> None:
     assert is_term.parse("is(test)") == IsTerm(["test"])
     assert is_term.parse("is(a, b, c)") == IsTerm(["a", "b", "c"])
     assert is_term.parse("is([a,b,c])") == IsTerm(["a", "b", "c"])
@@ -328,14 +333,33 @@
         parse_query("is(instance) and sort instance_cores")
 
     # parser read the reversed option as separate part, so following query became 3 parts
     q = parse_query("all sort kind desc limit 1 reversed -default-> all sort kind asc")
     assert len(q.parts) == 2
 
 
+def test_usage_parser() -> None:
+    def test_usage(s: str, start: datetime, end: Optional[datetime], metrics: List[str]) -> None:
+        usage: WithUsage = with_usage_parser.parse(s)
+        assert usage.start_from_now().timestamp() == approx(start.timestamp(), abs=1)
+        if end:
+            assert usage.end is not None
+            assert usage.end_from_now().timestamp() == approx(end.timestamp(), abs=1)
+        assert usage.metrics == metrics
+
+    oneweekago = utc() - timedelta(weeks=1)
+    twoweekago = utc() - timedelta(weeks=2)
+    at = parse_utc("2023-06-10T12:23:21Z")
+    test_usage("with_usage(1w, a,b,c)", oneweekago, None, ["a", "b", "c"])
+    test_usage("with_usage(2w::1w, a,b,c)", twoweekago, oneweekago, ["a", "b", "c"])
+    test_usage("with_usage(2w::1w, [a,b,c])", twoweekago, oneweekago, ["a", "b", "c"])
+    test_usage("with_usage(2023-06-10T12:23:21Z::1w, [a,b,c])", at, oneweekago, ["a", "b", "c"])
+    test_usage("with_usage(2023-06-10T12:23:21Z::2023-06-10T12:23:21Z, [a,b,c])", at, at, ["a", "b", "c"])
+
+
 @given(query)
 @settings(max_examples=200, suppress_health_check=list(HealthCheck))
 def test_generated_query(q: Query) -> None:
     assert str(q) == str(parse_query(str(q)))
 
 
 def assert_round_trip(parser: Parser, obj: object, after_parsed: Optional[Callable[[Any], Any]] = None) -> None:
```

### Comparing `resotocore-3.6.0/tests/resotocore/query/template_expander_test.py` & `resotocore-3.6.1/tests/resotocore/query/template_expander_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -150,7 +150,26 @@
     res = render_template(template, attrs2)
     assert res == 'query foo="123"'
 
 
 def test_custom_tags() -> None:
     res = render_template("@test@ and @rest@", dict(test="work", rest="play"), tags=("@", "@"))
     assert res == "work and play"
+
+
+@pytest.mark.asyncio
+async def test_abbreviation(expander: TemplateExpander) -> None:
+    async def with_section(section: Optional[str]) -> None:
+        # name form
+        assert str(await expander.parse_query("cloud=a", section)) == 'ancestors.cloud.reported.name == "a"'
+        assert str(await expander.parse_query("account=a", section)) == 'ancestors.account.reported.name == "a"'
+        assert str(await expander.parse_query("region=a", section)) == 'ancestors.region.reported.name == "a"'
+        assert str(await expander.parse_query("zone=a", section)) == 'ancestors.zone.reported.name == "a"'
+        # short form
+        assert str(await expander.parse_query("cloud.name=a", section)) == 'ancestors.cloud.reported.name == "a"'
+        assert str(await expander.parse_query("account.name=a", section)) == 'ancestors.account.reported.name == "a"'
+        assert str(await expander.parse_query("region.name=a", section)) == 'ancestors.region.reported.name == "a"'
+        assert str(await expander.parse_query("zone.name=a", section)) == 'ancestors.zone.reported.name == "a"'
+        assert str(await expander.parse_query("usage.cpu.max > 3", section)) == "usage.cpu.max > 3"
+
+    for s in Section.content_ordered + [None]:
+        await with_section(s)
```

### Comparing `resotocore-3.6.0/tests/resotocore/report/benchnmark_renderer_test.py` & `resotocore-3.6.1/tests/resotocore/report/benchnmark_renderer_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/report/inspector_service_test.py` & `resotocore-3.6.1/tests/resotocore/report/inspector_service_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/task/job_handler_test.py` & `resotocore-3.6.1/tests/resotocore/task/job_handler_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/task/start_workflow_on_first_subscriber_test.py` & `resotocore-3.6.1/tests/resotocore/task/start_workflow_on_first_subscriber_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/task/subscribers_test.py` & `resotocore-3.6.1/tests/resotocore/task/subscribers_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/task/task_description_test.py` & `resotocore-3.6.1/tests/resotocore/task/task_description_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from datetime import timedelta
 from typing import Any, List, Dict, Tuple, Callable
 
+from attr import evolve
 from deepdiff import DeepDiff
 from frozendict import frozendict
 
 from resotocore.ids import SubscriberId, TaskDescriptorId
 from resotocore.message_bus import Action, ActionDone, ActionError, Event, ActionProgress, ActionInfo
 from resotocore.model.typed_model import from_js, to_js
+from resotocore.task.task_dependencies import TaskDependencies
 from resotocore.task.model import Subscriber, Subscription
 from resotocore.task.task_description import (
     Workflow,
     Step,
     RunningTask,
     StepErrorBehaviour,
     PerformAction,
@@ -94,19 +96,22 @@
     events = wi.handle_error(ActionError("collect_done", wi.id, "done", s2.id, "boom"))
     assert wi.is_active is False
     assert wi.is_error is True
     assert len(events) == 0
 
 
 def test_complete_workflow(
-    workflow_instance: Tuple[RunningTask, Subscriber, Subscriber, Dict[str, List[Subscriber]]]
+    workflow_instance: Tuple[RunningTask, Subscriber, Subscriber, Dict[str, List[Subscriber]]],
+    task_dependencies: TaskDependencies,
 ) -> None:
     init, s1, s2, subscriptions = workflow_instance
     # start new workflow instance
-    wi, events = RunningTask.empty(init.descriptor, lambda: subscriptions)
+    wi, events = RunningTask.empty(
+        init.descriptor, evolve(task_dependencies, subscribers_by_event=lambda: subscriptions)
+    )
     assert wi.current_step.name == "start"
     assert len(events) == 2
     assert wi.progress.percentage == 0
     events = wi.handle_done(ActionDone("start", wi.id, "start", s1.id))
     assert wi.current_step.name == "wait"
     assert len(events) == 0
     assert wi.progress.percentage == 33
@@ -180,19 +185,19 @@
 
 def roundtrip(obj: Any) -> None:
     js = to_js(obj)
     again = from_js(js, type(obj))
     assert DeepDiff(obj, again) == {}, f"Json: {js} serialized as {again}"
 
 
-def test_task_progress() -> None:
+def test_task_progress(task_dependencies: TaskDependencies) -> None:
     actions = ["collect", "encode"]
     wf = Workflow(TaskDescriptorId("test_workflow"), "name", [Step(a, PerformAction(a)) for a in actions], [])
     sb = Subscriber(SubscriberId("test"), {s: Subscription(s) for s in actions})
-    rt, _ = RunningTask.empty(wf, lambda: {s: [sb] for s in actions})
+    rt, _ = RunningTask.empty(wf, evolve(task_dependencies, subscribers_by_event=lambda: {s: [sb] for s in actions}))
 
     def progress(step: str, fn: Callable[[int], ProgressDone]) -> None:
         # use revers order to test that the correct order is used
         for idx in range(3):
             rt.handle_progress(ActionProgress(step, rt.id, step, sb.id, fn(idx), utc()))
 
     # report progress start on the collect step
```

### Comparing `resotocore-3.6.0/tests/resotocore/task/task_handler_test.py` & `resotocore-3.6.1/tests/resotocore/task/task_handler_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,29 +4,31 @@
 from typing import List
 
 import pytest
 from pytest import LogCaptureFixture
 
 from resotocore.analytics import AnalyticsEventSender, InMemoryEventSender
 from resotocore.cli.cli import CLIService
+from tests.resotocore.conftest import eventually
 from resotocore.db.jobdb import JobDb
 from resotocore.db.runningtaskdb import RunningTaskDb
-from resotocore.dependencies import empty_config
+from resotocore.system_start import empty_config
 from resotocore.ids import SubscriberId, TaskDescriptorId
-from resotocore.message_bus import MessageBus, Event, Message, ActionDone, Action, ActionInfo, ActionError
-from resotocore.task import RunningTaskInfo
+from resotocore.message_bus import MessageBus, Event, Message, ActionDone, Action, ActionInfo, ActionError, CoreMessage
+from resotocore.model.db_updater import GraphMerger
 from resotocore.task.scheduler import Scheduler
 from resotocore.task.subscribers import SubscriptionHandler
 from resotocore.task.task_description import (
     Workflow,
     EventTrigger,
     TimeTrigger,
     Job,
     TaskSurpassBehaviour,
     ExecuteCommand,
+    RunningTask,
 )
 from resotocore.task.task_handler import TaskHandlerService
 from tests.resotocore.message_bus_test import wait_for_message
 
 
 @pytest.mark.asyncio
 async def test_run_job(task_handler: TaskHandlerService, all_events: List[Message]) -> None:
@@ -39,25 +41,27 @@
 @pytest.mark.asyncio
 async def test_recover_workflow(
     running_task_db: RunningTaskDb,
     job_db: JobDb,
     message_bus: MessageBus,
     event_sender: AnalyticsEventSender,
     subscription_handler: SubscriptionHandler,
+    graph_merger: GraphMerger,
     all_events: List[Message],
     cli: CLIService,
     test_workflow: Workflow,
 ) -> None:
     def handler() -> TaskHandlerService:
         th = TaskHandlerService(
             running_task_db,
             job_db,
             message_bus,
             event_sender,
             subscription_handler,
+            graph_merger,
             Scheduler(),
             cli,
             empty_config(),
         )
         th.task_descriptions = [test_workflow]
         return th
 
@@ -199,7 +203,41 @@
         await task_handler.delete_job("foo:bar")
 
     # delete a job with a valid name: should succeed if the validation disabled
     await task_handler.delete_job("foobar", force=True)
 
     # force delete a job should not throw an exception
     await task_handler.delete_job("foo:bar", force=True)
+
+
+@pytest.mark.asyncio
+async def test_wait_for_collect_done(
+    task_handler: TaskHandlerService, message_bus: MessageBus, graph_merger: GraphMerger
+) -> None:
+    async with task_handler:
+        # Test 1: start a task without any ongoing graph merges
+        # start task
+        task = await task_handler.start_task_by_descriptor_id(TaskDescriptorId("wait_for_collect_done"))
+        assert task is not None
+        rt: RunningTask = task.running_task
+        assert rt in await task_handler.running_tasks()
+        # no collect is in progress. The task should be finished immediately.
+        await message_bus.emit_event("collected", {})
+        await eventually(lambda: rt.current_step.name == "task_end")
+
+        # Test 2: start a task with an ongoing graph merge operations. The task should wait for the merge to finish.
+        # start task
+        task = await task_handler.start_task_by_descriptor_id(TaskDescriptorId("wait_for_collect_done"))
+        assert task is not None
+        rt = task.running_task
+        assert rt in await task_handler.running_tasks()
+        # fake some ongoing imports in graph merger
+        graph_merger.running_imports[rt.id] = 42
+        # send event to finish task
+        await message_bus.emit_event("collected", {})
+        # sleep a little bit to make sure the task is not finished
+        await asyncio.sleep(0.1)
+        await eventually(lambda: rt.current_step.name == "wait_for_collect_done")
+        # signal, that the import is finished
+        await message_bus.emit_event(CoreMessage.GraphMergeCompleted, dict(task_id=rt.id))
+        # make sure the task finishes
+        await eventually(lambda: rt.current_step.name == "task_end")
```

### Comparing `resotocore-3.6.0/tests/resotocore/user/user_management_service_test.py` & `resotocore-3.6.1/tests/resotocore/user/user_management_service_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/validator_test.py` & `resotocore-3.6.1/tests/resotocore/validator_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/web/api_client.py` & `resotocore-3.6.1/tests/resotocore/web/api_client.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/web/api_test.py` & `resotocore-3.6.1/tests/resotocore/web/api_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,19 +62,15 @@
           The fixture ensures that the underlying process has entered the ready state.
           It also ensures to clean up the process, when the test is done.
     """
     http_port = get_free_port()  # use a different port than the default one
     additional_args = ["--psk", psk] if psk else []
 
     # wipe and cleanly import the test model
-    await db_access.model_db.create_update_schema()
-    await db_access.model_db.wipe()
-    await db_access.model_db.update_many(foo_kinds)
-
-    for graph_name in [g, "test", "hello", "bonjour", "foo"]:
+    for graph_name in [g, "test", "hello", "bonjour", "foo", "resoto"]:
         db = await db_access.get_graph_model_db(GraphName(graph_name))
         await db.create_update_schema()
         await db.wipe()
         await db.update_many(foo_kinds)
 
     config_dir = tempfile.TemporaryDirectory()
     # todo: do not restart after the config override was loaded for the very first time and uncomment this part
```

### Comparing `resotocore-3.6.0/tests/resotocore/web/certificate_handler_test.py` & `resotocore-3.6.1/tests/resotocore/web/certificate_handler_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from tempfile import TemporaryDirectory
 from typing import Optional, cast
 
 from arango.database import StandardDatabase
 from attr import evolve
 
 from resotocore.core_config import CoreConfig
-from resotocore.dependencies import empty_config, parse_args
+from resotocore.system_start import empty_config, parse_args
 from resotocore.types import Json
 from resotocore.web.certificate_handler import CertificateHandler
 from resotolib.x509 import (
     load_cert_from_bytes,
     cert_fingerprint,
     csr_to_bytes,
     gen_csr,
```

### Comparing `resotocore-3.6.0/tests/resotocore/web/content_renderer_test.py` & `resotocore-3.6.1/tests/resotocore/web/content_renderer_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.6.0/tests/resotocore/worker_task_queue_test.py` & `resotocore-3.6.1/tests/resotocore/worker_task_queue_test.py`

 * *Files identical despite different names*

