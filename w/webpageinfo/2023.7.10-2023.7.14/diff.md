# Comparing `tmp/webpageinfo-2023.7.10.tar.gz` & `tmp/webpageinfo-2023.7.14.tar.gz`

## Comparing `webpageinfo-2023.7.10.tar` & `webpageinfo-2023.7.14.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/.pre-commit-config.yaml
--rw-r--r--   0        0        0    83903 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/poetry.lock
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/__init__.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/browser.py
--rw-r--r--   0        0        0     9557 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/page.py
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/safe_html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/config/__init__.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/config/ignored_html_tags.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/config/ignored_word_in_tags.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/config/rejected_content_class.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/config/rejected_content_id.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/config/removed_html_tags.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/config/simple_html_tags.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/webpageinfo/config/svg_tags.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/.gitignore
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/LICENSE
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/README.md
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/pyproject.toml
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 webpageinfo-2023.7.10/PKG-INFO
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    83903 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/poetry.lock
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/__init__.py
+-rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/browser.py
+-rw-r--r--   0        0        0     9557 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/page.py
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/safe_html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/config/__init__.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/config/ignored_html_tags.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/config/ignored_word_in_tags.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/config/rejected_content_class.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/config/rejected_content_id.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/config/removed_html_tags.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/config/simple_html_tags.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/config/svg_tags.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/LICENSE
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/README.md
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/pyproject.toml
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/PKG-INFO
```

### Comparing `webpageinfo-2023.7.10/.pre-commit-config.yaml` & `webpageinfo-2023.7.14/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `webpageinfo-2023.7.10/poetry.lock` & `webpageinfo-2023.7.14/poetry.lock`

 * *Files identical despite different names*

### Comparing `webpageinfo-2023.7.10/webpageinfo/browser.py` & `webpageinfo-2023.7.14/webpageinfo/browser.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,43 +5,65 @@
 
 
 class WebElementNotFound(Exception):
     pass
 
 
 def _find_elements_by(
-    root, tag: str = "", class_name: str = "", css: str = "", wait_time: float = 0
+    root,
+    tag: str = "",
+    class_name: str = "",
+    css: str = "",
+    xpath: str = "",
+    wait_time: float = 0,
 ) -> Iterable["WebElement"]:
     if tag:
         for elem in root.find_by_tag(tag, wait_time):
             yield WebElement(elem)
     if class_name:
         for elem in root.find_by_css(f".{class_name}", wait_time):
             yield WebElement(elem)
     if css:
         for elem in root.find_by_css(css, wait_time):
             yield WebElement(elem)
+    if xpath:
+        for elem in root.find_by_xpath(xpath, wait_time):
+            yield WebElement(elem)
 
 
 class _Findable:
     @property
     def _root(self):
         raise NotImplementedError
 
     def find_elements_by(
-        self, tag: str = "", class_name: str = "", css: str = "", wait_time: float = 0
+        self,
+        tag: str = "",
+        class_name: str = "",
+        css: str = "",
+        xpath: str = "",
+        wait_time: float = 0,
     ) -> Iterable["WebElement"]:
-        yield from _find_elements_by(self._root, tag, class_name, css, wait_time)
+        yield from _find_elements_by(self._root, tag, class_name, css, xpath, wait_time)
 
     def find_element_by(
-        self, tag: str = "", class_name: str = "", css: str = "", wait_time: float = 0
+        self,
+        tag: str = "",
+        class_name: str = "",
+        css: str = "",
+        xpath: str = "",
+        wait_time: float = 0,
     ) -> "WebElement":
         try:
             return next(
-                iter(_find_elements_by(self._root, tag, class_name, css, wait_time))
+                iter(
+                    _find_elements_by(
+                        self._root, tag, class_name, css, xpath, wait_time
+                    )
+                )
             )
         except StopIteration:
             raise WebElementNotFound
 
     def is_element_present_by(self, tag: str = "", wait_time: float = 0) -> bool:
         if tag:
             return self._root.is_element_present_by_tag(tag)
```

### Comparing `webpageinfo-2023.7.10/webpageinfo/page.py` & `webpageinfo-2023.7.14/webpageinfo/page.py`

 * *Files identical despite different names*

### Comparing `webpageinfo-2023.7.10/webpageinfo/safe_html.py` & `webpageinfo-2023.7.14/webpageinfo/safe_html.py`

 * *Files identical despite different names*

### Comparing `webpageinfo-2023.7.10/webpageinfo/config/ignored_word_in_tags.py` & `webpageinfo-2023.7.14/webpageinfo/config/ignored_word_in_tags.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     "faites",
     "fait",
     "faits",
     "first",
     "following",
     "for",
     "from",
+    "grâce",
     "how",
     "however",
     "http",
     "https",
     "ils",
     "import",
     "included",
```

### Comparing `webpageinfo-2023.7.10/.gitignore` & `webpageinfo-2023.7.14/.gitignore`

 * *Files identical despite different names*

### Comparing `webpageinfo-2023.7.10/LICENSE` & `webpageinfo-2023.7.14/LICENSE`

 * *Files identical despite different names*

### Comparing `webpageinfo-2023.7.10/pyproject.toml` & `webpageinfo-2023.7.14/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "webpageinfo"
-version = "2023.7.10"
+version = "2023.7.14"
 description = "Web page information (title, content, tags…)"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
@@ -29,15 +29,16 @@
 dev = [
     "python-dev-tools >= 2023",
     "pre-commit >=3,<4",
 ]
 
 [project.urls]
 "Source code" = "https://github.com/vpoulailleau/webpageinfo"
-documentation = "https://webpageinfo.readthedocs.io/en/latest/"
+Repository = "https://github.com/vpoulailleau/webpageinfo"
+Documentation = "https://webpageinfo.readthedocs.io/en/latest/"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
   ".gitignore",
   "/.github",
   "/docs",
 ]
@@ -57,8 +58,8 @@
 exclude_lines = [
     "pragma: no cover",
     "if TYPE_CHECKING:",
 ]
 
 [build-system]
 requires = ["hatchling"]
-build-backend = "hatchling.build" 
+build-backend = "hatchling.build"
```

### Comparing `webpageinfo-2023.7.10/PKG-INFO` & `webpageinfo-2023.7.14/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: webpageinfo
-Version: 2023.7.10
+Version: 2023.7.14
 Summary: Web page information (title, content, tags…)
 Project-URL: Source code, https://github.com/vpoulailleau/webpageinfo
-Project-URL: documentation, https://webpageinfo.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/vpoulailleau/webpageinfo
+Project-URL: Documentation, https://webpageinfo.readthedocs.io/en/latest/
 Author-email: Vincent Poulailleau <vpoulailleau@gmail.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Keywords: information,page,web
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

