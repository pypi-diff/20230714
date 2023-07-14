# Comparing `tmp/statute_utils-0.5.6.tar.gz` & `tmp/statute_utils-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_utils-0.5.6.tar", max compression
+gzip compressed data, was "statute_utils-0.5.7.tar", max compression
```

## Comparing `statute_utils-0.5.6.tar` & `statute_utils-0.5.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.5.6/LICENSE
--rw-r--r--   0        0        0     3579 2023-07-14 14:21:25.837838 statute_utils-0.5.6/README.md
--rw-r--r--   0        0        0     1314 2023-07-14 14:18:28.887359 statute_utils-0.5.6/pyproject.toml
--rw-r--r--   0        0        0      664 2023-07-14 12:18:01.173648 statute_utils-0.5.6/statute_utils/__init__.py
--rw-r--r--   0        0        0      460 2023-07-14 10:30:59.403468 statute_utils-0.5.6/statute_utils/components/__init__.py
--rw-r--r--   0        0        0     2108 2023-07-14 14:09:59.832215 statute_utils-0.5.6/statute_utils/components/builder.py
--rw-r--r--   0        0        0    11355 2023-07-14 11:40:42.946792 statute_utils-0.5.6/statute_utils/components/category.py
--rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.5.6/statute_utils/components/short.py
--rw-r--r--   0        0        0     6777 2023-07-08 03:56:13.807355 statute_utils-0.5.6/statute_utils/components/utils.py
--rw-r--r--   0        0        0     4002 2023-07-14 14:03:48.850339 statute_utils-0.5.6/statute_utils/display.py
--rw-r--r--   0        0        0    10207 2023-07-02 03:45:44.226710 statute_utils-0.5.6/statute_utils/main.py
--rw-r--r--   0        0        0     5022 2023-07-02 03:40:02.539984 statute_utils-0.5.6/statute_utils/models.py
--rw-r--r--   0        0        0     9892 2023-07-02 03:43:37.827535 statute_utils-0.5.6/statute_utils/models_names.py
--rw-r--r--   0        0        0     6699 2023-07-02 03:43:23.216281 statute_utils-0.5.6/statute_utils/models_serials.py
--rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.5.6/statute_utils/recipes/__init__.py
--rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.5.6/statute_utils/recipes/const.py
--rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.5.6/statute_utils/recipes/digits.py
--rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.5.6/statute_utils/recipes/roc.py
--rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.5.6/statute_utils/recipes/spain.py
--rw-r--r--   0        0        0       87 2023-07-14 12:22:55.153217 statute_utils-0.5.6/statute_utils/templates/branch.html
--rw-r--r--   0        0        0     1533 2023-07-14 14:11:30.649075 statute_utils-0.5.6/statute_utils/templates/tree.css
--rw-r--r--   0        0        0     1796 2023-07-14 14:05:56.493254 statute_utils-0.5.6/statute_utils/templates/tree.html
--rw-r--r--   0        0        0     6519 2023-07-14 12:30:11.704539 statute_utils-0.5.6/statute_utils/tree.py
--rw-r--r--   0        0        0     4421 1970-01-01 00:00:00.000000 statute_utils-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.5.7/LICENSE
+-rw-r--r--   0        0        0     3593 2023-07-14 16:18:39.431381 statute_utils-0.5.7/README.md
+-rw-r--r--   0        0        0     1314 2023-07-14 17:02:40.274795 statute_utils-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0      678 2023-07-14 16:17:42.904400 statute_utils-0.5.7/statute_utils/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-14 10:30:59.403468 statute_utils-0.5.7/statute_utils/components/__init__.py
+-rw-r--r--   0        0        0     2108 2023-07-14 14:09:59.832215 statute_utils-0.5.7/statute_utils/components/builder.py
+-rw-r--r--   0        0        0    11355 2023-07-14 11:40:42.946792 statute_utils-0.5.7/statute_utils/components/category.py
+-rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.5.7/statute_utils/components/short.py
+-rw-r--r--   0        0        0     6777 2023-07-08 03:56:13.807355 statute_utils-0.5.7/statute_utils/components/utils.py
+-rw-r--r--   0        0        0     3963 2023-07-14 16:17:14.380273 statute_utils-0.5.7/statute_utils/display.py
+-rw-r--r--   0        0        0    10207 2023-07-02 03:45:44.226710 statute_utils-0.5.7/statute_utils/main.py
+-rw-r--r--   0        0        0     5022 2023-07-02 03:40:02.539984 statute_utils-0.5.7/statute_utils/models.py
+-rw-r--r--   0        0        0     9892 2023-07-02 03:43:37.827535 statute_utils-0.5.7/statute_utils/models_names.py
+-rw-r--r--   0        0        0     6699 2023-07-02 03:43:23.216281 statute_utils-0.5.7/statute_utils/models_serials.py
+-rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.5.7/statute_utils/recipes/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.5.7/statute_utils/recipes/const.py
+-rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.5.7/statute_utils/recipes/digits.py
+-rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.5.7/statute_utils/recipes/roc.py
+-rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.5.7/statute_utils/recipes/spain.py
+-rw-r--r--   0        0        0       87 2023-07-14 12:22:55.153217 statute_utils-0.5.7/statute_utils/templates/branch.html
+-rw-r--r--   0        0        0     1114 2023-07-14 18:24:17.829710 statute_utils-0.5.7/statute_utils/templates/tree.css
+-rw-r--r--   0        0        0     2224 2023-07-14 18:27:08.881995 statute_utils-0.5.7/statute_utils/templates/tree.html
+-rw-r--r--   0        0        0     6519 2023-07-14 12:30:11.704539 statute_utils-0.5.7/statute_utils/tree.py
+-rw-r--r--   0        0        0     4435 1970-01-01 00:00:00.000000 statute_utils-0.5.7/PKG-INFO
```

### Comparing `statute_utils-0.5.6/LICENSE` & `statute_utils-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.6/README.md` & `statute_utils-0.5.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 datasette serve db.sqlite --plugins-dir=app/plugins/ {# plus the other arguments #}...
 ```
 
 It becomes possible to use custom functions and filters found in `tree.py` likeso:
 
 ```py title="datasette/plugins/tree.py"
 from datasette import hookimpl
-from statute_utils.display import from_json, is_hidden, is_excluded, from_mp, try_short, set_mp_slug, is_par, md_to_html, build_branch, crumb
+from statute_utils.display import from_json, is_hidden, is_excluded, from_mp, try_short, set_mp_slug, is_par, md_to_html, build_branch, crumb, tree_helpers
 
 @hookimpl
 def prepare_jinja2_environment(env): # custom filters can be used in datasette pages
   env.filters["from_json"] = from_json
   env.filters["is_hidden"] = is_hidden
   env.filters["is_excluded"] = is_excluded
   env.filters["from_mp"] = from_mp
```

### Comparing `statute_utils-0.5.6/pyproject.toml` & `statute_utils-0.5.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statute-utils"
-version = "0.5.6"
+version = "0.5.7"
 description = "Philippine statutory law pattern matching and unit retrieval."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/statute-utils"
 documentation = "https://justmars.github.io/statute-utils"
 classifiers = [
```

### Comparing `statute_utils-0.5.6/statute_utils/__init__.py` & `statute_utils-0.5.7/statute_utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     is_excluded,
     is_hidden,
     is_par,
     ltr,
     set_mp_slug,
     try_short,
 )
-from .display import build_branch, make_statute_string
+from .display import build_branch, make_statute_string, tree_helpers
 from .main import (
     CountedStatute,
     extract_named_rules,
     extract_rule,
     extract_rules,
     extract_serial_rules,
 )
```

### Comparing `statute_utils-0.5.6/statute_utils/components/builder.py` & `statute_utils-0.5.7/statute_utils/components/builder.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.6/statute_utils/components/category.py` & `statute_utils-0.5.7/statute_utils/components/category.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.6/statute_utils/components/short.py` & `statute_utils-0.5.7/statute_utils/components/short.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.6/statute_utils/components/utils.py` & `statute_utils-0.5.7/statute_utils/components/utils.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.6/statute_utils/display.py` & `statute_utils-0.5.7/statute_utils/display.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,17 @@
     is_excluded,
     is_hidden,
     is_par,
     set_mp_slug,
     try_short,
 )
 
-env = Environment(loader=PackageLoader("statute_utils"), autoescape=select_autoescape())
+tree_env = Environment(
+    loader=PackageLoader("statute_utils"), autoescape=select_autoescape()
+)
 
 
 def subtree(node: dict, nodes: list[dict]) -> dict:
     """Recursive function that adds `nodes` as deeply nested _units_
     key of the `node`. It presumes the result of a specific format, e.g.
     if the first `node` passed is `{}` (an empty dict), this will will be populated
     with a `units` key containing the content of the `nodes`:
@@ -96,32 +98,35 @@
 def md_to_html(value: str) -> Markup:
     """Convert markdown text to html.
 
     Args:
         value (str): convert value into html from
 
     Returns:
-        SafeString: Usable in template.
+        Markup: Usable in template.
     """
     exts = [
         "markdown.extensions.tables",
         "markdown.extensions.footnotes",
         "markdown.extensions.md_in_html",
     ]
     return Markup(markdown.markdown(value, extensions=exts))
 
 
+tree_helpers = {
+    "crumb": crumb,
+    "md_to_html": md_to_html,
+    "is_par": is_par,
+    "set_mp_slug": set_mp_slug,
+    "try_short": try_short,
+    "from_mp": from_mp,
+    "is_excluded": is_excluded,
+    "is_hidden": is_hidden,
+    "from_json": from_json,
+}
+tree_env.filters |= tree_helpers
+
+
 def create_html_tree(units: list[dict]) -> str:
-    template = env.get_template("branch.html")
+    template = tree_env.get_template("branch.html")
     result = template.render(units=units)
     return str(result).strip()
-
-
-env.filters["from_json"] = from_json
-env.filters["is_hidden"] = is_hidden
-env.filters["is_excluded"] = is_excluded
-env.filters["from_mp"] = from_mp
-env.filters["try_short"] = try_short
-env.filters["set_mp_slug"] = set_mp_slug
-env.filters["is_par"] = is_par
-env.filters["md_to_html"] = md_to_html
-env.filters["create_html_tree"] = create_html_tree
```

### Comparing `statute_utils-0.5.6/statute_utils/main.py` & `statute_utils-0.5.7/statute_utils/main.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.6/statute_utils/models.py` & `statute_utils-0.5.7/statute_utils/models.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.6/statute_utils/models_names.py` & `statute_utils-0.5.7/statute_utils/models_names.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.6/statute_utils/models_serials.py` & `statute_utils-0.5.7/statute_utils/models_serials.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.6/statute_utils/recipes/digits.py` & `statute_utils-0.5.7/statute_utils/recipes/digits.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.6/statute_utils/recipes/spain.py` & `statute_utils-0.5.7/statute_utils/recipes/spain.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.6/statute_utils/templates/tree.css` & `statute_utils-0.5.7/statute_utils/templates/tree.css`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,53 @@
-article header hgroup h3.crumbs {
-  margin-top: 2em;
+article > header > hgroup > h3.crumbs {
   display: flex;
-  row-gap: 1em;
-  flex-direction: column-reverse;
-}
-  /* This is a little complicated: the tree is built top-down,
-  thus the crumbs will be in top-down order. Citations are read
-  bottom-up, so we first reverse the crumbs (which are marked with
-  class 'crumb' */
-
-section.tree ul { /* Remove top-level indention */
-  padding-left: 0px;
-}
-
-section.tree li {
-  list-style-type: none;
-  margin-bottom: 0.25em;
-  padding-left: 0px;
-  padding-bottom:  0.25em;
-
-  > strong.label::after {
-    content: ". " /* divides item and (caption or content) */
-  }
-
-  > em.label::after {
-    content: " " /* divides caption and content */
-  }
+  flex-direction: row-reverse;
+  flex-wrap: wrap-reverse;
+  justify-content: start;
 
-  > strong.label:hover, em.label:hover
-  {
-    cursor: pointer;
-    text-decoration: underline;
-    text-decoration-color: var(--primary);
-    text-underline-offset: 3px;
-  }
-
-  > div {
-    display:inline; /* markdown convertor can add a <div></div> causing a block, display:inline prevents this. */
-  }
-
-  > div > p {
-    display:inline; /* markdown convertor can add a <div><p></p></div> causing a block on the <p> element, display:inline prevents this. */
-  }
-
-  > p {
-    display:inline; /* markdown convertor can add a <div></div> causing a block, display:inline prevents this. */
+  & span:not(:last-child):before {
+    content: ", "
   }
 }
 
-@media (min-width: 640px) {
-  section.tree ul li {
-    padding-left: 0.7rem; /* Indention > small screens */
-  }
-
-  section.tree ul li[data-par="true"] {
-    padding-left: 0px; /* No indention for paragraphs even if > small screens */
+section.tree {
+  & ul {
+    padding-left: 0px; /* No indent */
+
+    @media (min-width: 640px) {
+      & li {
+        padding-left: 0.7rem; /* Indent since > small screens */
+      }
+
+      & li[data-par="true"] {
+        padding-left: 0px; /* No indent even if > small screens */
+      }
+    }
+  }
+
+  & li {
+    list-style-type: none;
+    margin-bottom: 0.25em;
+    padding-left: 0px;
+    padding-bottom:  0.25em;
+
+    > strong.label::after {
+      content: ". " /* divides item and (caption or content) */
+    }
+
+    > em.label::after {
+      content: " " /* divides caption and content */
+    }
+
+    > strong.label:hover, em.label:hover
+    {
+      cursor: pointer;
+      text-decoration: underline;
+      text-decoration-color: var(--primary);
+      text-underline-offset: 3px;
+    }
+
+    > p {
+      display:inline; /* prevent separate line in a <li>...  because display:inline prevents this. */
+    }
   }
 }
```

### Comparing `statute_utils-0.5.6/statute_utils/tree.py` & `statute_utils-0.5.7/statute_utils/tree.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.6/PKG-INFO` & `statute_utils-0.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statute-utils
-Version: 0.5.6
+Version: 0.5.7
 Summary: Philippine statutory law pattern matching and unit retrieval.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
@@ -136,15 +136,15 @@
 datasette serve db.sqlite --plugins-dir=app/plugins/ {# plus the other arguments #}...
 ```
 
 It becomes possible to use custom functions and filters found in `tree.py` likeso:
 
 ```py title="datasette/plugins/tree.py"
 from datasette import hookimpl
-from statute_utils.display import from_json, is_hidden, is_excluded, from_mp, try_short, set_mp_slug, is_par, md_to_html, build_branch, crumb
+from statute_utils.display import from_json, is_hidden, is_excluded, from_mp, try_short, set_mp_slug, is_par, md_to_html, build_branch, crumb, tree_helpers
 
 @hookimpl
 def prepare_jinja2_environment(env): # custom filters can be used in datasette pages
   env.filters["from_json"] = from_json
   env.filters["is_hidden"] = is_hidden
   env.filters["is_excluded"] = is_excluded
   env.filters["from_mp"] = from_mp
```

