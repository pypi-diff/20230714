# Comparing `tmp/plone.api-2.0.3.tar.gz` & `tmp/plone.api-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.api-2.0.3.tar", last modified: Mon May 22 21:06:19 2023, max compression
+gzip compressed data, was "plone.api-2.0.4.tar", last modified: Fri Jul 14 10:10:14 2023, max compression
```

## Comparing `plone.api-2.0.3.tar` & `plone.api-2.0.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.108935 plone.api-2.0.3/
--rw-r--r--   0 maurits    (501) staff       (20)    21507 2023-05-22 21:06:18.000000 plone.api-2.0.3/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       73 2023-05-22 21:06:18.000000 plone.api-2.0.3/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      679 2023-05-22 21:06:18.000000 plone.api-2.0.3/LICENSE
--rw-r--r--   0 maurits    (501) staff       (20)      357 2023-05-22 21:06:18.000000 plone.api-2.0.3/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    25069 2023-05-22 21:06:19.109106 plone.api-2.0.3/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1936 2023-05-22 21:06:18.000000 plone.api-2.0.3/README.md
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.094941 plone.api-2.0.3/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     6015 2023-05-22 21:06:18.000000 plone.api-2.0.3/docs/about.md
--rw-r--r--   0 maurits    (501) staff       (20)    13950 2023-05-22 21:06:18.000000 plone.api-2.0.3/docs/content.md
--rw-r--r--   0 maurits    (501) staff       (20)     3311 2023-05-22 21:06:18.000000 plone.api-2.0.3/docs/env.md
--rw-r--r--   0 maurits    (501) staff       (20)     9491 2023-05-22 21:06:18.000000 plone.api-2.0.3/docs/group.md
--rw-r--r--   0 maurits    (501) staff       (20)     2295 2023-05-22 21:06:18.000000 plone.api-2.0.3/docs/index.md
--rw-r--r--   0 maurits    (501) staff       (20)    11162 2023-05-22 21:06:18.000000 plone.api-2.0.3/docs/portal.md
--rw-r--r--   0 maurits    (501) staff       (20)     3936 2023-05-22 21:06:18.000000 plone.api-2.0.3/docs/relation.md
--rw-r--r--   0 maurits    (501) staff       (20)    10599 2023-05-22 21:06:18.000000 plone.api-2.0.3/docs/user.md
--rw-r--r--   0 maurits    (501) staff       (20)      578 2023-05-22 21:06:18.000000 plone.api-2.0.3/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      654 2023-05-22 21:06:19.109688 plone.api-2.0.3/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2004 2023-05-22 21:06:18.000000 plone.api-2.0.3/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.088947 plone.api-2.0.3/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.095268 plone.api-2.0.3/src/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.101673 plone.api-2.0.3/src/plone/api/
--rw-r--r--   0 maurits    (501) staff       (20)      193 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)       98 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    22260 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/content.py
--rw-r--r--   0 maurits    (501) staff       (20)     8042 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/env.py
--rw-r--r--   0 maurits    (501) staff       (20)     1051 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/exc.py
--rw-r--r--   0 maurits    (501) staff       (20)    11142 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/group.py
--rw-r--r--   0 maurits    (501) staff       (20)    13908 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/portal.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.089301 plone.api-2.0.3/src/plone/api/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.102528 plone.api-2.0.3/src/plone/api/profiles/testfixture/
--rw-r--r--   0 maurits    (501) staff       (20)      229 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/profiles/testfixture/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.103026 plone.api-2.0.3/src/plone/api/profiles/testfixture/types/
--rw-r--r--   0 maurits    (501) staff       (20)     1734 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/profiles/testfixture/types/Dexterity_Folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1722 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/profiles/testfixture/types/Dexterity_Item.xml
--rw-r--r--   0 maurits    (501) staff       (20)      210 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/profiles/testfixture/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)    11553 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/relation.py
--rw-r--r--   0 maurits    (501) staff       (20)      578 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/testing.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.106701 plone.api-2.0.3/src/plone/api/tests/
--rw-r--r--   0 maurits    (501) staff       (20)      106 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/Dexterity_Folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)      106 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/Dexterity_Item.xml
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1658 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/base.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.108596 plone.api-2.0.3/src/plone/api/tests/doctests/
--rw-r--r--   0 maurits    (501) staff       (20)     6015 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/doctests/about.md
--rw-r--r--   0 maurits    (501) staff       (20)    13950 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/doctests/content.md
--rw-r--r--   0 maurits    (501) staff       (20)     3311 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/doctests/env.md
--rw-r--r--   0 maurits    (501) staff       (20)     9491 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/doctests/group.md
--rw-r--r--   0 maurits    (501) staff       (20)    11162 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/doctests/portal.md
--rw-r--r--   0 maurits    (501) staff       (20)     3936 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/doctests/relation.md
--rw-r--r--   0 maurits    (501) staff       (20)    10599 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/doctests/user.md
--rw-r--r--   0 maurits    (501) staff       (20)    48874 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/test_content.py
--rw-r--r--   0 maurits    (501) staff       (20)     3318 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)    17633 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/test_env.py
--rw-r--r--   0 maurits    (501) staff       (20)    26958 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/test_group.py
--rw-r--r--   0 maurits    (501) staff       (20)    30938 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/test_portal.py
--rw-r--r--   0 maurits    (501) staff       (20)    18992 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/test_relation.py
--rw-r--r--   0 maurits    (501) staff       (20)    35670 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/test_user.py
--rw-r--r--   0 maurits    (501) staff       (20)     9812 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/tests/test_validation.py
--rw-r--r--   0 maurits    (501) staff       (20)    14825 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/user.py
--rw-r--r--   0 maurits    (501) staff       (20)     4862 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone/api/validation.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-22 21:06:19.097850 plone.api-2.0.3/src/plone.api.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    25069 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone.api.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1682 2023-05-22 21:06:19.000000 plone.api-2.0.3/src/plone.api.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone.api.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone.api.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone.api.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      272 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone.api.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-22 21:06:18.000000 plone.api-2.0.3/src/plone.api.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     3625 2023-05-22 21:06:18.000000 plone.api-2.0.3/tox.ini
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:10:14.384624 plone.api-2.0.4/
+-rw-r--r--   0 maurits    (501) staff       (20)    22203 2023-07-14 10:10:13.000000 plone.api-2.0.4/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       73 2023-07-14 10:10:13.000000 plone.api-2.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      679 2023-07-14 10:10:13.000000 plone.api-2.0.4/LICENSE
+-rw-r--r--   0 maurits    (501) staff       (20)      357 2023-07-14 10:10:13.000000 plone.api-2.0.4/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    25765 2023-07-14 10:10:14.384750 plone.api-2.0.4/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1936 2023-07-14 10:10:13.000000 plone.api-2.0.4/README.md
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:10:14.368378 plone.api-2.0.4/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     6015 2023-07-14 10:10:13.000000 plone.api-2.0.4/docs/about.md
+-rw-r--r--   0 maurits    (501) staff       (20)    13950 2023-07-14 10:10:13.000000 plone.api-2.0.4/docs/content.md
+-rw-r--r--   0 maurits    (501) staff       (20)     3311 2023-07-14 10:10:13.000000 plone.api-2.0.4/docs/env.md
+-rw-r--r--   0 maurits    (501) staff       (20)     9491 2023-07-14 10:10:13.000000 plone.api-2.0.4/docs/group.md
+-rw-r--r--   0 maurits    (501) staff       (20)     2295 2023-07-14 10:10:13.000000 plone.api-2.0.4/docs/index.md
+-rw-r--r--   0 maurits    (501) staff       (20)    11162 2023-07-14 10:10:13.000000 plone.api-2.0.4/docs/portal.md
+-rw-r--r--   0 maurits    (501) staff       (20)     3936 2023-07-14 10:10:13.000000 plone.api-2.0.4/docs/relation.md
+-rw-r--r--   0 maurits    (501) staff       (20)    10599 2023-07-14 10:10:13.000000 plone.api-2.0.4/docs/user.md
+-rw-r--r--   0 maurits    (501) staff       (20)      578 2023-07-14 10:10:13.000000 plone.api-2.0.4/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      654 2023-07-14 10:10:14.385403 plone.api-2.0.4/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2004 2023-07-14 10:10:13.000000 plone.api-2.0.4/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:10:14.362448 plone.api-2.0.4/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:10:14.368716 plone.api-2.0.4/src/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:10:14.375260 plone.api-2.0.4/src/plone/api/
+-rw-r--r--   0 maurits    (501) staff       (20)      193 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)       98 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    22260 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/content.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8042 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/env.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1051 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/exc.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11142 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/group.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14057 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/portal.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:10:14.362852 plone.api-2.0.4/src/plone/api/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:10:14.376072 plone.api-2.0.4/src/plone/api/profiles/testfixture/
+-rw-r--r--   0 maurits    (501) staff       (20)      229 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/profiles/testfixture/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:10:14.377021 plone.api-2.0.4/src/plone/api/profiles/testfixture/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     1734 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/profiles/testfixture/types/Dexterity_Folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1722 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/profiles/testfixture/types/Dexterity_Item.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      210 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/profiles/testfixture/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)    11553 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/relation.py
+-rw-r--r--   0 maurits    (501) staff       (20)      578 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/testing.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:10:14.381912 plone.api-2.0.4/src/plone/api/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)      106 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/tests/Dexterity_Folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      106 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/tests/Dexterity_Item.xml
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1658 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/tests/base.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:10:14.384240 plone.api-2.0.4/src/plone/api/tests/doctests/
+-rw-r--r--   0 maurits    (501) staff       (20)     6015 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/tests/doctests/about.md
+-rw-r--r--   0 maurits    (501) staff       (20)    13950 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/tests/doctests/content.md
+-rw-r--r--   0 maurits    (501) staff       (20)     3311 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/tests/doctests/env.md
+-rw-r--r--   0 maurits    (501) staff       (20)     9491 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/tests/doctests/group.md
+-rw-r--r--   0 maurits    (501) staff       (20)    11162 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/tests/doctests/portal.md
+-rw-r--r--   0 maurits    (501) staff       (20)     3936 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/tests/doctests/relation.md
+-rw-r--r--   0 maurits    (501) staff       (20)    10599 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/tests/doctests/user.md
+-rw-r--r--   0 maurits    (501) staff       (20)    48845 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/tests/test_content.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3318 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17633 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/tests/test_env.py
+-rw-r--r--   0 maurits    (501) staff       (20)    26958 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/tests/test_group.py
+-rw-r--r--   0 maurits    (501) staff       (20)    30938 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/tests/test_portal.py
+-rw-r--r--   0 maurits    (501) staff       (20)    18992 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/tests/test_relation.py
+-rw-r--r--   0 maurits    (501) staff       (20)    35670 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/tests/test_user.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9812 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/tests/test_validation.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14825 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/user.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4862 2023-07-14 10:10:13.000000 plone.api-2.0.4/src/plone/api/validation.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-14 10:10:14.371161 plone.api-2.0.4/src/plone.api.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    25765 2023-07-14 10:10:14.000000 plone.api-2.0.4/src/plone.api.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1682 2023-07-14 10:10:14.000000 plone.api-2.0.4/src/plone.api.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-14 10:10:14.000000 plone.api-2.0.4/src/plone.api.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-07-14 10:10:14.000000 plone.api-2.0.4/src/plone.api.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-14 10:10:14.000000 plone.api-2.0.4/src/plone.api.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      272 2023-07-14 10:10:14.000000 plone.api-2.0.4/src/plone.api.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-07-14 10:10:14.000000 plone.api-2.0.4/src/plone.api.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3625 2023-07-14 10:10:13.000000 plone.api-2.0.4/tox.ini
```

### Comparing `plone.api-2.0.3/CHANGES.rst` & `plone.api-2.0.4/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,38 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.4 (2023-07-14)
+------------------
+
+Bug fixes:
+
+
+- Do not run GitHub Actions tests twice.
+  Only run GitHub Actions tests when commiting directly against master or main or
+  opening a pull request agains master or main. This avoids to run the same test
+  suite for the same environment twice.
+  [thet] (#0)
+- Mockup TinyMCE settings: Remove unused AtD related views.
+
+  Fix a test which was checking for "checkDocument" among other available views.
+  "checkDocument" was a TinyMCE endpoint for unmaintained "After the Deadline"
+  plugin, which is now removed. (#504)
+
+
+Documentation:
+
+
+- Enhance API docs of `portal.translate` to show that the domain is optional in some cases. @thet (#510)
+
+
 2.0.3 (2023-05-22)
 ------------------
 
 Bug fixes:
 
 
 - Create relation only if there is no existing one with same source, target, relationname.
```

### Comparing `plone.api-2.0.3/LICENSE` & `plone.api-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/PKG-INFO` & `plone.api-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.api
-Version: 2.0.3
+Version: 2.0.4
 Summary: A Plone API.
 Home-page: https://github.com/plone/plone.api
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone api
 Platform: Any
@@ -79,14 +79,38 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.4 (2023-07-14)
+------------------
+
+Bug fixes:
+
+
+- Do not run GitHub Actions tests twice.
+  Only run GitHub Actions tests when commiting directly against master or main or
+  opening a pull request agains master or main. This avoids to run the same test
+  suite for the same environment twice.
+  [thet] (#0)
+- Mockup TinyMCE settings: Remove unused AtD related views.
+
+  Fix a test which was checking for "checkDocument" among other available views.
+  "checkDocument" was a TinyMCE endpoint for unmaintained "After the Deadline"
+  plugin, which is now removed. (#504)
+
+
+Documentation:
+
+
+- Enhance API docs of `portal.translate` to show that the domain is optional in some cases. @thet (#510)
+
+
 2.0.3 (2023-05-22)
 ------------------
 
 Bug fixes:
 
 
 - Create relation only if there is no existing one with same source, target, relationname.
```

### Comparing `plone.api-2.0.3/README.md` & `plone.api-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/docs/about.md` & `plone.api-2.0.4/docs/about.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/docs/content.md` & `plone.api-2.0.4/docs/content.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/docs/env.md` & `plone.api-2.0.4/docs/env.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/docs/group.md` & `plone.api-2.0.4/docs/group.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/docs/index.md` & `plone.api-2.0.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/docs/portal.md` & `plone.api-2.0.4/docs/portal.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/docs/relation.md` & `plone.api-2.0.4/docs/relation.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/docs/user.md` & `plone.api-2.0.4/docs/user.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/pyproject.toml` & `plone.api-2.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/setup.cfg` & `plone.api-2.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/setup.py` & `plone.api-2.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
 long_description = (
     read("README.md") + "\n\n" + read("CHANGES.rst") + "\n\n" + read("LICENSE")
 )
 
-version = "2.0.3"
+version = "2.0.4"
 
 setup(
     name="plone.api",
     version=version,
     description="A Plone API.",
     long_description=long_description,
     author="Plone Foundation",
```

### Comparing `plone.api-2.0.3/src/plone/api/content.py` & `plone.api-2.0.4/src/plone/api/content.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/env.py` & `plone.api-2.0.4/src/plone/api/env.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/exc.py` & `plone.api-2.0.4/src/plone/api/exc.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/group.py` & `plone.api-2.0.4/src/plone/api/group.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/portal.py` & `plone.api-2.0.4/src/plone/api/portal.py`

 * *Files 2% similar despite different names*

```diff
@@ -404,15 +404,17 @@
 def translate(msgid, domain="plone", lang=None):
     """Translate a message into a given language.
 
     Default to current negotiated language if no target language specified.
 
     :param msgid: [required] message to translate
     :type msgid: string
-    :param domain: i18n domain to use
+    :type msgid: zope.i18nmessageid.Message
+    :param domain: i18n domain to use. When ``msgid`` is an instance of ``Message``,
+                   then the ``Message``'s domain is used.
     :type domain: string
     :param lang: target language
     :type lang: string
     :returns: translated message
     :rtype: str
     :Example: :ref:`portal-translate-example`
     """
```

### Comparing `plone.api-2.0.3/src/plone/api/profiles/testfixture/types/Dexterity_Folder.xml` & `plone.api-2.0.4/src/plone/api/profiles/testfixture/types/Dexterity_Folder.xml`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/profiles/testfixture/types/Dexterity_Item.xml` & `plone.api-2.0.4/src/plone/api/profiles/testfixture/types/Dexterity_Item.xml`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/relation.py` & `plone.api-2.0.4/src/plone/api/relation.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/testing.zcml` & `plone.api-2.0.4/src/plone/api/testing.zcml`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/tests/base.py` & `plone.api-2.0.4/src/plone/api/tests/base.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/tests/doctests/about.md` & `plone.api-2.0.4/src/plone/api/tests/doctests/about.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/tests/doctests/content.md` & `plone.api-2.0.4/src/plone/api/tests/doctests/content.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/tests/doctests/env.md` & `plone.api-2.0.4/src/plone/api/tests/doctests/env.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/tests/doctests/group.md` & `plone.api-2.0.4/src/plone/api/tests/doctests/group.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/tests/doctests/portal.md` & `plone.api-2.0.4/src/plone/api/tests/doctests/portal.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/tests/doctests/relation.md` & `plone.api-2.0.4/src/plone/api/tests/doctests/relation.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/tests/doctests/user.md` & `plone.api-2.0.4/src/plone/api/tests/doctests/user.md`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/tests/test_content.py` & `plone.api-2.0.4/src/plone/api/tests/test_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -1402,15 +1402,14 @@
 
         # This is just a sampling of views that should be present.
         # Test against only these rather than the full list. Otherwise, this
         # test has to maintain an up-to-date list of every view in Plone.
         should_be_theres = (
             "adapter",
             "authenticator",
-            "checkDocument",
             "get_macros",
             "history",
             "plone",
             "plone_tools",
             "resource",
             "search",
             "sharing",
```

### Comparing `plone.api-2.0.3/src/plone/api/tests/test_doctests.py` & `plone.api-2.0.4/src/plone/api/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/tests/test_env.py` & `plone.api-2.0.4/src/plone/api/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/tests/test_group.py` & `plone.api-2.0.4/src/plone/api/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/tests/test_portal.py` & `plone.api-2.0.4/src/plone/api/tests/test_portal.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/tests/test_relation.py` & `plone.api-2.0.4/src/plone/api/tests/test_relation.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/tests/test_user.py` & `plone.api-2.0.4/src/plone/api/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/tests/test_validation.py` & `plone.api-2.0.4/src/plone/api/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/user.py` & `plone.api-2.0.4/src/plone/api/user.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone/api/validation.py` & `plone.api-2.0.4/src/plone/api/validation.py`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/src/plone.api.egg-info/PKG-INFO` & `plone.api-2.0.4/src/plone.api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.api
-Version: 2.0.3
+Version: 2.0.4
 Summary: A Plone API.
 Home-page: https://github.com/plone/plone.api
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone api
 Platform: Any
@@ -79,14 +79,38 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.0.4 (2023-07-14)
+------------------
+
+Bug fixes:
+
+
+- Do not run GitHub Actions tests twice.
+  Only run GitHub Actions tests when commiting directly against master or main or
+  opening a pull request agains master or main. This avoids to run the same test
+  suite for the same environment twice.
+  [thet] (#0)
+- Mockup TinyMCE settings: Remove unused AtD related views.
+
+  Fix a test which was checking for "checkDocument" among other available views.
+  "checkDocument" was a TinyMCE endpoint for unmaintained "After the Deadline"
+  plugin, which is now removed. (#504)
+
+
+Documentation:
+
+
+- Enhance API docs of `portal.translate` to show that the domain is optional in some cases. @thet (#510)
+
+
 2.0.3 (2023-05-22)
 ------------------
 
 Bug fixes:
 
 
 - Create relation only if there is no existing one with same source, target, relationname.
```

### Comparing `plone.api-2.0.3/src/plone.api.egg-info/SOURCES.txt` & `plone.api-2.0.4/src/plone.api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.api-2.0.3/tox.ini` & `plone.api-2.0.4/tox.ini`

 * *Files identical despite different names*

