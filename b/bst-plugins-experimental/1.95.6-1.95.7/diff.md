# Comparing `tmp/bst-plugins-experimental-1.95.6.tar.gz` & `tmp/bst-plugins-experimental-1.95.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bst-plugins-experimental-1.95.6.tar", last modified: Sat Feb 25 17:00:27 2023, max compression
+gzip compressed data, was "bst-plugins-experimental-1.95.7.tar", last modified: Fri Jul 14 20:01:35 2023, max compression
```

## Comparing `bst-plugins-experimental-1.95.6.tar` & `bst-plugins-experimental-1.95.7.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-02-25 17:00:27.168530 bst-plugins-experimental-1.95.6/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    26471 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/LICENSE
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)       66 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/MANIFEST.in
--rw-r--r--   0 testuser  (1000) testuser  (1000)     3135 2023-02-25 17:00:27.168530 bst-plugins-experimental-1.95.6/PKG-INFO
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2705 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/README.rst
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      759 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/project.conf
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-02-25 17:00:27.149315 bst-plugins-experimental-1.95.6/requirements/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      205 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/requirements/plugin-requirements.txt
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      166 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/requirements/test-requirements.txt
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      546 2023-02-25 17:00:27.169445 bst-plugins-experimental-1.95.6/setup.cfg
--rwxrwxrwx   0 testuser  (1000) testuser  (1000)     4616 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/setup.py
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-02-25 17:00:27.143825 bst-plugins-experimental-1.95.6/src/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-02-25 17:00:27.150230 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)       42 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/__init__.py
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-02-25 17:00:27.162125 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/__init__.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2574 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/bazel_build.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1082 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/bazel_build.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    13870 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/bazelize.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      244 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/bazelize.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2087 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/check_forbidden.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3925 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/collect_integration.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    11735 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/collect_manifest.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     8503 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/dpkg_build.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1536 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/dpkg_build.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    10286 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/dpkg_deploy.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      912 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/dpkg_deploy.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2752 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/fastboot_bootimg.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1354 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/fastboot_bootimg.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3023 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/fastboot_ext4.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1045 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/fastboot_ext4.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4630 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/flatpak_image.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)       36 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/flatpak_image.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4757 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/flatpak_repo.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1432 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/flatpak_repo.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1634 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/makemaker.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1074 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/makemaker.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1650 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/modulebuild.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1079 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/modulebuild.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    35986 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/oci.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      985 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/pyproject.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      339 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/pyproject.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1570 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/qmake.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      894 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/qmake.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2841 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/snap_image.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)       60 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/snap_image.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3979 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/tar_element.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      286 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/tar_element.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3021 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/x86image.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4551 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/x86image.yaml
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-02-25 17:00:27.165785 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/__init__.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    13058 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/bazel_source.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     7560 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/cpan.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     8759 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/deb.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1685 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/git_module.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    13538 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/git_repo.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    35320 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/git_tag.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     9055 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/ostree.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2512 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/patch_queue.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     9718 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/pypi.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2672 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/quilt.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     6947 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/zip.py
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-02-25 17:00:27.165785 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/testutils/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      375 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/testutils/__init__.py
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-02-25 17:00:27.166700 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/testutils/repo/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      106 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/testutils/repo/__init__.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3831 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/testutils/repo/gitrepo.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1883 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/testutils/repo/ostreerepo.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      743 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/testutils/repo/tarrepo.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      946 2023-02-25 17:00:14.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/testutils/repo/ziprepo.py
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-02-25 17:00:27.151145 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental.egg-info/
--rw-r--r--   0 testuser  (1000) testuser  (1000)     3135 2023-02-25 17:00:26.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental.egg-info/PKG-INFO
--rw-r--r--   0 testuser  (1000) testuser  (1000)     3432 2023-02-25 17:00:27.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental.egg-info/SOURCES.txt
--rw-r--r--   0 testuser  (1000) testuser  (1000)        1 2023-02-25 17:00:26.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental.egg-info/dependency_links.txt
--rw-r--r--   0 testuser  (1000) testuser  (1000)     1807 2023-02-25 17:00:26.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental.egg-info/entry_points.txt
--rw-r--r--   0 testuser  (1000) testuser  (1000)        1 2023-02-25 17:00:26.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental.egg-info/not-zip-safe
--rw-r--r--   0 testuser  (1000) testuser  (1000)       40 2023-02-25 17:00:26.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental.egg-info/requires.txt
--rw-r--r--   0 testuser  (1000) testuser  (1000)       25 2023-02-25 17:00:26.000000 bst-plugins-experimental-1.95.6/src/bst_plugins_experimental.egg-info/top_level.txt
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-02-25 17:00:27.146570 bst-plugins-experimental-1.95.6/venv/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-02-25 17:00:27.144740 bst-plugins-experimental-1.95.6/venv/lib/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-02-25 17:00:27.146570 bst-plugins-experimental-1.95.6/venv/lib/python3.10/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-02-25 17:00:27.146570 bst-plugins-experimental-1.95.6/venv/lib/python3.10/site-packages/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-02-25 17:00:27.168530 bst-plugins-experimental-1.95.6/venv/lib/python3.10/site-packages/markdown_it/
--rw-r--r--   0 testuser  (1000) testuser  (1000)     2516 2023-02-25 17:00:25.000000 bst-plugins-experimental-1.95.6/venv/lib/python3.10/site-packages/markdown_it/port.yaml
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-02-25 17:00:27.146570 bst-plugins-experimental-1.95.6/venv/lib64/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-02-25 17:00:27.147485 bst-plugins-experimental-1.95.6/venv/lib64/python3.10/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-02-25 17:00:27.147485 bst-plugins-experimental-1.95.6/venv/lib64/python3.10/site-packages/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-02-25 17:00:27.168530 bst-plugins-experimental-1.95.6/venv/lib64/python3.10/site-packages/markdown_it/
--rw-r--r--   0 testuser  (1000) testuser  (1000)     2516 2023-02-25 17:00:25.000000 bst-plugins-experimental-1.95.6/venv/lib64/python3.10/site-packages/markdown_it/port.yaml
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-07-14 20:01:35.480219 bst-plugins-experimental-1.95.7/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    26471 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/LICENSE
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)       66 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/MANIFEST.in
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     3135 2023-07-14 20:01:35.480219 bst-plugins-experimental-1.95.7/PKG-INFO
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2705 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/README.rst
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      759 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/project.conf
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-07-14 20:01:35.471219 bst-plugins-experimental-1.95.7/requirements/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      205 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/requirements/plugin-requirements.txt
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      166 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/requirements/test-requirements.txt
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      546 2023-07-14 20:01:35.481219 bst-plugins-experimental-1.95.7/setup.cfg
+-rwxrwxrwx   0 testuser  (1000) testuser  (1000)     4616 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/setup.py
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-07-14 20:01:35.468219 bst-plugins-experimental-1.95.7/src/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-07-14 20:01:35.471219 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)       42 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/__init__.py
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-07-14 20:01:35.477219 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/__init__.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2574 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/bazel_build.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1082 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/bazel_build.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    13870 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/bazelize.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      244 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/bazelize.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2087 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/check_forbidden.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3925 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/collect_integration.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    11735 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/collect_manifest.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     8503 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/dpkg_build.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1536 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/dpkg_build.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    10286 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/dpkg_deploy.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      912 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/dpkg_deploy.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2752 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/fastboot_bootimg.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1354 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/fastboot_bootimg.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3023 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/fastboot_ext4.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1045 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/fastboot_ext4.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4630 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/flatpak_image.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)       36 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/flatpak_image.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4757 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/flatpak_repo.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1432 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/flatpak_repo.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1634 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/makemaker.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1074 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/makemaker.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1650 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/modulebuild.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1079 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/modulebuild.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    35832 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/oci.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      985 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/pyproject.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      339 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/pyproject.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1570 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/qmake.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      894 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/qmake.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2841 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/snap_image.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)       60 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/snap_image.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3979 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/tar_element.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      286 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/tar_element.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3021 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/x86image.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4551 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/x86image.yaml
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-07-14 20:01:35.479219 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/__init__.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    13058 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/bazel_source.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     7560 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/cpan.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     8759 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/deb.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1685 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/git_module.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    13940 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/git_repo.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    35320 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/git_tag.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     9055 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/ostree.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2512 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/patch_queue.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     9718 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/pypi.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2672 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/quilt.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     6947 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/zip.py
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-07-14 20:01:35.479219 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/testutils/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      375 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/testutils/__init__.py
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-07-14 20:01:35.480219 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/testutils/repo/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      106 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/testutils/repo/__init__.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3831 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/testutils/repo/gitrepo.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1883 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/testutils/repo/ostreerepo.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      743 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/testutils/repo/tarrepo.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      946 2023-07-14 20:01:24.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/testutils/repo/ziprepo.py
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-07-14 20:01:35.472219 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental.egg-info/
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     3135 2023-07-14 20:01:35.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental.egg-info/PKG-INFO
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     3432 2023-07-14 20:01:35.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental.egg-info/SOURCES.txt
+-rw-r--r--   0 testuser  (1000) testuser  (1000)        1 2023-07-14 20:01:35.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental.egg-info/dependency_links.txt
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     1807 2023-07-14 20:01:35.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental.egg-info/entry_points.txt
+-rw-r--r--   0 testuser  (1000) testuser  (1000)        1 2023-07-14 20:01:35.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental.egg-info/not-zip-safe
+-rw-r--r--   0 testuser  (1000) testuser  (1000)       40 2023-07-14 20:01:35.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental.egg-info/requires.txt
+-rw-r--r--   0 testuser  (1000) testuser  (1000)       25 2023-07-14 20:01:35.000000 bst-plugins-experimental-1.95.7/src/bst_plugins_experimental.egg-info/top_level.txt
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-07-14 20:01:35.469219 bst-plugins-experimental-1.95.7/venv/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-07-14 20:01:35.469219 bst-plugins-experimental-1.95.7/venv/lib/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-07-14 20:01:35.469219 bst-plugins-experimental-1.95.7/venv/lib/python3.10/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-07-14 20:01:35.469219 bst-plugins-experimental-1.95.7/venv/lib/python3.10/site-packages/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-07-14 20:01:35.480219 bst-plugins-experimental-1.95.7/venv/lib/python3.10/site-packages/markdown_it/
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     2446 2023-07-14 20:01:34.000000 bst-plugins-experimental-1.95.7/venv/lib/python3.10/site-packages/markdown_it/port.yaml
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-07-14 20:01:35.469219 bst-plugins-experimental-1.95.7/venv/lib64/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-07-14 20:01:35.470219 bst-plugins-experimental-1.95.7/venv/lib64/python3.10/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-07-14 20:01:35.470219 bst-plugins-experimental-1.95.7/venv/lib64/python3.10/site-packages/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2023-07-14 20:01:35.480219 bst-plugins-experimental-1.95.7/venv/lib64/python3.10/site-packages/markdown_it/
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     2446 2023-07-14 20:01:34.000000 bst-plugins-experimental-1.95.7/venv/lib64/python3.10/site-packages/markdown_it/port.yaml
```

### Comparing `bst-plugins-experimental-1.95.6/LICENSE` & `bst-plugins-experimental-1.95.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/PKG-INFO` & `bst-plugins-experimental-1.95.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bst-plugins-experimental
-Version: 1.95.6
+Version: 1.95.7
 Summary: A collection of experimental BuildStream plugins.
 Home-page: https://gitlab.com/BuildStream/bst-plugins-experimental
 License: LGPL
 Project-URL: Documentation, https://buildstream.gitlab.io/bst-plugins-experimental/
 Platform: UNKNOWN
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: bazel
```

### Comparing `bst-plugins-experimental-1.95.6/README.rst` & `bst-plugins-experimental-1.95.7/README.rst`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/project.conf` & `bst-plugins-experimental-1.95.7/project.conf`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/setup.cfg` & `bst-plugins-experimental-1.95.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/setup.py` & `bst-plugins-experimental-1.95.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     encoding="utf-8",
 ) as readme:
     long_description = readme.read()
 
 
 setup(
     name="bst-plugins-experimental",
-    version="1.95.6",
+    version="1.95.7",
     description="A collection of experimental BuildStream plugins.",
     long_description=long_description,
     long_description_content_type="text/x-rst; charset=UTF-8",
     license="LGPL",
     url="https://gitlab.com/BuildStream/bst-plugins-experimental",
     project_urls={
         "Documentation": "https://buildstream.gitlab.io/bst-plugins-experimental/",
```

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/bazel_build.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/bazel_build.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/bazel_build.yaml` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/bazel_build.yaml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/bazelize.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/bazelize.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/check_forbidden.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/check_forbidden.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/collect_integration.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/collect_integration.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/collect_manifest.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/collect_manifest.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/dpkg_build.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/dpkg_build.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/dpkg_build.yaml` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/dpkg_build.yaml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/dpkg_deploy.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/dpkg_deploy.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/dpkg_deploy.yaml` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/dpkg_deploy.yaml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/fastboot_bootimg.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/fastboot_bootimg.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/fastboot_bootimg.yaml` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/fastboot_bootimg.yaml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/fastboot_ext4.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/fastboot_ext4.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/fastboot_ext4.yaml` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/fastboot_ext4.yaml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/flatpak_image.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/flatpak_image.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/flatpak_repo.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/flatpak_repo.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/flatpak_repo.yaml` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/flatpak_repo.yaml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/makemaker.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/makemaker.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/makemaker.yaml` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/makemaker.yaml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/modulebuild.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/modulebuild.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/modulebuild.yaml` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/modulebuild.yaml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/oci.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/oci.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,20 +223,30 @@
 import hashlib
 import gzip
 import json
 import codecs
 import shutil
 from contextlib import contextmanager, ExitStack
 
-from buildstream import Element, ElementError, FileType
+from buildstream import Element, ElementError, FileType, FastEnum
+
+
+class Mode(FastEnum):
+    DOCKER = "docker"
+    OCI = "oci"
 
 
 class blob:
     def __init__(
-        self, root, media_type=None, text=False, mode="oci", legacy_config=None
+        self,
+        root,
+        media_type=None,
+        text=False,
+        mode=Mode.OCI,
+        legacy_config=None,
     ):
         self.root = root
         self.descriptor = None
         self.media_type = media_type
         self.text = text
         self.mode = mode
         self.path = None
@@ -266,15 +276,15 @@
                 f.seek(0)
                 h = hashlib.sha256()
                 while True:
                     data = f.read(16 * 1204)
                     if not data:
                         break
                     h.update(data)
-                if self.mode == "oci":
+                if self.mode == Mode.OCI:
                     self.descriptor["digest"] = "sha256:{}".format(
                         h.hexdigest()
                     )
                     self.path = ["blobs", "sha256", h.hexdigest()]
                 else:
                     assert self.mode == "docker"
                     if self.media_type.endswith("+json"):
@@ -311,24 +321,16 @@
 
 class OciElement(Element):
     BST_MIN_VERSION = "2.0"
 
     def configure(self, node):
         node.validate_keys(["mode", "gzip", "images", "annotations"])
 
-        self.mode = node.get_str("mode", "oci")
-        # FIXME: use a enum with node.get_enum here
-        if self.mode not in ["docker", "oci"]:
-            raise ElementError(
-                '{}: Mode must be "oci" or "docker"'.format(
-                    node.get_scalar("mode").get_provenance()
-                )
-            )
-
-        self.gzip = node.get_bool("gzip", self.mode == "oci")
+        self.mode = node.get_enum("mode", Mode, Mode.OCI)
+        self.gzip = node.get_bool("gzip", self.mode == Mode.OCI)
 
         if "annotations" not in node:
             self.annotations = None
         else:
             self.annotations = {}
             annotations = node.get_mapping("images")
             for k, value in annotations.items():
```

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/pyproject.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/pyproject.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/qmake.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/qmake.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/qmake.yaml` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/qmake.yaml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/snap_image.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/snap_image.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/tar_element.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/tar_element.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/x86image.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/x86image.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/elements/x86image.yaml` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/elements/x86image.yaml`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/bazel_source.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/bazel_source.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/cpan.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/cpan.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/deb.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/deb.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/git_module.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/git_module.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/git_repo.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/git_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,18 +110,20 @@
             for entry in repo.get_walker(commit.id, base.parents):
                 objects[entry.commit.id] = entry.commit
 
         # The shallow bases
         shallow = [base.id]
 
         # All the tree objects. `git log .` and `git describe --dirty` need them
-        trees = []
+        trees = set()
 
         def collect_trees(repo, root_sha):
-            trees.append(root_sha)
+            if root_sha in trees:
+                return
+            trees.add(root_sha)
 
             for _, mode, sha in repo[root_sha].items():
                 if S_ISDIR(mode):
                     collect_trees(repo, sha)
 
         for obj in objects.values():
             if not isinstance(obj, Commit):
@@ -133,16 +135,21 @@
             collect_trees(repo, obj.tree)
 
         for tree in trees:
             objects[tree] = repo[tree]
 
         with Repo.init(directory) as dest:
             log.status(f"Adding {len(objects)} objects")
-            for obj in objects.values():
-                dest.object_store.add_object(obj)
+            # Takes a Sequence[Tuple[ShaFile, Optional[str]]] in theory,
+            # but in practice second field of tuple is ignored
+            # and len() is called on the sequence (so it needs to be a
+            # list, not an iterator)
+            dest.object_store.add_objects(
+                [(o, None) for o in objects.values()]
+            )
 
             if tag:
                 dest.refs[tag_ref] = tag_obj.id
 
             dest.refs[b"HEAD"] = commit.id
             dest.update_shallow(shallow, [])
 
@@ -398,14 +405,17 @@
             ]
             matching_refs = [
                 ref
                 for ref in matching_refs
                 if not any(regex.match(ref) for regex in exclude_regexs)
             ]
 
+        if not matching_refs:
+            raise SourceError("No matching refs")
+
         self.debug("Refs to be tracked", detail="\n".join(matching_refs))
 
         ref = max(matching_refs, key=version_sort_key)
 
         # peel the ref if possible
         peeled_ref = ref + "^{}"
         if peeled_ref in refs_dict:
```

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/git_tag.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/git_tag.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/ostree.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/ostree.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/patch_queue.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/patch_queue.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/pypi.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/pypi.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/quilt.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/quilt.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/sources/zip.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/sources/zip.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/testutils/repo/gitrepo.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/testutils/repo/gitrepo.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/testutils/repo/ostreerepo.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/testutils/repo/ostreerepo.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/testutils/repo/tarrepo.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/testutils/repo/tarrepo.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental/testutils/repo/ziprepo.py` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental/testutils/repo/ziprepo.py`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental.egg-info/PKG-INFO` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bst-plugins-experimental
-Version: 1.95.6
+Version: 1.95.7
 Summary: A collection of experimental BuildStream plugins.
 Home-page: https://gitlab.com/BuildStream/bst-plugins-experimental
 License: LGPL
 Project-URL: Documentation, https://buildstream.gitlab.io/bst-plugins-experimental/
 Platform: UNKNOWN
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: bazel
```

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental.egg-info/SOURCES.txt` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/src/bst_plugins_experimental.egg-info/entry_points.txt` & `bst-plugins-experimental-1.95.7/src/bst_plugins_experimental.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `bst-plugins-experimental-1.95.6/venv/lib/python3.10/site-packages/markdown_it/port.yaml` & `bst-plugins-experimental-1.95.7/venv/lib/python3.10/site-packages/markdown_it/port.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 - package: markdown-it/markdown-it
-  version: 12.2.0
-  commit: 6e2de08a0b03d3d0dcc524b89710ce05f83a0283
-  date: Aug 2, 2021
+  version: 13.0.1
+  commit: e843acc9edad115cbf8cf85e676443f01658be08
+  date: May 3, 2022
   notes:
     - Rename variables that use python built-in names, e.g.
       - `max` -> `maximum`
       - `len` -> `length`
       - `str` -> `string`
     - |
       Convert JS `for` loops to `while` loops
@@ -19,16 +19,15 @@
       `Token.attrs` is a dictionary, instead of a list of lists.
       Upstream the list format is only used to guarantee order: https://github.com/markdown-it/markdown-it/issues/142,
       but in Python 3.7+ order of dictionaries is guaranteed.
       One should anyhow use the `attrGet`, `attrSet`, `attrPush` and `attrJoin` methods
       to manipulate `Token.attrs`, which have an identical signature to those upstream.
     - Use python version of `charCodeAt`
     - |
-      Reduce use of charCodeAt() by storing char codes in a srcCharCodes attribute for state
-      objects and sharing those whenever possible
+      Use `str` units instead of `int`s to represent Unicode codepoints.
       This provides a significant performance boost
     - |
       In markdown_it/rules_block/reference.py,
       record line range in state.env["references"] and add state.env["duplicate_refs"]
       This is to allow renderers to report on issues regarding references
     - |
       The `MarkdownIt.__init__` signature is slightly different for updating options,
```

### Comparing `bst-plugins-experimental-1.95.6/venv/lib64/python3.10/site-packages/markdown_it/port.yaml` & `bst-plugins-experimental-1.95.7/venv/lib64/python3.10/site-packages/markdown_it/port.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 - package: markdown-it/markdown-it
-  version: 12.2.0
-  commit: 6e2de08a0b03d3d0dcc524b89710ce05f83a0283
-  date: Aug 2, 2021
+  version: 13.0.1
+  commit: e843acc9edad115cbf8cf85e676443f01658be08
+  date: May 3, 2022
   notes:
     - Rename variables that use python built-in names, e.g.
       - `max` -> `maximum`
       - `len` -> `length`
       - `str` -> `string`
     - |
       Convert JS `for` loops to `while` loops
@@ -19,16 +19,15 @@
       `Token.attrs` is a dictionary, instead of a list of lists.
       Upstream the list format is only used to guarantee order: https://github.com/markdown-it/markdown-it/issues/142,
       but in Python 3.7+ order of dictionaries is guaranteed.
       One should anyhow use the `attrGet`, `attrSet`, `attrPush` and `attrJoin` methods
       to manipulate `Token.attrs`, which have an identical signature to those upstream.
     - Use python version of `charCodeAt`
     - |
-      Reduce use of charCodeAt() by storing char codes in a srcCharCodes attribute for state
-      objects and sharing those whenever possible
+      Use `str` units instead of `int`s to represent Unicode codepoints.
       This provides a significant performance boost
     - |
       In markdown_it/rules_block/reference.py,
       record line range in state.env["references"] and add state.env["duplicate_refs"]
       This is to allow renderers to report on issues regarding references
     - |
       The `MarkdownIt.__init__` signature is slightly different for updating options,
```

