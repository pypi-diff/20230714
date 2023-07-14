# Comparing `tmp/connect_cli-27.6.tar.gz` & `tmp/connect_cli-27.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connect_cli-27.6.tar", max compression
+gzip compressed data, was "connect_cli-27.7.tar", max compression
```

## Comparing `connect_cli-27.6.tar` & `connect_cli-27.7.tar`

### file list

```diff
@@ -1,287 +1,287 @@
--rw-r--r--   0        0        0    11357 2023-06-01 06:48:44.750235 connect_cli-27.6/LICENSE
--rw-r--r--   0        0        0     3280 2023-06-01 06:48:44.750235 connect_cli-27.6/README.md
--rw-r--r--   0        0        0     1823 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/.github/workflows/build.yml
--rw-r--r--   0        0        0      166 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/.gitignore
--rw-r--r--   0        0        0    10756 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/LICENSE
--rw-r--r--   0        0        0      708 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/README.md
--rw-r--r--   0        0        0   122573 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/poetry.lock
--rw-r--r--   0        0        0     1221 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/reports/__init__.py
--rw-r--r--   0        0        0      215 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/reports/billing_requests/Readme.md
--rw-r--r--   0        0        0        0 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/reports/billing_requests/__init__.py
--rw-r--r--   0        0        0     3762 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/reports/billing_requests/entrypoint.py
--rw-r--r--   0        0        0     9038 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/reports/billing_requests/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      377 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/reports/billing_requests_line_item/Readme.md
--rw-r--r--   0        0        0        0 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/reports/billing_requests_line_item/__init__.py
--rw-r--r--   0        0        0     4313 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/reports/billing_requests_line_item/entrypoint.py
--rw-r--r--   0        0        0     9214 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/reports/billing_requests_line_item/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      151 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/reports/contract_list/Readme.md
--rw-r--r--   0        0        0        0 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/reports/contract_list/__init__.py
--rw-r--r--   0        0        0     3114 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/reports/contract_list/entrypoint.py
--rw-r--r--   0        0        0     8883 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/reports/contract_list/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      175 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/reports/customers_list/Readme.md
--rw-r--r--   0        0        0        0 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/customers_list/__init__.py
--rw-r--r--   0        0        0     3595 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/customers_list/entrypoint.py
--rw-r--r--   0        0        0     8914 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/customers_list/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      546 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/executive_fullfilment_requests/Readme.md
--rw-r--r--   0        0        0        0 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/executive_fullfilment_requests/__init__.py
--rw-r--r--   0        0        0     6376 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/executive_fullfilment_requests/constants.py
--rw-r--r--   0        0        0    17465 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/executive_fullfilment_requests/entrypoint.py
--rw-r--r--   0        0        0     5254 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/img/ClouBlue-Logo.png
--rw-r--r--   0        0        0     3180 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.css
--rw-r--r--   0        0        0     1280 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.html.j2
--rw-r--r--   0        0        0      240 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/fulfillment_requests/Readme.md
--rw-r--r--   0        0        0        0 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/fulfillment_requests/__init__.py
--rw-r--r--   0        0        0     4584 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/fulfillment_requests/entrypoint.py
--rw-r--r--   0        0        0     9160 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/fulfillment_requests/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      301 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/fulfillment_requests_failed/Readme.md
--rw-r--r--   0        0        0        0 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/fulfillment_requests_failed/__init__.py
--rw-r--r--   0        0        0     4064 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/fulfillment_requests_failed/entrypoint.py
--rw-r--r--   0        0        0     9050 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/fulfillment_requests_failed/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      328 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/fulfillment_requests_line_item/Readme.md
--rw-r--r--   0        0        0        0 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/fulfillment_requests_line_item/__init__.py
--rw-r--r--   0        0        0     4982 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/fulfillment_requests_line_item/entrypoint.py
--rw-r--r--   0        0        0     9234 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/fulfillment_requests_line_item/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      180 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/helpdesk/Readme.md
--rw-r--r--   0        0        0        0 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/helpdesk/__init__.py
--rw-r--r--   0        0        0     2635 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/helpdesk/entrypoint.py
--rw-r--r--   0        0        0     8749 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/helpdesk/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      186 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/listing_list/Readme.md
--rw-r--r--   0        0        0        0 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/listing_list/__init__.py
--rw-r--r--   0        0        0     2632 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/listing_list/entrypoint.py
--rw-r--r--   0        0        0     8703 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/listing_list/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      194 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/listing_requests/Readme.md
--rw-r--r--   0        0        0        0 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/listing_requests/__init__.py
--rw-r--r--   0        0        0     2870 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/listing_requests/entrypoint.py
--rw-r--r--   0        0        0     8746 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/listing_requests/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      117 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/Readme.md
--rw-r--r--   0        0        0        0 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/__init__.py
--rw-r--r--   0        0        0     2582 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/entrypoint.py
--rwxr-xr-x   0        0        0     7209 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-connect-alone.png
--rw-r--r--   0        0        0    33448 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-logo.png
--rw-r--r--   0        0        0    11287 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-disabled.png
--rw-r--r--   0        0        0     9404 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-enabled.png
--rw-r--r--   0        0        0    91722 2023-06-01 06:51:33.234492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/connect-logo.png
--rw-r--r--   0        0        0   465078 2023-06-01 06:51:33.238492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cover-bg.png
--rw-r--r--   0        0        0    10941 2023-06-01 06:51:33.238492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/imc-small-color.png
--rw-r--r--   0        0        0    16685 2023-06-01 06:51:33.238492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-Black.png
--rw-r--r--   0        0        0     3555 2023-06-01 06:51:33.238492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-White.png
--rw-r--r--   0        0        0     5254 2023-06-01 06:51:33.238492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo.png
--rw-r--r--   0        0        0     8250 2023-06-01 06:51:33.238492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/accordo.png
--rw-r--r--   0        0        0     1311 2023-06-01 06:51:33.238492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-blue.png
--rw-r--r--   0        0        0     1968 2023-06-01 06:51:33.238492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-white.png
--rw-r--r--   0        0        0   124929 2023-06-01 06:51:33.238492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/adobe.jpeg
--rw-r--r--   0        0        0    10421 2023-06-01 06:51:33.238492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/airtame.png
--rw-r--r--   0        0        0      876 2023-06-01 06:51:33.238492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/allyhub.png
--rw-r--r--   0        0        0     4615 2023-06-01 06:51:33.238492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/alsid.png
--rw-r--r--   0        0        0    12369 2023-06-01 06:51:33.238492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/anchor.png
--rw-r--r--   0        0        0     5200 2023-06-01 06:51:33.238492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/australia.png
--rw-r--r--   0        0        0     3371 2023-06-01 06:51:33.238492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/austria.png
--rw-r--r--   0        0        0    60306 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/aws.png
--rw-r--r--   0        0        0     3030 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/belgium.png
--rw-r--r--   0        0        0     5606 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/brazil.png
--rw-r--r--   0        0        0     3693 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/canada.png
--rw-r--r--   0        0        0     3870 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/chile.png
--rw-r--r--   0        0        0     3086 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/colombia.png
--rw-r--r--   0        0        0     3670 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/france.png
--rw-r--r--   0        0        0     3212 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/germany.png
--rw-r--r--   0        0        0     4521 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/hong-kong.png
--rw-r--r--   0        0        0    12000 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/icon.png
--rw-r--r--   0        0        0     4491 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/india.png
--rw-r--r--   0        0        0     3622 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/italy.png
--rw-r--r--   0        0        0     5096 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/malaysia.png
--rw-r--r--   0        0        0     3897 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/mexico.png
--rw-r--r--   0        0        0     3633 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/netherlands.png
--rw-r--r--   0        0        0     5173 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/new-zealand.png
--rw-r--r--   0        0        0     4163 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/singapore.png
--rw-r--r--   0        0        0     4670 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/spain.png
--rw-r--r--   0        0        0     4802 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/sweden.png
--rw-r--r--   0        0        0     3622 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/switzerland.png
--rw-r--r--   0        0        0     4073 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/turkey.png
--rw-r--r--   0        0        0     3350 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uae.png
--rw-r--r--   0        0        0     5583 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uk.png
--rw-r--r--   0        0        0     4892 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/usa.png
--rw-r--r--   0        0        0     4063 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.css
--rw-r--r--   0        0        0     1736 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.html.j2
--rw-r--r--   0        0        0      592 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/sla/Readme.md
--rw-r--r--   0        0        0        0 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/sla/__init__.py
--rw-r--r--   0        0        0     4125 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/sla/entrypoint.py
--rw-r--r--   0        0        0     9679 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/sla/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      260 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/subscription_list/Readme.md
--rw-r--r--   0        0        0        0 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/subscription_list/__init__.py
--rw-r--r--   0        0        0     6276 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/subscription_list/entrypoint.py
--rw-r--r--   0        0        0     9302 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/subscription_list/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      203 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/tier_configuration_list/Readme.md
--rw-r--r--   0        0        0        0 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/tier_configuration_list/__init__.py
--rw-r--r--   0        0        0     4282 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/tier_configuration_list/entrypoint.py
--rw-r--r--   0        0        0     8925 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/tier_configuration_list/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      228 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/tier_configuration_requests/Readme.md
--rw-r--r--   0        0        0        0 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/tier_configuration_requests/__init__.py
--rw-r--r--   0        0        0     5147 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/tier_configuration_requests/entrypoint.py
--rw-r--r--   0        0        0     9070 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/tier_configuration_requests/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0      431 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/usage_in_subscription/Readme.md
--rw-r--r--   0        0        0        0 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/usage_in_subscription/__init__.py
--rw-r--r--   0        0        0     4106 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/usage_in_subscription/entrypoint.py
--rw-r--r--   0        0        0     9137 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/usage_in_subscription/templates/xlsx/template.xlsx
--rw-r--r--   0        0        0     1318 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/reports/utils.py
--rw-r--r--   0        0        0    37904 2023-06-01 06:51:33.230492 connect_cli-27.6/connect/.data/connect_reports/reports.json
--rw-r--r--   0        0        0      245 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/sonar-project.properties
--rw-r--r--   0        0        0      321 2023-06-01 06:51:33.242492 connect_cli-27.6/connect/.data/connect_reports/tox.ini
--rw-r--r--   0        0        0      352 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/__init__.py
--rw-r--r--   0        0        0     1761 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/ccli.py
--rw-r--r--   0        0        0       54 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/core/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/core/account/__init__.py
--rw-r--r--   0        0        0     2433 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/core/account/commands.py
--rw-r--r--   0        0        0     1233 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/core/account/helpers.py
--rw-r--r--   0        0        0     2781 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/core/base.py
--rw-r--r--   0        0        0     4049 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/core/config.py
--rw-r--r--   0        0        0      573 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/core/constants.py
--rw-r--r--   0        0        0     1424 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/core/http.py
--rw-r--r--   0        0        0      838 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/core/plugins.py
--rw-r--r--   0        0        0     6809 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/core/terminal.py
--rw-r--r--   0        0        0     3167 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/core/utils.py
--rw-r--r--   0        0        0        0 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/plugins/customer/__init__.py
--rw-r--r--   0        0        0     2138 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/plugins/customer/commands.py
--rw-r--r--   0        0        0      526 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/plugins/customer/constants.py
--rw-r--r--   0        0        0     5923 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/plugins/customer/export.py
--rw-r--r--   0        0        0    12428 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/plugins/customer/sync.py
--rw-r--r--   0        0        0        0 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/plugins/locale/__init__.py
--rw-r--r--   0        0        0     1363 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/plugins/locale/commands.py
--rw-r--r--   0        0        0      306 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/plugins/play/__init__.py
--rw-r--r--   0        0        0     2486 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/plugins/play/commands.py
--rw-r--r--   0        0        0     2395 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/plugins/play/context.py
--rw-r--r--   0        0        0      428 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/plugins/play/save.py
--rw-r--r--   0        0        0     1501 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/plugins/play/script.py
--rw-r--r--   0        0        0        0 2023-06-01 06:48:44.750235 connect_cli-27.6/connect/cli/plugins/product/__init__.py
--rw-r--r--   0        0        0     1675 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/product/api.py
--rw-r--r--   0        0        0     8632 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/product/clone.py
--rw-r--r--   0        0        0     9677 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/product/commands.py
--rw-r--r--   0        0        0     1289 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/product/constants.py
--rw-r--r--   0        0        0    33297 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/product/export.py
--rw-r--r--   0        0        0      846 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/product/sync/__init__.py
--rw-r--r--   0        0        0     5912 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/product/sync/actions.py
--rw-r--r--   0        0        0    10140 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/product/sync/capabilities.py
--rw-r--r--   0        0        0     3881 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/product/sync/configuration_values.py
--rw-r--r--   0        0        0     5129 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/product/sync/general.py
--rw-r--r--   0        0        0    11506 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/product/sync/items.py
--rw-r--r--   0        0        0     5740 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/product/sync/media.py
--rw-r--r--   0        0        0     9351 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/product/sync/params.py
--rw-r--r--   0        0        0     3598 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/product/sync/static_resources.py
--rw-r--r--   0        0        0     5260 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/product/sync/templates.py
--rw-r--r--   0        0        0      961 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/product/utils.py
--rw-r--r--   0        0        0        0 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/__init__.py
--rw-r--r--   0        0        0     5328 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/commands.py
--rw-r--r--   0        0        0        0 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/__init__.py
--rw-r--r--   0        0        0      411 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/constants.py
--rw-r--r--   0        0        0    10313 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/helpers.py
--rw-r--r--   0        0        0      103 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/__init__.py.j2
--rw-r--r--   0        0        0      852 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/anvil.py.j2
--rw-r--r--   0        0        0     2920 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/events.py.j2
--rw-r--r--   0        0        0      464 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/extension.json.j2
--rw-r--r--   0        0        0      560 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/schemas.py.j2
--rw-r--r--   0        0        0        0 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/static/.gitkeep.j2
--rw-r--r--   0        0        0     1762 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/tfnapp.py.j2
--rw-r--r--   0        0        0     7295 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/webapp.py.j2
--rw-r--r--   0        0        0      702 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.${project_slug}_dev.env.j2
--rw-r--r--   0        0        0     1083 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.eslintrc.yaml.j2
--rw-r--r--   0        0        0      231 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.flake8.j2
--rw-r--r--   0        0        0     1309 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.github/workflows/test.yml.j2
--rw-r--r--   0        0        0       96 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.gitignore.j2
--rw-r--r--   0        0        0       63 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/CHANGELOG.md.j2
--rw-r--r--   0        0        0      314 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/Dockerfile.j2
--rw-r--r--   0        0        0     1661 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/HOWTO.md.j2
--rw-r--r--   0        0        0    14063 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/LICENSE.j2
--rw-r--r--   0        0        0      195 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/README.md.j2
--rw-r--r--   0        0        0      111 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/__mocks__/fileMock.js.j2
--rw-r--r--   0        0        0       97 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/__mocks__/styleMock.js.j2
--rw-r--r--   0        0        0       39 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/babel.config.json.j2
--rw-r--r--   0        0        0     1162 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/docker-compose.yml.j2
--rw-r--r--   0        0        0      944 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/jest.config.js.j2
--rw-r--r--   0        0        0     1246 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/package.json.j2
--rw-r--r--   0        0        0       29 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/poetry.toml.j2
--rw-r--r--   0        0        0     1960 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/pyproject.toml.j2
--rw-r--r--   0        0        0      103 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/__init__.py.j2
--rw-r--r--   0        0        0      559 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/conftest.py.j2
--rw-r--r--   0        0        0      553 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_anvil.py.j2
--rw-r--r--   0        0        0     2602 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_events.py.j2
--rw-r--r--   0        0        0     1183 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_tfnapp.py.j2
--rw-r--r--   0        0        0     8794 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_webapp.py.j2
--rw-r--r--   0        0        0      947 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/images/mkp.svg.j2
--rw-r--r--   0        0        0      729 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/index.html.j2
--rw-r--r--   0        0        0      928 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/settings.html.j2
--rw-r--r--   0        0        0      470 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/transformations/copy.html.j2
--rw-r--r--   0        0        0     1590 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/transformations/manual.html.j2
--rw-r--r--   0        0        0     2609 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/components.js.j2
--rw-r--r--   0        0        0      323 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/index.js.j2
--rw-r--r--   0        0        0      320 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/settings.js.j2
--rw-r--r--   0        0        0      267 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/transformations/copy.js.j2
--rw-r--r--   0        0        0      308 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/transformations/manual.js.j2
--rw-r--r--   0        0        0    10273 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages.js.j2
--rw-r--r--   0        0        0     1579 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/utils.js.j2
--rw-r--r--   0        0        0     6381 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/index.css.j2
--rw-r--r--   0        0        0      693 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/manual.css.j2
--rw-r--r--   0        0        0     6508 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/components.spec.js.j2
--rw-r--r--   0        0        0     9181 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/pages.spec.js.j2
--rw-r--r--   0        0        0     4352 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/utils.spec.js.j2
--rw-r--r--   0        0        0     2512 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/webpack.config.js.j2
--rw-r--r--   0        0        0     4496 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/utils.py
--rw-r--r--   0        0        0      920 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/validators.py
--rw-r--r--   0        0        0    12120 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/extension/wizard.py
--rw-r--r--   0        0        0     5792 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/renderer.py
--rw-r--r--   0        0        0        0 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/report/__init__.py
--rw-r--r--   0        0        0     8611 2023-06-01 06:48:44.754235 connect_cli-27.6/connect/cli/plugins/project/report/helpers.py
--rw-r--r--   0        0        0       73 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/README.md.j2
--rw-r--r--   0        0        0        0 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/__init__.py.j2
--rw-r--r--   0        0        0     1507 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/entrypoint.py.j2
--rw-r--r--   0        0        0        0 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/templates/pdf/template.css.j2
--rw-r--r--   0        0        0      499 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/templates/pdf/template.html.j2.j2
--rw-r--r--   0        0        0      150 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/templates/xml/template.xml.j2.j2
--rw-r--r--   0        0        0       69 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/README.md.j2
--rw-r--r--   0        0        0        0 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/__init__.py.j2
--rw-r--r--   0        0        0     1507 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/entrypoint.py.j2
--rw-r--r--   0        0        0        0 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/pdf/template.css.j2
--rw-r--r--   0        0        0      518 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/pdf/template.html.j2.j2
--rw-r--r--   0        0        0      150 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/xml/template.xml.j2.j2
--rw-r--r--   0        0        0      271 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.flake8.j2
--rw-r--r--   0        0        0      803 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.github/workflows/build.yml.j2
--rw-r--r--   0        0        0       37 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.gitignore.j2
--rw-r--r--   0        0        0      458 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/HOWTO.md.j2
--rw-r--r--   0        0        0    14063 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/LICENSE.j2
--rw-r--r--   0        0        0      138 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/README.md.j2
--rw-r--r--   0        0        0       29 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/poetry.toml.j2
--rw-r--r--   0        0        0     1352 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/pyproject.toml.j2
--rw-r--r--   0        0        0     2589 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/reports.json.j2
--rw-r--r--   0        0        0      103 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/__init__.py.j2
--rw-r--r--   0        0        0     6397 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/conftest.py.j2
--rw-r--r--   0        0        0     2534 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/test_${project_slug}.py.j2
--rw-r--r--   0        0        0     5878 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/validations.py
--rw-r--r--   0        0        0     8603 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/report/wizard.py
--rw-r--r--   0        0        0     1403 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/utils.py
--rw-r--r--   0        0        0     2798 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/project/validators.py
--rw-r--r--   0        0        0        0 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/report/__init__.py
--rw-r--r--   0        0        0     2405 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/report/commands.py
--rw-r--r--   0        0        0       86 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/report/constants.py
--rw-r--r--   0        0        0     6210 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/report/helpers.py
--rw-r--r--   0        0        0     2812 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/report/utils.py
--rw-r--r--   0        0        0     8418 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/report/wizard.py
--rw-r--r--   0        0        0        0 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/shared/__init__.py
--rw-r--r--   0        0        0     2442 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/shared/base.py
--rw-r--r--   0        0        0     1973 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/shared/constants.py
--rw-r--r--   0        0        0       46 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/shared/exceptions.py
--rw-r--r--   0        0        0     2304 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/shared/export.py
--rw-r--r--   0        0        0     6248 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/shared/sync_stats.py
--rw-r--r--   0        0        0     5666 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/shared/translation_attr_sync.py
--rw-r--r--   0        0        0     6390 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/shared/translation_sync.py
--rw-r--r--   0        0        0     1996 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/shared/translations_synchronizers.py
--rw-r--r--   0        0        0     6794 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/shared/utils.py
--rw-r--r--   0        0        0        0 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/translation/__init__.py
--rw-r--r--   0        0        0      707 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/translation/activate.py
--rw-r--r--   0        0        0     6869 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/translation/commands.py
--rw-r--r--   0        0        0      795 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/translation/constants.py
--rw-r--r--   0        0        0     1216 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/translation/export.py
--rw-r--r--   0        0        0      950 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/translation/primarize.py
--rw-r--r--   0        0        0     8876 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/translation/translation_sync.py
--rw-r--r--   0        0        0      832 2023-06-01 06:48:44.758235 connect_cli-27.6/connect/cli/plugins/translation/utils.py
--rw-r--r--   0        0        0     3955 2023-06-01 06:51:33.954493 connect_cli-27.6/pyproject.toml
--rw-r--r--   0        0        0     5025 1970-01-01 00:00:00.000000 connect_cli-27.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-14 17:47:46.142966 connect_cli-27.7/LICENSE
+-rw-r--r--   0        0        0     3280 2023-07-14 17:47:46.142966 connect_cli-27.7/README.md
+-rw-r--r--   0        0        0     1823 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/.github/workflows/build.yml
+-rw-r--r--   0        0        0      166 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/.gitignore
+-rw-r--r--   0        0        0    10756 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/LICENSE
+-rw-r--r--   0        0        0      708 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/README.md
+-rw-r--r--   0        0        0   122573 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/poetry.lock
+-rw-r--r--   0        0        0     1221 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/__init__.py
+-rw-r--r--   0        0        0      215 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests/__init__.py
+-rw-r--r--   0        0        0     3762 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests/entrypoint.py
+-rw-r--r--   0        0        0     9038 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      377 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests_line_item/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests_line_item/__init__.py
+-rw-r--r--   0        0        0     4313 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests_line_item/entrypoint.py
+-rw-r--r--   0        0        0     9214 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests_line_item/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      151 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/contract_list/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/contract_list/__init__.py
+-rw-r--r--   0        0        0     3114 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/contract_list/entrypoint.py
+-rw-r--r--   0        0        0     8883 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/contract_list/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      175 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/customers_list/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/customers_list/__init__.py
+-rw-r--r--   0        0        0     3595 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/customers_list/entrypoint.py
+-rw-r--r--   0        0        0     8914 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/customers_list/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      546 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/__init__.py
+-rw-r--r--   0        0        0     6376 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/constants.py
+-rw-r--r--   0        0        0    17465 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/entrypoint.py
+-rw-r--r--   0        0        0     5254 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/img/ClouBlue-Logo.png
+-rw-r--r--   0        0        0     3180 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.css
+-rw-r--r--   0        0        0     1280 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.html.j2
+-rw-r--r--   0        0        0      240 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests/__init__.py
+-rw-r--r--   0        0        0     4584 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests/entrypoint.py
+-rw-r--r--   0        0        0     9160 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      301 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_failed/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_failed/__init__.py
+-rw-r--r--   0        0        0     4064 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_failed/entrypoint.py
+-rw-r--r--   0        0        0     9050 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_failed/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      328 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_line_item/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_line_item/__init__.py
+-rw-r--r--   0        0        0     4982 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_line_item/entrypoint.py
+-rw-r--r--   0        0        0     9234 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_line_item/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      180 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/helpdesk/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/helpdesk/__init__.py
+-rw-r--r--   0        0        0     2635 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/helpdesk/entrypoint.py
+-rw-r--r--   0        0        0     8749 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/helpdesk/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      186 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/listing_list/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/listing_list/__init__.py
+-rw-r--r--   0        0        0     2632 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/listing_list/entrypoint.py
+-rw-r--r--   0        0        0     8703 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/listing_list/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      194 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/listing_requests/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/listing_requests/__init__.py
+-rw-r--r--   0        0        0     2870 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/listing_requests/entrypoint.py
+-rw-r--r--   0        0        0     8746 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/listing_requests/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      117 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/__init__.py
+-rw-r--r--   0        0        0     2582 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/entrypoint.py
+-rwxr-xr-x   0        0        0     7209 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-connect-alone.png
+-rw-r--r--   0        0        0    33448 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-logo.png
+-rw-r--r--   0        0        0    11287 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-disabled.png
+-rw-r--r--   0        0        0     9404 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-enabled.png
+-rw-r--r--   0        0        0    91722 2023-07-14 17:51:00.193973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/connect-logo.png
+-rw-r--r--   0        0        0   465078 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cover-bg.png
+-rw-r--r--   0        0        0    10941 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/imc-small-color.png
+-rw-r--r--   0        0        0    16685 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-Black.png
+-rw-r--r--   0        0        0     3555 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-White.png
+-rw-r--r--   0        0        0     5254 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo.png
+-rw-r--r--   0        0        0     8250 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/accordo.png
+-rw-r--r--   0        0        0     1311 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-blue.png
+-rw-r--r--   0        0        0     1968 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-white.png
+-rw-r--r--   0        0        0   124929 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/adobe.jpeg
+-rw-r--r--   0        0        0    10421 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/airtame.png
+-rw-r--r--   0        0        0      876 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/allyhub.png
+-rw-r--r--   0        0        0     4615 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/alsid.png
+-rw-r--r--   0        0        0    12369 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/anchor.png
+-rw-r--r--   0        0        0     5200 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/australia.png
+-rw-r--r--   0        0        0     3371 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/austria.png
+-rw-r--r--   0        0        0    60306 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/aws.png
+-rw-r--r--   0        0        0     3030 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/belgium.png
+-rw-r--r--   0        0        0     5606 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/brazil.png
+-rw-r--r--   0        0        0     3693 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/canada.png
+-rw-r--r--   0        0        0     3870 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/chile.png
+-rw-r--r--   0        0        0     3086 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/colombia.png
+-rw-r--r--   0        0        0     3670 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/france.png
+-rw-r--r--   0        0        0     3212 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/germany.png
+-rw-r--r--   0        0        0     4521 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/hong-kong.png
+-rw-r--r--   0        0        0    12000 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/icon.png
+-rw-r--r--   0        0        0     4491 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/india.png
+-rw-r--r--   0        0        0     3622 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/italy.png
+-rw-r--r--   0        0        0     5096 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/malaysia.png
+-rw-r--r--   0        0        0     3897 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/mexico.png
+-rw-r--r--   0        0        0     3633 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/netherlands.png
+-rw-r--r--   0        0        0     5173 2023-07-14 17:51:00.197973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/new-zealand.png
+-rw-r--r--   0        0        0     4163 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/singapore.png
+-rw-r--r--   0        0        0     4670 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/spain.png
+-rw-r--r--   0        0        0     4802 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/sweden.png
+-rw-r--r--   0        0        0     3622 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/switzerland.png
+-rw-r--r--   0        0        0     4073 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/turkey.png
+-rw-r--r--   0        0        0     3350 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uae.png
+-rw-r--r--   0        0        0     5583 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uk.png
+-rw-r--r--   0        0        0     4892 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/usa.png
+-rw-r--r--   0        0        0     4063 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.css
+-rw-r--r--   0        0        0     1736 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.html.j2
+-rw-r--r--   0        0        0      592 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/sla/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/sla/__init__.py
+-rw-r--r--   0        0        0     4125 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/sla/entrypoint.py
+-rw-r--r--   0        0        0     9679 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/sla/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      260 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/subscription_list/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/subscription_list/__init__.py
+-rw-r--r--   0        0        0     6276 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/subscription_list/entrypoint.py
+-rw-r--r--   0        0        0     9302 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/subscription_list/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      203 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_list/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_list/__init__.py
+-rw-r--r--   0        0        0     4282 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_list/entrypoint.py
+-rw-r--r--   0        0        0     8925 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_list/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      228 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_requests/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_requests/__init__.py
+-rw-r--r--   0        0        0     5147 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_requests/entrypoint.py
+-rw-r--r--   0        0        0     9070 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_requests/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0      431 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/usage_in_subscription/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/usage_in_subscription/__init__.py
+-rw-r--r--   0        0        0     4106 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/usage_in_subscription/entrypoint.py
+-rw-r--r--   0        0        0     9137 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/usage_in_subscription/templates/xlsx/template.xlsx
+-rw-r--r--   0        0        0     1318 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/reports/utils.py
+-rw-r--r--   0        0        0    37904 2023-07-14 17:51:00.189972 connect_cli-27.7/connect/.data/connect_reports/reports.json
+-rw-r--r--   0        0        0      245 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/sonar-project.properties
+-rw-r--r--   0        0        0      321 2023-07-14 17:51:00.201973 connect_cli-27.7/connect/.data/connect_reports/tox.ini
+-rw-r--r--   0        0        0      352 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/__init__.py
+-rw-r--r--   0        0        0     1763 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/ccli.py
+-rw-r--r--   0        0        0       54 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/account/__init__.py
+-rw-r--r--   0        0        0     2433 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/account/commands.py
+-rw-r--r--   0        0        0     1233 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/account/helpers.py
+-rw-r--r--   0        0        0     2764 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/base.py
+-rw-r--r--   0        0        0     4048 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/config.py
+-rw-r--r--   0        0        0      573 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/constants.py
+-rw-r--r--   0        0        0     1424 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/http.py
+-rw-r--r--   0        0        0      838 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/plugins.py
+-rw-r--r--   0        0        0     6836 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/terminal.py
+-rw-r--r--   0        0        0     3139 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/core/utils.py
+-rw-r--r--   0        0        0        0 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/plugins/customer/__init__.py
+-rw-r--r--   0        0        0     2137 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/plugins/customer/commands.py
+-rw-r--r--   0        0        0      526 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/plugins/customer/constants.py
+-rw-r--r--   0        0        0     6040 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/plugins/customer/export.py
+-rw-r--r--   0        0        0    12696 2023-07-14 17:47:46.142966 connect_cli-27.7/connect/cli/plugins/customer/sync.py
+-rw-r--r--   0        0        0        0 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/locale/__init__.py
+-rw-r--r--   0        0        0     1363 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/locale/commands.py
+-rw-r--r--   0        0        0      306 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/play/__init__.py
+-rw-r--r--   0        0        0     2485 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/play/commands.py
+-rw-r--r--   0        0        0     2395 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/play/context.py
+-rw-r--r--   0        0        0      428 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/play/save.py
+-rw-r--r--   0        0        0     1647 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/play/script.py
+-rw-r--r--   0        0        0        0 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/__init__.py
+-rw-r--r--   0        0        0     1575 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/api.py
+-rw-r--r--   0        0        0     8628 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/clone.py
+-rw-r--r--   0        0        0     9659 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/commands.py
+-rw-r--r--   0        0        0     1289 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/constants.py
+-rw-r--r--   0        0        0    33455 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/export.py
+-rw-r--r--   0        0        0      846 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/sync/__init__.py
+-rw-r--r--   0        0        0     5932 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/sync/actions.py
+-rw-r--r--   0        0        0     8988 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/sync/capabilities.py
+-rw-r--r--   0        0        0     3881 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/sync/configuration_values.py
+-rw-r--r--   0        0        0     5096 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/sync/general.py
+-rw-r--r--   0        0        0    11349 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/sync/items.py
+-rw-r--r--   0        0        0     5846 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/sync/media.py
+-rw-r--r--   0        0        0     9460 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/sync/params.py
+-rw-r--r--   0        0        0     3598 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/sync/static_resources.py
+-rw-r--r--   0        0        0     5303 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/sync/templates.py
+-rw-r--r--   0        0        0      985 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/product/utils.py
+-rw-r--r--   0        0        0        0 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/__init__.py
+-rw-r--r--   0        0        0     5791 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/commands.py
+-rw-r--r--   0        0        0        0 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/__init__.py
+-rw-r--r--   0        0        0      411 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/constants.py
+-rw-r--r--   0        0        0    10802 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/helpers.py
+-rw-r--r--   0        0        0      103 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/__init__.py.j2
+-rw-r--r--   0        0        0      852 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/anvil.py.j2
+-rw-r--r--   0        0        0     2920 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/events.py.j2
+-rw-r--r--   0        0        0      464 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/extension.json.j2
+-rw-r--r--   0        0        0      560 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/schemas.py.j2
+-rw-r--r--   0        0        0        0 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/static/.gitkeep.j2
+-rw-r--r--   0        0        0     1762 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/tfnapp.py.j2
+-rw-r--r--   0        0        0     7295 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/webapp.py.j2
+-rw-r--r--   0        0        0      702 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.${project_slug}_dev.env.j2
+-rw-r--r--   0        0        0     1083 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.eslintrc.yaml.j2
+-rw-r--r--   0        0        0      231 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.flake8.j2
+-rw-r--r--   0        0        0     1309 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.github/workflows/test.yml.j2
+-rw-r--r--   0        0        0       96 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.gitignore.j2
+-rw-r--r--   0        0        0       63 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/CHANGELOG.md.j2
+-rw-r--r--   0        0        0      249 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/Dockerfile.j2
+-rw-r--r--   0        0        0     1661 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/HOWTO.md.j2
+-rw-r--r--   0        0        0    14063 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/LICENSE.j2
+-rw-r--r--   0        0        0      195 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/README.md.j2
+-rw-r--r--   0        0        0      111 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/__mocks__/fileMock.js.j2
+-rw-r--r--   0        0        0       97 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/__mocks__/styleMock.js.j2
+-rw-r--r--   0        0        0       39 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/babel.config.json.j2
+-rw-r--r--   0        0        0     1162 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/docker-compose.yml.j2
+-rw-r--r--   0        0        0      944 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/jest.config.js.j2
+-rw-r--r--   0        0        0     1246 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/package.json.j2
+-rw-r--r--   0        0        0       29 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/poetry.toml.j2
+-rw-r--r--   0        0        0     1960 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/pyproject.toml.j2
+-rw-r--r--   0        0        0      103 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/__init__.py.j2
+-rw-r--r--   0        0        0      559 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/conftest.py.j2
+-rw-r--r--   0        0        0      553 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_anvil.py.j2
+-rw-r--r--   0        0        0     2602 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_events.py.j2
+-rw-r--r--   0        0        0     1183 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_tfnapp.py.j2
+-rw-r--r--   0        0        0     8794 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_webapp.py.j2
+-rw-r--r--   0        0        0      947 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/images/mkp.svg.j2
+-rw-r--r--   0        0        0      729 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/index.html.j2
+-rw-r--r--   0        0        0      928 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/settings.html.j2
+-rw-r--r--   0        0        0      470 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/transformations/copy.html.j2
+-rw-r--r--   0        0        0     1590 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/transformations/manual.html.j2
+-rw-r--r--   0        0        0     2609 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/components.js.j2
+-rw-r--r--   0        0        0      323 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/index.js.j2
+-rw-r--r--   0        0        0      320 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/settings.js.j2
+-rw-r--r--   0        0        0      267 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/transformations/copy.js.j2
+-rw-r--r--   0        0        0      308 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages/transformations/manual.js.j2
+-rw-r--r--   0        0        0    10273 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages.js.j2
+-rw-r--r--   0        0        0     1579 2023-07-14 17:47:46.146966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/utils.js.j2
+-rw-r--r--   0        0        0     6381 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/index.css.j2
+-rw-r--r--   0        0        0      693 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/manual.css.j2
+-rw-r--r--   0        0        0     6508 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/components.spec.js.j2
+-rw-r--r--   0        0        0     9181 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/pages.spec.js.j2
+-rw-r--r--   0        0        0     4352 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/utils.spec.js.j2
+-rw-r--r--   0        0        0     2512 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/webpack.config.js.j2
+-rw-r--r--   0        0        0     4487 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/extension/utils.py
+-rw-r--r--   0        0        0      805 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/extension/validators.py
+-rw-r--r--   0        0        0    12083 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/extension/wizard.py
+-rw-r--r--   0        0        0     5929 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/renderer.py
+-rw-r--r--   0        0        0        0 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/__init__.py
+-rw-r--r--   0        0        0     8611 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/helpers.py
+-rw-r--r--   0        0        0       73 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/README.md.j2
+-rw-r--r--   0        0        0        0 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/__init__.py.j2
+-rw-r--r--   0        0        0     1507 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/entrypoint.py.j2
+-rw-r--r--   0        0        0        0 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/templates/pdf/template.css.j2
+-rw-r--r--   0        0        0      499 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/templates/pdf/template.html.j2.j2
+-rw-r--r--   0        0        0      150 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/templates/xml/template.xml.j2.j2
+-rw-r--r--   0        0        0       69 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/README.md.j2
+-rw-r--r--   0        0        0        0 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/__init__.py.j2
+-rw-r--r--   0        0        0     1507 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/entrypoint.py.j2
+-rw-r--r--   0        0        0        0 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/pdf/template.css.j2
+-rw-r--r--   0        0        0      518 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/pdf/template.html.j2.j2
+-rw-r--r--   0        0        0      150 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/xml/template.xml.j2.j2
+-rw-r--r--   0        0        0      271 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.flake8.j2
+-rw-r--r--   0        0        0      803 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.github/workflows/build.yml.j2
+-rw-r--r--   0        0        0       37 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.gitignore.j2
+-rw-r--r--   0        0        0      458 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/HOWTO.md.j2
+-rw-r--r--   0        0        0    14063 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/LICENSE.j2
+-rw-r--r--   0        0        0      138 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/README.md.j2
+-rw-r--r--   0        0        0       29 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/poetry.toml.j2
+-rw-r--r--   0        0        0     1352 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/pyproject.toml.j2
+-rw-r--r--   0        0        0     2589 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/reports.json.j2
+-rw-r--r--   0        0        0      103 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/__init__.py.j2
+-rw-r--r--   0        0        0     6397 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/conftest.py.j2
+-rw-r--r--   0        0        0     2534 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/test_${project_slug}.py.j2
+-rw-r--r--   0        0        0     5877 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/validations.py
+-rw-r--r--   0        0        0     8615 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/report/wizard.py
+-rw-r--r--   0        0        0     1443 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/utils.py
+-rw-r--r--   0        0        0     2798 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/project/validators.py
+-rw-r--r--   0        0        0        0 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/report/__init__.py
+-rw-r--r--   0        0        0     2405 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/report/commands.py
+-rw-r--r--   0        0        0       86 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/report/constants.py
+-rw-r--r--   0        0        0     6210 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/report/helpers.py
+-rw-r--r--   0        0        0     2822 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/report/utils.py
+-rw-r--r--   0        0        0     8345 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/report/wizard.py
+-rw-r--r--   0        0        0        0 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/shared/__init__.py
+-rw-r--r--   0        0        0     2441 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/shared/base.py
+-rw-r--r--   0        0        0     1973 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/shared/constants.py
+-rw-r--r--   0        0        0       46 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/shared/exceptions.py
+-rw-r--r--   0        0        0     2375 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/shared/export.py
+-rw-r--r--   0        0        0     6295 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/shared/sync_stats.py
+-rw-r--r--   0        0        0     5739 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/shared/translation_attr_sync.py
+-rw-r--r--   0        0        0     6534 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/shared/translation_sync.py
+-rw-r--r--   0        0        0     2103 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/shared/translations_synchronizers.py
+-rw-r--r--   0        0        0     6793 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/shared/utils.py
+-rw-r--r--   0        0        0        0 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/translation/__init__.py
+-rw-r--r--   0        0        0      707 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/translation/activate.py
+-rw-r--r--   0        0        0     6932 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/translation/commands.py
+-rw-r--r--   0        0        0      795 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/translation/constants.py
+-rw-r--r--   0        0        0     1228 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/translation/export.py
+-rw-r--r--   0        0        0      954 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/translation/primarize.py
+-rw-r--r--   0        0        0     9152 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/translation/translation_sync.py
+-rw-r--r--   0        0        0      818 2023-07-14 17:47:46.150966 connect_cli-27.7/connect/cli/plugins/translation/utils.py
+-rw-r--r--   0        0        0     4086 2023-07-14 17:51:01.037980 connect_cli-27.7/pyproject.toml
+-rw-r--r--   0        0        0     5060 1970-01-01 00:00:00.000000 connect_cli-27.7/PKG-INFO
```

### Comparing `connect_cli-27.6/LICENSE` & `connect_cli-27.7/LICENSE`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/README.md` & `connect_cli-27.7/README.md`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/.github/workflows/build.yml` & `connect_cli-27.7/connect/.data/connect_reports/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/LICENSE` & `connect_cli-27.7/connect/.data/connect_reports/LICENSE`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/README.md` & `connect_cli-27.7/connect/.data/connect_reports/README.md`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/poetry.lock` & `connect_cli-27.7/connect/.data/connect_reports/poetry.lock`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/pyproject.toml` & `connect_cli-27.7/connect/.data/connect_reports/pyproject.toml`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/billing_requests/entrypoint.py` & `connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/billing_requests/templates/xlsx/template.xlsx` & `connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/billing_requests_line_item/entrypoint.py` & `connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests_line_item/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/billing_requests_line_item/templates/xlsx/template.xlsx` & `connect_cli-27.7/connect/.data/connect_reports/reports/billing_requests_line_item/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/contract_list/entrypoint.py` & `connect_cli-27.7/connect/.data/connect_reports/reports/contract_list/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/contract_list/templates/xlsx/template.xlsx` & `connect_cli-27.7/connect/.data/connect_reports/reports/contract_list/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/customers_list/entrypoint.py` & `connect_cli-27.7/connect/.data/connect_reports/reports/customers_list/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/customers_list/templates/xlsx/template.xlsx` & `connect_cli-27.7/connect/.data/connect_reports/reports/customers_list/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/executive_fullfilment_requests/Readme.md` & `connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/Readme.md`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/executive_fullfilment_requests/constants.py` & `connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/constants.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/executive_fullfilment_requests/entrypoint.py` & `connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/img/ClouBlue-Logo.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/img/ClouBlue-Logo.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.css` & `connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.css`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.html.j2` & `connect_cli-27.7/connect/.data/connect_reports/reports/executive_fullfilment_requests/templates/pdf/template.html.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/fulfillment_requests/entrypoint.py` & `connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/fulfillment_requests/templates/xlsx/template.xlsx` & `connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/fulfillment_requests_failed/entrypoint.py` & `connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_failed/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/fulfillment_requests_failed/templates/xlsx/template.xlsx` & `connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_failed/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/fulfillment_requests_line_item/entrypoint.py` & `connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_line_item/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/fulfillment_requests_line_item/templates/xlsx/template.xlsx` & `connect_cli-27.7/connect/.data/connect_reports/reports/fulfillment_requests_line_item/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/helpdesk/entrypoint.py` & `connect_cli-27.7/connect/.data/connect_reports/reports/helpdesk/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/helpdesk/templates/xlsx/template.xlsx` & `connect_cli-27.7/connect/.data/connect_reports/reports/helpdesk/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/listing_list/entrypoint.py` & `connect_cli-27.7/connect/.data/connect_reports/reports/listing_list/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/listing_list/templates/xlsx/template.xlsx` & `connect_cli-27.7/connect/.data/connect_reports/reports/listing_list/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/listing_requests/entrypoint.py` & `connect_cli-27.7/connect/.data/connect_reports/reports/listing_requests/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/listing_requests/templates/xlsx/template.xlsx` & `connect_cli-27.7/connect/.data/connect_reports/reports/listing_requests/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/entrypoint.py` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-connect-alone.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-connect-alone.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-logo.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-logo.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-disabled.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-disabled.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-enabled.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cloudblue-small-color-enabled.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/connect-logo.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/connect-logo.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cover-bg.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/cover-bg.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/imc-small-color.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/assets/imc-small-color.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-Black.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-Black.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-White.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo-White.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/ClouBlue-Logo.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/accordo.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/accordo.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-blue.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-blue.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-white.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/acronis-white.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/adobe.jpeg` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/adobe.jpeg`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/airtame.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/airtame.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/allyhub.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/allyhub.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/alsid.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/alsid.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/anchor.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/anchor.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/australia.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/australia.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/austria.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/austria.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/aws.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/aws.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/belgium.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/belgium.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/brazil.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/brazil.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/canada.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/canada.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/chile.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/chile.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/colombia.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/colombia.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/france.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/france.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/germany.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/germany.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/hong-kong.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/hong-kong.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/icon.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/icon.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/india.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/india.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/italy.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/italy.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/malaysia.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/malaysia.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/mexico.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/mexico.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/netherlands.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/netherlands.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/new-zealand.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/new-zealand.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/singapore.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/singapore.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/spain.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/spain.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/sweden.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/sweden.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/switzerland.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/switzerland.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/turkey.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/turkey.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uae.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uae.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uk.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/uk.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/usa.png` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/img/usa.png`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.css` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.css`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.html.j2` & `connect_cli-27.7/connect/.data/connect_reports/reports/products_catalog/templates/pdf/template.html.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/sla/Readme.md` & `connect_cli-27.7/connect/.data/connect_reports/reports/sla/Readme.md`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/sla/entrypoint.py` & `connect_cli-27.7/connect/.data/connect_reports/reports/sla/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/sla/templates/xlsx/template.xlsx` & `connect_cli-27.7/connect/.data/connect_reports/reports/sla/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/subscription_list/entrypoint.py` & `connect_cli-27.7/connect/.data/connect_reports/reports/subscription_list/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/subscription_list/templates/xlsx/template.xlsx` & `connect_cli-27.7/connect/.data/connect_reports/reports/subscription_list/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/tier_configuration_list/entrypoint.py` & `connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_list/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/tier_configuration_list/templates/xlsx/template.xlsx` & `connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_list/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/tier_configuration_requests/entrypoint.py` & `connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_requests/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/tier_configuration_requests/templates/xlsx/template.xlsx` & `connect_cli-27.7/connect/.data/connect_reports/reports/tier_configuration_requests/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/usage_in_subscription/entrypoint.py` & `connect_cli-27.7/connect/.data/connect_reports/reports/usage_in_subscription/entrypoint.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/usage_in_subscription/templates/xlsx/template.xlsx` & `connect_cli-27.7/connect/.data/connect_reports/reports/usage_in_subscription/templates/xlsx/template.xlsx`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports/utils.py` & `connect_cli-27.7/connect/.data/connect_reports/reports/utils.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/.data/connect_reports/reports.json` & `connect_cli-27.7/connect/.data/connect_reports/reports.json`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/ccli.py` & `connect_cli-27.7/connect/cli/ccli.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 
 def main():
     _set_stdout_unbuffered()
     _ignore_openpyxl_warnings()
     try:
         import uvloop
+
         uvloop.install()
     except ImportError:
         pass
     print('')
     try:
         load_plugins(cli)
         cli(prog_name='ccli', standalone_mode=False)
@@ -41,14 +42,15 @@
     """
     Ignore warning about DataValidation extension not supported. This is shown when a xlsx file
     with unsupported data validation is opened (tipically after saving the file from Excel, which
     uses some custom extension).
     To avoid losing data validation, it should be re-created each time the file is saved by the cli.
     """
     import warnings
+
     warnings.filterwarnings('ignore', category=UserWarning, module='openpyxl.worksheet._reader')
 
 
 def _set_stdout_unbuffered():  # pragma: no cover
     if 'pytest' not in sys.modules:
         sys.stdout = io.TextIOWrapper(open(sys.stdout.fileno(), 'wb', 0), write_through=True)
         sys.stdout.reconfigure(encoding='utf-8')
```

### Comparing `connect_cli-27.6/connect/cli/core/account/commands.py` & `connect_cli-27.7/connect/cli/core/account/commands.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/core/account/helpers.py` & `connect_cli-27.7/connect/cli/core/account/helpers.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/core/base.py` & `connect_cli-27.7/connect/cli/core/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,37 +19,39 @@
         )
         return super().invoke(ctx)
 
 
 class CCliGroup(click.Group):
     def command(self, *args, **kwargs):
         from click.decorators import command
+
         kwargs['cls'] = CCliCommand
 
         def decorator(f):
             cmd = command(*args, **kwargs)(f)
             self.add_command(cmd)
             return cmd
 
         return decorator
 
     def group(self, *args, **kwargs):
         from click.decorators import group
+
         kwargs['cls'] = CCliGroup
 
         def decorator(f):
             cmd = group(*args, **kwargs)(f)
             self.add_command(cmd)
             return cmd
 
         return decorator
 
 
 def group(name=None, **attrs):
-    attrs.setdefault("cls", CCliGroup)
+    attrs.setdefault('cls', CCliGroup)
     return click.command(name, **attrs)
 
 
 def print_version(ctx, param, value):
     if not value or ctx.resilient_parsing:
         return
     console.echo(f'CloudBlue Connect CLI, version {get_version()}')
@@ -61,18 +63,21 @@
 @click.option(
     '--version',
     is_flag=True,
     expose_value=False,
     is_eager=True,
     callback=print_version,
 )
-@click.option('-c', '--config-dir',
-              default=os.path.join(os.path.expanduser('~'), '.ccli'),
-              type=click.Path(file_okay=False),
-              help='set the config directory.')
+@click.option(
+    '-c',
+    '--config-dir',
+    default=os.path.join(os.path.expanduser('~'), '.ccli'),
+    type=click.Path(file_okay=False),
+    help='set the config directory.',
+)
 @click.option(
     '-s',
     '--silent',
     is_flag=True,
     help='Prevent the output of informational messages.',
 )
 @click.option(
```

### Comparing `connect_cli-27.6/connect/cli/core/config.py` & `connect_cli-27.7/connect/cli/core/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
         if not os.path.isfile(self._config_path):
             return
 
         with open(self._config_path, 'r') as f:
             data = json.load(f)
             active_account_id = data['active']
             for account_data in data['accounts']:
-
                 account = Account(
                     **account_data,
                     client=ConnectClient(
                         account_data['api_key'],
                         endpoint=account_data['endpoint'],
                         use_specs=False,
                         max_retries=3,
```

### Comparing `connect_cli-27.6/connect/cli/core/constants.py` & `connect_cli-27.7/connect/cli/core/constants.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/core/http.py` & `connect_cli-27.7/connect/cli/core/http.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/core/plugins.py` & `connect_cli-27.7/connect/cli/core/plugins.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/core/terminal.py` & `connect_cli-27.7/connect/cli/core/terminal.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,14 @@
             spinner=spinner,
             spinner_style=spinner_style,
             speed=speed,
         )
 
 
 class Console(_Console):
-
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._skip_confirm = False
         self._silent = False
         self._verbose = False
         self._page_size = 25
 
@@ -129,15 +128,15 @@
     @page_size.setter
     def page_size(self, value):
         self._page_size = value
 
     def progress(self):
         return Progress(
             SpinnerColumn(),
-            TextColumn("[progress.description]{task.description:<80}"),
+            TextColumn('[progress.description]{task.description:<80}'),
             BarColumn(style='cyan', finished_style='green3'),
             MofNCompleteColumn(),
             TaskProgressColumn(),
             TimeElapsedColumn(),
             console=self,
             expand=True,
         )
@@ -155,15 +154,16 @@
         abort=False,
     ):
         if self._skip_confirm:
             return True
 
         self.print()
         prompt = Confirm(
-            message, console=self,
+            message,
+            console=self,
         )
 
         result = prompt(default=False)
         if not result and abort:
             raise Abort()
 
         self.print()
@@ -232,18 +232,19 @@
         columns=None,
         rows=None,
         expand=False,
     ):
         if not (columns and rows):
             return
 
-        chunks = [
-            rows[i:i + self.page_size]
-            for i in range(0, len(rows), self.page_size)
-        ] if not self.skip_confirm else [rows]
+        chunks = (
+            [rows[i : i + self.page_size] for i in range(0, len(rows), self.page_size)]
+            if not self.skip_confirm
+            else [rows]
+        )
 
         for chunk_count, chunk in enumerate(chunks):
             table = Table(
                 box=box.ROUNDED,
                 border_style='blue',
                 header_style='deep_sky_blue1',
                 expand=expand,
```

### Comparing `connect_cli-27.6/connect/cli/core/utils.py` & `connect_cli-27.7/connect/cli/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,39 +65,37 @@
     Common validation for commands using output path and file options.
     """
     if not default_file_name:
         default_file_name = default_dir_name
 
     output_path = output_path or os.getcwd()
     if not os.path.exists(output_path):
-        raise click.ClickException("Output Path does not exist")
+        raise click.ClickException('Output Path does not exist')
 
     output_path = os.path.join(output_path, default_dir_name)
     if not os.path.exists(output_path):
         os.mkdir(output_path)
     elif not os.path.isdir(output_path):  # pragma: no branch
         raise click.ClickException(
             f"Exists a file with name '{os.path.basename(output_path)}' but a directory is "
-            "expected, please rename it",
+            'expected, please rename it',
         )
 
     output_file = os.path.join(output_path, output_file or f'{default_file_name}.xlsx')
 
     return output_file
 
 
 def field_to_check_mark(predicate, false_value=''):
     """Change the value of a field to a check mark base on a predicate.
 
-        :param predicate: bool value / expression.
-        :param false_value: customizable value if predicate evaluates to false.
-        """
-    return (
-        '\u2713' if predicate else false_value
-    )
+    :param predicate: bool value / expression.
+    :param false_value: customizable value if predicate evaluates to false.
+    """
+    return '\u2713' if predicate else false_value
 
 
 def iter_entry_points(group, name=None):
     group_entrypoints = entry_points().get(group)
     if not group_entrypoints:
         return
     for ep in group_entrypoints:
```

### Comparing `connect_cli-27.6/connect/cli/plugins/customer/commands.py` & `connect_cli-27.7/connect/cli/plugins/customer/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,28 +53,27 @@
     )
 
 
 @grp_customer.command(
     name='sync',
     short_help='Synchronize customers from an excel file.',
 )
-
 @click.argument('input_file', metavar='input_file', nargs=1, required=True)  # noqa: E304
 @pass_config
 def cmd_sync_customers(config, input_file):
     acc_id = config.active.id
 
     if '.xlsx' not in input_file:
         input_file = f'{input_file}/{input_file}.xlsx'
 
     synchronizer = CustomerSynchronizer(
         client=config.active.client,
         account_id=acc_id,
     )
-    warnings.filterwarnings("ignore", category=UserWarning)
+    warnings.filterwarnings('ignore', category=UserWarning)
     synchronizer.open(input_file, 'Customers')
     synchronizer.sync()
     synchronizer.save(input_file)
     synchronizer.stats.print()
 
 
 def get_group():
```

### Comparing `connect_cli-27.6/connect/cli/plugins/customer/constants.py` & `connect_cli-27.7/connect/cli/plugins/customer/constants.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/customer/export.py` & `connect_cli-27.7/connect/cli/plugins/customer/export.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,28 +9,35 @@
 from connect.cli.core.terminal import console
 from connect.cli.core.utils import validate_output_options
 from connect.cli.plugins.customer.constants import COL_HEADERS
 
 
 def dump_customers(client, account_id, output_file, output_path=None):  # noqa: CCR001
     output_file = validate_output_options(
-        output_path, output_file, default_dir_name=account_id, default_file_name='customers',
+        output_path,
+        output_file,
+        default_dir_name=account_id,
+        default_file_name='customers',
     )
     try:
         wb = Workbook()
         _prepare_worksheet(wb.create_sheet('Customers'))
         _add_countries(wb.create_sheet('Countries'))
 
         customers = client.ns('tier').accounts.all()
         row_idx = 2
         count = customers.count()
         with console.progress() as progress:
             task = progress.add_task('Processing customer', total=count)
             for customer in customers:
-                progress.update(task, description=f'Processing customer {customer["id"]}', advance=1)
+                progress.update(
+                    task,
+                    description=f'Processing customer {customer["id"]}',
+                    advance=1,
+                )
                 _fill_customer_row(wb['Customers'], row_idx, customer)
                 row_idx += 1
             progress.update(task, completed=count)
     except ClientError as error:
         handle_http_error(error)
 
     default_sheet = wb['Sheet']
@@ -79,15 +86,17 @@
     ws.cell(row_idx, 14, value=customer['contact_info'].get('state', '-'))
     ws.cell(row_idx, 15, value=customer['contact_info'].get('zip', '-'))
     ws.cell(row_idx, 16, value=customer['contact_info'].get('country', '-'))
     ws.cell(row_idx, 17, value=customer['contact_info']['contact'].get('first_name', '-'))
     ws.cell(row_idx, 18, value=customer['contact_info']['contact'].get('last_name', '-'))
     ws.cell(row_idx, 19, value=customer['contact_info']['contact'].get('email', '-'))
     ws.cell(
-        row_idx, 20, value=_get_phone_number(
+        row_idx,
+        20,
+        value=_get_phone_number(
             customer['contact_info']['contact'].get(
                 'phone_number',
                 '-',
             ),
         ),
     )
 
@@ -109,15 +118,15 @@
         output_number += number['extension']
     return output_number
 
 
 def _prepare_worksheet(ws):
     color = Color('d3d3d3')
     fill = PatternFill('solid', color)
-    cels = ws['A1': 'T1']
+    cels = ws['A1':'T1']
     for cel in cels[0]:
         if cel.column_letter in ['J', 'K', 'L']:
             ws.column_dimensions[cel.column_letter].width = 50
         elif cel.column_letter in ['B', 'D', 'E', 'F']:
             ws.column_dimensions[cel.column_letter].width = 15
         else:
             ws.column_dimensions[cel.column_letter].width = 20
@@ -132,15 +141,15 @@
         'B': 'Country name',
     }
     color = Color('d3d3d3')
     fill = PatternFill('solid', color)
     ws.column_dimensions['A'].width = 15
     ws.column_dimensions['A'].auto_size = True
     ws.column_dimensions['B'].width = 50
-    cels = ws['A1': 'B1']
+    cels = ws['A1':'B1']
     for cel in cels[0]:
         cel.fill = fill
         cel.value = col_headers[cel.column_letter]
     row_idx = 2
     for country in countries:
         ws.cell(row_idx, 1, value=country.alpha2)
         ws.cell(row_idx, 2, value=country.name)
```

### Comparing `connect_cli-27.6/connect/cli/plugins/customer/sync.py` & `connect_cli-27.7/connect/cli/plugins/customer/sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         except InvalidFileException as ife:
             raise ClickException(str(ife))
         except BadZipFile:
             raise ClickException(f'{input_file} is not a valid xlsx file.')
 
     @staticmethod
     def _validate_worksheet_sheet(ws):
-        cels = ws['A1': 'T1']
+        cels = ws['A1':'T1']
         for cel in cels[0]:
             if cel.value != COL_HEADERS[cel.column_letter]:
                 raise ClickException(
                     f'Column `{cel.coordinate}` must be `{COL_HEADERS[cel.column_letter]}` '
                     f'and is `{cel.value}`.',
                 )
 
@@ -86,62 +86,67 @@
                     self.stats.skipped()
                     continue
                 row_errors = self._validate_row(data)
                 if row_errors:
                     self.stats.error(row_errors, row_idx)
                     continue
                 if data.parent_search_criteria and not data.parent_search_value:
-                    self.stats.error("Parent search value is needed if criteria is set", row_idx)
+                    self.stats.error('Parent search value is needed if criteria is set', row_idx)
                     continue
                 if data.hub_id and (data.hub_id != '' or data.hub_id != '-'):
                     if data.hub_id not in self.hubs:
-                        self.stats.error(f"Accounts on hub {data.hub_id} can not be modified", row_idx)
+                        self.stats.error(
+                            f'Accounts on hub {data.hub_id} can not be modified',
+                            row_idx,
+                        )
                         continue
                 name = f'{data.technical_contact_first_name} {data.technical_contact_last_name}'
                 model = {
-                    "type": data.type,
-                    "name": data.company_name if data.company_name else name,
-                    "contact_info": {
-                        "address_line1": data.address_line_1,
-                        "address_line2": data.address_line_2,
-                        "city": data.city,
-                        "country": data.country,
-                        "postal_code": data.zip,
-                        "state": data.state,
-                        "contact": {
-                            "first_name": data.technical_contact_first_name,
-                            "last_name": data.technical_contact_last_name,
-                            "email": data.technical_contact_email,
+                    'type': data.type,
+                    'name': data.company_name if data.company_name else name,
+                    'contact_info': {
+                        'address_line1': data.address_line_1,
+                        'address_line2': data.address_line_2,
+                        'city': data.city,
+                        'country': data.country,
+                        'postal_code': data.zip,
+                        'state': data.state,
+                        'contact': {
+                            'first_name': data.technical_contact_first_name,
+                            'last_name': data.technical_contact_last_name,
+                            'email': data.technical_contact_email,
                         },
                     },
                 }
                 if data.external_id:
                     model['external_id'] = data.external_id
                 if data.external_uid:
                     model['external_uid'] = data.external_uid
                 else:
                     model['external_uid'] = str(uuid.uuid4())
                 if data.technical_contact_phone:
                     try:
                         phone = phonenumbers.parse(data.technical_contact_phone, data.country)
                         phone_number = {
-                            "country_code": f'+{str(phone.country_code)}',
-                            "area_code": '',
-                            "extension": str(phone.extension) if phone.extension else '-',
+                            'country_code': f'+{str(phone.country_code)}',
+                            'area_code': '',
+                            'extension': str(phone.extension) if phone.extension else '-',
                             'phone_number': str(phone.national_number),
                         }
                         model['contact_info']['contact']['phone_number'] = phone_number
                     except Exception:
                         pass
                 if data.parent_search_criteria != '-':
                     model['parent'] = {}
                     if data.parent_search_criteria == 'id':
                         if data.parent_search_value not in parent_id:
                             try:
-                                pacc = self._client.ns('tier').accounts[data.parent_search_value].get()
+                                pacc = (
+                                    self._client.ns('tier').accounts[data.parent_search_value].get()
+                                )
                                 parent_id.append(pacc['id'])
                             except ClientError:
                                 self.stats.error(
                                     f'Parent with id {data.parent_search_value} does not exist',
                                     row_idx,
                                 )
                                 continue
@@ -163,15 +168,16 @@
                                         f'More than one Parent with external_id {data.parent_search_value}',
                                         row_idx,
                                     )
                                     continue
                                 parent_external_id[data.parent_search_value] = pacc[0]['id']
                             except ClientError:
                                 self.stats.error(
-                                    'Error when obtaining parent data from Connect', row_idx,
+                                    'Error when obtaining parent data from Connect',
+                                    row_idx,
                                 )
                                 continue
                         model['parent']['id'] = parent_external_id[data.parent_search_value]
                     else:
                         if data.parent_search_value not in parent_uuid:
                             try:
                                 r = R().external_uid.eq(str(data.parent_search_value))
@@ -187,35 +193,38 @@
                                         f'More than one Parent with external_uid {data.parent_search_value}',
                                         row_idx,
                                     )
                                     continue
                                 parent_uuid[data.parent_search_value] = pacc[0]['id']
                             except ClientError:
                                 self.stats.error(
-                                    'Error when obtaining parent data from Connect', row_idx,
+                                    'Error when obtaining parent data from Connect',
+                                    row_idx,
                                 )
                                 continue
                         model['parent']['id'] = parent_uuid[data.parent_search_value]
                 if data.action == 'create':
                     try:
                         account = self._client.ns('tier').accounts.create(model)
                     except ClientError as e:
                         self.stats.error(
-                            f'Error when creating account: {str(e)}', row_idx,
+                            f'Error when creating account: {str(e)}',
+                            row_idx,
                         )
                         continue
                     self.stats.created()
                     self._update_sheet_row(ws, row_idx, account)
                 else:
                     try:
                         model['id'] = data.id
                         account = self._client.ns('tier').accounts[data.id].update(model)
                     except ClientError as e:
                         self.stats.error(
-                            f'Error when updating account: {str(e)}', row_idx,
+                            f'Error when updating account: {str(e)}',
+                            row_idx,
                         )
                         continue
                     self.stats.updated()
                     self._update_sheet_row(ws, row_idx, account)
             progress.update(task, completed=ws.max_row - 1)
 
     @staticmethod
@@ -231,31 +240,33 @@
             return errors
         if row.action == '-':
             return
         if row.type not in ('customer', 'reseller'):
             errors.append(f'Customer type must be customer or reseller, not {row.type}')
             return errors
         if not all(
-                [
-                    row.address_line_1,
-                    row.city,
-                    row.state,
-                    row.zip,
-                    row.technical_contact_first_name,
-                    row.technical_contact_last_name,
-                    row.technical_contact_email,
-                ],
+            [
+                row.address_line_1,
+                row.city,
+                row.state,
+                row.zip,
+                row.technical_contact_first_name,
+                row.technical_contact_last_name,
+                row.technical_contact_email,
+            ],
         ):
             errors.append('Address line 1, city, state and zip are mandatory')
             return errors
         if row.action == 'create' and row.id is not None:
             errors.append(f'Create action must not have account id, is set to {row.id}')
             return errors
-        if row.action == 'create' and row.type == 'customer' and (
-                row.parent_search_criteria == '' or row.parent_search_criteria == '-'
+        if (
+            row.action == 'create'
+            and row.type == 'customer'
+            and (row.parent_search_criteria == '' or row.parent_search_criteria == '-')
         ):
             errors.append('Customers requires a parent account')
             return errors
         if row.action == 'update' and not row.id.startswith('TA-'):
             errors.append('Update operation requires account ID to be set')
             return errors
         if row.action == 'update':
```

### Comparing `connect_cli-27.6/connect/cli/plugins/locale/commands.py` & `connect_cli-27.7/connect/cli/plugins/locale/commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,18 +37,18 @@
             'ID',
             'Name',
             ('center', 'Autotranslation'),
             ('center', 'Translations'),
         ],
         rows=[
             (
-                resource["id"],
-                resource["name"],
-                field_to_check_mark(resource["auto_translation"], false_value='\u2716'),
-                resource["stats"]["translations"] or '-',
+                resource['id'],
+                resource['name'],
+                field_to_check_mark(resource['auto_translation'], false_value='\u2716'),
+                resource['stats']['translations'] or '-',
             )
             for resource in query_locales
         ],
     )
 
 
 def get_group():
```

### Comparing `connect_cli-27.6/connect/cli/plugins/play/commands.py` & `connect_cli-27.7/connect/cli/plugins/play/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 pass_arg = PassArgumentDecorator
 
 
 def setup_script_command(cls):
     @pass_config
     @pass_arg(cls)
     def cmd_play_custom(script_class, config, **kwargs):
-
         Context.context_file_name = PlayOptions.context_file
         ctx = Context.create(**kwargs)
 
         if 'endpoint' not in ctx or not ctx.endpoint:
             ctx.endpoint = config.active.endpoint
 
         if 'distributor_account_token' not in ctx or not ctx.distributor_account_token:
@@ -58,15 +57,15 @@
     grp_play.command(name=cls.command(), short_help=cls.help())(cmd_play_custom)
 
 
 def load_one_script(scripts, filename):
     modname = filename[0:-3]
 
     try:
-        mod = __import__(modname, globals={"__name__": __name__}, fromlist=['*'])
+        mod = __import__(modname, globals={'__name__': __name__}, fromlist=['*'])
 
         if not hasattr(mod, '__all__'):
             print(f'Warning: {filename} has no __all__ defined', file=sys.stderr)
             return
 
         for cname in mod.__all__:
             cls = getattr(mod, cname)
```

### Comparing `connect_cli-27.6/connect/cli/plugins/play/context.py` & `connect_cli-27.7/connect/cli/plugins/play/context.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/play/script.py` & `connect_cli-27.7/connect/cli/plugins/play/script.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,25 @@
 
     def __init__(self, context=None, **kwargs):
         self.context = context if context is not None else Context()
         self.context.update(kwargs)
 
     @classmethod
     def command(cls) -> str:
-        return str(re.sub(r'^([A-Z])', lambda x: x.group(1).lower(),
-                   re.sub(r'([a-z])([A-Z])', lambda x: f'{x.group(1)}-{x.group(2).lower()}', cls.__name__)))
+        return str(
+            re.sub(
+                r'^([A-Z])',
+                lambda x: x.group(1).lower(),
+                re.sub(
+                    r'([a-z])([A-Z])',
+                    lambda x: f'{x.group(1)}-{x.group(2).lower()}',
+                    cls.__name__,
+                ),
+            ),
+        )
 
     @classmethod
     def help(cls) -> str:
         return cls.__doc__
 
     @classmethod
     def options(cls) -> List[OptionWrapper]:
```

### Comparing `connect_cli-27.6/connect/cli/plugins/product/api.py` & `connect_cli-27.7/connect/cli/plugins/product/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,34 +26,26 @@
     return res
 
 
 def get_item_by_mpn(client, product_id, mpn):
     rql = R().mpn.eq(mpn)
 
     try:
-        res = (
-            client.products[product_id]
-            .items
-            .filter(rql)
-        )
+        res = client.products[product_id].items.filter(rql)
         return res.first()
 
     except ClientError as error:
         if error.status_code == 404:
             return
         handle_http_error(error)
 
 
 def create_item(client, product_id, data):
     try:
-        res = (
-            client.products[product_id]
-            .items
-            .create(data)
-        )
+        res = client.products[product_id].items.create(data)
     except ClientError as error:
         handle_http_error(error)
 
     return res
 
 
 def update_item(client, product_id, item_id, data):
```

### Comparing `connect_cli-27.6/connect/cli/plugins/product/clone.py` & `connect_cli-27.7/connect/cli/plugins/product/clone.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from connect.cli.plugins.shared.utils import get_translation_attributes_sheets
 
 
 class ProductCloner:
     def __init__(self, config, source_account, destination_account, product_id, progress, stats):
         self.fs = TempFS(identifier=f'_clone_{product_id}')
         self.config = config
-        self.source_account = (source_account if source_account else config.active.id)
-        self.destination_account = (destination_account if destination_account else config.active.id)
+        self.source_account = source_account if source_account else config.active.id
+        self.destination_account = destination_account if destination_account else config.active.id
         self.product_id = product_id
         self.stats = stats
         self.progress = progress
         self.destination_product = None
         self.wb = None
 
     def dump(self):
@@ -94,21 +94,21 @@
 
             synchronizer = ParamsSynchronizer(
                 self.config.active.client,
                 self.progress,
                 self.stats,
             )
 
-            synchronizer.open(input_file, "Ordering Parameters")
+            synchronizer.open(input_file, 'Ordering Parameters')
             synchronizer.sync()
 
-            synchronizer.open(input_file, "Fulfillment Parameters")
+            synchronizer.open(input_file, 'Fulfillment Parameters')
             synchronizer.sync()
 
-            synchronizer.open(input_file, "Configuration Parameters")
+            synchronizer.open(input_file, 'Configuration Parameters')
             synchronizer.sync()
 
             synchronizer = ActionsSynchronizer(
                 self.config.active.client,
                 self.progress,
                 self.stats,
             )
@@ -132,41 +132,41 @@
                 self.stats,
                 save=False,
                 is_clone=True,
             )
 
             self.config.activate(self.source_account)
         except ClientError as e:
-            raise ClickException(f"Error while cloning product: {str(e)}")
+            raise ClickException(f'Error while cloning product: {str(e)}')
 
     def load_wb(self):
         self.wb = load_workbook(
             f'{self.fs.root_path}/{self.product_id}/{self.product_id}.xlsx',
             data_only=True,
         )
 
     def create_product(self, name=None):
         if not name:
             time = datetime.today().strftime('%Y-%m-%d-%H:%M:%S')
-            name = f"Clone of {self.product_id} {time}"
+            name = f'Clone of {self.product_id} {time}'
         ws = self.wb['General Information']
         ws['B6'].value = name
         self.config.activate(self.destination_account)
 
         try:
             category = self._get_cat_id(self.config.active.client, ws['B8'].value)
             primary_locale_id = self._get_primary_locale_id(ws['B14'].value)
             product = self.config.active.client.products.create(
                 {
-                    "name": name,
-                    "category": {
-                        "id": category,
+                    'name': name,
+                    'category': {
+                        'id': category,
                     },
-                    "translations": [
-                        {"locale": {"id": primary_locale_id}, "primary": True},
+                    'translations': [
+                        {'locale': {'id': primary_locale_id}, 'primary': True},
                     ],
                 },
             )
             if name:
                 ws['B6'].value = name
             ws['B5'].value = product['id']
             self.destination_product = product['id']
```

### Comparing `connect_cli-27.6/connect/cli/plugins/product/commands.py` & `connect_cli-27.7/connect/cli/plugins/product/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,14 @@
     )
 
 
 @grp_product.command(
     name='export',
     short_help='Export a product to an excel file.',
 )
-
 @click.argument('product_id', metavar='product_id', nargs=1, required=True)  # noqa: E304
 @click.option(
     '--out',
     '-o',
     'output_file',
     type=click.Path(exists=False, file_okay=True, dir_okay=False),
     help='Output Excel file name.',
@@ -117,16 +116,15 @@
     if '.xlsx' not in input_file:
         input_file = f'{input_file}/{input_file}.xlsx'
 
     synchronizer = GeneralSynchronizer(config.active.client, None)
     product_id = synchronizer.open(input_file, 'General Information')
 
     console.confirm(
-        'Are you sure you want to synchronize '
-        f'the product {product_id} ?',
+        'Are you sure you want to synchronize ' f'the product {product_id} ?',
         abort=True,
     )
     console.echo('')
 
     with console.progress() as progress:
         general_errors = synchronizer.sync()
         if general_errors:
@@ -162,15 +160,14 @@
     stats.print()
 
 
 @grp_product.command(
     name='clone',
     short_help='Create a clone of a product.',
 )
-
 @click.argument('source_product_id', metavar='product_id', nargs=1, required=True)  # noqa: E304
 @click.option(
     '--source_account',
     '-s',
     'source_account',
     help='Source account ID',
 )
@@ -190,31 +187,30 @@
 def cmd_clone_products(config, source_product_id, source_account, destination_account, name):
     if not config.active.is_vendor():
         raise ClickException(
             'The clone command is only available for vendor accounts.',
         )
     if name and len(name) > 32:
         raise ClickException(
-            f'New product name can not exceed 32 chracters, provided as name {name}',
+            f'New product name can not exceed 32 characters, provided as name {name}',
         )
     if destination_account:
         if not config.exists(destination_account):
             raise ClickException(f'The destination account {destination_account} does not exist.')
     else:
         destination_account = config.active.id
 
     if source_account:
         if not config.exists(source_account):
             raise ClickException(f'The source account {source_account} does not exist.')
     else:
         source_account = config.active.id
 
     console.confirm(
-        'Are you sure you want to Clone '
-        f'the product {source_product_id} ?',
+        'Are you sure you want to Clone ' f'the product {source_product_id} ?',
         abort=True,
     )
     console.echo('')
 
     try:
         config.active.client.products[source_product_id].get()
     except ClientError:
@@ -222,15 +218,14 @@
 
     stats = SynchronizerStats(
         operation='Clone',
         header=f'Results of cloning {source_product_id}',
     )
 
     with console.status_progress() as (status, progress):
-
         synchronizer = ProductCloner(
             config=config,
             source_account=source_account,
             destination_account=destination_account,
             product_id=source_product_id,
             progress=progress,
             stats=stats,
```

### Comparing `connect_cli-27.6/connect/cli/plugins/product/constants.py` & `connect_cli-27.7/connect/cli/plugins/product/constants.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/product/export.py` & `connect_cli-27.7/connect/cli/plugins/product/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,27 +110,25 @@
     ws['A13'].value = 'Embedding getting started'
     ws['B13'].value = product['customer_ui_settings']['getting_started']
     ws['B13'].alignment = Alignment(
         wrap_text=True,
     )
     ws['A14'].value = 'Primary Translation Locale'
     primary_translation = (
-        client.ns('localization').translations
-        .filter(context__instance_id=product['id'], primary=True).first()
-    )
-    ws['B14'].value = (
-        f'{ primary_translation["locale"]["id"] } '
-        f'({ primary_translation["locale"]["name"] })'
+        client.ns('localization')
+        .translations.filter(context__instance_id=product['id'], primary=True)
+        .first()
     )
+    ws[
+        'B14'
+    ].value = f'{ primary_translation["locale"]["id"] } ({ primary_translation["locale"]["name"] })'
 
     categories = client.categories.all()
     unassignable_cat = ['Cloud Services', 'All Categories']
-    categories_list = [
-        cat['name'] for cat in categories if cat['name'] not in unassignable_cat
-    ]
+    categories_list = [cat['name'] for cat in categories if cat['name'] not in unassignable_cat]
     ws['AA1'].value = 'Categories'
     for idx, cat in enumerate(categories_list, 2):
         ws[f'AA{idx}'].value = cat
     categories_validation = DataValidation(
         type='list',
         formula1=f'{quote_sheetname("General Information")}!$AA$2:$AA${idx}',
         allow_blank=False,
@@ -141,26 +139,28 @@
 
 def _dump_image(image_location, image_name, media_path):
     image = requests.get(image_location)
     if image.status_code == 200:
         with open(os.path.join(media_path, image_name), 'wb') as f:
             f.write(image.content)
     else:
-        raise ClickException(f"Error obtaining image from {image_location}")
+        raise ClickException(f'Error obtaining image from {image_location}')
 
 
 def _setup_ws_header(ws, ws_type=None):  # noqa: CCR001
     if not ws_type:
         ws_type = 'items'
 
     color = Color('d3d3d3')
     fill = PatternFill('solid', color)
-    cels = ws['A1': '{cell}1'.format(
-        cell=get_col_limit_by_ws_type(ws_type),
-    )]
+    cels = ws[
+        'A1' : '{cell}1'.format(
+            cell=get_col_limit_by_ws_type(ws_type),
+        )
+    ]
     col_headers = get_col_headers_by_ws_type(ws_type)
     if ws_type == '_attributes':
         col_headers = {c.column_letter: c.value for c in next(ws.iter_rows(min_row=1, max_row=1))}
     for cel in cels[0]:
         ws.column_dimensions[cel.column_letter].width = 25
         ws.column_dimensions[cel.column_letter].auto_size = True
         cel.fill = fill
@@ -240,49 +240,57 @@
         vertical='top',
     )
     ws.cell(row_idx, 8, value=param['type']).alignment = Alignment(
         horizontal='left',
         vertical='top',
     )
     ws.cell(
-        row_idx, 9,
+        row_idx,
+        9,
         value=param['constraints']['required'] if param['constraints']['required'] else '-',
     ).alignment = Alignment(
         horizontal='left',
         vertical='top',
     )
     ws.cell(
-        row_idx, 10,
+        row_idx,
+        10,
         value=param['constraints']['unique'] if param['constraints']['unique'] else '-',
     ).alignment = Alignment(
         horizontal='left',
         vertical='top',
     )
     ws.cell(
-        row_idx, 11,
+        row_idx,
+        11,
         value=param['constraints']['hidden'] if param['constraints']['hidden'] else '-',
     ).alignment = Alignment(
         horizontal='left',
         vertical='top',
     )
     ws.cell(
-        row_idx, 12,
+        row_idx,
+        12,
         value=get_json_object_for_param(param),
     ).alignment = Alignment(
         wrap_text=True,
     )
     events = param.get('events', {})
     ws.cell(
-        row_idx, 13, value=events.get('created', {}).get('at', '-'),
+        row_idx,
+        13,
+        value=events.get('created', {}).get('at', '-'),
     ).alignment = Alignment(
         horizontal='left',
         vertical='top',
     )
     ws.cell(
-        row_idx, 14, value=events.get('updated', {}).get('at', '-'),
+        row_idx,
+        14,
+        value=events.get('updated', {}).get('at', '-'),
     ).alignment = Alignment(
         horizontal='left',
         vertical='top',
     )
 
 
 def _fill_media_row(ws, row_idx, media, location, product, media_path):
@@ -313,31 +321,37 @@
         vertical='top',
     )
     ws.cell(row_idx, 4, value=template['scope']).alignment = Alignment(
         horizontal='left',
         vertical='top',
     )
     ws.cell(
-        row_idx, 5, value=template['type'] if 'type' in template else 'fulfillment',
+        row_idx,
+        5,
+        value=template['type'] if 'type' in template else 'fulfillment',
     ).alignment = Alignment(
         horizontal='left',
         vertical='top',
     )
     ws.cell(row_idx, 6, value=template['body']).alignment = Alignment(
         wrap_text=True,
     )
     events = template.get('events', {})
     ws.cell(
-        row_idx, 7, value=events.get('created', {}).get('at', '-'),
+        row_idx,
+        7,
+        value=events.get('created', {}).get('at', '-'),
     ).alignment = Alignment(
         horizontal='left',
         vertical='top',
     )
     ws.cell(
-        row_idx, 8, value=events.get('updated', {}).get('at', '-'),
+        row_idx,
+        8,
+        value=events.get('updated', {}).get('at', '-'),
     ).alignment = Alignment(
         horizontal='left',
         vertical='top',
     )
 
 
 def _fill_action_row(ws, row_idx, action):
@@ -356,17 +370,24 @@
 def _fill_configuration_row(ws, row_idx, configuration, conf_id):
     ws.cell(row_idx, 1, value=conf_id)
     ws.cell(row_idx, 2, value=configuration['parameter']['id'])
     ws.cell(row_idx, 3, value=configuration['parameter']['scope'])
     ws.cell(row_idx, 4, value='-')
     ws.cell(row_idx, 5, value=configuration['item']['id'] if 'item' in configuration else '-')
     ws.cell(row_idx, 6, value=configuration['item']['name'] if 'item' in configuration else '-')
-    ws.cell(row_idx, 7, value=configuration['marketplace']['id'] if 'marketplace' in configuration else '-')
-    ws.cell(row_idx, 8,
-            value=configuration['marketplace']['name'] if 'marketplace' in configuration else '-')
+    ws.cell(
+        row_idx,
+        7,
+        value=configuration['marketplace']['id'] if 'marketplace' in configuration else '-',
+    )
+    ws.cell(
+        row_idx,
+        8,
+        value=configuration['marketplace']['name'] if 'marketplace' in configuration else '-',
+    )
     if 'structured_value' in configuration:
         value = configuration['structured_value']
         value = json.dumps(value, indent=4, sort_keys=True)
         ws.cell(row_idx, 9, value=value).alignment = Alignment(wrap_text=True)
     elif 'value' in configuration:
         ws.cell(row_idx, 9, value=configuration['value'])
     else:
@@ -377,15 +398,15 @@
     ws.cell(row_idx, 1, value=item['id'])
     ws.cell(row_idx, 2, value=item['mpn'])
     ws.cell(row_idx, 3, value='-')
     ws.cell(row_idx, 4, value=item['display_name'])
     ws.cell(row_idx, 5, value=item['description'])
     ws.cell(row_idx, 6, value=item['type'])
     ws.cell(row_idx, 7, value=item['precision'])
-    ws.cell(row_idx, 8, value=item['unit']['unit'])
+    ws.cell(row_idx, 8, value=item['unit']['id'])
     period = item.get('period', 'monthly')
     if period.startswith('years_'):
         period = f'{period.rsplit("_")[-1]} years'
     ws.cell(row_idx, 9, value=period)
     ws.cell(row_idx, 10, value=_calculate_commitment(item))
     ws.cell(row_idx, 11, value=item['status'])
     events = item.get('events', {})
@@ -462,15 +483,19 @@
 
     ws.add_data_validation(action_validation)
 
     task = progress.add_task('Processing parameter configuration', total=count)
 
     for configuration in configurations:
         conf_id = _calculate_configuration_id(configuration)
-        progress.update(task, description=f'Processing parameter configuration {conf_id}', advance=1)
+        progress.update(
+            task,
+            description=f'Processing parameter configuration {conf_id}',
+            advance=1,
+        )
         _fill_configuration_row(ws, row_idx, configuration, conf_id)
         action_validation.add(f'D{row_idx}')
         row_idx += 1
 
     progress.update(task, completed=count)
 
 
@@ -650,33 +675,27 @@
     ws.add_data_validation(action_validation)
     ws.add_data_validation(ppu_validation)
     ws.add_data_validation(disabled_enabled)
     ws.add_data_validation(tier_validation)
 
     ws['A2'].value = 'Pay-as-you-go support and schema'
     ws['B2'].value = '-'
-    ws['C2'].value = (ppu['schema'] if ppu else 'Disabled')
+    ws['C2'].value = ppu['schema'] if ppu else 'Disabled'
     ppu_validation.add(ws['C2'])
     ws['A3'].value = 'Pay-as-you-go dynamic items support'
     ws['B3'].value = '-'
-    ws['C3'].value = (
-        'Enabled' if ppu and 'dynamic' in ppu and ppu['dynamic'] else 'Disabled'
-    )
+    ws['C3'].value = 'Enabled' if ppu and 'dynamic' in ppu and ppu['dynamic'] else 'Disabled'
     disabled_enabled.add(ws['C3'])
     ws['A4'].value = 'Pay-as-you-go future charges support'
     ws['B4'].value = '-'
-    ws['C4'].value = (
-        'Enabled' if ppu and 'future' in ppu and ppu['future'] else 'Disabled'
-    )
+    ws['C4'].value = 'Enabled' if ppu and 'future' in ppu and ppu['future'] else 'Disabled'
     disabled_enabled.add(ws['C4'])
     ws['A5'].value = 'Consumption reporting for Reservation Items'
     ws['B5'].value = '-'
-    ws['C5'].value = (
-        'Enabled' if capabilities['reservation']['consumption'] else 'Disabled'
-    )
+    ws['C5'].value = 'Enabled' if capabilities['reservation']['consumption'] else 'Disabled'
     disabled_enabled.add(ws['C5'])
 
     def _get_reporting_consumption(reservation_cap):
         if 'consumption' in reservation_cap and reservation_cap['consumption']:
             return 'Enabled'
         return 'Disabled'
 
@@ -685,14 +704,15 @@
     ws['A6'].value = 'Dynamic Validation of the Draft Requests'
     ws['B6'].value = '-'
 
     def _get_dynamic_validation_draft(capabilities_cart):
         if 'validation' in capabilities_cart and capabilities['cart']['validation']:
             return 'Enabled'
         return 'Disabled'
+
     ws['C6'].value = _get_dynamic_validation_draft(capabilities['cart'])
     disabled_enabled.add(ws['C6'])
     ws['A7'].value = 'Dynamic Validation of the Inquiring Form'
     ws['B7'].value = '-'
 
     def _get_validation_inquiring(capabilities_inquiring):
         if 'validation' in capabilities_inquiring and capabilities_inquiring['validation']:
@@ -709,43 +729,39 @@
             return tiers['configs']['level']
         return 'Disabled'
 
     ws['C8'].value = _get_reseller_authorization_level(tiers)
     tier_validation.add(ws['C8'])
     ws['A9'].value = 'Tier Accounts Sync'
     ws['B9'].value = '-'
-    ws['C9'].value = (
-        'Enabled' if tiers and 'updates' in tiers and tiers['updates'] else 'Disabled'
-    )
+    ws['C9'].value = 'Enabled' if tiers and 'updates' in tiers and tiers['updates'] else 'Disabled'
     disabled_enabled.add(ws['C9'])
     ws['A10'].value = 'Administrative Hold'
     ws['B10'].value = '-'
 
     ws['A11'].value = 'Dynamic Validation of Tier Requests'
     ws['B11'].value = '-'
-    ws['C11'].value = (
-        'Enabled' if capabilities['tiers']['validation'] else 'Disabled'
-    )
+    ws['C11'].value = 'Enabled' if capabilities['tiers']['validation'] else 'Disabled'
     disabled_enabled.add(ws['C11'])
     ws['A12'].value = 'Editable Ordering Parameters in Change Request'
     ws['B12'].value = '-'
     ws['C12'].value = (
         'Enabled' if subscription['change']['editable_ordering_parameters'] else 'Disabled'
     )
     disabled_enabled.add(ws['C12'])
     ws['A13'].value = 'Validation of Draft Change Request'
     ws['B13'].value = '-'
-    ws['C13'].value = (
-        'Enabled' if 'validation' in change and change['validation'] else 'Disabled'
-    )
+    ws['C13'].value = 'Enabled' if 'validation' in change and change['validation'] else 'Disabled'
     disabled_enabled.add(ws['C13'])
     ws['A14'].value = 'Validation of inquiring form for Change Requests'
     ws['B14'].value = '-'
     ws['C14'].value = (
-        'Enabled' if 'inquiring_validation' in change and change['inquiring_validation'] else 'Disabled'
+        'Enabled'
+        if 'inquiring_validation' in change and change['inquiring_validation']
+        else 'Disabled'
     )
     disabled_enabled.add(ws['C14'])
 
     def _get_administrative_hold(capabilities):
         if 'hold' in capabilities['subscription'] and capabilities['subscription']['hold']:
             return 'Enabled'
         return 'Disabled'
@@ -867,19 +883,15 @@
     _setup_ws_header(ws, 'translations')
     ws.column_dimensions['F'].width = 30
     ws.column_dimensions['J'].width = 15
     ws.column_dimensions['K'].width = 15
 
     rql = R().context.instance_id.eq(product_id)
 
-    translations = (
-        client.ns('localization')
-        .translations
-        .filter(rql)
-    )
+    translations = client.ns('localization').translations.filter(rql)
     count = translations.count()
 
     action_validation = DataValidation(
         type='list',
         formula1='"-,delete,update,create"',
         allow_blank=False,
     )
@@ -921,22 +933,25 @@
             attr_ws[cell.coordinate].value = cell.value
             attr_ws[cell.coordinate].alignment = copy.copy(cell.alignment)
     alter_attributes_sheet(attr_ws)
     _setup_ws_header(attr_ws, '_attributes')
 
 
 def dump_product(  # noqa: CCR001
-    client, product_id, output_file, progress, output_path=None,
+    client,
+    product_id,
+    output_file,
+    progress,
+    output_path=None,
 ):
     output_file = validate_output_options(output_path, output_file, default_dir_name=product_id)
     media_path = os.path.join(os.path.dirname(output_file), 'media')
     if not os.path.exists(media_path):
         os.mkdir(media_path)
     try:
-
         product = client.products[product_id].get()
         wb = Workbook()
 
         _setup_locales_list(wb.active, client)
 
         connect_api_location = parse.urlparse(client.endpoint)
         media_location = f'{connect_api_location.scheme}://{connect_api_location.netloc}'
@@ -944,15 +959,19 @@
             wb.active,
             product,
             media_location,
             client,
             media_path,
         )
         _dump_capabilities(wb.create_sheet('Capabilities'), product, progress)
-        _dump_external_static_links(wb.create_sheet('Embedding Static Resources'), product, progress)
+        _dump_external_static_links(
+            wb.create_sheet('Embedding Static Resources'),
+            product,
+            progress,
+        )
         _dump_media(
             wb.create_sheet('Media'),
             client,
             product_id,
             media_location,
             media_path,
             progress,
```

### Comparing `connect_cli-27.6/connect/cli/plugins/product/sync/__init__.py` & `connect_cli-27.7/connect/cli/plugins/product/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/product/sync/actions.py` & `connect_cli-27.7/connect/cli/plugins/product/sync/actions.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 class ActionsSynchronizer(ProductSynchronizer):
     def __init__(self, client, progress, stats):
         super().__init__(client, progress)
         self._mstats = stats['Actions']
 
     def sync(self):  # noqa: CCR001
-        ws = self._wb["Actions"]
+        ws = self._wb['Actions']
         task = self._progress.add_task('Processing action', total=ws.max_row - 1)
         actions = self._get_actions()
         for row_idx in range(2, ws.max_row + 1):
             data = _RowData(*[ws.cell(row_idx, col_idx).value for col_idx in range(1, 10)])
             self._progress.update(
                 task,
                 description=f'Processing action {data.verbose_id or data.id}',
@@ -52,35 +52,39 @@
                     if e.status_code == 404:
                         self._mstats.deleted()
                         continue
                     self._mstats.error(str(e), row_idx)
                     continue
 
             payload = {
-                "action": data.id,
-                "type": "button",
-                "scope": data.scope,
-                "description": data.description,
-                "title": data.title,
+                'action': data.id,
+                'type': 'button',
+                'scope': data.scope,
+                'description': data.description,
+                'title': data.title,
             }
 
             if data.action == 'update':
                 try:
-                    action = self._client.products[self._product_id].actions[
-                        data.verbose_id
-                    ].update(payload)
+                    action = (
+                        self._client.products[self._product_id]
+                        .actions[data.verbose_id]
+                        .update(payload)
+                    )
                     self._update_sheet_row(ws, row_idx, action)
                     self._mstats.updated()
                 except Exception as e:
                     self._mstats.error(str(e), row_idx)
 
             if data.action == 'create':
                 try:
+
                     def _check_if_matches(data, x):
                         return x['action'] == data.id
+
                     original_action = list(filter(partial(_check_if_matches, data), actions))
                     if original_action:
                         self._updated_or_skipped(ws, row_idx, original_action[0], payload)
                         continue
                     payload['name'] = data.name
                     action = self._client.products[self._product_id].actions.create(payload)
                     self._update_sheet_row(ws, row_idx, action)
@@ -115,15 +119,15 @@
             return errors
         if data.action in ('delete', 'update') and not data.verbose_id:
             errors.append(
                 f'Verbose ID is required for {data.action} action.',
             )
             return errors
 
-        id_pattern = "^[A-Za-z0-9_-]*$"
+        id_pattern = '^[A-Za-z0-9_-]*$'
 
         if not bool(re.match(id_pattern, data.id)):
             errors.append(
                 f'Actions ID must contain only letters, numbers and `_`, provided {data.id}',
             )
             return errors
 
@@ -131,28 +135,24 @@
             errors.append(
                 f'Action scope must be one of `asset`, `tier1` or `tier2`. Provided {data.scope}',
             )
 
         return errors
 
     def _get_actions(self):
-        return (
-            self._client
-            .products[
-                self._product_id
-            ]
-            .actions
-        ).all()
+        return (self._client.products[self._product_id].actions).all()
 
     def _updated_or_skipped(self, ws, row_idx, original, payload):
         original_filter = {k: v for k, v in original.items() if k in payload.keys()}
         if original_filter == payload:
             self._update_sheet_row(ws, row_idx)
             self._mstats.skipped()
         else:
-            action = self._client.products[self._product_id].actions[
-                original["id"]
-            ].update(
-                payload,
+            action = (
+                self._client.products[self._product_id]
+                .actions[original['id']]
+                .update(
+                    payload,
+                )
             )
             self._update_sheet_row(ws, row_idx, action)
             self._mstats.updated()
```

### Comparing `connect_cli-27.6/connect/cli/plugins/product/sync/capabilities.py` & `connect_cli-27.7/connect/cli/plugins/product/sync/capabilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,28 +54,28 @@
                         else:
                             product['capabilities']['ppu'] = None
                     if data.capability == 'Pay-as-you-go dynamic items support':
                         if not product['capabilities'].get('ppu', False):
                             if data.value == 'Enabled':
                                 raise Exception(
                                     "Dynamic items support can't be enabled without Pay-as-you-go "
-                                    "support",
+                                    'support',
                                 )
                             update = False
                         else:
                             if data.value == 'Enabled':
                                 product['capabilities']['ppu']['dynamic'] = True
                             else:
                                 product['capabilities']['ppu']['dynamic'] = False
-                    if data.capability == "Pay-as-you-go future charges support":
+                    if data.capability == 'Pay-as-you-go future charges support':
                         if not product['capabilities'].get('ppu', False):
                             if data.value == 'Enabled':
                                 raise Exception(
                                     "Report of future charges can't be enabled without Pay-as-you-go "
-                                    "support",
+                                    'support',
                                 )
                             update = False
 
                         else:
                             if data.value == 'Enabled':
                                 product['capabilities']['ppu']['future'] = True
                             else:
@@ -118,73 +118,33 @@
                     if data.capability == 'Dynamic Validation of Tier Requests':
                         if data.value == 'Enabled':
                             product['capabilities']['tiers']['validation'] = True
                         else:
                             product['capabilities']['tiers']['validation'] = False
                     if data.capability == 'Editable Ordering Parameters in Change Request':
                         if data.value == 'Enabled':
-                            product[
-                                'capabilities'
-                            ][
-                                'subscription'
-                            ][
-                                'change'
-                            ][
+                            product['capabilities']['subscription']['change'][
                                 'editable_ordering_parameters'
                             ] = True
                         else:
-                            product[
-                                'capabilities'
-                            ][
-                                'subscription'
-                            ][
-                                'change'
-                            ][
+                            product['capabilities']['subscription']['change'][
                                 'editable_ordering_parameters'
                             ] = False
                     if data.capability == 'Validation of Draft Change Request':
                         if data.value == 'Enabled':
-                            product[
-                                'capabilities'
-                            ][
-                                'subscription'
-                            ][
-                                'change'
-                            ][
-                                'validation'
-                            ] = True
+                            product['capabilities']['subscription']['change']['validation'] = True
                         else:
-                            product[
-                                'capabilities'
-                            ][
-                                'subscription'
-                            ][
-                                'change'
-                            ][
-                                'validation'
-                            ] = False
+                            product['capabilities']['subscription']['change']['validation'] = False
                     if data.capability == 'Validation of inquiring form for Change Requests':
                         if data.value == 'Enabled':
-                            product[
-                                'capabilities'
-                            ][
-                                'subscription'
-                            ][
-                                'change'
-                            ][
+                            product['capabilities']['subscription']['change'][
                                 'inquiring_validation'
                             ] = True
                         else:
-                            product[
-                                'capabilities'
-                            ][
-                                'subscription'
-                            ][
-                                'change'
-                            ][
+                            product['capabilities']['subscription']['change'][
                                 'inquiring_validation'
                             ] = False
                     if update:
                         self._client.products[self._product_id].update(product)
                     self._mstats.updated()
 
                 except Exception as e:
@@ -196,20 +156,26 @@
         errors = []
         if data.capability not in CAPABILITIES:
             errors.append(
                 f'Capability {data.capability} is not valid capability',
             )
         if data.capability == 'Pay-as-you-go support and schema':
             if data.value not in (
-                'Disabled', 'QT', 'TR', 'PR', 'CR',
+                'Disabled',
+                'QT',
+                'TR',
+                'PR',
+                'CR',
             ):
                 errors.append(f'Schema {data.value} is not supported')
             return errors
         if data.capability == 'Reseller Authorization Level' and data.value not in (
-            'Disabled', 1, 2,
+            'Disabled',
+            1,
+            2,
         ):
             errors.append(f'{data.value } is not valid for Reseller Authorization level capability')
             return errors
         if (
             data.value not in ('Disabled', 'Enabled')
             and data.capability != 'Reseller Authorization Level'
         ):
```

### Comparing `connect_cli-27.6/connect/cli/plugins/product/sync/configuration_values.py` & `connect_cli-27.7/connect/cli/plugins/product/sync/configuration_values.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             )
         if errors:
             return errors
         if data.action == 'update' and (not data.value or data.value == '-'):
             errors.append(
                 'Value is required for update operation',
             )
-        id_pattern = "^[A-Za-z0-9_#-]*$"
+        id_pattern = '^[A-Za-z0-9_#-]*$'
 
         if not bool(re.match(id_pattern, data.id)):
             errors.append(
                 'ID is not properly formatted',
             )
             return errors
         if data.action not in ('-', 'update', 'delete'):
```

### Comparing `connect_cli-27.6/connect/cli/plugins/product/sync/general.py` & `connect_cli-27.7/connect/cli/plugins/product/sync/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,27 +48,26 @@
                 f'Product category {ws["B8"].value} is a not known category',
             )
         if ws['A9'] and ws['A9'].value != 'Product Icon file name':
             errors.append(
                 'A9 must be `Product Icon file name` and B9 contain the value',
             )
         if (ws['B9'] and ws['B9'].value) and not os.path.isfile(
-                os.path.join(
-                    self._media_path,
-                    'media',
-                    ws['B9'].value,
-                ),
+            os.path.join(
+                self._media_path,
+                'media',
+                ws['B9'].value,
+            ),
         ):
             errors.append(
                 f'File {ws["B9"].value} does not exist in the media folder',
             )
-        if (
-            (ws['A10'] and ws['A10'].value != 'Product Short Description')
-            or len(ws['B10'].value) > 512
-        ):
+        if (ws['A10'] and ws['A10'].value != 'Product Short Description') or len(
+            ws['B10'].value,
+        ) > 512:
             errors.append(
                 'Short description is mandatory and must be on B10, short description can not '
                 'exceed 512 characters',
             )
         if ws['A11'] and ws['A11'].value != 'Product Detailed Description':
             errors.append(
                 'Product detailed description is required',
@@ -107,15 +106,15 @@
         image_name = ws['B9'].value
         image_data = open(
             os.path.join(
                 self._media_path,
                 'media',
                 ws['B9'].value,
             ),
-            "rb",
+            'rb',
         )
         image_type, _ = guess_type(image_name)
         data = {
             'body': (None, json.dumps(product), 'application/json'),
             'icon': (image_name, image_data, image_type),
         }
         try:
```

### Comparing `connect_cli-27.6/connect/cli/plugins/product/sync/items.py` & `connect_cli-27.7/connect/cli/plugins/product/sync/items.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 class ItemSynchronizer(ProductSynchronizer):
     def __init__(self, client, progress, stats):
         self._units = list(client.ns('settings').units.all())
         self._mstats = stats['Items']
         super().__init__(client, progress)
 
     def sync(self):  # noqa: CCR001
-        ws = self._wb["Items"]
+        ws = self._wb['Items']
 
         task = self._progress.add_task('Processing item', total=ws.max_row - 1)
         for row_idx in range(2, ws.max_row + 1):
             data = _RowData(*[ws.cell(row_idx, col_idx).value for col_idx in range(1, 14)])
             self._progress.update(
                 task,
                 description=f'Processing item {data.id or data.mpn}',
@@ -53,20 +53,15 @@
             row_errors = self._validate_row(data)
             if row_errors:
                 self._mstats.error(row_errors, row_idx)
                 continue
 
             if data.action == 'create':
                 rql = R().mpn.eq(data.mpn)
-                item = (
-                    self._client.products[self._product_id]
-                    .items
-                    .filter(rql)
-                    .first()
-                )
+                item = self._client.products[self._product_id].items.filter(rql).first()
                 if item:
                     self._mstats.error(
                         f'Cannot create item: item with MPN `{data.mpn}`'
                         f' already exists with ID `{item["id"]}`.',
                         row_idx,
                     )
                     continue
@@ -160,16 +155,15 @@
             return [
                 f'the item `Commitment` must be one between '
                 f'{valid_commitment}, not `{row.commitment}`.',
             ]
 
         if row.type == 'ppu' and row.commitment != '-':
             return [
-                f'the commitment `{row.commitment}` '
-                'is invalid for `ppu` items.',
+                f'the commitment `{row.commitment}` ' 'is invalid for `ppu` items.',
             ]
 
         allowed_commitments = ALLOWED_COMMITMENTS.get(row.billing_period, [])
 
         if allowed_commitments and row.commitment not in allowed_commitments:
             valid_commitment = ', '.join([f'`{name}`' for name in allowed_commitments])
             return [
@@ -186,23 +180,21 @@
                 errors.append(
                     'one between the item `ID` or '
                     f'`MPN` is required for the `{row.action}` action.',
                 )
                 return errors
         if row.status == 'published' and row.action == 'delete':
             errors.append(
-                'the item status must be `draft` '
-                'for the `delete` action.',
+                'the item status must be `draft` for the `delete` action.',
             )
             return errors
 
         if row.action == 'create' and row.id:
             errors.append(
-                'the `ID` must not be specified '
-                'for the `create` action.',
+                'the `ID` must not be specified for the `create` action.',
             )
             return errors
 
         if not row.mpn:
             errors.append(
                 'the item `MPN` is required.',
             )
```

### Comparing `connect_cli-27.6/connect/cli/plugins/product/sync/media.py` & `connect_cli-27.7/connect/cli/plugins/product/sync/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
             image_data = open(
                 os.path.join(
                     self._media_path,
                     'media',
                     data.image_file,
                 ),
-                "rb",
+                'rb',
             )
             image_type, _ = guess_type(data.image_file)
             body = {
                 'type': data.type,
                 'position': str(data.position),
             }
 
@@ -81,16 +81,20 @@
             payload = {
                 'body': (None, json.dumps(body), 'application/json'),
                 'thumbnail': (data.image_file, image_data, image_type),
             }
 
             try:
                 if data.action == 'update':
-                    media = self._client.products[self._product_id].media[data.id].update(
-                        files=payload,
+                    media = (
+                        self._client.products[self._product_id]
+                        .media[data.id]
+                        .update(
+                            files=payload,
+                        )
                     )
                     self._update_sheet_row(ws, row_idx, media)
                     self._mstats.updated()
                 else:
                     media = self._client.products[self._product_id].media.create(
                         files=payload,
                     )
@@ -104,19 +108,19 @@
     def _update_sheet_row(ws, row_idx, media):
         ws.cell(row_idx, 1, value=media['position'])
         ws.cell(row_idx, 2, value=media['id'])
 
     def _validate_row(self, data):
         errors = []
         if not data.position or not str(data.position).isdigit() or int(data.position) > 8:
-            errors.append("Position is required and must be an integer between 1 and 8")
+            errors.append('Position is required and must be an integer between 1 and 8')
         elif data.action != 'create' and not data.id.startswith('PRDM-'):
             errors.append('ID does not seam to be valid.')
         elif not data.image_file:
-            errors.append("Image file is required")
+            errors.append('Image file is required')
         elif data.action not in ('-', 'create', 'update', 'delete'):
             errors.append(
                 f'Supported actions are `-`, `create`, `update` or `delete`. Provided {data.action}',
             )
         elif not data.type or data.type not in ('image', 'video'):
             errors.append(
                 f'Media can be either image or video type, provided {data.type}',
```

### Comparing `connect_cli-27.6/connect/cli/plugins/product/sync/params.py` & `connect_cli-27.7/connect/cli/plugins/product/sync/params.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,19 +26,19 @@
         self._param_type = None
         self._worksheet_name = None
         self.__stats = stats
         self._mstats = None
         super(ParamsSynchronizer, self).__init__(client, progress)
 
     def open(self, input_file, worksheet):
-        if worksheet == "Ordering Parameters":
+        if worksheet == 'Ordering Parameters':
             self._param_type = 'ordering'
-        elif worksheet == "Fulfillment Parameters":
+        elif worksheet == 'Fulfillment Parameters':
             self._param_type = 'fulfillment'
-        elif worksheet == "Configuration Parameters":
+        elif worksheet == 'Configuration Parameters':
             self._param_type = 'configuration'
         self._worksheet_name = worksheet
         self._mstats = self.__stats[self._worksheet_name]
         return super(ParamsSynchronizer, self).open(input_file, worksheet)
 
     def sync(self):  # noqa: CCR001
         ws = self._wb[self._worksheet_name]
@@ -85,18 +85,20 @@
 
             if data.action == 'update':
                 try:
                     original_param = self._get_original_param(data)
                     if original_param:
                         self._compare_param(original_param, data)
 
-                    param = self._client.products[self._product_id].parameters[
-                        data.verbose_id
-                    ].update(
-                        param_payload,
+                    param = (
+                        self._client.products[self._product_id]
+                        .parameters[data.verbose_id]
+                        .update(
+                            param_payload,
+                        )
                     )
                     self._update_sheet_row(ws, row_idx, param)
                     self._mstats.updated()
                 except Exception as e:
                     self._mstats.error(str(e), row_idx)
 
             if data.action == 'create':
@@ -142,52 +144,56 @@
             raise ParamSwitchNotSupported('Switching parameter type is not supported')
         if original['scope'] != data.scope:
             raise ParamSwitchNotSupported('switching scope is not supported')
         if original['phase'] != data.phase:
             raise ParamSwitchNotSupported('switching phase is not supported')
 
     def _validate_row(self, data):  # noqa: CCR001
-
         errors = []
         if not data.id:
             errors.append(
                 'Parameter must have an id',
             )
             return errors
-        id_pattern = "^[A-Za-z0-9_-]*$"
+        id_pattern = '^[A-Za-z0-9_-]*$'
 
         if not bool(re.match(id_pattern, data.id)):
             errors.append(
                 f'Parameter ID must contain only letters, numbers and `_`, provided {data.id}',
             )
 
         elif data.phase != self._param_type:
             errors.append(
                 f'Parameters of type {self._param_type} are only supported when processing '
                 f'{self._worksheet_name}. Has been provided {data.phase}.',
             )
         elif data.action in ('update', 'delete') and (
-                not data.verbose_id or not data.verbose_id.startswith('PRM-')
+            not data.verbose_id or not data.verbose_id.startswith('PRM-')
         ):
             errors.append(
                 'Verbose ID is required on update and delete actions.',
             )
         elif data.type not in PARAM_TYPES:
             errors.append(
                 f'Parameter type {data.type} is not one of the supported ones:'
                 f'{",".join(PARAM_TYPES)}',
             )
         elif self._param_type in ('ordering', 'fulfillment') and data.scope not in (
-            'asset', 'tier1', 'tier2',
+            'asset',
+            'tier1',
+            'tier2',
         ):
             errors.append(
                 f'Only asset, tier1 and tier2 scopes are supported for {self._worksheet_name}',
             )
         elif self._param_type == 'configuration' and data.scope not in (
-            'item', 'item_marketplace', 'marketplace', 'product',
+            'item',
+            'item_marketplace',
+            'marketplace',
+            'product',
         ):
             errors.append(
                 'Only item, item_marketplace, marketplace and product scopes are supported for '
                 f'{self._worksheet_name}',
             )
         elif data.required not in (True, 'True', '-'):
             errors.append(
@@ -216,27 +222,25 @@
 
     def _get_original_param(self, data):
         filter_kwargs = {}
         if data.verbose_id:
             filter_kwargs['id'] = data.verbose_id
         else:
             filter_kwargs['name'] = data.id
-        return (
-            self._client.products[self._product_id].parameters
-            .filter(**filter_kwargs)
-            .first()
-        )
+        return self._client.products[self._product_id].parameters.filter(**filter_kwargs).first()
 
     def _updated_or_skipped(self, ws, row_idx, original, payload):
         original_filter = {k: v for k, v in original.items() if k in payload.keys()}
 
         if original_filter == payload:
             self._update_sheet_row(ws, row_idx)
             self._mstats.skipped()
         else:
-            param = self._client.products[self._product_id].parameters[
-                original["id"]
-            ].update(
-                payload,
+            param = (
+                self._client.products[self._product_id]
+                .parameters[original['id']]
+                .update(
+                    payload,
+                )
             )
             self._update_sheet_row(ws, row_idx, param)
             self._mstats.updated()
```

### Comparing `connect_cli-27.6/connect/cli/plugins/product/sync/static_resources.py` & `connect_cli-27.7/connect/cli/plugins/product/sync/static_resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,24 +39,24 @@
                 continue
             if data.action == 'delete':
                 self._mstats.deleted()
                 continue
             if data.type == 'Download':
                 download.append(
                     {
-                        "title": data.title,
-                        "url": data.url,
-                        "visible_for": "admin",
+                        'title': data.title,
+                        'url': data.url,
+                        'visible_for': 'admin',
                     },
                 )
-            if data.type == "Documentation":
+            if data.type == 'Documentation':
                 documentation.append(
                     {
-                        "title": data.title,
-                        "url": data.url,
+                        'title': data.title,
+                        'url': data.url,
                     },
                 )
             if data.action == '-':
                 self._mstats.skipped()
             else:
                 self._mstats.created()
```

### Comparing `connect_cli-27.6/connect/cli/plugins/product/sync/templates.py` & `connect_cli-27.7/connect/cli/plugins/product/sync/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         self._action_handlers = {
             'create': self._action_create,
             'update': self._action_update,
             'delete': self._action_delete,
         }
 
     def sync(self):
-        ws = self._wb["Templates"]
+        ws = self._wb['Templates']
 
         task = self._progress.add_task('Processing Template', total=ws.max_row - 1)
         for row_idx in range(2, ws.max_row + 1):
             data = _RowData(*[ws.cell(row_idx, col_idx).value for col_idx in range(1, 9)])
             self._progress.update(
                 task,
                 description=f'Processing Template {data.id or data.title}',
@@ -99,18 +99,20 @@
     def _row_to_payload(data):
         template_payload = {
             'name': data.title,
             'scope': data.scope,
             'body': data.content,
         }
         if data.scope == 'asset':
-            template_payload.update({
-                'title': data.title,
-                'type': data.type,
-            })
+            template_payload.update(
+                {
+                    'title': data.title,
+                    'type': data.type,
+                },
+            )
         return template_payload
 
     @staticmethod
     def _update_sheet_row(ws, row_idx, template):
         ws.cell(row_idx, 1, value=template['id'])
         ws.cell(row_idx, 7, value=template['events']['created']['at'])
         ws.cell(row_idx, 8, value=template['events'].get('updated', {}).get('at'))
```

### Comparing `connect_cli-27.6/connect/cli/plugins/product/utils.py` & `connect_cli-27.7/connect/cli/plugins/product/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import json
 from copy import deepcopy
 
 
 def cleanup_product_for_update(product):
     del product['icon']
     ppu = product['capabilities'].get('ppu', False)
-    if product['capabilities']['subscription'] and 'schema' in product['capabilities']['subscription']:
+    if (
+        product['capabilities']['subscription']
+        and 'schema' in product['capabilities']['subscription']
+    ):
         del product['capabilities']['subscription']['schema']
     if ppu and 'predictive' in ppu:
         del product['capabilities']['ppu']['predictive']
     return product
 
 
 def get_json_object_for_param(original_param):
```

### Comparing `connect_cli-27.6/connect/cli/plugins/project/commands.py` & `connect_cli-27.7/connect/cli/plugins/project/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,32 +5,33 @@
 import click
 
 from connect.cli.core import group
 from connect.cli.core.config import pass_config
 from connect.cli.plugins.project.extension.helpers import (
     bootstrap_extension_project,
     bump_runner_extension_project,
+    deploy_extension_project,
     validate_extension_project,
 )
 from connect.cli.plugins.project.report.helpers import (
     add_report,
     bootstrap_report_project,
     validate_report_project,
 )
 
 
 class Mutex(click.Option):
     def __init__(self, *args, **kwargs):
-        self.conflict_with: list = kwargs.pop("conflict_with")
+        self.conflict_with: list = kwargs.pop('conflict_with')
 
         assert self.conflict_with, "'conflict_with' parameter required"
 
-        help_str = kwargs.get("help", "")
+        help_str = kwargs.get('help', '')
         help_str += f' This option is mutually exclusive with {", ".join(self.conflict_with)}.'
-        kwargs["help"] = help_str.strip()
+        kwargs['help'] = help_str.strip()
         super(Mutex, self).__init__(*args, **kwargs)
 
     def handle_parse_result(self, ctx, opts, args):
         current_opt: bool = self.name in opts
         for mutex_opt in self.conflict_with:
             if mutex_opt in opts:
                 if current_opt:
@@ -57,56 +58,61 @@
 
 
 @grp_project_report.command(
     name='bootstrap',
     short_help='Bootstrap new report project.',
 )
 @click.option(
-    '--output-dir', '-o',
+    '--output-dir',
+    '-o',
     default=os.getcwd(),
     type=click.Path(exists=False, file_okay=False, dir_okay=True),
     required=True,
     help='Directory where the new report project will be created.',
 )
 @click.option(
-    '--force-overwrite', '-f',
+    '--force-overwrite',
+    '-f',
     is_flag=True,
     help='Overwrite the destination project directory if exists.',
     default=False,
 )
 def cmd_bootstrap_report_project(output_dir, force_overwrite):
     bootstrap_report_project(output_dir, force_overwrite)
 
 
 @grp_project_report.command(
     name='validate',
     short_help='Validate given report project.',
 )
 @click.option(
-    '--project-dir', '-p',
+    '--project-dir',
+    '-p',
     required=True,
     type=click.Path(exists=True, file_okay=False, dir_okay=True),
     help='Project directory.',
 )
 def cmd_validate_report_project(project_dir):
     validate_report_project(project_dir)
 
 
 @grp_project_report.command(
     name='add',
     short_help='Add new report to the given project.',
 )
 @click.option(
-    '--project-dir', '-p',
+    '--project-dir',
+    '-p',
     required=True,
     type=click.Path(exists=True, file_okay=False, dir_okay=True),
     help='Project directory.',
 )
 @click.option(
-    '--package-name', '-n',
+    '--package-name',
+    '-n',
     default='reports',
     help='Package directory.',
 )
 def cmd_add_report(project_dir, package_name):
     add_report(project_dir, package_name)
 
 
@@ -120,47 +126,55 @@
 
 
 @grp_project_extension.command(
     name='bootstrap',
     short_help='Bootstrap new extension project.',
 )
 @click.option(
-    '--output-dir', '-o',
+    '--output-dir',
+    '-o',
     default=os.getcwd(),
     type=click.Path(exists=False, file_okay=False, dir_okay=True),
     required=False,
     help='Directory where the new extension project will be created.',
 )
 @click.option(
-    '--force-overwrite', '-f',
+    '--force-overwrite',
+    '-f',
     is_flag=True,
     help='Overwrite the destination project directory if exists.',
     default=False,
 )
 @click.option(
-    '--save-answers', '-s',
+    '--save-answers',
+    '-s',
     default=None,
     type=click.Path(exists=False, file_okay=True, dir_okay=False),
     required=False,
     help='Path to JSON file where to save wizard answers.',
     cls=Mutex,
     conflict_with=['load_answers'],
 )
 @click.option(
-    '--load-answers', '-l',
+    '--load-answers',
+    '-l',
     default=None,
     type=click.Path(exists=True, file_okay=True, dir_okay=False),
     required=False,
     help='Path to JSON file from where load wizard answers.',
     cls=Mutex,
     conflict_with=['save_answers'],
 )
 @pass_config
 def cmd_bootstrap_extension_project(
-        config, output_dir, force_overwrite, save_answers, load_answers,
+    config,
+    output_dir,
+    force_overwrite,
+    save_answers,
+    load_answers,
 ):
     bootstrap_extension_project(
         config,
         output_dir,
         force_overwrite,
         save_answers,
         load_answers,
@@ -184,18 +198,37 @@
 
 
 @grp_project_extension.command(
     name='bump',
     short_help='Update runner version to the latest one.',
 )
 @click.option(
-    '--project-dir', '-p',
+    '--project-dir',
+    '-p',
     required=True,
     type=click.Path(exists=True, file_okay=False, dir_okay=True),
     help='Project directory.',
 )
 def cmd_bump_extension_project(project_dir):
     bump_runner_extension_project(project_dir)
 
 
+@grp_project_extension.command(
+    name='deploy',
+    short_help='Deploy extension.',
+)
+@click.argument('repo', metavar='repo', nargs=1, required=True)
+@click.option(
+    '--tag',
+    '-t',
+    required=False,
+    default=None,
+    type=str,
+    help='Repository tag.',
+)
+@pass_config
+def cmd_deploy_extension(config, repo, tag):
+    deploy_extension_project(config, repo, tag)
+
+
 def get_group():
     return grp_project
```

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/helpers.py` & `connect_cli-27.7/connect/cli/plugins/project/extension/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import collections
 import json
 import os
 
 import yaml
 from click.exceptions import ClickException
+from connect.eaas.core.deployment.extension import deploy_extension
 from connect.eaas.core.validation.validators import get_validators
 from interrogatio.core.dialog import dialogus
 
 from connect.cli import get_version
 from connect.cli.core.terminal import console
 from connect.cli.plugins.project.extension.utils import (
     get_event_definitions,
@@ -21,15 +22,19 @@
 )
 from connect.cli.plugins.project.renderer import BoilerplateRenderer
 from connect.cli.plugins.project.utils import show_validation_result_table
 from connect.cli.plugins.project.validators import ProjectDirValidator
 
 
 def bootstrap_extension_project(  # noqa: CCR001
-        config, output_dir, overwrite, save_answers, load_answers,
+    config,
+    output_dir,
+    overwrite,
+    save_answers,
+    load_answers,
 ):
     console.secho('Bootstraping extension project...\n', fg='blue')
 
     if save_answers and os.path.exists(save_answers):
         raise ClickException(f'Answers cannot be saved, because {save_answers} already exists.')
 
     statuses_by_event = collections.defaultdict(lambda: collections.defaultdict())
@@ -98,44 +103,50 @@
 
     if answers['use_github_actions'] == 'n':
         exclude.extend(['.github', '.github/**/*'])
 
     application_types = answers.get('application_types', [])
 
     if answers.get('webapp_supports_ui') != 'y':
-        exclude.extend([
-            os.path.join('${package_name}', 'static', '.gitkeep'),
-            'ui',
-            'ui/**/*',
-            'package.json.j2',
-            'webpack.config.js.j2',
-            '__mocks__',
-            '__mocks__/*',
-            '.eslintrc.yaml.j2',
-            'babel.config.json.j2',
-            'jest.config.js.j2',
-        ])
+        exclude.extend(
+            [
+                os.path.join('${package_name}', 'static', '.gitkeep'),
+                'ui',
+                'ui/**/*',
+                'package.json.j2',
+                'webpack.config.js.j2',
+                '__mocks__',
+                '__mocks__/*',
+                '.eslintrc.yaml.j2',
+                'babel.config.json.j2',
+                'jest.config.js.j2',
+            ],
+        )
 
     elif 'tfnapp' not in application_types:
-        exclude.extend([
-            'ui/pages/transformations',
-            'ui/pages/transformations/*',
-            'ui/src/pages/transformations',
-            'ui/src/pages/transformations/*',
-            'ui/styles/manual.css.j2',
-        ])
+        exclude.extend(
+            [
+                'ui/pages/transformations',
+                'ui/pages/transformations/*',
+                'ui/src/pages/transformations',
+                'ui/src/pages/transformations/*',
+                'ui/styles/manual.css.j2',
+            ],
+        )
     else:
-        exclude.extend([
-            'ui/pages/index.html.j2',
-            'ui/pages/settings.html.j2',
-            'ui/src/pages/index.js.j2',
-            'ui/src/pages/settings.js.j2',
-            'ui/tests/pages.spec.js.j2',
-            'ui/tests/utils.spec.js.j2',
-        ])
+        exclude.extend(
+            [
+                'ui/pages/index.html.j2',
+                'ui/pages/settings.html.j2',
+                'ui/src/pages/index.js.j2',
+                'ui/src/pages/settings.js.j2',
+                'ui/tests/pages.spec.js.j2',
+                'ui/tests/utils.spec.js.j2',
+            ],
+        )
 
     for app_type in ['anvil', 'events', 'webapp', 'tfnapp']:
         if app_type not in application_types:
             exclude.append(
                 os.path.join(
                     '${package_name}',
                     f'{app_type}.py.j2',
@@ -194,15 +205,18 @@
         console.markdown('# Extension validation results')
         show_validation_result_table(validation_items)
         console.secho(
             f'Warning/errors have been found while validating the Extension Project {project_dir}.',
             fg='yellow',
         )
     else:
-        console.secho(f'Extension Project {project_dir} has been successfully validated.', fg='green')
+        console.secho(
+            f'Extension Project {project_dir} has been successfully validated.',
+            fg='green',
+        )
 
 
 def _update_docker_file_runner_from(dockerfile: str, latest_version: str):
     to_be_replaced = False
     last_runner = f'cloudblueconnect/connect-extension-runner:{latest_version}'
     lines = []
     with open(dockerfile, 'r') as f:
@@ -230,15 +244,17 @@
     console.secho(f'Bumping runner version on project {project_dir}...\n', fg='blue')
 
     updated_files = set()
     latest_version = get_pypi_runner_version()
     latest_runner_version = f'cloudblueconnect/connect-extension-runner:{latest_version}'
     docker_compose_file = os.path.join(project_dir, 'docker-compose.yml')
     if not os.path.isfile(docker_compose_file):
-        raise ClickException(f'Mandatory `docker-compose.yml` file on directory `{project_dir}` is missing.')
+        raise ClickException(
+            f'Mandatory `docker-compose.yml` file on directory `{project_dir}` is missing.',
+        )
     try:
         with open(docker_compose_file, 'r') as file_reader:
             data = yaml.load(file_reader, Loader=yaml.FullLoader)
             for service in data['services']:
                 if (
                     'image' in data['services'][service]
                     and data['services'][service]['image'].startswith(
@@ -255,17 +271,17 @@
                     dockerfile = data['services'][service]['build'].get('dockerfile', 'Dockerfile')
                     dockerfile_path = os.path.join(project_dir, dockerfile)
                     if not os.path.isfile(dockerfile_path):
                         raise ClickException(
                             f'The expected dockerfile `{dockerfile_path}` specified in '
                             f'{docker_compose_file} is missing.',
                         )
-                    if (
-                        dockerfile_path not in updated_files
-                        and _update_docker_file_runner_from(dockerfile_path, latest_version)
+                    if dockerfile_path not in updated_files and _update_docker_file_runner_from(
+                        dockerfile_path,
+                        latest_version,
                     ):
                         updated_files.add(dockerfile_path)
         with open(docker_compose_file, 'w') as file_writer:
             yaml.dump(data, file_writer, sort_keys=False)
     except yaml.YAMLError as error:
         raise ClickException(
             '`docker_compose.yml` file is not properly formatted. Please review it.\n'
@@ -276,7 +292,16 @@
         console.secho(
             f'Runner version has been successfully updated to {latest_version}. The following '
             f'files have been updated:\n{",".join(updated_files)}',
             fg='green',
         )
     else:
         console.secho(f'Nothing to update to {latest_version}', fg='yellow')
+
+
+def deploy_extension_project(config, repo_url, tag):
+    deploy_extension(
+        repo=repo_url,
+        client=config.active.client,
+        log=console.secho,
+        tag=tag,
+    )
```

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/anvil.py.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/anvil.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/events.py.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/events.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/schemas.py.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/schemas.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/tfnapp.py.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/tfnapp.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/webapp.py.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/${package_name}/webapp.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.${project_slug}_dev.env.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.${project_slug}_dev.env.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.eslintrc.yaml.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.eslintrc.yaml.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.github/workflows/test.yml.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/.github/workflows/test.yml.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/HOWTO.md.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/HOWTO.md.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/LICENSE.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/LICENSE.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/docker-compose.yml.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/jest.config.js.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/jest.config.js.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/package.json.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/package.json.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/pyproject.toml.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/conftest.py.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/conftest.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_anvil.py.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_anvil.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_events.py.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_events.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_tfnapp.py.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_tfnapp.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_webapp.py.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/tests/test_webapp.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/images/mkp.svg.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/images/mkp.svg.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/index.html.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/index.html.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/settings.html.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/settings.html.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/transformations/manual.html.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/pages/transformations/manual.html.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/components.js.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/components.js.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages.js.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/pages.js.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/utils.js.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/src/utils.js.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/index.css.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/index.css.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/manual.css.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/styles/manual.css.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/components.spec.js.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/components.spec.js.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/pages.spec.js.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/pages.spec.js.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/utils.spec.js.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/ui/tests/utils.spec.js.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/webpack.config.js.j2` & `connect_cli-27.7/connect/cli/plugins/project/extension/templates/bootstrap/${project_slug}/webpack.config.js.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/utils.py` & `connect_cli-27.7/connect/cli/plugins/project/extension/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 )
 
 
 def get_event_definitions(config):
     try:
         return list(config.active.client('devops').event_definitions.all())
     except ClientError as err:
-        raise ClickException(f"Error getting event definitions: {str(err)}")
+        raise ClickException(f'Error getting event definitions: {str(err)}')
 
 
 def get_pypi_runner_version():
     res = requests.get(PYPI_EXTENSION_RUNNER_URL)
     if res.status_code != 200:
         raise ClickException(
             f'We can not retrieve the current connect-extension-runner version from {PYPI_EXTENSION_RUNNER_URL}.',
@@ -103,18 +103,17 @@
 
 
 def check_event_type_applicable(event_type, context):
     return event_type not in context.get('event_types', [])
 
 
 def check_webapp_feature_not_selected(context):
-    return (
-        'webapp' not in context.get('application_types', [])
-        or context.get('extension_type') not in ('multiaccount', 'transformations')
-    )
+    return 'webapp' not in context.get('application_types', []) or context.get(
+        'extension_type',
+    ) not in ('multiaccount', 'transformations')
 
 
 def check_eventsapp_feature_not_selected(context):
     return 'events' not in context.get('application_types', [])
 
 
 def initialize_git_repository(tmp_dir, context):
```

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/validators.py` & `connect_cli-27.7/connect/cli/plugins/project/extension/validators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 from interrogatio.core.exceptions import ValidationError
 from interrogatio.validators import Validator
 
 
 class AppTypesValidator(Validator):
     def validate(self, value, context=None):
-        if (
-            context.get('extension_type') == 'transformations'
-            and (
-                'webapp' not in value
-                or 'tfnapp' not in value
-            )
+        if context.get('extension_type') == 'transformations' and (
+            'webapp' not in value or 'tfnapp' not in value
         ):
             raise ValidationError(
                 'Web Application and Transformations Application '
                 'are mandatory for Commerce type extensions.',
             )
 
 
 class UISupportValidator(Validator):
     def validate(self, value, context=None):
-        if (
-            context.get('extension_type') == 'transformations'
-            and value != 'y'
-        ):
+        if context.get('extension_type') == 'transformations' and value != 'y':
             raise ValidationError(
-                'Web Application UI support '
-                'is mandatory for Commerce type extensions.',
+                'Web Application UI support is mandatory for Commerce type extensions.',
             )
```

### Comparing `connect_cli-27.6/connect/cli/plugins/project/extension/wizard.py` & `connect_cli-27.7/connect/cli/plugins/project/extension/wizard.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     'to start writing your code.\n\n'
     'For more information please visit https://connect.cloudblue.com/community/modules/devops\n'
     'Have a nice trip!\n'
 )
 
 
 def get_summary(data):  # pragma: no cover
-
     def value(variable_name, formatted=False):
         if not data.get(variable_name):
             return ''
 
         data_value = data[variable_name]['formatted_value' if formatted else 'value']
 
         return data_value or '-'
@@ -269,29 +268,27 @@
 
     event_questions = [
         {
             'name': 'background',
             'label': 'Extension: Background events',
             'type': 'selectmany',
             'description': (
-                'What types of background'
-                'events do you want your Extension to process?'
+                'What types of background events do you want your Extension to process?'
             ),
             'values': partial(get_background_events, definitions),
             'formatting_template': '${label}',
             'disabled': partial(check_event_type_applicable, 'background'),
             'validators': (RequiredValidator(message='Please, select at least one option.'),),
         },
         {
             'name': 'interactive',
             'label': 'Extension: Interactive events',
             'type': 'selectmany',
             'description': (
-                'What types of interactive'
-                'events do you want your Extension to process?'
+                'What types of interactive events do you want your Extension to process?'
             ),
             'values': partial(get_interactive_events, definitions),
             'disabled': partial(check_event_type_applicable, 'interactive'),
             'formatting_template': '${label}',
             'validators': (RequiredValidator(message='Please, select at least one option.'),),
         },
     ]
```

### Comparing `connect_cli-27.6/connect/cli/plugins/project/renderer.py` & `connect_cli-27.7/connect/cli/plugins/project/renderer.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from jinja2 import Environment, FileSystemLoader, select_autoescape
 
 from connect.cli.core.terminal import console
 from connect.cli.plugins.project.utils import purge_dir
 
 
 class BoilerplateRenderer:
-
     def __init__(
         self,
         context,
         template_folder,
         output_dir,
         overwrite=False,
         pre_render=None,
@@ -53,40 +52,51 @@
         )
 
     @staticmethod
     def _get_excluded_patterns(template_dir, exclude):
         excludes = []
         for pattern in exclude:
             excludes.extend(
-                [
-                    str(p) for p in Path(os.path.join(template_dir, '${project_slug}')).glob(pattern)
-                ],
+                [str(p) for p in Path(os.path.join(template_dir, '${project_slug}')).glob(pattern)],
             )
         return excludes
 
     @staticmethod
-    def _validate_args(context, template_folder, output_dir, overwrite, pre_render, post_render, exclude):
+    def _validate_args(
+        context,
+        template_folder,
+        output_dir,
+        overwrite,
+        pre_render,
+        post_render,
+        exclude,
+    ):
         if not isinstance(context, dict):
             raise TypeError('The parameter context is invalid, it must be a dict.')
         if not isinstance(template_folder, str) or not os.path.exists(template_folder):
-            raise TypeError('The parameter template_folder is invalid, it must be a valid path string.')
+            raise TypeError(
+                'The parameter template_folder is invalid, it must be a valid path string.',
+            )
         if not isinstance(output_dir, str):
             raise TypeError('The parameter output_dir is invalid, it must be a valid path string.')
         if not isinstance(overwrite, bool):
             raise TypeError('The parameter overwrite is invalid, it must be bool type.')
         if pre_render and not callable(pre_render):
             raise TypeError('The parameter pre_render is invalid, it must be callable.')
         if post_render and not callable(post_render):
             raise TypeError('The parameter post_render is invalid, it must be callable.')
         if exclude and not isinstance(exclude, list):
             raise TypeError('The parameter exclude is invalid, it must be a list.')
 
     def _create_directories(self, output_dir):
         for element in Path(self.template_folder).rglob('*'):
-            directory = os.path.join(output_dir, os.path.relpath(str(element), self.template_folder))
+            directory = os.path.join(
+                output_dir,
+                os.path.relpath(str(element), self.template_folder),
+            )
             directory = Template(directory).safe_substitute(self.context)
             if element.is_dir() and not fnmatch.filter(self.excluded_patterns, element):
                 os.makedirs(directory, exist_ok=True)
                 console.print(
                     f'Folder {directory.replace(output_dir, "")}'
                     ' created [bold green]\u2713[/bold green]',
                 )
@@ -123,15 +133,18 @@
     def _render_template(self, template_name, destination):
         evaluated_template_path = Template(
             str(template_name),
         ).safe_substitute(
             self.context,
         )
 
-        if not fnmatch.filter(self.excluded_patterns, os.path.join(self.template_folder, template_name)):
+        if not fnmatch.filter(
+            self.excluded_patterns,
+            os.path.join(self.template_folder, template_name),
+        ):
             file_destination = os.path.join(
                 destination,
                 evaluated_template_path[:-3],
             )
             template = self.env.get_template(template_name)
             content = template.render(self.context)
             with open(file_destination, 'w') as outstream:
```

### Comparing `connect_cli-27.6/connect/cli/plugins/project/report/helpers.py` & `connect_cli-27.7/connect/cli/plugins/project/report/helpers.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/entrypoint.py.j2` & `connect_cli-27.7/connect/cli/plugins/project/report/templates/add/${initial_report_slug}/entrypoint.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/entrypoint.py.j2` & `connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/entrypoint.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/pdf/template.html.j2.j2` & `connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/${package_name}/${initial_report_slug}/templates/pdf/template.html.j2.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.github/workflows/build.yml.j2` & `connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/.github/workflows/build.yml.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/LICENSE.j2` & `connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/LICENSE.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/pyproject.toml.j2` & `connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/reports.json.j2` & `connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/reports.json.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/conftest.py.j2` & `connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/conftest.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/test_${project_slug}.py.j2` & `connect_cli-27.7/connect/cli/plugins/project/report/templates/bootstrap/${project_slug}/tests/test_${project_slug}.py.j2`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/project/report/validations.py` & `connect_cli-27.7/connect/cli/plugins/project/report/validations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 #  Copyright © 2022 CloudBlue. All rights reserved.
 
 import importlib
 import inspect
 import json
 import os
 import sys
```

### Comparing `connect_cli-27.6/connect/cli/plugins/project/report/wizard.py` & `connect_cli-27.7/connect/cli/plugins/project/report/wizard.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,14 +224,17 @@
 REPORT_SUMMARY = """<b><blue>Report</blue></b>
     <b>Name:</b> ${initial_report_name}
     <b>Description:</b> ${initial_report_description}
     <b>Output format:</b> ${initial_report_renderer}
     <b>Use Asyncio:</b> ${use_asyncio}
 """
 
-BOOTSTRAP_SUMMARY = """<b><blue>Project</blue></b>
+BOOTSTRAP_SUMMARY = (
+    """<b><blue>Project</blue></b>
     <b>Project Name:</b> ${project_name} - <b>Package Name:</b> ${package_name}
     <b>Description:</b> ${description}
     <b>Author:</b> ${author}
     <b>Version:</b> ${version} - <b>License:</b> ${license}
     <b>Use Github Actions:</b> ${use_github_actions}
-""" + REPORT_SUMMARY
+"""
+    + REPORT_SUMMARY
+)
```

### Comparing `connect_cli-27.6/connect/cli/plugins/project/utils.py` & `connect_cli-27.7/connect/cli/plugins/project/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 
 def purge_dir(dir):
     if os.path.isdir(dir):
         shutil.rmtree(dir, onerror=force_delete)
 
 
 def slugify(name):
-    return name.lower().strip().replace(' ', '_').replace('-', '_').replace('.', '_').replace(',', '')
+    return (
+        name.lower().strip().replace(' ', '_').replace('-', '_').replace('.', '_').replace(',', '')
+    )
 
 
 def show_validation_result_table(validation_items):
     for item in validation_items:
         table = Table(
             box=box.ROUNDED,
             show_header=False,
@@ -42,10 +44,12 @@
                 item.code,
                 'python3',
                 theme='ansi_light',
                 dedent=True,
                 line_numbers=True,
                 start_line=item.start_line,
                 highlight_lines={item.lineno},
-            ) if item.code else '-',
+            )
+            if item.code
+            else '-',
         )
         console.print(table)
```

### Comparing `connect_cli-27.6/connect/cli/plugins/project/validators.py` & `connect_cli-27.7/connect/cli/plugins/project/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,24 +5,22 @@
 
 import toml
 from interrogatio.core.exceptions import ValidationError
 from interrogatio.validators import Validator
 
 
 class PythonIdentifierValidator(Validator):
-
     def validate(self, value, context=None):
         if not value:
             return
         if not value.isidentifier():
             raise ValidationError('Introduced data is not a valid Python identifier')
 
 
 class ProjectDirValidator(Validator):
-
     def __init__(
         self,
         output_dir,
         message='The root folder for your project already exist.',
     ):
         super().__init__(message=message)
         self.output_dir = output_dir
@@ -61,15 +59,15 @@
 
     for idx, line in enumerate(source_lines[0]):  # pragma: no branchs
         if pattern in line:
             lineno += idx
             break
 
     if inspect.ismodule(obj):
-        code = ''.join(code.splitlines(keepends=True)[0:lineno + 3])
+        code = ''.join(code.splitlines(keepends=True)[0 : lineno + 3])
 
     return {
         'file': file,
         'start_line': start_line,
         'lineno': lineno,
         'code': code,
     }
```

### Comparing `connect_cli-27.6/connect/cli/plugins/report/commands.py` & `connect_cli-27.7/connect/cli/plugins/report/commands.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/report/helpers.py` & `connect_cli-27.7/connect/cli/plugins/report/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,20 +123,20 @@
 
 def execute_report(config, reports_dir, report_id, output_file, output_format):
     repo = load_repo(reports_dir)
     report = get_report_by_id(repo, report_id)
 
     if config.active.is_vendor() and 'vendor' not in report.audience:
         raise ClickException(
-            "This report is not expected to be executed on vendor accounts",
+            'This report is not expected to be executed on vendor accounts',
         )
 
     if config.active.is_provider() and 'provider' not in report.audience:
         raise ClickException(
-            "This report is not expected to be executed on provider accounts",
+            'This report is not expected to be executed on provider accounts',
         )
 
     available_renderers = [r.id for r in report.renderers]
 
     if output_format and output_format not in available_renderers:
         raise ClickException(
             f'The format {output_format} is not available for report {report_id}',
```

### Comparing `connect_cli-27.6/connect/cli/plugins/report/utils.py` & `connect_cli-27.7/connect/cli/plugins/report/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 
 
 def get_renderer_by_id(report, renderer_id):
     try:
         return next(filter(lambda r: r.id == renderer_id, report.renderers))
     except StopIteration:
         raise ClickException(
-            f'The output format `{renderer_id}` is not available for report {report.local_id}.')
+            f'The output format `{renderer_id}` is not available for report {report.local_id}.',
+        )
 
 
 def get_report_entrypoint(report):
     sys.path.append(report.root_path)
     module_name, func_name = report.entrypoint.rsplit('.', 1)
     try:
         module = import_module(module_name)
```

### Comparing `connect_cli-27.6/connect/cli/plugins/report/wizard.py` & `connect_cli-27.7/connect/cli/plugins/report/wizard.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,37 +13,37 @@
     Validator,
 )
 
 from connect.cli.plugins.report.utils import convert_to_utc_input
 
 
 class ObjectValidator(Validator):
-
     def validate(self, value, context=None):
         if not value:
             return
         try:
             json.loads(value)
         except ValueError:
             raise ValidationError('Introduced data is not a valid json object')
 
 
 def required_validator(param, validators=None):
     if not validators:
         validators = []
 
     if param.get('required', False):
-        validators.append(RequiredValidator(
-            message='Please select at least one value',
-        ))
+        validators.append(
+            RequiredValidator(
+                message='Please select at least one value',
+            ),
+        )
     return validators
 
 
 def single_line(param):
-
     return {
         'name': param['id'],
         'label': param['name'],
         'type': 'input',
         'description': f'{param["description"]}',
         'validators': required_validator(param),
     }
@@ -80,18 +80,19 @@
         'type': 'daterange',
         'description': description,
         'validators': required_validator(param, [DateTimeRangeValidator()]),
     }
 
 
 def date(param):
-
-    date_validator = [DateTimeValidator(
-        format_pattern='%Y-%m-%d',
-    )]
+    date_validator = [
+        DateTimeValidator(
+            format_pattern='%Y-%m-%d',
+        ),
+    ]
 
     return {
         'name': param['id'],
         'label': param['name'],
         'type': 'date',
         'description': f'{param["description"]}:',
         'validators': required_validator(param, date_validator),
@@ -101,18 +102,15 @@
 def marketplace_list(config, client, param):
     marketplaces = client.marketplaces.all()
     return {
         'name': param['id'],
         'label': param['name'],
         'type': 'selectmany',
         'description': f'{param["description"]} ({param["id"]})',
-        'values': [
-            (m['id'], f'{m["name"]} ({m["id"]})')
-            for m in marketplaces
-        ],
+        'values': [(m['id'], f'{m["name"]} ({m["id"]})') for m in marketplaces],
         'formatting_template': '${label}',
         'validators': required_validator(param),
     }
 
 
 def hub_list(config, client, param):
     marketplaces = client.marketplaces.all()
@@ -126,18 +124,15 @@
                     hubs.append(hub['hub'])
 
     return {
         'name': param['id'],
         'label': param['name'],
         'type': 'selectmany',
         'description': f'{param["description"]}',
-        'values': [
-            (h['id'], f'{h["name"]} ({h["id"]})')
-            for h in hubs
-        ],
+        'values': [(h['id'], f'{h["name"]} ({h["id"]})') for h in hubs],
         'formatting_template': '${label}',
         'validators': required_validator(param),
     }
 
 
 def product_list(config, client, param):
     if config.is_vendor():
@@ -146,18 +141,15 @@
         default_query = R().visibility.listing.eq(True) | R().visibility.syndication.eq(True)
     products = client.products.filter(default_query).order_by('name')
     return {
         'name': param['id'],
         'label': param['name'],
         'type': 'selectmany',
         'description': f'{param["description"]}',
-        'values': [
-            (p['id'], f'{p["name"]} ({p["id"]})')
-            for p in products
-        ],
+        'values': [(p['id'], f'{p["name"]} ({p["id"]})') for p in products],
         'formatting_template': '${label}',
         'validators': required_validator(param),
     }
 
 
 def checkbox(param):
     values = []
@@ -212,18 +204,15 @@
         handler = static_params[param['type']]
         return handler(param)
 
     raise ClickException(f'Unknown parameter type {param["type"]}')
 
 
 def generate_intro(config, report, output_format):
-    output_formats = {
-        format.id: format.description
-        for format in report.renderers
-    }
+    output_formats = {format.id: format.description for format in report.renderers}
     intro = """Welcome to the Connect CLI Report execution utility.
 
 <b><blue>Account</blue></b>
     <b>Id:</b> {account_id}
     <b>Name:</b> {account_name}
     <b>Type:</b> {account_type}
```

### Comparing `connect_cli-27.6/connect/cli/plugins/shared/base.py` & `connect_cli-27.7/connect/cli/plugins/shared/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         self._ws = self._wb[worksheet]
         self._validate_worksheet_sheet(self._ws, worksheet)
 
         self._product_id = product_id
         return self._product_id
 
     def sync(self):
-        raise NotImplementedError("Not implemented")
+        raise NotImplementedError('Not implemented')
 
     def save(self, output_file):
         self._wb.save(output_file)
 
     def _open_workbook(self, input_file):
         try:
             self._wb = load_workbook(
@@ -57,14 +57,14 @@
             raise ClickException(f'{input_file} is not a valid xlsx file.')
 
     @staticmethod
     def _validate_worksheet_sheet(ws, worksheet):
         ws_type = get_ws_type_by_worksheet_name(worksheet)
         max_letter = get_col_limit_by_ws_type(ws_type)
         col_headers = get_col_headers_by_ws_type(ws_type)
-        cels = ws['A1': f'{max_letter}1']
+        cels = ws['A1':f'{max_letter}1']
         for cel in cels[0]:
             if cel.value != col_headers[cel.column_letter]:
                 raise ClickException(
                     f'Invalid input file: column {cel.column_letter} '
                     f'must be {col_headers[cel.column_letter]}',
                 )
```

### Comparing `connect_cli-27.6/connect/cli/plugins/shared/constants.py` & `connect_cli-27.7/connect/cli/plugins/shared/constants.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/shared/export.py` & `connect_cli-27.7/connect/cli/plugins/shared/export.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,21 @@
 
 
 EXCEL_CONTENT_TYPE = 'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet'
 
 
 def get_translation_workbook(client, translation_id):
     try:
-        xls_data = client.ns('localization').translations[translation_id].action('attributes').get(
-            headers={'Accept': EXCEL_CONTENT_TYPE},
+        xls_data = (
+            client.ns('localization')
+            .translations[translation_id]
+            .action('attributes')
+            .get(
+                headers={'Accept': EXCEL_CONTENT_TYPE},
+            )
         )
         return load_workbook(filename=BytesIO(xls_data))
     except ClientError as error:
         if error.status_code == 404:
             status = format_http_status(error.status_code)
             raise ClickException(f'{status}: Translation {translation_id} not found.')
         handle_http_error(error)
```

### Comparing `connect_cli-27.6/connect/cli/plugins/shared/sync_stats.py` & `connect_cli-27.7/connect/cli/plugins/shared/sync_stats.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,22 +88,22 @@
 
         console.echo('')
         for module_stats in filter(lambda ms: ms._errors or ms._row_errors, self.values()):
             console.secho(f'Module {module_stats.name}:\n', fg='magenta')
 
             if module_stats._errors:
                 console.echo('  Errors')
-                console.echo("\n".join(f'    - {msg}' for msg in module_stats._errors))
+                console.echo('\n'.join(f'    - {msg}' for msg in module_stats._errors))
                 console.echo('')
 
             # group rows with same error message to avoid long prints in bulk errors
             first_row = None
             current_error = None
             for row_idx, messages in module_stats._row_errors.items():
-                error = "\n".join(f'    - {msg}' for msg in messages)
+                error = '\n'.join(f'    - {msg}' for msg in messages)
                 if not first_row:
                     first_row = row_idx
                 if not current_error:
                     current_error = error
                 if error != current_error:
                     self._print_error(current_error, first_row, row_idx - 1)
                     current_error = error
@@ -117,15 +117,14 @@
         else:
             console.echo(f'  Errors at rows #{row} to #{last_row}')
         console.echo(error)
         console.echo('')
 
 
 class _SynchronizerStatsModule:
-
     def __init__(self, name):
         self.name = name
         self.reset()
 
     def __str__(self):
         return ', '.join(f'{k}: {v}' for k, v in self.get_counts_as_dict().items())
 
@@ -159,16 +158,20 @@
             for r in row:
                 self._row_errors[r].extend(err)
         else:
             self._row_errors[row].extend(err)
 
     def get_processed_count(self):
         return (
-            self._updated + self._created + self._deleted + self._skipped
-            + len(self._errors) + len(self._row_errors)
+            self._updated
+            + self._created
+            + self._deleted
+            + self._skipped
+            + len(self._errors)
+            + len(self._row_errors)
         )
 
     def get_counts_as_dict(self):
         return {
             'processed': self.get_processed_count(),
             'created': self._created,
             'updated': self._updated,
```

### Comparing `connect_cli-27.6/connect/cli/plugins/shared/translation_attr_sync.py` & `connect_cli-27.7/connect/cli/plugins/shared/translation_attr_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from connect.cli.plugins.shared.sync_stats import SynchronizerStats
 
 
 class TranslationAttributesSynchronizer:
     """
     Synchronize the attributes of a translation from excel file.
     """
+
     _MAX_BATCH_SIZE = 10
 
     def __init__(self, client, progress, stats=None):
         self._client = client
         self._progress = progress
         self._wb = None
         self._ws = None
@@ -34,15 +35,17 @@
     @property
     def max_batch_size(self):
         return self._MAX_BATCH_SIZE
 
     def open(self, input_file, worksheet):
         self._open_workbook(input_file)
         if worksheet not in self._wb.sheetnames:
-            raise SheetNotFoundError(f"File does not contain worksheet '{worksheet}' to synchronize, skipping")
+            raise SheetNotFoundError(
+                f"File does not contain worksheet '{worksheet}' to synchronize, skipping",
+            )
         self._ws = self._wb[worksheet]
         self._validate_attributes_worksheet(self._ws)
 
     def save(self, output_file):
         self._wb.save(output_file)
 
     def sync(self, translation, is_clone=False):
@@ -111,15 +114,17 @@
         max_batch_size = self.max_batch_size
         try:
             translation_res = self._client.ns('localization').translations[translation_id]
             attr_value_list = list(attributes.values())
             chunk = 0
             # bulk update only support 10 items at a time
             for _ in range((math.ceil(len(attributes) / max_batch_size))):
-                translation_res.attributes.bulk_update(attr_value_list[chunk:chunk + max_batch_size])
+                translation_res.attributes.bulk_update(
+                    attr_value_list[chunk : chunk + max_batch_size],
+                )
                 chunk += max_batch_size
             self._mstats.updated(len(attributes))
             for row_idx in attributes.keys():
                 self._update_attributes_sheet_row(ws, row_idx)
         except ClientError as e:
             self._mstats.error(
                 f'Error while updating attributes: {str(e)}',
```

### Comparing `connect_cli-27.6/connect/cli/plugins/shared/translation_sync.py` & `connect_cli-27.7/connect/cli/plugins/shared/translation_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,17 @@
     @property
     def new_translations(self):
         return self._new_translations
 
     def sync(self):
         rows_data = defaultdict(dict)
         for row_idx, data in self._iterate_rows():
-            self._set_process_description(f'Processing Product translation {data.translation_id or data.locale}')
+            self._set_process_description(
+                f'Processing Product translation {data.translation_id or data.locale}',
+            )
             if data.action == '-' or data.is_primary == 'Yes':
                 self._mstats.skipped()
                 continue
             row_errors = self._validate_row(data)
             if row_errors:
                 self._mstats.error(row_errors, row_idx)
                 continue
@@ -76,17 +78,17 @@
                 f'Action must be `-`, `delete`, `update` or `create`. Provided {data.action}',
             )
             return errors
 
         if data.action in ('update', 'delete') and not data.translation_id:
             errors.append('Translation ID is required to update or delete a translation')
 
-        if (
-            data.action in ('update', 'create')
-            and data.autotranslation not in ('Enabled', 'Disabled')
+        if data.action in ('update', 'create') and data.autotranslation not in (
+            'Enabled',
+            'Disabled',
         ):
             errors.append(
                 'Autotranslation must be `Enabled` or `Disabled`. '
                 f'Provided {data.autotranslation}',
             )
 
         if data.action == 'create' and not data.locale:
@@ -102,17 +104,21 @@
 
         for row_idx, data in rows_data['update'].items():
             self._handle_action(self._action_update, row_idx, data)
 
         if len(rows_data['create']) > 0:
             # if there are any translations to create, then the context_id is needed
             try:
-                ctx = self._client.ns('localization').contexts.filter(
-                    instance_id=self._product_id,
-                ).first()
+                ctx = (
+                    self._client.ns('localization')
+                    .contexts.filter(
+                        instance_id=self._product_id,
+                    )
+                    .first()
+                )
                 for row_idx, data in rows_data['create'].items():
                     self._handle_action(partial(self._action_create, ctx['id']), row_idx, data)
             except ClientError as e:
                 self._mstats.error(str(e).split('\n'))
 
     def _handle_action(self, action_handler, row_idx, data):
         try:
@@ -130,31 +136,33 @@
             if e.status_code != 404:
                 raise
         self._mstats.deleted()
 
     def _action_update(self, data):
         self._set_process_description(f'Updating translation {data.translation_id}')
         payload = {
-            'description': data.description or "",
+            'description': data.description or '',
             'auto': {
                 'enabled': data.autotranslation == 'Enabled',
             },
         }
-        translation = self._client.ns('localization').translations[data.translation_id].update(payload)
+        translation = (
+            self._client.ns('localization').translations[data.translation_id].update(payload)
+        )
         self._mstats.updated()
         if translation['auto']['enabled']:
             self._translations_autotranslating.append(translation['id'])
         return translation
 
     def _action_create(self, context_id, data):
         self._set_process_description('Creating new translation')
         payload = {
             'context': {'id': context_id},
-            "locale": {'id': data.locale.split()[0]},
-            'description': data.description or "",
+            'locale': {'id': data.locale.split()[0]},
+            'description': data.description or '',
             'auto': {
                 'enabled': data.autotranslation == 'Enabled',
             },
         }
         translation = self._client.ns('localization').translations.create(payload)
         self._new_translations.append(translation)
         self._mstats.created()
```

### Comparing `connect_cli-27.6/connect/cli/plugins/shared/translations_synchronizers.py` & `connect_cli-27.7/connect/cli/plugins/shared/translations_synchronizers.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,15 +14,24 @@
     synchronizer.open(input_file, 'Translations')
     synchronizer.sync()
     if save:
         synchronizer.save(input_file)
     return synchronizer
 
 
-def translation_attributes_sync(worksheet, translation, client, progress, input_file, stats, save, is_clone):
+def translation_attributes_sync(
+    worksheet,
+    translation,
+    client,
+    progress,
+    input_file,
+    stats,
+    save,
+    is_clone,
+):
     synchronizer = TranslationAttributesSynchronizer(client, progress, stats)
     synchronizer.open(input_file, worksheet)
     synchronizer.sync(translation, is_clone)
     if save:
         synchronizer.save(input_file)
 
 
@@ -40,10 +49,16 @@
     for sheetname in get_translation_attributes_sheets(input_file):
         translation = sheetname.split()[1][1:-1]
         if is_clone:
             translation = next(iter_translation)
         if translation in translations_autotranslating:
             wait_for_autotranslation(client, progress, translation)
         translation_attributes_sync(
-            sheetname, translation, client,
-            progress, input_file, stats, save, is_clone,
+            sheetname,
+            translation,
+            client,
+            progress,
+            input_file,
+            stats,
+            save,
+            is_clone,
         )
```

### Comparing `connect_cli-27.6/connect/cli/plugins/shared/utils.py` & `connect_cli-27.7/connect/cli/plugins/shared/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         return 'F'
     return 'Z'
 
 
 def get_ws_type_by_worksheet_name(ws_name):
     if ws_name == 'Items':
         return 'items'
-    elif ws_name == "Ordering Parameters":
+    elif ws_name == 'Ordering Parameters':
         return 'params'
     elif ws_name == 'Fulfillment Parameters':
         return 'params'
     elif ws_name == 'Configuration Parameters':
         return 'params'
     elif ws_name == 'Media':
         return 'media'
@@ -156,24 +156,24 @@
     ws.cell(row_idx, 10, value=_calculate_translation_completion(translation)).number_format = '0%'
     ws.cell(row_idx, 11, value=translation['status'])
     ws.cell(row_idx, 12, value='Yes' if translation['primary'] else 'No')
     ws.cell(row_idx, 13, value=translation['events'].get('created', {}).get('at', '-'))
     ws.cell(row_idx, 14, value=translation['events'].get('updated', {}).get('at', '-'))
     if not update_mode:
         ws.cell(row_idx, 2, value='-')
-        ws.cell(row_idx, 8, value=translation.get('description', '-') or '-').alignment = Alignment(wrap_text=True)
+        ws.cell(row_idx, 8, value=translation.get('description', '-') or '-').alignment = Alignment(
+            wrap_text=True,
+        )
         ws.cell(row_idx, 9, value='Enabled' if translation['auto']['enabled'] else 'Disabled')
 
 
 def _calculate_translation_completion(translation):
     stats = translation['stats']
     try:
-        return (
-            stats.get('translated') / stats.get('total')
-        )
+        return stats.get('translated') / stats.get('total')
     except TypeError:
         return '-'
 
 
 def setup_locale_data_validation(general_ws, translations_ws):
     """
     Setup DataValidation on locale column.
```

### Comparing `connect_cli-27.6/connect/cli/plugins/translation/activate.py` & `connect_cli-27.7/connect/cli/plugins/translation/activate.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/translation/commands.py` & `connect_cli-27.7/connect/cli/plugins/translation/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,23 +50,23 @@
             ('center', 'Auto'),
             ('center', 'Status'),
             ('center', 'Primary'),
             ('center', 'Owner'),
         ),
         rows=[
             (
-                resource["id"],
-                resource["context"]["instance_id"],
-                resource["context"]["type"],
-                resource["context"]["name"],
-                resource["locale"]["name"],
-                resource["auto"]["status"],
-                resource["status"],
-                field_to_check_mark(resource["primary"]),
-                field_to_check_mark(acc_id == resource["owner"]["id"]),
+                resource['id'],
+                resource['context']['instance_id'],
+                resource['context']['type'],
+                resource['context']['name'],
+                resource['locale']['name'],
+                resource['auto']['status'],
+                resource['status'],
+                field_to_check_mark(resource['primary']),
+                field_to_check_mark(acc_id == resource['owner']['id']),
             )
             for resource in query_translations
         ],
     )
 
 
 @grp_translation.command(
@@ -204,15 +204,19 @@
     translation_id, should_wait_for_autotranslation = translation_sync.sync()
     translation_sync.save(input_file)
 
     if translation_id:
         with console.progress() as progress:
             if should_wait_for_autotranslation:
                 wait_for_autotranslation(config.active.client, progress, translation_id)
-            attributes_sync = TranslationAttributesSynchronizer(config.active.client, progress, stats)
+            attributes_sync = TranslationAttributesSynchronizer(
+                config.active.client,
+                progress,
+                stats,
+            )
             attributes_sync.open(input_file, 'Attributes')
             attributes_sync.sync(translation_id)
             attributes_sync.save(input_file)
 
     stats.print()
```

### Comparing `connect_cli-27.6/connect/cli/plugins/translation/constants.py` & `connect_cli-27.7/connect/cli/plugins/translation/constants.py`

 * *Files identical despite different names*

### Comparing `connect_cli-27.6/connect/cli/plugins/translation/export.py` & `connect_cli-27.7/connect/cli/plugins/translation/export.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 from openpyxl.worksheet.datavalidation import DataValidation
 
 from connect.cli.core.utils import validate_output_options
 from connect.cli.plugins.shared.export import alter_attributes_sheet, get_translation_workbook
 
 
 def dump_translation(
-    client, translation_id, output_file, output_path=None,
+    client,
+    translation_id,
+    output_file,
+    output_path=None,
 ):
     output_file = validate_output_options(output_path, output_file, default_dir_name=translation_id)
     wb = get_translation_workbook(client, translation_id)
     _alter_general_sheet(wb['General'])
     alter_attributes_sheet(wb['Attributes'])
     wb.save(output_file)
     return output_file
```

### Comparing `connect_cli-27.6/connect/cli/plugins/translation/primarize.py` & `connect_cli-27.7/connect/cli/plugins/translation/primarize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import click
 from connect.client import ClientError, ConnectClient
 
 from connect.cli.core.http import RequestLogger, format_http_status, handle_http_error
 
 
 def primarize_translation(
-    api_url, api_key,
+    api_url,
+    api_key,
     translation_id,
 ):
     try:
         client = ConnectClient(
             api_key=api_key,
             endpoint=api_url,
             use_specs=False,
```

### Comparing `connect_cli-27.6/connect/cli/plugins/translation/translation_sync.py` & `connect_cli-27.7/connect/cli/plugins/translation/translation_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,57 +19,58 @@
 
 
 class TranslationSynchronizer:
     """
     Synchronize a translation from excel file. It may update an existing
     translation or create a new one depending on some checks.
     """
+
     def __init__(self, client, account_id, stats=None):
         self._client = client
         self._wb = None
         self.account_id = account_id
         if stats is None:
             stats = SynchronizerStats()
         self._mstats = stats['Translation']
 
     def open(self, input_file):
         self._open_workbook(input_file)
         if 'General' not in self._wb.sheetnames:
-            raise SheetNotFoundError("File does not contain worksheet 'General' to synchronize, skipping")
+            raise SheetNotFoundError(
+                "File does not contain worksheet 'General' to synchronize, skipping",
+            )
         self._validate_general_worksheet(self._wb['General'])
 
     def save(self, output_file):
         self._wb.save(output_file)
 
     def sync(self):
         """
         Updates or creates the translation. Return the Translation ID and a boolean indicating
         if should wait for autotranslation to finish.
         If the operation is not successful then returns (None, False).
         """
         ws = self._wb['General']
         general_data = self._read_general_data(ws)
         current_translation = self._get_translation(general_data.translation_id)
-        do_create = (
-            not current_translation
-            or self._check_create(current_translation, general_data)
-        )
+        do_create = not current_translation or self._check_create(current_translation, general_data)
         translation_id = None
         if do_create:
             new_translation = self._try_create_translation(current_translation, general_data)
             if new_translation:
                 self._update_general_sheet(ws, new_translation)
                 translation_id = new_translation['id']
 
-                console.secho(f"\nCreated new translation {translation_id}\n", fg='yellow')
+                console.secho(f'\nCreated new translation {translation_id}\n', fg='yellow')
         else:
             translation_id = self._update_translation(general_data)
 
         should_wait_for_autotranslation = (
-            translation_id and general_data.auto_enabled == 'Enabled'
+            translation_id
+            and general_data.auto_enabled == 'Enabled'
             and (do_create or not current_translation['auto']['enabled'])
         )
         return translation_id, should_wait_for_autotranslation
 
     def _open_workbook(self, input_file):
         try:
             self._wb = load_workbook(input_file, data_only=True)
@@ -102,52 +103,52 @@
         return (
             translation['owner']['id'] != self.account_id
             or translation['locale']['id'] != general_data.locale_id
             or self._is_different_context(translation, general_data)
         )
 
     def _try_create_translation(self, current_translation, general_data):
-        if (
-            current_translation
-            and self._is_different_context(current_translation, general_data)
-        ):
+        if current_translation and self._is_different_context(current_translation, general_data):
             self._resolve_new_context(general_data)
 
         console.confirm(
-            click.style("A new translation will be created.\n", fg='yellow')
-            + "The owner will be the current active account, "
-            f"locale {general_data.locale_id} "
+            click.style('A new translation will be created.\n', fg='yellow')
+            + 'The owner will be the current active account, '
+            f'locale {general_data.locale_id} '
             f"and context '{general_data.context_name}' ({general_data.context_id}).\n"
-            "Do you want to continue?",
+            'Do you want to continue?',
             abort=True,
         )
 
         try:
-            translation = self._client.ns('localization').translations.create({
-                'context': {
-                    'id': general_data.context_id,
-                },
-                'locale': {
-                    'id': general_data.locale_id,
-                },
-                'description': general_data.description,
-                'auto': {
-                    'enabled': general_data.auto_enabled == 'Enabled',
+            translation = self._client.ns('localization').translations.create(
+                {
+                    'context': {
+                        'id': general_data.context_id,
+                    },
+                    'locale': {
+                        'id': general_data.locale_id,
+                    },
+                    'description': general_data.description,
+                    'auto': {
+                        'enabled': general_data.auto_enabled == 'Enabled',
+                    },
                 },
-            })
+            )
             self._mstats.created()
             return translation
         except ClientError as e:
             self._mstats.error(
                 f'Error while creating translation: {str(e)}',
             )
 
     def _is_different_context(self, translation, general_data):
         return (
-            general_data.context_id and general_data.context_id != translation['context']['id']
+            general_data.context_id
+            and general_data.context_id != translation['context']['id']
             or (
                 general_data.context_instance_id
                 and general_data.context_instance_id != translation['context']['instance_id']
             )
         )
 
     def _resolve_new_context(self, general_data):
@@ -162,21 +163,25 @@
                     )
                 if (
                     general_data.context_instance_id
                     and general_data.context_instance_id != ctx['instance_id']
                 ):
                     raise click.ClickException(
                         f"The Instance ID ({general_data.context_instance_id}) doesn't correspond "
-                        f"to the Context ID ({general_data.context_id})",
+                        f'to the Context ID ({general_data.context_id})',
                     )
                 general_data.context_name = ctx['name']
             elif general_data.context_instance_id:  # pragma: no branch
-                ctx = self._client.ns('localization').contexts.filter(
-                    instance_id=general_data.context_instance_id,
-                ).first()
+                ctx = (
+                    self._client.ns('localization')
+                    .contexts.filter(
+                        instance_id=general_data.context_instance_id,
+                    )
+                    .first()
+                )
                 if not ctx:
                     raise click.ClickException(
                         f"The Instance ID ({general_data.context_instance_id}) doesn't exist",
                     )
                 general_data.context_id = ctx['id']
                 general_data.context_name = ctx['name']
         except ClientError as error:
@@ -197,26 +202,33 @@
         ws['B3'].value = translation['owner']['name']
         ws['B5'].value = translation['context']['id']
         ws['B6'].value = translation['context']['instance_id']
         ws['B7'].value = translation['context']['name']
 
     def _update_translation(self, general_data):
         try:
-            translation_resource = self._client.ns('localization').translations[general_data.translation_id]
-            translation = translation_resource.update({
-                'description': general_data.description,
-                'auto': {
-                    'enabled': general_data.auto_enabled == 'Enabled',
+            translation_resource = self._client.ns('localization').translations[
+                general_data.translation_id
+            ]
+            translation = translation_resource.update(
+                {
+                    'description': general_data.description,
+                    'auto': {
+                        'enabled': general_data.auto_enabled == 'Enabled',
+                    },
                 },
-            })
+            )
             self._mstats.updated()
             return translation['id']
         except ClientError as e:
             self._mstats.error(
                 f'Error while updating translation information: {str(e)}',
             )
 
     @staticmethod
     def _read_general_data(ws):
-        return SimpleNamespace(**{
-            field: ws.cell(settings.row_idx, 2).value for field, settings in GENERAL_SHEET_FIELDS.items()
-        })
+        return SimpleNamespace(
+            **{
+                field: ws.cell(settings.row_idx, 2).value
+                for field, settings in GENERAL_SHEET_FIELDS.items()
+            }
+        )
```

### Comparing `connect_cli-27.6/connect/cli/plugins/translation/utils.py` & `connect_cli-27.7/connect/cli/plugins/translation/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,16 +11,15 @@
     column_widths.insert(column - 1, width)
     ws.insert_cols(idx=column, amount=1)
     _set_column_widths(ws, column_widths)
 
 
 def _get_column_widths(ws, total_columns):
     return [
-        ws.column_dimensions[
-            get_column_letter(column)
-        ].width for column in range(1, total_columns + 1)
+        ws.column_dimensions[get_column_letter(column)].width
+        for column in range(1, total_columns + 1)
     ]
 
 
 def _set_column_widths(ws, column_widths):
     for column, column_width in enumerate(column_widths, 1):
         ws.column_dimensions[get_column_letter(column)].width = column_width
```

### Comparing `connect_cli-27.6/pyproject.toml` & `connect_cli-27.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "connect-cli"
-version = "27.6"
+version = "27.7"
 description = "CloudBlue Connect Command Line Interface"
 authors = ["CloudBlue LLC"]
 license = "Apache-2.0"
 
 packages = [
     { include = "connect" },
 ]
@@ -63,28 +63,31 @@
 iso3166 = "^1.0.1"
 phonenumbers = "^8.12.19"
 connect-reports-core = "26.*"
 requests = "^2.25.1"
 toml = "^0.10.2"
 Jinja2 = "^3.1.2"
 jinja2-time = "^0.2.0"
-connect-eaas-core = ">=27.15,<28"
+connect-eaas-core = ">=28.10,<29"
 rich = "^12.4.1"
 poetry-core = "^1.3.0"  
 uvloop = { version = "^0.16.0", markers = "sys_platform == \"linux\" or sys_platform == \"darwin\"" }
 fs = "^2.4.12"
+pyyaml = "^6.0"
 
 [tool.poetry.group.test.dependencies]
+black = "23.*"
 pytest = "^6.1.2"
 pytest-cov = "^2.10.1"
 pytest-mock = "^3.3.1"
 freezegun = "^1.2.1"
 coverage = {extras = ["toml"], version = "^5.3"}
 responses = "^0.20.0"
 flake8 = "^5.0"
+flake8-black = "0.*"
 flake8-bugbear = "^22"
 flake8-cognitive-complexity = "^0.1"
 flake8-commas = "^2.1"
 flake8-future-import = "~0.4"
 flake8-isort = "5.*"
 flake8-broken-line = "~0.5"
 flake8-comprehensions = "^3.10"
@@ -146,21 +149,27 @@
     "connect/.data",
     "venv"
 ]
 
 show_source = true
 max_line_length = 120
 max_cognitive_complexity = 15
+select = "B"
 ignore = ["FI1", "W503"]
 
 
 [tool.isort]
 src_paths = "*"
 sections = ["FUTURE", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
 group_by_package = true
 multi_line_output = 3
 force_grid_wrap = 4
 combine_as_imports = true
 use_parentheses = true
 include_trailing_comma = true
 line_length = 100
 lines_after_imports = 2
+
+
+[tool.black]
+line_length = 100
+skip-string-normalization = true
```

### Comparing `connect_cli-27.6/PKG-INFO` & `connect_cli-27.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connect-cli
-Version: 27.6
+Version: 27.7
 Summary: CloudBlue Connect Command Line Interface
 Home-page: https://connect.cloudblue.com
 License: Apache-2.0
 Keywords: fulfillment,command,line,interface,utility,cli,vendor,connect,cloudblue
 Author: CloudBlue LLC
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,25 +15,26 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: connect-eaas-core (>=27.15,<28)
+Requires-Dist: connect-eaas-core (>=28.10,<29)
 Requires-Dist: connect-markdown-renderer (>=2.0.1,<3)
 Requires-Dist: connect-openapi-client (>=25.15)
 Requires-Dist: connect-reports-core (==26.*)
 Requires-Dist: fs (>=2.4.12,<3.0.0)
 Requires-Dist: interrogatio (>=2.3.1,<3.0.0)
 Requires-Dist: iso3166 (>=1.0.1,<2.0.0)
 Requires-Dist: jinja2-time (>=0.2.0,<0.3.0)
 Requires-Dist: openpyxl (>=3.0.7,<4.0.0)
 Requires-Dist: phonenumbers (>=8.12.19,<9.0.0)
 Requires-Dist: poetry-core (>=1.3.0,<2.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: rich (>=12.4.1,<13.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: uvloop (>=0.16.0,<0.17.0) ; sys_platform == "linux" or sys_platform == "darwin"
 Project-URL: Documentation, https://connect.cloudblue.com/community/sdk/cli/
 Project-URL: Repository, https://github.com/cloudblue/connect-cli
 Description-Content-Type: text/markdown
```

