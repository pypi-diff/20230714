# Comparing `tmp/cdmb-1.0.0.tar.gz` & `tmp/cdmb-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdmb-1.0.0.tar", max compression
+gzip compressed data, was "cdmb-1.1.0.tar", max compression
```

## Comparing `cdmb-1.0.0.tar` & `cdmb-1.1.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0    19345 2023-07-12 14:19:03.869238 cdmb-1.0.0/LICENSE
--rw-r--r--   0        0        0    34628 2023-07-12 14:19:03.869238 cdmb-1.0.0/README.md
--rw-r--r--   0        0        0    63899 2023-07-12 14:19:03.869238 cdmb-1.0.0/cdmb/CommonDataModel.py
--rw-r--r--   0        0        0      991 2023-07-12 14:19:03.869238 cdmb-1.0.0/cdmb/__init__.py
--rw-r--r--   0        0        0     8532 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/cohort/Cohort.py
--rw-r--r--   0        0        0     4576 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/cohort/Crosswalks.py
--rw-r--r--   0        0        0      120 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/cohort/__init__.py
--rw-r--r--   0        0        0     2921 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/entities/Catalog.py
--rw-r--r--   0        0        0    15180 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/entities/Entity.py
--rw-r--r--   0        0        0    22831 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/entities/Rule.py
--rw-r--r--   0        0        0    10189 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/entities/RuleSet.py
--rw-r--r--   0        0        0    11975 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/entities/Variable.py
--rw-r--r--   0        0        0      498 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/entities/__init__.py
--rw-r--r--   0        0        0     4637 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/project/Author.py
--rw-r--r--   0        0        0    12717 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/project/Metadata.py
--rw-r--r--   0        0        0       33 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/project/__init__.py
--rw-r--r--   0        0        0     6027 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/relationships/Relationship.py
--rw-r--r--   0        0        0       28 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/relationships/__init__.py
--rw-r--r--   0        0        0     1659 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/templates/Utils.py
--rw-r--r--   0        0        0       21 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/templates/__init__.py
--rw-r--r--   0        0        0       50 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/templates/files/.gitignore
--rw-r--r--   0        0        0    18656 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/templates/files/LICENSE.md
--rw-r--r--   0        0        0     5920 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/templates/files/README.md
--rw-r--r--   0        0        0       41 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/templates/files/_quarto.yml
--rw-r--r--   0        0        0    10224 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/templates/files/check_load.py
--rw-r--r--   0        0        0     2947 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/templates/files/dqa.py
--rw-r--r--   0        0        0      151 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/templates/files/man_container_deployment.md
--rw-r--r--   0        0        0     2855 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/templates/files/r_report_template.qmd
--rw-r--r--   0        0        0    10130 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/templates/files/validator.py
--rw-r--r--   0        0        0     3228 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/templates/files/validator_report.qmd
--rw-r--r--   0        0        0      554 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/typing/CommonDataModelTyping.py
--rw-r--r--   0        0        0       36 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/typing/__init__.py
--rw-r--r--   0        0        0    12472 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/ui/UILauncher.py
--rw-r--r--   0        0        0       65 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/ui/__init__.py
--rw-r--r--   0        0        0   111554 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/0.83e0eb50.css
--rw-r--r--   0        0        0      412 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/2.b838d5a7.css
--rw-r--r--   0        0        0     4495 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/4.18440754.css
--rw-r--r--   0        0        0     3111 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/6.bf404883.css
--rw-r--r--   0        0        0       34 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/Indicator.1d121e74.css
--rw-r--r--   0        0        0   111782 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/_layout.f2858481.css
--rw-r--r--   0        0        0     4491 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/_page.11cd5570.css
--rw-r--r--   0        0        0      412 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/_page.b838d5a7.css
--rw-r--r--   0        0        0     3111 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/_page.bf404883.css
--rw-r--r--   0        0        0    12580 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/eu_flag.c3360867.jpg
--rw-r--r--   0        0        0    25582 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/favicon.157dca14.png
--rw-r--r--   0        0        0    77364 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-all-400-normal.1e3b098c.woff
--rw-r--r--   0        0        0     9104 2023-07-12 14:19:03.873238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-400-normal.c7d433fd.woff2
--rw-r--r--   0        0        0    15772 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-ext-400-normal.3df7909e.woff2
--rw-r--r--   0        0        0    10520 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-400-normal.a8be01ce.woff2
--rw-r--r--   0        0        0     7508 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-ext-400-normal.9e2fe623.woff2
--rw-r--r--   0        0        0    16284 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-400-normal.e43b3538.woff2
--rw-r--r--   0        0        0    11364 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-ext-400-normal.6bfabd30.woff2
--rw-r--r--   0        0        0     1753 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/github.1ea8d62e.svg
--rw-r--r--   0        0        0    21305 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.15dffd2d.png
--rw-r--r--   0        0        0    11196 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.dcd54a0d.webp
--rw-r--r--   0        0        0     3663 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/Alert.2febe6fa.js
--rw-r--r--   0        0        0    10431 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/Button.68ac352c.js
--rw-r--r--   0        0        0     6362 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/CloseButton.0aecb936.js
--rw-r--r--   0        0        0    13044 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/Divider.623c8765.js
--rw-r--r--   0        0        0     2206 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/Fileupload.78d706fe.js
--rw-r--r--   0        0        0    15049 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/FloatingLabelInput.21cd1ebc.js
--rw-r--r--   0        0        0     1844 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/Heading.759b5df3.js
--rw-r--r--   0        0        0      817 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/Indicator.svelte_svelte_type_style_lang.e2c519f7.js
--rw-r--r--   0        0        0     9203 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/Modal.b90503ef.js
--rw-r--r--   0        0        0    45009 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/SimpleGrid.f308d3bd.js
--rw-r--r--   0        0        0    41583 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/Space.5d3c5051.js
--rw-r--r--   0        0        0     9044 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/TableHeadCell.a7fa45f2.js
--rw-r--r--   0        0        0     4606 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/Textarea.17eddb3d.js
--rw-r--r--   0        0        0     1484 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/Trash.33219cd3.js
--rw-r--r--   0        0        0    15089 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/combinator.becf7b0b.js
--rw-r--r--   0        0        0       27 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/environment.9aa685ef.js
--rw-r--r--   0        0        0      820 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/index.5b757cee.js
--rw-r--r--   0        0        0     1667 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/index.b7a14a97.js
--rw-r--r--   0        0        0    16042 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/index.d8ca07a9.js
--rw-r--r--   0        0        0     9918 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/navigation.8bb60df9.js
--rw-r--r--   0        0        0     2496 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/singletons.3dbe6478.js
--rw-r--r--   0        0        0      414 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/store.247e7f87.js
--rw-r--r--   0        0        0    11736 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/store.4d7a1ebc.js
--rw-r--r--   0        0        0      814 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/store.6cd3ab0e.js
--rw-r--r--   0        0        0     1379 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/store.c28f1804.js
--rw-r--r--   0        0        0      266 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/stores.d0e64236.js
--rw-r--r--   0        0        0     9868 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/entry/app.34f7a124.js
--rw-r--r--   0        0        0    23923 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/entry/start.07ad94a0.js
--rw-r--r--   0        0        0    13097 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/nodes/0.51906aee.js
--rw-r--r--   0        0        0      800 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/nodes/1.e22fd99e.js
--rw-r--r--   0        0        0    20534 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/nodes/2.7284b9d4.js
--rw-r--r--   0        0        0    27325 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/nodes/3.510394aa.js
--rw-r--r--   0        0        0    56093 2023-07-12 14:19:03.877238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/nodes/4.828fc947.js
--rw-r--r--   0        0        0   122218 2023-07-12 14:19:03.881238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/nodes/5.faf63ad8.js
--rw-r--r--   0        0        0    68782 2023-07-12 14:19:03.881238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/nodes/6.c31223f5.js
--rw-r--r--   0        0        0    61556 2023-07-12 14:19:03.881238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/nodes/7.56d911fb.js
--rw-r--r--   0        0        0    28637 2023-07-12 14:19:03.881238 cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/nodes/8.ed4ac5b3.js
--rw-r--r--   0        0        0       27 2023-07-12 14:19:03.881238 cdmb-1.0.0/cdmb/ui/static_ui/_app/version.json
--rw-r--r--   0        0        0    13602 2023-07-12 14:19:03.881238 cdmb-1.0.0/cdmb/ui/static_ui/about.html
--rw-r--r--   0        0        0    17310 2023-07-12 14:19:03.881238 cdmb-1.0.0/cdmb/ui/static_ui/cohort.html
--rw-r--r--   0        0        0     5151 2023-07-12 14:19:03.881238 cdmb-1.0.0/cdmb/ui/static_ui/entities.html
--rw-r--r--   0        0        0    25582 2023-07-12 14:19:03.881238 cdmb-1.0.0/cdmb/ui/static_ui/favicon.png
--rw-r--r--   0        0        0    10045 2023-07-12 14:19:03.881238 cdmb-1.0.0/cdmb/ui/static_ui/index.html
--rw-r--r--   0        0        0    21009 2023-07-12 14:19:03.881238 cdmb-1.0.0/cdmb/ui/static_ui/project.html
--rw-r--r--   0        0        0       67 2023-07-12 14:19:03.881238 cdmb-1.0.0/cdmb/ui/static_ui/robots.txt
--rw-r--r--   0        0        0    15244 2023-07-12 14:19:03.881238 cdmb-1.0.0/cdmb/ui/static_ui/summary.html
--rw-r--r--   0        0        0     8887 2023-07-12 14:19:03.881238 cdmb-1.0.0/cdmb/ui/static_ui/validation.html
--rw-r--r--   0        0        0     1472 2023-07-12 14:19:03.881238 cdmb-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    36277 1970-01-01 00:00:00.000000 cdmb-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    19345 2023-07-14 11:35:03.439263 cdmb-1.1.0/LICENSE
+-rw-r--r--   0        0        0    35035 2023-07-14 11:35:03.439263 cdmb-1.1.0/README.md
+-rw-r--r--   0        0        0    64829 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/CommonDataModel.py
+-rw-r--r--   0        0        0      991 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/__init__.py
+-rw-r--r--   0        0        0     8532 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/cohort/Cohort.py
+-rw-r--r--   0        0        0     4576 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/cohort/Crosswalks.py
+-rw-r--r--   0        0        0      120 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/cohort/__init__.py
+-rw-r--r--   0        0        0     2921 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/entities/Catalog.py
+-rw-r--r--   0        0        0    15180 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/entities/Entity.py
+-rw-r--r--   0        0        0    22831 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/entities/Rule.py
+-rw-r--r--   0        0        0    10189 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/entities/RuleSet.py
+-rw-r--r--   0        0        0    11975 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/entities/Variable.py
+-rw-r--r--   0        0        0      498 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/entities/__init__.py
+-rw-r--r--   0        0        0     4637 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/project/Author.py
+-rw-r--r--   0        0        0    12717 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/project/Metadata.py
+-rw-r--r--   0        0        0       33 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/project/__init__.py
+-rw-r--r--   0        0        0     6027 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/relationships/Relationship.py
+-rw-r--r--   0        0        0       28 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/relationships/__init__.py
+-rw-r--r--   0        0        0     1659 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/Utils.py
+-rw-r--r--   0        0        0       21 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/__init__.py
+-rw-r--r--   0        0        0       50 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/files/.gitignore
+-rw-r--r--   0        0        0    18656 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/files/LICENSE.md
+-rw-r--r--   0        0        0     5920 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/files/README.md
+-rw-r--r--   0        0        0       41 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/files/_quarto.yml
+-rw-r--r--   0        0        0    10224 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/files/check_load.py
+-rw-r--r--   0        0        0     2947 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/files/dqa.py
+-rw-r--r--   0        0        0      151 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/files/man_container_deployment.md
+-rw-r--r--   0        0        0     2855 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/files/r_report_template.qmd
+-rw-r--r--   0        0        0    10161 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/files/validator.py
+-rw-r--r--   0        0        0     3228 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/files/validator_report.qmd
+-rw-r--r--   0        0        0      554 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/typing/CommonDataModelTyping.py
+-rw-r--r--   0        0        0       36 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/typing/__init__.py
+-rw-r--r--   0        0        0    12472 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/UILauncher.py
+-rw-r--r--   0        0        0       65 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/__init__.py
+-rw-r--r--   0        0        0   111554 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/0.83e0eb50.css
+-rw-r--r--   0        0        0      412 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/2.b838d5a7.css
+-rw-r--r--   0        0        0     4495 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/4.18440754.css
+-rw-r--r--   0        0        0     3111 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/6.bf404883.css
+-rw-r--r--   0        0        0       34 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/Indicator.1d121e74.css
+-rw-r--r--   0        0        0   111782 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/_layout.f2858481.css
+-rw-r--r--   0        0        0     4491 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/_page.11cd5570.css
+-rw-r--r--   0        0        0      412 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/_page.b838d5a7.css
+-rw-r--r--   0        0        0     3111 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/_page.bf404883.css
+-rw-r--r--   0        0        0    12580 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/eu_flag.c3360867.jpg
+-rw-r--r--   0        0        0    25582 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/favicon.157dca14.png
+-rw-r--r--   0        0        0    77364 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-all-400-normal.1e3b098c.woff
+-rw-r--r--   0        0        0     9104 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-400-normal.c7d433fd.woff2
+-rw-r--r--   0        0        0    15772 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-ext-400-normal.3df7909e.woff2
+-rw-r--r--   0        0        0    10520 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-400-normal.a8be01ce.woff2
+-rw-r--r--   0        0        0     7508 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-ext-400-normal.9e2fe623.woff2
+-rw-r--r--   0        0        0    16284 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-400-normal.e43b3538.woff2
+-rw-r--r--   0        0        0    11364 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-ext-400-normal.6bfabd30.woff2
+-rw-r--r--   0        0        0     1753 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/github.1ea8d62e.svg
+-rw-r--r--   0        0        0    21305 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.15dffd2d.png
+-rw-r--r--   0        0        0    11196 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.dcd54a0d.webp
+-rw-r--r--   0        0        0     3663 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Alert.2febe6fa.js
+-rw-r--r--   0        0        0    10431 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Button.68ac352c.js
+-rw-r--r--   0        0        0     6362 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/CloseButton.0aecb936.js
+-rw-r--r--   0        0        0    13044 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Divider.623c8765.js
+-rw-r--r--   0        0        0     2206 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Fileupload.78d706fe.js
+-rw-r--r--   0        0        0    15049 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/FloatingLabelInput.21cd1ebc.js
+-rw-r--r--   0        0        0     1844 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Heading.759b5df3.js
+-rw-r--r--   0        0        0      817 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Indicator.svelte_svelte_type_style_lang.e2c519f7.js
+-rw-r--r--   0        0        0     9203 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Modal.b90503ef.js
+-rw-r--r--   0        0        0    45009 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/SimpleGrid.f308d3bd.js
+-rw-r--r--   0        0        0    41583 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Space.5d3c5051.js
+-rw-r--r--   0        0        0     9044 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/TableHeadCell.a7fa45f2.js
+-rw-r--r--   0        0        0     4606 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Textarea.17eddb3d.js
+-rw-r--r--   0        0        0     1484 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Trash.33219cd3.js
+-rw-r--r--   0        0        0    15089 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/combinator.becf7b0b.js
+-rw-r--r--   0        0        0       27 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/environment.9aa685ef.js
+-rw-r--r--   0        0        0      820 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/index.5b757cee.js
+-rw-r--r--   0        0        0     1667 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/index.b7a14a97.js
+-rw-r--r--   0        0        0    16042 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/index.d8ca07a9.js
+-rw-r--r--   0        0        0     9918 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/navigation.8bb60df9.js
+-rw-r--r--   0        0        0     2496 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/singletons.3dbe6478.js
+-rw-r--r--   0        0        0      414 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/store.247e7f87.js
+-rw-r--r--   0        0        0    11736 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/store.4d7a1ebc.js
+-rw-r--r--   0        0        0      814 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/store.6cd3ab0e.js
+-rw-r--r--   0        0        0     1379 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/store.c28f1804.js
+-rw-r--r--   0        0        0      266 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/stores.d0e64236.js
+-rw-r--r--   0        0        0     9868 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/entry/app.34f7a124.js
+-rw-r--r--   0        0        0    23923 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/entry/start.07ad94a0.js
+-rw-r--r--   0        0        0    13097 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/0.51906aee.js
+-rw-r--r--   0        0        0      800 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/1.e22fd99e.js
+-rw-r--r--   0        0        0    20534 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/2.7284b9d4.js
+-rw-r--r--   0        0        0    27325 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/3.510394aa.js
+-rw-r--r--   0        0        0    56093 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/4.828fc947.js
+-rw-r--r--   0        0        0   122218 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/5.faf63ad8.js
+-rw-r--r--   0        0        0    68782 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/6.c31223f5.js
+-rw-r--r--   0        0        0    61580 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/7.56d911fb.js
+-rw-r--r--   0        0        0    28637 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/8.ed4ac5b3.js
+-rw-r--r--   0        0        0       27 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/_app/version.json
+-rw-r--r--   0        0        0    13602 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/about.html
+-rw-r--r--   0        0        0    17310 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/cohort.html
+-rw-r--r--   0        0        0     5151 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/entities.html
+-rw-r--r--   0        0        0    25582 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/favicon.png
+-rw-r--r--   0        0        0    10045 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/index.html
+-rw-r--r--   0        0        0    21009 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/project.html
+-rw-r--r--   0        0        0       67 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/robots.txt
+-rw-r--r--   0        0        0    15250 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/summary.html
+-rw-r--r--   0        0        0     8887 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/validation.html
+-rw-r--r--   0        0        0     1472 2023-07-14 11:35:03.447264 cdmb-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    36684 1970-01-01 00:00:00.000000 cdmb-1.1.0/PKG-INFO
```

### Comparing `cdmb-1.0.0/LICENSE` & `cdmb-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/README.md` & `cdmb-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Logo of the project](https://cienciadedatosysalud.org/wp-content/uploads/Data-Science-and-VPM.png)
+![Logo of the project](https://cienciadedatosysalud.org/wp-content/uploads/logo-Data-Science-VPM.png)
 - [Common Data Model Builder (cdmb)](#common-data-model-builder-cdmb)
 - [User Interface](#user-interface)
 - [Outputs](#outputs)
 - [Classes](#classes)
   - [Metadata](#metadata)
   - [Author](#author)
   - [Cohort](#cohort)
@@ -48,14 +48,27 @@
 port = 8000
 
 launch_ui(server_address, port)
 # Open your web browser at http://<server_address>:<port>.
 # http://localhost:8000
 ```
 
+# Run in Docker
+Alternatively you can run the graphical interface provided by the Common Data Model Builder directly in a docker container.
+
+Use the following code snippet to create the container.
+```bash
+docker pull ghcr.io/cienciadedatosysalud/cdmb:latest
+
+docker run -p 127.0.0.1:8501:8501 --name cdmb_ui ghcr.io/cienciadedatosysalud/cdmb:latest
+
+# Open your web browser at http://localhost:8501.
+```
+
+
 # Outputs
 Outputs structure and content is described below including the files and folders that are generated when creating a research project with the `cdmb` Python library. There are four main folders corresponding to:
 
 - __docs/CDM/__
   - **cdmb_config.json**: Configuration file.
   - **cohort_definition_inclusion.csv**: csv file that defines the criteria (i.e., codes) for inclusion in a cohort.
   - **cohort_definition_exclusion.csv**: csv file that defines the criteria (i.e., codes) for exclusion in a cohort.
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 ![Logo of the project](https://cienciadedatosysalud.org/wp-content/uploads/
-Data-Science-and-VPM.png) - [Common Data Model Builder (cdmb)](#common-data-
+logo-Data-Science-VPM.png) - [Common Data Model Builder (cdmb)](#common-data-
 model-builder-cdmb) - [User Interface](#user-interface) - [Outputs](#outputs) -
 [Classes](#classes) - [Metadata](#metadata) - [Author](#author) - [Cohort]
 (#cohort) - [Crosswalks](#crosswalks) - [Entities](#entities) - [Variables]
 (#variables) - [Catalogs](#catalogs) - [Rules Set](#rules-set) - [Rules]
 (#rules) - [Comparison rule](#comparison-rule) - [BetweenComparison]
 (#betweencomparison) - [NullCheckingRule](#nullcheckingrule) - [InValuesRule]
 (#invaluesrule) - [ComposedRule](#composedrule) - [DummyRule](#dummyrule) -
@@ -22,31 +22,37 @@
 functionalities of Common Data Model Builder is to provide the user with a
 graphical interface to fill in the Common Data Model and export it in a simple
 way. Follow the following code snippet to access it. #### Inputs: -
 **server_address**: a string representing the server address, default value is
 "localhost" - **port**: a string representing the server port, default value is
 "8501" #### Example: ```python from cdmb import launch_ui server_address =
 "localhost" port = 8000 launch_ui(server_address, port) # Open your web browser
-at http://:. # http://localhost:8000 ``` # Outputs Outputs structure and
-content is described below including the files and folders that are generated
-when creating a research project with the `cdmb` Python library. There are four
-main folders corresponding to: - __docs/CDM/__ - **cdmb_config.json**:
-Configuration file. - **cohort_definition_inclusion.csv**: csv file that
-defines the criteria (i.e., codes) for inclusion in a cohort. -
-**cohort_definition_exclusion.csv**: csv file that defines the criteria (i.e.,
-codes) for exclusion in a cohort. - **common_datamodel.xlsx**: The definition
-of the common data model in Excel format. - **entities/**: Folder structure
-where, for each defined entity, the catalogs and the established validation
-rules are stored. - **ER.gv, ER.gv.png**: an Entity-Relationship Diagram of the
-entities included in the CDM. - **synthetic-data/**: Folder structure contaning
-an automatically generated set of 1000 synthetic records per entity included en
-the CDM. - **hashed_files_list.json**: List of the files generated or used
-after generating the project with their md5 hash. This file must be kept hidden
-and should be used to cross-check with the results obtained from the analysis
-from the original input files. - __inputs/__ - **data.duckdb**: Database that
+at http://:. # http://localhost:8000 ``` # Run in Docker Alternatively you can
+run the graphical interface provided by the Common Data Model Builder directly
+in a docker container. Use the following code snippet to create the container.
+```bash docker pull ghcr.io/cienciadedatosysalud/cdmb:latest docker run -
+p 127.0.0.1:8501:8501 --name cdmb_ui ghcr.io/cienciadedatosysalud/cdmb:latest #
+Open your web browser at http://localhost:8501. ``` # Outputs Outputs structure
+and content is described below including the files and folders that are
+generated when creating a research project with the `cdmb` Python library.
+There are four main folders corresponding to: - __docs/CDM/__ -
+**cdmb_config.json**: Configuration file. -
+**cohort_definition_inclusion.csv**: csv file that defines the criteria (i.e.,
+codes) for inclusion in a cohort. - **cohort_definition_exclusion.csv**: csv
+file that defines the criteria (i.e., codes) for exclusion in a cohort. -
+**common_datamodel.xlsx**: The definition of the common data model in Excel
+format. - **entities/**: Folder structure where, for each defined entity, the
+catalogs and the established validation rules are stored. - **ER.gv,
+ER.gv.png**: an Entity-Relationship Diagram of the entities included in the
+CDM. - **synthetic-data/**: Folder structure contaning an automatically
+generated set of 1000 synthetic records per entity included en the CDM. -
+**hashed_files_list.json**: List of the files generated or used after
+generating the project with their md5 hash. This file must be kept hidden and
+should be used to cross-check with the results obtained from the analysis from
+the original input files. - __inputs/__ - **data.duckdb**: Database that
 temporarily contains the data entered by the user (synthetic data by default) -
 __outputs/__ - (Default directory of all the outputs produced in the project
 execution) - __src/__ - __analysis-scripts/__ - (directory where the analysis
 scripts developed by the user are stored) - **r_report_template.qmd**: Quarto
 document, with an example analysis, showing the interaction with the folder
 structure and files generated in the project. - **_quarto.yml**: File
 containing the Metadata to execute Quarto documents. - __check_load-scripts/__
```

### Comparing `cdmb-1.0.0/cdmb/CommonDataModel.py` & `cdmb-1.1.0/cdmb/CommonDataModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -603,14 +603,19 @@
 
             con.sql("CREATE TABLE " + entity.name + " AS SELECT * FROM df")
 
     def __create_rog(self):
         crate = ROCrate()
         authors = []
         orcid_prefix = "https://orcid.org/"
+        crate.name = str(self.metadata.project or '')
+        crate.description = str(self.metadata.description or '')
+        crate.keywords = ', '.join(self.metadata.keywords)
+        crate.license = str(self.metadata.license or '')
+        crate.creator = "Common Data Model Builder"
         for author in self.metadata.authors:
             orcid_id_ = author.id
             name_ = author.name
             affiliation_ = author.affiliation
             if orcid_id_ is not None:
                 exp1 = re.search("[0-9]{4}-[0-9]{4}-[0-9]{4}-[0-9]{4}", orcid_id_)
                 if exp1 is not None:
@@ -937,44 +942,44 @@
         else:
             raise ValueError('The "entities" field does not exist in the configuration file and is a mandatory field.')
         # Create Relationships
         if 'relationships' in configuration:
             relationships_list: list[Relationship] = []
             for relationship in configuration['relationships']:
                 if 'left_entity' not in relationship:
-                    raise ValueError()
+                    raise ValueError("'left_entity' is not declared in the relationship")
                 if 'right_entity' not in relationship:
-                    raise ValueError()
+                    raise ValueError("'right_entity' is not declared in the relationship")
                 if 'join_type' not in relationship:
-                    raise ValueError()
+                    raise ValueError("'join_type' is not declared in the relationship")
                 if 'left_column' not in relationship:
-                    raise ValueError()
+                    raise ValueError("'left_column' is not declared in the relationship")
                 if 'right_column' not in relationship:
-                    raise ValueError()
+                    raise ValueError("'right_column' is not declared in the relationship")
                 left_entity_str = relationship["left_entity"]
                 if left_entity_str not in entities_catalog:
-                    raise ValueError()
+                    raise ValueError("The left entity of the relationship does not match any of the declared entities.")
                 left_entity = entities_catalog[left_entity_str]
 
                 right_entity_str = relationship["right_entity"]
                 if right_entity_str not in entities_catalog:
-                    raise ValueError()
+                    raise ValueError("The right entity of the relationship does not match any of the declared entities.")
                 right_entity = entities_catalog[right_entity_str]
 
                 join_type = relationship["join_type"]
                 if join_type not in JoinOptions.__args__:
-                    raise ValueError()
+                    raise ValueError('join_type must be in {literal_values}'.format(literal_values=JoinOptions.__args__))
 
                 left_column = left_entity.get_variable_by_label(relationship["left_column"])
                 if left_column is None:
-                    raise ValueError()
+                    raise ValueError('"left_column" variable has to be part of its entity ("left_entity")')
 
                 right_column = right_entity.get_variable_by_label(relationship["right_column"])
                 if right_column is None:
-                    raise ValueError()
+                    raise ValueError('"right_column" variable has to be part of its entity ("right_entity")')
 
                 relationships_list.append(Relationship(left_entity, right_entity, left_column, right_column, join_type))
         else:
             raise ValueError(
                 'The "relationships" field does not exist in the configuration file and is a mandatory field.')
         return metadata, cohort, entities_list, relationships_list
```

### Comparing `cdmb-1.0.0/cdmb/__init__.py` & `cdmb-1.1.0/cdmb/__init__.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/cohort/Cohort.py` & `cdmb-1.1.0/cdmb/cohort/Cohort.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/cohort/Crosswalks.py` & `cdmb-1.1.0/cdmb/cohort/Crosswalks.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/entities/Catalog.py` & `cdmb-1.1.0/cdmb/entities/Catalog.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/entities/Entity.py` & `cdmb-1.1.0/cdmb/entities/Entity.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/entities/Rule.py` & `cdmb-1.1.0/cdmb/entities/Rule.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/entities/RuleSet.py` & `cdmb-1.1.0/cdmb/entities/RuleSet.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/entities/Variable.py` & `cdmb-1.1.0/cdmb/entities/Variable.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/project/Author.py` & `cdmb-1.1.0/cdmb/project/Author.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/project/Metadata.py` & `cdmb-1.1.0/cdmb/project/Metadata.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/relationships/Relationship.py` & `cdmb-1.1.0/cdmb/relationships/Relationship.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/templates/Utils.py` & `cdmb-1.1.0/cdmb/templates/Utils.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/templates/files/LICENSE.md` & `cdmb-1.1.0/cdmb/templates/files/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/templates/files/README.md` & `cdmb-1.1.0/cdmb/templates/files/README.md`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/templates/files/check_load.py` & `cdmb-1.1.0/cdmb/templates/files/check_load.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/templates/files/dqa.py` & `cdmb-1.1.0/cdmb/templates/files/dqa.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/templates/files/r_report_template.qmd` & `cdmb-1.1.0/cdmb/templates/files/r_report_template.qmd`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/templates/files/validator.py` & `cdmb-1.1.0/cdmb/templates/files/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             if 'catalog_bl' not in variable:
                 logging.warning(
                     f"\"catalog_bl\" property is not defined for variable")
 
             if 'catalog_bl' in variable and variable['catalog_bl'] is True and str(variable['format']).lower() != "boolean":
                 logging.info(
                     f"Checking variables that are defined based on a catalog.")
-                if 'column_name' not in variable['catalog'] or 'filename' not in variable['catalog']:
+                if variable['catalog'] is None or 'column_name' not in variable['catalog'] or 'filename' not in variable['catalog']:
                     logging.error(
                         f"\"catalog\" for your variable \"{entity_name}\" is not well defined in your configuration file! Check the specifications!")
                     exit(1)
                 column_name = variable['catalog']["column_name"]
                 filename = variable['catalog']["filename"]
 
                 catalog_path = os.path.join('../../docs/CDM/entities', entity_name, 'catalogs', filename)
```

### Comparing `cdmb-1.0.0/cdmb/templates/files/validator_report.qmd` & `cdmb-1.1.0/cdmb/templates/files/validator_report.qmd`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/typing/CommonDataModelTyping.py` & `cdmb-1.1.0/cdmb/typing/CommonDataModelTyping.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/UILauncher.py` & `cdmb-1.1.0/cdmb/ui/UILauncher.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/0.83e0eb50.css` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/0.83e0eb50.css`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/4.18440754.css` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/4.18440754.css`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/6.bf404883.css` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/6.bf404883.css`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/_layout.f2858481.css` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/_layout.f2858481.css`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/_page.11cd5570.css` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/_page.11cd5570.css`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/_page.bf404883.css` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/_page.bf404883.css`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/eu_flag.c3360867.jpg` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/eu_flag.c3360867.jpg`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/favicon.157dca14.png` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/favicon.157dca14.png`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-all-400-normal.1e3b098c.woff` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-all-400-normal.1e3b098c.woff`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-400-normal.c7d433fd.woff2` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-400-normal.c7d433fd.woff2`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-ext-400-normal.3df7909e.woff2` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-ext-400-normal.3df7909e.woff2`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-400-normal.a8be01ce.woff2` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-400-normal.a8be01ce.woff2`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-ext-400-normal.9e2fe623.woff2` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-ext-400-normal.9e2fe623.woff2`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-400-normal.e43b3538.woff2` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-400-normal.e43b3538.woff2`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-ext-400-normal.6bfabd30.woff2` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-ext-400-normal.6bfabd30.woff2`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/github.1ea8d62e.svg` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/github.1ea8d62e.svg`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.15dffd2d.png` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.15dffd2d.png`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.dcd54a0d.webp` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.dcd54a0d.webp`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/Alert.2febe6fa.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Alert.2febe6fa.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/Button.68ac352c.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Button.68ac352c.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/CloseButton.0aecb936.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/CloseButton.0aecb936.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/Divider.623c8765.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Divider.623c8765.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/Fileupload.78d706fe.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Fileupload.78d706fe.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/FloatingLabelInput.21cd1ebc.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/FloatingLabelInput.21cd1ebc.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/Heading.759b5df3.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Heading.759b5df3.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/Indicator.svelte_svelte_type_style_lang.e2c519f7.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Indicator.svelte_svelte_type_style_lang.e2c519f7.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/Modal.b90503ef.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Modal.b90503ef.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/SimpleGrid.f308d3bd.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/SimpleGrid.f308d3bd.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/Space.5d3c5051.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Space.5d3c5051.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/TableHeadCell.a7fa45f2.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/TableHeadCell.a7fa45f2.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/Textarea.17eddb3d.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Textarea.17eddb3d.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/Trash.33219cd3.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Trash.33219cd3.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/combinator.becf7b0b.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/combinator.becf7b0b.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/index.5b757cee.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/index.5b757cee.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/index.b7a14a97.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/index.b7a14a97.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/index.d8ca07a9.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/index.d8ca07a9.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/navigation.8bb60df9.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/navigation.8bb60df9.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/singletons.3dbe6478.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/singletons.3dbe6478.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/store.4d7a1ebc.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/store.4d7a1ebc.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/store.6cd3ab0e.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/store.6cd3ab0e.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/chunks/store.c28f1804.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/store.c28f1804.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/entry/app.34f7a124.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/entry/app.34f7a124.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/entry/start.07ad94a0.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/entry/start.07ad94a0.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/nodes/0.51906aee.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/0.51906aee.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/nodes/1.e22fd99e.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/1.e22fd99e.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/nodes/2.7284b9d4.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/2.7284b9d4.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/nodes/3.510394aa.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/3.510394aa.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/nodes/4.828fc947.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/4.828fc947.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/nodes/5.faf63ad8.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/5.faf63ad8.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/nodes/6.c31223f5.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/6.c31223f5.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/nodes/7.56d911fb.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/7.56d911fb.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -898,26 +898,26 @@
 }
 
 function hl(f) {
     let e, l, t, n, r, s, a;
     return {
         c() {
             e = G("span"), l = g(f[13]), t = g("."), n = g(` Go to
-		`), r = G("a"), s = g("COHORT DEFITION"), a = g(" section."), this.h()
+		`), r = G("a"), s = g("COHORT DEFINITION"), a = g(" section."), this.h()
         },
         l(o) {
             e = L(o, "SPAN", {});
             var u = A(e);
             l = v(u, f[13]), t = v(u, "."), u.forEach(i), n = v(o, ` Go to
 		`), r = L(o, "A", {
                 href: !0,
                 class: !0
             });
             var z = A(r);
-            s = v(z, "COHORT DEFITION"), z.forEach(i), a = v(o, " section."), this.h()
+            s = v(z, "COHORT DEFINITION"), z.forEach(i), a = v(o, " section."), this.h()
         },
         h() {
             m(r, "href", "/cohort"), m(r, "class", "font-semibold underline hover:text-red-800 dark:hover:text-red-900")
         },
         m(o, u) {
             c(o, e, u), O(e, l), O(e, t), c(o, n, u), c(o, r, u), O(r, s), c(o, a, u)
         },
@@ -1016,26 +1016,26 @@
 }
 
 function vl(f) {
     let e, l, t, n, r, s, a;
     return {
         c() {
             e = G("span"), l = g(f[15]), t = g("."), n = g(` Go to
-		`), r = G("a"), s = g("COHORT DEFITION"), a = g(" section."), this.h()
+		`), r = G("a"), s = g("COHORT DEFINITION"), a = g(" section."), this.h()
         },
         l(o) {
             e = L(o, "SPAN", {});
             var u = A(e);
             l = v(u, f[15]), t = v(u, "."), u.forEach(i), n = v(o, ` Go to
 		`), r = L(o, "A", {
                 href: !0,
                 class: !0
             });
             var z = A(r);
-            s = v(z, "COHORT DEFITION"), z.forEach(i), a = v(o, " section."), this.h()
+            s = v(z, "COHORT DEFINITION"), z.forEach(i), a = v(o, " section."), this.h()
         },
         h() {
             m(r, "href", "/cohort"), m(r, "class", "font-semibold underline hover:text-red-800 dark:hover:text-red-900")
         },
         m(o, u) {
             c(o, e, u), O(e, l), O(e, t), c(o, n, u), c(o, r, u), O(r, s), c(o, a, u)
         },
@@ -1134,26 +1134,26 @@
 }
 
 function kl(f) {
     let e, l, t, n, r, s, a;
     return {
         c() {
             e = G("span"), l = g(f[17]), t = g("."), n = g(` Go to
-		`), r = G("a"), s = g("COHORT DEFITION"), a = g(" section."), this.h()
+		`), r = G("a"), s = g("COHORT DEFINITION"), a = g(" section."), this.h()
         },
         l(o) {
             e = L(o, "SPAN", {});
             var u = A(e);
             l = v(u, f[17]), t = v(u, "."), u.forEach(i), n = v(o, ` Go to
 		`), r = L(o, "A", {
                 href: !0,
                 class: !0
             });
             var z = A(r);
-            s = v(z, "COHORT DEFITION"), z.forEach(i), a = v(o, " section."), this.h()
+            s = v(z, "COHORT DEFINITION"), z.forEach(i), a = v(o, " section."), this.h()
         },
         h() {
             m(r, "href", "/cohort"), m(r, "class", "font-semibold underline hover:text-red-800 dark:hover:text-red-900")
         },
         m(o, u) {
             c(o, e, u), O(e, l), O(e, t), c(o, n, u), c(o, r, u), O(r, s), c(o, a, u)
         },
@@ -1246,27 +1246,27 @@
 
 function Cl(f) {
     let e, l, t, n, r, s;
     return {
         c() {
             e = G("span"), l = g("The entity name cannot contain spaces and is a required field."), t = g(`
 		Go to
-		`), n = G("a"), r = g("ENTITIES DEFITION"), s = g(" section."), this.h()
+		`), n = G("a"), r = g("ENTITIES DEFINITION"), s = g(" section."), this.h()
         },
         l(a) {
             e = L(a, "SPAN", {});
             var o = A(e);
             l = v(o, "The entity name cannot contain spaces and is a required field."), o.forEach(i), t = v(a, `
 		Go to
 		`), n = L(a, "A", {
                 href: !0,
                 class: !0
             });
             var u = A(n);
-            r = v(u, "ENTITIES DEFITION"), u.forEach(i), s = v(a, " section."), this.h()
+            r = v(u, "ENTITIES DEFINITION"), u.forEach(i), s = v(a, " section."), this.h()
         },
         h() {
             m(n, "href", "/entities"), m(n, "class", "font-semibold underline hover:text-red-800 dark:hover:text-red-900")
         },
         m(a, o) {
             c(a, e, o), O(e, l), c(a, t, o), c(a, n, o), O(n, r), c(a, s, o)
         },
@@ -1358,28 +1358,28 @@
 function zl(f) {
     let e, l, t, n, r, s;
     return {
         c() {
             e = G("span"), l = g(`Check the name of your entities. There cannot be two entities with
 			the same name..`), t = g(`
 		Go to
-		`), n = G("a"), r = g("ENTITIES DEFITION"), s = g(" section."), this.h()
+		`), n = G("a"), r = g("ENTITIES DEFINITION"), s = g(" section."), this.h()
         },
         l(a) {
             e = L(a, "SPAN", {});
             var o = A(e);
             l = v(o, `Check the name of your entities. There cannot be two entities with
 			the same name..`), o.forEach(i), t = v(a, `
 		Go to
 		`), n = L(a, "A", {
                 href: !0,
                 class: !0
             });
             var u = A(n);
-            r = v(u, "ENTITIES DEFITION"), u.forEach(i), s = v(a, " section."), this.h()
+            r = v(u, "ENTITIES DEFINITION"), u.forEach(i), s = v(a, " section."), this.h()
         },
         h() {
             m(n, "href", "/entities"), m(n, "class", "font-semibold underline hover:text-red-800 dark:hover:text-red-900")
         },
         m(a, o) {
             c(a, e, o), O(e, l), c(a, t, o), c(a, n, o), O(n, r), c(a, s, o)
         },
@@ -1469,26 +1469,26 @@
 }
 
 function Dl(f) {
     let e, l, t, n, r, s;
     return {
         c() {
             e = G("span"), l = g("Every entity must have at least one variable."), t = g(` Go to
-		`), n = G("a"), r = g("ENTITIES DEFITION"), s = g(" section."), this.h()
+		`), n = G("a"), r = g("ENTITIES DEFINITION"), s = g(" section."), this.h()
         },
         l(a) {
             e = L(a, "SPAN", {});
             var o = A(e);
             l = v(o, "Every entity must have at least one variable."), o.forEach(i), t = v(a, ` Go to
 		`), n = L(a, "A", {
                 href: !0,
                 class: !0
             });
             var u = A(n);
-            r = v(u, "ENTITIES DEFITION"), u.forEach(i), s = v(a, " section."), this.h()
+            r = v(u, "ENTITIES DEFINITION"), u.forEach(i), s = v(a, " section."), this.h()
         },
         h() {
             m(n, "href", "/entities"), m(n, "class", "font-semibold underline hover:text-red-800 dark:hover:text-red-900")
         },
         m(a, o) {
             c(a, e, o), O(e, l), c(a, t, o), c(a, n, o), O(n, r), c(a, s, o)
         },
```

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/_app/immutable/nodes/8.ed4ac5b3.js` & `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/8.ed4ac5b3.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/about.html` & `cdmb-1.1.0/cdmb/ui/static_ui/about.html`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/cohort.html` & `cdmb-1.1.0/cdmb/ui/static_ui/cohort.html`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/entities.html` & `cdmb-1.1.0/cdmb/ui/static_ui/entities.html`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/favicon.png` & `cdmb-1.1.0/cdmb/ui/static_ui/favicon.png`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/index.html` & `cdmb-1.1.0/cdmb/ui/static_ui/index.html`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/project.html` & `cdmb-1.1.0/cdmb/ui/static_ui/project.html`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/summary.html` & `cdmb-1.1.0/cdmb/ui/static_ui/summary.html`

 * *Files 0% similar despite different names*

```diff
@@ -96,39 +96,39 @@
 
 
 
 
 <div class="svelteui-c-iGtvjx svelteui-c-iGtvjx-iPJLV-css svelteui-c-PJLV svelteui-c-PJLV-iPJLV-css"></div>
 	<div class="bg-red-50 dark:bg-gray-800 text-red-800 dark:text-red-400 border-red-300 dark:border-red-800 p-4 text-sm border-t-4 " role="alert"><div class="flex items-center"><span slot="icon"><svg aria-hidden="true" class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M18 10a8 8 0 11-16 0 8 8 0 0116 0zm-7-4a1 1 0 11-2 0 1 1 0 012 0zM9 9a1 1 0 000 2v3a1 1 0 001 1h1a1 1 0 100-2v-3a1 1 0 00-1-1H9z" clip-rule="evenodd"></path></svg></span>
     <div class="ml-3"><span>Cohort name is a required input.</span> Go to
-		<a href="/cohort" class="font-semibold underline hover:text-red-800 dark:hover:text-red-900">COHORT DEFITION</a> section.
+		<a href="/cohort" class="font-semibold underline hover:text-red-800 dark:hover:text-red-900">COHORT DEFINITION</a> section.
 	</div>
 
     </div>
   </div>
 
 
 
 
 <div class="svelteui-c-iGtvjx svelteui-c-iGtvjx-iPJLV-css svelteui-c-PJLV svelteui-c-PJLV-iPJLV-css"></div>
 	<div class="bg-red-50 dark:bg-gray-800 text-red-800 dark:text-red-400 border-red-300 dark:border-red-800 p-4 text-sm border-t-4 " role="alert"><div class="flex items-center"><span slot="icon"><svg aria-hidden="true" class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M18 10a8 8 0 11-16 0 8 8 0 0116 0zm-7-4a1 1 0 11-2 0 1 1 0 012 0zM9 9a1 1 0 000 2v3a1 1 0 001 1h1a1 1 0 100-2v-3a1 1 0 00-1-1H9z" clip-rule="evenodd"></path></svg></span>
     <div class="ml-3"><span>Inclusion criteria is a required input.</span> Go to
-		<a href="/cohort" class="font-semibold underline hover:text-red-800 dark:hover:text-red-900">COHORT DEFITION</a> section.
+		<a href="/cohort" class="font-semibold underline hover:text-red-800 dark:hover:text-red-900">COHORT DEFINITION</a> section.
 	</div>
 
     </div>
   </div>
 
 
 
 
 <div class="svelteui-c-iGtvjx svelteui-c-iGtvjx-iPJLV-css svelteui-c-PJLV svelteui-c-PJLV-iPJLV-css"></div>
 	<div class="bg-red-50 dark:bg-gray-800 text-red-800 dark:text-red-400 border-red-300 dark:border-red-800 p-4 text-sm border-t-4 " role="alert"><div class="flex items-center"><span slot="icon"><svg aria-hidden="true" class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M18 10a8 8 0 11-16 0 8 8 0 0116 0zm-7-4a1 1 0 11-2 0 1 1 0 012 0zM9 9a1 1 0 000 2v3a1 1 0 001 1h1a1 1 0 100-2v-3a1 1 0 00-1-1H9z" clip-rule="evenodd"></path></svg></span>
     <div class="ml-3"><span>Description is a required input.</span> Go to
-		<a href="/cohort" class="font-semibold underline hover:text-red-800 dark:hover:text-red-900">COHORT DEFITION</a> section.
+		<a href="/cohort" class="font-semibold underline hover:text-red-800 dark:hover:text-red-900">COHORT DEFINITION</a> section.
 	</div>
 
     </div>
   </div>
```

#### html2text {}

```diff
@@ -16,17 +16,17 @@
 [GitHub]
 ****** Summary ******
 Errors found
 Project is a required input. Go to PROJECT section.
 Use case is a required input. Go to PROJECT section.
 Version does not comply with the semantic versioning Semantic Versioning 2.0.0
 format. Go to PROJECT section.
-Cohort name is a required input. Go to COHORT_DEFITION section.
-Inclusion criteria is a required input. Go to COHORT_DEFITION section.
-Description is a required input. Go to COHORT_DEFITION section.
+Cohort name is a required input. Go to COHORT_DEFINITION section.
+Inclusion criteria is a required input. Go to COHORT_DEFINITION section.
+Description is a required input. Go to COHORT_DEFINITION section.
 Main information
 Project         Cohort
                                  Beginning                           Are there
 Project Version Name Description of study   End of study Has         any files
                                  period     period       crosswalks? left to
                                                                      upload?
                                  Wed Jul 05 Wed Jul 05   No          No
```

### Comparing `cdmb-1.0.0/cdmb/ui/static_ui/validation.html` & `cdmb-1.1.0/cdmb/ui/static_ui/validation.html`

 * *Files identical despite different names*

### Comparing `cdmb-1.0.0/pyproject.toml` & `cdmb-1.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cdmb"
-version = "1.0.0"
+version = "1.1.0"
 description = "Common Data Model Builder library"
 authors = [
     "Javier González-Galindo <jgonzalezga.iacs@aragon.es>",
     "Francisco Estupiñan-Romero <festupinnan.iacs@aragon.es>",
     "Santiago Royo-Sierra <sroyo.iacs@aragon.es>"
 ]
```

### Comparing `cdmb-1.0.0/PKG-INFO` & `cdmb-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdmb
-Version: 1.0.0
+Version: 1.1.0
 Summary: Common Data Model Builder library
 Home-page: https://github.com/cienciadedatosysalud/cdmb
 License: CC-BY-NC-4.0
 Keywords: common data model,real-world data,health data,synthetic data,secondary use,health,healthcare
 Author: Javier González-Galindo
 Author-email: jgonzalezga.iacs@aragon.es
 Maintainer: Javier González-Galindo
@@ -31,15 +31,15 @@
 Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: rocrate (>=0.8.0,<0.9.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Project-URL: Repository, https://github.com/cienciadedatosysalud/cdmb
 Description-Content-Type: text/markdown
 
-![Logo of the project](https://cienciadedatosysalud.org/wp-content/uploads/Data-Science-and-VPM.png)
+![Logo of the project](https://cienciadedatosysalud.org/wp-content/uploads/logo-Data-Science-VPM.png)
 - [Common Data Model Builder (cdmb)](#common-data-model-builder-cdmb)
 - [User Interface](#user-interface)
 - [Outputs](#outputs)
 - [Classes](#classes)
   - [Metadata](#metadata)
   - [Author](#author)
   - [Cohort](#cohort)
@@ -85,14 +85,27 @@
 port = 8000
 
 launch_ui(server_address, port)
 # Open your web browser at http://<server_address>:<port>.
 # http://localhost:8000
 ```
 
+# Run in Docker
+Alternatively you can run the graphical interface provided by the Common Data Model Builder directly in a docker container.
+
+Use the following code snippet to create the container.
+```bash
+docker pull ghcr.io/cienciadedatosysalud/cdmb:latest
+
+docker run -p 127.0.0.1:8501:8501 --name cdmb_ui ghcr.io/cienciadedatosysalud/cdmb:latest
+
+# Open your web browser at http://localhost:8501.
+```
+
+
 # Outputs
 Outputs structure and content is described below including the files and folders that are generated when creating a research project with the `cdmb` Python library. There are four main folders corresponding to:
 
 - __docs/CDM/__
   - **cdmb_config.json**: Configuration file.
   - **cohort_definition_inclusion.csv**: csv file that defines the criteria (i.e., codes) for inclusion in a cohort.
   - **cohort_definition_exclusion.csv**: csv file that defines the criteria (i.e., codes) for exclusion in a cohort.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cdmb Version: 1.0.0 Summary: Common Data Model
+Metadata-Version: 2.1 Name: cdmb Version: 1.1.0 Summary: Common Data Model
 Builder library Home-page: https://github.com/cienciadedatosysalud/cdmb
 License: CC-BY-NC-4.0 Keywords: common data model,real-world data,health
 data,synthetic data,secondary use,health,healthcare Author: Javier GonzÃ¡lez-
 Galindo Author-email: jgonzalezga.iacs@aragon.es Maintainer: Javier GonzÃ¡lez-
 Galindo Maintainer-email: jgonzalezga.iacs@aragon.es Requires-Python:
 >=3.9,<4.0 Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Healthcare Industry Classifier: Intended Audience :: Science/
@@ -16,16 +16,16 @@
 Modules Requires-Dist: duckdb (>=0.8.1,<0.9.0) Requires-Dist: faker
 (>=18.11.2,<19.0.0) Requires-Dist: fastapi (>=0.99.1,<0.100.0) Requires-Dist:
 graphviz (>=0.20.1,<0.21.0) Requires-Dist: openpyxl (>=3.1.2,<4.0.0) Requires-
 Dist: pandas (>=2.0.3,<3.0.0) Requires-Dist: pytest (>=7.4.0,<8.0.0) Requires-
 Dist: python-multipart (>=0.0.6,<0.0.7) Requires-Dist: rocrate (>=0.8.0,<0.9.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0) Project-URL: Repository, https://
 github.com/cienciadedatosysalud/cdmb Description-Content-Type: text/markdown !
-[Logo of the project](https://cienciadedatosysalud.org/wp-content/uploads/Data-
-Science-and-VPM.png) - [Common Data Model Builder (cdmb)](#common-data-model-
+[Logo of the project](https://cienciadedatosysalud.org/wp-content/uploads/logo-
+Data-Science-VPM.png) - [Common Data Model Builder (cdmb)](#common-data-model-
 builder-cdmb) - [User Interface](#user-interface) - [Outputs](#outputs) -
 [Classes](#classes) - [Metadata](#metadata) - [Author](#author) - [Cohort]
 (#cohort) - [Crosswalks](#crosswalks) - [Entities](#entities) - [Variables]
 (#variables) - [Catalogs](#catalogs) - [Rules Set](#rules-set) - [Rules]
 (#rules) - [Comparison rule](#comparison-rule) - [BetweenComparison]
 (#betweencomparison) - [NullCheckingRule](#nullcheckingrule) - [InValuesRule]
 (#invaluesrule) - [ComposedRule](#composedrule) - [DummyRule](#dummyrule) -
@@ -44,31 +44,37 @@
 functionalities of Common Data Model Builder is to provide the user with a
 graphical interface to fill in the Common Data Model and export it in a simple
 way. Follow the following code snippet to access it. #### Inputs: -
 **server_address**: a string representing the server address, default value is
 "localhost" - **port**: a string representing the server port, default value is
 "8501" #### Example: ```python from cdmb import launch_ui server_address =
 "localhost" port = 8000 launch_ui(server_address, port) # Open your web browser
-at http://:. # http://localhost:8000 ``` # Outputs Outputs structure and
-content is described below including the files and folders that are generated
-when creating a research project with the `cdmb` Python library. There are four
-main folders corresponding to: - __docs/CDM/__ - **cdmb_config.json**:
-Configuration file. - **cohort_definition_inclusion.csv**: csv file that
-defines the criteria (i.e., codes) for inclusion in a cohort. -
-**cohort_definition_exclusion.csv**: csv file that defines the criteria (i.e.,
-codes) for exclusion in a cohort. - **common_datamodel.xlsx**: The definition
-of the common data model in Excel format. - **entities/**: Folder structure
-where, for each defined entity, the catalogs and the established validation
-rules are stored. - **ER.gv, ER.gv.png**: an Entity-Relationship Diagram of the
-entities included in the CDM. - **synthetic-data/**: Folder structure contaning
-an automatically generated set of 1000 synthetic records per entity included en
-the CDM. - **hashed_files_list.json**: List of the files generated or used
-after generating the project with their md5 hash. This file must be kept hidden
-and should be used to cross-check with the results obtained from the analysis
-from the original input files. - __inputs/__ - **data.duckdb**: Database that
+at http://:. # http://localhost:8000 ``` # Run in Docker Alternatively you can
+run the graphical interface provided by the Common Data Model Builder directly
+in a docker container. Use the following code snippet to create the container.
+```bash docker pull ghcr.io/cienciadedatosysalud/cdmb:latest docker run -
+p 127.0.0.1:8501:8501 --name cdmb_ui ghcr.io/cienciadedatosysalud/cdmb:latest #
+Open your web browser at http://localhost:8501. ``` # Outputs Outputs structure
+and content is described below including the files and folders that are
+generated when creating a research project with the `cdmb` Python library.
+There are four main folders corresponding to: - __docs/CDM/__ -
+**cdmb_config.json**: Configuration file. -
+**cohort_definition_inclusion.csv**: csv file that defines the criteria (i.e.,
+codes) for inclusion in a cohort. - **cohort_definition_exclusion.csv**: csv
+file that defines the criteria (i.e., codes) for exclusion in a cohort. -
+**common_datamodel.xlsx**: The definition of the common data model in Excel
+format. - **entities/**: Folder structure where, for each defined entity, the
+catalogs and the established validation rules are stored. - **ER.gv,
+ER.gv.png**: an Entity-Relationship Diagram of the entities included in the
+CDM. - **synthetic-data/**: Folder structure contaning an automatically
+generated set of 1000 synthetic records per entity included en the CDM. -
+**hashed_files_list.json**: List of the files generated or used after
+generating the project with their md5 hash. This file must be kept hidden and
+should be used to cross-check with the results obtained from the analysis from
+the original input files. - __inputs/__ - **data.duckdb**: Database that
 temporarily contains the data entered by the user (synthetic data by default) -
 __outputs/__ - (Default directory of all the outputs produced in the project
 execution) - __src/__ - __analysis-scripts/__ - (directory where the analysis
 scripts developed by the user are stored) - **r_report_template.qmd**: Quarto
 document, with an example analysis, showing the interaction with the folder
 structure and files generated in the project. - **_quarto.yml**: File
 containing the Metadata to execute Quarto documents. - __check_load-scripts/__
```

