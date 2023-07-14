# Comparing `tmp/lxd-sphinx-extensions-0.0.7.tar.gz` & `tmp/lxd-sphinx-extensions-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lxd-sphinx-extensions-0.0.7.tar", last modified: Mon Mar 13 10:16:29 2023, max compression
+gzip compressed data, was "lxd-sphinx-extensions-0.0.8.tar", last modified: Fri Jul 14 11:28:21 2023, max compression
```

## Comparing `lxd-sphinx-extensions-0.0.7.tar` & `lxd-sphinx-extensions-0.0.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-13 10:16:29.485232 lxd-sphinx-extensions-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2023-03-13 10:16:19.000000 lxd-sphinx-extensions-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       17 2023-03-13 10:16:19.000000 lxd-sphinx-extensions-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     8872 2023-03-13 10:16:29.485232 lxd-sphinx-extensions-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     8544 2023-03-13 10:16:19.000000 lxd-sphinx-extensions-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-13 10:16:29.481232 lxd-sphinx-extensions-0.0.7/config-options/
--rw-r--r--   0 runner    (1001) docker     (116)     5941 2023-03-13 10:16:19.000000 lxd-sphinx-extensions-0.0.7/config-options/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-13 10:16:29.485232 lxd-sphinx-extensions-0.0.7/config-options/_static/
--rw-r--r--   0 runner    (1001) docker     (116)      640 2023-03-13 10:16:19.000000 lxd-sphinx-extensions-0.0.7/config-options/_static/config-options.css
--rw-r--r--   0 runner    (1001) docker     (116)      866 2023-03-13 10:16:19.000000 lxd-sphinx-extensions-0.0.7/config-options/_static/config-options.js
--rw-r--r--   0 runner    (1001) docker     (116)      717 2023-03-13 10:16:19.000000 lxd-sphinx-extensions-0.0.7/config-options/common.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-13 10:16:29.485232 lxd-sphinx-extensions-0.0.7/custom-rst-roles/
--rw-r--r--   0 runner    (1001) docker     (116)      338 2023-03-13 10:16:19.000000 lxd-sphinx-extensions-0.0.7/custom-rst-roles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-13 10:16:29.485232 lxd-sphinx-extensions-0.0.7/lxd_sphinx_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     8872 2023-03-13 10:16:29.000000 lxd-sphinx-extensions-0.0.7/lxd_sphinx_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      714 2023-03-13 10:16:29.000000 lxd-sphinx-extensions-0.0.7/lxd_sphinx_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-13 10:16:29.000000 lxd-sphinx-extensions-0.0.7/lxd_sphinx_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       40 2023-03-13 10:16:29.000000 lxd-sphinx-extensions-0.0.7/lxd_sphinx_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       76 2023-03-13 10:16:29.000000 lxd-sphinx-extensions-0.0.7/lxd_sphinx_extensions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       85 2023-03-13 10:16:19.000000 lxd-sphinx-extensions-0.0.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-13 10:16:29.485232 lxd-sphinx-extensions-0.0.7/related-links/
--rw-r--r--   0 runner    (1001) docker     (116)     4003 2023-03-13 10:16:19.000000 lxd-sphinx-extensions-0.0.7/related-links/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-13 10:16:29.485232 lxd-sphinx-extensions-0.0.7/related-links/_static/
--rw-r--r--   0 runner    (1001) docker     (116)     1180 2023-03-13 10:16:19.000000 lxd-sphinx-extensions-0.0.7/related-links/_static/related-links.css
--rw-r--r--   0 runner    (1001) docker     (116)      717 2023-03-13 10:16:19.000000 lxd-sphinx-extensions-0.0.7/related-links/common.py
--rw-r--r--   0 runner    (1001) docker     (116)      585 2023-03-13 10:16:29.489232 lxd-sphinx-extensions-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-13 10:16:29.485232 lxd-sphinx-extensions-0.0.7/terminal-output/
--rw-r--r--   0 runner    (1001) docker     (116)     2304 2023-03-13 10:16:19.000000 lxd-sphinx-extensions-0.0.7/terminal-output/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-13 10:16:29.485232 lxd-sphinx-extensions-0.0.7/terminal-output/_static/
--rw-r--r--   0 runner    (1001) docker     (116)      510 2023-03-13 10:16:19.000000 lxd-sphinx-extensions-0.0.7/terminal-output/_static/terminal-output.css
--rw-r--r--   0 runner    (1001) docker     (116)      717 2023-03-13 10:16:19.000000 lxd-sphinx-extensions-0.0.7/terminal-output/common.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-13 10:16:29.485232 lxd-sphinx-extensions-0.0.7/youtube-links/
--rw-r--r--   0 runner    (1001) docker     (116)     1575 2023-03-13 10:16:19.000000 lxd-sphinx-extensions-0.0.7/youtube-links/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-13 10:16:29.485232 lxd-sphinx-extensions-0.0.7/youtube-links/_static/
--rw-r--r--   0 runner    (1001) docker     (116)      441 2023-03-13 10:16:19.000000 lxd-sphinx-extensions-0.0.7/youtube-links/_static/youtube.css
--rw-r--r--   0 runner    (1001) docker     (116)      717 2023-03-13 10:16:19.000000 lxd-sphinx-extensions-0.0.7/youtube-links/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.707597 lxd-sphinx-extensions-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-14 11:28:21.707597 lxd-sphinx-extensions-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.703597 lxd-sphinx-extensions-0.0.8/config-options/
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/config-options/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.703597 lxd-sphinx-extensions-0.0.8/config-options/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/config-options/_static/config-options.css
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/config-options/_static/config-options.js
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/config-options/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.703597 lxd-sphinx-extensions-0.0.8/custom-rst-roles/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/custom-rst-roles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.703597 lxd-sphinx-extensions-0.0.8/lxd_sphinx_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-14 11:28:21.000000 lxd-sphinx-extensions-0.0.8/lxd_sphinx_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-14 11:28:21.000000 lxd-sphinx-extensions-0.0.8/lxd_sphinx_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:28:21.000000 lxd-sphinx-extensions-0.0.8/lxd_sphinx_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 11:28:21.000000 lxd-sphinx-extensions-0.0.8/lxd_sphinx_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-14 11:28:21.000000 lxd-sphinx-extensions-0.0.8/lxd_sphinx_extensions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.703597 lxd-sphinx-extensions-0.0.8/related-links/
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/related-links/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.703597 lxd-sphinx-extensions-0.0.8/related-links/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/related-links/_static/related-links.css
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/related-links/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-14 11:28:21.707597 lxd-sphinx-extensions-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.707597 lxd-sphinx-extensions-0.0.8/terminal-output/
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/terminal-output/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.707597 lxd-sphinx-extensions-0.0.8/terminal-output/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/terminal-output/_static/terminal-output.css
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/terminal-output/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.707597 lxd-sphinx-extensions-0.0.8/youtube-links/
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/youtube-links/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:28:21.707597 lxd-sphinx-extensions-0.0.8/youtube-links/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/youtube-links/_static/youtube.css
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-14 11:28:13.000000 lxd-sphinx-extensions-0.0.8/youtube-links/common.py
```

### Comparing `lxd-sphinx-extensions-0.0.7/LICENSE` & `lxd-sphinx-extensions-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.7/PKG-INFO` & `lxd-sphinx-extensions-0.0.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxd-sphinx-extensions
-Version: 0.0.7
+Version: 0.0.8
 Summary: A collection of Sphinx extensions used in LXD
 Home-page: https://github.com/canonical/lxd-sphinx-extensions
 Author: Ruth Fuchss
 Author-email: ruth.fuchss@canonical.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -41,14 +41,23 @@
 If you want to add Discourse links, you must also configure the prefix for your Discourse instance in the `html_context` variable:
 
     html_context = {
                     (...),
                     "discourse_prefix": "https://discuss.linuxcontainers.org/t/"
                    }
 
+You can configure different Discourse prefixes by specifying a dict:
+
+    html_context = {
+                    (...),
+                    "discourse_prefix": {
+                        "lxc": "https://discuss.linuxcontainers.org/t/",
+                        "ubuntu": "https://discourse.ubuntu.com/t/"}
+                    }
+
 #### Add related links to the template
 
 The extension provides two functions that can be used in your template:
 
 * `discourse_links(meta.discourse)`: Returns an unordered list (`<ul>`) of Discourse links.
 * `related_links(meta.relatedlinks)`: Returns an unordered list (`<ul>`) of related links.
 
@@ -103,14 +112,15 @@
 You can override these styles or define your own, depending on the theme and template that you use.
 
 #### Specify links for a page
 
 Specify your Discourse links and related links in the metadata at the top of the page.
 
 For Discourse links, specify only the topic IDs (in a comma-separated list).
+If you have defined several Discourse prefixes, specify both key and ID (for example, `abc:1234`).
 
 For related links, specify the full URLs (in a comma-separated list).
 The link text is extracted automatically or can be specified in Markdown syntax.
 Note that spaces are ignored; if you need spaces in the title, replace them with `&#32;`.
 If Sphinx complains about the metadata value because it starts with "[", enclose the full value in double quotes.
 
 The following example uses MyST syntax for the metadata:
```

### Comparing `lxd-sphinx-extensions-0.0.7/README.md` & `lxd-sphinx-extensions-0.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,23 @@
 If you want to add Discourse links, you must also configure the prefix for your Discourse instance in the `html_context` variable:
 
     html_context = {
                     (...),
                     "discourse_prefix": "https://discuss.linuxcontainers.org/t/"
                    }
 
+You can configure different Discourse prefixes by specifying a dict:
+
+    html_context = {
+                    (...),
+                    "discourse_prefix": {
+                        "lxc": "https://discuss.linuxcontainers.org/t/",
+                        "ubuntu": "https://discourse.ubuntu.com/t/"}
+                    }
+
 #### Add related links to the template
 
 The extension provides two functions that can be used in your template:
 
 * `discourse_links(meta.discourse)`: Returns an unordered list (`<ul>`) of Discourse links.
 * `related_links(meta.relatedlinks)`: Returns an unordered list (`<ul>`) of related links.
 
@@ -92,14 +101,15 @@
 You can override these styles or define your own, depending on the theme and template that you use.
 
 #### Specify links for a page
 
 Specify your Discourse links and related links in the metadata at the top of the page.
 
 For Discourse links, specify only the topic IDs (in a comma-separated list).
+If you have defined several Discourse prefixes, specify both key and ID (for example, `abc:1234`).
 
 For related links, specify the full URLs (in a comma-separated list).
 The link text is extracted automatically or can be specified in Markdown syntax.
 Note that spaces are ignored; if you need spaces in the title, replace them with `&#32;`.
 If Sphinx complains about the metadata value because it starts with "[", enclose the full value in double quotes.
 
 The following example uses MyST syntax for the metadata:
```

### Comparing `lxd-sphinx-extensions-0.0.7/config-options/__init__.py` & `lxd-sphinx-extensions-0.0.8/config-options/__init__.py`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.7/config-options/_static/config-options.css` & `lxd-sphinx-extensions-0.0.8/config-options/_static/config-options.css`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.7/config-options/_static/config-options.js` & `lxd-sphinx-extensions-0.0.8/config-options/_static/config-options.js`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.7/config-options/common.py` & `lxd-sphinx-extensions-0.0.8/config-options/common.py`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.7/lxd_sphinx_extensions.egg-info/PKG-INFO` & `lxd-sphinx-extensions-0.0.8/lxd_sphinx_extensions.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxd-sphinx-extensions
-Version: 0.0.7
+Version: 0.0.8
 Summary: A collection of Sphinx extensions used in LXD
 Home-page: https://github.com/canonical/lxd-sphinx-extensions
 Author: Ruth Fuchss
 Author-email: ruth.fuchss@canonical.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -41,14 +41,23 @@
 If you want to add Discourse links, you must also configure the prefix for your Discourse instance in the `html_context` variable:
 
     html_context = {
                     (...),
                     "discourse_prefix": "https://discuss.linuxcontainers.org/t/"
                    }
 
+You can configure different Discourse prefixes by specifying a dict:
+
+    html_context = {
+                    (...),
+                    "discourse_prefix": {
+                        "lxc": "https://discuss.linuxcontainers.org/t/",
+                        "ubuntu": "https://discourse.ubuntu.com/t/"}
+                    }
+
 #### Add related links to the template
 
 The extension provides two functions that can be used in your template:
 
 * `discourse_links(meta.discourse)`: Returns an unordered list (`<ul>`) of Discourse links.
 * `related_links(meta.relatedlinks)`: Returns an unordered list (`<ul>`) of related links.
 
@@ -103,14 +112,15 @@
 You can override these styles or define your own, depending on the theme and template that you use.
 
 #### Specify links for a page
 
 Specify your Discourse links and related links in the metadata at the top of the page.
 
 For Discourse links, specify only the topic IDs (in a comma-separated list).
+If you have defined several Discourse prefixes, specify both key and ID (for example, `abc:1234`).
 
 For related links, specify the full URLs (in a comma-separated list).
 The link text is extracted automatically or can be specified in Markdown syntax.
 Note that spaces are ignored; if you need spaces in the title, replace them with `&#32;`.
 If Sphinx complains about the metadata value because it starts with "[", enclose the full value in double quotes.
 
 The following example uses MyST syntax for the metadata:
```

### Comparing `lxd-sphinx-extensions-0.0.7/lxd_sphinx_extensions.egg-info/SOURCES.txt` & `lxd-sphinx-extensions-0.0.8/lxd_sphinx_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.7/related-links/__init__.py` & `lxd-sphinx-extensions-0.0.8/related-links/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,14 +13,30 @@
 #   the top of the page using the tag "discourse".
 #   For example (in MyST syntax):
 #
 #   ---
 #   discourse: 12033,13128
 #   ---
 #
+#   You can use different Discourse instances by defining prefixes
+#   for each instance. For example:
+#
+#   html_context = {
+#       "discourse_prefix": {
+#           "lxc": "https://discuss.linuxcontainers.org/t/",
+#           "ubuntu": "https://discourse.ubuntu.com/t/"
+#       }
+#   }
+#
+#   Use these prefixes when linking (no prefix = first dict entry)
+#
+#   ---
+#   discourse: ubuntu:12033,lxc:13128
+#   ---
+#
 # - Add related URLs to the metadata at the top of the page using
 #   the tag "relatedlinks". The link text is extracted automatically
 #   or can be specified in Markdown syntax. Note that spaces are
 #   ignored; if you need spaces in the title, replace them with &#32;.
 #   Some examples (in MyST syntax):
 #
 #   ---
@@ -41,42 +57,64 @@
 # For both ways, check for errors in the output. Invalid links are
 # not added to the output.
 ######################################################################
 
 import requests
 import json
 from bs4 import BeautifulSoup
+from sphinx.util import logging
 from . import common
 
 cache = {}
+logger = logging.getLogger(__name__)
 
 
 def setup_func(app, pagename, templatename, context, doctree):
     def discourse_links(IDlist):
 
         if context["discourse_prefix"] and IDlist:
 
             posts = IDlist.strip().replace(" ", "").split(",")
 
             linklist = "<ul>"
 
             for post in posts:
                 title = ""
-                linkurl = context["discourse_prefix"] + post
+
+                if type(context["discourse_prefix"]) is dict:
+                    ID = post.split(":")
+                    if len(ID) == 1:
+                        linkurl = list(
+                            context["discourse_prefix"].values()
+                        )[0] + post
+                    elif ID[0] in context["discourse_prefix"]:
+                        linkurl = context["discourse_prefix"][ID[0]] + ID[1]
+                    else:
+                        logger.warning(
+                            pagename
+                            + ": Discourse prefix "
+                            + ID[0]
+                            + " is not defined."
+                        )
+                        continue
+                else:
+                    linkurl = context["discourse_prefix"] + post
 
                 if post in cache:
                     title = cache[post]
                 else:
                     try:
                         r = requests.get(linkurl + ".json")
                         r.raise_for_status()
                         title = json.loads(r.text)["title"]
                         cache[post] = title
                     except requests.HTTPError as err:
-                        print(err)
+                        logger.warning(pagename + ": " + str(err))
+                    except requests.ConnectionError as err:
+                        logger.warning(pagename + ": " + str(err))
 
                 if title:
                     linklist += '<li><a href="' + linkurl
                     linklist += '" target="_blank">' + title + "</a></li>"
 
             linklist += "</ul>"
 
@@ -103,18 +141,28 @@
                     title = split[0][1:]
                     link = split[2][:-1]
                 else:
                     try:
                         r = requests.get(link)
                         r.raise_for_status()
                         soup = BeautifulSoup(r.text, "html.parser")
-                        title = soup.title.get_text()
-                        cache[link] = title
+                        if soup is None:
+                            logger.warning(
+                                pagename
+                                + ": "
+                                + link
+                                + " doesn't have a title."
+                            )
+                        else:
+                            title = soup.title.get_text()
+                            cache[link] = title
                     except requests.HTTPError as err:
-                        print(err)
+                        logger.warning(pagename + ": " + str(err))
+                    except requests.ConnectionError as err:
+                        logger.warning(pagename + ": " + str(err))
 
                 if title:
                     linklist += '<li><a href="' + link + '" target="_blank">'
                     linklist += title + "</a></li>"
 
             linklist += "</ul>"
```

### Comparing `lxd-sphinx-extensions-0.0.7/related-links/_static/related-links.css` & `lxd-sphinx-extensions-0.0.8/related-links/_static/related-links.css`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.7/related-links/common.py` & `lxd-sphinx-extensions-0.0.8/related-links/common.py`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.7/setup.cfg` & `lxd-sphinx-extensions-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lxd-sphinx-extensions
-version = 0.0.7
+version = 0.0.8
 author = Ruth Fuchss
 author_email = ruth.fuchss@canonical.com
 description = A collection of Sphinx extensions used in LXD
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/canonical/lxd-sphinx-extensions
```

### Comparing `lxd-sphinx-extensions-0.0.7/terminal-output/__init__.py` & `lxd-sphinx-extensions-0.0.8/terminal-output/__init__.py`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.7/terminal-output/common.py` & `lxd-sphinx-extensions-0.0.8/terminal-output/common.py`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.7/youtube-links/__init__.py` & `lxd-sphinx-extensions-0.0.8/youtube-links/__init__.py`

 * *Files identical despite different names*

### Comparing `lxd-sphinx-extensions-0.0.7/youtube-links/common.py` & `lxd-sphinx-extensions-0.0.8/youtube-links/common.py`

 * *Files identical despite different names*

