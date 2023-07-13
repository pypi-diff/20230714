# Comparing `tmp/stripe-5.5.0b5.tar.gz` & `tmp/stripe-5.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stripe-5.5.0b5.tar", last modified: Thu Jun 22 20:53:39 2023, max compression
+gzip compressed data, was "stripe-5.6.0b1.tar", last modified: Thu Jul 13 22:56:51 2023, max compression
```

## Comparing `stripe-5.5.0b5.tar` & `stripe-5.6.0b1.tar`

### file list

```diff
@@ -1,334 +1,335 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.450146 stripe-5.5.0b5/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-22 20:53:19.000000 stripe-5.5.0b5/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-22 20:53:19.000000 stripe-5.5.0b5/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)    48386 2023-06-22 20:53:19.000000 stripe-5.5.0b5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-22 20:53:19.000000 stripe-5.5.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-22 20:53:19.000000 stripe-5.5.0b5/LONG_DESCRIPTION.rst
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-22 20:53:19.000000 stripe-5.5.0b5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-22 20:53:39.450146 stripe-5.5.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-06-22 20:53:19.000000 stripe-5.5.0b5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-22 20:53:19.000000 stripe-5.5.0b5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.418146 stripe-5.5.0b5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-22 20:53:19.000000 stripe-5.5.0b5/examples/charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-22 20:53:19.000000 stripe-5.5.0b5/examples/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-22 20:53:19.000000 stripe-5.5.0b5/examples/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-22 20:53:19.000000 stripe-5.5.0b5/examples/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-22 20:53:19.000000 stripe-5.5.0b5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-22 20:53:39.450146 stripe-5.5.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-22 20:53:19.000000 stripe-5.5.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.422146 stripe-5.5.0b5/stripe/
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_requestor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.430146 stripe-5.5.0b5/stripe/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.430146 stripe-5.5.0b5/stripe/api_resources/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/createable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/custom_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/deletable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/listable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/nested_resource_class_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/searchable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/singleton_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/updateable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/verify_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/account_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/account_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/apple_pay_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/application_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/application_fee_refund.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.430146 stripe-5.5.0b5/stripe/api_resources/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/apps/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/bank_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.430146 stripe-5.5.0b5/stripe/api_resources/billing_portal/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/billing_portal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/billing_portal/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/billing_portal/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/capability.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.430146 stripe-5.5.0b5/stripe/api_resources/capital/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/capital/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/capital/financing_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/capital/financing_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/capital/financing_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/cash_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/charge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.430146 stripe-5.5.0b5/stripe/api_resources/checkout/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/checkout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/checkout/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/country_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/coupon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/credit_note.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/credit_note_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/customer_balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/customer_cash_balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/customer_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/ephemeral_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/error_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/exchange_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/file_link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.434146 stripe-5.5.0b5/stripe/api_resources/financial_connections/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/financial_connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/financial_connections/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/financial_connections/account_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/financial_connections/account_ownership.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/financial_connections/inferred_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/financial_connections/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/financial_connections/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/funding_instructions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.434146 stripe-5.5.0b5/stripe/api_resources/gift_cards/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/gift_cards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/gift_cards/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/gift_cards/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.434146 stripe-5.5.0b5/stripe/api_resources/identity/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/identity/verification_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/identity/verification_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/invoice_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/invoice_line_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.434146 stripe-5.5.0b5/stripe/api_resources/issuing/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/issuing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/issuing/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/issuing/card.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/issuing/card_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/issuing/card_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/issuing/cardholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/issuing/dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/issuing/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/list_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/login_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/mandate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/payment_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/payment_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/payment_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/payout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/product.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/promotion_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    12693 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/quote_phase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.434146 stripe-5.5.0b5/stripe/api_resources/radar/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/radar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/radar/early_fraud_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/radar/value_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/radar/value_list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/recipient_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/refund.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.434146 stripe-5.5.0b5/stripe/api_resources/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/reporting/report_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/reporting/report_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/review.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/search_result_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/setup_attempt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/setup_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/shipping_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.434146 stripe-5.5.0b5/stripe/api_resources/sigma/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/sigma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/sigma/scheduled_query_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/source.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/source_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/subscription_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/subscription_schedule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.434146 stripe-5.5.0b5/stripe/api_resources/tax/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/tax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/tax/calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/tax/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/tax/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/tax/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/tax_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/tax_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/tax_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.438146 stripe-5.5.0b5/stripe/api_resources/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/terminal/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/terminal/connection_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/terminal/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/terminal/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.438146 stripe-5.5.0b5/stripe/api_resources/test_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/test_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/test_helpers/test_clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/topup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.438146 stripe-5.5.0b5/stripe/api_resources/treasury/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/credit_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/debit_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/financial_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/inbound_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/outbound_payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/outbound_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/received_credit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/received_debit.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/transaction_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/usage_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/usage_record_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/webhook_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.438146 stripe-5.5.0b5/stripe/data/
--rw-r--r--   0 runner    (1001) docker     (123)   215352 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/data/ca-certificates.crt
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    25754 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/multipart_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/oauth_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/object_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/raw_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/request_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    34581 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/six.py
--rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/stripe_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/stripe_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.422146 stripe-5.5.0b5/stripe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-22 20:53:39.000000 stripe-5.5.0b5/stripe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-06-22 20:53:39.000000 stripe-5.5.0b5/stripe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:53:39.000000 stripe-5.5.0b5/stripe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:53:39.000000 stripe-5.5.0b5/stripe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-22 20:53:39.000000 stripe-5.5.0b5/stripe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 20:53:39.000000 stripe-5.5.0b5/stripe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.442146 stripe-5.5.0b5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.446146 stripe-5.5.0b5/tests/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.450146 stripe-5.5.0b5/tests/api_resources/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/test_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/test_createable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/test_custom_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/test_deletable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/test_listable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/test_nested_resource_class_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/test_searchable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/test_singleton_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/test_test_helpers_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/test_updateable_api_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.450146 stripe-5.5.0b5/tests/api_resources/billing_portal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/billing_portal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/billing_portal/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/billing_portal/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.450146 stripe-5.5.0b5/tests/api_resources/checkout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/checkout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/checkout/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.450146 stripe-5.5.0b5/tests/api_resources/identity/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/identity/test_verification_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/identity/test_verification_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.450146 stripe-5.5.0b5/tests/api_resources/issuing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/issuing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/issuing/test_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/issuing/test_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/issuing/test_cardholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/issuing/test_dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/issuing/test_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.450146 stripe-5.5.0b5/tests/api_resources/radar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/radar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/radar/test_early_fraud_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/radar/test_value_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/radar/test_value_list_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.450146 stripe-5.5.0b5/tests/api_resources/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/reporting/test_report_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/reporting/test_report_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.450146 stripe-5.5.0b5/tests/api_resources/sigma/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/sigma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/sigma/test_scheduled_query_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.450146 stripe-5.5.0b5/tests/api_resources/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/terminal/test_connection_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/terminal/test_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/terminal/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_account_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_apple_pay_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_application_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_application_fee_refund.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_capability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_charge.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_country_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_coupon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_credit_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_customer_balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_ephemeral_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_exchange_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_file_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_file_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_invoice_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_invoice_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_list_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_mandate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_payment_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_payment_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_payout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_person.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_price.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_product.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_promotion_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_refund.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_review.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_search_result_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_setup_attempt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_setup_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_source_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_subscription_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_subscription_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_tax_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_tax_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_tax_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_topup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_usage_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_usage_record_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_webhook_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/request_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/stripe_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_api_requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)   116386 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_generated_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)    34161 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9928 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_multipart_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_oauth_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_raw_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_stripe_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_stripe_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.213709 stripe-5.6.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-13 22:56:28.000000 stripe-5.6.0b1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-13 22:56:28.000000 stripe-5.6.0b1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)    50537 2023-07-13 22:56:28.000000 stripe-5.6.0b1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-13 22:56:28.000000 stripe-5.6.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-13 22:56:28.000000 stripe-5.6.0b1/LONG_DESCRIPTION.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-13 22:56:28.000000 stripe-5.6.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-13 22:56:51.213709 stripe-5.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-07-13 22:56:28.000000 stripe-5.6.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 22:56:28.000000 stripe-5.6.0b1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.173709 stripe-5.6.0b1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-13 22:56:28.000000 stripe-5.6.0b1/examples/charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-13 22:56:28.000000 stripe-5.6.0b1/examples/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-13 22:56:28.000000 stripe-5.6.0b1/examples/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-13 22:56:28.000000 stripe-5.6.0b1/examples/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 22:56:28.000000 stripe-5.6.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-13 22:56:51.213709 stripe-5.6.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-13 22:56:28.000000 stripe-5.6.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.177709 stripe-5.6.0b1/stripe/
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_requestor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.185709 stripe-5.6.0b1/stripe/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.189709 stripe-5.6.0b1/stripe/api_resources/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/abstract/api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/abstract/createable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/abstract/custom_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/abstract/deletable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/abstract/listable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/abstract/nested_resource_class_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/abstract/searchable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/abstract/singleton_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/abstract/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/abstract/updateable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/abstract/verify_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/account_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/account_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/apple_pay_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/application_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/application_fee_refund.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.189709 stripe-5.6.0b1/stripe/api_resources/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/apps/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/bank_account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.189709 stripe-5.6.0b1/stripe/api_resources/billing_portal/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/billing_portal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/billing_portal/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/billing_portal/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/capability.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.189709 stripe-5.6.0b1/stripe/api_resources/capital/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/capital/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/capital/financing_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/capital/financing_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/capital/financing_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/cash_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/charge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.189709 stripe-5.6.0b1/stripe/api_resources/checkout/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/checkout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/checkout/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/country_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/coupon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/credit_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/credit_note_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/customer_balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/customer_cash_balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/customer_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/ephemeral_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/error_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/exchange_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/file_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.189709 stripe-5.6.0b1/stripe/api_resources/financial_connections/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/financial_connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/financial_connections/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/financial_connections/account_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/financial_connections/account_ownership.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/financial_connections/inferred_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/financial_connections/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/financial_connections/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/funding_instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.193709 stripe-5.6.0b1/stripe/api_resources/gift_cards/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/gift_cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/gift_cards/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/gift_cards/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.193709 stripe-5.6.0b1/stripe/api_resources/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/identity/verification_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/identity/verification_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/invoice_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/invoice_line_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.193709 stripe-5.6.0b1/stripe/api_resources/issuing/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/issuing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/issuing/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/issuing/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/issuing/card_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/issuing/card_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/issuing/cardholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/issuing/dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/issuing/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/list_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/login_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/mandate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/payment_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/payment_method_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/payout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/promotion_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12693 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/quote_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.193709 stripe-5.6.0b1/stripe/api_resources/radar/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/radar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/radar/early_fraud_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/radar/value_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/radar/value_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/recipient_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/refund.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.193709 stripe-5.6.0b1/stripe/api_resources/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/reporting/report_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/reporting/report_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/review.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/search_result_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/setup_attempt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/setup_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/shipping_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.193709 stripe-5.6.0b1/stripe/api_resources/sigma/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/sigma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/sigma/scheduled_query_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/source_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/subscription_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/subscription_schedule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.193709 stripe-5.6.0b1/stripe/api_resources/tax/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/tax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/tax/calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/tax/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/tax/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/tax/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/tax_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/tax_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/tax_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.197709 stripe-5.6.0b1/stripe/api_resources/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/terminal/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/terminal/connection_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/terminal/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/terminal/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.197709 stripe-5.6.0b1/stripe/api_resources/test_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/test_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/test_helpers/test_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/topup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.197709 stripe-5.6.0b1/stripe/api_resources/treasury/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/treasury/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/treasury/credit_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/treasury/debit_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/treasury/financial_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/treasury/inbound_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/treasury/outbound_payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/treasury/outbound_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/treasury/received_credit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/treasury/received_debit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/treasury/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/treasury/transaction_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/usage_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/usage_record_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_resources/webhook_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/api_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.197709 stripe-5.6.0b1/stripe/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   215352 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/data/ca-certificates.crt
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25754 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/multipart_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/oauth_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/object_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/raw_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/request_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34581 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/six.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/stripe_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/stripe_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-13 22:56:28.000000 stripe-5.6.0b1/stripe/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.177709 stripe-5.6.0b1/stripe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-13 22:56:51.000000 stripe-5.6.0b1/stripe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11615 2023-07-13 22:56:51.000000 stripe-5.6.0b1/stripe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 22:56:51.000000 stripe-5.6.0b1/stripe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 22:56:51.000000 stripe-5.6.0b1/stripe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-13 22:56:51.000000 stripe-5.6.0b1/stripe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 22:56:51.000000 stripe-5.6.0b1/stripe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.201709 stripe-5.6.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.209709 stripe-5.6.0b1/tests/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.209709 stripe-5.6.0b1/tests/api_resources/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/abstract/test_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/abstract/test_createable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/abstract/test_custom_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/abstract/test_deletable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/abstract/test_listable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/abstract/test_nested_resource_class_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/abstract/test_searchable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/abstract/test_singleton_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/abstract/test_test_helpers_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/abstract/test_updateable_api_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.209709 stripe-5.6.0b1/tests/api_resources/billing_portal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/billing_portal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/billing_portal/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/billing_portal/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.209709 stripe-5.6.0b1/tests/api_resources/checkout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/checkout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/checkout/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.209709 stripe-5.6.0b1/tests/api_resources/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/identity/test_verification_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/identity/test_verification_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.213709 stripe-5.6.0b1/tests/api_resources/issuing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/issuing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/issuing/test_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/issuing/test_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/issuing/test_cardholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/issuing/test_dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/issuing/test_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.213709 stripe-5.6.0b1/tests/api_resources/radar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/radar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/radar/test_early_fraud_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/radar/test_value_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/radar/test_value_list_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.213709 stripe-5.6.0b1/tests/api_resources/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/reporting/test_report_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/reporting/test_report_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.213709 stripe-5.6.0b1/tests/api_resources/sigma/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/sigma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/sigma/test_scheduled_query_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:51.213709 stripe-5.6.0b1/tests/api_resources/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/terminal/test_connection_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/terminal/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/terminal/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_account_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_apple_pay_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_application_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_application_fee_refund.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_capability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_country_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_coupon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_credit_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_customer_balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_ephemeral_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_exchange_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_file_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_invoice_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_invoice_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_list_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_mandate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_payout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_promotion_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_refund.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_review.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_search_result_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_setup_attempt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_setup_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_source_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_subscription_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_subscription_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_tax_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_tax_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_tax_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_topup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_usage_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_usage_record_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/api_resources/test_webhook_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/request_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/stripe_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/test_api_requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116386 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/test_generated_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34161 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9928 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/test_multipart_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/test_oauth_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/test_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/test_raw_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/test_stripe_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/test_stripe_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tests/test_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-13 22:56:28.000000 stripe-5.6.0b1/tox.ini
```

### Comparing `stripe-5.5.0b5/CHANGELOG.md` & `stripe-5.6.0b1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,47 @@
 # Changelog
 
+## 5.6.0b1 - 2023-07-13
+* [#991](https://github.com/stripe/stripe-python/pull/991) Update generated code for beta
+  Release specs are identical.
+* [#989](https://github.com/stripe/stripe-python/pull/989) Update generated code for beta
+  * Add support for new resource `PaymentMethodConfiguration`
+  * Add support for `create`, `list`, `modify`, and `retrieve` methods on resource `PaymentMethodConfiguration`
+* [#985](https://github.com/stripe/stripe-python/pull/985) Update generated code for beta
+
+* [#986](https://github.com/stripe/stripe-python/pull/986) Consolidate beta SDKs section
+
+## 5.5.0 - 2023-07-13
+* [#990](https://github.com/stripe/stripe-python/pull/990) Update generated code
+  * Add support for new resource `Tax.Settings`
+  * Add support for `modify` and `retrieve` methods on resource `Settings`
+* [#981](https://github.com/stripe/stripe-python/pull/981) Update generated code
+
+* [#984](https://github.com/stripe/stripe-python/pull/984) Stop testing Python 2.7
+* [#978](https://github.com/stripe/stripe-python/pull/978) Update generated code
+  * Release specs are identical.
+* [#977](https://github.com/stripe/stripe-python/pull/977) Add information about accessing response headers
+* [#972](https://github.com/stripe/stripe-python/pull/972) Update generated code
+
+* [#975](https://github.com/stripe/stripe-python/pull/975) Add constraints.txt
+* [#974](https://github.com/stripe/stripe-python/pull/974) Pin cryptography version
+* [#970](https://github.com/stripe/stripe-python/pull/970) Update generated code
+
+* [#967](https://github.com/stripe/stripe-python/pull/967) Update generated code
+  
+  Documentation updates.
+* [#963](https://github.com/stripe/stripe-python/pull/963) Update generated code
+
+* [#962](https://github.com/stripe/stripe-python/pull/962) ci: Fix github action warnings
+* [#960](https://github.com/stripe/stripe-python/pull/960) Fix build status badge in README.md
+* [#955](https://github.com/stripe/stripe-python/pull/955) Update generated code
+
+* [#958](https://github.com/stripe/stripe-python/pull/958) Fix coveralls condition
+* [#952](https://github.com/stripe/stripe-python/pull/952) Update generated code
+
 ## 5.5.0b5 - 2023-06-22
 * [#982](https://github.com/stripe/stripe-python/pull/982) Update generated code for beta
   * Add support for new resource `CustomerSession`
   * Add support for `create` method on resource `CustomerSession`
 * [#979](https://github.com/stripe/stripe-python/pull/979) Update generated code for beta
 * [#976](https://github.com/stripe/stripe-python/pull/976) Update generated code for beta
 
@@ -15,25 +53,22 @@
 ## 5.5.0b3 - 2023-05-19
 * [#966](https://github.com/stripe/stripe-python/pull/966) Update generated code for beta
   * Add support for `subscribe` and `unsubscribe` methods on resource `FinancialConnections.Account`
 * [#965](https://github.com/stripe/stripe-python/pull/965) Add raw_request
 * [#964](https://github.com/stripe/stripe-python/pull/964) Update generated code for beta
 * [#961](https://github.com/stripe/stripe-python/pull/961) Update generated code for beta
 
-
 ## 5.5.0b2 - 2023-04-13
 * [#954](https://github.com/stripe/stripe-python/pull/954) Update generated code for beta
   * Add support for `collect_payment_method` and `confirm_payment_intent` methods on resource `Terminal.Reader`
 * [#953](https://github.com/stripe/stripe-python/pull/953) Update generated code for beta
 
-
 ## 5.5.0b1 - 2023-03-30
 * [#950](https://github.com/stripe/stripe-python/pull/950) Update generated code for beta
 
-
 ## 5.4.0 - 2023-03-30
 * [#951](https://github.com/stripe/stripe-python/pull/951) Update generated code
   * Remove support for `create` method on resource `Tax.Transaction`
     * This is not a breaking change, as this method was deprecated before the Tax Transactions API was released in favor of the `create_from_calculation` method.
 
 ## 5.4.0b1 - 2023-03-23
 * [#941](https://github.com/stripe/stripe-python/pull/941) Update generated code for beta (new)
```

### Comparing `stripe-5.5.0b5/LICENSE` & `stripe-5.6.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/LONG_DESCRIPTION.rst` & `stripe-5.6.0b1/LONG_DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/PKG-INFO` & `stripe-5.6.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stripe
-Version: 5.5.0b5
+Version: 5.6.0b1
 Summary: Python bindings for the Stripe API
 Home-page: https://github.com/stripe/stripe-python
 Author: Stripe
 Author-email: support@stripe.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/stripe/stripe-python/issues
 Project-URL: Changes, https://github.com/stripe/stripe-python/blob/master/CHANGELOG.md
```

### Comparing `stripe-5.5.0b5/README.md` & `stripe-5.6.0b1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     import logging
     logging.basicConfig()
     logging.getLogger('stripe').setLevel(logging.DEBUG)
     ```
 
 ### Accessing response code and headers
 
-You can access the HTTP response code and headers using the `last_response` property of the returned resource. 
+You can access the HTTP response code and headers using the `last_response` property of the returned resource.
 
 ```python
 customer = stripe.Customer.retrieve(
     "cus_123456789"
 )
 
 print(customer.last_response.code)
@@ -202,38 +202,38 @@
 We would love for you to try these and share feedback with us before these features reach the stable phase.
 To install a beta version use `pip install` with the exact version you'd like to use:
 
 ```
 pip install stripe==5.3.0b3
 ```
 
+> **Note**
+> There can be breaking changes between beta versions. Therefore we recommend pinning the package version to a specific beta version in your [requirements file](https://pip.pypa.io/en/stable/user_guide/#requirements-files) or `setup.py`. This way you can install the same version each time without breaking changes unless you are intentionally looking for the latest beta version.
+
+We highly recommend keeping an eye on when the beta feature you are interested in goes from beta to stable so that you can move from using a beta version of the SDK to the stable version.
+
+If your beta feature requires a `Stripe-Version` header to be sent, use the `stripe.api_version` field to set it:
+
+```python
+stripe.api_version += "; feature_beta=v3"
+```
+
 ### Custom requests
 
 If you would like to send a request to an undocumented API (for example you are in a private beta), or if you prefer to bypass the method definitions in the library and specify your request details directly, you can use the `raw_request` method on `stripe`.
 
 ```python
 response = stripe.raw_request(
     "post", "/v1/beta_endpoint", param=123, stripe_version="2022-11-15; feature_beta=v3"
 )
 
 # (Optional) response is a StripeResponse. You can use `stripe.deserialize` to get a StripeObject.
 deserialized_resp = stripe.deserialize(response)
 ```
 
-> **Note**
-> There can be breaking changes between beta versions. Therefore we recommend pinning the package version to a specific beta version in your [requirements file](https://pip.pypa.io/en/stable/user_guide/#requirements-files) or `setup.py`. This way you can install the same version each time without breaking changes unless you are intentionally looking for the latest beta version.
-
-We highly recommend keeping an eye on when the beta feature you are interested in goes from beta to stable so that you can move from using a beta version of the SDK to the stable version.
-
-If your beta feature requires a `Stripe-Version` header to be sent, use the `stripe.api_version` field to set it:
-
-```python
-stripe.api_version += "; feature_beta=v3"
-```
-
 ## Support
 
 New features and bug fixes are released on the latest major version of the Stripe Python library. If you are on an older major version, we recommend that you upgrade to the latest in order to use the new features and bug fixes including those for security vulnerabilities. Older major versions of the package will continue to be available for use, but will not be receiving any updates.
 
 ## Development
 
 The test suite depends on [stripe-mock], so make sure to fetch and run it from a
```

### Comparing `stripe-5.5.0b5/examples/oauth.py` & `stripe-5.6.0b1/examples/oauth.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/examples/proxy.py` & `stripe-5.6.0b1/examples/proxy.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/examples/webhooks.py` & `stripe-5.6.0b1/examples/webhooks.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/setup.py` & `stripe-5.6.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/__init__.py` & `stripe-5.6.0b1/stripe/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_requestor.py` & `stripe-5.6.0b1/stripe/api_requestor.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/__init__.py` & `stripe-5.6.0b1/stripe/api_resources/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,17 @@
 from stripe.api_resources.line_item import LineItem
 from stripe.api_resources.login_link import LoginLink
 from stripe.api_resources.mandate import Mandate
 from stripe.api_resources.order import Order
 from stripe.api_resources.payment_intent import PaymentIntent
 from stripe.api_resources.payment_link import PaymentLink
 from stripe.api_resources.payment_method import PaymentMethod
+from stripe.api_resources.payment_method_configuration import (
+    PaymentMethodConfiguration,
+)
 from stripe.api_resources.payout import Payout
 from stripe.api_resources.person import Person
 from stripe.api_resources.plan import Plan
 from stripe.api_resources.price import Price
 from stripe.api_resources.product import Product
 from stripe.api_resources.promotion_code import PromotionCode
 from stripe.api_resources.quote import Quote
```

### Comparing `stripe-5.5.0b5/stripe/api_resources/abstract/__init__.py` & `stripe-5.6.0b1/stripe/api_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/abstract/api_resource.py` & `stripe-5.6.0b1/stripe/api_resources/abstract/api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/abstract/createable_api_resource.py` & `stripe-5.6.0b1/stripe/api_resources/abstract/createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/abstract/custom_method.py` & `stripe-5.6.0b1/stripe/api_resources/abstract/custom_method.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/abstract/deletable_api_resource.py` & `stripe-5.6.0b1/stripe/api_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/abstract/listable_api_resource.py` & `stripe-5.6.0b1/stripe/api_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/abstract/nested_resource_class_methods.py` & `stripe-5.6.0b1/stripe/api_resources/abstract/nested_resource_class_methods.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/abstract/searchable_api_resource.py` & `stripe-5.6.0b1/stripe/api_resources/abstract/searchable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/abstract/singleton_api_resource.py` & `stripe-5.6.0b1/stripe/api_resources/abstract/singleton_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/abstract/test_helpers.py` & `stripe-5.6.0b1/stripe/api_resources/abstract/test_helpers.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/abstract/updateable_api_resource.py` & `stripe-5.6.0b1/stripe/api_resources/abstract/updateable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/account.py` & `stripe-5.6.0b1/stripe/api_resources/account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/account_link.py` & `stripe-5.6.0b1/stripe/api_resources/account_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/account_session.py` & `stripe-5.6.0b1/stripe/api_resources/account_session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/apple_pay_domain.py` & `stripe-5.6.0b1/stripe/api_resources/apple_pay_domain.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/application_fee.py` & `stripe-5.6.0b1/stripe/api_resources/application_fee.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/application_fee_refund.py` & `stripe-5.6.0b1/stripe/api_resources/application_fee_refund.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/apps/secret.py` & `stripe-5.6.0b1/stripe/api_resources/apps/secret.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/balance.py` & `stripe-5.6.0b1/stripe/api_resources/balance.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/balance_transaction.py` & `stripe-5.6.0b1/stripe/api_resources/balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/bank_account.py` & `stripe-5.6.0b1/stripe/api_resources/bank_account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/billing_portal/configuration.py` & `stripe-5.6.0b1/stripe/api_resources/billing_portal/configuration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/billing_portal/session.py` & `stripe-5.6.0b1/stripe/api_resources/billing_portal/session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/capability.py` & `stripe-5.6.0b1/stripe/api_resources/capability.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/capital/financing_offer.py` & `stripe-5.6.0b1/stripe/api_resources/capital/financing_offer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/capital/financing_summary.py` & `stripe-5.6.0b1/stripe/api_resources/capital/financing_summary.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/card.py` & `stripe-5.6.0b1/stripe/api_resources/card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/cash_balance.py` & `stripe-5.6.0b1/stripe/api_resources/cash_balance.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/charge.py` & `stripe-5.6.0b1/stripe/api_resources/charge.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/checkout/session.py` & `stripe-5.6.0b1/stripe/api_resources/checkout/session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/country_spec.py` & `stripe-5.6.0b1/stripe/api_resources/country_spec.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/coupon.py` & `stripe-5.6.0b1/stripe/api_resources/coupon.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/credit_note.py` & `stripe-5.6.0b1/stripe/api_resources/credit_note.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/customer.py` & `stripe-5.6.0b1/stripe/api_resources/customer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/customer_balance_transaction.py` & `stripe-5.6.0b1/stripe/api_resources/customer_balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/customer_cash_balance_transaction.py` & `stripe-5.6.0b1/stripe/api_resources/customer_cash_balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/dispute.py` & `stripe-5.6.0b1/stripe/api_resources/dispute.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/ephemeral_key.py` & `stripe-5.6.0b1/stripe/api_resources/ephemeral_key.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/error_object.py` & `stripe-5.6.0b1/stripe/api_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/event.py` & `stripe-5.6.0b1/stripe/api_resources/event.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/exchange_rate.py` & `stripe-5.6.0b1/stripe/api_resources/exchange_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/file.py` & `stripe-5.6.0b1/stripe/api_resources/file.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/file_link.py` & `stripe-5.6.0b1/stripe/api_resources/file_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/financial_connections/__init__.py` & `stripe-5.6.0b1/stripe/api_resources/financial_connections/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/financial_connections/account.py` & `stripe-5.6.0b1/stripe/api_resources/financial_connections/account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/funding_instructions.py` & `stripe-5.6.0b1/stripe/api_resources/funding_instructions.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/gift_cards/card.py` & `stripe-5.6.0b1/stripe/api_resources/gift_cards/card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/gift_cards/transaction.py` & `stripe-5.6.0b1/stripe/api_resources/gift_cards/transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/identity/verification_report.py` & `stripe-5.6.0b1/stripe/api_resources/identity/verification_report.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/identity/verification_session.py` & `stripe-5.6.0b1/stripe/api_resources/identity/verification_session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/invoice.py` & `stripe-5.6.0b1/stripe/api_resources/invoice.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/invoice_item.py` & `stripe-5.6.0b1/stripe/api_resources/invoice_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/issuing/__init__.py` & `stripe-5.6.0b1/stripe/api_resources/issuing/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/issuing/authorization.py` & `stripe-5.6.0b1/stripe/api_resources/issuing/authorization.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/issuing/card.py` & `stripe-5.6.0b1/stripe/api_resources/issuing/card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/issuing/card_design.py` & `stripe-5.6.0b1/stripe/api_resources/issuing/card_design.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/issuing/cardholder.py` & `stripe-5.6.0b1/stripe/api_resources/issuing/cardholder.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/issuing/dispute.py` & `stripe-5.6.0b1/stripe/api_resources/issuing/dispute.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/issuing/transaction.py` & `stripe-5.6.0b1/stripe/api_resources/issuing/transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/list_object.py` & `stripe-5.6.0b1/stripe/api_resources/list_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/order.py` & `stripe-5.6.0b1/stripe/api_resources/order.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/payment_intent.py` & `stripe-5.6.0b1/stripe/api_resources/payment_intent.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/payment_link.py` & `stripe-5.6.0b1/stripe/api_resources/payment_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/payment_method.py` & `stripe-5.6.0b1/stripe/api_resources/payment_method.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/payout.py` & `stripe-5.6.0b1/stripe/api_resources/payout.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/person.py` & `stripe-5.6.0b1/stripe/api_resources/person.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/plan.py` & `stripe-5.6.0b1/stripe/api_resources/plan.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/price.py` & `stripe-5.6.0b1/stripe/api_resources/price.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/product.py` & `stripe-5.6.0b1/stripe/api_resources/product.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/promotion_code.py` & `stripe-5.6.0b1/stripe/api_resources/promotion_code.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/quote.py` & `stripe-5.6.0b1/stripe/api_resources/quote.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/quote_phase.py` & `stripe-5.6.0b1/stripe/api_resources/quote_phase.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/radar/early_fraud_warning.py` & `stripe-5.6.0b1/stripe/api_resources/radar/early_fraud_warning.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/radar/value_list.py` & `stripe-5.6.0b1/stripe/api_resources/radar/value_list.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/radar/value_list_item.py` & `stripe-5.6.0b1/stripe/api_resources/radar/value_list_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/refund.py` & `stripe-5.6.0b1/stripe/api_resources/refund.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/reporting/report_run.py` & `stripe-5.6.0b1/stripe/api_resources/reporting/report_run.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/reporting/report_type.py` & `stripe-5.6.0b1/stripe/api_resources/reporting/report_type.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/reversal.py` & `stripe-5.6.0b1/stripe/api_resources/reversal.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/review.py` & `stripe-5.6.0b1/stripe/api_resources/review.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/search_result_object.py` & `stripe-5.6.0b1/stripe/api_resources/search_result_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/setup_attempt.py` & `stripe-5.6.0b1/stripe/api_resources/setup_attempt.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/setup_intent.py` & `stripe-5.6.0b1/stripe/api_resources/setup_intent.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/shipping_rate.py` & `stripe-5.6.0b1/stripe/api_resources/shipping_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/sigma/scheduled_query_run.py` & `stripe-5.6.0b1/stripe/api_resources/sigma/scheduled_query_run.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/source.py` & `stripe-5.6.0b1/stripe/api_resources/source.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/source_transaction.py` & `stripe-5.6.0b1/stripe/api_resources/source_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/subscription.py` & `stripe-5.6.0b1/stripe/api_resources/subscription.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/subscription_item.py` & `stripe-5.6.0b1/stripe/api_resources/subscription_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/subscription_schedule.py` & `stripe-5.6.0b1/stripe/api_resources/subscription_schedule.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/tax/calculation.py` & `stripe-5.6.0b1/stripe/api_resources/tax/calculation.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/tax/registration.py` & `stripe-5.6.0b1/stripe/api_resources/tax/registration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/tax/settings.py` & `stripe-5.6.0b1/stripe/api_resources/tax/settings.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/tax/transaction.py` & `stripe-5.6.0b1/stripe/api_resources/tax/transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/tax_id.py` & `stripe-5.6.0b1/stripe/api_resources/tax_id.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/tax_rate.py` & `stripe-5.6.0b1/stripe/api_resources/tax_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/terminal/configuration.py` & `stripe-5.6.0b1/stripe/api_resources/terminal/configuration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/terminal/location.py` & `stripe-5.6.0b1/stripe/api_resources/terminal/location.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/terminal/reader.py` & `stripe-5.6.0b1/stripe/api_resources/terminal/reader.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/test_helpers/test_clock.py` & `stripe-5.6.0b1/stripe/api_resources/test_helpers/test_clock.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/token.py` & `stripe-5.6.0b1/stripe/api_resources/token.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/topup.py` & `stripe-5.6.0b1/stripe/api_resources/topup.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/transfer.py` & `stripe-5.6.0b1/stripe/api_resources/transfer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/treasury/__init__.py` & `stripe-5.6.0b1/stripe/api_resources/treasury/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/treasury/credit_reversal.py` & `stripe-5.6.0b1/stripe/api_resources/treasury/credit_reversal.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/treasury/debit_reversal.py` & `stripe-5.6.0b1/stripe/api_resources/treasury/debit_reversal.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/treasury/financial_account.py` & `stripe-5.6.0b1/stripe/api_resources/treasury/financial_account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/treasury/inbound_transfer.py` & `stripe-5.6.0b1/stripe/api_resources/treasury/inbound_transfer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/treasury/outbound_payment.py` & `stripe-5.6.0b1/stripe/api_resources/treasury/outbound_payment.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/treasury/outbound_transfer.py` & `stripe-5.6.0b1/stripe/api_resources/treasury/outbound_transfer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/treasury/received_credit.py` & `stripe-5.6.0b1/stripe/api_resources/treasury/received_credit.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/treasury/received_debit.py` & `stripe-5.6.0b1/stripe/api_resources/treasury/received_debit.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/treasury/transaction_entry.py` & `stripe-5.6.0b1/stripe/api_resources/treasury/transaction_entry.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/usage_record.py` & `stripe-5.6.0b1/stripe/api_resources/usage_record.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/api_resources/webhook_endpoint.py` & `stripe-5.6.0b1/stripe/api_resources/webhook_endpoint.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/data/ca-certificates.crt` & `stripe-5.6.0b1/stripe/data/ca-certificates.crt`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/error.py` & `stripe-5.6.0b1/stripe/error.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/http_client.py` & `stripe-5.6.0b1/stripe/http_client.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/multipart_data_generator.py` & `stripe-5.6.0b1/stripe/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/oauth.py` & `stripe-5.6.0b1/stripe/oauth.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/oauth_error.py` & `stripe-5.6.0b1/stripe/oauth_error.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/object_classes.py` & `stripe-5.6.0b1/stripe/object_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     api_resources.LineItem.OBJECT_NAME: api_resources.LineItem,
     api_resources.LoginLink.OBJECT_NAME: api_resources.LoginLink,
     api_resources.Mandate.OBJECT_NAME: api_resources.Mandate,
     api_resources.Order.OBJECT_NAME: api_resources.Order,
     api_resources.PaymentIntent.OBJECT_NAME: api_resources.PaymentIntent,
     api_resources.PaymentLink.OBJECT_NAME: api_resources.PaymentLink,
     api_resources.PaymentMethod.OBJECT_NAME: api_resources.PaymentMethod,
+    api_resources.PaymentMethodConfiguration.OBJECT_NAME: api_resources.PaymentMethodConfiguration,
     api_resources.Payout.OBJECT_NAME: api_resources.Payout,
     api_resources.Person.OBJECT_NAME: api_resources.Person,
     api_resources.Plan.OBJECT_NAME: api_resources.Plan,
     api_resources.Price.OBJECT_NAME: api_resources.Price,
     api_resources.Product.OBJECT_NAME: api_resources.Product,
     api_resources.PromotionCode.OBJECT_NAME: api_resources.PromotionCode,
     api_resources.Quote.OBJECT_NAME: api_resources.Quote,
```

### Comparing `stripe-5.5.0b5/stripe/preview.py` & `stripe-5.6.0b1/stripe/preview.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/raw_request.py` & `stripe-5.6.0b1/stripe/raw_request.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/six.py` & `stripe-5.6.0b1/stripe/six.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/stripe_object.py` & `stripe-5.6.0b1/stripe/stripe_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/stripe_response.py` & `stripe-5.6.0b1/stripe/stripe_response.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/util.py` & `stripe-5.6.0b1/stripe/util.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe/webhook.py` & `stripe-5.6.0b1/stripe/webhook.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/stripe.egg-info/PKG-INFO` & `stripe-5.6.0b1/stripe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stripe
-Version: 5.5.0b5
+Version: 5.6.0b1
 Summary: Python bindings for the Stripe API
 Home-page: https://github.com/stripe/stripe-python
 Author: Stripe
 Author-email: support@stripe.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/stripe/stripe-python/issues
 Project-URL: Changes, https://github.com/stripe/stripe-python/blob/master/CHANGELOG.md
```

### Comparing `stripe-5.5.0b5/stripe.egg-info/SOURCES.txt` & `stripe-5.6.0b1/stripe.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 stripe/api_resources/list_object.py
 stripe/api_resources/login_link.py
 stripe/api_resources/mandate.py
 stripe/api_resources/order.py
 stripe/api_resources/payment_intent.py
 stripe/api_resources/payment_link.py
 stripe/api_resources/payment_method.py
+stripe/api_resources/payment_method_configuration.py
 stripe/api_resources/payout.py
 stripe/api_resources/person.py
 stripe/api_resources/plan.py
 stripe/api_resources/price.py
 stripe/api_resources/product.py
 stripe/api_resources/promotion_code.py
 stripe/api_resources/quote.py
```

### Comparing `stripe-5.5.0b5/tests/api_resources/abstract/test_api_resource.py` & `stripe-5.6.0b1/tests/api_resources/abstract/test_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/abstract/test_createable_api_resource.py` & `stripe-5.6.0b1/tests/api_resources/abstract/test_createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/abstract/test_custom_method.py` & `stripe-5.6.0b1/tests/api_resources/abstract/test_custom_method.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/abstract/test_deletable_api_resource.py` & `stripe-5.6.0b1/tests/api_resources/abstract/test_deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/abstract/test_listable_api_resource.py` & `stripe-5.6.0b1/tests/api_resources/abstract/test_listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/abstract/test_nested_resource_class_methods.py` & `stripe-5.6.0b1/tests/api_resources/abstract/test_nested_resource_class_methods.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/abstract/test_searchable_api_resource.py` & `stripe-5.6.0b1/tests/api_resources/abstract/test_searchable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/abstract/test_singleton_api_resource.py` & `stripe-5.6.0b1/tests/api_resources/abstract/test_singleton_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/abstract/test_test_helpers_api_resource.py` & `stripe-5.6.0b1/tests/api_resources/abstract/test_test_helpers_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/abstract/test_updateable_api_resource.py` & `stripe-5.6.0b1/tests/api_resources/abstract/test_updateable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/billing_portal/test_configuration.py` & `stripe-5.6.0b1/tests/api_resources/billing_portal/test_configuration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/checkout/test_session.py` & `stripe-5.6.0b1/tests/api_resources/checkout/test_session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/identity/test_verification_report.py` & `stripe-5.6.0b1/tests/api_resources/identity/test_verification_report.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/identity/test_verification_session.py` & `stripe-5.6.0b1/tests/api_resources/identity/test_verification_session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/issuing/test_authorization.py` & `stripe-5.6.0b1/tests/api_resources/issuing/test_authorization.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/issuing/test_card.py` & `stripe-5.6.0b1/tests/api_resources/issuing/test_card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/issuing/test_cardholder.py` & `stripe-5.6.0b1/tests/api_resources/issuing/test_cardholder.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/issuing/test_dispute.py` & `stripe-5.6.0b1/tests/api_resources/issuing/test_dispute.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/issuing/test_transaction.py` & `stripe-5.6.0b1/tests/api_resources/issuing/test_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/radar/test_early_fraud_warning.py` & `stripe-5.6.0b1/tests/api_resources/radar/test_early_fraud_warning.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/radar/test_value_list.py` & `stripe-5.6.0b1/tests/api_resources/radar/test_value_list.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/radar/test_value_list_item.py` & `stripe-5.6.0b1/tests/api_resources/radar/test_value_list_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/reporting/test_report_run.py` & `stripe-5.6.0b1/tests/api_resources/reporting/test_report_run.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/reporting/test_report_type.py` & `stripe-5.6.0b1/tests/api_resources/reporting/test_report_type.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/sigma/test_scheduled_query_run.py` & `stripe-5.6.0b1/tests/api_resources/sigma/test_scheduled_query_run.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/terminal/test_location.py` & `stripe-5.6.0b1/tests/api_resources/terminal/test_location.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/terminal/test_reader.py` & `stripe-5.6.0b1/tests/api_resources/terminal/test_reader.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_account.py` & `stripe-5.6.0b1/tests/api_resources/test_account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_account_link.py` & `stripe-5.6.0b1/tests/api_resources/test_account_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_apple_pay_domain.py` & `stripe-5.6.0b1/tests/api_resources/test_apple_pay_domain.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_application_fee.py` & `stripe-5.6.0b1/tests/api_resources/test_application_fee.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_application_fee_refund.py` & `stripe-5.6.0b1/tests/api_resources/test_application_fee_refund.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_balance_transaction.py` & `stripe-5.6.0b1/tests/api_resources/test_balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_bank_account.py` & `stripe-5.6.0b1/tests/api_resources/test_bank_account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_capability.py` & `stripe-5.6.0b1/tests/api_resources/test_capability.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_card.py` & `stripe-5.6.0b1/tests/api_resources/test_card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_charge.py` & `stripe-5.6.0b1/tests/api_resources/test_charge.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_country_spec.py` & `stripe-5.6.0b1/tests/api_resources/test_country_spec.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_coupon.py` & `stripe-5.6.0b1/tests/api_resources/test_coupon.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_credit_note.py` & `stripe-5.6.0b1/tests/api_resources/test_credit_note.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_customer.py` & `stripe-5.6.0b1/tests/api_resources/test_customer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_customer_balance_transaction.py` & `stripe-5.6.0b1/tests/api_resources/test_customer_balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_dispute.py` & `stripe-5.6.0b1/tests/api_resources/test_dispute.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_ephemeral_key.py` & `stripe-5.6.0b1/tests/api_resources/test_ephemeral_key.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_event.py` & `stripe-5.6.0b1/tests/api_resources/test_event.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_exchange_rate.py` & `stripe-5.6.0b1/tests/api_resources/test_exchange_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_file.py` & `stripe-5.6.0b1/tests/api_resources/test_file.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_file_link.py` & `stripe-5.6.0b1/tests/api_resources/test_file_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_file_upload.py` & `stripe-5.6.0b1/tests/api_resources/test_file_upload.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_invoice.py` & `stripe-5.6.0b1/tests/api_resources/test_invoice.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_invoice_item.py` & `stripe-5.6.0b1/tests/api_resources/test_invoice_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_list_object.py` & `stripe-5.6.0b1/tests/api_resources/test_list_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_payment_intent.py` & `stripe-5.6.0b1/tests/api_resources/test_payment_intent.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_payment_method.py` & `stripe-5.6.0b1/tests/api_resources/test_payment_method.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_payout.py` & `stripe-5.6.0b1/tests/api_resources/test_payout.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_person.py` & `stripe-5.6.0b1/tests/api_resources/test_person.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_plan.py` & `stripe-5.6.0b1/tests/api_resources/test_plan.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_price.py` & `stripe-5.6.0b1/tests/api_resources/test_price.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_product.py` & `stripe-5.6.0b1/tests/api_resources/test_product.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_promotion_code.py` & `stripe-5.6.0b1/tests/api_resources/test_promotion_code.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_quote.py` & `stripe-5.6.0b1/tests/api_resources/test_quote.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_refund.py` & `stripe-5.6.0b1/tests/api_resources/test_refund.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_reversal.py` & `stripe-5.6.0b1/tests/api_resources/test_reversal.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_review.py` & `stripe-5.6.0b1/tests/api_resources/test_review.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_search_result_object.py` & `stripe-5.6.0b1/tests/api_resources/test_search_result_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_setup_intent.py` & `stripe-5.6.0b1/tests/api_resources/test_setup_intent.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_source.py` & `stripe-5.6.0b1/tests/api_resources/test_source.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_source_transaction.py` & `stripe-5.6.0b1/tests/api_resources/test_source_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_subscription.py` & `stripe-5.6.0b1/tests/api_resources/test_subscription.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_subscription_item.py` & `stripe-5.6.0b1/tests/api_resources/test_subscription_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_subscription_schedule.py` & `stripe-5.6.0b1/tests/api_resources/test_subscription_schedule.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_tax_code.py` & `stripe-5.6.0b1/tests/api_resources/test_tax_code.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_tax_id.py` & `stripe-5.6.0b1/tests/api_resources/test_tax_id.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_tax_rate.py` & `stripe-5.6.0b1/tests/api_resources/test_tax_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_topup.py` & `stripe-5.6.0b1/tests/api_resources/test_topup.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_transfer.py` & `stripe-5.6.0b1/tests/api_resources/test_transfer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_usage_record.py` & `stripe-5.6.0b1/tests/api_resources/test_usage_record.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_usage_record_summary.py` & `stripe-5.6.0b1/tests/api_resources/test_usage_record_summary.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/api_resources/test_webhook_endpoint.py` & `stripe-5.6.0b1/tests/api_resources/test_webhook_endpoint.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/conftest.py` & `stripe-5.6.0b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/request_mock.py` & `stripe-5.6.0b1/tests/request_mock.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/stripe_mock.py` & `stripe-5.6.0b1/tests/stripe_mock.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/test_api_requestor.py` & `stripe-5.6.0b1/tests/test_api_requestor.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/test_error.py` & `stripe-5.6.0b1/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/test_generated_examples.py` & `stripe-5.6.0b1/tests/test_generated_examples.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/test_http_client.py` & `stripe-5.6.0b1/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/test_integration.py` & `stripe-5.6.0b1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/test_multipart_data_generator.py` & `stripe-5.6.0b1/tests/test_multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/test_oauth.py` & `stripe-5.6.0b1/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/test_preview.py` & `stripe-5.6.0b1/tests/test_preview.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/test_raw_request.py` & `stripe-5.6.0b1/tests/test_raw_request.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/test_stripe_object.py` & `stripe-5.6.0b1/tests/test_stripe_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/test_stripe_response.py` & `stripe-5.6.0b1/tests/test_stripe_response.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/test_util.py` & `stripe-5.6.0b1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tests/test_webhook.py` & `stripe-5.6.0b1/tests/test_webhook.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b5/tox.ini` & `stripe-5.6.0b1/tox.ini`

 * *Files identical despite different names*

