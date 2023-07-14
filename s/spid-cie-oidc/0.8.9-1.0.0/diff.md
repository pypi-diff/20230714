# Comparing `tmp/spid_cie_oidc-0.8.9.tar.gz` & `tmp/spid_cie_oidc-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spid_cie_oidc-0.8.9.tar", last modified: Wed Nov 16 18:15:00 2022, max compression
+gzip compressed data, was "spid_cie_oidc-1.0.0.tar", last modified: Fri Jul 14 10:42:57 2023, max compression
```

## Comparing `spid_cie_oidc-0.8.9.tar` & `spid_cie_oidc-1.0.0.tar`

### file list

```diff
@@ -1,355 +1,376 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.884283 spid_cie_oidc-0.8.9/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    10641 2022-11-16 18:15:00.884283 spid_cie_oidc-0.8.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9889 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-16 18:15:00.884283 spid_cie_oidc-0.8.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.792282 spid_cie_oidc-0.8.9/spid_cie_oidc/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.792282 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/admin_inlines.py
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.792282 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     5254 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/migrations/0002_remove_user_taxpayer_id_user_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/migrations/0003_alter_user_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.796282 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/templatetags/has_group.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.796282 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.800282 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)    11942 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0002_alter_federationentityprofile_trust_mark_template.py
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0003_alter_federationdescendantcontact_entity_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0004_federationdescendant_jwks_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0005_alter_federationdescendant_jwks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0006_stafftoken.py
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0007_stafftoken_expire_at.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0008_alter_stafftoken_token.py
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0009_delete_stafftoken.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9571 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.804282 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/schemas/advanced_entity_list_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/schemas/fetch_endpoint_request.py
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/schemas/list_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)      815 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/schemas/trust_mark_status_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     2370 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.804282 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6202 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/mocked_responses.py
--rw-r--r--   0 runner    (1001) docker     (121)     7023 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    11765 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/test_02_trust_anchor_intermediary.py
--rw-r--r--   0 runner    (1001) docker     (121)     1991 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/test_05_validators.py
--rw-r--r--   0 runner    (1001) docker     (121)     2306 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/test_06_advanced_entity_listing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/test_08_schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1895 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/validators.py
--rw-r--r--   0 runner    (1001) docker     (121)     6730 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/authority/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.808282 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/abstract_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     6302 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1289 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/http_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2690 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/jwks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3047 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/jwtse.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.816282 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     9378 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1727 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0002_fetchedentitystatement.py
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0003_federationentityconfiguration_constraints.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0004_alter_federationentityconfiguration_authority_hints_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0005_alter_federationentityconfiguration_constraints.py
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0006_remove_trustchain_resultant_metadata_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0007_alter_trustchain_unique_together_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0008_fetchedentitystatement_jwt.py
--rw-r--r--   0 runner    (1001) docker     (121)      846 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0009_trustchain_trust_marks_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0010_federationentityconfiguration_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0011_alter_trustchain_status.py
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0012_delete_publicjwk.py
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0013_alter_federationentityconfiguration_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0014_alter_trustchain_unique_together_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0015_alter_trustchain_unique_together_trustchain_type_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0016_alter_trustchain_unique_together_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0017_remove_federationentityconfiguration_jwks_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0018_trustchain_jwks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0019_stafftoken.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12424 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/models.py
--rw-r--r--   0 runner    (1001) docker     (121)    12111 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.816282 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/fa_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/jwks.py
--rw-r--r--   0 runner    (1001) docker     (121)     4753 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/op_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)      916 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/resolve_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/rp_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    15554 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/statements.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.824282 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/fa_metadata_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/jwks_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     4024 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/op_metadata_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     4539 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/rp_metadata_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2658 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1861 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_01_entity_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_01_op_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_02_rp_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_03_jwks.py
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_04_fa_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     3868 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_05_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_06_http_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3046 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_07_resolve_entity_statement.py
--rw-r--r--   0 runner    (1001) docker     (121)     2727 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_07_validators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_08_statements.py
--rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_09_trust_chain.py
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_10_schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)    10918 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/trust_chain.py
--rw-r--r--   0 runner    (1001) docker     (121)     6647 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/trust_chain_operations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3758 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/validators.py
--rw-r--r--   0 runner    (1001) docker     (121)     3983 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/entity/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.824282 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1652 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     3420 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.828282 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0002_alter_onboardingregistration_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0003_alter_onboardingregistration_options.py
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0004_alter_onboardingregistration_public_jwks.py
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0005_alter_onboardingregistration_status.py
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0006_onboardingregistration_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0007_onboardingregistration_contact.py
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0008_onboardingregistration_auth_request_url.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2229 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.784282 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.828282 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/static/images/
--rw-r--r--   0 runner    (1001) docker     (121)    12269 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/static/images/SPID-e-CIE-696x383.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/static/images/logo-it.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.832282 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     9399 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_apply_policy.html
--rw-r--r--   0 runner    (1001) docker     (121)     1422 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_convert_jwk.html
--rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_convert_pem.html
--rw-r--r--   0 runner    (1001) docker     (121)     3036 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_decode_jwt.html
--rw-r--r--   0 runner    (1001) docker     (121)     3027 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_entities.html
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_jwk.html
--rw-r--r--   0 runner    (1001) docker     (121)     4450 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_landing.html
--rw-r--r--   0 runner    (1001) docker     (121)     2381 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_registration.html
--rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_resolve_statement.html
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_schemas.html
--rw-r--r--   0 runner    (1001) docker     (121)     1497 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_validate_ec.html
--rw-r--r--   0 runner    (1001) docker     (121)      939 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_validate_md.html
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_validating_tm.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.836282 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/mocked_responses.py
--rw-r--r--   0 runner    (1001) docker     (121)     4208 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/test_01_onboarding.py
--rw-r--r--   0 runner    (1001) docker     (121)    10247 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/test_02_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/test_11_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/tools_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     4484 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/validators.py
--rw-r--r--   0 runner    (1001) docker     (121)    16955 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.840282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.840282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.840282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3287 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/management/commands/fetch_openid_relying_parties.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.840282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     3103 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0002_remove_oidcsession_user_claims.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0003_remove_oidcsession_sub_issuedtoken_expires_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0004_alter_oidcsession_user.py
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0005_oidcsession_sid.py
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0006_oidcsession_acr.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0007_alter_issuedtoken_options_alter_oidcsession_options.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3488 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/processors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.844282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7508 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/authn_requests.py
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/authn_response.py
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/introspection_request.py
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/introspection_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/jwt.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/revocation_request.py
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/revocation_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3658 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/token_requests.py
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/token_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     8278 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.784282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.844282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     6337 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/css/provider.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.844282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/images/
--rw-r--r--   0 runner    (1001) docker     (121)   196297 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/images/logo-cie.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.848282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/svg/
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/svg/cie-ico-circle-bb.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2355 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/svg/logo-cie.svg
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/svg/no_image_available.svg
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/svg/spid-ico-circle-bb.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/svg/spid-logo-c-lb.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.848282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     2465 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templates/op_base.html
--rw-r--r--   0 runner    (1001) docker     (121)     4454 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templates/op_user_consent.html
--rw-r--r--   0 runner    (1001) docker     (121)     5096 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templates/op_user_history.html
--rw-r--r--   0 runner    (1001) docker     (121)     5978 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templates/op_user_login.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.848282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templatetags/spid_cie_op.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.856282 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5109 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/authn_request_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/authn_responses_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/introspection_request_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2493 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/introspection_response_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/revocation_request_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/revocation_response_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     6720 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    15443 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_02_authn_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     6257 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_03_authn_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     4619 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_03_refresh_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     3143 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_04_authn_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     3656 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_04_userinfo_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     4327 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_05_introspection_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     5691 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_05_token_request.py
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_06_processors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3001 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_06_token_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2556 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_07_fetch_relying_parties.py
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_07_introspection_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2888 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_08_introspection_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     5232 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_08_token_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     3875 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_09_revocation_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     2596 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_09_revocation_request.py
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_10_no_consent.py
--rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_10_revocation_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     2584 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_11_user_access_history.py
--rw-r--r--   0 runner    (1001) docker     (121)     1904 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_12_init.py
--rw-r--r--   0 runner    (1001) docker     (121)     4111 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/token_request_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1804 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/token_response_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.860283 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/
--rw-r--r--   0 runner    (1001) docker     (121)    12699 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10943 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/authz_request_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     5107 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/consent_page_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/introspection_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     3143 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/revocation_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     7928 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/token_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     2800 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/userinfo_endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.860283 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.860283 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.864282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2258 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/management/commands/fetch_openid_providers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.868282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     3568 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0002_rename_issuer_oidcauthentication_provider_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0003_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0004_rename_revoked_oidcauthenticationtoken_logged_out_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      825 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0005_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0006_alter_oidcauthentication_provider_configuration_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0007_alter_oidcauthentication_provider_jwks.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0008_remove_oidcauthentication_provider_and_more.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2671 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.868282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/oauth2/
--rw-r--r--   0 runner    (1001) docker     (121)     2351 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/oauth2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.868282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/oidc/
--rw-r--r--   0 runner    (1001) docker     (121)     2251 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/processors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3666 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.788282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.868282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     7900 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/css/access-button.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.868282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)     5247 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/js/spid-sp-access-button.js
--rw-r--r--   0 runner    (1001) docker     (121)     3335 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/js/spid_button.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.868282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/svg/
--rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/svg/cie-ico-circle-bb.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7406 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/svg/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/svg/spid-ico-circle-bb.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.868282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/templates/echo_attributes.html
--rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/templates/rp_base.html
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/templates/rp_error.html
--rw-r--r--   0 runner    (1001) docker     (121)     5186 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/templates/rp_landing.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.872283 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5684 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/mocked_response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1661 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_01_rp_ops.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_02_rp_commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     7872 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_03_rp_begin.py
--rw-r--r--   0 runner    (1001) docker     (121)     9164 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_04_rp_callback.py
--rw-r--r--   0 runner    (1001) docker     (121)     3010 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_05_oidc_rpinitiated_logout.py
--rw-r--r--   0 runner    (1001) docker     (121)     1770 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_06_fetch_openid_providers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_07_oidc_rp_landing.py
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_08_callback_echo_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2349 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_09_rp_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.876283 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/
--rw-r--r--   0 runner    (1001) docker     (121)     2916 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7600 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/rp_begin.py
--rw-r--r--   0 runner    (1001) docker     (121)    10419 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/rp_callback.py
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/rp_callback_echo_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3144 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/rp_initiated_logout.py
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/rp_landing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.876283 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      862 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.876283 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     2891 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/migrations/0002_alter_relyingpartytest_report.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2351 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.880282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/snippets/
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/snippets/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3207 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/snippets/crawler.py
--rw-r--r--   0 runner    (1001) docker     (121)      991 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/snippets/pyppeteer_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.788282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.880282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/static/images/
--rw-r--r--   0 runner    (1001) docker     (121)    11982 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/static/images/oops.webp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.880282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/templates/
--rw-r--r--   0 runner    (1001) docker     (121)    14291 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/templates/op_user_staff_test.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.880282 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2506 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/tests/test_01_user_staff.py
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     2313 2022-11-16 18:14:51.000000 spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-16 18:15:00.884283 spid_cie_oidc-0.8.9/spid_cie_oidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10641 2022-11-16 18:15:00.000000 spid_cie_oidc-0.8.9/spid_cie_oidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16427 2022-11-16 18:15:00.000000 spid_cie_oidc-0.8.9/spid_cie_oidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 18:15:00.000000 spid_cie_oidc-0.8.9/spid_cie_oidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-16 18:15:00.000000 spid_cie_oidc-0.8.9/spid_cie_oidc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-11-16 18:15:00.000000 spid_cie_oidc-0.8.9/spid_cie_oidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-16 18:15:00.000000 spid_cie_oidc-0.8.9/spid_cie_oidc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.580940 spid_cie_oidc-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-07-14 10:42:57.576940 spid_cie_oidc-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:42:57.580940 spid_cie_oidc-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.528936 spid_cie_oidc-1.0.0/spid_cie_oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.528936 spid_cie_oidc-1.0.0/spid_cie_oidc/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/accounts/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/accounts/admin_inlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/accounts/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.528936 spid_cie_oidc-1.0.0/spid_cie_oidc/accounts/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/accounts/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/accounts/migrations/0002_remove_user_taxpayer_id_user_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/accounts/migrations/0003_alter_user_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/accounts/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/accounts/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.528936 spid_cie_oidc-1.0.0/spid_cie_oidc/accounts/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/accounts/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/accounts/templatetags/has_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.532937 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.532937 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/migrations/0002_alter_federationentityprofile_trust_mark_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/migrations/0003_alter_federationdescendantcontact_entity_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/migrations/0004_federationdescendant_jwks_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/migrations/0005_alter_federationdescendant_jwks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/migrations/0006_stafftoken.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/migrations/0007_stafftoken_expire_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/migrations/0008_alter_stafftoken_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/migrations/0009_delete_stafftoken.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/migrations/0010_federationdescendant_metadata_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/migrations/0011_federationdescendant_issue_x509_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/migrations/0012_remove_federationdescendant_issue_x509.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10016 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.536937 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/schemas/advanced_entity_list_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/schemas/fetch_endpoint_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/schemas/list_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/schemas/trust_mark_status_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.536937 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/tests/mocked_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/tests/test_02_trust_anchor_intermediary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/tests/test_05_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/tests/test_06_advanced_entity_listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/tests/test_08_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/authority/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.540938 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/abstract_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/jwks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/jwtse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.544938 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0002_fetchedentitystatement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0003_federationentityconfiguration_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0004_alter_federationentityconfiguration_authority_hints_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0005_alter_federationentityconfiguration_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0006_remove_trustchain_resultant_metadata_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0007_alter_trustchain_unique_together_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0008_fetchedentitystatement_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0009_trustchain_trust_marks_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0010_federationentityconfiguration_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0011_alter_trustchain_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0012_delete_publicjwk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0013_alter_federationentityconfiguration_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0014_alter_trustchain_unique_together_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0015_alter_trustchain_unique_together_trustchain_type_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0016_alter_trustchain_unique_together_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0017_remove_federationentityconfiguration_jwks_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0018_trustchain_jwks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0019_stafftoken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0020_alter_federationentityconfiguration_jwks_core_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0021_federationhistoricalkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0021_federationhistoricalkey_squashed_0026_alter_federationhistoricalkey_jwk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0022_federationhistoricalkey_jwk_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0023_alter_federationhistoricalkey_jwk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0024_alter_federationhistoricalkey_kid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0025_alter_federationhistoricalkey_jwk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0026_alter_federationhistoricalkey_jwk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0027_alter_federationhistoricalkey_revocation_motivation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0028_federationentityconfiguration_issue_x509.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0029_alter_federationentityconfiguration_entity_type_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0030_remove_federationentityconfiguration_issue_x509.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.544938 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/schemas/fa_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/schemas/jwks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/schemas/op_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/schemas/resolve_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/schemas/rp_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15728 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/statements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.548938 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/fa_metadata_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/jwks_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/op_metadata_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/rp_metadata_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_01_entity_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_01_op_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_02_rp_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_03_jwks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_04_fa_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_05_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_06_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_07_resolve_entity_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_07_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_08_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_09_trust_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_10_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/trust_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/trust_chain_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/entity/x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.548938 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.552938 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/migrations/0002_alter_onboardingregistration_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/migrations/0003_alter_onboardingregistration_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/migrations/0004_alter_onboardingregistration_public_jwks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/migrations/0005_alter_onboardingregistration_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/migrations/0006_onboardingregistration_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/migrations/0007_onboardingregistration_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/migrations/0008_onboardingregistration_auth_request_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/migrations/0009_alter_onboardingregistration_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.524936 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.552938 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/static/images/SPID-e-CIE-696x383.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/static/images/logo-it.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.552938 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_apply_policy.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_convert_jwk.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_convert_pem.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_decode_jwt.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_entities.html
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_jwk.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_landing.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_registration.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_resolve_statement.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_schemas.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_validate_ec.html
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_validate_md.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_validating_tm.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.556939 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/tests/mocked_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/tests/test_01_onboarding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/tests/test_02_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/tests/test_11_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/tests/tools_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16955 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.556939 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.556939 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.556939 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/management/commands/fetch_openid_relying_parties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.556939 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/migrations/0002_remove_oidcsession_user_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/migrations/0003_remove_oidcsession_sub_issuedtoken_expires_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/migrations/0004_alter_oidcsession_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/migrations/0005_oidcsession_sid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/migrations/0006_oidcsession_acr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/migrations/0007_alter_issuedtoken_options_alter_oidcsession_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.560939 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/schemas/authn_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/schemas/authn_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/schemas/introspection_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/schemas/introspection_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/schemas/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/schemas/revocation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/schemas/revocation_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/schemas/token_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/schemas/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.524936 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.560939 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/static/css/provider.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.560939 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   196297 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/static/images/logo-cie.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.560939 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/static/svg/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/static/svg/cie-ico-circle-bb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/static/svg/logo-cie.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/static/svg/no_image_available.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/static/svg/spid-ico-circle-bb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/static/svg/spid-logo-c-lb.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.560939 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/templates/op_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/templates/op_user_consent.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/templates/op_user_history.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/templates/op_user_login.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.560939 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/templatetags/spid_cie_op.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.564939 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/authn_request_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/authn_responses_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/introspection_request_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/introspection_response_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/revocation_request_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/revocation_response_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15358 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_02_authn_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_03_authn_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_03_refresh_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_04_authn_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_04_userinfo_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_05_introspection_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_05_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_06_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_06_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_07_fetch_relying_parties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_07_introspection_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_08_introspection_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_08_token_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_09_revocation_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_09_revocation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_10_no_consent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_10_revocation_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_11_user_access_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_12_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/token_request_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/token_response_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.568939 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/views/
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/views/authz_request_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/views/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/views/consent_page_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/views/introspection_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/views/revocation_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/views/token_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/provider/views/userinfo_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.568939 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.568939 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.568939 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/management/commands/fetch_openid_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.568939 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/migrations/0002_rename_issuer_oidcauthentication_provider_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/migrations/0003_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/migrations/0004_rename_revoked_oidcauthenticationtoken_logged_out_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/migrations/0005_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/migrations/0006_alter_oidcauthentication_provider_configuration_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/migrations/0007_alter_oidcauthentication_provider_jwks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/migrations/0008_remove_oidcauthentication_provider_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.568939 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/oauth2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/oauth2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.572940 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.528936 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.572940 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/static/css/access-button.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.572940 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/static/js/spid-sp-access-button.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/static/js/spid_button.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.572940 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/static/svg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/static/svg/cie-ico-circle-bb.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/static/svg/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/static/svg/spid-ico-circle-bb.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.572940 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/templates/echo_attributes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/templates/rp_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/templates/rp_error.html
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/templates/rp_introspection.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/templates/rp_landing.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.572940 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/mocked_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/test_01_rp_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/test_02_rp_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/test_03_rp_begin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/test_04_rp_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/test_05_oidc_rpinitiated_logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/test_06_fetch_openid_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/test_07_oidc_rp_landing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/test_08_callback_echo_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/test_09_rp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.576940 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/views/
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/views/rp_begin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/views/rp_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/views/rp_callback_echo_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/views/rp_extend_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/views/rp_initiated_logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/views/rp_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/views/rp_landing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.576940 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.576940 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/migrations/0002_alter_relyingpartytest_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.576940 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/snippets/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/snippets/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/snippets/pyppeteer_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.528936 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.576940 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/static/images/oops.webp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.576940 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/templates/op_user_staff_test.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.576940 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/tests/test_01_user_staff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-14 10:42:47.000000 spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:57.576940 spid_cie_oidc-1.0.0/spid_cie_oidc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-07-14 10:42:57.000000 spid_cie_oidc-1.0.0/spid_cie_oidc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18035 2023-07-14 10:42:57.000000 spid_cie_oidc-1.0.0/spid_cie_oidc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:42:57.000000 spid_cie_oidc-1.0.0/spid_cie_oidc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:42:57.000000 spid_cie_oidc-1.0.0/spid_cie_oidc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-14 10:42:57.000000 spid_cie_oidc-1.0.0/spid_cie_oidc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 10:42:57.000000 spid_cie_oidc-1.0.0/spid_cie_oidc.egg-info/top_level.txt
```

### Comparing `spid_cie_oidc-0.8.9/LICENSE` & `spid_cie_oidc-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/PKG-INFO` & `spid_cie_oidc-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: spid_cie_oidc
-Version: 0.8.9
+Version: 1.0.0
 Summary: SPID/CIE OIDC Federation Entity
 Home-page: https://github.com/peppelinux/spid-cie-oidc
 Author: Giuseppe De Marco
 Author-email: demarcog83@gmail.com
 License: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 # SPID/CIE OIDC Federation SDK
 
 ![CI build](https://github.com/peppelinux/spid-cie-oidc-django/workflows/spid_cie_oidc/badge.svg)
 [![Maintainability](https://api.codeclimate.com/v1/badges/dd67eb5a241955b75585/maintainability)](https://codeclimate.com/github/italia/spid-cie-oidc-django/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/dd67eb5a241955b75585/test_coverage)](https://codeclimate.com/github/italia/spid-cie-oidc-django/test_coverage)
 ![Python version](https://img.shields.io/badge/license-Apache%202-blue.svg)
-![py-versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue.svg)
+![py-versions](https://img.shields.io/badge/python-3.10-blue.svg)
 [![GitHub issues](https://img.shields.io/github/issues/italia/spid-cie-oidc-django.svg)](https://github.com/italia/spid-cie-oidc-django/issues)
 [![Get invited](https://slack.developers.italia.it/badge.svg)](https://slack.developers.italia.it/)
 [![Join the #spid openid](https://img.shields.io/badge/Slack%20channel-%23spid%20openid-blue.svg)](https://developersitalia.slack.com/archives/C7E85ED1N/)
 
 
 SPID/CIE OIDC Federation is a suite of Django applications designed to
 make it easy to build an [Openid Connect Federation](https://openid.net/specs/openid-connect-federation-1_0.html), 
@@ -119,15 +119,15 @@
 Run the stack
 ````
 sudo docker-compose up
 ````
 
 Configure a proper DNS resolution for trust-anchor.org. In GNU/Linux we can configure it in `/etc/hosts`:
 ````
-127.0.0.1   localhost  trust-anchor.org relying-party.org cie-provider.org
+127.0.0.1   localhost  trust-anchor.org relying-party.org cie-provider.org wallet.trust-anchor.org
 ````
 
 Point your web browser to `http://relying-party.org:8001/oidc/rp/landing` and do your first oidc authentication.
 
 
 ## Usage
```

### Comparing `spid_cie_oidc-0.8.9/README.md` & `spid_cie_oidc-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPID/CIE OIDC Federation SDK
 
 ![CI build](https://github.com/peppelinux/spid-cie-oidc-django/workflows/spid_cie_oidc/badge.svg)
 [![Maintainability](https://api.codeclimate.com/v1/badges/dd67eb5a241955b75585/maintainability)](https://codeclimate.com/github/italia/spid-cie-oidc-django/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/dd67eb5a241955b75585/test_coverage)](https://codeclimate.com/github/italia/spid-cie-oidc-django/test_coverage)
 ![Python version](https://img.shields.io/badge/license-Apache%202-blue.svg)
-![py-versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue.svg)
+![py-versions](https://img.shields.io/badge/python-3.10-blue.svg)
 [![GitHub issues](https://img.shields.io/github/issues/italia/spid-cie-oidc-django.svg)](https://github.com/italia/spid-cie-oidc-django/issues)
 [![Get invited](https://slack.developers.italia.it/badge.svg)](https://slack.developers.italia.it/)
 [![Join the #spid openid](https://img.shields.io/badge/Slack%20channel-%23spid%20openid-blue.svg)](https://developersitalia.slack.com/archives/C7E85ED1N/)
 
 
 SPID/CIE OIDC Federation is a suite of Django applications designed to
 make it easy to build an [Openid Connect Federation](https://openid.net/specs/openid-connect-federation-1_0.html), 
@@ -100,15 +100,15 @@
 Run the stack
 ````
 sudo docker-compose up
 ````
 
 Configure a proper DNS resolution for trust-anchor.org. In GNU/Linux we can configure it in `/etc/hosts`:
 ````
-127.0.0.1   localhost  trust-anchor.org relying-party.org cie-provider.org
+127.0.0.1   localhost  trust-anchor.org relying-party.org cie-provider.org wallet.trust-anchor.org
 ````
 
 Point your web browser to `http://relying-party.org:8001/oidc/rp/landing` and do your first oidc authentication.
 
 
 ## Usage
```

### Comparing `spid_cie_oidc-0.8.9/setup.py` & `spid_cie_oidc-1.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 SRC_FOLDER = '.'
 PKG_NAME = 'spid_cie_oidc'
 
 INSTALL_REQUIRES = [
     "Django>=4.0",
     "cryptojwt>=1.8.2",
-    "pydantic>=1.8.2",
+    "pydantic>=1.8.2,<2.0",
     "pytz>=2021.3",
-    "aiohttp",
-    "requests",
+    "aiohttp>=3.8,<3.9",
+    "requests>=2.20,<3.0",
     "pydantic[email]",
     "djagger"
 ]
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), encoding='utf-8') as readme:
     README = readme.read()
 
@@ -55,15 +55,15 @@
             )
             if i and '__pycache__' not in i
         ]
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         LICENSE,
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules"],
     install_requires=INSTALL_REQUIRES,
     zip_safe=False,
 )
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/admin.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/accounts/admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/migrations/0001_initial.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/migrations/0002_remove_user_taxpayer_id_user_attributes.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/accounts/migrations/0002_remove_user_taxpayer_id_user_attributes.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/accounts/models.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/accounts/models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/admin.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/authority/admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0001_initial.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/authority/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0003_alter_federationdescendantcontact_entity_and_more.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/authority/migrations/0003_alter_federationdescendantcontact_entity_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0004_federationdescendant_jwks_and_more.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/authority/migrations/0004_federationdescendant_jwks_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0005_alter_federationdescendant_jwks.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/authority/migrations/0005_alter_federationdescendant_jwks.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0006_stafftoken.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/authority/migrations/0006_stafftoken.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/migrations/0008_alter_stafftoken_token.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/authority/migrations/0008_alter_stafftoken_token.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/models.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/authority/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,15 +113,24 @@
         blank=False,
         null=False,
         help_text=_("a list of public keys"),
         default=list,
         validators = [validate_public_jwks]
     )
     metadata_policy = models.JSONField(
-        blank=True, help_text=_("if present overloads the DEFAULT policy"), default=dict
+        blank=True, help_text=_(
+            "if present it overloads the DEFAULT policy. This will be applied "
+            "recursively to all the descendants."
+        ), default=dict
+    )
+    metadata = models.JSONField(
+        blank=True, help_text=_(
+            "if present it overloads the descendants metadata, "
+            "in the defined parts. This will be applied to the subordinate only."
+        ), default=dict
     )
     constraints = models.JSONField(
         blank=True, help_text=_("if present overloads the DEFAULT policy"), default=dict
     )
     extended_claims = models.JSONField(
         blank=True,
         help_text=_(
@@ -133,14 +142,15 @@
     status = models.CharField(
         max_length=33,
         default=False,
         help_text=_("Its entity configuration is periodically fetched and validated."),
         choices=[(i, i) for i in ENTITY_STATUS.keys()],
     )
     status_log = models.JSONField(blank=True, help_text=_("status log"), default=dict)
+
     is_active = models.BooleanField(
         default=False, help_text=_("If this entity is active. ")
     )
 
     class Meta:
         verbose_name = "Federation Entity Descendant"
         verbose_name_plural = "Federation Entity Descendants"
@@ -166,23 +176,27 @@
 
         policies = {
             k: FEDERATION_DEFAULT_POLICY[k] for k in self.entity_profiles
         }
 
         # apply custom policies if defined
         policies.update(self.metadata_policy)
-
+        ta = get_first_self_trust_anchor(iss)
         data = {
             "exp": exp_from_now(minutes=FEDERATION_DEFAULT_EXP),
             "iat": iat_now(),
-            "iss": get_first_self_trust_anchor(iss).sub,
+            "iss": ta.sub,
             "sub": self.sub,
             "jwks": {"keys": self.jwks},
             "metadata_policy": policies,
         }
+
+        if ta.fetch_endpoint:
+            data["source_endpoint"] = ta.fetch_endpoint
+
         if aud:
             data["aud"] = [aud] if isinstance(aud, str) else aud
 
         # add contacts
         contacts = FederationDescendantContact.objects.filter(entity=self).values_list(
             "contact", flat=True
         )
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/schemas/advanced_entity_list_endpoint.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/authority/schemas/advanced_entity_list_endpoint.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     prev_page_path: str
 
     def example():  # pragma: no cover
         return AdvancedEntityListResponse(
             iss= "https://registry.spid.gov.it/",
             iat= 1620050972,
             entities= [
-                # "{'https://rp.example.it/spid/': {'iat': 1588455866} }",
-                # "{'https://rp.another.it/spid/': {'iat': 1588455866} }"
+                # "{'https://rp.example.it/spid': {'iat': 1588455866} }",
+                # "{'https://rp.another.it/spid': {'iat': 1588455866} }"
             ],
             page= 1,
             total_pages= 2,
             total_entries= 189,
             next_page_path= "/federation_adv_list/?page=2",
             prev_page_path= ""
         )
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/schemas/trust_mark_status_endpoint.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/authority/schemas/trust_mark_status_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/settings.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/authority/settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/mocked_responses.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/authority/tests/mocked_responses.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/settings.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/authority/tests/settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/test_02_trust_anchor_intermediary.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/authority/tests/test_02_trust_anchor_intermediary.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,16 @@
     def test_fetch_endpoint(self):
         self.rp_profile.__str__()
         self.rp_profile.trust_mark_template_as_json
         url = reverse("oidcfed_fetch")
         c = Client()
         res = c.get(url, data={"sub": self.rp.sub})
         data = verify_jws(res.content.decode(), self.ta_conf.jwks_fed[0])
+        
+        self.assertEqual(data['source_endpoint'], 'http://testserver//fetch')
         self.assertTrue(data["jwks"])
 
     def test_list_endpoint(self):
         url = reverse("oidcfed_list")
         c = Client()
         res = c.get(url, data={})
         self.assertTrue(res.json())
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/test_05_validators.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/authority/tests/test_05_validators.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/test_06_advanced_entity_listing.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/authority/tests/test_06_advanced_entity_listing.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/tests/test_08_schemas.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/authority/tests/test_08_schemas.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/urls.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/authority/urls.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 from django.conf import settings
 from django.urls import path
 
 from .views import entity_list, fetch, trust_mark_status, advanced_entity_listing
 
 _PREF = getattr(settings, "OIDC_PREFIX", "")
 urlpatterns = [
-    path(f"{_PREF}fetch/", fetch, name="oidcfed_fetch"),
-    path(f"{_PREF}list/", entity_list, name="oidcfed_list"),
+    path(f"{_PREF}fetch", fetch, name="oidcfed_fetch"),
+    path(f"{_PREF}list", entity_list, name="oidcfed_list"),
     path(
-        f"{_PREF}trust_mark_status/",
+        f"{_PREF}trust_mark_status",
         trust_mark_status,
         name="oidcfed_trust_mark_status",
     ),
     path(
-        f"{_PREF}advanced_entity_listing/",
+        f"{_PREF}advanced_entity_listing",
         advanced_entity_listing,
         name="oidcfed_advanced_entity_listing",
     ),
 ]
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/validators.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/authority/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,11 +50,11 @@
         )
 
     superior_sub = import_string(
         "spid_cie_oidc.entity.models.get_first_self_trust_anchor"
     )().sub
     if superior_sub not in authority_hints:
         raise NotDescendant(
-            f"This participant MUST have {superior_sub} in"
+            f"This participant MUST have {superior_sub} in "
             f"its authority_hints claim. It has: {authority_hints}."
         )
     return ec
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/authority/views.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/authority/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
     tags = ['Federation API']
 )
 def trust_mark_status(request):
     failed_data = {"active": False}
     if request.POST.get("sub", "") and request.POST.get("id", ""):
         sub = request.POST["sub"]
         _id = request.POST["id"]
-    
+
     elif request.POST.get("trust_mark", ""):
         try:
             unpad_jwt_head(request.POST["trust_mark"])
             payload = unpad_jwt_payload(request.POST["trust_mark"])
             sub = payload.get("sub", "")
             _id = payload.get("id", "")
         except Exception:
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/abstract_models.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/abstract_models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/admin.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/admin.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,25 +7,34 @@
 # from prettyjson import PrettyJSONWidget
 
 from django.conf import settings
 from .jwtse import unpad_jwt_payload
 from .statements import EntityConfiguration, get_entity_configurations, get_entity_statements
 from .models import (
     FederationEntityConfiguration,
+    FederationHistoricalKey,
     FetchedEntityStatement,
     TrustChain,
     StaffToken
 )
 from spid_cie_oidc.entity.trust_chain_operations import get_or_create_trust_chain
 
 from . settings import HTTPC_PARAMS
 
 logger = logging.getLogger(__name__)
 
 
+@admin.register(FederationHistoricalKey)
+class FederationHistoricalKey(admin.ModelAdmin):
+    readonly_fields = ('jwk', "as_json")
+    list_display = ("entity", "kid", "inactive_from")
+    list_filter = ("created", "modified", "inactive_from")
+    search_fields = ("entity",)
+
+
 @admin.register(FederationEntityConfiguration)
 class FederationEntityConfigurationAdmin(admin.ModelAdmin):
     # formfield_overrides = {
     # JSONField: {
     # "widget": PrettyJSONWidget(
     # attrs={"initial": "parsed", "disabled": True}
     # )
@@ -164,15 +173,14 @@
     list_display = ("sub", "exp", "modified", "is_valid")
     list_filter = ("exp", "modified", "is_active")
     search_fields = ("sub",)
     readonly_fields = (
         "created",
         "modified",
         "parties_involved",
-        "metadata",
         "status",
         "log",
         "chain",
         "iat",
     )
     actions = [update_trust_chain]
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/exceptions.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/exceptions.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/http_client.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/http_client.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/jwks.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/jwks.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,22 @@
     key = key or new_rsa_key()
     thumbprint = key.thumbprint(hash_function=hash_func or DEFAULT_HASH_FUNC)
     jwk = key.to_dict()
     jwk["kid"] = thumbprint.decode()
     return jwk
 
 
+def public_jwk_from_private_jwk(jwk_dict: dict):
+    # exports public
+    _k = key_from_jwk_dict(jwk_dict)
+    jwk = _k.serialize()
+    jwk["kid"] = jwk_dict['kid']
+    return jwk
+
+
 def private_pem_from_jwk(jwk_dict: dict):
     # exports private
 
     _k = key_from_jwk_dict(jwk_dict)
     pk = _k.private_key()
     pem = pk.private_bytes(
         encoding=serialization.Encoding.PEM,
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/jwtse.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/jwtse.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,104 +1,137 @@
 import base64
 import binascii
 import json
 import logging
 
+import cryptojwt
 from cryptojwt.exception import UnsupportedAlgorithm, VerificationError
 from cryptojwt.jwe.jwe import factory
+from cryptojwt.jwe.jwe_ec import JWE_EC
 from cryptojwt.jwe.jwe_rsa import JWE_RSA
 from cryptojwt.jwk.jwk import key_from_jwk_dict
 from cryptojwt.jws.jws import JWS
+from cryptojwt.jws.utils import left_hash
 from typing import Union
 
 from .settings import (
     DEFAULT_JWE_ALG,
     DEFAULT_JWE_ENC,
     ENCRYPTION_ALG_VALUES_SUPPORTED,
     SIGNING_ALG_VALUES_SUPPORTED,
 )
 
-
 logger = logging.getLogger(__name__)
 
 
 def unpad_jwt_element(jwt: str, position: int) -> dict:
     b = jwt.split(".")[position]
-    padded = f"{b}{'=' * divmod(len(b),4)[1]}"
+    padded = f"{b}{'=' * divmod(len(b), 4)[1]}"
     data = json.loads(base64.urlsafe_b64decode(padded))
     return data
 
 
 def unpad_jwt_head(jwt: str) -> dict:
     return unpad_jwt_element(jwt, position=0)
 
 
 def unpad_jwt_payload(jwt: str) -> dict:
     return unpad_jwt_element(jwt, position=1)
 
 
-def create_jwe(plain_dict: Union[dict, None], jwk_dict: dict, **kwargs) -> str:
+def create_jwe(plain_dict: Union[dict, str, int, None], jwk_dict: dict, **kwargs) -> str:
     logger.debug(f"Encrypting dict as JWE: " f"{plain_dict}")
     _key = key_from_jwk_dict(jwk_dict)
-    _rsa = JWE_RSA(
-        json.dumps(plain_dict).encode(),
+
+    if isinstance(_key, cryptojwt.jwk.rsa.RSAKey):
+        JWE_CLASS = JWE_RSA
+    elif isinstance(_key, cryptojwt.jwk.ec.ECKey):
+        JWE_CLASS = JWE_EC
+
+    if isinstance(plain_dict, dict):
+        _payload = json.dumps(plain_dict).encode()
+    elif not plain_dict:
+        logger.warning(f"create_jwe with null payload!")
+        _payload = ""
+    elif isinstance(plain_dict, (str, int)):
+        _payload = plain_dict
+    else:
+        logger.error(f"create_jwe with unsupported payload type!")
+        _payload = ""
+
+    _keyobj = JWE_CLASS(
+        _payload,
         alg=DEFAULT_JWE_ALG,
         enc=DEFAULT_JWE_ENC,
         kid=_key.kid,
         **kwargs
     )
-    jwe = _rsa.encrypt(_key.public_key())
+
+    jwe = _keyobj.encrypt(_key.public_key())
     logger.debug(f"Encrypted dict as JWE: {jwe}")
     return jwe
 
 
 def decrypt_jwe(jwe: str, jwk_dict: dict) -> dict:
     # get header
     try:
         jwe_header = unpad_jwt_head(jwe)
-    except (binascii.Error, Exception) as e: # pragma: no cover
+    except (binascii.Error, Exception) as e:  # pragma: no cover
         logger.error(f"Failed to extract JWT header: {e}")
         raise VerificationError("The JWT is not valid")
 
     _alg = jwe_header.get("alg", DEFAULT_JWE_ALG)
     _enc = jwe_header.get("enc", DEFAULT_JWE_ENC)
     jwe_header.get("kid")
 
-    if _alg not in ENCRYPTION_ALG_VALUES_SUPPORTED: # pragma: no cover
+    if _alg not in ENCRYPTION_ALG_VALUES_SUPPORTED:  # pragma: no cover
         raise UnsupportedAlgorithm(f"{_alg} has beed disabled for security reason")
 
     _decryptor = factory(jwe, alg=_alg, enc=_enc)
 
     # _dkey = RSAKey(priv_key=PRIV_KEY)
     _dkey = key_from_jwk_dict(jwk_dict)
     msg = _decryptor.decrypt(jwe, [_dkey])
 
-    msg_dict = json.loads(msg)
-    logger.debug(f"Decrypted JWT as: {json.dumps(msg_dict, indent=2)}")
+    try:
+        msg_dict = json.loads(msg)
+        logger.debug(f"Decrypted JWT as: {json.dumps(msg_dict, indent=2)}")
+    except json.decoder.JSONDecodeError:
+        msg_dict = msg
+        logger.debug(f"Decrypted JWT as: {msg_dict}")
     return msg_dict
 
 
-def create_jws(payload: dict, jwk_dict: dict, alg: str = "RS256", **kwargs) -> str:
-
+def create_jws(payload: dict, jwk_dict: dict, alg: str = "RS256", protected:dict = {}, **kwargs) -> str:
     _key = key_from_jwk_dict(jwk_dict)
     _signer = JWS(payload, alg=alg, **kwargs)
 
-    signature = _signer.sign_compact([_key])
+    signature = _signer.sign_compact([_key], protected=protected, **kwargs)
     return signature
 
 
 def verify_jws(jws: str, pub_jwk: dict, **kwargs) -> str:
     _key = key_from_jwk_dict(pub_jwk)
 
     _head = unpad_jwt_head(jws)
-    if _head.get("kid") != pub_jwk["kid"]: # pragma: no cover
+    if _head.get("kid") != pub_jwk["kid"]:  # pragma: no cover
         raise Exception(
             f"kid error: {_head.get('kid')} != {pub_jwk['kid']}"
         )
 
     _alg = _head["alg"]
-    if _alg not in SIGNING_ALG_VALUES_SUPPORTED or not _alg: # pragma: no cover
+    if _alg not in SIGNING_ALG_VALUES_SUPPORTED or not _alg:  # pragma: no cover
         raise UnsupportedAlgorithm(f"{_alg} has beed disabled for security reason")
 
     verifier = JWS(alg=_head["alg"], **kwargs)
     msg = verifier.verify_compact(jws, [_key])
     return msg
+
+
+def verify_at_hash(id_token, access_token) -> bool:
+    id_token_at_hash = id_token['at_hash']
+    at_hash = left_hash(access_token, "HS256")
+    if at_hash != id_token_at_hash:
+        raise Exception(
+            f"at_hash error: {at_hash} != {id_token_at_hash}"
+        )
+    return True
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0001_initial.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0002_fetchedentitystatement.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0002_fetchedentitystatement.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0003_federationentityconfiguration_constraints.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0003_federationentityconfiguration_constraints.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0004_alter_federationentityconfiguration_authority_hints_and_more.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0004_alter_federationentityconfiguration_authority_hints_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0005_alter_federationentityconfiguration_constraints.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0005_alter_federationentityconfiguration_constraints.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0006_remove_trustchain_resultant_metadata_and_more.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0006_remove_trustchain_resultant_metadata_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0007_alter_trustchain_unique_together_and_more.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0007_alter_trustchain_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0009_trustchain_trust_marks_and_more.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0009_trustchain_trust_marks_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0010_federationentityconfiguration_entity_type.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0010_federationentityconfiguration_entity_type.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0011_alter_trustchain_status.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0011_alter_trustchain_status.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0013_alter_federationentityconfiguration_metadata.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0013_alter_federationentityconfiguration_metadata.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0015_alter_trustchain_unique_together_trustchain_type_and_more.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0015_alter_trustchain_unique_together_trustchain_type_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0016_alter_trustchain_unique_together_and_more.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0016_alter_trustchain_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0017_remove_federationentityconfiguration_jwks_and_more.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0017_remove_federationentityconfiguration_jwks_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/migrations/0019_stafftoken.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/migrations/0019_stafftoken.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/models.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,17 +22,20 @@
     ENTITY_TYPES,
     FEDERATION_DEFAULT_EXP
 )
 from spid_cie_oidc.entity.statements import EntityConfiguration
 from spid_cie_oidc.entity.utils import exp_from_now, iat_now, random_token
 from spid_cie_oidc.entity.validators import (
     validate_entity_metadata,
-    validate_metadata_algs
+    validate_metadata_algs,
+    validate_private_jwks
 )
 
+from .jwks import public_jwk_from_private_jwk
+
 logger = logging.getLogger(__name__)
 
 
 def is_leaf(statement_metadata):
     for _typ in ENTITY_TYPE_LEAFS:
         if _typ in statement_metadata:
             return True # pragma: no cover
@@ -76,20 +79,22 @@
         default=list,
     )
     jwks_fed = models.JSONField(
         blank=False,
         null=False,
         help_text=_("a list of private keys for Federation ops"),
         default=_create_jwks,
+        validators = [validate_private_jwks],
     )
     jwks_core = models.JSONField(
-        blank=False,
+        blank=True,
         null=False,
         help_text=_("a list of private keys for Core ops"),
         default=_create_jwks,
+        validators = [validate_private_jwks],
     )
     trust_marks = models.JSONField(
         blank=True,
         help_text=_("which trust marks MUST be exposed in its entity configuration"),
         default=list,
     )
     trust_marks_issuers = models.JSONField(
@@ -144,14 +149,15 @@
 }
 """
         ),
         default=dict,
         # TODO
         # validators=[validate_entity_metadata,]
     )
+
     is_active = models.BooleanField(
         default=False,
         help_text=_(
             "If this configuration is active. "
             "At least one configuration must be active"
         ),
     )
@@ -240,16 +246,29 @@
             self.entity_configuration_as_dict,
             self.jwks_fed[0],
             alg=self.default_signature_alg,
             typ="entity-statement+jwt",
             **kwargs,
         )
 
+    @property
+    def fetch_endpoint(self) -> Union[str, None]:
+        metadata = self.entity_configuration_as_dict.get('metadata', {})
+        if 'federation_entity' in metadata:
+            return metadata['federation_entity'].get("federation_fetch_endpoint", None)
+
+    def set_jwks_as_array(self):
+        for i in ('jwks_fed','jwks_core'):
+            value = getattr(self, i)
+            if not isinstance(value, list):
+                setattr(self, i, [value])
+
     def save(self, *args, **kwargs):
         self.entity_type = self.type[0]
+        self.set_jwks_as_array()
         super().save(*args, **kwargs)
 
     def __str__(self):
         return "{} [{}]".format(
             self.sub, "active" if self.is_active else "--"
         )
 
@@ -424,14 +443,89 @@
         else:
             return False
 
     def __str__(self):
         return f"{self.user} {self.is_active}"
 
 
+class FederationHistoricalKey(TimeStampedModel):
+    """
+    https://openid.net/specs/openid-connect-federation-1_0.html#name-federation-historical-keys-
+    """
+
+    REVOCATION_REASONS_MAP = (
+        ("0", 'unspecified'),
+        ("1", 'keyCompromise'),
+        ("2", 'cACompromise'),
+        ("3", 'affiliationChanged'),
+        ("4", 'superseded'),
+        ("5", 'cessationOfOperation'),
+        ("6", 'certificateHold'),
+        # 7 is unused in rfc5280
+        ("8", 'removeFromCRL'),
+        ("9", 'privilegeWithdrawn'),
+        ("10", 'aACompromise')
+    )
+
+    # REVOCATION_REASONS_CODES = {k:k for k in REVOCATION_REASONS_MAP.keys()}
+
+    entity = models.ForeignKey(FederationEntityConfiguration, on_delete=models.CASCADE)
+    kid = models.CharField(
+        blank=False, null=False, max_length=128
+    )
+    inactive_from = models.DateTimeField(help_text=_(
+        "Expired or Revocation date if revocation motivation is configured"
+    ))
+    revocation_motivation = models.CharField(
+        blank=True, null=False, max_length=33, choices=REVOCATION_REASONS_MAP
+    )
+
+    jwk = models.JSONField(help_text=_("private jwk"), default=dict)
+
+    class Meta:
+        verbose_name = "Federation Historical Key"
+        verbose_name_plural = "Federation Historical Keys"
+
+    @property
+    def as_dict(self):
+        if not self.jwk:
+            return {}
+
+        kdict = public_jwk_from_private_jwk(self.jwk)
+        if self.revocation_motivation:
+            kdict["revoked"] = {
+              "revoked_at": int(self.inactive_from.timestamp()),
+              "reason": dict(self.REVOCATION_REASONS_MAP)[self.revocation_motivation],
+              "reason_code": self.revocation_motivation
+            }
+        else:
+            kdict["exp"] = int(self.inactive_from.timestamp())
+        return kdict
+
+    @property
+    def as_json(self):
+        return json.dumps(self.as_dict)
+
+    def save(self, *args, **kwargs):
+        if self.kid:
+            for jwk in self.entity.jwks_fed:
+                if not jwk.get('kid', None):
+                    continue
+                elif self.kid == jwk['kid']:
+                    _indx = self.entity.jwks_fed.index(jwk)
+                    self.jwk = self.entity.jwks_fed.pop(_indx)
+                    self.entity.save()
+                    break
+
+        super().save(*args, **kwargs)
+
+    def __str__(self):
+        return f"{self.entity} {self.kid}"
+
+
 def get_first_self_trust_anchor(
     sub: str = None,
 ) -> Union[FederationEntityConfiguration, None]:
     """
     get the first available Trust Anchor that represent self
     as a qualified issuer
     """
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/policy.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/policy.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/jwks.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/schemas/jwks.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             "ES384",
             "ES512",
             "PS256",
             "PS384",
             "PS512",
         ]
     ]
-    use: Literal["sig", "enc"]
+    use: Optional[Literal["sig", "enc"]]
     n: Optional[str]  # Base64urlUInt-encoded
     e: Optional[str]  # Base64urlUInt-encoded
 
     def check_value_for_rsa(value, name, values):
         if "EC" == values.get("kty") and value:
             raise ValueError(f"{name} must be present only for kty = RSA")
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/op_metadata.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/schemas/op_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,27 +105,24 @@
     acr_values_supported: List[AcrValuesSupported]
     signed_jwks_uri: Optional[HttpUrl]
     jwks_uri: Optional[HttpUrl]
     jwks: Optional[JwksCie]
 
     @root_validator(pre=False)
     def validate(cls, values):
-        jwks = values.get("jwks")
-        jwks_uri = values.get("jwks_uri")
-        signed_jwks_uri = values.get("signed_jwks_uri")
-        if not jwks_uri and not jwks and not signed_jwks_uri:
+        jwks_there = False
+        for i in ("jwks_uri", "jwks", "signed_jwks_uri"):
+            if values.get(i):
+                jwks_there = True
+                break
+
+        if not jwks_there:
             raise ValueError(
                 "one of signed_jwks_uri or jwks_uri or jwks must be set"
             )
-        if jwks_uri and jwks:
-            raise ValueError("can't use jwks and jwks_uri together")
-        elif jwks_uri and signed_jwks_uri:
-            raise ValueError(
-                "can't use signed_jwks_uri and jwks_uri together"
-            )
         return values
 
 
 class OPMetadataCie(OPMetadata):
     scopes_supported: List[ScopeSupported]
     response_types_supported = ["code"]
     response_modes_supported: List[ResponseModesSupported]
@@ -133,11 +130,9 @@
     claims_supported: List[ClaimsSupported]
     claims_parameter_supported = True
     tls_client_certificate_bound_access_tokens = True
     authorization_response_iss_parameter_supported = True
 
 
 class OPMetadataSpid(OPMetadata):
-    # TODO: Could be specified in multiple languages
-    op_name: str
-    # TODO: Could be specified in multiple languages
-    op_uri: str
+    op_name: Optional[str]
+    op_uri: Optional[str]
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/resolve_endpoint.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/schemas/resolve_endpoint.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 class ResolveRequest(BaseModel):
     sub : HttpUrl
     anchor : HttpUrl
     format :Literal["json"]
 
     def example():  # pragma: no cover
         return ResolveRequest(
-            sub= "http://127.0.0.1:8000/oidc/rp/",
-            anchor= "http://127.0.0.1:8000/",
+            sub= "http://127.0.0.1:8000/oidc/rp",
+            anchor= "http://127.0.0.1:8000",
             format= "json",
         )
 
 
 #  class ResolveResponse(BaseModel):
     #  iss : HttpUrl
     #  sub : HttpUrl
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/schemas/rp_metadata.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/schemas/rp_metadata.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,27 +20,24 @@
 
     signed_jwks_uri: Optional[HttpUrl]
     jwks_uri: Optional[HttpUrl]
     jwks: Optional[JwksSpid]
 
     @root_validator(pre=False)
     def validate(cls, values):
-        jwks = values.get("jwks")
-        jwks_uri = values.get("jwks_uri")
-        signed_jwks_uri = values.get("signed_jwks_uri")
-        if not jwks_uri and not jwks and not signed_jwks_uri:
+        jwks_there = False
+        for i in ("jwks_uri", "jwks", "signed_jwks_uri"):
+            if values.get(i):
+                jwks_there = True
+                break
+
+        if not jwks_there:
             raise ValueError(
                 "one of signed_jwks_uri or jwks_uri or jwks must be set"
             )
-        if jwks_uri and jwks:
-            raise ValueError("can't use jwks and jwks_uri together")
-        elif jwks_uri and signed_jwks_uri:
-            raise ValueError(
-                "can't use signed_jwks_uri and jwks_uri together"
-            )
         return values
 
 
 class RPMetadataSpid(RPMetadata):
     pass
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/settings.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 # old, for requests
 # HTTPC_PARAMS = {
 # "verify": True,
 # "timeout": 4
 # }
 
 # for aiohttp
-HTTPC_TIMEOUT = 4
+HTTPC_TIMEOUT = getattr(settings, "HTTPC_TIMEOUT", 12)
 HTTPC_PARAMS = getattr(
     settings,
     "HTTPC_PARAMS",
     {
         "connection": {"ssl": True},
         "session": {"timeout": aiohttp.ClientTimeout(total=HTTPC_TIMEOUT)},
     },
@@ -69,15 +69,21 @@
     settings,
     "OIDCFED_MAXIMUM_AUTHORITY_HINTS",
     2,
 )
 
 FEDERATION_DEFAULT_EXP = getattr(settings, "FEDERATION_DEFAULT_EXP", 2880)
 
-ENTITY_TYPE_LEAFS = ["openid_relying_party", "openid_provider", "oauth_resource"]
+ENTITY_TYPE_LEAFS = [
+    "openid_relying_party", 
+    "openid_provider", 
+    "oauth_resource",
+    "wallet_provider",
+    "wallet_relying_party"
+]
 ENTITY_TYPES = ["federation_entity"] + ENTITY_TYPE_LEAFS
 ENTITY_STATUS = {
     "unreachable": False,
     "valid": True,
     "signature_failed": False,
     "not_valid": False,
     "unknown": None,
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/statements.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/statements.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     )
 
 
 def get_http_url(urls: list, httpc_params: dict = {}) -> list:
     if getattr(settings, "HTTP_CLIENT_SYNC", False):
         responses = []
         for i in urls:
-            res = requests.get(i, **httpc_params)
+            res = requests.get(i, **httpc_params) # nosec - B113
             responses.append(res.content.decode())
     else:
         responses = asyncio.run(http_get(urls, httpc_params)) # pragma: no cover
     return responses
 
 
 def get_entity_statements(urls: list, httpc_params: dict = {}) -> list:
@@ -432,13 +432,18 @@
                 continue
 
             else:
                 _url = f"{fetch_api_url}?sub={self.sub}"
                 logger.info(f"Getting entity statements from {_url}")
                 jwts = get_entity_statements([_url], self.httpc_params)
                 jwt = jwts[0]
-                self.validate_by_superior_statement(jwt, ec)
+                if jwt:
+                    self.validate_by_superior_statement(jwt, ec)
+                else:
+                    logger.error(
+                        f"Empty response for {_url}"
+                    )
 
         return self.verified_by_superiors
 
     def __repr__(self) -> str:
         return f"{self.sub} valid {self.is_valid}"
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/jwks_settings.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/jwks_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/op_metadata_settings.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/op_metadata_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/rp_metadata_settings.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/rp_metadata_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
 RP_METADATA_CIE_NO_REDIRECT_URIS = deepcopy(RP_METADATA_CIE)
 RP_METADATA_CIE_NO_REDIRECT_URIS.pop("redirect_uris")
 
 RP_METADATA_SPID_NOJWKS_NOJWKS_URI = deepcopy(RP_METADATA_SPID)
 RP_METADATA_SPID_NOJWKS_NOJWKS_URI.pop("jwks_uri")
 
+
 RP_METADATA_CIE_NOJWKS_NOJWKS_URI = deepcopy(RP_METADATA_CIE)
 RP_METADATA_CIE_NOJWKS_NOJWKS_URI.pop("jwks_uri")
 
 
 RP_METADATA_JWK1 = {'kty': 'RSA', 'n': 'w8H80eT2zrs2XQ-SApZG9TkuXDuIxANfCVHt4fFqNnOEZaCNWqlTQIo0JiSBE-QmzZ09TYP1BJpESuQf_PUeLRVPfYHsBVk5OYvhT27_nYlV7_1LsFGLxxsIa-hswMMzvW-1_huKLy6Fp0WP0ouUJAHsF_eYVtO1ApRhvlIVd5azM4k7t8Lh8lkCSdF1SfGHfXnXJRb-XensZ0cFSfe2Koq9mD7jpGLXlPpXxj8Ow0g7KYT5kVtWE5ULmNmO7BIN1Hx4HpggbbEGgC9FyjKw4GfFb-csnB-icBPf_60HomjrkFFt6vTjrcqQaHOj-sEjP36N8rMSBiMmiMSPnsHhMQ', 'e': 'AQAB', 'd': 'jEDxjcTZXBbgBV8Bgt7-qfW1FJoHDEFKFxhfMpHQQoETa-jTPhCxOD2MzYM8A-9kKc8tu9r-crTAl1PI42kPnMd283phixd5G5Tv8gSaGdnq-45ka0iRuC7TItUdDiMNb_2YzB4ZLGLNmaIKQJSGqCHEcQuRVyxJtTZwrXaMMOhDqJaWUvUQWF5C7g5O5mOVTkNKw6ujzhqcWa4N3NE-HwcbVW_9st4s1c_ng-DlwLTptaeM5j-LOeZMX1zcVlwYMi5ZkYYY6FHHjYI4nBWDtqhvf-64QaTv8exIjk8PcxHOwhfLTWiHPLk14af7U_pCzkP87WQCBgNfvt3WILQ5DQ', 'p': '75eNHkWaYQMgzVfFwif5uftSxqOhFU6VkxNKdqoRuFxJuVTO-M-vbQc3BwPxms2xrpizU6zGcoPGPvccDi0G040wZh34pWDVABMgGMKXKmeTwj8FuM1DzOVq8DKHmdrhk1gaQbPAP8JVOVYK7uh_lG5wmz3X-En1McMk-E8g8Ic', 'q': '0Sny6DLNtDP1_B9qiyCaMtRqPSAUZ1ohCZRlBT6-IGRR31Kt5S2JcVNDnF5w4dunlDY4nhIBZ0v0VyzWKgDXj6qrFY1pm1iE29gW227YsVRWQU8xWGpBwEu8nxNMr0u0zfe0QEGWU4RvNAsZPRa31HU87Vm7I3NSZ34DZsCZJoc', 'kid': 'HIvo33-Km7n03ZqKDJfWVnlFudsW28YhQZx5eaXtAKA'}
 RP_METADATA_JWK1_pub = {'kty': 'RSA', 'n': 'w8H80eT2zrs2XQ-SApZG9TkuXDuIxANfCVHt4fFqNnOEZaCNWqlTQIo0JiSBE-QmzZ09TYP1BJpESuQf_PUeLRVPfYHsBVk5OYvhT27_nYlV7_1LsFGLxxsIa-hswMMzvW-1_huKLy6Fp0WP0ouUJAHsF_eYVtO1ApRhvlIVd5azM4k7t8Lh8lkCSdF1SfGHfXnXJRb-XensZ0cFSfe2Koq9mD7jpGLXlPpXxj8Ow0g7KYT5kVtWE5ULmNmO7BIN1Hx4HpggbbEGgC9FyjKw4GfFb-csnB-icBPf_60HomjrkFFt6vTjrcqQaHOj-sEjP36N8rMSBiMmiMSPnsHhMQ', 'e': 'AQAB', 'kid': 'HIvo33-Km7n03ZqKDJfWVnlFudsW28YhQZx5eaXtAKA'}
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/settings.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_01_entity_configuration.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_01_entity_configuration.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_01_op_metadata.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_01_op_metadata.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,23 +16,21 @@
 
 
 class OpMetadataTest(TestCase):
     def test_op_metatada_cie(self):
         OPMetadataCie(**OP_METADATA_CIE)
 
     def test_op_metatada_cie_jwks_and_jwks_uri(self):
-        with self.assertRaises(ValidationError):
-            OPMetadataCie(**OP_METADATA_CIE_JWKS_AND_JWKS_URI)
+        self.assertTrue(OPMetadataCie(**OP_METADATA_CIE_JWKS_AND_JWKS_URI))
 
     def test_op_metatada_spid(self):
         OPMetadataSpid(**OP_METADATA_SPID)
 
     def test_op_metatada_spid_jwks_and_jwks_uri(self):
-        with self.assertRaises(ValidationError):
-            OPMetadataSpid(**OP_METADATA_SPID_JWKS_AND_JWKS_URI)
+        self.assertTrue(OPMetadataSpid(**OP_METADATA_SPID_JWKS_AND_JWKS_URI))
 
     def test_op_metatada_spid_jwks_no_jwks_uri(self):
         OPMetadataSpid(**OP_METADATA_SPID_JWKS_NO_JWKS_URI)
 
     def test_op_metatada_spid_jws_ec_no_correct(self):
         with self.assertRaises(ValidationError):
             OPMetadataSpid(**OP_METADATA_SPID_JWKS_EC_NO_CORRECT)
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_02_rp_metadata.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_02_rp_metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,26 +20,24 @@
     def test_rp_metadataSpid(self):
         RPMetadataSpid(**RP_METADATA_SPID)
 
     def test_rp_metadataSpid_no_redirect_uris(self):
         with self.assertRaises(ValidationError):
             RPMetadataSpid(**RP_METADATA_SPID_NO_REDIRECT_URIS)
 
-    def test_rp_metadataSpid_jwks_and_jkws_uri(self):
-        with self.assertRaises(ValidationError):
-            RPMetadataSpid(**RP_METADATA_SPID_JWKS_AND_JWKS_URI)
-
-    def test_rp_metadataSpid_no_jwks_and_no_jkws_uri(self):
+    def test_rp_metadataSpid_jwks_and_jwks_uri(self):
+        self.assertTrue(RPMetadataSpid(**RP_METADATA_SPID_JWKS_AND_JWKS_URI))
+            
+    def test_rp_metadataSpid_no_jwks_and_no_jwks_uri(self):
         with self.assertRaises(ValidationError):
             RPMetadataSpid(**RP_METADATA_SPID_NOJWKS_NOJWKS_URI)
 
-    def test_rp_metadataCie_jwks_and_jkws_uri(self):
-        with self.assertRaises(ValidationError):
-            RPMetadataCie(**RP_METADATA_CIE_JWKS_AND_JWKS_URI)
+    def test_rp_metadataCie_jwks_and_jwks_uri(self):
+        self.assertTrue(RPMetadataCie(**RP_METADATA_CIE_JWKS_AND_JWKS_URI))
 
     def test_rp_metadataCie_no_redirect_uris(self):
         with self.assertRaises(ValidationError):
             RPMetadataCie(**RP_METADATA_CIE_NO_REDIRECT_URIS)
 
-    def test_rp_metadataCie_no_jwks_and_no_jkws_uri(self):
+    def test_rp_metadataCie_no_jwks_and_no_jwks_uri(self):
         with self.assertRaises(ValidationError):
             RPMetadataCie(**RP_METADATA_CIE_NOJWKS_NOJWKS_URI)
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_03_jwks.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_03_jwks.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_05_policy.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_05_policy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from copy import deepcopy
 
 from django.test import TestCase
-from spid_cie_oidc.authority.settings import FEDERATION_DEFAULT_POLICY
 from spid_cie_oidc.entity.policy import (
     apply_policy, 
     diff2policy,
     gather_policies,
     PolicyError
 )
 from spid_cie_oidc.entity.tests.rp_metadata_settings import RP_METADATA
@@ -22,17 +21,14 @@
 
     def test_gather_polices_rp(self):
         combined_policy = gather_policies([{},rp_onboarding_data], "openid_relying_party")
         self.assertTrue(combined_policy == {'scope': {'value': ['openid']}})
 
     def test_apply_policy(self):
         fa_policy = {}
-        fa_policy["scope"] = FEDERATION_DEFAULT_POLICY["openid_relying_party"][
-            "scope"
-        ]
         fa_policy["contacts"] = {"add": "ciao@email.it"}
         combined_policy = apply_policy(deepcopy(RP_METADATA), fa_policy)
         combined_contacts = combined_policy["contacts"]
         self.assertTrue("ciao@email.it" in combined_contacts)
         self.assertTrue("ops@rp.example.it" in combined_contacts)
         
     def test_apply_policy_one_of(self):
@@ -78,17 +74,14 @@
         combined_contacts = apply_policy(deepcopy(RP_METADATA), fa_policy)
         self.assertTrue("ciao@email.it" in combined_contacts["contacts"])
         self.assertTrue("ops@rp.example.it" in combined_contacts["contacts"])
 
 
     def test_diff_two_policy(self):
         fa_policy_old = {}
-        fa_policy_old["scope"] = FEDERATION_DEFAULT_POLICY["openid_relying_party"][
-            "scope"
-        ]
         fa_policy_new = deepcopy(fa_policy_old)
         fa_policy_new["contacts"] = {"add": "test@email.it"}
         result = diff2policy(fa_policy_new, fa_policy_old)
         diff = {
             "contacts": {
                 "add": {
                     "add": "test@email.it"
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_07_resolve_entity_statement.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_07_resolve_entity_statement.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_07_validators.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_07_validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         op_md = {}
         op_md["openid_provider"] = deepcopy(OP_METADATA)
         validate_entity_metadata(op_md)
 
     def test_validate_entity_no_valid_op_metadata(self):
         op_md = {}
         op_md["openid_provider"] = deepcopy(OP_METADATA)
-        op_md["openid_provider"].pop("op_name")
+        op_md["openid_provider"].pop("issuer")
         with self.assertRaises(ValidationError):
             validate_entity_metadata(op_md)
 
     def test_validate_entity_rp_metadata(self):
         rp_md = {}
         rp_md["openid_relying_party"] = deepcopy(RP_METADATA_SPID)
         validate_entity_metadata(rp_md)
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_08_statements.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_08_statements.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/tests/test_09_trust_chain.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/tests/test_09_trust_chain.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/trust_chain.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/trust_chain.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/trust_chain_operations.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/trust_chain_operations.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/urls.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,28 @@
 Including another URLconf
     1. Import the include() function: from django.urls import include, path
     2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
 """
 from django.conf import settings
 from django.urls import path
 
-from .views import entity_configuration, resolve_entity_statement
+from .views import (
+    entity_configuration,
+    historical_keys,
+    resolve_entity_statement
+)
 
 _PREF = getattr(settings, "OIDC_PREFIX", "")
 
 urlpatterns = [
     path(
         f"{_PREF}.well-known/openid-federation",
         entity_configuration,
         name="entity_configuration",
     ),
-    path(f"{_PREF}resolve/", resolve_entity_statement, name="oidcfed_resolve"),
+    path(f"{_PREF}resolve", resolve_entity_statement, name="oidcfed_resolve"),
+    path(
+        f"{_PREF}.well-known/openid-federation-historical-jwks",
+        historical_keys,
+        name="oidcfed_historical_keys"
+    )
 ]
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/entity/validators.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/entity/validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,16 @@
         schema = RP_PROVIDER_PROFILES[RP_DEFAULT_PROVIDER_PROFILES]
         try:
             schema["rp_metadata"](**value["openid_relying_party"])
         except Exception as e:
             raise ValidationError(
                 f"RP metadata fail {e}. "
             )
+    
+    # TODO - add wallet_provider and wallet_relying_party once standardized
 
 
 def validate_private_jwks(values: Union[dict, list]):
     if isinstance(values, dict):
         values = [values]
     try:
         for jwk_dict in values:
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/admin.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/forms.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/forms.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,57 +20,63 @@
     )
 
 
 class OnboardingRegistrationForm(forms.Form):
 
     organization_name = forms.CharField(
         initial="",
-        label=_("organization Name"),
+        label=_("Organization Name"),
         error_messages={"required": _("Enter your organization name")},
     )
 
     url_entity = forms.URLField(
         initial="",
-        label=_("url of the entity"),
-        error_messages={"required": _("Enter your url of the entity")},
+        label=_("Entity URL"),
+        error_messages={"required": _("Enter the entity unique identifier (HTTP URL)")},
         validators=[validate_entity_configuration, unique_entity_url],
     )
 
     authn_buttons_page_url = forms.URLField(
         initial="",
-        label=_("url of the page where the SPID/CIE button is available"),
+        label=_("URL of the login page, if available"),
         error_messages={
             "required": _(
                 "Enter the url of the page where the SPID/CIE button is available"
             )
         },
+        required=False,
     )
 
     auth_request_url = forms.CharField(
         initial="",
-        label=_("authentication request url"),
+        label=_("Authentication request URL, if available"),
         required = False
     )
 
     contact = forms.EmailField(
         initial="",
-        label=_("contact email"),
+        label=_("Contact email"),
         error_messages={"required": _("Enter your contact email")},
     )
 
     type = forms.ChoiceField(
         choices=[(i, i) for i in ENTITY_TYPES],
         label="",
         error_messages={"required": _("Select a entity type")},
     )
 
     public_jwks = forms.JSONField(
         initial=list,
-        label=_("public jwks of the entities"),
-        error_messages={"required": _("Enter the public jwks of the entities")},
+        label=_("Public Federation JWKs"),
+        error_messages={
+            "required": _(
+                "Enter the public JWKs published in your Entity Configuration, "
+                "as double check."
+            )
+        },
         validators=[validate_public_jwks],
     )
 
 
 class OnboardingCreateTrustChain(forms.Form):
 
     sub = forms.URLField(
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0001_initial.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0002_alter_onboardingregistration_options_and_more.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/migrations/0002_alter_onboardingregistration_options_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0003_alter_onboardingregistration_options.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/migrations/0003_alter_onboardingregistration_options.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0004_alter_onboardingregistration_public_jwks.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/migrations/0004_alter_onboardingregistration_public_jwks.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0005_alter_onboardingregistration_status.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/migrations/0005_alter_onboardingregistration_status.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0006_onboardingregistration_type.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/migrations/0006_onboardingregistration_type.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0007_onboardingregistration_contact.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/migrations/0007_onboardingregistration_contact.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/migrations/0008_onboardingregistration_auth_request_url.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/migrations/0008_onboardingregistration_auth_request_url.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/models.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/static/images/SPID-e-CIE-696x383.jpg` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/static/images/SPID-e-CIE-696x383.jpg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/static/images/logo-it.svg` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/static/images/logo-it.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/base.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/base.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_apply_policy.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_apply_policy.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_convert_jwk.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_convert_jwk.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_convert_pem.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_convert_pem.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_decode_jwt.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_decode_jwt.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_entities.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_entities.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_jwk.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_jwk.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_landing.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_landing.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_registration.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_registration.html`

 * *Files 3% similar despite different names*

```diff
@@ -43,16 +43,17 @@
                <textarea id="id_{{ form_field.html_name }}" rows="5"
                   name="{{ form_field.name }}">{{ form.public_jwks.value}}</textarea>
             {% else %}
             <input type="{{ form_field.field.widget.input_type }}" class="form-control"
                id="id_{{ form_field.html_name }}" name="{{ form_field.name }}" value="{{form_field.value}}">
             {% endif %}
          </div>
+         <span for="id_{{ form_field.html_name }}_help" class="text-info">{{ form_field.help_text }}</span>
          <span for="id_{{ form_field.html_name }}" class="text-danger">{{ form_field.errors }}</span>
       </div>
       {% endfor %}
 
       <input type="submit" name="confirm" class="btn btn-lg btn-success btn-block" value="{% trans 'Submit' %}" />
    </form>
 
 </div>
-{% endblock %}
+{% endblock %}
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_resolve_statement.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_resolve_statement.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_schemas.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_schemas.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_validate_ec.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_validate_ec.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_validate_md.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_validate_md.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/templates/onboarding_validating_tm.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/templates/onboarding_validating_tm.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/test_01_onboarding.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/tests/test_01_onboarding.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,17 +39,20 @@
         client = Client()
         res = client.get(url, self.data)
         self.assertEqual(res.status_code, 200)
         res = client.post(url, self.data)
         self.assertFormError(
             res, "form", "organization_name", "Enter your organization name"
         )
-        self.assertFormError(res, "form", "url_entity", "Enter your url of the entity")
+        self.assertFormError(res, "form", "url_entity", 
+            "Enter the entity unique identifier (HTTP URL)"
+        )
         self.assertFormError(
-            res, "form", "public_jwks", "Enter the public jwks of the entities"
+            res, "form", "public_jwks", 
+            "Enter the public JWKs published in your Entity Configuration, as double check."
         )
         self.assertEqual(res.status_code, 200)
         self.data["organization_name"] = "test name"
         self.data["url_entity"] = "http://rp-test/oidc/rp"
         self.data["type"] = "openid_relying_party"
         self.data["authn_buttons_page_url"] = "https://authnurl.com"
         self.data["public_jwks"] = {"key": "ciao"}
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/test_02_tools.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/tests/test_02_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,28 +121,28 @@
         self.assertEqual(res.status_code, 200)
 
     def test_resolve_statement(self):
         url = reverse("oidc_onboarding_resolve_statement")
         res = self.client.get(url)
         self.assertEqual(res.status_code, 200)
         res = self.client.get(url, {
-            "sub":"http://127.0.0.1:8000/oidc/",
+            "sub":"http://127.0.0.1:8000/oidc",
             "type": "openid_provider",
-            "anchor": "http://127.0.0.1:8000/"
+            "anchor": "http://127.0.0.1:8000"
         })
         self.assertEqual(res.status_code, 200)
         self.assertIn("alert-error", res.content.decode())
         self.assertIn(
             "Failed to resolve entity statement, Please check your inserted data", 
             res.content.decode())
 
         form_data= {
-            "sub": "http://127.0.0.1:8000/oidc/op/",
+            "sub": "http://127.0.0.1:8000/oidc/op",
             "type": "openid_provider",
-            "anchor": "http://127.0.0.1:8000/",
+            "anchor": "http://127.0.0.1:8000",
         }
         res = self.client.get(url, form_data)
         self.assertEqual(res.status_code, 200)
         self.assertIsNotNone(res.context['resolved_statement'])
 
     def test_validating_trust_mark(self):
         url = reverse("oidc_onboarding_validating_trustmark")
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/test_11_admin.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/tests/test_11_admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/tests/tools_settings.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/tests/tools_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/urls.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,45 +39,45 @@
     onboarding_validate_ec,
 )
 
 _PREF = getattr(settings, "OIDC_PREFIX", "")
 
 urlpatterns = [
     path(
-        f"{_PREF}onboarding/landing/",
+        f"{_PREF}onboarding/landing",
         onboarding_landing,
         name="oidc_onboarding_landing",
     ),
     path(
-        f"{_PREF}onboarding/registration/",
+        f"{_PREF}onboarding/registration",
         onboarding_registration,
         name="oidc_onboarding_registration",
     ),
     path(
-        f"{_PREF}onboarding/entities/",
+        f"{_PREF}onboarding/entities",
         onboarding_entities,
         name="oidc_onboarding_entities",
     ),
     path(
-        f"{_PREF}onboarding/tools/create-jwk/",
+        f"{_PREF}onboarding/tools/create-jwk",
         onboarding_create_jwk,
         name="oidc_onboarding_create_jwk",
     ),
     path(
-        f"{_PREF}onboarding/tools/convert-jwk/",
+        f"{_PREF}onboarding/tools/convert-jwk",
         onboarding_convert_jwk,
         name="oidc_onboarding_convert_jwk",
     ),
     path(
-        f"{_PREF}onboarding/convert-pem/",
+        f"{_PREF}onboarding/convert-pem",
         onboarding_convert_pem,
         name="oidc_onboarding_convert_pem",
     ),
     path(
-        f"{_PREF}onboarding/tools/resolve-statement/",
+        f"{_PREF}onboarding/tools/resolve-statement",
         onboarding_resolve_statement,
         name="oidc_onboarding_resolve_statement",
     ),
     path(
         f"{_PREF}onboarding/tools/validating-trustmark",
         onboarding_validating_trustmark,
         name="oidc_onboarding_validating_trustmark",
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/onboarding/views.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/onboarding/views.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/admin.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/forms.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/forms.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/management/commands/fetch_openid_relying_parties.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/management/commands/fetch_openid_relying_parties.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0001_initial.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0003_remove_oidcsession_sub_issuedtoken_expires_and_more.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/migrations/0003_remove_oidcsession_sub_issuedtoken_expires_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0004_alter_oidcsession_user.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/migrations/0004_alter_oidcsession_user.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/migrations/0007_alter_issuedtoken_options_alter_oidcsession_options.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/migrations/0007_alter_issuedtoken_options_alter_oidcsession_options.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/models.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,17 +51,17 @@
         if session and destroy_session:
             session.delete()
         self.revoked = True
         iss_tokens = IssuedToken.objects.filter(session=self)
         iss_tokens.update(revoked=True)
         self.save()
 
-    def pairwised_sub(self):
+    def pairwised_sub(self, provider_id:str):
         return hashlib.sha256(
-            f"{self.user_uid}{self.client_id}{OIDCFED_PROVIDER_SALT}".encode()
+            f"{self.user_uid}{self.client_id}{provider_id}{OIDCFED_PROVIDER_SALT}".encode()
         ).hexdigest()
 
     def public_sub(self):
         return hashlib.sha256(
             f"{self.user_uid}{OIDCFED_PROVIDER_SALT}".encode()
         ).hexdigest()
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/authn_requests.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/schemas/authn_requests.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,59 +38,53 @@
 
 class ClaimsType(str, Enum):
     essential = ClaimsTypeEssential
     value = ClaimsTypeStringValue
     values = ClaimsTypeStringValues
 
 
-nameStr = "https://attributes.spid.gov.it/name"
-
-
 class UserInfoSpid(BaseModel):
     name: Optional[dict] = Field(
-        alias="https://attributes.spid.gov.it/name", default=None
+        alias="given_name", default=None
     )
     family_name: Optional[dict] = Field(
-        alias="https://attributes.spid.gov.it/familyName", default=None
+        alias="family_name", default=None
     )
     place_of_birth: Optional[dict] = Field(
-        alias="https://attributes.spid.gov.it/placeOfBirth", default=None
-    )
-    county_of_birth: Optional[dict] = Field(
-        alias="https://attributes.spid.gov.it/countyOfBirth", default=None
+        alias="place_of_birth", default=None
     )
     date_of_birth: Optional[dict] = Field(
-        alias="https://attributes.spid.gov.it/dateOfBirth", default=None
+        alias="date_of_birth", default=None
     )
     gender: Optional[dict] = Field(
-        alias="https://attributes.spid.gov.it/gender", default=None
+        alias="gender", default=None
     )
     company_name: Optional[dict] = Field(
         alias="https://attributes.spid.gov.it/companyName", default=None
     )
     registered_office: Optional[dict] = Field(
         alias="https://attributes.spid.gov.it/registeredOffice", default=None
     )
     fiscal_number: Optional[dict] = Field(
-        alias="https://attributes.spid.gov.it/fiscalNumber", default=None
+        alias="https://attributes.spid.gov.it/fiscal_number", default=None
     )
     iva_code: Optional[dict] = Field(
         alias="https://attributes.spid.gov.it/ivaCode", default=None
     )
     id_card: Optional[dict] = Field(
         alias="https://attributes.spid.gov.it/idCard", default=None
     )
     mobile_phone: Optional[dict] = Field(
         alias="https://attributes.spid.gov.it/mobilePhone", default=None
     )
     email: Optional[dict] = Field(
-        alias="https://attributes.spid.gov.it/email", default=None
+        alias="email", default=None
     )
     address: Optional[dict] = Field(
-        alias="https://attributes.spid.gov.it/address", default=None
+        alias="address", default=None
     )
     expiration_date: Optional[dict] = Field(
         alias="https://attributes.spid.gov.it/expirationDate", default=None
     )
     digital_address: Optional[dict] = Field(
         alias="https://attributes.spid.gov.it/digitalAddress", default=None
     )
@@ -145,16 +139,17 @@
     # could be reused as a private_key_jwt
     # sub: HttpUrl
 
     iss: HttpUrl
     iat: int
     exp: Optional[int]
     jti: Optional[str]
-    aud: List[HttpUrl]
-    acr_values: List[AcrValues]
+    aud: str | List[HttpUrl]
+    acr_values: Optional[List[AcrValues]]
+    prompt: Optional[Literal["consent", "consent login"]]
 
     @validator("claims")
     def validate_claims(cls, claims):
         for k_claim, v_claim in claims.items():
             cl = cls.get_claims()
             claims_items = cl.get(k_claim, None)
             if not claims_items:
@@ -170,15 +165,14 @@
     def validate_scope(cls, scope):
         if "openid" not in scope:
             raise ValueError("'scope' attribute must contain 'openid'")
 
 
 class AuthenticationRequestSpid(AuthenticationRequest):
     scope: List[ScopeSpid]
-    prompt: Literal["consent", "consent login"]
 
     def get_claims() -> dict:
         return CLAIMS_SPID
 
     def example():  # pragma: no cover
         return AuthenticationRequestSpid(  # nosec B106
             client_id= "https://rp.cie.it/callback1/",
@@ -200,15 +194,14 @@
             exp= 1648592200,
             jti= "a72d5df0-2415-4c7c-a44f-3988b354040b",
         )
 
 
 class AuthenticationRequestCie(AuthenticationRequest):
     scope: List[ScopeCie]
-    prompt: Literal["consent", "consent login"]
 
     def get_claims() -> dict:
         return CLAIMS_CIE
 
 
 class AuthenticationRequestDoc(BaseModel):
     client_id: HttpUrl
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/authn_response.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/schemas/authn_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/introspection_response.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/schemas/introspection_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/jwt.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/schemas/jwt.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/token_requests.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/schemas/token_requests.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/schemas/token_response.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/schemas/token_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/settings.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,32 +37,32 @@
 OIDCFED_PROVIDER_ATTRIBUTES_SPID_MAP = {
     "https://attributes.spid.gov.it/spidCode": (
         {
             "func": "spid_cie_oidc.provider.processors.spidCode",
             "kwargs": {"salt": "signiicusenz"},
         },
     ),
-    "https://attributes.spid.gov.it/name": ("name", "given_name"),
-    "https://attributes.spid.gov.it/familyName": ("family_name", "surname"),
-    "https://attributes.spid.gov.it/placeOfBirth": ("place_of_birth",),
-    "https://attributes.spid.gov.it/countyOfBirth": ("county_of_birth",),
-    "https://attributes.spid.gov.it/dateOfBirth": ("date_of_birth", "birthdate"),
-    "https://attributes.spid.gov.it/gender": ("gender",),
+    "given_name": ("name", "given_name"),
+    "family_name": ("family_name", "surname"),
+    "place_of_birth": ("place_of_birth",),
+    "county_of_birth": ("county_of_birth",),
+    "date_of_birth": ("date_of_birth", "birthdate"),
+    "gender": ("gender",),
     "https://attributes.spid.gov.it/companyName": ("company_name",),
     "https://attributes.spid.gov.it/registeredOffice": ("registered_office",),
-    "https://attributes.spid.gov.it/fiscalNumber": ("fiscal_number", "tin"),
+    "https://attributes.spid.gov.it/fiscal_number": ("fiscal_number", "tin"),
     "https://attributes.spid.gov.it/ivaCode": ("iva_code",),
     "https://attributes.spid.gov.it/idCard": ("id_card",),
     "https://attributes.spid.gov.it/mobilePhone": (
         "mobile_phone",
         "phone",
         "telephone",
     ),
-    "https://attributes.spid.gov.it/email": ("email",),
-    "https://attributes.spid.gov.it/address": ("address",),
+    "email": ("email",),
+    "address": ("address",),
     "https://attributes.spid.gov.it/expirationDate": ("expiration_date",),
     "https://attributes.spid.gov.it/digitalAddress": ("digital_address",),
 }
 
 OIDCFED_PROVIDER_ATTRIBUTES_CIE_MAP = {
     "given_name": ("name", "given_name"),
     "family_name": ("family_name", "surname"),
@@ -160,28 +160,27 @@
         cie = [AcrValues.l1.value]
     )
 )
 
 
 OIDCFED_ATTRNAME_I18N = {
     # SPID
-    "https://attributes.spid.gov.it/name": _("Name"),
-    "https://attributes.spid.gov.it/familyName": _("Family name"),
-    "https://attributes.spid.gov.it/placeOfBirth": _("Place of birth"),
-    "https://attributes.spid.gov.it/countyOfBirth": _("County of birth",),
-    "https://attributes.spid.gov.it/dateOfBirth": _("Date of birth"),
-    "https://attributes.spid.gov.it/gender": _("Gender"),
+    "given_name": _("Name"),
+    "family_name": _("Family name"),
+    "place_of_birth": _("Place of birth"),
+    "date_of_birth": _("Date of birth"),
+    "gender": _("Gender"),
     "https://attributes.spid.gov.it/companyName": _("Company Name"),
     "https://attributes.spid.gov.it/registeredOffice": _("Registered Office"),
-    "https://attributes.spid.gov.it/fiscalNumber": _("Tax payer id"),
+    "https://attributes.spid.gov.it/fiscal_number": _("Tax payer id"),
     "https://attributes.spid.gov.it/ivaCode": _("Vat number"),
     "https://attributes.spid.gov.it/idCard": _("Id card"),
     "https://attributes.spid.gov.it/mobilePhone": _("Mobile phone"),
-    "https://attributes.spid.gov.it/email": _("Email"),
-    "https://attributes.spid.gov.it/address": _("Address"),
+    "email": _("Email"),
+    "address": _("Address"),
     "https://attributes.spid.gov.it/expirationDate": _("Expiration date"),
     "https://attributes.spid.gov.it/digitalAddress": _("Digital address"),
 
     # CIE
     "given_name": _("Name"),
     "family_name": _("Family name"),
     "email": _("Email"),
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/css/provider.css` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/static/css/provider.css`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/images/logo-cie.png` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/static/images/logo-cie.png`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/svg/cie-ico-circle-bb.svg` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/static/svg/cie-ico-circle-bb.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/svg/logo-cie.svg` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/static/svg/logo-cie.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/svg/spid-ico-circle-bb.svg` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/static/svg/spid-ico-circle-bb.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/static/svg/spid-logo-c-lb.svg` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/static/svg/spid-logo-c-lb.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templates/op_base.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/templates/op_base.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templates/op_user_consent.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/templates/op_user_consent.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templates/op_user_history.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/templates/op_user_history.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templates/op_user_login.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/templates/op_user_login.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/templatetags/spid_cie_op.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/templatetags/spid_cie_op.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/authn_request_settings.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/authn_request_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 # TODO: we need factory function to get fresh now
 IAT = iat_now()
 EXP = exp_from_now()
 
 CLAIMS_SPID = {
     "userinfo": {
-        "https://attributes.spid.gov.it/name": {"values": ["str", "str"]},
-        "https://attributes.spid.gov.it/familyName": None,
-        "https://attributes.spid.gov.it/dateOfBirth": {"value": "str"},
+        "given_name": {"values": ["str", "str"]},
+        "family_name": None,
+        "date_of_birth": {"value": "str"},
     },
 }
 
 CLAIMS_CIE = {
     "userinfo": {
         "given_name": {"values": ["str", "str"]},
         "family_name": None,
@@ -49,15 +49,15 @@
 }
 
 AUTHN_REQUEST_SPID_NO_CLIENT_ID = deepcopy(AUTHN_REQUEST_SPID)
 AUTHN_REQUEST_SPID_NO_CLIENT_ID.pop("client_id")
 
 AUTHN_REQUEST_SPID_NO_CORRECT_CLAIMS = deepcopy(AUTHN_REQUEST_SPID)
 AUTHN_REQUEST_SPID_NO_CORRECT_CLAIMS["claims"]["userinfo"][
-    "https://attributes.spid.gov.it/name"
+    "given_name"
 ]["values"] = ["str"]
 
 AUTHN_REQUEST_SPID_NO_CODE_CHALLENGE = deepcopy(AUTHN_REQUEST_SPID)
 AUTHN_REQUEST_SPID_NO_CODE_CHALLENGE.pop("code_challenge")
 
 AUTHN_REQUEST_SPID_NO_CODE_CHALLENGE_METHOD = deepcopy(AUTHN_REQUEST_SPID)
 AUTHN_REQUEST_SPID_NO_CODE_CHALLENGE_METHOD.pop("code_challenge_method")
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/authn_responses_settings.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/authn_responses_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/introspection_request_settings.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/introspection_request_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/introspection_response_settings.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/introspection_response_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/revocation_request_settings.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/revocation_request_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/revocation_response_settings.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/revocation_response_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/settings.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,43 +17,42 @@
     "jwks_core": [op_conf_priv_jwk],
     "trust_marks": [],
     "trust_marks_issuers": {},
     "entity_type": "openid_provider",
     "metadata": {
         "openid_provider": {
             "authorization_endpoint": "http://op-test/oidc/op/authorization/",
-            "token_endpoint": "http://op-test/oidc/op/token/",
+            "token_endpoint": "http://op-test/oidc/op/token",
             "userinfo_endpoint": "http://op-test/oidc/op/userinfo/",
             "introspection_endpoint": "http://op-test/oidc/op/introspection/",
             "revocation_endpoint": "http://op-test/oidc/op/revocation/",
             "claims_parameter_supported": True,
             "contacts": ["ops@op-test.it"],
             "client_registration_types_supported": ["automatic"],
             "request_authentication_methods_supported": {"ar": ["request_object"]},
             "acr_values_supported": [
                 "https://www.spid.gov.it/SpidL1",
                 "https://www.spid.gov.it/SpidL2",
                 "https://www.spid.gov.it/SpidL3",
             ],
             "claims_supported": [
                 "https://attributes.spid.gov.it/spidCode",
-                "https://attributes.spid.gov.it/name",
-                "https://attributes.spid.gov.it/familyName",
-                "https://attributes.spid.gov.it/placeOfBirth",
-                "https://attributes.spid.gov.it/countyOfBirth",
-                "https://attributes.spid.gov.it/dateOfBirth",
-                "https://attributes.spid.gov.it/gender",
+                "given_name",
+                "family_name",
+                "place_of_birth",
+                "date_of_birth",
+                "gender",
                 "https://attributes.spid.gov.it/companyName",
                 "https://attributes.spid.gov.it/registeredOffice",
-                "https://attributes.spid.gov.it/fiscalNumber",
+                "https://attributes.spid.gov.it/fiscal_number",
                 "https://attributes.spid.gov.it/ivaCode",
                 "https://attributes.spid.gov.it/idCard",
                 "https://attributes.spid.gov.it/mobilePhone",
-                "https://attributes.spid.gov.it/email",
-                "https://attributes.spid.gov.it/address",
+                "email",
+                "address",
                 "https://attributes.spid.gov.it/expirationDate",
                 "https://attributes.spid.gov.it/digitalAddress",
             ],
             "grant_types_supported": ["authorization_code", "refresh_token"],
             "id_token_signing_alg_values_supported": ["RS256", "ES256"],
             "issuer": "http://op-test/oidc/op/",
             "jwks": {
@@ -132,8 +131,8 @@
                 "ES384",
                 "ES512",
             ],
         }
     },
     "constraints": {},
     "is_active": True,
-}
+}
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_02_authn_endpoint.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_02_authn_endpoint.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,25 +74,25 @@
             jwks = [],
             metadata=RP_METADATA,
             status="valid",
             trust_anchor=self.ta_fes,
             is_active=True,
         )
 
-    @override_settings(OIDCFED_DEFAULT_TRUST_ANCHOR=TA_SUB)
+    @override_settings(OIDCFED_TRUST_ANCHORS=[TA_SUB])
     def test_auth_request_unknown_error(self):
         jws = create_jws(self.REQUEST_OBJECT_PAYLOAD, RP_METADATA_JWK1)
         client = Client()
         TrustChain.objects.all().delete()
         url = reverse("oidc_provider_authnrequest")
         res = client.get(url, {"request": jws})
         self.assertTrue(res.status_code == 302)
         self.assertTrue("error=invalid_request" in res.url)
 
-    @override_settings(OIDCFED_DEFAULT_TRUST_ANCHOR=TA_SUB)
+    @override_settings(OIDCFED_TRUST_ANCHORS=[TA_SUB])
     @override_settings(OIDCFED_DEFAULT_PROVIDER_PROFILE="cie")
     def test_auth_request_id_token_claim(self):
         jws = create_jws(self.REQUEST_OBJECT_PAYLOAD, RP_METADATA_JWK1)
         client = Client()
         url = reverse("oidc_provider_authnrequest")
         res = client.get(url, {"request": jws})
         self.assertTrue(res.status_code == 200)
@@ -111,22 +111,22 @@
         issued_token = IssuedToken.objects.all().first()
         verify_jws(issued_token.id_token, op_conf_priv_jwk)
         id_token = unpad_jwt_payload(issued_token.id_token)
         self.assertEqual(id_token.get("family_name"), "rossi")
         self.assertEqual(id_token.get("email"), "test@test.it")
 
 
-    @override_settings(OIDCFED_DEFAULT_TRUST_ANCHOR=TA_SUB)
+    @override_settings(OIDCFED_TRUST_ANCHORS=[TA_SUB])
     def test_auth_no_request(self):
         client = Client()
         url = reverse("oidc_provider_authnrequest")
         res = client.get(url, {})
         self.assertTrue(res.status_code == 400)
 
-    @override_settings(OIDCFED_DEFAULT_TRUST_ANCHOR=TA_SUB)
+    @override_settings(OIDCFED_TRUST_ANCHORS=[TA_SUB])
     def test_auth_request_ok(self):
         jws = create_jws(self.REQUEST_OBJECT_PAYLOAD, RP_METADATA_JWK1)
         client = Client()
         url = reverse("oidc_provider_authnrequest")
         res = client.get(url, {"request": jws})
         self.assertTrue(res.status_code == 200)
         self.assertIn("username", res.content.decode())
@@ -140,15 +140,15 @@
         res = client.get(consent_page_url)
         self.assertTrue("agree" in res.content.decode())
         self.assertFalse("error" in res.content.decode())
         res = client.post(consent_page_url, {"agree": True})
         self.assertTrue(res.status_code == 302)
         self.assertTrue("code" in res.url)
 
-    @override_settings(OIDCFED_DEFAULT_TRUST_ANCHOR=TA_SUB)
+    @override_settings(OIDCFED_TRUST_ANCHORS=[TA_SUB])
     def test_auth_request_user_rejected_consent(self):
         jws = create_jws(self.REQUEST_OBJECT_PAYLOAD, RP_METADATA_JWK1)
         client = Client()
         url = reverse("oidc_provider_authnrequest")
         res = client.get(url, {"request": jws})
         self.assertTrue(res.status_code == 200)
         self.assertIn("username", res.content.decode())
@@ -163,15 +163,15 @@
         self.assertTrue("agree" in res.content.decode())
         self.assertFalse("error" in res.content.decode())
         res = client.post(consent_page_url, {"agree": False})
         self.assertTrue(res.status_code == 302)
         # TODO: this is not normative
         self.assertTrue("error=rejected_by_user" in res.url)
 
-    @override_settings(OIDCFED_DEFAULT_TRUST_ANCHOR=TA_SUB)
+    @override_settings(OIDCFED_TRUST_ANCHORS=[TA_SUB])
     def test_auth_request_no_session_in_post_consent(self):
         jws = create_jws(self.REQUEST_OBJECT_PAYLOAD, RP_METADATA_JWK1)
         client = Client()
         url = reverse("oidc_provider_authnrequest")
         res = client.get(url, {"request": jws})
         self.assertTrue(res.status_code == 200)
         self.assertIn("username", res.content.decode())
@@ -185,15 +185,15 @@
         res = client.get(consent_page_url)
         self.assertTrue("agree" in res.content.decode())
         self.assertFalse("error" in res.content.decode())
         OidcSession.objects.all().delete()
         res = client.post(consent_page_url, {"agree": True})
         self.assertTrue(res.status_code == 403)
 
-    @override_settings(OIDCFED_DEFAULT_TRUST_ANCHOR=TA_SUB)
+    @override_settings(OIDCFED_TRUST_ANCHORS=[TA_SUB])
     def test_auth_request_no_session_in_get_consent(self):
         jws = create_jws(self.REQUEST_OBJECT_PAYLOAD, RP_METADATA_JWK1)
         client = Client()
         url = reverse("oidc_provider_authnrequest")
         res = client.get(url, {"request": jws})
         self.assertTrue(res.status_code == 200)
         self.assertIn("username", res.content.decode())
@@ -209,15 +209,15 @@
         self.assertFalse("error" in res.content.decode())
         self.assertTrue(res.status_code == 302)
         consent_page_url = res.url
         OidcSession.objects.all().delete()
         res = client.get(consent_page_url)
         self.assertTrue(res.status_code == 403)
 
-    @override_settings(OIDCFED_DEFAULT_TRUST_ANCHOR=TA_SUB)
+    @override_settings(OIDCFED_TRUST_ANCHORS=[TA_SUB])
     def test_auth_request_auth_code_already_used(self):
         jws = create_jws(self.REQUEST_OBJECT_PAYLOAD, RP_METADATA_JWK1)
         client = Client()
         url = reverse("oidc_provider_authnrequest")
         res = client.get(url, {"request": jws})
         self.assertTrue(res.status_code == 200)
         self.assertIn("username", res.content.decode())
@@ -229,29 +229,29 @@
         self.assertTrue(res.status_code == 302)
         session = OidcSession.objects.all().first()
         IssuedToken.objects.create(session=session, expires=timezone.localtime())
         consent_page_url = res.url
         res = client.get(consent_page_url)
         self.assertTrue(res.status_code == 403)
 
-    @override_settings(OIDCFED_DEFAULT_TRUST_ANCHOR=TA_SUB)
+    @override_settings(OIDCFED_TRUST_ANCHORS=[TA_SUB])
     def test_auth_request_wrong_login(self):
         jws = create_jws(self.REQUEST_OBJECT_PAYLOAD, RP_METADATA_JWK1)
         client = Client()
         url = reverse("oidc_provider_authnrequest")
         res = client.get(url, {"request": jws})
         self.assertTrue(res.status_code == 200)
         self.assertIn("username", res.content.decode())
         self.assertIn("password", res.content.decode())
         res = client.post(
             url, {"username": "notest", "password": "test", "authz_request_object": jws}
         )
         self.assertIn("error", res.content.decode())
 
-    @override_settings(OIDCFED_DEFAULT_TRUST_ANCHOR=TA_SUB)
+    @override_settings(OIDCFED_TRUST_ANCHORS=[TA_SUB])
     def test_auth_request_preexistent_authz(self):
         jws = create_jws(self.REQUEST_OBJECT_PAYLOAD, RP_METADATA_JWK1)
         client = Client()
         url = reverse("oidc_provider_authnrequest")
         res = client.get(url, {"request": jws})
         self.assertTrue(res.status_code == 200)
         self.assertIn("username", res.content.decode())
@@ -260,27 +260,27 @@
             url, {"username": "test", "password": "test", "authz_request_object": jws}
         )
         res = client.get(url, {"request": jws})
         self.assertTrue(res.status_code == 302)
         self.assertIn("error=invalid_request", res.url)
         self.assertIn("state", res.url)
 
-    @override_settings(OIDCFED_DEFAULT_TRUST_ANCHOR=TA_SUB)
+    @override_settings(OIDCFED_TRUST_ANCHORS=[TA_SUB])
     def test_auth_request_trust_chain_no_active(self):
         self.trust_chain.is_active = False
         self.trust_chain.save()
         jws = create_jws(self.REQUEST_OBJECT_PAYLOAD, RP_METADATA_JWK1)
         client = Client()
         url = reverse("oidc_provider_authnrequest")
         res = client.get(url, {"request": jws})
         self.assertTrue(res.status_code == 302)
         self.assertIn("error=invalid_request", res.url)
         self.assertIn("state", res.url)
 
-    @override_settings(OIDCFED_DEFAULT_TRUST_ANCHOR=TA_SUB)
+    @override_settings(OIDCFED_TRUST_ANCHORS=[TA_SUB])
     def test_auth_request_invalid_jwk(self):
         jws = create_jws(self.REQUEST_OBJECT_PAYLOAD, RP_METADATA_JWK1)
         get_jwks(self.trust_chain.metadata['openid_relying_party'])[0][
             "kid"
         ] = "31ALfVXx9dcAMMHCVvh42qLTlanBL_r6BTnD5uMDzFT"
         self.trust_chain.save()
         client = Client()
@@ -290,60 +290,60 @@
         self.assertIn("error=invalid_request", res.url)
         self.assertIn("state", res.url)
         get_jwks(self.trust_chain.metadata['openid_relying_party'])[0][
             "kid"
         ] = RP_METADATA_JWK1['kid']
         self.trust_chain.save()
 
-    @override_settings(OIDCFED_DEFAULT_TRUST_ANCHOR=TA_SUB)
+    @override_settings(OIDCFED_TRUST_ANCHORS=[TA_SUB])
     def test_auth_request_no_correct_payload(self):
         NO_CORRECT_OBJECT_PAYLOAD = deepcopy(self.REQUEST_OBJECT_PAYLOAD)
         NO_CORRECT_OBJECT_PAYLOAD["response_type"] = "test"
         jws = create_jws(NO_CORRECT_OBJECT_PAYLOAD, RP_METADATA_JWK1)
         client = Client()
         url = reverse("oidc_provider_authnrequest")
         res = client.get(url, {"request": jws})
         self.assertTrue(res.status_code == 302)
         self.assertIn("error", res.url)
         self.assertIn("state", res.url)
 
-    @override_settings(OIDCFED_DEFAULT_TRUST_ANCHOR=TA_SUB)
+    @override_settings(OIDCFED_TRUST_ANCHORS=[TA_SUB])
     def test_auth_request_invalid_session(self):
         client = Client()
         url = reverse("oidc_provider_consent")
         res = client.get(url)
         self.assertTrue(res.status_code == 403)
         res = client.post(url)
         self.assertTrue(res.status_code == 403)
 
-    @override_settings(OIDCFED_DEFAULT_TRUST_ANCHOR=TA_SUB)
+    @override_settings(OIDCFED_TRUST_ANCHORS=[TA_SUB])
     def test_auth_request_no_correct_refresh_request(self):
         local_payload = deepcopy(self.REQUEST_OBJECT_PAYLOAD)
         local_payload["scope"] = "openid offline_access"
         local_payload["prompt"] = "login"
         jws = create_jws(local_payload, RP_METADATA_JWK1)
         client = Client()
         url = reverse("oidc_provider_authnrequest")
         res = client.get(url, {"request": jws})
         self.assertTrue(res.status_code == 403)
     
-    @override_settings(OIDCFED_DEFAULT_TRUST_ANCHOR=TA_SUB)
+    @override_settings(OIDCFED_TRUST_ANCHORS=[TA_SUB])
     def test_auth_request_user_staff(self):
         self.user.is_staff = True
         self.user.save()
         jws = create_jws(self.REQUEST_OBJECT_PAYLOAD, RP_METADATA_JWK1)
         client = Client()
         url = reverse("oidc_provider_authnrequest")
         res = client.post(
             url, {"username": "test", "password": "test", "authz_request_object": jws}
         )
         self.assertTrue(res.status_code == 302)
         self.assertTrue("/oidc/op/rp-test/landing/" == res.url)
 
-    @override_settings(OIDCFED_DEFAULT_TRUST_ANCHOR=TA_SUB)
+    @override_settings(OIDCFED_TRUST_ANCHORS=[TA_SUB])
     def test_auth_request_no_correct_authz_request(self):
         self.user.is_staff = True
         self.user.save()
         create_jws(self.REQUEST_OBJECT_PAYLOAD, RP_METADATA_JWK1)
         client = Client()
         url = reverse("oidc_provider_authnrequest")
         res = client.post(
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_03_authn_request.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_03_authn_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,30 +12,28 @@
     AUTHN_REQUEST_CIE_NO_ACR_VALUES,
     AUTHN_REQUEST_CIE_NO_CORRECT_ACR_VALUES,
     AUTHN_REQUEST_CIE_NO_CORRECT_PROMPT,
     AUTHN_REQUEST_CIE_NO_CORRECT_SCOPE,
     AUTHN_REQUEST_CIE_NO_PROMPT,
     AUTHN_REQUEST_CIE_NO_SCOPE,
     AUTHN_REQUEST_SPID,
-    AUTHN_REQUEST_SPID_NO_ACR_VALUES,
     AUTHN_REQUEST_SPID_NO_CLIENT_ID,
     AUTHN_REQUEST_SPID_NO_CODE_CHALLENGE,
     AUTHN_REQUEST_SPID_NO_CODE_CHALLENGE_METHOD,
     AUTHN_REQUEST_SPID_NO_CORRECT_ACR_VALUES,
     AUTHN_REQUEST_SPID_NO_CORRECT_CLAIMS,
     AUTHN_REQUEST_SPID_NO_CORRECT_CODE_CHALLENGE_METHOD,
     AUTHN_REQUEST_SPID_NO_CORRECT_NONCE,
     AUTHN_REQUEST_SPID_NO_CORRECT_PROMPT,
     AUTHN_REQUEST_SPID_NO_CORRECT_REDIRECT_URL,
     AUTHN_REQUEST_SPID_NO_CORRECT_RESPONSE_TYPE,
     AUTHN_REQUEST_SPID_NO_CORRECT_SCOPE,
     AUTHN_REQUEST_SPID_NO_CORRECT_STATE,
     AUTHN_REQUEST_SPID_NO_CORRECT_UI_LOCALES,
     AUTHN_REQUEST_SPID_NO_NONCE,
-    AUTHN_REQUEST_SPID_NO_PROMPT,
     AUTHN_REQUEST_SPID_NO_REDIRECT_URL,
     AUTHN_REQUEST_SPID_NO_RESPONSE_TYPE,
     AUTHN_REQUEST_SPID_NO_SCOPE,
     AUTHN_REQUEST_SPID_NO_STATE,
 )
 
 logger = logging.getLogger(__name__)
@@ -70,18 +68,19 @@
     def test_validate_spid_no_nonce(self):
         with self.assertRaises(ValidationError):
             AuthenticationRequestSpid(**AUTHN_REQUEST_SPID_NO_NONCE)
 
     def test_validate_spid_no_correct_nonce(self):
         with self.assertRaises(ValidationError):
             AuthenticationRequestSpid(**AUTHN_REQUEST_SPID_NO_CORRECT_NONCE)
-
-    def test_validate_spid_no_prompt(self):
-        with self.assertRaises(ValidationError):
-            AuthenticationRequestSpid(**AUTHN_REQUEST_SPID_NO_PROMPT)
+    
+    # removed, relaxed with the GAIN-PoC integration
+    #  def test_validate_spid_no_prompt(self):
+        #  with self.assertRaises(ValidationError):
+            #  AuthenticationRequestSpid(**AUTHN_REQUEST_SPID_NO_PROMPT)
 
     def test_validate_spid_no_correct_prompt(self):
         with self.assertRaises(ValidationError):
             AuthenticationRequestSpid(**AUTHN_REQUEST_SPID_NO_CORRECT_PROMPT)
 
     def test_validate_spid_no_redirect_url(self):
         with self.assertRaises(ValidationError):
@@ -103,17 +102,17 @@
         with self.assertRaises(ValidationError):
             AuthenticationRequestSpid(**AUTHN_REQUEST_SPID_NO_SCOPE)
 
     def test_validate_spid_no_correct_scope(self):
         with self.assertRaises(ValidationError):
             AuthenticationRequestSpid(**AUTHN_REQUEST_SPID_NO_CORRECT_SCOPE)
 
-    def test_validate_spid_no_acr_values(self):
-        with self.assertRaises(ValidationError):
-            AuthenticationRequestSpid(**AUTHN_REQUEST_SPID_NO_ACR_VALUES)
+#    def test_validate_spid_no_acr_values(self):
+#        with self.assertRaises(ValidationError):
+#            AuthenticationRequestSpid(**AUTHN_REQUEST_SPID_NO_ACR_VALUES)
 
     def test_validate_spid_no_correct_acr_values(self):
         with self.assertRaises(ValidationError):
             AuthenticationRequestSpid(**AUTHN_REQUEST_SPID_NO_CORRECT_ACR_VALUES)
 
     def test_validate_spid_no_state(self):
         with self.assertRaises(ValidationError):
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_03_refresh_token.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_03_refresh_token.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,51 +8,51 @@
     RP_METADATA,
     RP_METADATA_JWK1,
     rp_conf
 )
 from spid_cie_oidc.entity.jwtse import create_jws, verify_jws
 from spid_cie_oidc.entity.models import (
     FederationEntityConfiguration,
-    FetchedEntityStatement, 
+    FetchedEntityStatement,
     TrustChain
 )
 from spid_cie_oidc.entity.tests.settings import TA_SUB
 from spid_cie_oidc.entity.utils import (
-    datetime_from_timestamp, 
+    datetime_from_timestamp,
     exp_from_now,
     iat_now
 )
 from spid_cie_oidc.provider.models import IssuedToken, OidcSession
 from spid_cie_oidc.provider.tests.settings import op_conf, op_conf_priv_jwk
 
 RP_SUB = rp_conf["sub"]
 RP_CLIENT_ID = rp_conf["metadata"]["openid_relying_party"]["client_id"]
 
-class RefreshTokenTest(TestCase):
 
+class RefreshTokenTest(TestCase):
 
-    def setUp(self): 
+    def setUp(self):
         self.op_local_conf = deepcopy(op_conf)
         FederationEntityConfiguration.objects.create(**self.op_local_conf)
         self.ta_fes = FetchedEntityStatement.objects.create(
             sub=TA_SUB,
             iss=TA_SUB,
             exp=datetime_from_timestamp(exp_from_now(33)),
             iat=datetime_from_timestamp(iat_now()),
         )
         self.trust_chain = TrustChain.objects.create(
             sub=RP_SUB,
             exp=datetime_from_timestamp(exp_from_now(33)),
-            jwks = [],
+            jwks=[],
             metadata=RP_METADATA,
             status="valid",
             trust_anchor=self.ta_fes,
             is_active=True,
         )
-        self.jwt_auds = [op_conf["sub"], "http://testserver/oidc/op/", "http://testserver/oidc/op/token/"]
+        self.jwt_auds = [op_conf["sub"], "http://testserver/oidc/op/", "http://testserver/oidc/op/token"]
         CLIENT_ASSERTION = {
             "iss": RP_SUB,
             "sub": RP_SUB,
             "aud": self.jwt_auds,
             "exp": exp_from_now(),
             "iat": iat_now(),
             "jti": "jti",
@@ -63,65 +63,59 @@
             "sub": RP_SUB,
             "aud": self.jwt_auds,
             "client_id": RP_CLIENT_ID,
             "scope": "openid",
         }
         self.rt_jws = create_jws(refresh_token, op_conf_priv_jwk)
         session = OidcSession.objects.create(
-            user=User.objects.create(username = "username"),
+            user=User.objects.create(username="username"),
             user_uid="",
             nonce="",
-            authz_request={"scope": "offline_access", "prompt": "consent", "nonce": "123", "acr_values":["https://www.spid.gov.it/SpidL2"]},
-            client_id="",
+            authz_request={"scope": "offline_access", "prompt": "consent", "nonce": "123",
+                           "acr_values": ["https://www.spid.gov.it/SpidL2", "https://www.spid.gov.it/SpidL1"]},
+            client_id=RP_SUB,
             auth_code="code",
         )
         IssuedToken.objects.create(
-            refresh_token = self.rt_jws,
-            session = session,
-            expires = timezone.localtime()
+            refresh_token=self.rt_jws,
+            session=session,
+            expires=timezone.localtime()
         )
 
     def test_grant_refresh_token(self):
         client = Client()
         url = reverse("oidc_provider_token_endpoint")
         request = dict(
-            client_id = RP_CLIENT_ID,
-            client_assertion = self.ca_jws,
-            client_assertion_type = "urn:ietf:params:oauth:client-assertion-type:jwt-bearer",
-            refresh_token = self.rt_jws,
-            grant_type="refresh_token",
-            code = "code",
-            code_verifier = "code_verifier"
-
+            client_id=RP_CLIENT_ID,
+            client_assertion=self.ca_jws,
+            client_assertion_type="urn:ietf:params:oauth:client-assertion-type:jwt-bearer",
+            refresh_token=self.rt_jws,
+            grant_type="refresh_token"
         )
         res = client.post(url, request)
         self.assertTrue(res.status_code == 200)
         refresh_token = verify_jws(res.json().get("refresh_token"), op_conf_priv_jwk)
-        self.assertEqual(refresh_token["sub"], RP_SUB)
+        self.assertEqual(refresh_token["aud"], RP_CLIENT_ID)
+        self.assertEqual(refresh_token["iss"], self.op_local_conf["sub"])
 
-    @override_settings(OIDCFED_PROVIDER_MAX_REFRESH = 1)
+    @override_settings(OIDCFED_PROVIDER_MAX_REFRESH=1)
     def test_grant_refresh_token_two_times(self):
         client = Client()
         url = reverse("oidc_provider_token_endpoint")
         request = dict(
-            client_id = RP_CLIENT_ID,
-            client_assertion = self.ca_jws,
-            client_assertion_type = "urn:ietf:params:oauth:client-assertion-type:jwt-bearer",
-            refresh_token = self.rt_jws,
-            grant_type="refresh_token",
-            code = "code",
-            code_verifier = "code_verifier"
+            client_id=RP_CLIENT_ID,
+            client_assertion=self.ca_jws,
+            client_assertion_type="urn:ietf:params:oauth:client-assertion-type:jwt-bearer",
+            refresh_token=self.rt_jws,
+            grant_type="refresh_token"
         )
         res = client.post(url, request)
         self.assertTrue(res.status_code == 200)
         request = dict(
-            client_id = RP_CLIENT_ID,
-            client_assertion = self.ca_jws,
-            client_assertion_type = "urn:ietf:params:oauth:client-assertion-type:jwt-bearer",
-            refresh_token = res.json()["refresh_token"],
-            grant_type="refresh_token",
-            code = "code",
-            code_verifier = "code_verifier"
+            client_id=RP_CLIENT_ID,
+            client_assertion=self.ca_jws,
+            client_assertion_type="urn:ietf:params:oauth:client-assertion-type:jwt-bearer",
+            refresh_token=res.json()["refresh_token"],
+            grant_type="refresh_token"
         )
         res = client.post(url, request)
         self.assertTrue(res.status_code == 400)
-
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_04_authn_response.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_04_authn_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_04_userinfo_endpoint.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_04_userinfo_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_05_introspection_endpoint.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_05_introspection_endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 class IntrospectionEndpointTest(TestCase):
 
     def setUp(self):
         self.RP_SUB = rp_conf["sub"]
         self.RP_CLIENT_ID = rp_conf["metadata"]["openid_relying_party"]["client_id"]
-        self.jwt_auds = [op_conf["sub"], "http://testserver/oidc/op/", "http://testserver/oidc/op/introspection/"]
+        self.jwt_auds = [op_conf["sub"], "http://testserver/oidc/op/", "http://testserver/oidc/op/introspection"]
         CLIENT_ASSERTION = {
             "iss": self.RP_SUB,
             "sub": self.RP_SUB,
             "aud": self.jwt_auds,
             "exp": exp_from_now(),
             "iat": iat_now(),
             "jti": "jti",
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_05_token_request.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_05_token_request.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_06_token_response.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_06_token_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_07_fetch_relying_parties.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_07_fetch_relying_parties.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_07_introspection_request.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_07_introspection_request.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_08_introspection_response.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_08_introspection_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_08_token_endpoint.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_08_token_endpoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             exp=datetime_from_timestamp(exp_from_now(33)),
             jwks = [],
             metadata=RP_METADATA,
             status="valid",
             trust_anchor=self.ta_fes,
             is_active=True,
         )
-        self.jwt_auds = [op_conf["sub"], "http://testserver/oidc/op/", "http://testserver/oidc/op/token/"]
+        self.jwt_auds = [op_conf["sub"], "http://testserver/oidc/op/", "http://testserver/oidc/op/token"]
         CLIENT_ASSERTION = {
             "iss": RP_SUB,
             "sub": RP_SUB,
             "aud": self.jwt_auds,
             "exp": exp_from_now(),
             "iat": iat_now(),
             "jti": "jti",
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_09_revocation_endpoint.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_09_revocation_endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             sub=TA_SUB,
             iss=TA_SUB,
             exp=datetime_from_timestamp(exp_from_now(33)),
             iat=datetime_from_timestamp(iat_now()),
         )
         self.op_local_conf = deepcopy(op_conf)
         FederationEntityConfiguration.objects.create(**self.op_local_conf)
-        self.jwt_auds = [op_conf["sub"], "http://testserver/oidc/op/", "http://testserver/oidc/op/revocation/"]
+        self.jwt_auds = [op_conf["sub"], "http://testserver/oidc/op/", "http://testserver/oidc/op/revocation"]
         CLIENT_ASSERTION = {
             "iss": RP_SUB,
             "sub": RP_SUB,
             "aud": self.jwt_auds,
             "exp": exp_from_now(),
             "iat": iat_now(),
             "jti": "jti",
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_09_revocation_request.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_09_revocation_request.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_10_no_consent.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_10_no_consent.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_10_revocation_response.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_10_revocation_response.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_11_user_access_history.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_11_user_access_history.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,70 @@
-
 from django.contrib.auth import get_user_model
 from django.test import Client, TestCase
 from django.urls import reverse
 from spid_cie_oidc.authority.tests.settings import rp_conf
 from spid_cie_oidc.provider.models import OidcSession
 
 
 class UserAccessHistoryTest(TestCase):
 
-    def setUp(self): 
+    def setUp(self):
         self.user = get_user_model().objects.create(
             username="test",
             first_name="test",
             last_name="test",
             email="test@test.it",
-            is_staff = True
+            is_staff=True
         )
         self.user.set_password("test")
         self.user.save()
         OidcSession.objects.create(
             user=self.user,
             user_uid="uid",
             nonce="",
             authz_request={
-                "scope": "openid", 
-                "nonce": "123", 
-                "acr_values" : ["https://www.spid.gov.it/SpidL2"],            
-                "redirect_uri" : rp_conf["metadata"]["openid_relying_party"]["redirect_uris"][0],
-                "state" : "state",
+                "scope": "openid",
+                "nonce": "123",
+                "acr_values": ["https://www.spid.gov.it/SpidL2"],
+                "redirect_uri": rp_conf["metadata"]["openid_relying_party"]["redirect_uris"][0],
+                "state": "state",
             },
             client_id="",
             auth_code="auth_code",
         )
         OidcSession.objects.create(
             user=self.user,
             user_uid="uid",
             nonce="1234",
             authz_request={
-                "scope": "openid", 
-                "nonce": "1234", 
-                "acr_values" : ["https://www.spid.gov.it/SpidL2"],            
-                "redirect_uri" : rp_conf["metadata"]["openid_relying_party"]["redirect_uris"][0],
-                "state" : "state",
+                "scope": "openid",
+                "nonce": "1234",
+                "acr_values": ["https://www.spid.gov.it/SpidL2"],
+                "redirect_uri": rp_conf["metadata"]["openid_relying_party"]["redirect_uris"][0],
+                "state": "state",
             },
             client_id="",
             auth_code="code",
         )
 
-
     def test_user_access_history(self):
         client = Client()
         client.login(username="test", password="test")
         session = client.session
-        session.update({"oidc": {"auth_code": "code"}, "user_uid" : "uid"})
+        session.update({"oidc": {"auth_code": "code"}, "user_uid": "uid"})
         session.save()
         url = reverse("oidc_provider_access_history")
         res = client.get(url)
         self.assertTrue(res.status_code == 200)
         self.assertTrue("auth_code=auth_code" in res.content.decode())
 
     def test_user_access_history_revoke(self):
         client = Client()
         client.login(username="test", password="test")
         session = client.session
-        session.update({"oidc": {"auth_code": "code"}, "user_uid" : "uid"})
+        session.update({"oidc": {"auth_code": "code"}, "user_uid": "uid"})
         session.save()
         url = reverse("oidc_provider_revoke_session")
         res = client.get(url, {"auth_code": "auth_code"})
         self.assertTrue(res.status_code == 302)
         url_history = reverse("oidc_provider_access_history")
         self.assertTrue(url_history in res.url)
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/test_12_init.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/test_12_init.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/token_request_settings.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/token_request_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/tests/token_response_settings.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/tests/token_response_settings.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/urls.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/urls.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,84 @@
 from django.conf import settings
 from django.urls import path
 
 from .views.authz_request_view import AuthzRequestView
 from .views.userinfo_endpoint import UserInfoEndpoint
+from spid_cie_oidc.entity.views import (
+    openid_connect_jwks_uri,
+    openid_connect_signed_jwks_uri
+)
+from .views.connect import openid_configuration
 from .views.consent_page_view import (
     ConsentPageView,
     oidc_provider_not_consent,
     UserAccessHistoryView,
     RevokeSessionView,
 )
 from .views.token_endpoint import TokenEndpoint
 from .views.revocation_endpoint import RevocationEndpoint
 from .views.introspection_endpoint import IntrospectionEndpoint
 
 _PREF = getattr(settings, "OIDC_PREFIX", "oidc/op")
 
 urlpatterns = [
     path(
-        f"{_PREF}/authorization/",
+        f"{_PREF}/authorization",
         AuthzRequestView.as_view(),
         name="oidc_provider_authnrequest",
     ),
     path(
-        f"{_PREF}/consent/",
+        f"{_PREF}/consent",
         ConsentPageView.as_view(),
         name="oidc_provider_consent",
     ),
     path(
-        f"{_PREF}/token/",
+        f"{_PREF}/token",
         TokenEndpoint.as_view(),
         name="oidc_provider_token_endpoint",
     ),
     path(
-        f"{_PREF}/userinfo/",
+        f"{_PREF}/userinfo",
         UserInfoEndpoint.as_view(),
         name="oidc_provider_userinfo_endpoint",
     ),
     path(
-        f"{_PREF}/revocation/",
+        f"{_PREF}/revocation",
         RevocationEndpoint.as_view(),
         name="oidc_provider_end_session_endpoint",
     ),
     path(
-        f"{_PREF}/introspection/",
+        f"{_PREF}/introspection",
         IntrospectionEndpoint.as_view(),
         name="oidc_provider_introspection_endpoint",
     ),
     path(
-        f"{_PREF}/notconsent/",
+        f"{_PREF}/notconsent",
         oidc_provider_not_consent,
         name="oidc_provider_not_consent",
     ),
     path(
-        f"{_PREF}/history/",
+        f"{_PREF}/history",
         UserAccessHistoryView.as_view(),
         name="oidc_provider_access_history",
     ),
     path(
-        f"{_PREF}/revoke/",
+        f"{_PREF}/revoke",
         RevokeSessionView.as_view(),
         name="oidc_provider_revoke_session",
     ),
+    path(
+        f"{_PREF}/.well-known/openid-configuration",
+        openid_configuration,
+        name="oidc_provider_openid_configuration",
+    ),
+    path(
+        f"{_PREF}/<str:metadata_type>/jwks.json",
+        openid_connect_jwks_uri,
+        name="oidc_connect_jwks_uri",
+    ),
+    path(
+        f"{_PREF}/<str:metadata_type>/jwks.jose",
+        openid_connect_signed_jwks_uri,
+        name="oidc_connect_signed_jwks_uri",
+    ),
 ]
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/__init__.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/views/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,22 @@
 import urllib
 from spid_cie_oidc.entity.jwtse import create_jws, unpad_jwt_head, unpad_jwt_payload, verify_jws
 from spid_cie_oidc.entity.models import FederationEntityConfiguration, TrustChain
 from spid_cie_oidc.entity.settings import HTTPC_PARAMS
 from spid_cie_oidc.entity.trust_chain_operations import get_or_create_trust_chain
 from spid_cie_oidc.entity.utils import datetime_from_timestamp, exp_from_now, iat_now
 from spid_cie_oidc.entity.utils import get_jwks
-from spid_cie_oidc.provider.exceptions import AuthzRequestReplay, ExpiredAuthCode, InvalidSession, RevokedSession, ValidationException
+from spid_cie_oidc.entity.exceptions import TrustchainMissingMetadata
+from spid_cie_oidc.provider.exceptions import (
+    AuthzRequestReplay,
+    ExpiredAuthCode,
+    InvalidSession,
+    RevokedSession,
+    ValidationException
+)
 from spid_cie_oidc.provider.models import OidcSession
 
 from spid_cie_oidc.provider.settings import (
     OIDCFED_ATTRNAME_I18N,
     OIDCFED_DEFAULT_PROVIDER_PROFILE,
     OIDCFED_PROVIDER_AUTH_CODE_MAX_AGE,
     OIDCFED_PROVIDER_PROFILES,
@@ -28,20 +35,25 @@
 
 class OpBase:
     """
     Baseclass with common methods for OPs
     """
 
     def redirect_response_data(self, redirect_uri:str, **kwargs) -> HttpResponseRedirect:
-        url = f'{redirect_uri}?{urllib.parse.urlencode(kwargs)}'
+        if "?" in redirect_uri:
+            qstring = "&"
+        else:
+            qstring = "?"
+        url = f'{redirect_uri}{qstring}{urllib.parse.urlencode(kwargs)}'
         return HttpResponseRedirect(url)
 
     def find_jwk(self, header: dict, jwks: list) -> dict:
         for jwk in jwks:
-            if header["kid"] == jwk["kid"]:
+            valid_jwk = jwk.get("kid", None)
+            if valid_jwk and header["kid"] == valid_jwk:
                 return jwk
 
     def validate_authz_request_object(self, req) -> TrustChain:
         state = getattr(self, 'payload', {}).get("state", "")
         try:
             self.payload = unpad_jwt_payload(req)
             header = unpad_jwt_head(req)
@@ -54,35 +66,46 @@
             logger.error(_msg)
             raise Exception(_msg)
 
         self.is_a_replay_authz()
         rp_trust_chain = TrustChain.objects.filter(
             metadata__openid_relying_party__isnull=False,
             sub=self.payload["iss"],
-            trust_anchor__sub=settings.OIDCFED_DEFAULT_TRUST_ANCHOR
+            trust_anchor__sub__in=settings.OIDCFED_TRUST_ANCHORS
         ).first()
         if rp_trust_chain and not rp_trust_chain.is_active:
             _msg = (
                 f"Disabled client {rp_trust_chain.sub} requests an authorization. "
                 "error = access_denied, "
                 f"state={state}"
             )
             logger.warning(_msg)
             raise Exception(_msg)
 
         elif not rp_trust_chain or rp_trust_chain.is_expired:
-            rp_trust_chain = get_or_create_trust_chain(
-                subject=self.payload["iss"],
-                trust_anchor=settings.OIDCFED_DEFAULT_TRUST_ANCHOR,
-                httpc_params=HTTPC_PARAMS,
-                required_trust_marks=getattr(
-                    settings, "OIDCFED_REQUIRED_TRUST_MARKS", []
-                ),
-            )
-            if not rp_trust_chain.is_valid:
+            rp_trust_chain = None
+            # TODO: get async here
+            for ta in settings.OIDCFED_TRUST_ANCHORS:
+                try:
+                    rp_trust_chain = get_or_create_trust_chain(
+                        subject=self.payload["iss"],
+                        trust_anchor=ta,
+                        httpc_params=HTTPC_PARAMS,
+                        required_trust_marks=getattr(
+                            settings, "OIDCFED_REQUIRED_TRUST_MARKS", []
+                        ),
+                    )
+                    if rp_trust_chain and rp_trust_chain.metadata:
+                        break
+                except TrustchainMissingMetadata as e:
+                    logger.debug(f"TrustchainMissingMetadata: {e}")
+                    # unless we find the good TA
+                    continue
+
+            if not rp_trust_chain or not rp_trust_chain.is_valid:
                 _msg = (
                     f"Failed trust chain validation for {self.payload['iss']}. "
                     "error=unauthorized_client, "
                     f"state={state}"
                 )
                 logger.warning(_msg)
                 raise Exception(_msg)
@@ -295,22 +318,22 @@
             'consent' in authz.authz_request['prompt'] and
             set(refresh_acrs).intersection(set(acrs))
         ):
             refresh_token = {
                 "sub": sub,
                 "at_hash": left_hash(jwt_at, "HS256"),
                 "c_hash": left_hash(authz.auth_code, "HS256"),
-                "aud": [authz.client_id],
+                "aud": authz.client_id,
                 "iss": iss_sub,
             }
             refresh_token.update(commons)
             return refresh_token
 
     def get_iss_token_data(self, session : OidcSession, issuer: FederationEntityConfiguration):
-        _sub = session.pairwised_sub()
+        _sub = session.pairwised_sub(provider_id = issuer.sub)
         iss_sub = issuer.sub
         commons = self.get_jwt_common_data()
         jwk = issuer.jwks_core[0]
 
         access_token = self.get_access_token(iss_sub, _sub, session, commons)
         jwt_at = create_jws(access_token, jwk, typ="at+jwt")
         id_token = self.get_id_token(iss_sub, _sub, session, jwt_at, commons)
@@ -342,14 +365,20 @@
 
         # filter on requested claims
         filtered_user_claims = {}
         for target, claims in session.authz_request.get("claims", {}).items():
             for claim in claims:
                 if claim in user_claims:
                     filtered_user_claims[claim] = user_claims[claim]
+            # IDA support/overload of the claims, the verified has priorities and overwrite the unverified
+            if "verified_claims" in claims:
+                claims = claims["verified_claims"].get('claims', {})
+            for claim in claims:
+                if claim in user_claims:
+                    filtered_user_claims[claim] = user_claims[claim]
 
         # mapping with human names
         i18n_user_claims = [
             OIDCFED_ATTRNAME_I18N.get(i, i)
             for i in filtered_user_claims.keys()
         ]
         return dict(
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/authz_request_view.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/views/authz_request_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,17 +165,20 @@
                 error="invalid_request",
                 error_description=_("Authorization request validation error"),
                 state = self.payload.get("state", "")
             )
         except InvalidRefreshRequestException as e:
             logger.warning(f"Invalid session: {e}")
             return HttpResponseForbidden()
-
-        acr_value = AcrValues(self.payload["acr_values"][0])
-        prompt = self.payload["prompt"]
+        if self.payload.get("acr_values", None):
+            acr_value = AcrValues(self.payload["acr_values"][0])
+        else:
+            # set this as default
+            acr_value = AcrValues.l2
+        prompt = self.payload.get("prompt", "login")
         if request.user:
             if (
                     request.user.is_authenticated and
                     acr_value == AcrValues.l1 and
                     "login" not in prompt
             ):
                 try:
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/consent_page_view.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/views/consent_page_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from django.core.paginator import Paginator
 import urllib.parse
+from urllib.parse import urlparse
 
 from djagger.decorators import schema
 from django.contrib.auth import logout
 from django.http import (
     HttpResponseForbidden,
     HttpResponseRedirect,
 )
@@ -91,25 +92,25 @@
             code=session.auth_code,
             state=session.authz_request["state"],
             iss=issuer.sub if issuer else "",
         )
 
 
 def oidc_provider_not_consent(request):
-    redirect_uri = request.GET.get("redirect_uri")
+    redirect_uri = urlparse(request.GET.get("redirect_uri"))
     state = request.GET.get("state", "")
     logout(request)
     kwargs = dict(
         error = "invalid_request",
         error_description = _(
             "Authentication request rejected by user"
         ),
         state = state
     )
-    url = f'{redirect_uri}?{urllib.parse.urlencode(kwargs)}'
+    url = f'{redirect_uri.path if redirect_uri.path else "/"}?{urllib.parse.urlencode(kwargs)}'
     return HttpResponseRedirect(url)
 
 
 class UserAccessHistoryView(OpBase, View):
 
     def get(self, request, *args, **kwargs):
         try:
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/introspection_endpoint.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/views/introspection_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/revocation_endpoint.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/views/revocation_endpoint.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/token_endpoint.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/views/token_endpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,21 +149,18 @@
 
         jwk_at = unpad_jwt_payload(iss_token_data['access_token'])
         expires_in = self.get_expires_in(jwk_at['iat'], jwk_at['exp'])
 
         data = dict( # nosec B106
             access_token = iss_token_data['access_token'],
             id_token = iss_token_data['id_token'],
+            refresh_token = iss_token_data['refresh_token'],
             token_type = "Bearer", # nosec B106
             expires_in = expires_in,
-            # TODO: remove unsupported scope
-            scope = self.authz.authz_request["scope"],
         )
-        if issued_token.refresh_token:
-            data['refresh_token'] = issued_token.refresh_token
 
         return JsonResponse(data)
 
     def post(self, request, *args, **kwargs):
         logger.debug(f"{request.headers}: {request.POST}")
         try:
             self.validate_json_schema(
@@ -178,42 +175,43 @@
                     "error_description": "Token request object validation failed",
                 },
                 status = 400
             )
 
         self.commons = self.get_jwt_common_data()
         self.issuer = self.get_issuer()
-        self.authz = OidcSession.objects.filter(
-            auth_code=request.POST["code"],
-            revoked=False
-        ).first()
-
-        if not self.authz:
-            return HttpResponseBadRequest()
 
         # check client_assertion and client ownership
         try:
             self.check_client_assertion(
                 request.POST['client_id'],
                 request.POST['client_assertion']
             )
         except Exception as e: # pragma: no cover
             logger.warning(
                 "Client authentication failed for "
-                f"{request.POST.get('client_id', 'unknow')}: {e}"
+                f"{request.POST.get('client_id', 'unknown')}: {e}"
             )
             return JsonResponse(
                 # TODO: error message here
                 {
                     'error': "unauthorized_client",
                     'error_description': ""
 
                 }, status = 403
             )
 
         if request.POST.get("grant_type") == 'authorization_code':
+            self.authz = OidcSession.objects.filter(
+                auth_code=request.POST["code"],
+                revoked=False
+            ).first()
+
+            if not self.authz:
+                return HttpResponseBadRequest()
+
             return self.grant_auth_code(request)
         elif request.POST.get("grant_type") == 'refresh_token':
             return self.grant_refresh_token(request)
         else:
             # Token exchange? :-)
             raise NotImplementedError()
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/provider/views/userinfo_endpoint.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/provider/views/userinfo_endpoint.py`

 * *Files 14% similar despite different names*

```diff
@@ -83,16 +83,23 @@
             if claim in token.session.user.attributes:
                 jwt[claim] = token.session.user.attributes[claim]
 
         # sign the data
         jws = create_jws(jwt, issuer.jwks_core[0])
 
         # encrypt the data
+        client_jwks = get_jwks(
+            rp_tc.metadata['openid_relying_party'],
+            federation_jwks = rp_tc.jwks
+        )
+        client_jwk = client_jwks[0]
+        for k in client_jwks:
+            if k.get('kid') and len(k["kid"]) >= 1:
+                client_jwk = k
+                break
+
         jwe = create_jwe(
             jws,
-            get_jwks(
-                rp_tc.metadata['openid_relying_party'],
-                federation_jwks = rp_tc.jwks
-            )[0],
+            client_jwk,
             cty="JWT"
         )
         return HttpResponse(jwe, content_type="application/jose")
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/admin.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/management/commands/fetch_openid_providers.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/management/commands/fetch_openid_providers.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0001_initial.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0002_rename_issuer_oidcauthentication_provider_and_more.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/migrations/0002_rename_issuer_oidcauthentication_provider_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0003_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/migrations/0003_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0004_rename_revoked_oidcauthenticationtoken_logged_out_and_more.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/migrations/0004_rename_revoked_oidcauthenticationtoken_logged_out_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0005_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/migrations/0005_rename_logged_out_oidcauthenticationtoken_revoked_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/migrations/0006_alter_oidcauthentication_provider_configuration_and_more.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/migrations/0006_alter_oidcauthentication_provider_configuration_and_more.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/models.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/oauth2/__init__.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/oauth2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
                     "jti": str(uuid.uuid4()),
                 },
                 jwk_dict=client_conf.jwks_core[0],
             ),
         )
 
         logger.debug(f"Access Token Request for {state}: {grant_data} ")
-
         token_request = requests.post(
             token_endpoint_url,
             data=grant_data,
             verify=HTTPC_PARAMS["connection"]["ssl"],
             timeout=HTTPC_TIMEOUT,
         )
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/settings.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,55 +52,55 @@
         "sub": ("sub",),
         "username": (
             {
                 "func": "spid_cie_oidc.relying_party.processors.issuer_prefixed_sub",
                 "kwargs": {"sep": "__"},
             },
         ),
-        "first_name": ("given_name", "https://attributes.spid.gov.it/name"),
+        "first_name": ("given_name", "given_name"),
         "last_name": (
             "family_name",
-            "https://attributes.spid.gov.it/familyName",
+            "last_name",
         ),
         "email": (
             "email",
-            "https://attributes.spid.gov.it/email",
+            "email",
         ),
-        "fiscal_number": ("https://attributes.spid.gov.it/fiscalNumber", "fiscal_number"),
+        "fiscal_number": ("https://attributes.spid.gov.it/fiscal_number", "fiscal_number"),
     },
 )
 
 
 SPID_REQUESTED_CLAIMS = getattr(
     settings,
     "RP_REQUIRED_CLAIMS",
     {
         "id_token": {
-            "https://attributes.spid.gov.it/familyName": {"essential": True},
-            "https://attributes.spid.gov.it/email": {"essential": True},
+            "given_name": {"essential": True},
+            "email": {"essential": True},
         },
         "userinfo": {
-            "https://attributes.spid.gov.it/name": None,
-            "https://attributes.spid.gov.it/familyName": None,
-            "https://attributes.spid.gov.it/email": None,
-            "https://attributes.spid.gov.it/fiscalNumber": None,
+            "given_name": None,
+            "family_name": None,
+            "email": None,
+            "https://attributes.spid.gov.it/fiscal_number": None,
         },
     },
 )
 
 CIE_REQUESTED_CLAIMS = getattr(
     settings,
     "RP_REQUIRED_CLAIMS",
     {
-        "id_token": {"family_name": {"essential": True}, "email": {"essential": True}},
+        "id_token": {"family_name": {"essential": True}, "given_name": {"essential": True}},
         "userinfo": {
             "given_name": None,
             "family_name": None,
             "email": None,
-            "fiscal_number": None
+            "https://attributes.spid.gov.it/fiscal_number": None
         },
     },
 )
 
 RP_PKCE_CONF = getattr(
     settings,
     "RP_PKCE_CONF",
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/css/access-button.css` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/static/css/access-button.css`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/js/spid-sp-access-button.js` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/static/js/spid-sp-access-button.js`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/js/spid_button.js` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/static/js/spid_button.js`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/svg/cie-ico-circle-bb.svg` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/static/svg/cie-ico-circle-bb.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/svg/favicon.ico` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/static/svg/favicon.ico`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/static/svg/spid-ico-circle-bb.svg` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/static/svg/spid-ico-circle-bb.svg`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/templates/rp_base.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/templates/rp_base.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/templates/rp_error.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/templates/rp_error.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/templates/rp_landing.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/templates/rp_landing.html`

 * *Files 15% similar despite different names*

```diff
@@ -59,20 +59,32 @@
                                     <img src="{{ attrs.logo_uri }}" alt="{{ attrs.organization_name }}">
                                     {% else %}
                                     <img src="{% static 'svg/no_image_available.svg' %}" alt="{{ sub }}">
                                     <p>{{ sub }}</p>
                                     {% endif %}
                                 </a>
                             </li>
+                         <li>
+                            <a href="{% url 'spid_cie_rp_begin' %}?provider={{sub}}&profile=spid&scope=openid offline_access" id="provider-spid-refresh_token">
+                                <span class="spid-sr-only">{{ attrs.organization_name }} {% trans "LONG TERM SESSION" %}</span>
+                                {% if attrs.logo_uri %}
+                                <img src="{{ attrs.logo_uri }}" alt="{{ attrs.organization_name }}">
+                                 <p>{% trans "LONG TERM SESSION" %}</p>
+                                {% else %}
+                                <img src="{% static 'svg/no_image_available.svg' %}" alt="{{ sub }}">
+                                <p>{{ sub }}</p>
+                                {% endif %}
+                            </a>
+                         </li>
                         {% endfor %}
                     </ul>
                 </div>
 
             </span>
-            
+
             <span
                 class="badge square-corners mb-3 mr-2 ml-0 pr-10 p-2 mw-100"
                 style="font-size: 100%">
 
                 <a href="#" class="italia-it-button italia-it-button-size-m button-cie"
                     cie-idp-button="#cie-idp-button-medium-get">
                     <span class="italia-it-button-icon"><img
@@ -83,26 +95,37 @@
                 </a>
                 <div id="cie-idp-button-medium-get"
                     class="cie-idp-button cie-idp-button-tip cie-idp-button-relative"
                     style="display: none; left: 56.5px; top: 46.05px;">
 
                     <ul id="cie-idp-list-medium-root-get" class="cie-idp-button-menu" aria-labelledby="cie-idp">
                         {% for sub, attrs in cie_providers.items %}
-                            <li>
                                 <li>
                                     <a href="{% url 'spid_cie_rp_begin' %}?provider={{sub}}&profile=cie" id="provider-cie">
                                         <span class="spid-sr-only">{{ attrs.organization_name }}</span>
                                         {% if attrs.logo_uri %}
                                         <img src="{{ attrs.logo_uri }}" alt="{{ attrs.organization_name }}">
                                         {% else %}
                                         <img src="{% static 'svg/no_image_available.svg' %}" alt="{{ sub }}">
                                         <p>{{ sub }}</p>
                                         {% endif %}
                                     </a>
                                 </li>
+                                <li>
+                                    <a href="{% url 'spid_cie_rp_begin' %}?provider={{sub}}&profile=cie&scope=openid offline_access" id="provider-cie-refresh_token">
+                                        <span class="spid-sr-only">{{ attrs.organization_name }} {% trans "LONG TERM SESSION" %}</span>
+                                        {% if attrs.logo_uri %}
+                                        <img src="{{ attrs.logo_uri }}" alt="{{ attrs.organization_name }}">
+                                        <p>{% trans "LONG TERM SESSION" %}</p>
+                                        {% else %}
+                                        <img src="{% static 'svg/no_image_available.svg' %}" alt="{{ sub }}">
+
+                                        {% endif %}
+                                    </a>
+                                </li>
                         {% endfor %}
                     </ul>
                 </div>
             </span>
         </div>
     </div>
```

#### html2text {}

```diff
@@ -15,17 +15,27 @@
 
  {%_trans_"Entra_con_SPID"_%}
     * {% for sub, attrs in spid_providers.items %}
     * {{_attrs.organization_name_}}_{%_if_attrs.logo_uri_%}_[{
       {_attrs.organization_name_}}]_{%_else_%}_[{{_sub_}}]
       {{_sub_}}
       {%_endif_%}
+    * {{_attrs.organization_name_}}_{%_trans_"LONG_TERM_SESSION"_%}_{%_if
+      attrs.logo_uri_%}_[{{_attrs.organization_name_}}]
+      {%_trans_"LONG_TERM_SESSION"_%}
+      {%_else_%}_[{{_sub_}}]
+      {{_sub_}}
+      {%_endif_%}
     * {% endfor %}
 
   {%_trans_"Entra_con_CIE"_%}
     * {% for sub, attrs in cie_providers.items %}
     * {{_attrs.organization_name_}}_{%_if_attrs.logo_uri_%}_[{
       {_attrs.organization_name_}}]_{%_else_%}_[{{_sub_}}]
       {{_sub_}}
       {%_endif_%}
+    * {{_attrs.organization_name_}}_{%_trans_"LONG_TERM_SESSION"_%}_{%_if
+      attrs.logo_uri_%}_[{{_attrs.organization_name_}}]
+      {%_trans_"LONG_TERM_SESSION"_%}
+      {%_else_%}_[{{_sub_}}]_{%_endif_%}
     * {% endfor %}
  {% endblock %}
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/mocked_response.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/mocked_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 
 
 from spid_cie_oidc.provider.tests.settings import op_conf, op_conf_priv_jwk
 from spid_cie_oidc.authority.tests.settings import rp_conf, INTERMEDIARY_JWK1
 from spid_cie_oidc.entity.jwtse import create_jws, create_jwe
 from spid_cie_oidc.entity.utils import iat_now, exp_from_now
 from spid_cie_oidc.entity.utils import get_jwks
+from cryptojwt.jws.utils import left_hash
 logger = logging.getLogger(__name__)
 
 
 class MockedTokenEndPointResponse:
     def __init__(self):
         self.status_code = 200
 
     @property
     def content(self):
         id_token = {
             'sub': '2ed008b45e66ce53e48273dca5a4463bc8ebd036ebaa824f4582627683c2451b', 
             'nonce': 'ljbvL3rpscgS4ZGda7cgibXHr7vrNREW', 
-            'at_hash': 'u2RjeYbZSJZO55XwY2LJew', 
+            'at_hash': '',
             'c_hash': 'tij0h-zL_bSrsVXy-d3qHw', 
             'aud': [rp_conf["metadata"]["openid_relying_party"]["client_id"],], 
             'iss': op_conf["sub"], 
             'jti': '402e61bd-950c-4934-83d4-c09a05468828', 
             'exp': exp_from_now(), 
             'iat': iat_now()
         }
@@ -34,38 +35,40 @@
             'client_id': rp_conf["metadata"]["openid_relying_party"]["client_id"],
             'scope': 'openid', 
             'jti': '402e61bd-950c-4934-83d4-c09a05468828', 
             'exp': exp_from_now(), 
             'iat': iat_now()
         }
         jwt_at = create_jws(access_token, op_conf_priv_jwk, typ="at+jwt")
+        id_token['at_hash'] = left_hash(jwt_at, "HS256")
         jwt_id = create_jws(id_token, op_conf_priv_jwk)
 
         self.access_token = jwt_at
         self.id_token = jwt_id
 
         res = {
                 "access_token": jwt_at,
                 "id_token": jwt_id,
                 "token_type": "Bearer",
                 "expires_in": 3600,
                 "scope": "openid",
             }
         return json.dumps(res).encode()
 
+
 class MockedTokenEndPointNoCorrectResponse:
     def __init__(self):
         self.status_code = 200
 
     @property
     def content(self):
         id_token = {
             'sub': '2ed008b45e66ce53e48273dca5a4463bc8ebd036ebaa824f4582627683c2451b', 
             'nonce': 'ljbvL3rpscgS4ZGda7cgibXHr7vrNREW', 
-            'at_hash': 'u2RjeYbZSJZO55XwY2LJew', 
+            'at_hash': '',
             'c_hash': 'tij0h-zL_bSrsVXy-d3qHw', 
             'aud': [rp_conf["metadata"]["openid_relying_party"]["client_id"],], 
             'iss': op_conf["sub"], 
             'jti': '402e61bd-950c-4934-83d4-c09a05468828', 
             'exp': exp_from_now(), 
             'iat': iat_now()
         }
@@ -76,39 +79,39 @@
             'client_id': rp_conf["metadata"]["openid_relying_party"]["client_id"],
             'scope': 'openid', 
             'jti': '402e61bd-950c-4934-83d4-c09a05468828', 
             'exp': exp_from_now(), 
             'iat': iat_now()
         }
         jwt_at = create_jws(access_token, op_conf_priv_jwk, typ="at+jwt")
+        id_token['at_hash'] = left_hash(jwt_at, "HS256")
         jwt_id = create_jws(id_token, op_conf_priv_jwk)
 
         self.access_token = jwt_at
         self.id_token = jwt_id
 
         res = {
                 "access_token": jwt_at,
                 "token_type": "Bearer",
                 "expires_in": 3600,
                 "scope": "openid",
             }
         return json.dumps(res).encode()
 
 
-
 class MockedTokenEndPointNoCorrectIdTokenResponse:
     def __init__(self):
         self.status_code = 200
 
     @property
     def content(self):
         id_token = {
             'sub': '2ed008b45e66ce53e48273dca5a4463bc8ebd036ebaa824f4582627683c2451b', 
             'nonce': 'ljbvL3rpscgS4ZGda7cgibXHr7vrNREW', 
-            'at_hash': 'u2RjeYbZSJZO55XwY2LJew', 
+            'at_hash': '',
             'c_hash': 'tij0h-zL_bSrsVXy-d3qHw', 
             'aud': [rp_conf["metadata"]["openid_relying_party"]["client_id"],], 
             'iss': op_conf["sub"], 
             'jti': '402e61bd-950c-4934-83d4-c09a05468828', 
             'exp': exp_from_now(), 
             'iat': iat_now()
         }
@@ -119,37 +122,82 @@
             'client_id': rp_conf["metadata"]["openid_relying_party"]["client_id"],
             'scope': 'openid', 
             'jti': '402e61bd-950c-4934-83d4-c09a05468828', 
             'exp': exp_from_now(), 
             'iat': iat_now()
         }
         jwt_at = create_jws(access_token, op_conf_priv_jwk, typ="at+jwt")
+        id_token['at_hash'] = left_hash(jwt_at, "HS256")
         jwt_id = create_jws(id_token, INTERMEDIARY_JWK1)
 
         self.access_token = jwt_at
         self.id_token = jwt_id
 
         res = {
                 "access_token": jwt_at,
                 "token_type": "Bearer",
                 "id_token": jwt_id,
                 "expires_in": 3600,
                 "scope": "openid",
             }
         return json.dumps(res).encode()
 
+
+class MockedTokenEndPointNoCorrectAtHashResponse:
+    def __init__(self):
+        self.status_code = 200
+
+    @property
+    def content(self):
+        id_token = {
+            'sub': '2ed008b45e66ce53e48273dca5a4463bc8ebd036ebaa824f4582627683c2451b',
+            'nonce': 'ljbvL3rpscgS4ZGda7cgibXHr7vrNREW',
+            'at_hash': '45e66ce53e48273dca5a446',
+            'c_hash': 'tij0h-zL_bSrsVXy-d3qHw',
+            'aud': [rp_conf["metadata"]["openid_relying_party"]["client_id"],],
+            'iss': op_conf["sub"],
+            'jti': '402e61bd-950c-4934-83d4-c09a05468828',
+            'exp': exp_from_now(),
+            'iat': iat_now()
+        }
+        access_token = {
+            'iss': op_conf["sub"],
+            'sub': '2ed008b45e66ce53e48273dca5a4463bc8ebd036ebaa824f4582627683c2451b',
+            'aud': [rp_conf["metadata"]["openid_relying_party"]["client_id"],],
+            'client_id': rp_conf["metadata"]["openid_relying_party"]["client_id"],
+            'scope': 'openid',
+            'jti': '402e61bd-950c-4934-83d4-c09a05468828',
+            'exp': exp_from_now(),
+            'iat': iat_now()
+        }
+        jwt_at = create_jws(access_token, op_conf_priv_jwk, typ="at+jwt")
+        jwt_id = create_jws(id_token, op_conf_priv_jwk)
+
+        self.access_token = jwt_at
+        self.id_token = jwt_id
+
+        res = {
+                "access_token": jwt_at,
+                "id_token": jwt_id,
+                "token_type": "Bearer",
+                "expires_in": 3600,
+                "scope": "openid",
+            }
+        return json.dumps(res).encode()
+
+
 class MockedUserInfoResponse:
     def __init__(self):
         self.status_code = 200
 
     @property
     def content(self):
         jwt = {
             "sub": 'asdasdasdasasdasdas',
-            "https://attributes.spid.gov.it/fiscalNumber": "sdfsfs908df09s8df90s8fd0"
+            "https://attributes.spid.gov.it/fiscal_number": "sdfsfs908df09s8df90s8fd0"
         }
         jws = create_jws(jwt, op_conf_priv_jwk)
         jwe = create_jwe(
             jws, 
             get_jwks(rp_conf["metadata"]["openid_relying_party"])[0]
         )
         return jwe.encode()
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_01_rp_ops.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/test_01_rp_ops.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_03_rp_begin.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/test_03_rp_begin.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,22 +102,22 @@
         url = reverse("spid_cie_rp_begin")
         res = client.get(url, {"request": {}})
         self.assertTrue(res.status_code == 404)
         self.assertTrue("request rejected" in res.content.decode())
         self.assertTrue("Missing provider url" in res.content.decode())
 
     # I changed the code to get a smarter solution
-    @override_settings(OIDCFED_DEFAULT_TRUST_ANCHOR=TA_SUB)
+    @override_settings(OIDCFED_DEFAULT_TRUST_ANCHOR=TA_SUB, OIDCFED_TRUST_ANCHORS=[TA_SUB])
     def test_no_unallowed_tc(self):
         client = Client()
         url = reverse("spid_cie_rp_begin")
         res = client.get(url, {"provider": "provider"})
-        self.assertTrue(res.status_code == 404)
+        self.assertTrue(res.status_code == 403)
         self.assertTrue("request rejected" in res.content.decode())
-        self.assertTrue("Unallowed Trust Anchor" in res.content.decode())
+        #  self.assertTrue("Unallowed Trust Anchor" in res.content.decode())
 
     @override_settings(OIDCFED_DEFAULT_TRUST_ANCHOR=TA_SUB, OIDCFED_TRUST_ANCHORS=[TA_SUB])
     def test_no_rp_entity_conf(self):
         FederationEntityConfiguration.objects.all().delete()
         client = Client()
         url = reverse("spid_cie_rp_begin")
         res = client.get(url, {"provider": op_conf["sub"], "trust_anchor": TA_SUB})
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_04_rp_callback.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/test_04_rp_callback.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 from spid_cie_oidc.authority.tests.settings import rp_conf
 from spid_cie_oidc.provider.tests.settings import op_conf
 from spid_cie_oidc.provider.tests.authn_request_settings import AUTHN_REQUEST_SPID
 
 from spid_cie_oidc.relying_party.tests.mocked_response import (
     MockedTokenEndPointNoCorrectIdTokenResponse,
     MockedTokenEndPointNoCorrectResponse, 
-    MockedTokenEndPointResponse, 
+    MockedTokenEndPointResponse,
+    MockedTokenEndPointNoCorrectAtHashResponse,
     MockedUserInfoResponse
 )
 
 
 STATE = "fyZiOL9Lf2CeKuNT2JzxiLRDink0uPcd"
 CODE = "usDwMnEzJPpG5oaV8x3j&"
 
@@ -163,7 +164,17 @@
     @patch("requests.get", return_value=MockedUserInfoResponse())
     def test_rp_callback_no_correct_id_token_response(self, mocked, mocked1):
         client = Client()
         url = reverse("spid_cie_rp_callback")
         res = client.get(url, {"state": STATE, "code": CODE})
         self.assertTrue(res.status_code == 403)
         self.assertTrue("invalid_token" in res.content.decode())
+
+    @override_settings(HTTP_CLIENT_SYNC=True)
+    @patch("requests.post", return_value=MockedTokenEndPointNoCorrectAtHashResponse())
+    @patch("requests.get", return_value=MockedUserInfoResponse())
+    def test_rp_callback_no_correct_at_hash_response(self, mocked, mocked1):
+        client = Client()
+        url = reverse("spid_cie_rp_callback")
+        res = client.get(url, {"state": STATE, "code": CODE})
+        self.assertTrue(res.status_code == 403)
+        self.assertTrue("at_hash verification failed" in res.content.decode())
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_05_oidc_rpinitiated_logout.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/test_05_oidc_rpinitiated_logout.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,23 +36,23 @@
         FederationEntityConfiguration.objects.create(**rp_conf)
         self.admin_user = get_user_model().objects.create_superuser(
             username="superuser", password="secret", email="admin@example.com"
         )
 
     
     @patch("requests.post", return_value=MockedLogout())
-    def test_rpinitaited_logout(self, mokced):
+    def test_rpinitiated_logout(self, mokced):
         c = Client()
         c.login(username="test", password="test")
         url = reverse("spid_cie_rpinitiated_logout")
         res = c.get(url)
         self.assertTrue(res.status_code == 302)
         self.assertTrue(res.url == "/oidc/rp/landing")
 
-    def test_rpinitaited_logout_no_revocation_endpoint(self):
+    def test_rpinitiated_logout_no_revocation_endpoint(self):
         OidcAuthentication.objects.all().delete()
         op_conf_local = deepcopy(op_conf["metadata"]["openid_provider"])
         op_conf_local.pop("revocation_endpoint")
         authz_request = OidcAuthentication.objects.create(
             client_id=rp_conf["metadata"]["openid_relying_party"]["client_id"],
             provider_configuration=op_conf_local,
         )
@@ -63,15 +63,15 @@
         c = Client()
         c.login(username="test", password="test")
         url = reverse("spid_cie_rpinitiated_logout")
         res = c.get(url)
         self.assertTrue(res.status_code == 302)
         self.assertTrue(res.url == "/oidc/rp/landing")
 
-    def test_rpinitaited_logout_no_auth_token(self):
+    def test_rpinitiated_logout_no_auth_token(self):
         OidcAuthenticationToken.objects.all().delete()
         c = Client()
         c.login(username="test", password="test")
         url = reverse("spid_cie_rpinitiated_logout")
         res = c.get(url)
         self.assertTrue(res.status_code == 302)
         self.assertTrue(res.url == "/oidc/rp/landing")
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_06_fetch_openid_providers.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/test_06_fetch_openid_providers.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_07_oidc_rp_landing.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/test_07_oidc_rp_landing.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_08_callback_echo_attributes.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/test_08_callback_echo_attributes.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/tests/test_09_rp_model.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/tests/test_09_rp_model.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/utils.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 def random_string(n=32):
     return "".join(random.choices(string.ascii_letters + string.digits, k=n))  # nosec
 
 
 def get_pkce(code_challenge_method: str = "S256", code_challenge_length: int = 64):
     hashers = {"S256": hashlib.sha256}
 
-    code_verifier = base64.urlsafe_b64encode(os.urandom(40)).decode("utf-8")
+    code_verifier_length = random.randint(43, 128) # nosec - B311
+    code_verifier = base64.urlsafe_b64encode(os.urandom(code_verifier_length)).decode("utf-8")
     code_verifier = re.sub("[^a-zA-Z0-9]+", "", code_verifier)
 
     code_challenge = hashers.get(code_challenge_method)(
         code_verifier.encode("utf-8")
     ).digest()
     code_challenge = base64.urlsafe_b64encode(code_challenge).decode("utf-8")
     code_challenge = code_challenge.replace("=", "")
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/rp_begin.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/views/rp_begin.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,29 +60,29 @@
         try:
             tc = self.get_oidc_op(request)
             if not tc:
                 context = {
                     "error": "request rejected",
                     "error_description": "Trust Chain is unavailable.",
                 }
-                return render(request, self.error_template, context)
+                return render(request, self.error_template, context, status = 404)
 
         except InvalidTrustchain as exc:
             context = {
                 "error": "request rejected",
                 "error_description": str(exc.args),
             }
             return render(request, self.error_template, context, status=404)
 
         except Exception as exc:
             context = {
                 "error": "request rejected",
                 "error_description": _(str(exc.args)),
             }
-            return render(request, self.error_template, context)
+            return render(request, self.error_template, context, status=403)
 
         provider_metadata = tc.metadata.get('openid_provider', None)
         if not provider_metadata:
             context = {
                 "error": "request rejected",
                 "error_description": _("provider metadata not found"),
             }
@@ -98,17 +98,16 @@
                 "error": "request rejected",
                 "error_description": _("Missing configuration."),
             }
             return render(request, self.error_template, context, status=404)
 
         client_conf = entity_conf.metadata["openid_relying_party"]
         if not (
-            # TODO
-            # provider_metadata.get("jwks_uri", None)
-            # or
+            provider_metadata.get("jwks_uri", None)
+            or
             provider_metadata.get("jwks", None)
         ):
             context = {
                 "error": "request rejected",
                 "error_description": _("Invalid provider Metadata."),
             }
             return render(request, self.error_template, context, status=404)
@@ -196,10 +195,14 @@
                 "scope" : authz_data["scope"],
                 "response_type": authz_data["response_type"],
                 "code_challenge": authz_data["code_challenge"],
                 "code_challenge_method": authz_data["code_challenge_method"],
                 "request": authz_data["request"]
             }
         )
-        url = "?".join((authz_endpoint, uri_path))
+        if "?" in authz_endpoint:
+            qstring = "&"
+        else:
+            qstring = "?"
+        url = qstring.join((authz_endpoint, uri_path))
         logger.info(f"Starting Authz request to {url}")
         return HttpResponseRedirect(url)
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/rp_callback.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/views/rp_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from django.http import HttpResponseRedirect, JsonResponse
 from django.shortcuts import render
 from django.urls import reverse
 from django.utils.translation import gettext as _
 from django.views import View
 from spid_cie_oidc.entity.jwtse import (
     unpad_jwt_payload,
-    verify_jws
+    verify_jws,
+    verify_at_hash
 )
 from spid_cie_oidc.entity.models import FederationEntityConfiguration
 from spid_cie_oidc.entity.settings import HTTPC_PARAMS
 from spid_cie_oidc.entity.utils import get_jwks, get_jwk_from_jwt
 from spid_cie_oidc.relying_party.exceptions import ValidationException
 from spid_cie_oidc.relying_party.settings import RP_PROVIDER_PROFILES, RP_DEFAULT_PROVIDER_PROFILES
 
@@ -57,17 +58,24 @@
         /redirect_uri?code=tYkP854StRqBVcW4Kg4sQfEN5Qz&state=R9EVqaazGsj3wg5JgxIgm8e8U4BMvf7W
     """
 
     error_template = "rp_error.html"
 
     def user_reunification(self, user_attrs: dict):
         user_model = get_user_model()
-        lookup = {
-            f"attributes__{RP_USER_LOOKUP_FIELD}": user_attrs[RP_USER_LOOKUP_FIELD]
-        }
+
+        if user_attrs.get(RP_USER_LOOKUP_FIELD, None):
+            lookup = {
+                f"attributes__{RP_USER_LOOKUP_FIELD}": user_attrs.get(RP_USER_LOOKUP_FIELD)
+            }
+        else:
+            logger.warning("User attribute not found for reunification, try sub")
+            lookup = {
+                "username": user_attrs["username"]
+            }
         user = user_model.objects.filter(**lookup).first()
         if user:
             user.attributes.update(user_attrs)
             user.save()
             logger.info(f"{RP_USER_LOOKUP_FIELD} matched on user {user}")
             return user
         elif RP_USER_CREATE:
@@ -177,14 +185,15 @@
                         "error_description": "Token response object validation failed",
                     },
                     status = 400
                 )
         jwks = get_jwks(authz.provider_configuration)
         access_token = token_response["access_token"]
         id_token = token_response["id_token"]
+
         op_ac_jwk = get_jwk_from_jwt(access_token, jwks)
         op_id_jwk = get_jwk_from_jwt(id_token, jwks)
 
         if not op_ac_jwk or not op_id_jwk:
             logger.warning(
                 "Token signature validation error, "
                 f"the tokens were signed with a different kid from: {jwks}."
@@ -218,28 +227,41 @@
                 "error_description": _("ID token validation error."),
             }
             return render(request, self.error_template, context, status=403)
 
         decoded_id_token = unpad_jwt_payload(id_token)
         logger.debug(decoded_id_token)
 
+        try:
+            verify_at_hash(decoded_id_token, access_token)
+        except Exception as e:
+            logger.warning(
+                f"at_hash validation error: {e} "
+            )
+            context = {
+                "error": "at_hash verification failed",
+                "error_description": _("at_hash validation error."),
+            }
+            return render(request, self.error_template, context, status=403)
+
         decoded_access_token = unpad_jwt_payload(access_token)
         logger.debug(decoded_access_token)
 
         authz_token.access_token = access_token
         authz_token.id_token = id_token
         authz_token.scope = token_response.get("scope")
         authz_token.token_type = token_response["token_type"]
         authz_token.expires_in = token_response["expires_in"]
         authz_token.save()
+
         userinfo = self.get_userinfo(
             authz.state,
             authz_token.access_token,
             authz.provider_configuration,
-            verify=HTTPC_PARAMS,
+            verify=HTTPC_PARAMS.get("connection", {}).get("ssl", True)
         )
         if not userinfo:
             logger.warning(
                 "Userinfo request failed for state: "
                 f"{authz.state} to {authz.provider_id}"
             )
             context = {
@@ -262,17 +284,31 @@
 
         user = self.user_reunification(user_attrs)
         if not user:
             # TODO: verify error message and status
             context = {"error": _("No user found"), "error_description": _("")}
             return render(request, self.error_template, context, status=403)
 
+        request.session["rt_expiration"] = 0
+
+        if token_response.get('refresh_token', None):
+            refresh_token = token_response["refresh_token"]
+            authz_token.refresh_token = refresh_token
+            decoded_refresh_token = unpad_jwt_payload(refresh_token)
+            request.session["rt_expiration"] = decoded_refresh_token['exp'] - iat_now()
+            request.session["rt_jti"] = decoded_refresh_token['jti']
+            logger.info(decoded_refresh_token)
+
         # authenticate the user
         login(request, user)
         request.session["oidc_rp_user_attrs"] = user_attrs
+
+        request.session["at_expiration"] = decoded_access_token['exp'] - iat_now()
+        request.session["at_jti"] = decoded_access_token['jti']
+
         authz_token.user = user
         authz_token.save()
         return HttpResponseRedirect(
             getattr(
                 settings, "LOGIN_REDIRECT_URL", None
             ) or reverse("spid_cie_rp_echo_attributes")
         )
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party/views/rp_landing.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party/views/rp_landing.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/admin.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/admin.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/forms.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/forms.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/migrations/0001_initial.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/migrations/0002_alter_relyingpartytest_report.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/migrations/0002_alter_relyingpartytest_report.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/models.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/models.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/snippets/README.md` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/snippets/README.md`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/snippets/crawler.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/snippets/crawler.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/snippets/pyppeteer_tests.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/snippets/pyppeteer_tests.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/static/images/oops.webp` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/static/images/oops.webp`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/templates/op_user_staff_test.html` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/templates/op_user_staff_test.html`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/tests/test_01_user_staff.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/tests/test_01_user_staff.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc/relying_party_test/views.py` & `spid_cie_oidc-1.0.0/spid_cie_oidc/relying_party_test/views.py`

 * *Files identical despite different names*

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc.egg-info/PKG-INFO` & `spid_cie_oidc-1.0.0/spid_cie_oidc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: spid-cie-oidc
-Version: 0.8.9
+Version: 1.0.0
 Summary: SPID/CIE OIDC Federation Entity
 Home-page: https://github.com/peppelinux/spid-cie-oidc
 Author: Giuseppe De Marco
 Author-email: demarcog83@gmail.com
 License: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 # SPID/CIE OIDC Federation SDK
 
 ![CI build](https://github.com/peppelinux/spid-cie-oidc-django/workflows/spid_cie_oidc/badge.svg)
 [![Maintainability](https://api.codeclimate.com/v1/badges/dd67eb5a241955b75585/maintainability)](https://codeclimate.com/github/italia/spid-cie-oidc-django/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/dd67eb5a241955b75585/test_coverage)](https://codeclimate.com/github/italia/spid-cie-oidc-django/test_coverage)
 ![Python version](https://img.shields.io/badge/license-Apache%202-blue.svg)
-![py-versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue.svg)
+![py-versions](https://img.shields.io/badge/python-3.10-blue.svg)
 [![GitHub issues](https://img.shields.io/github/issues/italia/spid-cie-oidc-django.svg)](https://github.com/italia/spid-cie-oidc-django/issues)
 [![Get invited](https://slack.developers.italia.it/badge.svg)](https://slack.developers.italia.it/)
 [![Join the #spid openid](https://img.shields.io/badge/Slack%20channel-%23spid%20openid-blue.svg)](https://developersitalia.slack.com/archives/C7E85ED1N/)
 
 
 SPID/CIE OIDC Federation is a suite of Django applications designed to
 make it easy to build an [Openid Connect Federation](https://openid.net/specs/openid-connect-federation-1_0.html), 
@@ -119,15 +119,15 @@
 Run the stack
 ````
 sudo docker-compose up
 ````
 
 Configure a proper DNS resolution for trust-anchor.org. In GNU/Linux we can configure it in `/etc/hosts`:
 ````
-127.0.0.1   localhost  trust-anchor.org relying-party.org cie-provider.org
+127.0.0.1   localhost  trust-anchor.org relying-party.org cie-provider.org wallet.trust-anchor.org
 ````
 
 Point your web browser to `http://relying-party.org:8001/oidc/rp/landing` and do your first oidc authentication.
 
 
 ## Usage
```

### Comparing `spid_cie_oidc-0.8.9/spid_cie_oidc.egg-info/SOURCES.txt` & `spid_cie_oidc-1.0.0/spid_cie_oidc.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 ./spid_cie_oidc/authority/migrations/0003_alter_federationdescendantcontact_entity_and_more.py
 ./spid_cie_oidc/authority/migrations/0004_federationdescendant_jwks_and_more.py
 ./spid_cie_oidc/authority/migrations/0005_alter_federationdescendant_jwks.py
 ./spid_cie_oidc/authority/migrations/0006_stafftoken.py
 ./spid_cie_oidc/authority/migrations/0007_stafftoken_expire_at.py
 ./spid_cie_oidc/authority/migrations/0008_alter_stafftoken_token.py
 ./spid_cie_oidc/authority/migrations/0009_delete_stafftoken.py
+./spid_cie_oidc/authority/migrations/0010_federationdescendant_metadata_and_more.py
+./spid_cie_oidc/authority/migrations/0011_federationdescendant_issue_x509_and_more.py
+./spid_cie_oidc/authority/migrations/0012_remove_federationdescendant_issue_x509.py
 ./spid_cie_oidc/authority/migrations/__init__.py
 ./spid_cie_oidc/authority/schemas/__init__.py
 ./spid_cie_oidc/authority/schemas/advanced_entity_list_endpoint.py
 ./spid_cie_oidc/authority/schemas/fetch_endpoint_request.py
 ./spid_cie_oidc/authority/schemas/list_endpoint.py
 ./spid_cie_oidc/authority/schemas/trust_mark_status_endpoint.py
 ./spid_cie_oidc/authority/tests/__init__.py
@@ -59,14 +62,15 @@
 ./spid_cie_oidc/entity/statements.py
 ./spid_cie_oidc/entity/trust_chain.py
 ./spid_cie_oidc/entity/trust_chain_operations.py
 ./spid_cie_oidc/entity/urls.py
 ./spid_cie_oidc/entity/utils.py
 ./spid_cie_oidc/entity/validators.py
 ./spid_cie_oidc/entity/views.py
+./spid_cie_oidc/entity/x509.py
 ./spid_cie_oidc/entity/migrations/0001_initial.py
 ./spid_cie_oidc/entity/migrations/0002_fetchedentitystatement.py
 ./spid_cie_oidc/entity/migrations/0003_federationentityconfiguration_constraints.py
 ./spid_cie_oidc/entity/migrations/0004_alter_federationentityconfiguration_authority_hints_and_more.py
 ./spid_cie_oidc/entity/migrations/0005_alter_federationentityconfiguration_constraints.py
 ./spid_cie_oidc/entity/migrations/0006_remove_trustchain_resultant_metadata_and_more.py
 ./spid_cie_oidc/entity/migrations/0007_alter_trustchain_unique_together_and_more.py
@@ -78,14 +82,26 @@
 ./spid_cie_oidc/entity/migrations/0013_alter_federationentityconfiguration_metadata.py
 ./spid_cie_oidc/entity/migrations/0014_alter_trustchain_unique_together_and_more.py
 ./spid_cie_oidc/entity/migrations/0015_alter_trustchain_unique_together_trustchain_type_and_more.py
 ./spid_cie_oidc/entity/migrations/0016_alter_trustchain_unique_together_and_more.py
 ./spid_cie_oidc/entity/migrations/0017_remove_federationentityconfiguration_jwks_and_more.py
 ./spid_cie_oidc/entity/migrations/0018_trustchain_jwks.py
 ./spid_cie_oidc/entity/migrations/0019_stafftoken.py
+./spid_cie_oidc/entity/migrations/0020_alter_federationentityconfiguration_jwks_core_and_more.py
+./spid_cie_oidc/entity/migrations/0021_federationhistoricalkey.py
+./spid_cie_oidc/entity/migrations/0021_federationhistoricalkey_squashed_0026_alter_federationhistoricalkey_jwk.py
+./spid_cie_oidc/entity/migrations/0022_federationhistoricalkey_jwk_and_more.py
+./spid_cie_oidc/entity/migrations/0023_alter_federationhistoricalkey_jwk.py
+./spid_cie_oidc/entity/migrations/0024_alter_federationhistoricalkey_kid.py
+./spid_cie_oidc/entity/migrations/0025_alter_federationhistoricalkey_jwk.py
+./spid_cie_oidc/entity/migrations/0026_alter_federationhistoricalkey_jwk.py
+./spid_cie_oidc/entity/migrations/0027_alter_federationhistoricalkey_revocation_motivation.py
+./spid_cie_oidc/entity/migrations/0028_federationentityconfiguration_issue_x509.py
+./spid_cie_oidc/entity/migrations/0029_alter_federationentityconfiguration_entity_type_and_more.py
+./spid_cie_oidc/entity/migrations/0030_remove_federationentityconfiguration_issue_x509.py
 ./spid_cie_oidc/entity/migrations/__init__.py
 ./spid_cie_oidc/entity/schemas/__init__.py
 ./spid_cie_oidc/entity/schemas/fa_metadata.py
 ./spid_cie_oidc/entity/schemas/jwks.py
 ./spid_cie_oidc/entity/schemas/op_metadata.py
 ./spid_cie_oidc/entity/schemas/resolve_endpoint.py
 ./spid_cie_oidc/entity/schemas/rp_metadata.py
@@ -119,14 +135,15 @@
 ./spid_cie_oidc/onboarding/migrations/0002_alter_onboardingregistration_options_and_more.py
 ./spid_cie_oidc/onboarding/migrations/0003_alter_onboardingregistration_options.py
 ./spid_cie_oidc/onboarding/migrations/0004_alter_onboardingregistration_public_jwks.py
 ./spid_cie_oidc/onboarding/migrations/0005_alter_onboardingregistration_status.py
 ./spid_cie_oidc/onboarding/migrations/0006_onboardingregistration_type.py
 ./spid_cie_oidc/onboarding/migrations/0007_onboardingregistration_contact.py
 ./spid_cie_oidc/onboarding/migrations/0008_onboardingregistration_auth_request_url.py
+./spid_cie_oidc/onboarding/migrations/0009_alter_onboardingregistration_type.py
 ./spid_cie_oidc/onboarding/migrations/__init__.py
 ./spid_cie_oidc/onboarding/static/images/SPID-e-CIE-696x383.jpg
 ./spid_cie_oidc/onboarding/static/images/logo-it.svg
 ./spid_cie_oidc/onboarding/templates/base.html
 ./spid_cie_oidc/onboarding/templates/onboarding_apply_policy.html
 ./spid_cie_oidc/onboarding/templates/onboarding_convert_jwk.html
 ./spid_cie_oidc/onboarding/templates/onboarding_convert_pem.html
@@ -216,14 +233,15 @@
 ./spid_cie_oidc/provider/tests/test_10_revocation_response.py
 ./spid_cie_oidc/provider/tests/test_11_user_access_history.py
 ./spid_cie_oidc/provider/tests/test_12_init.py
 ./spid_cie_oidc/provider/tests/token_request_settings.py
 ./spid_cie_oidc/provider/tests/token_response_settings.py
 ./spid_cie_oidc/provider/views/__init__.py
 ./spid_cie_oidc/provider/views/authz_request_view.py
+./spid_cie_oidc/provider/views/connect.py
 ./spid_cie_oidc/provider/views/consent_page_view.py
 ./spid_cie_oidc/provider/views/introspection_endpoint.py
 ./spid_cie_oidc/provider/views/revocation_endpoint.py
 ./spid_cie_oidc/provider/views/token_endpoint.py
 ./spid_cie_oidc/provider/views/userinfo_endpoint.py
 ./spid_cie_oidc/relying_party/__init__.py
 ./spid_cie_oidc/relying_party/admin.py
@@ -253,14 +271,15 @@
 ./spid_cie_oidc/relying_party/static/js/spid_button.js
 ./spid_cie_oidc/relying_party/static/svg/cie-ico-circle-bb.svg
 ./spid_cie_oidc/relying_party/static/svg/favicon.ico
 ./spid_cie_oidc/relying_party/static/svg/spid-ico-circle-bb.svg
 ./spid_cie_oidc/relying_party/templates/echo_attributes.html
 ./spid_cie_oidc/relying_party/templates/rp_base.html
 ./spid_cie_oidc/relying_party/templates/rp_error.html
+./spid_cie_oidc/relying_party/templates/rp_introspection.html
 ./spid_cie_oidc/relying_party/templates/rp_landing.html
 ./spid_cie_oidc/relying_party/tests/__init__.py
 ./spid_cie_oidc/relying_party/tests/mocked_response.py
 ./spid_cie_oidc/relying_party/tests/test_01_rp_ops.py
 ./spid_cie_oidc/relying_party/tests/test_02_rp_commands.py
 ./spid_cie_oidc/relying_party/tests/test_03_rp_begin.py
 ./spid_cie_oidc/relying_party/tests/test_04_rp_callback.py
@@ -269,15 +288,17 @@
 ./spid_cie_oidc/relying_party/tests/test_07_oidc_rp_landing.py
 ./spid_cie_oidc/relying_party/tests/test_08_callback_echo_attributes.py
 ./spid_cie_oidc/relying_party/tests/test_09_rp_model.py
 ./spid_cie_oidc/relying_party/views/__init__.py
 ./spid_cie_oidc/relying_party/views/rp_begin.py
 ./spid_cie_oidc/relying_party/views/rp_callback.py
 ./spid_cie_oidc/relying_party/views/rp_callback_echo_attributes.py
+./spid_cie_oidc/relying_party/views/rp_extend_session.py
 ./spid_cie_oidc/relying_party/views/rp_initiated_logout.py
+./spid_cie_oidc/relying_party/views/rp_introspection.py
 ./spid_cie_oidc/relying_party/views/rp_landing.py
 ./spid_cie_oidc/relying_party_test/__init__.py
 ./spid_cie_oidc/relying_party_test/admin.py
 ./spid_cie_oidc/relying_party_test/apps.py
 ./spid_cie_oidc/relying_party_test/forms.py
 ./spid_cie_oidc/relying_party_test/models.py
 ./spid_cie_oidc/relying_party_test/urls.py
```

