# Comparing `tmp/Adyen-9.0.0.tar.gz` & `tmp/Adyen-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Adyen-9.0.0.tar", last modified: Fri Jun 30 13:00:28 2023, max compression
+gzip compressed data, was "Adyen-9.0.1.tar", last modified: Fri Jul 14 12:57:05 2023, max compression
```

## Comparing `Adyen-9.0.0.tar` & `Adyen-9.0.1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.789552 Adyen-9.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.777551 Adyen-9.0.0/Adyen/
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23474 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/httpclient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.777551 Adyen-9.0.0/Adyen/services/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.781551 Adyen-9.0.0/Adyen/services/balancePlatform/
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/balancePlatform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/balancePlatform/account_holders_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/balancePlatform/balance_accounts_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/balancePlatform/bank_account_validation_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/balancePlatform/grant_accounts_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/balancePlatform/grant_offers_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/balancePlatform/payment_instrument_groups_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/balancePlatform/payment_instruments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/balancePlatform/platform_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/balancePlatform/transaction_rules_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/binlookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.781551 Adyen-9.0.0/Adyen/services/checkout/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/checkout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/checkout/classic_checkout_sdk_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/checkout/modifications_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/checkout/orders_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/checkout/payment_links_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/checkout/payments_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/checkout/recurring_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/checkout/utility_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/dataProtection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.781551 Adyen-9.0.0/Adyen/services/legalEntityManagement/
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/legalEntityManagement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/legalEntityManagement/business_lines_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/legalEntityManagement/documents_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/legalEntityManagement/hosted_onboarding_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/legalEntityManagement/legal_entities_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/legalEntityManagement/pci_questionnaires_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/legalEntityManagement/terms_of_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/legalEntityManagement/transfer_instruments_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.785551 Adyen-9.0.0/Adyen/services/management/
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/account_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/account_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/account_store_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/allowed_origins_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/allowed_origins_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/api_credentials_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/api_credentials_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/api_key_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/api_key_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/client_key_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/client_key_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/my_api_credential_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/payment_methods_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/payout_settings_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/split_configuration_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/terminal_actions_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/terminal_actions_terminal_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/terminal_orders_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/terminal_orders_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/terminal_settings_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/terminal_settings_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/terminal_settings_store_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/terminal_settings_terminal_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/terminals_terminal_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/users_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/users_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/webhooks_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/management/webhooks_merchant_level_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.785551 Adyen-9.0.0/Adyen/services/payments/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/payments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/payments/general_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/payments/modifications_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.785551 Adyen-9.0.0/Adyen/services/payouts/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/payouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/payouts/initialization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/payouts/instant_payouts_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/payouts/reviewing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/recurring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/storedValue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.785551 Adyen-9.0.0/Adyen/services/transfers/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/transfers/capital_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/transfers/transactions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/services/transfers/transfers_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-30 13:00:17.000000 Adyen-9.0.0/Adyen/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.777551 Adyen-9.0.0/Adyen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-30 13:00:28.000000 Adyen-9.0.0/Adyen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-30 13:00:28.000000 Adyen-9.0.0/Adyen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:00:28.000000 Adyen-9.0.0/Adyen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-30 13:00:28.000000 Adyen-9.0.0/Adyen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-30 13:00:17.000000 Adyen-9.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-30 13:00:28.789552 Adyen-9.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-06-30 13:00:17.000000 Adyen-9.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-30 13:00:28.789552 Adyen-9.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-30 13:00:17.000000 Adyen-9.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:28.789552 Adyen-9.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/BaseTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/BinLookupTest.py
--rw-r--r--   0 runner    (1001) docker     (123)    32846 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/CheckoutTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/CheckoutUtilityTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/ClientTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/ConfigurationTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/DataProtectionTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/DetermineEndpointTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/LegalEntityManagementTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/ManagementTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/ModificationTest.py
--rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/PaymentTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/RecurringTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/StoredValueTest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/TerminalTest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/ThirdPartyPayoutTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/TransfersTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/UtilTest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:00:17.000000 Adyen-9.0.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:57:05.981922 Adyen-9.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:57:05.965921 Adyen-9.0.1/Adyen/
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23474 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/httpclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:57:05.969922 Adyen-9.0.1/Adyen/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:57:05.969922 Adyen-9.0.1/Adyen/services/balancePlatform/
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/balancePlatform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/balancePlatform/account_holders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/balancePlatform/balance_accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/balancePlatform/bank_account_validation_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/balancePlatform/grant_accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/balancePlatform/grant_offers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/balancePlatform/payment_instrument_groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/balancePlatform/payment_instruments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/balancePlatform/platform_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/balancePlatform/transaction_rules_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/binlookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:57:05.969922 Adyen-9.0.1/Adyen/services/checkout/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/checkout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/checkout/classic_checkout_sdk_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/checkout/modifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/checkout/orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/checkout/payment_links_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/checkout/payments_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/checkout/recurring_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/checkout/utility_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/dataProtection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:57:05.973922 Adyen-9.0.1/Adyen/services/legalEntityManagement/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/legalEntityManagement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/legalEntityManagement/business_lines_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/legalEntityManagement/documents_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/legalEntityManagement/hosted_onboarding_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/legalEntityManagement/legal_entities_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/legalEntityManagement/pci_questionnaires_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/legalEntityManagement/terms_of_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/legalEntityManagement/transfer_instruments_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:57:05.977922 Adyen-9.0.1/Adyen/services/management/
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/account_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/account_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/account_store_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/allowed_origins_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/allowed_origins_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/api_credentials_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/api_credentials_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/api_key_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/api_key_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/client_key_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/client_key_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/my_api_credential_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/payment_methods_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/payout_settings_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/split_configuration_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/terminal_actions_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/terminal_actions_terminal_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/terminal_orders_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/terminal_orders_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/terminal_settings_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/terminal_settings_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/terminal_settings_store_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/terminal_settings_terminal_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/terminals_terminal_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/users_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/users_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/webhooks_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/management/webhooks_merchant_level_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:57:05.977922 Adyen-9.0.1/Adyen/services/payments/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/payments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/payments/general_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/payments/modifications_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:57:05.977922 Adyen-9.0.1/Adyen/services/payouts/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/payouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/payouts/initialization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/payouts/instant_payouts_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/payouts/reviewing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/recurring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/storedValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:57:05.977922 Adyen-9.0.1/Adyen/services/transfers/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/transfers/capital_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/transfers/transactions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/services/transfers/transfers_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-14 12:56:55.000000 Adyen-9.0.1/Adyen/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:57:05.965921 Adyen-9.0.1/Adyen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-14 12:57:05.000000 Adyen-9.0.1/Adyen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-14 12:57:05.000000 Adyen-9.0.1/Adyen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:57:05.000000 Adyen-9.0.1/Adyen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 12:57:05.000000 Adyen-9.0.1/Adyen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-14 12:56:55.000000 Adyen-9.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-14 12:57:05.981922 Adyen-9.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-14 12:56:55.000000 Adyen-9.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-14 12:57:05.981922 Adyen-9.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-14 12:56:55.000000 Adyen-9.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:57:05.981922 Adyen-9.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-14 12:56:55.000000 Adyen-9.0.1/test/BaseTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-14 12:56:55.000000 Adyen-9.0.1/test/BinLookupTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32846 2023-07-14 12:56:55.000000 Adyen-9.0.1/test/CheckoutTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-14 12:56:55.000000 Adyen-9.0.1/test/CheckoutUtilityTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-14 12:56:55.000000 Adyen-9.0.1/test/ClientTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-07-14 12:56:55.000000 Adyen-9.0.1/test/ConfigurationTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-14 12:56:55.000000 Adyen-9.0.1/test/DataProtectionTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-07-14 12:56:55.000000 Adyen-9.0.1/test/DetermineEndpointTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-14 12:56:55.000000 Adyen-9.0.1/test/LegalEntityManagementTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-07-14 12:56:55.000000 Adyen-9.0.1/test/ManagementTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-14 12:56:55.000000 Adyen-9.0.1/test/ModificationTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-07-14 12:56:55.000000 Adyen-9.0.1/test/PaymentTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-07-14 12:56:55.000000 Adyen-9.0.1/test/RecurringTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-07-14 12:56:55.000000 Adyen-9.0.1/test/StoredValueTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-14 12:56:55.000000 Adyen-9.0.1/test/TerminalTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-07-14 12:56:55.000000 Adyen-9.0.1/test/ThirdPartyPayoutTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-14 12:56:55.000000 Adyen-9.0.1/test/TransfersTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-14 12:56:55.000000 Adyen-9.0.1/test/UtilTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:56:55.000000 Adyen-9.0.1/test/__init__.py
```

### Comparing `Adyen-9.0.0/Adyen/__init__.py` & `Adyen-9.0.1/Adyen/__init__.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/client.py` & `Adyen-9.0.1/Adyen/client.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/exceptions.py` & `Adyen-9.0.1/Adyen/exceptions.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/httpclient.py` & `Adyen-9.0.1/Adyen/httpclient.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/__init__.py` & `Adyen-9.0.1/Adyen/services/__init__.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/balancePlatform/__init__.py` & `Adyen-9.0.1/Adyen/services/balancePlatform/__init__.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/balancePlatform/account_holders_api.py` & `Adyen-9.0.1/Adyen/services/balancePlatform/account_holders_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/balancePlatform/balance_accounts_api.py` & `Adyen-9.0.1/Adyen/services/balancePlatform/balance_accounts_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/balancePlatform/bank_account_validation_api.py` & `Adyen-9.0.1/Adyen/services/balancePlatform/bank_account_validation_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/balancePlatform/grant_accounts_api.py` & `Adyen-9.0.1/Adyen/services/balancePlatform/grant_accounts_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/balancePlatform/grant_offers_api.py` & `Adyen-9.0.1/Adyen/services/balancePlatform/grant_offers_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/balancePlatform/payment_instrument_groups_api.py` & `Adyen-9.0.1/Adyen/services/balancePlatform/payment_instrument_groups_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/balancePlatform/payment_instruments_api.py` & `Adyen-9.0.1/Adyen/services/balancePlatform/payment_instruments_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/balancePlatform/platform_api.py` & `Adyen-9.0.1/Adyen/services/balancePlatform/platform_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/balancePlatform/transaction_rules_api.py` & `Adyen-9.0.1/Adyen/services/balancePlatform/transaction_rules_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/base.py` & `Adyen-9.0.1/Adyen/services/base.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/binlookup.py` & `Adyen-9.0.1/Adyen/services/binlookup.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/checkout/__init__.py` & `Adyen-9.0.1/Adyen/services/checkout/__init__.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/checkout/classic_checkout_sdk_api.py` & `Adyen-9.0.1/Adyen/services/checkout/classic_checkout_sdk_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/checkout/modifications_api.py` & `Adyen-9.0.1/Adyen/services/checkout/modifications_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/checkout/orders_api.py` & `Adyen-9.0.1/Adyen/services/checkout/orders_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/checkout/payment_links_api.py` & `Adyen-9.0.1/Adyen/services/checkout/payment_links_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/checkout/payments_api.py` & `Adyen-9.0.1/Adyen/services/terminal.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,54 @@
-from ..base import AdyenServiceBase
+from .base import AdyenServiceBase
 
 
-class PaymentsApi(AdyenServiceBase):
+class AdyenTerminalApi(AdyenServiceBase):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, client=None):
-        super(PaymentsApi, self).__init__(client=client)
-        self.service = "checkout"
+        super(AdyenTerminalApi, self).__init__(client=client)
+        self.service = "terminal"
 
-    def card_details(self, request, idempotency_key=None, **kwargs):
+    def assign_terminals(self, request, idempotency_key=None, **kwargs):
         """
-        Get the list of brands on the card
+        Assign terminals
         """
-        endpoint = f"/cardDetails"
+        endpoint = f"/assignTerminals"
         method = "POST"
         return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
 
-    def donations(self, request, idempotency_key=None, **kwargs):
+    def find_terminal(self, request, idempotency_key=None, **kwargs):
         """
-        Start a transaction for donations
+        Get the account or store of a terminal
         """
-        endpoint = f"/donations"
+        endpoint = f"/findTerminal"
         method = "POST"
         return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
 
-    def payment_methods(self, request, idempotency_key=None, **kwargs):
+    def get_stores_under_account(self, request, idempotency_key=None, **kwargs):
         """
-        Get a list of available payment methods
+        Get the stores of an account
         """
-        endpoint = f"/paymentMethods"
+        endpoint = f"/getStoresUnderAccount"
         method = "POST"
         return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
 
-    def payments(self, request, idempotency_key=None, **kwargs):
+    def get_terminal_details(self, request, idempotency_key=None, **kwargs):
         """
-        Start a transaction
+        Get the details of a terminal
         """
-        endpoint = f"/payments"
+        endpoint = f"/getTerminalDetails"
         method = "POST"
         return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
 
-    def payments_details(self, request, idempotency_key=None, **kwargs):
+    def get_terminals_under_account(self, request, idempotency_key=None, **kwargs):
         """
-        Submit details for a payment
+        Get the list of terminals
         """
-        endpoint = f"/payments/details"
-        method = "POST"
-        return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
-
-    def sessions(self, request, idempotency_key=None, **kwargs):
-        """
-        Create a payment session
-        """
-        endpoint = f"/sessions"
+        endpoint = f"/getTerminalsUnderAccount"
         method = "POST"
         return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
```

### Comparing `Adyen-9.0.0/Adyen/services/checkout/recurring_api.py` & `Adyen-9.0.1/Adyen/services/checkout/recurring_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/checkout/utility_api.py` & `Adyen-9.0.1/Adyen/services/checkout/utility_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/dataProtection.py` & `Adyen-9.0.1/Adyen/services/dataProtection.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/legalEntityManagement/__init__.py` & `Adyen-9.0.1/Adyen/services/legalEntityManagement/__init__.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/legalEntityManagement/business_lines_api.py` & `Adyen-9.0.1/Adyen/services/legalEntityManagement/business_lines_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/legalEntityManagement/documents_api.py` & `Adyen-9.0.1/Adyen/services/legalEntityManagement/documents_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/legalEntityManagement/hosted_onboarding_api.py` & `Adyen-9.0.1/Adyen/services/legalEntityManagement/hosted_onboarding_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/legalEntityManagement/legal_entities_api.py` & `Adyen-9.0.1/Adyen/services/legalEntityManagement/legal_entities_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/legalEntityManagement/pci_questionnaires_api.py` & `Adyen-9.0.1/Adyen/services/legalEntityManagement/pci_questionnaires_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/legalEntityManagement/terms_of_service_api.py` & `Adyen-9.0.1/Adyen/services/legalEntityManagement/terms_of_service_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,22 @@
         """
         Get Terms of Service information for a legal entity
         """
         endpoint = f"/legalEntities/{id}/termsOfServiceAcceptanceInfos"
         method = "GET"
         return self.client.call_adyen_api(None, self.service, method, endpoint, idempotency_key, **kwargs)
 
+    def get_terms_of_service_status(self, id, idempotency_key=None, **kwargs):
+        """
+        Get Terms of Service status
+        """
+        endpoint = f"/legalEntities/{id}/termsOfServiceStatus"
+        method = "GET"
+        return self.client.call_adyen_api(None, self.service, method, endpoint, idempotency_key, **kwargs)
+
     def accept_terms_of_service(self, request, id, termsofservicedocumentid, idempotency_key=None, **kwargs):
         """
         Accept Terms of Service
         """
         endpoint = f"/legalEntities/{id}/termsOfService/{termsofservicedocumentid}"
         method = "PATCH"
         return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
```

### Comparing `Adyen-9.0.0/Adyen/services/legalEntityManagement/transfer_instruments_api.py` & `Adyen-9.0.1/Adyen/services/legalEntityManagement/transfer_instruments_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/__init__.py` & `Adyen-9.0.1/Adyen/services/management/__init__.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/account_company_level_api.py` & `Adyen-9.0.1/Adyen/services/management/account_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/account_merchant_level_api.py` & `Adyen-9.0.1/Adyen/services/management/account_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/account_store_level_api.py` & `Adyen-9.0.1/Adyen/services/management/account_store_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/allowed_origins_company_level_api.py` & `Adyen-9.0.1/Adyen/services/management/allowed_origins_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/allowed_origins_merchant_level_api.py` & `Adyen-9.0.1/Adyen/services/management/allowed_origins_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/api_credentials_company_level_api.py` & `Adyen-9.0.1/Adyen/services/management/api_credentials_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/api_credentials_merchant_level_api.py` & `Adyen-9.0.1/Adyen/services/management/api_credentials_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/api_key_company_level_api.py` & `Adyen-9.0.1/Adyen/services/management/api_key_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/api_key_merchant_level_api.py` & `Adyen-9.0.1/Adyen/services/management/api_key_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/client_key_company_level_api.py` & `Adyen-9.0.1/Adyen/services/management/client_key_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/client_key_merchant_level_api.py` & `Adyen-9.0.1/Adyen/services/management/client_key_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/my_api_credential_api.py` & `Adyen-9.0.1/Adyen/services/management/my_api_credential_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/payment_methods_merchant_level_api.py` & `Adyen-9.0.1/Adyen/services/management/payment_methods_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/payout_settings_merchant_level_api.py` & `Adyen-9.0.1/Adyen/services/management/payout_settings_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/split_configuration_merchant_level_api.py` & `Adyen-9.0.1/Adyen/services/management/split_configuration_merchant_level_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,19 @@
         """
         Delete a split configuration
         """
         endpoint = f"/merchants/{merchantId}/splitConfigurations/{splitConfigurationId}"
         method = "DELETE"
         return self.client.call_adyen_api(None, self.service, method, endpoint, idempotency_key, **kwargs)
 
-    def delete_split_configuration_rule(self, merchantId, splitConfigurationId, splitConfigurationRuleId, idempotency_key=None, **kwargs):
+    def delete_split_configuration_rule(self, merchantId, splitConfigurationId, ruleId, idempotency_key=None, **kwargs):
         """
         Delete a split configuration rule
         """
-        endpoint = f"/merchants/{merchantId}/splitConfigurations/{splitConfigurationId}/rules/{splitConfigurationRuleId}"
+        endpoint = f"/merchants/{merchantId}/splitConfigurations/{splitConfigurationId}/rules/{ruleId}"
         method = "DELETE"
         return self.client.call_adyen_api(None, self.service, method, endpoint, idempotency_key, **kwargs)
 
     def list_split_configurations(self, merchantId, idempotency_key=None, **kwargs):
         """
         Get a list of split configurations
         """
```

### Comparing `Adyen-9.0.0/Adyen/services/management/terminal_actions_company_level_api.py` & `Adyen-9.0.1/Adyen/services/management/terminal_actions_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/terminal_actions_terminal_level_api.py` & `Adyen-9.0.1/Adyen/services/management/terminal_actions_terminal_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/terminal_orders_company_level_api.py` & `Adyen-9.0.1/Adyen/services/management/terminal_orders_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/terminal_orders_merchant_level_api.py` & `Adyen-9.0.1/Adyen/services/management/terminal_orders_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/terminal_settings_company_level_api.py` & `Adyen-9.0.1/Adyen/services/management/terminal_settings_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/terminal_settings_merchant_level_api.py` & `Adyen-9.0.1/Adyen/services/management/terminal_settings_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/terminal_settings_store_level_api.py` & `Adyen-9.0.1/Adyen/services/management/terminal_settings_store_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/terminal_settings_terminal_level_api.py` & `Adyen-9.0.1/Adyen/services/management/terminal_settings_terminal_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/terminals_terminal_level_api.py` & `Adyen-9.0.1/Adyen/services/management/terminals_terminal_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/users_company_level_api.py` & `Adyen-9.0.1/Adyen/services/management/users_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/users_merchant_level_api.py` & `Adyen-9.0.1/Adyen/services/management/users_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/webhooks_company_level_api.py` & `Adyen-9.0.1/Adyen/services/management/webhooks_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/management/webhooks_merchant_level_api.py` & `Adyen-9.0.1/Adyen/services/management/webhooks_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/payments/__init__.py` & `Adyen-9.0.1/Adyen/services/payments/__init__.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/payments/general_api.py` & `Adyen-9.0.1/Adyen/services/payments/general_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/payments/modifications_api.py` & `Adyen-9.0.1/Adyen/services/payments/modifications_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/payouts/__init__.py` & `Adyen-9.0.1/Adyen/services/payouts/__init__.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/payouts/initialization_api.py` & `Adyen-9.0.1/Adyen/services/payouts/initialization_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/payouts/instant_payouts_api.py` & `Adyen-9.0.1/Adyen/services/payouts/instant_payouts_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/payouts/reviewing_api.py` & `Adyen-9.0.1/Adyen/services/payouts/reviewing_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/recurring.py` & `Adyen-9.0.1/Adyen/services/recurring.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/storedValue.py` & `Adyen-9.0.1/Adyen/services/storedValue.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/terminal.py` & `Adyen-9.0.1/Adyen/services/checkout/payments_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,70 @@
-from .base import AdyenServiceBase
+from ..base import AdyenServiceBase
 
 
-class AdyenTerminalApi(AdyenServiceBase):
+class PaymentsApi(AdyenServiceBase):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, client=None):
-        super(AdyenTerminalApi, self).__init__(client=client)
-        self.service = "terminal"
+        super(PaymentsApi, self).__init__(client=client)
+        self.service = "checkout"
 
-    def assign_terminals(self, request, idempotency_key=None, **kwargs):
+    def get_synchronous_result_of_payment_session(self, sessionId, idempotency_key=None, **kwargs):
         """
-        Assign terminals
+        Get a synchronous result of a payment session
         """
-        endpoint = f"/assignTerminals"
+        endpoint = f"/sessions/{sessionId}"
+        method = "GET"
+        return self.client.call_adyen_api(None, self.service, method, endpoint, idempotency_key, **kwargs)
+
+    def card_details(self, request, idempotency_key=None, **kwargs):
+        """
+        Get the list of brands on the card
+        """
+        endpoint = f"/cardDetails"
+        method = "POST"
+        return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
+
+    def donations(self, request, idempotency_key=None, **kwargs):
+        """
+        Start a transaction for donations
+        """
+        endpoint = f"/donations"
         method = "POST"
         return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
 
-    def find_terminal(self, request, idempotency_key=None, **kwargs):
+    def payment_methods(self, request, idempotency_key=None, **kwargs):
         """
-        Get the account or store of a terminal
+        Get a list of available payment methods
         """
-        endpoint = f"/findTerminal"
+        endpoint = f"/paymentMethods"
         method = "POST"
         return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
 
-    def get_stores_under_account(self, request, idempotency_key=None, **kwargs):
+    def payments(self, request, idempotency_key=None, **kwargs):
         """
-        Get the stores of an account
+        Start a transaction
         """
-        endpoint = f"/getStoresUnderAccount"
+        endpoint = f"/payments"
         method = "POST"
         return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
 
-    def get_terminal_details(self, request, idempotency_key=None, **kwargs):
+    def payments_details(self, request, idempotency_key=None, **kwargs):
         """
-        Get the details of a terminal
+        Submit details for a payment
         """
-        endpoint = f"/getTerminalDetails"
+        endpoint = f"/payments/details"
         method = "POST"
         return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
 
-    def get_terminals_under_account(self, request, idempotency_key=None, **kwargs):
+    def sessions(self, request, idempotency_key=None, **kwargs):
         """
-        Get the list of terminals
+        Create a payment session
         """
-        endpoint = f"/getTerminalsUnderAccount"
+        endpoint = f"/sessions"
         method = "POST"
         return self.client.call_adyen_api(request, self.service, method, endpoint, idempotency_key, **kwargs)
```

### Comparing `Adyen-9.0.0/Adyen/services/transfers/__init__.py` & `Adyen-9.0.1/Adyen/services/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/transfers/capital_api.py` & `Adyen-9.0.1/Adyen/services/transfers/capital_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/transfers/transactions_api.py` & `Adyen-9.0.1/Adyen/services/transfers/transactions_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/services/transfers/transfers_api.py` & `Adyen-9.0.1/Adyen/services/transfers/transfers_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen/settings.py` & `Adyen-9.0.1/Adyen/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 API_PAYMENT_VERSION = "v68"
 API_PAYOUT_VERSION = "v68"
 API_TERMINAL_VERSION = "v1"
 API_TRANSFERS_VERSION = "v3"
 API_LEGAL_ENTITY_MANAGEMENT_VERSION = "v3"
 API_STORED_VALUE_VERSION = "v46"
 LIB_NAME = "adyen-python-api-library"
-LIB_VERSION = "9.0.0"
+LIB_VERSION = "9.0.1"
```

### Comparing `Adyen-9.0.0/Adyen/util.py` & `Adyen-9.0.1/Adyen/util.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/Adyen.egg-info/PKG-INFO` & `Adyen-9.0.1/Adyen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Adyen
-Version: 9.0.0
+Version: 9.0.1
 Summary: Adyen Python Api
 Home-page: https://github.com/Adyen/adyen-python-api-library
 Author: Adyen
 Author-email: support@adyen.com
 Maintainer: Adyen
 Maintainer-email: support@adyen.com
 Keywords: payments,adyen,fintech
```

### Comparing `Adyen-9.0.0/Adyen.egg-info/SOURCES.txt` & `Adyen-9.0.1/Adyen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/LICENSE.md` & `Adyen-9.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/PKG-INFO` & `Adyen-9.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Adyen
-Version: 9.0.0
+Version: 9.0.1
 Summary: Adyen Python Api
 Home-page: https://github.com/Adyen/adyen-python-api-library
 Author: Adyen
 Author-email: support@adyen.com
 Maintainer: Adyen
 Maintainer-email: support@adyen.com
 Keywords: payments,adyen,fintech
```

### Comparing `Adyen-9.0.0/README.md` & `Adyen-9.0.1/README.md`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/setup.py` & `Adyen-9.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Adyen',
     packages=find_packages(include="Adyen*"),
-    version='9.0.0',
+    version='9.0.1',
     maintainer='Adyen',
     maintainer_email='support@adyen.com',
     description='Adyen Python Api',
     long_description="A Python client library for accessing Adyen APIs",
     author='Adyen',
     author_email='support@adyen.com',
     url='https://github.com/Adyen/adyen-python-api-library',
```

### Comparing `Adyen-9.0.0/test/BaseTest.py` & `Adyen-9.0.1/test/BaseTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/test/BinLookupTest.py` & `Adyen-9.0.1/test/BinLookupTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/test/CheckoutTest.py` & `Adyen-9.0.1/test/CheckoutTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/test/CheckoutUtilityTest.py` & `Adyen-9.0.1/test/CheckoutUtilityTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/test/ConfigurationTest.py` & `Adyen-9.0.1/test/ConfigurationTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/test/DataProtectionTest.py` & `Adyen-9.0.1/test/DataProtectionTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/test/DetermineEndpointTest.py` & `Adyen-9.0.1/test/DetermineEndpointTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/test/LegalEntityManagementTest.py` & `Adyen-9.0.1/test/LegalEntityManagementTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/test/ManagementTest.py` & `Adyen-9.0.1/test/ManagementTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/test/ModificationTest.py` & `Adyen-9.0.1/test/ModificationTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/test/PaymentTest.py` & `Adyen-9.0.1/test/PaymentTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/test/RecurringTest.py` & `Adyen-9.0.1/test/RecurringTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/test/StoredValueTest.py` & `Adyen-9.0.1/test/StoredValueTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/test/TerminalTest.py` & `Adyen-9.0.1/test/TerminalTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/test/ThirdPartyPayoutTest.py` & `Adyen-9.0.1/test/ThirdPartyPayoutTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/test/TransfersTest.py` & `Adyen-9.0.1/test/TransfersTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.0/test/UtilTest.py` & `Adyen-9.0.1/test/UtilTest.py`

 * *Files identical despite different names*

