# Comparing `tmp/ddadevops-4.1.0.dev1.tar.gz` & `tmp/ddadevops-4.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddadevops-4.1.0.dev1.tar", last modified: Fri Jul 14 10:01:38 2023, max compression
+gzip compressed data, was "ddadevops-4.1.0.dev2.tar", last modified: Fri Jul 14 10:43:57 2023, max compression
```

## Comparing `ddadevops-4.1.0.dev1.tar` & `ddadevops-4.1.0.dev2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.922655 ddadevops-4.1.0.dev1/
--rw-rw-r--   0 jem       (1000) jem       (1000)      137 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/MANIFEST.in
--rw-rw-r--   0 jem       (1000) jem       (1000)     6698 2023-07-14 10:01:38.922655 ddadevops-4.1.0.dev1/PKG-INFO
--rw-rw-r--   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/__init__.py
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.918655 ddadevops-4.1.0.dev1/ddadevops/
--rw-rw-r--   0 jem       (1000) jem       (1000)    11357 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/LICENSE
--rw-rw-r--   0 jem       (1000) jem       (1000)      640 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/__init__.py
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.918655 ddadevops-4.1.0.dev1/ddadevops/application/
--rw-rw-r--   0 jem       (1000) jem       (1000)      150 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/application/__init__.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     2668 2023-07-14 09:33:55.000000 ddadevops-4.1.0.dev1/ddadevops/application/image_build_service.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     2515 2023-07-12 06:32:49.000000 ddadevops-4.1.0.dev1/ddadevops/application/release_mixin_services.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     9245 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/application/terraform_service.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     3953 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/aws_mfa_mixin.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     1540 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/c4k_build.py
--rw-rw-r--   0 jem       (1000) jem       (1000)      504 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/credential.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     1018 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/devops_build.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     1358 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/devops_image_build.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     2284 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/devops_terraform_build.py
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.922655 ddadevops-4.1.0.dev1/ddadevops/domain/
--rw-rw-r--   0 jem       (1000) jem       (1000)      647 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/domain/__init__.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     5182 2023-07-13 06:26:15.000000 ddadevops-4.1.0.dev1/ddadevops/domain/build_file.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     2982 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/domain/c4k.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     3284 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/domain/common.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     1916 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/domain/credentials.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     1870 2023-07-14 10:00:01.000000 ddadevops-4.1.0.dev1/ddadevops/domain/devops_factory.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     2425 2023-07-14 09:33:55.000000 ddadevops-4.1.0.dev1/ddadevops/domain/image.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     4531 2023-06-27 17:01:05.000000 ddadevops-4.1.0.dev1/ddadevops/domain/init_service.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     3687 2023-07-06 16:08:05.000000 ddadevops-4.1.0.dev1/ddadevops/domain/provider_aws.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     3891 2023-07-06 16:08:05.000000 ddadevops-4.1.0.dev1/ddadevops/domain/provider_digitalocean.py
--rw-rw-r--   0 jem       (1000) jem       (1000)      907 2023-07-06 16:08:05.000000 ddadevops-4.1.0.dev1/ddadevops/domain/provider_hetzner.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     3422 2023-06-13 11:42:08.000000 ddadevops-4.1.0.dev1/ddadevops/domain/provs_k3s.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     2381 2023-07-07 14:38:33.000000 ddadevops-4.1.0.dev1/ddadevops/domain/release.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     4101 2023-06-16 09:16:24.000000 ddadevops-4.1.0.dev1/ddadevops/domain/terraform.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     4564 2023-07-12 06:55:13.000000 ddadevops-4.1.0.dev1/ddadevops/domain/version.py
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.922655 ddadevops-4.1.0.dev1/ddadevops/infrastructure/
--rw-rw-r--   0 jem       (1000) jem       (1000)      226 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/infrastructure/__init__.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     7242 2023-07-14 09:46:06.000000 ddadevops-4.1.0.dev1/ddadevops/infrastructure/infrastructure.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     1097 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/infrastructure/repository.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     1332 2023-06-13 11:36:37.000000 ddadevops-4.1.0.dev1/ddadevops/provs_k3s_build.py
--rw-rw-r--   0 jem       (1000) jem       (1000)     1177 2023-06-28 06:49:15.000000 ddadevops-4.1.0.dev1/ddadevops/release_mixin.py
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.914655 ddadevops-4.1.0.dev1/ddadevops/src/
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.914655 ddadevops-4.1.0.dev1/ddadevops/src/main/
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.914655 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.914655 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/docker/
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.914655 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/docker/image/
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.922655 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/docker/image/resources/
--rwxrwxr-x   0 jem       (1000) jem       (1000)      628 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/docker/image/resources/install_functions.sh
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.922655 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/
--rw-rw-r--   0 jem       (1000) jem       (1000)       59 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/aws_backend.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       90 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/aws_backend_wkms_vars.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       65 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/aws_backend_wokms_vars.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)      113 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/aws_provider.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       83 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/aws_provider_vars.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)      191 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/do_backend.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)      109 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/do_backend_vars.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)      145 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/do_provider.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       99 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/do_provider_vars.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       91 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/hetzner_provider.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       31 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/hetzner_provider_vars.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)      392 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/provider_registry.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       40 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/terraform_build_vars.tf
--rw-rw-r--   0 jem       (1000) jem       (1000)       46 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/versions.tf
-drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.918655 ddadevops-4.1.0.dev1/ddadevops.egg-info/
--rw-rw-r--   0 jem       (1000) jem       (1000)     6698 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops.egg-info/PKG-INFO
--rw-rw-r--   0 jem       (1000) jem       (1000)     2144 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops.egg-info/SOURCES.txt
--rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops.egg-info/dependency_links.txt
--rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops.egg-info/namespace_packages.txt
--rw-rw-r--   0 jem       (1000) jem       (1000)       11 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops.egg-info/top_level.txt
--rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops.egg-info/zip-safe
--rw-rw-r--   0 jem       (1000) jem       (1000)       38 2023-07-14 10:01:38.922655 ddadevops-4.1.0.dev1/setup.cfg
--rwxr-xr-x   0 jem       (1000) jem       (1000)     8230 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/setup.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:43:57.228670 ddadevops-4.1.0.dev2/
+-rw-rw-r--   0 jem       (1000) jem       (1000)      137 2023-07-14 10:43:56.000000 ddadevops-4.1.0.dev2/MANIFEST.in
+-rw-rw-r--   0 jem       (1000) jem       (1000)     6698 2023-07-14 10:43:57.228670 ddadevops-4.1.0.dev2/PKG-INFO
+-rw-rw-r--   0 jem       (1000) jem       (1000)        0 2023-07-14 10:43:56.000000 ddadevops-4.1.0.dev2/__init__.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:43:57.224669 ddadevops-4.1.0.dev2/ddadevops/
+-rw-rw-r--   0 jem       (1000) jem       (1000)    11357 2023-07-14 10:43:56.000000 ddadevops-4.1.0.dev2/ddadevops/LICENSE
+-rw-rw-r--   0 jem       (1000) jem       (1000)      640 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev2/ddadevops/__init__.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:43:57.224669 ddadevops-4.1.0.dev2/ddadevops/application/
+-rw-rw-r--   0 jem       (1000) jem       (1000)      150 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev2/ddadevops/application/__init__.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2855 2023-07-14 10:39:45.000000 ddadevops-4.1.0.dev2/ddadevops/application/image_build_service.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2515 2023-07-12 06:32:49.000000 ddadevops-4.1.0.dev2/ddadevops/application/release_mixin_services.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     9245 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev2/ddadevops/application/terraform_service.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     3953 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev2/ddadevops/aws_mfa_mixin.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1540 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev2/ddadevops/c4k_build.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)      504 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev2/ddadevops/credential.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1018 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev2/ddadevops/devops_build.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1358 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev2/ddadevops/devops_image_build.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2284 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev2/ddadevops/devops_terraform_build.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:43:57.228670 ddadevops-4.1.0.dev2/ddadevops/domain/
+-rw-rw-r--   0 jem       (1000) jem       (1000)      647 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev2/ddadevops/domain/__init__.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     5182 2023-07-13 06:26:15.000000 ddadevops-4.1.0.dev2/ddadevops/domain/build_file.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2982 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev2/ddadevops/domain/c4k.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     3284 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev2/ddadevops/domain/common.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1916 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev2/ddadevops/domain/credentials.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1870 2023-07-14 10:42:15.000000 ddadevops-4.1.0.dev2/ddadevops/domain/devops_factory.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2425 2023-07-14 09:33:55.000000 ddadevops-4.1.0.dev2/ddadevops/domain/image.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     4531 2023-06-27 17:01:05.000000 ddadevops-4.1.0.dev2/ddadevops/domain/init_service.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     3687 2023-07-06 16:08:05.000000 ddadevops-4.1.0.dev2/ddadevops/domain/provider_aws.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     3891 2023-07-06 16:08:05.000000 ddadevops-4.1.0.dev2/ddadevops/domain/provider_digitalocean.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)      907 2023-07-06 16:08:05.000000 ddadevops-4.1.0.dev2/ddadevops/domain/provider_hetzner.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     3422 2023-06-13 11:42:08.000000 ddadevops-4.1.0.dev2/ddadevops/domain/provs_k3s.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2381 2023-07-07 14:38:33.000000 ddadevops-4.1.0.dev2/ddadevops/domain/release.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     4101 2023-06-16 09:16:24.000000 ddadevops-4.1.0.dev2/ddadevops/domain/terraform.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     4564 2023-07-12 06:55:13.000000 ddadevops-4.1.0.dev2/ddadevops/domain/version.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:43:57.228670 ddadevops-4.1.0.dev2/ddadevops/infrastructure/
+-rw-rw-r--   0 jem       (1000) jem       (1000)      226 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev2/ddadevops/infrastructure/__init__.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     6978 2023-07-14 10:40:42.000000 ddadevops-4.1.0.dev2/ddadevops/infrastructure/infrastructure.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1097 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev2/ddadevops/infrastructure/repository.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1332 2023-06-13 11:36:37.000000 ddadevops-4.1.0.dev2/ddadevops/provs_k3s_build.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1177 2023-06-28 06:49:15.000000 ddadevops-4.1.0.dev2/ddadevops/release_mixin.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:43:57.220669 ddadevops-4.1.0.dev2/ddadevops/src/
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:43:57.220669 ddadevops-4.1.0.dev2/ddadevops/src/main/
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:43:57.220669 ddadevops-4.1.0.dev2/ddadevops/src/main/resources/
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:43:57.220669 ddadevops-4.1.0.dev2/ddadevops/src/main/resources/docker/
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:43:57.220669 ddadevops-4.1.0.dev2/ddadevops/src/main/resources/docker/image/
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:43:57.228670 ddadevops-4.1.0.dev2/ddadevops/src/main/resources/docker/image/resources/
+-rwxrwxr-x   0 jem       (1000) jem       (1000)      628 2023-07-14 10:43:56.000000 ddadevops-4.1.0.dev2/ddadevops/src/main/resources/docker/image/resources/install_functions.sh
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:43:57.228670 ddadevops-4.1.0.dev2/ddadevops/src/main/resources/terraform/
+-rw-rw-r--   0 jem       (1000) jem       (1000)       59 2023-07-14 10:43:56.000000 ddadevops-4.1.0.dev2/ddadevops/src/main/resources/terraform/aws_backend.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       90 2023-07-14 10:43:56.000000 ddadevops-4.1.0.dev2/ddadevops/src/main/resources/terraform/aws_backend_wkms_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       65 2023-07-14 10:43:56.000000 ddadevops-4.1.0.dev2/ddadevops/src/main/resources/terraform/aws_backend_wokms_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)      113 2023-07-14 10:43:56.000000 ddadevops-4.1.0.dev2/ddadevops/src/main/resources/terraform/aws_provider.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       83 2023-07-14 10:43:56.000000 ddadevops-4.1.0.dev2/ddadevops/src/main/resources/terraform/aws_provider_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)      191 2023-07-14 10:43:56.000000 ddadevops-4.1.0.dev2/ddadevops/src/main/resources/terraform/do_backend.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)      109 2023-07-14 10:43:56.000000 ddadevops-4.1.0.dev2/ddadevops/src/main/resources/terraform/do_backend_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)      145 2023-07-14 10:43:56.000000 ddadevops-4.1.0.dev2/ddadevops/src/main/resources/terraform/do_provider.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       99 2023-07-14 10:43:56.000000 ddadevops-4.1.0.dev2/ddadevops/src/main/resources/terraform/do_provider_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       91 2023-07-14 10:43:56.000000 ddadevops-4.1.0.dev2/ddadevops/src/main/resources/terraform/hetzner_provider.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       31 2023-07-14 10:43:56.000000 ddadevops-4.1.0.dev2/ddadevops/src/main/resources/terraform/hetzner_provider_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)      392 2023-07-14 10:43:56.000000 ddadevops-4.1.0.dev2/ddadevops/src/main/resources/terraform/provider_registry.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       40 2023-07-14 10:43:56.000000 ddadevops-4.1.0.dev2/ddadevops/src/main/resources/terraform/terraform_build_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       46 2023-07-14 10:43:56.000000 ddadevops-4.1.0.dev2/ddadevops/src/main/resources/terraform/versions.tf
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:43:57.224669 ddadevops-4.1.0.dev2/ddadevops.egg-info/
+-rw-rw-r--   0 jem       (1000) jem       (1000)     6698 2023-07-14 10:43:57.000000 ddadevops-4.1.0.dev2/ddadevops.egg-info/PKG-INFO
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2144 2023-07-14 10:43:57.000000 ddadevops-4.1.0.dev2/ddadevops.egg-info/SOURCES.txt
+-rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-07-14 10:43:57.000000 ddadevops-4.1.0.dev2/ddadevops.egg-info/dependency_links.txt
+-rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-07-14 10:43:57.000000 ddadevops-4.1.0.dev2/ddadevops.egg-info/namespace_packages.txt
+-rw-rw-r--   0 jem       (1000) jem       (1000)       11 2023-07-14 10:43:57.000000 ddadevops-4.1.0.dev2/ddadevops.egg-info/top_level.txt
+-rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-07-14 10:43:57.000000 ddadevops-4.1.0.dev2/ddadevops.egg-info/zip-safe
+-rw-rw-r--   0 jem       (1000) jem       (1000)       38 2023-07-14 10:43:57.228670 ddadevops-4.1.0.dev2/setup.cfg
+-rwxr-xr-x   0 jem       (1000) jem       (1000)     8230 2023-07-14 10:43:56.000000 ddadevops-4.1.0.dev2/setup.py
```

### Comparing `ddadevops-4.1.0.dev1/PKG-INFO` & `ddadevops-4.1.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddadevops
-Version: 4.1.0.dev1
+Version: 4.1.0.dev2
 Summary: tools to support builds combining gopass, terraform, dda-pallet, aws & hetzner-cloud
 Home-page: https://repo.prod.meissa.de/meissa/dda-devops-build
 Author: meissa GmbH
 Author-email: buero@meissa-gmbh.de
 Maintainer: 
 Maintainer-email: 
 License: Apache Software License
```

### Comparing `ddadevops-4.1.0.dev1/ddadevops/LICENSE` & `ddadevops-4.1.0.dev2/ddadevops/LICENSE`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/__init__.py` & `ddadevops-4.1.0.dev2/ddadevops/__init__.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/application/image_build_service.py` & `ddadevops-4.1.0.dev2/ddadevops/application/image_build_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 from pathlib import Path
 from ..domain import Devops, BuildType
 from ..infrastructure import FileApi, ResourceApi, ImageApi
 
 
 class ImageBuildService:
-    def __init__(self, file_api: FileApi, resource_api: ResourceApi, image_api: ImageApi):
+    def __init__(
+        self, file_api: FileApi, resource_api: ResourceApi, image_api: ImageApi
+    ):
         self.file_api = file_api
         self.resource_api = resource_api
         self.image_api = image_api
 
     @classmethod
     def prod(cls):
         return cls(
             FileApi(),
             ResourceApi(),
             ImageApi(),
         )
 
     def __copy_build_resource_file_from_package__(self, resource_name, devops: Devops):
-        data = self.resource_api.read_resource(f"src/main/resources/docker/{resource_name}")
+        data = self.resource_api.read_resource(
+            f"src/main/resources/docker/{resource_name}"
+        )
         self.file_api.write_data_to_file(
             Path(f"{devops.build_path()}/{resource_name}"), data
         )
 
     def __copy_build_resources_from_package__(self, devops: Devops):
         self.__copy_build_resource_file_from_package__(
             "image/resources/install_functions.sh", devops
         )
 
     def __copy_build_resources_from_dir__(self, devops: Devops):
         image = devops.specialized_builds[BuildType.IMAGE]
-        self.file_api.cp_force(
-            image.build_commons_path(), devops.build_path()
-        )
+        self.file_api.cp_force(image.build_commons_path(), devops.build_path())
 
     def initialize_build_dir(self, devops: Devops):
         image = devops.specialized_builds[BuildType.IMAGE]
         build_path = devops.build_path()
         self.file_api.clean_dir(f"{build_path}/image/resources")
         if image.image_use_package_common_files:
             self.__copy_build_resources_from_package__(devops)
@@ -57,14 +59,18 @@
         image = devops.specialized_builds[BuildType.IMAGE]
         self.image_api.dockerhub_login(
             image.image_dockerhub_user, image.image_dockerhub_password
         )
 
     def dockerhub_publish(self, devops: Devops):
         image = devops.specialized_builds[BuildType.IMAGE]
+        if image.image_tag is not None:
+            self.image_api.dockerhub_publish(
+                image.image_name(), image.image_dockerhub_user, image.image_tag
+            )
         self.image_api.dockerhub_publish(
-            image.image_name(), image.image_dockerhub_user, image.image_tag
+            image.image_name(), image.image_dockerhub_user, 'latest'
         )
 
     def test(self, devops: Devops):
         image = devops.specialized_builds[BuildType.IMAGE]
         self.image_api.test(image.image_name(), devops.build_path())
```

### Comparing `ddadevops-4.1.0.dev1/ddadevops/application/release_mixin_services.py` & `ddadevops-4.1.0.dev2/ddadevops/application/release_mixin_services.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/application/terraform_service.py` & `ddadevops-4.1.0.dev2/ddadevops/application/terraform_service.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/aws_mfa_mixin.py` & `ddadevops-4.1.0.dev2/ddadevops/aws_mfa_mixin.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/c4k_build.py` & `ddadevops-4.1.0.dev2/ddadevops/c4k_build.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/devops_build.py` & `ddadevops-4.1.0.dev2/ddadevops/devops_build.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/devops_image_build.py` & `ddadevops-4.1.0.dev2/ddadevops/devops_image_build.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/devops_terraform_build.py` & `ddadevops-4.1.0.dev2/ddadevops/devops_terraform_build.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/domain/__init__.py` & `ddadevops-4.1.0.dev2/ddadevops/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/domain/build_file.py` & `ddadevops-4.1.0.dev2/ddadevops/domain/build_file.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/domain/c4k.py` & `ddadevops-4.1.0.dev2/ddadevops/domain/c4k.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/domain/common.py` & `ddadevops-4.1.0.dev2/ddadevops/domain/common.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/domain/credentials.py` & `ddadevops-4.1.0.dev2/ddadevops/domain/credentials.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/domain/devops_factory.py` & `ddadevops-4.1.0.dev2/ddadevops/domain/devops_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         devops = Devops(inp, specialized_builds=specialized_builds, mixins=mixins)
 
         devops.throw_if_invalid()
 
         return devops
 
     def merge(self, inp: dict, context: dict, authorization: dict) -> dict:
-        return {} | authorization | inp | context
+        return {} | context | authorization | inp
 
     def parse_build_types(self, build_types: List[str]) -> List[BuildType]:
         result = []
         for build_type in build_types:
             result += [BuildType[build_type]]
         return result
```

### Comparing `ddadevops-4.1.0.dev1/ddadevops/domain/image.py` & `ddadevops-4.1.0.dev2/ddadevops/domain/image.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/domain/init_service.py` & `ddadevops-4.1.0.dev2/ddadevops/domain/init_service.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/domain/provider_aws.py` & `ddadevops-4.1.0.dev2/ddadevops/domain/provider_aws.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/domain/provider_digitalocean.py` & `ddadevops-4.1.0.dev2/ddadevops/domain/provider_digitalocean.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/domain/provider_hetzner.py` & `ddadevops-4.1.0.dev2/ddadevops/domain/provider_hetzner.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/domain/provs_k3s.py` & `ddadevops-4.1.0.dev2/ddadevops/domain/provs_k3s.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/domain/release.py` & `ddadevops-4.1.0.dev2/ddadevops/domain/release.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/domain/terraform.py` & `ddadevops-4.1.0.dev2/ddadevops/domain/terraform.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/domain/version.py` & `ddadevops-4.1.0.dev2/ddadevops/domain/version.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/infrastructure/infrastructure.py` & `ddadevops-4.1.0.dev2/ddadevops/infrastructure/infrastructure.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,27 +63,20 @@
         )
 
     def dockerhub_login(self, username: str, password: str):
         self.execution_api.execute_live(
             f"docker login --username {username} --password {password}"
         )
 
-    def dockerhub_publish(self, name: str, username: str, tag=None):
-        if tag is not None:
-            self.execution_api.execute_live(
-                f"docker tag {name} {username}/{name}:{tag}"
-            )
-            self.execution_api.execute_live(
-                f"docker push {username}/{name}:{tag}"
-            )
+    def dockerhub_publish(self, name: str, username: str, tag: str):
         self.execution_api.execute_live(
-            f"docker tag {name} {username}/{name}:latest"
+            f"docker tag {name} {username}/{name}:{tag}"
         )
         self.execution_api.execute_live(
-            f"docker push {username}/{name}:latest"
+            f"docker push {username}/{name}:{tag}"
         )
 
     def test(self, name: str, path: Path):
         self.execution_api.execute_live(
             f"docker build -t {name} -test --file {path}/test/Dockerfile {path}/test"
         )
```

### Comparing `ddadevops-4.1.0.dev1/ddadevops/infrastructure/repository.py` & `ddadevops-4.1.0.dev2/ddadevops/infrastructure/repository.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/provs_k3s_build.py` & `ddadevops-4.1.0.dev2/ddadevops/provs_k3s_build.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/release_mixin.py` & `ddadevops-4.1.0.dev2/ddadevops/release_mixin.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops/src/main/resources/docker/image/resources/install_functions.sh` & `ddadevops-4.1.0.dev2/ddadevops/src/main/resources/docker/image/resources/install_functions.sh`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/ddadevops.egg-info/PKG-INFO` & `ddadevops-4.1.0.dev2/ddadevops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddadevops
-Version: 4.1.0.dev1
+Version: 4.1.0.dev2
 Summary: tools to support builds combining gopass, terraform, dda-pallet, aws & hetzner-cloud
 Home-page: https://repo.prod.meissa.de/meissa/dda-devops-build
 Author: meissa GmbH
 Author-email: buero@meissa-gmbh.de
 Maintainer: 
 Maintainer-email: 
 License: Apache Software License
```

### Comparing `ddadevops-4.1.0.dev1/ddadevops.egg-info/SOURCES.txt` & `ddadevops-4.1.0.dev2/ddadevops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ddadevops-4.1.0.dev1/setup.py` & `ddadevops-4.1.0.dev2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'ddadevops',
-        version = '4.1.0-dev1',
+        version = '4.1.0-dev2',
         description = 'tools to support builds combining gopass, terraform, dda-pallet, aws & hetzner-cloud',
         long_description = '# dda-devops-build\n\n[![Slack](https://img.shields.io/badge/chat-clojurians-green.svg?style=flat)](https://clojurians.slack.com/messages/#dda-pallet/) | [<img src="https://meissa-gmbh.de/img/community/Mastodon_Logotype.svg" width=20 alt="team@social.meissa-gmbh.de"> team@social.meissa-gmbh.de](https://social.meissa-gmbh.de/@team) | [Website & Blog](https://domaindrivenarchitecture.org)\n\n![release prod](https://github.com/DomainDrivenArchitecture/dda-devops-build/workflows/release%20prod/badge.svg)\n\ndda-devops-build integrates all the tools we use to work with clouds & provide some nice functions around.\n\nTools we support are\n\n* terraform: for setting up the plain infrastructure around.\n* docker: for creating images\n* c4k: for generating kubernetes manifests\n* provs: for setting up small single-node k3s clusters\n* gopass: for credential management on devops computers\n* cloud providers: hetzner, digitalocean, aws\n\nIn addition we provide a ReleaseMixin for release related tasks like tag / publish & version-bump\n\n```mermaid\nclassDiagram\n    class DevopsBuild {\n        name()\n        build_path()\n        initialize_build_dir()\n    }\n\n    class DevopsTerraformBuild {\n        initialize_build_dir()\n        post_build()\n        read_output_json()\n        plan()\n        plan_fail_on_diff()\n        apply(auto_approve=False)\n        refresh()\n        destroy(auto_approve=False)\n        tf_import(tf_import_name,tf_import_resource)\n    }\n\n    class DevopsImageBuild {\n        initialize_build_dir()\n        image()\n        drun()\n        dockerhub_login()\n        dockerhub_publish()\n        test()\n    }\n\n    class ReleaseMixin {\n        prepare_release()\n        tag_and_push_release()\n    }\n    \n    class ProvsK3sBuild {\n        def update_runtime_config(dns_record)\n        write_provs_config()\n        provs_apply(dry_run=False)\n    }\n\n    class C4kBuild {\n        def update_runtime_config(dns_record)\n        def write_c4k_config()\n        def write_c4k_auth()\n        c4k_apply(dry_run=False)\n    }\n\n    DevopsBuild <|-- DevopsImageBuild\n    DevopsBuild <|-- DevopsTerraformBuild\n    DevopsBuild <|-- ReleaseMixin\n    DevopsBuild <|-- ProvsK3sBuild\n    DevopsBuild <|-- C4kBuild\n\n    link DevopsBuild "./doc/DevopsBuild.md"\n    link DevopsImageBuild "./doc/DevopsImageBuild.md"\n    link DevopsTerraformBuild "./doc/DevopsTerraformBuild.md"\n    link ReleaseMixin "./doc/ReleaseMixin.md"\n    link ProvsK3sBuild "doc/ProvsK3sBuild.md"\n    link C4kBuild "doc/C4kBuild.md"\n\n```\n\nPrinciples we follow are:\n\n* Seperate build artefacts from version controlled code\n* Domain Driven Design - in order to stay sustainable\n\n## Installation\n\nEnsure that yout python3 version is at least Python 3.10\n\n```\nsudo apt install python3-pip\npip3 install -r requirements.txt\nexport PATH=$PATH:~/.local/bin\n```\n\n## Reference\n\n* [DevopsBuild](./doc/DevopsBuild.md)\n* [DevopsImageBuild](./doc/DevopsImageBuild.md)\n* [DevopsTerraformBuild](./doc/DevopsTerraformBuild.md)\n  * [AwsProvider](doc/DevopsTerraformBuildWithAwsProvider.md)\n  * [DigitaloceanProvider](doc/DevopsTerraformBuildWithDigitaloceanProvider.md)\n  * [HetznerProvider](doc/DevopsTerraformBuildWithHetznerProvider.md)\n* [ReleaseMixin](./doc/ReleaseMixin.md)\n* [ProvsK3sBuild](doc/ProvsK3sBuild.md)\n* [C4kBuild](doc/C4kBuild.md)\n\n## Example Build\n\nlets assume the following project structure\n\n```\nmy-project\n   | -> my-module\n   |       | -> build.py\n   |       | -> some-terraform.tf\n   | -> an-other-module\n   | -> target  (here will the build happen)\n   |       | -> ...\n```\n\n```python\nfrom pybuilder.core import task, init\nfrom ddadevops import *\n\nname = \'my-project\'\nMODULE = \'my-module\'\nPROJECT_ROOT_PATH = \'..\'\n\n\n@init\ndef initialize(project):\n    project.build_depends_on("ddadevops>=4.0.0-dev")\n\n    config = {\n        "credentials_mapping": [\n            {\n                "gopass_path": environ.get("DIGITALOCEAN_TOKEN_KEY_PATH", None),\n                "name": "do_api_key",\n            },\n            {\n                "gopass_path": environ.get("HETZNER_API_KEY_PATH", None),\n                "name": "hetzner_api_key",\n            },\n        ],\n        "name": name,\n        "module": MODULE,\n        "stage": environ["STAGE"],\n        "project_root_path": PROJECT_ROOT_PATH,\n        "build_types": ["TERRAFORM"],\n        "mixin_types": [],\n        "tf_provider_types": ["DIGITALOCEAN", "HETZNER"],\n        "tf_use_workspace": False,\n        "tf_terraform_semantic_version": "1.4.2",\n        "do_as_backend": True,\n        "do_bucket": "your-bucket",\n    }\n\n    build = DevopsTerraformBuild(project, config)\n    build.initialize_build_dir()\n\n\n@task\ndef plan(project):\n    build = get_devops_build(project)\n    build.plan()\n\n\n@task\ndef apply(project):\n    build = get_devops_build(project)\n    build.apply(True)\n\n\n@task\ndef destroy(project):\n    build = get_devops_build(project)\n    build.destroy(True)\n\n```\n\n## Snapshot & Release\n\n```\npyb dev publish upload\npip3 install --upgrade ddadevops --pre\n\npyb [patch|minor|major] release\npip3 install --upgrade ddadevops\n```\n\n## Development & mirrors\n\nDevelopment happens at: https://repo.prod.meissa.de/meissa/dda-devops-build\n\nMirrors are:\n\n* https://gitlab.com/domaindrivenarchitecture/dda-devops-build (issues and PR, CI)\n\nFor more details about our repository model see: https://repo.prod.meissa.de/meissa/federate-your-repos\n\n## License\n\nCopyright © 2021 meissa GmbH\nLicensed under the [Apache License, Version 2.0](LICENSE) (the "License")\n\n## License\n\nCopyright © 2023 meissa GmbH\nLicensed under the [Apache License, Version 2.0](LICENSE) (the "License")\n',
         long_description_content_type = 'text/markdown',
         classifiers = [
             'License :: OSI Approved :: Apache Software License',
             'Programming Language :: Python',
             'Programming Language :: Python :: 3',
```

