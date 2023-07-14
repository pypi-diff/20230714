# Comparing `tmp/statute_utils-0.5.4.tar.gz` & `tmp/statute_utils-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_utils-0.5.4.tar", max compression
+gzip compressed data, was "statute_utils-0.5.5.tar", max compression
```

## Comparing `statute_utils-0.5.4.tar` & `statute_utils-0.5.5.tar`

### file list

```diff
@@ -1,19 +1,23 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.5.4/LICENSE
--rw-r--r--   0        0        0      898 2023-07-01 01:29:45.722010 statute_utils-0.5.4/README.md
--rw-r--r--   0        0        0     1380 2023-07-08 02:35:12.669952 statute_utils-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      505 2023-07-08 03:56:43.843992 statute_utils-0.5.4/statute_utils/__init__.py
--rw-r--r--   0        0        0      331 2023-07-08 03:56:36.059597 statute_utils-0.5.4/statute_utils/components/__init__.py
--rw-r--r--   0        0        0    10002 2023-07-08 02:39:06.841639 statute_utils-0.5.4/statute_utils/components/category.py
--rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.5.4/statute_utils/components/short.py
--rw-r--r--   0        0        0     6777 2023-07-08 03:56:13.807355 statute_utils-0.5.4/statute_utils/components/utils.py
--rw-r--r--   0        0        0    10207 2023-07-02 03:45:44.226710 statute_utils-0.5.4/statute_utils/main.py
--rw-r--r--   0        0        0     5022 2023-07-02 03:40:02.539984 statute_utils-0.5.4/statute_utils/models.py
--rw-r--r--   0        0        0     9892 2023-07-02 03:43:37.827535 statute_utils-0.5.4/statute_utils/models_names.py
--rw-r--r--   0        0        0     6699 2023-07-02 03:43:23.216281 statute_utils-0.5.4/statute_utils/models_serials.py
--rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.5.4/statute_utils/recipes/__init__.py
--rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.5.4/statute_utils/recipes/const.py
--rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.5.4/statute_utils/recipes/digits.py
--rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.5.4/statute_utils/recipes/roc.py
--rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.5.4/statute_utils/recipes/spain.py
--rw-r--r--   0        0        0     6098 2023-07-08 04:17:18.808301 statute_utils-0.5.4/statute_utils/tree.py
--rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 statute_utils-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.5.5/LICENSE
+-rw-r--r--   0        0        0     3251 2023-07-14 12:56:04.212339 statute_utils-0.5.5/README.md
+-rw-r--r--   0        0        0     1314 2023-07-14 11:47:13.793393 statute_utils-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      664 2023-07-14 12:18:01.173648 statute_utils-0.5.5/statute_utils/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-14 10:30:59.403468 statute_utils-0.5.5/statute_utils/components/__init__.py
+-rw-r--r--   0        0        0     2040 2023-07-14 11:50:07.566656 statute_utils-0.5.5/statute_utils/components/builder.py
+-rw-r--r--   0        0        0    11355 2023-07-14 11:40:42.946792 statute_utils-0.5.5/statute_utils/components/category.py
+-rw-r--r--   0        0        0     2015 2023-07-01 04:37:03.664929 statute_utils-0.5.5/statute_utils/components/short.py
+-rw-r--r--   0        0        0     6777 2023-07-08 03:56:13.807355 statute_utils-0.5.5/statute_utils/components/utils.py
+-rw-r--r--   0        0        0     4007 2023-07-14 12:29:13.214633 statute_utils-0.5.5/statute_utils/display.py
+-rw-r--r--   0        0        0    10207 2023-07-02 03:45:44.226710 statute_utils-0.5.5/statute_utils/main.py
+-rw-r--r--   0        0        0     5022 2023-07-02 03:40:02.539984 statute_utils-0.5.5/statute_utils/models.py
+-rw-r--r--   0        0        0     9892 2023-07-02 03:43:37.827535 statute_utils-0.5.5/statute_utils/models_names.py
+-rw-r--r--   0        0        0     6699 2023-07-02 03:43:23.216281 statute_utils-0.5.5/statute_utils/models_serials.py
+-rw-r--r--   0        0        0      249 2023-07-01 04:12:57.597987 statute_utils-0.5.5/statute_utils/recipes/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.5.5/statute_utils/recipes/const.py
+-rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.5.5/statute_utils/recipes/digits.py
+-rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.5.5/statute_utils/recipes/roc.py
+-rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.5.5/statute_utils/recipes/spain.py
+-rw-r--r--   0        0        0       87 2023-07-14 12:22:55.153217 statute_utils-0.5.5/statute_utils/templates/branch.html
+-rw-r--r--   0        0        0     1594 2023-07-14 12:11:24.940530 statute_utils-0.5.5/statute_utils/templates/macros.html
+-rw-r--r--   0        0        0     6519 2023-07-14 12:30:11.704539 statute_utils-0.5.5/statute_utils/tree.py
+-rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 statute_utils-0.5.5/PKG-INFO
```

### Comparing `statute_utils-0.5.4/LICENSE` & `statute_utils-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.4/pyproject.toml` & `statute_utils-0.5.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statute-utils"
-version = "0.5.4"
+version = "0.5.5"
 description = "Philippine statutory law pattern matching and unit retrieval."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/statute-utils"
 documentation = "https://justmars.github.io/statute-utils"
 classifiers = [
@@ -15,23 +15,22 @@
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-slugify = "^8.0"
 sqlite-utils = "^3.33"
+markdown = "^3.4.3"
+jinja2 = "^3.1.2"
 
 [tool.poetry.group.dev.dependencies]
 python-frontmatter = "^1.0.0" # for testing local decisions
 pytest = "^7.3"
 pytest-cov = "^2.12.1"
 pre-commit = "^3.3"
-mkdocs = "^1.4.3"
-mkdocstrings = {extras = ["python"], version = "^0.22.0"}
-mkdocs-material = "^9.1.15"
 types-python-slugify = "^5.0"
 ipykernel = "^6.23.2"
 
 [tool.pytest.ini_options]
 minversion = "7.3"
 addopts = "-ra -q --cov --doctest-modules"
 filterwarnings = [
```

### Comparing `statute_utils-0.5.4/statute_utils/components/short.py` & `statute_utils-0.5.5/statute_utils/components/short.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.4/statute_utils/components/utils.py` & `statute_utils-0.5.5/statute_utils/components/utils.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.4/statute_utils/main.py` & `statute_utils-0.5.5/statute_utils/main.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.4/statute_utils/models.py` & `statute_utils-0.5.5/statute_utils/models.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.4/statute_utils/models_names.py` & `statute_utils-0.5.5/statute_utils/models_names.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.4/statute_utils/models_serials.py` & `statute_utils-0.5.5/statute_utils/models_serials.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.4/statute_utils/recipes/digits.py` & `statute_utils-0.5.5/statute_utils/recipes/digits.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.4/statute_utils/recipes/spain.py` & `statute_utils-0.5.5/statute_utils/recipes/spain.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.5.4/statute_utils/tree.py` & `statute_utils-0.5.5/statute_utils/tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import datetime
 from collections.abc import Iterator
-from copy import deepcopy
 from pathlib import Path
 from typing import Any, NamedTuple
 
 import yaml
 
 from .components import (
     StatuteSerialCategory,
     StatuteTitle,
     create_fts_snippet_column,
     create_unit_heading,
     set_node_ids,
     walk,
 )
+from .display import create_html_tree
 from .models import STATUTE_DIR, Rule
 
 
 class Statute(NamedTuple):
     """A instance is dependent on a statute path from a fixed
     `STATUTE_DIR`. The shape of the Python object will be different
     from the shape of the dumpable `.yml` export."""
@@ -57,23 +57,31 @@
     def make_row(self) -> dict:
         """All nodes in the tree are marked by a material path.
 
         The units key is manipulated to add a root node. This is
         useful for repeals and other changes since affecting the root node, affects all nodes.
 
         The root node for every key should be `1.`
+
+        A special `html` field exists for the purpose of performance. Since some units
+        are overly large, this creates an unstyled html blob that semantically represents
+        the tree object. The helper functions that were used to create the tree object
+        can be re-used using the same function via filters.
+        ```
         """  # noqa: E501
         set_node_ids(self.units)
+        units = [{"id": "1.", "units": self.units}]
         return {
             "id": self.slug,
             "cat": self.rule.cat.value,
             "num": self.rule.num,
             "date": self.date,
             "variant": self.variant,
-            "units": [{"id": "1.", "units": self.units}],
+            "units": units,
+            "html": create_html_tree(units),
         }
 
     @classmethod
     def flatten_units(
         cls, statute_id: str, units: list[dict[str, Any]], heading: str = ""
     ) -> Iterator[dict[str, str | None]]:
         """Recursive flattening of tree structure where each material path
@@ -139,15 +147,15 @@
                     Laws shall take effect after fifteen days following the
                     completion of their publication either in the Official
                     Gazette or in a newspaper of general circulation in the
                     Philippines, unless it is otherwise provided. (1a)
         ```
         """  # noqa: E501
         cat, num, date, variant = file.parts[-4:]
-        _date = [int(i) for i in date.split("-")]
+        _date = [int(i) for i in date.split("-") if i]
 
         data = yaml.safe_load(file.read_bytes())
         official = data.get("title")
         if not official:
             return None
 
         category = StatuteSerialCategory(cat)
```

