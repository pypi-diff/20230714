# Comparing `tmp/selenium_profiles-2.2.7.2.tar.gz` & `tmp/selenium_profiles-2.2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\selenium_profiles-2.2.7.2.tar", last modified: Mon Jul  3 16:15:51 2023, max compression
+gzip compressed data, was "dist\selenium_profiles-2.2.7.3.tar", last modified: Fri Jul 14 14:03:50 2023, max compression
```

## Comparing `selenium_profiles-2.2.7.2.tar` & `selenium_profiles-2.2.7.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/
--rw-rw-rw-   0        0        0      641 2022-11-24 08:41:11.000000 selenium_profiles-2.2.7.2/LICENSE.md
--rw-rw-rw-   0        0        0      261 2023-01-17 17:45:34.000000 selenium_profiles-2.2.7.2/MANIFEST.in
--rw-rw-rw-   0        0        0    14204 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/PKG-INFO
--rw-rw-rw-   0        0        0    12856 2023-06-27 07:02:11.000000 selenium_profiles-2.2.7.2/README.md
--rw-rw-rw-   0        0        0     1738 2023-06-27 11:47:23.000000 selenium_profiles-2.2.7.2/build_upload.md
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_profiles-2.2.7.2/pyproject.toml
--rw-rw-rw-   0        0        0      131 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/setup.cfg
--rw-rw-rw-   0        0        0     2083 2023-07-03 16:06:43.000000 selenium_profiles-2.2.7.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/
--rw-rw-rw-   0        0        0       25 2023-07-03 16:05:44.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/files/
--rw-rw-rw-   0        0        0       21 2022-11-24 09:43:39.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/files/proxy_extension/
--rw-rw-rw-   0        0        0      615 2023-01-17 17:37:32.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/files/proxy_extension/background.js
--rw-rw-rw-   0        0        0      347 2023-01-17 07:03:50.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/files/proxy_extension/manifest.json
-drwxrwxrwx   0        0        0        0 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/files/tmp/
--rw-rw-rw-   0        0        0        0 2023-01-17 07:50:51.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/files/tmp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/files/tmp/proxy_extension/
--rw-rw-rw-   0        0        0      652 2023-04-12 17:20:07.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/files/tmp/proxy_extension/background.js
--rw-rw-rw-   0        0        0      347 2023-04-12 17:20:07.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/files/tmp/proxy_extension/manifest.json
-drwxrwxrwx   0        0        0        0 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/js/
--rw-rw-rw-   0        0        0       21 2022-11-24 09:43:39.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/js/__init__.py
--rw-rw-rw-   0        0        0     3098 2023-04-09 15:39:08.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/js/export_profile.js
--rw-rw-rw-   0        0        0     1243 2023-04-09 15:50:01.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/js/fetch.js
-drwxrwxrwx   0        0        0        0 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/js/undetected/
--rw-rw-rw-   0        0        0        0 2022-11-30 15:39:00.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/js/undetected/__init.py
--rw-rw-rw-   0        0        0      291 2022-11-30 15:48:11.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/js/undetected/get_cdc_props.js
--rw-rw-rw-   0        0        0      392 2022-11-30 15:43:54.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/js/undetected/navigator_webdriver.js
--rw-rw-rw-   0        0        0      357 2022-11-30 15:51:50.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/js/undetected/remove_cdc_props.js
-drwxrwxrwx   0        0        0        0 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/profiles/
--rw-rw-rw-   0        0        0       85 2022-11-24 12:02:54.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/profiles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/profiles/__pycache__/
--rw-rw-rw-   0        0        0      293 2023-04-10 19:28:24.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/profiles/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      287 2023-04-09 11:28:56.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/profiles/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     1419 2023-04-10 19:28:24.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/profiles/__pycache__/profiles.cpython-310.pyc
--rw-rw-rw-   0        0        0     1418 2023-06-20 17:12:11.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/profiles/__pycache__/profiles.cpython-37.pyc
--rw-rw-rw-   0        0        0     3080 2023-04-10 20:03:55.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/profiles/default.json
--rw-rw-rw-   0        0        0     1856 2023-04-10 20:31:32.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/profiles/example.json
--rw-rw-rw-   0        0        0      837 2023-06-20 17:12:01.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/profiles/profiles.py
--rw-rw-rw-   0        0        0     1891 2022-12-17 00:01:23.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/profiles/scratch.json
-drwxrwxrwx   0        0        0        0 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/scripts/__init__.py
--rw-rw-rw-   0        0        0    10723 2023-06-20 19:25:57.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/scripts/driver_utils.py
--rw-rw-rw-   0        0        0    24902 2023-06-27 09:54:03.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/scripts/profiles.py
--rw-rw-rw-   0        0        0     4687 2023-06-27 07:04:38.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/scripts/proxy.py
--rw-rw-rw-   0        0        0     1649 2023-06-26 05:06:24.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/scripts/undetected.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/utils/
--rw-rw-rw-   0        0        0        0 2023-01-13 13:06:48.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/utils/__init__.py
--rw-rw-rw-   0        0        0     1887 2023-03-16 14:15:27.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/utils/colab_utils.py
--rw-rw-rw-   0        0        0     1755 2023-06-26 05:36:03.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/utils/utils.py
--rw-rw-rw-   0        0        0    11010 2023-07-03 15:54:01.000000 selenium_profiles-2.2.7.2/src/selenium_profiles/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/src/selenium_profiles.egg-info/
--rw-rw-rw-   0        0        0    14204 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/src/selenium_profiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1869 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/src/selenium_profiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/src/selenium_profiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/src/selenium_profiles.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/src/selenium_profiles.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-03 16:15:51.000000 selenium_profiles-2.2.7.2/tests/
--rw-rw-rw-   0        0        0     1617 2023-06-27 16:34:45.000000 selenium_profiles-2.2.7.2/tests/test_driver.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/
+-rw-rw-rw-   0        0        0      641 2022-11-24 08:41:11.000000 selenium_profiles-2.2.7.3/LICENSE.md
+-rw-rw-rw-   0        0        0      261 2023-01-17 17:45:34.000000 selenium_profiles-2.2.7.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    14374 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0    13026 2023-07-14 13:59:58.000000 selenium_profiles-2.2.7.3/README.md
+-rw-rw-rw-   0        0        0     1740 2023-07-03 16:17:23.000000 selenium_profiles-2.2.7.3/build_upload.md
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_profiles-2.2.7.3/pyproject.toml
+-rw-rw-rw-   0        0        0      131 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/setup.cfg
+-rw-rw-rw-   0        0        0     2083 2023-07-14 14:01:27.000000 selenium_profiles-2.2.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/
+-rw-rw-rw-   0        0        0       25 2023-07-14 14:01:02.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/files/
+-rw-rw-rw-   0        0        0       21 2022-11-24 09:43:39.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/files/proxy_extension/
+-rw-rw-rw-   0        0        0      615 2023-01-17 17:37:32.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/files/proxy_extension/background.js
+-rw-rw-rw-   0        0        0      347 2023-01-17 07:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/files/proxy_extension/manifest.json
+drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/files/tmp/
+-rw-rw-rw-   0        0        0        0 2023-01-17 07:50:51.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/files/tmp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/files/tmp/proxy_extension/
+-rw-rw-rw-   0        0        0      652 2023-04-12 17:20:07.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/files/tmp/proxy_extension/background.js
+-rw-rw-rw-   0        0        0      347 2023-04-12 17:20:07.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/files/tmp/proxy_extension/manifest.json
+drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/js/
+-rw-rw-rw-   0        0        0       21 2022-11-24 09:43:39.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/js/__init__.py
+-rw-rw-rw-   0        0        0     3098 2023-04-09 15:39:08.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/js/export_profile.js
+-rw-rw-rw-   0        0        0     1243 2023-04-09 15:50:01.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/js/fetch.js
+drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/js/undetected/
+-rw-rw-rw-   0        0        0        0 2022-11-30 15:39:00.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/js/undetected/__init.py
+-rw-rw-rw-   0        0        0      291 2022-11-30 15:48:11.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/js/undetected/get_cdc_props.js
+-rw-rw-rw-   0        0        0      392 2022-11-30 15:43:54.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/js/undetected/navigator_webdriver.js
+-rw-rw-rw-   0        0        0      357 2022-11-30 15:51:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/js/undetected/remove_cdc_props.js
+drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/
+-rw-rw-rw-   0        0        0       85 2022-11-24 12:02:54.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/__pycache__/
+-rw-rw-rw-   0        0        0      293 2023-04-10 19:28:24.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      287 2023-04-09 11:28:56.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1419 2023-04-10 19:28:24.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/__pycache__/profiles.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1418 2023-06-20 17:12:11.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/__pycache__/profiles.cpython-37.pyc
+-rw-rw-rw-   0        0        0     3080 2023-04-10 20:03:55.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/default.json
+-rw-rw-rw-   0        0        0     1856 2023-04-10 20:31:32.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/example.json
+-rw-rw-rw-   0        0        0      837 2023-06-20 17:12:01.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/profiles.py
+-rw-rw-rw-   0        0        0     1891 2022-12-17 00:01:23.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/scratch.json
+drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/scripts/__init__.py
+-rw-rw-rw-   0        0        0    10723 2023-06-20 19:25:57.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/scripts/driver_utils.py
+-rw-rw-rw-   0        0        0    24902 2023-06-27 09:54:03.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/scripts/profiles.py
+-rw-rw-rw-   0        0        0     4687 2023-06-27 07:04:38.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/scripts/proxy.py
+-rw-rw-rw-   0        0        0     1649 2023-06-26 05:06:24.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/scripts/undetected.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/utils/
+-rw-rw-rw-   0        0        0        0 2023-01-13 13:06:48.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/utils/__init__.py
+-rw-rw-rw-   0        0        0     1887 2023-03-16 14:15:27.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/utils/colab_utils.py
+-rw-rw-rw-   0        0        0     1755 2023-06-26 05:36:03.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/utils/utils.py
+-rw-rw-rw-   0        0        0    10234 2023-07-14 13:57:17.000000 selenium_profiles-2.2.7.3/src/selenium_profiles/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles.egg-info/
+-rw-rw-rw-   0        0        0    14374 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1869 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/src/selenium_profiles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 14:03:50.000000 selenium_profiles-2.2.7.3/tests/
+-rw-rw-rw-   0        0        0     1617 2023-06-27 16:34:45.000000 selenium_profiles-2.2.7.3/tests/test_driver.py
```

### Comparing `selenium_profiles-2.2.7.2/LICENSE.md` & `selenium_profiles-2.2.7.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.2/PKG-INFO` & `selenium_profiles-2.2.7.3/src/selenium_profiles.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: selenium_profiles
-Version: 2.2.7.2
+Name: selenium-profiles
+Version: 2.2.7.3
 Summary: Emulate and Automate Chrome using Profiles and Selenium
 Home-page: https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium_Profiles
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium_Profiles/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium_Profiles
@@ -67,15 +67,15 @@
 from selenium.webdriver.common.by import By  # locate elements
 from seleniumwire import webdriver
 
 
 profile = profiles.Windows() # or .Android
 options = webdriver.ChromeOptions()
 options.add_argument("--headless=new")
-driver = Chrome(profile, options=options, base_drivers=(webdriver.Chrome,),
+driver = Chrome(profile, options=options,
                 uc_driver=False
                 )
 
 # get url
 driver.get('https://abrahamjuliot.github.io/creepjs/')  # test fingerprint
 
 input("Press ENTER to exit: ")
@@ -168,14 +168,38 @@
 driver.get("https://httpbin.org/headers")
 
 input("Press ENTER to quit..")
 driver.quit()
 exit()
 ```
 
+Using [Selenium-Injector](https://github.com/kaliiiiiiiiii/Selenium-Injector)
+```python
+from selenium_profiles.webdriver import Chrome
+
+driver = Chrome(injector_options=True)
+injector = driver.profiles.injector
+
+# modify headers
+injector.declarativeNetRequest.update_headers({"test": "test_2", "sec-ch-ua-platform": "Android"})
+rules = injector.declarativeNetRequest.dynamic_rules
+headers = injector.declarativeNetRequest._headers
+
+driver.get("https://httpbin.org/headers")
+input("press ENTER to continue")
+
+# block images
+injector.declarativeNetRequest.update_block_on(resource_types=["image"])
+
+driver.get("https://www.wikimedia.org/")
+
+input("press ENTER to exit")
+driver.quit()
+```
+
 ### Touch_actions
 
 Example demonstration script
 ```python
 from selenium_profiles.webdriver import Chrome
 from selenium_profiles.profiles import profiles
 from selenium.webdriver.common.by import By
@@ -263,16 +287,14 @@
 
 ## Known Bugs
 
 - [click_as_touch makes automation hung](https://github.com/kaliiiiiiiiii/Selenium-Profiles/issues/1)
 
 
 ## Todo
-- [ ] use class instead of generator function at `selenium_profiles.webdriver.Chrome`
-- [ ] dynamic proxies [issue](https://github.com/kaliiiiiiiiii/Selenium-Profiles/issues/52)
 - [x] js-undetectability
   - [ ] [`navigator.connection`]
   - [ ] fonts don't match platform
   - [ ] does not match worker scope (Emulation) [crbug#1358491](https://bugs.chromium.org/p/chromium/issues/detail?id=1358491)
     - `Navigator.userAgent`
     - `Navigator.platform`
     - `navigator.hardwareConcurrency`
@@ -281,15 +303,14 @@
     - [ ] Either Devtools Console is open or CDP Runtime Domain is enabled => patch javascript objects using a Proxy or disable CDP.Runtime domain?
     - [ ] [document.$cdc_asdjflasutopfhvcZLmcfl_](https://source.chromium.org/chromium/chromium/src/+/main:chrome/test/chromedriver/js/call_function.js;l=219)
     - [ ] [`document.$chrome_asyncScriptInfo`](https://source.chromium.org/chromium/chromium/src/+/main:chrome/test/chromedriver/chrome/web_view_impl.cc;l=1586-1597;drc=2e14a3ac178ee87aa9154e5a15dcd986af1b6059)
     - [ ] driver.execute_script() usage (needs hook on called element)
     - [ ] driver.execute_async_script() usage (needs hook on called element)
     - [ ] driver.find_element() usage
     - [x] [`window.cdc_adoQpoasnfa76pfcZLmcfl`](https://source.chromium.org/chromium/chromium/src/+/main:chrome/test/chromedriver/chrome/devtools_client_impl.cc;l=526-532;drc=f915006bb8e09e0c29016cf9ab9e737cdebc1adc)
-- [x] allow passing seleniumwire-options => [discussion](https://github.com/kaliiiiiiiiii/Selenium-Profiles/discussions/36)
 - [x] default metrics
   - [x] Android
   - [x] Windows
   - [ ] IOS
   - [ ] Linux
   - [ ] Tablet
 - [ ] test.py script
@@ -299,19 +320,14 @@
         - [x] useragent-data
         - [ ] undetected
           - [ ] headless
       - [x] Android
        - [x] useragent-data
        - [ ] undetected
          - [ ] headless
-- [ ] [audio_captcha_solver](https://github.com/najmi9/solve-recaptcha-python-selenium/blob/master/main.py)
-- [X] support for 
-  - [x] Windows
-  - [x] Jupyter Notebook (Google-Colab)
-  - [x] Linux
 
 
 ## Deprecated
 
 * [Stealth method]((https://github.com/diprajpatra/selenium-stealth)) (Detected by Google)
 * [buster captcha solver](https://github.com/dessant/buster) | [wontfix](https://github.com/kaliiiiiiiiii/Selenium_Profiles/issues/3)
```

### Comparing `selenium_profiles-2.2.7.2/README.md` & `selenium_profiles-2.2.7.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+Metadata-Version: 2.1
+Name: selenium_profiles
+Version: 2.2.7.3
+Summary: Emulate and Automate Chrome using Profiles and Selenium
+Home-page: https://github.com/kaliiiiiiiiii/Selenium_Profiles
+Author: Aurin Aegerter
+Author-email: aurinliun@gmx.ch
+Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium_Profiles
+Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium_Profiles/issues
+Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium_Profiles
+Keywords: Selenium,emulation,automation,undetected-chromedriver,webautomation
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: Free for non-commercial use
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: Jupyter
+Classifier: Topic :: Internet
+Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.md
+
 # Selenium-Profiles
 
 [![Downloads](https://static.pepy.tech/badge/selenium-profiles)](https://pepy.tech/project/selenium-profiles) [![](https://img.shields.io/pypi/v/selenium-profiles.svg?color=3399EE)](https://pypi.org/project/selenium-profiles/)
 
 * Overwrite **device metrics** using Selenium
 * Mobile and Desktop **emulation**
 * **Undetected** by Google, Cloudflare, creep-js ..
@@ -37,15 +67,15 @@
 from selenium.webdriver.common.by import By  # locate elements
 from seleniumwire import webdriver
 
 
 profile = profiles.Windows() # or .Android
 options = webdriver.ChromeOptions()
 options.add_argument("--headless=new")
-driver = Chrome(profile, options=options, base_drivers=(webdriver.Chrome,),
+driver = Chrome(profile, options=options,
                 uc_driver=False
                 )
 
 # get url
 driver.get('https://abrahamjuliot.github.io/creepjs/')  # test fingerprint
 
 input("Press ENTER to exit: ")
@@ -138,14 +168,38 @@
 driver.get("https://httpbin.org/headers")
 
 input("Press ENTER to quit..")
 driver.quit()
 exit()
 ```
 
+Using [Selenium-Injector](https://github.com/kaliiiiiiiiii/Selenium-Injector)
+```python
+from selenium_profiles.webdriver import Chrome
+
+driver = Chrome(injector_options=True)
+injector = driver.profiles.injector
+
+# modify headers
+injector.declarativeNetRequest.update_headers({"test": "test_2", "sec-ch-ua-platform": "Android"})
+rules = injector.declarativeNetRequest.dynamic_rules
+headers = injector.declarativeNetRequest._headers
+
+driver.get("https://httpbin.org/headers")
+input("press ENTER to continue")
+
+# block images
+injector.declarativeNetRequest.update_block_on(resource_types=["image"])
+
+driver.get("https://www.wikimedia.org/")
+
+input("press ENTER to exit")
+driver.quit()
+```
+
 ### Touch_actions
 
 Example demonstration script
 ```python
 from selenium_profiles.webdriver import Chrome
 from selenium_profiles.profiles import profiles
 from selenium.webdriver.common.by import By
@@ -233,16 +287,14 @@
 
 ## Known Bugs
 
 - [click_as_touch makes automation hung](https://github.com/kaliiiiiiiiii/Selenium-Profiles/issues/1)
 
 
 ## Todo
-- [ ] use class instead of generator function at `selenium_profiles.webdriver.Chrome`
-- [ ] dynamic proxies [issue](https://github.com/kaliiiiiiiiii/Selenium-Profiles/issues/52)
 - [x] js-undetectability
   - [ ] [`navigator.connection`]
   - [ ] fonts don't match platform
   - [ ] does not match worker scope (Emulation) [crbug#1358491](https://bugs.chromium.org/p/chromium/issues/detail?id=1358491)
     - `Navigator.userAgent`
     - `Navigator.platform`
     - `navigator.hardwareConcurrency`
@@ -251,15 +303,14 @@
     - [ ] Either Devtools Console is open or CDP Runtime Domain is enabled => patch javascript objects using a Proxy or disable CDP.Runtime domain?
     - [ ] [document.$cdc_asdjflasutopfhvcZLmcfl_](https://source.chromium.org/chromium/chromium/src/+/main:chrome/test/chromedriver/js/call_function.js;l=219)
     - [ ] [`document.$chrome_asyncScriptInfo`](https://source.chromium.org/chromium/chromium/src/+/main:chrome/test/chromedriver/chrome/web_view_impl.cc;l=1586-1597;drc=2e14a3ac178ee87aa9154e5a15dcd986af1b6059)
     - [ ] driver.execute_script() usage (needs hook on called element)
     - [ ] driver.execute_async_script() usage (needs hook on called element)
     - [ ] driver.find_element() usage
     - [x] [`window.cdc_adoQpoasnfa76pfcZLmcfl`](https://source.chromium.org/chromium/chromium/src/+/main:chrome/test/chromedriver/chrome/devtools_client_impl.cc;l=526-532;drc=f915006bb8e09e0c29016cf9ab9e737cdebc1adc)
-- [x] allow passing seleniumwire-options => [discussion](https://github.com/kaliiiiiiiiii/Selenium-Profiles/discussions/36)
 - [x] default metrics
   - [x] Android
   - [x] Windows
   - [ ] IOS
   - [ ] Linux
   - [ ] Tablet
 - [ ] test.py script
@@ -269,19 +320,14 @@
         - [x] useragent-data
         - [ ] undetected
           - [ ] headless
       - [x] Android
        - [x] useragent-data
        - [ ] undetected
          - [ ] headless
-- [ ] [audio_captcha_solver](https://github.com/najmi9/solve-recaptcha-python-selenium/blob/master/main.py)
-- [X] support for 
-  - [x] Windows
-  - [x] Jupyter Notebook (Google-Colab)
-  - [x] Linux
 
 
 ## Deprecated
 
 * [Stealth method]((https://github.com/diprajpatra/selenium-stealth)) (Detected by Google)
 * [buster captcha solver](https://github.com/dessant/buster) | [wontfix](https://github.com/kaliiiiiiiiii/Selenium_Profiles/issues/3)
```

### Comparing `selenium_profiles-2.2.7.2/build_upload.md` & `selenium_profiles-2.2.7.3/build_upload.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,22 +25,22 @@
 # 3.11
 C:\Users\aurin\PycharmProjects\selenium_profiles\venv311\Scripts\pip.exe install C:\Users\aurin\PycharmProjects\selenium_profiles
 ```
 
 ## install all python versions from pypi
 ```shell
 # 3.7
-C:\Users\aurin\PycharmProjects\selenium_profiles\venv\Scripts\pip.exe install --no-cache-dir selenium_profiles==2.2.7.1
+C:\Users\aurin\PycharmProjects\selenium_profiles\venv\Scripts\pip.exe install --no-cache-dir selenium_profiles==2.2.7.2
 # 3.8
-C:\Users\aurin\PycharmProjects\selenium_profiles\venv38\Scripts\pip.exe install --no-cache-dir selenium-profiles==2.2.7.1
+C:\Users\aurin\PycharmProjects\selenium_profiles\venv38\Scripts\pip.exe install --no-cache-dir selenium-profiles==2.2.7.2
 # 3.9
-C:\Users\aurin\PycharmProjects\selenium_profiles\venv39\Scripts\pip.exe  install --no-cache-dir selenium-profiles==2.2.7.1
+C:\Users\aurin\PycharmProjects\selenium_profiles\venv39\Scripts\pip.exe  install --no-cache-dir selenium-profiles==2.2.7.2
 # 3.10
-C:\Users\aurin\PycharmProjects\selenium_profiles\venv310\Scripts\pip.exe install --no-cache-dir selenium-profiles==2.2.7.1
+C:\Users\aurin\PycharmProjects\selenium_profiles\venv310\Scripts\pip.exe install --no-cache-dir selenium-profiles==2.2.7.2
 # 3.11
-C:\Users\aurin\PycharmProjects\selenium_profiles\venv311\Scripts\pip.exe install --no-cache-dir selenium-profiles==2.2.7
+C:\Users\aurin\PycharmProjects\selenium_profiles\venv311\Scripts\pip.exe install --no-cache-dir selenium-profiles==2.2.7.2
 ```
 
 ## install from GitHub
 ```shell
 pip install https://github.com/kaliiiiiiiiii/Selenium-Profiles/archive/refs/heads/master.zip
 ```
```

### Comparing `selenium_profiles-2.2.7.2/setup.py` & `selenium_profiles-2.2.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 import sys
 
 
-requirements = ['selenium', 'requests', 'selenium-interceptor', "undetected-chromedriver", "selenium-wire", "webdriver-manager", "selenium-injector>=2.2"]
+requirements = ['selenium', 'requests', 'selenium-interceptor', "undetected-chromedriver", "selenium-wire", "webdriver-manager", "selenium-injector>=2.3"]
 
 if 'google.colab' in sys.modules: # we're on google-colab
     requirements.extend(['PyVirtualDisplay', "google-colab-shell"])
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
```

### Comparing `selenium_profiles-2.2.7.2/src/selenium_profiles/files/proxy_extension/background.js` & `selenium_profiles-2.2.7.3/src/selenium_profiles/files/proxy_extension/background.js`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.2/src/selenium_profiles/files/tmp/proxy_extension/background.js` & `selenium_profiles-2.2.7.3/src/selenium_profiles/files/tmp/proxy_extension/background.js`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.2/src/selenium_profiles/js/export_profile.js` & `selenium_profiles-2.2.7.3/src/selenium_profiles/js/export_profile.js`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.2/src/selenium_profiles/js/fetch.js` & `selenium_profiles-2.2.7.3/src/selenium_profiles/js/fetch.js`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.2/src/selenium_profiles/profiles/__pycache__/profiles.cpython-310.pyc` & `selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/__pycache__/profiles.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.2/src/selenium_profiles/profiles/__pycache__/profiles.cpython-37.pyc` & `selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/__pycache__/profiles.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.2/src/selenium_profiles/profiles/default.json` & `selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/default.json`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.2/src/selenium_profiles/profiles/example.json` & `selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/example.json`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.2/src/selenium_profiles/profiles/profiles.py` & `selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/profiles.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.2/src/selenium_profiles/profiles/scratch.json` & `selenium_profiles-2.2.7.3/src/selenium_profiles/profiles/scratch.json`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.2/src/selenium_profiles/scripts/driver_utils.py` & `selenium_profiles-2.2.7.3/src/selenium_profiles/scripts/driver_utils.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.2/src/selenium_profiles/scripts/profiles.py` & `selenium_profiles-2.2.7.3/src/selenium_profiles/scripts/profiles.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.2/src/selenium_profiles/scripts/proxy.py` & `selenium_profiles-2.2.7.3/src/selenium_profiles/scripts/proxy.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.2/src/selenium_profiles/scripts/undetected.py` & `selenium_profiles-2.2.7.3/src/selenium_profiles/scripts/undetected.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.2/src/selenium_profiles/utils/colab_utils.py` & `selenium_profiles-2.2.7.3/src/selenium_profiles/utils/colab_utils.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.2/src/selenium_profiles/utils/utils.py` & `selenium_profiles-2.2.7.3/src/selenium_profiles/utils/utils.py`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.2/src/selenium_profiles/webdriver.py` & `selenium_profiles-2.2.7.3/src/selenium_profiles/webdriver.py`

 * *Files 14% similar despite different names*

```diff
@@ -155,27 +155,14 @@
 
         self.profiles.cdp_handler.apply(cdp_profile=profile["cdp"])
 
         if not uc_driver:
             from selenium_profiles.scripts import undetected
             undetected.exec_cdp(self, cdp_handler=self.profiles.cdp_handler)
 
-        if injector_options or injector_options == {}:
-            from selenium_injector.scripts.injector import make_config
-
-            # connection to tab-0
-            tab_index = self.window_handles.index(self.current_window_handle).__str__()
-            self.profiles.injector.tab_user = "tab-" + tab_index
-            config = make_config(host=injector.socket.host, port=injector.socket.port, user=self.profiles.injector.tab_user, debug=True)
-
-            from selenium_injector.utils.utils import read
-            utils_js = read("files/js/utils.js")
-            self.execute_cdp_cmd("Page.addScriptToEvaluateOnNewDocument",
-                                 {"source": "(function(){%s})()" % (utils_js + self.profiles.injector.connection_js + config)})
-
         if proxy["proxy"]:
             from selenium_profiles.utils.utils import valid_key
             # noinspection PyUnresolvedReferences
             valid_key(proxy.keys(), ["proxy", "bypass_list"], '"profiles["proxy"]"')
             # noinspection PyUnresolvedReferences
             self.profiles.proxy.set_single(proxy["proxy"], bypass_list=proxy["bypass_list"])
```

### Comparing `selenium_profiles-2.2.7.2/src/selenium_profiles.egg-info/PKG-INFO` & `selenium_profiles-2.2.7.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.1
-Name: selenium-profiles
-Version: 2.2.7.2
-Summary: Emulate and Automate Chrome using Profiles and Selenium
-Home-page: https://github.com/kaliiiiiiiiii/Selenium_Profiles
-Author: Aurin Aegerter
-Author-email: aurinliun@gmx.ch
-Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium_Profiles
-Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium_Profiles/issues
-Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium_Profiles
-Keywords: Selenium,emulation,automation,undetected-chromedriver,webautomation
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: Free for non-commercial use
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: Jupyter
-Classifier: Topic :: Internet
-Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.md
-
 # Selenium-Profiles
 
 [![Downloads](https://static.pepy.tech/badge/selenium-profiles)](https://pepy.tech/project/selenium-profiles) [![](https://img.shields.io/pypi/v/selenium-profiles.svg?color=3399EE)](https://pypi.org/project/selenium-profiles/)
 
 * Overwrite **device metrics** using Selenium
 * Mobile and Desktop **emulation**
 * **Undetected** by Google, Cloudflare, creep-js ..
@@ -67,15 +37,15 @@
 from selenium.webdriver.common.by import By  # locate elements
 from seleniumwire import webdriver
 
 
 profile = profiles.Windows() # or .Android
 options = webdriver.ChromeOptions()
 options.add_argument("--headless=new")
-driver = Chrome(profile, options=options, base_drivers=(webdriver.Chrome,),
+driver = Chrome(profile, options=options,
                 uc_driver=False
                 )
 
 # get url
 driver.get('https://abrahamjuliot.github.io/creepjs/')  # test fingerprint
 
 input("Press ENTER to exit: ")
@@ -168,14 +138,38 @@
 driver.get("https://httpbin.org/headers")
 
 input("Press ENTER to quit..")
 driver.quit()
 exit()
 ```
 
+Using [Selenium-Injector](https://github.com/kaliiiiiiiiii/Selenium-Injector)
+```python
+from selenium_profiles.webdriver import Chrome
+
+driver = Chrome(injector_options=True)
+injector = driver.profiles.injector
+
+# modify headers
+injector.declarativeNetRequest.update_headers({"test": "test_2", "sec-ch-ua-platform": "Android"})
+rules = injector.declarativeNetRequest.dynamic_rules
+headers = injector.declarativeNetRequest._headers
+
+driver.get("https://httpbin.org/headers")
+input("press ENTER to continue")
+
+# block images
+injector.declarativeNetRequest.update_block_on(resource_types=["image"])
+
+driver.get("https://www.wikimedia.org/")
+
+input("press ENTER to exit")
+driver.quit()
+```
+
 ### Touch_actions
 
 Example demonstration script
 ```python
 from selenium_profiles.webdriver import Chrome
 from selenium_profiles.profiles import profiles
 from selenium.webdriver.common.by import By
@@ -263,16 +257,14 @@
 
 ## Known Bugs
 
 - [click_as_touch makes automation hung](https://github.com/kaliiiiiiiiii/Selenium-Profiles/issues/1)
 
 
 ## Todo
-- [ ] use class instead of generator function at `selenium_profiles.webdriver.Chrome`
-- [ ] dynamic proxies [issue](https://github.com/kaliiiiiiiiii/Selenium-Profiles/issues/52)
 - [x] js-undetectability
   - [ ] [`navigator.connection`]
   - [ ] fonts don't match platform
   - [ ] does not match worker scope (Emulation) [crbug#1358491](https://bugs.chromium.org/p/chromium/issues/detail?id=1358491)
     - `Navigator.userAgent`
     - `Navigator.platform`
     - `navigator.hardwareConcurrency`
@@ -281,15 +273,14 @@
     - [ ] Either Devtools Console is open or CDP Runtime Domain is enabled => patch javascript objects using a Proxy or disable CDP.Runtime domain?
     - [ ] [document.$cdc_asdjflasutopfhvcZLmcfl_](https://source.chromium.org/chromium/chromium/src/+/main:chrome/test/chromedriver/js/call_function.js;l=219)
     - [ ] [`document.$chrome_asyncScriptInfo`](https://source.chromium.org/chromium/chromium/src/+/main:chrome/test/chromedriver/chrome/web_view_impl.cc;l=1586-1597;drc=2e14a3ac178ee87aa9154e5a15dcd986af1b6059)
     - [ ] driver.execute_script() usage (needs hook on called element)
     - [ ] driver.execute_async_script() usage (needs hook on called element)
     - [ ] driver.find_element() usage
     - [x] [`window.cdc_adoQpoasnfa76pfcZLmcfl`](https://source.chromium.org/chromium/chromium/src/+/main:chrome/test/chromedriver/chrome/devtools_client_impl.cc;l=526-532;drc=f915006bb8e09e0c29016cf9ab9e737cdebc1adc)
-- [x] allow passing seleniumwire-options => [discussion](https://github.com/kaliiiiiiiiii/Selenium-Profiles/discussions/36)
 - [x] default metrics
   - [x] Android
   - [x] Windows
   - [ ] IOS
   - [ ] Linux
   - [ ] Tablet
 - [ ] test.py script
@@ -299,19 +290,14 @@
         - [x] useragent-data
         - [ ] undetected
           - [ ] headless
       - [x] Android
        - [x] useragent-data
        - [ ] undetected
          - [ ] headless
-- [ ] [audio_captcha_solver](https://github.com/najmi9/solve-recaptcha-python-selenium/blob/master/main.py)
-- [X] support for 
-  - [x] Windows
-  - [x] Jupyter Notebook (Google-Colab)
-  - [x] Linux
 
 
 ## Deprecated
 
 * [Stealth method]((https://github.com/diprajpatra/selenium-stealth)) (Detected by Google)
 * [buster captcha solver](https://github.com/dessant/buster) | [wontfix](https://github.com/kaliiiiiiiiii/Selenium_Profiles/issues/3)
```

### Comparing `selenium_profiles-2.2.7.2/src/selenium_profiles.egg-info/SOURCES.txt` & `selenium_profiles-2.2.7.3/src/selenium_profiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `selenium_profiles-2.2.7.2/tests/test_driver.py` & `selenium_profiles-2.2.7.3/tests/test_driver.py`

 * *Files identical despite different names*

