# Comparing `tmp/Products.PlonePAS-8.0.1.tar.gz` & `tmp/Products.PlonePAS-8.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.PlonePAS-8.0.1.tar", last modified: Thu May 25 13:42:55 2023, max compression
+gzip compressed data, was "Products.PlonePAS-8.0.2.tar", last modified: Thu Jul 13 21:55:17 2023, max compression
```

## Comparing `Products.PlonePAS-8.0.1.tar` & `Products.PlonePAS-8.0.2.tar`

### file list

```diff
@@ -1,123 +1,124 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.840801 Products.PlonePAS-8.0.1/
--rw-r--r--   0 maurits    (501) staff       (20)     1019 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/.editorconfig
--rw-r--r--   0 maurits    (501) staff       (20)      176 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/.gitignore
--rw-r--r--   0 maurits    (501) staff       (20)      128 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/.meta.toml
--rw-r--r--   0 maurits    (501) staff       (20)      973 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/.pre-commit-config.yaml
--rw-r--r--   0 maurits    (501) staff       (20)    31977 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      141 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    36326 2023-05-25 13:42:55.840958 Products.PlonePAS-8.0.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3432 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      438 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/buildout.cfg
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.813476 Products.PlonePAS-8.0.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     2160 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/docs/LICENSE.ZPL
--rw-r--r--   0 maurits    (501) staff       (20)      888 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/docs/STATUS.txt
--rw-r--r--   0 maurits    (501) staff       (20)     5720 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/docs/TODO.txt
--rw-r--r--   0 maurits    (501) staff       (20)      337 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/docs/copyright-and-license.txt
--rw-r--r--   0 maurits    (501) staff       (20)      891 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/docs/pas-dev.txt
--rw-r--r--   0 maurits    (501) staff       (20)      452 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/docs/scratchpad.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1248 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/mypy.ini
--rw-r--r--   0 maurits    (501) staff       (20)     1769 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      217 2023-05-25 13:42:55.841505 Products.PlonePAS-8.0.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1870 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.805673 Products.PlonePAS-8.0.1/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.813911 Products.PlonePAS-8.0.1/src/Products/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.821068 Products.PlonePAS-8.0.1/src/Products/PlonePAS/
--rw-r--r--   0 maurits    (501) staff       (20)     4655 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.822509 Products.PlonePAS-8.0.1/src/Products/PlonePAS/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      910 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1371 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/browser/info.py
--rw-r--r--   0 maurits    (501) staff       (20)      977 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/browser/member.py
--rw-r--r--   0 maurits    (501) staff       (20)     2617 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/browser/search.py
--rw-r--r--   0 maurits    (501) staff       (20)      584 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/config.py
--rw-r--r--   0 maurits    (501) staff       (20)      512 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      795 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/events.py
--rw-r--r--   0 maurits    (501) staff       (20)     1184 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/exportimport.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.825133 Products.PlonePAS-8.0.1/src/Products/PlonePAS/interfaces/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/interfaces/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3247 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/interfaces/browser.py
--rw-r--r--   0 maurits    (501) staff       (20)     2384 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/interfaces/capabilities.py
--rw-r--r--   0 maurits    (501) staff       (20)      192 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/interfaces/events.py
--rw-r--r--   0 maurits    (501) staff       (20)     3635 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/interfaces/group.py
--rw-r--r--   0 maurits    (501) staff       (20)      185 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/interfaces/memberdata.py
--rw-r--r--   0 maurits    (501) staff       (20)      272 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/interfaces/membership.py
--rw-r--r--   0 maurits    (501) staff       (20)     3424 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/interfaces/plugins.py
--rw-r--r--   0 maurits    (501) staff       (20)      402 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/interfaces/propertysheets.py
--rw-r--r--   0 maurits    (501) staff       (20)    20812 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/pas.py
--rw-r--r--   0 maurits    (501) staff       (20)     2222 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/patch.py
--rw-r--r--   0 maurits    (501) staff       (20)      519 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/permissions.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.828424 Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3907 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/autogroup.py
--rw-r--r--   0 maurits    (501) staff       (20)     4011 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/cookie_handler.py
--rw-r--r--   0 maurits    (501) staff       (20)     2007 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/crumbler.py
--rw-r--r--   0 maurits    (501) staff       (20)     9251 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/group.py
--rw-r--r--   0 maurits    (501) staff       (20)     5314 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/local_role.py
--rw-r--r--   0 maurits    (501) staff       (20)     2378 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/passwordpolicy.py
--rw-r--r--   0 maurits    (501) staff       (20)    10608 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/property.py
--rw-r--r--   0 maurits    (501) staff       (20)     5528 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/role.py
--rw-r--r--   0 maurits    (501) staff       (20)     7109 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/ufactory.py
--rw-r--r--   0 maurits    (501) staff       (20)     4465 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/user.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.806782 Products.PlonePAS-8.0.1/src/Products/PlonePAS/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.829033 Products.PlonePAS-8.0.1/src/Products/PlonePAS/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)       85 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)       65 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/profiles/default/plone-pas.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.829643 Products.PlonePAS-8.0.1/src/Products/PlonePAS/profiles/root-cookie/
--rw-r--r--   0 maurits    (501) staff       (20)       85 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/profiles/root-cookie/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      116 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/profiles/root-cookie/plone-pas-zope-root-cookie.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1387 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/profiles.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    19253 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     3771 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/sheet.py
--rw-r--r--   0 maurits    (501) staff       (20)     1806 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.833963 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2803 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/cookie_auth.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1393 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/dummy.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.834889 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/images/
--rw-r--r--   0 maurits    (501) staff       (20)     5714 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/images/test.gif
--rw-r--r--   0 maurits    (501) staff       (20)     1898 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/images/test.jpg
--rw-r--r--   0 maurits    (501) staff       (20)      315 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/images/test.png
--rw-r--r--   0 maurits    (501) staff       (20)     6138 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/test_basic_ops.py
--rw-r--r--   0 maurits    (501) staff       (20)      646 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)     6968 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/test_groupdatatool.py
--rw-r--r--   0 maurits    (501) staff       (20)    10213 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/test_groupstool.py
--rw-r--r--   0 maurits    (501) staff       (20)     5739 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/test_memberdatatool.py
--rw-r--r--   0 maurits    (501) staff       (20)    42530 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/test_membershiptool.py
--rw-r--r--   0 maurits    (501) staff       (20)    10526 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/test_properties.py
--rw-r--r--   0 maurits    (501) staff       (20)     3272 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/test_role_plugin.py
--rw-r--r--   0 maurits    (501) staff       (20)     5335 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     1007 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/test_views.py
--rw-r--r--   0 maurits    (501) staff       (20)      954 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tool.gif
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.836917 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tools/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tools/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      179 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tools/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    18192 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tools/groupdata.py
--rw-r--r--   0 maurits    (501) staff       (20)    14413 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tools/groups.py
--rw-r--r--   0 maurits    (501) staff       (20)    17323 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tools/memberdata.py
--rw-r--r--   0 maurits    (501) staff       (20)    29163 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/tools/membership.py
--rw-r--r--   0 maurits    (501) staff       (20)     2101 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)     6500 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.840556 Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/
--rw-r--r--   0 maurits    (501) staff       (20)     2089 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/AutoGroupForm.zpt
--rw-r--r--   0 maurits    (501) staff       (20)      847 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/CookieCrumblingPluginForm.dtml
--rw-r--r--   0 maurits    (501) staff       (20)      512 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/ExtendedCookieAuthHelperForm.dtml
--rw-r--r--   0 maurits    (501) staff       (20)      730 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/GroupAwareRoleManagerForm.dtml
--rw-r--r--   0 maurits    (501) staff       (20)      679 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/GroupManagerForm.dtml
--rw-r--r--   0 maurits    (501) staff       (20)      666 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/LocalRolesManagerForm.dtml
--rw-r--r--   0 maurits    (501) staff       (20)      703 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/MutablePropertyProviderForm.dtml
--rw-r--r--   0 maurits    (501) staff       (20)     1501 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/PasswordPolicyForm.zpt
--rw-r--r--   0 maurits    (501) staff       (20)      687 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/PloneUserFactoryForm.dtml
--rw-r--r--   0 maurits    (501) staff       (20)      659 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/UserManagerForm.dtml
--rw-r--r--   0 maurits    (501) staff       (20)     3569 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/membershipRolemapping.dtml
--rw-r--r--   0 maurits    (501) staff       (20)     1874 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/portrait_fix.dtml
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-25 13:42:55.816383 Products.PlonePAS-8.0.1/src/Products.PlonePAS.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    36326 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products.PlonePAS.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     4053 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products.PlonePAS.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products.PlonePAS.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        9 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products.PlonePAS.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products.PlonePAS.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      274 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products.PlonePAS.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        9 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/src/Products.PlonePAS.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1279 2023-05-25 13:42:55.000000 Products.PlonePAS-8.0.1/tox.ini
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.717869 Products.PlonePAS-8.0.2/
+-rw-r--r--   0 maurits    (501) staff       (20)     1342 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/.editorconfig
+-rw-r--r--   0 maurits    (501) staff       (20)      540 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/.flake8
+-rw-r--r--   0 maurits    (501) staff       (20)      663 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/.gitignore
+-rw-r--r--   0 maurits    (501) staff       (20)      312 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/.meta.toml
+-rw-r--r--   0 maurits    (501) staff       (20)     1879 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 maurits    (501) staff       (20)    32086 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      141 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    36472 2023-07-13 21:55:17.717579 Products.PlonePAS-8.0.2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3432 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      438 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/buildout.cfg
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.691338 Products.PlonePAS-8.0.2/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     2160 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/docs/LICENSE.ZPL
+-rw-r--r--   0 maurits    (501) staff       (20)      888 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/docs/STATUS.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     5720 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/docs/TODO.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      337 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/docs/copyright-and-license.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      891 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/docs/pas-dev.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      452 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/docs/scratchpad.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1248 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/mypy.ini
+-rw-r--r--   0 maurits    (501) staff       (20)     4243 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-07-13 21:55:17.717937 Products.PlonePAS-8.0.2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2020 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.683655 Products.PlonePAS-8.0.2/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.691579 Products.PlonePAS-8.0.2/src/Products/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.698041 Products.PlonePAS-8.0.2/src/Products/PlonePAS/
+-rw-r--r--   0 maurits    (501) staff       (20)     4655 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.699995 Products.PlonePAS-8.0.2/src/Products/PlonePAS/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      910 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1371 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/browser/info.py
+-rw-r--r--   0 maurits    (501) staff       (20)      977 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/browser/member.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2617 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/browser/search.py
+-rw-r--r--   0 maurits    (501) staff       (20)      584 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/config.py
+-rw-r--r--   0 maurits    (501) staff       (20)      512 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      795 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/events.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1184 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/exportimport.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.702467 Products.PlonePAS-8.0.2/src/Products/PlonePAS/interfaces/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/interfaces/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3247 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/interfaces/browser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2384 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/interfaces/capabilities.py
+-rw-r--r--   0 maurits    (501) staff       (20)      192 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/interfaces/events.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3635 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/interfaces/group.py
+-rw-r--r--   0 maurits    (501) staff       (20)      185 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/interfaces/memberdata.py
+-rw-r--r--   0 maurits    (501) staff       (20)      272 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/interfaces/membership.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3424 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/interfaces/plugins.py
+-rw-r--r--   0 maurits    (501) staff       (20)      402 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/interfaces/propertysheets.py
+-rw-r--r--   0 maurits    (501) staff       (20)    20812 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/pas.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2222 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/patch.py
+-rw-r--r--   0 maurits    (501) staff       (20)      519 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/permissions.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.705801 Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3907 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/autogroup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4011 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/cookie_handler.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2007 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/crumbler.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9251 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/group.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5314 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/local_role.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2378 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/passwordpolicy.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10608 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/property.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5528 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/role.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7109 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/ufactory.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4465 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/user.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.684556 Products.PlonePAS-8.0.2/src/Products/PlonePAS/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.706370 Products.PlonePAS-8.0.2/src/Products/PlonePAS/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       65 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/profiles/default/plone-pas.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.707051 Products.PlonePAS-8.0.2/src/Products/PlonePAS/profiles/root-cookie/
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/profiles/root-cookie/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      116 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/profiles/root-cookie/plone-pas-zope-root-cookie.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1387 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/profiles.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    19253 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3771 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/sheet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1806 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.710954 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2803 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/cookie_auth.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1393 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/dummy.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.711768 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/images/
+-rw-r--r--   0 maurits    (501) staff       (20)     5714 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/images/test.gif
+-rw-r--r--   0 maurits    (501) staff       (20)     1898 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/images/test.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)      315 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/images/test.png
+-rw-r--r--   0 maurits    (501) staff       (20)     6138 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/test_basic_ops.py
+-rw-r--r--   0 maurits    (501) staff       (20)      646 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6968 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/test_groupdatatool.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10213 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/test_groupstool.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5739 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/test_memberdatatool.py
+-rw-r--r--   0 maurits    (501) staff       (20)    42530 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/test_membershiptool.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10526 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/test_properties.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3272 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/test_role_plugin.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5335 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/test_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1007 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/test_views.py
+-rw-r--r--   0 maurits    (501) staff       (20)      954 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tool.gif
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.713459 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tools/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tools/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      179 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tools/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    18192 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tools/groupdata.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14413 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tools/groups.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17323 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tools/memberdata.py
+-rw-r--r--   0 maurits    (501) staff       (20)    29163 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/tools/membership.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2101 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6500 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.717253 Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/
+-rw-r--r--   0 maurits    (501) staff       (20)     2500 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/AutoGroupForm.zpt
+-rw-r--r--   0 maurits    (501) staff       (20)      847 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/CookieCrumblingPluginForm.dtml
+-rw-r--r--   0 maurits    (501) staff       (20)      512 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/ExtendedCookieAuthHelperForm.dtml
+-rw-r--r--   0 maurits    (501) staff       (20)      730 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/GroupAwareRoleManagerForm.dtml
+-rw-r--r--   0 maurits    (501) staff       (20)      679 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/GroupManagerForm.dtml
+-rw-r--r--   0 maurits    (501) staff       (20)      666 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/LocalRolesManagerForm.dtml
+-rw-r--r--   0 maurits    (501) staff       (20)      703 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/MutablePropertyProviderForm.dtml
+-rw-r--r--   0 maurits    (501) staff       (20)     1832 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/PasswordPolicyForm.zpt
+-rw-r--r--   0 maurits    (501) staff       (20)      687 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/PloneUserFactoryForm.dtml
+-rw-r--r--   0 maurits    (501) staff       (20)      659 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/UserManagerForm.dtml
+-rw-r--r--   0 maurits    (501) staff       (20)     3569 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/membershipRolemapping.dtml
+-rw-r--r--   0 maurits    (501) staff       (20)     1874 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/portrait_fix.dtml
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 21:55:17.693717 Products.PlonePAS-8.0.2/src/Products.PlonePAS.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    36472 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products.PlonePAS.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     4051 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products.PlonePAS.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products.PlonePAS.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        9 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products.PlonePAS.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products.PlonePAS.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      296 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products.PlonePAS.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        9 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/src/Products.PlonePAS.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4616 2023-07-13 21:55:17.000000 Products.PlonePAS-8.0.2/tox.ini
```

### Comparing `Products.PlonePAS-8.0.1/.editorconfig` & `Products.PlonePAS-8.0.2/.editorconfig`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Generated from:
 # https://github.com/plone/meta/tree/master/config/default
+# See the inline comments on how to expand/tweak this configuration file
 #
 # EditorConfig Configuration file, for more details see:
 # http://EditorConfig.org
 # EditorConfig is a convention description, that could be interpreted
 # by multiple editors to enforce common coding conventions for specific
 # file types
 
@@ -28,12 +29,25 @@
 # 4 space indentation
 indent_size = 4
 
 [*.{yml,zpt,pt,dtml,zcml}]
 # 2 space indentation
 indent_size = 2
 
+[*.{json,jsonl,js,jsx,ts,tsx,css,less,scss,html}]  # Frontend development
+# 2 space indentation
+indent_size = 2
+
 [{Makefile,.gitmodules}]
 # Tab indentation (no size specified, but view as 4 spaces)
 indent_style = tab
 indent_size = unset
 tab_width = unset
+
+
+##
+# Add extra configuration options in .meta.toml:
+#  [editorconfig]
+#  extra_lines = """
+#  _your own configuration lines_
+#  """
+##
```

### Comparing `Products.PlonePAS-8.0.1/CHANGES.rst` & `Products.PlonePAS-8.0.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+8.0.2 (2023-07-13)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (cfffba8c)
+
+
 8.0.1 (2023-05-25)
 ------------------
 
 Bug fixes:
 
 
 - Translate error message, simplify error handling. [tschorr] (#75)
```

### Comparing `Products.PlonePAS-8.0.1/PKG-INFO` & `Products.PlonePAS-8.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.PlonePAS
-Version: 8.0.1
+Version: 8.0.2
 Summary: PlonePAS modifies the PluggableAuthService for use by Plone.
 Home-page: https://github.com/plone/Products.PlonePAS
 Author: Kapil Thangavelu, Wichert Akkerman
 Author-email: plone-developers@lists.sourceforge.net
 License: ZPL
 Keywords: Zope CMF Plone PAS authentication
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,14 +16,15 @@
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: test
 
 Overview
 ========
 
 This product extends `PluggableAuthService <https://github.com/zopefoundation/Products.PluggableAuthService>`_ (PAS) for use in Plone.
 
@@ -109,14 +110,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+8.0.2 (2023-07-13)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (cfffba8c)
+
+
 8.0.1 (2023-05-25)
 ------------------
 
 Bug fixes:
 
 
 - Translate error message, simplify error handling. [tschorr] (#75)
```

### Comparing `Products.PlonePAS-8.0.1/README.rst` & `Products.PlonePAS-8.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/docs/LICENSE.ZPL` & `Products.PlonePAS-8.0.2/docs/LICENSE.ZPL`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/docs/STATUS.txt` & `Products.PlonePAS-8.0.2/docs/STATUS.txt`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/docs/TODO.txt` & `Products.PlonePAS-8.0.2/docs/TODO.txt`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/docs/pas-dev.txt` & `Products.PlonePAS-8.0.2/docs/pas-dev.txt`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/mypy.ini` & `Products.PlonePAS-8.0.2/mypy.ini`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/setup.py` & `Products.PlonePAS-8.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,42 @@
+from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "8.0.1"
+version = "8.0.2"
 
-
-longdescription = open("README.rst").read()
-longdescription += "\n"
-longdescription += open("CHANGES.rst").read()
+long_description = (
+    f"{Path('README.rst').read_text()}\n{Path('CHANGES.rst').read_text()}"
+)
 
 install_requires = [
     "AuthEncoding",
     "BTrees",
     "Pillow",
     "plone.base",
     "plone.i18n",
     "plone.memoize",
     "plone.protect>=2.0.3",
     "plone.registry",
     "plone.session",
+    "Products.BTreeFolder2",
     "Products.GenericSetup",
     "Products.PluggableAuthService>=2.0",
     "setuptools",
 ]
 
 setup(
     name="Products.PlonePAS",
     version=version,
     description="PlonePAS modifies the PluggableAuthService for use by Plone.",
-    long_description=longdescription,
+    long_description=long_description,
+    long_description_content_type="text/x-rst",
+    # Get more strings from
+    # https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Framework :: Plone",
         "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Core",
         "Framework :: Zope",
         "Framework :: Zope :: 5",
```

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/__init__.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/browser/configure.zcml` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/browser/info.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/browser/info.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/browser/member.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/browser/member.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/browser/search.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/browser/search.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/config.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/config.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/configure.zcml` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/events.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/events.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/exportimport.zcml` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/exportimport.zcml`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/interfaces/browser.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/interfaces/browser.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/interfaces/capabilities.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/interfaces/capabilities.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/interfaces/group.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/interfaces/group.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/interfaces/plugins.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/interfaces/plugins.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/pas.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/pas.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/patch.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/patch.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/permissions.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/permissions.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/autogroup.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/autogroup.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/cookie_handler.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/cookie_handler.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/crumbler.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/crumbler.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/group.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/group.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/local_role.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/local_role.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/passwordpolicy.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/passwordpolicy.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/property.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/property.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/role.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/role.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/ufactory.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/ufactory.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/plugins/user.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/plugins/user.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/profiles.zcml` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/profiles.zcml`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/setuphandlers.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/sheet.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/sheet.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/testing.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/testing.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/cookie_auth.rst` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/cookie_auth.rst`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/dummy.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/dummy.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/images/test.gif` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/images/test.gif`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/images/test.jpg` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/images/test.jpg`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/test_basic_ops.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/test_basic_ops.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/test_doctests.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/test_groupdatatool.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/test_groupdatatool.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/test_groupstool.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/test_groupstool.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/test_memberdatatool.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/test_memberdatatool.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/test_membershiptool.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/test_membershiptool.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/test_properties.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/test_role_plugin.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/test_role_plugin.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/test_setup.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/tests/test_views.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/tool.gif` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/tool.gif`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/tools/groupdata.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/tools/groupdata.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/tools/groups.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/tools/groups.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/tools/memberdata.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/tools/memberdata.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/tools/membership.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/tools/membership.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/upgrades.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/upgrades.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/utils.py` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/utils.py`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/AutoGroupForm.zpt` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/AutoGroupForm.zpt`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,24 @@
-<h1 tal:replace="structure here/manage_page_header">Header</h1>
+<h1 xmlns="http://www.w3.org/1999/xhtml"
+    xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+    xmlns:tal="http://xml.zope.org/namespaces/tal"
+    xml:lang="en"
+    tal:replace="structure here/manage_page_header"
+    i18n:domain="plone"
+>Header</h1>
 
 <h2 tal:define="
       form_title string:Add Auto Group plugin;
     "
     tal:replace="structure here/manage_form_title"
 >Form Title</h2>
 
-<p class="form-help">
+<p class="form-help"
+   i18n:translate=""
+>
 The Auto Group plugin automatically puts all authenticated users in a virtual
 group.
 </p>
 
 <form action="manage_addAutoGroup"
       method="post"
 >
@@ -18,15 +26,17 @@
          cellpadding="2"
          cellspacing="0"
   >
     <tr>
       <td align="left"
           valign="top"
       >
-        <div class="form-label">
+        <div class="form-label"
+             i18n:translate=""
+        >
     Id
         </div>
       </td>
       <td align="left"
           valign="top"
       >
         <input name="id"
@@ -35,15 +45,17 @@
         />
       </td>
     </tr>
     <tr>
       <td align="left"
           valign="top"
       >
-        <div class="form-optional">
+        <div class="form-optional"
+             i18n:translate=""
+        >
     Title
         </div>
       </td>
       <td align="left"
           valign="top"
       >
         <input name="title"
@@ -52,15 +64,17 @@
         />
       </td>
     </tr>
     <tr>
       <td align="left"
           valign="top"
       >
-        <div class="form-label">
+        <div class="form-label"
+             i18n:translate=""
+        >
     Group id
         </div>
       </td>
       <td align="left"
           valign="top"
       >
         <input name="group"
@@ -69,15 +83,17 @@
         />
       </td>
     </tr>
     <tr>
       <td align="left"
           valign="top"
       >
-        <div class="form-label">
+        <div class="form-label"
+             i18n:translate=""
+        >
     Description
         </div>
       </td>
       <td align="left"
           valign="top"
       >
         <input name="description"
@@ -95,14 +111,15 @@
           valign="top"
       >
         <div class="form-element">
           <input class="form-element"
                  name="submit"
                  type="submit"
                  value=" Add "
+                 i18n:attributes="value"
           />
         </div>
       </td>
     </tr>
   </table>
 </form>
```

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/CookieCrumblingPluginForm.dtml` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/CookieCrumblingPluginForm.dtml`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/ExtendedCookieAuthHelperForm.dtml` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/ExtendedCookieAuthHelperForm.dtml`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/GroupAwareRoleManagerForm.dtml` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/GroupAwareRoleManagerForm.dtml`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/GroupManagerForm.dtml` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/GroupManagerForm.dtml`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/LocalRolesManagerForm.dtml` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/LocalRolesManagerForm.dtml`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/MutablePropertyProviderForm.dtml` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/MutablePropertyProviderForm.dtml`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/PasswordPolicyForm.zpt` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/PasswordPolicyForm.zpt`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,41 @@
-<h1 tal:replace="structure here/manage_page_header">Header</h1>
+<h1 xmlns="http://www.w3.org/1999/xhtml"
+    xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+    xmlns:tal="http://xml.zope.org/namespaces/tal"
+    xml:lang="en"
+    tal:replace="structure here/manage_page_header"
+    i18n:domain="plone"
+>Header</h1>
 
 <h2 tal:define="
       form_title string:Add Default Plone Password Policy plugin;
     "
     tal:replace="structure here/manage_form_title"
 >Form Title</h2>
 
-<p class="form-help">
+<p class="form-help"
+   i18n:translate=""
+>
 The Default Plone Password Policy validates passwords to be at least 5 chars long
 </p>
 
 <form action="manage_addPasswordPolicyPlugin"
       method="post"
 >
   <table border="0"
          cellpadding="2"
          cellspacing="0"
   >
     <tr>
       <td align="left"
           valign="top"
       >
-        <div class="form-label">
+        <div class="form-label"
+             i18n:translate=""
+        >
     Id
         </div>
       </td>
       <td align="left"
           valign="top"
       >
         <input name="id"
@@ -34,15 +44,17 @@
         />
       </td>
     </tr>
     <tr>
       <td align="left"
           valign="top"
       >
-        <div class="form-optional">
+        <div class="form-optional"
+             i18n:translate=""
+        >
     Title
         </div>
       </td>
       <td align="left"
           valign="top"
       >
         <input name="title"
@@ -60,14 +72,15 @@
           valign="top"
       >
         <div class="form-element">
           <input class="form-element"
                  name="submit"
                  type="submit"
                  value=" Add "
+                 i18n:attributes="value"
           />
         </div>
       </td>
     </tr>
   </table>
 </form>
```

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/PloneUserFactoryForm.dtml` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/PloneUserFactoryForm.dtml`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/UserManagerForm.dtml` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/UserManagerForm.dtml`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/membershipRolemapping.dtml` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/membershipRolemapping.dtml`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products/PlonePAS/zmi/portrait_fix.dtml` & `Products.PlonePAS-8.0.2/src/Products/PlonePAS/zmi/portrait_fix.dtml`

 * *Files identical despite different names*

### Comparing `Products.PlonePAS-8.0.1/src/Products.PlonePAS.egg-info/PKG-INFO` & `Products.PlonePAS-8.0.2/src/Products.PlonePAS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.PlonePAS
-Version: 8.0.1
+Version: 8.0.2
 Summary: PlonePAS modifies the PluggableAuthService for use by Plone.
 Home-page: https://github.com/plone/Products.PlonePAS
 Author: Kapil Thangavelu, Wichert Akkerman
 Author-email: plone-developers@lists.sourceforge.net
 License: ZPL
 Keywords: Zope CMF Plone PAS authentication
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,14 +16,15 @@
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: test
 
 Overview
 ========
 
 This product extends `PluggableAuthService <https://github.com/zopefoundation/Products.PluggableAuthService>`_ (PAS) for use in Plone.
 
@@ -109,14 +110,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+8.0.2 (2023-07-13)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (cfffba8c)
+
+
 8.0.1 (2023-05-25)
 ------------------
 
 Bug fixes:
 
 
 - Translate error message, simplify error handling. [tschorr] (#75)
```

### Comparing `Products.PlonePAS-8.0.1/src/Products.PlonePAS.egg-info/SOURCES.txt` & `Products.PlonePAS-8.0.2/src/Products.PlonePAS.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 .editorconfig
+.flake8
 .gitignore
 .meta.toml
 .pre-commit-config.yaml
 CHANGES.rst
 CONTRIBUTING.rst
 MANIFEST.in
 README.rst
 buildout.cfg
 mypy.ini
 pyproject.toml
-setup.cfg
 setup.py
 tox.ini
 docs/LICENSE.ZPL
 docs/STATUS.txt
 docs/TODO.txt
 docs/copyright-and-license.txt
 docs/pas-dev.txt
```

