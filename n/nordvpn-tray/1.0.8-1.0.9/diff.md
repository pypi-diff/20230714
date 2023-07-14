# Comparing `tmp/nordvpn-tray-1.0.8.tar.gz` & `tmp/nordvpn-tray-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nordvpn-tray-1.0.8.tar", last modified: Thu Jul 13 23:02:37 2023, max compression
+gzip compressed data, was "nordvpn-tray-1.0.9.tar", last modified: Fri Jul 14 20:10:05 2023, max compression
```

## Comparing `nordvpn-tray-1.0.8.tar` & `nordvpn-tray-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 23:02:37.526793 nordvpn-tray-1.0.8/
--rw-rw-rw-   0        0        0    35823 2023-01-08 18:15:51.000000 nordvpn-tray-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     4531 2023-07-13 23:02:37.521265 nordvpn-tray-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3590 2023-07-13 22:56:08.000000 nordvpn-tray-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-13 23:02:37.527793 nordvpn-tray-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2517 2023-07-13 23:02:18.000000 nordvpn-tray-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:02:37.481810 nordvpn-tray-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-13 23:02:37.494394 nordvpn-tray-1.0.8/src/nordvpn_tray/
--rw-rw-rw-   0        0        0        0 2023-05-01 10:01:09.000000 nordvpn-tray-1.0.8/src/nordvpn_tray/__init__.py
--rw-rw-rw-   0        0        0     6262 2023-07-13 23:02:04.000000 nordvpn-tray-1.0.8/src/nordvpn_tray/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:02:37.517403 nordvpn-tray-1.0.8/src/nordvpn_tray/resources/
--rw-rw-rw-   0        0        0   119440 2023-05-01 20:17:36.000000 nordvpn-tray-1.0.8/src/nordvpn_tray/resources/nvt.ico
-drwxrwxrwx   0        0        0        0 2023-07-13 23:02:37.516265 nordvpn-tray-1.0.8/src/nordvpn_tray.egg-info/
--rw-rw-rw-   0        0        0     4531 2023-07-13 23:02:37.000000 nordvpn-tray-1.0.8/src/nordvpn_tray.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-07-13 23:02:37.000000 nordvpn-tray-1.0.8/src/nordvpn_tray.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 23:02:37.000000 nordvpn-tray-1.0.8/src/nordvpn_tray.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-13 23:02:37.000000 nordvpn-tray-1.0.8/src/nordvpn_tray.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-07-13 23:02:37.000000 nordvpn-tray-1.0.8/src/nordvpn_tray.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-13 23:02:37.000000 nordvpn-tray-1.0.8/src/nordvpn_tray.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 20:10:05.762169 nordvpn-tray-1.0.9/
+-rw-rw-rw-   0        0        0    35823 2023-01-08 18:15:51.000000 nordvpn-tray-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4793 2023-07-14 20:10:05.755059 nordvpn-tray-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3798 2023-07-14 11:12:39.000000 nordvpn-tray-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-14 20:10:05.762169 nordvpn-tray-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2568 2023-07-14 07:30:21.000000 nordvpn-tray-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:10:05.711010 nordvpn-tray-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 20:10:05.724521 nordvpn-tray-1.0.9/src/nordvpn_tray/
+-rw-rw-rw-   0        0        0        0 2023-05-01 10:01:09.000000 nordvpn-tray-1.0.9/src/nordvpn_tray/__init__.py
+-rw-rw-rw-   0        0        0     6262 2023-07-14 10:45:12.000000 nordvpn-tray-1.0.9/src/nordvpn_tray/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:10:05.750539 nordvpn-tray-1.0.9/src/nordvpn_tray/resources/
+-rw-rw-rw-   0        0        0   119440 2023-05-01 20:17:36.000000 nordvpn-tray-1.0.9/src/nordvpn_tray/resources/nvt.ico
+drwxrwxrwx   0        0        0        0 2023-07-14 20:10:05.747539 nordvpn-tray-1.0.9/src/nordvpn_tray.egg-info/
+-rw-rw-rw-   0        0        0     4793 2023-07-14 20:10:05.000000 nordvpn-tray-1.0.9/src/nordvpn_tray.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-07-14 20:10:05.000000 nordvpn-tray-1.0.9/src/nordvpn_tray.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 20:10:05.000000 nordvpn-tray-1.0.9/src/nordvpn_tray.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-14 20:10:05.000000 nordvpn-tray-1.0.9/src/nordvpn_tray.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-07-14 20:10:05.000000 nordvpn-tray-1.0.9/src/nordvpn_tray.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-14 20:10:05.000000 nordvpn-tray-1.0.9/src/nordvpn_tray.egg-info/top_level.txt
```

### Comparing `nordvpn-tray-1.0.8/LICENSE` & `nordvpn-tray-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nordvpn-tray-1.0.8/PKG-INFO` & `nordvpn-tray-1.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nordvpn-tray
-Version: 1.0.8
+Version: 1.0.9
 Summary: A cross-platform system tray application for interacting with NordVPN.
 Home-page: https://github.com/aviolaris/nordvpn-tray
 Author: Andreas Violaris
 Keywords: nord,nordvpn,nordvpn-tray,nordvpn_tray,vpn,vpn-client,tray,python,pypi,python3,tray,tray-application,pypi-package,tray-app
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NordVPN Tray
 
 ### A cross-platform system tray application for interacting with Nord VPN.
@@ -30,58 +31,70 @@
 [![license](https://img.shields.io/pypi/l/nordvpn-tray?color=blueviolet)](https://github.com/aviolaris/nordvpn-tray/blob/master/LICENSE)
 ![format](https://img.shields.io/pypi/format/nordvpn-tray?color=blueviolet)
 ![status](https://img.shields.io/pypi/status/nordvpn-tray?color=blue)
 [![GitHub Stars](https://img.shields.io/github/stars/aviolaris/nordvpn-tray?color=blue&logo=github&logoColor=white)](https://github.com/aviolaris/nordvpn-tray/stargazers)
 
 ## Description
 
-The official NordVPN clients for both Windows and Linux have well-known limitations. For instance, in Windows, to list all servers of a specific country, you must use a search pattern like ```country_name #```, while in Linux, it is not possible at all. Additionally, the official clients hide the server's load and external IP, even if you know its identification code.
-
-To address these limitations, the current project introduces a solution in the form of a system tray application. By placing an icon in the system tray, users can easily access a menu displaying the complete list of available NordVPN servers. The servers are conveniently categorized by continents and countries, allowing for effortless navigation. Moreover, the servers are ordered by their load, enabling users to select the server with the lowest load for optimal performance.
+The official NordVPN clients for both Windows and Linux have well-known limitations. For instance, in Windows, to list
+all servers of a specific country, you must use a search pattern like ```country_name #```, while in Linux, it is not
+possible at all. Furthermore, regardless of the platform, these clients do not provide essential information such as the
+server's load and external IP, even if the user has the corresponding identification code.
+
+To overcome these limitations, the current project expands the functionality of the official clients by introducing a
+solution in the form of a cross-platform system tray application. By placing an icon in the system tray, users can
+easily access a menu displaying the complete list of available NordVPN servers. The servers are conveniently categorized
+by continents and countries, allowing for effortless navigation. Moreover, they are ordered by their load, enabling
+users to select the server with the lowest load for optimal performance.
 
 ## Preview
 
 <img src="https://github.com/aviolaris/nordvpn-tray/assets/48277853/b4458286-efa2-4e0d-99e2-948d8df8aca8" alt="Preview" width="500">
 
 ## Requirements
 
-- Python 3.8 or higher
+- The official NordVPN client (available [here](https://nordvpn.com/download/))
 
 ## Installation
 
 To install NordVPN Tray, run the following command:
 
     pip install nordvpn-tray
 
 ## Usage
 
 To launch NordVPN Tray:
 
- - **On Windows**, double-click the `nordvpn-tray.exe` (usually located in `%LOCALAPPDATA%\Programs\Python\Python##\Scripts`) or run the `nordvpn-tray` command from the command prompt.
+- **On Windows**, double-click the `nordvpn-tray.exe` (usually located
+  in `%LOCALAPPDATA%\Programs\Python\Python##\Scripts`) or run the `nordvpn-tray` command from the command prompt.
 
 
- - **On Linux**, double-click the `nordvpn-tray` (usually located in `~/.local/bin`) or run the `./nordvpn-tray` command from the terminal.
+- **On Linux**, double-click the `nordvpn-tray` (usually located in `~/.local/bin`) or run the `./nordvpn-tray` command
+  from the terminal.
 
 ## Common Issues
 
 #### "ValueError: Namespace AppIndicator3 not available" (Linux Only)
 
-This error message indicates that the `AppIndicator3` module, which the application uses to display tray icons on Linux, is not available on your system.
+This error message indicates that the `AppIndicator3` module, which the application uses to display tray icons on Linux,
+is not available on your system.
 
-To resolve this issue, you will need to install the `libayatana-appindicator3-dev` package, which provides the necessary files and libraries for the `AppIndicator3` module. To install the package, use the following command:
+To resolve this issue, you will need to install the `libayatana-appindicator3-dev` package, which provides the necessary
+files and libraries for the `AppIndicator3` module. To install the package, use the following command:
 
     sudo apt-get install libayatana-appindicator3-dev
 
 ## Disclaimer
 
-All trademarks, logos and brand names are the property of their respective owners. All company and service names used in this repository are for identification purposes only. The use of NordVPN trademarks does not imply any endorsement, partnership, or sponsorship by Nordsec Ltd. 
+All trademarks, logos and brand names are the property of their respective owners. All company and service names used in
+this repository are for identification purposes only. The use of NordVPN trademarks does not imply any endorsement,
+partnership, or sponsorship by Nordsec Ltd.
 
 ## Contribution
 
 Pull requests and issues are welcome.
 
 ## License
 
 This project is licensed under the GNU General Public License v3.0.
 
 See the [LICENSE](https://github.com/aviolaris/nordvpn-tray/blob/master/LICENSE) file for details.
-
```

### Comparing `nordvpn-tray-1.0.8/README.md` & `nordvpn-tray-1.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,58 +10,70 @@
 [![license](https://img.shields.io/pypi/l/nordvpn-tray?color=blueviolet)](https://github.com/aviolaris/nordvpn-tray/blob/master/LICENSE)
 ![format](https://img.shields.io/pypi/format/nordvpn-tray?color=blueviolet)
 ![status](https://img.shields.io/pypi/status/nordvpn-tray?color=blue)
 [![GitHub Stars](https://img.shields.io/github/stars/aviolaris/nordvpn-tray?color=blue&logo=github&logoColor=white)](https://github.com/aviolaris/nordvpn-tray/stargazers)
 
 ## Description
 
-The official NordVPN clients for both Windows and Linux have well-known limitations. For instance, in Windows, to list all servers of a specific country, you must use a search pattern like ```country_name #```, while in Linux, it is not possible at all. Additionally, the official clients hide the server's load and external IP, even if you know its identification code.
-
-To address these limitations, the current project introduces a solution in the form of a system tray application. By placing an icon in the system tray, users can easily access a menu displaying the complete list of available NordVPN servers. The servers are conveniently categorized by continents and countries, allowing for effortless navigation. Moreover, the servers are ordered by their load, enabling users to select the server with the lowest load for optimal performance.
+The official NordVPN clients for both Windows and Linux have well-known limitations. For instance, in Windows, to list
+all servers of a specific country, you must use a search pattern like ```country_name #```, while in Linux, it is not
+possible at all. Furthermore, regardless of the platform, these clients do not provide essential information such as the
+server's load and external IP, even if the user has the corresponding identification code.
+
+To overcome these limitations, the current project expands the functionality of the official clients by introducing a
+solution in the form of a cross-platform system tray application. By placing an icon in the system tray, users can
+easily access a menu displaying the complete list of available NordVPN servers. The servers are conveniently categorized
+by continents and countries, allowing for effortless navigation. Moreover, they are ordered by their load, enabling
+users to select the server with the lowest load for optimal performance.
 
 ## Preview
 
 <img src="https://github.com/aviolaris/nordvpn-tray/assets/48277853/b4458286-efa2-4e0d-99e2-948d8df8aca8" alt="Preview" width="500">
 
 ## Requirements
 
-- Python 3.8 or higher
+- The official NordVPN client (available [here](https://nordvpn.com/download/))
 
 ## Installation
 
 To install NordVPN Tray, run the following command:
 
     pip install nordvpn-tray
 
 ## Usage
 
 To launch NordVPN Tray:
 
- - **On Windows**, double-click the `nordvpn-tray.exe` (usually located in `%LOCALAPPDATA%\Programs\Python\Python##\Scripts`) or run the `nordvpn-tray` command from the command prompt.
+- **On Windows**, double-click the `nordvpn-tray.exe` (usually located
+  in `%LOCALAPPDATA%\Programs\Python\Python##\Scripts`) or run the `nordvpn-tray` command from the command prompt.
 
 
- - **On Linux**, double-click the `nordvpn-tray` (usually located in `~/.local/bin`) or run the `./nordvpn-tray` command from the terminal.
+- **On Linux**, double-click the `nordvpn-tray` (usually located in `~/.local/bin`) or run the `./nordvpn-tray` command
+  from the terminal.
 
 ## Common Issues
 
 #### "ValueError: Namespace AppIndicator3 not available" (Linux Only)
 
-This error message indicates that the `AppIndicator3` module, which the application uses to display tray icons on Linux, is not available on your system.
+This error message indicates that the `AppIndicator3` module, which the application uses to display tray icons on Linux,
+is not available on your system.
 
-To resolve this issue, you will need to install the `libayatana-appindicator3-dev` package, which provides the necessary files and libraries for the `AppIndicator3` module. To install the package, use the following command:
+To resolve this issue, you will need to install the `libayatana-appindicator3-dev` package, which provides the necessary
+files and libraries for the `AppIndicator3` module. To install the package, use the following command:
 
     sudo apt-get install libayatana-appindicator3-dev
 
 ## Disclaimer
 
-All trademarks, logos and brand names are the property of their respective owners. All company and service names used in this repository are for identification purposes only. The use of NordVPN trademarks does not imply any endorsement, partnership, or sponsorship by Nordsec Ltd. 
+All trademarks, logos and brand names are the property of their respective owners. All company and service names used in
+this repository are for identification purposes only. The use of NordVPN trademarks does not imply any endorsement,
+partnership, or sponsorship by Nordsec Ltd.
 
 ## Contribution
 
 Pull requests and issues are welcome.
 
 ## License
 
 This project is licensed under the GNU General Public License v3.0.
 
-See the [LICENSE](https://github.com/aviolaris/nordvpn-tray/blob/master/LICENSE) file for details.
-
+See the [LICENSE](https://github.com/aviolaris/nordvpn-tray/blob/master/LICENSE) file for details.
```

### Comparing `nordvpn-tray-1.0.8/setup.py` & `nordvpn-tray-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     long_description = f.read()
 
 with open('requirements.txt', encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='nordvpn-tray',
-    version='1.0.8',
+    version='1.0.9',
     packages=find_namespace_packages(where="src"),
     package_dir={"": "src"},
     package_data={
         "nordvpn_tray": ["*.py"],
         "nordvpn_tray.resources": ["*.ico"],
     },
     description='A cross-platform system tray application for interacting with NordVPN.',
@@ -54,10 +54,11 @@
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX :: Linux',
         'Operating System :: MacOS',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
     ],
 )
```

### Comparing `nordvpn-tray-1.0.8/src/nordvpn_tray/__main__.py` & `nordvpn-tray-1.0.9/src/nordvpn_tray/__main__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,18 +32,14 @@
     country_name = country_converter.convert(names=country_code, to='name_short')
     if country_name:
         return f"{country_name} #{short_domain_identifier[2:]}"
     else:
         return "Invalid country code"
 
 
-def quit(icon, item):
-    icon.stop()
-
-
 def is_nordvpn_connected():
     user_info_data = requests.get(
         b'\x68\x74\x74\x70\x73\x3a\x2f\x2f\x6e\x6f\x72\x64\x76\x70\x6e\x2e\x63\x6f'
         b'\x6d\x2f\x77\x70\x2d\x61\x64\x6d\x69\x6e\x2f\x61\x64\x6d\x69\x6e\x2d\x61'
         b'\x6a\x61\x78\x2e\x70\x68\x70\x3f\x61\x63\x74\x69\x6f\x6e\x3d\x67\x65\x74'
         b'\x5f\x75\x73\x65\x72\x5f\x69\x6e\x66\x6f\x5f\x64\x61\x74\x61',
         timeout=10)
@@ -82,14 +78,18 @@
             subprocess.run(command, shell=True)
         else:
             icon.notify("You are not connected to a NordVPN server.")
 
     return callback
 
 
+def quit(icon, item):
+    icon.stop()
+
+
 def main():
     country_converter = CountryConverter()
 
     nord_api = requests.get(
         b'\x68\x74\x74\x70\x73\x3a\x2f\x2f\x61\x70\x69\x2e\x6e\x6f\x72'
         b'\x64\x76\x70\x6e\x2e\x63\x6f\x6d\x2f\x73\x65\x72\x76\x65\x72',
         timeout=10)
```

### Comparing `nordvpn-tray-1.0.8/src/nordvpn_tray/resources/nvt.ico` & `nordvpn-tray-1.0.9/src/nordvpn_tray/resources/nvt.ico`

 * *Files identical despite different names*

### Comparing `nordvpn-tray-1.0.8/src/nordvpn_tray.egg-info/PKG-INFO` & `nordvpn-tray-1.0.9/src/nordvpn_tray.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nordvpn-tray
-Version: 1.0.8
+Version: 1.0.9
 Summary: A cross-platform system tray application for interacting with NordVPN.
 Home-page: https://github.com/aviolaris/nordvpn-tray
 Author: Andreas Violaris
 Keywords: nord,nordvpn,nordvpn-tray,nordvpn_tray,vpn,vpn-client,tray,python,pypi,python3,tray,tray-application,pypi-package,tray-app
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NordVPN Tray
 
 ### A cross-platform system tray application for interacting with Nord VPN.
@@ -30,58 +31,70 @@
 [![license](https://img.shields.io/pypi/l/nordvpn-tray?color=blueviolet)](https://github.com/aviolaris/nordvpn-tray/blob/master/LICENSE)
 ![format](https://img.shields.io/pypi/format/nordvpn-tray?color=blueviolet)
 ![status](https://img.shields.io/pypi/status/nordvpn-tray?color=blue)
 [![GitHub Stars](https://img.shields.io/github/stars/aviolaris/nordvpn-tray?color=blue&logo=github&logoColor=white)](https://github.com/aviolaris/nordvpn-tray/stargazers)
 
 ## Description
 
-The official NordVPN clients for both Windows and Linux have well-known limitations. For instance, in Windows, to list all servers of a specific country, you must use a search pattern like ```country_name #```, while in Linux, it is not possible at all. Additionally, the official clients hide the server's load and external IP, even if you know its identification code.
-
-To address these limitations, the current project introduces a solution in the form of a system tray application. By placing an icon in the system tray, users can easily access a menu displaying the complete list of available NordVPN servers. The servers are conveniently categorized by continents and countries, allowing for effortless navigation. Moreover, the servers are ordered by their load, enabling users to select the server with the lowest load for optimal performance.
+The official NordVPN clients for both Windows and Linux have well-known limitations. For instance, in Windows, to list
+all servers of a specific country, you must use a search pattern like ```country_name #```, while in Linux, it is not
+possible at all. Furthermore, regardless of the platform, these clients do not provide essential information such as the
+server's load and external IP, even if the user has the corresponding identification code.
+
+To overcome these limitations, the current project expands the functionality of the official clients by introducing a
+solution in the form of a cross-platform system tray application. By placing an icon in the system tray, users can
+easily access a menu displaying the complete list of available NordVPN servers. The servers are conveniently categorized
+by continents and countries, allowing for effortless navigation. Moreover, they are ordered by their load, enabling
+users to select the server with the lowest load for optimal performance.
 
 ## Preview
 
 <img src="https://github.com/aviolaris/nordvpn-tray/assets/48277853/b4458286-efa2-4e0d-99e2-948d8df8aca8" alt="Preview" width="500">
 
 ## Requirements
 
-- Python 3.8 or higher
+- The official NordVPN client (available [here](https://nordvpn.com/download/))
 
 ## Installation
 
 To install NordVPN Tray, run the following command:
 
     pip install nordvpn-tray
 
 ## Usage
 
 To launch NordVPN Tray:
 
- - **On Windows**, double-click the `nordvpn-tray.exe` (usually located in `%LOCALAPPDATA%\Programs\Python\Python##\Scripts`) or run the `nordvpn-tray` command from the command prompt.
+- **On Windows**, double-click the `nordvpn-tray.exe` (usually located
+  in `%LOCALAPPDATA%\Programs\Python\Python##\Scripts`) or run the `nordvpn-tray` command from the command prompt.
 
 
- - **On Linux**, double-click the `nordvpn-tray` (usually located in `~/.local/bin`) or run the `./nordvpn-tray` command from the terminal.
+- **On Linux**, double-click the `nordvpn-tray` (usually located in `~/.local/bin`) or run the `./nordvpn-tray` command
+  from the terminal.
 
 ## Common Issues
 
 #### "ValueError: Namespace AppIndicator3 not available" (Linux Only)
 
-This error message indicates that the `AppIndicator3` module, which the application uses to display tray icons on Linux, is not available on your system.
+This error message indicates that the `AppIndicator3` module, which the application uses to display tray icons on Linux,
+is not available on your system.
 
-To resolve this issue, you will need to install the `libayatana-appindicator3-dev` package, which provides the necessary files and libraries for the `AppIndicator3` module. To install the package, use the following command:
+To resolve this issue, you will need to install the `libayatana-appindicator3-dev` package, which provides the necessary
+files and libraries for the `AppIndicator3` module. To install the package, use the following command:
 
     sudo apt-get install libayatana-appindicator3-dev
 
 ## Disclaimer
 
-All trademarks, logos and brand names are the property of their respective owners. All company and service names used in this repository are for identification purposes only. The use of NordVPN trademarks does not imply any endorsement, partnership, or sponsorship by Nordsec Ltd. 
+All trademarks, logos and brand names are the property of their respective owners. All company and service names used in
+this repository are for identification purposes only. The use of NordVPN trademarks does not imply any endorsement,
+partnership, or sponsorship by Nordsec Ltd.
 
 ## Contribution
 
 Pull requests and issues are welcome.
 
 ## License
 
 This project is licensed under the GNU General Public License v3.0.
 
 See the [LICENSE](https://github.com/aviolaris/nordvpn-tray/blob/master/LICENSE) file for details.
-
```

