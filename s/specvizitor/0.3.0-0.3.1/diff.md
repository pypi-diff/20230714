# Comparing `tmp/specvizitor-0.3.0.tar.gz` & `tmp/specvizitor-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specvizitor-0.3.0.tar", max compression
+gzip compressed data, was "specvizitor-0.3.1.tar", max compression
```

## Comparing `specvizitor-0.3.0.tar` & `specvizitor-0.3.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1532 2023-02-09 15:18:12.389760 specvizitor-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     2960 2023-06-25 12:46:39.526235 specvizitor-0.3.0/README.md
--rw-r--r--   0        0        0      787 2023-07-14 17:26:27.067144 specvizitor-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-08 22:04:29.513388 specvizitor-0.3.0/specvizitor/__init__.py
--rw-r--r--   0        0        0       31 2023-03-26 14:02:46.928611 specvizitor-0.3.0/specvizitor/__main__.py
--rw-r--r--   0        0        0     1370 2023-03-26 18:01:07.869089 specvizitor-0.3.0/specvizitor/appdata.py
--rw-r--r--   0        0        0      133 2023-07-13 11:53:21.467570 specvizitor-0.3.0/specvizitor/config/__init__.py
--rw-r--r--   0        0        0      465 2023-03-26 15:05:35.249523 specvizitor-0.3.0/specvizitor/config/appearance.py
--rw-r--r--   0        0        0      276 2023-03-22 23:56:11.227608 specvizitor-0.3.0/specvizitor/config/cache.py
--rw-r--r--   0        0        0      893 2023-07-13 17:03:20.853015 specvizitor-0.3.0/specvizitor/config/config.py
--rw-r--r--   0        0        0     2192 2023-07-14 14:11:47.060084 specvizitor-0.3.0/specvizitor/config/data_widgets.py
--rw-r--r--   0        0        0      226 2023-07-07 13:16:05.483242 specvizitor-0.3.0/specvizitor/config/spectral_lines.py
--rw-r--r--   0        0        0     2683 2023-03-13 17:19:17.930862 specvizitor-0.3.0/specvizitor/data/icons/dark/arrow-backward-starred.svg
--rw-r--r--   0        0        0     1550 2023-03-13 17:19:10.482762 specvizitor-0.3.0/specvizitor/data/icons/dark/arrow-backward.svg
--rw-r--r--   0        0        0     2672 2023-03-13 17:19:35.231095 specvizitor-0.3.0/specvizitor/data/icons/dark/arrow-forward-starred.svg
--rw-r--r--   0        0        0     1526 2023-03-13 17:19:28.327002 specvizitor-0.3.0/specvizitor/data/icons/dark/arrow-forward.svg
--rw-r--r--   0        0        0     2096 2023-03-13 18:11:02.673646 specvizitor-0.3.0/specvizitor/data/icons/dark/dark-mode.svg
--rw-r--r--   0        0        0     3408 2023-03-13 17:12:33.185381 specvizitor-0.3.0/specvizitor/data/icons/dark/gear.svg
--rw-r--r--   0        0        0     5541 2023-03-13 17:27:50.753743 specvizitor-0.3.0/specvizitor/data/icons/dark/reset-dock-state.svg
--rw-r--r--   0        0        0     2062 2023-03-13 17:28:09.813997 specvizitor-0.3.0/specvizitor/data/icons/dark/reset-view.svg
--rw-r--r--   0        0        0     3573 2023-03-13 17:40:05.591719 specvizitor-0.3.0/specvizitor/data/icons/dark/screenshot.svg
--rw-r--r--   0        0        0     1759 2023-03-13 18:10:03.412660 specvizitor-0.3.0/specvizitor/data/icons/dark/star-empty.svg
--rw-r--r--   0        0        0     2467 2023-03-11 17:32:54.146735 specvizitor-0.3.0/specvizitor/data/icons/dark/star.svg
--rw-r--r--   0        0        0     2682 2023-03-13 17:45:48.524369 specvizitor-0.3.0/specvizitor/data/icons/light/arrow-backward-starred.svg
--rw-r--r--   0        0        0     1550 2023-03-13 17:42:40.537824 specvizitor-0.3.0/specvizitor/data/icons/light/arrow-backward.svg
--rw-r--r--   0        0        0     2671 2023-03-13 17:45:37.424219 specvizitor-0.3.0/specvizitor/data/icons/light/arrow-forward-starred.svg
--rw-r--r--   0        0        0     1525 2023-03-13 17:45:42.380285 specvizitor-0.3.0/specvizitor/data/icons/light/arrow-forward.svg
--rw-r--r--   0        0        0     2112 2023-03-13 17:45:23.436029 specvizitor-0.3.0/specvizitor/data/icons/light/dark-mode.svg
--rw-r--r--   0        0        0     3409 2023-03-13 17:44:57.135674 specvizitor-0.3.0/specvizitor/data/icons/light/gear.svg
--rw-r--r--   0        0        0     5540 2023-03-13 17:44:49.051565 specvizitor-0.3.0/specvizitor/data/icons/light/reset-dock-state.svg
--rw-r--r--   0        0        0     2063 2023-03-13 17:43:52.838804 specvizitor-0.3.0/specvizitor/data/icons/light/reset-view.svg
--rw-r--r--   0        0        0     3573 2023-03-13 17:43:45.198700 specvizitor-0.3.0/specvizitor/data/icons/light/screenshot.svg
--rw-r--r--   0        0        0     1759 2023-03-13 18:10:03.412660 specvizitor-0.3.0/specvizitor/data/icons/light/star-empty.svg
--rw-r--r--   0        0        0     2467 2023-03-11 17:32:54.146735 specvizitor-0.3.0/specvizitor/data/icons/light/star.svg
--rw-r--r--   0        0        0      241 2023-07-13 17:13:08.073189 specvizitor-0.3.0/specvizitor/data/presets/config.yml
--rw-r--r--   0        0        0     1487 2023-07-14 14:11:47.032083 specvizitor-0.3.0/specvizitor/data/presets/data_widgets.yml
--rw-r--r--   0        0        0       35 2023-07-13 12:25:06.556814 specvizitor-0.3.0/specvizitor/data/presets/legacy.txt
--rw-r--r--   0        0        0     1493 2023-07-07 13:15:44.638933 specvizitor-0.3.0/specvizitor/data/presets/spectral_lines.yml
--rw-r--r--   0        0        0        0 2023-02-08 22:04:29.513388 specvizitor-0.3.0/specvizitor/io/__init__.py
--rw-r--r--   0        0        0     1902 2023-03-22 20:25:42.255721 specvizitor-0.3.0/specvizitor/io/catalogue.py
--rw-r--r--   0        0        0     4747 2023-07-13 16:57:19.751915 specvizitor-0.3.0/specvizitor/io/inspection_data.py
--rw-r--r--   0        0        0     7192 2023-07-12 23:18:39.255228 specvizitor-0.3.0/specvizitor/io/viewer_data.py
--rw-r--r--   0        0        0     3399 2023-07-13 12:45:33.020219 specvizitor-0.3.0/specvizitor/main.py
--rw-r--r--   0        0        0        0 2023-03-11 17:32:54.146735 specvizitor-0.3.0/specvizitor/plugins/__init__.py
--rw-r--r--   0        0        0     6583 2023-07-14 17:20:41.934176 specvizitor-0.3.0/specvizitor/plugins/grizli.py
--rw-r--r--   0        0        0      445 2023-07-14 17:20:41.950176 specvizitor-0.3.0/specvizitor/plugins/plugin_core.py
--rw-r--r--   0        0        0        1 2023-03-13 11:54:43.456351 specvizitor-0.3.0/specvizitor/utils/__init__.py
--rw-r--r--   0        0        0     1131 2023-07-12 22:59:17.563036 specvizitor-0.3.0/specvizitor/utils/logs.py
--rw-r--r--   0        0        0     4330 2023-07-13 12:01:03.747251 specvizitor-0.3.0/specvizitor/utils/params.py
--rw-r--r--   0        0        0      776 2023-03-14 22:55:55.102789 specvizitor-0.3.0/specvizitor/utils/table_tools.py
--rw-r--r--   0        0        0      451 2023-03-24 14:14:40.377012 specvizitor-0.3.0/specvizitor/utils/widget_tools.py
--rw-r--r--   0        0        0      982 2023-03-22 17:47:30.671778 specvizitor-0.3.0/specvizitor/widgets/AbstractWidget.py
--rw-r--r--   0        0        0     7683 2023-07-14 17:16:26.498606 specvizitor-0.3.0/specvizitor/widgets/DataViewer.py
--rw-r--r--   0        0        0     4160 2023-03-22 20:25:42.283721 specvizitor-0.3.0/specvizitor/widgets/FileBrowser.py
--rw-r--r--   0        0        0     4650 2023-07-13 11:53:21.439570 specvizitor-0.3.0/specvizitor/widgets/Image2D.py
--rw-r--r--   0        0        0     1356 2023-07-13 11:54:42.376026 specvizitor-0.3.0/specvizitor/widgets/LazyViewerElement.py
--rw-r--r--   0        0        0    20188 2023-07-14 16:21:03.684717 specvizitor-0.3.0/specvizitor/widgets/MainWindow.py
--rw-r--r--   0        0        0     7917 2023-03-26 13:59:44.845098 specvizitor-0.3.0/specvizitor/widgets/NewFile.py
--rw-r--r--   0        0        0     5560 2023-03-26 18:01:07.881089 specvizitor-0.3.0/specvizitor/widgets/ObjectInfo.py
--rw-r--r--   0        0        0     9409 2023-07-13 17:25:57.015814 specvizitor-0.3.0/specvizitor/widgets/Plot1D.py
--rw-r--r--   0        0        0     2449 2023-03-22 17:47:30.659778 specvizitor-0.3.0/specvizitor/widgets/QuickSearch.py
--rw-r--r--   0        0        0     2766 2023-07-14 11:54:18.387960 specvizitor-0.3.0/specvizitor/widgets/ReviewForm.py
--rw-r--r--   0        0        0     3465 2023-03-22 19:59:56.339180 specvizitor-0.3.0/specvizitor/widgets/Section.py
--rw-r--r--   0        0        0     7339 2023-07-11 20:32:31.598754 specvizitor-0.3.0/specvizitor/widgets/Settings.py
--rw-r--r--   0        0        0     5279 2023-03-25 12:42:40.560273 specvizitor-0.3.0/specvizitor/widgets/SmartSlider.py
--rw-r--r--   0        0        0     8587 2023-07-14 14:35:42.596406 specvizitor-0.3.0/specvizitor/widgets/Spec1D.py
--rw-r--r--   0        0        0     3454 2023-03-23 00:24:35.185243 specvizitor-0.3.0/specvizitor/widgets/TableColumns.py
--rw-r--r--   0        0        0     7568 2023-07-14 16:28:29.607076 specvizitor-0.3.0/specvizitor/widgets/ToolBar.py
--rw-r--r--   0        0        0     4884 2023-07-13 11:54:56.392115 specvizitor-0.3.0/specvizitor/widgets/ViewerElement.py
--rw-r--r--   0        0        0        0 2023-03-13 12:09:30.251077 specvizitor-0.3.0/specvizitor/widgets/__init__.py
--rw-r--r--   0        0        0     4381 1970-01-01 00:00:00.000000 specvizitor-0.3.0/setup.py
--rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 specvizitor-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1532 2023-02-09 15:18:12.389760 specvizitor-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     2960 2023-06-25 12:46:39.526235 specvizitor-0.3.1/README.md
+-rw-r--r--   0        0        0      788 2023-07-14 17:33:24.061027 specvizitor-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-08 22:04:29.513388 specvizitor-0.3.1/specvizitor/__init__.py
+-rw-r--r--   0        0        0       31 2023-03-26 14:02:46.928611 specvizitor-0.3.1/specvizitor/__main__.py
+-rw-r--r--   0        0        0     1370 2023-03-26 18:01:07.869089 specvizitor-0.3.1/specvizitor/appdata.py
+-rw-r--r--   0        0        0      133 2023-07-13 11:53:21.467570 specvizitor-0.3.1/specvizitor/config/__init__.py
+-rw-r--r--   0        0        0      465 2023-03-26 15:05:35.249523 specvizitor-0.3.1/specvizitor/config/appearance.py
+-rw-r--r--   0        0        0      276 2023-03-22 23:56:11.227608 specvizitor-0.3.1/specvizitor/config/cache.py
+-rw-r--r--   0        0        0      893 2023-07-13 17:03:20.853015 specvizitor-0.3.1/specvizitor/config/config.py
+-rw-r--r--   0        0        0     2192 2023-07-14 14:11:47.060084 specvizitor-0.3.1/specvizitor/config/data_widgets.py
+-rw-r--r--   0        0        0      226 2023-07-07 13:16:05.483242 specvizitor-0.3.1/specvizitor/config/spectral_lines.py
+-rw-r--r--   0        0        0     2683 2023-03-13 17:19:17.930862 specvizitor-0.3.1/specvizitor/data/icons/dark/arrow-backward-starred.svg
+-rw-r--r--   0        0        0     1550 2023-03-13 17:19:10.482762 specvizitor-0.3.1/specvizitor/data/icons/dark/arrow-backward.svg
+-rw-r--r--   0        0        0     2672 2023-03-13 17:19:35.231095 specvizitor-0.3.1/specvizitor/data/icons/dark/arrow-forward-starred.svg
+-rw-r--r--   0        0        0     1526 2023-03-13 17:19:28.327002 specvizitor-0.3.1/specvizitor/data/icons/dark/arrow-forward.svg
+-rw-r--r--   0        0        0     2096 2023-03-13 18:11:02.673646 specvizitor-0.3.1/specvizitor/data/icons/dark/dark-mode.svg
+-rw-r--r--   0        0        0     3408 2023-03-13 17:12:33.185381 specvizitor-0.3.1/specvizitor/data/icons/dark/gear.svg
+-rw-r--r--   0        0        0     5541 2023-03-13 17:27:50.753743 specvizitor-0.3.1/specvizitor/data/icons/dark/reset-dock-state.svg
+-rw-r--r--   0        0        0     2062 2023-03-13 17:28:09.813997 specvizitor-0.3.1/specvizitor/data/icons/dark/reset-view.svg
+-rw-r--r--   0        0        0     3573 2023-03-13 17:40:05.591719 specvizitor-0.3.1/specvizitor/data/icons/dark/screenshot.svg
+-rw-r--r--   0        0        0     1759 2023-03-13 18:10:03.412660 specvizitor-0.3.1/specvizitor/data/icons/dark/star-empty.svg
+-rw-r--r--   0        0        0     2467 2023-03-11 17:32:54.146735 specvizitor-0.3.1/specvizitor/data/icons/dark/star.svg
+-rw-r--r--   0        0        0     2682 2023-03-13 17:45:48.524369 specvizitor-0.3.1/specvizitor/data/icons/light/arrow-backward-starred.svg
+-rw-r--r--   0        0        0     1550 2023-03-13 17:42:40.537824 specvizitor-0.3.1/specvizitor/data/icons/light/arrow-backward.svg
+-rw-r--r--   0        0        0     2671 2023-03-13 17:45:37.424219 specvizitor-0.3.1/specvizitor/data/icons/light/arrow-forward-starred.svg
+-rw-r--r--   0        0        0     1525 2023-03-13 17:45:42.380285 specvizitor-0.3.1/specvizitor/data/icons/light/arrow-forward.svg
+-rw-r--r--   0        0        0     2112 2023-03-13 17:45:23.436029 specvizitor-0.3.1/specvizitor/data/icons/light/dark-mode.svg
+-rw-r--r--   0        0        0     3409 2023-03-13 17:44:57.135674 specvizitor-0.3.1/specvizitor/data/icons/light/gear.svg
+-rw-r--r--   0        0        0     5540 2023-03-13 17:44:49.051565 specvizitor-0.3.1/specvizitor/data/icons/light/reset-dock-state.svg
+-rw-r--r--   0        0        0     2063 2023-03-13 17:43:52.838804 specvizitor-0.3.1/specvizitor/data/icons/light/reset-view.svg
+-rw-r--r--   0        0        0     3573 2023-03-13 17:43:45.198700 specvizitor-0.3.1/specvizitor/data/icons/light/screenshot.svg
+-rw-r--r--   0        0        0     1759 2023-03-13 18:10:03.412660 specvizitor-0.3.1/specvizitor/data/icons/light/star-empty.svg
+-rw-r--r--   0        0        0     2467 2023-03-11 17:32:54.146735 specvizitor-0.3.1/specvizitor/data/icons/light/star.svg
+-rw-r--r--   0        0        0      241 2023-07-13 17:13:08.073189 specvizitor-0.3.1/specvizitor/data/presets/config.yml
+-rw-r--r--   0        0        0     1487 2023-07-14 14:11:47.032083 specvizitor-0.3.1/specvizitor/data/presets/data_widgets.yml
+-rw-r--r--   0        0        0       35 2023-07-13 12:25:06.556814 specvizitor-0.3.1/specvizitor/data/presets/legacy.txt
+-rw-r--r--   0        0        0     1493 2023-07-07 13:15:44.638933 specvizitor-0.3.1/specvizitor/data/presets/spectral_lines.yml
+-rw-r--r--   0        0        0        0 2023-02-08 22:04:29.513388 specvizitor-0.3.1/specvizitor/io/__init__.py
+-rw-r--r--   0        0        0     1902 2023-03-22 20:25:42.255721 specvizitor-0.3.1/specvizitor/io/catalogue.py
+-rw-r--r--   0        0        0     4747 2023-07-13 16:57:19.751915 specvizitor-0.3.1/specvizitor/io/inspection_data.py
+-rw-r--r--   0        0        0     7192 2023-07-12 23:18:39.255228 specvizitor-0.3.1/specvizitor/io/viewer_data.py
+-rw-r--r--   0        0        0     3399 2023-07-13 12:45:33.020219 specvizitor-0.3.1/specvizitor/main.py
+-rw-r--r--   0        0        0        0 2023-03-11 17:32:54.146735 specvizitor-0.3.1/specvizitor/plugins/__init__.py
+-rw-r--r--   0        0        0     6583 2023-07-14 17:20:41.934176 specvizitor-0.3.1/specvizitor/plugins/grizli.py
+-rw-r--r--   0        0        0      445 2023-07-14 17:20:41.950176 specvizitor-0.3.1/specvizitor/plugins/plugin_core.py
+-rw-r--r--   0        0        0        1 2023-03-13 11:54:43.456351 specvizitor-0.3.1/specvizitor/utils/__init__.py
+-rw-r--r--   0        0        0     1131 2023-07-12 22:59:17.563036 specvizitor-0.3.1/specvizitor/utils/logs.py
+-rw-r--r--   0        0        0     4330 2023-07-13 12:01:03.747251 specvizitor-0.3.1/specvizitor/utils/params.py
+-rw-r--r--   0        0        0      776 2023-03-14 22:55:55.102789 specvizitor-0.3.1/specvizitor/utils/table_tools.py
+-rw-r--r--   0        0        0      451 2023-03-24 14:14:40.377012 specvizitor-0.3.1/specvizitor/utils/widget_tools.py
+-rw-r--r--   0        0        0      982 2023-03-22 17:47:30.671778 specvizitor-0.3.1/specvizitor/widgets/AbstractWidget.py
+-rw-r--r--   0        0        0     7683 2023-07-14 17:16:26.498606 specvizitor-0.3.1/specvizitor/widgets/DataViewer.py
+-rw-r--r--   0        0        0     4160 2023-03-22 20:25:42.283721 specvizitor-0.3.1/specvizitor/widgets/FileBrowser.py
+-rw-r--r--   0        0        0     4650 2023-07-13 11:53:21.439570 specvizitor-0.3.1/specvizitor/widgets/Image2D.py
+-rw-r--r--   0        0        0     1356 2023-07-13 11:54:42.376026 specvizitor-0.3.1/specvizitor/widgets/LazyViewerElement.py
+-rw-r--r--   0        0        0    20188 2023-07-14 16:21:03.684717 specvizitor-0.3.1/specvizitor/widgets/MainWindow.py
+-rw-r--r--   0        0        0     7917 2023-03-26 13:59:44.845098 specvizitor-0.3.1/specvizitor/widgets/NewFile.py
+-rw-r--r--   0        0        0     5560 2023-03-26 18:01:07.881089 specvizitor-0.3.1/specvizitor/widgets/ObjectInfo.py
+-rw-r--r--   0        0        0     9409 2023-07-13 17:25:57.015814 specvizitor-0.3.1/specvizitor/widgets/Plot1D.py
+-rw-r--r--   0        0        0     2449 2023-03-22 17:47:30.659778 specvizitor-0.3.1/specvizitor/widgets/QuickSearch.py
+-rw-r--r--   0        0        0     2766 2023-07-14 11:54:18.387960 specvizitor-0.3.1/specvizitor/widgets/ReviewForm.py
+-rw-r--r--   0        0        0     3465 2023-03-22 19:59:56.339180 specvizitor-0.3.1/specvizitor/widgets/Section.py
+-rw-r--r--   0        0        0     7339 2023-07-11 20:32:31.598754 specvizitor-0.3.1/specvizitor/widgets/Settings.py
+-rw-r--r--   0        0        0     5279 2023-03-25 12:42:40.560273 specvizitor-0.3.1/specvizitor/widgets/SmartSlider.py
+-rw-r--r--   0        0        0     8587 2023-07-14 14:35:42.596406 specvizitor-0.3.1/specvizitor/widgets/Spec1D.py
+-rw-r--r--   0        0        0     3454 2023-03-23 00:24:35.185243 specvizitor-0.3.1/specvizitor/widgets/TableColumns.py
+-rw-r--r--   0        0        0     7568 2023-07-14 16:28:29.607076 specvizitor-0.3.1/specvizitor/widgets/ToolBar.py
+-rw-r--r--   0        0        0     4884 2023-07-13 11:54:56.392115 specvizitor-0.3.1/specvizitor/widgets/ViewerElement.py
+-rw-r--r--   0        0        0        0 2023-03-13 12:09:30.251077 specvizitor-0.3.1/specvizitor/widgets/__init__.py
+-rw-r--r--   0        0        0     4382 1970-01-01 00:00:00.000000 specvizitor-0.3.1/setup.py
+-rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 specvizitor-0.3.1/PKG-INFO
```

### Comparing `specvizitor-0.3.0/LICENSE.txt` & `specvizitor-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/README.md` & `specvizitor-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/pyproject.toml` & `specvizitor-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "specvizitor"
-version = "0.3.0"
+version = "0.3.1"
 description = "Python GUI application for a visual inspection of astronomical spectroscopic data"
 authors = ["Ivan Kramarenko <im.kramarenko@gmail.com>", "Josephine Kerutt <>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/ivkram/specvizitor"
 
 [tool.poetry.dependencies]
@@ -20,12 +20,12 @@
 pyqtdarktheme = "^2.1.0"
 pyqtgraph = "^0.13.1"
 qtpy = "^2.3.0"
 scipy = "^1.10.1"
 specutils = "^1.9.1"
 
 [tool.poetry.scripts]
-specvizitor = 'specvizitor.gui:main'
+specvizitor = 'specvizitor.main:main'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `specvizitor-0.3.0/specvizitor/appdata.py` & `specvizitor-0.3.1/specvizitor/appdata.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/config/config.py` & `specvizitor-0.3.1/specvizitor/config/config.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/config/data_widgets.py` & `specvizitor-0.3.1/specvizitor/config/data_widgets.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/dark/arrow-backward-starred.svg` & `specvizitor-0.3.1/specvizitor/data/icons/dark/arrow-backward-starred.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/dark/arrow-backward.svg` & `specvizitor-0.3.1/specvizitor/data/icons/dark/arrow-backward.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/dark/arrow-forward-starred.svg` & `specvizitor-0.3.1/specvizitor/data/icons/dark/arrow-forward-starred.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/dark/arrow-forward.svg` & `specvizitor-0.3.1/specvizitor/data/icons/dark/arrow-forward.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/dark/dark-mode.svg` & `specvizitor-0.3.1/specvizitor/data/icons/dark/dark-mode.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/dark/gear.svg` & `specvizitor-0.3.1/specvizitor/data/icons/dark/gear.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/dark/reset-dock-state.svg` & `specvizitor-0.3.1/specvizitor/data/icons/dark/reset-dock-state.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/dark/reset-view.svg` & `specvizitor-0.3.1/specvizitor/data/icons/dark/reset-view.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/dark/screenshot.svg` & `specvizitor-0.3.1/specvizitor/data/icons/dark/screenshot.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/dark/star-empty.svg` & `specvizitor-0.3.1/specvizitor/data/icons/dark/star-empty.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/dark/star.svg` & `specvizitor-0.3.1/specvizitor/data/icons/dark/star.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/light/arrow-backward-starred.svg` & `specvizitor-0.3.1/specvizitor/data/icons/light/arrow-backward-starred.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/light/arrow-backward.svg` & `specvizitor-0.3.1/specvizitor/data/icons/light/arrow-backward.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/light/arrow-forward-starred.svg` & `specvizitor-0.3.1/specvizitor/data/icons/light/arrow-forward-starred.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/light/arrow-forward.svg` & `specvizitor-0.3.1/specvizitor/data/icons/light/arrow-forward.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/light/dark-mode.svg` & `specvizitor-0.3.1/specvizitor/data/icons/light/dark-mode.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/light/gear.svg` & `specvizitor-0.3.1/specvizitor/data/icons/light/gear.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/light/reset-dock-state.svg` & `specvizitor-0.3.1/specvizitor/data/icons/light/reset-dock-state.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/light/reset-view.svg` & `specvizitor-0.3.1/specvizitor/data/icons/light/reset-view.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/light/screenshot.svg` & `specvizitor-0.3.1/specvizitor/data/icons/light/screenshot.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/light/star-empty.svg` & `specvizitor-0.3.1/specvizitor/data/icons/light/star-empty.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/icons/light/star.svg` & `specvizitor-0.3.1/specvizitor/data/icons/light/star.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/presets/data_widgets.yml` & `specvizitor-0.3.1/specvizitor/data/presets/data_widgets.yml`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/data/presets/spectral_lines.yml` & `specvizitor-0.3.1/specvizitor/data/presets/spectral_lines.yml`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/io/catalogue.py` & `specvizitor-0.3.1/specvizitor/io/catalogue.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/io/inspection_data.py` & `specvizitor-0.3.1/specvizitor/io/inspection_data.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/io/viewer_data.py` & `specvizitor-0.3.1/specvizitor/io/viewer_data.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/main.py` & `specvizitor-0.3.1/specvizitor/main.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/plugins/grizli.py` & `specvizitor-0.3.1/specvizitor/plugins/grizli.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/utils/logs.py` & `specvizitor-0.3.1/specvizitor/utils/logs.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/utils/params.py` & `specvizitor-0.3.1/specvizitor/utils/params.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/utils/table_tools.py` & `specvizitor-0.3.1/specvizitor/utils/table_tools.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/widgets/AbstractWidget.py` & `specvizitor-0.3.1/specvizitor/widgets/AbstractWidget.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/widgets/DataViewer.py` & `specvizitor-0.3.1/specvizitor/widgets/DataViewer.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/widgets/FileBrowser.py` & `specvizitor-0.3.1/specvizitor/widgets/FileBrowser.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/widgets/Image2D.py` & `specvizitor-0.3.1/specvizitor/widgets/Image2D.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/widgets/LazyViewerElement.py` & `specvizitor-0.3.1/specvizitor/widgets/LazyViewerElement.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/widgets/MainWindow.py` & `specvizitor-0.3.1/specvizitor/widgets/MainWindow.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/widgets/NewFile.py` & `specvizitor-0.3.1/specvizitor/widgets/NewFile.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/widgets/ObjectInfo.py` & `specvizitor-0.3.1/specvizitor/widgets/ObjectInfo.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/widgets/Plot1D.py` & `specvizitor-0.3.1/specvizitor/widgets/Plot1D.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/widgets/QuickSearch.py` & `specvizitor-0.3.1/specvizitor/widgets/QuickSearch.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/widgets/ReviewForm.py` & `specvizitor-0.3.1/specvizitor/widgets/ReviewForm.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/widgets/Section.py` & `specvizitor-0.3.1/specvizitor/widgets/Section.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/widgets/Settings.py` & `specvizitor-0.3.1/specvizitor/widgets/Settings.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/widgets/SmartSlider.py` & `specvizitor-0.3.1/specvizitor/widgets/SmartSlider.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/widgets/Spec1D.py` & `specvizitor-0.3.1/specvizitor/widgets/Spec1D.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/widgets/TableColumns.py` & `specvizitor-0.3.1/specvizitor/widgets/TableColumns.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/widgets/ToolBar.py` & `specvizitor-0.3.1/specvizitor/widgets/ToolBar.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/specvizitor/widgets/ViewerElement.py` & `specvizitor-0.3.1/specvizitor/widgets/ViewerElement.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.3.0/setup.py` & `specvizitor-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,19 +25,19 @@
  'pyqtdarktheme>=2.1.0,<3.0.0',
  'pyqtgraph>=0.13.1,<0.14.0',
  'qtpy>=2.3.0,<3.0.0',
  'scipy>=1.10.1,<2.0.0',
  'specutils>=1.9.1,<2.0.0']
 
 entry_points = \
-{'console_scripts': ['specvizitor = specvizitor.gui:main']}
+{'console_scripts': ['specvizitor = specvizitor.main:main']}
 
 setup_kwargs = {
     'name': 'specvizitor',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Python GUI application for a visual inspection of astronomical spectroscopic data',
     'long_description': '[![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)\n\nSpecvizitor is a Python GUI application for a visual inspection of astronomical spectroscopic data. The main goal is to provide a flexible tool for classifying **large**, **homogeneous** samples of galaxies observed with spectroscopy, which is a typical case for blind spectroscopic surveys. Originally developed for the JWST Cycle 1 program [FRESCO](https://jwst-fresco.astro.unige.ch), this software can be easily adapted for a variety of spectroscopic data sets represented in standard data formats used in the astronomy community (FITS, ASCII, etc.).\n\n![Specvizitor GUI](https://github.com/ivkram/specvizitor/blob/main/docs/screenshots/specvizitor_gui.png?raw=true "Specvizitor GUI")\n\n## Installation\n\n### Installing `specvizitor` using pip\n\nSet up a local environment (Python **3.10+**) and run\n\n```shell\n$ pip install specvizitor\n```\n\n### Installing `specvizitor` from source\n\n1. Clone the public repository:\n\n    ```shell\n    $ git clone https://github.com/ivkram/specvizitor\n    $ cd specvizitor\n    ```\n\n2. Set up a local environment (Python **3.10+**) and run\n\n    ```shell\n    $ pip install -e .\n    ```\n\n## Starting `specvizitor`\n    \nTo start `specvizitor`, activate the local environment and run this command in your terminal:\n\n```shell\n$ specvizitor\n```\n\n## Configuring `specvizitor`\n\nThe basic settings such as the path to the catalogue/data directory are available in `Tools > Settings`. For more advanced settings, open the directory indicated in the bottom of the `Settings` widget ("Advanced settings"). Its location is platform-specific and determined using the [platformdirs](https://pypi.org/project/platformdirs/) package. The directory should contain the following YAML files: `specvizitor.yml` (the general GUI settings), `lines.yml` (the list of spectral lines displayed along with a spectrum) and `docks.yml` (the configuration of the data viewer). Several examples of changing these files for your needs are given below, but note that in the future, `specvizitor` will be fully configurable from the GUI.\n\n### Adding spectral lines\n\nOpen `lines.yml` and add an entry with the name of a spectral line and its rest wavelength to `list`, e.g.:\n\n```yaml\nlist:\n  # ...\n  PaG: 10938.086\n```\n\nBy default, all wavelengths are represented in angstroms, which is determined by the `wave_unit` parameter in the same file.\n\n### Configuring the data viewer\n\nThe content of the data viewer is described in `docks.yml`. There are three types of data that can be displayed in the data viewer: `images`, `plots` and `spectra`. \n\n## Troubleshooting\n\nTo reset `specvizitor` to its initial state, run the script with the `--purge` option:\n\n```shell\n$ specvizitor --purge\n```\n\n## License\n\n`specvizitor` is licensed under a 3-clause BSD style license - see the [LICENSE.txt](https://github.com/ivkram/specvizitor/blob/main/LICENSE.txt) file.\n',
     'author': 'Ivan Kramarenko',
     'author_email': 'im.kramarenko@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ivkram/specvizitor',
```

### Comparing `specvizitor-0.3.0/PKG-INFO` & `specvizitor-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specvizitor
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python GUI application for a visual inspection of astronomical spectroscopic data
 Home-page: https://github.com/ivkram/specvizitor
 License: BSD-3-Clause
 Author: Ivan Kramarenko
 Author-email: im.kramarenko@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: BSD License
```

