# Comparing `tmp/lamin_logger-0.7.6.tar.gz` & `tmp/lamin_logger-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamin_logger-0.7.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamin_logger-0.7.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamin_logger-0.7.6.tar` & `lamin_logger-0.7.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.7.6/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.7.6/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.7.6/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.7.6/.gitignore
--rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.7.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.7.6/LICENSE
--rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.7.6/README.md
--rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.7.6/docs/api.md
--rw-r--r--   0        0        0     5120 2023-07-10 09:56:13.936880 lamin_logger-0.7.6/docs/changelog.md
--rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.7.6/docs/index.md
--rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.7.6/docs/quickstart.ipynb
--rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.7.6/lamin-project.yaml
--rw-r--r--   0        0        0      291 2023-07-10 09:56:03.461997 lamin_logger-0.7.6/lamin_logger/__init__.py
--rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.7.6/lamin_logger/_core.py
--rw-r--r--   0        0        0     3825 2023-06-29 16:02:11.111265 lamin_logger-0.7.6/lamin_logger/_inspect.py
--rw-r--r--   0        0        0     7332 2023-07-05 09:32:09.706797 lamin_logger-0.7.6/lamin_logger/_logger.py
--rw-r--r--   0        0        0     4202 2023-07-05 07:03:18.906964 lamin_logger-0.7.6/lamin_logger/_lookup.py
--rw-r--r--   0        0        0     7541 2023-07-10 09:54:24.354366 lamin_logger-0.7.6/lamin_logger/_map_synonyms.py
--rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.7.6/lamin_logger/_python_version.py
--rw-r--r--   0        0        0     3524 2023-07-10 09:54:24.354688 lamin_logger-0.7.6/lamin_logger/_search.py
--rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.7.6/noxfile.py
--rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.7.6/pyproject.toml
--rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.7.6/tests/test_base.py
--rw-r--r--   0        0        0     4154 2023-06-22 14:19:30.503574 lamin_logger-0.7.6/tests/test_inspect.py
--rw-r--r--   0        0        0     1608 2023-06-19 17:49:41.483785 lamin_logger-0.7.6/tests/test_lookup.py
--rw-r--r--   0        0        0     5965 2023-06-30 14:10:22.361575 lamin_logger-0.7.6/tests/test_map_synonyms.py
--rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.7.6/tests/test_notebooks.py
--rw-r--r--   0        0        0     2701 2023-06-19 17:49:41.484369 lamin_logger-0.7.6/tests/test_search.py
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.7.7/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.7.7/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.7.7/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.7.7/.gitignore
+-rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.7.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.7.7/LICENSE
+-rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.7.7/README.md
+-rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.7.7/docs/api.md
+-rw-r--r--   0        0        0     5269 2023-07-14 11:49:04.376377 lamin_logger-0.7.7/docs/changelog.md
+-rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.7.7/docs/index.md
+-rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.7.7/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.7.7/lamin-project.yaml
+-rw-r--r--   0        0        0      291 2023-07-14 11:48:56.688696 lamin_logger-0.7.7/lamin_logger/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.7.7/lamin_logger/_core.py
+-rw-r--r--   0        0        0     3825 2023-06-29 16:02:11.111265 lamin_logger-0.7.7/lamin_logger/_inspect.py
+-rw-r--r--   0        0        0     7332 2023-07-05 09:32:09.706797 lamin_logger-0.7.7/lamin_logger/_logger.py
+-rw-r--r--   0        0        0     4202 2023-07-05 07:03:18.906964 lamin_logger-0.7.7/lamin_logger/_lookup.py
+-rw-r--r--   0        0        0     7410 2023-07-14 11:45:47.889453 lamin_logger-0.7.7/lamin_logger/_map_synonyms.py
+-rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.7.7/lamin_logger/_python_version.py
+-rw-r--r--   0        0        0     3524 2023-07-10 09:54:24.354688 lamin_logger-0.7.7/lamin_logger/_search.py
+-rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.7.7/noxfile.py
+-rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.7.7/tests/test_base.py
+-rw-r--r--   0        0        0     4154 2023-06-22 14:19:30.503574 lamin_logger-0.7.7/tests/test_inspect.py
+-rw-r--r--   0        0        0     1608 2023-06-19 17:49:41.483785 lamin_logger-0.7.7/tests/test_lookup.py
+-rw-r--r--   0        0        0     6153 2023-07-14 11:45:47.889627 lamin_logger-0.7.7/tests/test_map_synonyms.py
+-rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.7.7/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2701 2023-06-19 17:49:41.484369 lamin_logger-0.7.7/tests/test_search.py
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.7.7/PKG-INFO
```

### Comparing `lamin_logger-0.7.6/.github/workflows/build.yml` & `lamin_logger-0.7.7/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.6/.github/workflows/latest-changes.yml` & `lamin_logger-0.7.7/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.6/.gitignore` & `lamin_logger-0.7.7/.gitignore`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.6/.pre-commit-config.yaml` & `lamin_logger-0.7.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.6/LICENSE` & `lamin_logger-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.6/docs/changelog.md` & `lamin_logger-0.7.7/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🐛 Fix map_synonyms bug | [36](https://github.com/laminlabs/lamin-logger/pull/36) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-14 | 0.7.7
 ⚡️ Speed up search 150x | [35](https://github.com/laminlabs/lamin-logger/pull/35) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-10 | 0.7.6
 🐛 Fix existing_categories for map_synonyms | [34](https://github.com/laminlabs/lamin-logger/pull/34) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-05 | 0.7.5
 🚑️ Fix for multiple matches in map_synonyms | [33](https://github.com/laminlabs/lamin-logger/pull/33) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-02 | 0.7.4
 🚑️ Handles categorical input | [32](https://github.com/laminlabs/lamin-logger/pull/32) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-30 | 0.7.3
 🐛 Fix case sensitivity in map_synonyms | [31](https://github.com/laminlabs/lamin-logger/pull/31) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-22 | 0.7.1
 🚚 Moved inspect from bionty | [30](https://github.com/laminlabs/lamin-logger/pull/30) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-21 | 0.7.0
 🚑️ Map_synonyms only returns mapped synonyms not names | [29](https://github.com/laminlabs/lamin-logger/pull/29) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-20 | 0.6.2
```

### Comparing `lamin_logger-0.7.6/docs/quickstart.ipynb` & `lamin_logger-0.7.7/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.6/lamin_logger/_core.py` & `lamin_logger-0.7.7/lamin_logger/_core.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.6/lamin_logger/_inspect.py` & `lamin_logger-0.7.7/lamin_logger/_inspect.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.6/lamin_logger/_logger.py` & `lamin_logger-0.7.7/lamin_logger/_logger.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.6/lamin_logger/_lookup.py` & `lamin_logger-0.7.7/lamin_logger/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.6/lamin_logger/_map_synonyms.py` & `lamin_logger-0.7.7/lamin_logger/_map_synonyms.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,18 +66,17 @@
     # __agg__ is a column of identifiers based on case_sensitive
     df["__agg__"] = to_str(df[field], case_sensitive=case_sensitive)
     field_map = pd.merge(mapped_df, df, on="__agg__").set_index("__agg__")[field]
 
     # only runs if synonyms mapping is needed
     # unique of field_map is needed here due to possible multiple matches of identifier
     if len(field_map.unique()) < mapped_df.shape[0]:
-        # only map synonyms for those ids that don't match the field case insensitively
         # {synonym: name}
         syn_map = explode_aggregated_column_to_map(
-            df=df[~df["__agg__"].isin(mapped_df["__agg__"])],
+            df=df,
             agg_col=synonyms_field,
             target_col=field,
             keep=keep,
             sep=sep,
         )
 
         if not case_sensitive:
```

### Comparing `lamin_logger-0.7.6/lamin_logger/_python_version.py` & `lamin_logger-0.7.7/lamin_logger/_python_version.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.6/lamin_logger/_search.py` & `lamin_logger-0.7.7/lamin_logger/_search.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.6/pyproject.toml` & `lamin_logger-0.7.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.6/tests/test_inspect.py` & `lamin_logger-0.7.7/tests/test_inspect.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.6/tests/test_lookup.py` & `lamin_logger-0.7.7/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.6/tests/test_map_synonyms.py` & `lamin_logger-0.7.7/tests/test_map_synonyms.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,21 @@
 def test_map_synonyms(genes):
     gene_symbols, df = genes
 
     mapping = map_synonyms(df=df, identifiers=gene_symbols, field="symbol")
     assert mapping == ["A1CF", "A1BG", "BRCA2", "FANCD20", "GCLC"]
 
 
+def test_map_synonyms_field_synonym(genes):
+    _, df = genes
+
+    mapping = map_synonyms(df=df, identifiers=["BRCA1", "BRCC1"], field="symbol")
+    assert mapping == ["BRCA1", "BRCA1"]
+
+
 def test_map_synonyms_return_mapper(genes):
     gene_symbols, df = genes
 
     mapper = map_synonyms(
         df=df, identifiers=gene_symbols, field="symbol", return_mapper=True
     )
```

### Comparing `lamin_logger-0.7.6/tests/test_search.py` & `lamin_logger-0.7.7/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.7.6/PKG-INFO` & `lamin_logger-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamin_logger
-Version: 0.7.6
+Version: 0.7.7
 Summary: Logging setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

