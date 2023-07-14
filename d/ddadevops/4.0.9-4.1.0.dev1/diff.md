# Comparing `tmp/ddadevops-4.0.9.tar.gz` & `tmp/ddadevops-4.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddadevops-4.0.9.tar", last modified: Fri Jul  7 14:41:00 2023, max compression
+gzip compressed data, was "ddadevops-4.1.0.dev1.tar", last modified: Fri Jul 14 10:01:38 2023, max compression
```

## Comparing `ddadevops-4.0.9.tar` & `ddadevops-4.1.0.dev1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:41:00.093139 ddadevops-4.0.9/
--rw-rw-r--   0 root         (0) root         (0)      137 2023-07-07 14:40:59.000000 ddadevops-4.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6727 2023-07-07 14:41:00.093139 ddadevops-4.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 14:40:59.000000 ddadevops-4.0.9/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:41:00.090139 ddadevops-4.0.9/ddadevops/
--rw-rw-rw-   0 root         (0) root         (0)    11357 2023-07-07 14:40:59.000000 ddadevops-4.0.9/ddadevops/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      640 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:41:00.090139 ddadevops-4.0.9/ddadevops/application/
--rw-rw-rw-   0 root         (0) root         (0)      150 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/application/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2463 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/application/image_build_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2525 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/application/release_mixin_services.py
--rw-rw-rw-   0 root         (0) root         (0)     9245 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/application/terraform_service.py
--rw-rw-rw-   0 root         (0) root         (0)     3953 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/aws_mfa_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1540 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/c4k_build.py
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/credential.py
--rw-rw-rw-   0 root         (0) root         (0)     1018 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/devops_build.py
--rw-rw-rw-   0 root         (0) root         (0)     1358 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/devops_image_build.py
--rw-rw-rw-   0 root         (0) root         (0)     2284 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/devops_terraform_build.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:41:00.091139 ddadevops-4.0.9/ddadevops/domain/
--rw-rw-rw-   0 root         (0) root         (0)      647 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/domain/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4845 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/domain/build_file.py
--rw-rw-rw-   0 root         (0) root         (0)     2982 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/domain/c4k.py
--rw-rw-rw-   0 root         (0) root         (0)     3284 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/domain/common.py
--rw-rw-rw-   0 root         (0) root         (0)     1916 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/domain/credentials.py
--rw-rw-rw-   0 root         (0) root         (0)     1870 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/domain/devops_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1753 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/domain/image.py
--rw-rw-rw-   0 root         (0) root         (0)     4531 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/domain/init_service.py
--rw-rw-rw-   0 root         (0) root         (0)     3687 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/domain/provider_aws.py
--rw-rw-rw-   0 root         (0) root         (0)     3891 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/domain/provider_digitalocean.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/domain/provider_hetzner.py
--rw-rw-rw-   0 root         (0) root         (0)     3422 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/domain/provs_k3s.py
--rw-rw-rw-   0 root         (0) root         (0)     2381 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/domain/release.py
--rw-rw-rw-   0 root         (0) root         (0)     4101 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/domain/terraform.py
--rw-rw-rw-   0 root         (0) root         (0)     3489 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/domain/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:41:00.092139 ddadevops-4.0.9/ddadevops/infrastructure/
--rw-rw-rw-   0 root         (0) root         (0)      226 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/infrastructure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6645 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/infrastructure/infrastructure.py
--rw-rw-rw-   0 root         (0) root         (0)     1097 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/infrastructure/repository.py
--rw-rw-rw-   0 root         (0) root         (0)     1332 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/provs_k3s_build.py
--rw-rw-rw-   0 root         (0) root         (0)     1177 2023-07-07 14:40:48.000000 ddadevops-4.0.9/ddadevops/release_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:41:00.089139 ddadevops-4.0.9/ddadevops/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:41:00.089139 ddadevops-4.0.9/ddadevops/src/main/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:41:00.089139 ddadevops-4.0.9/ddadevops/src/main/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:41:00.089139 ddadevops-4.0.9/ddadevops/src/main/resources/docker/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:41:00.089139 ddadevops-4.0.9/ddadevops/src/main/resources/docker/image/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:41:00.092139 ddadevops-4.0.9/ddadevops/src/main/resources/docker/image/resources/
--rwxrwxrwx   0 root         (0) root         (0)      628 2023-07-07 14:40:59.000000 ddadevops-4.0.9/ddadevops/src/main/resources/docker/image/resources/install_functions.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:41:00.093139 ddadevops-4.0.9/ddadevops/src/main/resources/terraform/
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-07 14:40:59.000000 ddadevops-4.0.9/ddadevops/src/main/resources/terraform/aws_backend.tf
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-07 14:40:59.000000 ddadevops-4.0.9/ddadevops/src/main/resources/terraform/aws_backend_wkms_vars.tf
--rw-rw-rw-   0 root         (0) root         (0)       65 2023-07-07 14:40:59.000000 ddadevops-4.0.9/ddadevops/src/main/resources/terraform/aws_backend_wokms_vars.tf
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-07 14:40:59.000000 ddadevops-4.0.9/ddadevops/src/main/resources/terraform/aws_provider.tf
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-07 14:40:59.000000 ddadevops-4.0.9/ddadevops/src/main/resources/terraform/aws_provider_vars.tf
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-07-07 14:40:59.000000 ddadevops-4.0.9/ddadevops/src/main/resources/terraform/do_backend.tf
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-07 14:40:59.000000 ddadevops-4.0.9/ddadevops/src/main/resources/terraform/do_backend_vars.tf
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-07-07 14:40:59.000000 ddadevops-4.0.9/ddadevops/src/main/resources/terraform/do_provider.tf
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-07 14:40:59.000000 ddadevops-4.0.9/ddadevops/src/main/resources/terraform/do_provider_vars.tf
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-07-07 14:40:59.000000 ddadevops-4.0.9/ddadevops/src/main/resources/terraform/hetzner_provider.tf
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-07-07 14:40:59.000000 ddadevops-4.0.9/ddadevops/src/main/resources/terraform/hetzner_provider_vars.tf
--rw-rw-rw-   0 root         (0) root         (0)      392 2023-07-07 14:40:59.000000 ddadevops-4.0.9/ddadevops/src/main/resources/terraform/provider_registry.tf
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-07 14:40:59.000000 ddadevops-4.0.9/ddadevops/src/main/resources/terraform/terraform_build_vars.tf
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-07 14:40:59.000000 ddadevops-4.0.9/ddadevops/src/main/resources/terraform/versions.tf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:41:00.090139 ddadevops-4.0.9/ddadevops.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6727 2023-07-07 14:41:00.000000 ddadevops-4.0.9/ddadevops.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2144 2023-07-07 14:41:00.000000 ddadevops-4.0.9/ddadevops.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 14:41:00.000000 ddadevops-4.0.9/ddadevops.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 14:41:00.000000 ddadevops-4.0.9/ddadevops.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-07 14:41:00.000000 ddadevops-4.0.9/ddadevops.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 14:41:00.000000 ddadevops-4.0.9/ddadevops.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 14:41:00.093139 ddadevops-4.0.9/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     8259 2023-07-07 14:40:59.000000 ddadevops-4.0.9/setup.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.922655 ddadevops-4.1.0.dev1/
+-rw-rw-r--   0 jem       (1000) jem       (1000)      137 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/MANIFEST.in
+-rw-rw-r--   0 jem       (1000) jem       (1000)     6698 2023-07-14 10:01:38.922655 ddadevops-4.1.0.dev1/PKG-INFO
+-rw-rw-r--   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/__init__.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.918655 ddadevops-4.1.0.dev1/ddadevops/
+-rw-rw-r--   0 jem       (1000) jem       (1000)    11357 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/LICENSE
+-rw-rw-r--   0 jem       (1000) jem       (1000)      640 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/__init__.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.918655 ddadevops-4.1.0.dev1/ddadevops/application/
+-rw-rw-r--   0 jem       (1000) jem       (1000)      150 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/application/__init__.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2668 2023-07-14 09:33:55.000000 ddadevops-4.1.0.dev1/ddadevops/application/image_build_service.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2515 2023-07-12 06:32:49.000000 ddadevops-4.1.0.dev1/ddadevops/application/release_mixin_services.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     9245 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/application/terraform_service.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     3953 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/aws_mfa_mixin.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1540 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/c4k_build.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)      504 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/credential.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1018 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/devops_build.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1358 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/devops_image_build.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2284 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/devops_terraform_build.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.922655 ddadevops-4.1.0.dev1/ddadevops/domain/
+-rw-rw-r--   0 jem       (1000) jem       (1000)      647 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/domain/__init__.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     5182 2023-07-13 06:26:15.000000 ddadevops-4.1.0.dev1/ddadevops/domain/build_file.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2982 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/domain/c4k.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     3284 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/domain/common.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1916 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/domain/credentials.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1870 2023-07-14 10:00:01.000000 ddadevops-4.1.0.dev1/ddadevops/domain/devops_factory.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2425 2023-07-14 09:33:55.000000 ddadevops-4.1.0.dev1/ddadevops/domain/image.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     4531 2023-06-27 17:01:05.000000 ddadevops-4.1.0.dev1/ddadevops/domain/init_service.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     3687 2023-07-06 16:08:05.000000 ddadevops-4.1.0.dev1/ddadevops/domain/provider_aws.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     3891 2023-07-06 16:08:05.000000 ddadevops-4.1.0.dev1/ddadevops/domain/provider_digitalocean.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)      907 2023-07-06 16:08:05.000000 ddadevops-4.1.0.dev1/ddadevops/domain/provider_hetzner.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     3422 2023-06-13 11:42:08.000000 ddadevops-4.1.0.dev1/ddadevops/domain/provs_k3s.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2381 2023-07-07 14:38:33.000000 ddadevops-4.1.0.dev1/ddadevops/domain/release.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     4101 2023-06-16 09:16:24.000000 ddadevops-4.1.0.dev1/ddadevops/domain/terraform.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     4564 2023-07-12 06:55:13.000000 ddadevops-4.1.0.dev1/ddadevops/domain/version.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.922655 ddadevops-4.1.0.dev1/ddadevops/infrastructure/
+-rw-rw-r--   0 jem       (1000) jem       (1000)      226 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/infrastructure/__init__.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     7242 2023-07-14 09:46:06.000000 ddadevops-4.1.0.dev1/ddadevops/infrastructure/infrastructure.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1097 2023-06-02 15:15:05.000000 ddadevops-4.1.0.dev1/ddadevops/infrastructure/repository.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1332 2023-06-13 11:36:37.000000 ddadevops-4.1.0.dev1/ddadevops/provs_k3s_build.py
+-rw-rw-r--   0 jem       (1000) jem       (1000)     1177 2023-06-28 06:49:15.000000 ddadevops-4.1.0.dev1/ddadevops/release_mixin.py
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.914655 ddadevops-4.1.0.dev1/ddadevops/src/
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.914655 ddadevops-4.1.0.dev1/ddadevops/src/main/
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.914655 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.914655 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/docker/
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.914655 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/docker/image/
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.922655 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/docker/image/resources/
+-rwxrwxr-x   0 jem       (1000) jem       (1000)      628 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/docker/image/resources/install_functions.sh
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.922655 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/
+-rw-rw-r--   0 jem       (1000) jem       (1000)       59 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/aws_backend.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       90 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/aws_backend_wkms_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       65 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/aws_backend_wokms_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)      113 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/aws_provider.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       83 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/aws_provider_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)      191 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/do_backend.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)      109 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/do_backend_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)      145 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/do_provider.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       99 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/do_provider_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       91 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/hetzner_provider.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       31 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/hetzner_provider_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)      392 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/provider_registry.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       40 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/terraform_build_vars.tf
+-rw-rw-r--   0 jem       (1000) jem       (1000)       46 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops/src/main/resources/terraform/versions.tf
+drwxrwxr-x   0 jem       (1000) jem       (1000)        0 2023-07-14 10:01:38.918655 ddadevops-4.1.0.dev1/ddadevops.egg-info/
+-rw-rw-r--   0 jem       (1000) jem       (1000)     6698 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops.egg-info/PKG-INFO
+-rw-rw-r--   0 jem       (1000) jem       (1000)     2144 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops.egg-info/SOURCES.txt
+-rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops.egg-info/dependency_links.txt
+-rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops.egg-info/namespace_packages.txt
+-rw-rw-r--   0 jem       (1000) jem       (1000)       11 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops.egg-info/top_level.txt
+-rw-rw-r--   0 jem       (1000) jem       (1000)        1 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/ddadevops.egg-info/zip-safe
+-rw-rw-r--   0 jem       (1000) jem       (1000)       38 2023-07-14 10:01:38.922655 ddadevops-4.1.0.dev1/setup.cfg
+-rwxr-xr-x   0 jem       (1000) jem       (1000)     8230 2023-07-14 10:01:38.000000 ddadevops-4.1.0.dev1/setup.py
```

### Comparing `ddadevops-4.0.9/PKG-INFO` & `ddadevops-4.1.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddadevops
-Version: 4.0.9
+Version: 4.1.0.dev1
 Summary: tools to support builds combining gopass, terraform, dda-pallet, aws & hetzner-cloud
 Home-page: https://repo.prod.meissa.de/meissa/dda-devops-build
 Author: meissa GmbH
 Author-email: buero@meissa-gmbh.de
 Maintainer: 
 Maintainer-email: 
 License: Apache Software License
@@ -209,15 +209,15 @@
 
 ## Snapshot & Release
 
 ```
 pyb dev publish upload
 pip3 install --upgrade ddadevops --pre
 
-pyb [patch|minor|major] prepare_release tag_bump_and_push_release
+pyb [patch|minor|major] release
 pip3 install --upgrade ddadevops
 ```
 
 ## Development & mirrors
 
 Development happens at: https://repo.prod.meissa.de/meissa/dda-devops-build
```

### Comparing `ddadevops-4.0.9/ddadevops/LICENSE` & `ddadevops-4.1.0.dev1/ddadevops/LICENSE`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/__init__.py` & `ddadevops-4.1.0.dev1/ddadevops/__init__.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/application/image_build_service.py` & `ddadevops-4.1.0.dev1/ddadevops/application/image_build_service.py`

 * *Files 15% similar despite different names*

```diff
@@ -42,26 +42,29 @@
             self.__copy_build_resources_from_package__(devops)
         else:
             self.__copy_build_resources_from_dir__(devops)
         self.file_api.cp_recursive("image", build_path)
         self.file_api.cp_recursive("test", build_path)
 
     def image(self, devops: Devops):
-        self.image_api.image(devops.name, devops.build_path())
+        image = devops.specialized_builds[BuildType.IMAGE]
+        self.image_api.image(image.image_name(), devops.build_path())
 
     def drun(self, devops: Devops):
-        self.image_api.drun(devops.name)
+        image = devops.specialized_builds[BuildType.IMAGE]
+        self.image_api.drun(image.image_name())
 
     def dockerhub_login(self, devops: Devops):
         image = devops.specialized_builds[BuildType.IMAGE]
         self.image_api.dockerhub_login(
             image.image_dockerhub_user, image.image_dockerhub_password
         )
 
     def dockerhub_publish(self, devops: Devops):
         image = devops.specialized_builds[BuildType.IMAGE]
         self.image_api.dockerhub_publish(
-            devops.name, image.image_dockerhub_user, image.image_tag
+            image.image_name(), image.image_dockerhub_user, image.image_tag
         )
 
     def test(self, devops: Devops):
-        self.image_api.test(devops.name, devops.build_path())
+        image = devops.specialized_builds[BuildType.IMAGE]
+        self.image_api.test(image.image_name(), devops.build_path())
```

### Comparing `ddadevops-4.0.9/ddadevops/application/release_mixin_services.py` & `ddadevops-4.1.0.dev1/ddadevops/application/release_mixin_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                 release_version = release.version.create_major()
             case ReleaseType.MINOR:
                 release_version = release.version.create_minor()
             case ReleaseType.PATCH:
                 release_version = release.version.create_patch()
             case _:
                 return
-        bump_version = release_version.create_bump("SNAPSHOT")
+        bump_version = release_version.create_bump()
         release_message = f"release: {release_version.to_string()}"
         bump_message = f"bump version to: {bump_version.to_string()}"
         self.git_api.tag_annotated(release_version.to_string(), release_message, 0)
         self.__set_version_and_commit__(
             bump_version,
             release.build_files(),
             bump_message,
```

### Comparing `ddadevops-4.0.9/ddadevops/application/terraform_service.py` & `ddadevops-4.1.0.dev1/ddadevops/application/terraform_service.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/aws_mfa_mixin.py` & `ddadevops-4.1.0.dev1/ddadevops/aws_mfa_mixin.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/c4k_build.py` & `ddadevops-4.1.0.dev1/ddadevops/c4k_build.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/devops_build.py` & `ddadevops-4.1.0.dev1/ddadevops/devops_build.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/devops_image_build.py` & `ddadevops-4.1.0.dev1/ddadevops/devops_image_build.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/devops_terraform_build.py` & `ddadevops-4.1.0.dev1/ddadevops/devops_terraform_build.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/domain/__init__.py` & `ddadevops-4.1.0.dev1/ddadevops/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/domain/build_file.py` & `ddadevops-4.1.0.dev1/ddadevops/domain/build_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import re
 from enum import Enum
+from typing import Optional
 from pathlib import Path
 from .common import Validateable
 from .version import Version
 
 
 class BuildFileType(Enum):
     JS = ".json"
@@ -22,17 +23,18 @@
         result = []
         result += self.__validate_is_not_empty__("file_path")
         result += self.__validate_is_not_empty__("content")
         if not self.build_file_type():
             result += [f"Suffix {self.file_path} is unknown."]
         return result
 
-    def build_file_type(self):
+    def build_file_type(self) -> Optional[BuildFileType]:
+        result: Optional[BuildFileType] = None
         if not self.file_path:
-            return None
+            return result
         config_file_type = self.file_path.suffix
         match config_file_type:
             case ".json":
                 result = BuildFileType.JS
             case ".gradle":
                 result = BuildFileType.JAVA_GRADLE
             case ".clj":
@@ -70,17 +72,17 @@
                     version_line = re.search("\\(defproject .*\n", self.content)
                     version_line_group = version_line.group()
                     version_string = re.search(
                         "[0-9]*\\.[0-9]*\\.[0-9]*(-SNAPSHOT)?", version_line_group
                     )
                     version_str = version_string.group()
         except:
-            raise Exception(f"Version not found in file {self.file_path}")
+            raise RuntimeError(f"Version not found in file {self.file_path}")
 
-        result = Version.from_str(version_str)
+        result = Version.from_str(version_str, self.get_default_suffix())
         result.throw_if_invalid()
 
         return result
 
     def set_version(self, new_version: Version):
         # TODO: How can we create regex-pattern constants to use them at both places?
         try:
@@ -109,14 +111,21 @@
                         '"[0-9]*\\.[0-9]*\\.[0-9]*(-SNAPSHOT)?"',
                         f'"{new_version.to_string()}"',
                         self.content,
                         1,
                     )
                     self.content = substitute
         except:
-            raise Exception(f"Version not found in file {self.file_path}")
+            raise RuntimeError(f"Version not found in file {self.file_path}")
+
+    def get_default_suffix(self) -> str:
+        result = "SNAPSHOT"
+        match self.build_file_type():
+            case BuildFileType.PYTHON:
+                result = "dev"
+        return result
 
     def __eq__(self, other):
         return other and self.file_path == other.file_path
 
     def __hash__(self) -> int:
         return self.file_path.__hash__()
```

### Comparing `ddadevops-4.0.9/ddadevops/domain/c4k.py` & `ddadevops-4.1.0.dev1/ddadevops/domain/c4k.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/domain/common.py` & `ddadevops-4.1.0.dev1/ddadevops/domain/common.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/domain/credentials.py` & `ddadevops-4.1.0.dev1/ddadevops/domain/credentials.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/domain/devops_factory.py` & `ddadevops-4.1.0.dev1/ddadevops/domain/devops_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         devops = Devops(inp, specialized_builds=specialized_builds, mixins=mixins)
 
         devops.throw_if_invalid()
 
         return devops
 
     def merge(self, inp: dict, context: dict, authorization: dict) -> dict:
-        return {} | context | authorization | inp
+        return {} | authorization | inp | context
 
     def parse_build_types(self, build_types: List[str]) -> List[BuildType]:
         result = []
         for build_type in build_types:
             result += [BuildType[build_type]]
         return result
```

### Comparing `ddadevops-4.0.9/ddadevops/domain/image.py` & `ddadevops-4.1.0.dev1/ddadevops/domain/image.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,67 @@
+from enum import Enum
 from typing import List, Dict
 from .common import (
     filter_none,
     Validateable,
 )
 
 
+class NamingType(Enum):
+    NAME_ONLY = 1
+    NAME_AND_MODULE = 2
+
+
 class Image(Validateable):
     def __init__(
         self,
         inp: dict,
     ):
+        self.module = inp.get("module")
+        self.name = inp.get("name")
         self.image_dockerhub_user = inp.get("image_dockerhub_user")
         self.image_dockerhub_password = inp.get("image_dockerhub_password")
         self.image_tag = inp.get("image_tag")
         self.image_build_commons_path = inp.get("image_build_commons_path")
+        self.image_naming = NamingType[inp.get("image_naming", "NAME_ONLY")]
         self.image_use_package_common_files = inp.get(
             "image_use_package_common_files", True
         )
         self.image_build_commons_dir_name = inp.get(
             "image_build_commons_dir_name", "docker"
         )
 
     def validate(self) -> List[str]:
         result = []
+        result += self.__validate_is_not_empty__("name")
         result += self.__validate_is_not_empty__("image_dockerhub_user")
         result += self.__validate_is_not_empty__("image_dockerhub_password")
+        result += self.__validate_is_not_empty__("image_naming")
         if not self.image_use_package_common_files:
             result += self.__validate_is_not_empty__("image_build_commons_path")
             result += self.__validate_is_not_empty__("image_build_commons_dir_name")
         return result
 
     def build_commons_path(self):
         commons_path = [
             self.image_build_commons_path,
             self.image_build_commons_dir_name,
         ]
         return "/".join(filter_none(commons_path)) + "/"
 
+    def image_name(self) -> str:
+        result: List[str] = [self.name]  # type: ignore
+        if (
+            self.image_naming == NamingType.NAME_AND_MODULE
+            and self.module
+            and self.module != ""
+        ):
+            result.append(self.module)
+        return "-".join(result)
+
     @classmethod
     def get_mapping_default(cls) -> List[Dict[str, str]]:
         return [
             {
                 "gopass_path": "meissa/web/docker.com",
                 "gopass_field": "login",
                 "name": "image_dockerhub_user",
```

### Comparing `ddadevops-4.0.9/ddadevops/domain/init_service.py` & `ddadevops-4.1.0.dev1/ddadevops/domain/init_service.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/domain/provider_aws.py` & `ddadevops-4.1.0.dev1/ddadevops/domain/provider_aws.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/domain/provider_digitalocean.py` & `ddadevops-4.1.0.dev1/ddadevops/domain/provider_digitalocean.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/domain/provider_hetzner.py` & `ddadevops-4.1.0.dev1/ddadevops/domain/provider_hetzner.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/domain/provs_k3s.py` & `ddadevops-4.1.0.dev1/ddadevops/domain/provs_k3s.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/domain/release.py` & `ddadevops-4.1.0.dev1/ddadevops/domain/release.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/domain/terraform.py` & `ddadevops-4.1.0.dev1/ddadevops/domain/terraform.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/domain/version.py` & `ddadevops-4.1.0.dev1/ddadevops/domain/version.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,36 +2,39 @@
 from .common import (
     Validateable,
 )
 
 
 class Version(Validateable):
     @classmethod
-    def from_str(cls, input_str: str):
+    def from_str(cls, input_str: str, default_snapshot_suffix):
         snapshot_parsed = input_str.split("-")
         version_str = snapshot_parsed[0]
         suffix_str = None
         if len(snapshot_parsed) > 1:
             suffix_str = snapshot_parsed[1]
         version_no_parsed = [int(x) for x in version_str.split(".")]
         return cls(
             version_no_parsed,
+            default_snapshot_suffix,
             suffix_str,
             input_str,
         )
 
     def __init__(
         self,
         version_list: list,
+        default_snapshot_suffix: str,
         snapshot_suffix: Optional[str] = None,
         version_str: Optional[str] = None,
     ):
         self.version_list = version_list
-        self.snapshot_suffix = snapshot_suffix
         self.version_string = version_str
+        self.snapshot_suffix = snapshot_suffix
+        self.default_snapshot_suffix = default_snapshot_suffix
 
     def __eq__(self, other):
         return other and self.to_string() == other.to_string()
 
     def __hash__(self) -> int:
         return self.to_string().__hash__()
 
@@ -43,57 +46,96 @@
         if self.is_snapshot():
             return f"{version_no}-{self.snapshot_suffix}"
         return version_no
 
     def validate(self):
         result = []
         result += self.__validate_is_not_empty__("version_list")
+        result += self.__validate_is_not_empty__("default_snapshot_suffix")
         if self.version_list and len(self.version_list) < 3:
             result += ["version_list must have at least 3 levels."]
         if (
             self.version_list
             and self.version_string
             and self.to_string() != self.version_string
         ):
             result += [
                 f"version_string not parsed correct. Input was {self.version_string} parsed was {self.to_string()}"
             ]
         return result
 
-    def create_bump(self, snapshot_suffix: Optional[str] = None):
+    def create_bump(self):
+        tmp_snapshot_suffix = self.default_snapshot_suffix
+
         new_version_list = self.version_list.copy()
         if self.is_snapshot():
             return Version(
-                new_version_list, snapshot_suffix=self.snapshot_suffix, version_str=None
+                new_version_list,
+                self.default_snapshot_suffix,
+                snapshot_suffix=tmp_snapshot_suffix,
+                version_str=None,
             )
         else:
             new_version_list[2] += 1
             return Version(
-                new_version_list, snapshot_suffix=snapshot_suffix, version_str=None
+                new_version_list,
+                self.default_snapshot_suffix,
+                snapshot_suffix=tmp_snapshot_suffix,
+                version_str=None,
             )
 
     def create_patch(self):
         new_version_list = self.version_list.copy()
         if self.is_snapshot():
-            return Version(new_version_list, snapshot_suffix=None, version_str=None)
+            return Version(
+                new_version_list,
+                self.default_snapshot_suffix,
+                snapshot_suffix=None,
+                version_str=None,
+            )
         else:
             new_version_list[2] += 1
-            return Version(new_version_list, snapshot_suffix=None, version_str=None)
+            return Version(
+                new_version_list,
+                self.default_snapshot_suffix,
+                snapshot_suffix=None,
+                version_str=None,
+            )
 
     def create_minor(self):
         new_version_list = self.version_list.copy()
         if self.is_snapshot() and new_version_list[2] == 0:
-            return Version(new_version_list, snapshot_suffix=None, version_str=None)
+            return Version(
+                new_version_list,
+                self.default_snapshot_suffix,
+                snapshot_suffix=None,
+                version_str=None,
+            )
         else:
             new_version_list[2] = 0
             new_version_list[1] += 1
-            return Version(new_version_list, snapshot_suffix=None, version_str=None)
+            return Version(
+                new_version_list,
+                self.default_snapshot_suffix,
+                snapshot_suffix=None,
+                version_str=None,
+            )
 
     def create_major(self):
         new_version_list = self.version_list.copy()
         if self.is_snapshot() and new_version_list[2] == 0 and new_version_list[1] == 0:
-            return Version(new_version_list, snapshot_suffix=None, version_str=None)
+            return Version(
+                new_version_list,
+                self.default_snapshot_suffix,
+                snapshot_suffix=None,
+                version_str=None,
+            )
         else:
             new_version_list[2] = 0
             new_version_list[1] = 0
             new_version_list[0] += 1
-            return Version(new_version_list, snapshot_suffix=None, version_str=None)
+            return Version(
+                new_version_list,
+                self.default_snapshot_suffix,
+                snapshot_suffix=None,
+                version_str=None,
+            )
```

### Comparing `ddadevops-4.0.9/ddadevops/infrastructure/infrastructure.py` & `ddadevops-4.1.0.dev1/ddadevops/infrastructure/infrastructure.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from subprocess import Popen, PIPE, run
+from subprocess import Popen, PIPE, run, CalledProcessError
 from pathlib import Path
 from sys import stdout
 from os import chmod, environ
 from json import load, dumps
 import yaml
 from pkg_resources import resource_string
 
@@ -45,63 +45,50 @@
 
     def read_json_fro_file(self, path: Path) -> map:
         with open(path, "r", encoding="utf-8") as input_file:
             return load(input_file)
 
 
 class ImageApi:
+    def __init__(self):
+        self.execution_api = ExecutionApi()
+
     def image(self, name: str, path: Path):
-        run(
-            f"docker build -t {name} --file {path}/image/Dockerfile {path}/image",
-            shell=True,
-            check=True,
+        self.execution_api.execute_live(
+            f"docker build -t {name} --file {path}/image/Dockerfile {path}/image"
         )
 
     def drun(self, name: str):
-        run(
-            f'docker run -it --entrypoint="" {name} /bin/bash',
-            shell=True,
-            check=True,
+        self.execution_api.execute_live(
+            f'docker run -it --entrypoint="" {name} /bin/bash'
         )
 
     def dockerhub_login(self, username: str, password: str):
-        run(
-            f"docker login --username {username} --password {password}",
-            shell=True,
-            check=True,
+        self.execution_api.execute_live(
+            f"docker login --username {username} --password {password}"
         )
 
     def dockerhub_publish(self, name: str, username: str, tag=None):
         if tag is not None:
-            run(
-                f"docker tag {name} {username}/{name}:{tag}",
-                shell=True,
-                check=True,
+            self.execution_api.execute_live(
+                f"docker tag {name} {username}/{name}:{tag}"
             )
-            run(
-                f"docker push {username}/{name}:{tag}",
-                shell=True,
-                check=True,
+            self.execution_api.execute_live(
+                f"docker push {username}/{name}:{tag}"
             )
-        run(
-            f"docker tag {name} {username}/{name}:latest",
-            shell=True,
-            check=True,
-        )
-        run(
-            f"docker push {username}/{name}:latest",
-            shell=True,
-            check=True,
+        self.execution_api.execute_live(
+            f"docker tag {name} {username}/{name}:latest"
+        )
+        self.execution_api.execute_live(
+            f"docker push {username}/{name}:latest"
         )
 
     def test(self, name: str, path: Path):
-        run(
-            f"docker build -t {name} -test --file {path}/test/Dockerfile {path}/test",
-            shell=True,
-            check=True,
+        self.execution_api.execute_live(
+            f"docker build -t {name} -test --file {path}/test/Dockerfile {path}/test"
         )
 
 
 class ExecutionApi:
     def execute(self, command: str, dry_run=False, shell=True, check=True):
         output = ""
         if dry_run:
@@ -110,24 +97,43 @@
             # output = check_output(command, encoding="UTF-8", shell=shell)
             output = run(
                 command, encoding="UTF-8", shell=shell, stdout=PIPE, check=check
             ).stdout
             output = output.rstrip()
         return output
 
-    def execute_live(self, command, dry_run=False, shell=True):
+    # TODO: check for exception handling
+    # TODO: can we return the output here also?
+    # TODO: should we also print stderr?
+    def execute_live(self, command: str, dry_run=False, shell=True):
         if dry_run:
             print(command)
         else:
             process = Popen(command, stdout=PIPE, shell=shell)
             for line in iter(process.stdout.readline, b""):
                 print(line.decode("utf-8"), end="")
             process.stdout.close()
             process.wait()
 
+    # TODO: move this enhancement to execute
+    def execute_handled(self, command: str, dry_run=False, shell=True, check=True):
+        if dry_run:
+            print(command)
+        else:
+            try:
+                run(
+                    command,
+                    shell=shell,
+                    check=check,
+                    stderr=PIPE,
+                    text=True)
+            except CalledProcessError as exc:
+                print("Command failed with code: ", exc.returncode, " and message:", exc.stderr)
+                raise exc
+
 
 class EnvironmentApi:
     def get(self, key):
         return environ.get(key)
 
 
 class CredentialsApi:
```

### Comparing `ddadevops-4.0.9/ddadevops/infrastructure/repository.py` & `ddadevops-4.1.0.dev1/ddadevops/infrastructure/repository.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/provs_k3s_build.py` & `ddadevops-4.1.0.dev1/ddadevops/provs_k3s_build.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/release_mixin.py` & `ddadevops-4.1.0.dev1/ddadevops/release_mixin.py`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops/src/main/resources/docker/image/resources/install_functions.sh` & `ddadevops-4.1.0.dev1/ddadevops/src/main/resources/docker/image/resources/install_functions.sh`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/ddadevops.egg-info/PKG-INFO` & `ddadevops-4.1.0.dev1/ddadevops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddadevops
-Version: 4.0.9
+Version: 4.1.0.dev1
 Summary: tools to support builds combining gopass, terraform, dda-pallet, aws & hetzner-cloud
 Home-page: https://repo.prod.meissa.de/meissa/dda-devops-build
 Author: meissa GmbH
 Author-email: buero@meissa-gmbh.de
 Maintainer: 
 Maintainer-email: 
 License: Apache Software License
@@ -209,15 +209,15 @@
 
 ## Snapshot & Release
 
 ```
 pyb dev publish upload
 pip3 install --upgrade ddadevops --pre
 
-pyb [patch|minor|major] prepare_release tag_bump_and_push_release
+pyb [patch|minor|major] release
 pip3 install --upgrade ddadevops
 ```
 
 ## Development & mirrors
 
 Development happens at: https://repo.prod.meissa.de/meissa/dda-devops-build
```

### Comparing `ddadevops-4.0.9/ddadevops.egg-info/SOURCES.txt` & `ddadevops-4.1.0.dev1/ddadevops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ddadevops-4.0.9/setup.py` & `ddadevops-4.1.0.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'ddadevops',
-        version = '4.0.9',
+        version = '4.1.0-dev1',
         description = 'tools to support builds combining gopass, terraform, dda-pallet, aws & hetzner-cloud',
-        long_description = '# dda-devops-build\n\n[![Slack](https://img.shields.io/badge/chat-clojurians-green.svg?style=flat)](https://clojurians.slack.com/messages/#dda-pallet/) | [<img src="https://meissa-gmbh.de/img/community/Mastodon_Logotype.svg" width=20 alt="team@social.meissa-gmbh.de"> team@social.meissa-gmbh.de](https://social.meissa-gmbh.de/@team) | [Website & Blog](https://domaindrivenarchitecture.org)\n\n![release prod](https://github.com/DomainDrivenArchitecture/dda-devops-build/workflows/release%20prod/badge.svg)\n\ndda-devops-build integrates all the tools we use to work with clouds & provide some nice functions around.\n\nTools we support are\n\n* terraform: for setting up the plain infrastructure around.\n* docker: for creating images\n* c4k: for generating kubernetes manifests\n* provs: for setting up small single-node k3s clusters\n* gopass: for credential management on devops computers\n* cloud providers: hetzner, digitalocean, aws\n\nIn addition we provide a ReleaseMixin for release related tasks like tag / publish & version-bump\n\n```mermaid\nclassDiagram\n    class DevopsBuild {\n        name()\n        build_path()\n        initialize_build_dir()\n    }\n\n    class DevopsTerraformBuild {\n        initialize_build_dir()\n        post_build()\n        read_output_json()\n        plan()\n        plan_fail_on_diff()\n        apply(auto_approve=False)\n        refresh()\n        destroy(auto_approve=False)\n        tf_import(tf_import_name,tf_import_resource)\n    }\n\n    class DevopsImageBuild {\n        initialize_build_dir()\n        image()\n        drun()\n        dockerhub_login()\n        dockerhub_publish()\n        test()\n    }\n\n    class ReleaseMixin {\n        prepare_release()\n        tag_and_push_release()\n    }\n    \n    class ProvsK3sBuild {\n        def update_runtime_config(dns_record)\n        write_provs_config()\n        provs_apply(dry_run=False)\n    }\n\n    class C4kBuild {\n        def update_runtime_config(dns_record)\n        def write_c4k_config()\n        def write_c4k_auth()\n        c4k_apply(dry_run=False)\n    }\n\n    DevopsBuild <|-- DevopsImageBuild\n    DevopsBuild <|-- DevopsTerraformBuild\n    DevopsBuild <|-- ReleaseMixin\n    DevopsBuild <|-- ProvsK3sBuild\n    DevopsBuild <|-- C4kBuild\n\n    link DevopsBuild "./doc/DevopsBuild.md"\n    link DevopsImageBuild "./doc/DevopsImageBuild.md"\n    link DevopsTerraformBuild "./doc/DevopsTerraformBuild.md"\n    link ReleaseMixin "./doc/ReleaseMixin.md"\n    link ProvsK3sBuild "doc/ProvsK3sBuild.md"\n    link C4kBuild "doc/C4kBuild.md"\n\n```\n\nPrinciples we follow are:\n\n* Seperate build artefacts from version controlled code\n* Domain Driven Design - in order to stay sustainable\n\n## Installation\n\nEnsure that yout python3 version is at least Python 3.10\n\n```\nsudo apt install python3-pip\npip3 install -r requirements.txt\nexport PATH=$PATH:~/.local/bin\n```\n\n## Reference\n\n* [DevopsBuild](./doc/DevopsBuild.md)\n* [DevopsImageBuild](./doc/DevopsImageBuild.md)\n* [DevopsTerraformBuild](./doc/DevopsTerraformBuild.md)\n  * [AwsProvider](doc/DevopsTerraformBuildWithAwsProvider.md)\n  * [DigitaloceanProvider](doc/DevopsTerraformBuildWithDigitaloceanProvider.md)\n  * [HetznerProvider](doc/DevopsTerraformBuildWithHetznerProvider.md)\n* [ReleaseMixin](./doc/ReleaseMixin.md)\n* [ProvsK3sBuild](doc/ProvsK3sBuild.md)\n* [C4kBuild](doc/C4kBuild.md)\n\n## Example Build\n\nlets assume the following project structure\n\n```\nmy-project\n   | -> my-module\n   |       | -> build.py\n   |       | -> some-terraform.tf\n   | -> an-other-module\n   | -> target  (here will the build happen)\n   |       | -> ...\n```\n\n```python\nfrom pybuilder.core import task, init\nfrom ddadevops import *\n\nname = \'my-project\'\nMODULE = \'my-module\'\nPROJECT_ROOT_PATH = \'..\'\n\n\n@init\ndef initialize(project):\n    project.build_depends_on("ddadevops>=4.0.0-dev")\n\n    config = {\n        "credentials_mapping": [\n            {\n                "gopass_path": environ.get("DIGITALOCEAN_TOKEN_KEY_PATH", None),\n                "name": "do_api_key",\n            },\n            {\n                "gopass_path": environ.get("HETZNER_API_KEY_PATH", None),\n                "name": "hetzner_api_key",\n            },\n        ],\n        "name": name,\n        "module": MODULE,\n        "stage": environ["STAGE"],\n        "project_root_path": PROJECT_ROOT_PATH,\n        "build_types": ["TERRAFORM"],\n        "mixin_types": [],\n        "tf_provider_types": ["DIGITALOCEAN", "HETZNER"],\n        "tf_use_workspace": False,\n        "tf_terraform_semantic_version": "1.4.2",\n        "do_as_backend": True,\n        "do_bucket": "your-bucket",\n    }\n\n    build = DevopsTerraformBuild(project, config)\n    build.initialize_build_dir()\n\n\n@task\ndef plan(project):\n    build = get_devops_build(project)\n    build.plan()\n\n\n@task\ndef apply(project):\n    build = get_devops_build(project)\n    build.apply(True)\n\n\n@task\ndef destroy(project):\n    build = get_devops_build(project)\n    build.destroy(True)\n\n```\n\n## Snapshot & Release\n\n```\npyb dev publish upload\npip3 install --upgrade ddadevops --pre\n\npyb [patch|minor|major] prepare_release tag_bump_and_push_release\npip3 install --upgrade ddadevops\n```\n\n## Development & mirrors\n\nDevelopment happens at: https://repo.prod.meissa.de/meissa/dda-devops-build\n\nMirrors are:\n\n* https://gitlab.com/domaindrivenarchitecture/dda-devops-build (issues and PR, CI)\n\nFor more details about our repository model see: https://repo.prod.meissa.de/meissa/federate-your-repos\n\n## License\n\nCopyright © 2021 meissa GmbH\nLicensed under the [Apache License, Version 2.0](LICENSE) (the "License")\n\n## License\n\nCopyright © 2023 meissa GmbH\nLicensed under the [Apache License, Version 2.0](LICENSE) (the "License")\n',
+        long_description = '# dda-devops-build\n\n[![Slack](https://img.shields.io/badge/chat-clojurians-green.svg?style=flat)](https://clojurians.slack.com/messages/#dda-pallet/) | [<img src="https://meissa-gmbh.de/img/community/Mastodon_Logotype.svg" width=20 alt="team@social.meissa-gmbh.de"> team@social.meissa-gmbh.de](https://social.meissa-gmbh.de/@team) | [Website & Blog](https://domaindrivenarchitecture.org)\n\n![release prod](https://github.com/DomainDrivenArchitecture/dda-devops-build/workflows/release%20prod/badge.svg)\n\ndda-devops-build integrates all the tools we use to work with clouds & provide some nice functions around.\n\nTools we support are\n\n* terraform: for setting up the plain infrastructure around.\n* docker: for creating images\n* c4k: for generating kubernetes manifests\n* provs: for setting up small single-node k3s clusters\n* gopass: for credential management on devops computers\n* cloud providers: hetzner, digitalocean, aws\n\nIn addition we provide a ReleaseMixin for release related tasks like tag / publish & version-bump\n\n```mermaid\nclassDiagram\n    class DevopsBuild {\n        name()\n        build_path()\n        initialize_build_dir()\n    }\n\n    class DevopsTerraformBuild {\n        initialize_build_dir()\n        post_build()\n        read_output_json()\n        plan()\n        plan_fail_on_diff()\n        apply(auto_approve=False)\n        refresh()\n        destroy(auto_approve=False)\n        tf_import(tf_import_name,tf_import_resource)\n    }\n\n    class DevopsImageBuild {\n        initialize_build_dir()\n        image()\n        drun()\n        dockerhub_login()\n        dockerhub_publish()\n        test()\n    }\n\n    class ReleaseMixin {\n        prepare_release()\n        tag_and_push_release()\n    }\n    \n    class ProvsK3sBuild {\n        def update_runtime_config(dns_record)\n        write_provs_config()\n        provs_apply(dry_run=False)\n    }\n\n    class C4kBuild {\n        def update_runtime_config(dns_record)\n        def write_c4k_config()\n        def write_c4k_auth()\n        c4k_apply(dry_run=False)\n    }\n\n    DevopsBuild <|-- DevopsImageBuild\n    DevopsBuild <|-- DevopsTerraformBuild\n    DevopsBuild <|-- ReleaseMixin\n    DevopsBuild <|-- ProvsK3sBuild\n    DevopsBuild <|-- C4kBuild\n\n    link DevopsBuild "./doc/DevopsBuild.md"\n    link DevopsImageBuild "./doc/DevopsImageBuild.md"\n    link DevopsTerraformBuild "./doc/DevopsTerraformBuild.md"\n    link ReleaseMixin "./doc/ReleaseMixin.md"\n    link ProvsK3sBuild "doc/ProvsK3sBuild.md"\n    link C4kBuild "doc/C4kBuild.md"\n\n```\n\nPrinciples we follow are:\n\n* Seperate build artefacts from version controlled code\n* Domain Driven Design - in order to stay sustainable\n\n## Installation\n\nEnsure that yout python3 version is at least Python 3.10\n\n```\nsudo apt install python3-pip\npip3 install -r requirements.txt\nexport PATH=$PATH:~/.local/bin\n```\n\n## Reference\n\n* [DevopsBuild](./doc/DevopsBuild.md)\n* [DevopsImageBuild](./doc/DevopsImageBuild.md)\n* [DevopsTerraformBuild](./doc/DevopsTerraformBuild.md)\n  * [AwsProvider](doc/DevopsTerraformBuildWithAwsProvider.md)\n  * [DigitaloceanProvider](doc/DevopsTerraformBuildWithDigitaloceanProvider.md)\n  * [HetznerProvider](doc/DevopsTerraformBuildWithHetznerProvider.md)\n* [ReleaseMixin](./doc/ReleaseMixin.md)\n* [ProvsK3sBuild](doc/ProvsK3sBuild.md)\n* [C4kBuild](doc/C4kBuild.md)\n\n## Example Build\n\nlets assume the following project structure\n\n```\nmy-project\n   | -> my-module\n   |       | -> build.py\n   |       | -> some-terraform.tf\n   | -> an-other-module\n   | -> target  (here will the build happen)\n   |       | -> ...\n```\n\n```python\nfrom pybuilder.core import task, init\nfrom ddadevops import *\n\nname = \'my-project\'\nMODULE = \'my-module\'\nPROJECT_ROOT_PATH = \'..\'\n\n\n@init\ndef initialize(project):\n    project.build_depends_on("ddadevops>=4.0.0-dev")\n\n    config = {\n        "credentials_mapping": [\n            {\n                "gopass_path": environ.get("DIGITALOCEAN_TOKEN_KEY_PATH", None),\n                "name": "do_api_key",\n            },\n            {\n                "gopass_path": environ.get("HETZNER_API_KEY_PATH", None),\n                "name": "hetzner_api_key",\n            },\n        ],\n        "name": name,\n        "module": MODULE,\n        "stage": environ["STAGE"],\n        "project_root_path": PROJECT_ROOT_PATH,\n        "build_types": ["TERRAFORM"],\n        "mixin_types": [],\n        "tf_provider_types": ["DIGITALOCEAN", "HETZNER"],\n        "tf_use_workspace": False,\n        "tf_terraform_semantic_version": "1.4.2",\n        "do_as_backend": True,\n        "do_bucket": "your-bucket",\n    }\n\n    build = DevopsTerraformBuild(project, config)\n    build.initialize_build_dir()\n\n\n@task\ndef plan(project):\n    build = get_devops_build(project)\n    build.plan()\n\n\n@task\ndef apply(project):\n    build = get_devops_build(project)\n    build.apply(True)\n\n\n@task\ndef destroy(project):\n    build = get_devops_build(project)\n    build.destroy(True)\n\n```\n\n## Snapshot & Release\n\n```\npyb dev publish upload\npip3 install --upgrade ddadevops --pre\n\npyb [patch|minor|major] release\npip3 install --upgrade ddadevops\n```\n\n## Development & mirrors\n\nDevelopment happens at: https://repo.prod.meissa.de/meissa/dda-devops-build\n\nMirrors are:\n\n* https://gitlab.com/domaindrivenarchitecture/dda-devops-build (issues and PR, CI)\n\nFor more details about our repository model see: https://repo.prod.meissa.de/meissa/federate-your-repos\n\n## License\n\nCopyright © 2021 meissa GmbH\nLicensed under the [Apache License, Version 2.0](LICENSE) (the "License")\n\n## License\n\nCopyright © 2023 meissa GmbH\nLicensed under the [Apache License, Version 2.0](LICENSE) (the "License")\n',
         long_description_content_type = 'text/markdown',
         classifiers = [
             'License :: OSI Approved :: Apache Software License',
             'Programming Language :: Python',
             'Programming Language :: Python :: 3',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.10',
```

