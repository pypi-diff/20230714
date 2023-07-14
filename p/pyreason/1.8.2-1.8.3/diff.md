# Comparing `tmp/pyreason-1.8.2.tar.gz` & `tmp/pyreason-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreason-1.8.2.tar", last modified: Wed Jun 21 14:05:50 2023, max compression
+gzip compressed data, was "pyreason-1.8.3.tar", last modified: Fri Jul 14 17:05:45 2023, max compression
```

## Comparing `pyreason-1.8.2.tar` & `pyreason-1.8.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.326357 pyreason-1.8.2/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-06-21 14:05:37.000000 pyreason-1.8.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-21 14:05:37.000000 pyreason-1.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-21 14:05:50.326357 pyreason-1.8.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-06-21 14:05:37.000000 pyreason-1.8.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.318357 pyreason-1.8.2/pyreason/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/.cache_status.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1001 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.318357 pyreason-1.8.2/pyreason/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.318357 pyreason-1.8.2/pyreason/examples/hello-world/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/examples/hello-world/facts.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/examples/hello-world/friends.graphml
--rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/examples/hello-world/ipl.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/examples/hello-world/labels.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/examples/hello-world/rules.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    28008 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/pyreason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.322357 pyreason-1.8.2/pyreason/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.322357 pyreason-1.8.2/pyreason/scripts/annotation_functions/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/annotation_functions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/annotation_functions/annotation_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.322357 pyreason-1.8.2/pyreason/scripts/components/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/components/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/components/label.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/components/world.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/diffuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.322357 pyreason-1.8.2/pyreason/scripts/facts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/facts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/facts/fact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/facts/fact_edge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/facts/fact_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.322357 pyreason-1.8.2/pyreason/scripts/interpretation/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/interpretation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    75254 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/interpretation/interpretation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.322357 pyreason-1.8.2/pyreason/scripts/interval/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/interval/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/interval/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.322357 pyreason-1.8.2/pyreason/scripts/numba_wrapper/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/numba_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.322357 pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6015 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/label_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10472 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/world_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.322357 pyreason-1.8.2/pyreason/scripts/program/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/program/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2028 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/program/program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.322357 pyreason-1.8.2/pyreason/scripts/rules/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1199 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.326357 pyreason-1.8.2/pyreason/scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/utils/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4587 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/utils/graphml_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/utils/output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/utils/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/utils/rule_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/utils/visuals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8756 2023-06-21 14:05:37.000000 pyreason-1.8.2/pyreason/scripts/utils/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.318357 pyreason-1.8.2/pyreason.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-21 14:05:50.000000 pyreason-1.8.2/pyreason.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-21 14:05:50.000000 pyreason-1.8.2/pyreason.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:05:50.000000 pyreason-1.8.2/pyreason.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 14:05:50.000000 pyreason-1.8.2/pyreason.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 14:05:50.000000 pyreason-1.8.2/pyreason.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 14:05:50.326357 pyreason-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-21 14:05:37.000000 pyreason-1.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:05:50.326357 pyreason-1.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-21 14:05:37.000000 pyreason-1.8.2/tests/test_hello_world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.992014 pyreason-1.8.3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-07-14 17:05:29.000000 pyreason-1.8.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-14 17:05:29.000000 pyreason-1.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-14 17:05:45.992014 pyreason-1.8.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-07-14 17:05:29.000000 pyreason-1.8.3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.976014 pyreason-1.8.3/pyreason/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/.cache_status.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.980014 pyreason-1.8.3/pyreason/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.980014 pyreason-1.8.3/pyreason/examples/hello-world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/examples/hello-world/facts.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/examples/hello-world/friends.graphml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/examples/hello-world/ipl.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/examples/hello-world/labels.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/examples/hello-world/rules.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30332 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/pyreason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.980014 pyreason-1.8.3/pyreason/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.984014 pyreason-1.8.3/pyreason/scripts/annotation_functions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/annotation_functions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/annotation_functions/annotation_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.984014 pyreason-1.8.3/pyreason/scripts/components/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/components/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/components/label.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/components/world.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/diffuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.984014 pyreason-1.8.3/pyreason/scripts/facts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/facts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/facts/fact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/facts/fact_edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/facts/fact_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.984014 pyreason-1.8.3/pyreason/scripts/interpretation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/interpretation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    76573 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/interpretation/interpretation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.984014 pyreason-1.8.3/pyreason/scripts/interval/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/interval/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/interval/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.984014 pyreason-1.8.3/pyreason/scripts/numba_wrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/numba_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.988014 pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6015 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/label_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10414 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/world_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.988014 pyreason-1.8.3/pyreason/scripts/program/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/program/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2130 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/program/program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.988014 pyreason-1.8.3/pyreason/scripts/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1188 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.992014 pyreason-1.8.3/pyreason/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/utils/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4551 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/utils/graphml_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/utils/output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/utils/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/utils/rule_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/utils/visuals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8756 2023-07-14 17:05:29.000000 pyreason-1.8.3/pyreason/scripts/utils/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.980014 pyreason-1.8.3/pyreason.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-14 17:05:45.000000 pyreason-1.8.3/pyreason.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-14 17:05:45.000000 pyreason-1.8.3/pyreason.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:05:45.000000 pyreason-1.8.3/pyreason.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 17:05:45.000000 pyreason-1.8.3/pyreason.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 17:05:45.000000 pyreason-1.8.3/pyreason.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:05:45.992014 pyreason-1.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-14 17:05:29.000000 pyreason-1.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:05:45.992014 pyreason-1.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-14 17:05:29.000000 pyreason-1.8.3/tests/test_hello_world.py
```

### Comparing `pyreason-1.8.2/LICENSE.md` & `pyreason-1.8.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/PKG-INFO` & `pyreason-1.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.8.2
+Version: 1.8.3
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.8.2/README.md` & `pyreason-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/__init__.py` & `pyreason-1.8.3/pyreason/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     cache_status = yaml.safe_load(file)
 
 if not cache_status['initialized']:
     print('Imported PyReason for the first time. Initializing ... this will take a minute')
     graph_path = os.path.join(package_path, 'examples', 'hello-world', 'friends.graphml')
 
     settings.verbose = False
-    load_graph(graph_path)
+    load_graphml(graph_path)
     add_rule('popular(x) <-1 popular(y), Friends(x,y), owns(y,z), owns(x,z)', 'popular_rule')
     add_fact(Fact('popular-fact', 'Mary', 'popular', [1, 1], 0, 2))
     reason(timesteps=2)
 
     # Update cache status
     cache_status['initialized'] = True
     with open(cache_status_path, 'w') as file:
```

### Comparing `pyreason-1.8.2/pyreason/examples/hello-world/facts.yaml` & `pyreason-1.8.3/pyreason/examples/hello-world/facts.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/examples/hello-world/friends.graphml` & `pyreason-1.8.3/pyreason/examples/hello-world/friends.graphml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/examples/hello-world/rules.yaml` & `pyreason-1.8.3/pyreason/examples/hello-world/rules.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/pyreason.py` & `pyreason-1.8.3/pyreason/pyreason.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This is the file that will be imported when "import pyreason" is called. All content will be run automatically
+import networkx as nx
 import numba
 import time
 import sys
 import warnings
 import memory_profiler as mp
-from typing import List, Type
+from typing import List, Type, Callable
 
 from pyreason.scripts.utils.output import Output
 from pyreason.scripts.utils.filter import Filter
 from pyreason.scripts.program.program import Program
 from pyreason.scripts.utils.graphml_parser import GraphmlParser
 import pyreason.scripts.utils.yaml_parser as yaml_parser
 import pyreason.scripts.utils.rule_parser as rule_parser
@@ -319,14 +320,16 @@
 __specific_edge_labels = None
 
 __non_fluent_graph_facts_node = None
 __non_fluent_graph_facts_edge = None
 __specific_graph_node_labels = None
 __specific_graph_edge_labels = None
 
+__annotation_functions = []
+
 __timestamp = ''
 __program = None
 
 __graphml_parser = GraphmlParser()
 settings = _Settings()
 
 
@@ -346,15 +349,15 @@
     Resets rules to none
     """
     global __rules
     __rules = None
 
 
 # FUNCTIONS
-def load_graph(path: str) -> None:
+def load_graphml(path: str) -> None:
     """Loads graph from GraphMl file path into program
 
     :param path: Path for the GraphMl file
     """
     global __graph, __graphml_parser, __non_fluent_graph_facts_node, __non_fluent_graph_facts_edge, __specific_graph_node_labels, __specific_graph_edge_labels, settings
     
     # Parse graph
@@ -364,15 +367,37 @@
     if settings.graph_attribute_parsing:
         __non_fluent_graph_facts_node, __non_fluent_graph_facts_edge, __specific_graph_node_labels, __specific_graph_edge_labels = __graphml_parser.parse_graph_attributes(settings.static_graph_facts)
     else:
         __non_fluent_graph_facts_node = numba.typed.List.empty_list(fact_node.fact_type)
         __non_fluent_graph_facts_edge = numba.typed.List.empty_list(fact_edge.fact_type)
         __specific_graph_node_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(numba.types.string))
         __specific_graph_edge_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(numba.types.Tuple((numba.types.string, numba.types.string))))
+
+
+def load_graph(graph: nx.DiGraph) -> None:
+    """Load a networkx DiGraph into pyreason
+
+    :param graph: Networkx DiGraph object to load into pyreason
+    :type graph: nx.DiGraph
+    :return: None
+    """
+    global __graph, __graphml_parser, __non_fluent_graph_facts_node, __non_fluent_graph_facts_edge, __specific_graph_node_labels, __specific_graph_edge_labels, settings
     
+    # Load graph
+    __graph = __graphml_parser.load_graph(graph)
+
+    # Graph attribute parsing
+    if settings.graph_attribute_parsing:
+        __non_fluent_graph_facts_node, __non_fluent_graph_facts_edge, __specific_graph_node_labels, __specific_graph_edge_labels = __graphml_parser.parse_graph_attributes(settings.static_graph_facts)
+    else:
+        __non_fluent_graph_facts_node = numba.typed.List.empty_list(fact_node.fact_type)
+        __non_fluent_graph_facts_edge = numba.typed.List.empty_list(fact_edge.fact_type)
+        __specific_graph_node_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(numba.types.string))
+        __specific_graph_edge_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(numba.types.Tuple((numba.types.string, numba.types.string))))
+
 
 def load_labels(path: str) -> None:
     """Load labels from YAML file path into program
 
     :param path: Path for the YAML labels file
     """
     global __node_labels, __edge_labels, __specific_node_labels, __specific_edge_labels
@@ -406,34 +431,35 @@
 
     :param path: Path for the YAML IPL file
     """
     global __ipl
     __ipl = yaml_parser.parse_ipl(path)
 
 
-def add_rule(rule_text: str, name: str, infer_edges: bool = False, immediate_rule: bool = False) -> None:
+def add_rule(rule_text: str, name: str, infer_edges: bool = False, set_static: bool = False, immediate_rule: bool = False) -> None:
     """Add a rule to pyreason from text format. This format is not as modular as the YAML format.
     1. It is not possible to specify thresholds. Threshold is greater than or equal to 1 by default
     2. It is not possible to have an annotation function.
     3. It is not possible to have weights for different clauses. Weights are 1 by default with bias 0
     TODO: Add threshold class where we can pass this as a parameter
     TODO: Add weights as a parameter
     TODO: Add annotation function and bounds as a parameter
 
     Example:
     `'pred1(x,y) : [0.2, 1] <- pred2(a, b) : [1,1], pred3(b, c)'`
 
     :param rule_text: The rule in text format
     :param name: The name of the rule. This will appear in the rule trace
     :param infer_edges: Whether to infer new edges after edge rule fires
+    :param set_static: Whether to set the atom in the head as static if the rule fires. The bounds will no longer change
     :param immediate_rule: Whether the rule is immediate. Immediate rules check for more applicable rules immediately after being applied
     """
     global __rules
 
-    r = rule_parser.parse_rule(rule_text, name, infer_edges, immediate_rule)
+    r = rule_parser.parse_rule(rule_text, name, infer_edges, set_static, immediate_rule)
     # Add to collection of rules
     if __rules is None:
         __rules = numba.typed.List.empty_list(rule.rule_type)
     __rules.append(r)
 
 
 def add_rules_from_file(file_path: str, infer_edges: bool = False) -> None:
@@ -470,14 +496,29 @@
     else:
         f = fact_edge.Fact(pyreason_fact.name, pyreason_fact.component, pyreason_fact.label, pyreason_fact.interval, pyreason_fact.t_lower, pyreason_fact.t_upper, pyreason_fact.static)
         if __edge_facts is None:
             __edge_facts = numba.typed.List.empty_list(fact_edge.fact_type)
         __edge_facts.append(f)
 
 
+def add_annotation_function(function: Callable) -> None:
+    """Function to add annotation functions to PyReason. The added functions can be used in rules
+
+    :param function: Function to be added. This has to be under a numba `njit` decorator. function has signature: two parameters as input -- annotations, weights
+    :type function: Callable
+    :return: None
+    """
+    global __annotation_functions
+    # Make sure that the functions are jitted so that they can be passed around in other jitted functions
+    # TODO: Remove if necessary
+    # assert hasattr(function, 'nopython_signatures'), 'The function to be added has to be under a `numba.njit` decorator'
+
+    __annotation_functions.append(function)
+
+
 def reason(timesteps: int=-1, convergence_threshold: int=-1, convergence_bound_threshold: float=-1, again: bool=False, node_facts: List[Type[fact_node.Fact]]=None, edge_facts: List[Type[fact_edge.Fact]]=None):
     """Function to start the main reasoning process. Graph and rules must already be loaded.
 
     :param timesteps: Max number of timesteps to run. -1 specifies run till convergence. If reasoning again, this is the number of timesteps to reason for extra (no zero timestep), defaults to -1
     :param convergence_threshold: Maximim number of interpretations that have changed between timesteps or fixed point operations until considered convergent. Program will end at convergence. -1 => no changes, perfect convergence, defaults to -1
     :param convergence_bound_threshold: Maximum change in any interpretation (bounds) between timesteps or fixed point operations until considered convergent, defaults to -1
     :param again: Whether to reason again on an existing interpretation, defaults to False
@@ -569,16 +610,19 @@
     all_node_facts.extend(__non_fluent_graph_facts_node)
     all_edge_facts.extend(__non_fluent_graph_facts_edge)
 
     # Atom trace cannot be true when store interpretations is false
     if not settings.store_interpretation_changes:
         settings.atom_trace = False
 
+    # Convert list of annotation functions into tuple to be numba compatible
+    annotation_functions = tuple(__annotation_functions)
+
     # Setup logical program
-    __program = Program(__graph, all_node_facts, all_edge_facts, __rules, __ipl, settings.reverse_digraph, settings.atom_trace, settings.save_graph_attributes_to_trace, settings.canonical, settings.inconsistency_check, settings.store_interpretation_changes)
+    __program = Program(__graph, all_node_facts, all_edge_facts, __rules, __ipl, annotation_functions, settings.reverse_digraph, settings.atom_trace, settings.save_graph_attributes_to_trace, settings.canonical, settings.inconsistency_check, settings.store_interpretation_changes)
     __program.available_labels_node = __node_labels
     __program.available_labels_edge = __edge_labels
     __program.specific_node_labels = __specific_node_labels
     __program.specific_edge_labels = __specific_edge_labels
 
     # Run Program and get final interpretation
     interpretation = __program.reason(timesteps, convergence_threshold, convergence_bound_threshold, settings.verbose)
```

### Comparing `pyreason-1.8.2/pyreason/scripts/annotation_functions/annotation_functions.py` & `pyreason-1.8.3/pyreason/scripts/annotation_functions/annotation_functions.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/scripts/args.py` & `pyreason-1.8.3/pyreason/scripts/args.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/scripts/components/world.py` & `pyreason-1.8.3/pyreason/scripts/components/world.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/scripts/diffuse.py` & `pyreason-1.8.3/pyreason/scripts/diffuse.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/scripts/facts/fact.py` & `pyreason-1.8.3/pyreason/scripts/facts/fact.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/scripts/facts/fact_edge.py` & `pyreason-1.8.3/pyreason/scripts/facts/fact_edge.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/scripts/facts/fact_node.py` & `pyreason-1.8.3/pyreason/scripts/facts/fact_node.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/scripts/interpretation/interpretation.py` & `pyreason-1.8.3/pyreason/scripts/interpretation/interpretation.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 node_type = numba.types.string
 edge_type = numba.types.UniTuple(numba.types.string, 2)
 
 # Type for storing list of qualified nodes/edges
 list_of_nodes = numba.types.ListType(node_type)
 list_of_edges = numba.types.ListType(edge_type)
 
+# Type for facts to be applied
+facts_to_be_applied_node_type = numba.types.Tuple((numba.types.uint16, node_type, label.label_type, interval.interval_type, numba.types.boolean, numba.types.boolean))
+facts_to_be_applied_edge_type = numba.types.Tuple((numba.types.uint16, edge_type, label.label_type, interval.interval_type, numba.types.boolean, numba.types.boolean))
+
 # Type for returning list of applicable rules for a certain rule
 # node/edge, annotations, qualified nodes, qualified edges, edges to be added
 node_applicable_rule_type = numba.types.Tuple((
 	node_type,
 	numba.types.ListType(numba.types.ListType(interval.interval_type)),
 	numba.types.ListType(numba.types.ListType(node_type)),
 	numba.types.ListType(numba.types.ListType(edge_type)),
@@ -36,17 +40,18 @@
 
 class Interpretation:
 	available_labels_node = []
 	available_labels_edge = []
 	specific_node_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(node_type))
 	specific_edge_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(edge_type))
 
-	def __init__(self, graph, ipl, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, store_interpretation_changes):
+	def __init__(self, graph, ipl, annotation_functions, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, store_interpretation_changes):
 		self.graph = graph
 		self.ipl = ipl
+		self.annotation_functions = annotation_functions
 		self.reverse_graph = reverse_graph
 		self.atom_trace = atom_trace
 		self.save_graph_attributes_to_rule_trace = save_graph_attributes_to_rule_trace
 		self.canonical = canonical
 		self.inconsistency_check = inconsistency_check
 		self.store_interpretation_changes = store_interpretation_changes
 
@@ -55,18 +60,18 @@
 		self.prev_reasoning_data = numba.typed.List([0, 0])
 
 		# Initialize list of tuples for rules/facts to be applied, along with all the ground atoms that fired the rule. One to One correspondence between rules_to_be_applied_node and rules_to_be_applied_node_trace if atom_trace is true
 		self.rules_to_be_applied_node_trace = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), numba.types.string)))
 		self.rules_to_be_applied_edge_trace = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), numba.types.string)))
 		self.facts_to_be_applied_node_trace = numba.typed.List.empty_list(numba.types.string)
 		self.facts_to_be_applied_edge_trace = numba.typed.List.empty_list(numba.types.string)
-		self.rules_to_be_applied_node = numba.typed.List.empty_list(numba.types.Tuple((numba.types.uint16, node_type, label.label_type, interval.interval_type, numba.types.boolean)))
-		self.rules_to_be_applied_edge = numba.typed.List.empty_list(numba.types.Tuple((numba.types.uint16, edge_type, label.label_type, interval.interval_type, numba.types.boolean)))
-		self.facts_to_be_applied_node = numba.typed.List.empty_list(numba.types.Tuple((numba.types.uint16, node_type, label.label_type, interval.interval_type, numba.types.boolean, numba.types.boolean)))
-		self.facts_to_be_applied_edge = numba.typed.List.empty_list(numba.types.Tuple((numba.types.uint16, edge_type, label.label_type, interval.interval_type, numba.types.boolean, numba.types.boolean)))
+		self.rules_to_be_applied_node = numba.typed.List.empty_list(numba.types.Tuple((numba.types.uint16, node_type, label.label_type, interval.interval_type, numba.types.boolean, numba.types.boolean)))
+		self.rules_to_be_applied_edge = numba.typed.List.empty_list(numba.types.Tuple((numba.types.uint16, edge_type, label.label_type, interval.interval_type, numba.types.boolean, numba.types.boolean)))
+		self.facts_to_be_applied_node = numba.typed.List.empty_list(facts_to_be_applied_node_type)
+		self.facts_to_be_applied_edge = numba.typed.List.empty_list(facts_to_be_applied_edge_type)
 		self.edges_to_be_added_node_rule = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(node_type), numba.types.ListType(node_type), label.label_type)))
 		self.edges_to_be_added_edge_rule = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(node_type), numba.types.ListType(node_type), label.label_type)))
 
 		# Keep track of all the rules that have affected each node/edge at each timestep/fp operation, and all ground atoms that have affected the rules as well. Keep track of previous bounds and name of the rule/fact here
 		self.rule_trace_node_atoms = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), interval.interval_type, numba.types.string)))
 		self.rule_trace_edge_atoms = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), interval.interval_type, numba.types.string)))
 		self.rule_trace_node = numba.typed.List.empty_list(numba.types.Tuple((numba.types.uint16, numba.types.uint16, node_type, label.label_type, interval.interval_type)))
@@ -181,30 +186,31 @@
 				graph_attribute = True if name=='graph-attribute-fact' else False
 				facts_to_be_applied_edge.append((numba.types.uint16(t), fact.get_component(), fact.get_label(), fact.get_bound(), fact.static, graph_attribute))
 				if atom_trace:
 					facts_to_be_applied_edge_trace.append(fact.get_name())
 		return max_time
 
 	def _start_fp(self, rules, max_facts_time, verbose):
-		fp_cnt, t = self.reason(self.interpretations_node, self.interpretations_edge, self.tmax, self.prev_reasoning_data, rules, self.nodes, self.edges, self.neighbors, self.reverse_neighbors, self.rules_to_be_applied_node, self.rules_to_be_applied_edge, self.edges_to_be_added_node_rule, self.edges_to_be_added_edge_rule, self.rules_to_be_applied_node_trace, self.rules_to_be_applied_edge_trace, self.facts_to_be_applied_node, self.facts_to_be_applied_edge, self.facts_to_be_applied_node_trace, self.facts_to_be_applied_edge_trace, self.ipl, self.rule_trace_node, self.rule_trace_edge, self.rule_trace_node_atoms, self.rule_trace_edge_atoms, self.reverse_graph, self.atom_trace, self.save_graph_attributes_to_rule_trace, self.canonical, self.inconsistency_check, self.store_interpretation_changes, max_facts_time, self._convergence_mode, self._convergence_delta, verbose)
+		fp_cnt, t = self.reason(self.interpretations_node, self.interpretations_edge, self.tmax, self.prev_reasoning_data, rules, self.nodes, self.edges, self.neighbors, self.reverse_neighbors, self.rules_to_be_applied_node, self.rules_to_be_applied_edge, self.edges_to_be_added_node_rule, self.edges_to_be_added_edge_rule, self.rules_to_be_applied_node_trace, self.rules_to_be_applied_edge_trace, self.facts_to_be_applied_node, self.facts_to_be_applied_edge, self.facts_to_be_applied_node_trace, self.facts_to_be_applied_edge_trace, self.ipl, self.rule_trace_node, self.rule_trace_edge, self.rule_trace_node_atoms, self.rule_trace_edge_atoms, self.reverse_graph, self.atom_trace, self.save_graph_attributes_to_rule_trace, self.canonical, self.inconsistency_check, self.store_interpretation_changes, max_facts_time, self.annotation_functions, self._convergence_mode, self._convergence_delta, verbose)
 		self.time = t - 1
 		# If we need to reason again, store the next timestep to start from
 		self.prev_reasoning_data[0] = t
 		self.prev_reasoning_data[1] = fp_cnt
 		if verbose:
 			print('Fixed Point iterations:', fp_cnt)
 
 	@staticmethod
 	@numba.njit(cache=True)
-	def reason(interpretations_node, interpretations_edge, tmax, prev_reasoning_data, rules, nodes, edges, neighbors, reverse_neighbors, rules_to_be_applied_node, rules_to_be_applied_edge, edges_to_be_added_node_rule, edges_to_be_added_edge_rule, rules_to_be_applied_node_trace, rules_to_be_applied_edge_trace, facts_to_be_applied_node, facts_to_be_applied_edge, facts_to_be_applied_node_trace, facts_to_be_applied_edge_trace, ipl, rule_trace_node, rule_trace_edge, rule_trace_node_atoms, rule_trace_edge_atoms, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, store_interpretation_changes, max_facts_time, convergence_mode, convergence_delta, verbose):
+	def reason(interpretations_node, interpretations_edge, tmax, prev_reasoning_data, rules, nodes, edges, neighbors, reverse_neighbors, rules_to_be_applied_node, rules_to_be_applied_edge, edges_to_be_added_node_rule, edges_to_be_added_edge_rule, rules_to_be_applied_node_trace, rules_to_be_applied_edge_trace, facts_to_be_applied_node, facts_to_be_applied_edge, facts_to_be_applied_node_trace, facts_to_be_applied_edge_trace, ipl, rule_trace_node, rule_trace_edge, rule_trace_node_atoms, rule_trace_edge_atoms, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, store_interpretation_changes, max_facts_time, annotation_functions, convergence_mode, convergence_delta, verbose):
 		t = prev_reasoning_data[0]
 		fp_cnt = prev_reasoning_data[1]
 		max_rules_time = 0
 		timestep_loop = True
-		facts_to_remove_idx = numba.typed.List.empty_list(numba.types.int64)
+		facts_to_be_applied_node_new = numba.typed.List.empty_list(facts_to_be_applied_node_type)
+		facts_to_be_applied_edge_new = numba.typed.List.empty_list(facts_to_be_applied_edge_type)
 		rules_to_remove_idx = numba.typed.List.empty_list(numba.types.int64)
 		while timestep_loop:
 			if t==tmax:
 				timestep_loop = False
 			if verbose:
 				with objmode():
 					print('Timestep:', t, flush=True)
@@ -239,15 +245,15 @@
 			# Initialize the above
 			for i in range(len(rules)):
 				nodes_to_skip[i] = numba.typed.List.empty_list(node_type)
 				edges_to_skip[i] = numba.typed.List.empty_list(edge_type)
 
 			# Start by applying facts
 			# Nodes
-			facts_to_remove_idx.clear()
+			facts_to_be_applied_node_new.clear()
 			for i in range(len(facts_to_be_applied_node)):
 				if facts_to_be_applied_node[i][0]==t:
 					comp, l, bnd, static, graph_attribute = facts_to_be_applied_node[i][1], facts_to_be_applied_node[i][2], facts_to_be_applied_node[i][3], facts_to_be_applied_node[i][4], facts_to_be_applied_node[i][5]
 					# Check if bnd is static. Then no need to update, just add to rule trace, check if graph attribute and add ipl complement to rule trace as well
 					if l in interpretations_node[comp].world and interpretations_node[comp].world[l].is_static():
 						# Check if we should even store any of the changes to the rule trace etc.
 						# Inverse of this is: if not save_graph_attributes_to_rule_trace and graph_attribute
@@ -289,24 +295,26 @@
 								# Update convergence params
 								if convergence_mode=='delta_bound':
 									bound_delta = max(bound_delta, changes)
 								else:
 									changes_cnt += changes
 
 					if static:
-						facts_to_be_applied_node[i] = (numba.types.uint16(facts_to_be_applied_node[i][0]+1), comp, l, bnd, static, graph_attribute)
-					else:
-						# Add to list to be removed later
-						facts_to_remove_idx.append(i)
+						facts_to_be_applied_node_new.append((numba.types.uint16(facts_to_be_applied_node[i][0]+1), comp, l, bnd, static, graph_attribute))
+
+				# If time doesn't match, fact to be applied later
+				else:
+					facts_to_be_applied_node_new.append(facts_to_be_applied_node[i])
 
-			# Delete facts that are not static
-			facts_to_be_applied_node[:] = numba.typed.List([facts_to_be_applied_node[i] for i in range(len(facts_to_be_applied_node)) if i not in facts_to_remove_idx])
+			# Update list of facts with ones that have not been applied yet (delete applied facts)
+			facts_to_be_applied_node[:] = facts_to_be_applied_node_new.copy()
+			facts_to_be_applied_node_new.clear()
 
 			# Edges
-			facts_to_remove_idx.clear()
+			facts_to_be_applied_edge_new.clear()
 			for i in range(len(facts_to_be_applied_edge)):
 				if facts_to_be_applied_edge[i][0]==t:
 					comp, l, bnd, static, graph_attribute = facts_to_be_applied_edge[i][1], facts_to_be_applied_edge[i][2], facts_to_be_applied_edge[i][3], facts_to_be_applied_edge[i][4], facts_to_be_applied_edge[i][5]
 					# Check if bnd is static. Then no need to update, just add to rule trace, check if graph attribute, and add ipl complement to rule trace as well
 					if l in interpretations_edge[comp].world and interpretations_edge[comp].world[l].is_static():
 						# Inverse of this is: if not save_graph_attributes_to_rule_trace and graph_attribute
 						if (save_graph_attributes_to_rule_trace or not graph_attribute) and store_interpretation_changes:
@@ -346,21 +354,23 @@
 								# Update convergence params
 								if convergence_mode=='delta_bound':
 									bound_delta = max(bound_delta, changes)
 								else:
 									changes_cnt += changes
 
 					if static:
-						facts_to_be_applied_edge[i] = (numba.types.uint16(facts_to_be_applied_edge[i][0]+1), comp, l, bnd, static, graph_attribute)
-					else:
-						# Add to list to be removed later
-						facts_to_remove_idx.append(i)
+						facts_to_be_applied_edge_new.append((numba.types.uint16(facts_to_be_applied_edge[i][0]+1), comp, l, bnd, static, graph_attribute))
 
-			# Delete facts that are not static
-			facts_to_be_applied_edge[:] = numba.typed.List([facts_to_be_applied_edge[i] for i in range(len(facts_to_be_applied_edge)) if i not in facts_to_remove_idx])
+				# Time doesn't match, fact to be applied later
+				else:
+					facts_to_be_applied_edge_new.append(facts_to_be_applied_edge[i])
+
+			# Update list of facts with ones that have not been applied yet (delete applied facts)
+			facts_to_be_applied_edge[:] = facts_to_be_applied_edge_new.copy()
+			facts_to_be_applied_edge_new.clear()
 
 			in_loop = True
 			while in_loop:
 				# This will become true only if delta_t = 0 for some rule, otherwise we go to the next timestep
 				in_loop = False
 
 				# Apply the rules that need to be applied at this timestep
@@ -369,63 +379,63 @@
 				for idx, i in enumerate(rules_to_be_applied_node):
 					# If we are coming here from an immediate rule firing with delta_t=0 we have to apply that one rule. Which was just added to the list to_be_applied
 					if immediate_node_rule_fire and rules_to_be_applied_node[-1][4]:
 						i = rules_to_be_applied_node[-1]
 						idx = -1
 
 					if i[0]==t:
-						comp, l, bnd, immediate = i[1], i[2], i[3], i[4]
+						comp, l, bnd, immediate, set_static = i[1], i[2], i[3], i[4], i[5]
 						sources, targets, edge_l = edges_to_be_added_node_rule[idx]
-						edges_added, changes = _add_edges(sources, targets, neighbors, nodes, edges, edge_l, interpretations_node, interpretations_edge)
+						edges_added, changes = _add_edges(sources, targets, neighbors, reverse_neighbors, nodes, edges, edge_l, interpretations_node, interpretations_edge)
 						changes_cnt += changes
 
 						# Update bound for newly added edges. Use bnd to update all edges if label is specified, else use bnd to update normally
 						if edge_l.value!='':
 							for e in edges_added:
 								if check_consistent_edge(interpretations_edge, e, (edge_l, bnd)):
-									u, changes = _update_edge(interpretations_edge, e, (edge_l, bnd), ipl, rule_trace_edge, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_node_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, store_interpretation_changes, mode='rule')
+									u, changes = _update_edge(interpretations_edge, e, (edge_l, bnd), ipl, rule_trace_edge, fp_cnt, t, set_static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_node_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, store_interpretation_changes, mode='rule')
 
 									update = u or update
 
 									# Update convergence params
 									if convergence_mode=='delta_bound':
 										bound_delta = max(bound_delta, changes)
 									else:
 										changes_cnt += changes
 								# Resolve inconsistency
 								else:
 									if inconsistency_check:
 										resolve_inconsistency_edge(interpretations_edge, e, (edge_l, bnd), ipl, t, fp_cnt, atom_trace, rule_trace_edge, rule_trace_edge_atoms, store_interpretation_changes)
 									else:
-										u, changes = _update_edge(interpretations_edge, e, (edge_l, bnd), ipl, rule_trace_edge, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_node_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, store_interpretation_changes, mode='rule', override=True)
+										u, changes = _update_edge(interpretations_edge, e, (edge_l, bnd), ipl, rule_trace_edge, fp_cnt, t, set_static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_node_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, store_interpretation_changes, mode='rule', override=True)
 
 										update = u or update
 
 										# Update convergence params
 										if convergence_mode=='delta_bound':
 											bound_delta = max(bound_delta, changes)
 										else:
 											changes_cnt += changes
 						else:
 							# Check for inconsistencies
 							if check_consistent_node(interpretations_node, comp, (l, bnd)):
-								u, changes = _update_node(interpretations_node, comp, (l, bnd), ipl, rule_trace_node, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_node_trace, idx, facts_to_be_applied_node_trace, rule_trace_node_atoms, store_interpretation_changes, mode='rule')
+								u, changes = _update_node(interpretations_node, comp, (l, bnd), ipl, rule_trace_node, fp_cnt, t, set_static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_node_trace, idx, facts_to_be_applied_node_trace, rule_trace_node_atoms, store_interpretation_changes, mode='rule')
 
 								update = u or update
 								# Update convergence params
 								if convergence_mode=='delta_bound':
 									bound_delta = max(bound_delta, changes)
 								else:
 									changes_cnt += changes
 							# Resolve inconsistency
 							else:
 								if inconsistency_check:
 									resolve_inconsistency_node(interpretations_node, comp, (l, bnd), ipl, t, fp_cnt, atom_trace, rule_trace_node, rule_trace_node_atoms, store_interpretation_changes)
 								else:
-									u, changes = _update_node(interpretations_node, comp, (l, bnd), ipl, rule_trace_node, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_node_trace, idx, facts_to_be_applied_node_trace, rule_trace_node_atoms, store_interpretation_changes, mode='rule', override=True)
+									u, changes = _update_node(interpretations_node, comp, (l, bnd), ipl, rule_trace_node, fp_cnt, t, set_static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_node_trace, idx, facts_to_be_applied_node_trace, rule_trace_node_atoms, store_interpretation_changes, mode='rule', override=True)
 
 									update = u or update
 									# Update convergence params
 									if convergence_mode=='delta_bound':
 										bound_delta = max(bound_delta, changes)
 									else:
 										changes_cnt += changes
@@ -457,64 +467,64 @@
 						break
 					# If we are coming here from an immediate rule firing with delta_t=0 we have to apply that one rule. Which was just added to the list to_be_applied
 					if immediate_edge_rule_fire and rules_to_be_applied_edge[-1][4]:
 						i = rules_to_be_applied_edge[-1]
 						idx = -1
 
 					if i[0]==t:
-						comp, l, bnd, immediate = i[1], i[2], i[3], i[4]
+						comp, l, bnd, immediate, set_static = i[1], i[2], i[3], i[4], i[5]
 						sources, targets, edge_l = edges_to_be_added_edge_rule[idx]
-						edges_added, changes = _add_edges(sources, targets, neighbors, nodes, edges, edge_l, interpretations_node, interpretations_edge)
+						edges_added, changes = _add_edges(sources, targets, neighbors, reverse_neighbors, nodes, edges, edge_l, interpretations_node, interpretations_edge)
 						changes_cnt += changes
 
 						# Update bound for newly added edges. Use bnd to update all edges if label is specified, else use bnd to update normally
 						if edge_l.value!='':
 							for e in edges_added:
 								if check_consistent_edge(interpretations_edge, e, (edge_l, bnd)):
-									u, changes = _update_edge(interpretations_edge, e, (edge_l, bnd), ipl, rule_trace_edge, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, store_interpretation_changes, mode='rule')
+									u, changes = _update_edge(interpretations_edge, e, (edge_l, bnd), ipl, rule_trace_edge, fp_cnt, t, set_static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, store_interpretation_changes, mode='rule')
 
 									update = u or update
 
 									# Update convergence params
 									if convergence_mode=='delta_bound':
 										bound_delta = max(bound_delta, changes)
 									else:
 										changes_cnt += changes
 								# Resolve inconsistency
 								else:
 									if inconsistency_check:
 										resolve_inconsistency_edge(interpretations_edge, e, (edge_l, bnd), ipl, t, fp_cnt, atom_trace, rule_trace_edge, rule_trace_edge_atoms, store_interpretation_changes)
 									else:
-										u, changes = _update_edge(interpretations_edge, e, (edge_l, bnd), ipl, rule_trace_edge, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, store_interpretation_changes, mode='rule', override=True)
+										u, changes = _update_edge(interpretations_edge, e, (edge_l, bnd), ipl, rule_trace_edge, fp_cnt, t, set_static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, store_interpretation_changes, mode='rule', override=True)
 
 										update = u or update
 
 										# Update convergence params
 										if convergence_mode=='delta_bound':
 											bound_delta = max(bound_delta, changes)
 										else:
 											changes_cnt += changes
 
 						else:
 							# Check for inconsistencies
 							if check_consistent_edge(interpretations_edge, comp, (l, bnd)):
-								u, changes = _update_edge(interpretations_edge, comp, (l, bnd), ipl, rule_trace_edge, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, store_interpretation_changes, mode='rule')
+								u, changes = _update_edge(interpretations_edge, comp, (l, bnd), ipl, rule_trace_edge, fp_cnt, t, set_static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, store_interpretation_changes, mode='rule')
 
 								update = u or update
 								# Update convergence params
 								if convergence_mode=='delta_bound':
 									bound_delta = max(bound_delta, changes)
 								else:
 									changes_cnt += changes
 							# Resolve inconsistency
 							else:
 								if inconsistency_check:
 									resolve_inconsistency_edge(interpretations_edge, comp, (l, bnd), ipl, t, fp_cnt, atom_trace, rule_trace_edge, rule_trace_edge_atoms, store_interpretation_changes)
 								else:
-									u, changes = _update_edge(interpretations_edge, comp, (l, bnd), ipl, rule_trace_edge, fp_cnt, t, False, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, store_interpretation_changes, mode='rule', override=True)
+									u, changes = _update_edge(interpretations_edge, comp, (l, bnd), ipl, rule_trace_edge, fp_cnt, t, set_static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, idx, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, store_interpretation_changes, mode='rule', override=True)
 
 									update = u or update
 									# Update convergence params
 									if convergence_mode=='delta_bound':
 										bound_delta = max(bound_delta, changes)
 									else:
 										changes_cnt += changes
@@ -558,18 +568,19 @@
 							applicable_edge_rules = _ground_edge_rule(rule, interpretations_node, interpretations_edge, nodes, edges, neighbors, reverse_neighbors, atom_trace, reverse_graph, edges_to_skip[i])
 
 							# Loop through applicable rules and add them to the rules to be applied for later or next fp operation
 							for applicable_rule in applicable_node_rules:
 								n, annotations, qualified_nodes, qualified_edges, edges_to_add = applicable_rule
 								# If there is an edge to add or the predicate doesn't exist or the interpretation is not static
 								if len(edges_to_add[0]) > 0 or rule.get_target() not in interpretations_node[n].world or not interpretations_node[n].world[rule.get_target()].is_static():
-									bnd = influence(rule, annotations, rule.get_weights())
+									bnd = annotate(annotation_functions, rule, annotations, rule.get_weights())
+									bnd = interval.closed(bnd[0], bnd[1])
 									max_rules_time = max(max_rules_time, t + delta_t)
 									edges_to_be_added_node_rule.append(edges_to_add)
-									rules_to_be_applied_node.append((numba.types.uint16(t + delta_t), n, rule.get_target(), bnd, immediate_rule))
+									rules_to_be_applied_node.append((numba.types.uint16(t + delta_t), n, rule.get_target(), bnd, immediate_rule, rule.is_static_rule()))
 									if atom_trace:
 										rules_to_be_applied_node_trace.append((qualified_nodes, qualified_edges, rule.get_name()))
 
 									# We apply a rule on a node/edge only once in each timestep to prevent it from being added to the to_be_added list continuously (this will improve performance
 									nodes_to_skip[i].append(n)
 
 									# Handle loop parameters for the next (maybe) fp operation
@@ -589,18 +600,19 @@
 							if immediate_node_rule_fire:
 								break
 
 							for applicable_rule in applicable_edge_rules:
 								e, annotations, qualified_nodes, qualified_edges, edges_to_add = applicable_rule
 								# If there is an edge to add or the predicate doesn't exist or the interpretation is not static
 								if len(edges_to_add[0]) > 0 or rule.get_target() not in interpretations_edge[e].world or not interpretations_edge[e].world[rule.get_target()].is_static():
-									bnd = influence(rule, annotations, rule.get_weights())
+									bnd = annotate(annotation_functions, rule, annotations, rule.get_weights())
+									bnd = interval.closed(bnd[0], bnd[1])
 									max_rules_time = max(max_rules_time, t+delta_t)
 									edges_to_be_added_edge_rule.append(edges_to_add)
-									rules_to_be_applied_edge.append((numba.types.uint16(t+delta_t), e, rule.get_target(), bnd, immediate_rule))
+									rules_to_be_applied_edge.append((numba.types.uint16(t+delta_t), e, rule.get_target(), bnd, immediate_rule, rule.is_static_rule()))
 									if atom_trace:
 										rules_to_be_applied_edge_trace.append((qualified_nodes, qualified_edges, rule.get_name()))
 
 									# We apply a rule on a node/edge only once in each timestep to prevent it from being added to the to_be_added list continuously (this will improve performance
 									edges_to_skip[i].append(e)
 
 									# Handle loop parameters for the next (maybe) fp operation
@@ -656,30 +668,37 @@
 					break
 
 			# Increment t
 			t += 1
 
 		return fp_cnt, t
 
+	def add_edge(self, edge, l):
+		# This function is useful for pyreason gym, called externally
+		_add_edge(edge[0], edge[1], self.neighbors, self.reverse_neighbors, self.nodes, self.edges, l, self.interpretations_node, self.interpretations_edge)
+
+	def delete_edge(self, edge):
+		# This function is useful for pyreason gym, called externally
+		_delete_edge(edge, self.neighbors, self.reverse_neighbors, self.edges, self.interpretations_edge)
+
 
 @numba.njit(cache=True)
 def _ground_node_rule(rule, interpretations_node, interpretations_edge, nodes, neighbors, reverse_neighbors, atom_trace, reverse_graph, nodes_to_skip):
 	# Extract rule params
 	rule_type = rule.get_type()
 	clauses = rule.get_clauses()
 	thresholds = rule.get_thresholds()
 	ann_fn = rule.get_annotation_function()
-	ann_fn_label = rule.get_annotation_label()
 	rule_edges = rule.get_edges()
 
 	# We return a list of tuples which specify the target nodes/edges that have made the rule body true
 	applicable_rules = numba.typed.List.empty_list(node_applicable_rule_type)
 
-	# Return empty list if rule is not node rule
-	if rule_type != 'node':
+	# Return empty list if rule is not node rule and if we are not inferring edges
+	if rule_type != 'node' and rule_edges[0] == '':
 		return applicable_rules
 
 	# Steps
 	# 1. Loop through all nodes and evaluate each clause with that node and check the truth with the thresholds
 	# 2. Inside the clause loop it may be necessary to loop through all nodes/edges while grounding the variables
 	# 3. If the clause is true add the qualified nodes and qualified edges to the atom trace, if on. Break otherwise
 	# 4. After going through all clauses, add to the annotations list all the annotations of the specified subset. These will be passed to the annotation function
@@ -718,14 +737,21 @@
 					subset = neighbors[target_node] if clause_var_1 not in subsets else subsets[clause_var_1]
 
 				subsets[clause_var_1] = get_qualified_components_node_clause(interpretations_node, subset, clause_label, clause_bnd)
 				if atom_trace:
 					qualified_nodes.append(numba.typed.List(subsets[clause_var_1]))
 					qualified_edges.append(numba.typed.List.empty_list(edge_type))
 
+				# Add annotations if necessary
+				if ann_fn != '':
+					a = numba.typed.List.empty_list(interval.interval_type)
+					for qn in subsets[clause_var_1]:
+						a.append(interpretations_node[qn].world[clause_label])
+					annotations.append(a)
+
 			# This is an edge clause
 			# There are 5 cases for predicate(Y,Z):
 			# 1. Either one or both of Y, Z are the target node
 			# 2. Both predicate variables Y and Z have not been encountered before
 			# 3. The source variable Y has not been encountered before but the target variable Z has
 			# 4. The target variable Z has not been encountered before but the source variable Y has
 			# 5. Both predicate variables Y and Z have been encountered before
@@ -782,14 +808,21 @@
 				subsets[clause_var_1] = qe[0]
 				subsets[clause_var_2] = qe[1]
 
 				if atom_trace:
 					qualified_nodes.append(numba.typed.List.empty_list(node_type))
 					qualified_edges.append(numba.typed.List(zip(subsets[clause_var_1], subsets[clause_var_2])))
 
+				# Add annotations if necessary
+				if ann_fn != '':
+					a = numba.typed.List.empty_list(interval.interval_type)
+					for qe in numba.typed.List(zip(subsets[clause_var_1], subsets[clause_var_2])):
+						a.append(interpretations_edge[qe].world[clause_label])
+					annotations.append(a)
+
 			# Check if thresholds are satisfied
 			if threshold_quantifier_type == 'total':
 				if clause_type == 'node':
 					neigh_len = len(subset)
 				else:
 					neigh_len = sum([len(l) for l in subset_target])
 
@@ -802,32 +835,15 @@
 
 			qualified_neigh_len = len(subsets[clause_var_1])
 			satisfaction = _satisfies_threshold(neigh_len, qualified_neigh_len, thresholds[i]) and satisfaction
 			# Exit loop if even one clause is not satisfied
 			if not satisfaction:
 				break
 
-		# Here we are done going through each clause of the rule
-		# If all clauses we're satisfied, proceed to collect annotations and prepare edges to be added
 		if satisfaction:
-			# Collect the annotations that might be used in the annotation function according to the correct subset
-			for clause in clauses:
-				clause_type = clause[0]
-				clause_var_1, clause_var_2 = clause[2][0], clause[2][1]
-				if ann_fn != '':
-					a = numba.typed.List.empty_list(interval.interval_type)
-					if clause_type == 'node':
-						for qn in subsets[clause_var_1]:
-							a.append(interpretations_node[qn].world[ann_fn_label])
-					else:
-						for qe in numba.typed.List(zip(subsets[clause_var_1], subsets[clause_var_2])):
-							a.append(interpretations_edge[qe].world[ann_fn_label])
-
-					annotations.append(a)
-
 			# Collect edges to be added
 			source, target, _ = rule_edges
 
 			# Edges to be added
 			if source != '' and target != '':
 				# Check if edge nodes are target
 				if source == '__target':
@@ -853,15 +869,14 @@
 @numba.njit(cache=True)
 def _ground_edge_rule(rule, interpretations_node, interpretations_edge, nodes, edges, neighbors, reverse_neighbors, atom_trace, reverse_graph, edges_to_skip):
 	# Extract rule params
 	rule_type = rule.get_type()
 	clauses = rule.get_clauses()
 	thresholds = rule.get_thresholds()
 	ann_fn = rule.get_annotation_function()
-	ann_fn_label = rule.get_annotation_label()
 	rule_edges = rule.get_edges()
 
 	# We return a list of tuples which specify the target nodes/edges that have made the rule body true
 	applicable_rules = numba.typed.List.empty_list(edge_applicable_rule_type)
 
 	# Return empty list if rule is not node rule
 	if rule_type != 'edge':
@@ -909,14 +924,21 @@
 					subset = neighbors[target_edge[0]] if clause_var_1 not in subsets else subsets[clause_var_1]
 
 				subsets[clause_var_1] = get_qualified_components_node_clause(interpretations_node, subset, clause_label, clause_bnd)
 				if atom_trace:
 					qualified_nodes.append(numba.typed.List(subsets[clause_var_1]))
 					qualified_edges.append(numba.typed.List.empty_list(edge_type))
 
+				# Add annotations if necessary
+				if ann_fn != '':
+					a = numba.typed.List.empty_list(interval.interval_type)
+					for qn in subsets[clause_var_1]:
+						a.append(interpretations_node[qn].world[clause_label])
+					annotations.append(a)
+
 			# This is an edge clause
 			# There are 5 cases for predicate(Y,Z):
 			# 1. Either one or both of Y, Z are the source or target node
 			# 2. Both predicate variables Y and Z have not been encountered before
 			# 3. The source variable Y has not been encountered before but the target variable Z has
 			# 4. The target variable Z has not been encountered before but the source variable Y has
 			# 5. Both predicate variables Y and Z have been encountered before
@@ -993,14 +1015,21 @@
 				subsets[clause_var_1] = qe[0]
 				subsets[clause_var_2] = qe[1]
 
 				if atom_trace:
 					qualified_nodes.append(numba.typed.List.empty_list(node_type))
 					qualified_edges.append(numba.typed.List(zip(subsets[clause_var_1], subsets[clause_var_2])))
 
+				# Add annotations if necessary
+				if ann_fn != '':
+					a = numba.typed.List.empty_list(interval.interval_type)
+					for qe in numba.typed.List(zip(subsets[clause_var_1], subsets[clause_var_2])):
+						a.append(interpretations_edge[qe].world[clause_label])
+					annotations.append(a)
+
 			# Check if thresholds are satisfied
 			if threshold_quantifier_type == 'total':
 				if clause_type == 'node':
 					neigh_len = len(subset)
 				else:
 					neigh_len = sum([len(l) for l in subset_target])
 
@@ -1016,29 +1045,14 @@
 			# Exit loop if even one clause is not satisfied
 			if not satisfaction:
 				break
 
 		# Here we are done going through each clause of the rule
 		# If all clauses we're satisfied, proceed to collect annotations and prepare edges to be added
 		if satisfaction:
-			# Collect the annotations that might be used in the annotation function according to the correct subset
-			for clause in clauses:
-				clause_type = clause[0]
-				clause_var_1, clause_var_2 = clause[2][0], clause[2][1]
-				if ann_fn != '':
-					a = numba.typed.List.empty_list(interval.interval_type)
-					if clause_type == 'node':
-						for qn in subsets[clause_var_1]:
-							a.append(interpretations_node[qn].world[ann_fn_label])
-					else:
-						for qe in numba.typed.List(zip(subsets[clause_var_1], subsets[clause_var_2])):
-							a.append(interpretations_edge[qe].world[ann_fn_label])
-
-					annotations.append(a)
-
 			# Collect edges to be added
 			source, target, _ = rule_edges
 
 			# Edges to be added
 			if source != '' and target != '':
 				# Check if edge nodes are source/target
 				if source == '__source':
@@ -1348,26 +1362,24 @@
 			result = False
 	else:
 		result = True
 	return result
 
 
 @numba.njit(cache=True)
-def influence(rule, annotations, weights):
+def annotate(annotation_functions, rule, annotations, weights):
 	func_name = rule.get_annotation_function()
-	if func_name=='':
-		return interval.closed(rule.get_bnd().lower, rule.get_bnd().upper)
-	elif func_name=='average':
-		return ann_fns.average(annotations, weights)
-	elif func_name=='average_lower':
-		return ann_fns.average_lower(annotations, weights)
-	elif func_name=='minimum':
-		return ann_fns.minimum(annotations, weights)
-	elif func_name=='maximum':
-		return ann_fns.maximum(annotations, weights)
+	if func_name == '':
+		return rule.get_bnd().lower, rule.get_bnd().upper
+	else:
+		with numba.objmode(annotation='Tuple((float64, float64))'):
+			for func in annotation_functions:
+				if func.__name__ == func_name:
+					annotation = func(annotations, weights)
+		return annotation
 
 
 @numba.njit(cache=True)
 def check_consistent_node(interpretations, comp, na):
 	world = interpretations[comp]
 	if na[0] in world.world:
 		bnd = world.world[na[0]]
@@ -1446,61 +1458,71 @@
 			w.world[p1].set_lower_upper(0, 1)
 			w.world[p1].set_static(True)
 			if store_interpretation_changes:
 				rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(0,1)))
 
 
 @numba.njit(cache=True)
-def _add_node(node, neighbors, nodes, interpretations_node):
+def _add_node(node, neighbors, reverse_neighbors, nodes, interpretations_node):
 	nodes.append(node)
 	neighbors[node] = numba.typed.List.empty_list(node_type)
+	reverse_neighbors[node] = numba.typed.List.empty_list(node_type)
 	interpretations_node[node] = world.World(numba.typed.List.empty_list(label.label_type))
 
 
 @numba.njit(cache=True)
-def _add_edge(source, target, neighbors, nodes, edges, l, interpretations_node, interpretations_edge):
+def _add_edge(source, target, neighbors, reverse_neighbors, nodes, edges, l, interpretations_node, interpretations_edge):
 	# If not a node, add to list of nodes and initialize neighbors
 	if source not in nodes:
-		_add_node(source, neighbors, nodes, interpretations_node)
+		_add_node(source, neighbors, reverse_neighbors, nodes, interpretations_node)
 
 	if target not in nodes:
-		_add_node(target, neighbors, nodes, interpretations_node)
+		_add_node(target, neighbors, reverse_neighbors, nodes, interpretations_node)
 
 	# Make sure edge doesn't already exist
 	# Make sure, if l=='', not to add the label
 	# Make sure, if edge exists, that we don't override the l label if it exists
 	edge = (source, target)
 	new_edge = False
 	if edge not in edges:
 		new_edge = True
 		edges.append(edge)
 		neighbors[source].append(target)
+		reverse_neighbors[target].append(source)
 		if l.value!='':
 			interpretations_edge[edge] = world.World(numba.typed.List([l]))
 		else:
 			interpretations_edge[edge] = world.World(numba.typed.List.empty_list(label.label_type))
 	else:
 		if l not in interpretations_edge[edge].world and l.value!='':
 			new_edge = True
 			interpretations_edge[edge].world[l] = interval.closed(0, 1)
 
 	return (edge, new_edge)
 
 
 @numba.njit(cache=True)
-def _add_edges(sources, targets, neighbors, nodes, edges, l, interpretations_node, interpretations_edge):
+def _add_edges(sources, targets, neighbors, reverse_neighbors, nodes, edges, l, interpretations_node, interpretations_edge):
 	changes = 0
 	edges_added = numba.typed.List.empty_list(edge_type)
 	for source in sources:
 		for target in targets:
-			edge, new_edge = _add_edge(source, target, neighbors, nodes, edges, l, interpretations_node, interpretations_edge)
+			edge, new_edge = _add_edge(source, target, neighbors, reverse_neighbors, nodes, edges, l, interpretations_node, interpretations_edge)
 			edges_added.append(edge)
 			changes = changes+1 if new_edge else changes
 	return (edges_added, changes)
 
+@numba.njit(cache=True)
+def _delete_edge(edge, neighbors, reverse_neighbors, edges, interpretations_edge):
+	source, target = edge
+	edges.remove(edge)
+	del interpretations_edge[edge]
+	neighbors[source].remove(target)
+	reverse_neighbors[target].remove(source)
+
 
 @numba.njit(cache=True)
 def float_to_str(value):
 	number = int(value)
 	decimal = int(value % 1 * 1000)
 	float_str = f'{number}.{decimal}'
 	return float_str
```

### Comparing `pyreason-1.8.2/pyreason/scripts/interval/interval.py` & `pyreason-1.8.3/pyreason/scripts/interval/interval.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py` & `pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py` & `pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/interval_type.py` & `pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/interval_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/label_type.py` & `pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/label_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/rule_type.py` & `pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/rule_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,84 +28,84 @@
 def typeof_rule(val, c):
     return rule_type
 
 
 # Construct object from Numba functions (Doesn't work. We don't need this currently)
 @type_callable(Rule)
 def type_rule(context):
-    def typer(rule_str, type, target, delta, clauses, bnd, thresholds, ann_fn, ann_label, weights, edges, immediate_rule):
-        if isinstance(rule_str, types.UnicodeType) and isinstance(type, types.UnicodeType) and isinstance(target, label.LabelType) and isinstance(delta, types.Integer) and isinstance(clauses, (types.NoneType, types.ListType)) and isinstance(bnd, interval.IntervalType) and isinstance(thresholds, types.ListType) and isinstance(ann_fn, types.UnicodeType) and isinstance(ann_label, label.LabelType) and isinstance(weights, types.Array) and isinstance(edges, types.Tuple) and isinstance(immediate_rule, types.Boolean):
+    def typer(rule_name, type, target, delta, clauses, bnd, thresholds, ann_fn, weights, edges, static,immediate_rule):
+        if isinstance(rule_name, types.UnicodeType) and isinstance(type, types.UnicodeType) and isinstance(target, label.LabelType) and isinstance(delta, types.Integer) and isinstance(clauses, (types.NoneType, types.ListType)) and isinstance(bnd, interval.IntervalType) and isinstance(thresholds, types.ListType) and isinstance(ann_fn, types.UnicodeType) and isinstance(weights, types.Array) and isinstance(edges, types.Tuple) and isinstance(static, types.Boolean) and isinstance(immediate_rule, types.Boolean):
             return rule_type
     return typer
 
 
 # Define native representation: data-model
 @register_model(RuleType)
 class RuleModel(models.StructModel):
     def __init__(self, dmm, fe_type):
         members = [
-            ('rule_str', types.string),
+            ('rule_name', types.string),
             ('type', types.string),
             ('target', label.label_type),
             ('delta', types.uint16),
             ('clauses', types.ListType(types.Tuple((types.string, label.label_type, types.UniTuple(types.string, 2), interval.interval_type)))),
             ('bnd', interval.interval_type),
             ('thresholds', types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), types.float64)))),
             ('ann_fn', types.string),
-            ('ann_label', label.label_type),
             ('weights', types.float64[::1]),
             ('edges', types.Tuple((types.string, types.string, label.label_type))),
+            ('static', types.boolean),
             ('immediate_rule', types.boolean)
             ]
         models.StructModel.__init__(self, dmm, fe_type, members)
 
 
 # Expose data-model attributes
-make_attribute_wrapper(RuleType, 'rule_str', 'rule_str')
+make_attribute_wrapper(RuleType, 'rule_name', 'rule_name')
 make_attribute_wrapper(RuleType, 'type', 'type')
 make_attribute_wrapper(RuleType, 'target', 'target')
 make_attribute_wrapper(RuleType, 'delta', 'delta')
 make_attribute_wrapper(RuleType, 'clauses', 'clauses')
 make_attribute_wrapper(RuleType, 'bnd', 'bnd')
 make_attribute_wrapper(RuleType, 'thresholds', 'thresholds')
 make_attribute_wrapper(RuleType, 'ann_fn', 'ann_fn')
-make_attribute_wrapper(RuleType, 'ann_label', 'ann_label')
 make_attribute_wrapper(RuleType, 'weights', 'weights')
 make_attribute_wrapper(RuleType, 'edges', 'edges')
+make_attribute_wrapper(RuleType, 'static', 'static')
 make_attribute_wrapper(RuleType, 'immediate_rule', 'immediate_rule')
 
 
 # Implement constructor
-@lower_builtin(Rule, types.string, types.string, label.label_type, types.uint16, types.ListType(types.Tuple((types.string, label.label_type, types.UniTuple(types.string, 2), interval.interval_type))), interval.interval_type, types.ListType(types.ListType(types.Tuple((types.string, types.string, types.float64)))), types.string, label.label_type, types.float64[::1], types.Tuple((types.string, types.string, label.label_type)), types.boolean)
+@lower_builtin(Rule, types.string, types.string, label.label_type, types.uint16, types.ListType(types.Tuple((types.string, label.label_type, types.UniTuple(types.string, 2), interval.interval_type))), interval.interval_type, types.ListType(types.ListType(types.Tuple((types.string, types.string, types.float64)))), types.string, types.float64[::1], types.Tuple((types.string, types.string, label.label_type)), types.boolean, types.boolean)
 def impl_rule(context, builder, sig, args):
     typ = sig.return_type
-    rule_str, type, target, delta, clauses, bnd, thresholds, ann_fn, ann_label, weights, edges, immediate_rule = args
+    rule_name, type, target, delta, clauses, bnd, thresholds, ann_fn, weights, edges, static, immediate_rule = args
     context.nrt.incref(builder, types.ListType(types.Tuple((types.string, label.label_type, types.UniTuple(types.string, 2), interval.interval_type))), clauses)
     context.nrt.incref(builder, types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), types.float64))), thresholds)
     rule = cgutils.create_struct_proxy(typ)(context, builder)
-    rule.rule_str = rule_str
+    rule.rule_name = rule_name
     rule.type = type
     rule.target = target
     rule.delta = delta
     rule.clauses = clauses
     rule.bnd = bnd
     rule.thresholds = thresholds
     rule.ann_fn = ann_fn
-    rule.ann_label = ann_label
     rule.weights = weights
     rule.edges = edges
+    rule.static = static
     rule.immediate_rule = immediate_rule
     return rule._getvalue()
 
 
 # Expose properties
 @overload_method(RuleType, "get_name")
 def get_name(rule):
     def getter(rule):
-        return rule.rule_str
+        return rule.rule_name
     return getter
 
 
 @overload_method(RuleType, "get_type")
 def get_type(rule):
     def getter(rule):
         return rule.type
@@ -150,110 +150,110 @@
 @overload_method(RuleType, "get_annotation_function")
 def get_annotation_function(rule):
     def impl(rule):
         return rule.ann_fn
     return impl
 
 
-@overload_method(RuleType, "get_annotation_label")
-def get_label(rule):
-    def impl(rule):
-        return rule.ann_label
-    return impl
-
-
 @overload_method(RuleType, "get_weights")
 def get_weights(rule):
     def impl(rule):
         return rule.weights
     return impl
 
 
 @overload_method(RuleType, "get_edges")
 def get_edges(rule):
     def impl(rule):
         return rule.edges
     return impl
 
 
+@overload_method(RuleType, "is_static_rule")
+def is_static_rule(rule):
+    def impl(rule):
+        return rule.static
+    return impl
+
+
 @overload_method(RuleType, "is_immediate_rule")
 def is_immediate_rule(rule):
     def impl(rule):
         return rule.immediate_rule
     return impl
 
 
 # Tell numba how to make native
 @unbox(RuleType)
 def unbox_rule(typ, obj, c):
-    name_obj = c.pyapi.object_getattr_string(obj, "_rule_str")
+    name_obj = c.pyapi.object_getattr_string(obj, "_rule_name")
     type_obj = c.pyapi.object_getattr_string(obj, "_type")
     target_obj = c.pyapi.object_getattr_string(obj, "_target")
     delta_obj = c.pyapi.object_getattr_string(obj, "_delta")
     clauses_obj = c.pyapi.object_getattr_string(obj, "_clauses")
     bnd_obj = c.pyapi.object_getattr_string(obj, "_bnd")
     thresholds_obj = c.pyapi.object_getattr_string(obj, "_thresholds")
     ann_fn_obj = c.pyapi.object_getattr_string(obj, "_ann_fn")
-    ann_label_obj = c.pyapi.object_getattr_string(obj, "_ann_label")
     weights_obj = c.pyapi.object_getattr_string(obj, "_weights")
     edges_obj = c.pyapi.object_getattr_string(obj, "_edges")
+    static_obj = c.pyapi.object_getattr_string(obj, "_static")
     immediate_rule_obj = c.pyapi.object_getattr_string(obj, "_immediate_rule")
     rule = cgutils.create_struct_proxy(typ)(c.context, c.builder)
-    rule.rule_str = c.unbox(types.string, name_obj).value
+    rule.rule_name = c.unbox(types.string, name_obj).value
     rule.type = c.unbox(types.string, type_obj).value
     rule.target = c.unbox(label.label_type, target_obj).value
     rule.delta = c.unbox(types.uint16, delta_obj).value
     rule.clauses = c.unbox(types.ListType(types.Tuple((types.string, label.label_type, types.UniTuple(types.string, 2), interval.interval_type))), clauses_obj).value
     rule.bnd = c.unbox(interval.interval_type, bnd_obj).value
     rule.thresholds = c.unbox(types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), types.float64))), thresholds_obj).value
     rule.ann_fn = c.unbox(types.string, ann_fn_obj).value
-    rule.ann_label = c.unbox(label.label_type, ann_label_obj).value
     rule.weights = c.unbox(types.float64[::1], weights_obj).value
     rule.edges = c.unbox(types.Tuple((types.string, types.string, label.label_type)), edges_obj).value
+    rule.static = c.unbox(types.boolean, static_obj).value
     rule.immediate_rule = c.unbox(types.boolean, immediate_rule_obj).value
     c.pyapi.decref(name_obj)
     c.pyapi.decref(type_obj)
     c.pyapi.decref(target_obj)
     c.pyapi.decref(delta_obj)
     c.pyapi.decref(clauses_obj)
     c.pyapi.decref(bnd_obj)
     c.pyapi.decref(thresholds_obj)
     c.pyapi.decref(ann_fn_obj)
-    c.pyapi.decref(ann_label_obj)
     c.pyapi.decref(weights_obj)
     c.pyapi.decref(edges_obj)
+    c.pyapi.decref(static_obj)
     c.pyapi.decref(immediate_rule_obj)
     is_error = cgutils.is_not_null(c.builder, c.pyapi.err_occurred())
     return NativeValue(rule._getvalue(), is_error=is_error)
 
 
 @box(RuleType)
 def box_rule(typ, val, c):
     rule = cgutils.create_struct_proxy(typ)(c.context, c.builder, value=val)
     class_obj = c.pyapi.unserialize(c.pyapi.serialize_object(Rule))
-    name_obj = c.box(types.string, rule.rule_str)
+    name_obj = c.box(types.string, rule.rule_name)
     type_obj = c.box(types.string, rule.type)
     target_obj = c.box(label.label_type, rule.target)
     delta_obj = c.box(types.uint16, rule.delta)
     clauses_obj = c.box(types.ListType(types.Tuple((types.string, label.label_type, types.UniTuple(types.string, 2), interval.interval_type))), rule.clauses)
     bnd_obj = c.box(interval.interval_type, rule.bnd)
     thresholds_obj = c.box(types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), types.float64))), rule.thresholds)
     ann_fn_obj = c.box(types.string, rule.ann_fn)
-    ann_label_obj = c.box(label.label_type, rule.ann_label)
     weights_obj = c.box(types.float64[::1], rule.weights)
     edges_obj = c.box(types.Tuple((types.string, types.string, label.label_type)), rule.edges)
+    static_obj = c.box(types.boolean, rule.static)
     immediate_rule_obj = c.box(types.boolean, rule.immediate_rule)
-    res = c.pyapi.call_function_objargs(class_obj, (name_obj, type_obj, target_obj, delta_obj, clauses_obj, bnd_obj, thresholds_obj, ann_fn_obj, ann_label_obj, weights_obj, edges_obj, immediate_rule_obj))
+    res = c.pyapi.call_function_objargs(class_obj, (name_obj, type_obj, target_obj, delta_obj, clauses_obj, bnd_obj, thresholds_obj, ann_fn_obj, weights_obj, edges_obj, static_obj, immediate_rule_obj))
     c.pyapi.decref(name_obj)
     c.pyapi.decref(type_obj)
     c.pyapi.decref(target_obj)
     c.pyapi.decref(delta_obj)
     c.pyapi.decref(clauses_obj)
     c.pyapi.decref(ann_fn_obj)
     c.pyapi.decref(bnd_obj)
     c.pyapi.decref(thresholds_obj)
-    c.pyapi.decref(ann_label_obj)
     c.pyapi.decref(weights_obj)
     c.pyapi.decref(edges_obj)
+    c.pyapi.decref(static_obj)
     c.pyapi.decref(immediate_rule_obj)
     c.pyapi.decref(class_obj)
     return res
```

### Comparing `pyreason-1.8.2/pyreason/scripts/numba_wrapper/numba_types/world_type.py` & `pyreason-1.8.3/pyreason/scripts/numba_wrapper/numba_types/world_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/scripts/program/program.py` & `pyreason-1.8.3/pyreason/scripts/program/program.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 
 class Program:
 	available_labels_node = []
 	available_labels_edge = []
 	specific_node_labels = []
 	specific_edge_labels = []
 
-	def __init__(self, graph, facts_node, facts_edge, rules, ipl, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, store_interpretation_changes):
+	def __init__(self, graph, facts_node, facts_edge, rules, ipl, annotation_functions, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, store_interpretation_changes):
 		self._graph = graph
 		self._facts_node = facts_node
 		self._facts_edge = facts_edge
 		self._rules = rules
 		self._ipl = ipl
+		self._annotation_functions = annotation_functions
 		self._reverse_graph = reverse_graph
 		self._atom_trace = atom_trace
 		self._save_graph_attributes_to_rule_trace = save_graph_attributes_to_rule_trace
 		self._canonical = canonical
 		self._inconsistency_check = inconsistency_check
 		self._store_interpretation_changes = store_interpretation_changes
 		self.interp = None
@@ -25,15 +26,15 @@
 		self._tmax = tmax
 		# Set up available labels
 		Interpretation.available_labels_node = self.available_labels_node
 		Interpretation.available_labels_edge = self.available_labels_edge
 		Interpretation.specific_node_labels = self.specific_node_labels
 		Interpretation.specific_edge_labels = self.specific_edge_labels
 
-		self.interp = Interpretation(self._graph, self._ipl, self._reverse_graph, self._atom_trace, self._save_graph_attributes_to_rule_trace, self._canonical, self._inconsistency_check, self._store_interpretation_changes)
+		self.interp = Interpretation(self._graph, self._ipl, self._annotation_functions, self._reverse_graph, self._atom_trace, self._save_graph_attributes_to_rule_trace, self._canonical, self._inconsistency_check, self._store_interpretation_changes)
 		self.interp.start_fp(self._tmax, self._facts_node, self._facts_edge, self._rules, verbose, convergence_threshold, convergence_bound_threshold)
 
 		return self.interp
 	
 	def reason_again(self, tmax, convergence_threshold, convergence_bound_threshold, facts_node, facts_edge, verbose=True):
 		assert self.interp is not None, 'Call reason before calling reason again'
 		self._tmax = self.interp.time + tmax
```

### Comparing `pyreason-1.8.2/pyreason/scripts/rules/rule.py` & `pyreason-1.8.3/pyreason/scripts/rules/rule.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 class Rule:
 
-    def __init__(self, rule_str, rule_type, target, delta, clauses, bnd, thresholds, ann_fn, ann_label, weights, edges, immediate_rule):
-        self._rule_str = rule_str
+    def __init__(self, rule_name, rule_type, target, delta, clauses, bnd, thresholds, ann_fn, weights, edges, static, immediate_rule):
+        self._rule_name = rule_name
         self._type = rule_type
         self._target = target
         self._delta = delta
         self._clauses = clauses
         self._bnd = bnd
         self._thresholds = thresholds
         self._ann_fn = ann_fn
-        self._ann_label = ann_label
         self._weights = weights
         self._edges = edges
+        self._static = static
         self._immediate_rule = immediate_rule
 
-    def get_rule_str(self):
-        return self._rule_str
+    def get_rule_name(self):
+        return self._rule_name
 
     def get_rule_type(self):
         return self._type
 
     def get_target(self):
         return self._target
 
@@ -33,16 +33,16 @@
         return self._bnd
 
     def get_thresholds(self):
         return self._thresholds 
 
     def get_annotation_function(self):
         return self._ann_fn
-
-    def get_ann_label(self):
-        return self._ann_label
     
     def get_edges(self):
         return self._edges
 
+    def is_static(self):
+        return self._static
+
     def is_immediate_rule(self):
         return self._immediate_rule
```

### Comparing `pyreason-1.8.2/pyreason/scripts/utils/filter.py` & `pyreason-1.8.3/pyreason/scripts/utils/filter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/scripts/utils/graphml_parser.py` & `pyreason-1.8.3/pyreason/scripts/utils/graphml_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,26 +10,29 @@
 class GraphmlParser:
     def __init__(self):
         self.graph = None
         self.non_fluent_facts = None
 
     def parse_graph(self, graph_path, reverse):
         self.graph = nx.read_graphml(graph_path)
+        self.graph = nx.DiGraph(self.graph)
         if reverse:
             self.graph = self.graph.reverse()
 
         return self.graph
 
+    def load_graph(self, graph):
+        self.graph = nx.DiGraph(graph)
+        return self.graph
+
     def parse_graph_attributes(self, static_facts):
         facts_node = numba.typed.List.empty_list(fact_node.fact_type)
         facts_edge = numba.typed.List.empty_list(fact_edge.fact_type)
-        specific_node_labels = numba.typed.Dict.empty(key_type=label.label_type,
-                                                      value_type=numba.types.ListType(numba.types.string))
-        specific_edge_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(
-            numba.types.Tuple((numba.types.string, numba.types.string))))
+        specific_node_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(numba.types.string))
+        specific_edge_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(numba.types.Tuple((numba.types.string, numba.types.string))))
         for n in self.graph.nodes:
             for key, value in self.graph.nodes[n].items():
                 # IF attribute is a float or int and it is less than 1, then make it a bound, else make it a label
                 if (isinstance(value, (float, int)) and 1 >= value >= 0) or (
                         isinstance(value, str) and value.replace('.', '').isdigit() and 1 >= float(value) >= 0):
                     l = str(key)
                     l_bnd = float(value)
@@ -50,16 +53,15 @@
                                 l = str(key)
                         except:
                             pass
 
                 if label.Label(l) not in specific_node_labels.keys():
                     specific_node_labels[label.Label(l)] = numba.typed.List.empty_list(numba.types.string)
                 specific_node_labels[label.Label(l)].append(n)
-                f = fact_node.Fact('graph-attribute-fact', n, label.Label(l), interval.closed(l_bnd, u_bnd), 0, 0,
-                                   static=static_facts)
+                f = fact_node.Fact('graph-attribute-fact', n, label.Label(l), interval.closed(l_bnd, u_bnd), 0, 0, static=static_facts)
                 facts_node.append(f)
         for e in self.graph.edges:
             for key, value in self.graph.edges[e].items():
                 # IF attribute is a float or int and it is less than 1, then make it a bound, else make it a label
                 if (isinstance(value, (float, int)) and 1 >= value >= 0) or (
                         isinstance(value, str) and value.replace('.', '').isdigit() and 1 >= float(value) >= 0):
                     l = str(key)
@@ -79,15 +81,13 @@
                                 l_bnd = low
                                 u_bnd = up
                                 l = str(key)
                         except:
                             pass
 
                 if label.Label(l) not in specific_edge_labels.keys():
-                    specific_edge_labels[label.Label(l)] = numba.typed.List.empty_list(
-                        numba.types.Tuple((numba.types.string, numba.types.string)))
+                    specific_edge_labels[label.Label(l)] = numba.typed.List.empty_list(numba.types.Tuple((numba.types.string, numba.types.string)))
                 specific_edge_labels[label.Label(l)].append((e[0], e[1]))
-                f = fact_edge.Fact('graph-attribute-fact', (e[0], e[1]), label.Label(l), interval.closed(l_bnd, u_bnd),
-                                   0, 0, static=static_facts)
+                f = fact_edge.Fact('graph-attribute-fact', (e[0], e[1]), label.Label(l), interval.closed(l_bnd, u_bnd), 0, 0, static=static_facts)
                 facts_edge.append(f)
 
-        return facts_node, facts_edge, specific_node_labels, specific_edge_labels                
+        return facts_node, facts_edge, specific_node_labels, specific_edge_labels
```

### Comparing `pyreason-1.8.2/pyreason/scripts/utils/output.py` & `pyreason-1.8.3/pyreason/scripts/utils/output.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/scripts/utils/plotter.py` & `pyreason-1.8.3/pyreason/scripts/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/scripts/utils/rule_parser.py` & `pyreason-1.8.3/pyreason/scripts/utils/rule_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 
 import pyreason.scripts.numba_wrapper.numba_types.rule_type as rule
 import pyreason.scripts.numba_wrapper.numba_types.label_type as label
 import pyreason.scripts.numba_wrapper.numba_types.interval_type as interval
 
 
-def parse_rule(rule_text: str, name: str, infer_edges: bool = False, immediate_rule: bool = False) -> rule.Rule:
+def parse_rule(rule_text: str, name: str, infer_edges: bool = False, set_static: bool = False, immediate_rule: bool = False) -> rule.Rule:
     # First remove all spaces from line
     r = rule_text.replace(' ', '')
 
     # Separate into head and body
     head, body = r.split('<-')
 
     # Extract delta_t of rule if it exists else set it to 0
@@ -67,19 +67,34 @@
 
     # 7
     for i in range(len(body_bounds)):
         bound = body_bounds[i]
         l, u = _str_bound_to_bound(bound)
         body_bounds[i] = [l, u]
 
-    # Find the target predicate
-    if head[-1] != ']':
+    # Find the target predicate and bounds and annotation function if any.
+    # Possible heads:
+    # pred(x) : [x,y]
+    # pred(x) : f
+    # pred(x)
+
+    # This means there is no bound or annotation function specified
+    if head[-1] == ')':
         head += ':[1,1]'
+
     head, head_bound = head.split(':')
-    target_bound = list(_str_bound_to_bound(head_bound))
+    # Check if we have a bound or annotation function
+    if _is_bound(head_bound):
+        target_bound = list(_str_bound_to_bound(head_bound))
+        target_bound = interval.closed(*target_bound)
+        ann_fn = ''
+    else:
+        target_bound = interval.closed(0, 1)
+        ann_fn = head_bound
+
     idx = head.find('(')
     target = head[:idx]
     target = label.Label(target)
 
     # Variable(s) in the head of the rule
     end_idx = head.find(')')
     head_variables = head[idx + 1:end_idx].split(',')
@@ -91,14 +106,18 @@
     body_predicates = []
     body_variables = []
     for clause in body_clauses:
         idx = clause.find('(')
         body_predicates.append(clause[:idx])
         body_variables.append(clause[idx+1:-1].split(','))
 
+    # Change infer edge parameter if it's a node rule
+    if rule_type == 'node':
+        infer_edges = False
+
     # Replace the variables in the body with source/target if they match the variables in the head
     # If infer_edges is true, then we consider all rules to be node rules, we infer the 2nd variable of the target predicate from the rule body
     # Else we consider the rule to be an edge rule and replace variables with source/target
     # Node rules with possibility of adding edges
     if infer_edges or len(head_variables) == 1:
         head_source_variable = head_variables[0]
         for i in range(len(body_variables)):
@@ -138,30 +157,40 @@
         quantifier_type = ('number', 'total')
         thresh = 1
         thresholds.append((quantifier, quantifier_type, thresh))
 
     # Assert that there are two variables in the head of the rule if we infer edges
     # Add edges between head variables if necessary
     if infer_edges:
-        assert len(head_variables) == 2, 'Cannot infer edges with a node rule. There have to be two variables in the head'
         var = '__target' if head_variables[0] == head_variables[1] else head_variables[1]
         edges = ('__target', var, target)
     else:
         edges = ('', '', label.Label(''))
 
-    # Bound to set atom if rule fires
-    bnd = interval.closed(*target_bound)
-    ann_fn = ''
-    ann_label = label.Label('')
-
     weights = np.ones(len(body_predicates), dtype=np.float64)
     weights = np.append(weights, 0)
 
-    r = rule.Rule(name, rule_type, target, numba.types.uint16(t), clauses, bnd, thresholds, ann_fn, ann_label, weights, edges, immediate_rule)
+    r = rule.Rule(name, rule_type, target, numba.types.uint16(t), clauses, target_bound, thresholds, ann_fn, weights, edges, set_static, immediate_rule)
     return r
 
 
 def _str_bound_to_bound(str_bound):
     str_bound = str_bound.replace('[', '')
     str_bound = str_bound.replace(']', '')
     l, u = str_bound.split(',')
     return float(l), float(u)
+
+def _is_bound(str_bound):
+    str_bound = str_bound.replace('[', '')
+    str_bound = str_bound.replace(']', '')
+    try:
+        l, u = str_bound.split(',')
+        l = l.replace('.', '')
+        u = u.replace('.', '')
+        if l.isdigit() and u.isdigit():
+            result = True
+        else:
+            result = False
+    except:
+        result = False
+
+    return result
```

### Comparing `pyreason-1.8.2/pyreason/scripts/utils/visuals.py` & `pyreason-1.8.3/pyreason/scripts/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason/scripts/utils/yaml_parser.py` & `pyreason-1.8.3/pyreason/scripts/utils/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/pyreason.egg-info/PKG-INFO` & `pyreason-1.8.3/pyreason.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.8.2
+Version: 1.8.3
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.8.2/pyreason.egg-info/SOURCES.txt` & `pyreason-1.8.3/pyreason.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.2/setup.py` & `pyreason-1.8.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pyreason',
-    version='1.8.2',
+    version='1.8.3',
     author='Dyuman Aditya',
     author_email='dyuman.aditya@gmail.com',
     description='An explainable inference software supporting annotated, real valued, graph based and temporal logic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/lab-v2/pyreason',
     license='BSD 3-clause',
```

### Comparing `pyreason-1.8.2/tests/test_hello_world.py` & `pyreason-1.8.3/tests/test_hello_world.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     # Modify the paths based on where you've stored the files we made above
     graph_path = './tests/friends_graph.graphml'
 
     # Modify pyreason settings to make verbose and to save the rule trace to a file
     pr.settings.verbose = True     # Print info to screen
 
     # Load all the files into pyreason
-    pr.load_graph(graph_path)
+    pr.load_graphml(graph_path)
     pr.add_rule('popular(x) <-1 popular(y), Friends(x,y), owns(y,z), owns(x,z)', 'popular_rule')
     pr.add_fact(pr.Fact('popular-fact', 'Mary', 'popular', [1, 1], 0, 2))
 
     # Run the program for two timesteps to see the diffusion take place
     interpretation = pr.reason(timesteps=2)
 
     # Display the changes in the interpretation for each timestep
```

