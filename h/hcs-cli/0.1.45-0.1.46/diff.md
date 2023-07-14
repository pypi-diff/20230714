# Comparing `tmp/hcs-cli-0.1.45.tar.gz` & `tmp/hcs-cli-0.1.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs-cli-0.1.45.tar", last modified: Wed Jul 12 01:23:09 2023, max compression
+gzip compressed data, was "hcs-cli-0.1.46.tar", last modified: Fri Jul 14 04:31:15 2023, max compression
```

## Comparing `hcs-cli-0.1.45.tar` & `hcs-cli-0.1.46.tar`

### file list

```diff
@@ -1,294 +1,297 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.314222 hcs-cli-0.1.45/
--rw-r--r--   0 nanw       (501) staff       (20)     2824 2023-06-21 18:44:48.000000 hcs-cli-0.1.45/.gitignore
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.964324 hcs-cli-0.1.45/.vscode/
--rw-r--r--   0 nanw       (501) staff       (20)     2575 2023-07-11 22:53:30.000000 hcs-cli-0.1.45/.vscode/launch.json
--rw-r--r--   0 nanw       (501) staff       (20)      179 2023-07-11 04:39:46.000000 hcs-cli-0.1.45/.vscode/settings.json
--rw-r--r--   0 nanw       (501) staff       (20)       98 2023-06-13 19:57:56.000000 hcs-cli-0.1.45/CHANGELOG.md
--rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-06-13 16:45:49.000000 hcs-cli-0.1.45/CODE_OF_CONDUCT.md
--rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-06-13 18:53:18.000000 hcs-cli-0.1.45/CONTRIBUTING_CLA.md
--rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-04-25 23:13:27.000000 hcs-cli-0.1.45/GOVERNANCE.md
--rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-06-13 16:45:49.000000 hcs-cli-0.1.45/LICENSE
--rw-r--r--   0 nanw       (501) staff       (20)      881 2023-07-11 00:05:40.000000 hcs-cli-0.1.45/Makefile
--rw-r--r--   0 nanw       (501) staff       (20)      411 2023-06-13 16:45:49.000000 hcs-cli-0.1.45/NOTICE
--rw-r--r--   0 nanw       (501) staff       (20)     3332 2023-07-12 01:23:09.313390 hcs-cli-0.1.45/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     2458 2023-07-06 08:03:28.000000 hcs-cli-0.1.45/README.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.973062 hcs-cli-0.1.45/doc/
--rw-r--r--   0 nanw       (501) staff       (20)      639 2023-07-10 17:49:04.000000 hcs-cli-0.1.45/doc/az-cheatsheet.md
--rw-r--r--   0 nanw       (501) staff       (20)     5950 2023-06-15 17:50:47.000000 hcs-cli-0.1.45/doc/dev-setup.md
--rw-r--r--   0 nanw       (501) staff       (20)      763 2023-06-13 17:49:20.000000 hcs-cli-0.1.45/doc/get-csp-user-api-token.md
--rw-r--r--   0 nanw       (501) staff       (20)     6802 2023-07-06 01:23:30.000000 hcs-cli-0.1.45/doc/hcs-cli-cheatsheet.md
--rw-r--r--   0 nanw       (501) staff       (20)     3763 2023-07-11 20:40:34.000000 hcs-cli-0.1.45/doc/hcs-plan.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.981198 hcs-cli-0.1.45/hcs_cli.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     3332 2023-07-12 01:23:08.000000 hcs-cli-0.1.45/hcs_cli.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     6841 2023-07-12 01:23:08.000000 hcs-cli-0.1.45/hcs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2023-07-12 01:23:08.000000 hcs-cli-0.1.45/hcs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)       43 2023-07-12 01:23:08.000000 hcs-cli-0.1.45/hcs_cli.egg-info/entry_points.txt
--rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-12 01:23:08.000000 hcs-cli-0.1.45/hcs_cli.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)       11 2023-07-12 01:23:08.000000 hcs-cli-0.1.45/hcs_cli.egg-info/top_level.txt
--rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.45/mypy.ini
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.905978 hcs-cli-0.1.45/payload/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.983219 hcs-cli-0.1.45/payload/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.45/payload/lcm/zero.json
--rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-06-13 19:56:09.000000 hcs-cli-0.1.45/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      194 2023-07-05 20:09:57.000000 hcs-cli-0.1.45/requirements-dev.txt
--rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-05 20:09:23.000000 hcs-cli-0.1.45/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2023-07-12 01:23:09.314554 hcs-cli-0.1.45/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-07-12 01:23:03.000000 hcs-cli-0.1.45/setup.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.987826 hcs-cli-0.1.45/tests/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.45/tests/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/tests/conftest.py
--rw-r--r--   0 nanw       (501) staff       (20)     3364 2023-07-05 16:02:01.000000 hcs-cli-0.1.45/tests/test_utils.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.989835 hcs-cli-0.1.45/tests/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.45/tests/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.991711 hcs-cli-0.1.45/tests/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.45/tests/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.998246 hcs-cli-0.1.45/tests/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.45/tests/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.000978 hcs-cli-0.1.45/tests/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.45/tests/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/tests/vhcs/cli/cmds/pki/get_root_ca.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.003989 hcs-cli-0.1.45/tests/vhcs/cli/cmds/plan/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-07-05 15:13:25.000000 hcs-cli-0.1.45/tests/vhcs/cli/cmds/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     9018 2023-07-11 08:13:52.000000 hcs-cli-0.1.45/tests/vhcs/cli/cmds/plan/test_plan.py
--rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/tests/vhcs/cli/cmds/test_context.py
--rw-r--r--   0 nanw       (501) staff       (20)      918 2023-07-03 19:18:10.000000 hcs-cli-0.1.45/tests/vhcs/cli/cmds/test_login.py
--rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-07-05 08:29:47.000000 hcs-cli-0.1.45/tests/vhcs/cli/cmds/test_profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.006774 hcs-cli-0.1.45/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.45/vhcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      687 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/__main__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.010230 hcs-cli-0.1.45/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.45/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.014609 hcs-cli-0.1.45/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.45/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.016288 hcs-cli-0.1.45/vhcs/cli/cmds/admin/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.018703 hcs-cli-0.1.45/vhcs/cli/cmds/admin/azure-infra/
--rw-r--r--   0 nanw       (501) staff       (20)     1069 2023-06-27 20:44:31.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/azure-infra/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.025652 hcs-cli-0.1.45/vhcs/cli/cmds/admin/edge/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/edge/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      941 2023-07-10 08:17:03.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/edge/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      852 2023-07-06 14:26:46.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/edge/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.028763 hcs-cli-0.1.45/vhcs/cli/cmds/admin/provider/
--rw-r--r--   0 nanw       (501) staff       (20)      986 2023-07-07 17:12:04.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1136 2023-06-15 22:34:38.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.035232 hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      949 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1841 2023-06-23 17:01:30.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.040531 hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/vm/
--rw-r--r--   0 nanw       (501) staff       (20)      622 2023-07-08 00:36:46.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/vm/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1018 2023-07-08 00:40:33.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/vm/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      953 2023-07-08 00:39:35.000000 hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/vm/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.042573 hcs-cli-0.1.45/vhcs/cli/cmds/auth/
--rw-r--r--   0 nanw       (501) staff       (20)      632 2023-07-11 01:47:20.000000 hcs-cli-0.1.45/vhcs/cli/cmds/auth/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.046452 hcs-cli-0.1.45/vhcs/cli/cmds/auth/admin/
--rw-r--r--   0 nanw       (501) staff       (20)      642 2023-07-11 01:47:42.000000 hcs-cli-0.1.45/vhcs/cli/cmds/auth/admin/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      931 2023-07-11 01:50:03.000000 hcs-cli-0.1.45/vhcs/cli/cmds/auth/admin/get_org_idp_map.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.047780 hcs-cli-0.1.45/vhcs/cli/cmds/daas/
--rw-r--r--   0 nanw       (501) staff       (20)      642 2023-06-15 22:15:00.000000 hcs-cli-0.1.45/vhcs/cli/cmds/daas/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.052883 hcs-cli-0.1.45/vhcs/cli/cmds/daas/infra/
--rw-r--r--   0 nanw       (501) staff       (20)      648 2023-06-21 17:56:47.000000 hcs-cli-0.1.45/vhcs/cli/cmds/daas/infra/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1041 2023-06-30 16:52:44.000000 hcs-cli-0.1.45/vhcs/cli/cmds/daas/infra/basic.py
--rw-r--r--   0 nanw       (501) staff       (20)     2571 2023-07-11 23:45:56.000000 hcs-cli-0.1.45/vhcs/cli/cmds/daas/infra/plan.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.059865 hcs-cli-0.1.45/vhcs/cli/cmds/daas/tenant/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-21 17:36:22.000000 hcs-cli-0.1.45/vhcs/cli/cmds/daas/tenant/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     4978 2023-07-12 00:02:14.000000 hcs-cli-0.1.45/vhcs/cli/cmds/daas/tenant/plan.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.068731 hcs-cli-0.1.45/vhcs/cli/cmds/ims/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-27 19:52:41.000000 hcs-cli-0.1.45/vhcs/cli/cmds/ims/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      915 2023-06-27 19:56:58.000000 hcs-cli-0.1.45/vhcs/cli/cmds/ims/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     1033 2023-06-27 20:14:16.000000 hcs-cli-0.1.45/vhcs/cli/cmds/ims/list_copies.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.075804 hcs-cli-0.1.45/vhcs/cli/cmds/inventory/
--rw-r--r--   0 nanw       (501) staff       (20)      637 2023-07-08 00:10:13.000000 hcs-cli-0.1.45/vhcs/cli/cmds/inventory/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1065 2023-07-08 00:42:44.000000 hcs-cli-0.1.45/vhcs/cli/cmds/inventory/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      958 2023-07-08 00:42:48.000000 hcs-cli-0.1.45/vhcs/cli/cmds/inventory/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.078752 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-27 19:52:37.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.106282 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/provider/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/provider/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      801 2023-06-23 02:35:21.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      792 2023-06-23 02:35:30.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      987 2023-06-23 02:35:40.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.137168 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/
--rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1857 2023-06-23 02:36:50.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/create.py
--rw-r--r--   0 nanw       (501) staff       (20)     1079 2023-06-23 02:36:58.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      840 2023-06-23 02:37:07.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1588 2023-06-23 02:37:18.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-06-23 02:37:44.000000 hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/wait.py
--rw-r--r--   0 nanw       (501) staff       (20)     6922 2023-07-06 00:55:04.000000 hcs-cli-0.1.45/vhcs/cli/cmds/login.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.921392 hcs-cli-0.1.45/vhcs/cli/cmds/org/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.139319 hcs-cli-0.1.45/vhcs/cli/cmds/org/datacenter/
--rw-r--r--   0 nanw       (501) staff       (20)      848 2023-06-30 15:40:06.000000 hcs-cli-0.1.45/vhcs/cli/cmds/org/datacenter/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      997 2023-06-30 15:40:15.000000 hcs-cli-0.1.45/vhcs/cli/cmds/org/datacenter/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.141544 hcs-cli-0.1.45/vhcs/cli/cmds/org/detail/
--rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:40:19.000000 hcs-cli-0.1.45/vhcs/cli/cmds/org/detail/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1201 2023-06-30 15:40:25.000000 hcs-cli-0.1.45/vhcs/cli/cmds/org/detail/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.148062 hcs-cli-0.1.45/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-13 19:45:45.000000 hcs-cli-0.1.45/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-06-30 15:38:40.000000 hcs-cli-0.1.45/vhcs/cli/cmds/pki/delete_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:38:40.000000 hcs-cli-0.1.45/vhcs/cli/cmds/pki/get_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      775 2023-06-30 15:38:40.000000 hcs-cli-0.1.45/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)     1804 2023-06-30 15:38:40.000000 hcs-cli-0.1.45/vhcs/cli/cmds/pki/sign_resource_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      726 2023-06-30 15:38:40.000000 hcs-cli-0.1.45/vhcs/cli/cmds/pki/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.152243 hcs-cli-0.1.45/vhcs/cli/cmds/plan/
--rw-r--r--   0 nanw       (501) staff       (20)      665 2023-06-28 17:52:44.000000 hcs-cli-0.1.45/vhcs/cli/cmds/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1777 2023-07-11 20:14:16.000000 hcs-cli-0.1.45/vhcs/cli/cmds/plan/deploy.py
--rw-r--r--   0 nanw       (501) staff       (20)     1556 2023-07-11 20:14:11.000000 hcs-cli-0.1.45/vhcs/cli/cmds/plan/destroy.py
--rw-r--r--   0 nanw       (501) staff       (20)     1660 2023-07-11 23:15:11.000000 hcs-cli-0.1.45/vhcs/cli/cmds/plan/graph.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.154025 hcs-cli-0.1.45/vhcs/cli/cmds/portal/
--rw-r--r--   0 nanw       (501) staff       (20)      634 2023-07-10 08:01:20.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.158555 hcs-cli-0.1.45/vhcs/cli/cmds/portal/entitlement/
--rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-11 03:23:55.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/entitlement/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      942 2023-07-11 20:54:29.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/entitlement/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      968 2023-07-11 03:24:19.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/entitlement/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      868 2023-07-11 03:24:49.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/entitlement/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.164345 hcs-cli-0.1.45/vhcs/cli/cmds/portal/pool/
--rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-10 08:01:44.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/pool/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      929 2023-07-11 20:55:25.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/pool/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      954 2023-07-10 08:18:40.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/pool/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      937 2023-07-10 08:26:34.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/pool/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.169662 hcs-cli-0.1.45/vhcs/cli/cmds/portal/site/
--rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-11 20:43:14.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/site/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-07-11 20:56:15.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/site/create.py
--rw-r--r--   0 nanw       (501) staff       (20)      928 2023-07-11 20:56:11.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/site/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      948 2023-07-11 20:56:50.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/site/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      854 2023-07-11 20:56:58.000000 hcs-cli-0.1.45/vhcs/cli/cmds/portal/site/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.171948 hcs-cli-0.1.45/vhcs/cli/cmds/profile/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.45/vhcs/cli/cmds/profile/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1765 2023-07-05 06:16:00.000000 hcs-cli-0.1.45/vhcs/cli/cmds/profile/init.py
--rw-r--r--   0 nanw       (501) staff       (20)      932 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/cli/cmds/upgrade.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.173031 hcs-cli-0.1.45/vhcs/cli/cmds/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/cli/cmds/vmhub/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.176356 hcs-cli-0.1.45/vhcs/cli/cmds/vmhub/otp/
--rw-r--r--   0 nanw       (501) staff       (20)      643 2023-06-29 21:49:43.000000 hcs-cli-0.1.45/vhcs/cli/cmds/vmhub/otp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1234 2023-06-29 21:49:20.000000 hcs-cli-0.1.45/vhcs/cli/cmds/vmhub/otp/redeem.py
--rw-r--r--   0 nanw       (501) staff       (20)     1143 2023-06-29 21:49:25.000000 hcs-cli-0.1.45/vhcs/cli/cmds/vmhub/otp/request.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2865 2023-06-23 02:40:39.000000 hcs-cli-0.1.45/vhcs/cli/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.181233 hcs-cli-0.1.45/vhcs/common/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.45/vhcs/common/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.200313 hcs-cli-0.1.45/vhcs/common/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)     1538 2023-07-03 20:20:16.000000 hcs-cli-0.1.45/vhcs/common/ctxp/README.md
--rw-r--r--   0 nanw       (501) staff       (20)      790 2023-07-03 20:45:37.000000 hcs-cli-0.1.45/vhcs/common/ctxp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-07-03 21:18:13.000000 hcs-cli-0.1.45/vhcs/common/ctxp/_init.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.204096 hcs-cli-0.1.45/vhcs/common/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.45/vhcs/common/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2421 2023-06-21 17:26:56.000000 hcs-cli-0.1.45/vhcs/common/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     3989 2023-07-05 23:22:13.000000 hcs-cli-0.1.45/vhcs/common/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     5129 2023-07-05 06:22:51.000000 hcs-cli-0.1.45/vhcs/common/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)      936 2023-07-03 21:17:12.000000 hcs-cli-0.1.45/vhcs/common/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-03 21:08:50.000000 hcs-cli-0.1.45/vhcs/common/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     6467 2023-06-23 00:26:19.000000 hcs-cli-0.1.45/vhcs/common/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/common/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     3060 2023-07-11 23:13:07.000000 hcs-cli-0.1.45/vhcs/common/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     5526 2023-07-11 08:29:40.000000 hcs-cli-0.1.45/vhcs/common/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-07-05 06:52:28.000000 hcs-cli-0.1.45/vhcs/common/ctxp/profile_store.py
--rw-r--r--   0 nanw       (501) staff       (20)     1604 2023-07-03 22:06:25.000000 hcs-cli-0.1.45/vhcs/common/ctxp/state.py
--rw-r--r--   0 nanw       (501) staff       (20)     6356 2023-07-11 02:38:58.000000 hcs-cli-0.1.45/vhcs/common/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/common/ctxp/var_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     2259 2023-07-05 18:05:17.000000 hcs-cli-0.1.45/vhcs/common/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     4846 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/common/logger.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.211971 hcs-cli-0.1.45/vhcs/common/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)      654 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/common/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     4648 2023-07-07 17:06:56.000000 hcs-cli-0.1.45/vhcs/common/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     8079 2023-07-05 07:42:49.000000 hcs-cli-0.1.45/vhcs/common/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     5200 2023-07-10 08:10:53.000000 hcs-cli-0.1.45/vhcs/common/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      906 2023-07-07 17:01:14.000000 hcs-cli-0.1.45/vhcs/common/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)     8243 2023-07-05 08:11:32.000000 hcs-cli-0.1.45/vhcs/common/sglib/login_support.py
--rw-r--r--   0 nanw       (501) staff       (20)     1443 2023-07-06 01:06:43.000000 hcs-cli-0.1.45/vhcs/common/sglib/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     9805 2023-07-11 07:29:39.000000 hcs-cli-0.1.45/vhcs/common/util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.214942 hcs-cli-0.1.45/vhcs/config/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.45/vhcs/config/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-07-03 22:19:24.000000 hcs-cli-0.1.45/vhcs/config/hcs-deployments.yaml
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.221082 hcs-cli-0.1.45/vhcs/plan/
--rw-r--r--   0 nanw       (501) staff       (20)       74 2023-07-11 20:07:10.000000 hcs-cli-0.1.45/vhcs/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)    14123 2023-07-12 01:16:46.000000 hcs-cli-0.1.45/vhcs/plan/core.py
--rw-r--r--   0 nanw       (501) staff       (20)     6729 2023-07-11 20:34:43.000000 hcs-cli-0.1.45/vhcs/plan/dag.py
--rw-r--r--   0 nanw       (501) staff       (20)     5469 2023-07-11 07:19:12.000000 hcs-cli-0.1.45/vhcs/plan/helper.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.222776 hcs-cli-0.1.45/vhcs/plan/provider/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-28 17:25:18.000000 hcs-cli-0.1.45/vhcs/plan/provider/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.234079 hcs-cli-0.1.45/vhcs/plan/provider/azure/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:51:51.000000 hcs-cli-0.1.45/vhcs/plan/provider/azure/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     4831 2023-07-12 00:07:32.000000 hcs-cli-0.1.45/vhcs/plan/provider/azure/_az_facade.py
--rw-r--r--   0 nanw       (501) staff       (20)      575 2023-06-30 00:26:03.000000 hcs-cli-0.1.45/vhcs/plan/provider/azure/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1196 2023-07-11 02:17:50.000000 hcs-cli-0.1.45/vhcs/plan/provider/azure/aad_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     1669 2023-07-11 02:11:35.000000 hcs-cli-0.1.45/vhcs/plan/provider/azure/aad_user.py
--rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-11 21:11:11.000000 hcs-cli-0.1.45/vhcs/plan/provider/azure/nsg.py
--rw-r--r--   0 nanw       (501) staff       (20)      982 2023-07-11 21:13:28.000000 hcs-cli-0.1.45/vhcs/plan/provider/azure/resource_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     1259 2023-07-12 00:09:22.000000 hcs-cli-0.1.45/vhcs/plan/provider/azure/subnet.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.237646 hcs-cli-0.1.45/vhcs/plan/provider/dev/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-07-05 15:12:02.000000 hcs-cli-0.1.45/vhcs/plan/provider/dev/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-07-05 15:12:02.000000 hcs-cli-0.1.45/vhcs/plan/provider/dev/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1351 2023-07-11 05:50:09.000000 hcs-cli-0.1.45/vhcs/plan/provider/dev/dummy.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.246338 hcs-cli-0.1.45/vhcs/plan/provider/hcs/
--rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-29 23:41:13.000000 hcs-cli-0.1.45/vhcs/plan/provider/hcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-06-29 23:41:19.000000 hcs-cli-0.1.45/vhcs/plan/provider/hcs/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1042 2023-07-11 08:52:37.000000 hcs-cli-0.1.45/vhcs/plan/provider/hcs/entitlement.py
--rw-r--r--   0 nanw       (501) staff       (20)     1326 2023-07-11 08:39:38.000000 hcs-cli-0.1.45/vhcs/plan/provider/hcs/launch_item.py
--rw-r--r--   0 nanw       (501) staff       (20)     1227 2023-07-12 00:45:19.000000 hcs-cli-0.1.45/vhcs/plan/provider/hcs/pool_group.py
--rw-r--r--   0 nanw       (501) staff       (20)     1685 2023-07-11 01:24:50.000000 hcs-cli-0.1.45/vhcs/plan/provider/hcs/pool_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     1087 2023-07-11 21:01:33.000000 hcs-cli-0.1.45/vhcs/plan/provider/hcs/site.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.248657 hcs-cli-0.1.45/vhcs/service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.45/vhcs/service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1586 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/service/_util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.255410 hcs-cli-0.1.45/vhcs/service/admin/
--rw-r--r--   0 nanw       (501) staff       (20)       59 2023-06-27 20:41:57.000000 hcs-cli-0.1.45/vhcs/service/admin/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-07-06 14:56:48.000000 hcs-cli-0.1.45/vhcs/service/admin/azure_infra.py
--rw-r--r--   0 nanw       (501) staff       (20)     1042 2023-07-10 08:03:20.000000 hcs-cli-0.1.45/vhcs/service/admin/edge.py
--rw-r--r--   0 nanw       (501) staff       (20)     1265 2023-06-23 01:29:22.000000 hcs-cli-0.1.45/vhcs/service/admin/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     1103 2023-06-27 19:44:57.000000 hcs-cli-0.1.45/vhcs/service/admin/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     2731 2023-07-10 05:17:36.000000 hcs-cli-0.1.45/vhcs/service/admin/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.258001 hcs-cli-0.1.45/vhcs/service/auth/
--rw-r--r--   0 nanw       (501) staff       (20)       19 2023-06-22 18:49:46.000000 hcs-cli-0.1.45/vhcs/service/auth/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      851 2023-06-22 18:45:24.000000 hcs-cli-0.1.45/vhcs/service/auth/admin.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.264172 hcs-cli-0.1.45/vhcs/service/ims_catalog/
--rw-r--r--   0 nanw       (501) staff       (20)       42 2023-06-27 19:54:19.000000 hcs-cli-0.1.45/vhcs/service/ims_catalog/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1218 2023-07-06 14:39:54.000000 hcs-cli-0.1.45/vhcs/service/ims_catalog/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)      915 2023-07-06 14:43:11.000000 hcs-cli-0.1.45/vhcs/service/ims_catalog/image_copies.py
--rw-r--r--   0 nanw       (501) staff       (20)      909 2023-06-22 01:03:55.000000 hcs-cli-0.1.45/vhcs/service/ims_catalog/images.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.266484 hcs-cli-0.1.45/vhcs/service/inventory/
--rw-r--r--   0 nanw       (501) staff       (20)       25 2023-07-08 00:42:34.000000 hcs-cli-0.1.45/vhcs/service/inventory/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1290 2023-07-08 00:32:38.000000 hcs-cli-0.1.45/vhcs/service/inventory/vm.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.270067 hcs-cli-0.1.45/vhcs/service/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)       32 2023-06-22 18:49:27.000000 hcs-cli-0.1.45/vhcs/service/lcm/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1437 2023-06-22 18:48:08.000000 hcs-cli-0.1.45/vhcs/service/lcm/provider.py
--rw-r--r--   0 nanw       (501) staff       (20)     2770 2023-06-22 18:47:45.000000 hcs-cli-0.1.45/vhcs/service/lcm/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.273806 hcs-cli-0.1.45/vhcs/service/org_service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:56.000000 hcs-cli-0.1.45/vhcs/service/org_service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1083 2023-06-30 15:37:59.000000 hcs-cli-0.1.45/vhcs/service/org_service/datacenter.py
--rw-r--r--   0 nanw       (501) staff       (20)     1040 2023-06-30 15:37:42.000000 hcs-cli-0.1.45/vhcs/service/org_service/details.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.276046 hcs-cli-0.1.45/vhcs/service/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:50.000000 hcs-cli-0.1.45/vhcs/service/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-06-30 15:38:16.000000 hcs-cli-0.1.45/vhcs/service/pki/certificate.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.280580 hcs-cli-0.1.45/vhcs/service/portal/
--rw-r--r--   0 nanw       (501) staff       (20)       37 2023-07-11 20:44:21.000000 hcs-cli-0.1.45/vhcs/service/portal/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1277 2023-07-11 08:42:42.000000 hcs-cli-0.1.45/vhcs/service/portal/entitlement.py
--rw-r--r--   0 nanw       (501) staff       (20)     1265 2023-07-11 20:55:47.000000 hcs-cli-0.1.45/vhcs/service/portal/pool.py
--rw-r--r--   0 nanw       (501) staff       (20)     1336 2023-07-11 21:02:10.000000 hcs-cli-0.1.45/vhcs/service/portal/site.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.282783 hcs-cli-0.1.45/vhcs/service/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)       17 2023-07-03 19:03:42.000000 hcs-cli-0.1.45/vhcs/service/vmhub/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1406 2023-06-29 21:48:05.000000 hcs-cli-0.1.45/vhcs/service/vmhub/otp.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.286390 hcs-cli-0.1.45/vhcs/support/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:35:24.000000 hcs-cli-0.1.45/vhcs/support/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.298156 hcs-cli-0.1.45/vhcs/support/daas/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-21 23:10:31.000000 hcs-cli-0.1.45/vhcs/support/daas/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     3580 2023-07-12 00:03:12.000000 hcs-cli-0.1.45/vhcs/support/daas/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     1797 2023-07-07 17:20:02.000000 hcs-cli-0.1.45/vhcs/support/daas/infra.py
--rw-r--r--   0 nanw       (501) staff       (20)     1280 2023-07-11 23:26:50.000000 hcs-cli-0.1.45/vhcs/support/daas/infra_calc.py
--rw-r--r--   0 nanw       (501) staff       (20)      424 2023-07-11 23:57:51.000000 hcs-cli-0.1.45/vhcs/support/daas/template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:08.944477 hcs-cli-0.1.45/vhcs/support/daas/templates/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.305229 hcs-cli-0.1.45/vhcs/support/daas/templates/v1/
--rw-r--r--   0 nanw       (501) staff       (20)      394 2023-07-11 23:33:48.000000 hcs-cli-0.1.45/vhcs/support/daas/templates/v1/infra.blueprint.yml
--rw-r--r--   0 nanw       (501) staff       (20)      133 2023-07-11 21:03:36.000000 hcs-cli-0.1.45/vhcs/support/daas/templates/v1/infra.vars.yml
--rw-r--r--   0 nanw       (501) staff       (20)     3645 2023-07-11 23:24:50.000000 hcs-cli-0.1.45/vhcs/support/daas/templates/v1/tenant.blueprint.yml
--rw-r--r--   0 nanw       (501) staff       (20)      224 2023-07-06 23:02:54.000000 hcs-cli-0.1.45/vhcs/support/daas/templates/v1/tenant.vars.yml
--rw-r--r--   0 nanw       (501) staff       (20)     1979 2023-06-22 21:16:18.000000 hcs-cli-0.1.45/vhcs/support/daas/tenant.py.xx
--rw-r--r--   0 nanw       (501) staff       (20)     3401 2023-07-12 00:05:12.000000 hcs-cli-0.1.45/vhcs/support/daas/tenant_calc.py
--rw-r--r--   0 nanw       (501) staff       (20)     1455 2023-07-11 20:14:32.000000 hcs-cli-0.1.45/vhcs/support/plan_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2621 2023-07-05 07:42:08.000000 hcs-cli-0.1.45/vhcs/support/profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-12 01:23:09.312008 hcs-cli-0.1.45/vhcs/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.45/vhcs/util/__init__.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/util/check_license.py
--rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/util/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1852 2023-07-08 00:14:58.000000 hcs-cli-0.1.45/vhcs/util/query_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1725 2023-06-13 19:40:36.000000 hcs-cli-0.1.45/vhcs/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.697916 hcs-cli-0.1.46/
+-rw-r--r--   0 nanw       (501) staff       (20)     2824 2023-06-21 18:44:48.000000 hcs-cli-0.1.46/.gitignore
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.372772 hcs-cli-0.1.46/.vscode/
+-rw-r--r--   0 nanw       (501) staff       (20)     2941 2023-07-12 18:10:42.000000 hcs-cli-0.1.46/.vscode/launch.json
+-rw-r--r--   0 nanw       (501) staff       (20)      179 2023-07-11 04:39:46.000000 hcs-cli-0.1.46/.vscode/settings.json
+-rw-r--r--   0 nanw       (501) staff       (20)       98 2023-06-13 19:57:56.000000 hcs-cli-0.1.46/CHANGELOG.md
+-rw-r--r--   0 nanw       (501) staff       (20)     5258 2023-06-13 16:45:49.000000 hcs-cli-0.1.46/CODE_OF_CONDUCT.md
+-rw-r--r--   0 nanw       (501) staff       (20)     2706 2023-06-13 18:53:18.000000 hcs-cli-0.1.46/CONTRIBUTING_CLA.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6095 2023-04-25 23:13:27.000000 hcs-cli-0.1.46/GOVERNANCE.md
+-rw-r--r--   0 nanw       (501) staff       (20)    10449 2023-06-13 16:45:49.000000 hcs-cli-0.1.46/LICENSE
+-rw-r--r--   0 nanw       (501) staff       (20)      881 2023-07-11 00:05:40.000000 hcs-cli-0.1.46/Makefile
+-rw-r--r--   0 nanw       (501) staff       (20)      411 2023-06-13 16:45:49.000000 hcs-cli-0.1.46/NOTICE
+-rw-r--r--   0 nanw       (501) staff       (20)     3332 2023-07-14 04:31:15.697112 hcs-cli-0.1.46/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     2458 2023-07-06 08:03:28.000000 hcs-cli-0.1.46/README.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.380883 hcs-cli-0.1.46/doc/
+-rw-r--r--   0 nanw       (501) staff       (20)      639 2023-07-10 17:49:04.000000 hcs-cli-0.1.46/doc/az-cheatsheet.md
+-rw-r--r--   0 nanw       (501) staff       (20)     5950 2023-06-15 17:50:47.000000 hcs-cli-0.1.46/doc/dev-setup.md
+-rw-r--r--   0 nanw       (501) staff       (20)      763 2023-06-13 17:49:20.000000 hcs-cli-0.1.46/doc/get-csp-user-api-token.md
+-rw-r--r--   0 nanw       (501) staff       (20)     6802 2023-07-06 01:23:30.000000 hcs-cli-0.1.46/doc/hcs-cli-cheatsheet.md
+-rw-r--r--   0 nanw       (501) staff       (20)     3763 2023-07-11 20:40:34.000000 hcs-cli-0.1.46/doc/hcs-plan.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.387186 hcs-cli-0.1.46/hcs_cli.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     3332 2023-07-14 04:31:14.000000 hcs-cli-0.1.46/hcs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     6946 2023-07-14 04:31:15.000000 hcs-cli-0.1.46/hcs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2023-07-14 04:31:14.000000 hcs-cli-0.1.46/hcs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       43 2023-07-14 04:31:14.000000 hcs-cli-0.1.46/hcs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-14 04:31:14.000000 hcs-cli-0.1.46/hcs_cli.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       11 2023-07-14 04:31:14.000000 hcs-cli-0.1.46/hcs_cli.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.46/mypy.ini
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.306710 hcs-cli-0.1.46/payload/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.388265 hcs-cli-0.1.46/payload/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.46/payload/lcm/zero.json
+-rw-r--r--   0 nanw       (501) staff       (20)     1187 2023-06-13 19:56:09.000000 hcs-cli-0.1.46/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      194 2023-07-05 20:09:57.000000 hcs-cli-0.1.46/requirements-dev.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      213 2023-07-05 20:09:23.000000 hcs-cli-0.1.46/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2023-07-14 04:31:15.698150 hcs-cli-0.1.46/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-07-14 04:31:10.000000 hcs-cli-0.1.46/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.390655 hcs-cli-0.1.46/tests/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.46/tests/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/tests/conftest.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3364 2023-07-05 16:02:01.000000 hcs-cli-0.1.46/tests/test_utils.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.391685 hcs-cli-0.1.46/tests/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.46/tests/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.392596 hcs-cli-0.1.46/tests/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.46/tests/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.396210 hcs-cli-0.1.46/tests/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.46/tests/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.398965 hcs-cli-0.1.46/tests/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.46/tests/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      599 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/tests/vhcs/cli/cmds/pki/get_root_ca.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.402135 hcs-cli-0.1.46/tests/vhcs/cli/cmds/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-07-05 15:13:25.000000 hcs-cli-0.1.46/tests/vhcs/cli/cmds/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     9018 2023-07-11 08:13:52.000000 hcs-cli-0.1.46/tests/vhcs/cli/cmds/plan/test_plan.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1943 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/tests/vhcs/cli/cmds/test_context.py
+-rw-r--r--   0 nanw       (501) staff       (20)      918 2023-07-03 19:18:10.000000 hcs-cli-0.1.46/tests/vhcs/cli/cmds/test_login.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1151 2023-07-05 08:29:47.000000 hcs-cli-0.1.46/tests/vhcs/cli/cmds/test_profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.407019 hcs-cli-0.1.46/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.46/vhcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      687 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/__main__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.410360 hcs-cli-0.1.46/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.46/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.414366 hcs-cli-0.1.46/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.46/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.416297 hcs-cli-0.1.46/vhcs/cli/cmds/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.417389 hcs-cli-0.1.46/vhcs/cli/cmds/admin/azure-infra/
+-rw-r--r--   0 nanw       (501) staff       (20)     1069 2023-06-27 20:44:31.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/azure-infra/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.423146 hcs-cli-0.1.46/vhcs/cli/cmds/admin/edge/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/edge/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      941 2023-07-10 08:17:03.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/edge/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      852 2023-07-06 14:26:46.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/edge/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.428624 hcs-cli-0.1.46/vhcs/cli/cmds/admin/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)     2220 2023-07-12 20:50:46.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/provider/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)      986 2023-07-07 17:12:04.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1136 2023-06-15 22:34:38.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.433681 hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      949 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1841 2023-06-23 17:01:30.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.437942 hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/vm/
+-rw-r--r--   0 nanw       (501) staff       (20)      622 2023-07-08 00:36:46.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/vm/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1018 2023-07-08 00:40:33.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/vm/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      953 2023-07-08 00:39:35.000000 hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/vm/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.439435 hcs-cli-0.1.46/vhcs/cli/cmds/auth/
+-rw-r--r--   0 nanw       (501) staff       (20)      632 2023-07-11 01:47:20.000000 hcs-cli-0.1.46/vhcs/cli/cmds/auth/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.442416 hcs-cli-0.1.46/vhcs/cli/cmds/auth/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)      642 2023-07-11 01:47:42.000000 hcs-cli-0.1.46/vhcs/cli/cmds/auth/admin/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      931 2023-07-11 01:50:03.000000 hcs-cli-0.1.46/vhcs/cli/cmds/auth/admin/get_org_idp_map.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.446258 hcs-cli-0.1.46/vhcs/cli/cmds/daas/
+-rw-r--r--   0 nanw       (501) staff       (20)      642 2023-06-15 22:15:00.000000 hcs-cli-0.1.46/vhcs/cli/cmds/daas/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.453579 hcs-cli-0.1.46/vhcs/cli/cmds/daas/infra/
+-rw-r--r--   0 nanw       (501) staff       (20)      648 2023-06-21 17:56:47.000000 hcs-cli-0.1.46/vhcs/cli/cmds/daas/infra/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1041 2023-06-30 16:52:44.000000 hcs-cli-0.1.46/vhcs/cli/cmds/daas/infra/basic.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3935 2023-07-13 00:26:26.000000 hcs-cli-0.1.46/vhcs/cli/cmds/daas/infra/plan.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.457316 hcs-cli-0.1.46/vhcs/cli/cmds/daas/tenant/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-21 17:36:22.000000 hcs-cli-0.1.46/vhcs/cli/cmds/daas/tenant/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3292 2023-07-12 23:34:52.000000 hcs-cli-0.1.46/vhcs/cli/cmds/daas/tenant/plan.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.461261 hcs-cli-0.1.46/vhcs/cli/cmds/ims/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-27 19:52:41.000000 hcs-cli-0.1.46/vhcs/cli/cmds/ims/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      915 2023-06-27 19:56:58.000000 hcs-cli-0.1.46/vhcs/cli/cmds/ims/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1033 2023-06-27 20:14:16.000000 hcs-cli-0.1.46/vhcs/cli/cmds/ims/list_copies.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.466800 hcs-cli-0.1.46/vhcs/cli/cmds/inventory/
+-rw-r--r--   0 nanw       (501) staff       (20)      637 2023-07-08 00:10:13.000000 hcs-cli-0.1.46/vhcs/cli/cmds/inventory/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1065 2023-07-08 00:42:44.000000 hcs-cli-0.1.46/vhcs/cli/cmds/inventory/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      958 2023-07-08 00:42:48.000000 hcs-cli-0.1.46/vhcs/cli/cmds/inventory/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.468362 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-27 19:52:37.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.474225 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/provider/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      801 2023-06-23 02:35:21.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      792 2023-06-23 02:35:30.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      987 2023-06-23 02:35:40.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.482054 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/
+-rw-r--r--   0 nanw       (501) staff       (20)      628 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1857 2023-06-23 02:36:50.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1079 2023-06-23 02:36:58.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      840 2023-06-23 02:37:07.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1588 2023-06-23 02:37:18.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-06-23 02:37:44.000000 hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/wait.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6922 2023-07-06 00:55:04.000000 hcs-cli-0.1.46/vhcs/cli/cmds/login.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.327338 hcs-cli-0.1.46/vhcs/cli/cmds/org/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.491886 hcs-cli-0.1.46/vhcs/cli/cmds/org/datacenter/
+-rw-r--r--   0 nanw       (501) staff       (20)      848 2023-06-30 15:40:06.000000 hcs-cli-0.1.46/vhcs/cli/cmds/org/datacenter/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      997 2023-06-30 15:40:15.000000 hcs-cli-0.1.46/vhcs/cli/cmds/org/datacenter/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.496451 hcs-cli-0.1.46/vhcs/cli/cmds/org/detail/
+-rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:40:19.000000 hcs-cli-0.1.46/vhcs/cli/cmds/org/detail/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1201 2023-06-30 15:40:25.000000 hcs-cli-0.1.46/vhcs/cli/cmds/org/detail/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.504490 hcs-cli-0.1.46/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)      631 2023-06-13 19:45:45.000000 hcs-cli-0.1.46/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-06-30 15:38:40.000000 hcs-cli-0.1.46/vhcs/cli/cmds/pki/delete_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      906 2023-06-30 15:38:40.000000 hcs-cli-0.1.46/vhcs/cli/cmds/pki/get_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      775 2023-06-30 15:38:40.000000 hcs-cli-0.1.46/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1804 2023-06-30 15:38:40.000000 hcs-cli-0.1.46/vhcs/cli/cmds/pki/sign_resource_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      726 2023-06-30 15:38:40.000000 hcs-cli-0.1.46/vhcs/cli/cmds/pki/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.510119 hcs-cli-0.1.46/vhcs/cli/cmds/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)      665 2023-06-28 17:52:44.000000 hcs-cli-0.1.46/vhcs/cli/cmds/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1777 2023-07-11 20:14:16.000000 hcs-cli-0.1.46/vhcs/cli/cmds/plan/deploy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1556 2023-07-11 20:14:11.000000 hcs-cli-0.1.46/vhcs/cli/cmds/plan/destroy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1660 2023-07-11 23:15:11.000000 hcs-cli-0.1.46/vhcs/cli/cmds/plan/graph.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.511950 hcs-cli-0.1.46/vhcs/cli/cmds/portal/
+-rw-r--r--   0 nanw       (501) staff       (20)      634 2023-07-10 08:01:20.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.519260 hcs-cli-0.1.46/vhcs/cli/cmds/portal/entitlement/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-11 03:23:55.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/entitlement/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      942 2023-07-11 20:54:29.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/entitlement/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      968 2023-07-11 03:24:19.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/entitlement/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      868 2023-07-11 03:24:49.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/entitlement/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.526642 hcs-cli-0.1.46/vhcs/cli/cmds/portal/pool/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-10 08:01:44.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/pool/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      929 2023-07-11 20:55:25.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/pool/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      954 2023-07-10 08:18:40.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/pool/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      937 2023-07-10 08:26:34.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/pool/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.534427 hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/
+-rw-r--r--   0 nanw       (501) staff       (20)      624 2023-07-11 20:43:14.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1154 2023-07-11 20:56:15.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)      928 2023-07-11 20:56:11.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      948 2023-07-11 20:56:50.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      854 2023-07-11 20:56:58.000000 hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.536976 hcs-cli-0.1.46/vhcs/cli/cmds/profile/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.46/vhcs/cli/cmds/profile/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1765 2023-07-05 06:16:00.000000 hcs-cli-0.1.46/vhcs/cli/cmds/profile/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)      932 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/cli/cmds/upgrade.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.538174 hcs-cli-0.1.46/vhcs/cli/cmds/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)      633 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/cli/cmds/vmhub/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.541959 hcs-cli-0.1.46/vhcs/cli/cmds/vmhub/otp/
+-rw-r--r--   0 nanw       (501) staff       (20)      643 2023-06-29 21:49:43.000000 hcs-cli-0.1.46/vhcs/cli/cmds/vmhub/otp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1234 2023-06-29 21:49:20.000000 hcs-cli-0.1.46/vhcs/cli/cmds/vmhub/otp/redeem.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1143 2023-06-29 21:49:25.000000 hcs-cli-0.1.46/vhcs/cli/cmds/vmhub/otp/request.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2865 2023-06-23 02:40:39.000000 hcs-cli-0.1.46/vhcs/cli/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.548259 hcs-cli-0.1.46/vhcs/common/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.46/vhcs/common/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.566068 hcs-cli-0.1.46/vhcs/common/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)     1538 2023-07-03 20:20:16.000000 hcs-cli-0.1.46/vhcs/common/ctxp/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)      790 2023-07-03 20:45:37.000000 hcs-cli-0.1.46/vhcs/common/ctxp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-07-03 21:18:13.000000 hcs-cli-0.1.46/vhcs/common/ctxp/_init.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.570866 hcs-cli-0.1.46/vhcs/common/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.46/vhcs/common/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2421 2023-06-21 17:26:56.000000 hcs-cli-0.1.46/vhcs/common/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3989 2023-07-05 23:22:13.000000 hcs-cli-0.1.46/vhcs/common/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5129 2023-07-05 06:22:51.000000 hcs-cli-0.1.46/vhcs/common/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)      936 2023-07-03 21:17:12.000000 hcs-cli-0.1.46/vhcs/common/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-03 21:08:50.000000 hcs-cli-0.1.46/vhcs/common/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6467 2023-06-23 00:26:19.000000 hcs-cli-0.1.46/vhcs/common/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/common/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3060 2023-07-11 23:13:07.000000 hcs-cli-0.1.46/vhcs/common/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5526 2023-07-11 08:29:40.000000 hcs-cli-0.1.46/vhcs/common/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-07-05 06:52:28.000000 hcs-cli-0.1.46/vhcs/common/ctxp/profile_store.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1604 2023-07-03 22:06:25.000000 hcs-cli-0.1.46/vhcs/common/ctxp/state.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6356 2023-07-11 02:38:58.000000 hcs-cli-0.1.46/vhcs/common/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3256 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/common/ctxp/var_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2259 2023-07-05 18:05:17.000000 hcs-cli-0.1.46/vhcs/common/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6329 2023-07-13 00:38:57.000000 hcs-cli-0.1.46/vhcs/common/logger.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.580641 hcs-cli-0.1.46/vhcs/common/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)      654 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/common/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4648 2023-07-07 17:06:56.000000 hcs-cli-0.1.46/vhcs/common/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8079 2023-07-05 07:42:49.000000 hcs-cli-0.1.46/vhcs/common/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5200 2023-07-10 08:10:53.000000 hcs-cli-0.1.46/vhcs/common/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      906 2023-07-07 17:01:14.000000 hcs-cli-0.1.46/vhcs/common/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8243 2023-07-05 08:11:32.000000 hcs-cli-0.1.46/vhcs/common/sglib/login_support.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1443 2023-07-06 01:06:43.000000 hcs-cli-0.1.46/vhcs/common/sglib/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     9805 2023-07-11 07:29:39.000000 hcs-cli-0.1.46/vhcs/common/util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.583133 hcs-cli-0.1.46/vhcs/config/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.46/vhcs/config/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-07-03 22:19:24.000000 hcs-cli-0.1.46/vhcs/config/hcs-deployments.yaml
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.590341 hcs-cli-0.1.46/vhcs/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)       74 2023-07-11 20:07:10.000000 hcs-cli-0.1.46/vhcs/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)    15274 2023-07-12 18:20:35.000000 hcs-cli-0.1.46/vhcs/plan/core.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6862 2023-07-13 01:02:57.000000 hcs-cli-0.1.46/vhcs/plan/dag.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5469 2023-07-11 07:19:12.000000 hcs-cli-0.1.46/vhcs/plan/helper.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.591840 hcs-cli-0.1.46/vhcs/plan/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-28 17:25:18.000000 hcs-cli-0.1.46/vhcs/plan/provider/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.602671 hcs-cli-0.1.46/vhcs/plan/provider/azure/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-30 00:51:51.000000 hcs-cli-0.1.46/vhcs/plan/provider/azure/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5381 2023-07-13 00:28:42.000000 hcs-cli-0.1.46/vhcs/plan/provider/azure/_az_facade.py
+-rw-r--r--   0 nanw       (501) staff       (20)      575 2023-06-30 00:26:03.000000 hcs-cli-0.1.46/vhcs/plan/provider/azure/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1331 2023-07-12 23:43:03.000000 hcs-cli-0.1.46/vhcs/plan/provider/azure/aad_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1879 2023-07-12 23:43:40.000000 hcs-cli-0.1.46/vhcs/plan/provider/azure/aad_user.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1205 2023-07-11 21:11:11.000000 hcs-cli-0.1.46/vhcs/plan/provider/azure/nsg.py
+-rw-r--r--   0 nanw       (501) staff       (20)      982 2023-07-11 21:13:28.000000 hcs-cli-0.1.46/vhcs/plan/provider/azure/resource_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1259 2023-07-12 00:09:22.000000 hcs-cli-0.1.46/vhcs/plan/provider/azure/subnet.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.606245 hcs-cli-0.1.46/vhcs/plan/provider/dev/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-07-05 15:12:02.000000 hcs-cli-0.1.46/vhcs/plan/provider/dev/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-07-05 15:12:02.000000 hcs-cli-0.1.46/vhcs/plan/provider/dev/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1351 2023-07-11 05:50:09.000000 hcs-cli-0.1.46/vhcs/plan/provider/dev/dummy.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.617878 hcs-cli-0.1.46/vhcs/plan/provider/hcs/
+-rw-r--r--   0 nanw       (501) staff       (20)       29 2023-06-29 23:41:13.000000 hcs-cli-0.1.46/vhcs/plan/provider/hcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-06-29 23:41:19.000000 hcs-cli-0.1.46/vhcs/plan/provider/hcs/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1042 2023-07-11 08:52:37.000000 hcs-cli-0.1.46/vhcs/plan/provider/hcs/entitlement.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1326 2023-07-11 08:39:38.000000 hcs-cli-0.1.46/vhcs/plan/provider/hcs/launch_item.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1227 2023-07-12 00:45:19.000000 hcs-cli-0.1.46/vhcs/plan/provider/hcs/pool_group.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1685 2023-07-11 01:24:50.000000 hcs-cli-0.1.46/vhcs/plan/provider/hcs/pool_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1188 2023-07-12 20:31:23.000000 hcs-cli-0.1.46/vhcs/plan/provider/hcs/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1087 2023-07-11 21:01:33.000000 hcs-cli-0.1.46/vhcs/plan/provider/hcs/site.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.620168 hcs-cli-0.1.46/vhcs/service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.46/vhcs/service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1586 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/service/_util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.628700 hcs-cli-0.1.46/vhcs/service/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)       59 2023-06-27 20:41:57.000000 hcs-cli-0.1.46/vhcs/service/admin/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-07-06 14:56:48.000000 hcs-cli-0.1.46/vhcs/service/admin/azure_infra.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1042 2023-07-10 08:03:20.000000 hcs-cli-0.1.46/vhcs/service/admin/edge.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1265 2023-06-23 01:29:22.000000 hcs-cli-0.1.46/vhcs/service/admin/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1313 2023-07-12 20:33:06.000000 hcs-cli-0.1.46/vhcs/service/admin/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2731 2023-07-10 05:17:36.000000 hcs-cli-0.1.46/vhcs/service/admin/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.631401 hcs-cli-0.1.46/vhcs/service/auth/
+-rw-r--r--   0 nanw       (501) staff       (20)       19 2023-06-22 18:49:46.000000 hcs-cli-0.1.46/vhcs/service/auth/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      851 2023-06-22 18:45:24.000000 hcs-cli-0.1.46/vhcs/service/auth/admin.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.636248 hcs-cli-0.1.46/vhcs/service/ims_catalog/
+-rw-r--r--   0 nanw       (501) staff       (20)       42 2023-06-27 19:54:19.000000 hcs-cli-0.1.46/vhcs/service/ims_catalog/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1218 2023-07-06 14:39:54.000000 hcs-cli-0.1.46/vhcs/service/ims_catalog/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)      915 2023-07-06 14:43:11.000000 hcs-cli-0.1.46/vhcs/service/ims_catalog/image_copies.py
+-rw-r--r--   0 nanw       (501) staff       (20)      909 2023-06-22 01:03:55.000000 hcs-cli-0.1.46/vhcs/service/ims_catalog/images.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.641423 hcs-cli-0.1.46/vhcs/service/inventory/
+-rw-r--r--   0 nanw       (501) staff       (20)       25 2023-07-08 00:42:34.000000 hcs-cli-0.1.46/vhcs/service/inventory/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1290 2023-07-08 00:32:38.000000 hcs-cli-0.1.46/vhcs/service/inventory/vm.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.644797 hcs-cli-0.1.46/vhcs/service/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)       32 2023-06-22 18:49:27.000000 hcs-cli-0.1.46/vhcs/service/lcm/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1437 2023-06-22 18:48:08.000000 hcs-cli-0.1.46/vhcs/service/lcm/provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2770 2023-06-22 18:47:45.000000 hcs-cli-0.1.46/vhcs/service/lcm/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.648563 hcs-cli-0.1.46/vhcs/service/org_service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:56.000000 hcs-cli-0.1.46/vhcs/service/org_service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1083 2023-06-30 15:37:59.000000 hcs-cli-0.1.46/vhcs/service/org_service/datacenter.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1040 2023-06-30 15:37:42.000000 hcs-cli-0.1.46/vhcs/service/org_service/details.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.651140 hcs-cli-0.1.46/vhcs/service/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:38:50.000000 hcs-cli-0.1.46/vhcs/service/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1211 2023-06-30 15:38:16.000000 hcs-cli-0.1.46/vhcs/service/pki/certificate.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.657052 hcs-cli-0.1.46/vhcs/service/portal/
+-rw-r--r--   0 nanw       (501) staff       (20)       37 2023-07-11 20:44:21.000000 hcs-cli-0.1.46/vhcs/service/portal/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1277 2023-07-11 08:42:42.000000 hcs-cli-0.1.46/vhcs/service/portal/entitlement.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1265 2023-07-11 20:55:47.000000 hcs-cli-0.1.46/vhcs/service/portal/pool.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1336 2023-07-11 21:02:10.000000 hcs-cli-0.1.46/vhcs/service/portal/site.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.659555 hcs-cli-0.1.46/vhcs/service/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)       17 2023-07-03 19:03:42.000000 hcs-cli-0.1.46/vhcs/service/vmhub/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1406 2023-06-29 21:48:05.000000 hcs-cli-0.1.46/vhcs/service/vmhub/otp.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.663014 hcs-cli-0.1.46/vhcs/support/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-30 15:35:24.000000 hcs-cli-0.1.46/vhcs/support/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.676442 hcs-cli-0.1.46/vhcs/support/daas/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-06-21 23:10:31.000000 hcs-cli-0.1.46/vhcs/support/daas/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1482 2023-07-13 00:23:42.000000 hcs-cli-0.1.46/vhcs/support/daas/cidr_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3580 2023-07-12 00:03:12.000000 hcs-cli-0.1.46/vhcs/support/daas/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1797 2023-07-07 17:20:02.000000 hcs-cli-0.1.46/vhcs/support/daas/infra.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1280 2023-07-12 21:56:02.000000 hcs-cli-0.1.46/vhcs/support/daas/infra_calc.py
+-rw-r--r--   0 nanw       (501) staff       (20)      424 2023-07-11 23:57:51.000000 hcs-cli-0.1.46/vhcs/support/daas/template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.349086 hcs-cli-0.1.46/vhcs/support/daas/templates/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.684412 hcs-cli-0.1.46/vhcs/support/daas/templates/v1/
+-rw-r--r--   0 nanw       (501) staff       (20)      394 2023-07-11 23:33:48.000000 hcs-cli-0.1.46/vhcs/support/daas/templates/v1/infra.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)      220 2023-07-12 23:47:56.000000 hcs-cli-0.1.46/vhcs/support/daas/templates/v1/infra.vars.yml
+-rw-r--r--   0 nanw       (501) staff       (20)     3690 2023-07-12 23:33:06.000000 hcs-cli-0.1.46/vhcs/support/daas/templates/v1/tenant.blueprint.yml
+-rw-r--r--   0 nanw       (501) staff       (20)      239 2023-07-12 23:32:53.000000 hcs-cli-0.1.46/vhcs/support/daas/templates/v1/tenant.vars.yml
+-rw-r--r--   0 nanw       (501) staff       (20)     1979 2023-06-22 21:16:18.000000 hcs-cli-0.1.46/vhcs/support/daas/tenant.py.xx
+-rw-r--r--   0 nanw       (501) staff       (20)     4088 2023-07-12 23:12:58.000000 hcs-cli-0.1.46/vhcs/support/daas/tenant_calc.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1455 2023-07-11 20:14:32.000000 hcs-cli-0.1.46/vhcs/support/plan_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2621 2023-07-05 07:42:08.000000 hcs-cli-0.1.46/vhcs/support/profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-07-14 04:31:15.695813 hcs-cli-0.1.46/vhcs/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.46/vhcs/util/__init__.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/util/check_license.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2759 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/util/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1852 2023-07-08 00:14:58.000000 hcs-cli-0.1.46/vhcs/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1725 2023-06-13 19:40:36.000000 hcs-cli-0.1.46/vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.45/.gitignore` & `hcs-cli-0.1.46/.gitignore`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/.vscode/launch.json` & `hcs-cli-0.1.46/.vscode/launch.json`

 * *Files 4% similar despite different names*

```diff
@@ -46,31 +46,41 @@
             "name": "hcs plan deploy",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": true,
             "cwd": "${workspaceFolder}/lab",
-            "args" : ["plan", "deploy", "-f", "nanw.plan.yml"]
+            "args" : ["plan", "deploy", "-f", "nanw.plan.yml", "--sequential"]
         },
         {
             "name": "hcs destroy",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": true,
             "cwd": "${workspaceFolder}/lab",
             "args" : ["plan", "destroy", "-f", "nanw.plan.yml"]
         },
         {
-            "name": "hcs admin template list",
+            "name": "plan deploy t",
             "type": "python",
             "request": "launch",
             "program": "/usr/local/bin/hcs",
             "console": "integratedTerminal",
             "justMyCode": false,
             "cwd": "${workspaceFolder}/lab",
-            "args" : ["admin", "template", "list"]
+            "args" : ["plan", "deploy", "-f", "t.plan.yml"]
+        },
+        {
+            "name": "plan destroy t",
+            "type": "python",
+            "request": "launch",
+            "program": "/usr/local/bin/hcs",
+            "console": "integratedTerminal",
+            "justMyCode": false,
+            "cwd": "${workspaceFolder}/lab",
+            "args" : ["plan", "destroy", "-f", "t.plan.yml"]
         },
     ]
 }
```

### Comparing `hcs-cli-0.1.45/CODE_OF_CONDUCT.md` & `hcs-cli-0.1.46/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/CONTRIBUTING_CLA.md` & `hcs-cli-0.1.46/CONTRIBUTING_CLA.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/GOVERNANCE.md` & `hcs-cli-0.1.46/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/LICENSE` & `hcs-cli-0.1.46/LICENSE`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/Makefile` & `hcs-cli-0.1.46/Makefile`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/PKG-INFO` & `hcs-cli-0.1.46/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.45
+Version: 0.1.46
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs-cli-0.1.45/README.md` & `hcs-cli-0.1.46/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/doc/az-cheatsheet.md` & `hcs-cli-0.1.46/doc/az-cheatsheet.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/doc/dev-setup.md` & `hcs-cli-0.1.46/doc/dev-setup.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/doc/get-csp-user-api-token.md` & `hcs-cli-0.1.46/doc/get-csp-user-api-token.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/doc/hcs-cli-cheatsheet.md` & `hcs-cli-0.1.46/doc/hcs-cli-cheatsheet.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/doc/hcs-plan.md` & `hcs-cli-0.1.46/doc/hcs-plan.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/hcs_cli.egg-info/PKG-INFO` & `hcs-cli-0.1.46/hcs_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.45
+Version: 0.1.46
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs-cli-0.1.45/hcs_cli.egg-info/SOURCES.txt` & `hcs-cli-0.1.46/hcs_cli.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 vhcs/cli/cmds/login.py
 vhcs/cli/cmds/upgrade.py
 vhcs/cli/cmds/admin/__init__.py
 vhcs/cli/cmds/admin/azure-infra/main.py
 vhcs/cli/cmds/admin/edge/__init__.py
 vhcs/cli/cmds/admin/edge/get.py
 vhcs/cli/cmds/admin/edge/list.py
+vhcs/cli/cmds/admin/provider/create.py
 vhcs/cli/cmds/admin/provider/get.py
 vhcs/cli/cmds/admin/provider/list.py
 vhcs/cli/cmds/admin/template/__init__.py
 vhcs/cli/cmds/admin/template/get.py
 vhcs/cli/cmds/admin/template/list.py
 vhcs/cli/cmds/admin/template/vm/__init__.py
 vhcs/cli/cmds/admin/template/vm/get.py
@@ -167,14 +168,15 @@
 vhcs/plan/provider/dev/dummy.py
 vhcs/plan/provider/hcs/__init__.py
 vhcs/plan/provider/hcs/_prepare.py
 vhcs/plan/provider/hcs/entitlement.py
 vhcs/plan/provider/hcs/launch_item.py
 vhcs/plan/provider/hcs/pool_group.py
 vhcs/plan/provider/hcs/pool_template.py
+vhcs/plan/provider/hcs/provider.py
 vhcs/plan/provider/hcs/site.py
 vhcs/service/__init__.py
 vhcs/service/_util.py
 vhcs/service/admin/__init__.py
 vhcs/service/admin/azure_infra.py
 vhcs/service/admin/edge.py
 vhcs/service/admin/helper.py
@@ -202,14 +204,15 @@
 vhcs/service/portal/site.py
 vhcs/service/vmhub/__init__.py
 vhcs/service/vmhub/otp.py
 vhcs/support/__init__.py
 vhcs/support/plan_util.py
 vhcs/support/profile.py
 vhcs/support/daas/__init__.py
+vhcs/support/daas/cidr_util.py
 vhcs/support/daas/helper.py
 vhcs/support/daas/infra.py
 vhcs/support/daas/infra_calc.py
 vhcs/support/daas/template.py
 vhcs/support/daas/tenant.py.xx
 vhcs/support/daas/tenant_calc.py
 vhcs/support/daas/templates/v1/infra.blueprint.yml
```

### Comparing `hcs-cli-0.1.45/payload/lcm/zero.json` & `hcs-cli-0.1.46/payload/lcm/zero.json`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/pyproject.toml` & `hcs-cli-0.1.46/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/setup.py` & `hcs-cli-0.1.46/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from setuptools_scm import get_version
 import os
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
-VERSION = "0.1.45"
+VERSION = "0.1.46"
 
 
 def get_version():
     version = VERSION
     local_version = os.environ.get("SCM_REV")
     if local_version:
         version += "+" + local_version
```

### Comparing `hcs-cli-0.1.45/tests/conftest.py` & `hcs-cli-0.1.46/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/tests/test_utils.py` & `hcs-cli-0.1.46/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/tests/vhcs/cli/cmds/pki/get_root_ca.py` & `hcs-cli-0.1.46/tests/vhcs/cli/cmds/pki/get_root_ca.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/tests/vhcs/cli/cmds/plan/test_plan.py` & `hcs-cli-0.1.46/tests/vhcs/cli/cmds/plan/test_plan.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/tests/vhcs/cli/cmds/test_context.py` & `hcs-cli-0.1.46/tests/vhcs/cli/cmds/test_context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/tests/vhcs/cli/cmds/test_login.py` & `hcs-cli-0.1.46/tests/vhcs/cli/cmds/test_login.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/tests/vhcs/cli/cmds/test_profile.py` & `hcs-cli-0.1.46/tests/vhcs/cli/cmds/test_profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/__main__.py` & `hcs-cli-0.1.46/vhcs/__main__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/admin/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/admin/azure-infra/main.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/admin/azure-infra/main.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/admin/edge/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/admin/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/admin/edge/get.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/admin/edge/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/admin/edge/list.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/admin/edge/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/admin/provider/get.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/admin/provider/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/admin/provider/list.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/admin/provider/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/get.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/list.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/vm/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/vm/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/vm/get.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/vm/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/admin/template/vm/list.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/admin/template/vm/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/auth/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/auth/admin/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/auth/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/auth/admin/get_org_idp_map.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/auth/admin/get_org_idp_map.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/daas/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/daas/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/daas/infra/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/daas/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/daas/infra/basic.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/daas/infra/basic.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/daas/tenant/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/daas/tenant/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/ims/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/ims/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/ims/list.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/ims/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/ims/list_copies.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/ims/list_copies.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/inventory/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/inventory/get.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/inventory/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/inventory/list.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/inventory/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/provider/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/provider/delete.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/provider/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/provider/get.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/provider/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/provider/list.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/provider/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/create.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/create.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/delete.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/get.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/list.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/lcm/template/wait.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/lcm/template/wait.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/login.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/login.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/org/datacenter/get.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/org/datacenter/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/org/datacenter/list.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/org/datacenter/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/org/detail/get.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/org/detail/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/org/detail/list.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/org/detail/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/pki/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/pki/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/pki/delete_org_cert.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/pki/delete_org_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/pki/get_org_cert.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/pki/get_org_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/pki/get_root_ca.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/pki/get_root_ca.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/pki/sign_resource_cert.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/pki/sign_resource_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/pki/test.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/pki/test.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/plan/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/plan/deploy.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/plan/deploy.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/plan/destroy.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/plan/destroy.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/plan/graph.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/plan/graph.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/portal/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/portal/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/portal/entitlement/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/portal/entitlement/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/portal/entitlement/delete.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/portal/entitlement/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/portal/entitlement/get.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/portal/entitlement/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/portal/entitlement/list.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/portal/entitlement/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/portal/pool/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/portal/pool/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/portal/pool/delete.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/portal/pool/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/portal/pool/get.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/portal/pool/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/portal/pool/list.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/portal/pool/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/portal/site/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/portal/site/create.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/create.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/portal/site/delete.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/delete.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/portal/site/get.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/get.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/portal/site/list.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/portal/site/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/profile/init.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/profile/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/upgrade.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/upgrade.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/vmhub/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/vmhub/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/vmhub/otp/__init__.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/vmhub/otp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/vmhub/otp/redeem.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/vmhub/otp/redeem.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/cmds/vmhub/otp/request.py` & `hcs-cli-0.1.46/vhcs/cli/cmds/vmhub/otp/request.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/cli/main.py` & `hcs-cli-0.1.46/vhcs/cli/main.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/ctxp/README.md` & `hcs-cli-0.1.46/vhcs/common/ctxp/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/ctxp/__init__.py` & `hcs-cli-0.1.46/vhcs/common/ctxp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/ctxp/_init.py` & `hcs-cli-0.1.46/vhcs/common/ctxp/_init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/ctxp/built_in_cmds/context.py` & `hcs-cli-0.1.46/vhcs/common/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/ctxp/built_in_cmds/profile.py` & `hcs-cli-0.1.46/vhcs/common/ctxp/built_in_cmds/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/ctxp/cli_processor.py` & `hcs-cli-0.1.46/vhcs/common/ctxp/cli_processor.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/ctxp/config.py` & `hcs-cli-0.1.46/vhcs/common/ctxp/config.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/ctxp/context.py` & `hcs-cli-0.1.46/vhcs/common/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/ctxp/fstore.py` & `hcs-cli-0.1.46/vhcs/common/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/ctxp/init.py` & `hcs-cli-0.1.46/vhcs/common/ctxp/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/ctxp/jsondot.py` & `hcs-cli-0.1.46/vhcs/common/ctxp/jsondot.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/ctxp/profile.py` & `hcs-cli-0.1.46/vhcs/common/ctxp/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/ctxp/profile_store.py` & `hcs-cli-0.1.46/vhcs/common/ctxp/profile_store.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/ctxp/state.py` & `hcs-cli-0.1.46/vhcs/common/ctxp/state.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/ctxp/util.py` & `hcs-cli-0.1.46/vhcs/common/ctxp/util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/ctxp/var_template.py` & `hcs-cli-0.1.46/vhcs/common/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/duration.py` & `hcs-cli-0.1.46/vhcs/common/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/logger.py` & `hcs-cli-0.1.46/vhcs/common/logger.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,26 +9,25 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-import sys
 import os
 import re
 import logging
 import coloredlogs
 from logging.handlers import RotatingFileHandler
 
-LOG_FORMAT_SIMPLE = "%(levelname)-7s %(asctime)s %(name)s %(message)s"
+LOG_FORMAT_SIMPLE = "%(levelname)-4s %(asctime)s %(name)-16s %(message)s"
 LOG_FORMAT_LONG = (
     "%(color_on)s%(asctime)s [%(process)-5d:%(threadName)-12s] %(levelname)-7s [%(name)-16s] %(message)s%(color_off)s"
 )
-
+DATE_FORMAT_SIMPLE = "%H:%M:%S"
 
 def mask_password(msg: str) -> str:
     msg = re.sub(r"(\"password\"\s*:\s*\"?)(.*?)(\"?[\s*,? | \s*\}])", r"\1******\3", msg)
     return msg
 
 
 class LogFormatter(logging.Formatter):
@@ -50,41 +49,79 @@
     def format(self, record, *args, **kwargs):
         if self.color == True and record.levelno in self.COLOR_CODES:
             record.color_on = self.COLOR_CODES[record.levelno]
             record.color_off = self.RESET_CODE
         else:
             record.color_on = ""
             record.color_off = ""
+
+        record.name = _shorten_package_name(record.name, 16)
+    
         msg = super(LogFormatter, self).format(record, *args, **kwargs)
         return mask_password(msg) if self.mask else msg
 
+class LogFormatterFixedNameWidth(logging.Formatter):
+
+    def __init__(self, *args, **kwargs):
+        super(LogFormatter, self).__init__(*args, **kwargs)
+
+    def format(self, record, *args, **kwargs):
+        record.name = _shorten_package_name(record.name, 16)
+        return super(LogFormatterFixedNameWidth, self).format(record, *args, **kwargs)
+    
+def _shorten_package_name(package_name, max_length):
+    if len(package_name) <= max_length:
+        return package_name
+
+    parts = package_name.split('.')
+    shortened_parts = []
+
+    for i, part in enumerate(parts):
+        shortened_parts.append(part[0])
+
+        if i == len(parts) - 1:
+            # Last package name
+            remaining_length = max_length - len('.'.join(shortened_parts))
+            if len(part) > remaining_length:
+                shortened_parts[-1] = '...' + part[-remaining_length + 3:]
+            else:
+                shortened_parts[-1] = part
+        else:
+            new_package_name = '.'.join(shortened_parts)
+
+            if len(new_package_name) + len(parts) - i - 1 > max_length:
+                break
+
+    return '.'.join(shortened_parts)
 
 def setup(
     console_log_output="stdout",
     console_log_level="INFO",
     console_log_color=True,
     console_log_mask=True,
     logfile_file=None,
     logfile_log_level="INFO",
     logfile_log_color=False,
     logfile_log_mask=True,
     log_line_template=LOG_FORMAT_SIMPLE,
+    date_fmt=DATE_FORMAT_SIMPLE
 ):
     # Alternative: 'global logger; logger = logging.getLogger("<name>")'
     logger = logging.getLogger()
     logger.setLevel(logging.INFO)
 
     if console_log_output is not None:
         setup_console_output(
             logger,
             console_log_output,
             console_log_level,
             console_log_color,
             console_log_mask,
             log_line_template,
+            date_fmt
         )
 
     if logfile_file:
         setup_file_output(
             logger,
             logfile_file,
             logfile_log_level,
@@ -97,16 +134,19 @@
 def setup_console_output(
     logger,
     console_log_output,
     console_log_level,
     console_log_color,
     console_log_mask,
     log_line_template,
+    date_fmt
 ):
-    coloredlogs.install(level=console_log_level, fmt=log_line_template)
+    if not date_fmt:
+        date_fmt = coloredlogs.DEFAULT_DATE_FORMAT
+    coloredlogs.install(level=console_log_level, fmt=log_line_template, datefmt=date_fmt, formatter=LogFormatter(fmt=log_line_template, color=console_log_color, mask=console_log_mask))
 
     # console_log_output = console_log_output.lower()
     # if console_log_output == "stdout":
     #     console_log_output = sys.stdout
     # elif console_log_output == "stderr":
     #     console_log_output = sys.stderr
     # else:
```

### Comparing `hcs-cli-0.1.45/vhcs/common/sglib/__init__.py` & `hcs-cli-0.1.46/vhcs/common/sglib/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/sglib/auth.py` & `hcs-cli-0.1.46/vhcs/common/sglib/auth.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/sglib/csp.py` & `hcs-cli-0.1.46/vhcs/common/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/sglib/ez_client.py` & `hcs-cli-0.1.46/vhcs/common/sglib/ez_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/sglib/hcs_client.py` & `hcs-cli-0.1.46/vhcs/common/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/sglib/login_support.py` & `hcs-cli-0.1.46/vhcs/common/sglib/login_support.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/sglib/util.py` & `hcs-cli-0.1.46/vhcs/common/sglib/util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/common/util.py` & `hcs-cli-0.1.46/vhcs/common/util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/config/hcs-deployments.yaml` & `hcs-cli-0.1.46/vhcs/config/hcs-deployments.yaml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/plan/core.py` & `hcs-cli-0.1.46/vhcs/plan/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,43 +42,43 @@
     state_file = deployment_id + '.state.yml'
     prev = _load_state(state_file)
     state = {'pending': pending}
     state.update(blueprint)
     state.update(prev)
 
     # try solving more variables
-    for k, v in state['output'].items():
-        if not v:
-            continue
-        if not _has_successful_deployment(state, k):
-            continue
-        _resolve_pending_keys(state, k)
+    # for k, v in state['output'].items():
+    #     if not v:
+    #         continue
+    #     if not _has_successful_deployment(state, k):
+    #         continue
+    #     _resolve_pending_keys(state, k)
     
     return blueprint, state, state_file
 
-def _has_successful_deployment(state, name):
-    for v in state['log']['deploy']:
-        if v['name'] != name:
-            continue
-        if v['action'] == 'success':
-            return True
+# def _has_successful_deployment(state, name):
+#     for v in state['log']['deploy']:
+#         if v['name'] != name:
+#             continue
+#         if v['action'] == 'success':
+#             return True
         
 def deploy(data: dict, additional_context: dict = None, resource_name: str = None, concurrency: int = 4):
     
     blueprint, state, state_file = _prepare_data(data, additional_context)
     state['log']['deploy'] = []    # clear deploy log
 
-    def process_resource(name: str, res_data: dict):
-        if name == 'defaults':
-            return
-        if res_data.get('type'):    #provider
+    def process_resource(name: str):
+        # ignore functional nodes (defaults, providers)
+        if name not in blueprint['resources']:
             return
+        res_data = blueprint['resources'][name]
         
         _deploy_res(name, res_data, state)
-        _resolve_pending_keys(state, name)
+        #_resolve_pending_keys(state, name)
         util.save_data_file(state, state_file)
         if resource_name and name == resource_name:
             return False
 
     try:
         dag.process_blueprint(blueprint, process_resource, concurrency)
     except CalledProcessError as e:
@@ -127,26 +127,49 @@
 def _get_value_by_path(state, var_name, required_by_attr_path):
     i = var_name.find('.')
     if i < 0:
         resource_name = var_name
     else:
         resource_name = var_name[:i]
 
+    def _raise(e):
+        msg = f"Plugin error: '{var_name}' does not exist in the output of resource '{resource_name}', which is required by '{required_by_attr_path}'"
+        raise PlanException(msg) from e
+    
     if resource_name in state['resources']:
         try:
             return util.deep_get_attr(state, "output." + var_name)
-        except:
-            raise PlanException(f"Plugin error: '{var_name}' does not exist in the output of resource '{resource_name}', which is required by '{required_by_attr_path}'")
-
+        except Exception as e:
+            _raise(e)
     if resource_name in state:
         try:
             return util.deep_get_attr(state, var_name)
-        except:
-            raise PlanException(f"Plugin error: '{var_name}' does not exist in the output of resource '{resource_name}', which is required by '{required_by_attr_path}'")
+        except Exception as e:
+            _raise(e)
+
+def _get_value_by_path2(state, var_name):
+    i = var_name.find('.')
+    if i < 0:
+        resource_name = var_name
+    else:
+        resource_name = var_name[:i]
 
+    if resource_name in state['resources']:
+        try:
+            return util.deep_get_attr(state, "output." + var_name), True
+        except Exception as e:
+            log.debug(e)
+            return None, False
+        
+    if resource_name in state:
+        try:
+            return util.deep_get_attr(state, var_name), True
+        except Exception as e:
+            log.debug(e)
+            return None, False
 
 def _deploy_res(name, res, state):
     def add_log(action: str, details: str = None):
         _add_log(state, 'deploy', res['kind'], name, action, details)
 
     def fn_deploy1(handler, res_data, res_state, fn_set_state):
         if res_state and not _is_runtime(res):
@@ -186,29 +209,42 @@
 #         i = int(match.group(1))
 #         name = state['resources'][i]['name']
 #         n = attr_path.index(']')
 #         readable_path = 'resources.' + name + attr_path[n + 1:]
 #         return readable_path
 #     return attr_path
 
-def _resolve_pending_keys(state, resource_name):
-    prefix = resource_name + "."
-    for attr_path, var_name in state['pending'].items():
-        if not var_name.startswith(prefix) and var_name != resource_name:
-            continue
-        # found a key to solve
+# def _resolve_pending_keys(state, resource_name):
+#     prefix = resource_name + "."
+#     for attr_path, var_name in state['pending'].items():
+#         if not var_name.startswith(prefix) and var_name != resource_name:
+#             continue
+#         # found a key to solve
         
-        # update that key
-        expr = util.deep_get_attr(state, attr_path)
-        def _get_value(path):
-            return _get_value_by_path(state, path, attr_path), True
-        resolved_value, _pending_var = util.resolve_expression(expr, _get_value)
-
-        log.debug('Resolved. %s: %s -> %s', attr_path, var_name, resolved_value)
-        util.deep_set_attr(state, attr_path, resolved_value)
+#         # update that key
+#         expr = util.deep_get_attr(state, attr_path)
+#         def _get_value(path):
+#             return _get_value_by_path(state, path, attr_path), True
+#         resolved_value, _pending_var = util.resolve_expression(expr, _get_value)
+
+#         log.debug('Resolved. %s: %s -> %s', attr_path, var_name, resolved_value)
+#         util.deep_set_attr(state, attr_path, resolved_value)
+
+def _resolve_vars(data, state, resource_name, raise_on_unresolvable):
+    data = deepcopy(data)
+    def _get_value(path):
+        return _get_value_by_path2(state, path)
+    ret = util.process_variables(data, _get_value)
+    if raise_on_unresolvable:
+        if ret['pending']:
+            msg = f"Fail resolving variables for resource '{resource_name}'. Unresolvable variables: {ret['pending']}"
+            raise PlanException(msg)
+    
+    state['resources'][resource_name]['data'] = data
+    return data
 
 def _assert_all_vars_resolved(data, name):
     def fn_on_value(path, value):
         if isinstance(value, str) and value.find('${') >= 0:
             raise PlanException(f"Unresolved variable '{path}' for plugin '{name}'. Value={value}")
         return value
     util.deep_update_object_value(data, fn_on_value)
@@ -242,16 +278,15 @@
     return set(iter1).intersection(set(iter2))
 
 def _handle_resource(name, res, state, vars_must_resolve: bool, add_log: typing.Callable, fn_process: typing.Callable):
     try:
         kind = res['kind']
         data = res.get('data', {})
         if data:
-            if vars_must_resolve:
-                _assert_all_vars_resolved(data, name)
+            data = _resolve_vars(data, state, name, vars_must_resolve)
 
         handler = _get_resource_handler(kind, state)
         def _handle_resource_1(resource_data, resource_state, fn_set_state):
             if _is_runtime(res):   # runtime has no refresh
                 pass
             else:
                 new_state = handler.refresh(resource_data, resource_state)
@@ -311,31 +346,31 @@
     entry = {
         'name': name,
         'time': time.time(),
         'action': action
     }
     if details:
         if isinstance(details, Exception):
-            if isinstance(details, PlanException):
+            if isinstance(details, PlanException) or isinstance(details, CalledProcessError):
                 pass
             else:
                 e = details
                 traceback.print_exception(type(e), e, e.__traceback__)
             details = details.__class__.__name__ + ': ' + str(details)
         else:
             details = str(details)
         entry['details'] = details
     state['log'][mode].append(entry)
     if action == 'error':
         log.warning('Plugin "%s:%s" failed: %s', kind, name, details)
 
 
-def _destroy_res(name, res, state, force):
+def _destroy_res(name, res_node, state, force):
     def add_log(action: str, details: str = None):
-        _add_log(state, 'destroy', res['kind'], name, action, details)
+        _add_log(state, 'destroy', res_node['kind'], name, action, details)
 
     def fn_destroy1(handler, res_data, res_state, fn_set_state):
         if not res_state:
             add_log('skipped', 'Not found')
             return
         
         add_log('start')
@@ -348,37 +383,34 @@
             if force:
                 add_log('error', e)
                 pass
             else:
                 # add_log('error', e) will be handled by framework.
                 raise
 
-    _handle_resource(name, res, state, False, add_log, fn_destroy1)
+    _handle_resource(name, res_node, state, False, add_log, fn_destroy1)
 
 def destroy(data, force: bool, resource_name: str = None, concurrency: int = 4, additional_context: dict = None):
     
     blueprint, state, state_file = _prepare_data(data, additional_context)
     state['log']['destroy'] = []    # clear destroy log
 
-    def destroy_resource(node_name, node):
-        # skip provider
-        if 'type' in node:  
-            return
-        kind = node.get('kind')
-        # skip non-resources, e.g. 'defaults'
-        if not kind:
+    def destroy_resource(node_name):
+        # ignore functional nodes (defaults, providers)
+        node = blueprint['resources'].get(node_name)
+        if not node:
             return
         # skip runtime
-        if kind.startswith('runtime/'):
+        if node['kind'].startswith('runtime/'):
             return
         
-        res = state['resources'].get(node_name)
-        if not res:
-            res = blueprint['resources'][node_name]
-        _destroy_res(node_name, res, state, force)
+        res_node = state['resources'].get(node_name)
+        if not res_node:
+            res_node = blueprint['resources'][node_name]
+        _destroy_res(node_name, res_node, state, force)
         util.save_data_file(state, state_file)
         if resource_name and resource_name == node_name:
             return True
 
     try:
         dag.reverse_traverse(blueprint, destroy_resource)
     except CalledProcessError as e:
```

### Comparing `hcs-cli-0.1.45/vhcs/plan/dag.py` & `hcs-cli-0.1.46/vhcs/plan/dag.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     dag.validate()
 
     topological_sorter = TopologicalSorter(dag.graph)
     sequence = list(topological_sorter.static_order())
     sequence.reverse()
 
     for node_name in sequence:
-        stop = fn_process_node(node_name, dag.data[node_name])
+        stop = fn_process_node(node_name)
         if stop == True:
             break
 
 def _build_graph(blueprint):
     dag = DAG()
 
     def add_node(name, obj):
@@ -109,15 +109,15 @@
         'err': None,
         'stop': False
     }
 
     def process_node(node_id):
         err = None
         try:
-            ret = fn_process_node(node_id, dag.data[node_id])
+            ret = fn_process_node(node_id)
             if ret == False:
                 flags['stop'] = True
         except Exception as e:
             err = e
 
         with lock:
             if err:
@@ -170,27 +170,33 @@
         }
         resource = {
         }
         vars = {
             'shape': 'note'
         }
 
+    def _is_deployed(node_name):
+        data = state['output'].get(node_name)
+        if isinstance(data, list):
+            return any(d for d in data)
+        return data
+
     def _get_node_style(node_name):
         n = dag.data[node_name]
         attr = {}
         if 'type' in n:
             attr |= styles.provider
         elif node_name in blueprint['resources']:
             if n['kind'].startswith('runtime/'):
                 attr |= styles.runtime
             else:
                 attr |= styles.resource
         elif node_name in state:
             attr |= styles.vars
-        if state['output'].get(node):
+        if _is_deployed(node_name):
             attr |= styles.deployed
         return attr
         
     
     for node in sorted_nodes:
         attrs = _get_node_style(node)
         graph.node(node, **attrs)
```

### Comparing `hcs-cli-0.1.45/vhcs/plan/helper.py` & `hcs-cli-0.1.46/vhcs/plan/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/plan/provider/azure/_az_facade.py` & `hcs-cli-0.1.46/vhcs/plan/provider/azure/_az_facade.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,28 +15,33 @@
 
 import subprocess
 import json
 import logging
 
 log = logging.getLogger(__name__)
 
-def _az(command: str, check=True) -> dict:
+def _az(command: str, silent: bool =False) -> dict:
     log.debug(command)
     args = command.split(' ')
-    try:
-        completed_process = subprocess.run(args, stdout=subprocess.PIPE, timeout=None, check=check)
-        output = completed_process.stdout
-        if output and completed_process.returncode == 0:
+    p = subprocess.run(args, capture_output=True, text=True, timeout=None, check=False)
+    if p.returncode:
+        if silent:
+            pass
+        else:
+            log.error("RETURN: " + str(p.returncode))
+            log.error("STDOUT: " + p.stdout)
+            log.error("STDERR: " + p.stderr)
+            raise subprocess.CalledProcessError(p.returncode, p.args, output=p.stdout, stderr=p.stderr)
+    else:
+        if p.stdout:
             try:
-                return json.loads(output)
+                return json.loads(p.stdout)
             except Exception as e:
                 log.error("Fail parsing response %s", e)
-                log.warning("Payload: %s", output)
-    except subprocess.CalledProcessError as e:
-        raise
+                log.warning("Payload: %s", p.stdout)
 
 def login(username: str, password: str, tenant_id: str):
     return _az(f"az login --service-principal -u {username} -p {password} --tenant {tenant_id}")
 
 def _formalize_tags(tags: dict) -> str:
     list_tags = []
     if tags:
@@ -57,46 +62,55 @@
     def delete(name: str):
         exists = _az(f"az group exists --name {name}")
         if exists:
             _az(f"az group delete --name {name} --yes")
             return True
         return False
 
+class _aad_group_member:
+
+    @staticmethod
+    def list(id_or_display_name: str):
+        return _az(f"az ad group member list --group {id_or_display_name}")
+
+    @staticmethod
+    def add(id_or_display_name: str, member_id: str):
+        return _az(f"az ad group member add --group {id_or_display_name} --member-id {member_id}")
+    
 class _aad_group:
+    member = _aad_group_member
+
     @staticmethod
     def create(display_name: str, mail_nickname: str, description: str = None):
         cmd = f"az ad group create --display-name {display_name} --mail-nickname {mail_nickname}"
         if description:
             cmd += f" --description {description}"
         return _az(cmd)
 
     @staticmethod
     def get(id_or_display_name: str):
-        return _az(f"az ad group show --group {id_or_display_name}", check=False)
+        return _az(f"az ad group show --group {id_or_display_name}", silent=True)
 
     @staticmethod
     def delete(id_or_display_name: str):
         return _az(f"az ad group delete --group {id_or_display_name}")
 
     @staticmethod
-    def list_members():
-        pass
-
-    @staticmethod
-    def add_member(id_or_display_name: str, member_id: str):
-        return _az(f"az ad group member add --group {id_or_display_name} --member-id {member_id}")
+    def list():
+        return _az(f"az ad group list")
+    
 
 class _aad_user:
     @staticmethod
     def create(display_name: str, password: str, principal_name: str):
         return _az(f"az ad user create --display-name {display_name} --password {password} --user-principal-name {principal_name}")
     
     @staticmethod
     def get(id_or_principal_name: str):
-        return _az(f"az ad user show --id {id_or_principal_name}", check=False)
+        return _az(f"az ad user show --id {id_or_principal_name}", silent=True)
 
     @staticmethod
     def delete(id: str):
         return _az(f"az ad user delete --id {id}")
 
 
 class aad:
@@ -136,12 +150,16 @@
     @staticmethod
     def delete_by_id(id: str):
         return _az(f"az network vnet subnet delete --ids {id}")
     
     @staticmethod
     def delete(rg_name: str, vnet_name: str, name: str):
         return _az(f"az network vnet subnet delete -g {rg_name} --vnet-name {vnet_name} -n {name}")
+    
+    @staticmethod
+    def list(rg_name: str, vnet_name: str):
+        return _az(f"az network vnet subnet list -g {rg_name} --vnet-name {vnet_name}")
 
 class network:
     vnet = _vnet
     nsg = _nsg
     subnet = _subnet
```

### Comparing `hcs-cli-0.1.45/vhcs/plan/provider/azure/_prepare.py` & `hcs-cli-0.1.46/vhcs/plan/provider/azure/_prepare.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/plan/provider/azure/aad_group.py` & `hcs-cli-0.1.46/vhcs/plan/provider/azure/aad_group.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 
 from . import _az_facade as az
 
 def deploy(data: dict) -> dict:
     display_name = data['displayName']
     mail_nickname = data['mailNickname']
     description = data.get('description')
-    return az.aad.group.create(display_name, mail_nickname, description)
+    parent_group = data.get('parentGroup')
+    ret = az.aad.group.create(display_name, mail_nickname, description)
+    if parent_group:
+        az.aad.group.member.add(parent_group, ret['id'])
+    return ret
 
 
 def refresh(data: dict, state: dict) -> dict:
     display_name = data['displayName']
     return az.aad.group.get(display_name)
 
 def destroy(data: dict, state: dict) -> dict:
```

### Comparing `hcs-cli-0.1.45/vhcs/plan/provider/azure/aad_user.py` & `hcs-cli-0.1.46/vhcs/plan/provider/azure/aad_user.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,43 +9,49 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+import random
 from . import _az_facade as az
 
 def deploy(data: dict) -> dict:
     group = data['group']
     email = data['email']
     domain_name = data['domainName']
 
     pname = _convert_email_to_principle(email, domain_name)
     display_name = pname
     password = _generate_password()
     principal_name = pname
     ret = az.aad.user.create(display_name, password, principal_name)
-    az.aad.group.add_member(group, ret['id'])
+    az.aad.group.member.add(group, ret['id'])
+    ret['password'] = password
     return ret
 
 def _convert_email_to_principle(email: str, domain_name: str) -> str:
     name = email.replace('@', '-').replace('.', '-')
     return name + '@' + domain_name
 
 def _generate_password() -> str:
-    return 'Hellomortal1!'
+    ret = random.choices("ABCDEFGHJKMNPQRSTUVWXY")
+    ret += random.choices("abcdefghjkmnpqrstuvwxy23456789", k=10)
+    ret += random.choices("!@$%&*")
+    return "".join(ret)
 
 def refresh(data: dict, state: dict) -> dict:
     if state:
         id = state['id']
         ret = az.aad.user.get(id)
         if ret:
             return ret
     email = data['email']
     domain_name = data['domainName']
     pname = _convert_email_to_principle(email, domain_name)
     return az.aad.user.get(pname)
 
 def destroy(data: dict, state: dict) -> dict:
     id = state['id']
-    ret = az.aad.user.delete(id)
+    ret = az.aad.user.delete(id)
+    return ret
```

### Comparing `hcs-cli-0.1.45/vhcs/plan/provider/azure/nsg.py` & `hcs-cli-0.1.46/vhcs/plan/provider/azure/nsg.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/plan/provider/azure/resource_group.py` & `hcs-cli-0.1.46/vhcs/plan/provider/azure/resource_group.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/plan/provider/azure/subnet.py` & `hcs-cli-0.1.46/vhcs/plan/provider/azure/subnet.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/plan/provider/dev/dummy.py` & `hcs-cli-0.1.46/vhcs/plan/provider/dev/dummy.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/plan/provider/hcs/entitlement.py` & `hcs-cli-0.1.46/vhcs/plan/provider/hcs/entitlement.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/plan/provider/hcs/launch_item.py` & `hcs-cli-0.1.46/vhcs/plan/provider/hcs/launch_item.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/plan/provider/hcs/pool_group.py` & `hcs-cli-0.1.46/vhcs/plan/provider/hcs/pool_group.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/plan/provider/hcs/pool_template.py` & `hcs-cli-0.1.46/vhcs/plan/provider/hcs/pool_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/plan/provider/hcs/site.py` & `hcs-cli-0.1.46/vhcs/plan/provider/hcs/site.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/service/_util.py` & `hcs-cli-0.1.46/vhcs/service/_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/service/admin/azure_infra.py` & `hcs-cli-0.1.46/vhcs/service/admin/azure_infra.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/service/admin/edge.py` & `hcs-cli-0.1.46/vhcs/service/admin/edge.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/service/admin/helper.py` & `hcs-cli-0.1.46/vhcs/service/admin/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/service/admin/provider.py` & `hcs-cli-0.1.46/vhcs/service/org_service/details.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from .._util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
-_client = hdc_service_client("admin")
+_client = hdc_service_client("org-service")
 
-def list(label: str, **kwargs):
+
+def get(id: str, **kwargs):
+    url = with_query(f"/v1/org-details/{id}", **kwargs)
+    return _client.get(url)
+
+def list(**kwargs):
     def _get_page(query_string):
-        url = f"/v2/providers/{label}/instances?{query_string}"
+        url = "/v1/org-details?" + query_string
         return _client.get(url)
 
     return PageRequest(_get_page, **kwargs).get()
-
-def get(label: str, id: str, **kwargs):
-    url = f"/v2/providers/{label}/instances/{id}"
-    url = with_query(url, **kwargs)
-    return _client.get(url)
```

### Comparing `hcs-cli-0.1.45/vhcs/service/admin/template.py` & `hcs-cli-0.1.46/vhcs/service/admin/template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/service/auth/admin.py` & `hcs-cli-0.1.46/vhcs/service/auth/admin.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/service/ims_catalog/helper.py` & `hcs-cli-0.1.46/vhcs/service/ims_catalog/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/service/ims_catalog/image_copies.py` & `hcs-cli-0.1.46/vhcs/service/ims_catalog/image_copies.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/service/ims_catalog/images.py` & `hcs-cli-0.1.46/vhcs/service/ims_catalog/images.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/service/inventory/vm.py` & `hcs-cli-0.1.46/vhcs/service/inventory/vm.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/service/lcm/provider.py` & `hcs-cli-0.1.46/vhcs/service/lcm/provider.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/service/lcm/template.py` & `hcs-cli-0.1.46/vhcs/service/lcm/template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/service/org_service/datacenter.py` & `hcs-cli-0.1.46/vhcs/service/org_service/datacenter.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/service/org_service/details.py` & `hcs-cli-0.1.46/vhcs/service/portal/pool.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,23 +9,32 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+import logging
 from .._util import hdc_service_client
 from vhcs.util.query_util import with_query, PageRequest
 
-_client = hdc_service_client("org-service")
+log = logging.getLogger(__name__)
+_client = hdc_service_client("portal")
 
 
-def get(id: str, **kwargs):
-    url = with_query(f"/v1/org-details/{id}", **kwargs)
+def create(payload: dict):
+    url = "/v2/pools"
+    return _client.post(url, payload)
+
+def get(id: str, org_id: str):
+    url = f"/v2/pools/{id}?org_id={org_id}"
     return _client.get(url)
 
 def list(**kwargs):
     def _get_page(query_string):
-        url = "/v1/org-details?" + query_string
+        url = "/v2/pools?" + query_string
         return _client.get(url)
-
     return PageRequest(_get_page, **kwargs).get()
+
+def delete(id: str, org_id: str):
+    url = f"/v2/pools/{id}?org_id={org_id}"
+    return _client.delete(url)
```

### Comparing `hcs-cli-0.1.45/vhcs/service/pki/certificate.py` & `hcs-cli-0.1.46/vhcs/service/pki/certificate.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/service/portal/entitlement.py` & `hcs-cli-0.1.46/vhcs/service/portal/entitlement.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/service/portal/pool.py` & `hcs-cli-0.1.46/vhcs/service/portal/site.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,23 +18,28 @@
 from vhcs.util.query_util import with_query, PageRequest
 
 log = logging.getLogger(__name__)
 _client = hdc_service_client("portal")
 
 
 def create(payload: dict):
-    url = "/v2/pools"
+    url = "/v2/sites"
     return _client.post(url, payload)
 
 def get(id: str, org_id: str):
-    url = f"/v2/pools/{id}?org_id={org_id}"
+    url = f"/v2/sites/{id}?org_id={org_id}"
     return _client.get(url)
 
 def list(**kwargs):
-    def _get_page(query_string):
-        url = "/v2/pools?" + query_string
-        return _client.get(url)
-    return PageRequest(_get_page, **kwargs).get()
+    url = with_query(f"/v2/sites", **kwargs)
+    return _client.get(url)
 
 def delete(id: str, org_id: str):
-    url = f"/v2/pools/{id}?org_id={org_id}"
-    return _client.delete(url)
+    url = f"/v2/sites/{id}?org_id={org_id}"
+    return _client.delete(url)
+
+def find_by_name(name: str, org_id: str):
+    sites = list(org_id=org_id)
+    for s in sites:
+        if s.get('name') == name:
+            return s
+
```

### Comparing `hcs-cli-0.1.45/vhcs/service/vmhub/otp.py` & `hcs-cli-0.1.46/vhcs/service/vmhub/otp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/support/daas/helper.py` & `hcs-cli-0.1.46/vhcs/support/daas/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/support/daas/infra.py` & `hcs-cli-0.1.46/vhcs/support/daas/infra.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/support/daas/infra_calc.py` & `hcs-cli-0.1.46/vhcs/support/daas/infra_calc.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/support/daas/templates/v1/tenant.blueprint.yml` & `hcs-cli-0.1.46/vhcs/support/daas/templates/v1/tenant.blueprint.yml`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
   myAADGroup:
     kind: azure/aad-group
     data:
       displayName: ${defaults.name}
       mailNickname: ${defaults.name}
       description:
+      parentGroup: ${vars.desktop.userGroup}
   
   myAADUser:
     kind: azure/aad-user
     for: email in vars.userEmails
     data:
       group: ${myAADGroup.id}
       domainName: ${myRuntime.orgIdpMap.domains[0]}
```

### Comparing `hcs-cli-0.1.45/vhcs/support/daas/tenant.py.xx` & `hcs-cli-0.1.46/vhcs/support/daas/tenant.py.xx`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/support/plan_util.py` & `hcs-cli-0.1.46/vhcs/support/plan_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/support/profile.py` & `hcs-cli-0.1.46/vhcs/support/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/util/check_license.py` & `hcs-cli-0.1.46/vhcs/util/check_license.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/util/duration.py` & `hcs-cli-0.1.46/vhcs/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/util/pki_util.py` & `hcs-cli-0.1.46/vhcs/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/util/query_util.py` & `hcs-cli-0.1.46/vhcs/util/query_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.45/vhcs/util/versions.py` & `hcs-cli-0.1.46/vhcs/util/versions.py`

 * *Files identical despite different names*

