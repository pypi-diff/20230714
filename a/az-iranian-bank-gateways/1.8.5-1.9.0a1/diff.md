# Comparing `tmp/az-iranian-bank-gateways-1.8.5.tar.gz` & `tmp/az-iranian-bank-gateways-1.9.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/learnwise/backend/az-iranian-bank-gateways/dist/.tmp-fxb16qpt/az-iranian-bank-gateways-1.8.5.tar", last modified: Tue Feb  7 17:33:44 2023, max compression
+gzip compressed data, was "/builds/learnwise/backend/az-iranian-bank-gateways/dist/.tmp-o9sw6pfz/az-iranian-bank-gateways-1.9.0a1.tar", last modified: Fri Jul 14 20:44:14 2023, max compression
```

## Comparing `az-iranian-bank-gateways-1.8.5.tar` & `az-iranian-bank-gateways-1.9.0a1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      958 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    17625 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/az_iranian_bank_gateways.egg-info/
--rw-r--r--   0 root         (0) root         (0)      958 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/az_iranian_bank_gateways.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2028 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/az_iranian_bank_gateways.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/az_iranian_bank_gateways.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/az_iranian_bank_gateways.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       78 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/az_iranian_bank_gateways.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/az_iranian_bank_gateways.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-02-07 17:33:33.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1439 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/bankfactories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/banks/
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/banks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4585 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/banks/bahamta.py
--rw-rw-rw-   0 root         (0) root         (0)    12435 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/banks/banks.py
--rw-rw-rw-   0 root         (0) root         (0)     5603 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/banks/bmi.py
--rw-rw-rw-   0 root         (0) root         (0)     4714 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/banks/idpay.py
--rw-rw-rw-   0 root         (0) root         (0)     5992 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/banks/mellat.py
--rw-rw-rw-   0 root         (0) root         (0)     5089 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/banks/payV1.py
--rw-rw-rw-   0 root         (0) root         (0)     5129 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/banks/sep.py
--rw-rw-rw-   0 root         (0) root         (0)     4217 2023-02-07 17:33:32.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/banks/zarinpal.py
--rw-rw-rw-   0 root         (0) root         (0)     4164 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/banks/zibal.py
--rwxrwxrwx   0 root         (0) root         (0)     1660 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/default_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/exceptions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      999 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/exceptions/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      219 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/locale/en/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/locale/en/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     2131 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/locale/fa/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/locale/fa/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1432 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/locale/fa/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     2477 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2673 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1418 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/migrations/0002_auto_20210102_0721.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/migrations/0003_bank_bank_choose_identifier.py
--rw-rw-rw-   0 root         (0) root         (0)      798 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/migrations/0004_auto_20211115_1500.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/models/
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2973 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/models/banks.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/models/enum.py
--rw-rw-rw-   0 root         (0) root         (0)     2621 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/models/enum_django.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/readers/
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/readers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/readers/bases.py
--rw-rw-rw-   0 root         (0) root         (0)      931 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/readers/defaults.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/templates/azbankgateways/
--rw-rw-rw-   0 root         (0) root         (0)      532 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/templates/azbankgateways/redirect_to_bank.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/templates/azbankgateways/samples/
--rw-rw-rw-   0 root         (0) root         (0)      944 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/templates/azbankgateways/samples/base.html
--rw-rw-rw-   0 root         (0) root         (0)      128 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/templates/azbankgateways/samples/base_site.html
--rw-rw-rw-   0 root         (0) root         (0)      727 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/templates/azbankgateways/samples/gateway.html
--rw-rw-rw-   0 root         (0) root         (0)     1054 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/templates/azbankgateways/samples/result.html
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/types.py
--rw-rw-rw-   0 root         (0) root         (0)      724 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/views/
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1199 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/views/banks.py
--rw-rw-rw-   0 root         (0) root         (0)     2671 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/azbankgateways/views/samples.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-02-07 17:22:55.000000 az-iranian-bank-gateways-1.8.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1333 2023-02-07 17:33:44.000000 az-iranian-bank-gateways-1.8.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      960 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    23641 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/az_iranian_bank_gateways.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      960 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/az_iranian_bank_gateways.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2028 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/az_iranian_bank_gateways.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/az_iranian_bank_gateways.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/az_iranian_bank_gateways.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       78 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/az_iranian_bank_gateways.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/az_iranian_bank_gateways.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-14 20:44:03.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1439 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/bankfactories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/banks/
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/banks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4585 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/banks/bahamta.py
+-rw-rw-rw-   0 root         (0) root         (0)    13334 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/banks/banks.py
+-rw-rw-rw-   0 root         (0) root         (0)     5603 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/banks/bmi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4714 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/banks/idpay.py
+-rw-rw-rw-   0 root         (0) root         (0)     5992 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/banks/mellat.py
+-rw-rw-rw-   0 root         (0) root         (0)     5089 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/banks/payV1.py
+-rw-rw-rw-   0 root         (0) root         (0)     5129 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/banks/sep.py
+-rw-rw-rw-   0 root         (0) root         (0)     4217 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/banks/zarinpal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4164 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/banks/zibal.py
+-rwxrwxrwx   0 root         (0) root         (0)     2418 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/default_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/exceptions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1120 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/exceptions/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      219 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/locale/en/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2131 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/locale/fa/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/locale/fa/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/locale/fa/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2673 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1418 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/migrations/0002_auto_20210102_0721.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/migrations/0003_bank_bank_choose_identifier.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/migrations/0004_auto_20211115_1500.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/models/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2973 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/models/banks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/models/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     2621 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/models/enum_django.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/readers/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/readers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      934 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/readers/bases.py
+-rw-rw-rw-   0 root         (0) root         (0)      931 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/readers/defaults.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/templates/azbankgateways/
+-rw-rw-rw-   0 root         (0) root         (0)      532 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/templates/azbankgateways/redirect_to_bank.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/templates/azbankgateways/samples/
+-rw-rw-rw-   0 root         (0) root         (0)      944 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/templates/azbankgateways/samples/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/templates/azbankgateways/samples/base_site.html
+-rw-rw-rw-   0 root         (0) root         (0)      727 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/templates/azbankgateways/samples/gateway.html
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/templates/azbankgateways/samples/result.html
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/views/
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/views/banks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2814 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/azbankgateways/views/samples.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-07-14 20:44:02.000000 az-iranian-bank-gateways-1.9.0a1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1333 2023-07-14 20:44:14.000000 az-iranian-bank-gateways-1.9.0a1/setup.cfg
```

### Comparing `az-iranian-bank-gateways-1.8.5/LICENSE` & `az-iranian-bank-gateways-1.9.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/PKG-INFO` & `az-iranian-bank-gateways-1.9.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: az-iranian-bank-gateways
-Version: 1.8.5
+Version: 1.9.0a1
 Summary: Iranian Bank Gateways for django
 Home-page: https://github.com/ali-zahedi/az-iranian-bank-gateways
 Author: Ali Zahedigol
 Author-email: alizahedigol@gmail.com
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `az-iranian-bank-gateways-1.8.5/README.md` & `az-iranian-bank-gateways-1.9.0a1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -104,14 +104,16 @@
     'TRACKING_CODE_LENGTH': 16, # اختیاری
     'SETTING_VALUE_READER_CLASS': 'azbankgateways.readers.DefaultReader', # اختیاری
     'BANK_PRIORITIES': [
         'BMI',
         'SEP',
         # and so on ...
     ], # اختیاری
+    'IS_SAFE_GET_GATEWAY_PAYMENT': False, #اختیاری، بهتر است True بزارید.
+    'CUSTOM_APP': None, # اختیاری 
 }
  ```
 
 1. `GATEWAYS` :  تنظیمات مربوط به هر بانک به صورت دیکشنری های جدا در این قسمت وجود دارد. تنظیماتی مانند کلاس اجرا کننده، کلیدهای امنیتی که توسط بانک در اختیار شما قرار می گیرد.
 
 1. `DEFAULT`: در زمانی که به سازنده فکتوری پارامتری ارسال نشود از این تنظیم به عنوان بانک پیش فرض استفاده خواهد شد و ارتباطات با این بانک برقرار می شود. 
 
@@ -124,15 +126,40 @@
 1. `SETTING_VALUE_READER_CLASS`: با مقدار دهی به این تنظیم شما می توانید حالت یک متغیر خوان اضافه کنید که قابلیت های دیگری مثل پروایدر و پشتیبانی از یک بانک با چند اکانت و ... را به آن اضافه کنید.
  
 1. `BANK_PRIORITIES`: این آرایه اختیاری است. زمانی که وضعیت اتصال به درگاه به صورت خودکار تعیین شده باشد، ابتدا به بانک پیش فرض متصل می شود و سپس بر این اساس شروع به اتصال خواهد کرد، تا به اولین درگاه فعال برسد. در حالت پیش فرض این آرایه خالی است که بعد از اتصال به درگاه مورد نظر در صورت خطا بقیه درگاه ها امتحان نخواهند شد.
 
 1. `IS_SAMPLE_FORM_ENABLE`: یو آر ال های مربوط به تست درگاه بانک را فعال و یا غیر فعال می کند. در صورت فعال بودن می توانید از طریق آدرس زیر درگاه پرداخت را امتحان کنید.
 
    * [Sample payment](http://127.0.0.1:8000/bankgateways/sample-payment/)
-   
+
+1. `CALLBACK_NAMESPACE`: اگر میخواهید تابع کال بک داخلی را اوررایت کنید یا پروژه دارای اپ های مختلفی است و قسمت پرداخت در اپ جداگانه ای قرار دارد میتوانید محل قرار گیری یو آر ال های پیشفرض را تغییر دهید  برای مثال:
+   ```
+   'CALLBACK_NAMESPACE': 'api:payment:callback',
+    ```
+1. `GO_TO_BANK_GATEWAY_NAMESPACE`: اگر میخواهید تابع رفتن به دروازه بانک داخلی را اوررایت کنید یا پروژه دارای اپ های مختلفی است وقسمت پرداخت در اپ جداگانه ای قرار دارد میتوانید محل قرار گیری یو آر ال های پیشفرض را تغییر دهید برای مثال:
+    ```
+     'GO_TO_BANK_GATEWAY_NAMESPACE': 'api:payment:go-to-bank-gateway',
+    ```
+1. `SAMPLE_RESULT_NAMESPACE`: اگر میخواهید صفحه نمونه داخلی را اوررایت کنید یا پروژه دارای اپ های مختلفی است وقسمت پرداخت در اپ جداگانه ای قرار دارد میتوانید محل قرار گیری یو آر ال های پیشفرض را تغییر دهید برای مثال:
+    ```
+     'SAMPLE_RESULT_NAMESPACE': 'api:payment:sample-result',
+    ```
+1. `'IS_SAFE_GET_GATEWAY_PAYMENT'`:<br>
+   ```
+   'IS_SAFE_GET_GATEWAY_PAYMENT': True,
+   ```
+   <p dir="rtl"> توصیه میشه True باشه.</p>
+   <p dir="rtl"> درصورتی که مقدار برابر با True قرار بگیرد تابع redirect_gateway از دسترس خارج میشودو باید از تابع get_gateway استفاده شود.</p>
+1. `CUSTOM_APP` : <br>
+   ```
+   CUSTOM_APP : 'api:payment',
+   ```
+   <p dir="rtl">
+   اگر نیاز ندارید توابع داخلی را اوررایت کنیدو فقط به این نیاز دارید که مسیر یو ار ال های داخلی را در اپ جداگانه ای قرارگیرد میتوانید از این گزینه برای ادرسی دهی محل قرار گیری اپ استفاده کنید 
+   </p>
 ### urls.py
 
 <p dir="rtl">
  در فایل `urls.py`
 </p>
 
 ```python
@@ -163,15 +190,15 @@
 
 <h4 dir="rtl">اگر از reverse proxy و https استفاده می کنید برای رفع موارد احتمالی حتما تنظیمات این <a href="https://stackoverflow.com/questions/62047354/build-absolute-uri-with-https-behind-reverse-proxy/65934202#65934202">لینک</a> را انجام دهید.</h4>
 
 
 <h1 dir="rtl">نحوه استفاده</h1>
 <h2 dir="rtl">ارسال به بانک</h2>
 
-
+<h3 dir="rtl">برای وقتی که تنظیمات IS_SAFE_GET_GATEWAY_PAYMENT': False'</h3>
 <p dir="rtl">
  برای استفاده و اتصال به درگاه بانک کافی است یک `BankFactory` ایجاد کنیم و پارامترهای اجباری را تنظیم کنیم. سپس کاربر را می توانیم به درگاه بانک هدایت  کنیم.
 </p>
 
   
 ```python
 import logging
@@ -203,22 +230,109 @@
         return bank.redirect_gateway()
     except AZBankGatewaysException as e:
         logging.critical(e)
         # TODO: redirect to failed page.
         raise e
 
 ```
+
+<h3 dir="rtl">برای وقتی که تنظیمات IS_SAFE_GET_GATEWAY_PAYMENT': True'</h3>
+<p dir="rtl">
+ در این قسمت مثل مثال قبل عمل میکنیم تنها تفاوت این است که از تابع get_gateway بجای redirect_gateway استفاده میکنیم دلیل این کار افزایش امنیت و تغییر صفحهredirect میباشد. 
+</p>
+
+  
+```python
+import logging
+from django.urls import reverse
+from django.shortcuts import render
+from azbankgateways import bankfactories, models as bank_models, default_settings as settings
+from azbankgateways.exceptions import AZBankGatewaysException
+
+
+def go_to_gateway_view(request):
+    # خواندن مبلغ از هر جایی که مد نظر است
+    amount = 1000
+    # تنظیم شماره موبایل کاربر از هر جایی که مد نظر است
+    user_mobile_number = '+989112221234'  # اختیاری
+
+    factory = bankfactories.BankFactory()
+    try:
+        bank = factory.auto_create() # or factory.create(bank_models.BankType.BMI) or set identifier
+        bank.set_request(request)
+        bank.set_amount(amount)
+        # یو آر ال بازگشت به نرم افزار برای ادامه فرآیند
+        bank.set_client_callback_url(reverse('callback-gateway'))
+        bank.set_mobile_number(user_mobile_number)  # اختیاری
+    
+        # در صورت تمایل اتصال این رکورد به رکورد فاکتور یا هر چیزی که بعدا بتوانید ارتباط بین محصول یا خدمات را با این
+        # پرداخت برقرار کنید. 
+        bank_record = bank.ready()
+        
+        # هدایت کاربر به درگاه بانک
+        context = bank.get_gateway()
+        return render(request, 'redirect_to_bank.html', context=context)
+    except AZBankGatewaysException as e:
+        logging.critical(e)
+        return render(request, 'redirect_to_bank.html')
+
+```
+
 <p dir="rtl"> 
 در صورتیکه تمایل دارید به صورت خودکار به اولین درگاه در دسترس متصل شوید. ابتدا از قسمت تنظیمات در بخش `BANK_PRIORITIES
 ` اولویت های بانک های مد نظر را وارید کنید. سپس به جای استفاده از متد `factory.create` از متد ‍`factory.auto_create` در این بخش استفاده کنید.
 به متد auto_create می توانید مبلغ مد نظر را نیز برای صحت سنجی از حداقل مبلغ نیز ارسال کنید.
  </p>
 
 `set_mobile_number` متدی است که پارامتر شماره موبایل کاربری که قصد خرید دارد را به آن پاس میدهیم. این شماره موبایل جهت پرداخت و پیگیری آسان تر به درگاه ارسال می شود
 
+<h2 dir="rtl">ساخت صفحه redirect_to_bank.html </h2>
+<p dir="rtl"> 
+این صفحه درصورتی کارمیکند که IS_SAFE_GET_GATEWAY_PAYMENT': True' و view مربوطه تنظیم شود.<br> برای این کار در پوشه templates پروژه فایل redirect_to_bank.html را ایجاد کرده و محتوای زیر را در آن قرار میدیم (میتونید با سلیقه خودتون سفاریشی کنید) 
+ </p>
+
+```html
+<!DOCTYPE html>
+<html lang="fa">
+<head>
+    <meta charset="UTF-8">
+    <title>انتقال به درگاه پرداخت</title>
+</head>
+<body>
+
+   {% if url %}
+     <h5>در حال اتصال به درگاه پرداخت ...</h5>
+   {% else %}
+     <h5>خطا در ارتباط با درگاه</h5>
+   {% endif %}
+   
+   {% if url %}
+      <form id='id_form' action="{{ url }}" method="{{ method }}">
+          {% csrf_token %}
+          {% for key, value in params.items %}
+              <input type="hidden" name="{{ key }}" value="{{ value }}">
+          {% endfor %}
+      </form>
+      
+      <script type="text/javascript">
+          window.onload = function () {
+      
+              function submitForm() {
+                  document.forms['id_form'].submit();
+              }
+      
+              submitForm();
+          }
+      </script>
+   {% endif %}
+</body>
+</html>
+```
+
+
 <h2 dir="rtl">بازگشت از بانک</h2>
 
 <p dir="rtl"> 
 وضعیت رکورد بانک به شرح ذیل می باشد.
  </p>
 
 1. `WAITING`: در انتظار برای انتقال کاربر به درگاه بانک
@@ -343,15 +457,17 @@
 * [mash5026](https://github.com/mash5026) برای رفع مشکل unmarshalling ERROR: For input string
 * [hypy13](https://github.com/hypy13) برای آپدیت به ورژن های بالاتر از جنگو ۳.۲
 * [jam4li](https://github.com/jam4li) برای اضافه کردن سندباکس زرین پال
 * [ravexina](https://github.com/ravexina) رفع مشکل تسویه حساب بانک ملت
 * [nimaes80](https://github.com/nimaes80) اضافه کردن درگاه pay.ir ورژن یک
 * [khademmilad](https://github.com/khademmilad) پشتیبانی از پایتون ۳.۱۰ و ۳.۱۱
 * [Saman-Zand-H](https://github.com/Saman-Zand-H) رفع مشکل اتصال pay.ir در برخی موارد
-
+* [MrMRM1](https://github.com/MrMRM1)  [بابت رفع مشکل امنیتی](https://github.com/ali-zahedi/az-iranian-bank-gateways/pull/65#issuecomment-1624927632)
+* [MrMRM1](https://github.com/MrMRM1) اضافه شدن قابلیت اوررایت یا تغییر ادرس یو آر ال های پیشفرض
+  
 ## License
 
 The MIT License (MIT). Please see [License File](LICENSE) for more information.
 
 
 [لینک]: https://stackoverflow.com/questions/62047354/build-absolute-uri-with-https-behind-reverse-proxy/65934202#65934202را
```

### Comparing `az-iranian-bank-gateways-1.8.5/az_iranian_bank_gateways.egg-info/PKG-INFO` & `az-iranian-bank-gateways-1.9.0a1/az_iranian_bank_gateways.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: az-iranian-bank-gateways
-Version: 1.8.5
+Version: 1.9.0a1
 Summary: Iranian Bank Gateways for django
 Home-page: https://github.com/ali-zahedi/az-iranian-bank-gateways
 Author: Ali Zahedigol
 Author-email: alizahedigol@gmail.com
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `az-iranian-bank-gateways-1.8.5/az_iranian_bank_gateways.egg-info/SOURCES.txt` & `az-iranian-bank-gateways-1.9.0a1/az_iranian_bank_gateways.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/admin.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/admin.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/bankfactories.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/bankfactories.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/banks/bahamta.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/banks/bahamta.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/banks/banks.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/banks/banks.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from .. import default_settings as settings
 from ..exceptions import (
     AmountDoesNotSupport,
     BankGatewayStateInvalid,
     BankGatewayTokenExpired,
     CurrencyDoesNotSupport,
+    SafeSettingsEnabled,
 )
 from ..models import Bank, CurrencyEnum, PaymentStatus
 from ..utils import append_querystring
 
 
 # TODO: handle and expire record after 15 minutes
 @six.add_metaclass(abc.ABCMeta)
@@ -305,24 +306,44 @@
         """این متد بسته به بانک متفاوت پر می شود."""
         """
         :return
         method: POST, GET
         """
         pass
 
-    def redirect_gateway(self):
-        """کاربر را به درگاه بانک هدایت می کند"""
+    def _verify_payment_expiry(self):
+        """برسی میکند درگاه ساخته شده اعتبار دارد یا خیر"""
         if (timezone.now() - self._bank.created_at).seconds > 120:
             self._set_payment_status(PaymentStatus.EXPIRE_GATEWAY_TOKEN)
             logging.debug("Redirect to bank expire!")
             raise BankGatewayTokenExpired()
+
+    def redirect_gateway(self):
+        """کاربر را به درگاه بانک هدایت می کند"""
+        self._verify_payment_expiry()
+        if settings.IS_SAFE_GET_GATEWAY_PAYMENT:
+            raise SafeSettingsEnabled()
         logging.debug("Redirect to bank")
         self._set_payment_status(PaymentStatus.REDIRECT_TO_BANK)
         return redirect(self.get_gateway_payment_url())
 
+    def get_gateway(self):
+        """اطلاعات درگاه پرداخت را برمیگرداند"""
+        self._verify_payment_expiry()
+        logging.debug("Redirect to bank")
+        self._set_payment_status(PaymentStatus.REDIRECT_TO_BANK)
+        return self.safe_get_gateway_payment_url()
+
+    def safe_get_gateway_payment_url(self):
+        url = self._get_gateway_payment_url_parameter()
+        params = self._get_gateway_payment_parameter()
+        method = self._get_gateway_payment_method_parameter()
+        context = {"params": params, "url": url, "method": method}
+        return context
+
     def get_gateway_payment_url(self):
         redirect_url = reverse(settings.GO_TO_BANK_GATEWAY_NAMESPACE)
         url = self._get_gateway_payment_url_parameter()
         params = self._get_gateway_payment_parameter()
         method = self._get_gateway_payment_method_parameter()
         params.update(
             {
```

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/banks/bmi.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/banks/bmi.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/banks/idpay.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/banks/idpay.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/banks/mellat.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/banks/mellat.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/banks/payV1.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/banks/payV1.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/banks/sep.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/banks/sep.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/banks/zarinpal.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/banks/zarinpal.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/banks/zibal.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/banks/zibal.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/default_settings.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/default_settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,10 +33,22 @@
 BANK_DEFAULT = _AZ_IRANIAN_BANK_GATEWAYS.get("DEFAULT", "BMI")
 SETTING_VALUE_READER_CLASS = _AZ_IRANIAN_BANK_GATEWAYS.get(
     "SETTING_VALUE_READER_CLASS", "azbankgateways.readers.DefaultReader"
 )
 CURRENCY = _AZ_IRANIAN_BANK_GATEWAYS.get("CURRENCY", "IRR")
 TRACKING_CODE_QUERY_PARAM = _AZ_IRANIAN_BANK_GATEWAYS.get("TRACKING_CODE_QUERY_PARAM", "tc")
 TRACKING_CODE_LENGTH = _AZ_IRANIAN_BANK_GATEWAYS.get("TRACKING_CODE_LENGTH", 16)
-CALLBACK_NAMESPACE = f"{AZIranianBankGatewaysConfig.name}:callback"
-GO_TO_BANK_GATEWAY_NAMESPACE = f"{AZIranianBankGatewaysConfig.name}:go-to-bank-gateway"
 IS_SAMPLE_FORM_ENABLE = _AZ_IRANIAN_BANK_GATEWAYS.get("IS_SAMPLE_FORM_ENABLE", False)
+IS_SAFE_GET_GATEWAY_PAYMENT = _AZ_IRANIAN_BANK_GATEWAYS.get("IS_SAFE_GET_GATEWAY_PAYMENT", False)
+CUSTOM_APP = _AZ_IRANIAN_BANK_GATEWAYS.get("CUSTOM_APP", None)
+if CUSTOM_APP:
+    CALLBACK_NAMESPACE = f"{CUSTOM_APP}:{AZIranianBankGatewaysConfig.name}:callback"
+    GO_TO_BANK_GATEWAY_NAMESPACE = f"{CUSTOM_APP}:{AZIranianBankGatewaysConfig.name}:go-to-bank-gateway"
+    SAMPLE_RESULT_NAMESPACE = f"{CUSTOM_APP}:{AZIranianBankGatewaysConfig.name}:sample-result"
+else:
+    CALLBACK_NAMESPACE = _AZ_IRANIAN_BANK_GATEWAYS.get("CALLBACK_NAMESPACE", f"{AZIranianBankGatewaysConfig.name}:callback")
+    GO_TO_BANK_GATEWAY_NAMESPACE = _AZ_IRANIAN_BANK_GATEWAYS.get(
+        "GO_TO_BANK_GATEWAY_NAMESPACE", f"{AZIranianBankGatewaysConfig.name}:go-to-bank-gateway"
+    )
+    SAMPLE_RESULT_NAMESPACE = _AZ_IRANIAN_BANK_GATEWAYS.get(
+        "SAMPLE_RESULT_NAMESPACE", f"{AZIranianBankGatewaysConfig.name}:sample-result"
+    )
```

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/locale/en/LC_MESSAGES/django.po` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/locale/fa/LC_MESSAGES/django.mo` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/locale/fa/LC_MESSAGES/django.po` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/migrations/0001_initial.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/migrations/0002_auto_20210102_0721.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/migrations/0002_auto_20210102_0721.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/migrations/0003_bank_bank_choose_identifier.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/migrations/0003_bank_bank_choose_identifier.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/migrations/0004_auto_20211115_1500.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/migrations/0004_auto_20211115_1500.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/models/banks.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/models/banks.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/models/enum.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/models/enum.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/models/enum_django.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/models/enum_django.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/readers/bases.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/readers/bases.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/readers/defaults.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/readers/defaults.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/templates/azbankgateways/redirect_to_bank.html` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/templates/azbankgateways/redirect_to_bank.html`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/templates/azbankgateways/samples/base.html` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/templates/azbankgateways/samples/base.html`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/templates/azbankgateways/samples/gateway.html` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/templates/azbankgateways/samples/gateway.html`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/templates/azbankgateways/samples/result.html` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/templates/azbankgateways/samples/result.html`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         <div class="card text-center">
             <div class="card-header">
                {{ bank_record.bank_type }} - نتیجه پرداخت
             </div>
             <div class="card-body">
                 <h5 class="card-title {% if bank_record.is_success %}bg-success{% else %}bg-danger{% endif %}">{% if bank_record.is_success %}پرداخت موفق{% else %}پرداخت نا موفق{% endif %}</h5>
                 <p class="card-text">{{ bank_record.tracking_code }} - {{ bank_record.reference_number }} - {{ bank_record.response_result }} - {{ bank_record.extra_information }}</p>
-                <a href="{% url 'azbankgateways:sample-payment' %}" class="btn btn-primary">Go somewhere</a>
+                <a href="{{ bank_record.callback_url|cut:'/sample-result/'|add:'/sample-payment/' }}" class="btn btn-primary">Go somewhere</a>
             </div>
             <div class="card-footer text-muted">
                 {{ bank_record.created_at }}
             </div>
         </div>
     </div>
 {% endblock %}
```

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/urls.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/urls.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,17 +9,21 @@
     sample_result_view,
 )
 
 app_name = AZIranianBankGatewaysConfig.name
 
 _urlpatterns = [
     path("callback/", callback_view, name="callback"),
-    path("go-to-bank-gateway/", go_to_bank_gateway, name="go-to-bank-gateway"),
 ]
 
+if not settings.IS_SAFE_GET_GATEWAY_PAYMENT:
+    _urlpatterns += [
+        path("go-to-bank-gateway/", go_to_bank_gateway, name="go-to-bank-gateway"),
+    ]
+
 if settings.IS_SAMPLE_FORM_ENABLE:
     _urlpatterns += [
         path("sample-payment/", sample_payment_view, name="sample-payment"),
         path("sample-result/", sample_result_view, name="sample-result"),
     ]
```

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/utils.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/utils.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/views/banks.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/views/banks.py`

 * *Files identical despite different names*

### Comparing `az-iranian-bank-gateways-1.8.5/azbankgateways/views/samples.py` & `az-iranian-bank-gateways-1.9.0a1/azbankgateways/views/samples.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,24 +24,26 @@
             mobile_number = form.cleaned_data["mobile_number"]
             factory = bankfactories.BankFactory()
             try:
                 bank = factory.auto_create()
                 bank.set_request(request)
                 bank.set_amount(amount)
                 # یو آر ال بازگشت به نرم افزار برای ادامه فرآیند
-                bank.set_client_callback_url(reverse(f"{AZIranianBankGatewaysConfig.name}:sample-result"))
+                bank.set_client_callback_url(reverse(settings.SAMPLE_RESULT_NAMESPACE))
                 bank.set_mobile_number(mobile_number)  # اختیاری
 
                 # در صورت تمایل اتصال این رکورد به رکورد فاکتور یا هر چیزی که
                 # بعدا بتوانید ارتباط بین محصول یا خدمات را با این
                 # پرداخت برقرار کنید.
 
                 bank_record = bank.ready()  # noqa
 
                 # هدایت کاربر به درگاه بانک
+                if settings.IS_SAMPLE_FORM_ENABLE:
+                    return render(request, 'azbankgateways/redirect_to_bank.html', context=bank.get_gateway())
                 return bank.redirect_gateway()
             except AZBankGatewaysException as e:
                 logging.critical(e)
                 # TODO: redirect to failed result.
                 raise e
 
     # if a GET (or any other method) we'll create a blank form
```

### Comparing `az-iranian-bank-gateways-1.8.5/setup.cfg` & `az-iranian-bank-gateways-1.9.0a1/setup.cfg`

 * *Files identical despite different names*

