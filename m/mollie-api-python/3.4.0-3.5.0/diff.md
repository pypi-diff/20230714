# Comparing `tmp/mollie-api-python-3.4.0.tar.gz` & `tmp/mollie-api-python-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mollie-api-python-3.4.0.tar", last modified: Thu Jul  6 07:12:20 2023, max compression
+gzip compressed data, was "mollie-api-python-3.5.0.tar", last modified: Fri Jul 14 11:00:29 2023, max compression
```

## Comparing `mollie-api-python-3.4.0.tar` & `mollie-api-python-3.5.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:12:20.579783 mollie-api-python-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-07-06 07:12:20.579783 mollie-api-python-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:12:20.571782 mollie-api-python-3.4.0/mollie/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:12:20.571782 mollie-api-python-3.4.0/mollie/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:12:20.575783 mollie-api-python-3.4.0/mollie/api/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/balance_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/capture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/chargeback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/issuer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/mandate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/onboarding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/order_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/payment_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/refund.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/settlement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/shipment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:12:20.579783 mollie-api-python-3.4.0/mollie/api/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/balances.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/captures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/chargebacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/customers.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/invoices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/mandates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/onboarding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/order_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/payment_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/payments.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/refunds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/settlements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/shipments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:12:20.579783 mollie-api-python-3.4.0/mollie_api_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-07-06 07:12:20.000000 mollie-api-python-3.4.0/mollie_api_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-06 07:12:20.000000 mollie-api-python-3.4.0/mollie_api_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:12:20.000000 mollie-api-python-3.4.0/mollie_api_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-06 07:12:20.000000 mollie-api-python-3.4.0/mollie_api_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 07:12:20.000000 mollie-api-python-3.4.0/mollie_api_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 07:12:20.579783 mollie-api-python-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:00:29.397591 mollie-api-python-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-07-14 11:00:29.397591 mollie-api-python-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:00:29.381591 mollie-api-python-3.5.0/mollie/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:00:29.381591 mollie-api-python-3.5.0/mollie/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:00:29.389591 mollie-api-python-3.5.0/mollie/api/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/balance_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/chargeback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/issuer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/mandate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/onboarding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/order_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/payment_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/refund.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/settlement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/shipment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/objects/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:00:29.393591 mollie-api-python-3.5.0/mollie/api/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/balances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/captures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/chargebacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/customers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/invoices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/mandates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/onboarding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/order_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/payment_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/payments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/refunds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/settlements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/shipments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/resources/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/mollie/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:00:29.397591 mollie-api-python-3.5.0/mollie_api_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-07-14 11:00:29.000000 mollie-api-python-3.5.0/mollie_api_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-14 11:00:29.000000 mollie-api-python-3.5.0/mollie_api_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:00:29.000000 mollie-api-python-3.5.0/mollie_api_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-14 11:00:29.000000 mollie-api-python-3.5.0/mollie_api_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 11:00:29.000000 mollie-api-python-3.5.0/mollie_api_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 11:00:29.397591 mollie-api-python-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-14 11:00:15.000000 mollie-api-python-3.5.0/setup.py
```

### Comparing `mollie-api-python-3.4.0/LICENSE.txt` & `mollie-api-python-3.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/PKG-INFO` & `mollie-api-python-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mollie-api-python
-Version: 3.4.0
+Version: 3.5.0
 Summary: Mollie API client for Python
 Home-page: https://github.com/mollie/mollie-api-python
 Author: Mollie B.V.
 Author-email: info@mollie.com
 Maintainer: Four Digits B.V.
 Maintainer-email: info@fourdigits.nl
 License: BSD
```

### Comparing `mollie-api-python-3.4.0/README.md` & `mollie-api-python-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/client.py` & `mollie-api-python-3.5.0/mollie/api/client.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/error.py` & `mollie-api-python-3.5.0/mollie/api/error.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/balance.py` & `mollie-api-python-3.5.0/mollie/api/objects/balance.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/balance_report.py` & `mollie-api-python-3.5.0/mollie/api/objects/balance_report.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/balance_transaction.py` & `mollie-api-python-3.5.0/mollie/api/objects/balance_transaction.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/base.py` & `mollie-api-python-3.5.0/mollie/api/objects/base.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/capture.py` & `mollie-api-python-3.5.0/mollie/api/objects/capture.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/chargeback.py` & `mollie-api-python-3.5.0/mollie/api/objects/chargeback.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/client.py` & `mollie-api-python-3.5.0/mollie/api/objects/client.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/customer.py` & `mollie-api-python-3.5.0/mollie/api/objects/customer.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/invoice.py` & `mollie-api-python-3.5.0/mollie/api/objects/invoice.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/issuer.py` & `mollie-api-python-3.5.0/mollie/api/objects/issuer.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/list.py` & `mollie-api-python-3.5.0/mollie/api/objects/list.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/mandate.py` & `mollie-api-python-3.5.0/mollie/api/objects/mandate.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/method.py` & `mollie-api-python-3.5.0/mollie/api/objects/method.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/onboarding.py` & `mollie-api-python-3.5.0/mollie/api/objects/onboarding.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/order.py` & `mollie-api-python-3.5.0/mollie/api/objects/order.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/order_line.py` & `mollie-api-python-3.5.0/mollie/api/objects/order_line.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/organization.py` & `mollie-api-python-3.5.0/mollie/api/objects/organization.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/payment.py` & `mollie-api-python-3.5.0/mollie/api/objects/payment.py`

 * *Files 8% similar despite different names*

```diff
@@ -198,14 +198,26 @@
     @property
     def captures(self):
         """Return the captures related to this payment"""
         from ..resources import PaymentCaptures
 
         return PaymentCaptures(self.client, self)
 
+    @property
+    def capture_before(self):
+        return self._get_property("captureBefore")
+
+    @property
+    def capture_mode(self):
+        return self._get_property("captureMode")
+
+    @property
+    def capture_delay(self):
+        return self._get_property("captureDelay")
+
     def get_settlement(self):
         """Return the settlement for this payment."""
         if self.settlement_id:
             return self.client.settlements.get(self.settlement_id)
 
     def get_mandate(self):
         """Return the mandate for this payment."""
```

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/payment_link.py` & `mollie-api-python-3.5.0/mollie/api/objects/payment_link.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/permission.py` & `mollie-api-python-3.5.0/mollie/api/objects/permission.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/profile.py` & `mollie-api-python-3.5.0/mollie/api/objects/profile.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/refund.py` & `mollie-api-python-3.5.0/mollie/api/objects/refund.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/settlement.py` & `mollie-api-python-3.5.0/mollie/api/objects/settlement.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/shipment.py` & `mollie-api-python-3.5.0/mollie/api/objects/shipment.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/objects/subscription.py` & `mollie-api-python-3.5.0/mollie/api/objects/subscription.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/__init__.py` & `mollie-api-python-3.5.0/mollie/api/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/balances.py` & `mollie-api-python-3.5.0/mollie/api/resources/balances.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/base.py` & `mollie-api-python-3.5.0/mollie/api/resources/base.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/captures.py` & `mollie-api-python-3.5.0/mollie/api/resources/captures.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import TYPE_CHECKING, Any
 
 from ..objects.capture import Capture
-from .base import ResourceBase, ResourceGetMixin, ResourceListMixin
+from .base import ResourceBase, ResourceCreateMixin, ResourceGetMixin, ResourceListMixin
 
 if TYPE_CHECKING:
     from ..client import Client
     from ..objects.payment import Payment
     from ..objects.settlement import Settlement
 
 __all__ = [
@@ -17,15 +17,15 @@
 class CapturesBase(ResourceBase):
     RESOURCE_ID_PREFIX: str = "cpt_"
 
     def get_resource_object(self, result: dict) -> Capture:
         return Capture(result, self.client)
 
 
-class PaymentCaptures(CapturesBase, ResourceGetMixin, ResourceListMixin):
+class PaymentCaptures(CapturesBase, ResourceGetMixin, ResourceListMixin, ResourceCreateMixin):
     """Resource handler for the `/payments/:payment_id:/captures` endpoint."""
 
     _payment: "Payment"
 
     def __init__(self, client: "Client", payment: "Payment") -> None:
         self._payment = payment
         super().__init__(client)
```

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/chargebacks.py` & `mollie-api-python-3.5.0/mollie/api/resources/chargebacks.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/clients.py` & `mollie-api-python-3.5.0/mollie/api/resources/clients.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/customers.py` & `mollie-api-python-3.5.0/mollie/api/resources/customers.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/invoices.py` & `mollie-api-python-3.5.0/mollie/api/resources/invoices.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/mandates.py` & `mollie-api-python-3.5.0/mollie/api/resources/mandates.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/methods.py` & `mollie-api-python-3.5.0/mollie/api/resources/methods.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/onboarding.py` & `mollie-api-python-3.5.0/mollie/api/resources/onboarding.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/order_lines.py` & `mollie-api-python-3.5.0/mollie/api/resources/order_lines.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/orders.py` & `mollie-api-python-3.5.0/mollie/api/resources/orders.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/organizations.py` & `mollie-api-python-3.5.0/mollie/api/resources/organizations.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/payment_links.py` & `mollie-api-python-3.5.0/mollie/api/resources/payment_links.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/payments.py` & `mollie-api-python-3.5.0/mollie/api/resources/payments.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/permissions.py` & `mollie-api-python-3.5.0/mollie/api/resources/permissions.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/profiles.py` & `mollie-api-python-3.5.0/mollie/api/resources/profiles.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/refunds.py` & `mollie-api-python-3.5.0/mollie/api/resources/refunds.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/settlements.py` & `mollie-api-python-3.5.0/mollie/api/resources/settlements.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/shipments.py` & `mollie-api-python-3.5.0/mollie/api/resources/shipments.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie/api/resources/subscriptions.py` & `mollie-api-python-3.5.0/mollie/api/resources/subscriptions.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/mollie_api_python.egg-info/PKG-INFO` & `mollie-api-python-3.5.0/mollie_api_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mollie-api-python
-Version: 3.4.0
+Version: 3.5.0
 Summary: Mollie API client for Python
 Home-page: https://github.com/mollie/mollie-api-python
 Author: Mollie B.V.
 Author-email: info@mollie.com
 Maintainer: Four Digits B.V.
 Maintainer-email: info@fourdigits.nl
 License: BSD
```

### Comparing `mollie-api-python-3.4.0/mollie_api_python.egg-info/SOURCES.txt` & `mollie-api-python-3.5.0/mollie_api_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.4.0/setup.py` & `mollie-api-python-3.5.0/setup.py`

 * *Files identical despite different names*

