# Comparing `tmp/ogc_na-0.3.2.tar.gz` & `tmp/ogc_na-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogc_na-0.3.2.tar", last modified: Thu Jul 13 12:32:16 2023, max compression
+gzip compressed data, was "ogc_na-0.3.3.tar", last modified: Fri Jul 14 06:31:54 2023, max compression
```

## Comparing `ogc_na-0.3.2.tar` & `ogc_na-0.3.3.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:32:16.579192 ogc_na-0.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:32:16.571192 ogc_na-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:32:16.575192 ogc_na-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-13 12:32:02.000000 ogc_na-0.3.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-07-13 12:32:02.000000 ogc_na-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-13 12:32:02.000000 ogc_na-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-13 12:32:16.579192 ogc_na-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-13 12:32:02.000000 ogc_na-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:32:16.575192 ogc_na-0.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-07-13 12:32:02.000000 ogc_na-0.3.2/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-13 12:32:02.000000 ogc_na-0.3.2/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-13 12:32:02.000000 ogc_na-0.3.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-13 12:32:02.000000 ogc_na-0.3.2/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-13 12:32:02.000000 ogc_na-0.3.2/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:32:16.571192 ogc_na-0.3.2/ogc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:32:16.575192 ogc_na-0.3.2/ogc/na/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-13 12:32:02.000000 ogc_na-0.3.2/ogc/na/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 12:32:16.000000 ogc_na-0.3.2/ogc/na/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    33816 2023-07-13 12:32:02.000000 ogc_na-0.3.2/ogc/na/annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-07-13 12:32:02.000000 ogc_na-0.3.2/ogc/na/domain_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-13 12:32:02.000000 ogc_na-0.3.2/ogc/na/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-13 12:32:02.000000 ogc_na-0.3.2/ogc/na/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    35338 2023-07-13 12:32:02.000000 ogc_na-0.3.2/ogc/na/ingest_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:32:16.575192 ogc_na-0.3.2/ogc/na/input_filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-13 12:32:02.000000 ogc_na-0.3.2/ogc/na/input_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-13 12:32:02.000000 ogc_na-0.3.2/ogc/na/input_filters/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    16477 2023-07-13 12:32:02.000000 ogc_na-0.3.2/ogc/na/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-13 12:32:02.000000 ogc_na-0.3.2/ogc/na/provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    18229 2023-07-13 12:32:02.000000 ogc_na-0.3.2/ogc/na/update_vocabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-07-13 12:32:02.000000 ogc_na-0.3.2/ogc/na/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-13 12:32:02.000000 ogc_na-0.3.2/ogc/na/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:32:16.575192 ogc_na-0.3.2/ogc_na.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-13 12:32:16.000000 ogc_na-0.3.2/ogc_na.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 12:32:16.000000 ogc_na-0.3.2/ogc_na.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:32:16.000000 ogc_na-0.3.2/ogc_na.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-13 12:32:16.000000 ogc_na-0.3.2/ogc_na.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-13 12:32:16.000000 ogc_na-0.3.2/ogc_na.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-13 12:32:02.000000 ogc_na-0.3.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:32:16.579192 ogc_na-0.3.2/rdf/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 12:32:02.000000 ogc_na-0.3.2/rdf/catalog-v001.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-13 12:32:02.000000 ogc_na-0.3.2/rdf/domaincfg.vocab.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-13 12:32:02.000000 ogc_na-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 12:32:16.579192 ogc_na-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-13 12:32:02.000000 ogc_na-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:32:16.579192 ogc_na-0.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:32:02.000000 ogc_na-0.3.2/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:32:16.579192 ogc_na-0.3.2/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:32:02.000000 ogc_na-0.3.2/test/data/empty.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-13 12:32:02.000000 ogc_na-0.3.2/test/data/headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-13 12:32:02.000000 ogc_na-0.3.2/test/data/no-headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-13 12:32:02.000000 ogc_na-0.3.2/test/data/profile_tree.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-13 12:32:02.000000 ogc_na-0.3.2/test/data/profile_tree_cyclic.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-13 12:32:02.000000 ogc_na-0.3.2/test/data/sample-context.jsonld
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-13 12:32:02.000000 ogc_na-0.3.2/test/data/sample-schema-prop-c.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-13 12:32:02.000000 ogc_na-0.3.2/test/data/sample-schema.yml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-13 12:32:02.000000 ogc_na-0.3.2/test/data/uplift_context_valid.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-13 12:32:02.000000 ogc_na-0.3.2/test/test_annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-13 12:32:02.000000 ogc_na-0.3.2/test/test_ingest_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-13 12:32:02.000000 ogc_na-0.3.2/test/test_input_filters_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-13 12:32:02.000000 ogc_na-0.3.2/test/test_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:31:54.598916 ogc_na-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:31:54.590916 ogc_na-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:31:54.590916 ogc_na-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-14 06:31:44.000000 ogc_na-0.3.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-07-14 06:31:44.000000 ogc_na-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-14 06:31:44.000000 ogc_na-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-14 06:31:54.594916 ogc_na-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-14 06:31:44.000000 ogc_na-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:31:54.590916 ogc_na-0.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-07-14 06:31:44.000000 ogc_na-0.3.3/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-14 06:31:44.000000 ogc_na-0.3.3/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-14 06:31:44.000000 ogc_na-0.3.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-14 06:31:44.000000 ogc_na-0.3.3/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-14 06:31:44.000000 ogc_na-0.3.3/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:31:54.590916 ogc_na-0.3.3/ogc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:31:54.594916 ogc_na-0.3.3/ogc/na/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-14 06:31:44.000000 ogc_na-0.3.3/ogc/na/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 06:31:54.000000 ogc_na-0.3.3/ogc/na/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33988 2023-07-14 06:31:44.000000 ogc_na-0.3.3/ogc/na/annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-07-14 06:31:44.000000 ogc_na-0.3.3/ogc/na/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-14 06:31:44.000000 ogc_na-0.3.3/ogc/na/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-14 06:31:44.000000 ogc_na-0.3.3/ogc/na/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35338 2023-07-14 06:31:44.000000 ogc_na-0.3.3/ogc/na/ingest_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:31:54.594916 ogc_na-0.3.3/ogc/na/input_filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-14 06:31:44.000000 ogc_na-0.3.3/ogc/na/input_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-14 06:31:44.000000 ogc_na-0.3.3/ogc/na/input_filters/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16477 2023-07-14 06:31:44.000000 ogc_na-0.3.3/ogc/na/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-14 06:31:44.000000 ogc_na-0.3.3/ogc/na/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18229 2023-07-14 06:31:44.000000 ogc_na-0.3.3/ogc/na/update_vocabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-07-14 06:31:44.000000 ogc_na-0.3.3/ogc/na/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-14 06:31:44.000000 ogc_na-0.3.3/ogc/na/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:31:54.594916 ogc_na-0.3.3/ogc_na.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-14 06:31:54.000000 ogc_na-0.3.3/ogc_na.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-14 06:31:54.000000 ogc_na-0.3.3/ogc_na.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 06:31:54.000000 ogc_na-0.3.3/ogc_na.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-14 06:31:54.000000 ogc_na-0.3.3/ogc_na.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-14 06:31:54.000000 ogc_na-0.3.3/ogc_na.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-14 06:31:44.000000 ogc_na-0.3.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:31:54.594916 ogc_na-0.3.3/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-14 06:31:44.000000 ogc_na-0.3.3/rdf/catalog-v001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-14 06:31:44.000000 ogc_na-0.3.3/rdf/domaincfg.vocab.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-14 06:31:44.000000 ogc_na-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 06:31:54.598916 ogc_na-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-14 06:31:44.000000 ogc_na-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:31:54.594916 ogc_na-0.3.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:31:44.000000 ogc_na-0.3.3/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:31:54.594916 ogc_na-0.3.3/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 06:31:44.000000 ogc_na-0.3.3/test/data/empty.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-14 06:31:44.000000 ogc_na-0.3.3/test/data/headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-14 06:31:44.000000 ogc_na-0.3.3/test/data/no-headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-14 06:31:44.000000 ogc_na-0.3.3/test/data/profile_tree.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-14 06:31:44.000000 ogc_na-0.3.3/test/data/profile_tree_cyclic.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-14 06:31:44.000000 ogc_na-0.3.3/test/data/sample-context.jsonld
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-14 06:31:44.000000 ogc_na-0.3.3/test/data/sample-schema-prop-c.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-14 06:31:44.000000 ogc_na-0.3.3/test/data/sample-schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-14 06:31:44.000000 ogc_na-0.3.3/test/data/schema-vocab.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-14 06:31:44.000000 ogc_na-0.3.3/test/data/uplift_context_valid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-14 06:31:44.000000 ogc_na-0.3.3/test/test_annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-14 06:31:44.000000 ogc_na-0.3.3/test/test_ingest_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-14 06:31:44.000000 ogc_na-0.3.3/test/test_input_filters_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-14 06:31:44.000000 ogc_na-0.3.3/test/test_profile.py
```

### Comparing `ogc_na-0.3.2/.github/workflows/python-publish.yml` & `ogc_na-0.3.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/.gitignore` & `ogc_na-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/PKG-INFO` & `ogc_na-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc_na
-Version: 0.3.2
+Version: 0.3.3
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.io/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.3.2/README.md` & `ogc_na-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/docs/examples.md` & `ogc_na-0.3.3/docs/examples.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/docs/gen_ref_pages.py` & `ogc_na-0.3.3/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/docs/index.md` & `ogc_na-0.3.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/docs/tutorials.md` & `ogc_na-0.3.3/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/mkdocs.yml` & `ogc_na-0.3.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/ogc/na/annotate_schema.py` & `ogc_na-0.3.3/ogc/na/annotate_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,15 +325,15 @@
 
 def resolve_context(ctx: Path | str | dict | list, expand_uris=True) -> ResolvedContext:
     if not ctx:
         return ResolvedContext()
 
     prefixes = {}
     def expand_uri(curie, ctx_stack):
-        if not expand_uris or not ctx_stack or not curie:
+        if not expand_uris or not ctx_stack or not curie or curie[0] == '@':
             return curie
         if ':' in curie:
             prefix, localpart = curie.split(':', 1)
         else:
             prefix, localpart = None, None
         for c in reversed(ctx_stack):
             if localpart:
@@ -465,26 +465,26 @@
 
         def find_prop_context(prop, context_stack) -> dict | None:
             for ctx in reversed(context_stack):
                 vocab = ctx.get('@vocab')
                 if prop in ctx:
                     prop_ctx = ctx[prop]
                     if isinstance(prop_ctx, str):
-                        if vocab and ':' not in prop_ctx:
+                        if vocab and ':' not in prop_ctx and prop_ctx[0] != '@':
                             prop_ctx = f"{vocab}{prop_ctx}"
                         return {'@id': prop_ctx}
                     elif '@id' not in prop_ctx and not vocab:
                         raise ValueError(f'Missing @id for property {prop} in context {json.dumps(ctx, indent=2)}')
                     else:
                         result = {k: v for k, v in prop_ctx.items() if k.startswith('@')}
                         if vocab:
                             prop_id = result.get('@id')
                             if not prop_id:
                                 result['@id'] = f"{vocab}{prop}"
-                            elif ':' not in prop_id:
+                            elif ':' not in prop_id and prop_id[0] != '@':
                                 result['@id'] = f"{vocab}{prop_id}"
                         return result
                 elif '@vocab' in ctx:
                     return {'@id': f"{ctx['@vocab']}{prop}"}
 
         def process_properties(obj: dict, context_stack: list[dict[str, Any]],
                                from_schema: ReferencedSchema, level) -> Iterable[str]:
@@ -493,14 +493,17 @@
             if not properties:
                 return ()
             if not isinstance(properties, dict):
                 raise ValueError('"properties" must be a dictionary')
 
             used_terms = set()
             for prop in list(properties.keys()):
+                if prop[0] == '@':
+                    # skip JSON-LD keywords
+                    continue
                 prop_value = properties[prop]
                 prop_ctx = find_prop_context(prop, context_stack)
                 if prop_ctx:
                     used_terms.add(prop)
                     prop_schema_ctx = {f"{ANNOTATION_PREFIX}{k[1:]}": v
                                        for k, v in prop_ctx.items()
                                        if k[0] == '@' and k != '@context'}
```

### Comparing `ogc_na-0.3.2/ogc/na/domain_config.py` & `ogc_na-0.3.3/ogc/na/domain_config.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/ogc/na/download.py` & `ogc_na-0.3.3/ogc/na/download.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/ogc/na/gsp.py` & `ogc_na-0.3.3/ogc/na/gsp.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/ogc/na/ingest_json.py` & `ogc_na-0.3.3/ogc/na/ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/ogc/na/input_filters/__init__.py` & `ogc_na-0.3.3/ogc/na/input_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/ogc/na/input_filters/csv.py` & `ogc_na-0.3.3/ogc/na/input_filters/csv.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/ogc/na/profile.py` & `ogc_na-0.3.3/ogc/na/profile.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/ogc/na/provenance.py` & `ogc_na-0.3.3/ogc/na/provenance.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/ogc/na/update_vocabs.py` & `ogc_na-0.3.3/ogc/na/update_vocabs.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/ogc/na/util.py` & `ogc_na-0.3.3/ogc/na/util.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/ogc/na/validation.py` & `ogc_na-0.3.3/ogc/na/validation.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/ogc_na.egg-info/PKG-INFO` & `ogc_na-0.3.3/ogc_na.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc-na
-Version: 0.3.2
+Version: 0.3.3
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.io/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.3.2/ogc_na.egg-info/SOURCES.txt` & `ogc_na-0.3.3/ogc_na.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -40,8 +40,9 @@
 test/data/headers.csv
 test/data/no-headers.csv
 test/data/profile_tree.ttl
 test/data/profile_tree_cyclic.ttl
 test/data/sample-context.jsonld
 test/data/sample-schema-prop-c.yml
 test/data/sample-schema.yml
+test/data/schema-vocab.yml
 test/data/uplift_context_valid.yml
```

### Comparing `ogc_na-0.3.2/pyproject.toml` & `ogc_na-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/rdf/domaincfg.vocab.ttl` & `ogc_na-0.3.3/rdf/domaincfg.vocab.ttl`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/test/data/headers.csv` & `ogc_na-0.3.3/test/data/headers.csv`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/test/data/uplift_context_valid.yml` & `ogc_na-0.3.3/test/data/uplift_context_valid.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/test/test_annotate_schema.py` & `ogc_na-0.3.3/test/test_annotate_schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -71,7 +71,24 @@
                                             'propA': 'another:a',
                                             'propC': 'another:c'
                                         }
                                     }).schema
 
         self.assertEqual(deep_get(schema, 'properties', 'propA', 'x-jsonld-id'), 'http://example.com/props/a')
         self.assertEqual(deep_get(schema, 'properties', 'propC', 'x-jsonld-id'), 'http://example.net/another/c')
+
+    def test_vocab(self):
+        annotator = SchemaAnnotator()
+        vocab = 'http://example.com/vocab#'
+        schema = annotator.process_schema(DATA_DIR / 'schema-vocab.yml', default_context={
+            '@context': {
+                '@vocab': vocab,
+                'propA': 'test',
+                'propB': '@id',
+                'propC': 'http://www.another.com/',
+            }
+        }).schema
+
+        self.assertEqual(deep_get(schema, 'properties', 'propA', 'x-jsonld-id'), vocab + 'test')
+        self.assertEqual(deep_get(schema, 'properties', 'propB', 'x-jsonld-id'), '@id')
+        self.assertEqual(deep_get(schema, 'properties', 'propC', 'x-jsonld-id'), 'http://www.another.com/')
+        self.assertEqual(deep_get(schema, 'properties', 'propD', 'x-jsonld-id'), vocab + 'propD')
```

### Comparing `ogc_na-0.3.2/test/test_ingest_json.py` & `ogc_na-0.3.3/test/test_ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/test/test_input_filters_csv.py` & `ogc_na-0.3.3/test/test_input_filters_csv.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.3.2/test/test_profile.py` & `ogc_na-0.3.3/test/test_profile.py`

 * *Files identical despite different names*

