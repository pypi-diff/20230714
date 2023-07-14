# Comparing `tmp/ns_asphalt9-0.1.4.tar.gz` & `tmp/ns_asphalt9-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_asphalt9-0.1.4.tar", last modified: Fri Jul 14 17:47:00 2023, max compression
+gzip compressed data, was "ns_asphalt9-0.1.5.tar", last modified: Fri Jul 14 17:51:28 2023, max compression
```

## Comparing `ns_asphalt9-0.1.4.tar` & `ns_asphalt9-0.1.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:47:00.110654 ns_asphalt9-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-14 17:47:00.110654 ns_asphalt9-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:47:00.102654 ns_asphalt9-0.1.4/ns_asphalt9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:47:00.106654 ns_asphalt9-0.1.4/ns_asphalt9/core/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:47:00.106654 ns_asphalt9-0.1.4/ns_asphalt9/core/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/actions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/actions/enter_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/actions/process_race.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/actions/select_car.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:47:00.106654 ns_asphalt9-0.1.4/ns_asphalt9/core/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23659 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/gui/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:47:00.110654 ns_asphalt9-0.1.4/ns_asphalt9/core/gui/images/
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/gui/images/help.png
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/gui/images/home.png
--rw-r--r--   0 runner    (1001) docker     (123)   202347 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/gui/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/gui/images/settings.png
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/page_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:47:00.110654 ns_asphalt9-0.1.4/ns_asphalt9/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/utils/fetch_cars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/utils/fetch_tracks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/core/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/ns_asphalt9/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:47:00.106654 ns_asphalt9-0.1.4/ns_asphalt9.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-14 17:47:00.000000 ns_asphalt9-0.1.4/ns_asphalt9.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-14 17:47:00.000000 ns_asphalt9-0.1.4/ns_asphalt9.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:47:00.000000 ns_asphalt9-0.1.4/ns_asphalt9.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-14 17:47:00.000000 ns_asphalt9-0.1.4/ns_asphalt9.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:46:59.000000 ns_asphalt9-0.1.4/ns_asphalt9.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-14 17:47:00.000000 ns_asphalt9-0.1.4/ns_asphalt9.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 17:47:00.000000 ns_asphalt9-0.1.4/ns_asphalt9.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-14 17:47:00.110654 ns_asphalt9-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:47:00.110654 ns_asphalt9-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-14 17:46:40.000000 ns_asphalt9-0.1.4/tests/test_ocr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:51:28.660193 ns_asphalt9-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-14 17:51:28.660193 ns_asphalt9-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:51:28.656193 ns_asphalt9-0.1.5/ns_asphalt9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:51:28.660193 ns_asphalt9-0.1.5/ns_asphalt9/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:51:28.660193 ns_asphalt9-0.1.5/ns_asphalt9/core/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/actions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/actions/enter_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/actions/process_race.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/actions/select_car.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:51:28.660193 ns_asphalt9-0.1.5/ns_asphalt9/core/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23659 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/gui/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:51:28.660193 ns_asphalt9-0.1.5/ns_asphalt9/core/gui/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/gui/images/help.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/gui/images/home.png
+-rw-r--r--   0 runner    (1001) docker     (123)   202347 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/gui/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/gui/images/settings.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/page_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:51:28.660193 ns_asphalt9-0.1.5/ns_asphalt9/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/utils/fetch_cars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/utils/fetch_tracks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/core/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/ns_asphalt9/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:51:28.656193 ns_asphalt9-0.1.5/ns_asphalt9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-14 17:51:28.000000 ns_asphalt9-0.1.5/ns_asphalt9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-14 17:51:28.000000 ns_asphalt9-0.1.5/ns_asphalt9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:51:28.000000 ns_asphalt9-0.1.5/ns_asphalt9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-14 17:51:28.000000 ns_asphalt9-0.1.5/ns_asphalt9.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:51:28.000000 ns_asphalt9-0.1.5/ns_asphalt9.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-14 17:51:28.000000 ns_asphalt9-0.1.5/ns_asphalt9.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 17:51:28.000000 ns_asphalt9-0.1.5/ns_asphalt9.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-14 17:51:28.660193 ns_asphalt9-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:51:28.660193 ns_asphalt9-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-14 17:51:18.000000 ns_asphalt9-0.1.5/tests/test_ocr.py
```

### Comparing `ns_asphalt9-0.1.4/LICENSE` & `ns_asphalt9-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/PKG-INFO` & `ns_asphalt9-0.1.5/ns_asphalt9.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ns_asphalt9
-Version: 0.1.4
+Name: ns-asphalt9
+Version: 0.1.5
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.1.4/README.md` & `ns_asphalt9-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/actions/common.py` & `ns_asphalt9-0.1.5/ns_asphalt9/core/actions/common.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/actions/enter_page.py` & `ns_asphalt9-0.1.5/ns_asphalt9/core/actions/enter_page.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/actions/process_race.py` & `ns_asphalt9-0.1.5/ns_asphalt9/core/actions/process_race.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/actions/select_car.py` & `ns_asphalt9-0.1.5/ns_asphalt9/core/actions/select_car.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         pro.press_group([Buttons.A], 2)
 
         page = ocr_screen()
 
         # 如果没有进到车辆详情页面, router到默认任务
         if page.name != consts.car_info:
             TaskManager.task_enter(globals.CONFIG["模式"], page)
-            break
+            return
 
         pro.press_group([Buttons.A], 2)
 
         page = ocr_screen()
 
         if page.name in [
             consts.loading_race,
```

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/cache.py` & `ns_asphalt9-0.1.5/ns_asphalt9/core/cache.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/consts.py` & `ns_asphalt9-0.1.5/ns_asphalt9/core/consts.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/controller.py` & `ns_asphalt9-0.1.5/ns_asphalt9/core/controller.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/globals.py` & `ns_asphalt9-0.1.5/ns_asphalt9/core/globals.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/gui/app.py` & `ns_asphalt9-0.1.5/ns_asphalt9/core/gui/app.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/gui/images/help.png` & `ns_asphalt9-0.1.5/ns_asphalt9/core/gui/images/help.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/gui/images/home.png` & `ns_asphalt9-0.1.5/ns_asphalt9/core/gui/images/home.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/gui/images/logo.png` & `ns_asphalt9-0.1.5/ns_asphalt9/core/gui/images/logo.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/gui/images/settings.png` & `ns_asphalt9-0.1.5/ns_asphalt9/core/gui/images/settings.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/ocr.py` & `ns_asphalt9-0.1.5/ns_asphalt9/core/ocr.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/page_factory.py` & `ns_asphalt9-0.1.5/ns_asphalt9/core/page_factory.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/pages.py` & `ns_asphalt9-0.1.5/ns_asphalt9/core/pages.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/tasks.py` & `ns_asphalt9-0.1.5/ns_asphalt9/core/tasks.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/utils/decorator.py` & `ns_asphalt9-0.1.5/ns_asphalt9/core/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/utils/fetch_tracks.py` & `ns_asphalt9-0.1.5/ns_asphalt9/core/utils/fetch_tracks.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/utils/log.py` & `ns_asphalt9-0.1.5/ns_asphalt9/core/utils/log.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/core/utils/timer.py` & `ns_asphalt9-0.1.5/ns_asphalt9/core/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9/main.py` & `ns_asphalt9-0.1.5/ns_asphalt9/main.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9.egg-info/PKG-INFO` & `ns_asphalt9-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ns-asphalt9
-Version: 0.1.4
+Name: ns_asphalt9
+Version: 0.1.5
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.1.4/ns_asphalt9.egg-info/SOURCES.txt` & `ns_asphalt9-0.1.5/ns_asphalt9.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.1.4/setup.cfg` & `ns_asphalt9-0.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nxbt
-version = 0.1.4
+version = 0.1.5
 author = codehai
 author-email = wmpksb@gmail.com
 project_urls = 
 	Code = https://github.com/codehai/ns_asphalt9
 	Issue tracker = https://github.com/codehai/ns_asphalt9/issues
 license = GNU General Public License v3 (GPLv3)
 license-file = LICENSE
```

### Comparing `ns_asphalt9-0.1.4/tests/test_ocr.py` & `ns_asphalt9-0.1.5/tests/test_ocr.py`

 * *Files identical despite different names*

