# Comparing `tmp/xbrl-us-0.0.2.tar.gz` & `tmp/xbrl-us-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbrl-us-0.0.2.tar", last modified: Fri Jul 14 15:48:31 2023, max compression
+gzip compressed data, was "xbrl-us-0.0.3.tar", last modified: Fri Jul 14 19:00:40 2023, max compression
```

## Comparing `xbrl-us-0.0.2.tar` & `xbrl-us-0.0.3.tar`

### file list

```diff
@@ -1,111 +1,112 @@
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.470951 xbrl-us-0.0.2/
--rw-r--r--   0 hamid      (501) staff       (20)      527 2023-07-14 15:47:57.000000 xbrl-us-0.0.2/.bumpversion.cfg
--rw-r--r--   0 hamid      (501) staff       (20)     2015 2023-07-14 15:47:57.000000 xbrl-us-0.0.2/.cookiecutterrc
--rw-r--r--   0 hamid      (501) staff       (20)      175 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/.coveragerc
--rw-r--r--   0 hamid      (501) staff       (20)      353 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/.editorconfig
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.420849 xbrl-us-0.0.2/.github/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.428399 xbrl-us-0.0.2/.github/workflows/
--rw-r--r--   0 hamid      (501) staff       (20)     4514 2023-07-12 22:29:46.000000 xbrl-us-0.0.2/.github/workflows/github-actions.yml
--rw-r--r--   0 hamid      (501) staff       (20)      688 2023-06-26 21:40:12.000000 xbrl-us-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 hamid      (501) staff       (20)      285 2023-07-08 20:32:20.000000 xbrl-us-0.0.2/.readthedocs.yml
--rw-r--r--   0 hamid      (501) staff       (20)       71 2023-07-06 22:38:13.000000 xbrl-us-0.0.2/AUTHORS.rst
--rw-r--r--   0 hamid      (501) staff       (20)      377 2023-07-12 21:27:40.000000 xbrl-us-0.0.2/CHANGELOG.rst
--rw-r--r--   0 hamid      (501) staff       (20)     2376 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/CONTRIBUTING.rst
--rw-r--r--   0 hamid      (501) staff       (20)     1105 2023-06-26 21:41:13.000000 xbrl-us-0.0.2/LICENSE
--rw-r--r--   0 hamid      (501) staff       (20)      458 2023-07-12 23:53:11.000000 xbrl-us-0.0.2/MANIFEST.in
--rw-r--r--   0 hamid      (501) staff       (20)     9385 2023-07-14 15:48:31.470263 xbrl-us-0.0.2/PKG-INFO
--rw-r--r--   0 hamid      (501) staff       (20)     7743 2023-07-13 01:01:08.000000 xbrl-us-0.0.2/README.rst
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.428972 xbrl-us-0.0.2/ci/
--rwxr-xr-x   0 hamid      (501) staff       (20)     2867 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/ci/bootstrap.py
--rw-r--r--   0 hamid      (501) staff       (20)       72 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/ci/requirements.txt
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.421286 xbrl-us-0.0.2/ci/templates/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.421393 xbrl-us-0.0.2/ci/templates/.github/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.429288 xbrl-us-0.0.2/ci/templates/.github/workflows/
--rw-r--r--   0 hamid      (501) staff       (20)     1963 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.432919 xbrl-us-0.0.2/docs/
--rw-r--r--   0 hamid      (501) staff       (20)       28 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/docs/authors.rst
--rw-r--r--   0 hamid      (501) staff       (20)       30 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/docs/changelog.rst
--rw-r--r--   0 hamid      (501) staff       (20)     1155 2023-07-14 15:47:57.000000 xbrl-us-0.0.2/docs/conf.py
--rw-r--r--   0 hamid      (501) staff       (20)       33 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/docs/contributing.rst
--rw-r--r--   0 hamid      (501) staff       (20)      219 2023-07-09 12:54:31.000000 xbrl-us-0.0.2/docs/index.rst
--rw-r--r--   0 hamid      (501) staff       (20)       27 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/docs/readme.rst
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.433620 xbrl-us-0.0.2/docs/reference/
--rw-r--r--   0 hamid      (501) staff       (20)       59 2023-07-09 15:02:31.000000 xbrl-us-0.0.2/docs/reference/index.rst
--rw-r--r--   0 hamid      (501) staff       (20)       98 2023-07-09 15:02:46.000000 xbrl-us-0.0.2/docs/reference/xbrl_us.rst
--rw-r--r--   0 hamid      (501) staff       (20)       35 2023-07-09 00:13:53.000000 xbrl-us-0.0.2/docs/requirements.txt
--rw-r--r--   0 hamid      (501) staff       (20)      109 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/docs/spelling_wordlist.txt
--rw-r--r--   0 hamid      (501) staff       (20)     1194 2023-07-12 22:49:38.000000 xbrl-us-0.0.2/pyproject.toml
--rw-r--r--   0 hamid      (501) staff       (20)      772 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/pytest.ini
--rw-r--r--   0 hamid      (501) staff       (20)       38 2023-07-14 15:48:31.471122 xbrl-us-0.0.2/setup.cfg
--rwxr-xr-x   0 hamid      (501) staff       (20)     2930 2023-07-14 15:47:57.000000 xbrl-us-0.0.2/setup.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.422065 xbrl-us-0.0.2/src/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.435628 xbrl-us-0.0.2/src/xbrl_us/
--rw-r--r--   0 hamid      (501) staff       (20)       69 2023-07-14 15:47:57.000000 xbrl-us-0.0.2/src/xbrl_us/__init__.py
--rw-r--r--   0 hamid      (501) staff       (20)      372 2023-07-12 22:27:55.000000 xbrl-us-0.0.2/src/xbrl_us/__main__.py
--rw-r--r--   0 hamid      (501) staff       (20)    15086 2023-07-14 15:26:16.000000 xbrl-us-0.0.2/src/xbrl_us/app.py
--rw-r--r--   0 hamid      (501) staff       (20)      373 2023-07-12 22:49:38.000000 xbrl-us-0.0.2/src/xbrl_us/cli.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.459478 xbrl-us-0.0.2/src/xbrl_us/methods/
--rw-r--r--   0 hamid      (501) staff       (20)      964 2023-07-10 12:13:32.000000 xbrl-us-0.0.2/src/xbrl_us/methods/assertion search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      297 2023-07-10 18:27:24.000000 xbrl-us-0.0.2/src/xbrl_us/methods/assertion validate.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1002 2023-07-10 12:13:32.000000 xbrl-us-0.0.2/src/xbrl_us/methods/concept name search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1555 2023-07-10 12:13:32.000000 xbrl-us-0.0.2/src/xbrl_us/methods/concept search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1077 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/cube search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      964 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/dimension search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      672 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/document search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      480 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/dts id concept label.yml
--rw-r--r--   0 hamid      (501) staff       (20)      870 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/dts id concept name.yml
--rw-r--r--   0 hamid      (501) staff       (20)      589 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/dts id concept reference.yml
--rw-r--r--   0 hamid      (501) staff       (20)      953 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/dts id concept search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1270 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/dts id network search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      850 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/dts id network.yml
--rw-r--r--   0 hamid      (501) staff       (20)      525 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/dts search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1229 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/entity id report search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      343 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/entity id.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1273 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/entity report search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      387 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/entity search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1552 2023-07-10 19:53:06.000000 xbrl-us-0.0.2/src/xbrl_us/methods/fact id.yml
--rw-r--r--   0 hamid      (501) staff       (20)      960 2023-07-10 19:53:06.000000 xbrl-us-0.0.2/src/xbrl_us/methods/fact search oim.yml
--rw-r--r--   0 hamid      (501) staff       (20)     9191 2023-07-13 13:17:04.000000 xbrl-us-0.0.2/src/xbrl_us/methods/fact search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      519 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/label dts id search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      510 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/label search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1332 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/network id relationship search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      394 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/network id.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1319 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/network relationship search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1323 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/relationship search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      956 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/relationship tree search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     2923 2023-07-10 21:15:17.000000 xbrl-us-0.0.2/src/xbrl_us/methods/report fact search.yml
--rw-r--r--   0 hamid      (501) staff       (20)       99 2023-07-10 19:53:06.000000 xbrl-us-0.0.2/src/xbrl_us/methods/report id delete.yml
--rw-r--r--   0 hamid      (501) staff       (20)     2743 2023-07-10 20:49:26.000000 xbrl-us-0.0.2/src/xbrl_us/methods/report id fact search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      731 2023-07-10 20:05:31.000000 xbrl-us-0.0.2/src/xbrl_us/methods/report id.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1150 2023-07-10 19:53:06.000000 xbrl-us-0.0.2/src/xbrl_us/methods/report search.yml
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.466346 xbrl-us-0.0.2/src/xbrl_us/schemas/
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:52:58.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/__init__.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:14.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/assertion_details.py
--rw-r--r--   0 hamid      (501) staff       (20)     5257 2023-07-07 22:17:57.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/concept_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:14.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/cube_details.py
--rw-r--r--   0 hamid      (501) staff       (20)     1501 2023-07-07 22:17:57.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/dimension_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:36.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/document_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:29.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/dts_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:05.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/entity_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:56:32.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/fact_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:47.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/label_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:54.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/network_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:04.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/relationship_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:41:48.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/report_details.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.468644 xbrl-us-0.0.2/src/xbrl_us/utils/
--rw-r--r--   0 hamid      (501) staff       (20)       97 2023-07-10 21:39:35.000000 xbrl-us-0.0.2/src/xbrl_us/utils/__init__.py
--rw-r--r--   0 hamid      (501) staff       (20)     1377 2023-07-12 17:14:14.000000 xbrl-us-0.0.2/src/xbrl_us/utils/exceptions.py
--rw-r--r--   0 hamid      (501) staff       (20)      464 2023-07-08 23:56:22.000000 xbrl-us-0.0.2/src/xbrl_us/utils/fields.py
--rw-r--r--   0 hamid      (501) staff       (20)    26377 2023-07-07 22:12:20.000000 xbrl-us-0.0.2/src/xbrl_us/utils/paramters.py
--rw-r--r--   0 hamid      (501) staff       (20)    26440 2023-07-14 15:15:23.000000 xbrl-us-0.0.2/src/xbrl_us/xbrl_us.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.439068 xbrl-us-0.0.2/src/xbrl_us.egg-info/
--rw-r--r--   0 hamid      (501) staff       (20)     9385 2023-07-14 15:48:31.000000 xbrl-us-0.0.2/src/xbrl_us.egg-info/PKG-INFO
--rw-r--r--   0 hamid      (501) staff       (20)     2915 2023-07-14 15:48:31.000000 xbrl-us-0.0.2/src/xbrl_us.egg-info/SOURCES.txt
--rw-r--r--   0 hamid      (501) staff       (20)        1 2023-07-14 15:48:31.000000 xbrl-us-0.0.2/src/xbrl_us.egg-info/dependency_links.txt
--rw-r--r--   0 hamid      (501) staff       (20)       45 2023-07-14 15:48:31.000000 xbrl-us-0.0.2/src/xbrl_us.egg-info/entry_points.txt
--rw-r--r--   0 hamid      (501) staff       (20)        1 2023-07-12 23:37:24.000000 xbrl-us-0.0.2/src/xbrl_us.egg-info/not-zip-safe
--rw-r--r--   0 hamid      (501) staff       (20)       88 2023-07-14 15:48:31.000000 xbrl-us-0.0.2/src/xbrl_us.egg-info/requires.txt
--rw-r--r--   0 hamid      (501) staff       (20)        8 2023-07-14 15:48:31.000000 xbrl-us-0.0.2/src/xbrl_us.egg-info/top_level.txt
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.469412 xbrl-us-0.0.2/tests/
--rw-r--r--   0 hamid      (501) staff       (20)      515 2023-07-12 23:36:14.000000 xbrl-us-0.0.2/tests/test_xbrl_us.py
--rw-r--r--   0 hamid      (501) staff       (20)     1572 2023-07-12 22:40:42.000000 xbrl-us-0.0.2/tox.ini
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:00:40.303525 xbrl-us-0.0.3/
+-rw-r--r--   0 hamid      (501) staff       (20)      527 2023-07-14 18:29:56.000000 xbrl-us-0.0.3/.bumpversion.cfg
+-rw-r--r--   0 hamid      (501) staff       (20)     2015 2023-07-14 18:29:56.000000 xbrl-us-0.0.3/.cookiecutterrc
+-rw-r--r--   0 hamid      (501) staff       (20)      175 2023-06-26 21:38:04.000000 xbrl-us-0.0.3/.coveragerc
+-rw-r--r--   0 hamid      (501) staff       (20)      353 2023-06-26 21:38:04.000000 xbrl-us-0.0.3/.editorconfig
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:00:40.242473 xbrl-us-0.0.3/.github/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:00:40.251289 xbrl-us-0.0.3/.github/workflows/
+-rw-r--r--   0 hamid      (501) staff       (20)     4558 2023-07-14 18:54:07.000000 xbrl-us-0.0.3/.github/workflows/github-actions.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      688 2023-06-26 21:40:12.000000 xbrl-us-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 hamid      (501) staff       (20)      285 2023-07-08 20:32:20.000000 xbrl-us-0.0.3/.readthedocs.yml
+-rw-r--r--   0 hamid      (501) staff       (20)       71 2023-07-06 22:38:13.000000 xbrl-us-0.0.3/AUTHORS.rst
+-rw-r--r--   0 hamid      (501) staff       (20)      377 2023-07-12 21:27:40.000000 xbrl-us-0.0.3/CHANGELOG.rst
+-rw-r--r--   0 hamid      (501) staff       (20)     2376 2023-06-26 21:38:04.000000 xbrl-us-0.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 hamid      (501) staff       (20)     1105 2023-06-26 21:41:13.000000 xbrl-us-0.0.3/LICENSE
+-rw-r--r--   0 hamid      (501) staff       (20)      457 2023-07-14 18:26:55.000000 xbrl-us-0.0.3/MANIFEST.in
+-rw-r--r--   0 hamid      (501) staff       (20)     9384 2023-07-14 19:00:40.302267 xbrl-us-0.0.3/PKG-INFO
+-rw-r--r--   0 hamid      (501) staff       (20)     7743 2023-07-13 01:01:08.000000 xbrl-us-0.0.3/README.rst
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:00:40.252432 xbrl-us-0.0.3/ci/
+-rwxr-xr-x   0 hamid      (501) staff       (20)     2867 2023-06-26 21:38:04.000000 xbrl-us-0.0.3/ci/bootstrap.py
+-rw-r--r--   0 hamid      (501) staff       (20)       72 2023-06-26 21:38:04.000000 xbrl-us-0.0.3/ci/requirements.txt
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:00:40.243112 xbrl-us-0.0.3/ci/templates/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:00:40.243239 xbrl-us-0.0.3/ci/templates/.github/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:00:40.253184 xbrl-us-0.0.3/ci/templates/.github/workflows/
+-rw-r--r--   0 hamid      (501) staff       (20)     1963 2023-06-26 21:38:04.000000 xbrl-us-0.0.3/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:00:40.257493 xbrl-us-0.0.3/docs/
+-rw-r--r--   0 hamid      (501) staff       (20)       28 2023-06-26 21:38:04.000000 xbrl-us-0.0.3/docs/authors.rst
+-rw-r--r--   0 hamid      (501) staff       (20)       30 2023-06-26 21:38:04.000000 xbrl-us-0.0.3/docs/changelog.rst
+-rw-r--r--   0 hamid      (501) staff       (20)     1155 2023-07-14 18:29:56.000000 xbrl-us-0.0.3/docs/conf.py
+-rw-r--r--   0 hamid      (501) staff       (20)       33 2023-06-26 21:38:04.000000 xbrl-us-0.0.3/docs/contributing.rst
+-rw-r--r--   0 hamid      (501) staff       (20)      219 2023-07-09 12:54:31.000000 xbrl-us-0.0.3/docs/index.rst
+-rw-r--r--   0 hamid      (501) staff       (20)       27 2023-06-26 21:38:04.000000 xbrl-us-0.0.3/docs/readme.rst
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:00:40.259040 xbrl-us-0.0.3/docs/reference/
+-rw-r--r--   0 hamid      (501) staff       (20)       59 2023-07-09 15:02:31.000000 xbrl-us-0.0.3/docs/reference/index.rst
+-rw-r--r--   0 hamid      (501) staff       (20)       98 2023-07-09 15:02:46.000000 xbrl-us-0.0.3/docs/reference/xbrl_us.rst
+-rw-r--r--   0 hamid      (501) staff       (20)       35 2023-07-09 00:13:53.000000 xbrl-us-0.0.3/docs/requirements.txt
+-rw-r--r--   0 hamid      (501) staff       (20)      109 2023-06-26 21:38:04.000000 xbrl-us-0.0.3/docs/spelling_wordlist.txt
+-rw-r--r--   0 hamid      (501) staff       (20)     1194 2023-07-12 22:49:38.000000 xbrl-us-0.0.3/pyproject.toml
+-rw-r--r--   0 hamid      (501) staff       (20)      772 2023-06-26 21:38:04.000000 xbrl-us-0.0.3/pytest.ini
+-rw-r--r--   0 hamid      (501) staff       (20)       54 2023-07-14 18:22:29.000000 xbrl-us-0.0.3/secrets.yml
+-rw-r--r--   0 hamid      (501) staff       (20)       38 2023-07-14 19:00:40.303769 xbrl-us-0.0.3/setup.cfg
+-rwxr-xr-x   0 hamid      (501) staff       (20)     2929 2023-07-14 18:29:56.000000 xbrl-us-0.0.3/setup.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:00:40.243900 xbrl-us-0.0.3/src/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:00:40.261691 xbrl-us-0.0.3/src/xbrl_us/
+-rw-r--r--   0 hamid      (501) staff       (20)       69 2023-07-14 18:29:56.000000 xbrl-us-0.0.3/src/xbrl_us/__init__.py
+-rw-r--r--   0 hamid      (501) staff       (20)      372 2023-07-12 22:27:55.000000 xbrl-us-0.0.3/src/xbrl_us/__main__.py
+-rw-r--r--   0 hamid      (501) staff       (20)    15086 2023-07-14 18:15:04.000000 xbrl-us-0.0.3/src/xbrl_us/app.py
+-rw-r--r--   0 hamid      (501) staff       (20)      373 2023-07-12 22:49:38.000000 xbrl-us-0.0.3/src/xbrl_us/cli.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:00:40.289287 xbrl-us-0.0.3/src/xbrl_us/methods/
+-rw-r--r--   0 hamid      (501) staff       (20)      964 2023-07-10 12:13:32.000000 xbrl-us-0.0.3/src/xbrl_us/methods/assertion search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      297 2023-07-10 18:27:24.000000 xbrl-us-0.0.3/src/xbrl_us/methods/assertion validate.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1002 2023-07-10 12:13:32.000000 xbrl-us-0.0.3/src/xbrl_us/methods/concept name search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1555 2023-07-10 12:13:32.000000 xbrl-us-0.0.3/src/xbrl_us/methods/concept search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1077 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/cube search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      964 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/dimension search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      672 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/document search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      480 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/dts id concept label.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      870 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/dts id concept name.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      589 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/dts id concept reference.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      953 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/dts id concept search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1270 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/dts id network search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      850 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/dts id network.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      525 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/dts search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1229 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/entity id report search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      343 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/entity id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1273 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/entity report search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      387 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/entity search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1552 2023-07-10 19:53:06.000000 xbrl-us-0.0.3/src/xbrl_us/methods/fact id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      960 2023-07-10 19:53:06.000000 xbrl-us-0.0.3/src/xbrl_us/methods/fact search oim.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     9191 2023-07-13 13:17:04.000000 xbrl-us-0.0.3/src/xbrl_us/methods/fact search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      519 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/label dts id search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      510 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/label search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1332 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/network id relationship search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      394 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/network id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1319 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/network relationship search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1323 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/relationship search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      956 2023-07-10 12:16:52.000000 xbrl-us-0.0.3/src/xbrl_us/methods/relationship tree search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     2923 2023-07-10 21:15:17.000000 xbrl-us-0.0.3/src/xbrl_us/methods/report fact search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)       99 2023-07-10 19:53:06.000000 xbrl-us-0.0.3/src/xbrl_us/methods/report id delete.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     2743 2023-07-10 20:49:26.000000 xbrl-us-0.0.3/src/xbrl_us/methods/report id fact search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      731 2023-07-10 20:05:31.000000 xbrl-us-0.0.3/src/xbrl_us/methods/report id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1150 2023-07-10 19:53:06.000000 xbrl-us-0.0.3/src/xbrl_us/methods/report search.yml
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:00:40.297349 xbrl-us-0.0.3/src/xbrl_us/schemas/
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:52:58.000000 xbrl-us-0.0.3/src/xbrl_us/schemas/__init__.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:14.000000 xbrl-us-0.0.3/src/xbrl_us/schemas/assertion_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)     5257 2023-07-07 22:17:57.000000 xbrl-us-0.0.3/src/xbrl_us/schemas/concept_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:14.000000 xbrl-us-0.0.3/src/xbrl_us/schemas/cube_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)     1501 2023-07-07 22:17:57.000000 xbrl-us-0.0.3/src/xbrl_us/schemas/dimension_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:36.000000 xbrl-us-0.0.3/src/xbrl_us/schemas/document_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:29.000000 xbrl-us-0.0.3/src/xbrl_us/schemas/dts_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:05.000000 xbrl-us-0.0.3/src/xbrl_us/schemas/entity_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:56:32.000000 xbrl-us-0.0.3/src/xbrl_us/schemas/fact_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:47.000000 xbrl-us-0.0.3/src/xbrl_us/schemas/label_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:54.000000 xbrl-us-0.0.3/src/xbrl_us/schemas/network_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:04.000000 xbrl-us-0.0.3/src/xbrl_us/schemas/relationship_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:41:48.000000 xbrl-us-0.0.3/src/xbrl_us/schemas/report_details.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:00:40.300468 xbrl-us-0.0.3/src/xbrl_us/utils/
+-rw-r--r--   0 hamid      (501) staff       (20)       97 2023-07-10 21:39:35.000000 xbrl-us-0.0.3/src/xbrl_us/utils/__init__.py
+-rw-r--r--   0 hamid      (501) staff       (20)     1377 2023-07-12 17:14:14.000000 xbrl-us-0.0.3/src/xbrl_us/utils/exceptions.py
+-rw-r--r--   0 hamid      (501) staff       (20)      464 2023-07-08 23:56:22.000000 xbrl-us-0.0.3/src/xbrl_us/utils/fields.py
+-rw-r--r--   0 hamid      (501) staff       (20)    26377 2023-07-07 22:12:20.000000 xbrl-us-0.0.3/src/xbrl_us/utils/paramters.py
+-rw-r--r--   0 hamid      (501) staff       (20)    26110 2023-07-14 18:15:12.000000 xbrl-us-0.0.3/src/xbrl_us/xbrl_us.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:00:40.265360 xbrl-us-0.0.3/src/xbrl_us.egg-info/
+-rw-r--r--   0 hamid      (501) staff       (20)     9384 2023-07-14 19:00:40.000000 xbrl-us-0.0.3/src/xbrl_us.egg-info/PKG-INFO
+-rw-r--r--   0 hamid      (501) staff       (20)     2927 2023-07-14 19:00:40.000000 xbrl-us-0.0.3/src/xbrl_us.egg-info/SOURCES.txt
+-rw-r--r--   0 hamid      (501) staff       (20)        1 2023-07-14 19:00:40.000000 xbrl-us-0.0.3/src/xbrl_us.egg-info/dependency_links.txt
+-rw-r--r--   0 hamid      (501) staff       (20)       45 2023-07-14 19:00:40.000000 xbrl-us-0.0.3/src/xbrl_us.egg-info/entry_points.txt
+-rw-r--r--   0 hamid      (501) staff       (20)        1 2023-07-14 18:18:57.000000 xbrl-us-0.0.3/src/xbrl_us.egg-info/not-zip-safe
+-rw-r--r--   0 hamid      (501) staff       (20)       88 2023-07-14 19:00:40.000000 xbrl-us-0.0.3/src/xbrl_us.egg-info/requires.txt
+-rw-r--r--   0 hamid      (501) staff       (20)        8 2023-07-14 19:00:40.000000 xbrl-us-0.0.3/src/xbrl_us.egg-info/top_level.txt
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 19:00:40.301282 xbrl-us-0.0.3/tests/
+-rw-r--r--   0 hamid      (501) staff       (20)      515 2023-07-12 23:36:14.000000 xbrl-us-0.0.3/tests/test_xbrl_us.py
+-rw-r--r--   0 hamid      (501) staff       (20)     1572 2023-07-12 22:40:42.000000 xbrl-us-0.0.3/tox.ini
```

### Comparing `xbrl-us-0.0.2/.bumpversion.cfg` & `xbrl-us-0.0.3/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.0.2
+current_version = 0.0.3
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `xbrl-us-0.0.2/.cookiecutterrc` & `xbrl-us-0.0.3/.cookiecutterrc`

 * *Files 7% similar despite different names*

```diff
@@ -50,12 +50,12 @@
     scrutinizer: "no"
     setup_py_uses_setuptools_scm: "no"
     sphinx_docs: "yes"
     sphinx_docs_hosting: "https://python-xbrl-us.readthedocs.io/"
     sphinx_doctest: "no"
     sphinx_theme: "furo"
     test_matrix_separate_coverage: "no"
-    version: "0.0.2"
+    version: "0.0.3"
     version_manager: "bump2version"
     website: "https://hamidvakilzadeh.com"
     year_from: "2023"
     year_to: "2023"
```

### Comparing `xbrl-us-0.0.2/.github/workflows/github-actions.yml` & `xbrl-us-0.0.3/.github/workflows/github-actions.yml`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,15 @@
       with:
         python-version: ${{ matrix.python }}
         architecture: ${{ matrix.python_arch }}
     - name: install dependencies
       run: |
         python -mpip install --progress-bar=off -r ci/requirements.txt
         virtualenv --version
+        python -m pip install --upgrade pip
         pip --version
         tox --version
         pip list --format=freeze
     - name: test
       env:
         TOXPYTHON: '${{ matrix.toxpython }}'
       run: >
```

### Comparing `xbrl-us-0.0.2/.pre-commit-config.yaml` & `xbrl-us-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/CONTRIBUTING.rst` & `xbrl-us-0.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/LICENSE` & `xbrl-us-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/PKG-INFO` & `xbrl-us-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbrl-us
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python wrapper for xbrl.us API
 Home-page: https://github.com/hamid-vakilzadeh/python-xbrl-us
 Author: hamid-vakilzadeh
 Author-email: vakilzas@uww.edu
 License: MIT
 Project-URL: Documentation, https://python-xbrl-us.readthedocs.io/
 Project-URL: Changelog, https://python-xbrl-us.readthedocs.io/en/latest/changelog.html
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ======================
 XBRL-US Python Library
 ======================
```

### Comparing `xbrl-us-0.0.2/README.rst` & `xbrl-us-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/ci/bootstrap.py` & `xbrl-us-0.0.3/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/ci/templates/.github/workflows/github-actions.yml` & `xbrl-us-0.0.3/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/docs/conf.py` & `xbrl-us-0.0.3/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "xbrl-us"
 year = "2023"
 author = "hamid-vakilzadeh"
 copyright = f"{year}, {author}"
-version = release = "0.0.2"
+version = release = "0.0.3"
 
 pygments_style = "emacs"
 highlight_language = "python"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/hamid-vakilzadeh/python-xbrl-us/issues/%s", "#"),
     "pr": ("https://github.com/hamid-vakilzadeh/python-xbrl-us/pull/%s", "PR #"),
```

### Comparing `xbrl-us-0.0.2/pyproject.toml` & `xbrl-us-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/pytest.ini` & `xbrl-us-0.0.3/pytest.ini`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/setup.py` & `xbrl-us-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(*names, **kwargs):
     with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
     name="xbrl-us",
-    version="0.0.2",
+    version="0.0.3",
     license="MIT",
     description="Python wrapper for xbrl.us API",
     long_description_content_type="text/x-rst",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
@@ -57,15 +57,15 @@
         "Documentation": "https://python-xbrl-us.readthedocs.io/",
         "Changelog": "https://python-xbrl-us.readthedocs.io/en/latest/changelog.html",
         "Issue Tracker": "https://github.com/hamid-vakilzadeh/python-xbrl-us/issues",
     },
     keywords=[
         # eg: "xbrl-us", "xbrl", "sec",
     ],
-    python_requires=">=3.10",
+    python_requires=">=3.8",
     install_requires=["requests>=2.25.1", "pandas>=1.2.4", "PyYAML>=5.3", "sphinx-copybutton", "streamlit", "retry", "tqdm", "stqdm"],
     extras_require={
         # eg:
         #   "rst": ["docutils>=0.11"],
         #   ":python_version=="2.6"": ["argparse"],
     },
     entry_points={
```

### Comparing `xbrl-us-0.0.2/src/xbrl_us/app.py` & `xbrl-us-0.0.3/src/xbrl_us/app.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/assertion search.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/assertion search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/concept name search.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/concept name search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/concept search.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/concept search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/cube search.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/cube search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/dimension search.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/dimension search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/document search.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/document search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/dts id concept name.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/dts id concept name.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/dts id concept reference.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/dts id concept reference.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/dts id concept search.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/dts id concept search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/dts id network search.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/dts id network search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/dts id network.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/dts id network.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/dts search.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/dts search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/entity id report search.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/entity id report search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/entity report search.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/entity report search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/fact id.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/fact id.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/fact search oim.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/fact search oim.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/fact search.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/fact search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/label dts id search.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/label dts id search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/network id relationship search.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/network id relationship search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/network relationship search.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/network relationship search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/relationship search.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/relationship search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/relationship tree search.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/relationship tree search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/report fact search.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/report fact search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/report id fact search.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/report id fact search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/report id.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/report id.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/methods/report search.yml` & `xbrl-us-0.0.3/src/xbrl_us/methods/report search.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/schemas/concept_details.py` & `xbrl-us-0.0.3/src/xbrl_us/schemas/concept_details.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/schemas/dimension_details.py` & `xbrl-us-0.0.3/src/xbrl_us/schemas/dimension_details.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/utils/exceptions.py` & `xbrl-us-0.0.3/src/xbrl_us/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/utils/paramters.py` & `xbrl-us-0.0.3/src/xbrl_us/utils/paramters.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/src/xbrl_us/xbrl_us.py` & `xbrl-us-0.0.3/src/xbrl_us/xbrl_us.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,257 @@
 from .utils import exceptions
 
 logging.basicConfig()
 
 _dir = Path(__file__).resolve()
 
 
+def _remove_special_fields(fields):
+    # Define the patterns to be removed
+    patterns = [r"(.+)\.(sort\((.+)\))?$", r"(.+)\.(limit\((\d+)\))?$", r"(.+)\.(offset\((\d+)\))?$"]
+
+    # For each field, check if it matches any of the patterns. If it does, remove it.
+    for field in fields[:]:  # iterate over a slice copy of the list to safely modify it during iteration
+        if any(re.match(pattern, field, re.IGNORECASE) for pattern in patterns):
+            fields.remove(field)
+
+    return fields
+
+
+def _methods():
+    """
+    Get the names of the attributes that are allowed to be used for
+        the given method.
+    """
+    # location of all method files
+    file_path = _dir.parent / "methods"
+
+    # list all the files in the directory
+    method_files = Path(file_path).glob("*.yml")
+
+    return [file_path.stem for file_path in method_files]
+
+
+def _validate_parameters():
+    def decorator(func):
+        @wraps(func)
+        def wrapper(**kwargs):
+            """
+            Validate the parameters passed to the query method including fields, parameters, sort, limit, and offset.
+            This is a decorator for the ``_build_query_params`` method in XBRL class.
+
+            Args:
+                **kwargs: Arbitrary keyword arguments.
+
+            Returns:
+                The result of the wrapped function.
+            """
+            method_name = kwargs.get("method")
+
+            if not method_name:
+                raise exceptions.XBRLMissingValueError(param="method", expected_value=_methods())
+            elif method_name not in _methods():
+                raise exceptions.XBRLInvalidValueError(key=method_name, param="method", expected_value=_methods())
+
+            elif not isinstance(method_name, str):
+                raise exceptions.XBRLInvalidTypeError(key=method_name, received_type=type(method_name), expected_type=str)
+
+            # load the yaml file that has allowed parameters for the method
+            file_path = _dir.parent / "methods" / f"{method_name.lower()}.yml"
+
+            with file_path.open("r") as file:
+                allowed_for_query = safe_load(file)
+
+            # get the parameters, fields, limit, sort, and offset from kwargs that the user passed in
+            parameters = kwargs.get("parameters")
+            fields = kwargs.get("fields")
+            limit = kwargs.get("limit")
+            sort = kwargs.get("sort")
+            offset = kwargs.get("offset")
+            kwargs.get("print_query")
+
+            # get the allowed parameters, fields, limit, sort, and offset from the yaml file
+            allowed_params = list(allowed_for_query.get("parameters", set()).keys())
+            allowed_fields = allowed_for_query.get("fields", set())
+            allowed_limit_fields = allowed_for_query.get("limit", set())
+            allowed_sort_fields = [field for field in allowed_fields if "*" not in field]
+            allowed_offset_fields = allowed_limit_fields
+
+            # Validate fields
+            if not fields:
+                raise exceptions.XBRLMissingValueError(param="fields", expected_value=allowed_fields)
+
+            # clear the conditions from the previous query
+            # this could happen when the limit is greater than account limit or
+            # when the user passes in a field with a condition
+            fields = _remove_special_fields(fields)
+            for field in fields:
+                if not isinstance(field, str):
+                    raise exceptions.XBRLInvalidTypeError(key=field, expected_type=str, received_type=type(field))
+
+                if field not in allowed_fields:
+                    raise exceptions.XBRLInvalidValueError(key=field, param="fields", expected_value=allowed_fields, method=method_name)
+
+            # Validate parameters
+            if parameters:
+                for param in parameters:
+                    if param not in allowed_params:
+                        raise exceptions.XBRLInvalidValueError(
+                            key=param, param="parameters", expected_value=allowed_params, method=method_name
+                        )
+
+            # Validate limit
+            if limit:
+                # if not dict or an int, raise an error
+                if not isinstance(limit, int):
+                    raise exceptions.XBRLInvalidTypeError(key=limit, expected_type=int, received_type=type(limit))
+
+            else:
+                warnings.warn(
+                    "You have not set a limit; returning the first page only.",
+                    UserWarning,
+                    stacklevel=2,
+                )
+
+            # Validate sort
+            if sort:
+                if not isinstance(sort, dict):
+                    raise ValueError("Sort must be a dictionary")
+                sort = {_remove_special_fields(key): value for key, value in sort.items()}
+                for key, value in sort.items():
+                    if key not in allowed_sort_fields:
+                        raise exceptions.XBRLInvalidValueError(
+                            key=key, param="sort", expected_value=allowed_sort_fields, method=method_name
+                        )
+                    if value.lower() not in ["asc", "desc"]:
+                        raise exceptions.XBRLInvalidValueError(key=value, param="sort", expected_value=["asc", "desc"])
+            else:
+                warnings.warn(
+                    "You have not passed a sort value; for reliable results, set a field to sort.",
+                    UserWarning,
+                    stacklevel=2,
+                )
+
+            # Validate offset
+            if offset:
+                if not isinstance(offset, int):
+                    raise exceptions.XBRLInvalidTypeError(key=offset, expected_type=int, received_type=type(offset))
+
+            limit_field = next(iter(allowed_limit_fields))
+            offset_field = next(iter(allowed_offset_fields))
+
+            return func(
+                fields=fields,
+                parameters=parameters,
+                limit=limit,
+                sort=sort,
+                offset=offset,
+                limit_field=limit_field,
+                offset_field=offset_field,
+            )
+
+        return wrapper
+
+    return decorator
+
+
+def _convert_params_to_dict_decorator():
+    def decorator(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            """
+            Convert the Parameters object to a dictionary before building the query.
+            This is a decorator for the ``query`` method in XBRL class.
+
+            Args:
+                *args: Variable length argument list.
+                **kwargs: Arbitrary keyword arguments.
+
+            Returns:
+                The result of the wrapped function.
+            """
+            parameters = kwargs.get("parameters")
+            if isinstance(parameters, Parameters):
+                kwargs["parameters"] = parameters.get_parameters_dict()
+            elif parameters and not isinstance(parameters, dict):
+                raise ValueError(f"Parameters must be a dict or Parameters object. " f"Got {type(parameters)} instead.")
+            return func(*args, **kwargs)
+
+        return wrapper
+
+    return decorator
+
+
+@_validate_parameters()
+def _build_query_params(
+    fields: Optional[list] = None,
+    parameters: Optional[dict] = None,
+    limit: Optional[int] = None,
+    sort: Optional[dict] = None,
+    offset: Optional[int] = 0,
+    limit_field: Optional[str] = None,
+    offset_field: Optional[str] = None,
+) -> dict:
+    """
+    Build the query parameters for the API request in the format required by the API.
+
+    Args:
+        fields (list): The list of fields to include in the query.
+        parameters (dict): The parameters for the query.
+        limit (dict): The limit parameters for the query.
+        sort (dict): The sort parameters for the query.
+        offset (dict): dynamically set if needed
+        limit_field (str): The limit field accepted for the chosen method.
+        offset_field (str): The offset field accepted for the chosen method (which is usually the same as the
+            ``limit_filed``).
+
+    Returns:
+        dict: The query parameters that will be submitted to the API.
+    """
+    query_params = {}
+
+    if parameters:
+        # convert the parameters to a string and add it to the query_params
+        query_params.update(
+            {f"{k}": ",".join(map(str, v)) if isinstance(v, Iterable) and not isinstance(v, str) else str(v) for k, v in parameters.items()}
+        )
+
+    # Handle sort
+    if sort:
+        # check if the sort field is in the fields list
+        for field, direction in sort.items():
+            # name the field name followed by .sort(value)
+            sorted_arg = f"{field}.sort({direction.upper()})"
+            if field in fields:
+                # if the field is in the fields list, remove the field
+                fields.remove(field)
+            fields.append(sorted_arg)
+
+    # Handle limit
+    if limit:
+        # name and add the field name followed by .limit(value)
+        limit_arg = f"{limit_field}.limit({limit})"
+        if limit_field in fields:
+            # if the field is in the fields list, remove the field
+            fields.remove(limit_field)
+        fields.append(limit_arg)
+
+    # Handle offset
+    if offset:
+        # name and add the field name followed by .offset(value)
+        offset_arg = f"{offset_field}.offset({offset})"
+        if offset_field in fields:
+            fields.remove(offset_field)
+        fields.append(offset_arg)
+
+    query_params["fields"] = ",".join(fields)
+
+    return query_params
+
+
 class XBRL:
     """
     XBRL US API client. Initializes an instance of XBRL authorized connection.
 
     Args:
         client_id (str): Unique identifier agreed upon by XBRL US and the 3rd party client.
         client_secret (str): Base64 key used to authenticate the 3rd party client.
@@ -57,41 +300,14 @@
         self.access_token = None
         self.refresh_token = None
         self.account_limit = None
         self._access_token_expires_at = 0
         self._refresh_token_expires_at = 0
 
     @staticmethod
-    def acceptable_params(method_name: str):
-        """
-        Get the names of the attributes that are allowed to be used for
-            the given method.
-
-        Args:
-            method_name (str): The name of the API method to get the acceptable parameters for (e.g. "search_fact").
-
-        Returns:
-
-        """
-        file_path = _dir.parent / "methods" / f"{method_name.lower()}.yml"
-
-        with file_path.open("r") as file:
-            method_features = safe_load(file)
-
-        _attributes = {"method_name": method_name}
-        for key, _value in method_features.items():
-            _attributes[f"{key}"] = method_features.get(key)
-
-        _attributes["sort"] = [value for value in _attributes["fields"] if "*" not in value]
-
-        # Create the dynamic class using type()
-        _class = type(method_name, (), _attributes)
-        return _class()
-
-    @staticmethod
     def methods():
         """
         Get the names of the attributes that are allowed to be used for
             the given method. A list of available methods are:
 
             ===================================  ==================================================
             Method                               API Endpoint
@@ -128,21 +344,42 @@
             ``report id``                         ``/api/v1/report/{report.id}``
             ``report id delete``                  ``/api/v1/report/{report.id}/delete``
             ``report id fact``                    ``/api/v1/report/{report.id}/fact/search``
             ``report search``                     ``/api/v1/report/search``
             ===================================  ==================================================
 
         """
-        # location of all method files
-        file_path = _dir.parent / "methods"
+        return _methods()
+
+    @staticmethod
+    def acceptable_params(method_name: str):
+        """
+        Get the names of the attributes that are allowed to be used for
+            the given method.
+
+        Args:
+            method_name (str): The name of the API method to get the acceptable parameters for (e.g. "search_fact").
+
+        Returns:
+
+        """
+        file_path = _dir.parent / "methods" / f"{method_name.lower()}.yml"
+
+        with file_path.open("r") as file:
+            method_features = safe_load(file)
+
+        _attributes = {"method_name": method_name}
+        for key, _value in method_features.items():
+            _attributes[f"{key}"] = method_features.get(key)
 
-        # list all the files in the directory
-        method_files = Path(file_path).glob("*.yml")
+        _attributes["sort"] = [value for value in _attributes["fields"] if "*" not in value]
 
-        return [file_path.stem for file_path in method_files]
+        # Create the dynamic class using type()
+        _class = type(method_name, (), _attributes)
+        return _class()
 
     def _get_token(self, grant_type: Optional[str] = None, refresh_token=None):
         """
         Retrieves an access token from the token URL.
 
         Args:
             grant_type (str): The grant type (default: "password").
@@ -227,244 +464,15 @@
         match = re.search(r"user limit amount is (\d+)", response.text)
         if match:
             self.account_limit = int(match.group(1))
         else:
             print(f"Error: {response.status_code}")
             self.account_limit = None
 
-    @staticmethod
-    def _remove_special_fields(fields):
-        # Define the patterns to be removed
-        patterns = [r"(.+)\.(sort\((.+)\))?$", r"(.+)\.(limit\((\d+)\))?$", r"(.+)\.(offset\((\d+)\))?$"]
-
-        # For each field, check if it matches any of the patterns. If it does, remove it.
-        for field in fields[:]:  # iterate over a slice copy of the list to safely modify it during iteration
-            if any(re.match(pattern, field, re.IGNORECASE) for pattern in patterns):
-                fields.remove(field)
-
-        return fields
-
-    @staticmethod
-    def _validate_parameters(func):
-        @wraps(func)
-        def wrapper(instance, **kwargs):
-            """
-            Validate the parameters passed to the query method including fields, parameters, sort, limit, and offset.
-            This is a decorator for the query _build_query_params method.
-
-            Args:
-                instance (XBRLAPIClient): The instance of the XBRLAPIClient.
-                **kwargs: Arbitrary keyword arguments.
-
-            Returns:
-                The result of the wrapped function.
-            """
-            method_name = kwargs.get("method")
-
-            if not method_name:
-                raise exceptions.XBRLMissingValueError(param="method", expected_value=instance.methods())
-            elif method_name not in instance.methods():
-                raise exceptions.XBRLInvalidValueError(key=method_name, param="method", expected_value=instance.methods())
-
-            elif not isinstance(method_name, str):
-                raise exceptions.XBRLInvalidTypeError(key=method_name, received_type=type(method_name), expected_type=str)
-
-            # load the yaml file that has allowed parameters for the method
-            file_path = _dir.parent / "methods" / f"{method_name.lower()}.yml"
-
-            with file_path.open("r") as file:
-                allowed_for_query = safe_load(file)
-
-            # get the parameters, fields, limit, sort, and offset from kwargs that the user passed in
-            parameters = kwargs.get("parameters")
-            fields = kwargs.get("fields")
-            limit = kwargs.get("limit")
-            sort = kwargs.get("sort")
-            offset = kwargs.get("offset")
-            kwargs.get("print_query")
-
-            # get the allowed parameters, fields, limit, sort, and offset from the yaml file
-            allowed_params = list(allowed_for_query.get("parameters", set()).keys())
-            allowed_fields = allowed_for_query.get("fields", set())
-            allowed_limit_fields = allowed_for_query.get("limit", set())
-            allowed_sort_fields = [field for field in allowed_fields if "*" not in field]
-            allowed_offset_fields = allowed_limit_fields
-
-            # Validate fields
-            if not fields:
-                raise exceptions.XBRLMissingValueError(param="fields", expected_value=allowed_fields)
-
-            # clear the conditions from the previous query
-            # this could happen when the limit is greater than account limit or
-            # when the user passes in a field with a condition
-            fields = instance._remove_special_fields(fields)
-            for field in fields:
-                if not isinstance(field, str):
-                    raise exceptions.XBRLInvalidTypeError(key=field, expected_type=str, received_type=type(field))
-
-                if field not in allowed_fields:
-                    raise exceptions.XBRLInvalidValueError(key=field, param="fields", expected_value=allowed_fields, method=method_name)
-
-            # Validate parameters
-            if parameters:
-                for param in parameters:
-                    if param not in allowed_params:
-                        raise exceptions.XBRLInvalidValueError(
-                            key=param, param="parameters", expected_value=allowed_params, method=method_name
-                        )
-
-            # Validate limit
-            if limit:
-                # if not dict or an int, raise an error
-                if not isinstance(limit, int):
-                    raise exceptions.XBRLInvalidTypeError(key=limit, expected_type=int, received_type=type(limit))
-
-            else:
-                warnings.warn(
-                    "You have not set a limit; returning the first page only.",
-                    UserWarning,
-                    stacklevel=2,
-                )
-
-            # Validate sort
-            if sort:
-                if not isinstance(sort, dict):
-                    raise ValueError("Sort must be a dictionary")
-                sort = {instance._remove_special_fields(key): value for key, value in sort.items()}
-                for key, value in sort.items():
-                    if key not in allowed_sort_fields:
-                        raise exceptions.XBRLInvalidValueError(
-                            key=key, param="sort", expected_value=allowed_sort_fields, method=method_name
-                        )
-                    if value.lower() not in ["asc", "desc"]:
-                        raise exceptions.XBRLInvalidValueError(key=value, param="sort", expected_value=["asc", "desc"])
-            else:
-                warnings.warn(
-                    "You have not passed a sort value; for reliable results, set a field to sort.",
-                    UserWarning,
-                    stacklevel=2,
-                )
-
-            # Validate offset
-            if offset:
-                if not isinstance(offset, int):
-                    raise exceptions.XBRLInvalidTypeError(key=offset, expected_type=int, received_type=type(offset))
-
-            limit_field = next(iter(allowed_limit_fields))
-            offset_field = next(iter(allowed_offset_fields))
-
-            return func(
-                instance,
-                fields=fields,
-                parameters=parameters,
-                limit=limit,
-                sort=sort,
-                offset=offset,
-                limit_field=limit_field,
-                offset_field=offset_field,
-            )
-
-        return wrapper
-
-    @_validate_parameters
-    def _build_query_params(
-        self,
-        fields: Optional[list] = None,
-        parameters: Optional[dict] = None,
-        limit: Optional[int] = None,
-        sort: Optional[dict] = None,
-        offset: Optional[int] = 0,
-        limit_field: Optional[str] = None,
-        offset_field: Optional[str] = None,
-    ) -> dict:
-        """
-        Build the query parameters for the API request in the format required by the API.
-
-        Args:
-            fields (list): The list of fields to include in the query.
-            parameters (dict): The parameters for the query.
-            limit (dict): The limit parameters for the query.
-            sort (dict): The sort parameters for the query.
-            offset (dict): dynamically set if needed
-            limit_field (str): The limit field accepted for the chosen method.
-            offset_field (str): The offset field accepted for the chosen method (which is usually the same as the
-                ``limit_filed``).
-
-        Returns:
-            dict: The query parameters that will be submitted to the API.
-        """
-        query_params = {}
-
-        if parameters:
-            # convert the parameters to a string and add it to the query_params
-            query_params.update(
-                {
-                    f"{k}": ",".join(map(str, v)) if isinstance(v, Iterable) and not isinstance(v, str) else str(v)
-                    for k, v in parameters.items()
-                }
-            )
-
-        # Handle sort
-        if sort:
-            # check if the sort field is in the fields list
-            for field, direction in sort.items():
-                # name the field name followed by .sort(value)
-                sorted_arg = f"{field}.sort({direction.upper()})"
-                if field in fields:
-                    # if the field is in the fields list, remove the field
-                    fields.remove(field)
-                fields.append(sorted_arg)
-
-        # Handle limit
-        if limit:
-            # name and add the field name followed by .limit(value)
-            limit_arg = f"{limit_field}.limit({limit})"
-            if limit_field in fields:
-                # if the field is in the fields list, remove the field
-                fields.remove(limit_field)
-            fields.append(limit_arg)
-
-        # Handle offset
-        if offset:
-            # name and add the field name followed by .offset(value)
-            offset_arg = f"{offset_field}.offset({offset})"
-            if offset_field in fields:
-                fields.remove(offset_field)
-            fields.append(offset_arg)
-
-        query_params["fields"] = ",".join(fields)
-
-        return query_params
-
-    @staticmethod
-    def _convert_params_to_dict_decorator(func):
-        @wraps(func)
-        def wrapper(self, *args, **kwargs):
-            """
-            Convert the Parameters object to a dictionary before building the query.
-
-            Args:
-                self: The instance of the XBRL class.
-                *args: Variable length argument list.
-                **kwargs: Arbitrary keyword arguments.
-
-            Returns:
-                The result of the wrapped function.
-            """
-            parameters = kwargs.get("parameters")
-            if isinstance(parameters, Parameters):
-                kwargs["parameters"] = parameters.get_parameters_dict()
-            elif parameters and not isinstance(parameters, dict):
-                raise ValueError(f"Parameters must be a dict or Parameters object. " f"Got {type(parameters)} instead.")
-            return func(self, *args, **kwargs)
-
-        return wrapper
-
-    @staticmethod
-    def _get_method_url(method_name: str, parameters) -> str:
+    def _get_method_url(self, method_name: str, parameters) -> str:
         """
         Get the URL for the specified method from the YAML file.
 
         Args:
             method_name (str): The name of the method.
             parameters: The parameters for the method.
 
@@ -493,15 +501,15 @@
 
             # get the required parameters for this method
             for key, value in values.items():
                 placeholder = "{" + key + "}"
                 url = url.replace(placeholder, str(value))
         return f"https://api.xbrl.us{url}?"
 
-    @_convert_params_to_dict_decorator
+    @_convert_params_to_dict_decorator()
     def query(
         self,
         method: str,
         fields: Optional[list] = None,
         parameters: Optional[Union[Parameters, dict]] = None,
         limit: Optional[int] = None,
         sort: Optional[dict] = None,
@@ -532,15 +540,15 @@
 
         method_url = self._get_method_url(method, parameters)
         # if limit is all
         if limit == "all":
             # arbitrary large number
             limit = 999999999
 
-        query_params = self._build_query_params(
+        query_params = _build_query_params(
             method=method,
             fields=fields,
             parameters=parameters,
             limit=limit,
             sort=sort,
         )
 
@@ -560,15 +568,15 @@
 
             pbar = stqdm(total=None, desc="Downloading Data:", ncols=80)
         else:
             # create a progress bar
             pbar = tqdm(total=None, desc="Downloading Data:", ncols=80)
 
         # update the limit in the query params with the new limit
-        query_params = self._build_query_params(
+        query_params = _build_query_params(
             method=method,
             fields=fields,
             parameters=parameters,
             limit=account_limit,
             sort=sort,
         )
 
@@ -606,15 +614,15 @@
 
         offset = len(data)
 
         while remaining_limit > 0:
             # Determine the limit for the current request
             try:
                 current_limit = min(account_limit, remaining_limit)
-                query_params = self._build_query_params(
+                query_params = _build_query_params(
                     method=method,
                     fields=fields,
                     parameters=parameters,
                     limit=current_limit,
                     sort=sort,
                     offset=offset,
                 )
```

### Comparing `xbrl-us-0.0.2/src/xbrl_us.egg-info/PKG-INFO` & `xbrl-us-0.0.3/src/xbrl_us.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbrl-us
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python wrapper for xbrl.us API
 Home-page: https://github.com/hamid-vakilzadeh/python-xbrl-us
 Author: hamid-vakilzadeh
 Author-email: vakilzas@uww.edu
 License: MIT
 Project-URL: Documentation, https://python-xbrl-us.readthedocs.io/
 Project-URL: Changelog, https://python-xbrl-us.readthedocs.io/en/latest/changelog.html
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ======================
 XBRL-US Python Library
 ======================
```

### Comparing `xbrl-us-0.0.2/src/xbrl_us.egg-info/SOURCES.txt` & `xbrl-us-0.0.3/src/xbrl_us.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 pytest.ini
+secrets.yml
 setup.py
 tox.ini
 .github/workflows/github-actions.yml
 ci/bootstrap.py
 ci/requirements.txt
 ci/templates/.github/workflows/github-actions.yml
 docs/authors.rst
```

### Comparing `xbrl-us-0.0.2/tests/test_xbrl_us.py` & `xbrl-us-0.0.3/tests/test_xbrl_us.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.2/tox.ini` & `xbrl-us-0.0.3/tox.ini`

 * *Files identical despite different names*

