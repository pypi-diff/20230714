# Comparing `tmp/nordvpn-tray-1.0.7.tar.gz` & `tmp/nordvpn-tray-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nordvpn-tray-1.0.7.tar", last modified: Thu Jul 13 22:56:11 2023, max compression
+gzip compressed data, was "nordvpn-tray-1.0.8.tar", last modified: Thu Jul 13 23:02:37 2023, max compression
```

## Comparing `nordvpn-tray-1.0.7.tar` & `nordvpn-tray-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 22:56:11.680185 nordvpn-tray-1.0.7/
--rw-rw-rw-   0        0        0    35823 2023-01-08 18:15:51.000000 nordvpn-tray-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     4531 2023-07-13 22:56:11.675166 nordvpn-tray-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3590 2023-07-13 22:56:08.000000 nordvpn-tray-1.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-13 22:56:11.681166 nordvpn-tray-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2517 2023-07-13 22:56:08.000000 nordvpn-tray-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 22:56:11.635003 nordvpn-tray-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-13 22:56:11.648133 nordvpn-tray-1.0.7/src/nordvpn_tray/
--rw-rw-rw-   0        0        0        0 2023-05-01 10:01:09.000000 nordvpn-tray-1.0.7/src/nordvpn_tray/__init__.py
--rw-rw-rw-   0        0        0     6342 2023-07-13 18:59:04.000000 nordvpn-tray-1.0.7/src/nordvpn_tray/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 22:56:11.671166 nordvpn-tray-1.0.7/src/nordvpn_tray/resources/
--rw-rw-rw-   0        0        0   119440 2023-05-01 20:17:36.000000 nordvpn-tray-1.0.7/src/nordvpn_tray/resources/nvt.ico
-drwxrwxrwx   0        0        0        0 2023-07-13 22:56:11.669166 nordvpn-tray-1.0.7/src/nordvpn_tray.egg-info/
--rw-rw-rw-   0        0        0     4531 2023-07-13 22:56:11.000000 nordvpn-tray-1.0.7/src/nordvpn_tray.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-07-13 22:56:11.000000 nordvpn-tray-1.0.7/src/nordvpn_tray.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 22:56:11.000000 nordvpn-tray-1.0.7/src/nordvpn_tray.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-13 22:56:11.000000 nordvpn-tray-1.0.7/src/nordvpn_tray.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-07-13 22:56:11.000000 nordvpn-tray-1.0.7/src/nordvpn_tray.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-13 22:56:11.000000 nordvpn-tray-1.0.7/src/nordvpn_tray.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 23:02:37.526793 nordvpn-tray-1.0.8/
+-rw-rw-rw-   0        0        0    35823 2023-01-08 18:15:51.000000 nordvpn-tray-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     4531 2023-07-13 23:02:37.521265 nordvpn-tray-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3590 2023-07-13 22:56:08.000000 nordvpn-tray-1.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 23:02:37.527793 nordvpn-tray-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2517 2023-07-13 23:02:18.000000 nordvpn-tray-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 23:02:37.481810 nordvpn-tray-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-13 23:02:37.494394 nordvpn-tray-1.0.8/src/nordvpn_tray/
+-rw-rw-rw-   0        0        0        0 2023-05-01 10:01:09.000000 nordvpn-tray-1.0.8/src/nordvpn_tray/__init__.py
+-rw-rw-rw-   0        0        0     6262 2023-07-13 23:02:04.000000 nordvpn-tray-1.0.8/src/nordvpn_tray/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 23:02:37.517403 nordvpn-tray-1.0.8/src/nordvpn_tray/resources/
+-rw-rw-rw-   0        0        0   119440 2023-05-01 20:17:36.000000 nordvpn-tray-1.0.8/src/nordvpn_tray/resources/nvt.ico
+drwxrwxrwx   0        0        0        0 2023-07-13 23:02:37.516265 nordvpn-tray-1.0.8/src/nordvpn_tray.egg-info/
+-rw-rw-rw-   0        0        0     4531 2023-07-13 23:02:37.000000 nordvpn-tray-1.0.8/src/nordvpn_tray.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-07-13 23:02:37.000000 nordvpn-tray-1.0.8/src/nordvpn_tray.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 23:02:37.000000 nordvpn-tray-1.0.8/src/nordvpn_tray.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-13 23:02:37.000000 nordvpn-tray-1.0.8/src/nordvpn_tray.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-07-13 23:02:37.000000 nordvpn-tray-1.0.8/src/nordvpn_tray.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-13 23:02:37.000000 nordvpn-tray-1.0.8/src/nordvpn_tray.egg-info/top_level.txt
```

### Comparing `nordvpn-tray-1.0.7/LICENSE` & `nordvpn-tray-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nordvpn-tray-1.0.7/PKG-INFO` & `nordvpn-tray-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nordvpn-tray
-Version: 1.0.7
+Version: 1.0.8
 Summary: A cross-platform system tray application for interacting with NordVPN.
 Home-page: https://github.com/aviolaris/nordvpn-tray
 Author: Andreas Violaris
 Keywords: nord,nordvpn,nordvpn-tray,nordvpn_tray,vpn,vpn-client,tray,python,pypi,python3,tray,tray-application,pypi-package,tray-app
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `nordvpn-tray-1.0.7/README.md` & `nordvpn-tray-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `nordvpn-tray-1.0.7/setup.py` & `nordvpn-tray-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     long_description = f.read()
 
 with open('requirements.txt', encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='nordvpn-tray',
-    version='1.0.7',
+    version='1.0.8',
     packages=find_namespace_packages(where="src"),
     package_dir={"": "src"},
     package_data={
         "nordvpn_tray": ["*.py"],
         "nordvpn_tray.resources": ["*.ico"],
     },
     description='A cross-platform system tray application for interacting with NordVPN.',
```

### Comparing `nordvpn-tray-1.0.7/src/nordvpn_tray/__main__.py` & `nordvpn-tray-1.0.8/src/nordvpn_tray/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,16 +137,15 @@
         for country_submenu_flag in sorted(country_submenus_flags):
             country, submenu, flag = country_submenu_flag
             country_item = pystray.MenuItem(f"{country} ({flag})", submenu)
             country_items.append(country_item)
         continent_menu = pystray.Menu(*country_items)
         menu_items.append(pystray.MenuItem(continent, continent_menu))
 
-    menu_items.append(pystray.MenuItem('- - - -', None))
-    menu_items.append(pystray.Menu.SEPARATOR)  # Add separator here
+    menu_items.append(pystray.Menu.SEPARATOR)
     menu_items.append(pystray.MenuItem("Disconnect", create_disconnect_callback()))
     menu_items.append(pystray.MenuItem("Quit", quit))
 
     menu = pystray.Menu(*menu_items)
 
     tray = Icon("NordVPN Tray")
     tray.icon = Image.open(pkg_resources.resource_filename(__name__, 'resources/nvt.ico'))
```

### Comparing `nordvpn-tray-1.0.7/src/nordvpn_tray/resources/nvt.ico` & `nordvpn-tray-1.0.8/src/nordvpn_tray/resources/nvt.ico`

 * *Files identical despite different names*

### Comparing `nordvpn-tray-1.0.7/src/nordvpn_tray.egg-info/PKG-INFO` & `nordvpn-tray-1.0.8/src/nordvpn_tray.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nordvpn-tray
-Version: 1.0.7
+Version: 1.0.8
 Summary: A cross-platform system tray application for interacting with NordVPN.
 Home-page: https://github.com/aviolaris/nordvpn-tray
 Author: Andreas Violaris
 Keywords: nord,nordvpn,nordvpn-tray,nordvpn_tray,vpn,vpn-client,tray,python,pypi,python3,tray,tray-application,pypi-package,tray-app
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Microsoft :: Windows
```

