# Comparing `tmp/specvizitor-0.2.1.tar.gz` & `tmp/specvizitor-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specvizitor-0.2.1.tar", max compression
+gzip compressed data, was "specvizitor-0.3.0.tar", max compression
```

## Comparing `specvizitor-0.2.1.tar` & `specvizitor-0.3.0.tar`

### file list

```diff
@@ -1,71 +1,72 @@
--rw-r--r--   0        0        0     1532 2023-02-09 15:18:12.389760 specvizitor-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0      895 2023-03-11 17:32:54.138735 specvizitor-0.2.1/README.md
--rw-r--r--   0        0        0      787 2023-03-25 13:05:54.536945 specvizitor-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-08 22:04:29.513388 specvizitor-0.2.1/specvizitor/__init__.py
--rw-r--r--   0        0        0       30 2023-02-08 22:04:29.513388 specvizitor-0.2.1/specvizitor/__main__.py
--rw-r--r--   0        0        0     3022 2023-03-22 23:49:26.532222 specvizitor-0.2.1/specvizitor/appdata.py
--rw-r--r--   0        0        0      120 2023-03-11 17:32:54.142735 specvizitor-0.2.1/specvizitor/config/__init__.py
--rw-r--r--   0        0        0      457 2023-03-22 18:36:57.486099 specvizitor-0.2.1/specvizitor/config/appearance.py
--rw-r--r--   0        0        0      276 2023-03-22 23:56:11.227608 specvizitor-0.2.1/specvizitor/config/cache.py
--rw-r--r--   0        0        0      901 2023-03-24 00:12:03.223355 specvizitor-0.2.1/specvizitor/config/config.py
--rw-r--r--   0        0        0     2065 2023-03-25 12:42:40.572273 specvizitor-0.2.1/specvizitor/config/docks.py
--rw-r--r--   0        0        0      207 2023-03-11 17:32:54.142735 specvizitor-0.2.1/specvizitor/config/spectral_lines.py
--rw-r--r--   0        0        0      276 2023-03-24 13:03:39.871340 specvizitor-0.2.1/specvizitor/data/default_config.yml
--rw-r--r--   0        0        0      997 2023-03-25 12:42:40.580273 specvizitor-0.2.1/specvizitor/data/default_docks.yml
--rw-r--r--   0        0        0      402 2023-03-23 15:24:46.052189 specvizitor-0.2.1/specvizitor/data/default_lines.yml
--rw-r--r--   0        0        0     2683 2023-03-13 17:19:17.930862 specvizitor-0.2.1/specvizitor/data/icons/dark/arrow-backward-starred.svg
--rw-r--r--   0        0        0     1550 2023-03-13 17:19:10.482762 specvizitor-0.2.1/specvizitor/data/icons/dark/arrow-backward.svg
--rw-r--r--   0        0        0     2672 2023-03-13 17:19:35.231095 specvizitor-0.2.1/specvizitor/data/icons/dark/arrow-forward-starred.svg
--rw-r--r--   0        0        0     1526 2023-03-13 17:19:28.327002 specvizitor-0.2.1/specvizitor/data/icons/dark/arrow-forward.svg
--rw-r--r--   0        0        0     2096 2023-03-13 18:11:02.673646 specvizitor-0.2.1/specvizitor/data/icons/dark/dark-mode.svg
--rw-r--r--   0        0        0     3408 2023-03-13 17:12:33.185381 specvizitor-0.2.1/specvizitor/data/icons/dark/gear.svg
--rw-r--r--   0        0        0     5541 2023-03-13 17:27:50.753743 specvizitor-0.2.1/specvizitor/data/icons/dark/reset-dock-state.svg
--rw-r--r--   0        0        0     2062 2023-03-13 17:28:09.813997 specvizitor-0.2.1/specvizitor/data/icons/dark/reset-view.svg
--rw-r--r--   0        0        0     3573 2023-03-13 17:40:05.591719 specvizitor-0.2.1/specvizitor/data/icons/dark/screenshot.svg
--rw-r--r--   0        0        0     1759 2023-03-13 18:10:03.412660 specvizitor-0.2.1/specvizitor/data/icons/dark/star-empty.svg
--rw-r--r--   0        0        0     2467 2023-03-11 17:32:54.146735 specvizitor-0.2.1/specvizitor/data/icons/dark/star.svg
--rw-r--r--   0        0        0     2682 2023-03-13 17:45:48.524369 specvizitor-0.2.1/specvizitor/data/icons/light/arrow-backward-starred.svg
--rw-r--r--   0        0        0     1550 2023-03-13 17:42:40.537824 specvizitor-0.2.1/specvizitor/data/icons/light/arrow-backward.svg
--rw-r--r--   0        0        0     2671 2023-03-13 17:45:37.424219 specvizitor-0.2.1/specvizitor/data/icons/light/arrow-forward-starred.svg
--rw-r--r--   0        0        0     1525 2023-03-13 17:45:42.380285 specvizitor-0.2.1/specvizitor/data/icons/light/arrow-forward.svg
--rw-r--r--   0        0        0     2112 2023-03-13 17:45:23.436029 specvizitor-0.2.1/specvizitor/data/icons/light/dark-mode.svg
--rw-r--r--   0        0        0     3409 2023-03-13 17:44:57.135674 specvizitor-0.2.1/specvizitor/data/icons/light/gear.svg
--rw-r--r--   0        0        0     5540 2023-03-13 17:44:49.051565 specvizitor-0.2.1/specvizitor/data/icons/light/reset-dock-state.svg
--rw-r--r--   0        0        0     2063 2023-03-13 17:43:52.838804 specvizitor-0.2.1/specvizitor/data/icons/light/reset-view.svg
--rw-r--r--   0        0        0     3573 2023-03-13 17:43:45.198700 specvizitor-0.2.1/specvizitor/data/icons/light/screenshot.svg
--rw-r--r--   0        0        0     1759 2023-03-13 18:10:03.412660 specvizitor-0.2.1/specvizitor/data/icons/light/star-empty.svg
--rw-r--r--   0        0        0     2467 2023-03-11 17:32:54.146735 specvizitor-0.2.1/specvizitor/data/icons/light/star.svg
--rw-r--r--   0        0        0    21283 2023-03-24 17:27:14.751167 specvizitor-0.2.1/specvizitor/gui.py
--rw-r--r--   0        0        0        0 2023-02-08 22:04:29.513388 specvizitor-0.2.1/specvizitor/io/__init__.py
--rw-r--r--   0        0        0     1902 2023-03-22 20:25:42.255721 specvizitor-0.2.1/specvizitor/io/catalogue.py
--rw-r--r--   0        0        0     5747 2023-03-21 23:18:29.116010 specvizitor-0.2.1/specvizitor/io/inspection_data.py
--rw-r--r--   0        0        0     6505 2023-03-24 18:56:01.846895 specvizitor-0.2.1/specvizitor/io/viewer_data.py
--rw-r--r--   0        0        0     7925 2023-03-23 10:45:22.360020 specvizitor-0.2.1/specvizitor/menu/NewFile.py
--rw-r--r--   0        0        0     7277 2023-03-23 09:34:42.545727 specvizitor-0.2.1/specvizitor/menu/Settings.py
--rw-r--r--   0        0        0        0 2023-03-13 12:12:38.141286 specvizitor-0.2.1/specvizitor/menu/__init__.py
--rw-r--r--   0        0        0        0 2023-03-11 17:32:54.146735 specvizitor-0.2.1/specvizitor/plugins/__init__.py
--rw-r--r--   0        0        0     4287 2023-03-24 23:42:53.139649 specvizitor-0.2.1/specvizitor/plugins/grizli.py
--rw-r--r--   0        0        0      202 2023-03-23 13:13:58.507422 specvizitor-0.2.1/specvizitor/plugins/plugin_core.py
--rw-r--r--   0        0        0        1 2023-03-13 11:54:43.456351 specvizitor-0.2.1/specvizitor/utils/__init__.py
--rw-r--r--   0        0        0     1131 2023-03-13 12:25:21.966200 specvizitor-0.2.1/specvizitor/utils/logs.py
--rw-r--r--   0        0        0     4311 2023-03-13 12:25:21.982200 specvizitor-0.2.1/specvizitor/utils/params.py
--rw-r--r--   0        0        0      776 2023-03-14 22:55:55.102789 specvizitor-0.2.1/specvizitor/utils/table_tools.py
--rw-r--r--   0        0        0      451 2023-03-24 14:14:40.377012 specvizitor-0.2.1/specvizitor/utils/widget_tools.py
--rw-r--r--   0        0        0      982 2023-03-22 17:47:30.671778 specvizitor-0.2.1/specvizitor/widgets/AbstractWidget.py
--rw-r--r--   0        0        0     6583 2023-03-24 11:04:03.118513 specvizitor-0.2.1/specvizitor/widgets/DataViewer.py
--rw-r--r--   0        0        0     4160 2023-03-22 20:25:42.283721 specvizitor-0.2.1/specvizitor/widgets/FileBrowser.py
--rw-r--r--   0        0        0     2990 2023-03-24 15:43:16.474495 specvizitor-0.2.1/specvizitor/widgets/Image2D.py
--rw-r--r--   0        0        0     1588 2023-03-23 14:59:38.960192 specvizitor-0.2.1/specvizitor/widgets/LazyViewerElement.py
--rw-r--r--   0        0        0     5556 2023-03-23 08:59:02.597529 specvizitor-0.2.1/specvizitor/widgets/ObjectInfo.py
--rw-r--r--   0        0        0     9401 2023-03-25 12:31:19.419611 specvizitor-0.2.1/specvizitor/widgets/Plot1D.py
--rw-r--r--   0        0        0     2449 2023-03-22 17:47:30.659778 specvizitor-0.2.1/specvizitor/widgets/QuickSearch.py
--rw-r--r--   0        0        0     2577 2023-03-22 17:47:30.711779 specvizitor-0.2.1/specvizitor/widgets/ReviewForm.py
--rw-r--r--   0        0        0     3465 2023-03-22 19:59:56.339180 specvizitor-0.2.1/specvizitor/widgets/Section.py
--rw-r--r--   0        0        0     5279 2023-03-25 12:42:40.560273 specvizitor-0.2.1/specvizitor/widgets/SmartSlider.py
--rw-r--r--   0        0        0     8531 2023-03-25 01:22:08.348323 specvizitor-0.2.1/specvizitor/widgets/Spec1D.py
--rw-r--r--   0        0        0     3454 2023-03-23 00:24:35.185243 specvizitor-0.2.1/specvizitor/widgets/TableColumns.py
--rw-r--r--   0        0        0     7478 2023-03-22 19:09:36.486513 specvizitor-0.2.1/specvizitor/widgets/ToolBar.py
--rw-r--r--   0        0        0     4856 2023-03-25 12:42:40.532273 specvizitor-0.2.1/specvizitor/widgets/ViewerElement.py
--rw-r--r--   0        0        0        0 2023-03-13 12:09:30.251077 specvizitor-0.2.1/specvizitor/widgets/__init__.py
--rw-r--r--   0        0        0     2294 1970-01-01 00:00:00.000000 specvizitor-0.2.1/setup.py
--rw-r--r--   0        0        0     2047 1970-01-01 00:00:00.000000 specvizitor-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1532 2023-02-09 15:18:12.389760 specvizitor-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     2960 2023-06-25 12:46:39.526235 specvizitor-0.3.0/README.md
+-rw-r--r--   0        0        0      787 2023-07-14 17:26:27.067144 specvizitor-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-08 22:04:29.513388 specvizitor-0.3.0/specvizitor/__init__.py
+-rw-r--r--   0        0        0       31 2023-03-26 14:02:46.928611 specvizitor-0.3.0/specvizitor/__main__.py
+-rw-r--r--   0        0        0     1370 2023-03-26 18:01:07.869089 specvizitor-0.3.0/specvizitor/appdata.py
+-rw-r--r--   0        0        0      133 2023-07-13 11:53:21.467570 specvizitor-0.3.0/specvizitor/config/__init__.py
+-rw-r--r--   0        0        0      465 2023-03-26 15:05:35.249523 specvizitor-0.3.0/specvizitor/config/appearance.py
+-rw-r--r--   0        0        0      276 2023-03-22 23:56:11.227608 specvizitor-0.3.0/specvizitor/config/cache.py
+-rw-r--r--   0        0        0      893 2023-07-13 17:03:20.853015 specvizitor-0.3.0/specvizitor/config/config.py
+-rw-r--r--   0        0        0     2192 2023-07-14 14:11:47.060084 specvizitor-0.3.0/specvizitor/config/data_widgets.py
+-rw-r--r--   0        0        0      226 2023-07-07 13:16:05.483242 specvizitor-0.3.0/specvizitor/config/spectral_lines.py
+-rw-r--r--   0        0        0     2683 2023-03-13 17:19:17.930862 specvizitor-0.3.0/specvizitor/data/icons/dark/arrow-backward-starred.svg
+-rw-r--r--   0        0        0     1550 2023-03-13 17:19:10.482762 specvizitor-0.3.0/specvizitor/data/icons/dark/arrow-backward.svg
+-rw-r--r--   0        0        0     2672 2023-03-13 17:19:35.231095 specvizitor-0.3.0/specvizitor/data/icons/dark/arrow-forward-starred.svg
+-rw-r--r--   0        0        0     1526 2023-03-13 17:19:28.327002 specvizitor-0.3.0/specvizitor/data/icons/dark/arrow-forward.svg
+-rw-r--r--   0        0        0     2096 2023-03-13 18:11:02.673646 specvizitor-0.3.0/specvizitor/data/icons/dark/dark-mode.svg
+-rw-r--r--   0        0        0     3408 2023-03-13 17:12:33.185381 specvizitor-0.3.0/specvizitor/data/icons/dark/gear.svg
+-rw-r--r--   0        0        0     5541 2023-03-13 17:27:50.753743 specvizitor-0.3.0/specvizitor/data/icons/dark/reset-dock-state.svg
+-rw-r--r--   0        0        0     2062 2023-03-13 17:28:09.813997 specvizitor-0.3.0/specvizitor/data/icons/dark/reset-view.svg
+-rw-r--r--   0        0        0     3573 2023-03-13 17:40:05.591719 specvizitor-0.3.0/specvizitor/data/icons/dark/screenshot.svg
+-rw-r--r--   0        0        0     1759 2023-03-13 18:10:03.412660 specvizitor-0.3.0/specvizitor/data/icons/dark/star-empty.svg
+-rw-r--r--   0        0        0     2467 2023-03-11 17:32:54.146735 specvizitor-0.3.0/specvizitor/data/icons/dark/star.svg
+-rw-r--r--   0        0        0     2682 2023-03-13 17:45:48.524369 specvizitor-0.3.0/specvizitor/data/icons/light/arrow-backward-starred.svg
+-rw-r--r--   0        0        0     1550 2023-03-13 17:42:40.537824 specvizitor-0.3.0/specvizitor/data/icons/light/arrow-backward.svg
+-rw-r--r--   0        0        0     2671 2023-03-13 17:45:37.424219 specvizitor-0.3.0/specvizitor/data/icons/light/arrow-forward-starred.svg
+-rw-r--r--   0        0        0     1525 2023-03-13 17:45:42.380285 specvizitor-0.3.0/specvizitor/data/icons/light/arrow-forward.svg
+-rw-r--r--   0        0        0     2112 2023-03-13 17:45:23.436029 specvizitor-0.3.0/specvizitor/data/icons/light/dark-mode.svg
+-rw-r--r--   0        0        0     3409 2023-03-13 17:44:57.135674 specvizitor-0.3.0/specvizitor/data/icons/light/gear.svg
+-rw-r--r--   0        0        0     5540 2023-03-13 17:44:49.051565 specvizitor-0.3.0/specvizitor/data/icons/light/reset-dock-state.svg
+-rw-r--r--   0        0        0     2063 2023-03-13 17:43:52.838804 specvizitor-0.3.0/specvizitor/data/icons/light/reset-view.svg
+-rw-r--r--   0        0        0     3573 2023-03-13 17:43:45.198700 specvizitor-0.3.0/specvizitor/data/icons/light/screenshot.svg
+-rw-r--r--   0        0        0     1759 2023-03-13 18:10:03.412660 specvizitor-0.3.0/specvizitor/data/icons/light/star-empty.svg
+-rw-r--r--   0        0        0     2467 2023-03-11 17:32:54.146735 specvizitor-0.3.0/specvizitor/data/icons/light/star.svg
+-rw-r--r--   0        0        0      241 2023-07-13 17:13:08.073189 specvizitor-0.3.0/specvizitor/data/presets/config.yml
+-rw-r--r--   0        0        0     1487 2023-07-14 14:11:47.032083 specvizitor-0.3.0/specvizitor/data/presets/data_widgets.yml
+-rw-r--r--   0        0        0       35 2023-07-13 12:25:06.556814 specvizitor-0.3.0/specvizitor/data/presets/legacy.txt
+-rw-r--r--   0        0        0     1493 2023-07-07 13:15:44.638933 specvizitor-0.3.0/specvizitor/data/presets/spectral_lines.yml
+-rw-r--r--   0        0        0        0 2023-02-08 22:04:29.513388 specvizitor-0.3.0/specvizitor/io/__init__.py
+-rw-r--r--   0        0        0     1902 2023-03-22 20:25:42.255721 specvizitor-0.3.0/specvizitor/io/catalogue.py
+-rw-r--r--   0        0        0     4747 2023-07-13 16:57:19.751915 specvizitor-0.3.0/specvizitor/io/inspection_data.py
+-rw-r--r--   0        0        0     7192 2023-07-12 23:18:39.255228 specvizitor-0.3.0/specvizitor/io/viewer_data.py
+-rw-r--r--   0        0        0     3399 2023-07-13 12:45:33.020219 specvizitor-0.3.0/specvizitor/main.py
+-rw-r--r--   0        0        0        0 2023-03-11 17:32:54.146735 specvizitor-0.3.0/specvizitor/plugins/__init__.py
+-rw-r--r--   0        0        0     6583 2023-07-14 17:20:41.934176 specvizitor-0.3.0/specvizitor/plugins/grizli.py
+-rw-r--r--   0        0        0      445 2023-07-14 17:20:41.950176 specvizitor-0.3.0/specvizitor/plugins/plugin_core.py
+-rw-r--r--   0        0        0        1 2023-03-13 11:54:43.456351 specvizitor-0.3.0/specvizitor/utils/__init__.py
+-rw-r--r--   0        0        0     1131 2023-07-12 22:59:17.563036 specvizitor-0.3.0/specvizitor/utils/logs.py
+-rw-r--r--   0        0        0     4330 2023-07-13 12:01:03.747251 specvizitor-0.3.0/specvizitor/utils/params.py
+-rw-r--r--   0        0        0      776 2023-03-14 22:55:55.102789 specvizitor-0.3.0/specvizitor/utils/table_tools.py
+-rw-r--r--   0        0        0      451 2023-03-24 14:14:40.377012 specvizitor-0.3.0/specvizitor/utils/widget_tools.py
+-rw-r--r--   0        0        0      982 2023-03-22 17:47:30.671778 specvizitor-0.3.0/specvizitor/widgets/AbstractWidget.py
+-rw-r--r--   0        0        0     7683 2023-07-14 17:16:26.498606 specvizitor-0.3.0/specvizitor/widgets/DataViewer.py
+-rw-r--r--   0        0        0     4160 2023-03-22 20:25:42.283721 specvizitor-0.3.0/specvizitor/widgets/FileBrowser.py
+-rw-r--r--   0        0        0     4650 2023-07-13 11:53:21.439570 specvizitor-0.3.0/specvizitor/widgets/Image2D.py
+-rw-r--r--   0        0        0     1356 2023-07-13 11:54:42.376026 specvizitor-0.3.0/specvizitor/widgets/LazyViewerElement.py
+-rw-r--r--   0        0        0    20188 2023-07-14 16:21:03.684717 specvizitor-0.3.0/specvizitor/widgets/MainWindow.py
+-rw-r--r--   0        0        0     7917 2023-03-26 13:59:44.845098 specvizitor-0.3.0/specvizitor/widgets/NewFile.py
+-rw-r--r--   0        0        0     5560 2023-03-26 18:01:07.881089 specvizitor-0.3.0/specvizitor/widgets/ObjectInfo.py
+-rw-r--r--   0        0        0     9409 2023-07-13 17:25:57.015814 specvizitor-0.3.0/specvizitor/widgets/Plot1D.py
+-rw-r--r--   0        0        0     2449 2023-03-22 17:47:30.659778 specvizitor-0.3.0/specvizitor/widgets/QuickSearch.py
+-rw-r--r--   0        0        0     2766 2023-07-14 11:54:18.387960 specvizitor-0.3.0/specvizitor/widgets/ReviewForm.py
+-rw-r--r--   0        0        0     3465 2023-03-22 19:59:56.339180 specvizitor-0.3.0/specvizitor/widgets/Section.py
+-rw-r--r--   0        0        0     7339 2023-07-11 20:32:31.598754 specvizitor-0.3.0/specvizitor/widgets/Settings.py
+-rw-r--r--   0        0        0     5279 2023-03-25 12:42:40.560273 specvizitor-0.3.0/specvizitor/widgets/SmartSlider.py
+-rw-r--r--   0        0        0     8587 2023-07-14 14:35:42.596406 specvizitor-0.3.0/specvizitor/widgets/Spec1D.py
+-rw-r--r--   0        0        0     3454 2023-03-23 00:24:35.185243 specvizitor-0.3.0/specvizitor/widgets/TableColumns.py
+-rw-r--r--   0        0        0     7568 2023-07-14 16:28:29.607076 specvizitor-0.3.0/specvizitor/widgets/ToolBar.py
+-rw-r--r--   0        0        0     4884 2023-07-13 11:54:56.392115 specvizitor-0.3.0/specvizitor/widgets/ViewerElement.py
+-rw-r--r--   0        0        0        0 2023-03-13 12:09:30.251077 specvizitor-0.3.0/specvizitor/widgets/__init__.py
+-rw-r--r--   0        0        0     4381 1970-01-01 00:00:00.000000 specvizitor-0.3.0/setup.py
+-rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 specvizitor-0.3.0/PKG-INFO
```

### Comparing `specvizitor-0.2.1/LICENSE.txt` & `specvizitor-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/pyproject.toml` & `specvizitor-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "specvizitor"
-version = "0.2.1"
+version = "0.3.0"
 description = "Python GUI application for a visual inspection of astronomical spectroscopic data"
 authors = ["Ivan Kramarenko <im.kramarenko@gmail.com>", "Josephine Kerutt <>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/ivkram/specvizitor"
 
 [tool.poetry.dependencies]
```

### Comparing `specvizitor-0.2.1/specvizitor/appdata.py` & `specvizitor-0.3.0/specvizitor/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,92 @@
-from astropy.table import Table
-from platformdirs import user_config_dir, user_cache_dir
+import pyqtgraph as pg
+from qtpy import QtWidgets
 
-from dataclasses import dataclass
+import argparse
+import importlib
 import logging
 import pathlib
+from platformdirs import user_config_dir, user_cache_dir
+import sys
 
-from .config import Config, Docks, SpectralLines, Cache
-from .io.inspection_data import InspectionData
+from .config.appearance import set_up_appearance
+from .config import Config, DataWidgets, SpectralLines, Cache
+from .io.viewer_data import add_enabled_aliases
 from .utils.params import LocalFile
 
+from .widgets.MainWindow import MainWindow
+
 logger = logging.getLogger(__name__)
 
+ORGANIZATION_NAME = 'FRESCO'
+APPLICATION_NAME = __package__.split('.')[0]
+
+CONFIG_DIR = user_config_dir(APPLICATION_NAME)
+CACHE_DIR = user_cache_dir(APPLICATION_NAME)
+
+
+def main():
+    parser = argparse.ArgumentParser()
+    parser.add_argument('--verbose', action='store_true')
+    parser.add_argument('--purge', action='store_true')
+
+    args = parser.parse_args()
+
+    # configure logging parameters
+    level = logging.INFO if args.verbose else logging.WARNING
+    logging.basicConfig(format='%(asctime)s - %(name)s - %(levelname)s - %(message)s', level=level)
+
+    # configure pyqtgraph options
+    pg.setConfigOption('imageAxisOrder', 'row-major')
+
+    # read local config files
+    local_files: dict[str, LocalFile] = {
+        'config': LocalFile(CONFIG_DIR, filename='config.yml', full_name='General GUI settings'),
+        'cache': LocalFile(CACHE_DIR, full_name='Cache', auto_backup=False),
+        'widgets': LocalFile(CONFIG_DIR, filename='data_widgets.yml', full_name='Data viewer configuration'),
+        'lines': LocalFile(CONFIG_DIR, filename='spectral_lines.yml', full_name='List of spectral lines'),
+    }
+
+    if args.purge:
+        # deleting old configuration files which are no longer in use
+        with open(pathlib.Path(__file__).parent / 'data' / 'presets' / 'legacy.txt', 'r') as file:
+            for line in file:
+                legacy_config = pathlib.Path(CONFIG_DIR) / line.rstrip()
+                legacy_config.unlink(missing_ok=True)
+                (legacy_config.parent / (legacy_config.name + '.bak')).unlink(missing_ok=True)
+
+        for f in local_files.values():
+            f.delete()  # safe delete
+
+    config = Config.read_user_params(local_files['config'], default='config.yml')
+
+    # register unit aliases
+    if config.data.enabled_unit_aliases is not None:
+        add_enabled_aliases(config.data.enabled_unit_aliases)
+
+    # start the application
+    app = QtWidgets.QApplication(sys.argv)
+    app.setOrganizationName(ORGANIZATION_NAME)
+    app.setApplicationName(APPLICATION_NAME.capitalize())
+    logger.info("Application started")
+
+    # set up the GUI appearance
+    set_up_appearance(cfg=config.appearance)
+
+    # "discover" and "register" plugins (to be updated)
+    plugins = [importlib.import_module("specvizitor.plugins." + plugin_name).Plugin()
+               for plugin_name in config.plugins]
+
+    # create the main window
+    window = MainWindow(config=config,
+                        cache=Cache.read_user_params(local_files['cache']),
+                        viewer_cfg=DataWidgets.read_user_params(local_files['widgets'], default='data_widgets.yml'),
+                        spectral_lines=SpectralLines.read_user_params(local_files['lines'],
+                                                                      default='spectral_lines.yml'),
+                        plugins=plugins)
+    window.show()
+
+    sys.exit(app.exec_())
 
-@dataclass
-class AppData:
-    config: Config
-    cache: Cache
-
-    docks: Docks
-    lines: SpectralLines
-
-    output_path: pathlib.Path | None = None  # the path to the output (a.k.a. inspection) file
-    cat: Table | None = None                 # the catalogue
-    notes: InspectionData | None = None      # inspection results
-
-    j: int = None  # the index of the current object
-
-    @classmethod
-    def init_from_disk(cls, purge=False):
-
-        user_files: dict[str, LocalFile] = {
-            'config': LocalFile(user_config_dir('specvizitor'), full_name='Settings file'),
-            'docks': LocalFile(user_config_dir('specvizitor'), filename='docks.yml',
-                               full_name='Dock configuration file'),
-            'lines': LocalFile(user_config_dir('specvizitor'), filename='lines.yml',
-                               full_name='List of spectral lines'),
-            'cache': LocalFile(user_cache_dir('specvizitor'), full_name='Cache file', auto_backup=False)
-        }
-
-        if purge:
-            for f in user_files.values():
-                f.delete()
-
-        return cls(config=Config.read_user_params(user_files['config'], default='default_config.yml'),
-                   docks=Docks.read_user_params(user_files['docks'], default='default_docks.yml'),
-                   lines=SpectralLines.read_user_params(user_files['lines'], default='default_lines.yml'),
-                   cache=Cache.read_user_params(user_files['cache']))
-
-    def create(self):
-        """ Create an object for storing inspection data.
-        """
-        if self.cat is None:
-            logger.error("Failed to create a new object for storing inspection data: the catalogue is not loaded"
-                         "to the memory")
-            return
-
-        self.notes = InspectionData.create(self.cat['id'], self.config.review_form.default_checkboxes)
-
-    def read(self):
-        """ Read the inspection file. If the catalogue hasn't been already initialized, load it from the disk. If
-        unsuccessful, create a new catalogue with a single column of IDs given by the inspection file.
-        """
-        if self.output_path is None:
-            logger.error("Failed to read the inspection file: the file path is not specified")
-            return
-
-        self.notes = InspectionData.read(self.output_path)
-
-    def save(self):
-        """ Save inspection data to the output file.
-        """
-        if self.output_path is None:
-            logger.error("Failed to save the inspection data: the output path is not specified")
-            return
 
-        self.notes.write(self.output_path)
-        logger.info('Project saved (path: {})'.format(self.output_path))
+if __name__ == '__main__':
+    main()
```

### Comparing `specvizitor-0.2.1/specvizitor/config/config.py` & `specvizitor-0.3.0/specvizitor/config/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,28 +9,28 @@
     translate: dict[str, list[str]] | None = None
 
 
 @dataclass
 class Data:
     dir: str = '.'
     id_pattern: str = r'\d+'
-    user_defined_units: dict[str, str] | None = None
+    enabled_unit_aliases: dict[str, str] | None = None
 
 
 @dataclass
 class Appearance:
     theme: str = 'light'
     antialiasing: bool = False
     viewer_spacing: int = 5
     viewer_margins: int = 5
 
 
 @dataclass
 class ReviewForm:
-    default_checkboxes: dict[str, str] | None = None
+    default_flags: list[str] | None = None
 
 
 @dataclass
 class Config(Params):
     appearance: Appearance = field(default_factory=lambda: Appearance())
     catalogue: Catalogue = field(default_factory=lambda: Catalogue())
     data: Data = field(default_factory=lambda: Data())
```

### Comparing `specvizitor-0.2.1/specvizitor/config/docks.py` & `specvizitor-0.3.0/specvizitor/config/data_widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     limits: Limits = field(default_factory=Limits)
     label: Label = field(default_factory=Label)
 
 
 @dataclass
 class LazyViewerElement:
     visible: bool = True
-
     position: str | None = None
     relative_to: str | None = None
 
 
 @dataclass
 class DataElement:
     filename_keyword: str | None = None
@@ -58,22 +57,25 @@
     loader_params: dict[str, Any] | None = None
 
 
 @dataclass
 class ViewerElement(LazyViewerElement):
     data: DataElement = field(default_factory=DataElement)
     smoothing_slider: Slider = field(default_factory=lambda: Slider(max_value=3, step=0.05))
+    dock_title_fmt: str | None = None
 
 
 @dataclass
 class Image(ViewerElement):
-    rotate: int = 0
-    scale: float = 1
+    rotate: int | None = None
+    scale: float | None = None
     container: str = 'ViewBox'
     color_bar: ColorBar = field(default_factory=ColorBar)
+    central_axes: str | None = None
+    crosshair: bool = False
 
 
 @dataclass
 class Plot1D(ViewerElement):
     x_axis: Axis = field(default_factory=Axis)
     y_axis: Axis = field(default_factory=Axis)
 
@@ -87,11 +89,11 @@
 class Spectrum(Plot1D):
     data: DataElement = field(default_factory=lambda: DataElement(loader='specutils'))
     redshift_slider: Slider = field(default_factory=lambda: Slider(max_value=10, step=1e-4))
     tracked_lines: dict[str, SpectrumRegion] | None = None
 
 
 @dataclass
-class Docks(Params):
+class DataWidgets(Params):
     images: dict[str, Image] | None
     plots: dict[str, Plot1D] | None
     spectra: dict[str, Spectrum] | None
```

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/dark/arrow-backward-starred.svg` & `specvizitor-0.3.0/specvizitor/data/icons/dark/arrow-backward-starred.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/dark/arrow-backward.svg` & `specvizitor-0.3.0/specvizitor/data/icons/dark/arrow-backward.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/dark/arrow-forward-starred.svg` & `specvizitor-0.3.0/specvizitor/data/icons/dark/arrow-forward-starred.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/dark/arrow-forward.svg` & `specvizitor-0.3.0/specvizitor/data/icons/dark/arrow-forward.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/dark/dark-mode.svg` & `specvizitor-0.3.0/specvizitor/data/icons/dark/dark-mode.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/dark/gear.svg` & `specvizitor-0.3.0/specvizitor/data/icons/dark/gear.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/dark/reset-dock-state.svg` & `specvizitor-0.3.0/specvizitor/data/icons/dark/reset-dock-state.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/dark/reset-view.svg` & `specvizitor-0.3.0/specvizitor/data/icons/dark/reset-view.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/dark/screenshot.svg` & `specvizitor-0.3.0/specvizitor/data/icons/dark/screenshot.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/dark/star-empty.svg` & `specvizitor-0.3.0/specvizitor/data/icons/dark/star-empty.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/dark/star.svg` & `specvizitor-0.3.0/specvizitor/data/icons/dark/star.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/light/arrow-backward-starred.svg` & `specvizitor-0.3.0/specvizitor/data/icons/light/arrow-backward-starred.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/light/arrow-backward.svg` & `specvizitor-0.3.0/specvizitor/data/icons/light/arrow-backward.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/light/arrow-forward-starred.svg` & `specvizitor-0.3.0/specvizitor/data/icons/light/arrow-forward-starred.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/light/arrow-forward.svg` & `specvizitor-0.3.0/specvizitor/data/icons/light/arrow-forward.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/light/dark-mode.svg` & `specvizitor-0.3.0/specvizitor/data/icons/light/dark-mode.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/light/gear.svg` & `specvizitor-0.3.0/specvizitor/data/icons/light/gear.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/light/reset-dock-state.svg` & `specvizitor-0.3.0/specvizitor/data/icons/light/reset-dock-state.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/light/reset-view.svg` & `specvizitor-0.3.0/specvizitor/data/icons/light/reset-view.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/light/screenshot.svg` & `specvizitor-0.3.0/specvizitor/data/icons/light/screenshot.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/light/star-empty.svg` & `specvizitor-0.3.0/specvizitor/data/icons/light/star-empty.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/data/icons/light/star.svg` & `specvizitor-0.3.0/specvizitor/data/icons/light/star.svg`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/gui.py` & `specvizitor-0.3.0/specvizitor/widgets/MainWindow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,136 +1,132 @@
 from astropy.table import Table
-import pyqtgraph as pg
 import qtpy.compat
-from qtpy import QtGui, QtWidgets, QtCore
-from qtpy.QtCore import Slot
+from qtpy import QtWidgets, QtCore, QtGui
 
-import argparse
 from dataclasses import asdict
-import importlib
 from importlib.metadata import version
 import logging
 import pathlib
-import sys
 
-from .appdata import AppData
-from .config import appearance, config, Docks
-from .utils.logs import LogMessageBox
-from .utils.params import save_yaml
-from .io.catalogue import read_cat, create_cat
-from .io.inspection_data import InspectionData
-from .io.viewer_data import add_enabled_aliases
-
-from .menu.NewFile import NewFile
-from .menu.Settings import Settings
-
-from .widgets.DataViewer import DataViewer
-from .widgets.ToolBar import ToolBar
-from .widgets.QuickSearch import QuickSearch
-from .widgets.ObjectInfo import ObjectInfo
-from .widgets.ReviewForm import ReviewForm
+from ..appdata import AppData
+from ..config import config as cfg
+from ..config.appearance import set_up_appearance
+from ..config import Config, Cache, DataWidgets, SpectralLines
+from ..io.catalogue import read_cat, create_cat
+from ..io.inspection_data import InspectionData
+from ..utils.logs import LogMessageBox
+from ..utils.params import save_yaml
+
+from .DataViewer import DataViewer
+from .NewFile import NewFile
+from .ObjectInfo import ObjectInfo
+from .QuickSearch import QuickSearch
+from .ReviewForm import ReviewForm
+from .Settings import Settings
+from .ToolBar import ToolBar
 
 logger = logging.getLogger(__name__)
 
 
 class MainWindow(QtWidgets.QMainWindow):
     project_loaded = QtCore.Signal(InspectionData)
     data_requested = QtCore.Signal()
-    object_selected = QtCore.Signal(int, InspectionData, Table, config.Data)
+    object_selected = QtCore.Signal(int, InspectionData, Table, cfg.Data)
 
     theme_changed = QtCore.Signal()
     catalogue_changed = QtCore.Signal(object)
     visible_columns_updated = QtCore.Signal(list)
     dock_layout_updated = QtCore.Signal(dict)
-    dock_configuration_updated = QtCore.Signal(Docks)
+    viewer_configuration_updated = QtCore.Signal(DataWidgets)
 
     screenshot_path_selected = QtCore.Signal(str)
 
-    def __init__(self, appdata: AppData, parent=None):
+    def __init__(self, config: Config, cache: Cache, viewer_cfg: DataWidgets,
+                 spectral_lines: SpectralLines | None = None, plugins=None, parent=None):
         super().__init__(parent)
 
-        self.rd = appdata
+        self.rd = AppData()
+        
+        self._config = config
+        self._cache = cache
+
+        self._viewer_cfg = viewer_cfg
+        self._spectral_lines = spectral_lines
+
+        self._plugins = plugins
 
         self.was_maximized: bool = False
         self.setFocusPolicy(QtCore.Qt.StrongFocus)
 
         self._update_window_title()  # set the title of the main window
         # self.setWindowIcon(QtGui.QIcon('logo2_2.png'))
 
-        # register user-defined units
-        if appdata.config.data.user_defined_units is not None:
-            add_enabled_aliases(appdata.config.data.user_defined_units)
-
-        # "discover" and "register" plugins
-        self._plugins = [importlib.import_module("specvizitor.plugins." + plugin_name).Plugin()
-                         for plugin_name in self.rd.config.plugins]
-
         # add a status bar
         # self.statusBar().showMessage("Message in the statusbar")
 
-        self.data_viewer: DataViewer | None = None
-        self.toolbar: ToolBar | None = None
-        self.quick_search: QuickSearch | None = None
-        self.object_info: ObjectInfo | None = None
-        self.review_form: ReviewForm | None = None
-
-        self.quick_search_dock: QtWidgets.QDockWidget | None = None
-        self.object_info_dock: QtWidgets.QDockWidget | None = None
-        self.review_form_dock: QtWidgets.QDockWidget | None = None
+        self._data_viewer: DataViewer | None = None
+        self._commands_bar: ToolBar | None = None
+        self._quick_search: QuickSearch | None = None
+        self._object_info: ObjectInfo | None = None
+        self._review_form: ReviewForm | None = None
+
+        self._quick_search_dock: QtWidgets.QDockWidget | None = None
+        self._object_info_dock: QtWidgets.QDockWidget | None = None
+        self._review_form_dock: QtWidgets.QDockWidget | None = None
 
         self.init_ui()
         self.populate()
         self.connect()
 
         self.restore_window_state()
 
         # restore the dock state (= the layout of the data viewer) from cache
-        if self.rd.cache.dock_layout:
-            self.dock_layout_updated.emit(self.rd.cache.dock_layout)
+        if self._cache.dock_layout:
+            self.dock_layout_updated.emit(self._cache.dock_layout)
 
         # load the catalogue to the memory
-        if self.rd.config.catalogue.filename:
+        if self._config.catalogue.filename:
             self.load_catalogue()
 
         # update the list of catalogue columns visible in the object info widget
         # write "is not None" explicitly in case visible_columns == []
-        if self.rd.cat and self.rd.cache.visible_columns is not None:
-            self.visible_columns_updated.emit(self.rd.cache.visible_columns)
+        if self.rd.cat and self._cache.visible_columns is not None:
+            self.visible_columns_updated.emit(self._cache.visible_columns)
 
         # read cache and try to load the last active project
-        if self.rd.cache.last_inspection_file:
-            self.open_file(self.rd.cache.last_inspection_file, self.rd.cache.last_object_index)
+        if self._cache.last_inspection_file:
+            self.open_file(self._cache.last_inspection_file, self._cache.last_object_index)
 
     def init_ui(self):
         # create a central widget
-        self.data_viewer = DataViewer(self.rd.docks, self.rd.config.appearance,
-                                      spectral_lines=self.rd.lines, plugins=self._plugins, parent=self)
+        self._data_viewer = DataViewer(self._viewer_cfg, self._config.appearance,
+                                       spectral_lines=self._spectral_lines, plugins=self._plugins, parent=self)
 
         # create a toolbar
-        self.toolbar = ToolBar(self.rd, self.rd.config.appearance, parent=self)
-        self.toolbar.setObjectName('Toolbar')
-        self.toolbar.setEnabled(True)
+        self._commands_bar = ToolBar(self.rd, self._config.appearance, parent=self)
+        self._commands_bar.setObjectName('Toolbar')
+        self._commands_bar.setEnabled(True)
 
         # create a quick search widget
-        self.quick_search = QuickSearch(parent=self)
-        self.quick_search_dock = QtWidgets.QDockWidget('Quick Search', self)
-        self.quick_search_dock.setObjectName('Quick Search')
-        self.quick_search_dock.setWidget(self.quick_search)
+        self._quick_search = QuickSearch(parent=self)
+        self._quick_search_dock = QtWidgets.QDockWidget('Quick Search', self)
+        self._quick_search_dock.setObjectName('Quick Search')
+        self._quick_search_dock.setWidget(self._quick_search)
 
         # create a widget displaying information about the object
-        self.object_info = ObjectInfo(parent=self)
-        self.object_info_dock = QtWidgets.QDockWidget('Object Information', self)
-        self.object_info_dock.setObjectName('Object Information')
-        self.object_info_dock.setWidget(self.object_info)
+        self._object_info = ObjectInfo(parent=self)
+        self._object_info_dock = QtWidgets.QDockWidget('Object Information', self)
+        self._object_info_dock.setObjectName('Object Information')
+        self._object_info_dock.setWidget(self._object_info)
 
         # create a widget for writing comments
-        self.review_form = ReviewForm(cfg=self.rd.config.review_form, parent=self)
-        self.review_form_dock = QtWidgets.QDockWidget('Review Form', self)
-        self.review_form_dock.setObjectName('Review Form')
-        self.review_form_dock.setWidget(self.review_form)
+        self._review_form = ReviewForm(cfg=self._config.review_form, parent=self)
+        self._review_form_dock = QtWidgets.QDockWidget('Review Form', self)
+        self._review_form_dock.setObjectName('Review Form')
+        self._review_form_dock.setWidget(self._review_form)
 
         self._init_menu()
 
     def _init_menu(self):
         self._menu = self.menuBar()
 
         self._file = self._menu.addMenu("&File")
@@ -172,50 +168,48 @@
         self._quit.triggered.connect(self._exit_action)
         self._quit.setShortcut(QtGui.QKeySequence('Ctrl+Q'))
         self._file.addAction(self._quit)
 
         self._view = self._menu.addMenu("&View")
 
         self._reset_view = QtWidgets.QAction("Reset View")
-        self._reset_view.setShortcut('F5')
         self._reset_view.setEnabled(False)
-        self._reset_view.triggered.connect(self.data_viewer.view_reset.emit)
+        self._reset_view.triggered.connect(self._data_viewer.view_reset.emit)
         self._view.addAction(self._reset_view)
 
         self._reset_dock_layout = QtWidgets.QAction("Reset Layout")
         self._reset_dock_layout.setEnabled(False)
-        self._reset_dock_layout.triggered.connect(self.data_viewer.reset_dock_layout)
+        self._reset_dock_layout.triggered.connect(self._data_viewer.init_docks)
         self._view.addAction(self._reset_dock_layout)
 
         self._view.addSeparator()
 
         self._fullscreen = QtWidgets.QAction("Fullscreen")
         self._fullscreen.triggered.connect(lambda:
                                            self._exit_fullscreen() if self.isFullScreen() else self._enter_fullscreen())
         self._fullscreen.setShortcut('F11')
         self._view.addAction(self._fullscreen)
 
-        self._shortcut_fullscreen = QtWidgets.QShortcut('Esc', self)
-        self._shortcut_fullscreen.activated.connect(lambda: self._exit_fullscreen() if self.isFullScreen() else None)
+        QtWidgets.QShortcut('Esc', self, lambda: self._exit_fullscreen() if self.isFullScreen() else None)
 
-        self._docks = self._menu.addMenu("&Docks")
+        self._widgets = self._menu.addMenu("&Widgets")
 
-        self._add_dock = QtWidgets.QAction("Add...")
-        self._add_dock.setEnabled(False)
-        self._docks.addAction(self._add_dock)
+        self._add_widget = QtWidgets.QAction("Add...")
+        self._add_widget.setEnabled(False)
+        self._widgets.addAction(self._add_widget)
 
-        self._docks.addSeparator()
+        self._widgets.addSeparator()
 
-        self._backup_dock_configuration = QtWidgets.QAction("Backup...")
-        self._backup_dock_configuration.triggered.connect(self._backup_dock_configuration_action)
-        self._docks.addAction(self._backup_dock_configuration)
+        self._backup_viewer_config = QtWidgets.QAction("Backup...")
+        self._backup_viewer_config.triggered.connect(self._backup_viewer_config_action)
+        self._widgets.addAction(self._backup_viewer_config)
 
-        self._restore_dock_configuration = QtWidgets.QAction("Restore...")
-        self._restore_dock_configuration.triggered.connect(self._restore_dock_configuration_action)
-        self._docks.addAction(self._restore_dock_configuration)
+        self._restore_viewer_config = QtWidgets.QAction("Restore...")
+        self._restore_viewer_config.triggered.connect(self._restore_viewer_config_action)
+        self._widgets.addAction(self._restore_viewer_config)
 
         self._tools = self._menu.addMenu("&Tools")
 
         self._screenshot = QtWidgets.QAction("Take Screenshot...")
         self._screenshot.triggered.connect(self._screenshot_action)
         self._tools.addAction(self._screenshot)
 
@@ -228,61 +222,61 @@
         self._help = self._menu.addMenu("&Help")
         self._about = QtWidgets.QAction("&About...")
         self._about.triggered.connect(self._about_action)
         self._help.addAction(self._about)
 
     def connect(self):
         # connect the main window to the child widgets
-        for w in (self.data_viewer, self.toolbar, self.quick_search, self.object_info, self.review_form):
+        for w in (self._data_viewer, self._commands_bar, self._quick_search, self._object_info, self._review_form):
             self.project_loaded.connect(w.load_project)
 
-        for w in (self.data_viewer, self.object_info, self.review_form):
+        for w in (self._data_viewer, self._object_info, self._review_form):
             self.data_requested.connect(w.collect)
 
-        for w in (self.data_viewer, self.toolbar, self.object_info, self.review_form):
+        for w in (self._data_viewer, self._commands_bar, self._object_info, self._review_form):
             self.object_selected.connect(w.load_object)
 
-        self.theme_changed.connect(self.data_viewer.init_ui)
-        self.theme_changed.connect(self.toolbar.set_icons)
-        self.catalogue_changed.connect(self.object_info.update_table_items)
-        self.visible_columns_updated.connect(self.object_info.update_visible_columns)
+        self.theme_changed.connect(self._data_viewer.init_ui)
+        self.theme_changed.connect(self._commands_bar.set_icons)
+        self.catalogue_changed.connect(self._object_info.update_table_items)
+        self.visible_columns_updated.connect(self._object_info.update_visible_columns)
 
-        self.dock_layout_updated.connect(self.data_viewer.restore_dock_layout)
-        self.dock_configuration_updated.connect(self.data_viewer.update_dock_configuration)
+        self.dock_layout_updated.connect(self._data_viewer.restore_dock_layout)
+        self.viewer_configuration_updated.connect(self._data_viewer.update_viewer_configuration)
 
-        self.screenshot_path_selected.connect(self.data_viewer.take_screenshot)
+        self.screenshot_path_selected.connect(self._data_viewer.take_screenshot)
 
         # connect the child widgets to the main window
-        self.quick_search.id_selected.connect(self._select_by_id)
-        self.quick_search.index_selected.connect(self._select_by_index)
-        self.toolbar.object_selected.connect(self.load_object)
-        self.toolbar.screenshot_button_clicked.connect(self._screenshot_action)
-        self.toolbar.settings_button_clicked.connect(self._settings_action)
-
-        self.data_viewer.data_collected.connect(self._save_viewer_data)
-        self.object_info.data_collected.connect(self._save_obj_info_data)
-        self.review_form.data_collected.connect(self._save_review_data)
+        self._quick_search.id_selected.connect(self._select_by_id)
+        self._quick_search.index_selected.connect(self._select_by_index)
+        self._commands_bar.object_selected.connect(self.load_object)
+        self._commands_bar.screenshot_button_clicked.connect(self._screenshot_action)
+        self._commands_bar.settings_button_clicked.connect(self._settings_action)
+
+        self._data_viewer.data_collected.connect(self._save_viewer_data)
+        self._object_info.data_collected.connect(self._save_obj_info_data)
+        self._review_form.data_collected.connect(self._save_review_data)
 
         # connect the child widgets between each other
-        self.toolbar.reset_view_button_clicked.connect(self.data_viewer.view_reset.emit)
-        self.toolbar.reset_layout_button_clicked.connect(self.data_viewer.reset_dock_layout)
+        self._commands_bar.reset_view_button_clicked.connect(self._data_viewer.view_reset.emit)
+        self._commands_bar.reset_layout_button_clicked.connect(self._data_viewer.init_docks)
 
     def populate(self):
-        self.setCentralWidget(self.data_viewer)
+        self.setCentralWidget(self._data_viewer)
 
-        self.addToolBar(QtCore.Qt.TopToolBarArea, self.toolbar)
-        self.addDockWidget(QtCore.Qt.RightDockWidgetArea, self.quick_search_dock)
-        self.addDockWidget(QtCore.Qt.RightDockWidgetArea, self.object_info_dock)
-        self.addDockWidget(QtCore.Qt.RightDockWidgetArea, self.review_form_dock)
+        self.addToolBar(QtCore.Qt.TopToolBarArea, self._commands_bar)
+        self.addDockWidget(QtCore.Qt.RightDockWidgetArea, self._quick_search_dock)
+        self.addDockWidget(QtCore.Qt.RightDockWidgetArea, self._object_info_dock)
+        self.addDockWidget(QtCore.Qt.RightDockWidgetArea, self._review_form_dock)
 
     def load_catalogue(self):
-        cat = read_cat(self.rd.config.catalogue.filename, translate=self.rd.config.catalogue.translate)
+        cat = read_cat(self._config.catalogue.filename, translate=self._config.catalogue.translate)
         if cat is None:
-            self.rd.config.catalogue.filename = None
-            self.rd.config.save()
+            self._config.catalogue.filename = None
+            self._config.save()
 
         self.update_catalogue(cat)
 
     def restore_window_state(self):
         settings = QtCore.QSettings()
         if settings.value("geometry") is None or settings.value("windowState") is None:
             self.showMaximized()
@@ -290,19 +284,19 @@
         else:
             self.restoreGeometry(settings.value("geometry"))
             self.restoreState(settings.value("windowState"))
 
     def _new_file_action(self):
         """ Create a new inspection file via the NewFile dialog.
         """
-        dialog = NewFile(cfg=self.rd.config, parent=self)
+        dialog = NewFile(cfg=self._config, parent=self)
         dialog.catalogue_changed.connect(self.update_catalogue)
         dialog.output_path_selected.connect(self.update_output_path)
         if dialog.exec():
-            self.rd.create()
+            self.rd.create(flags=self._config.review_form.default_flags)
             self.load_project()
 
     def _open_file_action(self):
         """ Open an existing inspection file via QFileDialog.
         """
         path = qtpy.compat.getopenfilename(self, caption='Open Inspection File', filters='CSV Files (*.csv)')[0]
         if path:
@@ -324,62 +318,62 @@
 
     def load_project(self, j: int | None = None):
         """ Update the state of the main window and activate the central widget after loading inspection data.
         """
         for w in (self._save, self._save_as, self._export, self._reset_view, self._reset_dock_layout):
             w.setEnabled(True)
 
-        self.project_loaded.emit(self.rd.notes)
+        self.project_loaded.emit(self.rd.review)
 
-        if j is None or (j < 0 or j >= self.rd.notes.n_objects):
+        if j is None or (j < 0 or j >= self.rd.review.n_objects):
             j = 0
 
         self.load_object(j, request_data=False)
 
-    @Slot(int)
+    @QtCore.Slot(int)
     def load_object(self, j: int, request_data=True):
         """ Load a new object to the central widget.
         @param j: the index of the object to display
         @param request_data:
         """
         if request_data:
             self.data_requested.emit()
 
         self.rd.j = j
 
         # cache the index of the object
-        self.rd.cache.last_object_index = j
-        self.rd.cache.save()
+        self._cache.last_object_index = j
+        self._cache.save()
 
-        self.object_selected.emit(self.rd.j, self.rd.notes, self.rd.cat, self.rd.config.data)
+        self.object_selected.emit(self.rd.j, self.rd.review, self.rd.cat, self._config.data)
 
         self._update_window_title()
 
     def reload(self):
         if self.rd.j is not None:
             self.load_object(self.rd.j)
 
     def _update_window_title(self):
         title = ''
         if self.rd.output_path is not None:
             title += f'{self.rd.output_path.name} – '
         if self.rd.j is not None:
-            title += f'ID {self.rd.notes.get_id(self.rd.j)} [#{self.rd.j + 1}/{self.rd.notes.n_objects}] – '
+            title += f'ID {self.rd.review.get_id(self.rd.j)} [#{self.rd.j + 1}/{self.rd.review.n_objects}] – '
         title += 'Specvizitor'
         self.setWindowTitle(title)
 
-    @Slot(str)
+    @QtCore.Slot(str)
     def _select_by_id(self, obj_id: str):
-        if self.rd.notes.validate_id(obj_id):
+        if self.rd.review.validate_id(obj_id):
             self.setFocus()
-            self.load_object(self.rd.notes.get_id_loc(obj_id))
+            self.load_object(self.rd.review.get_id_loc(obj_id))
 
-    @Slot(int)
+    @QtCore.Slot(int)
     def _select_by_index(self, index: int):
-        if self.rd.notes.validate_index(index):
+        if self.rd.review.validate_index(index):
             self.setFocus()
             self.load_object(index - 1)
 
     def _save_action(self):
         """ Instead of saving inspection results, display a message saying that the auto-save mode is enabled.
         """
         msg = 'The project data is saved automatically'
@@ -397,150 +391,114 @@
 
     def _export_action(self):
         path = qtpy.compat.getsavefilename(self, caption='Export To FITS',
                                            basedir=str(self.rd.output_path.with_suffix('.fits')),
                                            filters='FITS Files (*.fits)')[0]
 
         if path:
-            self.rd.notes.write(self.rd.output_path.with_suffix('.fits'), 'fits')
+            self.rd.review.write(self.rd.output_path.with_suffix('.fits'), 'fits')
 
     def _exit_action(self):
         if self.rd.j is not None:
             self.data_requested.emit()
 
         # save the state and geometry of the main window
         settings = QtCore.QSettings()
         settings.setValue('geometry', self.saveGeometry())
         settings.setValue('windowState', self.saveState())
 
         self.close()
         logger.info("Application closed")
 
-    def _restore_dock_configuration_action(self):
-        path = qtpy.compat.getopenfilename(self, caption='Open Dock Configuration',
+    def _restore_viewer_config_action(self):
+        path = qtpy.compat.getopenfilename(self, caption='Open Viewer Configuration',
                                            filters='YAML Files (*.yml)')[0]
         if path:
-            new_docks = self.rd.docks.replace_params(pathlib.Path(path))
-            if new_docks is None:
-                logger.error('Failed to restore the dock configuration')
+            new_viewer_cfg = self._viewer_cfg.replace_params(pathlib.Path(path))
+            if new_viewer_cfg is None:
+                logger.error('Failed to restore the viewer configuration')
             else:
-                self.rd.docks = new_docks
-                self.rd.docks.save()
+                self._viewer_cfg = new_viewer_cfg
+                self._viewer_cfg.save()
 
-                self.dock_configuration_updated.emit(self.rd.docks)
+                self.viewer_configuration_updated.emit(self._viewer_cfg)
 
                 self.reload()
 
-                logger.info('Dock configuration restored')
+                logger.info('Viewer configuration restored')
 
-    def _backup_dock_configuration_action(self):
-        path = qtpy.compat.getsavefilename(self, caption='Save Dock Configuration',
-                                           basedir=str(pathlib.Path() / 'docks.yml'),
+    def _backup_viewer_config_action(self):
+        path = qtpy.compat.getsavefilename(self, caption='Save Viewer Configuration',
+                                           basedir=str(pathlib.Path() / 'data_widgets.yml'),
                                            filters='YAML Files (*.yml)')[0]
 
         if path:
-            save_yaml(path, asdict(self.rd.docks))
-            logger.info('Dock configuration saved')
+            save_yaml(path, asdict(self._viewer_cfg))
+            logger.info('Viewer configuration saved')
 
     def _enter_fullscreen(self):
         self.was_maximized = True if self.isMaximized() else False
         self.showFullScreen()
 
     def _exit_fullscreen(self):
         self.showNormal()
         if self.was_maximized:
             self.showMaximized()
 
     def _screenshot_action(self):
-        default_filename = f'{self.rd.output_path.stem.replace(" ", "_")}_ID{self.rd.notes.get_id(self.rd.j)}.png'
+        default_filename = f'{self.rd.output_path.stem.replace(" ", "_")}_ID{self.rd.review.get_id(self.rd.j)}.png'
         path, extension = qtpy.compat.getsavefilename(self, caption='Save/Save As',
                                                       basedir=str(pathlib.Path().resolve() / default_filename),
                                                       filters='Images (*.png)')
         if path:
             self.screenshot_path_selected.emit(path)
 
     def _settings_action(self):
-        dialog = Settings(self.rd.config, parent=self)
+        dialog = Settings(self._config, parent=self)
         dialog.appearance_changed.connect(self.update_appearance)
         dialog.catalogue_changed.connect(self.update_catalogue)
         if dialog.exec():
             self.reload()
 
-    @Slot(bool)
+    @QtCore.Slot(bool)
     def update_appearance(self, theme_changed: bool = False):
-        appearance.configure(self.rd.config.appearance)
+        set_up_appearance(self._config.appearance)
         if theme_changed:
             self.theme_changed.emit()
 
-    @Slot(object)
+    @QtCore.Slot(object)
     def update_catalogue(self, cat: Table | None):
-        if cat is None and self.rd.notes is not None:
-            self.rd.cat = create_cat(self.rd.notes.ids)
+        if cat is None and self.rd.review is not None:
+            self.rd.cat = create_cat(self.rd.review.ids)
         else:
             self.rd.cat = cat
         self.catalogue_changed.emit(self.rd.cat)
 
-    @Slot(pathlib.Path)
+    @QtCore.Slot(pathlib.Path)
     def update_output_path(self, path: pathlib.Path):
         self.rd.output_path = path
-        self.rd.cache.last_inspection_file = str(path)
-        self.rd.cache.save()
+        self._cache.last_inspection_file = str(path)
+        self._cache.save()
         self._update_window_title()
 
     def _about_action(self):
         QtWidgets.QMessageBox.about(self, "About Specvizitor", "Specvizitor v{}".format(version('specvizitor')))
 
     def closeEvent(self, _):
         self._exit_action()
 
     @QtCore.Slot(dict)
     def _save_viewer_data(self, layout: dict):
-        self.rd.cache.dock_layout = layout
-        self.rd.cache.save()
+        self._cache.dock_layout = layout
+        self._cache.save()
 
     @QtCore.Slot(list)
     def _save_obj_info_data(self, visible_columns: list[str]):
-        self.rd.cache.visible_columns = visible_columns
-        self.rd.cache.save()
+        self._cache.visible_columns = visible_columns
+        self._cache.save()
 
     @QtCore.Slot(str, dict)
     def _save_review_data(self, comments: str, checkboxes: dict[str, bool]):
-        self.rd.notes.update_value(self.rd.j, 'comment', comments)
+        self.rd.review.update_value(self.rd.j, 'comment', comments)
         for cname, is_checked in checkboxes.items():
-            self.rd.notes.update_value(self.rd.j, cname, is_checked)
+            self.rd.review.update_value(self.rd.j, cname, is_checked)
         self.rd.save()
-
-
-def main():
-    parser = argparse.ArgumentParser()
-    parser.add_argument('--verbose', action='store_true')
-    parser.add_argument('--purge', action='store_true')
-
-    args = parser.parse_args()
-
-    # logging configuration
-    level = logging.INFO if args.verbose else logging.WARNING
-    logging.basicConfig(format='%(asctime)s - %(name)s - %(levelname)s - %(message)s', level=level)
-
-    # initialize the application data
-    appdata = AppData.init_from_disk(purge=args.purge)
-
-    # start the application
-    app = QtWidgets.QApplication(sys.argv)
-    app.setOrganizationName('FRESCO')
-    app.setApplicationName('Specvizitor')
-    logger.info("Application started")
-
-    # pyqtgraph configuration
-    pg.setConfigOption('imageAxisOrder', 'row-major')
-
-    # GUI appearance
-    appearance.configure(cfg=appdata.config.appearance)
-
-    # initialize the main window
-    window = MainWindow(appdata=appdata)
-    window.show()
-    sys.exit(app.exec_())
-
-
-if __name__ == '__main__':
-    main()
```

### Comparing `specvizitor-0.2.1/specvizitor/io/catalogue.py` & `specvizitor-0.3.0/specvizitor/io/catalogue.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/io/inspection_data.py` & `specvizitor-0.3.0/specvizitor/io/inspection_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 @dataclass
 class InspectionData:
     df: pd.DataFrame
     default_columns: list[str] = field(default_factory=lambda: ['starred', 'comment'])
 
     @classmethod
-    def create(cls, ids, flags: list[str] | None):
+    def create(cls, ids, flags: list[str] | None = None):
         """ Create a new instance of the InspectionData class with a Pandas dataframe containing:
               - a column of IDs;
               - a column for comments;
               - one column per each user-defined flag.
         @param ids: the list of IDs
         @param flags: the list of user-defined flags
         @return: an instance of the InspectionData class
@@ -65,18 +65,18 @@
         df = pd.read_csv(filename, index_col='id')
 
         if 'starred' not in df.columns:
             df['starred'] = False
 
         df['comment'] = '' if 'comment' not in df.columns else df['comment'].fillna('')
 
-        notes = cls(df=df)
-        notes.reorder_columns()
+        review = cls(df=df)
+        review.reorder_columns()
 
-        return notes
+        return review
 
     def write(self, filename: pathlib.Path, fmt: str = 'csv'):
         """ Write inspection data to the output file.
         @param filename: the output filename
         @param fmt: the output format
         @return: None
         """
@@ -84,14 +84,15 @@
         writers: dict[str, type[WriterBase]] = {
             'csv': CSVWriter,
             'fits': FITSWriter
         }
 
         if writers.get(fmt):
             writers[fmt]().write(self.df, filename)
+            logger.info(f'Project saved (path: {filename})')
         else:
             logger.error(f"Unknown output format: {fmt}")
 
     @property
     def n_objects(self) -> int | None:
         """
         @return: the total number of objects under inspection.
@@ -138,34 +139,14 @@
 
     def get_id_loc(self, obj_id: str):
         if self.ids_are_int:
             obj_id = int(obj_id)
 
         return self.df.index.get_loc(obj_id)
 
-    def get_checkboxes(self, default_checkboxes: dict[str, str] | None = None) -> dict[str, str]:
-        """ Get the full description of checkboxes to be displayed in the review form (column name + label). By default,
-        each checkbox is automatically assigned a label by a simple capitalization of the column name, e.g. a flag named
-        `extended` would become a checkbox with a label `Extended`. The `default_checkboxes` parameter is used as a
-        lookup table to overrides these labels.
-        @param default_checkboxes: the description of default checkboxes used to override automatically created labels
-        @return: a dictionary describing the checkboxes to be displayed in the review form
-        """
-
-        checkboxes = {}
-
-        for cname in self.flag_columns:
-            checkboxes[cname] = cname.capitalize()
-
-        if default_checkboxes is not None:
-            checkboxes.update({key: value for key, value in default_checkboxes.items()
-                               if key in self.user_defined_columns})
-
-        return checkboxes
-
     def update_value(self, j: int, cname: str, value):
         self.df.iat[j, self.df.columns.get_loc(cname)] = value
 
     def validate_id(self, obj_id: str | int) -> bool:
         if self.ids_are_int:
             try:
                 obj_id = int(obj_id)
```

### Comparing `specvizitor-0.2.1/specvizitor/io/viewer_data.py` & `specvizitor-0.3.0/specvizitor/io/viewer_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,26 +31,37 @@
         logger.error(f'{type(self).__name__}: {e}')
 
 
 @dataclass
 class GenericFITSLoader(BaseLoader):
     name: str = 'generic_fits'
 
-    def load(self, filename: pathlib.Path, extname: str = None, extver: str = None, **kwargs):
+    def load(self, filename: pathlib.Path, extname: str = None, extver: str = None, extver_index: int = None, **kwargs):
 
         try:
             hdul = fits.open(filename, **kwargs)
         except Exception as e:
             self.raise_error(e)
             return None, None
 
-        if extname is not None and extver is None:
-            index = extname
-        elif extname is not None and extver is not None:
+        if extname is not None and extver is not None:
             index = (extname, extver)
+        elif extname is not None and extver_index is not None:
+            extname_matching_mask = ['EXTNAME' in hdu.header and hdu.header['EXTNAME'] == extname for hdu in hdul]
+            index = 0
+            counter = -1
+            while counter != extver_index:
+                index += 1
+                if index >= len(extname_matching_mask):
+                    self.raise_error(f'EXTVER `{extver_index}` out of range (filename: {filename.name})')
+                    return None, None
+                if extname_matching_mask[index]:
+                    counter += 1
+        elif extname is not None:
+            index = extname
         else:
             index = 1
 
         try:
             hdu = hdul[index]
         except KeyError:
             self.raise_error(f'Extension `{index}` not found (filename: {filename.name})')
@@ -107,14 +118,19 @@
             self.raise_error(f'Invalid spectral axis unit: {spec.spectral_axis.unit}')
             return None, None
 
         return spec, spec.meta
 
 
 def load(loader_name: str | None, filename: pathlib.Path, widget_name: str, **kwargs):
+    if kwargs.get('silent'):
+        logger.disabled = True
+    else:
+        logger.disabled = False
+
     registered_loaders: dict[str, BaseLoader] =\
         {loader.name: loader for loader in (GenericFITSLoader(), PILLoader(), SpecutilsLoader())}
 
     allowed_loader_names = ('auto',) + tuple(loader.name for loader in registered_loaders.values())
     if loader_name not in allowed_loader_names:
         logger.error(f'Unknown loader type: `{loader_name}` (widget: {widget_name}).'
                      f'Available loaders: {allowed_loader_names}')
```

### Comparing `specvizitor-0.2.1/specvizitor/menu/NewFile.py` & `specvizitor-0.3.0/specvizitor/widgets/NewFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import logging
 import pathlib
 
 from ..config import config
 from ..io.catalogue import read_cat, create_cat, cat_browser
 from ..io.viewer_data import get_ids_from_dir, data_browser
 from ..utils.logs import qlog
-from ..widgets.FileBrowser import FileBrowser
+
+from .FileBrowser import FileBrowser
 
 logger = logging.getLogger(__name__)
 
 
 class NewFile(QtWidgets.QDialog):
     output_path_selected = QtCore.Signal(pathlib.Path)
     catalogue_changed = QtCore.Signal(object)
```

### Comparing `specvizitor-0.2.1/specvizitor/menu/Settings.py` & `specvizitor-0.3.0/specvizitor/widgets/Settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from platformdirs import user_config_dir
-from qtpy import QtWidgets, QtCore
+from qtpy import QtWidgets, QtCore, QtGui
 
 from abc import abstractmethod
 import logging
 
 from ..config import config
 from ..io.catalogue import read_cat, cat_browser
 from ..io.viewer_data import data_browser
 from ..utils.logs import qlog
 
-from ..widgets.AbstractWidget import AbstractWidget
-from ..widgets.Section import Section
-from ..widgets.FileBrowser import FileBrowser
+from .AbstractWidget import AbstractWidget
+from .FileBrowser import FileBrowser
+from .Section import Section
 
 logger = logging.getLogger(__name__)
 
 
 class SettingsWidget(AbstractWidget):
     SPACING = 20
 
@@ -204,14 +204,15 @@
     def init_ui(self):
         self._tab_widget = QtWidgets.QTabWidget(self)
 
         self.create_tabs()
         self.add_tabs()
 
         self._info_label = QtWidgets.QLabel(f"Advanced settings: {user_config_dir('specvizitor')}", self)
+        self._info_label.setTextInteractionFlags(QtCore.Qt.TextSelectableByMouse)
 
         # add OK/Cancel buttons
         self._button_box = QtWidgets.QDialogButtonBox(
             QtWidgets.QDialogButtonBox.Ok | QtWidgets.QDialogButtonBox.Cancel, self)
 
         self._button_box.accepted.connect(self.accept)
         self._button_box.rejected.connect(self.reject)
```

### Comparing `specvizitor-0.2.1/specvizitor/utils/logs.py` & `specvizitor-0.3.0/specvizitor/utils/logs.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/utils/params.py` & `specvizitor-0.3.0/specvizitor/utils/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import dacite
 from dacite.exceptions import WrongTypeError, MissingValueError
 from dictdiffer import diff, patch, swap
 
-from dataclasses import dataclass, asdict
+from dataclasses import asdict, dataclass, field
 from functools import wraps
 import logging
 import pathlib
 import shutil
 import yaml
 
 logger = logging.getLogger(__name__)
@@ -69,15 +69,15 @@
     @classmethod
     def _read(cls, filename: pathlib.Path):
         params_dict = read_yaml(filename)
         return dacite.from_dict(data_class=cls, data=params_dict, config=dacite.Config(strict=True))
 
     @classmethod
     def read_default_params(cls, filename: str):
-        return cls._read(pathlib.Path(__file__).parent.parent / 'data' / filename)
+        return cls._read(pathlib.Path(__file__).parent.parent / 'data' / 'presets' / filename)
 
     @classmethod
     def read_user_params(cls, file: LocalFile, default: str | None = None):
         if default is None:
             params = dacite.from_dict(data_class=cls, data={})
         else:
             params = cls.read_default_params(default)
```

### Comparing `specvizitor-0.2.1/specvizitor/utils/table_tools.py` & `specvizitor-0.3.0/specvizitor/utils/table_tools.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/widgets/AbstractWidget.py` & `specvizitor-0.3.0/specvizitor/widgets/AbstractWidget.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/widgets/DataViewer.py` & `specvizitor-0.3.0/specvizitor/widgets/DataViewer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 from astropy.table import Table
 from pyqtgraph.dockarea.Dock import Dock
 from pyqtgraph.dockarea.DockArea import DockArea
 from qtpy import QtWidgets, QtCore
 
+import logging
+
 from ..config import config
-from ..config.docks import Docks
+from ..config.data_widgets import DataWidgets
 from ..config.spectral_lines import SpectralLines
 from ..io.inspection_data import InspectionData
 from ..plugins.plugin_core import PluginCore
 
 from .AbstractWidget import AbstractWidget
 from .LazyViewerElement import LazyViewerElement
 from .ViewerElement import ViewerElement
 from .Image2D import Image2D
 from .Plot1D import Plot1D
 from .Spec1D import Spec1D
 
+logger = logging.getLogger(__name__)
+
 
 class DataViewer(AbstractWidget):
     object_selected = QtCore.Signal(int, InspectionData, Table, config.Data)
     view_reset = QtCore.Signal()
     data_collected = QtCore.Signal(dict)
 
     def __init__(self,
-                 dock_cfg: Docks,
+                 viewer_cfg: DataWidgets,
                  appearance: config.Appearance,
-                 spectral_lines: SpectralLines = None,
+                 spectral_lines: SpectralLines | None = None,
                  plugins: list[PluginCore] | None = None,
                  parent=None):
 
-        self.appearance = appearance
-        self.dock_cfg = dock_cfg
-        self.spectral_lines = spectral_lines
+        self._appearance = appearance
+        self._viewer_cfg = viewer_cfg
+        self._spectral_lines = spectral_lines
         self._plugins: list[PluginCore] = plugins if plugins is not None else []
 
         self.dock_area = DockArea()
         self.added_docks: list[str] = []
 
         self.core_widgets: dict[str, ViewerElement] = {}
         self.docks: dict[str, Dock] = {}
@@ -69,33 +73,36 @@
             for w in self.widgets:
                 w.graphics_layout.clear()
                 w.deleteLater()
 
         widgets = {}
 
         # create widgets for images (e.g. image cutouts, 2D spectra)
-        if self.dock_cfg.images is not None:
-            for name, image_cfg in self.dock_cfg.images.items():
-                widgets[name] = Image2D(cfg=image_cfg, title=name, appearance=self.appearance, parent=self)
+        if self._viewer_cfg.images is not None:
+            for name, image_cfg in self._viewer_cfg.images.items():
+                widgets[name] = Image2D(cfg=image_cfg, title=name, appearance=self._appearance, parent=self)
 
         # create widgets for plots (does not include any spectra!)
-        if self.dock_cfg.plots is not None:
-            for name, plot_cfg in self.dock_cfg.plots.items():
-                widgets[name] = Plot1D(cfg=plot_cfg, title=name, appearance=self.appearance, parent=self)
+        if self._viewer_cfg.plots is not None:
+            for name, plot_cfg in self._viewer_cfg.plots.items():
+                widgets[name] = Plot1D(cfg=plot_cfg, title=name, appearance=self._appearance, parent=self)
 
         # create widgets for 1D spectra
-        if self.dock_cfg.spectra is not None:
-            for name, spec_cfg in self.dock_cfg.spectra.items():
-                widgets[name] = Spec1D(lines=self.spectral_lines, cfg=spec_cfg, title=name,
-                                       appearance=self.appearance, parent=self)
+        if self._viewer_cfg.spectra is not None:
+            for name, spec_cfg in self._viewer_cfg.spectra.items():
+                widgets[name] = Spec1D(lines=self._spectral_lines, cfg=spec_cfg, title=name,
+                                       appearance=self._appearance, parent=self)
 
         for w in widgets.values():
             self.object_selected.connect(w.load_object)
         self.core_widgets = widgets
 
+        for plugin in self._plugins:
+            plugin.overwrite_widget_configs(self.core_widgets)
+
     def _create_docks(self):
         # delete previously added docks
         for dock_name in self.added_docks:
             self.docks[dock_name].close()
 
         docks = {}
         for widget in self.widgets:
@@ -115,45 +122,51 @@
         self.added_docks = []
 
         for widget in self.widgets:
             if widget.cfg.visible:
                 self._add_dock(widget)
                 self.added_docks.append(widget.title)
 
+        for plugin in self._plugins:
+            plugin.tweak_docks(self.docks)
+
     @QtCore.Slot()
-    def reset_dock_layout(self):
+    def init_docks(self):
         self._create_docks()
         self._add_docks()
         self._update_dock_titles()
 
     @QtCore.Slot(dict)
     def restore_dock_layout(self, layout: dict):
         try:
             # set `extra` to None to catch an exception (KeyError) when adding extra docks not mentioned in `layout`
             self.dock_area.restoreState(layout, missing='ignore', extra=None)
+            logger.info('Dock layout restored')
+
+            for plugin in self._plugins:
+                plugin.tweak_docks(self.docks)
+
         except (KeyError, ValueError, TypeError):
-            self.reset_dock_layout()
+            self.init_docks()  # to reset the dock layout
+            logger.error('Failed to restore the dock layout')
 
     def init_ui(self):
         self._create_widgets()
-        self._create_docks()
-        self._add_docks()
-
-        self.reset_dock_layout()
+        self.init_docks()
 
     def set_layout(self):
         self.setLayout(QtWidgets.QGridLayout())
         self.set_geometry(spacing=0, margins=0)
 
     def populate(self):
         self.layout().addWidget(self.dock_area, 1, 1, 1, 1)
 
-    @QtCore.Slot(Docks)
-    def update_dock_configuration(self, dock_cfg: Docks):
-        self.dock_cfg = dock_cfg
+    @QtCore.Slot(DataWidgets)
+    def update_viewer_configuration(self, viewer_cfg: DataWidgets):
+        self._viewer_cfg = viewer_cfg
         self.init_ui()
 
     @QtCore.Slot()
     def load_project(self):
         self.setEnabled(True)
 
     @QtCore.Slot(int, InspectionData, Table, config.Data)
@@ -166,28 +179,45 @@
             self.view_reset.disconnect()
         except TypeError:
             pass
         for w in self.core_widgets.values():
             if w.data is not None:
                 self.view_reset.connect(w.reset_view)
 
-        for plugin in self._plugins:
-            plugin.invoke(self.active_core_widgets)
-
-        # update the dock titles
         self._update_dock_titles()
 
+        for plugin in self._plugins:
+            plugin.tweak_widgets(self.active_core_widgets)
+
     @QtCore.Slot()
     def collect(self):
         self.data_collected.emit(self.dock_area.saveState())
 
     @QtCore.Slot(str)
     def take_screenshot(self, filename: str):
         self.grab().save(filename)
 
     def _update_dock_titles(self):
         for core_widget in self.core_widgets.values():
-            for w in (core_widget,) + tuple(core_widget.lazy_widgets):
-                if core_widget.filename is not None and core_widget.data is not None:
-                    self.docks[w.title].setTitle(core_widget.filename.name)
-                else:
+            if core_widget.filename is not None and core_widget.data is not None:
+                title = core_widget.filename.name
+
+                # adding EXTNAME and EXTVER to the dock title
+                fits_meta = core_widget.meta.get('EXTNAME'), core_widget.meta.get('EXTVER')
+                j = 0
+                while j < len(fits_meta) and fits_meta[j] is not None:
+                    j += 1
+                title_extra = ', '.join(fits_meta[:j])
+
+                if title_extra:
+                    if core_widget.cfg.dock_title_fmt == 'short':
+                        title = fits_meta[j - 1]
+                    else:
+                        title += f' [{title_extra}]'
+
+                for w in (core_widget,) + tuple(core_widget.lazy_widgets):
+                    self.docks[w.title].setTitle(title)
+
+            else:
+                for w in (core_widget,) + tuple(core_widget.lazy_widgets):
                     self.docks[w.title].setTitle(w.title)
+
```

### Comparing `specvizitor-0.2.1/specvizitor/widgets/FileBrowser.py` & `specvizitor-0.3.0/specvizitor/widgets/FileBrowser.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/widgets/LazyViewerElement.py` & `specvizitor-0.3.0/specvizitor/widgets/LazyViewerElement.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pyqtgraph as pg
 from qtpy import QtWidgets
 
-from ..config import docks, config
+from ..config import data_widgets, config
 from .AbstractWidget import AbstractWidget
 
 
 class LazyViewerElement(AbstractWidget):
-    def __init__(self, title: str, cfg: docks.LazyViewerElement, appearance: config.Appearance, parent=None):
+    def __init__(self, title: str, cfg: data_widgets.LazyViewerElement, appearance: config.Appearance, parent=None):
         self.title = title
         self.cfg = cfg
         self.appearance = appearance
 
         self.graphics_view: pg.GraphicsView | None = None
         self.graphics_layout: pg.GraphicsLayout | None = None
 
@@ -32,15 +32,7 @@
 
     def set_layout(self):
         self.setLayout(QtWidgets.QGridLayout())
         self.set_geometry(spacing=self.appearance.viewer_spacing, margins=self.appearance.viewer_margins)
 
     def populate(self):
         self.layout().addWidget(self.graphics_view, 1, 1, 1, 1)
-
-    def register_item(self, item: pg.GraphicsItem):
-        self._added_items.append(item)
-
-    def remove_registered_items(self):
-        for item in self._added_items:
-            self.container.removeItem(item)
-        self._added_items = []
```

### Comparing `specvizitor-0.2.1/specvizitor/widgets/ObjectInfo.py` & `specvizitor-0.3.0/specvizitor/widgets/ObjectInfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,25 +109,25 @@
         self.layout().addLayout(sub_layout)
 
     @QtCore.Slot()
     def load_project(self):
         self.setEnabled(True)
 
     @QtCore.Slot(int, InspectionData, Table)
-    def load_object(self, j: int, notes: InspectionData, cat: Table):
+    def load_object(self, j: int, review: InspectionData, cat: Table):
         try:
-            cat.loc[notes.get_id(j)]
+            cat.loc[review.get_id(j)]
         except KeyError:
-            logger.warning('Object not found in the catalogue (ID: {})'.format(notes.get_id(j)))
+            logger.warning('Object not found in the catalogue (ID: {})'.format(review.get_id(j)))
             return
 
         for row in self._table_items:
             cname = row[0].text()
             try:
-                row[1].setText(str(cat.loc[notes.get_id(j)][cname]))
+                row[1].setText(str(cat.loc[review.get_id(j)][cname]))
             except KeyError:
                 logger.warning(column_not_found_message(cname, cat.meta.get('aliases')))
                 row[1].setText('')
 
         # if 'ra' in self._cat.colnames and 'dec' in self._cat.colnames:
         #     c = SkyCoord(ra=self._cat['ra'][self._j], dec=self._cat['dec'][self._j], frame='icrs', unit='deg')
         #     ra, dec = c.to_string('hmsdms').split(' ')
```

### Comparing `specvizitor-0.2.1/specvizitor/widgets/Plot1D.py` & `specvizitor-0.3.0/specvizitor/widgets/Plot1D.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pyqtgraph as pg
 from scipy.ndimage import gaussian_filter1d
 from qtpy import QtCore
 
 from dataclasses import dataclass, field
 import logging
 
-from ..config import config, docks
+from ..config import config, data_widgets
 from ..utils.table_tools import column_not_found_message
 from .ViewerElement import ViewerElement
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
@@ -30,25 +30,25 @@
         if np.isnan(data).all():
             return 0, 1
         else:
             return np.nanmin(data), np.nanmax(data)
 
     def freeze(self, limits: tuple[float | None, float | None]) -> None:
         """
-        Override axis limits and prevent their modification in the future (e.g. after smoothing of axis data).
+        overwrite axis limits and prevent their modification in the future (e.g. after smoothing of axis data).
         @param limits: new axis limits; if a new limit value is None, leave the limit editable
         """
         self.values = (limits[0] if limits[0] else self.values[0],
                        limits[1] if limits[1] else self.values[1])
 
         self.editable = (limits[0] is None, limits[1] is None)
 
     def update(self, limits: tuple[float, float]) -> None:
         """
-        Override editable axis limits.
+        overwrite editable axis limits.
         @param limits: new axis limits
         """
         self.values = (limits[0] if self.editable[0] else self.values[0],
                        limits[1] if self.editable[1] else self.values[1])
 
 
 @dataclass
@@ -68,16 +68,16 @@
         self.value = value
         self.default_lims = DefaultAxisLimits.init_from_arr(self.value)
 
     @property
     def label(self):
         label = self.name
         if self.unit is not None:
-            # TODO: convert to inline unicode after next astropy release
-            label += f' [{self.unit}]'.replace('Angstrom', 'Å')
+            unit_repr = self.unit.to_string('unicode')
+            label += f' [{unit_repr}]'
         return label
 
     def scale(self, scaling_factor: float):
         self.set_value(self.value * scaling_factor)
         if self.unc is not None:
             self.unc = self.unc * scaling_factor
 
@@ -134,23 +134,23 @@
         unc = self.unc.copy()
 
         unc[np.isnan(unc)] = 1E10  # NaNs have to be replaced before applying a gaussian filter
         flux[(gaussian_filter1d(unc, 3) > cutoff)] = np.nan
 
         self.set_value(flux)
 
-    def apply_settings(self, cfg: docks.Axis):
+    def apply_settings(self, cfg: data_widgets.Axis):
         # apply unit transformation
         if cfg.unit is not None:
             self.convert_units(cfg.unit)
 
         # scale axis
         self.apply_scale(cfg.scale)
 
-        # override default limits
+        # overwrite default limits
         self.default_lims.freeze((cfg.limits.min, cfg.limits.max))
 
 
 @dataclass
 class PlotData:
     x: AxisData
     y: AxisData
@@ -168,15 +168,15 @@
 
         self._y_plot: pg.PlotDataItem | None = None
         self._y_unc_plot: pg.PlotDataItem | None = None
 
     def set_plot_data(self, data: PlotData):
         self.data = data
 
-    def update_labels(self, x_label: docks.Label, y_label: docks.Label):
+    def update_labels(self, x_label: data_widgets.Label, y_label: data_widgets.Label):
         self.setLabel('bottom' if x_label.position is None else x_label.position, self.data.x.label)
         self.setLabel('left' if y_label.position is None else y_label.position, self.data.y.label)
 
     def add_items(self):
         self._y_plot = self.plot(pen='k' if self.appearance.theme == 'light' else 'w')
         self._y_unc_plot = self.plot(pen='r')
 
@@ -205,17 +205,17 @@
         self.data.y.default_lims.update(DefaultAxisLimits.get_limits_from_arr(y_smoothed))
         self._y_plot.setData(self.data.x.value, y_smoothed)
 
 
 class Plot1D(ViewerElement):
     plot_data_loaded = QtCore.Signal(object)
     plot_refreshed = QtCore.Signal()
-    labels_updated = QtCore.Signal(docks.Label, docks.Label)
+    labels_updated = QtCore.Signal(data_widgets.Label, data_widgets.Label)
 
-    def __init__(self, cfg: docks.Plot1D, **kwargs):
+    def __init__(self, cfg: data_widgets.Plot1D, **kwargs):
         self.cfg = cfg
         self.allowed_data_types = (Table,)
 
         self.plot_item: Plot1DItem | None = None
         self.plot_data: PlotData | None = None
 
         super().__init__(cfg=cfg, **kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `specvizitor-0.2.1/specvizitor/widgets/QuickSearch.py` & `specvizitor-0.3.0/specvizitor/widgets/QuickSearch.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/widgets/ReviewForm.py` & `specvizitor-0.3.0/specvizitor/widgets/ReviewForm.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,30 +16,33 @@
         self._checkbox_widgets: dict[str, QtWidgets.QCheckBox] | None = None
         self._comments_widget: QtWidgets.QTextEdit | None = None
 
         super().__init__(parent=parent)
         self.setEnabled(False)
         self.setSizePolicy(QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.Preferred)
 
-    def create_checkbox_widgets(self, notes: InspectionData | None = None):
+    def create_checkbox_widgets(self, review: InspectionData | None = None):
         if self._checkbox_widgets is not None:
             for w in self._checkbox_widgets.values():
                 w.deleteLater()
 
-        if notes is None:
-            checkboxes = self.cfg.default_checkboxes
+        if review is None:
+            flags = self.cfg.default_flags
         else:
-            checkboxes = notes.get_checkboxes(self.cfg.default_checkboxes)
-
-        if checkboxes is None:
-            return {}
+            flags = review.flag_columns
 
         checkbox_widgets = {}
-        for i, (cname, label) in enumerate(checkboxes.items()):
-            checkbox_widgets[cname] = QtWidgets.QCheckBox(label, self)
+        if flags is not None:
+            for i, flag_name in enumerate(flags):
+                # TODO: overwrite the keyPressEvent method of QtWidgets.QCheckBox to add shortcuts
+                checkbox_widget = QtWidgets.QCheckBox(flag_name, self)
+                checkbox_widgets[flag_name] = checkbox_widget
+                
+                if i < 9:
+                    checkbox_widget.setShortcut(str(i + 1))
 
         self._checkbox_widgets = checkbox_widgets
 
     def init_ui(self):
         self.create_checkbox_widgets()
         self._comments_widget = QtWidgets.QTextEdit(self)
 
@@ -50,25 +53,25 @@
         for i, widget in enumerate(self._checkbox_widgets.values()):
             self.layout().addWidget(widget, i + 1, 1, 1, 1)
 
         self.layout().addWidget(QtWidgets.QLabel('Comments:', self), len(self._checkbox_widgets) + 1, 1, 1, 1)
         self.layout().addWidget(self._comments_widget, len(self._checkbox_widgets) + 2, 1, 1, 1)
 
     @QtCore.Slot(InspectionData)
-    def load_project(self, notes: InspectionData):
+    def load_project(self, review: InspectionData):
         self.setEnabled(True)
 
-        self.create_checkbox_widgets(notes=notes)
+        self.create_checkbox_widgets(review=review)
         self.repopulate()
 
     @QtCore.Slot(int, InspectionData)
-    def load_object(self, j: int, notes: InspectionData):
-        self._comments_widget.setText(notes.get_value(j, 'comment'))
+    def load_object(self, j: int, review: InspectionData):
+        self._comments_widget.setText(review.get_value(j, 'comment'))
         for cname, widget in self._checkbox_widgets.items():
-            widget.setChecked(notes.get_value(j, cname))
+            widget.setChecked(review.get_value(j, cname))
 
     @QtCore.Slot()
     def collect(self):
         comment = self._comments_widget.toPlainText()
         checkboxes = {cname: widget.isChecked() for cname, widget in self._checkbox_widgets.items()}
 
         self.data_collected.emit(comment, checkboxes)
```

### Comparing `specvizitor-0.2.1/specvizitor/widgets/Section.py` & `specvizitor-0.3.0/specvizitor/widgets/Section.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/widgets/SmartSlider.py` & `specvizitor-0.3.0/specvizitor/widgets/SmartSlider.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/widgets/Spec1D.py` & `specvizitor-0.3.0/specvizitor/widgets/Spec1D.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from qtpy import QtCore
 from specutils import Spectrum1D
 
 from dataclasses import asdict
 from functools import partial
 import logging
 
-from ..config import docks
+from ..config import data_widgets
 from ..config.spectral_lines import SpectralLines
 
 from .LazyViewerElement import LazyViewerElement
 from .Plot1D import AxisData, PlotData, Plot1D, Plot1DItem
 from .SmartSlider import SmartSliderWithEditor
 
 logger = logging.getLogger(__name__)
@@ -30,15 +30,15 @@
         self.window = window
 
         # set up the spectral lines
         self._line_artists = {}
         # TODO: store colors in config
         line_color = (175.68072, 220.68924, 46.59488)
         line_pen = pg.mkPen(color=line_color, width=1)
-        for line_name, lambda0 in self.lines.list.items():
+        for line_name, lambda0 in self.lines.wavelengths.items():
             line = pg.InfiniteLine(pen=line_pen)
             label = pg.TextItem(text=line_name, color=line_color, anchor=(1, 1), angle=-90)
             self._line_artists[line_name] = {'line': line, 'label': label}
 
     def add_items(self):
         for line_name, line_artist in self._line_artists.items():
             self.addItem(line_artist['line'], ignoreBounds=True)
@@ -56,30 +56,30 @@
         return y_min + 0.6 * (y_max - y_min)
 
     def set_line_positions(self, redshift: float = 0):
         scale0 = 1 + redshift
         label_height = self.get_line_label_height()
 
         for line_name, line_artist in self._line_artists.items():
-            line_wave = (self.lines.list[line_name] * u.Unit(self.lines.wave_unit)).to(self.data.x.unit)
+            line_wave = (self.lines.wavelengths[line_name] * u.Unit(self.lines.wave_unit)).to(self.data.x.unit)
             line_wave = line_wave.value * scale0
             line_artist['line'].setPos(line_wave)
             line_artist['label'].setPos(QtCore.QPointF(line_wave, label_height))
 
         if self.window is not None:
             self.fit_in_window((scale0 * (self.window[0] + self.window[1]) / 2 - (self.window[1] - self.window[0]) / 2,
                                 scale0 * (self.window[0] + self.window[1]) / 2 + (self.window[1] - self.window[0]) / 2))
 
     def reset_x_range(self):
         if self.window is None:
             super().reset_x_range()
 
 
 class Spec1DRegion(LazyViewerElement):
-    def __init__(self, title: str, line: tuple[str, u.Quantity], cfg: docks.SpectrumRegion, **kwargs):
+    def __init__(self, title: str, line: tuple[str, u.Quantity], cfg: data_widgets.SpectrumRegion, **kwargs):
 
         self.cfg = cfg
         self.line = line
 
         window_center = line[1]
         window_size = u.Quantity(self.cfg.window_size)
         self.window = (window_center - window_size / 2, window_center + window_size / 2)
@@ -87,26 +87,26 @@
         self.spec_1d: Spec1DItem | None = None
 
         super().__init__(title=title, cfg=cfg, **kwargs)
 
     def init_ui(self):
         super().init_ui()
 
-        lines = SpectralLines(wave_unit=self.line[1].unit, list={self.line[0]: self.line[1].value})
+        lines = SpectralLines(wave_unit=self.line[1].unit, wavelengths={self.line[0]: self.line[1].value})
         self.spec_1d = Spec1DItem(lines=lines, window=self.window, name=self.title, appearance=self.appearance)
 
     def populate(self):
         super().populate()
         self.graphics_layout.addItem(self.spec_1d)
 
 
 class Spec1D(Plot1D):
     redshift_changed = QtCore.Signal(float)
 
-    def __init__(self, cfg: docks.Spectrum, lines: SpectralLines | None = None, **kwargs):
+    def __init__(self, cfg: data_widgets.Spectrum, lines: SpectralLines | None = None, **kwargs):
         self.lines = lines
         self.cfg = cfg
         self.allowed_data_types = (Spectrum1D, Table)
 
         self.plot_item: Spec1DItem | None = None
         self.z_slider: SmartSliderWithEditor | None = None
 
@@ -122,17 +122,17 @@
         if self.lines is None or self.cfg.tracked_lines is None:
             return
 
         region_widgets = []
         region_items = []
 
         for line, line_cfg in self.cfg.tracked_lines.items():
-            if line in self.lines.list.keys():
-                spec_region = Spec1DRegion(title=f"{self.title} [{line}]",
-                                           line=(line, self.lines.list[line] * u.Unit(self.lines.wave_unit)),
+            if line in self.lines.wavelengths.keys():
+                spec_region = Spec1DRegion(title=f"{self.title} - {line}",
+                                           line=(line, self.lines.wavelengths[line] * u.Unit(self.lines.wave_unit)),
                                            cfg=line_cfg, appearance=self.appearance,
                                            parent=self.parent())
 
                 region_widgets.append(spec_region)
 
                 lr = pg.LinearRegionItem()
                 region_items.append(lr)
```

### Comparing `specvizitor-0.2.1/specvizitor/widgets/TableColumns.py` & `specvizitor-0.3.0/specvizitor/widgets/TableColumns.py`

 * *Files identical despite different names*

### Comparing `specvizitor-0.2.1/specvizitor/widgets/ToolBar.py` & `specvizitor-0.3.0/specvizitor/widgets/ToolBar.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,22 +70,24 @@
 
     def init_ui(self):
         # create buttons for switching to the next or previous object
         self._pn_buttons = self.create_pn_buttons()
 
         # create a `star` button
         self._star_button = QtWidgets.QAction(self)
+        self._star_button.setShortcut('S')
         self._star_button.setToolTip('Star the object')
 
         # create a `screenshot` button
         self._screenshot_button = QtWidgets.QAction(self)
         self._screenshot_button.setToolTip('Take a screenshot')
 
         # create a `reset view` button
         self._reset_view_button = QtWidgets.QAction(self)
+        self._reset_view_button.setShortcut('R')
         self._reset_view_button.setToolTip('Reset the view')
 
         # create a `reset layout` button
         self._reset_layout_button = QtWidgets.QAction(self)
         self._reset_layout_button.setToolTip('Reset the layout')
 
         for b in self.viewer_connected_buttons:
@@ -97,15 +99,15 @@
         self._settings_button = QtWidgets.QAction(self)
         self._settings_button.setToolTip('GUI and Project Settings')
 
         self.set_icons()
 
         # connect button signals to slots
         for pn_text, b in self._pn_buttons.items():
-            b.triggered.connect(partial(self.previous_next_object, pn_text.split(' ')[0], 'starred' in pn_text))
+            b.triggered.connect(partial(self.change_object, pn_text.split(' ')[0], 'starred' in pn_text))
 
         self._star_button.triggered.connect(self.star)
         self._reset_view_button.triggered.connect(self.reset_view_button_clicked.emit)
         self._reset_layout_button.triggered.connect(self.reset_layout_button_clicked.emit)
         self._screenshot_button.triggered.connect(self.screenshot_button_clicked.emit)
         self._settings_button.triggered.connect(self.settings_button_clicked)
 
@@ -134,27 +136,27 @@
 
     @QtCore.Slot()
     def load_project(self):
         for b in self.viewer_connected_buttons:
             b.setEnabled(True)
 
     @QtCore.Slot(int, InspectionData)
-    def load_object(self, j: int, notes: InspectionData):
-        self._star_button.setIcon(self.get_icon(self.get_star_icon_name(notes.get_value(j, 'starred'))))
+    def load_object(self, j: int, review: InspectionData):
+        self._star_button.setIcon(self.get_icon(self.get_star_icon_name(review.get_value(j, 'starred'))))
 
-        self._pn_buttons['previous starred'].setEnabled(notes.has_starred)
-        self._pn_buttons['next starred'].setEnabled(notes.has_starred)
+        self._pn_buttons['previous starred'].setEnabled(review.has_starred)
+        self._pn_buttons['next starred'].setEnabled(review.has_starred)
 
-    def previous_next_object(self, command: str, starred: bool):
-        j_upd = self.update_index(self.rd.j, self.rd.notes.n_objects, command)
+    def change_object(self, command: str, starred: bool):
+        j_upd = self.update_index(self.rd.j, self.rd.review.n_objects, command)
 
         if starred:
-            if self.rd.notes.has_starred:
-                while not self.rd.notes.get_value(j_upd, 'starred'):
-                    j_upd = self.update_index(j_upd, self.rd.notes.n_objects, command)
+            if self.rd.review.has_starred:
+                while not self.rd.review.get_value(j_upd, 'starred'):
+                    j_upd = self.update_index(j_upd, self.rd.review.n_objects, command)
             else:
                 return
 
         self.object_selected.emit(j_upd)
 
     @staticmethod
     def update_index(current_index, n_objects, command: str):
@@ -182,14 +184,14 @@
         icon_name = 'star.svg' if starred else 'star-empty.svg'
         return icon_name
 
     def get_icon(self, icon_name):
         return QtGui.QIcon(str(self.get_icon_abs_path(icon_name)))
 
     def star(self):
-        starred = not self.rd.notes.get_value(self.rd.j, 'starred')
+        starred = not self.rd.review.get_value(self.rd.j, 'starred')
 
-        self.rd.notes.update_value(self.rd.j, 'starred', starred)
+        self.rd.review.update_value(self.rd.j, 'starred', starred)
         self._star_button.setIcon(self.get_icon(self.get_star_icon_name(starred)))
 
-        self._pn_buttons['previous starred'].setEnabled(self.rd.notes.has_starred)
-        self._pn_buttons['next starred'].setEnabled(self.rd.notes.has_starred)
+        self._pn_buttons['previous starred'].setEnabled(self.rd.review.has_starred)
+        self._pn_buttons['next starred'].setEnabled(self.rd.review.has_starred)
```

### Comparing `specvizitor-0.2.1/specvizitor/widgets/ViewerElement.py` & `specvizitor-0.3.0/specvizitor/widgets/ViewerElement.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from qtpy import QtWidgets, QtCore
 
 import abc
 from dataclasses import asdict
 import logging
 import pathlib
 
-from ..config import config, docks
+from ..config import config, data_widgets
 from ..io.inspection_data import InspectionData
 from ..io.viewer_data import get_filename, load
 
 from .LazyViewerElement import LazyViewerElement
 from .SmartSlider import SmartSliderWithEditor
 
 logger = logging.getLogger(__name__)
@@ -19,15 +19,15 @@
 
 class ViewerElement(LazyViewerElement, abc.ABC):
     content_added = QtCore.Signal()
     view_reset = QtCore.Signal()
     content_cleared = QtCore.Signal()
     smoothing_applied = QtCore.Signal(float)
 
-    def __init__(self, cfg: docks.ViewerElement, **kwargs):
+    def __init__(self, cfg: data_widgets.ViewerElement, **kwargs):
         self.cfg = cfg
 
         self.filename: pathlib.Path | None = None
         self.data = None
         self.meta: dict | Header | None = None
         self.allowed_data_types: tuple | None = None
 
@@ -63,58 +63,56 @@
         # add horizontal sliders
         for s in self.sliders:
             if s.show_text_editor:
                 sub_layout.addWidget(s)
         self.layout().addLayout(sub_layout, 2, 1, 1, 1)
 
     @QtCore.Slot(int, InspectionData, Table, config.Data)
-    def load_object(self, j: int, notes: InspectionData, cat: Table, data_cfg: config.Data):
+    def load_object(self, j: int, review: InspectionData, cat: Table, data_cfg: config.Data):
         # clear the widget content
         if self.data is not None:
             self.clear_content()
-            self.remove_registered_items()
-
             for s in self.sliders:
                 s.clear()
 
         # load catalogue values to the sliders
         for s in self.sliders:
             if s.name_in_catalogue is not None:
-                s.update_default_value(cat, notes.get_id(j))
+                s.update_default_value(cat, review.get_id(j))
 
         # load data to the widget
-        self._load_data(j=j, cat=cat, notes=notes, data_cfg=data_cfg)
+        self._load_data(j=j, cat=cat, review=review, data_cfg=data_cfg)
 
         # display the data
         if self.data is not None:
             self.setEnabled(True)
             self.add_content()
 
             for s in self.sliders:
                 s.update_from_slider()
 
             self.reset_view()
         else:
             self.setEnabled(False)
 
-    def _load_data(self, j: int, cat: Table, notes: InspectionData, data_cfg: config.Data):
+    def _load_data(self, j: int, cat: Table, review: InspectionData, data_cfg: config.Data):
         if self.cfg.data.filename_keyword is None:
             logger.error(f'Filename keyword not specified (object ID: {self.title})')
             return
 
-        self.filename = get_filename(data_cfg.dir, self.cfg.data.filename_keyword, notes.get_id(j))
+        loader_params = {} if self.cfg.data.loader_params is None else self.cfg.data.loader_params
 
+        self.filename = get_filename(data_cfg.dir, self.cfg.data.filename_keyword, review.get_id(j))
         if self.filename is None:
-            logger.error('{} not found (object ID: {})'.format(self.title, notes.get_id(j)))
+            if not loader_params.get('silent'):
+                logger.error('{} not found (object ID: {})'.format(self.title, review.get_id(j)))
             self.data, self.meta = None, None
             return
 
-        loader_config = {} if self.cfg.data.loader_params is None else self.cfg.data.loader_params
-
-        self.data, self.meta = load(self.cfg.data.loader, self.filename, self.title, **loader_config)
+        self.data, self.meta = load(self.cfg.data.loader, self.filename, self.title, **loader_params)
         if self.data is None:
             return
 
         if not self.validate_dtype():
             self.data, self.meta = None, None
             return
```

