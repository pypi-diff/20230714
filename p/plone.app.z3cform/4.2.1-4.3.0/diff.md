# Comparing `tmp/plone.app.z3cform-4.2.1.tar.gz` & `tmp/plone.app.z3cform-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.z3cform-4.2.1.tar", last modified: Fri Jun 16 16:50:58 2023, max compression
+gzip compressed data, was "plone.app.z3cform-4.3.0.tar", last modified: Thu Jul 13 22:10:35 2023, max compression
```

## Comparing `plone.app.z3cform-4.2.1.tar` & `plone.app.z3cform-4.3.0.tar`

### file list

```diff
@@ -1,103 +1,105 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:50:57.996962 plone.app.z3cform-4.2.1/
--rw-r--r--   0 maurits    (501) staff       (20)    25399 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      146 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    48652 2023-06-16 16:50:57.997105 plone.app.z3cform-4.2.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)    13825 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:50:57.972939 plone.app.z3cform-4.2.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      749 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:50:57.973241 plone.app.z3cform-4.2.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:50:57.975758 plone.app.z3cform-4.2.1/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:50:57.980489 plone.app.z3cform-4.2.1/plone/app/z3cform/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2763 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    18540 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/converters.py
--rw-r--r--   0 maurits    (501) staff       (20)     1310 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/converters.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      724 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/csrf.py
--rw-r--r--   0 maurits    (501) staff       (20)      110 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/factories.py
--rw-r--r--   0 maurits    (501) staff       (20)     2349 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/inline_validation.py
--rw-r--r--   0 maurits    (501) staff       (20)     7482 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/inline_validation.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2500 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      212 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/layout.py
--rw-r--r--   0 maurits    (501) staff       (20)      152 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/overrides.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:50:57.969503 plone.app.z3cform-4.2.1/plone/app/z3cform/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:50:57.981106 plone.app.z3cform-4.2.1/plone/app/z3cform/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      163 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)       85 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      635 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/profiles.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:50:57.989330 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     1013 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/ajaxselect_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3643 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/checkbox_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      140 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/contentprovider-widget.pt
--rw-r--r--   0 maurits    (501) staff       (20)      209 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/error.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4806 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/file_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      829 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/form.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4798 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/image_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      677 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/layout.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3547 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/link_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     9551 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/macros.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4033 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/multi_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1861 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/object_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5558 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/orderedselect_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1448 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/password_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      650 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/radio_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1418 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/radio_input_single.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1869 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/relateditems_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1937 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/select_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      976 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/singlecheckbox.pt
--rw-r--r--   0 maurits    (501) staff       (20)      765 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/singlecheckboxbool_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1357 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/singlecheckboxbool_hidden.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4046 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/singlecheckboxbool_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1335 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/submit_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1574 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/text_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1414 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/textarea_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3703 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/textfield_widget_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1356 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/textlines_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1812 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/templates/widget.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:50:57.992312 plone.app.z3cform-4.2.1/plone/app/z3cform/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2421 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/tests/example.py
--rw-r--r--   0 maurits    (501) staff       (20)     1139 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/tests/layer.py
--rw-r--r--   0 maurits    (501) staff       (20)      907 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/tests/test_csrf.py
--rw-r--r--   0 maurits    (501) staff       (20)    17512 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/tests/test_patterns.py
--rw-r--r--   0 maurits    (501) staff       (20)     4921 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1349 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/tests/test_widget.py
--rw-r--r--   0 maurits    (501) staff       (20)    67618 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/tests/test_widgets.py
--rw-r--r--   0 maurits    (501) staff       (20)      776 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/tests/testing.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2208 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/tests/tests.py
--rw-r--r--   0 maurits    (501) staff       (20)     6163 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     2739 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/views.py
--rw-r--r--   0 maurits    (501) staff       (20)     2959 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/widget.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:50:57.995065 plone.app.z3cform-4.2.1/plone/app/z3cform/widgets/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/widgets/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1807 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/widgets/base.py
--rw-r--r--   0 maurits    (501) staff       (20)     4970 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/widgets/datetime.py
--rw-r--r--   0 maurits    (501) staff       (20)     1978 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/widgets/link.py
--rw-r--r--   0 maurits    (501) staff       (20)     9722 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/widgets/patterns.py
--rw-r--r--   0 maurits    (501) staff       (20)     2712 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/widgets/querystring.py
--rw-r--r--   0 maurits    (501) staff       (20)     8804 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/widgets/relateditems.py
--rw-r--r--   0 maurits    (501) staff       (20)     6381 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/widgets/richtext.py
--rw-r--r--   0 maurits    (501) staff       (20)    11155 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/widgets/select.py
--rw-r--r--   0 maurits    (501) staff       (20)     2962 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/widgets/singlecheckbox.py
--rw-r--r--   0 maurits    (501) staff       (20)     9303 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/widgets.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:50:57.996641 plone.app.z3cform-4.2.1/plone/app/z3cform/wysiwyg/
--rw-r--r--   0 maurits    (501) staff       (20)      919 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/wysiwyg/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      127 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/wysiwyg/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      639 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/wysiwyg/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1693 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/wysiwyg/widget.py
--rw-r--r--   0 maurits    (501) staff       (20)      601 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/wysiwyg/wysiwyg_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1048 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone/app/z3cform/wysiwyg/wysiwyg_input.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:50:57.975463 plone.app.z3cform-4.2.1/plone.app.z3cform.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    48652 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone.app.z3cform.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3335 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone.app.z3cform.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone.app.z3cform.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone.app.z3cform.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone.app.z3cform.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      578 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone.app.z3cform.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/plone.app.z3cform.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1692 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      242 2023-06-16 16:50:57.997579 plone.app.z3cform-4.2.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2625 2023-06-16 16:50:57.000000 plone.app.z3cform-4.2.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 22:10:35.319877 plone.app.z3cform-4.3.0/
+-rw-r--r--   0 maurits    (501) staff       (20)    25853 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      146 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    49142 2023-07-13 22:10:35.319568 plone.app.z3cform-4.3.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)    13825 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 22:10:35.293222 plone.app.z3cform-4.3.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      749 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 22:10:35.293473 plone.app.z3cform-4.3.0/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 22:10:35.296090 plone.app.z3cform-4.3.0/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 22:10:35.300969 plone.app.z3cform-4.3.0/plone/app/z3cform/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2763 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    18540 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/converters.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1310 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/converters.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      724 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/csrf.py
+-rw-r--r--   0 maurits    (501) staff       (20)      110 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/factories.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2349 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/inline_validation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7482 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/inline_validation.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2589 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      212 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/layout.py
+-rw-r--r--   0 maurits    (501) staff       (20)      152 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/overrides.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 22:10:35.289291 plone.app.z3cform-4.3.0/plone/app/z3cform/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 22:10:35.301728 plone.app.z3cform-4.3.0/plone/app/z3cform/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      163 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      635 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/profiles.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 22:10:35.310466 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)     1013 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/ajaxselect_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3643 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/checkbox_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      140 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/contentprovider-widget.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1575 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/email_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      209 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/error.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4806 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/file_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      829 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4798 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/image_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      677 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/layout.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3686 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/link_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     9579 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/macros.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4033 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/multi_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1861 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/object_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5202 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/orderedselect_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1448 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/password_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      650 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/radio_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1418 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/radio_input_single.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1869 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/relateditems_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1937 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/select_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      976 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/singlecheckbox.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      765 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/singlecheckboxbool_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1357 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/singlecheckboxbool_hidden.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4046 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/singlecheckboxbool_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1335 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/submit_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1574 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/text_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1414 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/textarea_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3703 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/textfield_widget_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1356 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/textlines_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1812 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/templates/widget.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 22:10:35.314060 plone.app.z3cform-4.3.0/plone/app/z3cform/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2421 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/tests/example.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1139 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/tests/layer.py
+-rw-r--r--   0 maurits    (501) staff       (20)      907 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/tests/test_csrf.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17512 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/tests/test_patterns.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4921 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1349 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/tests/test_widget.py
+-rw-r--r--   0 maurits    (501) staff       (20)    67601 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/tests/test_widgets.py
+-rw-r--r--   0 maurits    (501) staff       (20)      776 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/tests/testing.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2208 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/tests/tests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6162 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2739 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/views.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2959 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/widget.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 22:10:35.317496 plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1807 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4970 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/datetime.py
+-rw-r--r--   0 maurits    (501) staff       (20)      528 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/email.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1978 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/link.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9722 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/patterns.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2712 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/querystring.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8803 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/relateditems.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6381 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/richtext.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11155 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/select.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2962 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/singlecheckbox.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9658 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/widgets.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 22:10:35.319221 plone.app.z3cform-4.3.0/plone/app/z3cform/wysiwyg/
+-rw-r--r--   0 maurits    (501) staff       (20)      919 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/wysiwyg/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      127 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/wysiwyg/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      639 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/wysiwyg/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1693 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/wysiwyg/widget.py
+-rw-r--r--   0 maurits    (501) staff       (20)      601 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/wysiwyg/wysiwyg_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1048 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/plone/app/z3cform/wysiwyg/wysiwyg_input.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 22:10:35.295843 plone.app.z3cform-4.3.0/plone.app.z3cform.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    49142 2023-07-13 22:10:35.000000 plone.app.z3cform-4.3.0/plone.app.z3cform.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3403 2023-07-13 22:10:35.000000 plone.app.z3cform-4.3.0/plone.app.z3cform.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-13 22:10:35.000000 plone.app.z3cform-4.3.0/plone.app.z3cform.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-07-13 22:10:35.000000 plone.app.z3cform-4.3.0/plone.app.z3cform.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-13 22:10:35.000000 plone.app.z3cform-4.3.0/plone.app.z3cform.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      593 2023-07-13 22:10:35.000000 plone.app.z3cform-4.3.0/plone.app.z3cform.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-07-13 22:10:35.000000 plone.app.z3cform-4.3.0/plone.app.z3cform.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4244 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-07-13 22:10:35.319997 plone.app.z3cform-4.3.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2751 2023-07-13 22:10:34.000000 plone.app.z3cform-4.3.0/setup.py
```

### Comparing `plone.app.z3cform-4.2.1/CHANGES.rst` & `plone.app.z3cform-4.3.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,41 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.3.0 (2023-07-14)
+------------------
+
+New features:
+
+
+- Introduce new Email-Widget which is used for `plone.schema.email.IEmail` fields.
+  It uses the input type `email`.
+  [jensens] (#173)
+
+
+Bug fixes:
+
+
+- Fix OrdereSelectWidget browser validation when the input is required.
+  [petschki] (#178)
+- Ignore form validation when `ignoreRequiredOnExtract` is set.
+  [petschki] (#179)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (cfffba8c)
+
+
 4.2.1 (2023-06-16)
 ------------------
 
 Bug fixes:
 
 
 - Add `required` to orderedselect widget.
```

### Comparing `plone.app.z3cform-4.2.1/PKG-INFO` & `plone.app.z3cform-4.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.z3cform
-Version: 4.2.1
+Version: 4.3.0
 Summary: A collection of widgets, templates and other components for use with z3c.form and Plone
 Home-page: https://pypi.org/project/plone.app.z3cform
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: zope plone form widget template
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,14 +17,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: tests
 
 =================
 plone.app.z3cform
 =================
 
@@ -677,14 +678,41 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.3.0 (2023-07-14)
+------------------
+
+New features:
+
+
+- Introduce new Email-Widget which is used for `plone.schema.email.IEmail` fields.
+  It uses the input type `email`.
+  [jensens] (#173)
+
+
+Bug fixes:
+
+
+- Fix OrdereSelectWidget browser validation when the input is required.
+  [petschki] (#178)
+- Ignore form validation when `ignoreRequiredOnExtract` is set.
+  [petschki] (#179)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (cfffba8c)
+
+
 4.2.1 (2023-06-16)
 ------------------
 
 Bug fixes:
 
 
 - Add `required` to orderedselect widget.
@@ -1817,8 +1845,7 @@
 
 
 0.3 - 2008-07-24
 ----------------
 
 - Create this package from Plone-specific bits that have been factored
   out of plone.z3cform.
-
```

### Comparing `plone.app.z3cform-4.2.1/README.rst` & `plone.app.z3cform-4.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/docs/LICENSE.GPL` & `plone.app.z3cform-4.3.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/docs/LICENSE.txt` & `plone.app.z3cform-4.3.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/configure.zcml` & `plone.app.z3cform-4.3.0/plone/app/z3cform/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/converters.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/converters.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/converters.zcml` & `plone.app.z3cform-4.3.0/plone/app/z3cform/converters.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/csrf.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/csrf.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/inline_validation.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/inline_validation.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/inline_validation.rst` & `plone.app.z3cform-4.3.0/plone/app/z3cform/inline_validation.rst`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/interfaces.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,14 +66,18 @@
     """Marker interface for the TinyMCEWidget."""
 
 
 class ILinkWidget(ITextWidget):
     """Marker interface for the enhanced link widget."""
 
 
+class IEmailWidget(ITextWidget):
+    """Marker interface for the dumb email widget."""
+
+
 class ISingleCheckBoxBoolWidget(ISingleCheckBoxWidget):
     """Marker interface for the SingleCheckboxBoolWidget."""
 
 
 class IRadioWidget(IRadioWidget):
     """Radio widget."""
```

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/profiles.zcml` & `plone.app.z3cform-4.3.0/plone/app/z3cform/profiles.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/ajaxselect_display.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/ajaxselect_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/checkbox_input.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/checkbox_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/file_input.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/file_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/form.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/form.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/image_input.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/image_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/layout.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/layout.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/link_input.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/link_input.pt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,16 @@
-<div i18n:domain="plone">
+<div xmlns="http://www.w3.org/1999/xhtml"
+     xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+     xmlns:metal="http://xml.zope.org/namespaces/metal"
+     xmlns:tal="http://xml.zope.org/namespaces/tal"
+     lang="en"
+     xml:lang="en"
+     i18n:domain="plone"
+>
+
   <div class="linkModal">
 
     <div class="pat-autotoc autotabs"
          data-pat-autotoc="section:span.linkType;levels:span.linkLabel;"
     >
 
       <span class="linkType internal"
@@ -47,21 +55,19 @@
         >External</span>
         <div class="mb-3 main">
           <label class="form-label"
                  for="external"
                  i18n:translate="help_external_url"
           >External URL (can be relative within this site or absolute if it starts with http:// or https://)</label>
           <input class="form-control"
-                 name="external"
+                 name="${view/name}.external"
                  placeholder="https://domain.com"
                  type="text"
-                 tal:attributes="
-                   name string:${view/name}.external;
-                   value value;
-                 "
+                 value="${value}"
+                 i18n:attributes="placeholder"
           />
         </div>
       </span>
 
       <span class="linkType email"
             data-linktype="email"
             tal:define="
@@ -76,32 +82,30 @@
         >Email</span>
         <div class="form-inline">
           <div class="mb-3 main">
             <label class="form-label"
                    i18n:translate="help_email_url"
             >Email Address</label>
             <input class="form-control"
-                   name="email"
+                   name="${view/name}.email"
                    placeholder="name@domain.com"
                    type="email"
-                   tal:attributes="
-                     name string:${view/name}.email;
-                     value value;
-                   "
+                   value="${value}"
+                   i18n:attributes="placeholder"
             />
           </div>
           <div class="mb-3">
             <label class="form-label"
                    i18n:translate="help_email_url_subject"
             >Email Subject (optional)</label>
             <input class="form-control"
-                   name="subject"
+                   name="${view/name}.subject"
                    type="text"
-                   tal:attributes="
-                     name string:${view/name}.subject;
+                   value="${value}"
+                   tal:define="
                      value view/value/email_subject | nothing;
                    "
             />
           </div>
         </div>
       </span>
```

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/macros.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/macros.pt`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
                 form_class view/css_class | string:;
                 default_fieldset_label view/default_fieldset_label | form_name;
                 enable_form_tabbing view/enable_form_tabbing | python:True;
                 enable_unload_protection view/enable_unload_protection|python:True;
                 unload_protection python:enable_unload_protection and 'pat-formunloadalert';
                 enable_autofocus view/enable_autofocus|python:True;
                 autofocus python:enable_autofocus and 'pat-formautofocus';
-                validation python:'pat-validation' if True else '';
+                validation python:'pat-validation' if not view.ignoreRequiredOnExtract else '';
                 has_groups python:bool(groups);
                 form_tabbing python:(has_groups and enable_form_tabbing) and 'enableFormTabbing pat-autotoc' or '';
                 show_default_label python:has_groups and default_fieldset_label and len(view.widgets);
                 form_view_name_raw python:view.__name__ or request.getURL().split('/')[-1];
                 form_view_name python:'-'.join(['view', 'name'] + [x for x in form_view_name_raw.split('++') if x]);
               "
               tal:attributes="
```

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/multi_input.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/multi_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/object_input.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/object_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/orderedselect_input.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/orderedselect_input.pt`

 * *Files 23% similar despite different names*

```diff
@@ -3,51 +3,43 @@
       xmlns:tal="http://xml.zope.org/namespaces/tal"
       tal:omit-tag=""
 >
   <script src="++resource++orderedselect_input.js"
           type="text/javascript"
   ></script>
 
-  <table class="ordered-selection-field"
+  <table class="ordered-selection-field table table-borderless"
+         id="${view/id}"
          border="0"
-         tal:attributes="
-           id view/id;
-         "
   >
     <tr>
       <td>
-        <select class=""
-                id="from"
-                name="from"
-                size="5"
-                tal:attributes="
-                  id string:${view/id}-from;
-                  name string:${view/name}.from;
-                  class string:form-control ${view/klass};
-                  style view/style;
-                  title view/title;
-                  lang view/lang;
-                  onclick view/onclick;
-                  ondblclick view/ondblclick;
-                  onmousedown view/onmousedown;
-                  onmouseup view/onmouseup;
-                  onmouseover view/onmouseover;
-                  onmousemove view/onmousemove;
-                  onmouseout view/onmouseout;
-                  onkeypress view/onkeypress;
-                  onkeydown view/onkeydown;
-                  onkeyup view/onkeyup;
-                  disabled view/disabled;
-                  tabindex view/tabindex;
-                  onfocus view/onfocus;
-                  onblur view/onblur;
-                  onchange view/onchange;
-                  multiple view/multiple;
-                  size view/size;
-                "
+        <select class="form-control ${view/klass}"
+                id="${view/id}-from"
+                disabled="${view/disabled}"
+                lang="${view/lang}"
+                multiple="${view/multiple}"
+                name="${view/name}.from"
+                onblur="${view/onblur}"
+                onchange="${view/onchange}"
+                onclick="${view/onclick}"
+                ondblclick="${view/ondblclick}"
+                onfocus="${view/onfocus}"
+                onkeydown="${view/onkeydown}"
+                onkeypress="${view/onkeypress}"
+                onkeyup="${view/onkeyup}"
+                onmousedown="${view/onmousedown}"
+                onmousemove="${view/onmousemove}"
+                onmouseout="${view/onmouseout}"
+                onmouseover="${view/onmouseover}"
+                onmouseup="${view/onmouseup}"
+                size="${view/size}"
+                style="${view/style}"
+                tabindex="${view/tabindex}"
+                title="${view/title}"
         >
           <option tal:repeat="entry view/notselectedItems"
                   tal:content="nocall:entry/content"
                   tal:attributes="
                     value entry/value;
                   "
                   i18n:translate=""
@@ -72,46 +64,41 @@
                 value="&larr;"
                 tal:attributes="
                   onClick string:javascript:to2from('${view/id}');
                 "
         >&larr;</button>
       </td>
       <td>
-        <select class=""
-                id="to"
-                name="to"
-                size="5"
-                tal:attributes="
-                  id string:${view/id}-to;
-                  name string:${view/name}.to;
-                  class string:form-control ${view/klass};
-                  style view/style;
-                  title view/title;
-                  lang view/lang;
-                  onclick view/onclick;
-                  ondblclick view/ondblclick;
-                  onmousedown view/onmousedown;
-                  onmouseup view/onmouseup;
-                  onmouseover view/onmouseover;
-                  onmousemove view/onmousemove;
-                  onmouseout view/onmouseout;
-                  onkeypress view/onkeypress;
-                  onkeydown view/onkeydown;
-                  onkeyup view/onkeyup;
-                  disabled view/disabled;
-                  tabindex view/tabindex;
-                  onfocus view/onfocus;
-                  onblur view/onblur;
-                  onchange view/onchange;
-                  multiple view/multiple;
-                  size view/size;
-                  required python:view.required and 'required' or None;
-                "
+        <select class="form-select ${view/klass}"
+                id="${view/id}-to"
+                disabled="${view/disabled}"
+                lang="${view/lang}"
+                multiple="${view/multiple}"
+                name="${view/name}.to"
+                onblur="${view/onblur}"
+                onchange="${view/onchange}"
+                onclick="${view/onclick}"
+                ondblclick="${view/ondblclick}"
+                onfocus="${view/onfocus}"
+                onkeydown="${view/onkeydown}"
+                onkeypress="${view/onkeypress}"
+                onkeyup="${view/onkeyup}"
+                onmousedown="${view/onmousedown}"
+                onmousemove="${view/onmousemove}"
+                onmouseout="${view/onmouseout}"
+                onmouseover="${view/onmouseover}"
+                onmouseup="${view/onmouseup}"
+                required="${python:view.required and 'required' or None}"
+                size="${view/size}"
+                style="${view/style}"
+                tabindex="${view/tabindex}"
+                title="${view/title}"
         >
-          <option tal:repeat="entry view/selectedItems"
+          <option selected="selected"
+                  tal:repeat="entry view/selectedItems"
                   tal:content="nocall:entry/content"
                   tal:attributes="
                     value entry/value;
                   "
                   i18n:translate=""
           ></option>
         </select>
@@ -126,18 +113,15 @@
               tal:attributes="
                 id string:${view/id}-toDataContainer;
               "
         >
           <script type="text/javascript"
                   tal:content="string:copyDataForSubmit('${view/id}');"
           >
-          /*  <![CDATA[ */
           // initial copying of field "field.to" --> "field"
-          copyDataForSubmit("<i tal:replace="${view/id}"/>");
-          /* ]]> */
           </script>
         </span>
       </td>
       <td>
         <button class="btn btn-sm btn-outline-secondary"
                 name="upButton"
                 onclick="javascript:moveUp()"
```

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/password_input.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/password_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/radio_input.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/radio_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/radio_input_single.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/radio_input_single.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/relateditems_display.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/relateditems_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/select_input.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/select_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/singlecheckbox.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/singlecheckbox.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/singlecheckboxbool_display.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/singlecheckboxbool_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/singlecheckboxbool_hidden.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/singlecheckboxbool_hidden.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/singlecheckboxbool_input.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/singlecheckboxbool_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/submit_input.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/submit_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/text_input.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/text_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/textarea_input.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/textarea_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/textfield_widget_input.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/textfield_widget_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/textlines_input.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/textlines_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/templates/widget.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/templates/widget.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/tests/example.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/tests/example.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/tests/layer.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/tests/layer.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/tests/test_csrf.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/tests/test_csrf.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/tests/test_patterns.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/tests/test_utils.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/tests/test_widget.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/tests/test_widgets.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/tests/test_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1283,16 +1283,16 @@
         )
         self.assertEqual(
             EXPECTED_VOCAB_URL,
             result["pattern_options"]["vocabularyUrl"],
         )
 
     def test_related_items_widget_nav_root(self):
-        from plone.app.layout.navigation.interfaces import INavigationRoot
         from plone.app.z3cform.widgets.relateditems import RelatedItemsWidget
+        from plone.base.interfaces import INavigationRoot
 
         EXPECTED_ROOT_PATH = "/plone"
         EXPECTED_ROOT_URL = "http://nohost/plone"
         EXPECTED_BASE_PATH = "/plone/subfolder"
         EXPECTED_VOCAB_URL = "http://nohost/plone/@@getVocabulary?name=plone.app.vocabularies.Catalog"  # noqa
 
         self.portal.invokeFactory("Folder", "subfolder")
```

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/tests/testing.zcml` & `plone.app.z3cform-4.3.0/plone/app/z3cform/tests/testing.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/tests/tests.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/tests/tests.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/utils.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from Acquisition import aq_base
 from copy import deepcopy
-from plone.app.layout.navigation.root import getNavigationRootObject
+from plone.base.navigationroot import get_navigation_root_object
 from Products.CMFCore.interfaces import IContentish
 from Products.CMFCore.interfaces import IFolderish
 from Products.CMFCore.interfaces import ISiteRoot
 from z3c.form.interfaces import IForm
 from zope.component import providedBy
 from zope.component.hooks import getSite
 from zope.globalrequest import getRequest
@@ -155,15 +155,15 @@
             if ISiteRoot in providedBy(potential_portal):
                 return potential_portal
 
 
 def get_portal_url(context):
     portal = get_portal()
     if portal:
-        root = getNavigationRootObject(context, portal)
+        root = get_navigation_root_object(context, portal)
         if root:
             try:
                 return root.absolute_url()
             except AttributeError:
                 return portal.absolute_url()
         else:
             return portal.absolute_url()
```

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/views.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/views.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/widget.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/widget.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/widgets/base.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/base.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/widgets/datetime.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/datetime.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/widgets/link.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/link.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/widgets/patterns.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/patterns.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/widgets/querystring.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/querystring.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/widgets/relateditems.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/relateditems.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from Acquisition import aq_parent
 from OFS.interfaces import IFolder
 from OFS.interfaces import ISimpleItem
 from plone.app.contentlisting.interfaces import IContentListing
-from plone.app.layout.navigation.root import getNavigationRootObject
 from plone.app.z3cform.interfaces import IRelatedItemsWidget
 from plone.app.z3cform.utils import dict_merge
 from plone.app.z3cform.utils import get_context_url
 from plone.app.z3cform.utils import get_widget_form
 from plone.app.z3cform.widgets.base import BaseWidget
 from plone.app.z3cform.widgets.patterns import InputWidget
 from plone.base import PloneMessageFactory as _
+from plone.base.navigationroot import get_navigation_root_object
 from plone.base.utils import get_top_site_from_url
 from Products.CMFCore.utils import getToolByName
 from z3c.form.browser.text import TextWidget as z3cform_TextWidget
 from z3c.form.interfaces import IEditForm
 from z3c.form.interfaces import IFieldWidget
 from z3c.form.interfaces import IForm
 from z3c.form.widget import FieldWidget
@@ -60,15 +60,15 @@
         for value in value.split(separator):
             title = value
             if catalog:
                 result = catalog(UID=value)
                 title = result[0].Title if result else value
             options["initialValues"][value] = title
 
-    nav_root = getNavigationRootObject(context, site)
+    nav_root = get_navigation_root_object(context, site)
 
     if not ISimpleItem.providedBy(context):
         context = nav_root
 
     # basePath - start to search/browse in here.
     base_path_context = context
     if not IFolder.providedBy(base_path_context):
```

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/widgets/richtext.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/richtext.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/widgets/select.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/select.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/widgets/singlecheckbox.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/widgets/singlecheckbox.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/widgets.zcml` & `plone.app.z3cform-4.3.0/plone/app/z3cform/widgets.zcml`

 * *Files 0% similar despite different names*

```diff
@@ -202,14 +202,28 @@
   <z3c:widgetTemplate
       widget=".interfaces.ILinkWidget"
       template="templates/link_input.pt"
       layer=".interfaces.IPloneFormLayer"
       mode="input"
       />
 
+  <!-- email -->
+  <adapter
+      factory=".widgets.email.EmailFieldWidget"
+      for="plone.schema.email.IEmail
+           plone.app.z3cform.interfaces.IPloneFormLayer"
+      />
+
+  <z3c:widgetTemplate
+      widget=".interfaces.IEmailWidget"
+      template="templates/email_input.pt"
+      layer=".interfaces.IPloneFormLayer"
+      mode="input"
+      />
+
   <!-- z3c.form overrides -->
 
   <z3c:widgetTemplate
       widget="z3c.form.interfaces.ITextWidget"
       template="templates/text_input.pt"
       layer=".interfaces.IPloneFormLayer"
       mode="input"
```

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/wysiwyg/README.rst` & `plone.app.z3cform-4.3.0/plone/app/z3cform/wysiwyg/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/wysiwyg/configure.zcml` & `plone.app.z3cform-4.3.0/plone/app/z3cform/wysiwyg/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/wysiwyg/widget.py` & `plone.app.z3cform-4.3.0/plone/app/z3cform/wysiwyg/widget.py`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/wysiwyg/wysiwyg_display.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/wysiwyg/wysiwyg_display.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone/app/z3cform/wysiwyg/wysiwyg_input.pt` & `plone.app.z3cform-4.3.0/plone/app/z3cform/wysiwyg/wysiwyg_input.pt`

 * *Files identical despite different names*

### Comparing `plone.app.z3cform-4.2.1/plone.app.z3cform.egg-info/PKG-INFO` & `plone.app.z3cform-4.3.0/plone.app.z3cform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.z3cform
-Version: 4.2.1
+Version: 4.3.0
 Summary: A collection of widgets, templates and other components for use with z3c.form and Plone
 Home-page: https://pypi.org/project/plone.app.z3cform
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL
 Keywords: zope plone form widget template
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,14 +17,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: tests
 
 =================
 plone.app.z3cform
 =================
 
@@ -677,14 +678,41 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.3.0 (2023-07-14)
+------------------
+
+New features:
+
+
+- Introduce new Email-Widget which is used for `plone.schema.email.IEmail` fields.
+  It uses the input type `email`.
+  [jensens] (#173)
+
+
+Bug fixes:
+
+
+- Fix OrdereSelectWidget browser validation when the input is required.
+  [petschki] (#178)
+- Ignore form validation when `ignoreRequiredOnExtract` is set.
+  [petschki] (#179)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (cfffba8c)
+
+
 4.2.1 (2023-06-16)
 ------------------
 
 Bug fixes:
 
 
 - Add `required` to orderedselect widget.
@@ -1817,8 +1845,7 @@
 
 
 0.3 - 2008-07-24
 ----------------
 
 - Create this package from Plone-specific bits that have been factored
   out of plone.z3cform.
-
```

### Comparing `plone.app.z3cform-4.2.1/plone.app.z3cform.egg-info/SOURCES.txt` & `plone.app.z3cform-4.3.0/plone.app.z3cform.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 CHANGES.rst
 CONTRIBUTING.rst
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
 setup.py
 docs/LICENSE.GPL
 docs/LICENSE.txt
 plone/__init__.py
 plone.app.z3cform.egg-info/PKG-INFO
 plone.app.z3cform.egg-info/SOURCES.txt
 plone.app.z3cform.egg-info/dependency_links.txt
@@ -33,14 +32,15 @@
 plone/app/z3cform/widget.py
 plone/app/z3cform/widgets.zcml
 plone/app/z3cform/profiles/default/browserlayer.xml
 plone/app/z3cform/profiles/default/metadata.xml
 plone/app/z3cform/templates/ajaxselect_display.pt
 plone/app/z3cform/templates/checkbox_input.pt
 plone/app/z3cform/templates/contentprovider-widget.pt
+plone/app/z3cform/templates/email_input.pt
 plone/app/z3cform/templates/error.pt
 plone/app/z3cform/templates/file_input.pt
 plone/app/z3cform/templates/form.pt
 plone/app/z3cform/templates/image_input.pt
 plone/app/z3cform/templates/layout.pt
 plone/app/z3cform/templates/link_input.pt
 plone/app/z3cform/templates/macros.pt
@@ -71,14 +71,15 @@
 plone/app/z3cform/tests/test_widget.py
 plone/app/z3cform/tests/test_widgets.py
 plone/app/z3cform/tests/testing.zcml
 plone/app/z3cform/tests/tests.py
 plone/app/z3cform/widgets/__init__.py
 plone/app/z3cform/widgets/base.py
 plone/app/z3cform/widgets/datetime.py
+plone/app/z3cform/widgets/email.py
 plone/app/z3cform/widgets/link.py
 plone/app/z3cform/widgets/patterns.py
 plone/app/z3cform/widgets/querystring.py
 plone/app/z3cform/widgets/relateditems.py
 plone/app/z3cform/widgets/richtext.py
 plone/app/z3cform/widgets/select.py
 plone/app/z3cform/widgets/singlecheckbox.py
```

### Comparing `plone.app.z3cform-4.2.1/plone.app.z3cform.egg-info/requires.txt` & `plone.app.z3cform-4.3.0/plone.app.z3cform.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 plone.app.textfield>=1.3.6
 plone.base
+plone.app.contentlisting
+plone.dexterity
+plone.i18n
 plone.protect
 plone.registry
 plone.schema
 plone.uuid
 plone.z3cform
 Products.GenericSetup
 pytz
 setuptools
 z3c.form>=4.0
-z3c.formwidget.query
+z3c.relationfield
 zope.deprecation
 zope.globalrequest
 Zope
 
 [test]
 plone.app.contenttypes[test]
-plone.app.layout
 plone.app.testing
 plone.autoform
 plone.browserlayer
 plone.supermodel
 plone.testing
 zope.annotation
 zope.intid
 zope.publisher
 
 [tests]
 plone.app.contenttypes[test]
-plone.app.layout
 plone.app.testing
 plone.autoform
 plone.browserlayer
 plone.supermodel
 plone.testing
 zope.annotation
 zope.intid
```

### Comparing `plone.app.z3cform-4.2.1/setup.py` & `plone.app.z3cform-4.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,23 @@
+from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
-import os
 
-
-def read(*rnames):
-    return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
-
-
-version = "4.2.1"
+version = "4.3.0"
 
 long_description = (
-    read("README.rst")
-    + "\n"
-    + read("plone", "app", "z3cform", "wysiwyg", "README.rst")
-    + "\n"
-    + read("plone", "app", "z3cform", "inline_validation.rst")
-    + "\n"
-    + read("CHANGES.rst")
-    + "\n"
+    f"{Path('README.rst').read_text()}\n"
+    f"{(Path('plone') / 'app' / 'z3cform' / 'wysiwyg' / 'README.rst').read_text()}\n"
+    f"{(Path('plone') / 'app' / 'z3cform' / 'inline_validation.rst').read_text()}\n"
+    f"{Path('CHANGES.rst').read_text()}"
 )
+
 test_requirements = [
     "plone.app.contenttypes[test]",
-    "plone.app.layout",
     "plone.app.testing",
     "plone.autoform",
     "plone.browserlayer",
     "plone.supermodel",
     "plone.testing",
     "zope.annotation",
     "zope.intid",
@@ -35,14 +26,17 @@
 
 setup(
     name="plone.app.z3cform",
     version=version,
     description="A collection of widgets, templates and other components "
     "for use with z3c.form and Plone",
     long_description=long_description,
+    long_description_content_type="text/x-rst",
+    # Get more strings from
+    # https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Core",
         "Framework :: Zope :: 5",
@@ -63,24 +57,27 @@
     namespace_packages=["plone", "plone.app"],
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.8",
     install_requires=[
         "plone.app.textfield>=1.3.6",
         "plone.base",
+        "plone.app.contentlisting",
+        "plone.dexterity",
+        "plone.i18n",
         "plone.protect",
         "plone.registry",
         "plone.schema",
         "plone.uuid",
         "plone.z3cform",
         "Products.GenericSetup",
         "pytz",
         "setuptools",
         "z3c.form >= 4.0",
-        "z3c.formwidget.query",
+        "z3c.relationfield",
         "zope.deprecation",
         "zope.globalrequest",
         "Zope",
     ],
     extras_require={
         # Until plone.app.z3cform 4.0.2 we only had the 'tests' extra.
         # In 4.0.3 we introduced the 'test' extra.
```

