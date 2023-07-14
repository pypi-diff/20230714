# Comparing `tmp/libcoveweb-0.27.0.tar.gz` & `tmp/libcoveweb-0.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libcoveweb-0.27.0.tar", last modified: Mon Mar  6 16:26:05 2023, max compression
+gzip compressed data, was "libcoveweb-0.28.0.tar", last modified: Fri Jul 14 13:58:38 2023, max compression
```

## Comparing `libcoveweb-0.27.0.tar` & `libcoveweb-0.28.0.tar`

### file list

```diff
@@ -1,200 +1,201 @@
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.490204 libcoveweb-0.27.0/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2141 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/LICENCE.rst
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      410 2023-03-06 16:26:05.490204 libcoveweb-0.27.0/PKG-INFO
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3483 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/README.md
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.450204 libcoveweb-0.27.0/cove/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/__init__.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      544 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/context_processors.py
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.450204 libcoveweb-0.27.0/cove/fixtures/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/fixtures/bad.xlsx
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    25816 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/fixtures/badfile.json
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     5771 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/fixtures/basic.xlsx
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)       65 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/fixtures/utf8.json
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     9401 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/html_error_msg.py
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.450204 libcoveweb-0.27.0/cove/input/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/input/__init__.py
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.454203 libcoveweb-0.27.0/cove/input/migrations/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      565 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/input/migrations/0001_initial.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      455 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/input/migrations/0002_supplieddata_current_app.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      893 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/input/migrations/0003_auto_20150506_1649.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      462 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/input/migrations/0004_auto_20150908_1533.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      422 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/input/migrations/0005_auto_20160104_1208.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      444 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/input/migrations/0006_supplieddata_rendered.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      591 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/input/migrations/0007_supplied_data_schema_version.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      488 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/input/migrations/0008_supplieddata_data_schema_version.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      415 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/input/migrations/0009_supplieddata_parameters.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/input/migrations/__init__.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3863 2023-03-06 16:25:33.000000 libcoveweb-0.27.0/cove/input/models.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3745 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/input/views.py
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.454203 libcoveweb-0.27.0/cove/lib/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/lib/__init__.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1992 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/lib/common.py
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.446204 libcoveweb-0.27.0/cove/locale/
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.446204 libcoveweb-0.27.0/cove/locale/en/
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.454203 libcoveweb-0.27.0/cove/locale/en/LC_MESSAGES/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      337 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    13391 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.446204 libcoveweb-0.27.0/cove/locale/es/
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.454203 libcoveweb-0.27.0/cove/locale/es/LC_MESSAGES/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    13337 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    19509 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.454203 libcoveweb-0.27.0/cove/management/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/management/__init__.py
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.458204 libcoveweb-0.27.0/cove/management/commands/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/management/commands/__init__.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1594 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/management/commands/base_command.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      649 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/management/commands/expire_files.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1370 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/management/commands/tests.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      592 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/management/commands/upload.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      354 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/middleware.py
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.446204 libcoveweb-0.27.0/cove/sass/
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.458204 libcoveweb-0.27.0/cove/sass/bootstrap/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      178 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/_bootstrap-compass.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      757 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/_bootstrap-mincer.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      168 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/_bootstrap-sprockets.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1486 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/_bootstrap.scss
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.470204 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1550 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_alerts.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1228 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_badges.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      700 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_breadcrumbs.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     5758 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_button-groups.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3819 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_buttons.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     5725 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_carousel.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      815 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_close.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1401 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_code.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      819 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_component-animations.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4889 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_dropdowns.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    16162 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_forms.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    20448 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_glyphicons.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1443 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_grid.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4313 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_input-groups.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1152 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_jumbotron.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1156 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_labels.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3172 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_list-group.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      900 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_media.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      986 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_mixins.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3568 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_modals.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    14729 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_navbar.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4950 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_navs.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     7559 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_normalize.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      855 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_pager.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2091 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_pagination.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     6385 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_panels.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3502 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_popovers.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1939 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_print.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1992 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_progress-bars.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      546 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_responsive-embed.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4409 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_responsive-utilities.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3031 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_scaffolding.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4662 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_tables.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     8558 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_theme.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      892 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_thumbnails.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3007 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_tooltip.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     6149 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_type.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      765 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_utilities.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    31290 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_variables.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      535 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_wells.scss
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.478204 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      263 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_alerts.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      233 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_background-variant.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      492 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_border-radius.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1453 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_buttons.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      126 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_center-block.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      611 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_clearfix.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2771 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_forms.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4392 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_gradients.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2360 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_grid-framework.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3216 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_grid.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      590 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_hide-text.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1208 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_image.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      167 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_labels.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      672 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_list-group.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      238 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_nav-divider.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      370 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_nav-vertical-align.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      149 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_opacity.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      507 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_pagination.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      543 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_panels.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      200 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_progress-bar.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      246 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_reset-filter.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      476 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_reset-text.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      202 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_resize.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      514 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_responsive-visibility.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      147 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_size.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      338 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_tab-focus.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      715 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_table-row.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      210 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_text-emphasis.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      168 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_text-overflow.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     6645 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_vendor-prefixes.scss
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4941 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/settings.py
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.446204 libcoveweb-0.27.0/cove/static/
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.446204 libcoveweb-0.27.0/cove/static/dataexplore/
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.478204 libcoveweb-0.27.0/cove/static/dataexplore/css/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1833 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/static/dataexplore/css/style.css
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.446204 libcoveweb-0.27.0/cove/static/dataexplore/fonts/
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.478204 libcoveweb-0.27.0/cove/static/dataexplore/fonts/bootstrap/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    20127 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.eot
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)   108738 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.svg
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    45404 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    23424 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    18028 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff2
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.482204 libcoveweb-0.27.0/cove/static/dataexplore/fonts/tick/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      408 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/static/dataexplore/fonts/tick/tick.css
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2328 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/static/dataexplore/fonts/tick/tick.eot
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3063 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/static/dataexplore/fonts/tick/tick.svg
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2168 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/static/dataexplore/fonts/tick/tick.ttf
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1604 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/static/dataexplore/fonts/tick/tick.woff
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1064 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/static/dataexplore/fonts/tick/tick.woff2
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.490204 libcoveweb-0.27.0/cove/templates/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1114 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/500.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      949 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/additional_codelist_values.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      405 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/additional_fields_table.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2722 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/additional_fields_table_all.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4938 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/base.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      748 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/error.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      405 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/error_extra.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2431 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/explore.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      479 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/google_analytics.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3845 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/input.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3004 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/modal_errors.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      534 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/modal_list.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1647 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/page_header.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1157 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/piwik.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1092 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/stats.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1034 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1954 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_conditions.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2351 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_conditions_intro.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2043 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_cookies.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      195 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_cookies_link_google_analytics.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      124 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_cookies_link_matmo.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      105 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_cookies_links.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      484 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_cookies_we_use.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      830 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_data_deleting.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      764 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_data_uploaded.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1357 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_disclaimer.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      525 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_links.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1448 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_privacy.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1165 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_privacy_intro.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      279 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_security.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_tracker_data_controller_international.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      804 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_tracker_google_analytics.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1197 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_tracker_matmo.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)       81 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_tracker_no_international.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      969 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_tracker_sentry.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      856 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_tracker_server.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      427 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/terms_trackers.html
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2506 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templates/validation_table.html
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.490204 libcoveweb-0.27.0/cove/templatetags/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templatetags/__init__.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1690 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/templatetags/cove_tags.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     9021 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/tests.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      983 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/cove/urls.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     5116 2023-03-06 12:52:05.000000 libcoveweb-0.27.0/cove/views.py
-drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-03-06 16:26:05.490204 libcoveweb-0.27.0/libcoveweb.egg-info/
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      410 2023-03-06 16:26:05.000000 libcoveweb-0.27.0/libcoveweb.egg-info/PKG-INFO
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     7192 2023-03-06 16:26:05.000000 libcoveweb-0.27.0/libcoveweb.egg-info/SOURCES.txt
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        1 2023-03-06 16:26:05.000000 libcoveweb-0.27.0/libcoveweb.egg-info/dependency_links.txt
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      230 2023-03-06 16:26:05.000000 libcoveweb-0.27.0/libcoveweb.egg-info/requires.txt
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        5 2023-03-06 16:26:05.000000 libcoveweb-0.27.0/libcoveweb.egg-info/top_level.txt
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      247 2023-01-12 10:32:22.000000 libcoveweb-0.27.0/manage.py
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      147 2023-03-06 16:26:05.494204 libcoveweb-0.27.0/setup.cfg
--rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1367 2023-03-06 16:25:33.000000 libcoveweb-0.27.0/setup.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.693714 libcoveweb-0.28.0/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2141 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/LICENCE.rst
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      410 2023-07-14 13:58:38.693714 libcoveweb-0.28.0/PKG-INFO
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3483 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/README.md
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.657714 libcoveweb-0.28.0/cove/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/__init__.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      544 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/context_processors.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.657714 libcoveweb-0.28.0/cove/fixtures/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/fixtures/bad.xlsx
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    25816 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/fixtures/badfile.json
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     5771 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/fixtures/basic.xlsx
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)       65 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/fixtures/utf8.json
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     9401 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/html_error_msg.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.657714 libcoveweb-0.28.0/cove/input/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/input/__init__.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.661714 libcoveweb-0.28.0/cove/input/migrations/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      565 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/input/migrations/0001_initial.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      455 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/input/migrations/0002_supplieddata_current_app.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      893 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/input/migrations/0003_auto_20150506_1649.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      462 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/input/migrations/0004_auto_20150908_1533.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      422 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/input/migrations/0005_auto_20160104_1208.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      444 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/input/migrations/0006_supplieddata_rendered.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      591 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/input/migrations/0007_supplied_data_schema_version.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      488 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/input/migrations/0008_supplieddata_data_schema_version.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      415 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/input/migrations/0009_supplieddata_parameters.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      468 2023-07-12 16:53:34.000000 libcoveweb-0.28.0/cove/input/migrations/0010_alter_supplieddata_original_file.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/input/migrations/__init__.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3863 2023-03-06 16:25:33.000000 libcoveweb-0.28.0/cove/input/models.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3745 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/input/views.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.661714 libcoveweb-0.28.0/cove/lib/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/lib/__init__.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1992 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/lib/common.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.653714 libcoveweb-0.28.0/cove/locale/
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.653714 libcoveweb-0.28.0/cove/locale/en/
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.661714 libcoveweb-0.28.0/cove/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      337 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    13391 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.653714 libcoveweb-0.28.0/cove/locale/es/
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.661714 libcoveweb-0.28.0/cove/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    13344 2023-07-12 16:53:51.000000 libcoveweb-0.28.0/cove/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    19516 2023-07-12 16:53:51.000000 libcoveweb-0.28.0/cove/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.661714 libcoveweb-0.28.0/cove/management/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/management/__init__.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.665714 libcoveweb-0.28.0/cove/management/commands/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/management/commands/__init__.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1594 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/management/commands/base_command.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      649 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/management/commands/expire_files.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1370 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/management/commands/tests.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      592 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/management/commands/upload.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      354 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/middleware.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.653714 libcoveweb-0.28.0/cove/sass/
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.665714 libcoveweb-0.28.0/cove/sass/bootstrap/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      178 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/_bootstrap-compass.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      757 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/_bootstrap-mincer.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      168 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/_bootstrap-sprockets.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1486 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/_bootstrap.scss
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.673714 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1550 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_alerts.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1228 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_badges.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      700 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_breadcrumbs.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     5758 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_button-groups.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3819 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_buttons.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     5725 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_carousel.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      815 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_close.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1401 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_code.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      819 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_component-animations.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4889 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_dropdowns.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    16162 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_forms.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    20448 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_glyphicons.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1443 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_grid.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4313 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_input-groups.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1152 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_jumbotron.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1156 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_labels.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3172 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_list-group.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      900 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_media.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      986 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_mixins.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3568 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_modals.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    14729 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_navbar.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4950 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_navs.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     7559 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_normalize.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      855 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_pager.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2091 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_pagination.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     6385 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_panels.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3502 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_popovers.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1939 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_print.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1992 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_progress-bars.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      546 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_responsive-embed.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4409 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_responsive-utilities.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3031 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_scaffolding.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4662 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_tables.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     8558 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_theme.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      892 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_thumbnails.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3007 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_tooltip.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     6149 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_type.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      765 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_utilities.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    31290 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_variables.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      535 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_wells.scss
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.681714 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      263 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_alerts.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      233 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_background-variant.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      492 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_border-radius.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1453 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_buttons.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      126 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_center-block.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      611 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_clearfix.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2771 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_forms.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4392 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_gradients.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2360 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_grid-framework.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3216 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_grid.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      590 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_hide-text.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1208 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_image.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      167 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_labels.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      672 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_list-group.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      238 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_nav-divider.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      370 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_nav-vertical-align.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      149 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_opacity.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      507 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_pagination.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      543 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_panels.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      200 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_progress-bar.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      246 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_reset-filter.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      476 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_reset-text.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      202 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_resize.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      514 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_responsive-visibility.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      147 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_size.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      338 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_tab-focus.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      715 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_table-row.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      210 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_text-emphasis.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      168 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_text-overflow.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     6645 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_vendor-prefixes.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4941 2023-07-07 14:22:33.000000 libcoveweb-0.28.0/cove/settings.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.653714 libcoveweb-0.28.0/cove/static/
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.653714 libcoveweb-0.28.0/cove/static/dataexplore/
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.681714 libcoveweb-0.28.0/cove/static/dataexplore/css/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1833 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/static/dataexplore/css/style.css
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.653714 libcoveweb-0.28.0/cove/static/dataexplore/fonts/
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.685714 libcoveweb-0.28.0/cove/static/dataexplore/fonts/bootstrap/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    20127 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.eot
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)   108738 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.svg
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    45404 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.ttf
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    23424 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    18028 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff2
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.685714 libcoveweb-0.28.0/cove/static/dataexplore/fonts/tick/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      408 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/static/dataexplore/fonts/tick/tick.css
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2328 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/static/dataexplore/fonts/tick/tick.eot
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3063 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/static/dataexplore/fonts/tick/tick.svg
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2168 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/static/dataexplore/fonts/tick/tick.ttf
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1604 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/static/dataexplore/fonts/tick/tick.woff
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1064 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/static/dataexplore/fonts/tick/tick.woff2
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.693714 libcoveweb-0.28.0/cove/templates/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1114 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/500.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      949 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/additional_codelist_values.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      405 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/additional_fields_table.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2722 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/additional_fields_table_all.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4938 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/base.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      748 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/error.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      405 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/error_extra.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2431 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/explore.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      479 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/google_analytics.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3845 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/input.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3004 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/modal_errors.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      534 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/modal_list.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1647 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/page_header.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1157 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/piwik.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1092 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/stats.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1034 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1954 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_conditions.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2351 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_conditions_intro.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2043 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_cookies.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      195 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_cookies_link_google_analytics.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      124 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_cookies_link_matmo.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      105 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_cookies_links.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      484 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_cookies_we_use.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      830 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_data_deleting.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      764 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_data_uploaded.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1357 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_disclaimer.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      525 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_links.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1448 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_privacy.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1165 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_privacy_intro.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      279 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_security.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_tracker_data_controller_international.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      804 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_tracker_google_analytics.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1197 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_tracker_matmo.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)       81 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_tracker_no_international.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      969 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_tracker_sentry.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      856 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_tracker_server.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      427 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/terms_trackers.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2506 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templates/validation_table.html
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.693714 libcoveweb-0.28.0/cove/templatetags/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templatetags/__init__.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1690 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/templatetags/cove_tags.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     9021 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/tests.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      983 2023-01-12 10:32:22.000000 libcoveweb-0.28.0/cove/urls.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     5116 2023-03-06 12:52:05.000000 libcoveweb-0.28.0/cove/views.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2023-07-14 13:58:38.693714 libcoveweb-0.28.0/libcoveweb.egg-info/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      410 2023-07-14 13:58:38.000000 libcoveweb-0.28.0/libcoveweb.egg-info/PKG-INFO
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     7255 2023-07-14 13:58:38.000000 libcoveweb-0.28.0/libcoveweb.egg-info/SOURCES.txt
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        1 2023-07-14 13:58:38.000000 libcoveweb-0.28.0/libcoveweb.egg-info/dependency_links.txt
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      230 2023-07-14 13:58:38.000000 libcoveweb-0.28.0/libcoveweb.egg-info/requires.txt
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        5 2023-07-14 13:58:38.000000 libcoveweb-0.28.0/libcoveweb.egg-info/top_level.txt
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)      247 2023-07-12 16:53:34.000000 libcoveweb-0.28.0/manage.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      147 2023-07-14 13:58:38.693714 libcoveweb-0.28.0/setup.cfg
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1367 2023-07-12 17:05:44.000000 libcoveweb-0.28.0/setup.py
```

### Comparing `libcoveweb-0.27.0/LICENCE.rst` & `libcoveweb-0.28.0/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/README.md` & `libcoveweb-0.28.0/README.md`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/context_processors.py` & `libcoveweb-0.28.0/cove/context_processors.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/fixtures/badfile.json` & `libcoveweb-0.28.0/cove/fixtures/badfile.json`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/fixtures/basic.xlsx` & `libcoveweb-0.28.0/cove/fixtures/basic.xlsx`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/html_error_msg.py` & `libcoveweb-0.28.0/cove/html_error_msg.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/input/migrations/0001_initial.py` & `libcoveweb-0.28.0/cove/input/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/input/migrations/0003_auto_20150506_1649.py` & `libcoveweb-0.28.0/cove/input/migrations/0003_auto_20150506_1649.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/input/migrations/0007_supplied_data_schema_version.py` & `libcoveweb-0.28.0/cove/input/migrations/0007_supplied_data_schema_version.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/input/models.py` & `libcoveweb-0.28.0/cove/input/models.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/input/views.py` & `libcoveweb-0.28.0/cove/input/views.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/lib/common.py` & `libcoveweb-0.28.0/cove/lib/common.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/locale/en/LC_MESSAGES/django.po` & `libcoveweb-0.28.0/cove/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/locale/es/LC_MESSAGES/django.mo` & `libcoveweb-0.28.0/cove/locale/es/LC_MESSAGES/django.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,15 +9,15 @@
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "%(each)s is a dependency of %(property)s"
-msgstr "%(each)ses una dependencia de %(property)s"
+msgstr "%(each)s es una dependencia de %(property)s"
 
 msgid "%(extras)s does not match any of the regexes: %(patterns)s"
 msgid_plural "%(extras)s do not match any of the regexes: %(patterns)s"
 msgstr[0] ""
 "%(extras)s no coincide con ninguna de las expresiones regulares: %(patterns)s"
 msgstr[1] ""
 "%(extras)s no coinciden con ninguna de las expresiones regulares: "
@@ -28,15 +28,15 @@
 msgstr "%(instance)s es menor o igual que el mínimo de %(validator_value)s"
 
 msgid "%(instance)s is less than the minimum of %(validator_value)s"
 msgstr "%(instance)s es menor que el mínimo de %(validator_value)s"
 
 msgid ""
 "%(instance)s is more than or equal to the maximum of %(validator_value)s"
-msgstr "%(instance)ses mayor o igual que el máximo de %(validator_value)s"
+msgstr "%(instance)s es mayor o igual que el máximo de %(validator_value)s"
 
 msgid "%(instance)s is more than the maximum of %(validator_value)s"
 msgstr "%(instance)s es mayor que el máximo de %(validator_value)s"
 
 msgid "%(instance)s is not a %(validator_value)s"
 msgstr "%(instance)s no es un %(validator_value)s"
 
@@ -52,40 +52,40 @@
 msgid "(See child fields)"
 msgstr "(Vea todos los campos secundarios)"
 
 msgid "(more info)"
 msgstr "(más información)"
 
 msgid "<code>{}</code> does not match the regex <code>{}</code>"
-msgstr "<code>{}</code>no coincide con la expresión regular <code>{}</code>"
+msgstr "<code>{}</code> no coincide con la expresión regular <code>{}</code>"
 
 msgid "<code>{}</code> is missing but required"
-msgstr "<code>{}</code>falta pero se requiere"
+msgstr "<code>{}</code> falta pero se requiere"
 
 msgid "<code>{}</code> is missing but required within <code>{}</code>"
 msgstr "<code>{}</code> falta pero se requiere dentro de <code>{}</code>"
 
 msgid "<code>{}</code> is too long"
-msgstr "<code>{}</code>es muy largo"
+msgstr "<code>{}</code> es muy largo"
 
 msgid "<code>{}</code> is too short"
-msgstr "<code>{}</code>es muy corto"
+msgstr "<code>{}</code> es muy corto"
 
 msgid ""
 "<code>{}</code> is too short. Strings must be at least one character. This "
 "error typically indicates a missing value."
 msgstr ""
-"<code>{}</code>es muy corto. Las cadenas deben ser de al menos un caracter. "
+"<code>{}</code> es muy corto. Las cadenas deben ser de al menos un caracter. "
 "Este error generalmente indica que hay un valor faltante. "
 
 msgid ""
 "<code>{}</code> is too short. You must supply at least one value, or remove "
 "the item entirely (unless it’s required)."
 msgstr ""
-"<code>{}</code>es muy corto. Debe proporcionar al menos un valor o eliminar "
+"<code>{}</code> es muy corto. Debe proporcionar al menos un valor o eliminar "
 "el artículo por completo (a menos que sea necesario)."
 
 msgid "AGPLv3"
 msgstr "AGPLv3"
 
 msgid "About"
 msgstr "Acerca de"
@@ -96,17 +96,16 @@
 msgid "Additional items are not allowed (%s was unexpected)"
 msgid_plural "Additional items are not allowed (%s were unexpected)"
 msgstr[0] "Items adicionales no están permitidos (%s fue inesperado)"
 msgstr[1] "Items adicionales no están permitidos (%s fueron inesperados)"
 
 msgid "Additional properties are not allowed (%s was unexpected)"
 msgid_plural "Additional properties are not allowed (%s were unexpected)"
-msgstr[0] "Propiedades adicionales no están permitidas (%s fue inesperado )"
-msgstr[1] ""
-"Propiedades adicionales no están permitidas (%s fueron inesperados )"
+msgstr[0] "Propiedades adicionales no están permitidas (%s fue inesperado)"
+msgstr[1] "Propiedades adicionales no están permitidas (%s fueron inesperados)"
 
 msgid "Array Element "
 msgstr "Elemento de matriz"
 
 msgid "Array has non-unique elements"
 msgstr "La matriz tiene elementos no únicos"
 
@@ -449,15 +448,15 @@
 "no deben estar entre comillas."
 
 msgid ""
 "{}<code>{}</code> is not a number. Check that the value {} doesn’t contain "
 "any characters other than 0-9 and dot (<code>.</code>). Number values should "
 "not be in quotes. "
 msgstr ""
-"{}<code>{}</code>no es un número. Compruebe que el valor {} no contenga "
+"{}<code>{}</code> no es un número. Compruebe que el valor {} no contenga "
 "ningún carácter más que 0-9 y el punto (.). Los valores numéricos no deben "
 "estar entre comillas"
 
 msgid ""
 "{}<code>{}</code> is not a string. Check that the value {} has quotes at the "
 "start and end. Escape any quotes in the value with <code>\\</code>"
 msgstr ""
```

### Comparing `libcoveweb-0.27.0/cove/locale/es/LC_MESSAGES/django.po` & `libcoveweb-0.28.0/cove/locale/es/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 #: cove/html_error_msg.py:26
 msgid ""
 "{}<code>{}</code> is not a number. Check that the value {} doesn’t contain "
 "any characters other than 0-9 and dot (<code>.</code>). Number values should"
 " not be in quotes. "
 msgstr ""
-"{}<code>{}</code>no es un número. Compruebe que el valor {} no contenga "
+"{}<code>{}</code> no es un número. Compruebe que el valor {} no contenga "
 "ningún carácter más que 0-9 y el punto (.). Los valores numéricos no deben "
 "estar entre comillas"
 
 #: cove/html_error_msg.py:27
 msgid "{}<code>{}</code> is not a JSON object"
 msgstr "{}<code>{}</code> no es un objeto JSON."
 
@@ -95,47 +95,47 @@
 
 #: cove/html_error_msg.py:88
 msgid "<code>{}</code> is missing but required within <code>{}</code>"
 msgstr "<code>{}</code> falta pero se requiere dentro de <code>{}</code>"
 
 #: cove/html_error_msg.py:94
 msgid "<code>{}</code> is missing but required"
-msgstr "<code>{}</code>falta pero se requiere"
+msgstr "<code>{}</code> falta pero se requiere"
 
 #: cove/html_error_msg.py:98
 msgid "Invalid code found in <code>{}</code>"
 msgstr "Código inválido encontrado en <code>{}</code>"
 
 #: cove/html_error_msg.py:102
 msgid "<code>{}</code> does not match the regex <code>{}</code>"
-msgstr "<code>{}</code>no coincide con la expresión regular <code>{}</code>"
+msgstr "<code>{}</code> no coincide con la expresión regular <code>{}</code>"
 
 #: cove/html_error_msg.py:110
 msgid ""
 "<code>{}</code> is too short. You must supply at least one value, or remove "
 "the item entirely (unless it’s required)."
 msgstr ""
-"<code>{}</code>es muy corto. Debe proporcionar al menos un valor o eliminar "
+"<code>{}</code> es muy corto. Debe proporcionar al menos un valor o eliminar "
 "el artículo por completo (a menos que sea necesario)."
 
 #: cove/html_error_msg.py:115 cove/html_error_msg.py:127
 msgid "<code>{}</code> is too short"
-msgstr "<code>{}</code>es muy corto"
+msgstr "<code>{}</code> es muy corto"
 
 #: cove/html_error_msg.py:122
 msgid ""
 "<code>{}</code> is too short. Strings must be at least one character. This "
 "error typically indicates a missing value."
 msgstr ""
-"<code>{}</code>es muy corto. Las cadenas deben ser de al menos un caracter. "
+"<code>{}</code> es muy corto. Las cadenas deben ser de al menos un caracter. "
 "Este error generalmente indica que hay un valor faltante. "
 
 #: cove/html_error_msg.py:133 cove/html_error_msg.py:139
 msgid "<code>{}</code> is too long"
-msgstr "<code>{}</code>es muy largo"
+msgstr "<code>{}</code> es muy largo"
 
 #: cove/html_error_msg.py:144
 msgid "{} does not have enough properties"
 msgstr "{} no tiene suficientes propiedades"
 
 #: cove/html_error_msg.py:147
 msgid "{} has too many properties"
@@ -152,15 +152,15 @@
 msgid "%(instance)s is less than the minimum of %(validator_value)s"
 msgstr "%(instance)s es menor que el mínimo de %(validator_value)s"
 
 #: cove/html_error_msg.py:163
 #, python-format
 msgid ""
 "%(instance)s is more than or equal to the maximum of %(validator_value)s"
-msgstr "%(instance)ses mayor o igual que el máximo de %(validator_value)s"
+msgstr "%(instance)s es mayor o igual que el máximo de %(validator_value)s"
 
 #: cove/html_error_msg.py:168
 #, python-format
 msgid "%(instance)s is more than the maximum of %(validator_value)s"
 msgstr "%(instance)s es mayor que el máximo de %(validator_value)s"
 
 #: cove/html_error_msg.py:174
@@ -184,15 +184,15 @@
 msgid_plural "Additional items are not allowed (%s were unexpected)"
 msgstr[0] "Items adicionales no están permitidos (%s fue inesperado)"
 msgstr[1] "Items adicionales no están permitidos (%s fueron inesperados)"
 
 #: cove/html_error_msg.py:197
 #, python-format
 msgid "%(each)s is a dependency of %(property)s"
-msgstr "%(each)ses una dependencia de %(property)s"
+msgstr "%(each)s es una dependencia de %(property)s"
 
 #: cove/html_error_msg.py:204
 msgid "Array has non-unique elements"
 msgstr "La matriz tiene elementos no únicos"
 
 #: cove/html_error_msg.py:210
 msgid "Non-unique combination of {} values"
@@ -202,17 +202,17 @@
 msgid "Non-unique {} values"
 msgstr "Valores {} no únicos"
 
 #: cove/html_error_msg.py:217
 #, python-format
 msgid "Additional properties are not allowed (%s was unexpected)"
 msgid_plural "Additional properties are not allowed (%s were unexpected)"
-msgstr[0] "Propiedades adicionales no están permitidas (%s fue inesperado )"
+msgstr[0] "Propiedades adicionales no están permitidas (%s fue inesperado)"
 msgstr[1] ""
-"Propiedades adicionales no están permitidas (%s fueron inesperados )"
+"Propiedades adicionales no están permitidas (%s fueron inesperados)"
 
 #: cove/html_error_msg.py:225
 #, python-format
 msgid "%(extras)s does not match any of the regexes: %(patterns)s"
 msgid_plural "%(extras)s do not match any of the regexes: %(patterns)s"
 msgstr[0] ""
 "%(extras)s no coincide con ninguna de las expresiones regulares: "
```

### Comparing `libcoveweb-0.27.0/cove/management/commands/base_command.py` & `libcoveweb-0.28.0/cove/management/commands/base_command.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/management/commands/expire_files.py` & `libcoveweb-0.28.0/cove/management/commands/expire_files.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/management/commands/tests.py` & `libcoveweb-0.28.0/cove/management/commands/tests.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/management/commands/upload.py` & `libcoveweb-0.28.0/cove/management/commands/upload.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/_bootstrap-mincer.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/_bootstrap-mincer.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/_bootstrap.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/_bootstrap.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_alerts.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_alerts.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_badges.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_badges.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_breadcrumbs.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_breadcrumbs.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_button-groups.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_button-groups.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_buttons.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_buttons.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_carousel.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_carousel.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_close.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_close.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_code.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_code.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_component-animations.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_component-animations.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_dropdowns.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_dropdowns.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_forms.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_forms.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_glyphicons.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_glyphicons.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_grid.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_grid.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_input-groups.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_input-groups.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_jumbotron.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_jumbotron.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_labels.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_labels.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_list-group.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_list-group.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_media.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_media.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_mixins.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_mixins.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_modals.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_modals.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_navbar.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_navbar.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_navs.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_navs.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_normalize.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_normalize.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_pager.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_pager.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_pagination.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_pagination.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_panels.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_panels.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_popovers.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_popovers.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_print.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_print.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_progress-bars.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_progress-bars.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_responsive-embed.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_responsive-embed.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_responsive-utilities.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_responsive-utilities.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_scaffolding.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_scaffolding.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_tables.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_tables.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_theme.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_theme.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_thumbnails.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_thumbnails.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_tooltip.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_type.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_type.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_utilities.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_utilities.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_variables.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_variables.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/_wells.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/_wells.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_buttons.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_clearfix.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_clearfix.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_forms.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_gradients.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_grid-framework.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_grid-framework.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_grid.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_hide-text.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_hide-text.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_image.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_image.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_list-group.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_list-group.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_panels.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_panels.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_responsive-visibility.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_responsive-visibility.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_table-row.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_table-row.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/sass/bootstrap/bootstrap/mixins/_vendor-prefixes.scss` & `libcoveweb-0.28.0/cove/sass/bootstrap/bootstrap/mixins/_vendor-prefixes.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/settings.py` & `libcoveweb-0.28.0/cove/settings.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/static/dataexplore/css/style.css` & `libcoveweb-0.28.0/cove/static/dataexplore/css/style.css`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.eot` & `libcoveweb-0.28.0/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.svg` & `libcoveweb-0.28.0/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.ttf` & `libcoveweb-0.28.0/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff` & `libcoveweb-0.28.0/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff2` & `libcoveweb-0.28.0/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/static/dataexplore/fonts/tick/tick.eot` & `libcoveweb-0.28.0/cove/static/dataexplore/fonts/tick/tick.eot`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/static/dataexplore/fonts/tick/tick.svg` & `libcoveweb-0.28.0/cove/static/dataexplore/fonts/tick/tick.svg`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/static/dataexplore/fonts/tick/tick.ttf` & `libcoveweb-0.28.0/cove/static/dataexplore/fonts/tick/tick.ttf`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/static/dataexplore/fonts/tick/tick.woff` & `libcoveweb-0.28.0/cove/static/dataexplore/fonts/tick/tick.woff`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/static/dataexplore/fonts/tick/tick.woff2` & `libcoveweb-0.28.0/cove/static/dataexplore/fonts/tick/tick.woff2`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/500.html` & `libcoveweb-0.28.0/cove/templates/500.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/additional_codelist_values.html` & `libcoveweb-0.28.0/cove/templates/additional_codelist_values.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/additional_fields_table_all.html` & `libcoveweb-0.28.0/cove/templates/additional_fields_table_all.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/base.html` & `libcoveweb-0.28.0/cove/templates/base.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/error.html` & `libcoveweb-0.28.0/cove/templates/error.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/explore.html` & `libcoveweb-0.28.0/cove/templates/explore.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/input.html` & `libcoveweb-0.28.0/cove/templates/input.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/modal_errors.html` & `libcoveweb-0.28.0/cove/templates/modal_errors.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/modal_list.html` & `libcoveweb-0.28.0/cove/templates/modal_list.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/page_header.html` & `libcoveweb-0.28.0/cove/templates/page_header.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/piwik.html` & `libcoveweb-0.28.0/cove/templates/piwik.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/stats.html` & `libcoveweb-0.28.0/cove/templates/stats.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/terms.html` & `libcoveweb-0.28.0/cove/templates/terms.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/terms_conditions.html` & `libcoveweb-0.28.0/cove/templates/terms_conditions.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/terms_conditions_intro.html` & `libcoveweb-0.28.0/cove/templates/terms_conditions_intro.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/terms_cookies.html` & `libcoveweb-0.28.0/cove/templates/terms_cookies.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/terms_data_deleting.html` & `libcoveweb-0.28.0/cove/templates/terms_data_deleting.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/terms_data_uploaded.html` & `libcoveweb-0.28.0/cove/templates/terms_data_uploaded.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/terms_disclaimer.html` & `libcoveweb-0.28.0/cove/templates/terms_disclaimer.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/terms_links.html` & `libcoveweb-0.28.0/cove/templates/terms_links.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/terms_privacy.html` & `libcoveweb-0.28.0/cove/templates/terms_privacy.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/terms_privacy_intro.html` & `libcoveweb-0.28.0/cove/templates/terms_privacy_intro.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/terms_tracker_google_analytics.html` & `libcoveweb-0.28.0/cove/templates/terms_tracker_google_analytics.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/terms_tracker_matmo.html` & `libcoveweb-0.28.0/cove/templates/terms_tracker_matmo.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/terms_tracker_sentry.html` & `libcoveweb-0.28.0/cove/templates/terms_tracker_sentry.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/terms_tracker_server.html` & `libcoveweb-0.28.0/cove/templates/terms_tracker_server.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templates/validation_table.html` & `libcoveweb-0.28.0/cove/templates/validation_table.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/templatetags/cove_tags.py` & `libcoveweb-0.28.0/cove/templatetags/cove_tags.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/tests.py` & `libcoveweb-0.28.0/cove/tests.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/urls.py` & `libcoveweb-0.28.0/cove/urls.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/cove/views.py` & `libcoveweb-0.28.0/cove/views.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.27.0/libcoveweb.egg-info/SOURCES.txt` & `libcoveweb-0.28.0/libcoveweb.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 cove/input/migrations/0003_auto_20150506_1649.py
 cove/input/migrations/0004_auto_20150908_1533.py
 cove/input/migrations/0005_auto_20160104_1208.py
 cove/input/migrations/0006_supplieddata_rendered.py
 cove/input/migrations/0007_supplied_data_schema_version.py
 cove/input/migrations/0008_supplieddata_data_schema_version.py
 cove/input/migrations/0009_supplieddata_parameters.py
+cove/input/migrations/0010_alter_supplieddata_original_file.py
 cove/input/migrations/__init__.py
 cove/lib/__init__.py
 cove/lib/common.py
 cove/locale/en/LC_MESSAGES/django.mo
 cove/locale/en/LC_MESSAGES/django.po
 cove/locale/es/LC_MESSAGES/django.mo
 cove/locale/es/LC_MESSAGES/django.po
```

### Comparing `libcoveweb-0.27.0/setup.py` & `libcoveweb-0.28.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 install_requires = []
 
 setup(
     name='libcoveweb',
-    version='0.27.0',
+    version='0.28.0',
     author='Open Data Services',
     author_email='code@opendataservices.coop',
     packages=find_packages(),
     package_data={
         'cove': [
             'fixtures/*',
             'locale/*/*/*.po',
@@ -26,15 +26,15 @@
     url='https://github.com/OpenDataServices/lib-cove-web',
     description='',
     classifiers=[
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
     ],
     python_requires=">=3.7",
     install_requires=[
-        "Django>=2.2,<3.3",
+        "Django>=2.2,<4.3",
         "django-bootstrap3",
         "requests",
         "django-environ",
         "flattentool",
         "werkzeug",
         "libcove>=0.17.0",
     ],
```

