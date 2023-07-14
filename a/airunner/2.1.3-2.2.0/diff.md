# Comparing `tmp/airunner-2.1.3.tar.gz` & `tmp/airunner-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airunner-2.1.3.tar", last modified: Tue Jul 11 03:33:19 2023, max compression
+gzip compressed data, was "airunner-2.2.0.tar", last modified: Fri Jul 14 01:37:41 2023, max compression
```

## Comparing `airunner-2.1.3.tar` & `airunner-2.2.0.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:33:19.422656 airunner-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-11 03:33:09.000000 airunner-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-11 03:33:19.422656 airunner-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-11 03:33:09.000000 airunner-2.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 03:33:19.422656 airunner-2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-11 03:33:09.000000 airunner-2.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:33:19.406656 airunner-2.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:33:19.410656 airunner-2.1.3/src/airunner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/balloon.py
--rw-r--r--   0 runner    (1001) docker     (123)    21820 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/canvas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:33:19.410656 airunner-2.1.3/src/airunner/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/history.py
--rw-r--r--   0 runner    (1001) docker     (123)    27986 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:33:19.414656 airunner-2.1.3/src/airunner/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/mixins/brushes_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/mixins/canvas_active_grid_area_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/mixins/canvas_brushes_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/mixins/canvas_grid_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    23004 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/mixins/canvas_image_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/mixins/canvas_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/mixins/canvas_selectionbox_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/mixins/canvas_widgets_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/mixins/comic_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/mixins/embedding_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/mixins/extension_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    32361 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/mixins/generator_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/mixins/history_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/mixins/lora_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/mixins/menubar_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/mixins/toolbar_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:33:19.418656 airunner-2.1.3/src/airunner/pyqt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/base_window_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/embedding_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    38106 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/generate_form_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/lora_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/main_window_new_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    54139 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/main_window_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/model_merger_model_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/model_merger_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/noise_filter_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/prompt_browser_prompt_widget_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/prompt_browser_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/saturation_window_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:33:19.422656 airunner-2.1.3/src/airunner/pyqt/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/widgets/canvas_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/widgets/embedding_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/widgets/generator_tab_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/widgets/grid_preferences_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/widgets/header_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/widgets/layer_container_widget_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/widgets/layer_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/widgets/lora_container_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/widgets/lora_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    25322 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/widgets/prompt_builder_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/widgets/prompt_builder_variable_widget_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/widgets/slider_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/widgets/tool_menu_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/pyqt/widgets/toolbar_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/runai_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-07-11 03:33:09.000000 airunner-2.1.3/src/airunner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:33:19.410656 airunner-2.1.3/src/airunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-11 03:33:19.000000 airunner-2.1.3/src/airunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-11 03:33:19.000000 airunner-2.1.3/src/airunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 03:33:19.000000 airunner-2.1.3/src/airunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 03:33:19.000000 airunner-2.1.3/src/airunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 03:33:19.000000 airunner-2.1.3/src/airunner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:37:41.723592 airunner-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-14 01:37:31.000000 airunner-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-14 01:37:41.723592 airunner-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-14 01:37:31.000000 airunner-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 01:37:41.723592 airunner-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-14 01:37:31.000000 airunner-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:37:41.715592 airunner-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:37:41.715592 airunner-2.2.0/src/airunner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/balloon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/build_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22210 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/canvas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:37:41.719592 airunner-2.2.0/src/airunner/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/data/prompt_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35037 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:37:41.719592 airunner-2.2.0/src/airunner/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/mixins/brushes_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/mixins/canvas_active_grid_area_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/mixins/canvas_brushes_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/mixins/canvas_grid_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22695 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/mixins/canvas_image_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/mixins/canvas_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/mixins/canvas_selectionbox_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/mixins/canvas_widgets_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/mixins/comic_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/mixins/extension_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27566 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/mixins/generator_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/mixins/history_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/mixins/lora_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/mixins/menubar_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/mixins/toolbar_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:37:41.723592 airunner-2.2.0/src/airunner/pyqt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/base_window_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/embedding_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38106 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/generate_form_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/lora_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20905 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/main_window_new_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54139 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/main_window_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/model_merger_model_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/model_merger_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/noise_filter_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/prompt_browser_prompt_widget_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/prompt_browser_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/saturation_window_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:37:41.723592 airunner-2.2.0/src/airunner/pyqt/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/widgets/canvas_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/widgets/embedding_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/widgets/generator_tab_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/widgets/grid_preferences_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/widgets/header_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/widgets/layer_container_widget_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/widgets/layer_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/widgets/lora_container_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/widgets/lora_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24741 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/widgets/prompt_builder_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/widgets/prompt_builder_variable_widget_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/widgets/slider_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/widgets/tool_menu_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/pyqt/widgets/toolbar_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/runai_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-07-14 01:37:31.000000 airunner-2.2.0/src/airunner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:37:41.719592 airunner-2.2.0/src/airunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-14 01:37:41.000000 airunner-2.2.0/src/airunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-14 01:37:41.000000 airunner-2.2.0/src/airunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:37:41.000000 airunner-2.2.0/src/airunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 01:37:41.000000 airunner-2.2.0/src/airunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 01:37:41.000000 airunner-2.2.0/src/airunner.egg-info/top_level.txt
```

### Comparing `airunner-2.1.3/LICENSE` & `airunner-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/PKG-INFO` & `airunner-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airunner
-Version: 2.1.3
+Version: 2.2.0
 Summary: A Stable Diffusion GUI
 Home-page: https://github.com/Capsize-Games/airunner
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `airunner-2.1.3/README.md` & `airunner-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/setup.py` & `airunner-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='airunner',
-    version="2.1.3",
+    version="2.2.0",
     author="Capsize LLC",
     description="A Stable Diffusion GUI",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="ai, chatbot, chat, ai",
     license="AGPL-3.0",
     author_email="contact@capsize.gg",
     url="https://github.com/Capsize-Games/airunner",
     package_dir={"": "src"},
     packages=find_packages("src"),
     python_requires=">=3.10.0",
     install_requires=[
-        "aihandler==1.18.2",
+        "aihandler==1.19.0",
     ]
 )
```

### Comparing `airunner-2.1.3/src/airunner/balloon.py` & `airunner-2.2.0/src/airunner/balloon.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/canvas.py` & `airunner-2.2.0/src/airunner/canvas.py`

 * *Files 4% similar despite different names*

```diff
@@ -504,31 +504,41 @@
         layer_name = f"Layer {len(self.layers) + 1}"
         self.layers.insert(0, LayerData(len(self.layers), layer_name))
         self.set_current_layer(0)
 
     def get_layers_copy(self):
         return [layer for layer in self.layers]
 
-    def delete_layer(self, index):
+    def delete_layer(self):
         self.parent.history.add_event({
             "event": "delete_layer",
             "layers": self.get_layers_copy(),
             "layer_index": self.current_layer_index
         })
         if len(self.layers) == 1:
             self.layers = [LayerData(0, "Layer 1")]
         else:
             try:
-                self.layers.pop(index)
+                layer = self.layers.pop(self.current_layer_index)
+                self.container.layout().removeWidget(layer.layer_widget)
+                layer.layer_widget.deleteLater()
             except IndexError:
                 pass
         self.current_layer_index = 0
         self.show_layers()
         self.update()
 
+    def clear_layers(self):
+        # delete all widgets from self.container.layout()
+        for index, layer in enumerate(self.layers):
+            self.container.layout().removeWidget(layer.layer_widget)
+            layer.layer_widget.deleteLater()
+        self.layers = [LayerData(0, "Layer 1")]
+        self.current_layer_index = 0
+
     def layer_up(self):
         self.move_layer_up(self.current_layer)
         self.show_layers()
 
     def layer_down(self):
         self.move_layer_down(self.current_layer)
         self.show_layers()
@@ -581,20 +591,17 @@
         self.update()
         layer_obj.set_icon()
 
     def set_current_layer(self, index):
         if not hasattr(self, "container"):
             return
         if self.container:
-            try:
-                item = self.container.layout().itemAt(self.current_layer_index)
-                if item:
-                    item.widget().frame.setStyleSheet(self.parent.css("layer_normal_style"))
-            except RuntimeError:
-                item = None
+            item = self.container.layout().itemAt(self.current_layer_index)
+            if item:
+                item.widget().frame.setStyleSheet(self.parent.css("layer_normal_style"))
         self.current_layer_index = index
         if self.container:
             item = self.container.layout().itemAt(self.current_layer_index)
             if item:
                 item.widget().frame.setStyleSheet(self.parent.css("layer_highlight_style"))
         # change the layer opacity
         self.parent.tool_menu_widget.set_opacity_slider(
```

### Comparing `airunner-2.1.3/src/airunner/extensions.py` & `airunner-2.2.0/src/airunner/extensions.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/main.py` & `airunner-2.2.0/src/airunner/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,64 @@
 import os
 import pickle
+import signal
 import sys
 import traceback
 from functools import partial
 import psutil
 import torch
 from PyQt6 import uic, QtCore
-from PyQt6.QtWidgets import QApplication, QFileDialog, QSplashScreen, QMainWindow, QSplitter, QTabWidget
+from PyQt6.QtWidgets import QApplication, QFileDialog, QSplashScreen, QMainWindow, QSplitter, QTabWidget, QWidget, \
+    QVBoxLayout
 from PyQt6.QtCore import pyqtSlot, Qt, QThread, pyqtSignal, QObject, QTimer
 from PyQt6.QtGui import QGuiApplication, QPixmap, QShortcut, QKeySequence
 from aihandler.qtvar import TQDMVar, ImageVar, MessageHandlerVar, ErrorHandlerVar
 from aihandler.logger import logger
-from aihandler.settings import LOG_LEVEL
+from aihandler.settings import LOG_LEVEL, MessageCode
 from airunner.mixins.canvas_mixin import CanvasMixin
 from airunner.mixins.comic_mixin import ComicMixin
-from airunner.mixins.embedding_mixin import EmbeddingMixin
 from airunner.mixins.extension_mixin import ExtensionMixin
 from airunner.mixins.generator_mixin import GeneratorMixin
 from airunner.mixins.history_mixin import HistoryMixin
 from airunner.mixins.menubar_mixin import MenubarMixin
 from airunner.mixins.toolbar_mixin import ToolbarMixin
 from airunner.themes import Themes
 from airunner.widgets.canvas_widget import CanvasWidget
+from airunner.widgets.embedding_widget import EmbeddingWidget
 from airunner.widgets.footer_widget import FooterWidget
 from airunner.widgets.generator_tab_widget import GeneratorTabWidget
 from airunner.widgets.prompt_builder import PromptBuilderWidget
 from airunner.widgets.tool_bar_widget import ToolBarWidget
 from airunner.widgets.tool_menu_widget import ToolMenuWidget
 from airunner.widgets.header_widget import HeaderWidget
+from airunner.windows.deterministic_generation_window import DeterministicGenerationWindow
 from airunner.windows.update_window import UpdateWindow
 from airunner.utils import get_version, get_latest_version
 from aihandler.settings_manager import SettingsManager, PromptManager
 from airunner.runai_client import OfflineClient
 import qdarktheme
 from PyQt6.QtGui import QIcon
 
 
 class MainWindow(
     QMainWindow,
-    EmbeddingMixin,
     ToolbarMixin,
     HistoryMixin,
     MenubarMixin,
     CanvasMixin,
     GeneratorMixin,
     ComicMixin,
     ExtensionMixin
 ):
     current_filter = None
     tqdm_callback_triggered = False
     _document_name = "Untitled"
     is_saved = False
     action = "txt2img"
-    tqdm_var = None
     message_var = None
-    error_var = None
-    image_var = None
     progress_bar_started = False
     window = None
     history = None
     canvas = None
     settings_manager = None
     prompts_manager = None
     models = None
@@ -72,14 +71,24 @@
     add_image_to_canvas_signal = pyqtSignal(dict)
     data = None  # this is set in the generator_mixin image_handler function and used for deterministic generation
     status_error_color = "#ff0000"
     status_normal_color_light = "#000000"
     status_normal_color_dark = "#ffffff"
     is_started = False
 
+    _embedding_names = None
+    embedding_widgets = {}
+    bad_model_embedding_map = {}
+
+    @property
+    def embedding_names(self):
+        if self._embedding_names is None:
+            self._embedding_names = self.get_list_of_available_embedding_names()
+        return self._embedding_names
+
     @property
     def is_dark(self):
         return self.settings_manager.settings.dark_mode_enabled.get()
 
     @property
     def grid_size(self):
         return self.settings_manager.settings.size.get()
@@ -113,20 +122,24 @@
             "txt2img": None,
             "img2img": None,
             "outpaint": None,
             "depth2img": None,
             "pix2pix": None,
             "upscale": None,
             "superresolution": None,
-            "txt2vid": None,
+            "txt2vid": None
         },
         "kandinsky": {
             "txt2img": None,
             "img2img": None,
             "outpaint": None,
+        },
+        "shapegif": {
+            "txt2img": None,
+            "img2img": None,
         }
     }
 
     @property
     def currentTabSection(self):
         if self.override_tab_section:
             return self.override_tab_section
@@ -140,21 +153,25 @@
     def tabs(self, val):
         self._tabs[self.currentTabSection] = val
 
     @property
     def tabWidget(self):
         if self.currentTabSection == "stablediffusion":
             return self.generator_tab_widget.stableDiffusionTabWidget
-        else:
+        elif self.currentTabSection == "kandinsky":
             return self.generator_tab_widget.kandinskyTabWidget
+        elif self.currentTabSection == "shapegif":
+            return self.generator_tab_widget.shapegifTabWidget
+        else:
+            raise Exception("Invalid tab section")
 
     @property
     def generator_type(self):
         """
-        Returns either stablediffusion or kandinsky
+        Returns either stablediffusion, shapegif, kandinsky
         :return: string
         """
         return self._generator_type
 
     @property
     def current_index(self):
         return self.tabWidget.currentIndex()
@@ -200,28 +217,14 @@
         self._latest_version = val
 
     @property
     def document_name(self):
         name = f"{self._document_name}{'*' if self.canvas and self.canvas.is_dirty else ''}"
         return f"{name} - {self.version}"
 
-    @pyqtSlot(int, int, str, object, object)
-    def tqdm_callback(self, step, total, action, image=None, data=None):
-        if step == 0 and total == 0:
-            current = 0
-        else:
-            if self.progress_bar_started and not self.tqdm_callback_triggered:
-                self.tqdm_callback_triggered = True
-                self.generator_tab_widget.data[action]["progressBar"].setRange(0, 100)
-            try:
-                current = (step / total)
-            except ZeroDivisionError:
-                current = 0
-        self.generator_tab_widget.set_progress_bar_value(action, int(current * 100))
-
     @property
     def is_windows(self):
         return sys.platform.startswith("win") or sys.platform.startswith("cygwin") or sys.platform.startswith("msys")
 
     @property
     def is_maximized(self):
         return self.settings_manager.settings.is_maximized.get()
@@ -386,15 +389,14 @@
         self.toolbar_widget.set_stylesheet()
         self.footer_widget.set_stylesheet()
 
     def initialize(self):
         self.initialize_settings_manager()
         self.instantiate_widgets()
         self.initialize_saved_prompts()
-        self.initialize_tqdm()
         self.initialize_handlers()
         self.initialize_window()
         self.initialize_widgets()
         self.initialize_mixins()
         self.header_widget.initialize()
         self.header_widget.set_size_increment_levels()
         self.initialize_shortcuts()
@@ -409,15 +411,14 @@
 
     def initialize_mixins(self):
         HistoryMixin.initialize(self)
         CanvasMixin.initialize(self)
         GeneratorMixin.initialize(self)
         MenubarMixin.initialize(self)
         ToolbarMixin.initialize(self)
-        EmbeddingMixin.initialize(self)
 
     # a list of tuples that represents a signal name and its handler
     registered_settings_handlers = []
 
     def register_setting_handler(self, signal, handler):
         """
         Connect a signal to a handler. Signals must be part of settings_manager.settings
@@ -431,14 +432,21 @@
     def connect_signals(self):
         logger.info("Connecting signals...")
         self.canvas._is_dirty.connect(self.set_window_title)
 
         for signal, handler in self.registered_settings_handlers:
             getattr(self.settings_manager.settings, signal).connect(handler)
 
+        self.model_var.connect(self.enable_embeddings)
+        self.settings_manager.settings.embeddings_path.my_signal.connect(self.update_embedding_names)
+        self.seed_var.my_signal.connect(self.prompt_builder.process_prompt)
+        self.settings_manager.settings.use_prompt_builder_checkbox.my_signal.connect(
+            self.generator_tab_widget.toggle_all_prompt_builder_checkboxes
+        )
+
     def instantiate_widgets(self):
         logger.info("Instantiating widgets...")
         self.generator_tab_widget = GeneratorTabWidget(app=self)
         self.header_widget = HeaderWidget(app=self)
         self.canvas_widget = CanvasWidget(app=self)
         self.tool_menu_widget = ToolMenuWidget(app=self)
         self.toolbar_widget = ToolBarWidget(app=self)
@@ -447,19 +455,21 @@
     def initialize_widgets(self):
         logger.info("Initializing widgets...")
         self.gridLayout.setColumnStretch(1, 1)
         self.gridLayout.addWidget(self.header_widget, 0, 0, 1, 4)
 
         self.splitter = QSplitter()
         self.center_splitter = QSplitter(Qt.Orientation.Vertical)
-        prompt_builder = PromptBuilderWidget(app=self)
+        self.prompt_builder = PromptBuilderWidget(app=self)
         center_panel = QTabWidget()
         center_panel.setStyleSheet(self.css("center_panel"))
         center_panel.setTabPosition(QTabWidget.TabPosition.South)
-        center_panel.addTab(prompt_builder, "Prompt Builder")
+        center_panel.addTab(self.prompt_builder, "Prompt Builder")
+        # auto hide tabs
+        center_panel.tabBar().hide()
         self.center_splitter.setStretchFactor(1, 1)
         self.center_splitter.setStretchFactor(2, 0)
         self.splitter.addWidget(self.generator_tab_widget)
         self.center_splitter.addWidget(self.canvas_widget)
         self.center_splitter.addWidget(center_panel)
         # listen to center_splitter size changes
         self.center_splitter.splitterMoved.connect(self.handle_bottom_splitter_moved)
@@ -503,56 +513,43 @@
 
     def handle_bottom_splitter_moved(self, pos, index):
         top_height = self.center_splitter.widget(0).height()
         bottom_height = self.center_splitter.widget(1).height()
         self.settings_manager.settings.bottom_splitter_sizes.set([top_height, bottom_height])
 
     def initialize_saved_prompts(self):
-        print("INITIALZING PROMPTS")
         self.prompts_manager = PromptManager()
-        print(self.prompts_manager.settings.prompts)
         self.prompts_manager.enable_save()
 
     def initialize_settings_manager(self):
         self.settings_manager = SettingsManager()
         self.settings_manager.disable_save()
         # self.get_extensions_from_path()  TODO: Extensions
         self.settings_manager.settings.size.my_signal.connect(self.set_size_form_element_step_values)
         self.settings_manager.settings.line_width.my_signal.connect(self.set_size_form_element_step_values)
 
     def initialize_shortcuts(self):
         # on shift + mouse scroll change working width
         self.wheelEvent = self.change_width
 
-    def initialize_tqdm(self):
-        self.tqdm_var = TQDMVar()
-        self.tqdm_var.my_signal.connect(self.tqdm_callback)
-
     def initialize_handlers(self):
         self.message_var = MessageHandlerVar()
         self.message_var.my_signal.connect(self.message_handler)
-        self.error_var = ErrorHandlerVar()
-        self.error_var.my_signal.connect(self.error_handler)
-        self.image_var = ImageVar()
-        self.image_var.my_signal.connect(self.image_handler)
 
     def initialize_window(self):
         HERE = os.path.dirname(os.path.abspath(__file__))
         self.window = uic.loadUi(os.path.join(HERE, "pyqt/main_window_new.ui"), self)
         self.center()
         self.set_window_title()
         self.set_window_icon()
 
     def initialize_stable_diffusion(self):
         logger.info("Initializing stable diffusion...")
         self.client = OfflineClient(
             app=self,
-            tqdm_var=self.tqdm_var,
-            image_var=self.image_var,
-            error_var=self.error_var,
             message_var=self.message_var,
             settings_manager=self.settings_manager,
         )
 
     def save_settings(self):
         self.settings_manager.save_settings()
 
@@ -616,42 +613,117 @@
         """
         self.setWindowTitle(f"AI Runner {self.document_name}")
 
     def set_window_icon(self):
         self.setWindowIcon(QIcon("src/icon_256.png"))
 
     def new_document(self):
-        CanvasMixin.initialize(self)
+        self.canvas.clear_layers()
+        self.clear_history()
+        #CanvasMixin.initialize(self)
         self.is_saved = False
         self.canvas.is_dirty = False
         self._document_name = "Untitled"
         self.set_window_title()
-        # clear the layers list widget
-        #self.tool_menu_widget.layers.setWidget(None)
         self.current_filter = None
         self.canvas.update()
         self.canvas.show_layers()
 
     def set_status_label(self, txt, error=False):
         color = self.status_normal_color_dark if self.is_dark else \
             self.status_normal_color_light
         self.footer_widget.status_label.setText(txt)
         self.footer_widget.status_label.setStyleSheet(
             f"color: {self.status_error_color if error else color};"
         )
 
-    def message_handler(self, msg):
-        if isinstance(msg, dict):
-            msg = msg["response"]
-        self.set_status_label(msg)
-
-    def error_handler(self, msg):
-        if isinstance(msg, dict):
-            msg = msg["response"]
-        self.set_status_label(msg, error=True)
+    @pyqtSlot(dict)
+    def message_handler(self, response: dict):
+        try:
+            code = response["code"]
+        except TypeError:
+            # logger.error(f"Invalid response message: {response}")
+            # traceback.print_exc()
+            return
+        message = response["message"]
+        {
+            MessageCode.STATUS: self.handle_status,
+            MessageCode.ERROR: self.handle_error,
+            MessageCode.PROGRESS: self.handle_progress,
+            MessageCode.IMAGE_GENERATED: self.handle_image_generated,
+            MessageCode.EMBEDDING_LOAD_FAILED: self.handle_embedding_load_failed,
+        }.get(code, self.handle_unknown)(message)
+
+    def handle_image_generated(self, message):
+        images = message["images"]
+        data = message["data"]
+        nsfw_content_detected = message["nsfw_content_detected"]
+        self.clear_status_message()
+        self.data = data
+        if data["action"] == "txt2vid":
+            return self.video_handler(data)
+
+        self.generator_tab_widget.stop_progress_bar(
+            data["tab_section"], data["action"]
+        )
+
+        if self.settings_manager.settings.auto_export_images.get():
+            self.auto_export_image(images[0], data)
+
+        self.generator_tab_widget.stop_progress_bar(
+            data["tab_section"], data["action"]
+        )
+        if nsfw_content_detected and self.settings_manager.settings.nsfw_filter.get():
+            self.message_handler("NSFW content detected, try again.", error=True)
+        elif data["options"][f"deterministic_generation"]:
+            self.deterministic_images = images
+            DeterministicGenerationWindow(
+                self.settings_manager,
+                app=self,
+                images=self.deterministic_images,
+                data=data)
+        else:
+            if data[
+                "action"] != "outpaint" and self.image_to_new_layer and self.canvas.current_layer.image_data.image is not None:
+                self.canvas.add_layer()
+            # print width and height of image
+            self.canvas.image_handler(images[0], data)
+            self.message_handler("")
+            self.canvas.show_layers()
+
+    def handle_status(self, message):
+        self.set_status_label(message)
+
+    def handle_error(self, message):
+        self.set_status_label(message, error=True)
+
+    def handle_progress(self, message):
+        step = message.get("step")
+        total = message.get("total")
+        action = message.get("action")
+        tab_section = message.get("tab_section")
+
+        if step == 0 and total == 0:
+            current = 0
+        else:
+            try:
+                current = (step / total)
+            except ZeroDivisionError:
+                current = 0
+        self.generator_tab_widget.set_progress_bar_value(tab_section, action, int(current * 100))
+
+    def handle_embedding_load_failed(self, message):
+        # TODO:
+        #  on model change, re-enable the buttons
+        embedding_name = message["embedding_name"]
+        model_name = message["model_name"]
+        self.disable_embedding(embedding_name, model_name)
+
+    def handle_unknown(self, message):
+        logger.error(f"Unknown message code: {message}")
 
     def clear_status_message(self):
         self.set_status_label("")
 
     def set_size_form_element_step_values(self):
         """
         This function is called when grid_size is changed in the settings.
@@ -672,32 +744,44 @@
         if not file_path.endswith(".airunner"):
             file_path += ".airunner"
 
         self.do_save(file_path)
 
     def do_save(self, document_name):
         # save self.canvas.layers as pickle
+        layers = []
+        # we need to save self.canvas.layers but it contains a QWdget
+        # so we will remove the QWidget from each layer, add the layer to a new
+        # list and then restore the QWidget
+        layer_widgets = []
+        for layer in self.canvas.layers:
+            layer_widgets.append(layer.layer_widget)
+            layer.layer_widget = None
+            layers.append(layer)
         data = {
-            "layers": self.canvas.layers,
+            "layers": layers,
             "image_pivot_point": self.canvas.image_pivot_point,
             "image_root_point": self.canvas.image_root_point,
         }
         with open(document_name, "wb") as f:
             pickle.dump(data, f)
+        # restore the QWidget
+        for i, layer in enumerate(layers):
+            layer.layer_widget = layer_widgets[i]
         # get the document name stripping .airunner from the end
+        self._document_path = document_name
         self._document_name = document_name.split("/")[-1].split(".")[0]
         self.set_window_title()
         self.is_saved = True
         self.canvas.is_dirty = False
 
     def save_document(self):
         if not self.is_saved:
             return self.saveas_document()
-        document_name = f"{self._document_name}.airunner"
-        self.do_save(document_name)
+        self.do_save(self._document_path)
 
     def load_document(self):
         self.new_document()
         # load all settings and layer data from a file called "<document_name>.airunner"
 
         # get file path
         file_path, _ = QFileDialog.getOpenFileName(
@@ -715,14 +799,15 @@
                 layers = data["layers"]
                 image_pivot_point = data["image_pivot_point"]
                 image_root_point = data["image_root_point"]
             except Exception as e:
                 layers = data
 
         # get the document name stripping .airunner from the end
+        self._document_path = file_path
         self._document_name = file_path.split("/")[-1].split(".")[0]
 
         # load document data
         self.canvas.layers = layers
         self.canvas.image_pivot_point = image_pivot_point
         self.canvas.image_root_point = image_root_point
         self.canvas.update()
@@ -732,16 +817,98 @@
 
     def update_system_stats(self):
         system_memory_percentage = psutil.virtual_memory().percent
         cuda_memory = f"VRAM allocated {torch.cuda.memory_allocated() / 1024 ** 3:.1f}GB cached {torch.cuda.memory_cached() / 1024 ** 3:.1f}GB"
         system_memory = f"RAM {system_memory_percentage:.1f}%"
         self.footer_widget.system_status.setText(f"{system_memory}, {cuda_memory}")
 
+    def update_embedding_names(self, _):
+        self._embedding_names = None
+        for tab_name in self.tabs.keys():
+            tab = self.tabs[tab_name]
+            # clear embeddings
+            try:
+                tab.embeddings.widget().deleteLater()
+            except AttributeError:
+                pass
+            self.load_embeddings(tab)
+
+    def register_embedding_widget(self, name, widget):
+        self.embedding_widgets[name] = widget
+
+    def disable_embedding(self, name, model_name):
+        self.embedding_widgets[name].setEnabled(False)
+        if name not in self.bad_model_embedding_map:
+            self.bad_model_embedding_map[name] = []
+        if model_name not in self.bad_model_embedding_map[name]:
+            self.bad_model_embedding_map[name].append(model_name)
+
+    def enable_embeddings(self):
+        for name in self.embedding_widgets.keys():
+            enable = True
+            if name in self.bad_model_embedding_map:
+                if self.model in self.bad_model_embedding_map[name]:
+                    enable = False
+            self.embedding_widgets[name].setEnabled(enable)
+
+    def load_embeddings(self, tab):
+        container = QWidget()
+        container.setLayout(QVBoxLayout())
+        for embedding_name in self.embedding_names:
+            embedding_widget = EmbeddingWidget(
+                app=self,
+                name=embedding_name
+            )
+            self.register_embedding_widget(embedding_name, embedding_widget)
+            container.layout().addWidget(embedding_widget)
+        container.layout().addStretch()
+        self.tool_menu_widget.embeddings_container_widget.embeddings.setWidget(container)
+
+    def get_list_of_available_embedding_names(self):
+        embeddings_path = self.settings_manager.settings.embeddings_path.get() or "embeddings"
+        if embeddings_path == "embeddings":
+            embeddings_path = os.path.join(self.settings_manager.settings.model_base_path.get(), embeddings_path)
+        return self.find_embeddings_in_path(embeddings_path)
+
+    def find_embeddings_in_path(self, embeddings_path, tokens=None):
+        if tokens is None:
+            tokens = []
+        if not os.path.exists(embeddings_path):
+            return tokens
+        if os.path.exists(embeddings_path):
+            for f in os.listdir(embeddings_path):
+                # check if f is directory
+                if os.path.isdir(os.path.join(embeddings_path, f)):
+                    return self.find_embeddings_in_path(os.path.join(embeddings_path, f), tokens)
+                words = f.split(".")
+                if words[-1] in ["pt", "ckpt", "pth", "safetensors"]:
+                    words = words[:-1]
+                words = ".".join(words).lower()
+                tokens.append(words)
+        return tokens
+
+    def insert_into_prompt(self, text, negative_prompt=False):
+        prompt_widget = self.generator_tab_widget.data[self.currentTabSection][self.current_section]["prompt_widget"]
+        negative_prompt_widget = self.generator_tab_widget.data[self.currentTabSection][self.current_section]["negative_prompt_widget"]
+        if negative_prompt:
+            current_text = negative_prompt_widget.toPlainText()
+            text = f"{current_text}, {text}" if current_text != "" else text
+            negative_prompt_widget.setPlainText(text)
+        else:
+            current_text = prompt_widget.toPlainText()
+            text = f"{current_text}, {text}" if current_text != "" else text
+            prompt_widget.setPlainText(text)
+
 
 if __name__ == "__main__":
+    def signal_handler(signal, frame):
+        print("\nExiting...")
+        sys.exit(0)
+
+    signal.signal(signal.SIGINT, signal_handler)
     QApplication.setAttribute(Qt.ApplicationAttribute.AA_UseDesktopOpenGL)
     app = QApplication([])
 
     def display_splash_screen(app):
         screens = QGuiApplication.screens()
         try:
             screen = screens.at(0)
```

### Comparing `airunner-2.1.3/src/airunner/mixins/brushes_mixin.py` & `airunner-2.2.0/src/airunner/mixins/brushes_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/mixins/canvas_active_grid_area_mixin.py` & `airunner-2.2.0/src/airunner/mixins/canvas_active_grid_area_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
             brush_color = QColor(0, 255, 255)
         elif self.parent.current_section == "upscale":
             brush_color = QColor(255, 0, 155)
         elif self.parent.current_section == "superresolution":
             brush_color = QColor(255, 0, 255)
         elif self.parent.current_section == "controlnet":
             brush_color = QColor(255, 255, 255)
+        elif self.parent.current_section == "txt2vid":
+            brush_color = QColor(144, 144, 144)
         else:
             brush_color = QColor(0, 0, 0)
         return brush_color
 
     @property
     def active_grid_area_rect(self):
         width = self.settings_manager.settings.working_width.get()
```

### Comparing `airunner-2.1.3/src/airunner/mixins/canvas_brushes_mixin.py` & `airunner-2.2.0/src/airunner/mixins/canvas_brushes_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/mixins/canvas_grid_mixin.py` & `airunner-2.2.0/src/airunner/mixins/canvas_grid_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/mixins/canvas_image_mixin.py` & `airunner-2.2.0/src/airunner/mixins/canvas_image_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,32 +226,22 @@
             filtered_image = filtered_image.filter(GaussianBlur(radius=0.03 * 20))
             self.current_layer.image_data.image = filtered_image
             self.image_data = None
         self.update()
 
     def load_image(self, image_path):
         image = Image.open(image_path)
-        self.load_metadata(image)
 
         # if settings_manager.settings.resize_on_paste, resize the image to working width and height while mainting its aspect ratio
         if self.settings_manager.settings.resize_on_paste.get():
             image.thumbnail((self.settings_manager.settings.working_width.get(), self.settings_manager.settings.working_height.get()), Image.ANTIALIAS)
 
         self.create_image(QPoint(0, 0), image)
         self.update()
 
-    def load_metadata(self, image):
-        if not self.settings_manager.settings.import_metadata.get():
-            return
-        try:
-            metadata = image.text
-        except AttributeError:
-            metadata = None
-        self.parent.load_metadata(metadata)
-
     def save_image(self, image_path, image=None):
         if self.current_layer.image_data.image is None:
             return
         if image is None:
             image = self.current_layer.image_data.image
         image = image.convert("RGBA")
         if not "." in image_path:
```

### Comparing `airunner-2.1.3/src/airunner/mixins/canvas_selectionbox_mixin.py` & `airunner-2.2.0/src/airunner/mixins/canvas_selectionbox_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/mixins/comic_mixin.py` & `airunner-2.2.0/src/airunner/mixins/comic_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/mixins/embedding_mixin.py` & `airunner-2.2.0/src/airunner/mixins/extension_mixin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,88 @@
+import importlib
 import os
-from functools import partial
+from aihandler.util import get_extensions_from_path
 
-import torch
-from PyQt6 import uic
-from PyQt6.QtWidgets import QLabel, QWidget, QVBoxLayout
 
-from airunner.widgets.embedding_widget import EmbeddingWidget
-
-
-class EmbeddingMixin:
-    _embedding_names = None
-
-    @property
-    def embedding_names(self):
-        if self._embedding_names is None:
-            self._embedding_names = self.get_list_of_available_embedding_names()
-        return self._embedding_names
+class ExtensionMixin:
+    """
+    This is a mixin class that is used to manage extensions.
+    """
+    active_extensions = []
 
     def initialize(self):
-        # listen to self.settings_manager.settings.embeddings_path and update self.embedding_names on change
-        self.settings_manager.settings.embeddings_path.my_signal.connect(self.update_embedding_names)
-
         for tab_name in self.tabs.keys():
-            tab = self.tabs[tab_name]
-            self.load_embeddings(tab)
+            self.do_generator_tab_injection(self.tabs[tab_name], tab_name)
+        self.do_menubar_injection()
+        self.do_toolbar_injection()
+
+    def get_extensions_from_path(self):
+        """
+        Initialize extensions by loading them from the extensions_directory.
+        These are extensions that have been activated by the user.
+        Extensions can be activated by manually adding them to the extensions folder
+        or by browsing for them in the extensions menu and activating them there.
+
+        This method initializes active extensions.
+        :return:
+        """
+        extensions = []
+        base_path = self.settings_manager.settings.model_base_path.get()
+        extensions_path = self.settings_manager.settings.extensions_path.get() or "extensions"
+        if extensions_path == "extensions":
+            extensions_path = os.path.join(base_path, extensions_path)
+        if not os.path.exists(extensions_path):
+            return extensions
+        available_extensions = get_extensions_from_path(extensions_path)
+        for extension in available_extensions:
+            if extension.name.get() in self.settings_manager.settings.enabled_extensions.get():
+                repo = extension.repo.get()
+                name = repo.split("/")[-1]
+                path = os.path.join(extensions_path, name)
+                if os.path.exists(path):
+                    for f in os.listdir(path):
+                        if os.path.isfile(os.path.join(path, f)) and f == "main.py":
+                            # get Extension class from main.py
+                            spec = importlib.util.spec_from_file_location("main", os.path.join(path, f))
+                            module = importlib.util.module_from_spec(spec)
+                            spec.loader.exec_module(module)
+                            ExtensionClass = getattr(module, "Extension")
+                            try:
+                                extensions.append(ExtensionClass(self, self.settings_manager))
+                            except TypeError:
+                                pass
+        self.settings_manager.settings.active_extensions.set(extensions)
+
+    def do_generator_tab_injection(self, tab, tab_name):
+        """
+        Ibjects extensions into the generator tab widget.
+        :param tab_name:
+        :param tab:
+        :return:
+        """
+        for extension in self.settings_manager.settings.active_extensions.get():
+            try:
+                extension.generator_tab_injection(tab, tab_name)
+            except AttributeError:
+                pass
 
-    def update_embedding_names(self, _):
-        self._embedding_names = None
-        for tab_name in self.tabs.keys():
-            tab = self.tabs[tab_name]
-            # clear embeddings
+    def do_menubar_injection(self):
+        for extension in self.settings_manager.settings.active_extensions.get():
+            try:
+                extension.menubar_injection(self.menubar)
+            except AttributeError:
+                pass
+
+    def do_toolbar_injection(self):
+        for extension in self.settings_manager.settings.active_extensions.get():
+            try:
+                extension.toolbar_injection(self.horizontalFrame)
+            except AttributeError:
+                pass
+
+    def do_preferences_injection(self, window):
+        for extension in self.settings_manager.settings.active_extensions.get():
             try:
-                tab.embeddings.widget().deleteLater()
+                extension.preferences_injection(window)
             except AttributeError:
                 pass
-            self.load_embeddings(tab)
 
-    def load_embeddings(self, tab):
-        container = QWidget()
-        container.setLayout(QVBoxLayout())
-        for embedding_name in self.embedding_names:
-            embedding_widget = EmbeddingWidget(
-                app=self,
-                name=embedding_name
-            )
-            container.layout().addWidget(embedding_widget)
-        container.layout().addStretch()
-        self.tool_menu_widget.embeddings_container_widget.embeddings.setWidget(container)
-
-    def get_list_of_available_embedding_names(self):
-        embeddings_path = self.settings_manager.settings.embeddings_path.get() or "embeddings"
-        if embeddings_path == "embeddings":
-            embeddings_path = os.path.join(self.settings_manager.settings.model_base_path.get(), embeddings_path)
-        return self.find_embeddings_in_path(embeddings_path)
-
-    def find_embeddings_in_path(self, embeddings_path, tokens=None):
-        if tokens is None:
-            tokens = []
-        if not os.path.exists(embeddings_path):
-            return tokens
-        if os.path.exists(embeddings_path):
-            for f in os.listdir(embeddings_path):
-                # check if f is directory
-                if os.path.isdir(os.path.join(embeddings_path, f)):
-                    return self.find_embeddings_in_path(os.path.join(embeddings_path, f), tokens)
-                words = f.split(".")
-                # if the last word is pt, ckpt, or pth, then join all words except the last one
-                if words[-1] in ["pt", "ckpt", "pth", "safetensors"]:
-                    words = words[:-1]
-                words = ".".join(words).lower()
-                tokens.append(words)
-        return tokens
-
-    def insert_into_prompt(self, text, negative_prompt=False):
-        tab = self.tabWidget.currentWidget()
-        if negative_prompt:
-            current_text = tab.negative_prompt.toPlainText()
-            text = f"{current_text}, {text}" if current_text != "" else text
-            tab.negative_prompt.setPlainText(text)
-        else:
-            current_text = tab.prompt.toPlainText()
-            text = f"{current_text}, {text}" if current_text != "" else text
-            tab.prompt.setPlainText(text)
```

### Comparing `airunner-2.1.3/src/airunner/mixins/generator_mixin.py` & `airunner-2.2.0/src/airunner/mixins/generator_mixin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import random
 from PIL import Image
 from PyQt6 import uic
 from PyQt6.QtCore import QRect, pyqtSignal, Qt
 from PyQt6.QtGui import QShortcut, QKeySequence
 from PyQt6.uic.exceptions import UIFileException
-from aihandler.settings import MAX_SEED, AVAILABLE_SCHEDULERS_BY_ACTION, MODELS
-from airunner.windows.deterministic_generation_window import DeterministicGenerationWindow
+from aihandler.settings import MAX_SEED, MODELS, MessageCode
 from airunner.windows.video import VideoPopup
 from airunner.mixins.lora_mixin import LoraMixin
 from PIL import PngImagePlugin
 
 
 class GeneratorMixin(LoraMixin):
     generate_signal = pyqtSignal(dict)
@@ -139,14 +138,26 @@
         return self.strength_var.get()
 
     @strength.setter
     def strength(self, val):
         self.strength_var.set(val)
 
     @property
+    def zeroshot_var(self):
+        return self.settings.zeroshot
+
+    @property
+    def zeroshot(self):
+        return self.zeroshot_var.get()
+
+    @zeroshot.setter
+    def zeroshot(self, val):
+        self.zeroshot_var.set(val)
+
+    @property
     def enable_controlnet_var(self):
         return self.settings.enable_controlnet
 
     @property
     def enable_controlnet(self):
         return self.enable_controlnet_var.get()
 
@@ -171,19 +182,20 @@
 
     @property
     def use_prompt_builder_checkbox_var(self):
         return self.settings.use_prompt_builder_checkbox
 
     @property
     def use_prompt_builder_checkbox(self):
-        return self.use_prompt_builder_checkbox_var.get()
+        val = self.use_prompt_builder_checkbox_var.get()
+        return val == 2 or val == True
 
     @use_prompt_builder_checkbox.setter
     def use_prompt_builder_checkbox(self, val):
-        self.use_prompt_builder_checkbox_var.set(val)
+        self.use_prompt_builder_checkbox_var.set(val == True or val == 2)
 
     @property
     def controlnet_scale_var(self):
         return self.settings.controlnet_guidance_scale
 
     @property
     def controlnet_guidance_scale(self):
@@ -310,44 +322,22 @@
     def update_controlnet(self, tab, index):
         controlnet = self.tabs[tab].controlnet_dropdown.itemText(index)
         controlnet = controlnet.lower()
         if controlnet == "":
             controlnet = None
         self.settings.controlnet_var.set(controlnet)
 
-    def handle_controlnet_checkbox_change(self, tab, val):
-        self.enable_controlnet = val == 2
-        self.toggle_controlnet_elements(tab)
-
-    def toggle_controlnet_elements(self, tab):
-        tab.controlnet_dropdown.setEnabled(self.enable_controlnet)
-        tab.controlnet_guidance_scale_slider.setEnabled(self.enable_controlnet)
-        tab.controlnet_guidance_scale_spinbox.setEnabled(self.enable_controlnet)
-
-    def handle_deterministic_radio_change(self, val, tab):
-        self.deterministic = tab.deterministic_radio.isChecked()
-
-    def handle_downscale_spinbox_change(self, value, tab):
-        current_value = self.downscale_amount
-        new_value = value
-        if value == 1:
-            if value > current_value or value == current_value:
-                new_value = 2
-            else:
-                new_value = 0
-        self.downscale_amount = value
-        tab.downscale_spinbox.setValue(new_value)
-        self.set_final_size_label(tab)
-
     def set_final_size_label(self, tab=None):
         if tab is None:
             tab = self.tabs[self.current_section]
 
-        if self.current_section not in ["upscale", "superresolution"]:
-            return
+        """
+        Early return to hack aronud final size for now
+        """
+        return
 
         image = self.canvas.current_layer.image_data.image
         if image:
             if self.do_upscale_by_active_grid:
                 width = self.settings_manager.settings.working_width.get()
                 height = self.settings_manager.settings.working_height.get()
             else:
@@ -388,15 +378,14 @@
     def reset_settings(self):
         self.settings_manager.reset_settings_to_default()
         for tab_name in self.tabs.keys():
             tab = self.tabs[tab_name]
             self.set_default_values(tab_name, tab)
         self.canvas.update()
 
-
     def text_changed(self, tab):
         try:
             val = int(tab.seed.toPlainText())
             self.seed = val
         except ValueError:
             pass
 
@@ -407,102 +396,14 @@
             self.random_seed = False
         _tab.seed.setEnabled(not self.random_seed)
 
     def video_handler(self, data):
         filename = data["video_filename"]
         VideoPopup(settings_manager=self.settings_manager, file_path=filename)
 
-    def image_handler(self, images, data, nsfw_content_detected):
-        self.clear_status_message()
-        self.data = data
-        if data["action"] == "txt2vid":
-            return self.video_handler(data)
-
-        if self.settings_manager.settings.auto_export_images.get():
-            self.auto_export_image(images[0], data)
-
-        self.generator_tab_widget.stop_progress_bar(
-            data["action"])
-        if nsfw_content_detected and self.settings_manager.settings.nsfw_filter.get():
-            self.message_handler("NSFW content detected, try again.", error=True)
-        elif data["options"][f"deterministic_generation"]:
-            self.deterministic_images = images
-            DeterministicGenerationWindow(self.settings_manager, app=self, images=self.deterministic_images, data=data)
-        else:
-            if data["action"] != "outpaint" and self.image_to_new_layer and self.canvas.current_layer.image_data.image is not None:
-                self.canvas.add_layer()
-            # print width and height of image
-            self.canvas.image_handler(images[0], data)
-            self.message_handler("")
-            self.canvas.show_layers()
-
-    def load_metadata(self, metadata):
-        """
-        Early return to patch import of image until a real fix is implemented
-        :param metadata:
-        :return:
-        """
-        """
-        if metadata:
-            action = metadata.get("action")
-            prompt = None
-            negative_prompt = None
-            if "prompt" in metadata:
-                prompt = metadata.get("prompt", "")
-            if "negative_prompt" in metadata:
-                negative_prompt = metadata.get("negative_prompt", "")
-            scale = metadata.get("scale", None)
-            seed = metadata.get("seed", None)
-            steps = metadata.get("steps", None)
-            ddim_eta = metadata.get("ddim_eta", None)
-            n_iter = metadata.get("n_iter", None)
-            n_samples = metadata.get("n_samples", None)
-            model = metadata.get("model", None)
-            # model_branch = metadata.get("model_branch", None)
-            scheduler = metadata.get("scheduler", None)
-            if prompt is not None:
-                self.tabs[action].prompt.setPlainText(prompt)
-            if negative_prompt is not None:
-                self.tabs[action].negative_prompt.setPlainText(negative_prompt)
-            if scale:
-                scale = float(scale)
-                self.tabs[action].scale_spinbox.setValue(float(scale))
-                self.tabs[action].scale_slider.setValue(int(float(scale) * 100))
-            if seed:
-                self.tabs[action].seed.setPlainText(seed)
-            if steps:
-                steps = int(steps)
-                self.tabs[action].steps_spinbox.setValue(steps)
-                self.tabs[action].steps_slider.setValue(steps)
-            if ddim_eta:
-                ddim_eta = float(ddim_eta)
-                self.tabs[action].ddim_eta_spinbox.setValue(ddim_eta)
-                self.tabs[action].ddim_eta_slider.setValue(ddim_eta * 100)
-            if n_iter:
-                n_iter = int(n_iter)
-                try:
-                    self.tabs[action].n_iter_spinbox.setValue(n_iter)
-                except AttributeError:
-                    pass
-                try:
-                    self.tabs[action].n_iter_slider.setValue(n_iter)
-                except AttributeError:
-                    pass
-            if n_samples:
-                n_samples = int(n_samples)
-                self.tabs[action].samples_spinbox.setValue(n_samples)
-                self.tabs[action].samples_slider.setValue(n_samples)
-            if model:
-                self.tabs[action].model_dropdown.setCurrentText(model)
-            if scheduler:
-                self.tabs[action].scheduler_dropdown.setCurrentText(scheduler)
-        """
-        return
-
-
     def prepare_metadata(self, data):
         if not self.settings_manager.settings.export_metadata.get() or \
                 self.settings_manager.settings.image_export_type.get() != "png":
             return None
         metadata = PngImagePlugin.PngInfo()
         options = data["options"]
         action = data["action"]
@@ -556,19 +457,15 @@
         metadata = self.prepare_metadata(data)
         if metadata:
             image.save(os.path.join(path, filename + extension), pnginfo=metadata)
         else:
             image.save(os.path.join(path, filename + extension))
 
     def generate_callback(self):
-        # check that the correct model is in use for txt2vid
-        if self.current_section == "txt2vid" and self.tabs[self.current_section].model_dropdown.currentText() != "damo-vilab":
-            self.error_handler("Must use damo-vilab model with txt2vid")
-        else:
-            self.generate(True)
+        self.generate(True)
 
     def prep_video(self):
         pass
 
     @property
     def active_rect(self):
         rect = QRect(
@@ -601,15 +498,18 @@
         self.deterministic_images = None
 
     def generate(self, image=None):
         if self.current_section in ("upscale", "superresolution") and self.do_upscale_full_image:
             image_data = self.canvas.current_layer.image_data
             image = image_data.image if image_data else None
             if image is None:
-                self.error_handler("No image to upscale")
+                self.message_var.emit({
+                    "code": MessageCode.ERROR,
+                    "message": "No image to upscale",
+                })
                 return
             downscale_amount = self.downscale_amount
             if downscale_amount > 0:
                 # downscale the image first
                 image = image.resize(
                     (
                         int(image.width // downscale_amount),
@@ -805,14 +705,15 @@
             "pos_y": 0,
             "outpaint_box_rect": self.active_rect,
             "hf_token": self.settings_manager.settings.hf_api_key.get(),
             "enable_controlnet": self.enable_controlnet and self.controlnet is not None,
             "controlnet": self.controlnet,
             "deterministic_generation": self.deterministic,
             "deterministic_seed": False,
+            "zeroshot": self.zeroshot
         }
 
         if action == "superresolution":
             options["original_image_width"] = self.canvas.current_active_image_data.image.width
             options["original_image_height"] = self.canvas.current_active_image_data.image.height
 
         if action in ["txt2img", "img2img", "outpaint", "depth2img", "pix2pix"]:
```

### Comparing `airunner-2.1.3/src/airunner/mixins/history_mixin.py` & `airunner-2.2.0/src/airunner/mixins/history_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,7 +220,10 @@
         sorted_layers = []
         for uuid in layer_order:
             for layer in self.canvas.layers:
                 if layer.uuid == uuid:
                     sorted_layers.append(layer)
                     break
         self.canvas.layers = sorted_layers
+
+    def clear_history(self):
+        self.history.clear()
```

### Comparing `airunner-2.1.3/src/airunner/mixins/lora_mixin.py` & `airunner-2.2.0/src/airunner/mixins/lora_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/mixins/menubar_mixin.py` & `airunner-2.2.0/src/airunner/mixins/menubar_mixin.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,26 @@
         self.actionCopy.triggered.connect(self.copy_image)
         self.actionRotate_90_clockwise.triggered.connect(self.canvas.rotate_90_clockwise)
         self.actionRotate_90_counter_clockwise.triggered.connect(self.canvas.rotate_90_counterclockwise)
         self.initialize_filter_actions()
         self.actionSave_prompt.triggered.connect(self.save_prompt)
         self.actionPrompt_Browser.triggered.connect(self.show_prompt_browser)
         self.image_interpolation.triggered.connect(self.show_image_interpolation)
-        self.actionDeterministic_generation.triggered.connect(self.show_deterministic_generation)
+        self.actionClear_all_prompts.triggered.connect(self.clear_all_prompts)
+
+    def clear_all_prompts(self):
+        for tab_section in self._tabs.keys():
+            self.override_tab_section = tab_section
+            for tab in self.tabs.keys():
+                self.override_section = tab
+                self.prompt = ""
+                self.negative_prompt = ""
+                self.generator_tab_widget.clear_prompts(tab_section, tab)
+        self.override_tab_section = None
+        self.override_section = None
 
     def show_prompt_browser(self):
         PromptBrowser(settings_manager=self.prompts_manager, app=self)
 
     def save_prompt(self):
         saved_prompts = self.prompts_manager.settings.prompts.get()
         saved_prompts.append({
```

### Comparing `airunner-2.1.3/src/airunner/mixins/toolbar_mixin.py` & `airunner-2.2.0/src/airunner/mixins/toolbar_mixin.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/pyqt/base_window_ui.py` & `airunner-2.2.0/src/airunner/pyqt/base_window_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/pyqt/embedding_ui.py` & `airunner-2.2.0/src/airunner/pyqt/embedding_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/pyqt/generate_form_ui.py` & `airunner-2.2.0/src/airunner/pyqt/generate_form_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/pyqt/lora_ui.py` & `airunner-2.2.0/src/airunner/pyqt/lora_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/pyqt/main_window_new_ui.py` & `airunner-2.2.0/src/airunner/pyqt/main_window_new_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 from PyQt6 import QtCore, QtGui, QtWidgets
 
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
         MainWindow.setObjectName("MainWindow")
         MainWindow.resize(1150, 990)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Preferred)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(MainWindow.sizePolicy().hasHeightForWidth())
         MainWindow.setSizePolicy(sizePolicy)
-        MainWindow.setMinimumSize(QtCore.QSize(0, 0))
+        MainWindow.setMinimumSize(QtCore.QSize(0, 900))
         self.centralwidget = QtWidgets.QWidget(parent=MainWindow)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.MinimumExpanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.centralwidget.sizePolicy().hasHeightForWidth())
         self.centralwidget.setSizePolicy(sizePolicy)
         self.centralwidget.setMinimumSize(QtCore.QSize(1000, 512))
@@ -153,36 +153,35 @@
         self.actionBox_Blur_2.setObjectName("actionBox_Blur_2")
         self.actionRotate_90_clockwise = QtGui.QAction(parent=MainWindow)
         self.actionRotate_90_clockwise.setObjectName("actionRotate_90_clockwise")
         self.actionRotate_90_counter_clockwise = QtGui.QAction(parent=MainWindow)
         self.actionRotate_90_counter_clockwise.setObjectName("actionRotate_90_counter_clockwise")
         self.actionSave_prompt = QtGui.QAction(parent=MainWindow)
         self.actionSave_prompt.setObjectName("actionSave_prompt")
-        self.actionPrompt_Browser = QtGui.QAction(parent=MainWindow)
-        self.actionPrompt_Browser.setObjectName("actionPrompt_Browser")
         self.actionShow_Active_Image_Area = QtGui.QAction(parent=MainWindow)
         self.actionShow_Active_Image_Area.setCheckable(True)
         self.actionShow_Active_Image_Area.setObjectName("actionShow_Active_Image_Area")
         self.actionImage_Interpolation = QtGui.QAction(parent=MainWindow)
         self.actionImage_Interpolation.setObjectName("actionImage_Interpolation")
         self.image_interpolation = QtGui.QAction(parent=MainWindow)
         self.image_interpolation.setObjectName("image_interpolation")
         self.actionFilm = QtGui.QAction(parent=MainWindow)
         self.actionFilm.setObjectName("actionFilm")
         self.actionDeterministic_generation = QtGui.QAction(parent=MainWindow)
-        self.actionDeterministic_generation.setObjectName("actionDeterministic_generation")
         self.actionDark_mode = QtGui.QAction(parent=MainWindow)
         self.actionDark_mode.setCheckable(True)
         self.actionDark_mode.setObjectName("actionDark_mode")
         self.actionConsole_window = QtGui.QAction(parent=MainWindow)
         self.actionConsole_window.setObjectName("actionConsole_window")
         self.actionSettings = QtGui.QAction(parent=MainWindow)
         self.actionSettings.setObjectName("actionSettings")
-        self.actionEasy_prompt = QtGui.QAction(parent=MainWindow)
-        self.actionEasy_prompt.setObjectName("actionEasy_prompt")
+        self.actionPrompt_Browser = QtGui.QAction(parent=MainWindow)
+        self.actionPrompt_Browser.setObjectName("actionPrompt_Browser")
+        self.actionClear_all_prompts = QtGui.QAction(parent=MainWindow)
+        self.actionClear_all_prompts.setObjectName("actionClear_all_prompts")
         self.menuFile.addAction(self.actionNew)
         self.menuFile.addAction(self.actionLoad)
         self.menuFile.addAction(self.actionSave)
         self.menuFile.addSeparator()
         self.menuFile.addAction(self.actionSettings)
         self.menuFile.addSeparator()
         self.menuFile.addAction(self.actionExport)
@@ -194,14 +193,16 @@
         self.menuEdit.addAction(self.actionCopy)
         self.menuEdit.addAction(self.actionPaste)
         self.menuEdit.addAction(self.actionUndo)
         self.menuEdit.addAction(self.actionRedo)
         self.menuEdit.addSeparator()
         self.menuEdit.addAction(self.actionRotate_90_clockwise)
         self.menuEdit.addAction(self.actionRotate_90_counter_clockwise)
+        self.menuEdit.addSeparator()
+        self.menuEdit.addAction(self.actionClear_all_prompts)
         self.menuBlur.addSeparator()
         self.menuBlur.addAction(self.actionGaussian_Blur_2)
         self.menuBlur.addAction(self.actionBox_Blur_2)
         self.menuFilters.addAction(self.menuBlur.menuAction())
         self.menuFilters.addSeparator()
         self.menuFilters.addAction(self.actionColor_Balance)
         self.menuFilters.addAction(self.actionSaturation_Filter)
@@ -213,21 +214,17 @@
         self.menuFilters.addAction(self.actionFilm)
         self.menuAbout.addAction(self.actionAbout)
         self.menuAbout.addAction(self.actionBug_report)
         self.menuAbout.addAction(self.actionReport_vulnerability)
         self.menuAbout.addAction(self.actionDiscord)
         self.menuModel_merge.addAction(self.image_interpolation)
         self.menuModel_merge.addSeparator()
-        self.menuModel_merge.addAction(self.actionDeterministic_generation)
-        self.menuModel_merge.addSeparator()
         self.menuModel_merge.addAction(self.actionModel_Merger)
         self.menuModel_merge.addSeparator()
         self.menuModel_merge.addAction(self.actionPrompt_Browser)
-        self.menuModel_merge.addSeparator()
-        self.menuModel_merge.addAction(self.actionEasy_prompt)
         self.menubar.addAction(self.menuFile.menuAction())
         self.menubar.addAction(self.menuEdit.menuAction())
         self.menubar.addAction(self.menuModel_merge.menuAction())
         self.menubar.addAction(self.menuFilters.menuAction())
         self.menubar.addAction(self.menuAbout.menuAction())
 
         self.retranslateUi(MainWindow)
@@ -306,17 +303,17 @@
         self.actionGaussian_Blur_2.setText(_translate("MainWindow", "Gaussian Blur"))
         self.actionBox_Blur_2.setText(_translate("MainWindow", "Box Blur"))
         self.actionRotate_90_clockwise.setText(_translate("MainWindow", "Rotate 90° clockwise"))
         self.actionRotate_90_clockwise.setShortcut(_translate("MainWindow", "Ctrl+R"))
         self.actionRotate_90_counter_clockwise.setText(_translate("MainWindow", "Rotate 90° counter clockwise"))
         self.actionRotate_90_counter_clockwise.setShortcut(_translate("MainWindow", "Ctrl+Shift+R"))
         self.actionSave_prompt.setText(_translate("MainWindow", "Save prompt"))
-        self.actionPrompt_Browser.setText(_translate("MainWindow", "Prompt Browser"))
         self.actionShow_Active_Image_Area.setText(_translate("MainWindow", "Show Active Image Area"))
         self.actionImage_Interpolation.setText(_translate("MainWindow", "Image Interpolation"))
         self.image_interpolation.setText(_translate("MainWindow", "Image Interpolation"))
         self.actionFilm.setText(_translate("MainWindow", "Film"))
-        self.actionDeterministic_generation.setText(_translate("MainWindow", "Deterministic generator"))
         self.actionDark_mode.setText(_translate("MainWindow", "Dark mode"))
         self.actionConsole_window.setText(_translate("MainWindow", "Console window"))
         self.actionSettings.setText(_translate("MainWindow", "Settings"))
-        self.actionEasy_prompt.setText(_translate("MainWindow", "Easy prompt"))
+        self.actionPrompt_Browser.setText(_translate("MainWindow", "Prompt browser"))
+        self.actionClear_all_prompts.setText(_translate("MainWindow", "Clear all prompts"))
+        self.actionClear_all_prompts.setToolTip(_translate("MainWindow", "Remove text from all prompts and negative prompts"))
```

### Comparing `airunner-2.1.3/src/airunner/pyqt/main_window_ui.py` & `airunner-2.2.0/src/airunner/pyqt/main_window_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/pyqt/model_merger_model_ui.py` & `airunner-2.2.0/src/airunner/pyqt/model_merger_model_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/pyqt/model_merger_ui.py` & `airunner-2.2.0/src/airunner/pyqt/model_merger_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/pyqt/noise_filter_ui.py` & `airunner-2.2.0/src/airunner/pyqt/noise_filter_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/pyqt/prompt_browser_prompt_widget_ui.py` & `airunner-2.2.0/src/airunner/pyqt/widgets/slider_ui.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,48 @@
-# Form implementation generated from reading ui file '/home/joe/Projects/imagetopixel/airunner/src/airunner/pyqt/prompt_browser_prompt_widget.ui'
+# Form implementation generated from reading ui file '/home/joe/Projects/imagetopixel/airunner/src/airunner/pyqt/widgets/slider.ui'
 #
 # Created by: PyQt6 UI code generator 6.4.2
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic6 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 
 
 class Ui_Form(object):
     def setupUi(self, Form):
         Form.setObjectName("Form")
-        Form.resize(395, 304)
-        self.gridLayout_2 = QtWidgets.QGridLayout(Form)
-        self.gridLayout_2.setObjectName("gridLayout_2")
-        self.gridLayout = QtWidgets.QGridLayout()
+        Form.resize(242, 93)
+        self.gridLayout = QtWidgets.QGridLayout(Form)
+        self.gridLayout.setContentsMargins(0, 0, 0, 0)
+        self.gridLayout.setSpacing(0)
         self.gridLayout.setObjectName("gridLayout")
-        self.label = QtWidgets.QLabel(parent=Form)
-        font = QtGui.QFont()
-        font.setPointSize(11)
-        font.setBold(True)
-        self.label.setFont(font)
-        self.label.setObjectName("label")
-        self.gridLayout.addWidget(self.label, 0, 0, 1, 1)
-        self.prompt = QtWidgets.QTextBrowser(parent=Form)
-        self.prompt.setObjectName("prompt")
-        self.gridLayout.addWidget(self.prompt, 1, 0, 1, 1)
-        self.label_3 = QtWidgets.QLabel(parent=Form)
-        font = QtGui.QFont()
-        font.setBold(True)
-        self.label_3.setFont(font)
-        self.label_3.setObjectName("label_3")
-        self.gridLayout.addWidget(self.label_3, 2, 0, 1, 1)
-        self.negative_prompt = QtWidgets.QTextBrowser(parent=Form)
-        self.negative_prompt.setObjectName("negative_prompt")
-        self.gridLayout.addWidget(self.negative_prompt, 3, 0, 1, 1)
-        self.horizontalLayout = QtWidgets.QHBoxLayout()
-        self.horizontalLayout.setObjectName("horizontalLayout")
-        self.load_button = QtWidgets.QPushButton(parent=Form)
-        self.load_button.setObjectName("load_button")
-        self.horizontalLayout.addWidget(self.load_button)
-        self.delete_button = QtWidgets.QPushButton(parent=Form)
-        self.delete_button.setObjectName("delete_button")
-        self.horizontalLayout.addWidget(self.delete_button)
-        self.gridLayout.addLayout(self.horizontalLayout, 4, 0, 1, 1)
-        self.gridLayout_2.addLayout(self.gridLayout, 0, 0, 1, 1)
+        self.slider = QtWidgets.QSlider(parent=Form)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Preferred)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.slider.sizePolicy().hasHeightForWidth())
+        self.slider.setSizePolicy(sizePolicy)
+        self.slider.setAutoFillBackground(False)
+        self.slider.setMaximum(100)
+        self.slider.setOrientation(QtCore.Qt.Orientation.Horizontal)
+        self.slider.setObjectName("slider")
+        self.gridLayout.addWidget(self.slider, 0, 0, 1, 1)
+        self.spinbox = QtWidgets.QDoubleSpinBox(parent=Form)
+        self.spinbox.setStyleSheet("background-color: transparent;")
+        self.spinbox.setWrapping(False)
+        self.spinbox.setFrame(False)
+        self.spinbox.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.spinbox.setButtonSymbols(QtWidgets.QAbstractSpinBox.ButtonSymbols.UpDownArrows)
+        self.spinbox.setProperty("showGroupSeparator", False)
+        self.spinbox.setMaximum(1.0)
+        self.spinbox.setSingleStep(0.01)
+        self.spinbox.setObjectName("spinbox")
+        self.gridLayout.addWidget(self.spinbox, 0, 1, 1, 1)
 
         self.retranslateUi(Form)
         QtCore.QMetaObject.connectSlotsByName(Form)
 
     def retranslateUi(self, Form):
         _translate = QtCore.QCoreApplication.translate
         Form.setWindowTitle(_translate("Form", "Form"))
-        self.label.setText(_translate("Form", "Prompt"))
-        self.label_3.setText(_translate("Form", "Negative Prompt"))
-        self.load_button.setText(_translate("Form", "Load"))
-        self.delete_button.setText(_translate("Form", "Delete"))
```

### Comparing `airunner-2.1.3/src/airunner/pyqt/prompt_browser_ui.py` & `airunner-2.2.0/src/airunner/pyqt/prompt_browser_ui.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 
 
 class Ui_Dialog(object):
     def setupUi(self, Dialog):
         Dialog.setObjectName("Dialog")
-        Dialog.resize(397, 304)
+        Dialog.resize(768, 597)
         self.gridLayout_2 = QtWidgets.QGridLayout(Dialog)
         self.gridLayout_2.setObjectName("gridLayout_2")
         self.scrollArea = QtWidgets.QScrollArea(parent=Dialog)
         self.scrollArea.setWidgetResizable(True)
         self.scrollArea.setObjectName("scrollArea")
         self.scrollAreaWidgetContents = QtWidgets.QWidget()
-        self.scrollAreaWidgetContents.setGeometry(QtCore.QRect(0, 0, 377, 284))
+        self.scrollAreaWidgetContents.setGeometry(QtCore.QRect(0, 0, 748, 577))
         self.scrollAreaWidgetContents.setObjectName("scrollAreaWidgetContents")
         self.scrollArea.setWidget(self.scrollAreaWidgetContents)
         self.gridLayout_2.addWidget(self.scrollArea, 0, 0, 1, 1)
 
         self.retranslateUi(Dialog)
         QtCore.QMetaObject.connectSlotsByName(Dialog)
```

### Comparing `airunner-2.1.3/src/airunner/pyqt/saturation_window_ui.py` & `airunner-2.2.0/src/airunner/pyqt/saturation_window_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/pyqt/widgets/canvas_ui.py` & `airunner-2.2.0/src/airunner/pyqt/widgets/canvas_ui.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,27 +20,47 @@
         Form.setSizePolicy(sizePolicy)
         Form.setMinimumSize(QtCore.QSize(66, 66))
         Form.setStyleSheet("b")
         self.gridLayout = QtWidgets.QGridLayout(Form)
         self.gridLayout.setContentsMargins(0, 0, 0, 0)
         self.gridLayout.setSpacing(0)
         self.gridLayout.setObjectName("gridLayout")
-        self.canvas_container = QtWidgets.QFrame(parent=Form)
+        self.central_widget = QtWidgets.QWidget(parent=Form)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.MinimumExpanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.canvas_container.sizePolicy().hasHeightForWidth())
-        self.canvas_container.setSizePolicy(sizePolicy)
-        self.canvas_container.setMinimumSize(QtCore.QSize(200, 200))
-        self.canvas_container.setStyleSheet("")
+        sizePolicy.setHeightForWidth(self.central_widget.sizePolicy().hasHeightForWidth())
+        self.central_widget.setSizePolicy(sizePolicy)
+        self.central_widget.setMinimumSize(QtCore.QSize(200, 200))
+        self.central_widget.setStyleSheet("")
+        self.central_widget.setObjectName("central_widget")
+        self.gridLayout_2 = QtWidgets.QGridLayout(self.central_widget)
+        self.gridLayout_2.setContentsMargins(0, 0, 0, 3)
+        self.gridLayout_2.setHorizontalSpacing(0)
+        self.gridLayout_2.setVerticalSpacing(3)
+        self.gridLayout_2.setObjectName("gridLayout_2")
+        self.canvas_position = QtWidgets.QLabel(parent=self.central_widget)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Maximum)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.canvas_position.sizePolicy().hasHeightForWidth())
+        self.canvas_position.setSizePolicy(sizePolicy)
+        font = QtGui.QFont()
+        font.setPointSize(8)
+        self.canvas_position.setFont(font)
+        self.canvas_position.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
+        self.canvas_position.setObjectName("canvas_position")
+        self.gridLayout_2.addWidget(self.canvas_position, 1, 0, 1, 1)
+        self.canvas_container = QtWidgets.QFrame(parent=self.central_widget)
         self.canvas_container.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
         self.canvas_container.setFrameShadow(QtWidgets.QFrame.Shadow.Plain)
-        self.canvas_container.setMidLineWidth(0)
         self.canvas_container.setObjectName("canvas_container")
-        self.gridLayout.addWidget(self.canvas_container, 0, 0, 1, 1)
+        self.gridLayout_2.addWidget(self.canvas_container, 0, 0, 1, 1)
+        self.gridLayout.addWidget(self.central_widget, 0, 0, 1, 1)
 
         self.retranslateUi(Form)
         QtCore.QMetaObject.connectSlotsByName(Form)
 
     def retranslateUi(self, Form):
         _translate = QtCore.QCoreApplication.translate
         Form.setWindowTitle(_translate("Form", "Form"))
+        self.canvas_position.setText(_translate("Form", "TextLabel"))
```

### Comparing `airunner-2.1.3/src/airunner/pyqt/widgets/embedding_ui.py` & `airunner-2.2.0/src/airunner/pyqt/widgets/embedding_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/pyqt/widgets/generator_tab_ui.py` & `airunner-2.2.0/src/airunner/pyqt/widgets/generator_tab_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/pyqt/widgets/grid_preferences_ui.py` & `airunner-2.2.0/src/airunner/pyqt/widgets/grid_preferences_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/pyqt/widgets/header_ui.py` & `airunner-2.2.0/src/airunner/pyqt/widgets/header_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/pyqt/widgets/layer_container_widget_ui.py` & `airunner-2.2.0/src/airunner/pyqt/widgets/layer_container_widget_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/pyqt/widgets/layer_ui.py` & `airunner-2.2.0/src/airunner/pyqt/widgets/layer_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/pyqt/widgets/lora_container_ui.py` & `airunner-2.2.0/src/airunner/pyqt/widgets/lora_container_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/pyqt/widgets/lora_ui.py` & `airunner-2.2.0/src/airunner/pyqt/widgets/lora_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/pyqt/widgets/prompt_builder_ui.py` & `airunner-2.2.0/src/airunner/pyqt/widgets/prompt_builder_ui.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,26 +8,42 @@
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 
 
 class Ui_Form(object):
     def setupUi(self, Form):
         Form.setObjectName("Form")
-        Form.resize(430, 315)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.MinimumExpanding)
+        Form.resize(816, 405)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Minimum)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(Form.sizePolicy().hasHeightForWidth())
         Form.setSizePolicy(sizePolicy)
-        Form.setMinimumSize(QtCore.QSize(0, 315))
+        Form.setMinimumSize(QtCore.QSize(0, 405))
+        font = QtGui.QFont()
+        font.setPointSize(9)
+        Form.setFont(font)
         self.gridLayout = QtWidgets.QGridLayout(Form)
         self.gridLayout.setContentsMargins(0, 0, 0, 9)
         self.gridLayout.setObjectName("gridLayout")
+        self.line = QtWidgets.QFrame(parent=Form)
+        self.line.setFrameShape(QtWidgets.QFrame.Shape.HLine)
+        self.line.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
+        self.line.setObjectName("line")
+        self.gridLayout.addWidget(self.line, 1, 0, 1, 1)
         self.weights = QtWidgets.QGridLayout()
         self.weights.setObjectName("weights")
+        self.label_5 = QtWidgets.QLabel(parent=Form)
+        font = QtGui.QFont()
+        font.setPointSize(9)
+        font.setBold(False)
+        self.label_5.setFont(font)
+        self.label_5.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
+        self.label_5.setObjectName("label_5")
+        self.weights.addWidget(self.label_5, 2, 4, 1, 1)
         self.label_4 = QtWidgets.QLabel(parent=Form)
         font = QtGui.QFont()
         font.setPointSize(9)
         font.setBold(False)
         self.label_4.setFont(font)
         self.label_4.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.label_4.setObjectName("label_4")
@@ -36,54 +52,29 @@
         font = QtGui.QFont()
         font.setPointSize(9)
         font.setBold(False)
         self.label_3.setFont(font)
         self.label_3.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.label_3.setObjectName("label_3")
         self.weights.addWidget(self.label_3, 1, 4, 1, 1)
-        self.label_7 = QtWidgets.QLabel(parent=Form)
-        font = QtGui.QFont()
-        font.setPointSize(8)
-        font.setBold(True)
-        self.label_7.setFont(font)
-        self.label_7.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
-        self.label_7.setObjectName("label_7")
-        self.weights.addWidget(self.label_7, 0, 2, 1, 1)
-        self.text_prompt_weight_label = QtWidgets.QLabel(parent=Form)
-        font = QtGui.QFont()
-        font.setPointSize(9)
-        font.setBold(True)
-        self.text_prompt_weight_label.setFont(font)
-        self.text_prompt_weight_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignVCenter)
-        self.text_prompt_weight_label.setObjectName("text_prompt_weight_label")
-        self.weights.addWidget(self.text_prompt_weight_label, 1, 1, 1, 1)
-        self.auto_prompt_weight_label = QtWidgets.QLabel(parent=Form)
-        font = QtGui.QFont()
-        font.setPointSize(9)
-        font.setBold(True)
-        self.auto_prompt_weight_label.setFont(font)
-        self.auto_prompt_weight_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
-        self.auto_prompt_weight_label.setObjectName("auto_prompt_weight_label")
-        self.weights.addWidget(self.auto_prompt_weight_label, 1, 3, 1, 1)
-        self.negative_auto_prompt_weight_label = QtWidgets.QLabel(parent=Form)
-        font = QtGui.QFont()
-        font.setPointSize(9)
-        font.setBold(True)
-        self.negative_auto_prompt_weight_label.setFont(font)
-        self.negative_auto_prompt_weight_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
-        self.negative_auto_prompt_weight_label.setObjectName("negative_auto_prompt_weight_label")
-        self.weights.addWidget(self.negative_auto_prompt_weight_label, 2, 3, 1, 1)
-        self.label_6 = QtWidgets.QLabel(parent=Form)
-        font = QtGui.QFont()
-        font.setPointSize(9)
-        font.setBold(False)
-        self.label_6.setFont(font)
-        self.label_6.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignVCenter)
-        self.label_6.setObjectName("label_6")
-        self.weights.addWidget(self.label_6, 2, 0, 1, 1)
+        self.negative_prompt_weight_distribution_slider = QtWidgets.QSlider(parent=Form)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Fixed)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.negative_prompt_weight_distribution_slider.sizePolicy().hasHeightForWidth())
+        self.negative_prompt_weight_distribution_slider.setSizePolicy(sizePolicy)
+        self.negative_prompt_weight_distribution_slider.setMinimumSize(QtCore.QSize(50, 0))
+        self.negative_prompt_weight_distribution_slider.setMaximum(100)
+        self.negative_prompt_weight_distribution_slider.setPageStep(1)
+        self.negative_prompt_weight_distribution_slider.setProperty("value", 50)
+        self.negative_prompt_weight_distribution_slider.setOrientation(QtCore.Qt.Orientation.Horizontal)
+        self.negative_prompt_weight_distribution_slider.setTickPosition(QtWidgets.QSlider.TickPosition.NoTicks)
+        self.negative_prompt_weight_distribution_slider.setTickInterval(1)
+        self.negative_prompt_weight_distribution_slider.setObjectName("negative_prompt_weight_distribution_slider")
+        self.weights.addWidget(self.negative_prompt_weight_distribution_slider, 2, 2, 1, 1)
         self.prompt_weight_distribution_slider = QtWidgets.QSlider(parent=Form)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.prompt_weight_distribution_slider.sizePolicy().hasHeightForWidth())
         self.prompt_weight_distribution_slider.setSizePolicy(sizePolicy)
         self.prompt_weight_distribution_slider.setMinimumSize(QtCore.QSize(50, 0))
@@ -94,333 +85,329 @@
         self.prompt_weight_distribution_slider.setPageStep(1)
         self.prompt_weight_distribution_slider.setProperty("value", 50)
         self.prompt_weight_distribution_slider.setOrientation(QtCore.Qt.Orientation.Horizontal)
         self.prompt_weight_distribution_slider.setTickPosition(QtWidgets.QSlider.TickPosition.NoTicks)
         self.prompt_weight_distribution_slider.setTickInterval(1)
         self.prompt_weight_distribution_slider.setObjectName("prompt_weight_distribution_slider")
         self.weights.addWidget(self.prompt_weight_distribution_slider, 1, 2, 1, 1)
+        self.auto_prompt_weight_label = QtWidgets.QLabel(parent=Form)
+        font = QtGui.QFont()
+        font.setPointSize(9)
+        font.setBold(True)
+        self.auto_prompt_weight_label.setFont(font)
+        self.auto_prompt_weight_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
+        self.auto_prompt_weight_label.setObjectName("auto_prompt_weight_label")
+        self.weights.addWidget(self.auto_prompt_weight_label, 1, 3, 1, 1)
         self.negative_text_prompt_weight_label = QtWidgets.QLabel(parent=Form)
         font = QtGui.QFont()
         font.setPointSize(9)
         font.setBold(True)
         self.negative_text_prompt_weight_label.setFont(font)
         self.negative_text_prompt_weight_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.negative_text_prompt_weight_label.setObjectName("negative_text_prompt_weight_label")
         self.weights.addWidget(self.negative_text_prompt_weight_label, 2, 1, 1, 1)
-        self.negative_prompt_weight_distribution_slider = QtWidgets.QSlider(parent=Form)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Fixed)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.negative_prompt_weight_distribution_slider.sizePolicy().hasHeightForWidth())
-        self.negative_prompt_weight_distribution_slider.setSizePolicy(sizePolicy)
-        self.negative_prompt_weight_distribution_slider.setMinimumSize(QtCore.QSize(50, 0))
-        self.negative_prompt_weight_distribution_slider.setMaximum(100)
-        self.negative_prompt_weight_distribution_slider.setPageStep(1)
-        self.negative_prompt_weight_distribution_slider.setProperty("value", 50)
-        self.negative_prompt_weight_distribution_slider.setOrientation(QtCore.Qt.Orientation.Horizontal)
-        self.negative_prompt_weight_distribution_slider.setTickPosition(QtWidgets.QSlider.TickPosition.NoTicks)
-        self.negative_prompt_weight_distribution_slider.setTickInterval(1)
-        self.negative_prompt_weight_distribution_slider.setObjectName("negative_prompt_weight_distribution_slider")
-        self.weights.addWidget(self.negative_prompt_weight_distribution_slider, 2, 2, 1, 1)
-        self.label_5 = QtWidgets.QLabel(parent=Form)
+        self.label_6 = QtWidgets.QLabel(parent=Form)
         font = QtGui.QFont()
         font.setPointSize(9)
         font.setBold(False)
-        self.label_5.setFont(font)
-        self.label_5.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
-        self.label_5.setObjectName("label_5")
-        self.weights.addWidget(self.label_5, 2, 4, 1, 1)
+        self.label_6.setFont(font)
+        self.label_6.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignVCenter)
+        self.label_6.setObjectName("label_6")
+        self.weights.addWidget(self.label_6, 2, 0, 1, 1)
+        self.label_7 = QtWidgets.QLabel(parent=Form)
+        font = QtGui.QFont()
+        font.setPointSize(8)
+        font.setBold(True)
+        self.label_7.setFont(font)
+        self.label_7.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
+        self.label_7.setObjectName("label_7")
+        self.weights.addWidget(self.label_7, 0, 2, 1, 1)
+        self.negative_auto_prompt_weight_label = QtWidgets.QLabel(parent=Form)
+        font = QtGui.QFont()
+        font.setPointSize(9)
+        font.setBold(True)
+        self.negative_auto_prompt_weight_label.setFont(font)
+        self.negative_auto_prompt_weight_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
+        self.negative_auto_prompt_weight_label.setObjectName("negative_auto_prompt_weight_label")
+        self.weights.addWidget(self.negative_auto_prompt_weight_label, 2, 3, 1, 1)
+        self.text_prompt_weight_label = QtWidgets.QLabel(parent=Form)
+        font = QtGui.QFont()
+        font.setPointSize(9)
+        font.setBold(True)
+        self.text_prompt_weight_label.setFont(font)
+        self.text_prompt_weight_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignVCenter)
+        self.text_prompt_weight_label.setObjectName("text_prompt_weight_label")
+        self.weights.addWidget(self.text_prompt_weight_label, 1, 1, 1, 1)
         self.gridLayout.addLayout(self.weights, 2, 0, 1, 1)
         self.tabs = QtWidgets.QTabWidget(parent=Form)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.tabs.sizePolicy().hasHeightForWidth())
         self.tabs.setSizePolicy(sizePolicy)
         font = QtGui.QFont()
         font.setPointSize(9)
         self.tabs.setFont(font)
         self.tabs.setStyleSheet("")
+        self.tabs.setTabBarAutoHide(True)
         self.tabs.setObjectName("tabs")
-        self.basic = QtWidgets.QWidget()
-        self.basic.setObjectName("basic")
-        self.gridLayout_3 = QtWidgets.QGridLayout(self.basic)
-        self.gridLayout_3.setObjectName("gridLayout_3")
-        self.verticalLayout_2 = QtWidgets.QVBoxLayout()
-        self.verticalLayout_2.setSpacing(6)
-        self.verticalLayout_2.setObjectName("verticalLayout_2")
-        self.label_8 = QtWidgets.QLabel(parent=self.basic)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Fixed)
+        self.advanced = QtWidgets.QWidget()
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Minimum)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.advanced.sizePolicy().hasHeightForWidth())
+        self.advanced.setSizePolicy(sizePolicy)
+        self.advanced.setMinimumSize(QtCore.QSize(0, 300))
+        self.advanced.setObjectName("advanced")
+        self.gridLayout_2 = QtWidgets.QGridLayout(self.advanced)
+        self.gridLayout_2.setObjectName("gridLayout_2")
+        self.gridLayout_9 = QtWidgets.QGridLayout()
+        self.gridLayout_9.setHorizontalSpacing(9)
+        self.gridLayout_9.setObjectName("gridLayout_9")
+        self.scrollArea = QtWidgets.QScrollArea(parent=self.advanced)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Expanding)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.scrollArea.sizePolicy().hasHeightForWidth())
+        self.scrollArea.setSizePolicy(sizePolicy)
+        self.scrollArea.setMinimumSize(QtCore.QSize(250, 120))
+        self.scrollArea.setWidgetResizable(True)
+        self.scrollArea.setObjectName("scrollArea")
+        self.scroll_grid = QtWidgets.QWidget()
+        self.scroll_grid.setGeometry(QtCore.QRect(0, 0, 390, 214))
+        self.scroll_grid.setObjectName("scroll_grid")
+        self.scrollArea.setWidget(self.scroll_grid)
+        self.gridLayout_9.addWidget(self.scrollArea, 0, 1, 1, 1)
+        self.verticalLayout_3 = QtWidgets.QVBoxLayout()
+        self.verticalLayout_3.setObjectName("verticalLayout_3")
+        self.label_16 = QtWidgets.QLabel(parent=self.advanced)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Maximum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.label_8.sizePolicy().hasHeightForWidth())
-        self.label_8.setSizePolicy(sizePolicy)
+        sizePolicy.setHeightForWidth(self.label_16.sizePolicy().hasHeightForWidth())
+        self.label_16.setSizePolicy(sizePolicy)
+        self.label_16.setMaximumSize(QtCore.QSize(200, 16777215))
         font = QtGui.QFont()
         font.setPointSize(8)
         font.setBold(True)
-        self.label_8.setFont(font)
-        self.label_8.setObjectName("label_8")
-        self.verticalLayout_2.addWidget(self.label_8)
-        self.basic_category = QtWidgets.QComboBox(parent=self.basic)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Fixed)
+        self.label_16.setFont(font)
+        self.label_16.setObjectName("label_16")
+        self.verticalLayout_3.addWidget(self.label_16)
+        self.advanced_prompt_text = QtWidgets.QTextBrowser(parent=self.advanced)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Expanding)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.advanced_prompt_text.sizePolicy().hasHeightForWidth())
+        self.advanced_prompt_text.setSizePolicy(sizePolicy)
+        self.advanced_prompt_text.setMinimumSize(QtCore.QSize(200, 0))
+        self.advanced_prompt_text.setMaximumSize(QtCore.QSize(16777215, 16777215))
+        font = QtGui.QFont()
+        font.setPointSize(8)
+        self.advanced_prompt_text.setFont(font)
+        self.advanced_prompt_text.setReadOnly(False)
+        self.advanced_prompt_text.setObjectName("advanced_prompt_text")
+        self.verticalLayout_3.addWidget(self.advanced_prompt_text)
+        self.label_17 = QtWidgets.QLabel(parent=self.advanced)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Maximum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.basic_category.sizePolicy().hasHeightForWidth())
-        self.basic_category.setSizePolicy(sizePolicy)
+        sizePolicy.setHeightForWidth(self.label_17.sizePolicy().hasHeightForWidth())
+        self.label_17.setSizePolicy(sizePolicy)
+        self.label_17.setMaximumSize(QtCore.QSize(200, 16777215))
         font = QtGui.QFont()
         font.setPointSize(9)
-        self.basic_category.setFont(font)
-        self.basic_category.setObjectName("basic_category")
-        self.verticalLayout_2.addWidget(self.basic_category)
-        self.label_9 = QtWidgets.QLabel(parent=self.basic)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Fixed)
+        font.setBold(True)
+        self.label_17.setFont(font)
+        self.label_17.setObjectName("label_17")
+        self.verticalLayout_3.addWidget(self.label_17)
+        self.advanced_negative_prompt_text = QtWidgets.QTextBrowser(parent=self.advanced)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.label_9.sizePolicy().hasHeightForWidth())
-        self.label_9.setSizePolicy(sizePolicy)
+        sizePolicy.setHeightForWidth(self.advanced_negative_prompt_text.sizePolicy().hasHeightForWidth())
+        self.advanced_negative_prompt_text.setSizePolicy(sizePolicy)
+        self.advanced_negative_prompt_text.setMinimumSize(QtCore.QSize(200, 0))
+        self.advanced_negative_prompt_text.setMaximumSize(QtCore.QSize(16777215, 16777215))
         font = QtGui.QFont()
         font.setPointSize(8)
-        font.setBold(True)
-        self.label_9.setFont(font)
-        self.label_9.setObjectName("label_9")
-        self.verticalLayout_2.addWidget(self.label_9)
-        self.basic_prompt = QtWidgets.QComboBox(parent=self.basic)
+        self.advanced_negative_prompt_text.setFont(font)
+        self.advanced_negative_prompt_text.setReadOnly(False)
+        self.advanced_negative_prompt_text.setObjectName("advanced_negative_prompt_text")
+        self.verticalLayout_3.addWidget(self.advanced_negative_prompt_text)
+        self.gridLayout_9.addLayout(self.verticalLayout_3, 0, 2, 1, 1)
+        self.gridLayout_2.addLayout(self.gridLayout_9, 1, 0, 1, 1)
+        self.horizontalLayout_3 = QtWidgets.QHBoxLayout()
+        self.horizontalLayout_3.setObjectName("horizontalLayout_3")
+        self.randomize_values_button = QtWidgets.QPushButton(parent=self.advanced)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.basic_prompt.sizePolicy().hasHeightForWidth())
-        self.basic_prompt.setSizePolicy(sizePolicy)
+        sizePolicy.setHeightForWidth(self.randomize_values_button.sizePolicy().hasHeightForWidth())
+        self.randomize_values_button.setSizePolicy(sizePolicy)
+        self.randomize_values_button.setMinimumSize(QtCore.QSize(20, 0))
+        self.randomize_values_button.setMaximumSize(QtCore.QSize(16777215, 16777215))
+        font = QtGui.QFont()
+        font.setPointSize(8)
+        self.randomize_values_button.setFont(font)
+        self.randomize_values_button.setObjectName("randomize_values_button")
+        self.horizontalLayout_3.addWidget(self.randomize_values_button)
+        self.values_to_random_button = QtWidgets.QPushButton(parent=self.advanced)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Minimum)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.values_to_random_button.sizePolicy().hasHeightForWidth())
+        self.values_to_random_button.setSizePolicy(sizePolicy)
+        self.values_to_random_button.setMinimumSize(QtCore.QSize(20, 0))
+        self.values_to_random_button.setMaximumSize(QtCore.QSize(16777215, 16777215))
         font = QtGui.QFont()
-        font.setPointSize(9)
-        self.basic_prompt.setFont(font)
-        self.basic_prompt.setObjectName("basic_prompt")
-        self.verticalLayout_2.addWidget(self.basic_prompt)
-        self.label_10 = QtWidgets.QLabel(parent=self.basic)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Fixed)
+        font.setPointSize(8)
+        self.values_to_random_button.setFont(font)
+        self.values_to_random_button.setObjectName("values_to_random_button")
+        self.horizontalLayout_3.addWidget(self.values_to_random_button)
+        self.reset_weights_button = QtWidgets.QPushButton(parent=self.advanced)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.label_10.sizePolicy().hasHeightForWidth())
-        self.label_10.setSizePolicy(sizePolicy)
+        sizePolicy.setHeightForWidth(self.reset_weights_button.sizePolicy().hasHeightForWidth())
+        self.reset_weights_button.setSizePolicy(sizePolicy)
+        self.reset_weights_button.setMinimumSize(QtCore.QSize(20, 0))
+        self.reset_weights_button.setMaximumSize(QtCore.QSize(16777215, 16777215))
         font = QtGui.QFont()
         font.setPointSize(8)
-        font.setBold(True)
-        self.label_10.setFont(font)
-        self.label_10.setObjectName("label_10")
-        self.verticalLayout_2.addWidget(self.label_10)
-        self.basic_style = QtWidgets.QComboBox(parent=self.basic)
+        self.reset_weights_button.setFont(font)
+        self.reset_weights_button.setObjectName("reset_weights_button")
+        self.horizontalLayout_3.addWidget(self.reset_weights_button)
+        self.clear_values_button = QtWidgets.QPushButton(parent=self.advanced)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.basic_style.sizePolicy().hasHeightForWidth())
-        self.basic_style.setSizePolicy(sizePolicy)
+        sizePolicy.setHeightForWidth(self.clear_values_button.sizePolicy().hasHeightForWidth())
+        self.clear_values_button.setSizePolicy(sizePolicy)
+        self.clear_values_button.setMinimumSize(QtCore.QSize(20, 0))
+        self.clear_values_button.setMaximumSize(QtCore.QSize(16777215, 16777215))
         font = QtGui.QFont()
-        font.setPointSize(9)
-        self.basic_style.setFont(font)
-        self.basic_style.setObjectName("basic_style")
-        self.verticalLayout_2.addWidget(self.basic_style)
-        self.basic_randomize_checkbox = QtWidgets.QCheckBox(parent=self.basic)
-        font = QtGui.QFont()
-        font.setPointSize(9)
-        self.basic_randomize_checkbox.setFont(font)
-        self.basic_randomize_checkbox.setObjectName("basic_randomize_checkbox")
-        self.verticalLayout_2.addWidget(self.basic_randomize_checkbox)
-        spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
-        self.verticalLayout_2.addItem(spacerItem)
-        self.gridLayout_3.addLayout(self.verticalLayout_2, 0, 0, 1, 1)
-        self.tabs.addTab(self.basic, "")
-        self.advanced = QtWidgets.QWidget()
-        self.advanced.setObjectName("advanced")
-        self.gridLayout_2 = QtWidgets.QGridLayout(self.advanced)
-        self.gridLayout_2.setObjectName("gridLayout_2")
-        self.horizontalLayout_3 = QtWidgets.QHBoxLayout()
-        self.horizontalLayout_3.setObjectName("horizontalLayout_3")
-        self.verticalLayout_8 = QtWidgets.QVBoxLayout()
-        self.verticalLayout_8.setObjectName("verticalLayout_8")
+        font.setPointSize(8)
+        self.clear_values_button.setFont(font)
+        self.clear_values_button.setObjectName("clear_values_button")
+        self.horizontalLayout_3.addWidget(self.clear_values_button)
+        self.gridLayout_2.addLayout(self.horizontalLayout_3, 2, 0, 1, 1)
+        self.gridLayout_10 = QtWidgets.QGridLayout()
+        self.gridLayout_10.setObjectName("gridLayout_10")
         self.label_2 = QtWidgets.QLabel(parent=self.advanced)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Maximum, QtWidgets.QSizePolicy.Policy.Preferred)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Maximum, QtWidgets.QSizePolicy.Policy.Maximum)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_2.sizePolicy().hasHeightForWidth())
         self.label_2.setSizePolicy(sizePolicy)
         font = QtGui.QFont()
         font.setPointSize(8)
         font.setBold(True)
         self.label_2.setFont(font)
         self.label_2.setObjectName("label_2")
-        self.verticalLayout_8.addWidget(self.label_2)
-        self.advanced_category = QtWidgets.QComboBox(parent=self.advanced)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Fixed)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.advanced_category.sizePolicy().hasHeightForWidth())
-        self.advanced_category.setSizePolicy(sizePolicy)
-        self.advanced_category.setMinimumSize(QtCore.QSize(80, 22))
-        self.advanced_category.setMaximumSize(QtCore.QSize(16777215, 16777215))
-        font = QtGui.QFont()
-        font.setPointSize(9)
-        self.advanced_category.setFont(font)
-        self.advanced_category.setObjectName("advanced_category")
-        self.verticalLayout_8.addWidget(self.advanced_category)
-        self.horizontalLayout_3.addLayout(self.verticalLayout_8)
-        self.verticalLayout_9 = QtWidgets.QVBoxLayout()
-        self.verticalLayout_9.setObjectName("verticalLayout_9")
+        self.gridLayout_10.addWidget(self.label_2, 0, 0, 1, 1)
         self.label = QtWidgets.QLabel(parent=self.advanced)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Maximum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label.sizePolicy().hasHeightForWidth())
         self.label.setSizePolicy(sizePolicy)
         font = QtGui.QFont()
         font.setPointSize(8)
         font.setBold(True)
         self.label.setFont(font)
         self.label.setObjectName("label")
-        self.verticalLayout_9.addWidget(self.label)
+        self.gridLayout_10.addWidget(self.label, 0, 1, 1, 1)
+        self.advanced_style = QtWidgets.QComboBox(parent=self.advanced)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Fixed)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.advanced_style.sizePolicy().hasHeightForWidth())
+        self.advanced_style.setSizePolicy(sizePolicy)
+        self.advanced_style.setMinimumSize(QtCore.QSize(80, 22))
+        self.advanced_style.setMaximumSize(QtCore.QSize(16777215, 16777215))
+        font = QtGui.QFont()
+        font.setPointSize(9)
+        self.advanced_style.setFont(font)
+        self.advanced_style.setObjectName("advanced_style")
+        self.gridLayout_10.addWidget(self.advanced_style, 1, 2, 1, 1)
         self.advanced_prompt = QtWidgets.QComboBox(parent=self.advanced)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.advanced_prompt.sizePolicy().hasHeightForWidth())
         self.advanced_prompt.setSizePolicy(sizePolicy)
         self.advanced_prompt.setMinimumSize(QtCore.QSize(80, 22))
         self.advanced_prompt.setMaximumSize(QtCore.QSize(16777215, 16777215))
         font = QtGui.QFont()
         font.setPointSize(9)
         self.advanced_prompt.setFont(font)
         self.advanced_prompt.setObjectName("advanced_prompt")
-        self.verticalLayout_9.addWidget(self.advanced_prompt)
-        self.horizontalLayout_3.addLayout(self.verticalLayout_9)
-        self.verticalLayout_10 = QtWidgets.QVBoxLayout()
-        self.verticalLayout_10.setObjectName("verticalLayout_10")
+        self.gridLayout_10.addWidget(self.advanced_prompt, 1, 1, 1, 1)
+        self.advanced_category = QtWidgets.QComboBox(parent=self.advanced)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Fixed)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.advanced_category.sizePolicy().hasHeightForWidth())
+        self.advanced_category.setSizePolicy(sizePolicy)
+        self.advanced_category.setMinimumSize(QtCore.QSize(80, 22))
+        self.advanced_category.setMaximumSize(QtCore.QSize(16777215, 16777215))
+        font = QtGui.QFont()
+        font.setPointSize(9)
+        self.advanced_category.setFont(font)
+        self.advanced_category.setObjectName("advanced_category")
+        self.gridLayout_10.addWidget(self.advanced_category, 1, 0, 1, 1)
         self.label_11 = QtWidgets.QLabel(parent=self.advanced)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Maximum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_11.sizePolicy().hasHeightForWidth())
         self.label_11.setSizePolicy(sizePolicy)
         font = QtGui.QFont()
         font.setPointSize(8)
         font.setBold(True)
         self.label_11.setFont(font)
         self.label_11.setObjectName("label_11")
-        self.verticalLayout_10.addWidget(self.label_11)
-        self.advanced_style = QtWidgets.QComboBox(parent=self.advanced)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Fixed)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.advanced_style.sizePolicy().hasHeightForWidth())
-        self.advanced_style.setSizePolicy(sizePolicy)
-        self.advanced_style.setMinimumSize(QtCore.QSize(80, 22))
-        self.advanced_style.setMaximumSize(QtCore.QSize(16777215, 16777215))
-        font = QtGui.QFont()
-        font.setPointSize(9)
-        self.advanced_style.setFont(font)
-        self.advanced_style.setObjectName("advanced_style")
-        self.verticalLayout_10.addWidget(self.advanced_style)
-        self.horizontalLayout_3.addLayout(self.verticalLayout_10)
-        self.gridLayout_2.addLayout(self.horizontalLayout_3, 0, 0, 1, 2)
-        self.horizontalLayout_4 = QtWidgets.QHBoxLayout()
-        self.horizontalLayout_4.setObjectName("horizontalLayout_4")
-        self.reset_weights_button = QtWidgets.QPushButton(parent=self.advanced)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Fixed)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.reset_weights_button.sizePolicy().hasHeightForWidth())
-        self.reset_weights_button.setSizePolicy(sizePolicy)
-        self.reset_weights_button.setMinimumSize(QtCore.QSize(20, 0))
-        self.reset_weights_button.setMaximumSize(QtCore.QSize(16777215, 16777215))
+        self.gridLayout_10.addWidget(self.label_11, 0, 2, 1, 1)
+        self.advanced_radio = QtWidgets.QRadioButton(parent=self.advanced)
         font = QtGui.QFont()
         font.setPointSize(8)
-        self.reset_weights_button.setFont(font)
-        self.reset_weights_button.setObjectName("reset_weights_button")
-        self.horizontalLayout_4.addWidget(self.reset_weights_button)
-        self.clear_values_button = QtWidgets.QPushButton(parent=self.advanced)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Fixed)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.clear_values_button.sizePolicy().hasHeightForWidth())
-        self.clear_values_button.setSizePolicy(sizePolicy)
-        self.clear_values_button.setMinimumSize(QtCore.QSize(20, 0))
-        self.clear_values_button.setMaximumSize(QtCore.QSize(16777215, 16777215))
-        font = QtGui.QFont()
-        font.setPointSize(8)
-        self.clear_values_button.setFont(font)
-        self.clear_values_button.setObjectName("clear_values_button")
-        self.horizontalLayout_4.addWidget(self.clear_values_button)
-        self.values_to_random_button = QtWidgets.QPushButton(parent=self.advanced)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Fixed)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.values_to_random_button.sizePolicy().hasHeightForWidth())
-        self.values_to_random_button.setSizePolicy(sizePolicy)
-        self.values_to_random_button.setMinimumSize(QtCore.QSize(20, 0))
-        self.values_to_random_button.setMaximumSize(QtCore.QSize(16777215, 16777215))
+        self.advanced_radio.setFont(font)
+        self.advanced_radio.setObjectName("advanced_radio")
+        self.gridLayout_10.addWidget(self.advanced_radio, 1, 3, 1, 1)
+        self.basic_radio = QtWidgets.QRadioButton(parent=self.advanced)
         font = QtGui.QFont()
         font.setPointSize(8)
-        self.values_to_random_button.setFont(font)
-        self.values_to_random_button.setObjectName("values_to_random_button")
-        self.horizontalLayout_4.addWidget(self.values_to_random_button)
-        self.randomize_values_button = QtWidgets.QPushButton(parent=self.advanced)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Fixed)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.randomize_values_button.sizePolicy().hasHeightForWidth())
-        self.randomize_values_button.setSizePolicy(sizePolicy)
-        self.randomize_values_button.setMinimumSize(QtCore.QSize(20, 0))
-        self.randomize_values_button.setMaximumSize(QtCore.QSize(16777215, 16777215))
-        font = QtGui.QFont()
-        font.setPointSize(8)
-        self.randomize_values_button.setFont(font)
-        self.randomize_values_button.setObjectName("randomize_values_button")
-        self.horizontalLayout_4.addWidget(self.randomize_values_button)
-        self.gridLayout_2.addLayout(self.horizontalLayout_4, 1, 0, 1, 2)
-        self.scrollArea = QtWidgets.QScrollArea(parent=self.advanced)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Expanding)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.scrollArea.sizePolicy().hasHeightForWidth())
-        self.scrollArea.setSizePolicy(sizePolicy)
-        self.scrollArea.setMinimumSize(QtCore.QSize(250, 120))
-        self.scrollArea.setWidgetResizable(True)
-        self.scrollArea.setObjectName("scrollArea")
-        self.scroll_grid = QtWidgets.QWidget()
-        self.scroll_grid.setGeometry(QtCore.QRect(0, 0, 406, 118))
-        self.scroll_grid.setObjectName("scroll_grid")
-        self.scrollArea.setWidget(self.scroll_grid)
-        self.gridLayout_2.addWidget(self.scrollArea, 8, 0, 1, 2)
+        self.basic_radio.setFont(font)
+        self.basic_radio.setObjectName("basic_radio")
+        self.gridLayout_10.addWidget(self.basic_radio, 0, 3, 1, 1)
+        self.gridLayout_2.addLayout(self.gridLayout_10, 0, 0, 1, 1)
         self.tabs.addTab(self.advanced, "")
         self.gridLayout.addWidget(self.tabs, 0, 0, 1, 1)
-        self.line = QtWidgets.QFrame(parent=Form)
-        self.line.setFrameShape(QtWidgets.QFrame.Shape.HLine)
-        self.line.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
-        self.line.setObjectName("line")
-        self.gridLayout.addWidget(self.line, 1, 0, 1, 1)
 
         self.retranslateUi(Form)
         self.tabs.setCurrentIndex(0)
         QtCore.QMetaObject.connectSlotsByName(Form)
 
     def retranslateUi(self, Form):
         _translate = QtCore.QCoreApplication.translate
         Form.setWindowTitle(_translate("Form", "Form"))
+        self.label_5.setText(_translate("Form", "Auto Neg Prompt"))
         self.label_4.setText(_translate("Form", "Text Prompt"))
         self.label_3.setText(_translate("Form", "Auto Prompt"))
-        self.label_7.setText(_translate("Form", "Weight distribution"))
-        self.text_prompt_weight_label.setText(_translate("Form", "0.50"))
         self.auto_prompt_weight_label.setText(_translate("Form", "0.50"))
-        self.negative_auto_prompt_weight_label.setText(_translate("Form", "0.5"))
-        self.label_6.setText(_translate("Form", "Negative Prompt"))
         self.negative_text_prompt_weight_label.setText(_translate("Form", "0.5"))
-        self.label_5.setText(_translate("Form", "Auto Neg Prompt"))
-        self.label_8.setText(_translate("Form", "Category"))
-        self.label_9.setText(_translate("Form", "Prompt"))
-        self.label_10.setText(_translate("Form", "Style"))
-        self.basic_randomize_checkbox.setText(_translate("Form", "Randomize settings"))
-        self.tabs.setTabText(self.tabs.indexOf(self.basic), _translate("Form", "Basic"))
+        self.label_6.setText(_translate("Form", "Negative Prompt"))
+        self.label_7.setText(_translate("Form", "Weight distribution"))
+        self.negative_auto_prompt_weight_label.setText(_translate("Form", "0.5"))
+        self.text_prompt_weight_label.setText(_translate("Form", "0.50"))
+        self.label_16.setText(_translate("Form", "Prompt"))
+        self.label_17.setText(_translate("Form", "Negative Prompt"))
+        self.randomize_values_button.setText(_translate("Form", "Randomize"))
+        self.values_to_random_button.setText(_translate("Form", "To Random"))
+        self.reset_weights_button.setText(_translate("Form", "Reset Weights"))
+        self.clear_values_button.setText(_translate("Form", "Clear"))
         self.label_2.setText(_translate("Form", "Category"))
         self.label.setText(_translate("Form", "Prompt"))
         self.label_11.setText(_translate("Form", "Style"))
-        self.reset_weights_button.setText(_translate("Form", "Reset Weights"))
-        self.clear_values_button.setText(_translate("Form", "Clear Values"))
-        self.values_to_random_button.setText(_translate("Form", "Values to Random"))
-        self.randomize_values_button.setText(_translate("Form", "Randomize values"))
+        self.advanced_radio.setText(_translate("Form", "Advanced"))
+        self.basic_radio.setText(_translate("Form", "Basic"))
         self.tabs.setTabText(self.tabs.indexOf(self.advanced), _translate("Form", "Advanced"))
```

### Comparing `airunner-2.1.3/src/airunner/pyqt/widgets/slider_ui.py` & `airunner-2.2.0/src/airunner/pyqt/widgets/tool_menu_ui.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-# Form implementation generated from reading ui file '/home/joe/Projects/imagetopixel/airunner/src/airunner/pyqt/widgets/slider.ui'
+# Form implementation generated from reading ui file '/home/joe/Projects/imagetopixel/airunner/src/airunner/pyqt/widgets/tool_menu.ui'
 #
 # Created by: PyQt6 UI code generator 6.4.2
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic6 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 
 
 class Ui_Form(object):
     def setupUi(self, Form):
         Form.setObjectName("Form")
-        Form.resize(242, 93)
+        Form.resize(410, 495)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Preferred)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(Form.sizePolicy().hasHeightForWidth())
+        Form.setSizePolicy(sizePolicy)
+        Form.setMinimumSize(QtCore.QSize(250, 0))
         self.gridLayout = QtWidgets.QGridLayout(Form)
         self.gridLayout.setContentsMargins(0, 0, 0, 0)
         self.gridLayout.setSpacing(0)
         self.gridLayout.setObjectName("gridLayout")
-        self.slider = QtWidgets.QSlider(parent=Form)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Preferred)
+        self.right_toolbar = QtWidgets.QWidget(parent=Form)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.slider.sizePolicy().hasHeightForWidth())
-        self.slider.setSizePolicy(sizePolicy)
-        self.slider.setAutoFillBackground(False)
-        self.slider.setMaximum(100)
-        self.slider.setOrientation(QtCore.Qt.Orientation.Horizontal)
-        self.slider.setObjectName("slider")
-        self.gridLayout.addWidget(self.slider, 0, 0, 1, 1)
-        self.spinbox = QtWidgets.QDoubleSpinBox(parent=Form)
-        self.spinbox.setStyleSheet("background-color: transparent;")
-        self.spinbox.setWrapping(False)
-        self.spinbox.setFrame(False)
-        self.spinbox.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
-        self.spinbox.setButtonSymbols(QtWidgets.QAbstractSpinBox.ButtonSymbols.UpDownArrows)
-        self.spinbox.setProperty("showGroupSeparator", False)
-        self.spinbox.setMaximum(1.0)
-        self.spinbox.setSingleStep(0.01)
-        self.spinbox.setObjectName("spinbox")
-        self.gridLayout.addWidget(self.spinbox, 0, 1, 1, 1)
+        sizePolicy.setHeightForWidth(self.right_toolbar.sizePolicy().hasHeightForWidth())
+        self.right_toolbar.setSizePolicy(sizePolicy)
+        self.right_toolbar.setMinimumSize(QtCore.QSize(0, 0))
+        self.right_toolbar.setMaximumSize(QtCore.QSize(16777215, 16777215))
+        font = QtGui.QFont()
+        font.setItalic(False)
+        self.right_toolbar.setFont(font)
+        self.right_toolbar.setStyleSheet("border-top-color: rgba(191, 64, 64, 0);")
+        self.right_toolbar.setObjectName("right_toolbar")
+        self.gridLayout_2 = QtWidgets.QGridLayout(self.right_toolbar)
+        self.gridLayout_2.setContentsMargins(0, 0, 0, 0)
+        self.gridLayout_2.setSpacing(0)
+        self.gridLayout_2.setObjectName("gridLayout_2")
+        self.gridLayout.addWidget(self.right_toolbar, 0, 0, 1, 1)
 
         self.retranslateUi(Form)
         QtCore.QMetaObject.connectSlotsByName(Form)
 
     def retranslateUi(self, Form):
         _translate = QtCore.QCoreApplication.translate
         Form.setWindowTitle(_translate("Form", "Form"))
```

### Comparing `airunner-2.1.3/src/airunner/pyqt/widgets/toolbar_ui.py` & `airunner-2.2.0/src/airunner/pyqt/widgets/toolbar_ui.py`

 * *Files identical despite different names*

### Comparing `airunner-2.1.3/src/airunner/runai_client.py` & `airunner-2.2.0/src/airunner/runai_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,17 +66,14 @@
         self.app = kwargs.get("app", None)
         self.settings_manager = kwargs.get("settings_manager", None)
         self.quit_event = BooleanVar()
         self.queue = queue.Queue()
         self.res_queue = queue.Queue()
         self.quit_event.set(False)
         self.logger = logging.getLogger()
-        self.image_var = kwargs.get("image_var")
-        self.error_var = kwargs.get("error_var")
-        self.tqdm_var = kwargs.get("tqdm_var")
         self.message_var = kwargs.get("message_var")
         self.do_start()
 
     def do_start(self):
         # create a stable diffusion runner service
         # sd_runner_thread = self.start_thread(
         #     target=self.init_sd_runner,
@@ -90,19 +87,16 @@
     def init_sd_runner(self):
         # save sd_runner to disc and load from it next time
         # this is to avoid the overhead of creating a new sd_runner
         # every time we start the client
         self.logger.info("Initialzing SDRunner")
         self.sd_runner = SDRunner(
             app=self.app,
-            tqdm_var=self.tqdm_var,
-            image_var=self.image_var,
             message_var=self.message_var,
             settings_manager=self.settings_manager,
-            error_var=self.error_var,
         )
 
     def handle_response(self, response):
         """
         Handle the response from the server
         :param response:
         :return: None
@@ -136,19 +130,15 @@
                 self.sd_runner.initialized = False
                 self.sd_runner.reload_model = True
 
         if (action in ("txt2img", "img2img") and self.sd_runner.action in ("inpaint", "outpaint")) or \
             (action in ("inpaint", "outpaint") and self.sd_runner.action in ("txt2img", "img2img")):
             self.sd_runner.initialized = False
 
-        self.sd_runner.generator_sample(
-            data,
-            self.image_var,
-            self.error_var
-        )
+        self.sd_runner.generator_sample(data)
 
     def create_worker_thread(self):
         # start worker in a new thread using the self.worker method
         self.response_worker = ResponseWorker(client=self)
         self.request_worker = RequestWorker(client=self, callback=self.callback)
         self.response_worker_thread = QThread()
         self.response_worker_thread.started.connect(self.response_worker.startWork)
```

### Comparing `airunner-2.1.3/src/airunner/themes.py` & `airunner-2.2.0/src/airunner/themes.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,14 +170,15 @@
                    border-radius: 0px;
                }
                background-color: transparent;
             """,
             "slider_label": """
                 font-size: 9pt;
                 color: #ffffff;
+                font-weight: bold;
             """,
             "slider_spinbox": """
                 background-color: #444444;
                 border-left: none;
                 border-color: #555;
                 border-radius: 0px;
             """,
```

### Comparing `airunner-2.1.3/src/airunner/utils.py` & `airunner-2.2.0/src/airunner/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,19 +155,22 @@
 
 def get_latest_version():
     # get latest release from https://github.com/Capsize-Games/airunner/releases/latest
     # follow the redirect to get the version number
     import requests
     import re
     url = "https://github.com/Capsize-Games/airunner/releases/latest"
-    r = requests.get(url)
-    if r.status_code == 200:
-        m = re.search(r"\/Capsize-Games\/airunner\/releases\/tag\/v([0-9\.]+)", r.text)
-        if m:
-            return m.group(1)
+    try:
+        r = requests.get(url)
+        if r.status_code == 200:
+            m = re.search(r"\/Capsize-Games\/airunner\/releases\/tag\/v([0-9\.]+)", r.text)
+            if m:
+                return m.group(1)
+    except ConnectionError:
+        return None
     return None
 
 
 def load_default_models(tab_section, section_name):
     if section_name == "txt2img":
         section_name = "generate"
     section_name = f"{tab_section}_{section_name}"
```

### Comparing `airunner-2.1.3/src/airunner.egg-info/PKG-INFO` & `airunner-2.2.0/src/airunner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airunner
-Version: 2.1.3
+Version: 2.2.0
 Summary: A Stable Diffusion GUI
 Home-page: https://github.com/Capsize-Games/airunner
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `airunner-2.1.3/src/airunner.egg-info/SOURCES.txt` & `airunner-2.2.0/src/airunner.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 LICENSE
 README.md
 setup.py
 src/airunner/__init__.py
 src/airunner/balloon.py
+src/airunner/build_prompt.py
 src/airunner/canvas.py
 src/airunner/error_handler.py
 src/airunner/extensions.py
 src/airunner/history.py
 src/airunner/main.py
 src/airunner/runai_client.py
 src/airunner/themes.py
 src/airunner/utils.py
 src/airunner.egg-info/PKG-INFO
 src/airunner.egg-info/SOURCES.txt
 src/airunner.egg-info/dependency_links.txt
 src/airunner.egg-info/requires.txt
 src/airunner.egg-info/top_level.txt
 src/airunner/data/__init__.py
+src/airunner/data/prompt_data.py
 src/airunner/mixins/__init__.py
 src/airunner/mixins/brushes_mixin.py
 src/airunner/mixins/canvas_active_grid_area_mixin.py
 src/airunner/mixins/canvas_brushes_mixin.py
 src/airunner/mixins/canvas_grid_mixin.py
 src/airunner/mixins/canvas_image_mixin.py
 src/airunner/mixins/canvas_mixin.py
 src/airunner/mixins/canvas_selectionbox_mixin.py
 src/airunner/mixins/canvas_widgets_mixin.py
 src/airunner/mixins/comic_mixin.py
-src/airunner/mixins/embedding_mixin.py
 src/airunner/mixins/extension_mixin.py
 src/airunner/mixins/generator_mixin.py
 src/airunner/mixins/history_mixin.py
 src/airunner/mixins/lora_mixin.py
 src/airunner/mixins/menubar_mixin.py
 src/airunner/mixins/toolbar_mixin.py
 src/airunner/pyqt/__init__.py
```

