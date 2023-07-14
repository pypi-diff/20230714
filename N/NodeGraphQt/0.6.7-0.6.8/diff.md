# Comparing `tmp/NodeGraphQt-0.6.7.tar.gz` & `tmp/NodeGraphQt-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NodeGraphQt-0.6.7.tar", last modified: Thu Jul 13 12:39:52 2023, max compression
+gzip compressed data, was "NodeGraphQt-0.6.8.tar", last modified: Fri Jul 14 08:11:28 2023, max compression
```

## Comparing `NodeGraphQt-0.6.7.tar` & `NodeGraphQt-0.6.8.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.867165 NodeGraphQt-0.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.859164 NodeGraphQt-0.6.7/NodeGraphQt/
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.863164 NodeGraphQt-0.6.7/NodeGraphQt/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/base/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/base/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)   101117 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/base/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/base/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    20287 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/base/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/base/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/base/port.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.863164 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/nodes_palette.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/nodes_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.863164 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    26941 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.863164 NodeGraphQt-0.6.7/NodeGraphQt/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/nodes/backdrop_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    27955 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/nodes/base_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/nodes/base_node_circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/nodes/group_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/nodes/port_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/pkg_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.867165 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_backdrop.py
--rw-r--r--   0 runner    (1001) docker     (123)    36302 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_circle.py
--rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_overlay_disabled.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_port_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_port_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_text_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    23109 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/port.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/slicer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.867165 NodeGraphQt-0.6.7/NodeGraphQt/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/widgets/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/widgets/dialogs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.867165 NodeGraphQt-0.6.7/NodeGraphQt/widgets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/widgets/icons/node_base.png
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/widgets/node_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/widgets/node_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/widgets/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/widgets/tab_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    54896 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/widgets/viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/NodeGraphQt/widgets/viewer_nav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.863164 NodeGraphQt-0.6.7/NodeGraphQt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-13 12:39:52.000000 NodeGraphQt-0.6.7/NodeGraphQt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-13 12:39:52.000000 NodeGraphQt-0.6.7/NodeGraphQt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:39:52.000000 NodeGraphQt-0.6.7/NodeGraphQt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 12:39:52.000000 NodeGraphQt-0.6.7/NodeGraphQt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-13 12:39:52.000000 NodeGraphQt-0.6.7/NodeGraphQt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-13 12:39:52.867165 NodeGraphQt-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.859164 NodeGraphQt-0.6.7/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.867165 NodeGraphQt-0.6.7/examples/hotkeys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/examples/hotkeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/examples/hotkeys/hotkey_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:52.867165 NodeGraphQt-0.6.7/examples/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/examples/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/examples/nodes/basic_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/examples/nodes/custom_ports_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/examples/nodes/group_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/examples/nodes/widget_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-13 12:39:52.871165 NodeGraphQt-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-13 12:39:44.000000 NodeGraphQt-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.620957 NodeGraphQt-0.6.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.608956 NodeGraphQt-0.6.8/NodeGraphQt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.612956 NodeGraphQt-0.6.8/NodeGraphQt/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/base/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/base/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101486 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/base/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/base/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20287 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/base/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/base/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/base/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.612956 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/nodes_palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/nodes_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.616956 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.616956 NodeGraphQt-0.6.8/NodeGraphQt/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/nodes/backdrop_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27955 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/nodes/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/nodes/base_node_circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/nodes/group_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/nodes/port_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/pkg_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.620957 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_backdrop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36302 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_overlay_disabled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_port_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_port_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_text_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23109 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/slicer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.620957 NodeGraphQt-0.6.8/NodeGraphQt/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/widgets/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/widgets/dialogs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.620957 NodeGraphQt-0.6.8/NodeGraphQt/widgets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/widgets/icons/node_base.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/widgets/node_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/widgets/node_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/widgets/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/widgets/tab_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54896 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/widgets/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/NodeGraphQt/widgets/viewer_nav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.612956 NodeGraphQt-0.6.8/NodeGraphQt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-14 08:11:28.000000 NodeGraphQt-0.6.8/NodeGraphQt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-14 08:11:28.000000 NodeGraphQt-0.6.8/NodeGraphQt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:11:28.000000 NodeGraphQt-0.6.8/NodeGraphQt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 08:11:28.000000 NodeGraphQt-0.6.8/NodeGraphQt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-14 08:11:28.000000 NodeGraphQt-0.6.8/NodeGraphQt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-14 08:11:28.620957 NodeGraphQt-0.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.608956 NodeGraphQt-0.6.8/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.620957 NodeGraphQt-0.6.8/examples/hotkeys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/examples/hotkeys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/examples/hotkeys/hotkey_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:28.620957 NodeGraphQt-0.6.8/examples/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/examples/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/examples/nodes/basic_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/examples/nodes/custom_ports_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/examples/nodes/group_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/examples/nodes/widget_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-14 08:11:28.624957 NodeGraphQt-0.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-14 08:11:19.000000 NodeGraphQt-0.6.8/setup.py
```

### Comparing `NodeGraphQt-0.6.7/LICENSE.md` & `NodeGraphQt-0.6.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/__init__.py` & `NodeGraphQt-0.6.8/NodeGraphQt/__init__.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/base/commands.py` & `NodeGraphQt-0.6.8/NodeGraphQt/base/commands.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/base/factory.py` & `NodeGraphQt-0.6.8/NodeGraphQt/base/factory.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/base/graph.py` & `NodeGraphQt-0.6.8/NodeGraphQt/base/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1546,14 +1546,26 @@
         """
         Clears the selection in the node graph.
         """
         self._undo_stack.beginMacro('clear selection')
         [node.set_selected(False) for node in self.all_nodes()]
         self._undo_stack.endMacro()
 
+    def invert_selection(self):
+        """
+        Inverts the current node selection.
+        """
+        if not self.selected_nodes():
+            self.select_all()
+            return
+        self._undo_stack.beginMacro('invert selection')
+        for node in self.all_nodes():
+            node.set_selected(not node.selected())
+        self._undo_stack.endMacro()
+
     def get_node_by_id(self, node_id=None):
         """
         Returns the node from the node id string.
 
         Args:
             node_id (str): node id (:attr:`NodeObject.id`)
```

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/base/menu.py` & `NodeGraphQt-0.6.8/NodeGraphQt/base/menu.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/base/model.py` & `NodeGraphQt-0.6.8/NodeGraphQt/base/model.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/base/node.py` & `NodeGraphQt-0.6.8/NodeGraphQt/base/node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/base/port.py` & `NodeGraphQt-0.6.8/NodeGraphQt/base/port.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/constants.py` & `NodeGraphQt-0.6.8/NodeGraphQt/constants.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/nodes_palette.py` & `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/nodes_palette.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/nodes_tree.py` & `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/nodes_tree.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py` & `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py` & `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py` & `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py` & `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py` & `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py` & `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py` & `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,17 +51,19 @@
         self.setItemDelegate(_PropertiesDelegate())
         self.setColumnCount(1)
         self.setShowGrid(False)
         self.verticalHeader().hide()
         self.horizontalHeader().hide()
 
         QtCompat.QHeaderView.setSectionResizeMode(
-            self.verticalHeader(), QtWidgets.QHeaderView.ResizeToContents)
+            self.verticalHeader(), QtWidgets.QHeaderView.ResizeToContents
+        )
         QtCompat.QHeaderView.setSectionResizeMode(
-            self.horizontalHeader(), 0, QtWidgets.QHeaderView.Stretch)
+            self.horizontalHeader(), 0, QtWidgets.QHeaderView.Stretch
+        )
         self.setVerticalScrollMode(QtWidgets.QAbstractItemView.ScrollPerPixel)
 
     def wheelEvent(self, event):
         """
         Args:
             event (QtGui.QWheelEvent):
         """
@@ -144,20 +146,22 @@
 
     def __init__(self, parent=None, node=None):
         super(_PortConnectionsContainer, self).__init__(parent)
         self._node = node
         self._ports = {}
 
         in_group, self.in_tree = self._build_tree_group('Input Ports')
+        in_group.setToolTip('Display input port connections')
         for _, port in node.inputs().items():
             self._build_row(self.in_tree, port)
         for col in range(self.in_tree.columnCount()):
             self.in_tree.resizeColumnToContents(col)
 
         out_group, self.out_tree = self._build_tree_group('Output Ports')
+        out_group.setToolTip('Display output port connections')
         for _, port in node.outputs().items():
             self._build_row(self.out_tree, port)
         for col in range(self.out_tree.columnCount()):
             self.out_tree.resizeColumnToContents(col)
 
         layout = QtWidgets.QVBoxLayout(self)
         layout.addWidget(in_group)
@@ -223,15 +227,15 @@
         item.setText(1, port.name())
         item.setToolTip(0, 'Lock Port')
         item.setToolTip(1, 'Port Name')
         item.setToolTip(2, 'Select connected port.')
         item.setToolTip(3, 'Center on connected port node.')
 
         # TODO: will need to update this checkbox lock logic to work with
-        #       the unde/redo functionality.
+        #       the undo/redo functionality.
         lock_chb = QtWidgets.QCheckBox()
         lock_chb.setChecked(port.locked())
         lock_chb.clicked.connect(lambda x: port.set_locked(x))
         tree.setItemWidget(item, 0, lock_chb)
 
         combo = QtWidgets.QComboBox()
         for cp in port.connected_ports():
@@ -283,15 +287,17 @@
         super(NodePropWidget, self).__init__(parent)
         self.__node_id = node.id
         self.__tab_windows = {}
         self.__tab = QtWidgets.QTabWidget()
 
         close_btn = QtWidgets.QPushButton()
         close_btn.setIcon(QtGui.QIcon(
-            self.style().standardPixmap(QtWidgets.QStyle.SP_DialogCancelButton)
+            self.style().standardPixmap(
+                QtWidgets.QStyle.SP_DialogCancelButton
+            )
         ))
         close_btn.setMaximumWidth(40)
         close_btn.setToolTip('close property')
         close_btn.clicked.connect(self._on_close)
 
         self.name_wgt = PropLineEdit()
         self.name_wgt.setToolTip('name')
@@ -369,16 +375,19 @@
         for prop_name, prop_val in model.custom_properties.items():
             tab_name = model.get_tab_name(prop_name)
             tab_mapping[tab_name].append((prop_name, prop_val))
 
         # add tabs.
         reserved_tabs = ['Node', 'Ports']
         for tab in sorted(tab_mapping.keys()):
-            if tab not in reserved_tabs:
-                self.add_tab(tab)
+            if tab in reserved_tabs:
+                print('tab name "{}" is reserved by the "NodePropWidget" '
+                      'please use a different tab name.')
+                continue
+            self.add_tab(tab)
 
         # property widget factory.
         widget_factory = NodePropertyWidgetFactory()
 
         # populate tab properties.
         for tab in sorted(tab_mapping.keys()):
             prop_window = self.__tab_windows[tab]
@@ -410,15 +419,15 @@
             prop_window.add_widget(prop_name,
                                    widget,
                                    model.get_property(prop_name),
                                    prop_name.replace('_', ' '))
 
             widget.value_changed.connect(self._on_property_changed)
 
-        self.type_wgt.setText(model.get_property('type_'))
+        self.type_wgt.setText(model.get_property('type_') or '')
 
         # add "ports" tab connections.
         if node.inputs() or node.outputs():
             ports_container = _PortConnectionsContainer(self, node=node)
             self.__tab.addTab(ports_container, 'Ports')
             return ports_container
 
@@ -527,28 +536,28 @@
         self._limit.setValue(2)
         self._limit.valueChanged.connect(self.__on_limit_changed)
         self.resize(450, 400)
 
         self._block_signal = False
 
         self._lock = False
-        self.btn_lock = QtWidgets.QPushButton('Lock')
-        self.btn_lock.setToolTip(
+        self._btn_lock = QtWidgets.QPushButton('Lock')
+        self._btn_lock.setToolTip(
             'Lock the properties bin prevent nodes from being loaded.')
-        self.btn_lock.clicked.connect(self.lock_bin)
+        self._btn_lock.clicked.connect(self.lock_bin)
 
         btn_clr = QtWidgets.QPushButton('Clear')
         btn_clr.setToolTip('Clear the properties bin.')
         btn_clr.clicked.connect(self.clear_bin)
 
         top_layout = QtWidgets.QHBoxLayout()
         top_layout.setSpacing(2)
         top_layout.addWidget(self._limit)
         top_layout.addStretch(1)
-        top_layout.addWidget(self.btn_lock)
+        top_layout.addWidget(self._btn_lock)
         top_layout.addWidget(btn_clr)
 
         layout = QtWidgets.QVBoxLayout(self)
         layout.addLayout(top_layout)
         layout.addWidget(self._prop_list, 1)
 
         # wire up node graph.
@@ -706,17 +715,17 @@
 
     def lock_bin(self):
         """
         Lock/UnLock the properties bin.
         """
         self._lock = not self._lock
         if self._lock:
-            self.btn_lock.setText('UnLock')
+            self._btn_lock.setText('UnLock')
         else:
-            self.btn_lock.setText('Lock')
+            self._btn_lock.setText('Lock')
 
     def clear_bin(self):
         """
         Clear the properties bin.
         """
         self._prop_list.setRowCount(0)
 
@@ -731,90 +740,7 @@
             NodePropWidget: node property widget.
         """
         node_id = node if isinstance(node, str) else node.id
         itm_find = self._prop_list.findItems(node_id, QtCore.Qt.MatchExactly)
         if itm_find:
             item = itm_find[0]
             return self._prop_list.cellWidget(item.row(), 0)
-
-
-# if __name__ == '__main__':
-#     from NodeGraphQt import BaseNode, NodeGraph
-#     from NodeGraphQt.constants import NodePropWidgetEnum
-#
-#
-#     class _TestNode(BaseNode):
-#
-#         __identifier__ = 'property.test'
-#         NODE_NAME = 'test node'
-#
-#         def __init__(self):
-#             super(_TestNode, self).__init__()
-#             self.create_property(
-#                 'label_test',
-#                 value='foo bar',
-#                 widget_type=NodePropWidgetEnum.QLABEL.value
-#             )
-#             self.create_property(
-#                 'text_edit',
-#                 value='text edit test',
-#                 widget_type=NodePropWidgetEnum.QLABEL.value
-#             )
-#             self.create_property(
-#                 "file",
-#                 value="",
-#                 widget_type=NodePropWidgetEnum.FILE_OPEN.value
-#             )
-#             self.create_property(
-#                 'color_picker',
-#                 value=(0, 0, 255),
-#                 widget_type=NodePropWidgetEnum.COLOR_PICKER.value
-#             )
-#             self.create_property(
-#                 'integer',
-#                 value=10,
-#                 widget_type=NodePropWidgetEnum.QSPIN_BOX.value
-#             )
-#             self.create_property(
-#                 'list',
-#                 value='itm2',
-#                 items=['itm1', 'itm2', 'itm3'],
-#                 widget_type=NodePropWidgetEnum.QCOMBO_BOX.value
-#             )
-#             self.create_property(
-#                 'range',
-#                 value=50,
-#                 range=(45, 55),
-#                 widget_type=NodePropWidgetEnum.SLIDER.value
-#             )
-#             self.create_property(
-#                 'float_range',
-#                 value=150.5,
-#                 range=(50.5, 200),
-#                 widget_type=NodePropWidgetEnum.DOUBLE_SLIDER.value
-#             )
-#             self.create_property(
-#                 'color4_picker',
-#                 value=(255, 0, 0, 122),
-#                 widget_type=NodePropWidgetEnum.COLOR4_PICKER.value
-#             )
-#
-#     def _prop_changed(node_id, prop_name, prop_value):
-#         print('-'*100)
-#         print(node_id, prop_name, prop_value)
-#
-#
-#     app = QtWidgets.QApplication([])
-#
-#     graph = NodeGraph()
-#     graph.register_node(_TestNode)
-#
-#     prop_bin = PropertiesBinWidget(node_graph=graph)
-#     prop_bin.resize(800, 600)
-#     prop_bin.property_changed.connect(_prop_changed)
-#
-#     node = graph.create_node('property.test._TestNode')
-#
-#     prop_bin.add_node(node)
-#     prop_bin.show()
-#
-#     app.exec_()
```

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py` & `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py` & `NodeGraphQt-0.6.8/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/nodes/backdrop_node.py` & `NodeGraphQt-0.6.8/NodeGraphQt/nodes/backdrop_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/nodes/base_node.py` & `NodeGraphQt-0.6.8/NodeGraphQt/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/nodes/base_node_circle.py` & `NodeGraphQt-0.6.8/NodeGraphQt/nodes/base_node_circle.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/nodes/group_node.py` & `NodeGraphQt-0.6.8/NodeGraphQt/nodes/group_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/nodes/port_node.py` & `NodeGraphQt-0.6.8/NodeGraphQt/nodes/port_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_abstract.py` & `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_abstract.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_backdrop.py` & `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_backdrop.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_base.py` & `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_base.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_circle.py` & `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_circle.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_group.py` & `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_group.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_overlay_disabled.py` & `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_overlay_disabled.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_port_in.py` & `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_port_in.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_port_out.py` & `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_port_out.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/node_text_item.py` & `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/node_text_item.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/pipe.py` & `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/pipe.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/port.py` & `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/port.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/qgraphics/slicer.py` & `NodeGraphQt-0.6.8/NodeGraphQt/qgraphics/slicer.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/widgets/actions.py` & `NodeGraphQt-0.6.8/NodeGraphQt/widgets/actions.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/widgets/dialogs.py` & `NodeGraphQt-0.6.8/NodeGraphQt/widgets/dialogs.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/widgets/icons/node_base.png` & `NodeGraphQt-0.6.8/NodeGraphQt/widgets/icons/node_base.png`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/widgets/node_graph.py` & `NodeGraphQt-0.6.8/NodeGraphQt/widgets/node_graph.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/widgets/node_widgets.py` & `NodeGraphQt-0.6.8/NodeGraphQt/widgets/node_widgets.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/widgets/scene.py` & `NodeGraphQt-0.6.8/NodeGraphQt/widgets/scene.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/widgets/tab_search.py` & `NodeGraphQt-0.6.8/NodeGraphQt/widgets/tab_search.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/widgets/viewer.py` & `NodeGraphQt-0.6.8/NodeGraphQt/widgets/viewer.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt/widgets/viewer_nav.py` & `NodeGraphQt-0.6.8/NodeGraphQt/widgets/viewer_nav.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt.egg-info/PKG-INFO` & `NodeGraphQt-0.6.8/NodeGraphQt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NodeGraphQt
-Version: 0.6.7
+Version: 0.6.8
 Summary: Node graph framework for PySide2/PyQt5 that can be
 Home-page: https://github.com/jchanvfx/NodeGraphQt
 Author: Johnny Chan
 License: MIT License
 Project-URL: Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/
 Project-URL: Tracker, https://github.com/jchanvfx/NodeGraphQt/issues
@@ -40,28 +40,28 @@
 
 
 ## Documentation
 
 <a href="https://jchanvfx.github.io/NodeGraphQt" target="_blank">https://jchanvfx.github.io/NodeGraphQt</a>
 
 See the [basic_example.py](/examples/basic_example.py) script to get started or check out the API example overview 
-<a href="https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_overview.html#simple-example" target="_blank">here.</a>
+<a href="https://jchanvfx.github.io/NodeGraphQt/api/examples/ex_overview.html#simple-example" target="_blank">here.</a>
 
 ## Vertical Layout
 
-https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_pipe.html#layout-direction
+https://jchanvfx.github.io/NodeGraphQt/api/examples/ex_pipe.html#layout-direction
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/vertical_layout.png" width="800" title="Vertical Layout">
 
 ## Pipe Layout
 
-https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_pipe.html#layout-styles
+https://jchanvfx.github.io/NodeGraphQt/api/examples/ex_pipe.html#layout-styles
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/pipe_layout_types.gif" width="600" title="Pipe Layout">
 
 ## Custom Widgets
 
-https://jchanvfx.github.io/NodeGraphQt/api/html/custom_widgets.html
+https://jchanvfx.github.io/NodeGraphQt/api/custom_widgets.html
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png" width="600" title="Properties Bin">
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/nodes_palette.png" width="450" title="Node Palette">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.7 Summary: Node graph
+Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.8 Summary: Node graph
 framework for PySide2/PyQt5 that can be Home-page: https://github.com/jchanvfx/
 NodeGraphQt Author: Johnny Chan License: MIT License Project-URL:
 Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/ Project-URL:
 Tracker, https://github.com/jchanvfx/NodeGraphQt/issues Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.6
@@ -15,17 +15,17 @@
 NodeGraphQt/main/docs/_images/screenshot.png] ## Install NodeGraphQt is
 available on The Python Package Index (PyPI) [here](https://pypi.org/project/
 NodeGraphQt) so it can be installed with: ``` pip install NodeGraphQt ``` or
 you can download previous versions from the [releases](https://github.com/
 jchanvfx/NodeGraphQt/releases) page. ## Documentation https://
 jchanvfx.github.io/NodeGraphQt See the [basic_example.py](/examples/
 basic_example.py) script to get started or check out the API example overview
-here. ## Vertical Layout https://jchanvfx.github.io/NodeGraphQt/api/html/
-examples/ex_pipe.html#layout-direction [https://raw.githubusercontent.com/
-jchanvfx/NodeGraphQt/main/docs/_images/vertical_layout.png] ## Pipe Layout
-https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_pipe.html#layout-
-styles [https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/
-_images/pipe_layout_types.gif] ## Custom Widgets https://jchanvfx.github.io/
-NodeGraphQt/api/html/custom_widgets.html [https://raw.githubusercontent.com/
+here. ## Vertical Layout https://jchanvfx.github.io/NodeGraphQt/api/examples/
+ex_pipe.html#layout-direction [https://raw.githubusercontent.com/jchanvfx/
+NodeGraphQt/main/docs/_images/vertical_layout.png] ## Pipe Layout https://
+jchanvfx.github.io/NodeGraphQt/api/examples/ex_pipe.html#layout-styles [https:/
+/raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
+pipe_layout_types.gif] ## Custom Widgets https://jchanvfx.github.io/
+NodeGraphQt/api/custom_widgets.html [https://raw.githubusercontent.com/
 jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png] [https://
 raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
 nodes_palette.png]
```

### Comparing `NodeGraphQt-0.6.7/NodeGraphQt.egg-info/SOURCES.txt` & `NodeGraphQt-0.6.8/NodeGraphQt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/PKG-INFO` & `NodeGraphQt-0.6.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NodeGraphQt
-Version: 0.6.7
+Version: 0.6.8
 Summary: Node graph framework for PySide2/PyQt5 that can be
 Home-page: https://github.com/jchanvfx/NodeGraphQt
 Author: Johnny Chan
 License: MIT License
 Project-URL: Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/
 Project-URL: Tracker, https://github.com/jchanvfx/NodeGraphQt/issues
@@ -40,28 +40,28 @@
 
 
 ## Documentation
 
 <a href="https://jchanvfx.github.io/NodeGraphQt" target="_blank">https://jchanvfx.github.io/NodeGraphQt</a>
 
 See the [basic_example.py](/examples/basic_example.py) script to get started or check out the API example overview 
-<a href="https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_overview.html#simple-example" target="_blank">here.</a>
+<a href="https://jchanvfx.github.io/NodeGraphQt/api/examples/ex_overview.html#simple-example" target="_blank">here.</a>
 
 ## Vertical Layout
 
-https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_pipe.html#layout-direction
+https://jchanvfx.github.io/NodeGraphQt/api/examples/ex_pipe.html#layout-direction
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/vertical_layout.png" width="800" title="Vertical Layout">
 
 ## Pipe Layout
 
-https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_pipe.html#layout-styles
+https://jchanvfx.github.io/NodeGraphQt/api/examples/ex_pipe.html#layout-styles
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/pipe_layout_types.gif" width="600" title="Pipe Layout">
 
 ## Custom Widgets
 
-https://jchanvfx.github.io/NodeGraphQt/api/html/custom_widgets.html
+https://jchanvfx.github.io/NodeGraphQt/api/custom_widgets.html
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png" width="600" title="Properties Bin">
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/nodes_palette.png" width="450" title="Node Palette">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.7 Summary: Node graph
+Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.8 Summary: Node graph
 framework for PySide2/PyQt5 that can be Home-page: https://github.com/jchanvfx/
 NodeGraphQt Author: Johnny Chan License: MIT License Project-URL:
 Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/ Project-URL:
 Tracker, https://github.com/jchanvfx/NodeGraphQt/issues Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.6
@@ -15,17 +15,17 @@
 NodeGraphQt/main/docs/_images/screenshot.png] ## Install NodeGraphQt is
 available on The Python Package Index (PyPI) [here](https://pypi.org/project/
 NodeGraphQt) so it can be installed with: ``` pip install NodeGraphQt ``` or
 you can download previous versions from the [releases](https://github.com/
 jchanvfx/NodeGraphQt/releases) page. ## Documentation https://
 jchanvfx.github.io/NodeGraphQt See the [basic_example.py](/examples/
 basic_example.py) script to get started or check out the API example overview
-here. ## Vertical Layout https://jchanvfx.github.io/NodeGraphQt/api/html/
-examples/ex_pipe.html#layout-direction [https://raw.githubusercontent.com/
-jchanvfx/NodeGraphQt/main/docs/_images/vertical_layout.png] ## Pipe Layout
-https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_pipe.html#layout-
-styles [https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/
-_images/pipe_layout_types.gif] ## Custom Widgets https://jchanvfx.github.io/
-NodeGraphQt/api/html/custom_widgets.html [https://raw.githubusercontent.com/
+here. ## Vertical Layout https://jchanvfx.github.io/NodeGraphQt/api/examples/
+ex_pipe.html#layout-direction [https://raw.githubusercontent.com/jchanvfx/
+NodeGraphQt/main/docs/_images/vertical_layout.png] ## Pipe Layout https://
+jchanvfx.github.io/NodeGraphQt/api/examples/ex_pipe.html#layout-styles [https:/
+/raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
+pipe_layout_types.gif] ## Custom Widgets https://jchanvfx.github.io/
+NodeGraphQt/api/custom_widgets.html [https://raw.githubusercontent.com/
 jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png] [https://
 raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
 nodes_palette.png]
```

### Comparing `NodeGraphQt-0.6.7/README.md` & `NodeGraphQt-0.6.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -22,28 +22,28 @@
 
 
 ## Documentation
 
 <a href="https://jchanvfx.github.io/NodeGraphQt" target="_blank">https://jchanvfx.github.io/NodeGraphQt</a>
 
 See the [basic_example.py](/examples/basic_example.py) script to get started or check out the API example overview 
-<a href="https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_overview.html#simple-example" target="_blank">here.</a>
+<a href="https://jchanvfx.github.io/NodeGraphQt/api/examples/ex_overview.html#simple-example" target="_blank">here.</a>
 
 ## Vertical Layout
 
-https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_pipe.html#layout-direction
+https://jchanvfx.github.io/NodeGraphQt/api/examples/ex_pipe.html#layout-direction
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/vertical_layout.png" width="800" title="Vertical Layout">
 
 ## Pipe Layout
 
-https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_pipe.html#layout-styles
+https://jchanvfx.github.io/NodeGraphQt/api/examples/ex_pipe.html#layout-styles
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/pipe_layout_types.gif" width="600" title="Pipe Layout">
 
 ## Custom Widgets
 
-https://jchanvfx.github.io/NodeGraphQt/api/html/custom_widgets.html
+https://jchanvfx.github.io/NodeGraphQt/api/custom_widgets.html
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png" width="600" title="Properties Bin">
 
 <img src="https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/nodes_palette.png" width="450" title="Node Palette">
```

#### html2text {}

```diff
@@ -6,17 +6,17 @@
 NodeGraphQt/main/docs/_images/screenshot.png] ## Install NodeGraphQt is
 available on The Python Package Index (PyPI) [here](https://pypi.org/project/
 NodeGraphQt) so it can be installed with: ``` pip install NodeGraphQt ``` or
 you can download previous versions from the [releases](https://github.com/
 jchanvfx/NodeGraphQt/releases) page. ## Documentation https://
 jchanvfx.github.io/NodeGraphQt See the [basic_example.py](/examples/
 basic_example.py) script to get started or check out the API example overview
-here. ## Vertical Layout https://jchanvfx.github.io/NodeGraphQt/api/html/
-examples/ex_pipe.html#layout-direction [https://raw.githubusercontent.com/
-jchanvfx/NodeGraphQt/main/docs/_images/vertical_layout.png] ## Pipe Layout
-https://jchanvfx.github.io/NodeGraphQt/api/html/examples/ex_pipe.html#layout-
-styles [https://raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/
-_images/pipe_layout_types.gif] ## Custom Widgets https://jchanvfx.github.io/
-NodeGraphQt/api/html/custom_widgets.html [https://raw.githubusercontent.com/
+here. ## Vertical Layout https://jchanvfx.github.io/NodeGraphQt/api/examples/
+ex_pipe.html#layout-direction [https://raw.githubusercontent.com/jchanvfx/
+NodeGraphQt/main/docs/_images/vertical_layout.png] ## Pipe Layout https://
+jchanvfx.github.io/NodeGraphQt/api/examples/ex_pipe.html#layout-styles [https:/
+/raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
+pipe_layout_types.gif] ## Custom Widgets https://jchanvfx.github.io/
+NodeGraphQt/api/custom_widgets.html [https://raw.githubusercontent.com/
 jchanvfx/NodeGraphQt/main/docs/_images/prop_bin.png] [https://
 raw.githubusercontent.com/jchanvfx/NodeGraphQt/main/docs/_images/
 nodes_palette.png]
```

### Comparing `NodeGraphQt-0.6.7/examples/hotkeys/hotkey_functions.py` & `NodeGraphQt-0.6.8/examples/hotkeys/hotkey_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -160,14 +160,21 @@
 def clear_node_selection(graph):
     """
     Clear node selection.
     """
     graph.clear_selection()
 
 
+def invert_node_selection(graph):
+    """
+    Invert node selection.
+    """
+    graph.invert_selection()
+
+
 def disable_nodes(graph):
     """
     Toggle disable on selected nodes.
     """
     graph.disable_nodes(graph.selected_nodes())
```

### Comparing `NodeGraphQt-0.6.7/examples/nodes/basic_nodes.py` & `NodeGraphQt-0.6.8/examples/nodes/basic_nodes.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/examples/nodes/custom_ports_node.py` & `NodeGraphQt-0.6.8/examples/nodes/custom_ports_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/examples/nodes/widget_nodes.py` & `NodeGraphQt-0.6.8/examples/nodes/widget_nodes.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.7/setup.cfg` & `NodeGraphQt-0.6.8/setup.cfg`

 * *Files identical despite different names*

