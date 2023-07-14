# Comparing `tmp/skoufas_dbf_reader-0.0.4rc166.post1.tar.gz` & `tmp/skoufas_dbf_reader-0.0.4rc170.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skoufas_dbf_reader-0.0.4rc166.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "skoufas_dbf_reader-0.0.4rc170.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `skoufas_dbf_reader-0.0.4rc166.post1.tar` & `skoufas_dbf_reader-0.0.4rc170.post1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      358 2023-07-07 13:17:29.823163 skoufas_dbf_reader-0.0.4rc166.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     2310 2023-07-07 13:17:29.823163 skoufas_dbf_reader-0.0.4rc166.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0       93 2023-07-07 13:17:29.827163 skoufas_dbf_reader-0.0.4rc166.post1/.flake8
--rw-r--r--   0        0        0      239 2023-07-07 13:17:29.827163 skoufas_dbf_reader-0.0.4rc166.post1/.github/dependabot.yml
--rw-r--r--   0        0        0     1552 2023-07-07 13:17:29.827163 skoufas_dbf_reader-0.0.4rc166.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0     1521 2023-07-07 13:17:29.827163 skoufas_dbf_reader-0.0.4rc166.post1/.github/workflows/jekyll-gh-pages.yml
--rw-r--r--   0        0        0      263 2023-07-07 13:17:29.827163 skoufas_dbf_reader-0.0.4rc166.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1824 2023-07-07 13:17:29.827163 skoufas_dbf_reader-0.0.4rc166.post1/.gitignore
--rw-r--r--   0        0        0     1540 2023-07-07 13:17:29.827163 skoufas_dbf_reader-0.0.4rc166.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2023-07-07 13:17:29.827163 skoufas_dbf_reader-0.0.4rc166.post1/.pypirc
--rw-r--r--   0        0        0      129 2023-07-07 13:17:29.827163 skoufas_dbf_reader-0.0.4rc166.post1/.vscode/extensions.json
--rw-r--r--   0        0        0      127 2023-07-07 13:17:29.827163 skoufas_dbf_reader-0.0.4rc166.post1/.vscode/settings.json
--rw-r--r--   0        0        0    34523 2023-07-07 13:17:29.827163 skoufas_dbf_reader-0.0.4rc166.post1/LICENSE
--rw-r--r--   0        0        0     6267 2023-07-07 13:17:29.827163 skoufas_dbf_reader-0.0.4rc166.post1/README.md
--rw-r--r--   0        0        0     5746 2023-07-07 13:17:29.827163 skoufas_dbf_reader-0.0.4rc166.post1/pyproject.toml
--rw-r--r--   0        0        0       95 2023-07-07 13:17:34.679106 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/__init__.py
--rw-r--r--   0        0        0     4563 2023-07-07 13:17:29.827163 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/correction_data.py
--rw-r--r--   0        0        0   678429 2023-07-07 13:17:29.831163 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/author_corrections.yml
--rw-r--r--   0        0        0 18257158 2023-07-07 13:17:29.895162 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/converted_entries.yml
--rw-r--r--   0        0        0   261526 2023-07-07 13:17:29.895162 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/editor_corrections.yml
--rw-r--r--   0        0        0  6078529 2023-07-07 13:17:29.923161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/entries.yml
--rw-r--r--   0        0        0     2236 2023-07-07 13:17:29.923161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field04_corrections.yml
--rw-r--r--   0        0        0     1492 2023-07-07 13:17:29.923161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field05_corrections.yml
--rw-r--r--   0        0        0     1662 2023-07-07 13:17:29.923161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field06_corrections.yml
--rw-r--r--   0        0        0     2149 2023-07-07 13:17:29.923161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field07_corrections.yml
--rw-r--r--   0        0        0   133171 2023-07-07 13:17:29.923161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field08_corrections.yml
--rw-r--r--   0        0        0    12404 2023-07-07 13:17:29.923161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field09_corrections.yml
--rw-r--r--   0        0        0      493 2023-07-07 13:17:29.923161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field10_corrections.yml
--rw-r--r--   0        0        0      440 2023-07-07 13:17:29.923161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field11_corrections.yml
--rw-r--r--   0        0        0     1816 2023-07-07 13:17:29.923161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field16_corrections.yml
--rw-r--r--   0        0        0    45765 2023-07-07 13:17:29.923161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field17_corrections.yml
--rw-r--r--   0        0        0     1081 2023-07-07 13:17:29.923161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field18_corrections.yml
--rw-r--r--   0        0        0    38584 2023-07-07 13:17:29.927161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field19_corrections.yml
--rw-r--r--   0        0        0      247 2023-07-07 13:17:29.927161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field20_corrections.yml
--rw-r--r--   0        0        0    24214 2023-07-07 13:17:29.927161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field30_corrections.yml
--rw-r--r--   0        0        0     6773 2023-07-07 13:17:29.927161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/first_names.yml
--rw-r--r--   0        0        0       50 2023-07-07 13:17:29.927161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/language_codes.yml
--rw-r--r--   0        0        0    65691 2023-07-07 13:17:29.927161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/topic_replacements.yml
--rw-r--r--   0        0        0   109074 2023-07-07 13:17:29.927161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/translator_corrections.yml
--rw-r--r--   0        0        0     1192 2023-07-07 13:17:29.927161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/dbf_to_yaml.py
--rw-r--r--   0        0        0    22109 2023-07-07 13:17:29.927161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/field_extractors.py
--rw-r--r--   0        0        0    28054 2023-07-07 13:17:29.927161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/generate_reports.py
--rw-r--r--   0        0        0     6286 2023-07-07 13:17:29.927161 skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/utilities.py
--rw-r--r--   0        0        0    18910 2023-07-07 13:17:29.927161 skoufas_dbf_reader-0.0.4rc166.post1/tests/test_field_extractors.py
--rw-r--r--   0        0        0    19317 2023-07-07 13:17:29.927161 skoufas_dbf_reader-0.0.4rc166.post1/tests/test_reports.py
--rw-r--r--   0        0        0     1173 2023-07-07 13:17:29.927161 skoufas_dbf_reader-0.0.4rc166.post1/tests/test_utilities.py
--rw-r--r--   0        0        0     7971 1970-01-01 00:00:00.000000 skoufas_dbf_reader-0.0.4rc166.post1/PKG-INFO
+-rw-r--r--   0        0        0      358 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     2310 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0       93 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.flake8
+-rw-r--r--   0        0        0      239 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1552 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0     1521 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.github/workflows/jekyll-gh-pages.yml
+-rw-r--r--   0        0        0      263 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1824 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.pypirc
+-rw-r--r--   0        0        0      129 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.vscode/extensions.json
+-rw-r--r--   0        0        0      127 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/.vscode/settings.json
+-rw-r--r--   0        0        0    34523 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/LICENSE
+-rw-r--r--   0        0        0     6267 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/README.md
+-rw-r--r--   0        0        0     5746 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/pyproject.toml
+-rw-r--r--   0        0        0       95 2023-07-14 13:25:52.629534 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/__init__.py
+-rw-r--r--   0        0        0     4563 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/correction_data.py
+-rw-r--r--   0        0        0    80900 2023-07-14 13:25:49.357322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/author_corrections.yml
+-rw-r--r--   0        0        0 18255023 2023-07-14 13:25:49.417322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/converted_entries.yml
+-rw-r--r--   0        0        0   261526 2023-07-14 13:25:49.421322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/editor_corrections.yml
+-rw-r--r--   0        0        0  6074952 2023-07-14 13:25:49.445322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/entries.yml
+-rw-r--r--   0        0        0     2236 2023-07-14 13:25:49.445322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field04_corrections.yml
+-rw-r--r--   0        0        0     1492 2023-07-14 13:25:49.445322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field05_corrections.yml
+-rw-r--r--   0        0        0     1662 2023-07-14 13:25:49.445322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field06_corrections.yml
+-rw-r--r--   0        0        0     2149 2023-07-14 13:25:49.445322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field07_corrections.yml
+-rw-r--r--   0        0        0   133171 2023-07-14 13:25:49.445322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field08_corrections.yml
+-rw-r--r--   0        0        0    12404 2023-07-14 13:25:49.445322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field09_corrections.yml
+-rw-r--r--   0        0        0      493 2023-07-14 13:25:49.445322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field10_corrections.yml
+-rw-r--r--   0        0        0      440 2023-07-14 13:25:49.445322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field11_corrections.yml
+-rw-r--r--   0        0        0     1816 2023-07-14 13:25:49.445322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field16_corrections.yml
+-rw-r--r--   0        0        0    45765 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field17_corrections.yml
+-rw-r--r--   0        0        0     1081 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field18_corrections.yml
+-rw-r--r--   0        0        0    38584 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field19_corrections.yml
+-rw-r--r--   0        0        0      247 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field20_corrections.yml
+-rw-r--r--   0        0        0    24214 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field30_corrections.yml
+-rw-r--r--   0        0        0     6773 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/first_names.yml
+-rw-r--r--   0        0        0       50 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/language_codes.yml
+-rw-r--r--   0        0        0    65691 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/topic_replacements.yml
+-rw-r--r--   0        0        0   109074 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/translator_corrections.yml
+-rw-r--r--   0        0        0     1192 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/dbf_to_yaml.py
+-rw-r--r--   0        0        0    22109 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/field_extractors.py
+-rw-r--r--   0        0        0    28054 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/generate_reports.py
+-rw-r--r--   0        0        0     6286 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/utilities.py
+-rw-r--r--   0        0        0    18910 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/tests/test_field_extractors.py
+-rw-r--r--   0        0        0    20756 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/tests/test_reports.py
+-rw-r--r--   0        0        0     1173 2023-07-14 13:25:49.449322 skoufas_dbf_reader-0.0.4rc170.post1/tests/test_utilities.py
+-rw-r--r--   0        0        0     7971 1970-01-01 00:00:00.000000 skoufas_dbf_reader-0.0.4rc170.post1/PKG-INFO
```

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/.devcontainer/devcontainer.json` & `skoufas_dbf_reader-0.0.4rc170.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/.github/workflows/CI.yml` & `skoufas_dbf_reader-0.0.4rc170.post1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/.github/workflows/jekyll-gh-pages.yml` & `skoufas_dbf_reader-0.0.4rc170.post1/.github/workflows/jekyll-gh-pages.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/.gitignore` & `skoufas_dbf_reader-0.0.4rc170.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/.pre-commit-config.yaml` & `skoufas_dbf_reader-0.0.4rc170.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/LICENSE` & `skoufas_dbf_reader-0.0.4rc170.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/README.md` & `skoufas_dbf_reader-0.0.4rc170.post1/README.md`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/pyproject.toml` & `skoufas_dbf_reader-0.0.4rc170.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/correction_data.py` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/correction_data.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/converted_entries.yml` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/converted_entries.yml`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4
   authors:
-  - ΑΘΑΝΑΣ,Γ
+  - ΑΘΑΝΑΣΙΑΔΗΣ-ΝΟΒΑΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΤΡΑΓΟΥΔΙΑ ΤΩΝ ΒΟΥΝΩΝ
   dewey: 782.42 ΑΘΑ
   entry_numbers:
   - '711'
   editor: ΣΙΔΕΡΗΣ // ΑΘΗΝΑ
   edition_year: 1980
@@ -201,15 +201,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5
   authors:
-  - ΑΘΑΝΑΣΙΑΔΗ,ΝΟΒΑ-ΘΕΜ
+  - ΑΘΑΝΑΣΙΑΔΗΣ-ΝΟΒΑΣ,ΘΕΜΙΣΤΟΚΛΗΣ
   language: el
   title: ΑΘΗΝΑΙΚΗ ΔΡΑΜΑΤΟΥΡΓΙΑ
   subtitle: ΚΡΙΤΙΚΗ ΤΟΥ ΘΕΑΤΡΟΥ
   dewey: 880.09 ΑΘΑ
   entry_numbers:
   - '1446'
   editor: None // ΑΘΗΝΑ
@@ -253,15 +253,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6
   authors:
-  - ΑΘΑΝΑΣΙΑΔΗ-ΝΟΒΑ,ΘΕΜ
+  - ΑΘΑΝΑΣΙΑΔΗΣ-ΝΟΒΑΣ,ΘΕΜΙΣΤΟΚΛΗΣ
   language: el
   title: ΑΛΕΞΑΝΔΡΟΣ ΠΑΠΑΔΙΑΜΑΝΤΗΣ
   subtitle: ΤΟ ΠΑΣΧΑ ΤΗΣ ΛΟΓΟΤΕΧΝΙΑΣ ΜΑΣ
   dewey: 889.35 ΑΘΑ
   entry_numbers:
   - '1124'
   editor: None // ΑΘΗΝΑ
@@ -303,15 +303,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7
   authors:
-  - ΑΘΑΝΑΣΙΑΔΗ-ΝΟΒΑ,ΘΕΜ
+  - ΑΘΑΝΑΣΙΑΔΗΣ-ΝΟΒΑΣ,ΘΕΜΙΣΤΟΚΛΗΣ
   language: el
   title: ΠΕΡΙΠΛΑΝΗΣΕΙΣ
   dewey: 915 ΑΘΑ
   entry_numbers:
   - '2334'
   editor: None // ΑΘΗΝΑ
   edition_year: 1964
@@ -407,15 +407,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9
   authors:
-  - ΑΙΖΕΝΣΤΑΙΝ,ΣΕΡΓΚΕΙ
+  - Eisenstein,Sergei
   language: el
   title: ΣΚΕΨΕΙΣ ΜΟΥ ΓΙΑ ΤΟΝ ΚΙΝΗΜΑΤΟΓΡΑΦΟ
   dewey: 800.203 ΑΙΖ
   entry_numbers:
   - '1599'
   translators:
   - ΜΟΣΧΟΒΑΚΗΣ,ΑΝΤΩΝΗΣ Θ.
@@ -459,15 +459,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10
   authors:
-  - ΑΙΜΙΛΙΟΥ,ΑΧΙΛΕΩΣ
+  - ΑΙΜΙΛΙΟΥ,ΑΧΙΛΕΑΣ
   language: el
   title: ΠΑΛΙΑ ΚΥΠΡΟΣ
   dewey: 938.497 ΑΙΜ
   entry_numbers:
   - '2231'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   pages: 177
@@ -508,15 +508,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11
   authors:
-  - ΑΙΝΙΑΝ,ΔΗΜΗΤΡ
+  - ΑΙΝΙΑΝ,ΔΗΜΗΤΡΙΟΣ
   language: el
   title: Ο ΚΑΡΑΙΣΚΑΚΗΣ
   dewey: 938.566 ΑΙΝ
   entry_numbers:
   - '1704'
   editor: ΕΡΜΗΣ // ΑΘΗΝΑ
   edition_year: 1974
@@ -980,15 +980,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 20
   authors:
-  - ΑΜΑΝΤΟΣ,Ι.ΚΩΣΤΑΝΤΙΝΟΣ
+  - ΑΜΑΝΤΟΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ,Ι.
   language: el
   title: ΙΣΤΟΡΙΑ ΤΟΥ ΒΥΖΑΝΤΙΝΟΥ ΚΡΑΤΟΥΣ
   dewey: 938.3 ΑΜΑ
   entry_numbers:
   - '1765'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 1939
@@ -1033,15 +1033,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 21
   authors:
-  - ΑΜΑΝΤΟΣ,Ι.ΚΩΝΣΤΑΝΤΙΝΟΣ
+  - ΑΜΑΝΤΟΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ,Ι.
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΕΛΛΑΔΟΣ
   subtitle: ΑΠΟ ΤΩΝ ΑΡΧΑΙΟΤΑΤΩΝ ΧΡΟΝΩΝ ΜΕΧΡΙ ΤΟΥ 1071Μ.Χ
   dewey: 938 ΑΜΑ
   entry_numbers:
   - '1916'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
@@ -1085,15 +1085,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 22
   authors:
-  - ΑΜΑΝΤΟΣ,Ι.ΚΩΝΣΤΑΝΤΙΝΟΣ
+  - ΑΜΑΝΤΟΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ,Ι.
   language: el
   title: ΙΣΤΟΡΙΚΑΙ ΣΧΕΣΕΙΣ ΕΛΛΗΝΩΝ ΣΕΡΒΩΝ ΚΑΙ ΒΟΥΛΓΑΡΩΝ
   dewey: 938.692 ΑΜΑ
   entry_numbers:
   - '2088'
   editor: None // ΑΘΗΝΑ
   edition_year: 1949
@@ -1140,15 +1140,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 23
   authors:
-  - ΑΜΠΕΛΑΣ,ΔΗΜΗΤΡΙΟΣ ΤΙΜΟΛ
+  - ΑΜΠΕΛΑΣ,ΔΗΜΗΤΡΙΟΣ,ΤΙΜΟΛ.
   language: el
   title: Η ΚΑΘΟΔΟΣ ΤΩΝ ΝΕΟΤΕΡΩΝ ΜΥΡΙΩΝ
   dewey: 938.163 ΑΜΠ
   entry_numbers:
   - '1953'
   edition: '2'
   editor: None // ΑΘΗΝΑ
@@ -1398,15 +1398,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 28
   authors:
-  - ΑΝΑΣΤΑΣΟΠΟΥΛΟΣ,Γ.Α
+  - ΑΝΑΣΤΑΣΟΠΟΥΛΟΣ,ΓΕΩΡΓΙΟΣ,Α.
   language: el
   title: ΝΕΑ ΥΟΡΚΗ
   subtitle: Η ΘΛΙΒΕΡΗ ΠΟΛΙΣ
   dewey: 970 ΑΝΑ
   entry_numbers:
   - '431'
   editor: None // ΑΘΗΝΑ
@@ -1500,15 +1500,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 30
   authors:
-  - ΑΝΕΣΤΟΠΟΥΛΟΣ,ΑΓΓΕΛΛΟΣ Κ
+  - ΑΝΕΣΤΟΠΟΥΛΟΣ,ΑΓΓΕΛΛΟΣ,Κ.
   language: el
   title: Η ΙΣΤΟΡΙΑ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΕΠΟΥΣ
   subtitle: ΕΙΣ ΤΗΝ ΑΙΜΑΤΟΒΑΜΜΕΝΗΝ ΓΗΝ ΤΗΣ Β.ΗΠΕΙΡΟΥ:28 ΟΚΤΩΜΒΡΙΟΥ 1940
   dewey: 938.751 ΑΝΕ
   entry_numbers:
   - '1945'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -1553,15 +1553,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 31
   authors:
-  - ΑΝΤΟΝΙΟΝΙ,ΜΙΚΕΛΑΝΤΖΕΛΟ
+  - ANTONIONI,MICHELANGELO
   language: el
   title: ΜΙΚΕΛΑΝΤΖΕΛΟ ΑΝΤΟΝΙΟΝΙ
   dewey: 800.203 ΑΝΤ
   entry_numbers:
   - '1620'
   editor: ΑΙΓΟΚΕΡΩΣ // ΑΘΗΝΑ
   edition_year: 1984
@@ -1606,15 +1606,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 32
   authors:
-  - ΑΝΤΩΝΟΠΟΥΛΟΣ,ΚΟΣΜΑΣ ΕΜΜ
+  - ΑΝΤΩΝΟΠΟΥΛΟΣ,ΚΟΣΜΑΣ
   language: el
   title: ΕΛΛΗΝΙΣΜΟΣ ΚΑΙ ΔΗΜΟΚΡΑΤΙΑ
   dewey: 938 ΑΝΤ
   entry_numbers:
   - '2533'
   editor: None // ΑΘΗΝΑ
   edition_year: 1971
@@ -1657,15 +1657,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 33
   authors:
-  - ΑΝΤΩΝΟΠΟΥΛΟΣ,ΚΟΣΜΑΣ ΕΜΜ
+  - ΑΝΤΩΝΟΠΟΥΛΟΣ,ΚΟΣΜΑΣ
   language: el
   title: Η ΕΠΑΡΧΙΑ
   subtitle: ΕΛΛΑΔΑ ΔΕΝ ΕΙΝΑΙ ΜΟΝΑΧΑ Η ΑΘΗΝΑ
   dewey: 938 ΑΝΤ
   entry_numbers:
   - '2522'
   edition: '2'
@@ -1814,15 +1814,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 36
   authors:
-  - ΑΞΙΩΤΗΣ,ΠΕΤΡΟΣ Ι
+  - ΑΞΙΩΤΗΣ,ΠΕΤΡΟΣ,Ι.
   language: el
   title: Η ΑΝΔΡΙΑΝΟΥΠΟΛΙΣ
   dewey: 938.21 ΑΞΙ
   entry_numbers:
   - '2489'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1949
@@ -1863,15 +1863,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 37
   authors:
-  - ΑΟΥΤΖΙΕΡ,ΑΙΜΙΛΙΟΣ
+  - AUGIER,EMILE
   language: el
   title: ΟΙ ΧΑΛΚΟΠΡΟΣΩΠΟΙ
   subtitle: ΚΩΜΩΔΙΑ
   dewey: 842 ΑUG
   entry_numbers:
   - '1391'
   translators:
@@ -1924,16 +1924,15 @@
   authors:
   - ΑΠΕΡΓΗΣ,ΠΑΝΤΕΛΗΣ
   language: el
   title: ΤΡΙΑ ΠΡΟΣΩΠΑ
   subtitle: ΕΙΣΑΓΩΓΗ ΣΤΗΝ ΕΠΟΧΗ ΚΑΙ ΤΟ ΕΡΓΟ ΤΟΥΣ
   dewey: 880.3 ΑΠΕ
   entry_numbers:
-  - '1004'
-  - '2688'
+  - '9274'
   editor: ΙΩΛΚΟΣ // ΑΘΗΝΑ
   edition_year: 1980
   pages: 88
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΣΥΓΓΡΑΦΕΙΣ
   - ΕΜΜΑΝΟΥΗΛ ΡΟΙΔΗΣ
@@ -1944,16 +1943,16 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 38
     1: ΑΠΕΡΓΗΣ,ΠΑΝΤΕΛΗΣ
     2: ΤΡΙΑ ΠΡΟΣΩΠΑ
     3: ΕΙΣΑΓΩΓΗ ΣΤΗΝ ΕΠΟΧΗ ΚΑΙ ΤΟ ΕΡΓΟ ΤΟΥΣ
-    4: 880.3 ΑΠΕ
-    5: 1004-2688
+    4: 880.3ΑΠΕ
+    5: '9274'
     8: ΙΩΛΚΟΣ
     9: ΑΘΗΝΑ
     10: '1980'
     11: 88Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
     13: ΡΟΙΔΗΣ,ΕΜΜΑΝΟΥΗΛ
     14: ΚΑΒΑΦΗΣ,Κ.Π
@@ -1973,15 +1972,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 39
   authors:
-  - ΑΠΟΣΤΟΛΑΚΗΣ,ΓΙΑΝΝΗΣ Μ
+  - ΑΠΟΣΤΟΛΑΚΗΣ,ΓΙΑΝΝΗΣ,Μ.
   language: el
   title: Η ΠΟΙΗΣΗ ΣΤΗ ΖΩΗ ΜΑΣ
   dewey: 889.09 ΑΠΟ
   entry_numbers:
   - '2641'
   edition: '2'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
@@ -2025,15 +2024,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 40
   authors:
-  - ΑΠΟΣΤΟΛΙΔΗΣ,ΗΡ Ν
+  - ΑΠΟΣΤΟΛΙΔΗΣ,ΗΡΑΚΛΗΣ,Ν.
   language: el
   title: ΤΟ ΑΛΛΟ ΣΤΗΝ ΑΝΘΟΛΟΓΙΑ
   dewey: 880.08 ΑΠΟ
   entry_numbers:
   - '2662'
   editor: ΒΛΑΣΣΗ // ΑΘΗΝΑ
   edition_year: 1964
@@ -2076,15 +2075,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 41
   authors:
-  - ΑΠΟΣΤΟΛΟΠΟΥΛΟΣ,ΔΗΜΗΤΡΙΟΣ
+  - ΑΠΟΣΤΟΛΟΠΟΥΛΟΣ,ΔΗΜΗΤΡΗΣ
   language: el
   title: Η ΓΑΛΛΙΚΗ ΕΠΑΝΑΣΤΑΣΗ ΣΤΗΝ ΤΟΥΡΚΟΚΡΑΤΟΥΜΕΝΗ ΕΛΛΗΝΙΚΗ ΚΟΙΝΩΝΙΑ
   dewey: 938.4 ΑΠΟ
   entry_numbers:
   - '2460'
   editor: None // ΑΘΗΝΑ
   edition_year: 1989
@@ -2129,15 +2128,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 42
   authors:
-  - ΑΠΟΣΤΟΛΙΔΗΣ,ΡΕΝΟΣ-ΗΡΑΚΛΗΣ
+  - ΑΠΟΣΤΟΛΙΔΗΣ,ΡΕΝΟΣ,ΗΡΑΚΛΗΣ
   language: el
   title: ΑΝΘΟΛΟΓΙΑ ΤΗΣ ΝΕΟΕΛΛΗΝΙΚΗΣ ΓΡΑΜΜΑΤΕΙΑΣ
   dewey: 880.08 ΑΠΟ
   entry_numbers:
   - '634'
   - '632'
   - '631'
@@ -2187,15 +2186,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 43
   authors:
-  - ΑΠΟΣΤΟΛΙΔΗΣ,ΡΕΝΟΣ-ΗΡΑΚΛΗΣ
+  - ΑΠΟΣΤΟΛΙΔΗΣ,ΡΕΝΟΣ,ΗΡΑΚΛΗΣ
   language: el
   title: ΚΑΤΗΓΟΡΩ
   dewey: 938.774 ΑΠΟ
   entry_numbers:
   - '10663'
   editor: ΒΛΑΣΣΗ // ΑΘΗΝΑ
   edition_year: 1965
@@ -2239,15 +2238,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 44
   authors:
-  - ΑΡΑΒΑΝΤΙΝΟΣ,Π
+  - ΑΡΑΒΑΝΤΙΝΟΣ,ΠΑΝΑΓΙΩΤΗΣ
   language: el
   title: ΣΥΛΛΟΓΗ ΔΗΜΟΔΩΝ ΑΣΜΑΤΩΝ ΤΗΣ ΗΠΕΙΡΟΥ
   dewey: 782.42 ΑΡΑ
   entry_numbers:
   - '755'
   editor: ΠΕΡΡΗ // ΑΘΗΝΑ
   edition_year: 1880
@@ -2293,15 +2292,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 45
   authors:
-  - ΑΡΑΒΑΝΤΙΝΟΣ,Π
+  - ΑΡΑΒΑΝΤΙΝΟΣ,ΠΑΝΑΓΙΩΤΗΣ
   language: el
   title: ΠΑΡΟΙΜΙΑΣΤΗΡΙΟΝ Ή ΣΥΛΛΟΓΗ ΠΑΡΟΙΜΙΩΝ
   dewey: 938.21 ΑΡΑ
   entry_numbers:
   - '2184'
   editor: ΔΩΔΩΝΗ // ΙΩΑΝΝΙΝΑ
   edition_year: 1863
@@ -2345,15 +2344,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 46
   authors:
-  - ΑΡΑΒΑΝΤΙΝΟΣ,Π
+  - ΑΡΑΒΑΝΤΙΝΟΣ,ΠΑΝΑΓΙΩΤΗΣ
   language: el
   title: ΧΡΟΝΟΓΡΑΦΙΑ ΤΗΣ ΗΠΕΙΡΟΥ
   dewey: 938.21 ΑΡΑ
   entry_numbers:
   - '2180'
   - '2183'
   - '2182'
@@ -2397,15 +2396,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 47
   authors:
-  - ΑΡΑΒΑΝΤΙΝΟΣ,Π
+  - ΑΡΑΒΑΝΤΙΝΟΣ,ΠΑΝΑΓΙΩΤΗΣ
   language: el
   title: ΒΙΟΓΡΑΦΙΚΗ ΣΥΛΛΟΓΗ ΛΟΓΙΩΝ ΤΗΣ ΤΟΥΡΚΟΚΡΑΤΙΑΣ
   dewey: 938.509 ΑΡΑ
   entry_numbers:
   - '1971'
   - '1972'
   editor: ΗΠΕΙΡΩΤΙΚΩΝ ΜΕΛΕΤΩΝ // ΙΩΑΝΝΙΝΑ
@@ -2451,15 +2450,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 48
   authors:
-  - ΑΡΓΥΡΟΣ,ΣΠΥΡΙΔΩΝΟΣ
+  - ΑΡΓΥΡΟΣ,ΣΠΥΡΙΔΩΝ
   language: el
   title: Η ΠΕΙΡΑΤΕΙΑ ΑΠΟ ΤΟ 1500 Π.Χ ΕΩΣ ΤΟ 1860
   dewey: 938 ΑΡΓ
   entry_numbers:
   - '2319'
   editor: None // ΑΘΗΝΑ
   edition_year: 1956
@@ -2782,15 +2781,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 54
   authors:
-  - ΑΡΜΑΚΟΛΛΑΣ,ΜΑΡΚΟΣ Π.Μ
+  - ΑΡΜΑΚΟΛΛΑΣ,ΜΑΡΚΟΣ,Π.Μ.
   language: el
   title: Η ΤΥΦΛΗ ΤΡΑΓΟΥΔΙΣΤΡΙΑ
   subtitle: ΔΡΑΜΑ
   dewey: 886.2 ΑΡΜ
   entry_numbers:
   - '1527'
   editor: None // ΑΘΗΝΑ
@@ -2888,15 +2887,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 56
   authors:
-  - ΑΣΙΜΩΦ,ΙΣΑΑΚ
+  - ASIMOV,ISAAC
   language: el
   title: ΠΩΣ ΒΡΗΚΑΜΕ ΟΤΙ Η ΓΗ ΕΙΝΑΙ ΣΤΡΟΓΓΥΛΗ
   dewey: 808.99 ΑΣΙ
   entry_numbers:
   - '1260'
   editor: None // ΑΘΗΝΑ
   edition_year: 1981
@@ -2993,15 +2992,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 58
   authors:
-  - ΑΣΩΠΙΟΣ,ΕΙΡΗΝΑΙΟΣ Κ
+  - ΑΣΩΠΙΟΣ,ΕΙΡΗΝΑΙΟΣ,Κ.
   language: el
   title: ΠΑΛΑΙΑ ΚΑΙ ΝΕΑ
   dewey: 938 ΑΣΩ
   entry_numbers:
   - '2102'
   editor: ΣΑΚΕΛΛΑΡΙΟΥ // ΑΘΗΝΑ
   edition_year: 1903
@@ -3047,15 +3046,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 59
   authors:
-  - ΑΝΤΖΕΛ,ΧΕΡΝΙ
+  - AGEL,HENRI
   language: el
   title: ΑΙΣΘΗΤΙΚΗ ΤΟΥ ΚΙΝΗΜΑΤΟΓΡΑΦΟΥ
   dewey: 800.203 ΑGE
   entry_numbers:
   - '1594'
   translators:
   - ΖΑΡΟΥΚΑΣ,ΚΩΣΤΑΣ
@@ -3100,25 +3099,23 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 60
   authors:
-  - ΒΑΒΑΡΕΤΟΣ,ΓΕΩΡΓΙΟΣ
+  - ΒΑΒΑΡΕΤΟΣ,ΓΕΩΡΓΙΟΣ,ΑΧΙΛ.
   language: el
   title: Η ΣΥΜΒΟΛΗ ΤΗΣ ΗΠΕΙΡΟΥ ΕΙΣ ΤΟΥΣ ΑΓΩΝΑΣ ΥΠΕΡ ΤΗΣ ΕΛΕΥΘΕΡΙΑΣ
   dewey: 938.5 ΒΑΒ
   entry_numbers:
   - '2167'
   - '2168'
   - '2046'
   - '2047'
-  - '2048'
-  - '9258'
   editor: None // ΑΘΗΝΑ
   edition_year: 1963
   pages: 31
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΗΠΕΙΡΟΣ
   - ΣΥΜΒΟΛΗ ΣΤΗΝ ΕΛΕΥΘΕΡΙΑ
@@ -3132,27 +3129,27 @@
   offprint: false
   original_entry:
     0: 60
     1: ΒΑΒΑΡΕΤΟΣ,ΓΕΩΡΓΙΟΣ
     2: Η ΣΥΜΒΟΛΗ ΤΗΣ ΗΠΕΙΡΟΥ ΕΙΣ ΤΟΥΣ ΑΓΩΝΑΣ ΥΠΕΡ ΤΗΣ ΕΛΕΥΘΕΡΙΑΣ
     4: 938.5ΒΑΒ
     5: 2167-2168-2046-2047
-    6: 2048-9258
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1963'
     11: 31Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΣΥΜΒΟΛΗ ΣΤΗΝ ΕΛΕΥΘΕΡΙΑ
     13: ΗΠΕΙΡΟΣ-ΑΓΩΝΕΣ ΕΛΕΥΘΕΡΙΑΣ
     14: ΑΓΩΝΕΣ ΕΛΕΥΘΕΡΙΑΣ
     15: ΕΛΕΥΘΕΡΙΑ-ΑΓΩΝΕΣ
     17: 2 ΑΝΤΙΤΥΠΑ
     22: ΣΥΜΒΟΛΗ
     23: ΑΓΩΝΑΣ
     3: null
+    6: null
     7: null
     16: null
     18: null
     19: null
     20: null
     21: null
     24: null
@@ -3160,15 +3157,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 61
   authors:
-  - ΒΑΒΑΡΕΤΟΣ,ΓΕΩΡΓΙΟΣ ΑΧΙΛ
+  - ΒΑΒΑΡΕΤΟΣ,ΓΕΩΡΓΙΟΣ,ΑΧΙΛ.
   language: el
   title: Ο ΑΛΗ ΠΑΣΑΣ ΑΠΟ ΤΗΝ ΑΛΛΗ ΠΛΕΥΡΑ
   dewey: 938.484 ΒΑΒ
   entry_numbers:
   - '1818'
   - '2735'
   editor: None // ΑΘΗΝΑ
@@ -3215,15 +3212,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 62
   authors:
-  - ΒΑΓΙΑΚΑΚΟΣ,ΔΙΚΑΙΟΣ Β
+  - ΒΑΓΙΑΚΑΚΟΣ,ΔΙΚΑΙΟΣ,Β.
   language: el
   title: ΟΙ ΜΑΝΙΑΤΑΙ ΤΗΣ ΔΙΑΣΠΟΡΑΣ
   subtitle: ΟΙ ΜΑΝΙΑΤΑΙ ΤΗΣ ΚΟΡΣΙΚΗΣ
   dewey: 938.655 ΒΑΓ
   entry_numbers:
   - '1902'
   editor: None // ΑΘΗΝΑ
@@ -3269,15 +3266,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 63
   authors:
-  - ΒΑΙΣ,ΠΕΤΕΡ
+  - WEISS,PETER
   language: el
   title: Ο ΤΡΟΤΣΚΙ ΕΞΟΡΙΣΤΟΣ
   dewey: 891.79 ΒΑΙ
   entry_numbers:
   - '1372'
   translators:
   - ΠΑΠΑΡΑ,ΜΑΡΙ-ΠΩΛ
@@ -3532,15 +3529,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 68
   authors:
-  - ΒΑΛΕΤΑΣ,Γ
+  - ΒΑΛΕΤΑΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΓΙΑΝΝΗΣ ΘΕΟΦΙΛΟΠΟΥΛΟΣ
   subtitle: Ο ΚΑΡΑΒΟΓΙΑΝΝΗΣ
   dewey: 938.5 ΒΑΛ
   entry_numbers:
   - '1964'
   editor: None // ΑΘΗΝΑ
@@ -3584,15 +3581,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 69
   authors:
-  - ΒΑΛΕΤΑΣ,Γ
+  - ΒΑΛΕΤΑΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΠΑΠΑΔΙΑΜΑΝΤΗΣ
   subtitle: Η ΖΩΗ-ΤΟΕΡΓΟ-Η ΕΠΟΧΗ ΤΟΥ
   dewey: 889.35 ΒΑΛ
   entry_numbers:
   - '1118'
   editor: None // ΜΥΤΙΛΗΝΗ
@@ -3635,15 +3632,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 70
   authors:
-  - ΒΑΛΕΤΑΣ,Γ
+  - ΒΑΛΕΤΑΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΤΟ ΠΡΟΔΟΜΕΝΟ ΕΙΚΟΣΙΕΝΑ
   dewey: 938.5 ΒΑΛ
   entry_numbers:
   - '1845'
   edition: '2'
   editor: ΦΙΛΙΠΠΟΤΗ // ΑΘΗΝΑ
@@ -3689,15 +3686,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 71
   authors:
-  - ΒΑΛΖΕΡ,ΜΑΡΤΙΝ
+  - WALSER,MARTIN
   language: el
   title: ΔΡΥΣ ΚΑΙ ΚΟΥΝΕΛΙΑ ΑΓΚΟΡΑ
   dewey: 832 ΒΑΛ
   entry_numbers:
   - '1370'
   translators:
   - ΜΟΥΣΤΡΗΣ,ΓΙΩΡΓΟΣ
@@ -3855,15 +3852,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 74
   authors:
-  - ΒΑΡΒΙΑΝΗΣ,Ν.Α
+  - ΒΑΡΒΙΑΝΗΣ,Ν.,Α.
   language: el
   title: Η ΖΑΚΥΝΘΟΣ
   dewey: 938.967 ΒΑΡ
   entry_numbers:
   - '341'
   editor: None // ΑΘΗΝΑ
   edition_year: 1977
@@ -3904,15 +3901,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 75
   authors:
-  - ΒΑΡΔΑΚΟΥΛΑΣ,Ι Δ
+  - ΒΑΡΔΑΚΟΥΛΑΣ,ΙΩΑΝΝΗΣ Δ.
   language: el
   title: Η ΚΟΙΝΩΝΙΚΗ ΠΡΟΣΤΑΣΙΑ ΚΑΙ ΟΙ ΚΑΤΕΥΘΥΝΣΕΙΣ ΤΗΣ
   subtitle: ΣΤΑ ΧΡΟΝΙΑ ΤΟΥ ΚΑΠΟΔΙΣΤΡΙΑ
   dewey: 938.571 ΒΑΡ
   entry_numbers:
   - '1784'
   editor: None // ΑΘΗΝΑ
@@ -4014,15 +4011,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 77
   authors:
-  - ΒΑΡΙΚΟΣ,ΔΗΜΗΤΡΙΟΣ Π
+  - ΒΑΡΙΚΟΣ,ΔΗΜΗΤΡΙΟΣ,Π.
   language: el
   title: ΝΕΟΕΛΛΗΝΙΚΑ ΜΕΛΕΤΗΜΑΤΑ
   subtitle: ΔΗΜΟΤΙΚΗ ΠΟΙΗΣΗ
   dewey: 782.842 ΒΑΡ
   entry_numbers:
   - '2695'
   editor: None // ΑΘΗΝΑ
@@ -4226,15 +4223,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 81
   authors:
-  - ΒΑΡΤΣΟΣ,ΙΩΑΝΝΗΣ Α
+  - ΒΑΡΤΣΟΣ,ΙΩΑΝΝΗΣ,Α.
   language: el
   title: ΑΘΗΝΑΙΚΑΙ ΚΛΗΡΟΥΧΙΑΙ
   dewey: 938.12 ΒΑΡ
   entry_numbers:
   - '2315'
   editor: None // ΑΘΗΝΑ
   edition_year: 1972
@@ -4278,15 +4275,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 82
   authors:
-  - ΒΑΡΤΣΟΣ,ΙΩΑΝΝΗΣ Α.
+  - ΒΑΡΤΣΟΣ,ΙΩΑΝΝΗΣ,Α.
   language: el
   title: Ο ΠΥΡΡΟΣ ΕΝ ΙΤΑΛΙΑ
   subtitle: ΣΚΟΠΟΙ ΚΑΙ ΔΡΑΣΙΣ ΑΥΤΟΥ
   dewey: 938.184 ΒΑΡ
   entry_numbers:
   - '2205'
   editor: None // ΑΘΗΝΑ
@@ -4332,15 +4329,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 83
   authors:
-  - ΒΑΣΔΡΑΒΕΛΛΗΣ,ΙΩΑΝ
+  - ΒΑΣΔΡΑΒΕΛΛΗΣ,ΙΩΑΝΝΗΣ,Κ.
   language: el
   title: Η ΝΑΟΥΣΑ ΚΑΤΑ ΤΟΝ ΑΓΩΝΑ ΤΗΣ ΑΝΕΞΑΡΤΗΣΙΑΣ
   dewey: 938.535 ΒΑΣ
   entry_numbers:
   - '1887'
   editor: ΠΕΡΓΑΜΗΛΗ // ΑΘΗΝΑ
   edition_year: 1953
@@ -4653,15 +4650,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 89
   authors:
-  - ΒΑΣΙΛΙΕΦ,Α.Α
+  - VASILIEV,ALEXANDER,ALEXANDROVICH
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΒΥΖΑΝΤΙΝΗΣ ΑΥΤΟΚΡΑΤΟΡΙΑΣ
   dewey: 938.3 ΒΑΣ
   entry_numbers:
   - '2213'
   - '2214'
   translators:
@@ -4707,15 +4704,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 90
   authors:
-  - ΒΑΣΙΛΕΙΟΥ,ΒΑΣΟΥ
+  - ΒΑΣΙΛΕΙΟΥ,ΒΑΣΟΣ
   language: el
   title: Η ΔΕΥΤΕΡΗ ΟΚΤΩΒΡΙΑΝΗ ΕΠΑΝΑΣΤΑΣΗ
   dewey: 947 ΒΑΣ
   entry_numbers:
   - '2531'
   pages: 195
   topics:
@@ -4757,15 +4754,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 91
   authors:
-  - ΒΑΣΙΛΕΙΟΥ,Ι
+  - ΒΑΣΙΛΕΙΟΥ,Ι.
   language: el
   title: ΑΝΓΚΟΡ
   subtitle: ΜΙΑ ΞΩΤΙΚΗ ΠΟΛΙΤΕΙΑ
   dewey: 915.39 ΒΑΣ
   entry_numbers:
   - '448'
   edition: '2'
@@ -4812,15 +4809,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 92
   authors:
-  - ΒΑΣΙΛΕΙΟΥ,Ι
+  - ΒΑΣΙΛΕΙΟΥ,Ι.
   language: el
   title: ΣΤΗ ΣΙΚΕΛΙΑ ΑΝΑΖΗΤΩΝΤΑΣ ΤΗ ΜΕΓΑΛΗ ΕΛΛΑΔΑ
   dewey: 914.37 ΒΑΣ
   entry_numbers:
   - '389'
   - '388'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
@@ -4864,15 +4861,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 93
   authors:
-  - ΒΑΣΙΛΕΙΟΥ,Ι
+  - ΒΑΣΙΛΕΙΟΥ,Ι.
   language: el
   title: ΣΤΙΣ ΠΑΓΟΔΕΣ ΤΟΥ ΝΕΠΑΛ
   dewey: 915 ΒΑΣ
   entry_numbers:
   - '453'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   pages: 177
@@ -4914,15 +4911,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 94
   authors:
-  - ΒΑΣΙΛΕΙΟΥ,Ι
+  - ΒΑΣΙΛΕΙΟΥ,Ι.
   language: el
   title: ΚΟΝΤΙΝΑ ΚΑΙ ΜΑΚΡΙΝΑ ΤΑΞΙΔΙΑ
   subtitle: ΕΛΛΑΣ-ΙΣΠΑΝΙΑ-ΒΙΡΜΑΝΙΑ-ΙΝΔΟΝΗΣΙΑ-ΚΙΝΑ
   dewey: 914.95 ΒΑΣ
   entry_numbers:
   - '411'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
@@ -4971,15 +4968,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 95
   authors:
-  - ΒΑΣΙΛΕΙΟΥ,Ι
+  - ΒΑΣΙΛΕΙΟΥ,Ι.
   language: el
   title: ΕΝΑ ΤΑΞΙΔΙ ΣΤΗΝ ΙΝΔΙΑ
   dewey: 915.34 ΒΑΣ
   entry_numbers:
   - '445'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   pages: 153
@@ -5020,15 +5017,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 96
   authors:
-  - ΒΑΣΙΛΕΙΟΥ,Ι
+  - ΒΑΣΙΛΕΙΟΥ,Ι.
   language: el
   title: ΤΑΞΙΔΙΑ ΣΤΗΝ ΑΣΙΑ
   subtitle: ΙΝΔΙΑ-ΙΝΔΟΝΗΣΙΑ-ΚΑΜΠΟΤΖΗ-ΝΕΠΑΛ
   dewey: 915 ΒΑΣ
   entry_numbers:
   - '447'
   editor: ΝΙΚΟΔΗΜΟΣ // ΑΘΗΝΑ
@@ -5074,15 +5071,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 97
   authors:
-  - ΒΑΣΙΛΙΚΟΣ ΒΑΣΙΛΗΣ
+  - ΒΑΣΙΛΙΚΟΣ,ΒΑΣΙΛΗΣ
   language: el
   title: Η ΜΥΘΟΛΟΓΙΑ ΤΗΣ ΑΜΕΡΙΚΗΣ
   dewey: 889.21 ΒΑΣ
   entry_numbers:
   - '2657'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   topics:
@@ -5337,15 +5334,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 102
   authors:
-  - ΒΑΦΟΠΟΥΛΟΣ,Γ.Θ
+  - ΒΑΦΟΠΟΥΛΟΣ,Γ.,Θ.
   language: el
   title: ΣΕΛΙΔΕΣ ΑΥΤΟΒΙΟΓΡΑΦΙΑΣ
   dewey: 938.009 ΒΑΦ
   entry_numbers:
   - '2646'
   editor: None // ΑΘΗΝΑ
   pages: 438
@@ -6008,15 +6005,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 115
   authors:
-  - ΒΕΡΤΟΛΙΝΗΣ,ΦΡΑΓΚΙΣΚΟΥ
+  - ΒΕΡΤΟΛΙΝΗΣ,ΦΡΑΓΚΙΣΚΟΣ
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΙΤΑΛΙΚΗΣ ΠΑΛΙΓΓΕΝΕΣΙΑΣ
   dewey: 945 ΒΕΡ
   entry_numbers:
   - '2309'
   - '2308'
   translators:
@@ -6061,15 +6058,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 116
   authors:
-  - ΒΕΡΤΟΛΙΝΗΣ,ΦΡΑΓΚΙΣΚΟΝ
+  - ΒΕΡΤΟΛΙΝΗΣ,ΦΡΑΓΚΙΣΚΟΣ
   language: el
   title: ΡΩΜΑΙΚΗ ΙΣΤΟΡΙΑ ΑΠΟ ΤΩΝ ΑΡΧΑΙΟΤΑΤΩΝ ΧΡΟΝΩΝ
   subtitle: ΜΕΧΡΙ ΚΑΤΑΛΥΣΕΩΣ ΤΗΣ Δ.ΑΥΤΟΚΡΑΤΟΡΙΑΣ
   dewey: 937 ΒΕΡ
   entry_numbers:
   - '1769'
   translators:
@@ -6117,15 +6114,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 117
   authors:
-  - ΒΙΚΕΛΑΣ,Δ
+  - ΒΙΚΕΛΑΣ,ΔΗΜΗΤΡΙΟΣ
   language: el
   title: ΑΠΟ ΝΙΚΟΠΟΛΕΩΣ ΕΙΣ ΟΛΥΜΠΙΑΝ
   dewey: 938.21 ΒΙΚ
   entry_numbers:
   - '1709'
   editor: ΕΚΑΤΗ // ΑΘΗΝΑ
   edition_year: 1991
@@ -6167,15 +6164,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 118
   authors:
-  - ΒΙΤΙ,ΜΑΡΙΟ
+  - VITTI,MARIO
   language: el
   title: ΦΘΟΡΑ ΚΑΙ ΛΟΓΟΣ
   subtitle: ΕΙΣΑΓΩΓΗ ΣΤΗΝ ΠΟΙΗΣΗ ΤΟΥ ΓΙΩΡΓΟΥ ΣΕΦΕΡΗΣ
   dewey: 889.11 VIT
   entry_numbers:
   - '1083'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
@@ -6221,15 +6218,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 119
   authors:
-  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ
+  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ,
   language: el
   title: Ο ΚΑΜΠΑΝΟΠΥΡΓΟΣ
   dewey: 886.2 ΒΛΑ
   entry_numbers:
   - '1363'
   editor: ΔΩΔΩΝΗ // ΑΘΗΝΑ
   pages: 83
@@ -6273,15 +6270,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 120
   authors:
-  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ ΣΤ.
+  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ,
   language: el
   title: ΔΕΚΑ ΧΡΟΝΙΑ ΚΥΠΡΙΑΚΟΥ
   dewey: 938.497 ΒΛΑ
   entry_numbers:
   - '2232'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 1980
@@ -6472,15 +6469,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 124
   authors:
-  - ΒΟΤΣΦΟΡΝΤ
+  - BOTSFORD,GEORGE,WILLIS
   language: el
   title: ΙΣΤΟΡΙΚΟΣ ΑΤΛΑΣ ΚΑΙ ΕΙΚΟΝΟΓΡΑΦΙΑ
   dewey: 938.1 ΒΟΤ
   entry_numbers:
   - '2500'
   editor: None // ΑΘΗΝΑ
   edition_year: 1979
@@ -6523,15 +6520,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 125
   authors:
-  - ΒΟΤΣΦΟΡΝΤ
+  - BOTSFORD,GEORGE,WILLIS
   language: el
   title: ΑΡΧΑΙΑ ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   dewey: 938.1 ΒΟΤ
   entry_numbers:
   - '1915'
   translators:
   - ΤΣΙΤΣΩΝΗΣ,ΣΩΤΗΡΗΣ
@@ -6576,15 +6573,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 126
   authors:
-  - ΒΟΓΟΥΕΝ,ΤΖΟΝ
+  - BOWEN,JOHN,GRIFFITH
   language: el
   title: ΜΙΚΡΑ ΚΟΥΤΙΑ
   dewey: 822 ΒΟW
   entry_numbers:
   - '1407'
   translators:
   - ΤΟΛΙΚΑ,ΟΛΥΜΠΙΑ
@@ -6629,15 +6626,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 127
   authors:
-  - ΒΟΓΡΑ,Ψ.Μ
+  - BOWRA,C.,M.
   language: el
   title: ΑΡΧΑΙΑ ΕΛΛΗΝΙΚΗ ΛΥΡΙΚΗ ΠΟΙΗΣΗ
   dewey: 881.2 ΒΟW
   entry_numbers:
   - '2613'
   translators:
   - ΚΑΖΑΖΗΣ,Ι.Ν.
@@ -6684,15 +6681,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 128
   authors:
-  - ΒΟΥΒΙΕΡ,ΜΠΕΡΤΡΑΝΤ
+  - ΜΠΟΥΒΙΕ,ΜΠΕΡΤΡΑΝΤ
   language: el
   title: ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ ΑΠΟ ΧΕΙΡΟΓΡΑΦΟ ΤΗΣ ΜΟΝΗΣ ΙΒΗΡΩΝ
   dewey: 782.42 BOU
   entry_numbers:
   - '730'
   editor: None // ΑΘΗΝΑ
   edition_year: 1960
@@ -6789,15 +6786,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 130
   authors:
-  - ΒΟΥΛΤΕΨΗΣ,ΓΙΑΝΝΗΣΣ
+  - ΒΟΥΛΤΕΨΗΣ,ΓΙΑΝΝΗΣ
   language: el
   title: ΣΥΝΑΓΩΝΙΣΤΗΣ ΑΚΕΛΑΣ
   dewey: 938.754 ΒΟΥ
   entry_numbers:
   - '2016'
   editor: ΓΛΑΡΟΣ // ΑΘΗΝΑ
   edition_year: 1983
@@ -6997,15 +6994,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 134
   authors:
-  - ΒΟΥΡΝ,Α.Ρ
+  - BURN,A.,R.
   language: el
   title: ΟΙ ΝΕΩΤΕΡΟΙ ΕΛΛΗΝΕΣ
   dewey: 938.9 BUR
   entry_numbers:
   - '2599'
   translators:
   - ΧΑΛΑΣ,Α.Φ.
@@ -7104,15 +7101,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 136
   authors:
-  - ΒΟΥΤΙΕΡΙΔΗΣ,ΗΛΙΑΣ Π
+  - ΒΟΥΤΙΕΡΙΔΗΣ,ΗΛΙΑΣ,Π.
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΝΕΟΕΛΛΗΝΙΚΗΣ ΛΟΓΟΤΕΧΝΕΙΑΣ
   subtitle: ΑΠΟ ΤΩΝ ΜΕΣΩΝ ΤΟΥ ΙΕ ΑΙΩΝΟΣ ΜΕΧΡΙ ΤΩΝ ΝΕΩΤΑΤΩΝ ΧΡΟΝΩΝ
   dewey: 880.09 ΒΟΥ
   entry_numbers:
   - '182'
   editor: ΖΗΚΑΚΗ // ΑΘΗΝΑ
@@ -7155,15 +7152,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 137
   authors:
-  - ΒΟΥΤΙΕΡΙΔΗΣ,ΗΛΙΑΣ Π.
+  - ΒΟΥΤΙΕΡΙΔΗΣ,ΗΛΙΑΣ.Π.
   language: el
   title: ΜΙΚΡΑΣΙΑ
   subtitle: ΣΑΝ ΘΡΥΛΟΣ ΤΡΑΓΙΚΟΣ
   dewey: 912 ΒΟΥ
   entry_numbers:
   - '2604'
   editor: None // ΑΘΗΝΑ
@@ -7207,15 +7204,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 138
   authors:
-  - ΒΡΑΝΟΥΣΗΣ,Λ
+  - ΒΡΑΝΟΥΣΗΣ,ΛΕΑΝΔΡΟΣ,Ι.
   language: el
   title: ΤΟ ΔΕΣΠΟΤΑΤΟ ΤΗΣ ΗΠΕΙΡΟΥ
   dewey: 938.375 ΒΡΑ
   entry_numbers:
   - '529'
   edition_year: 1990
   pages: 15
@@ -7257,15 +7254,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 139
   authors:
-  - ΒΡΑΝΟΥΣΗΣ,Λ
+  - ΒΡΑΝΟΥΣΗΣ,ΛΕΑΝΔΡΟΣ,Ι.
   language: el
   title: Η "ΑΝΟΙΞΗ" ΤΟΥ ΒΗΛΑΡΑ ΚΑΙ ΤΟ ΙΤΑΛΙΚΟ ΤΗΣ ΠΡΟΤΥΠΟ
   dewey: 880.4 ΒΡΑ
   entry_numbers:
   - '2716'
   editor: None // ΑΘΗΝΑ
   edition_year: 1980
@@ -7310,15 +7307,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 140
   authors:
-  - ΒΡΑΝΟΥΣΗΣ,Λ
+  - ΒΡΑΝΟΥΣΗΣ,ΛΕΑΝΔΡΟΣ,Ι.
   language: el
   title: Ο "ΠΑΤΡΙΩΤΙΚΟΣ ΥΜΝΟΣ" ΤΟΥ ΡΗΓΑ ΚΑΙ Η ΕΛΛΗΝΙΚΗ "ΚΑΡΜΑΝΙΟΛΑ"
   dewey: 938.483 ΒΡΑ
   entry_numbers:
   - '1797'
   editor: None // ΑΘΗΝΑ
   edition_year: 1960
@@ -7362,15 +7359,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 141
   authors:
-  - ΒΡΑΝΟΥΣΗΣ,Λ.Ι
+  - ΒΡΑΝΟΥΣΗΣ,ΛΕΑΝΔΡΟΣ,Ι.
   language: el
   title: ΡΗΓΑΣ ΒΕΛΕΣΤΙΝΛΗΣ (1757-1798)
   dewey: 938.483 ΒΡΑ
   entry_numbers:
   - '1795'
   editor: None // ΑΘΗΝΑ
   edition_year: 1957
@@ -7413,15 +7410,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 142
   authors:
-  - ΒΡΑΝΟΥΣΗΣ,Λ.Ι
+  - ΒΡΑΝΟΥΣΗΣ,ΛΕΑΝΔΡΟΣ,Ι.
   language: el
   title: '"ΕΠΑΙΝΟΣ ΙΩΑΝΝΙΝΩΝ"'
   subtitle: Η ΠΡΩΤΕΥΟΥΣΑ ΤΗΣ ΗΠΕΙΡΟΥ ΣΤΗΝ ΙΣΤΟΡΙΚΗ ΤΗΣ ΔΙΑΔΡΟΜΗ
   dewey: 938.492 ΒΡΑ
   entry_numbers:
   - '2267'
   editor: None // ΙΩΑΝΝΙΝΑ
@@ -7464,15 +7461,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 143
   authors:
-  - ΒΡΑΝΟΥΣΗΣ,Λ
+  - ΒΡΑΝΟΥΣΗΣ,ΛΕΑΝΔΡΟΣ,Ι.
   language: el
   title: Η ΕΝ ΗΠΕΙΡΩ ΜΟΝΗ ΣΩΣΙΝΟΥ
   dewey: 938.936 ΒΡΑ
   entry_numbers:
   - '2328'
   editor: None // ΑΘΗΝΑ
   edition_year: 1957
@@ -7515,15 +7512,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 144
   authors:
-  - ΒΡΑΝΟΥΣΗΣ,Λ.Ι
+  - ΒΡΑΝΟΥΣΗΣ,ΛΕΑΝΔΡΟΣ,Ι.
   language: el
   title: ΙΣΤΟΡΙΚΑ ΚΑΙ ΤΟΠΟΓΡΑΦΙΚΑ ΤΟΥ ΜΕΣΑΙΩΝΙΚΟΥ ΚΑΣΤΡΟΥ ΙΩΑΝΝΙΝΩΝ
   dewey: 938.21 ΒΡΑ
   entry_numbers:
   - '2260'
   editor: None // ΑΘΗΝΑ
   edition_year: 1968
@@ -7566,15 +7563,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 145
   authors:
-  - ΒΡΑΝΟΥΣΗΣ,Λ
+  - ΒΡΑΝΟΥΣΗΣ,ΛΕΑΝΔΡΟΣ,Ι.
   language: el
   title: ΤΟ ΔΕΣΠΟΤΑΤΟ ΤΗΣ ΗΠΕΙΡΟΥ
   dewey: 938.375 ΒΡΑ
   entry_numbers:
   - '2361'
   edition_year: 1990
   pages: 16
@@ -7616,15 +7613,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 146
   authors:
-  - ΒΡΑΝΟΥΣΗΣ,Λ
+  - ΒΡΑΝΟΥΣΗΣ,ΛΕΑΝΔΡΟΣ,Ι.
   language: el
   title: ΚΟΜΙΣΚΟΡΤΗΣ Ο ΕΞ ΑΡΒΑΝΩΝ
   subtitle: ΣΧΟΛΙΑ ΕΙΣ ΧΩΡΙΟΝ ΤΗΣ ΑΝΝΗΣ ΚΟΜΝΗΝΗΣ
   dewey: 398 ΒΡΑ
   entry_numbers:
   - '2062'
   editor: ΕΤΑΙΡ.ΗΠΕΙΡ.ΜΕΛΕΤΩΝ // ΙΩΑΝΝΙΝΑ
@@ -7667,15 +7664,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 147
   authors:
-  - ΒΡΑΝΟΠΟΥΛΟΣ,ΕΠΑΜ Α
+  - ΒΡΑΝΟΠΟΥΛΟΣ,ΕΠΑΜΕΙΝΩΝΔΑΣ,Α.
   language: el
   title: ΟΔΟΙΠΟΡΙΚΟ ΣΤΗ ΜΕΓΑΛΗ ΕΛΛΑΔΑ
   dewey: 938.199 ΒΡΑ
   entry_numbers:
   - '2465'
   editor: None // ΑΘΗΝΑ
   edition_year: 1989
@@ -7718,15 +7715,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 148
   authors:
-  - ΒΡΑΝΟΠΟΥΛΟΣ,ΕΠΑΜ.Α
+  - ΒΡΑΝΟΠΟΥΛΟΣ,ΕΠΑΜΕΙΝΩΝΔΑΣ,Α.
   language: el
   title: Η ΕΠΙΣΤΡΟΦΗ ΤΩΝ ΕΛΓΙΝΕΙΩΝ
   dewey: 938 ΒΡΑ
   entry_numbers:
   - '2499'
   - '2508'
   editor: None // ΑΘΗΝΑ
@@ -7769,15 +7766,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 149
   authors:
-  - ΒΡΕΛΛΗΣ,ΓΙΩΡΓΟΣ
+  - ΒΡΕΛΛΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΓΙΑΝΝΙΩΤΙΚΑ ΣΟΝΕΤΑ (1945-1979)
   dewey: 782.42 ΒΡΕ
   entry_numbers:
   - '739'
   - '740'
   - '741'
@@ -7824,15 +7821,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 150
   authors:
-  - ΒΡΕΛΛΗΣ,ΓΙΩΡΓΟΣ
+  - ΒΡΕΛΛΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΛΟΡΕΝΤΖΟΣ ΜΑΒΙΛΗΣ
   dewey: 889.16 ΒΡΕ
   entry_numbers:
   - '1146'
   editor: None // ΙΩΑΝΝΙΝΑ
   pages: 190
@@ -7875,15 +7872,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 151
   authors:
-  - ΒΡΕΛΛΗΣ,ΓΙΩΡΓΟΣ
+  - ΒΡΕΛΛΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΚΩΣΤΑΣ ΚΡΥΣΤΑΛΛΗΣ
   subtitle: ΤΟ ΠΟΝΕΜΕΝΟ Τ'ΑΓΝΟ ΠΑΙΔΙ ΤΗΣ ΠΙΝΔΟΥ
   dewey: 889.10 ΒΡΕ
   entry_numbers:
   - '1216'
   editor: None // ΙΩΑΝΝΙΝΑ
@@ -8450,55 +8447,39 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 162
-  authors:
-  - ΓΑΡΔΙΚΑΣ,ΓΕΩΡΓΙΟΣ Κ
-  language: el
-  title: ΙΦΙΓΕΝΕΙΑ Η ΕΝ ΑΥΛΙΔΙ
-  dewey: 881.24 ΕΥΡ
-  entry_numbers:
-  - '1455'
-  - '2664'
-  editor: None // ΑΘΗΝΑ
-  edition_year: 1962
-  pages: 215
-  topics:
-  - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
-  - ΘΕΑΤΡΟ
-  - ΑΡΧΑΙΟ
-  - ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ
-  - ΕΥΡΙΠΙΔΗΣ
-  - ΙΦΙΓΕΝΕΙΑ Η ΕΝ ΑΥΛΙΔΙ
-  copies: 2
+  authors: []
+  entry_numbers: []
+  topics: []
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 162
-    1: ΓΑΡΔΙΚΑΣ,ΓΕΩΡΓΙΟΣ Κ
-    2: ΙΦΙΓΕΝΕΙΑ Η ΕΝ ΑΥΛΙΔΙ
-    4: 881.24ΕΥΡ
-    5: 1455-2664
-    8: Χ.Ε
-    9: ΑΘΗΝΑ
-    10: '1962'
-    11: 215Σ
-    12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ-ΑΡΧΑΙΟ
-    13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΑΡΧΑΙΟ-ΕΥΡΙΠΙΔΗΣ
-    14: ΕΥΡΙΠΙΔΗΣ-ΙΦΙΓΕΝΕΙΑ Η ΕΝ ΑΥΛΙΔΙ
-    15: ΙΦΙΓΕΝΕΙΑ Η ΕΝ ΑΥΛΙΔΙ
-    17: 2 ΑΝΤΙΤΥΠΑ
+    1: null
+    2: null
     3: null
+    4: null
+    5: null
     6: null
     7: null
+    8: null
+    9: null
+    10: null
+    11: null
+    12: null
+    13: null
+    14: null
+    15: null
     16: null
+    17: null
     18: null
     19: null
     20: null
     21: null
     22: null
     23: null
     24: null
@@ -12433,15 +12414,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 238
     1: ΔΗΜΗΤΡΑΚΟΣ,ΔΗΜ
     2: Η ΕΥΡΩΠΗ
-    4: 914 ΔΗΜ
+    4: 914ΔΗΜ
     5: '386'
     8: ΔΗΜΗΤΡΑΚΟΥ
     9: ΑΘΗΝΑ
     10: '1931'
     11: 310Σ
     12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΕΥΡΩΠΗ
     13: ΕΥΡΩΠΗ-ΤΑΞΙΔΙΑ
@@ -12470,15 +12451,14 @@
   - ΔΗΜΙΤΣΑ,ΜΑΡΓΑΡΙΤΑ
   language: el
   title: ΒΙΟΓΡΑΦΙΑ ΟΛΥΜΠΙΑΔΟΣ ΤΗΣ ΗΠΕΙΡΩΤΙΔΟΣ ΝΕΟΠΤΟΛΕΜΟΥ ΤΟΥ ΑΛΚΕΤΟΥ
   subtitle: ΘΥΓΑΤΡΟΣ ΝΟΜΙΜΟΥ ΤΟΥ ΦΙΛΙΠΠΟΥ Β'ΓΥΝΑΙΚΟΣ ΚΑΙ ΑΛΕΞΑΝ.ΜΗΤΡΟΣ
   dewey: 938.17 ΔΗΜ
   entry_numbers:
   - '1947'
-  - '2357'
   editor: None // ΑΘΗΝΑ
   edition_year: 1887
   pages: 136
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΜΑΚΕΔΟΝΙΑ
   - ΜΑΚΕΔΟΝΙΚΗ ΚΥΡΙΑΡΧΙΑ
@@ -12491,16 +12471,16 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 239
     1: ΔΗΜΙΤΣΑ,ΜΑΡΓΑΡΙΤΑ
     2: ΒΙΟΓΡΑΦΙΑ ΟΛΥΜΠΙΑΔΟΣ ΤΗΣ ΗΠΕΙΡΩΤΙΔΟΣ ΝΕΟΠΤΟΛΕΜΟΥ ΤΟΥ ΑΛΚΕΤΟΥ
     3: ΘΥΓΑΤΡΟΣ ΝΟΜΙΜΟΥ ΤΟΥ ΦΙΛΙΠΠΟΥ Β'ΓΥΝΑΙΚΟΣ ΚΑΙ ΑΛΕΞΑΝ.ΜΗΤΡΟΣ
-    4: 938.17 ΔΗΜ
-    5: 1947-2357
+    4: 938.17ΔΗΜ
+    5: '1947'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1887'
     11: 136Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
     13: ΜΑΚΕΔΟΝΙΚΗ ΚΥΡΙΑΡΧΙΑ-ΟΛΥΜΠΙΑΔΑ
     14: ΟΛΥΜΠΙΑΔΑ-ΒΙΟΓΡΑΦΙΑ
@@ -12545,15 +12525,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 240
     1: ΔΗΜΟΠΟΥΛΟΣ,ΕΥΑΓ
     2: Η ΕΛΛΗΝΙΚΗ ΨΥΧΗ
     3: ΤΡΙΠΡΑΚΤΟΝ ΕΡΓΟΝ
-    4: 886.2 ΔΗΜ
+    4: 886.2ΔΗΜ
     5: '1463'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1949'
     11: 30Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΙΣΤΟΡΙΚΟ ΕΡΓΟ
@@ -13715,49 +13695,37 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 263
-  authors:
-  - ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ,ΤΖΕΝΗ
-  language: el
-  title: ΠΟΡΕΙΑ ΣΤΗ ΜΕΓΑΛΗ ΕΛΛΑΔΑ
-  dewey: 914.95 ΔΙΑ
-  entry_numbers:
-  - '391'
-  editor: None // ΑΘΗΝΑ
-  edition_year: 1969
-  pages: 172
-  topics:
-  - ΓΕΩΓΡΑΦΙΑ
-  - ΤΑΞΙΔΙΑ
-  - ΕΛΛΑΔΑ
-  - ΣΙΚΕΛΙΑ
+  authors: []
+  entry_numbers: []
+  topics: []
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 263
-    1: ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ,ΤΖΕΝΗ
-    2: ΠΟΡΕΙΑ ΣΤΗ ΜΕΓΑΛΗ ΕΛΛΑΔΑ
-    4: 914.95 ΔΙΑ
-    5: '391'
-    8: Χ.Ε
-    9: ΑΘΗΝΑ
-    10: '1969'
-    11: 172Σ
-    12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΕΛΛΑΔΑ
-    13: ΕΛΛΑΔΑ-ΤΑΞΙΔΙΑ
-    14: ΣΙΚΕΛΙΑ-ΤΑΞΙΔΙΑ
-    15: ΤΑΞΙΔΙΔΙΑ-ΕΛΛΑΔΑ-ΣΙΚΕΛΙΑ
+    1: null
+    2: null
     3: null
+    4: null
+    5: null
     6: null
     7: null
+    8: null
+    9: null
+    10: null
+    11: null
+    12: null
+    13: null
+    14: null
+    15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
     22: null
@@ -16277,14 +16245,15 @@
   authors:
   - ΕΥΡΙΠΙΔΗΣ
   language: el
   title: ΙΦΙΓΕΝΕΙΑ Η ΕΝ ΑΥΛΙΔΙ
   dewey: 881.24 ΕΥΡ
   entry_numbers:
   - '2664'
+  - '1455'
   translators:
   - ΓΑΡΔΙΚΑΣ,ΓΕΩΡΓΙΟΣ Κ.
   editor: None // ΑΘΗΝΑ
   edition_year: 1962
   pages: 215
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -16297,15 +16266,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 312
     1: ΕΥΡΙΠΙΔΗΣ
     2: ΙΦΙΓΕΝΕΙΑ Η ΕΝ ΑΥΛΙΔΙ
     4: 881.24ΕΥΡ
-    5: '2664'
+    5: 2664-1455
     6: ΓΑΡΔΙΚΑΣ,ΓΕΩΡΓΙΟΣ Κ
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1962'
     11: 215Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ-ΑΡΧΑΙΟ
     13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΑΡΧΑΙΟ
@@ -23488,15 +23457,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 450
     1: ΚΑΡΑΤΖΕΝΗΣ,ΔΗΜΗΤΡΙΟΣ ΦΩΤΙΟΣ
     2: ΕΠΑΝΑΣΤΑΣΙΣ ΚΑΙ ΚΑΤΑΣΤΡΟΦΗ ΚΑΛΑΡΥΤΩΝ-ΣΥΡΡΑΚΟΥ
-    4: 938.5 ΚΑΡ
+    4: 938.5ΚΑΡ
     5: '2054'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1988'
     11: 102Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΙΩΑΝΝΙΝΑ-ΚΑΛΑΡΡΥΤΕΣ-ΣΥΡΡΑΚΟ
     13: ΙΩΑΝΝΙΝΑ-ΚΑΛΑΡΡΥΤΕΣ-ΣΥΡΡΑΚΟ
@@ -24417,15 +24386,14 @@
   - ΚΑΡΟΛΙΔΟΥ,Π
   language: el
   title: ΣΥΓΧΡΟΝΟΣ ΙΣΤΟΡΙΑ ΤΩΝ ΕΛΛΗΝΩΝ ΚΑΙ ΤΩΝ ΛΟΙΠΩΝ ΛΑΩΝ ΤΗΣ ΑΝΑΤΟΛ
   subtitle: ΑΠΟ 1821 ΜΕΧΡΙ 1921
   dewey: 938.5 ΚΑΡ
   entry_numbers:
   - '2057'
-  - '2058'
   - '1750'
   - '2056'
   editor: ΒΙΤΣΙΚΟΥΝΑΚΗ // ΑΘΗΝΑ
   edition_year: 1929
   pages: 488
   topics:
   - 1821-1921
@@ -24439,15 +24407,15 @@
   offprint: false
   original_entry:
     0: 468
     1: ΚΑΡΟΛΙΔΟΥ,Π
     2: ΣΥΓΧΡΟΝΟΣ ΙΣΤΟΡΙΑ ΤΩΝ ΕΛΛΗΝΩΝ ΚΑΙ ΤΩΝ ΛΟΙΠΩΝ ΛΑΩΝ ΤΗΣ ΑΝΑΤΟΛ
     3: ΑΠΟ 1821 ΜΕΧΡΙ 1921
     4: 938.5 ΚΑΡ
-    5: 2057-2058-1750-2056
+    5: 2057-1750-2056
     8: ΒΙΤΣΙΚΟΥΝΑΚΗ
     9: ΑΘΗΝΑ
     10: '1929'
     11: 488Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-(1821-1921)
     13: 1821-ΕΛΛΑΔΑ
     14: ΑΝΑΤΟΛΗ-ΛΑΟΙ-1821
@@ -25399,31 +25367,30 @@
   authors:
   - ΚΑΤΩΠΟΔΗΣ,ΓΕΡΑΣΙΜΟΣ Σ
   language: el
   title: ΑΙΤΩΛΙΚΗ ΣΥΜΠΟΛΙΤΕΙΑ
   dewey: 938.22 ΚΑΤ
   entry_numbers:
   - '2322'
-  - '2291'
   editor: ΓΡΑΜΜΗ // ΑΘΗΝΑ
   edition_year: 1977
   pages: 457
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΑΙΤΩΛΙΑ
   - ΑΙΤΩΛΙΚΗ ΣΥΜΠΟΛΙΤΕΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 487
     1: ΚΑΤΩΠΟΔΗΣ,ΓΕΡΑΣΙΜΟΣ Σ
     2: ΑΙΤΩΛΙΚΗ ΣΥΜΠΟΛΙΤΕΙΑ
-    4: 938.22 ΚΑΤ
-    5: 2322-2291
+    4: 938.22ΚΑΤ
+    5: '2322'
     8: ΓΡΑΜΜΗ
     9: ΑΘΗΝΑ
     10: '1977'
     11: 457Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΙΤΩΛΙΑ
     13: ΑΙΤΩΛΙΑ
     14: ΑΙΤΩΛΙΚΗ ΣΥΜΠΟΛΙΤΕΙΑ
@@ -25467,15 +25434,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 488
     1: ΚΑΨΙΩΤΗΣ,ΑΘΑΝΑΣΙΟΣ  Η.
     2: ΘΕΣΣΑΛΟΙ ΟΙ ΠΡΩΤΟΙ ΑΥΤΟΧΘΟΝΕΣ ΕΛΛΗΝΕΣ
     3: ΚΑΙ ΠΡΩΤΟΙ ΑΠΟΙΚΟΙ ΝΗΣΙΩΝ ΤΟΥ ΑΙΓΑΙΟΥ ΚΑΙ ΤΩΝ ΜΙΚΡΑΣΙΑΤΚΩΝ Α
-    4: 938.21 ΚΑΨ
+    4: 938.21ΚΑΨ
     5: '2560'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1979'
     11: 198Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΕΣΣΑΛΙΑ
     13: ΘΕΣΣΑΛΙΑ-ΘΕΣΣΑΛΟΙ
@@ -30973,15 +30940,14 @@
   authors:
   - ΛΑΜΠΡΙΔΗΣ,ΙΩΑΝΝΗΣ
   language: el
   title: ΗΠΕΙΡΩΤΙΚΑ ΑΓΑΘΟΕΡΓΗΜΑΤΑ ΚΑΙ ΑΛΛΑ ΔΗΜΟΣΙΕΥΜΑΤΑ
   dewey: 938.5 ΛΑΜ
   entry_numbers:
   - '2053'
-  - '2054'
   editor: None // ΙΩΑΝΝΙΝΑ
   edition_year: 1971
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΗΠΕΙΡΟΣ
   - ΔΗΜΟΣΙΕΥΜΑΤΑ
   - ΑΓΑΘΟΕΡΓΗΜΑΤΑ
@@ -30989,15 +30955,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 594
     1: ΛΑΜΠΡΙΔΗΣ,ΙΩΑΝΝΗΣ
     2: ΗΠΕΙΡΩΤΙΚΑ ΑΓΑΘΟΕΡΓΗΜΑΤΑ ΚΑΙ ΑΛΛΑ ΔΗΜΟΣΙΕΥΜΑΤΑ
     4: 938.5 ΛΑΜ
-    5: 2053-2054
+    5: '2053'
     8: Χ.Ε
     9: ΙΩΑΝΝΙΝΑ
     10: '1971'
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΔΗΜΟΣΙΕΥΜΑΤΑ
     14: ΔΗΜΟΣΙΕΥΜΑΤΑ
     15: ΑΓΑΘΟΕΡΓΗΜΑΤΑ
@@ -31040,15 +31006,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 595
     1: ΛΑΜΠΡΙΔΗΣ,ΙΩΑΝΝΗΣ
     2: ΗΠΕΙΡΩΤΙΚΑ ΜΕΛΕΤΗΜΑΤΑ
     4: 938.501ΛΑΜ
-    5: 2052-2357-
+    5: 2052-2357
     8: ΕΤΑΙΡ.ΗΠΕΙΡ.ΜΕΛΕΤΩΝ
     9: ΙΩΑΝΝΙΝΑ
     10: '1971'
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΜΕΛΕΤΗΜΑΤΑ
     14: ΜΕΛΕΤΗΜΑΤΑ-ΗΠΕΙΡΟΣ
     15: ΗΠΕΙΡΩΤΙΚΑ ΜΕΛΕΤΗΜΑΤΑ
@@ -33531,15 +33497,15 @@
   language: el
   title: ΗΠΕΙΡΟΣ ΚΑΙ ΛΑΚΩΝΙΑ ΑΠΟ ΤΗΝ ΣΠΛΑΝΤΖΑ
   subtitle: ΕΩΣ ΤΟΝ ΑΥΤΟΝΟΜΙΑΚΟΝ ΑΓΩΝΑ 1914
   dewey: 938.68 ΜΑΜ
   entry_numbers:
   - '2042'
   - '2043'
-  - 9250Α
+  - 09250
   editor: None // ΑΘΗΝΑ
   edition_year: 1968
   pages: 38
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΗΠΕΙΡΟΣ
   - ΛΑΚΩΝΙΑ
@@ -33549,15 +33515,15 @@
   offprint: false
   original_entry:
     0: 643
     1: ΜΑΜΜΟΠΟΥΛΟΣ,ΑΛΕΞΑΝΔΡΟΣ Χ.
     2: ΗΠΕΙΡΟΣ ΚΑΙ ΛΑΚΩΝΙΑ ΑΠΟ ΤΗΝ ΣΠΛΑΝΤΖΑ
     3: ΕΩΣ ΤΟΝ ΑΥΤΟΝΟΜΙΑΚΟΝ ΑΓΩΝΑ 1914
     4: 938.68ΜΑΜ
-    5: 2042-2043-9250Α
+    5: 2042-2043-09250
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1968'
     11: 38Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΛΑΚΩΝΙΑ
     14: ΛΑΚΩΝΙΑ-ΗΠΕΙΡΟΣ
@@ -33840,15 +33806,14 @@
   authors:
   - ΜΑΝΟΥΚΑΣ,ΓΕΩΡΓΙΟΣ Χ
   language: el
   title: ΠΑΙΔΟΜΑΖΩΜΑ
   subtitle: ΤΟ ΜΕΓΑΛΟ ΕΓΚΛΗΜΑ ΚΑΤΑ ΤΗΣ ΦΥΛΗΣ
   dewey: 938.413 ΜΑΝ
   entry_numbers:
-  - '1823'
   - '8509'
   - '9274'
   editor: None // ΑΘΗΝΑ
   edition_year: 1961
   pages: 254
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -33860,15 +33825,15 @@
   offprint: false
   original_entry:
     0: 649
     1: ΜΑΝΟΥΚΑΣ,ΓΕΩΡΓΙΟΣ Χ
     2: ΠΑΙΔΟΜΑΖΩΜΑ
     3: ΤΟ ΜΕΓΑΛΟ ΕΓΚΛΗΜΑ ΚΑΤΑ ΤΗΣ ΦΥΛΗΣ
     4: 938.413ΜΑΝ
-    5: 1823-8509-9274
+    5: 8509-9274
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1961'
     11: 254Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΑΙΔΟΜΑΖΩΜΑ
     13: ΠΑΙΔΟΜΑΖΩΜΑ
     14: ΠΑΙΔΙ-ΠΑΙΔΟΜΑΖΩΜΑ
@@ -33947,15 +33912,14 @@
   - ΜΑΡΑΖΙΩΤΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: Ο ΗΠΕΙΡΩΤΗΣ ΕΘΝΑΠΟΣΤΟΛΟΣ ΠΕΤΡΟΣ ΗΠΙΤΗΣ
   dewey: 938.5 ΜΑΡ
   entry_numbers:
   - '2061'
   - '2760'
-  - '9258'
   editor: None // ΑΘΗΝΑ
   edition_year: 1973
   pages: 50
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΗΠΕΙΡΟΣ
   - ΕΘΝΑΠΟΣΤΟΛΟΣ
@@ -33964,15 +33928,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 651
     1: ΜΑΡΑΖΙΩΤΗΣ,ΓΕΩΡΓΙΟΣ
     2: Ο ΗΠΕΙΡΩΤΗΣ ΕΘΝΑΠΟΣΤΟΛΟΣ ΠΕΤΡΟΣ ΗΠΙΤΗΣ
     4: 938.5ΜΑΡ
-    5: 2061-2760-9258
+    5: 2061-2760
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1973'
     11: 50Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΕΘΝΑΠΟΣΤΟΛΟΣ
     13: ΗΠΕΙΡΟΣ-ΗΠΙΤΗΣ
     14: ΗΠΙΤΗΣ-ΕΘΝΑΠΟΣΤΟΛΟΣ
@@ -35695,15 +35659,15 @@
 - dbase_number: 685
   authors:
   - ΜΗΤΣΟΤΑΚΗΣ,ΚΥΡΙΑΚΟΣ
   language: el
   title: ΠΡΟΣΩΠΑ ΚΑΙ ΤΟΠΟΙ
   dewey: 889.21 ΜΗΤ
   entry_numbers:
-  - '2533'
+  - '2048'
   editor: ΑΙΓΑΓΡΟΣ // ΑΘΗΝΑ
   edition_year: 1966
   pages: 116
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΠΡΟΣΩΠΑ
   - ΕΛΛΑΔΑ
@@ -35712,15 +35676,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 685
     1: ΜΗΤΣΟΤΑΚΗΣ,ΚΥΡΙΑΚΟΣ
     2: ΠΡΟΣΩΠΑ ΚΑΙ ΤΟΠΟΙ
     4: 889.21ΜΗΤ
-    5: '2533'
+    5: '2048'
     8: ΑΙΓΑΓΡΟΣ
     9: ΑΘΗΝΑ
     10: '1966'
     11: 116Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
     13: ΠΡΟΣΩΠΑ-ΕΛΛΑΔΑ
     14: ΤΟΠΟΙ-ΕΛΛΑΔΑ
@@ -36721,14 +36685,15 @@
     30: null
 - dbase_number: 705
   authors:
   - MURAT,JOHN
   language: el
   title: ΤΟ ΜΕΓΑΛΥΤΕΡΟ ΕΓΚΛΗΜΑ ΤΟΥ ΑΙΩΝΑ
   subtitle: ΤΟ ΞΕΚΛΗΡΙΣΜΑ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
+  dewey: 938.001 MUR
   entry_numbers:
   - '2082'
   - '1950'
   edition_year: 1982
   pages: 542
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -36738,15 +36703,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 705
     1: MURAT,JOHN
     2: ΤΟ ΜΕΓΑΛΥΤΕΡΟ ΕΓΚΛΗΜΑ ΤΟΥ ΑΙΩΝΑ
     3: ΤΟ ΞΕΚΛΗΡΙΣΜΑ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
-    4: 938.ΟΟ1MUR
+    4: 938.001MUR
     5: 2082-1950
     8: Χ.Ε
     9: Χ.Τ
     10: '1982'
     11: 542Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΣΜΟΣ
     13: ΕΛΛΗΝΙΣΜΟΣ-ΞΕΚΛΗΡΙΣΜΑ
@@ -38626,15 +38591,15 @@
   authors:
   - ΜΥΡΙΒΗΛΗΣ,ΣΤΡΑΤΗΣ
   language: el
   title: ΤΟ ΚΟΚΚΙΝΟ ΒΙΒΛΙΟ
   dewey: 889.34 ΜΥΡ
   entry_numbers:
   - '1185'
-  - 9143Α
+  - 09143
   edition: '3'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 1956
   pages: 186
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΠΕΖΟΓΡΑΦΙΑ
@@ -38643,15 +38608,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 742
     1: ΜΥΡΙΒΗΛΗΣ,ΣΤΡΑΤΗΣ
     2: ΤΟ ΚΟΚΚΙΝΟ ΒΙΒΛΙΟ
     4: 889.34ΜΥΡ
-    5: 1185-9143Α
+    5: 1185-09143
     7: 3ΕΚΔ
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: '1956'
     11: 186Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
     13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ
@@ -38878,15 +38843,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 747
   authors:
-  - ΑΛΙΠΡΑΝΤΗΣ,ΝΙΚΟΣ ΧΡ
+  - ΑΛΙΠΡΑΝΤΗΣ,ΝΙΚΟΣ,ΧΡ.
   language: el
   title: ΕΘΝΙΚΑ ΟΝΟΜΑΤΑ ΣΤΗΝ ΠΑΡΟ
   dewey: 938.972 ΑΛΙ
   entry_numbers:
   - '2338'
   editor: None // ΑΘΗΝΑ
   edition_year: 1984
@@ -39187,15 +39152,15 @@
   - ΚΙΤΣΟΣ,ΑΘΑΝΑΣΙΟΣ
   language: el
   title: ΘΕΣΠΡΩΤΙΚΗ ΓΗ
   dewey: 938.937 ΚΙΤ
   entry_numbers:
   - '2763'
   - '2790'
-  - 9253Α
+  - 09253
   editor: None // ΑΘΗΝΑ
   edition_year: 1977
   pages: 37
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΘΕΣΠΡΩΤΙΑ
   copies: 3
@@ -39204,15 +39169,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 753
     1: ΚΙΤΣΟΣ,ΑΘΑΝΑΣΙΟΣ
     2: ΘΕΣΠΡΩΤΙΚΗ ΓΗ
     4: 938.937ΚΙΤ
-    5: 2763-2790-9253Α
+    5: 2763-2790-09253
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1977'
     11: 37Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΕΣΠΡΩΤΙΑ
     13: ΘΕΣΠΡΩΤΙΑ-ΙΣΤΟΡΙΑ
     17: 3 ΑΝΤΙΤΥΠΑ
@@ -39601,15 +39566,15 @@
   authors:
   - ΜΠΟΤΣΑΡΗΣ,ΔΗΜ Τ ΝΟΤΗ
   language: el
   title: ΑΓΩΝΕΣ ΕΛΕΥΘΕΡΙΑΣ
   dewey: 938.526 ΜΠΟ
   entry_numbers:
   - '2769'
-  - 9260Α
+  - 09260
   editor: None // ΑΘΗΝΑ
   edition_year: 1973
   pages: 76
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΗΠΕΙΡΟΣ
   - ΣΟΥΛΙ
@@ -39618,24 +39583,24 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 761
     1: ΜΠΟΤΣΑΡΗΣ,ΔΗΜ Τ ΝΟΤΗ
     2: ΑΓΩΝΕΣ ΕΛΕΥΘΕΡΙΑΣ
     4: 938.526ΜΠΟ
-    5: 2769-9260Α
-    6: '     -'
+    5: 2769-09260
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1973'
     11: 76Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΣΟΥΛΙ
     14: ΣΟΥΛΙ-ΑΓΩΝΕΣ
     3: null
+    6: null
     7: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
@@ -43806,21 +43771,18 @@
 - dbase_number: 843
   authors:
   - ΠΑΠΑΓΕΩΡΓΙΟΥ,ΣΠΥΡΟΣ
   language: el
   title: ΤΑ ΚΡΙΣΙΜΑ  ΝΤΟΚΟΥΜΕΝΤΑ ΤΟΥ ΚΥΠΡΙΑΚΟΥ
   dewey: 938.497 ΠΑΠ
   entry_numbers:
+  - '2394'
+  - '2395'
+  - '2396'
   - '2397'
-  - '2398'
-  - '2399'
-  - '2857'
-  - '2852'
-  - '2853'
-  - '2854'
   editor: ΛΑΔΙΑ // ΑΘΗΝΑ
   edition_year: 1983
   pages: 378
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΚΥΠΡΟΣ
   - ΚΥΠΡΙΑΚΟ
@@ -43829,24 +43791,24 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 843
     1: ΠΑΠΑΓΕΩΡΓΙΟΥ,ΣΠΥΡΟΣ
     2: ΤΑ ΚΡΙΣΙΜΑ  ΝΤΟΚΟΥΜΕΝΤΑ ΤΟΥ ΚΥΠΡΙΑΚΟΥ
     4: 938.497ΠΑΠ
-    5: 2397-2398-2399-2857-
-    6: 2852-2853-2854
+    5: 2394-2395-2396-2397
     8: ΛΑΔΙΑ
     9: ΑΘΗΝΑ
     10: '1983'
     11: 378Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
     13: ΚΥΠΡΟΣ-ΚΥΠΡΙΑΚΟ
     14: ΝΤΟΚΟΥΜΕΝΤΑ-ΚΥΠΡΙΑΚΟ
     3: null
+    6: null
     7: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
@@ -43863,22 +43825,18 @@
 - dbase_number: 844
   authors:
   - ΠΑΠΑΓΕΩΡΓΙΟΥ,ΣΠΥΡΟΣ
   language: el
   title: ΑΠΟ ΤΗΝ ΖΥΡΙΧΗΝ ΕΙΣ ΤΟΝ ΑΤΤΙΛΑΝ
   dewey: 938.497 ΠΑΠ
   entry_numbers:
-  - '2394'
-  - '2395'
-  - '2396'
+  - '2854'
   - '2855'
   - '2856'
   - '2857'
-  - '5201'
-  - '5200'
   editor: ΛΑΔΙΑ // ΑΘΗΝΑ
   pages: 350
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΚΥΠΡΟΣ
   - ΦΑΚΕΛΛΟΣ
   - ΑΤΤΙΛΑΣ
@@ -43887,25 +43845,25 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 844
     1: ΠΑΠΑΓΕΩΡΓΙΟΥ,ΣΠΥΡΟΣ
     2: ΑΠΟ ΤΗΝ ΖΥΡΙΧΗΝ ΕΙΣ ΤΟΝ ΑΤΤΙΛΑΝ
     4: 938.497ΠΑΠ
-    5: 2394-2395-2396-2855-
-    6: 2856-2857-5201-5200
+    5: 2854-2855-2856-2857
     8: ΛΑΔΙΑ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 350Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
     13: ΚΥΠΡΟΣ-ΦΑΚΕΛΛΟΣ
     14: ΑΤΤΙΛΑΣ-ΚΥΠΡΟΣ
     15: ΖΥΡΙΧΗ-ΚΥΠΡΟΣ
     3: null
+    6: null
     7: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -45630,15 +45588,15 @@
   - ΠΑΠΑΘΑΝΑΣΙΟΥ,ΖΗΣΗΣ
   language: el
   title: ΣΠΥΡΟΣ ΧΑΣΙΩΤΗΣ
   subtitle: Ο ΗΠΕΙΡΩΤΗΣ ΠΑΤΗΡ ΤΗΣ ΓΕΩΡΓΙΑΣ
   dewey: 938.629 ΠΑΠ
   entry_numbers:
   - '2028'
-  - 2029Α
+  - '2029'
   editor: None // ΑΘΗΝΑ
   edition_year: 1969
   pages: 27
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΗΠΕΙΡΟΣ
   - ΧΑΣΙΩΤΗΣ
@@ -45649,15 +45607,15 @@
   offprint: false
   original_entry:
     0: 878
     1: ΠΑΠΑΘΑΝΑΣΙΟΥ,ΖΗΣΗΣ
     2: ΣΠΥΡΟΣ ΧΑΣΙΩΤΗΣ
     3: Ο ΗΠΕΙΡΩΤΗΣ ΠΑΤΗΡ ΤΗΣ ΓΕΩΡΓΙΑΣ
     4: 938.629ΠΑΠ
-    5: 2028-2029Α
+    5: 2028-2029
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1969'
     11: 27Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΧΑΣΙΩΤΗΣ
     14: ΧΑΣΙΩΤΗΣ-ΗΠΕΙΡΩΤΗΣ
@@ -47500,15 +47458,15 @@
   language: el
   title: ΛΟΡΕΤΖΟΣ ΜΑΒΙΛΗΣ
   subtitle: Ο ΗΡΩΣ ΤΟΥ ΔΡΙΣΚΟΥ
   dewey: 938.654 ΠΕΡ
   entry_numbers:
   - '2036'
   - '2037'
-  - 9267Α
+  - 09267
   editor: None // ΑΘΗΝΑ
   edition_year: 1969
   pages: 23
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΜΑΒΙΛΗΣ
   - ΔΡΙΣΚΟ
@@ -47517,15 +47475,15 @@
   offprint: false
   original_entry:
     0: 914
     1: ΠΕΡΑΝΘΗΣ,ΜΙΧΑΗΛ
     2: ΛΟΡΕΤΖΟΣ ΜΑΒΙΛΗΣ
     3: Ο ΗΡΩΣ ΤΟΥ ΔΡΙΣΚΟΥ
     4: 938.654ΠΕΡ
-    5: 2036-2037-9267Α
+    5: 2036-2037-09267
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1969'
     11: 23Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΒΙΛΗΣ
     13: ΜΑΒΙΛΗΣ-ΔΡΙΣΚΟ
     14: ΔΡΙΣΚΟ-ΜΑΒΙΛΗΣ
@@ -47572,15 +47530,15 @@
   offprint: false
   original_entry:
     0: 915
     1: ΠΕΡΑΝΘΗΣ,ΜΙΧ
     2: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ
     3: 1453 ΕΩΣ ΣΗΜΕΡΑ
     4: 880.08ΠΕΡ
-    5: 205-206-207-208-209-
+    5: 205-206-207-208-209
     8: Χ.Ε
     9: Χ.Τ
     10: Χ.Χ
     11: 607Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
     13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ-ΙΣΤΟΡΙΑ
     14: ΠΕΖΟΓΡΑΦΙΑ-ΙΣΤΟΡΙΑ
@@ -48070,15 +48028,14 @@
   - ΠΕΡΑΝΘΗΣ,ΜΙΧ
   language: el
   title: ΑΜΒΡΑΚΙΑ
   subtitle: ΧΡΟΝΟΓΡΑΦΙΑ ΜΙΑΣ ΠΡΩΤΕΥΟΥΣΑΣ
   dewey: 938.21 ΠΕΡ
   entry_numbers:
   - '2187'
-  - '2273'
   - '13268'
   editor: None // ΑΘΗΝΑ
   edition_year: 1954
   pages: 212
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΑΜΒΡΑΚΙΑ
@@ -48088,15 +48045,15 @@
   offprint: false
   original_entry:
     0: 925
     1: ΠΕΡΑΝΘΗΣ,ΜΙΧ
     2: ΑΜΒΡΑΚΙΑ
     3: ΧΡΟΝΟΓΡΑΦΙΑ ΜΙΑΣ ΠΡΩΤΕΥΟΥΣΑΣ
     4: 938.21ΠΕΡ
-    5: 2187-2273-13268
+    5: 2187-13268
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1954'
     11: 212Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΜΒΡΑΚΙΑ
     13: ΑΜΒΡΑΚΙΑ-ΧΡΟΝΟΓΡΑΦΙΑ
     14: ΧΡΟΝΟΓΡΑΦΙΑ
@@ -55695,15 +55652,15 @@
   authors:
   - ΣΑΚΚΑΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: Η ΙΣΤΟΡΙΑ ΤΩΝ ΕΛΛΗΝΩΝ ΤΗΣ ΤΡΙΠΟΛΕΩΣ ΤΟΥ ΠΟΝΤΟΥ
   dewey: 938.498 ΣΑΚ
   entry_numbers:
   - '2123'
-  - 9277Α
+  - 09277
   editor: None // ΑΘΗΝΑ
   edition_year: 1957
   pages: 254
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΤΡΙΠΟΛΗ
   - ΠΟΝΤΟΣ
@@ -55711,15 +55668,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1070
     1: ΣΑΚΚΑΣ,ΓΕΩΡΓΙΟΣ
     2: Η ΙΣΤΟΡΙΑ ΤΩΝ ΕΛΛΗΝΩΝ ΤΗΣ ΤΡΙΠΟΛΕΩΣ ΤΟΥ ΠΟΝΤΟΥ
     4: 938.498ΣΑΚ
-    5: 2123-9277Α
+    5: 2123-09277
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1957'
     11: 254Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΡΙΠΟΛΗ-ΠΟΝΤΟΣ
     13: ΤΡΙΠΟΛΗ-ΠΟΝΤΟΣ
     14: ΠΟΝΤΟΣ-ΤΡΙΠΟΛΗ
@@ -56015,15 +55972,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1076
     1: ΣΑΡΑΝΤΗΣ,ΘΕΟΔΩΡΟΣ Κ.Π.
     2: Ο ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ ΑΠΟ ΤΗΝ ΙΣΤΟΡΙΑ ΕΩΣ ΤΟΝ ΘΡΥΛΟ
     4: 938.174ΣΑΡ
-    5: 2197-2198-
+    5: 2197-2198
     8: Χ.Ρ
     9: ΑΘΗΝΑ
     10: '1970'
     11: 396Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΡΟΣ
     13: ΜΕΓΑΣ ΑΛΕΞΑΝΡΟΣ
     3: null
@@ -56051,15 +56008,15 @@
   - ΣΑΡΑΝΤΗΣ,ΘΕΟΔΩΡΟΥ Κ.
   language: el
   title: ΤΟ ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟ ΖΗΤΗΜΑ ΚΑΙ Ο ΝΑΠΟΛΕΩΝ
   dewey: 938.694 ΣΑΡ
   entry_numbers:
   - '2778'
   - '2868'
-  - 9273Α
+  - 09273
   editor: None // ΑΘΗΝΑ
   edition_year: 1985
   pages: 22
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟ ΖΗΤΗΜΑ
   - ΒΟΡΕΙΑ ΗΠΕΙΡΟΣ
@@ -56069,15 +56026,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1077
     1: ΣΑΡΑΝΤΗΣ,ΘΕΟΔΩΡΟΥ Κ.
     2: ΤΟ ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟ ΖΗΤΗΜΑ ΚΑΙ Ο ΝΑΠΟΛΕΩΝ
     4: 938.694ΣΑΡ
-    5: 2778-2868-9273Α
+    5: 2778-2868-09273
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1985'
     11: 22Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟ ΖΗΤΗΜΑ
     13: ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟ ΖΗΤΗΜΑ
     14: Β.ΗΠΕΙΡΟΣ-ΖΗΤΗΜΑ
@@ -57848,17 +57805,15 @@
 - dbase_number: 1112
   authors:
   - ΣΙΩΜΟΠΟΥΛΟΣ,ΔΗΜ Β.
   language: el
   title: ΗΠΕΙΡΩΤΙΚΑ
   dewey: 938.21 ΣΙΩ
   entry_numbers:
-  - '2188'
   - '2520'
-  - '2578'
   editor: None // ΙΩΑΝΝΙΝΑ
   edition_year: 1975
   pages: 245
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΗΠΕΙΡΟΣ
   - ΗΠΕΙΡΩΤΙΚΑ
@@ -57866,15 +57821,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1112
     1: ΣΙΩΜΟΠΟΥΛΟΣ,ΔΗΜ Β.
     2: ΗΠΕΙΡΩΤΙΚΑ
     4: 938.21ΣΙΩ
-    5: 2188-2520-2578
+    5: '2520'
     8: Χ.Ε
     9: ΙΩΑΝΝΙΝΑ
     10: '1975'
     11: 245Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΗΠΕΙΡΩΤΙΚΑ
     14: ΗΠΕΙΡΩΤΙΚΑ
@@ -58419,18 +58374,18 @@
 - dbase_number: 1123
   authors:
   - ΣΟΛΔΑΤΟΣ,ΓΙΑΝΝΗΣ
   language: el
   title: ΙΣΤΟΡΙΑ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΚΙΝΗΜΑΤΟΓΡΑΦΟΥ
   dewey: 880.203 ΣΟΛ
   entry_numbers:
-  - '2435'
   - '2434'
-  - '2437'
+  - '2435'
   - '2436'
+  - '2437'
   edition: '5'
   editor: ΑΙΓΟΚΕΡΩΣ // ΑΘΗΝΑ
   edition_year: 1989
   pages: 254
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
@@ -58439,15 +58394,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1123
     1: ΣΟΛΔΑΤΟΣ,ΓΙΑΝΝΗΣ
     2: ΙΣΤΟΡΙΑ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΚΙΝΗΜΑΤΟΓΡΑΦΟΥ
     4: 880.203ΣΟΛ
-    5: 2435-2434-2437-2436-
+    5: 2434-2435-2436-2437
     7: 5ΕΚΔ
     8: ΑΙΓΟΚΕΡΩΣ
     9: ΑΘΗΝΑ
     10: '1989'
     11: 254Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
     13: ΕΛΛΗΝΙΚΟΣ ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΙΣΤΟΡΙΑ
@@ -61072,15 +61027,14 @@
 - dbase_number: 1174
   authors:
   - ΣΤΕΡΓΙΟΠΟΥΛΟΣ,Κ.Δ
   language: el
   title: Η ΑΡΧΑΙΑ ΑΙΤΩΛΙΑ
   dewey: 938.22 ΣΤΕ
   entry_numbers:
-  - '2215'
   - '2587'
   editor: ΔΗΜΗΤΡΑΚΟΥ // ΑΘΗΝΑ
   edition_year: 1939
   pages: 191
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΑΡΧΑΙΑ
@@ -61090,15 +61044,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1174
     1: ΣΤΕΡΓΙΟΠΟΥΛΟΣ,Κ.Δ
     2: Η ΑΡΧΑΙΑ ΑΙΤΩΛΙΑ
     4: 938.22ΣΤΕ
-    5: 2215-2587
+    5: '2587'
     8: ΔΗΜΗΤΡΑΚΟΥ
     9: ΑΘΗΝΑ
     10: '1939'
     11: 191Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
     13: ΑΡΧΑΙΑ ΙΣΤΟΡΙΑ-ΑΙΤΩΛΙΑ
     14: ΑΙΤΩΛΙΑ-ΑΡΧΑΙΑ
@@ -62626,15 +62580,15 @@
 - dbase_number: 1204
   authors:
   - ΤΑΡΝΑΝΑΣ,ΑΝΤΡΕΑΣ
   language: el
   title: ΓΟΥΝΤΥ ΑΛΛΕΝ
   dewey: 800.203 ΤΑΡ
   entry_numbers:
-  - '1625'
+  - '5393'
   editor: ΑΙΓΟΚΕΡΩΣ // ΑΘΗΝΑ
   edition_year: 1984
   pages: 82
   topics:
   - ΠΑΓΚΟΣΜΙΟΣ ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
   - ΑΡΧΕΙΟ
   - ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
@@ -62643,15 +62597,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1204
     1: ΤΑΡΝΑΝΑΣ,ΑΝΤΡΕΑΣ
     2: ΓΟΥΝΤΥ ΑΛΛΕΝ
     4: 800.203ΤΑΡ
-    5: '1625'
+    5: '5393'
     8: ΑΙΓΟΚΕΡΩΣ
     9: ΑΘΗΝΑ
     10: '1984'
     11: 82Σ
     12: ΠΑΓΚΟΣΜΙΟΣ ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΑΡΧΕΙΟ
     13: ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΑΡΧΕΙΟ
     14: ΑΡΧΕΙΟ-ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
@@ -62886,15 +62840,15 @@
   title: ΝΙΚΟΛΑΟΣ ΣΚΟΥΦΑΣ
   subtitle: Ο ΕΘΝΕΓΕΡΤΗΣ ΑΡΧΗΓΟΣ ΤΗΣ ΦΙΛΙΚΗΣ ΕΤΑΙΡΕΙΑΣ
   dewey: 938.487 ΤΑΤ
   entry_numbers:
   - '2256'
   - '1034'
   - '1661'
-  - '1482.'
+  - '1482'
   editor: None // ΙΩΑΝΝΙΝΑ
   edition_year: 1980
   pages: 73
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΣΚΟΥΦΑΣ
   - ΦΙΛΙΚΗ ΕΤΑΙΡΕΙΑ
@@ -62904,15 +62858,15 @@
   offprint: false
   original_entry:
     0: 1209
     1: ΤΑΤΣΙΟΠΟΥΛΟΣ,ΛΑΜΠΡΟΣ ΑΠ
     2: ΝΙΚΟΛΑΟΣ ΣΚΟΥΦΑΣ
     3: Ο ΕΘΝΕΓΕΡΤΗΣ ΑΡΧΗΓΟΣ ΤΗΣ ΦΙΛΙΚΗΣ ΕΤΑΙΡΕΙΑΣ
     4: 938.487ΤΑΤ
-    5: 2256-1034-1661-1482.
+    5: 2256-1034-1661-1482
     8: Χ.Ε
     9: ΙΩΑΝΝΙΝΑ
     10: '1980'
     11: 73Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΣΚΟΥΦΑΣ
     13: ΣΚΟΥΦΑΣ-ΦΙΛΙΚΗ ΕΤΑΙΡΕΙΑ
     14: ΦΙΛΙΚΗ ΕΤΑΙΡΕΙΑ-ΣΚΟΥΦΑΣ
@@ -64058,15 +64012,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1232
   authors:
-  - ΑΠΟΣΤΟΛΑΚΗΣ,ΣΤΑΜΑΤΙΟΣ Α.
+  - ΑΠΟΣΤΟΛΑΚΗΣ,ΣΤΑΜΑΤΙΟΣ,Α.
   language: el
   title: ΤΟΠΩΝΥΜΙΚΟΝ ΚΑΜΠΑΝΟΥ
   subtitle: ΧΑΝΙΩΝ ΚΡΗΤΗΣ
   dewey: 938.981 ΑΠΟ
   entry_numbers:
   - '970'
   editor: None // ΑΘΗΝΑ
@@ -64981,15 +64935,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1250
   authors:
-  - ΒΙΤΤΗΣ,ΦΩΤΗΣ Σ.
+  - ΒΙΤΤΗΣ,ΦΩΤΗΣ,Σ.
   language: el
   title: ΙΣΤΟΡΙΚΑ ΠΑΡΑΔΟΣΙΑΚΑ ΠΑΡΑΘΕΜΑΤΑ
   dewey: 938.4 ΒΙΤ
   entry_numbers:
   - '2766'
   editor: None // ΑΘΗΝΑ
   edition_year: 1984
@@ -65038,15 +64992,15 @@
   - ΛΑΜΠΡΙΔΗΣ,ΣΤΑΘΗΣ Δ.
   language: el
   title: ΧΡΙΣΤΟΔΟΥΛΟΣ ΚΛΟΝΑΡΗΣ,ΖΑΓΟΡΙΤΗΣ Ο ΠΡΩΤΟΣ ΠΡΟΕΔΡΟΣ
   subtitle: ΤΟΥ ΑΡΕΙΟΥ ΠΑΓΟΥ
   dewey: 938.503 ΛΑΜ
   entry_numbers:
   - '2793'
-  - 9259Α
+  - 09259
   editor: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ // ΑΘΗΝΑ
   edition_year: 1975
   pages: 43
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΠΡΟΣΩΠΑ
   - ΚΛΟΝΑΡΗΣ
@@ -65056,15 +65010,15 @@
   offprint: false
   original_entry:
     0: 1251
     1: ΛΑΜΠΡΙΔΗΣ,ΣΤΑΘΗΣ Δ.
     2: ΧΡΙΣΤΟΔΟΥΛΟΣ ΚΛΟΝΑΡΗΣ,ΖΑΓΟΡΙΤΗΣ Ο ΠΡΩΤΟΣ ΠΡΟΕΔΡΟΣ
     3: ΤΟΥ ΑΡΕΙΟΥ ΠΑΓΟΥ
     4: 938.503ΛΑΜ
-    5: 2793-9259Α
+    5: 2793-09259
     8: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ
     9: ΑΘΗΝΑ
     10: '1975'
     11: 43Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΩΣΟΠΑ
     13: ΚΛΟΝΑΡΗΣ-ΑΡΕΙΟΣ ΠΑΓΟΣ
     14: ΑΡΕΙΟΣ ΠΑΓΟΣ-ΚΛΟΝΑΡΗΣ
@@ -65349,15 +65303,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1257
   authors:
-  - ADAMS,TUSLO,ADAMS
+  - TRUSLOW ADAMS,JAMES
   language: el
   title: Η ΕΠΟΠΟΙΙΑ ΤΗΣ ΑΜΕΡΙΚΗΣ
   dewey: 970 ADA
   entry_numbers:
   - '433'
   editor: ΑΕΤΟΣ // ΑΘΗΝΑ
   edition_year: 1952
@@ -65407,15 +65361,15 @@
   language: el
   title: ΠΑΡΓΑ
   subtitle: ΤΟΠΙΑ ΚΑΙ ΟΜΟΡΦΙΕΣ ΕΚΚΛΗΣΙΕΣ ΚΑΙ ΚΕΙΜΗΛΙΑ ΕΞΟΔΟΣ ΚΑΙ ΘΡΥΛΟΣ
   dewey: 938.938 ΤΣΑ
   entry_numbers:
   - '2737'
   - '3666'
-  - 9264Α
+  - 09264
   editor: None // ΑΘΗΝΑ
   edition_year: 1966
   pages: 32
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΠΑΡΓΑ
   - ΗΠΕΙΡΟΣ
@@ -65425,15 +65379,15 @@
   offprint: false
   original_entry:
     0: 1258
     1: ΤΣΑΚΑΣ,ΝΙΚΟΛΑΟΣ
     2: ΠΑΡΓΑ
     3: ΤΟΠΙΑ ΚΑΙ ΟΜΟΡΦΙΕΣ ΕΚΚΛΗΣΙΕΣ ΚΑΙ ΚΕΙΜΗΛΙΑ ΕΞΟΔΟΣ ΚΑΙ ΘΡΥΛΟΣ
     4: 938.938ΤΣΑ
-    5: 2737-3666-9264Α
+    5: 2737-3666-09264
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1966'
     11: 32Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΑΡΓΑ
     13: ΠΑΡΓΑ-ΙΣΤΟΡΙΑ
     14: ΗΠΕΙΡΟΣ-ΠΑΡΓΑ
@@ -66172,15 +66126,15 @@
   - ΤΣΑΤΣΟΥ,ΙΩΑΝΝΑ
   language: el
   title: Η ΠΟΙΗΣΗ ΚΑΙ Ο ΑΔΗΣ
   subtitle: Ο RIERRE EMMANYEL KAI H ELLADA
   dewey: 889.09 ΤΣΑ
   entry_numbers:
   - '2611'
-  - '1612'
+  - '2612'
   editor: None // ΑΘΗΝΑ
   edition_year: 1987
   pages: 65
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΠΟΙΗΣΗ
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -66190,15 +66144,15 @@
   offprint: false
   original_entry:
     0: 1273
     1: ΤΣΑΤΣΟΥ,ΙΩΑΝΝΑ
     2: Η ΠΟΙΗΣΗ ΚΑΙ Ο ΑΔΗΣ
     3: Ο RIERRE EMMANYEL KAI H ELLADA
     4: 889.09ΤΣΑ
-    5: 2611-1612
+    5: 2611-2612
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1987'
     11: 65Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
     13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΑΔΗΣ
     6: null
@@ -67754,17 +67708,14 @@
   title: ΔΟΚΙΜΙΟΝ ΙΣΤΟΡΙΚΟΝ ΠΕΡΙ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΕΩΣ
   dewey: 938.501 ΦΙΛ
   entry_numbers:
   - '1823'
   - '1824'
   - '1825'
   - '1826'
-  - '1747'
-  - '1746'
-  - '1745'
   editor: None // ΑΘΗΝΑ
   edition_year: 1859
   pages: 416
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΕΠΑΝΑΣΤΑΣΗ
   - ΔΟΚΙΜΙΟ
@@ -67773,25 +67724,25 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1304
     1: ΦΙΛΗΜΟΝΟΣ,ΙΩΑΝΝΗΣ
     2: ΔΟΚΙΜΙΟΝ ΙΣΤΟΡΙΚΟΝ ΠΕΡΙ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΕΩΣ
     4: 938.501ΦΙΛ
-    5: 1823-1824-1825-1826-
-    6: 1747-1746-1745-
+    5: 1823-1824-1825-1826
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1859'
     11: 416Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΑΝΑΣΤΑΣΗ
     13: ΕΠΑΝΑΣΤΑΣΗ-ΔΟΚΙΜΙΟ
     14: ΔΟΚΙΜΙΟ-ΕΠΑΝΑΣΤΑΣΗ
     15: 1821-ΕΠΑΝΑΣΤΑΣΗ
     3: null
+    6: null
     7: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -69086,15 +69037,15 @@
   language: el
   title: ΣΠΥΡΙΔΩΝ ΛΑΜΠΡΟΣ
   subtitle: ΜΝΗΜΟΣΥΝΟΣ ΛΟΓΟΣ
   dewey: 938 ΦΩΤ
   entry_numbers:
   - '2023'
   - '2733'
-  - 9254Α
+  - 09254
   edition: '2'
   editor: None // ΑΘΗΝΑ
   edition_year: 1967
   pages: 35
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΠΡΟΣΩΠΑ
@@ -69106,15 +69057,15 @@
   offprint: false
   original_entry:
     0: 1330
     1: ΦΩΤΙΑΔΗΣ,ΕΥΑΓΓΕΛΟΣ Π.
     2: ΣΠΥΡΙΔΩΝ ΛΑΜΠΡΟΣ
     3: ΜΝΗΜΟΣΥΝΟΣ ΛΟΓΟΣ
     4: 938ΦΩΤ
-    5: 2023-2733-9254Α
+    5: 2023-2733-09254
     7: 2ΕΚΔ
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1967'
     11: 35Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
     13: ΛΑΜΠΡΟΣ-ΙΣΤΟΡΙΑ
@@ -69414,15 +69365,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1336
     1: ΧΑΜΜΕΡ,Ι
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΟΘΩΜΑΝΙΚΗΣ ΑΥΤΟΚΡΑΤΟΡΙΑΣ
     4: 956.1ΧΑΜ
-    5: 2302-2303-2304-2305-
+    5: 2302-2303-2304-2305
     6: ΚΡ0ΚΙΔΑΣ,Κ
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1870'
     11: 385Σ
     12: ΟΘΩΜΑΝΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ-ΙΣΤΟΡΙΑ
     13: ΤΟΥΡΚΙΑ-ΟΘΩΜΑΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -70900,14 +70851,15 @@
     28: null
     29: null
 - dbase_number: 1365
   authors:
   - ΧΟΦΜΑΝ,ΦΡΕΝΤ
   language: el
   title: ΤΟ ΣΥΓΧΡΟΝΟ ΑΜΕΡΙΚΑΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ(1900-1950)
+  dewey: 880.03 ΧΟΦ
   entry_numbers:
   - '2655'
   editor: ΑΕΤΟΣ // ΑΘΗΝΑ
   edition_year: 1954
   pages: 167
   topics:
   - ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -70917,15 +70869,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1365
     1: ΧΟΦΜΑΝ,ΦΡΕΝΤ
     2: ΤΟ ΣΥΓΧΡΟΝΟ ΑΜΕΡΙΚΑΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ(1900-1950)
-    4: 880.ΧΟΦ
+    4: 880.03ΧΟΦ
     5: '2655'
     8: ΑΕΤΟΣ
     9: ΑΘΗΝΑ
     10: '1954'
     11: 167Σ
     12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΑΜΕΡΙΚΑΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ-ΙΣΤΟΡΙΑ
@@ -71513,15 +71465,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1377
   authors:
-  - WOODHOYSE,C
+  - WOODHOUSE,CRISTOPHER,MONTAGUE
   title: CAPODISTRIA
   subtitle: THE FOYHDER OF GREEK INDEPEHDENCE
   dewey: 938.571 WOO
   entry_numbers:
   - '1785'
   editor: None // NEW YORK
   edition_year: 1973
@@ -71614,15 +71566,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1379
   authors:
-  - WILDER THORNTON
+  - WILDER,THORNTON
   language: el
   title: Η ΜΙΚΡΗ ΜΑΣ ΠΟΛΗ
   dewey: 812.54 WIL
   entry_numbers:
   - '1395'
   translators:
   - ΒΟΛΑΝΑΚΗΣ,Μ.
@@ -72327,15 +72279,14 @@
   language: el
   title: Η ΕΚΣΤΡΑΤΕΙΑ ΕΙΣ ΤΗΝ ΜΙΚΡΑΝ ΑΣΙΑΝ(1919-1922)
   subtitle: ΕΠΙΘΕΤΙΚΑΙ ΕΠΙΧΕΙΡΗΣΕΙΣ ΔΕΚΕΜΒΡΙΟΥ 1920 ΜΑΡΤΙΟΥ 1921
   dewey: 938.721 ΧΣ
   entry_numbers:
   - '1793'
   - '1873'
-  - '8192'
   editor: ΓΕΝ.ΕΠΙΤ.ΣΤΡΑΤΟΥ // ΑΘΗΝΑ
   edition_year: 1963
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΜΙΚΡΑ ΑΣΙΑ
   - ΕΚΣΤΡΑΤΕΙΑ
   - '1919'
@@ -72346,15 +72297,15 @@
   offprint: false
   original_entry:
     0: 1393
     1: Χ.Σ
     2: Η ΕΚΣΤΡΑΤΕΙΑ ΕΙΣ ΤΗΝ ΜΙΚΡΑΝ ΑΣΙΑΝ(1919-1922)
     3: ΕΠΙΘΕΤΙΚΑΙ ΕΠΙΧΕΙΡΗΣΕΙΣ ΔΕΚΕΜΒΡΙΟΥ 1920 ΜΑΡΤΙΟΥ 1921
     4: 938.721Χ.Σ
-    5: 1793-1873-8192
+    5: 1793-1873
     8: ΓΕΝ.ΕΠΙΤ.ΣΤΡΑΤΟΥ
     9: ΑΘΗΝΑ
     10: '1963'
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΙΚΡΑ ΑΣΙΑ
     13: ΜΙΚΡΑ ΑΣΙΑ-ΕΚΣΤΡΑΤΕΙΑ
     14: 1919-ΜΙΚΡΑ ΑΣΙΑ
     15: ΓΕΝΙΚΟ ΕΠΙΤΕΛΕΙΟ ΣΤΡΑΤΟΥ
@@ -73185,15 +73136,14 @@
     30: null
 - dbase_number: 1410
   authors: []
   language: el
   title: ΕΠΙΤΟΜΟΣ ΙΣΤΟΡΙΑ ΤΗΣ ΕΙΣ ΜΙΚΡΑΝ ΑΣΙΑΝ ΕΚΣΤΡΑΤΕΙΑΣ (1919-1922
   dewey: 938.721 ΧΣ
   entry_numbers:
-  - '1793'
   - '8192'
   editor: None // ΑΘΗΝΑ
   edition_year: 1967
   pages: 495
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΜΙΚΡΑ ΑΣΙΑ
@@ -73203,15 +73153,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1410
     1: Χ.Σ
     2: ΕΠΙΤΟΜΟΣ ΙΣΤΟΡΙΑ ΤΗΣ ΕΙΣ ΜΙΚΡΑΝ ΑΣΙΑΝ ΕΚΣΤΡΑΤΕΙΑΣ (1919-1922
     4: 938.721Χ.Σ
-    5: 1793-8192
+    5: '8192'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1967'
     11: 495Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΙΚΡΑ ΑΣΙΑ
     13: ΜΙΚΡΑ ΑΣΙΑ-1919
     14: 1919-ΜΙΚΡΑ ΑΣΙΑ
@@ -73681,30 +73631,30 @@
     30: null
 - dbase_number: 1420
   authors: []
   language: el
   title: Η ΚΑΤΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ ΕΠΙΒΟΛΗΣ
   dewey: 938.666 ΧΣ
   entry_numbers:
-  - '1237'
+  - '2237'
   editor: None // ΑΘΗΝΑ
   edition_year: 1966
   pages: 369
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΜΑΚΕΔΟΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1420
     1: Χ.Σ
     2: Η ΚΑΤΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ ΕΠΙΒΟΛΗΣ
     4: 938.666Χ.Σ
-    5: '1237'
+    5: '2237'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1966'
     11: 369Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
     13: ΜΑΚΕΔΟΝΙΑ
     3: null
@@ -74376,29 +74326,29 @@
     30: null
 - dbase_number: 1434
   authors: []
   language: el
   title: ΤΟ ΡΟΥΜΑΝΙΚΟ ΒΙΒΛΙΟ
   dewey: 949.8 ΧΣ
   entry_numbers:
-  - '2563'
+  - '2562'
   editor: None // ΑΘΗΝΑ
   pages: 133
   topics:
   - ΡΟΥΜΑΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΡΟΥΜΑΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1434
     1: Χ.Σ
     2: ΤΟ ΡΟΥΜΑΝΙΚΟ ΒΙΒΛΙΟ
     4: 949.8Χ.Σ
-    5: '2563'
+    5: '2562'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: Χ.Τ
     11: 133Σ
     12: ΡΟΥΜΑΝΙΚΗ ΙΣΤΟΡΙΑ
     13: ΡΟΥΜΑΝΙΑ-ΙΣΤΟΡΙΑ
     3: null
@@ -76038,16 +75988,16 @@
     30: null
 - dbase_number: 1467
   authors: []
   language: el
   title: ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ 65
   dewey: 880.203 ΚΙΝ
   entry_numbers:
+  - '1603'
   - '1604'
-  - '1605'
   editor: None // ΑΘΗΝΑ
   edition_year: 1965
   pages: 31
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
   - ΕΛΛΗΝΙΚΟΣ ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
@@ -76056,15 +76006,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1467
     1: Χ.Σ
     2: ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ 65
     4: 880.203ΚΙΝ
-    5: 1604-1605-
+    5: 1603-1604
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1965'
     11: 31Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
     13: ΕΛΛΗΝΙΚΟΣ ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΠΕΡΙΟΔΙΚΟ
     14: ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΠΕΡΙΟΔΙΚΟ
@@ -76847,15 +76797,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1483
   authors:
-  - ΒΟΚΟΤΟΠΟΥΛΟΣ,Π
+  - ΒΟΚΟΤΟΠΟΥΛΟΣ,ΠΑΝΑΓΙΩΤΗΣ
   language: el
   title: ΜΕΣΑΙΩΝΙΚΑ ΜΝΗΜΕΙΑ ΝΟΜΟΥ ΑΡΤΗΣ 1966
   dewey: 938.939 ΒΟΚ
   entry_numbers:
   - '278'
   editor: None // ΑΘΗΝΑ
   edition_year: 1969
@@ -76897,15 +76847,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1484
   authors:
-  - ΒΟΚΟΤΟΠΟΥΛΟΣ,ΠΑΝ
+  - ΒΟΚΟΤΟΠΟΥΛΟΣ,ΠΑΝΑΓΙΩΤΗΣ
   language: el
   title: ΠΑΡΑΤΗΡΗΣΕΙΣ ΕΠΙ ΤΗΣ ΠΑΝΑΓΙΑΣ ΤΟΥ ΜΠΡΥΩΝΗ
   dewey: 938.939 ΒΟΚ
   entry_numbers:
   - '264'
   editor: None // ΑΘΗΝΑ
   edition_year: 1975
@@ -76947,15 +76897,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1485
   authors:
-  - ΑΧΕΙΜΑΣΤΟΥ-ΠΟΤΑΜΙΑΝΟΥ,Μ
+  - ΑΧΕΙΜΑΣΤΟΥ-ΠΟΤΑΜΙΑΝΟΥ,ΜΥΡΤΑΛΗ
   language: el
   title: ΦΟΡΗΤΗ ΕΙΚΩΝ ΤΩΝ ΑΓΙΟΥ ΣΥΜΕΩΝ ΤΟΥ ΣΤΥΛΙΤΟΥ ΕΚ ΚΟΡΥΤΙΑΝΗΣ ΕΙΣ
   subtitle: ΤΟ ΜΟΥΣΕΙΟΝ ΤΩΝ ΙΩΑΝΝΙΝΩΝ
   dewey: 938.936 ΑΧΕ
   entry_numbers:
   - '459'
   editor: None // ΑΘΗΝΑ
@@ -77413,15 +77363,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1494
   authors:
-  - ΒΑΒΑΡΕΤΟΣ,ΓΕΩΡΓΙΟΣ
+  - ΒΑΒΑΡΕΤΟΣ,ΓΕΩΡΓΙΟΣ,ΑΧΙΛ.
   language: el
   title: ΙΩΑΝΝΗΣ ΒΗΛΑΡΑΣ
   dewey: 880.2 ΒΑΒ
   entry_numbers:
   - '1033'
   - '1022'
   - '2833'
@@ -77567,15 +77517,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1497
   authors:
-  - ΒΑΚΑΛΗΣ,ΔΗΜΗΤΡ
+  - ΒΑΚΑΛΗΣ,ΔΗΜΗΤΡΗΣ
   language: el
   title: Η ΚΑΘΟΔΟΣ ΤΩΝ ΒΟΡΕΙΩΝ ΗΠΕΙΡΩΤΩΝ ΚΑΙ ΤΟ ΕΘΝΙΚΟΝ ΧΡΕΟΣ
   subtitle: ΤΩΝ ΣΗΜΕΡΙΝΩΝ ΕΛΛΗΝΩΝ
   dewey: 938.694 ΒΑΚ
   entry_numbers:
   - '1652'
   editor: None // ΙΩΑΝΝΙΝΑ
@@ -77629,18 +77579,14 @@
   title: ΒΥΖΑΝΤΙΝΩΝ ΒΙΟΣ ΚΑΙ ΠΟΛΙΤΙΣΜΟΣ
   dewey: 938.303 ΚΟΥ
   entry_numbers:
   - '2749'
   - '2750'
   - '2751'
   - '2752'
-  - '2756'
-  - '2753'
-  - '2754'
-  - '2755'
   editor: None // ΑΘΗΝΑ
   edition_year: 1948
   pages: 224
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΒΥΖΑΝΤΙΟ
   - ΠΟΛΙΤΙΣΜΟΣ
@@ -77650,24 +77596,24 @@
   offprint: false
   original_entry:
     0: 1498
     1: ΚΟΥΚΟΥΛΕ,ΦΑΙΔΩΝΑΣ
     2: ΒΥΖΑΝΤΙΝΩΝ ΒΙΟΣ ΚΑΙ ΠΟΛΙΤΙΣΜΟΣ
     4: 938.303ΚΟΥ
     5: 2749-2750-2751-2752-
-    6: 2756-2753-2754-2755
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1948'
     11: 224Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΥΝΑΝΤΙΟ
     13: ΒΥΖΑΝΤΙΟ-ΠΟΛΙΤΙΣΜΟΣ
     14: ΠΟΛΙΤΙΣΜΟΣ-ΒΥΖΑΝΤΙΟ
     17: 8 ΑΝΤΙΤΥΠΑ
     3: null
+    6: null
     7: null
     15: null
     16: null
     18: null
     19: null
     20: null
     21: null
@@ -77877,15 +77823,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1503
   authors:
-  - ΒΙΤΤΙ,ΜΑΡΙΟ
+  - VITTI,MARIO
   language: el
   title: Η ΓΕΝΙΑ ΤΟΥ ΤΡΙΑΝΤΑ ΙΔΕΟΛΟΓΙΑ
   dewey: 889.09 ΒΙΤ
   entry_numbers:
   - '2822'
   editor: ΕΡΜΗΣ // ΑΘΗΝΑ
   edition_year: 1979
@@ -78393,15 +78339,15 @@
   authors:
   - ΣΚΟΠΑΣ,ΝΙΚ.Α-ΧΑΡΑΜΟΠΟΥΛΟΣ,Λ.Χ
   language: el
   title: Ο ΑΓΩΝΑΣ ΤΩΝ 16 ΧΩΡΙΩΝ ΤΗΣ ΕΠΑΡΧΙΑΣ ΦΙΛΙΑΤΩΝ
   subtitle: ΕΝΑ ΑΓΡΟΤΙΚΟ ΞΕΣΗΚΩΜΑ (1858-1930)
   dewey: 938.937 ΣΚΟ
   entry_numbers:
-  - '2842'
+  - '2841'
   editor: None // ΑΘΗΝΑ
   pages: 249
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΗΠΕΙΡΟΣ
   - ΦΙΛΙΑΤΕΣ
   - ΑΓΡΟΤΙΚΟ ΞΕΣΗΚΩΜΑ
@@ -78410,15 +78356,15 @@
   offprint: false
   original_entry:
     0: 1513
     1: ΣΚΟΠΑΣ,ΝΙΚ.Α-ΧΑΡΑΜΟΠΟΥΛΟΣ,Λ.Χ
     2: Ο ΑΓΩΝΑΣ ΤΩΝ 16 ΧΩΡΙΩΝ ΤΗΣ ΕΠΑΡΧΙΑΣ ΦΙΛΙΑΤΩΝ
     3: ΕΝΑ ΑΓΡΟΤΙΚΟ ΞΕΣΗΚΩΜΑ (1858-1930)
     4: 938.937ΣΚΟ
-    5: '2842'
+    5: '2841'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 249Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΦΙΛΙΑΤΕΣ
     14: ΦΙΛΙΑΤΕΣ-ΑΓΡΟΤΙΚΟ ΞΕΣΗΚΩΜΑ
@@ -79101,15 +79047,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1527
   authors:
-  - ΒΑΒΑΡΕΤΟΣ,ΓΕΩΡΓΙΟΣ ΑΧ
+  - ΒΑΒΑΡΕΤΟΣ,ΓΕΩΡΓΙΟΣ,ΑΧΙΛ.
   language: el
   title: ΚΟΜΠΟΓΙΑΝΝΙΤΕΣ,ΜΑΤΣΟΥΚΑΔΕΣ
   subtitle: ΟΙ ΞΑΚΟΥΣΜΕΝΟΙ ΑΥΤΟΔΙΔΑΚΤΟΙ ΓΙΑΤΡΟΙ
   dewey: 938.936 ΒΑΒ
   entry_numbers:
   - '2824'
   - '2825'
@@ -79416,15 +79362,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1533
   authors:
-  - ΒΡΑΝΟΥΣΗΣ,Λ
+  - ΒΡΑΝΟΥΣΗΣ,ΛΕΑΝΔΡΟΣ,Ι.
   language: el
   title: ΡΗΓΑΣ
   subtitle: ΒΕΛΕΣΤΙΝΛΗΣ-ΦΕΡΑΙΟΣ
   dewey: 938.483 ΒΡΑ
   entry_numbers:
   - '2860'
   editor: None // ΑΘΗΝΑ
@@ -79468,15 +79414,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1534
   authors:
-  - ΒΡΑΝΟΥΣΗΣ,Λ.Ι.
+  - ΒΡΑΝΟΥΣΗΣ,ΛΕΑΝΔΡΟΣ,Ι.
   language: el
   title: ΤΟ ΧΡΟΝΙΚΟΝ ΤΩΝ ΙΩΑΝΝΙΝΩΝ ΚΑΤ'ΑΝΕΚΔΟΤΟΝ ΔΗΜΩΔΗ ΕΠΙΤΟΜΗΝ
   dewey: 938.936 ΒΡΑ
   entry_numbers:
   - '2881'
   editor: None // ΑΘΗΝΑ
   edition_year: 1965
@@ -79518,15 +79464,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1535
   authors:
-  - ΒΡΑΝΟΥΣΗΣ,Λ
+  - ΒΡΑΝΟΥΣΗΣ,ΛΕΑΝΔΡΟΣ,Ι.
   language: el
   title: Η ΣΗΜΑΙΑ ΤΟ ΕΘΝΟΣΗΜΟ ΚΑΙ Η ΣΦΡΑΓΙΔΑ ΤΗΣ
   subtitle: '"ΕΛΛΗΝΙΚΗΣ ΔΗΜΟΚΡΑΤΙΑΣ" ΤΟΥ ΡΗΓΑ'
   dewey: 938.483 ΒΡΑ
   entry_numbers:
   - '2878'
   editor: None // ΑΘΗΝΑ
@@ -79669,15 +79615,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1538
   authors:
-  - ΑΛΑΜΑΓΚΑΣ,Δ
+  - ΣΑΛΑΜΑΓΚΑΣ,ΔΗΜΗΤΡΙΟΣ
   language: el
   title: ΓΙΑΝΝΙΩΤΙΚΑ ΙΣΤΟΡΙΟΔΙΦΙΚΑ ΜΕΛΕΤΗΜΑΤΑ
   dewey: 938.936 ΣΑΛ
   entry_numbers:
   - '2865'
   editor: None // ΙΩΑΝΝΙΝΑ
   edition_year: 1958
@@ -80131,15 +80077,14 @@
   authors:
   - ΛΟΥΚΑΤΟΣ,ΔΗΜΗΤΡΙΟΣ Σ
   language: el
   title: Ο ΠΑΡΟΙΜΙΑΚΟΣ ΛΟΓΟΣ ΤΩΝ ΗΠΕΙΡΩΤΩΝ
   dewey: 938.93 ΛΟΥ
   entry_numbers:
   - '2768'
-  - '2887'
   editor: ΑΘΗΝΑ // None
   edition_year: 1976
   pages: 36
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΗΠΕΙΡΟΣ
   - ΠΑΡΟΙΜΙΑΚΟΣ ΛΟΓΟΣ
@@ -80149,15 +80094,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1547
     1: ΛΟΥΚΑΤΟΣ,ΔΗΜΗΤΡΙΟΣ Σ
     2: Ο ΠΑΡΟΙΜΙΑΚΟΣ ΛΟΓΟΣ ΤΩΝ ΗΠΕΙΡΩΤΩΝ
     4: 938.93ΛΟΥ
-    5: 2768-2887
+    5: '2768'
     8: ΑΘΗΝΑ
     9: Χ.Ε
     10: '1976'
     11: 36Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
     13: ΗΠΕΙΡΟΣ-ΠΑΡΟΙΜΙΑΚΟΣ ΛΟΓΟΣ
     14: ΠΑΡΟΙΜΙΕΣ-ΗΠΕΙΡΟΣ
@@ -80855,15 +80800,15 @@
   authors: []
   language: el
   title: ΣΠΥΡΙΔΩΝ ΒΛΑΧΟΣ
   subtitle: Α ΑΠΟ ΙΩΑΝΝΙΝΩΝ ΑΡΧΙΕΠΙΣΚΟΠΟΣ ΑΘΗΝΩΝ ΚΑΙ ΠΑΣΗΣ ΕΛΛΑΔΟΣ
   dewey: 938.936 ΣΠΥ
   entry_numbers:
   - '2783'
-  - 9255Α
+  - 09255
   editor: None // ΑΘΗΝΑ
   edition_year: 1970
   pages: 51
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΙΩΑΝΝΙΝΑ
   - ΑΡΧΙΕΠΙΣΚΟΠΟΣ
@@ -80877,15 +80822,15 @@
   offprint: false
   original_entry:
     0: 1561
     1: Χ.Σ
     2: ΣΠΥΡΙΔΩΝ ΒΛΑΧΟΣ
     3: Α ΑΠΟ ΙΩΑΝΝΙΝΩΝ ΑΡΧΙΕΠΙΣΚΟΠΟΣ ΑΘΗΝΩΝ ΚΑΙ ΠΑΣΗΣ ΕΛΛΑΔΟΣ
     4: 938.936ΣΠΥ
-    5: 2783-9255Α
+    5: 2783-09255
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1970'
     11: 51Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΙΩΑΝΝΙΝΑ
     13: ΙΩΑΝΝΙΝΑ-ΑΡΧΙΕΠΙΣΚΟΠΟΣ
     14: ΒΛΑΧΟΣ-ΑΡΧΙΕΠΙΣΚΟΠΟΣ
@@ -81166,15 +81111,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1567
   authors:
-  - ΒΑΒΑΡΕΤΟΣ,ΓΕΩΡΓΙΟΣ ΑΧ
+  - ΒΑΒΑΡΕΤΟΣ,ΓΕΩΡΓΙΟΣ,ΑΧΙΛ.
   language: el
   title: ΓΕΩΡΓΙΟΣ ΧΑΤΖΗΣ-ΠΕΛΛΕΡΕΝ
   subtitle: Ο ΗΠΕΙΡΩΤΗΣ ΑΓΩΝΙΣΤΗΣ,Ο ΔΗΜΟΣΙΟΓΡΑΦΟΣ,Ο ΠΟΙΗΤΗΣ
   dewey: 938.93 ΒΑΒ
   entry_numbers:
   - '2773'
   editor: None // ΑΘΗΝΑ
@@ -81387,19 +81332,16 @@
 - dbase_number: 1571
   authors:
   - ΜΟΣΧΟΠΟΥΛΟΣ,ΙΩΑΝΝΗΣ ΝΙΚ
   language: el
   title: ΠΑΝΣΛΑΥΙΣΜΟΣ ΚΑΙ ΕΛΛΗΝΙΣΜΟΣ
   dewey: 938.05 ΣΦΑ
   entry_numbers:
-  - '2742'
-  - '2743'
-  - '2744'
-  - '2746'
   - '2745'
+  - '2746'
   editor: None // ΑΘΗΝΑ
   edition_year: 1978
   pages: 66
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΠΑΝΣΛΑΥΙΣΜΟΣ
   - ΕΛΛΗΝΙΣΜΟΣ
@@ -81408,25 +81350,25 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1571
     1: ΜΟΣΧΟΠΟΥΛΟΣ,ΙΩΑΝΝΗΣ ΝΙΚ
     2: ΠΑΝΣΛΑΥΙΣΜΟΣ ΚΑΙ ΕΛΛΗΝΙΣΜΟΣ
     4: 938.05ΣΦΑ
-    5: 2742-2743-2744-2746-
-    6: '2745'
+    5: 2745-2746
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1978'
     11: 66Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΑΝΣΛΑΙΣΜΟΣ
     13: ΠΑΝΣΛΑΙΣΜΟΣ-ΕΛΛΗΝΙΣΜΟΣ
     14: ΕΛΛΗΝΙΣΜΟΣ-ΠΑΝΣΛΑΥΙΣΜΟΣ
     21: ΙΩΑΝΝΗΣ ΚΑΠΟΔΙΣΤΡΙΑΣ;5
     3: null
+    6: null
     7: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
@@ -81606,15 +81548,15 @@
   - ΛΑΜΠΡΙΔΗΣ,ΣΤΑΘΗΣ Δ
   language: el
   title: ΙΩΑΝΝΗΣ ΛΑΜΠΡΙΔΗΣ
   dewey: 938.936 ΛΑΜ
   entry_numbers:
   - '2826'
   - '3693'
-  - 9265Α
+  - 09265
   editor: None // ΑΘΗΝΑ
   edition_year: 1979
   pages: 67
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΖΑΓΟΡΙ
   - ΛΑΜΠΡΙΔΗΣ
@@ -81624,15 +81566,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1575
     1: ΛΑΜΠΡΙΔΗΣ,ΣΤΑΘΗΣ Δ
     2: ΙΩΑΝΝΗΣ ΛΑΜΠΡΙΔΗΣ
     4: 938.936ΛΑΜ
-    5: 2826-3693-9265Α
+    5: 2826-3693-09265
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: '1979'
     11: 67Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΖΑΓΟΡΙ
     13: ΖΑΓΟΡΙ-ΛΑΜΠΡΙΔΗΣ
     14: ΛΑΜΠΡΙΔΗΣ-ΓΙΑΤΡΟΣ
@@ -82271,15 +82213,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1588
   authors:
-  - ΒΑΣΙΛΑΚΗΣ,ΚΩΝ/ΝΟΣ
+  - ΒΑΣΙΛΑΚΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΠΛΑΤΩΝΙΚΑΙ ΕΡΕΥΝΑΙ
   subtitle: Ο ΠΛΑΤΩΝ ΚΑΙ Η ΕΠΟΠΤΙΚΗ ΔΙΔΑΣΚΑΛΙΑ
   dewey: 184.1 ΒΑΣ
   entry_numbers:
   - '2912'
   editor: None // ΑΘΗΝΑ
@@ -82831,15 +82773,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1599
   authors:
-  - ΑΡΙΣΤΟΤΕΛΕΙΟ ΠΑΝΕΠΙΣΤΗΜΙΟ ΘΕΣ/ΝΙΚΗΣ
+  - ΑΡΙΣΤΟΤΕΛΕΙΟ ΠΑΝΕΠΙΣΤΗΜΙΟ ΘΕΣΣΑΛΟΝΙΚΗΣ
   language: el
   title: ΜΕΚΕΔΟΝΙΑ
   subtitle: ΤΟ ΙΣΟΤΡΙΚΟ ΠΡΟΣΩΠΟ ΤΟΥ ΒΟΡΡΑ
   dewey: 938.666 ΧΣ
   entry_numbers:
   - '10640'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -82931,15 +82873,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1601
   authors:
-  - ΑΝΑΣΤΑΣΙΑΔΟΣ,ΗΛΙΑΣ Κ
+  - ΑΝΑΣΤΑΣΙΑΔΗΣ,ΗΛΙΑΣ,Κ.
   language: el
   title: ΝΟΜΙΚΑ ΦΙΛΟΣΟΦΗΜΑΤΑ
   dewey: 107 ΑΝΑ
   entry_numbers:
   - '258'
   editor: None // ΑΘΗΝΑ
   edition_year: 1927
@@ -83868,15 +83810,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1619
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.Α
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: ΕΦΗΒΕΙΑ
   subtitle: ΑΠΟ ΤΑ ΨΥΧΟΛΟΓΙΚΑ ΠΡΟΒΛΗΜΑΤΑ ΤΟΥ ΚΟΡΙΤΣΙΟΥ
   dewey: 136.73 ΑΣΠ
   entry_numbers:
   - '2986'
   editor: None // ΑΘΗΝΑ
@@ -83922,15 +83864,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1620
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.Α
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: ΤΟ ΚΟΡΙΤΣΙ ΚΑΙ Η ΚΟΙΝΩΝΙΑ
   subtitle: ΑΠΟ ΤΑ ΨΥΧΟΛΟΓΙΚΑ ΠΡΟΒΛΗΜΑΤΑΤΟΥ ΚΟΡΙΤΣΙΟΥ
   dewey: 136.73 ΑΣΠ
   entry_numbers:
   - '3000'
   editor: None // ΑΘΗΝΑ
@@ -83976,15 +83918,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1621
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.Α
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: Η ΕΠΑΓΓΕΛΜΑΤΙΚΗ ΖΩΗ ΤΟΥ ΚΟΡΙΤΣΙΟΥ
   subtitle: ΑΠΟ ΤΑ ΨΥΧΟΛΟΓΙΚΑ ΠΡΟΒΛΗΜΑΤΑ ΤΟΥ ΚΟΡΙΤΣΙΟΥ
   dewey: 150.1 ΑΣΠ
   entry_numbers:
   - '3001'
   editor: None // ΑΘΗΝΑ
@@ -84029,15 +83971,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1622
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.Α
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: Η ΨΥΧΙΚΗ ΩΡΙΜΟΤΗΣ ΤΟΥ ΑΝΘΡΩΠΟΥ
   dewey: 136.5 ΑΣΠ
   entry_numbers:
   - '3002'
   editor: None // ΑΘΗΝΑ
   edition_year: 1959
@@ -84081,15 +84023,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1623
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.Α
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: ΤΟ ΠΑΙΔΙ ΚΑΙ Η ΠΕΙΘΑΡΧΙΑ
   subtitle: ΑΠΟ ΤΑ ΨΥΧΟΛΟΓΙΚΑ ΠΡΟΒΛΗΜΑΤΑ ΤΟΥ ΠΑΙΔΙΟΥ
   dewey: 136 ΑΣΠ
   entry_numbers:
   - '3003'
   editor: None // ΑΘΗΝΑ
@@ -84134,15 +84076,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1624
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.Α
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: ΤΟ ΠΑΙΔΙ ΚΑΙ Ο ΨΥΧΙΚΟΣ ΤΟΥ ΚΟΣΜΟΣ
   subtitle: ΑΠΟ ΤΑ ΨΥΧΟΛΟΓΙΚΑ ΠΡΟΒΛΗΜΑΤΑ ΤΟΥ ΠΑΙΔΙΟΥ
   dewey: 136 ΑΣΠ
   entry_numbers:
   - '3004'
   editor: None // ΑΘΗΝΑ
@@ -84187,15 +84129,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1625
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.Α
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: ΑΠΟ ΤΗΝ ΣΦΑΙΡΑΝ ΤΟΥ ΑΡΡΩΣΤΟΥ ΨΥΧΙΚΟΥ ΟΡΓΑΝΙΣΜΟΥ
   subtitle: ΕΙΣΑΓΩΓΗ ΕΙΣ ΤΗΝ ΣΠΟΥΔΗΝ ΤΗΣ ΣΥΓΧΡΟΝΟΥ ΑΝΘΡΩΠΟΛΟΓΙΑ
   dewey: 131.3 ΑΣΠ
   entry_numbers:
   - '2988'
   editor: None // ΑΘΗΝΑ
@@ -84240,15 +84182,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1626
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.Α
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: ΘΕΜΑΤΑ ΤΗΣ ΣΗΜΕΡΙΝΗΣ ΨΥΧΟΛΟΓΙΑΣ
   subtitle: ΕΙΣΑΓΩΓΗ ΕΙΣ ΤΗΝ ΣΠΟΥΔΗΝ ΤΗΣ ΣΥΓΧΡΟΝΟΥ ΑΝΘΡΩΠΟΛΟΓΙΑΣ
   dewey: 150 ΑΣΠ
   entry_numbers:
   - '2989'
   editor: None // ΑΘΗΝΑ
@@ -84293,15 +84235,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1627
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.Α
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: ΠΡΟΣ ΟΛΟΚΛΗΡΩΣΙΝ ΤΗΣ ΠΡΟΣΩΠΙΚΟΤΗΤΟΣ
   subtitle: ΕΙΣΑΓΩΓΗ ΕΙΣ ΤΗΝ ΣΠΟΥΔΗΝ ΤΗΣ ΣΥΧΡΟΝΟΥ ΑΝΘΡΩΠΟΛΟΓΙΑΣ
   dewey: 126 ΑΣΠ
   entry_numbers:
   - '2990'
   editor: None // ΑΘΗΝΑ
@@ -84347,15 +84289,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1628
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.Α
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: Η ΕΦΗΒΟΣ ΚΟΡΗ ΚΑΙ ΤΟ ΟΙΚΟΓΕΝΕΙΑΚΟΝ ΠΕΡΙΒΑΛΛΟΝ
   subtitle: ΑΠΟ ΤΑ ΨΥΧΟΛΟΓΙΚΑ ΠΡΟΒΛΗΜΑΤΑ ΤΟΥ ΚΟΡΙΤΣΙΟΥ
   dewey: 136.73 ΑΣΠ
   entry_numbers:
   - '2991'
   editor: None // ΑΘΗΝΑ
@@ -84401,15 +84343,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1629
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.Α
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: Η ΣΥΝΑΝΤΗΣΙΣ ΜΕ ΤΟ ΑΛΛΟ ΦΥΛΟΝ
   subtitle: ΑΠΟ ΤΑ ΨΥΧΟΛΟΓΙΚΑ ΠΡΟΒΛΗΜΑΤΑ ΤΟΥ ΚΟΡΙΤΣΙΟΥ
   dewey: 136.73 ΑΣΠ
   entry_numbers:
   - '2993'
   editor: None // ΑΘΗΝΑ
@@ -84455,15 +84397,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1630
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.Α
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: Η ΓΥΝΑΙΚΑΙ ΚΑΙ Ο ΨΥΧΙΚΟΣ ΤΗΣ ΚΟΣΜΟΣ
   dewey: 137 ΑΣΠ
   entry_numbers:
   - '2968'
   editor: None // ΑΘΗΝΑ
   edition_year: 1953
@@ -84507,15 +84449,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1631
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.Α
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: Ο ΕΠΑΓΓΕΛΜΑΤΙΚΟΣ ΠΡΟΣΑΝΑΤΟΛΙΣΜΟΣ
   subtitle: ΑΠΟ ΤΑ ΨΥΧΟΛΟΓΙΚΑ ΠΡΟΒΛΗΜΑΤΑ ΤΟΥ ΕΦΗΒΟΥ
   dewey: 150.1 ΑΣΠ
   entry_numbers:
   - '2972'
   editor: None // ΑΘΗΝΑ
@@ -84560,15 +84502,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1632
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.Α
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: Ο ΕΦΗΒΟΣ ΚΑΙ Η ΟΙΚΟΓΕΝΕΙΑ
   subtitle: ΑΠΟ ΤΑ ΨΥΧΟΛΟΓΙΚΑ ΠΡΟΒΛΗΜΑΤΑ ΤΟΥ ΕΦΗΒΟΥ
   dewey: 136.73 ΑΣΠ
   entry_numbers:
   - '2973'
   editor: None // ΑΘΗΝΑ
@@ -84614,15 +84556,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1633
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.Α
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: ΤΑ ΑΙΣΘΗΜΑΤΑ ΜΕΙΟΝΕΚΤΙΚΟΤΗΤΟΣ
   subtitle: ΑΠΟ ΤΑ ΨΥΧΟΛΟΓΙΚΑ ΠΡΟΒΛΗΜΑΤΑ ΤΟΥ ΕΦΗΒΟΥ
   dewey: 136.73 ΑΣΠ
   entry_numbers:
   - '2974'
   editor: None // ΑΘΗΝΑ
@@ -84667,15 +84609,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1634
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.Α
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: Ο ΕΦΗΒΟΣ ΚΑΙ Η ΚΟΙΝΩΝΙΑ
   subtitle: ΑΠΟ ΤΑ ΨΥΧΟΛΟΓΙΚΑ ΠΡΟΒΛΗΜΑΤΑ ΤΟΥ ΕΦΗΒΟΥ
   dewey: 136.73 ΑΣΠ
   entry_numbers:
   - '2975'
   editor: None // ΑΘΗΝΑ
@@ -84721,15 +84663,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1635
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.Α
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: Ο ΕΦΗΒΟΣ ΚΑΙ Η ΠΑΙΔΕΙΑ
   subtitle: ΑΠΟ ΤΑ ΨΥΧΟΛΟΓΙΚΑ ΠΡΟΒΛΗΜΑΤΑ ΤΟΥ ΕΦΗΒΟΥ
   dewey: 136.73 ΑΣΠ
   entry_numbers:
   - '2976'
   editor: None // ΑΘΗΝΑ
@@ -84775,15 +84717,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1636
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.Α
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: Ο ΕΦΗΒΟΣ ΚΑΙ Η ΘΡΗΣΚΕΥΤΙΚΗ ΖΩΗ
   subtitle: ΑΠΟ ΤΑ ΨΥΧΟΛΟΓΙΑ ΠΡΟΒΛΗΜΑΤΑ ΤΟΥ ΕΦΗΒΟΥ
   dewey: 136.73 ΑΣΠ
   entry_numbers:
   - '2977'
   editor: None // ΑΘΗΝΑ
@@ -84829,15 +84771,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1637
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.Α
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: Η ΥΓΕΙΑ Η ΑΣΘΕΝΕΙΑ ΚΑΙ Η ΨΥΧΗ ΤΟΥ ΕΦΗΒΟΥ
   subtitle: ΑΠΟ ΤΑ ΨΥΧΟΛΟΓΙΚΑ ΠΡΟΒΛΗΜΑΤΑ ΤΟΥ ΕΦΗΒΟΥ
   dewey: 136.73 ΑΣΠ
   entry_numbers:
   - '2979'
   editor: None // ΑΘΗΝΑ
@@ -86936,30 +86878,30 @@
 - dbase_number: 1678
   authors:
   - ΡΟΖΕΝΤΑΛ,Μ
   language: el
   title: ΦΙΛΟΣΟΦΙΚΟ ΛΕΞΙΚΟ
   dewey: 103 ΡΟΖ
   entry_numbers:
-  - '1909'
+  - '2909'
   editor: None // ΑΘΗΝΑ
   pages: 233
   topics:
   - ΠΑΓΚΟΣΜΙΑ ΦΙΛΟΣΟΦΙΑ
   - ΛΕΞΙΚΟ
   - ΦΙΛΟΣΟΦΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1678
     1: ΡΟΖΕΝΤΑΛ,Μ
     2: ΦΙΛΟΣΟΦΙΚΟ ΛΕΞΙΚΟ
-    4: 103 ΡΟΖ
-    5: '1909'
+    4: 103ΡΟΖ
+    5: '2909'
     8: Χ.Ε
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 233Σ
     12: ΠΑΓΚΟΣΜΙΑ ΦΙΛΟΣΟΦΙΑ-ΛΕΞΙΚΟ
     13: ΦΙΛΟΣΟΦΙΚΟ-ΛΕΞΙΚΟ
     14: ΛΕΞΙΚΟ-ΦΙΛΟΣΟΦΙΑ
@@ -86979,46 +86921,36 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1679
-  authors:
-  - ΓΙΟΥΝΤΙΝ,Π
-  language: el
-  title: ΦΙΛΟΣΟΦΙΚΟ ΛΕΞΙΚΟ
-  dewey: 103 ΡΟΖ
-  entry_numbers:
-  - '2909'
-  editor: None // ΑΘΗΝΑ
-  pages: 233
-  topics:
-  - ΠΑΓΚΟΣΜΙΑ ΦΙΛΟΣΟΦΙΑ
-  - ΛΕΞΙΚΟ
-  - ΦΙΛΟΣΟΦΙΑ
+  authors: []
+  entry_numbers: []
+  topics: []
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1679
-    1: ΓΙΟΥΝΤΙΝ,Π
-    2: ΦΙΛΟΣΟΦΙΚΟ ΛΕΞΙΚΟ
-    4: 103 ΡΟΖ
-    5: '2909'
-    8: Χ.Ε
-    9: ΑΘΗΝΑ
-    10: Χ.Χ
-    11: 233Σ
-    12: ΠΑΓΚΟΣΜΙΑ ΦΙΛΟΣΟΦΙΑ-ΛΕΞΙΚΟ
-    13: ΦΙΛΟΣΟΦΙΑ-ΛΕΞΙΚΟ
-    14: ΛΕΞΙΚΟ-ΦΙΛΟΣΟΦΙΑ
+    1: null
+    2: null
     3: null
+    4: null
+    5: null
     6: null
     7: null
+    8: null
+    9: null
+    10: null
+    11: null
+    12: null
+    13: null
+    14: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -87028,49 +86960,37 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1680
-  authors:
-  - ΤΣΟΥΤΣΙΝΟΣ,ΘΕΟΧΑΡΗΣ
-  language: el
-  title: Ο ΟΜΗΡΟΣ ΚΑΤΑ ΤΟΝ ΦΙΛΟΣΟΦΟΥ
-  dewey: 185.1 ΤΣΟ
-  entry_numbers:
-  - '2910'
-  editor: None // ΑΘΗΝΑ
-  edition_year: 1928
-  pages: 208
-  topics:
-  - ΕΛΛΗΝΙΚΗ ΦΙΛΟΣΟΦΙΑ
-  - ΑΡΙΣΤΟΤΕΛΗΣ
-  - ΦΙΛΟΣΟΦΙΑ
-  - ΟΜΗΡΟΣ
+  authors: []
+  entry_numbers: []
+  topics: []
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1680
-    1: ΤΣΟΥΤΣΙΝΟΣ,ΘΕΟΧΑΡΗΣ
-    2: Ο ΟΜΗΡΟΣ ΚΑΤΑ ΤΟΝ ΦΙΛΟΣΟΦΟΥ
-    4: 185.1 ΤΣΟ
-    5: '2910'
-    8: Χ.Ε
-    9: ΑΘΗΝΑ
-    10: '1928'
-    11: 208Σ
-    12: ΕΛΛΗΝΙΚΗ ΦΙΛΟΣΟΦΙΑ-ΑΡΙΣΤΟΤΕΛΗ
-    13: ΦΙΛΟΣΟΦΙΑ-ΑΡΙΣΤΟΤΕΛΗ
-    14: ΑΡΙΣΤΟΤΕΛΗ-ΟΜΗΡΟΣ
-    15: ΟΜΗΡΟΣ-ΑΡΙΣΤΟΤΕΛΗ
+    1: null
+    2: null
     3: null
+    4: null
+    5: null
     6: null
     7: null
+    8: null
+    9: null
+    10: null
+    11: null
+    12: null
+    13: null
+    14: null
+    15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
     22: null
@@ -88309,15 +88229,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1704
   authors:
-  - WILAMOWITZ-MOELLENDORFF,ULRICH
+  - VON WILAMOWITZ-MOELLENDORFF,ULRICH
   title: ARISTOTELES UHD ATHEN
   dewey: 185.1 WIL
   entry_numbers:
   - '3006'
   editor: None // BERLIN
   edition_year: 1893
   pages: 428
@@ -88329,15 +88249,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1704
     1: WILAMOWITZ-MOELLENDORFF,ULRICH
     2: ARISTOTELES UHD ATHEN
-    4: 185.1 WIL
+    4: 185.1WIL
     5: '3006'
     8: X.E
     9: BERLIN
     10: '1893'
     11: 428S
     12: ΕΛΛΗΝΙΚΗ ΦΙΛΟΣΟΦΙΑ-ΑΡΙΣΤΟΤΕΛΗΣ
     13: ΦΙΛΟΣΟΦΙΑ-ΑΡΙΣΤΟΤΕΛΗΣ
@@ -88671,15 +88591,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1711
   authors:
-  - ΑΓΑΠΗΤΟΣ,ΓΕΩΡΓΙΟΣ Ι.
+  - ΑΓΑΠΗΤΟΣ,ΓΕΩΡΓΙΟΣ,Ι.
   language: el
   title: Η ΝΕΑ ΕΥΡΩΠΗ ΤΟΥ ΜΑΑΣΤΡΙΧΤ ΚΑΙ Η ΕΛΛΑΔΑ ΤΟΥ 2000
   dewey: 938.87 ΑΓΑ
   entry_numbers:
   - '3166'
   editor: ΟΙΚΟΝΟΜΙΚΟ // ΑΘΗΝΑ
   edition_year: 1993
@@ -89137,51 +89057,39 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1720
-  authors:
-  - ΔΗΜΗΤΟΚΑΛΛΗΣ,Γ
-  language: el
-  title: Η ΕΛΛΗΝΙΚΗ ΗΜΙΣΕΛΗΝΟΣ
-  dewey: 938.101 ΜΟΥ
-  entry_numbers:
-  - '3171'
-  editor: None // ΑΘΗΝΑ
-  edition_year: 1988
-  pages: 125
-  topics:
-  - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
-  - ΕΠΙΓΡΑΦΕΣ
-  - ΗΜΙΣΕΛΗΝΟΣ
-  notes: 'Β ΣΥΓΓΡΑΦΕΑΣ: ΜΟΥΤΣΟΠΟΥΛΟΣ,Ν.'
+  authors: []
+  entry_numbers: []
+  topics: []
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1720
-    1: ΔΗΜΗΤΟΚΑΛΛΗΣ,Γ
-    2: Η ΕΛΛΗΝΙΚΗ ΗΜΙΣΕΛΗΝΟΣ
-    4: 938.101ΜΟΥ
-    5: '3171'
-    8: Χ.Ε
-    9: ΑΘΗΝΑ
-    10: '1988'
-    11: 125Σ
-    12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΙΓΡΑΦΕΣ
-    13: ΕΠΙΓΡΑΦΕΣ-ΗΜΙΣΕΛΗΝΟΣ
-    14: ΗΜΙΣΕΛΗΝΟΣ
-    17: Β ΣΥΓΓΡΑΦΕΑΣ:ΜΟΥΤΣΟΠΟΥΛΟΣ,Ν
+    1: null
+    2: null
     3: null
+    4: null
+    5: null
     6: null
     7: null
+    8: null
+    9: null
+    10: null
+    11: null
+    12: null
+    13: null
+    14: null
     15: null
     16: null
+    17: null
     18: null
     19: null
     20: null
     21: null
     22: null
     23: null
     24: null
@@ -89864,15 +89772,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1734
   authors:
-  - ΑΡΑΒΑΝΤΙΝΟΣ,Π
+  - ΑΡΑΒΑΝΤΙΝΟΣ,ΠΑΝΑΓΙΩΤΗΣ
   language: el
   title: ΗΠΕΙΡΩΤΙΚΟΝ ΓΛΩΣΣΑΡΙΟΝ
   dewey: 938.93 ΑΡΑ
   entry_numbers:
   - '3021'
   editor: ΠΕΤΡΑΚΟΥ // ΑΘΗΝΑ
   edition_year: 1909
@@ -91037,35 +90945,36 @@
   dewey: 938 CUR
   entry_numbers:
   - '3088'
   editor: WEIDMANNSHE // BERLIN
   edition_year: 1887
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
+  - ΙΣΤΟΡΙΑ ΕΛΛΗΝΙΚΗ
   notes: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1757
     1: CURTIUS ERNST                       GER
     2: GRIECHISCHE GESCHCHTE
     4: 938 CUR
-    5: 3088-
+    5: '3088'
     8: WEIDMANNSHE
     9: BERLIN
     10: '1887'
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
+    13: ΙΣΤΟΡΙΑ ΕΛΛΗΝΙΚΗ
+    14: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
     17: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
     3: null
     6: null
     7: null
     11: null
-    13: null
-    14: null
     15: null
     16: null
     18: null
     19: null
     20: null
     21: null
     22: null
@@ -91277,15 +91186,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 1762
   authors:
-  - WILCKEN ULRICH
+  - WILCKEN,ULRICH
   language: de
   title: GRIECHISCHE GESCHICHTE
   dewey: 938 WIL
   entry_numbers:
   - '3594'
   editor: OLDENBOURG // MUNCHEN
   edition_year: 1962
@@ -91428,15 +91337,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1765
   authors:
-  - WELWEI-KARL-WILHELN
+  - WELWEI,KARL-WILHELM
   language: de
   title: UNFREIE IN ANTIKEN KRIEGS DIENST
   subtitle: ERSTER TEIL ATHEN U SPARTA
   dewey: 938.035 WEL
   entry_numbers:
   - '3515'
   editor: STEINER // WIESBADEN
@@ -91484,15 +91393,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 1766
   authors:
-  - WEBER GARL
+  - WEBER,CARL
   language: de
   title: ATHEN-AYFSTIEGY GROHSSE DES ANTIKEN STADT STAATES
   dewey: 938.122 WEB
   entry_numbers:
   - '3421'
   editor: ECON // VIENNA
   edition_year: 1979
@@ -92152,15 +92061,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1779
   authors:
-  - ALTHEIM FRANZ
+  - ALTHEIM,FRANZ
   language: de
   title: NIEDERGANG DER ALTEN WELT DIE AUSSERROHMISCHE WELT
   dewey: 938.192 ALT
   entry_numbers:
   - '3434'
   editor: KLOSTERMANN // FRANKFURT
   edition_year: 1952
@@ -92206,15 +92115,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 1780
   authors:
-  - WEBER MAX
+  - WEBER,MAX
   language: de
   title: WIRTSCHAFTSGESCHICHTE
   dewey: 330.9 WEB
   entry_numbers:
   - '3462'
   editor: DUNCKER // MUNCHEN
   edition_year: 1923
@@ -93478,15 +93387,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1805
   authors:
-  - WLLAMOWITZ URLICH
+  - VON WILAMOWITZ-MOELLENDORFF,ULRICH
   language: de
   title: REDEN YND VORTRAHGE
   dewey: 943 WLL
   entry_numbers:
   - '3355'
   editor: WEIDMANNSCHE // BERLIN
   edition_year: 1913
@@ -93943,15 +93852,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 1814
   authors:
-  - ALTHEIM FRANS
+  - ALTHEIM,FRANZ
   language: de
   title: DIE KRISE DER ALTEN WELT DIE AYSSERROHMISCHE WELT
   dewey: 938.192 ALT
   entry_numbers:
   - '3364'
   editor: AHNENERBE // BERLIN
   edition_year: 1943
@@ -94504,15 +94413,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1825
   authors:
-  - WUHST FRITZ
+  - WUST,FRITZ,R.
   language: de
   title: PHILIPP II VON MAKEDONIEN UND GRIECHENLAND
   dewey: 938.171 WUH
   entry_numbers:
   - '3378'
   editor: BECK C. H. // MUNCHEN
   edition_year: 1938
@@ -94707,15 +94616,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1829
   authors:
-  - WEBER ADOLF
+  - WEBER,ADOLF
   language: de
   title: KAPITAL ARBEIT
   dewey: 326 KAP
   entry_numbers:
   - '3382'
   editor: MOHR // TUBINGEN
   edition_year: 1930
@@ -94809,15 +94718,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1831
   authors:
-  - WACHSMUTH WILHELM
+  - WACHSMUTH,WILHELM
   language: de
   title: HELLENISCHE ALTERTHUMSKU NDE
   dewey: 938.11 WAC
   entry_numbers:
   - '3384'
   editor: SCHWETSCHKE // HALLE
   edition_year: 1846
@@ -94860,15 +94769,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 1832
   authors:
-  - ALTHEIM FRANZ
+  - ALTHEIM,FRANZ
   language: de
   title: EPOCHEN DER ROHMISCHEN GESCHICHTE
   dewey: 938.192 ALT
   entry_numbers:
   - '3385'
   editor: KLOSTERMANN // FRANKFURT
   topics:
@@ -95366,15 +95275,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1842
   authors:
-  - WEDDIGEN W
+  - WEDDIGEN,WALTER
   title: SOZIALPOLITIK
   dewey: 335 WED
   entry_numbers:
   - '3396'
   editor: FISCHER // JENA
   edition_year: 1933
   topics:
@@ -97400,15 +97309,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1882
   authors:
-  - WAGEMANN ERNST
+  - WAGEMANN,ERNST
   language: de
   title: WO KOMMT DAS VIELE GELD HER
   dewey: 332 WAG
   entry_numbers:
   - '3442'
   editor: None // DUSSELDORF
   topics:
@@ -97450,15 +97359,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1883
   authors:
-  - WEDDIGEN WALTER
+  - WEDDIGEN,WALTER
   language: de
   title: ALLGEMEINE FINANZWISSEN SCHAFT
   dewey: 330 WED
   entry_numbers:
   - '3443'
   editor: OUELLE // LEIPZIG
   edition_year: 1938
@@ -97602,15 +97511,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 1886
   authors:
-  - WILLRICH
+  - WILLRICH,H.
   language: de
   title: PERIKLES
   dewey: 938.145 WIL
   entry_numbers:
   - '3446'
   editor: DANDEN HORD // GOETTINGEN
   edition_year: 1936
@@ -98361,15 +98270,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1901
   authors:
-  - WINDELBAND WILHELM
+  - WINDELBAND,WILHELM
   language: de
   title: LEHRBUCH DER GESCHICHTE DER PHILOSOPHIE
   dewey: 107 WIE
   entry_numbers:
   - '3461'
   editor: MOHR // TUBINGEN
   edition_year: 1935
@@ -98413,15 +98322,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1902
   authors:
-  - WEBER MAX
+  - WEBER,MAX
   language: de
   title: GESAMMELTE AUFSAHTZE ZUR WISSENSCHAFTSLEHRE
   dewey: 304 WEB
   entry_numbers:
   - '3463'
   editor: MOHR // TUBINGEN
   edition_year: 1922
@@ -98515,15 +98424,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1904
   authors:
-  - WOLF HEINRICH
+  - HEINRICH,WOLF
   language: de
   title: KULTURGESCHICHTE
   dewey: 901 WOL
   entry_numbers:
   - '3465'
   editor: WEICHER // LEIPZIG
   edition_year: 1923
@@ -98722,15 +98631,15 @@
 - dbase_number: 1908
   authors:
   - DRONSEN JOH
   language: de
   title: GESCHICHTE ALEXANDER DES GROSSEN
   dewey: 938.174 DRO
   entry_numbers:
-  - '3471'
+  - '3428'
   editor: GCHEND // BERLIN
   edition_year: 1913
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   - ΜΑΚΕΔΟΝΙΑ
   notes: Η ΙΣΤΟΡΙΑ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
@@ -98738,15 +98647,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1908
     1: DRONSEN JOH                        GER
     2: GESCHICHTE ALEXANDER DES GROSSEN
     4: 938.174DRO
-    5: 3471-
+    5: '3428'
     8: GCHEND
     9: BERLIN
     10: '1913'
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     13: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     14: ΜΑΚΕΔΟΝΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     17: Η ΙΣΤΟΡΙΑ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
@@ -98787,15 +98696,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1909
     1: NIEBUHR B                           GER
     2: KLEINE HISTORISCHE UND PHILOLOSCH
-    4: 102 NIE
+    4: 102NIE
     5: '3471'
     8: ZELLER
     9: OSNABRUHCK
     10: '1269'
     12: ΠΑΓΚΟΣΜΙΑ ΦΙΛΟΣΟΦΙΑ-ΔΙΑΤΡΙΒΕΣ
     13: ΦΙΛΟΣΟΦΙΑ-ΔΙΑΤΡΙΒΕΣ
     14: ΔΙΑΤΡΙΒΕΣ-ΦΙΛΟΣΟΦΙΑ
@@ -98817,15 +98726,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1910
   authors:
-  - WEBER ALFRED
+  - WEBER,ALFRED
   language: de
   title: KULTURGESCHICHTE ALS KULTURSOZIOLOGIE
   dewey: 301 WEB
   entry_numbers:
   - '3472'
   editor: SIJTHOFF'S // LEIDEN
   edition_year: 1935
@@ -98870,16 +98779,15 @@
     30: null
 - dbase_number: 1911
   authors:
   - GEBER FRITS
   language: de
   title: ALEXANDER DER GROSSE YND DIE DIADOCHEN
   dewey: 938.174 GEB
-  entry_numbers:
-  - '3473'
+  entry_numbers: []
   editor: OUELLE-WENER // LEIPZIG
   edition_year: 1925
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   - ΔΙΑΔΟΧΟΙ
   - ΜΑΚΕΔΟΝΙΑ
@@ -98888,24 +98796,24 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 1911
     1: GEBER FRITS                         GER
     2: ALEXANDER DER GROSSE YND DIE DIADOCHEN
     4: 938.174GEB
-    5: '3473'
     8: OUELLE-WENER
     9: LEIPZIG
     10: '1925'
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     13: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ-ΔΙΑΔΟΧΟΙ
     14: ΜΑΚΕΔΟΝΙΑ-ΔΙΑΔΟΧΟΙ
     15: ΔΙΑΔΟΧΟΙ-ΜΑΚΕΔΟΝΙΑ
     17: Ο ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ ΚΑΙ ΟΙ ΔΙΑΔΟΧΟΙ
     3: null
+    5: null
     6: null
     7: null
     11: null
     16: null
     18: null
     19: null
     20: null
@@ -99828,15 +99736,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1930
   authors:
-  - WIETERSHEIM EDUARD
+  - VON WIETERSHEIM,KARL,AUGUST WILHEML EDUARD
   language: de
   title: GESCHCHTE DER VOHLKER WANDERUNG
   dewey: 909 WIE
   entry_numbers:
   - '3491'
   editor: WEIGEL // LEIPZIG
   edition_year: 1839
@@ -100029,15 +99937,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1934
   authors:
-  - VOGT JOSEPH
+  - VOGT,JOSEPH
   language: de
   title: CONSTANTIN DER GROSSE UNT SEIN JAHRHUNDERT
   dewey: 938.311 VOG
   entry_numbers:
   - '3495'
   editor: BRUCKMANN // MUNCHEN
   edition_year: 1949
@@ -100431,15 +100339,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1942
   authors:
-  - WOLF HEINRICH
+  - HEINRICH,WOLF
   language: de
   title: ANGEWANDE RASSEKUNDE
   dewey: 909 WOL
   entry_numbers:
   - '3507'
   editor: WEICHER // BERLIN
   edition_year: 1938
@@ -101039,15 +100947,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1954
   authors:
-  - ANDREAE WILHELM
+  - ANDREAE,WILHELM
   language: de
   title: KAPITALISMUS-BOLSCHEWISMUS FASCHISMUS
   dewey: 335 AND
   entry_numbers:
   - '3523'
   editor: FISCHER // JENA
   edition_year: 1933
@@ -101090,15 +100998,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1955
   authors:
-  - WAGNER ADOLPH
+  - WAGNER,ADOLPH
   language: de
   title: FINANZWISSENSCHAFT
   dewey: 330 WAG
   entry_numbers:
   - '3524'
   editor: WINTER // LEIPZIG
   edition_year: 1910
@@ -101648,15 +101556,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1966
   authors:
-  - VORLAHNDER KARL
+  - VORLANDER,KARL
   language: de
   title: GESICHTE DER PHILOSOPHIE
   dewey: 109 VOR
   entry_numbers:
   - '3539'
   editor: KIEPENHEUER // BERLIN
   edition_year: 1932
@@ -102551,15 +102459,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1984
   authors:
-  - ALTHEIM FRANZ
+  - ALTHEIM,FRANZ
   language: de
   title: ITALIEN UND ROM
   dewey: 945 ALT
   entry_numbers:
   - '3559'
   editor: PANTHEON // AMSTERDAM
   topics:
@@ -102760,49 +102668,39 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1988
-  authors:
-  - STAMMLER RUDOLF
-  language: de
-  title: WIRTSCHAFT UND RECHT
-  dewey: 340 STA
-  entry_numbers:
-  - '3562'
-  editor: GRUYTER // BERLIN
-  edition_year: 1924
-  topics:
-  - ΔΙΚΑΙΟ
-  - ΕΠΙΣΤΗΜΗ
-  notes: ΕΠΙΣΤΗΜΗ ΚΑΙ ΔΙΚΑΙΟ
+  authors: []
+  entry_numbers: []
+  topics: []
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1988
-    1: STAMMLER RUDOLF                   GER
-    2: WIRTSCHAFT UND RECHT
-    4: 340 STA
-    5: '3562'
-    8: GRUYTER
-    9: BERLIN
-    10: '1924'
-    12: ΔΙΚΑΙΟ-ΕΠΙΣΤΗΜΗ
-    13: ΕΠΙΣΤΗΜΗ-ΔΙΚΑΙΟ
-    17: ΕΠΙΣΤΗΜΗ ΚΑΙ ΔΙΚΑΙΟ
+    1: null
+    2: null
     3: null
+    4: null
+    5: null
     6: null
     7: null
+    8: null
+    9: null
+    10: null
     11: null
+    12: null
+    13: null
     14: null
     15: null
     16: null
+    17: null
     18: null
     19: null
     20: null
     21: null
     22: null
     23: null
     24: null
@@ -102960,15 +102858,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 1992
   authors:
-  - WILAMOWITZ ULRICH
+  - VON WILAMOWITZ-MOELLENDORFF,ULRICH
   language: de
   title: DER GLAUBE DER HELLENEN
   dewey: 938.031 WIL
   entry_numbers:
   - '3566'
   editor: WEIDMANNSCHE // BERLIN
   edition_year: 1931
@@ -103336,16 +103234,16 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 1999
     1: SOMBART WERNER                     GER
     2: DER MODERNE KAPITALISMUS
-    4: 320 SOM
-    5: 3575-
+    4: 320SOM
+    5: '3575'
     8: DUNCKER
     9: MUHNCHEN
     10: '1922'
     12: ΠΟΛΙΤΙΚΗ ΕΠΙΣΤΗΜΗ-ΚΕΦΑΛΟΚΡΑΤΙΑ
     13: ΕΠΙΣΤΗΜΗ-ΠΟΛΙΤΙΚΗ
     14: ΚΕΦΑΛΟΚΡΑΤΙΑ
     17: Η ΜΟΝΤΕΡΝΑ ΚΕΦΑΛΟΚΡΑΤΙΑ
@@ -103366,20 +103264,19 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2000
   authors:
-  - WILAMOWIZ URICH
+  - VON WILAMOWITZ-MOELLENDORFF,ULRICH
   language: de
   title: KLEINE SCHRIFTEN
   dewey: 834 WIL
-  entry_numbers:
-  - '3575'
+  entry_numbers: []
   editor: AKADEMIE VERLAG // BERLIN
   edition_year: 1971
   topics:
   - ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΚΕΙΜΕΝΑ
   - ΛΟΓΟΤΕΧΝΙΑ
   - ΓΕΡΜΑΝΙΚΑ
@@ -103388,25 +103285,25 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 2000
     1: WILAMOWIZ URICH                     GER
     2: KLEINE SCHRIFTEN
-    4: 834 WIL
-    5: 3575-
+    4: 834WIL
     8: AKADEMIE VERLAG
     9: BERLIN
     10: '1971'
     12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΚΕΙΜΕΝΑ
     13: ΛΟΓΟΤΕΧΝΙΑ-ΚΕΙΜΕΝΑ
     14: ΚΕΙΜΕΝΑ-ΓΕΡΜΑΝΙΚΑ
     17: ΚΕΙΜΕΝΑ
     30: 4 ΤΟΜΟΙ
     3: null
+    5: null
     6: null
     7: null
     11: null
     15: null
     16: null
     18: null
     19: null
@@ -103972,15 +103869,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2012
   authors:
-  - WEIGALL ARTHUR
+  - WEIGALL,ARTHUR
   language: de
   title: NERO-KAISER VON ROM
   dewey: 938.192 WEI
   entry_numbers:
   - '3589'
   editor: HOHGER // VIENNA
   edition_year: 1936
@@ -104225,15 +104122,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2017
   authors:
-  - VEZIN AUG
+  - VEZIN,AUGUST
   language: de
   title: EUMENES VON KARDIA
   dewey: 909 VEZ
   entry_numbers:
   - '3597'
   topics:
   - ΠΑΓΚΟΣΜΙΑ ΙΣΤΟΡΙΑ
@@ -104473,15 +104370,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2022
   authors:
-  - ALTHEIM FRANZ
+  - ALTHEIM,FRANZ
   language: de
   title: ROHMISCHE GESCHICHTE
   dewey: 945 ALT
   entry_numbers:
   - '3604'
   editor: KLOSTERMANN // FRANKFURT
   edition_year: 1951
@@ -104826,15 +104723,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2029
   authors:
-  - VOGT JOSEPH
+  - VOGT,JOSEPH
   language: de
   title: ROHMISCHE GESCHICHTE DIE ROHMISCHE REPUBLIK
   dewey: 945 VOG
   entry_numbers:
   - '3614'
   editor: HERDER // FREIBURG
   edition_year: 1932
@@ -104876,15 +104773,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2030
   authors:
-  - WOLF JULIUS
+  - WOLF,JULIUS
   language: de
   title: ROHMISCHE GESCHICHTE DIE ROHMISCHE KAISERZEIT
   dewey: 945 WOL
   entry_numbers:
   - '3615'
   editor: HERDER // FREIBURG
   edition_year: 1932
@@ -104926,15 +104823,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2031
   authors:
-  - WENDEL CARL
+  - WENDEL,CARL
   language: de
   title: DIE UHBERLIEFERUNG DER SCHOLIEN ZU APOLLONIOS VON RHODOS
   dewey: 104 WEN
   entry_numbers:
   - '3616'
   editor: WEIDMANN // BERLIN
   edition_year: 1932
@@ -107355,15 +107252,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2079
   authors:
-  - VAGN POULSEN
+  - POULSEN,VAGN
   language: de
   title: GRIECHISCHE KUNST
   dewey: 730 VAG
   entry_numbers:
   - '3083'
   editor: STEINKOPF // MUNCHEN
   edition_year: 1962
@@ -107863,38 +107760,37 @@
     29: null
 - dbase_number: 2089
   authors:
   - BEKGTSON HERMANN
   language: de
   title: HERRSCHERGESTALTE DES HELLENISMUS
   dewey: 938 BEK
-  entry_numbers:
-  - '3088'
+  entry_numbers: []
   editor: BECK // MUNCHEN
   edition_year: 1975
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΕΛΛΗΝΙΣΜΟΣ
   notes: Η ΒΑΣΙΚΗ ΜΟΡΦΗ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 2089
     1: BEKGTSON HERMANN                   GER
     2: HERRSCHERGESTALTE DES HELLENISMUS
-    4: 938 BEK
-    5: '3088'
+    4: 938BEK
     8: BECK
     9: MUHNCHEN
     10: '1975'
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΣΜΟΣ
     13: ΕΛΛΗΝΙΣΜΟΣ
     17: Η ΒΑΣΙΚΗ ΜΟΡΦΗ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
     3: null
+    5: null
     6: null
     7: null
     11: null
     14: null
     15: null
     16: null
     18: null
@@ -108587,16 +108483,17 @@
   editor: ROTHSCHILD // BERLIN
   edition_year: 1920
   topics:
   - ΠΟΛΙΤΙΚΗ ΟΙΚΟΝΟΜΙΑ
   - ΛΕΞΙΚΟ
   - ΟΙΚΟΝΟΜΙΑ
   - ΠΟΛΙΤΙΚΗ
-  volume: ΤΟΜΟΣ IV
-  notes: ΛΕΞΙΚΟ ΤΗΣ ΠΟΛΙΤΙΚΗΣ ΟΙΚΟΝΟΜΙΑΣ ΑΝΟΙΚΟΔΟΜΗΣΗ
+  notes: 'ΛΕΞΙΚΟ ΤΗΣ ΠΟΛΙΤΙΚΗΣ ΟΙΚΟΝΟΜΙΑΣ ΑΝΟΙΚΟΔΟΜΗΣΗ
+
+    <<ΤΟΜΟΣ Ι,IV>>'
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 2103
     1: HANDBUCH DER POLITIK.               GER
     2: DER WIRTSCHAFTLICHE WIE DERAUFBAU
@@ -108605,15 +108502,15 @@
     8: ROTHSCHILD
     9: BERLIN
     10: '1920'
     12: ΠΟΛΙΤΙΚΗ ΟΙΚΟΝΟΜΙΑ-ΛΕΞΙΚΟ
     13: ΛΕΞΙΚΟ-ΠΟΛΙΤΙΚΗ ΟΙΚΟΝΟΜΙΑ
     14: ΟΙΚΟΝΟΜΙΑ-ΠΟΛΙΤΙΚΗ
     17: ΛΕΞΙΚΟ ΤΗΣ ΠΟΛΙΤΙΚΗΣ ΟΙΚΟΝΟΜΙΑΣ ΑΝΟΙΚΟΔΟΜΗΣΗ
-    30: '                <<ΤΟΜΟΣ IV>>'
+    30: '                <<ΤΟΜΟΣ Ι,IV>>'
     3: null
     6: null
     7: null
     11: null
     15: null
     16: null
     18: null
@@ -108675,63 +108572,52 @@
     24: null
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2105
-  authors:
-  - HANDBUCH DER POLITIK
-  language: de
-  title: DIE GRUNDLAGEN DER POLITIK
-  dewey: 303 HAN
-  entry_numbers:
-  - '3141'
-  editor: ROTHSCHILD // BERLIN
-  edition_year: 1920
-  topics:
-  - ΠΟΛΙΤΙΚΗ
-  - ΛΕΞΙΚΟ
-  volume: ΤΟΜΟΣ I
-  notes: ΛΕΞΙΚΟ ΠΟΛΙΤΙΚΗ ΟΙ ΒΑΣΕΙΣ ΤΗΣ ΠΟΛΙΤΙΚΗΣ
+  authors: []
+  entry_numbers: []
+  topics: []
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 2105
-    1: HANDBUCH DER POLITIK                GER
-    2: DIE GRUNDLAGEN DER POLITIK
-    4: 303 HAN
-    5: '3141'
-    8: ROTHSCHILD
-    9: BERLIN
-    10: '1920'
-    12: ΠΟΛΙΤΙΚΗ-ΛΕΞΙΚΟ
-    13: ΛΕΞΙΚΟ-ΠΟΛΙΤΙΚΗ
-    17: ΛΕΞΙΚΟ ΠΟΛΙΤΙΚΗ ΟΙ ΒΑΣΕΙΣ ΤΗΣ ΠΟΛΙΤΙΚΗΣ
-    30: '              <<ΤΟΜΟΣ I>>'
+    1: null
+    2: null
     3: null
+    4: null
+    5: null
     6: null
     7: null
+    8: null
+    9: null
+    10: null
     11: null
+    12: null
+    13: null
     14: null
     15: null
     16: null
+    17: null
     18: null
     19: null
     20: null
     21: null
     22: null
     23: null
     24: null
     25: null
     26: null
     27: null
     28: null
     29: null
+    30: null
 - dbase_number: 2106
   authors:
   - BRANDSTAETER
   language: de
   title: GESCHICHTEN AETOLISCHEN LANDES-VOLKES YND BYNDES
   dewey: 838.22 BRA
   entry_numbers:
@@ -109220,15 +109106,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2116
   authors:
-  - WILAMOWITZ-MOELLENDORFF U
+  - VON WILAMOWITZ-MOELLENDORFF,ULRICH
   language: de
   title: PLATON
   subtitle: LEBEN UND WERKE
   dewey: 888.4 WIL
   entry_numbers:
   - '3155'
   editor: WEIDMANNSCHE // BERLIN
@@ -109271,15 +109157,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2117
   authors:
-  - VAHLEN IOHANNES
+  - VAHLEN,JOHANNES
   language: de
   title: ENNIANAE POESIS
   subtitle: RELIOUIAE
   dewey: 800 VAH
   entry_numbers:
   - '3156'
   editor: HAKKERT // AMSTERDAM
@@ -109322,15 +109208,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2118
   authors:
-  - WILAMOWITZ-MOELLENDORFF U
+  - VON WILAMOWITZ-MOELLENDORFF,ULRICH
   language: de
   title: GRIECHISCHE PROSA
   dewey: 880.3 WIL
   entry_numbers:
   - '3157'
   editor: AKADEMIE // BERLIN
   edition_year: 1969
@@ -109470,15 +109356,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2121
   authors:
-  - ASTHOLZ HILDEGARD
+  - URNER-ASTHOLZ,HILDEGARD
   language: de
   title: DAS PROBLEM GESCHICHTE UNTERSUCHT BEI JOHANN GUSTAV DROYSEN
   dewey: 904 AST
   entry_numbers:
   - '3160'
   editor: EBERING // BERLIN
   edition_year: 1933
@@ -110123,15 +110009,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2134
   authors:
-  - WILAMOWITZ-MOELLDORFF U
+  - VON WILAMOWITZ-MOELLENDORFF,ULRICH
   language: de
   title: PINDAROS
   dewey: 885.166 WIL
   entry_numbers:
   - '3188'
   editor: WEIDMANN // BERLIN
   edition_year: 1922
@@ -110173,15 +110059,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2135
   authors:
-  - WILAMOWITZ-MOELLENDORFF U
+  - VON WILAMOWITZ-MOELLENDORFF,ULRICH
   language: de
   title: HELLENISTICHE-SPAEGRIECHISCHE UND LATEINISCHE POESIE
   dewey: 881 WIL
   entry_numbers:
   - '3189'
   editor: HAKKERT // AMSTERDAM
   edition_year: 1971
@@ -110275,15 +110161,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2137
   authors:
-  - ALTHEIM FRANZ-FELBER DIETR
+  - ALTHEIM,FRANZ
+  - FELBER,DIETRICH
   language: de
   title: UNTERSUCHUNGEN ZUR ROH MISCHEN GESCHICHTE
   dewey: 937 ALT
   entry_numbers:
   - '3191'
   editor: KLOSTERMANN // FRANKFURT
   edition_year: 1961
@@ -110324,15 +110211,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2138
   authors:
-  - ASTER ERNST
+  - VON ASTER,ERNST,LUDWIG
   language: de
   title: GESCHICHTE DER PHILOSOPHIE
   dewey: 109 AST
   entry_numbers:
   - '3192'
   editor: KPOHNER // STUTTGART
   topics:
@@ -111072,15 +110959,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2153
   authors:
-  - ALTHEIM FRANZ-STIEHL RUTH
+  - ALTHEIM,FRANZ
+  - STIEHL,RUTH
   language: de
   title: FINANZGESCHICHTE DER SPAHTANTIKE
   dewey: 330 ALT
   entry_numbers:
   - '3208'
   editor: KLOSTERMANN // FRANKFURT
   edition_year: 1957
@@ -111283,15 +111171,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2157
   authors:
-  - WACHSMUT WILHELM
+  - WACHSMUTH,WILHELM
   language: de
   title: HELLENISCHE ALTERTHUMS KUNDE
   dewey: 300 WAC
   entry_numbers:
   - '3213'
   editor: SCHWETSCHKE // HALLE
   edition_year: 1846
@@ -111937,15 +111825,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2170
   authors:
-  - WEBER ADOLF
+  - WEBER,ADOLF
   language: de
   title: KURZGEFASSTE VOLKSWIRTSCHAFTSLEHRE
   dewey: 321 WEB
   entry_numbers:
   - '3625'
   editor: DUNCKER // BERLIN
   edition_year: 1942
@@ -112039,15 +111927,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2172
   authors:
-  - WERTHEIMER OSKAR
+  - WERTHEIMER,OSKAR
   language: de
   title: KLEOPATRA
   dewey: 932 WER
   entry_numbers:
   - '3627'
   editor: AMALTHEA // ZURICH
   edition_year: 1930
@@ -112445,64 +112333,52 @@
     24: null
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2180
-  authors:
-  - WILAMOWITZ ULRICH
-  language: de
-  title: ARISTOLELES UND ATHEN
-  dewey: 185.1 WIL
-  entry_numbers:
-  - '3006'
-  editor: WEIDMANN // BERLIN
-  edition_year: 1893
-  topics:
-  - ΕΛΛΗΝΙΚΗ ΦΙΛΟΣΟΦΙΑ
-  - ΑΡΙΣΤΟΤΕΛΗΣ
-  - ΑΘΗΝΑ
-  volume: ΤΟΜΟΣ Β
-  notes: ΑΡΙΣΤΟΤΕΛΗΣ ΚΑΙ ΑΘΗΝΑΙ
+  authors: []
+  entry_numbers: []
+  topics: []
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 2180
-    1: WILAMOWITZ ULRICH                   GER
-    2: ARISTOLELES UND ATHEN
-    4: 185.1 WIL
-    5: '3006'
-    8: WEIDMANN
-    9: BERLIN
-    10: '1893'
-    12: ΕΛΛΗΝΙΚΗ ΦΙΛΟΣΟΦΙΑ-ΑΡΙΣΤΟΤΕΛΗΣ
-    13: ΑΡΙΣΤΟΤΕΛΗΣ-ΑΘΗΝΑ
-    14: ΑΘΗΝΑ-ΑΡΙΣΤΟΤΕΛΗΣ
-    17: ΑΡΙΣΤΟΤΕΛΗΣ ΚΑΙ ΑΘΗΝΑΙ
-    30: ΤΟΜΟΣ Β
+    1: null
+    2: null
     3: null
+    4: null
+    5: null
     6: null
     7: null
+    8: null
+    9: null
+    10: null
     11: null
+    12: null
+    13: null
+    14: null
     15: null
     16: null
+    17: null
     18: null
     19: null
     20: null
     21: null
     22: null
     23: null
     24: null
     25: null
     26: null
     27: null
     28: null
     29: null
+    30: null
 - dbase_number: 2181
   authors:
   - BAHRDT HANS
   language: de
   title: WEGE ZUR SOZIOLOGIE
   dewey: 301 BAH
   entry_numbers:
@@ -112741,15 +112617,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2186
   authors:
-  - WAGNER ADOLF
+  - WAGNER,ADOLF
   language: de
   title: FINANZWISSENSCHAFT
   dewey: 330 WAG
   entry_numbers:
   - '3230'
   editor: WINTERSCHE // LEIPZIG
   edition_year: 1890
@@ -112791,15 +112667,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2187
   authors:
-  - WAGNER ADOLF
+  - WAGNER,ADOLF
   language: de
   title: LEHR-UND HANBUCH DER POLITISCHEN OEKONOMIE
   dewey: 321 WAG
   entry_numbers:
   - '3231'
   editor: WINTERSCHE // LEIPZIG
   edition_year: 1883
@@ -112944,15 +112820,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2190
   authors:
-  - WIETRSCHEIM EDUARD
+  - VON WIETERSHEIM,KARL,AUGUST WILHEML EDUARD
   language: de
   title: GESCHICHTE DER VOHLKER WANDERUNG
   dewey: 900 WIE
   entry_numbers:
   - '3234'
   editor: WEIGEL // LEIPZIG
   edition_year: 1860
@@ -113044,15 +112920,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2192
   authors:
-  - WIRTH PETER
+  - WIRTH,PETER
   language: de
   title: EUSTAHIANA
   dewey: 200 WIR
   entry_numbers:
   - '3237'
   editor: HAKKER // AMSTERDAM
   edition_year: 1980
@@ -113654,15 +113530,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2204
   authors:
-  - WEDDIGEN
+  - WEDDIGEN,WALTER
   language: de
   title: GRUNDRISS DER WIRTSCHAFTS THEORIE
   dewey: 330.1 WED
   entry_numbers:
   - '3250'
   editor: FISCHER // JENA
   edition_year: 1934
@@ -113966,15 +113842,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2210
   authors:
-  - WILSON WOODROW
+  - WOODROW WILSON,THOMAS
   language: de
   title: MEMOIREN UND DOMUMENTE YHBER DEN VERTRAG WERSAILLES
   dewey: 909 WIL
   entry_numbers:
   - '3256'
   editor: LIST // LEIPZIG
   edition_year: 1923
@@ -114265,15 +114141,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2216
   authors:
-  - APELT OTTO
+  - APELT,OTTO
   language: de
   title: DIOGENES LAERTIUS
   dewey: 938.2 APE
   entry_numbers:
   - '3262'
   editor: MEINER // LEIPZIG
   edition_year: 1921
@@ -114518,15 +114394,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2221
   authors:
-  - WILAMOWITZ-MOELLENDORE URLICH
+  - VON WILAMOWITZ-MOELLENDORFF,ULRICH
   language: de
   title: ANTIGONOS VON KARYSTOS
   dewey: 180 WIL
   entry_numbers:
   - '3268'
   editor: WEIDMANN // BERLIN
   edition_year: 1965
@@ -114618,15 +114494,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2223
   authors:
-  - WAATZ ALEXANDER
+  - WAATZ,ALEXANDER
   language: de
   title: AOWJETISCHE KOLLEKTIWIRT SCHAFT
   dewey: 947 WAA
   entry_numbers:
   - '3270'
   editor: WEICHER // BERLIN
   edition_year: 1941
@@ -114674,16 +114550,15 @@
     30: null
 - dbase_number: 2224
   authors:
   - DEUSSEN PAUL
   language: de
   title: DIE PHILOSOPHIE DER GRIECEN
   dewey: 180.938 DEU
-  entry_numbers:
-  - '3271'
+  entry_numbers: []
   editor: BROCKHAUS // LEIPZIG
   edition_year: 1921
   topics:
   - ΕΛΛΗΝΙΚΗ ΦΙΛΟΣΟΦΙΑ
   - ΦΙΛΟΣΟΦΙΑ
   - ΕΛΛΗΝΙΚΗ
   notes: Η ΕΛΛΗΝΙΚΗ ΦΙΛΟΣΟΦΙΑ
@@ -114691,22 +114566,22 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 2224
     1: DEUSSEN PAUL                       GER
     2: DIE PHILOSOPHIE DER GRIECEN
     4: 180.938DEU
-    5: '3271'
     8: BROCKHAUS
     9: LEIPZIG
     10: '1921'
     12: ΕΛΛΗΝΙΚΗ ΦΙΛΟΣΟΦΙΑ
     13: ΦΙΛΟΣΟΦΙΑ-ΕΛΛΗΝΙΚΗ
     17: Η ΕΛΛΗΝΙΚΗ ΦΙΛΟΣΟΦΙΑ
     3: null
+    5: null
     6: null
     7: null
     11: null
     14: null
     15: null
     16: null
     18: null
@@ -114972,15 +114847,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2230
   authors:
-  - WILAMOWITZ-MOELLENDORFF
+  - VON WILAMOWITZ-MOELLENDORFF,ULRICH
   language: de
   title: GESCHICHTE DER PHILOLOGIE
   dewey: 109 WIL
   entry_numbers:
   - '3276'
   editor: TEYBNER // LEIPZIG
   edition_year: 1959
@@ -115090,15 +114965,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 2232
     1: FINLAY GEORG                        GER
     2: GRIECHENLAND UNTER DEN ROHMERIN
-    4: 938.19 FIN
+    4: 938.19FIN
     5: '3278'
     8: WIGANT
     9: LEIPZIG
     10: '1861'
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΡΩΜΑΙΟΙ
     13: ΡΩΜΑΙΚΗ ΚΥΡΙΑΡΧΙΑ-ΕΛΛΗΝΕΣ
     14: ΡΩΜΑΙΟΙ
@@ -115119,50 +114994,39 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2233
-  authors:
-  - FINLAY,GEORGE
-  language: de
-  title: GRIECHENLAND UNTER DEN ROHMERN
-  dewey: 938.19 FIN
-  entry_numbers:
-  - '3278'
-  editor: WIGANT // LEIPZIG
-  edition_year: 1861
-  topics:
-  - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
-  - ΡΩΜΑΙΟΙ
-  - ΡΩΜΑΙΚΗ ΚΥΡΙΑΡΧΙΑ
-  notes: ΟΙ ΕΛΛΗΝΕΣ ΥΠΟ ΤΗΝ ΚΑΤΟΧΗ ΤΩΝ ΡΩΜΑΙΩΝ
+  authors: []
+  entry_numbers: []
+  topics: []
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 2233
-    1: FINLAY GEORG                       GER
-    2: GRIECHENLAND UNTER DEN ROHMERN
-    4: 938.19 FIN
-    5: '3278'
-    8: WIGANT
-    9: LEIPZIG
-    10: '1861'
-    12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΡΩΜΑΙΟΙ
-    13: ΡΩΜΑΙΟΙ
-    14: ΡΩΜΑΙΚΗ ΚΥΡΙΑΡΧΙΑ
-    17: ΟΙ ΕΛΛΗΝΕΣ ΥΠΟ ΤΗΝ ΚΑΤΟΧΗ ΤΩΝ ΡΩΜΑΙΩΝ
+    1: null
+    2: null
     3: null
+    4: null
+    5: null
     6: null
     7: null
+    8: null
+    9: null
+    10: null
     11: null
+    12: null
+    13: null
+    14: null
     15: null
     16: null
+    17: null
     18: null
     19: null
     20: null
     21: null
     22: null
     23: null
     24: null
@@ -115731,15 +115595,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2245
   authors:
-  - ABBOTT G F
+  - ABBOTT,George,Frederick
   language: de
   title: MACEDONIAN FOLKORE
   dewey: 938.21 ABB
   entry_numbers:
   - '3297'
   editor: ARGONAUT INC // CHICAGO
   edition_year: 1969
@@ -115880,15 +115744,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2248
   authors:
-  - VEITH G
+  - VEITH,G.
   language: de
   title: JULIUS CAESARS
   subtitle: GESCHICHTE DER FELDZYHGE
   dewey: 938.192 VEI
   entry_numbers:
   - '3295'
   editor: SELDEL // VIENNA
@@ -116035,15 +115899,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2251
   authors:
-  - WILAMOWITZ-MOELLNDORFF U
+  - VON WILAMOWITZ-MOELLENDORFF,ULRICH
   language: de
   title: EINLETUNG IN DIE GRIECHSCHE TRAGOHDIE
   dewey: 881.2 WIL
   entry_numbers:
   - '3291'
   editor: WEIDMANN // BERLIN
   edition_year: 1910
@@ -117262,15 +117126,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2275
   authors:
-  - WILAMOWITZ-MOELLENDORFFU
+  - VON WILAMOWITZ-MOELLENDORFF,ULRICH
   language: de
   title: HELLENISTISCHE DICHTUNG IN DER ZEIT DES KALLIMACHOS
   dewey: 880.1 WIL
   entry_numbers:
   - '3324'
   editor: WEIDMANN // BERLIN
   edition_year: 1924
@@ -117569,15 +117433,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2281
   authors:
-  - WEIGALL ARTHUR
+  - WEIGALL,ARTHUR
   language: de
   title: ALEXANDER DER GROSSE
   dewey: 938.174 WEI
   entry_numbers:
   - '3331'
   editor: None // LEIPZIG
   topics:
@@ -118896,49 +118760,50 @@
 - dbase_number: 2307
   authors:
   - ΜΟΜΣΕΝ,ΘΕΟΔΩΡΟΥ
   language: el
   title: ΡΩΜΑΙΚΗ ΙΣΤΟΡΙΑ
   dewey: 937 ΜΟΜ
   entry_numbers:
-  - '3648'
   - '3647'
+  - '3648'
   - '3649'
   translators:
   - ΣΑΚΕΛΛΑΡΟΠΟΥΛΟΣ,
   editor: ΣΑΚΕΛΛΑΡΙΟΥ // ΑΘΗΝΑ
   edition_year: 1906
   pages: 706
   topics:
   - ΡΩΜΑΙΚΗ ΙΣΤΟΡΙΑ
+  - ΙΣΤΟΡΙΑ ΡΩΜΑΙΚΗ
   copies: 2
   volume: 'ΤΟΜΟΣ 1
 
     ΤΟΜΟΣ 2'
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 2307
     1: ΜΟΜΣΕΝ,ΘΕΟΔΩΡΟΥ
     2: ΡΩΜΑΙΚΗ ΙΣΤΟΡΙΑ
     4: 937 ΜΟΜ
-    5: 3648-3647-3649-
+    5: 3647-3648-3649
     6: ΣΑΚΕΛΛΑΡΟΠΟΥΛΟΣ
     8: ΣΑΚΕΛΛΑΡΙΟΥ
     9: ΑΘΗΝΑ
     10: '1906'
     11: 706Σ
     12: ΡΩΜΑΙΚΗ ΙΣΤΟΡΙΑ
+    13: ΙΣΤΟΡΙΑ ΡΩΜΑΙΚΗ
+    14: ΡΩΜΑΙΚΗ ΙΣΤΟΡΙΑ
     17: 2 ΑΝΤΙΤΥΠΑ ΤΟΜΟΣ 1
     30: 1 ΑΝΤΙΤΥΠΟ ΤΟΜΟΣ 2
     3: null
     7: null
-    13: null
-    14: null
     15: null
     16: null
     18: null
     19: null
     20: null
     21: null
     22: null
@@ -118946,45 +118811,34 @@
     24: null
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2308
-  authors:
-  - ΣΑΚΕΛΛΑΡΟΠΟΥΛΟΣ,
-  language: el
-  title: ΡΩΜΑΙΚΗ ΙΣΤΟΡΙΑ
-  dewey: 937 ΜΟΜ
-  entry_numbers:
-  - '3648'
-  - '3647'
-  - '3649'
-  editor: ΣΑΚΕΛΛΑΡΙΟΥ // ΑΘΗΝΑ
-  edition_year: 1906
-  pages: 704
-  topics:
-  - ΡΩΜΑΙΚΗ ΙΣΤΟΡΙΑ
+  authors: []
+  entry_numbers: []
+  topics: []
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 2308
-    1: ΣΑΚΕΛΛΑΡΟΠΟΥΛΟΣ,
-    2: ΡΩΜΑΙΚΗ ΙΣΤΟΡΙΑ
-    4: 937 ΜΟΜ
-    5: 3648-3647-3649-
-    8: ΣΑΚΕΛΛΑΡΙΟΥ
-    9: ΑΘΗΝΑ
-    10: '1906'
-    11: 704Σ
-    12: ΡΩΜΑΙΚΗ ΙΣΤΟΡΙΑ
+    1: null
+    2: null
     3: null
+    4: null
+    5: null
     6: null
     7: null
+    8: null
+    9: null
+    10: null
+    11: null
+    12: null
     13: null
     14: null
     15: null
     16: null
     17: null
     18: null
     19: null
@@ -119920,15 +119774,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2327
   authors:
-  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ
+  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ,
   language: el
   title: ΜΕΡΟΛΗΨΙΕΣ ΤΟΥ ΘΟΥΚΥΔΙΔΗ
   subtitle: ΔΟΚΙΜΙΟ
   dewey: 881.2 ΒΛΑ
   entry_numbers:
   - '2927'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
@@ -120329,15 +120183,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2335
   authors:
-  - ΒΡΕΛΛΗΣ,ΑΡΙΣΤΟΤΕΛΗΣ ΠΑΝ
+  - ΒΡΕΛΛΗΣ,ΑΡΙΣΤΟΤΕΛΗΣ,ΠΑΝ.
   language: el
   title: ΣΥΜΒΟΛΗ ΣΤΗΝ ΕΡΕΥΝΑ ΤΗΣ ΔΗΜΟΤΙΚΗΣ ΗΠΕΙΡΩΤΙΚΗΣ ΜΟΥΣΙΚΗΣ
   dewey: 782.42 ΒΡΕ
   entry_numbers:
   - '754'
   editor: None // ΙΩΑΝΝΙΝΑ
   edition_year: 1985
@@ -120793,15 +120647,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2344
   authors:
-  - ΑΘΑΝΑΣΙΑΔΗ-ΝΟΒΑ,ΘΕΜ
+  - ΑΘΑΝΑΣΙΑΔΗΣ-ΝΟΒΑΣ,ΘΕΜΙΣΤΟΚΛΗΣ
   language: el
   title: ΣΤΗΝ ΤΟΥΡΚΙΑ ΜΕ ΔΗΜΟΣΙΑΓΡΑΦΙΚΟ ΦΑΚΟ(1925-1926)
   dewey: 938.73 ΑΘΑ
   entry_numbers:
   - '2540'
   editor: None // ΑΘΗΝΑ
   edition_year: 1967
@@ -121520,15 +121374,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2358
   authors:
-  - ΒΛΑΧΟΣ,Κ.Π
+  - ΒΛΑΧΟΣ,Κ.,Π.
   language: el
   title: Η ΑΛΛΗΛΟΓΡΑΦΙΑ ΤΟΥ ΓΑΛΛΙΚΟΥ ΥΠΟΠΡΟΞΕΝΕΙΟΥ ΤΗΣ ΑΡΤΑΣ 1815-17
   dewey: 938.481 ΒΛΑ
   entry_numbers:
   - '3708'
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -121879,15 +121733,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2365
   authors:
-  - ΑΛΦΙΕΡΗ,ΒΙΚΤΩΡΟΣ
+  - ALFIERI,VITTORIO
   language: el
   title: ΣΑΟΥΛ
   subtitle: ΤΡΑΓΩΔΙΑ
   dewey: 852 ΑΛΦ
   entry_numbers:
   - '1396'
   translators:
@@ -121984,15 +121838,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2367
   authors:
-  - ΑΝΝΙΝΟΥ,ΜΠΑΜΠΗΣ
+  - ΑΝΝΙΝΟΣ,ΜΠΑΜΠΗΣ
   language: el
   title: ΙΣΤΟΡΙΚΑ ΣΗΜΕΙΩΜΑΤΑ
   dewey: 938.501 ΑΝΝ
   entry_numbers:
   - '1817'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 1925
@@ -122035,15 +121889,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2368
   authors:
-  - ΑΡΧΙΜΑΝΔΡΙΤΟΥ,ΙΩΑΝ
+  - ΙΩΑΝΝΗΣ,ΑΡΧΙΜΑΝΔΡΙΤΗΣ
   language: el
   title: ΤΣΑΜΗΔΕΣ
   subtitle: ΟΔΥΝΗ ΚΑΙ ΔΑΚΡΥΑ ΤΗΣ ΘΕΣΠΡΩΤΙΑΣ
   dewey: 938.937 ΑΡΧ
   entry_numbers:
   - '2151'
   editor: ΓΕΩΡΓΙΑΔΗ // None
@@ -123982,15 +123836,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2407
   authors:
-  - ARISTOPHANE
+  - ΑΡΙΣΤΟΦΑΝΗΣ
   language: fr
   title: THEATRE COMPLET
   subtitle: LES OISEAUX,LUSISTRATA,LES THESMOPHORIES,LES GRENOULLES,PLUT
   dewey: 881.28 ARI
   entry_numbers:
   - '4045'
   editor: LE LIVE DE POCHE // PARIS
@@ -124085,15 +123939,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2409
   authors:
-  - VASILIEV A
+  - VASILIEV,ALEXANDER,ALEXANDROVICH
   language: fr
   title: HISTORE L'EMPIRE BYZANTIN (1081-1453)
   dewey: 938.3 VAS
   entry_numbers:
   - '4043'
   editor: PICARD // PARIS
   edition_year: 1932
@@ -125152,15 +125006,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2430
   authors:
-  - WICART A
+  - WICART,ALEXIS
   language: fr
   title: L'ORATEUR
   dewey: 808 WIC
   entry_numbers:
   - '4022'
   editor: VOX // None
   edition_year: 1935
@@ -125360,15 +125214,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2434
   authors:
-  - VELLEIUS PATERCULUS ET
+  - VELLEIUS PATERCULUS,MARCUS
   language: fr
   title: FLORUS
   subtitle: HISTOIRE ROMAINE
   dewey: 937 VEL
   entry_numbers:
   - '4018'
   editor: GARNIER // PARIS
@@ -125567,15 +125421,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2438
   authors:
-  - ANGEL JACOUES
+  - ANCEL,JACOUES
   language: fr
   title: PEUPLES ET NATIONS DES BALKANS
   dewey: 940 ANG
   entry_numbers:
   - '4014'
   editor: COLIN // PARIS
   edition_year: 1926
@@ -125763,15 +125617,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2442
   authors:
-  - VASILIEV A
+  - VASILIEV,ALEXANDER,ALEXANDROVICH
   language: fr
   title: LA DYNASTIE D'AMORIUM  820-867
   dewey: 938.34 VAS
   entry_numbers:
   - '4010'
   editor: None // BRUXELLES
   edition_year: 1956
@@ -125913,15 +125767,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2445
   authors:
-  - ALTHEIM E
+  - ALTHEIM,FRANZ
   language: fr
   title: LE DECLIN DU MONDE ANTIOUE
   dewey: 909 ALT
   entry_numbers:
   - '4007'
   editor: PAYOT // PARIS
   edition_year: 1953
@@ -126416,15 +126270,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2455
   authors:
-  - AYMARD ANDRE
+  - AYMARD,ANDRE
   language: fr
   title: LE MONDE GREC AU TEMPS DE PHILIPPE II DE MACEDOINE ET D'ALEX
   subtitle: XANDRE LE GRAND
   dewey: 938.497 ΛΟΙ
   entry_numbers:
   - '3997'
   editor: None // PARIS
@@ -126779,15 +126633,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2462
   authors:
-  - VELLAY CHARLES
+  - VELLAY,CHARLES
   language: fr
   title: LIRREDENTISME HELLENIGUE
   dewey: 938.6 VEL
   entry_numbers:
   - '3990'
   editor: PERRIN // PARIS
   edition_year: 1913
@@ -126980,15 +126834,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2466
   authors:
-  - VALERE MAXIME
+  - MAXIME,VALERE
   language: fr
   title: ACTIONS ET PAROLES MEMORABLES
   dewey: 189.5 VAL
   entry_numbers:
   - '3986'
   editor: CARNIER // PARIS
   topics:
@@ -127584,15 +127438,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2478
   authors:
-  - AYMARD A
+  - AYMARD,ANDRE
   language: fr
   title: LE ROUAUME DE MACEDOINE DE LA MORT D'ALEXANDRE A SA DISPARIT
   dewey: 938.174 AYM
   entry_numbers:
   - '3974'
   editor: None // PARIS
   topics:
@@ -128332,15 +128186,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2493
   authors:
-  - WARMIGTON B
+  - WARMIGTON,BRIAN,HERBERT
   language: fr
   title: HISTOIRE ET CIVILISATION DE CARTHAGE(814-146)
   dewey: 913 WAR
   entry_numbers:
   - '3959'
   editor: PAYOT // PARIS
   edition_year: 1961
@@ -128382,15 +128236,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2494
   authors:
-  - VIRGILE
+  - VIRGILIO
   language: fr
   title: ENEIDE
   dewey: 840 VIR
   entry_numbers:
   - '3958'
   editor: LES BELLES LETTRES // PARIS
   edition_year: 1962
@@ -128983,15 +128837,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2506
   authors:
-  - ARMAND LOUIS
+  - ARMAND,LOUIS
   language: fr
   title: SUEDE SOCIALISTE ET LIBRE ENTREPRISE
   dewey: 335.1 ARM
   entry_numbers:
   - '3946'
   editor: FAYARD-MAME // None
   edition_year: 1970
@@ -129782,15 +129636,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2522
   authors:
-  - AYMARD ANDRE
+  - AYMARD,ANDRE
   language: fr
   title: ETUDES D'HISTOIRE ANCIENNE
   dewey: 913 AYM
   entry_numbers:
   - '3930'
   editor: None // PARIS
   edition_year: 1967
@@ -130075,15 +129929,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2528
   authors:
-  - WILCKEN ULRICH
+  - WILCKEN,ULRICH
   language: fr
   title: ALEXANDRE LE GRAND
   dewey: 938.174 WIL
   entry_numbers:
   - '3924'
   editor: PAYOT // PARIS
   edition_year: 1952
@@ -130823,15 +130677,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2543
   authors:
-  - AFTALION ALBERT
+  - AFTALION,ALBERT
   language: fr
   title: MONNAIE PRIX ET CHANGE
   dewey: 332 AFT
   entry_numbers:
   - '3909'
   editor: SIREX // PARIS
   edition_year: 1950
@@ -131373,15 +131227,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2554
   authors:
-  - ALBERT MAURICE
+  - MAURICE,ALBERT
   language: fr
   title: LE CULTE DE CASTOR EN ITALIE
   dewey: 945 ALB
   entry_numbers:
   - '3898'
   editor: THORIN // PARIS
   edition_year: 1883
@@ -131472,15 +131326,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2556
   authors:
-  - VERPEAUN J
+  - VERPEAUX,JEAN
   language: fr
   title: NICEPHORE CHOUMNOS
   dewey: 938.3 VER
   entry_numbers:
   - '3896'
   editor: PICARD // PARIS
   edition_year: 1959
@@ -131571,15 +131425,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2558
   authors:
-  - WICART A
+  - WICART,ALEXIS
   language: fr
   title: L'ORATEUR
   dewey: 845 WIC
   entry_numbers:
   - '3894'
   editor: VOX // PARIS
   edition_year: 1935
@@ -132418,15 +132272,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2575
   authors:
-  - VATIN CLAUDE
+  - VATIN,CLAUDE
   language: fr
   title: RECHERCHES SUR LE MARIAGE ET LA CONDITION DE LA FEMME MARIE
   subtitle: AL'EPOUE HELLENISTIOUE
   dewey: 938.18 VAT
   entry_numbers:
   - '3877'
   editor: BICCARD // PARIS
@@ -133179,15 +133033,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2590
   authors:
-  - VAUCHER R-LIGNY J
+  - VAUCHER,ROBERT
+  - LIGNY,JEAN
   language: fr
   title: LE COLOSSE RUSSE
   dewey: 947 VAU
   entry_numbers:
   - '3857'
   editor: NEUCHATEL // BOUDRY
   topics:
@@ -133579,15 +133434,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2598
   authors:
-  - VASILIEV A
+  - VASILIEV,ALEXANDER,ALEXANDROVICH
   language: fr
   title: L'EMPIRE BYZANTIN
   dewey: 938.3 VAS
   entry_numbers:
   - '3849'
   editor: PICARD // PARIS
   edition_year: 1932
@@ -133978,15 +133833,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2606
   authors:
-  - VOJISLAV DJURIC
+  - DJURIC,VOJISLAV
   language: fr
   title: ICONES DE YOUGOSLAVIE
   dewey: 949.7 VOJ
   entry_numbers:
   - '3842'
   editor: NAUCNO DELO // BELGRADE
   edition_year: 1961
@@ -134232,15 +134087,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2611
   authors:
-  - VERNANT JEAN-PIERR
+  - VERNANT,JEAN-PIERRE
   language: fr
   title: PROBLEMES DE LA GUERRE EN GRECE ANCIENNE
   dewey: 938.105 VER
   entry_numbers:
   - '3837'
   editor: MOUTON // PARIS
   edition_year: 1968
@@ -134730,15 +134585,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2621
   authors:
-  - WILL EDOUARD
+  - EDOUARD,WILL
   language: fr
   title: LE MONDE GREC ET L'ORIENT LE SIECLE 510-403
   dewey: 938 WIL
   entry_numbers:
   - '3827'
   editor: UNIVERSITAIRES FRA // PARIS
   edition_year: 1972
@@ -135890,15 +135745,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2644
   authors:
-  - WUILLEUMIER PIERRE
+  - WUILLEUMIER,PIERRE
   language: fr
   title: LE TRESOR DE TARENTE
   dewey: 720 WUI
   entry_numbers:
   - '3808'
   editor: LEROUX // PARIS
   edition_year: 1930
@@ -136642,15 +136497,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2659
   authors:
-  - WILL EDOUARD
+  - EDOUARD,WILL
   language: fr
   title: HISTOIRE POLITIOUE DU MONDE HELLENISTIOUE
   dewey: 938.032 WIL
   entry_numbers:
   - '3794'
   editor: None // NANCY
   edition_year: 1966
@@ -137347,15 +137202,17 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2673
   authors:
-  - WILLE-MOSSE COUKOWSKY
+  - WILL,EDOUARD
+  - MOSSE,CLAUDE
+  - GOUKOWSKY,PAUL
   language: fr
   title: LE MONDE CREG ET L'ORIENT
   dewey: 938 WIL
   entry_numbers:
   - '3781'
   editor: UNIVERSITAIRES // PARIS
   edition_year: 1975
@@ -138046,15 +137903,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2687
   authors:
-  - ALTHEIM F
+  - ALTHEIM,FRANZ
   language: fr
   title: ALEXANDRE ET ASIE
   dewey: 938.174 ALT
   entry_numbers:
   - '3734'
   editor: PAYOT // PARIS
   edition_year: 1954
@@ -138891,20 +138748,19 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2704
   authors:
-  - VRANOUSSIS L
+  - ΒΡΑΝΟΥΣΗΣ,ΛΕΑΝΔΡΟΣ,Ι.
   language: fr
   title: L'HELLENISME POTBYZANTIN ET L'EUROPE
   dewey: 938.301 VRA
-  entry_numbers:
-  - '3753'
+  entry_numbers: []
   editor: LIVRES // None
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΒΥΖΑΝΤΙΟ
   - ΠΗΓΕΣ
   - ΕΥΡΩΠΗ
   - ΧΕΙΡΟΓΡΑΦΑ
@@ -138915,23 +138771,23 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 2704
     1: VRANOUSSIS L                       GAL
     2: L'HELLENISME POTBYZANTIN ET L'EUROPE
     4: 938.301VRA
-    5: '3753'
     8: LIVRES
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
     13: ΒΥΖΑΝΤΙΟ-ΠΗΓΕΣ
     14: ΕΥΡΩΠΗ-ΧΕΙΡΟΓΡΑΦΑ
     15: ΧΕΙΡΟΓΡΑΦΑ-ΕΥΡΩΠΗ
     17: Ο ΜΕΤΑΒΥΖΑΝΤΙΝΟΣ ΕΛΛΗΝΙΣΜΟΣ ΚΑΙ Η ΕΥΡΩΠΗ
     30: ΧΕΙΡΟΓΡΑΦΑ,ΒΙΒΛΙΑ,ΕΝΤΥΠΑ
     3: null
+    5: null
     6: null
     7: null
     9: null
     10: null
     11: null
     16: null
     18: null
@@ -139440,15 +139296,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2715
   authors:
-  - WILL EDOUARD
+  - EDOUARD,WILL
   language: fr
   title: KORINTHIAKA-RECHRCHES SUR L'HISTORIE ET LA CIVILISATION
   dewey: 938.25 WIL
   entry_numbers:
   - '3742'
   editor: BOCCARD // PARIS
   edition_year: 1955
@@ -139493,15 +139349,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2716
   authors:
-  - WUILLEUMIER PIERRE
+  - WUILLEUMIER,PIERRE
   language: fr
   title: TARENTE DES ORIGINES A LA CONOUETE ROMAINE
   dewey: 938.192 WUI
   entry_numbers:
   - '3741'
   editor: BOCCARD // PARIS
   edition_year: 1963
@@ -140505,15 +140361,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2736
   authors:
-  - WALLON HENRI
+  - WALLON,HENRI
   language: fr
   title: HISTOIRE DE L'ESCLAVAGE DANS L'ANTIGUITE
   dewey: 368.75 WAL
   entry_numbers:
   - '3720'
   editor: HACHETTE // PARIS
   edition_year: 1879
@@ -140556,15 +140412,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2737
   authors:
-  - AYMARD ANDRE-AUBOYER JEAN
+  - AYMARD,ANDRE-AUBOYER,JEANNINE
   language: fr
   title: L'ORIENT ET LA GRECE ANTIOUE
   dewey: 938.1 AYM
   entry_numbers:
   - '3719'
   editor: UNIVERSITAIRES // PARIS
   edition_year: 1963
@@ -140659,15 +140515,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2739
   authors:
-  - WEHRLI CLAUDE
+  - WEHRLI,CLAUDE
   language: fr
   title: ANTIGONE ET DEMETRIOS
   dewey: 881.231 WEH
   entry_numbers:
   - '3717'
   editor: DROZ // GENEVE
   edition_year: 1969
@@ -141167,15 +141023,15 @@
   authors:
   - ΓΑΛΑΝΗΣ,ΓΙΩΡΓΟΣ
   language: el
   title: ΨΥΧΟΛΟΓΙΑ ΤΗΣ (ΕΠΙ)ΜΟΡΦΩΣΗΣ ΕΝΗΛΙΚΩΝ
   subtitle: ΘΕΩΡΗΤΙΚΕΣ ΚΑΙ ΠΡΑΚΤΙΚΕΣ ΠΡΟΣΕΓΓΙΣΕΙΣ
   dewey: 136.5 ΓΑΛ
   entry_numbers:
-  - '4092'
+  - '4091'
   editor: ΠΑΠΑΖΗΣΗ // ΑΘΗΝΑ
   edition_year: 1993
   topics:
   - ΨΥΧΟΛΟΓΙΑ
   - ΕΝΗΛΙΚΟΙ
   - ΜΟΡΦΩΣΗ
   has_cd: false
@@ -141183,15 +141039,15 @@
   offprint: false
   original_entry:
     0: 2749
     1: ΓΑΛΑΝΗΣ,ΓΙΩΡΓΟΣ
     2: ΨΥΧΟΛΟΓΙΑ ΤΗΣ (ΕΠΙ)ΜΟΡΦΩΣΗΣ ΕΝΗΛΙΚΩΝ
     3: ΘΕΩΡΗΤΙΚΕΣ ΚΑΙ ΠΡΑΚΤΙΚΕΣ ΠΡΟΣΕΓΓΙΣΕΙΣ
     4: 136.5 ΓΑΛ
-    5: '4092'
+    5: '4091'
     8: ΠΑΠΑΖΗΣΗ
     9: ΑΘΗΝΑ
     10: '1993'
     12: ΨΥΧΟΛΟΓΙΑ-ΕΝΗΛΙΚΟΙ
     13: ΕΝΗΛΙΚΟΙ-ΨΥΧΟΛΟΓΙΑ
     14: ΜΟΡΦΩΣΗ-ΨΥΧΟΛΟΓΙΑ
     6: null
@@ -141362,15 +141218,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2753
   authors:
-  - ΒΑΦΙΑΣ,ΤΑΚΗΣ Γ
+  - ΒΑΦΙΑΣ,ΤΑΚΗΣ,Γ.
   language: el
   title: ΤΟ ΕΡΑΣΙΤΕΧΝΙΚΟ ΘΕΑΤΡΟ ΣΤΗΝ ΑΡΤΑ
   dewey: 886.2 ΒΑΦ
   entry_numbers:
   - '4086'
   - '4087'
   editor: None // ΑΘΗΝΑ
@@ -141979,15 +141835,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2765
   authors:
-  - ΑΡΓΥΡΟΠΟΥΛΟΣ,Π
+  - ΑΡΓΥΡΟΠΟΥΛΟΣ,ΠΕΡΙΚΛΗΣ
   language: el
   title: Ο ΜΑΚΕΔΟΝΙΚΟΣ ΑΓΩΝΑΣ
   subtitle: ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ
   dewey: 938.664 ΑΡΓ
   entry_numbers:
   - '3022'
   editor: Ι.Μ.Χ.Α // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -145284,15 +145140,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2830
   authors:
-  - ΒΟΙΝΤ,ΡΟΜΠΕΡΤ
+  - BOYD,ROBERT
   language: el
   title: ΜΠΟΡΟΥΜΕ ΝΑ ΓΝΩΡΙΣΟΥΜΕ ΤΟΥ ΘΕΟ
   dewey: 231 ΒΟΙ
   entry_numbers:
   - '543'
   translators:
   - ΦΙΛΟΣ,ΣΠΥΡΟΣ
@@ -145690,15 +145546,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2838
   authors:
-  - ΑΡΝΕΛΛΟΣ,ΙΩΑΝΝΗΣ Γ
+  - ΑΡΝΕΛΛΟΣ,ΙΩΑΝΝΗΣ,Γ.
   language: el
   title: Ο ΘΕΟΣ ΕΝ ΤΗ ΕΠΙΣΤΗΜΗ
   dewey: 231 ΑΡΝ
   entry_numbers:
   - '4108'
   editor: ΒΟΥΡΝΑ // CHICAGO
   pages: 168
@@ -145739,15 +145595,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2839
   authors:
-  - ΒΑΣΙΛΟΠΟΥΛΟΣ,ΧΑΡΑΛΑΜΠΟΣ
+  - ΒΑΣΙΛΟΠΟΥΛΟΣ,ΑΡΧΙΜΑΝΔΡΙΤΗΣ ΧΑΡΑΛΑΜΠΟΣ
   language: el
   title: Ο ΟΙΚΟΥΜΕΝΙΣΜΟΣ
   subtitle: ΧΩΡΙΣ ΜΑΣΚΑ
   dewey: 289 ΒΑΣ
   entry_numbers:
   - '3047'
   editor: None // ΑΘΗΝΑ
@@ -149123,15 +148979,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2905
   authors:
-  - ΒΡΑΝΟΠΟΥΛΟΣ,ΕΠΑΜ
+  - ΒΡΑΝΟΠΟΥΛΟΣ,ΕΠΑΜΕΙΝΩΝΔΑΣ,Α.
   language: el
   title: Η ΚΑΤΑ ΤΩΝ ΡΩΜΑΙΩΝ ΕΚΣΤΡΑΤΕΙΑ ΤΟΥ ΑΝΤΙΟΧΟΥ ΤΟΥ Γ'ΕΙΣ ΤΗΝ
   subtitle: ΕΛΛΑΔΑ
   dewey: 938.19 ΒΡΑ
   entry_numbers:
   - '4174'
   editor: ΣΠΑΝΟΠΟΥΛΟΥ // ΑΘΗΝΑ
@@ -149176,15 +149032,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2906
   authors:
-  - ΒΡΑΝΟΠΟΥΛΟΣ,ΕΠΑΜ
+  - ΒΡΑΝΟΠΟΥΛΟΣ,ΕΠΑΜΕΙΝΩΝΔΑΣ,Α.
   language: el
   title: ΕΛΛΗΝΙΣΤΙΚΗ ΧΑΛΚΙΣ
   subtitle: ΣΥΜΒΟΛΗ ΕΙΣ ΤΗΝ ΙΣΤΟΡΙΑΝ ΤΩΝ ΕΛΛΗΝΙΣΤΙΚΩΝ ΧΡΟΝΩΝ ΤΗΣ ΧΑΛΚΙΔΟ
   dewey: 938.915 ΒΡΑ
   entry_numbers:
   - '4172'
   editor: ΣΠΑΝΟΠΟΥΛΟΥ // ΑΘΗΝΑ
@@ -149534,15 +149390,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2913
   authors:
-  - ΒΕΛΛΙΑΝΙΤΟΣ,Θ
+  - ΒΕΛΛΙΑΝΙΤΗΣ,ΘΕΟΔΩΡΟΣ
   language: el
   title: ΠΟΛΥΛΑΣ,ΜΑΡΚΟΡΑΣ ΚΑΙ Η ΣΧΟΛΗ ΤΗΣ ΚΕΡΚΥΡΑΣ
   dewey: 889.09 ΒΕΛ
   entry_numbers:
   - '4195'
   editor: None // ΑΘΗΝΑ
   edition_year: 1970
@@ -149900,15 +149756,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 2920
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: ΤΟ ΠΑΙΔΙ ΚΑΙ Η ΘΡΗΣΚΕΥΤΙΚΗ ΔΙΑΠΑΙΔΑΓΩΓΗΣΙΣ
   dewey: 136.73 ΑΣΠ
   entry_numbers:
   - '597'
   editor: None // ΑΘΗΝΑ
   edition_year: 1962
@@ -149950,15 +149806,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2921
   authors:
-  - ΑΝΤΕΡΣΟΝ,
+  - ANDERSON,CHARLES
   language: el
   title: ΠΡΟΣ ΜΙΑ ΝΕΑ ΚΟΙΝΩΝΙΟΛΟΓΙΑ
   dewey: 301 ΑΝΤ
   entry_numbers:
   - '4161'
   editor: ΠΑΠΑΖΗΣΗ // ΑΘΗΝΑ
   edition_year: 1986
@@ -150056,16 +149912,15 @@
     30: null
 - dbase_number: 2923
   authors:
   - ΧΑΜΠΣΟΝ,ΝΟΡΜΑΝ
   language: el
   title: Ο ΔΙΑΦΩΤΙΣΜΟΣ
   dewey: 938.482 ΧΑΜ
-  entry_numbers:
-  - '4152'
+  entry_numbers: []
   translators:
   - ΜΠΕΧΛΙΚΑΛΗ,ΔΗΜΗΤΡΑ
   editor: ΠΑΠΑΖΗΣΗ // ΑΘΗΝΑ
   pages: 326
   topics:
   - ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   - ΔΙΑΦΩΤΙΣΜΟΣ
@@ -150074,24 +149929,24 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 2923
     1: ΧΑΜΠΣΟΝ,ΝΟΡΜΑΝ
     2: Ο ΔΙΑΦΩΤΙΣΜΟΣ
     4: 938.482ΧΑΜ
-    5: '4152'
     6: ΜΠΕΧΛΙΚΑΛΗ ΔΗΜΗΤΡΑ
     8: ΠΑΠΑΖΗΣΗ
     9: ΑΘΗΝΑ
     10: Χ.Χ
     11: 326Σ
     12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΙΑΦΩΤΙΣΜΟΣ
     13: ΔΙΑΦΩΤΙΣΜΟΣ
     17: HAMPSON NORMAN
     3: null
+    5: null
     7: null
     14: null
     15: null
     16: null
     18: null
     19: null
     20: null
@@ -150417,17 +150272,16 @@
     29: null
     30: null
 - dbase_number: 2930
   authors:
   - ΠΕΤΣΚΟΣ,ΧΑΡΑΛΑΜΠΟΣ
   language: el
   title: ΔΙΨΑ ΖΩΗΣ
-  dewey: 889 ΠΕΤ
-  entry_numbers:
-  - '5744'
+  dewey: 889.21 ΠΕΤ
+  entry_numbers: []
   editor: None // ΑΘΗΝΑ
   edition_year: 1976
   pages: 245
   topics:
   - ΣΥΓΧΡΟΝΟ ΚΟΙΝΩΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
   - ΣΥΓΧΡΟΝΗ ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΜΥΘΙΣΤΟΡΗΜΑ
@@ -150435,23 +150289,23 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 2930
     1: ΠΕΤΣΚΟΣ,ΧΑΡΑΛΑΜΠΟΣ
     2: ΔΙΨΑ ΖΩΗΣ
-    4: 889ΠΕΤ
-    5: '5744'
+    4: 889.21ΠΕΤ
     9: ΑΘΗΝΑ
     10: '1976'
     11: 245Σ
     12: ΣΥΓΧΡΟΝΟ ΚΟΙΝΩΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΣΥΓΧΡΟΝΗ ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΜΥΘΙΣΤΟΡΗΜΑ-ΛΟΓΟΤΕΧΝΙΑ
     3: null
+    5: null
     6: null
     7: null
     8: null
     15: null
     16: null
     17: null
     18: null
@@ -150470,30 +150324,30 @@
 - dbase_number: 2931
   authors:
   - ΜΠΑΛΟΥΜΗΣ,ΕΠΑΜΕΙΝΩΝΔΑΣ
   language: el
   title: ΓΙΑ ΤΗΝ ΚΟΛΧΙΔΑ
   dewey: 889.21 ΜΠΑ
   entry_numbers:
-  - '5869'
+  - '5684'
   editor: ΚΕΔΡΟΣ // ΑΘΗΝΑ
   edition_year: 1963
   pages: 125
   topics:
   - ΣΥΓΧΡΟΝΗ ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 2931
     1: ΜΠΑΛΟΥΜΗΣ,ΕΠΑΜΕΙΝΩΝΔΑΣ
     2: ΓΙΑ ΤΗΝ ΚΟΛΧΙΔΑ
     4: 889.21ΜΠΑ
-    5: '5869'
+    5: '5684'
     8: ΚΕΔΡΟΣ
     9: ΑΘΗΝΑ
     10: '1963'
     11: 125Σ
     12: ΣΥΓΧΡΟΝΗ ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     3: null
@@ -150671,15 +150525,15 @@
 - dbase_number: 2935
   authors:
   - ΖΑΔΕΣ,ΔΗΜΟΣΘΕΝΗΣ
   language: el
   title: ΚΑΤΩ ΕΚΕΙ ΣΤΟΥΣ ΚΟΡΣΕΟΥΣ
   dewey: 889.21 ΖΑΔ
   entry_numbers:
-  - '2063'
+  - '5536'
   editor: ΜΑΥΡΙΔΗΣ // None
   edition_year: 1958
   pages: 99
   topics:
   - ΣΥΓΧΡΟΝΗ ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΝΟΥΒΕΛΕΣ
@@ -150687,15 +150541,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 2935
     1: ΖΑΔΕΣ,ΔΗΜΟΣΘΕΝΗΣ
     2: ΚΑΤΩ ΕΚΕΙ ΣΤΟΥΣ ΚΟΡΣΕΟΥΣ
     4: 889.21ΖΑΔ
-    5: '2063'
+    5: '5536'
     8: ΜΑΥΡΙΔΗΣ
     10: '1958'
     11: 99Σ
     12: ΣΥΓΧΡΟΝΗ ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΝΟΥΒΕΛΑ
     3: null
@@ -151015,15 +150869,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2942
   authors:
-  - ΒΟΥΤΥΡΑ,ΔΗΜΟΣΘΕΝΗ
+  - ΒΟΥΤΥΡΑΣ,ΔΗΜΟΣΘΕΝΗΣ
   language: el
   title: ΑΡΓΟ ΞΗΜΕΡΩΜΑ
   dewey: 889.21 ΒΟΥ
   entry_numbers:
   - '5456'
   editor: ΚΟΤΣΙΩΡΗ // ΑΘΗΝΑ
   edition_year: 1950
@@ -153001,33 +152855,33 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 2982
   authors:
-  - ΒΑΝΤΖΙΑΣ,ΓΙΑΝΝΗΣ
+  - ΒΑΤΖΙΑΣ,ΓΙΑΝΝΗΣ
   title: ΠΕΡIΠΛΑΝΩΜΕΝΟΙ
-  dewey: 889 ΒΑΤ
+  dewey: 889.21 ΒΑΤ
   entry_numbers:
   - '4338'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 1983
   pages: 172
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 2982
-    1: ΒΑΝΤΖΙΑΣ,ΓΙΑΝΝΗΣ
+    1: ΒΑΤΖΙΑΣ,ΓΙΑΝΝΗΣ
     2: ΠΕΡIΠΛΑΝΩΜΕΝΟΙ
-    4: 889ΒΑΤ
+    4: 889.21ΒΑΤ
     5: '4338'
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: '1983'
     11: 172Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -153054,30 +152908,30 @@
 - dbase_number: 2983
   authors:
   - ΙΕΡΩΝΥΜΙΔΗΣ,ΛΟΥΛΑΣ
   language: el
   title: ΜΙΑ ΚΑΠΟΙΑ ΕΥΑ
   dewey: 889.21 ΙΕΡ
   entry_numbers:
-  - '5743'
+  - '6083'
   editor: ΑΛΚΑΙΟΣ // ΑΘΗΝΑ
   edition_year: 1975
   pages: 117
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 2983
     1: ΙΕΡΩΝΥΜΙΔΗΣ,ΛΟΥΛΑΣ
     2: ΜΙΑ ΚΑΠΟΙΑ ΕΥΑ
     4: 889.21ΙΕΡ
-    5: '5743'
+    5: '6083'
     8: ΑΛΚΑΙΟΣ
     9: ΑΘΗΝΑ
     10: '1975'
     11: 117Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΜΥΘΙΣΤΟΡΗΜΑΤΑ
@@ -153943,15 +153797,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3001
   authors:
-  - ΒΟΒΟΛΙΝΗ ΠΟΛΥΒΙΟΥ
+  - ΒΟΒΟΛΙΝΗΣ,ΠΟΛΥΒΙΟΣ
   language: el
   title: ΣΕ ΚΕΙΝΗ ΤΗΝ ΑΚΡΗ ΤΗΣ ΠΟΛΗΣ
   dewey: 889.21 ΒΟΒ
   entry_numbers:
   - '10264'
   editor: None // ΑΘΗΝΑ
   pages: 240
@@ -154294,30 +154148,30 @@
 - dbase_number: 3008
   authors:
   - ΕΥΑΓΓΕΛΟΥ,ΑΝΕΣΤΗΣ
   language: el
   title: ΤΟ ΞΕΝΟΔΟΧΕΙΟ ΚΑΙ ΤΟ ΣΠΙΤΙ
   dewey: 889.21 ΕΥΑ
   entry_numbers:
-  - '2355'
+  - '5531'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1966
   pages: 38
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΠΕΖΟΓΡΑΦΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3008
     1: ΕΥΑΓΓΕΛΟΥ,ΑΝΕΣΤΗΣ
     2: ΤΟ ΞΕΝΟΔΟΧΕΙΟ ΚΑΙ ΤΟ ΣΠΙΤΙ
     4: 889.21ΕΥΑ
-    5: '2355'
+    5: '5531'
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '1966'
     11: 38Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΗΜΑ
     13: ΠΕΖΟΓΡΑΦΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΕΖΟΓΡΑΦΗΜΑ
     3: null
@@ -155730,30 +155584,30 @@
 - dbase_number: 3037
   authors:
   - ΚΑΡΑΒΙΑ-ΧΑΤΖΟΠΟΥΛΟΥ,ΛΕΙΑ
   language: el
   title: Ο ΔΡΟΜΟΣ ΤΟΥ ΘΥΜΩΜΕΝΟΥ ΠΟΤΑΜΟΥ
   dewey: 889.21 ΚΑΡ
   entry_numbers:
-  - '5629'
+  - '5622'
   editor: None // ΑΘΗΝΑ
   edition_year: 1963
   pages: 110
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΔΙΗΓΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3037
     1: ΚΑΡΑΒΙΑ-ΧΑΤΖΟΠΟΥΛΟΥ,ΛΕΙΑ
     2: Ο ΔΡΟΜΟΣ ΤΟΥ ΘΥΜΩΜΕΝΟΥ ΠΟΤΑΜΟΥ
     4: 889.21ΚΑΡ
-    5: '5629'
+    5: '5622'
     9: ΑΘΗΝΑ
     10: '1963'
     11: 110Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
     13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΔΙΗΓΗΜΑΤΑ
     3: null
@@ -156126,15 +155980,15 @@
   authors:
   - ΠΟΛΙΤΗ,ΚΟΣΜΑ
   language: el
   title: ΣΤΟΥ ΧΑΤΖΗΦΡΑΓΚΟΥ
   subtitle: ΤΑ ΣΑΡΑΝΤΑ ΧΡΟΝΙΑ ΜΙΑΣ ΧΑΜΕΝΗΣ ΠΟΛΙΤΕΙΑΣ
   dewey: 889.21 ΠΟΛ
   entry_numbers:
-  - '2036'
+  - '5784'
   editor: ΚΑΡΑΒΙΑ // ΑΘΗΝΑ
   edition_year: 1963
   pages: 318
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
@@ -156142,15 +155996,15 @@
   offprint: false
   original_entry:
     0: 3045
     1: ΠΟΛΙΤΗ,ΚΟΣΜΑ
     2: ΣΤΟΥ ΧΑΤΖΗΦΡΑΓΚΟΥ
     3: ΤΑ ΣΑΡΑΝΤΑ ΧΡΟΝΙΑ ΜΙΑΣ ΧΑΜΕΝΗΣ ΠΟΛΙΤΕΙΑΣ
     4: 889.21ΠΟΛ
-    5: '2036'
+    5: '5784'
     8: ΚΑΡΑΒΙΑ
     9: ΑΘΗΝΑ
     10: '1963'
     11: 318Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΜΥΘΙΣΤΟΡΗΜΑΤΑ
@@ -156723,30 +156577,30 @@
 - dbase_number: 3057
   authors:
   - ΝΑΚΟΥ,ΛΙΛΙΚΑ
   language: el
   title: ΓΙΑ ΜΙΑ ΚΑΙΝΟΥΡΓΙΑ ΖΩΗ
   dewey: 889.21 ΝΑΚ
   entry_numbers:
-  - '2305'
+  - '2306'
   editor: None // ΑΘΗΝΑ
   edition_year: 1960
   pages: 342
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΡΟΜΑΝΤΖΟ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3057
     1: ΝΑΚΟΥ,ΛΙΛΙΚΑ
     2: ΓΙΑ ΜΙΑ ΚΑΙΝΟΥΡΓΙΑ ΖΩΗ
     4: 889.21ΝΑΚ
-    5: '2305'
+    5: '2306'
     9: ΑΘΗΝΑ
     10: '1960'
     11: 342Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΡΟΜΑΝΤΖΟ
     13: ΡΟΜΑΝΤΖΟ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΡΟΜΑΝΤΖΟ
     3: null
@@ -157214,31 +157068,31 @@
     29: null
     30: null
 - dbase_number: 3067
   authors:
   - ΚΩΣΤΑΡΑ,ΒΑΣΙΛΗΣ
   language: el
   title: Η ΚΡΑΥΓΗ ΤΟΥ ΗΛΙΟΥ
-  dewey: 889 ΚΩΣ
+  dewey: 889.21 ΚΩΣ
   entry_numbers:
-  - '4359'
+  - '4353'
   editor: ΑΧΑΙΚΕΣ ΕΚΔΟΣΕΙΣ // ΠΑΤΡΑ
   pages: 177
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3067
     1: ΚΩΣΤΑΡΑ,ΒΑΣΙΛΗΣ
     2: Η ΚΡΑΥΓΗ ΤΟΥ ΗΛΙΟΥ
-    4: 889ΚΩΣ
-    5: '4359'
+    4: 889.21ΚΩΣ
+    5: '4353'
     8: ΑΧΑΙΚΕΣ ΕΚΔΟΣΕΙΣ
     9: ΠΑΤΡΑ
     11: 177Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΜΥΘΙΣΤΟΡΗΜΑ
     3: null
@@ -157412,29 +157266,29 @@
 - dbase_number: 3071
   authors:
   - ΕΛΕΥΘΕΡΙΑΔΗΣ,ΜΙΜΗΣ
   language: el
   title: ΑΜΑΡΤΩΛΗ ΓΗ
   dewey: 889.21 ΕΛΕ
   entry_numbers:
-  - '5062'
+  - '5532'
   edition_year: 1977
   pages: 177
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΔΙΗΓΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3071
     1: ΕΛΕΥΘΕΡΙΑΔΗΣ,ΜΙΜΗΣ
     2: ΑΜΑΡΤΩΛΗ ΓΗ
     4: 889.21ΕΛΕ
-    5: '5062'
+    5: '5532'
     10: '1977'
     11: 177Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
     13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΔΙΗΓΗΜΑΤΑ
     3: null
     6: null
@@ -158047,15 +157901,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3084
   authors:
-  - ΑΜΠΟΤ,Γ-Ν
+  - ΑΜΠΟΤ,ΓΟΥΛΙΕΛΜΟΣ,Ν.
   language: el
   title: ΓΗ ΚΑΙ ΝΕΡΟ
   dewey: 889.21 ΑΜΠ
   entry_numbers:
   - '1243'
   edition: Β
   editor: ΦΕΞΗ // ΑΘΗΝΑ
@@ -158353,30 +158207,30 @@
 - dbase_number: 3090
   authors:
   - ΑΡΒΑΝΙΤΗΣ,ΔΙΟΝΥΣΗΣ
   language: el
   title: ΑΝΑΜΝΗΣΕΙΣ ΑΠΟ ΤΑ ΧΡΟΝΙΑ ΕΚΕΙΝΑ
   dewey: 889.21 ΑΡΒ
   entry_numbers:
-  - '2356'
+  - '5432'
   editor: None // ΑΘΗΝΑ
   edition_year: 1969
   pages: 94
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΔΙΗΓΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3090
     1: ΑΡΒΑΝΙΤΗΣ,ΔΙΟΝΥΣΗΣ
     2: ΑΝΑΜΝΗΣΕΙΣ ΑΠΟ ΤΑ ΧΡΟΝΙΑ ΕΚΕΙΝΑ
     4: 889.21ΑΡΒ
-    5: '2356'
+    5: '5432'
     9: ΑΘΗΝΑ
     10: '1969'
     11: 94Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
     13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΔΙΗΓΗΜΑΤΑ
     3: null
@@ -158648,40 +158502,39 @@
     29: null
     30: null
 - dbase_number: 3096
   authors:
   - ΜΟΣΚΟΒΗ,ΒΑΣΙΛΗ
   language: el
   title: Η ΑΥΛΗ ΤΗΣ ΜΗΤΕΡΑΣ
-  dewey: 889 ΜΟΣ
-  entry_numbers:
-  - '2153'
+  dewey: 889.21 ΜΟΣ
+  entry_numbers: []
   editor: ΜΑΥΡΙΔΗΣ // ΑΘΗΝΑ
   edition_year: 1958
   pages: 270
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΔΙΗΓΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3096
     1: ΜΟΣΚΟΒΗ,ΒΑΣΙΛΗ
     2: Η ΑΥΛΗ ΤΗΣ ΜΗΤΕΡΑΣ
-    4: 889ΜΟΣ
-    5: '2153'
+    4: 889.21ΜΟΣ
     8: ΜΑΥΡΙΔΗΣ
     9: ΑΘΗΝΑ
     10: '1958'
     11: 270Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
     13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΔΙΗΓΗΜΑΤΑ
     3: null
+    5: null
     6: null
     7: null
     15: null
     16: null
     17: null
     18: null
     19: null
@@ -158941,15 +158794,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3102
   authors:
-  - ΒΑΣΙΛΙΚΟΥ,ΒΑΣΙΛΗ
+  - ΒΑΣΙΛΙΚΟΣ,ΒΑΣΙΛΗΣ
   language: el
   title: ΟΙ ΦΩΤΟΓΡΑΦΙΕΣ
   dewey: 889.21 ΒΑΣ
   entry_numbers:
   - '5467'
   editor: ΕΣΤΙΑ // None
   pages: 162
@@ -159043,15 +158896,15 @@
 - dbase_number: 3104
   authors:
   - ΣΚΑΡΙΜΠΑ,ΓΙΑΝΝΗ
   language: el
   title: Η ΜΑΘΗΤΕΥΟΜΕΝΗ ΤΩΝ ΤΑΚΟΥΝΙΩΝ
   dewey: 889 ΣΚΑ
   entry_numbers:
-  - '2211'
+  - '10269'
   editor: ΔΙΦΡΟΣ // ΑΘΗΝΑ
   edition_year: 1960
   pages: 152
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΔΙΗΓΗΜΑ
   copies: 2
@@ -159059,15 +158912,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 3104
     1: ΣΚΑΡΙΜΠΑ,ΓΙΑΝΝΗ
     2: Η ΜΑΘΗΤΕΥΟΜΕΝΗ ΤΩΝ ΤΑΚΟΥΝΙΩΝ
     4: 889ΣΚΑ
-    5: '2211'
+    5: '10269'
     8: ΔΙΦΡΟΣ
     9: ΑΘΗΝΑ
     10: '1960'
     11: 152Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
     13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΔΙΗΓΗΜΑΤΑ
@@ -159385,15 +159238,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3111
   authors:
-  - ΑΜΠΑΤΖΟΓΛΟΥ,ΠΕΤΡΟΥ
+  - ΑΜΠΑΤΖΟΓΛΟΥ,ΠΕΤΡΟΣ
   language: el
   title: ΙΣΟΡΡΟΠΙΑ ΤΡΟΜΟΥ
   dewey: 889.21 ΑΜΠ
   entry_numbers:
   - '5420'
   editor: ΦΕΞΗ // ΑΘΗΝΑ
   edition_year: 1964
@@ -160132,15 +159985,15 @@
     29: null
     30: null
 - dbase_number: 3126
   authors:
   - ΜΑΝΙΑΤΑΚΟΥ,ΓΙΩΡΓΟΥ
   language: el
   title: ΤΟ ΣΥΝΝΕΦΟ ΔΕΝ ΕΦΕΡΕ ΒΡΟΧΗ
-  dewey: 889 ΜΑΝ
+  dewey: 889.21 ΜΑΝ
   entry_numbers:
   - '2273'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 1961
   pages: 241
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -160148,15 +160001,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3126
     1: ΜΑΝΙΑΤΑΚΟΥ,ΓΙΩΡΓΟΥ
     2: ΤΟ ΣΥΝΝΕΦΟ ΔΕΝ ΕΦΕΡΕ ΒΡΟΧΗ
-    4: 889ΜΑΝ
+    4: 889.21ΜΑΝ
     5: '2273'
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: '1961'
     11: 241Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -160676,15 +160529,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3137
   authors:
-  - ΒΛΑΜΗ,ΕΥΗ
+  - ΒΛΑΜΗ,ΕΥΑ
   language: el
   title: ΣΤΟΝ ΑΡΓΑΛΕΙΟ ΤΟΥ ΦΕΓΓΑΡΙΟΥ
   dewey: 889.21 ΒΛΑ
   entry_numbers:
   - '2024'
   editor: ΦΕΞΗ // ΑΘΗΝΑ
   edition_year: 1963
@@ -160928,29 +160781,29 @@
 - dbase_number: 3142
   authors:
   - ΦΛΩΡΟΥ,ΠΑΥΛΟΥ
   language: el
   title: ΑΠΟΙΚΟΙ
   dewey: 889.21 ΦΛΩ
   entry_numbers:
-  - '4701'
+  - '5901'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   pages: 414
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΔΙΗΓΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3142
     1: ΦΛΩΡΟΥ,ΠΑΥΛΟΥ
     2: ΑΠΟΙΚΟΙ
     4: 889.21ΦΛΩ
-    5: '4701'
+    5: '5901'
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     11: 414Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
     13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΔΙΗΓΗΜΑΤΑ
     3: null
@@ -161658,15 +161511,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3157
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: Η ΧΩΡΑ ΤΩΝ ΑΔΑΜΑΝΤΩΝ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '5468'
   translators:
   - ΚΑΖΑΝΤΖΑΚΗ,Ν.
@@ -161859,15 +161712,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3161
   authors:
-  - ΑΝΑΓΝΩΣΤΟΥ,ΤΑΣΟΣ.Γ
+  - ΑΝΑΓΝΩΣΤΟΥ,ΤΑΣΟΣ,Γ.
   language: el
   title: Ο ΚΑΘΡΕΦΤΗΣ ΚΑΙ ΤΟ ΠΡΟΣΩΠΟ
   dewey: 889.21 ΑΝΑ
   entry_numbers:
   - '5428'
   editor: ΝΕΑ ΣΚΕΨΗ // ΑΘΗΝΑ
   edition_year: 1976
@@ -162449,15 +162302,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3173
   authors:
-  - ΒΡΕΛΛΗ,ΓΕΩΡΓΙΟΥ
+  - ΒΡΕΛΛΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΓΕΝΙΚΗ ΘΕΩΡΗΣΗ ΣΤΗΝ ΠΟΙΗΣΗ ΤΟΥ ΘΑΛΗ ΡΗΤΟΡΙΔΗ
   dewey: 889.21 ΒΡΕ
   entry_numbers:
   - '5464'
   editor: ΒΩΜΟΥ ΤΕΧΝΗΣ // ΡΩΜΗ
   edition_year: 1982
@@ -162895,15 +162748,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3182
   authors:
-  - ΑΜΠΟΤ,Γ.Ν
+  - ΑΜΠΟΤ,ΓΟΥΛΙΕΛΜΟΣ,Ν.Ν
   language: el
   title: ΔΗΜΗΤΡΙΟΣ ΓΑΒΡΙΗΛ
   subtitle: ΧΡΟΝΙΚΟ ΤΟΥ ΞΕΝΗΤΕΜΟΥ
   dewey: 889.21 ΑΜΠ
   entry_numbers:
   - '5427'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
@@ -163690,15 +163543,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3198
   authors:
-  - ΑΜΠΟΤ,Γ.Ν
+  - ΑΜΠΟΤ,ΓΟΥΛΙΕΛΜΟΣ,Ν.Ν
   language: el
   title: ΕΓΩ Ο ΝΟΜΟΣ
   dewey: 889.21 ΑΜΠ
   entry_numbers:
   - '5421'
   editor: ΤΟ ΕΛΛΗΝΙΚΟ ΒΙΒΛΙΟ // ΑΘΗΝΑ
   edition_year: 1977
@@ -163788,15 +163641,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3200
   authors:
-  - ΒΟΥΝΑ,ΧΡΗΣΤΟΥ
+  - ΒΟΥΝΑΣ,ΧΡΗΣΤΟΣ
   language: el
   title: ΕΥΘΥΜΑ ΚΕΦΑΛΟΝΙΤΙΚΑ ΑΦΗΓΗΜΑΤΑ
   dewey: 889.21 ΒΟΥ
   entry_numbers:
   - '5461'
   editor: ΦΑΝΟΣ ΤΗΣ ΚΕΦΑΛΟΝΙΑΣ // ΠΑΤΡΑ
   edition_year: 1965
@@ -163836,46 +163689,36 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3201
-  authors:
-  - ΒΑΤΖΙΑΣ ΓΙΑΝΝΗΣ
-  language: el
-  title: ΠΕΡΙΠΛΑΝΩΜΕΝΟΙ
-  dewey: 889.21 ΒΑΤ
-  entry_numbers:
-  - '4338'
-  editor: ΕΣΤΙΑ // ΑΘΗΝΑ
-  edition_year: 1983
-  pages: 172
-  topics:
-  - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
-  - ΜΥΘΙΣΤΟΡΗΜΑ
+  authors: []
+  entry_numbers: []
+  topics: []
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3201
-    1: ΒΑΤΖΙΑΣ ΓΙΑΝΝΗΣ
-    2: ΠΕΡΙΠΛΑΝΩΜΕΝΟΙ
-    4: 889.21ΒΑΤ
-    5: '4338'
-    8: ΕΣΤΙΑ
-    9: ΑΘΗΝΑ
-    10: '1983'
-    11: 172Σ
-    12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
-    13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
-    14: ΜΥΘΙΣΤΟΡΗΜΑ
+    1: null
+    2: null
     3: null
+    4: null
+    5: null
     6: null
     7: null
+    8: null
+    9: null
+    10: null
+    11: null
+    12: null
+    13: null
+    14: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -163988,38 +163831,39 @@
     30: null
 - dbase_number: 3204
   authors:
   - ΡΕΝΟΣ
   language: el
   title: ΠΥΡΑΜΙΔΑ 67
   dewey: 889.21 ΡΕΝ
-  entry_numbers: []
+  entry_numbers:
+  - '5028'
   editor: ΚΟΛΛΑΡΟΣ // ΑΘΗΝΑ
   edition_year: 1950
   pages: 320
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΔΙΗΓΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3204
     1: ΡΕΝΟΣ
     2: ΠΥΡΑΜΙΔΑ 67
     4: 889.21ΡΕΝ
+    5: '5028'
     8: ΚΟΛΛΑΡΟΣ
     9: ΑΘΗΝΑ
     10: '1950'
     11: 320Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
     13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΔΙΗΓΗΜΑΤΑ
     3: null
-    5: null
     6: null
     7: null
     15: null
     16: null
     17: null
     18: null
     19: null
@@ -164284,30 +164128,30 @@
 - dbase_number: 3210
   authors:
   - ΖΑΔΕ,ΔΗΜΟΣΘΕΝΗΣ
   language: el
   title: ΓΙΑ ΣΜΕΡΝΕΣ
   dewey: 889.21 ΖΑΔ
   entry_numbers:
-  - '5892'
+  - '5529'
   editor: ΤΡΙΦΥΛΙΑΚΗ ΕΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 1977
   pages: 133
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΔΙΗΓΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3210
     1: ΖΑΔΕ,ΔΗΜΟΣΘΕΝΗΣ
     2: ΓΙΑ ΣΜΕΡΝΕΣ
     4: 889.21ΖΑΔ
-    5: '5892'
+    5: '5529'
     8: ΤΡΙΦΥΛΙΑΚΗ ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: '1977'
     11: 133Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
     13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΔΙΗΓΗΜΑΤΑ
@@ -164728,30 +164572,30 @@
 - dbase_number: 3219
   authors:
   - ΣΑΡΑΝΤΗ,ΓΑΛΑΤΕΙΑ
   language: el
   title: ΠΑΣΧΑΛΙΕΣ
   dewey: 889.21 ΣΑΡ
   entry_numbers:
-  - '5825'
+  - '5824'
   editor: ΑΛΦΑ // ΑΘΗΝΑ
   edition_year: 1949
   pages: 245
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3219
     1: ΣΑΡΑΝΤΗ,ΓΑΛΑΤΕΙΑ
     2: ΠΑΣΧΑΛΙΕΣ
     4: 889.21ΣΑΡ
-    5: '5825'
+    5: '5824'
     8: ΑΛΦΑ
     9: ΑΘΗΝΑ
     10: '1949'
     11: 245Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΜΥΘΙΣΤΟΡΗΜΑΤΑ
@@ -166710,37 +166554,38 @@
     30: null
 - dbase_number: 3259
   authors:
   - ΣΚΑΡΟΥ,ΖΗΣΗ
   language: el
   title: ΤΟ ΤΑΞΙΔΙ ΤΗΣ ΦΙΛΙΑΣ
   dewey: 889.21 ΣΚΑ
-  entry_numbers: []
+  entry_numbers:
+  - '22165'
   editor: None // ΑΘΗΝΑ
   edition_year: 1956
   pages: 232
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΔΙΗΓΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3259
     1: ΣΚΑΡΟΥ,ΖΗΣΗ
     2: ΤΟ ΤΑΞΙΔΙ ΤΗΣ ΦΙΛΙΑΣ
     4: 889.21ΣΚΑ
+    5: '22165'
     9: ΑΘΗΝΑ
     10: '1956'
     11: 232Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
     13: ΔΙΗΓΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΔΙΗΓΗΜΑΤΑ
     3: null
-    5: null
     6: null
     7: null
     8: null
     15: null
     16: null
     17: null
     18: null
@@ -167006,30 +166851,30 @@
 - dbase_number: 3265
   authors:
   - ΜΗΤΡΟΠΟΥΛΟΥ,ΚΩΣΤΟΥΛΑΣ
   language: el
   title: ΑΡΘΡΟ Νο 22
   dewey: 889.21 ΜΗΤ
   entry_numbers:
-  - '5969'
+  - '5696'
   editor: ΜΙΝΩΑΣ // ΑΘΗΝΑ
   pages: 220
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΔΙΗΓΗΜΑ
   copies: 2
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3265
     1: ΜΗΤΡΟΠΟΥΛΟΥ,ΚΩΣΤΟΥΛΑΣ
     2: ΑΡΘΡΟ Νο 22
     4: 889.21ΜΗΤ
-    5: '5969'
+    5: '5696'
     8: ΜΙΝΩΑΣ
     9: ΑΘΗΝΑ
     11: 220Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
     13: ΔΙΗΓΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΔΙΗΓΗΜΑΤΑ
     17: 2 ΑΝΤΙΤΥΠΑ
@@ -167443,15 +167288,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3274
   authors:
-  - ΒΟΛΑΝΑΚΗ,ΛΑΜΠΗ
+  - ΒΟΛΑΝΑΚΗΣ,ΛΑΜΠΗΣ
   language: el
   title: '...ΕΠΙ ΓΗΣ ΕΙΡΗΝΗ...'
   dewey: 889.21 ΒΟΛ
   entry_numbers:
   - '5454'
   editor: ΓΡΑΜΜΗ // ΑΘΗΝΑ
   edition_year: 1977
@@ -168526,15 +168371,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3296
   authors:
-  - ΒΑΛΕΤΑΣ,Γ.
+  - ΒΑΛΕΤΑΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΤΗΣ ΡΩΜΙΟΣΥΝΗΣ
   dewey: 889.21 ΒΑΛ
   entry_numbers:
   - '1011'
   editor: ΠΗΓΗ // ΑΘΗΝΑ
   edition_year: 1976
@@ -168579,38 +168424,37 @@
     30: null
 - dbase_number: 3297
   authors:
   - ΡΩ-ΣΙΓΜΑ,ΖΗΤΑ
   language: el
   title: ΣΤΑ ΣΥΡΜΑΤΟΠΛΕΓΜΑΤΑ ΤΗΣ ΣΚΛΑΒΙΑΣ
   dewey: 889.21 ΣΡΩ
-  entry_numbers:
-  - '2076'
+  entry_numbers: []
   editor: None // ΑΘΗΝΑ
   edition_year: 1959
   pages: 259
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΔΙΗΓΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3297
     1: ΡΩ-ΣΙΓΜΑ,ΖΗΤΑ
     2: ΣΤΑ ΣΥΡΜΑΤΟΠΛΕΓΜΑΤΑ ΤΗΣ ΣΚΛΑΒΙΑΣ
     4: 889.21ΣΡΩ
-    5: '2076'
     9: ΑΘΗΝΑ
     10: '1959'
     11: 259Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
     13: ΔΙΗΓΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΔΙΗΓΗΜΑΤΑ
     3: null
+    5: null
     6: null
     7: null
     8: null
     15: null
     16: null
     17: null
     18: null
@@ -169318,15 +169162,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3312
   authors:
-  - ΑΓΓΕΛΗ,ΝΙΚΟΥ
+  - ΑΓΓΕΛΗΣ,ΝΙΚΟΣ
   language: el
   title: ΑΛΕΞΙΟΣ ΚΑΛΛΕΡΓΗΣ Ο ΜΕΓΑΣ ΑΡΧΩΝ
   dewey: 889.21 ΑΓΓ
   entry_numbers:
   - '5411'
   editor: None // ΑΘΗΝΑ
   edition_year: 1963
@@ -171339,15 +171183,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3353
   authors:
-  - ΑΘΑΝΑΣΙΟΥ,ΤΑΚΗ
+  - ΑΘΑΝΑΣΙΟΥ,ΤΑΚΗΣ
   language: el
   title: ΣΕ ΧΡΩΜΑ ΜΩΒ
   dewey: 889.21 ΑΘΑ
   entry_numbers:
   - '5415'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1965
@@ -171634,15 +171478,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3359
   authors:
-  - ΑΓΝΑΝΤΗ,ΚΩΣΤΑΣ
+  - ΑΓΝΑΝΤΗΣ,ΚΩΣΤΑΣ
   language: el
   title: ΜΑΤΩΜΕΝΗ ΑΝΑΣΤΑΣΗ
   dewey: 889.21 ΑΓΝ
   entry_numbers:
   - '5414'
   editor: None // ΙΩΑΝΝΙΝΑ
   edition_year: 1959
@@ -172124,15 +171968,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3369
   authors:
-  - ΑΚΡΟΠΟΛΙΤΗΣ,Σ.
+  - ΑΚΡΟΠΟΛΙΤΗΣ,ΣΠΥΡΟΣ
   language: el
   title: ΝΕΡΑΙΔΑ ΤΗΣ ΜΑΝΗΣ
   dewey: 889.21 ΑΚΡ
   entry_numbers:
   - '5422'
   editor: ΕΛΛΗΝΙΚΟ ΜΕΛΛΟΝ // None
   pages: 161
@@ -172172,42 +172016,41 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3370
   authors:
-  - ΑΠΟΣΤΟΛΙΔΗ,ΗΡ.Ν
+  - ΑΠΟΣΤΟΛΙΔΗΣ,ΗΡΑΚΛΗΣ,Ν.
   language: el
   title: ΤΟ ΔΙΗΓΗΜΑ
-  dewey: 889 ΑΠΟ
-  entry_numbers:
-  - '2154'
+  dewey: 889.21 ΑΠΟ
+  entry_numbers: []
   editor: None // ΑΘΗΝΑ
   edition_year: 1953
   pages: 538
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΔΙΗΓΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3370
     1: ΑΠΟΣΤΟΛΙΔΗ,ΗΡ.Ν
     2: ΤΟ ΔΙΗΓΗΜΑ
-    4: 889ΑΠΟ
-    5: '2154'
+    4: 889.21ΑΠΟ
     9: ΑΘΗΝΑ
     10: '1953'
     11: 538Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
     13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΔΙΗΓΗΜΑ
     3: null
+    5: null
     6: null
     7: null
     8: null
     15: null
     16: null
     17: null
     18: null
@@ -172221,34 +172064,34 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3371
   authors:
-  - ΒΗΚΑΣ,Β
+  - ΒΗΚΑΣ,ΒΑΣΙΛΗΣ
   language: el
   title: ΣΥΝΤΡΙΜΜΙΑ
   dewey: 889.21 ΒΗΚ
   entry_numbers:
-  - '5463'
+  - '5465'
   editor: ΑΘΗΝΑ // ΑΘΗΝΑ
   pages: 112
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΡΟΜΑΝΤΖΟ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3371
     1: ΒΗΚΑΣ,Β
     2: ΣΥΝΤΡΙΜΜΙΑ
     4: 889.21ΒΗΚ
-    5: '5463'
+    5: '5465'
     8: ΑΘΗΝΑ
     9: ΑΘΗΝΑ
     11: 112Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΡΟΜΑΝΤΖΟ
     13: ΡΟΜΑΝΤΖΟ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΡΟΜΑΝΤΖΟ
     3: null
@@ -173102,35 +172945,35 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3389
   authors:
-  - ΑΘΑΝΑΣΙΑΔΗ,ΝΙΚΟ
+  - ΑΘΑΝΑΣΙΑΔΗΣ,ΝΙΚΟΣ
   language: el
   title: ΠΕΡΑ ΑΠΟ ΤΟ ΑΝΘΡΩΠΙΝΟ
   dewey: 889.21 ΑΘΑ
   entry_numbers:
-  - '2182'
+  - '54092182'
   editor: ΣΤΕΓΗ ΤΟΥ ΒΙΒΛΙΟΥ // ΑΘΗΝΑ
   edition_year: 1956
   pages: 540
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3389
     1: ΑΘΑΝΑΣΙΑΔΗ,ΝΙΚΟ
     2: ΠΕΡΑ ΑΠΟ ΤΟ ΑΝΘΡΩΠΙΝΟ
     4: 889.21ΑΘΑ
-    5: '2182'
+    5: '54092182'
     8: ΣΤΕΓΗ ΤΟΥ ΒΙΒΛΙΟΥ
     9: ΑΘΗΝΑ
     10: '1956'
     11: 540Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΜΥΘΙΣΤΟΡΗΜΑ
@@ -174633,30 +174476,30 @@
 - dbase_number: 3420
   authors:
   - ΠΕΦΑΝΗ,ΔΩΡΟΥ
   language: el
   title: ΤΟ ΜΟΙΡΑΙΟ ΡΟΜΑΝΤΖΟ
   dewey: 889.21 ΠΕΦ
   entry_numbers:
-  - '5788'
+  - 05788
   editor: ΚΟΝΤΖΑΝΑΣΤΗ // ΑΘΗΝΑ
   edition_year: 1935
   pages: 80
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3420
     1: ΠΕΦΑΝΗ,ΔΩΡΟΥ
     2: ΤΟ ΜΟΙΡΑΙΟ ΡΟΜΑΝΤΖΟ
     4: 889.21ΠΕΦ
-    5: '5788'
+    5: 05788
     8: ΚΟΝΤΖΑΝΑΣΤΗ
     9: ΑΘΗΝΑ
     10: '1935'
     11: 80Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΜΥΘΙΣΤΟΡΗΜΑ
@@ -175171,30 +175014,30 @@
 - dbase_number: 3431
   authors:
   - ΣΚΙΑΔΑΡΕΣΗ,ΣΠΥΡΟΥ
   language: el
   title: ΚΕΦΑΛΟΝΙΤΙΚΕΣ ΙΣΤΟΡΙΕΣ
   dewey: 889.21 ΣΚΙ
   entry_numbers:
-  - '2151'
+  - '5850'
   editor: ΔΙΦΡΟΣ // ΑΘΗΝΑ
   edition_year: 1959
   pages: 180
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΔΙΗΓΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3431
     1: ΣΚΙΑΔΑΡΕΣΗ,ΣΠΥΡΟΥ
     2: ΚΕΦΑΛΟΝΙΤΙΚΕΣ ΙΣΤΟΡΙΕΣ
     4: 889.21ΣΚΙ
-    5: '2151'
+    5: '5850'
     8: ΔΙΦΡΟΣ
     9: ΑΘΗΝΑ
     10: '1959'
     11: 180Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
     13: ΔΙΗΓΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΔΙΗΓΗΜΑΤΑ
@@ -175215,43 +175058,42 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3432
   authors:
-  - ΑΡΚΑΔΙΟΥ,ΛΕΥΚΟΥ
+  - ΑΡΚΑΔΙΟΥ,ΛΕΥΚΟΣ
   language: el
   title: ΔΑΙΜΟΝΕΣ ΚΑΙ ΣΤΑΥΡΟΙ
   dewey: 889 ΑΡΚ
-  entry_numbers:
-  - '2116'
+  entry_numbers: []
   editor: ΜΑΥΡΙΔΗΣ // ΑΘΗΝΑ
   edition_year: 1959
   pages: 415
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3432
     1: ΑΡΚΑΔΙΟΥ,ΛΕΥΚΟΥ
     2: ΔΑΙΜΟΝΕΣ ΚΑΙ ΣΤΑΥΡΟΙ
     4: 889ΑΡΚ
-    5: '2116'
     8: ΜΑΥΡΙΔΗΣ
     9: ΑΘΗΝΑ
     10: '1959'
     11: 415Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΜΥΘΙΣΤΟΡΗΜΑ
     3: null
+    5: null
     6: null
     7: null
     15: null
     16: null
     17: null
     18: null
     19: null
@@ -175857,38 +175699,37 @@
     30: null
 - dbase_number: 3445
   authors:
   - ORWELL,GEORGE
   language: el
   title: ΤΟ ΤΣΙΦΛΙΚΙ ΤΩΝ ΖΩΩΝ
   dewey: 823 ORW
-  entry_numbers:
-  - '2347'
+  entry_numbers: []
   editor: None // ΑΘΗΝΑ
   edition_year: 1951
   pages: 133
   topics:
   - ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3445
     1: ORWELL,GEORGE
     2: ΤΟ ΤΣΙΦΛΙΚΙ ΤΩΝ ΖΩΩΝ
     4: 823ORW
-    5: '2347'
     9: ΑΘΗΝΑ
     10: '1951'
     11: 133Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΜΥΘΙΣΤΟΡΗΜΑ
     3: null
+    5: null
     6: null
     7: null
     8: null
     15: null
     16: null
     17: null
     18: null
@@ -175902,15 +175743,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3446
   authors:
-  - ALLEN,FREDERICK LEWIS
+  - ALLEN,FREDERICK,LEWIS
   language: el
   title: Η ΜΕΓΑΛΗ ΑΛΛΑΓΗ
   dewey: 810.11 ALL
   entry_numbers:
   - '5437'
   editor: ΙΚΑΡΟΣ // ΑΘΗΝΑ
   edition_year: 1956
@@ -176746,30 +176587,30 @@
 - dbase_number: 3463
   authors:
   - ΜΑΝΙΑΤΑΚΟΥ,ΓΙΩΡΓΟΥ
   language: el
   title: ΚΑΤΩ ΑΠΟ ΞΕΝΟΝ ΗΛΙΟ
   dewey: 889.21 ΜΑΝ
   entry_numbers:
-  - '5746'
+  - '6086'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 1958
   pages: 332
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3463
     1: ΜΑΝΙΑΤΑΚΟΥ,ΓΙΩΡΓΟΥ
     2: ΚΑΤΩ ΑΠΟ ΞΕΝΟΝ ΗΛΙΟ
     4: 889.21ΜΑΝ
-    5: '5746'
+    5: '6086'
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: '1958'
     11: 332Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΜΥΘΙΣΤΟΡΗΜΑ
@@ -176839,15 +176680,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3465
   authors:
-  - ΒΑΛΙΝΟΥ,ΓΙΑΝΝΗ
+  - ΒΑΛΙΝΟΣ,ΓΙΑΝΝΗΣ
   language: el
   title: Η ΑΜΦΙΒΟΛΙΑ
   dewey: 889.21 ΒΑΛ
   entry_numbers:
   - '4957'
   editor: None // ΑΘΗΝΑ
   edition_year: 1998
@@ -177430,15 +177271,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3477
   authors:
-  - ΒΟΥΡΛΕΚΗ,ΣΩΤΟΥ
+  - ΒΟΥΡΛΕΚΗΣ,ΣΩΤΟΣ
   language: el
   title: ΕΞΟΜΟΛΟΓΗΣΕΙΣ ΝΕΥΡΑΣΘΕΝΙΚΟΥ
   dewey: 889.21 ΒΟΥ
   entry_numbers:
   - '5463'
   editor: None // ΑΘΗΝΑ
   edition_year: 1929
@@ -177674,15 +177515,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3482
   authors:
-  - ΑΡΓΥΡΗ,ΚΩΣΤΑ
+  - ΑΡΓΥΡΗΣ,ΚΩΣΤΑΣ
   language: el
   title: ΟΙ ΜΕΓΑΛΟΙ ΟΡΙΖΟΝΤΕΣ
   dewey: 889.21 ΑΡΓ
   entry_numbers:
   - '5430'
   editor: ΙΚΑΡΟΣ // ΑΘΗΝΑ
   edition_year: 1956
@@ -178666,40 +178507,39 @@
     29: null
     30: null
 - dbase_number: 3502
   authors:
   - ΑΘΑΝΑΣΙΑΔΗΣ,ΠΕΤΡΟΣ
   language: el
   title: ΤΟ ΓΥΜΝΟ ΚΟΡΙΤΣΙ
-  dewey: 889 ΑΘΑ
-  entry_numbers:
-  - '2106'
+  dewey: 889.21 ΑΘΑ
+  entry_numbers: []
   editor: ΗΕΛΛΑΣ // ΑΘΗΝΑ
   edition_year: 1964
   pages: 236
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3502
     1: ΑΘΑΝΑΣΙΑΔΗΣ,ΠΕΤΡΟΣ
     2: ΤΟ ΓΥΜΝΟ ΚΟΡΙΤΣΙ
-    4: 889ΑΘΑ
-    5: '2106'
+    4: 889.21ΑΘΑ
     8: ΗΕΛΛΑΣ
     9: ΑΘΗΝΑ
     10: '1964'
     11: 236Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΜΥΘΙΣΤΟΡΗΜΑ
     3: null
+    5: null
     6: null
     7: null
     15: null
     16: null
     17: null
     18: null
     19: null
@@ -178910,15 +178750,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3507
   authors:
-  - ΑΛΑΒΕΡΑ,ΤΗΛ.
+  - ΑΛΑΒΕΡΑΣ,ΤΗΛΕΜΑΧΟΣ
   language: el
   title: ΤΟ ΜΙΣΟ ΤΟΥ ΦΕΓΓΑΡΙΟΥ
   dewey: 889 ΑΛΑ
   entry_numbers:
   - '5417'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1960
@@ -179057,15 +178897,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3510
   authors:
-  - ΒΟΥΛΟΔΗΜΟΥ,ΓΙΩΡΓΟΥ
+  - ΒΟΥΛΟΔΗΜΟΣ,ΓΙΩΡΓΟΣ
   language: el
   title: ΑΝΤΑΡΚΤΙΔΑ
   dewey: 889.21 ΒΟΥ
   entry_numbers:
   - '4701'
   editor: ΔΙΦΡΟΣ // ΑΘΗΝΑ
   edition_year: 1957
@@ -179455,15 +179295,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3518
   authors:
-  - ΑΓΓΕΛΗ,ΝΙΚΟΥ
+  - ΑΓΓΕΛΗΣ,ΝΙΚΟΣ
   language: el
   title: ΣΤΟΝ ΙΣΚΙΟ ΤΗΣ ΜΑΔΑΡΑΣ
   dewey: 889 ΑΓΓ
   entry_numbers:
   - '4679'
   editor: None // ΑΘΗΝΑ
   edition_year: 1961
@@ -179906,15 +179746,15 @@
   authors:
   - WHARTON,EDITH
   language: el
   title: ΣΤΑ ΔΕΝΤΡΑ ΣΤΟ ΧΙΟΝΙ
   subtitle: ΕΘΑΝ ΦΡΟΜ
   dewey: 889 WHA
   entry_numbers:
-  - '2323'
+  - '1294'
   translators:
   - ΚΩΝΣΤΑΝΤΙΝΟΥ,Ν.
   editor: ΙΚΑΡΟΣ // ΑΘΗΝΑ
   edition_year: 1956
   pages: 136
   topics:
   - ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -179924,15 +179764,15 @@
   offprint: false
   original_entry:
     0: 3527
     1: WHARTON,EDITH
     2: ΣΤΑ ΔΕΝΤΡΑ ΣΤΟ ΧΙΟΝΙ
     3: ΕΘΑΝ ΦΡΟΜ
     4: 889WHA
-    5: '2323'
+    5: '1294'
     6: Ν.ΚΩΝΣΤΑΝΤΙΝΟΥ
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: '1956'
     11: 136Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
     13: ΔΙΗΓΗΜΑ-ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -180492,15 +180332,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3539
   authors:
-  - ΑΘΑΝΑΣ,Γ
+  - ΑΘΑΝΑΣΙΑΔΗΣ-ΝΟΒΑΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΒΑΘΙΕΣ ΡΙΖΕΣ
   dewey: 889.21 ΑΘΑ
   entry_numbers:
   - '5438'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   pages: 365
@@ -180687,15 +180527,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3543
   authors:
-  - ΑΘΑΝΑΣΙΑΔΗ,ΤΑΣΟΥ
+  - ΑΘΑΝΑΣΙΑΔΗΣ,ΤΑΣΟΣ
   language: el
   title: Ο ΝΤΟΣΤΟΓΕΦΣΚΙ ΑΠΟ ΤΟ ΚΑΤΕΡΓΟ ΣΤΟ ΠΑΘΟΣ
   dewey: 889.21 ΑΘΑ
   entry_numbers:
   - '5410'
   edition: '2'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
@@ -180788,15 +180628,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3545
   authors:
-  - ΒΛΑΧΟΥ,Α.Σ
+  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,Σ.
   language: el
   title: ΟΔΟΙΠΟΡΟΙ ΓΙΑ ΤΑ ΣΟΥΣΑ
   dewey: 889.21 ΒΛΑ
   entry_numbers:
   - '5453'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   pages: 216
@@ -180836,15 +180676,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3546
   authors:
-  - ΒΛΑΧΟΥ,ΑΓΓΕΛΟΥ Σ.
+  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,Σ.
   language: el
   title: Ο ΚΥΡΙΟΣ ΜΟΥ ΑΛΚΙΒΙΑΔΗΣ
   dewey: 889.21 ΒΛΑ
   entry_numbers:
   - '5448'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   pages: 439
@@ -181083,15 +180923,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3551
   authors:
-  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ
+  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ,
   language: el
   title: ΟΙ ΤΕΛΕΥΤΑΙΟΙ ΓΑΛΗΝΟΤΑΤΟΙ
   dewey: 889.21 ΒΛΑ
   entry_numbers:
   - '5447'
   edition: '2'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
@@ -181284,15 +181124,15 @@
 - dbase_number: 3555
   authors:
   - ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛ.
   language: el
   title: ΚΑΛΗΝΥΧΤΑ ΖΩΗ
   dewey: 889.21 ΛΟΥ
   entry_numbers:
-  - '5656'
+  - '5650'
   edition: '2'
   editor: ΚΕΔΡΟΣ // ΑΘΗΝΑ
   edition_year: 1956
   pages: 228
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΜΥΘΙΣΤΟΡΗΜΑ
@@ -181300,15 +181140,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 3555
     1: ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛ.
     2: ΚΑΛΗΝΥΧΤΑ ΖΩΗ
     4: 889.21ΛΟΥ
-    5: '5656'
+    5: '5650'
     7: 2ΕΚΔ
     8: ΚΕΔΡΟΣ
     9: ΑΘΗΝΑ
     10: '1956'
     11: 228Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -181432,29 +181272,29 @@
 - dbase_number: 3558
   authors:
   - ΡΩΜΑ,ΔΙΟΝ.
   language: el
   title: Ο ΣΟΠΡΑΚΟΜΙΤΟΣ
   dewey: 889.21 ΡΩΜ
   entry_numbers:
-  - '2435'
+  - '5804'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   pages: 444
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΧΡΟΝΙΚΟ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3558
     1: ΡΩΜΑ,ΔΙΟΝ.
     2: Ο ΣΟΠΡΑΚΟΜΙΤΟΣ
     4: 889.21ΡΩΜ
-    5: '2435'
+    5: '5804'
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     11: 444Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΧΡΟΝΙΚΟ
     13: ΧΡΟΝΙΚΟ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΧΡΟΝΙΚΟ
     3: null
@@ -182312,15 +182152,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3576
   authors:
-  - ΑΘΑΝΑΣΙΑΔΗ,ΤΑΣΟΥ
+  - ΑΘΑΝΑΣΙΑΔΗΣ,ΤΑΣΟΣ
   language: el
   title: ΑΝΑΓΝΩΡΙΣΕΙΣ
   dewey: 889.21 ΑΘΑ
   entry_numbers:
   - '5406'
   edition: '2'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
@@ -182414,29 +182254,29 @@
     30: null
 - dbase_number: 3578
   authors: []
   language: el
   title: Ο ΜΙΚΡΟΣ ΔΗΜΗΤΡΙΟΣ ΑΡΚΕΤΗΣ
   dewey: 889.21 ΧΣ
   entry_numbers:
-  - '3925'
+  - '5925'
   editor: ΣΙΔΕΡΗΣ // ΑΘΗΝΑ
   pages: 80
   topics:
   - ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΔΙΗΓΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3578
     1: Χ.Σ
     2: Ο ΜΙΚΡΟΣ ΔΗΜΗΤΡΙΟΣ ΑΡΚΕΤΗΣ
     4: 889.21Χ.Σ
-    5: '3925'
+    5: '5925'
     8: ΣΙΔΕΡΗΣ
     9: ΑΘΗΝΑ
     11: 80Σ
     12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
     13: ΔΙΗΓΗΜΑ-ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΔΙΗΓΗΜΑ
     3: null
@@ -182511,29 +182351,29 @@
 - dbase_number: 3580
   authors:
   - ΨΑΛΤΟΠΟΥΛΟΥ,Λ.
   language: el
   title: ΘΕΙΑ ΤΡΑΓΩΔΙΑ
   dewey: 889.21 ΨΑΛ
   entry_numbers:
-  - '4691'
+  - '5937'
   editor: ΤΡΙΑΝΤΑΦΥΛΛΟΥ // ΘΕΣΣΑΛΟΝΙΚΗ
   pages: 124
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΔΙΗΓΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3580
     1: ΨΑΛΤΟΠΟΥΛΟΥ,Λ.
     2: ΘΕΙΑ ΤΡΑΓΩΔΙΑ
     4: 889.21ΨΑΛ
-    5: '4691'
+    5: '5937'
     8: ΤΡΙΑΝΤΑΦΥΛΛΟΥ
     9: ΘΕΣΣΑΛΟΝΙΚ
     11: 124Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
     13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΔΙΗΓΗΜΑ
     3: null
@@ -182705,15 +182545,15 @@
 - dbase_number: 3584
   authors:
   - NEALE,A.
   language: el
   title: ΘΕΟΔΩΡΑ ΦΡΑΝΤΖΗ
   dewey: 823 NEA
   entry_numbers:
-  - '5726'
+  - '5725'
   editor: ΤΣΑΓΚΑΡΑΚΗΣ // ΑΘΗΝΑ
   edition_year: 1901
   pages: 351
   topics:
   - ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   volume: ΤΟΜΟΣ Β.
@@ -182721,15 +182561,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 3584
     1: NEALE,A.
     2: ΘΕΟΔΩΡΑ ΦΡΑΝΤΖΗ
     4: 823NEA
-    5: '5726'
+    5: '5725'
     8: ΤΣΑΓΚΑΡΑΚΗΣ
     9: ΑΘΗΝΑ
     10: '1901'
     11: 351Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -182799,15 +182639,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3586
   authors:
-  - ΒΟΥΤΥΡΑ,ΔΗΜΟΣΘΕΝΗ
+  - ΒΟΥΤΥΡΑΣ,ΔΗΜΟΣΘΕΝΗΣ
   language: el
   title: Η ΑΡΙΣΤΟΚΡΑΤΙΚΗ ΓΕΙΤΟΝΙΑ
   dewey: 889.21 ΒΟΥ
   entry_numbers:
   - '5455'
   editor: ΒΑΣΙΛΕΙΟΥ // ΑΘΗΝΑ
   edition_year: 1924
@@ -183416,30 +183256,30 @@
 - dbase_number: 3598
   authors:
   - ΕΦΤΑΛΙΩΤΗΣ,ΑΡΓΥΡΗΣ
   language: el
   title: ΝΗΣΙΩΤΙΚΕΣ ΙΣΤΟΡΙΕΣ
   dewey: 889.21 ΕΦΤ
   entry_numbers:
-  - '2197'
+  - '5535'
   editor: ΦΕΞΗ // ΑΘΗΝΑ
   edition_year: 1941
   pages: 152
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΔΙΗΓΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3598
     1: ΕΦΤΑΛΙΩΤΗΣ,ΑΡΓΥΡΗΣ
     2: ΝΗΣΙΩΤΙΚΕΣ ΙΣΤΟΡΙΕΣ
     4: 889.21ΕΦΤ
-    5: '2197'
+    5: '5535'
     8: ΦΕΞΗ
     9: ΑΘΗΝΑ
     10: '1941'
     11: 152Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
     13: ΔΙΗΓΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΔΙΗΓΗΜΑΤΑ
@@ -183563,15 +183403,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3601
   authors:
-  - ΑΘΑΝΑΣΙΑΔΗ,ΤΑΣΟΥ
+  - ΑΘΑΝΑΣΙΑΔΗΣ,ΤΑΣΟΣ
   language: el
   title: ΟΙ ΠΑΝΘΕΟΙ
   subtitle: ΜΑΡΜΩ ΠΑΝΘΕΟΥ
   dewey: 889.21 ΑΘΑ
   entry_numbers:
   - '5407'
   edition: '4'
@@ -183614,15 +183454,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3602
   authors:
-  - ΑΘΑΝΑΣΙΑΔΗ,ΤΑΣΟΥ
+  - ΑΘΑΝΑΣΙΑΔΗΣ,ΤΑΣΟΣ
   language: el
   title: ΟΙ ΠΑΝΘΕΟΙ
   subtitle: Η ΧΑΡΙΣΑΜΕΝΟΙ ΕΠΟΧΗ
   dewey: 889 ΑΘΑ
   entry_numbers:
   - '5869'
   edition: '2'
@@ -183716,15 +183556,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3604
   authors:
-  - ΒΙΖΥΗΝΟΥ,Γ.Μ
+  - ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ,M.
   language: el
   title: ΤΟ ΑΜΑΡΤΗΜΑ ΤΗΣ ΜΗΤΡΟΣ ΜΟΥ
   dewey: 889.21 ΒΙΖ
   entry_numbers:
   - '1015'
   editor: ΓΑΛΑΞΙΑΣ // ΑΘΗΝΑ
   edition_year: 1961
@@ -183816,15 +183656,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3606
   authors:
-  - ΒΙΚΕΛΑ,ΔΗΜ
+  - ΒΙΚΕΛΑΣ,ΔΗΜΗΤΡΙΟΣ
   language: el
   title: ΛΟΥΚΗΣ ΛΑΡΑΣ
   dewey: 889.21 ΒΙΚ
   entry_numbers:
   - '5444'
   editor: ΓΑΛΑΞΙΑΣ // ΑΘΗΝΑ
   edition_year: 1961
@@ -183963,20 +183803,21 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3609
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: ΑΠΑΝΤΑ
   subtitle: ΕΝΑ ΔΡΑΜΑ ΣΤΗ ΛΙΒΟΝΙΑ
   dewey: 808.899 ΒΕΡ
-  entry_numbers: []
+  entry_numbers:
+  - '20686'
   translators:
   - ΠΑΠΑΔΑΤΟΥ,Μ.
   editor: ΓΕΜΕΝΤΖΟΠΟΥΛΟΣ // ΑΘΗΝΑ
   pages: 165
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
@@ -183984,22 +183825,22 @@
   offprint: false
   original_entry:
     0: 3609
     1: ΒΕΡΝ,ΙΟΥΛΙΟΣ
     2: ΑΠΑΝΤΑ
     3: ΕΝΑ ΔΡΑΜΑ ΣΤΗ ΛΙΒΟΝΙΑ
     4: 808.899ΒΕΡ
+    5: '20686'
     6: Μ.ΠΑΠΑΔΑΤΟΥ
     8: ΓΕΜΕΝΤΖΟΠΟΥΛΟΣ
     9: ΑΘΗΝΑ
     11: 165Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
-    5: null
     7: null
     10: null
     15: null
     16: null
     17: null
     18: null
     19: null
@@ -184216,15 +184057,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3614
   authors:
-  - ΒΛΑΧΟΥ,ΑΓΓΕΛΟΥ
+  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,Σ.
   language: el
   title: ΤΟ ΜΝΗΜΑ ΤΗΣ ΓΡΙΑΣ
   subtitle: ΟΙ ΩΡΕΣ ΖΩΗΣ
   dewey: 889.21 ΒΛΑ
   entry_numbers:
   - '5450'
   editor: ΓΑΛΑΞΙΑΣ // ΑΘΗΝΑ
@@ -184423,15 +184264,15 @@
 - dbase_number: 3618
   authors:
   - MALAMUD,BERNARD
   language: el
   title: ΤΟ ΜΑΓΙΚΟ ΒΑΡΕΛΙ
   dewey: 810.11 MAL
   entry_numbers:
-  - '2234'
+  - '1313'
   translators:
   - ΚΡΙΣΠΗΣ,ΜΑΝΘΟΣ
   editor: Η ΣΥΓΧΡΟΝΗ ΑΜΕΡΙΚΗ // ΑΘΗΝΑ
   edition_year: 1953
   pages: 202
   topics:
   - ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -184440,15 +184281,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 3618
     1: MALAMUD,BERNARD
     2: ΤΟ ΜΑΓΙΚΟ ΒΑΡΕΛΙ
     4: 810.11MAL
-    5: '2234'
+    5: '1313'
     6: ΜΑΝΘΟΣ ΚΡΙΣΠΗΣ
     8: Η ΣΥΓΧΡΟΝΗ ΑΜΕΡΙΚΗ
     9: ΑΘΗΝΑ
     10: '1953'
     11: 202Σ
     12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
     13: ΔΙΗΓΗΜΑΤΑ-ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -184577,16 +184418,15 @@
 - dbase_number: 3621
   authors:
   - ΧΙΛΤΟΝ,ΤΖΕΗΜΣ
   language: el
   title: ΧΑΜΕΝΟΣ ΟΡΙΖΩΝ
   dewey: 823 ΧΙΛ
   entry_numbers:
-  - '2240'
-  - '20420'
+  - '1321'
   translators:
   - ΚΑΙΝΑΔΑ,ΜΑΓΔΑ
   editor: ΓΑΛΑΞΙΑΣ // ΑΘΗΝΑ
   edition_year: 1961
   pages: 172
   topics:
   - ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -184595,15 +184435,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 3621
     1: ΧΙΛΤΟΝ,ΤΖΕΗΜΣ
     2: ΧΑΜΕΝΟΣ ΟΡΙΖΩΝ
     4: 823ΧΙΛ
-    5: 2240-20420
+    5: '1321'
     6: ΜΑΓΔΑ ΚΑΙΝΑΔΑ
     8: ΓΑΛΑΞΙΑΣ
     9: ΑΘΗΝΑ
     10: '1961'
     11: 172Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
     13: ΔΙΗΓΗΜΑΤΑ-ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -184829,15 +184669,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3626
   authors:
-  - AGEEE,JAMES
+  - AGEE,JAMES
   language: el
   title: ΑΥΤΟΙ ΠΟΥ ΕΜΕΙΝΑΝ...
   dewey: 810.11 AGE
   entry_numbers:
   - '1317'
   translators:
   - ΑΝΑΓΝΩΣΤΟΠΟΥΛΟΣ,Π.
@@ -186539,16 +186379,15 @@
     30: null
 - dbase_number: 3660
   authors:
   - ΣΙΝΟΠΟΥΛΟΥ,ΤΑΚΗ
   language: el
   title: Η ΠΟΙΗΣΗ ΤΗΣ ΠΟΙΗΣΗΣ
   dewey: 889.1 ΣΙΝ
-  entry_numbers:
-  - '2813'
+  entry_numbers: []
   editor: None // ΑΘΗΝΑ
   edition_year: 1964
   pages: 61
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   - ΠΟΙΗΣΗ
@@ -186556,22 +186395,22 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 3660
     1: ΣΙΝΟΠΟΥΛΟΥ,ΤΑΚΗ
     2: Η ΠΟΙΗΣΗ ΤΗΣ ΠΟΙΗΣΗΣ
     4: 889.1ΣΙΝ
-    5: '2813'
     9: ΑΘΗΝΑ
     10: '1964'
     11: 61Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΠΟΙΗΣΗ
     3: null
+    5: null
     6: null
     7: null
     8: null
     15: null
     16: null
     17: null
     18: null
@@ -187036,15 +186875,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3670
   authors:
-  - ΑΛΕΠΗ,ΚΟΥΛΗ
+  - ΑΛΕΠΗΣ,ΚΟΥΛΗΣ
   language: el
   title: ΧΡΥΣΕΣ ΜΝΗΜΕΣ
   dewey: 889.1 ΑΛΕ
   entry_numbers:
   - '5969'
   editor: ΝΕΣΤΩΡ // ΚΑΛΑΜΑΤΑ
   edition_year: 1959
@@ -187086,15 +186925,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3671
   authors:
-  - ΑΝΩΓΗΣ,Ν
+  - ΑΝΩΓΗΣ,ΝΙΚΟΣ
   language: el
   title: ΚΥΝΗΓΩΝΤΑΣ ΤΟΝ ΙΣΚΙΟ ΜΑΣ
   dewey: 889.1 ΑΝΩ
   entry_numbers:
   - '5087'
   editor: None // ΑΘΗΝΑ
   edition_year: 1981
@@ -187897,15 +187736,15 @@
 - dbase_number: 3687
   authors:
   - ΛΟΥΡΑΝΑΣ,ΠΕΤΡΑΣ
   language: el
   title: ΑΝΘΡΩΠΙΝΑ
   dewey: 889.1 ΛΟΥ
   entry_numbers:
-  - '6306'
+  - '6227'
   editor: ΠΥΡΣΟΣ // ΑΘΗΝΑ
   edition_year: 1941
   pages: 32
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   - ΠΟΙΗΣΗ
@@ -187914,15 +187753,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 3687
     1: ΛΟΥΡΑΝΑΣ,ΠΕΤΡΑΣ
     2: ΑΝΘΡΩΠΙΝΑ
     4: 889.1ΛΟΥ
-    5: '6306'
+    5: '6227'
     8: ΠΥΡΣΟΣ
     9: ΑΘΗΝΑ
     10: '1941'
     11: 32Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΠΟΙΗΣΗ
@@ -188803,18 +188642,17 @@
     29: null
     30: null
 - dbase_number: 3705
   authors:
   - ΚΟΚΚΙΝΟΣ,ΔΗΜΟΣΘ.
   language: el
   title: ΗΡΩΙΚΑ
-  dewey: 889.1 ΚΟΚ
+  dewey: 889.11 ΚΟΚ
   entry_numbers:
   - '6169'
-  - '5112'
   editor: ΔΩΔΩΝΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1977
   pages: 53
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   - ΠΟΙΗΣΗ
@@ -188822,16 +188660,16 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3705
     1: ΚΟΚΚΙΝΟΣ,ΔΗΜΟΣΘ.
     2: ΗΡΩΙΚΑ
-    4: 889.1ΚΟΚ
-    5: 6169-5112
+    4: 889.11ΚΟΚ
+    5: '6169'
     8: ΔΩΔΩΝΗ
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '1977'
     11: 53Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΠΟΙΗΣΗ
@@ -189560,17 +189398,17 @@
     30: null
 - dbase_number: 3720
   authors:
   - ΠΑΠΑ-ΜΠΟΥΜΗ,ΡΙΤΑ
   language: el
   title: ΜΟΡΓΚΑΝ ΙΩΑΝΝΗΣ
   subtitle: Ο ΓΥΑΛΙΝΟΣ ΠΡΙΓΚΙΠΑΣ ΚΑΙ ΟΙ ΜΕΤΑΜΟΡΦΩΣΕΙΣ ΤΟΥ
-  dewey: 889.1 ΠΑΠ
+  dewey: 889.11 ΠΑΠ
   entry_numbers:
-  - '6354'
+  - '6334'
   editor: ΚΑΡΑΝΑΣΗ // ΑΘΗΝΑ
   edition_year: 1976
   pages: 228
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   - ΠΟΙΗΣΗ
@@ -189579,16 +189417,16 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 3720
     1: ΠΑΠΑ-ΜΠΟΥΜΗ,ΡΙΤΑ
     2: ΜΟΡΓΚΑΝ ΙΩΑΝΝΗΣ
     3: Ο ΓΥΑΛΙΝΟΣ ΠΡΙΓΚΙΠΑΣ ΚΑΙ ΟΙ ΜΕΤΑΜΟΡΦΩΣΕΙΣ ΤΟΥ
-    4: 889.1ΠΑΠ
-    5: '6354'
+    4: 889.11ΠΑΠ
+    5: '6334'
     8: ΚΑΡΑΝΑΣΗ
     9: ΑΘΗΝΑ
     10: '1976'
     11: 228Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΠΟΙΗΣΗ
@@ -190413,15 +190251,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3737
   authors:
-  - ΑΘΑΝΑΣ,Γ.
+  - ΑΘΑΝΑΣΙΑΔΗΣ-ΝΟΒΑΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΤΙΜΙΑ ΔΩΡΑ
   dewey: 889.1 ΑΘΑ
   entry_numbers:
   - '4568'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 1969
@@ -192232,15 +192070,15 @@
 - dbase_number: 3773
   authors:
   - ΛΟΥΚΑΚΗΣ,ΚΩΣΤΑΣ
   language: el
   title: ΤΟ ΠΑΙΔΑΑΚΙ ΠΟΥ ΕΦΥΓΕ
   dewey: 889.1 ΛΟΥ
   entry_numbers:
-  - '2862'
+  - '2542'
   editor: Ο ΛΟΓΟΣ // ΑΘΗΝΑ
   edition_year: 1965
   pages: 84
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   - ΠΟΙΗΣΗ
@@ -192248,15 +192086,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 3773
     1: ΛΟΥΚΑΚΗΣ,ΚΩΣΤΑΣ
     2: ΤΟ ΠΑΙΔΑΑΚΙ ΠΟΥ ΕΦΥΓΕ
     4: 889.1ΛΟΥ
-    5: '2862'
+    5: '2542'
     8: Ο ΛΟΓΟΣ
     9: ΑΘΗΝΑ
     10: '1965'
     11: 84Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΠΟΙΗΣΗ
@@ -192477,15 +192315,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3778
   authors:
-  - ΒΕΛΜΥΡΑ,ΚΩΣΤΗ
+  - ΒΕΛΜΥΡΑΣ,ΚΩΣΤΗΣ
   language: el
   title: ΛΙΓΑ ΤΡΑΓΟΥΔΙΑ
   dewey: 889.1 ΒΕΛ
   entry_numbers:
   - '5982'
   editor: ΡΑΛΛΗ // ΑΘΗΝΑ
   edition_year: 1929
@@ -192632,15 +192470,15 @@
 - dbase_number: 3781
   authors:
   - ΓΚΑΤΣΟΣ,ΝΙΚΟΣ
   language: el
   title: ΑΜΟΡΓΟΣ
   dewey: 889.1 ΓΚΑ
   entry_numbers:
-  - '2509'
+  - '4644'
   edition: Β
   editor: ΙΚΑΡΟΣ // ΑΘΗΝΑ
   edition_year: 1963
   pages: 45
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
@@ -192649,15 +192487,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 3781
     1: ΓΚΑΤΣΟΣ,ΝΙΚΟΣ
     2: ΑΜΟΡΓΟΣ
     4: 889.1ΓΚΑ
-    5: '2509'
+    5: '4644'
     7: Β'ΕΚΔ
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: '1963'
     11: 45Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -192728,15 +192566,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3783
   authors:
-  - ΑΘΑΝΑΣΟΥΛΗΣ,ΚΡΙΤΩΝ
+  - ΑΘΑΝΑΣΟΥΛΗΣ,ΚΡΙΤΩΝΑΣ
   language: el
   title: Ο ΑΓΡΙΟΧΟΙΡΟΣ
   dewey: 889.1 ΑΘΑ
   entry_numbers:
   - '5960'
   editor: ΔΙΦΡΟΣ // ΑΘΗΝΑ
   edition_year: 1963
@@ -193131,15 +192969,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3791
   authors:
-  - ΑΡΤΟΓΚ,ΕΡΡΙΚΟΥ
+  - ΑΡΤΟΓΚ,ΕΡΡΙΚΟΣ
   language: el
   title: ΛΙΛΙΟ
   subtitle: Η ΡΕΚΒΙΕΜ ΓΙΑ ΕΝΑΝ ΚΟΣΜΟ
   dewey: 889.1 ΑΡΤ
   entry_numbers:
   - '6019'
   edition_year: 1976
@@ -193481,15 +193319,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3798
   authors:
-  - ΒΟΚΟΒΙΤΣ,ΝΙΚΟΥ
+  - ΒΟΚΟΒΙΤΣ,ΝΙΚΟΣ
   language: el
   title: ΑΝΑΒΙΩΣΗ
   dewey: 889.1 ΒΟΚ
   entry_numbers:
   - '5991'
   editor: ΝΙΚΟΛΑΙΔΗ // ΑΘΗΝΑ
   edition_year: 1988
@@ -194185,15 +194023,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3812
   authors:
-  - ΒΑΦΟΠΟΥΛΟΣ,Γ.Θ
+  - ΒΑΦΟΠΟΥΛΟΣ,Γ.,Θ.
   language: el
   title: ΤΑ ΕΠΙΓΕΝΟΜΕΝΑ
   dewey: 889.1 ΒΑΦ
   entry_numbers:
   - '5983'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1977
@@ -194745,15 +194583,14 @@
 - dbase_number: 3823
   authors:
   - ΚΑΤΣΑΝΟΥ,ΓΙΑΝΝΗΣ
   language: el
   title: ΑΝΘΡΩΠΟΙ ΚΑΙ ΤΟΠΙΟ
   dewey: 889.1 ΚΑΤ
   entry_numbers:
-  - '4644'
   - '4533'
   editor: None // ΑΘΗΝΑ
   edition_year: 1989
   pages: 29
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
@@ -194763,15 +194600,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 3823
     1: ΚΑΤΣΑΝΟΥ,ΓΙΑΝΝΗΣ
     2: ΑΝΘΡΩΠΟΙ ΚΑΙ ΤΟΠΙΟ
     4: 889.1ΚΑΤ
-    5: 4644-4533
+    5: '4533'
     9: ΑΘΗΝΑ
     10: '1989'
     11: 29Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΠΟΙΗΣΗ
     17: 2 ΑΝΤΙΤΥΠΑ
@@ -195840,15 +195677,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3845
   authors:
-  - ΑΝΩΒΟΛΙΩΤΗ,ΓΙΩΡΓΟ
+  - ΑΝΩΒΟΛΙΩΤΗΣ,ΓΙΩΡΓΟΣ
   language: el
   title: ΑΝΘΗ ΣΕ ΜΑΥΡΟ ΒΑΖΟ
   dewey: 889.1 ΑΝΩ
   entry_numbers:
   - '4628'
   editor: None // ΑΘΗΝΑ
   edition_year: 1993
@@ -196792,15 +196629,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3864
   authors:
-  - ΑΝΤΩΝΙΑΔΗ,ΓΙΑΝΑΚΟΣ,ΑΛ.
+  - ΓΙΑΝΑΚΟΣ ΑΝΤΩΝΙΑΔΗΣ,ΑΛΕΚΟΣ
   language: el
   title: ΕΙΡΗΝΙΚΟΙ ΡΥΘΜΟΙ
   dewey: 889.1 ΑΝΤ
   entry_numbers:
   - '4500'
   editor: None // ΑΘΗΝΑ
   edition_year: 1983
@@ -197791,47 +197628,36 @@
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3884
-  authors:
-  - ΙΑΝΝΗ
-  language: el
-  title: ΑΝΘΡΩΠΟΙ ΚΑΙ ΤΟΠΙΟ
-  dewey: 889.1 ΚΑΤ
-  entry_numbers:
-  - '4533'
-  editor: None // ΑΘΗΝΑ
-  edition_year: 1989
-  pages: 29
-  topics:
-  - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
-  - ΠΟΙΗΜΑΤΑ
-  - ΠΟΙΗΣΗ
+  authors: []
+  entry_numbers: []
+  topics: []
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3884
-    1: ΙΑΝΝΗ
-    2: ΑΝΘΡΩΠΟΙ ΚΑΙ ΤΟΠΙΟ
-    4: 889.1ΚΑΤ
-    5: '4533'
-    9: ΑΘΗΝΑ
-    10: '1989'
-    11: 29Σ
-    12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
-    13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
-    14: ΠΟΙΗΣΗ
+    1: null
+    2: null
     3: null
+    4: null
+    5: null
     6: null
     7: null
     8: null
+    9: null
+    10: null
+    11: null
+    12: null
+    13: null
+    14: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -198295,33 +198121,33 @@
     29: null
     30: null
 - dbase_number: 3894
   authors:
   - ΝΤΑΚΟΥ,Θ.
   language: el
   title: ΔΕΥΤΕΡΑ ΠΡΩΙ
-  dewey: 889.1 ΝΤΑ
+  dewey: 889.11 ΝΤΑ
   entry_numbers:
-  - '2776'
+  - '2578'
   editor: ΔΙΑΓΩΝΙΟΥ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1966
   pages: 26
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   - ΠΟΙΗΣΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3894
     1: ΝΤΑΚΟΥ,Θ.
     2: ΔΕΥΤΕΡΑ ΠΡΩΙ
-    4: 889.1ΝΤΑ
-    5: '2776'
+    4: 889.11ΝΤΑ
+    5: '2578'
     8: ΔΙΑΓΩΝΙΟΥ
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '1966'
     11: 26Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΠΟΙΗΣΗ
@@ -198843,15 +198669,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3905
   authors:
-  - ΑΣΠΙΩΤΗ,ΕΥΑΓΓΕΛΟΥ
+  - ΑΣΠΙΩΤΗΣ,ΕΥΑΓΓΕΛΟΣ
   language: el
   title: ΝΟΣΤΑΛΓΙΚΑ
   dewey: 889.1 ΑΣΠ
   entry_numbers:
   - '5948'
   editor: None // ΑΘΗΝΑ
   edition_year: 1969
@@ -199345,15 +199171,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3915
   authors:
-  - ΒΑΛΑΣΚΑΝΤΖΗ,ΔΗΜΗΤΡΗ
+  - ΒΑΛΑΣΚΑΝΤΖΗΣ,ΔΗΜΗΤΡΗΣ
   language: el
   title: ΑΚΜΩΝ
   dewey: 889.1 ΒΑΛ
   entry_numbers:
   - '4527'
   edition: Β
   editor: ΝΕΑ ΣΥΝΟΡΑ // ΑΘΗΝΑ
@@ -199396,15 +199222,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3916
   authors:
-  - ΒΑΛΑΣΚΑΝΤΖΗ,ΔΗΜΗΤΡΗ
+  - ΒΑΛΑΣΚΑΝΤΖΗΣ,ΔΗΜΗΤΡΗΣ
   language: el
   title: ΠΟΙΗΜΑΤΑ
   dewey: 889.1 ΒΑΛ
   entry_numbers:
   - '4528'
   edition: Β
   editor: ΝΕΑ ΣΥΝΟΡΑ // ΑΘΗΝΑ
@@ -199448,15 +199274,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3917
   authors:
-  - ΒΑΛΑΣΚΑΝΤΖΗ,ΔΗΜΗΤΡΗ
+  - ΒΑΛΑΣΚΑΝΤΖΗΣ,ΔΗΜΗΤΡΗΣ
   language: el
   title: ΑΜΙΧΕΣ
   dewey: 889.1 ΒΑΛ
   entry_numbers:
   - '4529'
   editor: ΝΕΑ ΣΥΝΟΡΑ // ΑΘΗΝΑ
   edition_year: 1979
@@ -200201,17 +200027,17 @@
     29: null
     30: null
 - dbase_number: 3932
   authors:
   - ΕΓΓΟΝΟΠΟΥΛΟΣ,ΝΙΚΟΣ
   language: el
   title: ΜΠΟΛΙΒΑΡ
-  dewey: 889.1 ΕΓΓ
+  dewey: 889.11 ΕΓΓ
   entry_numbers:
-  - '2513'
+  - '2188'
   edition: '2'
   editor: ΙΚΑΡΟΣ // ΑΘΗΝΑ
   edition_year: 1962
   pages: 45
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
@@ -200219,16 +200045,16 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3932
     1: ΕΓΓΟΝΟΠΟΥΛΟΣ,ΝΙΚΟΣ
     2: ΜΠΟΛΙΒΑΡ
-    4: 889.1ΕΓΓ
-    5: '2513'
+    4: 889.11ΕΓΓ
+    5: '2188'
     7: 2ΕΚΔ
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: '1962'
     11: 45Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -200552,33 +200378,33 @@
     29: null
     30: null
 - dbase_number: 3939
   authors:
   - ΔΗΜΟΥΛΑ,ΚΙΚΗ
   language: el
   title: ΕΠΙ ΤΑ ΙΧΝΗ
-  dewey: 889.1 ΔΗΜ
+  dewey: 889.11 ΔΗΜ
   entry_numbers:
-  - '2546'
+  - '20565'
   editor: ΦΕΞΗ // ΑΘΗΝΑ
   edition_year: 1963
   pages: 61
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   - ΠΟΙΗΣΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3939
     1: ΔΗΜΟΥΛΑ,ΚΙΚΗ
     2: ΕΠΙ ΤΑ ΙΧΝΗ
-    4: 889.1ΔΗΜ
-    5: '2546'
+    4: 889.11ΔΗΜ
+    5: '20565'
     8: ΦΕΞΗ
     9: ΑΘΗΝΑ
     10: '1963'
     11: 61Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΠΟΙΗΣΗ
@@ -201758,15 +201584,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3963
   authors:
-  - ΑΝΔΡΕΙΑΔΗ,ΚΟΡΑΛΙΑΣ
+  - ΑΝΔΡΕΙΑΔΗ,ΚΟΡΑΛΙΑ
   language: el
   title: ΑΠΟΠΕΙΡΕΣ
   dewey: 889.1 ΑΝΔ
   entry_numbers:
   - '5973'
   editor: ΦΕΞΗΣ // ΑΘΗΝΑ
   edition_year: 1963
@@ -202467,41 +202293,40 @@
     29: null
     30: null
 - dbase_number: 3977
   authors:
   - ΠΑΠΑΔΙΤΣΑ,Δ.Π
   language: el
   title: ΠΟΙΗΣΗ 2
-  dewey: 889.1 ΠΑΠ
-  entry_numbers:
-  - '2971'
+  dewey: 889.11 ΠΑΠ
+  entry_numbers: []
   editor: ΕΚΔΟΣΕΙΣ ΤΩΝ ΦΙΛΩΝ // ΑΘΗΝΑ
   edition_year: 1974
   pages: 151
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   - ΠΟΙΗΣΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 3977
     1: ΠΑΠΑΔΙΤΣΑ,Δ.Π
     2: ΠΟΙΗΣΗ 2
-    4: 889.1ΠΑΠ
-    5: '2971'
+    4: 889.11ΠΑΠ
     8: ΕΚΔΟΣΕΙΣ ΤΩΝ ΦΙΛΩΝ
     9: ΑΘΗΝΑ
     10: '1974'
     11: 151Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΠΟΙΗΣΗ
     3: null
+    5: null
     6: null
     7: null
     15: null
     16: null
     17: null
     18: null
     19: null
@@ -203120,15 +202945,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 3990
   authors:
-  - ΒΑΜΒΑΚΙΑΣ-ΙΩΑΝΝΙΔΗΣ,ΝΙΚΟΣ.Γ
+  - ΒΑΜΒΑΚΙΑΣ-ΙΩΑΝΝΙΔΗΣ,ΝΙΚΟΣ,Γ.
   language: el
   title: ΤΟ ΘΛΙΜΜΕΝΟ ΛΑΟΥΤΟ
   dewey: 889.1 ΒΑΜ
   entry_numbers:
   - '4720'
   editor: None // ΑΘΗΝΑ
   edition_year: 1949
@@ -204074,15 +203899,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4009
   authors:
-  - ΑΘΑΝΑΣΟΥΛΗΣ,ΚΡΙΤΩΝ
+  - ΑΘΑΝΑΣΟΥΛΗΣ,ΚΡΙΤΩΝΑΣ
   language: el
   title: ΠΕΡΙΠΤΩΣΕΙΣ ΚΑΘΗΜΕΡΙΝΟΤΗΤΑΣ
   dewey: 889.1 ΑΘΑ
   entry_numbers:
   - '5955'
   editor: ΝΕΣΤΩΡ // ΑΘΗΝΑ
   edition_year: 1959
@@ -204528,96 +204353,86 @@
     28: null
     29: null
     30: null
 - dbase_number: 4018
   authors:
   - ΠΑΠΑΤΣΩΝΗΣ,Τ.Κ
   language: el
-  title: ΕΚΛΟΓΗ Α'
+  title: ΕΚΛΟΓΗ Α', Β'
   subtitle: URSA MINOR
   dewey: 888.08 ΠΑΠ
   entry_numbers:
   - '6343'
   edition: Β
   editor: ΙΚΑΡΟΣ // ΑΘΗΝΑ
   edition_year: 1962
   pages: 166
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   - ΠΟΙΗΣΗ
+  notes: ΤΟΜΟΙ Α, Β
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 4018
     1: ΠΑΠΑΤΣΩΝΗΣ,Τ.Κ
-    2: ΕΚΛΟΓΗ Α'
+    2: ΕΚΛΟΓΗ Α', Β'
     3: URSA MINOR
     4: 888.08ΠΑΠ
     5: '6343'
     7: Β'ΕΚΔ
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: '1962'
     11: 166Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΠΟΙΗΣΗ
+    17: ΤΟΜΟΙ Α, Β
     6: null
     15: null
     16: null
-    17: null
     18: null
     19: null
     20: null
     21: null
     22: null
     23: null
     24: null
     25: null
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4019
-  authors:
-  - ΠΑΠΑΤΣΩΝΗΣ,Τ.Κ
-  language: el
-  title: ΕΚΛΟΓΗ Β'
-  dewey: 880.08 ΠΑΠ
-  entry_numbers:
-  - '6343'
-  editor: ΙΚΑΡΟΣ // ΑΘΗΝΑ
-  edition_year: 1962
-  pages: 175
-  topics:
-  - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
-  - ΠΟΙΗΜΑΤΑ
-  - ΠΟΙΗΣΗ
+  authors: []
+  entry_numbers: []
+  topics: []
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 4019
-    1: ΠΑΠΑΤΣΩΝΗΣ,Τ.Κ
-    2: ΕΚΛΟΓΗ Β'
-    4: 880.08ΠΑΠ
-    5: '6343'
-    8: ΙΚΑΡΟΣ
-    9: ΑΘΗΝΑ
-    10: '1962'
-    11: 175Σ
-    12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
-    13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
-    14: ΠΟΙΗΣΗ
+    1: null
+    2: null
     3: null
+    4: null
+    5: null
     6: null
     7: null
+    8: null
+    9: null
+    10: null
+    11: null
+    12: null
+    13: null
+    14: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -204930,15 +204745,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4026
   authors:
-  - ΑΝΩΒΟΛΙΩΤΗ,ΓΙΩΡΓΟΥ
+  - ΑΝΩΒΟΛΙΩΤΗΣ,ΓΙΩΡΓΟΣ
   language: el
   title: ΕΣΠΕΡΙΝΑ
   dewey: 889.1 ΑΝΩ
   entry_numbers:
   - '1645'
   editor: None // ΑΘΗΝΑ
   edition_year: 1991
@@ -204986,15 +204801,15 @@
   authors:
   - ΠΑΠΑΔΗΜΗΤΡΙΟΥ,Κ.Κ
   language: el
   title: ΜΑΡΤΥΡΙΕΣ
   dewey: 889.1 ΠΑΠ
   entry_numbers:
   - '1679'
-  - '1978'
+  - '1678'
   editor: ΓΚΟΒΟΣΤΗΣ // ΑΘΗΝΑ
   edition_year: 1990
   pages: 78
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   - ΠΟΙΗΣΗ
@@ -205003,15 +204818,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 4027
     1: ΠΑΠΑΔΗΜΗΤΡΙΟΥ,Κ.Κ
     2: ΜΑΡΤΥΡΙΕΣ
     4: 889.1ΠΑΠ
-    5: 1679-1978
+    5: 1679-1678
     8: ΓΚΟΒΟΣΤΗΣ
     9: ΑΘΗΝΑ
     10: '1990'
     11: 78Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΠΟΙΗΣΗ
@@ -205432,15 +205247,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4036
   authors:
-  - ΑΘΑΝΑΣΟΥΛΗΣ,ΚΡΙΤΩΝ
+  - ΑΘΑΝΑΣΟΥΛΗΣ,ΚΡΙΤΩΝΑΣ
   language: el
   title: ΔΥΟ ΑΝΘΡΩΠΟΙ ΜΕΣΑ ΜΟΥ
   dewey: 889.1 ΑΘΑ
   entry_numbers:
   - '5956'
   editor: ΔΑΙΔΑΛΟΣ // ΑΘΗΝΑ
   edition_year: 1957
@@ -205583,15 +205398,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4039
   authors:
-  - ΒΑΡΒΙΤΣΙΩΤΗ,ΤΑΚΗ
+  - ΒΑΡΒΙΤΣΙΩΤΗΣ,ΤΑΚΗΣ
   language: el
   title: ΤΟ ΠΕΠΛΟ ΚΑΙ ΤΟ ΧΑΜΟΓΕΛΟ
   dewey: 889.1 ΒΑΡ
   entry_numbers:
   - '5979'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1963
@@ -206585,15 +206400,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4059
   authors:
-  - ΑΒΕΛΛΙΟΣ,ΑΘΑΝΑΣΙΟΣ
+  - ΑΒΕΛΙΟΣ,ΑΘΑΝΑΣΙΟΣ
   language: el
   title: ΤΟ ΒΙΟΣ ΤΟΥ ΑΠΟΛΥΤΟΥ
   dewey: 889.1 ΑΒΕ
   entry_numbers:
   - '5959'
   editor: None // ΑΘΗΝΑ
   edition_year: 1976
@@ -207089,41 +206904,40 @@
     29: null
     30: null
 - dbase_number: 4069
   authors:
   - ΠΑΠΑΔΙΤΣΑΣ,Δ.Π
   language: el
   title: ΠΟΙΗΣΗ 1
-  dewey: 889.1 ΠΑΠ
-  entry_numbers:
-  - '2604'
+  dewey: 889.11 ΠΑΠ
+  entry_numbers: []
   editor: ΠΡΩΤΗ ΥΛΗ // ΑΘΗΝΑ
   edition_year: 1963
   pages: 132
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   - ΠΟΙΗΣΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 4069
     1: ΠΑΠΑΔΙΤΣΑΣ,Δ.Π
     2: ΠΟΙΗΣΗ 1
-    4: 889.1ΠΑΠ
-    5: '2604'
+    4: 889.11ΠΑΠ
     8: ΠΡΩΤΗ ΥΛΗ
     9: ΑΘΗΝΑ
     10: '1963'
     11: 132Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΠΟΙΗΣΗ
     3: null
+    5: null
     6: null
     7: null
     15: null
     16: null
     17: null
     18: null
     19: null
@@ -207286,15 +207100,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4073
   authors:
-  - ΒΑΦΟΠΟΥΛΟΥ,Γ.Θ
+  - ΒΑΦΟΠΟΥΛΟΣ,Γ.,Θ.
   language: el
   title: Η ΜΕΓΑΛΗ ΝΥΧΤΑ ΚΑΙ ΤΟ ΠΑΡΑΘΥΡΟ
   dewey: 889.1 ΒΑΦ
   entry_numbers:
   - '5989'
   editor: ΔΙΦΡΟΣ // ΑΘΗΝΑ
   edition_year: 1959
@@ -207386,15 +207200,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4075
   authors:
-  - ΑΒΕΛΛΙΟΣ,ΑΘΑΝΑΣΙΟΣ
+  - ΑΒΕΛΙΟΣ,ΑΘΑΝΑΣΙΟΣ
   language: el
   title: Η ΠΕΝΘΙΜΗ ΔΟΞΑ
   dewey: 889.1 ΑΒΕ
   entry_numbers:
   - '5953'
   editor: None // ΑΘΗΝΑ
   edition_year: 1959
@@ -210096,15 +209910,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4129
   authors:
-  - ΑΒΕΛΛΙΟΣ,ΑΘΑΝΑΣΙΟΣ
+  - ΑΒΕΛΙΟΣ,ΑΘΑΝΑΣΙΟΣ
   language: el
   title: Ο ΜΕΤΑΜΦΙΕΣΜΕΝΟΣ ΚΑΙΡΟΣ
   dewey: 889.1 ΑΒΕ
   entry_numbers:
   - '5958'
   editor: None // ΑΘΗΝΑ
   edition_year: 1957
@@ -211301,15 +211115,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4153
   authors:
-  - ΑΡΚΟΜΑΝΗ,ΣΕΡΑΦΕΙΜ
+  - ΑΡΚΟΜΑΝΗΣ,ΣΕΡΑΦΕΙΜ
   language: el
   title: ΤΣΟΥΚΝΙΔΕΣ
   dewey: 889.1 ΑΡΚ
   entry_numbers:
   - '5938'
   editor: None // ΑΘΗΝΑ
   edition_year: 1936
@@ -211953,15 +211767,15 @@
 - dbase_number: 4166
   authors:
   - ΓΑΡΙΔΗΣ,ΚΩΣΤΑΣ
   language: el
   title: ΖΗΤΗΜΑ ΠΛΕΥΣΕΩΣ
   dewey: 889.1 ΓΑΡ
   entry_numbers:
-  - '6041'
+  - '6011'
   editor: ΣΕΙΡΙΟΣ // ΑΘΗΝΑ
   edition_year: 1975
   pages: 32
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   - ΠΟΙΗΣΗ
@@ -211969,15 +211783,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 4166
     1: ΓΑΡΙΔΗΣ,ΚΩΣΤΑΣ
     2: ΖΗΤΗΜΑ ΠΛΕΥΣΕΩΣ
     4: 889.1ΓΑΡ
-    5: '6041'
+    5: '6011'
     8: ΣΕΙΡΙΟΣ
     9: ΑΘΗΝΑ
     10: '1975'
     11: 32Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΠΟΙΗΣΗ
@@ -212450,15 +212264,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4176
   authors:
-  - ΒΑΛΕΝΤΙΝΗ
+  - ΒΑΛΕΝΤΙΝΗ,
   language: el
   title: ΠΟΘΟΙ ΣΥΝΩΜΟΤΕΣ
   dewey: 889.1 ΒΑΛ
   entry_numbers:
   - '4726'
   editor: ΠΑΠΑΖΗΣΗ // ΑΘΗΝΑ
   edition_year: 1982
@@ -213302,15 +213116,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4193
   authors:
-  - ΑΝΩΒΟΛΙΩΤΗ,ΓΙΩΡΓΟΥ
+  - ΑΝΩΒΟΛΙΩΤΗΣ,ΓΙΩΡΓΟΣ
   language: el
   title: ΕΛΛΙΜΕΝΙΣΜΕΝΑ
   dewey: 889.1 ΑΝΩ
   entry_numbers:
   - '4620'
   editor: None // ΑΘΗΝΑ
   edition_year: 1989
@@ -215759,15 +215573,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4242
   authors:
-  - ΒΑΛΙΟΥΛΗ,ΣΤΕΡΓΙΟΥ
+  - ΒΑΛΙΟΥΛΗΣ,ΣΤΕΡΓΙΟΣ
   language: el
   title: ΑΠΛΑ ΜΟΤΙΒΑ
   dewey: 889.1 ΒΑΛ
   entry_numbers:
   - '5977'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1964
@@ -216618,15 +216432,14 @@
 - dbase_number: 4259
   authors:
   - ΚΑΡΟΥΖΟΥ,Ν.Δ
   language: el
   title: Ο ΥΠΝΟΣΑΚΚΟΣ
   dewey: 889.1 ΚΑΡ
   entry_numbers:
-  - '6142'
   - '6143'
   editor: None // ΑΘΗΝΑ
   edition_year: 1964
   pages: 58
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
@@ -216636,15 +216449,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 4259
     1: ΚΑΡΟΥΖΟΥ,Ν.Δ
     2: Ο ΥΠΝΟΣΑΚΚΟΣ
     4: 889.1ΚΑΡ
-    5: 6142-6143
+    5: '6143'
     9: ΑΘΗΝΑ
     10: '1964'
     11: 58Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΠΟΙΗΣΗ
     17: 2 ΑΝΤΙΤΥΠΑ
@@ -216819,17 +216632,17 @@
     30: null
 - dbase_number: 4263
   authors:
   - ΧΡΙΣΤΙΑΝΟΠΟΥΛΟΣ,ΝΤΙΝΟΣ
   language: el
   title: ΠΟΙΗΜΑΤΑ
   subtitle: 1950-1955
-  dewey: 889.1 ΧΡΙ
+  dewey: 889.11 ΧΡΙ
   entry_numbers:
-  - '2587'
+  - '2215'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1957
   pages: 52
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   - ΠΟΙΗΣΗ
@@ -216837,16 +216650,16 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 4263
     1: ΧΡΙΣΤΙΑΝΟΠΟΥΛΟΣ,ΝΤΙΝΟΣ
     2: ΠΟΙΗΜΑΤΑ
     3: 1950-1955
-    4: 889.1ΧΡΙ
-    5: '2587'
+    4: 889.11ΧΡΙ
+    5: '2215'
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '1957'
     11: 52Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΠΟΙΗΣΗ
     6: null
@@ -216968,33 +216781,33 @@
     29: null
     30: null
 - dbase_number: 4266
   authors:
   - ΔΗΜΟΥΛΑ,ΑΘΟΥ
   language: el
   title: ΕΝΔΟΝ
-  dewey: 889.1 ΔΗΜ
+  dewey: 889.11 ΔΗΜ
   entry_numbers:
-  - '2750'
+  - '2756'
   editor: ΔΙΦΡΟΣ // ΑΘΗΝΑ
   edition_year: 1960
   pages: 36
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   - ΠΟΙΗΣΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 4266
     1: ΔΗΜΟΥΛΑ,ΑΘΟΥ
     2: ΕΝΔΟΝ
-    4: 889.1ΔΗΜ
-    5: '2750'
+    4: 889.11ΔΗΜ
+    5: '2756'
     8: ΔΙΦΡΟΣ
     9: ΑΘΗΝΑ
     10: '1960'
     11: 36Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΠΟΙΗΣΗ
@@ -218166,15 +217979,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4290
   authors:
-  - ΒΕΜΗ,ΜΠΙΛΛΥ
+  - ΒΕΜΗ,ΜΠΙΛΗ
   language: el
   title: ΝΕΛΤΟ
   dewey: 889.1 ΒΕΜ
   entry_numbers:
   - '5984'
   editor: None // ΑΘΗΝΑ
   edition_year: 1966
@@ -218716,15 +218529,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4301
   authors:
-  - ΑΘΑΝΑΣΟΥΛΗΣ,ΚΡΙΤΩΝ
+  - ΑΘΑΝΑΣΟΥΛΗΣ,ΚΡΙΤΩΝΑΣ
   language: el
   title: ΕΝΑΣ ΠΟΙΗΤΗΣ ΣΤΟ ΔΡΟΜΟ
   subtitle: ΚΑΙ ΟΙ ΣΑΤΙΡΕΣ ΓΙΑ ΤΗ ΛΕΟΝΩΡΑ
   dewey: 889.1 ΑΘΑ
   entry_numbers:
   - '5966'
   editor: None // ΑΘΗΝΑ
@@ -219420,15 +219233,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4315
   authors:
-  - ΒΑΣΙΛΕΙΟΥ,ΑΛΕΚΟΥ
+  - ΒΑΣΙΛΕΙΟΥ,ΑΛΕΚΟΣ
   language: el
   title: ΕΠΟΠΤΕΙΑ ΣΤΗΝ ΑΝΕΚΔΟΤΗ ΠΟΙΗΣΗ ΤΟΥ ΦΟΙΒΟΥ ΔΕΛΦΗ
   dewey: 889.1 ΒΑΣ
   entry_numbers:
   - '4589'
   editor: ΙΩΛΚΟΣ // ΑΘΗΝΑ
   edition_year: 1971
@@ -220072,15 +219885,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4328
   authors:
-  - ΑΜΠΑΤΗ,ΓΕΡΑΣΙΜΟΥ
+  - ΑΜΠΑΤΗΣ,ΓΕΡΑΣΙΜΟΣ
   language: el
   title: ΟΙ ΝΕΟΙ ΚΕΝΤΑΥΡΟΙ
   dewey: 889.1 ΑΜΠ
   entry_numbers:
   - '5968'
   editor: None // ΑΘΗΝΑ
   edition_year: 1956
@@ -220323,15 +220136,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4333
   authors:
-  - ΑΜΑΡΥΛΛΙΣ
+  - ΚΟΝΤΡΑΡΟΥ,ΑΜΑΡΥΛΛΙΣ,ΕΛΕΝΗ
   language: el
   title: ΟΙΩΝΟΙ
   dewey: 889.1 ΑΜΑ
   entry_numbers:
   - '4595'
   editor: ΜΑΥΡΙΔΗΣ // ΑΘΗΝΑ
   edition_year: 1980
@@ -223877,15 +223690,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4404
   authors:
-  - ΑΘΑΝΑΣΟΥΛΗΣ,ΚΡΙΤΩΝ
+  - ΑΘΑΝΑΣΟΥΛΗΣ,ΚΡΙΤΩΝΑΣ
   language: el
   title: Η ΕΠΙΣΚΕΨΗ ΤΟΥ ΑΓΓΕΛΟΥ
   dewey: 889.1 ΑΘΑ
   entry_numbers:
   - '5957'
   editor: ΝΕΣΤΩΡ // ΑΘΗΝΑ
   edition_year: 1961
@@ -224478,15 +224291,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4416
   authors:
-  - ΒΕΛΜΥΡΑ,ΚΩΣΤΗ
+  - ΒΕΛΜΥΡΑΣ,ΚΩΣΤΗΣ
   language: el
   title: ΕΙΔΩΛΙΑ
   dewey: 889.1 ΒΕΛ
   entry_numbers:
   - '5985'
   editor: Ε.Δ.Ε.Β // ΑΘΗΝΑ
   edition_year: 1961
@@ -225082,15 +224895,15 @@
 - dbase_number: 4428
   authors:
   - ΠΑΠΑΠΟΛΙΤΗΣ,ΣΩΤΗΡΗΣ
   language: el
   title: ΔΑΚΡΥΑ ΔΙΧΩΣ ΤΙΤΛΟΥΣ...
   dewey: 889.1 ΠΑΠ
   entry_numbers:
-  - '6363'
+  - '6323'
   editor: ΙΚΑΡΟΣ // ΑΘΗΝΑ
   edition_year: 1965
   pages: 81
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   - ΠΟΙΗΣΗ
@@ -225098,15 +224911,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 4428
     1: ΠΑΠΑΠΟΛΙΤΗΣ,ΣΩΤΗΡΗΣ
     2: ΔΑΚΡΥΑ ΔΙΧΩΣ ΤΙΤΛΟΥΣ...
     4: 889.1ΠΑΠ
-    5: '6363'
+    5: '6323'
     8: ΙΚΑΡΟΣ
     9: ΑΘΗΝΑ
     10: '1965'
     11: 81Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΠΟΙΗΣΗ
@@ -227279,15 +227092,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4472
   authors:
-  - ΑΝΥΦΑΝΤΗ,ΓΙΩΡΓΟΥ
+  - ΑΝΥΦΑΝΤΗΣ,ΓΙΩΡΓΟΣ
   language: el
   title: ΤΟ ΔΩΡΟ ΤΟΥ ΠΟΙΗΤΗ
   dewey: 889.1 ΑΝΥ
   entry_numbers:
   - '4739'
   editor: None // ΚΑΡΔΙΤΣΑ
   edition_year: 1996
@@ -227580,15 +227393,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4478
   authors:
-  - ΒΙΤΑΛΗ,ΦΙΛΑΡΕΤΟΥ
+  - ΒΙΤΑΛΗΣ,ΦΙΛΑΡΕΤΟΣ
   language: el
   title: Η ΙΕΡΑ ΜΟΝΗ ΖΑΛΟΓΓΟΥ
   dewey: 230 ΒΙΤ
   entry_numbers:
   - '294'
   editor: ΣΩΤ.ΣΠΥΡΟΠΟΥΛΟΣ // ΑΘΗΝΑ
   edition_year: 1959
@@ -228124,15 +227937,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4489
   authors:
-  - ΒΙΤΑΛΗ,ΦΙΛΑΡΕΤΟΥ
+  - ΒΙΤΑΛΗΣ,ΦΙΛΑΡΕΤΟΣ
   language: el
   title: Ο ΑΠΟΣΤΟΛΟΣ ΠΑΥΛΟΣ ΕΝ ΔΙΩΓΜΟΙΣ!...
   dewey: 230 ΒΙΤ
   entry_numbers:
   - '608'
   editor: Ι.Μ.ΝΙΚΟΠΟΛ.ΠΡΕΒΕΖΗΣ // ΑΘΗΝΑ
   edition_year: 1969
@@ -228672,15 +228485,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4500
   authors:
-  - ΒΙΤΑΛΗΣ,ΦΙΛΑΡΕΤΟΥ
+  - ΒΙΤΑΛΗΣ,ΦΙΛΑΡΕΤΟΣ
   language: el
   title: Ο ΜΗΤΡΟΠΟΛΙΤΗΣ ΤΗΝΟΥ ΓΑΒΡΙΗΛ
   dewey: 230 ΒΙΤ
   entry_numbers:
   - '4739'
   editor: ΙΕΡΑ ΜΗΤΡΟΠ ΠΡΕΒΕΖΑΣ // None
   edition_year: 1957
@@ -229117,15 +228930,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4509
   authors:
-  - ΒΙΤΑΛΗ,ΦΙΛΑΡΕΤΟΥ
+  - ΒΙΤΑΛΗΣ,ΦΙΛΑΡΕΤΟΣ
   language: el
   title: Ο ΗΠΕΙΡΩΤΗΣ ΜΑΞΙΜΟΣ ΩΣ ΠΡΟΜΑΧΟΣ ΤΗΣ ΟΡΘΟΔΟΞΙΑΣ ΕΝ ΡΩΣΙΑ
   dewey: 230 ΒΙΤ
   entry_numbers:
   - '4754'
   editor: None // ΑΘΗΝΑ
   edition_year: 1965
@@ -232316,15 +232129,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4574
   authors:
-  - ΒΙΤΑΛΗ,ΦΙΛΑΡΕΤΟΥ
+  - ΒΙΤΑΛΗΣ,ΦΙΛΑΡΕΤΟΣ
   language: el
   title: ΦΩΤΙΟΣ Ο Β'
   dewey: 230 ΒΙΤ
   entry_numbers:
   - '6590'
   editor: None // ΑΘΗΝΑ
   edition_year: 1965
@@ -232365,15 +232178,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4575
   authors:
-  - ΒΑΛΜΑ,ΣΤΑΜΑΤΗ
+  - ΒΑΛΜΑΣ,ΣΤΑΜΑΤΗΣ
   language: el
   title: ΣΤΙΣ ΠΗΓΕΣ ΤΩΝ ΥΔΑΤΩΝ
   dewey: 230 ΒΑΛ
   entry_numbers:
   - '6598'
   editor: None // ΑΘΗΝΑ
   edition_year: 1980
@@ -234612,15 +234425,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4621
   authors:
-  - ΑΛΕΞΑΝΔΡΟΠΟΥΛΟΥ,ΜΗΤΣΟΥ
+  - ΑΛΕΞΑΝΔΡΟΠΟΥΛΟΣ,ΜΗΤΣΟΣ
   language: el
   title: ΣΚΗΝΕΣ ΑΠΟ ΤΟ ΒΙΟ ΤΟΥ ΜΑΞΙΜΟΥ ΤΟΥ ΓΡΑΙΚΟΥ
   dewey: 230 ΑΛΕ
   entry_numbers:
   - '1674'
   editor: ΔΙΦΡΟΣ // ΑΘΗΝΑ
   edition_year: 1975
@@ -234661,15 +234474,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4622
   authors:
-  - ΒΑΣΙΛΕΙΟΥ,ΠΑΝΟΥ
+  - ΒΑΣΙΛΕΙΟΥ,ΠΑΝΟΣ
   language: el
   title: ΕΥΓΕΝΙΟΣ ΓΙΑΝΝΟΥΛΗΣ Ο ΑΙΤΩΛΟΣ ΚΑΙ ΟΙ ΣΠΟΥΔΑΙΟΤΕΡΟΙ ΜΑΘΗΤΕΣ Τ
   subtitle: ΤΩΝ ΣΧΟΛΩΝ ΤΩΝ ΑΓΡΑΦΩΝ
   dewey: 230 ΒΑΣ
   entry_numbers:
   - '611'
   editor: None // ΑΘΗΝΑ
@@ -234759,15 +234572,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4624
   authors:
-  - ΑΓΓΕΛΙΝΑΡΑ,ΓΕΩΡΓΙΟΥ
+  - ΑΓΓΕΛΙΝΑΡΑΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΘΡΑΣΥΒΟΥΛΟΣ ΣΤΑΝΙΤΣΑΣ
   subtitle: ΑΡΧΩΝ ΠΡΩΤΟΨΑΛΤΗΣ ΤΗΣ ΜΕΓΑΛΗΣ ΤΟΥ ΧΡΙΣΤΟΥ ΕΚΚΛΗΣΙΑΣ
   dewey: 230 ΑΓΓ
   entry_numbers:
   - '1729'
   editor: ΚΟΥΛΤΟΥΡΑ // ΑΘΗΝΑ
@@ -234907,15 +234720,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4627
   authors:
-  - ΑΛΕΞΙΑΔΗ,ΜΗΝΑ
+  - ΑΛΕΞΙΑΔΗΣ,ΜΗΝΑΣ
   language: el
   title: ΕΘΙΜΙΚΟΙ ΕΚΚΛΗΣΙΑΣΤΙΚΟΙ ΠΛΕΙΣΤΗΡΙΑΣΜΟΙ
   dewey: 230 ΑΛΕ
   entry_numbers:
   - '579'
   editor: None // ΙΩΑΝΝΙΝΑ
   edition_year: 1977
@@ -234955,15 +234768,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4628
   authors:
-  - ΒΛΑΧΟΥ,ΠΑΝΑΓΙΩΤΗ
+  - ΒΛΑΧΟΥ,ΠΑΝΑΓΙΩΤΗΣ
   language: el
   title: ΣΥΝΑΞΙΣ ΕΥΓΕΝΙΟΣ Ο ΑΙΤΩΛΟΣ ΚΑΙ Η ΕΠΟΧΗ ΤΟΥ
   entry_numbers:
   - '1724'
   editor: None // ΑΘΗΝΑ
   edition_year: 1986
   pages: 706
@@ -235944,15 +235757,15 @@
   authors:
   - ΝΤΙΚΕΝΣ,ΚΑΡΟΛΟΣ
   language: el
   title: ΟΛΙΒΕΡ ΤΟΥΙΣΤ
   dewey: 808.899 ΝΤΙ
   entry_numbers:
   - '4787'
-  - 9194Α
+  - 09194
   translators:
   - ΣΤΡΑΤΙΚΗΣ,Π.
   editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
   edition_year: 1991
   pages: 122
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -235962,15 +235775,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 4648
     1: ΝΤΙΚΕΝΣ,ΚΑΡΟΛΟΣ
     2: ΟΛΙΒΕΡ ΤΟΥΙΣΤ
     4: 808.899ΝΤΙ
-    5: 4787,9194Α
+    5: 4787-09194
     6: Π.ΣΤΡΑΤΙΚΗΣ
     8: ΑΓΚΥΡΑ
     9: ΑΘΗΝΑ
     10: '1991'
     11: 122Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -236389,15 +236202,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4657
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: ΠΕΡΙΠΕΤΕΙΕΣ ΚΙΝΕΖΟΥ ΣΤΗΝ ΚΙΝΑ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '6679'
   editor: ΑΣΤΗΡ // ΑΘΗΝΑ
   edition_year: 1958
@@ -236537,15 +236350,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4660
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  - VERNE,JULES
   language: el
   title: ΟΙ ΑΔΕΛΦΟΙ ΚΙΠ
   dewey: 880.09 ΒΕΡ
   entry_numbers:
   - '6684'
   translators:
   - ΤΣΙΜΙΚΑΛΗ,ΠΙΠΙΝΑ
@@ -236795,14 +236608,15 @@
     29: null
     30: null
 - dbase_number: 4665
   authors:
   - ΚΡΟΝΙΝ,Α
   language: el
   title: ΤΑ ΑΓΟΥΡΑ ΧΡΟΝΙΑ
+  dewey: 808.899 ΚΡΟ
   entry_numbers:
   - '6666'
   - '9596'
   - '20585'
   translators:
   - ΜΑΥΡΟΕΙΔΗ-ΠΑΠΑΔΑΚΗ,ΣΟΦΙΑ
   editor: ΑΣΤΗΡ // ΑΘΗΝΑ
@@ -236814,15 +236628,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 4665
     1: ΚΡΟΝΙΝ,Α
     2: ΤΑ ΑΓΟΥΡΑ ΧΡΟΝΙΑ
-    4: 8Ο8.899ΚΡΟ
+    4: 808.899ΚΡΟ
     5: 6666,9596,20585
     6: ΠΑΠΑΔΑΚΗ-ΜΑΥΡΟΕΙΔΗ,Σ
     8: ΑΣΤΗΡ
     9: ΑΘΗΝΑ
     10: '1978'
     11: 320Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
@@ -238405,15 +238219,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 4697
   authors:
-  - ΑΛΕΞΙΑΔΗ,ΜΗΝΑ
+  - ΑΛΕΞΙΑΔΗΣ,ΜΗΝΑΣ
   language: el
   title: Η ΕΛΛΗΝΙΚΗ ΚΑΙ ΔΙΕΘΝΗΣ ΕΠΙΣΤΗΜΟΝΙΚΗ ΟΡΟΛΟΓΙΑ ΤΗΣ ΛΑΟΓΡΑΦΙΑΣ
   dewey: 398 ΑΛΕ
   entry_numbers:
   - '6541'
   editor: None // ΙΩΑΝΝΙΝΑ
   edition_year: 1984
@@ -238807,15 +238621,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4705
   authors:
-  - ΑΝΑΓΝΩΣΤΟΠΟΥΛΟΥ,ΞΕΝΟΦΩΝΤΟΣ
+  - ΑΝΑΓΝΩΣΤΟΠΟΥΛΟΣ,ΞΕΝΟΦΩΝΤΑΣ
   language: el
   title: ΛΑΟΓΡΑΦΙΚΑ ΡΟΥΜΕΛΗΣ
   dewey: 398 ΑΝΑ
   entry_numbers:
   - '786'
   editor: None // ΑΘΗΝΑ
   edition_year: 1955
@@ -239053,15 +238867,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4710
   authors:
-  - ΒΟΥΡΝΑΣ,ΤΑΣΟΣ-ΓΑΡΙΔΗ,ΕΛΕΝΗ
+  - ΒΟΥΡΝΑΣ,ΤΑΣΟΣ
+  - ΓΑΡΙΔΗ,ΕΛΕΝΗ
   language: el
   title: Η ΠΑΡΑΔΟΣΗ ΚΑΙ Η ΕΠΙΒΙΩΣΗ ΤΗΣ ΣΤΟ ΣΗΜΕΡΙΝΟ ΠΟΛΙΤΙΣΜΟ ΜΑΣ
   dewey: 398 ΒΟΥ
   entry_numbers:
   - '686'
   editor: ΤΟΛΙΔΗ // ΑΘΗΝΑ
   pages: 200
@@ -239696,15 +239511,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4723
   authors:
-  - ΑΛΕΞΙΑΔΗ,ΜΗΝΑ
+  - ΑΛΕΞΙΑΔΗΣ,ΜΗΝΑΣ
   language: el
   title: ΗΠΕΙΡΩΤΙΚΑ ΧΕΙΡΟΓΡΑΦΑ ΛΑΟΓΡΑΦΙΑΣ ΠΑΝΕΠΙΣΤΗΜΙΟΥ ΙΩΑΝΝΙΝΩΝ
   dewey: 398 ΑΛΕ
   entry_numbers:
   - '831'
   editor: None // ΙΩΑΝΝΙΝΑ
   edition_year: 1980
@@ -239843,15 +239658,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4726
   authors:
-  - ΒΕΤΣΟΠΟΥΛΟΥ,ΒΑΣΙΛΕΙΟΥ
+  - ΒΕΤΣΟΠΟΥΛΟΣ,ΒΑΣΙΛΕΙΟΣ
   language: el
   title: Ο ΓΑΜΟΣ ΣΤΗ ΠΥΡΣΟΓΙΑΝΝΗ ΤΑ ΠΑΛΙΑ ΤΑ ΧΡΟΝΙΑ
   dewey: 398 ΒΕΤ
   entry_numbers:
   - '4806'
   editor: None // ΑΘΗΝΑ
   edition_year: 1973
@@ -240142,15 +239957,18 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4732
   authors:
-  - ΑΓΓΕΛΙΩΝΑ,Δ.
+  - ΑΓΓΕΛΙΩΝΙΑ,Δ.
+  - ΠΕΤΡΟΥΔΑΣ,Γ.
+  - ΑΝΤΖΑΝΟΣ,ΑΝΤ.
+  - ΣΤΕΡΓΙΟΥ,ΔΗΜ.
   language: el
   title: Η ΑΚΡΙΤΙΚΗ ΣΑΜΟΘΡΑΚΗ
   dewey: 398 ΑΓΓ
   entry_numbers:
   - '791'
   editor: None // ΑΘΗΝΑ
   pages: 102
@@ -242899,15 +242717,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4788
   authors:
-  - ΒΟΥΡΒΕΡΗ,ΚΩΝΣΤΑΝΤΙΝΟΥ
+  - ΒΟΥΡΒΕΡΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΠΡΟΒΛΗΜΑΤΑ ΜΟΡΦΩΣΕΩΣ ΤΟΥ ΕΡΓΑΖΟΜΕΝΟΥ ΛΑΟΥ
   entry_numbers:
   - '4818'
   editor: ΕΛΛ.ΑΝΘΡΩΠΙΣΤΙΚΗ ΕΤ // ΑΘΗΝΑ
   edition_year: 1962
   pages: 16
@@ -244420,15 +244238,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4819
   authors:
-  - ΑΓΓΕΛΟΠΟΥΛΟΥ,ΑΓΓΕΛΟΥ
+  - ΑΓΓΕΛΟΠΟΥΛΟΣ,ΑΓΓΕΛΟΣ
   language: el
   title: Η ΑΛΗΘΕΙΑ ΓΙΑ ΤΑΣ ΕΚΤΡΩΣΕΙΣ
   entry_numbers:
   - '862'
   editor: ΛΥΧΝΟΣ // ΑΘΗΝΑ
   edition_year: 1980
   pages: 119
@@ -246408,15 +246226,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4860
   authors:
-  - Β'ΝΕΟΓΝΙΚΟ ΤΜΗΜ.ΝΟΣ.ΠΑΙΔΩΝ ΑΓΙΑ ΣΟΦΙΑ
+  - Β' ΝΕΟΓΝΙΚΟ ΤΜΗΜΑ ΝΟΣΟΚΟΜΕΙΟΥ ΠΑΙΔΩΝ ΑΓΙΑ ΣΟΦΙΑ
   language: el
   title: ΝΕΥΡΟΛΟΓΙΑ ΕΜΒΡΥΟΥ ΚΑΙ ΝΕΟΓΝΟΥ
   entry_numbers:
   - '3054'
   editor: ΒΗΤΑ // ΑΘΗΝΑ
   edition_year: 1991
   pages: 101
@@ -246747,15 +246565,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4867
   authors:
-  - ΑΝΔΡΟΥΛΑΚΗΣ,Γ.-ΒΑΣΙΛΕΙΟΥ,Ι.
+  - ΑΝΔΡΟΥΛΑΚΗΣ,ΓΕΩΡΓΙΟΣ
+  - ΒΑΣΙΛΕΙΟΥ,ΙΩΑΝΝΗΣ
   title: ΠΡΟΟΔΟΙ ΣΤΟ SHOCK
   entry_numbers:
   - '3059'
   editor: ΒΗΤΑ // None
   pages: 112
   topics:
   - ΙΑΤΡΙΚΗ
@@ -246988,15 +246807,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4872
   authors:
-  - ΑΝΔΡΟΥΛΙΔΑΚΗ,ΣΤΑΥΡΟΥ
+  - ΑΝΔΡΟΥΛΙΔΑΚΗΣ,ΣΤΑΥΡΟΣ
   language: el
   title: ΣΤΟΙΧΕΙΑ ΕΔΑΦΟΛΟΓΙΑΣ ΚΑΙ ΓΕΩΡΓΙΚΩΝ ΜΗΧΑΝΗΜΑΤΩΝ
   entry_numbers:
   - '6419'
   editor: ΕΥΓΕΝΙΔΙΟ ΙΔΡΥΜΑ // ΑΘΗΝΑ
   edition_year: 1979
   pages: 167
@@ -247228,15 +247047,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4877
   authors:
-  - ΑΝΑΣΗ,ΕΜΜ.
+  - ΑΝΑΣΗΣ,ΕΜΜΑΝΟΥΗΛ
   language: el
   title: Ο ΠΡΑΚΤΙΚΟΣ ΟΔΗΓΟΣ ΤΟΥ ΒΑΜΒΑΚΟΚΑΛΛΙΕΡΓΗΤΟΥ
   entry_numbers:
   - '6003'
   editor: ΣΠ.ΣΠΥΡΟΥ // ΑΘΗΝΑ
   edition_year: 1959
   pages: 175
@@ -250492,40 +250311,39 @@
     29: null
     30: null
 - dbase_number: 4943
   authors:
   - ΕΥΓΕΝΙΔΙΟ ΙΔΡΥΜΑ
   language: el
   title: ΟΙΚΟΔΟΜΙΚΗ
-  entry_numbers:
-  - '5788'
+  entry_numbers: []
   editor: ΕΥΓΕΝΙΔΙΟ ΙΔΡΥΜΑ // ΑΘΗΝΑ
   edition_year: 1975
   pages: 348
   topics:
   - ΟΙΚΟΔΟΜΙΚΗ
   volume: ΤΟΜΟΣ Β'
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 4943
     1: ΕΥΓΕΝΙΔΙΟ ΙΔΡΥΜΑ
     2: ΟΙΚΟΔΟΜΙΚΗ
-    5: '5788'
     8: ΕΥΓΕΝΙΔΙΟ ΙΔΡΥΜΑ
     9: ΑΘΗΝΑ
     10: '1975'
     11: 348Σ
     12: ΟΙΚΟΔΟΜΙΚΗ
     13: ΟΙΚΟΔΟΜΙΚΗ
     14: ΟΙΚΟΔΟΜΙΚΗ
     17: ΤΟΜΟΣ Β'
     3: null
     4: null
+    5: null
     6: null
     7: null
     15: null
     16: null
     18: null
     19: null
     20: null
@@ -252108,15 +251926,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4976
   authors:
-  - ΒΟΚΟΒΙΤΣ,ΝΙΚΟΥ
+  - ΒΟΚΟΒΙΤΣ,ΝΙΚΟΣ
   language: el
   title: Ο ΘΕΟΣ ΕΙΝΑΙ ΔΙΚΟΣ ΜΑΣ
   dewey: 886.2 ΒΟΚ
   entry_numbers:
   - '4883'
   editor: None // ΑΘΗΝΑ
   edition_year: 1995
@@ -253002,15 +252820,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 4994
   authors:
-  - ΑΡΜΕΝΤΟ ΒΙΤΟ
+  - D'ARMENTO,VITO,ANTONIO
   language: el
   title: ΕΛΑΦΡΑ ΑΠΟΣΚΕΗ
   subtitle: ΠΟΙΗΜΑΤΑ
   dewey: 851 ΑΡΜ
   entry_numbers:
   - '5023'
   translators:
@@ -255081,37 +254899,36 @@
     29: null
     30: null
 - dbase_number: 5036
   authors:
   - BARNARD & EDWARDS
   language: el
   title: ΘΕΜΕΛΙΩΔΕΙΣ ΑΡΧΑΙ ΤΗΣ ΦΥΣΙΚΗΣ
-  entry_numbers:
-  - '5892'
+  entry_numbers: []
   editor: ΠΕΧΛΙΒΑΝΙΔΗΣ // ΑΘΗΝΑ
   pages: 704
   topics:
   - ΦΥΣΙΚΗ
   - ΘΕΜΕΛΙΩΔΕΙΣ ΑΡΧΕΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 5036
     1: BARNARD & EDWARDS
     2: ΘΕΜΕΛΙΩΔΕΙΣ ΑΡΧΑΙ ΤΗΣ ΦΥΣΙΚΗΣ
-    5: '5892'
     8: ΠΕΧΛΙΒΑΝΙΔΗΣ
     9: ΑΘΗΝΑ
     11: 704Σ
     12: ΦΥΣΙΚΗ-ΘΕΜΕΛΙΩΔΕΙΣ ΑΡΧΕΣ
     13: ΘΕΜΕΛΙΩΔΕΙΣ ΑΡΧΕΣ-ΦΥΣΙΚΗ
     14: ΦΥΣΙΚΗ
     3: null
     4: null
+    5: null
     6: null
     7: null
     10: null
     15: null
     16: null
     17: null
     18: null
@@ -255414,15 +255231,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5043
   authors:
-  - ΒΑΣΙΛΟΠΟΥΛΟΥ,ΑΝΔΡ.
+  - ΒΑΣΙΛΟΠΟΥΛΟΣ,ΑΝΔΡΕΑΣ
   language: el
   title: ΧΗΜΕΙΑ
   entry_numbers:
   - '5820'
   editor: ΕΥΓΕΝΙΔΙΟ ΙΔΡΥΜΑ // ΑΘΗΝΑ
   edition_year: 1978
   pages: 142
@@ -256033,39 +255850,38 @@
     29: null
     30: null
 - dbase_number: 5056
   authors:
   - ΖΑΧΑΡΗ,ΕΥΣΤΑΘΙΟΥ
   language: el
   title: ΓΕΩΡΓΙΚΟΣ ΠΡΟΣΑΝΑΤΟΛΙΣΜΟΣ
-  entry_numbers:
-  - '5825'
+  entry_numbers: []
   editor: ΕΥΓΕΝΙΔΙΟ ΙΔΡΥΜΑ // ΑΘΗΝΑ
   edition_year: 1978
   pages: 126
   topics:
   - ΓΕΩΡΓΙΑ
   - ΓΕΩΡΓΙΚΟΣ ΠΡΟΣΑΝΑΤΟΛΙΣΜΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 5056
     1: ΖΑΧΑΡΗ,ΕΥΣΤΑΘΙΟΥ
     2: ΓΕΩΡΓΙΚΟΣ ΠΡΟΣΑΝΑΤΟΛΙΣΜΟΣ
-    5: '5825'
     8: ΕΥΓΕΝΙΔΙΟ ΙΔΡΥΜΑ
     9: ΑΘΗΝΑ
     10: '1978'
     11: 126Σ
     12: ΓΕΩΡΓΙΑ
     13: ΓΕΩΡΓΙΚΟΣ ΠΡΟΣΑΝΑΤΟΛΙΣΜΟΣ
     14: ΠΡΟΣΑΝΑΤΟΛΙΣΜΟΣ ΓΕΩΡΓΙΚΟΣ
     3: null
     4: null
+    5: null
     6: null
     7: null
     15: null
     16: null
     17: null
     18: null
     19: null
@@ -256126,15 +255942,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5058
   authors:
-  - ΒΑΛΑΩΡΑ,ΒΑΣΙΛΕΙΟΥ
+  - ΒΑΛΑΩΡΑΣ,ΒΑΣΙΛΕΙΟΣ
   language: el
   title: ΠΕΡΙΒΑΛΛΟΝ ΚΑΙ ΥΓΕΙΑ
   entry_numbers:
   - '5824'
   editor: ΕΥΓΕΝΙΔΙΟ ΙΔΡΥΜΑ // ΑΘΗΝΑ
   edition_year: 1978
   pages: 113
@@ -256366,15 +256182,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5063
   authors:
-  - ΒΑΛΑΩΡΑ,ΒΑΣΙΛΕΙΟΥ
+  - ΒΑΛΑΩΡΑΣ,ΒΑΣΙΛΕΙΟΣ
   language: el
   title: ΑΤΟΜΙΚΗ ΚΑΙ ΔΗΜΟΣΙΑ ΥΓΙΕΙΝΗ
   entry_numbers:
   - '6421'
   editor: ΕΥΓΕΝΙΔΙΟ ΙΔΡΥΜΑ // ΑΘΗΝΑ
   edition_year: 1979
   pages: 166
@@ -257520,15 +257336,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5087
   authors:
-  - ΑΠ.ΣΤΑΥΡΑΚΑ-ΔΗΜ,ΧΑΛΙΩΤΗ
+  - ΣΤΑΥΡΑΚΑΣ,ΑΠΟΣΤΟΛΟΣ
+  - ΧΑΛΙΩΤΗΣ,ΔΗΜΗΤΡΗΣ
   language: el
   title: ΑΣΚΗΣΕΙΣ ΜΑΘΗΜΑΤΙΚΩΝ
   entry_numbers: []
   editor: ΓΕΩΡΓΙΟΥ ΚΟΡΦΙΑΤΗ // ΑΘΗΝΑ
   pages: 208
   topics:
   - ΑΣΚΗΣΕΙΣ ΜΑΘΗΜΑΤΙΚΩΝ
@@ -258259,15 +258076,18 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5103
   authors:
-  - ΒΕΛΤΣΟΥ-ΚΡΙΑΡΑ-ΔΕΣΠΟΤΟΠΟΥΛΟΥ-ΜΠΑΜΠΙΝΙΩΤΗ
+  - ΒΕΛΤΣΟΣ,ΓΙΩΡΓΟΣ
+  - ΚΡΙΑΡΑΣ,ΕΜΜΑΝΟΥΗΛ
+  - ΔΕΣΠΟΤΟΠΟΥΛΟΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
+  - ΜΠΑΜΠΙΝΙΩΤΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΔΗΜΟΤΙΚΗ ΓΛΩΣΣΑ
   entry_numbers:
   - '4975'
   editor: ΓΡΗΓΟΡΗ // ΑΘΗΝΑ
   pages: 166
   topics:
@@ -258682,15 +258502,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5112
   authors:
-  - ΑΠΟΚΟΡΙΤΟΥ,ΕΥΑΓΓΕΛΟΥ
+  - ΑΠΟΚΟΡΙΤΟΣ,ΕΥΑΓΓΕΛΟΣ
   language: el
   title: ΔΙΕΘΝΕΙΣ ΣΥΓΚΟΙΝΩΝΙΑΙ ΙΣΤΟΡΙΚΑ ΣΤΑΥΡΟΔΡΟΜΙΑ ΚΑΙ ΜΕΤΑΦΟΡΑΙ
   entry_numbers:
   - '5917'
   editor: None // ΑΘΗΝΑ
   edition_year: 1953
   pages: 264
@@ -259163,15 +258983,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5122
   authors:
-  - ΑΝΑΓΝΩΣΤΟΠΟΥΛΟΥ,Ν.Η
+  - ΑΝΑΓΝΩΣΤΟΠΟΥΛΟΣ,Ν.,Η.
   language: el
   title: ΑΚΡΙΔΕΣ,ΑΡΟΥΡΑΙΟΙ ΚΑΙ ΠΟΝΤΙΚΙΑ
   entry_numbers:
   - '6015'
   editor: None // ΑΘΗΝΑ
   edition_year: 1928
   pages: 46
@@ -259261,15 +259081,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5124
   authors:
-  - ANDREWS,E.
+  - ANDREWS,H.
   language: el
   title: ΘΕΣΕΙΣ ΥΠΟΘΕΣΕΙΣ ΘΕΩΡΙΕΣ
   entry_numbers:
   - '7416'
   editor: ΠΕΡΓΑΜΟΣ // ΑΘΗΝΑ
   edition_year: 1983
   pages: 45
@@ -259356,15 +259176,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5126
   authors:
-  - ΑΝΔΡΕΑΔΗ,ΣΤΡΑΤΗ
+  - ΑΝΔΡΕΑΔΗΣ,ΣΤΡΑΤΗΣ
   language: el
   title: Η ΕΞΕΛΙΞΙΣ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΕΜΠΟΡΙΚΗΣ ΝΑΥΤΙΛΙΑΣ
   entry_numbers:
   - '4979'
   editor: None // ΑΘΗΝΑ
   edition_year: 1960
   pages: 33
@@ -260560,15 +260380,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5151
   authors:
-  - ΑΝΤΩΝΙΑΔΟΥ,ΔΗΜΗΤΡΙΟΥ
+  - ΑΝΤΩΝΙΑΔΗΣ,ΔΗΜΗΤΡΗΣ
   language: el
   title: ΑΙ ΠΥΡΑΜΙΔΕΣ ΚΑΙ ΟΙ ΙΔΡΥΤΑΙ ΤΩΝ
   dewey: 909 ΑΝΤ
   entry_numbers:
   - '4987'
   editor: ΡΟΔΑΚΗΣ // ΑΘΗΝΑ
   edition_year: 1960
@@ -261814,30 +261634,30 @@
   - ΜΑΜΜΟΠΟΥΛΟΥ,ΑΛΕΞΑΝΔΡΟΥ
   language: el
   title: ΑΓΓΕΛΙΚΗ ΧΑΤΖΗΜΙΧΑΛΗ ΚΑΙ Η ΗΠΕΙΡΩΤΙΚΗ ΛΑΙΚΗ ΤΕΧΝΗ
   dewey: 938.93 ΜΑΜ
   entry_numbers:
   - '693'
   - '2823'
-  - 9251Α
+  - 09251
   editor: None // ΑΘΗΝΑ
   edition_year: 1967
   pages: 47
   topics:
   - ΛΑΙΚΗ ΤΕΧΝΗ
   - ΑΓΓΕΛΙΚΗ ΧΑΤΖΗΜΙΧΑΛΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 5177
     1: ΜΑΜΜΟΠΟΥΛΟΥ,ΑΛΕΞΑΝΔΡΟΥ
     2: ΑΓΓΕΛΙΚΗ ΧΑΤΖΗΜΙΧΑΛΗ ΚΑΙ Η ΗΠΕΙΡΩΤΙΚΗ ΛΑΙΚΗ ΤΕΧΝΗ
     4: 938.93ΜΑΜ
-    5: 693-2823-9251Α
+    5: 693-2823-09251
     9: ΑΘΗΝΑ
     10: '1967'
     11: 47Σ
     12: ΛΑΙΚΗ ΤΕΧΝΗ-ΑΓΓΕΛΙΚΗ ΧΑΤΖΗΜΙΧΑΛΗ
     13: ΛΑΙΚΗ ΤΕΧΝΗ-ΑΓΓΕΛΙΚΗ ΧΑΤΖΗΜΙΧΑΛΗ
     14: ΛΑΙΚΗ ΤΕΧΝΗ-ΑΓΓΕΛΙΚΗ ΧΑΤΖΗΜΙΧΑΛΗ
     3: null
@@ -262147,15 +261967,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5184
   authors:
-  - ΑΝΔΡΟΝΙΚΟΥ,ΜΑΝΩΛΗ
+  - ΑΝΔΡΟΝΙΚΟΣ,ΜΑΝΩΛΗΣ
   language: el
   title: ΟΙ ΒΑΣΙΛΙΚΟΙ ΤΑΦΟΙ ΤΗΣ ΒΕΡΓΙΝΑΣ
   entry_numbers:
   - '4996'
   editor: None // ΑΘΗΝΑ
   edition_year: 1978
   pages: 55
@@ -262737,15 +262557,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5196
   authors:
-  - ΒΑΛΙΝΟΥ,ΓΙΑΝΝΗ
+  - ΒΑΛΙΝΟΣ,ΓΙΑΝΝΗΣ
   language: el
   title: ΜΙΑ ΓΕΥΣΗ ΖΩΗΣ
   dewey: 889.21 ΒΑΛ
   entry_numbers:
   - '5043'
   editor: None // ΑΘΗΝΑ
   edition_year: 1995
@@ -263507,15 +263327,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5212
   authors:
-  - ΑΝΤΩΝΙΟΥ ΝΙΚΟΛΑΟΥ ΑΘΑΝΑΣΑΚΗ
+  - ΑΘΑΝΑΣΑΚΗΣ,ΑΝΤΩΝΙΟΣ,ΝΙΚΟΛΑΟΥ
   language: el
   title: ΕΥΤΡΑΠΕΛΑ ΠΕΡΙΣΤΑΤΙΚΑ ΚΑΙ ΔΙΗΓΗΜΑΤΑ
   dewey: 889 ΑΘΑ
   entry_numbers:
   - '5080'
   editor: None // ΑΘΗΝΑ
   edition_year: 1998
@@ -263656,15 +263476,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5215
   authors:
-  - ΑΡΧΙΓΕΝΗ,ΔΗΜΗΤΡΗ
+  - ΑΡΧΙΓΕΝΗΣ,ΔΗΜΗΤΡΗΣ
   language: el
   title: ΑΝΤΙΛΑΛΟΙ
   dewey: 889.1 ΑΡΧ
   entry_numbers:
   - '5241'
   editor: None // ΑΘΗΝΑ
   edition_year: 1972
@@ -265023,15 +264843,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5243
   authors:
-  - ΑΞΙΩΤΗ,ΠΕΤΡΟΥ
+  - ΑΞΙΩΤΗΣ,ΠΕΤΡΟΣ,Ι.
   language: el
   title: ΤΟ ΜΕΓΑΛΟ ΞΥΠΝΗΜΑ
   dewey: 889.21 ΑΞΙ
   entry_numbers:
   - '2415'
   editor: None // ΑΘΗΝΑ
   pages: 420
@@ -265166,15 +264986,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5246
   authors:
-  - ΑΡΕΤΙΝΟΣ,ΝΤΑΒΙΝΟΥΣ
+  - ARETINO,PIETRO
   title: Η ΤΡΙΛΟΓΙΑ ΤΟΥ RAGIONAMENTI
   subtitle: Η ΝΑΝΑ ΚΑΛΟΓΡΙΑ-Η ΝΑΝΑ ΠΑΝΤΡΕΜΕΝΗ-Η ΝΑΝΑ ΕΤΑΙΡΑ
   dewey: 850.11 ΑΡΕ
   entry_numbers:
   - '5230'
   translators:
   - ΡΟΔΟΚΑΝΑΚΗ,Δ.Ν.
@@ -267847,15 +267667,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5300
   authors:
-  - ΒΑΒΛΙΔΑ,ΑΘΑΝΑΣΙΟΥ
+  - ΒΑΒΛΙΔΑΣ,ΑΘΑΝΑΣΙΟΣ
   language: el
   title: ΚΛΕΙΣΤΟΦΟΒΙΑ
   dewey: 886.2 ΒΑΒ
   entry_numbers:
   - '5122'
   editor: ΔΩΔΩΝΗ // ΑΘΗΝΑ
   edition_year: 1991
@@ -269075,15 +268895,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5326
   authors:
-  - ΑΡΑΓΚΟΝ
+  - ARAGON,LOUIS
   language: el
   title: Μ'ΑΝΟΙΧΤΑ ΧΑΡΤΙΑ
   dewey: 843 ΑΡΑ
   entry_numbers:
   - '5429'
   editor: ΘΕΜΕΛΙΟ // ΑΘΗΝΑ
   edition_year: 1965
@@ -269123,15 +268943,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5327
   authors:
-  - ΑΡΓΥΡΙΟΥ ΑΛΕΞΑΝΔΡΟΣ
+  - ΑΡΓΥΡΙΟΥ,ΑΛΕΞΑΝΔΡΟΣ
   language: el
   title: ΕΠΤΑ ΚΕΙΜΕΝΑ ΓΙΑ ΤΟΝ ΝΙΚΟ ΚΑΒΒΑΔΙΑ
   dewey: 889.21 ΑΡΓ
   entry_numbers:
   - '4693'
   editor: ΠΟΛΥΤΥΠΟ // ΑΘΗΝΑ
   edition_year: 1982
@@ -269172,15 +268992,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5328
   authors:
-  - ΑΚΡΟΠΟΛΙΤΗΣ,Σ
+  - ΑΚΡΟΠΟΛΙΤΗΣ,ΣΠΥΡΟΣ
   language: el
   title: ΜΑΡΙΑ ΡΕΝΤΗ
   dewey: 889.21 ΑΚΡ
   entry_numbers:
   - '5416'
   editor: None // ΑΘΗΝΑ
   edition_year: 1935
@@ -269220,15 +269040,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5329
   authors:
-  - ΑΝΤΩΝΟΠΟΥΛΟΣ,ΠΑΝ
+  - ΑΝΤΩΝΟΠΟΥΛΟΣ,ΠΑΝΟΣ
   language: el
   title: Ο ΓΡΑΜΜΑΤΙΚΟΣ
   dewey: 889 ΑΝΤ
   entry_numbers:
   - '5045'
   editor: None // ΑΘΗΝΑ
   edition_year: 1974
@@ -269366,15 +269186,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5332
   authors:
-  - ΑΓΓΕΛΑΤΟΥ,ΜΙΛΤ
+  - ΑΓΓΕΛΑΤΟΣ,ΜΙΛΤΙΑΔΗΣ
   language: el
   title: ΤΟ ΜΗΝΥΜΑ ΤΟΥ ΚΗΡΥΚΑ
   dewey: 889.21 ΑΓΓ
   entry_numbers:
   - '4663'
   editor: ΒΙΒΛΙΚΟΣ ΣΥΝΔΕΣΜΟΣ // ΑΘΗΝΑ
   pages: 222
@@ -269461,15 +269281,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5334
   authors:
-  - ΑΛΙΓΚΙΕΡΗ,ΔΑΝΤΟΥ
+  - ALIGHIERI,DANTE
   language: el
   title: ΘΕΙΑ ΚΩΜΩΔΙΑ
   subtitle: ΚΑΘΑΡΤΗΡΙΟΝ
   dewey: 850.11 ΑΛΙ
   entry_numbers:
   - '5423'
   translators:
@@ -269559,15 +269379,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5336
   authors:
-  - ΒΑΣΙΛΕΙΑΔΗΣ,ΝΙΚΟΣ
+  - ΒΑΣΙΛΕΙΑΔΗΣ,ΝΙΚΟΛΑΟΣ
   language: el
   title: ΓΙΑ ΤΗΝ ΕΛΕΥΘΕΡΙΑ
   dewey: 889 ΒΑΣ
   entry_numbers:
   - '4416'
   editor: Ο ΣΩΤΗΡ // ΑΘΗΝΑ
   edition_year: 1983
@@ -274259,15 +274079,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5434
   authors:
-  - WILDE
+  - WILDE,OSCAR
   language: el
   title: ΣΤΟΧΑΣΜΟΙ
   dewey: 322.33 WIL
   entry_numbers:
   - '5935'
   pages: 224
   topics:
@@ -274403,15 +274223,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5437
   authors:
-  - ΑΓΑΠΗ-ΚΑΤΣΑΡΟΥ,ΑΛΕΞΑΝΔΡΟΥ
+  - ΑΓΑΠΗΣ-ΚΑΤΣΑΡΟΣ,ΑΛΕΞΑΝΔΡΟΣ
   language: el
   title: ΜΥΡΙΣΤΙΚΑ ΧΑΜΟΚΛΑΡΑ ... ΣΑΝ ΠΟΙΗΜΑΤΑ
   dewey: 889.1 ΑΓΑ
   entry_numbers:
   - '5109'
   editor: ΗΛΙΑΔΗ // ΑΘΗΝΑ
   edition_year: 1984
@@ -274450,15 +274270,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5438
   authors:
-  - ΒΑΡΟΠΟΥΛΟΥ,ΑΛΕΞΑΝΔΡΟΥ
+  - ΒΑΡΟΠΟΥΛΟΣ,ΑΛΕΞΑΝΔΡΟΣ
   language: el
   title: ΠΡΟΣΕΓΓΙΣΕΙΣ
   dewey: 889.1 ΒΑΡ
   entry_numbers:
   - '4389'
   editor: None // ΑΓΡΙΝΙΟ
   edition_year: 1995
@@ -275073,15 +274893,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5451
   authors:
-  - ΑΡΧΙΕΠΙΣΚΟΠΟΥ ΑΥΣΤΡΑΛΙΑΣ ΣΤΥΛΙΑΝΟΥ
+  - ΣΤΥΛΙΑΝΟΣ,ΑΡΧΙΕΠΙΣΚΟΠΟΣ ΑΥΣΤΡΑΛΙΑΣ
   language: el
   title: Ο ΝΕΟΣ ΕΡΩΤΟΚΡΙΤΟΣ ΤΟΥ ΠΑΝΤΕΛΗ ΠΡΕΒΕΛΑΚΗ
   dewey: 889.1 ΣΤΥ
   entry_numbers:
   - '5110'
   editor: ΟΙ ΕΚΔΟΣΕΙΣ ΤΩΝ ΦΙΛΩ // ΑΘΗΝΑ
   edition_year: 1982
@@ -276854,15 +276674,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5487
   authors:
-  - ΑΛΕΞΑΝΔΡΟΠΟΥΛΟΣ,Μ.
+  - ΑΛΕΞΑΝΔΡΟΠΟΥΛΟΣ,ΜΗΤΣΟΣ
   language: el
   title: ΣΚΗΝΕΣ ΑΠΟ ΤΟ ΒΙΟ ΤΟΥ ΜΑΞΙΜΟΥ ΤΟΥ ΓΡΑΙΚΟΥ
   dewey: 230 ΑΛΕ
   entry_numbers:
   - '6638'
   editor: ΔΙΦΡΟΣ // ΑΘΗΝΑ
   edition_year: 1975
@@ -276998,15 +276818,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5490
   authors:
-  - ΒΙΤΑΛΗ,ΦΙΛΑΡΕΤΟΥ
+  - ΒΙΤΑΛΗΣ,ΦΙΛΑΡΕΤΟΣ
   language: el
   title: Ο ΑΠΟΣΤΟΛΟΣ ΠΑΥΛΟΣ ΚΑΙ ΟΙ ΣΥΓΧΡΟΝΟΙ ΝΕΟΙ
   dewey: 230 ΒΙΤ
   entry_numbers:
   - '6641'
   editor: None // ΠΡΕΒΕΖΑ
   edition_year: 1975
@@ -277046,15 +276866,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5491
   authors:
-  - ΒΑΣΙΛΕΙΑΔΗ,ΝΙΚΟΛΑΟΥ
+  - ΒΑΣΙΛΕΙΑΔΗΣ,ΝΙΚΟΛΑΟΣ
   language: el
   title: ΜΑΡΚΟΣ Ο ΕΥΓΕΝΙΚΟΣ ΚΑΙ Η ΕΝΩΣΙΣ ΤΩΝ ΕΚΚΛΗΣΙΩΝ
   dewey: 230 ΒΑΣ
   entry_numbers:
   - '4249'
   editor: None // ΑΘΗΝΑ
   edition_year: 1972
@@ -277094,15 +276914,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5492
   authors:
-  - ΒΕΚΙΑΡΕΛΛΗ,Β.Ε
+  - ΒΕΚΙΑΡΕΛΛΗ,Β.,Ε.
   language: el
   title: ΤΑ ΜΕΓΑΛΑ ΠΡΟΒΛΗΜΑΤΑ
   dewey: 230 ΒΕΚ
   entry_numbers:
   - '6635'
   editor: None // ΑΘΗΝΑ
   edition_year: 1938
@@ -279009,15 +278829,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5532
   authors:
-  - ΒΛΑΧΟΥ,ΠΑΝΑΓΙΩΤΟΥ
+  - ΒΛΑΧΟΥ,ΠΑΝΑΓΙΩΤΗΣ
   language: el
   title: ΣΥΝΑΞΙΣ ΕΥΓΕΝΙΟΣ Ο ΑΙΤΩΛΟΣ ΚΑΙ Η ΕΠΟΧΗ ΤΟΥ
   dewey: 230 ΒΛΑ
   entry_numbers:
   - '1724'
   editor: None // ΑΘΗΝΑ
   edition_year: 1986
@@ -279779,15 +279599,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5548
   authors:
-  - ΒΟΥΝΤ,ΒΙΛΧΕΛΜ
+  - WUNDT,WILHELM
   language: el
   title: ΜΕΤΑΦΥΣΙΚΗ
   dewey: 110 ΒΟΥ
   entry_numbers:
   - '4264'
   editor: None // ΑΘΗΝΑ
   edition_year: 1990
@@ -280580,15 +280400,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5565
   authors:
-  - ΒΑΡΝΑΛΗ,Κ.
+  - ΒΑΡΝΑΛΗΣ,ΚΩΣΤΑΣ
   language: el
   title: ΔΩΔΕΚΑ ΔΙΑΛΕΧΤΑ ΠΑΡΑΜΥΘΙΑ
   dewey: 808.899 ΒΑΡ
   entry_numbers:
   - '6674'
   editor: ΑΣΤΗΡ // ΑΘΗΝΑ
   edition_year: 1978
@@ -280675,15 +280495,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5567
   authors:
-  - ΒΛΕΣΣΑ,Γ.Σ
+  - ΒΛΕΣΣΑ,Γ.,Σ.
   language: el
   title: ΣΤΟ ΘΡΟΝΟ ΤΟΥ ΒΥΖΑΝΤΙΟΥ
   dewey: 808.899 ΒΛΕ
   entry_numbers:
   - '6676'
   editor: None // ΑΘΗΝΑ
   pages: 82
@@ -280770,15 +280590,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5569
   authors:
-  - ΑΝΤΕΡΣΕΝ,ΧΑΝΣ
+  - ANDERSEN,HANS,CHRISTIAN
   language: el
   title: ΠΑΡΑΜΥΘΙΑ ΤΟΥ ΑΝΤΕΡΣΕΝ
   dewey: 808.899 ΑΝΤ
   entry_numbers:
   - '6678'
   - '6689'
   editor: ΑΛΚΙΩΤΗΣ // ΑΘΗΝΑ
@@ -280820,15 +280640,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5570
   authors:
-  - ΒΑΡΕΛΛΑ ΑΓΓΕΛΙΚΗ
+  - ΒΑΡΕΛΛΑ,ΑΓΓΕΛΙΚΗ
   language: el
   title: ΚΟΡΙΝΘΟΣ
   subtitle: ΗΡΩΕΣ ΤΟΠΟΙ ΠΟΛΙΤΙΣΜΟΙ
   dewey: 808.899 ΒΑΡ
   entry_numbers:
   - '6874'
   editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
@@ -282190,15 +282010,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5597
   authors:
-  - ΑΓΚΑΘΑ,ΚΡΙΣΤΙ
+  - CHRISTIE,AGATHA
   language: el
   title: ΕΓΚΛΗΜΑ ΣΤΗ ΜΕΣΟΠΟΤΑΜΙΑ
   dewey: 823 ΚΡΙ
   entry_numbers:
   - '6934'
   editor: ΚΑΛΟΚΑΘΗ // ΑΘΗΝΑ
   edition_year: 1991
@@ -282548,15 +282368,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5604
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: Η ΠΛΩΤΗ ΠΟΛΙΤΕΙΑ
   dewey: 889 ΒΕΡ
   entry_numbers:
   - '6953'
   editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
   edition_year: 1989
@@ -283771,15 +283591,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5628
   authors:
-  - ΑΝΕ,ΚΛΩΝΤ
+  - ANET,CLAUDE
   language: el
   title: ΜΑΓΕΡΛΙΝΓΚ
   dewey: 889 ΑΝΕ
   entry_numbers:
   - '7265'
   translators:
   - ΚΟΝΔΥΛΗΣ,ΦΩΝΤΑΣ
@@ -284391,15 +284211,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5640
   authors:
-  - ΒΟΥΤΥΡΑ,ΔΗΜΟΣΘΕΝΗ
+  - ΒΟΥΤΥΡΑΣ,ΔΗΜΟΣΘΕΝΗΣ
   language: el
   title: ΑΡΓΟ ΞΗΜΕΡΩΜΑ
   dewey: 889.21 ΒΟΥ
   entry_numbers:
   - '7225'
   editor: Θ,ΚΟΤΣΙΩΡΗ // ΑΘΗΝΑ
   edition_year: 1950
@@ -284441,15 +284261,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5641
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  - VERNE,JULES
   language: el
   title: ΤΑ ΠΑΙΔΙΑ ΤΟΥ ΠΛΟΙΑΡΧΟΥ ΓΚΡΑΝΤ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '7226'
   editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
   edition_year: 1990
@@ -285311,15 +285131,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5658
   authors:
-  - ΒΕΝΕΖΗ,ΗΛΙΑ
+  - ΒΕΝΕΖΗΣ,ΗΛΙΑΣ
   language: el
   title: ΤΟ ΝΟΥΜΕΡΟ 31328
   dewey: 889.37 ΒΕΝ
   entry_numbers:
   - '7024'
   edition: '3'
   editor: ΑΛΦΑ // ΑΘΗΝΑ
@@ -285367,15 +285187,16 @@
 - dbase_number: 5659
   authors:
   - ΝΤΑΓΚΛΑΣ,ΛΟΥΔ
   language: el
   title: Ο ΧΙΤΩΝ
   dewey: 808.899 ΝΤΑ
   entry_numbers:
-  - 6999,6665
+  - '6999'
+  - '6665'
   translators:
   - ΛΑΜΨΑΣ,ΓΙΑΝΝΗΣ
   edition: '2'
   editor: ΔΑΜΑΣΚΟΣ // ΑΘΗΝΑ
   edition_year: 1950
   pages: 438
   topics:
@@ -285386,15 +285207,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 5659
     1: ΝΤΑΓΚΛΑΣ,ΛΟΥΔ
     2: Ο ΧΙΤΩΝ
     4: 808.899ΝΤΑ
-    5: 6999,6665
+    5: 6999-6665
     6: ΓΙΑΝΝΗ ΛΑΜΨΑ
     7: 2η
     8: ΔΑΜΑΣΚΟΣ
     9: ΑΘΗΝΑ
     10: '1950'
     11: 438Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -285929,15 +285750,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 5670
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  - VERNE,JULES
   language: el
   title: ΑΠΟ ΤΗ ΓΗ ΣΤΗ ΣΕΛΗΝΗ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '6982'
   translators:
   - ΣΦΑΕΛΛΟΥ-ΒΕΝΙΖΕΛΟΥ,ΚΑΛΛΙΩΠΗ Α.
@@ -285980,15 +285801,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5671
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  - VERNE,JULES
   language: el
   title: ΤΟ ΜΥΣΤΗΡΙΩΔΕΣ ΝΗΣΙ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '6983'
   translators:
   - ΣΦΑΕΛΛΟΥ-ΒΕΝΙΖΕΛΟΥ,ΚΑΛΛΙΩΠΗ Α.
@@ -286861,15 +286682,15 @@
   authors:
   - ΔΕΛΤΑ,Π.Σ
   language: el
   title: ΤΟΝ ΚΑΙΡΟ ΤΟΥ ΒΟΥΛΓΑΡΟΚΤΟΝΟΥ
   dewey: 808.899 ΔΕΛ
   entry_numbers:
   - '6976'
-  - 9192Α
+  - 09192
   editor: ΔΑΜΙΑΝΟΣ // ΑΘΗΝΑ
   pages: 447
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   copies: 2
   donors:
   - ΓΩΓΟΣ,
@@ -286877,15 +286698,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 5688
     1: ΔΕΛΤΑ,Π.Σ
     2: ΤΟΝ ΚΑΙΡΟ ΤΟΥ ΒΟΥΛΓΑΡΟΚΤΟΝΟΥ
     4: 808.899ΔΕΛ
-    5: 6976,9192Α
+    5: 6976-09192
     8: ΔΑΜΙΑΝΟΣ
     9: ΑΘΗΝΑ
     11: 447Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΔΩΡΕΑ ΓΩΓΟΥ
@@ -287528,15 +287349,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5701
   authors:
-  - ΑΘΑΝΑΣΙΑΔΗ,Ν.
+  - ΑΘΑΝΑΣΙΑΔΗΣ,ΝΙΚΟΣ
   language: el
   title: ΣΤΑΥΡΩΣΗ ΧΩΡΙΣ ΑΝΑΣΤΑΣΗ
   dewey: 889.21 ΑΘΑ
   entry_numbers:
   - '7244'
   editor: ΔΩΡΙΚΟΣ // ΑΘΗΝΑ
   edition_year: 1972
@@ -287835,15 +287656,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5707
   authors:
-  - WHITE,PATRIK
+  - WHITE,PATRICK
   language: el
   title: ΤΟ ΔΕΝΤΡΟ ΤΟΥ ΑΝΘΡΩΠΟΥ
   dewey: 889 WHI
   entry_numbers:
   - '7170'
   translators:
   - ΓΑΛΑΝΟΠΟΥΛΟΥ,
@@ -289472,15 +289293,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5739
   authors:
-  - ΒΟΛΤΑΙΡΟΣ
+  - VOLTAIRE
   language: el
   title: ΚΑΝΤΙΝΤ
   dewey: 889 ΒΟΛ
   entry_numbers:
   - '7192'
   editor: ΦΟΝΤΑΝΑ // ΑΘΗΝΑ
   edition_year: 1973
@@ -289929,15 +289750,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5748
   authors:
-  - ΒΕΡΚΟΡ
+  - BRULLER,JEAN,VERCORS
   language: el
   title: Η ΣΙΩΠΗ ΤΗΣ ΘΑΛΑΣΣΑΣ
   dewey: 843 ΒΕΡ
   entry_numbers:
   - '7277'
   editor: ΚΑΠΟΠΟΥΛΟΣ // ΑΘΗΝΑ
   edition_year: 1977
@@ -290079,15 +289900,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5751
   authors:
-  - ΒΕΡΣΙΓΚΟΡΑ,ΠΙΟΤΡ
+  - VERSHIGORA,PYOTR
   language: el
   title: ΑΝΘΡΩΠΟΙ ΜΕ ΚΑΘΑΡΗ ΣΥΝΕΙΔΗΣΗ
   dewey: 889 ΒΕΡ
   entry_numbers:
   - '7276'
   editor: ΚΑΠΟΠΟΥΛΟΣ // ΑΘΗΝΑ
   edition_year: 1977
@@ -290284,15 +290105,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5755
   authors:
-  - ΒΟΚΚΑΚΚΙΟ,ΤΖΟΒΑΝΝΙ
+  - BOCCACCIO,GIOVANNI
   language: el
   title: ΤΟ ΔΕΚΑΗΜΕΡΟ
   dewey: 889 ΒΟΚ
   entry_numbers:
   - '7130'
   translators:
   - ΒΑΤΑΛΑΣ,ΜΑΝΩΛΗΣ
@@ -294906,15 +294727,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 5847
   authors:
-  - ΒΑΛ,ΖΑΝ
+  - WAHL,JEAN
   language: el
   title: ΦΙΛΟΣΟΦΙΕΣ ΥΠΑΡΞΙΣΜΟΥ
   entry_numbers:
   - '7109'
   editor: ΔΩΔΩΝΗ // ΑΘΗΝΑ
   edition_year: 1970
   pages: 257
@@ -296718,15 +296539,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5883
   authors:
-  - ΒΕΡΦΕΛ,ΦΡΑΝΤΣ
+  - WERFEL,FRANZ
   language: el
   title: ΒΕΡΝΤΙ
   dewey: 780.92 ΒΕΡ
   entry_numbers:
   - '7242'
   translators:
   - ΔΡΟΣΟΣ,ΓΙΩΡΓΟΣ
@@ -297334,15 +297155,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5895
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: ΨΥΧΟΛΟΓΙΚΑ ΠΡΟΒΛΗΜΑΤΑ ΤΟΥ ΕΦΗΒΟΥ
   entry_numbers:
   - '7007'
   editor: None // ΑΘΗΝΑ
   edition_year: 1952
   pages: 132
@@ -297536,15 +297357,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5899
   authors:
-  - ΑΣΠΙΩΤΗ,ΑΡ.
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: ΣΠΟΥΔΗ ΣΥΓΧΡΟΝΟΥ ΑΝΘΡΩΠΟΛΟΓΙΑΣ
   entry_numbers:
   - '7071'
   editor: None // ΑΘΗΝΑ
   edition_year: 1955
   pages: 94
@@ -297738,15 +297559,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5903
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: Η ΓΥΝΑΙΚΑ & Ο ΨΥΧΙΚΟΣ ΤΗΣ ΚΟΣΜΟΣ
   entry_numbers:
   - '7230'
   editor: None // ΑΘΗΝΑ
   edition_year: 1953
   pages: 179
@@ -297787,15 +297608,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5904
   authors:
-  - ΑΣΠΙΩΤΗ,ΑΡ.
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: Η ΑΡΡΩΣΤΙΑ & Η ΨΥΧΗ
   entry_numbers:
   - '6921'
   editor: ΔΑΜΑΣΚΟΣ // ΑΘΗΝΑ
   edition_year: 1951
   pages: 479
@@ -297987,15 +297808,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5908
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: ΨΥΧΟΛΟΓΙΚΑ ΠΡΟΒΛΗΜΑΤΑ ΤΟΥ ΚΟΡΙΤΣΙΟΥ
   entry_numbers:
   - '7041'
   editor: None // ΑΘΗΝΑ
   edition_year: 1954
   pages: 141
@@ -298086,15 +297907,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5910
   authors:
-  - ΑΣΠΙΩΤΗΣ,ΑΡ.
+  - ΑΣΠΙΩΤΗΣ,ΑΡΙΣΤΟΣ,Α.
   language: el
   title: ΑΝΘΡΩΠΟΛΟΓΙΚΑΙ ΒΑΣΕΙΣ ΑΓΩΓΗΣ
   entry_numbers:
   - '7073'
   editor: None // ΑΘΗΝΑ
   edition_year: 1959
   pages: 140
@@ -299396,15 +299217,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5936
   authors:
-  - ΒΑΣΙΛΕΙΑΔΗ,ΝΙΚ.
+  - ΒΑΣΙΛΕΙΑΔΗΣ,ΝΙΚΟΛΑΟΣ
   language: el
   title: ΤΟ ΛΥΚΟΦΩΣ ΤΟΥ ΜΑΡΞΙΣΜΟΥ
   entry_numbers:
   - '7084'
   editor: Ο ΣΩΤΗΡ // ΑΘΗΝΑ
   edition_year: 1981
   pages: 606
@@ -299445,15 +299266,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5937
   authors:
-  - ΑΞΙΩΤΗ,ΘΕΟΔΩΡΟΥ
+  - ΑΞΙΩΤΗΣ,ΘΕΟΔΩΡΟΣ
   language: el
   title: ΑΝΑΖΗΤΩΝΤΑΣ ΤΗ ΧΑΜΕΝΗ ΚΙΒΩΤΟ
   dewey: 889.21 ΑΞΙ
   entry_numbers:
   - '7058'
   editor: ΣΜΥΡΝΙΩΤΑΚΗΣ // ΑΘΗΝΑ
   pages: 247
@@ -300782,15 +300603,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5964
   authors:
-  - ΒΑΣΙΛΕΙΑΔΗ,ΝΙΚΟΛΑΟΥ
+  - ΒΑΣΙΛΕΙΑΔΗΣ,ΝΙΚΟΛΑΟΣ
   language: el
   title: ΧΡΙΣΤΙΑΝΙΣΜΟΣ ΚΑΙ ΑΝΘΡΩΠΙΣΜΟΣ
   dewey: 230 ΒΑΣ
   entry_numbers:
   - '7234'
   editor: ΣΩΤΗΡ // ΑΘΗΝΑ
   edition_year: 1981
@@ -301673,15 +301494,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5982
   authors:
-  - ΑΞΙΩΤΗ,ΘΕΟΔΩΡΟΥ
+  - ΑΞΙΩΤΗΣ,ΘΕΟΔΩΡΟΣ
   language: el
   title: Η ΑΠΟΚΡΥΠΤΟΓΡΑΦΗΣΗ ΤΟΥ ΔΙΣΚΟΥ ΤΗΣ ΦΑΙΣΤΟΥ ΓΕΝΕΣΗ
   dewey: 938.113 ΑΞΙ
   entry_numbers:
   - '6949'
   editor: ΣΜΥΡΝΙΩΤΑΚΗΣ // None
   pages: 496
@@ -301819,15 +301640,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5985
   authors:
-  - ΑΝΔΡΟΝΙΚΟΣ
+  - ΑΝΔΡΟΝΙΚΟΣ,ΜΑΝΩΛΗΣ
   language: el
   title: Ο ΠΛΑΤΩΝ ΚΑΙ Η ΤΕΧΝΗ
   entry_numbers:
   - '6919'
   editor: ΝΕΦΕΛΗ // ΑΘΗΝΑ
   edition_year: 1984
   pages: 286
@@ -302268,15 +302089,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 5994
   authors:
-  - ΒΑΛΑΩΡΙΤΗΣ,Α.
+  - ΒΑΛΑΩΡΙΤΗΣ,ΑΡΙΣΤΟΤΕΛΗΣ
   language: el
   title: ΑΠΑΝΤΑ
   entry_numbers:
   - '7241'
   editor: ΔΕΛΗ ΧΡΥΣΟ // None
   pages: 736
   topics:
@@ -308405,15 +308226,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6116
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: ΤΑΞΙΔΙ ΣΤΟΝ ΑΜΑΖΟΝΙΟ
   entry_numbers:
   - '7371'
   translators:
   - ΔΕΛΗΓΙΑΝΝΗ,ΓΕΩΡΓΙΑ
   editor: ΜΙΝΩΑΣ // ΑΘΗΝΑ
@@ -310676,15 +310497,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6161
   authors:
-  - ΒΕΤΣΙΟΣ,Ε.Λ
+  - ΒΕΤΣΙΟΣ,ΕΛΕΥΘΕΡΙΟΣ,Λ.
   language: el
   title: ΓΕΩΡΓΙΟΣ ΚΟΥΜΑΝΟΣ Ο ΠΡΩΤΟΣ ΒΕΝΕΤΟΣ ΠΡΟΞΕΝΟΣ ΣΤΗΝ ΑΡΤΑ ΤΟ
   subtitle: 1720 ΔΙΚΑΙΟΔΟΣΙΑ - ΚΑΘΗΚΟΝΤΑ (ΜΕ ΒΑΣΗ ΤΑ ΒΕΝΕΤΙΚΑ ΑΡΧΕΙΑ)
   dewey: 938.462 ΒΕΤ
   entry_numbers:
   - '8025'
   editor: None // ΑΡΤΑ
@@ -311232,15 +311053,15 @@
   authors:
   - ΣΚΟΥΤΕΛΑ,ΠΕΤΡΟΥ
   language: el
   title: ΤΟΥ ΧΩΡΙΟΥ ΚΑΙ ΤΗΣ ΠΟΛΗΣ
   dewey: 398 ΣΚΟ
   entry_numbers:
   - '8045'
-  - 9146Α
+  - 09146
   editor: None // ΑΘΗΝΑ
   edition_year: 2002
   pages: 142
   topics:
   - ΛΑΟΓΡΑΦΙΑ
   - ΒΙΩΜΑΤΑ
   - ΛΑΟΓΡΑΦΙΚΑ ΣΤΟΙΧΕΙΑ
@@ -311249,15 +311070,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 6172
     1: ΣΚΟΥΤΕΛΑ,ΠΕΤΡΟΥ
     2: ΤΟΥ ΧΩΡΙΟΥ ΚΑΙ ΤΗΣ ΠΟΛΗΣ
     4: 398ΣΚΟ
-    5: 8045-9146Α
+    5: 8045-09146
     9: ΑΘΗΝΑ
     10: '2002'
     11: 142Σ
     12: ΛΑΟΓΡΑΦΙΑ-ΒΙΩΜΑΤΑ
     13: ΛΑΟΓΡΑΦΙΚΑ ΣΤΟΙΧΕΙΑ
     14: ΒΙΩΜΑΤΑ-ΛΑΟΓΡΑΦΙΑ
     17: 6 ΑΝΤΙΤΥΠΑ
@@ -311672,15 +311493,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6181
   authors:
-  - ΑΛΕΞΑΚΗΣ,ΕΛΕΥΘ.
+  - ΑΛΕΞΑΚΗΣ,ΕΛΕΥΘΕΡΙΟΣ
   language: el
   title: Η ΣΗΜΑΙΑ ΣΤΟ ΓΑΜΟ
   entry_numbers:
   - '8064'
   editor: None // ΑΘΗΝΑ
   edition_year: 1990
   pages: 77
@@ -311820,15 +311641,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6184
   authors:
-  - ΑΘΑΝΑΣΑΚΗ,ΑΝΤΩΝΙΟΥ ΝΙΚΟΛΑΟΥ
+  - ΑΘΑΝΑΣΑΚΗΣ,ΑΝΤΩΝΗΣ,ΝΙΚΟΛΑΟΥ
   language: el
   title: ΠΑΡΟΙΜΙΕΣ ΚΑΙ ΦΡΑΣΕΙΣ ΤΟΥ ΤΟΠΟΥ ΜΑΣ
   dewey: 398 ΑΘΑ
   entry_numbers:
   - '5081'
   editor: None // ΑΘΗΝΑ
   edition_year: 1998
@@ -318636,15 +318457,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6323
   authors:
-  - ΑΛΕΞΙΑΔΗ,ΣΤΕΡΓΙΟΥ
+  - ΑΛΕΞΙΑΔΗΣ,ΣΤΕΡΓΙΟΣ
   language: el
   title: ΣΩΦΡΟΝΙΣΤΙΚΗ
   entry_numbers:
   - '8224'
   editor: ΣΑΚΚΟΥΛΑ // ΑΘΗΝΑ
   edition_year: 2001
   pages: 413
@@ -318875,15 +318696,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6328
   authors:
-  - ΑΠΑΛΑΓΑΚΗ,ΧΑΡ.
+  - ΑΠΑΛΑΓΑΚΗ,ΧΑΡΙΚΛΕΙΑ
   language: el
   title: ΔΕΔΙΚΑΣΜΕΝΟ ΚΑΙ ΕΚΤΕΛΕΣΤΟΤΗΤΑ ΣΤΑ ΝΟΜΙΚΑ ΠΡΟΣΩΠΑ ΚΑΙ ΣΤΑ ΜΕΛ
   entry_numbers:
   - '8229'
   editor: ΣΑΚΚΟΥΛΑ // ΑΘΗΝΑ
   edition_year: 2001
   pages: 367
@@ -321408,15 +321229,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6379
   authors:
-  - ΒΟΥΛΓΑΡΗ,ΜΕΛ.
+  - ΒΟΥΛΓΑΡΗΣ,ΜΕΛΕΤΙΟΣ
   language: el
   title: ΜΗΧΑΝΟΛΟΓΙΚΟ ΣΧΕΔΙΟ
   entry_numbers:
   - '8280'
   editor: ΙΩΝ // ΑΘΗΝΑ
   edition_year: 1991
   pages: 284
@@ -322107,15 +321928,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6393
   authors:
-  - ΒΑΣΙΛΙΚΟΥ,ΝΤΟΡΑΣ
+  - ΒΑΣΙΛΙΚΟΥ,ΝΤΟΡΑ
   language: el
   title: ΜΥΚΗΝΑΙΚΑ ΣΦΡΑΓΙΣΤΙΚΑ ΔΑΧΤΥΛΙΔΙΑ
   entry_numbers:
   - '8294'
   editor: None // ΑΘΗΝΑ
   edition_year: 1997
   pages: 72
@@ -325552,15 +325373,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 6463
   authors:
-  - ΑΡΑΒΑΝΤΙΝΟΥ,ΣΠ
+  - ΑΡΑΒΑΝΤΙΝΟΣ,ΣΠΥΡΙΔΩΝ,Π.
   language: el
   title: ΙΣΤΟΡΙΑ ΤΟΥ ΑΛΗ ΠΑΣΑ ΤΟΥ ΤΕΠΕΛΕΝΗ
   dewey: 938.21 ΑΡΑ
   entry_numbers:
   - '8375'
   editor: ΠΥΡΡΟΣ // ΑΘΗΝΑ
   edition_year: 1895
@@ -325749,15 +325570,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6467
   authors:
-  - ΒΥΛΕΡΜΟΖ,ΕΜΙΛ
+  - VUILLERMOZ,EMILE
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΜΟΥΣΙΚΗΣ
   dewey: 780.9 ΒΥΛ
   entry_numbers:
   - '8371'
   editor: ΥΠΟΔΟΜΗ // ΑΘΗΝΑ
   edition_year: 1980
@@ -327779,15 +327600,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6509
   authors:
-  - ΑΝΤΟΩΝΟΠΟΥΛΟΥ,ΚΟΣΜΑ
+  - ΑΝΤΩΝΟΠΟΥΛΟΣ,ΚΟΣΜΑΣ
   language: el
   title: Η ΕΛΛΗΝΙΚΗ ΠΑΙΔΕΙΑ ΚΑΙ Η ΝΕΑ ΓΕΝΙΑ
   entry_numbers:
   - '8533'
   editor: None // ΚΥΠΑΡΙΣΣΙΑ
   edition_year: 1991
   pages: 350
@@ -328255,15 +328076,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6519
   authors:
-  - ΒΑΣΙΛΕΙΑΔΗ,ΝΙΚΟΛΑΟΥ
+  - ΒΑΣΙΛΕΙΑΔΗΣ,ΝΙΚΟΛΑΟΣ
   language: el
   title: Η ΕΛΛΑΣ ΣΤΗΝ ΕΝΩΜΕΝΗ ΕΥΡΩΠΗ
   entry_numbers: []
   editor: Ο ΣΩΤΗΡ // ΑΘΗΝΑ
   edition_year: 1991
   pages: 64
   topics:
@@ -331206,30 +331027,30 @@
   authors:
   - ΤΟΥΡΑΤΣΟΓΛΟΥ,ΙΩΑΝΝΗΣ
   language: el
   title: ΜΑΚΕΔΟΝΙΑ
   subtitle: ΙΣΤΟΡΙΑ ΜΝΗΜΕΙΑ ΜΟΥΣΕΙΑ
   dewey: 938.666 ΤΟΥ
   entry_numbers:
-  - 9298Α
+  - 09298
   editor: ΕΚΔΟΤΙΚΗ ΑΘΗΝΩΝ // ΑΘΗΝΑ
   edition_year: 1996
   pages: 459
   topics:
   - ΜΑΚΕΔΟΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 6579
     1: ΤΟΥΡΑΤΣΟΓΛΟΥ,ΙΩΑΝΝΗΣ
     2: ΜΑΚΕΔΟΝΙΑ
     3: ΙΣΤΟΡΙΑ ΜΝΗΜΕΙΑ ΜΟΥΣΕΙΑ
     4: 938.666ΤΟΥ
-    5: 9298Α
+    5: 09298
     8: ΕΚΔΟΤΙΚΗ ΑΘΗΝΩΝ
     9: ΑΘΗΝΑ
     10: '1996'
     11: 459Σ
     12: ΜΑΚΕΔΟΝΙΑ
     13: ΜΑΚΕΔΟΝΙΑ
     14: ΜΑΚΕΔΟΝΙΑ
@@ -331258,34 +331079,36 @@
   title: Η ΑΓΑΠΗ ΠΟΥ ΑΝΘΙΣΕ ΣΤΗΣ ΚΑΤΟΧΗΣ ΤΑ ΧΡΟΝΙΑ
   dewey: 889.21 ΑΘΑ
   entry_numbers:
   - '8643'
   editor: None // ΑΘΗΝΑ
   edition_year: 2003
   pages: 172
-  topics: []
+  topics:
+  - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  - ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 6580
     1: ΑΘΑΝΑΣΙΟΥ,ΘΕΟΦΙΛΟΣ
     2: Η ΑΓΑΠΗ ΠΟΥ ΑΝΘΙΣΕ ΣΤΗΣ ΚΑΤΟΧΗΣ ΤΑ ΧΡΟΝΙΑ
     4: 889.21ΑΘΑ
     5: '8643'
     9: ΑΘΗΝΑ
     10: '2003'
     11: 172Σ
+    12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΛΟΓΟΤΕΧΝΙΑ
+    14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     3: null
     6: null
     7: null
     8: null
-    12: null
-    13: null
-    14: null
     15: null
     16: null
     17: null
     18: null
     19: null
     20: null
     21: null
@@ -332107,15 +331930,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6598
   authors:
-  - ΒΑΣΙΛΕΙΟΥ, ΣΩΚΡΑΤΗΣ
+  - ΒΑΣΙΛΕΙΟΥ,ΣΩΚΡΑΤΗΣ
   language: el
   title: ΚΑΓΚΕΛΑΡΗΣ ΠΑΠΑΔΑΤΩΝ ⁿΛΑΚΚΑ ΣΟΥΛΙⁿ
   dewey: 398 ΒΑΣ
   entry_numbers:
   - '8651'
   editor: None // ΑΘΗΝΑ
   edition_year: 2003
@@ -332671,15 +332494,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6610
   authors:
-  - ΒΑΣΙΛΕΙΑΔΗ.ΝΙΚΟΛΑΟΥ
+  - ΒΑΣΙΛΕΙΑΔΗΣ,ΝΙΚΟΛΑΟΣ
   language: el
   title: Η ΕΛΛΑΣ ΣΤΗΝ ΕΝΩΜΕΝΗ ΕΥΡΩΠΗ
   entry_numbers:
   - '8667'
   editor: Ο ΣΩΤΗΡ // ΑΘΗΝΑ
   edition_year: 1991
   pages: 60
@@ -333607,15 +333430,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6629
   authors:
-  - ΑΝΤΟΝΙΟ ΛΟΜΠΟ ΑΝΤΟΥΝΕΣ
+  - ANTUNES,ANTONIO,LOBO
   language: el
   title: ΤΟ ΕΓΧΕΙΡΙΔΙΟ ΤΩΝ ΙΕΡΟΕΞΕΤΑΣΤΩΝ
   dewey: 869 ΑΝΤ
   entry_numbers:
   - '8691'
   - '9854'
   translators:
@@ -334216,15 +334039,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6641
   authors:
-  - ΑΠΝΤΑΙΚ, ΤΖΩΝ
+  - UPDIKE,JOHN
   language: el
   title: ΓΕΡΤΡΟΥΔΗ ΚΑΙ ΚΛΑΥΔΙΟΣ
   dewey: 823 ΑΠΝ
   entry_numbers:
   - '8703'
   translators:
   - ΣΤΕΦΑΝΑΚΗΣ,ΔΗΜΗΤΡΗΣ
@@ -336479,15 +336302,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6687
   authors:
-  - ΑΝΑΣΗ,ΕΜΜ.
+  - ΑΝΑΣΗΣ,ΕΜΜΑΝΟΥΗΛ
   language: el
   title: ΓΕΝΙΚΗ ΠΤΗΝΟΤΡΟΦΙΑ
   dewey: 598 ΑΝΑ
   entry_numbers:
   - '8792'
   editor: ΚΑΜΠΑΝΑ // ΑΘΗΝΑ
   pages: 222
@@ -336671,15 +336494,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6691
   authors:
-  - ΑΝΑΣΗ,ΕΜΜ
+  - ΑΝΑΣΗΣ,ΕΜΜΑΝΟΥΗΛ
   language: el
   title: Ο ΚΗΠΟΣ ΤΗΣ ΟΙΚΟΓΕΝΕΙΑΣ
   dewey: 634 ΑΝΑ
   entry_numbers:
   - '8796'
   editor: ΚΑΜΠΑΝΑ // ΑΘΗΝΑ
   pages: 388
@@ -338521,15 +338344,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6728
   authors:
-  - ΒΙΚΕΛΑ,ΔΗΜΗΤΡΙΟΥ
+  - ΒΙΚΕΛΑΣ,ΔΗΜΗΤΡΙΟΣ
   language: el
   title: ΛΟΥΚΗΣ ΛΑΡΑΣ
   dewey: 889.21 ΒΙΚ
   entry_numbers:
   - '8805'
   editor: ΣΜΥΡΝΙΩΤΑΚΗΣ // ΑΘΗΝΑ
   pages: 198
@@ -339398,15 +339221,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6746
   authors:
-  - ΒΑΛΜΑ,ΣΤΑΜΑΤΗ
+  - ΒΑΛΜΑΣ,ΣΤΑΜΑΤΗΣ
   language: el
   title: ΣΤΟΥ ΕΞΑΝΘΡΩΠΙΣΜΟΥ ΤΟ ΜΟΝΟΠΑΤΙ
   subtitle: ΤΟΥ ΚΟΣΜΟΥ Η ΕΛΠΙΔΑ
   dewey: 578.7 ΒΑΛ
   entry_numbers:
   - '8867'
   pages: 310
@@ -339446,15 +339269,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6747
   authors:
-  - ΒΑΛΜΑ,ΣΤΑΜΑΤΗ
+  - ΒΑΛΜΑΣ,ΣΤΑΜΑΤΗΣ
   language: el
   title: ΣΤΟΥ ΕΞΑΝΘΡΩΠΙΣΜΟΥ ΤΟ ΜΟΝΟΠΑΤΙ
   subtitle: ΙΑΤΡΟΙ-ΦΥΣΙΚΟΘΕΡΑΠΕΥΤΕΣ-ΠΡΑΚΤΙΚΟΙ
   dewey: 578.7 ΒΑΛ
   entry_numbers:
   - '8865'
   pages: 356
@@ -339494,15 +339317,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6748
   authors:
-  - ΒΑΛΜΑ,ΣΤΑΜΑΤΗ
+  - ΒΑΛΜΑΣ,ΣΤΑΜΑΤΗΣ
   language: el
   title: ΣΤΟΥ ΕΞΑΝΘΡΩΠΙΣΜΟΥ ΤΟ ΜΟΝΟΠΑΤΙ
   subtitle: ΤΑ ΑΝΕΠΑΝΑΛΗΠΤΑ ΦΑΡΜΑΚΑ ΤΗΣ ΖΩΗΣ
   dewey: 578.7 ΒΑΛ
   entry_numbers:
   - '8866'
   pages: 152
@@ -339542,15 +339365,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6749
   authors:
-  - ΒΑΛΜΑ,ΣΤΑΜΑΤΗ
+  - ΒΑΛΜΑΣ,ΣΤΑΜΑΤΗΣ
   language: el
   title: ΣΤΟΥ ΕΞΑΝΘΡΩΠΙΣΜΟΥ ΤΟ ΜΟΝΟΠΑΤΙ
   dewey: 578 ΒΑΛ
   entry_numbers:
   - '8869'
   pages: 221
   topics:
@@ -339588,15 +339411,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6750
   authors:
-  - ΒΑΛΜΑ,ΣΤΑΜΑΤΗ
+  - ΒΑΛΜΑΣ,ΣΤΑΜΑΤΗΣ
   language: el
   title: ΣΤΟΥ ΕΞΑΝΘΡΩΠΙΣΜΟΥ ΤΟ ΜΟΝΟΠΑΤΙ
   dewey: 578.7 ΒΑΛ
   entry_numbers:
   - '8870'
   pages: 160
   topics:
@@ -339634,15 +339457,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6751
   authors:
-  - ΒΑΛΜΑ,ΣΤΑΜΑΤΗ
+  - ΒΑΛΜΑΣ,ΣΤΑΜΑΤΗΣ
   language: el
   title: ΕΣΩΤΕΡΙΚΟ ΤΑΞΙΔΙ
   subtitle: ΠΩΣ ΑΝΘΙΖΕΙ ΤΗΣ ΨΥΧΟ-ΣΩΜΑΤΙΚΗΣ ΥΓΕΑΣ ΤΟ ΛΟΥΛΟΥΔΙ
   dewey: 578.7 ΒΑΛ
   entry_numbers:
   - '8868'
   pages: 320
@@ -339682,15 +339505,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6752
   authors:
-  - ΒΕΤΣΙΟΣ,ΕΛΕΥΘΕΡΙΟΣ
+  - ΒΕΤΣΙΟΣ,ΕΛΕΥΘΕΡΙΟΣ,Λ.
   language: el
   title: Η ΔΙΠΛΩΜΑΤΙΚΗ ΚΑΙ ΟΙΚΟΝΟΜΙΚΗ ΠΑΡΟΥΣΙΑ ΤΩΝ ΒΕΝΕΤΩΝ ΣΤΗΝ
   subtitle: ΠΕΡΙΟΧΗ ΤΗΣ ΑΡΤΑΣ ΚΑΤΑ ΤΟΝ 18Ο ΑΙΩΝΑ
   dewey: 938.462 ΒΕΤ
   entry_numbers:
   - '8964'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -341941,15 +341764,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6798
   authors:
-  - ΑΝΑΓΝΩΣΤΟΠΟΥΛΟΥ,ΣΤΕΦΑΝΟΥ
+  - ΑΝΑΓΝΩΣΤΟΠΟΥΛΟΣ,ΣΤΕΦΑΝΟΣ
   language: el
   title: ΑΝΑΣΑΣΜΟΙ ΣΩΤΗΡΙΑΣ
   dewey: 230 ΑΝΑ
   entry_numbers:
   - '8899'
   editor: None // ΠΕΙΡΑΙΑΣ
   edition_year: 1998
@@ -342469,15 +342292,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6809
   authors:
-  - ΑΝΤΟΥΡΑΚΗ,ΓΕΩΡΓΙΟΥ
+  - ΑΝΤΟΥΡΑΚΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΧΡΙΣΤΙΑΝΙΚΗ ΑΡΧΑΙΟΛΟΓΙΑ
   subtitle: ΣΤΟΙΧΕΙΑ ΑΠΟ ΤΗΝ ΤΕΧΝΗ ΑΝΑΤΟΛΗΣ ΚΑΙ ΔΥΣΕΩΣ
   dewey: 230 ΑΝΤ
   entry_numbers:
   - '8950'
   editor: None // ΑΘΗΝΑ
@@ -344997,15 +344820,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6860
   authors:
-  - ΑΛΕΞΑΚΗΣ,ΕΛΕΥΘ.
+  - ΑΛΕΞΑΚΗΣ,ΕΛΕΥΘΕΡΙΟΣ
   language: el
   title: Η ΣΗΜΑΙΑ ΣΤΟ ΓΑΜΟ
   subtitle: ΤΕΛΕΤΟΥΡΓΙΑ-ΕΞΑΠΛΩΣΗ-ΠΡΟΕΛΕΥΣΗ
   dewey: 398 ΑΛΕ
   entry_numbers:
   - '8064'
   editor: None // ΑΘΗΝΑ
@@ -346173,15 +345996,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6884
   authors:
-  - ΑΡΓΥΡΗ,ΑΝΔΡΕΑ
+  - ΑΡΓΥΡΗΣ,ΑΝΔΡΕΑΣ
   language: el
   title: Ο ΣΑΜΠΟΤΕΡ ΦΑΝΤΑΣΜΑ ΤΟΥ ΔΕΥΤΕΡΟΥ ΠΑΓΚΟΣΜΙΟΥ ΠΟΛΕΜΟΥ
   dewey: 938.75 ΑΡΓ
   entry_numbers:
   - '5362'
   editor: None // ΑΘΗΝΑ
   edition_year: 1987
@@ -347491,15 +347314,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6911
   authors:
-  - ΑΝΤΩΝΙΑΔΗ,Γ.-ΤΑΝΙΜΑΝΙΔΗ Π.Γ.
+  - ΑΝΤΩΝΙΑΔΗΣ,ΓΕΩΡΓΙΟΣ.
+  - ΤΑΝΙΜΑΝΙΔΗΣ,ΠΑΝΑΓΙΩΤΗΣ,Γ.
   language: el
   title: ΤΟ ΑΝΤΑΡΤΙΚΟ ΣΤΟΝ ΠΟΝΤΟ
   dewey: 938.71 ΑΝΤ
   entry_numbers:
   - '5346'
   - '16965'
   editor: ΠΑΝΑΓΙΑ ΣΟΥΜΕΛΑ // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -349072,15 +348896,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6943
   authors:
-  - ΑΔΑΜΑΚΟΠΟΥΛΟΣ,ΤΡΙΑΝΤΑΦΥΛΛΟΣ,ΜΑΤΣΟΥΚΑ ΠΗΝ
+  - ΑΔΑΜΑΚΟΠΟΥΛΟΣ,ΤΡΙΑΝΤΑΦΥΛΛΟΣ
+  - ΜΑΤΣΟΥΚΑ,ΠΗΝΕΛΟΠΗ
   language: el
   title: ΠΙΝΔΟΣ-ΓΡΕΒΕΝΑ
   dewey: 938.95 ΑΔΑ
   entry_numbers:
   - '8996'
   editor: ΤΕΔΚ ΓΡΕΒΕΝΩΝ // ΓΡΕΒΕΝΑ
   edition_year: 1998
@@ -349773,15 +349598,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6957
   authors:
-  - ΑΛΙΠΡΑΝΤΗΣ,ΝΙΚΟΣ
+  - ΑΛΙΠΡΑΝΤΗΣ,ΝΙΚΟΣ,ΧΡ.
   language: el
   title: ΠΡΟΟΔΕΥΤΙΚΟΣ ΣΥΛΛΟΓΟΣ ΛΕΥΚΙΑΝΩΝ ΠΑΡΟΥ
   subtitle: Η ΙΣΤΟΡΙΑ ΤΩΝ ΕΒΔΟΜΗΝΤΑ ΧΡΟΝΩΝ ΤΟΥ 1925-1995
   dewey: 398 ΑΛΙ
   entry_numbers:
   - '4297'
   editor: None // ΑΘΗΝΑ
@@ -350304,15 +350129,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6968
   authors:
-  - ΑΘΑΝΑΣΙΑΔΗΣ, ΤΙΤΟΣ
+  - ΑΘΑΝΑΣΙΑΔΗΣ,ΤΙΤΟΣ
   language: el
   title: ΟΙ ΠΑΤΡΙΑΡΧΕΣ ΒΥΖΑΝΤΙΟΥ ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΕΩΣ
   entry_numbers:
   - '9009'
   editor: ΑΠΟΓΕΥΜΑΤΙΝΗ // ΑΘΗΝΑ
   edition_year: 2003
   pages: 304
@@ -351362,22 +351187,22 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6989
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: Ο ΓΥΡΟΣ ΤΟΥ ΚΟΣΜΟΥ ΣΕ 80 ΜΕΡΕΣ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '9018'
   - '9091'
-  - 9169Α
+  - 09169
   editor: ΑΛΚΥΩΝ,ΠΑΠΑΔΟΠΟΥΛΟΣ // ΑΘΗΝΑ
   edition_year: 2004
   pages: 271
   topics:
   - ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΜΥΘΙΣΤΟΡΗΜΑ
   copies: 3
@@ -351386,15 +351211,15 @@
   offprint: false
   isbn: '9603261009'
   original_entry:
     0: 6989
     1: ΒΕΡΝ,ΙΟΥΛΙΟΣ
     2: Ο ΓΥΡΟΣ ΤΟΥ ΚΟΣΜΟΥ ΣΕ 80 ΜΕΡΕΣ
     4: 808.899ΒΕΡ
-    5: 9018,9091,9169Α
+    5: 9018-9091-09169
     8: ΑΛΚΥΩΝ,ΠΑΠΑΔΟΠΟΥΛΟΣ
     9: ΑΘΗΝΑ
     10: '2004'
     11: 271Σ
     12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΜΥΘΙΣΤΟΡΗΜΑ
@@ -351655,15 +351480,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 6995
   authors:
-  - ΑΠΕΡΓΗΣ,ΠΑΝΤΕΛΗΣ-ΚΟΥΔΟΥΝΗΣ,ΘΑΝΑΣΗΣ
+  - ΑΠΕΡΓΗΣ,ΠΑΝΤΕΛΗΣ
+  - ΚΟΥΔΟΥΝΗΣ,ΘΑΝΑΣΗΣ
   language: el
   title: ΤΟ ΠΟΙΗΤΙΚΟ ΕΡΓΟ ΤΟΥ ΒΑΣΙΛΗ ΚΟΥΡΗ
   subtitle: ΜΕΛΕΤΕΣ-ΚΡΙΤΙΚΕΣ
   dewey: 889.09 ΑΠΕ
   entry_numbers:
   - '9027'
   editor: ΙΩΛΚΟΣ // ΑΘΗΝΑ
@@ -352157,15 +351983,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7005
   authors:
-  - ΒΑΣΙΛΕΙΟΥ,Σ. ΣΩΚΡΑΤΗ
+  - ΒΑΣΙΛΕΙΟΥ,ΣΩΚΡΑΤΗΣ,Σ.
   language: el
   title: ΓΥΝΑΙΚΕΣ ΗΠΕΙΡΩΤΙΣΣΕΣ
   subtitle: ΞΑΦΝΙΑΣΜΑ ΤΗΣ ΦΥΣΗΣ
   dewey: 398 ΒΑΣ
   entry_numbers:
   - '9045'
   - '9290'
@@ -352263,15 +352089,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7007
   authors:
-  - ΒΕΝΕΤΗΣ,Π
+  - ΒΕΝΕΤΗΣ,ΠΕΤΡΟΣ
   language: el
   title: ΑΦΟΥ ΜΕΓΑΛΩΣΕΣ...ΚΑΛΑ ΝΑ ΠΑΘΕΙΣ!
   dewey: 889.21 ΒΕΝ
   entry_numbers:
   - '9060'
   editor: ΜΟΝΤΕΡΝΟΙ ΚΑΙΡΟΙ // ΑΘΗΝΑ
   edition_year: 1996
@@ -353305,15 +353131,15 @@
   authors:
   - ΣΤΟΟΥ ΜΠΙΤΣΕΡ
   language: el
   title: Η ΚΑΛΥΒΑ ΤΟΥ ΜΠΑΡΜΠΑ ΘΩΜΑ
   dewey: 808.899 ΣΤΟ
   entry_numbers:
   - '9093'
-  - 9173Α
+  - 09173
   - '20640'
   translators:
   - ΠΑΠΠΑ,ΜΑΡΙΑ
   editor: ΠΑΠΑΔΟΠΟΛΥΛΟΣ // ΑΘΗΝΑ
   edition_year: 2001
   pages: 143
   topics:
@@ -353324,15 +353150,15 @@
   offprint: false
   isbn: 960-412-017-4
   original_entry:
     0: 7028
     1: ΣΤΟΟΥ ΜΠΙΤΣΕΡ
     2: Η ΚΑΛΥΒΑ ΤΟΥ ΜΠΑΡΜΠΑ ΘΩΜΑ
     4: 808.899ΣΤΟ
-    5: 9093-9173Α-20640
+    5: 9093-09173-20640
     6: ΜΑΡΙΑ ΠΑΠΠΑ
     8: ΠΑΠΑΔΟΠΟΛΥΛΟΣ
     9: ΑΘΗΝΑ
     10: '2001'
     11: 143Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -353703,15 +353529,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7036
   authors:
-  - ΑΝΔΡΟΤΣΟΠΟΥΛΟΥ-ΠΕΤΡΟΒΙΤΣ,ΛΟΤΗ
+  - ΑΝΔΡΟΥΤΣΟΠΟΥΛΟΥ-ΠΕΤΡΟΒΙΤΣ,ΛΟΤΗ
   language: el
   title: ΙΣΤΟΡΙΕΣ ΓΙΑ ΠΑΙΧΝΙΔΙ ΚΑΙ ΓΕΛΙΑ
   dewey: 889.09 ΑΝΔ
   entry_numbers:
   - '9088'
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2006
@@ -353751,15 +353577,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7037
   authors:
-  - ΑΝΤΟΥΑΝ ΝΤΕ ΣΑΙΝ ΕΞΥΠΕΡΥ
+  - DE SAINT-EXUPERY, ANTOINE
   language: el
   title: Ο ΜΙΚΡΟΣ ΠΡΙΓΚΙΠΑΣ
   dewey: 889.09 ΕΞΥ
   entry_numbers:
   - '9096'
   translators:
   - ΚΑΡΑΚΩΣΤΑ,ΜΕΛΙΝΑ
@@ -354695,15 +354521,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7056
   authors:
-  - ΒΕΤΣΙΟΣ,ΕΛΕΥΘΕΡΙΟΣ
+  - ΒΕΤΣΙΟΣ,ΕΛΕΥΘΕΡΙΟΣ,Λ.
   language: el
   title: Η ΔΙΠΛΩΜΑΤΙΚΗ ΚΑΙ ΟΙΚΟΝΟΜΙΚΗ ΠΑΡΟΥΣΙΑ ΤΩΝ ΒΕΝΕΤΩΝ ΣΤΗΝ ΠΕΡΙΟ
   subtitle: ΧΗ ΤΗΣ ΑΡΤΑΣ ΚΑΤΑ ΤΟΝ 18Ο ΑΙΩΝΑ
   entry_numbers:
   - '9123'
   editor: ΑΝΤ. ΣΤΑΜΟΥΛΗΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
@@ -355595,15 +355421,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7074
   authors:
-  - ΒΕΡΤΟΔΟΥΛΟΥ,ΑΠΟΣΤΟΛΟΥ
+  - ΒΕΡΤΟΔΟΥΛΟΥ,ΑΠΟΣΤΟΛΟΣ
   language: el
   title: ΗΠΕΙΡΟΣ ΠΟΛΙΤΙΣΤΙΚΗ ΚΛΗΡΟΝΟΜΙΑ ΚΑΙ ΦΥΣΗ
   dewey: 938.939 ΒΕΡ
   entry_numbers:
   - '9144'
   editor: ΔΩΔΩΝΗ // ΙΩΑΝΝΙΝΑ
   edition_year: 1995
@@ -356186,15 +356012,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7086
   authors:
-  - ΒΛΑΧΟΠΑΝΟΣ, ΔΗΜΗΤΡΗΣ
+  - ΒΛΑΧΟΠΑΝΟΣ,ΔΗΜΗΤΡΗΣ
   language: el
   title: ΑΙ ΚΟΜΜΕΝΟ ΤΗΣ ΑΣΒΕΣΤΗΣ ΜΝΗΜΗΣ
   dewey: 889.21 ΒΛΑ
   entry_numbers:
   - '9156'
   editor: ΕΝΤΥΠΩΣΙΣ // ΑΡΤΑ
   edition_year: 2007
@@ -356388,20 +356214,20 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7090
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: ΜΙΧΑΗΛ ΣΤΡΟΓΚΟΦ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
-  - 9171Α
+  - 09171
   - '19992'
   translators:
   - ΦΕΡΤΑΚΗ,ΑΝΝΙΚΑ
   editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
   edition_year: 2008
   pages: 323
   topics:
@@ -356411,15 +356237,15 @@
   offprint: false
   ean: 978-960-422-271-1
   original_entry:
     0: 7090
     1: ΒΕΡΝ,ΙΟΥΛΙΟΣ
     2: ΜΙΧΑΗΛ ΣΤΡΟΓΚΟΦ
     4: 808.899ΒΕΡ
-    5: 9171Α,19992
+    5: 09171-19992
     6: ΑΝΝΙΚΑ ΦΕΡΤΑΚΗ
     8: ΑΓΚΥΡΑ
     9: ΑΘΗΝΑ
     10: '2008'
     11: 323Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -356497,15 +356323,15 @@
 - dbase_number: 7092
   authors:
   - ΤΟΥΕΙΝ,ΜΑΡΚ
   language: el
   title: ΠΡΙΓΚΙΠΑΣ ΚΑΙ ΦΤΩΧΟΣ
   dewey: 808.899 TOY
   entry_numbers:
-  - 9195Α
+  - 09195
   translators:
   - ΧΑΤΖΟΠΟΥΛΟΥ,ΡΟΥΛΑ
   edition: '5'
   editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
   edition_year: 2006
   pages: 220
   topics:
@@ -356515,15 +356341,15 @@
   offprint: false
   isbn: 960-422-120-5
   original_entry:
     0: 7092
     1: ΤΟΥΕΙΝ,ΜΑΡΚ
     2: ΠΡΙΓΚΙΠΑΣ ΚΑΙ ΦΤΩΧΟΣ
     4: 808.899TOY
-    5: 9195A
+    5: 09195
     6: ΡΟΥΛΑ ΧΑΤΖΟΠΟΥΛΟΥ
     7: 5η
     8: ΑΓΚΥΡΑ
     9: ΑΘΗΝΑ
     10: '2006'
     11: 220Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -356544,20 +356370,20 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7093
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: ΡΟΒΗΡΟΣ Ο ΚΑΤΑΚΤΗΤΗΣ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
-  - 9175Α
+  - 09175
   translators:
   - ΚΡΙΜΠΑΣ,ΓΙΩΡΓΟΣ
   editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
   edition_year: 2004
   pages: 211
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -356566,15 +356392,15 @@
   offprint: false
   isbn: 960-422-082-9
   original_entry:
     0: 7093
     1: ΒΕΡΝ,ΙΟΥΛΙΟΣ
     2: ΡΟΒΗΡΟΣ Ο ΚΑΤΑΚΤΗΤΗΣ
     4: 808.899ΒΕΡ
-    5: 9175Α
+    5: 09175
     6: ΓΙΩΡΓΟΥ ΚΡΙΜΠΑ
     8: ΑΓΚΥΡΑ
     9: ΑΘΗΝΑ
     10: '2004'
     11: 211Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -356600,15 +356426,15 @@
 - dbase_number: 7094
   authors:
   - ΚΙΠΛΙΝΓΚ,Ρ.
   language: el
   title: ΟΙ ΜΙΚΡΟΙ ΘΑΛΑΣΣΟΛΥΚΟΙ
   dewey: 808.899 ΚΙΠ
   entry_numbers:
-  - 9197Α
+  - 09197
   translators:
   - ΤΣΟΥΚΑΛΑΣ,Γ.
   editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
   edition_year: 2004
   pages: 203
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -356617,15 +356443,15 @@
   offprint: false
   isbn: 960-422-134-5
   original_entry:
     0: 7094
     1: ΚΙΠΛΙΝΓΚ,Ρ.
     2: ΟΙ ΜΙΚΡΟΙ ΘΑΛΑΣΣΟΛΥΚΟΙ
     4: 808.899ΚΙΠ
-    5: 9197Α
+    5: 09197
     6: Γ.ΤΣΟΥΚΑΛΑΣ
     8: ΑΓΚΥΡΑ
     9: ΑΘΗΝΑ
     10: '2004'
     11: 203Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -356646,20 +356472,20 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7095
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: Ο ΔΕΚΑΠΕΝΤΑΕΤΗΣ ΠΛΟΙΑΡΧΟΣ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
-  - 9170Α
+  - 09170
   translators:
   - ΦΕΡΤΑΚΗ,ΑΝΝΙΚΑ
   edition: '5'
   editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
   edition_year: 2006
   pages: 362
   topics:
@@ -356669,15 +356495,15 @@
   offprint: false
   isbn: 960-422-098-5
   original_entry:
     0: 7095
     1: ΒΕΡΝ,ΙΟΥΛΙΟΣ
     2: Ο ΔΕΚΑΠΕΝΤΑΕΤΗΣ ΠΛΟΙΑΡΧΟΣ
     4: 808.899ΒΕΡ
-    5: 9170Α
+    5: 09170
     6: ΑΝΝΙΚΑ ΦΕΡΤΑΚΗ
     7: 5η
     8: ΑΓΚΥΡΑ
     9: ΑΘΗΝΑ
     10: '2006'
     11: 362Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -356703,15 +356529,15 @@
 - dbase_number: 7096
   authors:
   - ΝΤΕΦΟΕ,ΝΤΑΝΙΕΛ
   language: el
   title: ΡΟΒΙΝΣΩΝ ΚΡΟΥΣΟΣ
   dewey: 808.899 ΝΤΕ
   entry_numbers:
-  - 9172Α
+  - 09172
   translators:
   - ΦΕΡΤΑΚΗ,ΑΝΝΙΚΑ
   editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
   edition_year: 2004
   pages: 403
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -356720,15 +356546,15 @@
   offprint: false
   isbn: 960-422-070-5
   original_entry:
     0: 7096
     1: ΝΤΕΦΟΕ,ΝΤΑΝΙΕΛ
     2: ΡΟΒΙΝΣΩΝ ΚΡΟΥΣΟΣ
     4: 808.899ΝΤΕ
-    5: 9172Α
+    5: 09172
     6: ΑΝΝΙΚΑ ΦΕΡΤΑΚΗ
     8: ΑΓΚΥΡΑ
     9: ΑΘΗΝΑ
     10: '2004'
     11: 403Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -356754,15 +356580,15 @@
 - dbase_number: 7097
   authors:
   - ΔΟΥΜΑΣ,ΑΛΕΞΑΝΔΡΟΣ
   language: el
   title: ΟΙ ΤΡΕΙΣ ΣΩΜΑΤΟΦΥΛΑΚΕΣ
   dewey: 808.899 ΔΟΥ
   entry_numbers:
-  - 9196Α
+  - 09196
   - '9096'
   translators:
   - ΤΣΟΥΚΑΛΑΣ,Γ.
   editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
   edition_year: 2008
   pages: 284
   topics:
@@ -356773,15 +356599,15 @@
   offprint: false
   ean: 978-960-422-587-3
   original_entry:
     0: 7097
     1: ΔΟΥΜΑΣ,ΑΛΕΞΑΝΔΡΟΣ
     2: ΟΙ ΤΡΕΙΣ ΣΩΜΑΤΟΦΥΛΑΚΕΣ
     4: 808.899ΔΟΥ
-    5: 9196Α-9096
+    5: 09196-9096
     6: Γ.ΤΣΟΥΚΑΛΑΣ
     8: ΑΓΚΥΡΑ
     9: ΑΘΗΝΑ
     10: '2008'
     11: 284Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -356807,30 +356633,30 @@
 - dbase_number: 7098
   authors:
   - ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
   language: el
   title: Ο ΗΡΑΚΛΗΣ
   dewey: 808.899 ΛΟΥ
   entry_numbers:
-  - 9182Α
+  - 09182
   editor: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ // ΑΘΗΝΑ
   edition_year: 2000
   pages: 213
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   isbn: 960-393-135-7
   original_entry:
     0: 7098
     1: ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
     2: Ο ΗΡΑΚΛΗΣ
     4: 808.899ΛΟΥ
-    5: 9182Α
+    5: 09182
     8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
     9: ΑΘΗΝΑ
     10: '2000'
     11: 213Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -356856,30 +356682,30 @@
 - dbase_number: 7099
   authors:
   - ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
   language: el
   title: ΕΝΑ ΠΑΙΔΙ ΜΕΤΡΑΕΙ ΤΑ ΑΣΤΡΑ
   dewey: 808.899 ΛΟΥ
   entry_numbers:
-  - 9180Α
+  - 09180
   editor: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ // ΑΘΗΝΑ
   edition_year: 1999
   pages: 540
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-344-768-9
   original_entry:
     0: 7099
     1: ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
     2: ΕΝΑ ΠΑΙΔΙ ΜΕΤΡΑΕΙ ΤΑ ΑΣΤΡΑ
     4: 808.899ΛΟΥ
-    5: 9180A
+    5: 09180
     8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
     9: ΑΘΗΝΑ
     10: '1999'
     11: 540Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -356905,30 +356731,30 @@
 - dbase_number: 7100
   authors:
   - ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
   language: el
   title: ΒΟΥΡΚΩΜΕΝΕΣ ΜΕΡΕΣ
   dewey: 808.899 ΛΟΥ
   entry_numbers:
-  - 9226Α
+  - 09226
   editor: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ // ΑΘΗΝΑ
   edition_year: 2000
   pages: 150
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   isbn: 960-344-914-8
   original_entry:
     0: 7100
     1: ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
     2: ΒΟΥΡΚΩΜΕΝΕΣ ΜΕΡΕΣ
     4: 808.899ΛΟΥ
-    5: 9226Α
+    5: 09226
     8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
     9: ΑΘΗΝΑ
     10: '2000'
     11: 150Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -356954,30 +356780,30 @@
 - dbase_number: 7101
   authors:
   - ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
   language: el
   title: ΔΑΙΔΑΛΟΣ
   dewey: 808.899 ΛΟΥ
   entry_numbers:
-  - 9181Α
+  - 09181
   editor: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ // ΑΘΗΝΑ
   edition_year: 2000
   pages: 243
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   isbn: 960-393-136-5
   original_entry:
     0: 7101
     1: ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
     2: ΔΑΙΔΑΛΟΣ
     4: 808.899ΛΟΥ
-    5: 9181Α
+    5: 09181
     8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
     9: ΑΘΗΝΑ
     10: '2000'
     11: 243Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357003,30 +356829,30 @@
 - dbase_number: 7102
   authors:
   - ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
   language: el
   title: Ο ΙΚΑΡΟΣ
   dewey: 808.899 ΛΟΥ
   entry_numbers:
-  - 9179Α
+  - 09179
   editor: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ // ΑΘΗΝΑ
   edition_year: 1999
   pages: 233
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   isbn: 960-344-835-4
   original_entry:
     0: 7102
     1: ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
     2: Ο ΙΚΑΡΟΣ
     4: 808.899ΛΟΥ
-    5: 9179Α
+    5: 09179
     8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
     9: ΑΘΗΝΑ
     10: '1999'
     11: 233Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357052,30 +356878,30 @@
 - dbase_number: 7103
   authors:
   - ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
   language: el
   title: ΘΗΣΕΑΣ
   dewey: 808.899 ΛΟΥ
   entry_numbers:
-  - 9178Α
+  - 09178
   editor: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ // ΑΘΗΝΑ
   edition_year: 1999
   pages: 280
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   isbn: 960-344-771-4
   original_entry:
     0: 7103
     1: ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
     2: ΘΗΣΕΑΣ
     4: 808.899ΛΟΥ
-    5: 9178Α
+    5: 09178
     8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
     9: ΑΘΗΝΑ
     10: '1999'
     11: 280Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357101,30 +356927,30 @@
 - dbase_number: 7104
   authors:
   - ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
   language: el
   title: ΚΑΛΗΝΥΧΤΑ ΖΩΗ
   dewey: 808.899 ΛΟΥ
   entry_numbers:
-  - 9214Α
+  - 09214
   editor: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ // ΑΘΗΝΑ
   edition_year: 2000
   pages: 259
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   isbn: 960-393-138-1
   original_entry:
     0: 7104
     1: ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
     2: ΚΑΛΗΝΥΧΤΑ ΖΩΗ
     4: 808.899ΛΟΥ
-    5: 9214Α
+    5: 09214
     8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
     9: ΑΘΗΝΑ
     10: '2000'
     11: 259Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357150,15 +356976,15 @@
 - dbase_number: 7105
   authors:
   - ΤΟΥΕΙΝ,ΜΑΡΚ
   language: el
   title: ΟΙ ΠΕΡΙΠΕΤΕΙΕΣ ΤΟΥ ΤΟΜ ΣΟΓΙΕΡ
   dewey: 808.899 ΤΟΥ
   entry_numbers:
-  - 9185Α
+  - 09185
   translators:
   - ΔΙΑΜΑΝΤΟΠΟΥΛ,ΠΙΕΡΕΤΑ
   editor: ΕΡΕΥΝΗΤΕΣ // ΑΘΗΝΑ
   edition_year: 1999
   pages: 284
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357167,15 +356993,15 @@
   offprint: false
   isbn: 960-368-155-5
   original_entry:
     0: 7105
     1: ΤΟΥΕΙΝ,ΜΑΡΚ
     2: ΟΙ ΠΕΡΙΠΕΤΕΙΕΣ ΤΟΥ ΤΟΜ ΣΟΓΙΕΡ
     4: 808.899ΤΟΥ
-    5: 9185Α
+    5: 09185
     6: ΠΙΕΡΕΤΑ ΔΙΑΜΑΝΤΟΠΟΥΛ
     8: ΕΡΕΥΝΗΤΕΣ
     9: ΑΘΗΝΑ
     10: '1999'
     11: 284Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357201,15 +357027,15 @@
 - dbase_number: 7106
   authors:
   - ΣΙΟΥΕΛ,ΑΝΝΑ
   language: el
   title: ΜΑΥΡΗ ΚΑΛΛΟΝΗ
   dewey: 808.899 ΣΙΟ
   entry_numbers:
-  - 9177Α
+  - 09177
   translators:
   - ΜΑΡΚΑΚΗΣ,ΓΙΩΡΓΟΣ
   editor: ΕΡΕΥΝΗΤΕΣ // ΑΘΗΝΑ
   edition_year: 2001
   pages: 207
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357218,15 +357044,15 @@
   offprint: false
   isbn: 960-368-232-2
   original_entry:
     0: 7106
     1: ΣΙΟΥΕΛ,ΑΝΝΑ
     2: ΜΑΥΡΗ ΚΑΛΛΟΝΗ
     4: 808.899ΣΙΟ
-    5: 9177Α
+    5: 09177
     6: ΓΙΩΡΓΟΣ ΜΑΡΚΑΚΗΣ
     8: ΕΡΕΥΝΗΤΕΣ
     9: ΑΘΗΝΑ
     10: '2001'
     11: 207Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357247,15 +357073,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7107
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: ΤΟ ΑΙΓΑΙΟ ΣΤΙΣ ΦΛΟΓΕΣ
   dewey: 880.09 ΒΕΡ
   entry_numbers:
   - '9187'
   translators:
   - ΚΟΥΤΑΛΟΥ,ΜΑΡΙΑΝΝΑ
@@ -357351,15 +357177,15 @@
 - dbase_number: 7109
   authors:
   - ΛΟΝΤΟΝ,ΤΖΑΚ
   language: el
   title: ΑΣΠΡΟΔΟΝΤΗΣ
   dewey: 808.899 ΛΟΝ
   entry_numbers:
-  - 9184Α
+  - 09184
   translators:
   - ΜΑΡΚΑΚΗΣ,ΓΙΩΡΓΟΣ
   editor: ΕΡΕΥΝΗΤΕΣ // ΑΘΗΝΑ
   edition_year: 2002
   pages: 237
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357368,15 +357194,15 @@
   offprint: false
   isbn: 960-368-238-1
   original_entry:
     0: 7109
     1: ΛΟΝΤΟΝ,ΤΖΑΚ
     2: ΑΣΠΡΟΔΟΝΤΗΣ
     4: 808.899ΛΟΝ
-    5: 9184Α
+    5: 09184
     6: ΓΙΩΡΓΟΣ ΜΑΡΚΑΚΗΣ
     8: ΕΡΕΥΝΗΤΕΣ
     9: ΑΘΗΝΑ
     10: '2002'
     11: 237Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357402,15 +357228,15 @@
 - dbase_number: 7110
   authors:
   - ΣΑΡΗ,ΖΩΡΖ
   language: el
   title: ΤΑ ΓΕΝΕΘΛΙΑ
   dewey: 808.899 ΣΑΡ
   entry_numbers:
-  - 9204Α
+  - 09204
   edition: '25'
   editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
   edition_year: 2007
   pages: 247
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
@@ -357418,15 +357244,15 @@
   offprint: false
   ean: 978-960-293-681-8
   original_entry:
     0: 7110
     1: ΣΑΡΗ,ΖΩΡΖ
     2: ΤΑ ΓΕΝΕΘΛΙΑ
     4: 808.899ΣΑΡ
-    5: 9204Α
+    5: 09204
     7: 25η
     8: ΠΑΤΑΚΗ
     9: ΑΘΗΝΑ
     10: '2007'
     11: 247Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357452,15 +357278,15 @@
 - dbase_number: 7111
   authors:
   - ΣΑΡΗ,ΖΩΡΖ
   language: el
   title: ΤΟ ΠΑΡΑΡΑΔΙΑΣΜΑ
   dewey: 808.899 ΣΑΡ
   entry_numbers:
-  - 9205Α
+  - 09205
   edition: '22'
   editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
   edition_year: 2006
   pages: 202
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
@@ -357468,15 +357294,15 @@
   offprint: false
   isbn: 960-293-477-8
   original_entry:
     0: 7111
     1: ΣΑΡΗ,ΖΩΡΖ
     2: ΤΟ ΠΑΡΑΡΑΔΙΑΣΜΑ
     4: 808.899ΣΑΡ
-    5: 9205Α
+    5: 09205
     7: 22η
     8: ΠΑΤΑΚΗ
     9: ΑΘΗΝΑ
     10: '2006'
     11: 202Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357502,15 +357328,15 @@
 - dbase_number: 7112
   authors:
   - ΣΑΡΗ,ΖΩΡΖ
   language: el
   title: ΚΟΚΚΙΝΗ ΚΛΩΣΤΗ ΔΕΜΕΝΗ
   dewey: 808.899 ΣΑΡ
   entry_numbers:
-  - 9199Α
+  - 09199
   edition: '19'
   editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
   edition_year: 2007
   pages: 114
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
@@ -357518,15 +357344,15 @@
   offprint: false
   ean: 978-960-293-682-5
   original_entry:
     0: 7112
     1: ΣΑΡΗ,ΖΩΡΖ
     2: ΚΟΚΚΙΝΗ ΚΛΩΣΤΗ ΔΕΜΕΝΗ
     4: 808.899ΣΑΡ
-    5: 9199Α
+    5: 09199
     7: 19η
     8: ΠΑΤΑΚΗ
     9: ΑΘΗΝΑ
     10: '2007'
     11: 114Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357552,15 +357378,15 @@
 - dbase_number: 7113
   authors:
   - ΣΑΡΗ,ΖΩΡΖ
   language: el
   title: ΤΑ ΣΤΕΝΑ ΠΑΠΟΥΤΣΙΑ
   dewey: 808.899 ΣΑΡ
   entry_numbers:
-  - 9208Α
+  - 09208
   edition: '27'
   editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
   edition_year: 2007
   pages: 166
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
@@ -357568,15 +357394,15 @@
   offprint: false
   ean: 978-960-293-676-4
   original_entry:
     0: 7113
     1: ΣΑΡΗ,ΖΩΡΖ
     2: ΤΑ ΣΤΕΝΑ ΠΑΠΟΥΤΣΙΑ
     4: 808.899ΣΑΡ
-    5: 9208Α
+    5: 09208
     7: 27η
     8: ΠΑΤΑΚΗ
     9: ΑΘΗΝΑ
     10: '2007'
     11: 166Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357602,15 +357428,15 @@
 - dbase_number: 7114
   authors:
   - ΖΕΗ,ΑΛΚΗ
   language: el
   title: ΤΟ ΚΑΠΛΑΝΙ ΤΗΣ ΒΙΤΡΙΝΑΣ
   dewey: 808.899 ΖΕΗ
   entry_numbers:
-  - 9209Α
+  - 09209
   edition: '238'
   editor: ΚΕΔΡΟΣ // ΑΘΗΝΑ
   edition_year: 2007
   pages: 183
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
@@ -357618,15 +357444,15 @@
   offprint: false
   ean: 978-960-04-0007-6
   original_entry:
     0: 7114
     1: ΖΕΗ,ΑΛΚΗ
     2: ΤΟ ΚΑΠΛΑΝΙ ΤΗΣ ΒΙΤΡΙΝΑΣ
     4: 808.899ΖΕΗ
-    5: 9209Α
+    5: 09209
     7: 238η
     8: ΚΕΔΡΟΣ
     9: ΑΘΗΝΑ
     10: '2007'
     11: 183Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357652,15 +357478,15 @@
 - dbase_number: 7115
   authors:
   - ΣΑΡΗ,ΖΩΡΖ
   language: el
   title: ΣΟΦΙΑ
   dewey: 808.899 ΣΑΡ
   entry_numbers:
-  - 9200Α
+  - 09200
   edition: '11'
   editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
   edition_year: 2008
   pages: 133
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
@@ -357668,15 +357494,15 @@
   offprint: false
   ean: 978-960-600-774-3
   original_entry:
     0: 7115
     1: ΣΑΡΗ,ΖΩΡΖ
     2: ΣΟΦΙΑ
     4: 808.899ΣΑΡ
-    5: 9200Α
+    5: 09200
     7: 11η
     8: ΠΑΤΑΚΗ
     9: ΑΘΗΝΑ
     10: '2008'
     11: 133Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357702,15 +357528,15 @@
 - dbase_number: 7116
   authors:
   - ΣΑΡΗ,ΖΩΡΖ
   language: el
   title: ΟΤΑΝ Ο ΗΛΙΟΣ...
   dewey: 808.899 ΣΑΡ
   entry_numbers:
-  - 9203Α
+  - 09203
   edition: '21'
   editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
   edition_year: 2007
   pages: 260
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
@@ -357718,15 +357544,15 @@
   offprint: false
   ean: 978-960-293-677-1
   original_entry:
     0: 7116
     1: ΣΑΡΗ,ΖΩΡΖ
     2: ΟΤΑΝ Ο ΗΛΙΟΣ...
     4: 808.899ΣΑΡ
-    5: 9203Α
+    5: 09203
     7: 21η
     8: ΠΑΤΑΚΗ
     9: ΑΘΗΝΑ
     10: '2007'
     11: 260Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357752,15 +357578,15 @@
 - dbase_number: 7117
   authors:
   - ΣΑΡΗ,ΖΩΡΖ
   language: el
   title: ΤΟΤΕ...
   dewey: 808.899 ΣΑΡ
   entry_numbers:
-  - 9207Α
+  - 09207
   edition: '4'
   editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
   edition_year: 2006
   pages: 124
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
@@ -357768,15 +357594,15 @@
   offprint: false
   isbn: 960-16-1318-8
   original_entry:
     0: 7117
     1: ΣΑΡΗ,ΖΩΡΖ
     2: ΤΟΤΕ...
     4: 808.899ΣΑΡ
-    5: 9207Α
+    5: 09207
     7: 4η
     8: ΠΑΤΑΚΗ
     9: ΑΘΗΝΑ
     10: '2006'
     11: 124Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357802,15 +357628,15 @@
 - dbase_number: 7118
   authors:
   - ΣΑΡΗ,ΖΩΡΖ
   language: el
   title: Ο ΚΥΡΙΟΣ ΜΟΥ
   dewey: 808.899 ΣΑΡ
   entry_numbers:
-  - 9202Α
+  - 09202
   edition: '9'
   editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
   edition_year: 2007
   pages: 131
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
@@ -357818,15 +357644,15 @@
   offprint: false
   ean: 978-960-16-0382-7
   original_entry:
     0: 7118
     1: ΣΑΡΗ,ΖΩΡΖ
     2: Ο ΚΥΡΙΟΣ ΜΟΥ
     4: 808.899ΣΑΡ
-    5: 9202Α
+    5: 09202
     7: 9η
     8: ΠΑΤΑΚΗ
     9: ΑΘΗΝΑ
     10: '2007'
     11: 131Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357852,15 +357678,15 @@
 - dbase_number: 7119
   authors:
   - ΣΑΡΗ,ΖΩΡΖ
   language: el
   title: ΚΡΙΜΑ ΚΙ ΑΔΙΚΟ
   dewey: 808.899 ΣΑΡ
   entry_numbers:
-  - 9206Α
+  - 09206
   edition: '21'
   editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
   edition_year: 2008
   pages: 142
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
@@ -357868,15 +357694,15 @@
   offprint: false
   ean: 978-960-293-563-7
   original_entry:
     0: 7119
     1: ΣΑΡΗ,ΖΩΡΖ
     2: ΚΡΙΜΑ ΚΙ ΑΔΙΚΟ
     4: 808.899ΣΑΡ
-    5: 9206Α
+    5: 09206
     7: 21η
     8: ΠΑΤΑΚΗ
     9: ΑΘΗΝΑ
     10: '2008'
     11: 142Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357902,15 +357728,15 @@
 - dbase_number: 7120
   authors:
   - ΔΕΛΤΑ,ΠΗΝΕΛΟΠΗ
   language: el
   title: ΤΡΕΛΑΝΤΩΝΗΣ
   dewey: 808.899 ΔΕΛ
   entry_numbers:
-  - 9189Α
+  - 09189
   edition: '22'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 2006
   pages: 286
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
@@ -357918,15 +357744,15 @@
   offprint: false
   isbn: 960-05-0379-6
   original_entry:
     0: 7120
     1: ΔΕΛΤΑ,ΠΗΝΕΛΟΠΗ
     2: ΤΡΕΛΑΝΤΩΝΗΣ
     4: 808.899ΔΕΛ
-    5: 9189Α
+    5: 09189
     7: 22η
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: '2006'
     11: 286Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΝΧΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΝΧΙΑ
@@ -357952,15 +357778,15 @@
 - dbase_number: 7121
   authors:
   - ΣΚΟΤΤ,ΟΥΟΛΤΕΡ
   language: el
   title: ΙΒΑΝΟΗΣ
   dewey: 808.899 ΣΚΟ
   entry_numbers:
-  - 9183Α
+  - 09183
   translators:
   - ΣΠΑΝΔΩΝΗΣ,ΓΙΑΝΝΗΣ
   editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
   edition_year: 1994
   pages: 483
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -357969,15 +357795,15 @@
   offprint: false
   isbn: 960-360-028-8
   original_entry:
     0: 7121
     1: ΣΚΟΤΤ,ΟΥΟΛΤΕΡ
     2: ΙΒΑΝΟΗΣ
     4: 808.899ΣΚΟ
-    5: 9183Α
+    5: 09183
     6: ΓΙΑΝΝΗΣ ΣΠΑΝΔΩΝΗΣ
     8: ΠΑΤΑΚΗ
     9: ΑΘΗΝΑ
     10: '1994'
     11: '483'
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -358003,15 +357829,15 @@
 - dbase_number: 7122
   authors:
   - ΔΕΛΤΑ,ΠΗΝΕΛΟΠΗ
   language: el
   title: Η ΖΩΗ ΤΟΥ ΧΡΙΣΤΟΥ
   dewey: 808.899 ΔΕΛ
   entry_numbers:
-  - 9193Α
+  - 09193
   edition: '4'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 2000
   pages: 483
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
@@ -358019,15 +357845,15 @@
   offprint: false
   isbn: 960-05-0386-9
   original_entry:
     0: 7122
     1: ΔΕΛΤΑ,ΠΗΝΕΛΟΠΗ
     2: Η ΖΩΗ ΤΟΥ ΧΡΙΣΤΟΥ
     4: 808.899ΔΕΛ
-    5: 9193Α
+    5: 09193
     7: 4η
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: '2000'
     11: 483Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -358105,15 +357931,15 @@
 - dbase_number: 7124
   authors:
   - ΔΕΛΤΑ,ΠΗΝΕΛΟΠΗ
   language: el
   title: ΣΤΑ ΜΥΣΤΙΚΑ ΤΟΥ ΒΑΛΤΟΥ
   dewey: 808.899 ΔΕΛ
   entry_numbers:
-  - 9190Α
+  - 09190
   edition: '19'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 2007
   pages: 645
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   copies: 2
@@ -358122,15 +357948,15 @@
   offprint: false
   isbn: 960-05-0343-5
   original_entry:
     0: 7124
     1: ΔΕΛΤΑ,ΠΗΝΕΛΟΠΗ
     2: ΣΤΑ ΜΥΣΤΙΚΑ ΤΟΥ ΒΑΛΤΟΥ
     4: 808.899ΔΕΛ
-    5: 9190Α
+    5: 09190
     7: 19η
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: '2007'
     11: 645Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -358156,30 +357982,30 @@
 - dbase_number: 7125
   authors:
   - ΠΑΠΑΝΤΩΝΙΟΥ,ΖΑΧΑΡΙΑΣ
   language: el
   title: ΤΑ ΨΗΛΑ ΒΟΥΝΑ
   dewey: 808.899 ΠΑΠ
   entry_numbers:
-  - 9188Α
+  - 09188
   edition: '33'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 2007
   pages: 225
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7125
     1: ΠΑΠΑΝΤΩΝΙΟΥ,ΖΑΧΑΡΙΑΣ
     2: ΤΑ ΨΗΛΑ ΒΟΥΝΑ
     4: 808.899ΠΑΠ
-    5: 9188Α
+    5: 09188
     7: 33η
     8: ΕΣΤΙΑ
     9: ΑΘΗΝΑ
     10: '2007'
     11: 225Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -358675,15 +358501,15 @@
 - dbase_number: 7135
   authors:
   - ΣΕΤΣΙΝΓΚ,ΦΡΑΝΚ
   language: el
   title: ΤΟ ΣΜΗΝΟΣ
   dewey: 830.11 ΣΕΤ
   entry_numbers:
-  - 9212Α
+  - 09212
   translators:
   - ΤΖΑΝΝΕΤΑΤΟΣ,ΣΤΕΦΑΝΟΣ
   editor: ΚΑΣΤΑΝΙΩΤΗΣ // ΑΘΗΝΑ
   edition_year: 2007
   pages: 1018
   topics:
   - ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -358693,15 +358519,15 @@
   offprint: false
   ean: 978-960-03-4265-9
   original_entry:
     0: 7135
     1: ΣΕΤΣΙΝΓΚ,ΦΡΑΝΚ
     2: ΤΟ ΣΜΗΝΟΣ
     4: 830.11ΣΕΤ
-    5: 9212Α
+    5: 09212
     6: ΣΤΕΦΑΝΟΣ ΤΖΑΝΝΕΤΑΤΟΣ
     8: ΚΑΣΤΑΝΙΩΤΗΣ
     9: ΑΘΗΝΑ
     10: '2007'
     11: 1018Σ
     12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -358778,15 +358604,15 @@
 - dbase_number: 7137
   authors:
   - ΠΟΛΥΡΑΚΗΣ,ΓΙΩΡΓΟΣ
   language: el
   title: ΣΙΩΠΗΛΕΣ ΚΡΑΥΓΕΣ
   dewey: 889.21 ΠΟΛ
   entry_numbers:
-  - 9159Α
+  - 09159
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
   edition_year: 2007
   pages: 447
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
@@ -358794,15 +358620,15 @@
   offprint: false
   ean: 978-960-453-158-5
   original_entry:
     0: 7137
     1: ΠΟΛΥΡΑΚΗΣ,ΓΙΩΡΓΟΣ
     2: ΣΙΩΠΗΛΕΣ ΚΡΑΥΓΕΣ
     4: 889.21ΠΟΛ
-    5: 9159Α
+    5: 09159
     8: ΨΥΧΟΓΙΟΣ
     9: ΑΘΗΝΑ
     10: '2007'
     11: 447Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΜΥΘΙΣΤΟΡΗΜΑ
@@ -358930,15 +358756,15 @@
 - dbase_number: 7140
   authors:
   - NEVILLE,KATHERINE
   language: el
   title: ΟΧΤΩ
   dewey: 823 NEV
   entry_numbers:
-  - 9153Α
+  - 09153
   translators:
   - ΣΑΚΕΛΛΑΡΟΠΟΥΛΟ,ΧΡΙΣΤ.
   editor: ΝΕΑ ΣΥΝΟΡΑ // ΑΘΗΝΑ
   edition_year: 2005
   pages: 767
   topics:
   - ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -358948,15 +358774,15 @@
   offprint: false
   isbn: 960-14-1043-0
   original_entry:
     0: 7140
     1: NEVILLE,KATHERINE
     2: ΟΧΤΩ
     4: 823NEV
-    5: 9153Α
+    5: 09153
     6: ΧΡΙΣΤ.ΣΑΚΕΛΛΑΡΟΠΟΥΛΟ
     8: ΝΕΑ ΣΥΝΟΡΑ
     9: ΑΘΗΝΑ
     10: '2005'
     11: 767Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -358981,15 +358807,16 @@
     30: null
 - dbase_number: 7141
   authors:
   - BROWN,DAN
   language: el
   title: ΑΡΚΤΙΚΟΣ ΚΥΚΛΟΣ
   dewey: 810.11 BRO
-  entry_numbers: []
+  entry_numbers:
+  - '9258'
   translators:
   - ΚΑΨΑΛΗΣ,ΧΡΗΣΤΟΣ
   editor: ΛΙΒΑΝΗ // ΑΘΗΝΑ
   edition_year: 2005
   pages: 644
   topics:
   - ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -358999,26 +358826,26 @@
   offprint: false
   isbn: 960-14-1024-4
   original_entry:
     0: 7141
     1: BROWN,DAN
     2: ΑΡΚΤΙΚΟΣ ΚΥΚΛΟΣ
     4: 810.11BRO
+    5: '9258'
     6: ΧΡΗΣΤΟΣ ΚΑΨΑΛΗΣ
     8: ΛΙΒΑΝΗ
     9: ΑΘΗΝΑ
     10: '2005'
     11: 644Σ
     12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΑΜΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΜΥΘΙΣΤΟΡΗΜΑ
     18: 960-14-102
     19: 4-4
     3: null
-    5: null
     7: null
     15: null
     16: null
     17: null
     20: null
     21: null
     22: null
@@ -359033,15 +358860,15 @@
 - dbase_number: 7142
   authors:
   - GOLDEN,ARTHUR
   language: el
   title: ΑΝΑΜΝΗΣΕΙΣ ΜΙΑΣ ΓΚΕΙΣΑΣ
   dewey: 810.11 GOL
   entry_numbers:
-  - 9168Α
+  - 09168
   translators:
   - ΛΕΚΚΟΥ-ΔΑΝΤΟΥ,ΡΕΝΑ
   editor: ΛΙΒΑΝΗ // ΑΘΗΝΑ
   edition_year: 1998
   pages: 732
   topics:
   - ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -359051,15 +358878,15 @@
   offprint: false
   isbn: 960-236-913-2
   original_entry:
     0: 7142
     1: GOLDEN,ARTHUR
     2: ΑΝΑΜΝΗΣΕΙΣ ΜΙΑΣ ΓΚΕΙΣΑΣ
     4: 810.11GOL
-    5: 9168Α
+    5: 09168
     6: ΡΕΝΑ ΛΕΚΚΟΥ-ΔΑΝΤΟΥ
     8: ΛΙΒΑΝΗ
     9: ΑΘΗΝΑ
     10: '1998'
     11: 732Σ
     12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -359085,15 +358912,15 @@
 - dbase_number: 7143
   authors:
   - ΔΗΜΟΥΛΙΔΟΥ,ΧΡΥΣΑ
   language: el
   title: ΤΟ ΦΙΛΙ ΤΟΥ ΔΡΑΚΟΥ
   dewey: 889.21 ΔΗΜ
   entry_numbers:
-  - 9162Α
+  - 09162
   editor: ΛΙΒΑΝΗ // ΑΘΗΝΑ
   edition_year: 2007
   pages: 460
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
@@ -359101,15 +358928,15 @@
   offprint: false
   ean: 978-960-14-1475-1
   original_entry:
     0: 7143
     1: ΔΗΜΟΥΛΙΔΟΥ,ΧΡΥΣΑ
     2: ΤΟ ΦΙΛΙ ΤΟΥ ΔΡΑΚΟΥ
     4: 889.21ΔΗΜ
-    5: 9162Α
+    5: 09162
     8: ΛΙΒΑΝΗ
     9: ΑΘΗΝΑ
     10: '2007'
     11: 460Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -359236,15 +359063,15 @@
     30: null
 - dbase_number: 7146
   authors:
   - HAMMOND,N.G.
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   subtitle: Η ΙΣΤΟΡΙΚΗ ΓΕΩΓΡΑΦΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ (ΜΕΡΟΣ Α)
-  dewey: '398.666'
+  dewey: 938.1 HAM
   entry_numbers:
   - '9217'
   - '9473'
   editor: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
   pages: 280
   topics:
@@ -359256,15 +359083,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 7146
     1: HAMMOND,N.G.
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     3: Η ΙΣΤΟΡΙΚΗ ΓΕΩΓΡΑΦΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ (ΜΕΡΟΣ Α)
-    4: '398.666'
+    4: 938.1HAM
     5: 9217-9473
     8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2007'
     11: 280Σ
     12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
     13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
@@ -359289,15 +359116,15 @@
     30: null
 - dbase_number: 7147
   authors:
   - HAMMOND,N.G.
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   subtitle: Η ΙΣΤΟΡΙΚΗ ΓΕΩΓΡΑΦΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ (ΜΕΡΟΣ Β)
-  dewey: '398.666'
+  dewey: 938.1 HAM
   entry_numbers:
   - '9217'
   - '9473'
   editor: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
   pages: 280
   topics:
@@ -359310,16 +359137,16 @@
   offprint: false
   ean: 978-960-457-138-3
   original_entry:
     0: 7147
     1: HAMMOND,N.G.
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     3: Η ΙΣΤΟΡΙΚΗ ΓΕΩΓΡΑΦΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ (ΜΕΡΟΣ Β)
-    4: '398.666'
-    5: 9217 -9473
+    4: 938.1HAM
+    5: 9217-9473
     8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2007'
     11: 280Σ
     12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
     13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     14: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
@@ -359343,15 +359170,15 @@
     30: null
 - dbase_number: 7148
   authors:
   - HAMMOND,N.G.
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   subtitle: Η ΠΡΟΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
-  dewey: '398.666'
+  dewey: 938.1 HAM
   entry_numbers:
   - '9217'
   - '9473'
   editor: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
   pages: 300
   topics:
@@ -359364,15 +359191,15 @@
   offprint: false
   ean: 978-960-457-139-0
   original_entry:
     0: 7148
     1: HAMMOND,N.G.
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     3: Η ΠΡΟΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
-    4: '398.666'
+    4: 938.1HAM
     5: 9217-9473
     8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2007'
     11: 300Σ
     12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
     13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
@@ -359397,14 +359224,15 @@
     30: null
 - dbase_number: 7149
   authors:
   - HAMMOND,N.G.
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   subtitle: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 800-452 Π.Χ.
+  dewey: 938.1 HAM
   entry_numbers:
   - '9217'
   editor: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
   pages: 300
   topics:
   - ΙΣΤΟΡΙΑ ΜΑΚΕΔΟΝΙΑΣ
@@ -359416,26 +359244,26 @@
   offprint: false
   ean: 978-960-457-140-6
   original_entry:
     0: 7149
     1: HAMMOND,N.G.
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     3: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 800-452 Π.Χ.
+    4: 938.1HAM
     5: '9217'
     8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2007'
     11: 300Σ
     12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
     13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     14: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
     17: ΤΟΜΟΣ 4
     18: 978-960-45
     19: 7-140-6
-    4: null
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -359449,14 +359277,15 @@
     30: null
 - dbase_number: 7150
   authors:
   - HAMMOND,N.G.
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   subtitle: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 452-355 Π.Χ.
+  dewey: 938.1 HAM
   entry_numbers:
   - '9217'
   editor: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
   pages: 300
   topics:
   - ΙΣΤΟΡΙΑ ΜΑΚΕΔΟΝΙΑΣ
@@ -359468,26 +359297,26 @@
   offprint: false
   ean: 978-960-457-143-7
   original_entry:
     0: 7150
     1: HAMMOND,N.G.
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     3: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 452-355 Π.Χ.
+    4: 938.1HAM
     5: '9217'
     8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2007'
     11: 300Σ
     12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
     13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     14: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
     17: ΤΟΜΟΣ 5
     18: 978-960-45
     19: 7-143-7
-    4: null
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -359501,14 +359330,15 @@
     30: null
 - dbase_number: 7151
   authors:
   - HAMMOND,N.G.
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   subtitle: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 355-346 Π.Χ.
+  dewey: 938.1 HAM
   entry_numbers:
   - '9217'
   editor: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
   pages: 300
   topics:
   - ΙΣΤΟΡΙΑ ΜΑΚΕΔΟΝΙΑΣ
@@ -359520,26 +359350,26 @@
   offprint: false
   ean: 978-960-457-167-3
   original_entry:
     0: 7151
     1: HAMMOND,N.G.
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     3: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 355-346 Π.Χ.
+    4: 938.1HAM
     5: '9217'
     8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2007'
     11: 300Σ
     12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
     13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     14: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
     17: ΤΟΜΟΣ 6
     18: 978-960-45
     19: 7-167-3
-    4: null
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -359553,14 +359383,15 @@
     30: null
 - dbase_number: 7152
   authors:
   - HAMMOND,N.G.
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   subtitle: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 346-342 Π.Χ.
+  dewey: 938.1 HAM
   entry_numbers:
   - '9217'
   editor: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
   pages: 300
   topics:
   - ΙΣΤΟΡΙΑ ΜΑΚΕΔΟΝΙΑΣ
@@ -359572,26 +359403,26 @@
   offprint: false
   ean: 978-960-457-168-0
   original_entry:
     0: 7152
     1: HAMMOND,N.G.
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     3: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 346-342 Π.Χ.
+    4: 938.1HAM
     5: '9217'
     8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2007'
     11: 300Σ
     12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
     13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     14: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
     17: ΤΟΜΟΣ 7
     18: 978-960-45
     19: 7-168-0
-    4: null
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -359605,14 +359436,15 @@
     30: null
 - dbase_number: 7153
   authors:
   - HAMMOND,N.G.
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   subtitle: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 342-336 Π.Χ.
+  dewey: 938.1 HAM
   entry_numbers:
   - '9217'
   editor: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
   pages: 300
   topics:
   - ΙΣΤΟΡΙΑ ΜΑΚΕΔΟΝΙΑΣ
@@ -359624,26 +359456,26 @@
   offprint: false
   ean: 978-960-457-169-7
   original_entry:
     0: 7153
     1: HAMMOND,N.G.
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     3: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 342-336 Π.Χ.
+    4: 938.1HAM
     5: '9217'
     8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2007'
     11: 300Σ
     12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
     13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     14: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
     17: ΤΟΜΟΣ 8
     18: 978-960-45
     19: 7-169-7
-    4: null
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -359657,14 +359489,15 @@
     30: null
 - dbase_number: 7154
   authors:
   - HAMMOND,N.G.
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   subtitle: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 336-301 Π.Χ.
+  dewey: 938.1 HAM
   entry_numbers:
   - '9217'
   editor: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
   pages: 300
   topics:
   - ΙΣΤΟΡΙΑ ΜΑΚΕΔΟΝΙΑΣ
@@ -359676,26 +359509,26 @@
   offprint: false
   ean: 978-960-457-170-3
   original_entry:
     0: 7154
     1: HAMMOND,N.G.
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     3: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 336-301 Π.Χ.
+    4: 938.1HAM
     5: '9217'
     8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2007'
     11: 300Σ
     12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
     13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     14: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
     17: ΤΟΜΟΣ 9
     18: 978-960-45
     19: 7-170-3
-    4: null
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -359709,14 +359542,15 @@
     30: null
 - dbase_number: 7155
   authors:
   - HAMMOND,N.G.
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   subtitle: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 323-239 Π.Χ.
+  dewey: 938.1 HAM
   entry_numbers:
   - '9217'
   editor: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
   pages: 300
   topics:
   - ΙΣΤΟΡΙΑ ΜΑΚΕΔΟΝΙΑΣ
@@ -359728,26 +359562,26 @@
   offprint: false
   ean: 978-960-457-171-0
   original_entry:
     0: 7155
     1: HAMMOND,N.G.
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     3: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 323-239 Π.Χ.
+    4: 938.1HAM
     5: '9217'
     8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2007'
     11: 300Σ
     12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
     13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     14: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
     17: ΤΟΜΟΣ 10
     18: 978-960-45
     19: 7-171-0
-    4: null
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -359761,14 +359595,15 @@
     30: null
 - dbase_number: 7156
   authors:
   - HAMMOND,N.G.
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   subtitle: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 239-196 Π.Χ.
+  dewey: 938.1 HAM
   entry_numbers:
   - '9217'
   editor: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
   pages: 300
   topics:
   - ΙΣΤΟΡΙΑ ΜΑΚΕΔΟΝΙΑΣ
@@ -359780,26 +359615,26 @@
   offprint: false
   ean: 978-960-457-172-7
   original_entry:
     0: 7156
     1: HAMMOND,N.G.
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     3: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 239-196 Π.Χ.
+    4: 938.1HAM
     5: '9217'
     8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2007'
     11: 300Σ
     12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
     13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     14: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
     17: ΤΟΜΟΣ 11
     18: 978-960-45
     19: 7-172-7
-    4: null
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -359813,14 +359648,15 @@
     30: null
 - dbase_number: 7157
   authors:
   - HAMMOND,N.G.
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   subtitle: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 196-168 Π.Χ.
+  dewey: 938.1 HAM
   entry_numbers:
   - '9217'
   editor: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
   pages: 300
   topics:
   - ΙΣΤΟΡΙΑ ΜΑΚΕΔΟΝΙΑΣ
@@ -359832,26 +359668,26 @@
   offprint: false
   ean: 978-960-457-173-4
   original_entry:
     0: 7157
     1: HAMMOND,N.G.
     2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     3: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 196-168 Π.Χ.
+    4: 938.1HAM
     5: '9217'
     8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2007'
     11: 300Σ
     12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
     13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
     14: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
     17: ΤΟΜΟΣ 12
     18: 978-960-45
     19: 7-173-4
-    4: null
     6: null
     7: null
     15: null
     16: null
     20: null
     21: null
     22: null
@@ -359862,16 +359698,16 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7158
   authors:
   - HAMMOND,N.G.
-  language: el
-  title: ΦΙΛΙΠΠΟΣ Ο ΑΜΚΕΔΩΝ
+  title: ΦΙΛΙΠΠΟΣ Ο ΜAΚΕΔΩΝ
+  dewey: 938.1 HAM
   entry_numbers:
   - '9217'
   editor: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
   pages: 300
   topics:
   - ΦΙΛΙΠΠΟΣ Ο ΜΑΚΕΔΩΝ
@@ -359879,29 +359715,29 @@
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-457-121-5
   original_entry:
     0: 7158
     1: HAMMOND,N.G.
-    2: ΦΙΛΙΠΠΟΣ Ο ΑΜΚΕΔΩΝ
+    2: ΦΙΛΙΠΠΟΣ Ο ΜAΚΕΔΩΝ
+    4: 938.1HAM
     5: '9217'
     8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2007'
     11: 300Σ
     12: ΙΣΤΟΡΙΑ-ΦΙΛΙΠΠΟΣ Ο ΜΑΚΕΔΩΝ
     13: ΦΙΛΙΠΠΟΣ Ο ΜΑΚΕΔΩΝ-ΙΣΤΟΡΙΑ
     14: ΙΣΤΟΡΙΑ
     15: ΦΙΛΙΠΠΟΣ Ο ΜΑΚΕΔΩΝ
     17: ΠΑΡΑΡΤΗΜΑ Α
     18: 978-960-45
     19: 7-121-5
     3: null
-    4: null
     6: null
     7: null
     16: null
     20: null
     21: null
     22: null
     23: null
@@ -359914,14 +359750,15 @@
     30: null
 - dbase_number: 7159
   authors:
   - HAMMOND,N.G.
   language: el
   title: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   subtitle: ΕΝΑΣ ΙΔΙΟΦΥΗΣ
+  dewey: 938.070 HAM
   entry_numbers:
   - '9217'
   editor: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
   pages: 300
   topics:
   - ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
@@ -359931,27 +359768,27 @@
   offprint: false
   ean: 978-960-457-123-9
   original_entry:
     0: 7159
     1: HAMMOND,N.G.
     2: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     3: ΕΝΑΣ ΙΔΙΟΦΥΗΣ
+    4: 938.070HAM
     5: '9217'
     8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2007'
     11: 300Σ
     12: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     13: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ-ΙΣΤΟΡΙΑ
     14: ΙΣΤΟΡΙΑ
     15: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
     17: ΠΑΡΑΡΤΗΜΑ Β
     18: 978-960-45
     19: 7-123-9
-    4: null
     6: null
     7: null
     16: null
     20: null
     21: null
     22: null
     23: null
@@ -360315,15 +360152,15 @@
 - dbase_number: 7167
   authors:
   - ΠΙΛΤΣΕΡ,ΡΟΖΑΜΟΥΝΤ
   language: el
   title: ΤΟ ΕΡΗΜΟ ΣΠΙΤΙ
   dewey: 823 ΠΛΙ
   entry_numbers:
-  - 9166Α
+  - 09166
   translators:
   - ΚΟΥΜΠΑΡΕΛΗ,ΜΠΕΛΙΚΑ
   editor: ΩΚΕΑΝΙΔΑ // ΑΘΗΝΑ
   edition_year: 2000
   pages: 186
   topics:
   - ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -360333,15 +360170,15 @@
   offprint: false
   isbn: 960-410-132-3
   original_entry:
     0: 7167
     1: ΠΙΛΤΣΕΡ,ΡΟΖΑΜΟΥΝΤ
     2: ΤΟ ΕΡΗΜΟ ΣΠΙΤΙ
     4: 823ΠΛΙ
-    5: 9166Α
+    5: 09166
     6: ΜΠΕΛΙΚΑ ΚΟΥΜΠΑΡΕΛΗ
     8: ΩΚΕΑΝΙΔΑ
     9: ΑΘΗΝΑ
     10: '2000'
     11: 186Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -360517,14 +360354,15 @@
     29: null
     30: null
 - dbase_number: 7171
   authors:
   - ΒΑΣΙΛΙΚΟΣ,ΒΑΣΙΛΗΣ
   language: el
   title: ΤΟ ΤΕΛΕΥΤΑΙΟ ΑΝΤΙΟ
+  dewey: 889.21 ΒΑΣ
   entry_numbers:
   - '9248'
   editor: ΝΕΑ ΣΥΝΟΡΑ // ΑΘΗΝΑ
   edition_year: 1994
   pages: 165
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -360533,27 +360371,27 @@
   has_dvd: false
   offprint: false
   isbn: 960-236-429-7
   original_entry:
     0: 7171
     1: ΒΑΣΙΛΙΚΟΣ,ΒΑΣΙΛΗΣ
     2: ΤΟ ΤΕΛΕΥΤΑΙΟ ΑΝΤΙΟ
+    4: 889.21ΒΑΣ
     5: '9248'
     8: ΝΕΑ ΣΥΝΟΡΑ
     9: ΑΘΗΝΑ
     10: '1994'
     11: 165Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     15: ΜΥΘΙΣΤΟΡΗΜΑ
     18: 960-236-42
     19: 9-7
     3: null
-    4: null
     6: null
     7: null
     16: null
     17: null
     20: null
     21: null
     22: null
@@ -360673,14 +360511,15 @@
     29: null
     30: null
 - dbase_number: 7174
   authors:
   - ΣΑΡΤΡ
   language: el
   title: Η ΑΝΑΣΤΟΛΗ
+  dewey: 843 ΣΑΡ
   entry_numbers:
   - '9249'
   translators:
   - ΧΟΥΡΜΟΥΖΙΟΥ,ΑΙΜ.
   editor: ΑΡΣΕΝΙΔΗΣ // ΑΘΗΝΑ
   pages: 559
   topics:
@@ -360689,25 +360528,25 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7174
     1: ΣΑΡΤΡ
     2: Η ΑΝΑΣΤΟΛΗ
+    4: 843ΣΑΡ
     5: '9249'
     6: ΑΙΜ.ΧΟΥΡΜΟΥΖΙΟΥ
     8: ΑΡΣΕΝΙΔΗΣ
     9: ΑΘΗΝΑ
     11: 559Σ
     12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
     15: ΜΥΘΙΣΤΟΡΗΜΑ
     3: null
-    4: null
     7: null
     10: null
     16: null
     17: null
     18: null
     19: null
     20: null
@@ -360982,30 +360821,30 @@
 - dbase_number: 7180
   authors:
   - ΑΙΣΩΠΟΣ
   language: el
   title: 135 ΜΥΘΟΙ ΤΟΥ ΑΙΣΩΠΟΥ
   dewey: 808.899 AIΣ
   entry_numbers:
-  - 9198Α
+  - 09198
   editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
   edition_year: 2007
   pages: 330
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-422-543-9
   original_entry:
     0: 7180
     1: ΑΙΣΩΠΟΣ
     2: 135 ΜΥΘΟΙ ΤΟΥ ΑΙΣΩΠΟΥ
     4: 808.899AIΣ
-    5: 9198A
+    5: 09198
     8: ΑΓΚΥΡΑ
     9: ΑΘΗΝΑ
     10: '2007'
     11: 330Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -361207,15 +361046,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 7184
     1: ΜΠΛΟΚ,ΛΟΡΕΝΣ
     2: Ο ΔΙΑΡΡΗΚΤΗΣ ΠΟΥ ΖΩΓΡΑΦΙΖΕ ΣΑΝ ΤΟΝ ΜΟΝΤΡΙΑΝ
     4: 810.11ΜΠΛ
-    5: 9230,12492,20617
+    5: 9230-12492-20617
     6: ΚΑΤΕΡΙΝΑ ΡΟΝΤΟΓΙΑΝΝΗ
     8: ΜΟΝΤΕΡΝΟΙ ΚΑΙΡΟΙ
     9: ΑΘΗΝΑ
     10: '2004'
     11: 349Σ
     12: ΒΙΠΕΡ-ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΣΤΥΝΟΜΙΚΟ
     13: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΣΤΥΝΟΜΙΚΟ-ΒΙΠΕΡ
@@ -361546,41 +361385,43 @@
     29: null
     30: null
 - dbase_number: 7191
   authors:
   - ΖΟΛΑ,ΕΜΙΛ
   language: el
   title: ΝΑΝΑ
-  entry_numbers: []
+  dewey: 843 ΖΟΛ
+  entry_numbers:
+  - '9260'
   translators:
   - ΠΡΑΤΣΙΚΑΣ,ΓΙΩΡΓΟΣ
   editor: ΓΚΟΒΟΣΤΗΣ // ΑΘΗΝΑ
   pages: 536
   topics:
   - ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   isbn: 960-270-634-1
   original_entry:
     0: 7191
     1: ΖΟΛΑ,ΕΜΙΛ
     2: ΝΑΝΑ
+    4: 843ΖΟΛ
+    5: '9260'
     6: ΓΙΩΡΓΟΣ ΠΡΑΤΣΙΚΑΣ
     8: ΓΚΟΒΟΣΤΗΣ
     9: ΑΘΗΝΑ
     11: 536Σ
     12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
     18: 960-270-63
     19: 4-1
     3: null
-    4: null
-    5: null
     7: null
     10: null
     15: null
     16: null
     17: null
     20: null
     21: null
@@ -361715,15 +361556,15 @@
   has_dvd: false
   offprint: false
   ean: 978-88-8371-279-1
   original_entry:
     0: 7194
     1: ΓΟΥΛΦ,ΒΙΡΤΖΙΝΙΑ
     2: ΜΕΧΡΙ ΤΟ ΦΑΡΟ
-    4: 823 ΓΟΥ
+    4: 823ΓΟΥ
     5: '9221'
     6: ΕΛΛΗ ΜΑΡΜΑΡΑ
     8: ΤΟ ΒΗΜΑ
     9: ΑΘΗΝΑ
     10: '2007'
     11: 219Σ
     12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
@@ -363912,15 +363753,15 @@
   authors:
   - ΣΚΟΥΤΕΛΑΣ,ΠΕΤΡΟΣ
   language: el
   title: ΑΠΟ ΤΑ ΑΓΡΙΜΙΑ ΚΙ ΑΓΡΙΟΠΟΥΛΙΑ ΤΩΝ ΒΟΥΝΩΝ ΜΑΣ
   subtitle: ΚΑΙ Η ΛΑΙΚΗ ΜΑΣ ΠΑΡΑΔΟΣΗ
   dewey: 398 ΣΚΟ
   entry_numbers:
-  - 9145Α
+  - 09145
   - '9644'
   editor: None // ΑΘΗΝΑ
   edition_year: 2008
   pages: 148
   topics:
   - ΛΑΟΓΡΑΦΙΑ
   copies: 4
@@ -363929,15 +363770,15 @@
   offprint: false
   original_entry:
     0: 7238
     1: ΣΚΟΥΤΕΛΑΣ,ΠΕΤΡΟΣ
     2: ΑΠΟ ΤΑ ΑΓΡΙΜΙΑ ΚΙ ΑΓΡΙΟΠΟΥΛΙΑ ΤΩΝ ΒΟΥΝΩΝ ΜΑΣ
     3: ΚΑΙ Η ΛΑΙΚΗ ΜΑΣ ΠΑΡΑΔΟΣΗ
     4: 398ΣΚΟ
-    5: 9145Α-9644
+    5: 09145-9644
     9: ΑΘΗΝΑ
     10: '2008'
     11: 148Σ
     12: ΛΑΟΓΡΑΦΙΑ
     13: ΛΑΟΓΡΑΦΙΑ
     14: ΛΑΟΓΡΑΦΙΑ
     17: 4 ΑΝΤΙΤΥΠΑ
@@ -363957,15 +363798,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7239
   authors:
-  - ΑΠΟΣΤΟΛΙΔΗΣ,ΡΕΝΟΣ
+  - ΑΠΟΣΤΟΛΙΔΗΣ,ΡΕΝΟΣ,ΗΡΑΚΛΗΣ
   language: el
   title: ΠΥΡΑΜΙΔΑ 67
   subtitle: ΤΟ ΒΙΒΛΙΟ ΤΟΥ ΕΜΦΥΛΙΟΥ
   dewey: 938.764 ΑΠΟ
   entry_numbers:
   - '9173'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
@@ -364605,15 +364446,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7252
   authors:
-  - ΑΡΒΑΝΙΤΗΣ ΝΙΚΟΣ
+  - ΑΡΒΑΝΙΤΗΣ,ΝΙΚΟΣ
   language: el
   title: ΑΠΟ ΤΟ ΒΟΛΓΑ ΣΤΗ ΜΕΣΟΓΕΙΟ
   dewey: 808.899 ΑΡΒ
   entry_numbers:
   - '10411'
   editor: ΔΑΜΑΣΚΟΣ // ΑΘΗΝΑ
   edition_year: 1983
@@ -365095,35 +364936,35 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7262
   authors:
-  - ΑΘΑΝΑΣΑΚΗ,ΑΝΤΩΝΙΟΥ
+  - ΑΘΑΝΑΣΑΚΗΣ,ΑΝΤΩΝΗΣ,ΝΙΚΟΛΑΟΥ
   language: el
   title: ΤΟ ΑΣΤΡΟΧΩΡΙ ΑΡΤΑΣ
-  dewey: '938.939'
+  dewey: 938.939 ΑΘΑ
   entry_numbers:
-  - 9215Α
+  - 09215
   - '9215'
   editor: NEW TYPE // ΑΡΤΑ
   edition_year: 2000
   pages: 396
   topics:
   - ΑΣΤΡΟΧΩΡΙ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7262
     1: ΑΘΑΝΑΣΑΚΗ,ΑΝΤΩΝΙΟΥ
     2: ΤΟ ΑΣΤΡΟΧΩΡΙ ΑΡΤΑΣ
-    4: '938.939'
-    5: 9215Α
+    4: 938.939ΑΘΑ
+    5: 09215
     6: '9215'
     8: NEW TYPE
     9: ΑΡΤΑ
     10: '2000'
     11: 396Σ
     12: ΑΣΤΡΟΧΩΡΙ
     13: ΑΣΤΡΟΧΩΡΙ
@@ -365198,29 +365039,29 @@
 - dbase_number: 7264
   authors:
   - ΜΠΟΚΟΓΙΑΝΝΗΣ,ΧΡΥΣΟΣΤΟΜΟΣ
   language: el
   title: ΟΙ ΡΙΖΕΣ ΜΑΣ
   dewey: 398 ΜΠΟ
   entry_numbers:
-  - 9225Α
+  - 09225
   editor: None // ΑΡΤΑ
   edition_year: 2008
   pages: 71
   topics:
   - ΛΑΟΓΡΑΦΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7264
     1: ΜΠΟΚΟΓΙΑΝΝΗΣ,ΧΡΥΣΟΣΤΟΜΟΣ
     2: ΟΙ ΡΙΖΕΣ ΜΑΣ
-    4: 398 ΜΠΟ
-    5: 9225Α
+    4: 398ΜΠΟ
+    5: 09225
     9: ΑΡΤΑ
     10: '2008'
     11: 71Σ
     12: ΛΑΟΓΡΑΦΙΑ
     13: ΛΑΟΓΡΑΦΙΑ
     14: ΛΑΟΓΡΑΦΙΑ
     3: null
@@ -366584,15 +366425,15 @@
 - dbase_number: 7292
   authors:
   - ΧΑΤΖΗΜΙΧΑΛΗ,ΑΓΓΕΛΙΚΗ
   language: el
   title: Η ΕΛΛΗΝΙΚΗ ΛΑΙΚΗ ΦΟΡΕΣΙΑ
   dewey: 398 ΧΑΤ
   entry_numbers:
-  - 9133Α
+  - 09133
   editor: ΜΕΛΙΣΣΑ // ΑΘΗΝΑ
   edition_year: 1983
   pages: 464
   topics:
   - ΛΑΙΚΗ ΦΟΡΕΣΙΑ
   - ΛΑΟΓΡΑΦΙΑ
   - ΕΛΛΗΝΙΚΗ ΛΑΙΚΗ ΦΟΡΕΣΙΑ
@@ -366600,16 +366441,16 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7292
     1: ΧΑΤΖΗΜΙΧΑΛΗ,ΑΓΓΕΛΙΚΗ
     2: Η ΕΛΛΗΝΙΚΗ ΛΑΙΚΗ ΦΟΡΕΣΙΑ
-    4: 398 ΧΑΤ
-    5: 9133Α
+    4: 398ΧΑΤ
+    5: 09133
     8: ΜΕΛΙΣΣΑ
     9: ΑΘΗΝΑ
     10: '1983'
     11: 464Σ
     12: ΛΑΙΚΗ ΦΟΡΕΣΙΑ-ΛΑΟΓΡΑΦΙΑ
     13: ΛΑΟΓΡΑΦΙΑ-ΛΑΙΚΗ ΦΟΡΕΣΙΑ
     14: ΕΛΛΗΝΙΚΗ ΛΑΙΚΗ ΦΟΡΕΣΙΑ
@@ -366727,15 +366568,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7295
   authors:
-  - ΒΑΣΙΛΕΙΟΥ,ΣΩΚΡΑΤΗ
+  - ΒΑΣΙΛΕΙΟΥ,ΣΩΚΡΑΤΗΣ,Σ.
   language: el
   title: ΓΥΝΑΙΚΕΣ ΗΠΕΙΡΩΤΙΣΣΕΣ
   subtitle: ΞΑΦΝΙΑΣΜΑΤΑ ΤΗΣ ΦΥΣΗΣ
   entry_numbers:
   - '9290'
   editor: ΚΕΝΤΡΟ ΕΡΕΥΝΑΣ ΙΣΟΤΗ // ΑΘΗΝΑ
   edition_year: 2005
@@ -367982,15 +367823,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7320
     1: ΠΑΠΠΑΣ,ΑΝΔΡΕΑΣ
     2: ΑΠ ΤΗΝ ΟΨΗ ΤΗΣ ΠΑΤΡΙΔΑΣ
-    4: 398 ΠΑΠ
+    4: 398ΠΑΠ
     5: '9296'
     9: ΚΑΛΕΝΤΙΝΗ
     10: '2005'
     11: 130Σ
     12: ΔΙΗΓΗΜΑΤΑ
     13: ΔΙΗΓΗΜΑΤΑ
     14: ΔΙΗΓΗΜΑΤΑ
@@ -368030,15 +367871,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7321
     1: ΠΑΠΠΑΣ,ΑΝΔΡΕΑΣ
     2: Ο ΘΡΥΛΟΣ ΤΗΣ ΓΚΟΛΦΩΣ
-    4: 398 ΠΑΠ
+    4: 398ΠΑΠ
     5: '9295'
     9: ΚΑΛΕΝΤΙΝΗ
     10: '2004'
     11: 144Σ
     12: ΔΙΗΓΗΜΑΤΑ
     13: ΔΙΗΓΗΜΑΤΑ
     14: ΔΙΗΓΗΜΑΤΑ
@@ -368207,33 +368048,34 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7325
   authors: []
   language: el
-  title: ΑΓΡΙΑ  ΛΟΥΛΟΥΔΙΑ
+  title: ΑΓΡΙΑ ΛΟΥΛΟΥΔΙΑ
   subtitle: Η ΕΚΘΑΜΒΩΤΙΚΗ ΕΛΛΗΝΙΚΗ ΧΛΩΡΙΔΑ ΜΕ ΤΟ ΦΑΚΟ ΤΟΥ ΓΙΩΡΓΟΥ ΑΒΑΓΙΑ
+  dewey: 582.13 ΧΣ
   entry_numbers:
   - '9385'
   editor: EXPLORE NATURE // None
   pages: 170
   topics:
   - ΑΓΡΙΑ ΛΟΥΛΟΥΔΙΑ
   - ΛΟΥΛΟΥΔΙΑ
   - ΥΠΕΡΟΧΗ ΕΛΛΑΔΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7325
     1: Χ.Σ.
-    2: ΑΓΡΙΑ  ΛΟΥΛΟΥΔΙΑ
+    2: ΑΓΡΙΑ ΛΟΥΛΟΥΔΙΑ
     3: Η ΕΚΘΑΜΒΩΤΙΚΗ ΕΛΛΗΝΙΚΗ ΧΛΩΡΙΔΑ ΜΕ ΤΟ ΦΑΚΟ ΤΟΥ ΓΙΩΡΓΟΥ ΑΒΑΓΙΑ
-    4: ΝΟΥ
+    4: 582.13Χ.Σ
     5: '9385'
     8: EXPLORE NATURE
     11: '170'
     12: ΑΓΡΙΑ ΛΟΥΛΟΥΔΙΑ
     13: ΛΟΥΛΟΥΔΙΑ
     14: ΥΠΕΡΟΧΗ ΕΛΛΑΔΑ
     6: null
@@ -368304,15 +368146,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7327
   authors:
-  - ΒΑΛΜΑ,ΣΤΑΜΑΤΗ
+  - ΒΑΛΜΑΣ,ΣΤΑΜΑΤΗΣ
   language: el
   title: 12 ΚΕΡΑΚΙΑ ΓΙΑ ΝΑ ΜΗΝ ΑΡΡΩΣΤΟΥΝ ΠΑΤΡΙΩΤΑΚΙΑ
   subtitle: ΕΜΠΕΙΡΙΕΣ ΜΙΑΣ ΦΙΛΕΡΕΥΝΗΣ ΠΥΞΙΔΑΣ
   dewey: 578.7 ΒΑΛ
   entry_numbers:
   - '9155'
   editor: None // ΑΘΗΝΑ
@@ -368353,15 +368195,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7328
   authors:
-  - ΒΑΛΜΑ,ΣΤΑΜΑΤΗ
+  - ΒΑΛΜΑΣ,ΣΤΑΜΑΤΗΣ
   language: el
   title: ΚΥΝΗΓΩΝΤΑΣ ΤΗΝ ΥΓΕΙΑ ΝΟ 2
   subtitle: ΘΕΡΑΠΕΙΕΣ
   dewey: 578.7 ΒΑΛ
   entry_numbers:
   - '9390'
   editor: None // ΑΘΗΝΑ
@@ -368407,15 +368249,15 @@
 - dbase_number: 7329
   authors:
   - ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   language: el
   title: ΕΥΘΑΛΗΣ ΚΛΩΝΟΣ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
-  - 9245Α
+  - 09245
   editor: UNIVERSITY STUDIO PR // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2001
   pages: 88
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   has_cd: false
@@ -368423,15 +368265,15 @@
   offprint: false
   isbn: 960-12-0950-6
   original_entry:
     0: 7329
     1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
     2: ΕΥΘΑΛΗΣ ΚΛΩΝΟΣ
     4: 889.1ΜΠΟ
-    5: 9245Α
+    5: 09245
     8: UNIVERSITY STUDIO PR
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2001'
     11: 88Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -368457,15 +368299,15 @@
 - dbase_number: 7330
   authors:
   - ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   language: el
   title: ΕΛΙΞ ΤΗΣ ΓΑΛΑΞΙΑΚΗΣ ΔΟΜΗΣ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
-  - 9241Α
+  - 09241
   editor: UNIVERSITY STUDIO PR // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1998
   pages: 62
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   has_cd: false
@@ -368473,15 +368315,15 @@
   offprint: false
   isbn: 960-12-0710-4
   original_entry:
     0: 7330
     1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
     2: ΕΛΙΞ ΤΗΣ ΓΑΛΑΞΙΑΚΗΣ ΔΟΜΗΣ
     4: 889.1ΜΠΟ
-    5: 9241Α
+    5: 09241
     8: UNIVERSITY STUDIO PR
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '1998'
     11: 62Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -368507,15 +368349,15 @@
 - dbase_number: 7331
   authors:
   - ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   language: el
   title: ΡΙΖΑ ΑΠΟ ΑΛΜΗ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
-  - 9244Α
+  - 09244
   editor: UNIVERSITY STUDIO PR // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2001
   pages: 51
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   has_cd: false
@@ -368523,15 +368365,15 @@
   offprint: false
   isbn: 960-12-0948-4
   original_entry:
     0: 7331
     1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
     2: ΡΙΖΑ ΑΠΟ ΑΛΜΗ
     4: 889.1ΜΠΟ
-    5: 9244Α
+    5: 09244
     8: UNIVERSITY STUDIO PR
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2001'
     11: 51Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -368557,30 +368399,30 @@
 - dbase_number: 7332
   authors:
   - ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   language: el
   title: Η ΝΥΧΤΑ ΤΗΣ ΑΥΓΗΣ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
-  - 9243Α
+  - 09243
   editor: UNIVERSITY STUDIO PR // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2001
   pages: 59
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7332
     1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
     2: Η ΝΥΧΤΑ ΤΗΣ ΑΥΓΗΣ
     4: 889.1ΜΠΟ
-    5: 9243Α
+    5: 09243
     8: UNIVERSITY STUDIO PR
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2001'
     11: 59Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -368606,15 +368448,15 @@
 - dbase_number: 7333
   authors:
   - ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   language: el
   title: ΦΩΤΟΣΥΝΘΕΣΗ-ΦΩΤΟΔΙΑΧΥΣΗ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
-  - 9242Α
+  - 09242
   editor: UNIVERSITY STUDIO PR // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2001
   pages: 50
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   has_cd: false
@@ -368622,15 +368464,15 @@
   offprint: false
   isbn: 960-12-0941-7
   original_entry:
     0: 7333
     1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
     2: ΦΩΤΟΣΥΝΘΕΣΗ-ΦΩΤΟΔΙΑΧΥΣΗ
     4: 889.1ΜΠΟ
-    5: 9242Α
+    5: 09242
     8: UNIVERSITY STUDIO PR
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2001'
     11: 50Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -368656,15 +368498,15 @@
 - dbase_number: 7334
   authors:
   - ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   language: el
   title: ΑΝΑΖΗΤΩΝΤΑΣ ΤΟ ΑΠΟΛΥΤΟ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
-  - 9232Α
+  - 09232
   editor: UNIVERSITY STUDIO PR // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
   pages: 209
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   has_cd: false
@@ -368672,15 +368514,15 @@
   offprint: false
   ean: 978-960-12-1659-1
   original_entry:
     0: 7334
     1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
     2: ΑΝΑΖΗΤΩΝΤΑΣ ΤΟ ΑΠΟΛΥΤΟ
     4: 889.1ΜΠΟ
-    5: 9232Α
+    5: 09232
     8: UNIVERSITY STUDIO PR
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2007'
     11: 209Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -368706,15 +368548,15 @@
 - dbase_number: 7335
   authors:
   - ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   language: el
   title: ΔΙΑΥΛΟΣ ΖΩΗΣ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
-  - 9234Α
+  - 09234
   editor: UNIVERSITY STUDIO PR // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2001
   pages: 83
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   has_cd: false
@@ -368722,15 +368564,15 @@
   offprint: false
   isbn: 960-12-0947-6
   original_entry:
     0: 7335
     1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
     2: ΔΙΑΥΛΟΣ ΖΩΗΣ
     4: 889.1ΜΠΟ
-    5: 9234Α
+    5: 09234
     8: UNIVERSITY STUDIO PR
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2001'
     11: 83Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -368756,15 +368598,15 @@
 - dbase_number: 7336
   authors:
   - ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   language: el
   title: ΒΟΜΒΑ ΥΔΡΟΓΟΝΟΥ ΤΗΣ ΕΛΕΥΘΕΡΙΑΣ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
-  - 9230Β
+  - 09230
   editor: UNIVERSITY STUDIO PR // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1998
   pages: 77
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   has_cd: false
@@ -368772,15 +368614,15 @@
   offprint: false
   isbn: 960-12-0712-0
   original_entry:
     0: 7336
     1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
     2: ΒΟΜΒΑ ΥΔΡΟΓΟΝΟΥ ΤΗΣ ΕΛΕΥΘΕΡΙΑΣ
     4: 889.1ΜΠΟ
-    5: 9230Β
+    5: 09230
     8: UNIVERSITY STUDIO PR
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '1998'
     11: 77Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -368806,15 +368648,15 @@
 - dbase_number: 7337
   authors:
   - ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   language: el
   title: ΣΚΟΤΩΜΕΝΟ ΑΙΜΑ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
-  - 9231Β
+  - 09231
   editor: UNIVERSITY STUDIO PR // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1998
   pages: 102
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   has_cd: false
@@ -368822,15 +368664,15 @@
   offprint: false
   isbn: 960-12-0711-2
   original_entry:
     0: 7337
     1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
     2: ΣΚΟΤΩΜΕΝΟ ΑΙΜΑ
     4: 889.1.ΜΠΟ
-    5: 9231Β
+    5: 09231
     8: UNIVERSITY STUDIO PR
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '1998'
     11: 102Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -368856,15 +368698,15 @@
 - dbase_number: 7338
   authors:
   - ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   language: el
   title: ΗΛΙΟΣ ΠΟΥ ΑΠΟ ΤΗ ΓΗ ΦΩΤΑ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
-  - 9237Α
+  - 09237
   editor: UNIVERSITY STUDIO PR // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2001
   pages: 102
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   has_cd: false
@@ -368872,15 +368714,15 @@
   offprint: false
   isbn: 960-12-0939-5
   original_entry:
     0: 7338
     1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
     2: ΗΛΙΟΣ ΠΟΥ ΑΠΟ ΤΗ ΓΗ ΦΩΤΑ
     4: 889.1ΜΠΟ
-    5: 9237Α
+    5: 09237
     8: UNIVERSITY STUDIO PR
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2001'
     11: 102Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
@@ -368906,15 +368748,15 @@
 - dbase_number: 7339
   authors:
   - ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   language: el
   title: ΠΑΝΘΕΟΝ-ΕΠΙΤΑΞΙΣ-ΝΤΟΜΙΝΟ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
-  - 9236Α
+  - 09236
   editor: UNIVERSITY STUDIO PR // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2003
   pages: 206
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   has_cd: false
@@ -368922,15 +368764,15 @@
   offprint: false
   isbn: 960-91636-6-1
   original_entry:
     0: 7339
     1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
     2: ΠΑΝΘΕΟΝ-ΕΠΙΤΑΞΙΣ-ΝΤΟΜΙΝΟ
     4: 889.1ΜΠΟ
-    5: 9236Α
+    5: 09236
     8: UNIVERSITY STUDIO PR
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2003'
     11: 206Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -368956,15 +368798,15 @@
 - dbase_number: 7340
   authors:
   - ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   language: el
   title: ΓΑΛΑΖΙΟ ΠΑΡΑΘΥΡΟ ΘΕΣΦΑΤΑ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
-  - 9235Α
+  - 09235
   editor: Α.Α.ΑΛΤΙΝΤΖΗΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2003
   pages: 188
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   has_cd: false
@@ -368972,15 +368814,15 @@
   offprint: false
   isbn: 960-91636-5-3
   original_entry:
     0: 7340
     1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
     2: ΓΑΛΑΖΙΟ ΠΑΡΑΘΥΡΟ ΘΕΣΦΑΤΑ
     4: 889.1ΜΠΟ
-    5: 9235Α
+    5: 09235
     8: Α.Α.ΑΛΤΙΝΤΖΗΣ
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2003'
     11: 188Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -369006,15 +368848,15 @@
 - dbase_number: 7341
   authors:
   - ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   language: el
   title: ΝΕΑ ΓΗ-ΝΙΚΗ ΖΩΗΣ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
-  - 9233Α
+  - 09233
   editor: UNUIVERSITY STUDIO P // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
   pages: 147
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   has_cd: false
@@ -369022,15 +368864,15 @@
   offprint: false
   ean: 978-960-12-1658-4
   original_entry:
     0: 7341
     1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
     2: ΝΕΑ ΓΗ-ΝΙΚΗ ΖΩΗΣ
     4: 889.1ΜΠΟ
-    5: 9233Α
+    5: 09233
     8: UNUIVERSITY STUDIO P
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2007'
     11: 147Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -369056,15 +368898,15 @@
 - dbase_number: 7342
   authors:
   - ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   language: el
   title: ΔΕΚΑ ΚΑΙ ΟΚΤΩ ΚΥΚΛΟΙ ΕΚΛΕΙΣΑΝ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
-  - 9240Α
+  - 09240
   editor: UNIVERSITY STUDIO PR // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2001
   pages: 55
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   has_cd: false
@@ -369072,15 +368914,15 @@
   offprint: false
   isbn: 960-12-0942-5
   original_entry:
     0: 7342
     1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
     2: ΔΕΚΑ ΚΑΙ ΟΚΤΩ ΚΥΚΛΟΙ ΕΚΛΕΙΣΑΝ
     4: 889.1ΜΠΟ
-    5: 9240Α
+    5: 09240
     8: UNIVERSITY STUDIO PR
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2001'
     11: 55Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -369106,15 +368948,15 @@
 - dbase_number: 7343
   authors:
   - ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   language: el
   title: ΚΡΥΣΤΑΛΛΩΣΙΣ ΚΡΑΔΑΣΜΩΝ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
-  - 9239Α
+  - 09239
   editor: UNIVERSITY STUDIO PR // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2001
   pages: 65
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   has_cd: false
@@ -369122,15 +368964,15 @@
   offprint: false
   isbn: 960-12-0944-1
   original_entry:
     0: 7343
     1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
     2: ΚΡΥΣΤΑΛΛΩΣΙΣ ΚΡΑΔΑΣΜΩΝ
     4: 889.1ΜΠΟ
-    5: 9239Α
+    5: 09239
     8: UNIVERSITY STUDIO PR
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '2001'
     11: 65Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -369156,15 +368998,15 @@
 - dbase_number: 7344
   authors:
   - ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   language: el
   title: ΡΑΔΙΕΝΕΡΓΕΙΑ
   dewey: 889.1 ΜΠΟ
   entry_numbers:
-  - 9238Α
+  - 09238
   editor: UNIVERSITY STUDIO PR // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1998
   pages: 54
   topics:
   - ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   - ΠΟΙΗΜΑΤΑ
   has_cd: false
@@ -369172,15 +369014,15 @@
   offprint: false
   isbn: 960-12-0709-0
   original_entry:
     0: 7344
     1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
     2: ΡΑΔΙΕΝΕΡΓΕΙΑ
     4: 889.1ΜΠΟ
-    5: 9238Α
+    5: 09238
     8: UNIVERSITY STUDIO PR
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '1998'
     11: 54Σ
     12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
     13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
     14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -369609,35 +369451,36 @@
     30: null
 - dbase_number: 7353
   authors:
   - ΜΑΡΕΣ,ΝΤΕΛΙΑ
   language: el
   title: ΓΝΩΡΙΣΤΕ ΤΟΝ ΚΟΜΜΟΥΝΙΣΜΟ
   dewey: 335.430 ΜΑΡ
-  entry_numbers: []
+  entry_numbers:
+  - '9437'
   pages: 92
   topics:
   - ΚΟΜΜΟΥΝΙΣΜΟΣ
   - ΜΑΡΞ
   - ΛΕΝΙΝ
   - ΣΤΑΛΙΝ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7353
     1: ΜΑΡΕΣ,ΝΤΕΛΙΑ
     2: ΓΝΩΡΙΣΤΕ ΤΟΝ ΚΟΜΜΟΥΝΙΣΜΟ
     4: 335.430ΜΑΡ
+    5: '9437'
     11: 92Σ
     12: ΚΟΜΜΟΥΝΙΣΜΟΣ
     13: ΜΑΡΞ-ΛΕΝΙΝ-ΣΤΑΛΙΝ
     14: ΚΟΥΜΜΟΥΝΙΣΜΟΣ
     3: null
-    5: null
     6: null
     7: null
     8: null
     9: null
     10: null
     15: null
     16: null
@@ -369754,30 +369597,30 @@
 - dbase_number: 7356
   authors:
   - ΣΕΒΑΣΤΙΑΝΟΥ
   language: el
   title: Η ΕΣΤΑΥΡΩΜΕΝΗ ΗΠΕΙΡΟΣ
   dewey: 938.936 ΣΕΒ
   entry_numbers:
-  - 9285Α
   - '8422'
+  - 09285
   editor: None // ΑΘΗΝΑ
   edition_year: 1985
   pages: 189
   topics:
   - ΒΟΡΕΙΑ ΗΠΕΙΡΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7356
     1: ΣΕΒΑΣΤΙΑΝΟΥ
     2: Η ΕΣΤΑΥΡΩΜΕΝΗ ΗΠΕΙΡΟΣ
     4: 938.936ΣΕΒ
-    5: 9285Α-8422
+    5: 8422-09285
     9: ΑΘΗΝΑ
     10: '1985'
     11: 189Σ
     12: ΒΟΡΕΙΟΣ ΗΠΕΙΡΟΣ
     13: ΒΟΡΕΙΟΣ ΗΠΕΙΡΟΣ
     14: ΒΟΡΕΙΟΣ ΗΠΕΙΡΟΣ
     3: null
@@ -369849,15 +369692,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7358
   authors:
-  - ΒΑΛΑΩΡΙΤΗΣ ΝΑΝΟΣ
+  - ΒΑΛΑΩΡΙΤΗΣ,ΝΑΝΟΣ
   language: el
   title: ΜΟΝΤΕΡΝΙΣΜΟΣ, ΠΡΩΤΟΠΟΡΙΑ ΚΑΙ ΠΑΛΙ
   dewey: 889.21 ΒΑΛ
   entry_numbers:
   - '6853'
   editor: ΚΑΣΤΑΝΙΩΤΗ // ΑΘΗΝΑ
   edition_year: 1997
@@ -369948,15 +369791,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7360
   authors:
-  - ΑΠΟΣΤΟΛΟΠΟΥΛΟΥ-ΧΑΤΖΗΑΝΤΩΝΙΟΥ
+  - ΑΠΟΣΤΟΛΟΠΟΥΛΟΣ,Μ.
+  - ΧΑΤΖΗΑΝΤΩΝΙΟΥ,ΚΩΣΤΑΣ
   language: el
   title: ΙΣΤΟΡΙΑ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΕΘΝΟΥΣ 1821-1941
   dewey: 949.507 ΑΠΟ
   entry_numbers:
   - '9306'
   editor: ΠΕΛΕΚΑΝΟΣ // ΑΘΗΝΑ
   pages: 384
@@ -370101,15 +369945,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7363
   authors:
-  - ΑΝΔΡΕΑΔΗ,ΓΕΩΡΓΙΟΥ
+  - ΑΝΔΡΕΑΔΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: Ο ΠΟΛΙΤΙΣΜΟΣ ΤΟΥ ΠΟΝΤΟΥ
   dewey: 938.3 ΑΝΔ
   entry_numbers:
   - '9382'
   editor: None // ΑΘΗΝΑ
   edition_year: 1964
@@ -371887,15 +371731,15 @@
   authors:
   - ΚΑΡΖΗ,ΘΟΔΩΡΟΥ
   language: el
   title: ΟΙ ΠΑΤΡΙΔΕΣ ΤΩΝ ΕΛΛΗΝΩΝ
   subtitle: ΜΙΚΡΑ ΑΣΙΑ-ΠΟΝΤΟΣ
   dewey: 938.393 ΚΑΡ
   entry_numbers:
-  - 9292Α
+  - 09292
   editor: ΛΙΒΑΝΗ // ΑΘΗΝΑ
   edition_year: 2002
   pages: 147
   topics:
   - ΜΙΚΡΑ ΑΣΙΑ
   - ΠΟΝΤΟΣ
   volume: ΤΟΜΟΣ Α
@@ -371905,15 +371749,15 @@
   isbn: 960-14-0453-8
   original_entry:
     0: 7399
     1: ΚΑΡΖΗ,ΘΟΔΩΡΟΥ
     2: ΟΙ ΠΑΤΡΙΔΕΣ ΤΩΝ ΕΛΛΗΝΩΝ
     3: ΜΙΚΡΑ ΑΣΙΑ-ΠΟΝΤΟΣ
     4: 938.393ΚΑΡ
-    5: 9292Α
+    5: 09292
     8: ΛΙΒΑΝΗ
     9: ΑΘΗΝΑ
     10: '2002'
     11: 147Σ
     12: ΙΣΤΟΡΙΑ-Μ.ΑΣΙΑ-ΠΟΝΤΟΣ
     13: Μ.ΑΣΙΑ-ΠΟΝΤΟΣ
     14: ΠΟΝΤΟΣ-Μ,ΑΣΙΑ
@@ -371939,15 +371783,15 @@
   authors:
   - ΚΑΡΖΗ,ΘΟΔΩΡΟΥ
   language: el
   title: ΟΙ ΠΑΤΡΙΔΕΣ ΤΩΝ ΕΛΛΗΝΩΝ
   subtitle: ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ
   dewey: 938.393 ΚΑΡ
   entry_numbers:
-  - 9292Α
+  - 09292
   editor: ΛΙΒΑΝΗ // ΑΘΗΝΑ
   edition_year: 2002
   pages: 254
   topics:
   - ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ
   volume: ΤΟΜΟΣ Β
   has_cd: false
@@ -371956,15 +371800,15 @@
   isbn: 960-14-0453-8
   original_entry:
     0: 7400
     1: ΚΑΡΖΗ,ΘΟΔΩΡΟΥ
     2: ΟΙ ΠΑΤΡΙΔΕΣ ΤΩΝ ΕΛΛΗΝΩΝ
     3: ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ
     4: 938.393ΚΑΡ
-    5: 9292Α
+    5: 09292
     8: ΛΙΒΑΝΗ
     9: ΑΘΗΝΑ
     10: '2002'
     11: 254Σ
     12: ΙΣΤΟΡΙΑ-ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ
     13: ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ-ΙΣΤΟΡΙΑ
     14: ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ
@@ -371990,15 +371834,15 @@
   authors:
   - ΚΑΡΖΗ,ΘΟΔΩΡΟΥ
   language: el
   title: ΟΙ ΠΑΤΡΙΔΕΣ ΤΩΝ ΕΛΛΗΝΩΝ
   subtitle: ΠΕΛΑΓΟΝΙΑ-ΒΟΡΕΙΑ ΗΠΕΙΡΟΣ
   dewey: 938.393 ΚΑΡ
   entry_numbers:
-  - 9292Α
+  - 09292
   editor: ΛΙΒΑΝΗ // ΑΘΗΝΑ
   edition_year: 2002
   pages: 386
   topics:
   - ΠΕΛΑΓΟΝΙΑ
   - ΒΟΡΕΙΑ ΗΠΕΙΡΟΣ
   volume: ΤΟΜΟΣ Δ
@@ -372008,15 +371852,15 @@
   isbn: 960-14-0453-8
   original_entry:
     0: 7401
     1: ΚΑΡΖΗ,ΘΟΔΩΡΟΥ
     2: ΟΙ ΠΑΤΡΙΔΕΣ ΤΩΝ ΕΛΛΗΝΩΝ
     3: ΠΕΛΑΓΟΝΙΑ-ΒΟΡΕΙΑ ΗΠΕΙΡΟΣ
     4: 938.393ΚΑΡ
-    5: 9292Α
+    5: 09292
     8: ΛΙΒΑΝΗ
     9: ΑΘΗΝΑ
     10: '2002'
     11: 386Σ
     12: ΙΣΤΟΡΙΑ-ΠΕΛΑΓΟΝΙΑ-ΒΟΡΕΙΑ ΗΠΕΙΡΟΣ
     13: ΠΕΛΑΓΟΝΙΑ-ΒΟΡΕΙΑ ΗΠΕΙΡΟΣ
     14: ΙΣΤΟΡΙΑ
@@ -372291,30 +372135,30 @@
   authors:
   - ΣΙΔΕΡΗΣ,Ι
   language: el
   title: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΙΣ ΚΑΙ ΕΘΝΙΚΗ ΜΕΙΟΔΟΣΙΑ
   subtitle: ΧΡΟΝΙΚΟΝ 1941-1944
   dewey: 938.764 ΣΙΔ
   entry_numbers:
-  - 9289Α
+  - 09289
   editor: ΣΙΔΕΡΗΣ // ΑΘΗΝΑ
   edition_year: 1983
   pages: 440
   topics:
   - ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7407
     1: ΣΙΔΕΡΗΣ,Ι
     2: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΙΣ ΚΑΙ ΕΘΝΙΚΗ ΜΕΙΟΔΟΣΙΑ
     3: ΧΡΟΝΙΚΟΝ 1941-1944
     4: 938.764ΣΙΔ
-    5: 9289Α
+    5: 09289
     8: ΣΙΔΕΡΗΣ
     9: ΑΘΗΝΑ
     10: '1983'
     11: 440Σ
     12: ΙΣΤΟΡΙΑ-ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
     13: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ-ΙΣΤΟΡΙΑ
     14: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
@@ -372340,30 +372184,31 @@
   authors:
   - ΒΙΔΑΛΗΣ,ΟΡΕΣΤΗΣ
   language: el
   title: ΙΣΤΟΡΙΚΟ ΗΜΕΡΟΛΟΓΙΟ
   subtitle: ΧΡΟΝΙΑ ΕΚΠΑΤΡΙΣΜΟΥ 1968-1975
   dewey: 938.790 ΒΙΔ
   entry_numbers:
-  - 4288,4292
+  - '4288'
+  - '4292'
   editor: LIBRO // ΑΘΗΝΑ
   edition_year: 1997
   pages: 570
   topics:
   - ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 7408
     1: ΒΙΔΑΛΗΣ,ΟΡΕΣΤΗΣ
     2: ΙΣΤΟΡΙΚΟ ΗΜΕΡΟΛΟΓΙΟ
     3: ΧΡΟΝΙΑ ΕΚΠΑΤΡΙΣΜΟΥ 1968-1975
     4: 938.790ΒΙΔ
-    5: 4288,4292
+    5: 4288-4292
     8: LIBRO
     9: ΑΘΗΝΑ
     10: '1997'
     11: '570'
     12: ΙΣΤΟΡΙΑ-ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
     13: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ-ΙΣΤΟΡΙΑ
     14: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
@@ -372388,15 +372233,15 @@
 - dbase_number: 7409
   authors: []
   language: el
   title: ΜΕΓΑΛΗ ΕΛΛΑΔΑ
   subtitle: ΠΕΡΙΟΔΟΣ 1944-1945
   dewey: 938.752 ΧΣ
   entry_numbers:
-  - 9283Α
+  - 09283
   - '6759'
   - '5007'
   editor: None // ΑΘΗΝΑ
   edition_year: 1998
   pages: 135
   topics:
   - ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
@@ -372406,15 +372251,15 @@
   offprint: false
   original_entry:
     0: 7409
     1: Χ.Σ.
     2: ΜΕΓΑΛΗ ΕΛΛΑΔΑ
     3: ΠΕΡΙΟΔΟΣ 1944-1945
     4: 938.752Χ.Σ
-    5: 9283Α-6759-5007
+    5: 09283-6759-5007
     9: ΑΘΗΝΑ
     10: '1998'
     11: 135Σ
     12: ΙΣΤΟΡΙΑ-ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
     13: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ-ΙΣΤΟΡΙΑ
     14: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
     17: 3 ΑΝΤΙΤΥΠΑ
@@ -373692,15 +373537,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7436
   authors:
-  - ΒΙΖΥΗΝΟΣ, Γ, Δ
+  - ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ,M.
   language: el
   title: ΑΙ ΣΥΝΕΠΕΙΑΙ ΤΗΣ ΠΑΛΑΙΑΣ ΙΣΤΟΡΙΑΣ
   dewey: 889 ΒΙΖ
   entry_numbers:
   - '9925'
   editor: ΓΑΛΑΞΙΑΣ // ΑΘΗΝΑ
   edition_year: 1971
@@ -373743,15 +373588,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7437
   authors:
-  - ΒΙΖΥΗΝΟΣ, Γ, Μ
+  - ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ,M.
   language: el
   title: ΤΟ ΑΜΑΡΤΗΜΑ ΤΗΣ ΜΗΤΡΟΣ ΜΟΥ
   dewey: 889 ΒΙΖ
   entry_numbers:
   - '9924'
   edition: '5'
   editor: ΓΑΛΑΞΙΑΣ // ΑΘΗΝΑ
@@ -373795,15 +373640,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7438
   authors:
-  - ΑΝΝΙΝΟΣ, ΜΠΑΜΠΗΣ
+  - ΑΝΝΙΝΟΣ,ΜΠΑΜΠΗΣ
   language: el
   title: Η ΑΠΟΛΟΓΙΑ ΤΟΥ ΟΔΥΣΣΕΩΣ ΑΝΔΡΟΥΤΣΟΥ
   dewey: 889 ΑΝΝ
   entry_numbers:
   - '9919'
   - '9917'
   edition: '2'
@@ -373820,15 +373665,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 7438
     1: ΑΝΝΙΝΟΣ, ΜΠΑΜΠΗΣ
     2: Η ΑΠΟΛΟΓΙΑ ΤΟΥ ΟΔΥΣΣΕΩΣ ΑΝΔΡΟΥΤΣΟΥ
     4: 889ΑΝΝ
-    5: 9919,9917
+    5: 9919-9917
     7: 2Η
     8: ΓΑΛΑΞΙΑΣ
     9: ΑΘΗΝΑ
     10: '1969'
     11: 133Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΚΑ ΣΗΜΕΙΩΜΑΤΑ
     13: ΙΣΤΟΡΙΚΑ ΣΗΜΕΙΩΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -373875,15 +373720,15 @@
   offprint: false
   original_entry:
     0: 7439
     1: ΑΝΝΙΝΟΣ,ΜΠΑΜΠΗΣ
     2: ΑΙ ΑΘΗΝΑΙ ΤΟΥ 1850
     3: ΕΚΤΥΠΩΣΕΙΣ ΔΥΟ ΓΑΛΛΩΝ ΠΕΡΙΗΓΗΤΩΝ
     4: 889ΑΝΝ
-    5: 9918,9916
+    5: 9918-9916
     8: ΓΑΛΑΞΙΑΣ
     9: ΑΘΗΝΑ
     10: '1971'
     11: 127Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΚΑ ΣΗΜΕΙΩΜΑΤΑ
     13: ΙΣΤΟΡΙΚΑ ΣΗΜΕΙΩΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΒΙΒΛΙΟΘΗΚΗ ΓΑΡΟΥΦΑΛΙΑ
@@ -374110,15 +373955,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7444
   authors:
-  - ΑΜΠΟΥ,ΕΝΤΜΟΝΤ
+  - ABOUT,EDMOND,FRANCOIS VALENTIN
   language: el
   title: Ο ΒΑΣΙΛΕΥΣ ΤΩΝ ΟΡΕΩΝ
   dewey: 889 ΑΜΠ
   entry_numbers:
   - '9904'
   editor: ΓΑΛΑΞΙΑΣ // ΑΘΗΝΑ
   edition_year: 1968
@@ -374608,15 +374453,15 @@
   offprint: false
   original_entry:
     0: 7453
     1: ΞΕΝΟΦΩΝΤΑΣ
     2: ΕΛΛΗΝΙΚΑ
     3: ΤΟΜΟΣ ΠΡΩΤΟΣ Α-Γ
     4: 180ΞΕΝ
-    5: 9926,9914
+    5: 9926-9914
     6: ΡΟΥΦΟΥ.ΡΟΔΗ
     8: ΓΑΛΑΞΙΑΣ
     9: ΑΘΗΝΑ
     10: '1966'
     11: 151Σ
     12: ΑΡΧΑΙΟΙ ΣΥΓΓΡΑΦΕΙΣ-ΞΕΝΟΦΩΝΤΑΣ
     13: ΞΕΝΟΦΩΝΤΑΣ-ΑΡΧΑΙΟΙ ΣΥΓΓΡΑΦΕΙΣ
@@ -375731,15 +375576,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 7474
     1: ΧΡΗΣΤΟΜΑΝΟΣ, ΚΩΝΣΤΑΝΤΙΝΟΣ
     2: Η ΚΕΡΕΝΙΑ ΚΟΥΚΛΑ
     4: 889.21ΧΡΗ
-    5: 8742,9948
+    5: 8742-9948
     8: ΓΑΛΑΞΙΑΣ
     9: ΑΘΗΝΑ
     10: '1969'
     11: 176Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     17: ΒΙΒΛΙΟΘΗΚΗ ΓΑΡΟΥΦΑΛΙΑ
@@ -375912,15 +375757,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7478
   authors:
-  - ΒΛΑΧΟΣ, ΑΓΓΕΛΟΣ
+  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ,
   language: el
   title: ΤΟ ΜΝΗΜΑ ΤΗΣ ΓΡΗΑΣ ΚΑΙ ΟΙ ΩΡΕΣ ΖΩΗΣ
   dewey: 889.21 ΒΛΑ
   entry_numbers:
   - '9934'
   edition: '2'
   editor: ΓΑΛΑΞΙΑΣ // ΑΘΗΝΑ
@@ -376169,15 +376014,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7483
   authors:
-  - ΒΛΑΧΟΓΙΑΝΝΗΣ. Ι
+  - ΒΛΑΧΟΓΙΑΝΝΗΣ,ΓΙΑΝΝΗΣ
   language: el
   title: ΣΤΡΑΤΗΓΟΥ ΜΑΚΡΥΓΙΑΝΝΗ ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ
   dewey: 889 ΒΛΑ
   entry_numbers:
   - '9955'
   edition: '3'
   editor: ΓΑΛΑΞΙΑΣ // ΑΘΗΝΑ
@@ -376273,15 +376118,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7485
   authors:
-  - ΒΕΡΝΑΡΔΑΚΗΣ, ΔΗΜΗΤΡΙΟΣ
+  - ΒΕΡΝΑΡΔΑΚΗΣ,ΔΗΜΗΤΡΙΟΣ
   language: el
   title: ΚΑΠΟΔΙΣΤΡΙΑΣ ΚΑΙ ΟΘΩΝ
   subtitle: ΕΠΙΣΤΟΛΙΜΑΙΑ ΒΙΒΛΙΟΚΡΙΣΙΑ
   dewey: 889 ΒΕΡ
   entry_numbers:
   - '9950'
   edition: '3'
@@ -376439,17 +376284,16 @@
   title: ΑΛΩΣΗ ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΕΩΣ 1453
   dewey: 938.389 ΡΑΝ
   entry_numbers:
   - '9957'
   - '1997'
   - '1998'
   - '2848'
-  - '2847'
   translators:
-  - ΠΑΠΑΡΡΟΔΟΥ,ΝΙΚΟΛΑΟΣ
+  - ΠΑΠΑΡΡΟΔΟΣ,ΝΙΚ.
   editor: ΜΠΕΡΓΑΔΗ // ΑΘΗΝΑ
   edition_year: 1972
   pages: 189
   topics:
   - ΛΟΓΟΤΕΧΝΙΑ
   - ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
   donors:
@@ -376459,16 +376303,16 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 7488
     1: ΡΑΝΣΙΜΑΝ, ΣΤ
     2: ΑΛΩΣΗ ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΕΩΣ 1453
     4: 938.389ΡΑΝ
-    5: 9957-1997-1998-2848-
-    6: 2847 ΠΑΠΑΡΡΟΔΟΥ,ΝΙΚ
+    5: 9957-1997-1998-2848
+    6: ΠΑΠΑΡΡΟΔΟΥ,ΝΙΚ
     8: ΜΠΕΡΓΑΔΗ
     9: ΑΘΗΝΑ
     10: '1972'
     11: 189Σ
     12: ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ-ΛΟΓΟΤΕΧΝΙΑ
     17: ΒΙΒΛΙΟΘΗΚΗ ΓΑΡΟΥΦΑΛΙΑ
@@ -377836,15 +377680,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7516
   authors:
-  - ΑΙΓΙΑΛΕΙΔΟΥ. ΓΕΩΡΓΙΟΥ
+  - ΑΙΓΙΑΛΕΙΔΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΤΟ ΧΡΟΝΙΚΟ ΤΗΣ ΑΘΗΝΑΙΚΗΣ ΛΕΣΧΗΣ
   entry_numbers:
   - '9989'
   editor: ΠΑΤΡΙΣ // ΑΘΗΝΑ
   edition_year: 1975
   pages: 65
@@ -377984,15 +377828,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 7519
   authors:
-  - ΒΑΡΒΙΤΣΙΩΤΗΣ. ΜΙΛΤ. ΙΩΑΝΝΗΣ
+  - ΒΑΡΒΙΤΣΙΩΤΗΣ,ΜΙΛΤΙΑΔΗΣ,ΙΩΑΝΝΗ
   language: el
   title: Η ΕΥΡΩΠΑΙΚΗ ΟΙΚΟΝΟΜΙΚΗ ΚΟΙΝΟΤΗΣ ΚΑΙ ΤΟ ΕΤΑΙΡΙΚΟΝ ΔΙΚΑΙΟΝ
   entry_numbers:
   - '9981'
   editor: ΤΥΠΟ ΤΕΧΝΙΚΗ // ΑΘΗΝΑ
   edition_year: 1970
   pages: 130
@@ -378625,15 +378469,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7532
   authors:
-  - ΑΜΑΝΑΤΙΔΗΣ.Δ.Η.
+  - ΑΜΑΝΑΤΙΔΗΣ,Δ.,Η.
   language: el
   title: ΕΜΒΟΛΙΜΑ
   dewey: 889.1 ΑΜΑ
   entry_numbers:
   - '9984'
   editor: ΝΕΑ ΣΚΕΨΗ // ΑΘΗΝΑ
   edition_year: 1971
@@ -378724,15 +378568,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7534
   authors:
-  - ΑΒΡΑΑΜ ΚΩΣΤΑΣ
+  - ΑΒΡΑΑΜ,ΚΩΣΤΑΣ
   language: el
   title: ΕΠΙΜΥΘΙΑ
   dewey: 889.1 ΑΒΡ
   entry_numbers:
   - '10076'
   editor: ΝΕΑ ΣΚΕΨΗ // ΑΘΗΝΑ
   edition_year: 1972
@@ -379160,15 +379004,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7543
   authors:
-  - ΑΓΓΕΛΙΔΗΣ ΑΡ. Δ.
+  - ΑΓΓΕΛΙΔΗΣ,ΑΡ.,Δ.
   language: el
   title: ΝΟΜΟΛΟΓΙΑΚΗ ΜΕΛΕΤΗ ΕΠΙ ΜΙΣΘΩΣΕΩΣ ΠΡΑΓΜΑΤΟΣ
   entry_numbers:
   - '10095'
   editor: ΚΑΣΙΜΗΣ // ΑΘΗΝΑ
   edition_year: 1936
   pages: 147
@@ -379352,15 +379196,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7547
   authors:
-  - ΑΤΤΑΛΙΩΤΗΣ ΠΑΝΟΣ
+  - ΑΤΤΑΛΙΩΤΗΣ,ΠΑΝΟΣ
   language: el
   title: ΓΥΜΝΑΣΕΙΣ
   entry_numbers:
   - '10091'
   editor: ΣΦΥΡΙΔΟΥ // ΑΘΗΝΑ
   edition_year: 1972
   pages: 22
@@ -380030,15 +379874,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7561
   authors:
-  - ΒΑΡΟΥΞΗΣ ΣΠΥΡΙΔΩΝ
+  - ΒΑΡΟΥΞΗΣ,ΣΠΥΡΙΔΩΝ
   language: el
   title: Η ΕΝ ΕΛΛΑΔΙ ΦΟΡΟΛΟΓΙΑ
   entry_numbers:
   - '10063'
   editor: None // ΑΘΗΝΑ
   edition_year: 1936
   pages: 600
@@ -380078,15 +379922,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7562
   authors:
-  - ΑΝΔΡΕΟΥ ΑΠΟΣΤΟΛΟΣ
+  - ΑΝΔΡΕΟΥ,ΑΠΟΣΤΟΛΟΣ
   language: el
   title: Η ΕΞΩΤΕΡΙΚΗ ΕΜΠΟΡΙΚΗ ΠΟΛΙΤΙΚΗ ΤΗΣ ΕΛΛΑΔΟΣ
   entry_numbers:
   - '10061'
   editor: ΡΟΔΗ // ΑΘΗΝΑ
   edition_year: 1933
   pages: 552
@@ -381319,15 +381163,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7588
   authors:
-  - ΒΥΤΙΝΑΡΟΣ ΒΑΣ.
+  - ΒΥΤΙΝΑΡΟΣ,ΒΑΣΙΛΗΣ
   language: el
   title: ΟΛΥΜΠΙΑΚΗ ΗΜΕΡΑ
   entry_numbers:
   - '10114'
   editor: ΑΘΑΝΑΣΟΠΟΥΛΟΣ // None
   edition_year: 1973
   pages: 31
@@ -381895,15 +381739,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7600
   authors:
-  - ΑΝΩΝΥΜΟΣ
+  - ΑΝΩΝΥΜΟΣ ΣΥΓΓΡΑΦΕΑΣ
   language: el
   title: ΔΟΚΙΜΙΑ
   entry_numbers:
   - '10032'
   editor: ΚΛΑΠΑΚΗΣ // ΑΘΗΝΑ
   edition_year: 1971
   pages: 215
@@ -382568,15 +382412,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7614
   authors:
-  - ΑΝΑΓΝΩΣΤΟΠΟΥΛΟΣ ΝΙΚΟΛΑΟΣ
+  - ΑΝΑΓΝΩΣΤΟΠΟΥΛΟΣ,ΝΙΚΟΛΑΟΣ
   language: el
   title: Η ΣΥΧΡΟΝΟΣ ΚΡΙΣΙΣ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
   entry_numbers:
   - '9986'
   editor: None // ΑΘΗΝΑ
   edition_year: 1974
   pages: 71
@@ -383047,15 +382891,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7624
   authors:
-  - ΒΑΜΒΕΤΣΟΣ ΑΛΕΞΑΝΔΡΟΣ
+  - ΒΑΜΒΕΤΣΟΣ,ΑΛΕΞΑΝΔΡΟΣ
   language: el
   title: ΧΩΡΙΣ ΟΡΓΗΝ ΚΑΙ ΜΙΣΟΣ
   entry_numbers:
   - '10040'
   editor: None // ΑΘΗΝΑ
   edition_year: 1966
   pages: 50
@@ -383142,15 +382986,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7626
   authors:
-  - ΑΥΑΓΓΕΛΑΤΟΣ ΧΡΗΣΤΟΣ
+  - ΑΥΑΓΓΕΛΑΤΟΣ,ΧΡΗΣΤΟΣ
   language: el
   title: ΤΙΝΕΣ ΛΟΓΟΙ ΕΠΙΒΑΛΟΥΝ ΤΗΝ ΕΠΑΝΙΔΡΥΣΙΝ ΤΗΣ ΕΝΩΣΕΩΣ ΤΩΝ
   subtitle: ΔΗΜΩΝ ΚΑΙ ΚΟΙΝΟΤΗΤΩΝ ΤΗΣ ΕΛΛΑΔΟΣ
   entry_numbers:
   - '10036'
   editor: ΚΛΕΙΣΙΟΥΝΗΣ // ΑΘΗΝΑ
   edition_year: 1945
@@ -385799,15 +385643,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 7680
   authors:
-  - ALEXANDRE DUMAS
+  - DUMAS,ALEXANDRE
   language: el
   title: Η ΜΑΥΡΗ ΤΟΥΛΙΠΑ
   dewey: 843 DUM
   entry_numbers:
   - '10179'
   translators:
   - ΔΗΜΟΥΛΑΣ,ΔΗΜΗΤΡΗΣ
@@ -385956,15 +385800,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7683
   authors:
-  - VAN GULIK ROBERT
+  - VAN GULIK,ROBERT
   language: el
   title: ΤΟ ΜΥΣΤΗΡΙΩΔΕΣ ΠΑΡΑΒΑΝ
   dewey: 890.3 GUL
   entry_numbers:
   - '10176'
   translators:
   - ΖΑΧΟΥ,ΝΤΙΝΤΑ
@@ -386059,15 +385903,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7685
   authors:
-  - ΑΝΤΩΝΙΟΥ_ΜΑΡΚΟΣ
+  - ΑΝΤΩΝΙΟΥ,ΜΑΡΚΟΣ
   language: el
   title: ΠΡΟΣΩ ΚΡΑΤΙΚΟΙ
   entry_numbers:
   - '10174'
   edition_year: 2000
   pages: 124
   topics:
@@ -386107,15 +385951,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7686
   authors:
-  - ΑΝΤΩΝΙΟΥ_ΜΑΡΚΟΣ
+  - ΑΝΤΩΝΙΟΥ,ΜΑΡΚΟΣ
   language: el
   title: ΘΟΥΚΥΔΙΔΗ ΕΒΔΟΜΗΝΤΑ ΕΦΤΑ
   entry_numbers:
   - '10173'
   edition_year: 2001
   pages: 155
   topics:
@@ -386206,15 +386050,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7688
   authors:
-  - ΒΑΣΙΛΕΙΟΥ_ΚΩΝΣΤΑΝΤΙΝΟΣ
+  - ΒΑΣΙΛΕΙΟΥ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΚΑΠΙΤΑΛΙΣΜΟΣ ΑΝΕΥ ΔΑΣΚΑΛΟΥ
   dewey: 889.21 ΒΑΣ
   entry_numbers:
   - '10171'
   editor: ΜΠΑΡΤΖΟΥΛΙΑΝΟΣ // ΑΘΗΝΑ
   edition_year: 2009
@@ -386309,15 +386153,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7690
   authors:
-  - ΑΝΤΩΝΙΟΥ ΜΑΡΚΟΣ
+  - ΑΝΤΩΝΙΟΥ,ΜΑΡΚΟΣ
   language: el
   title: ΚΑΙΡΟΣ
   dewey: 230 ΑΝΤ
   entry_numbers:
   - '10202'
   editor: ΓΙΑΠΟΥΛΗΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2003
@@ -386412,15 +386256,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7692
   authors:
-  - ΒΑΜΒΟΥΝΑΚΗ ΜΑΡΩ
+  - ΒΑΜΒΟΥΝΑΚΗ,ΜΑΡΩ
   language: el
   title: Ο ΑΝΤΙΠΑΛΟΣ ΕΡΑΣΤΗΣ
   dewey: 889.21 ΒΑΜ
   entry_numbers:
   - '10196'
   edition: '18'
   editor: ΦΙΛΙΠΠΟΤΗ // ΑΘΗΝΑ
@@ -386877,15 +386721,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7701
   authors:
-  - ΑΚΟΥΝΙΝ ΜΠΟΡΙΣ
+  - AKUNIN,BORIS
   language: el
   title: ΑΖΑΖΕΛ
   subtitle: Ο ΕΒΡΑΙΚΟΣ ΔΑΙΜΟΝΑΣ
   dewey: 891.73 ΑΚΟ
   entry_numbers:
   - '10183'
   translators:
@@ -387384,15 +387228,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7711
   authors:
-  - ΑΝΤΩΝΙΟΥ ΜΑΡΚΟΣ
+  - ΑΝΤΩΝΙΟΥ,ΜΑΡΚΟΣ
   language: el
   title: ΑΓΡΟΙΚΟΝ ΜΕΛΟΣ
   dewey: 230 ΑΝΤ
   entry_numbers:
   - '10204'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2008
@@ -387434,15 +387278,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7712
   authors:
-  - ΑΝΤΩΝΙΟΥ ΜΑΡΚΟΣ
+  - ΑΝΤΩΝΙΟΥ,ΜΑΡΚΟΣ
   language: el
   title: ΠΟΛΙΤΕΙΑ
   subtitle: Ο ΚΥΚΛΟΣ ΤΟΥ ΠΑΘΟΥΣ
   entry_numbers:
   - '10203'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2008
@@ -387889,15 +387733,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7721
   authors:
-  - ΑΝΤΩΝΙΟΥ ΜΑΡΚΟΣ
+  - ΑΝΤΩΝΙΟΥ,ΜΑΡΚΟΣ
   language: el
   title: ΛΟΓΟΣ
   dewey: 230 ΑΝΤ
   entry_numbers:
   - '10222'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2004
@@ -387987,15 +387831,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7723
   authors:
-  - ΑΘΑΝΑΣΙΑΔΗΣ ΤΙΤΟΣ
+  - ΑΘΑΝΑΣΙΑΔΗΣ,ΤΙΤΟΣ
   language: el
   title: ΠΟΛΙΤΙΚΗ ΖΩΗ ΚΑΙ ΟΛΥΜΠΙΑΚΟΙ ΑΓΩΝΕΣ ΣΤΗΝ ΑΡΧΑΙΟΤΗΤΑ
   entry_numbers:
   - '10224'
   editor: ΚΑΘΗΜΕΡΙΝΗ // ΑΘΗΝΑ
   pages: 159
   topics:
@@ -389468,15 +389312,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7753
   authors:
-  - ΒΕΦΑ ΑΛΕΞΙΑ ΑΛΕΞΙΑΔΟΥ
+  - ΑΛΕΞΙΑΔΟΥ,ΒΕΦΑ
+  - ΑΛΕΞΙΑΔΟΥ,ΑΛΕΞΙΑ
   language: el
   title: ΝΗΣΤΗΣΙΜΑ ΚΑΙ ΥΓΙΕΙΝΑ
   dewey: 641.5 ΑΛΕ
   entry_numbers:
   - '10260'
   editor: ΠΕΡΓΑΜΟΣ // None
   edition_year: 1999
@@ -389619,15 +389464,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7756
   authors:
-  - ΑΘΑΝΑΣΙΑΔΗΣ ΤΑΣΟΣ
+  - ΑΘΑΝΑΣΙΑΔΗΣ,ΤΑΣΟΣ
   language: el
   title: ΤΑ ΠΑΙΔΙΑ ΤΗΣ ΝΙΟΒΗΣ
   dewey: '889'
   entry_numbers:
   - '8893'
   edition: '13'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
@@ -390018,15 +389863,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7764
   authors:
-  - ΒΟΥΝΑ,ΧΡΗΣΤΟΥ
+  - ΒΟΥΝΑΣ,ΧΡΗΣΤΟΣ
   language: el
   title: ΚΕΦΑΛΟΝΙΤΙΚΕΣ ΙΣΤΟΡΙΕΣ ΚΑΙ ΘΡΥΛΟΙ
   dewey: 889.21 ΒΟΥ
   entry_numbers:
   - '5460'
   editor: None // ΠΑΤΡΑ
   edition_year: 1966
@@ -390666,15 +390511,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7777
   authors:
-  - ΒΑΛΑΚΑ ΜΗΤΣΗ
+  - ΒΑΛΑΚΑ,ΜΗΤΣΗ
   language: el
   title: ΟΙ ΜΕΓΑΛΟΙ ΕΡΩΤΕΣ ΔΕ ΦΟΡΑΝΕ ΝΥΦΙΚΟ
   dewey: '889.21'
   entry_numbers:
   - '9098'
   editor: ΛΙΒΑΝΗ // ΑΘΗΝΑ
   edition_year: 2002
@@ -390766,15 +390611,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7779
   authors:
-  - ΑΝΑΣΤΑΣΟΠΟΥΛΟΣ ΓΙΑΝΙΣ
+  - ΑΝΑΣΤΑΣΟΠΟΥΛΟΣ,ΓΙΑΝΝΗΣ
   language: el
   title: ΤΟ ΠΕΡΙΒΑΛΛΟΝ
   dewey: 889.21 ΑΝΑ
   entry_numbers:
   - '7721'
   edition: '3'
   editor: ΣΤΕΦΑΝ,ΒΑΣΙΛΟΠΟΥΛΟΣ // ΑΘΗΝΑ
@@ -391016,15 +390861,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7784
   authors:
-  - ΑΡΓΥΡΑΚΗΣ ΜΙΝΟΣ
+  - ΑΡΓΥΡΑΚΗΣ,ΜΙΝΟΣ
   language: el
   title: Ο ΓΥΡΟΣ ΤΟΥ ΚΟΣΜΟΥ
   dewey: 889.21 ΑΡΓ
   entry_numbers:
   - '8103'
   editor: ΓΑΛΑΞΙΑ // ΑΘΗΝΑ
   edition_year: 1964
@@ -391259,15 +391104,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7789
   authors:
-  - ΑΝΔΡΙΚΟΠΟΥΛΟΥ ΓΡΟΠΙΩΤΗ ΓΙΑΝΝΗ
+  - ΑΝΔΡΙΚΟΠΟΥΛΟΣ ΓΡΟΠΙΩΤΗΣ,ΓΙΑΝΝΗΣ
   language: el
   title: ΤΥΦΛΗ ΠΟΡΕΙΑ
   dewey: 889.21 ΑΝΔ
   entry_numbers:
   - '7725'
   editor: None // ΑΘΗΝΑ
   edition_year: 2000
@@ -391361,15 +391206,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7791
   authors:
-  - ΑΚΡΙΤΑ ΕΛΕΝΑ
+  - ΑΚΡΙΤΑ,ΕΛΕΝΑ
   language: el
   title: ΑΠΟ ΤΗΝ ΕΛΕΝΑ ΜΕ ΧΑΜΟΓΕΛΟ!
   dewey: 889.21 ΑΚΡ
   entry_numbers:
   - '8510'
   edition: Β
   editor: ΚΑΚΤΟΣ // ΑΘΗΝΑ
@@ -391463,15 +391308,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7793
   authors:
-  - ΑΥΓΟΥΣΤΙΔΗΣ ΙΑΤΡΟΥ ΣΤΡΑΤΗΣ
+  - ΑΥΓΟΥΣΤΙΔΗΣ,ΣΤΡΑΤΗΣ
   language: el
   title: Ο ΑΝΕΛΕΥΘΕΡΟΣ ΚΑΙ ΑΛΛΑ ΔΙΗΓΗΜΑΤΑ
   dewey: 889.21 ΑΥΓ
   entry_numbers:
   - '10298'
   editor: None // ΑΘΗΝΑ
   edition_year: 1986
@@ -392012,15 +391857,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7804
   authors:
-  - ΑΓΑΠΗΤΟΣ ΙΩΣΗΦ
+  - ΑΓΑΠΗΤΟΣ,ΙΩΣΗΦ
   language: el
   title: Η ΠΑΝΕΜΟΡΦΗ
   dewey: 889.21 ΑΓΑ
   entry_numbers:
   - '9664'
   editor: ΚΑΡΔΙΑΣ // ΑΘΗΝΑ
   pages: 110
@@ -392655,15 +392500,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7817
   authors:
-  - ΒΙΓΛΑΣ ΙΩΑΝΝΗΣ
+  - ΒΙΓΛΑΣ,ΙΩΑΝΝΗΣ
   language: el
   title: ΔΙΗΓΗΜΑΤΑ
   subtitle: ΑΦΗΓΗΣΕΙΣ ΠΕΡΙΓΡΑΦΕΣ ΜΥΘΟΙ
   dewey: 889.21 ΒΙΓ
   entry_numbers:
   - '10272'
   editor: ΜΟΡΙΑΣ // ΑΘΗΝΑ
@@ -392762,15 +392607,15 @@
 - dbase_number: 7819
   authors:
   - ΖΗΚΟΥ ΜΑΙΡΗ
   language: el
   title: Η ΠΡΟΣΤΥΧΗ
   dewey: 889.21 ΖΗΚ
   entry_numbers:
-  - 9160Α
+  - 09160
   editor: ΜΟΝΤΕΡΝΟΙ ΚΑΙΡΟΙ // ΑΘΗΝΑ
   edition_year: 2007
   pages: 264
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ ΜΥΘΙΣΤΟΡΗΜΑ
   - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
@@ -392778,15 +392623,15 @@
   offprint: false
   ean: 978-960-441-621-9
   original_entry:
     0: 7819
     1: ΖΗΚΟΥ ΜΑΙΡΗ
     2: Η ΠΡΟΣΤΥΧΗ
     4: 889.21ΖΗΚ
-    5: 9160Α
+    5: 09160
     8: ΜΟΝΤΕΡΝΟΙ ΚΑΙΡΟΙ
     9: ΑΘΗΝΑ
     10: '2007'
     11: 264Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΜΥΘΙΣΤΟΡΗΜΑ
@@ -393996,15 +393841,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7843
   authors:
-  - ΒΕΖΙΝΟΡ ΠΑΒΕΛ
+  - VESINOV,PAVEL
   language: el
   title: ΑΣΠΡΑ ΑΛΟΓΑ ΜΕΣ ΣΤΗ ΝΥΧΤΑ
   dewey: 891.81 ΒΕΖ
   entry_numbers:
   - '7728'
   translators:
   - ΧΑΤΖΗΓΙΑΝΝΗ,ΜΑΡΙΑ
@@ -394509,15 +394354,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7853
   authors:
-  - ΑΝΤΟΥΝΕΣ ΛΟΜΠΟ ΑΝΤΟΝΙΟ
+  - ANTUNES,ANTONIO,LOBO
   language: el
   title: ΤΟ ΜΕΓΑΛΕΙΟ ΤΗΣ ΠΟΡΤΟΓΑΛΙΑΣ
   dewey: 869 ΑΝΤ
   entry_numbers:
   - '9858'
   translators:
   - ΨΥΛΛΙΑ,ΑΘΗΝΑ
@@ -394561,15 +394406,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7854
   authors:
-  - ΑΜΑΝΤΟ ΖΟΡΖΕ
+  - AMADO,JORGE
   language: el
   title: Η ΑΝΑΚΑΛΥΨΗ ΤΗΣ ΤΟΥΡΚΙΑ ΑΠΟ ΤΟΥΣ ΤΟΥΡΚΟΥΣ
   dewey: 869 ΑΜΑ
   entry_numbers:
   - '9855'
   translators:
   - ΨΥΛΛΙΑ,ΑΘΗΝΑ
@@ -396114,15 +395959,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7885
   authors:
-  - AJAR EMILE
+  - AJAR,EMILE
   language: el
   title: Η ΖΩΗ ΜΠΡΟΣΤΑ ΣΟΥ
   dewey: 843 AJA
   entry_numbers:
   - '10325'
   translators:
   - ΜΟΥΡΕΛΑΤΟΥ,ΡΕΝΑ
@@ -397781,15 +397626,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7918
   authors:
-  - ΑΡΙΑΣ ΑΜΠΕΛΑΡΔΟ
+  - ARIAS,ABELARDO
   language: el
   title: ΚΟΥΡΝΙΑΧΤΟΣ ΚΑΙ ΤΡΟΜΟΣ
   dewey: 860.11 ΑΡΙ
   entry_numbers:
   - '10338'
   translators:
   - ΧΟΥΜΟΥΡΖΙΑΔΗΣ,Γ.
@@ -397985,15 +397830,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7922
   authors:
-  - ΒΙΛΛΙΕ ΖΕΡΑΡ
+  - DE VILLIERS,GERARD
   language: el
   title: ΘΑΝΑΤΟΣ ΣΤΗ ΒΗΡΥΤΟ
   dewey: 843 ΒΙΛ
   entry_numbers:
   - '10360'
   translators:
   - ΚΑΒΒΑΔΙΑ,ΤΑΣΣΩ
@@ -398036,15 +397881,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7923
   authors:
-  - ΒΙΛΛΙΕ ΖΕΡΑΡ
+  - DE VILLIERS,GERARD
   language: el
   title: ΟΙ ΟΜΗΡΟΙ ΤΟΥ ΤΟΚΙΟ
   dewey: 843 ΒΙΛ
   entry_numbers:
   - '10359'
   translators:
   - ΚΑΒΒΑΔΙΑ,ΤΑΣΣΩ
@@ -398942,15 +398787,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7941
   authors:
-  - ΑΝΤΖΑΚΑ ΣΟΦΙΑ
+  - ΑΝΤΖΑΚΑ,ΣΟΦΙΑ
   language: el
   title: Η ΑΛΛΗ ΤΕΧΝΗ
   dewey: 889.1 ΑΝΤ
   entry_numbers:
   - '8479'
   editor: ΑΝΤΙΝΕΑ // ΑΘΗΝΑ
   pages: 178
@@ -398991,15 +398836,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7942
   authors:
-  - ΑΝΔΡΕΟΥ ΑΥΓΕΡΙΝΟΣ
+  - ΑΝΔΡΕΟΥ,ΑΥΓΕΡΙΝΟΣ
   language: el
   title: ΑΝΤΙΣΤΡΟΦΕΣ
   dewey: 889.1 ΑΝΔ
   entry_numbers:
   - '7646'
   editor: ΑΡΕΝΖΟ // ΑΘΗΝΑ
   edition_year: 2001
@@ -399040,15 +398885,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7943
   authors:
-  - ΑΡΓΥΡΗ - ΛΙΑΡΟΥ ΕΥΑ
+  - ΑΡΓΥΡΗ-ΛΙΑΡΟΥ,ΕΥΑ
   language: el
   title: ΤΟ ΜΕΤΑΞΥ ΤΩΝ ΖΕΥΓΑΡΙΩΝ
   dewey: 889.1 ΑΡΓ
   entry_numbers:
   - '5293'
   editor: ΒΙΒΛΙΟΘ.ΛΕΒΑΔΕΙΑΣ // ΑΘΗΝΑ
   edition_year: 1998
@@ -399090,15 +398935,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7944
   authors:
-  - ΑΝΥΦΑΝΤΗΣ ΓΙΩΡΓΟΣ
+  - ΑΝΥΦΑΝΤΗΣ,ΓΙΩΡΓΟΣ
   language: el
   title: ΤΟ ΔΩΡΟ ΤΟΥ ΠΟΝΟΥ
   dewey: 889.1 ΑΝΥ
   entry_numbers:
   - '4739'
   editor: None // ΚΑΡΔΙΤΣΑ
   edition_year: 1997
@@ -399140,15 +398985,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7945
   authors:
-  - ΑΝΤΩΝΟΠΟΥΛΟΣ ΚΟΣΜΑΣ
+  - ΑΝΤΩΝΟΠΟΥΛΟΣ,ΚΟΣΜΑΣ
   language: el
   title: ΦΩΣ ΚΑΙ ΦΩΝΗ ΑΠΟ ΤΗΝ ΕΛΛΗΝΙΚΗ ΖΩΗ
   dewey: 889.1 ΑΝΤ
   entry_numbers:
   - '3706'
   pages: 112
   topics:
@@ -399188,15 +399033,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7946
   authors:
-  - ΑΒΕΛΙΟΣ ΑΘΑΝΑΣΙΟΣ
+  - ΑΒΕΛΙΟΣ,ΑΘΑΝΑΣΙΟΣ
   language: el
   title: Ο ΠΟΙΗΤΗΣ ΑΘΑΝΑΣΙΟΣ ΑΒΕΛΛΙΟΣ ΚΑΙ Η ΚΡΙΤΙΚΗ
   dewey: 889.1 ΑΒΕ
   entry_numbers:
   - '5379'
   editor: ΜΑΥΡΙΔΗΣ // ΑΘΗΝΑ
   edition_year: 2000
@@ -399584,15 +399429,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7954
   authors:
-  - ΒΑΙΤΣΗΣ ΚΩΣΤΑΣ-ΤΡΑΧΑΝΑΣ ΚΩΣΤΑΣ
+  - ΒΑΙΤΣΗΣ,ΚΩΣΤΑΣ
+  - ΤΡΑΧΑΝΑΣ,ΚΩΣΤΑΣ
   language: el
   title: ΠΡΩΤΗ ΛΟΓΟΤΕΧΝΙΚΗ ΣΥΝΑΝΤΗΣΗ
   dewey: 889.1 ΒΑΙ
   entry_numbers:
   - '5319'
   pages: 32
   topics:
@@ -399631,15 +399477,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7955
   authors:
-  - ARGHEZI TUDOR
+  - ARGHEZI,TUDOR
   language: el
   title: ΠΟΙΗΜΑΤΑ
   dewey: 859.13 ARG
   entry_numbers:
   - '1295'
   translators:
   - ΜΠΟΥΜΗ-ΠΑΠΑ,ΡΙΤΑ
@@ -400328,15 +400174,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7969
   authors:
-  - ΑΝΔΡΕΟΥ ΑΥΓΕΡΙΝΟΣ
+  - ΑΝΔΡΕΟΥ,ΑΥΓΕΡΙΝΟΣ
   language: el
   title: ΚΟΚΚΙΝΗ ΠΕΤΡΑ
   dewey: 889.1 ΑΝΔ
   entry_numbers:
   - '9897'
   editor: ΜΑΡΚΑΚΗ // ΑΘΗΝΑ
   edition_year: 2011
@@ -400724,15 +400570,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7977
   authors:
-  - ΒΛΑΧΟΠΑΝΟΣ ΔΗΜΗΤΡΗΣ
+  - ΒΛΑΧΟΠΑΝΟΣ,ΔΗΜΗΤΡΗΣ
   language: el
   title: ΛΙΓΟ ΠΡΙΝ ΤΑ ΣΥΝΝΕΦΑ
   dewey: 889.21 ΒΛΑ
   entry_numbers:
   - '10396'
   editor: ΕΜΠΕΙΡΙΑ // ΑΘΗΝΑ
   edition_year: 2011
@@ -400778,15 +400624,15 @@
 - dbase_number: 7978
   authors:
   - ΧΟΚ ΙΘΑΝ
   language: el
   title: ΑΛΗΘΙΝΗ ΑΓΑΠΗ
   dewey: 810.11 ΧΟΚ
   entry_numbers:
-  - 9220Α
+  - 09220
   translators:
   - ΚΟΥΜΟΥΤΣΗ,ΠΕΡΣΑ
   editor: ΕΜΠΕΙΡΙΑ // ΑΘΗΝΑ
   edition_year: 2003
   pages: 267
   topics:
   - ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -400795,15 +400641,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 7978
     1: ΧΟΚ ΙΘΑΝ
     2: ΑΛΗΘΙΝΗ ΑΓΑΠΗ
     4: 810.11ΧΟΚ
-    5: 9220Α
+    5: 09220
     6: ΠΕΡΣΑ ΚΟΥΜΟΥΤΣΗ
     8: ΕΜΠΕΙΡΙΑ
     9: ΑΘΗΝΑ
     10: '2003'
     11: 267Σ
     12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -401463,15 +401309,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7992
   authors:
-  - ΑΘΑΝΑΣΙΑΔΗΣ ΤΑΣΟΣ
+  - ΑΘΑΝΑΣΙΑΔΗΣ,ΤΑΣΟΣ
   language: el
   title: ΜΕΣΑΙΩΝΙΚΟ ΤΡΙΠΤΥΧΟ
   dewey: 889.21 ΑΘΑ
   entry_numbers:
   - '9506'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 1998
@@ -401663,15 +401509,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 7996
   authors:
-  - ΒΑΣΙΛΙΚΟΣ ΒΑΣΙΛΗΣ
+  - ΒΑΣΙΛΙΚΟΣ,ΒΑΣΙΛΗΣ
   language: el
   title: 25ΕΤΙΑ
   dewey: 889.21 ΒΑΣ
   entry_numbers:
   - '9521'
   editor: ΠΑΠΑΖΗΣΗ // ΑΘΗΝΑ
   edition_year: 1976
@@ -403199,15 +403045,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8027
   authors:
-  - ΑΛΤΕΡ,ΜΑΡΕΚ
+  - HALTER,MAREK
   language: el
   title: ΣΙΑΡΡΑ
   subtitle: ΓΥΝΑΙΚΕΣ ΤΗΣ ΒΙΒΛΟΥ
   entry_numbers:
   - '19620'
   translators:
   - ΠΑΛΛΑΝΤΙΟΥ,ΛΗΔΑ
@@ -403347,15 +403193,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8030
   authors:
-  - ΒΛΑΧΟΠΑΝΟΣ ΔΗΜΗΤΡΗΣ
+  - ΒΛΑΧΟΠΑΝΟΣ,ΔΗΜΗΤΡΗΣ
   language: el
   title: ΤΟΥ ΕΡΩΤΑ ΚΑΙ ΤΟΥ ΜΥΘΟΥ
   dewey: 889.1 ΒΛΑ
   entry_numbers:
   - '9450'
   editor: ΠΛΑΝΟΔΙΟΝ // ΑΘΗΝΑ
   edition_year: 2009
@@ -403742,15 +403588,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8038
   authors:
-  - ΑΝΔΡΕΟΥ ΑΥΓΕΡΙΝΟΣ
+  - ΑΝΔΡΕΟΥ,ΑΥΓΕΡΙΝΟΣ
   language: el
   title: ΑΝΤΙΣΤΡΟΦΕΣ
   dewey: 889.1 ΑΝΔ
   entry_numbers:
   - '7676'
   editor: ΑΡΕΝΖΟ // ΑΘΗΝΑ
   edition_year: 2001
@@ -403990,15 +403836,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8043
   authors:
-  - ΒΟΥΛΓΑΡΑΚΗΣ ΓΙΩΡΓΟΣ
+  - ΒΟΥΛΓΑΡΑΚΗΣ,ΓΙΩΡΓΟΣ
   language: el
   title: Η ΦΟΡΑ ΤΩΝ ΠΡΑΓΜΑΤΩΝ
   dewey: 889.1 ΒΟΥ
   entry_numbers:
   - '8236'
   editor: ΖΑΧΑΡΟΠΟΥΛΟΣ // ΑΘΗΝΑ
   pages: 64
@@ -404282,15 +404128,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8049
   authors:
-  - ΑΝΑΣΤΑΣΟΠΟΥΛΟΥ-ΚΑΡΥΔΗ ΓΙΩΤΑ
+  - ΑΝΑΣΤΑΣΟΠΟΥΛΟΥ-ΚΑΡΥΔΗ,ΓΙΩΤΑ
   language: el
   title: ΣΤΗ ΛΑΜΨΗ ΟΥ ΦΕΓΓΑΡΙΟΥ
   dewey: 889.1 ΑΝΑ
   entry_numbers:
   - '9574'
   editor: ΘΟΥΚΙΔΙΔΗΣ // ΑΘΗΝΑ
   edition_year: 1990
@@ -405570,15 +405416,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8075
   authors:
-  - ΒΟΥΡΛΕΚΗ ΓΑΛΑΝΑΚΗ ΑΝΤΙΓΟΝΗ
+  - ΒΒΟΥΡΛΕΚΗ-ΓΑΛΑΝΑΚΗ,ΑΝΤΙΓΟΝΗ
   language: el
   title: ΕΥΘΕΙΕΣ ΚΑΙ ΚΑΜΠΥΛΕΣ
   dewey: 889.1 ΒΟΥ
   entry_numbers:
   - '9975'
   editor: ΜΑΥΡΙΔΗΣ // ΑΘΗΝΑ
   edition_year: 1965
@@ -406419,41 +406265,43 @@
   authors:
   - ΔΡΑΚΟΠΟΥΛΟΣ ΓΕΩΡΓΙΟΣ ΚΥΡΙΑΚΟΣ
   language: el
   title: ΑΙΣΘΗΤΙΚΗ ΑΓΩΓΗ ΤΗΣ ΤΗΛΕΟΡΑΣΗΣ
   dewey: 800.203 ΔΡΑ
   entry_numbers:
   - '7984'
-  - 9276Α
+  - 09276
   edition: '1'
   editor: ΚΑΜΙΝΑ // ΙΩΑΝΝΙΝΑ
   edition_year: 1976
   pages: 104
-  topics: []
+  topics:
+  - ΤΗΛΕΟΡΑΣΗ
+  - ΑΙΣΘΗΤΙΚΗ ΑΓΩΓΗ
   copies: 4
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8092
     1: ΔΡΑΚΟΠΟΥΛΟΣ ΓΕΩΡΓΙΟΣ ΚΥΡΙΑΚΟΣ
     2: ΑΙΣΘΗΤΙΚΗ ΑΓΩΓΗ ΤΗΣ ΤΗΛΕΟΡΑΣΗΣ
     4: 800.203ΔΡΑ
-    5: 7984-9276Α
+    5: 7984-09276
     7: ΠΡΩΤΗ
     8: ΚΑΜΙΝΑ
     9: ΙΩΑΝΝΙΝΑ
     10: '1976'
     11: '104'
+    12: ΤΗΛΕΟΡΑΣΗ
+    13: ΑΙΣΘΗΤΙΚΗ ΑΓΩΓΗ
+    14: ΤΗΛΕΟΡΑΣΗ
     17: 4 ΑΝΤΙΤΥΠΑ
     3: null
     6: null
-    12: null
-    13: null
-    14: null
     15: null
     16: null
     18: null
     19: null
     20: null
     21: null
     22: null
@@ -406473,15 +406321,17 @@
   dewey: 800.203 ΔΡΑ
   entry_numbers:
   - '9275'
   edition: Β
   editor: ΧΑΡΤΟΤΥΠΟΓΡΑΦΙΚΗ // ΑΓΡΙΝΙΟ
   edition_year: 1969
   pages: 120
-  topics: []
+  topics:
+  - ΜΟΥΣΙΚΕΣ ΤΕΧΝΕΣ
+  - ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
   copies: 2
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8093
     1: ΔΡΑΚΟΠΟΥΛΟΣ ΓΕΩΡΓΙΟΣ ΚΥΡΙΑΚΟΣ
@@ -406489,19 +406339,19 @@
     4: 800.203ΔΡΑ
     5: '9275'
     7: Β
     8: ΧΑΡΤΟΤΥΠΟΓΡΑΦΙΚΗ
     9: ΑΓΡΙΝΙΟΧΑΡ
     10: '1969'
     11: 120Σ
+    12: ΜΟΥΣΙΚΕΣ ΤΕΧΝΕΣ
+    13: ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
     17: 2 ΑΝΤΙΤΥΠΑ
     3: null
     6: null
-    12: null
-    13: null
     14: null
     15: null
     16: null
     18: null
     19: null
     20: null
     21: null
@@ -407393,15 +407243,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8112
   authors:
-  - ΑΝΔΡΕΟΥ ΑΥΓΕΡΙΝΟΣ
+  - ΑΝΔΡΕΟΥ,ΑΥΓΕΡΙΝΟΣ
   language: el
   title: ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
   dewey: 782.42 ΑΝΔ
   entry_numbers:
   - '9463'
   editor: ΙΑΜΒΟΣ // ΑΘΗΝΑ
   edition_year: 2010
@@ -407680,15 +407530,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8118
   authors:
-  - ΒΑΒΛΙΔΑΣ ΑΘΑΝΑΣΙΟΣ
+  - ΒΑΒΛΙΔΑΣ,ΑΘΑΝΑΣΙΟΣ
   language: el
   title: Η ΜΟΥΣΙΚΗ ΤΟΥ ΧΡΟΝΟΥ
   dewey: 782.42 ΒΑΒ
   entry_numbers:
   - '5119'
   editor: ΝΙΚΟΛΑΙΔΗΣ // ΑΘΗΝΑ
   edition_year: 1987
@@ -409048,15 +408898,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8146
   authors:
-  - ΒΑΛΙΝΟΣ ΓΙΑΝΝΗΣ
+  - ΒΑΛΙΝΟΣ,ΓΙΑΝΝΗΣ
   language: el
   title: ΑΧΡΟΝΕΣ ΣΚΕΨΕΙΣ
   subtitle: ΥΠΑΡΞΙΑΚΟ ΤΕΧΝΗΜΑ
   dewey: 880.4 ΒΑΛ
   entry_numbers:
   - '4542'
   editor: Η ΣΕΛΙΣ // ΑΘΗΝΑ
@@ -409096,15 +408946,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8147
   authors:
-  - ΑΝΔΡΕΟΥ ΑΥΓΕΡΙΝΟΣ
+  - ΑΝΔΡΕΟΥ,ΑΥΓΕΡΙΝΟΣ
   language: el
   title: Η 9Η ΙΟΥΛΙΟΥ ΤΟΥ 1981 ΕΝ ΛΕΥΚΩΣΙΑ Η ΤΟ ΤΡΑΓΟΥΔΙΝ ΤΟΥ ΚΥΠΡΙΑΝ
   subtitle: ΟΥ
   dewey: 889.1 ΑΝΔ
   entry_numbers:
   - '9639'
   editor: None // ΑΘΗΝΑ
@@ -409243,15 +409093,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8150
   authors:
-  - ΑΒΛΙΔΑΣ ΑΘΑΝΑΣΙΟΣ
+  - ΑΒΛΙΔΑΣ,ΑΘΑΝΑΣΙΟΣ
   language: el
   title: ΕΤΗ ΚΑΙ ΕΤΗ ΕΝ ΠΟΙΗΣΗ
   dewey: 880.9 ΑΒΛ
   entry_numbers:
   - '5118'
   editor: ΔΩΔΩΝΗ // ΙΩΑΝΝΙΝΑ
   edition_year: 1990
@@ -409442,15 +409292,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8154
   authors:
-  - ΑΥΓΕΡΗΣ ΜΑΡΚΟΣ
+  - ΑΥΓΕΡΗΣ,ΜΑΡΚΟΣ
   language: el
   title: ΑΠΑΝΤΑ
   dewey: 889.109 ΑΥΓ
   entry_numbers:
   - '84'
   editor: ΝΕΑ ΤΕΧΝΗ // None
   pages: 415
@@ -409836,15 +409686,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8162
   authors:
-  - ΒΑΛΕΤΑΣ Γ.
+  - ΒΑΛΕΤΑΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΤΕΡΤΣΕΤΗΣ
   subtitle: ΑΠΑΝΤΑ
   dewey: 889.21 ΒΑΛ
   entry_numbers:
   - '74'
   editor: ΠΗΓΗ // ΑΘΗΝΑ
@@ -409885,15 +409735,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8163
   authors:
-  - ΒΟΥΤΗΡΑΣ ΔΗΜΟΣΘΕΝΗΣ
+  - ΒΟΥΤΥΡΑΣ,ΔΗΜΟΣΘΕΝΗΣ
   language: el
   title: ΑΠΑΝΤΑ
   dewey: 889.41 ΒΟΥ
   entry_numbers:
   - '90'
   editor: ΔΙΦΡΟΣ // ΑΘΗΝΑ
   edition_year: 1960
@@ -410173,15 +410023,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8169
   authors:
-  - ΒΗΛΑΡΑΣ ΙΩΑΝΝΗΣ
+  - ΒΗΛΑΡΑΣ,ΙΩΑΝΝΗΣ
   language: el
   title: ΑΠΑΝΤΑ
   dewey: 880.08 ΒΗΛ
   entry_numbers:
   - '73'
   editor: ΠΑΝΕΚΔΟΤΙΚΗ // ΑΘΗΝΑ
   edition_year: 1962
@@ -410900,15 +410750,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8184
   authors:
-  - ΒΑΓΕΝΑΣ ΝΑΣΟΣ
+  - ΒΑΓΕΝΑΣ,ΝΑΣΟΣ
   language: el
   title: ΜΕΛΕΤΗΜΑΤΑ
   dewey: '880.08'
   entry_numbers:
   - '10476'
   editor: ΤΡΑΠΕΖΑ ΑΤΤΙΚΗΣ // ΑΘΗΝΑ
   edition_year: 2004
@@ -411189,15 +411039,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8190
   authors:
-  - ΑΓΑΠΗΤΟΣ ΙΩΣΗΦ
+  - ΑΓΑΠΗΤΟΣ,ΙΩΣΗΦ
   language: el
   title: Ο ΤΡΥΦΕΡΟΣ ΚΛΕΦΤΗΣ
   dewey: 808.899 ΑΓΑ
   entry_numbers:
   - '10467'
   edition: '2'
   editor: ΤΗΣ ΚΑΡΔΙΑΣ // ΑΘΗΝΑ
@@ -411623,15 +411473,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8199
   authors:
-  - ΑΝΤΕΡΣΕΝ ΧΑΝΣ ΚΡΙΣΤΙΑΝ
+  - ANDERSEN,HANS,CHRISTIAN
   language: el
   title: Η ΞΑΝΘΟΜΑΛΛΗ ΣΕΙΡΗΝΑ
   subtitle: ΚΑΙ ΑΛΛΑ ΠΑΡΑΜΥΘΙΑ
   dewey: 808.899 ΑΝΤ
   entry_numbers:
   - '10499'
   editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
@@ -411819,15 +411669,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8203
   authors:
-  - ΒΕΡΝ ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: Ο ΘΑΥΜΑΣΙΟΣ ΟΡΕΝΟΚΟΣ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '10502'
   translators:
   - ΨΑΡΡΑΣ,
@@ -411875,30 +411725,30 @@
 - dbase_number: 8204
   authors:
   - ΚΟΚΟΡΕΛΗ ΑΡΓΥΡΩ-ΖΩΡΖ ΣΑΡΗ
   language: el
   title: ΜΙΑ ΑΓΑΠΗ ΓΙΑ ΔΥΟ
   dewey: 808.899 ΚΟΚ
   entry_numbers:
-  - 9201Α
+  - 09201
   edition: '12'
   editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
   edition_year: 2007
   pages: 171
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8204
     1: ΚΟΚΟΡΕΛΗ ΑΡΓΥΡΩ-ΖΩΡΖ ΣΑΡΗ
     2: ΜΙΑ ΑΓΑΠΗ ΓΙΑ ΔΥΟ
     4: 808.899ΚΟΚ
-    5: 9201Α
+    5: 09201
     7: '12'
     8: ΠΑΤΑΚΗ
     9: ΑΘΗΝΑ
     10: '2007'
     11: 171Σ
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -412295,15 +412145,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8213
   authors:
-  - ΑΛΚΟΤ ΛΟΥΙΖΑ
+  - ALCOTT,LOUISA,MAY
   language: el
   title: ΜΙΚΡΕΣ ΚΥΡΙΕΣ
   dewey: 808.899 ΑΛΚ
   entry_numbers:
   - '10504'
   translators:
   - ΤΣΟΥΚΑΛΑ,
@@ -413175,15 +413025,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8231
   authors:
-  - ΒΑUMGART KLAUS
+  - ΒΑUMGART,KLAUS
   title: LAURAS STERN
   dewey: 808.899 BAU
   entry_numbers:
   - '10509'
   editor: BAUMHAUS VERLAG // SINGAPORE
   edition_year: 1999
   pages: 10
@@ -414672,15 +414522,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8262
   authors:
-  - ΑΛΕΞΙΑΔΗΣ ΜΗΝΑΣ
+  - ΑΛΕΞΙΑΔΗΣ,ΜΗΝΑΣ
   language: el
   title: ΟΙ ΕΛΛΗΝΙΚΕΣ ΠΑΡΑΛΛΑΓΕΣ ΓΙΑ ΤΟΝ ΔΡΑΚΟΝΤΟΚΤΟΝΟ ΗΡΩΑ
   dewey: 398 ΑΛΕ
   entry_numbers:
   - '6790'
   editor: None // ΙΩΑΝΝΙΝΑ
   edition_year: 1982
@@ -415197,15 +415047,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8273
   authors:
-  - ΑΝΤΩΝΟΠΟΥΛΟΣ ΚΟΣΜΑΣ
+  - ΑΝΤΩΝΟΠΟΥΛΟΣ,ΚΟΣΜΑΣ
   language: el
   title: ΕΛΛΗΝΙΣΜΟΣ ΚΑΙ ΕΘΝΙΚΕΣ ΠΑΡΑΔΟΣΕΙΣ
   dewey: 398 ΑΝΤ
   entry_numbers:
   - '7681'
   pages: 56
   topics:
@@ -415725,15 +415575,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8284
   authors:
-  - ΒΙΤΑΛΗ ΛΕΙΑ
+  - ΒΙΤΑΛΗ,ΛΕΙΑ
   language: el
   title: ΙΕΡΗ ΠΑΓΙΔΑ
   subtitle: ΤΟ ΑΠΟΚΡΥΦΟ ΧΡΟΝΙΚΟ ΤΗΣ ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗΣ
   dewey: 889.21 ΒΙΤ
   entry_numbers:
   - '9886'
   edition: '2'
@@ -416264,30 +416114,30 @@
     30: null
 - dbase_number: 8295
   authors: []
   language: el
   title: ΗΠΕΙΡΟΣ
   dewey: 398 ΧΣ
   entry_numbers:
-  - 9278Α
+  - 09278
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1978
   pages: 64
   topics:
   - ΛΑΟΓΡΑΦΙΑ
   - ΠΕΡΙΟΔΙΚΗ ΕΚΔΟΣΗ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8295
     1: Χ.Σ.
     2: ΗΠΕΙΡΟΣ
     4: 398 Χ.Σ
-    5: 9278Α
+    5: 09278
     9: ΘΕΣ\ΝΙΚΗ
     10: '1978'
     11: 64Σ
     12: ΛΑΟΓΡΑΦΙΑ
     13: ΠΕΡΙΟΔΙΚΗ ΕΚΔΟΣΗ
     14: ΛΑΟΓΡΑΦΙΑ
     3: null
@@ -416326,15 +416176,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8296
     1: Χ.Σ.
     2: ΗΠΕΙΡΟΣ
-    4: 398 Χ.Σ.
+    4: 398Χ.Σ.
     5: '10544'
     9: ΘΕΣ\ΝΙΚΗ
     10: '1981'
     11: 121Σ
     12: ΠΕΡΙΟΔΙΚΗ ΕΚΔΟΣΗ
     13: ΛΑΟΓΡΑΦΙΑ
     14: ΛΑΟΓΡΑΦΙΑ
@@ -416356,15 +416206,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8297
   authors:
-  - ΑΚΟΓΛΟΥ ΞΕΝΟΦΩΝΤΑΣ
+  - ΑΚΟΓΛΟΥ,ΞΕΝΟΦΩΝΤΑΣ
   language: el
   title: ΑΠΟ ΤΗ ΖΩΗ ΤΟΥ ΠΟΝΤΟΥ
   subtitle: ΛΑΟΓΡΑΦΙΚΑ ΚΟΤΥΩΡΩΝ
   dewey: 398 ΑΚΟ
   entry_numbers:
   - '10545'
   editor: ΞΕΝΟΣ // ΑΘΗΝΑ
@@ -416376,15 +416226,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 8297
     1: ΑΚΟΓΛΟΥ ΞΕΝΟΦΩΝΤΑΣ
     2: ΑΠΟ ΤΗ ΖΩΗ ΤΟΥ ΠΟΝΤΟΥ
     3: ΛΑΟΓΡΑΦΙΚΑ ΚΟΤΥΩΡΩΝ
-    4: 398 ΑΚΟ
+    4: 398ΑΚΟ
     5: '10545'
     8: ΞΕΝΟΣ
     9: ΑΘΗΝΑ
     10: '1939'
     11: 532Σ
     12: ΛΑΟΓΡΑΦΙΑ
     13: ΛΑΟΓΡΑΦΙΑ
@@ -416423,15 +416273,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8298
     1: ΜΕΡΑΝΤΖΑΣ ΧΡΗΣΤΟΣ
     2: ΠΡΑΚΤΙΚΑ Α ΕΠΙΣΤΗΜΟΝΙΚΟΥ ΣΥΝΕΔΡΙΟΥ ΓΙΑ ΤΑ ΤΖΟΥΜΕΡΚΑ
-    4: 398 ΜΕΡ
+    4: 398ΜΕΡ
     5: '10546'
     8: ΙΚΛΕΤ
     9: ΙΩΑΝΝΙΝΑ
     10: '2008'
     11: 512Σ
     12: ΛΑΟΓΡΑΦΙΑ
     13: ΛΑΟΓΡΑΦΙΑ
@@ -416453,15 +416303,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8299
   authors:
-  - ΑΥΔΙΚΟΣ ΕΥΑΓΓΕΛΟΣ
+  - ΑΥΔΙΚΟΣ,ΕΥΑΓΓΕΛΟΣ
   language: el
   title: ΠΡΕΒΕΖΑ
   subtitle: 1945-1990
   dewey: 398 ΑΥΔ
   entry_numbers:
   - '9550'
   editor: ΔΗΜΟΣ ΠΡΕΒΕΖΑΣ // ΠΡΕΒΕΖΑ
@@ -416473,15 +416323,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 8299
     1: ΑΥΔΙΚΟΣ ΕΥΑΓΓΕΛΟΣ
     2: ΠΡΕΒΕΖΑ
     3: 1945-1990
-    4: 398 ΑΥΔ
+    4: 398ΑΥΔ
     5: '9550'
     8: ΔΗΜΟΣ ΠΡΕΒΕΖΑΣ
     9: ΠΡΕΒΕΖΑ
     10: '2000'
     11: 457Σ
     12: ΛΑΟΓΡΑΦΙΑ
     13: ΛΑΟΓΡΑΦΙΑ
@@ -416518,15 +416368,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8300
     1: Χ.Σ.
     2: ΣΑΡΑΚΑΤΣΑΝΟΙ
-    4: 398 Χ.Σ.
+    4: 398Χ.Σ.
     5: '9899'
     8: ΠΗΓΑΣΟΣ
     11: 142Σ
     12: ΛΑΟΓΡΑΦΙΑ
     13: ΛΑΟΓΡΑΦΙΑ
     14: ΛΑΟΓΡΑΦΙΑ
     3: null
@@ -416568,15 +416418,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 8301
     1: ΚΟΛΙΟΣ ΑΠΟΣΤΟΛΟΣ
     2: ΛΕΛΟΒΑ 1941
     3: ΕΝΑΣ ΠΑΠΠΟΥΣ ΘΥΜΑΤΑΙ
-    4: 398 ΚΟΛ
+    4: 398ΚΟΛ
     5: '10549'
     8: ΡΟΚΟΣ
     9: ΠΡΕΒΕΖΑ
     10: '2009'
     11: 102Σ
     12: ΛΑΟΓΡΑΦΙΑ
     13: ΛΑΟΓΡΦΑΙΑ
@@ -416597,15 +416447,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8302
   authors:
-  - ΒΙΓΛΑΣ ΙΩΑΝΝΗΣ
+  - ΒΙΓΛΑΣ,ΙΩΑΝΝΗΣ
   language: el
   title: ΣΑΡΑΝΤΑΠΕΝΤΕ ΓΙΑΝΝΗΔΕΣ...
   subtitle: ΗΘΟΓΡΑΦΙΑ
   dewey: 398 ΒΙΓ
   entry_numbers:
   - '10548'
   editor: ΓΡΑΦΙΚΕΣ ΤΕΧΝΕΣ // ΑΘΗΝΑ
@@ -416617,15 +416467,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 8302
     1: ΒΙΓΛΑΣ ΙΩΑΝΝΗΣ
     2: ΣΑΡΑΝΤΑΠΕΝΤΕ ΓΙΑΝΝΗΔΕΣ...
     3: ΗΘΟΓΡΑΦΙΑ
-    4: 398 ΒΙΓ
+    4: 398ΒΙΓ
     5: '10548'
     8: ΓΡΑΦΙΚΕΣ ΤΕΧΝΕΣ
     9: ΑΘΗΝΑ
     10: '1995'
     11: 191Σ
     12: ΛΑΟΓΡΑΦΙΑ
     13: ΛΑΟΓΡΑΦΙΑ
@@ -416664,15 +416514,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8303
     1: Χ.Σ.
     2: ΤΖΟΥΜΕΡΚΙΩΤΙΚΑ ΧΡΟΝΙΚΑ
-    4: 398 Χ.Σ.
+    4: 398Χ.Σ.
     5: '10551'
     8: ΝΑΙ
     9: ΙΩΑΝΝΙΝΑ
     10: '2009'
     11: 224Σ
     12: ΛΑΟΓΡΑΦΙΑ
     13: ΠΕΡΙΟΔΙΚΗ ΕΚΔΟΣΗ
@@ -416713,24 +416563,24 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8304
     1: ΜΑΚΡΥΓΙΑΝΝΗΣ ΧΡΗΣΤΟΣ ΚΑΙ ΑΘΑΝΑΣΙΟΣ
     2: ΙΣΤΟΡΙΟΓΡΑΦΙΑ ΤΗΣ ΠΙΝΔΟΥ
-    4: 398 ΜΑΚ
+    4: 398ΜΑΚ
     5: '10547'
     8: ΔΗΜΟΣ ΑΓΝΑΝΤΩΝ
     9: ΑΘΗΝΑ
     10: '2010'
     11: 252Σ
     12: ΛΑΟΓΡΑΦΙΑ
     13: ΛΑΟΓΡΑΦΙΑ
     14: ΛΑΟΓΡΑΦΙΑ
-    17: 2 αντιτυπα
+    17: 2 ΑΝΤΙΤΥΠΑ
     3: null
     6: null
     7: null
     15: null
     16: null
     18: null
     19: null
@@ -416761,15 +416611,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8305
     1: ΤΣΙΠΑΣ ΝΙΚΟΛΑΟΣ
     2: ΣΕΡΓΙΑΝΙΣΜΑ ΣΤΟΥΣ ΧΩΡΟΥΣ ΚΑΙ ΣΤΗΝ ΙΣΤΟΡΙΑ ΤΗΣ ΠΥΡΣΟΓΙΑΝΝΗΣ
-    4: 398 ΤΣΙ
+    4: 398ΤΣΙ
     5: '10550'
     9: ΜΑΡΟΥΣΙ
     10: '1995'
     11: 143Σ
     12: ΛΑΟΓΡΑΦΙΑ
     13: ΛΑΟΓΡΑΦΙΑ
     14: ΛΑΟΓΡΑΦΙΑ
@@ -416810,15 +416660,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8306
     1: ΚΙΚΟΠΟΥΛΟΣ ΜΕΝΕΛΑΟΣ
     2: ΕΛΑΦΟΤΟΠΟΣ (ΤΣΕΡΒΑΡΙ)
-    4: 398 ΚΙΚ
+    4: 398ΚΙΚ
     5: '5340'
     8: ΔΟΥΒΑΛΗ
     9: ΓΙΑΝΝΕΝΑ
     10: '2000'
     11: 462Σ
     12: ΛΑΟΓΡΑΦΙΑ
     13: ΛΑΟΓΡΑΦΙΑ
@@ -416860,15 +416710,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8307
     1: ΝΙΚΟΛΣ ΚΩΣΤΑ
     2: Ο ΧΟΡΟΣ-Η ΙΣΤΟΡΙΑ ΜΙΑΣ ΤΕΧΝΗΣ:ΤΟ ΜΠΑΛΛΕΤΟ
-    4: 398 ΝΙΚ
+    4: 398ΝΙΚ
     5: '957'
     8: ΔΙΦΡΟΣ
     9: ΑΘΗΝΑ
     10: '1957'
     11: 206Σ
     12: ΜΠΑΛΛΕΤΟ-ΧΟΡΟΣ
     13: ΛΑΟΓΡΑΦΙΑ
@@ -419658,15 +419508,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8365
   authors:
-  - ΑΛΕΞΙΑΔΟΥ ΒΕΦΑ
+  - ΑΛΕΞΙΑΔΟΥ,ΒΕΦΑ
   language: el
   title: ΟΙ 20 ΚΑΛΥΤΕΡΕΣ ΣΥΝΤΑΓΕΣ ΓΡΗΓΟΡΕΣ-ΕΥΚΟΛΕΣ
   dewey: 641.5 ΑΛΕ
   entry_numbers:
   - '10589'
   editor: 7 ΜΕΡΕΣ TV // None
   pages: 15
@@ -419705,15 +419555,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8366
   authors:
-  - ΑΛΕΞΙΑΔΟΥ ΒΕΦΑ
+  - ΑΛΕΞΙΑΔΟΥ,ΒΕΦΑ
   language: el
   title: ΟΙ 20 ΚΑΛΥΤΕΡΕΣ ΣΥΝΤΑΓΕΣ ΓΙΑ ΛΑΧΑΝΙΚΑ
   dewey: 641.5 ΑΛΕ
   entry_numbers:
   - '10590'
   editor: 7 ΜΕΡΕΣ TV // None
   pages: 15
@@ -419752,15 +419602,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8367
   authors:
-  - ΑΛΕΞΙΑΔΟΥ ΒΕΦΑ
+  - ΑΛΕΞΙΑΔΟΥ,ΒΕΦΑ
   language: el
   title: 20+2 ΒΡΑΒΕΥΜΕΝΕΣ ΠΑΡΑΔΟΣΙΑΚΕΣ ΣΥΝΤΑΓΕΣ
   dewey: 641.5 ΑΛΕ
   entry_numbers:
   - '10588'
   editor: 7 ΜΕΡΕΣ TV // None
   pages: 15
@@ -420968,38 +420818,38 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8391
   authors:
-  - ΠΑΜΟΥΚ ΟΡΧΑΝ
+  - ΠΑΜΟΥΚ,ΟΡΧΑΝ
   language: el
   title: ΧΙΟΝΙ
   dewey: 894.35 ΠΑΜ
   entry_numbers:
-  - 9158Α
+  - 09158
   translators:
   - ΒΡΕΤΟΥ,ΣΤΕΛΛΑ
   editor: ΩΚΕΑΝΙΔΑ // ΑΘΗΝΑ
   edition_year: 2007
   pages: 686
   topics:
   - ΤΟΥΡΚΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-410-468-0
   original_entry:
     0: 8391
-    1: ΠΑΜΟΥΚ ΟΡΧΑΝ
+    1: ΠΑΜΟΥΚ,ΟΡΧΑΝ
     2: ΧΙΟΝΙ
     4: 894.35 ΠΑΜ
-    5: 9158Α
+    5: 09158
     6: ΣΤΕΛΛΑ ΒΡΕΤΟΥ
     8: ΩΚΕΑΝΙΔΑ
     9: ΑΘΗΝΑ
     10: '2007'
     11: 686Σ
     12: ΤΟΥΡΚΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΤΟΥΡΚΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -421020,15 +420870,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8392
   authors:
-  - ΚΑΛΠΟΥΖΟΣ ΓΙΑΝΝΗΣ
+  - ΚΑΛΠΟΥΖΟΣ,ΓΙΑΝΝΗΣ
   language: el
   title: ΠΑΝΤΟΜΙΜΑ ΦΑΝΤΑΣΜΑΤΩΝ
   dewey: 889.21 ΚΑΛ
   entry_numbers:
   - '9162'
   editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
   edition_year: 2005
@@ -421038,15 +420888,15 @@
   - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   isbn: 960-422-244-9
   original_entry:
     0: 8392
-    1: ΚΑΛΠΟΥΖΟΣ ΓΙΑΝΝΗΣ
+    1: ΚΑΛΠΟΥΖΟΣ,ΓΙΑΝΝΗΣ
     2: ΠΑΝΤΟΜΙΜΑ ΦΑΝΤΑΣΜΑΤΩΝ
     4: 889.21ΚΑΛ
     5: '9162'
     8: ΑΓΚΥΡΑ
     9: ΑΘΗΝΑ
     10: '2005'
     11: 506Σ
@@ -421070,15 +420920,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8393
   authors:
-  - COELHO PAULO
+  - COELHO,PAULO
   language: el
   title: ΟΙ ΕΞΟΜΟΛΟΓΗΣΕΙΣ ΕΟΣ ΠΡΟΣΚΥΝΗΤΗ
   dewey: 869 COE
   entry_numbers:
   - '9592'
   translators:
   - ΚΑΛΑΤΖΟΠΟΥΛΟΥ,ΚΑΤΕΡΙΝΑ
@@ -421090,15 +420940,15 @@
   - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   isbn: 960-14-0358-2
   original_entry:
     0: 8393
-    1: COELHO PAULO
+    1: COELHO,PAULO
     2: ΟΙ ΕΞΟΜΟΛΟΓΗΣΕΙΣ ΕΟΣ ΠΡΟΣΚΥΝΗΤΗ
     4: 869 COE
     5: '9592'
     6: ΚΑΛΑΤΖΟΠΟΥΛΟΥ ΚΑΤΕΡΙ
     8: ΛΙΒΑΝΗ
     9: ΑΘΗΝΑ
     10: '2001'
@@ -421122,15 +420972,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8394
   authors:
-  - ΠΑΠΑΒΑΣΙΛΕΙΟΥ ΙΩΑΝΝΗΣ
+  - ΠΑΠΑΒΑΣΙΛΕΙΟΥ,ΙΩΑΝΝΗΣ
   language: el
   title: Η ΕΘΝΙΚΗ ΜΑΣ ΓΛΩΣΣΑ
   subtitle: ΜΙΚΡΗ ΙΣΤΟΡΙΚΗ ΑΝΑΔΡΟΜΗ
   dewey: 938.031 ΠΑΠ
   entry_numbers:
   - '2861'
   - '2862'
@@ -421140,15 +420990,15 @@
   topics: []
   copies: 2
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8394
-    1: ΠΑΠΑΒΑΣΙΛΕΙΟΥ ΙΩΑΝΝΗΣ
+    1: ΠΑΠΑΒΑΣΙΛΕΙΟΥ,ΙΩΑΝΝΗΣ
     2: Η ΕΘΝΙΚΗ ΜΑΣ ΓΛΩΣΣΑ
     3: ΜΙΚΡΗ ΙΣΤΟΡΙΚΗ ΑΝΑΔΡΟΜΗ
     4: 938.031ΠΑΠ
     5: 2861-2862
     9: ΑΘΗΝΑ
     10: '1971'
     11: 31Σ
@@ -421172,15 +421022,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8395
   authors:
-  - ΓΟΥΕΣΤΕΡΦΕΛΝΤ ΣΚΟΤ
+  - ΓΟΥΕΣΤΕΡΦΕΛΝΤ,ΣΚΟΤ
   title: UGLIES
   dewey: 810.11 ΓΟΥ
   entry_numbers:
   - '10620'
   translators:
   - ΟΙΚΟΝΟΜΟΥ,ΚΑΙΤΗ
   editor: ΜΕΤΑΙΧΜΙΟ // ΑΘΗΝΑ
@@ -421192,17 +421042,17 @@
   copies: 2
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-455-674-8
   original_entry:
     0: 8395
-    1: ΓΟΥΕΣΤΕΡΦΕΛΝΤ ΣΚΟΤ
+    1: ΓΟΥΕΣΤΕΡΦΕΛΝΤ,ΣΚΟΤ
     2: UGLIES
-    4: 810.11 ΓΟΥ
+    4: 810.11ΓΟΥ
     5: '10620'
     6: ΟΙΚΟΝΟΜΟΙ ΚΑΙΤΗ
     8: ΜΕΤΑΙΧΜΙΟ
     9: ΑΘΗΝΑ
     10: '2009'
     11: 462Σ
     12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
@@ -421224,15 +421074,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8396
   authors:
-  - ΠΑΧΟΡ ΠΟΡΙΣ
+  - ΠΑΧΟΡ,ΠΟΡΙΣ
   language: el
   title: ΑΠΑΓΟΡΕΥΕΤΑΙ ΤΟ ΟΜΙΛΕΙΝ
   dewey: 891.84 ΠΑΧ
   entry_numbers:
   - '10619'
   translators:
   - ΒΕΚΙΑΡΕΛΛΗ,ΤΕΡΕΖΑ
@@ -421245,15 +421095,15 @@
   - '2'
   copies: 2
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8396
-    1: ΠΑΧΟΡ ΠΟΡΙΣ
+    1: ΠΑΧΟΡ,ΠΟΡΙΣ
     2: ΑΠΑΓΟΡΕΥΕΤΑΙ ΤΟ ΟΜΙΛΕΙΝ
     4: 891.84ΠΑΧ
     5: '10619'
     6: ΤΕΡΕΖΑ ΒΕΚΙΑΡΗΛΛΗ
     8: ΜΕΤΑΙΧΜΙΟ
     9: ΑΘΗΝΑ
     10: '2009'
@@ -421277,15 +421127,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8397
   authors:
-  - ΓΚΟΝΤΕ ΛΟΡΑΝ
+  - ΓΚΟΝΤΕ,ΛΟΡΑΝ
   language: el
   title: Η ΠΥΛΗ ΤΗΣ ΚΟΛΑΣΕΩΣ
   dewey: 843 ΓΚΟ
   entry_numbers:
   - '10618'
   translators:
   - ΣΙΟΥΓΓΑΡΗ,ΕΥΗ
@@ -421298,17 +421148,17 @@
   copies: 2
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-455-642-7
   original_entry:
     0: 8397
-    1: ΓΚΟΝΤΕ ΛΟΡΑΝ
+    1: ΓΚΟΝΤΕ,ΛΟΡΑΝ
     2: Η ΠΥΛΗ ΤΗΣ ΚΟΛΑΣΕΩΣ
-    4: 843 ΓΚΟ
+    4: 843ΓΚΟ
     5: '10618'
     6: ΕΥΗ ΣΙΟΥΓΓΑΡΗ
     8: ΜΕΤΑΙΧΜΙΟ
     9: ΑΘΗΝΑ
     10: '2008'
     11: 199Σ
     12: ΓΑΛΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
@@ -421330,15 +421180,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8398
   authors:
-  - ΕΛΕΥΘΕΡΙΟΥ ΜΑΝΟΣ
+  - ΕΛΕΥΘΕΡΙΟΥ,ΜΑΝΟΣ
   language: el
   title: Η ΜΕΛΑΓΧΟΛΙΑ ΤΗΣ ΠΑΤΡΙΔΑΣ ΜΕΤΑ ΤΙΣ ΕΙΔΗΣΕΙΣ ΤΩΝ ΟΚΤΩ
   dewey: 889.21 ΕΛΕ
   entry_numbers:
   - '10615'
   editor: ΜΕΤΑΙΧΜΙΟ // ΑΘΗΝΑ
   edition_year: 2007
@@ -421349,17 +421199,17 @@
   copies: 2
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-455-268-9
   original_entry:
     0: 8398
-    1: ΕΛΕΥΘΕΡΙΟΥ ΜΑΝΟΣ
+    1: ΕΛΕΥΘΕΡΙΟΥ,ΜΑΝΟΣ
     2: Η ΜΕΛΑΓΧΟΛΙΑ ΤΗΣ ΠΑΤΡΙΔΑΣ ΜΕΤΑ ΤΙΣ ΕΙΔΗΣΕΙΣ ΤΩΝ ΟΚΤΩ
-    4: 889.21 ΕΛΕ
+    4: 889.21ΕΛΕ
     5: '10615'
     8: ΜΕΤΑΙΧΜΙΟ
     9: ΑΘΗΝΑ
     10: '2007'
     11: 235Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -421381,15 +421231,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8399
   authors:
-  - ΑΚΡΙΒΟΣ ΚΩΣΤΑΣ
+  - ΑΚΡΙΒΟΣ,ΚΩΣΤΑΣ
   language: el
   title: ΤΕΛΕΤΕΣ ΕΝΗΛΙΚΙΩΣΗΣ
   subtitle: ΜΙΑ ΖΩΗ ΣΕ ΔΕΚΑΕΦΤΑ ΕΠΕΙΣΟΔΙΑ
   dewey: 889.21 ΑΚΡ
   entry_numbers:
   - '10621'
   - '16720'
@@ -421402,15 +421252,15 @@
   copies: 2
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-455-536-9
   original_entry:
     0: 8399
-    1: ΑΚΡΙΒΟΣ ΚΩΣΤΑΣ
+    1: ΑΚΡΙΒΟΣ,ΚΩΣΤΑΣ
     2: ΤΕΛΕΤΕΣ ΕΝΗΛΙΚΙΩΣΗΣ
     3: ΜΙΑ ΖΩΗ ΣΕ ΔΕΚΑΕΦΤΑ ΕΠΕΙΣΟΔΙΑ
     4: 889.21ΑΚΡ
     5: 10621-16720
     8: ΜΕΤΑΙΧΜΙΟ
     9: ΑΘΗΝΑ
     10: '2009'
@@ -421434,15 +421284,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8400
   authors:
-  - ΕΛΕΥΘΕΡΙΟΥ ΜΑΝΟΣ
+  - ΕΛΕΥΘΕΡΙΟΥ,ΜΑΝΟΣ
   language: el
   title: ΑΝΘΡΩΠΟΣ ΣΤΟ ΠΗΓΑΔΙ
   dewey: 889.21 ΕΛΕ
   entry_numbers:
   - '10622'
   editor: ΜΕΤΑΙΧΜΙΟ // ΑΘΗΝΑ
   edition_year: 2008
@@ -421452,17 +421302,17 @@
   - ΜΥΘΙΣΤΟΡΗΜΑ
   copies: 2
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8400
-    1: ΕΛΕΥΘΕΡΙΟΥ ΜΑΝΟΣ
+    1: ΕΛΕΥΘΕΡΙΟΥ,ΜΑΝΟΣ
     2: ΑΝΘΡΩΠΟΣ ΣΤΟ ΠΗΓΑΔΙ
-    4: 889.21 ΕΛΕ
+    4: 889.21ΕΛΕ
     5: '10622'
     8: ΜΕΤΑΙΧΜΙΟ
     9: ΑΘΗΝΑ
     10: '2008'
     11: 267Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
     13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -421484,15 +421334,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8401
   authors:
-  - ΝΤΕΙΒΙΝΤΣΟΝ ΙΑΝ
+  - ΝΤΕΙΒΙΝΤΣΟΝ,ΙΑΝ
   language: el
   title: ΤΑ ΤΕΛΕΥΤΑΙΑ ΧΡΟΝΙΑ ΤΟΥ ΒΟΛΤΑΙΡΟΥ
   dewey: 190 NTE
   entry_numbers:
   - '10613'
   translators:
   - ΠΡΟΔΡΟΜΙΔΟΥ,ΝΙΚΗ
@@ -421505,17 +421355,17 @@
   copies: 2
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-455-649-6
   original_entry:
     0: 8401
-    1: ΝΤΕΙΒΙΝΤΣΟΝ ΙΑΝ
+    1: ΝΤΕΙΒΙΝΤΣΟΝ,ΙΑΝ
     2: ΤΑ ΤΕΛΕΥΤΑΙΑ ΧΡΟΝΙΑ ΤΟΥ ΒΟΛΤΑΙΡΟΥ
-    4: 190 NTE
+    4: 190NTE
     5: '10613'
     6: ΝΙΚΗ ΠΡΟΔΡΟΜΙΔΟΥ
     8: ΜΕΤΑΙΧΜΙΟ
     9: ΑΘΗΝΑ
     10: '2008'
     11: 295Σ
     12: ΒΙΟΓΡΑΦΙΑ ΒΟΛΤΑΙΡΟΥ
@@ -421537,15 +421387,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8402
   authors:
-  - FEARN NICHOLAS
+  - FEARN,NICHOLAS
   language: el
   title: ΦΙΛΟΣΟΦΙΑ
   subtitle: ΟΙ ΠΙΟ ΠΡΟΣΦΑΤΕΣ ΑΠΑΝΤΗΣΕΙΣ ΣΤΑ ΑΡΧΑΙΟΤΤΕΡΑ ΕΡΩΤΗΜΑΤΑ
   dewey: 100 FEA
   entry_numbers:
   - '10616'
   translators:
@@ -421558,15 +421408,15 @@
   copies: 2
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-455-670-0
   original_entry:
     0: 8402
-    1: FEARN NICHOLAS
+    1: FEARN,NICHOLAS
     2: ΦΙΛΟΣΟΦΙΑ
     3: ΟΙ ΠΙΟ ΠΡΟΣΦΑΤΕΣ ΑΠΑΝΤΗΣΕΙΣ ΣΤΑ ΑΡΧΑΙΟΤΤΕΡΑ ΕΡΩΤΗΜΑΤΑ
     4: 100FEA
     5: '10616'
     6: ΣΕΒΥ ΣΠΥΡΙΔΟΓΙΑΝΝΑΚΗ
     8: ΜΕΤΑΙΧΜΙΟ
     9: ΑΘΗΝΑ
@@ -421590,15 +421440,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8403
   authors:
-  - JOHNSON GEORGE
+  - JOHNSON,GEORGE
   language: el
   title: ΤΑ ΔΕΚΑ ΠΙΟ ΟΜΟΡΦΑ ΠΕΙΡΑΜΑΤΑ
   dewey: 620.11 JOH
   entry_numbers:
   - '10614'
   translators:
   - ΜΠΑΡΟΥΞΗΣ,ΓΙΩΡΓΟΣ
@@ -421612,17 +421462,17 @@
   copies: 2
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-455-671-7
   original_entry:
     0: 8403
-    1: JOHNSON GEORGE
+    1: JOHNSON,GEORGE
     2: ΤΑ ΔΕΚΑ ΠΙΟ ΟΜΟΡΦΑ ΠΕΙΡΑΜΑΤΑ
-    4: 620.11 JOH
+    4: 620.11JOH
     5: '10614'
     6: ΓΙΩΡΓΟΣ ΜΠΑΡΟΥΞΗΣ
     8: ΜΕΤΑΙΧΜΙΟ
     9: ΑΘΗΝΑ
     10: '2008'
     11: 241Σ
     12: ΕΠΙΣΤΗΜΟΝΙΚΑ- ΦΥΣΙΚΗ
@@ -421666,15 +421516,15 @@
   offprint: false
   ean: 978-960-455-269-6
   original_entry:
     0: 8404
     1: ΤΑΤΣΟΠΟΥΛΟΣ ΠΕΤΡΟΣ
     2: ΝΕΟΕΛΛΗΝΕΣ
     3: ΠΟΡΤΡΕΤΑ
-    4: 889.21 ΤΑΤ
+    4: 889.21ΤΑΤ
     5: '10617'
     8: ΜΕΤΑΙΧΜΙΟ
     9: ΑΘΗΝΑ
     10: '2004'
     11: 383Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΕΤΧΝΙΑ
@@ -421695,15 +421545,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8405
   authors:
-  - ΚΟΥΡΚΟΥΜΕΛΗΣ Ν.Κ.
+  - ΚΟΥΡΚΟΥΜΕΛΗΣ,Ν.Κ.
   language: el
   title: ΠΡΑΚΤΙΚΑ ΗΜΕΡΙΔΩΝ 2009 ΚΑΙ2010
   dewey: 938.101 ΚΟΥ
   entry_numbers:
   - '10623'
   editor: ΦΙΛΟΙ ΒΙΒΛΙΟΘ ΑΛΕΞΑΝ // ΑΘΗΝΑ
   edition_year: 2011
@@ -421712,15 +421562,15 @@
   - ΑΡΧΑΙΑ ΕΛΛΑΔΑ
   - ΠΡΑΚΤΙΚΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 8405
-    1: ΚΟΥΡΚΟΥΜΕΛΗΣ Ν.Κ.
+    1: ΚΟΥΡΚΟΥΜΕΛΗΣ,Ν.Κ.
     2: ΠΡΑΚΤΙΚΑ ΗΜΕΡΙΔΩΝ 2009 ΚΑΙ2010
     4: 938.101ΚΟΥ
     5: '10623'
     8: ΦΙΛΟΙ ΒΙΒΛΙΟΘ ΑΛΕΞΑΝ
     9: ΑΘΗΝΑ
     10: '2011'
     11: 394Σ
@@ -421744,15 +421594,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8406
   authors:
-  - ΣΙΝΓΚΕΡ ΜΠΑΣΕΒΙΤΣ ΙΣΑΑΚ
+  - ΣΙΝΓΚΕΡ,ΜΠΑΣΕΒΙΤΣ ΙΣΑΑΚ
   language: el
   title: ΕΧΘΡΟΙ, ΜΙΑ ΕΡΩΤΙΚΗ ΙΣΤΟΡΙΑ
   dewey: 839.73 ΣΙΝ
   entry_numbers:
   - '10624'
   translators:
   - ΑΜΑΝΑΤΙΔΗΣ,
@@ -421764,17 +421614,17 @@
   - ΜΥΘΙΣΤΟΡΗΜΑ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-03-4872-9
   original_entry:
     0: 8406
-    1: ΣΙΝΓΚΕΡ ΜΠΑΣΕΒΙΤΣ ΙΣΑΑΚ
+    1: ΣΙΝΓΚΕΡ,ΜΠΑΣΕΒΙΤΣ ΙΣΑΑΚ
     2: ΕΧΘΡΟΙ, ΜΙΑ ΕΡΩΤΙΚΗ ΙΣΤΟΡΙΑ
-    4: 839.73 ΣΙΝ
+    4: 839.73ΣΙΝ
     5: '10624'
     6: ΑΜΑΝΑΤΙΔΗΣ
     8: ΚΑΣΤΑΝΙΩΤΗΣ
     9: ΑΘΗΝΑ
     10: '2009'
     11: 308Σ
     12: ΠΟΛΩΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΗΡΜΑ
@@ -421796,15 +421646,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8407
   authors:
-  - ΕΚΟ ΟΥΜΠΕΡΤΟ
+  - ΕΚΟ,ΟΥΜΠΕΡΤΟ
   language: el
   title: ΤΟ ΝΗΣΙ ΤΗΣ ΠΡΟΗΓΟΥΜΕΝΗΣ ΜΕΡΑΣ
   dewey: 850.11 ΕΚΟ
   entry_numbers:
   - '9591'
   translators:
   - ΚΑΛΛΙΦΑΤΙΔΗ,
@@ -421815,17 +421665,17 @@
   - ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   isbn: 960-406-800-8
   original_entry:
     0: 8407
-    1: ΕΚΟ ΟΥΜΠΕΡΤΟ
+    1: ΕΚΟ,ΟΥΜΠΕΡΤΟ
     2: ΤΟ ΝΗΣΙ ΤΗΣ ΠΡΟΗΓΟΥΜΕΝΗΣ ΜΕΡΑΣ
-    4: 850.11 ΕΚΟ
+    4: 850.11ΕΚΟ
     5: '9591'
     6: ΚΑΛΛΙΦΑΤΙΔΗ
     8: ΕΛΛΗΝΙΚΗ ΓΡΑΜΜΑΤΑ
     9: ΑΘΗΝΑ
     10: '2004'
     11: 551ΣΕΛ
     12: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -421847,15 +421697,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8408
   authors:
-  - ΚΟΡΝΑΡΟΣ ΘΕΜΟΣ-ΚΑΖΑΤΖΑΚΗ ΓΑΛΑΤΕΙΑ
+  - ΚΟΡΝΑΡΟΣ,ΘΕΜΟΣ-ΚΑΖΑΤΖΑΚΗ ΓΑΛΑΤΕΙΑ
   language: el
   title: ΤΟ ΝΗΣΙ ΤΩΝ ΣΗΜΑΔΕΜΕΝΩΝ
   subtitle: ΣΠΙΝΑΛΟΓΚΑ-Η ΑΡΡΩΣΤΗ ΠΟΛΙΤΕΙΑ
   dewey: 889.21 ΚΟΡ
   entry_numbers:
   - '10625'
   edition: '4'
@@ -421866,18 +421716,18 @@
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   ean: 978-960-03-5142-2
   original_entry:
     0: 8408
-    1: ΚΟΡΝΑΡΟΣ ΘΕΜΟΣ-ΚΑΖΑΤΖΑΚΗ ΓΑΛΑΤΕΙΑ
+    1: ΚΟΡΝΑΡΟΣ,ΘΕΜΟΣ-ΚΑΖΑΤΖΑΚΗ ΓΑΛΑΤΕΙΑ
     2: ΤΟ ΝΗΣΙ ΤΩΝ ΣΗΜΑΔΕΜΕΝΩΝ
     3: ΣΠΙΝΑΛΟΓΚΑ-Η ΑΡΡΩΣΤΗ ΠΟΛΙΤΕΙΑ
-    4: 88921ΚΟΡ
+    4: 889.21ΚΟΡ
     5: '10625'
     7: '4'
     8: ΚΑΣΤΑΝΙΩΤΗ
     9: ΑΘΗΝΑ
     10: '2010'
     11: 209Σ
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -422236,15 +422086,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8416
   authors:
-  - ΒΛΑΧΟΠΟΥΛΟΥ ΣΤΕΛΛΑ
+  - ΒΛΑΧΟΠΟΥΛΟΥ,ΣΤΕΛΛΑ
   language: el
   title: ΓΟΡΓΟΝΕΣ ΚΑΙ ΝΕΡΑΙΔΕΣ
   dewey: 808.899 ΒΛΑ
   entry_numbers:
   - '10639'
   editor: ΚΕΔΡΟΣ // ΑΘΗΝΑ
   edition_year: 2005
@@ -422285,15 +422135,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8417
   authors:
-  - ΒΛΑΧΟΠΟΥΛΟΥ ΣΤΕΛΛΑ
+  - ΒΛΑΧΟΠΟΥΛΟΥ,ΣΤΕΛΛΑ
   language: el
   title: ΠΑΡΑΞΕΝΑ ΜΥΘΙΚΑ
   dewey: 808.899 ΒΛΑ
   entry_numbers:
   - '10638'
   editor: ΚΕΔΡΟΣ // ΑΘΗΝΑ
   edition_year: 2005
@@ -422333,15 +422183,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8418
   authors:
-  - ΒΛΑΧΟΠΟΥΛΟΥ ΣΤΕΛΛΑ
+  - ΒΛΑΧΟΠΟΥΛΟΥ,ΣΤΕΛΛΑ
   language: el
   title: ΔΩΔΕΚΑ ΘΕΟΙ ΔΩΔΕΚΑ ΑΣΤΕΡΙΣΜΟΙ
   dewey: 808.899 ΒΛΑ
   entry_numbers:
   - '10637'
   editor: ΚΕΔΡΟΣ // ΑΘΗΝΑ
   edition_year: 2005
@@ -422837,15 +422687,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8428
   authors:
-  - ΒΑΦΙΑΣ ΤΑΚΗΣ
+  - ΒΑΦΙΑΣ,ΤΑΚΗΣ,Γ.
   language: el
   title: ΑΝΑΜΝΗΣΕΙΣ ΑΠΟ ΤΗΝ ΠΑΛΙΑ ΑΡΤΑ
   dewey: 938.939 ΒΑΦ
   entry_numbers:
   - '9583'
   editor: None // ΑΡΤΑ
   edition_year: 2010
@@ -423510,15 +423360,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8442
   authors:
-  - ΑΘΑΝΑΣΑΚΗ,ΑΝΤΩΝΙΟΥ
+  - ΑΘΑΝΑΣΑΚΗΣ,ΑΝΤΩΝΗΣ,ΝΙΚΟΛΑΟΥ
   language: el
   title: ΠΕΡΙΛΗΠΤΙΚΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ
   subtitle: ΑΠΟ ΤΟ 1897 ΜΕΧΡΙ ΤΟ 1940-41
   dewey: 938.764 ΑΘΑ
   entry_numbers:
   - '9659'
   editor: ΠΕΤΡΑ // ΑΘΗΝΑ
@@ -423789,15 +423639,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8448
   authors:
-  - ΑΡΚΑΔΙΝΟΣ ΠΟΛΙΒΙΟΣ
+  - ΑΡΚΑΔΙΝΟΣ,ΠΟΛΥΒΙΟΣ
   language: el
   title: Η ΕΣΩΤΕΡΙΚΗ ΚΡΙΣΙΣ ΤΟΥ Κ.Κ.Ε
   dewey: 938.8 ΑΡΚ
   entry_numbers:
   - '9839'
   editor: None // ΑΘΗΝΑ
   edition_year: 1954
@@ -424586,15 +424436,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8465
   authors:
-  - ΒΕΤΣΙΟΣ ΕΛΕΥΘΕΡΙΟΣ
+  - ΒΕΤΣΙΟΣ,ΕΛΕΥΘΕΡΙΟΣ,Λ.
   language: el
   title: ΗΠΕΙΡΩΤΙΚΑ ΧΡΟΝΙΚΑ
   dewey: 938.939 ΒΕΤ
   entry_numbers:
   - '10672'
   editor: None // ΙΩΑΝΝΙΝΑ
   edition_year: 2008
@@ -425111,15 +424961,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8476
   authors:
-  - ΒΑΚΑΛΟΠΟΥΛΟΣ ΚΩΝΣΤΑΝΤΙΝΟΣ
+  - ΒΑΚΑΛΟΠΟΥΛΟΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΙΣΤΟΡΙΑ ΤΟΥ ΒΟΡΕΙΟΥ ΕΛΛΗΝΙΣΜΟΥ ΘΡΑΚΗ
   dewey: 938.695 ΒΑΚ
   entry_numbers:
   - '9305'
   editor: ΚΥΡΙΑΚΙΗΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1993
@@ -426106,15 +425956,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8496
   authors:
-  - ΒΑΣΙΛΕΙΟΥ,ΚΩΝ/ΝΟΣ
+  - ΒΑΣΙΛΕΙΟΥ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΑΡΠΑΚΤΙΚΑ
   dewey: 889.21 ΒΑΣ
   entry_numbers:
   - '10700'
   editor: ΜΠΑΡΤΖΟΥΛΙΑΝΟΣ // ΑΘΗΝΑ
   edition_year: 2006
@@ -426306,15 +426156,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8500
   authors:
-  - ΒΑΣΙΛΕΙΟΥ,ΚΩΝ/ΝΟΣ
+  - ΒΑΣΙΛΕΙΟΥ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: Ο ΑΡΧΑΙΟΚΑΠΗΛΟΣ
   dewey: 889.21 ΒΑΣ
   entry_numbers:
   - '10704'
   editor: ΜΠΑΡΤΖΟΥΛΙΑΝΟΣ // ΑΘΗΝΑ
   edition_year: 2008
@@ -426751,15 +426601,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8509
   authors:
-  - ΑΡΟΥΝΤΑΤΙ,ΡΟΙ
+  - ARUNDHATI,ROY
   language: el
   title: Η ΑΛΓΕΒΡΑ ΤΗΣ ΑΙΩΝΙΑΣ ΔΙΚΑΙΟΣΥΝΗΣ
   entry_numbers:
   - '10724'
   translators:
   - ΚΑΤΣΑΝΗΣ,ΒΑΓΓΕΛΗΣ
   editor: ΨΥΧΟΓΙΟΣ // ΑΘΗΝΑ
@@ -427200,15 +427050,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8518
   authors:
-  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ
+  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ,
   language: el
   title: Ο ΚΥΡΙΟΣ ΜΟΥ ΑΛΚΙΒΙΑΔΗΣ
   dewey: 889.21 ΒΛΑ
   entry_numbers:
   - '10738'
   editor: None // ΑΘΗΝΑ
   edition_year: 2008
@@ -428121,15 +427971,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8536
   authors:
-  - ΑΝΑΣΤΑΣΙΑΔΗΣ,Γ.
+  - ΑΝΑΣΤΑΣΙΑΔΗΣ,ΙΩΑΝΝΗΣ
   language: el
   title: ΝΕΑΝΙΚΑ ΑΝΕΚΔΟΤΑ
   dewey: 808.899 ΑΝΑ
   entry_numbers:
   - '10817'
   editor: ΑΝΑΣΤΑΣΙΑΔΗΣ // ΑΘΗΝΑ
   edition_year: 1994
@@ -428999,15 +428849,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8553
   authors:
-  - ΒΑΦΕΙΑΔΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ Μ.
+  - ΒΑΦΕΙΑΔΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ,Μ.
   language: el
   title: ΠΕΡΙ ΤΗΣ ΕΝ ΑΘΩ <<ΚΡΗΤΙΚΗΣ>>ΖΩΓΡΑΦΙΚΗΣ
   subtitle: ΕΙΚΟΝΕΣ ΚΑΙ ΤΟΙΧΟΓΡΑΦΙΕΣ ΤΗΣ Ι.Μ. ΔΙΟΝΥΣΙΟΥ ΚΑΙ ΟΙ ΔΗΜΙΟΥΡΓΟ
   entry_numbers:
   - '10693'
   editor: ΜΠΑΡΤΖΟΥΛΙΑΝΟΣ // ΑΘΗΝΑ
   edition_year: 2010
@@ -429196,15 +429046,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8557
   authors:
-  - ΑΝΤΩΝΟΠΟΥΛΟΣ ,ΓΙΑΝΝΗΣ
+  - ΑΝΤΩΝΟΠΟΥΛΟΣ,ΓΙΑΝΝΗΣ
   language: el
   title: ΦΟΡΤΙΣΜΕΝΑ ΣΥΝΑΙΣΘΗΜΑΤΑ
   entry_numbers:
   - '10728'
   editor: None // ΑΘΗΝΑ
   edition_year: 2009
   pages: 232
@@ -430608,15 +430458,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8585
   authors:
-  - ΒΟΚΑΚΙΟΣ
+  - BOCCACCIO,GIOVANNI
   language: el
   title: ΔΕΚΑΗΜΕΡΟΝ
   subtitle: ΤΡΙΤΗ ΗΜΕΡΑ
   dewey: 850.11 ΒΟΚ
   entry_numbers:
   - '10839'
   translators:
@@ -431245,15 +431095,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8597
   authors:
-  - ΒΑΝΤΙΜ,ΡΟΖΕ
+  - VADIM,ROGER
   language: el
   title: Ο ΠΕΙΝΑΣΜΕΝΟΣ ΑΓΓΕΛΟΣ
   dewey: 843 ΒΑΝ
   entry_numbers:
   - '10851'
   translators:
   - ΠΑΠΑΓΚΙΚΑ,ΕΥΔΟΚΙΑ
@@ -432635,15 +432485,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8623
   authors:
-  - ΒΟΓΚΤ,ΒΑΝ
+  - VAN VOGT,ALFRED,ELTON
   language: el
   title: ΕΠΙΣΤΗΜΟΝΙΚΗ ΦΑΝΤΑΣΙΑ ΣΛΑΝ
   dewey: 832 ΒΟΓ
   entry_numbers:
   - '10838'
   translators:
   - ΑΡΒΑΝΙΤΗΣ,ΦΟΙΒΟΣ
@@ -432688,15 +432538,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8624
   authors:
-  - ΑΛΕΝΤΕ,ΙΖΑΜΠΕΛ
+  - ALLENDE,ISABEL
   language: el
   title: ΠΑΟΥΛΑ
   dewey: 860.11 ΑΛΙ
   entry_numbers:
   - '10837'
   translators:
   - ΣΩΤΗΡΙΑΔΟΥ-ΜΠΑΡΑΧΑΣ,ΚΛΑΙΤΗ
@@ -434983,15 +434833,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8668
   authors:
-  - ΒΟΝΝΕΓΚΑΤ,ΚΕΡΤ
+  - VONNEGUT,KURT
   language: el
   title: ΕΝΑΣ ΑΝΘΡΩΠΟΣ ΧΩΡΙΣ ΠΑΤΡΙΔΑ
   dewey: 810.11 ΒΟΝ
   entry_numbers:
   - '10920'
   translators:
   - ΓΙΑΝΝΑΚΟΠΟΥΛ,ΘΑΝΑΣΗΣ
@@ -436806,15 +436656,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8703
   authors:
-  - ΑΛΤΟΥΣΕΡ,ΛΟΥΙ
+  - ALTHUSSER,LOUIS
   language: el
   title: ΘΕΣΕΙΣ
   dewey: 330 ΑΛΤ
   entry_numbers:
   - '10952'
   editor: ΘΕΜΕΛΙΟ // None
   edition_year: 1983
@@ -437370,15 +437220,20 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8714
   authors:
-  - ΑΜΙΝ,Σ
+  - ΑΜΙΝ,Σ.
+  - ΑΞΤ,Χ.Γ.
+  - ΑΡΣΕΝΗΣ,Γ.
+  - ΛΑΖΑΡΗΣ,Α.
+  - ΒΕΡΓΟΠΟΥΛΟΣ,Κ.!ΣΑΦΙΕΧ,Α.
+  - ΠΑΠΑΝΔΡΕΟΥ,ΑΝΔΡΕΑΣ
   language: el
   title: ΜΕΤΑΒΑΣΗ ΣΤΟ ΣΟΣΙΑΛΙΣΜΟ
   dewey: 320 ΑΜΙΝ
   entry_numbers:
   - '10939'
   editor: ΑΛΕΤΡΙ // ΑΘΗΝΑ
   edition_year: 1981
@@ -439076,15 +438931,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8747
   authors:
-  - ΑΡΓΥΡΙΟΥ,ΑΛΕΞΑΝΔΡΟΥ
+  - ΑΡΓΥΡΙΟΥ,ΑΛΕΞΑΝΔΡΟΣ
   language: el
   title: Η ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   subtitle: ΝΕΩΤΕΡΙΚΟΙ ΠΟΙΗΤΕΣ ΤΟΥ ΜΕΣΟΠΟΛΕΜΟΥ
   dewey: 880.08 ΑΡΓ
   entry_numbers:
   - '11014'
   editor: ΣΟΚΟΛΗ // ΑΘΗΝΑ
@@ -439128,15 +438983,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8748
   authors:
-  - ΑΡΓΥΡΙΟΥ,ΑΛΕΞΑΝΔΡΟΥ
+  - ΑΡΓΥΡΙΟΥ,ΑΛΕΞΑΝΔΡΟΣ
   language: el
   title: Η ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   subtitle: Η ΠΡΩΤΗ ΜΕΤΑΠΟΛΕΜΙΚΗ ΓΕΝΙΑ
   dewey: 880.08 ΑΡΓ
   entry_numbers:
   - '11015'
   editor: ΣΟΚΟΛΗ // ΑΘΗΝΑ
@@ -439652,15 +439507,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8758
   authors:
-  - ANDERSON.PERRY
+  - ANDERSON,PERRY
   language: el
   title: ΟΙ ΔΙΑΙΡΕΣΕΙΣ ΤΗΣ ΚΥΠΡΟΥ
   dewey: 956.93 AND
   entry_numbers:
   - '11034'
   editor: ΑΓΡΑ // ΑΘΗΝΑ
   edition_year: 2008
@@ -448022,15 +447877,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8922
   authors:
-  - ARNOLO,JOHN H.
+  - ARNOLD,JOHN,H.
   language: el
   title: ΙΣΤΟΡΙΑ
   dewey: 709.38 ARN
   entry_numbers:
   - '11283'
   translators:
   - ΧΕΚΙΜΟΓΛΟΥ,ΕΥΑΓΓΕΛΟΣ
@@ -451108,15 +450963,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 8980
   authors:
-  - ΑΡΕΤΙΝΟ,ΠΙΕΤΡΟ
+  - ARETINO,PIETRO
   language: el
   title: ΤΟ ΣΧΟΛΕΙΟ ΤΗΣ ΠΟΡΝΕΙΑΣ
   dewey: 850.11 ΑΡΕ
   entry_numbers:
   - '11210'
   translators:
   - ΜΠΑΡΟΥΞΗΣ,ΓΙΩΡΓΟΣ
@@ -452270,15 +452125,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9002
   authors:
-  - ΑΡΕΤΙΝΟ,ΠΙΕΤΡΟ
+  - ARETINO,PIETRO
   language: el
   title: Η ΚΡΥΦΗ ΖΩΗ ΤΩΝ ΚΑΛΟΓΡΙΩΝ
   dewey: 850.11 ΑΡΕ
   entry_numbers:
   - '11230'
   translators:
   - ΜΗΤΣΟΜΠΟΝΟΥ,ΑΣΗΜΙΝΑ
@@ -454070,15 +453925,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9037
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: ΣΤΑ ΚΥΜΑΤΑ ΚΑΙ ΣΤΗΝ ΦΩΤΙΑ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '11290'
   translators:
   - ΜΠΑΡΟΥΞΗ,ΤΖΟΥΛΙΑΝΝΑ
@@ -454486,15 +454341,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9045
   authors:
-  - ΑΥΔΗΣ.Λ
+  - ΑΥΔΗΣ,ΛΕΩΝ
   language: el
   title: ΟΙ ΣΥΝΔΙΚΑΛΙΣΤΙΚΕΣ ΕΛΕΥΘΕΡΙΕΣ:ΠΟΙΝΙΚΟΠΟΙΗΣΗ ΑΠΕΡΓΙΩΝ
   dewey: 330 ΑΥΔ
   entry_numbers:
   - '11316'
   - '11772'
   editor: ΟΛΜΕ // ΑΘΗΝΑ
@@ -454539,15 +454394,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 9046
   authors:
-  - ΒΑΚΑΛΙΟΣ,ΘΑΝ.
+  - ΒΑΚΑΛΙΟΣ,ΘΑΝΑΣΗΣ
   language: el
   title: Ο ΚΟΙΝΩΝΙΚΟΣ ΡΟΛΟΣ ΤΟΥ ΕΚΠΑΙΔΕΥΤΙΚΟΥ ΣΤΗ ΣΥΓΧΡΟΝΗ ΕΠΟΧΗ
   dewey: 378 ΒΑΚ
   entry_numbers:
   - '11317'
   editor: ΟΛΜΕ // ΑΘΗΝΑ
   edition_year: 1988
@@ -455401,15 +455256,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9063
   authors:
-  - ANDERSON,LYNN R.
+  - ANDERSON,LYNN,R.
   language: el
   title: ΠΡΟΣΩΠΙΚΟΤΗΤΑ ΚΑΙ ΣΤΑΣΕΙΣ ΤΩΝ ΦΟΙΤΗΤΩΝ ΤΩΝ ΕΛΛΗΝΙΚΩΝ ΑΝΩΤΑΤΩ
   dewey: 378 AND
   entry_numbers:
   - '11331'
   translators:
   - ΑΔΑΜΗ,ΠΑΝΥ
@@ -456961,15 +456816,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9094
   authors:
-  - ΒΑΚΑΛΙΟΣ ΘΑΝΑΣΗΣ
+  - ΒΑΚΑΛΙΟΣ,ΘΑΝΑΣΗΣ
   language: el
   title: Η ΕΠΙΣΤΗΜΟΝΙΚΟ-ΤΕΧΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
   subtitle: Ο ΣΟΣΙΑΛΙΣΜΟΣ ΚΑΙ Ο ΑΝΘΡΩΠΟΣ
   dewey: 320 ΒΑΚ
   entry_numbers:
   - '11431'
   editor: ΘΕΜΕΛΙΟ // ΑΘΗΝΑ
@@ -457643,15 +457498,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9107
   authors:
-  - ΑΔΑΜΙΔΗΣ ΓΙΩΡΓΟΣ Α.
+  - ΑΔΑΜΙΔΗΣ,ΓΙΩΡΓΟΣ,Α.
   language: el
   title: ΒΕΝΕΖΟΥΕΛΑ ΤΟΥ ΟΥΓΚΟ ΤΣΑΒΕΣ
   subtitle: ΟΔΟΙΠΟΡΙΚΟ ΣΤΗ ΒΕΝΕΖΟΥΕΛΑ
   dewey: 320 ΑΔΑ
   entry_numbers:
   - '11430'
   editor: None // ΑΘΗΝΑ
@@ -457749,15 +457604,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9109
   authors:
-  - ΒΑΚΑΛΙΟΣ Θ.
+  - ΒΑΚΑΛΙΟΣ,ΘΑΝΑΣΗΣ
   language: el
   title: ΤΕΧΝΟΛΟΓΙΑ ΚΟΙΝΩΝΙΑ ΠΟΛΙΤΙΣΜΟΣ
   dewey: 303.4 ΒΑΚ
   entry_numbers:
   - '11428'
   editor: ΨΗΦΙΔΑ // ΑΘΗΝΑ
   edition_year: 2002
@@ -459168,15 +459023,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9136
   authors:
-  - ΒΑΒΛΙΔΑ ΑΘΑΝΑΣΙΟΣ
+  - ΒΑΒΛΙΔΑΣ,ΑΘΑΝΑΣΙΟΣ
   language: el
   title: ΚΛΕΙΣΤΟΦΟΒΙΑ
   subtitle: ΤΡΙΠΡΑΚΤΟ ΦΑΝΤΑΣΤΙΚΟ ΔΡΑΜΑ
   dewey: 886.2 ΒΑΒ
   entry_numbers:
   - '11376'
   editor: ΔΩΔΩΝΗ // ΑΘΗΝΑ
@@ -459590,15 +459445,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9144
   authors:
-  - ΑΣΤΕΡΙΟΥ ΕΛΕΝΗ
+  - ΑΣΤΕΡΙΟΥ,ΕΛΕΝΗ
   language: el
   title: ΜΑΡΞΙΣΤΙΚΗ ΣΚΕΨΗ
   dewey: 320 ΑΣΤ
   entry_numbers:
   - '11501'
   editor: ΤΟΠΟΣ // ΑΘΗΝΑ
   edition_year: 2011
@@ -459800,15 +459655,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9148
   authors:
-  - ΑΛΜΠΕΡΤ ΜΙΣΕΛ
+  - MICHELE,ALBERT
   language: el
   title: ΟΥΡΑΝΟΣ ΚΑΙ ΓΗ
   subtitle: ΡΙΖΟΣΠΑΣΤΙΚΟ ΜΑΝΙΦΕΣΤΟ
   dewey: 320 ΑΛΜ
   entry_numbers:
   - '11517'
   translators:
@@ -460008,15 +459863,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 9152
   authors:
-  - ΑΡΝΟΛ ΖΑΚ
+  - ARNAULT,JACQUES
   language: el
   title: ΟΙ ΑΜΕΡΙΚΑΝΟΙ ΕΡΓΑΤΕΣ ΕΙΝΑΙ ΣΥΝΤΗΡΗΤΙΚΟΙ;
   subtitle: ΑΝΑΤΟΜΙΑ ΤΗΣ ΕΡΓΑΤΙΚΗΣ ΤΑΞΗΣ ΤΩΝ ΗΠΑ
   dewey: 330 ΑΡΝ
   entry_numbers:
   - '11427'
   translators:
@@ -461135,15 +460990,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 9174
   authors:
-  - ΑΣΔΡΑΧΑΣ ΣΠΥΡΟΣ Ι.
+  - ΑΣΔΡΑΧΑΣ,ΣΠΥΡΟΣ,Ι.
   language: el
   title: ΕΛΛΗΝΙΚΗ ΚΟΙΝΩΝΙΑ ΚΑΙ ΟΙΚΟΝΟΜΙΑ
   subtitle: ιη ΚΑΙ ιθ ΑΙΩΝΕΣ
   dewey: 945.505 ΑΣΔ
   entry_numbers:
   - '11516'
   editor: ΕΡΜΗΣ // ΑΘΗΝΑ
@@ -461241,15 +461096,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9176
   authors:
-  - ΒΑΚΑΛΙΟΣ ΘΑΝΑΣΗΣ
+  - ΒΑΚΑΛΙΟΣ,ΘΑΝΑΣΗΣ
   language: el
   title: Η ΝΕΑ ΑΝΤΙΛΗΨΗ ΓΙΑ ΤΗ ΣΟΣ/ΚΗ ΕΠΑΝ/ΣΗ ΣΤΙΣ ΣΗΜ/ΝΕΣ ΣΥΝ/ΚΕΣ
   dewey: 320 ΒΑΚ
   entry_numbers:
   - '11505'
   editor: OFFSET // ΑΘΗΝΑ
   edition_year: 1980
@@ -461645,15 +461500,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9184
   authors:
-  - ΑΠΟΣΤΟΛΙΔΟΥ ΒΕΝΕΤΙΑ
+  - ΑΠΟΣΤΟΛΙΔΟΥ,ΒΕΝΕΤΙΑ
   language: el
   title: Ο ΚΩΣΤΗΣ ΠΑΛΑΜΑΣ ΚΑΙ ΤΟ ΠΑΝΕΠΙΣΤΗΜΙΟ
   dewey: 889.106 ΑΠΟ
   entry_numbers:
   - '11467'
   editor: ΠΑΝ/ΜΙΟ:ΙΔΕΟΛΟΓΙΑ // ΑΘΗΝΑ
   edition_year: 1989
@@ -464372,15 +464227,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 9237
   authors:
-  - ΑΠΟΛΛΙΝΑΙΡ,ΓΚΥΓΙΩΜ
+  - APOLLINAIRE,GUILLAUME
   language: el
   title: ΣΑΛΤΙΜΠΑΓΚΟΙ ΚΑΙ ΑΛΛΑ ΠΟΙΗΜΑΤΑ
   dewey: 841.912 ΑΠΟ
   entry_numbers:
   - '11461'
   translators:
   - ΛΙΟΝΤΑΚΗΣ,ΧΡΙΣΤΟΦΟΡΟΣ
@@ -465725,15 +465580,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9263
   authors:
-  - ΑΠΟΣΤΟΛΙΔΗΣ,ΛΟΥΚΑΣ Θ.
+  - ΑΠΟΣΤΟΛΙΔΗΣ,ΛΟΥΚΑΣ,Θ.
   language: el
   title: ΣΥΝΔΙΚΑΛΙΣΤΙΚΗ ΕΚΠΑΙΔΕΥΣΗ ΚΑΙ ΙΝΣΤΙΤΟΥΤΑ ΕΡΓΑΣΙΑΣ[ΕΥΡΩΠΗ-ΕΛΛ
   subtitle: ΛΑΔΑ]
   dewey: 320 ΑΠΟ
   entry_numbers:
   - '11360'
   editor: ΑΙΧΜΗ // ΑΘΗΝΑ
@@ -466248,15 +466103,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 9273
   authors:
-  - ΑΝΔΡΟΝΙΚΟΣ,ΜΑΝΟΛΗΣ
+  - ΑΝΔΡΟΝΙΚΟΣ,ΜΑΝΩΛΗΣ
   language: el
   title: ΕΛΛΗΝΙΚΟΣ ΘΗΣΑΥΡΟΣ
   dewey: 938 ΑΝΔ
   entry_numbers:
   - '11969'
   editor: ΚΑΣΤΑΝΙΩΤΗ // ΑΘΗΝΑ
   edition_year: 1993
@@ -467171,15 +467026,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9291
   authors:
-  - ΑΓΤΖΙΔΗΣ,Β
+  - ΑΓΤΖΙΔΗΣ,ΒΛΑΣΗΣ
   language: el
   title: Ο ΡΟΛΟΣ ΤΗΣ ΟΡΘΟΔΟΞΙΑΣ ΣΤΗ ΝΕΑ ΔΙΕΘΝΗ ΠΡΑΓΜΑΤΙΚΟΤΗΤΑ
   dewey: 230 ΑΓΤ
   entry_numbers:
   - '11600'
   editor: ΓΝΩΣΗ // ΑΘΗΝΑ
   edition_year: 1995
@@ -468311,15 +468166,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9313
   authors:
-  - ΑΣΔΡΑΧΑΣ,ΣΠΥΡΟΣ
+  - ΑΣΔΡΑΧΑΣ,ΣΠΥΡΟΣ,Ι.
   language: el
   title: ΜΗΧΑΝΙΣΜΟΙ ΤΗΣ ΑΓΡΟΤΙΚΗΣ ΟΙΚΟΝΟΜΙΑΣ ΣΤΗΝ ΤΟΥΡΚΡΟΚΡΑΤΙΑ[ΙΕ-ΙΣ
   subtitle: Τ ΑΙΩΝΑΣ]
   dewey: 330 ΑΣΔ
   entry_numbers:
   - '11576'
   editor: ΘΕΜΕΛΙΟ // ΑΘΗΝΑ
@@ -468672,15 +468527,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 9320
   authors:
-  - ΑΠΟΣΤΟΛΟΥ,ΑΠΟΣΤΟΛΟΣ Ε.
+  - ΑΠΟΣΤΟΛΟΥ,ΑΠΟΣΤΟΛΟΣ,Ε.
   language: el
   title: ΣΚΟΡΠΙΑ ΑΠΟ ΤΗΝ ΑΝΤΙΣΤΑΣΗ
   dewey: 938.764 ΑΠΟ
   entry_numbers:
   - '11581'
   editor: ΚΑΠΟΠΟΥΛΟΣ // ΑΘΗΝΑ
   edition_year: 1986
@@ -469364,15 +469219,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9334
   authors:
-  - ΒΙΤΙΝ,Μ
+  - VITIN,MIKHAILGRIGOREVICH
   language: el
   title: ΝΙΚΟΣ ΜΠΕΛΟΓΙΑΝΝΗΣ
   subtitle: ΖΩΗ ΚΑΤΑΠΛΗΚΤΙΚΩΝ ΑΝΘΡΩΠΩΝ
   dewey: 938.764 ΒΙΤ
   entry_numbers:
   - '11622'
   editor: None // ΑΘΗΝΑ
@@ -470347,15 +470202,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9353
   authors:
-  - ΑΝΤΟΡΝΟ,ΤΕΟΝΤΟΡ
+  - ADORNO,THEODOR
   language: el
   title: ΕΠΙΣΤ/ΚΕΣ ΕΜΠΕΙΡΙΕΣ ΕΝΟΣ ΕΥΡΩΠΑΙΟΥ ΔΙΑΝΟΟΥΜΕΝΟΥ ΣΤΗΝ ΑΜΕΡΙΚΗ
   dewey: 193 ΑΝΤ
   entry_numbers:
   - '11630'
   translators:
   - ΓΚΙΝΤΗ,ΒΑΣΩ
@@ -471184,15 +471039,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9369
   authors:
-  - ΒΑΣΙΛΕΙΟΥ,ΝΙΚΟΣ Ν.
+  - ΒΑΣΙΛΕΙΟΥ,ΝΙΚΟΣ,Ν.
   language: el
   title: Ο ΑΝΕΜΟΣ ΣΑΝ ΠΑΡΑΓΟΝΤΑΣ ΚΑΤΑΠΟΝΗΣΗΣ ΤΩΝ ΘΕΡΜΟΚΗΠΙΩΝ
   dewey: 631.583 ΒΑΣ
   entry_numbers:
   - '11661'
   editor: ΑΓΡΟΤΙΚΗ ΤΡΑΠΕΖΑ // ΑΘΗΝΑ
   edition_year: 1987
@@ -471392,15 +471247,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9373
   authors:
-  - ΑΠΟΣΤΟΛΟΥ,ΑΠΟΣΤΟΛΟΣ Ε.
+  - ΑΠΟΣΤΟΛΟΥ,ΑΠΟΣΤΟΛΟΣ,Ε.
   language: el
   title: ΜΝΗΜΕΣ
   dewey: 889.21 ΑΠΟ
   entry_numbers:
   - '11657'
   editor: ΚΑΠΟΠΟΥΛΟΣ // ΑΘΗΝΑ
   edition_year: 1985
@@ -472048,15 +471903,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9386
   authors:
-  - ΑΝΑΣΤΑΣΙΑΔΗ,ΚΥΡΙΑΚΟΥ Κ.
+  - ΑΝΑΣΤΑΣΙΑΔΗΣ,ΚΥΡΙΑΚΟΣ,Κ.
   language: el
   title: ΠΙΝΑΚΕΣ ΑΝΤΙΣΕΙΣΜΙΚΟΥ ΥΠΟΛΟΓΙΣΜΟΥ ΚΕΝΤΡΙΚΩΝ ΠΕΔΙΛΩΝ
   dewey: 624.183 ΑΝΑ
   entry_numbers:
   - '11675'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1970
@@ -474872,15 +474727,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9442
   authors:
-  - ΑΛΤΟΥΣΕΡ,ΛΟΥΙ
+  - ALTHUSSER,LOUIS
   language: el
   title: ΚΡΙΤΙΚΗ ΤΟΥ ΕΡΓΟΥ ΤΟΥ ΛΟΥΙ ΑΛΤΟΥΣΕΡ
   dewey: 320 ΑΛΤ
   entry_numbers:
   - '11726'
   editor: ΘΕΜΕΛΙΟ // ΑΘΗΝΑ
   edition_year: 1977
@@ -476267,15 +476122,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9469
   authors:
-  - ΑΥΔΗΣ,Λ
+  - ΑΥΔΗΣ,ΛΕΩΝ
   language: el
   title: ΟΙ ΣΥΝΔΙΚΑΛΙΣΤΙΚΕΣ ΕΛΕΥΘΕΡΙΕΣ:ΠΟΙΝ/ΠΟΙΗΣΗ ΑΠΕΡΓΙΩΝ.ΔΙΩΞΕΙΣ Α
   subtitle: ΠΕΡΓΩΝ
   dewey: 330 ΑΥΔ
   entry_numbers:
   - '11772'
   editor: ΟΛΜΕ // ΑΘΗΝΑ
@@ -476888,15 +476743,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9481
   authors:
-  - ΑΠΟΣΤΟΛΙΔΗΣ,ΛΟΥΚΑΣ Θ.
+  - ΑΠΟΣΤΟΛΙΔΗΣ,ΛΟΥΚΑΣ,Θ.
   language: el
   title: ΣΥΝΤΑΞΙΟΥΧΟΙ ΚΑΙ ΑΣΦΑΛΙΣΤΙΚΗ ΜΕΤΑΡΡΥΘΜΙΣΗ
   dewey: 330 ΑΠΟ
   entry_numbers:
   - '11760'
   editor: ΚΑΣΤΑΛΙΑ // ΑΘΗΝΑ
   edition_year: 2006
@@ -477042,15 +476897,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9484
   authors:
-  - VILANOVA,MEREDES
+  - VILANOVA,MERCEDES
   language: el
   title: ΟΙ ΑΟΡΑΤΕΣ ΠΛΕΙΟΨΗΦΙΕΣ
   subtitle: ΕΡΓΑΤΙΚΗ ΕΚΜΕΤΑΛΛΕΥΣΗ,ΕΠΑΝΑΣΤΑΣΗ ΚΑΙ ΚΑΤΑΣΤΟΛΗ
   dewey: 330 VIL
   entry_numbers:
   - '11772'
   translators:
@@ -478916,15 +478771,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9521
   authors:
-  - ΒΑΦΙΑ,ΓΡΗΓΟΡΗ
+  - ΒΑΦΙΑΣ,ΓΡΗΓΟΡΗΣ
   language: el
   title: ΟΙ ΠΙΘΗΚΟΙ
   dewey: 886.2 ΒΑΦ
   entry_numbers:
   - '11812'
   editor: ΔΩΔΩΝΗ // ΑΘΗΝΑ
   edition_year: 1991
@@ -482382,15 +482237,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9589
   authors:
-  - ΒΕΓΛΕΡΗ,ΦΑΙΔΩΝΟΣ Θ.
+  - ΒΕΓΛΕΡΗΣ,ΦΑΙΔΩΝ,Θ.
   language: el
   title: ΥΠΟΜΝΗΜΑ ΓΙΑ ΕΝΑ ΣΥΝΤΑΓΜΑ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΛΑΟΥ
   dewey: 342.495 ΒΕΓ
   entry_numbers:
   - '11885'
   editor: ΘΕΜΕΛΙΟ // ΑΘΗΝΑ
   pages: 177
@@ -482585,15 +482440,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9593
   authors:
-  - ΑΝΤΟΡΝΟ,ΤΟΝΤΟΡ
+  - ADORNO,THEODOR
   language: el
   title: ΚΟΙΝΩΝΙΟΛΟΓΙΑ.ΕΙΣΑΓΩΓΙΚΑ ΔΟΚΙΜΙΑ
   dewey: 530 ΑΝΤ
   entry_numbers:
   - '11902'
   translators:
   - ΓΡΑΒΑΡΗΣ,ΔΙΟΝΥΣΗΣ
@@ -483045,15 +482900,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9602
   authors:
-  - ΒΟΥΡΒΑΧΗΣ,ΕΛΕΥΘΕΡΙΟΣ ΑΓΓ.
+  - ΒΟΥΡΒΑΧΗΣ,ΕΛΕΥΘΕΡΙΟΣ,ΑΓΓ.
   language: el
   title: ΠΟΙΟΣ ΣΚΟΤΩΣΕ ΤΟΝ ΠΟΛΚ;
   dewey: 330 ΒΟΥ
   entry_numbers:
   - '11892'
   editor: ΠΡΟΣΚΗΝΙΟ // ΑΘΗΝΑ
   edition_year: 2003
@@ -484040,15 +483895,15 @@
 - dbase_number: 9621
   authors:
   - ΣΤΑΟΥΤ,ΡΕΞ
   language: el
   title: ΠΑΡΑ ΠΟΛΛΕΣ ΓΥΝΑΙΚΕΣ
   dewey: 810.11 ΣΤΑ
   entry_numbers:
-  - 11921Α
+  - '11921'
   translators:
   - ΚΟΝΤΟΣΙΑΝΟΥ,Α.
   editor: ΛΑΜΠΡΑΚΗ // ΑΘΗΝΑ
   edition_year: 2009
   pages: 264
   topics:
   - ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -484060,15 +483915,15 @@
   offprint: false
   ean: 978-960-469-647-5
   original_entry:
     0: 9621
     1: ΣΤΑΟΥΤ,ΡΕΞ
     2: ΠΑΡΑ ΠΟΛΛΕΣ ΓΥΝΑΙΚΕΣ
     4: 810.11ΣΤΑ
-    5: 11921(α)
+    5: '11921'
     6: Α.ΚΟΝΤΟΣΙΑΝΟΥ
     8: ΛΑΜΠΡΑΚΗ
     9: ΑΘΗΝΑ
     10: '2009'
     11: 264Σ
     12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -484467,15 +484322,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9629
   authors:
-  - ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ
+  - ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ,M.
   language: el
   title: ΤΟ ΑΜΑΡΤΗΜΑ ΤΗΣ ΜΗΤΡΟΣ ΜΟΥ
   dewey: 889.21 ΒΙΖ
   entry_numbers:
   - '11940'
   editor: ΛΑΜΠΡΑΚΗ // ΑΘΗΝΑ
   edition_year: 2009
@@ -485820,15 +485675,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9655
   authors:
-  - ΑΝΤΩΝΟΠΟΥΛΟΥ,Μ.Ν
+  - ΑΝΤΩΝΟΠΟΥΛΟΥ,ΜΑΡΙΑ,Ν.
   language: el
   title: Η ΔΟΜΗ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΚΟΙΝΩΝΙΑΣ
   dewey: 320 ΑΝΤ
   entry_numbers:
   - '11918'
   editor: ΚΕΝΤΑΥΡΟΣ // ΑΘΗΝΑ
   edition_year: 1986
@@ -486336,15 +486191,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9665
   authors:
-  - ΑΛΤΟΥΣΕΡ,ΛΟΥΙ
+  - ALTHUSSER,LOUIS
   language: el
   title: ΤΟ ΜΕΛΛΟΝ ΔΙΑΡΚΕΙ ΠΟΛΥ
   subtitle: ΤΑ ΓΕΓΟΝΟΤΑ
   dewey: 330 ΑΛΤ
   entry_numbers:
   - '11938'
   editor: Ο ΠΟΛΙΤΗΣ // ΑΘΗΝΑ
@@ -486489,15 +486344,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9668
   authors:
-  - ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ
+  - ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ,M.
   language: el
   title: ΠΟΙΟΣ ΗΤΟ Ο ΦΟΝΕΥΣ ΤΟΥ ΑΔΕΛΦΟΥ ΜΟΥ
   dewey: 889.21 ΒΙΖ
   entry_numbers:
   - '11950'
   editor: ΛΑΜΠΡΑΚΗ // ΑΘΗΝΑ
   edition_year: 2009
@@ -486590,15 +486445,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9670
   authors:
-  - ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ
+  - ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ,M.
   language: el
   title: ΑΙ ΣΥΝΕΠΕΙΑΙ ΤΗΣ ΠΑΛΑΙΑΣ ΙΣΤΟΡΙΑΣ
   dewey: 889.21 ΒΙΖ
   entry_numbers:
   - '11958'
   editor: ΛΑΜΠΡΑΚΗ // ΑΘΗΝΑ
   edition_year: 2009
@@ -488451,15 +488306,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9707
   authors:
-  - ΑΠΟΣΤΟΛΟΠΟΥΛΟΣ,ΑΠΟΣΤΟΛΟΣ
+  - ΑΠΟΣΤΟΛΟΠΟΥΛΟΣ,ΑΠΟΣΤΟΛΗΣ
   language: el
   title: ΟΔΟΙΠΟΡΙΚΟ
   dewey: 889.21 ΑΠΟ
   entry_numbers:
   - '11987'
   editor: ΣΥΓΧΡΟΝΗ ΓΝΩΜΗ // ΑΘΗΝΑ
   edition_year: 1993
@@ -490906,15 +490761,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9756
   authors:
-  - ΒΑΗ,ΘΕΟΔΩΡΟΥ
+  - ΒΑΗΣ,ΘΕΟΔΩΡΟΣ
   language: el
   title: Η ΣΥΝΤΑΓΜΑΤΙΚΗ ΘΕΜΕΛΙΩΣΗ ΤΟΥ ΕΡΓΑΤΙΚΟΥ ΑΓΩΝΑ
   dewey: 330 ΒΑΗ
   entry_numbers:
   - '12032'
   editor: None // ΑΘΗΝΑ
   edition_year: 1982
@@ -492875,15 +492730,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9795
   authors:
-  - ΑΙΝΣΤΑΙΝ
+  - EINSTEIN,ALBERT
   language: el
   title: ΟΙ ΔΙΑΛΕΞΕΙΣ ΤΟΥ ΠΡΙΝΣΤΟΝ
   dewey: 530.11 ΑΙΝ
   entry_numbers:
   - '12092'
   editor: ΚΟΡΟΝΤΖΗ // None
   pages: 147
@@ -494001,15 +493856,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9818
   authors:
-  - ΒΑΚΑΛΙΟΣ,Θ
+  - ΒΑΚΑΛΙΟΣ,ΘΑΝΑΣΗΣ
   language: el
   title: Η ΑΠΟΤΕΛΕΣΜΑΤΙΚΟΤΗΤΑ ΤΩΝ ΠΡΟΓΡΑΜΜΑΤΩΝ ΣΠΟΥΔΩΝ
   dewey: 378 ΒΑΚ
   entry_numbers:
   - '12113'
   editor: None // ΑΘΗΝΑ
   edition_year: 1985
@@ -494800,15 +494655,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9834
   authors:
-  - ΑΙΤΩΛΟΑΚΑΡΝΑΝΙΑ
+  - Νομαρχιακή Αυτοδιοίκηση Αιτωλοακαρνανιας
   language: el
   title: Η ΑΙΤΩΛΟΑΚΑΡΝΑΝΙΑ ΚΑΘΕ ΜΕΡΑ
   dewey: 633.71 ΑΙΤ
   entry_numbers:
   - '12124'
   editor: ΝΟΜ.ΑΥΤ/ΚΗΣΗ ΑΙΤ.ΝΙΑ // None
   edition_year: 2008
@@ -500207,15 +500062,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 9951
   authors:
-  - VARGA,E.
+  - VARGA,EVGENIJ,SAMUILOVIC
   title: GRUNDFRAGEN DER OKONOMIK UND PLITIK DES IMPERIALISMUS
   dewey: 430 ΓΕΡ
   entry_numbers:
   - '12213'
   edition_year: 1955
   pages: 740
   topics:
@@ -503357,15 +503212,15 @@
 - dbase_number: 10019
   authors:
   - ΑΝΔΡΟΥΛΑΚΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΑΝΑΝΗΨΗ ΤΩΝ ΒΑΡΙΑ ΠΑΣΧΟΝΤΩΝ
   dewey: 615.5 ΑΝΔ
   entry_numbers:
-  - 10793Α
+  - '10793'
   edition: '3'
   editor: ΠΑΡΙΣΙΑΝΟΣ // ΑΘΗΝΑ
   edition_year: 1982
   pages: 486
   topics:
   - ΙΑΤΡΙΚΑ
   donors:
@@ -503374,15 +503229,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 10019
     1: ΑΝΔΡΟΥΛΑΚΗΣ,ΓΕΩΡΓΙΟΣ
     2: ΑΝΑΝΗΨΗ ΤΩΝ ΒΑΡΙΑ ΠΑΣΧΟΝΤΩΝ
     4: 615.5ΑΝΔ
-    5: 10793 Α
+    5: '10793'
     7: ΤΡΙΤΗ
     8: ΠΑΡΙΣΙΑΝΟΣ
     9: ΑΘΗΝΑ
     10: '1982'
     11: '486'
     12: ΙΑΤΡΙΚΑ
     13: ΙΑΤΡΙΚΑ
@@ -503952,15 +503807,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10031
   authors:
-  - WOOD,M.J
+  - WOOD,M.J.
   language: el
   title: ΕΡΠΗΤΑΣ ΖΩΣΤΗΡΑΣ
   dewey: 615.5 WOO
   entry_numbers:
   - '10797'
   editor: None // ΑΘΗΝΑ
   pages: 41
@@ -504350,15 +504205,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10039
   authors:
-  - ΑΓΓΕΛΟΠΟΥΛΟΣ,ΒΑΣΙΛΗΣ
+  - ΑΓΓΕΛΟΠΟΥΛΟΣ,ΒΑΣΙΛΕΙΟΣ
   language: el
   title: ΕΠΙΤΟΜΟΣ ΚΛΙΝΙΚΗ ΠΑΘΟΛΟΓΙΚΗ ΦΥΣΙΟΛΟΓΙΑ
   dewey: 615.5 ΑΓΓ
   entry_numbers:
   - '10809'
   editor: ΠΑΡΙΣΙΑΝΟΣ // ΑΘΗΝΑ
   edition_year: 1975
@@ -504400,15 +504255,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10040
   authors:
-  - ΑΓΙΟΥΛΑΝΤΗΣ,Γ
+  - ΑΓΙΟΥΤΑΝΤΗΣ,Γ.
   language: el
   title: ΤΟΞΙΚΟΛΟΓΙΑ
   dewey: 615.5 ΑΓΙ
   entry_numbers:
   - '10788'
   editor: ΠΑΡΙΣΙΑΝΟΣ // ΑΘΗΝΑ
   edition_year: 1978
@@ -504747,15 +504602,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10047
   authors:
-  - ΒΕΛΙΣΣΑΡΟΠΟΥΛΟΥ,ΠΑΝΑΓΙΩΤΟΥ Κ.
+  - ΒΕΛΙΣΣΑΡΟΠΟΥΛΟΣ,ΠΑΝΑΓΙΩΤΗΣ,Κ.
   language: el
   title: ΕΠΙΤΟΜΟΣ ΟΦΘΑΛΜΟΛΟΓΙΑ
   dewey: 615.5 ΒΕΛ
   entry_numbers:
   - '10753'
   editor: ΠΑΝΕΠΙΣΤΗΜΙΟ ΑΘΗΝΩΝ // ΑΘΗΝΑ
   pages: 260
@@ -505297,29 +505152,29 @@
 - dbase_number: 10058
   authors:
   - ΠΑΠΑΖΑΧΟΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΤΟ ΗΛΕΚΤΟΚΑΡΔΙΟΓΡΑΦΗΜΑ
   dewey: 615.5 ΠΑΠ
   entry_numbers:
-  - 10794Α
+  - '10794'
   editor: None // ΛΙΤΣΑΣ
   topics:
   - ΙΑΤΡΙΚΑ
   donors:
   - ΜΙΧΑΛΗ,ΓΙΑΝΝΟΥΛΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 10058
     1: ΠΑΠΑΖΑΧΟΣ,ΓΕΩΡΓΙΟΣ
     2: ΤΟ ΗΛΕΚΤΟΚΑΡΔΙΟΓΡΑΦΗΜΑ
     4: 615.5ΠΑΠ
-    5: 10794 Α
+    5: '10794'
     9: ΛΙΤΣΑΣ
     12: ΙΑΤΡΙΚΑ
     13: ΙΑΤΡΙΚΑ
     14: ΙΑΤΡΙΚΑ
     17: ΔΩΡΕΑ ΓΙΑΝΝΟΥΛΑ ΜΙΧΑΛΗ
     3: null
     6: null
@@ -505636,15 +505491,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10065
   authors:
-  - ΒΑΡΩΝΟΥ,Δ.Δ
+  - ΒΑΡΩΝΟΣ,Δ.,Δ.
   language: el
   title: ΙΑΤΡΙΚΗ ΦΑΡΜΑΚΟΛΟΓΙΑ
   dewey: 615.5 ΒΑΡ
   entry_numbers:
   - '10788'
   editor: ΠΑΡΙΣΙΑΝΟΣ // ΑΘΗΝΑ
   edition_year: 1976
@@ -506727,15 +506582,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10087
   authors:
-  - DR WOOD,M.J
+  - WOOD,M.J.
   language: el
   title: ΕΡΠΗΤΑΣ ΖΩΣΤΗΡΑΣ
   dewey: 615.5 WOO
   entry_numbers:
   - '12291'
   editor: None // ΑΘΗΝΑ
   pages: 41
@@ -507176,15 +507031,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10096
   authors:
-  - ATKINSON,R.S
+  - ATKINSON,R.S.
   language: el
   title: ΕΠΙΤΟΜΟΣ ΑΝΑΙΣΘΗΣΙΟΛΟΓΙΑ
   dewey: 615.5 ATK
   entry_numbers:
   - '12320'
   editor: ΠΑΡΙΣΙΑΝΟΣ // ΑΘΗΝΑ
   edition_year: 1979
@@ -507875,15 +507730,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10110
   authors:
-  - ΒΑΣΙΛΕΙΑΔΗ,Π
+  - ΒΑΣΙΛΕΙΑΔΗΣ,ΠΕΤΡΟΣ
   language: el
   title: ΜΑΘΗΜΑΤΑ ΥΓΙΕΙΝΗΣ ΚΑΙ ΕΠΙΔΗΜΙΟΛΟΓΙΑΣ
   dewey: 615.5 ΒΑΣ
   entry_numbers:
   - '12284'
   editor: ΠΑΡΙΣΙΑΝΟΣ // ΑΘΗΝΑ
   pages: 508
@@ -508363,15 +508218,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10120
   authors:
-  - ΑΓΙΟΥΤΑΝΗ,Γ.
+  - ΑΓΙΟΥΤΑΝΤΗΣ,Γ.
   language: el
   title: ΙΑΤΡΟΔΙΚΑΣΤΙΚΑ ΘΕΜΑΤΑ
   dewey: 615.5 ΑΓΙ
   entry_numbers:
   - '12324'
   editor: ΠΑΡΙΣΙΑΝΟΣ // ΑΘΗΝΑ
   edition_year: 1980
@@ -509594,15 +509449,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10145
   authors:
-  - ΑΓΓΕΛΟΠΟΥΛΟΣ,ΒΑΣΙΛΗΣ
+  - ΑΓΓΕΛΟΠΟΥΛΟΣ,ΒΑΣΙΛΕΙΟΣ
   language: el
   title: ΑΙ ΣΥΓΧΡΟΝΟΙ ΑΝΤΙΛΗΨΕΙΣ ΕΠΙ ΤΗΣ ΘΕΡΑΠΕΙΑΣ ΤΩΝ ΕΣΩΤΕΡΙΚΩΝ
   dewey: 615.5 ΑΓΓ
   entry_numbers:
   - '12343'
   editor: None // ΑΘΗΝΑ
   edition_year: 1963
@@ -510719,15 +510574,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10168
   authors:
-  - ΑΓΓΕΛΟΠΟΥΛΟΣ,ΒΑΣΙΛΗΣ
+  - ΑΓΓΕΛΟΠΟΥΛΟΣ,ΒΑΣΙΛΕΙΟΣ
   language: el
   title: ΕΠΕΞΗΓΗΣΕΙΣ ΚΑΙ ΚΛΙΝΙΚΗ ΣΗΜΑΣΙΑ ΤΩΝ ΕΡΓΑΣΤΗΡΙΑΚΩΝ ΕΞΕΤΑΣΕΩΝ
   dewey: 615.5 ΑΓΓ
   entry_numbers:
   - '12359'
   editor: ΠΑΡΙΣΙΑΝΟΣ // ΑΘΗΝΑ
   pages: 491
@@ -514035,15 +513890,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10235
   authors:
-  - ANDREWS,V,C,
+  - ANDREWS,VIRGINIA,CLEO
   language: el
   title: ΗΜΙΤΕΛΗΣ ΣΥΜΦΩΝΙΑ
   dewey: 823 AND
   entry_numbers:
   - '12507'
   translators:
   - ΤΟΥΣΑ,ΔΕΣΠΟΙΝΑ
@@ -514232,15 +514087,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10239
   authors:
-  - ANDREWS,V,C
+  - ANDREWS,VIRGINIA,CLEO
   language: el
   title: ΤΟ ΣΠΙΤΙ ΤΗΣ ΛΙΜΝΗΣ
   dewey: 823 AND
   entry_numbers:
   - '12506'
   translators:
   - ΝΙΚΟΛΟΠΟΥΛΟΥ,ΚΑΙΤΗ
@@ -514736,15 +514591,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10249
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: Ο ΓΥΡΟΣ ΤΟΥ ΚΟΣΜΟΥ ΣΕ 80 ΗΜΕΡΕΣ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '12490'
   pages: 201
   topics:
@@ -516029,15 +515884,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10275
   authors:
-  - ΒΑΒΑΛΕΚΑΣ,ΚΩΝ/ΝΟΣ
+  - ΒΑΒΑΛΕΚΑΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΣΕΡΡΕΣ ΑΠΟ ΤΟ ΧΘΕΣ ΣΤΟ ΣΗΜΕΡΑ
   dewey: 914.95 ΒΑΒ
   entry_numbers:
   - '12631'
   editor: ΔΗΝΟΣ ΣΕΡΡΩΝ // ΣΕΡΡΕΣ
   edition_year: 2001
@@ -516480,15 +516335,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10284
   authors:
-  - ΒΛΑΧΟΥ,ΑΓΓΕΛΟΥ
+  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,Σ.
   language: el
   title: ΗΡΟΔΟΤΟΥ ΙΣΤΟΡΙΑΙ
   dewey: 884.3 ΒΛΑ
   entry_numbers:
   - '12649'
   editor: ΚΕΝΡ.ΕΛΛΗΝ.ΣΥΓΓΡΑΦΕΩ // ΑΘΗΝΑ
   edition_year: 1989
@@ -516582,15 +516437,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10286
   authors:
-  - ΑΔΑΜΟΥ-ΦΙΚΑ,Κ.
+  - ΑΔΑΜΟΥ-ΦΙΚΑ,ΚΩΣΤΟΥΛΑ
   title: ΟΙ ΙΔΕΑΤΕΣ ΠΟΛΙΤΕΙΕΣ ΑΠΟ ΤΟΝ ΠΛΑΤΩΝΑ ΣΤΟΝ CAMPANELLA
   dewey: 195 ΑΔΑ
   entry_numbers:
   - '12653'
   editor: ΑΚΑΔΗΜΙΑ ΑΘΗΝΩΝ // ΑΘΗΝΑ
   edition_year: 2006
   pages: 186
@@ -518828,15 +518683,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10330
   authors:
-  - ΒΟΛΤΙ,ΧΟΡΧΕ
+  - VOLPI,JORGE
   language: el
   title: ΑΝΑΖΗΤΩΝΤΑΣ ΤΟΝ ΚΛΙΝΓΚΣΟΡ
   dewey: 860.11 ΒΟΛ
   entry_numbers:
   - '12697'
   translators:
   - ΚΑΡΑΤΖΑΣ,ΛΕΩΝΙΔΑΣ
@@ -518984,15 +518839,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10333
   authors:
-  - ΑΣΕΝΑ,ΝΤΟΥΙΓΚΟΥ
+  - ASENA,DUYGU
   language: el
   title: ΟΥΤΕ ΕΡΩΤΑΣ ΥΠΑΡΧΕΙ
   dewey: 894.35 ΑΣΕ
   entry_numbers:
   - '12711'
   translators:
   - ΒΡΕΤΟΥ,ΣΤΕΛΛΑ
@@ -519553,15 +519408,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10344
   authors:
-  - ΑΤΓΟΥΝΤ,ΜΑΡΓΚΑΡΕΤ
+  - ATWOOD,MARGARET
   language: el
   title: ΟΡΥΞ ΚΑΙ ΚΡΕΙΚ
   dewey: 810.11 ΑΤΓ
   entry_numbers:
   - '12698'
   translators:
   - ΑΓΓΕΛΙΔΟΥ,ΜΑΡΙΑ
@@ -519861,15 +519716,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10350
   authors:
-  - ΒΟΛΠΙ,ΧΟΡΧΕ
+  - VOLPI,JORGE
   language: el
   title: Η ΕΠΟΧΗ ΤΗΣ ΣΤΑΧΤΗΣ
   dewey: 860.11 ΒΟΛ
   entry_numbers:
   - '12714'
   translators:
   - ΚΑΡΑΤΖΑΣ,ΛΕΩΝΙΔΑΣ
@@ -529257,15 +529112,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10529
   authors:
-  - ΒΑΛΙΟΥΛΗ,ΠΑΝΤΕΛΗ
+  - ΒΑΛΙΟΥΛΗΣ,ΠΑΝΤΕΛΗΣ
   language: el
   title: ΣΕΛΙΔΕΣ ΕΚ ΤΗΣ ΣΥΜΦΟΡΑΣ ΤΟΥ ΠΟΝΤΟΥ 1921-1924
   dewey: 938.73 ΒΑΛ
   entry_numbers:
   - '13123'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2005
@@ -531128,15 +530983,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10565
   authors:
-  - ΑΠΟΣΤΟΛΙΔΗ,ΠΑΥΛΟΥ
+  - ΑΠΟΣΤΟΛΙΔΗΣ,ΠΑΥΛΟΣ
   language: el
   title: Η ΜΗΤΡΟΠΟΛΙΣ ΡΟΔΟΠΟΛΕΩΣ
   subtitle: ΤΟ ΖΗΤΗΜΑ ΤΩΝ ΕΞΑΡΧΙΩΝ ΤΟΥ ΠΟΝΤΟΥ
   dewey: 938.498 ΑΠΟ
   entry_numbers:
   - '12958'
   - '16967'
@@ -531396,15 +531251,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10570
   authors:
-  - ΑΝΔΡΙΩΤΗ,ΝΙΚΟΛΑΟΥ
+  - ΑΝΔΡΙΩΤΗΣ,ΝΙΚΟΛΑΟΣ,ΠΑΝΤΕΛΗΣ
   language: el
   title: ΚΡΥΠΤΟΧΡΙΣΤΙΑΝΙΚΑ ΚΕΙΜΕΝΑ
   dewey: 956.5 ΑΝΔ
   entry_numbers:
   - '12970'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2008
@@ -531874,15 +531729,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10579
   authors:
-  - ΒΗΣΣΑΡΙΩΝΟΣ
+  - ΒΗΣΣΑΡΙΩΝ,ΒΑΣΙΛΕΙΟΣ
   language: el
   title: ΕΓΚΩΜΙΟΝ ΕΙΣ ΤΡΑΠΕΖΟΥΝΤΑ
   dewey: 938.498 ΒΗΣ
   entry_numbers:
   - '12950'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2000
@@ -532185,15 +532040,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10585
   authors:
-  - ANDREADIS,GEORGIOS
+  - ΑΝΔΡΕΑΔΗΣ,ΓΕΩΡΓΙΟΣ
   title: THE CRYPTOCHRISTIANS
   dewey: 956.5 AND
   entry_numbers:
   - '12967'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1995
   pages: 102
@@ -532656,15 +532511,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10594
   authors:
-  - ΑΓΑΘΑΓΓΕΛΟΥ,Α.Ι
+  - ΑΓΑΘΑΓΓΕΛΟΥ,ΑΘΑΝΑΣΙΟΣ,Ι.
   language: el
   title: ΠΕΠΕΡΕΚ
   dewey: 915 ΑΓΑ
   entry_numbers:
   - '13003'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2007
@@ -534325,15 +534180,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10626
   authors:
-  - ΑΠΟΣΤΟΛΙΔΗ,ΠΑΥΛΟΥ
+  - ΑΠΟΣΤΟΛΙΔΗΣ,ΠΑΥΛΟΣ
   language: el
   title: Ο ΜΗΤΡΟΠΟΛΙΤΗΣ ΤΡΑΠΕΖΟΥΝΤΟΣ ΧΡΥΣΑΝΘΟΣ ΦΙΛΙΠΠΙΔΗΣ (191301923)
   dewey: 956.5 ΑΠΟ
   entry_numbers:
   - '13069'
   - '16966'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -534434,15 +534289,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10628
   authors:
-  - ΑΝΔΡΕΑΔΗ,ΧΡΗΣΤΟΥ
+  - ΑΝΔΡΕΑΔΗΣ,ΧΡΗΣΤΟΣ,Γ.
   language: el
   title: Ο ΚΟΡΥΤΣΑΣ ΚΑΙ ΠΡΕΜΕΤΗΣ ΦΩΤΙΟΣ ΚΑΛΠΙΔΗΣ (1862-1906)
   dewey: 938.993 ΑΝΔ
   entry_numbers:
   - '13076'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2004
@@ -535600,15 +535455,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10650
   authors:
-  - ΑΠΟΣΤΟΛΙΔΗ,ΛΕΩΝΙΔΑ
+  - ΑΠΟΣΤΟΛΙΔΗΣ,ΛΕΩΝΙΔΑΣ
   language: el
   title: ΑΓΝΩΣΤΕΣ ΣΕΛΙΔΕΣ ΤΟΥ ΠΟΝΤΟΥ
   dewey: 938 ΑΠΟ
   entry_numbers:
   - '13086'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2001
@@ -535652,15 +535507,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10651
   authors:
-  - ΒΑΛΑΒΑΝΗ,ΓΕΩΡΓΙΟΥ
+  - ΒΑΛΑΒΑΝΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΣΥΓΧΡΟΝΟΣ ΓΕΝΙΚΗ ΙΣΤΟΡΙΑ ΤΟΥ ΠΟΝΤΟΥ
   dewey: 938.4 ΒΑΛ
   entry_numbers:
   - '13088'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1986
@@ -535914,15 +535769,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10656
   authors:
-  - ΒΑΛΑΒΑΝΗ,ΓΕΩΡΓΙΟΥ
+  - ΒΑΛΑΒΑΝΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΛΑΟΓΡΑΦΙΚΑ ΚΕΡΑΣΟΥΝΤΟΣ
   dewey: 398 ΒΑΛ
   entry_numbers:
   - '12532'
   editor: ΕΠΙΤΡ.ΠΟΝΤΙΑΚΩΝ ΜΕΛΕ // ΑΘΗΝΑ
   edition_year: 2010
@@ -539539,15 +539394,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10725
   authors:
-  - ΑΝΔΡΕΑΔΗ,ΓΕΩΡΓΙΟΥ
+  - ΑΝΔΡΕΑΔΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΤΟ ΤΣΑΓΡΑΚ ΤΗΣ ΚΕΡΑΣΟΥΝΤΑΣ ΤΟΥ ΠΟΝΤΟΥ
   dewey: 938.498 ΑΝΔ
   entry_numbers:
   - '13182'
   editor: None // ΑΘΗΝΑ
   edition_year: 1999
@@ -542008,15 +541863,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10773
   authors:
-  - ΑΛ-ΑΣΟΥΑΝΙ,ΑΛΑΑ
+  - AL ASWANY,ALAA
   language: el
   title: ΘΑ ΗΘΕΛΑ ΝΑ ΗΜΟΥΝ ΑΙΓΥΠΤΙΟΣ
   dewey: 892.721 ΑΣΟ
   entry_numbers:
   - '13285'
   translators:
   - ΓΡΑΜΜΑΤΙΚΟΠΟΥΛΟΥ,ΕΥΓ.
@@ -543433,15 +543288,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10801
   authors:
-  - ΒΑΣΙΛΑΤΟΣ,Ν.
+  - ΒΑΣΙΛΑΤΟΣ,ΝΙΚΟΣ
   language: el
   title: ΚΑΣΤΡΑ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΓΗΣ
   dewey: 725 ΒΑΣ
   entry_numbers:
   - '9141'
   editor: ΜΠΑΛΤΕΡ // None
   edition_year: 1991
@@ -548423,15 +548278,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10898
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: ΔΥΟ ΧΡΟΝΙΑ ΔΙΑΚΟΠΕΣ
   dewey: 880.09 ΒΕΡ
   entry_numbers:
   - '13463'
   translators:
   - ΑΝΤΩΝΟΠΟΥΛΟΣ,ΠΑΝ.
@@ -548473,15 +548328,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10899
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: Ο ΠΥΡΓΟΣ ΤΩΝ ΚΑΡΠΑΘΙΩΝ
   dewey: 880.09 ΒΕΡ
   entry_numbers:
   - '13462'
   translators:
   - ΤΣΟΥΚΑΛΑ,Γ.
@@ -549326,15 +549181,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10916
   authors:
-  - ASYMEONIDOU-PAPADOPOULOU,,PARYSATIS
+  - ΠΑΠΑΔΟΠΟΥΛΟΥ-ΣΥΜΕΩΝΙΔΟΥ,ΠΑΡΥΣΑΤΙΣ
   title: PONTOS BETWEEN YESTERDAY AMN TOMORROW
   dewey: 938.498 SYM
   entry_numbers:
   - '13125'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2001
   pages: 102
@@ -549377,15 +549232,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10917
   authors:
-  - ΑΝΔΡΕΑΔΗ,ΧΡΗΣΤΟΥ
+  - ΑΝΔΡΕΑΔΗΣ,ΧΡΗΣΤΟΣ,Γ.
   language: el
   title: ΚΕΙΜΕΝΑ ΕΦΗΜΕΡΙΔΩΝ ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΕΩΣ ΓΙΑ ΤΟΝ ΕΛΛΗΝΙΣΜΟ ΤΟΥ
   subtitle: ΠΟΝΤΟΥ 1843-1903
   dewey: 938.6 ΑΝΔ
   entry_numbers:
   - '13479'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -550328,15 +550183,15 @@
   authors:
   - ΗΛΙΑΔΗΣ,ΧΡΗΣΤΟΣ
   language: el
   title: ΠΟΝΤΟΣ-ΓΕΝΟΚΤΟΝΙΑ
   subtitle: ΟΣΑ ΑΝΘΥΜΟΥΜΑΙ ΑΠΟ ΤΗΝ ΠΕΡΙΠΕΤΕΙΩΔΗ ΖΩΗ ΜΟΥ
   dewey: 938.73 ΗΛΙ
   entry_numbers:
-  - isplay status
+  - '13499'
   editor: ΓΟΡΔΙΟΣ // ΑΘΗΝΑ
   edition_year: 2002
   pages: 222
   topics:
   - ΠΟΝΤΟΣ
   copies: 2
   donors:
@@ -550347,15 +550202,15 @@
   isbn: 960-7083-53-9
   original_entry:
     0: 10935
     1: ΗΛΙΑΔΗΣ,ΧΡΗΣΤΟΣ
     2: ΠΟΝΤΟΣ-ΓΕΝΟΚΤΟΝΙΑ
     3: ΟΣΑ ΑΝΘΥΜΟΥΜΑΙ ΑΠΟ ΤΗΝ ΠΕΡΙΠΕΤΕΙΩΔΗ ΖΩΗ ΜΟΥ
     4: 938.73ΗΛΙ
-    5: isplay status
+    5: '13499'
     8: ΓΟΡΔΙΟΣ
     9: ΑΘΗΝΑ
     10: '2002'
     11: 222Σ
     12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
     13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
     14: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
@@ -551369,15 +551224,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 10955
   authors:
-  - ΑΛΕΞΑΝΔΡΟΥ,ΓΙΑΝΝΗΣ-ΜΑΡΙΑ
+  - ΑΛΕΞΑΝΔΡΟΥ,ΓΙΑΝΝΗΣ
+  - ΑΛΕΞΑΝΔΡΟΥ,ΜΑΡΙΑ
   language: el
   title: ΠΑΛΑΤΙΑ ΤΟΥ ΒΟΣΠΟΡΟΥ
   dewey: 889.21 ΑΛΕ
   entry_numbers:
   - '13518'
   editor: ΛΙΒΑΝΗ // ΑΘΗΝΑ
   edition_year: 2004
@@ -552953,15 +552809,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10986
   authors:
-  - ΑΝΔΡΕΑΔΗ,ΚΩΝ/ΝΟΥ
+  - ΑΝΔΡΕΑΔΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΠΟΙΗΜΑΤΑ
   subtitle: ΚΑΤΙΝΑΝ ΝΑ ΒΑΛΛΩ ΓΩ ΣΟΝ ΝΟΥ Μ ΚΑΙ ΑΡΧΙΝΩ ΚΑΙ ΓΡΑΦΤΩ ...
   dewey: 889.1 ΑΝΔ
   entry_numbers:
   - '13614'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -553321,15 +553177,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10993
   authors:
-  - ΒΑΚΑΛΟΠΟΥΛΟΣ,ΚΩΝ/ΝΟΣ
+  - ΒΑΚΑΛΟΠΟΥΛΟΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΦΙΛΕΚΠΑΙΔΕΥΤΙΚΟΣ ΣΥΛΛΟΓΟΣ ΑΔΡΙΑΝΟΥΠΟΛΕΩΣ (1872-1996)
   dewey: 956.5 ΒΑΚ
   entry_numbers:
   - '13626'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1996
@@ -553373,15 +553229,16 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10994
   authors:
-  - ΒΑΡΒΟΥΝΗΣ.Μ.Γ-ΙΩΑΝΝΙΔΟΥ ΑΝΑΣΤΑΣΙΑ
+  - ΒΑΡΒΟΥΝΗΣ,ΜΑΝΟΛΗΣ,Γ.
+  - ΙΩΑΝΝΙΔΟΥ,ΑΝΑΣΤΑΣΙΑ
   language: el
   title: ΛΑΟΓΡΑΦΙΚΗ ΚΑΙ ΔΗΜΟΓΡΑΦΙΚΗ ΦΥΣΙΟΓΝΩΜΙΑ ΤΩΝ ΘΡΑΚΙΚΩΝ ΟΙΚΙΣΜΩΝ
   subtitle: Η ΠΕΡΙΠΤΩΣΗ ΤΗΣ ΚΑΡΥΔΙΑΣ ΤΟΥ ΝΟΜΟΥ ΡΟΔΟΠΗΣ
   dewey: 398 ΒΑΡ
   entry_numbers:
   - '13622'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -553532,15 +553389,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 10997
   authors:
-  - ΑΝΘΕΜΙΔΗ,ΑΧΙΛΛΕΑ
+  - ΑΝΘΕΜΙΔΗΣ,ΑΧΙΛΛΕΑΣ
   language: el
   title: ΤΟΥΡΚΙΑ
   subtitle: Η ΧΩΡΑ ΤΩΝ ΘΡΗΣΚΕΥΤΙΚΩΝ ΚΑΙ ΕΘΝΙΚΩΝ ΜΕΙΟΝΟΤΗΤΩΝ
   dewey: 938.498 ΑΝΘ
   entry_numbers:
   - '13631'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -553691,15 +553548,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 11000
   authors:
-  - ΒΑΚΑΛΟΠΟΥΛΟΣ,ΚΩΝ/ΝΟΣ
+  - ΒΑΚΑΛΟΠΟΥΛΟΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: Ο ΕΛΛΗΝΙΣΜΟΣ ΤΗΣ ΒΟΡΕΙΑΣ ΘΡΑΚΗΣ ΚΑΙ ΤΟΥ ΘΡΑΚΙΚΟΥ ΕΥΞ.ΠΟΝΤΟΥ
   dewey: 938.99 ΒΑΚ
   entry_numbers:
   - '13624'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1995
@@ -553743,15 +553600,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 11001
   authors:
-  - ΒΑΚΑΛΟΠΟΥΛΟΣ,ΚΩΝ/ΝΟΣ
+  - ΒΑΚΑΛΟΠΟΥΛΟΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΝΕΟΤΟΥΡΚΟΙ ΚΑΙ ΜΑΚΕΔΟΝΙΑ (1908-1912)
   dewey: 938.498 ΒΑΚ
   entry_numbers:
   - '13623'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1988
@@ -553793,15 +553650,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 11002
   authors:
-  - ΑΓΑΘΑΓΓΕΛΟΥ,Α.Ι
+  - ΑΓΑΘΑΓΓΕΛΟΥ,ΑΘΑΝΑΣΙΟΣ,Ι.
   language: el
   title: ΟΙ ΜΕΙΖΕΤΕΡ
   dewey: 889.21 ΑΓΑ
   entry_numbers:
   - '13625'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2011
@@ -554313,15 +554170,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 11012
   authors:
-  - ΑΝΔΡΕΑΔΗ,ΧΡΗΣΤΟΥ
+  - ΑΝΔΡΕΑΔΗΣ,ΧΡΗΣΤΟΣ,Γ.
   language: el
   title: ΕΚΘΕΣΕΙΣ ΠΡΟΞΕΝΙΚΕΣ ΕΚΠΑΙΔΕΥΤΙΚΕΣ-ΕΚΚΛΗΣΙΑΣΤΙΚΕΣ ΚΑΙ ΛΟΙΠΑ
   subtitle: ΣΥΝΑΦΗ ΕΓΓΡΑΦΑ ΤΟΥ 19ΟΥ ΑΙΩΝΑ ΓΙΑ ΤΟΝ ΥΠΟΔΟΥΛΟ ΚΑΙ ΜΗ ΕΛΛΗΝΙ
   dewey: 938.601 ΑΝΔ
   entry_numbers:
   - '13604'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -555886,15 +555743,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11042
   authors:
-  - ΒΑΣΙΛΙΚΟΣ,ΒΑΣΙΛΙΚΟΣ
+  - ΒΑΣΙΛΙΚΟΣ,ΒΑΣΙΛΗΣ
   language: el
   title: ΥΠΑΡΧΩ
   subtitle: ΣΤΕΛΙΟΣ ΚΑΖΑΝΤΖΙΔΗΣ
   dewey: 889.21 ΒΑΣ
   entry_numbers:
   - '13647'
   editor: ΛΙΒΑΝΗ // ΑΘΗΝΑ
@@ -556299,15 +556156,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11050
   authors:
-  - ΑΛΛΕΝ-ΑΝΤΙΣΟΝ,ΣΑΡΑ
+  - ADDISON ALLEN,SARAH
   language: el
   title: Ο ΜΑΓΙΚΟΣ ΚΗΠΟΣ
   dewey: 810.11 ΑΛΛ
   entry_numbers:
   - '13651'
   translators:
   - ΑΓΓΕΛΙΔΟΥ,ΜΑΡΙΑ
@@ -556908,15 +556765,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11062
   authors:
-  - ΒΕΝΕΖΗ,ΗΛΙΑ
+  - ΒΕΝΕΖΗΣ,ΗΛΙΑΣ
   language: el
   title: ΑΙΟΛΙΚΗ ΓΗ
   dewey: 889.21 ΒΕΝ
   entry_numbers:
   - '13654'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   edition_year: 1969
@@ -561693,15 +561550,16 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 11156
   authors:
-  - ΑΝΔΡΙΤΣΟΠΟΥΛΟΥ Σ., ΚΕΝΤΕΠΟΖΙΔΗ Ν, ΠΡΑΠΑ
+  - ΑΝΔΡΙΤΣΟΠΟΥΛΟΥ,Σ.
+  - ΚΕΝΤΕΠΟΖΙΔΗ,Ν.,ΠΡΑΠΑ,
   language: el
   title: Ο ΡΟΛΟΣ ΤΩΝ ΚΟΙΝΩΝΙΚΩΝ ΥΠΗΡΕΣΙΩΝ ΣΤΗΝ ΚΑΤΑΠΟΛΕΜΗΣΗ ΤΟΥ ΡΑΤΣΙ
   subtitle: ΣΜΟΥ ΚΑΙ ΤΟΥ ΚΟΙΝΩΝΙΚΟΥ ΑΠΟΚΛΕΙΣΜΟΥ
   dewey: 305.8 ΑΝΔ
   entry_numbers:
   - '13812'
   topics:
@@ -562198,15 +562056,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11166
   authors:
-  - ΒΑΣΙΛΕΙΑΔΗΣ ΧΑΡΑΛΑΜΠΟΣ
+  - ΒΑΣΙΛΕΙΑΔΗΣ,ΧΑΡΑΛΑΜΠΟΣ
   language: el
   title: Ο ΛΑΜΠΟΝ Α ΣΟ ΚΑΡΣ
   subtitle: Η ΟΔΥΣΣΕΙΑ ΕΝΟΣ ΠΟΝΤΙΟΥ ΑΠΟ ΤΟΝ ΚΑΥΚΑΣΟ
   dewey: 938.7 ΒΑΣ
   entry_numbers:
   - '13929'
   editor: ΣΤΟΧΑΣΤΗΣ // ΑΘΗΝΑ
@@ -562348,15 +562206,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11169
   authors:
-  - ΑΡΧΙΤΕΚΤΟΝΙΔΗΣ Ι., ΒΑΣΙΛΗΣ
+  - ΑΡΧΙΤΕΚΤΟΝΙΔΗΣ,ΒΑΣΙΛΗΣ,Ι.
   language: el
   title: ΠΡΑΓΜΜΑΤΕΙΑ ΓΙΑ ΤΗ ΔΙΔΑΣΚΑΛΙΑ ΤΗΣ ΠΟΝΤΙΑΚΗΣ ΛΥΡΑΣ
   dewey: 389 ΑΡΧ
   entry_numbers:
   - '13972'
   editor: ΨΩΜΙΑΔΕΙΟΝ // ΑΘΗΝΑ
   edition_year: 2008
@@ -562596,15 +562454,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11174
   authors:
-  - ΑΓΤΖΙΔΗΣ, ΒΛΑΣΗΣ
+  - ΑΓΤΖΙΔΗΣ,ΒΛΑΣΗΣ
   language: el
   title: Η ΚΑΤΑΡΡΕΥΣΗ ΤΗΣ ΣΟΒΙΕΤΙΚΗΣ ΕΝΩΣΗΣ
   subtitle: ΟΙ ΣΥΝΕΠΕΙΕΣ ΓΙΑ ΤΟΝ ΕΛΛΗΝΙΣΜΟ
   dewey: 938.498 ΑΓΤ
   entry_numbers:
   - '13876'
   edition: '2'
@@ -562995,15 +562853,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11182
   authors:
-  - ΑΝΔΡΕΑΔΗ Γ, ΧΡΗΣΤΟΣ
+  - ΑΝΔΡΕΑΔΗΣ,ΧΡΗΣΤΟΣ,Γ.
   language: el
   title: Ο ΚΟΡΥΤΣΑΣ ΚΑΙ ΠΡΕΜΕΤΗΣ ΦΩΤΙΟΣ ΚΑΛΠΙΔΗΣ (1862-1906)
   subtitle: Ο ΠΟΝΤΙΟΣ ΕΘΝΟΜΑΡΤΥΣ ΙΕΡΑΡΧΗΣ ΠΡΩΤΟ ΘΥΜΑ ΤΟΥ ΜΑΚΕΔ ΑΓΩΝΑ
   dewey: 938.993 ΑΝΔ
   entry_numbers:
   - '13935'
   editor: ΑΦΟΙ ΚΥΡΙΑΚΙΔΗ // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -563046,15 +562904,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11183
   authors:
-  - ΑΝΔΡΙΚΟΠΟΥΛΟΣ ΕΥΓΕΝΙΟΣ
+  - ΑΝΔΡΙΚΟΠΟΥΛΟΣ,ΕΥΓΕΝΙΟΣ
   language: el
   title: ΜΕΣΑ ΑΠΟ... ΤΑ ΜΕΣΑ
   dewey: 938.498 ΑΝΔ
   entry_numbers:
   - '13963'
   editor: ΚΑΜΠΑΝΑ // ΑΘΗΝΑ
   edition_year: 1995
@@ -563348,15 +563206,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11189
   authors:
-  - ΑΒΑΡΙΚΙΩΤΟΣ, Κ., ΑΡΙΣΤΟΤΕΛΗΣ
+  - ΑΒΑΡΙΚΙΩΤΗΣ,ΑΡΙΣΤΟΤΕΛΗΣ,Κ.
   language: el
   title: ΟΡΘΟΔΟΞΙΑΣ ΣΤΥΛΟΙ
   dewey: 230 ΑΒΑ
   entry_numbers:
   - '13903'
   editor: None // ΑΘΗΝΑ
   edition_year: 1972
@@ -564743,15 +564601,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11217
   authors:
-  - VESCO DEL PAOLO
+  - DEL VESCO,PAOLO
   language: el
   title: ΜΟΥΣΕΙΑ ΤΟΥ ΚΟΣΜΟΥ
   subtitle: ΑΙΓΥΠΤΙΑΚΟ ΜΟΥΣΕΙΟ ΚΑΙΡΟ
   dewey: 938.993 VES
   entry_numbers:
   - '13965'
   edition_year: 2007
@@ -565537,15 +565395,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11233
   authors:
-  - ΑΝΔΡΟΝΙΚΟΣ, Μ., ΓΙΑΛΟΥΡΗΣ Ν.,
+  - ΑΝΔΡΟΝΙΚΟΣ,ΜΑΝΩΛΗΣ
+  - ΓΙΑΛΟΥΡΗΣ,ΝΙΚΟΛΑΟΣ
   language: el
   title: ΟΙ ΟΛΥΜΠΙΑΚΟΙ ΑΓΩΝΕΣ ΣΤΗΝ ΑΡΧΑΙΑⁿ ΕΛΛΑΔΑ
   subtitle: ΑΡΧΑΙΑ ΟΛΥΜΠΙΑ ΚΑΙ ΟΛΥΜΠΙΑΚΟΙ ΑΓΩΝΕΣ
   dewey: 938.498 ΑΝΔ
   entry_numbers:
   - '13917'
   editor: ΕΚΔΟΤΙΚΗ ΕΛΛΑΔΟΣ // ΑΘΗΝΑ
@@ -566979,15 +566838,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11262
   authors:
-  - ΑΓΤΖΙΔΗΣ, ΒΛΑΣΗΣ
+  - ΑΓΤΖΙΔΗΣ,ΒΛΑΣΗΣ
   language: el
   title: ΟΙ ΣΤΑΛΙΝΙΚΕΣ ΔΙΩΞΕΙΣ ΚΑΤΑ ΤΩΝ ΕΛΛΗΝΩΝ ΤΗΣ ΣΟΒΟΙΕΤΙΚΗΣΕΝΩΣΗΣ
   dewey: 938.498 ΑΓΤ
   entry_numbers:
   - '13954'
   pages: 39
   topics:
@@ -567521,15 +567380,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11273
   authors:
-  - ΑΓΓΕΛΟΠΟΥΛΟΥ,ΑΝΝΑ-ΜΠΡΟΥΣΚΟΥ,ΑΙΓΛΗ
+  - ΑΓΓΕΛΟΠΟΥΛΟΥ,ΑΝΝΑ
+  - ΜΠΡΟΥΣΚΟΥ,ΑΙΓΛΗ
   language: el
   title: ΕΠΕΞΕΡΓΑΣΙΑ ΠΑΡΑΜΥΘΙΑΚΩΝ ΤΥΠΩΝ ΚΑΙ ΠΑΡΑΛΛΑΓΩΝ ΑΤ 300-499 Α-Β
   dewey: 885.95 ΑΓΓΕ
   entry_numbers:
   - '13561'
   editor: ΓΕΝ.ΓΡΑΜ.ΝΕΑΣ ΓΕΝΙΑΣ // ΑΘΗΝΑ
   edition_year: 1999
@@ -567982,15 +567842,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11282
   authors:
-  - VIZIINOS,GEORGIOS
+  - ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ,M.
   title: MOSCOV-SELIM LA HISTORIA DE UN SOLDADO
   dewey: 938.993 VIZ
   entry_numbers:
   - '13568'
   editor: None // GRANADA
   edition_year: 2002
   pages: 70
@@ -568082,15 +567942,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11284
   authors:
-  - ΑΛΕΞΙΑΔΗ,ΘΩΜΑ
+  - ΑΛΕΞΙΑΔΗΣ,ΘΩΜΑΣ
   language: el
   title: Η ΠΑΦΡΑ ΤΟΥ ΠΟΝΤΟΥ ΙΣΤΟΡΙΑ,ΕΚΚΛΗΣΙΑ,ΕΘΝΙΚΟΙ ΑΓΩΝΕΣ
   dewey: 938.498 ΑΛΕ
   entry_numbers:
   - '14131'
   editor: ΕΠΙΤΡ.ΠΟΝΤΙΑΚ.ΜΕΛΕΤΩ // ΑΘΗΝΑ
   edition_year: 2014
@@ -569678,15 +569538,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11317
   authors:
-  - AMBASSADOR HENRY MORGENTHAU
+  - MORGENTHAU,HENRY
   title: SECRETS OF THE BOSPHORUS
   dewey: 938.498 MOR
   entry_numbers:
   - '14066'
   editor: None // LONDON
   edition_year: 2001
   pages: 267
@@ -569924,15 +569784,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11322
   authors:
-  - WILHELM WORRINGER
+  - WORRINGER,WILHELM
   title: SOYUTLAMA VE EINFUHLUNG
   dewey: 372.65 WOR
   entry_numbers:
   - '14073'
   editor: None // ISTANBUL
   edition_year: 1963
   pages: 116
@@ -570822,15 +570682,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11340
   authors:
-  - ANTONIOS MILIARAKIS
+  - ΜΗΛΙΑΡΑΚΗΣ,ΑΝΤΩΝΙΟΣ
   title: THE SEIZURE OF THE PARTHENON SCULPTURES
   subtitle: AN ACCOUNT OF THE TERRIBLE DESTRUCTION OF THAT FAMOUS MONUM,
   dewey: 722.8 MIL
   entry_numbers:
   - '14081'
   editor: SOC FOR THE ST OF GH // ΑΘΗΝΑ
   edition_year: 2002
@@ -572123,15 +571983,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11366
   authors:
-  - ARMEN DADOUR
+  - DADOUR,ARMEN
   title: TALES OF THE NILE
   dewey: 372.65 DAD
   entry_numbers:
   - '14058'
   editor: None // CALIFORNIA
   edition_year: 2001
   pages: 63
@@ -572173,15 +572033,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11367
   authors:
-  - ALEXANDROS YANNIS
+  - YANNIS,ALEXANDROS
   title: KOSOVO UNDER INTERNATIONAL ADMISTRATION
   subtitle: AN UNFINISHED CONFLICT
   dewey: 372.65 YAN
   entry_numbers:
   - '14057'
   editor: ELIAMEP // ΑΘΗΝΑ
   edition_year: 2001
@@ -572325,15 +572185,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11370
   authors:
-  - ΒΑΛΗΝΑΚΗΣ Γ., ΚΟΥΛΟΥΜΠΗΣ Θ.
+  - ΒΑΛΗΝΑΚΗΣ,Γ.
+  - ΚΟΥΛΟΥΜΠΗΣ,Θ.
   language: el
   title: ΕΠΕΤΗΡΙΔΑ ΑΜΥΝΤΙΚΗΣ & ΕΞΩΤΕΡΙΚΗΣ ΠΟΛΙΤΙΚΗΣ
   subtitle: Η ΕΛΛΑΔΑ ΚΑΙ Ο ΚΟΣΜΟΣ
   dewey: '327.495'
   entry_numbers:
   - '13540'
   editor: ΠΑΡΑΤΗΡΗΤΗΣ // ΑΘΗΝΑ
@@ -573374,15 +573235,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 11391
   authors:
-  - ΑΥΓΟΥΣΤΗΣ Ν. ΜΠΑΛΚΑΣ
+  - ΜΠΑΛΚΑΣ,ΑΥΓΟΥΣΤΗΣ,Ν.
   language: el
   title: ΑΝΔΡΟΣ ΚΑΙ ΧΑΛΙΚΙΔΙΚΗ
   dewey: 027 ΜΠΑ
   entry_numbers:
   - '14044'
   editor: ΚΑΙΡΕΙΟΣ ΒΙΒΛΙΟΘΗΚΗ // ΑΝΔΡΟΣ
   edition_year: 1998
@@ -575311,15 +575172,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11430
   authors:
-  - ΑΝΤΩΝΙΟΣ ΕΠΑΜΕΙΝΩΝΔΑΣ ΣΠΗΛΙΩΤΟΠΟΥΛΟΣ
+  - ΣΠΗΛΙΩΤΟΠΟΥΛΟΣ,ΑΝΤΩΝΙΟΣ,ΕΠΑΜΕΙΝΩΝΔΑΣ
   language: el
   title: ΓΥΝΑΙΚΕΣ ΑΦΘΟΝΕΣ
   dewey: 889.21 ΣΠΗ
   entry_numbers:
   - '13994'
   editor: None // ΑΘΗΝΑ
   edition_year: 2000
@@ -576757,15 +576618,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11459
   authors:
-  - ΑΓΑΠΗΤΟΥ,ΙΩΣΗΦ
+  - ΑΓΑΠΗΤΟΣ,ΙΩΣΗΦ
   language: el
   title: ΥΠΑΡΧΕΙ ΘΕΟΣ ΑΓΑΠΗΣ ;
   dewey: 230 ΑΓΑ
   entry_numbers:
   - '14139'
   editor: None // ΑΘΗΝΑ
   pages: 107
@@ -576903,29 +576764,30 @@
     29: null
     30: null
 - dbase_number: 11462
   authors:
   - ΠΕΡΙΟΔΙΚΟ
   language: el
   title: ΟΡΥΚΤΑ ΚΑΙ ΟΡΥΧΕΙΑ
+  dewey: 050 ΠΕΡ
   entry_numbers:
   - '14142'
   pages: 169
   topics:
   - ΠΕΡΙΟΔΙΚΟ
   donors:
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 11462
     1: ΠΕΡΙΟΔΙΚΟ
     2: ΟΡΥΚΤΑ ΚΑΙ ΟΡΥΧΕΙΑ
-    4: Ο50ΠΕΡ
+    4: 050ΠΕΡ
     5: '14142'
     11: 169Σ
     12: ΠΕΡΙΟΔΙΚΟ
     13: ΠΕΡΙΟΔΙΚΟ
     14: ΠΕΡΙΟΔΙΚΟ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
     3: null
@@ -576948,28 +576810,29 @@
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11463
   authors:
   - ΠΕΡΙΟΔΙΚΟ
+  dewey: 050 ΠΕΡ
   entry_numbers:
   - '14141'
   pages: 64
   topics:
   - ΠΕΡΙΟΔΙΚΟ
   donors:
   - ΠΟΡΤΟΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 11463
     1: ΠΕΡΙΟΔΙΚΟ
-    4: Ο50ΠΕΡ
+    4: 050ΠΕΡ
     5: '14141'
     11: 64Σ
     12: ΠΕΡΙΟΔΙΚΟ
     13: ΠΕΡΙΟΔΙΚΟ
     14: ΠΕΡΙΟΔΙΚΟ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
     2: null
@@ -577736,15 +577599,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11479
   authors:
-  - ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ
+  - ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ,M.
   language: el
   title: ΑΤΘΙΔΕΣ ΑΥΡΑΙ
   dewey: 889.21 ΒΙΖ
   entry_numbers:
   - '14163'
   editor: ΛΑΜΠΡΑΚΗΣ // None
   edition_year: 2014
@@ -578828,15 +578691,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11501
   authors:
-  - ΒΑΛ,ΖΑΝ
+  - WAHL,JEAN
   language: el
   title: ΕΙΣΑΓΩΓΗ ΣΤΙΣ ΦΙΛΟΣΟΦΙΕΣ ΤΟΥ ΥΠΑΡΞΙΣΜΟΥ
   dewey: 101 ΒΑΛ
   entry_numbers: []
   translators:
   - ΜΑΛΕΒΙΤΣΗΣ,ΧΡΗΣΤΟΣ
   editor: ΔΩΔΩΝΗ // ΑΘΗΝΑ
@@ -579180,15 +579043,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11508
   authors:
-  - ΑΘΑΝΑΣΟΠΟΥΛΟΥ,ΔΗΜΗΤΡΙΟΥ
+  - ΑΘΑΝΑΣΟΠΟΥΛΟΣ,ΔΗΜΗΤΡΙΟΣ
   language: el
   title: ΤΟ ΚΟΡΑΝΙΟ ΚΑΙ Η ΕΛΕΥΘΕΡΙΑ ΤΟΥ ΕΥΑΓΓΕΛΙΟΥ
   dewey: 230 ΑΘΑ
   entry_numbers:
   - '15009'
   edition: Β
   editor: ΠΑΝΑΓΟΠΟΥΛΟΣ // ΑΘΗΝΑ
@@ -580488,14 +580351,15 @@
     29: null
     30: null
 - dbase_number: 11534
   authors:
   - ΠΕΡΙΟΔΙΚΟ
   language: el
   title: ΘΕΣΕΙΣ ΚΑΙ ΙΔΕΑΙ
+  dewey: 050 ΠΕΡ
   entry_numbers:
   - '15019'
   edition_year: 1970
   pages: 63
   topics:
   - ΠΕΡΙΟΔΙΚΟ
   donors:
@@ -580504,15 +580368,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 11534
     1: ΠΕΡΙΟΔΙΚΟ
     2: ΘΕΣΕΙΣ ΚΑΙ ΙΔΕΑΙ
-    4: Ο50ΠΕΡ
+    4: 050ΠΕΡ
     5: '15019'
     10: '1970'
     11: 63Σ
     12: ΠΕΡΙΟΔΙΚΟ
     13: ΠΕΡΙΟΔΙΚΟ
     14: ΠΕΡΙΟΔΙΚΟ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
@@ -580832,15 +580696,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11541
   authors:
-  - ΘΑΒΩΡΗΣ,Α
+  - ΘΑΒΩΡΗΣ,Α,
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΓΛΩΣΣΑΣ
   dewey: 938.498 ΘΑΒ
   entry_numbers:
   - '15001'
   editor: None // ΙΩΑΝΝΙΝΑ
   edition_year: 1971
@@ -581275,15 +581139,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 11550
   authors:
-  - ΒΟΚΑΚΙΟΣ
+  - BOCCACCIO,GIOVANNI
   language: el
   title: ΔΕΚΑΗΜΕΡΟΝ
   dewey: 873 ΒΟΚ
   entry_numbers:
   - '15062'
   editor: ΓΡΑΜΜΑΤΑ // ΑΘΗΝΑ
   edition_year: 1993
@@ -582043,15 +581907,18 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 11565
   authors:
-  - ΑΡΧΙΛΟΧΟΣ,ΣΙΜΩΝΙΔΗΣ,ΑΝΑΚΡΕΩΝ,ΑΛΚΑΙΟΣ,ΣΑΠ
+  - ΑΡΧΙΛΟΧΟΣ
+  - ΣΙΜΩΝΙΔΗΣ
+  - ΑΝΑΚΡΕΩΝ
+  - ΑΛΚΑΙΟΣ!ΣΑΠ
   language: el
   title: ΛΥΡΙΚΗ ΠΟΙΗΣΗ
   dewey: 880.08 ΑΝΑ
   entry_numbers:
   - '15089'
   editor: NATIONAL GEOGRAPHIC // ΑΘΗΝΑ
   edition_year: 2012
@@ -582198,15 +582065,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 11568
   authors:
-  - ΒΛΑΣΙΟΥ ΜΟΝΑΧΟΥ ΑΓΙΟΡΕΙΤΟΥ
+  - ΒΛΑΣΙΟΣ,ΜΟΝΑΧΟΣ ΑΓΙΟΡΕΙΤΗΣ
   language: el
   title: ΟΙ ΑΣΚΗΤΕΣ ΚΑΙ ΤΑ ΣΠΗΛΑΙΑ ΤΟΥ ΑΓΟΥΥ ΟΡΟΥΣ
   dewey: 230 ΒΛΑ
   entry_numbers:
   - '15065'
   pages: 135
   topics:
@@ -582733,15 +582600,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11579
   authors:
-  - Β. ΚΑΛΦΑΣ ΚΑΙ Γ. ΖΩΓΡΑΦΙΔΗΣ
+  - ΚΑΛΦΑΣ,Β.
+  - ΖΩΓΡΑΦΙΔΗΣ,Γ.
   language: el
   title: ΑΡΧΑΙΟΙ ΕΛΛΗΝΕΣ ΦΙΛΟΣΟΦΟΙ
   dewey: 880.07 ΚΑΛ
   entry_numbers:
   - '15081'
   editor: ΤΟ ΒΗΜΑ // None
   edition_year: 2013
@@ -583709,15 +583577,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11599
   authors:
-  - ΑΡΓΥΡΗΣ ΤΣΑΚΙΡΗΣ
+  - ΤΣΑΚΙΡΗΣ,ΑΡΓΥΡΗΣ
   language: el
   title: ΤΟ ΔΙΚΟ ΜΑΣ ΚΡΑΣΙ
   dewey: 641.22 ΤΣΙ
   entry_numbers:
   - '15068'
   editor: ΨΥΧΑΛΟΥ // None
   edition_year: 2012
@@ -583760,15 +583628,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11600
   authors:
-  - ΒΑΣΙΛΙΚΗ ΛΑΖΟΥ
+  - ΛΑΖΟΥ,ΒΑΣΙΛΙΚΗ
   language: el
   title: Η ΠΑΝΑΓΙΑ ΤΩΝ ΕΛΛΗΝΩΝ
   dewey: 230 ΛΑΖ
   entry_numbers:
   - '15055'
   pages: 94
   topics:
@@ -585595,15 +585463,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11636
   authors:
-  - ΑΝΤΛΕΡ,ΑΛΦΡΕΝΤ
+  - ADLER,ALFRED
   language: el
   title: Ο ΝΙΤΣΕ ΚΑΙ Η ΦΙΛΟΣΟΦΙΑ ΤΟΥ
   dewey: 101 ΑΝΤ
   entry_numbers:
   - '15151'
   translators:
   - ΑΝΔΡΟΥΛΙΔΑΚΗ,Ε.
@@ -586578,15 +586446,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11655
   authors:
-  - ΑΓΙΟΥ ΝΕΚΤΑΡΙΟΥ
+  - ΚΕΦΑΛΑΣ,ΑΓΙΟΣ ΝΕΚΤΑΡΙΟΣ,ΠΕΝΤΑΠΟΛΕΩΣ
   language: el
   title: ΠΕΡΙ ΑΛΗΘΟΥΣ ΚΑΙ ΨΕΥΔΟΥΣ ΜΟΡΦΩΣΕΩΣ
   dewey: 230 ΝΕΚ
   entry_numbers:
   - '15130'
   editor: ΝΕΚ.ΠΑΝΑΓΟΠΟΥΛΟΣ // ΑΘΗΝΑ
   pages: 48
@@ -586676,15 +586544,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11657
   authors:
-  - ΑΡΧΙΕΠΙΣΚΟΠΟΣ ΧΡΙΣΤΟΔΟΥΛΟΣ
+  - ΧΡΙΣΤΟΔΟΥΛΟΣ,ΑΡΧΙΕΠΙΣΚΟΠΟΣ
   language: el
   title: ΓΑΤΙ ΓΙΝΑΜΕ ΧΡΙΣΤΙΑΝΟΙ
   subtitle: Η ΜΕΤΑΒΑΣΗ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ ΑΠΟ ΤΗΝ ΑΡΧΑΙΑ ΘΡΗΣΚΕΙΑ ΣΤΟΝ ΧΡΙΣΤ
   dewey: 230 ΧΡΙ
   entry_numbers:
   - '15118'
   editor: ΧΡΙΣΤΙΑΝΙΚΗ ΒΙΒΛΙΟΘΗ // ΑΘΗΝΑ
@@ -586827,15 +586695,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11660
   authors:
-  - ΒΕΛΙΜΙΡΟΒΙΤΣ,ΑΓΙΟΥ ΝΙΚΟΛΑΟΥ
+  - ΒΕΛΙΜΙΡΟΒΙΤΣ,ΑΓΙΟΣ ΝΙΚΟΛΑΟΣ
   language: el
   title: ΑΡΓΑ ΒΑΔΙΖΕΙ Ο ΧΡΙΣΤΟΣ
   dewey: 230 ΒΕΛ
   entry_numbers:
   - '15106'
   editor: ΕΝ ΠΛΩ // ΑΘΗΝΑ
   pages: 207
@@ -588187,15 +588055,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11687
   authors:
-  - ΑΡΧΙΜ. ΕΥΣΕΒΙΟΣ
+  - ΕΥΣΕΒΙΟΣ,ΑΡΧΙΜΑΝΔΡΙΤΗΣ
   language: el
   title: ΜΙΚΡΗ ΦΙΛΟΚΑΛΙΑ
   dewey: 230 ΣΥΜ
   entry_numbers:
   - '15224'
   editor: ΑΠΟΣΤΟΛΙΚΗΣ ΔΙΑΚΟΝΙΑ // None
   pages: 302
@@ -588237,15 +588105,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11688
   authors:
-  - ΑΝΑΣΤΑΣΙΟΥ ΑΡΧΙΕΠΙΣΚΟΠΟΥ ΑΛΒΑΝΙΑΣ
+  - ΑΝΑΣΤΑΣΙΟΥ,ΑΡΧΙΕΠΙΣΚΟΠΟΥ ΑΛΒΑΝΙΑΣ
   language: el
   title: ΕΩΣ ΕΣΧΑΤΟΥ ΤΗΣ ΓΗΣ
   dewey: 230 ΑΝΑ
   entry_numbers:
   - '15226'
   editor: ΑΠΟΣΤ. ΔΙΑΚΟΝΙΑ // None
   pages: 388
@@ -591976,15 +591844,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11763
   authors:
-  - ΒΕΛΟΠΟΥΛΟΣ,ΚΥΡΙΑΚΟΣ,ΑΘΑΝΑΣΟΠΟΥΛΟΣ,ΗΛΙΑΣ
+  - ΒΕΛΟΠΟΥΛΟΣ,ΚΥΡΙΑΚΟΣ
+  - ΑΘΑΝΑΣΟΠΟΥΛΟΣ,ΗΛΙΑΣ
   language: el
   title: ΠΕΡΙ ΕΛΛΗΝΩΝ ΑΓΩΓΗΣ
   dewey: 000 ΒΕΛ
   entry_numbers:
   - '15270'
   editor: ΚΑΔΜΟΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   pages: 206
@@ -592432,15 +592301,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11772
   authors:
-  - ΑΓΓΕΛΟΣ ΠΑΝ. ΣΑΚΚΕΤΟΣ
+  - ΣΑΚΚΕΤΟΣ,ΑΓΓΕΛΟΣ,ΠΑΝ.
   language: el
   title: ΛΕΞΙΚΟ ΕΛΛΗΝΙΚΩΝ ΟΝΟΜΑΤΩΝ ΚΑΙ ΤΟΠΩΝΥΜΙΩΝ ΤΗΣ ΕΓΓΥΣ ΑΝΑΤΟΛΗΣ
   dewey: 000 ΔΙΑ
   entry_numbers:
   - '15097'
   editor: ΛΙΑΚΟΠΟΥΛΟΣ // None
   edition_year: 2009
@@ -592582,15 +592451,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11775
   authors:
-  - ΑΓΓΕΛΟΥ ΠΑΝ. ΣΑΚΚΕΤΟΥ
+  - ΣΑΚΚΕΤΟΣ,ΑΓΓΕΛΟΣ,ΠΑΝ.
   language: el
   title: ΠΟΥ ΒΡΙΣΚΟΝΤΑΙ ΤΑ ΑΡΧΑΙΑ ΕΛΛΗΝΙΚΑ ΧΕΙΡΟΓΡΑΦΑ
   dewey: 000 ΔΙΑ
   entry_numbers:
   - '15115'
   editor: ΛΙΑΚΟΠΟΥΛΟΣ // None
   pages: 458
@@ -593033,15 +592902,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11784
   authors:
-  - ΑΓΓΕΛΟΣ ΠΑΝ. ΣΑΚΚΕΤΟΣ
+  - ΣΑΚΚΕΤΟΣ,ΑΓΓΕΛΟΣ,ΠΑΝ.
   language: el
   title: Η ΑΝΩΣΤΗ ΖΩΗ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
   dewey: 000 ΛΙΑ
   entry_numbers:
   - '15159'
   editor: ΛΙΑΚΟΠΟΥΛΟΣ // None
   pages: 317
@@ -593432,15 +593301,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11792
   authors:
-  - ΑΘΑΝΑΣΙΟΣ ΑΓΓΕΛΟΠΟΥΛΟΣ
+  - ΑΓΓΕΛΟΠΟΥΛΟΣ,ΑΘΑΝΑΣΙΟΣ
   language: el
   title: ΟΙ ΓΕΝΝΗΤΡΙΕΣ ΤΟΥ ΔΙΑΣΤΗΜΑΤΟΣ
   dewey: 000 ΛΙΑ
   entry_numbers:
   - '15138'
   editor: ΛΙΑΚΟΠΟΥΛΟΣ // None
   pages: 313
@@ -593482,15 +593351,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11793
   authors:
-  - ΑΘΑΝΑΣΙΟΣ ΑΓΓΕΛΟΠΟΥΛΟΣ
+  - ΑΓΓΕΛΟΠΟΥΛΟΣ,ΑΘΑΝΑΣΙΟΣ
   language: el
   title: ΧΕΟΨ Ο ΜΕΓΑΛΟΣ ΑΡΧΙΤΕΚΤΩΝ
   dewey: 000 ΛΙΑ
   entry_numbers:
   - '15140'
   editor: ΛΙΑΚΟΠΟΥΛΟΣ // None
   pages: 368
@@ -593532,15 +593401,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11794
   authors:
-  - ΑΘΑΝΑΣΙΟΣ ΑΓΓΕΛΟΠΟΥΛΟΣ
+  - ΑΓΓΕΛΟΠΟΥΛΟΣ,ΑΘΑΝΑΣΙΟΣ
   language: el
   title: ΤΑ ΜΥΣΤΙΚΑ ΤΩΝ ΠΥΡΑΜΙΔΩΝ ΤΗΣ ΖΩΗΣ
   dewey: 000 ΛΙΑ
   entry_numbers:
   - '15137'
   editor: ΛΙΑΚΟΠΟΥΛΟΣ // None
   pages: 220
@@ -593937,15 +593806,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 11802
   authors:
-  - ΣΑΚΚΕΤΟΣ,ΑΓΓΕΛΟΣ
+  - ΣΑΚΚΕΤΟΣ,ΑΓΓΕΛΟΣ,ΠΑΝ.
   language: el
   title: Ο ΚΩΔΙΚΑΣ ΤΗΣ ΧΑΜΕΝΗΣ ΓΝΩΣΗΣ
   dewey: 000 ΣΑΚ
   entry_numbers:
   - '15100'
   editor: ΛΙΑΚΟΠΟΥΛΟΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   pages: 393
@@ -594935,15 +594804,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11822
   authors:
-  - ΣΑΚΚΕΤΟΣ,ΑΓΓΕΛΟΣ
+  - ΣΑΚΚΕΤΟΣ,ΑΓΓΕΛΟΣ,ΠΑΝ.
   language: el
   title: Η ΘΕΙΑ ΠΡΟΕΛΕΥΣΗ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΑΛΦΑΒΗΤΟΥ ΚΑΙ Ο ΓΕΩΔΑΙΤΙΚΟΣ
   subtitle: ΤΡΙΓΩΝΙΣΜΟΣ ΤΗΣ ΕΛΛΑΔΟΣ
   dewey: 000 ΣΑΚ
   entry_numbers:
   - '15286'
   editor: ΛΙΑΚΟΠΟΥΛΟΣ // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -595134,15 +595003,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11826
   authors:
-  - ΣΑΚΚΕΤΟΣ,ΑΓΓΕΛΟΣ
+  - ΣΑΚΚΕΤΟΣ,ΑΓΓΕΛΟΣ,ΠΑΝ.
   language: el
   title: ΙΣΤΟΡΙΚΕΣ ΑΠΟΔΕΙΞΕΙΣ ΠΕΡΙ ΤΗΝ ΕΛΛΗΝΙΚΟΤΗΤΑΣ ΤΗΣ ΕΓΓΥΣ ΑΝΑΤΟΛ
   subtitle: ΟΙ ΕΛΛΗΝΕΣ ΤΗΣ ΒΙΒΛΟΥ (ΠΑΛΑΙΑ ΔΙΑΘΗΚΗ)
   dewey: 000 ΣΑΚ
   entry_numbers:
   - '15217'
   editor: ΛΙΑΚΟΠΟΥΛΟΣ // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -595283,15 +595152,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11829
   authors:
-  - ΣΑΚΚΕΤΟΣ,ΑΓΓΕΛΟΣ
+  - ΣΑΚΚΕΤΟΣ,ΑΓΓΕΛΟΣ,ΠΑΝ.
   language: el
   title: Η ΚΑΡΔΙΑ ΤΗΣ ΕΛΛΑΔΟΣ
   dewey: 000 ΣΑΚ
   entry_numbers:
   - '15187'
   editor: ΛΙΑΚΟΠΟΥΛΟΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2005
@@ -595334,15 +595203,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11830
   authors:
-  - ΣΑΚΚΕΤΟΣ,ΑΓΓΕΛΟΣ
+  - ΣΑΚΚΕΤΟΣ,ΑΓΓΕΛΟΣ,ΠΑΝ.
   language: el
   title: ΠΟΥ ΒΡΙΣΚΟΝΤΑΙ ΤΑ ΑΡΧΑΙΑ ΕΛΛΗΝΙΚΑ ΧΕΙΡΟΓΡΑΦΑ 2
   dewey: 000 ΣΑΚ
   entry_numbers:
   - '15115'
   editor: ΛΙΑΚΟΠΟΥΛΟΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2005
@@ -596320,15 +596189,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11849
   authors:
-  - ΒΕΝΙΖΕΛΟΥ,ΘΕΟΔΟΣΙΟΥ
+  - ΒΕΝΙΖΕΛΟΣ,ΘΕΟΔΟΣΙΟΣ
   language: el
   title: ΠΕΡΙ ΤΟΥ ΙΔΙΩΤΙΚΟΥ ΒΙΟΥ ΤΩΝ ΑΡΧΑΙΩΝ ΕΛΛΗΝΩΝ
   dewey: 938 ΒΕΝ
   entry_numbers:
   - '15322'
   editor: ΔΗΜΙΟΥΡΓΙΑ // ΑΘΗΝΑ
   edition_year: 1995
@@ -596528,15 +596397,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11853
   authors:
-  - ΒΑΡΤΣΟΥ,ΙΩΑΝΝΟΥ
+  - ΒΑΡΤΣΟΣ,ΙΩΑΝΝΗΣ,Α.
   language: el
   title: ΔΥΤΙΚΗ ΠΟΛΙΤΙΚΗ ΤΩΝ ΑΘΗΝΩΝ ΚΑΤΑ ΤΟΝ ΠΕΜΠΤΟΝ Π.Χ ΑΙΩΝΑ
   dewey: 938 ΒΑΡ
   entry_numbers:
   - '16318'
   editor: ΙΜΙΑΧ // ΙΩΑΝΝΙΝΑ
   edition_year: 1978
@@ -598274,15 +598143,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11888
   authors:
-  - ΒΕΙΝ ΠΟΙΛ
+  - VEYNE,PAUL
   language: el
   title: ΟΙ ΕΛΛΗΝΕΣ ΠΙΣΤΕΥΑΝ ΣΤΟΥΣ ΜΥΘΟΥΣ ΤΟΥΣ;
   dewey: 938 ΒΕΙ
   entry_numbers:
   - '15394'
   translators:
   - ΤΣΑΓΚΑΣ,ΝΙΚΟΣ Μ.
@@ -598840,15 +598709,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11899
   authors:
-  - ΑΝΤΕΡΣΟΝ,ΠΕΡΥ
+  - ANDERSON,PERRY
   language: el
   title: ΑΠΟ ΤΗΝ ΑΡΧΑΙΟΤΗΤΑ ΣΤΟΝ ΦΕΟΥΔΑΡΧΙΣΜΟ
   dewey: 938.498 ΑΝΤ
   entry_numbers:
   - '15305'
   editor: ΟΔΥΣΣΕΑΣ // ΑΘΗΝΑ
   edition_year: 1981
@@ -599388,15 +599257,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11910
   authors:
-  - ΒΑΒΑΡΕΤΟΥ,Γ,Α,
+  - ΒΑΒΑΡΕΤΟΣ,ΓΕΩΡΓΙΟΣ,ΑΧΙΛ.
   language: el
   title: ΑΣΤΙΚΟΣ ΚΩΔΙΞ
   dewey: 346.495 ΒΑΒ
   entry_numbers:
   - '13750'
   editor: ΣΑΚΚΟΥΛΑ // ΑΘΗΝΑ
   edition_year: 1978
@@ -600045,15 +599914,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11923
   authors:
-  - ΑΒΡΑΜΙΔΗ,ΔΗΜΗΤΡΙΟΥ
+  - ΑΒΡΑΜΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
   language: el
   title: Η ΙΔΙΟΤΥΠΙΑ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΠΡΟΒΛΗΜΑΤΟΣ
   subtitle: ΕΙΣΑΓΩΓΗ ΕΙΣ ΤΗΝ ΔΗΜΟΣΙΟΤΗΤΑ
   dewey: 338.9 ΑΒΡ
   entry_numbers:
   - '15337'
   editor: TRANSORIENT // ΑΘΗΝΑ
@@ -602661,15 +602530,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11975
   authors:
-  - ΒΛΑΧΟΥ,Γ.Κ
+  - ΒΛΑΧΟΣ,ΓΕΩΡΓΙΟΣ,Κ.
   language: el
   title: ΠΟΛΙΤΙΚΗ ΘΕΩΡΙΑ
   subtitle: ΕΙΣΑΓΩΓΙΚΕΣ ΕΝΝΟΙΕΣ
   dewey: 320.01 ΒΛΑ
   entry_numbers:
   - '15407'
   editor: ΠΑΠΑΖΗΣΗ // ΑΘΗΝΑ
@@ -603785,15 +603654,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 11997
   authors:
-  - ΒΥΣΣΟΥΛΗ,ΠΑΝΤΕΛΗ
+  - ΒΥΣΣΟΥΛΗΣ,ΠΑΝΤΕΛΗΣ
   language: el
   title: Ο ΜΑΚΕΔΟΝΙΚΟΣ ΕΛΛΗΝΙΣΜΟΣ
   subtitle: ΑΓΩΝΕΣ ΚΑΙ ΘΥΣΙΕΣ ΑΙΩΝΩΝ
   dewey: 938 ΒΥΣ
   entry_numbers:
   - '15457'
   editor: None // ΑΘΗΝΑ
@@ -604329,15 +604198,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12008
   authors:
-  - ANDRONICOS,MANOLIS
+  - ΑΝΔΡΟΝΙΚΟΣ,ΜΑΝΩΛΗΣ
   title: THESSALONIKE MUSEUM
   dewey: 708.956 AND
   entry_numbers:
   - '15463'
   editor: TRAVEL GUIDE // ΑΘΗΝΑ
   edition_year: 1992
   pages: 79
@@ -604916,15 +604785,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12020
   authors:
-  - ΑΝΑΓΝΩΣΤΟΥ,ΤΑΣΟΥ
+  - ΑΝΑΓΝΩΣΤΟΥ,ΤΑΣΟΣ,Γ.
   language: el
   title: ΕΝΑΣ ΙΣΚΙΟΣ ΣΤΗΝ ΠΟΛΗ
   dewey: 889.1 ΑΝΑ
   entry_numbers:
   - '15773'
   editor: ΔΩΔΕΚΑΤΗ ΩΡΑ // ΑΘΗΝΑ
   edition_year: 1972
@@ -605116,15 +604985,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12024
   authors:
-  - ΑΣΛΑΝΙΔΗΣ,Ε.Γ
+  - ΑΣΛΑΝΙΔΗΣ,ΕΠΑΜΕΙΝΩΝΔΑΣ,Γ.
   language: el
   title: ΕΛΛΗΝ ΕΝ ΛΟΝΔΙΝΩ
   dewey: 889.1 ΑΣΛ
   entry_numbers:
   - '15776'
   editor: ΠΛΕΘΡΟΝ // ΑΘΗΝΑ
   edition_year: 1979
@@ -605415,15 +605284,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12030
   authors:
-  - ΒΑΚΑΛΗ,ΓΕΩΡΓΙΟΥ
+  - ΒΑΚΑΛΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΑΝΕΣΠΕΡΗ ΜΕΡΑ
   dewey: 889.1 ΒΑΚ
   entry_numbers:
   - '15782'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1984
@@ -607516,15 +607385,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12072
   authors:
-  - ΑΛΙΚΑΚΟΥ,ΝΙΚΟΛΑΟΥ
+  - ΑΛΙΚΑΚΟΣ,ΝΙΚΟΛΑΟΣ
   language: el
   title: ΑΓΩΓΗ ΤΟΥ ΠΟΛΙΤΟΥ
   dewey: 320.04 ΑΛΙ
   entry_numbers:
   - '15527'
   editor: ΣΙΔΕΡΗ // ΑΘΗΝΑ
   edition_year: 1960
@@ -607566,15 +607435,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12073
   authors:
-  - ΒΟΛΟΝΑΚΗ,ΜΙΧΑΗΛ
+  - ΒΟΛΟΝΑΚΗΣ,ΜΙΧΑΗΛ
   language: el
   title: ΑΓΩΓΗ ΤΟΥ ΠΟΛΙΤΟΥ
   dewey: 320.04 ΒΟΛ
   entry_numbers:
   - '15526'
   editor: ΜΑΝΖΤΕΒΕΛΑΚΗ // ΑΘΗΝΑ
   edition_year: 1914
@@ -607715,15 +607584,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12076
   authors:
-  - ΑΙΔΑΛΗ,ΒΑΣΙΛΕΙΟΥ
+  - ΑΙΔΑΛΗΣ,ΒΑΣΙΛΕΙΟΣ
   language: el
   title: ΑΙ ΠΑΡΕΚΤΡΟΠΑΙ ΤΟΥ ΤΥΠΟΥ
   dewey: 343.099 ΑΙΔ
   entry_numbers:
   - '15520'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1966
@@ -608214,15 +608083,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12086
   authors:
-  - ΑΘΑΝΑΣΟΥΛΗΣ,ΚΡΙΤΩΝΟΣ
+  - ΑΘΑΝΑΣΟΥΛΗΣ,ΚΡΙΤΩΝΑΣ
   language: el
   title: ΣΗΜΕΡΑ Η ΠΟΙΗΣΗ
   dewey: 889.1 ΑΘΑ
   entry_numbers:
   - '15506'
   editor: ΟΙΚΟΝΟΜΟΥ // ΑΘΗΝΑ
   edition_year: 1972
@@ -608465,15 +608334,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12091
   authors:
-  - ΒΑΡΥΜΠΟΠΙΩΤΗ,ΑΘΑΝ.
+  - ΒΑΡΥΜΠΟΠΙΩΤΗΣ,ΑΘΑΝΑΣΙΟΣ
   language: el
   title: ΑΣΤΙΚΟΣ ΚΩΔΙΞ ΚΑΙ ΕΙΣΑΓΩΓΙΚΟΣ ΝΟΜΟΣ
   dewey: 345.04 ΒΑΡ
   entry_numbers:
   - '15533'
   editor: ΣΑΚΚΟΥΛΑ // ΑΘΗΝΑ
   edition_year: 1961
@@ -608565,15 +608434,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12093
   authors:
-  - ΒΑΛΛΗΝΔΑ,ΠΕΤΡΟΥ
+  - ΒΑΛΛΗΝΔΑΣ,ΠΕΤΡΟΣ
   language: el
   title: ΕΙΣΑΓΩΓΗ ΕΙΣ ΤΟ ΣΥΓΚΡΙΤΙΚΟΝ ΔΙΚΑΙΟΝ
   dewey: 345.04 ΒΑΛ
   entry_numbers:
   - '15485'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1951
@@ -608819,15 +608688,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12098
   authors:
-  - ΑΛΕΞΙΑΔΗ,ΣΤΕΡΓΙΟΥ
+  - ΑΛΕΞΙΑΔΗΣ,ΣΤΕΡΓΙΟΣ
   language: el
   title: ΟΙ ΕΠΑΙΤΑΙ ΕΙΣ ΤΗΝ ΠΕΡΙΦΕΡΕΙΑΝ ΤΟΥ ΠΡΩΤΟΔΙΚΕΙΟΥ ΘΕΣΣΑΛΟΝΙΚΗΣ
   dewey: 341.242 ΑΛΕ
   entry_numbers:
   - '15501'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1966
@@ -608968,15 +608837,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12101
   authors:
-  - ΑΙΝΣΤΑΙΝ,ΑΛΜΠΕΡΤ
+  - EINSTEIN,ALBERT
   language: el
   title: Ο ΣΗΜΕΡΙΝΟΣ ΚΟΣΜΟΣ
   dewey: 190 ΑΙΝ
   entry_numbers:
   - '15496'
   translators:
   - ΖΩΓΡΑΦΟΥ-ΜΕΡΑΝΑΙΟΥ,ΜΙΝΑ
@@ -609570,15 +609439,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12113
   authors:
-  - ADAMS,TRASLOW-JAMES
+  - TRUSLOW ADAMS,JAMES
   language: el
   title: Η ΕΠΟΠΟΙΙΑ ΤΗΣ ΑΜΕΡΙΚΗΣ
   dewey: 973 ADA
   entry_numbers:
   - '15517'
   editor: ΑΕΤΟΣ // ΑΘΗΝΑ
   edition_year: 1951
@@ -609719,15 +609588,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12116
   authors:
-  - ΑΛΒΑΝΟΥ,ΧΡΗΣΤΟΥ
+  - ΑΛΒΑΝΟΣ,ΧΡΗΣΤΟΣ
   language: el
   title: ΜΑΤΙΕΣ ΣΤΗΝ ΕΞΕΛΙΞΗ ΤΟΥ ΑΝΘΡΩΠΟΥ
   dewey: 909 ΑΛΒ
   entry_numbers:
   - '15500'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1967
@@ -610962,15 +610831,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12141
   authors:
-  - ΒΑΡΒΙΤΣΙΩΤΗ,ΤΑΚΗ
+  - ΒΑΡΒΙΤΣΙΩΤΗΣ,ΤΑΚΗΣ
   language: el
   title: ΤΟ ΠΕΠΛΟ ΚΑΙ ΤΟ ΧΑΜΕΓΕΛΟ
   dewey: 889.1 ΒΑΡ
   entry_numbers:
   - '15732'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1963
@@ -611704,15 +611573,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12156
   authors:
-  - ΒΡΑΧΑ,ΦΡΙΞΟΥ
+  - ΒΡΑΧΑΣ,ΦΡΙΞΟΣ
   language: el
   title: ΖΩΗ ΚΑΙ ΠΡΟΠΑΓΑΝΔΑ ΣΤΗΝ ΑΡΧΑΙΑ ΕΛΛΑΔΑ
   dewey: 303.380 ΒΡΑ
   entry_numbers:
   - '15547'
   editor: None // ΑΘΗΝΑ
   edition_year: 1981
@@ -612298,15 +612167,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12168
   authors:
-  - ΑΡΓΥΡΟΥ,ΓΙΑΝΝΗ
+  - ΑΡΓΥΡΟΣ,ΓΙΑΝΝΗΣ
   language: el
   title: ΜΕΛΩΔΙΚΑΙ ΑΣΚΗΣΕΙΣ ΚΑΙ ΜΟΥΣΙΚΗ ΕΠΙΦΥΛΛΙΣ
   dewey: 781.07 ΑΡΓ
   entry_numbers:
   - '15540'
   editor: None // ΑΘΗΝΑ
   pages: 155
@@ -612593,15 +612462,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 12174
   authors:
-  - ANGELLUCCI ENZO
+  - ANGELUCCI,ENZO
   language: el
   title: ΟΙ ΜΕΓΑΛΟΙ ΟΛΩΝ ΤΩΝ ΕΠΟΧΩΝ
   subtitle: ΓΚΑΙΤΕ-ΝΤΑ ΒΙΝΤΣΙ-ΚΟΛΟΜΒΟΣ
   dewey: 920 ANG
   entry_numbers:
   - '15804'
   editor: ΟΡΓ ΕΥΡΩΠ ΕΚΔΟΣΕΩΝ // ΑΘΗΝΑ
@@ -612643,15 +612512,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 12175
   authors:
-  - ΑΝΔΡΟΥΤΣΟΠΟΥΛΟΣ ΔΗΜ
+  - ΑΝΔΡΟΥΤΣΟΠΟΥΛΟΣ,ΔΗΜΗΤΡΙΟΣ
   language: el
   title: ΠΡΑΚΤΙΚΟΣ ΔΙΚΗΓΟΡΟΣ
   dewey: 340.094 ΑΝΔ
   entry_numbers:
   - '15711'
   editor: ΠΗΓΑΣΟΣ // ΑΘΗΝΑ
   topics:
@@ -612742,15 +612611,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12177
   authors:
-  - ΒΑΡΒΙΤΣΙΩΤΗΣ ΤΑΚΗΣ
+  - ΒΑΡΒΙΤΣΙΩΤΗΣ,ΤΑΚΗΣ
   title: FRAGMENTA
   subtitle: Η ΒΛΑΣΤΗΣΗ ΤΩΝ ΟΡΥΚΤΩΝ
   dewey: 889.1 ΒΑΡ
   entry_numbers:
   - '15625'
   editor: ΠΑΡΑΤΗΡΗΤΗΣ // None
   edition_year: 1985
@@ -612842,15 +612711,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12179
   authors:
-  - WEBSTER T.B.L.
+  - WEBSTER,THOMAS,BERTRAM LONSDALE
   title: ENERYDAY LIFE IN CLASSICAL ATHENS
   dewey: 372.65 WEB
   entry_numbers:
   - '15660'
   editor: BATSFORD // LONDON
   edition_year: 1969
   pages: 192
@@ -613944,15 +613813,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12201
   authors:
-  - ΑΡΧΙΜΑΝΔΡΙΤΗΣ ΓΕΩΡΓΙΟΣ
+  - ΓΕΩΡΓΙΟΣ,ΑΡΧΙΜΑΝΔΡΙΤΗΣ
   language: el
   title: ΤΟ ΕΡΓΟ ΤΩΝ ΑΓΙΩΝ ΚΥΡΙΛΛΟΥ ΚΑΙ ΜΕΘΟΔΙΟΥ ΚΑΙ ΤΟ ΜΗΝΥΜΑ ΤΟΥΣ Π
   subtitle: ΡΟΣ ΤΟΥΣ ΣΥΓΧΡΟΝΟΥΣ ΟΡΘΟΔΟΞΟΥΣ ΛΑΟΥΣ
   dewey: 230 ΓΕΩ
   entry_numbers:
   - '15595'
   editor: ΜΗΝΥΜΑ // ΑΘΗΝΑ
@@ -614748,15 +614617,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12217
   authors:
-  - ΑΡΜΑΟΥ,ΔΗΜΗΤΡΗ
+  - ΑΡΜΑΟΣ,ΔΗΜΗΤΡΗΣ
   language: el
   title: ΠΟΙΗΜΑΤΑ (1979-1984)
   dewey: 889.1 ΑΡΜ
   entry_numbers:
   - '15622'
   editor: GUTENBERG // ΑΘΗΝΑ
   edition_year: 1985
@@ -615600,15 +615469,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12234
   authors:
-  - ΒΑΦΟΠΟΥΛΟΣ,Γ.Θ
+  - ΒΑΦΟΠΟΥΛΟΣ,Γ.,Θ.
   language: el
   title: ΣΕΛΙΔΕΣ ΑΥΤΟΒΙΟΓΡΑΦΙΑΣ
   subtitle: ΤΑΞΙΔΙΑ ΚΑΙ ΠΑΡΕΝΘΕΣΕΙΣ
   dewey: 889.14 ΒΑΦ
   entry_numbers:
   - '15631'
   editor: ΡΟΔΗ // ΑΘΗΝΑ
@@ -615701,15 +615570,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12236
   authors:
-  - ΒΙΤΑΛΗ,ΦΙΛΑΡΕΤΟΥ
+  - ΒΙΤΑΛΗΣ,ΦΙΛΑΡΕΤΟΣ
   language: el
   title: ΣΙΦΝΟΣ-ΠΑΤΜΟΣ
   dewey: 230 ΒΙΤ
   entry_numbers:
   - '15576'
   editor: None // ΑΘΗΝΑ
   edition_year: 1988
@@ -615851,15 +615720,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12239
   authors:
-  - ΒΑΚΑΛΗΣ,Γ.Α
+  - ΒΑΚΑΛΗΣ,Γ.,Α.
   language: el
   title: ΟΡΘΟΔΟΞΙΑ
   dewey: 889.1 ΒΑΚ
   entry_numbers:
   - '15626'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1990
@@ -616453,15 +616322,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12251
   authors:
-  - ΑΜΑΝΤΟΥ,Κ.
+  - ΑΜΑΝΤΟΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ,Ι.
   language: el
   title: ΣΥΝΤΟΜΟΣ ΙΣΤΟΡΙΑ ΤΗΣ ΙΕΡΑΣ ΜΟΝΗΣ ΤΟΥ ΣΙΝΑ
   dewey: 230 ΑΜΑ
   entry_numbers:
   - '15578'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1953
@@ -616853,15 +616722,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12259
   authors:
-  - ΑΝΑΓΝΩΣΤΟΠΟΥΛΟΥ,ΓΙΩΡΓΟΥ
+  - ΑΝΑΓΝΩΣΤΟΠΟΥΛΟΣ,ΓΙΩΡΓΟΣ
   language: el
   title: ΟΙ ΥΜΝΟΙ ΤΟΥ ΠΑΝΗΓΥΡΙΚΟΥ ΕΣΠΕΡΙΝΟΥ
   dewey: 230 ΑΝΑ
   entry_numbers:
   - '15601'
   editor: None // ΑΘΗΝΑ
   pages: 153
@@ -617408,15 +617277,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12270
   authors:
-  - ΒΑΚΑΛΟΠΟΥΛΟΣ,ΚΩΝ/ΝΟΣ
+  - ΒΑΚΑΛΟΠΟΥΛΟΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΤΟ ΜΑΚΕΔΟΝΙΚΟ ΖΗΤΗΜΑ 1856-1913
   dewey: 938.498 ΒΑΚ
   entry_numbers:
   - '15619'
   editor: ΤΟ ΒΗΜΑ // ΑΘΗΝΑ
   edition_year: 2009
@@ -619423,15 +619292,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12310
   authors:
-  - ΑΥΓΕΡΗ,ΜΑΡΚΟΥ
+  - ΑΥΓΕΡΗΣ,ΜΑΡΚΟΣ
   language: el
   title: ΑΙΣΘΗΤΙΚΗ
   subtitle: ΜΑΡΞΙΣΤΙΚΗ-ΛΕΝΙΝΙΣΤΙΚΗ
   dewey: 111.85 ΑΥΓ
   entry_numbers:
   - '15581'
   editor: ΟΡΙΖΟΝΤΕΣ // ΑΘΗΝΑ
@@ -620214,15 +620083,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12326
   authors:
-  - ΑΘΑΝΑΣ,Γ.
+  - ΑΘΑΝΑΣΙΑΔΗΣ-ΝΟΒΑΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΑΙΝΟΣ ΚΑΙ ΘΡΗΝΟΣ
   dewey: 889.1 ΑΘΑ
   entry_numbers:
   - '15924'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   pages: 216
@@ -620313,15 +620182,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12328
   authors:
-  - ΒΙΓΛΑΡΗ,ΠΑΝΟΥ
+  - ΒΙΓΛΑΡΗΣ,ΠΑΝΟΣ
   language: el
   title: ΑΠΟ ΤΗΝ ΚΟΚΚΙΝΗ ΜΗΛΙΑ ΕΙΣ ΤΗΝ ΚΟΚΚΙΝΗ ΕΔΕΜ
   dewey: 889.1 ΒΙΓ
   entry_numbers:
   - '15922'
   editor: None // ΑΘΗΝΑ
   edition_year: 1976
@@ -621416,15 +621285,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12350
   authors:
-  - ΑΣΛΑΝΟΓΛΟΥ,ΝΙΚΟΣ-ΑΛΕΞΗΣ
+  - ΑΣΛΑΝΟΓΛΟΥ,ΝΙΚΟΣ,ΑΛΕΞΗΣ
   language: el
   title: ΔΥΣΚΟΛΟΣ ΘΑΝΑΤΟΣ
   dewey: 889.1 ΑΣΛ
   entry_numbers:
   - '15897'
   editor: ΚΟΧΛΙΑ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1954
@@ -621517,15 +621386,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 12352
   authors:
-  - ΒΑΡΒΙΤΣΙΩΤΗ,ΤΑΚΗ
+  - ΒΑΡΒΙΤΣΙΩΤΗΣ,ΤΑΚΗΣ
   language: el
   title: Η ΜΕΤΑΜΟΡΦΩΣΗ
   dewey: 889.1 ΒΑΡ
   entry_numbers:
   - '15886'
   editor: ΕΓΝΑΤΙΑ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1971
@@ -621567,15 +621436,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12353
   authors:
-  - ΒΡΕΤΤΑΚΟΥ,ΝΙΚΗΦΟΡΟΥ
+  - ΒΡΕΤΤΑΚΟΣ,ΝΙΚΗΦΟΡΟΣ
   language: el
   title: ΟΔΟΙΠΟΡΙΑ
   dewey: 889.1 ΒΡΕ
   entry_numbers:
   - '15896'
   editor: ΔΙΟΓΕΝΗΣ // ΑΘΗΝΑ
   edition_year: 1972
@@ -621617,15 +621486,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12354
   authors:
-  - ΑΘΑΝΑΣΟΥΛΗΣ,ΚΡΙΤΩΝ
+  - ΑΘΑΝΑΣΟΥΛΗΣ,ΚΡΙΤΩΝΑΣ
   language: el
   title: ΕΝΑΣ ΠΟΙΗΤΗΣ ΣΤΟ ΔΡΟΜΟ
   subtitle: ΚΑΙ ΟΙ ΣΑΤΙΡΕΣ ΓΙΑ ΤΗ ΛΕΟΝΩΡΑ
   dewey: 889.1 ΑΘΑ
   entry_numbers:
   - '15895'
   editor: None // ΑΘΗΝΑ
@@ -623169,15 +623038,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12385
   authors:
-  - ΑΕΤΟΥΔΑΚΗ,ΔΗΜΗΤΡΗ
+  - ΑΕΤΟΥΔΑΚΗΣ,ΔΗΜΗΤΡΗΣ
   language: el
   title: ΜΕΡΕΣ ΑΓΩΝΙΑΣ ΑΠΟ ΤΟΝ ΠΥΡΗΝΙΚΟ ΚΙΝΔΥΝΟ
   dewey: 889.21 ΑΕΤ
   entry_numbers:
   - '15953'
   editor: None // ΑΘΗΝΑ
   edition_year: 1984
@@ -624175,15 +624044,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12405
   authors:
-  - ΑΝΤΑΜΙ,ΓΚΙΟΥΖΕΠΠΕ
+  - ADAMI,GIUSEPPE
   language: el
   title: ΠΟΥΤΣΙΝΙ
   dewey: 780.92 ΑΝΤ
   entry_numbers:
   - '15862'
   translators:
   - ΚΑΛΛΟΝΑ,Δ.
@@ -624577,15 +624446,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12413
   authors:
-  - ΒΟΥΤΣΑ,ΚΩΝ/ΝΟΥ
+  - ΒΟΥΤΣΑΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΤΟ ΕΓΚΛΗΜΑ ΤΗΣ ΕΞΥΒΡΙΣΕΩΣ
   dewey: 340.094 ΒΟΥ
   entry_numbers: []
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1969
   pages: 67
@@ -626235,15 +626104,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12446
   authors:
-  - ΑΛΕΞΙΑΔΗ,ΣΤΕΡΓΙΟΥ
+  - ΑΛΕΞΙΑΔΗΣ,ΣΤΕΡΓΙΟΣ
   language: el
   title: ΟΙ ΔΙΑΝΟΗΤΙΚΩΣ ΚΑΘΥΣΤΕΡΗΜΕΝΟΙ ΕΓΚΛΗΜΑΤΙΑΙ
   dewey: 330 ΑΛΕ
   entry_numbers:
   - '15837'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1971
@@ -626485,15 +626354,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12451
   authors:
-  - ΑΥΓΕΛΗ,Ν.Γ.
+  - ΑΥΓΕΛΗΣ,ΝΙΚΟΣ,Γ.
   language: el
   title: Η ΕΝΝΟΙΑ ΤΗΣ ΑΙΤΙΟΤΗΤΑΣ ΣΤΟΝ ΛΟΓΙΚΟ ΘΕΤΙΚΙΣΜΟ
   dewey: 530.01 ΑΥΓ
   entry_numbers:
   - '15836'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1971
@@ -626836,15 +626705,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12458
   authors:
-  - ΒΟΥΒΑΛΟΥΔΗ,ΔΗΜΟΣΘΕΝΟΥΣ
+  - ΒΟΥΒΑΛΟΥΔΗΣ,ΔΗΜΟΣΘΕΝΗΣ
   language: el
   title: ΣΥΜΒΟΛΗ ΕΙΣ ΤΗΝ ΜΕΛΕΤΗΝ ΤΩΝ ΜΟΝΗΡΩΝ ΚΑΚΟΗΘΩΝ ΝΕΥΡΙΜΑΤΩΝ
   dewey: 610.28 ΒΟΥ
   entry_numbers:
   - '15816'
   editor: None // ΑΘΗΝΑ
   edition_year: 1965
@@ -627401,15 +627270,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12469
   authors:
-  - ΑΛΕΞΙΑΔΗ,Σ.
+  - ΑΛΕΞΙΑΔΗΣ,ΣΤΕΡΓΙΟΣ
   language: el
   title: Η ΕΓΚΛΗΜΑΤΙΚΟΤΗΣ ΤΩΝ ΑΝΗΛΙΚΩΝ ΕΝ ΘΕΣΣΑΛΟΝΙΚΗ ΑΠΟ ΤΟΥ 1958-65
   dewey: 330 ΑΛΕ
   entry_numbers:
   - '15655'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1966
@@ -627855,15 +627724,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12478
   authors:
-  - ΑΝΔΡΙΚΑΝΗ,ΕΜΜΑΝΟΥΗΛ
+  - ΑΝΔΡΙΚΑΝΗΣ,ΕΜΜΑΝΟΥΗΛ
   language: el
   title: Η ΕΓΚΛΗΜΑΤΙΚΟΤΗΣ ΕΝ ΚΡΗΤΗ
   dewey: 330 ΑΝΔ
   entry_numbers:
   - '15808'
   editor: None // ΑΘΗΝΑ
   edition_year: 1968
@@ -627905,15 +627774,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12479
   authors:
-  - ΒΑΡΔΑΚΟΥΛΑ,ΙΩΑΝΝΟΥ
+  - ΒΑΡΔΑΚΟΥΛΑΣ,ΙΩΑΝΝΗΣ Δ.
   language: el
   title: Η ΣΥΜΜΕΤΟΧΗ ΤΩΝ ΕΡΓΑΖΟΜΕΝΩΝ ΕΙΣ ΤΑΣ ΕΠΙΧΕΙΡΗΣΕΙΣ
   dewey: 658.81 ΒΑΡ
   entry_numbers:
   - '15840'
   editor: None // ΑΘΗΝΑ
   edition_year: 1970
@@ -628255,15 +628124,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12486
   authors:
-  - ΑΓΑΠΙΔΗ,ΙΩΑΝΝΟΥ
+  - ΑΓΑΠΙΔΗΣ,ΙΩΑΝΝΗΣ
   language: el
   title: Η ΝΟΜΙΚΗ ΘΕΣΙΣ ΤΩΝ ΑΛΛΟΔΑΠΩΝ ΕΝ ΤΗ ΑΡΧΑΙΑ ΕΒΡΑΙΚΗ ΠΟΛΙΤΕΙΑ
   dewey: 938.629 ΑΓΑ
   entry_numbers:
   - '15853'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1964
@@ -629907,15 +629776,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12519
   authors:
-  - ΑΔΟΛΦΟΥ ΝΤ ΕΝΕΡΥ
+  - D'ENNERY,ADOLPHE
   language: el
   title: ΟΙ ΔΥΟ ΟΡΦΑΝΕΣ
   dewey: 886.2 ΕΝΕ
   entry_numbers:
   - '15995'
   translators:
   - ΑΡΓΥΡΟΠΟΥΛΟΥ,ΟΘ.
@@ -630404,15 +630273,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12529
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: ΣΤΗ ΧΩΡΑ ΤΩΝ ΓΟΥΝΑΡΙΚΩΝ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '15985'
   translators:
   - ΑΚΡΙΤΑ,Α.
@@ -632246,15 +632115,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12566
   authors:
-  - ΒΑΚΑΛΗΣ,Γ.Α.
+  - ΒΑΚΑΛΗΣ,Γ.,Α.
   language: el
   title: ΕΣΩΤΕΡΙΚΗ ΑΝΑΖΗΤΗΣΗ
   dewey: 889.1 ΒΑΚ
   entry_numbers:
   - '16042'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   pages: 39
@@ -632898,15 +632767,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12579
   authors:
-  - VELDE,VAN DE
+  - VAN DE VELDE,HENRY
   language: el
   title: Ο ΤΕΛΕΙΟΣ ΓΑΜΟΣ
   dewey: 306.81 VEL
   entry_numbers:
   - '16055'
   translators:
   - ΠΕΤΡΑ,ΝΕΛΛΗ
@@ -633959,15 +633828,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12600
   authors:
-  - ΑΝΘΕΜΙΔΗΣ ΑΧΙΛΛΕΑΣ
+  - ΑΝΘΕΜΙΔΗΣ,ΑΧΙΛΛΕΑΣ
   language: el
   title: ΤΑ ΑΝΩΤΑΤΑ ΕΚΠΑΙΔΕΥΤΙΚΑ ΙΔΡΥΜΑΤΑ ΕΝ ΕΛΛΑΔΙ ΑΠΟ ΤΩΝ ΑΡΧΑΙΟΤΑΤ
   subtitle: ΩΝ ΧΡΟΝΩΝ ΜΕΧΡΙ ΤΗΣ ΕΠΑΝΑΣΤΑΣΕΩΣ ΤΟΥ 1821
   dewey: 374.949 ΑΝΘ
   entry_numbers:
   - '16086'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -634159,15 +634028,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12604
   authors:
-  - ΑΙΤΜΑΤΟΦ ΤΖΙΝΓΚΙΖ
+  - AITMATOV,CHINGHIZ
   language: el
   title: ΤΖΑΜΙΛΙΑ
   dewey: 881.73 ΑΙΤ
   entry_numbers:
   - '16115'
   editor: ΘΕΜΕΛΙΟ // None
   edition_year: 1975
@@ -634706,15 +634575,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12615
   authors:
-  - ΒΑΣΙΛΕΙΟΥ Ι.
+  - ΒΑΣΙΛΕΙΟΥ,Ι.
   language: el
   title: ΣΤΙΣ ΠΑΓΟΔΕΣ ΤΟΥ ΝΕΠΑΛ
   dewey: 915.496 ΒΑΣ
   entry_numbers:
   - '16071'
   editor: ΒΙΒΛΙΟΠ ΤΗΣ ΕΣΤΙΑΣ // None
   pages: 195
@@ -634755,15 +634624,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12616
   authors:
-  - ΒΑΣΙΛΑΚΗΣ ΓΕΩΡΓΙΟΣ Β.
+  - ΒΑΣΙΛΑΚΗΣ,ΓΕΩΡΓΙΟΣ,Β.
   language: el
   title: Η ΜΑΚΕΔΟΝΙΚΗ ΦΙΛΕΚΠΑΙΔΕΥΤΙΚΗ ΑΔΕΛΦΟΤΗΣ
   dewey: 370.6 ΒΑΣ
   entry_numbers:
   - '16114'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1972
@@ -634907,15 +634776,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12619
   authors:
-  - ΒΙΓΛΑΡΗΣ ΠΑΝΟΣ
+  - ΒΙΓΛΑΡΗΣ,ΠΑΝΟΣ
   language: el
   title: ΦΙΛΟΠΑΤΩΡ ΕΝ ΟΨΕΙ ΒΑΡΒΑΡΩΝ
   dewey: 889.1 ΒΙΓ
   entry_numbers:
   - '16124'
   editor: None // ΑΘΗΝΑ
   edition_year: 1970
@@ -634957,15 +634826,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12620
   authors:
-  - ADLER ALFRED
+  - ADLER,ALFRED
   language: el
   title: ΑΝΘΡΩΠΟΓΝΩΣΙΑ
   dewey: 150.195 ADL
   entry_numbers:
   - '16090'
   editor: ΔΗΜΗΤΡΑΚΟΣ // ΑΘΗΝΑ
   edition_year: 1948
@@ -635007,15 +634876,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12621
   authors:
-  - ΑΝΔΡΙΩΤΗΣ Ν. Π.
+  - ΑΝΔΡΙΩΤΗΣ,ΝΙΚΟΛΑΟΣ,ΠΑΝΤΕΛΗΣ
   language: el
   title: ΟΙ ΠΡΟΕΛΛΗΝΕΣ
   dewey: 938 ΑΝΔ
   entry_numbers:
   - '16103'
   editor: ΕΤΑΙΡ ΜΑΚΕΔΟΝ ΣΠΟΥΔ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1953
@@ -636056,15 +635925,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12642
   authors:
-  - ΒΑΦΕΙΑΔΟΥ,ΜΑΡΙΑΣ
+  - ΒΑΦΕΙΑΔΟΥ,ΜΑΡΙΑ
   language: el
   title: Η ΕΚΚΛΗΣΙΑ ΤΟΥ ΑΓΙΟΥ ΓΕΩΡΓΙΟΥ ΣΤΑ ΘΕΣΣΑΛΙΚΑ ΑΜΠΕΛΑΚΙΑ
   dewey: 230 ΒΑΦ
   entry_numbers:
   - '16119'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1967
@@ -636502,15 +636371,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12651
   authors:
-  - ΒERTINO,SERGE
+  - BERTINO,SERGE
   title: LES CONQUERANTS DE LA TERR
   dewey: 372.65 BER
   entry_numbers:
   - '16154'
   editor: HACHETTE COLLECTION // None
   edition_year: 1974
   pages: 155
@@ -638602,15 +638471,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12694
   authors:
-  - ΒΙΚΕΛΑ,Δ.
+  - ΒΙΚΕΛΑΣ,ΔΗΜΗΤΡΙΟΣ
   language: el
   title: ΑΠΟ ΝΙΚΟΠΟΛΕΩΣ ΕΙΣ ΟΛΥΜΠΙΑΝ
   dewey: 914.95 ΒΙΚ
   entry_numbers:
   - '22979'
   editor: ΕΚΑΤΗ // ΑΘΗΝΑ
   pages: 200
@@ -638707,15 +638576,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12696
   authors:
-  - ΑΡΝΟΛ,ΖΑΚ
+  - ARNAULT,JACQUES
   language: el
   title: ΟΙ ΑΜΕΡΙΚΑΝΟΙ ΕΡΓΑΤΕΣ ΕΙΝΑΙ ΣΥΝΤΗΡΗΤΙΚΟΙ
   dewey: 330 ΑΡΝ
   entry_numbers:
   - '16170'
   translators:
   - ΒΡΑΧΝΙΑΡΗ,ΧΡ.
@@ -641889,15 +641758,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12759
   authors:
-  - ΒΕΙΚΟΥ,ΘΕΟΦΙΛΟΥ
+  - ΒΕΙΚΟΣ,ΘΕΟΦΙΛΟΣ
   language: el
   title: ΦΙΛΟΣΟΦΙΑ ΤΗΣ ΙΣΤΟΡΙΑΣ
   dewey: 901 ΒΕΙ
   entry_numbers:
   - '16198'
   editor: ΓΡΗΓΟΡΗ // ΑΘΗΝΑ
   edition_year: 1980
@@ -642092,15 +641961,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12763
   authors:
-  - ΑΓΓΕΛΙΝΟΥΔΗ,Α.Β.
+  - ΑΓΓΕΛΙΝΟΥΔΗΣ,ΑΘΑΝΑΣΙΟΣ,Β.
   language: el
   title: Η ΙΣΤΟΡΙΑ ΤΟΥ ΧΟΡΤΙΑΤΗ
   dewey: 949.565 ΑΓΓ
   entry_numbers:
   - '16246'
   editor: None // ΧΟΡΤΙΑΤΗΣ
   edition_year: 1994
@@ -642292,15 +642161,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12767
   authors:
-  - ΒΕΙΚΟΥ,ΘΕΟΦΙΛΟΥ
+  - ΒΕΙΚΟΣ,ΘΕΟΦΙΛΟΣ
   language: el
   title: ΚΟΣΜΟΛΟΓΙΑ ΚΑΙ ΚΟΣΜΙΚΗ ΔΙΚΑΙΟΣΥΝΗ ΣΤΗΝ ΑΡΧ. ΕΛΛΗΝΙΚΗ ΔΙΑΝΟΗΣ
   dewey: 182 ΒΕΙ
   entry_numbers:
   - '16240'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1969
@@ -643539,15 +643408,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12792
   authors:
-  - ΑΡΤΕΜΑΚΗ,ΣΤΕΛΙΟΥ
+  - ΑΡΤΕΜΑΚΗΣ,ΣΤΕΛΙΟΣ
   language: el
   title: ΕΛΛΗΝΙΚΕΣ ΜΟΡΦΕΣ
   dewey: 888.84 ΑΡΤ
   entry_numbers:
   - '16272'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   pages: 120
@@ -644789,15 +644658,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12817
   authors:
-  - ΒΕΤΣΙΟΣ,ΕΛΕΥΘΕΡΙΟΣ
+  - ΒΕΤΣΙΟΣ,ΕΛΕΥΘΕΡΙΟΣ,Λ.
   language: el
   title: ΤΟ ΕΜΠΟΡΙΟ ΣΤΗΝ ΠΕΡΙΟΧΗ ΤΗΣ ΑΡΤΑΣ ΤΗΝ ΠΕΡΙΟΔΟ 1449-1821Μ.Χ
   dewey: 938.993 ΒΕΤ
   entry_numbers:
   - '16286'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1995
@@ -646334,15 +646203,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12848
   authors:
-  - ΒΑΣΔΡΑΒΕΛΛΗ,Ι.Κ.
+  - ΒΑΣΔΡΑΒΕΛΛΗΣ,ΙΩΑΝΝΗΣ,Κ.
   language: el
   title: ΟΙ ΜΑΚΕΔΟΝΕΣ ΕΙΣ ΤΟΥΣ ΥΠΕΡ ΤΗΣ ΑΝΕΞΑΡΤΗΣΙΑΣ ΑΓΩΝΑΣ 1796-1832
   dewey: 938.492 ΒΑΣ
   entry_numbers:
   - '16315'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1950
@@ -647037,15 +646906,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12862
   authors:
-  - ΒΑΛΙΝΟΥ,ΓΙΑΝΝΗ
+  - ΒΑΛΙΝΟΣ,ΓΙΑΝΝΗΣ
   language: el
   title: Η ΑΜΦΙΒΟΛΙΑ
   dewey: 501 ΒΑΛ
   entry_numbers:
   - '16328'
   editor: None // ΑΘΗΝΑ
   edition_year: 1998
@@ -647087,15 +646956,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12863
   authors:
-  - ΒΑΛΙΝΟΥ,ΓΙΑΝΝΗ
+  - ΒΑΛΙΝΟΣ,ΓΙΑΝΝΗΣ
   language: el
   title: ΑΧΡΟΝΕΣ ΣΚΕΨΕΙΣ
   subtitle: ΥΠΑΡΞΙΑΚΟ ΤΕΧΝΗΜΑ
   dewey: 501 ΒΑΛ
   entry_numbers:
   - '16329'
   editor: None // ΑΘΗΝΑ
@@ -647490,15 +647359,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12871
   authors:
-  - ΑΡΜΕΝΗ,ΒΡΑΙΛΑ.Π
+  - ΑΡΜΕΝΗ,ΒΡΑΙΛΑ,Π.
   language: el
   title: ΠΕΡΙ ΠΡΩΤΩΝ ΙΔΕΩΝ ΚΑΙ ΑΡΧΩΝ
   dewey: 102 ΒΡΑ
   entry_numbers:
   - '16390'
   editor: ΦΕΞΗ // ΑΘΗΝΑ
   edition_year: 1910
@@ -648286,15 +648155,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12887
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: ΤΑΞΙΔΙ ΣΤΟ ΚΕΝΤΡΟ ΤΗΣ ΓΗΣ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '16375'
   translators:
   - ΒΡΕΤΤΑ,ΣΑΝΤΡΑ
@@ -649088,15 +648957,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12903
   authors:
-  - ΒΑΚΑΛΗΣ,Γ.Α.
+  - ΒΑΚΑΛΗΣ,Γ.,Α.
   language: el
   title: ΠΟΙΟΣ ΘΑ ΜΑΣ ΦΥΛΑΞΕΙ ΑΠΟ ΤΟΥΣ ΦΥΛΑΚΕΣ;
   dewey: 889.1 ΒΑΚ
   entry_numbers:
   - '16369'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1998
@@ -649337,15 +649206,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12908
   authors:
-  - ΒΑΛΛΗΝΔΑ,ΠΕΤΡΟΥ
+  - ΒΑΛΛΗΝΔΑΣ,ΠΕΤΡΟΣ
   language: el
   title: Η ΑΝΑΠΤΥΞΙΣ ΤΟΥ ΔΙΕΘΝΟΥΣ ΟΜΟΙΟΜΟΡΦΟΥ ΔΙΚΑΙΟΥ
   dewey: 344.01 ΒΑΛ
   entry_numbers:
   - '16363'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1958
@@ -649437,15 +649306,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12910
   authors:
-  - ΒΟΥΓΙΟΥΚΑ,ΚΩΝ/ΝΟΥ
+  - ΒΟΥΓΙΟΥΚΑΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: Η ΤΕΧΝΗ ΤΗΣ ΚΙΝΗΜΑΤΟΓΡΑΦΙΑΣ ΚΑΙ Η ΕΠΙΔΡΑΣΙΣ ΑΥΤΗΣ
   dewey: 791.43 ΒΟΥ
   entry_numbers:
   - '16361'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1963
@@ -651132,15 +651001,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12944
   authors:
-  - ΑΝΤΛΕΡ,ΑΛΦΡΕΝΤ
+  - ADLER,ALFRED
   language: el
   title: ΑΝΘΡΩΠΟΓΝΩΣΙΑ
   dewey: 150.195 ΑΝΤ
   entry_numbers:
   - '16429'
   editor: ΜΠΟΥΚΟΥΜΑΝΗ // ΑΘΗΝΑ
   edition_year: 1971
@@ -651731,15 +651600,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12956
   authors:
-  - ΑΛΒΑΝΟΥ,ΧΡΗΣΤΟΥ
+  - ΑΛΒΑΝΟΣ,ΧΡΗΣΤΟΣ
   language: el
   title: Η ΠΡΟΣΤΑΣΙΑ ΤΟΥ ΔΙΚΑΙΩΜΑΤΟΣ ΤΗΣ ΕΛΕΥΘΕΡΙΑΣ ΑΝΑΠΤΥΞΕΩΣ ΤΗΣ
   subtitle: ΠΡΟΣΩΠΙΚΟΤΗΤΟΣ
   dewey: 158.7 ΑΛΒ
   entry_numbers:
   - '16420'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -652229,15 +652098,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 12966
   authors:
-  - ΑΣΤΡΙΔΗ,ΓΕΩΡΓΙΟΥ
+  - ΑΣΤΡΙΔΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΓΕΝΙΚΗ ΜΙΚΡΟΒΙΟΛΟΓΙΑ
   dewey: 616.904 ΑΣΤ
   entry_numbers:
   - '16461'
   editor: None // ΑΘΗΝΑ
   edition_year: 1974
@@ -654348,15 +654217,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13008
   authors:
-  - ΑΠΟΣΤΟΛΟΠΟΥΛΟΣ,ΑΠΟΣΤΟΛΟΣ
+  - ΑΠΟΣΤΟΛΟΠΟΥΛΟΣ,ΑΠΟΣΤΟΛΗΣ
   language: el
   title: ΣΤΟ ΟΝΕΙΡΟ
   dewey: 889.1 ΑΠΟ
   entry_numbers:
   - '16471'
   editor: None // ΑΘΗΝΑ
   edition_year: 2002
@@ -654948,15 +654817,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13020
   authors:
-  - ATCHLEY,S.C.
+  - ATCHLEY,SHIRLEY CLIFFORD
   language: el
   title: Ο ΛΟΡΔΟΣ ΒΥΡΩΝ ΣΤΗΝ ΕΛΛΑΔΑ
   dewey: 938.545 ATC
   entry_numbers:
   - '22966'
   editor: ΒΑΓΙΟΝΑΚΗΣ // ΑΘΗΝΑ
   pages: 127
@@ -657280,15 +657149,16 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 13067
   authors:
-  - ΑΣΤΕΡΙΟΥ,ΘΕΑΝΩ-ΚΑΜΑΚΑΣ,ΓΕΩΡΓΙΟΣ
+  - ΑΣΤΕΡΙΟΥ,ΘΕΑΝΩ
+  - ΚΑΜΑΚΑΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΟΙ ΕΛΛΗΝΕΣ ΤΟΥ ΜΟΝΑΧΟΥ
   dewey: 304.8 ΑΣΤ
   entry_numbers:
   - '16557'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1989
@@ -657480,15 +657350,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13071
   authors:
-  - ΑΛΙΕΝΤΕ,ΙΖΑΜΠΕΛ
+  - ALLENDE,ISABEL
   language: el
   title: ΕΥΑ ΛΟΥΝΑ
   dewey: 863 ΑΛΙ
   entry_numbers:
   - '16545'
   translators:
   - ΣΩΤΗΡΙΑΔΟΥ-ΜΠΑΡΑΧΑΣ,ΚΛΑΙΤΗ
@@ -657533,15 +657403,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13072
   authors:
-  - ΑΛΙΕΝΤΕ,ΙΖΑΜΠΕΛ
+  - ALLENDE,ISABEL
   language: el
   title: ΤΑ ΒΑΣΙΛΕΙΟ ΤΟΥ ΧΡΥΣΟΥ ΔΡΑΚΟΝΤΑ
   dewey: 863 ΑΛΙ
   entry_numbers:
   - '16544'
   translators:
   - ΣΩΤΗΡΙΑΔΟΥ-ΜΠΑΡΑΧΑΣ,ΚΛΑΙΤΗ
@@ -657586,15 +657456,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13073
   authors:
-  - ΑΛΙΕΝΤΕ,ΙΖΑΜΠΕΛ
+  - ALLENDE,ISABEL
   language: el
   title: ΦΩΤΟΓΡΑΦΙΑ ΣΕ ΣΕΠΙΑ
   dewey: 863 ΑΛΙ
   entry_numbers:
   - '16543'
   translators:
   - ΣΩΤΗΡΙΑΔΟΥ-ΜΠΑΡΑΧΑΣ,ΚΛΑΙΤΗ
@@ -657639,15 +657509,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13074
   authors:
-  - ΑΛΙΕΝΤΕ,ΙΖΑΜΠΕΛ
+  - ALLENDE,ISABEL
   language: el
   title: ΠΑΟΥΛΑ
   dewey: 863 ΑΛΙ
   entry_numbers:
   - '16541'
   translators:
   - ΣΩΤΗΡΙΑΔΟΥ-ΜΠΑΡΑΧΑΣ,ΚΛΑΙΤΗ
@@ -657692,15 +657562,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13075
   authors:
-  - ΑΛΙΕΝΤΕ,ΙΖΑΜΠΕΛ
+  - ALLENDE,ISABEL
   language: el
   title: ΤΑ ΔΑΣΟΣ ΤΩΝ ΠΥΓΜΑΙΩΝ
   dewey: 863 ΑΛΙ
   entry_numbers:
   - '16540'
   translators:
   - ΣΩΤΗΡΙΑΔΟΥ-ΜΠΑΡΑΧΑΣ,ΚΛΑΙΤΗ
@@ -657745,15 +657615,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13076
   authors:
-  - ΑΛΙΕΝΤΕ,ΙΖΑΜΠΕΛ
+  - ALLENDE,ISABEL
   language: el
   title: Η ΠΟΛΗ ΤΩΝ ΘΗΡΙΩΝ
   dewey: 863 ΑΛΙ
   entry_numbers:
   - '16539'
   translators:
   - ΣΩΤΗΡΙΑΔΟΥ-ΜΠΑΡΑΧΑΣ,ΚΛΑΙΤΗ
@@ -657798,15 +657668,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13077
   authors:
-  - ΑΛΙΕΝΤΕ,ΙΖΑΜΠΕΛ
+  - ALLENDE,ISABEL
   language: el
   title: ΤΟ ΕΠΟΥΡΑΝΙΟ ΣΧΕΔΙΟ
   dewey: 863 ΑΛΙ
   entry_numbers:
   - '16538'
   translators:
   - ΣΩΤΗΡΙΑΔΟΥ-ΜΠΑΡΑΧΑΣ,ΚΛΑΙΤΗ
@@ -657851,15 +657721,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13078
   authors:
-  - ΑΛΙΕΝΤΕ,ΙΖΑΜΠΕΛ
+  - ALLENDE,ISABEL
   language: el
   title: ΚΟΡΗ ΤΗΣ ΜΟΙΡΑΣ
   dewey: 863 ΑΛΙ
   entry_numbers:
   - '16542'
   translators:
   - ΣΩΤΗΡΙΑΔΟΥ-ΜΠΑΡΑΧΑΣ,ΚΛΑΙΤΗ
@@ -657903,15 +657773,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13079
   authors:
-  - ΑΛΙΕΝΤΕ,ΙΖΑΜΠΕΛ
+  - ALLENDE,ISABEL
   language: el
   title: ΤΟΥ ΕΡΩΤΑ ΚΑΙ ΤΗΣ ΣΚΙΑΣ
   dewey: 863 ΑΛΙ
   entry_numbers:
   - '16546'
   translators:
   - ΣΩΤΗΡΙΑΔΟΥ-ΜΠΑΡΑΧΑΣ,ΚΛΑΙΤΗ
@@ -659463,15 +659333,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 13109
   authors:
-  - ΑΝΑΓΝΩΣΤΑΚΗΣ,ΜΑΝΟΛΗΣ
+  - ΑΝΑΓΝΩΣΤΑΚΗΣ,ΜΑΝΩΛΗΣ
   language: el
   title: ΔΗΜΙΟΥΡΓΩΝΤΑΣ ΜΙΑ ΠΟΙΗΣΗ ΠΑΝΩ ΑΠΟ ΚΑΘΕ ΚΑΤΑΣΤΡΟΦΗ
   dewey: 889.1 ΑΝΑ
   entry_numbers:
   - '16594'
   editor: Η ΚΑΘΗΜΕΡΙΝΗ // ΑΘΗΝΑ
   edition_year: 2014
@@ -660862,15 +660732,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13136
   authors:
-  - ΒΟΥΣΒΟΥΝΗ,ΑΝΤΩΝΗ
+  - ΒΟΥΣΒΟΥΝΗΣ,ΑΝΤΩΝΗΣ
   language: el
   title: ΠΡΟΜΗΝΥΜΑ
   dewey: 889.21 ΒΟΥ
   entry_numbers:
   - '16626'
   editor: ΕΡΜΕΙΑΣ // ΑΘΗΝΑ
   edition_year: 1976
@@ -662705,15 +662575,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13173
   authors:
-  - ΑΝΤΡΙΤΣ,ΙΒΟ
+  - ANDRIC,IVO
   language: el
   title: ΚΑΤΑΡΑΜΕΝΗ ΑΥΛΗ
   dewey: 891.82 ΑΝΤ
   entry_numbers:
   - '16685'
   translators:
   - ΚΩΤΟΥΛΑΣ,ΙΩΑΝΝΗΣ
@@ -663354,15 +663224,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13186
   authors:
-  - ΑΝΤΕΡΣΕΝ,ΧΑΝΣ,ΚΡΙΣΤΙΑΝ
+  - ANDERSEN,HANS,CHRISTIAN
   language: el
   title: ΤΟ ΚΟΡΙΤΣΑΚΙ ΜΕ ΤΑ ΣΠΙΡΤΑ
   dewey: 808.899 ΑΝΤ
   entry_numbers:
   - '16676'
   editor: ΑΠΟΚΑΛΥΨΕΙΣ // ΑΘΗΝΑ
   edition_year: 1996
@@ -663983,15 +663853,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13198
   authors:
-  - ΒΕΝΙΖΕΛΟΣ,ΚΩΣΤΑΣ-ΙΓΝΑΤΙΟΥ,ΜΙΧΑΛΗΣ
+  - ΒΕΝΙΖΕΛΟΣ,ΚΩΣΤΑΣ
+  - ΙΓΝΑΤΙΟΥ,ΜΙΧΑΛΗΣ
   language: el
   title: ΤΑ ΜΥΣΤΙΚΑ ΑΡΧΕΙΑ ΤΟΥ ΚΙΣΙΝΤΖΕΡ
   dewey: 327.569 ΒΕΝ
   entry_numbers:
   - '16649'
   editor: ΛΙΒΑΝΗ // ΑΘΗΝΑ
   edition_year: 2002
@@ -664186,15 +664057,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13202
   authors:
-  - ΑΠΟΣΤΟΛΟΠΟΥΛΟΥ,Θ.
+  - ΑΠΟΣΤΟΛΟΠΟΥΛΟΣ,ΘΕΟΔΩΡΟΣ
   language: el
   title: Ο ΕΛΛΗΝ ΠΟΛΙΤΗΣ
   dewey: 889.3 ΑΠΟ
   entry_numbers:
   - '16664'
   editor: ΛΑΜΠΡΑΚΗΣ // ΑΘΗΝΑ
   edition_year: 2014
@@ -667295,15 +667166,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13263
   authors:
-  - ΒΟΛΟΝΑΚΗΣ,ΕΛ.Κ.
+  - ΒΟΛΟΝΑΚΗΣ,ΕΛΕΥΘΕΡΙΟΣ,.Κ.
   language: el
   title: ΓΡΑΜΜΑΤΙΚΗ ΤΗΣ ΑΡΧΑΙΑΣ ΕΛΛΗΝΙΚΗΣ ΓΛΩΣΣΑΣ
   dewey: 485 ΒΟΛ
   entry_numbers:
   - '16740'
   editor: ΒΟΛΟΝΑΚΗ // ΑΘΗΝΑ
   pages: 420
@@ -667446,15 +667317,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13266
   authors:
-  - ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ
+  - ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ,M.
   language: el
   title: ΠΟΙΟΣ ΗΤΟΝ Ο ΦΟΝΕΥΣ ΤΟΥ ΑΔΕΛΦΟΥ ΜΟΥ ΚΑΙ ΑΛΛΑ ΔΙΗΓΗΜΑΤΑ
   dewey: 889.21 ΒΙΖ
   entry_numbers:
   - '16734'
   editor: ΤΑ ΝΕΑ // None
   pages: 250
@@ -668667,15 +668538,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13290
   authors:
-  - ΑΙΤΜΑΤΟΦ,ΤΣΙΝΓΚΙΖ
+  - AITMATOV,CHINGHIZ
   language: el
   title: ΤΟ ΜΑΤΙ ΤΗΣ ΚΑΜΗΛΑΣ
   dewey: 891.73 ΑΙΤ
   entry_numbers:
   - '16790'
   translators:
   - ΖΩΙΔΗΣ,ΓΙΩΡΓΗΣ
@@ -674719,15 +674590,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 13409
   authors:
-  - ΒΑΛΛΗΝΔΑ,ΠΕΤΡΟΥ
+  - ΒΑΛΛΗΝΔΑΣ,ΠΕΤΡΟΣ
   language: el
   title: ΕΙΣΑΓΩΓΗ ΕΙΣ ΤΗΝ ΕΠΙΣΤΗΜΗΝ ΤΟΥ ΔΙΚΑΙΟΥ
   dewey: 340.1 ΒΑΛ
   entry_numbers:
   - '16929'
   editor: ΣΑΚΚΟΥΛΑ // ΑΘΗΝΑ
   edition_year: 1960
@@ -676886,15 +676757,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13452
   authors:
-  - ΑΥΔΙΚΟΣ,ΒΑΓΓΕΛΗΣ
+  - ΑΥΔΙΚΟΣ,ΕΥΑΓΓΕΛΟΣ
   language: el
   title: Η ΣΚΙΑ ΤΗΣ ΜΙΚΑΣ
   dewey: 889.21 ΑΥΔ
   entry_numbers:
   - '16957'
   editor: ΤΑΞΙΔΕΥΤΗΣ // ΑΘΗΝΑ
   edition_year: 2013
@@ -678136,15 +678007,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13477
   authors:
-  - ΒΑΛΑΒΑΝΗ,ΕΛΕΝΗ-ΤΣΟΥΡΕΚΗ,ΙΩΑΝΝΑ
+  - ΒΑΛΑΒΑΝΗ,ΕΛΕΝΗ
+  - ΤΣΟΥΡΕΚΗ,ΙΩΑΝΝΑ
   language: el
   title: ΑΛΦΑΒΗΤΑΡΙΟ
   dewey: 966.5 ΒΑΛ
   entry_numbers:
   - '16996'
   editor: Ο.Ε.Δ.Β // ΑΘΗΝΑ
   edition_year: 1979
@@ -680593,15 +680465,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13525
   authors:
-  - ΑΝΤΕΡΣΕΝ,ΧΑΝΣ-ΚΡΙΣΤΙΑΝ
+  - ANDERSEN,HANS,CHRISTIAN
   language: el
   title: Η ΠΡΙΓΚΙΠΙΣΣΑ ΚΑΙ ΤΟ ΡΕΒΥΘΑΚΙ
   dewey: 808.899 ΑΝΤ
   entry_numbers:
   - '17049'
   editor: ΠΑΠΑΔΟΠΟΥΛΟΣ // ΑΘΗΝΑ
   edition_year: 1997
@@ -681882,15 +681754,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13551
   authors:
-  - ΒΟΥΛΤΣΙΑΔΗ,ΓΕΩΡΓΙΟΥ
+  - ΒΟΥΛΤΣΙΑΔΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: Η ΣΜΑΡΑΓΔΕΝΙΑ ΠΟΛΙΤΕΙΑ
   dewey: 889.21 ΒΟΥ
   entry_numbers:
   - '12421'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1997
@@ -681931,15 +681803,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13552
   authors:
-  - ΒΟΥΛΤΣΙΑΔΗ,ΓΕΩΡΓΙΟ
+  - ΒΟΥΛΤΣΙΑΔΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: Η ΜΕΓΑΛΗ ΑΡΕΝΑ
   dewey: 889.21 ΒΟΥ
   entry_numbers:
   - '12422'
   editor: ΤΟ ΠΑΛΙΜΨΗΣΤΟΝ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1998
@@ -681980,15 +681852,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13553
   authors:
-  - ΒΟΥΛΤΣΙΑΔΗ,ΓΙΩΡΓΟΥ
+  - ΒΟΥΛΤΣΙΑΔΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΤΑ ΤΕΣΣΕΡΑ ΔΙΑΜΑΝΤΙΑ
   dewey: 889.21 ΒΟΥ
   entry_numbers:
   - '12420'
   editor: ΤΟ ΠΑΛΙΜΨΗΣΤΟΝ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1999
@@ -688385,15 +688257,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13681
   authors:
-  - ΒΟΥΛΓΑΡΗ,ΣΤΕΡΓΙΟΥ
+  - ΒΟΥΛΓΑΡΗΣ,ΣΤΕΡΓΙΟΣ
   language: el
   title: ΓΟΡΓΟΠΟΤΑΜΟΣ
   dewey: 949.507 ΒΟΥ
   entry_numbers:
   - '17150'
   editor: None // ΑΘΗΝΑ
   edition_year: 1971
@@ -688486,15 +688358,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13683
   authors:
-  - ΒΛΑΧΟΥ,ΑΓΓΕΛΟΥ
+  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,Σ.
   language: el
   title: ΜΕΡΟΛΗΨΙΕΣ ΤΟΥ ΘΟΥΚΙΔΙΔΗ
   dewey: 884.07 ΒΛΑ
   entry_numbers:
   - '17137'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   pages: 249
@@ -688586,15 +688458,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13685
   authors:
-  - ΒΑΚΑΛΟΠΟΥΛΟΥ,ΑΠΟΣΤΟΛΟΥ
+  - ΒΑΚΑΛΟΠΟΥΛΟΣ,ΑΠΟΣΤΟΛΟΣ
   language: el
   title: ΤΟΥΡΚΟΚΡΑΤΙΑ 1453-1669 ΟΙ ΙΣΤΟΡΙΚΕΣ ΒΑΣΙΕΣ ΤΗΣ ΝΕΟΕΛΛΗΝΙΚΗΣ
   subtitle: ΚΟΙΝΩΝΙΑΣ ΚΑΙ ΟΙΚΟΝΟΜΙΑΣ
   dewey: 938 ΒΑΚ
   entry_numbers:
   - '17206'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -689137,15 +689009,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13696
   authors:
-  - ΒΟΥΓΙΟΥΚΑ,ΚΩΝ/ΝΟΥ
+  - ΒΟΥΓΙΟΥΚΑΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΟΙ ΚΟΙΝΩΝΙΚΩΣ ΑΠΡΟΣΑΡΜΟΣΤΟΙ ΑΝΗΛΙΚΟΙ ΕΙΣ ΤΗΝ ΑΡΧΑΙΑΝ ΕΛΛΑΔΑ
   dewey: 345.04 ΒΟΥ
   entry_numbers:
   - '17201'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1960
@@ -689831,15 +689703,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13710
   authors:
-  - ΑΧΙΛΛΕΩΣ,ΣΑΒΑ
+  - ΑΧΙΛΛΕΩΣ,ΣΑΒΒΑΣ
   language: el
   title: ΑΥΤΟΙ ΠΟΥ ΔΕΝ ΕΧΟΥΝ ΦΩΝΗ
   dewey: 230 ΑΧΙ
   entry_numbers:
   - '17219'
   pages: 38
   topics:
@@ -690208,15 +690080,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13718
   authors:
-  - ΑΙΝΙΑΝ-ΜΑΖΑΡΑΚΗΣ,ΙΩΑΝΝΗΣ
+  - ΑΙΝΙΑΝ-ΜΑΖΑΡΑΚΗΣ,ΙΩΑΝΝΗΣ,Κ.
   language: el
   title: ΤΟ ΕΠΟΣ ΤΟΥ 40 ΛΑΙΚΗ ΕΙΚΟΝΟΓΡΑΦΙΑ
   dewey: 938.68 ΑΙΝ
   entry_numbers:
   - '17227'
   editor: None // ΑΘΗΝΑ
   edition_year: 1987
@@ -690258,15 +690130,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13719
   authors:
-  - ΒΑΙΤΣΗΣ,ΚΩΝ/ΝΟΣ
+  - ΒΑΙΤΣΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΑΡΤΙΝΟΙ ΖΩΓΡΑΦΟΙ ΚΑΙ Η ΑΡΤΑ
   dewey: 759.949 ΒΑΙ
   entry_numbers:
   - '17228'
   editor: None // ΑΡΤΑ
   edition_year: 2005
@@ -690664,15 +690536,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13727
   authors:
-  - ΒΑΣΙΛΟΠΟΥΛΟΥ,ΧΑΡΑΛΑΜΠΟΥΣ
+  - ΒΑΣΙΛΟΠΟΥΛΟΣ,ΑΡΧΙΜΑΝΔΡΙΤΗΣ ΧΑΡΑΛΑΜΠΟΣ
   language: el
   title: Ο ΑΓΙΟΣ ΓΕΩΡΓΙΟΣ Ο ΕΞ ΙΩΑΝΝΙΝΩΝ
   dewey: 230 ΒΑΣ
   entry_numbers:
   - '17301'
   editor: ΟΡΘΟΔΟΞΟΣ ΤΥΠΟΣ // ΑΘΗΝΑ
   edition_year: 1995
@@ -693254,15 +693126,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13779
   authors:
-  - ΑΘΑΝΑΣΙΑΔΗ,ΤΑΣΟΥ
+  - ΑΘΑΝΑΣΙΑΔΗΣ,ΤΑΣΟΣ
   language: el
   title: ΑΝΑΓΝΩΡΙΣΕΙΣ
   dewey: 889.21 ΑΘΑ
   entry_numbers:
   - '17293'
   editor: ΕΣΤΙΑ // ΑΘΗΝΑ
   pages: 335
@@ -693354,15 +693226,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13781
   authors:
-  - ΑΛΕΒΙΖΟΠΟΥΛΟΥ,ΑΝΤΩΝΙΟΥ
+  - ΑΛΕΒΙΖΟΠΟΥΛΟΣ,ΑΝΤΩΝΙΟΣ
   language: el
   title: Η ΑΣΤΡΟΛΟΓΙΑ ΣΤΟ ΦΩΣ ΤΗΣ ΟΡΘΟΔΟΞΙΑΣ
   dewey: 133 ΑΛΕ
   entry_numbers:
   - '17296'
   editor: None // ΑΘΗΝΑ
   edition_year: 1995
@@ -694254,15 +694126,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13799
   authors:
-  - ΒΑΡΒΙΤΣΙΩΤΗ,ΤΑΚΗ
+  - ΒΑΡΒΙΤΣΙΩΤΗΣ,ΤΑΚΗΣ
   language: el
   title: Η ΑΤΡΑΠΟΣ
   dewey: 889.1 ΒΑΡ
   entry_numbers:
   - '17372'
   editor: ΦΙΛΟΛΟΓΙΚΗ // None
   edition_year: 1984
@@ -694862,15 +694734,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13811
   authors:
-  - ΑΝΤΩΝΙΟΥ,Δ.Ι
+  - ΑΝΤΩΝΙΟΥ,ΔΗΜΗΤΡΙΟΣ,Ι.
   language: el
   title: ΧΑΙ - ΚΑΙ ΚΑΙ ΤΑΝΚΑ
   dewey: 889.1 ΑΝΤ
   entry_numbers:
   - '17367'
   editor: ΕΡΜΗΣ // ΑΘΗΝΑ
   edition_year: 1972
@@ -696314,15 +696186,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13840
   authors:
-  - ALCOTT,LOUISA
+  - ALCOTT,LOUISA,MAY
   title: LITTLE WOMAN
   entry_numbers:
   - '17336'
   editor: LONGMAN // None
   edition_year: 1965
   pages: 129
   topics:
@@ -696363,15 +696235,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13841
   authors:
-  - WHITE,MANCHIP
+  - MANCHIP WHITE,JON,EWBANK
   title: ANTHROPOLOGY
   entry_numbers:
   - '17359'
   editor: TEACH YOURSELF BOOKS // LONDON
   edition_year: 1971
   pages: 190
   topics:
@@ -696512,15 +696384,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13844
   authors:
-  - ALLEN,FREDERICK LEWIS
+  - ALLEN,FREDERICK,LEWIS
   language: el
   title: Η ΜΕΓΑΛΗ ΑΛΛΑΓΗ
   dewey: 973.91 ALL
   entry_numbers:
   - '17388'
   editor: ΙΚΑΡΟΣ // None
   edition_year: 1956
@@ -698354,15 +698226,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13881
   authors:
-  - ΣΑΚΚΕΤΟΣ,ΑΓΓΕΛΟΣ
+  - ΣΑΚΚΕΤΟΣ,ΑΓΓΕΛΟΣ,ΠΑΝ.
   language: el
   title: Η ΑΓΝΩΣΤΗ ΖΩΗ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
   dewey: 938.07 ΣΑΚ
   entry_numbers:
   - '17422'
   editor: ΛΙΑΚΟΠΟΥΛΟΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2004
@@ -699196,15 +699068,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13898
   authors:
-  - ΑΓΓΕΛΟΥ,ΑΛΚΗ
+  - ΑΓΓΕΛΟΥ,ΑΛΚΗΣ
   language: el
   title: ΠΛΑΤΩΝΟΣ ΤΥΧΑΙ
   dewey: 938.482 ΑΓΓ
   entry_numbers:
   - '17401'
   editor: None // ΑΘΗΝΑ
   edition_year: 1963
@@ -700518,15 +700390,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13924
   authors:
-  - ΒΛΑΧΟΥ,ΓΕΩΡΓΙΟΥ
+  - ΒΛΑΧΟΣ,ΓΕΩΡΓΙΟΣ,Κ.
   language: el
   title: ΕΙΣΑΓΩΓΗ ΣΤΗΝ ΙΣΤΟΡΙΑ ΤΗΣ ΠΟΛΙΤΙΚΗΣ ΣΧΕΨΕΩΣ
   dewey: 320 ΒΛΑ
   entry_numbers:
   - '17433'
   editor: ΠΑΠΑΖΗΣΗ // ΑΘΗΝΑ
   edition_year: 1975
@@ -701163,15 +701035,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13937
   authors:
-  - ΑΝΔΡΙΩΤΗΣ,ΝΙΚΟΛΑΟΣ
+  - ΑΝΔΡΙΩΤΗΣ,ΝΙΚΟΛΑΟΣ,ΠΑΝΤΕΛΗΣ
   language: el
   title: ΙΣΤΟΡΙΑ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΓΛΩΣΣΑΣ
   dewey: 489.309 ΑΝΔ
   entry_numbers:
   - '17457'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1995
@@ -701566,15 +701438,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13945
   authors:
-  - ΒΑΚΑΛΟΠΟΥΛΟΥ,ΑΠΟΣΤΟΛΟΥ
+  - ΒΑΚΑΛΟΠΟΥΛΟΣ,ΑΠΟΣΤΟΛΟΣ
   language: el
   title: ΙΣΤΟΡΙΑ ΤΟΥ ΝΕΟΥ ΕΛΛΗΝΙΣΜΟΥ
   dewey: 938 ΒΑΚ
   entry_numbers:
   - '17465'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1968
@@ -702259,15 +702131,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13959
   authors:
-  - ΒΟΓΙΑΤΖΗ,ΒΑΣ.
+  - ΒΟΓΙΑΤΖΗΣ,ΒΑΣΙΛΕΙΟΣ
   language: el
   title: ΛΑΟΣ ΧΩΡΙΣ ΧΩΡΟ
   entry_numbers: []
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1946
   pages: 100
   topics:
@@ -703107,15 +702979,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13976
   authors:
-  - ΑΡΡΙΑΝΟΣ
+  - ARRIANO,LUCIO FLAVIO
   language: el
   title: ΑΛΕΞΑΝΔΡΟΥ ΑΝΑΒΑΣΙΣ
   dewey: 938.09 ΑΡΡ
   entry_numbers:
   - '17486'
   edition_year: 1971
   pages: 147
@@ -703910,15 +703782,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13992
   authors:
-  - ΒΑΣΙΛΟΠΟΥΛΟΥ,ΧΑΡΑΛΑΜΠΟΥΣ
+  - ΒΑΣΙΛΟΠΟΥΛΟΣ,ΑΡΧΙΜΑΝΔΡΙΤΗΣ ΧΑΡΑΛΑΜΠΟΣ
   language: el
   title: ΞΕΣΚΕΠΑΣΜΑ ΤΟΥ ΡΟΤΑΡΥ
   dewey: 230 ΒΑΣ
   entry_numbers:
   - '17491'
   editor: ΟΡΘΟΔΟΞΟΣ ΤΥΠΟΣ // ΑΘΗΝΑ
   edition_year: 1991
@@ -703960,15 +703832,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13993
   authors:
-  - WOODHOUSE,C.M
+  - WOODHOUSE,CRISTOPHER,MONTAGUE
   title: THE PHILHELLENES
   dewey: 938.545 WOO
   entry_numbers:
   - '17511'
   editor: DORIC LIBRARY // LONDON
   edition_year: 1977
   pages: 264
@@ -704059,15 +703931,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 13995
   authors:
-  - ΑΘΑΝΑΣΟΠΟΥΛΟΥ,ΧΡΗΣΤΟΥ
+  - ΑΘΑΝΑΣΟΠΟΥΛΟΣ,ΧΡΗΣΤΟΣ
   language: el
   title: ΕΠΙΔΡΑΣΙΣ ΤΟΥ ΜΕΓΕΘΟΥΣ ΕΠΙ ΤΗΣ ΑΠΟΔΟΤΙΚΟΤΗΤΟΣ ΕΙΣ ΤΗΝ ΕΛΛΗΝ
   dewey: 338.094 ΑΘΑ
   entry_numbers:
   - '17509'
   editor: None // ΑΘΗΝΑ
   edition_year: 1970
@@ -704559,15 +704431,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14005
   authors:
-  - ΒΟΓΙΑΤΖΗ,ΒΑΣΙΛΕΙΟΥ
+  - ΒΟΓΙΑΤΖΗΣ,ΒΑΣΙΛΕΙΟΣ
   language: el
   title: ΑΓΡΟΤΙΚΗ ΚΟΙΝΩΝΙΚΗ ΑΣΦΑΛΙΣΙΣ
   dewey: 368.4 ΒΟΓ
   entry_numbers:
   - '17518'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1956
@@ -705262,15 +705134,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14019
   authors:
-  - ΒΑΒΟΥΣΚΟΥ,ΚΩΝΣΤΑΝΤΙΝΟΥ
+  - ΒΑΒΟΥΣΚΟΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: Η ΜΕΓΑΛΗ ΙΔΕΑ ΩΣ ΙΔΕΑ ΚΑΙ ΠΡΑΓΜΑΤΙΚΟΤΗΣ
   dewey: 938 ΒΑΒ
   entry_numbers:
   - '17551'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1970
@@ -705908,15 +705780,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14032
   authors:
-  - ΒΟΥΓΙΟΥΚΑ,ΚΩΝ/ΝΟΥ
+  - ΒΟΥΓΙΟΥΚΑΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: Ο ΔΙΚΑΣΤΗΣ ΑΝΗΛΙΚΩΝ ΚΑΙ ΑΙ ΠΑΡ ΑΥΤΩ ΒΟΗΘΗΤΙΚΑΙ ΥΠΗΡΕΣΙΑΙ ΤΟΥ
   subtitle: ΙΑΤΡΟΥ ΤΟΥ ΕΠΙΜΕΛΗΤΟΥ ΚΑΙ ΤΟΥ ΠΑΙΔΑΓΩΓΟΥΤ
   dewey: 364.168 ΒΟΥ
   entry_numbers:
   - '17232'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -706218,14 +706090,15 @@
   authors:
   - ΓΕΩΡΓΙΑΔΟΥ,ΝΙΚΟΛΑΟΥ
   language: el
   title: ΟΣΑ ΕΓΡΑΨΑ ΣΤΟ ΜΟΝΑΣΤΗΡΙ 1903-1912
   dewey: 938.676 ΓΕΩ
   entry_numbers:
   - '17576'
+  - '3668'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1984
   pages: 245
   topics:
   - ΜΑΚΕΔΟΝΙΑ
   donors:
   - ΤΟΜΠΟΥΛΙΔΗΣ,ΔΗΜΗΤΡΙΟΣ
@@ -706233,15 +706106,15 @@
   has_dvd: false
   offprint: false
   original_entry:
     0: 14038
     1: ΓΕΩΡΓΙΑΔΟΥ,ΝΙΚΟΛΑΟΥ
     2: ΟΣΑ ΕΓΡΑΨΑ ΣΤΟ ΜΟΝΑΣΤΗΡΙ 1903-1912
     4: 938.676ΓΕΩ
-    5: '17576'
+    5: 17576-3668
     9: ΘΕΣ/ΝΙΚΗ
     10: '1984'
     11: 245Σ
     12: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
     13: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
     14: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
     17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
@@ -706712,15 +706585,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14048
   authors:
-  - ΑΚΡΟΚΕΡΑΥΝΙΟΥ
+  - ΑΚΡΟΚΕΡΑΥΝΙΟΣ
   language: el
   title: ΤΟ ΛΥΚΟΦΩΣ ΤΩΝ ΘΕΩΝ ΣΤΗΝ ΑΛΒΑΝΙΑ
   dewey: 956.100 ΑΚΡ
   entry_numbers:
   - '17565'
   editor: ΠΑΝΗΠΕΙΡΩΤΙΚΟΥ ΑΓΩΝΟ // None
   pages: 72
@@ -706960,15 +706833,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14053
   authors:
-  - ΒΑΒΑΡΕΤΟΥ,ΓΕΩΡΓΙΟΥ
+  - ΒΑΒΑΡΕΤΟΣ,ΓΕΩΡΓΙΟΣ,ΑΧΙΛ.
   language: el
   title: ΙΩΑΝΝΗΣ ΚΩΛΕΤΤΗΣ Ο ΗΠΕΙΡΩΤΗΣ ΠΡΩΘΥΠΟΥΡΓΟΣ
   dewey: 938 ΒΑΒ
   entry_numbers:
   - '17560'
   editor: None // ΑΘΗΝΑ
   edition_year: 1966
@@ -707060,15 +706933,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14055
   authors:
-  - ΒΑΒΑΡΕΤΟΥ,ΓΕΩΡΓΙΟΥ
+  - ΒΑΒΑΡΕΤΟΣ,ΓΕΩΡΓΙΟΣ,ΑΧΙΛ.
   language: el
   title: Ο ΓΕΩΡΓΙΟΣ ΣΤΑΥΡΟΥ ΚΑΙ Η ΕΘΝΙΚΗ ΤΡΑΠΕΖΑ
   dewey: 938 ΒΑΒ
   entry_numbers:
   - '17558'
   editor: None // ΑΘΗΝΑ
   edition_year: 1967
@@ -707159,15 +707032,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14057
   authors:
-  - ΒΑΒΑΡΕΟΥ,ΓΕΩΡΓΙΟΥ
+  - ΒΑΒΑΡΕΤΟΣ,ΓΕΩΡΓΙΟΣ,ΑΧΙΛ.
   language: el
   title: ΔΡΟΣΟΥΛΙΤΕΣ ΗΠΕΙΡΟΣ-ΚΡΗΤΗ
   dewey: 398 ΒΑΒ
   entry_numbers:
   - '17556'
   editor: None // ΑΘΗΝΑ
   edition_year: 1967
@@ -707620,15 +707493,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 14066
   authors:
-  - ΑΣΛΑΝΙΔΗ,ΣΑΒΒΑ
+  - ΑΣΛΑΝΙΔΗΣ,ΣΑΒΒΑΣ
   language: el
   title: Η ΩΡΑΙΑ ΚΕΡΑΣΟΥΝΤΑ
   subtitle: Η ΑΛΗΣΜΟΝΗΤΗ ΝΥΜΦΗ ΤΟΥ ΕΥΞΕΙΝΟΥ ΠΟΝΤΟΥ
   dewey: 938.498 ΑΣΛ
   entry_numbers:
   - '17590'
   editor: ΑΡΓΟΝΑΥΤΑΙ -ΚΟΜΝΗΝΟΙ // ΑΘΗΝΑ
@@ -708732,15 +708605,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14088
   authors:
-  - ΑΝΤΩΝΙΟΥ,ΚΩΝΣΤΑΝΤΙΝΟΥ
+  - ΑΝΤΩΝΙΟΥ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΤΑ ΔΩΔΩΝΟΧΩΡΙΑ
   dewey: 398 ΑΝΤ
   entry_numbers: []
   editor: ΑΡΧΑΙΑ ΔΩΔΩΝΗ // ΙΩΑΝΝΙΝΑ
   edition_year: 1973
   pages: 173
@@ -709016,15 +708889,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14094
   authors:
-  - ΒΑΛΜΑ,ΣΤΑΜΑΤΗ
+  - ΒΑΛΜΑΣ,ΣΤΑΜΑΤΗΣ
   language: el
   title: ΑΙΝΙΓΜΑΤΑ
   dewey: 578.78 ΒΑΛ
   entry_numbers:
   - '12514'
   pages: 109
   topics:
@@ -709063,15 +708936,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14095
   authors:
-  - ΒΑΛΜΑ,ΣΤΑΜΑΤΗ
+  - ΒΑΛΜΑΣ,ΣΤΑΜΑΤΗΣ
   language: el
   title: ΚΑΙ ΤΑ ΑΙΝΙΓΜΑΤΑ ΠΟΥ ΔΕΝ ΠΡΟΣΦΕΝΟΜΕ ΝΑ ΜΑΣ ΠΟΥΝΕ ΟΙ ΔΑΣΚΑΛΟΙ
   dewey: 578.78 ΒΑΛ
   entry_numbers:
   - '12515'
   pages: 232
   topics:
@@ -709361,15 +709234,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14101
   authors:
-  - ΑΛΕΞΑΝΤΕΡ,ΤΑΣΑ
+  - ALEXANDER,TASHA
   language: el
   title: ΠΙΣΩ ΑΠΟ ΤΗ ΒΙΤΡΙΝΑ
   dewey: 823 ΑΛΕ
   entry_numbers:
   - '17612'
   translators:
   - ΣΠΑΝΔΩΝΗΣ,ΓΙΑΝΝΗΣ
@@ -710969,15 +710842,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14133
   authors:
-  - ΑΡΒΑΝΙΤΗ,ΝΙΚΟΥ
+  - ΑΡΒΑΝΙΤΗΣ,ΝΙΚΟΣ
   language: el
   title: ΤΟ ΑΙΓΑΙΟ ΣΤΙΣ ΦΛΟΓΕΣ
   dewey: 808.899 ΑΡΒ
   entry_numbers:
   - '17661'
   editor: ΠΑΙΔΙΚΟΙ ΟΡΙΖΟΝΤΕΣ // ΑΘΗΝΑ
   edition_year: 1983
@@ -711727,15 +711600,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14148
   authors:
-  - ALEXANDER,J
+  - ALEXANDER,J.
   language: el
   title: ΝΑΤΑΗΔΕΣ ΕΞΥΠΝΑΚΗΔΕΣ ΣΗΘΕΝ ΦΙΛΟΙ ... ΚΑΙ ΕΣΥ
   subtitle: ΜΑΘΑΙΝΩ ΝΑ ΘΩΡΑΚΙΖΟΜΑΙ, ΓΙΝΟΜΑΙ ΔΥΝΑΤΟΣ !
   dewey: 808.899 ALE
   entry_numbers:
   - '17654'
   translators:
@@ -711989,15 +711862,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14153
   authors:
-  - ΑΣΕΝΑ,ΝΤΟΥΙΓΚΟΥ
+  - ASENA,DUYGU
   language: el
   title: ΕΙΣΑΙ ΕΛΕΥΘΕΡΗ
   dewey: 894.35 ΑΣΕ
   entry_numbers:
   - '17645'
   translators:
   - ΔΕΜΕΣΤΙΧΑ,ΜΑΡΙΑ
@@ -712251,15 +712124,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14158
   authors:
-  - ΑΡΙΣΤΟΤΕΛΟΥΣ
+  - ΑΡΙΣΤΟΤΕΛΗΣ
   language: el
   title: ΡΗΤΟΡΙΚΗ
   dewey: 101 ΑΡΙ
   entry_numbers: []
   editor: ΖΑΧΑΡΟΠΟΥΛΟΣ // ΑΘΗΝΑ
   edition_year: 1940
   pages: 445
@@ -712632,15 +712505,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14166
   authors:
-  - AΡΙΣΤΟΤΕΛΟΥΣ
+  - ΑΡΙΣΤΟΤΕΛΗΣ
   language: el
   title: ΜΙΚΡΑ ΦΥΣΙΚΑ
   dewey: 101 ΑΡΙ
   entry_numbers: []
   editor: ΖΑΧΑΡΟΠΟΥΛΟΣ // ΑΘΗΝΑ
   pages: 221
   topics:
@@ -712727,15 +712600,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14168
   authors:
-  - ΒΩΡΟΣ,Φ.Κ.
+  - ΒΩΡΟΣ,ΦΑΝΟΥΡΙΟΣ,Κ.
   language: el
   title: Η ΦΙΛΟΣΟΦΙΑ ΤΗΣ ΕΚΠΑΙΔΕΥΣΗΣ
   dewey: 305.82 ΒΩΡ
   entry_numbers:
   - '4748'
   editor: None // ΑΘΗΝΑ
   edition_year: 1997
@@ -712825,15 +712698,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14170
   authors:
-  - ΑΓΓΕΛΟΠΟΥΛΟΥ,ΑΓΓΕΛΟΥ
+  - ΑΓΓΕΛΟΠΟΥΛΟΣ,ΑΓΓΕΛΟΣ
   language: el
   title: Η ΑΛΗΘΕΙΑ ΔΙΑ ΤΑΣ ΕΚΤΡΩΣΕΙΣ
   dewey: 363.460 ΑΓΓ
   entry_numbers:
   - '862'
   editor: None // ΑΘΗΝΑ
   edition_year: 1980
@@ -717109,15 +716982,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14255
   authors:
-  - ΑΜΠΑΤΖΗ,ΕΥΡΙΔΙΚΗ
+  - ΑΜΠΑΤΖΗ,ΕΥΡΥΔΙΚΗ
   language: el
   title: Η ΑΤΤΙΚΗ ΓΗ ΥΠΟΔΕΧΕΤΑΙ ΤΟΥΣ ΠΡΟΣΦΥΓΕΣ ΤΟΥ 22
   dewey: 938.498 ΑΜΠ
   entry_numbers:
   - '17720'
   editor: ΙΔΡ.ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩ // ΑΘΗΝΑ
   edition_year: 2016
@@ -717521,15 +717394,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14263
   authors:
-  - ΑΜΠΑΤΖΗ,ΕΥΡΙΔΙΚΗ
+  - ΑΜΠΑΤΖΗ,ΕΥΡΥΔΙΚΗ
   language: el
   title: 60 ΧΡΟΝΙΑ ΑΠΟ ΤΗ ΛΗΞΗ ΤΟΥ Β ΠΑΓΚΟΣΜΙΟΥ ΠΟΛΕΜΟΥ ΕΛΛΗΝΕΣ ΚΑΙ
   subtitle: ΑΥΣΤΡΑΛΟΙ ΣΤΟΝ ΚΟΙΝΟ ΑΓΩΝΑ ΓΙΑ ΤΗΝ ΕΛΕΥΘΕΡΙΑ
   dewey: 949.53 ΑΜΠ
   entry_numbers:
   - '17711'
   editor: ΙΔΡ.ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩ // ΑΘΗΝΑ
@@ -717573,15 +717446,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14264
   authors:
-  - ΑΜΠΑΤΖΗ,ΕΥΡΙΔΙΚΗ
+  - ΑΜΠΑΤΖΗ,ΕΥΡΥΔΙΚΗ
   language: el
   title: ΔΗΜΟΤΙΚΑ ΤΡΑΓΟΥΔΙΑ
   subtitle: ΙΣΤΟΡΙΑ - ΠΑΡΑΔΟΣΗ- ΤΑΥΤΟΤΗΤΑ
   dewey: 782.421 ΑΜΠ
   entry_numbers:
   - '17709'
   editor: ΙΔΡ.ΒΟΥΛΗ ΤΩΝ ΕΛΛΗΝΩ // ΑΘΗΝΑ
@@ -718495,15 +718368,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14282
   authors:
-  - ΒΑΚΑΛΟΠΟΥΛΟΣ,ΚΩΝ/ΝΟΣ
+  - ΒΑΚΑΛΟΠΟΥΛΟΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΤΟ ΝΕΟΤΟΥΡΚΙΚΟ ΚΙΝΗΜΑ ΚΑΙ Ο ΕΛΛΗΝΙΣΜΟΣ (1908-1912)
   dewey: 938.498 ΒΑΚ
   entry_numbers:
   - '17768'
   editor: ΑΝΤ.ΣΤΑΜΟΥΛΗΣ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2002
@@ -723000,15 +722873,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14371
   authors:
-  - ΑΘΑΝΑΣΙΑΔΗ,ΓΑΒΡΙΗΛ
+  - ΑΘΑΝΑΣΙΑΔΗΣ,ΓΑΒΡΙΗΛ
   language: el
   title: Ο ΘΥΜΟΣ
   dewey: 230 ΑΘΑ
   entry_numbers:
   - '12891'
   editor: ΣΩΤΗΡ // ΑΘΗΝΑ
   edition_year: 2004
@@ -723334,15 +723207,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14378
   authors:
-  - ΒΙΤΑΛΗ,ΦΙΛΑΡΕΤΟΥ
+  - ΒΙΤΑΛΗΣ,ΦΙΛΑΡΕΤΟΣ
   language: el
   title: ΤΟ ΜΕΓΑΛΕΙΟΝ ΤΗΣ ΟΡΘΟΔΟΞΙΑΣ ΜΑΣ
   dewey: 230 ΒΙΤ
   entry_numbers:
   - '9331'
   editor: None // ΑΘΗΝΑ
   pages: 22
@@ -723523,15 +723396,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14382
   authors:
-  - ΑΛΕΞΙΟΥ,ΣΠΥΡΟΥ
+  - ΑΛΕΞΙΟΥ,ΣΠΥΡΟΣ
   language: el
   title: Η ΕΚΚΛΗΣΙΑ ΣΤΗΝ ΕΠΟΧΗ ΜΑΣ
   dewey: 230 ΑΛΕ
   entry_numbers:
   - '9341'
   editor: ΚΑΘΗΜΕΡΙΝΗ // ΑΘΗΝΑ
   edition_year: 1980
@@ -723808,15 +723681,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14388
   authors:
-  - ΒΑΣΙΛΕΙΑΔΗ,ΝΙΚΟΛΑΟΥ
+  - ΒΑΣΙΛΕΙΑΔΗΣ,ΝΙΚΟΛΑΟΣ
   language: el
   title: ΤΟ ΜΥΣΤΗΡΙΟΝ ΘΑΝΑΤΟΥ
   dewey: 230 ΒΑΣ
   entry_numbers:
   - '8940'
   editor: ΣΩΤΗΡ // ΑΘΗΝΑ
   edition_year: 1983
@@ -724660,15 +724533,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14406
   authors:
-  - ΑΔΑΜΟΠΟΥΛΟΥ,ΧΡΙΣΤΟΥ
+  - ΑΔΑΜΟΠΟΥΛΟΣ,ΧΡΙΣΤΟΣ
   language: el
   title: ΑΙ ΠΥΛΑΙ ΤΟΥ ΑΔΟΥ
   dewey: 230 ΑΔΑ
   entry_numbers:
   - '8419'
   editor: None // ΑΘΗΝΑ
   edition_year: 1977
@@ -725189,15 +725062,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14417
   authors:
-  - ΑΛΚΟΤ,ΛΟΥΙΖ
+  - ALCOTT,LOUISA,MAY
   language: el
   title: ΜΙΚΡΕΣ ΚΥΡΙΕΣ
   dewey: 808.899 ΑΛΚ
   entry_numbers:
   - '17842'
   editor: ΤΟΞΟΤΗΣ // ΑΘΗΝΑ
   pages: 128
@@ -732847,15 +732720,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14569
   authors:
-  - ΑΛΙΕΝΤΕ,ΙΖΑΜΠΕΛ
+  - ALLENDE,ISABEL
   language: el
   title: ΤΟ ΣΠΙΤΙ ΤΩΝ ΠΝΕΥΜΑΤΩΝ
   dewey: 863 ΑΛΙ
   entry_numbers:
   - '19168'
   translators:
   - ΣΩΤΗΡΙΑΔΟΥ-ΜΠΑΡΑΧΑΣ,ΚΛΑΙΤΗ
@@ -733766,15 +733639,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14587
   authors:
-  - ΑΣΙΜΩΦ
+  - ASIMOV,ISAAC
   language: el
   title: ΜΕΓΑΛΗ ΑΝΘΟΛΟΓΙΑ
   entry_numbers:
   - '19186'
   editor: ΕΞΑΝΤΑΣ // ΑΘΗΝΑ
   edition_year: 1976
   pages: 444
@@ -739724,15 +739597,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14707
   authors:
-  - ALLEN,WOODY
+  - WOODY,ALLEN
   language: el
   title: ΟΛΑ ΤΑ ΓΡΑΠΤΑ ΤΟΥ
   dewey: 810.11 ALL
   entry_numbers:
   - '19487'
   translators:
   - ΚΑΚΙΣΗΣ,ΣΩΤΗΡΗΣ
@@ -740772,15 +740645,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14728
   authors:
-  - ΑΠΕΛΓΙΑΡΝΤ,ΝΤΑΙΑΝΑ
+  - APPLEYARD,DIANA
   language: el
   title: Η ΚΑΛΗ ΝΟΙΚΟΚΥΡΑ
   dewey: 823 ΑΠΕ
   entry_numbers:
   - '19513'
   translators:
   - ΟΙΚΟΝΟΜΟΥ,ΚΑΙΤΗ
@@ -741382,15 +741255,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14740
   authors:
-  - ΒΑΝΣ,ΝΤΕΙΒΙΝΤ,ΤΖΕΙΜΣ
+  - VANCE,JAMES,DAVID
   language: el
   title: ΤΟ ΤΡΑΓΟΥΔΙ ΤΟΥ ΧΙΛΜΠΙΛΗ
   dewey: 810.11 ΒΑΝ
   entry_numbers:
   - '19552'
   translators:
   - ΜΑΛΛΙΑΡΟΣ,ΑΡΙΣΤΕΙΔΗΣ
@@ -743146,15 +743019,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14776
   authors:
-  - ΑΝΤΕΡΣΕΝ,ΚΡΙΣΤΙΑΝ,ΧΑΝΣ
+  - ANDERSEN,HANS,CHRISTIAN
   language: el
   title: ΤΟ ΚΟΡΙΤΣΑΚΙ ΜΕ ΤΑ ΣΠΙΡΤΑ
   dewey: 808.899 ΑΝΤ
   entry_numbers:
   - '19585'
   editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
   edition_year: 2012
@@ -744394,15 +744267,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14802
   authors:
-  - ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ
+  - ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ,M.
   language: el
   title: ΣΤΘΙΔΕΣ ΑΥΡΑΙ
   dewey: 889.11 ΒΙΖ
   entry_numbers: []
   editor: ΤΟ ΒΗΜΑ // ΑΘΗΝΑ
   edition_year: 2014
   pages: 330
@@ -749178,15 +749051,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14898
   authors:
-  - ΑΜΠΕΝΤΙ,ΙΖΑΜΠΕΛ
+  - ABEDI,ISABEL
   language: el
   title: ΕΡΧΕΤΑΙ Η ΛΟΛΑ!
   dewey: 808.899 ΑΜΠ
   entry_numbers:
   - '19816'
   translators:
   - ΠΑΣΠΑΡΔΑΝΗΣ,ΑΛΕΞΑΝΔΡΟΣ
@@ -749623,15 +749496,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14907
   authors:
-  - ΒΙΚΕΡΣ,ΣΑΛΙ
+  - VICKERS,SALLEY
   language: el
   title: Ο ΑΓΓΕΛΟΣ ΤΗΣ ΔΕΣΠΟΙΝΙΔΑΣ ΓΚΑΡΝΕΡ
   dewey: 823 ΒΙΚ
   entry_numbers:
   - '19848'
   translators:
   - ΛΑΜΠΡΙΝΙΔΟΥ,ΒΑΝΙΑ
@@ -749723,15 +749596,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14909
   authors:
-  - ΑΣΙΜΑΝ, ΑΝΤΡΕ
+  - ACIMAN,ANDRE
   language: el
   title: ΕΞΟΔΟΣ ΑΠΟ ΤΗΝ ΑΙΓΥΠΤΟ
   entry_numbers:
   - '19869'
   translators:
   - ΣΧΙΝΑ,ΚΑΤΕΡΙΝΑ
   editor: ΜΕΤΑΙΧΜΙΟ // ΑΘΗΝΑ
@@ -750122,15 +749995,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14917
   authors:
-  - ΑΣΜΠΕ,ΖΑΝ
+  - ASHBE,JEANNE
   language: el
   title: Α ΤΙ ΚΑΛΑ!
   dewey: 808.899 ΑΣΜ
   entry_numbers:
   - '19913'
   editor: ΣΥΓΧΡΟΝΟΙ ΟΡΙΖΟΝΤΕΣ // ΑΘΗΝΑ
   pages: 10
@@ -751719,15 +751592,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 14949
   authors:
-  - ΑΝΣΓΟΥΩΡΘ,ΜΠΑΡΥ
+  - UNSWORTH,BARRY
   language: el
   title: ΙΕΡΗ ΠΕΙΝΑ
   dewey: 823 ΑΝΣ
   entry_numbers:
   - '19849'
   translators:
   - ΣΚΑΡΠΕΛΟΣ,ΓΙΑΝΝΗΣ
@@ -755552,15 +755425,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15025
   authors:
-  - ΒΡΑΤΣΙΣΤΑ-ΚΑΤΣΑΔΩΡΑΚΗ, ΔΟΜΝΑ
+  - ΒΡΑΤΣΙΣΤΑ-ΚΑΤΣΑΔΩΡΑΚΗ,ΔΟΜΝΑ
   language: el
   title: ΜΟΝΟΠΤΕΡΟΣ ΑΓΓΕΛΟΣ
   dewey: 889.11 ΒΡΑ
   entry_numbers:
   - '20017'
   editor: None // ΑΡΤΑ
   edition_year: 2003
@@ -756823,15 +756696,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15050
   authors:
-  - ΒΕΝΣΑΝ,ΖΙΛ
+  - VINCENT,GILLES
   language: el
   title: ΤΟ ΦΙΛΙ ΤΟΥ ΘΑΝΑΤΟΥ
   dewey: 843 ΒΕΝ
   entry_numbers:
   - '20047'
   translators:
   - ΚΟΛΑΙΤΗ,ΡΙΤΑ
@@ -758630,15 +758503,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15086
   authors:
-  - ΒΕΡΝ.ΙΟΥΛΙΟΥ
+  - VERNE,JULES
   language: el
   title: ΤΟ ΜΥΣΤΗΡΙΩΔΕΣ ΕΓΚΛΗΜΑ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '1995'
   editor: ΑΣΤΗΡ // ΑΘΗΝΑ
   edition_year: 1974
@@ -758678,15 +758551,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15087
   authors:
-  - WALKER,RITCHARD
+  - WALKER,RICHARD
   language: el
   title: Η ΔΥΝΑΜΗ ΤΩΝ ΑΙΣΘΗΣΕΩΝ
   dewey: 808.899 WAL
   entry_numbers:
   - '19997'
   editor: ΣΑΒΒΑΛΑΣ // ΑΘΗΝΑ
   edition_year: 2002
@@ -759077,15 +758950,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 15095
   authors:
-  - ΒΕΡΝ.ΙΟΥΛΙΟΥ
+  - VERNE,JULES
   language: el
   title: ΤΑ ΤΕΡΑΤΑ ΤΩΝ ΘΑΛΑΣΣΩΝ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '20091'
   translators:
   - ΠΥΡΓΙΩΤΗΣ,ΑΓΓΕΛΟΣ
@@ -759126,15 +758999,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15096
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  - VERNE,JULES
   language: el
   title: 20.000 ΛΕΥΓΕΣ ΥΠΟ ΤΗΝ ΘΑΛΑΣΣΑ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '20090'
   translators:
   - ΣΤΑΘΑΤΟΥ,ΕΛΕΝΗ
@@ -760024,15 +759897,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15114
   authors:
-  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ
+  - ΒΛΑΧΟΣ,ΑΓΓΕΛΟΣ,ΣΤ,
   language: el
   title: Ο ΚΥΡΙΟΣ ΑΛΚΙΒΙΑΔΗΣ
   dewey: 889.21 ΒΛΑ
   entry_numbers:
   - '20112'
   editor: ΤΟ ΒΗΜΑ // ΑΘΗΝΑ
   edition_year: 2008
@@ -760171,15 +760044,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15117
   authors:
-  - ΑΠΟΣΤΟΛΙΔΗΣ,ΡΕΝΟΣ
+  - ΑΠΟΣΤΟΛΙΔΗΣ,ΡΕΝΟΣ,ΗΡΑΚΛΗΣ
   language: el
   title: ΠΥΡΑΜΙΔΑ 67
   subtitle: ΤΟ ΒΙΒΛΙΟ ΤΟΥ ΕΜΦΥΛΙΟΥ
   dewey: 889.21 ΑΠΟ
   entry_numbers:
   - '20099'
   editor: ΤΟ ΒΗΜΑ // ΑΘΗΝΑ
@@ -761025,15 +760898,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15134
   authors:
-  - ΑΝΤΕΡΣΕΝ, ΧΑΝΣ ΚΡΙΣΤΙΑΝ
+  - ANDERSEN,HANS,CHRISTIAN
   language: el
   title: Η ΒΑΣΙΛΙΣΣΑ ΤΟΥ ΧΙΟΝΙΟΥ
   dewey: 808.899 ΑΝΤ
   entry_numbers:
   - '19987'
   translators:
   - ΚΟΝΤΟΛΕΩΝ,ΜΑΝΟΣ
@@ -763661,15 +763534,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15187
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  - VERNE,JULES
   language: el
   title: ΤΑΞΙΔΙ ΣΤΟ ΚΕΝΤΡΟ ΤΗΣ ΓΗΣ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '20170'
   - '20643'
   translators:
@@ -763818,15 +763691,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15190
   authors:
-  - ΑΡΓΥΡΗ, ΑΝΔΡΕΑ
+  - ΑΡΓΥΡΗΣ,ΑΝΔΡΕΑΣ
   language: el
   title: Η ΖΩΗ ΣΤΟ ΠΕΡΑΣΜΑ ΤΟΥ ΧΡΟΝΟΥ
   dewey: 808.899 ΑΡΓ
   entry_numbers:
   - '20167'
   editor: None // ΑΘΗΝΑ
   edition_year: 1984
@@ -764072,15 +763945,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15195
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  - VERNE,JULES
   language: el
   title: ΓΥΡΩ ΑΠΟ ΤΗ ΣΕΛΗΝΗ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '20162'
   translators:
   - ΚΑΡΟΥΖΟΥ,ΚΑΙΤΗ
@@ -764946,15 +764819,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15212
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  - VERNE,JULES
   language: el
   title: Ο ΔΕΚΑΠΕΝΤΑΕΤΗΣ ΠΛΟΙΑΡΧΟΣ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '20190'
   translators:
   - ΚΩΣΤΑΚΗΣ,ΑΛΕΚΟΣ
@@ -765646,15 +765519,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15226
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  - VERNE,JULES
   language: el
   title: Ο ΝΑΥΑΓΟΣ ΤΗΣ ΚΥΝΘΙΑΣ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '20177'
   translators:
   - ΣΦΑΕΛΛΟΥ-ΒΕΝΙΖΕΛΟΥ,ΚΑΛΛΙΩΠΗ Α.
@@ -765698,15 +765571,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15227
   authors:
-  - ΒΕΡΝ.ΙΟΥΛΙΟΥ
+  - VERNE,JULES
   language: el
   title: ΔΥΟ ΧΡΟΝΙΑ ΔΙΑΚΟΠΕΣ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '20174'
   translators:
   - ΑΝΤΩΝΟΠΟΥΛΟΥ,ΠΑΝ.
@@ -769180,15 +769053,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15296
   authors:
-  - ΑΘΑΝΑΣΙΑΔΗ,ΝΙΚΟΥ
+  - ΑΘΑΝΑΣΙΑΔΗΣ,ΝΙΚΟΣ
   language: el
   title: ΘΥΕΛΛΑ ΚΑΙ ΓΑΛΗΝΗ
   dewey: 889.21 ΑΘΑ
   entry_numbers:
   - '20236'
   editor: ΔΩΡΙΚΟΣ // ΑΘΗΝΑ
   edition_year: 1975
@@ -769230,15 +769103,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15297
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: ΚΥΡΙΑ ΜΠΡΑΝΙΚΑΝ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '20238'
   editor: ΤΕΣΣΕΡΑ ΠΙ // ΑΘΗΝΑ
   edition_year: 2011
@@ -770021,15 +769894,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15313
   authors:
-  - ΑΡΝΤΙΤΙ,ΜΕΤΙΝ
+  - ARDITI,METIN
   language: el
   title: ΤΟ ΤΟΥΡΚΑΚΙ
   dewey: 843 ΑΡΝ
   entry_numbers:
   - '20053'
   translators:
   - ΚΟΛΑΙΤΗ,ΡΙΤΑ
@@ -771023,15 +770896,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15333
   authors:
-  - ΑΤΓΟΥΝΤ,ΜΑΡΓΚΑΡΕΤ
+  - ATWOOD,MARGARET
   language: el
   title: Η ΙΣΤΟΡΙΑ ΤΗΣ ΘΕΡΑΠΑΙΝΙΔΑΣ
   dewey: 810.11 ΑΤΓ
   entry_numbers:
   - '20276'
   translators:
   - ΚΟΡΤΩ,ΑΥΓΟΥΣΤΟΣ
@@ -771638,15 +771511,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15345
   authors:
-  - ΑΛΙΕΝΤΕ, ΙΖΑΜΠΕΛ
+  - ALLENDE,ISABEL
   language: el
   title: ΤΟ ΝΗΣΙ ΚΑΤΩ ΑΠ ΤΗ ΘΑΛΑΣΣΑ
   dewey: 863 ΑΛΙ
   entry_numbers:
   - '20291'
   translators:
   - ΚΑΡΑΤΖΑΣ,ΛΕΩΝΙΔΑΣ
@@ -771993,15 +771866,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15352
   authors:
-  - ΑΣΤΟΥΡΙΑΣ-ΑΝΧΕΛ,ΜΙΓΚΕΛ
+  - ASTURIAS ROSALES,MIGUEL ANGEL
   language: el
   title: ΜΙΑ ΚΑΠΟΙΑ ΜΙΓΑΔΑ
   dewey: 860.11 ΑΣΤ
   entry_numbers:
   - '20297'
   translators:
   - ΛΥΚΟΥΔΗΣ,ΜΠΑΜΠΗΣ
@@ -772199,15 +772072,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15356
   authors:
-  - ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ
+  - ΒΙΖΥΗΝΟΣ,ΓΕΩΡΓΙΟΣ,M.
   language: el
   title: ΑΤΘΙΔΕΣ ΑΥΡΑΙ
   subtitle: ΟΙ ΠΟΙΗΤΕΣ ΤΗΣ ΡΩΜΙΟΣΥΝΗΣ
   dewey: 889.11 ΒΙΖ
   entry_numbers:
   - '20303'
   editor: ΤΟ ΒΗΜΑ // ΑΘΗΝΑ
@@ -772815,15 +772688,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15368
   authors:
-  - ΑΠΟΣΤΟΛΟΠΟΥΛΟΥ,Θ.
+  - ΑΠΟΣΤΟΛΟΠΟΥΛΟΣ,ΘΕΟΔΩΡΟΣ
   language: el
   title: Ο ΕΛΛΗΝ ΠΟΛΙΤΗΣ
   dewey: 889.07 ΑΠΟ
   entry_numbers:
   - '20320'
   editor: None // ΑΘΗΝΑ
   pages: 160
@@ -773373,15 +773246,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15379
   authors:
-  - ΑΝΑΓΝΩΣΤΟΠΟΥΛΟΥ,ΘΥΜΙΟΥ-ΒΟΣΤΑΝΤΖΗ,ΚΩΝ/ΝΟΥ
+  - ΑΝΑΓΝΩΣΤΟΠΟΥΛΟΣ,ΘΥΜΙΟΣ
+  - ΒΟΣΤΑΝΤΖΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΠΡΑΚΤΙΚΗ ΑΡΙΘΜΗΤΙΚΗ
   dewey: 889.07 ΑΝΑ
   entry_numbers:
   - '20325'
   editor: ΝΙΚΗ // ΑΘΗΝΑ
   edition_year: 1961
@@ -773424,15 +773298,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15380
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: Η ΣΧΟΛΗ ΤΩΝ ΡΟΒΙΣΝΩΝΩΝ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '20236'
   editor: ΑΓΚΥΡΑ // ΑΘΗΝΑ
   edition_year: 1983
@@ -773627,15 +773501,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15384
   authors:
-  - ΑΛΕΞΑΝΔΡΟΥ,ΓΙΑΝΝΗΣ & ΜΑΡΙΑ
+  - ΑΛΕΞΑΝΔΡΟΥ,ΓΙΑΝΝΗΣ
+  - ΑΛΕΞΑΝΔΡΟΥ,ΜΑΡΙΑ
   language: el
   title: ΑΠΛΑ Σ ΑΓΑΠΩ
   dewey: 889.21 ΑΛΕ
   entry_numbers:
   - '20362'
   editor: ΛΙΒΑΝΗ // ΑΘΗΝΑ
   edition_year: 1999
@@ -774356,15 +774231,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15398
   authors:
-  - ΑΛΚΟΤ,ΛΟΥΙΖΑ,ΜΕΥ
+  - ALCOTT,LOUISA,MAY
   language: el
   title: ΜΙΚΡΕΣ ΚΥΡΙΕΣ
   dewey: 810.11 ΑΛΚ
   entry_numbers:
   - '20345'
   translators:
   - ΧΑΤΧΟΥΤ,ΡΕΝΑ
@@ -776493,15 +776368,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15440
   authors:
-  - ΒΑΛΕΣ ΖΥΛ
+  - VALLES,JULES
   language: el
   title: ΤΟ ΠΑΙΔΙ
   dewey: 843 ΒΑΛ
   entry_numbers:
   - '20477'
   translators:
   - ΑΝΑΣΤΟΠΟΥΛΟΥ,ΓΙΟΥΛΗ
@@ -778796,15 +778671,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15487
   authors:
-  - ΑΙΤΜΑΤΟΦ,ΤΑΝΓΚΙΖ
+  - AITMATOV,CHINGHIZ
   language: el
   title: ΤΟ ΙΚΡΙΩΜΑ
   dewey: 891.73 ΑΙΤ
   entry_numbers:
   - '20493'
   translators:
   - ΠΑΠΑΝΔΡΕΟΥ,ΝΙΚΟΣ
@@ -779472,15 +779347,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15501
   authors:
-  - ΒΙΑΝ,ΜΠΟΡΙΣ
+  - VIAN,BORIS
   language: el
   title: ΘΑ ΦΤΥΣΩ ΣΤΟΥΣ ΤΑΦΟΥΣ ΣΑΣ
   dewey: 843 ΒΙΑ
   entry_numbers:
   - '19419'
   translators:
   - ΛΟΙΖΟΥ,ΣΥΛΒΙΑ
@@ -780400,15 +780275,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15520
   authors:
-  - ΒΑΡΝΑΚΙΩΤΗ,ΑΝΔΡΕΑΣ
+  - ΒΑΡΝΑΚΙΩΤΗΣ,ΑΝΔΡΕΑΣ
   language: el
   title: ΚΕΙΝΑ ΤΑ ΧΡΟΝΙΑ...
   subtitle: ΧΑΙΡΕΤΙΣΜΟΣ ΣΤΑ ΜΕΓΑΛΑ ΠΑΙΔΙΑ
   dewey: 889.1 ΒΑΡ
   entry_numbers:
   - '20512'
   editor: ΝΕΑ ΣΚΕΨΗ // ΑΘΗΝΑ
@@ -780895,15 +780770,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15530
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟ
+  - VERNE,JULES
   language: el
   title: ΤΟ ΑΙΓΑΙΟ ΑΝΑΣΤΑΤΟ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '20425'
   translators:
   - ΑΡΚΑΔΗ-ΚΩΣΤΑΚΗ,ΣΤΕΛΛΑ
@@ -780944,15 +780819,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15531
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  - VERNE,JULES
   language: el
   title: ΠΕΝΤΕ ΕΒΔΟΜΑΔΕΣ ΑΕΡΟΣΤΑΤΟ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '20416'
   translators:
   - ΜΙΧΑΗΛΙΔΗΣ,Τ.
@@ -783563,14 +783438,15 @@
     29: null
     30: null
 - dbase_number: 15584
   authors:
   - ΠΑΠΑΦΛΩΡΑΤΟΣ,ΙΩΑΝΝΗΣ
   language: el
   title: Ο ΕΛΛΗΝΙΣΜΟΣ ΤΟΥ ΠΟΝΤΟΥ
+  dewey: 938 ΠΑΠ
   entry_numbers:
   - '20707'
   editor: ΛΕΙΜΩΝ // ΑΘΗΝΑ
   edition_year: 2021
   pages: 701
   topics:
   - ΠΟΝΤΟΣ
@@ -783580,15 +783456,15 @@
   has_dvd: false
   offprint: false
   ean: '9786185259884'
   original_entry:
     0: 15584
     1: ΠΑΠΑΦΛΩΡΑΤΟΣ,ΙΩΑΝΝΗΣ
     2: Ο ΕΛΛΗΝΙΣΜΟΣ ΤΟΥ ΠΟΝΤΟΥ
-    4: 9388ΠΑΠ
+    4: 938ΠΑΠ
     5: '20707'
     8: ΛΕΙΜΩΝ
     9: ΑΘΗΝΑ
     10: '2021'
     11: 701Σ
     12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
     13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
@@ -784226,15 +784102,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15597
   authors:
-  - ΑΝΔΡΙΩΤΗΣ,ΝΙΚΟΣ
+  - ΑΝΔΡΙΩΤΗΣ,ΝΙΚΟΛΑΟΣ,ΠΑΝΤΕΛΗΣ
   language: el
   title: ΠΡΟΣΦΥΓΕΣ ΣΤΗΝ ΕΛΛΑΔΑ 1821-1940
   dewey: 938.993 ΑΝΔ
   entry_numbers:
   - '20727'
   editor: ΙΔΡ.ΒΟΥΛΗΣ ΤΩΝ ΕΛΛΛΗ // ΑΘΗΝΑ
   edition_year: 2020
@@ -784638,15 +784514,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15605
   authors:
-  - ΒΕΤΣΙΟΣ,ΕΛΕΥΘΕΡΙΟΣ
+  - ΒΕΤΣΙΟΣ,ΕΛΕΥΘΕΡΙΟΣ,Λ.
   language: el
   title: ΕΠΙΣΤΟΛΕΣ ΚΑΙ ΑΝΑΦΟΡΕΣ ΒΕΝΕΤΩΝ ΑΞΙΩΜΑΤΟΥΧΩΝ ΤΗΣ ΒΟΡΕΙΟΔΥΤΙΚΗ
   subtitle: Σ ΕΛΛΑΔΑΣ ΚΑΤΑ ΤΟΝ 18Ο ΑΙΩΝΑ
   entry_numbers:
   - '20733'
   editor: ΣΤΑΜΟΥΛΗ // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 2021
@@ -784844,15 +784720,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15609
   authors:
-  - ΒΛΑΧΟΠΑΝΟΣ, ΔΗΜΗΤΡΗΣ
+  - ΒΛΑΧΟΠΑΝΟΣ,ΔΗΜΗΤΡΗΣ
   language: el
   title: ΝΟΜΙΚΗ ΚΑΙ ΔΕΝΤΡΑ ΕΝ ΔΡΑΣΕΙ
   dewey: 889.21 ΒΛΑ
   entry_numbers:
   - '20737'
   editor: 24 ΓΡΑΜΜΑΤΑ // ΑΘΗΝΑ
   edition_year: 2021
@@ -785925,15 +785801,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15631
   authors:
-  - ΑΛΛΕΝ,ΓΟΥΝΤΥ
+  - WOODY,ALLEN
   language: el
   title: ΧΩΡΙΣ ΦΤΕΡΑ
   dewey: 810.11 ΑΛΛ
   entry_numbers:
   - '20596'
   translators:
   - ΚΑΚΙΤΣΗΣ,ΣΩΤΗΡΗΣ
@@ -786437,15 +786313,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15641
   authors:
-  - ΒΙΣΚΟΝΤΙ,ΛΟΥΚΙΝΟ
+  - VISCONTI,LUCHINO
   language: el
   title: ΑΝΤΖΕΛΟ
   entry_numbers: []
   translators:
   - ΧΡΥΣΟΣΤΟΜΙΔΗΣ,ΑΝΤΑΙΟΣ
   editor: ΝΕΑ ΣΥΝΟΡΑ // ΑΘΗΝΑ
   edition_year: 1993
@@ -787760,15 +787636,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15668
   authors:
-  - ΒΑΛΕΡΥ,ΠΩΛ
+  - VALERY,PAUL
   language: el
   title: ΤΟ ΘΑΛΑΣΣΙΝΟ ΚΟΙΜΗΤΗΡΙΟ
   dewey: 889.11 ΒΑΛ
   entry_numbers:
   - '20516'
   translators:
   - ΒΛΑΧΟΣ,ΙΩΑΝΝΗΣ-ΑΝΔΡΕΑΣ
@@ -788557,15 +788433,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15684
   authors:
-  - ΑΞΙΟΝΟΦ,ΒΑΣΙΛΗ
+  - ΑΞΙΟΝΟΦ,ΒΑΣΙΛΗΣ
   language: el
   title: ΟΙ ΣΥΝΑΔΕΛΦΟΙ
   dewey: 891.73 ΑΞΙ
   entry_numbers:
   - '20600'
   translators:
   - ΚΟΤΖΙΑΣ,ΚΩΣΤΑΣ
@@ -788657,15 +788533,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15686
   authors:
-  - ΑΙΧΕΝΔΟΡΦ,ΙΩΣΗΦ ΒΑΡΩΝΟΥ
+  - VON EICHENDORFF,JOSEPH,FREIHERR
   language: el
   title: ΑΠΟ ΤΗ ΖΩΗ ΕΝΟΣ ΑΚΑΜΑΤΗ
   dewey: 850.11 ΑΙΧ
   entry_numbers:
   - '8500'
   editor: ΒΑΣΙΛΕΙΟΥ // ΑΘΗΝΑ
   pages: 164
@@ -789039,15 +788915,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15694
   authors:
-  - ΑΣΙΜΩΦ,ΙΣΑΑΚ
+  - ASIMOV,ISAAC
   language: el
   title: ΕΓΩ ... ΤΟ ΡΟΜΠΟΤ
   dewey: 891.73 ΑΣΙ
   entry_numbers:
   - '20499'
   translators:
   - ΠΑΝΤΑΛΕΟΝΤΑΣ,ΝΙΚΟΣ
@@ -789738,15 +789614,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15709
   authors:
-  - ΑΝΔΡΕΑΔΗ,ΓΕΩΡΓΙΟΥ Α.
+  - ΑΝΔΡΕΑΔΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΠΟΝΤΙΑΚΑ ΔΕΙΝΟΠΑΘΗΜΑΤΑ
   dewey: 938.726 ΑΝΔ
   entry_numbers:
   - '20907'
   editor: ΚΟΡΑΛΛΙ // ΑΘΗΝΑ
   edition_year: 2021
@@ -790503,15 +790379,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15725
   authors:
-  - ALVIN LESKY
+  - LESKY,ALBIN
   title: H ΤΡΑΓΙΚΗ ΠΟΙΗΣΗ ΤΩΝ ΑΡΧΑΙΩΝ ΕΛΛΗΝΩΝ ΤΟΜΟΣ Α
   dewey: '882'
   entry_numbers:
   - '20925'
   translators:
   - ΧΟΥΡΜΟΥΖΙΑΔΗΣ,Ν.
   editor: None // ΑΘΗΝΑ
@@ -790552,15 +790428,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15726
   authors:
-  - ALVIN LESKY
+  - LESKY,ALBIN
   language: el
   title: Η ΤΡΑΓΙΚΗ ΠΟΙΗΣΗ ΤΩΝ ΑΡΧΑΙΩΝ ΕΛΛΗΝΩΝ ΤΟΜΟΣ Β
   dewey: 882 ALV
   entry_numbers:
   - '20926'
   translators:
   - ΧΟΥΡΜΟΥΖΙΑΔΗΣ,Ν.
@@ -791261,15 +791137,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15741
   authors:
-  - ΒΟΥΛΤΣΙΑΔΗ,ΓΕΩΡΓΙΟΥ
+  - ΒΟΥΛΤΣΙΑΔΗΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: Η ΠΡΟΣΩΤΣΑΝΗ ΜΕΣΑ ΑΠΟ ΤΗΝ ΙΣΤΟΡΙΑ
   dewey: 938.764 ΒΟΥ
   entry_numbers:
   - '12423'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1995
@@ -792993,15 +792869,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15778
   authors:
-  - ΒΑΣΔΡΑΒΕΛΛΗ,ΙΩΑΝ.
+  - ΒΑΣΔΡΑΒΕΛΛΗΣ,ΙΩΑΝΝΗΣ,Κ.
   language: el
   title: Η ΘΕΣΣΑΛΟΝΙΚΗ
   subtitle: ΚΑΤΑ ΤΟΝ ΑΓΩΝΑ ΤΗΣ ΑΝΕΞΑΡΤΗΣΙΑΣ
   dewey: 938.498 ΒΑΣ
   entry_numbers:
   - '21114'
   editor: ΜΑΚΕΔΟΝΙΚΗ ΒΙΒ/ΚΗ // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -793086,15 +792962,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15780
   authors:
-  - ΒΙΤΑΛΗ, ΦΙΛΑΡΕΤΟΥ
+  - ΒΙΤΑΛΗΣ,ΦΙΛΑΡΕΤΟΣ
   language: el
   title: ΑΣΜΑΤΙΚΗ ΑΚΟΛΟΥΘΕΙΑ ΤΩΝ ΕΝ ΟΣΙΟΙΣ ΠΑΤΕΡΩΝ ΗΜΩΝ ΜΑΞΙΜΟΥ
   dewey: 230 ΒΙΤ
   entry_numbers:
   - '21116'
   editor: None // ΑΘΗΝΑ
   edition_year: 1977
@@ -793179,15 +793055,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15782
   authors:
-  - ΑΓΓΕΛΗ,ΙΩΑΝΝΗΣ
+  - ΑΓΓΕΛΗΣ,ΙΩΑΝΝΗΣ
   language: el
   title: ΠΑΙΔΑΓΩΓΙΚΑ ΕΡΕΘΙΣΜΑΤΑ
   entry_numbers:
   - '21118'
   editor: None // ΑΡΤΑ
   edition_year: 1975
   pages: 75
@@ -794391,15 +794267,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15808
   authors:
-  - ΑΝΑΓΝΩΣΤΟΠΟΥΛΟΥ-ΠΑΛΑΙΟΛΟΓΟΥ Θ.
+  - ΑΝΑΓΝΩΣΤΟΠΟΥΛΟΣ-ΠΑΛΑΙΟΛΟΓΟΣ,ΘΑΝΟΣ
   language: el
   title: ΠΕΡΙ ΗΠΕΙΡΟΥ ΚΑΙ ΑΛΒΑΝΙΑΣ
   dewey: 949.507 ΧΣ
   entry_numbers:
   - '21144'
   editor: None // ΑΘΗΝΑ
   edition_year: 1966
@@ -794536,15 +794412,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15811
   authors:
-  - ΑΡΧΙΜΑΝΔΡΙΤΟΥ ΣΑΒΒΑ ΑΧΙΛΛΕΩΣ
+  - ΣΑΒΒΑΣ ΑΧΙΛΛΕΑΣ,ΑΡΧΙΜΑΝΔΡΙΤΗΣ
   language: el
   title: ΤΟ ΒΙΒΛΙΟ ΤΟΥ ΘΕΟΥ
   dewey: 230 ΑΧΙ
   entry_numbers:
   - '21147'
   pages: 55
   topics: []
@@ -797105,15 +796981,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15864
   authors:
-  - ΒΑΓΙΑΚΑΚΟΥ,Δ.Β.
+  - ΒΑΓΙΑΚΑΚΟΣ,ΔΙΚΑΙΟΣ,Β.
   language: el
   title: ΜΑΝΗ (ΜΕΣΑ ΜΑΝΗ)
   dewey: 782.42 ΒΑΓ
   entry_numbers:
   - '21168'
   editor: ΠΑΡΝΑΣΣΟΣ // ΑΘΗΝΑ
   edition_year: 1968
@@ -797289,15 +797165,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15868
   authors:
-  - ΒΑΣΙΛΕΙΟΥ,ΣΩΚΤΡΑΤΗΣ
+  - ΒΑΣΙΛΕΙΟΥ,ΣΩΚΡΑΤΗΣ,Σ.
   language: el
   title: ΠΕΡΙΗΓΗΣΗ ΣΤΟ ΔΗΜΟΤΙΚΟ ΤΡΑΓΟΥΔΙ
   dewey: 782.42 ΒΑΣ
   entry_numbers:
   - '21172'
   editor: ΑΠΕΙΡΟΣ ΧΩΡΑ // ΑΘΗΝΑ
   edition_year: 2010
@@ -797338,15 +797214,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15869
   authors:
-  - ΒΑΣΙΛΕΙΟΥ,ΣΩΚΡΑΤΗΣ
+  - ΒΑΣΙΛΕΙΟΥ,ΣΩΚΡΑΤΗΣ,Σ.
   language: el
   title: ΠΕΡΙΗΓΗΣΗ ΣΤΟ ΔΗΜΟΤΙΚΟ ΤΡΑΓΟΥΔΙ
   dewey: 782.42 ΒΑΣ
   entry_numbers:
   - '21172'
   editor: None // ΑΘΗΝΑ
   edition_year: 2011
@@ -797387,15 +797263,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15870
   authors:
-  - ΒΑΣΙΛΕΙΟΥ,ΣΩΚΡΑΤΗΣ
+  - ΒΑΣΙΛΕΙΟΥ,ΣΩΚΡΑΤΗΣ,Σ.
   language: el
   title: ΠΕΡΙΗΓΗΣΗ ΣΤΟ ΔΗΜΟΤΙΚΟ ΤΡΑΓΟΥΔΙ
   dewey: 782.42 ΒΑΣ
   entry_numbers:
   - '21173'
   editor: ΑΠΕΙΡΟΣ ΧΩΡΑ // ΑΘΗΝΑ
   edition_year: 2013
@@ -797668,15 +797544,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15876
   authors:
-  - ΒΑΡΝΑΛΗΣ.ΚΩΣΤΑΣ
+  - ΒΑΡΝΑΛΗΣ,ΚΩΣΤΑΣ
   language: el
   title: ΠΡΟΣΚΥΝΗΤΗΣ
   dewey: 889.11 ΒΑΡ
   entry_numbers:
   - '21187'
   editor: ΚΕΔΡΟΣ // ΑΘΗΝΑ
   edition_year: 1976
@@ -799346,15 +799222,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15908
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: Ο ΓΥΡΟΣ ΤΟΥ ΚΟΣΜΟΥ ΣΕ 80 ΗΜΕΡΕΣ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '20971'
   editor: ΤΑ ΝΕΑ ΑΛΤΕΡ ΕΓΚΟ // ΑΘΗΝΑ
   edition_year: 2018
@@ -799866,15 +799742,15 @@
 - dbase_number: 15918
   authors: []
   language: el
   title: ΑΝΘΟΛΟΓΙΟ
   subtitle: ΓΙΑ ΤΑ ΠΑΙΔΙΑ ΤΟΥ ΔΗΜΟΤΙΚΟΥ ΜΕΡΟΣ ΤΡΙΤΟ
   dewey: 808.899 ΧΣ
   entry_numbers:
-  - Α1029
+  - '21029'
   editor: ΤΟ ΒΗΜΑ ΑΛΤΕΡ ΕΓΚΟ // ΑΘΗΝΑ
   edition_year: 2016
   pages: 335
   topics:
   - ΑΝΘΟΛΟΓΙΟ
   curator: ΚΕΧΑΓΙΟΓΛΟΥ,ΕΛΕΝΗ
   donors:
@@ -799885,15 +799761,15 @@
   ean: '9789605037710'
   original_entry:
     0: 15918
     1: Χ.Σ.
     2: ΑΝΘΟΛΟΓΙΟ
     3: ΓΙΑ ΤΑ ΠΑΙΔΙΑ ΤΟΥ ΔΗΜΟΤΙΚΟΥ ΜΕΡΟΣ ΤΡΙΤΟ
     4: 808.899Χ.Σ
-    5: Α1029
+    5: '21029'
     8: ΤΟ ΒΗΜΑ ΑΛΤΕΡ ΕΓΚΟ
     9: ΑΘΗΝΑ
     10: '2016'
     11: 335Σ
     12: ΑΝΘΟΛΟΓΙΟ
     13: ΑΝΘΟΛΟΓΙΟ
     14: ΑΝΘΟΛΟΓΙΟ
@@ -800832,15 +800708,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15937
   authors:
-  - ΑΝΤΕΡΣΕΝ,ΧΑΝΣ ΚΡΙΣΤΙΑΝ
+  - ANDERSEN,HANS,CHRISTIAN
   language: el
   title: ΤΑ ΠΙΟ ΓΝΩΣΤΑ ΠΑΡΑΜΥΘΙΑ
   dewey: 808.899 ΑΝΤ
   entry_numbers:
   - '21012'
   editor: ΤΑ ΝΕΑ ΑΛΤΕΡ ΕΓΚΟ // ΑΘΗΝΑ
   edition_year: 2018
@@ -801350,15 +801226,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15947
   authors:
-  - ΑΔΑΜΟΠΟΥΛΟΥ,ΝΤΙΝΑ-ΠΡΑΣΣΑ,ΑΝΝΙΤΑ
+  - ΑΔΑΜΟΠΟΥΛΟΥ,ΝΤΙΝΑ
+  - ΠΡΑΣΣΑ,ΑΝΝΙΤΑ
   language: el
   title: ΑΝΔΡΕΑΣ ΜΙΑΟΥΛΗΣ
   dewey: 938.509 ΑΔΑ
   entry_numbers:
   - '21051'
   edition: '2'
   editor: ΤΑ ΝΕΑ ΑΛΤΕΡ ΕΓΚΟ // ΑΘΗΝΑ
@@ -801920,15 +801797,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15958
   authors:
-  - ΒΙΣΚΟΝΤΙ,ΛΟΥΚΙΝΟ
+  - VISCONTI,LUCHINO
   language: el
   title: ΑΝΤΖΕΛΟ
   dewey: 850.11 ΒΙΣ
   entry_numbers:
   - '21190'
   translators:
   - ΧΡΙΣΤΟΣΤΟΜΙΔΗΣ,Α.
@@ -803935,15 +803812,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15998
   authors:
-  - ΒΑΡΔΙΝΟΓΙΑΝΝΗΣ,ΒΑΡΔΗΣ-ΑΡΩΝΗΣ,ΠΑΝΑΓΙΩΤΗΣ
+  - ΒΑΡΔΙΝΟΓΙΑΝΝΗΣ,ΒΑΡΔΗΣ
+  - ΑΡΩΝΗΣ,ΠΑΝΑΓΙΩΤΗΣ
   language: el
   title: ΟΙ ΜΙΣΟΙ ΣΤΑ ΣΙΔΕΡΑ
   subtitle: ΟΤΑΝ ΑΝΟΙΞΑΝ ΟΙ ΒΑΡΙΕΣ ΑΜΠΑΡΕΣ ΚΙ ΕΚΛΕΙΣΑΝ ΜΕΤΑ ΤΟΥΣ ΤΟ ΜΙΣΟ
   dewey: 949.507 ΒΑΡ
   entry_numbers:
   - '21207'
   editor: ΦΙΛΙΣΤΩΡ // ΑΘΗΝΑ
@@ -803985,15 +803863,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 15999
   authors:
-  - ΑΝΔΡΕΑΔΟΥ,ΧΑΡΑ
+  - ΑΝΔΡΕΙΔΟΥ,ΧΑΡΑ
   language: el
   title: ΣΤΑ ΤΕΣΣΕΡΑ ΣΗΜΕΙΑ ΤΟΥ ΟΡΙΖΟΝΤΑ
   dewey: 889.21 ΑΝΔ
   entry_numbers:
   - '21208'
   editor: ΛΙΒΑΝΗ // ΑΘΗΝΑ
   edition_year: 2014
@@ -808691,15 +808569,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16093
   authors:
-  - ΒΑΣΙΛΑΚΗΣ,ΧΡΗΣΟΣ
+  - ΒΑΣΙΛΑΚΗΣ,ΧΡΗΣΤΟΣ
   language: el
   title: Ο ΙΕΡΟΣ ΝΑΟΣ ΚΟΙΜΗΣΕΩΣ ΘΕΟΤΟΚΟΥ ΚΟΜΜΕΝΟΥ ΑΡΤΑΣ
   dewey: 230 ΒΑΣ
   entry_numbers:
   - '21310'
   editor: ΒΙΒΛΙΟΓΝΩΣΙΑ // ΑΘΗΝΑ
   edition_year: 2021
@@ -810177,15 +810055,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 16122
   authors:
-  - VERDET,JAEN-PIERRE
+  - VERDET,JEAN-PIERRE
   language: el
   title: ΜΙΚΡΗ ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΤΟ ΣΥΜΠΑΝ
   dewey: 808.899 VER
   entry_numbers:
   - '21334'
   editor: ΑΜΜΟΣ // ΑΘΗΝΑ
   edition_year: 1993
@@ -817561,15 +817439,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16269
   authors:
-  - ΒΑΓΕΝΑ-ΠΑΠΑΙΩΑΝΝΟΥ ΛΑΜΠΡΙΝΗ
+  - ΒΑΓΕΝΑ-ΠΑΠΑΙΩΑΝΝΟΥ,ΛΑΜΠΡΙΝΗ
   language: el
   title: ΒΑΛΚΑΝΙΚΗ ΠΑΡΑΔΟΣΙΑΚΗ ΑΡΧΙΤΕΚΤΟΝΙΚΗ
   dewey: 721 ΒΑΓ
   entry_numbers:
   - '21731'
   translators:
   - ΜΟΛΦΕΤΑ,ΝΙΚΗ
@@ -817760,15 +817638,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16273
   authors:
-  - ΑΛΕΞΑΝΔΡΟΣ ΔΟΥΜΑΣ
+  - DUMAS,ALEXANDRE
   language: el
   title: ΟΙ ΤΡΕΙΣ ΣΩΜΑΤΟΦΥΛΑΚΕΣ
   dewey: 808.899 ΔΟΥ
   entry_numbers:
   - '21743'
   editor: ΠΑΠΑΔΟΠΟΥΛΟΣ // None
   pages: 139
@@ -818824,15 +818702,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16295
   authors:
-  - ΒΑΛΕΤΑΣ,Γ.
+  - ΒΑΛΕΤΑΣ,ΓΕΩΡΓΙΟΣ
   language: el
   title: ΚΟΡΑΗΣ ΑΠΑΝΤΑ - ΤΑ ΠΡΩΤΟΤΥΠΑ ΕΡΓΑ
   dewey: 888.34 ΒΑΛ
   entry_numbers:
   - '21761'
   editor: ΕΚΔΟΣΕΙΣ ΔΩΡΙΚΟΣ // None
   topics:
@@ -820547,15 +820425,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16331
   authors:
-  - ΑΡΝΤΟΝΕ,ΒΙΟΛΑ
+  - ARDONE,VIOLA
   language: el
   title: ΤΟ ΤΡΕΝΟ ΤΩΝ ΠΑΙΔΙΩΝ
   dewey: 850.11 ΑΡΝ
   entry_numbers:
   - '21815'
   editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
   pages: 302
@@ -820596,15 +820474,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16332
   authors:
-  - ΑΡΑΜΠΟΥΡΟΥ,ΦΕΡΝΑΝΤΟ
+  - ARAMBURU,FERNANDO
   language: el
   title: ΤΑ ΧΡΟΝΙΑ ΤΗΣ ΒΡΑΔΥΤΗΤΑΣ
   dewey: 860.11 ΑΡΑ
   entry_numbers:
   - '21816'
   editor: ΠΑΤΑΚΗ // ΑΘΗΝΑ
   pages: 252
@@ -822874,15 +822752,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16379
   authors:
-  - ΑΡΡΙΑΝΟΣ
+  - ARRIANO,LUCIO FLAVIO
   language: el
   title: ΑΛΕΞΑΝΔΡΟΥ ΑΝΑΒΑΣΙΣ
   dewey: 881 ΑΡΡ
   entry_numbers:
   - '21870'
   editor: ΖΗΤΡΟΣ // None
   edition_year: 2004
@@ -822923,15 +822801,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16380
   authors:
-  - ΑΡΡΙΑΝΟΣ
+  - ARRIANO,LUCIO FLAVIO
   language: el
   title: ΑΛΕΞΑΝΔΡΟΥ ΑΝΑΒΑΣΙΣ ΒΙΒΛΙΑ 3,4,5
   dewey: 881 ΑΡΡ
   entry_numbers:
   - '21869'
   editor: ΖΗΤΡΟΣ // None
   edition_year: 2003
@@ -822972,15 +822850,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16381
   authors:
-  - ΑΡΡΙΑΝΟΣ
+  - ARRIANO,LUCIO FLAVIO
   language: el
   title: ΑΛΕΞΑΝΔΡΟΥ ΑΝΑΒΑΣΙΣ ΒΙΒΛΙΑ 1,2
   dewey: 881 ΑΡΡ
   entry_numbers:
   - '21868'
   editor: ΖΗΤΡΟΣ // None
   edition_year: 2004
@@ -828546,15 +828424,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16493
   authors:
-  - ΑΝΝΑ ΚΟΜΝΗΝΗ
+  - ΚΟΜΝΗΝΗ,ΑΝΝΑ
   language: el
   title: ΑΛΕΞΙΑΣ ΤΟΜΟΙ Α,Β
   dewey: 881 ΚΟΜ
   entry_numbers:
   - '21892'
   translators:
   - ΚΩΝΣΤΑΝΤΟΠΟΥΛΟΣ,
@@ -829049,15 +828927,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16503
   authors:
-  - ΑΡΡΙΑΝΟΣ
+  - ARRIANO,LUCIO FLAVIO
   language: el
   title: ΑΛΕΞΑΝΔΡΟΥ ΑΝΑΒΑΣΙΣ Α,Β,Γ,Δ,Ε,ΣΤ,Ζ
   dewey: 881 ΑΡΡ
   entry_numbers:
   - '21911'
   translators:
   - ΛΥΚΑΣ,
@@ -829808,15 +829686,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 16518
   authors:
-  - ΒΑΡΑΣ ΔΗΜΗΤΡΙΟΣ
+  - ΒΑΡΑΣ,ΔΗΜΗΤΡΙΟΣ
   language: el
   title: ΙΔΟΥ Ο ΝΥΜΦΙΟΣ ΕΡΧΕΤΑΙ ΕΝ ΤΩ ΜΕΣΩ ΤΗΣ ΝΥΚΤΟΣ!
   dewey: 230 ΒΑΡ
   entry_numbers:
   - '22004'
   editor: None // ΑΓΡΙΝΙΟ
   edition_year: 1979
@@ -829856,15 +829734,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16519
   authors:
-  - ΒΑΣΙΛΟΠΟΥΛΟΣ ΧΑΡΑΛΑΜΠΟΣ
+  - ΒΑΣΙΛΟΠΟΥΛΟΣ,ΑΡΧΙΜΑΝΔΡΙΤΗΣ ΧΑΡΑΛΑΜΠΟΣ
   language: el
   title: ΟΙ ΑΓΙΟΙ ΤΗΣ ΜΥΤΙΛΗΝΗΣ ΡΑΦΑΗΛ ΚΑΙ ΟΙ ΣΥΝ ΑΥΤΟ
   dewey: 230 ΒΑΣ
   entry_numbers:
   - '22003'
   editor: ΟΡΘΟΔΟΞΟΣ ΤΥΠΟΣ // ΑΘΗΝΑ
   edition_year: 2001
@@ -830001,15 +829879,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16522
   authors:
-  - ΒΑΣΙΛΟΠΟΥΛΟΣ,ΧΑΡΑΛΑΜΠΟΣ ΑΡΧΙΜΑΝΔΡΙΤΗΣ
+  - ΒΑΣΙΛΟΠΟΥΛΟΣ,ΑΡΧΙΜΑΝΔΡΙΤΗΣ ΧΑΡΑΛΑΜΠΟΣ
   language: el
   title: ΒΙΟΙ ΑΓΙΩΝ ΣΕΙΡΑ 9
   dewey: 230 ΒΑΣ
   entry_numbers:
   - '22000'
   editor: ΟΡΘΟΔΟΞΟΣ ΤΥΠΟΣ // ΑΘΗΝΑ
   pages: 72
@@ -830048,15 +829926,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16523
   authors:
-  - ΒΑΣΙΛΟΠΟΥΛΟΣ,ΧΑΡΑΛΑΜΠΟΣ
+  - ΒΑΣΙΛΟΠΟΥΛΟΣ,ΑΡΧΙΜΑΝΔΡΙΤΗΣ ΧΑΡΑΛΑΜΠΟΣ
   language: el
   title: Ο ΓΑΜΟΣ ΠΩΣ ΘΑ ΕΠΙΤΥΧΗ
   dewey: 230 ΒΑΣ
   entry_numbers:
   - '7802'
   editor: ΟΡΘΟΔΟΞΟΣ ΤΥΠΟΣ // ΑΘΗΝΑ
   pages: 96
@@ -830143,15 +830021,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16525
   authors:
-  - ΒΑΣΙΛΟΠΟΥΛΟΣ,ΧΑΡΑΛΑΜΠΟΣ
+  - ΒΑΣΙΛΟΠΟΥΛΟΣ,ΑΡΧΙΜΑΝΔΡΙΤΗΣ ΧΑΡΑΛΑΜΠΟΣ
   language: el
   title: ΚΑΤΑ ΑΝΤΙΧΡΙΣΤΩΝ
   dewey: 230 ΒΑΣ
   entry_numbers:
   - '22005'
   editor: ΟΡΘΟΔΟΞΟΣ ΤΥΠΟΥ // ΑΘΗΝΑ
   edition_year: 1984
@@ -830334,15 +830212,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16529
   authors:
-  - ΒΕΡΝΕΖΟΣ,ΙΩΑΝΝΗΣ ΙΕΡΕΑΣ
+  - ΒΕΡΝΕΖΟΣ,ΙΩΑΝΝΗΣ
   language: el
   title: ΒΙΟΣ ΚΑΙ ΝΕΑ ΘΑΥΜΑΤΑ ΤΟΥ ΟΣΙΟΥ ΙΩΑΝΝΟΥ ΤΟΥ ΡΩΣΣΟΥ
   dewey: 230 ΒΕΡ
   entry_numbers:
   - '22006'
   editor: ΜΕΛΙΣΣΑ // ΑΘΗΝΑ
   edition_year: 1999
@@ -830382,15 +830260,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16530
   authors:
-  - ΒΑΣΤΑΣ,ΙΕΡΕΜΙΑΣ ΑΡΧΙΜΑΝΔΡΗΤΗΣ
+  - ΒΑΣΤΑΣ,ΑΡΧΙΜΑΝΔΡΗΤΗΣ ΙΕΡΕΜΙΑΣ
   language: el
   title: ΠΑΝΑΓΙΑ Η ΔΙΑΣΩΖΟΥΣΑ
   dewey: 230 ΒΑΣ
   entry_numbers:
   - '22007'
   edition: '4'
   editor: Ι.Μ.ΠΡ.ΠΑΝΑ.ΔΙΑΣ. // ΠΑΤΜΟΣ
@@ -843923,15 +843801,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16810
   authors:
-  - ΑΒΡΑΑΜ,ΚΩΣΤΑ
+  - ΑΒΡΑΑΜ,ΚΩΣΤΑΣ
   language: el
   title: ΠΙΚΡΕΣ ΩΡΕΣ
   dewey: 889.21 ΑΒΡ
   entry_numbers:
   - '22183'
   editor: ΕΛΛΗΝΙΚΗ ΓΡΑΜΜΗ // ΑΘΗΝΑ
   edition_year: 1975
@@ -844181,15 +844059,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16815
   authors:
-  - ΑΙΤΜΑΤΩΦ,ΤΣΙΝΓΚΙΖ
+  - AITMATOV,CHINGHIZ
   language: el
   title: ΠΡΟΣΩΠΟ ΜΕ ΠΡΟΣΩΠΟ
   dewey: 891.73 ΑΙΤ
   entry_numbers:
   - '22187'
   editor: ΚΟΤΟΝΤΖΗ // ΑΘΗΝΑ
   edition_year: 1979
@@ -845218,15 +845096,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16836
   authors:
-  - ΑΡΡΙΑΝΟΥ
+  - ARRIANO,LUCIO FLAVIO
   language: el
   title: ΑΛΕΞΑΝΔΡΟΥ ΑΝΑΒΑΣΙΣ
   dewey: 881 ΑΡΙ
   entry_numbers:
   - '22166'
   pages: 195
   topics:
@@ -845513,15 +845391,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16842
   authors:
-  - ΒΛΑΧΟΓΙΑΝΝΗ,ΓΙΑΝΝΗ
+  - ΒΛΑΧΟΓΙΑΝΝΗΣ,ΓΙΑΝΝΗΣ
   language: el
   title: ΤΑ ΠΑΛΗΚΑΡΙΑ ΤΑ ΠΑΛΙΑ
   dewey: 889.21 ΒΛΑ
   entry_numbers:
   - '22164'
   editor: ΙΣΤΟΡΙΚΗ ΕΡΕΥΝΑ // ΑΘΗΝΑ
   pages: 132
@@ -846912,15 +846790,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16871
   authors:
-  - ΒΑΡΒΑΡΕΣΟΣ,ΑΝ
+  - ΒΑΡΒΑΡΕΣΟΣ,ΑΝ.
   language: el
   title: Η ΠΑΡΑΓΩΓΙΚΟΤΗΣ ΕΙΣ ΤΑΣ ΔΗΜΟΣΙΑΣ ΥΠΗΡΕΣΙΑΣ
   dewey: 351 ΒΑΡ
   entry_numbers:
   - '22242'
   editor: ΓΚΕΛΜΠΕΣΗΣ // ΑΘΗΝΑ
   edition_year: 1959
@@ -848015,15 +847893,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16894
   authors:
-  - ΒΟΥΡΒΕΡΗΣ,ΚΩΝΣΤ.
+  - ΒΟΥΡΒΕΡΗΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΚΛΑΣΣΙΚΗ ΠΑΙΔΕΙΑ ΚΑΙ ΖΩΗ
   dewey: 880.9 ΒΟΥ
   entry_numbers:
   - '22220'
   editor: ΕΛΛ.ΑΝΘΡΩΠ.ΕΤΑΙΡΕΙΑ // ΑΘΗΝΑ
   edition_year: 1969
@@ -849097,15 +848975,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16916
   authors:
-  - ΑΙΝΙΑΝ-ΜΑΖΑΡΑΚΗΣ,Ι.Κ
+  - ΑΙΝΙΑΝ-ΜΑΖΑΡΑΚΗΣ,ΙΩΑΝΝΗΣ,Κ.
   language: el
   title: ΔΙΑΓΡΑΜΜΑ ΤΗΣ ΝΕΟΤΕΡΗΣ ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑΣ
   dewey: 938.401 ΑΙΝ
   entry_numbers:
   - '9424'
   editor: None // ΑΘΗΝΑ
   edition_year: 2007
@@ -850169,15 +850047,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16938
   authors:
-  - ΑΠΟΣΤΟΛΙΔΗΣ,Τ.-ΠΑΠΑΔΑΤΟΣ,ΑΛΕΚΟΣ
+  - ΑΠΟΣΤΟΛΙΔΗΣ,ΤΑΣΟΣ
+  - ΠΑΠΑΔΑΤΟΣ,ΑΛΕΚΟΣ
   language: el
   title: ΑΡΙΣΤΟΤΕΛΗΣ
   dewey: 808.899 ΑΠΟ
   entry_numbers:
   - '22275'
   editor: ΙΚΑΡΟΣ // ΑΘΗΝΑ
   edition_year: 2022
@@ -852834,15 +852713,16 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 16993
   authors:
-  - ΑΙΖΕΝΜΑΝ,ΡΟΜΠΕΡΤ-ΜΑΙΚΛ ΟΥΑΙΖ
+  - EISENMAN,ROBERT
+  - WISE,MICHAEL
   language: el
   title: ΑΠΟΚΑΛΥΠΤΟΝΤΑΣ ΤΑ 50 ΧΕΙΡΟΓΡΑΦΑ-ΚΛΕΙΔΙΑ ΤΗΣ ΝΕΚΡΗΣ ΘΑΛΑΣΣΑΣ
   dewey: 296.155 ΑΙΖ
   entry_numbers:
   - '22325'
   translators:
   - ΜΟΡΦΟΣ,ΧΡΗΣΤΟΣ
@@ -855361,15 +855241,17 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 17044
   authors:
-  - ADELBERG,E-JAWETZ,E-MELNICK,J
+  - ADELBERG,E.
+  - JAWETZ,E.
+  - MELNICK,J.
   language: el
   title: ΙΑΤΡΙΚΗ ΜΙΚΡΟΒΙΟΛΟΓΙΑ
   dewey: 616.904 ADE
   entry_numbers:
   - '22442'
   translators:
   - ΠΑΠΑΚΩΝΣΤΑΝΤΙΝΟΥ,ΑΘ.
@@ -856109,15 +855991,15 @@
     25: null
     26: null
     27: null
     28: null
     29: null
 - dbase_number: 17059
   authors:
-  - ΒΛΑΧΟΣ,Ι.Δ
+  - ΒΛΑΧΟΣ,Ι.,Δ.
   language: el
   title: ΚΕΝΤΡΙΚΟ ΝΕΥΡΙΚΟ ΣΥΣΤΗΜΑ
   dewey: 616.8 ΒΛΑ
   entry_numbers:
   - '22647'
   editor: ΠΑΡΙΣΙΑΝΟΣ // ΑΘΗΝΑ
   edition_year: 1985
@@ -856765,15 +856647,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17072
   authors:
-  - ΒΑΡΩΝΟΥ,Δ.Δ.
+  - ΒΑΡΩΝΟΣ,Δ.,Δ.
   language: el
   title: ΙΑΤΡΙΚΗ ΦΑΡΜΑΚΟΛΟΓΙΑ
   dewey: 615.1 ΒΑΡ
   entry_numbers:
   - '22521'
   editor: ΠΑΡΙΣΙΑΝΟΣ // ΑΘΗΝΑ
   edition_year: 1987
@@ -857113,15 +856995,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17079
   authors:
-  - ΒΑΣΙΛΕΙΟΥ,Δ.Ν.
+  - ΒΑΣΙΛΕΙΟΥ,Δ.,Ν.
   language: el
   title: ΚΛΙΝΙΚΑ ΘΕΜΑΤΑ ΠΡΑΚΤΙΚΟΥ ΕΝΔΙΑΦΕΡΟΝΤΟΣ
   dewey: 616.075 ΒΑΣ
   entry_numbers:
   - '22525'
   editor: ΓΑΛΗΝΟΣ // ΑΘΗΝΑ
   edition_year: 1966
@@ -857311,15 +857193,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17083
   authors:
-  - ΒΑΛΑΩΡΑ,ΒΑΣΙΛΕΙΟΥ
+  - ΒΑΛΑΩΡΑΣ,ΒΑΣΙΛΕΙΟΣ
   language: el
   title: ΠΕΡΙΒΑΛΛΟΝ ΚΑΙ ΥΓΕΙΑ
   dewey: 613 ΒΑΛ
   entry_numbers:
   - '22528'
   editor: None // ΑΘΗΝΑ
   edition_year: 1978
@@ -857844,15 +857726,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17094
   authors:
-  - ΒΑΛΑΩΡΑ,ΒΑΣΙΛΕΙΟΥ
+  - ΒΑΛΑΩΡΑΣ,ΒΑΣΙΛΕΙΟΣ
   language: el
   title: ΑΤΟΜΙΚΗ ΚΑΙ ΔΗΜΟΣΙΑ ΥΓΙΕΙΝΗ
   dewey: 614 ΒΑΛ
   entry_numbers:
   - '22541'
   editor: None // ΑΘΗΝΑ
   edition_year: 1979
@@ -866895,15 +866777,17 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17274
   authors:
-  - ΒΑΡΣΑΜΗΣ-ΚΟΜΙΤΟΠΟΥΛΟΣ-ΣΑΒΒΑΚΗΣ
+  - ΒΑΡΣΑΜΗΣ
+  - ΚΟΜΙΤΟΠΟΥΛΟΣ
+  - ΣΑΒΒΑΚΗΣ
   language: el
   title: ΘΕΜΑΤΑ ΕΣΩΤΕΡΙΚΗΣ ΠΑΘΟΛΟΓΙΑΣ
   dewey: 615.5 ΒΑΡ
   entry_numbers:
   - '22667'
   editor: None // ΑΘΗΝΑ
   edition_year: 1996
@@ -869220,15 +869104,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17319
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: ΜΙΑ ΠΛΩΤΗ ΠΟΛΙΤΕΙΑ
   subtitle: ΝΑΥΤΙΚΟΣ ΑΠΟΚΛΕΙΣΜΟΣ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '22777'
   translators:
@@ -869274,15 +869158,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17320
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: ΡΟΒΗΡΟΣ Ο ΚΑΤΑΚΤΗΤΗΣ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '20776'
   translators:
   - ΤΡΑΙΤΟΡΑΚΗ,Χ.
@@ -869327,15 +869211,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17321
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΣ
+  - VERNE,JULES
   language: el
   title: ΒΟΡΡΑΣ ΕΝΑΝΤΙΟΝ ΝΟΤΟΥ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '22775'
   translators:
   - ΜΑΥΡΟΜΑΤΑΚΗ,Μ.
@@ -869538,16 +869422,17 @@
     29: null
     30: null
 - dbase_number: 17325
   authors:
   - ΚΑΡΙΖΩΝΗ,ΚΑΤΕΡΙΝΑ
   language: el
   title: ΜΕΓΑΛΟ ΑΛΓΕΡΙ
+  dewey: 889.21 ΚΑΡ
   entry_numbers:
-  - '2770'
+  - '22770'
   editor: ΚΑΣΤΑΝΙΩΤΗΣ // ΑΘΗΝΑ
   edition_year: 2006
   pages: 272
   topics:
   - ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   donors:
   - ΚΑΛΟΜΠΑΤΣΟΥ,ΑΘΗΝΑ
@@ -869555,16 +869440,16 @@
   has_dvd: false
   offprint: false
   isbn: '9600342547'
   original_entry:
     0: 17325
     1: ΚΑΡΙΖΩΝΗ,ΚΑΤΕΡΙΝΑ
     2: ΜΕΓΑΛΟ ΑΛΓΕΡΙ
-    4: 889.21ΚΑΡ2
-    5: '2770'
+    4: 889.21ΚΑΡ
+    5: '22770'
     8: ΚΑΣΤΑΝΙΩΤΗΣ
     9: ΑΘΗΝΑ
     10: '2006'
     11: '272'
     12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -871234,35 +871119,35 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17358
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  - VERNE,JULES
   language: el
   title: Ο ΚΥΡΙΑΡΧΟΣ ΤΟΥ ΚΟΣΜΟΥ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
-  - 9170Α
+  - 09170
   translators:
   - ΟΛΥΜΠΙΟΥ,Λ.
   editor: ΑΤΤΙΚΟΣ // ΑΘΗΝΑ
   pages: 212
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 17358
     1: ΒΕΡΝ,ΙΟΥΛΙΟΥ
     2: Ο ΚΥΡΙΑΡΧΟΣ ΤΟΥ ΚΟΣΜΟΥ
     4: 808.899ΒΕΡ
-    5: 9170Α
+    5: 09170
     6: Λ.ΟΛΥΜΠΙΟΥ
     8: ΑΤΤΙΚΟΣ
     9: ΑΘΗΝΑ
     11: '212'
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -871283,35 +871168,35 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17359
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  - VERNE,JULES
   language: el
   title: ΚΟΥΡΣΑΡΟΙ ΤΟΥ ΑΙΓΑΙΟΥ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
-  - 9175Α
+  - 09175
   translators:
   - ΚΩΣΤΕΛΕΝΟΣ,Δ.Π.
   editor: ΑΤΤΙΚΟΣ // ΑΘΗΝΑ
   pages: 206
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 17359
     1: ΒΕΡΝ,ΙΟΥΛΙΟΥ
     2: ΚΟΥΡΣΑΡΟΙ ΤΟΥ ΑΙΓΑΙΟΥ
     4: 808.899ΒΕΡ
-    5: 9175Α
+    5: 09175
     6: Δ.Π.ΚΩΣΤΕΛΕΝΟΣ
     8: ΑΤΤΙΚΟΣ
     9: ΑΘΗΝΑ
     11: '206'
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -871332,15 +871217,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17360
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  - VERNE,JULES
   language: el
   title: ΑΠΟ ΤΗ ΓΗ ΣΤΗ ΣΕΛΗΝΗ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '13461'
   translators:
   - ΟΛΥΜΠΙΟΥ,Λ.
@@ -871381,42 +871266,43 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17361
   authors:
-  - ΑΝΤΕΡΣΕΝ,ΧΑΝΣ ΚΡΙΣΤΙΑΝ
+  - ANDERSEN,HANS,CHRISTIAN
   language: el
   title: ΑΠΑΝΤΑ Ε
   dewey: 808.899 ΑΝΤ
-  entry_numbers: []
+  entry_numbers:
+  - '22802'
   translators:
   - ΠΡΩΤΟΠΑΠΑ,Σ.
   editor: ΑΡΣΕΝΙΔΗΣ // ΑΘΗΝΑ
   pages: 188
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 17361
     1: ΑΝΤΕΡΣΕΝ,ΧΑΝΣ ΚΡΙΣΤΙΑΝ
     2: ΑΠΑΝΤΑ Ε
     4: 808.899ΑΝΤ
+    5: '22802'
     6: Σ.ΠΡΩΤΟΠΑΠΑ
     8: ΑΡΣΕΝΙΔΗΣ
     9: ΑΘΗΝΑ
     11: '188'
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     3: null
-    5: null
     7: null
     10: null
     15: null
     16: null
     17: null
     18: null
     19: null
@@ -871429,42 +871315,43 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17362
   authors:
-  - ΑΝΤΡΙΟΥΣ,ΤΖΟΥΛΙ
+  - ANDREWS,JULIE
   language: el
   title: ΜΑΝΤΥ
   dewey: 808.899 ΑΝΤ
-  entry_numbers: []
+  entry_numbers:
+  - '22803'
   translators:
   - ΣΙΝΟΥ,Κ.
   editor: ΓΕΜΕΝΤΖΟΠΟΥΛΟΣ // ΑΘΗΝΑ
   pages: 148
   topics:
   - ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 17362
     1: ΑΝΤΡΙΟΥΣ,ΤΖΟΥΛΙ
     2: ΜΑΝΤΥ
     4: 808.899ΑΝΤ
+    5: '22803'
     6: Κ.ΣΙΝΟΥ
     8: ΓΕΜΕΝΤΖΟΠΟΥΛΟΣ
     9: ΑΘΗΝΑ
     11: '148'
     12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
     3: null
-    5: null
     7: null
     10: null
     15: null
     16: null
     17: null
     18: null
     19: null
@@ -871627,15 +871514,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17366
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  - VERNE,JULES
   language: el
   title: ΜΠΡΟΣΤΑ ΣΤΗ ΣΗΜΑΙΑ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '22804'
   editor: ΑΣΤΗΡ // ΑΘΗΝΑ
   edition_year: 1978
@@ -875001,15 +874888,16 @@
 - dbase_number: 17436
   authors:
   - ΚΑΛΑΤΖΟΠΟΥΛΟΣ,ΓΙΑΝΝΗΣ
   language: el
   title: ΘΕΑΤΡΟ ΓΙΑ ΠΑΙΔΙΑ ΚΑΙ ... ΕΞΥΠΝΟΥΣ ΜΕΓΑΛΟΥΣ
   dewey: 886.2 ΚΑΛ
   entry_numbers:
-  - 22839,22840
+  - '22839'
+  - '22840'
   editor: ΦΙΛΝΤΙΣΙ // ΑΘΗΝΑ
   edition_year: 2021
   pages: 335
   topics:
   - ΘΕΑΤΡΟ
   - ΘΕΑΤΡΟ ΓΙΑ ΠΑΙΔΙΑ
   - ΘΕΑΤΡΙΚΟ ΓΙΑ ΠΑΙΔΙΑ
@@ -875021,15 +874909,15 @@
   offprint: false
   ean: '9786185456481'
   original_entry:
     0: 17436
     1: ΚΑΛΑΤΖΟΠΟΥΛΟΣ,ΓΙΑΝΝΗΣ
     2: ΘΕΑΤΡΟ ΓΙΑ ΠΑΙΔΙΑ ΚΑΙ ... ΕΞΥΠΝΟΥΣ ΜΕΓΑΛΟΥΣ
     4: 886.2ΚΑΛ
-    5: 22839,22840
+    5: 22839-22840
     8: ΦΙΛΝΤΙΣΙ
     9: ΑΘΗΝΑ
     10: '2021'
     11: '335'
     12: ΘΕΑΤΡΟ
     13: ΘΕΑΤΡΟ ΓΙΑ ΠΑΙΔΙΑ
     14: ΘΕΑΤΡΙΚΟ ΓΙΑ ΠΑΙΔΙΑ
@@ -875726,15 +875614,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17450
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  - VERNE,JULES
   language: el
   title: ΜΙΧΑΗΛ ΣΤΡΟΓΚΟΦ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '22859'
   editor: ΣΜΥΡΝΙΩΤΑΚΗΣ // ΑΘΗΝΑ
   pages: 254
@@ -875776,15 +875664,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17451
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  - VERNE,JULES
   language: el
   title: Ο ΔΕΚΑΠΕΝΤΑΕΤΗΣ ΠΛΟΙΑΡΧΟΣ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '22860'
   editor: ΣΜΥΡΝΙΩΤΑΚΗΣ // ΑΘΗΝΑ
   pages: 254
@@ -875826,15 +875714,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17452
   authors:
-  - ΒΕΡΝ,ΙΟΥΛΙΟΥ
+  - VERNE,JULES
   language: el
   title: ΑΠΟ ΤΗ ΓΗ ΣΤΗ ΣΕΛΗΝΗ
   dewey: 808.899 ΒΕΡ
   entry_numbers:
   - '22861'
   translators:
   - ΚΑΡΑΔΗΜΑΣ,ΔΗΜΗΤΡΗΣ
@@ -876698,15 +876586,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17469
   authors:
-  - ΒΕΤΣΙΟΣ,ΕΛΕΥΘΕΡΙΟΣ
+  - ΒΕΤΣΙΟΣ,ΕΛΕΥΘΕΡΙΟΣ,Λ.
   language: el
   title: ΔΗΜΟΣΘΕΝΟΥΣ ΠΡΟΣ ΠΟΛΥΚΛΕΑ ΠΕΡΙ ΤΟΥ ΕΠΙΤΡΙΗΡΑΡΧΗΜΑΤΟΣ
   subtitle: Η ΕΞΩΤΕΡΙΚΗ ΠΟΛΙΤΙΚΗ ΤΗΣ ΑΘΗΝΑΣ ΚΑΤΑ ΤΟΝ 4ΟΝ ΑΙΩΝΑ Π.Χ
   dewey: 938.02 ΒΕΤ
   entry_numbers:
   - '22873'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -877644,15 +877532,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17488
   authors:
-  - ΑΣΔΡΑΧΑΣ,ΣΠΥΡΟΣ
+  - ΑΣΔΡΑΧΑΣ,ΣΠΥΡΟΣ,Ι.
   language: el
   title: ΟΙΚΟΝΟΜΙΑ ΚΑΙ ΝΟΟΤΡΟΠΙΕΣ
   dewey: 949.505 ΑΣΔ
   entry_numbers:
   - '22907'
   editor: ΕΡΜΗΣ // ΑΘΗΝΑ
   edition_year: 1988
@@ -878351,15 +878239,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17502
   authors:
-  - ΒΑΚΑΛΟΠΟΥΛΟΥ,ΚΩΝΣΤΑΝΤΙΝΟΥ
+  - ΒΑΚΑΛΟΠΟΥΛΟΣ,ΚΩΝΣΤΑΝΤΙΝΟΣ
   language: el
   title: ΟΙΚΟΝΟΜΙΚΗ ΛΕΙΤΟΥΡΓΙΑ ΤΟΥ ΜΑΚΕΔΟΝΙΚΟΥ ΚΑΙ ΘΡΑΚΙΚΟΥ ΧΩΡΟΥ ΣΤΑ
   subtitle: ΜΕΣΑ ΤΟΥ 19ΟΥ ΑΙΩΝΑ ΣΤΑ ΠΛΑΙΣΙΑ ΤΟΥ ΔΙΕΘΝΟΥΣ ΕΜΠΟΡΙΟΥ
   dewey: 330.949 ΒΑΚ
   entry_numbers:
   - '22891'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
@@ -879653,14 +879541,15 @@
     28: null
     29: null
     30: null
 - dbase_number: 17528
   authors:
   - ΦΩΤΙΑΔΟΥ,ΜΑΡΙΑ
   title: ΟΜΑΔΕΣ ΑΙΜΑΤΟΣ-RH-ΑΙΜΟΛΥΤΙΚΗ ΑΝΑΙΜΙΑ ΤΩΝ ΝΕΟΓΝΩΝ
+  dewey: 610.73 ΦΩΤ
   entry_numbers:
   - '22930'
   editor: None // ΘΕΣΣΑΛΟΝΙΚΗ
   edition_year: 1980
   pages: 38
   topics:
   - ΠΤΥΧΙΑΚΗ ΕΡΓΑΣΙΑ
@@ -879669,15 +879558,15 @@
   has_cd: false
   has_dvd: false
   offprint: false
   original_entry:
     0: 17528
     1: ΦΩΤΙΑΔΟΥ,ΜΑΡΙΑ
     2: ΟΜΑΔΕΣ ΑΙΜΑΤΟΣ-RH-ΑΙΜΟΛΥΤΙΚΗ ΑΝΑΙΜΙΑ ΤΩΝ ΝΕΟΓΝΩΝ
-    4: 610.73ΦΩΤ0
+    4: 610.73ΦΩΤ
     5: '22930'
     9: ΘΕΣΣΑΛΟΝΙΚ
     10: '1980'
     11: '38'
     12: ΠΤΥΧΙΑΚΗ ΕΡΓΑΣΙΑ
     13: ΠΤΥΧΙΑΚΗ ΕΡΓΑΣΙΑ
     14: ΠΤΥΧΙΑΚΗ ΕΡΓΑΣΙΑ
@@ -880710,15 +880599,15 @@
     26: null
     27: null
     28: null
     29: null
     30: null
 - dbase_number: 17549
   authors:
-  - ΒΑΓΙΑΚΑΚΟΥ,Β.
+  - ΒΑΓΙΑΚΑΚΟΣ,ΔΙΚΑΙΟΣ,Β.
   language: el
   title: ΣΥΜΒΟΛΗ ΕΙΣ ΤΗΝ ΜΕΛΕΤΗΝ ΤΩΝ ΝΑΥΤΙΚΩΝ ΕΜΠΟΡΙΚΩΝ ΚΑΙ ΟΙΚΟΝΟΜΙΚ
   subtitle: ΩΝ ΟΡΩΝ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΧΩΡΟΥ
   dewey: 380.509 ΒΑΓ
   entry_numbers:
   - '22945'
   editor: None // ΑΘΗΝΑ
@@ -881895,11 +881784,62 @@
     20: null
     21: null
     22: null
     23: null
     24: null
     25: null
     26: null
+    27: null
+    28: null
+    29: null
+    30: null
+- dbase_number: 17573
+  authors:
+  - ΜΟΡΤΟΝ,ΚΕΙΤ
+  language: el
+  title: Η ΚΟΡΗ ΤΟΥ ΡΟΛΟΓΑ
+  dewey: 823 ΜΟΡ
+  entry_numbers:
+  - '23015'
+  translators:
+  - ΧΡΙΣΤ. ΣΑΚΕΛΛΑΡΟΠΟΥΛ
+  editor: ΛΙΒΑΝΗ // ΑΘΗΝΑ
+  edition_year: 2019
+  pages: 603
+  topics:
+  - ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  has_cd: false
+  has_dvd: false
+  offprint: false
+  ean: '9789601435077'
+  original_entry:
+    0: 17573
+    1: ΜΟΡΤΟΝ,ΚΕΙΤ
+    2: Η ΚΟΡΗ ΤΟΥ ΡΟΛΟΓΑ
+    4: 823ΜΟΡ
+    5: '23015'
+    6: ΧΡΙΣΤ. ΣΑΚΕΛΛΑΡΟΠΟΥΛ
+    8: ΛΙΒΑΝΗΣ
+    9: ΑΘΗΝΑ
+    10: '2019'
+    11: '603'
+    12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+    13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+    14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+    18: '9789601435'
+    19: '077'
+    3: null
+    7: null
+    15: null
+    16: null
+    17: null
+    20: null
+    21: null
+    22: null
+    23: null
+    24: null
+    25: null
+    26: null
     27: null
     28: null
     29: null
     30: null
```

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/editor_corrections.yml` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/editor_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/entries.yml` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/entries.yml`

 * *Files 0% similar despite different names*

```diff
@@ -507,16 +507,16 @@
   12: ΓΑΛΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΓΑΛΛΙΚΟ ΘΕΑΤΡΟ-ΚΩΜΩΔΙΑ
   14: ΚΩΜΩΔΙΑ-ΟΙ ΧΑΛΚΟΓΡΑΦΟΙ
 - 0: 38
   1: ΑΠΕΡΓΗΣ,ΠΑΝΤΕΛΗΣ
   2: ΤΡΙΑ ΠΡΟΣΩΠΑ
   3: ΕΙΣΑΓΩΓΗ ΣΤΗΝ ΕΠΟΧΗ ΚΑΙ ΤΟ ΕΡΓΟ ΤΟΥΣ
-  4: 880.3 ΑΠΕ
-  5: 1004-2688
+  4: 880.3ΑΠΕ
+  5: '9274'
   8: ΙΩΛΚΟΣ
   9: ΑΘΗΝΑ
   10: '1980'
   11: 88Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΡΟΙΔΗΣ,ΕΜΜΑΝΟΥΗΛ
   14: ΚΑΒΑΦΗΣ,Κ.Π
@@ -823,15 +823,14 @@
   15: ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΑΙΣΘΗΤΙΚΗ
   22: ΑΙΣΘΗΤΙΚΗ
 - 0: 60
   1: ΒΑΒΑΡΕΤΟΣ,ΓΕΩΡΓΙΟΣ
   2: Η ΣΥΜΒΟΛΗ ΤΗΣ ΗΠΕΙΡΟΥ ΕΙΣ ΤΟΥΣ ΑΓΩΝΑΣ ΥΠΕΡ ΤΗΣ ΕΛΕΥΘΕΡΙΑΣ
   4: 938.5ΒΑΒ
   5: 2167-2168-2046-2047
-  6: 2048-9258
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1963'
   11: 31Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΣΥΜΒΟΛΗ ΣΤΗΝ ΕΛΕΥΘΕΡΙΑ
   13: ΗΠΕΙΡΟΣ-ΑΓΩΝΕΣ ΕΛΕΥΘΕΡΙΑΣ
   14: ΑΓΩΝΕΣ ΕΛΕΥΘΕΡΙΑΣ
@@ -2197,27 +2196,14 @@
   9: ΠΑΤΡΑ
   10: '1985'
   11: 47Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΚΥΠΡΟΣ
   13: ΤΑΞΙΔΙΑ-ΚΥΠΡΟΣ
   14: ΚΥΠΡΟΣ-ΤΑΞΙΔΙΑ
 - 0: 162
-  1: ΓΑΡΔΙΚΑΣ,ΓΕΩΡΓΙΟΣ Κ
-  2: ΙΦΙΓΕΝΕΙΑ Η ΕΝ ΑΥΛΙΔΙ
-  4: 881.24ΕΥΡ
-  5: 1455-2664
-  8: Χ.Ε
-  9: ΑΘΗΝΑ
-  10: '1962'
-  11: 215Σ
-  12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ-ΑΡΧΑΙΟ
-  13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΑΡΧΑΙΟ-ΕΥΡΙΠΙΔΗΣ
-  14: ΕΥΡΙΠΙΔΗΣ-ΙΦΙΓΕΝΕΙΑ Η ΕΝ ΑΥΛΙΔΙ
-  15: ΙΦΙΓΕΝΕΙΑ Η ΕΝ ΑΥΛΙΔΙ
-  17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 163
   1: ΓΑΡΟΥΦΑΛΙΑΣ,ΔΗΜΗΤΡΙΟΣ ΕΥΑΓΓ
   2: ΚΕΙΜΕΝΑ ΚΑΙ ΑΝΑΜΝΗΣΕΙΣ ΑΠΟ ΤΟΝ ΤΡΑΓΙΚΟ ΔΕΚΕΜΒΡΙΟ 1944
   4: 938.771ΓΑΡ
   5: '2371'
   8: Χ.Ε
   9: ΑΘΗΝΑ
@@ -3198,29 +3184,29 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΣΥΓΓΡΑΦΕΙΣ
   14: ΣΥΓΓΡΑΦΕΙΣ-ΠΑΛΑΜΑΣ
   15: ΠΑΛΑΜΑΣ
 - 0: 238
   1: ΔΗΜΗΤΡΑΚΟΣ,ΔΗΜ
   2: Η ΕΥΡΩΠΗ
-  4: 914 ΔΗΜ
+  4: 914ΔΗΜ
   5: '386'
   8: ΔΗΜΗΤΡΑΚΟΥ
   9: ΑΘΗΝΑ
   10: '1931'
   11: 310Σ
   12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΕΥΡΩΠΗ
   13: ΕΥΡΩΠΗ-ΤΑΞΙΔΙΑ
   14: ΤΑΞΙΔΙΑ-ΕΥΡΩΠΗ
 - 0: 239
   1: ΔΗΜΙΤΣΑ,ΜΑΡΓΑΡΙΤΑ
   2: ΒΙΟΓΡΑΦΙΑ ΟΛΥΜΠΙΑΔΟΣ ΤΗΣ ΗΠΕΙΡΩΤΙΔΟΣ ΝΕΟΠΤΟΛΕΜΟΥ ΤΟΥ ΑΛΚΕΤΟΥ
   3: ΘΥΓΑΤΡΟΣ ΝΟΜΙΜΟΥ ΤΟΥ ΦΙΛΙΠΠΟΥ Β'ΓΥΝΑΙΚΟΣ ΚΑΙ ΑΛΕΞΑΝ.ΜΗΤΡΟΣ
-  4: 938.17 ΔΗΜ
-  5: 1947-2357
+  4: 938.17ΔΗΜ
+  5: '1947'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1887'
   11: 136Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
   13: ΜΑΚΕΔΟΝΙΚΗ ΚΥΡΙΑΡΧΙΑ-ΟΛΥΜΠΙΑΔΑ
   14: ΟΛΥΜΠΙΑΔΑ-ΒΙΟΓΡΑΦΙΑ
@@ -3230,15 +3216,15 @@
   24: ΝΟΜΙΜΟΥ
   25: ΑΛΕΞΑΝΔΡΟΥ
   26: ΜΕΓΑΛΟΥ
 - 0: 240
   1: ΔΗΜΟΠΟΥΛΟΣ,ΕΥΑΓ
   2: Η ΕΛΛΗΝΙΚΗ ΨΥΧΗ
   3: ΤΡΙΠΡΑΚΤΟΝ ΕΡΓΟΝ
-  4: 886.2 ΔΗΜ
+  4: 886.2ΔΗΜ
   5: '1463'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1949'
   11: 30Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΙΣΤΟΡΙΚΟ ΕΡΓΟ
@@ -3530,26 +3516,14 @@
   9: ΑΘΗΝΑ
   10: '1988'
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΣΥΓΓΡΑΦΕΙΣ
   13: ΣΥΓΓΡΑΦΕΙΣ-ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ
   14: ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ
   15: ΠΑΠΑΙΩΑΝΝΟΥ-ΔΙΑΜΑΝΤΗ
 - 0: 263
-  1: ΔΙΑΜΑΝΤΗ-ΠΑΠΑΙΩΑΝΝΟΥ,ΤΖΕΝΗ
-  2: ΠΟΡΕΙΑ ΣΤΗ ΜΕΓΑΛΗ ΕΛΛΑΔΑ
-  4: 914.95 ΔΙΑ
-  5: '391'
-  8: Χ.Ε
-  9: ΑΘΗΝΑ
-  10: '1969'
-  11: 172Σ
-  12: ΓΕΩΓΡΑΦΙΑ-ΤΑΞΙΔΙΑ-ΕΛΛΑΔΑ
-  13: ΕΛΛΑΔΑ-ΤΑΞΙΔΙΑ
-  14: ΣΙΚΕΛΙΑ-ΤΑΞΙΔΙΑ
-  15: ΤΑΞΙΔΙΔΙΑ-ΕΛΛΑΔΑ-ΣΙΚΕΛΙΑ
 - 0: 264
   1: ΔΙΖΙΚΙΡΙΚΗΣ,ΓΙΩΡΓΟΣ
   2: ΛΕΞΙΚΟ ΤΟΥ ΚΙΝΗΜΑΤΟΓΡΑΦΟΥ
   3: ΑΙΣΘΗΤΙΚΩΝ ΚΑΙΤΕΧΝΙΚΩΝ ΟΡΩΝ
   4: 880.203ΔΙΖ
   5: '1600'
   8: ΑΙΓΟΚΕΡΩΣ
@@ -4174,15 +4148,15 @@
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΑΡΧΑΙΟ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΑΡΧΑΙΟ
   15: ΕΥΡΙΠΙΔΗΣ
 - 0: 312
   1: ΕΥΡΙΠΙΔΗΣ
   2: ΙΦΙΓΕΝΕΙΑ Η ΕΝ ΑΥΛΙΔΙ
   4: 881.24ΕΥΡ
-  5: '2664'
+  5: 2664-1455
   6: ΓΑΡΔΙΚΑΣ,ΓΕΩΡΓΙΟΣ Κ
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1962'
   11: 215Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ-ΑΡΧΑΙΟ
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΑΡΧΑΙΟ
@@ -5967,15 +5941,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΤΑ-ΠΡΟΣΩΠΙΚΟΤΗΤΕΣ
   13: ΑΡΤΑ-ΠΡΟΣΩΠΙΚΟΤΗΤΕΣ
   14: ΠΡΟΣΩΠΙΚΟΤΗΤΕΣ-ΓΑΡΟΥΦΑΛΙΑΣ Ε
   15: ΓΑΡΟΥΦΑΛΙΑΣ ΕΥΑΓΓΕΛΟΣ
 - 0: 450
   1: ΚΑΡΑΤΖΕΝΗΣ,ΔΗΜΗΤΡΙΟΣ ΦΩΤΙΟΣ
   2: ΕΠΑΝΑΣΤΑΣΙΣ ΚΑΙ ΚΑΤΑΣΤΡΟΦΗ ΚΑΛΑΡΥΤΩΝ-ΣΥΡΡΑΚΟΥ
-  4: 938.5 ΚΑΡ
+  4: 938.5ΚΑΡ
   5: '2054'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1988'
   11: 102Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΙΩΑΝΝΙΝΑ-ΚΑΛΑΡΡΥΤΕΣ-ΣΥΡΡΑΚΟ
   13: ΙΩΑΝΝΙΝΑ-ΚΑΛΑΡΡΥΤΕΣ-ΣΥΡΡΑΚΟ
@@ -6207,15 +6181,15 @@
   14: ΔΙΗΓΗΜΑ
   15: ΣΥΓΓΡΑΦΕΙΣ-ΚΑΡΚΑΒΙΤΣΑΣ
 - 0: 468
   1: ΚΑΡΟΛΙΔΟΥ,Π
   2: ΣΥΓΧΡΟΝΟΣ ΙΣΤΟΡΙΑ ΤΩΝ ΕΛΛΗΝΩΝ ΚΑΙ ΤΩΝ ΛΟΙΠΩΝ ΛΑΩΝ ΤΗΣ ΑΝΑΤΟΛ
   3: ΑΠΟ 1821 ΜΕΧΡΙ 1921
   4: 938.5 ΚΑΡ
-  5: 2057-2058-1750-2056
+  5: 2057-1750-2056
   8: ΒΙΤΣΙΚΟΥΝΑΚΗ
   9: ΑΘΗΝΑ
   10: '1929'
   11: 488Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-(1821-1921)
   13: 1821-ΕΛΛΑΔΑ
   14: ΑΝΑΤΟΛΗ-ΛΑΟΙ-1821
@@ -6444,28 +6418,28 @@
   11: 124Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΝΕΟΕΛΛΗΝΙΚΑ ΚΕΙΜΕΜΕΝΑ
   13: ΝΕΟΕΛΛΗΝΙΚΑ ΚΕΙΜΕΝΑ
   14: ΚΕΙΜΕΝΑ-ΝΕΟΕΛΛΗΝΙΚΑ
 - 0: 487
   1: ΚΑΤΩΠΟΔΗΣ,ΓΕΡΑΣΙΜΟΣ Σ
   2: ΑΙΤΩΛΙΚΗ ΣΥΜΠΟΛΙΤΕΙΑ
-  4: 938.22 ΚΑΤ
-  5: 2322-2291
+  4: 938.22ΚΑΤ
+  5: '2322'
   8: ΓΡΑΜΜΗ
   9: ΑΘΗΝΑ
   10: '1977'
   11: 457Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΙΤΩΛΙΑ
   13: ΑΙΤΩΛΙΑ
   14: ΑΙΤΩΛΙΚΗ ΣΥΜΠΟΛΙΤΕΙΑ
 - 0: 488
   1: ΚΑΨΙΩΤΗΣ,ΑΘΑΝΑΣΙΟΣ  Η.
   2: ΘΕΣΣΑΛΟΙ ΟΙ ΠΡΩΤΟΙ ΑΥΤΟΧΘΟΝΕΣ ΕΛΛΗΝΕΣ
   3: ΚΑΙ ΠΡΩΤΟΙ ΑΠΟΙΚΟΙ ΝΗΣΙΩΝ ΤΟΥ ΑΙΓΑΙΟΥ ΚΑΙ ΤΩΝ ΜΙΚΡΑΣΙΑΤΚΩΝ Α
-  4: 938.21 ΚΑΨ
+  4: 938.21ΚΑΨ
   5: '2560'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1979'
   11: 198Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΕΣΣΑΛΙΑ
   13: ΘΕΣΣΑΛΙΑ-ΘΕΣΣΑΛΟΙ
@@ -7838,27 +7812,27 @@
   13: ΗΠΕΙΡΟΣ-ΑΡΤΑ-ΣΚΙΑΔΑΔΕΣ
   14: ΑΡΤΑ-ΣΚΙΑΔΑΔΕΣ
   15: ΣΚΙΑΔΑΔΕΣ
 - 0: 594
   1: ΛΑΜΠΡΙΔΗΣ,ΙΩΑΝΝΗΣ
   2: ΗΠΕΙΡΩΤΙΚΑ ΑΓΑΘΟΕΡΓΗΜΑΤΑ ΚΑΙ ΑΛΛΑ ΔΗΜΟΣΙΕΥΜΑΤΑ
   4: 938.5 ΛΑΜ
-  5: 2053-2054
+  5: '2053'
   8: Χ.Ε
   9: ΙΩΑΝΝΙΝΑ
   10: '1971'
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΔΗΜΟΣΙΕΥΜΑΤΑ
   14: ΔΗΜΟΣΙΕΥΜΑΤΑ
   15: ΑΓΑΘΟΕΡΓΗΜΑΤΑ
 - 0: 595
   1: ΛΑΜΠΡΙΔΗΣ,ΙΩΑΝΝΗΣ
   2: ΗΠΕΙΡΩΤΙΚΑ ΜΕΛΕΤΗΜΑΤΑ
   4: 938.501ΛΑΜ
-  5: 2052-2357-
+  5: 2052-2357
   8: ΕΤΑΙΡ.ΗΠΕΙΡ.ΜΕΛΕΤΩΝ
   9: ΙΩΑΝΝΙΝΑ
   10: '1971'
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΜΕΛΕΤΗΜΑΤΑ
   14: ΜΕΛΕΤΗΜΑΤΑ-ΗΠΕΙΡΟΣ
   15: ΗΠΕΙΡΩΤΙΚΑ ΜΕΛΕΤΗΜΑΤΑ
@@ -8480,15 +8454,15 @@
   14: ΦΙΛΕΚΠΑΙΔΕΥΤΙΚΗ ΕΤΑΙΡΕΙΑ
   21: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ ΑΘΗΝΩΝ;31
 - 0: 643
   1: ΜΑΜΜΟΠΟΥΛΟΣ,ΑΛΕΞΑΝΔΡΟΣ Χ.
   2: ΗΠΕΙΡΟΣ ΚΑΙ ΛΑΚΩΝΙΑ ΑΠΟ ΤΗΝ ΣΠΛΑΝΤΖΑ
   3: ΕΩΣ ΤΟΝ ΑΥΤΟΝΟΜΙΑΚΟΝ ΑΓΩΝΑ 1914
   4: 938.68ΜΑΜ
-  5: 2042-2043-9250Α
+  5: 2042-2043-09250
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1968'
   11: 38Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΛΑΚΩΝΙΑ
   14: ΛΑΚΩΝΙΑ-ΗΠΕΙΡΟΣ
@@ -8557,15 +8531,15 @@
   13: ΗΠΕΙΡΟΣ-ΑΝΘΟΛΟΓΙΑ
   14: ΑΝΘΟΛΟΓΙΑ-ΗΠΕΙΡΟΣ
 - 0: 649
   1: ΜΑΝΟΥΚΑΣ,ΓΕΩΡΓΙΟΣ Χ
   2: ΠΑΙΔΟΜΑΖΩΜΑ
   3: ΤΟ ΜΕΓΑΛΟ ΕΓΚΛΗΜΑ ΚΑΤΑ ΤΗΣ ΦΥΛΗΣ
   4: 938.413ΜΑΝ
-  5: 1823-8509-9274
+  5: 8509-9274
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1961'
   11: 254Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΑΙΔΟΜΑΖΩΜΑ
   13: ΠΑΙΔΟΜΑΖΩΜΑ
   14: ΠΑΙΔΙ-ΠΑΙΔΟΜΑΖΩΜΑ
@@ -8584,15 +8558,15 @@
   13: ΤΟΥΡΚΟΚΡΑΤΙΑ-ΚΡΗΤΗ
   14: ΚΡΗΤΗ-ΣΥΝΩΜΟΣΙΕΣ
   15: ΣΥΝΩΜΟΣΙΕΣ-ΚΡΗΤΗ
 - 0: 651
   1: ΜΑΡΑΖΙΩΤΗΣ,ΓΕΩΡΓΙΟΣ
   2: Ο ΗΠΕΙΡΩΤΗΣ ΕΘΝΑΠΟΣΤΟΛΟΣ ΠΕΤΡΟΣ ΗΠΙΤΗΣ
   4: 938.5ΜΑΡ
-  5: 2061-2760-9258
+  5: 2061-2760
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1973'
   11: 50Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ-ΕΘΝΑΠΟΣΤΟΛΟΣ
   13: ΗΠΕΙΡΟΣ-ΗΠΙΤΗΣ
   14: ΗΠΙΤΗΣ-ΕΘΝΑΠΟΣΤΟΛΟΣ
@@ -9009,15 +8983,15 @@
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΤΡΑΓΩΔΙΑ
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΤΡΑΓΩΔΙΑ
   15: ΤΡΑΓΩΔΙΑ-ΕΡΓΟ
 - 0: 685
   1: ΜΗΤΣΟΤΑΚΗΣ,ΚΥΡΙΑΚΟΣ
   2: ΠΡΟΣΩΠΑ ΚΑΙ ΤΟΠΟΙ
   4: 889.21ΜΗΤ
-  5: '2533'
+  5: '2048'
   8: ΑΙΓΑΓΡΟΣ
   9: ΑΘΗΝΑ
   10: '1966'
   11: 116Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
   13: ΠΡΟΣΩΠΑ-ΕΛΛΑΔΑ
   14: ΤΟΠΟΙ-ΕΛΛΑΔΑ
@@ -9255,15 +9229,15 @@
   12: ΚΙΝΕΖΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΘΕΑΤΡΟ
   13: ΚΙΝΕΖΙΚΟ ΘΕΑΤΡΟ-ΙΣΤΟΡΙΑ
   14: ΚΙΝΑ-ΘΕΑΤΡΟ
 - 0: 705
   1: MURAT,JOHN
   2: ΤΟ ΜΕΓΑΛΥΤΕΡΟ ΕΓΚΛΗΜΑ ΤΟΥ ΑΙΩΝΑ
   3: ΤΟ ΞΕΚΛΗΡΙΣΜΑ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
-  4: 938.ΟΟ1MUR
+  4: 938.001MUR
   5: 2082-1950
   8: Χ.Ε
   9: Χ.Τ
   10: '1982'
   11: 542Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΣΜΟΣ
   13: ΕΛΛΗΝΙΣΜΟΣ-ΞΕΚΛΗΡΙΣΜΑ
@@ -9712,15 +9686,15 @@
   11: 165Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
   13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ
 - 0: 742
   1: ΜΥΡΙΒΗΛΗΣ,ΣΤΡΑΤΗΣ
   2: ΤΟ ΚΟΚΚΙΝΟ ΒΙΒΛΙΟ
   4: 889.34ΜΥΡ
-  5: 1185-9143Α
+  5: 1185-09143
   7: 3ΕΚΔ
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: '1956'
   11: 186Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
   13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ
@@ -9848,15 +9822,15 @@
   11: 30Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
   13: ΚΥΠΡΟΣ-ΙΣΤΟΡΙΑ
 - 0: 753
   1: ΚΙΤΣΟΣ,ΑΘΑΝΑΣΙΟΣ
   2: ΘΕΣΠΡΩΤΙΚΗ ΓΗ
   4: 938.937ΚΙΤ
-  5: 2763-2790-9253Α
+  5: 2763-2790-09253
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1977'
   11: 37Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΘΕΣΠΡΩΤΙΑ
   13: ΘΕΣΠΡΩΤΙΑ-ΙΣΤΟΡΙΑ
   17: 3 ΑΝΤΙΤΥΠΑ
@@ -9951,16 +9925,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ
   13: ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ-ΦΡΑΓΚΟΙ
   14: ΦΡΑΓΚΟΙ-ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ
 - 0: 761
   1: ΜΠΟΤΣΑΡΗΣ,ΔΗΜ Τ ΝΟΤΗ
   2: ΑΓΩΝΕΣ ΕΛΕΥΘΕΡΙΑΣ
   4: 938.526ΜΠΟ
-  5: 2769-9260Α
-  6: '     -'
+  5: 2769-09260
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1973'
   11: 76Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΣΟΥΛΙ
   14: ΣΟΥΛΙ-ΑΓΩΝΕΣ
@@ -10980,29 +10953,27 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
   13: ΚΥΠΡΟΣ-ΙΣΤΟΡΙΑ
   14: ΚΥΠΡΙΑΚΟ ΖΗΤΗΜΑ
 - 0: 843
   1: ΠΑΠΑΓΕΩΡΓΙΟΥ,ΣΠΥΡΟΣ
   2: ΤΑ ΚΡΙΣΙΜΑ  ΝΤΟΚΟΥΜΕΝΤΑ ΤΟΥ ΚΥΠΡΙΑΚΟΥ
   4: 938.497ΠΑΠ
-  5: 2397-2398-2399-2857-
-  6: 2852-2853-2854
+  5: 2394-2395-2396-2397
   8: ΛΑΔΙΑ
   9: ΑΘΗΝΑ
   10: '1983'
   11: 378Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
   13: ΚΥΠΡΟΣ-ΚΥΠΡΙΑΚΟ
   14: ΝΤΟΚΟΥΜΕΝΤΑ-ΚΥΠΡΙΑΚΟ
 - 0: 844
   1: ΠΑΠΑΓΕΩΡΓΙΟΥ,ΣΠΥΡΟΣ
   2: ΑΠΟ ΤΗΝ ΖΥΡΙΧΗΝ ΕΙΣ ΤΟΝ ΑΤΤΙΛΑΝ
   4: 938.497ΠΑΠ
-  5: 2394-2395-2396-2855-
-  6: 2856-2857-5201-5200
+  5: 2854-2855-2856-2857
   8: ΛΑΔΙΑ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 350Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΚΥΠΡΟΣ
   13: ΚΥΠΡΟΣ-ΦΑΚΕΛΛΟΣ
   14: ΑΤΤΙΛΑΣ-ΚΥΠΡΟΣ
@@ -11431,15 +11402,15 @@
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΚΩΜΩΔΙΑ
   15: ΚΩΜΩΔΙΑ-ΘΕΑΤΡΙΚΟ ΕΡΓΟ
 - 0: 878
   1: ΠΑΠΑΘΑΝΑΣΙΟΥ,ΖΗΣΗΣ
   2: ΣΠΥΡΟΣ ΧΑΣΙΩΤΗΣ
   3: Ο ΗΠΕΙΡΩΤΗΣ ΠΑΤΗΡ ΤΗΣ ΓΕΩΡΓΙΑΣ
   4: 938.629ΠΑΠ
-  5: 2028-2029Α
+  5: 2028-2029
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1969'
   11: 27Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΧΑΣΙΩΤΗΣ
   14: ΧΑΣΙΩΤΗΣ-ΗΠΕΙΡΩΤΗΣ
@@ -11893,28 +11864,28 @@
   13: ΑΡΘΡΑ-1971
   14: 1971-ΑΡΘΡΑ
 - 0: 914
   1: ΠΕΡΑΝΘΗΣ,ΜΙΧΑΗΛ
   2: ΛΟΡΕΤΖΟΣ ΜΑΒΙΛΗΣ
   3: Ο ΗΡΩΣ ΤΟΥ ΔΡΙΣΚΟΥ
   4: 938.654ΠΕΡ
-  5: 2036-2037-9267Α
+  5: 2036-2037-09267
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1969'
   11: 23Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΒΙΛΗΣ
   13: ΜΑΒΙΛΗΣ-ΔΡΙΣΚΟ
   14: ΔΡΙΣΚΟ-ΜΑΒΙΛΗΣ
 - 0: 915
   1: ΠΕΡΑΝΘΗΣ,ΜΙΧ
   2: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ
   3: 1453 ΕΩΣ ΣΗΜΕΡΑ
   4: 880.08ΠΕΡ
-  5: 205-206-207-208-209-
+  5: 205-206-207-208-209
   8: Χ.Ε
   9: Χ.Τ
   10: Χ.Χ
   11: 607Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
   13: ΕΛΛΗΝΙΚΗ ΠΕΖΟΓΡΑΦΙΑ-ΙΣΤΟΡΙΑ
   14: ΠΕΖΟΓΡΑΦΙΑ-ΙΣΤΟΡΙΑ
@@ -12034,15 +12005,15 @@
   14: ΑΘΟΛΟΓΙΑ-ΠΟΙΗΣΗ
   15: ΠΟΙΗΣΗ
 - 0: 925
   1: ΠΕΡΑΝΘΗΣ,ΜΙΧ
   2: ΑΜΒΡΑΚΙΑ
   3: ΧΡΟΝΟΓΡΑΦΙΑ ΜΙΑΣ ΠΡΩΤΕΥΟΥΣΑΣ
   4: 938.21ΠΕΡ
-  5: 2187-2273-13268
+  5: 2187-13268
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1954'
   11: 212Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΜΒΡΑΚΙΑ
   13: ΑΜΒΡΑΚΙΑ-ΧΡΟΝΟΓΡΑΦΙΑ
   14: ΧΡΟΝΟΓΡΑΦΙΑ
@@ -13886,15 +13857,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΧΡΟΝΟΓΡΑΦΗΜΑΤΑ
   14: ΧΡΟΝΟΓΡΑΦΗΜΑΤΑ-ΗΠΕΙΡΟΣ
 - 0: 1070
   1: ΣΑΚΚΑΣ,ΓΕΩΡΓΙΟΣ
   2: Η ΙΣΤΟΡΙΑ ΤΩΝ ΕΛΛΗΝΩΝ ΤΗΣ ΤΡΙΠΟΛΕΩΣ ΤΟΥ ΠΟΝΤΟΥ
   4: 938.498ΣΑΚ
-  5: 2123-9277Α
+  5: 2123-09277
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1957'
   11: 254Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΤΡΙΠΟΛΗ-ΠΟΝΤΟΣ
   13: ΤΡΙΠΟΛΗ-ΠΟΝΤΟΣ
   14: ΠΟΝΤΟΣ-ΤΡΙΠΟΛΗ
@@ -13959,26 +13930,26 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΙΩΑΝΝΙΝΑ
   13: ΙΩΑΝΝΙΝΑ-ΖΑΓΟΡΙ
   14: ΖΑΓΟΡΙ-ΙΩΑΝΝΙΝΑ
 - 0: 1076
   1: ΣΑΡΑΝΤΗΣ,ΘΕΟΔΩΡΟΣ Κ.Π.
   2: Ο ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ ΑΠΟ ΤΗΝ ΙΣΤΟΡΙΑ ΕΩΣ ΤΟΝ ΘΡΥΛΟ
   4: 938.174ΣΑΡ
-  5: 2197-2198-
+  5: 2197-2198
   8: Χ.Ρ
   9: ΑΘΗΝΑ
   10: '1970'
   11: 396Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΡΟΣ
   13: ΜΕΓΑΣ ΑΛΕΞΑΝΡΟΣ
 - 0: 1077
   1: ΣΑΡΑΝΤΗΣ,ΘΕΟΔΩΡΟΥ Κ.
   2: ΤΟ ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟ ΖΗΤΗΜΑ ΚΑΙ Ο ΝΑΠΟΛΕΩΝ
   4: 938.694ΣΑΡ
-  5: 2778-2868-9273Α
+  5: 2778-2868-09273
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1985'
   11: 22Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟ ΖΗΤΗΜΑ
   13: ΒΟΡΕΙΟΗΠΕΙΡΩΤΙΚΟ ΖΗΤΗΜΑ
   14: Β.ΗΠΕΙΡΟΣ-ΖΗΤΗΜΑ
@@ -14404,15 +14375,15 @@
   13: ΣΥΓΓΡΑΦΕΙΣ-ΠΑΛΑΜΑΣ
   14: ΠΑΛΑΜΑΣ-ΠΑΡΑΔΟΣΗ
   15: ΠΑΡΑΔΟΣΗ-ΕΛΛΗΝΙΚΗ
 - 0: 1112
   1: ΣΙΩΜΟΠΟΥΛΟΣ,ΔΗΜ Β.
   2: ΗΠΕΙΡΩΤΙΚΑ
   4: 938.21ΣΙΩ
-  5: 2188-2520-2578
+  5: '2520'
   8: Χ.Ε
   9: ΙΩΑΝΝΙΝΑ
   10: '1975'
   11: 245Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΗΠΕΙΡΩΤΙΚΑ
   14: ΗΠΕΙΡΩΤΙΚΑ
@@ -14543,15 +14514,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
   13: ΕΛΛΗΝΙΚΟ ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΙΣΤΟΡΙΑ
   14: ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΙΣΤΟΡΙΑ
 - 0: 1123
   1: ΣΟΛΔΑΤΟΣ,ΓΙΑΝΝΗΣ
   2: ΙΣΤΟΡΙΑ ΤΟΥ ΕΛΛΗΝΙΚΟΥ ΚΙΝΗΜΑΤΟΓΡΑΦΟΥ
   4: 880.203ΣΟΛ
-  5: 2435-2434-2437-2436-
+  5: 2434-2435-2436-2437
   7: 5ΕΚΔ
   8: ΑΙΓΟΚΕΡΩΣ
   9: ΑΘΗΝΑ
   10: '1989'
   11: 254Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
   13: ΕΛΛΗΝΙΚΟΣ ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΙΣΤΟΡΙΑ
@@ -15188,15 +15159,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΣΥΝΟΡΑ
   14: ΣΥΝΟΡΑ-ΗΠΕΙΡΟΣ
 - 0: 1174
   1: ΣΤΕΡΓΙΟΠΟΥΛΟΣ,Κ.Δ
   2: Η ΑΡΧΑΙΑ ΑΙΤΩΛΙΑ
   4: 938.22ΣΤΕ
-  5: 2215-2587
+  5: '2587'
   8: ΔΗΜΗΤΡΑΚΟΥ
   9: ΑΘΗΝΑ
   10: '1939'
   11: 191Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΑΡΧΑΙΑ
   13: ΑΡΧΑΙΑ ΙΣΤΟΡΙΑ-ΑΙΤΩΛΙΑ
   14: ΑΙΤΩΛΙΑ-ΑΡΧΑΙΑ
@@ -15569,15 +15540,15 @@
   13: ΕΛΛΗΝΙΚΟ ΘΕΑΤΡΟ-ΜΟΝΟΠΡΑΚΤΟ
   14: ΜΟΝΟΠΡΑΚΤΟ-ΕΡΓΟ
   15: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΜΟΝΟΠΡΑΚΤΟ
 - 0: 1204
   1: ΤΑΡΝΑΝΑΣ,ΑΝΤΡΕΑΣ
   2: ΓΟΥΝΤΥ ΑΛΛΕΝ
   4: 800.203ΤΑΡ
-  5: '1625'
+  5: '5393'
   8: ΑΙΓΟΚΕΡΩΣ
   9: ΑΘΗΝΑ
   10: '1984'
   11: 82Σ
   12: ΠΑΓΚΟΣΜΙΟΣ ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΑΡΧΕΙΟ
   13: ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΑΡΧΕΙΟ
   14: ΑΡΧΕΙΟ-ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
@@ -15636,15 +15607,15 @@
   15: ΑΓΡΟΤΙΚΟ ΚΙΝΗΜΑ-ΚΟΜΠΟΤΙ
   17: 3 ΑΝΤΙΤΥΠΑ
 - 0: 1209
   1: ΤΑΤΣΙΟΠΟΥΛΟΣ,ΛΑΜΠΡΟΣ ΑΠ
   2: ΝΙΚΟΛΑΟΣ ΣΚΟΥΦΑΣ
   3: Ο ΕΘΝΕΓΕΡΤΗΣ ΑΡΧΗΓΟΣ ΤΗΣ ΦΙΛΙΚΗΣ ΕΤΑΙΡΕΙΑΣ
   4: 938.487ΤΑΤ
-  5: 2256-1034-1661-1482.
+  5: 2256-1034-1661-1482
   8: Χ.Ε
   9: ΙΩΑΝΝΙΝΑ
   10: '1980'
   11: 73Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΣΚΟΥΦΑΣ
   13: ΣΚΟΥΦΑΣ-ΦΙΛΙΚΗ ΕΤΑΙΡΕΙΑ
   14: ΦΙΛΙΚΗ ΕΤΑΙΡΕΙΑ-ΣΚΟΥΦΑΣ
@@ -16168,15 +16139,15 @@
   13: ΠΑΡΑΔΟΣΗ-1821
   14: 1821-ΠΑΡΑΔΟΣΗ
 - 0: 1251
   1: ΛΑΜΠΡΙΔΗΣ,ΣΤΑΘΗΣ Δ.
   2: ΧΡΙΣΤΟΔΟΥΛΟΣ ΚΛΟΝΑΡΗΣ,ΖΑΓΟΡΙΤΗΣ Ο ΠΡΩΤΟΣ ΠΡΟΕΔΡΟΣ
   3: ΤΟΥ ΑΡΕΙΟΥ ΠΑΓΟΥ
   4: 938.503ΛΑΜ
-  5: 2793-9259Α
+  5: 2793-09259
   8: ΗΠΕΙΡΩΤΙΚΗ ΕΤΑΙΡΕΙΑ
   9: ΑΘΗΝΑ
   10: '1975'
   11: 43Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΩΣΟΠΑ
   13: ΚΛΟΝΑΡΗΣ-ΑΡΕΙΟΣ ΠΑΓΟΣ
   14: ΑΡΕΙΟΣ ΠΑΓΟΣ-ΚΛΟΝΑΡΗΣ
@@ -16259,15 +16230,15 @@
   13: ΑΜΕΡΙΚΗ-ΕΠΟΠΟΙΙΑ
   14: ΕΠΟΠΟΙΙΑ-ΑΜΕΡΙΚΗ
 - 0: 1258
   1: ΤΣΑΚΑΣ,ΝΙΚΟΛΑΟΣ
   2: ΠΑΡΓΑ
   3: ΤΟΠΙΑ ΚΑΙ ΟΜΟΡΦΙΕΣ ΕΚΚΛΗΣΙΕΣ ΚΑΙ ΚΕΙΜΗΛΙΑ ΕΞΟΔΟΣ ΚΑΙ ΘΡΥΛΟΣ
   4: 938.938ΤΣΑ
-  5: 2737-3666-9264Α
+  5: 2737-3666-09264
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1966'
   11: 32Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΑΡΓΑ
   13: ΠΑΡΓΑ-ΙΣΤΟΡΙΑ
   14: ΗΠΕΙΡΟΣ-ΠΑΡΓΑ
@@ -16449,15 +16420,15 @@
   14: ΣΥΓΓΡΑΦΕΙΣ-ΣΕΦΕΡΗΣ
   15: ΣΕΦΕΡΗΣ
 - 0: 1273
   1: ΤΣΑΤΣΟΥ,ΙΩΑΝΝΑ
   2: Η ΠΟΙΗΣΗ ΚΑΙ Ο ΑΔΗΣ
   3: Ο RIERRE EMMANYEL KAI H ELLADA
   4: 889.09ΤΣΑ
-  5: 2611-1612
+  5: 2611-2612
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1987'
   11: 65Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΟΙΗΣΗ
   13: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΑΔΗΣ
 - 0: 1274
@@ -16823,16 +16794,15 @@
   11: 154Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΕΤΑΠΟΛΙΤΕΥΣΗ
   13: ΜΕΤΑΠΟΛΙΤΕΥΣΗ-ΕΛΛΑΔΑ
 - 0: 1304
   1: ΦΙΛΗΜΟΝΟΣ,ΙΩΑΝΝΗΣ
   2: ΔΟΚΙΜΙΟΝ ΙΣΤΟΡΙΚΟΝ ΠΕΡΙ ΤΗΣ ΕΛΛΗΝΙΚΗΣ ΕΠΑΝΑΣΤΑΣΕΩΣ
   4: 938.501ΦΙΛ
-  5: 1823-1824-1825-1826-
-  6: 1747-1746-1745-
+  5: 1823-1824-1825-1826
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1859'
   11: 416Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΑΝΑΣΤΑΣΗ
   13: ΕΠΑΝΑΣΤΑΣΗ-ΔΟΚΙΜΙΟ
   14: ΔΟΚΙΜΙΟ-ΕΠΑΝΑΣΤΑΣΗ
@@ -17146,15 +17116,15 @@
   14: ΓΑΛΛΙΑ-ΤΑΞΙΔΙΑ
   15: ΕΛΒΕΤΙΑ-ΤΑΞΙΔΙΑ
 - 0: 1330
   1: ΦΩΤΙΑΔΗΣ,ΕΥΑΓΓΕΛΟΣ Π.
   2: ΣΠΥΡΙΔΩΝ ΛΑΜΠΡΟΣ
   3: ΜΝΗΜΟΣΥΝΟΣ ΛΟΓΟΣ
   4: 938ΦΩΤ
-  5: 2023-2733-9254Α
+  5: 2023-2733-09254
   7: 2ΕΚΔ
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1967'
   11: 35Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
   13: ΛΑΜΠΡΟΣ-ΙΣΤΟΡΙΑ
@@ -17220,15 +17190,15 @@
   13: ΣΚΟΥΦΑΣ-ΦΙΛΙΚΗ ΕΤΑΙΡΕΙΑ
   14: ΦΙΛΙΚΗ ΕΤΑΙΡΕΙΑ-ΙΔΡΥΤΗΣ
   17: 3 ΑΝΤΙΤΥΠΑ
 - 0: 1336
   1: ΧΑΜΜΕΡ,Ι
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΟΘΩΜΑΝΙΚΗΣ ΑΥΤΟΚΡΑΤΟΡΙΑΣ
   4: 956.1ΧΑΜ
-  5: 2302-2303-2304-2305-
+  5: 2302-2303-2304-2305
   6: ΚΡ0ΚΙΔΑΣ,Κ
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1870'
   11: 385Σ
   12: ΟΘΩΜΑΝΙΚΗ ΑΥΤΟΚΡΑΤΟΡΙΑ-ΙΣΤΟΡΙΑ
   13: ΤΟΥΡΚΙΑ-ΟΘΩΜΑΝΙΚΗ ΙΣΤΟΡΙΑ
@@ -17582,15 +17552,15 @@
   14: ΗΠΕΙΡΟΣ-ΤΑΞΙΔΙΑ
   15: ΙΟΝΙΑ ΝΗΣΙΑ-ΤΑΞΙΔΙΑ
   17: ΞΕΝΟΙ ΠΕΡΙΗΓΗΤΕΣ ΣΤΟΝ ΕΛΛΗΝΙΚΟ ΧΩΡΟ 8
   30: HENRY HOLLAND
 - 0: 1365
   1: ΧΟΦΜΑΝ,ΦΡΕΝΤ
   2: ΤΟ ΣΥΓΧΡΟΝΟ ΑΜΕΡΙΚΑΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ(1900-1950)
-  4: 880.ΧΟΦ
+  4: 880.03ΧΟΦ
   5: '2655'
   8: ΑΕΤΟΣ
   9: ΑΘΗΝΑ
   10: '1954'
   11: 167Σ
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΑΜΕΡΙΚΑΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ-ΙΣΤΟΡΙΑ
@@ -17939,15 +17909,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΡΟΣΩΠΑ
   13: ΑΜΑΝΤΟΣ-ΜΝΗΜΗ
 - 0: 1393
   1: Χ.Σ
   2: Η ΕΚΣΤΡΑΤΕΙΑ ΕΙΣ ΤΗΝ ΜΙΚΡΑΝ ΑΣΙΑΝ(1919-1922)
   3: ΕΠΙΘΕΤΙΚΑΙ ΕΠΙΧΕΙΡΗΣΕΙΣ ΔΕΚΕΜΒΡΙΟΥ 1920 ΜΑΡΤΙΟΥ 1921
   4: 938.721Χ.Σ
-  5: 1793-1873-8192
+  5: 1793-1873
   8: ΓΕΝ.ΕΠΙΤ.ΣΤΡΑΤΟΥ
   9: ΑΘΗΝΑ
   10: '1963'
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΙΚΡΑ ΑΣΙΑ
   13: ΜΙΚΡΑ ΑΣΙΑ-ΕΚΣΤΡΑΤΕΙΑ
   14: 1919-ΜΙΚΡΑ ΑΣΙΑ
   15: ΓΕΝΙΚΟ ΕΠΙΤΕΛΕΙΟ ΣΤΡΑΤΟΥ
@@ -18157,15 +18127,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
   13: ΜΑΚΕΔΟΝΙΑ-ΠΑΥΛΟΣ ΜΕΛΑΣ
   14: ΜΕΛΑΣ-ΜΑΚΕΔΟΝΙΑ
 - 0: 1410
   1: Χ.Σ
   2: ΕΠΙΤΟΜΟΣ ΙΣΤΟΡΙΑ ΤΗΣ ΕΙΣ ΜΙΚΡΑΝ ΑΣΙΑΝ ΕΚΣΤΡΑΤΕΙΑΣ (1919-1922
   4: 938.721Χ.Σ
-  5: 1793-8192
+  5: '8192'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1967'
   11: 495Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΙΚΡΑ ΑΣΙΑ
   13: ΜΙΚΡΑ ΑΣΙΑ-1919
   14: 1919-ΜΙΚΡΑ ΑΣΙΑ
@@ -18278,15 +18248,15 @@
   11: 360Σ
   12: ΙΣΡΑΗΛΙΝΗ ΙΣΤΟΡΙΑ
   13: ΙΣΡΑΗΛ-ΙΣΤΟΡΙΑ
 - 0: 1420
   1: Χ.Σ
   2: Η ΚΑΤΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ ΕΠΙΒΟΛΗΣ
   4: 938.666Χ.Σ
-  5: '1237'
+  5: '2237'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1966'
   11: 369Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
   13: ΜΑΚΕΔΟΝΙΑ
 - 0: 1421
@@ -18449,15 +18419,15 @@
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΕΛΕΣΤΙΝΛΗΣ
   13: ΒΕΛΕΣΤΙΝΛΗΣ
   14: ΦΕΡΑΙΟΣ
 - 0: 1434
   1: Χ.Σ
   2: ΤΟ ΡΟΥΜΑΝΙΚΟ ΒΙΒΛΙΟ
   4: 949.8Χ.Σ
-  5: '2563'
+  5: '2562'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: Χ.Τ
   11: 133Σ
   12: ΡΟΥΜΑΝΙΚΗ ΙΣΤΟΡΙΑ
   13: ΡΟΥΜΑΝΙΑ-ΙΣΤΟΡΙΑ
 - 0: 1435
@@ -18864,15 +18834,15 @@
   13: ΠΑΓΚΟΣΜΙΟΣ ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΣΚΗΝΟΘΕΤΗΣ
   14: ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΣΚΗΝΟΘΕΤΗΣ
   15: ΧΙΟΥΣΤΟΝ-ΣΚΗΝΟΘΕΤΗΣ
 - 0: 1467
   1: Χ.Σ
   2: ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ 65
   4: 880.203ΚΙΝ
-  5: 1604-1605-
+  5: 1603-1604
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1965'
   11: 31Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
   13: ΕΛΛΗΝΙΚΟΣ ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΠΕΡΙΟΔΙΚΟ
   14: ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ-ΠΕΡΙΟΔΙΚΟ
@@ -19260,15 +19230,14 @@
   13: ΒΟΡΕΙΟΣ ΗΠΕΙΡΟΣ-ΚΑΘΟΔΟΣ
   14: ΕΘΝΙΚΟ ΧΡΕΟΣ-ΕΛΛΑΔΑ
 - 0: 1498
   1: ΚΟΥΚΟΥΛΕ,ΦΑΙΔΩΝΑΣ
   2: ΒΥΖΑΝΤΙΝΩΝ ΒΙΟΣ ΚΑΙ ΠΟΛΙΤΙΣΜΟΣ
   4: 938.303ΚΟΥ
   5: 2749-2750-2751-2752-
-  6: 2756-2753-2754-2755
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1948'
   11: 224Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΥΝΑΝΤΙΟ
   13: ΒΥΖΑΝΤΙΟ-ΠΟΛΙΤΙΣΜΟΣ
   14: ΠΟΛΙΤΙΣΜΟΣ-ΒΥΖΑΝΤΙΟ
@@ -19448,15 +19417,15 @@
   14: ΘΕΑΤΡΙΚΟ ΕΡΓΟ-ΚΩΜΩΔΙΑ
   15: ΚΩΜΩΔΙΑ-ΘΕΑΤΡΙΚΟ ΕΡΓΟ
 - 0: 1513
   1: ΣΚΟΠΑΣ,ΝΙΚ.Α-ΧΑΡΑΜΟΠΟΥΛΟΣ,Λ.Χ
   2: Ο ΑΓΩΝΑΣ ΤΩΝ 16 ΧΩΡΙΩΝ ΤΗΣ ΕΠΑΡΧΙΑΣ ΦΙΛΙΑΤΩΝ
   3: ΕΝΑ ΑΓΡΟΤΙΚΟ ΞΕΣΗΚΩΜΑ (1858-1930)
   4: 938.937ΣΚΟ
-  5: '2842'
+  5: '2841'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 249Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΦΙΛΙΑΤΕΣ
   14: ΦΙΛΙΑΤΕΣ-ΑΓΡΟΤΙΚΟ ΞΕΣΗΚΩΜΑ
@@ -19883,15 +19852,15 @@
   11: 13Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΒΙΒΛΙΟΚΡΙΣΙΕΣ
   13: ΒΙΒΛΙΟΚΡΙΣΙΕΣ-ΛΟΓΟΤΕΧΝΙΑ
 - 0: 1547
   1: ΛΟΥΚΑΤΟΣ,ΔΗΜΗΤΡΙΟΣ Σ
   2: Ο ΠΑΡΟΙΜΙΑΚΟΣ ΛΟΓΟΣ ΤΩΝ ΗΠΕΙΡΩΤΩΝ
   4: 938.93ΛΟΥ
-  5: 2768-2887
+  5: '2768'
   8: ΑΘΗΝΑ
   9: Χ.Ε
   10: '1976'
   11: 36Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΗΠΕΙΡΟΣ
   13: ΗΠΕΙΡΟΣ-ΠΑΡΟΙΜΙΑΚΟΣ ΛΟΓΟΣ
   14: ΠΑΡΟΙΜΙΕΣ-ΗΠΕΙΡΟΣ
@@ -20074,15 +20043,15 @@
   13: ΘΡΑΚΗ-(1919-1922)
   14: ΕΛΛΗΝΙΚΑ ΕΛΕΥΘΕΡΙΑ-ΘΡΑΚΗ
 - 0: 1561
   1: Χ.Σ
   2: ΣΠΥΡΙΔΩΝ ΒΛΑΧΟΣ
   3: Α ΑΠΟ ΙΩΑΝΝΙΝΩΝ ΑΡΧΙΕΠΙΣΚΟΠΟΣ ΑΘΗΝΩΝ ΚΑΙ ΠΑΣΗΣ ΕΛΛΑΔΟΣ
   4: 938.936ΣΠΥ
-  5: 2783-9255Α
+  5: 2783-09255
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1970'
   11: 51Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΙΩΑΝΝΙΝΑ
   13: ΙΩΑΝΝΙΝΑ-ΑΡΧΙΕΠΙΣΚΟΠΟΣ
   14: ΒΛΑΧΟΣ-ΑΡΧΙΕΠΙΣΚΟΠΟΣ
@@ -20212,16 +20181,15 @@
   13: ΕΞΩΤΕΡΙΚΗ ΠΟΛΙΤΙΚΗ-ΕΛΛΑΣ
   17: Η ΣΥΓΧΡΟΝΟΣ ΕΘΝΙΚΗ ΚΡΙΣΙΣ
   21: ΙΩΑΝΝΗΣ ΚΑΠΟΔΙΣΤΡΙΑΣ;7
 - 0: 1571
   1: ΜΟΣΧΟΠΟΥΛΟΣ,ΙΩΑΝΝΗΣ ΝΙΚ
   2: ΠΑΝΣΛΑΥΙΣΜΟΣ ΚΑΙ ΕΛΛΗΝΙΣΜΟΣ
   4: 938.05ΣΦΑ
-  5: 2742-2743-2744-2746-
-  6: '2745'
+  5: 2745-2746
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1978'
   11: 66Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΠΑΝΣΛΑΙΣΜΟΣ
   13: ΠΑΝΣΛΑΙΣΜΟΣ-ΕΛΛΗΝΙΣΜΟΣ
   14: ΕΛΛΗΝΙΣΜΟΣ-ΠΑΝΣΛΑΥΙΣΜΟΣ
@@ -20269,15 +20237,15 @@
   14: ΠΑΙΔΕΙΑ-ΕΘΝΙΚΗ
   17: ΤΡΙΑ ΑΡΘΡΑ ΠΕΡΙ ΠΑΙΔΕΙΑΣ
   21: ΙΩΑΝΝΗΣ ΚΑΠΟΔΙΣΤΡΙΑΣ;2
 - 0: 1575
   1: ΛΑΜΠΡΙΔΗΣ,ΣΤΑΘΗΣ Δ
   2: ΙΩΑΝΝΗΣ ΛΑΜΠΡΙΔΗΣ
   4: 938.936ΛΑΜ
-  5: 2826-3693-9265Α
+  5: 2826-3693-09265
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: '1979'
   11: 67Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΖΑΓΟΡΙ
   13: ΖΑΓΟΡΙ-ΛΑΜΠΡΙΔΗΣ
   14: ΛΑΜΠΡΙΔΗΣ-ΓΙΑΤΡΟΣ
@@ -21653,48 +21621,25 @@
   12: ΠΑΓΚΟΣΜΙΑ ΦΙΛΟΣΟΦΙΑ-ΜΕΤΑΦΥΣΙΚΗ
   13: ΦΙΛΟΣΟΦΙΑ-ΜΕΤΑΦΥΣΙΚΗ
   14: ΜΕΤΑΦΥΣΙΚΗ-ΦΙΛΟΣΟΦΙΑ
   15: ΧΡΟΝΟΣ-ΦΙΛΟΣΟΦΙΑ
 - 0: 1678
   1: ΡΟΖΕΝΤΑΛ,Μ
   2: ΦΙΛΟΣΟΦΙΚΟ ΛΕΞΙΚΟ
-  4: 103 ΡΟΖ
-  5: '1909'
+  4: 103ΡΟΖ
+  5: '2909'
   8: Χ.Ε
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 233Σ
   12: ΠΑΓΚΟΣΜΙΑ ΦΙΛΟΣΟΦΙΑ-ΛΕΞΙΚΟ
   13: ΦΙΛΟΣΟΦΙΚΟ-ΛΕΞΙΚΟ
   14: ΛΕΞΙΚΟ-ΦΙΛΟΣΟΦΙΑ
 - 0: 1679
-  1: ΓΙΟΥΝΤΙΝ,Π
-  2: ΦΙΛΟΣΟΦΙΚΟ ΛΕΞΙΚΟ
-  4: 103 ΡΟΖ
-  5: '2909'
-  8: Χ.Ε
-  9: ΑΘΗΝΑ
-  10: Χ.Χ
-  11: 233Σ
-  12: ΠΑΓΚΟΣΜΙΑ ΦΙΛΟΣΟΦΙΑ-ΛΕΞΙΚΟ
-  13: ΦΙΛΟΣΟΦΙΑ-ΛΕΞΙΚΟ
-  14: ΛΕΞΙΚΟ-ΦΙΛΟΣΟΦΙΑ
 - 0: 1680
-  1: ΤΣΟΥΤΣΙΝΟΣ,ΘΕΟΧΑΡΗΣ
-  2: Ο ΟΜΗΡΟΣ ΚΑΤΑ ΤΟΝ ΦΙΛΟΣΟΦΟΥ
-  4: 185.1 ΤΣΟ
-  5: '2910'
-  8: Χ.Ε
-  9: ΑΘΗΝΑ
-  10: '1928'
-  11: 208Σ
-  12: ΕΛΛΗΝΙΚΗ ΦΙΛΟΣΟΦΙΑ-ΑΡΙΣΤΟΤΕΛΗ
-  13: ΦΙΛΟΣΟΦΙΑ-ΑΡΙΣΤΟΤΕΛΗ
-  14: ΑΡΙΣΤΟΤΕΛΗ-ΟΜΗΡΟΣ
-  15: ΟΜΗΡΟΣ-ΑΡΙΣΤΟΤΕΛΗ
 - 0: 1681
   1: ΤΟΥΡΝΙΕΡ,ΠΟΛ
   2: ΤΟ ΠΡΟΣΩΠΕΙΟΝ ΚΑΙ Η ΠΡΟΣΩΠΙΚΟΤΗΣ
   4: 126 ΤΟΥ
   5: '2995'
   6: ΧΑΡΟΚΟΠΟΥ,ΔΗΜ
   8: Χ.Ε
@@ -22018,15 +21963,15 @@
   12: ΠΑΓΚΟΣΜΙΑ ΦΙΛΟΣΟΦΙΑ-ΨΥΧΟΛΟΓΙΑ
   13: ΦΙΛΟΣΟΦΙΑ-ΨΥΧΟΛΟΓΙΑ
   14: ΨΥΧΟΛΟΓΙΑ-ΔΙΑΙΣΘΗΣΕΙΣ
   15: ΑΓΑΠΗ-ΠΡΟΒΛΗΜΑΤΑ
 - 0: 1704
   1: WILAMOWITZ-MOELLENDORFF,ULRICH
   2: ARISTOTELES UHD ATHEN
-  4: 185.1 WIL
+  4: 185.1WIL
   5: '3006'
   8: X.E
   9: BERLIN
   10: '1893'
   11: 428S
   12: ΕΛΛΗΝΙΚΗ ΦΙΛΟΣΟΦΙΑ-ΑΡΙΣΤΟΤΕΛΗΣ
   13: ΦΙΛΟΣΟΦΙΑ-ΑΡΙΣΤΟΤΕΛΗΣ
@@ -22235,26 +22180,14 @@
   11: 125Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΙΓΡΑΦΕΣ
   13: ΕΠΙΓΡΑΦΕΣ-ΗΜΙΣΕΛΗΝΟΣ
   14: ΗΜΙΣΕΛΗΝΟΣ
   15: ΑΡΧΑΙΟΤΗΤΑ-ΗΜΙΣΕΛΗΝΟΣ
   17: Β ΣΥΓΓΡΑΦΕΑΣ:ΔΗΜΗΤΟΚΑΛΛΗΣ Γ
 - 0: 1720
-  1: ΔΗΜΗΤΟΚΑΛΛΗΣ,Γ
-  2: Η ΕΛΛΗΝΙΚΗ ΗΜΙΣΕΛΗΝΟΣ
-  4: 938.101ΜΟΥ
-  5: '3171'
-  8: Χ.Ε
-  9: ΑΘΗΝΑ
-  10: '1988'
-  11: 125Σ
-  12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΠΙΓΡΑΦΕΣ
-  13: ΕΠΙΓΡΑΦΕΣ-ΗΜΙΣΕΛΗΝΟΣ
-  14: ΗΜΙΣΕΛΗΝΟΣ
-  17: Β ΣΥΓΓΡΑΦΕΑΣ:ΜΟΥΤΣΟΠΟΥΛΟΣ,Ν
 - 0: 1721
   1: Χ.Σ
   2: ΔΟΚΙΜΙΟΝ ΠΕΡΙ ΑΡΤΗΣ
   4: 938.21 ΔΟΚ
   5: '282'
   8: Χ.Ε
   9: ΑΡΤΑ
@@ -22701,19 +22634,21 @@
   13: ΔΗΜΟΣΘΕΝΗΣ-ΠΟΛΙΤΙΚΟΣ
   14: ΠΟΛΙΤΙΚΟΣ-ΔΗΜΟΣΘΕΝΗΣ
   17: ΔΗΜΟΣΘΕΝΗΣ Ο ΠΟΛΙΤΙΚΟΣ ΚΑΙ ΟΙ ΣΚΟΠΟΙ ΤΟΥ
 - 0: 1757
   1: CURTIUS ERNST                       GER
   2: GRIECHISCHE GESCHCHTE
   4: 938 CUR
-  5: 3088-
+  5: '3088'
   8: WEIDMANNSHE
   9: BERLIN
   10: '1887'
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
+  13: ΙΣΤΟΡΙΑ ΕΛΛΗΝΙΚΗ
+  14: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
   17: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ
 - 0: 1758
   1: BENGTSON HERMANN                   GER
   2: GRIECHISCHE GESCHICHTE
   4: 938.19 BEN
   5: '3103'
   8: BECK'SCHE
@@ -24546,26 +24481,26 @@
   14: ΚΑΠΙΤΑΛΙΣΜΟΣ-ΚΕΦΑΛΑΙΟ
   15: ΚΕΦΑΛΑΙΟ-ΚΑΠΙΤΑΛΙΣΜΟΣ
   17: ΚΕΦΑΛΑΙΟ ΚΑΙ ΚΑΠΙΤΑΛΙΣΜΟΣ ΘΕΤΙΚΗ ΘΕΩΡΙΑ ΤΟΥ ΚΕΦΑΛΑΙΟ
 - 0: 1908
   1: DRONSEN JOH                        GER
   2: GESCHICHTE ALEXANDER DES GROSSEN
   4: 938.174DRO
-  5: 3471-
+  5: '3428'
   8: GCHEND
   9: BERLIN
   10: '1913'
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   13: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   14: ΜΑΚΕΔΟΝΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   17: Η ΙΣΤΟΡΙΑ ΤΟΥ ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
 - 0: 1909
   1: NIEBUHR B                           GER
   2: KLEINE HISTORISCHE UND PHILOLOSCH
-  4: 102 NIE
+  4: 102NIE
   5: '3471'
   8: ZELLER
   9: OSNABRUHCK
   10: '1269'
   12: ΠΑΓΚΟΣΜΙΑ ΦΙΛΟΣΟΦΙΑ-ΔΙΑΤΡΙΒΕΣ
   13: ΦΙΛΟΣΟΦΙΑ-ΔΙΑΤΡΙΒΕΣ
   14: ΔΙΑΤΡΙΒΕΣ-ΦΙΛΟΣΟΦΙΑ
@@ -24582,15 +24517,14 @@
   12: ΤΕΧΝΗ-ΙΣΤΟΡΙΑ
   13: ΚΟΙΝΩΝΙΟΛΟΓΙΑ-ΤΕΧΝΗ
   17: Η ΙΣΤΟΡΙΑ ΤΗΣ ΤΕΧΝΗΣ ΑΠΟ ΚΟΙΝΩΝΙΟΛΟΓΙΚΗΣ ΑΠΟΨΗΣ
 - 0: 1911
   1: GEBER FRITS                         GER
   2: ALEXANDER DER GROSSE YND DIE DIADOCHEN
   4: 938.174GEB
-  5: '3473'
   8: OUELLE-WENER
   9: LEIPZIG
   10: '1925'
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   13: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ-ΔΙΑΔΟΧΟΙ
   14: ΜΑΚΕΔΟΝΙΑ-ΔΙΑΔΟΧΟΙ
   15: ΔΙΑΔΟΧΟΙ-ΜΑΚΕΔΟΝΙΑ
@@ -25491,24 +25425,14 @@
   8: GRUYTER
   9: BERLIN
   10: '1924'
   12: ΔΙΚΑΙΟ-ΕΠΙΣΤΗΜΗ
   13: ΕΠΙΣΤΗΜΗ-ΔΙΚΑΙΟ
   17: ΕΠΙΣΤΗΜΗ ΚΑΙ ΔΙΚΑΙΟ
 - 0: 1988
-  1: STAMMLER RUDOLF                   GER
-  2: WIRTSCHAFT UND RECHT
-  4: 340 STA
-  5: '3562'
-  8: GRUYTER
-  9: BERLIN
-  10: '1924'
-  12: ΔΙΚΑΙΟ-ΕΠΙΣΤΗΜΗ
-  13: ΕΠΙΣΤΗΜΗ-ΔΙΚΑΙΟ
-  17: ΕΠΙΣΤΗΜΗ ΚΑΙ ΔΙΚΑΙΟ
 - 0: 1989
   1: GULDENPENNING A                     GER
   2: GESCHICHTE DES OSTROHMISCHEN REICHES
   4: 938.192GUL
   5: '3563'
   8: HAKKERT
   9: AMSTERDAM
@@ -25619,29 +25543,28 @@
   12: ΠΟΛΙΤΙΚΗ ΕΠΙΣΤΗΜΗ-ΑΡΧΙΤΕΧΝΙΤΕΣ
   13: ΑΡΧΙΤΕΧΝΙΤΕΣ-ΠΟΛΙΤΙΚΗ
   14: ΠΟΛΙΤΙΚΗ-ΑΡΧΙΤΕΧΝΙΤΕΣ
   17: ΑΡΧΙΤΕΧΝΙΤΕΣ ΤΗΣ ΠΟΛΙΤΙΚΗΣ
 - 0: 1999
   1: SOMBART WERNER                     GER
   2: DER MODERNE KAPITALISMUS
-  4: 320 SOM
-  5: 3575-
+  4: 320SOM
+  5: '3575'
   8: DUNCKER
   9: MUHNCHEN
   10: '1922'
   12: ΠΟΛΙΤΙΚΗ ΕΠΙΣΤΗΜΗ-ΚΕΦΑΛΟΚΡΑΤΙΑ
   13: ΕΠΙΣΤΗΜΗ-ΠΟΛΙΤΙΚΗ
   14: ΚΕΦΑΛΟΚΡΑΤΙΑ
   17: Η ΜΟΝΤΕΡΝΑ ΚΕΦΑΛΟΚΡΑΤΙΑ
   30: 3 ΤΟΜΟΙ
 - 0: 2000
   1: WILAMOWIZ URICH                     GER
   2: KLEINE SCHRIFTEN
-  4: 834 WIL
-  5: 3575-
+  4: 834WIL
   8: AKADEMIE VERLAG
   9: BERLIN
   10: '1971'
   12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΚΕΙΜΕΝΑ
   13: ΛΟΓΟΤΕΧΝΙΑ-ΚΕΙΜΕΝΑ
   14: ΚΕΙΜΕΝΑ-ΓΕΡΜΑΝΙΚΑ
   17: ΚΕΙΜΕΝΑ
@@ -26688,16 +26611,15 @@
   12: ΡΩΜΑΙΚΗ ΙΣΤΟΡΙΑ
   13: ΡΩΜΗ-ΙΣΤΟΡΙΑ
   17: ΡΩΜΑΙΚΗ ΙΣΤΟΡΙΑ
   30: 3 ΤΟΜΟΙ
 - 0: 2089
   1: BEKGTSON HERMANN                   GER
   2: HERRSCHERGESTALTE DES HELLENISMUS
-  4: 938 BEK
-  5: '3088'
+  4: 938BEK
   8: BECK
   9: MUHNCHEN
   10: '1975'
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΣΜΟΣ
   13: ΕΛΛΗΝΙΣΜΟΣ
   17: Η ΒΑΣΙΚΗ ΜΟΡΦΗ ΤΟΥ ΕΛΛΗΝΙΣΜΟΥ
 - 0: 2090
@@ -26872,39 +26794,28 @@
   8: ROTHSCHILD
   9: BERLIN
   10: '1920'
   12: ΠΟΛΙΤΙΚΗ ΟΙΚΟΝΟΜΙΑ-ΛΕΞΙΚΟ
   13: ΛΕΞΙΚΟ-ΠΟΛΙΤΙΚΗ ΟΙΚΟΝΟΜΙΑ
   14: ΟΙΚΟΝΟΜΙΑ-ΠΟΛΙΤΙΚΗ
   17: ΛΕΞΙΚΟ ΤΗΣ ΠΟΛΙΤΙΚΗΣ ΟΙΚΟΝΟΜΙΑΣ ΑΝΟΙΚΟΔΟΜΗΣΗ
-  30: '                <<ΤΟΜΟΣ IV>>'
+  30: '                <<ΤΟΜΟΣ Ι,IV>>'
 - 0: 2104
   1: HANDBUCH DER POLITIK                GER
   2: URCUNDEN ZUR POLITIK UNSERER ZEIT
   4: 303 HAN
   5: '3142'
   8: ROTHSCHILD
   9: BERLIN
   10: '1926'
   12: ΠΟΛΙΤΙΚΗ-ΛΕΞΙΚΟ
   13: ΛΕΞΙΚΟ-ΠΟΛΙΤΙΚΗ
   17: ΛΕΞΙΚΟ ΠΟΛΙΤΙΚΗ ΕΓΓΡΑΦΑ ΕΠΙ ΤΗΣ ΠΟΛΙΤΙΚΗΣ ΤΗΣ ΕΠΟΧΗΣ ΜΑΣ
   30: '                   <<ΤΟΜΟΙ VI>>'
 - 0: 2105
-  1: HANDBUCH DER POLITIK                GER
-  2: DIE GRUNDLAGEN DER POLITIK
-  4: 303 HAN
-  5: '3141'
-  8: ROTHSCHILD
-  9: BERLIN
-  10: '1920'
-  12: ΠΟΛΙΤΙΚΗ-ΛΕΞΙΚΟ
-  13: ΛΕΞΙΚΟ-ΠΟΛΙΤΙΚΗ
-  17: ΛΕΞΙΚΟ ΠΟΛΙΤΙΚΗ ΟΙ ΒΑΣΕΙΣ ΤΗΣ ΠΟΛΙΤΙΚΗΣ
-  30: '              <<ΤΟΜΟΣ I>>'
 - 0: 2106
   1: BRANDSTAETER                        GER
   2: GESCHICHTEN AETOLISCHEN LANDES-VOLKES YND BYNDES
   4: 838.22 BRA
   5: '3143'
   8: KAIMER
   9: BERLIN
@@ -27764,26 +27675,14 @@
   10: '1925'
   12: ΕΛΛΗΝΙΚΗ ΦΙΛΟΣΟΦΙΑ-ΦΙΛΟΣΟΦΟΙ
   13: ΦΙΛΟΣΟΦΟΙ-ΕΛΛΗΝΕΣ
   14: ΦΙΛΟΣΟΦΙΑ-ΦΙΛΟΣΟΦΟΙ
   17: ΕΛΛΗΝΕΣ ΦΙΛΟΣΟΦΟΙ
   30: ΤΟΜΟΣ 2ΚΑΙ3
 - 0: 2180
-  1: WILAMOWITZ ULRICH                   GER
-  2: ARISTOLELES UND ATHEN
-  4: 185.1 WIL
-  5: '3006'
-  8: WEIDMANN
-  9: BERLIN
-  10: '1893'
-  12: ΕΛΛΗΝΙΚΗ ΦΙΛΟΣΟΦΙΑ-ΑΡΙΣΤΟΤΕΛΗΣ
-  13: ΑΡΙΣΤΟΤΕΛΗΣ-ΑΘΗΝΑ
-  14: ΑΘΗΝΑ-ΑΡΙΣΤΟΤΕΛΗΣ
-  17: ΑΡΙΣΤΟΤΕΛΗΣ ΚΑΙ ΑΘΗΝΑΙ
-  30: ΤΟΜΟΣ Β
 - 0: 2181
   1: BAHRDT HANS                         GER
   2: WEGE ZUR SOZIOLOGIE
   4: 301 BAH
   5: '3224'
   12: ΚΟΙΝΩΝΙΟΛΟΓΙΑ
   17: ΒΗΜΑΤΑ ΣΤΗΝ ΚΟΙΝΩΝΙΟΛΟΓΙΑ
@@ -28285,15 +28184,14 @@
   14: ΕΠΙΣΤΗΜΗ-ΚΟΛΛΕΒΙΣΤΙΚΗ
   15: ΣΟΒΙΕΤ-ΕΠΙΣΤΗΜΗ
   17: ΣΟΒΙΕΤΙΚΗ ΕΠΙΣΤΗΜΗ ΚΟΛΛΕΒΙΣΤΙΚΗ
 - 0: 2224
   1: DEUSSEN PAUL                       GER
   2: DIE PHILOSOPHIE DER GRIECEN
   4: 180.938DEU
-  5: '3271'
   8: BROCKHAUS
   9: LEIPZIG
   10: '1921'
   12: ΕΛΛΗΝΙΚΗ ΦΙΛΟΣΟΦΙΑ
   13: ΦΙΛΟΣΟΦΙΑ-ΕΛΛΗΝΙΚΗ
   17: Η ΕΛΛΗΝΙΚΗ ΦΙΛΟΣΟΦΙΑ
 - 0: 2225
@@ -28378,35 +28276,24 @@
   10: '1936'
   12: ΦΙΛΟΣΟΦΙΑ-ΠΑΡΑΚΕΛΣΟΣ
   13: ΠΑΡΑΚΕΛΣΟΣ-ΦΙΛΟΣΟΦΙΑ
   17: ΠΑΡΑΚΕΛΣΟΣ
 - 0: 2232
   1: FINLAY GEORG                        GER
   2: GRIECHENLAND UNTER DEN ROHMERIN
-  4: 938.19 FIN
+  4: 938.19FIN
   5: '3278'
   8: WIGANT
   9: LEIPZIG
   10: '1861'
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΡΩΜΑΙΟΙ
   13: ΡΩΜΑΙΚΗ ΚΥΡΙΑΡΧΙΑ-ΕΛΛΗΝΕΣ
   14: ΡΩΜΑΙΟΙ
   17: ΟΙ ΕΛΛΗΝΕΣ ΥΠΟ ΤΗΝ ΚΑΤΟΧΗ ΤΩΝ ΡΩΜΑΙΩΝ
 - 0: 2233
-  1: FINLAY GEORG                       GER
-  2: GRIECHENLAND UNTER DEN ROHMERN
-  4: 938.19 FIN
-  5: '3278'
-  8: WIGANT
-  9: LEIPZIG
-  10: '1861'
-  12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΡΩΜΑΙΟΙ
-  13: ΡΩΜΑΙΟΙ
-  14: ΡΩΜΑΙΚΗ ΚΥΡΙΑΡΧΙΑ
-  17: ΟΙ ΕΛΛΗΝΕΣ ΥΠΟ ΤΗΝ ΚΑΤΟΧΗ ΤΩΝ ΡΩΜΑΙΩΝ
 - 0: 2234
   1: SCHILLNG KURT                     GER
   2: EINFUHRUNG IN DIE STAATS UND RECHTS-PHILOSOPHIE
   4: 177 SCH
   5: '3279'
   8: JUNKER
   9: BERLIN
@@ -29303,33 +29190,26 @@
   13: ΗΠΕΙΡΟΣ-ΜΟΛΟΣΣΟΙ
   14: ΜΟΛΟΣΣΟΙ-ΜΥΘΟΙ
   15: ΜΥΘΟΙ-ΜΟΛΟΣΣΟΙ
 - 0: 2307
   1: ΜΟΜΣΕΝ,ΘΕΟΔΩΡΟΥ
   2: ΡΩΜΑΙΚΗ ΙΣΤΟΡΙΑ
   4: 937 ΜΟΜ
-  5: 3648-3647-3649-
+  5: 3647-3648-3649
   6: ΣΑΚΕΛΛΑΡΟΠΟΥΛΟΣ
   8: ΣΑΚΕΛΛΑΡΙΟΥ
   9: ΑΘΗΝΑ
   10: '1906'
   11: 706Σ
   12: ΡΩΜΑΙΚΗ ΙΣΤΟΡΙΑ
+  13: ΙΣΤΟΡΙΑ ΡΩΜΑΙΚΗ
+  14: ΡΩΜΑΙΚΗ ΙΣΤΟΡΙΑ
   17: 2 ΑΝΤΙΤΥΠΑ ΤΟΜΟΣ 1
   30: 1 ΑΝΤΙΤΥΠΟ ΤΟΜΟΣ 2
 - 0: 2308
-  1: ΣΑΚΕΛΛΑΡΟΠΟΥΛΟΣ,
-  2: ΡΩΜΑΙΚΗ ΙΣΤΟΡΙΑ
-  4: 937 ΜΟΜ
-  5: 3648-3647-3649-
-  8: ΣΑΚΕΛΛΑΡΙΟΥ
-  9: ΑΘΗΝΑ
-  10: '1906'
-  11: 704Σ
-  12: ΡΩΜΑΙΚΗ ΙΣΤΟΡΙΑ
 - 0: 2309
   1: ΠΑΠΑΣΤΑΥΡΟΣ.ΙΩΑΝΝΗΣ Σ
   2: ΡΩΜΑΙΚΗ ΙΣΤΟΡΙΑ ΑΠΟ ΤΗΝ ΠΑΛΑΙΟΤΑΤΩΝ ΧΡΟΝΩΝ ΜΕΧΡΙ ΤΟΥ 395Μ.Χ
   4: 937 ΠΑΠ
   5: '3646'
   8: Χ.Ε
   9: ΑΘΗΝΑ
@@ -33983,15 +33863,14 @@
   14: ΛΕΝΙΝ-ΣΟΣΙΑΛΙΣΜΟΣ
   17: Η ΕΦΑΡΜΟΓΗ ΤΟΥ ΣΟΣΙΑΛΙΣΜΟΥ
   30: ΠΛΑΤΩΝ-ΛΕΝΙΝ
 - 0: 2704
   1: VRANOUSSIS L                       GAL
   2: L'HELLENISME POTBYZANTIN ET L'EUROPE
   4: 938.301VRA
-  5: '3753'
   8: LIVRES
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΒΥΖΑΝΤΙΟ
   13: ΒΥΖΑΝΤΙΟ-ΠΗΓΕΣ
   14: ΕΥΡΩΠΗ-ΧΕΙΡΟΓΡΑΦΑ
   15: ΧΕΙΡΟΓΡΑΦΑ-ΕΥΡΩΠΗ
   17: Ο ΜΕΤΑΒΥΖΑΝΤΙΝΟΣ ΕΛΛΗΝΙΣΜΟΣ ΚΑΙ Η ΕΥΡΩΠΗ
   30: ΧΕΙΡΟΓΡΑΦΑ,ΒΙΒΛΙΑ,ΕΝΤΥΠΑ
@@ -34511,15 +34390,15 @@
   14: ΠΛΑΤΙΑΝΑ
   15: ΟΛΥΜΠΙΑ
 - 0: 2749
   1: ΓΑΛΑΝΗΣ,ΓΙΩΡΓΟΣ
   2: ΨΥΧΟΛΟΓΙΑ ΤΗΣ (ΕΠΙ)ΜΟΡΦΩΣΗΣ ΕΝΗΛΙΚΩΝ
   3: ΘΕΩΡΗΤΙΚΕΣ ΚΑΙ ΠΡΑΚΤΙΚΕΣ ΠΡΟΣΕΓΓΙΣΕΙΣ
   4: 136.5 ΓΑΛ
-  5: '4092'
+  5: '4091'
   8: ΠΑΠΑΖΗΣΗ
   9: ΑΘΗΝΑ
   10: '1993'
   12: ΨΥΧΟΛΟΓΙΑ-ΕΝΗΛΙΚΟΙ
   13: ΕΝΗΛΙΚΟΙ-ΨΥΧΟΛΟΓΙΑ
   14: ΜΟΡΦΩΣΗ-ΨΥΧΟΛΟΓΙΑ
 - 0: 2750
@@ -36743,15 +36622,14 @@
   12: ΑΦΡΙΚΗ-ΑΝΤΑΡΤΙΚΟ
   13: ΑΝΤΑΡΤΙΚΟ-ΑΦΡΙΚΗ
   17: CORNEWALL BARBARA
 - 0: 2923
   1: ΧΑΜΠΣΟΝ,ΝΟΡΜΑΝ
   2: Ο ΔΙΑΦΩΤΙΣΜΟΣ
   4: 938.482ΧΑΜ
-  5: '4152'
   6: ΜΠΕΧΛΙΚΑΛΗ ΔΗΜΗΤΡΑ
   8: ΠΑΠΑΖΗΣΗ
   9: ΑΘΗΝΑ
   10: Χ.Χ
   11: 326Σ
   12: ΕΛΛΗΝΙΚΗ ΙΣΤΟΡΙΑ-ΔΙΑΦΩΤΙΣΜΟΣ
   13: ΔΙΑΦΩΤΙΣΜΟΣ
@@ -36834,27 +36712,26 @@
   11: 95Σ
   12: ΣΥΓΧΡΟΝΗ ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΝΟΥΒΕΛΛΕΣ
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
 - 0: 2930
   1: ΠΕΤΣΚΟΣ,ΧΑΡΑΛΑΜΠΟΣ
   2: ΔΙΨΑ ΖΩΗΣ
-  4: 889ΠΕΤ
-  5: '5744'
+  4: 889.21ΠΕΤ
   9: ΑΘΗΝΑ
   10: '1976'
   11: 245Σ
   12: ΣΥΓΧΡΟΝΟ ΚΟΙΝΩΝΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΣΥΓΧΡΟΝΗ ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ-ΛΟΓΟΤΕΧΝΙΑ
 - 0: 2931
   1: ΜΠΑΛΟΥΜΗΣ,ΕΠΑΜΕΙΝΩΝΔΑΣ
   2: ΓΙΑ ΤΗΝ ΚΟΛΧΙΔΑ
   4: 889.21ΜΠΑ
-  5: '5869'
+  5: '5684'
   8: ΚΕΔΡΟΣ
   9: ΑΘΗΝΑ
   10: '1963'
   11: 125Σ
   12: ΣΥΓΧΡΟΝΗ ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
 - 0: 2932
@@ -36891,15 +36768,15 @@
   12: ΣΥΓΧΡΟΝΟ ΕΛΛΗΝΙΚΟ ΠΝΕΥΜΑ ΚΑΙ ΣΑΤΥΡΑ
   13: ΧΡΟΝΟΓΡΑΦΗΜΑ
   14: ΣΥΓΧΡΟΝΟ ΕΛΛΗΝΙΚΟ ΧΡΟΝΟΓΡΑΦΗΜΑ
 - 0: 2935
   1: ΖΑΔΕΣ,ΔΗΜΟΣΘΕΝΗΣ
   2: ΚΑΤΩ ΕΚΕΙ ΣΤΟΥΣ ΚΟΡΣΕΟΥΣ
   4: 889.21ΖΑΔ
-  5: '2063'
+  5: '5536'
   8: ΜΑΥΡΙΔΗΣ
   10: '1958'
   11: 99Σ
   12: ΣΥΓΧΡΟΝΗ ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΝΟΥΒΕΛΑ
 - 0: 2936
@@ -37447,30 +37324,30 @@
   9: ΑΘΗΝΑ
   10: '1987'
   11: 165Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑΤΑ
 - 0: 2982
-  1: ΒΑΝΤΖΙΑΣ,ΓΙΑΝΝΗΣ
+  1: ΒΑΤΖΙΑΣ,ΓΙΑΝΝΗΣ
   2: ΠΕΡIΠΛΑΝΩΜΕΝΟΙ
-  4: 889ΒΑΤ
+  4: 889.21ΒΑΤ
   5: '4338'
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: '1983'
   11: 172Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑΤΑ
 - 0: 2983
   1: ΙΕΡΩΝΥΜΙΔΗΣ,ΛΟΥΛΑΣ
   2: ΜΙΑ ΚΑΠΟΙΑ ΕΥΑ
   4: 889.21ΙΕΡ
-  5: '5743'
+  5: '6083'
   8: ΑΛΚΑΙΟΣ
   9: ΑΘΗΝΑ
   10: '1975'
   11: 117Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑΤΑ
@@ -37755,15 +37632,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 3008
   1: ΕΥΑΓΓΕΛΟΥ,ΑΝΕΣΤΗΣ
   2: ΤΟ ΞΕΝΟΔΟΧΕΙΟ ΚΑΙ ΤΟ ΣΠΙΤΙ
   4: 889.21ΕΥΑ
-  5: '2355'
+  5: '5531'
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '1966'
   11: 38Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΗΜΑ
   13: ΠΕΖΟΓΡΑΦΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΕΖΟΓΡΑΦΗΜΑ
 - 0: 3009
@@ -38104,15 +37981,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 3037
   1: ΚΑΡΑΒΙΑ-ΧΑΤΖΟΠΟΥΛΟΥ,ΛΕΙΑ
   2: Ο ΔΡΟΜΟΣ ΤΟΥ ΘΥΜΩΜΕΝΟΥ ΠΟΤΑΜΟΥ
   4: 889.21ΚΑΡ
-  5: '5629'
+  5: '5622'
   9: ΑΘΗΝΑ
   10: '1963'
   11: 110Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 3038
@@ -38196,15 +38073,15 @@
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑΤΑ
 - 0: 3045
   1: ΠΟΛΙΤΗ,ΚΟΣΜΑ
   2: ΣΤΟΥ ΧΑΤΖΗΦΡΑΓΚΟΥ
   3: ΤΑ ΣΑΡΑΝΤΑ ΧΡΟΝΙΑ ΜΙΑΣ ΧΑΜΕΝΗΣ ΠΟΛΙΤΕΙΑΣ
   4: 889.21ΠΟΛ
-  5: '2036'
+  5: '5784'
   8: ΚΑΡΑΒΙΑ
   9: ΑΘΗΝΑ
   10: '1963'
   11: 318Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑΤΑ
@@ -38342,15 +38219,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 3057
   1: ΝΑΚΟΥ,ΛΙΛΙΚΑ
   2: ΓΙΑ ΜΙΑ ΚΑΙΝΟΥΡΓΙΑ ΖΩΗ
   4: 889.21ΝΑΚ
-  5: '2305'
+  5: '2306'
   9: ΑΘΗΝΑ
   10: '1960'
   11: 342Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΡΟΜΑΝΤΖΟ
   13: ΡΟΜΑΝΤΖΟ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΡΟΜΑΝΤΖΟ
 - 0: 3058
@@ -38458,16 +38335,16 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
   17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 3067
   1: ΚΩΣΤΑΡΑ,ΒΑΣΙΛΗΣ
   2: Η ΚΡΑΥΓΗ ΤΟΥ ΗΛΙΟΥ
-  4: 889ΚΩΣ
-  5: '4359'
+  4: 889.21ΚΩΣ
+  5: '4353'
   8: ΑΧΑΙΚΕΣ ΕΚΔΟΣΕΙΣ
   9: ΠΑΤΡΑ
   11: 177Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
 - 0: 3068
@@ -38507,15 +38384,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΠΕΖΟΓΡΑΦΙΑ
   13: ΠΕΖΟΓΡΑΦΙΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΕΖΟΓΡΑΦΙΑ
 - 0: 3071
   1: ΕΛΕΥΘΕΡΙΑΔΗΣ,ΜΙΜΗΣ
   2: ΑΜΑΡΤΩΛΗ ΓΗ
   4: 889.21ΕΛΕ
-  5: '5062'
+  5: '5532'
   10: '1977'
   11: 177Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 3072
   1: ΡΥΣΣΙΑΝΟΣ,ΝΟΤΗΣ
@@ -38736,15 +38613,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑΤΑ
 - 0: 3090
   1: ΑΡΒΑΝΙΤΗΣ,ΔΙΟΝΥΣΗΣ
   2: ΑΝΑΜΝΗΣΕΙΣ ΑΠΟ ΤΑ ΧΡΟΝΙΑ ΕΚΕΙΝΑ
   4: 889.21ΑΡΒ
-  5: '2356'
+  5: '5432'
   9: ΑΘΗΝΑ
   10: '1969'
   11: 94Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 3091
@@ -38806,16 +38683,15 @@
   11: 332Σ
   12: ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑΤΑ
 - 0: 3096
   1: ΜΟΣΚΟΒΗ,ΒΑΣΙΛΗ
   2: Η ΑΥΛΗ ΤΗΣ ΜΗΤΕΡΑΣ
-  4: 889ΜΟΣ
-  5: '2153'
+  4: 889.21ΜΟΣ
   8: ΜΑΥΡΙΔΗΣ
   9: ΑΘΗΝΑ
   10: '1958'
   11: 270Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
@@ -38899,15 +38775,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑΤΑ
 - 0: 3104
   1: ΣΚΑΡΙΜΠΑ,ΓΙΑΝΝΗ
   2: Η ΜΑΘΗΤΕΥΟΜΕΝΗ ΤΩΝ ΤΑΚΟΥΝΙΩΝ
   4: 889ΣΚΑ
-  5: '2211'
+  5: '10269'
   8: ΔΙΦΡΟΣ
   9: ΑΘΗΝΑ
   10: '1960'
   11: 152Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
@@ -39164,15 +39040,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ-ΠΑΙΔΙΚΟ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑΤΑ
   15: ΠΑΙΔΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
 - 0: 3126
   1: ΜΑΝΙΑΤΑΚΟΥ,ΓΙΩΡΓΟΥ
   2: ΤΟ ΣΥΝΝΕΦΟ ΔΕΝ ΕΦΕΡΕ ΒΡΟΧΗ
-  4: 889ΜΑΝ
+  4: 889.21ΜΑΝ
   5: '2273'
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: '1961'
   11: 241Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -39358,15 +39234,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 3142
   1: ΦΛΩΡΟΥ,ΠΑΥΛΟΥ
   2: ΑΠΟΙΚΟΙ
   4: 889.21ΦΛΩ
-  5: '4701'
+  5: '5901'
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   11: 414Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 3143
@@ -40055,25 +39931,14 @@
   9: ΠΑΤΡΑ
   10: '1965'
   11: 32Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΦΗΓΗΜΑΤΑ
   13: ΑΦΗΓΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΑΦΗΓΗΜΑΤΑ
 - 0: 3201
-  1: ΒΑΤΖΙΑΣ ΓΙΑΝΝΗΣ
-  2: ΠΕΡΙΠΛΑΝΩΜΕΝΟΙ
-  4: 889.21ΒΑΤ
-  5: '4338'
-  8: ΕΣΤΙΑ
-  9: ΑΘΗΝΑ
-  10: '1983'
-  11: 172Σ
-  12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
-  13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
-  14: ΜΥΘΙΣΤΟΡΗΜΑ
 - 0: 3202
   1: ΠΡΑΤΣΙΚΑ,ΜΑΝΩΛΗ
   2: Η ΑΓΟΝΗ ΓΡΑΜΜΗ
   4: 889.21ΠΡΑ
   5: '5779'
   9: ΠΑΤΡΑ
   10: '1966'
@@ -40093,14 +39958,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 3204
   1: ΡΕΝΟΣ
   2: ΠΥΡΑΜΙΔΑ 67
   4: 889.21ΡΕΝ
+  5: '5028'
   8: ΚΟΛΛΑΡΟΣ
   9: ΑΘΗΝΑ
   10: '1950'
   11: 320Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
@@ -40162,15 +40028,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 3210
   1: ΖΑΔΕ,ΔΗΜΟΣΘΕΝΗΣ
   2: ΓΙΑ ΣΜΕΡΝΕΣ
   4: 889.21ΖΑΔ
-  5: '5892'
+  5: '5529'
   8: ΤΡΙΦΥΛΙΑΚΗ ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: '1977'
   11: 133Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
@@ -40268,15 +40134,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 3219
   1: ΣΑΡΑΝΤΗ,ΓΑΛΑΤΕΙΑ
   2: ΠΑΣΧΑΛΙΕΣ
   4: 889.21ΣΑΡ
-  5: '5825'
+  5: '5824'
   8: ΑΛΦΑ
   9: ΑΘΗΝΑ
   10: '1949'
   11: 245Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑΤΑ
@@ -40751,14 +40617,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
   13: ΔΙΗΓΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 3259
   1: ΣΚΑΡΟΥ,ΖΗΣΗ
   2: ΤΟ ΤΑΞΙΔΙ ΤΗΣ ΦΙΛΙΑΣ
   4: 889.21ΣΚΑ
+  5: '22165'
   9: ΑΘΗΝΑ
   10: '1956'
   11: 232Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
   13: ΔΙΗΓΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 3260
@@ -40819,15 +40686,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
   13: ΔΙΗΓΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 3265
   1: ΜΗΤΡΟΠΟΥΛΟΥ,ΚΩΣΤΟΥΛΑΣ
   2: ΑΡΘΡΟ Νο 22
   4: 889.21ΜΗΤ
-  5: '5969'
+  5: '5696'
   8: ΜΙΝΩΑΣ
   9: ΑΘΗΝΑ
   11: 220Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
   13: ΔΙΗΓΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
   17: 2 ΑΝΤΙΤΥΠΑ
@@ -41188,15 +41055,14 @@
   11: 229Σ
   12: ΕΛΛΗΝΙΚΑ ΔΟΚΙΜΙΑ
   13: ΔΟΚΙΜΙΑ
 - 0: 3297
   1: ΡΩ-ΣΙΓΜΑ,ΖΗΤΑ
   2: ΣΤΑ ΣΥΡΜΑΤΟΠΛΕΓΜΑΤΑ ΤΗΣ ΣΚΛΑΒΙΑΣ
   4: 889.21ΣΡΩ
-  5: '2076'
   9: ΑΘΗΝΑ
   10: '1959'
   11: 259Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
   13: ΔΙΗΓΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 3298
@@ -42049,27 +41915,26 @@
   11: 161Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑ
 - 0: 3370
   1: ΑΠΟΣΤΟΛΙΔΗ,ΗΡ.Ν
   2: ΤΟ ΔΙΗΓΗΜΑ
-  4: 889ΑΠΟ
-  5: '2154'
+  4: 889.21ΑΠΟ
   9: ΑΘΗΝΑ
   10: '1953'
   11: 538Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑ
 - 0: 3371
   1: ΒΗΚΑΣ,Β
   2: ΣΥΝΤΡΙΜΜΙΑ
   4: 889.21ΒΗΚ
-  5: '5463'
+  5: '5465'
   8: ΑΘΗΝΑ
   9: ΑΘΗΝΑ
   11: 112Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΡΟΜΑΝΤΖΟ
   13: ΡΟΜΑΝΤΖΟ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΡΟΜΑΝΤΖΟ
 - 0: 3372
@@ -42270,15 +42135,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
 - 0: 3389
   1: ΑΘΑΝΑΣΙΑΔΗ,ΝΙΚΟ
   2: ΠΕΡΑ ΑΠΟ ΤΟ ΑΝΘΡΩΠΙΝΟ
   4: 889.21ΑΘΑ
-  5: '2182'
+  5: '54092182'
   8: ΣΤΕΓΗ ΤΟΥ ΒΙΒΛΙΟΥ
   9: ΑΘΗΝΑ
   10: '1956'
   11: 540Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
@@ -42630,15 +42495,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑ
 - 0: 3420
   1: ΠΕΦΑΝΗ,ΔΩΡΟΥ
   2: ΤΟ ΜΟΙΡΑΙΟ ΡΟΜΑΝΤΖΟ
   4: 889.21ΠΕΦ
-  5: '5788'
+  5: 05788
   8: ΚΟΝΤΖΑΝΑΣΤΗ
   9: ΑΘΗΝΑ
   10: '1935'
   11: 80Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
@@ -42756,27 +42621,26 @@
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑ
 - 0: 3431
   1: ΣΚΙΑΔΑΡΕΣΗ,ΣΠΥΡΟΥ
   2: ΚΕΦΑΛΟΝΙΤΙΚΕΣ ΙΣΤΟΡΙΕΣ
   4: 889.21ΣΚΙ
-  5: '2151'
+  5: '5850'
   8: ΔΙΦΡΟΣ
   9: ΑΘΗΝΑ
   10: '1959'
   11: 180Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
   13: ΔΙΗΓΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 3432
   1: ΑΡΚΑΔΙΟΥ,ΛΕΥΚΟΥ
   2: ΔΑΙΜΟΝΕΣ ΚΑΙ ΣΤΑΥΡΟΙ
   4: 889ΑΡΚ
-  5: '2116'
   8: ΜΑΥΡΙΔΗΣ
   9: ΑΘΗΝΑ
   10: '1959'
   11: 415Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
@@ -42916,15 +42780,14 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑ
 - 0: 3445
   1: ORWELL,GEORGE
   2: ΤΟ ΤΣΙΦΛΙΚΙ ΤΩΝ ΖΩΩΝ
   4: 823ORW
-  5: '2347'
   9: ΑΘΗΝΑ
   10: '1951'
   11: 133Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
 - 0: 3446
@@ -43128,15 +42991,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑ
 - 0: 3463
   1: ΜΑΝΙΑΤΑΚΟΥ,ΓΙΩΡΓΟΥ
   2: ΚΑΤΩ ΑΠΟ ΞΕΝΟΝ ΗΛΙΟ
   4: 889.21ΜΑΝ
-  5: '5746'
+  5: '6086'
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: '1958'
   11: 332Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
@@ -43588,16 +43451,15 @@
   11: 73Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑ
 - 0: 3502
   1: ΑΘΑΝΑΣΙΑΔΗΣ,ΠΕΤΡΟΣ
   2: ΤΟ ΓΥΜΝΟ ΚΟΡΙΤΣΙ
-  4: 889ΑΘΑ
-  5: '2106'
+  4: 889.21ΑΘΑ
   8: ΗΕΛΛΑΣ
   9: ΑΘΗΝΑ
   10: '1964'
   11: 236Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
@@ -43888,15 +43750,15 @@
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑ
 - 0: 3527
   1: WHARTON,EDITH
   2: ΣΤΑ ΔΕΝΤΡΑ ΣΤΟ ΧΙΟΝΙ
   3: ΕΘΑΝ ΦΡΟΜ
   4: 889WHA
-  5: '2323'
+  5: '1294'
   6: Ν.ΚΩΝΣΤΑΝΤΙΝΟΥ
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: '1956'
   11: 136Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -44219,15 +44081,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑ
 - 0: 3555
   1: ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛ.
   2: ΚΑΛΗΝΥΧΤΑ ΖΩΗ
   4: 889.21ΛΟΥ
-  5: '5656'
+  5: '5650'
   7: 2ΕΚΔ
   8: ΚΕΔΡΟΣ
   9: ΑΘΗΝΑ
   10: '1956'
   11: 228Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -44256,15 +44118,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑ
 - 0: 3558
   1: ΡΩΜΑ,ΔΙΟΝ.
   2: Ο ΣΟΠΡΑΚΟΜΙΤΟΣ
   4: 889.21ΡΩΜ
-  5: '2435'
+  5: '5804'
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   11: 444Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΧΡΟΝΙΚΟ
   13: ΧΡΟΝΙΚΟ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΧΡΟΝΙΚΟ
 - 0: 3559
@@ -44498,15 +44360,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑ
 - 0: 3578
   1: Χ.Σ
   2: Ο ΜΙΚΡΟΣ ΔΗΜΗΤΡΙΟΣ ΑΡΚΕΤΗΣ
   4: 889.21Χ.Σ
-  5: '3925'
+  5: '5925'
   8: ΣΙΔΕΡΗΣ
   9: ΑΘΗΝΑ
   11: 80Σ
   12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑ
 - 0: 3579
@@ -44521,15 +44383,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΚΟ ΔΙΗΓΗΜΑ
   13: ΙΣΤΟΡΙΚΟ ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΙΣΤΟΡΙΚΟ ΔΙΗΓΗΜΑ
 - 0: 3580
   1: ΨΑΛΤΟΠΟΥΛΟΥ,Λ.
   2: ΘΕΙΑ ΤΡΑΓΩΔΙΑ
   4: 889.21ΨΑΛ
-  5: '4691'
+  5: '5937'
   8: ΤΡΙΑΝΤΑΦΥΛΛΟΥ
   9: ΘΕΣΣΑΛΟΝΙΚ
   11: 124Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑ
 - 0: 3581
@@ -44567,15 +44429,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
   13: ΔΙΗΓΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 3584
   1: NEALE,A.
   2: ΘΕΟΔΩΡΑ ΦΡΑΝΤΖΗ
   4: 823NEA
-  5: '5726'
+  5: '5725'
   8: ΤΣΑΓΚΑΡΑΚΗΣ
   9: ΑΘΗΝΑ
   10: '1901'
   11: 351Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -44747,15 +44609,15 @@
   12: ΓΑΛΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
   13: ΔΙΗΓΗΜΑΤΑ-ΓΑΛΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 3598
   1: ΕΦΤΑΛΙΩΤΗΣ,ΑΡΓΥΡΗΣ
   2: ΝΗΣΙΩΤΙΚΕΣ ΙΣΤΟΡΙΕΣ
   4: 889.21ΕΦΤ
-  5: '2197'
+  5: '5535'
   8: ΦΕΞΗ
   9: ΑΘΗΝΑ
   10: '1941'
   11: 152Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
   13: ΔΙΗΓΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
@@ -44892,14 +44754,15 @@
   13: ΔΙΗΓΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑ
 - 0: 3609
   1: ΒΕΡΝ,ΙΟΥΛΙΟΣ
   2: ΑΠΑΝΤΑ
   3: ΕΝΑ ΔΡΑΜΑ ΣΤΗ ΛΙΒΟΝΙΑ
   4: 808.899ΒΕΡ
+  5: '20686'
   6: Μ.ΠΑΠΑΔΑΤΟΥ
   8: ΓΕΜΕΝΤΖΟΠΟΥΛΟΣ
   9: ΑΘΗΝΑ
   11: 165Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -45006,15 +44869,15 @@
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑ
   13: ΔΙΗΓΗΜΑ-ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑ
 - 0: 3618
   1: MALAMUD,BERNARD
   2: ΤΟ ΜΑΓΙΚΟ ΒΑΡΕΛΙ
   4: 810.11MAL
-  5: '2234'
+  5: '1313'
   6: ΜΑΝΘΟΣ ΚΡΙΣΠΗΣ
   8: Η ΣΥΓΧΡΟΝΗ ΑΜΕΡΙΚΗ
   9: ΑΘΗΝΑ
   10: '1953'
   11: 202Σ
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
   13: ΔΙΗΓΗΜΑΤΑ-ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -45045,15 +44908,15 @@
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
   13: ΔΙΗΓΗΜΑΤΑ-ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 3621
   1: ΧΙΛΤΟΝ,ΤΖΕΗΜΣ
   2: ΧΑΜΕΝΟΣ ΟΡΙΖΩΝ
   4: 823ΧΙΛ
-  5: 2240-20420
+  5: '1321'
   6: ΜΑΓΔΑ ΚΑΙΝΑΔΑ
   8: ΓΑΛΑΞΙΑΣ
   9: ΑΘΗΝΑ
   10: '1961'
   11: 172Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
   13: ΔΙΗΓΗΜΑΤΑ-ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -45508,15 +45371,14 @@
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
 - 0: 3660
   1: ΣΙΝΟΠΟΥΛΟΥ,ΤΑΚΗ
   2: Η ΠΟΙΗΣΗ ΤΗΣ ΠΟΙΗΣΗΣ
   4: 889.1ΣΙΝ
-  5: '2813'
   9: ΑΘΗΝΑ
   10: '1964'
   11: 61Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
 - 0: 3661
@@ -45822,15 +45684,15 @@
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
 - 0: 3687
   1: ΛΟΥΡΑΝΑΣ,ΠΕΤΡΑΣ
   2: ΑΝΘΡΩΠΙΝΑ
   4: 889.1ΛΟΥ
-  5: '6306'
+  5: '6227'
   8: ΠΥΡΣΟΣ
   9: ΑΘΗΝΑ
   10: '1941'
   11: 32Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
@@ -46035,16 +45897,16 @@
   11: 64Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
 - 0: 3705
   1: ΚΟΚΚΙΝΟΣ,ΔΗΜΟΣΘ.
   2: ΗΡΩΙΚΑ
-  4: 889.1ΚΟΚ
-  5: 6169-5112
+  4: 889.11ΚΟΚ
+  5: '6169'
   8: ΔΩΔΩΝΗ
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '1977'
   11: 53Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
@@ -46214,16 +46076,16 @@
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
 - 0: 3720
   1: ΠΑΠΑ-ΜΠΟΥΜΗ,ΡΙΤΑ
   2: ΜΟΡΓΚΑΝ ΙΩΑΝΝΗΣ
   3: Ο ΓΥΑΛΙΝΟΣ ΠΡΙΓΚΙΠΑΣ ΚΑΙ ΟΙ ΜΕΤΑΜΟΡΦΩΣΕΙΣ ΤΟΥ
-  4: 889.1ΠΑΠ
-  5: '6354'
+  4: 889.11ΠΑΠ
+  5: '6334'
   8: ΚΑΡΑΝΑΣΗ
   9: ΑΘΗΝΑ
   10: '1976'
   11: 228Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
@@ -46848,15 +46710,15 @@
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
 - 0: 3773
   1: ΛΟΥΚΑΚΗΣ,ΚΩΣΤΑΣ
   2: ΤΟ ΠΑΙΔΑΑΚΙ ΠΟΥ ΕΦΥΓΕ
   4: 889.1ΛΟΥ
-  5: '2862'
+  5: '2542'
   8: Ο ΛΟΓΟΣ
   9: ΑΘΗΝΑ
   10: '1965'
   11: 84Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
@@ -46943,15 +46805,15 @@
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
 - 0: 3781
   1: ΓΚΑΤΣΟΣ,ΝΙΚΟΣ
   2: ΑΜΟΡΓΟΣ
   4: 889.1ΓΚΑ
-  5: '2509'
+  5: '4644'
   7: Β'ΕΚΔ
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: '1963'
   11: 45Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -47435,15 +47297,15 @@
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
 - 0: 3823
   1: ΚΑΤΣΑΝΟΥ,ΓΙΑΝΝΗΣ
   2: ΑΝΘΡΩΠΟΙ ΚΑΙ ΤΟΠΙΟ
   4: 889.1ΚΑΤ
-  5: 4644-4533
+  5: '4533'
   9: ΑΘΗΝΑ
   10: '1989'
   11: 29Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
   17: 2 ΑΝΤΙΤΥΠΑ
@@ -48141,24 +48003,14 @@
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2004'
   11: 97Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
 - 0: 3884
-  1: ΙΑΝΝΗ
-  2: ΑΝΘΡΩΠΟΙ ΚΑΙ ΤΟΠΙΟ
-  4: 889.1ΚΑΤ
-  5: '4533'
-  9: ΑΘΗΝΑ
-  10: '1989'
-  11: 29Σ
-  12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
-  13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
-  14: ΠΟΙΗΣΗ
 - 0: 3885
   1: ΓΙΑΝΝΟΠΟΥΛΟΣ,ΤΑΚΗΣ
   2: ΕΠΑΝΟΔΟΣ
   4: 889.1ΓΙΑ
   5: '4534'
   9: ΑΘΗΝΑ
   10: '1982'
@@ -48257,16 +48109,16 @@
   11: 94Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
 - 0: 3894
   1: ΝΤΑΚΟΥ,Θ.
   2: ΔΕΥΤΕΡΑ ΠΡΩΙ
-  4: 889.1ΝΤΑ
-  5: '2776'
+  4: 889.11ΝΤΑ
+  5: '2578'
   8: ΔΙΑΓΩΝΙΟΥ
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '1966'
   11: 26Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
@@ -48704,16 +48556,16 @@
   11: 192Σ
   12: ΕΛΛΗΝΙΚΗ ΛΥΡΙΚΟΙ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΥΡΙΚΟΙ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ ΛΥΡΙΚΟΙ
 - 0: 3932
   1: ΕΓΓΟΝΟΠΟΥΛΟΣ,ΝΙΚΟΣ
   2: ΜΠΟΛΙΒΑΡ
-  4: 889.1ΕΓΓ
-  5: '2513'
+  4: 889.11ΕΓΓ
+  5: '2188'
   7: 2ΕΚΔ
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: '1962'
   11: 45Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -48789,16 +48641,16 @@
   11: 108Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
 - 0: 3939
   1: ΔΗΜΟΥΛΑ,ΚΙΚΗ
   2: ΕΠΙ ΤΑ ΙΧΝΗ
-  4: 889.1ΔΗΜ
-  5: '2546'
+  4: 889.11ΔΗΜ
+  5: '20565'
   8: ΦΕΞΗ
   9: ΑΘΗΝΑ
   10: '1963'
   11: 61Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
@@ -49254,16 +49106,15 @@
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
   17: 3 ΑΝΤΙΤΥΠΑ
 - 0: 3977
   1: ΠΑΠΑΔΙΤΣΑ,Δ.Π
   2: ΠΟΙΗΣΗ 2
-  4: 889.1ΠΑΠ
-  5: '2971'
+  4: 889.11ΠΑΠ
   8: ΕΚΔΟΣΕΙΣ ΤΩΝ ΦΙΛΩΝ
   9: ΑΘΗΝΑ
   10: '1974'
   11: 151Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
@@ -49740,38 +49591,28 @@
   10: '1954'
   11: 35Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
 - 0: 4018
   1: ΠΑΠΑΤΣΩΝΗΣ,Τ.Κ
-  2: ΕΚΛΟΓΗ Α'
+  2: ΕΚΛΟΓΗ Α', Β'
   3: URSA MINOR
   4: 888.08ΠΑΠ
   5: '6343'
   7: Β'ΕΚΔ
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: '1962'
   11: 166Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
+  17: ΤΟΜΟΙ Α, Β
 - 0: 4019
-  1: ΠΑΠΑΤΣΩΝΗΣ,Τ.Κ
-  2: ΕΚΛΟΓΗ Β'
-  4: 880.08ΠΑΠ
-  5: '6343'
-  8: ΙΚΑΡΟΣ
-  9: ΑΘΗΝΑ
-  10: '1962'
-  11: 175Σ
-  12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
-  13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
-  14: ΠΟΙΗΣΗ
 - 0: 4020
   1: ΚΙΝΤΖΟΝΙΔΗΣ,ΛΕΥΤΕΡΗΣ ΠΑΝΤ.
   2: ΣΚΙΟΦΩΤΑ ΚΑΙ ΧΑΡΑΥΓΕΣ
   4: 889.1ΚΙΤ
   5: '4429'
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '1991'
@@ -49849,15 +49690,15 @@
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
 - 0: 4027
   1: ΠΑΠΑΔΗΜΗΤΡΙΟΥ,Κ.Κ
   2: ΜΑΡΤΥΡΙΕΣ
   4: 889.1ΠΑΠ
-  5: 1679-1978
+  5: 1679-1678
   8: ΓΚΟΒΟΣΤΗΣ
   9: ΑΘΗΝΑ
   10: '1990'
   11: 78Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
@@ -50332,16 +50173,15 @@
   11: 35Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
 - 0: 4069
   1: ΠΑΠΑΔΙΤΣΑΣ,Δ.Π
   2: ΠΟΙΗΣΗ 1
-  4: 889.1ΠΑΠ
-  5: '2604'
+  4: 889.11ΠΑΠ
   8: ΠΡΩΤΗ ΥΛΗ
   9: ΑΘΗΝΑ
   10: '1963'
   11: 132Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
@@ -51453,15 +51293,15 @@
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
 - 0: 4166
   1: ΓΑΡΙΔΗΣ,ΚΩΣΤΑΣ
   2: ΖΗΤΗΜΑ ΠΛΕΥΣΕΩΣ
   4: 889.1ΓΑΡ
-  5: '6041'
+  5: '6011'
   8: ΣΕΙΡΙΟΣ
   9: ΑΘΗΝΑ
   10: '1975'
   11: 32Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
@@ -52539,15 +52379,15 @@
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
 - 0: 4259
   1: ΚΑΡΟΥΖΟΥ,Ν.Δ
   2: Ο ΥΠΝΟΣΑΚΚΟΣ
   4: 889.1ΚΑΡ
-  5: 6142-6143
+  5: '6143'
   9: ΑΘΗΝΑ
   10: '1964'
   11: 58Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
   17: 2 ΑΝΤΙΤΥΠΑ
@@ -52586,16 +52426,16 @@
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
 - 0: 4263
   1: ΧΡΙΣΤΙΑΝΟΠΟΥΛΟΣ,ΝΤΙΝΟΣ
   2: ΠΟΙΗΜΑΤΑ
   3: 1950-1955
-  4: 889.1ΧΡΙ
-  5: '2587'
+  4: 889.11ΧΡΙ
+  5: '2215'
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '1957'
   11: 52Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
 - 0: 4264
@@ -52618,16 +52458,16 @@
   11: 39Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
 - 0: 4266
   1: ΔΗΜΟΥΛΑ,ΑΘΟΥ
   2: ΕΝΔΟΝ
-  4: 889.1ΔΗΜ
-  5: '2750'
+  4: 889.11ΔΗΜ
+  5: '2756'
   8: ΔΙΦΡΟΣ
   9: ΑΘΗΝΑ
   10: '1960'
   11: 36Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
@@ -54497,15 +54337,15 @@
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
   17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 4428
   1: ΠΑΠΑΠΟΛΙΤΗΣ,ΣΩΤΗΡΗΣ
   2: ΔΑΚΡΥΑ ΔΙΧΩΣ ΤΙΤΛΟΥΣ...
   4: 889.1ΠΑΠ
-  5: '6363'
+  5: '6323'
   8: ΙΚΑΡΟΣ
   9: ΑΘΗΝΑ
   10: '1965'
   11: 81Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΠΟΙΗΣΗ
@@ -57011,15 +56851,15 @@
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
   13: ΔΙΗΓΗΜΑΤΑ-ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 4648
   1: ΝΤΙΚΕΝΣ,ΚΑΡΟΛΟΣ
   2: ΟΛΙΒΕΡ ΤΟΥΙΣΤ
   4: 808.899ΝΤΙ
-  5: 4787,9194Α
+  5: 4787-09194
   6: Π.ΣΤΡΑΤΙΚΗΣ
   8: ΑΓΚΥΡΑ
   9: ΑΘΗΝΑ
   10: '1991'
   11: 122Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -57226,15 +57066,15 @@
   11: '160'
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
   13: ΔΙΗΓΗΜΑΤΑ-ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 4665
   1: ΚΡΟΝΙΝ,Α
   2: ΤΑ ΑΓΟΥΡΑ ΧΡΟΝΙΑ
-  4: 8Ο8.899ΚΡΟ
+  4: 808.899ΚΡΟ
   5: 6666,9596,20585
   6: ΠΑΠΑΔΑΚΗ-ΜΑΥΡΟΕΙΔΗ,Σ
   8: ΑΣΤΗΡ
   9: ΑΘΗΝΑ
   10: '1978'
   11: 320Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΔΙΗΓΗΜΑΤΑ
@@ -60450,15 +60290,14 @@
   12: ΟΙΚΟΔΟΜΙΚΗ
   13: ΟΙΚΟΔΟΜΙΚΗ
   14: ΟΙΚΟΔΟΜΙΚΗ
   17: ΤΟΜΟΣ Α'
 - 0: 4943
   1: ΕΥΓΕΝΙΔΙΟ ΙΔΡΥΜΑ
   2: ΟΙΚΟΔΟΜΙΚΗ
-  5: '5788'
   8: ΕΥΓΕΝΙΔΙΟ ΙΔΡΥΜΑ
   9: ΑΘΗΝΑ
   10: '1975'
   11: 348Σ
   12: ΟΙΚΟΔΟΜΙΚΗ
   13: ΟΙΚΟΔΟΜΙΚΗ
   14: ΟΙΚΟΔΟΜΙΚΗ
@@ -61545,15 +61384,14 @@
   12: ΧΗΜΕΙΑ-ΓΕΝΙΚΗ ΧΗΜΕΙΑ
   13: ΓΕΝΙΚΗ ΧΗΜΕΙΑ
   14: ΧΗΜΕΙΑ
   17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 5036
   1: BARNARD & EDWARDS
   2: ΘΕΜΕΛΙΩΔΕΙΣ ΑΡΧΑΙ ΤΗΣ ΦΥΣΙΚΗΣ
-  5: '5892'
   8: ΠΕΧΛΙΒΑΝΙΔΗΣ
   9: ΑΘΗΝΑ
   11: 704Σ
   12: ΦΥΣΙΚΗ-ΘΕΜΕΛΙΩΔΕΙΣ ΑΡΧΕΣ
   13: ΘΕΜΕΛΙΩΔΕΙΣ ΑΡΧΕΣ-ΦΥΣΙΚΗ
   14: ΦΥΣΙΚΗ
 - 0: 5037
@@ -61757,15 +61595,14 @@
   11: 180Σ
   12: ΗΛΕΚΤΡΟΛΟΓΙΚΟ ΕΡΓΑΣΤΗΡΙΟ
   13: ΕΡΓΑΣΤΗΡΙΟ ΗΛΕΚΤΡΟΛΟΓΙΚΟ
   14: ΗΛΕΚΤΡΟΛΟΓΙΚΟ ΕΡΓΑΣΤΗΡΙΟ
 - 0: 5056
   1: ΖΑΧΑΡΗ,ΕΥΣΤΑΘΙΟΥ
   2: ΓΕΩΡΓΙΚΟΣ ΠΡΟΣΑΝΑΤΟΛΙΣΜΟΣ
-  5: '5825'
   8: ΕΥΓΕΝΙΔΙΟ ΙΔΡΥΜΑ
   9: ΑΘΗΝΑ
   10: '1978'
   11: 126Σ
   12: ΓΕΩΡΓΙΑ
   13: ΓΕΩΡΓΙΚΟΣ ΠΡΟΣΑΝΑΤΟΛΙΣΜΟΣ
   14: ΠΡΟΣΑΝΑΤΟΛΙΣΜΟΣ ΓΕΩΡΓΙΚΟΣ
@@ -63034,15 +62871,15 @@
   12: ΠΡΟΙΣΤΟΡΙΚΗ ΑΡΧΑΙΟΛΟΓΙΑ
   13: ΑΡΧΑΙΟΛΟΓΙΑ ΠΡΟΙΣΤΟΡΙΚΗ
   14: ΠΡΟΙΣΤΟΡΙΚΗ ΑΡΧΑΙΟΛΟΓΙΑ
 - 0: 5177
   1: ΜΑΜΜΟΠΟΥΛΟΥ,ΑΛΕΞΑΝΔΡΟΥ
   2: ΑΓΓΕΛΙΚΗ ΧΑΤΖΗΜΙΧΑΛΗ ΚΑΙ Η ΗΠΕΙΡΩΤΙΚΗ ΛΑΙΚΗ ΤΕΧΝΗ
   4: 938.93ΜΑΜ
-  5: 693-2823-9251Α
+  5: 693-2823-09251
   9: ΑΘΗΝΑ
   10: '1967'
   11: 47Σ
   12: ΛΑΙΚΗ ΤΕΧΝΗ-ΑΓΓΕΛΙΚΗ ΧΑΤΖΗΜΙΧΑΛΗ
   13: ΛΑΙΚΗ ΤΕΧΝΗ-ΑΓΓΕΛΙΚΗ ΧΑΤΖΗΜΙΧΑΛΗ
   14: ΛΑΙΚΗ ΤΕΧΝΗ-ΑΓΓΕΛΙΚΗ ΧΑΤΖΗΜΙΧΑΛΗ
 - 0: 5178
@@ -68706,15 +68543,15 @@
   13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΓΩΓΟΥ
 - 0: 5659
   1: ΝΤΑΓΚΛΑΣ,ΛΟΥΔ
   2: Ο ΧΙΤΩΝ
   4: 808.899ΝΤΑ
-  5: 6999,6665
+  5: 6999-6665
   6: ΓΙΑΝΝΗ ΛΑΜΨΑ
   7: 2η
   8: ΔΑΜΑΣΚΟΣ
   9: ΑΘΗΝΑ
   10: '1950'
   11: 438Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -69103,15 +68940,15 @@
   13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΓΩΓΟΥ
 - 0: 5688
   1: ΔΕΛΤΑ,Π.Σ
   2: ΤΟΝ ΚΑΙΡΟ ΤΟΥ ΒΟΥΛΓΑΡΟΚΤΟΝΟΥ
   4: 808.899ΔΕΛ
-  5: 6976,9192Α
+  5: 6976-09192
   8: ΔΑΜΙΑΝΟΣ
   9: ΑΘΗΝΑ
   11: 447Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΓΩΓΟΥ
@@ -75247,15 +75084,15 @@
   12: ΠΕΖΟΓΡΑΦΙΑ-ΠΟΙΗΣΗ
   13: ΙΣΤΟΡΙΑ-ΚΡΙΤΙΚΗ
   14: ΔΟΚΙΜΙΟ-ΘΕΑΤΡΟ
 - 0: 6172
   1: ΣΚΟΥΤΕΛΑ,ΠΕΤΡΟΥ
   2: ΤΟΥ ΧΩΡΙΟΥ ΚΑΙ ΤΗΣ ΠΟΛΗΣ
   4: 398ΣΚΟ
-  5: 8045-9146Α
+  5: 8045-09146
   9: ΑΘΗΝΑ
   10: '2002'
   11: 142Σ
   12: ΛΑΟΓΡΑΦΙΑ-ΒΙΩΜΑΤΑ
   13: ΛΑΟΓΡΑΦΙΚΑ ΣΤΟΙΧΕΙΑ
   14: ΒΙΩΜΑΤΑ-ΛΑΟΓΡΑΦΙΑ
   17: 6 ΑΝΤΙΤΥΠΑ
@@ -80090,15 +79927,15 @@
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   15: ΔΙΗΓΗΜΑΤΑ
 - 0: 6579
   1: ΤΟΥΡΑΤΣΟΓΛΟΥ,ΙΩΑΝΝΗΣ
   2: ΜΑΚΕΔΟΝΙΑ
   3: ΙΣΤΟΡΙΑ ΜΝΗΜΕΙΑ ΜΟΥΣΕΙΑ
   4: 938.666ΤΟΥ
-  5: 9298Α
+  5: 09298
   8: ΕΚΔΟΤΙΚΗ ΑΘΗΝΩΝ
   9: ΑΘΗΝΑ
   10: '1996'
   11: 459Σ
   12: ΜΑΚΕΔΟΝΙΑ
   13: ΜΑΚΕΔΟΝΙΑ
   14: ΜΑΚΕΔΟΝΙΑ
@@ -80106,14 +79943,17 @@
   1: ΑΘΑΝΑΣΙΟΥ,ΘΕΟΦΙΛΟΣ
   2: Η ΑΓΑΠΗ ΠΟΥ ΑΝΘΙΣΕ ΣΤΗΣ ΚΑΤΟΧΗΣ ΤΑ ΧΡΟΝΙΑ
   4: 889.21ΑΘΑ
   5: '8643'
   9: ΑΘΗΝΑ
   10: '2003'
   11: 172Σ
+  12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΛΟΓΟΤΕΧΝΙΑ
+  14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
 - 0: 6581
   1: ΗΛΙΑΔΗ,ΑΜΑΛΙΑ
   2: Ο ΚΛΗΡΟΣ ΣΤΟΝ ΜΑΚΕΔΟΝΙΚΟ ΑΓΩΝΑ
   5: '8642'
   8: ΠΡΟΤΥΠΕΣ ΘΕΣΣΑΛΙΚΕΣ
   9: ΤΡΙΚΑΛΑ
   10: '2003'
@@ -85104,15 +84944,15 @@
   14: ΔΙΗΓΗΜΑΤΑ
   15: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   19: '9608359333'
 - 0: 6989
   1: ΒΕΡΝ,ΙΟΥΛΙΟΣ
   2: Ο ΓΥΡΟΣ ΤΟΥ ΚΟΣΜΟΥ ΣΕ 80 ΜΕΡΕΣ
   4: 808.899ΒΕΡ
-  5: 9018,9091,9169Α
+  5: 9018-9091-09169
   8: ΑΛΚΥΩΝ,ΠΑΠΑΔΟΠΟΥΛΟΣ
   9: ΑΘΗΝΑ
   10: '2004'
   11: 271Σ
   12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
@@ -85621,15 +85461,15 @@
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-412-57
   19: 3-7
 - 0: 7028
   1: ΣΤΟΟΥ ΜΠΙΤΣΕΡ
   2: Η ΚΑΛΥΒΑ ΤΟΥ ΜΠΑΡΜΠΑ ΘΩΜΑ
   4: 808.899ΣΤΟ
-  5: 9093-9173Α-20640
+  5: 9093-09173-20640
   6: ΜΑΡΙΑ ΠΑΠΠΑ
   8: ΠΑΠΑΔΟΠΟΛΥΛΟΣ
   9: ΑΘΗΝΑ
   10: '2001'
   11: 143Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -86489,15 +86329,15 @@
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 7090
   1: ΒΕΡΝ,ΙΟΥΛΙΟΣ
   2: ΜΙΧΑΗΛ ΣΤΡΟΓΚΟΦ
   4: 808.899ΒΕΡ
-  5: 9171Α,19992
+  5: 09171-19992
   6: ΑΝΝΙΚΑ ΦΕΡΤΑΚΗ
   8: ΑΓΚΥΡΑ
   9: ΑΘΗΝΑ
   10: '2008'
   11: 323Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -86520,15 +86360,15 @@
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-422-06
   19: 9-1
 - 0: 7092
   1: ΤΟΥΕΙΝ,ΜΑΡΚ
   2: ΠΡΙΓΚΙΠΑΣ ΚΑΙ ΦΤΩΧΟΣ
   4: 808.899TOY
-  5: 9195A
+  5: 09195
   6: ΡΟΥΛΑ ΧΑΤΖΟΠΟΥΛΟΥ
   7: 5η
   8: ΑΓΚΥΡΑ
   9: ΑΘΗΝΑ
   10: '2006'
   11: 220Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -86536,45 +86376,45 @@
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-422-12
   19: 0-5
 - 0: 7093
   1: ΒΕΡΝ,ΙΟΥΛΙΟΣ
   2: ΡΟΒΗΡΟΣ Ο ΚΑΤΑΚΤΗΤΗΣ
   4: 808.899ΒΕΡ
-  5: 9175Α
+  5: 09175
   6: ΓΙΩΡΓΟΥ ΚΡΙΜΠΑ
   8: ΑΓΚΥΡΑ
   9: ΑΘΗΝΑ
   10: '2004'
   11: 211Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-422-08
   19: 2-9
 - 0: 7094
   1: ΚΙΠΛΙΝΓΚ,Ρ.
   2: ΟΙ ΜΙΚΡΟΙ ΘΑΛΑΣΣΟΛΥΚΟΙ
   4: 808.899ΚΙΠ
-  5: 9197Α
+  5: 09197
   6: Γ.ΤΣΟΥΚΑΛΑΣ
   8: ΑΓΚΥΡΑ
   9: ΑΘΗΝΑ
   10: '2004'
   11: 203Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-422-13
   19: 4-5
 - 0: 7095
   1: ΒΕΡΝ,ΙΟΥΛΙΟΣ
   2: Ο ΔΕΚΑΠΕΝΤΑΕΤΗΣ ΠΛΟΙΑΡΧΟΣ
   4: 808.899ΒΕΡ
-  5: 9170Α
+  5: 09170
   6: ΑΝΝΙΚΑ ΦΕΡΤΑΚΗ
   7: 5η
   8: ΑΓΚΥΡΑ
   9: ΑΘΗΝΑ
   10: '2006'
   11: 362Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -86582,30 +86422,30 @@
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-422-09
   19: 8-5
 - 0: 7096
   1: ΝΤΕΦΟΕ,ΝΤΑΝΙΕΛ
   2: ΡΟΒΙΝΣΩΝ ΚΡΟΥΣΟΣ
   4: 808.899ΝΤΕ
-  5: 9172Α
+  5: 09172
   6: ΑΝΝΙΚΑ ΦΕΡΤΑΚΗ
   8: ΑΓΚΥΡΑ
   9: ΑΘΗΝΑ
   10: '2004'
   11: 403Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-422-07
   19: 0-5
 - 0: 7097
   1: ΔΟΥΜΑΣ,ΑΛΕΞΑΝΔΡΟΣ
   2: ΟΙ ΤΡΕΙΣ ΣΩΜΑΤΟΦΥΛΑΚΕΣ
   4: 808.899ΔΟΥ
-  5: 9196Α-9096
+  5: 09196-9096
   6: Γ.ΤΣΟΥΚΑΛΑΣ
   8: ΑΓΚΥΡΑ
   9: ΑΘΗΝΑ
   10: '2008'
   11: 284Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -86613,128 +86453,128 @@
   17: 2 ΑΝΤΙΤΥΠΑ
   18: 978-960-42
   19: 2-587-3
 - 0: 7098
   1: ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
   2: Ο ΗΡΑΚΛΗΣ
   4: 808.899ΛΟΥ
-  5: 9182Α
+  5: 09182
   8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
   9: ΑΘΗΝΑ
   10: '2000'
   11: 213Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-393-13
   19: 5-7
 - 0: 7099
   1: ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
   2: ΕΝΑ ΠΑΙΔΙ ΜΕΤΡΑΕΙ ΤΑ ΑΣΤΡΑ
   4: 808.899ΛΟΥ
-  5: 9180A
+  5: 09180
   8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
   9: ΑΘΗΝΑ
   10: '1999'
   11: 540Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 978-960-34
   19: 4-768-9
 - 0: 7100
   1: ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
   2: ΒΟΥΡΚΩΜΕΝΕΣ ΜΕΡΕΣ
   4: 808.899ΛΟΥ
-  5: 9226Α
+  5: 09226
   8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
   9: ΑΘΗΝΑ
   10: '2000'
   11: 150Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-344-91
   19: 4-8
 - 0: 7101
   1: ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
   2: ΔΑΙΔΑΛΟΣ
   4: 808.899ΛΟΥ
-  5: 9181Α
+  5: 09181
   8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
   9: ΑΘΗΝΑ
   10: '2000'
   11: 243Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-393-13
   19: 6-5
 - 0: 7102
   1: ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
   2: Ο ΙΚΑΡΟΣ
   4: 808.899ΛΟΥ
-  5: 9179Α
+  5: 09179
   8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
   9: ΑΘΗΝΑ
   10: '1999'
   11: 233Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-344-83
   19: 5-4
 - 0: 7103
   1: ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
   2: ΘΗΣΕΑΣ
   4: 808.899ΛΟΥ
-  5: 9178Α
+  5: 09178
   8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
   9: ΑΘΗΝΑ
   10: '1999'
   11: 280Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-344-77
   19: 1-4
 - 0: 7104
   1: ΛΟΥΝΤΕΜΗΣ,ΜΕΝΕΛΑΟΣ
   2: ΚΑΛΗΝΥΧΤΑ ΖΩΗ
   4: 808.899ΛΟΥ
-  5: 9214Α
+  5: 09214
   8: ΕΛΛΗΝΙΚΑ ΓΡΑΜΜΑΤΑ
   9: ΑΘΗΝΑ
   10: '2000'
   11: 259Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-393-13
   19: 8-1
 - 0: 7105
   1: ΤΟΥΕΙΝ,ΜΑΡΚ
   2: ΟΙ ΠΕΡΙΠΕΤΕΙΕΣ ΤΟΥ ΤΟΜ ΣΟΓΙΕΡ
   4: 808.899ΤΟΥ
-  5: 9185Α
+  5: 09185
   6: ΠΙΕΡΕΤΑ ΔΙΑΜΑΝΤΟΠΟΥΛ
   8: ΕΡΕΥΝΗΤΕΣ
   9: ΑΘΗΝΑ
   10: '1999'
   11: 284Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-368-15
   19: 5-5
 - 0: 7106
   1: ΣΙΟΥΕΛ,ΑΝΝΑ
   2: ΜΑΥΡΗ ΚΑΛΛΟΝΗ
   4: 808.899ΣΙΟ
-  5: 9177Α
+  5: 09177
   6: ΓΙΩΡΓΟΣ ΜΑΡΚΑΚΗΣ
   8: ΕΡΕΥΝΗΤΕΣ
   9: ΑΘΗΝΑ
   10: '2001'
   11: 207Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -86767,210 +86607,210 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
 - 0: 7109
   1: ΛΟΝΤΟΝ,ΤΖΑΚ
   2: ΑΣΠΡΟΔΟΝΤΗΣ
   4: 808.899ΛΟΝ
-  5: 9184Α
+  5: 09184
   6: ΓΙΩΡΓΟΣ ΜΑΡΚΑΚΗΣ
   8: ΕΡΕΥΝΗΤΕΣ
   9: ΑΘΗΝΑ
   10: '2002'
   11: 237Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-368-23
   19: 8-1
 - 0: 7110
   1: ΣΑΡΗ,ΖΩΡΖ
   2: ΤΑ ΓΕΝΕΘΛΙΑ
   4: 808.899ΣΑΡ
-  5: 9204Α
+  5: 09204
   7: 25η
   8: ΠΑΤΑΚΗ
   9: ΑΘΗΝΑ
   10: '2007'
   11: 247Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 978-960-29
   19: 3-681-8
 - 0: 7111
   1: ΣΑΡΗ,ΖΩΡΖ
   2: ΤΟ ΠΑΡΑΡΑΔΙΑΣΜΑ
   4: 808.899ΣΑΡ
-  5: 9205Α
+  5: 09205
   7: 22η
   8: ΠΑΤΑΚΗ
   9: ΑΘΗΝΑ
   10: '2006'
   11: 202Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-293-47
   19: 7-8
 - 0: 7112
   1: ΣΑΡΗ,ΖΩΡΖ
   2: ΚΟΚΚΙΝΗ ΚΛΩΣΤΗ ΔΕΜΕΝΗ
   4: 808.899ΣΑΡ
-  5: 9199Α
+  5: 09199
   7: 19η
   8: ΠΑΤΑΚΗ
   9: ΑΘΗΝΑ
   10: '2007'
   11: 114Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 978-960-29
   19: 3-682-5
 - 0: 7113
   1: ΣΑΡΗ,ΖΩΡΖ
   2: ΤΑ ΣΤΕΝΑ ΠΑΠΟΥΤΣΙΑ
   4: 808.899ΣΑΡ
-  5: 9208Α
+  5: 09208
   7: 27η
   8: ΠΑΤΑΚΗ
   9: ΑΘΗΝΑ
   10: '2007'
   11: 166Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 978-960-29
   19: 3-676-4
 - 0: 7114
   1: ΖΕΗ,ΑΛΚΗ
   2: ΤΟ ΚΑΠΛΑΝΙ ΤΗΣ ΒΙΤΡΙΝΑΣ
   4: 808.899ΖΕΗ
-  5: 9209Α
+  5: 09209
   7: 238η
   8: ΚΕΔΡΟΣ
   9: ΑΘΗΝΑ
   10: '2007'
   11: 183Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 978-960-04
   19: -0007-6
 - 0: 7115
   1: ΣΑΡΗ,ΖΩΡΖ
   2: ΣΟΦΙΑ
   4: 808.899ΣΑΡ
-  5: 9200Α
+  5: 09200
   7: 11η
   8: ΠΑΤΑΚΗ
   9: ΑΘΗΝΑ
   10: '2008'
   11: 133Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 978-960-60
   19: 0-774-3
 - 0: 7116
   1: ΣΑΡΗ,ΖΩΡΖ
   2: ΟΤΑΝ Ο ΗΛΙΟΣ...
   4: 808.899ΣΑΡ
-  5: 9203Α
+  5: 09203
   7: 21η
   8: ΠΑΤΑΚΗ
   9: ΑΘΗΝΑ
   10: '2007'
   11: 260Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 978-960-29
   19: 3-677-1
 - 0: 7117
   1: ΣΑΡΗ,ΖΩΡΖ
   2: ΤΟΤΕ...
   4: 808.899ΣΑΡ
-  5: 9207Α
+  5: 09207
   7: 4η
   8: ΠΑΤΑΚΗ
   9: ΑΘΗΝΑ
   10: '2006'
   11: 124Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-16-131
   19: 8-8
 - 0: 7118
   1: ΣΑΡΗ,ΖΩΡΖ
   2: Ο ΚΥΡΙΟΣ ΜΟΥ
   4: 808.899ΣΑΡ
-  5: 9202Α
+  5: 09202
   7: 9η
   8: ΠΑΤΑΚΗ
   9: ΑΘΗΝΑ
   10: '2007'
   11: 131Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 978-960-16
   19: -0382-7
 - 0: 7119
   1: ΣΑΡΗ,ΖΩΡΖ
   2: ΚΡΙΜΑ ΚΙ ΑΔΙΚΟ
   4: 808.899ΣΑΡ
-  5: 9206Α
+  5: 09206
   7: 21η
   8: ΠΑΤΑΚΗ
   9: ΑΘΗΝΑ
   10: '2008'
   11: 142Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 978-960-29
   19: 3-563-7
 - 0: 7120
   1: ΔΕΛΤΑ,ΠΗΝΕΛΟΠΗ
   2: ΤΡΕΛΑΝΤΩΝΗΣ
   4: 808.899ΔΕΛ
-  5: 9189Α
+  5: 09189
   7: 22η
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: '2006'
   11: 286Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΝΧΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΝΧΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-05-037
   19: 9-6
 - 0: 7121
   1: ΣΚΟΤΤ,ΟΥΟΛΤΕΡ
   2: ΙΒΑΝΟΗΣ
   4: 808.899ΣΚΟ
-  5: 9183Α
+  5: 09183
   6: ΓΙΑΝΝΗΣ ΣΠΑΝΔΩΝΗΣ
   8: ΠΑΤΑΚΗ
   9: ΑΘΗΝΑ
   10: '1994'
   11: '483'
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-360-02
   19: 8-8
 - 0: 7122
   1: ΔΕΛΤΑ,ΠΗΝΕΛΟΠΗ
   2: Η ΖΩΗ ΤΟΥ ΧΡΙΣΤΟΥ
   4: 808.899ΔΕΛ
-  5: 9193Α
+  5: 09193
   7: 4η
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: '2000'
   11: 483Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -86991,15 +86831,15 @@
   13: ΔΟΚΙΜΙΑ
   14: ΔΟΚΙΜΙΑ ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 7124
   1: ΔΕΛΤΑ,ΠΗΝΕΛΟΠΗ
   2: ΣΤΑ ΜΥΣΤΙΚΑ ΤΟΥ ΒΑΛΤΟΥ
   4: 808.899ΔΕΛ
-  5: 9190Α
+  5: 09190
   7: 19η
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: '2007'
   11: 645Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -87007,15 +86847,15 @@
   17: 2 ΑΝΤΙΤΥΠΑ
   18: 960-05-034
   19: 3-5
 - 0: 7125
   1: ΠΑΠΑΝΤΩΝΙΟΥ,ΖΑΧΑΡΙΑΣ
   2: ΤΑ ΨΗΛΑ ΒΟΥΝΑ
   4: 808.899ΠΑΠ
-  5: 9188Α
+  5: 09188
   7: 33η
   8: ΕΣΤΙΑ
   9: ΑΘΗΝΑ
   10: '2007'
   11: 225Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -87157,15 +86997,15 @@
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 978-960-45
   19: 5-080-7
 - 0: 7135
   1: ΣΕΤΣΙΝΓΚ,ΦΡΑΝΚ
   2: ΤΟ ΣΜΗΝΟΣ
   4: 830.11ΣΕΤ
-  5: 9212Α
+  5: 09212
   6: ΣΤΕΦΑΝΟΣ ΤΖΑΝΝΕΤΑΤΟΣ
   8: ΚΑΣΤΑΝΙΩΤΗΣ
   9: ΑΘΗΝΑ
   10: '2007'
   11: 1018Σ
   12: ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΓΕΡΜΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -87187,15 +87027,15 @@
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 978-960-45
   19: 3-325-1
 - 0: 7137
   1: ΠΟΛΥΡΑΚΗΣ,ΓΙΩΡΓΟΣ
   2: ΣΙΩΠΗΛΕΣ ΚΡΑΥΓΕΣ
   4: 889.21ΠΟΛ
-  5: 9159Α
+  5: 09159
   8: ΨΥΧΟΓΙΟΣ
   9: ΑΘΗΝΑ
   10: '2007'
   11: 447Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
@@ -87231,15 +87071,15 @@
   15: ΜΥΘΙΣΤΟΡΗΜΑ
   18: 960-14-028
   19: 0-2
 - 0: 7140
   1: NEVILLE,KATHERINE
   2: ΟΧΤΩ
   4: 823NEV
-  5: 9153Α
+  5: 09153
   6: ΧΡΙΣΤ.ΣΑΚΕΛΛΑΡΟΠΟΥΛΟ
   8: ΝΕΑ ΣΥΝΟΡΑ
   9: ΑΘΗΝΑ
   10: '2005'
   11: 767Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -87247,29 +87087,30 @@
   15: ΜΥΘΙΣΤΟΡΗΜΑ
   18: 960-14-104
   19: 3-0
 - 0: 7141
   1: BROWN,DAN
   2: ΑΡΚΤΙΚΟΣ ΚΥΚΛΟΣ
   4: 810.11BRO
+  5: '9258'
   6: ΧΡΗΣΤΟΣ ΚΑΨΑΛΗΣ
   8: ΛΙΒΑΝΗ
   9: ΑΘΗΝΑ
   10: '2005'
   11: 644Σ
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΑΜΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
   18: 960-14-102
   19: 4-4
 - 0: 7142
   1: GOLDEN,ARTHUR
   2: ΑΝΑΜΝΗΣΕΙΣ ΜΙΑΣ ΓΚΕΙΣΑΣ
   4: 810.11GOL
-  5: 9168Α
+  5: 09168
   6: ΡΕΝΑ ΛΕΚΚΟΥ-ΔΑΝΤΟΥ
   8: ΛΙΒΑΝΗ
   9: ΑΘΗΝΑ
   10: '1998'
   11: 732Σ
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -87277,15 +87118,15 @@
   15: ΜΥΘΙΣΤΟΡΗΜΑ
   18: 960-236-91
   19: 3-2
 - 0: 7143
   1: ΔΗΜΟΥΛΙΔΟΥ,ΧΡΥΣΑ
   2: ΤΟ ΦΙΛΙ ΤΟΥ ΔΡΑΚΟΥ
   4: 889.21ΔΗΜ
-  5: 9162Α
+  5: 09162
   8: ΛΙΒΑΝΗ
   9: ΑΘΗΝΑ
   10: '2007'
   11: 460Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -87323,15 +87164,15 @@
   15: ΜΥΘΙΣΤΟΡΗΜΑ
   18: 960-14-081
   19: 9-3
 - 0: 7146
   1: HAMMOND,N.G.
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   3: Η ΙΣΤΟΡΙΚΗ ΓΕΩΓΡΑΦΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ (ΜΕΡΟΣ Α)
-  4: '398.666'
+  4: 938.1HAM
   5: 9217-9473
   8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2007'
   11: 280Σ
   12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
   13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
@@ -87339,31 +87180,31 @@
   17: ΤΟΜΟΣ 1
   18: 978-960-45
   19: 7-137-9
 - 0: 7147
   1: HAMMOND,N.G.
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   3: Η ΙΣΤΟΡΙΚΗ ΓΕΩΓΡΑΦΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ (ΜΕΡΟΣ Β)
-  4: '398.666'
-  5: 9217 -9473
+  4: 938.1HAM
+  5: 9217-9473
   8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2007'
   11: 280Σ
   12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
   13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   14: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
   17: ΤΟΜΟΣ 2
   18: 978-960-45
   19: 7-138-3
 - 0: 7148
   1: HAMMOND,N.G.
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   3: Η ΠΡΟΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
-  4: '398.666'
+  4: 938.1HAM
   5: 9217-9473
   8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2007'
   11: 300Σ
   12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
   13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
@@ -87371,14 +87212,15 @@
   17: ΤΟΜΟΣ 3
   18: 978-960-45
   19: 7-139-0
 - 0: 7149
   1: HAMMOND,N.G.
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   3: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 800-452 Π.Χ.
+  4: 938.1HAM
   5: '9217'
   8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2007'
   11: 300Σ
   12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
   13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
@@ -87386,14 +87228,15 @@
   17: ΤΟΜΟΣ 4
   18: 978-960-45
   19: 7-140-6
 - 0: 7150
   1: HAMMOND,N.G.
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   3: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 452-355 Π.Χ.
+  4: 938.1HAM
   5: '9217'
   8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2007'
   11: 300Σ
   12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
   13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
@@ -87401,14 +87244,15 @@
   17: ΤΟΜΟΣ 5
   18: 978-960-45
   19: 7-143-7
 - 0: 7151
   1: HAMMOND,N.G.
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   3: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 355-346 Π.Χ.
+  4: 938.1HAM
   5: '9217'
   8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2007'
   11: 300Σ
   12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
   13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
@@ -87416,14 +87260,15 @@
   17: ΤΟΜΟΣ 6
   18: 978-960-45
   19: 7-167-3
 - 0: 7152
   1: HAMMOND,N.G.
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   3: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 346-342 Π.Χ.
+  4: 938.1HAM
   5: '9217'
   8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2007'
   11: 300Σ
   12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
   13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
@@ -87431,14 +87276,15 @@
   17: ΤΟΜΟΣ 7
   18: 978-960-45
   19: 7-168-0
 - 0: 7153
   1: HAMMOND,N.G.
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   3: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 342-336 Π.Χ.
+  4: 938.1HAM
   5: '9217'
   8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2007'
   11: 300Σ
   12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
   13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
@@ -87446,14 +87292,15 @@
   17: ΤΟΜΟΣ 8
   18: 978-960-45
   19: 7-169-7
 - 0: 7154
   1: HAMMOND,N.G.
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   3: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 336-301 Π.Χ.
+  4: 938.1HAM
   5: '9217'
   8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2007'
   11: 300Σ
   12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
   13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
@@ -87461,14 +87308,15 @@
   17: ΤΟΜΟΣ 9
   18: 978-960-45
   19: 7-170-3
 - 0: 7155
   1: HAMMOND,N.G.
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   3: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 323-239 Π.Χ.
+  4: 938.1HAM
   5: '9217'
   8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2007'
   11: 300Σ
   12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
   13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
@@ -87476,14 +87324,15 @@
   17: ΤΟΜΟΣ 10
   18: 978-960-45
   19: 7-171-0
 - 0: 7156
   1: HAMMOND,N.G.
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   3: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 239-196 Π.Χ.
+  4: 938.1HAM
   5: '9217'
   8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2007'
   11: 300Σ
   12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
   13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
@@ -87491,28 +87340,30 @@
   17: ΤΟΜΟΣ 11
   18: 978-960-45
   19: 7-172-7
 - 0: 7157
   1: HAMMOND,N.G.
   2: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   3: ΤΑ ΙΣΤΟΡΙΚΑ ΓΕΓΟΝΟΤΑ 196-168 Π.Χ.
+  4: 938.1HAM
   5: '9217'
   8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2007'
   11: 300Σ
   12: ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ-ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ
   13: ΕΓΚΥΚΛΟΠΑΙΔΕΙΑ-ΙΣΤΟΡΙΑ ΤΗΣ ΜΑΚΕΔΟΝΙΑΣ
   14: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
   17: ΤΟΜΟΣ 12
   18: 978-960-45
   19: 7-173-4
 - 0: 7158
   1: HAMMOND,N.G.
-  2: ΦΙΛΙΠΠΟΣ Ο ΑΜΚΕΔΩΝ
+  2: ΦΙΛΙΠΠΟΣ Ο ΜAΚΕΔΩΝ
+  4: 938.1HAM
   5: '9217'
   8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2007'
   11: 300Σ
   12: ΙΣΤΟΡΙΑ-ΦΙΛΙΠΠΟΣ Ο ΜΑΚΕΔΩΝ
   13: ΦΙΛΙΠΠΟΣ Ο ΜΑΚΕΔΩΝ-ΙΣΤΟΡΙΑ
@@ -87521,14 +87372,15 @@
   17: ΠΑΡΑΡΤΗΜΑ Α
   18: 978-960-45
   19: 7-121-5
 - 0: 7159
   1: HAMMOND,N.G.
   2: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   3: ΕΝΑΣ ΙΔΙΟΦΥΗΣ
+  4: 938.070HAM
   5: '9217'
   8: ΜΑΛΛΙΑΡΗΣ ΠΑΙΔΕΙΑ
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2007'
   11: 300Σ
   12: ΙΣΤΟΡΙΑ-ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ
   13: ΜΕΓΑΣ ΑΛΕΞΑΝΔΡΟΣ-ΙΣΤΟΡΙΑ
@@ -87638,15 +87490,15 @@
   15: ΜΥΘΙΣΤΟΡΗΜΑ
   18: 978-960-41
   19: 0-468-0
 - 0: 7167
   1: ΠΙΛΤΣΕΡ,ΡΟΖΑΜΟΥΝΤ
   2: ΤΟ ΕΡΗΜΟ ΣΠΙΤΙ
   4: 823ΠΛΙ
-  5: 9166Α
+  5: 09166
   6: ΜΠΕΛΙΚΑ ΚΟΥΜΠΑΡΕΛΗ
   8: ΩΚΕΑΝΙΔΑ
   9: ΑΘΗΝΑ
   10: '2000'
   11: 186Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -87700,14 +87552,15 @@
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   15: ΜΥΘΙΣΤΟΡΗΜΑ
   18: 978-960-36
   19: 5-679-8
 - 0: 7171
   1: ΒΑΣΙΛΙΚΟΣ,ΒΑΣΙΛΗΣ
   2: ΤΟ ΤΕΛΕΥΤΑΙΟ ΑΝΤΙΟ
+  4: 889.21ΒΑΣ
   5: '9248'
   8: ΝΕΑ ΣΥΝΟΡΑ
   9: ΑΘΗΝΑ
   10: '1994'
   11: 165Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -87747,14 +87600,15 @@
   14: ΓΑΛΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   15: ΜΥΘΙΣΤΟΡΗΜΑ
   18: 960-240-00
   19: 1-3
 - 0: 7174
   1: ΣΑΡΤΡ
   2: Η ΑΝΑΣΤΟΛΗ
+  4: 843ΣΑΡ
   5: '9249'
   6: ΑΙΜ.ΧΟΥΡΜΟΥΖΙΟΥ
   8: ΑΡΣΕΝΙΔΗΣ
   9: ΑΘΗΝΑ
   11: 559Σ
   12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -87830,15 +87684,15 @@
   14: ΜΥΘΙΣΤΟΡΗΜΑ
   18: 960-7221-2
   19: 2-2
 - 0: 7180
   1: ΑΙΣΩΠΟΣ
   2: 135 ΜΥΘΟΙ ΤΟΥ ΑΙΣΩΠΟΥ
   4: 808.899AIΣ
-  5: 9198A
+  5: 09198
   8: ΑΓΚΥΡΑ
   9: ΑΘΗΝΑ
   10: '2007'
   11: 330Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -87886,15 +87740,15 @@
   13: ΑΣΤΥΝΟΜΙΚΟ-ΒΙΠΕΡ-ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΒΙΠΕΡ
   15: ΑΣΤΥΝΟΜΙΚΟ
 - 0: 7184
   1: ΜΠΛΟΚ,ΛΟΡΕΝΣ
   2: Ο ΔΙΑΡΡΗΚΤΗΣ ΠΟΥ ΖΩΓΡΑΦΙΖΕ ΣΑΝ ΤΟΝ ΜΟΝΤΡΙΑΝ
   4: 810.11ΜΠΛ
-  5: 9230,12492,20617
+  5: 9230-12492-20617
   6: ΚΑΤΕΡΙΝΑ ΡΟΝΤΟΓΙΑΝΝΗ
   8: ΜΟΝΤΕΡΝΟΙ ΚΑΙΡΟΙ
   9: ΑΘΗΝΑ
   10: '2004'
   11: 349Σ
   12: ΒΙΠΕΡ-ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΣΤΥΝΟΜΙΚΟ
   13: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΣΤΥΝΟΜΙΚΟ-ΒΙΠΕΡ
@@ -87981,14 +87835,16 @@
   13: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-216-04
   19: 2-Χ
 - 0: 7191
   1: ΖΟΛΑ,ΕΜΙΛ
   2: ΝΑΝΑ
+  4: 843ΖΟΛ
+  5: '9260'
   6: ΓΙΩΡΓΟΣ ΠΡΑΤΣΙΚΑΣ
   8: ΓΚΟΒΟΣΤΗΣ
   9: ΑΘΗΝΑ
   11: 536Σ
   12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -88022,15 +87878,15 @@
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   15: ΜΥΘΙΣΤΟΡΗΜΑ
   18: 960-03-082
   19: 3-3
 - 0: 7194
   1: ΓΟΥΛΦ,ΒΙΡΤΖΙΝΙΑ
   2: ΜΕΧΡΙ ΤΟ ΦΑΡΟ
-  4: 823 ΓΟΥ
+  4: 823ΓΟΥ
   5: '9221'
   6: ΕΛΛΗ ΜΑΡΜΑΡΑ
   8: ΤΟ ΒΗΜΑ
   9: ΑΘΗΝΑ
   10: '2007'
   11: 219Σ
   12: ΑΓΓΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
@@ -88648,15 +88504,15 @@
   14: ΠΑΙΔΙΚΑ ΒΙΒΛΙΑ
   17: 6 ΤΟΜΟΙ
 - 0: 7238
   1: ΣΚΟΥΤΕΛΑΣ,ΠΕΤΡΟΣ
   2: ΑΠΟ ΤΑ ΑΓΡΙΜΙΑ ΚΙ ΑΓΡΙΟΠΟΥΛΙΑ ΤΩΝ ΒΟΥΝΩΝ ΜΑΣ
   3: ΚΑΙ Η ΛΑΙΚΗ ΜΑΣ ΠΑΡΑΔΟΣΗ
   4: 398ΣΚΟ
-  5: 9145Α-9644
+  5: 09145-9644
   9: ΑΘΗΝΑ
   10: '2008'
   11: 148Σ
   12: ΛΑΟΓΡΑΦΙΑ
   13: ΛΑΟΓΡΑΦΙΑ
   14: ΛΑΟΓΡΑΦΙΑ
   17: 4 ΑΝΤΙΤΥΠΑ
@@ -88975,16 +88831,16 @@
   11: 127Σ
   12: ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
   13: ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
   14: ΜΕΓΑΛΟΥ ΑΛΕΞΑΝΔΡΟΥ
 - 0: 7262
   1: ΑΘΑΝΑΣΑΚΗ,ΑΝΤΩΝΙΟΥ
   2: ΤΟ ΑΣΤΡΟΧΩΡΙ ΑΡΤΑΣ
-  4: '938.939'
-  5: 9215Α
+  4: 938.939ΑΘΑ
+  5: 09215
   6: '9215'
   8: NEW TYPE
   9: ΑΡΤΑ
   10: '2000'
   11: 396Σ
   12: ΑΣΤΡΟΧΩΡΙ
   13: ΑΣΤΡΟΧΩΡΙ
@@ -89002,16 +88858,16 @@
   13: ΑΝΤΙΣΤΑΣΗ-ΕΜΦΥΛΙΟΣ
   14: ΙΣΤΟΡΙΑ
   18: 960-234-83
   19: 3-Χ
 - 0: 7264
   1: ΜΠΟΚΟΓΙΑΝΝΗΣ,ΧΡΥΣΟΣΤΟΜΟΣ
   2: ΟΙ ΡΙΖΕΣ ΜΑΣ
-  4: 398 ΜΠΟ
-  5: 9225Α
+  4: 398ΜΠΟ
+  5: 09225
   9: ΑΡΤΑ
   10: '2008'
   11: 71Σ
   12: ΛΑΟΓΡΑΦΙΑ
   13: ΛΑΟΓΡΑΦΙΑ
   14: ΛΑΟΓΡΑΦΙΑ
 - 0: 7265
@@ -89374,16 +89230,16 @@
   13: ΖΩΓΡΑΦΙΚΗ
   14: ΖΩΓΡΑΦΙΚΗ
   18: 960-7970-0
   19: 5-5
 - 0: 7292
   1: ΧΑΤΖΗΜΙΧΑΛΗ,ΑΓΓΕΛΙΚΗ
   2: Η ΕΛΛΗΝΙΚΗ ΛΑΙΚΗ ΦΟΡΕΣΙΑ
-  4: 398 ΧΑΤ
-  5: 9133Α
+  4: 398ΧΑΤ
+  5: 09133
   8: ΜΕΛΙΣΣΑ
   9: ΑΘΗΝΑ
   10: '1983'
   11: 464Σ
   12: ΛΑΙΚΗ ΦΟΡΕΣΙΑ-ΛΑΟΓΡΑΦΙΑ
   13: ΛΑΟΓΡΑΦΙΑ-ΛΑΙΚΗ ΦΟΡΕΣΙΑ
   14: ΕΛΛΗΝΙΚΗ ΛΑΙΚΗ ΦΟΡΕΣΙΑ
@@ -89732,26 +89588,26 @@
   12: ΙΣΤΟΡΙΑ-ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
   13: ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ-ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
   15: ΕΛΛΗΝΙΚΗ ΕΠΑΝΑΣΤΑΣΗ
 - 0: 7320
   1: ΠΑΠΠΑΣ,ΑΝΔΡΕΑΣ
   2: ΑΠ ΤΗΝ ΟΨΗ ΤΗΣ ΠΑΤΡΙΔΑΣ
-  4: 398 ΠΑΠ
+  4: 398ΠΑΠ
   5: '9296'
   9: ΚΑΛΕΝΤΙΝΗ
   10: '2005'
   11: 130Σ
   12: ΔΙΗΓΗΜΑΤΑ
   13: ΔΙΗΓΗΜΑΤΑ
   14: ΔΙΗΓΗΜΑΤΑ
 - 0: 7321
   1: ΠΑΠΠΑΣ,ΑΝΔΡΕΑΣ
   2: Ο ΘΡΥΛΟΣ ΤΗΣ ΓΚΟΛΦΩΣ
-  4: 398 ΠΑΠ
+  4: 398ΠΑΠ
   5: '9295'
   9: ΚΑΛΕΝΤΙΝΗ
   10: '2004'
   11: 144Σ
   12: ΔΙΗΓΗΜΑΤΑ
   13: ΔΙΗΓΗΜΑΤΑ
   14: ΔΙΗΓΗΜΑΤΑ
@@ -89789,17 +89645,17 @@
   13: ΠΟΛΕΜΟΣ 1940-ΙΣΤΟΡΙΑ
   14: ΗΡΩΕΣ 1940
   15: ΠΟΛΕΜΟΣ 1940
   18: 978-960-78
   19: 97-53-4
 - 0: 7325
   1: Χ.Σ.
-  2: ΑΓΡΙΑ  ΛΟΥΛΟΥΔΙΑ
+  2: ΑΓΡΙΑ ΛΟΥΛΟΥΔΙΑ
   3: Η ΕΚΘΑΜΒΩΤΙΚΗ ΕΛΛΗΝΙΚΗ ΧΛΩΡΙΔΑ ΜΕ ΤΟ ΦΑΚΟ ΤΟΥ ΓΙΩΡΓΟΥ ΑΒΑΓΙΑ
-  4: ΝΟΥ
+  4: 582.13Χ.Σ
   5: '9385'
   8: EXPLORE NATURE
   11: '170'
   12: ΑΓΡΙΑ ΛΟΥΛΟΥΔΙΑ
   13: ΛΟΥΛΟΥΔΙΑ
   14: ΥΠΕΡΟΧΗ ΕΛΛΑΔΑ
 - 0: 7326
@@ -89838,239 +89694,239 @@
   13: ΒΙΟΓΡΑΦΙΚΕΣ ΑΠΟΨΕΙΣ
   14: ΒΙΟΓΡΑΦΙΚΕΣ ΑΠΟΨΕΙΣ
   17: 3 ΑΝΤΙΤΥΠΑ
 - 0: 7329
   1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   2: ΕΥΘΑΛΗΣ ΚΛΩΝΟΣ
   4: 889.1ΜΠΟ
-  5: 9245Α
+  5: 09245
   8: UNIVERSITY STUDIO PR
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2001'
   11: 88Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   15: ΠΟΙΗΜΑΤΑ
   18: 960-12-095
   19: 0-6
 - 0: 7330
   1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   2: ΕΛΙΞ ΤΗΣ ΓΑΛΑΞΙΑΚΗΣ ΔΟΜΗΣ
   4: 889.1ΜΠΟ
-  5: 9241Α
+  5: 09241
   8: UNIVERSITY STUDIO PR
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '1998'
   11: 62Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   15: ΠΟΙΗΜΑΤΑ
   18: 960-12-071
   19: 0-4
 - 0: 7331
   1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   2: ΡΙΖΑ ΑΠΟ ΑΛΜΗ
   4: 889.1ΜΠΟ
-  5: 9244Α
+  5: 09244
   8: UNIVERSITY STUDIO PR
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2001'
   11: 51Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   15: ΠΟΙΗΜΑΤΑ
   18: 960-12-094
   19: 8-4
 - 0: 7332
   1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   2: Η ΝΥΧΤΑ ΤΗΣ ΑΥΓΗΣ
   4: 889.1ΜΠΟ
-  5: 9243Α
+  5: 09243
   8: UNIVERSITY STUDIO PR
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2001'
   11: 59Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   15: ΠΟΙΗΜΑΤΑ
   18: 960-12-094
   19: 5-Χ
 - 0: 7333
   1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   2: ΦΩΤΟΣΥΝΘΕΣΗ-ΦΩΤΟΔΙΑΧΥΣΗ
   4: 889.1ΜΠΟ
-  5: 9242Α
+  5: 09242
   8: UNIVERSITY STUDIO PR
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2001'
   11: 50Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   15: ΠΟΙΗΜΑΤΑ
   18: 960-12-094
   19: 1-7
 - 0: 7334
   1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   2: ΑΝΑΖΗΤΩΝΤΑΣ ΤΟ ΑΠΟΛΥΤΟ
   4: 889.1ΜΠΟ
-  5: 9232Α
+  5: 09232
   8: UNIVERSITY STUDIO PR
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2007'
   11: 209Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   15: ΠΟΙΗΜΑΤΑ
   18: 978-960-12
   19: -1659-1
 - 0: 7335
   1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   2: ΔΙΑΥΛΟΣ ΖΩΗΣ
   4: 889.1ΜΠΟ
-  5: 9234Α
+  5: 09234
   8: UNIVERSITY STUDIO PR
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2001'
   11: 83Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   15: ΠΟΙΗΜΑΤΑ
   18: 960-12-094
   19: 7-6
 - 0: 7336
   1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   2: ΒΟΜΒΑ ΥΔΡΟΓΟΝΟΥ ΤΗΣ ΕΛΕΥΘΕΡΙΑΣ
   4: 889.1ΜΠΟ
-  5: 9230Β
+  5: 09230
   8: UNIVERSITY STUDIO PR
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '1998'
   11: 77Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   15: ΠΟΙΗΜΑΤΑ
   18: 960-12-071
   19: 2-0
 - 0: 7337
   1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   2: ΣΚΟΤΩΜΕΝΟ ΑΙΜΑ
   4: 889.1.ΜΠΟ
-  5: 9231Β
+  5: 09231
   8: UNIVERSITY STUDIO PR
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '1998'
   11: 102Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   15: ΠΟΙΗΜΑΤΑ
   18: 960-12-071
   19: 1-2
 - 0: 7338
   1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   2: ΗΛΙΟΣ ΠΟΥ ΑΠΟ ΤΗ ΓΗ ΦΩΤΑ
   4: 889.1ΜΠΟ
-  5: 9237Α
+  5: 09237
   8: UNIVERSITY STUDIO PR
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2001'
   11: 102Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   18: 960-12-093
   19: 9-5
 - 0: 7339
   1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   2: ΠΑΝΘΕΟΝ-ΕΠΙΤΑΞΙΣ-ΝΤΟΜΙΝΟ
   4: 889.1ΜΠΟ
-  5: 9236Α
+  5: 09236
   8: UNIVERSITY STUDIO PR
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2003'
   11: 206Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   15: ΠΟΙΗΜΑΤΑ
   18: 960-91636-
   19: 6-1
 - 0: 7340
   1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   2: ΓΑΛΑΖΙΟ ΠΑΡΑΘΥΡΟ ΘΕΣΦΑΤΑ
   4: 889.1ΜΠΟ
-  5: 9235Α
+  5: 09235
   8: Α.Α.ΑΛΤΙΝΤΖΗΣ
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2003'
   11: 188Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   15: ΠΟΙΗΜΑΤΑ
   18: 960-91636-
   19: 5-3
 - 0: 7341
   1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   2: ΝΕΑ ΓΗ-ΝΙΚΗ ΖΩΗΣ
   4: 889.1ΜΠΟ
-  5: 9233Α
+  5: 09233
   8: UNUIVERSITY STUDIO P
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2007'
   11: 147Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   15: ΠΟΙΗΜΑΤΑ
   18: 978-960-12
   19: -1658-4
 - 0: 7342
   1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   2: ΔΕΚΑ ΚΑΙ ΟΚΤΩ ΚΥΚΛΟΙ ΕΚΛΕΙΣΑΝ
   4: 889.1ΜΠΟ
-  5: 9240Α
+  5: 09240
   8: UNIVERSITY STUDIO PR
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2001'
   11: 55Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   15: ΠΟΙΗΜΑΤΑ
   18: 960-12-094
   19: 2-5
 - 0: 7343
   1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   2: ΚΡΥΣΤΑΛΛΩΣΙΣ ΚΡΑΔΑΣΜΩΝ
   4: 889.1ΜΠΟ
-  5: 9239Α
+  5: 09239
   8: UNIVERSITY STUDIO PR
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '2001'
   11: 65Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   15: ΠΟΙΗΜΑΤΑ
   18: 960-12-094
   19: 4-1
 - 0: 7344
   1: ΜΠΟΜΠΟΤΗ,ΘΕΟΧΑΡΟΥΛΑ
   2: ΡΑΔΙΕΝΕΡΓΕΙΑ
   4: 889.1ΜΠΟ
-  5: 9238Α
+  5: 09238
   8: UNIVERSITY STUDIO PR
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '1998'
   11: 54Σ
   12: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ-ΠΟΙΗΜΑΤΑ
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   14: ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
@@ -90183,14 +90039,15 @@
   17: 2 ΑΝΤΙΤΥΠΑ
   18: 978-960-71
   19: 65-03-9
 - 0: 7353
   1: ΜΑΡΕΣ,ΝΤΕΛΙΑ
   2: ΓΝΩΡΙΣΤΕ ΤΟΝ ΚΟΜΜΟΥΝΙΣΜΟ
   4: 335.430ΜΑΡ
+  5: '9437'
   11: 92Σ
   12: ΚΟΜΜΟΥΝΙΣΜΟΣ
   13: ΜΑΡΞ-ΛΕΝΙΝ-ΣΤΑΛΙΝ
   14: ΚΟΥΜΜΟΥΝΙΣΜΟΣ
 - 0: 7354
   1: ΠΑΠΑΚΩΝΣΤΑΝΤΙΝΟΥ,ΘΕΟΦ
   2: ΠΟΛΙΤΙΚΗ ΑΓΩΓΗ
@@ -90214,15 +90071,15 @@
   12: ΦΙΛΟΣΟΦΙΑ-ΓΑΜΟΣ
   13: ΓΑΜΟΣ-ΦΙΛΟΣΟΦΙΑ
   14: ΦΙΛΟΣΟΦΙΑ
 - 0: 7356
   1: ΣΕΒΑΣΤΙΑΝΟΥ
   2: Η ΕΣΤΑΥΡΩΜΕΝΗ ΗΠΕΙΡΟΣ
   4: 938.936ΣΕΒ
-  5: 9285Α-8422
+  5: 8422-09285
   9: ΑΘΗΝΑ
   10: '1985'
   11: 189Σ
   12: ΒΟΡΕΙΟΣ ΗΠΕΙΡΟΣ
   13: ΒΟΡΕΙΟΣ ΗΠΕΙΡΟΣ
   14: ΒΟΡΕΙΟΣ ΗΠΕΙΡΟΣ
 - 0: 7357
@@ -90782,15 +90639,15 @@
   18: 978-960-56
   19: 0-089-1
 - 0: 7399
   1: ΚΑΡΖΗ,ΘΟΔΩΡΟΥ
   2: ΟΙ ΠΑΤΡΙΔΕΣ ΤΩΝ ΕΛΛΗΝΩΝ
   3: ΜΙΚΡΑ ΑΣΙΑ-ΠΟΝΤΟΣ
   4: 938.393ΚΑΡ
-  5: 9292Α
+  5: 09292
   8: ΛΙΒΑΝΗ
   9: ΑΘΗΝΑ
   10: '2002'
   11: 147Σ
   12: ΙΣΤΟΡΙΑ-Μ.ΑΣΙΑ-ΠΟΝΤΟΣ
   13: Μ.ΑΣΙΑ-ΠΟΝΤΟΣ
   14: ΠΟΝΤΟΣ-Μ,ΑΣΙΑ
@@ -90798,15 +90655,15 @@
   18: 960-14-045
   19: 3-8
 - 0: 7400
   1: ΚΑΡΖΗ,ΘΟΔΩΡΟΥ
   2: ΟΙ ΠΑΤΡΙΔΕΣ ΤΩΝ ΕΛΛΗΝΩΝ
   3: ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ
   4: 938.393ΚΑΡ
-  5: 9292Α
+  5: 09292
   8: ΛΙΒΑΝΗ
   9: ΑΘΗΝΑ
   10: '2002'
   11: 254Σ
   12: ΙΣΤΟΡΙΑ-ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ
   13: ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ-ΙΣΤΟΡΙΑ
   14: ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΗ
@@ -90814,15 +90671,15 @@
   18: 960-14-04
   19: 53-8
 - 0: 7401
   1: ΚΑΡΖΗ,ΘΟΔΩΡΟΥ
   2: ΟΙ ΠΑΤΡΙΔΕΣ ΤΩΝ ΕΛΛΗΝΩΝ
   3: ΠΕΛΑΓΟΝΙΑ-ΒΟΡΕΙΑ ΗΠΕΙΡΟΣ
   4: 938.393ΚΑΡ
-  5: 9292Α
+  5: 09292
   8: ΛΙΒΑΝΗ
   9: ΑΘΗΝΑ
   10: '2002'
   11: 386Σ
   12: ΙΣΤΟΡΙΑ-ΠΕΛΑΓΟΝΙΑ-ΒΟΡΕΙΑ ΗΠΕΙΡΟΣ
   13: ΠΕΛΑΓΟΝΙΑ-ΒΟΡΕΙΑ ΗΠΕΙΡΟΣ
   14: ΙΣΤΟΡΙΑ
@@ -90901,41 +90758,41 @@
   18: 960-7122-7
   19: 3-9
 - 0: 7407
   1: ΣΙΔΕΡΗΣ,Ι
   2: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΙΣ ΚΑΙ ΕΘΝΙΚΗ ΜΕΙΟΔΟΣΙΑ
   3: ΧΡΟΝΙΚΟΝ 1941-1944
   4: 938.764ΣΙΔ
-  5: 9289Α
+  5: 09289
   8: ΣΙΔΕΡΗΣ
   9: ΑΘΗΝΑ
   10: '1983'
   11: 440Σ
   12: ΙΣΤΟΡΙΑ-ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
   13: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ-ΙΣΤΟΡΙΑ
   14: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
 - 0: 7408
   1: ΒΙΔΑΛΗΣ,ΟΡΕΣΤΗΣ
   2: ΙΣΤΟΡΙΚΟ ΗΜΕΡΟΛΟΓΙΟ
   3: ΧΡΟΝΙΑ ΕΚΠΑΤΡΙΣΜΟΥ 1968-1975
   4: 938.790ΒΙΔ
-  5: 4288,4292
+  5: 4288-4292
   8: LIBRO
   9: ΑΘΗΝΑ
   10: '1997'
   11: '570'
   12: ΙΣΤΟΡΙΑ-ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
   13: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ-ΙΣΤΟΡΙΑ
   14: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
 - 0: 7409
   1: Χ.Σ.
   2: ΜΕΓΑΛΗ ΕΛΛΑΔΑ
   3: ΠΕΡΙΟΔΟΣ 1944-1945
   4: 938.752Χ.Σ
-  5: 9283Α-6759-5007
+  5: 09283-6759-5007
   9: ΑΘΗΝΑ
   10: '1998'
   11: 135Σ
   12: ΙΣΤΟΡΙΑ-ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
   13: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ-ΙΣΤΟΡΙΑ
   14: ΕΘΝΙΚΗ ΑΝΤΙΣΤΑΣΗ
   17: 3 ΑΝΤΙΤΥΠΑ
@@ -91282,30 +91139,30 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΑΦΗΓΗΜΑΤΑ
   13: ΑΦΗΓΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΒΙΒΛΙΟΘΗΚΗ ΓΑΡΟΥΦΑΛΙΑ
 - 0: 7438
   1: ΑΝΝΙΝΟΣ, ΜΠΑΜΠΗΣ
   2: Η ΑΠΟΛΟΓΙΑ ΤΟΥ ΟΔΥΣΣΕΩΣ ΑΝΔΡΟΥΤΣΟΥ
   4: 889ΑΝΝ
-  5: 9919,9917
+  5: 9919-9917
   7: 2Η
   8: ΓΑΛΑΞΙΑΣ
   9: ΑΘΗΝΑ
   10: '1969'
   11: 133Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΚΑ ΣΗΜΕΙΩΜΑΤΑ
   13: ΙΣΤΟΡΙΚΑ ΣΗΜΕΙΩΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΒΙΒΛΙΟΘΗΚΗ ΓΑΡΟΥΦΑΛΙΑ
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 7439
   1: ΑΝΝΙΝΟΣ,ΜΠΑΜΠΗΣ
   2: ΑΙ ΑΘΗΝΑΙ ΤΟΥ 1850
   3: ΕΚΤΥΠΩΣΕΙΣ ΔΥΟ ΓΑΛΛΩΝ ΠΕΡΙΗΓΗΤΩΝ
   4: 889ΑΝΝ
-  5: 9918,9916
+  5: 9918-9916
   8: ΓΑΛΑΞΙΑΣ
   9: ΑΘΗΝΑ
   10: '1971'
   11: 127Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΚΑ ΣΗΜΕΙΩΜΑΤΑ
   13: ΙΣΤΟΡΙΚΑ ΣΗΜΕΙΩΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΒΙΒΛΙΟΘΗΚΗ ΓΑΡΟΥΦΑΛΙΑ
@@ -91480,15 +91337,15 @@
   13: ΠΟΙΗΜΑΤΑ-ΕΛΛΗΝΙΚΗ ΠΟΙΗΣΗ
   17: ΒΙΒΛΙΟΘΗΚΗ ΓΑΡΟΥΦΑΛΙΑ
 - 0: 7453
   1: ΞΕΝΟΦΩΝΤΑΣ
   2: ΕΛΛΗΝΙΚΑ
   3: ΤΟΜΟΣ ΠΡΩΤΟΣ Α-Γ
   4: 180ΞΕΝ
-  5: 9926,9914
+  5: 9926-9914
   6: ΡΟΥΦΟΥ.ΡΟΔΗ
   8: ΓΑΛΑΞΙΑΣ
   9: ΑΘΗΝΑ
   10: '1966'
   11: 151Σ
   12: ΑΡΧΑΙΟΙ ΣΥΓΓΡΑΦΕΙΣ-ΞΕΝΟΦΩΝΤΑΣ
   13: ΞΕΝΟΦΩΝΤΑΣ-ΑΡΧΑΙΟΙ ΣΥΓΓΡΑΦΕΙΣ
@@ -91770,15 +91627,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΒΙΒΛΙΟΘΗΚΗ ΓΑΡΟΥΦΑΛΙΑ
 - 0: 7474
   1: ΧΡΗΣΤΟΜΑΝΟΣ, ΚΩΝΣΤΑΝΤΙΝΟΣ
   2: Η ΚΕΡΕΝΙΑ ΚΟΥΚΛΑ
   4: 889.21ΧΡΗ
-  5: 8742,9948
+  5: 8742-9948
   8: ΓΑΛΑΞΙΑΣ
   9: ΑΘΗΝΑ
   10: '1969'
   11: 176Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΒΙΒΛΙΟΘΗΚΗ ΓΑΡΟΥΦΑΛΙΑ
@@ -91947,16 +91804,16 @@
   13: ΑΠΟΜΝΗΜΟΝΕΥΜΑΤΑ-ΓΑΛΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΒΙΒΛΙΟΘΗΚΗ ΓΑΡΟΥΦΑΛΙΑ
   30: ΒΕΠ 1
 - 0: 7488
   1: ΡΑΝΣΙΜΑΝ, ΣΤ
   2: ΑΛΩΣΗ ΚΩΝΣΤΑΝΤΙΝΟΥΠΟΛΕΩΣ 1453
   4: 938.389ΡΑΝ
-  5: 9957-1997-1998-2848-
-  6: 2847 ΠΑΠΑΡΡΟΔΟΥ,ΝΙΚ
+  5: 9957-1997-1998-2848
+  6: ΠΑΠΑΡΡΟΔΟΥ,ΝΙΚ
   8: ΜΠΕΡΓΑΔΗ
   9: ΑΘΗΝΑ
   10: '1972'
   11: 189Σ
   12: ΛΟΓΟΤΕΧΝΙΑ-ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ-ΛΟΓΟΤΕΧΝΙΑ
   17: ΒΙΒΛΙΟΘΗΚΗ ΓΑΡΟΥΦΑΛΙΑ
@@ -95539,15 +95396,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΙΣΤΟΡΙΚΟ ΜΥΘΙΣΤΟΡΗΜΑ
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
 - 0: 7819
   1: ΖΗΚΟΥ ΜΑΙΡΗ
   2: Η ΠΡΟΣΤΥΧΗ
   4: 889.21ΖΗΚ
-  5: 9160Α
+  5: 09160
   8: ΜΟΝΤΕΡΝΟΙ ΚΑΙΡΟΙ
   9: ΑΘΗΝΑ
   10: '2007'
   11: 264Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
@@ -97556,15 +97413,15 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
 - 0: 7978
   1: ΧΟΚ ΙΘΑΝ
   2: ΑΛΗΘΙΝΗ ΑΓΑΠΗ
   4: 810.11ΧΟΚ
-  5: 9220Α
+  5: 09220
   6: ΠΕΡΣΑ ΚΟΥΜΟΥΤΣΗ
   8: ΕΜΠΕΙΡΙΑ
   9: ΑΘΗΝΑ
   10: '2003'
   11: 267Σ
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -98911,31 +98768,36 @@
   12: ΙΣΤΟΡΙΚΟ ΘΕΑΤΡΟ
   13: ΘΕΑΤΡΙΚΟ ΕΡΓΟ
   14: ΘΕΑΤΡΟ
 - 0: 8092
   1: ΔΡΑΚΟΠΟΥΛΟΣ ΓΕΩΡΓΙΟΣ ΚΥΡΙΑΚΟΣ
   2: ΑΙΣΘΗΤΙΚΗ ΑΓΩΓΗ ΤΗΣ ΤΗΛΕΟΡΑΣΗΣ
   4: 800.203ΔΡΑ
-  5: 7984-9276Α
+  5: 7984-09276
   7: ΠΡΩΤΗ
   8: ΚΑΜΙΝΑ
   9: ΙΩΑΝΝΙΝΑ
   10: '1976'
   11: '104'
+  12: ΤΗΛΕΟΡΑΣΗ
+  13: ΑΙΣΘΗΤΙΚΗ ΑΓΩΓΗ
+  14: ΤΗΛΕΟΡΑΣΗ
   17: 4 ΑΝΤΙΤΥΠΑ
 - 0: 8093
   1: ΔΡΑΚΟΠΟΥΛΟΣ ΓΕΩΡΓΙΟΣ ΚΥΡΙΑΚΟΣ
   2: ΑΙ ΜΟΥΣΙΚΑΙ ΤΕΧΝΑΙ ΚΑΙ ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
   4: 800.203ΔΡΑ
   5: '9275'
   7: Β
   8: ΧΑΡΤΟΤΥΠΟΓΡΑΦΙΚΗ
   9: ΑΓΡΙΝΙΟΧΑΡ
   10: '1969'
   11: 120Σ
+  12: ΜΟΥΣΙΚΕΣ ΤΕΧΝΕΣ
+  13: ΚΙΝΗΜΑΤΟΓΡΑΦΟΣ
   17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 8094
   1: ΧΑΤΖΟΠΟΥΛΟΥ ΣΟΦΙΑ
   2: Η ΜΙΣΗΤΗ ΕΙΚΟΝΑ
   4: 886.2ΧΑΤ
   5: '7936'
   8: ΜΕΛΙΣΣΑ
@@ -100223,15 +100085,15 @@
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-234-03
   19: 4-7
 - 0: 8204
   1: ΚΟΚΟΡΕΛΗ ΑΡΓΥΡΩ-ΖΩΡΖ ΣΑΡΗ
   2: ΜΙΑ ΑΓΑΠΗ ΓΙΑ ΔΥΟ
   4: 808.899ΚΟΚ
-  5: 9201Α
+  5: 09201
   7: '12'
   8: ΠΑΤΑΚΗ
   9: ΑΘΗΝΑ
   10: '2007'
   11: 171Σ
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -101288,159 +101150,159 @@
   13: ΠΕΡΙΟΔΙΚΗ ΕΚΔΟΣΗ
   14: ΛΑΟΓΡΑΦΙΑ
   17: 5 ΤΟΜΟΙ
 - 0: 8295
   1: Χ.Σ.
   2: ΗΠΕΙΡΟΣ
   4: 398 Χ.Σ
-  5: 9278Α
+  5: 09278
   9: ΘΕΣ\ΝΙΚΗ
   10: '1978'
   11: 64Σ
   12: ΛΑΟΓΡΑΦΙΑ
   13: ΠΕΡΙΟΔΙΚΗ ΕΚΔΟΣΗ
   14: ΛΑΟΓΡΑΦΙΑ
 - 0: 8296
   1: Χ.Σ.
   2: ΗΠΕΙΡΟΣ
-  4: 398 Χ.Σ.
+  4: 398Χ.Σ.
   5: '10544'
   9: ΘΕΣ\ΝΙΚΗ
   10: '1981'
   11: 121Σ
   12: ΠΕΡΙΟΔΙΚΗ ΕΚΔΟΣΗ
   13: ΛΑΟΓΡΑΦΙΑ
   14: ΛΑΟΓΡΑΦΙΑ
 - 0: 8297
   1: ΑΚΟΓΛΟΥ ΞΕΝΟΦΩΝΤΑΣ
   2: ΑΠΟ ΤΗ ΖΩΗ ΤΟΥ ΠΟΝΤΟΥ
   3: ΛΑΟΓΡΑΦΙΚΑ ΚΟΤΥΩΡΩΝ
-  4: 398 ΑΚΟ
+  4: 398ΑΚΟ
   5: '10545'
   8: ΞΕΝΟΣ
   9: ΑΘΗΝΑ
   10: '1939'
   11: 532Σ
   12: ΛΑΟΓΡΑΦΙΑ
   13: ΛΑΟΓΡΑΦΙΑ
   14: ΛΑΟΓΡΑΦΙΑ
 - 0: 8298
   1: ΜΕΡΑΝΤΖΑΣ ΧΡΗΣΤΟΣ
   2: ΠΡΑΚΤΙΚΑ Α ΕΠΙΣΤΗΜΟΝΙΚΟΥ ΣΥΝΕΔΡΙΟΥ ΓΙΑ ΤΑ ΤΖΟΥΜΕΡΚΑ
-  4: 398 ΜΕΡ
+  4: 398ΜΕΡ
   5: '10546'
   8: ΙΚΛΕΤ
   9: ΙΩΑΝΝΙΝΑ
   10: '2008'
   11: 512Σ
   12: ΛΑΟΓΡΑΦΙΑ
   13: ΛΑΟΓΡΑΦΙΑ
   14: ΛΑΟΓΡΑΦΙΑ
 - 0: 8299
   1: ΑΥΔΙΚΟΣ ΕΥΑΓΓΕΛΟΣ
   2: ΠΡΕΒΕΖΑ
   3: 1945-1990
-  4: 398 ΑΥΔ
+  4: 398ΑΥΔ
   5: '9550'
   8: ΔΗΜΟΣ ΠΡΕΒΕΖΑΣ
   9: ΠΡΕΒΕΖΑ
   10: '2000'
   11: 457Σ
   12: ΛΑΟΓΡΑΦΙΑ
   13: ΛΑΟΓΡΑΦΙΑ
   14: ΛΑΟΓΡΑΦΙΑ
 - 0: 8300
   1: Χ.Σ.
   2: ΣΑΡΑΚΑΤΣΑΝΟΙ
-  4: 398 Χ.Σ.
+  4: 398Χ.Σ.
   5: '9899'
   8: ΠΗΓΑΣΟΣ
   11: 142Σ
   12: ΛΑΟΓΡΑΦΙΑ
   13: ΛΑΟΓΡΑΦΙΑ
   14: ΛΑΟΓΡΑΦΙΑ
 - 0: 8301
   1: ΚΟΛΙΟΣ ΑΠΟΣΤΟΛΟΣ
   2: ΛΕΛΟΒΑ 1941
   3: ΕΝΑΣ ΠΑΠΠΟΥΣ ΘΥΜΑΤΑΙ
-  4: 398 ΚΟΛ
+  4: 398ΚΟΛ
   5: '10549'
   8: ΡΟΚΟΣ
   9: ΠΡΕΒΕΖΑ
   10: '2009'
   11: 102Σ
   12: ΛΑΟΓΡΑΦΙΑ
   13: ΛΑΟΓΡΦΑΙΑ
   14: ΛΑΟΓΡΑΦΙΑ
 - 0: 8302
   1: ΒΙΓΛΑΣ ΙΩΑΝΝΗΣ
   2: ΣΑΡΑΝΤΑΠΕΝΤΕ ΓΙΑΝΝΗΔΕΣ...
   3: ΗΘΟΓΡΑΦΙΑ
-  4: 398 ΒΙΓ
+  4: 398ΒΙΓ
   5: '10548'
   8: ΓΡΑΦΙΚΕΣ ΤΕΧΝΕΣ
   9: ΑΘΗΝΑ
   10: '1995'
   11: 191Σ
   12: ΛΑΟΓΡΑΦΙΑ
   13: ΛΑΟΓΡΑΦΙΑ
   14: ΛΑΟΓΡΑΦΙΑ
 - 0: 8303
   1: Χ.Σ.
   2: ΤΖΟΥΜΕΡΚΙΩΤΙΚΑ ΧΡΟΝΙΚΑ
-  4: 398 Χ.Σ.
+  4: 398Χ.Σ.
   5: '10551'
   8: ΝΑΙ
   9: ΙΩΑΝΝΙΝΑ
   10: '2009'
   11: 224Σ
   12: ΛΑΟΓΡΑΦΙΑ
   13: ΠΕΡΙΟΔΙΚΗ ΕΚΔΟΣΗ
   14: ΛΑΟΓΡΑΦΙΑ
 - 0: 8304
   1: ΜΑΚΡΥΓΙΑΝΝΗΣ ΧΡΗΣΤΟΣ ΚΑΙ ΑΘΑΝΑΣΙΟΣ
   2: ΙΣΤΟΡΙΟΓΡΑΦΙΑ ΤΗΣ ΠΙΝΔΟΥ
-  4: 398 ΜΑΚ
+  4: 398ΜΑΚ
   5: '10547'
   8: ΔΗΜΟΣ ΑΓΝΑΝΤΩΝ
   9: ΑΘΗΝΑ
   10: '2010'
   11: 252Σ
   12: ΛΑΟΓΡΑΦΙΑ
   13: ΛΑΟΓΡΑΦΙΑ
   14: ΛΑΟΓΡΑΦΙΑ
-  17: 2 αντιτυπα
+  17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 8305
   1: ΤΣΙΠΑΣ ΝΙΚΟΛΑΟΣ
   2: ΣΕΡΓΙΑΝΙΣΜΑ ΣΤΟΥΣ ΧΩΡΟΥΣ ΚΑΙ ΣΤΗΝ ΙΣΤΟΡΙΑ ΤΗΣ ΠΥΡΣΟΓΙΑΝΝΗΣ
-  4: 398 ΤΣΙ
+  4: 398ΤΣΙ
   5: '10550'
   9: ΜΑΡΟΥΣΙ
   10: '1995'
   11: 143Σ
   12: ΛΑΟΓΡΑΦΙΑ
   13: ΛΑΟΓΡΑΦΙΑ
   14: ΛΑΟΓΡΑΦΙΑ
 - 0: 8306
   1: ΚΙΚΟΠΟΥΛΟΣ ΜΕΝΕΛΑΟΣ
   2: ΕΛΑΦΟΤΟΠΟΣ (ΤΣΕΡΒΑΡΙ)
-  4: 398 ΚΙΚ
+  4: 398ΚΙΚ
   5: '5340'
   8: ΔΟΥΒΑΛΗ
   9: ΓΙΑΝΝΕΝΑ
   10: '2000'
   11: 462Σ
   12: ΛΑΟΓΡΑΦΙΑ
   13: ΛΑΟΓΡΑΦΙΑ
   14: ΛΑΟΓΡΑΦΙΑ
   17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 8307
   1: ΝΙΚΟΛΣ ΚΩΣΤΑ
   2: Ο ΧΟΡΟΣ-Η ΙΣΤΟΡΙΑ ΜΙΑΣ ΤΕΧΝΗΣ:ΤΟ ΜΠΑΛΛΕΤΟ
-  4: 398 ΝΙΚ
+  4: 398ΝΙΚ
   5: '957'
   8: ΔΙΦΡΟΣ
   9: ΑΘΗΝΑ
   10: '1957'
   11: 206Σ
   12: ΜΠΑΛΛΕΤΟ-ΧΟΡΟΣ
   13: ΛΑΟΓΡΑΦΙΑ
@@ -102404,88 +102266,88 @@
   11: 433Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
   18: 978-960-45
   19: 3-353-4
 - 0: 8391
-  1: ΠΑΜΟΥΚ ΟΡΧΑΝ
+  1: ΠΑΜΟΥΚ,ΟΡΧΑΝ
   2: ΧΙΟΝΙ
   4: 894.35 ΠΑΜ
-  5: 9158Α
+  5: 09158
   6: ΣΤΕΛΛΑ ΒΡΕΤΟΥ
   8: ΩΚΕΑΝΙΔΑ
   9: ΑΘΗΝΑ
   10: '2007'
   11: 686Σ
   12: ΤΟΥΡΚΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΤΟΥΡΚΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
   18: 978-960-41
   19: 0-468-0
 - 0: 8392
-  1: ΚΑΛΠΟΥΖΟΣ ΓΙΑΝΝΗΣ
+  1: ΚΑΛΠΟΥΖΟΣ,ΓΙΑΝΝΗΣ
   2: ΠΑΝΤΟΜΙΜΑ ΦΑΝΤΑΣΜΑΤΩΝ
   4: 889.21ΚΑΛ
   5: '9162'
   8: ΑΓΚΥΡΑ
   9: ΑΘΗΝΑ
   10: '2005'
   11: 506Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΗΠΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
   18: 960-422-24
   19: 4-9
 - 0: 8393
-  1: COELHO PAULO
+  1: COELHO,PAULO
   2: ΟΙ ΕΞΟΜΟΛΟΓΗΣΕΙΣ ΕΟΣ ΠΡΟΣΚΥΝΗΤΗ
   4: 869 COE
   5: '9592'
   6: ΚΑΛΑΤΖΟΠΟΥΛΟΥ ΚΑΤΕΡΙ
   8: ΛΙΒΑΝΗ
   9: ΑΘΗΝΑ
   10: '2001'
   11: '312'
   12: ΒΡΑΖΙΛΙΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
   18: 960-14-035
   19: 8-2
 - 0: 8394
-  1: ΠΑΠΑΒΑΣΙΛΕΙΟΥ ΙΩΑΝΝΗΣ
+  1: ΠΑΠΑΒΑΣΙΛΕΙΟΥ,ΙΩΑΝΝΗΣ
   2: Η ΕΘΝΙΚΗ ΜΑΣ ΓΛΩΣΣΑ
   3: ΜΙΚΡΗ ΙΣΤΟΡΙΚΗ ΑΝΑΔΡΟΜΗ
   4: 938.031ΠΑΠ
   5: 2861-2862
   9: ΑΘΗΝΑ
   10: '1971'
   11: 31Σ
   12: ΙΣΤΟΡΙΑ
   13: ΙΣΤΟΡΙΑ
   14: ΙΣΤΟΡΙΑ
   17: 2 ΑΝΤΙΤΥΠΑ
 - 0: 8395
-  1: ΓΟΥΕΣΤΕΡΦΕΛΝΤ ΣΚΟΤ
+  1: ΓΟΥΕΣΤΕΡΦΕΛΝΤ,ΣΚΟΤ
   2: UGLIES
-  4: 810.11 ΓΟΥ
+  4: 810.11ΓΟΥ
   5: '10620'
   6: ΟΙΚΟΝΟΜΟΙ ΚΑΙΤΗ
   8: ΜΕΤΑΙΧΜΙΟ
   9: ΑΘΗΝΑ
   10: '2009'
   11: 462Σ
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
   17: 2 ΑΝΤΙΤΥΠΑ
   18: 978-960-45
   19: 5-674-8
 - 0: 8396
-  1: ΠΑΧΟΡ ΠΟΡΙΣ
+  1: ΠΑΧΟΡ,ΠΟΡΙΣ
   2: ΑΠΑΓΟΡΕΥΕΤΑΙ ΤΟ ΟΜΙΛΕΙΝ
   4: 891.84ΠΑΧ
   5: '10619'
   6: ΤΕΡΕΖΑ ΒΕΚΙΑΡΗΛΛΗ
   8: ΜΕΤΑΙΧΜΙΟ
   9: ΑΘΗΝΑ
   10: '2009'
@@ -102494,46 +102356,46 @@
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΣΛΟΒΕΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΗΡΜΑ
   17: 2 ΑΝΤΙΤΥΠΑ
   18: 978-960-96
   19: 0-455-647-
   22: '2'
 - 0: 8397
-  1: ΓΚΟΝΤΕ ΛΟΡΑΝ
+  1: ΓΚΟΝΤΕ,ΛΟΡΑΝ
   2: Η ΠΥΛΗ ΤΗΣ ΚΟΛΑΣΕΩΣ
-  4: 843 ΓΚΟ
+  4: 843ΓΚΟ
   5: '10618'
   6: ΕΥΗ ΣΙΟΥΓΓΑΡΗ
   8: ΜΕΤΑΙΧΜΙΟ
   9: ΑΘΗΝΑ
   10: '2008'
   11: 199Σ
   12: ΓΑΛΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΓΑΛΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
   17: 2 ΑΝΤΙΤΥΠΑ
   18: 978-960-45
   19: 5-642-7
 - 0: 8398
-  1: ΕΛΕΥΘΕΡΙΟΥ ΜΑΝΟΣ
+  1: ΕΛΕΥΘΕΡΙΟΥ,ΜΑΝΟΣ
   2: Η ΜΕΛΑΓΧΟΛΙΑ ΤΗΣ ΠΑΤΡΙΔΑΣ ΜΕΤΑ ΤΙΣ ΕΙΔΗΣΕΙΣ ΤΩΝ ΟΚΤΩ
-  4: 889.21 ΕΛΕ
+  4: 889.21ΕΛΕ
   5: '10615'
   8: ΜΕΤΑΙΧΜΙΟ
   9: ΑΘΗΝΑ
   10: '2007'
   11: 235Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΜΑ
   17: 2 ΑΝΤΙΤΥΠΑ
   18: 978-960-45
   19: 5-268-9
 - 0: 8399
-  1: ΑΚΡΙΒΟΣ ΚΩΣΤΑΣ
+  1: ΑΚΡΙΒΟΣ,ΚΩΣΤΑΣ
   2: ΤΕΛΕΤΕΣ ΕΝΗΛΙΚΙΩΣΗΣ
   3: ΜΙΑ ΖΩΗ ΣΕ ΔΕΚΑΕΦΤΑ ΕΠΕΙΣΟΔΙΑ
   4: 889.21ΑΚΡ
   5: 10621-16720
   8: ΜΕΤΑΙΧΜΙΟ
   9: ΑΘΗΝΑ
   10: '2009'
@@ -102541,46 +102403,46 @@
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
   17: 2 ΑΝΤΙΤΥΠΑ
   18: 978-960-45
   19: 5-536-9
 - 0: 8400
-  1: ΕΛΕΥΘΕΡΙΟΥ ΜΑΝΟΣ
+  1: ΕΛΕΥΘΕΡΙΟΥ,ΜΑΝΟΣ
   2: ΑΝΘΡΩΠΟΣ ΣΤΟ ΠΗΓΑΔΙ
-  4: 889.21 ΕΛΕ
+  4: 889.21ΕΛΕ
   5: '10622'
   8: ΜΕΤΑΙΧΜΙΟ
   9: ΑΘΗΝΑ
   10: '2008'
   11: 267Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΡΗΜΑ
   13: ΜΥΘΙΣΤΟΡΗΜΑ-ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
   17: 2 ΑΝΤΙΤΥΠΑ
   18: 978-455-44
   19: 3-0
 - 0: 8401
-  1: ΝΤΕΙΒΙΝΤΣΟΝ ΙΑΝ
+  1: ΝΤΕΙΒΙΝΤΣΟΝ,ΙΑΝ
   2: ΤΑ ΤΕΛΕΥΤΑΙΑ ΧΡΟΝΙΑ ΤΟΥ ΒΟΛΤΑΙΡΟΥ
-  4: 190 NTE
+  4: 190NTE
   5: '10613'
   6: ΝΙΚΗ ΠΡΟΔΡΟΜΙΔΟΥ
   8: ΜΕΤΑΙΧΜΙΟ
   9: ΑΘΗΝΑ
   10: '2008'
   11: 295Σ
   12: ΒΙΟΓΡΑΦΙΑ ΒΟΛΤΑΙΡΟΥ
   13: ΒΙΟΓΡΑΦΙΑ
   14: ΒΙΟΓΡΑΦΙΑ
   17: 2 ΑΝΤΙΤΥΠΑ
   18: 978-960-45
   19: 5-649-6
 - 0: 8402
-  1: FEARN NICHOLAS
+  1: FEARN,NICHOLAS
   2: ΦΙΛΟΣΟΦΙΑ
   3: ΟΙ ΠΙΟ ΠΡΟΣΦΑΤΕΣ ΑΠΑΝΤΗΣΕΙΣ ΣΤΑ ΑΡΧΑΙΟΤΤΕΡΑ ΕΡΩΤΗΜΑΤΑ
   4: 100FEA
   5: '10616'
   6: ΣΕΒΥ ΣΠΥΡΙΔΟΓΙΑΝΝΑΚΗ
   8: ΜΕΤΑΙΧΜΙΟ
   9: ΑΘΗΝΑ
@@ -102589,17 +102451,17 @@
   12: ΦΙΛΟΣΟΦΙΑ
   13: ΦΙΛΟΣΟΦΙΑ
   14: ΦΙΛΟΣΟΦΙΑ
   17: 2 ΑΝΤΙΤΥΠΑ
   18: 978-960-45
   19: 5-670-0
 - 0: 8403
-  1: JOHNSON GEORGE
+  1: JOHNSON,GEORGE
   2: ΤΑ ΔΕΚΑ ΠΙΟ ΟΜΟΡΦΑ ΠΕΙΡΑΜΑΤΑ
-  4: 620.11 JOH
+  4: 620.11JOH
   5: '10614'
   6: ΓΙΩΡΓΟΣ ΜΠΑΡΟΥΞΗΣ
   8: ΜΕΤΑΙΧΜΙΟ
   9: ΑΘΗΝΑ
   10: '2008'
   11: 241Σ
   12: ΕΠΙΣΤΗΜΟΝΙΚΑ- ΦΥΣΙΚΗ
@@ -102609,73 +102471,73 @@
   17: 2 ΑΝΤΙΤΥΠΑ
   18: 978-960-45
   19: 5-671-7
 - 0: 8404
   1: ΤΑΤΣΟΠΟΥΛΟΣ ΠΕΤΡΟΣ
   2: ΝΕΟΕΛΛΗΝΕΣ
   3: ΠΟΡΤΡΕΤΑ
-  4: 889.21 ΤΑΤ
+  4: 889.21ΤΑΤ
   5: '10617'
   8: ΜΕΤΑΙΧΜΙΟ
   9: ΑΘΗΝΑ
   10: '2004'
   11: 383Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΕΤΧΝΙΑ
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: 2 ΑΝΤΙΤΥΠΑ
   18: 978-960-45
   19: 5-269-6
 - 0: 8405
-  1: ΚΟΥΡΚΟΥΜΕΛΗΣ Ν.Κ.
+  1: ΚΟΥΡΚΟΥΜΕΛΗΣ,Ν.Κ.
   2: ΠΡΑΚΤΙΚΑ ΗΜΕΡΙΔΩΝ 2009 ΚΑΙ2010
   4: 938.101ΚΟΥ
   5: '10623'
   8: ΦΙΛΟΙ ΒΙΒΛΙΟΘ ΑΛΕΞΑΝ
   9: ΑΘΗΝΑ
   10: '2011'
   11: 394Σ
   12: ΑΡΧΑΙΑ ΕΛΛΑΔΑ-ΠΡΑΚΤΙΚΑ
   13: ΠΡΑΚΤΙΚΑ-ΑΡΧΑΙΑ ΕΛΛΑΔΑ
   14: ΠΡΑΚΤΙΚΑ
 - 0: 8406
-  1: ΣΙΝΓΚΕΡ ΜΠΑΣΕΒΙΤΣ ΙΣΑΑΚ
+  1: ΣΙΝΓΚΕΡ,ΜΠΑΣΕΒΙΤΣ ΙΣΑΑΚ
   2: ΕΧΘΡΟΙ, ΜΙΑ ΕΡΩΤΙΚΗ ΙΣΤΟΡΙΑ
-  4: 839.73 ΣΙΝ
+  4: 839.73ΣΙΝ
   5: '10624'
   6: ΑΜΑΝΑΤΙΔΗΣ
   8: ΚΑΣΤΑΝΙΩΤΗΣ
   9: ΑΘΗΝΑ
   10: '2009'
   11: 308Σ
   12: ΠΟΛΩΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ-ΜΥΘΙΣΤΟΗΡΜΑ
   13: ΜΥΘΟΣΤΟΡΗΜΑ-ΠΟΛΩΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΜΥΘΙΣΤΟΡΗΜΑ
   18: 978-960-03
   19: -4872-9
 - 0: 8407
-  1: ΕΚΟ ΟΥΜΠΕΡΤΟ
+  1: ΕΚΟ,ΟΥΜΠΕΡΤΟ
   2: ΤΟ ΝΗΣΙ ΤΗΣ ΠΡΟΗΓΟΥΜΕΝΗΣ ΜΕΡΑΣ
-  4: 850.11 ΕΚΟ
+  4: 850.11ΕΚΟ
   5: '9591'
   6: ΚΑΛΛΙΦΑΤΙΔΗ
   8: ΕΛΛΗΝΙΚΗ ΓΡΑΜΜΑΤΑ
   9: ΑΘΗΝΑ
   10: '2004'
   11: 551ΣΕΛ
   12: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΙΤΑΛΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   18: 960-406-80
   19: 0-8
 - 0: 8408
-  1: ΚΟΡΝΑΡΟΣ ΘΕΜΟΣ-ΚΑΖΑΤΖΑΚΗ ΓΑΛΑΤΕΙΑ
+  1: ΚΟΡΝΑΡΟΣ,ΘΕΜΟΣ-ΚΑΖΑΤΖΑΚΗ ΓΑΛΑΤΕΙΑ
   2: ΤΟ ΝΗΣΙ ΤΩΝ ΣΗΜΑΔΕΜΕΝΩΝ
   3: ΣΠΙΝΑΛΟΓΚΑ-Η ΑΡΡΩΣΤΗ ΠΟΛΙΤΕΙΑ
-  4: 88921ΚΟΡ
+  4: 889.21ΚΟΡ
   5: '10625'
   7: '4'
   8: ΚΑΣΤΑΝΙΩΤΗ
   9: ΑΘΗΝΑ
   10: '2010'
   11: 209Σ
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -119639,15 +119501,15 @@
   17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
   18: 978-960-46
   19: 9-633-8
 - 0: 9621
   1: ΣΤΑΟΥΤ,ΡΕΞ
   2: ΠΑΡΑ ΠΟΛΛΕΣ ΓΥΝΑΙΚΕΣ
   4: 810.11ΣΤΑ
-  5: 11921(α)
+  5: '11921'
   6: Α.ΚΟΝΤΟΣΙΑΝΟΥ
   8: ΛΑΜΠΡΑΚΗ
   9: ΑΘΗΝΑ
   10: '2009'
   11: 264Σ
   12: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΑΜΕΡΙΚΑΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -124224,15 +124086,15 @@
   13: ΙΡΑΚ
   14: ΙΡΑΚ
   17: ΔΩΡΕΑ ΓΙΑΝΝΗ ΜΠΑΝΙΑ
 - 0: 10019
   1: ΑΝΔΡΟΥΛΑΚΗΣ,ΓΕΩΡΓΙΟΣ
   2: ΑΝΑΝΗΨΗ ΤΩΝ ΒΑΡΙΑ ΠΑΣΧΟΝΤΩΝ
   4: 615.5ΑΝΔ
-  5: 10793 Α
+  5: '10793'
   7: ΤΡΙΤΗ
   8: ΠΑΡΙΣΙΑΝΟΣ
   9: ΑΘΗΝΑ
   10: '1982'
   11: '486'
   12: ΙΑΤΡΙΚΑ
   13: ΙΑΤΡΙΚΑ
@@ -124718,15 +124580,15 @@
   13: ΙΑΤΡΙΚΑ
   14: ΙΑΤΡΙΚΑ
   17: ΔΩΡΕΑ ΓΙΑΝΝΟΥΛΑ ΜΙΧΑΛΗ
 - 0: 10058
   1: ΠΑΠΑΖΑΧΟΣ,ΓΕΩΡΓΙΟΣ
   2: ΤΟ ΗΛΕΚΤΟΚΑΡΔΙΟΓΡΑΦΗΜΑ
   4: 615.5ΠΑΠ
-  5: 10794 Α
+  5: '10794'
   9: ΛΙΤΣΑΣ
   12: ΙΑΤΡΙΚΑ
   13: ΙΑΤΡΙΚΑ
   14: ΙΑΤΡΙΚΑ
   17: ΔΩΡΕΑ ΓΙΑΝΝΟΥΛΑ ΜΙΧΑΛΗ
 - 0: 10059
   1: Χ.Σ
@@ -137635,15 +137497,15 @@
   19: 1-2
   30: 2 ΑΝΤΙΤΥΠΑ
 - 0: 10935
   1: ΗΛΙΑΔΗΣ,ΧΡΗΣΤΟΣ
   2: ΠΟΝΤΟΣ-ΓΕΝΟΚΤΟΝΙΑ
   3: ΟΣΑ ΑΝΘΥΜΟΥΜΑΙ ΑΠΟ ΤΗΝ ΠΕΡΙΠΕΤΕΙΩΔΗ ΖΩΗ ΜΟΥ
   4: 938.73ΗΛΙ
-  5: isplay status
+  5: '13499'
   8: ΓΟΡΔΙΟΣ
   9: ΑΘΗΝΑ
   10: '2002'
   11: 222Σ
   12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   14: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
@@ -144959,24 +144821,24 @@
   9: ΑΘΗΝΑ
   10: '1959'
   11: 455Σ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
 - 0: 11462
   1: ΠΕΡΙΟΔΙΚΟ
   2: ΟΡΥΚΤΑ ΚΑΙ ΟΡΥΧΕΙΑ
-  4: Ο50ΠΕΡ
+  4: 050ΠΕΡ
   5: '14142'
   11: 169Σ
   12: ΠΕΡΙΟΔΙΚΟ
   13: ΠΕΡΙΟΔΙΚΟ
   14: ΠΕΡΙΟΔΙΚΟ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
 - 0: 11463
   1: ΠΕΡΙΟΔΙΚΟ
-  4: Ο50ΠΕΡ
+  4: 050ΠΕΡ
   5: '14141'
   11: 64Σ
   12: ΠΕΡΙΟΔΙΚΟ
   13: ΠΕΡΙΟΔΙΚΟ
   14: ΠΕΡΙΟΔΙΚΟ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
 - 0: 11464
@@ -145876,15 +145738,15 @@
   12: ΑΦΗΓΗΜΑΤΑ
   13: ΑΦΗΓΗΜΑΤΑ
   14: ΑΦΗΓΗΜΑΤΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
 - 0: 11534
   1: ΠΕΡΙΟΔΙΚΟ
   2: ΘΕΣΕΙΣ ΚΑΙ ΙΔΕΑΙ
-  4: Ο50ΠΕΡ
+  4: 050ΠΕΡ
   5: '15019'
   10: '1970'
   11: 63Σ
   12: ΠΕΡΙΟΔΙΚΟ
   13: ΠΕΡΙΟΔΙΚΟ
   14: ΠΕΡΙΟΔΙΚΟ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΠΟΡΤΟΒΑΡΑ
@@ -178806,15 +178668,15 @@
   13: ΙΣΤΟΡΙΑ-ΒΟΡΕΙΟΣ ΗΠΕΙΡΟΣ
   14: ΙΣΤΟΡΙΑ-ΒΟΡΕΙΟΣ ΗΠΕΙΡΟΣ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
 - 0: 14038
   1: ΓΕΩΡΓΙΑΔΟΥ,ΝΙΚΟΛΑΟΥ
   2: ΟΣΑ ΕΓΡΑΨΑ ΣΤΟ ΜΟΝΑΣΤΗΡΙ 1903-1912
   4: 938.676ΓΕΩ
-  5: '17576'
+  5: 17576-3668
   9: ΘΕΣ/ΝΙΚΗ
   10: '1984'
   11: 245Σ
   12: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
   13: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
   14: ΙΣΤΟΡΙΑ-ΜΑΚΕΔΟΝΙΑ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
@@ -200160,15 +200022,15 @@
   14: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   17: ΔΩΡΕΑ ΔΗΜΗΤΡΙΟΥ ΤΟΜΠΟΥΛΙΔΗ
   18: '9789606440'
   19: '984'
 - 0: 15584
   1: ΠΑΠΑΦΛΩΡΑΤΟΣ,ΙΩΑΝΝΗΣ
   2: Ο ΕΛΛΗΝΙΣΜΟΣ ΤΟΥ ΠΟΝΤΟΥ
-  4: 9388ΠΑΠ
+  4: 938ΠΑΠ
   5: '20707'
   8: ΛΕΙΜΩΝ
   9: ΑΘΗΝΑ
   10: '2021'
   11: 701Σ
   12: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
   13: ΙΣΤΟΡΙΑ-ΠΟΝΤΟΣ
@@ -204093,15 +203955,15 @@
   18: '9789605037'
   19: '703'
 - 0: 15918
   1: Χ.Σ.
   2: ΑΝΘΟΛΟΓΙΟ
   3: ΓΙΑ ΤΑ ΠΑΙΔΙΑ ΤΟΥ ΔΗΜΟΤΙΚΟΥ ΜΕΡΟΣ ΤΡΙΤΟ
   4: 808.899Χ.Σ
-  5: Α1029
+  5: '21029'
   8: ΤΟ ΒΗΜΑ ΑΛΤΕΡ ΕΓΚΟ
   9: ΑΘΗΝΑ
   10: '2016'
   11: 335Σ
   12: ΑΝΘΟΛΟΓΙΟ
   13: ΑΝΘΟΛΟΓΙΟ
   14: ΑΝΘΟΛΟΓΙΟ
@@ -222463,16 +222325,16 @@
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΑΘΗΝΑ ΚΑΛΟΜΠΑΤΣΟΥ
   18: '9789600353'
   19: '723'
 - 0: 17325
   1: ΚΑΡΙΖΩΝΗ,ΚΑΤΕΡΙΝΑ
   2: ΜΕΓΑΛΟ ΑΛΓΕΡΙ
-  4: 889.21ΚΑΡ2
-  5: '2770'
+  4: 889.21ΚΑΡ
+  5: '22770'
   8: ΚΑΣΤΑΝΙΩΤΗΣ
   9: ΑΘΗΝΑ
   10: '2006'
   11: '272'
   12: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΕΛΛΗΝΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -222945,27 +222807,27 @@
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   17: ΔΩΡΕΑ ΣΠΥΡΙΔΩΝ ΣΠΥΡΟΥ
 - 0: 17358
   1: ΒΕΡΝ,ΙΟΥΛΙΟΥ
   2: Ο ΚΥΡΙΑΡΧΟΣ ΤΟΥ ΚΟΣΜΟΥ
   4: 808.899ΒΕΡ
-  5: 9170Α
+  5: 09170
   6: Λ.ΟΛΥΜΠΙΟΥ
   8: ΑΤΤΙΚΟΣ
   9: ΑΘΗΝΑ
   11: '212'
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
 - 0: 17359
   1: ΒΕΡΝ,ΙΟΥΛΙΟΥ
   2: ΚΟΥΡΣΑΡΟΙ ΤΟΥ ΑΙΓΑΙΟΥ
   4: 808.899ΒΕΡ
-  5: 9175Α
+  5: 09175
   6: Δ.Π.ΚΩΣΤΕΛΕΝΟΣ
   8: ΑΤΤΙΚΟΣ
   9: ΑΘΗΝΑ
   11: '206'
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -222981,25 +222843,27 @@
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
 - 0: 17361
   1: ΑΝΤΕΡΣΕΝ,ΧΑΝΣ ΚΡΙΣΤΙΑΝ
   2: ΑΠΑΝΤΑ Ε
   4: 808.899ΑΝΤ
+  5: '22802'
   6: Σ.ΠΡΩΤΟΠΑΠΑ
   8: ΑΡΣΕΝΙΔΗΣ
   9: ΑΘΗΝΑ
   11: '188'
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
 - 0: 17362
   1: ΑΝΤΡΙΟΥΣ,ΤΖΟΥΛΙ
   2: ΜΑΝΤΥ
   4: 808.899ΑΝΤ
+  5: '22803'
   6: Κ.ΣΙΝΟΥ
   8: ΓΕΜΕΝΤΖΟΠΟΥΛΟΣ
   9: ΑΘΗΝΑ
   11: '148'
   12: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
@@ -223921,15 +223785,15 @@
   13: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
   14: ΠΑΙΔΙΚΗ ΛΟΓΟΤΕΧΝΙΑ
 - 0: 17435
 - 0: 17436
   1: ΚΑΛΑΤΖΟΠΟΥΛΟΣ,ΓΙΑΝΝΗΣ
   2: ΘΕΑΤΡΟ ΓΙΑ ΠΑΙΔΙΑ ΚΑΙ ... ΕΞΥΠΝΟΥΣ ΜΕΓΑΛΟΥΣ
   4: 886.2ΚΑΛ
-  5: 22839,22840
+  5: 22839-22840
   8: ΦΙΛΝΤΙΣΙ
   9: ΑΘΗΝΑ
   10: '2021'
   11: '335'
   12: ΘΕΑΤΡΟ
   13: ΘΕΑΤΡΟ ΓΙΑ ΠΑΙΔΙΑ
   14: ΘΕΑΤΡΙΚΟ ΓΙΑ ΠΑΙΔΙΑ
@@ -225158,15 +225022,15 @@
   12: ΘΕΑΤΡΟ
   13: ΘΕΑΤΡΟ
   14: ΘΕΑΤΡΟ
   17: ΔΩΡΕΑ ΧΡ. ΣΤΑΥΡΟΥΔΗ - 2 ΒΙΒΛΙΑ
 - 0: 17528
   1: ΦΩΤΙΑΔΟΥ,ΜΑΡΙΑ
   2: ΟΜΑΔΕΣ ΑΙΜΑΤΟΣ-RH-ΑΙΜΟΛΥΤΙΚΗ ΑΝΑΙΜΙΑ ΤΩΝ ΝΕΟΓΝΩΝ
-  4: 610.73ΦΩΤ0
+  4: 610.73ΦΩΤ
   5: '22930'
   9: ΘΕΣΣΑΛΟΝΙΚ
   10: '1980'
   11: '38'
   12: ΠΤΥΧΙΑΚΗ ΕΡΓΑΣΙΑ
   13: ΠΤΥΧΙΑΚΗ ΕΡΓΑΣΙΑ
   14: ΠΤΥΧΙΑΚΗ ΕΡΓΑΣΙΑ
@@ -225726,7 +225590,22 @@
   8: Δ/ΝΣΗ ΙΣΤΟΡΙΑΣ ΣΤΡΑΤ
   9: ΑΘΗΝΑ
   10: '1957'
   11: '434'
   12: ΙΣΤΟΡΙΑ ΣΤΡΑΤΟΥ
   13: ΙΣΤΟΡΙΑ ΣΤΡΑΤΟΥ
   14: ΙΣΤΟΡΙΑ ΣΤΡΑΤΟΥ
+- 0: 17573
+  1: ΜΟΡΤΟΝ,ΚΕΙΤ
+  2: Η ΚΟΡΗ ΤΟΥ ΡΟΛΟΓΑ
+  4: 823ΜΟΡ
+  5: '23015'
+  6: ΧΡΙΣΤ. ΣΑΚΕΛΛΑΡΟΠΟΥΛ
+  8: ΛΙΒΑΝΗΣ
+  9: ΑΘΗΝΑ
+  10: '2019'
+  11: '603'
+  12: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  13: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  14: ΞΕΝΗ ΛΟΓΟΤΕΧΝΙΑ
+  18: '9789601435'
+  19: '077'
```

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field04_corrections.yml` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field04_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field05_corrections.yml` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field05_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field06_corrections.yml` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field06_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field07_corrections.yml` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field07_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field08_corrections.yml` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field08_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field09_corrections.yml` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field09_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field16_corrections.yml` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field16_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field17_corrections.yml` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field17_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field18_corrections.yml` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field18_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field19_corrections.yml` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field19_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/field30_corrections.yml` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/field30_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/first_names.yml` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/first_names.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/topic_replacements.yml` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/topic_replacements.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/data/translator_corrections.yml` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/data/translator_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/dbf_to_yaml.py` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/dbf_to_yaml.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/field_extractors.py` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/field_extractors.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/generate_reports.py` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/generate_reports.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/src/skoufas_dbf_reader/utilities.py` & `skoufas_dbf_reader-0.0.4rc170.post1/src/skoufas_dbf_reader/utilities.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/tests/test_field_extractors.py` & `skoufas_dbf_reader-0.0.4rc170.post1/tests/test_field_extractors.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/tests/test_reports.py` & `skoufas_dbf_reader-0.0.4rc170.post1/tests/test_reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -479,7 +479,50 @@
         yaml.dump(
             {"titles": titles},
             outfile,
             default_flow_style=False,
             allow_unicode=True,
             sort_keys=False,
         )
+
+
+def test_report_authors_with_no_correction(reports_directory: str):
+    authors = []
+    for entry in all_entries():
+        a01 = entry[1]
+        if not a01:
+            continue
+        if not has_author(a01):
+            continue
+        strip_finals = list(language_codes().keys()) + [
+            " Ι",
+            " .",
+        ]
+        for final in strip_finals:
+            if a01.endswith(" " + final):
+                a01 = a01.replace(final, "")
+        author = a01.strip()
+        if author not in author_corrections():
+            authors.append(author)
+
+    def correct_name(name):
+        return name.replace("ΚΩΝ/ΝΟΣ", "ΚΩΝΣΤΑΝΤΙΝΟΣ")
+
+    with open(os.path.join(reports_directory, "authors_with_no_correction.yml"), "w", encoding="utf-8") as outfile:
+        yaml.dump(
+            {"authors_with_no_correction": {k: correct_name(k) for k in sorted(authors)}},
+            outfile,
+            default_flow_style=False,
+            allow_unicode=True,
+            sort_keys=False,
+        )
+
+    with open(
+        os.path.join(reports_directory, "authors_with_no_correction_phonetic.yml"), "w", encoding="utf-8"
+    ) as outfile:
+        yaml.dump(
+            {"authors_with_no_correction": {k: correct_name(k) for k in sorted(authors, key=lambda x: romanize(x))}},
+            outfile,
+            default_flow_style=False,
+            allow_unicode=True,
+            sort_keys=False,
+        )
```

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/tests/test_utilities.py` & `skoufas_dbf_reader-0.0.4rc170.post1/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.4rc166.post1/PKG-INFO` & `skoufas_dbf_reader-0.0.4rc170.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skoufas-dbf-reader
-Version: 0.0.4rc166.post1
+Version: 0.0.4rc170.post1
 Summary: Library for reading legacy DBF file with library data
 Author-email: Claudio Bantaloukas <rockreamer@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

