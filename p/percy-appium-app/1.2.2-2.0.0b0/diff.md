# Comparing `tmp/percy-appium-app-1.2.2.tar.gz` & `tmp/percy-appium-app-2.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "percy-appium-app-1.2.2.tar", last modified: Mon May 29 07:43:16 2023, max compression
+gzip compressed data, was "percy-appium-app-2.0.0b0.tar", last modified: Fri Jul 14 15:32:33 2023, max compression
```

## Comparing `percy-appium-app-1.2.2.tar` & `percy-appium-app-2.0.0b0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:43:16.764246 percy-appium-app-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-29 07:43:16.760246 percy-appium-app-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:43:16.752246 percy-appium-app-1.2.2/percy/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:43:16.752246 percy-appium-app-1.2.2/percy/common/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:43:16.752246 percy-appium-app-1.2.2/percy/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/configs/devices.json
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:43:16.756246 percy-appium-app-1.2.2/percy/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/errors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:43:16.756246 percy-appium-app-1.2.2/percy/lib/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/lib/app_percy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/lib/cli_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/lib/ignore_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/lib/percy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/lib/tile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:43:16.756246 percy-appium-app-1.2.2/percy/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/metadata/android_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/metadata/ios_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/metadata/metadata_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:43:16.756246 percy-appium-app-1.2.2/percy/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/providers/app_automate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/providers/generic_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/providers/provider_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:43:16.756246 percy-appium-app-1.2.2/percy_appium_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-29 07:43:16.000000 percy-appium-app-1.2.2/percy_appium_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-29 07:43:16.000000 percy-appium-app-1.2.2/percy_appium_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 07:43:16.000000 percy-appium-app-1.2.2/percy_appium_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 07:43:16.000000 percy-appium-app-1.2.2/percy_appium_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-29 07:43:16.000000 percy-appium-app-1.2.2/percy_appium_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 07:43:16.000000 percy-appium-app-1.2.2/percy_appium_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 07:43:16.764246 percy-appium-app-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:43:16.760246 percy-appium-app-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_android_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_app_automate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_app_percy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_cli_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_generic_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_ignore_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_ios_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_metadata_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_percy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_tile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:33.254371 percy-appium-app-2.0.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-07-14 15:32:33.254371 percy-appium-app-2.0.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:33.246371 percy-appium-app-2.0.0b0/percy/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:33.250371 percy-appium-app-2.0.0b0/percy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:33.250371 percy-appium-app-2.0.0b0/percy/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/configs/devices.json
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:33.250371 percy-appium-app-2.0.0b0/percy/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/errors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:33.250371 percy-appium-app-2.0.0b0/percy/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/lib/app_percy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/lib/cli_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/lib/ignore_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/lib/percy_automate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/lib/percy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/lib/tile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:33.250371 percy-appium-app-2.0.0b0/percy/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/metadata/android_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/metadata/ios_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/metadata/metadata_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:33.250371 percy-appium-app-2.0.0b0/percy/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/providers/app_automate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/providers/generic_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/providers/provider_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/percy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:33.250371 percy-appium-app-2.0.0b0/percy_appium_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-07-14 15:32:33.000000 percy-appium-app-2.0.0b0/percy_appium_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-14 15:32:33.000000 percy-appium-app-2.0.0b0/percy_appium_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:32:33.000000 percy-appium-app-2.0.0b0/percy_appium_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:32:33.000000 percy-appium-app-2.0.0b0/percy_appium_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 15:32:33.000000 percy-appium-app-2.0.0b0/percy_appium_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 15:32:33.000000 percy-appium-app-2.0.0b0/percy_appium_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 15:32:33.254371 percy-appium-app-2.0.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:32:33.254371 percy-appium-app-2.0.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_android_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_app_automate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_app_percy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_cli_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_generic_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_ignore_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_ios_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_metadata_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_percy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-14 15:32:13.000000 percy-appium-app-2.0.0b0/tests/test_tile.py
```

### Comparing `percy-appium-app-1.2.2/LICENSE` & `percy-appium-app-2.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/PKG-INFO` & `percy-appium-app-2.0.0b0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: percy-appium-app
-Version: 1.2.2
+Version: 2.0.0b0
 Summary: Python client for visual testing with Percy for mobile apps
 Home-page: https://github.com/percy/percy-appium-python
 Author: Perceptual Inc.
 Author-email: team@percy.io
 License: MIT
 Keywords: appium percy visual testing
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -103,22 +103,41 @@
       ```
       init(self, top, bottom, left, right)
       ```
 
     - Parameters:
 
       `top` (int): Top coordinate of the ignore region.
-
       `bottom` (int): Bottom coordinate of the ignore region.
-
       `left` (int): Left coordinate of the ignore region.
-
       `right` (int): Right coordinate of the ignore region.
     - Raises:ValueError: If top, bottom, left, or right is less than 0 or top is greater than or equal to bottom or left is greater than or equal to right.
     - valid: Ignore region should be within the boundaries of the screen.
+
+## Running with Hybrid Apps
+
+For a hybrid app, we need to switch to native context before taking screenshot.
+
+- Add a helper method similar to following for say flutter based hybrid app:
+```python
+def percy_screenshot_flutter(driver, name: str, **kwargs):
+  driver.switch_to.context('NATIVE_APP')
+  percy_screenshot(driver, name, **kwargs)
+  driver.switch_to.context('FLUTTER')
+```
+
+- Call PercyScreenshotFlutter helper function when you want to take screenshot.
+```python
+percy_screenshot_flutter(driver, name, **kwargs)
+```
+
+> Note: 
+>
+> For other hybrid apps the `driver.switch_to.context('FLUTTER')` would change to context that it uses like say WEBVIEW etc.
+>
 ### Migrating Config
 
 If you have a previous Percy configuration file, migrate it to the newest version with the
 [`config:migrate`](https://github.com/percy/cli/tree/master/packages/cli-config#percy-configmigrate-filepath-output) command:
 
 ```sh-session
 $ percy config:migrate
```

### Comparing `percy-appium-app-1.2.2/README.md` & `percy-appium-app-2.0.0b0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -82,22 +82,41 @@
       ```
       init(self, top, bottom, left, right)
       ```
 
     - Parameters:
 
       `top` (int): Top coordinate of the ignore region.
-
       `bottom` (int): Bottom coordinate of the ignore region.
-
       `left` (int): Left coordinate of the ignore region.
-
       `right` (int): Right coordinate of the ignore region.
     - Raises:ValueError: If top, bottom, left, or right is less than 0 or top is greater than or equal to bottom or left is greater than or equal to right.
     - valid: Ignore region should be within the boundaries of the screen.
+
+## Running with Hybrid Apps
+
+For a hybrid app, we need to switch to native context before taking screenshot.
+
+- Add a helper method similar to following for say flutter based hybrid app:
+```python
+def percy_screenshot_flutter(driver, name: str, **kwargs):
+  driver.switch_to.context('NATIVE_APP')
+  percy_screenshot(driver, name, **kwargs)
+  driver.switch_to.context('FLUTTER')
+```
+
+- Call PercyScreenshotFlutter helper function when you want to take screenshot.
+```python
+percy_screenshot_flutter(driver, name, **kwargs)
+```
+
+> Note: 
+>
+> For other hybrid apps the `driver.switch_to.context('FLUTTER')` would change to context that it uses like say WEBVIEW etc.
+>
 ### Migrating Config
 
 If you have a previous Percy configuration file, migrate it to the newest version with the
 [`config:migrate`](https://github.com/percy/cli/tree/master/packages/cli-config#percy-configmigrate-filepath-output) command:
 
 ```sh-session
 $ percy config:migrate
```

### Comparing `percy-appium-app-1.2.2/percy/__init__.py` & `percy-appium-app-2.0.0b0/percy/__init__.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/percy/configs/devices.json` & `percy-appium-app-2.0.0b0/percy/configs/devices.json`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/percy/lib/app_percy.py` & `percy-appium-app-2.0.0b0/percy/lib/app_percy.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/percy/lib/cache.py` & `percy-appium-app-2.0.0b0/percy/lib/cache.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/percy/lib/cli_wrapper.py` & `percy-appium-app-2.0.0b0/percy/lib/cli_wrapper.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,14 +21,15 @@
             response = requests.get(f'{PERCY_CLI_API}/percy/healthcheck', timeout=10)
             response.raise_for_status()
             data = response.json()
 
             if not data['success']: raise CLIException(data['error'])
             Environment.percy_build_id = data['build']['id']
             Environment.percy_build_url = data['build']['url']
+            Environment.session_type = data['type']
             version = response.headers.get('x-percy-core-version')
 
             if version.split('.')[0] != '1':
                 log(f'Unsupported Percy CLI version, {version}')
                 return False
 
             return True
@@ -47,12 +48,34 @@
         # Handle errors
         response.raise_for_status()
         data = response.json()
 
         if response.status_code != 200:
             raise CLIException(data.get('error', 'UnknownException'))
         return data
+
+    def post_poa_screenshots(self, name, session_id, command_executor_url, capabilities, desired_capabilities, options=None):
+        body = {
+                'sessionId': session_id,
+                'commandExecutorUrl': command_executor_url,
+                'capabilities': dict(capabilities),
+                'sessionCapabilites':dict(desired_capabilities),
+                'snapshotName': name,
+                'options': options
+            }
+
+        body['client_info'] = Environment._get_client_info()
+        body['environment_info'] = Environment._get_env_info()
+
+        response = requests.post(f'{PERCY_CLI_API}/percy/automateScreenshot', json=body, timeout=30)
+        # Handle errors
+        response.raise_for_status()
+        data = response.json()
+
+        if response.status_code != 200:
+            raise CLIException(data.get('error', 'UnknownException'))
+        return data
 
     @staticmethod
     def _request_body(name, tag, tiles, external_debug_url, ignored_elements_data):
         tiles = list(map(dict, tiles))
         return {"name": name, "tag": tag, "tiles": tiles, "ignored_elements_data": ignored_elements_data, "external_debug_url": external_debug_url}
```

### Comparing `percy-appium-app-1.2.2/percy/lib/ignore_region.py` & `percy-appium-app-2.0.0b0/percy/lib/ignore_region.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/percy/lib/percy_options.py` & `percy-appium-app-2.0.0b0/percy/lib/percy_options.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/percy/lib/tile.py` & `percy-appium-app-2.0.0b0/percy/lib/tile.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/percy/metadata/android_metadata.py` & `percy-appium-app-2.0.0b0/percy/metadata/android_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/percy/metadata/ios_metadata.py` & `percy-appium-app-2.0.0b0/percy/metadata/ios_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/percy/metadata/metadata.py` & `percy-appium-app-2.0.0b0/percy/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/percy/providers/app_automate.py` & `percy-appium-app-2.0.0b0/percy/providers/app_automate.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/percy/providers/generic_provider.py` & `percy-appium-app-2.0.0b0/percy/providers/generic_provider.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/percy/providers/provider_resolver.py` & `percy-appium-app-2.0.0b0/percy/providers/provider_resolver.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/percy_appium_app.egg-info/PKG-INFO` & `percy-appium-app-2.0.0b0/percy_appium_app.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: percy-appium-app
-Version: 1.2.2
+Version: 2.0.0b0
 Summary: Python client for visual testing with Percy for mobile apps
 Home-page: https://github.com/percy/percy-appium-python
 Author: Perceptual Inc.
 Author-email: team@percy.io
 License: MIT
 Keywords: appium percy visual testing
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -103,22 +103,41 @@
       ```
       init(self, top, bottom, left, right)
       ```
 
     - Parameters:
 
       `top` (int): Top coordinate of the ignore region.
-
       `bottom` (int): Bottom coordinate of the ignore region.
-
       `left` (int): Left coordinate of the ignore region.
-
       `right` (int): Right coordinate of the ignore region.
     - Raises:ValueError: If top, bottom, left, or right is less than 0 or top is greater than or equal to bottom or left is greater than or equal to right.
     - valid: Ignore region should be within the boundaries of the screen.
+
+## Running with Hybrid Apps
+
+For a hybrid app, we need to switch to native context before taking screenshot.
+
+- Add a helper method similar to following for say flutter based hybrid app:
+```python
+def percy_screenshot_flutter(driver, name: str, **kwargs):
+  driver.switch_to.context('NATIVE_APP')
+  percy_screenshot(driver, name, **kwargs)
+  driver.switch_to.context('FLUTTER')
+```
+
+- Call PercyScreenshotFlutter helper function when you want to take screenshot.
+```python
+percy_screenshot_flutter(driver, name, **kwargs)
+```
+
+> Note: 
+>
+> For other hybrid apps the `driver.switch_to.context('FLUTTER')` would change to context that it uses like say WEBVIEW etc.
+>
 ### Migrating Config
 
 If you have a previous Percy configuration file, migrate it to the newest version with the
 [`config:migrate`](https://github.com/percy/cli/tree/master/packages/cli-config#percy-configmigrate-filepath-output) command:
 
 ```sh-session
 $ percy config:migrate
```

### Comparing `percy-appium-app-1.2.2/percy_appium_app.egg-info/SOURCES.txt` & `percy-appium-app-2.0.0b0/percy_appium_app.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 percy/configs/devices.json
 percy/errors/__init__.py
 percy/lib/__init__.py
 percy/lib/app_percy.py
 percy/lib/cache.py
 percy/lib/cli_wrapper.py
 percy/lib/ignore_region.py
+percy/lib/percy_automate.py
 percy/lib/percy_options.py
 percy/lib/tile.py
 percy/metadata/__init__.py
 percy/metadata/android_metadata.py
 percy/metadata/ios_metadata.py
 percy/metadata/metadata.py
 percy/metadata/metadata_resolver.py
```

### Comparing `percy-appium-app-1.2.2/setup.py` & `percy-appium-app-2.0.0b0/setup.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/tests/test_android_metadata.py` & `percy-appium-app-2.0.0b0/tests/test_android_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/tests/test_app_automate.py` & `percy-appium-app-2.0.0b0/tests/test_app_automate.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/tests/test_app_percy.py` & `percy-appium-app-2.0.0b0/tests/test_app_percy.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/tests/test_cache.py` & `percy-appium-app-2.0.0b0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/tests/test_cli_wrapper.py` & `percy-appium-app-2.0.0b0/tests/test_cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/tests/test_generic_provider.py` & `percy-appium-app-2.0.0b0/tests/test_generic_provider.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/tests/test_ignore_region.py` & `percy-appium-app-2.0.0b0/tests/test_ignore_region.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/tests/test_ios_metadata.py` & `percy-appium-app-2.0.0b0/tests/test_ios_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/tests/test_metadata.py` & `percy-appium-app-2.0.0b0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/tests/test_metadata_resolver.py` & `percy-appium-app-2.0.0b0/tests/test_metadata_resolver.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/tests/test_percy_options.py` & `percy-appium-app-2.0.0b0/tests/test_percy_options.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.2/tests/test_screenshot.py` & `percy-appium-app-2.0.0b0/tests/test_screenshot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # pylint: disable=[arguments-differ]
 import unittest
-from unittest.mock import patch, MagicMock, PropertyMock
+import json
+from unittest.mock import patch, MagicMock, PropertyMock, Mock
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from threading import Thread
 from appium.webdriver.webdriver import WebDriver
 from appium.webdriver.common.appiumby import AppiumBy
 
 
 import httpretty
@@ -31,16 +32,16 @@
 mock_server = HTTPServer(("localhost", 8000), MockServerRequestHandler)
 mock_server_thread = Thread(target=mock_server.serve_forever)
 mock_server_thread.daemon = True
 mock_server_thread.start()
 
 
 # mock helpers
-def mock_healthcheck(fail=False, fail_how="error"):
-    health_body = '{ "success": true, "build": {"id": "123", "url": "dummy_url"} }'
+def mock_healthcheck(fail=False, fail_how="error", type="AppPercy"):
+    health_body = json.dumps({ "success": True, "build": {"id": "123", "url": "dummy_url"}, "type": type })
     health_headers = {"X-Percy-Core-Version": "1.0.0"}
     health_status = 200
 
     if fail and fail_how == "error":
         health_body = '{ "success": false, "error": "test" }'
         health_status = 500
     elif fail and fail_how == "wrong-version":
@@ -63,14 +64,24 @@
         "http://localhost:5338/percy/comparison",
         body=(
             '{ "success": ' + ("true" if not fail else 'false, "error": "test"') + "}"
         ),
         status=(500 if fail else 200),
     )
 
+def mock_poa_screenshot(fail=False):
+    httpretty.register_uri(
+        httpretty.POST,
+        "http://localhost:5338/percy/automateScreenshot",
+        body=(
+            '{ "success": ' + ("true" if not fail else 'false, "error": "test"') + "}"
+        ),
+        status=(500 if fail else 200),
+    )
+
 
 class TestPercyScreenshot(unittest.TestCase):
     @patch("appium.webdriver.webdriver.WebDriver")
     def setUp(self, mock_webdriver) -> None:
         mock_webdriver.__class__ = WebDriver
         CLIWrapper.is_percy_enabled.cache_clear()
         httpretty.enable()
@@ -219,10 +230,58 @@
         self.assertRegex(body["environment_info"][0], r"appium/\d+")
         self.assertDictEqual(body["ignored_elements_data"], ignored_elements_data)
         self.mock_webdriver.find_element.assert_called_with(
             by=AppiumBy.XPATH, value="//path/to/element"
         )
         self.assertEqual(self.mock_webdriver.find_element.call_count, 1)
 
+    def test_throws_error_when_a_driver_is_not_provided_poa(self):
+        mock_healthcheck(type="automate")
+        with self.assertRaises(Exception):
+            percy_screenshot()
+
+    def test_throws_error_when_invalid_driver_provided_poa(self):
+        mock_healthcheck(type="automate")
+        with self.assertRaises(Exception):
+            percy_screenshot("Wrong driver")
+
+    def test_throws_error_when_a_name_is_not_provided_poa(self):
+        mock_healthcheck(type="automate")
+        with self.assertRaises(Exception):
+            percy_screenshot(self.mock_webdriver)
+
+    def test_posts_screenshot_poa(self):
+        mock_healthcheck(type="automate")
+        mock_poa_screenshot()
+
+        driver = Mock(spec=WebDriver)
+        driver.session_id = 'Dummy_session_id'
+        driver.capabilities = { 'key': 'value' }
+        driver.desired_capabilities = { 'key': 'value' }
+        driver.command_executor = Mock()
+        driver.command_executor._url = 'https://hub-cloud.browserstack.com/wd/hub'
+
+        element = Mock()
+        element.id = 'Dummy_id'
+        self.mock_webdriver.capabilities = { 'key': 'value' }
+        percy_screenshot(driver, 'Snapshot 1')
+        percy_screenshot(driver, 'Snapshot 2', options = {'enable_javascript': True,
+                          'ignore_region_appium_elements': [element]})
+
+        self.assertEqual(httpretty.last_request().path, '/percy/automateScreenshot')
+
+        s1 = httpretty.latest_requests()[1].parsed_body
+        self.assertEqual(s1['snapshotName'], 'Snapshot 1')
+        self.assertEqual(s1['sessionId'], driver.session_id)
+        self.assertEqual(s1['commandExecutorUrl'], driver.command_executor._url) # pylint: disable=W0212
+        self.assertEqual(s1['capabilities'], dict(driver.capabilities))
+        self.assertEqual(s1['sessionCapabilites'], dict(driver.desired_capabilities))
+        self.assertRegex(s1['client_info'], r'percy-appium-app/\d+')
+        self.assertRegex(s1['environment_info'][0], r'appium/\d+')
+        self.assertRegex(s1['environment_info'][1], r'python/\d+')
+        s2 = httpretty.latest_requests()[-1].parsed_body
+        self.assertEqual(s2['snapshotName'], 'Snapshot 2')
+        self.assertEqual(s2['options']['enable_javascript'], True)
+        self.assertEqual(s2['options']['ignore_region_elements'], ['Dummy_id'])
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `percy-appium-app-1.2.2/tests/test_tile.py` & `percy-appium-app-2.0.0b0/tests/test_tile.py`

 * *Files identical despite different names*

