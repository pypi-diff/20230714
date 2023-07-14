# Comparing `tmp/pyjd-1.0.6.tar.gz` & `tmp/pyjd-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjd-1.0.6.tar", last modified: Fri Jul  7 08:07:03 2023, max compression
+gzip compressed data, was "pyjd-1.0.7.tar", last modified: Mon Jul 10 09:33:25 2023, max compression
```

## Comparing `pyjd-1.0.6.tar` & `pyjd-1.0.7.tar`

### file list

```diff
@@ -1,36 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:07:03.027970 pyjd-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-07 08:06:51.000000 pyjd-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-07 08:07:03.027970 pyjd-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-07 08:06:51.000000 pyjd-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:07:03.027970 pyjd-1.0.6/pyjd/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/captcha.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/content.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/direct_connection_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/direct_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/jd_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19038 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/jd_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/linkgrabber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/myjd_connection_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    16630 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/myjd_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/polling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-07 08:06:51.000000 pyjd-1.0.6/pyjd/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:07:03.027970 pyjd-1.0.6/pyjd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-07 08:07:03.000000 pyjd-1.0.6/pyjd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 08:07:03.000000 pyjd-1.0.6/pyjd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:07:03.000000 pyjd-1.0.6/pyjd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-07 08:07:03.000000 pyjd-1.0.6/pyjd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 08:07:03.000000 pyjd-1.0.6/pyjd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 08:07:03.027970 pyjd-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-07 08:06:51.000000 pyjd-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:33:25.631484 pyjd-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-10 09:33:17.000000 pyjd-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-10 09:33:25.627484 pyjd-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-10 09:33:17.000000 pyjd-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:33:25.627484 pyjd-1.0.7/pyjd/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/captcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/direct_connection_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/direct_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14315 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/jd_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/jd_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/linkgrabber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/myjd_connection_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16630 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/myjd_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-10 09:33:17.000000 pyjd-1.0.7/pyjd/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:33:25.627484 pyjd-1.0.7/pyjd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-10 09:33:25.000000 pyjd-1.0.7/pyjd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-10 09:33:25.000000 pyjd-1.0.7/pyjd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 09:33:25.000000 pyjd-1.0.7/pyjd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-10 09:33:25.000000 pyjd-1.0.7/pyjd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 09:33:25.000000 pyjd-1.0.7/pyjd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 09:33:25.631484 pyjd-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-10 09:33:17.000000 pyjd-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 09:33:25.627484 pyjd-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-10 09:33:17.000000 pyjd-1.0.7/tests/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-10 09:33:17.000000 pyjd-1.0.7/tests/test_captcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-10 09:33:17.000000 pyjd-1.0.7/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-10 09:33:17.000000 pyjd-1.0.7/tests/test_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-10 09:33:17.000000 pyjd-1.0.7/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-10 09:33:17.000000 pyjd-1.0.7/tests/test_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-10 09:33:17.000000 pyjd-1.0.7/tests/test_downloads.py
```

### Comparing `pyjd-1.0.6/LICENSE` & `pyjd-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.6/PKG-INFO` & `pyjd-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjd
-Version: 1.0.6
+Version: 1.0.7
 Summary: A wapper for the JDownloader API
 Home-page: https://git.sr.ht/~pglaum/pyjd-api
 Author: Philipp Glaum
 Author-email: p@pglaum.de
 License: GPLv3
 Keywords: api jdownloader
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyjd-1.0.6/README.md` & `pyjd-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.6/pyjd/accounts.py` & `pyjd-1.0.7/pyjd/accounts.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.6/pyjd/captcha.py` & `pyjd-1.0.7/pyjd/captcha.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 class Captcha:
     def __init__(self, device: "JDDevice") -> None:
 
         self.device = device
         self.endpoint = "captcha"
 
-    def action(self, route: str, params: Optional[Any] = None, binary: bool = False) -> Any:
+    def action(
+        self, route: str, params: Optional[Any] = None, binary: bool = False
+    ) -> Any:
         route = f"/{self.endpoint}{route}"
         return self.device.connection_helper.action(route, params, binary=binary)
 
     def get(self, captcha_id: int, c_format: Optional[str] = None) -> str:
         """Get the base64 captcha image.
 
         The result is a captcha image as base64 encoded data url.
@@ -76,15 +78,17 @@
         :rtype: boolean
         """
 
         params = [captcha_id, skip_type.value]
         resp = self.action("/skip", params)
         return resp
 
-    def solve(self, captcha_id: int, result: str, result_format: Optional[str] = None) -> bool:
+    def solve(
+        self, captcha_id: int, result: str, result_format: Optional[str] = None
+    ) -> bool:
         """Solve a captcha.
 
         :param captcha_id: The ID of the captcha that is solved.
         :type captcha_id: int
         :param result: The solution of the captcha.
         :type result: str
         :param result_format: Format of the result
```

### Comparing `pyjd-1.0.6/pyjd/config.py` & `pyjd-1.0.7/pyjd/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self.device = device
         self.endpoint = "config"
 
     def action(self, route: str, params: Optional[Any] = None) -> Any:
         route = f"/{self.endpoint}{route}"
         return self.device.connection_helper.action(route, params)
 
-    def get(self, interface_name: str, storage: str, key: str) -> Any:
+    def get(self, interface_name: str, storage: Optional[str], key: str) -> Any:
         """Get value from interface by key.
 
         :param interface_name: The name of the JDownloader interface
         :type interface_name: str
         :param storage: The storage for the config entry.
             (None, for normal settings, or the extensions name for extension
             settings)
```

### Comparing `pyjd-1.0.6/pyjd/content.py` & `pyjd-1.0.7/pyjd/content.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.6/pyjd/device.py` & `pyjd-1.0.7/pyjd/device.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.6/pyjd/direct_connection_helper.py` & `pyjd-1.0.7/pyjd/direct_connection_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,10 +40,10 @@
         if binary:
             return requests.get(rurl + rparams).content
 
         rstr = requests.get(rurl + rparams).content.decode()
         robj = json.loads(rstr)
 
         if "data" in robj:
-            robj = robj["data"]
+            return robj["data"]
 
         return robj
```

### Comparing `pyjd-1.0.6/pyjd/direct_connector.py` & `pyjd-1.0.7/pyjd/direct_connector.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.6/pyjd/downloads.py` & `pyjd-1.0.7/pyjd/downloads.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 
     def action(self, route: str, params: Optional[Any] = None) -> Any:
         route = f"/{self.endpoint}{route}"
         return self.device.connection_helper.action(route, params)
 
     def cleanup(
         self,
-        link_ids: List[int],
-        package_ids: List[int],
-        delete_action: DeleteAction,
-        mode: Mode,
-        selection_type: SelectionType,
-    ) -> Any:
+        link_ids: List[int] = [],
+        package_ids: List[int] = [],
+        delete_action: DeleteAction = DeleteAction.DELETE_DISABLED,
+        mode: Mode = Mode.REMOVE_LINKS_ONLY,
+        selection_type: SelectionType = SelectionType.ALL,
+    ) -> bool:
         """Cleanup the link_ids & package_ids in the download list.
 
         :param link_ids: Link IDs that are used
         :type link_ids: List[int]
         :param package_ids: Package IDs that are used
         :type package_ids: List[int]
         :param action: The class:`jd_types.DeleteAction` that will be performed
@@ -50,17 +50,21 @@
             link_ids,
             package_ids,
             delete_action.value,
             mode.value,
             selection_type.value,
         ]
         resp = self.action("/cleanup", params)
-        return resp
+        if resp == "":
+            return True
+        return False
 
-    def force_download(self, link_ids: List[int], package_ids: List[int]) -> bool:
+    def force_download(
+        self, link_ids: List[int] = [], package_ids: List[int] = []
+    ) -> bool:
         """Force downloads for link_ids and package_ids.
 
         :param link_ids: Link IDs that are used
         :type link_ids: List[int]
         :param package_ids: Package IDs that are used
         :type package_ids: List[int]
         :returns: Success
@@ -68,17 +72,20 @@
         """
 
         params = [link_ids, package_ids]
         resp = self.action("/forceDownload", params)
         return resp
 
     def get_download_urls(
-        self, link_ids: List[int], package_ids: List[int], url_display_type: List[str]
+        self,
+        link_ids: List[int] = [],
+        package_ids: List[int] = [],
+        url_display_type: List[str] = ["ORIGIN"],
     ) -> Dict[str, List[int]]:
-        """Force downloads for link_ids and package_ids.
+        """Get the download urls for link_ids and package_ids.
 
         :param link_ids: Link IDs that are used
         :type link_ids: List[int]
         :param package_ids: Package IDs that are used
         :type package_ids: List[int]
         :param url_display_type: The type of urls that should be returned.
             Example: ['ORIGIN']
@@ -114,30 +121,33 @@
 
         if resp:
             download_link = DownloadLink(**resp)
             return download_link
 
         return None
 
-    def get_structure_change_counter(self, old_counter_value: int) -> int:
+    def get_structure_change_counter(self, old_counter_value: int = 0) -> int:
         """Get the structure change counter.
 
         Update the application layout, if the structure_change_counter is
         higher than the last.
 
         :returns: Structure change counter, or -1 if there is no newer change.
         :rtype: int
         """
 
         params = [old_counter_value]
         resp = self.action("/getStructureChangeCounter", params)
         return resp
 
     def move_links(
-        self, link_ids: List[int], after_link_id: int, dest_package_id: int
+        self,
+        link_ids: List[int] = [],
+        after_link_id: int = -1,
+        dest_package_id: int = -1,
     ) -> Any:
         """Move links to a package.
 
         :param link_ids: Link IDs that are used
         :type link_ids: List[int]
         :param after_link_id: ?
         :type after_link_id: int
@@ -147,15 +157,17 @@
         :rtype: Any
         """
 
         params = [link_ids, after_link_id, dest_package_id]
         resp = self.action("/moveLinks", params)
         return resp
 
-    def move_packages(self, package_ids: List[int], after_dest_package_id: int) -> Any:
+    def move_packages(
+        self, package_ids: List[int] = [], after_dest_package_id: int = -1
+    ) -> Any:
         """Move packages.
 
         :param package_ids: Package IDs that are used
         :type package_ids: List[int]
         :param after_dest_package_id: ?
         :type after_dest_package_id: int
         :returns: resp
@@ -164,18 +176,18 @@
 
         params = [package_ids, after_dest_package_id]
         resp = self.action("/movePackages", params)
         return resp
 
     def move_to_new_package(
         self,
-        link_ids: List[int],
-        pkg_ids: List[int],
-        new_pkg_name: str,
-        download_path: str,
+        link_ids: List[int] = [],
+        pkg_ids: List[int] = [],
+        new_pkg_name: str = "",
+        download_path: str = "",
     ) -> Any:
         """Move link_ids and pkg_ids to a new package
 
         :param link_ids: Link IDs that are used
         :type link_ids: List[int]
         :param package_ids: Package IDs that are used
         :type package_ids: List[int]
@@ -239,15 +251,17 @@
         download_packages = []
         for package in resp:
             download_package = FilePackage(**package)
             download_packages.append(download_package)
 
         return download_packages
 
-    def remove_links(self, link_ids: List[int], package_ids: List[int]) -> None:
+    def remove_links(
+        self, link_ids: List[int] = [], package_ids: List[int] = []
+    ) -> None:
         """Remove links/packages from download list.
 
         :param link_ids: Link IDs that are used
         :type link_ids: List[int]
         :param package_ids: Package IDs that are used
         :type package_ids: List[int]
         """
@@ -256,78 +270,84 @@
         self.action("/removeLinks", params)
 
     def remove_stop_mark(self) -> None:
         """Remove the stop mark."""
 
         self.action("/removeStopMark")
 
-    def rename_link(self, link: int, new_name: str) -> None:
+    def rename_link(self, link: int = -1, new_name: str = "") -> None:
         """Rename a link.
 
         :param link: The ID of the link
         :type link: int
         :param new_name: The new name for the link
         :type new_name: str
         """
 
         params = [link, new_name]
         self.action("/renameLink", params)
 
-    def rename_package(self, package_id: str, new_name: str) -> None:
+    def rename_package(self, package_id: str = "", new_name: str = "") -> None:
         """Rename a package.
 
         :param package_id: ID of the packages
         :type package_id: int
         :param new_name: New name for the package
         :type new_name: str
         """
 
         params = [package_id, new_name]
         resp = self.action("/renamePackage", params)
         return resp
 
-    def reset_links(self, link_ids: List[int], package_ids: List[int]) -> None:
+    def reset_links(
+        self, link_ids: List[int] = [], package_ids: List[int] = []
+    ) -> None:
         """Reset links/packages in the download list.
 
         :param link_ids: Link IDs that are used
         :type link_ids: List[int]
         :param package_ids: Package IDs that are used
         :type package_ids: List[int]
         """
 
         params = [link_ids, package_ids]
         self.action("/resetLinks", params)
 
-    def resume_links(self, link_ids: List[int], package_ids: List[int]) -> None:
+    def resume_links(
+        self, link_ids: List[int] = [], package_ids: List[int] = []
+    ) -> None:
         """Resume links/packages.
 
         :param link_ids: Link IDs that are used
         :type link_ids: List[int]
         :param package_ids: Package IDs that are used
         :type package_ids: List[int]
         """
 
         params = [link_ids, package_ids]
         self.action("/resumeLinks", params)
 
-    def set_download_directory(self, directory: str, package_ids: List[int]) -> None:
+    def set_download_directory(
+        self, directory: str = "", package_ids: List[int] = []
+    ) -> None:
         """Set the download directory for a packages.
 
         :param directory: Path of the download directory
         :type directory: str
         :param package_ids: List of package IDs that are changed.
         :type package_ids: List[int]
         """
 
         params = [directory, package_ids]
         resp = self.action("/setDownloadDirectory", params)
         return resp
 
     def set_download_password(
-        self, link_ids: List[int], package_ids: List[int], password: str
+        self, link_ids: List[int] = [], package_ids: List[int] = [], password: str = ""
     ) -> bool:
         """Set the download password for links/packages.
 
         :param link_ids: Link IDs that are used
         :type link_ids: List[int]
         :param package_ids: List of package IDs that are changed.
         :type package_ids: List[int]
@@ -338,15 +358,18 @@
         """
 
         params = [link_ids, package_ids, password]
         resp = self.action("/setDownloadPassword", params)
         return resp
 
     def set_enabled(
-        self, enabled: bool, link_ids: List[int], package_ids: List[int]
+        self,
+        enabled: bool = True,
+        link_ids: List[int] = [],
+        package_ids: List[int] = [],
     ) -> bool:
         """Enable/disable links and packages.
 
         :param enabled: Enable on or off
         :type enabled: bool
         :param link_ids: Link IDs that are used
         :type link_ids: List[int]
@@ -355,73 +378,81 @@
         """
 
         params = [enabled, link_ids, package_ids]
         resp = self.action("/setEnabled", params)
         return resp
 
     def set_priority(
-        self, priority: Priority, link_ids: List[int], package_ids: List[int]
+        self,
+        priority: Priority = Priority.DEFAULT,
+        link_ids: List[int] = [],
+        package_ids: List[int] = [],
     ) -> None:
         """Set the priority for links and packages.
 
         :param priority: The priority for the links/packages.
         :type priority: Priority
         :param link_ids: Link IDs that are used
         :type link_ids: List[int]
         :param package_ids: List of package IDs that are changed.
         :type package_ids: List[int]
         """
 
         params = [priority.value, link_ids, package_ids]
         self.action("/setPriority", params)
 
-    def set_stop_mark(self, link_id: Optional[int] = None, package_id: Optional[int] = None) -> None:
+    def set_stop_mark(
+        self, link_id: Optional[int] = None, package_id: Optional[int] = None
+    ) -> None:
         """Set the stop mark to the specified id.
 
         Only one of link_id and package_id has to be given.
 
         :param link_id: A link id for the stop mark
         :type link_id: int
         :param package_id: A package id for the stop mark
         :type package_id: int
         """
 
         params = [link_id, package_id]
         self.action("/setStopMark", params)
 
     def split_package_by_hoster(
-        self, link_ids: List[int], package_ids: List[int]
+        self, link_ids: List[int] = [], package_ids: List[int] = []
     ) -> None:
         """Split the packages/links by hoster.
 
         :param link_ids: Link IDs that are used
         :type link_ids: List[int]
         :param package_ids: List of package IDs that are changed.
         :type package_ids: List[int]
         """
 
         params = [link_ids, package_ids]
         self.action("/splitPackageByHoster", params)
 
     def start_online_status_check(
-        self, link_ids: List[int], package_ids: List[int]
+        self, link_ids: List[int] = [], package_ids: List[int] = []
     ) -> None:
         """Start an online status check for links and packages.
 
         :param link_ids: Link IDs that are used
         :type link_ids: List[int]
         :param package_ids: List of package IDs that are changed.
         :type package_ids: List[int]
         """
 
         params = [link_ids, package_ids]
         self.action("/startOnlineStatusCheck", params)
 
     def unskip(
-        self, link_ids: List[int], package_ids: List[int], filter_by_reason: Reason
+        self,
+        link_ids: List[int] = [],
+        package_ids: List[int] = [],
+        filter_by_reason: Reason = Reason.DISK_FULL,
     ) -> bool:
         """Un-skip links and packages
 
         :param package_ids: List of package IDs that are changed.
         :type package_ids: List[int]
         :param link_ids: Link IDs that are used
         :type link_ids: List[int]
```

### Comparing `pyjd-1.0.6/pyjd/events.py` & `pyjd-1.0.7/pyjd/events.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.6/pyjd/extensions.py` & `pyjd-1.0.7/pyjd/extensions.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.6/pyjd/jd_device.py` & `pyjd-1.0.7/pyjd/jd_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .accounts import Accounts
 from .captcha import Captcha
 from .config import Config
 from .content import Content
+from .dialogs import Dialogs
 from .device import Device
 from .downloads import Downloads
 from .events import Events
 from .extensions import Extensions
 from .linkgrabber import LinkGrabber
 from .log import Log
 from .plugins import Plugins
@@ -38,14 +39,15 @@
         self.connector = connector
         self.connection_helper = connection_helper(self)
 
         self.accounts = Accounts(self)
         self.captcha = Captcha(self)
         self.config = Config(self)
         self.content = Content(self)
+        self.dialogs = Dialogs(self)
         self.device = Device(self)
         self.downloads = Downloads(self)
         self.events = Events(self)
         self.extensions = Extensions(self)
         self.linkgrabber = LinkGrabber(self)
         self.log = Log(self)
         self.plugins = Plugins(self)
```

### Comparing `pyjd-1.0.6/pyjd/jd_types.py` & `pyjd-1.0.7/pyjd/jd_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 For more information, see here:
     https://my.jdownloader.org/developers/index.html#tag_342
 """
 
 from __future__ import annotations
 
 from enum import Enum
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 from typing import Any, List, Optional
 
 
 #
 # enums and constants
 #
 
@@ -469,14 +469,30 @@
             priority=True,
             saveTo=True,
             startAt=0,
             status=True,
         )
 
 
+class DialogInfo(BaseModel):
+    properties: Optional[dict[str, str]]
+    type: Optional[str]
+
+    def __repr__(self):
+        return f"<DialogInfo ({self.type})>"
+
+
+class DialogTypeInfo(BaseModel):
+    in_: Optional[dict[str, str]] = Field(..., alias="in")
+    out: Optional[dict[str, str]]
+
+    def __repr__(self):
+        return "<DialogTypeInfo>"
+
+
 class DownloadLink(BaseModel):
 
     addedDate: Optional[int]
     bytesLoaded: Optional[int]
     bytesTotal: Optional[int]
     comment: Optional[str]
     downloadPassword: Optional[str]
```

### Comparing `pyjd-1.0.6/pyjd/linkgrabber.py` & `pyjd-1.0.7/pyjd/linkgrabber.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.6/pyjd/log.py` & `pyjd-1.0.7/pyjd/log.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.6/pyjd/myjd_connection_helper.py` & `pyjd-1.0.7/pyjd/myjd_connection_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,22 +110,26 @@
             # No direct connection available, use the MyJD API
             response = self.device.connector.request_api(
                 path, http_action, params, action_url, binary=binary
             )
 
             if response is None:
                 return None
+            elif binary:
+                return response
             else:
                 if (
                     self.__direct_connection_enabled
                     and time.time() >= self.__direct_connection_cooldown
                 ):
                     self.__refresh_direct_connections()
 
-                return response["data"]
+                if "data" in response:
+                    return response["data"]
+                return response
 
         else:
 
             # A direct connection is available, try to use it
             for conn in self.__direct_connection_info:
 
                 if time.time() > conn["cooldown"]:
@@ -134,28 +138,31 @@
                     connection = conn["conn"]
                     api = f'http://{connection["ip"]}:{connection["port"]}'
 
                     response = self.device.connector.request_api(
                         path, http_action, params, action_url, api, binary=binary
                     )
 
-                    if response is not None:
+                    if response is None:
+                        # Don't try this connection for a minute.
+                        conn["cooldown"] = time.time() + 60
+
+                    elif binary:
+                        return response
 
+                    else:
                         # This connection worked, push it to the top of the
                         # list.
                         self.__direct_connection_info.remove(conn)
                         self.__direct_connection_info.insert(0, conn)
                         self.__direct_connection_consecutive_failures = 0
 
-                        return response["data"]
-
-                    else:
-
-                        # Don't try this connection for a minute.
-                        conn["cooldown"] = time.time() + 60
+                        if "data" in response:
+                            return response["data"]
+                        return response
 
             # None of the direct connections worked, set a cooldown for all
             # direct connections
             self.__direct_connection_consecutive_failures += 1
             self.__direct_connection_cooldown = int(
                 time.time() + (60 * self.__direct_connection_consecutive_failures)
             )
@@ -166,15 +173,17 @@
             )
 
             if response is None:
                 return None
 
             self.__refresh_direct_connections()
 
-            return response["data"]
+            if "data" in response:
+                return response["data"]
+            return response
 
     def __action_url(self) -> str:
         """Generate the action url for the device and session."""
 
         return (
             "/t_"
             + self.device.connector.get_session_token()
```

### Comparing `pyjd-1.0.6/pyjd/myjd_connector.py` & `pyjd-1.0.7/pyjd/myjd_connector.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.6/pyjd/plugins.py` & `pyjd-1.0.7/pyjd/plugins.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.6/pyjd/polling.py` & `pyjd-1.0.7/pyjd/polling.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.6/pyjd/system.py` & `pyjd-1.0.7/pyjd/system.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.6/pyjd/toolbar.py` & `pyjd-1.0.7/pyjd/toolbar.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.6/pyjd/ui.py` & `pyjd-1.0.7/pyjd/ui.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.6/pyjd/update.py` & `pyjd-1.0.7/pyjd/update.py`

 * *Files identical despite different names*

### Comparing `pyjd-1.0.6/pyjd.egg-info/PKG-INFO` & `pyjd-1.0.7/pyjd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjd
-Version: 1.0.6
+Version: 1.0.7
 Summary: A wapper for the JDownloader API
 Home-page: https://git.sr.ht/~pglaum/pyjd-api
 Author: Philipp Glaum
 Author-email: p@pglaum.de
 License: GPLv3
 Keywords: api jdownloader
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyjd-1.0.6/setup.py` & `pyjd-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="pyjd",
-    version="1.0.6",
+    version="1.0.7",
     author="Philipp Glaum",
     author_email="p@pglaum.de",
     description=("A wapper for the JDownloader API"),
     license="GPLv3",
     keywords="api jdownloader",
     url="https://git.sr.ht/~pglaum/pyjd-api",
     packages=["pyjd"],
```

