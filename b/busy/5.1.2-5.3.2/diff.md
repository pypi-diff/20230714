# Comparing `tmp/busy-5.1.2.tar.gz` & `tmp/busy-5.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "busy-5.1.2.tar", last modified: Wed Jun 14 07:31:55 2023, max compression
+gzip compressed data, was "busy-5.3.2.tar", last modified: Fri Jul 14 03:54:27 2023, max compression
```

## Comparing `busy-5.1.2.tar` & `busy-5.3.2.tar`

### file list

```diff
@@ -1,66 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:31:55.939469 busy-5.1.2/
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-06-14 07:31:39.000000 busy-5.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    22714 2023-06-14 07:31:55.939469 busy-5.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    22464 2023-06-14 07:31:39.000000 busy-5.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:31:55.928470 busy-5.1.2/busy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 07:31:39.000000 busy-5.1.2/busy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-14 07:31:39.000000 busy-5.1.2/busy/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:31:55.934470 busy-5.1.2/busy/command/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 07:31:39.000000 busy-5.1.2/busy/command/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1641 2023-06-14 07:31:39.000000 busy-5.1.2/busy/command/activate_command.py
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-06-14 07:31:39.000000 busy-5.1.2/busy/command/add_command.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2023-06-14 07:31:39.000000 busy-5.1.2/busy/command/base_command.py
--rw-rw-rw-   0 root         (0) root         (0)     6844 2023-06-14 07:31:39.000000 busy-5.1.2/busy/command/command.py
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-06-14 07:31:39.000000 busy-5.1.2/busy/command/curses_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1714 2023-06-14 07:31:39.000000 busy-5.1.2/busy/command/defer_command.py
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-06-14 07:31:39.000000 busy-5.1.2/busy/command/delete_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-06-14 07:31:39.000000 busy-5.1.2/busy/command/drop_and_pop_command.py
--rw-rw-rw-   0 root         (0) root         (0)      767 2023-06-14 07:31:39.000000 busy-5.1.2/busy/command/edit_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1973 2023-06-14 07:31:39.000000 busy-5.1.2/busy/command/finish_command.py
--rw-rw-rw-   0 root         (0) root         (0)      758 2023-06-14 07:31:39.000000 busy-5.1.2/busy/command/list_command.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-06-14 07:31:39.000000 busy-5.1.2/busy/command/print_command.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-06-14 07:31:39.000000 busy-5.1.2/busy/command/queues_command.py
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-06-14 07:31:39.000000 busy-5.1.2/busy/command/resource_command.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-06-14 07:31:39.000000 busy-5.1.2/busy/command/show_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1039 2023-06-14 07:31:39.000000 busy-5.1.2/busy/command/switch_command.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-06-14 07:31:39.000000 busy-5.1.2/busy/command/tags_command.py
--rw-rw-rw-   0 root         (0) root         (0)     3551 2023-06-14 07:31:39.000000 busy-5.1.2/busy/handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:31:55.935469 busy-5.1.2/busy/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 07:31:39.000000 busy-5.1.2/busy/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:31:55.936469 busy-5.1.2/busy/model/collection/
--rw-rw-rw-   0 root         (0) root         (0)     5023 2023-06-14 07:31:39.000000 busy-5.1.2/busy/model/collection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-14 07:31:39.000000 busy-5.1.2/busy/model/collection/done_collection.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-14 07:31:39.000000 busy-5.1.2/busy/model/collection/plan_collection.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-06-14 07:31:39.000000 busy-5.1.2/busy/model/collection/skip_collection.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-06-14 07:31:39.000000 busy-5.1.2/busy/model/collection/todo_collection.py
--rw-rw-rw-   0 root         (0) root         (0)     3376 2023-06-14 07:31:39.000000 busy-5.1.2/busy/model/item.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:31:55.936469 busy-5.1.2/busy/storage/
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-14 07:31:39.000000 busy-5.1.2/busy/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2196 2023-06-14 07:31:39.000000 busy-5.1.2/busy/storage/file_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:31:55.937469 busy-5.1.2/busy/ui/
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-14 07:31:39.000000 busy-5.1.2/busy/ui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6589 2023-06-14 07:31:39.000000 busy-5.1.2/busy/ui/curses_ui.py
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-06-14 07:31:39.000000 busy-5.1.2/busy/ui/shell_ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:31:55.937469 busy-5.1.2/busy/ui/tcl_ui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 07:31:39.000000 busy-5.1.2/busy/ui/tcl_ui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-06-14 07:31:39.000000 busy-5.1.2/busy/ui/tcl_ui/edit_task_widget.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-06-14 07:31:39.000000 busy-5.1.2/busy/ui/tcl_ui/get_item_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     5599 2023-06-14 07:31:39.000000 busy-5.1.2/busy/ui/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:31:55.939469 busy-5.1.2/busy/util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 07:31:39.000000 busy-5.1.2/busy/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4443 2023-06-14 07:31:39.000000 busy-5.1.2/busy/util/checklist.py
--rw-rw-rw-   0 root         (0) root         (0)     5935 2023-06-14 07:31:39.000000 busy-5.1.2/busy/util/class_family.py
--rw-rw-rw-   0 root         (0) root         (0)     2844 2023-06-14 07:31:39.000000 busy-5.1.2/busy/util/date_util.py
--rw-rw-rw-   0 root         (0) root         (0)      218 2023-06-14 07:31:39.000000 busy-5.1.2/busy/util/python_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2477 2023-06-14 07:31:39.000000 busy-5.1.2/busy/util/selector.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2023-06-14 07:31:39.000000 busy-5.1.2/busy/util/super_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 07:31:55.930470 busy-5.1.2/busy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    22714 2023-06-14 07:31:55.000000 busy-5.1.2/busy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1436 2023-06-14 07:31:55.000000 busy-5.1.2/busy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 07:31:55.000000 busy-5.1.2/busy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-14 07:31:55.000000 busy-5.1.2/busy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       99 2023-06-14 07:31:55.000000 busy-5.1.2/busy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-14 07:31:55.000000 busy-5.1.2/busy.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-06-14 07:31:39.000000 busy-5.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 07:31:55.939469 busy-5.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-06-14 07:31:39.000000 busy-5.1.2/version
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 03:54:27.026199 busy-5.3.2/
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-14 03:53:36.000000 busy-5.3.2/.version
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-07-14 03:54:18.000000 busy-5.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    22714 2023-07-14 03:54:27.026199 busy-5.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    22464 2023-07-14 03:54:18.000000 busy-5.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 03:54:27.017032 busy-5.3.2/busy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 03:54:18.000000 busy-5.3.2/busy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-14 03:54:18.000000 busy-5.3.2/busy/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 03:54:27.020699 busy-5.3.2/busy/command/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 03:54:18.000000 busy-5.3.2/busy/command/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1641 2023-07-14 03:54:18.000000 busy-5.3.2/busy/command/activate_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-07-14 03:54:18.000000 busy-5.3.2/busy/command/add_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2023-07-14 03:54:18.000000 busy-5.3.2/busy/command/base_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     6834 2023-07-14 03:54:18.000000 busy-5.3.2/busy/command/command.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-07-14 03:54:18.000000 busy-5.3.2/busy/command/curses_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1714 2023-07-14 03:54:18.000000 busy-5.3.2/busy/command/defer_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-07-14 03:54:18.000000 busy-5.3.2/busy/command/delete_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-07-14 03:54:18.000000 busy-5.3.2/busy/command/drop_and_pop_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      767 2023-07-14 03:54:18.000000 busy-5.3.2/busy/command/edit_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1973 2023-07-14 03:54:18.000000 busy-5.3.2/busy/command/finish_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      758 2023-07-14 03:54:18.000000 busy-5.3.2/busy/command/list_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-07-14 03:54:18.000000 busy-5.3.2/busy/command/print_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-07-14 03:54:18.000000 busy-5.3.2/busy/command/queues_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-07-14 03:54:18.000000 busy-5.3.2/busy/command/resource_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-14 03:54:18.000000 busy-5.3.2/busy/command/show_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2023-07-14 03:54:18.000000 busy-5.3.2/busy/command/switch_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-07-14 03:54:18.000000 busy-5.3.2/busy/command/tags_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     3555 2023-07-14 03:54:18.000000 busy-5.3.2/busy/handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 03:54:27.021615 busy-5.3.2/busy/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 03:54:18.000000 busy-5.3.2/busy/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 03:54:27.023449 busy-5.3.2/busy/model/collection/
+-rw-rw-rw-   0 root         (0) root         (0)     5020 2023-07-14 03:54:18.000000 busy-5.3.2/busy/model/collection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-14 03:54:18.000000 busy-5.3.2/busy/model/collection/done_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-14 03:54:18.000000 busy-5.3.2/busy/model/collection/plan_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-07-14 03:54:18.000000 busy-5.3.2/busy/model/collection/skip_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-07-14 03:54:18.000000 busy-5.3.2/busy/model/collection/todo_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)     3376 2023-07-14 03:54:18.000000 busy-5.3.2/busy/model/item.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 03:54:27.023449 busy-5.3.2/busy/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-07-14 03:54:18.000000 busy-5.3.2/busy/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2196 2023-07-14 03:54:18.000000 busy-5.3.2/busy/storage/file_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 03:54:27.024365 busy-5.3.2/busy/ui/
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-07-14 03:54:18.000000 busy-5.3.2/busy/ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6589 2023-07-14 03:54:18.000000 busy-5.3.2/busy/ui/curses_ui.py
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-07-14 03:54:18.000000 busy-5.3.2/busy/ui/shell_ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 03:54:27.025282 busy-5.3.2/busy/ui/tcl_ui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 03:54:18.000000 busy-5.3.2/busy/ui/tcl_ui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-07-14 03:54:18.000000 busy-5.3.2/busy/ui/tcl_ui/edit_task_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-07-14 03:54:18.000000 busy-5.3.2/busy/ui/tcl_ui/get_item_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     5588 2023-07-14 03:54:18.000000 busy-5.3.2/busy/ui/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 03:54:27.026199 busy-5.3.2/busy/util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 03:54:18.000000 busy-5.3.2/busy/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4443 2023-07-14 03:54:18.000000 busy-5.3.2/busy/util/checklist.py
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2023-07-14 03:54:18.000000 busy-5.3.2/busy/util/date_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-07-14 03:54:18.000000 busy-5.3.2/busy/util/python_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-07-14 03:54:18.000000 busy-5.3.2/busy/util/selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 03:54:27.017949 busy-5.3.2/busy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22714 2023-07-14 03:54:27.000000 busy-5.3.2/busy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1384 2023-07-14 03:54:27.000000 busy-5.3.2/busy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 03:54:27.000000 busy-5.3.2/busy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-07-14 03:54:27.000000 busy-5.3.2/busy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       99 2023-07-14 03:54:27.000000 busy-5.3.2/busy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-14 03:54:27.000000 busy-5.3.2/busy.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      627 2023-07-14 03:54:18.000000 busy-5.3.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 03:54:27.026199 busy-5.3.2/setup.cfg
```

### Comparing `busy-5.1.2/LICENSE` & `busy-5.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `busy-5.1.2/PKG-INFO` & `busy-5.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: busy
-Version: 5.1.2
+Version: 5.3.2
 Summary: Personal time management for techies
 Author-email: Francis Potter <busy@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `busy-5.1.2/README.md` & `busy-5.3.2/README.md`

 * *Files identical despite different names*

### Comparing `busy-5.1.2/busy/command/activate_command.py` & `busy-5.3.2/busy/command/activate_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.1.2/busy/command/add_command.py` & `busy-5.3.2/busy/command/add_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.1.2/busy/command/command.py` & `busy-5.3.2/busy/command/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 
 from argparse import Namespace
 from dataclasses import dataclass
 
 from busy.model.collection import Collection
 from busy.storage import Storage
 from busy.ui.ui import UI
-from busy.util.class_family import ClassFamily
-from busy.util.super_wrapper import SuperWrapper
+from wizlib.class_family import ClassFamily
+from wizlib.super_wrapper import SuperWrapper
 
 
 @dataclass
 class Command(ClassFamily, SuperWrapper):
     """
     Base class for all commands
 
@@ -193,8 +193,8 @@
         if indices:
             if with_index:
                 return '\n'.join([func(collection[i], i) for i in indices])
             else:
                 return '\n'.join([func(collection[i]) for i in indices])
         else:
             self.status = f"Queue '{self.queue}' has " + \
-                    f"no {self.collection_state} items"
+                f"no {self.collection_state} items"
```

### Comparing `busy-5.1.2/busy/command/defer_command.py` & `busy-5.3.2/busy/command/defer_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.1.2/busy/command/delete_command.py` & `busy-5.3.2/busy/command/delete_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.1.2/busy/command/drop_and_pop_command.py` & `busy-5.3.2/busy/command/drop_and_pop_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.1.2/busy/command/edit_command.py` & `busy-5.3.2/busy/command/edit_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.1.2/busy/command/finish_command.py` & `busy-5.3.2/busy/command/finish_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.1.2/busy/command/list_command.py` & `busy-5.3.2/busy/command/list_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.1.2/busy/command/print_command.py` & `busy-5.3.2/busy/command/print_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,14 @@
         collection = self.storage.get_collection(
             self.queue, self.collection_state)
         indices = collection.select(*self.criteria)
         if indices:
             items = [collection[i].base for i in indices]
         else:
             self.status = f"Queue '{self.queue}' has " + \
-                    f"no {self.collection_state} items that meet the criteria"
+                f"no {self.collection_state} items that meet the criteria"
         queue = self.queue.capitalize()
         state = self.collection_state.capitalize()
         criteria = (": "+",".join(self.criteria)) \
             if (self.criteria != self.default_criteria) else ""
         title = f"{queue} ({state}{criteria})"
         checklist.generate(title, items)
```

### Comparing `busy-5.1.2/busy/command/switch_command.py` & `busy-5.3.2/busy/command/switch_command.py`

 * *Files identical despite different names*

### Comparing `busy-5.1.2/busy/handler.py` & `busy-5.3.2/busy/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 # program. It's called when busy is run, and there are some functions to get
 # things configured and started. Then one Handler is instantiated. This is the
 # only place that imports the UI, Command, and Root classes. So the handler
 # instance is passed around, and other classes can access what they need from
 # there. Keeping the imports in one place allows the class families to be more
 # modular.
 #
-# A Handler instance provides the following properties. For the most part, these
+# A Handler instance provides the following properties. For the most part,
+# these
 # properties are how commands access other class families. Remember that the
-# Namespace from the Handler is the original Namespace, so use the one passed in
-# to the execute() method of the Command for actual usage in an interactive UI.
+# Namespace from the Handler is the original Namespace, so use the one passed
+# in to the execute() method of the Command for actual usage in an interactive
+# UI.
 
 
 import sys
 from argparse import ArgumentParser
 from pathlib import Path
 from sys import argv
 
@@ -83,15 +85,15 @@
 
     # Some useful methods so other components don't need to import from
     # different class families
 
     def get_commands(self, *attributes):
         return Command.family_members(*attributes)
 
-    # A method for commands within interactive UIs. Use our own storage but the UI
-    # is passed in. Returns None if attribute value doesn't resolve.
+    # A method for commands within interactive UIs. Use our own storage but the
+    # UI is passed in. Returns None if attribute value doesn't resolve.
 
     def get_command(self, attribute, value, **kwargs):
         member = Command.family_member(attribute, value)
         if member:
             args = {'storage': self.storage} | kwargs
             return member(**kwargs)
```

### Comparing `busy-5.1.2/busy/model/collection/__init__.py` & `busy-5.3.2/busy/model/collection/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import UserList
 from collections.abc import Iterable
 from csv import DictReader, DictWriter
 from io import IOBase
 
 from busy.model.item import Item
-from busy.util.class_family import ClassFamily
+from wizlib.class_family import ClassFamily
 from busy.util.selector import Selector
 
 
 class CollectionError(Exception):
     pass
```

### Comparing `busy-5.1.2/busy/model/item.py` & `busy-5.3.2/busy/model/item.py`

 * *Files identical despite different names*

### Comparing `busy-5.1.2/busy/storage/file_storage.py` & `busy-5.3.2/busy/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `busy-5.1.2/busy/ui/curses_ui.py` & `busy-5.3.2/busy/ui/curses_ui.py`

 * *Files identical despite different names*

### Comparing `busy-5.1.2/busy/ui/shell_ui.py` & `busy-5.3.2/busy/ui/shell_ui.py`

 * *Files identical despite different names*

### Comparing `busy-5.1.2/busy/ui/tcl_ui/edit_task_widget.py` & `busy-5.3.2/busy/ui/tcl_ui/edit_task_widget.py`

 * *Files identical despite different names*

### Comparing `busy-5.1.2/busy/ui/tcl_ui/get_item_widget.py` & `busy-5.3.2/busy/ui/tcl_ui/get_item_widget.py`

 * *Files identical despite different names*

### Comparing `busy-5.1.2/busy/ui/ui.py` & `busy-5.3.2/busy/ui/ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 from dataclasses import dataclass, field
 from enum import Enum
 from io import StringIO
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 
 from busy.model.collection import Collection
-from busy.util.class_family import ClassFamily
+from wizlib.class_family import ClassFamily
 
 
 @dataclass
 class Choice:
     """One option of several"""
 
     keys: list[str] = field(default_factory=list)
@@ -155,16 +155,16 @@
             tempfile.seek(0)
             command = [os.environ.get('EDITOR')]
             if not command[0] or not shutil.which(command[0]):
                 iterator = (c for c in commands if shutil.which(c[0]))
                 command = next(filter(None, iterator), None)
                 if not command:
                     raise RuntimeError(
-                            "A text editor at the $EDITOR " +
-                            "environment variable is required")
+                        "A text editor at the $EDITOR " +
+                        "environment variable is required")
             subprocess.run(command + [tempfile.name])
             tempfile.seek(0)
             return tempfile.read()
 
     def edit_items(self, collection: Collection, indices):
         with StringIO() as oldio:
             collection.write_items(oldio, indices)
```

### Comparing `busy-5.1.2/busy/util/checklist.py` & `busy-5.3.2/busy/util/checklist.py`

 * *Files identical despite different names*

### Comparing `busy-5.1.2/busy/util/date_util.py` & `busy-5.3.2/busy/util/date_util.py`

 * *Files identical despite different names*

### Comparing `busy-5.1.2/busy/util/selector.py` & `busy-5.3.2/busy/util/selector.py`

 * *Files identical despite different names*

### Comparing `busy-5.1.2/busy.egg-info/PKG-INFO` & `busy-5.3.2/busy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: busy
-Version: 5.1.2
+Version: 5.3.2
 Summary: Personal time management for techies
 Author-email: Francis Potter <busy@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `busy-5.1.2/busy.egg-info/SOURCES.txt` & `busy-5.3.2/busy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+.version
 LICENSE
 README.md
 pyproject.toml
-version
 busy/__init__.py
 busy/__main__.py
 busy/handler.py
 busy.egg-info/PKG-INFO
 busy.egg-info/SOURCES.txt
 busy.egg-info/dependency_links.txt
 busy.egg-info/entry_points.txt
@@ -43,12 +43,10 @@
 busy/ui/shell_ui.py
 busy/ui/ui.py
 busy/ui/tcl_ui/__init__.py
 busy/ui/tcl_ui/edit_task_widget.py
 busy/ui/tcl_ui/get_item_widget.py
 busy/util/__init__.py
 busy/util/checklist.py
-busy/util/class_family.py
 busy/util/date_util.py
 busy/util/python_version.py
-busy/util/selector.py
-busy/util/super_wrapper.py
+busy/util/selector.py
```

### Comparing `busy-5.1.2/pyproject.toml` & `busy-5.3.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 [tool.setuptools.package-dir]
 busy = "busy"
 
 [project.scripts]
 busy = "busy.handler:main"
 
 [tool.setuptools.dynamic]
-version = {file = ["version"]}
+version = {file = [".version"]}
```

