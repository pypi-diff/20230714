# Comparing `tmp/python-owasp-zap-v2.4-0.0.8.tar.gz` & `tmp/python-owasp-zap-v2.4-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-owasp-zap-v2.4-0.0.8.tar", last modified: Fri Jun  3 13:21:42 2016, max compression
+gzip compressed data, was "dist/python-owasp-zap-v2.4-0.0.9.tar", last modified: Mon Mar 27 15:16:21 2017, max compression
```

## Comparing `python-owasp-zap-v2.4-0.0.8.tar` & `python-owasp-zap-v2.4-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2016-06-03 13:21:42.000000 python-owasp-zap-v2.4-0.0.8/
--rw-rw-r--   0 simon     (1000) simon     (1000)     1223 2016-06-03 13:07:37.000000 python-owasp-zap-v2.4-0.0.8/setup.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2016-06-03 13:21:42.000000 python-owasp-zap-v2.4-0.0.8/src/
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2016-06-03 13:21:42.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/
--rw-rw-r--   0 simon     (1000) simon     (1000)     3063 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/pscan.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     6138 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/search.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     2680 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/selenium.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     5564 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/autoupdate.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     3031 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/pnh.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     2975 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/script.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     4778 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/__init__.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     2688 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/importLogFiles.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     1378 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/reveal.py
--rw-rw-r--   0 simon     (1000) simon     (1000)    17111 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/ascan.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     4613 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/stats.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     1701 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/brk.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     1910 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/acsrf.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     1177 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/params.py
--rw-rw-r--   0 simon     (1000) simon     (1000)    13025 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/spider.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     4456 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/httpSessions.py
--rw-rw-r--   0 simon     (1000) simon     (1000)    16977 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/core.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     3229 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/users.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     8486 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/ajaxSpider.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     2262 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/authorization.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     6354 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/context.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     2039 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/forcedUser.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     1924 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/sessionManagement.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     2906 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.8/src/zapv2/authentication.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2016-06-03 13:21:42.000000 python-owasp-zap-v2.4-0.0.8/src/python_owasp_zap_v2.4.egg-info/
--rw-r--r--   0 simon     (1000) root         (0)        6 2016-06-03 13:21:42.000000 python-owasp-zap-v2.4-0.0.8/src/python_owasp_zap_v2.4.egg-info/top_level.txt
--rw-r--r--   0 simon     (1000) root         (0)      818 2016-06-03 13:21:42.000000 python-owasp-zap-v2.4-0.0.8/src/python_owasp_zap_v2.4.egg-info/PKG-INFO
--rw-r--r--   0 simon     (1000) root         (0)        1 2016-06-03 13:21:42.000000 python-owasp-zap-v2.4-0.0.8/src/python_owasp_zap_v2.4.egg-info/dependency_links.txt
--rw-r--r--   0 simon     (1000) root         (0)      728 2016-06-03 13:21:42.000000 python-owasp-zap-v2.4-0.0.8/src/python_owasp_zap_v2.4.egg-info/SOURCES.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)       59 2016-06-03 13:21:42.000000 python-owasp-zap-v2.4-0.0.8/setup.cfg
--rw-rw-r--   0 simon     (1000) simon     (1000)      818 2016-06-03 13:21:42.000000 python-owasp-zap-v2.4-0.0.8/PKG-INFO
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2017-03-27 15:16:21.000000 python-owasp-zap-v2.4-0.0.9/
+-rwxrwxr-x   0 simon     (1000) simon     (1000)     1477 2017-03-27 15:13:47.000000 python-owasp-zap-v2.4-0.0.9/setup.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2017-03-27 15:16:21.000000 python-owasp-zap-v2.4-0.0.9/src/
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2017-03-27 15:16:21.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3723 2017-03-27 13:37:40.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/pscan.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     6138 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/search.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3916 2017-03-27 13:37:40.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/selenium.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     7194 2017-03-27 13:37:40.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/autoupdate.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3031 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/pnh.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2975 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/script.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     5563 2017-03-27 15:13:47.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/__init__.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2784 2017-03-27 13:37:40.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/importLogFiles.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1378 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/reveal.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)    22471 2017-03-27 13:37:40.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/ascan.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     4613 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/stats.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     4532 2017-03-27 13:37:40.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/brk.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1910 2017-03-27 13:37:40.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/acsrf.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1177 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/params.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)    17144 2017-03-27 13:37:40.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/spider.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     4663 2016-09-29 09:39:29.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/httpSessions.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)    21869 2017-03-27 13:37:40.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/core.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3229 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/users.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     9548 2017-03-27 13:37:40.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/ajaxSpider.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2262 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/authorization.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     6354 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/context.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2039 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/forcedUser.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1924 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/sessionManagement.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2906 2016-06-03 12:37:51.000000 python-owasp-zap-v2.4-0.0.9/src/zapv2/authentication.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2017-03-27 15:16:21.000000 python-owasp-zap-v2.4-0.0.9/src/python_owasp_zap_v2.4.egg-info/
+-rw-rw-r--   0 simon     (1000) simon     (1000)       51 2017-03-27 15:16:21.000000 python-owasp-zap-v2.4-0.0.9/src/python_owasp_zap_v2.4.egg-info/requires.txt
+-rw-r--r--   0 simon     (1000) root         (0)        6 2017-03-27 15:16:21.000000 python-owasp-zap-v2.4-0.0.9/src/python_owasp_zap_v2.4.egg-info/top_level.txt
+-rw-r--r--   0 simon     (1000) root         (0)      818 2017-03-27 15:16:21.000000 python-owasp-zap-v2.4-0.0.9/src/python_owasp_zap_v2.4.egg-info/PKG-INFO
+-rw-r--r--   0 simon     (1000) root         (0)        1 2017-03-27 15:16:21.000000 python-owasp-zap-v2.4-0.0.9/src/python_owasp_zap_v2.4.egg-info/dependency_links.txt
+-rw-r--r--   0 simon     (1000) root         (0)      776 2017-03-27 15:16:21.000000 python-owasp-zap-v2.4-0.0.9/src/python_owasp_zap_v2.4.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)       59 2017-03-27 15:16:21.000000 python-owasp-zap-v2.4-0.0.9/setup.cfg
+-rw-rw-r--   0 simon     (1000) simon     (1000)      818 2017-03-27 15:16:21.000000 python-owasp-zap-v2.4-0.0.9/PKG-INFO
```

### Comparing `python-owasp-zap-v2.4-0.0.8/setup.py` & `python-owasp-zap-v2.4-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,23 +9,32 @@
 try:
     from setuptools import setup, find_packages
 except ImportError:
     print "You must have setuptools installed to use setup.py. Exiting..."
     raise SystemExit(1)
 
 
+install_dependencies = (
+    'requests'
+)
+test_requirements = (
+    'mock',
+    'pylama',
+    'pytest',
+    'requests_mock'
+)
 setup(
     name="python-owasp-zap-v2.4",
-    version="0.0.8",
-    description="OWASP ZAP 2.5 API client",
-    long_description="OWASP Zed Attack Proxy 2.5 API python client (the 2.4 package name has been kept to make it easier to upgrade)",
+    version="0.0.9",
+    description="OWASP ZAP 2.6 API client",
+    long_description="OWASP Zed Attack Proxy 2.6 API python client (the 2.4 package name has been kept to make it easier to upgrade)",
     author="ZAP development team",
     author_email='',
     url="https://www.owasp.org/index.php/OWASP_Zed_Attack_Proxy_Project",
-    download_url="https://github.com/zaproxy/zap-api-python/releases/tag/0.0.8",
+    download_url="https://github.com/zaproxy/zap-api-python/releases/tag/0.0.9",
     platforms=['any'],
 
     license="ASL2.0",
 
     package_dir={
         '': 'src',
     },
@@ -35,8 +44,11 @@
         'License :: OSI Approved :: Apache Software License',
         'Development Status :: 5 - Production/Stable',
         'Topic :: Security',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
         'Programming Language :: Python'],
+    install_requires=install_dependencies,
+    tests_require=test_requirements,
+    extras_require={'tests': test_requirements}
 )
```

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/pscan.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/pscan.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,14 +21,21 @@
 
 class pscan(object):
 
     def __init__(self, zap):
         self.zap = zap
 
     @property
+    def scan_only_in_scope(self):
+        """
+        Tells whether or not the passive scan should be performed only on messages that are in scope.
+        """
+        return next(self.zap._request(self.zap.base + 'pscan/view/scanOnlyInScope/').itervalues())
+
+    @property
     def records_to_scan(self):
         """
         The number of records the passive scanner still has to scan
         """
         return next(self.zap._request(self.zap.base + 'pscan/view/recordsToScan/').itervalues())
 
     @property
@@ -36,18 +43,24 @@
         """
         Lists all passive scanners with its ID, name, enabled state and alert threshold.
         """
         return next(self.zap._request(self.zap.base + 'pscan/view/scanners/').itervalues())
 
     def set_enabled(self, enabled, apikey=''):
         """
-        Sets whether or not the passive scanning is enabled
+        Sets whether or not the passive scanning is enabled (Note: the enabled state is not persisted).
         """
         return next(self.zap._request(self.zap.base + 'pscan/action/setEnabled/', {'enabled' : enabled, 'apikey' : apikey}).itervalues())
 
+    def set_scan_only_in_scope(self, onlyinscope, apikey=''):
+        """
+        Sets whether or not the passive scan should be performed only on messages that are in scope.
+        """
+        return next(self.zap._request(self.zap.base + 'pscan/action/setScanOnlyInScope/', {'onlyInScope' : onlyinscope, 'apikey' : apikey}).itervalues())
+
     def enable_all_scanners(self, apikey=''):
         """
         Enables all passive scanners
         """
         return next(self.zap._request(self.zap.base + 'pscan/action/enableAllScanners/', {'apikey' : apikey}).itervalues())
 
     def disable_all_scanners(self, apikey=''):
```

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/search.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/search.py`

 * *Files identical despite different names*

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/selenium.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/selenium.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,14 +28,28 @@
     def option_chrome_driver_path(self):
         """
         This component is optional and therefore the API will only work if it is installed
         """
         return next(self.zap._request(self.zap.base + 'selenium/view/optionChromeDriverPath/').itervalues())
 
     @property
+    def option_firefox_binary_path(self):
+        """
+        This component is optional and therefore the API will only work if it is installed
+        """
+        return next(self.zap._request(self.zap.base + 'selenium/view/optionFirefoxBinaryPath/').itervalues())
+
+    @property
+    def option_firefox_driver_path(self):
+        """
+        This component is optional and therefore the API will only work if it is installed
+        """
+        return next(self.zap._request(self.zap.base + 'selenium/view/optionFirefoxDriverPath/').itervalues())
+
+    @property
     def option_ie_driver_path(self):
         """
         This component is optional and therefore the API will only work if it is installed
         """
         return next(self.zap._request(self.zap.base + 'selenium/view/optionIeDriverPath/').itervalues())
 
     @property
@@ -47,14 +61,26 @@
 
     def set_option_chrome_driver_path(self, string, apikey=''):
         """
         This component is optional and therefore the API will only work if it is installed
         """
         return next(self.zap._request(self.zap.base + 'selenium/action/setOptionChromeDriverPath/', {'String' : string, 'apikey' : apikey}).itervalues())
 
+    def set_option_firefox_binary_path(self, string, apikey=''):
+        """
+        This component is optional and therefore the API will only work if it is installed
+        """
+        return next(self.zap._request(self.zap.base + 'selenium/action/setOptionFirefoxBinaryPath/', {'String' : string, 'apikey' : apikey}).itervalues())
+
+    def set_option_firefox_driver_path(self, string, apikey=''):
+        """
+        This component is optional and therefore the API will only work if it is installed
+        """
+        return next(self.zap._request(self.zap.base + 'selenium/action/setOptionFirefoxDriverPath/', {'String' : string, 'apikey' : apikey}).itervalues())
+
     def set_option_ie_driver_path(self, string, apikey=''):
         """
         This component is optional and therefore the API will only work if it is installed
         """
         return next(self.zap._request(self.zap.base + 'selenium/action/setOptionIeDriverPath/', {'String' : string, 'apikey' : apikey}).itervalues())
 
     def set_option_phantom_js_binary_path(self, string, apikey=''):
```

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/autoupdate.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/autoupdate.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,14 +35,42 @@
     def is_latest_version(self):
         """
         Returns 'true' if ZAP is on the latest version
         """
         return next(self.zap._request(self.zap.base + 'autoupdate/view/isLatestVersion/').itervalues())
 
     @property
+    def installed_addons(self):
+        """
+        Return a list of all of the installed add-ons
+        """
+        return next(self.zap._request(self.zap.base + 'autoupdate/view/installedAddons/').itervalues())
+
+    @property
+    def new_addons(self):
+        """
+        Return a list of any add-ons that have been added to the Marketplace since the last check for updates
+        """
+        return next(self.zap._request(self.zap.base + 'autoupdate/view/newAddons/').itervalues())
+
+    @property
+    def updated_addons(self):
+        """
+        Return a list of any add-ons that have been changed in the Marketplace since the last check for updates
+        """
+        return next(self.zap._request(self.zap.base + 'autoupdate/view/updatedAddons/').itervalues())
+
+    @property
+    def marketplace_addons(self):
+        """
+        Return a list of all of the add-ons on the ZAP Marketplace (this information is read once and then cached)
+        """
+        return next(self.zap._request(self.zap.base + 'autoupdate/view/marketplaceAddons/').itervalues())
+
+    @property
     def option_addon_directories(self):
         return next(self.zap._request(self.zap.base + 'autoupdate/view/optionAddonDirectories/').itervalues())
 
     @property
     def option_day_last_checked(self):
         return next(self.zap._request(self.zap.base + 'autoupdate/view/optionDayLastChecked/').itervalues())
 
@@ -92,14 +120,26 @@
 
     def download_latest_release(self, apikey=''):
         """
         Downloads the latest release, if any 
         """
         return next(self.zap._request(self.zap.base + 'autoupdate/action/downloadLatestRelease/', {'apikey' : apikey}).itervalues())
 
+    def install_addon(self, id, apikey=''):
+        """
+        Installs or updates the specified add-on, returning when complete (ie not asynchronously)
+        """
+        return next(self.zap._request(self.zap.base + 'autoupdate/action/installAddon/', {'id' : id, 'apikey' : apikey}).itervalues())
+
+    def uninstall_addon(self, id, apikey=''):
+        """
+        Uninstalls the specified add-on 
+        """
+        return next(self.zap._request(self.zap.base + 'autoupdate/action/uninstallAddon/', {'id' : id, 'apikey' : apikey}).itervalues())
+
     def set_option_check_addon_updates(self, boolean, apikey=''):
         return next(self.zap._request(self.zap.base + 'autoupdate/action/setOptionCheckAddonUpdates/', {'Boolean' : boolean, 'apikey' : apikey}).itervalues())
 
     def set_option_check_on_start(self, boolean, apikey=''):
         return next(self.zap._request(self.zap.base + 'autoupdate/action/setOptionCheckOnStart/', {'Boolean' : boolean, 'apikey' : apikey}).itervalues())
 
     def set_option_download_new_release(self, boolean, apikey=''):
```

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/pnh.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/pnh.py`

 * *Files identical despite different names*

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/script.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/script.py`

 * *Files identical despite different names*

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/__init__.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 # limitations under the License.
 """
 Client implementation for using the ZAP pentesting proxy remotely.
 """
 
 __docformat__ = 'restructuredtext'
 
-import json
-import urllib
+import requests
+from requests.packages.urllib3.exceptions import InsecureRequestWarning
+
 from acsrf import acsrf
 from ascan import ascan
 from ajaxSpider import ajaxSpider
 from authentication import authentication
 from authorization import authorization
 from autoupdate import autoupdate
 from brk import brk
@@ -43,44 +44,41 @@
 from search import search
 from selenium import selenium
 from sessionManagement import sessionManagement
 from spider import spider
 from stats import stats
 from users import users
 
-class ZapError(Exception):
-    """
-    Base ZAP exception.
-    """
-    pass
-
 
 class ZAPv2(object):
     """
     Client API implementation for integrating with ZAP v2.
     """
-
     # base JSON api url
     base = 'http://zap/JSON/'
+
     # base OTHER api url
     base_other = 'http://zap/OTHER/'
 
-    def __init__(self, proxies={'http': 'http://127.0.0.1:8080',
-        'https': 'http://127.0.0.1:8080'}):
+    def __init__(self, proxies=None, apikey=None):
         """
         Creates an instance of the ZAP api client.
 
         :Parameters:
            - `proxies`: dictionary of ZAP proxies to use.
-           
+
         Note that all of the other classes in this directory are generated
         new ones will need to be manually added to this file
         """
-        self.__proxies = proxies
-        
+        self.__proxies = proxies or {
+            'http': 'http://127.0.0.1:8080',
+            'https': 'http://127.0.0.1:8080'
+        }
+        self.__apikey = apikey
+
         self.acsrf = acsrf(self)
         self.ajaxSpider = ajaxSpider(self)
         self.ascan = ascan(self)
         self.authentication = authentication(self)
         self.authorization = authorization(self)
         self.autoupdate = autoupdate(self)
         self.brk = brk(self)
@@ -97,59 +95,71 @@
         self.search = search(self)
         self.selenium = selenium(self)
         self.sessionManagement = sessionManagement(self)
         self.spider = spider(self)
         self.stats = stats(self)
         self.users = users(self)
 
-    def _expect_ok(self, json_data):
-        """
-        Checks that we have an OK response, else raises an exception.
+        # not very nice, but prevents warnings when accessing the ZAP API via https
+        requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
 
-        :Parameters:
-           - `json_data`: the json data to look at.
-        """
-        if type(json_data) == type(list()) and json_data[0] == u'OK':
-            return json_data
-        raise ZapError(*json_data.values())
+        # Currently create a new session for each request to prevent request failing
+        # e.g. when polling the spider status
+        #self.session = requests.Session()
+        #if apikey is not None:
+        #  self.session.headers['X-ZAP-API-Key'] = apikey
 
     def urlopen(self, *args, **kwargs):
         """
         Opens a url forcing the proxies to be used.
 
         :Parameters:
            - `args`:  all non-keyword arguments.
            - `kwargs`: all other keyword arguments.
         """
-        kwargs['proxies'] = self.__proxies
-        return urllib.urlopen(*args, **kwargs).read()
+        # Must never leak the API key via proxied requests
+        return requests.get(*args, proxies=self.__proxies, verify=False, **kwargs).text
+
+    def _request_api(self, url, query=None):
+        """
+        Shortcut for an API request. Will always add the apikey (if defined)
 
-    def status_code(self, *args, **kwargs):
-      """
-      Open a url forcing the proxies to be used.
-
-      :Parameters:
-         - `args`: all non-keyword arguments.
-         - `kwargs`: all other keyword arguments.
-      """
-      kwargs['proxies'] = self.__proxies
-      return urllib.urlopen(*args, **kwargs).getcode()
+        :Parameters:
+           - `url`: the url to GET at.
+        """
+        if not url.startswith('http://zap/'):
+          # Only allow requests to the API so that we never leak the apikey
+          raise ValueError('A non ZAP API url was specified ' + url)
+          return;
+
+        # In theory we should be able to reuse the session,
+        # but there have been problems with that
+        self.session = requests.Session()
+        if self.__apikey is not None:
+          self.session.headers['X-ZAP-API-Key'] = self.__apikey
+
+        query = query or {}
+        if self.__apikey is not None:
+          # Add the apikey to get params for backwards compatibility
+          if not query.get('apikey'):
+            query['apikey'] = self.__apikey
+        return self.session.get(url, params=query, proxies=self.__proxies, verify=False)
 
-    def _request(self, url, get={}):
+    def _request(self, url, get=None):
         """
         Shortcut for a GET request.
 
         :Parameters:
            - `url`: the url to GET at.
-           - `get`: the disctionary to turn into GET variables.
+           - `get`: the dictionary to turn into GET variables.
         """
-        return json.loads(self.urlopen(url + '?' + urllib.urlencode(get)))
+        return self._request_api(url, get).json()
 
-    def _request_other(self, url, get={}):
+    def _request_other(self, url, get=None):
         """
         Shortcut for an API OTHER GET request.
 
         :Parameters:
            - `url`: the url to GET at.
-           - `get`: the disctionary to turn into GET variables.
+           - `get`: the dictionary to turn into GET variables.
         """
-        return self.urlopen(url + '?' + urllib.urlencode(get))
+        return self._request_api(url, get).text
```

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/importLogFiles.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/importLogFiles.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,31 +20,31 @@
 """
 
 class importLogFiles(object):
 
     def __init__(self, zap):
         self.zap = zap
 
-    def import_zap_log_from_file(self, filepath):
+    def import_zap_log_from_file(self, filepath, apikey=''):
         """
         This component is optional and therefore the API will only work if it is installed
         """
-        return next(self.zap._request(self.zap.base + 'importLogFiles/view/ImportZAPLogFromFile/', {'FilePath' : filepath}).itervalues())
+        return next(self.zap._request(self.zap.base + 'importLogFiles/action/ImportZAPLogFromFile/', {'FilePath' : filepath, 'apikey' : apikey}).itervalues())
 
-    def import_mod_security_log_from_file(self, filepath):
+    def import_mod_security_log_from_file(self, filepath, apikey=''):
         """
         This component is optional and therefore the API will only work if it is installed
         """
-        return next(self.zap._request(self.zap.base + 'importLogFiles/view/ImportModSecurityLogFromFile/', {'FilePath' : filepath}).itervalues())
+        return next(self.zap._request(self.zap.base + 'importLogFiles/action/ImportModSecurityLogFromFile/', {'FilePath' : filepath, 'apikey' : apikey}).itervalues())
 
-    def import_zap_http_request_response_pair(self, httprequest, httpresponse):
+    def import_zap_http_request_response_pair(self, httprequest, httpresponse, apikey=''):
         """
         This component is optional and therefore the API will only work if it is installed
         """
-        return next(self.zap._request(self.zap.base + 'importLogFiles/view/ImportZAPHttpRequestResponsePair/', {'HTTPRequest' : httprequest, 'HTTPResponse' : httpresponse}).itervalues())
+        return next(self.zap._request(self.zap.base + 'importLogFiles/action/ImportZAPHttpRequestResponsePair/', {'HTTPRequest' : httprequest, 'HTTPResponse' : httpresponse, 'apikey' : apikey}).itervalues())
 
     def post_mod_security_audit_event(self, auditeventstring=None, apikey=''):
         """
         This component is optional and therefore the API will only work if it is installed
         """
         params = {'apikey' : apikey}
         if auditeventstring is not None:
```

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/reveal.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/reveal.py`

 * *Files identical despite different names*

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/ascan.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/ascan.py`

 * *Files 23% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 
     @property
     def scan_policy_names(self):
         return next(self.zap._request(self.zap.base + 'ascan/view/scanPolicyNames/').itervalues())
 
     @property
     def excluded_from_scan(self):
+        """
+        Gets the regexes of URLs excluded from the active scans.
+        """
         return next(self.zap._request(self.zap.base + 'ascan/view/excludedFromScan/').itervalues())
 
     def scanners(self, scanpolicyname=None, policyid=None):
         params = {}
         if scanpolicyname is not None:
             params['scanPolicyName'] = scanpolicyname
         if policyid is not None:
@@ -71,30 +74,47 @@
         return next(self.zap._request(self.zap.base + 'ascan/view/policies/', params).itervalues())
 
     @property
     def attack_mode_queue(self):
         return next(self.zap._request(self.zap.base + 'ascan/view/attackModeQueue/').itervalues())
 
     @property
+    def excluded_params(self):
+        """
+        Gets all the parameters that are excluded. For each parameter the following are shown: the name, the URL, and the parameter type.
+        """
+        return next(self.zap._request(self.zap.base + 'ascan/view/excludedParams/').itervalues())
+
+    @property
+    def option_excluded_param_list(self):
+        """
+        Use view excludedParams instead.
+        """
+        return next(self.zap._request(self.zap.base + 'ascan/view/optionExcludedParamList/').itervalues())
+
+    @property
+    def excluded_param_types(self):
+        """
+        Gets all the types of excluded parameters. For each type the following are shown: the ID and the name.
+        """
+        return next(self.zap._request(self.zap.base + 'ascan/view/excludedParamTypes/').itervalues())
+
+    @property
     def option_attack_policy(self):
         return next(self.zap._request(self.zap.base + 'ascan/view/optionAttackPolicy/').itervalues())
 
     @property
     def option_default_policy(self):
         return next(self.zap._request(self.zap.base + 'ascan/view/optionDefaultPolicy/').itervalues())
 
     @property
     def option_delay_in_ms(self):
         return next(self.zap._request(self.zap.base + 'ascan/view/optionDelayInMs/').itervalues())
 
     @property
-    def option_excluded_param_list(self):
-        return next(self.zap._request(self.zap.base + 'ascan/view/optionExcludedParamList/').itervalues())
-
-    @property
     def option_handle_anti_csrf_tokens(self):
         return next(self.zap._request(self.zap.base + 'ascan/view/optionHandleAntiCSRFTokens/').itervalues())
 
     @property
     def option_host_per_scan(self):
         return next(self.zap._request(self.zap.base + 'ascan/view/optionHostPerScan/').itervalues())
 
@@ -103,14 +123,22 @@
         return next(self.zap._request(self.zap.base + 'ascan/view/optionMaxChartTimeInMins/').itervalues())
 
     @property
     def option_max_results_to_list(self):
         return next(self.zap._request(self.zap.base + 'ascan/view/optionMaxResultsToList/').itervalues())
 
     @property
+    def option_max_rule_duration_in_mins(self):
+        return next(self.zap._request(self.zap.base + 'ascan/view/optionMaxRuleDurationInMins/').itervalues())
+
+    @property
+    def option_max_scan_duration_in_mins(self):
+        return next(self.zap._request(self.zap.base + 'ascan/view/optionMaxScanDurationInMins/').itervalues())
+
+    @property
     def option_max_scans_in_ui(self):
         return next(self.zap._request(self.zap.base + 'ascan/view/optionMaxScansInUI/').itervalues())
 
     @property
     def option_target_params_enabled_rpc(self):
         return next(self.zap._request(self.zap.base + 'ascan/view/optionTargetParamsEnabledRPC/').itervalues())
 
@@ -124,14 +152,17 @@
 
     @property
     def option_allow_attack_on_start(self):
         return next(self.zap._request(self.zap.base + 'ascan/view/optionAllowAttackOnStart/').itervalues())
 
     @property
     def option_inject_plugin_id_in_header(self):
+        """
+        Tells whether or not the active scanner should inject the HTTP request header X-ZAP-Scan-ID, with the ID of the scanner that's sending the requests.
+        """
         return next(self.zap._request(self.zap.base + 'ascan/view/optionInjectPluginIdInHeader/').itervalues())
 
     @property
     def option_prompt_in_attack_mode(self):
         return next(self.zap._request(self.zap.base + 'ascan/view/optionPromptInAttackMode/').itervalues())
 
     @property
@@ -149,33 +180,46 @@
         """
         return next(self.zap._request(self.zap.base + 'ascan/view/optionScanHeadersAllRequests/').itervalues())
 
     @property
     def option_show_advanced_dialog(self):
         return next(self.zap._request(self.zap.base + 'ascan/view/optionShowAdvancedDialog/').itervalues())
 
-    def scan(self, url, recurse=None, inscopeonly=None, scanpolicyname=None, method=None, postdata=None, apikey=''):
-        params = {'url' : url, 'apikey' : apikey}
+    def scan(self, url=None, recurse=None, inscopeonly=None, scanpolicyname=None, method=None, postdata=None, contextid=None, apikey=''):
+        """
+        Runs the active scanner against the given URL and/or Context. Optionally, the 'recurse' parameter can be used to scan URLs under the given URL, the parameter 'inScopeOnly' can be used to constrain the scan to URLs that are in scope (ignored if a Context is specified), the parameter 'scanPolicyName' allows to specify the scan policy (if none is given it uses the default scan policy), the parameters 'method' and 'postData' allow to select a given request in conjunction with the given URL.
+        """
+        params = {'apikey' : apikey}
+        if url is not None:
+            params['url'] = url
         if recurse is not None:
             params['recurse'] = recurse
         if inscopeonly is not None:
             params['inScopeOnly'] = inscopeonly
         if scanpolicyname is not None:
             params['scanPolicyName'] = scanpolicyname
         if method is not None:
             params['method'] = method
         if postdata is not None:
             params['postData'] = postdata
+        if contextid is not None:
+            params['contextId'] = contextid
         return next(self.zap._request(self.zap.base + 'ascan/action/scan/', params).itervalues())
 
-    def scan_as_user(self, url, contextid, userid, recurse=None, scanpolicyname=None, method=None, postdata=None, apikey=''):
+    def scan_as_user(self, url=None, contextid=None, userid=None, recurse=None, scanpolicyname=None, method=None, postdata=None, apikey=''):
         """
         Active Scans from the perspective of a User, obtained using the given Context ID and User ID. See 'scan' action for more details.
         """
-        params = {'url' : url, 'contextId' : contextid, 'userId' : userid, 'apikey' : apikey}
+        params = {'apikey' : apikey}
+        if url is not None:
+            params['url'] = url
+        if contextid is not None:
+            params['contextId'] = contextid
+        if userid is not None:
+            params['userId'] = userid
         if recurse is not None:
             params['recurse'] = recurse
         if scanpolicyname is not None:
             params['scanPolicyName'] = scanpolicyname
         if method is not None:
             params['method'] = method
         if postdata is not None:
@@ -203,17 +247,23 @@
     def stop_all_scans(self, apikey=''):
         return next(self.zap._request(self.zap.base + 'ascan/action/stopAllScans/', {'apikey' : apikey}).itervalues())
 
     def remove_all_scans(self, apikey=''):
         return next(self.zap._request(self.zap.base + 'ascan/action/removeAllScans/', {'apikey' : apikey}).itervalues())
 
     def clear_excluded_from_scan(self, apikey=''):
+        """
+        Clears the regexes of URLs excluded from the active scans.
+        """
         return next(self.zap._request(self.zap.base + 'ascan/action/clearExcludedFromScan/', {'apikey' : apikey}).itervalues())
 
     def exclude_from_scan(self, regex, apikey=''):
+        """
+        Adds a regex of URLs that should be excluded from the active scans.
+        """
         return next(self.zap._request(self.zap.base + 'ascan/action/excludeFromScan/', {'regex' : regex, 'apikey' : apikey}).itervalues())
 
     def enable_all_scanners(self, scanpolicyname=None, apikey=''):
         params = {'apikey' : apikey}
         if scanpolicyname is not None:
             params['scanPolicyName'] = scanpolicyname
         return next(self.zap._request(self.zap.base + 'ascan/action/enableAllScanners/', params).itervalues())
@@ -262,20 +312,63 @@
 
     def set_scanner_alert_threshold(self, id, alertthreshold, scanpolicyname=None, apikey=''):
         params = {'id' : id, 'alertThreshold' : alertthreshold, 'apikey' : apikey}
         if scanpolicyname is not None:
             params['scanPolicyName'] = scanpolicyname
         return next(self.zap._request(self.zap.base + 'ascan/action/setScannerAlertThreshold/', params).itervalues())
 
-    def add_scan_policy(self, scanpolicyname, apikey=''):
-        return next(self.zap._request(self.zap.base + 'ascan/action/addScanPolicy/', {'scanPolicyName' : scanpolicyname, 'apikey' : apikey}).itervalues())
+    def add_scan_policy(self, scanpolicyname, alertthreshold=None, attackstrength=None, apikey=''):
+        params = {'scanPolicyName' : scanpolicyname, 'apikey' : apikey}
+        if alertthreshold is not None:
+            params['alertThreshold'] = alertthreshold
+        if attackstrength is not None:
+            params['attackStrength'] = attackstrength
+        return next(self.zap._request(self.zap.base + 'ascan/action/addScanPolicy/', params).itervalues())
 
     def remove_scan_policy(self, scanpolicyname, apikey=''):
         return next(self.zap._request(self.zap.base + 'ascan/action/removeScanPolicy/', {'scanPolicyName' : scanpolicyname, 'apikey' : apikey}).itervalues())
 
+    def update_scan_policy(self, scanpolicyname, alertthreshold=None, attackstrength=None, apikey=''):
+        params = {'scanPolicyName' : scanpolicyname, 'apikey' : apikey}
+        if alertthreshold is not None:
+            params['alertThreshold'] = alertthreshold
+        if attackstrength is not None:
+            params['attackStrength'] = attackstrength
+        return next(self.zap._request(self.zap.base + 'ascan/action/updateScanPolicy/', params).itervalues())
+
+    def add_excluded_param(self, name, type=None, url=None, apikey=''):
+        """
+        Adds a new parameter excluded from the scan, using the specified name. Optionally sets if the new entry applies to a specific URL (default, all URLs) and sets the ID of the type of the parameter (default, ID of any type). The type IDs can be obtained with the view excludedParamTypes. 
+        """
+        params = {'name' : name, 'apikey' : apikey}
+        if type is not None:
+            params['type'] = type
+        if url is not None:
+            params['url'] = url
+        return next(self.zap._request(self.zap.base + 'ascan/action/addExcludedParam/', params).itervalues())
+
+    def modify_excluded_param(self, idx, name=None, type=None, url=None, apikey=''):
+        """
+        Modifies a parameter excluded from the scan. Allows to modify the name, the URL and the type of parameter. The parameter is selected with its index, which can be obtained with the view excludedParams.
+        """
+        params = {'idx' : idx, 'apikey' : apikey}
+        if name is not None:
+            params['name'] = name
+        if type is not None:
+            params['type'] = type
+        if url is not None:
+            params['url'] = url
+        return next(self.zap._request(self.zap.base + 'ascan/action/modifyExcludedParam/', params).itervalues())
+
+    def remove_excluded_param(self, idx, apikey=''):
+        """
+        Removes a parameter excluded from the scan, with the given index. The index can be obtained with the view excludedParams.
+        """
+        return next(self.zap._request(self.zap.base + 'ascan/action/removeExcludedParam/', {'idx' : idx, 'apikey' : apikey}).itervalues())
+
     def set_option_attack_policy(self, string, apikey=''):
         return next(self.zap._request(self.zap.base + 'ascan/action/setOptionAttackPolicy/', {'String' : string, 'apikey' : apikey}).itervalues())
 
     def set_option_default_policy(self, string, apikey=''):
         return next(self.zap._request(self.zap.base + 'ascan/action/setOptionDefaultPolicy/', {'String' : string, 'apikey' : apikey}).itervalues())
 
     def set_option_allow_attack_on_start(self, boolean, apikey=''):
@@ -287,22 +380,31 @@
     def set_option_handle_anti_csrf_tokens(self, boolean, apikey=''):
         return next(self.zap._request(self.zap.base + 'ascan/action/setOptionHandleAntiCSRFTokens/', {'Boolean' : boolean, 'apikey' : apikey}).itervalues())
 
     def set_option_host_per_scan(self, integer, apikey=''):
         return next(self.zap._request(self.zap.base + 'ascan/action/setOptionHostPerScan/', {'Integer' : integer, 'apikey' : apikey}).itervalues())
 
     def set_option_inject_plugin_id_in_header(self, boolean, apikey=''):
+        """
+        Sets whether or not the active scanner should inject the HTTP request header X-ZAP-Scan-ID, with the ID of the scanner that's sending the requests.
+        """
         return next(self.zap._request(self.zap.base + 'ascan/action/setOptionInjectPluginIdInHeader/', {'Boolean' : boolean, 'apikey' : apikey}).itervalues())
 
     def set_option_max_chart_time_in_mins(self, integer, apikey=''):
         return next(self.zap._request(self.zap.base + 'ascan/action/setOptionMaxChartTimeInMins/', {'Integer' : integer, 'apikey' : apikey}).itervalues())
 
     def set_option_max_results_to_list(self, integer, apikey=''):
         return next(self.zap._request(self.zap.base + 'ascan/action/setOptionMaxResultsToList/', {'Integer' : integer, 'apikey' : apikey}).itervalues())
 
+    def set_option_max_rule_duration_in_mins(self, integer, apikey=''):
+        return next(self.zap._request(self.zap.base + 'ascan/action/setOptionMaxRuleDurationInMins/', {'Integer' : integer, 'apikey' : apikey}).itervalues())
+
+    def set_option_max_scan_duration_in_mins(self, integer, apikey=''):
+        return next(self.zap._request(self.zap.base + 'ascan/action/setOptionMaxScanDurationInMins/', {'Integer' : integer, 'apikey' : apikey}).itervalues())
+
     def set_option_max_scans_in_ui(self, integer, apikey=''):
         return next(self.zap._request(self.zap.base + 'ascan/action/setOptionMaxScansInUI/', {'Integer' : integer, 'apikey' : apikey}).itervalues())
 
     def set_option_prompt_in_attack_mode(self, boolean, apikey=''):
         return next(self.zap._request(self.zap.base + 'ascan/action/setOptionPromptInAttackMode/', {'Boolean' : boolean, 'apikey' : apikey}).itervalues())
 
     def set_option_prompt_to_clear_finished_scans(self, boolean, apikey=''):
```

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/stats.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/stats.py`

 * *Files identical despite different names*

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/acsrf.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/acsrf.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,30 +23,30 @@
 
     def __init__(self, zap):
         self.zap = zap
 
     @property
     def option_tokens_names(self):
         """
-        Lists the names of all anti CSRF tokens
+        Lists the names of all anti-CSRF tokens
         """
         return next(self.zap._request(self.zap.base + 'acsrf/view/optionTokensNames/').itervalues())
 
     def add_option_token(self, string, apikey=''):
         """
-        Adds an anti CSRF token with the given name, enabled by default
+        Adds an anti-CSRF token with the given name, enabled by default
         """
         return next(self.zap._request(self.zap.base + 'acsrf/action/addOptionToken/', {'String' : string, 'apikey' : apikey}).itervalues())
 
     def remove_option_token(self, string, apikey=''):
         """
-        Removes the anti CSRF token with the given name
+        Removes the anti-CSRF token with the given name
         """
         return next(self.zap._request(self.zap.base + 'acsrf/action/removeOptionToken/', {'String' : string, 'apikey' : apikey}).itervalues())
 
     def gen_form(self, hrefid, apikey=''):
         """
-        Generate a form for testing lack of anti CSRF tokens - typically invoked via ZAP
+        Generate a form for testing lack of anti-CSRF tokens - typically invoked via ZAP
         """
         return (self.zap._request_other(self.zap.base_other + 'acsrf/other/genForm/', {'hrefId' : hrefid, 'apikey' : apikey}))
```

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/params.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/params.py`

 * *Files identical despite different names*

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/spider.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/spider.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,29 +41,59 @@
 
     @property
     def scans(self):
         return next(self.zap._request(self.zap.base + 'spider/view/scans/').itervalues())
 
     @property
     def excluded_from_scan(self):
+        """
+        Gets the regexes of URLs excluded from the spider scans.
+        """
         return next(self.zap._request(self.zap.base + 'spider/view/excludedFromScan/').itervalues())
 
     @property
+    def all_urls(self):
+        """
+        Returns a list of unique URLs from the history table based on HTTP messages added by the Spider.
+        """
+        return next(self.zap._request(self.zap.base + 'spider/view/allUrls/').itervalues())
+
+    @property
+    def domains_always_in_scope(self):
+        """
+        Gets all the domains that are always in scope. For each domain the following are shown: the index, the value (domain), if enabled, and if specified as a regex.
+        """
+        return next(self.zap._request(self.zap.base + 'spider/view/domainsAlwaysInScope/').itervalues())
+
+    @property
     def option_domains_always_in_scope(self):
+        """
+        Use view domainsAlwaysInScope instead.
+        """
         return next(self.zap._request(self.zap.base + 'spider/view/optionDomainsAlwaysInScope/').itervalues())
 
     @property
     def option_domains_always_in_scope_enabled(self):
+        """
+        Use view domainsAlwaysInScope instead.
+        """
         return next(self.zap._request(self.zap.base + 'spider/view/optionDomainsAlwaysInScopeEnabled/').itervalues())
 
     @property
     def option_handle_parameters(self):
         return next(self.zap._request(self.zap.base + 'spider/view/optionHandleParameters/').itervalues())
 
     @property
+    def option_max_children(self):
+        """
+        Gets the maximum number of child nodes (per node) that can be crawled, 0 means no limit.
+        """
+        return next(self.zap._request(self.zap.base + 'spider/view/optionMaxChildren/').itervalues())
+
+    @property
     def option_max_depth(self):
         return next(self.zap._request(self.zap.base + 'spider/view/optionMaxDepth/').itervalues())
 
     @property
     def option_max_duration(self):
         return next(self.zap._request(self.zap.base + 'spider/view/optionMaxDuration/').itervalues())
 
@@ -126,15 +156,15 @@
     @property
     def option_process_form(self):
         return next(self.zap._request(self.zap.base + 'spider/view/optionProcessForm/').itervalues())
 
     @property
     def option_send_referer_header(self):
         """
-        Sets whether or not the 'Referer' header should be sent while spidering
+        Gets whether or not the 'Referer' header should be sent while spidering.
         """
         return next(self.zap._request(self.zap.base + 'spider/view/optionSendRefererHeader/').itervalues())
 
     @property
     def option_show_advanced_dialog(self):
         return next(self.zap._request(self.zap.base + 'spider/view/optionShowAdvancedDialog/').itervalues())
 
@@ -194,34 +224,91 @@
     def stop_all_scans(self, apikey=''):
         return next(self.zap._request(self.zap.base + 'spider/action/stopAllScans/', {'apikey' : apikey}).itervalues())
 
     def remove_all_scans(self, apikey=''):
         return next(self.zap._request(self.zap.base + 'spider/action/removeAllScans/', {'apikey' : apikey}).itervalues())
 
     def clear_excluded_from_scan(self, apikey=''):
+        """
+        Clears the regexes of URLs excluded from the spider scans.
+        """
         return next(self.zap._request(self.zap.base + 'spider/action/clearExcludedFromScan/', {'apikey' : apikey}).itervalues())
 
     def exclude_from_scan(self, regex, apikey=''):
+        """
+        Adds a regex of URLs that should be excluded from the spider scans.
+        """
         return next(self.zap._request(self.zap.base + 'spider/action/excludeFromScan/', {'regex' : regex, 'apikey' : apikey}).itervalues())
 
+    def add_domain_always_in_scope(self, value, isregex=None, isenabled=None, apikey=''):
+        """
+        Adds a new domain that's always in scope, using the specified value. Optionally sets if the new entry is enabled (default, true) and whether or not the new value is specified as a regex (default, false).
+        """
+        params = {'value' : value, 'apikey' : apikey}
+        if isregex is not None:
+            params['isRegex'] = isregex
+        if isenabled is not None:
+            params['isEnabled'] = isenabled
+        return next(self.zap._request(self.zap.base + 'spider/action/addDomainAlwaysInScope/', params).itervalues())
+
+    def modify_domain_always_in_scope(self, idx, value=None, isregex=None, isenabled=None, apikey=''):
+        """
+        Modifies a domain that's always in scope. Allows to modify the value, if enabled or if a regex. The domain is selected with its index, which can be obtained with the view domainsAlwaysInScope.
+        """
+        params = {'idx' : idx, 'apikey' : apikey}
+        if value is not None:
+            params['value'] = value
+        if isregex is not None:
+            params['isRegex'] = isregex
+        if isenabled is not None:
+            params['isEnabled'] = isenabled
+        return next(self.zap._request(self.zap.base + 'spider/action/modifyDomainAlwaysInScope/', params).itervalues())
+
+    def remove_domain_always_in_scope(self, idx, apikey=''):
+        """
+        Removes a domain that's always in scope, with the given index. The index can be obtained with the view domainsAlwaysInScope.
+        """
+        return next(self.zap._request(self.zap.base + 'spider/action/removeDomainAlwaysInScope/', {'idx' : idx, 'apikey' : apikey}).itervalues())
+
+    def enable_all_domains_always_in_scope(self, apikey=''):
+        """
+        Enables all domains that are always in scope.
+        """
+        return next(self.zap._request(self.zap.base + 'spider/action/enableAllDomainsAlwaysInScope/', {'apikey' : apikey}).itervalues())
+
+    def disable_all_domains_always_in_scope(self, apikey=''):
+        """
+        Disables all domains that are always in scope.
+        """
+        return next(self.zap._request(self.zap.base + 'spider/action/disableAllDomainsAlwaysInScope/', {'apikey' : apikey}).itervalues())
+
     def set_option_handle_parameters(self, string, apikey=''):
         return next(self.zap._request(self.zap.base + 'spider/action/setOptionHandleParameters/', {'String' : string, 'apikey' : apikey}).itervalues())
 
     def set_option_scope_string(self, string, apikey=''):
+        """
+        Use actions [add|modify|remove]DomainAlwaysInScope instead.
+        """
         return next(self.zap._request(self.zap.base + 'spider/action/setOptionScopeString/', {'String' : string, 'apikey' : apikey}).itervalues())
 
     def set_option_skip_url_string(self, string, apikey=''):
         return next(self.zap._request(self.zap.base + 'spider/action/setOptionSkipURLString/', {'String' : string, 'apikey' : apikey}).itervalues())
 
     def set_option_user_agent(self, string, apikey=''):
         return next(self.zap._request(self.zap.base + 'spider/action/setOptionUserAgent/', {'String' : string, 'apikey' : apikey}).itervalues())
 
     def set_option_handle_o_data_parameters_visited(self, boolean, apikey=''):
         return next(self.zap._request(self.zap.base + 'spider/action/setOptionHandleODataParametersVisited/', {'Boolean' : boolean, 'apikey' : apikey}).itervalues())
 
+    def set_option_max_children(self, integer, apikey=''):
+        """
+        Sets the maximum number of child nodes (per node) that can be crawled, 0 means no limit.
+        """
+        return next(self.zap._request(self.zap.base + 'spider/action/setOptionMaxChildren/', {'Integer' : integer, 'apikey' : apikey}).itervalues())
+
     def set_option_max_depth(self, integer, apikey=''):
         return next(self.zap._request(self.zap.base + 'spider/action/setOptionMaxDepth/', {'Integer' : integer, 'apikey' : apikey}).itervalues())
 
     def set_option_max_duration(self, integer, apikey=''):
         return next(self.zap._request(self.zap.base + 'spider/action/setOptionMaxDuration/', {'Integer' : integer, 'apikey' : apikey}).itervalues())
 
     def set_option_max_scans_in_ui(self, integer, apikey=''):
@@ -248,14 +335,17 @@
     def set_option_process_form(self, boolean, apikey=''):
         return next(self.zap._request(self.zap.base + 'spider/action/setOptionProcessForm/', {'Boolean' : boolean, 'apikey' : apikey}).itervalues())
 
     def set_option_request_wait_time(self, integer, apikey=''):
         return next(self.zap._request(self.zap.base + 'spider/action/setOptionRequestWaitTime/', {'Integer' : integer, 'apikey' : apikey}).itervalues())
 
     def set_option_send_referer_header(self, boolean, apikey=''):
+        """
+        Sets whether or not the 'Referer' header should be sent while spidering.
+        """
         return next(self.zap._request(self.zap.base + 'spider/action/setOptionSendRefererHeader/', {'Boolean' : boolean, 'apikey' : apikey}).itervalues())
 
     def set_option_show_advanced_dialog(self, boolean, apikey=''):
         return next(self.zap._request(self.zap.base + 'spider/action/setOptionShowAdvancedDialog/', {'Boolean' : boolean, 'apikey' : apikey}).itervalues())
 
     def set_option_thread_count(self, integer, apikey=''):
         return next(self.zap._request(self.zap.base + 'spider/action/setOptionThreadCount/', {'Integer' : integer, 'apikey' : apikey}).itervalues())
```

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/httpSessions.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/httpSessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,24 @@
 """
 
 class httpSessions(object):
 
     def __init__(self, zap):
         self.zap = zap
 
+    @property
+    def sites(self):
+        """
+        Gets all of the sites that have sessions.
+        """
+        return next(self.zap._request(self.zap.base + 'httpSessions/view/sites/').itervalues())
+
     def sessions(self, site, session=None):
         """
-        Gets the sessions of the given site. Optionally returning just the session with the given name.
+        Gets the sessions for the given site. Optionally returning just the session with the given name.
         """
         params = {'site' : site}
         if session is not None:
             params['session'] = session
         return next(self.zap._request(self.zap.base + 'httpSessions/view/sessions/', params).itervalues())
 
     def active_session(self, site):
```

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/core.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -123,18 +123,60 @@
         return next(self.zap._request(self.zap.base + 'core/view/excludedFromProxy/').itervalues())
 
     @property
     def home_directory(self):
         return next(self.zap._request(self.zap.base + 'core/view/homeDirectory/').itervalues())
 
     @property
+    def session_location(self):
+        """
+        Gets the location of the current session file
+        """
+        return next(self.zap._request(self.zap.base + 'core/view/sessionLocation/').itervalues())
+
+    @property
+    def proxy_chain_excluded_domains(self):
+        """
+        Gets all the domains that are excluded from the outgoing proxy. For each domain the following are shown: the index, the value (domain), if enabled, and if specified as a regex.
+        """
+        return next(self.zap._request(self.zap.base + 'core/view/proxyChainExcludedDomains/').itervalues())
+
+    @property
+    def option_proxy_chain_skip_name(self):
+        """
+        Use view proxyChainExcludedDomains instead.
+        """
+        return next(self.zap._request(self.zap.base + 'core/view/optionProxyChainSkipName/').itervalues())
+
+    @property
+    def option_proxy_excluded_domains(self):
+        """
+        Use view proxyChainExcludedDomains instead.
+        """
+        return next(self.zap._request(self.zap.base + 'core/view/optionProxyExcludedDomains/').itervalues())
+
+    @property
+    def option_proxy_excluded_domains_enabled(self):
+        """
+        Use view proxyChainExcludedDomains instead.
+        """
+        return next(self.zap._request(self.zap.base + 'core/view/optionProxyExcludedDomainsEnabled/').itervalues())
+
+    @property
     def option_default_user_agent(self):
         return next(self.zap._request(self.zap.base + 'core/view/optionDefaultUserAgent/').itervalues())
 
     @property
+    def option_dns_ttl_successful_queries(self):
+        """
+        Gets the TTL (in seconds) of successful DNS queries.
+        """
+        return next(self.zap._request(self.zap.base + 'core/view/optionDnsTtlSuccessfulQueries/').itervalues())
+
+    @property
     def option_http_state(self):
         return next(self.zap._request(self.zap.base + 'core/view/optionHttpState/').itervalues())
 
     @property
     def option_proxy_chain_name(self):
         return next(self.zap._request(self.zap.base + 'core/view/optionProxyChainName/').itervalues())
 
@@ -147,30 +189,18 @@
         return next(self.zap._request(self.zap.base + 'core/view/optionProxyChainPort/').itervalues())
 
     @property
     def option_proxy_chain_realm(self):
         return next(self.zap._request(self.zap.base + 'core/view/optionProxyChainRealm/').itervalues())
 
     @property
-    def option_proxy_chain_skip_name(self):
-        return next(self.zap._request(self.zap.base + 'core/view/optionProxyChainSkipName/').itervalues())
-
-    @property
     def option_proxy_chain_user_name(self):
         return next(self.zap._request(self.zap.base + 'core/view/optionProxyChainUserName/').itervalues())
 
     @property
-    def option_proxy_excluded_domains(self):
-        return next(self.zap._request(self.zap.base + 'core/view/optionProxyExcludedDomains/').itervalues())
-
-    @property
-    def option_proxy_excluded_domains_enabled(self):
-        return next(self.zap._request(self.zap.base + 'core/view/optionProxyExcludedDomainsEnabled/').itervalues())
-
-    @property
     def option_timeout_in_secs(self):
         return next(self.zap._request(self.zap.base + 'core/view/optionTimeoutInSecs/').itervalues())
 
     @property
     def option_http_state_enabled(self):
         return next(self.zap._request(self.zap.base + 'core/view/optionHttpStateEnabled/').itervalues())
 
@@ -231,41 +261,53 @@
             params['overwrite'] = overwrite
         return next(self.zap._request(self.zap.base + 'core/action/saveSession/', params).itervalues())
 
     def snapshot_session(self, apikey=''):
         return next(self.zap._request(self.zap.base + 'core/action/snapshotSession/', {'apikey' : apikey}).itervalues())
 
     def clear_excluded_from_proxy(self, apikey=''):
+        """
+        Clears the regexes of URLs excluded from the proxy.
+        """
         return next(self.zap._request(self.zap.base + 'core/action/clearExcludedFromProxy/', {'apikey' : apikey}).itervalues())
 
     def exclude_from_proxy(self, regex, apikey=''):
+        """
+        Adds a regex of URLs that should be excluded from the proxy.
+        """
         return next(self.zap._request(self.zap.base + 'core/action/excludeFromProxy/', {'regex' : regex, 'apikey' : apikey}).itervalues())
 
     def set_home_directory(self, dir, apikey=''):
         return next(self.zap._request(self.zap.base + 'core/action/setHomeDirectory/', {'dir' : dir, 'apikey' : apikey}).itervalues())
 
     def set_mode(self, mode, apikey=''):
         """
         Sets the mode, which may be one of [safe, protect, standard, attack]
         """
         return next(self.zap._request(self.zap.base + 'core/action/setMode/', {'mode' : mode, 'apikey' : apikey}).itervalues())
 
     def generate_root_ca(self, apikey=''):
+        """
+        Generates a new Root CA certificate for the Local Proxy.
+        """
         return next(self.zap._request(self.zap.base + 'core/action/generateRootCA/', {'apikey' : apikey}).itervalues())
 
     def send_request(self, request, followredirects=None, apikey=''):
         """
-        Sends the HTTP request, optionally following redirections. Returns the request sent and response received and followed redirections, if any.
+        Sends the HTTP request, optionally following redirections. Returns the request sent and response received and followed redirections, if any. The Mode is enforced when sending the request (and following redirections), custom manual requests are not allowed in 'Safe' mode nor in 'Protected' mode if out of scope.
         """
         params = {'request' : request, 'apikey' : apikey}
         if followredirects is not None:
             params['followRedirects'] = followredirects
         return next(self.zap._request(self.zap.base + 'core/action/sendRequest/', params).itervalues())
 
     def delete_all_alerts(self, apikey=''):
+        """
+        Deletes all alerts of the current session.
+        """
         return next(self.zap._request(self.zap.base + 'core/action/deleteAllAlerts/', {'apikey' : apikey}).itervalues())
 
     def run_garbage_collection(self, apikey=''):
         return next(self.zap._request(self.zap.base + 'core/action/runGarbageCollection/', {'apikey' : apikey}).itervalues())
 
     def delete_site_node(self, url, method=None, postdata=None, apikey=''):
         """
@@ -274,32 +316,83 @@
         params = {'url' : url, 'apikey' : apikey}
         if method is not None:
             params['method'] = method
         if postdata is not None:
             params['postData'] = postdata
         return next(self.zap._request(self.zap.base + 'core/action/deleteSiteNode/', params).itervalues())
 
+    def add_proxy_chain_excluded_domain(self, value, isregex=None, isenabled=None, apikey=''):
+        """
+        Adds a domain to be excluded from the outgoing proxy, using the specified value. Optionally sets if the new entry is enabled (default, true) and whether or not the new value is specified as a regex (default, false).
+        """
+        params = {'value' : value, 'apikey' : apikey}
+        if isregex is not None:
+            params['isRegex'] = isregex
+        if isenabled is not None:
+            params['isEnabled'] = isenabled
+        return next(self.zap._request(self.zap.base + 'core/action/addProxyChainExcludedDomain/', params).itervalues())
+
+    def modify_proxy_chain_excluded_domain(self, idx, value=None, isregex=None, isenabled=None, apikey=''):
+        """
+        Modifies a domain excluded from the outgoing proxy. Allows to modify the value, if enabled or if a regex. The domain is selected with its index, which can be obtained with the view proxyChainExcludedDomains.
+        """
+        params = {'idx' : idx, 'apikey' : apikey}
+        if value is not None:
+            params['value'] = value
+        if isregex is not None:
+            params['isRegex'] = isregex
+        if isenabled is not None:
+            params['isEnabled'] = isenabled
+        return next(self.zap._request(self.zap.base + 'core/action/modifyProxyChainExcludedDomain/', params).itervalues())
+
+    def remove_proxy_chain_excluded_domain(self, idx, apikey=''):
+        """
+        Removes a domain excluded from the outgoing proxy, with the given index. The index can be obtained with the view proxyChainExcludedDomains.
+        """
+        return next(self.zap._request(self.zap.base + 'core/action/removeProxyChainExcludedDomain/', {'idx' : idx, 'apikey' : apikey}).itervalues())
+
+    def enable_all_proxy_chain_excluded_domains(self, apikey=''):
+        """
+        Enables all domains excluded from the outgoing proxy.
+        """
+        return next(self.zap._request(self.zap.base + 'core/action/enableAllProxyChainExcludedDomains/', {'apikey' : apikey}).itervalues())
+
+    def disable_all_proxy_chain_excluded_domains(self, apikey=''):
+        """
+        Disables all domains excluded from the outgoing proxy.
+        """
+        return next(self.zap._request(self.zap.base + 'core/action/disableAllProxyChainExcludedDomains/', {'apikey' : apikey}).itervalues())
+
     def set_option_default_user_agent(self, string, apikey=''):
         return next(self.zap._request(self.zap.base + 'core/action/setOptionDefaultUserAgent/', {'String' : string, 'apikey' : apikey}).itervalues())
 
     def set_option_proxy_chain_name(self, string, apikey=''):
         return next(self.zap._request(self.zap.base + 'core/action/setOptionProxyChainName/', {'String' : string, 'apikey' : apikey}).itervalues())
 
     def set_option_proxy_chain_password(self, string, apikey=''):
         return next(self.zap._request(self.zap.base + 'core/action/setOptionProxyChainPassword/', {'String' : string, 'apikey' : apikey}).itervalues())
 
     def set_option_proxy_chain_realm(self, string, apikey=''):
         return next(self.zap._request(self.zap.base + 'core/action/setOptionProxyChainRealm/', {'String' : string, 'apikey' : apikey}).itervalues())
 
     def set_option_proxy_chain_skip_name(self, string, apikey=''):
+        """
+        Use actions [add|modify|remove]ProxyChainExcludedDomain instead.
+        """
         return next(self.zap._request(self.zap.base + 'core/action/setOptionProxyChainSkipName/', {'String' : string, 'apikey' : apikey}).itervalues())
 
     def set_option_proxy_chain_user_name(self, string, apikey=''):
         return next(self.zap._request(self.zap.base + 'core/action/setOptionProxyChainUserName/', {'String' : string, 'apikey' : apikey}).itervalues())
 
+    def set_option_dns_ttl_successful_queries(self, integer, apikey=''):
+        """
+        Sets the TTL (in seconds) of successful DNS queries (applies after ZAP restart).
+        """
+        return next(self.zap._request(self.zap.base + 'core/action/setOptionDnsTtlSuccessfulQueries/', {'Integer' : integer, 'apikey' : apikey}).itervalues())
+
     def set_option_http_state_enabled(self, boolean, apikey=''):
         return next(self.zap._request(self.zap.base + 'core/action/setOptionHttpStateEnabled/', {'Boolean' : boolean, 'apikey' : apikey}).itervalues())
 
     def set_option_proxy_chain_port(self, integer, apikey=''):
         return next(self.zap._request(self.zap.base + 'core/action/setOptionProxyChainPort/', {'Integer' : integer, 'apikey' : apikey}).itervalues())
 
     def set_option_proxy_chain_prompt(self, boolean, apikey=''):
@@ -317,14 +410,17 @@
     def set_option_use_proxy_chain_auth(self, boolean, apikey=''):
         return next(self.zap._request(self.zap.base + 'core/action/setOptionUseProxyChainAuth/', {'Boolean' : boolean, 'apikey' : apikey}).itervalues())
 
     def proxy_pac(self, apikey=''):
         return (self.zap._request_other(self.zap.base_other + 'core/other/proxy.pac/', {'apikey' : apikey}))
 
     def rootcert(self, apikey=''):
+        """
+        Gets the Root CA certificate of the Local Proxy.
+        """
         return (self.zap._request_other(self.zap.base_other + 'core/other/rootcert/', {'apikey' : apikey}))
 
     def setproxy(self, proxy, apikey=''):
         return (self.zap._request_other(self.zap.base_other + 'core/other/setproxy/', {'proxy' : proxy, 'apikey' : apikey}))
 
     def xmlreport(self, apikey=''):
         """
@@ -334,14 +430,20 @@
 
     def htmlreport(self, apikey=''):
         """
         Generates a report in HTML format
         """
         return (self.zap._request_other(self.zap.base_other + 'core/other/htmlreport/', {'apikey' : apikey}))
 
+    def mdreport(self, apikey=''):
+        """
+        Generates a report in Markdown format
+        """
+        return (self.zap._request_other(self.zap.base_other + 'core/other/mdreport/', {'apikey' : apikey}))
+
     def message_har(self, id, apikey=''):
         """
         Gets the message with the given ID in HAR format
         """
         return (self.zap._request_other(self.zap.base_other + 'core/other/messageHar/', {'id' : id, 'apikey' : apikey}))
 
     def messages_har(self, baseurl=None, start=None, count=None, apikey=''):
@@ -355,15 +457,15 @@
             params['start'] = start
         if count is not None:
             params['count'] = count
         return (self.zap._request_other(self.zap.base_other + 'core/other/messagesHar/', params))
 
     def send_har_request(self, request, followredirects=None, apikey=''):
         """
-        Sends the first HAR request entry, optionally following redirections. Returns, in HAR format, the request sent and response received and followed redirections, if any.
+        Sends the first HAR request entry, optionally following redirections. Returns, in HAR format, the request sent and response received and followed redirections, if any. The Mode is enforced when sending the request (and following redirections), custom manual requests are not allowed in 'Safe' mode nor in 'Protected' mode if out of scope.
         """
         params = {'request' : request, 'apikey' : apikey}
         if followredirects is not None:
             params['followRedirects'] = followredirects
         return (self.zap._request_other(self.zap.base_other + 'core/other/sendHarRequest/', params))
```

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/users.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/users.py`

 * *Files identical despite different names*

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/ajaxSpider.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/ajaxSpider.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,21 @@
     def number_of_results(self):
         """
         This component is optional and therefore the API will only work if it is installed
         """
         return next(self.zap._request(self.zap.base + 'ajaxSpider/view/numberOfResults/').itervalues())
 
     @property
+    def full_results(self):
+        """
+        This component is optional and therefore the API will only work if it is installed
+        """
+        return next(self.zap._request(self.zap.base + 'ajaxSpider/view/fullResults/').itervalues())
+
+    @property
     def option_browser_id(self):
         """
         This component is optional and therefore the API will only work if it is installed
         """
         return next(self.zap._request(self.zap.base + 'ajaxSpider/view/optionBrowserId/').itervalues())
 
     @property
@@ -115,23 +122,40 @@
     @property
     def option_random_inputs(self):
         """
         This component is optional and therefore the API will only work if it is installed
         """
         return next(self.zap._request(self.zap.base + 'ajaxSpider/view/optionRandomInputs/').itervalues())
 
-    def scan(self, url, inscope=None, apikey=''):
+    def scan(self, url=None, inscope=None, contextname=None, subtreeonly=None, apikey=''):
         """
         This component is optional and therefore the API will only work if it is installed
         """
-        params = {'url' : url, 'apikey' : apikey}
+        params = {'apikey' : apikey}
+        if url is not None:
+            params['url'] = url
         if inscope is not None:
             params['inScope'] = inscope
+        if contextname is not None:
+            params['contextName'] = contextname
+        if subtreeonly is not None:
+            params['subtreeOnly'] = subtreeonly
         return next(self.zap._request(self.zap.base + 'ajaxSpider/action/scan/', params).itervalues())
 
+    def scan_as_user(self, contextname, username, url=None, subtreeonly=None, apikey=''):
+        """
+        This component is optional and therefore the API will only work if it is installed
+        """
+        params = {'contextName' : contextname, 'userName' : username, 'apikey' : apikey}
+        if url is not None:
+            params['url'] = url
+        if subtreeonly is not None:
+            params['subtreeOnly'] = subtreeonly
+        return next(self.zap._request(self.zap.base + 'ajaxSpider/action/scanAsUser/', params).itervalues())
+
     def stop(self, apikey=''):
         """
         This component is optional and therefore the API will only work if it is installed
         """
         return next(self.zap._request(self.zap.base + 'ajaxSpider/action/stop/', {'apikey' : apikey}).itervalues())
 
     def set_option_browser_id(self, string, apikey=''):
```

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/authorization.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/authorization.py`

 * *Files identical despite different names*

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/context.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/context.py`

 * *Files identical despite different names*

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/forcedUser.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/forcedUser.py`

 * *Files identical despite different names*

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/sessionManagement.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/sessionManagement.py`

 * *Files identical despite different names*

### Comparing `python-owasp-zap-v2.4-0.0.8/src/zapv2/authentication.py` & `python-owasp-zap-v2.4-0.0.9/src/zapv2/authentication.py`

 * *Files identical despite different names*

### Comparing `python-owasp-zap-v2.4-0.0.8/src/python_owasp_zap_v2.4.egg-info/PKG-INFO` & `python-owasp-zap-v2.4-0.0.9/src/python_owasp_zap_v2.4.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.1
 Name: python-owasp-zap-v2.4
-Version: 0.0.8
-Summary: OWASP ZAP 2.5 API client
+Version: 0.0.9
+Summary: OWASP ZAP 2.6 API client
 Home-page: https://www.owasp.org/index.php/OWASP_Zed_Attack_Proxy_Project
 Author: ZAP development team
 Author-email: UNKNOWN
 License: ASL2.0
-Download-URL: https://github.com/zaproxy/zap-api-python/releases/tag/0.0.8
-Description: OWASP Zed Attack Proxy 2.5 API python client (the 2.4 package name has been kept to make it easier to upgrade)
+Download-URL: https://github.com/zaproxy/zap-api-python/releases/tag/0.0.9
+Description: OWASP Zed Attack Proxy 2.6 API python client (the 2.4 package name has been kept to make it easier to upgrade)
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `python-owasp-zap-v2.4-0.0.8/src/python_owasp_zap_v2.4.egg-info/SOURCES.txt` & `python-owasp-zap-v2.4-0.0.9/src/python_owasp_zap_v2.4.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 setup.py
 src/python_owasp_zap_v2.4.egg-info/PKG-INFO
 src/python_owasp_zap_v2.4.egg-info/SOURCES.txt
 src/python_owasp_zap_v2.4.egg-info/dependency_links.txt
+src/python_owasp_zap_v2.4.egg-info/requires.txt
 src/python_owasp_zap_v2.4.egg-info/top_level.txt
 src/zapv2/__init__.py
 src/zapv2/acsrf.py
 src/zapv2/ajaxSpider.py
 src/zapv2/ascan.py
 src/zapv2/authentication.py
 src/zapv2/authorization.py
```

### Comparing `python-owasp-zap-v2.4-0.0.8/PKG-INFO` & `python-owasp-zap-v2.4-0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.1
 Name: python-owasp-zap-v2.4
-Version: 0.0.8
-Summary: OWASP ZAP 2.5 API client
+Version: 0.0.9
+Summary: OWASP ZAP 2.6 API client
 Home-page: https://www.owasp.org/index.php/OWASP_Zed_Attack_Proxy_Project
 Author: ZAP development team
 Author-email: UNKNOWN
 License: ASL2.0
-Download-URL: https://github.com/zaproxy/zap-api-python/releases/tag/0.0.8
-Description: OWASP Zed Attack Proxy 2.5 API python client (the 2.4 package name has been kept to make it easier to upgrade)
+Download-URL: https://github.com/zaproxy/zap-api-python/releases/tag/0.0.9
+Description: OWASP Zed Attack Proxy 2.6 API python client (the 2.4 package name has been kept to make it easier to upgrade)
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

