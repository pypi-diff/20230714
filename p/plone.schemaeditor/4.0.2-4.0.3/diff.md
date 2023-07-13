# Comparing `tmp/plone.schemaeditor-4.0.2.tar.gz` & `tmp/plone.schemaeditor-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.schemaeditor-4.0.2.tar", last modified: Tue Feb  7 23:02:42 2023, max compression
+gzip compressed data, was "plone.schemaeditor-4.0.3.tar", last modified: Tue Mar 14 22:43:34 2023, max compression
```

## Comparing `plone.schemaeditor-4.0.2.tar` & `plone.schemaeditor-4.0.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:02:42.551123 plone.schemaeditor-4.0.2/
--rw-r--r--   0 maurits    (501) staff       (20)    17448 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    19773 2023-02-07 23:02:42.551322 plone.schemaeditor-4.0.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1414 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:02:42.529883 plone.schemaeditor-4.0.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     1484 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/docs/LICENSE.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:02:42.530306 plone.schemaeditor-4.0.2/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:02:42.537491 plone.schemaeditor-4.0.2/plone/schemaeditor/
--rw-r--r--   0 maurits    (501) staff       (20)       76 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:02:42.538323 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      216 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:02:42.541169 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/field/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/field/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1138 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/field/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      462 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/field/edit.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5908 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/field/edit.py
--rw-r--r--   0 maurits    (501) staff       (20)     1002 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/field/fieldset.py
--rw-r--r--   0 maurits    (501) staff       (20)     2178 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/field/order.py
--rw-r--r--   0 maurits    (501) staff       (20)     1272 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/field/traversal.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:02:42.545020 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/schema/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/schema/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      462 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/schema/add.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4229 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/schema/add_field.py
--rw-r--r--   0 maurits    (501) staff       (20)     2060 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/schema/add_fieldset.py
--rw-r--r--   0 maurits    (501) staff       (20)      979 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/schema/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1694 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/schema/delete_fieldset.py
--rw-r--r--   0 maurits    (501) staff       (20)     6108 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/schema/listing.py
--rw-r--r--   0 maurits    (501) staff       (20)     5774 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/schema/schema_listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1589 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/browser/schema/traversal.py
--rw-r--r--   0 maurits    (501) staff       (20)      786 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    10104 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/fields.py
--rw-r--r--   0 maurits    (501) staff       (20)     1718 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/fields.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5823 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     2592 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/schema.py
--rw-r--r--   0 maurits    (501) staff       (20)      758 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/schema.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      587 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:02:42.550361 plone.schemaeditor-4.0.2/plone/schemaeditor/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2572 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/tests/browser_testing.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     7337 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/tests/choice.rst
--rw-r--r--   0 maurits    (501) staff       (20)    18502 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/tests/editing.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3377 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/tests/extending.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1471 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/tests/field_schemata.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1722 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/tests/fixtures.py
--rw-r--r--   0 maurits    (501) staff       (20)      163 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/tests/layout.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2193 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/tests/minmax.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:02:42.550778 plone.schemaeditor-4.0.2/plone/schemaeditor/tests/robot/
--rw-r--r--   0 maurits    (501) staff       (20)     9217 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/tests/robot/test_fields.robot
--rw-r--r--   0 maurits    (501) staff       (20)      605 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/tests/robot_testing.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1367 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/tests/test_fields.py
--rw-r--r--   0 maurits    (501) staff       (20)      789 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/tests/test_robot.py
--rw-r--r--   0 maurits    (501) staff       (20)     2159 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/tests/tests.py
--rw-r--r--   0 maurits    (501) staff       (20)     7902 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)      826 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/plone/schemaeditor/vocabularies.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-02-07 23:02:42.533297 plone.schemaeditor-4.0.2/plone.schemaeditor.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    19773 2023-02-07 23:02:42.000000 plone.schemaeditor-4.0.2/plone.schemaeditor.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2104 2023-02-07 23:02:42.000000 plone.schemaeditor-4.0.2/plone.schemaeditor.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-02-07 23:02:42.000000 plone.schemaeditor-4.0.2/plone.schemaeditor.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-02-07 23:02:42.000000 plone.schemaeditor-4.0.2/plone.schemaeditor.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-02-07 23:02:42.000000 plone.schemaeditor-4.0.2/plone.schemaeditor.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      485 2023-02-07 23:02:42.000000 plone.schemaeditor-4.0.2/plone.schemaeditor.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-02-07 23:02:42.000000 plone.schemaeditor-4.0.2/plone.schemaeditor.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      925 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      215 2023-02-07 23:02:42.552282 plone.schemaeditor-4.0.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2176 2023-02-07 23:02:41.000000 plone.schemaeditor-4.0.2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:43:34.689318 plone.schemaeditor-4.0.3/
+-rw-r--r--   0 maurits    (501) staff       (20)    17557 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    19882 2023-03-14 22:43:34.689437 plone.schemaeditor-4.0.3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1414 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:43:34.674513 plone.schemaeditor-4.0.3/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     1484 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/docs/LICENSE.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:43:34.674801 plone.schemaeditor-4.0.3/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:43:34.679959 plone.schemaeditor-4.0.3/plone/schemaeditor/
+-rw-r--r--   0 maurits    (501) staff       (20)       76 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:43:34.680466 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      218 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:43:34.682293 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/field/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/field/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1077 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/field/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      485 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/field/edit.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5907 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/field/edit.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1002 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/field/fieldset.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2178 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/field/order.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1272 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/field/traversal.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:43:34.685059 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/schema/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/schema/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      485 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/schema/add.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4228 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/schema/add_field.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2059 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/schema/add_fieldset.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1020 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/schema/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1694 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/schema/delete_fieldset.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6107 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/schema/listing.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6412 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/schema/schema_listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1589 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/browser/schema/traversal.py
+-rw-r--r--   0 maurits    (501) staff       (20)      815 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    10101 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/fields.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1723 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/fields.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5820 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2588 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/schema.py
+-rw-r--r--   0 maurits    (501) staff       (20)      754 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/schema.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      586 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:43:34.688735 plone.schemaeditor-4.0.3/plone/schemaeditor/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2520 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/tests/browser_testing.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     7337 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/tests/choice.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    18502 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/tests/editing.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3377 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/tests/extending.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1471 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/tests/field_schemata.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1718 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/tests/fixtures.py
+-rw-r--r--   0 maurits    (501) staff       (20)      186 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/tests/layout.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2193 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/tests/minmax.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:43:34.689109 plone.schemaeditor-4.0.3/plone/schemaeditor/tests/robot/
+-rw-r--r--   0 maurits    (501) staff       (20)     9217 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/tests/robot/test_fields.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      601 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/tests/robot_testing.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1366 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/tests/test_fields.py
+-rw-r--r--   0 maurits    (501) staff       (20)      789 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/tests/test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2159 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/tests/tests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7902 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)      826 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/plone/schemaeditor/vocabularies.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-14 22:43:34.677100 plone.schemaeditor-4.0.3/plone.schemaeditor.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    19882 2023-03-14 22:43:34.000000 plone.schemaeditor-4.0.3/plone.schemaeditor.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2104 2023-03-14 22:43:34.000000 plone.schemaeditor-4.0.3/plone.schemaeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-14 22:43:34.000000 plone.schemaeditor-4.0.3/plone.schemaeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-14 22:43:34.000000 plone.schemaeditor-4.0.3/plone.schemaeditor.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-14 22:43:34.000000 plone.schemaeditor-4.0.3/plone.schemaeditor.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      485 2023-03-14 22:43:34.000000 plone.schemaeditor-4.0.3/plone.schemaeditor.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-14 22:43:34.000000 plone.schemaeditor-4.0.3/plone.schemaeditor.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      925 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      240 2023-03-14 22:43:34.689885 plone.schemaeditor-4.0.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2176 2023-03-14 22:43:33.000000 plone.schemaeditor-4.0.3/setup.py
```

### Comparing `plone.schemaeditor-4.0.2/CHANGES.rst` & `plone.schemaeditor-4.0.3/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.3 (2023-03-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (13d8d6c0)
+
+
 4.0.2 (2023-02-08)
 ------------------
 
 Bug fixes:
 
 
 - Declare all dependencies.
```

### Comparing `plone.schemaeditor-4.0.2/PKG-INFO` & `plone.schemaeditor-4.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.schemaeditor
-Version: 4.0.2
+Version: 4.0.3
 Summary: Provides through-the-web editing of a zope schema/interface.
 Home-page: https://github.com/plone/plone.schemaeditor
 Author: David Glick
 Author-email: dglick@gmail.com
 License: BSD
 Keywords: plone schema ttw
 Classifier: Development Status :: 6 - Mature
@@ -96,14 +96,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.3 (2023-03-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (13d8d6c0)
+
+
 4.0.2 (2023-02-08)
 ------------------
 
 Bug fixes:
 
 
 - Declare all dependencies.
```

### Comparing `plone.schemaeditor-4.0.2/README.rst` & `plone.schemaeditor-4.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `plone.schemaeditor-4.0.2/docs/LICENSE.rst` & `plone.schemaeditor-4.0.3/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/browser/field/configure.zcml` & `plone.schemaeditor-4.0.3/plone/schemaeditor/browser/field/configure.zcml`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    xmlns:five="http://namespaces.zope.org/five"
     xmlns:browser="http://namespaces.zope.org/browser"
-    i18n_domain="plone">
+    xmlns:five="http://namespaces.zope.org/five"
+    i18n_domain="plone"
+    >
 
-    <browser:page
-        name="edit"
-        for="...interfaces.IFieldContext"
-        class=".edit.EditView"
-        permission="plone.schemaeditor.ManageSchemata" />
-
-    <adapter
-        factory=".edit.FieldTitleAdapter" />
-    <adapter
-        factory=".edit.FieldDataManager" />
-
-    <browser:page
-        name="order"
-        for="...interfaces.IFieldContext"
-        class=".order.FieldOrderView"
-        attribute="move"
-        permission="plone.schemaeditor.ManageSchemata"
-        />
-
-    <browser:page
-        name="delete"
-        for="...interfaces.IFieldContext"
-        class=".order.FieldOrderView"
-        attribute="delete"
-        permission="plone.schemaeditor.ManageSchemata"
-        />
-
-    <browser:page
-        name="changefieldset"
-        for="...interfaces.IFieldContext"
-        class=".fieldset.ChangeFieldsetView"
-        attribute="change"
-        permission="plone.schemaeditor.ManageSchemata"
-        />
+  <browser:page
+      name="edit"
+      for="...interfaces.IFieldContext"
+      class=".edit.EditView"
+      permission="plone.schemaeditor.ManageSchemata"
+      />
+
+  <adapter factory=".edit.FieldTitleAdapter" />
+  <adapter factory=".edit.FieldDataManager" />
+
+  <browser:page
+      name="order"
+      for="...interfaces.IFieldContext"
+      class=".order.FieldOrderView"
+      attribute="move"
+      permission="plone.schemaeditor.ManageSchemata"
+      />
+
+  <browser:page
+      name="delete"
+      for="...interfaces.IFieldContext"
+      class=".order.FieldOrderView"
+      attribute="delete"
+      permission="plone.schemaeditor.ManageSchemata"
+      />
+
+  <browser:page
+      name="changefieldset"
+      for="...interfaces.IFieldContext"
+      class=".fieldset.ChangeFieldsetView"
+      attribute="change"
+      permission="plone.schemaeditor.ManageSchemata"
+      />
 
 </configure>
```

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/browser/field/edit.py` & `plone.schemaeditor-4.0.3/plone/schemaeditor/browser/field/edit.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
             return getObjectSpecification(cls)
         else:
             return inst.__provides__
 
 
 @implementer(IFieldProxy)
 class FieldProxy:
-
     __providedBy__ = FieldProxySpecification()
 
     def __init__(self, context):
         self.__class__ = type(
             context.__class__.__name__, (self.__class__, context.__class__), {}
         )
         self.__dict__ = context.__dict__
```

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/browser/field/fieldset.py` & `plone.schemaeditor-4.0.3/plone/schemaeditor/browser/field/fieldset.py`

 * *Files identical despite different names*

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/browser/field/order.py` & `plone.schemaeditor-4.0.3/plone/schemaeditor/browser/field/order.py`

 * *Files identical despite different names*

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/browser/field/traversal.py` & `plone.schemaeditor-4.0.3/plone/schemaeditor/browser/field/traversal.py`

 * *Files identical despite different names*

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/browser/schema/add_field.py` & `plone.schemaeditor-4.0.3/plone/schemaeditor/browser/schema/add_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from zope.event import notify
 from zope.interface import Interface
 from zope.interface import Invalid
 from zope.lifecycleevent import ObjectAddedEvent
 
 
 class FieldAddForm(AutoExtensibleForm, form.AddForm):
-
     fields = field.Fields(interfaces.INewField)
     label = _("Add new field")
     id = "add-field-form"
 
     # This is a trick: we want autoform to handle the additionalSchemata,
     # but want to provide our own base schema below in updateFields.
     schema = Interface
```

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/browser/schema/add_fieldset.py` & `plone.schemaeditor-4.0.3/plone/schemaeditor/browser/schema/add_fieldset.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from z3c.form.interfaces import WidgetActionExecutionError
 from zope.container.contained import notifyContainerModified
 from zope.event import notify
 from zope.interface import Invalid
 
 
 class FieldsetAddForm(form.AddForm):
-
     fields = field.Fields(INewFieldset)
     label = _("Add new fieldset")
     id = "add-fieldset-form"
 
     def create(self, data):
         return Fieldset(**data)
```

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/browser/schema/configure.zcml` & `plone.schemaeditor-4.0.3/plone/schemaeditor/browser/schema/configure.zcml`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    xmlns:five="http://namespaces.zope.org/five"
     xmlns:browser="http://namespaces.zope.org/browser"
-    i18n_domain="plone">
+    xmlns:five="http://namespaces.zope.org/five"
+    i18n_domain="plone"
+    >
 
   <browser:page
       name="edit"
       for="plone.schemaeditor.interfaces.ISchemaContext"
       class=".listing.SchemaListingPage"
-      permission="plone.schemaeditor.ManageSchemata" />
+      permission="plone.schemaeditor.ManageSchemata"
+      />
 
   <browser:page
-    name="add-field"
-    for="plone.schemaeditor.interfaces.ISchemaContext"
-    class=".add_field.FieldAddFormPage"
-    permission="plone.schemaeditor.ManageSchemata"
-    />
+      name="add-field"
+      for="plone.schemaeditor.interfaces.ISchemaContext"
+      class=".add_field.FieldAddFormPage"
+      permission="plone.schemaeditor.ManageSchemata"
+      />
 
   <browser:page
-    name="add-fieldset"
-    for="plone.schemaeditor.interfaces.ISchemaContext"
-    class=".add_fieldset.FieldsetAddFormPage"
-    permission="plone.schemaeditor.ManageSchemata"
-    />
+      name="add-fieldset"
+      for="plone.schemaeditor.interfaces.ISchemaContext"
+      class=".add_fieldset.FieldsetAddFormPage"
+      permission="plone.schemaeditor.ManageSchemata"
+      />
 
   <browser:page
-    name="delete-fieldset"
-    for="plone.schemaeditor.interfaces.ISchemaContext"
-    class=".delete_fieldset.DeleteFieldset"
-    permission="plone.schemaeditor.ManageSchemata"
-    />
+      name="delete-fieldset"
+      for="plone.schemaeditor.interfaces.ISchemaContext"
+      class=".delete_fieldset.DeleteFieldset"
+      permission="plone.schemaeditor.ManageSchemata"
+      />
 
 </configure>
```

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/browser/schema/delete_fieldset.py` & `plone.schemaeditor-4.0.3/plone/schemaeditor/browser/schema/delete_fieldset.py`

 * *Files identical despite different names*

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/browser/schema/listing.py` & `plone.schemaeditor-4.0.3/plone/schemaeditor/browser/schema/listing.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 except ImportError:
     # plone.protect < 3.x, e.g. in Plone 4.3
     addTokenToUrl = None
 
 
 @implementer(IEditForm)
 class SchemaListing(AutoExtensibleForm, form.Form):
-
     ignoreContext = True
     ignoreRequest = True
     showEmptyGroups = True
     template = ViewPageTemplateFile("schema_listing.pt")
     ignoreRequiredOnExtract = True
 
     @property
```

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/browser/schema/schema_listing.pt` & `plone.schemaeditor-4.0.3/plone/schemaeditor/browser/schema/schema_listing.pt`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-<div xmlns:tal="http://xml.zope.org/namespaces/tal"
+<div xmlns:i18n="http://xml.zope.org/namespaces/i18n"
      xmlns:metal="http://xml.zope.org/namespaces/metal"
-     xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+     xmlns:tal="http://xml.zope.org/namespaces/tal"
+     class="pat-schemaeditor"
      i18n:domain="plone"
-     class="pat-schemaeditor">
-  <a id="add-field" class="pat-plone-modal btn btn-secondary float-end ms-3"
+>
+  <a class="pat-plone-modal btn btn-secondary float-end ms-3"
+     id="add-field"
      href="${context/absolute_url}/@@add-field"
-     i18n:translate="add_new_field_hellip">
+     i18n:translate="add_new_field_hellip"
+  >
      Add new field&hellip;
   </a>
 
-  <a id="add-fieldset" class="pat-plone-modal btn btn-secondary float-end" tal:condition="context/enableFieldsets"
+  <a class="pat-plone-modal btn btn-secondary float-end"
+     id="add-fieldset"
      href="${context/absolute_url}/@@add-fieldset"
-     i18n:translate="add_fieldset_hellip">
+     tal:condition="context/enableFieldsets"
+     i18n:translate="add_fieldset_hellip"
+  >
      Add new fieldset&hellip;
   </a>
 
   <metal:form metal:use-macro="context/@@ploneform-macros/form">
     <metal:top-slot metal:fill-slot="formtop">
       <input tal:replace="structure context/@@authenticator/authenticator" />
       <style type="text/css">
@@ -70,81 +76,116 @@
   }
       </style>
     </metal:top-slot>
 
     <metal:fields-slot metal:fill-slot="fields">
 
       <tal:block tal:repeat="group python:[view] + list(view.groups)">
-        <fieldset tal:define="fieldset_name repeat/group/index;
-                              can_delete python:view.can_delete_fieldset(group);"
-                  tal:attributes="id string:fieldset-${fieldset_name};
-                                  class string:kssattr-fieldset-${fieldset_name};
-                                  data-can-add-fields python:(repeat['group'].start or can_delete) and 'true' or 'false'">
-
-          <legend tal:define="group_name python:group.label or view.default_fieldset_label"
-                  tal:content="group_name">Fieldset name</legend>
-
-          <a id="delete-fieldset-${fieldset_name}" class="btn btn-sm btn-danger" tal:condition="python:context.enableFieldsets and can_delete"
-             href="${context/absolute_url}/@@delete-fieldset?name=${python:group.__name__}&_authenticator=${context/@@authenticator/token}"
-                  i18n:translate="delete_fieldset_hellip">Delete fieldset
+        <fieldset tal:define="
+                    fieldset_name repeat/group/index;
+                    can_delete python:view.can_delete_fieldset(group);
+                  "
+                  tal:attributes="
+                    id string:fieldset-${fieldset_name};
+                    class string:kssattr-fieldset-${fieldset_name};
+                    data-can-add-fields python:(repeat['group'].start or can_delete) and 'true' or 'false';
+                  "
+        >
+
+          <legend tal:define="
+                    group_name python:group.label or view.default_fieldset_label;
+                  "
+                  tal:content="group_name"
+          >Fieldset name</legend>
+
+          <a class="btn btn-sm btn-danger"
+             id="delete-fieldset-${fieldset_name}"
+             href="${context/absolute_url}/@@delete-fieldset?name=${python:group.__name__}&amp;_authenticator=${context/@@authenticator/token}"
+             i18n:translate="delete_fieldset_hellip"
+          >Delete fieldset
           </a>
 
-          <tal:block tal:define="errors group/widgets/errors"
+          <tal:block tal:define="
+                       errors group/widgets/errors;
+                     "
                      tal:condition="errors"
-                     tal:repeat="error errors">
-              <div class="field error"
-                  tal:condition="not:nocall:error/widget"
-                  tal:content="structure error/render"
-                  />
+                     tal:repeat="error errors"
+          >
+            <div class="field error"
+                 tal:condition="not:nocall:error/widget"
+                 tal:content="structure error/render"
+            ></div>
           </tal:block>
 
           <tal:widgets repeat="widget group/widgets/values">
-            <tal:block
-              tal:define="
-                disabled widget/disabled|nothing;
-                protected python:view.protected_field(widget.field);">
-
-              <div tal:condition="python:disabled or protected" class="fieldPreview fieldFromBehavior">
+            <tal:block tal:define="
+                         disabled widget/disabled|nothing;
+                         protected python:view.protected_field(widget.field);
+                       ">
+
+              <div class="fieldPreview fieldFromBehavior"
+                   tal:condition="python:disabled or protected"
+              >
                 <div class="fieldLabel">
-                    <tal:block tal:condition="disabled" i18n:translate="">From the
-                      <tal:block i18n:name="behavior_name" tal:replace="python:widget.__name__.split('.')[0]"/> behavior:</tal:block>
-                    <strong tal:content="widget/field/__name__" /> &ndash;
-                    <tal:block tal:content="python:view.field_type(widget.field)"/>
+                  <tal:block tal:condition="disabled"
+                             i18n:translate=""
+                  >From the
+                    <tal:block tal:replace="python:widget.__name__.split('.')[0]"
+                               i18n:name="behavior_name"
+                    />
+                    behavior:</tal:block>
+                  <strong tal:content="widget/field/__name__"></strong>
+                 &ndash;
+                  <tal:block tal:content="python:view.field_type(widget.field)" />
                 </div>
                 <tal:field tal:replace="structure widget/@@ploneform-render-widget" />
                 <div class="disabled-field-overlay"></div>
               </div>
 
-              <div tal:condition="python:not(disabled or protected)"
-                   class="fieldPreview orderable" tal:attributes="data-field_id widget/field/__name__">
+              <div class="fieldPreview orderable"
+                   tal:condition="python:not(disabled or protected)"
+                   tal:attributes="
+                     data-field_id widget/field/__name__;
+                   "
+              >
 
                 <div class="fieldLabel">
-                    <strong tal:content="widget/field/__name__" /> &ndash;
-                    <tal:block tal:content="python:view.field_type(widget.field)"/>
+                  <strong tal:content="widget/field/__name__"></strong>
+                 &ndash;
+                  <tal:block tal:content="python:view.field_type(widget.field)" />
                 </div>
 
                 <div class="fieldControls">
-                    <a class="fieldSettings pat-plone-modal btn btn-sm btn-secondary"
-                       tal:define="edit_url python:view.edit_url(widget.field)"
-                       tal:condition="edit_url"
-                       i18n:translate=""
-                       tal:attributes="href edit_url">Settings&hellip;</a>
-                    <a class="schemaeditor-delete-field btn btn-sm btn-danger ms-1"
-                       i18n:attributes="title; data-confirm_msg"
-                       title="Delete field"
-                       data-confirm_msg="Are you sure you want to delete this field?"
-                       tal:define="delete_url python:view.delete_url(widget.field)"
-                       tal:condition="delete_url"
-                       tal:attributes="href delete_url">&times;</a>
+                  <a class="fieldSettings pat-plone-modal btn btn-sm btn-secondary"
+                     tal:define="
+                       edit_url python:view.edit_url(widget.field);
+                     "
+                     tal:condition="edit_url"
+                     tal:attributes="
+                       href edit_url;
+                     "
+                     i18n:translate=""
+                  >Settings&hellip;</a>
+                  <a class="schemaeditor-delete-field btn btn-sm btn-danger ms-1"
+                     title="Delete field"
+                     data-confirm_msg="Are you sure you want to delete this field?"
+                     tal:define="
+                       delete_url python:view.delete_url(widget.field);
+                     "
+                     tal:condition="delete_url"
+                     tal:attributes="
+                       href delete_url;
+                     "
+                     i18n:attributes="title; data-confirm_msg"
+                  >&times;</a>
                 </div>
 
                 <div style="width: 80%">
                   <tal:field tal:replace="structure widget/@@ploneform-render-widget" />
                 </div>
-
               </div>
             </tal:block>
 
           </tal:widgets>
 
         </fieldset>
       </tal:block>
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 Add_new_field… Add_new_fieldset…   [                    ]
      Fieldset name Delete_fieldset
 
-From the  behavior: –
-–
+From the  behavior:  –
+ –
 Settings… ×
```

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/browser/schema/traversal.py` & `plone.schemaeditor-4.0.3/plone/schemaeditor/browser/schema/traversal.py`

 * *Files identical despite different names*

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/configure.zcml` & `plone.schemaeditor-4.0.3/plone/schemaeditor/configure.zcml`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:five="http://namespaces.zope.org/five"
     xmlns:i18n="http://namespaces.zope.org/i18n"
-    i18n_domain="plone">
+    i18n_domain="plone"
+    >
 
-  <include package="plone.z3cform"/>
-  <include package="plone.protect"/>
-  <include package="Products.statusmessages"/>
+  <include package="plone.z3cform" />
+  <include package="plone.protect" />
+  <include package="Products.statusmessages" />
 
-  <include file="schema.zcml"/>
+  <include file="schema.zcml" />
 
   <permission
       id="plone.schemaeditor.ManageSchemata"
       title="Manage schemata"
-  />
+      />
 
   <!-- adapter for adding/removing fields on schemata -->
-  <adapter factory=".utils.EditableSchema"/>
+  <adapter factory=".utils.EditableSchema" />
 
-  <include file="fields.zcml"/>
-  <include package=".browser"/>
+  <include file="fields.zcml" />
+  <include package=".browser" />
 
-  <utility factory=".vocabularies.VocabulariesVocabulary"
+  <utility
+      factory=".vocabularies.VocabulariesVocabulary"
+      provides="zope.schema.interfaces.IVocabularyFactory"
       name="plone.schemaeditor.VocabulariesVocabulary"
-      provides="zope.schema.interfaces.IVocabularyFactory"/>
+      />
 
 </configure>
```

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/fields.py` & `plone.schemaeditor-4.0.3/plone/schemaeditor/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     return [
         s for s in field.__provides__.__iro__ if s.isOrExtends(schema_ifaces.IField)
     ][0]
 
 
 @implementer(IFieldFactory)
 class FieldFactory:
-
     title = ""
 
     def __init__(self, fieldcls, title, *args, **kw):
         self.fieldcls = fieldcls
         self.title = title
         self.args = args
         self.kw = kw
@@ -61,15 +60,15 @@
     field_factories = getUtilitiesFor(IFieldFactory)
     allowedFields = getattr(context, "allowedFields", None)
     if allowedFields is not None:
         field_factories = [
             (id, factory) for id, factory in field_factories if id in allowedFields
         ]
     terms = []
-    for (field_id, factory) in field_factories:
+    for field_id, factory in field_factories:
         terms.append(
             SimpleVocabulary.createTerm(
                 factory, factory.title, translate(factory.title, context=request)
             )
         )
     terms = sorted(terms, key=operator.attrgetter("title"))
     return SimpleVocabulary(terms)
```

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/fields.zcml` & `plone.schemaeditor-4.0.3/plone/schemaeditor/fields.zcml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    i18n_domain="plone">
+    i18n_domain="plone"
+    >
 
   <adapter factory=".fields.getFirstFieldSchema" />
 
   <utility
-      component=".fields.FieldsVocabularyFactory"
       provides="zope.schema.interfaces.IVocabularyFactory"
       name="Fields"
+      component=".fields.FieldsVocabularyFactory"
       />
 
   <utility
       name="zope.schema._bootstrapfields.TextLine"
       component=".fields.TextLineFactory"
       />
   <utility
```

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/interfaces.py` & `plone.schemaeditor-4.0.3/plone/schemaeditor/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,14 @@
         """List of field names that may not be deleted from this schema."""
     )
 
     enableFieldsets = Attribute("""Enable extra fieldsets.""")
 
 
 class ISchemaModifiedEvent(IObjectEvent):
-
     object = Object(schema=ISchemaContext)
 
 
 class IFieldContext(IItem):
     """A publishable wrapper of a zope 3 schema field"""
 
     field = Object(schema=IField)
@@ -138,15 +137,14 @@
         )
     if value in RESERVED_NAMES:
         raise Invalid(_("'${name}' is a reserved field name.", mapping={"name": value}))
     return True
 
 
 class INewField(Interface):
-
     fieldset_id = Int(
         title=_("Fieldset ID"),
         description=_("Used to decide where to put this field."),
         required=True,
     )
 
     title = TextLine(title=_("Title"), required=True)
@@ -188,15 +186,14 @@
                     _("The 'title' field must be a Text line (string) field.")
                 )
             if data.__name__ == "description" and data.factory.fieldcls is not Text:
                 raise Invalid(_("The 'description' field must be a Text field."))
 
 
 class INewFieldset(Interface):
-
     label = TextLine(title=_("Title"), required=True)
 
     __name__ = ASCIILine(
         title=_("Short Name"),
         description=_("Used for programmatic access to the fieldset."),
         required=True,
         constraint=isValidFieldName,
```

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/schema.py` & `plone.schemaeditor-4.0.3/plone/schemaeditor/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,45 +14,42 @@
 
 
 class IBool(interfaces.IBool, interfaces.IFromUnicode):
     pass
 
 
 class IFloat(interfaces.IFloat, interfaces.IFromUnicode):
-
     min = schema.Float(
         title=interfaces.IFloat["min"].title,
         required=interfaces.IFloat["min"].required,
         default=interfaces.IFloat["min"].default,
     )
 
     max = schema.Float(
         title=interfaces.IFloat["max"].title,
         required=interfaces.IFloat["max"].required,
         default=interfaces.IFloat["max"].default,
     )
 
 
 class IDatetime(IDatetimeField):
-
     min = schema.Datetime(
         title=interfaces.IDatetime["min"].title,
         required=interfaces.IDatetime["min"].required,
         default=interfaces.IDatetime["min"].default,
     )
 
     max = schema.Datetime(
         title=interfaces.IDatetime["max"].title,
         required=interfaces.IDatetime["max"].required,
         default=interfaces.IDatetime["max"].default,
     )
 
 
 class IDate(IDateField):
-
     min = schema.Date(
         title=interfaces.IDate["min"].title,
         required=interfaces.IDate["min"].required,
         default=interfaces.IDate["min"].default,
     )
 
     max = schema.Date(
@@ -68,15 +65,14 @@
 
 class ITextLinesField(interfaces.IList):
 
     """A marker for fields which should get the textlines widget"""
 
 
 class ITextLineChoice(interfaces.IField):
-
     values = schema.List(
         title=_("Possible values"),
         description=_("Enter allowed choices one per line."),
         required=interfaces.IChoice["vocabulary"].required,
         default=interfaces.IChoice["vocabulary"].default,
         value_type=schema.TextLine(),
     )
```

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/schema.zcml` & `plone.schemaeditor-4.0.3/plone/schemaeditor/schema.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-<configure
-    xmlns="http://namespaces.zope.org/zope">
+<configure xmlns="http://namespaces.zope.org/zope">
 
   <class class="zope.schema.Bool">
     <implements interface=".schema.IBool" />
   </class>
 
   <class class="zope.schema.Float">
     <implements interface=".schema.IFloat" />
```

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/testing.py` & `plone.schemaeditor-4.0.3/plone/schemaeditor/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import PLONE_FIXTURE
 from plone.app.testing import PloneSandboxLayer
 from plone.testing import z2
 
 
 class PloneSchemaeditorRobotLayer(PloneSandboxLayer):
-
     defaultBases = (PLONE_FIXTURE,)
 
 
 FIXTURE = PloneSchemaeditorRobotLayer(
     name="ROBOT",
 )
```

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/tests/browser_testing.zcml` & `plone.schemaeditor-4.0.3/plone/schemaeditor/tests/browser_testing.zcml`

 * *Files 13% similar despite different names*

```diff
@@ -1,74 +1,89 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:browser="http://namespaces.zope.org/browser"
-    xmlns:zcml="http://namespaces.zope.org/zcml">
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    >
 
-    <!-- only load PageTemplates zcml in Zope 4 -->
-    <configure zcml:condition="installed Products.PageTemplates.engine">
-        <include package="Products.PageTemplates" />
-    </configure>
-
-    <include package="Products.GenericSetup" file="meta.zcml" />
-    <include package="Products.Five" file="meta.zcml" />
-    <include package="Products.Five" />
-    <include package="plone.schemaeditor"/>
-
-    <!-- dummy keyring -->
-    <utility component=".fixtures.DummyKeyManager"
-             provides="plone.keyring.interfaces.IKeyManager" />
-
-    <!-- dummy schema editing context -->
-    <browser:page
-        name="schemaeditor"
-        for="*"
-        class=".fixtures.DummySchemaContext"
-        permission="plone.schemaeditor.ManageSchemata"
-        allowed_interface="OFS.interfaces.IItem" />
-
-    <subscriber
-        for="plone.schemaeditor.interfaces.IField
-             zope.lifecycleevent.interfaces.IObjectModifiedEvent"
-        handler=".fixtures.log_event"
-        />
-    <subscriber
-        for="plone.schemaeditor.interfaces.IField
-             zope.lifecycleevent.interfaces.IObjectMovedEvent"
-        handler=".fixtures.log_event"
-        />
-    <subscriber
-        for="zope.interface.interfaces.IInterface
-             zope.container.interfaces.IContainerModifiedEvent"
-        handler=".fixtures.log_event"
-        />
-    <subscriber
-        for="plone.schemaeditor.interfaces.ISchemaContext
-             plone.schemaeditor.interfaces.ISchemaModifiedEvent"
-        handler=".fixtures.log_event"
-        />
-
-    <!-- use a form layout that doesn't pull in main_template -->
-    <adapter factory=".tests.layout_factory"/>
-
-    <!-- provide a widget renderer a la plone.app.z3cform -->
-    <browser:page
-        name="ploneform-render-widget"
-        for="z3c.form.interfaces.IWidget"
-        class=".tests.RenderWidget"
-        permission="zope2.View"
-        />
-
-    <browser:page
-        name="contexteditor"
-        for="*"
-        class=".fixtures.EditView"
-        permission="plone.schemaeditor.ManageSchemata" />
-
-    <utility provides="zope.schema.interfaces.IVocabularyFactory"
-             name="plone.schemaeditor.test.Countries"
-             factory=".fixtures.CountriesVocabulary" />
-
-    <utility provides="zope.schema.interfaces.IVocabularyFactory"
-             name="plone.schemaeditor.test.Categories"
-             factory=".fixtures.CategoriesVocabulary" />
+  <!-- only load PageTemplates zcml in Zope 4 -->
+  <configure zcml:condition="installed Products.PageTemplates.engine">
+    <include package="Products.PageTemplates" />
+  </configure>
+
+  <include
+      package="Products.GenericSetup"
+      file="meta.zcml"
+      />
+  <include
+      package="Products.Five"
+      file="meta.zcml"
+      />
+  <include package="Products.Five" />
+  <include package="plone.schemaeditor" />
+
+  <!-- dummy keyring -->
+  <utility
+      provides="plone.keyring.interfaces.IKeyManager"
+      component=".fixtures.DummyKeyManager"
+      />
+
+  <!-- dummy schema editing context -->
+  <browser:page
+      name="schemaeditor"
+      for="*"
+      class=".fixtures.DummySchemaContext"
+      allowed_interface="OFS.interfaces.IItem"
+      permission="plone.schemaeditor.ManageSchemata"
+      />
+
+  <subscriber
+      for="plone.schemaeditor.interfaces.IField
+           zope.lifecycleevent.interfaces.IObjectModifiedEvent"
+      handler=".fixtures.log_event"
+      />
+  <subscriber
+      for="plone.schemaeditor.interfaces.IField
+           zope.lifecycleevent.interfaces.IObjectMovedEvent"
+      handler=".fixtures.log_event"
+      />
+  <subscriber
+      for="zope.interface.interfaces.IInterface
+           zope.container.interfaces.IContainerModifiedEvent"
+      handler=".fixtures.log_event"
+      />
+  <subscriber
+      for="plone.schemaeditor.interfaces.ISchemaContext
+           plone.schemaeditor.interfaces.ISchemaModifiedEvent"
+      handler=".fixtures.log_event"
+      />
+
+  <!-- use a form layout that doesn't pull in main_template -->
+  <adapter factory=".tests.layout_factory" />
+
+  <!-- provide a widget renderer a la plone.app.z3cform -->
+  <browser:page
+      name="ploneform-render-widget"
+      for="z3c.form.interfaces.IWidget"
+      class=".tests.RenderWidget"
+      permission="zope2.View"
+      />
+
+  <browser:page
+      name="contexteditor"
+      for="*"
+      class=".fixtures.EditView"
+      permission="plone.schemaeditor.ManageSchemata"
+      />
+
+  <utility
+      factory=".fixtures.CountriesVocabulary"
+      provides="zope.schema.interfaces.IVocabularyFactory"
+      name="plone.schemaeditor.test.Countries"
+      />
+
+  <utility
+      factory=".fixtures.CategoriesVocabulary"
+      provides="zope.schema.interfaces.IVocabularyFactory"
+      name="plone.schemaeditor.test.Categories"
+      />
 
 </configure>
```

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/tests/choice.rst` & `plone.schemaeditor-4.0.3/plone/schemaeditor/tests/choice.rst`

 * *Files identical despite different names*

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/tests/editing.rst` & `plone.schemaeditor-4.0.3/plone/schemaeditor/tests/editing.rst`

 * *Files identical despite different names*

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/tests/extending.rst` & `plone.schemaeditor-4.0.3/plone/schemaeditor/tests/extending.rst`

 * *Files identical despite different names*

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/tests/field_schemata.rst` & `plone.schemaeditor-4.0.3/plone/schemaeditor/tests/field_schemata.rst`

 * *Files identical despite different names*

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/tests/fixtures.py` & `plone.schemaeditor-4.0.3/plone/schemaeditor/tests/fixtures.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from z3c.form.form import EditForm
 from zope import schema
 from zope.interface import Interface
 from zope.schema.vocabulary import SimpleVocabulary
 
 
 class IDummySchema(Interface):
-
     model.fieldset("alpha", fields=["fieldA"])
 
     field1 = schema.TextLine()
     field2 = schema.TextLine()
     field3 = schema.TextLine()
     field4 = schema.TextLine()
     field5 = schema.TextLine()
@@ -31,15 +30,14 @@
             event.__class__.__name__,
             object.__class__.__name__,
         )
     )  # noqa
 
 
 class EditForm(EditForm):
-
     ignoreContext = True
     ignoreRequest = True
 
     def update(self):
         self.fields = field.Fields(IDummySchema)
         super().update()
 
@@ -53,20 +51,18 @@
             SimpleVocabulary.createTerm(value, value, label)
             for value, label in self.values_list
         ]
         return SimpleVocabulary(terms)
 
 
 class CountriesVocabulary(BaseVocabulary):
-
     values_list = [("fr", "France"), ("uk", "United Kingdom"), ("es", "Spain")]
 
 
 class CategoriesVocabulary(BaseVocabulary):
-
     values_list = [("php", "PHP"), ("c", "C"), ("ruby", "Ruby")]
 
 
 class DummyKeyring:
     def random(self):
         return "a"
```

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/tests/minmax.rst` & `plone.schemaeditor-4.0.3/plone/schemaeditor/tests/minmax.rst`

 * *Files identical despite different names*

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/tests/robot/test_fields.robot` & `plone.schemaeditor-4.0.3/plone/schemaeditor/tests/robot/test_fields.robot`

 * *Files identical despite different names*

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/tests/robot_testing.zcml` & `plone.schemaeditor-4.0.3/plone/schemaeditor/tests/robot_testing.zcml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    xmlns:gs="http://namespaces.zope.org/genericsetup"
     xmlns:browser="http://namespaces.zope.org/browser"
-    i18n_domain="plone">
+    xmlns:gs="http://namespaces.zope.org/genericsetup"
+    i18n_domain="plone"
+    >
 
-    <include package="plone.schemaeditor"/>
+  <include package="plone.schemaeditor" />
 
-    <utility provides="zope.schema.interfaces.IVocabularyFactory"
-             name="plone.schemaeditor.test.Countries"
-             factory=".fixtures.CountriesVocabulary" />
+  <utility
+      factory=".fixtures.CountriesVocabulary"
+      provides="zope.schema.interfaces.IVocabularyFactory"
+      name="plone.schemaeditor.test.Countries"
+      />
 
-    <utility provides="zope.schema.interfaces.IVocabularyFactory"
-             name="plone.schemaeditor.test.Categories"
-             factory=".fixtures.CategoriesVocabulary" />
+  <utility
+      factory=".fixtures.CategoriesVocabulary"
+      provides="zope.schema.interfaces.IVocabularyFactory"
+      name="plone.schemaeditor.test.Categories"
+      />
 
 </configure>
```

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/tests/test_fields.py` & `plone.schemaeditor-4.0.3/plone/schemaeditor/tests/test_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     def __init__(self):
         self.value_type = self
 
     vocabulary = None
 
 
 class VocabularyTestCase(unittest.TestCase):
-
     layer = PLONE_FIXTURE
 
     def assertVocabulary(self, voc, values):
         self.assertTrue(IVocabularyTokenized.providedBy(voc))
         self.assertEqual([(term.value, term.token, term.title) for term in voc], values)
 
     def test_singlechoice_voc(self):
```

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/tests/test_robot.py` & `plone.schemaeditor-4.0.3/plone/schemaeditor/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/tests/tests.py` & `plone.schemaeditor-4.0.3/plone/schemaeditor/tests/tests.py`

 * *Files identical despite different names*

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/utils.py` & `plone.schemaeditor-4.0.3/plone/schemaeditor/utils.py`

 * *Files identical despite different names*

### Comparing `plone.schemaeditor-4.0.2/plone/schemaeditor/vocabularies.py` & `plone.schemaeditor-4.0.3/plone/schemaeditor/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.schemaeditor-4.0.2/plone.schemaeditor.egg-info/PKG-INFO` & `plone.schemaeditor-4.0.3/plone.schemaeditor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.schemaeditor
-Version: 4.0.2
+Version: 4.0.3
 Summary: Provides through-the-web editing of a zope schema/interface.
 Home-page: https://github.com/plone/plone.schemaeditor
 Author: David Glick
 Author-email: dglick@gmail.com
 License: BSD
 Keywords: plone schema ttw
 Classifier: Development Status :: 6 - Mature
@@ -96,14 +96,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.3 (2023-03-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (13d8d6c0)
+
+
 4.0.2 (2023-02-08)
 ------------------
 
 Bug fixes:
 
 
 - Declare all dependencies.
```

### Comparing `plone.schemaeditor-4.0.2/plone.schemaeditor.egg-info/SOURCES.txt` & `plone.schemaeditor-4.0.3/plone.schemaeditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.schemaeditor-4.0.2/pyproject.toml` & `plone.schemaeditor-4.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.schemaeditor-4.0.2/setup.py` & `plone.schemaeditor-4.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.0.2"
+version = "4.0.3"
 
 setup(
     name="plone.schemaeditor",
     version=version,
     description="Provides through-the-web editing of a zope schema/interface.",
     long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
     classifiers=[
```

