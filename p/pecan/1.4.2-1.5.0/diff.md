# Comparing `tmp/pecan-1.4.2.tar.gz` & `tmp/pecan-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pecan-1.4.2.tar", last modified: Sun Jul  3 00:19:12 2022, max compression
+gzip compressed data, was "pecan-1.5.0.tar", last modified: Fri Jul 14 15:07:04 2023, max compression
```

## Comparing `pecan-1.4.2.tar` & `pecan-1.5.0.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.402547 pecan-1.4.2/
--rw-r--r--   0 rpetrello   (502) staff       (20)      262 2022-07-03 00:16:08.000000 pecan-1.4.2/AUTHORS
--rw-r--r--   0 rpetrello   (502) staff       (20)     1505 2022-07-03 00:16:08.000000 pecan-1.4.2/LICENSE
--rw-r--r--   0 rpetrello   (502) staff       (20)      287 2022-07-03 00:16:08.000000 pecan-1.4.2/MANIFEST.in
--rw-r--r--   0 rpetrello   (502) staff       (20)     1252 2022-07-03 00:19:12.402631 pecan-1.4.2/PKG-INFO
--rw-r--r--   0 rpetrello   (502) staff       (20)     1239 2022-07-03 00:16:08.000000 pecan-1.4.2/README.rst
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.375400 pecan-1.4.2/bin/
--rw-r--r--   0 rpetrello   (502) staff       (20)      135 2022-07-03 00:16:08.000000 pecan-1.4.2/bin/pecan
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.378401 pecan-1.4.2/pecan/
--rw-r--r--   0 rpetrello   (502) staff       (20)     5028 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/__init__.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.379945 pecan-1.4.2/pecan/commands/
--rw-r--r--   0 rpetrello   (502) staff       (20)      175 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/commands/__init__.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     4720 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/commands/base.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     1656 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/commands/create.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     6827 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/commands/serve.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     5517 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/commands/shell.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.380097 pecan-1.4.2/pecan/compat/
--rw-r--r--   0 rpetrello   (502) staff       (20)      917 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/compat/__init__.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     7419 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/configuration.py
--rw-r--r--   0 rpetrello   (502) staff       (20)    32396 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/core.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     5875 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/decorators.py
--rw-r--r--   0 rpetrello   (502) staff       (20)      182 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/deploy.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.380229 pecan-1.4.2/pecan/ext/
--rw-r--r--   0 rpetrello   (502) staff       (20)      133 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/ext/__init__.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     2573 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/extensions.py
--rw-r--r--   0 rpetrello   (502) staff       (20)    12814 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/hooks.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     4738 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/jsonify.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     1670 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/log.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.380901 pecan-1.4.2/pecan/middleware/
--rw-r--r--   0 rpetrello   (502) staff       (20)       73 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/middleware/__init__.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     3025 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/middleware/debug.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     2531 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/middleware/errordocument.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     6948 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/middleware/recursive.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     5654 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/middleware/static.py
--rw-r--r--   0 rpetrello   (502) staff       (20)    15457 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/rest.py
--rw-r--r--   0 rpetrello   (502) staff       (20)    11633 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/routing.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.381036 pecan-1.4.2/pecan/scaffolds/
--rw-r--r--   0 rpetrello   (502) staff       (20)     4181 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/__init__.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.385657 pecan-1.4.2/pecan/scaffolds/base/
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.385966 pecan-1.4.2/pecan/scaffolds/base/+package+/
--rw-r--r--   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/base/+package+/__init__.py
--rw-r--r--   0 rpetrello   (502) staff       (20)      262 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/base/+package+/app.py_tmpl
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.386297 pecan-1.4.2/pecan/scaffolds/base/+package+/controllers/
--rw-r--r--   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/base/+package+/controllers/__init__.py
--rw-r--r--   0 rpetrello   (502) staff       (20)      629 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/base/+package+/controllers/root.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.386604 pecan-1.4.2/pecan/scaffolds/base/+package+/model/
--rw-r--r--   0 rpetrello   (502) staff       (20)      463 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/base/+package+/model/__init__.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.387309 pecan-1.4.2/pecan/scaffolds/base/+package+/templates/
--rw-r--r--   0 rpetrello   (502) staff       (20)      273 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/base/+package+/templates/error.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      865 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/base/+package+/templates/index.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      448 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/base/+package+/templates/layout.html
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.387974 pecan-1.4.2/pecan/scaffolds/base/+package+/tests/
--rw-r--r--   0 rpetrello   (502) staff       (20)      518 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/base/+package+/tests/__init__.py_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)      563 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/base/+package+/tests/config.py_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)      691 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/base/+package+/tests/test_functional.py_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)      113 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/base/+package+/tests/test_units.py
--rw-r--r--   0 rpetrello   (502) staff       (20)       27 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/base/MANIFEST.in
--rw-r--r--   0 rpetrello   (502) staff       (20)     1490 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/base/config.py_tmpl
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.372507 pecan-1.4.2/pecan/scaffolds/base/public/
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.388136 pecan-1.4.2/pecan/scaffolds/base/public/css/
--rw-r--r--   0 rpetrello   (502) staff       (20)      569 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/base/public/css/style.css
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.388278 pecan-1.4.2/pecan/scaffolds/base/public/images/
--rw-r--r--   0 rpetrello   (502) staff       (20)    20596 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/base/public/images/logo.png
--rw-r--r--   0 rpetrello   (502) staff       (20)       92 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/base/setup.cfg_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)      490 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/base/setup.py_tmpl
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.388954 pecan-1.4.2/pecan/scaffolds/rest-api/
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.389385 pecan-1.4.2/pecan/scaffolds/rest-api/+package+/
--rw-r--r--   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/rest-api/+package+/__init__.py
--rw-r--r--   0 rpetrello   (502) staff       (20)      339 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/rest-api/+package+/app.py_tmpl
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.389649 pecan-1.4.2/pecan/scaffolds/rest-api/+package+/controllers/
--rw-r--r--   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/rest-api/+package+/controllers/__init__.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     1085 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/rest-api/+package+/controllers/root.py
--rw-r--r--   0 rpetrello   (502) staff       (20)      496 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/rest-api/+package+/errors.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.389814 pecan-1.4.2/pecan/scaffolds/rest-api/+package+/model/
--rw-r--r--   0 rpetrello   (502) staff       (20)      463 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/rest-api/+package+/model/__init__.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.390702 pecan-1.4.2/pecan/scaffolds/rest-api/+package+/tests/
--rw-r--r--   0 rpetrello   (502) staff       (20)      518 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/rest-api/+package+/tests/__init__.py_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)      384 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/rest-api/+package+/tests/config.py_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)     1174 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/rest-api/+package+/tests/test_functional.py_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)      113 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/rest-api/+package+/tests/test_units.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     1311 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/rest-api/config.py_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)       92 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/rest-api/setup.cfg_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)      490 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/scaffolds/rest-api/setup.py_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)     7242 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/secure.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     8391 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/templating.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     1711 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/testing.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.395011 pecan-1.4.2/pecan/tests/
--rw-r--r--   0 rpetrello   (502) staff       (20)      197 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/__init__.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.395796 pecan-1.4.2/pecan/tests/config_fixtures/
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.396353 pecan-1.4.2/pecan/tests/config_fixtures/bad/
--rw-r--r--   0 rpetrello   (502) staff       (20)       36 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/config_fixtures/bad/importerror.py
--rw-r--r--   0 rpetrello   (502) staff       (20)       48 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/config_fixtures/bad/module_and_underscore.py
--rw-r--r--   0 rpetrello   (502) staff       (20)      439 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/config_fixtures/config.py
--rw-r--r--   0 rpetrello   (502) staff       (20)       21 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/config_fixtures/empty.py
--rw-r--r--   0 rpetrello   (502) staff       (20)       12 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/config_fixtures/foobar.py
--rw-r--r--   0 rpetrello   (502) staff       (20)      338 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/config_fixtures/forcedict.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.397142 pecan-1.4.2/pecan/tests/middleware/
--rw-r--r--   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/middleware/__init__.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.397572 pecan-1.4.2/pecan/tests/middleware/static_fixtures/
--rw-r--r--   0 rpetrello   (502) staff       (20)     6976 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/middleware/static_fixtures/self.png
--rw-r--r--   0 rpetrello   (502) staff       (20)      473 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/middleware/static_fixtures/text.txt
--rw-r--r--   0 rpetrello   (502) staff       (20)     3006 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/middleware/test_errordocument.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     5532 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/middleware/test_recursive.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     2390 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/middleware/test_static.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     4495 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/scaffold_builder.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.397772 pecan-1.4.2/pecan/tests/scaffold_fixtures/
--rw-r--r--   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/scaffold_fixtures/__init__.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.397869 pecan-1.4.2/pecan/tests/scaffold_fixtures/content_sub/
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.398097 pecan-1.4.2/pecan/tests/scaffold_fixtures/content_sub/bar/
--rw-r--r--   0 rpetrello   (502) staff       (20)       17 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/scaffold_fixtures/content_sub/bar/spam.txt_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)       15 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/scaffold_fixtures/content_sub/foo_tmpl
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.398315 pecan-1.4.2/pecan/tests/scaffold_fixtures/file_sub/
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.398533 pecan-1.4.2/pecan/tests/scaffold_fixtures/file_sub/bar_+package+/
--rw-r--r--   0 rpetrello   (502) staff       (20)        6 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/scaffold_fixtures/file_sub/bar_+package+/spam.txt
--rw-r--r--   0 rpetrello   (502) staff       (20)        4 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/scaffold_fixtures/file_sub/foo_+package+
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.398753 pecan-1.4.2/pecan/tests/scaffold_fixtures/simple/
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.398962 pecan-1.4.2/pecan/tests/scaffold_fixtures/simple/bar/
--rw-r--r--   0 rpetrello   (502) staff       (20)        6 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/scaffold_fixtures/simple/bar/spam.txt
--rw-r--r--   0 rpetrello   (502) staff       (20)        4 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/scaffold_fixtures/simple/foo
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.402315 pecan-1.4.2/pecan/tests/templates/
--rw-r--r--   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/templates/__init__.py
--rw-r--r--   0 rpetrello   (502) staff       (20)      207 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/templates/form_colors.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      139 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/templates/form_colors_invalid.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      128 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/templates/form_colors_valid.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      143 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/templates/form_login_invalid.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      116 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/templates/form_login_valid.html
--rw-r--r--   0 rpetrello   (502) staff       (20)       75 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/templates/form_name.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      147 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/templates/form_name_invalid.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      152 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/templates/form_name_invalid_custom.html
--rw-r--r--   0 rpetrello   (502) staff       (20)       57 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/templates/form_name_valid.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      472 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/templates/genshi.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      518 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/templates/genshi_bad.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      115 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/templates/jinja.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      163 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/templates/jinja_bad.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      109 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/templates/kajiki.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      108 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/templates/mako.html
--rw-r--r--   0 rpetrello   (502) staff       (20)       46 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/templates/mako_bad.html
--rw-r--r--   0 rpetrello   (502) staff       (20)    74202 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/test_base.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     1611 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/test_commands.py
--rw-r--r--   0 rpetrello   (502) staff       (20)    12826 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/test_conf.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     2900 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/test_generic.py
--rw-r--r--   0 rpetrello   (502) staff       (20)    51703 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/test_hooks.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     6529 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/test_jsonify.py
--rw-r--r--   0 rpetrello   (502) staff       (20)    50004 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/test_no_thread_locals.py
--rw-r--r--   0 rpetrello   (502) staff       (20)    45765 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/test_rest.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     5210 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/test_scaffolds.py
--rw-r--r--   0 rpetrello   (502) staff       (20)    17809 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/test_secure.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     1449 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/test_templating.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     4239 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/tests/test_util.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     1540 2022-07-03 00:16:08.000000 pecan-1.4.2/pecan/util.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2022-07-03 00:19:12.379246 pecan-1.4.2/pecan.egg-info/
--rw-r--r--   0 rpetrello   (502) staff       (20)     1252 2022-07-03 00:19:12.000000 pecan-1.4.2/pecan.egg-info/PKG-INFO
--rw-r--r--   0 rpetrello   (502) staff       (20)     4349 2022-07-03 00:19:12.000000 pecan-1.4.2/pecan.egg-info/SOURCES.txt
--rw-r--r--   0 rpetrello   (502) staff       (20)        1 2022-07-03 00:19:12.000000 pecan-1.4.2/pecan.egg-info/dependency_links.txt
--rw-r--r--   0 rpetrello   (502) staff       (20)      350 2022-07-03 00:19:12.000000 pecan-1.4.2/pecan.egg-info/entry_points.txt
--rw-r--r--   0 rpetrello   (502) staff       (20)        1 2022-07-03 00:19:12.000000 pecan-1.4.2/pecan.egg-info/not-zip-safe
--rw-r--r--   0 rpetrello   (502) staff       (20)       52 2022-07-03 00:19:12.000000 pecan-1.4.2/pecan.egg-info/requires.txt
--rw-r--r--   0 rpetrello   (502) staff       (20)        6 2022-07-03 00:19:12.000000 pecan-1.4.2/pecan.egg-info/top_level.txt
--rw-r--r--   0 rpetrello   (502) staff       (20)       52 2022-07-03 00:16:08.000000 pecan-1.4.2/requirements.txt
--rw-r--r--   0 rpetrello   (502) staff       (20)      209 2022-07-03 00:19:12.402931 pecan-1.4.2/setup.cfg
--rw-r--r--   0 rpetrello   (502) staff       (20)     3167 2022-07-03 00:16:08.000000 pecan-1.4.2/setup.py
--rw-r--r--   0 rpetrello   (502) staff       (20)       94 2022-07-03 00:16:08.000000 pecan-1.4.2/test-requirements.txt
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.495615 pecan-1.5.0/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      262 2023-07-14 15:06:47.000000 pecan-1.5.0/AUTHORS
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1505 2023-07-14 15:06:47.000000 pecan-1.5.0/LICENSE
+-rw-r--r--   0 rpetrello   (502) staff       (20)      287 2023-07-14 15:06:47.000000 pecan-1.5.0/MANIFEST.in
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1280 2023-07-14 15:07:04.495684 pecan-1.5.0/PKG-INFO
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1239 2023-07-14 15:06:47.000000 pecan-1.5.0/README.rst
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.479584 pecan-1.5.0/bin/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      135 2023-07-14 15:06:47.000000 pecan-1.5.0/bin/pecan
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.481579 pecan-1.5.0/pecan/
+-rw-r--r--   0 rpetrello   (502) staff       (20)     5028 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/__init__.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.483112 pecan-1.5.0/pecan/commands/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      175 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/commands/__init__.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     4695 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/commands/base.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1656 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/commands/create.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     6827 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/commands/serve.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     5525 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/commands/shell.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.483239 pecan-1.5.0/pecan/compat/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      692 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/compat/__init__.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     7196 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/configuration.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)    32093 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/core.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     5826 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/decorators.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)      182 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/deploy.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.483368 pecan-1.5.0/pecan/ext/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      133 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/ext/__init__.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     2573 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/extensions.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)    12809 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/hooks.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     4909 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/jsonify.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1670 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/log.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.484348 pecan-1.5.0/pecan/middleware/
+-rw-r--r--   0 rpetrello   (502) staff       (20)       73 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/middleware/__init__.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     2978 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/middleware/debug.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     2560 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/middleware/errordocument.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     6948 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/middleware/recursive.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     5588 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/middleware/static.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)    15361 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/rest.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)    11597 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/routing.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.484485 pecan-1.5.0/pecan/scaffolds/
+-rw-r--r--   0 rpetrello   (502) staff       (20)     3982 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/__init__.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.485010 pecan-1.5.0/pecan/scaffolds/base/
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.485396 pecan-1.5.0/pecan/scaffolds/base/+package+/
+-rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/__init__.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)      262 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/app.py_tmpl
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.485767 pecan-1.5.0/pecan/scaffolds/base/+package+/controllers/
+-rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/controllers/__init__.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)      629 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/controllers/root.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.485940 pecan-1.5.0/pecan/scaffolds/base/+package+/model/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      463 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/model/__init__.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.486374 pecan-1.5.0/pecan/scaffolds/base/+package+/templates/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      273 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/templates/error.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      865 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/templates/index.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      448 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/templates/layout.html
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.486918 pecan-1.5.0/pecan/scaffolds/base/+package+/tests/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      518 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/tests/__init__.py_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)      563 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/tests/config.py_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)      691 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/tests/test_functional.py_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)      113 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/tests/test_units.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)       27 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/MANIFEST.in
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1490 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/config.py_tmpl
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.465188 pecan-1.5.0/pecan/scaffolds/base/public/
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.487055 pecan-1.5.0/pecan/scaffolds/base/public/css/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      569 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/public/css/style.css
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.487185 pecan-1.5.0/pecan/scaffolds/base/public/images/
+-rw-r--r--   0 rpetrello   (502) staff       (20)    20596 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/public/images/logo.png
+-rw-r--r--   0 rpetrello   (502) staff       (20)       92 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/setup.cfg_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)      490 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/setup.py_tmpl
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.487605 pecan-1.5.0/pecan/scaffolds/rest-api/
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.487986 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/
+-rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/__init__.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)      339 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/app.py_tmpl
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.488228 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/controllers/
+-rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/controllers/__init__.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1085 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/controllers/root.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)      496 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/errors.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.488364 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/model/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      463 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/model/__init__.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.488900 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/tests/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      518 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/tests/__init__.py_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)      384 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/tests/config.py_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1174 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/tests/test_functional.py_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)      113 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/tests/test_units.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1311 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/config.py_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)       92 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/setup.cfg_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)      490 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/setup.py_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)     7084 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/secure.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     8391 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/templating.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1711 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/testing.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.490891 pecan-1.5.0/pecan/tests/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      197 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/__init__.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.491407 pecan-1.5.0/pecan/tests/config_fixtures/
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.491664 pecan-1.5.0/pecan/tests/config_fixtures/bad/
+-rw-r--r--   0 rpetrello   (502) staff       (20)       36 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/config_fixtures/bad/importerror.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)       48 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/config_fixtures/bad/module_and_underscore.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)      439 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/config_fixtures/config.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)       21 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/config_fixtures/empty.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)       12 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/config_fixtures/foobar.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)      338 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/config_fixtures/forcedict.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.492166 pecan-1.5.0/pecan/tests/middleware/
+-rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/middleware/__init__.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.492434 pecan-1.5.0/pecan/tests/middleware/static_fixtures/
+-rw-r--r--   0 rpetrello   (502) staff       (20)     6976 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/middleware/static_fixtures/self.png
+-rw-r--r--   0 rpetrello   (502) staff       (20)      473 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/middleware/static_fixtures/text.txt
+-rw-r--r--   0 rpetrello   (502) staff       (20)     3002 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/middleware/test_errordocument.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     5499 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/middleware/test_recursive.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     2390 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/middleware/test_static.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     4467 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/scaffold_builder.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.492561 pecan-1.5.0/pecan/tests/scaffold_fixtures/
+-rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/scaffold_fixtures/__init__.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.492669 pecan-1.5.0/pecan/tests/scaffold_fixtures/content_sub/
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.492801 pecan-1.5.0/pecan/tests/scaffold_fixtures/content_sub/bar/
+-rw-r--r--   0 rpetrello   (502) staff       (20)       17 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/scaffold_fixtures/content_sub/bar/spam.txt_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)       15 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/scaffold_fixtures/content_sub/foo_tmpl
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.492937 pecan-1.5.0/pecan/tests/scaffold_fixtures/file_sub/
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.493068 pecan-1.5.0/pecan/tests/scaffold_fixtures/file_sub/bar_+package+/
+-rw-r--r--   0 rpetrello   (502) staff       (20)        6 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/scaffold_fixtures/file_sub/bar_+package+/spam.txt
+-rw-r--r--   0 rpetrello   (502) staff       (20)        4 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/scaffold_fixtures/file_sub/foo_+package+
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.493194 pecan-1.5.0/pecan/tests/scaffold_fixtures/simple/
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.493323 pecan-1.5.0/pecan/tests/scaffold_fixtures/simple/bar/
+-rw-r--r--   0 rpetrello   (502) staff       (20)        6 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/scaffold_fixtures/simple/bar/spam.txt
+-rw-r--r--   0 rpetrello   (502) staff       (20)        4 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/scaffold_fixtures/simple/foo
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.495480 pecan-1.5.0/pecan/tests/templates/
+-rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/__init__.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)      207 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/form_colors.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      139 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/form_colors_invalid.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      128 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/form_colors_valid.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      143 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/form_login_invalid.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      116 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/form_login_valid.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)       75 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/form_name.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      147 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/form_name_invalid.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      152 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/form_name_invalid_custom.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)       57 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/form_name_valid.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      472 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/genshi.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      518 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/genshi_bad.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      115 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/jinja.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      163 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/jinja_bad.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      109 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/kajiki.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      108 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/mako.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)       46 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/mako_bad.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)    73374 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_base.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1611 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_commands.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)    12788 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_conf.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     2915 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_generic.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)    51501 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_hooks.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     6648 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_jsonify.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)    49620 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_no_thread_locals.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)    44973 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_rest.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     5189 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_scaffolds.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)    17728 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_secure.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1421 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_templating.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     4239 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_util.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1498 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/util.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.482478 pecan-1.5.0/pecan.egg-info/
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1280 2023-07-14 15:07:04.000000 pecan-1.5.0/pecan.egg-info/PKG-INFO
+-rw-r--r--   0 rpetrello   (502) staff       (20)     4349 2023-07-14 15:07:04.000000 pecan-1.5.0/pecan.egg-info/SOURCES.txt
+-rw-r--r--   0 rpetrello   (502) staff       (20)        1 2023-07-14 15:07:04.000000 pecan-1.5.0/pecan.egg-info/dependency_links.txt
+-rw-r--r--   0 rpetrello   (502) staff       (20)      393 2023-07-14 15:07:04.000000 pecan-1.5.0/pecan.egg-info/entry_points.txt
+-rw-r--r--   0 rpetrello   (502) staff       (20)        1 2023-07-14 15:07:04.000000 pecan-1.5.0/pecan.egg-info/not-zip-safe
+-rw-r--r--   0 rpetrello   (502) staff       (20)       48 2023-07-14 15:07:04.000000 pecan-1.5.0/pecan.egg-info/requires.txt
+-rw-r--r--   0 rpetrello   (502) staff       (20)        6 2023-07-14 15:07:04.000000 pecan-1.5.0/pecan.egg-info/top_level.txt
+-rw-r--r--   0 rpetrello   (502) staff       (20)       48 2023-07-14 15:06:47.000000 pecan-1.5.0/requirements.txt
+-rw-r--r--   0 rpetrello   (502) staff       (20)      209 2023-07-14 15:07:04.495947 pecan-1.5.0/setup.cfg
+-rw-r--r--   0 rpetrello   (502) staff       (20)     3167 2023-07-14 15:06:47.000000 pecan-1.5.0/setup.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)       94 2023-07-14 15:06:47.000000 pecan-1.5.0/test-requirements.txt
```

### Comparing `pecan-1.4.2/LICENSE` & `pecan-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/PKG-INFO` & `pecan-1.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pecan
-Version: 1.4.2
+Version: 1.5.0
 Summary: A WSGI object-dispatching web framework, designed to be lean and fast, with few dependencies.
 Home-page: http://github.com/pecan/pecan
 Author: Jonathan LaCour
 Author-email: info@pecanpy.org
 License: BSD
 Keywords: web framework wsgi object-dispatch http
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
@@ -23,7 +24,10 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 License-File: LICENSE
 License-File: AUTHORS
+
+UNKNOWN
+
```

### Comparing `pecan-1.4.2/README.rst` & `pecan-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/__init__.py` & `pecan-1.5.0/pecan/__init__.py`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/commands/base.py` & `pecan-1.5.0/pecan/commands/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import pkg_resources
 import argparse
 import logging
 import sys
 from warnings import warn
 
-import six
-
 log = logging.getLogger(__name__)
 
 
 class HelpfulArgumentParser(argparse.ArgumentParser):
 
     def error(self, message):  # pragma: nocover
         """error(message: string)
@@ -77,15 +75,15 @@
         for name, cmd in self.commands.items():
             sub = subparsers.add_parser(
                 name,
                 help=cmd.summary
             )
             for arg in getattr(cmd, 'arguments', tuple()):
                 arg = arg.copy()
-                if isinstance(arg.get('name'), six.string_types):
+                if isinstance(arg.get('name'), str):
                     sub.add_argument(arg.pop('name'), **arg)
                 elif isinstance(arg.get('name'), list):
                     sub.add_argument(*arg.pop('name'), **arg)
 
     def run(self, args):
         ns = self.parser.parse_args(args)
         self.commands[ns.command_name]().run(ns)
```

### Comparing `pecan-1.4.2/pecan/commands/create.py` & `pecan-1.5.0/pecan/commands/create.py`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/commands/serve.py` & `pecan-1.5.0/pecan/commands/serve.py`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/commands/shell.py` & `pecan-1.5.0/pecan/commands/shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         locs['response'] = response
 
         # prepare the banner
         banner = '  The following objects are available:\n'
         banner += '  %-10s - This project\'s WSGI App instance\n' % 'wsgiapp'
         banner += '  %-10s - The current configuration\n' % 'conf'
         if TestApp:
-            banner += '  %-10s - webtest.TestApp wrapped around wsgiapp\n' % 'app'
+            banner += '  %-10s - webtest.TestApp wrapped around wsgiapp\n' % 'app'  # noqa
         if model:
             model_name = getattr(
                 model,
                 '__module__',
                 getattr(model, '__name__', 'model')
             )
             banner += '  %-10s - Models from %s\n' % ('model', model_name)
```

### Comparing `pecan-1.4.2/pecan/compat/__init__.py` & `pecan-1.5.0/pecan/compat/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 import inspect
 
-import six
-
-if six.PY3:
-    import urllib.parse as urlparse
-    from urllib.parse import quote, unquote_plus
-    from urllib.request import urlopen, URLError
-    from html import escape
-    izip = zip
-else:
-    import urlparse  # noqa
-    from urllib import quote, unquote_plus  # noqa
-    from urllib2 import urlopen, URLError  # noqa
-    from cgi import escape  # noqa
-    from itertools import izip
+import urllib.parse as urlparse  # noqa
+from urllib.parse import quote, unquote_plus  # noqa
+from urllib.request import urlopen, URLError  # noqa
+from html import escape  # noqa
+izip = zip
 
 
 def is_bound_method(ob):
-    return inspect.ismethod(ob) and six.get_method_self(ob) is not None
+    return inspect.ismethod(ob) and ob.__self__ is not None
 
 
 def getargspec(func):
     import sys
     if sys.version_info < (3, 5):
         return inspect.getargspec(func)
```

### Comparing `pecan-1.4.2/pecan/configuration.py` & `pecan-1.5.0/pecan/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,12 @@
 import re
 import inspect
 import os
 import sys
-
-import six
-
-if six.PY3:
-    from importlib.machinery import SourceFileLoader
-else:
-    import imp
+from importlib.machinery import SourceFileLoader
 
 
 IDENTIFIER = re.compile(r'[a-z_](\w)*$', re.IGNORECASE)
 
 DEFAULT = {
     # Server Specific Configurations
     'server': {
@@ -59,15 +53,15 @@
         Updates this configuration with a dictionary.
 
         :param conf_dict: A python dictionary to update this configuration
                           with.
         '''
 
         if isinstance(conf_dict, dict):
-            iterator = six.iteritems(conf_dict)
+            iterator = iter(conf_dict.items())
         else:
             iterator = iter(conf_dict)
 
         for k, v in iterator:
             if not IDENTIFIER.match(k):
                 msg = ("'%s' is not a valid Python identifier,"
                        "consider using the '__force_dict__' key if requiring "
@@ -130,22 +124,22 @@
     def __setitem__(self, key, value):
         if isinstance(value, dict) and not isinstance(value, ConfigDict):
             if value.get('__force_dict__'):
                 del value['__force_dict__']
                 self.__values__[key] = ConfigDict(value)
             else:
                 self.__values__[key] = Config(value, filename=self.__file__)
-        elif isinstance(value, six.string_types) and '%(confdir)s' in value:
+        elif isinstance(value, str) and '%(confdir)s' in value:
             confdir = os.path.dirname(self.__file__) or os.getcwd()
             self.__values__[key] = value.replace('%(confdir)s', confdir)
         else:
             self.__values__[key] = value
 
     def __iter__(self):
-        return six.iteritems(self.__values__)
+        return iter(self.__values__.items())
 
     def __dir__(self):
         """
         When using dir() returns a list of the values in the config.  Note:
         This function only works in Python2.6 or later.
         """
         return list(self.__values__.keys())
@@ -170,21 +164,15 @@
     with open(abspath, 'rb') as f:
         compiled = compile(f.read(), abspath, 'exec')
 
     # Next, attempt to actually import the file as a module.
     # This provides more verbose import-related error reporting than exec()
     absname, _ = os.path.splitext(abspath)
     basepath, module_name = absname.rsplit(os.sep, 1)
-    if six.PY3:
-        SourceFileLoader(module_name, abspath).load_module(module_name)
-    else:
-        imp.load_module(
-            module_name,
-            *imp.find_module(module_name, [basepath])
-        )
+    SourceFileLoader(module_name, abspath).load_module(module_name)
 
     # If we were able to import as a module, actually exec the compiled code
     exec(compiled, globals(), conf_dict)
     conf_dict['__file__'] = abspath
 
     return conf_from_dict(conf_dict)
 
@@ -211,15 +199,15 @@
     '''
     Creates a configuration dictionary from a dictionary.
 
     :param conf_dict: The configuration dictionary.
     '''
     conf = Config(filename=conf_dict.get('__file__', ''))
 
-    for k, v in six.iteritems(conf_dict):
+    for k, v in iter(conf_dict.items()):
         if k.startswith('__'):
             continue
         elif inspect.ismodule(v):
             continue
 
         conf[k] = v
     return conf
@@ -244,15 +232,15 @@
     if config is None:
         config = get_conf_path_from_env()
 
     # must be after the fallback other a bad fallback will incorrectly clear
     if overwrite is True:
         _runtime_conf.empty()
 
-    if isinstance(config, six.string_types):
+    if isinstance(config, str):
         config = conf_from_file(config)
         _runtime_conf.update(config)
         if config.__file__:
             _runtime_conf.__file__ = config.__file__
     elif isinstance(config, dict):
         _runtime_conf.update(conf_from_dict(config))
     else:
```

### Comparing `pecan-1.4.2/pecan/core.py` & `pecan-1.5.0/pecan/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,32 +3,26 @@
 from mimetypes import guess_type, add_type
 from os.path import splitext
 import logging
 import operator
 import sys
 import types
 
-import six
-
 from webob import (Request as WebObRequest, Response as WebObResponse, exc,
                    acceptparse)
 from webob.multidict import NestedMultiDict
 
-from .compat import urlparse, izip
+from .compat import urlparse, izip, is_bound_method as ismethod
 from .jsonify import encode as dumps
 from .secure import handle_security
 from .templating import RendererFactory
 from .routing import lookup_controller, NonCanonicalPath
 from .util import _cfg, getargspec
 from .middleware.recursive import ForwardRequestException
 
-if six.PY3:
-    from .compat import is_bound_method as ismethod
-else:
-    from inspect import ismethod
 
 # make sure that json is defined in mimetypes
 add_type('application/json', '.json', True)
 
 state = None
 logger = logging.getLogger(__name__)
 
@@ -126,20 +120,15 @@
         _, _, traceback = sys.exc_info()
         webob_exception = exc.status_map[status_code](
             detail=detail,
             headers=headers,
             comment=comment,
             **kw
         )
-
-        if six.PY3:
-            raise webob_exception.with_traceback(traceback)
-        else:
-            # Using exec to avoid python 3 parsers from crashing
-            exec('raise webob_exception, None, traceback')
+        raise webob_exception.with_traceback(traceback)
     finally:
         # Per the suggestion of the Python docs, delete the traceback object
         del traceback
 
 
 def redirect(location=None, internal=False, code=None, headers={},
              add_slash=False, request=None):
@@ -232,25 +221,25 @@
 
     def __init__(self, root, default_renderer='mako',
                  template_path='templates', hooks=lambda: [],
                  custom_renderers={}, extra_template_vars={},
                  force_canonical=True, guess_content_type_from_ext=True,
                  context_local_factory=None, request_cls=Request,
                  response_cls=Response, **kw):
-        if isinstance(root, six.string_types):
+        if isinstance(root, str):
             root = self.__translate_root__(root)
 
         self.root = root
         self.request_cls = request_cls
         self.response_cls = response_cls
         self.renderers = RendererFactory(custom_renderers, extra_template_vars)
         self.default_renderer = default_renderer
 
         # pre-sort these so we don't have to do it per-request
-        if six.callable(hooks):
+        if callable(hooks):
             hooks = hooks()
 
         self.hooks = list(sorted(
             hooks,
             key=operator.attrgetter('priority')
         ))
         self.template_path = template_path
@@ -271,15 +260,15 @@
             parts = item.split('.')
             name = '.'.join(parts[:-1])
             fromlist = parts[-1:]
 
             module = __import__(name, fromlist=fromlist)
             kallable = getattr(module, parts[-1])
             msg = "%s does not represent a callable class or function."
-            if not six.callable(kallable):
+            if not callable(kallable):
                 raise TypeError(msg % item)
             return kallable()
 
         raise ImportError('No item named %s' % item)
 
     def route(self, req, node, path):
         '''
@@ -393,15 +382,15 @@
             elif name in defaults:
                 args.append(defaults[name])
             else:
                 break
 
         # handle wildcard GET/POST params
         if argspec[2]:
-            for name, value in six.iteritems(all_params):
+            for name, value in iter(all_params.items()):
                 if name not in argspec[0]:
                     kwargs[name] = value
 
         return args, varargs, kwargs
 
     def render(self, template, namespace):
         if template == 'json':
@@ -462,15 +451,15 @@
 
         if cfg.get('generic_handler'):
             raise exc.HTTPNotFound
 
         # handle generic controllers
         im_self = None
         if cfg.get('generic'):
-            im_self = six.get_method_self(controller)
+            im_self = controller.__self__
             handlers = cfg['generic_handlers']
             controller = handlers.get(req.method, handlers['DEFAULT'])
             handle_security(controller, im_self)
             cfg = _cfg(controller)
 
         # add the controller to the state so that hooks can use it
         state.controller = controller
@@ -618,15 +607,15 @@
         if req.environ.get('paste.testing'):
             testing_variables = req.environ['paste.testing_variables']
             testing_variables['namespace'] = raw_namespace
             testing_variables['template_name'] = template
             testing_variables['controller_output'] = result
 
         # set the body content
-        if result and isinstance(result, six.text_type):
+        if result and isinstance(result, str):
             resp.text = result
         elif result:
             resp.body = result
 
         if pecan_state['content_type']:
             # set the content type
             resp.content_type = pecan_state['content_type']
@@ -703,15 +692,15 @@
                 state.response = e
                 if best_match == 'application/json':
                     json_body = dumps({
                         'code': e.status_int,
                         'title': e.title,
                         'description': e.detail
                     })
-                    if isinstance(json_body, six.text_type):
+                    if isinstance(json_body, str):
                         e.text = json_body
                     else:
                         e.body = json_body
                     state.response.content_type = best_match
                 environ['pecan.original_exception'] = e
 
             # note if this is an internal redirect
```

### Comparing `pecan-1.4.2/pecan/decorators.py` & `pecan-1.5.0/pecan/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from inspect import getmembers, isclass, ismethod, isfunction
-
-import six
+from inspect import getmembers, isclass, isfunction
 
 from .util import _cfg, getargspec
 
 __all__ = [
     'expose', 'transactional', 'accept_noncanonical', 'after_commit',
     'after_rollback'
 ]
@@ -105,15 +103,15 @@
                              for this controller or not.
     '''
 
     def deco(f):
         if isclass(f):
             for meth in [
                 m[1] for m in getmembers(f)
-                if (isfunction if six.PY3 else ismethod)(m[1])
+                if isfunction(m[1])
             ]:
                 if getattr(meth, 'exposed', False):
                     _cfg(meth)['transactional'] = True
                     _cfg(meth)['transactional_ignore_redirects'] = _cfg(
                         meth
                     ).get(
                         'transactional_ignore_redirects',
```

### Comparing `pecan-1.4.2/pecan/extensions.py` & `pecan-1.5.0/pecan/extensions.py`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/hooks.py` & `pecan-1.5.0/pecan/hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
+import builtins
 import types
 import sys
 from inspect import getmembers
 
-import six
 from webob.exc import HTTPFound
 
 from .util import iscontroller, _cfg
 
 __all__ = [
     'PecanHook', 'TransactionHook', 'HookController',
     'RequestViewerHook'
 ]
 
 
 def walk_controller(root_class, controller, hooks, seen=None):
     seen = seen or set()
-    if type(controller) not in vars(six.moves.builtins).values():
+    if type(controller) not in vars(builtins).values():
         # Avoid recursion loops
         try:
             if controller in seen:
                 return
             seen.add(controller)
         except TypeError:
             # If we discover an unhashable item (like a list), it's not
```

### Comparing `pecan-1.4.2/pecan/jsonify.py` & `pecan-1.5.0/pecan/jsonify.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,34 +8,34 @@
     from webob.multidict import MultiDict, UnicodeMultiDict
     webob_dicts = (MultiDict, UnicodeMultiDict)  # pragma: no cover
 except ImportError:  # pragma no cover
     # WebOb >= 1.2
     from webob.multidict import MultiDict
     webob_dicts = (MultiDict,)
 
-import six
 try:
     from functools import singledispatch
 except ImportError:  # pragma: no cover
     from singledispatch import singledispatch
 
 try:
-    from sqlalchemy.engine.result import ResultProxy, RowProxy
-except ImportError:  # pragma no cover
+    import sqlalchemy  # noqa
     try:
-        from sqlalchemy.engine.base import ResultProxy, RowProxy
-    except ImportError:  # pragma no cover
-        # dummy classes since we don't have SQLAlchemy installed
-
-        class ResultProxy(object):  # noqa
-            pass
-
-        class RowProxy(object):  # noqa
-            pass
+        # SQLAlchemy 2.0 support
+        from sqlalchemy.engine import CursorResult as ResultProxy
+        from sqlalchemy.engine import Row as RowProxy
+    except ImportError:
+        from sqlalchemy.engine.result import ResultProxy, RowProxy
+except ImportError:
+    # dummy classes since we don't have SQLAlchemy installed
+    class ResultProxy(object):  # noqa
+        pass
 
+    class RowProxy(object):  # noqa
+        pass
 
 try:
     from sqlalchemy.engine.cursor import LegacyCursorResult, LegacyRow
 except ImportError:  # pragma no cover
     # dummy classes since we don't have SQLAlchemy installed
     # or we're using SQLAlchemy < 1.4
 
@@ -89,15 +89,15 @@
             Casts the RowProxy cursor object into a dictionary, probably
             losing its ordered dictionary behavior in the process but
             making it JSON-friendly.
         * webob_dicts objects
             returns webob_dicts.mixed() dictionary, which is guaranteed
             to be JSON-friendly.
         '''
-        if hasattr(obj, '__json__') and six.callable(obj.__json__):
+        if hasattr(obj, '__json__') and callable(obj.__json__):
             return obj.__json__()
         elif isinstance(obj, (date, datetime)):
             return str(obj)
         elif isinstance(obj, Decimal):
             # XXX What to do about JSONEncoder crappy handling of Decimals?
             # SimpleJSON has better Decimal encoding than the std lib
             # but only in recent versions
@@ -115,14 +115,17 @@
             return props
         elif isinstance(obj, LegacyCursorResult):
             rows = [dict(row._mapping) for row in obj.fetchall()]
             return {'count': len(rows), 'rows': rows}
         elif isinstance(obj, LegacyRow):
             return dict(obj._mapping)
         elif isinstance(obj, RowProxy):
+            if obj.__class__.__name__ == 'Row':
+                # SQLAlchemy 2.0 support
+                obj = obj._mapping
             return dict(obj)
         elif isinstance(obj, webob_dicts):
             return obj.mixed()
         else:
             return JSONEncoder.default(self, obj)
 
 _default = GenericJSON()
```

### Comparing `pecan-1.4.2/pecan/log.py` & `pecan-1.5.0/pecan/log.py`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/middleware/debug.py` & `pecan-1.5.0/pecan/middleware/debug.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-__CONFIG_HELP__ = '''
+__CONFIG_HELP__ = b'''
 <div class="traceback">
   <b>To disable this interface, set </b>
   <a target="window"
   href="https://pecan.readthedocs.io/en/latest/deployment.html#disabling-debug-mode">
     <pre>conf.app.debug = False</pre>
   </a>
 </div>
 '''  # noqa
 
 try:
     import re
-    from six import b
     from backlash.debug import DebuggedApplication
 
     class DebugMiddleware(DebuggedApplication):
 
-        body_re = re.compile(b('(<body[^>]*>)'), re.I)
+        body_re = re.compile(b'(<body[^>]*>)', re.I)
 
         def debug_application(self, environ, start_response):
             for part in super(DebugMiddleware, self).debug_application(
                 environ, start_response
             ):
-                yield self.body_re.sub(b('\g<1>%s' % __CONFIG_HELP__), part)
+                yield self.body_re.sub(b'<1>%s' % __CONFIG_HELP__, part)
 
 
 except ImportError:
     import logging
     from traceback import print_exc
     from pprint import pformat
 
     from mako.template import Template
-    from six.moves import cStringIO as StringIO
+    from io import StringIO
     from webob import Response
     from webob.exc import HTTPException
 
     LOG = logging.getLogger(__file__)
 
     debug_template_raw = '''<html>
      <head>
```

### Comparing `pecan-1.4.2/pecan/middleware/errordocument.py` & `pecan-1.5.0/pecan/middleware/errordocument.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import sys
 
-from six import b as b_
 from .recursive import ForwardRequestException, RecursionLoop
 
 
 class StatusPersist(object):
 
     def __init__(self, app, status, url):
         self.app = app
@@ -28,17 +27,19 @@
                 'Recursion error getting error page: %s\n' % e
             )
             keep_status_start_response(
                 '500 Server Error',
                 [('Content-type', 'text/plain')],
                 sys.exc_info()
             )
-            return [b_(
-                'Error: %s.  (Error page could not be fetched)' % self.status
-            )]
+            return [
+                b'Error: %s.  (Error page could not be fetched)' % (
+                    self.status.encode('utf-8')
+                )
+            ]
 
 
 class ErrorDocumentMiddleware(object):
     '''
     Intersects HTTP response status code, looks it up in the error map defined
     in the Pecan app config.py, and routes to the controller assigned to that
     status.
```

### Comparing `pecan-1.4.2/pecan/middleware/recursive.py` & `pecan-1.5.0/pecan/middleware/recursive.py`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/middleware/static.py` & `pecan-1.5.0/pecan/middleware/static.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 """
 
 import os
 import mimetypes
 from datetime import datetime
 from time import gmtime
 
-import six
-
 
 class FileWrapper(object):
     """This class can be used to convert a :class:`file`-like object into
     an iterable.  It yields `buffer_size` blocks until the file is fully
     read.
 
     You should not use this class directly but rather use the
@@ -33,25 +31,21 @@
     def close(self):
         if hasattr(self.file, 'close'):
             self.file.close()
 
     def __iter__(self):
         return self
 
-    def next(self):
+    def __next__(self):
         data = self.file.read(self.buffer_size)
         if data:
             return data
         raise StopIteration()
 
 
-if six.PY3:
-    FileWrapper.__next__ = FileWrapper.next
-
-
 def wrap_file(environ, file, buffer_size=8192):
     """Wraps a file.  This uses the WSGI server's file wrapper if available
     or otherwise the generic :class:`FileWrapper`.
 
     If the file wrapper from the WSGI server is used it's important to not
     iterate over it from inside the application but to pass it through
     unchanged.
```

### Comparing `pecan-1.4.2/pecan/rest.py` & `pecan-1.5.0/pecan/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from inspect import ismethod, getmembers
 import warnings
 
 from webob import exc
-import six
 
 from .core import abort
 from .decorators import expose
 from .routing import lookup_controller, handle_lookup_traversal
 from .util import iscontroller, getargspec
 
 
@@ -45,16 +44,15 @@
                         cls.__module__, cls.__name__, value.__name__
                     )
                 )
 
         # object.__new__ will error if called with extra arguments, and either
         # __new__ is overridden or __init__ is not overridden;
         # https://hg.python.org/cpython/file/78d36d54391c/Objects/typeobject.c#l3034
-        # In PY3, this is actually a TypeError (in PY2, it just raises
-        # a DeprecationWarning)
+        # In PY3, this is a TypeError
         new = super(RestController, cls).__new__
         if new is object.__new__:
             return new(cls)
         return new(cls, *args, **kwargs)
 
     def _get_args_for_controller(self, controller):
         """
@@ -178,15 +176,15 @@
         return result
 
     def _handle_lookup(self, args, request=None):
         if request is None:
             self._raise_method_deprecation_warning(self.handle_lookup)
 
         # filter empty strings from the arg list
-        args = list(six.moves.filter(bool, args))
+        args = list(filter(bool, args))
 
         # check for lookup controllers
         lookup = getattr(self, '_lookup', None)
         if args and iscontroller(lookup):
             result = handle_lookup_traversal(lookup, args)
             if result:
                 obj, remainder = result
@@ -272,15 +270,15 @@
         Routes ``GET`` actions to the appropriate controller.
         '''
         if request is None:
             self._raise_method_deprecation_warning(self._handle_get)
 
         # route to a get_all or get if no additional parts are available
         if not remainder or remainder == ['']:
-            remainder = list(six.moves.filter(bool, remainder))
+            remainder = list(filter(bool, remainder))
             controller = self._find_controller('get_all', 'get')
             if controller:
                 self._handle_bad_rest_arguments(controller, remainder, request)
                 return controller, []
             abort(405)
 
         method_name = remainder[-1]
```

### Comparing `pecan-1.4.2/pecan/routing.py` & `pecan-1.5.0/pecan/routing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 import re
 import warnings
 from inspect import getmembers, ismethod
 
 from webob import exc
-import six
 
 from .secure import handle_security, cross_boundary
 from .util import iscontroller, getargspec, _cfg
 
 __all__ = ['lookup_controller', 'find_object', 'route']
 __observed_controllers__ = set()
 __custom_routes__ = {}
@@ -38,15 +37,15 @@
         class Controller(object):
             pass
 
         pecan.route(Controller, 'with-dashes', SubController())
     """
 
     def _validate_route(route):
-        if not isinstance(route, six.string_types):
+        if not isinstance(route, str):
             raise TypeError('%s must be a string' % route)
 
         if route in ('.', '..') or not re.match(
             '^[0-9a-zA-Z-_$\(\)\.~!,;:*+@=]+$', route
         ):
             raise ValueError(
                 '%s must be a valid path segment.  Keep in mind '
@@ -276,15 +275,15 @@
 
     attrs = set(dir(obj))
 
     if obj.__class__ not in __observed_controllers__:
         for key, val in getmembers(obj):
             if iscontroller(val) and isinstance(
                 getattr(val, 'custom_route', None),
-                six.string_types
+                str,
             ):
                 route = val.custom_route
 
                 # Detect class attribute name conflicts
                 for conflict in attrs.intersection(set((route,))):
                     raise RuntimeError(
                         (
```

### Comparing `pecan-1.4.2/pecan/scaffolds/__init__.py` & `pecan-1.5.0/pecan/scaffolds/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import sys
 import os
 import re
 import pkg_resources
 from string import Template
 
-import six
-
 DEFAULT_SCAFFOLD = 'base'
 _bad_chars_re = re.compile('[^a-zA-Z0-9_]')
 
 
 class PecanScaffold(object):
     """
     A base Pecan scaffold.  New scaffolded implementations should extend this
@@ -121,22 +119,17 @@
     """
     Return a bytestring representing a templated file based on the
     input (content) and the variable names defined (vars).
     """
     fsenc = sys.getfilesystemencoding()
 
     def to_native(s, encoding='latin-1', errors='strict'):
-        if six.PY3:
-            if isinstance(s, six.text_type):
-                return s
-            return str(s, encoding, errors)
-        else:
-            if isinstance(s, six.text_type):
-                return s.encode(encoding, errors)
-            return str(s)
+        if isinstance(s, str):
+            return s
+        return str(s, encoding, errors)
 
     output = Template(
         to_native(content, fsenc)
     ).substitute(variables)
-    if isinstance(output, six.text_type):
+    if isinstance(output, str):
         output = output.encode(fsenc, 'strict')
     return output
```

### Comparing `pecan-1.4.2/pecan/scaffolds/base/+package+/controllers/root.py` & `pecan-1.5.0/pecan/scaffolds/base/+package+/controllers/root.py`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/scaffolds/base/+package+/templates/index.html` & `pecan-1.5.0/pecan/scaffolds/base/+package+/templates/index.html`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/scaffolds/base/+package+/tests/__init__.py_tmpl` & `pecan-1.5.0/pecan/scaffolds/base/+package+/tests/__init__.py_tmpl`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/scaffolds/base/+package+/tests/config.py_tmpl` & `pecan-1.5.0/pecan/scaffolds/base/+package+/tests/config.py_tmpl`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/scaffolds/base/+package+/tests/test_functional.py_tmpl` & `pecan-1.5.0/pecan/scaffolds/base/+package+/tests/test_functional.py_tmpl`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/scaffolds/base/config.py_tmpl` & `pecan-1.5.0/pecan/scaffolds/base/config.py_tmpl`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/scaffolds/base/public/css/style.css` & `pecan-1.5.0/pecan/scaffolds/base/public/css/style.css`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/scaffolds/base/public/images/logo.png` & `pecan-1.5.0/pecan/scaffolds/base/public/images/logo.png`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/scaffolds/rest-api/+package+/controllers/root.py` & `pecan-1.5.0/pecan/scaffolds/rest-api/+package+/controllers/root.py`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/scaffolds/rest-api/+package+/tests/__init__.py_tmpl` & `pecan-1.5.0/pecan/scaffolds/rest-api/+package+/tests/__init__.py_tmpl`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/scaffolds/rest-api/+package+/tests/test_functional.py_tmpl` & `pecan-1.5.0/pecan/scaffolds/rest-api/+package+/tests/test_functional.py_tmpl`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/scaffolds/rest-api/config.py_tmpl` & `pecan-1.5.0/pecan/scaffolds/rest-api/config.py_tmpl`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/secure.py` & `pecan-1.5.0/pecan/secure.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 from functools import wraps
 from inspect import getmembers, isfunction
 from webob import exc
 
-import six
-
+from .compat import is_bound_method as ismethod
 from .decorators import expose
 from .util import _cfg, iscontroller
 
 __all__ = ['unlocked', 'secure', 'SecureController']
 
-if six.PY3:
-    from .compat import is_bound_method as ismethod
-else:
-    from inspect import ismethod
-
 
 class _SecureState(object):
     def __init__(self, desc, boolean_value):
         self.description = desc
         self.boolean_value = boolean_value
 
     def __repr__(self):
@@ -62,25 +56,25 @@
 class _SecuredAttribute(object):
     def __init__(self, obj, check_permissions):
         self.obj = obj
         self.check_permissions = check_permissions
         self._parent = None
 
     def _check_permissions(self):
-        if isinstance(self.check_permissions, six.string_types):
+        if isinstance(self.check_permissions, str):
             return getattr(self.parent, self.check_permissions)()
         else:
             return self.check_permissions()
 
     def __get_parent(self):
         return self._parent
 
     def __set_parent(self, parent):
         if ismethod(parent):
-            self._parent = six.get_method_self(parent)
+            self._parent = parent.__self__
         else:
             self._parent = parent
     parent = property(__get_parent, __set_parent)
 
     @_secure_method('_check_permissions')
     @expose()
     def _lookup(self, *remainder):
@@ -88,15 +82,15 @@
 
 
 # helper for secure decorator
 def _allowed_check_permissions_types(x):
     return (
         ismethod(x) or
         isfunction(x) or
-        isinstance(x, six.string_types)
+        isinstance(x, str)
     )
 
 
 # methods that can either decorate functions or wrap classes
 # these should be the main methods used for securing or unlocking
 def unlocked(func_or_obj):
     """
@@ -141,15 +135,15 @@
         cls._pecan = dict(
             secured=Protected,
             check_permissions=cls.check_permissions,
             unlocked=[]
         )
 
         for name, value in getmembers(cls)[:]:
-            if (isfunction if six.PY3 else ismethod)(value):
+            if isfunction(value):
                 if iscontroller(value) and value._pecan.get(
                     'secured'
                 ) is None:
                     # Wrap the function so that the security context is
                     # local to this class definition.  This works around
                     # the fact that unbound method attributes are shared
                     # across classes with the same bases.
@@ -203,17 +197,17 @@
 
 # methods to evaluate security during routing
 def handle_security(controller, im_self=None):
     """ Checks the security of a controller.  """
     if controller._pecan.get('secured', False):
         check_permissions = controller._pecan['check_permissions']
 
-        if isinstance(check_permissions, six.string_types):
+        if isinstance(check_permissions, str):
             check_permissions = getattr(
-                im_self or six.get_method_self(controller),
+                im_self or controller.__self__,
                 check_permissions
             )
 
         if not check_permissions():
             raise exc.HTTPUnauthorized
```

### Comparing `pecan-1.4.2/pecan/templating.py` & `pecan-1.5.0/pecan/templating.py`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/testing.py` & `pecan-1.5.0/pecan/testing.py`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/tests/middleware/static_fixtures/self.png` & `pecan-1.5.0/pecan/tests/middleware/static_fixtures/self.png`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/tests/middleware/test_errordocument.py` & `pecan-1.5.0/pecan/tests/middleware/test_errordocument.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import json
 
 from webtest import TestApp
-from six import b as b_
 
 import pecan
 from pecan.middleware.errordocument import ErrorDocumentMiddleware
 from pecan.middleware.recursive import RecursiveMiddleware
 from pecan.tests import PecanTestCase
 
 
 def four_oh_four_app(environ, start_response):
     if environ['PATH_INFO'].startswith('/error'):
-        code = environ['PATH_INFO'].split('/')[2]
+        code = environ['PATH_INFO'].split('/')[2].encode('utf-8')
         start_response("200 OK", [('Content-type', 'text/plain')])
 
-        body = "Error: %s" % code
+        body = b"Error: %s" % code
         if environ['QUERY_STRING']:
-            body += "\nQS: %s" % environ['QUERY_STRING']
-        return [b_(body)]
+            body += b"\nQS: %s" % environ['QUERY_STRING'].encode('utf-8')
+        return [body]
     start_response("404 Not Found", [('Content-type', 'text/plain')])
     return []
 
 
 class TestErrorDocumentMiddleware(PecanTestCase):
 
     def setUp(self):
@@ -29,37 +28,37 @@
         self.app = TestApp(RecursiveMiddleware(ErrorDocumentMiddleware(
             four_oh_four_app, {404: '/error/404'}
         )))
 
     def test_hit_error_page(self):
         r = self.app.get('/error/404')
         assert r.status_int == 200
-        assert r.body == b_('Error: 404')
+        assert r.body == b'Error: 404'
 
     def test_middleware_routes_to_404_message(self):
         r = self.app.get('/', expect_errors=True)
         assert r.status_int == 404
-        assert r.body == b_('Error: 404')
+        assert r.body == b'Error: 404'
 
     def test_error_endpoint_with_query_string(self):
         app = TestApp(RecursiveMiddleware(ErrorDocumentMiddleware(
             four_oh_four_app, {404: '/error/404?foo=bar'}
         )))
         r = app.get('/', expect_errors=True)
         assert r.status_int == 404
-        assert r.body == b_('Error: 404\nQS: foo=bar')
+        assert r.body == b'Error: 404\nQS: foo=bar'
 
     def test_error_with_recursion_loop(self):
         app = TestApp(RecursiveMiddleware(ErrorDocumentMiddleware(
             four_oh_four_app, {404: '/'}
         )))
         r = app.get('/', expect_errors=True)
         assert r.status_int == 404
-        assert r.body == b_(
-            'Error: 404 Not Found.  (Error page could not be fetched)'
+        assert r.body == (
+            b'Error: 404 Not Found.  (Error page could not be fetched)'
         )
 
     def test_original_exception(self):
 
         class RootController(object):
 
             @pecan.expose()
```

### Comparing `pecan-1.4.2/pecan/tests/middleware/test_recursive.py` & `pecan-1.5.0/pecan/tests/middleware/test_recursive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from webtest import TestApp
-from six import b as b_
 
 from pecan.middleware.recursive import (RecursiveMiddleware,
                                         ForwardRequestException)
 from pecan.tests import PecanTestCase
 
 
 def simple_app(environ, start_response):
     start_response("200 OK", [('Content-type', 'text/plain')])
-    return [b_('requested page returned')]
+    return [b'requested page returned']
 
 
 def error_docs_app(environ, start_response):
     if environ['PATH_INFO'] == '/not_found':
         start_response("404 Not found", [('Content-type', 'text/plain')])
-        return [b_('Not found')]
+        return [b'Not found']
     elif environ['PATH_INFO'] == '/error':
         start_response("200 OK", [('Content-type', 'text/plain')])
-        return [b_('Page not found')]
+        return [b'Page not found']
     elif environ['PATH_INFO'] == '/recurse':
         raise ForwardRequestException('/recurse')
     else:
         return simple_app(environ, start_response)
 
 
 class Middleware(object):
```

### Comparing `pecan-1.4.2/pecan/tests/middleware/test_static.py` & `pecan-1.5.0/pecan/tests/middleware/test_static.py`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/tests/scaffold_builder.py` & `pecan-1.5.0/pecan/tests/scaffold_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import os
 import sys
 import subprocess
 import time
 
-from six import b as b_
-
 from pecan.compat import urlopen, URLError
 from pecan.tests import PecanTestCase
 
 import unittest
 
 
 if __name__ == '__main__':
@@ -75,15 +73,15 @@
                 stderr=subprocess.PIPE,
                 stdin=subprocess.PIPE
             )
 
             self.poll(proc)
 
             out, _ = proc.communicate(
-                b_('{"model" : model, "conf" : conf, "app" : app}')
+                b'{"model" : model, "conf" : conf, "app" : app}'
             )
             assert 'testing123.model' in out.decode(), out
             assert 'Config(' in out.decode(), out
             assert 'webtest.app.TestApp' in out.decode(), out
 
             try:
                 # just in case stdin doesn't close
```

### Comparing `pecan-1.4.2/pecan/tests/templates/genshi_bad.html` & `pecan-1.5.0/pecan/tests/templates/genshi_bad.html`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/tests/test_base.py` & `pecan-1.5.0/pecan/tests/test_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 # -*- coding: utf-8 -*-
 
 import sys
 import os
 import json
 import traceback
 import warnings
-from unittest import mock
+from io import StringIO, BytesIO
 
 import webob
 from webob.exc import HTTPNotFound
 from webtest import TestApp
-import six
-from six import b as b_
-from six import u as u_
-from six.moves import cStringIO as StringIO
 
 from pecan import (
     Pecan, Request, Response, expose, request, response, redirect,
     abort, make_app, override_template, render, route
 )
 from pecan.templating import (
     _builtin_renderers as builtin_renderers, error_formatters, MakoRenderer
@@ -45,27 +41,27 @@
         class RootController(object):
             @expose()
             def index(self):
                 pass
 
             @expose()
             def explicit_body(self):
-                response.body = b_('Hello, World!')
+                response.body = b'Hello, World!'
 
             @expose()
             def empty_body(self):
-                response.body = b_('')
+                response.body = b''
 
             @expose()
             def explicit_text(self):
-                response.text = six.text_type('Hello, World!')
+                response.text = 'Hello, World!'
 
             @expose()
             def empty_text(self):
-                response.text = six.text_type('')
+                response.text = ''
 
             @expose()
             def explicit_json(self):
                 response.json = {'foo': 'bar'}
 
             @expose()
             def explicit_json_body(self):
@@ -87,30 +83,30 @@
     def test_index_with_non_unicode(self):
         r = self.app_.get('/non_unicode/')
         self.assertEqual(r.status_int, 200)
 
     def test_explicit_body(self):
         r = self.app_.get('/explicit_body/')
         self.assertEqual(r.status_int, 200)
-        self.assertEqual(r.body, b_('Hello, World!'))
+        self.assertEqual(r.body, b'Hello, World!')
 
     def test_empty_body(self):
         r = self.app_.get('/empty_body/')
         self.assertEqual(r.status_int, 204)
-        self.assertEqual(r.body, b_(''))
+        self.assertEqual(r.body, b'')
 
     def test_explicit_text(self):
         r = self.app_.get('/explicit_text/')
         self.assertEqual(r.status_int, 200)
-        self.assertEqual(r.body, b_('Hello, World!'))
+        self.assertEqual(r.body, b'Hello, World!')
 
     def test_empty_text(self):
         r = self.app_.get('/empty_text/')
         self.assertEqual(r.status_int, 204)
-        self.assertEqual(r.body, b_(''))
+        self.assertEqual(r.body, b'')
 
     def test_explicit_json(self):
         r = self.app_.get('/explicit_json/')
         self.assertEqual(r.status_int, 200)
         json_resp = json.loads(r.body.decode())
         assert json_resp == {'foo': 'bar'}
 
@@ -123,28 +119,28 @@
 
 class TestAppIterFile(PecanTestCase):
     @property
     def app_(self):
         class RootController(object):
             @expose()
             def index(self):
-                body = six.BytesIO(b_('Hello, World!'))
+                body = BytesIO(b'Hello, World!')
                 response.body_file = body
 
             @expose()
             def empty(self):
-                body = six.BytesIO(b_(''))
+                body = BytesIO(b'')
                 response.body_file = body
 
         return TestApp(Pecan(RootController()))
 
     def test_body_generator(self):
         r = self.app_.get('/')
         self.assertEqual(r.status_int, 200)
-        assert r.body == b_('Hello, World!')
+        assert r.body == b'Hello, World!'
 
     def test_empty_body_generator(self):
         r = self.app_.get('/empty')
         self.assertEqual(r.status_int, 204)
         assert len(r.body) == 0
 
 
@@ -175,25 +171,25 @@
                 return 'Hello, World!'
 
         return TestApp(Pecan(RootController()))
 
     def test_empty_root(self):
         r = self.app_.get('/')
         assert r.status_int == 200
-        assert r.body == b_('Hello, World!')
+        assert r.body == b'Hello, World!'
 
     def test_index(self):
         r = self.app_.get('/index')
         assert r.status_int == 200
-        assert r.body == b_('Hello, World!')
+        assert r.body == b'Hello, World!'
 
     def test_index_html(self):
         r = self.app_.get('/index.html')
         assert r.status_int == 200
-        assert r.body == b_('Hello, World!')
+        assert r.body == b'Hello, World!'
 
 
 class TestObjectDispatch(PecanTestCase):
 
     @property
     def app_(self):
         class SubSubController(object):
@@ -228,68 +224,67 @@
             sub = SubController()
 
         return TestApp(Pecan(RootController()))
 
     def test_index(self):
         r = self.app_.get('/')
         assert r.status_int == 200
-        assert r.body == b_('/')
+        assert r.body == b'/'
 
     def test_one_level(self):
         r = self.app_.get('/deeper')
         assert r.status_int == 200
-        assert r.body == b_('/deeper')
+        assert r.body == b'/deeper'
 
     def test_one_level_with_trailing(self):
         r = self.app_.get('/sub/')
         assert r.status_int == 200
-        assert r.body == b_('/sub/')
+        assert r.body == b'/sub/'
 
     def test_two_levels(self):
         r = self.app_.get('/sub/deeper')
         assert r.status_int == 200
-        assert r.body == b_('/sub/deeper')
+        assert r.body == b'/sub/deeper'
 
     def test_two_levels_with_trailing(self):
         r = self.app_.get('/sub/sub/')
         assert r.status_int == 200
 
     def test_three_levels(self):
         r = self.app_.get('/sub/sub/deeper')
         assert r.status_int == 200
-        assert r.body == b_('/sub/sub/deeper')
+        assert r.body == b'/sub/sub/deeper'
 
 
-@unittest.skipIf(not six.PY3, "tests are Python3 specific")
 class TestUnicodePathSegments(PecanTestCase):
 
     def test_unicode_methods(self):
         class RootController(object):
             pass
         setattr(RootController, '🌰', expose()(lambda self: 'Hello, World!'))
         app = TestApp(Pecan(RootController()))
 
         resp = app.get('/%F0%9F%8C%B0/')
         assert resp.status_int == 200
-        assert resp.body == b_('Hello, World!')
+        assert resp.body == b'Hello, World!'
 
     def test_unicode_child(self):
         class ChildController(object):
             @expose()
             def index(self):
                 return 'Hello, World!'
 
         class RootController(object):
             pass
         setattr(RootController, '🌰', ChildController())
         app = TestApp(Pecan(RootController()))
 
         resp = app.get('/%F0%9F%8C%B0/')
         assert resp.status_int == 200
-        assert resp.body == b_('Hello, World!')
+        assert resp.body == b'Hello, World!'
 
 
 class TestLookups(PecanTestCase):
 
     @property
     def app_(self):
         class LookupController(object):
@@ -314,25 +309,25 @@
                 return LookupController(someID), remainder
 
         return TestApp(Pecan(RootController()))
 
     def test_index(self):
         r = self.app_.get('/')
         assert r.status_int == 200
-        assert r.body == b_('/')
+        assert r.body == b'/'
 
     def test_lookup(self):
         r = self.app_.get('/100/')
         assert r.status_int == 200
-        assert r.body == b_('/100')
+        assert r.body == b'/100'
 
     def test_lookup_with_method(self):
         r = self.app_.get('/100/name')
         assert r.status_int == 200
-        assert r.body == b_('/100/name')
+        assert r.body == b'/100/name'
 
     def test_lookup_with_wrong_argspec(self):
         class RootController(object):
             @expose()
             def _lookup(self, someID):
                 return 'Bad arg spec'  # pragma: nocover
 
@@ -374,15 +369,15 @@
 
         return TestApp(Pecan(RootController()))
 
     def test_canonical_lookup(self):
         assert self.app_.get('/users', expect_errors=404).status_int == 404
         assert self.app_.get('/users/', expect_errors=404).status_int == 404
         assert self.app_.get('/users/100').status_int == 302
-        assert self.app_.get('/users/100/').body == b_('100')
+        assert self.app_.get('/users/100/').body == b'100'
 
 
 class TestControllerArguments(PecanTestCase):
 
     @property
     def app_(self):
         class RootController(object):
@@ -462,538 +457,534 @@
                     "index() missing 1 required positional argument: 'id'"
                 ),
             )  # this messaging changed in Python 3.3 and again in Python 3.10
 
     def test_single_argument(self):
         r = self.app_.get('/1')
         assert r.status_int == 200
-        assert r.body == b_('index: 1')
+        assert r.body == b'index: 1'
 
     def test_single_argument_with_encoded_url(self):
         r = self.app_.get('/This%20is%20a%20test%21')
         assert r.status_int == 200
-        assert r.body == b_('index: This is a test!')
+        assert r.body == b'index: This is a test!'
 
     def test_single_argument_with_plus(self):
         r = self.app_.get('/foo+bar')
         assert r.status_int == 200
-        assert r.body == b_('index: foo+bar')
+        assert r.body == b'index: foo+bar'
 
     def test_single_argument_with_encoded_plus(self):
         r = self.app_.get('/foo%2Bbar')
         assert r.status_int == 200
-        assert r.body == b_('index: foo+bar')
+        assert r.body == b'index: foo+bar'
 
     def test_two_arguments(self):
         r = self.app_.get('/1/dummy', status=404)
         assert r.status_int == 404
 
     def test_keyword_argument(self):
         r = self.app_.get('/?id=2')
         assert r.status_int == 200
-        assert r.body == b_('index: 2')
+        assert r.body == b'index: 2'
 
     def test_keyword_argument_with_encoded_url(self):
         r = self.app_.get('/?id=This%20is%20a%20test%21')
         assert r.status_int == 200
-        assert r.body == b_('index: This is a test!')
+        assert r.body == b'index: This is a test!'
 
     def test_keyword_argument_with_plus(self):
         r = self.app_.get('/?id=foo+bar')
         assert r.status_int == 200
-        assert r.body == b_('index: foo bar')
+        assert r.body == b'index: foo bar'
 
     def test_keyword_argument_with_encoded_plus(self):
         r = self.app_.get('/?id=foo%2Bbar')
         assert r.status_int == 200
-        assert r.body == b_('index: foo+bar')
+        assert r.body == b'index: foo+bar'
 
     def test_argument_and_keyword_argument(self):
         r = self.app_.get('/3?id=three')
         assert r.status_int == 200
-        assert r.body == b_('index: 3')
+        assert r.body == b'index: 3'
 
     def test_encoded_argument_and_keyword_argument(self):
         r = self.app_.get('/This%20is%20a%20test%21?id=three')
         assert r.status_int == 200
-        assert r.body == b_('index: This is a test!')
+        assert r.body == b'index: This is a test!'
 
     def test_explicit_kwargs(self):
         r = self.app_.post('/', {'id': '4'})
         assert r.status_int == 200
-        assert r.body == b_('index: 4')
+        assert r.body == b'index: 4'
 
     def test_path_with_explicit_kwargs(self):
         r = self.app_.post('/4', {'id': 'four'})
         assert r.status_int == 200
-        assert r.body == b_('index: 4')
+        assert r.body == b'index: 4'
 
     def test_explicit_json_kwargs(self):
         r = self.app_.post_json('/', {'id': '4'})
         assert r.status_int == 200
-        assert r.body == b_('index: 4')
+        assert r.body == b'index: 4'
 
     def test_path_with_explicit_json_kwargs(self):
         r = self.app_.post_json('/4', {'id': 'four'})
         assert r.status_int == 200
-        assert r.body == b_('index: 4')
+        assert r.body == b'index: 4'
 
     def test_multiple_kwargs(self):
         r = self.app_.get('/?id=5&dummy=dummy')
         assert r.status_int == 200
-        assert r.body == b_('index: 5')
+        assert r.body == b'index: 5'
 
     def test_kwargs_from_root(self):
         r = self.app_.post('/', {'id': '6', 'dummy': 'dummy'})
         assert r.status_int == 200
-        assert r.body == b_('index: 6')
+        assert r.body == b'index: 6'
 
     def test_json_kwargs_from_root(self):
         r = self.app_.post_json('/', {'id': '6', 'dummy': 'dummy'})
         assert r.status_int == 200
-        assert r.body == b_('index: 6')
+        assert r.body == b'index: 6'
 
         # multiple args
 
     def test_multiple_positional_arguments(self):
         r = self.app_.get('/multiple/one/two')
         assert r.status_int == 200
-        assert r.body == b_('multiple: one, two')
+        assert r.body == b'multiple: one, two'
 
     def test_multiple_positional_arguments_with_url_encode(self):
         r = self.app_.get('/multiple/One%20/Two%21')
         assert r.status_int == 200
-        assert r.body == b_('multiple: One , Two!')
+        assert r.body == b'multiple: One , Two!'
 
     def test_multiple_positional_arguments_with_kwargs(self):
         r = self.app_.get('/multiple?one=three&two=four')
         assert r.status_int == 200
-        assert r.body == b_('multiple: three, four')
+        assert r.body == b'multiple: three, four'
 
     def test_multiple_positional_arguments_with_url_encoded_kwargs(self):
         r = self.app_.get('/multiple?one=Three%20&two=Four%20%21')
         assert r.status_int == 200
-        assert r.body == b_('multiple: Three , Four !')
+        assert r.body == b'multiple: Three , Four !'
 
     def test_positional_args_with_dictionary_kwargs(self):
         r = self.app_.post('/multiple', {'one': 'five', 'two': 'six'})
         assert r.status_int == 200
-        assert r.body == b_('multiple: five, six')
+        assert r.body == b'multiple: five, six'
 
     def test_positional_args_with_json_kwargs(self):
         r = self.app_.post_json('/multiple', {'one': 'five', 'two': 'six'})
         assert r.status_int == 200
-        assert r.body == b_('multiple: five, six')
+        assert r.body == b'multiple: five, six'
 
     def test_positional_args_with_url_encoded_dictionary_kwargs(self):
         r = self.app_.post('/multiple', {'one': 'Five%20', 'two': 'Six%20%21'})
         assert r.status_int == 200
-        assert r.body == b_('multiple: Five%20, Six%20%21')
+        assert r.body == b'multiple: Five%20, Six%20%21'
 
         # optional arg
     def test_optional_arg(self):
         r = self.app_.get('/optional')
         assert r.status_int == 200
-        assert r.body == b_('optional: None')
+        assert r.body == b'optional: None'
 
     def test_multiple_optional(self):
         r = self.app_.get('/optional/1')
         assert r.status_int == 200
-        assert r.body == b_('optional: 1')
+        assert r.body == b'optional: 1'
 
     def test_multiple_optional_url_encoded(self):
         r = self.app_.get('/optional/Some%20Number')
         assert r.status_int == 200
-        assert r.body == b_('optional: Some Number')
+        assert r.body == b'optional: Some Number'
 
     def test_multiple_optional_missing(self):
         r = self.app_.get('/optional/2/dummy', status=404)
         assert r.status_int == 404
 
     def test_multiple_with_kwargs(self):
         r = self.app_.get('/optional?id=2')
         assert r.status_int == 200
-        assert r.body == b_('optional: 2')
+        assert r.body == b'optional: 2'
 
     def test_multiple_with_url_encoded_kwargs(self):
         r = self.app_.get('/optional?id=Some%20Number')
         assert r.status_int == 200
-        assert r.body == b_('optional: Some Number')
+        assert r.body == b'optional: Some Number'
 
     def test_multiple_args_with_url_encoded_kwargs(self):
         r = self.app_.get('/optional/3?id=three')
         assert r.status_int == 200
-        assert r.body == b_('optional: 3')
+        assert r.body == b'optional: 3'
 
     def test_url_encoded_positional_args(self):
         r = self.app_.get('/optional/Some%20Number?id=three')
         assert r.status_int == 200
-        assert r.body == b_('optional: Some Number')
+        assert r.body == b'optional: Some Number'
 
     def test_optional_arg_with_kwargs(self):
         r = self.app_.post('/optional', {'id': '4'})
         assert r.status_int == 200
-        assert r.body == b_('optional: 4')
+        assert r.body == b'optional: 4'
 
     def test_optional_arg_with_json_kwargs(self):
         r = self.app_.post_json('/optional', {'id': '4'})
         assert r.status_int == 200
-        assert r.body == b_('optional: 4')
+        assert r.body == b'optional: 4'
 
     def test_optional_arg_with_url_encoded_kwargs(self):
         r = self.app_.post('/optional', {'id': 'Some%20Number'})
         assert r.status_int == 200
-        assert r.body == b_('optional: Some%20Number')
+        assert r.body == b'optional: Some%20Number'
 
     def test_multiple_positional_arguments_with_dictionary_kwargs(self):
         r = self.app_.post('/optional/5', {'id': 'five'})
         assert r.status_int == 200
-        assert r.body == b_('optional: 5')
+        assert r.body == b'optional: 5'
 
     def test_multiple_positional_arguments_with_json_kwargs(self):
         r = self.app_.post_json('/optional/5', {'id': 'five'})
         assert r.status_int == 200
-        assert r.body == b_('optional: 5')
+        assert r.body == b'optional: 5'
 
     def test_multiple_positional_url_encoded_arguments_with_kwargs(self):
         r = self.app_.post('/optional/Some%20Number', {'id': 'five'})
         assert r.status_int == 200
-        assert r.body == b_('optional: Some Number')
+        assert r.body == b'optional: Some Number'
 
     def test_optional_arg_with_multiple_kwargs(self):
         r = self.app_.get('/optional?id=6&dummy=dummy')
         assert r.status_int == 200
-        assert r.body == b_('optional: 6')
+        assert r.body == b'optional: 6'
 
     def test_optional_arg_with_multiple_url_encoded_kwargs(self):
         r = self.app_.get('/optional?id=Some%20Number&dummy=dummy')
         assert r.status_int == 200
-        assert r.body == b_('optional: Some Number')
+        assert r.body == b'optional: Some Number'
 
     def test_optional_arg_with_multiple_dictionary_kwargs(self):
         r = self.app_.post('/optional', {'id': '7', 'dummy': 'dummy'})
         assert r.status_int == 200
-        assert r.body == b_('optional: 7')
+        assert r.body == b'optional: 7'
 
     def test_optional_arg_with_multiple_json_kwargs(self):
         r = self.app_.post_json('/optional', {'id': '7', 'dummy': 'dummy'})
         assert r.status_int == 200
-        assert r.body == b_('optional: 7')
+        assert r.body == b'optional: 7'
 
     def test_optional_arg_with_multiple_url_encoded_dictionary_kwargs(self):
         r = self.app_.post('/optional', {
             'id': 'Some%20Number',
             'dummy': 'dummy'
         })
         assert r.status_int == 200
-        assert r.body == b_('optional: Some%20Number')
+        assert r.body == b'optional: Some%20Number'
 
         # multiple optional args
 
     def test_multiple_optional_positional_args(self):
         r = self.app_.get('/multiple_optional')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: None, None, None')
+        assert r.body == b'multiple_optional: None, None, None'
 
     def test_multiple_optional_positional_args_one_arg(self):
         r = self.app_.get('/multiple_optional/1')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: 1, None, None')
+        assert r.body == b'multiple_optional: 1, None, None'
 
     def test_multiple_optional_positional_args_one_url_encoded_arg(self):
         r = self.app_.get('/multiple_optional/One%21')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: One!, None, None')
+        assert r.body == b'multiple_optional: One!, None, None'
 
     def test_multiple_optional_positional_args_all_args(self):
         r = self.app_.get('/multiple_optional/1/2/3')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: 1, 2, 3')
+        assert r.body == b'multiple_optional: 1, 2, 3'
 
     def test_multiple_optional_positional_args_all_url_encoded_args(self):
         r = self.app_.get('/multiple_optional/One%21/Two%21/Three%21')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: One!, Two!, Three!')
+        assert r.body == b'multiple_optional: One!, Two!, Three!'
 
     def test_multiple_optional_positional_args_too_many_args(self):
         r = self.app_.get('/multiple_optional/1/2/3/dummy', status=404)
         assert r.status_int == 404
 
     def test_multiple_optional_positional_args_with_kwargs(self):
         r = self.app_.get('/multiple_optional?one=1')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: 1, None, None')
+        assert r.body == b'multiple_optional: 1, None, None'
 
     def test_multiple_optional_positional_args_with_url_encoded_kwargs(self):
         r = self.app_.get('/multiple_optional?one=One%21')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: One!, None, None')
+        assert r.body == b'multiple_optional: One!, None, None'
 
     def test_multiple_optional_positional_args_with_string_kwargs(self):
         r = self.app_.get('/multiple_optional/1?one=one')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: 1, None, None')
+        assert r.body == b'multiple_optional: 1, None, None'
 
     def test_multiple_optional_positional_args_with_encoded_str_kwargs(self):
         r = self.app_.get('/multiple_optional/One%21?one=one')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: One!, None, None')
+        assert r.body == b'multiple_optional: One!, None, None'
 
     def test_multiple_optional_positional_args_with_dict_kwargs(self):
         r = self.app_.post('/multiple_optional', {'one': '1'})
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: 1, None, None')
+        assert r.body == b'multiple_optional: 1, None, None'
 
     def test_multiple_optional_positional_args_with_json_kwargs(self):
         r = self.app_.post_json('/multiple_optional', {'one': '1'})
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: 1, None, None')
+        assert r.body == b'multiple_optional: 1, None, None'
 
     def test_multiple_optional_positional_args_with_encoded_dict_kwargs(self):
         r = self.app_.post('/multiple_optional', {'one': 'One%21'})
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: One%21, None, None')
+        assert r.body == b'multiple_optional: One%21, None, None'
 
     def test_multiple_optional_positional_args_and_dict_kwargs(self):
         r = self.app_.post('/multiple_optional/1', {'one': 'one'})
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: 1, None, None')
+        assert r.body == b'multiple_optional: 1, None, None'
 
     def test_multiple_optional_positional_args_and_json_kwargs(self):
         r = self.app_.post_json('/multiple_optional/1', {'one': 'one'})
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: 1, None, None')
+        assert r.body == b'multiple_optional: 1, None, None'
 
     def test_multiple_optional_encoded_positional_args_and_dict_kwargs(self):
         r = self.app_.post('/multiple_optional/One%21', {'one': 'one'})
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: One!, None, None')
+        assert r.body == b'multiple_optional: One!, None, None'
 
     def test_multiple_optional_args_with_multiple_kwargs(self):
         r = self.app_.get('/multiple_optional?one=1&two=2&three=3&four=4')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: 1, 2, 3')
+        assert r.body == b'multiple_optional: 1, 2, 3'
 
     def test_multiple_optional_args_with_multiple_encoded_kwargs(self):
         r = self.app_.get(
             '/multiple_optional?one=One%21&two=Two%21&three=Three%21&four=4'
         )
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: One!, Two!, Three!')
+        assert r.body == b'multiple_optional: One!, Two!, Three!'
 
     def test_multiple_optional_args_with_multiple_dict_kwargs(self):
         r = self.app_.post(
             '/multiple_optional',
             {'one': '1', 'two': '2', 'three': '3', 'four': '4'}
         )
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: 1, 2, 3')
+        assert r.body == b'multiple_optional: 1, 2, 3'
 
     def test_multiple_optional_args_with_multiple_json_kwargs(self):
         r = self.app_.post_json(
             '/multiple_optional',
             {'one': '1', 'two': '2', 'three': '3', 'four': '4'}
         )
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: 1, 2, 3')
+        assert r.body == b'multiple_optional: 1, 2, 3'
 
     def test_multiple_optional_args_with_multiple_encoded_dict_kwargs(self):
         r = self.app_.post(
             '/multiple_optional',
             {
                 'one': 'One%21',
                 'two': 'Two%21',
                 'three': 'Three%21',
                 'four': '4'
             }
         )
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: One%21, Two%21, Three%21')
+        assert r.body == b'multiple_optional: One%21, Two%21, Three%21'
 
     def test_multiple_optional_args_with_last_kwarg(self):
         r = self.app_.get('/multiple_optional?three=3')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: None, None, 3')
+        assert r.body == b'multiple_optional: None, None, 3'
 
     def test_multiple_optional_args_with_last_encoded_kwarg(self):
         r = self.app_.get('/multiple_optional?three=Three%21')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: None, None, Three!')
+        assert r.body == b'multiple_optional: None, None, Three!'
 
     def test_multiple_optional_args_with_middle_arg(self):
         r = self.app_.get('/multiple_optional', {'two': '2'})
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: None, 2, None')
+        assert r.body == b'multiple_optional: None, 2, None'
 
     def test_variable_args(self):
         r = self.app_.get('/variable_args')
         assert r.status_int == 200
-        assert r.body == b_('variable_args: ')
+        assert r.body == b'variable_args: '
 
     def test_multiple_variable_args(self):
         r = self.app_.get('/variable_args/1/dummy')
         assert r.status_int == 200
-        assert r.body == b_('variable_args: 1, dummy')
+        assert r.body == b'variable_args: 1, dummy'
 
     def test_multiple_encoded_variable_args(self):
         r = self.app_.get('/variable_args/Testing%20One%20Two/Three%21')
         assert r.status_int == 200
-        assert r.body == b_('variable_args: Testing One Two, Three!')
+        assert r.body == b'variable_args: Testing One Two, Three!'
 
     def test_variable_args_with_kwargs(self):
         r = self.app_.get('/variable_args?id=2&dummy=dummy')
         assert r.status_int == 200
-        assert r.body == b_('variable_args: ')
+        assert r.body == b'variable_args: '
 
     def test_variable_args_with_dict_kwargs(self):
         r = self.app_.post('/variable_args', {'id': '3', 'dummy': 'dummy'})
         assert r.status_int == 200
-        assert r.body == b_('variable_args: ')
+        assert r.body == b'variable_args: '
 
     def test_variable_args_with_json_kwargs(self):
         r = self.app_.post_json(
             '/variable_args',
             {'id': '3', 'dummy': 'dummy'}
         )
         assert r.status_int == 200
-        assert r.body == b_('variable_args: ')
+        assert r.body == b'variable_args: '
 
     def test_variable_kwargs(self):
         r = self.app_.get('/variable_kwargs')
         assert r.status_int == 200
-        assert r.body == b_('variable_kwargs: ')
+        assert r.body == b'variable_kwargs: '
 
     def test_multiple_variable_kwargs(self):
         r = self.app_.get('/variable_kwargs/1/dummy', status=404)
         assert r.status_int == 404
 
     def test_multiple_variable_kwargs_with_explicit_kwargs(self):
         r = self.app_.get('/variable_kwargs?id=2&dummy=dummy')
         assert r.status_int == 200
-        assert r.body == b_('variable_kwargs: dummy=dummy, id=2')
+        assert r.body == b'variable_kwargs: dummy=dummy, id=2'
 
     def test_multiple_variable_kwargs_with_explicit_encoded_kwargs(self):
         r = self.app_.get(
             '/variable_kwargs?id=Two%21&dummy=This%20is%20a%20test'
         )
         assert r.status_int == 200
-        assert r.body == b_('variable_kwargs: dummy=This is a test, id=Two!')
+        assert r.body == b'variable_kwargs: dummy=This is a test, id=Two!'
 
     def test_multiple_variable_kwargs_with_dict_kwargs(self):
         r = self.app_.post('/variable_kwargs', {'id': '3', 'dummy': 'dummy'})
         assert r.status_int == 200
-        assert r.body == b_('variable_kwargs: dummy=dummy, id=3')
+        assert r.body == b'variable_kwargs: dummy=dummy, id=3'
 
     def test_multiple_variable_kwargs_with_json_kwargs(self):
         r = self.app_.post_json(
             '/variable_kwargs',
             {'id': '3', 'dummy': 'dummy'}
         )
         assert r.status_int == 200
-        assert r.body == b_('variable_kwargs: dummy=dummy, id=3')
+        assert r.body == b'variable_kwargs: dummy=dummy, id=3'
 
     def test_multiple_variable_kwargs_with_encoded_dict_kwargs(self):
         r = self.app_.post(
             '/variable_kwargs',
             {'id': 'Three%21', 'dummy': 'This%20is%20a%20test'}
         )
         assert r.status_int == 200
-        result = 'variable_kwargs: dummy=This%20is%20a%20test, id=Three%21'
-        assert r.body == b_(result)
+        result = b'variable_kwargs: dummy=This%20is%20a%20test, id=Three%21'
+        assert r.body == result
 
     def test_variable_all(self):
         r = self.app_.get('/variable_all')
         assert r.status_int == 200
-        assert r.body == b_('variable_all: ')
+        assert r.body == b'variable_all: '
 
     def test_variable_all_with_one_extra(self):
         r = self.app_.get('/variable_all/1')
         assert r.status_int == 200
-        assert r.body == b_('variable_all: 1')
+        assert r.body == b'variable_all: 1'
 
     def test_variable_all_with_two_extras(self):
         r = self.app_.get('/variable_all/2/dummy')
         assert r.status_int == 200
-        assert r.body == b_('variable_all: 2, dummy')
+        assert r.body == b'variable_all: 2, dummy'
 
     def test_variable_mixed(self):
         r = self.app_.get('/variable_all/3?month=1&day=12')
         assert r.status_int == 200
-        assert r.body == b_('variable_all: 3, day=12, month=1')
+        assert r.body == b'variable_all: 3, day=12, month=1'
 
     def test_variable_mixed_explicit(self):
         r = self.app_.get('/variable_all/4?id=four&month=1&day=12')
         assert r.status_int == 200
-        assert r.body == b_('variable_all: 4, day=12, id=four, month=1')
+        assert r.body == b'variable_all: 4, day=12, id=four, month=1'
 
     def test_variable_post(self):
         r = self.app_.post('/variable_all/5/dummy')
         assert r.status_int == 200
-        assert r.body == b_('variable_all: 5, dummy')
+        assert r.body == b'variable_all: 5, dummy'
 
     def test_variable_post_with_kwargs(self):
         r = self.app_.post('/variable_all/6', {'month': '1', 'day': '12'})
         assert r.status_int == 200
-        assert r.body == b_('variable_all: 6, day=12, month=1')
+        assert r.body == b'variable_all: 6, day=12, month=1'
 
     def test_variable_post_with_json_kwargs(self):
         r = self.app_.post_json(
             '/variable_all/6',
             {'month': '1', 'day': '12'}
         )
         assert r.status_int == 200
-        assert r.body == b_('variable_all: 6, day=12, month=1')
+        assert r.body == b'variable_all: 6, day=12, month=1'
 
     def test_variable_post_mixed(self):
         r = self.app_.post(
             '/variable_all/7',
             {'id': 'seven', 'month': '1', 'day': '12'}
         )
         assert r.status_int == 200
-        assert r.body == b_('variable_all: 7, day=12, id=seven, month=1')
+        assert r.body == b'variable_all: 7, day=12, id=seven, month=1'
 
     def test_variable_post_mixed_with_json(self):
         r = self.app_.post_json(
             '/variable_all/7',
             {'id': 'seven', 'month': '1', 'day': '12'}
         )
         assert r.status_int == 200
-        assert r.body == b_('variable_all: 7, day=12, id=seven, month=1')
+        assert r.body == b'variable_all: 7, day=12, id=seven, month=1'
 
     def test_duplicate_query_parameters_GET(self):
         r = self.app_.get('/variable_kwargs?list=1&list=2')
-        l = [u_('1'), u_('2')]
         assert r.status_int == 200
-        assert r.body == b_('variable_kwargs: list=%s' % l)
+        assert r.body == b"variable_kwargs: list=['1', '2']"
 
     def test_duplicate_query_parameters_POST(self):
         r = self.app_.post('/variable_kwargs',
                            {'list': ['1', '2']})
-        l = [u_('1'), u_('2')]
         assert r.status_int == 200
-        assert r.body == b_('variable_kwargs: list=%s' % l)
+        assert r.body == b"variable_kwargs: list=['1', '2']"
 
     def test_duplicate_query_parameters_POST_mixed(self):
         r = self.app_.post('/variable_kwargs?list=1&list=2',
                            {'list': ['3', '4']})
-        l = [u_('1'), u_('2'), u_('3'), u_('4')]
         assert r.status_int == 200
-        assert r.body == b_('variable_kwargs: list=%s' % l)
+        assert r.body == b"variable_kwargs: list=['1', '2', '3', '4']"
 
     def test_duplicate_query_parameters_POST_mixed_json(self):
         r = self.app_.post('/variable_kwargs?list=1&list=2',
                            {'list': 3})
-        l = [u_('1'), u_('2'), u_('3')]
         assert r.status_int == 200
-        assert r.body == b_('variable_kwargs: list=%s' % l)
+        assert r.body == b"variable_kwargs: list=['1', '2', '3']"
 
     def test_staticmethod(self):
         r = self.app_.get('/static/foobar')
         assert r.status_int == 200
-        assert r.body == b_('id is foobar')
+        assert r.body == b'id is foobar'
 
     def test_no_remainder(self):
         try:
             r = self.app_.get('/eater')
             assert r.status_int != 200  # pragma: nocover
         except Exception as ex:
             assert type(ex) == TypeError
@@ -1005,104 +996,104 @@
                     "eater() missing 1 required positional argument: 'id'"
                 ),
             )  # this messaging changed in Python 3.3 and again in Python 3.10
 
     def test_one_remainder(self):
         r = self.app_.get('/eater/1')
         assert r.status_int == 200
-        assert r.body == b_('eater: 1, None, ')
+        assert r.body == b'eater: 1, None, '
 
     def test_two_remainders(self):
         r = self.app_.get('/eater/2/dummy')
         assert r.status_int == 200
-        assert r.body == b_('eater: 2, dummy, ')
+        assert r.body == b'eater: 2, dummy, '
 
     def test_many_remainders(self):
         r = self.app_.get('/eater/3/dummy/foo/bar')
         assert r.status_int == 200
-        assert r.body == b_('eater: 3, dummy, foo, bar')
+        assert r.body == b'eater: 3, dummy, foo, bar'
 
     def test_remainder_with_kwargs(self):
         r = self.app_.get('/eater/4?month=1&day=12')
         assert r.status_int == 200
-        assert r.body == b_('eater: 4, None, day=12, month=1')
+        assert r.body == b'eater: 4, None, day=12, month=1'
 
     def test_remainder_with_many_kwargs(self):
         r = self.app_.get('/eater/5?id=five&month=1&day=12&dummy=dummy')
         assert r.status_int == 200
-        assert r.body == b_('eater: 5, dummy, day=12, month=1')
+        assert r.body == b'eater: 5, dummy, day=12, month=1'
 
     def test_post_remainder(self):
         r = self.app_.post('/eater/6')
         assert r.status_int == 200
-        assert r.body == b_('eater: 6, None, ')
+        assert r.body == b'eater: 6, None, '
 
     def test_post_three_remainders(self):
         r = self.app_.post('/eater/7/dummy')
         assert r.status_int == 200
-        assert r.body == b_('eater: 7, dummy, ')
+        assert r.body == b'eater: 7, dummy, '
 
     def test_post_many_remainders(self):
         r = self.app_.post('/eater/8/dummy/foo/bar')
         assert r.status_int == 200
-        assert r.body == b_('eater: 8, dummy, foo, bar')
+        assert r.body == b'eater: 8, dummy, foo, bar'
 
     def test_post_remainder_with_kwargs(self):
         r = self.app_.post('/eater/9', {'month': '1', 'day': '12'})
         assert r.status_int == 200
-        assert r.body == b_('eater: 9, None, day=12, month=1')
+        assert r.body == b'eater: 9, None, day=12, month=1'
 
     def test_post_empty_remainder_with_json_kwargs(self):
         r = self.app_.post_json('/eater/9/', {'month': '1', 'day': '12'})
         assert r.status_int == 200
-        assert r.body == b_('eater: 9, None, day=12, month=1')
+        assert r.body == b'eater: 9, None, day=12, month=1'
 
     def test_post_remainder_with_json_kwargs(self):
         r = self.app_.post_json('/eater/9', {'month': '1', 'day': '12'})
         assert r.status_int == 200
-        assert r.body == b_('eater: 9, None, day=12, month=1')
+        assert r.body == b'eater: 9, None, day=12, month=1'
 
     def test_post_many_remainders_with_many_kwargs(self):
         r = self.app_.post(
             '/eater/10',
             {'id': 'ten', 'month': '1', 'day': '12', 'dummy': 'dummy'}
         )
         assert r.status_int == 200
-        assert r.body == b_('eater: 10, dummy, day=12, month=1')
+        assert r.body == b'eater: 10, dummy, day=12, month=1'
 
     def test_post_many_remainders_with_many_json_kwargs(self):
         r = self.app_.post_json(
             '/eater/10',
             {'id': 'ten', 'month': '1', 'day': '12', 'dummy': 'dummy'}
         )
         assert r.status_int == 200
-        assert r.body == b_('eater: 10, dummy, day=12, month=1')
+        assert r.body == b'eater: 10, dummy, day=12, month=1'
 
 
 class TestDefaultErrorRendering(PecanTestCase):
 
     def test_plain_error(self):
         class RootController(object):
             pass
 
         app = TestApp(Pecan(RootController()))
         r = app.get('/', status=404)
         assert r.status_int == 404
         assert r.content_type == 'text/plain'
-        assert r.body == b_(HTTPNotFound().plain_body({}))
+        assert r.body == HTTPNotFound().plain_body({}).encode('utf-8')
 
     def test_html_error(self):
         class RootController(object):
             pass
 
         app = TestApp(Pecan(RootController()))
         r = app.get('/', headers={'Accept': 'text/html'}, status=404)
         assert r.status_int == 404
         assert r.content_type == 'text/html'
-        assert r.body == b_(HTTPNotFound().html_body({}))
+        assert r.body == HTTPNotFound().html_body({}).encode('utf-8')
 
     def test_json_error(self):
         class RootController(object):
             pass
 
         app = TestApp(Pecan(RootController()))
         r = app.get('/', headers={'Accept': 'application/json'}, status=404)
@@ -1196,30 +1187,30 @@
         return TestApp(make_app(RootController(), debug=False))
 
     def test_index(self):
         r = self.app_.get('/')
         assert r.status_int == 302
         r = r.follow()
         assert r.status_int == 200
-        assert r.body == b_('it worked!')
+        assert r.body == b'it worked!'
 
     def test_internal(self):
         r = self.app_.get('/internal')
         assert r.status_int == 200
-        assert r.body == b_('it worked!')
+        assert r.body == b'it worked!'
 
     def test_internal_with_301(self):
         self.assertRaises(ValueError, self.app_.get, '/bad_internal')
 
     def test_permanent_redirect(self):
         r = self.app_.get('/permanent')
         assert r.status_int == 301
         r = r.follow()
         assert r.status_int == 200
-        assert r.body == b_('it worked!')
+        assert r.body == b'it worked!'
 
     def test_x_forward_proto(self):
         class ChildController(object):
             @expose()
             def index(self):
                 redirect('/testing')  # pragma: nocover
 
@@ -1282,48 +1273,48 @@
     def test_streaming_response(self):
 
         class RootController(object):
             @expose(content_type='text/plain')
             def test(self, foo):
                 if foo == 'stream':
                     # mimic large file
-                    contents = six.BytesIO(b_('stream'))
+                    contents = BytesIO(b'stream')
                     response.content_type = 'application/octet-stream'
                     contents.seek(0, os.SEEK_END)
                     response.content_length = contents.tell()
                     contents.seek(0, os.SEEK_SET)
                     response.app_iter = contents
                     return response
                 else:
                     return 'plain text'
 
         app = TestApp(Pecan(RootController()))
         r = app.get('/test/stream')
         assert r.content_type == 'application/octet-stream'
-        assert r.body == b_('stream')
+        assert r.body == b'stream'
 
         r = app.get('/test/plain')
         assert r.content_type == 'text/plain'
-        assert r.body == b_('plain text')
+        assert r.body == b'plain text'
 
 
 class TestManualResponse(PecanTestCase):
 
     def test_manual_response(self):
 
         class RootController(object):
             @expose()
             def index(self):
                 resp = webob.Response(response.environ)
-                resp.body = b_('Hello, World!')
+                resp.body = b'Hello, World!'
                 return resp
 
         app = TestApp(Pecan(RootController()))
         r = app.get('/')
-        assert r.body == b_('Hello, World!')
+        assert r.body == b'Hello, World!'
 
 
 class TestCustomResponseandRequest(PecanTestCase):
 
     def test_custom_objects(self):
 
         class CustomRequest(Request):
@@ -1349,15 +1340,15 @@
 
         app = TestApp(Pecan(
             RootController(),
             request_cls=CustomRequest,
             response_cls=CustomResponse
         ))
         r = app.get('/')
-        assert r.body == b_('ABC')
+        assert r.body == b'ABC'
         assert r.headers.get('X-Custom-Response') == 'XYZ'
 
 
 class TestThreadLocalState(PecanTestCase):
 
     def test_thread_local_dir(self):
         """
@@ -1370,15 +1361,15 @@
                 assert 'method' in dir(request)
                 assert 'status' in dir(response)
                 return '/'
 
         app = TestApp(Pecan(RootController()))
         r = app.get('/')
         assert r.status_int == 200
-        assert r.body == b_('/')
+        assert r.body == b'/'
 
     def test_request_state_cleanup(self):
         """
         After a request, the state local() should be totally clean
         except for state.app (so that objects don't leak between requests)
         """
         from pecan.core import state
@@ -1387,15 +1378,15 @@
             @expose()
             def index(self):
                 return '/'
 
         app = TestApp(Pecan(RootController()))
         r = app.get('/')
         assert r.status_int == 200
-        assert r.body == b_('/')
+        assert r.body == b'/'
 
         assert state.__dict__ == {}
 
 
 class TestFileTypeExtensions(PecanTestCase):
 
     @property
@@ -1414,48 +1405,48 @@
 
         return TestApp(Pecan(RootController()))
 
     def test_html_extension(self):
         for path in ('/index.html', '/index.html/'):
             r = self.app_.get(path)
             assert r.status_int == 200
-            assert r.body == b_('.html')
+            assert r.body == b'.html'
 
     def test_image_extension(self):
         for path in ('/index.png', '/index.png/'):
             r = self.app_.get(path)
             assert r.status_int == 200
-            assert r.body == b_('.png')
+            assert r.body == b'.png'
 
     def test_hidden_file(self):
         for path in ('/.vimrc', '/.vimrc/'):
             r = self.app_.get(path)
             assert r.status_int == 204
-            assert r.body == b_('')
+            assert r.body == b''
 
     def test_multi_dot_extension(self):
         for path in ('/gradient.min.js', '/gradient.min.js/'):
             r = self.app_.get(path)
             assert r.status_int == 200
-            assert r.body == b_('.js')
+            assert r.body == b'.js'
 
     def test_bad_content_type(self):
         class RootController(object):
             @expose()
             def index(self):
                 return '/'
 
         app = TestApp(Pecan(RootController()))
         r = app.get('/')
         assert r.status_int == 200
-        assert r.body == b_('/')
+        assert r.body == b'/'
 
         r = app.get('/index.html', expect_errors=True)
         assert r.status_int == 200
-        assert r.body == b_('/')
+        assert r.body == b'/'
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             r = app.get('/index.txt', expect_errors=True)
             assert r.status_int == 404
 
     def test_unknown_file_extension(self):
@@ -1466,30 +1457,30 @@
                 assert request.pecan['extension'] is None
                 return 'SOME VALUE'
 
         app = TestApp(Pecan(RootController()))
 
         r = app.get('/example:x.tiny')
         assert r.status_int == 200
-        assert r.body == b_('SOME VALUE')
+        assert r.body == b'SOME VALUE'
 
     def test_guessing_disabled(self):
         class RootController(object):
             @expose(content_type=None)
             def _default(self, *args):
                 assert 'index.html' in args
                 assert request.pecan['extension'] is None
                 return 'SOME VALUE'
 
         app = TestApp(Pecan(RootController(),
                             guess_content_type_from_ext=False))
 
         r = app.get('/index.html')
         assert r.status_int == 200
-        assert r.body == b_('SOME VALUE')
+        assert r.body == b'SOME VALUE'
 
     def test_content_type_guessing_disabled(self):
 
         class ResourceController(object):
 
             def __init__(self, name):
                 self.name = name
@@ -1613,31 +1604,31 @@
             accept = AcceptController()
 
         return TestApp(Pecan(RootController()))
 
     def test_root(self):
         r = self.app_.get('/')
         assert r.status_int == 200
-        assert b_('index') in r.body
+        assert b'index' in r.body
 
     def test_index(self):
         r = self.app_.get('/index')
         assert r.status_int == 200
-        assert b_('index') in r.body
+        assert b'index' in r.body
 
     def test_broken_clients(self):
         # for broken clients
         r = self.app_.get('', status=302)
         assert r.status_int == 302
         assert r.location == 'http://localhost/'
 
     def test_sub_controller_with_trailing(self):
         r = self.app_.get('/sub/')
         assert r.status_int == 200
-        assert b_('subindex') in r.body
+        assert b'subindex' in r.body
 
     def test_sub_controller_redirect(self):
         r = self.app_.get('/sub', status=302)
         assert r.status_int == 302
         assert r.location == 'http://localhost/sub/'
 
     def test_with_query_string(self):
@@ -1652,25 +1643,25 @@
             raise Exception("Post should fail")  # pragma: nocover
         except Exception as e:
             assert isinstance(e, RuntimeError)
 
     def test_with_args(self):
         r = self.app_.get('/arg/index/foo')
         assert r.status_int == 200
-        assert r.body == b_('foo')
+        assert r.body == b'foo'
 
     def test_accept_noncanonical(self):
         r = self.app_.get('/accept/')
         assert r.status_int == 200
-        assert r.body == b_('accept')
+        assert r.body == b'accept'
 
     def test_accept_noncanonical_no_trailing_slash(self):
         r = self.app_.get('/accept')
         assert r.status_int == 200
-        assert r.body == b_('accept')
+        assert r.body == b'accept'
 
 
 class TestNonCanonical(PecanTestCase):
 
     @property
     def app_(self):
         class ArgSubController(object):
@@ -1699,30 +1690,30 @@
             accept = AcceptController()
 
         return TestApp(Pecan(RootController(), force_canonical=False))
 
     def test_index(self):
         r = self.app_.get('/')
         assert r.status_int == 200
-        assert b_('index') in r.body
+        assert b'index' in r.body
 
     def test_subcontroller(self):
         r = self.app_.get('/sub')
         assert r.status_int == 200
-        assert b_('subindex') in r.body
+        assert b'subindex' in r.body
 
     def test_subcontroller_with_kwargs(self):
         r = self.app_.post('/sub', dict(foo=1))
         assert r.status_int == 200
-        assert b_('subindex') in r.body
+        assert b'subindex' in r.body
 
     def test_sub_controller_with_trailing(self):
         r = self.app_.get('/sub/')
         assert r.status_int == 200
-        assert b_('subindex') in r.body
+        assert b'subindex' in r.body
 
     def test_proxy(self):
         class RootController(object):
             @expose()
             def index(self):
                 request.testing = True
                 assert request.testing is True
@@ -1825,19 +1816,19 @@
                 return dict()
 
         app = TestApp(
             Pecan(RootController(), template_path=self.template_path)
         )
         r = app.get('/')
         assert r.status_int == 200
-        assert b_("<h1>Hello, Jonathan!</h1>") in r.body
+        assert b"<h1>Hello, Jonathan!</h1>" in r.body
 
         r = app.get('/index.html?name=World')
         assert r.status_int == 200
-        assert b_("<h1>Hello, World!</h1>") in r.body
+        assert b"<h1>Hello, World!</h1>" in r.body
 
         error_msg = None
         try:
             r = app.get('/badtemplate.html')
         except Exception as e:
             for error_f in error_formatters:
                 error_msg = error_f(e)
@@ -1854,19 +1845,19 @@
                 return dict(name=name)
 
         app = TestApp(
             Pecan(RootController(), template_path=self.template_path)
         )
         r = app.get('/')
         assert r.status_int == 200
-        assert b_("<h1>Hello, Jonathan!</h1>") in r.body
+        assert b"<h1>Hello, Jonathan!</h1>" in r.body
 
         r = app.get('/index.html?name=World')
         assert r.status_int == 200
-        assert b_("<h1>Hello, World!</h1>") in r.body
+        assert b"<h1>Hello, World!</h1>" in r.body
 
     @unittest.skipIf('jinja' not in builtin_renderers, 'Jinja not installed')
     def test_jinja(self):
 
         class RootController(object):
             @expose('jinja:jinja.html')
             def index(self, name='Jonathan'):
@@ -1877,15 +1868,15 @@
                 return dict()
 
         app = TestApp(
             Pecan(RootController(), template_path=self.template_path)
         )
         r = app.get('/')
         assert r.status_int == 200
-        assert b_("<h1>Hello, Jonathan!</h1>") in r.body
+        assert b"<h1>Hello, Jonathan!</h1>" in r.body
 
         error_msg = None
         try:
             r = app.get('/badtemplate.html')
         except Exception as e:
             for error_f in error_formatters:
                 error_msg = error_f(e)
@@ -1906,19 +1897,19 @@
                 return dict()
 
         app = TestApp(
             Pecan(RootController(), template_path=self.template_path)
         )
         r = app.get('/')
         assert r.status_int == 200
-        assert b_("<h1>Hello, Jonathan!</h1>") in r.body
+        assert b"<h1>Hello, Jonathan!</h1>" in r.body
 
         r = app.get('/index.html?name=World')
         assert r.status_int == 200
-        assert b_("<h1>Hello, World!</h1>") in r.body
+        assert b"<h1>Hello, World!</h1>" in r.body
 
         error_msg = None
         try:
             r = app.get('/badtemplate.html')
         except Exception as e:
             for error_f in error_formatters:
                 error_msg = error_f(e)
@@ -1980,45 +1971,45 @@
         app = TestApp(Pecan(
             RootController(),
             template_path=self.template_path,
             custom_renderers={'backwards': BackwardsRenderer}
         ))
         r = app.get('/')
         assert r.status_int == 200
-        assert b_("<h1>Hello, eoJ!</h1>") in r.body
+        assert b"<h1>Hello, eoJ!</h1>" in r.body
 
         r = app.get('/index.html?name=Tim')
         assert r.status_int == 200
-        assert b_("<h1>Hello, miT!</h1>") in r.body
+        assert b"<h1>Hello, miT!</h1>" in r.body
 
     def test_override_template(self):
         class RootController(object):
             @expose('foo.html')
             def index(self):
                 override_template(None, content_type='text/plain')
                 return 'Override'
 
         app = TestApp(Pecan(RootController()))
         r = app.get('/')
         assert r.status_int == 200
-        assert b_('Override') in r.body
+        assert b'Override' in r.body
         assert r.content_type == 'text/plain'
 
     def test_render(self):
         class RootController(object):
             @expose()
             def index(self, name='Jonathan'):
                 return render('mako.html', dict(name=name))
 
         app = TestApp(
             Pecan(RootController(), template_path=self.template_path)
         )
         r = app.get('/')
         assert r.status_int == 200
-        assert b_("<h1>Hello, Jonathan!</h1>") in r.body
+        assert b"<h1>Hello, Jonathan!</h1>" in r.body
 
     def test_default_json_renderer(self):
 
         class RootController(object):
             @expose()
             def index(self, name='Bill'):
                 return dict(name=name)
@@ -2035,15 +2026,15 @@
             @expose(content_type='text/plain')
             def index(self, name='Bill'):
                 return name
 
         app = TestApp(Pecan(RootController(), default_renderer='json'))
         r = app.get('/')
         assert r.status_int == 200
-        assert r.body == b_("Bill")
+        assert r.body == b"Bill"
 
 
 class TestDeprecatedRouteMethod(PecanTestCase):
 
     @property
     def app_(self):
         class RootController(object):
@@ -2059,15 +2050,15 @@
         return TestApp(Pecan(RootController()))
 
     def test_required_argument(self):
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             r = self.app_.get('/foo/bar/')
             assert r.status_int == 200
-            assert b_('foo, bar') in r.body
+            assert b'foo, bar' in r.body
 
 
 class TestExplicitRoute(PecanTestCase):
 
     def test_alternate_route(self):
 
         class RootController(object):
@@ -2076,15 +2067,15 @@
             def some_path(self):
                 return 'Hello, World!'
 
         app = TestApp(Pecan(RootController()))
 
         r = app.get('/some-path/')
         assert r.status_int == 200
-        assert r.body == b_('Hello, World!')
+        assert r.body == b'Hello, World!'
 
         r = app.get('/some_path/', expect_errors=True)
         assert r.status_int == 404
 
     def test_manual_route(self):
 
         class SubController(object):
@@ -2098,15 +2089,15 @@
 
         route(RootController, 'some-controller', SubController())
 
         app = TestApp(Pecan(RootController()))
 
         r = app.get('/some-controller/some-path/')
         assert r.status_int == 200
-        assert r.body == b_('Hello, World!')
+        assert r.body == b'Hello, World!'
 
         r = app.get('/some-controller/some_path/', expect_errors=True)
         assert r.status_int == 404
 
     def test_manual_route_conflict(self):
 
         class SubController(object):
@@ -2134,19 +2125,19 @@
             def index(self):
                 return 'Hello, World!'
 
         app = TestApp(Pecan(RootController()))
 
         r = app.get('/some-path/')
         assert r.status_int == 200
-        assert r.body == b_('Hello, World!')
+        assert r.body == b'Hello, World!'
 
         r = app.get('/')
         assert r.status_int == 200
-        assert r.body == b_('Hello, World!')
+        assert r.body == b'Hello, World!'
 
         r = app.get('/index/', expect_errors=True)
         assert r.status_int == 404
 
     def test_custom_route_with_attribute_conflict(self):
 
         class RootController(object):
@@ -2200,18 +2191,18 @@
 
         class RootController(BaseController):
             child = ChildController()
 
         app = TestApp(Pecan(RootController()))
 
         r = app.get('/testing/')
-        assert r.body == b_('/testing/')
+        assert r.body == b'/testing/'
 
         r = app.get('/child/testing/')
-        assert r.body == b_('/child/testing/')
+        assert r.body == b'/child/testing/'
 
     def test_custom_route_prohibited_on_lookup(self):
         try:
             class RootController(object):
 
                 @expose(route='some-path')
                 def _lookup(self):
@@ -2263,22 +2254,22 @@
             def handle_post(self):
                 return 'POST!'
 
         app = TestApp(Pecan(RootController()))
 
         r = app.get('/some-path/')
         assert r.status_int == 200
-        assert r.body == b_('Hello, World!')
+        assert r.body == b'Hello, World!'
 
         r = app.get('/foo/', expect_errors=True)
         assert r.status_int == 404
 
         r = app.post('/some-path/')
         assert r.status_int == 200
-        assert r.body == b_('POST!')
+        assert r.body == b'POST!'
 
         r = app.post('/foo/', expect_errors=True)
         assert r.status_int == 404
 
     def test_custom_route_prohibited_on_generic_controllers(self):
         try:
             class RootController(object):
```

### Comparing `pecan-1.4.2/pecan/tests/test_commands.py` & `pecan-1.5.0/pecan/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/tests/test_conf.py` & `pecan-1.5.0/pecan/tests/test_conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import os
-import sys
 import tempfile
 import unittest
 
-from six import b as b_
 from webtest import TestApp
 
 import pecan
 from pecan.tests import PecanTestCase
 
 
 __here__ = os.path.dirname(__file__)
@@ -144,28 +142,28 @@
             configuration.conf_from_file,
             os.path.join(__here__, 'config_fixtures', *path)
         )
 
     def test_config_with_syntax_error(self):
         from pecan import configuration
         with tempfile.NamedTemporaryFile('wb') as f:
-            f.write(b_('\n'.join(['if false', 'var = 3'])))
+            f.write(b'\n'.join([b'if false', b'var = 3']))
             f.flush()
             configuration.Config({})
 
             self.assertRaises(
                 SyntaxError,
                 configuration.conf_from_file,
                 f.name
             )
 
     def test_config_with_non_package_relative_import(self):
         from pecan import configuration
         with tempfile.NamedTemporaryFile('wb', suffix='.py') as f:
-            f.write(b_('\n'.join(['from . import variables'])))
+            f.write(b'\n'.join([b'from . import variables']))
             f.flush()
             configuration.Config({})
 
             try:
                 configuration.conf_from_file(f.name)
             except (ValueError, SystemError, ImportError) as e:
                 assert 'relative import' in str(e)
```

### Comparing `pecan-1.4.2/pecan/tests/test_generic.py` & `pecan-1.5.0/pecan/tests/test_generic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from json import dumps
 from webtest import TestApp
 
-from six import b as b_
-
 from pecan import Pecan, expose, abort
 from pecan.tests import PecanTestCase
 
 
 class TestGeneric(PecanTestCase):
 
     def test_simple_generic(self):
@@ -22,19 +20,19 @@
             @index.when(method='GET')
             def do_get(self):
                 return 'GET'
 
         app = TestApp(Pecan(RootController()))
         r = app.get('/')
         assert r.status_int == 200
-        assert r.body == b_('GET')
+        assert r.body == b'GET'
 
         r = app.post('/')
         assert r.status_int == 200
-        assert r.body == b_(dumps(dict(result='POST')))
+        assert r.body == dumps(dict(result='POST')).encode('utf-8')
 
         r = app.get('/do_get', status=404)
         assert r.status_int == 404
 
     def test_generic_allow_header(self):
         class RootController(object):
             @expose(generic=True)
@@ -74,19 +72,21 @@
 
         class RootController(object):
             sub = SubController()
 
         app = TestApp(Pecan(RootController()))
         r = app.get('/sub/sub/')
         assert r.status_int == 200
-        assert r.body == b_('GET')
+        assert r.body == b'GET'
 
         r = app.delete('/sub/sub/joe/is/cool')
         assert r.status_int == 200
-        assert r.body == b_(dumps(dict(result='joe', args='is, cool')))
+        assert r.body == dumps(
+            dict(result='joe', args='is, cool')
+        ).encode('utf-8')
 
 
 class TestGenericWithSpecialMethods(PecanTestCase):
 
     def test_generics_not_allowed(self):
 
         class C(object):
```

### Comparing `pecan-1.4.2/pecan/tests/test_hooks.py` & `pecan-1.5.0/pecan/tests/test_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import inspect
 import operator
+from io import StringIO
 
 from webtest import TestApp
-from six import PY3
-from six import b as b_
-from six import u as u_
-from six.moves import cStringIO as StringIO
 
 from pecan import make_app, expose, redirect, abort, rest, Request, Response
 from pecan.hooks import (
     PecanHook, TransactionHook, HookController, RequestViewerHook
 )
 from pecan.configuration import Config
 from pecan.decorators import transactional, after_commit, after_rollback
 from pecan.tests import PecanTestCase
 
 # The `inspect.Arguments` namedtuple is different between PY2/3
-kwargs = operator.attrgetter('varkw' if PY3 else 'keywords')
+kwargs = operator.attrgetter('varkw')
 
 
 class TestHooks(PecanTestCase):
 
     def test_basic_single_hook(self):
         run_hook = []
 
@@ -42,15 +39,15 @@
 
             def on_error(self, state, e):
                 run_hook.append('error')
 
         app = TestApp(make_app(RootController(), hooks=[SimpleHook()]))
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
 
         assert len(run_hook) == 4
         assert run_hook[0] == 'on_route'
         assert run_hook[1] == 'before'
         assert run_hook[2] == 'inside'
         assert run_hook[3] == 'after'
 
@@ -80,15 +77,15 @@
                 run_hook.append('error' + self.id)
 
         app = TestApp(make_app(RootController(), hooks=[
             SimpleHook(1), SimpleHook(2), SimpleHook(3)
         ]))
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
 
         assert len(run_hook) == 10
         assert run_hook[0] == 'on_route1'
         assert run_hook[1] == 'on_route2'
         assert run_hook[2] == 'on_route3'
         assert run_hook[3] == 'before1'
         assert run_hook[4] == 'before2'
@@ -121,15 +118,15 @@
 
         app = TestApp(make_app(RootController(), hooks=[
             ErrorHook(), OnRouteHook()
         ]))
 
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello World!')
+        assert response.body == b'Hello World!'
 
         assert len(run_hook) == 2
         assert run_hook[0] == 'on_route'
         assert run_hook[1] == 'inside'
 
         run_hook = []
         try:
@@ -150,15 +147,15 @@
                 return [][1]
 
         class ErrorHook(PecanHook):
             def on_error(self, state, e):
                 run_hook.append('error')
 
                 r = Response()
-                r.text = u_('on_error')
+                r.text = 'on_error'
 
                 return r
 
         app = TestApp(make_app(RootController(), hooks=[
             ErrorHook()
         ]))
 
@@ -197,15 +194,15 @@
 
         papp = make_app(RootController(), hooks=[
             SimpleHook(1, 3), SimpleHook(2, 2), SimpleHook(3, 1)
         ])
         app = TestApp(papp)
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
 
         assert len(run_hook) == 10
         assert run_hook[0] == 'on_route3'
         assert run_hook[1] == 'on_route2'
         assert run_hook[2] == 'on_route1'
         assert run_hook[3] == 'before3'
         assert run_hook[4] == 'before2'
@@ -254,34 +251,34 @@
                 return 'Hello, World!'
 
             sub = SubController()
 
         app = TestApp(make_app(RootController()))
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
 
         assert len(run_hook) == 1
         assert run_hook[0] == 'inside'
 
         run_hook = []
 
         response = app.get('/sub/')
         assert response.status_int == 200
-        assert response.body == b_('Inside here!')
+        assert response.body == b'Inside here!'
 
         assert len(run_hook) == 3
         assert run_hook[0] == 'before'
         assert run_hook[1] == 'inside_sub'
         assert run_hook[2] == 'after'
 
         run_hook = []
         response = app.get('/sub/sub/')
         assert response.status_int == 200
-        assert response.body == b_('Deep inside here!')
+        assert response.body == b'Deep inside here!'
 
         assert len(run_hook) == 3
         assert run_hook[0] == 'before'
         assert run_hook[1] == 'inside_sub_sub'
         assert run_hook[2] == 'after'
 
     def test_isolated_hook_with_global_hook(self):
@@ -318,27 +315,27 @@
                 return 'Hello, World!'
 
             sub = SubController()
 
         app = TestApp(make_app(RootController(), hooks=[SimpleHook(1)]))
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
 
         assert len(run_hook) == 4
         assert run_hook[0] == 'on_route1'
         assert run_hook[1] == 'before1'
         assert run_hook[2] == 'inside'
         assert run_hook[3] == 'after1'
 
         run_hook = []
 
         response = app.get('/sub/')
         assert response.status_int == 200
-        assert response.body == b_('Inside here!')
+        assert response.body == b'Inside here!'
 
         assert len(run_hook) == 6
         assert run_hook[0] == 'on_route1'
         assert run_hook[1] == 'before2'
         assert run_hook[2] == 'before1'
         assert run_hook[3] == 'inside_sub'
         assert run_hook[4] == 'after1'
@@ -391,26 +388,26 @@
 
             sub = SubController()
 
         papp = make_app(RootController())
         app = TestApp(papp)
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
 
         assert len(run_hook) == 4
         assert run_hook[0] == 'simple - before hook', run_hook[0]
         assert run_hook[1] == 'helper - before hook', run_hook[1]
         assert run_hook[2] == 'last - before hook', run_hook[2]
         assert run_hook[3] == 'inside', run_hook[3]
 
         run_hook = []
         response = app.get('/sub/')
         assert response.status_int == 200
-        assert response.body == b_('This is sub controller!')
+        assert response.body == b'This is sub controller!'
 
         assert len(run_hook) == 4, run_hook
         assert run_hook[0] == 'simple - before hook', run_hook[0]
         assert run_hook[1] == 'helper - before hook', run_hook[1]
         assert run_hook[2] == 'last - before hook', run_hook[2]
         # LastHook is invoked once again -
         # for each different instance of the Hook in the two Controllers
@@ -430,15 +427,15 @@
 
         class SimpleHook(PecanHook):
             def after(self, state):
                 run_hook.append('after')
 
         app = TestApp(make_app(RootController(), hooks=[SimpleHook()]))
         response = app.get('/internal')
-        assert response.body == b_('it worked!')
+        assert response.body == b'it worked!'
 
         assert len(run_hook) == 1
 
 
 class TestStateAccess(PecanTestCase):
 
     def setUp(self):
@@ -826,26 +823,26 @@
                 rollback=gen('rollback'),
                 clear=gen('clear')
             )
         ]))
 
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
 
         assert len(run_hook) == 3
         assert run_hook[0] == 'start_ro'
         assert run_hook[1] == 'inside'
         assert run_hook[2] == 'clear'
 
         run_hook = []
 
         response = app.post('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
 
         assert len(run_hook) == 4
         assert run_hook[0] == 'start'
         assert run_hook[1] == 'inside'
         assert run_hook[2] == 'commit'
         assert run_hook[3] == 'clear'
 
@@ -932,39 +929,39 @@
                 rollback=gen('rollback'),
                 clear=gen('clear')
             )
         ]))
 
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Index Method!')
+        assert response.body == b'Index Method!'
 
         assert len(run_hook) == 3
         assert run_hook[0] == 'start_ro'
         assert run_hook[1] == 'inside'
         assert run_hook[2] == 'clear'
 
         run_hook = []
 
         response = app.post('/')
         assert response.status_int == 200
-        assert response.body == b_('Index Method!')
+        assert response.body == b'Index Method!'
 
         assert len(run_hook) == 5
         assert run_hook[0] == 'start'
         assert run_hook[1] == 'inside'
         assert run_hook[2] == 'commit'
         assert run_hook[3] == 'action-one'
         assert run_hook[4] == 'clear'
 
         run_hook = []
 
         response = app.get('/decorated')
         assert response.status_int == 200
-        assert response.body == b_('Decorated Method!')
+        assert response.body == b'Decorated Method!'
 
         assert len(run_hook) == 7
         assert run_hook[0] == 'start_ro'
         assert run_hook[1] == 'clear'
         assert run_hook[2] == 'start'
         assert run_hook[3] == 'inside'
         assert run_hook[4] == 'commit'
@@ -1061,28 +1058,28 @@
                 rollback=gen('rollback'),
                 clear=gen('clear')
             )
         ]))
 
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
 
         assert len(run_hook) == 3
         assert run_hook[0] == 'start_ro'
         assert run_hook[1] == 'inside'
         assert run_hook[2] == 'clear'
 
         run_hook = []
 
         # test hooks for /
 
         response = app.post('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
 
         assert len(run_hook) == 4
         assert run_hook[0] == 'start'
         assert run_hook[1] == 'inside'
         assert run_hook[2] == 'commit'
         assert run_hook[3] == 'clear'
 
@@ -1304,15 +1301,15 @@
                 rollback=gen('rollback'),
                 clear=gen('clear')
             )
         ]))
 
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
 
         assert len(run_hook) == 6
         assert run_hook[0] == 'start_ro'
         assert run_hook[1] == 'clear'
         assert run_hook[2] == 'start'
         assert run_hook[3] == 'inside'
         assert run_hook[4] == 'commit'
@@ -1320,15 +1317,15 @@
 
         run_hook = []
 
         # test hooks for /
 
         response = app.post('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
 
         assert len(run_hook) == 4
         assert run_hook[0] == 'start'
         assert run_hook[1] == 'inside'
         assert run_hook[2] == 'commit'
         assert run_hook[3] == 'clear'
 
@@ -1429,15 +1426,15 @@
         # This controller should always be transactional,
         #
 
         run_hook = []
 
         response = app.get('/generic')
         assert response.status_int == 200
-        assert response.body == b_('generic get')
+        assert response.body == b'generic get'
         assert len(run_hook) == 6
         assert run_hook[0] == 'start_ro'
         assert run_hook[1] == 'clear'
         assert run_hook[2] == 'start'
         assert run_hook[3] == 'inside'
         assert run_hook[4] == 'commit'
         assert run_hook[5] == 'clear'
@@ -1447,15 +1444,15 @@
         # This controller should always be transactional,
         #
 
         run_hook = []
 
         response = app.post('/generic')
         assert response.status_int == 200
-        assert response.body == b_('generic post')
+        assert response.body == b'generic post'
         assert len(run_hook) == 4
         assert run_hook[0] == 'start'
         assert run_hook[1] == 'inside'
         assert run_hook[2] == 'commit'
         assert run_hook[3] == 'clear'
 
     def test_transaction_hook_with_broken_hook(self):
@@ -1521,15 +1518,15 @@
             )
         )
         response = app.get('/')
 
         out = _stdout.getvalue()
 
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
         assert 'path' in out
         assert 'method' in out
         assert 'status' in out
         assert 'method' in out
         assert 'params' in out
         assert 'hooks' in out
         assert '200 OK' in out
@@ -1588,15 +1585,15 @@
             )
         )
         response = app.get('/')
 
         out = _stdout.getvalue()
 
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
         assert '/' in out
         assert 'path' in out
         assert 'method' not in out
         assert 'status' not in out
         assert 'method' not in out
         assert 'params' not in out
         assert 'hooks' not in out
@@ -1623,15 +1620,15 @@
             )
         )
         response = app.get('/')
 
         out = _stdout.getvalue()
 
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
         assert out == ''
 
     def test_item_not_in_defaults(self):
 
         _stdout = StringIO()
 
         class RootController(object):
@@ -1650,15 +1647,15 @@
             )
         )
         response = app.get('/')
 
         out = _stdout.getvalue()
 
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
         assert 'date' in out
         assert 'method' not in out
         assert 'status' not in out
         assert 'method' not in out
         assert 'params' not in out
         assert 'hooks' not in out
         assert '200 OK' not in out
@@ -1720,14 +1717,14 @@
             make_app(
                 RootController()
             )
         )
 
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
         assert response.headers['X-Testing'] == 'XYZ'
 
         response = app.delete('/100/')
         assert response.status_int == 200
-        assert response.body == b_('Deleting 100')
+        assert response.body == b'Deleting 100'
         assert response.headers['X-Testing'] == 'XYZ'
```

### Comparing `pecan-1.4.2/pecan/tests/test_jsonify.py` & `pecan-1.5.0/pecan/tests/test_jsonify.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from datetime import datetime, date
 from decimal import Decimal
 from json import loads
 try:
     from sqlalchemy import orm, schema, types
     from sqlalchemy.engine import create_engine
+    from sqlalchemy.orm import registry
 except ImportError:
     create_engine = None  # noqa
 
 from webtest import TestApp
 from webob.multidict import MultiDict
 
 from pecan.jsonify import jsonify, encode, ResultProxy, RowProxy
@@ -175,56 +176,56 @@
         self.row_proxy = FakeRowProxy([
             ('id', 1), ('first_name', 'Jonathan'), ('last_name', 'LaCour')
         ])
 
     def create_sa_proxies(self):
 
         # create the table and mapper
+        mapper_registry = registry()
         metadata = schema.MetaData()
         user_table = schema.Table(
             'user',
             metadata,
             schema.Column('id', types.Integer, primary_key=True),
             schema.Column('first_name', types.Unicode(25)),
             schema.Column('last_name', types.Unicode(25))
         )
 
         class User(object):
             pass
-        orm.mapper(User, user_table)
+        mapper_registry.map_imperatively(User, user_table)
 
         # create the session
         engine = create_engine('sqlite:///:memory:')
         metadata.bind = engine
-        metadata.create_all()
+        metadata.create_all(metadata.bind)
         session = orm.sessionmaker(bind=engine)()
 
         # add some dummy data
-        user_table.insert().execute([
-            {'first_name': 'Jonathan', 'last_name': 'LaCour'},
-            {'first_name': 'Yoann', 'last_name': 'Roman'}
-        ])
+        session.add(User(first_name='Jonathan', last_name='LaCour'))
+        session.add(User(first_name='Ryan', last_name='Petrello'))
+        session.commit()
 
         # get the SA objects
         self.sa_object = session.query(User).first()
         select = user_table.select()
-        self.result_proxy = select.execute()
-        self.row_proxy = select.execute().fetchone()
+        self.result_proxy = session.execute(select)
+        self.row_proxy = session.execute(select).fetchone()
 
     def test_sa_object(self):
         result = encode(self.sa_object)
         assert loads(result) == {
             'id': 1, 'first_name': 'Jonathan', 'last_name': 'LaCour'
         }
 
     def test_result_proxy(self):
         result = encode(self.result_proxy)
         assert loads(result) == {'count': 2, 'rows': [
             {'id': 1, 'first_name': 'Jonathan', 'last_name': 'LaCour'},
-            {'id': 2, 'first_name': 'Yoann', 'last_name': 'Roman'}
+            {'id': 2, 'first_name': 'Ryan', 'last_name': 'Petrello'}
         ]}
 
     def test_row_proxy(self):
         result = encode(self.row_proxy)
         assert loads(result) == {
             'id': 1, 'first_name': 'Jonathan', 'last_name': 'LaCour'
         }
```

### Comparing `pecan-1.4.2/pecan/tests/test_no_thread_locals.py` & `pecan-1.5.0/pecan/tests/test_no_thread_locals.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import time
 from json import dumps, loads
 import warnings
 from unittest import mock
 
 from webtest import TestApp
-from six import b as b_
-from six import u as u_
 import webob
 
 from pecan import Pecan, expose, abort, Request, Response
 from pecan.rest import RestController
 from pecan.hooks import PecanHook, HookController
 from pecan.tests import PecanTestCase
 
@@ -44,15 +42,15 @@
 
     def test_locals_are_not_used(self):
         with mock.patch('threading.local', side_effect=AssertionError()):
 
             app = TestApp(Pecan(self.root(), use_context_locals=False))
             r = app.get('/')
             assert r.status_int == 200
-            assert r.body == b_('Hello, World!')
+            assert r.body == b'Hello, World!'
 
             self.assertRaises(AssertionError, Pecan, self.root)
 
     def test_threadlocal_argument_warning(self):
         with mock.patch('threading.local', side_effect=AssertionError()):
 
             app = TestApp(Pecan(self.root(), use_context_locals=False))
@@ -95,41 +93,41 @@
                 return 'Hello, World!'
 
         return TestApp(Pecan(RootController(), use_context_locals=False))
 
     def test_empty_root(self):
         r = self.app_.get('/')
         assert r.status_int == 200
-        assert r.body == b_('Hello, World!')
+        assert r.body == b'Hello, World!'
 
     def test_index(self):
         r = self.app_.get('/index')
         assert r.status_int == 200
-        assert r.body == b_('Hello, World!')
+        assert r.body == b'Hello, World!'
 
     def test_index_html(self):
         r = self.app_.get('/index.html')
         assert r.status_int == 200
-        assert r.body == b_('Hello, World!')
+        assert r.body == b'Hello, World!'
 
 
 class TestManualResponse(PecanTestCase):
 
     def test_manual_response(self):
 
         class RootController(object):
             @expose()
             def index(self, req, resp):
                 resp = webob.Response(resp.environ)
-                resp.body = b_('Hello, World!')
+                resp.body = b'Hello, World!'
                 return resp
 
         app = TestApp(Pecan(RootController(), use_context_locals=False))
         r = app.get('/')
-        assert r.body == b_('Hello, World!'), r.body
+        assert r.body == b'Hello, World!', r.body
 
 
 class TestDispatch(PecanTestCase):
 
     @property
     def app_(self):
         class SubSubController(object):
@@ -176,39 +174,39 @@
             sub = SubController()
 
         return TestApp(Pecan(RootController(), use_context_locals=False))
 
     def test_index(self):
         r = self.app_.get('/')
         assert r.status_int == 200
-        assert r.body == b_('/')
+        assert r.body == b'/'
 
     def test_one_level(self):
         r = self.app_.get('/deeper')
         assert r.status_int == 200
-        assert r.body == b_('/deeper')
+        assert r.body == b'/deeper'
 
     def test_one_level_with_trailing(self):
         r = self.app_.get('/sub/')
         assert r.status_int == 200
-        assert r.body == b_('/sub/')
+        assert r.body == b'/sub/'
 
     def test_two_levels(self):
         r = self.app_.get('/sub/deeper')
         assert r.status_int == 200
-        assert r.body == b_('/sub/deeper')
+        assert r.body == b'/sub/deeper'
 
     def test_two_levels_with_trailing(self):
         r = self.app_.get('/sub/sub/')
         assert r.status_int == 200
 
     def test_three_levels(self):
         r = self.app_.get('/sub/sub/deeper')
         assert r.status_int == 200
-        assert r.body == b_('/sub/sub/deeper')
+        assert r.body == b'/sub/sub/deeper'
 
 
 class TestLookups(PecanTestCase):
 
     @property
     def app_(self):
         class LookupController(object):
@@ -233,25 +231,25 @@
                 return LookupController(someID), remainder
 
         return TestApp(Pecan(RootController(), use_context_locals=False))
 
     def test_index(self):
         r = self.app_.get('/')
         assert r.status_int == 200
-        assert r.body == b_('/')
+        assert r.body == b'/'
 
     def test_lookup(self):
         r = self.app_.get('/100/')
         assert r.status_int == 200
-        assert r.body == b_('/100')
+        assert r.body == b'/100'
 
     def test_lookup_with_method(self):
         r = self.app_.get('/100/name')
         assert r.status_int == 200
-        assert r.body == b_('/100/name')
+        assert r.body == b'/100/name'
 
     def test_lookup_with_wrong_argspec(self):
         class RootController(object):
             @expose()
             def _lookup(self, someID):
                 return 'Bad arg spec'  # pragma: nocover
 
@@ -284,15 +282,15 @@
 
         return TestApp(Pecan(RootController(), use_context_locals=False))
 
     def test_canonical_lookup(self):
         assert self.app_.get('/users', expect_errors=404).status_int == 404
         assert self.app_.get('/users/', expect_errors=404).status_int == 404
         assert self.app_.get('/users/100').status_int == 302
-        assert self.app_.get('/users/100/').body == b_('100')
+        assert self.app_.get('/users/100/').body == b'100'
 
 
 class TestControllerArguments(PecanTestCase):
 
     @property
     def app_(self):
         class RootController(object):
@@ -368,401 +366,401 @@
                     "index() missing 1 required positional argument: 'id'"
                 ),
             )  # this messaging changed in Python 3.3 and again in Python 3.10
 
     def test_single_argument(self):
         r = self.app_.get('/1')
         assert r.status_int == 200
-        assert r.body == b_('index: 1')
+        assert r.body == b'index: 1'
 
     def test_single_argument_with_encoded_url(self):
         r = self.app_.get('/This%20is%20a%20test%21')
         assert r.status_int == 200
-        assert r.body == b_('index: This is a test!')
+        assert r.body == b'index: This is a test!'
 
     def test_two_arguments(self):
         r = self.app_.get('/1/dummy', status=404)
         assert r.status_int == 404
 
     def test_keyword_argument(self):
         r = self.app_.get('/?id=2')
         assert r.status_int == 200
-        assert r.body == b_('index: 2')
+        assert r.body == b'index: 2'
 
     def test_keyword_argument_with_encoded_url(self):
         r = self.app_.get('/?id=This%20is%20a%20test%21')
         assert r.status_int == 200
-        assert r.body == b_('index: This is a test!')
+        assert r.body == b'index: This is a test!'
 
     def test_argument_and_keyword_argument(self):
         r = self.app_.get('/3?id=three')
         assert r.status_int == 200
-        assert r.body == b_('index: 3')
+        assert r.body == b'index: 3'
 
     def test_encoded_argument_and_keyword_argument(self):
         r = self.app_.get('/This%20is%20a%20test%21?id=three')
         assert r.status_int == 200
-        assert r.body == b_('index: This is a test!')
+        assert r.body == b'index: This is a test!'
 
     def test_explicit_kwargs(self):
         r = self.app_.post('/', {'id': '4'})
         assert r.status_int == 200
-        assert r.body == b_('index: 4')
+        assert r.body == b'index: 4'
 
     def test_path_with_explicit_kwargs(self):
         r = self.app_.post('/4', {'id': 'four'})
         assert r.status_int == 200
-        assert r.body == b_('index: 4')
+        assert r.body == b'index: 4'
 
     def test_multiple_kwargs(self):
         r = self.app_.get('/?id=5&dummy=dummy')
         assert r.status_int == 200
-        assert r.body == b_('index: 5')
+        assert r.body == b'index: 5'
 
     def test_kwargs_from_root(self):
         r = self.app_.post('/', {'id': '6', 'dummy': 'dummy'})
         assert r.status_int == 200
-        assert r.body == b_('index: 6')
+        assert r.body == b'index: 6'
 
         # multiple args
 
     def test_multiple_positional_arguments(self):
         r = self.app_.get('/multiple/one/two')
         assert r.status_int == 200
-        assert r.body == b_('multiple: one, two')
+        assert r.body == b'multiple: one, two'
 
     def test_multiple_positional_arguments_with_url_encode(self):
         r = self.app_.get('/multiple/One%20/Two%21')
         assert r.status_int == 200
-        assert r.body == b_('multiple: One , Two!')
+        assert r.body == b'multiple: One , Two!'
 
     def test_multiple_positional_arguments_with_kwargs(self):
         r = self.app_.get('/multiple?one=three&two=four')
         assert r.status_int == 200
-        assert r.body == b_('multiple: three, four')
+        assert r.body == b'multiple: three, four'
 
     def test_multiple_positional_arguments_with_url_encoded_kwargs(self):
         r = self.app_.get('/multiple?one=Three%20&two=Four%20%21')
         assert r.status_int == 200
-        assert r.body == b_('multiple: Three , Four !')
+        assert r.body == b'multiple: Three , Four !'
 
     def test_positional_args_with_dictionary_kwargs(self):
         r = self.app_.post('/multiple', {'one': 'five', 'two': 'six'})
         assert r.status_int == 200
-        assert r.body == b_('multiple: five, six')
+        assert r.body == b'multiple: five, six'
 
     def test_positional_args_with_url_encoded_dictionary_kwargs(self):
         r = self.app_.post('/multiple', {'one': 'Five%20', 'two': 'Six%20%21'})
         assert r.status_int == 200
-        assert r.body == b_('multiple: Five%20, Six%20%21')
+        assert r.body == b'multiple: Five%20, Six%20%21'
 
         # optional arg
     def test_optional_arg(self):
         r = self.app_.get('/optional')
         assert r.status_int == 200
-        assert r.body == b_('optional: None')
+        assert r.body == b'optional: None'
 
     def test_multiple_optional(self):
         r = self.app_.get('/optional/1')
         assert r.status_int == 200
-        assert r.body == b_('optional: 1')
+        assert r.body == b'optional: 1'
 
     def test_multiple_optional_url_encoded(self):
         r = self.app_.get('/optional/Some%20Number')
         assert r.status_int == 200
-        assert r.body == b_('optional: Some Number')
+        assert r.body == b'optional: Some Number'
 
     def test_multiple_optional_missing(self):
         r = self.app_.get('/optional/2/dummy', status=404)
         assert r.status_int == 404
 
     def test_multiple_with_kwargs(self):
         r = self.app_.get('/optional?id=2')
         assert r.status_int == 200
-        assert r.body == b_('optional: 2')
+        assert r.body == b'optional: 2'
 
     def test_multiple_with_url_encoded_kwargs(self):
         r = self.app_.get('/optional?id=Some%20Number')
         assert r.status_int == 200
-        assert r.body == b_('optional: Some Number')
+        assert r.body == b'optional: Some Number'
 
     def test_multiple_args_with_url_encoded_kwargs(self):
         r = self.app_.get('/optional/3?id=three')
         assert r.status_int == 200
-        assert r.body == b_('optional: 3')
+        assert r.body == b'optional: 3'
 
     def test_url_encoded_positional_args(self):
         r = self.app_.get('/optional/Some%20Number?id=three')
         assert r.status_int == 200
-        assert r.body == b_('optional: Some Number')
+        assert r.body == b'optional: Some Number'
 
     def test_optional_arg_with_kwargs(self):
         r = self.app_.post('/optional', {'id': '4'})
         assert r.status_int == 200
-        assert r.body == b_('optional: 4')
+        assert r.body == b'optional: 4'
 
     def test_optional_arg_with_url_encoded_kwargs(self):
         r = self.app_.post('/optional', {'id': 'Some%20Number'})
         assert r.status_int == 200
-        assert r.body == b_('optional: Some%20Number')
+        assert r.body == b'optional: Some%20Number'
 
     def test_multiple_positional_arguments_with_dictionary_kwargs(self):
         r = self.app_.post('/optional/5', {'id': 'five'})
         assert r.status_int == 200
-        assert r.body == b_('optional: 5')
+        assert r.body == b'optional: 5'
 
     def test_multiple_positional_url_encoded_arguments_with_kwargs(self):
         r = self.app_.post('/optional/Some%20Number', {'id': 'five'})
         assert r.status_int == 200
-        assert r.body == b_('optional: Some Number')
+        assert r.body == b'optional: Some Number'
 
     def test_optional_arg_with_multiple_kwargs(self):
         r = self.app_.get('/optional?id=6&dummy=dummy')
         assert r.status_int == 200
-        assert r.body == b_('optional: 6')
+        assert r.body == b'optional: 6'
 
     def test_optional_arg_with_multiple_url_encoded_kwargs(self):
         r = self.app_.get('/optional?id=Some%20Number&dummy=dummy')
         assert r.status_int == 200
-        assert r.body == b_('optional: Some Number')
+        assert r.body == b'optional: Some Number'
 
     def test_optional_arg_with_multiple_dictionary_kwargs(self):
         r = self.app_.post('/optional', {'id': '7', 'dummy': 'dummy'})
         assert r.status_int == 200
-        assert r.body == b_('optional: 7')
+        assert r.body == b'optional: 7'
 
     def test_optional_arg_with_multiple_url_encoded_dictionary_kwargs(self):
         r = self.app_.post('/optional', {
             'id': 'Some%20Number',
             'dummy': 'dummy'
         })
         assert r.status_int == 200
-        assert r.body == b_('optional: Some%20Number')
+        assert r.body == b'optional: Some%20Number'
 
         # multiple optional args
 
     def test_multiple_optional_positional_args(self):
         r = self.app_.get('/multiple_optional')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: None, None, None')
+        assert r.body == b'multiple_optional: None, None, None'
 
     def test_multiple_optional_positional_args_one_arg(self):
         r = self.app_.get('/multiple_optional/1')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: 1, None, None')
+        assert r.body == b'multiple_optional: 1, None, None'
 
     def test_multiple_optional_positional_args_one_url_encoded_arg(self):
         r = self.app_.get('/multiple_optional/One%21')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: One!, None, None')
+        assert r.body == b'multiple_optional: One!, None, None'
 
     def test_multiple_optional_positional_args_all_args(self):
         r = self.app_.get('/multiple_optional/1/2/3')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: 1, 2, 3')
+        assert r.body == b'multiple_optional: 1, 2, 3'
 
     def test_multiple_optional_positional_args_all_url_encoded_args(self):
         r = self.app_.get('/multiple_optional/One%21/Two%21/Three%21')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: One!, Two!, Three!')
+        assert r.body == b'multiple_optional: One!, Two!, Three!'
 
     def test_multiple_optional_positional_args_too_many_args(self):
         r = self.app_.get('/multiple_optional/1/2/3/dummy', status=404)
         assert r.status_int == 404
 
     def test_multiple_optional_positional_args_with_kwargs(self):
         r = self.app_.get('/multiple_optional?one=1')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: 1, None, None')
+        assert r.body == b'multiple_optional: 1, None, None'
 
     def test_multiple_optional_positional_args_with_url_encoded_kwargs(self):
         r = self.app_.get('/multiple_optional?one=One%21')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: One!, None, None')
+        assert r.body == b'multiple_optional: One!, None, None'
 
     def test_multiple_optional_positional_args_with_string_kwargs(self):
         r = self.app_.get('/multiple_optional/1?one=one')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: 1, None, None')
+        assert r.body == b'multiple_optional: 1, None, None'
 
     def test_multiple_optional_positional_args_with_encoded_str_kwargs(self):
         r = self.app_.get('/multiple_optional/One%21?one=one')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: One!, None, None')
+        assert r.body == b'multiple_optional: One!, None, None'
 
     def test_multiple_optional_positional_args_with_dict_kwargs(self):
         r = self.app_.post('/multiple_optional', {'one': '1'})
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: 1, None, None')
+        assert r.body == b'multiple_optional: 1, None, None'
 
     def test_multiple_optional_positional_args_with_encoded_dict_kwargs(self):
         r = self.app_.post('/multiple_optional', {'one': 'One%21'})
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: One%21, None, None')
+        assert r.body == b'multiple_optional: One%21, None, None'
 
     def test_multiple_optional_positional_args_and_dict_kwargs(self):
         r = self.app_.post('/multiple_optional/1', {'one': 'one'})
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: 1, None, None')
+        assert r.body == b'multiple_optional: 1, None, None'
 
     def test_multiple_optional_encoded_positional_args_and_dict_kwargs(self):
         r = self.app_.post('/multiple_optional/One%21', {'one': 'one'})
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: One!, None, None')
+        assert r.body == b'multiple_optional: One!, None, None'
 
     def test_multiple_optional_args_with_multiple_kwargs(self):
         r = self.app_.get('/multiple_optional?one=1&two=2&three=3&four=4')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: 1, 2, 3')
+        assert r.body == b'multiple_optional: 1, 2, 3'
 
     def test_multiple_optional_args_with_multiple_encoded_kwargs(self):
         r = self.app_.get(
             '/multiple_optional?one=One%21&two=Two%21&three=Three%21&four=4'
         )
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: One!, Two!, Three!')
+        assert r.body == b'multiple_optional: One!, Two!, Three!'
 
     def test_multiple_optional_args_with_multiple_dict_kwargs(self):
         r = self.app_.post(
             '/multiple_optional',
             {'one': '1', 'two': '2', 'three': '3', 'four': '4'}
         )
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: 1, 2, 3')
+        assert r.body == b'multiple_optional: 1, 2, 3'
 
     def test_multiple_optional_args_with_multiple_encoded_dict_kwargs(self):
         r = self.app_.post(
             '/multiple_optional',
             {
                 'one': 'One%21',
                 'two': 'Two%21',
                 'three': 'Three%21',
                 'four': '4'
             }
         )
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: One%21, Two%21, Three%21')
+        assert r.body == b'multiple_optional: One%21, Two%21, Three%21'
 
     def test_multiple_optional_args_with_last_kwarg(self):
         r = self.app_.get('/multiple_optional?three=3')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: None, None, 3')
+        assert r.body == b'multiple_optional: None, None, 3'
 
     def test_multiple_optional_args_with_last_encoded_kwarg(self):
         r = self.app_.get('/multiple_optional?three=Three%21')
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: None, None, Three!')
+        assert r.body == b'multiple_optional: None, None, Three!'
 
     def test_multiple_optional_args_with_middle_arg(self):
         r = self.app_.get('/multiple_optional', {'two': '2'})
         assert r.status_int == 200
-        assert r.body == b_('multiple_optional: None, 2, None')
+        assert r.body == b'multiple_optional: None, 2, None'
 
     def test_variable_args(self):
         r = self.app_.get('/variable_args')
         assert r.status_int == 200
-        assert r.body == b_('variable_args: ')
+        assert r.body == b'variable_args: '
 
     def test_multiple_variable_args(self):
         r = self.app_.get('/variable_args/1/dummy')
         assert r.status_int == 200
-        assert r.body == b_('variable_args: 1, dummy')
+        assert r.body == b'variable_args: 1, dummy'
 
     def test_multiple_encoded_variable_args(self):
         r = self.app_.get('/variable_args/Testing%20One%20Two/Three%21')
         assert r.status_int == 200
-        assert r.body == b_('variable_args: Testing One Two, Three!')
+        assert r.body == b'variable_args: Testing One Two, Three!'
 
     def test_variable_args_with_kwargs(self):
         r = self.app_.get('/variable_args?id=2&dummy=dummy')
         assert r.status_int == 200
-        assert r.body == b_('variable_args: ')
+        assert r.body == b'variable_args: '
 
     def test_variable_args_with_dict_kwargs(self):
         r = self.app_.post('/variable_args', {'id': '3', 'dummy': 'dummy'})
         assert r.status_int == 200
-        assert r.body == b_('variable_args: ')
+        assert r.body == b'variable_args: '
 
     def test_variable_kwargs(self):
         r = self.app_.get('/variable_kwargs')
         assert r.status_int == 200
-        assert r.body == b_('variable_kwargs: ')
+        assert r.body == b'variable_kwargs: '
 
     def test_multiple_variable_kwargs(self):
         r = self.app_.get('/variable_kwargs/1/dummy', status=404)
         assert r.status_int == 404
 
     def test_multiple_variable_kwargs_with_explicit_kwargs(self):
         r = self.app_.get('/variable_kwargs?id=2&dummy=dummy')
         assert r.status_int == 200
-        assert r.body == b_('variable_kwargs: dummy=dummy, id=2')
+        assert r.body == b'variable_kwargs: dummy=dummy, id=2'
 
     def test_multiple_variable_kwargs_with_explicit_encoded_kwargs(self):
         r = self.app_.get(
             '/variable_kwargs?id=Two%21&dummy=This%20is%20a%20test'
         )
         assert r.status_int == 200
-        assert r.body == b_('variable_kwargs: dummy=This is a test, id=Two!')
+        assert r.body == b'variable_kwargs: dummy=This is a test, id=Two!'
 
     def test_multiple_variable_kwargs_with_dict_kwargs(self):
         r = self.app_.post('/variable_kwargs', {'id': '3', 'dummy': 'dummy'})
         assert r.status_int == 200
-        assert r.body == b_('variable_kwargs: dummy=dummy, id=3')
+        assert r.body == b'variable_kwargs: dummy=dummy, id=3'
 
     def test_multiple_variable_kwargs_with_encoded_dict_kwargs(self):
         r = self.app_.post(
             '/variable_kwargs',
             {'id': 'Three%21', 'dummy': 'This%20is%20a%20test'}
         )
         assert r.status_int == 200
-        result = 'variable_kwargs: dummy=This%20is%20a%20test, id=Three%21'
-        assert r.body == b_(result)
+        result = b'variable_kwargs: dummy=This%20is%20a%20test, id=Three%21'
+        assert r.body == result
 
     def test_variable_all(self):
         r = self.app_.get('/variable_all')
         assert r.status_int == 200
-        assert r.body == b_('variable_all: ')
+        assert r.body == b'variable_all: '
 
     def test_variable_all_with_one_extra(self):
         r = self.app_.get('/variable_all/1')
         assert r.status_int == 200
-        assert r.body == b_('variable_all: 1')
+        assert r.body == b'variable_all: 1'
 
     def test_variable_all_with_two_extras(self):
         r = self.app_.get('/variable_all/2/dummy')
         assert r.status_int == 200
-        assert r.body == b_('variable_all: 2, dummy')
+        assert r.body == b'variable_all: 2, dummy'
 
     def test_variable_mixed(self):
         r = self.app_.get('/variable_all/3?month=1&day=12')
         assert r.status_int == 200
-        assert r.body == b_('variable_all: 3, day=12, month=1')
+        assert r.body == b'variable_all: 3, day=12, month=1'
 
     def test_variable_mixed_explicit(self):
         r = self.app_.get('/variable_all/4?id=four&month=1&day=12')
         assert r.status_int == 200
-        assert r.body == b_('variable_all: 4, day=12, id=four, month=1')
+        assert r.body == b'variable_all: 4, day=12, id=four, month=1'
 
     def test_variable_post(self):
         r = self.app_.post('/variable_all/5/dummy')
         assert r.status_int == 200
-        assert r.body == b_('variable_all: 5, dummy')
+        assert r.body == b'variable_all: 5, dummy'
 
     def test_variable_post_with_kwargs(self):
         r = self.app_.post('/variable_all/6', {'month': '1', 'day': '12'})
         assert r.status_int == 200
-        assert r.body == b_('variable_all: 6, day=12, month=1')
+        assert r.body == b'variable_all: 6, day=12, month=1'
 
     def test_variable_post_mixed(self):
         r = self.app_.post(
             '/variable_all/7',
             {'id': 'seven', 'month': '1', 'day': '12'}
         )
         assert r.status_int == 200
-        assert r.body == b_('variable_all: 7, day=12, id=seven, month=1')
+        assert r.body == b'variable_all: 7, day=12, id=seven, month=1'
 
     def test_no_remainder(self):
         try:
             r = self.app_.get('/eater')
             assert r.status_int != 200  # pragma: nocover
         except Exception as ex:
             assert type(ex) == TypeError
@@ -774,63 +772,63 @@
                     "eater() missing 1 required positional argument: 'id'"
                 ),
             )  # this messaging changed in Python 3.3 and again in Python 3.10
 
     def test_one_remainder(self):
         r = self.app_.get('/eater/1')
         assert r.status_int == 200
-        assert r.body == b_('eater: 1, None, ')
+        assert r.body == b'eater: 1, None, '
 
     def test_two_remainders(self):
         r = self.app_.get('/eater/2/dummy')
         assert r.status_int == 200
-        assert r.body == b_('eater: 2, dummy, ')
+        assert r.body == b'eater: 2, dummy, '
 
     def test_many_remainders(self):
         r = self.app_.get('/eater/3/dummy/foo/bar')
         assert r.status_int == 200
-        assert r.body == b_('eater: 3, dummy, foo, bar')
+        assert r.body == b'eater: 3, dummy, foo, bar'
 
     def test_remainder_with_kwargs(self):
         r = self.app_.get('/eater/4?month=1&day=12')
         assert r.status_int == 200
-        assert r.body == b_('eater: 4, None, day=12, month=1')
+        assert r.body == b'eater: 4, None, day=12, month=1'
 
     def test_remainder_with_many_kwargs(self):
         r = self.app_.get('/eater/5?id=five&month=1&day=12&dummy=dummy')
         assert r.status_int == 200
-        assert r.body == b_('eater: 5, dummy, day=12, month=1')
+        assert r.body == b'eater: 5, dummy, day=12, month=1'
 
     def test_post_remainder(self):
         r = self.app_.post('/eater/6')
         assert r.status_int == 200
-        assert r.body == b_('eater: 6, None, ')
+        assert r.body == b'eater: 6, None, '
 
     def test_post_three_remainders(self):
         r = self.app_.post('/eater/7/dummy')
         assert r.status_int == 200
-        assert r.body == b_('eater: 7, dummy, ')
+        assert r.body == b'eater: 7, dummy, '
 
     def test_post_many_remainders(self):
         r = self.app_.post('/eater/8/dummy/foo/bar')
         assert r.status_int == 200
-        assert r.body == b_('eater: 8, dummy, foo, bar')
+        assert r.body == b'eater: 8, dummy, foo, bar'
 
     def test_post_remainder_with_kwargs(self):
         r = self.app_.post('/eater/9', {'month': '1', 'day': '12'})
         assert r.status_int == 200
-        assert r.body == b_('eater: 9, None, day=12, month=1')
+        assert r.body == b'eater: 9, None, day=12, month=1'
 
     def test_post_many_remainders_with_many_kwargs(self):
         r = self.app_.post(
             '/eater/10',
             {'id': 'ten', 'month': '1', 'day': '12', 'dummy': 'dummy'}
         )
         assert r.status_int == 200
-        assert r.body == b_('eater: 10, dummy, day=12, month=1')
+        assert r.body == b'eater: 10, dummy, day=12, month=1'
 
 
 class TestRestController(PecanTestCase):
 
     @property
     def app_(self):
 
@@ -911,84 +909,86 @@
 
         # create the app
         return TestApp(Pecan(RootController(), use_context_locals=False))
 
     def test_get_all(self):
         r = self.app_.get('/things')
         assert r.status_int == 200
-        assert r.body == b_(dumps(dict(items=['zero', 'one', 'two', 'three'])))
+        assert r.body == dumps(
+            dict(items=['zero', 'one', 'two', 'three'])
+        ).encode('utf-8')
 
     def test_get_one(self):
-        for i, value in enumerate(['zero', 'one', 'two', 'three']):
+        for i, value in enumerate([b'zero', b'one', b'two', b'three']):
             r = self.app_.get('/things/%d' % i)
             assert r.status_int == 200
-            assert r.body == b_(value)
+            assert r.body == value
 
     def test_post(self):
         r = self.app_.post('/things', {'value': 'four'})
         assert r.status_int == 302
-        assert r.body == b_('CREATED')
+        assert r.body == b'CREATED'
 
     def test_custom_action(self):
         r = self.app_.get('/things/3/edit')
         assert r.status_int == 200
-        assert r.body == b_('EDIT three')
+        assert r.body == b'EDIT three'
 
     def test_put(self):
         r = self.app_.put('/things/3', {'value': 'THREE!'})
         assert r.status_int == 200
-        assert r.body == b_('UPDATED')
+        assert r.body == b'UPDATED'
 
     def test_put_with_method_parameter_and_get(self):
         r = self.app_.get('/things/3?_method=put', {'value': 'X'}, status=405)
         assert r.status_int == 405
 
     def test_put_with_method_parameter_and_post(self):
         r = self.app_.post('/things/3?_method=put', {'value': 'THREE!'})
         assert r.status_int == 200
-        assert r.body == b_('UPDATED')
+        assert r.body == b'UPDATED'
 
     def test_get_delete(self):
         r = self.app_.get('/things/3/delete')
         assert r.status_int == 200
-        assert r.body == b_('DELETE three')
+        assert r.body == b'DELETE three'
 
     def test_delete_method(self):
         r = self.app_.delete('/things/3')
         assert r.status_int == 200
-        assert r.body == b_('DELETED')
+        assert r.body == b'DELETED'
 
     def test_delete_with_method_parameter(self):
         r = self.app_.get('/things/3?_method=DELETE', status=405)
         assert r.status_int == 405
 
     def test_delete_with_method_parameter_and_post(self):
         r = self.app_.post('/things/3?_method=DELETE')
         assert r.status_int == 200
-        assert r.body == b_('DELETED')
+        assert r.body == b'DELETED'
 
     def test_custom_method_type(self):
         r = self.app_.request('/things', method='RESET')
         assert r.status_int == 200
-        assert r.body == b_('RESET')
+        assert r.body == b'RESET'
 
     def test_custom_method_type_with_method_parameter(self):
         r = self.app_.get('/things?_method=RESET')
         assert r.status_int == 200
-        assert r.body == b_('RESET')
+        assert r.body == b'RESET'
 
     def test_options(self):
         r = self.app_.request('/things', method='OPTIONS')
         assert r.status_int == 200
-        assert r.body == b_('OPTIONS')
+        assert r.body == b'OPTIONS'
 
     def test_options_with_method_parameter(self):
         r = self.app_.post('/things', {'_method': 'OPTIONS'})
         assert r.status_int == 200
-        assert r.body == b_('OPTIONS')
+        assert r.body == b'OPTIONS'
 
     def test_other_custom_action(self):
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             r = self.app_.request('/things/other', method='MISC', status=405)
             assert r.status_int == 405
 
@@ -997,15 +997,15 @@
         assert r.status_int == 405
 
     def test_nested_controller_with_trailing_slash(self):
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             r = self.app_.request('/things/others/', method='MISC')
             assert r.status_int == 200
-            assert r.body == b_('OTHERS')
+            assert r.body == b'OTHERS'
 
     def test_nested_controller_without_trailing_slash(self):
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             r = self.app_.request('/things/others', method='MISC', status=302)
             assert r.status_int == 302
 
@@ -1013,27 +1013,27 @@
         r = self.app_.get('/things?_method=BAD', status=405)
         assert r.status_int == 405
 
     def test_named_action(self):
         # test custom "GET" request "length"
         r = self.app_.get('/things/1/length')
         assert r.status_int == 200
-        assert r.body == b_(str(len('one')))
+        assert r.body == b'3'
 
     def test_named_nested_action(self):
         # test custom "GET" request through subcontroller
         r = self.app_.get('/things/others/echo?value=test')
         assert r.status_int == 200
-        assert r.body == b_('test')
+        assert r.body == b'test'
 
     def test_nested_post(self):
         # test custom "POST" request through subcontroller
         r = self.app_.post('/things/others/echo', {'value': 'test'})
         assert r.status_int == 200
-        assert r.body == b_('test')
+        assert r.body == b'test'
 
 
 class TestHooks(PecanTestCase):
 
     def test_basic_single_hook(self):
         run_hook = []
 
@@ -1059,15 +1059,15 @@
         app = TestApp(Pecan(
             RootController(),
             hooks=[SimpleHook()],
             use_context_locals=False
         ))
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
 
         assert len(run_hook) == 4
         assert run_hook[0] == 'on_route'
         assert run_hook[1] == 'before'
         assert run_hook[2] == 'inside'
         assert run_hook[3] == 'after'
 
@@ -1097,15 +1097,15 @@
                 run_hook.append('error' + self.id)
 
         app = TestApp(Pecan(RootController(), hooks=[
             SimpleHook(1), SimpleHook(2), SimpleHook(3)
         ], use_context_locals=False))
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
 
         assert len(run_hook) == 10
         assert run_hook[0] == 'on_route1'
         assert run_hook[1] == 'on_route2'
         assert run_hook[2] == 'on_route3'
         assert run_hook[3] == 'before1'
         assert run_hook[4] == 'before2'
@@ -1138,15 +1138,15 @@
 
         app = TestApp(Pecan(RootController(), hooks=[
             ErrorHook(), OnRouteHook()
         ], use_context_locals=False))
 
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello World!')
+        assert response.body == b'Hello World!'
 
         assert len(run_hook) == 2
         assert run_hook[0] == 'on_route'
         assert run_hook[1] == 'inside'
 
         run_hook = []
         try:
@@ -1167,15 +1167,15 @@
                 return [][1]
 
         class ErrorHook(PecanHook):
             def on_error(self, state, e):
                 run_hook.append('error')
 
                 r = webob.Response()
-                r.text = u_('on_error')
+                r.text = 'on_error'
 
                 return r
 
         app = TestApp(Pecan(RootController(), hooks=[
             ErrorHook()
         ], use_context_locals=False))
 
@@ -1214,15 +1214,15 @@
 
         papp = Pecan(RootController(), hooks=[
             SimpleHook(1, 3), SimpleHook(2, 2), SimpleHook(3, 1)
         ], use_context_locals=False)
         app = TestApp(papp)
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
 
         assert len(run_hook) == 10
         assert run_hook[0] == 'on_route3'
         assert run_hook[1] == 'on_route2'
         assert run_hook[2] == 'on_route1'
         assert run_hook[3] == 'before3'
         assert run_hook[4] == 'before2'
@@ -1271,34 +1271,34 @@
                 return 'Hello, World!'
 
             sub = SubController()
 
         app = TestApp(Pecan(RootController(), use_context_locals=False))
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
 
         assert len(run_hook) == 1
         assert run_hook[0] == 'inside'
 
         run_hook = []
 
         response = app.get('/sub/')
         assert response.status_int == 200
-        assert response.body == b_('Inside here!')
+        assert response.body == b'Inside here!'
 
         assert len(run_hook) == 3
         assert run_hook[0] == 'before'
         assert run_hook[1] == 'inside_sub'
         assert run_hook[2] == 'after'
 
         run_hook = []
         response = app.get('/sub/sub/')
         assert response.status_int == 200
-        assert response.body == b_('Deep inside here!')
+        assert response.body == b'Deep inside here!'
 
         assert len(run_hook) == 3
         assert run_hook[0] == 'before'
         assert run_hook[1] == 'inside_sub_sub'
         assert run_hook[2] == 'after'
 
     def test_isolated_hook_with_global_hook(self):
@@ -1339,27 +1339,27 @@
         app = TestApp(Pecan(
             RootController(),
             hooks=[SimpleHook(1)],
             use_context_locals=False
         ))
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
 
         assert len(run_hook) == 4
         assert run_hook[0] == 'on_route1'
         assert run_hook[1] == 'before1'
         assert run_hook[2] == 'inside'
         assert run_hook[3] == 'after1'
 
         run_hook = []
 
         response = app.get('/sub/')
         assert response.status_int == 200
-        assert response.body == b_('Inside here!')
+        assert response.body == b'Inside here!'
 
         assert len(run_hook) == 6
         assert run_hook[0] == 'on_route1'
         assert run_hook[1] == 'before2'
         assert run_hook[2] == 'before1'
         assert run_hook[3] == 'inside_sub'
         assert run_hook[4] == 'after1'
```

### Comparing `pecan-1.4.2/pecan/tests/test_rest.py` & `pecan-1.5.0/pecan/tests/test_rest.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from json import dumps, loads
 import unittest
 import struct
 import sys
 import warnings
 
-from six import b as b_, PY3
 from webtest import TestApp
 
 from pecan import abort, expose, make_app, response, redirect
 from pecan.rest import RestController
 from pecan.tests import PecanTestCase
 
 
@@ -103,75 +102,77 @@
 
         # create the app
         app = TestApp(make_app(RootController()))
 
         # test get_all
         r = app.get('/things')
         assert r.status_int == 200
-        assert r.body == b_(dumps(dict(items=ThingsController.data)))
+        assert r.body == dumps(
+            dict(items=ThingsController.data)
+        ).encode('utf-8')
 
         # test get_one
         for i, value in enumerate(ThingsController.data):
             r = app.get('/things/%d' % i)
             assert r.status_int == 200
-            assert r.body == b_(value)
+            assert r.body == value.encode('utf-8')
 
         # test post
         r = app.post('/things', {'value': 'four'})
         assert r.status_int == 302
-        assert r.body == b_('CREATED')
+        assert r.body == b'CREATED'
 
         # make sure it works
         r = app.get('/things/4')
         assert r.status_int == 200
-        assert r.body == b_('four')
+        assert r.body == b'four'
 
         # test edit
         r = app.get('/things/3/edit')
         assert r.status_int == 200
-        assert r.body == b_('EDIT three')
+        assert r.body == b'EDIT three'
 
         # test put
         r = app.put('/things/4', {'value': 'FOUR'})
         assert r.status_int == 200
-        assert r.body == b_('UPDATED')
+        assert r.body == b'UPDATED'
 
         # make sure it works
         r = app.get('/things/4')
         assert r.status_int == 200
-        assert r.body == b_('FOUR')
+        assert r.body == b'FOUR'
 
         # test put with _method parameter and GET
         r = app.get('/things/4?_method=put', {'value': 'FOUR!'}, status=405)
         assert r.status_int == 405
 
         # make sure it works
         r = app.get('/things/4')
         assert r.status_int == 200
-        assert r.body == b_('FOUR')
+        assert r.body == b'FOUR'
 
         # test put with _method parameter and POST
         r = app.post('/things/4?_method=put', {'value': 'FOUR!'})
         assert r.status_int == 200
-        assert r.body == b_('UPDATED')
+        assert r.body == b'UPDATED'
 
         # make sure it works
         r = app.get('/things/4')
         assert r.status_int == 200
-        assert r.body == b_('FOUR!')
+        assert r.body == b'FOUR!'
 
         # test get delete
         r = app.get('/things/4/delete')
         assert r.status_int == 200
-        assert r.body == b_('DELETE FOUR!')
+        assert r.body == b'DELETE FOUR!'
 
         # test delete
         r = app.delete('/things/4')
         assert r.status_int == 200
-        assert r.body == b_('DELETED')
+        assert r.body == b'DELETED'
 
         # make sure it works
         r = app.get('/things')
         assert r.status_int == 200
         assert len(loads(r.body.decode())['items']) == 4
 
         # test delete with _method parameter and GET
@@ -182,40 +183,40 @@
         r = app.get('/things')
         assert r.status_int == 200
         assert len(loads(r.body.decode())['items']) == 4
 
         # test delete with _method parameter and POST
         r = app.post('/things/3?_method=DELETE')
         assert r.status_int == 200
-        assert r.body == b_('DELETED')
+        assert r.body == b'DELETED'
 
         # make sure it works
         r = app.get('/things')
         assert r.status_int == 200
         assert len(loads(r.body.decode())['items']) == 3
 
         # test "RESET" custom action
         r = app.request('/things', method='RESET')
         assert r.status_int == 200
-        assert r.body == b_('RESET')
+        assert r.body == b'RESET'
 
         # test "RESET" custom action with _method parameter
         r = app.get('/things?_method=RESET')
         assert r.status_int == 200
-        assert r.body == b_('RESET')
+        assert r.body == b'RESET'
 
         # test the "OPTIONS" custom action
         r = app.request('/things', method='OPTIONS')
         assert r.status_int == 200
-        assert r.body == b_('OPTIONS')
+        assert r.body == b'OPTIONS'
 
         # test the "OPTIONS" custom action with the _method parameter
         r = app.post('/things', {'_method': 'OPTIONS'})
         assert r.status_int == 200
-        assert r.body == b_('OPTIONS')
+        assert r.body == b'OPTIONS'
 
         # test the "other" custom action
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             r = app.request('/things/other', method='MISC', status=405)
             assert r.status_int == 405
 
@@ -224,55 +225,55 @@
         assert r.status_int == 405
 
         # test the "others" custom action
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             r = app.request('/things/others/', method='MISC')
             assert r.status_int == 200
-            assert r.body == b_('OTHERS')
+            assert r.body == b'OTHERS'
 
         # test the "others" custom action missing trailing slash
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             r = app.request('/things/others', method='MISC', status=302)
             assert r.status_int == 302
 
         # test the "others" custom action with the _method parameter
         r = app.get('/things/others/?_method=MISC')
         assert r.status_int == 200
-        assert r.body == b_('OTHERS')
+        assert r.body == b'OTHERS'
 
         # test an invalid custom action
         r = app.get('/things?_method=BAD', status=405)
         assert r.status_int == 405
 
         # test custom "GET" request "count"
         r = app.get('/things/count')
         assert r.status_int == 200
-        assert r.body == b_('3')
+        assert r.body == b'3'
 
         # test custom "GET" request "length"
         r = app.get('/things/1/length')
         assert r.status_int == 200
-        assert r.body == b_(str(len('one')))
+        assert r.body == b'3'
 
         # test custom "GET" request through subcontroller
         r = app.get('/things/others/echo?value=test')
         assert r.status_int == 200
-        assert r.body == b_('test')
+        assert r.body == b'test'
 
         # test custom "POST" request "length"
         r = app.post('/things/1/length', {'value': 'test'})
         assert r.status_int == 200
-        assert r.body == b_(str(len('onetest')))
+        assert r.body == b'7'
 
         # test custom "POST" request through subcontroller
         r = app.post('/things/others/echo', {'value': 'test'})
         assert r.status_int == 200
-        assert r.body == b_('test')
+        assert r.body == b'test'
 
     def test_getall_with_trailing_slash(self):
 
         class ThingsController(RestController):
 
             data = ['zero', 'one', 'two', 'three']
 
@@ -285,15 +286,17 @@
 
         # create the app
         app = TestApp(make_app(RootController()))
 
         # test get_all
         r = app.get('/things/')
         assert r.status_int == 200
-        assert r.body == b_(dumps(dict(items=ThingsController.data)))
+        assert r.body == dumps(
+            dict(items=ThingsController.data)
+        ).encode('utf-8')
 
     def test_405_with_lookup(self):
 
         class LookupController(RestController):
 
             def __init__(self, _id):
                 self._id = _id
@@ -317,15 +320,15 @@
         # these should 405
         for path in ('/things', '/things/'):
             r = app.get(path, expect_errors=True)
             assert r.status_int == 405
 
         r = app.get('/things/foo')
         assert r.status_int == 200
-        assert r.body == b_('ID: foo')
+        assert r.body == b'ID: foo'
 
     def test_getall_with_lookup(self):
 
         class LookupController(RestController):
 
             def __init__(self, _id):
                 self._id = _id
@@ -352,19 +355,21 @@
         # create the app
         app = TestApp(make_app(RootController()))
 
         # test get_all
         for path in ('/things', '/things/'):
             r = app.get(path)
             assert r.status_int == 200
-            assert r.body == b_(dumps(dict(items=ThingsController.data)))
+            assert r.body == dumps(
+                dict(items=ThingsController.data)
+            ).encode('utf-8')
 
         r = app.get('/things/foo')
         assert r.status_int == 200
-        assert r.body == b_('ID: foo')
+        assert r.body == b'ID: foo'
 
     def test_simple_nested_rest(self):
 
         class BarController(RestController):
 
             @expose()
             def post(self):
@@ -390,27 +395,27 @@
             foo = FooController()
 
         # create the app
         app = TestApp(make_app(RootController()))
 
         r = app.post('/foo')
         assert r.status_int == 200
-        assert r.body == b_("FOO-POST")
+        assert r.body == b"FOO-POST"
 
         r = app.delete('/foo/1')
         assert r.status_int == 200
-        assert r.body == b_("FOO-1")
+        assert r.body == b"FOO-1"
 
         r = app.post('/foo/bar')
         assert r.status_int == 200
-        assert r.body == b_("BAR-POST")
+        assert r.body == b"BAR-POST"
 
         r = app.delete('/foo/bar/2')
         assert r.status_int == 200
-        assert r.body == b_("BAR-2")
+        assert r.body == b"BAR-2"
 
     def test_complicated_nested_rest(self):
 
         class BarsController(RestController):
 
             data = [['zero-zero', 'zero-one'], ['one-zero', 'one-one']]
 
@@ -500,149 +505,153 @@
 
         # create the app
         app = TestApp(make_app(RootController()))
 
         # test get_all
         r = app.get('/foos')
         assert r.status_int == 200
-        assert r.body == b_(dumps(dict(items=FoosController.data)))
+        assert r.body == dumps(
+            dict(items=FoosController.data)
+        ).encode('utf-8')
 
         # test nested get_all
         r = app.get('/foos/1/bars')
         assert r.status_int == 200
-        assert r.body == b_(dumps(dict(items=BarsController.data[1])))
+        assert r.body == dumps(
+            dict(items=BarsController.data[1])
+        ).encode('utf-8')
 
         # test get_one
         for i, value in enumerate(FoosController.data):
             r = app.get('/foos/%d' % i)
             assert r.status_int == 200
-            assert r.body == b_(value)
+            assert r.body == value.encode('utf-8')
 
         # test nested get_one
         for i, value in enumerate(FoosController.data):
             for j, value in enumerate(BarsController.data[i]):
                 r = app.get('/foos/%s/bars/%s' % (i, j))
                 assert r.status_int == 200
-                assert r.body == b_(value)
+                assert r.body == value.encode('utf-8')
 
         # test post
         r = app.post('/foos', {'value': 'two'})
         assert r.status_int == 302
-        assert r.body == b_('CREATED')
+        assert r.body == b'CREATED'
 
         # make sure it works
         r = app.get('/foos/2')
         assert r.status_int == 200
-        assert r.body == b_('two')
+        assert r.body == b'two'
 
         # test nested post
         r = app.post('/foos/2/bars', {'value': 'two-zero'})
         assert r.status_int == 302
-        assert r.body == b_('CREATED FOR 2')
+        assert r.body == b'CREATED FOR 2'
 
         # make sure it works
         r = app.get('/foos/2/bars/0')
         assert r.status_int == 200
-        assert r.body == b_('two-zero')
+        assert r.body == b'two-zero'
 
         # test edit
         r = app.get('/foos/1/edit')
         assert r.status_int == 200
-        assert r.body == b_('EDIT one')
+        assert r.body == b'EDIT one'
 
         # test nested edit
         r = app.get('/foos/1/bars/1/edit')
         assert r.status_int == 200
-        assert r.body == b_('EDIT one-one')
+        assert r.body == b'EDIT one-one'
 
         # test put
         r = app.put('/foos/2', {'value': 'TWO'})
         assert r.status_int == 200
-        assert r.body == b_('UPDATED')
+        assert r.body == b'UPDATED'
 
         # make sure it works
         r = app.get('/foos/2')
         assert r.status_int == 200
-        assert r.body == b_('TWO')
+        assert r.body == b'TWO'
 
         # test nested put
         r = app.put('/foos/2/bars/0', {'value': 'TWO-ZERO'})
         assert r.status_int == 200
-        assert r.body == b_('UPDATED')
+        assert r.body == b'UPDATED'
 
         # make sure it works
         r = app.get('/foos/2/bars/0')
         assert r.status_int == 200
-        assert r.body == b_('TWO-ZERO')
+        assert r.body == b'TWO-ZERO'
 
         # test put with _method parameter and GET
         r = app.get('/foos/2?_method=put', {'value': 'TWO!'}, status=405)
         assert r.status_int == 405
 
         # make sure it works
         r = app.get('/foos/2')
         assert r.status_int == 200
-        assert r.body == b_('TWO')
+        assert r.body == b'TWO'
 
         # test nested put with _method parameter and GET
         r = app.get(
             '/foos/2/bars/0?_method=put',
             {'value': 'ZERO-TWO!'}, status=405
         )
         assert r.status_int == 405
 
         # make sure it works
         r = app.get('/foos/2/bars/0')
         assert r.status_int == 200
-        assert r.body == b_('TWO-ZERO')
+        assert r.body == b'TWO-ZERO'
 
         # test put with _method parameter and POST
         r = app.post('/foos/2?_method=put', {'value': 'TWO!'})
         assert r.status_int == 200
-        assert r.body == b_('UPDATED')
+        assert r.body == b'UPDATED'
 
         # make sure it works
         r = app.get('/foos/2')
         assert r.status_int == 200
-        assert r.body == b_('TWO!')
+        assert r.body == b'TWO!'
 
         # test nested put with _method parameter and POST
         r = app.post('/foos/2/bars/0?_method=put', {'value': 'TWO-ZERO!'})
         assert r.status_int == 200
-        assert r.body == b_('UPDATED')
+        assert r.body == b'UPDATED'
 
         # make sure it works
         r = app.get('/foos/2/bars/0')
         assert r.status_int == 200
-        assert r.body == b_('TWO-ZERO!')
+        assert r.body == b'TWO-ZERO!'
 
         # test get delete
         r = app.get('/foos/2/delete')
         assert r.status_int == 200
-        assert r.body == b_('DELETE TWO!')
+        assert r.body == b'DELETE TWO!'
 
         # test nested get delete
         r = app.get('/foos/2/bars/0/delete')
         assert r.status_int == 200
-        assert r.body == b_('DELETE TWO-ZERO!')
+        assert r.body == b'DELETE TWO-ZERO!'
 
         # test nested delete
         r = app.delete('/foos/2/bars/0')
         assert r.status_int == 200
-        assert r.body == b_('DELETED')
+        assert r.body == b'DELETED'
 
         # make sure it works
         r = app.get('/foos/2/bars')
         assert r.status_int == 200
         assert len(loads(r.body.decode())['items']) == 0
 
         # test delete
         r = app.delete('/foos/2')
         assert r.status_int == 200
-        assert r.body == b_('DELETED')
+        assert r.body == b'DELETED'
 
         # make sure it works
         r = app.get('/foos')
         assert r.status_int == 200
         assert len(loads(r.body.decode())['items']) == 2
 
         # test nested delete with _method parameter and GET
@@ -662,25 +671,25 @@
         r = app.get('/foos')
         assert r.status_int == 200
         assert len(loads(r.body.decode())['items']) == 2
 
         # test nested delete with _method parameter and POST
         r = app.post('/foos/1/bars/1?_method=DELETE')
         assert r.status_int == 200
-        assert r.body == b_('DELETED')
+        assert r.body == b'DELETED'
 
         # make sure it works
         r = app.get('/foos/1/bars')
         assert r.status_int == 200
         assert len(loads(r.body.decode())['items']) == 1
 
         # test delete with _method parameter and POST
         r = app.post('/foos/1?_method=DELETE')
         assert r.status_int == 200
-        assert r.body == b_('DELETED')
+        assert r.body == b'DELETED'
 
         # make sure it works
         r = app.get('/foos')
         assert r.status_int == 200
         assert len(loads(r.body.decode())['items']) == 1
 
     def test_nested_get_all(self):
@@ -711,27 +720,27 @@
             foos = FoosController()
 
         # create the app
         app = TestApp(make_app(RootController()))
 
         r = app.get('/foos/')
         assert r.status_int == 200
-        assert r.body == b_('1')
+        assert r.body == b'1'
 
         r = app.get('/foos/1/')
         assert r.status_int == 200
-        assert r.body == b_('2')
+        assert r.body == b'2'
 
         r = app.get('/foos/1/bars/')
         assert r.status_int == 200
-        assert r.body == b_('3')
+        assert r.body == b'3'
 
         r = app.get('/foos/1/bars/2/')
         assert r.status_int == 200
-        assert r.body == b_('4')
+        assert r.body == b'4'
 
         r = app.get('/foos/bars/', status=404)
         assert r.status_int == 404
 
         r = app.get('/foos/bars/1', status=404)
         assert r.status_int == 404
 
@@ -767,27 +776,27 @@
             foos = FoosController()
 
         # create the app
         app = TestApp(make_app(RootController()))
 
         r = app.get('/foos/')
         assert r.status_int == 200
-        assert r.body == b_('1')
+        assert r.body == b'1'
 
         r = app.get('/foos/1/')
         assert r.status_int == 200
-        assert r.body == b_('2')
+        assert r.body == b'2'
 
         r = app.get('/foos/1/bars/')
         assert r.status_int == 200
-        assert r.body == b_('3')
+        assert r.body == b'3'
 
         r = app.get('/foos/1/bars/2/')
         assert r.status_int == 200
-        assert r.body == b_('4')
+        assert r.body == b'4'
 
         r = app.get('/foos/bars/')
         assert r.status_int == 302
         assert r.headers['Location'].endswith('/lookup-hit/')
 
         r = app.get('/foos/bars/1')
         assert r.status_int == 302
@@ -882,20 +891,24 @@
 
         # create the app
         app = TestApp(make_app(RootController()))
 
         # test get_all
         r = app.get('/foos')
         self.assertEqual(r.status_int, 200)
-        self.assertEqual(r.body, b_(dumps(dict(items=FoosController.data))))
+        self.assertEqual(r.body, dumps(
+            dict(items=FoosController.data)
+        ).encode('utf-8'))
 
         # test nested get_all
         r = app.get('/foos/1/bars')
         self.assertEqual(r.status_int, 200)
-        self.assertEqual(r.body, b_(dumps(dict(items=BarsController.data[1]))))
+        self.assertEqual(r.body, dumps(
+            dict(items=BarsController.data[1])
+        ).encode('utf-8'))
 
         r = app.get('/foos/bars', expect_errors=True)
         self.assertEqual(r.status_int, 404)
 
     def test_custom_with_trailing_slash(self):
 
         class CustomController(RestController):
@@ -923,43 +936,43 @@
             def remove(self, id):
                 return id
 
         app = TestApp(make_app(CustomController()))
 
         r = app.get('/detail')
         assert r.status_int == 200
-        assert r.body == b_('DETAIL')
+        assert r.body == b'DETAIL'
 
         r = app.get('/detail/')
         assert r.status_int == 200
-        assert r.body == b_('DETAIL')
+        assert r.body == b'DETAIL'
 
         r = app.post('/create')
         assert r.status_int == 200
-        assert r.body == b_('CREATE')
+        assert r.body == b'CREATE'
 
         r = app.post('/create/')
         assert r.status_int == 200
-        assert r.body == b_('CREATE')
+        assert r.body == b'CREATE'
 
         r = app.put('/update/123')
         assert r.status_int == 200
-        assert r.body == b_('123')
+        assert r.body == b'123'
 
         r = app.put('/update/123/')
         assert r.status_int == 200
-        assert r.body == b_('123')
+        assert r.body == b'123'
 
         r = app.delete('/remove/456')
         assert r.status_int == 200
-        assert r.body == b_('456')
+        assert r.body == b'456'
 
         r = app.delete('/remove/456/')
         assert r.status_int == 200
-        assert r.body == b_('456')
+        assert r.body == b'456'
 
     def test_custom_delete(self):
 
         class OthersController(object):
 
             @expose()
             def index(self):
@@ -994,38 +1007,38 @@
         # test bad delete with _method parameter and POST
         r = app.post('/things/delete_fail', {'_method': 'delete'}, status=405)
         assert r.status_int == 405
 
         # test custom delete without ID
         r = app.delete('/things/others/')
         assert r.status_int == 200
-        assert r.body == b_('DELETE')
+        assert r.body == b'DELETE'
 
         # test custom delete without ID with _method parameter and GET
         r = app.get('/things/others/?_method=delete', status=405)
         assert r.status_int == 405
 
         # test custom delete without ID with _method parameter and POST
         r = app.post('/things/others/', {'_method': 'delete'})
         assert r.status_int == 200
-        assert r.body == b_('DELETE')
+        assert r.body == b'DELETE'
 
         # test custom delete with ID
         r = app.delete('/things/others/reset/1')
         assert r.status_int == 200
-        assert r.body == b_('1')
+        assert r.body == b'1'
 
         # test custom delete with ID with _method parameter and GET
         r = app.get('/things/others/reset/1?_method=delete', status=405)
         assert r.status_int == 405
 
         # test custom delete with ID with _method parameter and POST
         r = app.post('/things/others/reset/1', {'_method': 'delete'})
         assert r.status_int == 200
-        assert r.body == b_('1')
+        assert r.body == b'1'
 
     def test_get_with_var_args(self):
 
         class OthersController(object):
 
             @expose()
             def index(self, one, two, three):
@@ -1044,20 +1057,20 @@
 
         # create the app
         app = TestApp(make_app(RootController()))
 
         # test get request
         r = app.get('/things/one/two/three')
         assert r.status_int == 200
-        assert r.body == b_('one, two, three')
+        assert r.body == b'one, two, three'
 
         # test nested get request
         r = app.get('/things/one/two/three/others/')
         assert r.status_int == 200
-        assert r.body == b_('NESTED: one, two, three')
+        assert r.body == b'NESTED: one, two, three'
 
     def test_sub_nested_rest(self):
 
         class BazsController(RestController):
 
             data = [[['zero-zero-zero']]]
 
@@ -1090,15 +1103,15 @@
 
         # create the app
         app = TestApp(make_app(RootController()))
 
         # test sub-nested get_one
         r = app.get('/foos/0/bars/0/bazs/0')
         assert r.status_int == 200
-        assert r.body == b_('zero-zero-zero')
+        assert r.body == b'zero-zero-zero'
 
     def test_sub_nested_rest_with_overwrites(self):
 
         class FinalController(object):
 
             @expose()
             def index(self):
@@ -1166,43 +1179,43 @@
             foos = FoosController()
 
         # create the app
         app = TestApp(make_app(RootController()))
 
         r = app.post('/foos')
         assert r.status_int == 200
-        assert r.body == b_('POST')
+        assert r.body == b'POST'
 
         r = app.put('/foos/0')
         assert r.status_int == 200
-        assert r.body == b_('PUT')
+        assert r.body == b'PUT'
 
         r = app.post('/foos/bars')
         assert r.status_int == 200
-        assert r.body == b_('POST-CHILD')
+        assert r.body == b'POST-CHILD'
 
         r = app.put('/foos/bars/0')
         assert r.status_int == 200
-        assert r.body == b_('PUT-CHILD')
+        assert r.body == b'PUT-CHILD'
 
         r = app.post('/foos/bars/bazs')
         assert r.status_int == 200
-        assert r.body == b_('POST-GRAND-CHILD')
+        assert r.body == b'POST-GRAND-CHILD'
 
         r = app.put('/foos/bars/bazs/0')
         assert r.status_int == 200
-        assert r.body == b_('PUT-GRAND-CHILD')
+        assert r.body == b'PUT-GRAND-CHILD'
 
         r = app.get('/foos/bars/bazs/final/')
         assert r.status_int == 200
-        assert r.body == b_('FINAL')
+        assert r.body == b'FINAL'
 
         r = app.get('/foos/bars/bazs/final/named')
         assert r.status_int == 200
-        assert r.body == b_('NAMED')
+        assert r.body == b'NAMED'
 
     def test_post_with_kwargs_only(self):
 
         class RootController(RestController):
 
             @expose()
             def get_all(self):
@@ -1213,15 +1226,15 @@
                 return kw
 
         # create the app
         app = TestApp(make_app(RootController()))
 
         r = app.get('/')
         assert r.status_int == 200
-        assert r.body == b_('INDEX')
+        assert r.body == b'INDEX'
 
         kwargs = {'foo': 'bar', 'spam': 'eggs'}
         r = app.post('/', kwargs)
         assert r.status_int == 200
         assert r.namespace['foo'] == 'bar'
         assert r.namespace['spam'] == 'eggs'
 
@@ -1302,51 +1315,51 @@
         class RootController(RestController):
             foo = FooController()
 
         app = TestApp(make_app(RootController()))
 
         r = app.get('/foo')
         assert r.status_int == 200
-        assert r.body == b_('INDEX')
+        assert r.body == b'INDEX'
 
         r = app.post('/foo')
         assert r.status_int == 200
-        assert r.body == b_('POST')
+        assert r.body == b'POST'
 
         r = app.get('/foo/1')
         assert r.status_int == 200
-        assert r.body == b_('GET ONE')
+        assert r.body == b'GET ONE'
 
         r = app.post('/foo/1')
         assert r.status_int == 200
-        assert r.body == b_('POST-LOOKUP-1')
+        assert r.body == b'POST-LOOKUP-1'
 
         r = app.put('/foo/1')
         assert r.status_int == 200
-        assert r.body == b_('PUT-1')
+        assert r.body == b'PUT-1'
 
         r = app.delete('/foo/1')
         assert r.status_int == 200
-        assert r.body == b_('DELETE-1')
+        assert r.body == b'DELETE-1'
 
         r = app.put('/foo/1/2')
         assert r.status_int == 200
-        assert r.body == b_('PUT-LOOKUP-1-2')
+        assert r.body == b'PUT-LOOKUP-1-2'
 
         r = app.delete('/foo/1/2')
         assert r.status_int == 200
-        assert r.body == b_('DELETE-LOOKUP-1-2')
+        assert r.body == b'DELETE-LOOKUP-1-2'
 
         r = app.get('/foo/1/2')
         assert r.status_int == 200
-        assert r.body == b_('FINAL-2')
+        assert r.body == b'FINAL-2'
 
         r = app.post('/foo/1/2')
         assert r.status_int == 200
-        assert r.body == b_('POST-2')
+        assert r.body == b'POST-2'
 
     def test_nested_rest_with_default(self):
 
         class FooController(RestController):
 
             @expose()
             def _default(self, *remainder):
@@ -1355,36 +1368,15 @@
         class RootController(RestController):
             foo = FooController()
 
         app = TestApp(make_app(RootController()))
 
         r = app.get('/foo/missing')
         assert r.status_int == 200
-        assert r.body == b_("DEFAULT missing")
-
-    def test_rest_with_non_utf_8_body(self):
-        if PY3:
-            # webob+PY3 doesn't suffer from this bug; the POST parsing in PY3
-            # seems to more gracefully detect the bytestring
-            return
-
-        class FooController(RestController):
-
-            @expose()
-            def post(self):
-                return "POST"
-
-        class RootController(RestController):
-            foo = FooController()
-
-        app = TestApp(make_app(RootController()))
-
-        data = struct.pack('255h', *range(0, 255))
-        r = app.post('/foo/', data, expect_errors=True)
-        assert r.status_int == 400
+        assert r.body == b"DEFAULT missing"
 
     def test_dynamic_rest_lookup(self):
         class BarController(RestController):
             @expose()
             def get_all(self):
                 return "BAR"
 
@@ -1440,51 +1432,51 @@
         class RootController(RestController):
             foos = FoosController()
 
         app = TestApp(make_app(RootController()))
 
         r = app.get('/foos')
         assert r.status_int == 200
-        assert r.body == b_('FOOS')
+        assert r.body == b'FOOS'
 
         r = app.post('/foos')
         assert r.status_int == 200
-        assert r.body == b_('POST_FOOS')
+        assert r.body == b'POST_FOOS'
 
         r = app.get('/foos/foo')
         assert r.status_int == 200
-        assert r.body == b_('FOO')
+        assert r.body == b'FOO'
 
         r = app.put('/foos/foo')
         assert r.status_int == 200
-        assert r.body == b_('PUT_FOO')
+        assert r.body == b'PUT_FOO'
 
         r = app.delete('/foos/foo')
         assert r.status_int == 200
-        assert r.body == b_('DELETE_FOO')
+        assert r.body == b'DELETE_FOO'
 
         r = app.get('/foos/foo/bars')
         assert r.status_int == 200
-        assert r.body == b_('BARS')
+        assert r.body == b'BARS'
 
         r = app.post('/foos/foo/bars')
         assert r.status_int == 200
-        assert r.body == b_('POST_BARS')
+        assert r.body == b'POST_BARS'
 
         r = app.get('/foos/foo/bars/bar')
         assert r.status_int == 200
-        assert r.body == b_('BAR')
+        assert r.body == b'BAR'
 
         r = app.put('/foos/foo/bars/bar')
         assert r.status_int == 200
-        assert r.body == b_('PUT_BAR')
+        assert r.body == b'PUT_BAR'
 
         r = app.delete('/foos/foo/bars/bar')
         assert r.status_int == 200
-        assert r.body == b_('DELETE_BAR')
+        assert r.body == b'DELETE_BAR'
 
     def test_method_not_allowed_get(self):
         class ThingsController(RestController):
 
             @expose()
             def put(self, id_, value):
                 response.status = 200
@@ -1550,15 +1542,15 @@
         assert r.status_int == 405
         assert r.headers['Allow'] == 'GET'
 
     @unittest.skipIf(sys.maxunicode <= 65536, 'narrow python build with UCS-2')
     def test_rest_with_utf8_uri(self):
 
         class FooController(RestController):
-            key = chr(0x1F330) if PY3 else unichr(0x1F330)
+            key = chr(0x1F330)
             data = {key: 'Success!'}
 
             @expose()
             def get_one(self, id_):
                 return self.data[id_]
 
             @expose()
@@ -1590,15 +1582,14 @@
         assert r.status_int == 200
         assert r.body == b'Success!'
 
         r = app.get('/foo/')
         assert r.status_int == 200
         assert r.body == b'Hello, World!'
 
-    @unittest.skipIf(not PY3, "test is Python3 specific")
     def test_rest_with_utf8_endpoint(self):
         class ChildController(object):
             @expose()
             def index(self):
                 return 'Hello, World!'
 
         class FooController(RestController):
```

### Comparing `pecan-1.4.2/pecan/tests/test_scaffolds.py` & `pecan-1.5.0/pecan/tests/test_scaffolds.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import shutil
 import sys
 import tempfile
 import unittest
-
-from six.moves import cStringIO as StringIO
+from io import StringIO
 
 from pecan.tests import PecanTestCase
 
 
 class TestPecanScaffold(PecanTestCase):
 
     def test_normalize_pkg_name(self):
```

### Comparing `pecan-1.4.2/pecan/tests/test_secure.py` & `pecan-1.5.0/pecan/tests/test_secure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import sys
 import unittest
 
-from six import b as b_
 from webtest import TestApp
 
 from pecan import expose, make_app
 from pecan.secure import secure, unlocked, SecureController
 from pecan.tests import PecanTestCase
 
 try:
@@ -52,29 +51,29 @@
         app = TestApp(make_app(
             RootController(),
             debug=True,
             static_root='tests/static'
         ))
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
 
         response = app.get('/unlocked')
         assert response.status_int == 200
-        assert response.body == b_('Sure thing')
+        assert response.body == b'Sure thing'
 
         response = app.get('/locked', expect_errors=True)
         assert response.status_int == 401
 
         response = app.get('/secret/', expect_errors=True)
         assert response.status_int == 401
 
         response = app.get('/secret/allowed')
         assert response.status_int == 200
-        assert response.body == b_('Allowed!')
+        assert response.body == b'Allowed!'
 
     def test_unlocked_attribute(self):
         class AuthorizedSubController(object):
             @expose()
             def index(self):
                 return 'Index'
 
@@ -114,37 +113,37 @@
         app = TestApp(make_app(
             RootController(),
             debug=True,
             static_root='tests/static'
         ))
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello, World!')
+        assert response.body == b'Hello, World!'
 
         response = app.get('/unlocked')
         assert response.status_int == 200
-        assert response.body == b_('Sure thing')
+        assert response.body == b'Sure thing'
 
         response = app.get('/locked', expect_errors=True)
         assert response.status_int == 401
 
         response = app.get('/secret/', expect_errors=True)
         assert response.status_int == 401
 
         response = app.get('/secret/allowed')
         assert response.status_int == 200
-        assert response.body == b_('Allowed!')
+        assert response.body == b'Allowed!'
 
         response = app.get('/secret/authorized/')
         assert response.status_int == 200
-        assert response.body == b_('Index')
+        assert response.body == b'Index'
 
         response = app.get('/secret/authorized/allowed')
         assert response.status_int == 200
-        assert response.body == b_('Allowed!')
+        assert response.body == b'Allowed!'
 
     def test_secure_attribute(self):
         authorized = False
 
         class SubController(object):
             @expose()
             def index(self):
@@ -156,23 +155,23 @@
                 return 'Hello from root!'
 
             sub = secure(SubController(), lambda: authorized)
 
         app = TestApp(make_app(RootController()))
         response = app.get('/')
         assert response.status_int == 200
-        assert response.body == b_('Hello from root!')
+        assert response.body == b'Hello from root!'
 
         response = app.get('/sub/', expect_errors=True)
         assert response.status_int == 401
 
         authorized = True
         response = app.get('/sub/')
         assert response.status_int == 200
-        assert response.body == b_('Hello from sub!')
+        assert response.body == b'Hello from sub!'
 
     def test_secured_generic_controller(self):
         authorized = False
 
         class RootController(object):
 
             @classmethod
@@ -409,24 +408,24 @@
         self.permissions_checked.clear()
         self.secret_cls.authorized = False
         self.deepsecret_cls.authorized = False
 
     def test_sub_of_both_not_secret(self):
         response = self.app.get('/notsecret/hi/')
         assert response.status_int == 200
-        assert response.body == b_('Index hi')
+        assert response.body == b'Index hi'
 
     def test_protected_lookup(self):
         response = self.app.get('/secret/hi/', expect_errors=True)
         assert response.status_int == 401
 
         self.secret_cls.authorized = True
         response = self.app.get('/secret/hi/')
         assert response.status_int == 200
-        assert response.body == b_('Index hi')
+        assert response.body == b'Index hi'
         assert 'secretcontroller' in self.permissions_checked
 
     def test_secured_notfound_lookup(self):
         response = self.app.get('/secret/notfound/', expect_errors=True)
         assert response.status_int == 404
 
     def test_secret_through_lookup(self):
@@ -445,31 +444,31 @@
         assert response.status_int == 401
         assert 'secretcontroller' in self.permissions_checked
         assert 'deepsecret' in self.permissions_checked
 
         self.deepsecret_cls.authorized = True
         response = self.app.get('/secret/hi/deepsecret/')
         assert response.status_int == 200
-        assert response.body == b_('Deep Secret')
+        assert response.body == b'Deep Secret'
         assert 'secretcontroller' in self.permissions_checked
         assert 'deepsecret' in self.permissions_checked
 
     def test_cyclical_protection(self):
         self.secret_cls.authorized = True
         self.deepsecret_cls.authorized = True
         response = self.app.get('/secret/1/deepsecret/2/deepsecret/')
         assert response.status_int == 200
-        assert response.body == b_('Deep Secret')
+        assert response.body == b'Deep Secret'
         assert 'secretcontroller' in self.permissions_checked
         assert 'deepsecret' in self.permissions_checked
 
     def test_unlocked_lookup(self):
         response = self.app.get('/notsecret/1/deepsecret/2/')
         assert response.status_int == 200
-        assert response.body == b_('Index 2')
+        assert response.body == b'Index 2'
         assert 'deepsecret' not in self.permissions_checked
 
         response = self.app.get(
             '/notsecret/1/deepsecret/notfound/', expect_errors=True
         )
         assert response.status_int == 404
         assert 'deepsecret' not in self.permissions_checked
@@ -489,47 +488,47 @@
         assert len(self.permissions_checked) == 1
         assert 'independent' in self.permissions_checked
 
     def test_independent_check_success(self):
         self.secret_cls.independent_authorization = True
         response = self.app.get('/secret/independent')
         assert response.status_int == 200
-        assert response.body == b_('Independent Security')
+        assert response.body == b'Independent Security'
         assert len(self.permissions_checked) == 1
         assert 'independent' in self.permissions_checked
 
     def test_wrapped_attribute_failure(self):
         self.secret_cls.independent_authorization = False
         response = self.app.get('/secret/wrapped/', expect_errors=True)
         assert response.status_int == 401
         assert len(self.permissions_checked) == 1
         assert 'independent' in self.permissions_checked
 
     def test_wrapped_attribute_success(self):
         self.secret_cls.independent_authorization = True
         response = self.app.get('/secret/wrapped/')
         assert response.status_int == 200
-        assert response.body == b_('Index wrapped')
+        assert response.body == b'Index wrapped'
         assert len(self.permissions_checked) == 1
         assert 'independent' in self.permissions_checked
 
     def test_lookup_to_wrapped_attribute_on_self(self):
         self.secret_cls.authorized = True
         self.secret_cls.independent_authorization = True
         response = self.app.get('/secret/lookup_wrapped/')
         assert response.status_int == 200
-        assert response.body == b_('Index wrapped')
+        assert response.body == b'Index wrapped'
         assert len(self.permissions_checked) == 2
         assert 'independent' in self.permissions_checked
         assert 'secretcontroller' in self.permissions_checked
 
     def test_unlocked_attribute_in_insecure(self):
         response = self.app.get('/notsecret/unlocked/')
         assert response.status_int == 200
-        assert response.body == b_('Index unlocked')
+        assert response.body == b'Index unlocked'
 
 
 class SecureControllerSharedPermissionsRegression(PecanTestCase):
     """Regression tests for https://github.com/dreamhost/pecan/issues/131"""
 
     def setUp(self):
         super(SecureControllerSharedPermissionsRegression, self).setUp()
```

### Comparing `pecan-1.4.2/pecan/tests/test_templating.py` & `pecan-1.5.0/pecan/tests/test_templating.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import tempfile
 
-from six import b as b_
-
 from pecan.templating import RendererFactory, format_line_context
 from pecan.tests import PecanTestCase
 
 
 class TestTemplate(PecanTestCase):
     def setUp(self):
         super(TestTemplate, self).setUp()
@@ -40,11 +38,11 @@
         self.f = tempfile.NamedTemporaryFile()
 
     def tearDown(self):
         del self.f
 
     def test_format_line_context(self):
         for i in range(11):
-            self.f.write(b_('Testing Line %d\n' % i))
+            self.f.write(b'Testing Line %d\n' % i)
         self.f.flush()
 
         assert format_line_context(self.f.name, 0).count('Testing Line') == 10
```

### Comparing `pecan-1.4.2/pecan/tests/test_util.py` & `pecan-1.5.0/pecan/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/pecan/util.py` & `pecan-1.5.0/pecan/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-import sys
-
-import six
-
 from pecan.compat import getargspec as _getargspec
 
 
 def iscontroller(obj):
     return getattr(obj, 'exposed', False)
 
 
@@ -18,30 +14,30 @@
     argspec = _getargspec(method)
     args = argspec[0]
     if args and args[0] == 'self':
         return argspec
     if hasattr(method, '__func__'):
         method = method.__func__
 
-    func_closure = six.get_function_closure(method)
+    func_closure = method.__closure__
 
     # NOTE(sileht): if the closure is None we cannot look deeper,
     # so return actual argspec, this occurs when the method
     # is static for example.
     if not func_closure:
         return argspec
 
     closure = None
     # In the case of deeply nested decorators (with arguments), it's possible
     # that there are several callables in scope;  Take a best guess and go
     # with the one that looks most like a pecan controller function
     # (has a __code__ object, and 'self' is the first argument)
     func_closure = filter(
         lambda c: (
-            six.callable(c.cell_contents) and
+            callable(c.cell_contents) and
             hasattr(c.cell_contents, '__code__')
         ),
         func_closure
     )
     func_closure = sorted(
         func_closure,
         key=lambda c: 'self' in c.cell_contents.__code__.co_varnames,
```

### Comparing `pecan-1.4.2/pecan.egg-info/PKG-INFO` & `pecan-1.5.0/pecan.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pecan
-Version: 1.4.2
+Version: 1.5.0
 Summary: A WSGI object-dispatching web framework, designed to be lean and fast, with few dependencies.
 Home-page: http://github.com/pecan/pecan
 Author: Jonathan LaCour
 Author-email: info@pecanpy.org
 License: BSD
 Keywords: web framework wsgi object-dispatch http
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
@@ -23,7 +24,10 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 License-File: LICENSE
 License-File: AUTHORS
+
+UNKNOWN
+
```

### Comparing `pecan-1.4.2/pecan.egg-info/SOURCES.txt` & `pecan-1.5.0/pecan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pecan-1.4.2/setup.py` & `pecan-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import platform
 
 from setuptools import setup, find_packages
 
-version = '1.4.2'
+version = '1.5.0'
 
 #
 # determine requirements
 #
 with open('requirements.txt') as reqs:
     requirements = [
         line for line in reqs.read().split('\n')
```

