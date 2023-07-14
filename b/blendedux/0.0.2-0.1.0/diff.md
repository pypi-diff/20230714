# Comparing `tmp/blendedux-0.0.2.tar.gz` & `tmp/blendedux-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blendedux-0.0.2.tar", last modified: Fri Aug 26 06:22:11 2022, max compression
+gzip compressed data, was "blendedux-0.1.0.tar", last modified: Fri Jul 14 05:54:07 2023, max compression
```

## Comparing `blendedux-0.0.2.tar` & `blendedux-0.1.0.tar`

### file list

```diff
@@ -1,153 +1,155 @@
-drwxrwxrwx   0        0        0        0 2022-08-26 06:22:11.130946 blendedux-0.0.2/
--rw-rw-rw-   0        0        0     1096 2022-08-25 09:38:05.000000 blendedux-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     5312 2022-08-26 06:22:11.129949 blendedux-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5070 2022-08-26 06:21:17.000000 blendedux-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-08-26 06:22:10.790547 blendedux-0.0.2/blendedUx/
--rw-rw-rw-   0        0        0       97 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-26 06:22:10.804475 blendedux-0.0.2/blendedUx/blended_flask/
--rw-rw-rw-   0        0        0     1202 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/__init__.py
--rw-rw-rw-   0        0        0       97 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/app.py
-drwxrwxrwx   0        0        0        0 2022-08-26 06:22:10.812474 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/
--rw-rw-rw-   0        0        0        0 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-26 06:22:10.821939 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/backend/
--rw-rw-rw-   0        0        0       24 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/backend/__init__.py
--rw-rw-rw-   0        0        0    44898 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/backend/backend.py
--rw-rw-rw-   0        0        0     8056 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/backend/intermediary.py
--rw-rw-rw-   0        0        0     1016 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/backend/settings.py
-drwxrwxrwx   0        0        0        0 2022-08-26 06:22:10.827082 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/controller/
--rw-rw-rw-   0        0        0       27 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/controller/__init__.py
--rw-rw-rw-   0        0        0   150877 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/controller/controller.py
-drwxrwxrwx   0        0        0        0 2022-08-26 06:22:10.831108 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/exceptions/
--rw-rw-rw-   0        0        0       25 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/exceptions/__init__.py
--rw-rw-rw-   0        0        0      456 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/exceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-08-26 06:22:10.837495 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/functions/
--rw-rw-rw-   0        0        0       26 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/functions/__init__.py
--rw-rw-rw-   0        0        0      655 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/functions/functions.py
--rw-rw-rw-   0        0        0    24684 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/initializer.py
-drwxrwxrwx   0        0        0        0 2022-08-26 06:22:10.842485 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/network/
--rw-rw-rw-   0        0        0       24 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/network/__init__.py
--rw-rw-rw-   0        0        0    36830 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/network/network.py
--rw-rw-rw-   0        0        0      102 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/network/settings.py
-drwxrwxrwx   0        0        0        0 2022-08-26 06:22:10.853578 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/
--rw-rw-rw-   0        0        0     6577 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/__init__.py
--rw-rw-rw-   0        0        0    21458 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/api_client.py
-drwxrwxrwx   0        0        0        0 2022-08-26 06:22:10.859875 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/
--rw-rw-rw-   0        0        0      152 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/__init__.py
--rw-rw-rw-   0        0        0   141226 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/accounts_api.py
--rw-rw-rw-   0        0        0   242470 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/packages_api.py
--rw-rw-rw-   0        0        0     7574 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/configuration.py
-drwxrwxrwx   0        0        0        0 2022-08-26 06:22:11.105970 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/
--rw-rw-rw-   0        0        0     5530 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/__init__.py
--rw-rw-rw-   0        0        0     8007 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account.py
--rw-rw-rw-   0        0        0     5983 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invite_pending.py
--rw-rw-rw-   0        0        0     4369 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invites_pending_list.py
--rw-rw-rw-   0        0        0     4168 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/accounts.py
--rw-rw-rw-   0        0        0    10818 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition.py
--rw-rw-rw-   0        0        0     3597 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response.py
--rw-rw-rw-   0        0        0    10364 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response_data.py
--rw-rw-rw-   0        0        0     4303 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/activationchallenge.py
--rw-rw-rw-   0        0        0     7352 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/active_account.py
--rw-rw-rw-   0        0        0     3547 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_account.py
--rw-rw-rw-   0        0        0     3489 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_admin.py
--rw-rw-rw-   0        0        0     4114 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_license.py
--rw-rw-rw-   0        0        0     5149 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_pending.py
--rw-rw-rw-   0        0        0     3543 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_rating.py
--rw-rw-rw-   0        0        0     7377 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/all_license_price.py
--rw-rw-rw-   0        0        0    22811 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/blended_package.py
--rw-rw-rw-   0        0        0     3503 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body.py
--rw-rw-rw-   0        0        0     3727 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body_1.py
--rw-rw-rw-   0        0        0     7110 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages.py
--rw-rw-rw-   0        0        0    12189 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages_error.py
--rw-rw-rw-   0        0        0    18472 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/canonical_version.py
--rw-rw-rw-   0        0        0     3615 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_current_account.py
--rw-rw-rw-   0        0        0     3735 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_privilege.py
--rw-rw-rw-   0        0        0     5504 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_account.py
--rw-rw-rw-   0        0        0     4973 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_canonical.py
--rw-rw-rw-   0        0        0     4853 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_package.py
--rw-rw-rw-   0        0        0     7008 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_version.py
--rw-rw-rw-   0        0        0     5695 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies.py
--rw-rw-rw-   0        0        0     4261 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies_list.py
--rw-rw-rw-   0        0        0    11135 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail.py
--rw-rw-rw-   0        0        0     5279 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail_dependency_of_package.py
--rw-rw-rw-   0        0        0     4151 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/documents.py
--rw-rw-rw-   0        0        0     4125 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error.py
--rw-rw-rw-   0        0        0     5150 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response400.py
--rw-rw-rw-   0        0        0     5198 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response401.py
--rw-rw-rw-   0        0        0     9159 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response409.py
--rw-rw-rw-   0        0        0     9152 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response412.py
--rw-rw-rw-   0        0        0     6037 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response500.py
--rw-rw-rw-   0        0        0     8824 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/failed_dependency_error.py
--rw-rw-rw-   0        0        0     4246 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_account.py
--rw-rw-rw-   0        0        0     3645 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_canonical_version.py
--rw-rw-rw-   0        0        0     7652 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_current_account.py
--rw-rw-rw-   0        0        0     4399 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_dependency_packages.py
--rw-rw-rw-   0        0        0     9790 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_draft.py
--rw-rw-rw-   0        0        0     4256 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_licenses.py
--rw-rw-rw-   0        0        0     4308 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_pending_user.py
--rw-rw-rw-   0        0        0     4239 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_ratings.py
--rw-rw-rw-   0        0        0     4201 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_user.py
--rw-rw-rw-   0        0        0     4286 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_validators.py
--rw-rw-rw-   0        0        0    10246 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_package.py
--rw-rw-rw-   0        0        0     4251 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_packages.py
--rw-rw-rw-   0        0        0     3735 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/inline_response_200.py
--rw-rw-rw-   0        0        0     5230 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/license.py
--rw-rw-rw-   0        0        0     4598 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/like.py
--rw-rw-rw-   0        0        0     5095 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/login.py
--rw-rw-rw-   0        0        0     3651 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/logout.py
--rw-rw-rw-   0        0        0     4919 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/new_draft.py
--rw-rw-rw-   0        0        0     2986 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/operands.py
--rw-rw-rw-   0        0        0     6127 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_detail_data.py
--rw-rw-rw-   0        0        0     5293 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_images.py
--rw-rw-rw-   0        0        0     4181 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/packages.py
--rw-rw-rw-   0        0        0     5560 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_user.py
--rw-rw-rw-   0        0        0     4212 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_users.py
--rw-rw-rw-   0        0        0    10618 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication.py
--rw-rw-rw-   0        0        0    14020 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_error.py
--rw-rw-rw-   0        0        0    17540 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_validation_error.py
--rw-rw-rw-   0        0        0     8618 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version.py
--rw-rw-rw-   0        0        0     8540 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version_error.py
--rw-rw-rw-   0        0        0     4303 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions.py
--rw-rw-rw-   0        0        0     4368 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions_error.py
--rw-rw-rw-   0        0        0     5025 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications.py
--rw-rw-rw-   0        0        0     7275 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications_error.py
--rw-rw-rw-   0        0        0     5218 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/rating.py
--rw-rw-rw-   0        0        0    13040 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reject_acquisition_package.py
--rw-rw-rw-   0        0        0     4502 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/remove_pending.py
--rw-rw-rw-   0        0        0     3659 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_account_verification_link.py
--rw-rw-rw-   0        0        0     5940 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_invite.py
--rw-rw-rw-   0        0        0     3624 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reset_password.py
--rw-rw-rw-   0        0        0    16618 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_result.py
--rw-rw-rw-   0        0        0     5002 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_results.py
--rw-rw-rw-   0        0        0     5133 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/session_data.py
--rw-rw-rw-   0        0        0     4390 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/share_approval_list_error.py
--rw-rw-rw-   0        0        0     9362 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_account.py
--rw-rw-rw-   0        0        0     4385 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_accounts_list.py
--rw-rw-rw-   0        0        0     9033 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_account.py
--rw-rw-rw-   0        0        0     4935 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_draft.py
--rw-rw-rw-   0        0        0     3569 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_license.py
--rw-rw-rw-   0        0        0     6351 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_package.py
--rw-rw-rw-   0        0        0     4537 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_publication.py
--rw-rw-rw-   0        0        0     3780 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_version.py
--rw-rw-rw-   0        0        0     4799 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/upload_media.py
--rw-rw-rw-   0        0        0    12227 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/user.py
--rw-rw-rw-   0        0        0     4121 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/users.py
--rw-rw-rw-   0        0        0     8930 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator.py
--rw-rw-rw-   0        0        0     6347 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_detail.py
--rw-rw-rw-   0        0        0     6614 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_plan.py
--rw-rw-rw-   0        0        0     9282 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_sets_in_badge.py
--rw-rw-rw-   0        0        0    17690 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/version.py
--rw-rw-rw-   0        0        0     4152 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/versions.py
--rw-rw-rw-   0        0        0     9542 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/rest.py
--rw-rw-rw-   0        0        0     3319 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/tests.py
--rw-rw-rw-   0        0        0    11926 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/transform_image.py
--rw-rw-rw-   0        0        0     3762 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/functions.py
--rw-rw-rw-   0        0        0      329 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/settings.py
--rw-rw-rw-   0        0        0     3799 2022-08-25 06:08:33.000000 blendedux-0.0.2/blendedUx/blended_flask/utils.py
-drwxrwxrwx   0        0        0        0 2022-08-26 06:22:11.128960 blendedux-0.0.2/blendedux.egg-info/
--rw-rw-rw-   0        0        0     5312 2022-08-26 06:22:10.000000 blendedux-0.0.2/blendedux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10076 2022-08-26 06:22:10.000000 blendedux-0.0.2/blendedux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-26 06:22:10.000000 blendedux-0.0.2/blendedux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      217 2022-08-26 06:22:10.000000 blendedux-0.0.2/blendedux.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-08-26 06:22:10.000000 blendedux-0.0.2/blendedux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-26 06:22:11.130946 blendedux-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      997 2022-08-26 06:21:29.000000 blendedux-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:54:07.668617 blendedux-0.1.0/
+-rw-rw-rw-   0        0        0     1096 2022-08-25 09:38:05.000000 blendedux-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-07-14 05:47:24.000000 blendedux-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5406 2023-07-14 05:54:07.665610 blendedux-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5119 2023-07-14 04:16:19.000000 blendedux-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 05:54:06.739562 blendedux-0.1.0/blendedUx/
+-rw-rw-rw-   0        0        0      107 2023-07-13 12:14:39.000000 blendedux-0.1.0/blendedUx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:54:06.769113 blendedux-0.1.0/blendedUx/blended_flask/
+-rw-rw-rw-   0        0        0      160 2023-07-13 13:32:53.000000 blendedux-0.1.0/blendedUx/blended_flask/__init__.py
+-rw-rw-rw-   0        0        0     1208 2023-07-13 13:32:53.000000 blendedux-0.1.0/blendedUx/blended_flask/app.py
+-rw-rw-rw-   0        0        0     3758 2023-07-13 13:32:53.000000 blendedux-0.1.0/blendedUx/blended_flask/bl_flask_app.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:54:06.777119 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/
+-rw-rw-rw-   0        0        0        0 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:54:06.910350 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/backend/
+-rw-rw-rw-   0        0        0       24 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/backend/__init__.py
+-rw-rw-rw-   0        0        0    44898 2023-07-13 13:32:53.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/backend/backend.py
+-rw-rw-rw-   0        0        0     8056 2023-07-13 13:32:53.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/backend/intermediary.py
+-rw-rw-rw-   0        0        0     1016 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/backend/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:54:06.914334 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/controller/
+-rw-rw-rw-   0        0        0       27 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/controller/__init__.py
+-rw-rw-rw-   0        0        0   150877 2023-07-13 13:32:53.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/controller/controller.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:54:06.919336 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/exceptions/
+-rw-rw-rw-   0        0        0       25 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      456 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/exceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:54:06.923333 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/functions/
+-rw-rw-rw-   0        0        0       26 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/functions/__init__.py
+-rw-rw-rw-   0        0        0      655 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/functions/functions.py
+-rw-rw-rw-   0        0        0    24684 2023-07-13 13:32:53.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/initializer.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:54:06.928341 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/network/
+-rw-rw-rw-   0        0        0       24 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/network/__init__.py
+-rw-rw-rw-   0        0        0    36830 2023-07-13 13:32:53.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/network/network.py
+-rw-rw-rw-   0        0        0      102 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/network/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:54:06.946334 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/
+-rw-rw-rw-   0        0        0     6577 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/__init__.py
+-rw-rw-rw-   0        0        0    21458 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/api_client.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:54:06.958349 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/
+-rw-rw-rw-   0        0        0      152 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/__init__.py
+-rw-rw-rw-   0        0        0   141226 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/accounts_api.py
+-rw-rw-rw-   0        0        0   242470 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/packages_api.py
+-rw-rw-rw-   0        0        0     7574 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/configuration.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:54:07.604257 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/
+-rw-rw-rw-   0        0        0     5530 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/__init__.py
+-rw-rw-rw-   0        0        0     8007 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account.py
+-rw-rw-rw-   0        0        0     5983 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invite_pending.py
+-rw-rw-rw-   0        0        0     4369 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invites_pending_list.py
+-rw-rw-rw-   0        0        0     4168 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/accounts.py
+-rw-rw-rw-   0        0        0    10818 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition.py
+-rw-rw-rw-   0        0        0     3597 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response.py
+-rw-rw-rw-   0        0        0    10364 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response_data.py
+-rw-rw-rw-   0        0        0     4303 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/activationchallenge.py
+-rw-rw-rw-   0        0        0     7352 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/active_account.py
+-rw-rw-rw-   0        0        0     3547 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_account.py
+-rw-rw-rw-   0        0        0     3489 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_admin.py
+-rw-rw-rw-   0        0        0     4114 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_license.py
+-rw-rw-rw-   0        0        0     5149 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_pending.py
+-rw-rw-rw-   0        0        0     3543 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_rating.py
+-rw-rw-rw-   0        0        0     7377 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/all_license_price.py
+-rw-rw-rw-   0        0        0    22811 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/blended_package.py
+-rw-rw-rw-   0        0        0     3503 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body.py
+-rw-rw-rw-   0        0        0     3727 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body_1.py
+-rw-rw-rw-   0        0        0     7110 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages.py
+-rw-rw-rw-   0        0        0    12189 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages_error.py
+-rw-rw-rw-   0        0        0    18472 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/canonical_version.py
+-rw-rw-rw-   0        0        0     3615 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_current_account.py
+-rw-rw-rw-   0        0        0     3735 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_privilege.py
+-rw-rw-rw-   0        0        0     5504 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_account.py
+-rw-rw-rw-   0        0        0     4973 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_canonical.py
+-rw-rw-rw-   0        0        0     4853 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_package.py
+-rw-rw-rw-   0        0        0     7008 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_version.py
+-rw-rw-rw-   0        0        0     5695 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies.py
+-rw-rw-rw-   0        0        0     4261 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies_list.py
+-rw-rw-rw-   0        0        0    11135 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail.py
+-rw-rw-rw-   0        0        0     5279 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail_dependency_of_package.py
+-rw-rw-rw-   0        0        0     4151 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/documents.py
+-rw-rw-rw-   0        0        0     4125 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error.py
+-rw-rw-rw-   0        0        0     5150 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response400.py
+-rw-rw-rw-   0        0        0     5198 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response401.py
+-rw-rw-rw-   0        0        0     9159 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response409.py
+-rw-rw-rw-   0        0        0     9152 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response412.py
+-rw-rw-rw-   0        0        0     6037 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response500.py
+-rw-rw-rw-   0        0        0     8824 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/failed_dependency_error.py
+-rw-rw-rw-   0        0        0     4246 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_account.py
+-rw-rw-rw-   0        0        0     3645 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_canonical_version.py
+-rw-rw-rw-   0        0        0     7652 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_current_account.py
+-rw-rw-rw-   0        0        0     4399 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_dependency_packages.py
+-rw-rw-rw-   0        0        0     9790 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_draft.py
+-rw-rw-rw-   0        0        0     4256 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_licenses.py
+-rw-rw-rw-   0        0        0     4308 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_pending_user.py
+-rw-rw-rw-   0        0        0     4239 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_ratings.py
+-rw-rw-rw-   0        0        0     4201 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_user.py
+-rw-rw-rw-   0        0        0     4286 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_validators.py
+-rw-rw-rw-   0        0        0    10246 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_package.py
+-rw-rw-rw-   0        0        0     4251 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_packages.py
+-rw-rw-rw-   0        0        0     3735 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/inline_response_200.py
+-rw-rw-rw-   0        0        0     5230 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/license.py
+-rw-rw-rw-   0        0        0     4598 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/like.py
+-rw-rw-rw-   0        0        0     5095 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/login.py
+-rw-rw-rw-   0        0        0     3651 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/logout.py
+-rw-rw-rw-   0        0        0     4919 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/new_draft.py
+-rw-rw-rw-   0        0        0     2986 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/operands.py
+-rw-rw-rw-   0        0        0     6127 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_detail_data.py
+-rw-rw-rw-   0        0        0     5293 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_images.py
+-rw-rw-rw-   0        0        0     4181 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/packages.py
+-rw-rw-rw-   0        0        0     5560 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_user.py
+-rw-rw-rw-   0        0        0     4212 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_users.py
+-rw-rw-rw-   0        0        0    10618 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication.py
+-rw-rw-rw-   0        0        0    14020 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_error.py
+-rw-rw-rw-   0        0        0    17540 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_validation_error.py
+-rw-rw-rw-   0        0        0     8618 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version.py
+-rw-rw-rw-   0        0        0     8540 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version_error.py
+-rw-rw-rw-   0        0        0     4303 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions.py
+-rw-rw-rw-   0        0        0     4368 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions_error.py
+-rw-rw-rw-   0        0        0     5025 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications.py
+-rw-rw-rw-   0        0        0     7275 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications_error.py
+-rw-rw-rw-   0        0        0     5218 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/rating.py
+-rw-rw-rw-   0        0        0    13040 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reject_acquisition_package.py
+-rw-rw-rw-   0        0        0     4502 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/remove_pending.py
+-rw-rw-rw-   0        0        0     3659 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_account_verification_link.py
+-rw-rw-rw-   0        0        0     5940 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_invite.py
+-rw-rw-rw-   0        0        0     3624 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reset_password.py
+-rw-rw-rw-   0        0        0    16618 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_result.py
+-rw-rw-rw-   0        0        0     5002 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_results.py
+-rw-rw-rw-   0        0        0     5133 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/session_data.py
+-rw-rw-rw-   0        0        0     4390 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/share_approval_list_error.py
+-rw-rw-rw-   0        0        0     9362 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_account.py
+-rw-rw-rw-   0        0        0     4385 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_accounts_list.py
+-rw-rw-rw-   0        0        0     9033 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_account.py
+-rw-rw-rw-   0        0        0     4935 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_draft.py
+-rw-rw-rw-   0        0        0     3569 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_license.py
+-rw-rw-rw-   0        0        0     6351 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_package.py
+-rw-rw-rw-   0        0        0     4537 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_publication.py
+-rw-rw-rw-   0        0        0     3780 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_version.py
+-rw-rw-rw-   0        0        0     4799 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/upload_media.py
+-rw-rw-rw-   0        0        0    12227 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/user.py
+-rw-rw-rw-   0        0        0     4121 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/users.py
+-rw-rw-rw-   0        0        0     8930 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator.py
+-rw-rw-rw-   0        0        0     6347 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_detail.py
+-rw-rw-rw-   0        0        0     6614 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_plan.py
+-rw-rw-rw-   0        0        0     9282 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_sets_in_badge.py
+-rw-rw-rw-   0        0        0    17690 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/version.py
+-rw-rw-rw-   0        0        0     4152 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/versions.py
+-rw-rw-rw-   0        0        0     9542 2023-04-24 05:51:06.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/rest.py
+-rw-rw-rw-   0        0        0     3319 2023-07-13 13:32:53.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/tests.py
+-rw-rw-rw-   0        0        0    11975 2023-07-06 12:33:23.000000 blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/transform_image.py
+-rw-rw-rw-   0        0        0     4612 2023-07-13 13:32:53.000000 blendedux-0.1.0/blendedUx/blended_flask/functions.py
+-rw-rw-rw-   0        0        0      329 2023-05-03 09:50:10.000000 blendedux-0.1.0/blendedUx/blended_flask/settings.py
+-rw-rw-rw-   0        0        0     3799 2023-07-13 13:32:53.000000 blendedux-0.1.0/blendedUx/blended_flask/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:54:07.662301 blendedux-0.1.0/blendedux.egg-info/
+-rw-rw-rw-   0        0        0     5406 2023-07-14 05:54:06.000000 blendedux-0.1.0/blendedux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10128 2023-07-14 05:54:06.000000 blendedux-0.1.0/blendedux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 05:54:06.000000 blendedux-0.1.0/blendedux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      234 2023-07-14 05:54:06.000000 blendedux-0.1.0/blendedux.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 05:54:06.000000 blendedux-0.1.0/blendedux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 05:54:07.669596 blendedux-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1060 2023-07-14 05:52:37.000000 blendedux-0.1.0/setup.py
```

### Comparing `blendedux-0.0.2/LICENSE` & `blendedux-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/PKG-INFO` & `blendedux-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,61 +1,67 @@
 Metadata-Version: 2.1
 Name: blendedux
-Version: 0.0.2
+Version: 0.1.0
 Summary: A cross-platform design theme framework.
+Home-page: UNKNOWN
 Author: Himanshu
 Author-email: <hbhadu@cognam.com>
-License: MIT
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Blended python flask is a web framework, it is a python module that lets you develop web applications easily. Flask is very Pythonic. It is easy to get started with Flask, because it does not have a huge learning curve. On top of that it is very explicit, which increases readability. Simply, you can install the blended python flask, specify the path of your theme, run the server and can browse your website which is running on a Blended theme.
 
 ## Installation
 
-pip install blendedux
+pip install ux-blended
 
 ## Usages
 
 #### Setup of Blended Python Flask
 
-Run the following commands sequentially. First will create virtual environment, second will take you to the newly created virtual environment, third will activate the virtual environment and fourth will install blendedux inside the virtual environment.
+Run the following commands sequentially. First will create virtual environment, second will take you to the newly created virtual environment, third will activate the virtual environment and fourth will install ux-blended inside the virtual environment.
 ```
 python -m virtualenv env_name
 cd env_name
 Scripts\activate
-pip install blendedux
+pip install ux-blended
 ```
 
 #### Create a file name app.py in the root directory and paste below line of code and save.
 
 ```
-import os
 from flask import Flask
-app = Flask(__name__)
 from blendedUx import *
+from blendedUx.blended_flask.bl_flask_app import Bl_Flask
 
-PACKAGE_DIR = "Package directory"
-themes = BlendedFlask(app,PACKAGE_DIR)
-user_name = 'username'
-theme_name = 'themename'
+PACKAGE_DIR = "themes-directory"
+
+app = Bl_Flask(__name__, package_dir= PACKAGE_DIR)
+
+user_name = 'user_name'
+theme_name = 'theme_name'
 password = ''
-theme = themes.load(theme_name, user_name)
-@app.route("/css/<path:path>") 
+
+theme = app.load(theme_name, user_name)
+
+@app.route("/css/<path:path>")
 @get_css('css_path')
 def css():
    pass
 @app.route("/media/<path:path>")
 @get_media('media_path')
 def media():
     pass
 @app.route("/js/<path:path>")
 @get_js('js_path')
 def js():
     pass
+
 @app.route('/')
 def home(**kwargs):
     """
     """
     context = theme
     file_content = get_template('home.html')
     try:
@@ -147,7 +153,9 @@
 ```
 Note: It is registering the root URL for your application. This route is rendering a home.html template file by accepting the Blended theme context object. The home.html is a Blended host template and you can add many more as per your requirements in templates directory and then define a route for that template based on above code snippet in app.py. 
  
 For more details go to [Quickstart Python Flask](https://hub.blended.co/learn/quickstart_blended_flask/)
 
 ## License
 MIT
+
+
```

### Comparing `blendedux-0.0.2/README.md` & `blendedux-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 Blended python flask is a web framework, it is a python module that lets you develop web applications easily. Flask is very Pythonic. It is easy to get started with Flask, because it does not have a huge learning curve. On top of that it is very explicit, which increases readability. Simply, you can install the blended python flask, specify the path of your theme, run the server and can browse your website which is running on a Blended theme.
 
 ## Installation
 
-pip install blendedux
+pip install ux-blended
 
 ## Usages
 
 #### Setup of Blended Python Flask
 
-Run the following commands sequentially. First will create virtual environment, second will take you to the newly created virtual environment, third will activate the virtual environment and fourth will install blendedux inside the virtual environment.
+Run the following commands sequentially. First will create virtual environment, second will take you to the newly created virtual environment, third will activate the virtual environment and fourth will install ux-blended inside the virtual environment.
 ```
 python -m virtualenv env_name
 cd env_name
 Scripts\activate
-pip install blendedux
+pip install ux-blended
 ```
 
 #### Create a file name app.py in the root directory and paste below line of code and save.
 
 ```
-import os
 from flask import Flask
-app = Flask(__name__)
 from blendedUx import *
+from blendedUx.blended_flask.bl_flask_app import Bl_Flask
 
-PACKAGE_DIR = "Package directory"
-themes = BlendedFlask(app,PACKAGE_DIR)
-user_name = 'username'
-theme_name = 'themename'
+PACKAGE_DIR = "themes-directory"
+
+app = Bl_Flask(__name__, package_dir= PACKAGE_DIR)
+
+user_name = 'user_name'
+theme_name = 'theme_name'
 password = ''
-theme = themes.load(theme_name, user_name)
-@app.route("/css/<path:path>") 
+
+theme = app.load(theme_name, user_name)
+
+@app.route("/css/<path:path>")
 @get_css('css_path')
 def css():
    pass
 @app.route("/media/<path:path>")
 @get_media('media_path')
 def media():
     pass
 @app.route("/js/<path:path>")
 @get_js('js_path')
 def js():
     pass
+
 @app.route('/')
 def home(**kwargs):
     """
     """
     context = theme
     file_content = get_template('home.html')
     try:
@@ -136,8 +140,8 @@
       return render_code(file_content.decode("utf-8"), context)
 ```
 Note: It is registering the root URL for your application. This route is rendering a home.html template file by accepting the Blended theme context object. The home.html is a Blended host template and you can add many more as per your requirements in templates directory and then define a route for that template based on above code snippet in app.py. 
  
 For more details go to [Quickstart Python Flask](https://hub.blended.co/learn/quickstart_blended_flask/)
 
 ## License
-MIT
+MIT
```

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/__init__.py` & `blendedux-0.1.0/blendedUx/blended_flask/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 from blendedUx.blended_flask.blended_hostlib.backend import FileSystemBackend
 from blendedUx.blended_flask.blended_hostlib.network import Network
 from blendedUx.blended_flask.blended_hostlib.controller import Controller
 from flask import Flask, send_from_directory, send_file
 from blendedUx.blended_flask.settings import blended_static_dir
 import os
 
@@ -29,7 +31,8 @@
         context = controller.context_loader(theme_name, user_slug)
         return context
 
     def login(self, user_slug, password):
         """
         """
         pass
+
```

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/backend/backend.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/backend/backend.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/backend/intermediary.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/backend/intermediary.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/backend/settings.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/backend/settings.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/controller/controller.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/controller/controller.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/functions/functions.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/functions/functions.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/initializer.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/initializer.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/network/network.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/network/network.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/__init__.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/api_client.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/accounts_api.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/accounts_api.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/packages_api.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/apis/packages_api.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/configuration.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/__init__.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invite_pending.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invite_pending.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invites_pending_list.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/account_invites_pending_list.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/accounts.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/accounts.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response_data.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/acquisition_response_data.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/activationchallenge.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/activationchallenge.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/active_account.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/active_account.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_account.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_account.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_admin.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_admin.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_license.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_license.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_pending.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_pending.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_rating.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/add_rating.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/all_license_price.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/all_license_price.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/blended_package.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/blended_package.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body_1.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/body_1.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages_error.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/bundled_packages_error.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/canonical_version.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/canonical_version.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_current_account.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_current_account.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_privilege.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/change_privilege.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_account.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_account.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_canonical.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_canonical.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_package.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_package.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_version.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/create_version.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies_list.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependencies_list.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail_dependency_of_package.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/dependency_package_detail_dependency_of_package.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/documents.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/documents.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response400.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response400.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response401.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response401.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response409.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response409.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response412.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response412.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response500.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/error_response500.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/failed_dependency_error.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/failed_dependency_error.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_account.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_account.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_canonical_version.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_canonical_version.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_current_account.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_current_account.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_dependency_packages.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_dependency_packages.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_draft.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_draft.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_licenses.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_licenses.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_pending_user.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_pending_user.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_ratings.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_ratings.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_user.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_user.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_validators.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/hyper_link_validators.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_package.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_package.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_packages.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/initial_packages.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/inline_response_200.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/inline_response_200.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/license.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/license.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/like.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/like.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/login.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/login.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/logout.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/logout.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/new_draft.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/new_draft.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/operands.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/operands.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_detail_data.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_detail_data.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_images.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/package_images.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/packages.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/packages.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_user.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_user.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_users.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/pending_users.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_error.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_error.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_validation_error.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_validation_error.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version_error.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_version_error.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions_error.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publication_versions_error.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications_error.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/publications_error.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/rating.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/rating.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reject_acquisition_package.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reject_acquisition_package.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/remove_pending.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/remove_pending.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_account_verification_link.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_account_verification_link.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_invite.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/resend_invite.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reset_password.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/reset_password.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_result.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_result.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_results.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/search_results.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/session_data.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/session_data.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/share_approval_list_error.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/share_approval_list_error.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_account.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_account.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_accounts_list.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/shared_package_accounts_list.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_account.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_account.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_draft.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_draft.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_license.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_license.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_package.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_package.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_publication.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_publication.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_version.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/update_version.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/upload_media.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/upload_media.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/user.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/user.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/users.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/users.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_detail.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_detail.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_plan.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_plan.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_sets_in_badge.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/validator_sets_in_badge.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/version.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/version.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/models/versions.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/models/versions.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/swagger_client/rest.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/tests.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/tests.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/blended_hostlib/transform_image.py` & `blendedux-0.1.0/blendedUx/blended_flask/blended_hostlib/transform_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,16 @@
         the bounding box,
         '''
         if retain == "center":
             crop_w = (self.w-self.width)/2
             crop_h = (self.h-self.height)/2
 
             cropbox = (crop_w, crop_h, crop_w+self.width, crop_h+self.height)
-            cropbox = map(lambda x: int(x), cropbox)
+            # cropbox = map(lambda x: int(x), cropbox)
+            cropbox = list(map(int, cropbox))
 
             self.image = self.image.crop(cropbox)
             self.w, self.h = self.image.size[0]*1.0, self.image.size[1]*1.0
 
         elif retain == "top-left":
             cropbox = (0, 0, int(self.width), int(self.height))
```

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/functions.py` & `blendedux-0.1.0/blendedUx/blended_flask/functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import absolute_import
 import os.path
 from os.path import relpath
 import shutil
 import os
 import sys
 import jinja2
+import typing as t
 
-from blendedUxLang import BlendedEnvironment
+# from blendedUxLang import BlendedEnvironment
+from blended.jinjaenv import BlendedEnvironment
 from blendedUx.blended_flask.blended_hostlib.exceptions import BlendedException
 from blendedUx.blended_flask.utils import *
 
 env = BlendedEnvironment()
 
 if not os.path.exists(IMAGE_CACHE_DIR):
     os.makedirs(IMAGE_CACHE_DIR)
@@ -33,14 +35,15 @@
 def render_code(file_content, context):
     """
     :param file_content: compiled template content
     :param context: theme_object or context
     :return: rendered content of template.
     """
     template = env.from_string(file_content)
+    
     return template.render(context)
 
 def image(image_dict_obj, height=None, width=None, filters=None):
     """
     """
     if filters:
         if ((height == 0) or height) and ((width == 0) or width):
@@ -61,56 +64,83 @@
         raise BlendedException("Please pass numerical value of height and width before using filters. "
                                "Default values are (0, 0)! error in:%s)" % image_dict_obj)
     try:
         relative_path = image_dict_obj.get('path')
         output = get_image_path(relative_path, height=height, width=width, filters=filters)
         url = "blended_static/media/%s" % (relpath(output, IMAGE_CACHE_DIR))
     except jinja2.exceptions.UndefinedError as exc:
+        
         filename = exc.message.rsplit('attribute ')[1].replace("'", "")
         url = "blended_static/media/not_found/%s" % (filename)
+    
     return url
 
 def css(theme_object):
     """
     function to generate css file path dynamically.
     """
+    # breakpoint()
     css_path = theme_object.get('meta', {}).get('css', {})
     source_path = css_path.get('compile_targets')
     rendered_require = css_path.get('render_required')
     context = {'theme': dict(theme_object)}
     try:
-        css = theme_object['css']['blendedcss']
+        try: 
+            css = theme_object['css']['blendedcss']       #  code_iteration issue
+        except TypeError:
+            css = theme_object['css']     
+                 
         file_path = os.path.join(COMPILE_DIR, 'blendedcss')
         if(rendered_require):
             css = render_code(css, context)
         try:
             path = save_css(file_path, css)
         except BlendedException as exc:
             raise BlendedException(exc)
         else:
             split_path = path.split(COMPILE_DIR)
             css_file_url = split_path[1]
+            # css_file_url = "/blended_static/css/blended/blendedcss.css"
             css_file_url = "/blended_static/css/blended/%s" % (css_file_url)
             return css_file_url
     except Exception as e:
         raise(e)
 
-def url_for(path, filename=""):
-    """
-    """
-    return "/%s/%s" % (path, filename)
+from flask import url_for, get_flashed_messages
+
+# def url_for(path, filename=""):
+#     """
+#     """
+#     return "/%s/%s" % (path, filename)
 
 def blended_home():
     """
     """
-    return 'http://127.0.0.1:5000/'
+    default_host = '127.0.0.1'
+    
+    if os.environ.get("custom_host"):
+        host = os.environ.get("custom_host")
+    else:
+        host = default_host
+    if os.environ.get("custom_port"):
+        try:
+            port = int(os.environ.get("custom_port"))
+        except:
+            raise Exception("port number should be integer type!")
+    else:
+        port = 5000
+
+    return "http://%s:%s"%(host,port)
 
 def nav_links(theme, filename):
     return "%s" % (filename)
 
+
 env.globals.update({'css': css,
                     'css_links': css,
                     'nav_links': nav_links,
                     'image': image,
                     "url_for": url_for,
-                    'home': blended_home
+                    'home': blended_home,
+                    'get_flashed_messages': get_flashed_messages,
                     })
+
```

### Comparing `blendedux-0.0.2/blendedUx/blended_flask/utils.py` & `blendedux-0.1.0/blendedUx/blended_flask/utils.py`

 * *Files identical despite different names*

### Comparing `blendedux-0.0.2/blendedux.egg-info/PKG-INFO` & `blendedux-0.1.0/blendedux.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,61 +1,67 @@
 Metadata-Version: 2.1
 Name: blendedux
-Version: 0.0.2
+Version: 0.1.0
 Summary: A cross-platform design theme framework.
+Home-page: UNKNOWN
 Author: Himanshu
 Author-email: <hbhadu@cognam.com>
-License: MIT
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Blended python flask is a web framework, it is a python module that lets you develop web applications easily. Flask is very Pythonic. It is easy to get started with Flask, because it does not have a huge learning curve. On top of that it is very explicit, which increases readability. Simply, you can install the blended python flask, specify the path of your theme, run the server and can browse your website which is running on a Blended theme.
 
 ## Installation
 
-pip install blendedux
+pip install ux-blended
 
 ## Usages
 
 #### Setup of Blended Python Flask
 
-Run the following commands sequentially. First will create virtual environment, second will take you to the newly created virtual environment, third will activate the virtual environment and fourth will install blendedux inside the virtual environment.
+Run the following commands sequentially. First will create virtual environment, second will take you to the newly created virtual environment, third will activate the virtual environment and fourth will install ux-blended inside the virtual environment.
 ```
 python -m virtualenv env_name
 cd env_name
 Scripts\activate
-pip install blendedux
+pip install ux-blended
 ```
 
 #### Create a file name app.py in the root directory and paste below line of code and save.
 
 ```
-import os
 from flask import Flask
-app = Flask(__name__)
 from blendedUx import *
+from blendedUx.blended_flask.bl_flask_app import Bl_Flask
 
-PACKAGE_DIR = "Package directory"
-themes = BlendedFlask(app,PACKAGE_DIR)
-user_name = 'username'
-theme_name = 'themename'
+PACKAGE_DIR = "themes-directory"
+
+app = Bl_Flask(__name__, package_dir= PACKAGE_DIR)
+
+user_name = 'user_name'
+theme_name = 'theme_name'
 password = ''
-theme = themes.load(theme_name, user_name)
-@app.route("/css/<path:path>") 
+
+theme = app.load(theme_name, user_name)
+
+@app.route("/css/<path:path>")
 @get_css('css_path')
 def css():
    pass
 @app.route("/media/<path:path>")
 @get_media('media_path')
 def media():
     pass
 @app.route("/js/<path:path>")
 @get_js('js_path')
 def js():
     pass
+
 @app.route('/')
 def home(**kwargs):
     """
     """
     context = theme
     file_content = get_template('home.html')
     try:
@@ -147,7 +153,9 @@
 ```
 Note: It is registering the root URL for your application. This route is rendering a home.html template file by accepting the Blended theme context object. The home.html is a Blended host template and you can add many more as per your requirements in templates directory and then define a route for that template based on above code snippet in app.py. 
  
 For more details go to [Quickstart Python Flask](https://hub.blended.co/learn/quickstart_blended_flask/)
 
 ## License
 MIT
+
+
```

### Comparing `blendedux-0.0.2/blendedux.egg-info/SOURCES.txt` & `blendedux-0.1.0/blendedux.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 LICENSE
+MANIFEST.in
 README.md
 setup.py
 blendedUx/__init__.py
 blendedUx/blended_flask/__init__.py
 blendedUx/blended_flask/app.py
+blendedUx/blended_flask/bl_flask_app.py
 blendedUx/blended_flask/functions.py
 blendedUx/blended_flask/settings.py
 blendedUx/blended_flask/utils.py
 blendedUx/blended_flask/blended_hostlib/__init__.py
 blendedUx/blended_flask/blended_hostlib/initializer.py
 blendedUx/blended_flask/blended_hostlib/tests.py
 blendedUx/blended_flask/blended_hostlib/transform_image.py
```

### Comparing `blendedux-0.0.2/setup.py` & `blendedux-0.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 from setuptools import setup, find_packages
+
 import pathlib
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
-README = (HERE / "README.md").read_text()
+README = (HERE / "README.md").read_text(encoding="utf-8")
 
-VERSION = '0.0.2'
+VERSION = '0.1.0'
 DESCRIPTION = 'A cross-platform design theme framework.'
 
 
+
 # Setting up
 setup(
     name="blendedux",
     version=VERSION,
     author="Himanshu",
     author_email="<hbhadu@cognam.com>",
     description=DESCRIPTION,
     long_description=README,
     long_description_content_type="text/markdown",
-    license="MIT",
+    include_package_data = True,
     packages=find_packages(),
     install_requires=[
         'certifi==2022.5.18.1',
         'click==8.1.3',
-        'colorama==0.4.4',
-        'Flask==0.11.1',
-        'itsdangerous==2.0.1',
-        'Jinja2==2.8',
-        'MarkupSafe==2.0.1',
-        'Pillow==8.0.1',
+        'colorama==0.4.6',
+        'Flask==2.2.3',
+        'itsdangerous==2.1.2',
+        'Jinja2==3.1.2',
+        'MarkupSafe==2.1.2',
+        'Pillow==9.5.0',
         'python-dateutil==2.8.2',
         'six==1.16.0',
-        'urllib3==1.26.9',
-        'Werkzeug==2.0.3',
-        'blendedUx-Lang==1.0.0'
+        'urllib3==1.26.15',
+        'Werkzeug==2.2.3',
+        'blinker==1.6.2',
+        'blendedUx-Lang==1.1.0'
     ]
 )
```

