# Comparing `tmp/selenium_injector-2.2.tar.gz` & `tmp/selenium_injector-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\selenium_injector-2.2.tar", last modified: Mon Jul  3 16:13:20 2023, max compression
+gzip compressed data, was "dist\selenium_injector-2.3.tar", last modified: Fri Jul 14 13:53:44 2023, max compression
```

## Comparing `selenium_injector-2.2.tar` & `selenium_injector-2.3.tar`

### file list

```diff
@@ -1,44 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/
--rw-rw-rw-   0        0        0      641 2022-11-24 08:41:11.000000 selenium_injector-2.2/LICENSE.md
--rw-rw-rw-   0        0        0      275 2023-07-03 15:31:02.000000 selenium_injector-2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6171 2023-07-03 16:13:20.000000 selenium_injector-2.2/PKG-INFO
--rw-rw-rw-   0        0        0     4865 2023-07-03 14:55:29.000000 selenium_injector-2.2/README.md
--rw-rw-rw-   0        0        0      522 2023-04-06 21:41:47.000000 selenium_injector-2.2/build_upload.md
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_injector-2.2/pyproject.toml
--rw-rw-rw-   0        0        0      131 2023-07-03 16:13:20.000000 selenium_injector-2.2/setup.cfg
--rw-rw-rw-   0        0        0     1835 2023-07-03 16:06:03.000000 selenium_injector-2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector/
--rw-rw-rw-   0        0        0       21 2023-07-03 16:05:19.000000 selenium_injector-2.2/src/selenium_injector/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector/files/
-drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector/files/extension/
--rw-rw-rw-   0        0        0     2158 2023-07-03 08:21:18.000000 selenium_injector-2.2/src/selenium_injector/files/extension/background.js
--rw-rw-rw-   0        0        0     1661 2023-07-03 15:10:30.000000 selenium_injector-2.2/src/selenium_injector/files/extension/manifest_2.json
--rw-rw-rw-   0        0        0     1928 2023-07-03 14:10:59.000000 selenium_injector-2.2/src/selenium_injector/files/extension/manifest_3.json
--rw-rw-rw-   0        0        0      818 2023-07-03 08:21:18.000000 selenium_injector-2.2/src/selenium_injector/files/extension/stay_alive.js
-drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector/files/js/
--rw-rw-rw-   0        0        0     8796 2023-07-02 20:13:16.000000 selenium_injector-2.2/src/selenium_injector/files/js/connection.js
--rw-rw-rw-   0        0        0      310 2023-06-20 10:28:07.000000 selenium_injector-2.2/src/selenium_injector/files/js/utils.js
-drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector/files/tmp/
-drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector/files/tmp/mv2_extension/
--rw-rw-rw-   0        0        0    11075 2023-07-03 15:12:26.000000 selenium_injector-2.2/src/selenium_injector/files/tmp/mv2_extension/background.js
--rw-rw-rw-   0        0        0     1661 2023-07-03 15:12:26.000000 selenium_injector-2.2/src/selenium_injector/files/tmp/mv2_extension/manifest.json
-drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector/files/tmp/mv3_extension/
--rw-rw-rw-   0        0        0    11893 2023-07-03 15:12:26.000000 selenium_injector-2.2/src/selenium_injector/files/tmp/mv3_extension/background.js
--rw-rw-rw-   0        0        0     1928 2023-07-03 15:12:26.000000 selenium_injector-2.2/src/selenium_injector/files/tmp/mv3_extension/manifest.json
-drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_injector-2.2/src/selenium_injector/scripts/__init__.py
--rw-rw-rw-   0        0        0    11664 2023-07-03 15:41:38.000000 selenium_injector-2.2/src/selenium_injector/scripts/injector.py
--rw-rw-rw-   0        0        0     2115 2023-07-02 17:58:37.000000 selenium_injector-2.2/src/selenium_injector/scripts/js.py
--rw-rw-rw-   0        0        0     2080 2023-07-02 18:08:57.000000 selenium_injector-2.2/src/selenium_injector/scripts/socket.py
--rw-rw-rw-   0        0        0     6753 2023-07-02 19:26:13.000000 selenium_injector-2.2/src/selenium_injector/scripts/sync_websocket.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector/utils/
--rw-rw-rw-   0        0        0        0 2023-06-20 13:26:36.000000 selenium_injector-2.2/src/selenium_injector/utils/__init__.py
--rw-rw-rw-   0        0        0     1586 2023-07-02 17:56:54.000000 selenium_injector-2.2/src/selenium_injector/utils/utils.py
--rw-rw-rw-   0        0        0     1992 2023-07-03 14:25:42.000000 selenium_injector-2.2/src/selenium_injector/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector.egg-info/
--rw-rw-rw-   0        0        0     6171 2023-07-03 16:13:19.000000 selenium_injector-2.2/src/selenium_injector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1197 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 16:13:19.000000 selenium_injector-2.2/src/selenium_injector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-07-03 16:13:19.000000 selenium_injector-2.2/src/selenium_injector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-03 16:13:19.000000 selenium_injector-2.2/src/selenium_injector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 13:53:44.000000 selenium_injector-2.3/
+-rw-rw-rw-   0        0        0      641 2022-11-24 08:41:11.000000 selenium_injector-2.3/LICENSE.md
+-rw-rw-rw-   0        0        0      171 2023-07-07 07:54:27.000000 selenium_injector-2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     8151 2023-07-14 13:53:44.000000 selenium_injector-2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6845 2023-07-14 13:49:27.000000 selenium_injector-2.3/README.md
+-rw-rw-rw-   0        0        0      522 2023-04-06 21:41:47.000000 selenium_injector-2.3/build_upload.md
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_injector-2.3/pyproject.toml
+-rw-rw-rw-   0        0        0      131 2023-07-14 13:53:44.000000 selenium_injector-2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1835 2023-07-14 13:52:41.000000 selenium_injector-2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:53:44.000000 selenium_injector-2.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 13:53:44.000000 selenium_injector-2.3/src/selenium_injector/
+-rw-rw-rw-   0        0        0       21 2023-07-14 13:51:32.000000 selenium_injector-2.3/src/selenium_injector/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:53:44.000000 selenium_injector-2.3/src/selenium_injector/files/
+drwxrwxrwx   0        0        0        0 2023-07-14 13:53:44.000000 selenium_injector-2.3/src/selenium_injector/files/extension/
+-rw-rw-rw-   0        0        0     3266 2023-07-12 08:43:15.000000 selenium_injector-2.3/src/selenium_injector/files/extension/background.js
+-rw-rw-rw-   0        0        0     1661 2023-07-06 19:19:06.000000 selenium_injector-2.3/src/selenium_injector/files/extension/manifest_2.json
+-rw-rw-rw-   0        0        0     1928 2023-07-03 14:10:59.000000 selenium_injector-2.3/src/selenium_injector/files/extension/manifest_3.json
+-rw-rw-rw-   0        0        0      866 2023-07-06 16:49:03.000000 selenium_injector-2.3/src/selenium_injector/files/extension/stay_alive.js
+drwxrwxrwx   0        0        0        0 2023-07-14 13:53:44.000000 selenium_injector-2.3/src/selenium_injector/files/js/
+-rw-rw-rw-   0        0        0     9457 2023-07-13 09:08:44.000000 selenium_injector-2.3/src/selenium_injector/files/js/connection.js
+-rw-rw-rw-   0        0        0     8299 2023-07-13 16:11:56.000000 selenium_injector-2.3/src/selenium_injector/files/js/returner.js
+drwxrwxrwx   0        0        0        0 2023-07-14 13:53:44.000000 selenium_injector-2.3/src/selenium_injector/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_injector-2.3/src/selenium_injector/scripts/__init__.py
+-rw-rw-rw-   0        0        0    26811 2023-07-13 19:38:35.000000 selenium_injector-2.3/src/selenium_injector/scripts/injector.py
+-rw-rw-rw-   0        0        0     2364 2023-07-13 16:37:51.000000 selenium_injector-2.3/src/selenium_injector/scripts/socket.py
+-rw-rw-rw-   0        0        0     6790 2023-07-09 15:57:13.000000 selenium_injector-2.3/src/selenium_injector/scripts/sync_websocket.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:53:44.000000 selenium_injector-2.3/src/selenium_injector/types/
+-rw-rw-rw-   0        0        0        0 2023-07-12 08:43:16.000000 selenium_injector-2.3/src/selenium_injector/types/__init__.py
+-rw-rw-rw-   0        0        0     1084 2023-07-12 08:43:16.000000 selenium_injector-2.3/src/selenium_injector/types/by.py
+-rw-rw-rw-   0        0        0     3129 2023-07-13 19:11:20.000000 selenium_injector-2.3/src/selenium_injector/types/js.py
+-rw-rw-rw-   0        0        0    18606 2023-07-13 19:38:35.000000 selenium_injector-2.3/src/selenium_injector/types/webelement.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:53:44.000000 selenium_injector-2.3/src/selenium_injector/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-20 13:26:36.000000 selenium_injector-2.3/src/selenium_injector/utils/__init__.py
+-rw-rw-rw-   0        0        0     1586 2023-07-02 17:56:54.000000 selenium_injector-2.3/src/selenium_injector/utils/utils.py
+-rw-rw-rw-   0        0        0     1372 2023-07-13 19:31:27.000000 selenium_injector-2.3/src/selenium_injector/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:53:44.000000 selenium_injector-2.3/src/selenium_injector.egg-info/
+-rw-rw-rw-   0        0        0     8151 2023-07-14 13:53:44.000000 selenium_injector-2.3/src/selenium_injector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1074 2023-07-14 13:53:44.000000 selenium_injector-2.3/src/selenium_injector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 13:53:44.000000 selenium_injector-2.3/src/selenium_injector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-07-14 13:53:44.000000 selenium_injector-2.3/src/selenium_injector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-14 13:53:44.000000 selenium_injector-2.3/src/selenium_injector.egg-info/top_level.txt
```

### Comparing `selenium_injector-2.2/LICENSE.md` & `selenium_injector-2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_injector-2.2/PKG-INFO` & `selenium_injector-2.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.1
-Name: selenium_injector
-Version: 2.2
-Summary: inject javascript into chrome
-Home-page: https://github.com/kaliiiiiiiiii/Selenium-Injector
-Author: Aurin Aegerter
-Author-email: aurinliun@gmx.ch
-Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Injector
-Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Injector/issues
-Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Injector
-Keywords: Selenium,interception,proxy,webautomation
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
-Classifier: Topic :: Internet :: Proxy Servers
-Classifier: Topic :: Internet
-Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.md
-
 # Selenium-Injector
 
 * Change proxy while running (auth supported)
 * remotely contoll Chrome using websockets and extensions
 
 ### Feel free to test my code!
 
@@ -47,59 +17,30 @@
 
 * [Windows] Install [Chrome-Browser](https://www.google.de/chrome/)
 * ```pip install selenium_injector```
 
 
 ### Example scripts
 
-
-#### click on element
-```python
-from selenium_injector.webdriver import Chrome
-
-# base driver to use
-# from selenium.webdriver import Chrome as base_driver
-from undetected_chromedriver import Chrome as base_driver
-
-driver = Chrome(base_drivers=(base_driver,))
-
-driver.get("https://www.wikipedia.org/")
-driver.injector.socket.exec_command("utils.find_element.ByXpath", '//*[@id="js-link-box-en"]/strong', user=driver.injector.tab_user)
-
-js = driver.injector.socket.js
-t = js.types
-u = js.utils
-
-prev_url = driver.current_url[:]
-try:
-    driver.injector.socket.exec(u.click_element(u.find_element_by_xpath('//*[@id="js-link-box-en"]/strong')), user=driver.injector.tab_user, timeout=2)
-except TimeoutError as e:
-    if driver.current_url != prev_url:
-        pass # new page loaded before send_response
-    else:
-        raise e
-
-driver.quit()
-```
-Don't forget to execute
-`driver.quit()`
-in the End. Else-wise your temporary folder will get flooded! and it keeps running
-
 #### set proxy dynamically
 ```python
 from selenium_injector.webdriver import Chrome
 driver = Chrome()
 
 driver.injector.proxy.set_single(host="example_host.com", port=143, password="password", username="user-1")
 
 driver.get("https://whatismyipaddress.com/")
 
 driver.injector.proxy.clear()
 driver.quit()
 ```
+Don't forget to execute
+`driver.quit()`
+in the End. Else-wise your temporary folder will get flooded! and it keeps running
+
 #### use events
 ```python
 from selenium_injector.webdriver import Chrome
 import json
 
 driver = Chrome()
 
@@ -120,40 +61,147 @@
 
 event = driver.injector.socket.event(event_id, user=user)
 for e in event:  # will block forever
     e = json.loads(e)
     data = e["result"][0]
     time = e["t"]
     print(time + "\n", data['url'])
-
 ```
 warning: as `driver.quit()` isn't called in this example, it will leave files in your temp directories
 
+#### modify network requests
+note: this is only experimental yet (not included in pypi package)
+
+example script
+```python
+from selenium_injector.webdriver import Chrome
+
+driver = Chrome()
+
+# modify headers
+driver.injector.declarativeNetRequest.update_headers({"test": "test_2", "sec-ch-ua-platform": "Android"})
+rules = driver.injector.declarativeNetRequest.dynamic_rules
+headers = driver.injector.declarativeNetRequest._headers
+
+driver.get("https://httpbin.org/headers")
+input("press ENTER to continue")
+
+# block images
+driver.injector.declarativeNetRequest.update_block_on(resource_types=["image"])
+
+driver.get("https://www.wikimedia.org/")
+
+input("press ENTER to exit")
+driver.quit()
+```
+
+#### use chrome-developer-protocoll
+note: this is only experimental yet (not included in pypi package)
+
+example script
+```python
+import json
+from selenium_injector.webdriver import Chrome
+
+driver = Chrome()
+
+dbg = driver.injector.debugger
+dbg.attach()
+dbg.execute("Console.enable")
+
+events = dbg.on_event()
+
+driver.execute_script("console.log('Hello World!')")
+
+for event in events:
+    event = json.loads(event)
+    result = event["result"]
+    time = event["t"]
+    if result[1] == 'Console.messageAdded':
+        message_text = result[2]["message"]["text"]
+        print(time, message_text)
+        break
+
+driver.quit()
+```
+
+#### execute script within tab
+note: this is only experimental yet (not included in pypi package)
+
+from string
+```python
+from selenium_injector.webdriver import Chrome
+driver = Chrome(injector_options={"mv2":True, "mv3":True})
+
+driver.get("https://www.wikipedia.org/")
+
+# result only returned with mv2 extension enabled
+results = driver.injector.tabs.eval_str(
+            '''
+            console.log(window);
+            navigator.userAgent
+            ''', tab_id=driver.injector.tabs.active_tab["id"])
+print(results[0])
+
+driver.quit()
+```
+
+with types, always returns
+resolves promises with MV3 automatically
+```python
+from selenium_injector.webdriver import Chrome
+driver = Chrome(injector_options={"mv3":True})
+
+driver.get("https://www.wikipedia.org/")
+
+t = driver.injector.socket.js.types
+results = driver.injector.tabs.exec(t.exec(t.path("fetch"), args=[t.value("https://www.wikipedia.org/")]), timeout=40)
+print(results["result"][0])
+
+driver.quit()
+```
+
+#### find element
+note: this is only experimental yet (not included in pypi package)
+```python
+from selenium_injector.webdriver import Chrome
+from selenium_injector.types.by import By
+
+driver = Chrome(injector_options={"mv2":True, "mv3":True})
+driver.get("https://www.wikipedia.org/")
+
+
+elem = driver.injector.find_elements(By.XPATH, '//*[@id="js-link-box-en"]')
+elem[0].click()
+
+driver.quit()
+```
 
 ## Help
 
 Please feel free to open an issue or fork!
 
 ## Todo
-
-- [ ] eval within tab scope from extension
-- [x] Add MV2 extension
-  - [ ] change headers
+- [x] eval within tab scope from extension
+  - [x] mv2
+    - [x] return 
+    - [ ] stringify obj
+  - [x] mv3
+    - [ ] return
+    - [ ] stringify obj
 - [x] add events
   - [x] make protocoll use `UUIDS`'s
   - [ ] allow response to event within scope
     - using `(...args) => {new event_handler(...args)}`
 - [x] types.eval
   - [ ] for-loops
-  - [x] async execution
 - [x] authentificaten proxies
   - [x] manage webrtc-leak
   - [x] manage location api leak
   - [ ] proxy per request
-- [ ] add `chrome.scripting` support
 - [ ] add automation tools
   - [x] click
   - [ ] send_keys
   - [ ] find_element
     - [x] by XPATH
 - [ ] undetectability
   - [x] make tab scripts private
@@ -189,7 +237,8 @@
 * [Chrome-devtools-protocol](https://chromedevtools.github.io/devtools-protocol/tot/Fetch/#method-enable)
 * [cdp_event_listeners](https://stackoverflow.com/questions/66227508/selenium-4-0-0-beta-1-how-add-event-listeners-in-cdp)
 * [sync websocket server](https://stackoverflow.com/questions/68939894/implement-a-python-websocket-listener-without-async-asyncio)
 * [chrome-extension-docs](https://developer.chrome.com/docs/extensions/reference/)
 * [PEG-parser](https://github.com/pegjs/pegjs)
 * [make-SV-stayalive](https://stackoverflow.com/a/75082732/20443541)
 * [stringify-obj](https://stackoverflow.com/a/58416333/20443541)
+* [inject code from mv3](https://stackoverflow.com/a/70949953/20443541)
```

### Comparing `selenium_injector-2.2/build_upload.md` & `selenium_injector-2.3/build_upload.md`

 * *Files identical despite different names*

### Comparing `selenium_injector-2.2/setup.py` & `selenium_injector-2.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-requirements = ['selenium', 'requests', "selenium_profiles>=2.2.7.2", "websockets"]
+requirements = ['selenium', 'requests', "selenium-profiles>=2.2.7.3", "websockets"]
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='selenium_injector',
     author='Aurin Aegerter',
```

### Comparing `selenium_injector-2.2/src/selenium_injector/files/extension/manifest_2.json` & `selenium_injector-2.3/src/selenium_injector/files/extension/manifest_2.json`

 * *Files identical despite different names*

### Comparing `selenium_injector-2.2/src/selenium_injector/files/extension/manifest_3.json` & `selenium_injector-2.3/src/selenium_injector/files/extension/manifest_3.json`

 * *Files identical despite different names*

### Comparing `selenium_injector-2.2/src/selenium_injector/files/extension/stay_alive.js` & `selenium_injector-2.3/src/selenium_injector/files/extension/stay_alive.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -15,14 +15,15 @@
         if (alivePort == null) {
             alivePort = chrome.runtime.connect({
                 name: INTERNAL_STAYALIVE_PORT
             })
 
             alivePort.onDisconnect.addListener((p) => {
                 alivePort = null;
+                if (chrome.runtime.lastError) {}
             });
         }
 
         if (alivePort) {
             alivePort.postMessage({
                 content: "ping"
             });
```

### Comparing `selenium_injector-2.2/src/selenium_injector/files/js/connection.js` & `selenium_injector-2.3/src/selenium_injector/files/js/connection.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -36,41 +36,56 @@
                 this.not_return = request["not_return"]
             }
             if (request.hasOwnProperty("max_depth")) {
                 this.max_depth = request["max_depth"]
             }
 
             var result = this.eval(request)
-
-            if (this.not_return && result && result.catch && this.isFunction(result.catch)) {
-                // handle async errors
-                result.catch((e) => {
-                    result = {
-                        "message": e.message,
-                        "stack": e.stack
-                    };
-                    this.status = "error"
-                })
-            }
+            this.catch_async(result)
         } catch (e) {
             // handle sync errors
-            var result = {
+            var result = result = {
                 "message": e.message,
                 "stack": e.stack
             };
             this.status = "error"
         };
-        if (!(this.not_return) || this.status === "error") {
+        if (!(this.not_return)) {
             this.send_back(result)
         }
     }
+    catch_async(result) {
+        if (result && result.catch && this.isFunction(result.catch)) {
+            // handle async errors
+
+            result.catch(function(e) {
+                // we dont want multiple responses
+                if (!(this.status == "error")) {
+                    result = result = {
+                        "message": e.message,
+                        "stack": e.stack
+                    };
+                    this.status = "error"
+                    this.send_back(result)
+                    this.not_return = true
+                }
+            }.bind(this))
+        }
+    }
     parse(results, status) {
         var date = new Date()
         date = date.toLocaleString()
-
+        if (chrome.runtime && chrome.runtime.lastError) {
+            // handle async errors in extension
+            results = [{
+                "message": chrome.runtime.lastError.message,
+                "stack": chrome.runtime.lastError.message
+            }];
+            status = "error"
+        }
         try {
             var parsed = '{"result":' + this.stringify(results, 0, this.max_depth) + ', "status":' + JSON.stringify(status) + ',"t":"' + date + '"}'
         } catch (e) {
             var parsed = this.parse([{
                 "message": e.message,
                 "stack": e.stack
             }], "error")
@@ -164,14 +179,17 @@
 
     path(path, obj = undefined) {
         if (obj == undefined) {
             obj = globalThis
         } else {
             obj = this.eval(obj)
         }
+        if (typeof path === "number") {
+            return obj[path]
+        }
         for (var i = 0, path = path.split('.'), len = path.length; i < len; i++) {
             if (this.isFunction(obj[path[i]])) {
                 obj = obj[path[i]].bind(obj)
             } else {
                 obj = obj[path[i]]
             };
         };
@@ -182,15 +200,17 @@
         var res_args = [];
         var do_eval = this.eval.bind(this)
         args.forEach(function(item, index) {
             res_args.push(do_eval(item))
         });
         var res_func = this.eval(func)
         if (this.isFunction(res_func)) {
-            return res_func(...res_args)
+            var result = res_func(...res_args)
+            this.catch_async(result)
+            return result
         } else {
             throw new TypeError("Expected a function, got " + this.stringify(res_func))
         };
     }
 
     list(list) {
         var results = [];
```

### Comparing `selenium_injector-2.2/src/selenium_injector/scripts/js.py` & `selenium_injector-2.3/src/selenium_injector/types/js.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 class JS:
     def __init__(self):
         self.types = self.types()
-        self.utils = self.utils(self.types)
+        self.find_elements = self.find_elements(self.types)
 
     class types:
         def __init__(self):
             self.not_return = {"not_return": True}
 
         def path(self, path: str, obj: dict = None):
             return {"type": "path", "path": path, "obj": obj}
@@ -44,17 +44,38 @@
             return self.path("event_callback", obj=self.this())
 
         def set_event_id(self, event_id):
             return self.exec(self.path("set_event_id", obj=self.this()),
                              args=[self.value(event_id)]
                              )
 
-    class utils:
+    class find_elements:
         def __init__(self, types):
-            self.types = types
+            self.t = types
 
-        def find_element_by_xpath(self, xpath: str):
-            return self.types.exec(self.types.path("utils.find_element.ByXpath"),
-                                   args=[self.types.value(xpath)])
-
-        def click_element(self, element: dict):
-            return self.types.exec(self.types.path("click", element))
+        def _by_xpath_result_length(self, value, base_element):
+            script = self._by_xpath(value, base_element)
+            return self.t.path("snapshotLength", obj=script)
+
+        def _by_xpath(self, value, base_element):
+            script = self.t.exec(self.t.path("document.evaluate"), args=[
+                                     self.t.value(value),
+                                     base_element, self.t.value(None),
+                                     self.t.value(7),  # "XPathResult.ORDERED_NODE_SNAPSHOT_TYPE"
+                                     self.t.value(None)
+                                 ])
+            return script
+
+        def by_xpath(self, value: str, base_element, idx: int):
+            script = self._by_xpath(value, base_element)
+            return self.t.exec(self.t.path("snapshotItem", obj=script), args=[self.t.value(idx)])
+
+        def by_tag_name(self, value, base_element):
+            return self.t.exec(self.t.path("getElementsByTagName", obj=base_element), args=[
+                self.t.value(value)
+            ])
+
+        def by_css_selector(self, value, base_element):
+            script = self.t.exec(self.t.path("querySelectorAll", obj=base_element), args=[
+                self.t.value(value)
+            ])
+            return script
```

### Comparing `selenium_injector-2.2/src/selenium_injector/scripts/socket.py` & `selenium_injector-2.3/src/selenium_injector/scripts/socket.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 from selenium_injector.scripts.sync_websocket import SynchronousWebsocketServer
-from selenium_injector.scripts.js import JS
+from selenium_injector.types.js import JS
+
+
+class JSEvalException(Exception):
+    def __init__(self, message: str, stack: str = None):
+        super().__init__(stack)
+        self.message = message
+        self.stack = stack
 
 
 class socket(SynchronousWebsocketServer):
     def __init__(self):
         self.js = JS()
         self.send_back = self.js.types.send_back()
         self.not_return = {"not_return": True}
@@ -16,15 +23,17 @@
 
         script["max_depth"] = max_depth
 
         import json
         result = self.post(json.dumps(script), user=user, timeout=timeout, start_time=start_time, interval=interval)
         result = json.loads(result)
         if result["status"] == "error":
-            raise Exception(result["result"][0]["stack"])
+            message = result["result"][0]["message"]
+            stack = result["result"][0]["stack"]
+            raise JSEvalException(message, stack)
         return result
 
     def exec_async(self, script: dict, user: str = None, max_depth=2, timeout: int = 10, start_time=None,
                    interval: float = 0.1):
         if not start_time:
             start_time = self.time
```

### Comparing `selenium_injector-2.2/src/selenium_injector/scripts/sync_websocket.py` & `selenium_injector-2.3/src/selenium_injector/scripts/sync_websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,21 +28,19 @@
 class SynchronousWebsocketServer:
     """
     Synchronous wrapper around asynchronous websockets server by Pier-Yves Lessard, modified by Aurin Aegerter
     https://stackoverflow.com/questions/68939894/implement-a-python-websocket-listener-without-async-asyncio
     """
 
     def __init__(self):
-        import atexit
         self.loop = asyncio.new_event_loop()
         self.ws_server = None
         self.users = {}
         self.host = None
         self.port = None
-        atexit.register(self.stop)
 
     # Executed for each websocket
     async def server_routine(self, websocket):
         # noinspection PyUnresolvedReferences
         try:
             user = await websocket.recv()
         except websockets.exceptions.ConnectionClosedError:
@@ -56,17 +54,18 @@
             async for message in websocket:
                 response = message[32:]
                 resp_id = message[0:32]
 
                 if resp_id[0] == "E":  # is event
                     self.users[user]["events"][resp_id].queue.put(response)
                 else:  # is response
-                    if resp_id in self.users[user]["rx"]:
-                        raise ConnectionError(f'already got ["{user}"]["rx"]["{resp_id}"], dublicate response-id')
-                    self.users[user]["rx"].update({resp_id: response})
+                    if user in self.users:
+                        if resp_id in self.users[user]["rx"]:
+                            raise ConnectionError(f'already got ["{user}"]["rx"]["{resp_id}"], dublicate response-id. \n this might be due to an async error')
+                        self.users[user]["rx"].update({resp_id: response})
         except websockets.exceptions.ConnectionClosedError:
             pass
         finally:
             try:
                 del self.users[user]
             except KeyError:
                 pass
```

### Comparing `selenium_injector-2.2/src/selenium_injector/utils/utils.py` & `selenium_injector-2.3/src/selenium_injector/utils/utils.py`

 * *Files identical despite different names*

### Comparing `selenium_injector-2.2/src/selenium_injector.egg-info/PKG-INFO` & `selenium_injector-2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: selenium-injector
-Version: 2.2
+Name: selenium_injector
+Version: 2.3
 Summary: inject javascript into chrome
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Injector
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Injector
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Injector/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Injector
@@ -47,59 +47,30 @@
 
 * [Windows] Install [Chrome-Browser](https://www.google.de/chrome/)
 * ```pip install selenium_injector```
 
 
 ### Example scripts
 
-
-#### click on element
-```python
-from selenium_injector.webdriver import Chrome
-
-# base driver to use
-# from selenium.webdriver import Chrome as base_driver
-from undetected_chromedriver import Chrome as base_driver
-
-driver = Chrome(base_drivers=(base_driver,))
-
-driver.get("https://www.wikipedia.org/")
-driver.injector.socket.exec_command("utils.find_element.ByXpath", '//*[@id="js-link-box-en"]/strong', user=driver.injector.tab_user)
-
-js = driver.injector.socket.js
-t = js.types
-u = js.utils
-
-prev_url = driver.current_url[:]
-try:
-    driver.injector.socket.exec(u.click_element(u.find_element_by_xpath('//*[@id="js-link-box-en"]/strong')), user=driver.injector.tab_user, timeout=2)
-except TimeoutError as e:
-    if driver.current_url != prev_url:
-        pass # new page loaded before send_response
-    else:
-        raise e
-
-driver.quit()
-```
-Don't forget to execute
-`driver.quit()`
-in the End. Else-wise your temporary folder will get flooded! and it keeps running
-
 #### set proxy dynamically
 ```python
 from selenium_injector.webdriver import Chrome
 driver = Chrome()
 
 driver.injector.proxy.set_single(host="example_host.com", port=143, password="password", username="user-1")
 
 driver.get("https://whatismyipaddress.com/")
 
 driver.injector.proxy.clear()
 driver.quit()
 ```
+Don't forget to execute
+`driver.quit()`
+in the End. Else-wise your temporary folder will get flooded! and it keeps running
+
 #### use events
 ```python
 from selenium_injector.webdriver import Chrome
 import json
 
 driver = Chrome()
 
@@ -120,40 +91,147 @@
 
 event = driver.injector.socket.event(event_id, user=user)
 for e in event:  # will block forever
     e = json.loads(e)
     data = e["result"][0]
     time = e["t"]
     print(time + "\n", data['url'])
-
 ```
 warning: as `driver.quit()` isn't called in this example, it will leave files in your temp directories
 
+#### modify network requests
+note: this is only experimental yet (not included in pypi package)
+
+example script
+```python
+from selenium_injector.webdriver import Chrome
+
+driver = Chrome()
+
+# modify headers
+driver.injector.declarativeNetRequest.update_headers({"test": "test_2", "sec-ch-ua-platform": "Android"})
+rules = driver.injector.declarativeNetRequest.dynamic_rules
+headers = driver.injector.declarativeNetRequest._headers
+
+driver.get("https://httpbin.org/headers")
+input("press ENTER to continue")
+
+# block images
+driver.injector.declarativeNetRequest.update_block_on(resource_types=["image"])
+
+driver.get("https://www.wikimedia.org/")
+
+input("press ENTER to exit")
+driver.quit()
+```
+
+#### use chrome-developer-protocoll
+note: this is only experimental yet (not included in pypi package)
+
+example script
+```python
+import json
+from selenium_injector.webdriver import Chrome
+
+driver = Chrome()
+
+dbg = driver.injector.debugger
+dbg.attach()
+dbg.execute("Console.enable")
+
+events = dbg.on_event()
+
+driver.execute_script("console.log('Hello World!')")
+
+for event in events:
+    event = json.loads(event)
+    result = event["result"]
+    time = event["t"]
+    if result[1] == 'Console.messageAdded':
+        message_text = result[2]["message"]["text"]
+        print(time, message_text)
+        break
+
+driver.quit()
+```
+
+#### execute script within tab
+note: this is only experimental yet (not included in pypi package)
+
+from string
+```python
+from selenium_injector.webdriver import Chrome
+driver = Chrome(injector_options={"mv2":True, "mv3":True})
+
+driver.get("https://www.wikipedia.org/")
+
+# result only returned with mv2 extension enabled
+results = driver.injector.tabs.eval_str(
+            '''
+            console.log(window);
+            navigator.userAgent
+            ''', tab_id=driver.injector.tabs.active_tab["id"])
+print(results[0])
+
+driver.quit()
+```
+
+with types, always returns
+resolves promises with MV3 automatically
+```python
+from selenium_injector.webdriver import Chrome
+driver = Chrome(injector_options={"mv3":True})
+
+driver.get("https://www.wikipedia.org/")
+
+t = driver.injector.socket.js.types
+results = driver.injector.tabs.exec(t.exec(t.path("fetch"), args=[t.value("https://www.wikipedia.org/")]), timeout=40)
+print(results["result"][0])
+
+driver.quit()
+```
+
+#### find element
+note: this is only experimental yet (not included in pypi package)
+```python
+from selenium_injector.webdriver import Chrome
+from selenium_injector.types.by import By
+
+driver = Chrome(injector_options={"mv2":True, "mv3":True})
+driver.get("https://www.wikipedia.org/")
+
+
+elem = driver.injector.find_elements(By.XPATH, '//*[@id="js-link-box-en"]')
+elem[0].click()
+
+driver.quit()
+```
 
 ## Help
 
 Please feel free to open an issue or fork!
 
 ## Todo
-
-- [ ] eval within tab scope from extension
-- [x] Add MV2 extension
-  - [ ] change headers
+- [x] eval within tab scope from extension
+  - [x] mv2
+    - [x] return 
+    - [ ] stringify obj
+  - [x] mv3
+    - [ ] return
+    - [ ] stringify obj
 - [x] add events
   - [x] make protocoll use `UUIDS`'s
   - [ ] allow response to event within scope
     - using `(...args) => {new event_handler(...args)}`
 - [x] types.eval
   - [ ] for-loops
-  - [x] async execution
 - [x] authentificaten proxies
   - [x] manage webrtc-leak
   - [x] manage location api leak
   - [ ] proxy per request
-- [ ] add `chrome.scripting` support
 - [ ] add automation tools
   - [x] click
   - [ ] send_keys
   - [ ] find_element
     - [x] by XPATH
 - [ ] undetectability
   - [x] make tab scripts private
@@ -189,7 +267,8 @@
 * [Chrome-devtools-protocol](https://chromedevtools.github.io/devtools-protocol/tot/Fetch/#method-enable)
 * [cdp_event_listeners](https://stackoverflow.com/questions/66227508/selenium-4-0-0-beta-1-how-add-event-listeners-in-cdp)
 * [sync websocket server](https://stackoverflow.com/questions/68939894/implement-a-python-websocket-listener-without-async-asyncio)
 * [chrome-extension-docs](https://developer.chrome.com/docs/extensions/reference/)
 * [PEG-parser](https://github.com/pegjs/pegjs)
 * [make-SV-stayalive](https://stackoverflow.com/a/75082732/20443541)
 * [stringify-obj](https://stackoverflow.com/a/58416333/20443541)
+* [inject code from mv3](https://stackoverflow.com/a/70949953/20443541)
```

### Comparing `selenium_injector-2.2/src/selenium_injector.egg-info/SOURCES.txt` & `selenium_injector-2.3/src/selenium_injector.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,19 +13,18 @@
 src/selenium_injector.egg-info/requires.txt
 src/selenium_injector.egg-info/top_level.txt
 src/selenium_injector/files/extension/background.js
 src/selenium_injector/files/extension/manifest_2.json
 src/selenium_injector/files/extension/manifest_3.json
 src/selenium_injector/files/extension/stay_alive.js
 src/selenium_injector/files/js/connection.js
-src/selenium_injector/files/js/utils.js
-src/selenium_injector/files/tmp/mv2_extension/background.js
-src/selenium_injector/files/tmp/mv2_extension/manifest.json
-src/selenium_injector/files/tmp/mv3_extension/background.js
-src/selenium_injector/files/tmp/mv3_extension/manifest.json
+src/selenium_injector/files/js/returner.js
 src/selenium_injector/scripts/__init__.py
 src/selenium_injector/scripts/injector.py
-src/selenium_injector/scripts/js.py
 src/selenium_injector/scripts/socket.py
 src/selenium_injector/scripts/sync_websocket.py
+src/selenium_injector/types/__init__.py
+src/selenium_injector/types/by.py
+src/selenium_injector/types/js.py
+src/selenium_injector/types/webelement.py
 src/selenium_injector/utils/__init__.py
 src/selenium_injector/utils/utils.py
```

