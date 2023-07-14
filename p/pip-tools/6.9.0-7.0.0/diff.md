# Comparing `tmp/pip-tools-6.9.0.tar.gz` & `tmp/pip-tools-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip-tools-6.9.0.tar", last modified: Wed Oct  5 19:50:10 2022, max compression
+gzip compressed data, was "pip-tools-7.0.0.tar", last modified: Fri Jul 14 19:40:40 2023, max compression
```

## Comparing `pip-tools-6.9.0.tar` & `pip-tools-7.0.0.tar`

### file list

```diff
@@ -1,129 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.651691 pip-tools-6.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.bandit
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.635689 pip-tools-6.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.635689 pip-tools-6.9.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.639690 pip-tools-6.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     4548 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2989 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.github/workflows/cron.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1838 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.github/workflows/qa.yml
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.prettierrc.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-10-05 19:49:52.000000 pip-tools-6.9.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    36887 2022-10-05 19:49:52.000000 pip-tools-6.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     2375 2022-10-05 19:49:52.000000 pip-tools-6.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     2871 2022-10-05 19:49:52.000000 pip-tools-6.9.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-10-05 19:49:52.000000 pip-tools-6.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    22014 2022-10-05 19:50:10.651691 pip-tools-6.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    20862 2022-10-05 19:49:52.000000 pip-tools-6.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-10-05 19:49:52.000000 pip-tools-6.9.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.639690 pip-tools-6.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-10-05 19:49:52.000000 pip-tools-6.9.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-10-05 19:49:52.000000 pip-tools-6.9.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-10-05 19:49:52.000000 pip-tools-6.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-10-05 19:49:52.000000 pip-tools-6.9.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-10-05 19:49:52.000000 pip-tools-6.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-05 19:49:52.000000 pip-tools-6.9.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.639690 pip-tools-6.9.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-10-05 19:49:52.000000 pip-tools-6.9.0/examples/django.in
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-05 19:49:52.000000 pip-tools-6.9.0/examples/flask.in
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-10-05 19:49:52.000000 pip-tools-6.9.0/examples/hypothesis.in
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-10-05 19:49:52.000000 pip-tools-6.9.0/examples/protection.in
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-05 19:49:52.000000 pip-tools-6.9.0/examples/sentry.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.639690 pip-tools-6.9.0/img/
--rw-r--r--   0 runner    (1001) docker     (121)    10481 2022-10-05 19:49:52.000000 pip-tools-6.9.0/img/pip-tools-overview.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.639690 pip-tools-6.9.0/pip_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    22014 2022-10-05 19:50:10.000000 pip-tools-6.9.0/pip_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3342 2022-10-05 19:50:10.000000 pip-tools-6.9.0/pip_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 19:50:10.000000 pip-tools-6.9.0/pip_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-10-05 19:50:10.000000 pip-tools-6.9.0/pip_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 19:50:10.000000 pip-tools-6.9.0/pip_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-10-05 19:50:10.000000 pip-tools-6.9.0/pip_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-05 19:50:10.000000 pip-tools-6.9.0/pip_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.643690 pip-tools-6.9.0/piptools/
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.643690 pip-tools-6.9.0/piptools/_compat/
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/_compat/click.py
--rw-r--r--   0 runner    (1001) docker     (121)     3023 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/_compat/pip_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     5981 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/locations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.643690 pip-tools-6.9.0/piptools/repositories/
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/repositories/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3685 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/repositories/local.py
--rw-r--r--   0 runner    (1001) docker     (121)    20253 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/repositories/pypi.py
--rw-r--r--   0 runner    (1001) docker     (121)    29822 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.643690 pip-tools-6.9.0/piptools/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    17876 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/scripts/compile.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9158 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/scripts/sync.py
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8208 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/sync.py
--rw-r--r--   0 runner    (1001) docker     (121)    16164 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10670 2022-10-05 19:49:52.000000 pip-tools-6.9.0/piptools/writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2566 2022-10-05 19:50:10.651691 pip-tools-6.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-10-05 19:49:52.000000 pip-tools-6.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.647691 pip-tools-6.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11576 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     3708 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)    74698 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_cli_compile.py
--rw-r--r--   0 runner    (1001) docker     (121)    10435 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_cli_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.647691 pip-tools-6.9.0/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/fake-editables.json
--rw-r--r--   0 runner    (1001) docker     (121)     2737 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/fake-index.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.647691 pip-tools-6.9.0/tests/test_data/minimal_wheels/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small-fake-multi-arch-0.1.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_a-0.1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1632 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_a-0.2-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_a-0.3b1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_b-0.1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_b-0.2-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_b-0.3-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_i686.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_x86_64.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-win32.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_with_deps-0.1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_with_deps_and_sub_deps-0.1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_with_unpinned_deps-0.1-py2.py3-none-any.whl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.631688 pip-tools-6.9.0/tests/test_data/packages/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.647691 pip-tools-6.9.0/tests/test_data/packages/fake_with_deps/
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/packages/fake_with_deps/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.647691 pip-tools-6.9.0/tests/test_data/packages/small_fake_a/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/packages/small_fake_a/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.647691 pip-tools-6.9.0/tests/test_data/packages/small_fake_with_deps/
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/packages/small_fake_with_deps/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.647691 pip-tools-6.9.0/tests/test_data/packages/small_fake_with_deps_and_sub_deps/
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/packages/small_fake_with_deps_and_sub_deps/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.631688 pip-tools-6.9.0/tests/test_data/packages/small_fake_with_subdir/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.651691 pip-tools-6.9.0/tests/test_data/packages/small_fake_with_subdir/subdir/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/packages/small_fake_with_subdir/subdir/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 19:50:10.651691 pip-tools-6.9.0/tests/test_data/packages/small_fake_with_unpinned_deps/
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_data/packages/small_fake_with_unpinned_deps/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     2897 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_fake_index.py
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_minimal_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (121)     2192 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_repository_local.py
--rw-r--r--   0 runner    (1001) docker     (121)    13116 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_repository_pypi.py
--rw-r--r--   0 runner    (1001) docker     (121)    23734 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    14541 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_top_level_editable.py
--rw-r--r--   0 runner    (1001) docker     (121)    19334 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    12133 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/test_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2872 2022-10-05 19:49:52.000000 pip-tools-6.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.610777 pip-tools-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.bandit
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.586777 pip-tools-7.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.586777 pip-tools-7.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.586777 pip-tools-7.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.github/workflows/cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.github/workflows/reusable-qa.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-14 19:40:12.000000 pip-tools-7.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    42979 2023-07-14 19:40:12.000000 pip-tools-7.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-14 19:40:12.000000 pip-tools-7.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-14 19:40:12.000000 pip-tools-7.0.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-14 19:40:12.000000 pip-tools-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22696 2023-07-14 19:40:40.610777 pip-tools-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-07-14 19:40:12.000000 pip-tools-7.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 19:40:12.000000 pip-tools-7.0.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.590777 pip-tools-7.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-14 19:40:12.000000 pip-tools-7.0.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 19:40:12.000000 pip-tools-7.0.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-14 19:40:12.000000 pip-tools-7.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 19:40:12.000000 pip-tools-7.0.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-14 19:40:12.000000 pip-tools-7.0.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-14 19:40:12.000000 pip-tools-7.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.590777 pip-tools-7.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-14 19:40:12.000000 pip-tools-7.0.0/examples/django.in
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 19:40:12.000000 pip-tools-7.0.0/examples/flask.in
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 19:40:12.000000 pip-tools-7.0.0/examples/hypothesis.in
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-14 19:40:12.000000 pip-tools-7.0.0/examples/protection.in
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 19:40:12.000000 pip-tools-7.0.0/examples/sentry.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.590777 pip-tools-7.0.0/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-07-14 19:40:12.000000 pip-tools-7.0.0/img/pip-tools-overview.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.590777 pip-tools-7.0.0/pip_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22696 2023-07-14 19:40:40.000000 pip-tools-7.0.0/pip_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-14 19:40:40.000000 pip-tools-7.0.0/pip_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:40:40.000000 pip-tools-7.0.0/pip_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-14 19:40:40.000000 pip-tools-7.0.0/pip_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-14 19:40:40.000000 pip-tools-7.0.0/pip_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 19:40:40.000000 pip-tools-7.0.0/pip_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.594777 pip-tools-7.0.0/piptools/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.594777 pip-tools-7.0.0/piptools/_compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/_compat/pip_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.594777 pip-tools-7.0.0/piptools/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/repositories/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/repositories/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/repositories/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30467 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.594777 pip-tools-7.0.0/piptools/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22000 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/scripts/compile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9713 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/scripts/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22678 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11060 2023-07-14 19:40:12.000000 pip-tools-7.0.0/piptools/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-14 19:40:12.000000 pip-tools-7.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 19:40:40.610777 pip-tools-7.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.602777 pip-tools-7.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92853 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_cli_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12174 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_cli_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.602777 pip-tools-7.0.0/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/fake-editables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/fake-index.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.606778 pip-tools-7.0.0/tests/test_data/minimal_wheels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small-fake-multi-arch-0.1.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_a-0.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_a-0.2-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_a-0.3b1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_b-0.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_b-0.2-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_b-0.3-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_i686.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_x86_64.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-win32.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_with_deps-0.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_with_deps_and_sub_deps-0.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_with_unpinned_deps-0.1-py2.py3-none-any.whl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.582777 pip-tools-7.0.0/tests/test_data/packages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.606778 pip-tools-7.0.0/tests/test_data/packages/fake_with_deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/packages/fake_with_deps/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.606778 pip-tools-7.0.0/tests/test_data/packages/small_fake_a/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/packages/small_fake_a/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.610777 pip-tools-7.0.0/tests/test_data/packages/small_fake_with_deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/packages/small_fake_with_deps/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.610777 pip-tools-7.0.0/tests/test_data/packages/small_fake_with_deps_and_sub_deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/packages/small_fake_with_deps_and_sub_deps/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.582777 pip-tools-7.0.0/tests/test_data/packages/small_fake_with_subdir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.610777 pip-tools-7.0.0/tests/test_data/packages/small_fake_with_subdir/subdir/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/packages/small_fake_with_subdir/subdir/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:40.610777 pip-tools-7.0.0/tests/test_data/packages/small_fake_with_unpinned_deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_data/packages/small_fake_with_unpinned_deps/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_fake_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_minimal_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_repository_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15868 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_repository_pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23770 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_top_level_editable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24294 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-14 19:40:12.000000 pip-tools-7.0.0/tox.ini
```

### Comparing `pip-tools-6.9.0/.github/ISSUE_TEMPLATE/feature-request.md` & `pip-tools-7.0.0/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `pip-tools-6.9.0/.github/PULL_REQUEST_TEMPLATE.md` & `pip-tools-7.0.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pip-tools-6.9.0/.github/release-drafter.yml` & `pip-tools-7.0.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pip-tools-6.9.0/.github/workflows/qa.yml` & `pip-tools-7.0.0/.github/workflows/reusable-qa.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,11 @@
 name: QA
 
 on:
-  pull_request:
-  push:
-    branches:
-      - master
-    tags:
-
-concurrency:
-  group: ${{ github.workflow }}-${{ github.event.pull_request.number || github.sha }}
-  cancel-in-progress: true
+  workflow_call:
 
 jobs:
   qa:
     name: ${{ matrix.toxenv }}
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
@@ -25,37 +17,37 @@
         python-version:
           - "3.x"
     env:
       PY_COLORS: 1
       TOXENV: ${{ matrix.toxenv }}
       TOX_PARALLEL_NO_SPINNER: 1
     steps:
-      - uses: actions/checkout@master
+      - uses: actions/checkout@main
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Get pip cache dir
         id: pip-cache
         run: |
-          echo "::set-output name=dir::$(pip cache dir)"
+          echo "dir=$(pip cache dir)" >> $GITHUB_OUTPUT
       - name: Pip cache
         uses: actions/cache@v3
         with:
           path: ${{ steps.pip-cache.outputs.dir }}
           key: >-
             ${{ runner.os }}-pip-${{ hashFiles('setup.cfg') }}-${{
-            hashFiles('setup.py') }}-${{ hashFiles('tox.ini') }}-${{
+            hashFiles('pyproject.toml') }}-${{ hashFiles('tox.ini') }}-${{
             hashFiles('.pre-commit-config.yaml') }}
           restore-keys: |
             ${{ runner.os }}-pip-
             ${{ runner.os }}-
       - name: Prepare cache key
         id: cache-key
-        run: echo "::set-output name=sha-256::$(python -VV | sha256sum | cut -d' ' -f1)"
+        run: echo "sha-256=$(python -VV | sha256sum | cut -d' ' -f1)" >> $GITHUB_OUTPUT
       - uses: actions/cache@v3
         with:
           path: ~/.cache/pre-commit
           key: pre-commit|${{ steps.cache-key.outputs.sha-256 }}|${{ hashFiles('.pre-commit-config.yaml') }}
       - name: Install tox
         run: pip install tox
       - name: Prepare test environment
```

### Comparing `pip-tools-6.9.0/.github/workflows/release-drafter.yml` & `pip-tools-7.0.0/.github/workflows/release-drafter.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 name: release-drafter
 
 on:
   push:
     # branches to consider in the event; optional, defaults to all
     branches:
-      - master
+      - main
       - "releases/**"
       - "stable/**"
 
 jobs:
   update_release_draft:
     permissions:
       contents: write
       pull-requests: read
     if: github.repository == 'jazzband/pip-tools'
     runs-on: ubuntu-latest
     steps:
-      # Drafts your next release notes as Pull Requests are merged into "master"
+      # Drafts your next release notes as Pull Requests are merged into "main"
       - uses: release-drafter/release-drafter@v5
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `pip-tools-6.9.0/.github/workflows/release.yml` & `pip-tools-7.0.0/.github/workflows/release.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Release
 
 on:
   push:
     branches:
-      - master
+      - main
   release:
     types:
       - published
 
 jobs:
   build:
     if: github.repository == 'jazzband/pip-tools'
@@ -22,22 +22,22 @@
         uses: actions/setup-python@v4
         with:
           python-version: 3.9
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
-          python -m pip install -U setuptools twine wheel
+          python -m pip install -U twine build setuptools-scm
 
       - name: Build package
         run: |
-          python setup.py --version
-          python setup.py sdist --format=gztar bdist_wheel
-          twine check dist/*
+          python -m setuptools_scm
+          python -m build
+          twine check --strict dist/*
 
       - name: Upload packages to Jazzband
         if: github.event.action == 'published'
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: jazzband
           password: ${{ secrets.JAZZBAND_RELEASE_KEY }}
           repository_url: https://jazzband.co/projects/pip-tools/upload
```

### Comparing `pip-tools-6.9.0/.pre-commit-config.yaml` & `pip-tools-7.0.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 repos:
   - repo: https://github.com/psf/black
-    rev: 22.8.0
+    rev: 23.3.0
     hooks:
       - id: black
-        args: [--target-version=py36]
+        args: [--target-version=py38]
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.38.2
+    rev: v3.3.1
     hooks:
       - id: pyupgrade
-        args: [--py37-plus]
+        args: [--py38-plus]
   - repo: https://github.com/PyCQA/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies:
           - flake8-pytest-style
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.981
+    rev: v1.2.0
     hooks:
       - id: mypy
         # Avoid error: Duplicate module named 'setup'
         # https://github.com/python/mypy/issues/4008
         # Keep exclude in sync with mypy own excludes
         exclude: ^tests/test_data/
         additional_dependencies:
           - click==8.0.1
           - pep517==0.10.0
           - toml==0.10.2
           - pip==20.3.4
+          - build==0.9.0
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.4
+    rev: 1.7.5
     hooks:
       - id: bandit
         args: [--ini, .bandit]
         exclude: ^tests/
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.0
+    rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
+        additional_dependencies:
+          - "prettier"
+          - "prettier-plugin-toml"
```

### Comparing `pip-tools-6.9.0/CHANGELOG.md` & `pip-tools-7.0.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,166 @@
+## 7.0.0 (2023-07-14)
+
+Backwards Incompatible Changes:
+
+- Default to `--resolver=backtracking`
+  ([#1897](https://github.com/jazzband/pip-tools/pull/1897)). Thanks @atugushev
+- Drop support for Python 3.7
+  ([#1879](https://github.com/jazzband/pip-tools/pull/1879)). Thanks @chrysle
+
+Features:
+
+- Add support for `pip==23.2` where refactored out `DEV_PKGS`
+  ([#1906](https://github.com/jazzband/pip-tools/pull/1906)). Thanks @atugushev
+- Add `--no-config` option ([#1896](https://github.com/jazzband/pip-tools/pull/1896)).
+  Thanks @atugushev
+
+Bug Fixes:
+
+- Sync direct references with hashes
+  ([#1885](https://github.com/jazzband/pip-tools/pull/1885)). Thanks @siddharthab
+- Fix missing `via`s when more than two input files are used
+  ([#1890](https://github.com/jazzband/pip-tools/pull/1890)). Thanks @lpulley
+
+## 6.14.0 (2023-06-28)
+
+Features:
+
+- Support config defaults using `.pip-tools.toml` or `pyproject.toml`
+  ([#1863](https://github.com/jazzband/pip-tools/pull/1863)). Thanks @j00bar
+- Log a warning if the user specifies `-P` and the output file is present but empty
+  ([#1822](https://github.com/jazzband/pip-tools/pull/1822)). Thanks @davidmreed
+- Improve warning for `pip-compile` if no `--allow-unsafe` was passed
+  ([#1867](https://github.com/jazzband/pip-tools/pull/1867)). Thanks @chrysle
+
+Other Changes:
+
+- Correct in README `pre-commit` hook to run off `requirements.in`
+  ([#1847](https://github.com/jazzband/pip-tools/pull/1847)). Thanks @atugushev
+- Add pyprojects.toml example for using setuptools
+  ([#1851](https://github.com/jazzband/pip-tools/pull/1851)). Thanks @shatakshiiii
+
+## 6.13.0 (2023-04-07)
+
+Features:
+
+- Add support for self-referential extras
+  ([#1791](https://github.com/jazzband/pip-tools/pull/1791)). Thanks @q0w
+- Add support for `pip==23.1` where removed `FormatControl` in `WheelCache`
+  ([#1834](https://github.com/jazzband/pip-tools/pull/1834)). Thanks @atugushev
+- Add support for `pip==23.1` where refactored requirement options
+  ([#1832](https://github.com/jazzband/pip-tools/pull/1832)). Thanks @atugushev
+- Add support for `pip==23.1` where deprecated `--install-option` has been removed
+  ([#1828](https://github.com/jazzband/pip-tools/pull/1828)). Thanks @atugushev
+
+Bug Fixes:
+
+- Pass `--cache-dir` to `--pip-args` for backtracking resolver
+  ([#1827](https://github.com/jazzband/pip-tools/pull/1827)). Thanks @q0w
+
+Other Changes:
+
+- Update examples in README ([#1835](https://github.com/jazzband/pip-tools/pull/1835)).
+  Thanks @lucaswerkmeister
+
+## 6.12.3 (2023-03-01)
+
+Bug Fixes:
+
+- Remove extras from user-supplied constraints in backtracking resolver
+  ([#1808](https://github.com/jazzband/pip-tools/pull/1808)). Thanks @thomdixon
+- Fix for sync error when the ireqs being merged have no names
+  ([#1802](https://github.com/jazzband/pip-tools/pull/1802)). Thanks @richafrank
+
+## 6.12.2 (2022-12-25)
+
+Bug Fixes:
+
+- Raise error if input and output filenames are matched
+  ([#1787](https://github.com/jazzband/pip-tools/pull/1787)). Thanks @atugushev
+- Add `pyproject.toml` as default input file format
+  ([#1780](https://github.com/jazzband/pip-tools/pull/1780)). Thanks @berislavlopac
+- Fix a regression with unsafe packages for `--allow-unsafe`
+  ([#1788](https://github.com/jazzband/pip-tools/pull/1788)). Thanks @q0w
+
+## 6.12.1 (2022-12-16)
+
+Bug Fixes:
+
+- Set explicitly packages for setuptools
+  ([#1782](https://github.com/jazzband/pip-tools/pull/1782)). Thanks @q0w
+
+## 6.12.0 (2022-12-13)
+
+Features:
+
+- Add `--no-index` flag to `pip-compile`
+  ([#1745](https://github.com/jazzband/pip-tools/pull/1745)). Thanks @atugushev
+
+Bug Fixes:
+
+- Treat `--upgrade-packages` PKGSPECs as constraints (not just minimums), consistently
+  ([#1578](https://github.com/jazzband/pip-tools/pull/1578)). Thanks @AndydeCleyre
+- Filter out the user provided unsafe packages
+  ([#1766](https://github.com/jazzband/pip-tools/pull/1766)). Thanks @q0w
+- Adopt PEP-621 for packaging
+  ([#1763](https://github.com/jazzband/pip-tools/pull/1763)). Thanks @ssbarnea
+
+## 6.11.0 (2022-11-30)
+
+Features:
+
+- Add `pyproject.toml` file ([#1643](https://github.com/jazzband/pip-tools/pull/1643)).
+  Thanks @otherJL0
+- Support build isolation using `setuptools/pyproject.toml` requirement files
+  ([#1727](https://github.com/jazzband/pip-tools/pull/1727)). Thanks @atugushev
+
+Bug Fixes:
+
+- Improve punctuation/grammar with `pip-compile` header
+  ([#1547](https://github.com/jazzband/pip-tools/pull/1547)). Thanks @blueyed
+- Generate hashes for all available candidates
+  ([#1723](https://github.com/jazzband/pip-tools/pull/1723)). Thanks @neykov
+
+Other Changes:
+
+- Bump click minimum version to `>= 8`
+  ([#1733](https://github.com/jazzband/pip-tools/pull/1733)). Thanks @atugushev
+- Bump pip minimum version to `>= 22.2`
+  ([#1729](https://github.com/jazzband/pip-tools/pull/1729)). Thanks @atugushev
+
+## 6.10.0 (2022-11-13)
+
+Features:
+
+- Deprecate `pip-compile --resolver=legacy`
+  ([#1724](https://github.com/jazzband/pip-tools/pull/1724)). Thanks @atugushev
+- Prompt user to use the backtracking resolver on errors
+  ([#1719](https://github.com/jazzband/pip-tools/pull/1719)). Thanks @maxfenv
+- Add support for Python 3.11 final
+  ([#1708](https://github.com/jazzband/pip-tools/pull/1708)). Thanks @hugovk
+- Add `--newline=[LF|CRLF|native|preserve]` option to `pip-compile`
+  ([#1652](https://github.com/jazzband/pip-tools/pull/1652)). Thanks @AndydeCleyre
+
+Bug Fixes:
+
+- Fix inconsistent handling of constraints comments with backtracking resolver
+  ([#1713](https://github.com/jazzband/pip-tools/pull/1713)). Thanks @mkniewallner
+- Fix some encoding warnings in Python 3.10 (PEP 597)
+  ([#1614](https://github.com/jazzband/pip-tools/pull/1614)). Thanks @GalaxySnail
+
+Other Changes:
+
+- Update pip-tools version in the README's pre-commit examples
+  ([#1701](https://github.com/jazzband/pip-tools/pull/1701)). Thanks @Kludex
+- Document use of the backtracking resolver
+  ([#1718](https://github.com/jazzband/pip-tools/pull/1718)). Thanks @maxfenv
+- Use HTTPS in a readme link ([#1716](https://github.com/jazzband/pip-tools/pull/1716)).
+  Thanks @Arhell
+
 ## 6.9.0 (2022-10-05)
 
 Features:
 
 - Add `--all-extras` flag to `pip-compile`
   ([#1630](https://github.com/jazzband/pip-tools/pull/1630)). Thanks @apljungquist
 - Support Exclude Package with custom unsafe packages
```

### Comparing `pip-tools-6.9.0/CODE_OF_CONDUCT.md` & `pip-tools-7.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pip-tools-6.9.0/CONTRIBUTING.md` & `pip-tools-7.0.0/CONTRIBUTING.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 to abide by the [Contributor Code of Conduct](https://jazzband.co/about/conduct)
 and follow the [guidelines](https://jazzband.co/about/guidelines).
 
 ## Project Contribution Guidelines
 
 Here are a few additional or emphasized guidelines to follow when contributing to `pip-tools`:
 
-- If you need to have a virtualenv outside of `tox`, it is possible to reuse its configuration to provision it as [described in the docs](https://tox.readthedocs.io/en/latest/example/devenv.html#creating-development-environments-using-the-devenv-option).
+- If you need to have a virtualenv outside of `tox`, it is possible to reuse its configuration to provision it with [tox devenv](<https://tox.wiki/en/latest/cli_interface.html#tox-devenv-(d)>).
 - Always provide tests for your changes and run `tox -p all` to make sure they are passing the checks locally.
 - Give a clear one-line description in the PR (that the maintainers can add to [CHANGELOG] afterwards).
 - Wait for the review of at least one other contributor before merging (even if you're a Jazzband member).
 - Before merging, assign the PR to a milestone for a version to help with the release process.
 
 The only exception to those guidelines is for trivial changes, such as
 documentation corrections or contributions that do not change pip-tools itself.
@@ -28,18 +28,18 @@
 
 - Check to see if any recently merged PRs are missing from the milestone of the version about to be released.
 - Create a branch for the release. _Ex: release-3.4.0_.
 - Update the [CHANGELOG] with the version, date and add the text from [drafter release](https://github.com/jazzband/pip-tools/releases).
 - Push the branch to your fork and create a pull request.
 - Merge the pull request after the changes being approved.
 - Make sure that the tests/CI still pass.
-- Once ready, go to [releases](https://github.com/jazzband/pip-tools/releases) page and publish the latest draft release. This will push a tag on the HEAD of master, trigger the CI pipeline and
+- Once ready, go to [releases](https://github.com/jazzband/pip-tools/releases) page and publish the latest draft release. This will push a tag on the HEAD of the main branch, trigger the CI pipeline and
   deploy a pip-tools release in the **Jazzband private package index** upon success.
 - The pip-tools "lead" project members will receive an email notification to review the release and
   deploy it to the public PyPI if all is correct.
 - Once the release to the public PyPI is confirmed, close the milestone.
 
 Please be mindful of other before and when performing a release, and use this access responsibly.
 
 Do not hesitate to ask questions if you have any before performing a release.
 
-[changelog]: https://github.com/jazzband/pip-tools/blob/master/CHANGELOG.md
+[changelog]: https://github.com/jazzband/pip-tools/blob/main/CHANGELOG.md
```

### Comparing `pip-tools-6.9.0/LICENSE` & `pip-tools-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pip-tools-6.9.0/PKG-INFO` & `pip-tools-7.0.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,627 +1,612 @@
-Metadata-Version: 2.1
-Name: pip-tools
-Version: 6.9.0
-Summary: pip-tools keeps your pinned dependencies fresh.
-Home-page: https://github.com/jazzband/pip-tools/
-Author: Vincent Driessen
-Author-email: me@nvie.com
-License: BSD 3 Clause
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: System :: Systems Administration
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Provides-Extra: testing
-Provides-Extra: coverage
-License-File: LICENSE
-
-|jazzband| |pypi| |pyversions| |pre-commit| |buildstatus-gha| |codecov|
-
-==================================
-pip-tools = pip-compile + pip-sync
-==================================
-
-A set of command line tools to help you keep your ``pip``-based packages fresh,
-even when you've pinned them.  You do pin them, right? (In building your Python application and its dependencies for production, you want to make sure that your builds are predictable and deterministic.)
-
-.. image:: https://github.com/jazzband/pip-tools/raw/master/img/pip-tools-overview.svg
-   :alt: pip-tools overview for phase II
-
-.. |buildstatus-gha| image:: https://github.com/jazzband/pip-tools/workflows/CI/badge.svg
-   :alt: GitHub Actions build status
-   :target: https://github.com/jazzband/pip-tools/actions?query=workflow%3ACI
-.. |codecov| image:: https://codecov.io/gh/jazzband/pip-tools/branch/master/graph/badge.svg
-   :alt: Coverage
-   :target: https://codecov.io/gh/jazzband/pip-tools
-.. |jazzband| image:: https://jazzband.co/static/img/badge.svg
-   :alt: Jazzband
-   :target: https://jazzband.co/
-.. |pre-commit| image:: https://results.pre-commit.ci/badge/github/jazzband/pip-tools/master.svg
-   :alt: pre-commit.ci status
-   :target: https://results.pre-commit.ci/latest/github/jazzband/pip-tools/master
-.. |pypi| image:: https://img.shields.io/pypi/v/pip-tools.svg
-   :alt: PyPI version
-   :target: https://pypi.org/project/pip-tools/
-.. |pyversions| image:: https://img.shields.io/pypi/pyversions/pip-tools.svg
-   :alt: Supported Python versions
-   :target: https://pypi.org/project/pip-tools/
-.. _You do pin them, right?: http://nvie.com/posts/pin-your-packages/
-
-Installation
-============
-
-Similar to ``pip``, ``pip-tools`` must be installed in each of your project's
-`virtual environments`_:
-
-.. code-block:: bash
-
-    $ source /path/to/venv/bin/activate
-    (venv) $ python -m pip install pip-tools
+[![jazzband-image]][jazzband]
+[![pypi][pypi-image]][pypi]
+[![pyversions][pyversions-image]][pyversions]
+[![pre-commit][pre-commit-image]][pre-commit]
+[![buildstatus-gha][buildstatus-gha-image]][buildstatus-gha]
+[![codecov][codecov-image]][codecov]
+[![Matrix Room Badge]][Matrix Room]
+[![Matrix Space Badge]][Matrix Space]
+[![discord-chat-image]][discord-chat]
+
+# pip-tools = pip-compile + pip-sync
+
+A set of command line tools to help you keep your `pip`-based packages fresh,
+even when you've pinned them. You do pin them, right? (In building your Python application and its dependencies for production, you want to make sure that your builds are predictable and deterministic.)
+
+[![pip-tools overview for phase II][pip-tools-overview]][pip-tools-overview]
+
+## Installation
+
+Similar to `pip`, `pip-tools` must be installed in each of your project's
+[virtual environments](https://packaging.python.org/tutorials/installing-packages/#creating-virtual-environments):
+
+```console
+$ source /path/to/venv/bin/activate
+(venv) $ python -m pip install pip-tools
+```
 
 **Note**: all of the remaining example commands assume you've activated your
 project's virtual environment.
 
-.. _virtual environments: https://packaging.python.org/tutorials/installing-packages/#creating-virtual-environments
+## Example usage for `pip-compile`
 
-Example usage for ``pip-compile``
-=================================
+The `pip-compile` command lets you compile a `requirements.txt` file from
+your dependencies, specified in either `pyproject.toml`, `setup.cfg`,
+`setup.py`, or `requirements.in`.
 
-The ``pip-compile`` command lets you compile a ``requirements.txt`` file from
-your dependencies, specified in either ``pyproject.toml``, ``setup.cfg``,
-``setup.py``, or ``requirements.in``.
+Run it with `pip-compile` or `python -m piptools compile`. If you use
+multiple Python versions, you can also run `py -X.Y -m piptools compile` on
+Windows and `pythonX.Y -m piptools compile` on other systems.
 
-Run it with ``pip-compile`` or ``python -m piptools compile``. If you use
-multiple Python versions, you can also run ``py -X.Y -m piptools compile`` on
-Windows and ``pythonX.Y -m piptools compile`` on other systems.
-
-``pip-compile`` should be run from the same virtual environment as your
+`pip-compile` should be run from the same virtual environment as your
 project so conditional dependencies that require a specific Python version,
 or other environment markers, resolve relative to your project's
 environment.
 
-**Note**: If ``pip-compile`` finds an existing ``requirements.txt`` file that
+**Note**: If `pip-compile` finds an existing `requirements.txt` file that
 fulfils the dependencies then no changes will be made, even if updates are
 available. To compile from scratch, first delete the existing
-``requirements.txt`` file, or see `Updating requirements`_ for alternative
-approaches.
+`requirements.txt` file, or see
+[Updating requirements](#updating-requirements)
+for alternative approaches.
+
+### Requirements from `pyproject.toml`
+
+The `pyproject.toml` file is the
+[latest standard](https://peps.python.org/pep-0621/) for configuring
+packages and applications, and is recommended for new projects. `pip-compile`
+supports both installing your `project.dependencies` as well as your
+`project.optional-dependencies`. Thanks to the fact that this is an
+official standard, you can use `pip-compile` to pin the dependencies
+in projects that use modern standards-adhering packaging tools like
+[Setuptools](https://setuptools.pypa.io), [Hatch](https://hatch.pypa.io/)
+or [flit](https://flit.pypa.io/).
 
-Requirements from ``pyproject.toml``
-------------------------------------
+Suppose you have a 'foobar' Python application that is packaged using `Setuptools`,
+and you want to pin it for production. You can declare the project metadata as:
 
-The ``pyproject.toml`` file is the
-`latest standard <https://peps.python.org/pep-0621/>`_ for configuring
-packages and applications, and is recommended for new projects. ``pip-compile``
-supports both installing your ``project.dependencies`` as well as your
-``project.optional-dependencies``. Thanks to the fact that this is an
-official standard, you can use ``pip-compile`` to pin the dependencies
-in projects that use modern standards-adhering packaging tools like
-`Hatch <https://hatch.pypa.io/>`_ or `flit <https://flit.pypa.io/>`_.
+```toml
+[build-system]
+requires = ["setuptools", "setuptools-scm"]
+build-backend = "setuptools.build_meta"
 
-Suppose you have a Django application that is packaged using ``Hatch``, and you
+[project]
+requires-python = ">=3.9"
+name = "foobar"
+dynamic = ["dependencies", "optional-dependencies"]
+
+[tool.setuptools.dynamic]
+dependencies = { file = ["requirements.in"] }
+optional-dependencies.test = { file = ["requirements-test.txt"] }
+
+```
+
+If you have a Django application that is packaged using `Hatch`, and you
 want to pin it for production. You also want to pin your development tools
-in a separate pin file. You declare ``django`` as a dependency and create an
-optional dependency ``dev`` that includes ``pytest``:
+in a separate pin file. You declare `django` as a dependency and create an
+optional dependency `dev` that includes `pytest`:
 
-.. code-block:: toml
+```toml
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "my-cool-django-app"
+version = "42"
+dependencies = ["django"]
 
-    [build-system]
-    requires = ["hatchling"]
-    build-backend = "hatchling.build"
-
-    [project]
-    name = "my-cool-django-app"
-    version = "42"
-    dependencies = ["django"]
-    
-    [project.optional-dependencies]
-    dev = ["pytest"]
+[project.optional-dependencies]
+dev = ["pytest"]
 
-You can produce your pin files as easily as:
+```
 
-.. code-block:: console
+You can produce your pin files as easily as:
 
-    $ pip-compile -o requirements.txt pyproject.toml
-    #
-    # This file is autogenerated by pip-compile with python 3.10
-    # To update, run:
-    #
-    #    pip-compile --output-file=requirements.txt pyproject.toml
-    #
-
-    asgiref==3.5.2
-       # via django
-    django==4.1
-        # via my-cool-django-app (pyproject.toml)
-    sqlparse==0.4.2
-        # via django
-
-    $ pip-compile --extra dev -o dev-requirements.txt pyproject.toml
-    #  
-    # This file is autogenerated by pip-compile with python 3.10
-    # To update, run:
-    #
-    #    pip-compile --extra=dev --output-file=dev-requirements.txt pyproject.toml
-    #
-
-    asgiref==3.5.2
-        # via django
-    attrs==22.1.0
-        # via pytest
-    django==4.1
-        # via my-cool-django-app (pyproject.toml)
-    iniconfig==1.1.1
-        # via pytest
-    packaging==21.3
-        # via pytest
-    pluggy==1.0.0
-        # via pytest
-    py==1.11.0
-        # via pytest
-    pyparsing==3.0.9
-        # via packaging
-    pytest==7.1.2
-        # via my-cool-django-app (pyproject.toml)
-    sqlparse==0.4.2
-        # via django
-    tomli==2.0.1
-        # via pytest
+```console
+$ pip-compile -o requirements.txt pyproject.toml
+#
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
+#
+#    pip-compile --output-file=requirements.txt pyproject.toml
+#
+asgiref==3.6.0
+    # via django
+django==4.1.7
+    # via my-cool-django-app (pyproject.toml)
+sqlparse==0.4.3
+    # via django
+
+$ pip-compile --extra dev -o dev-requirements.txt pyproject.toml
+#
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
+#
+#    pip-compile --extra=dev --output-file=dev-requirements.txt pyproject.toml
+#
+asgiref==3.6.0
+    # via django
+attrs==22.2.0
+    # via pytest
+django==4.1.7
+    # via my-cool-django-app (pyproject.toml)
+exceptiongroup==1.1.1
+    # via pytest
+iniconfig==2.0.0
+    # via pytest
+packaging==23.0
+    # via pytest
+pluggy==1.0.0
+    # via pytest
+pytest==7.2.2
+    # via my-cool-django-app (pyproject.toml)
+sqlparse==0.4.3
+    # via django
+tomli==2.0.1
+    # via pytest
+```
 
 This is great for both pinning your applications, but also to keep the CI
 of your open-source Python package stable.
 
-Requirements from ``setup.py`` and ``setup.cfg``
-------------------------------------------------
+### Requirements from `setup.py` and `setup.cfg`
 
-``pip-compile`` has also full support for ``setup.py``- and
-``setup.cfg``-based projects that use ``setuptools``.
+`pip-compile` has also full support for `setup.py`- and
+`setup.cfg`-based projects that use `setuptools`.
 
 Just define your dependencies and extras as usual and run
-``pip-compile`` as above.
+`pip-compile` as above.
 
-Requirements from ``requirements.in``
--------------------------------------
+### Requirements from `requirements.in`
 
 You can also use plain text files for your requirements (e.g. if you don't
-want your application to be a package). To use a ``requirements.in`` file to
+want your application to be a package). To use a `requirements.in` file to
 declare the Django dependency:
 
-.. code-block:: ini
+```
+# requirements.in
+django
+```
+
+Now, run `pip-compile requirements.in`:
+
+```console
+$ pip-compile requirements.in
+#
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
+#
+#    pip-compile requirements.in
+#
+asgiref==3.6.0
+    # via django
+django==4.1.7
+    # via -r requirements.in
+sqlparse==0.4.3
+    # via django
+```
 
-    # requirements.in
-    django
-
-Now, run ``pip-compile requirements.in``:
-
-.. code-block:: bash
-
-    $ pip-compile requirements.in
-    #
-    # This file is autogenerated by pip-compile
-    # To update, run:
-    #
-    #    pip-compile requirements.in
-    #
-    asgiref==3.2.3
-        # via django
-    django==3.0.3
-        # via -r requirements.in
-    pytz==2019.3
-        # via django
-    sqlparse==0.3.0
-        # via django
-
-And it will produce your ``requirements.txt``, with all the Django dependencies
+And it will produce your `requirements.txt`, with all the Django dependencies
 (and all underlying dependencies) pinned.
 
-.. _Updating requirements:
+(updating-requirements)=
 
-Updating requirements
----------------------
+### Updating requirements
 
-``pip-compile`` generates a ``requirements.txt`` file using the latest versions
+`pip-compile` generates a `requirements.txt` file using the latest versions
 that fulfil the dependencies you specify in the supported files.
 
-If ``pip-compile`` finds an existing ``requirements.txt`` file that fulfils the
+If `pip-compile` finds an existing `requirements.txt` file that fulfils the
 dependencies then no changes will be made, even if updates are available.
 
-To force ``pip-compile`` to update all packages in an existing
-``requirements.txt``, run ``pip-compile --upgrade``.
+To force `pip-compile` to update all packages in an existing
+`requirements.txt`, run `pip-compile --upgrade`.
 
 To update a specific package to the latest or a specific version use the
-``--upgrade-package`` or ``-P`` flag:
-
-.. code-block:: bash
+`--upgrade-package` or `-P` flag:
 
-    # only update the django package
-    $ pip-compile --upgrade-package django
+```console
+# only update the django package
+$ pip-compile --upgrade-package django
 
-    # update both the django and requests packages
-    $ pip-compile --upgrade-package django --upgrade-package requests
+# update both the django and requests packages
+$ pip-compile --upgrade-package django --upgrade-package requests
 
-    # update the django package to the latest, and requests to v2.0.0
-    $ pip-compile --upgrade-package django --upgrade-package requests==2.0.0
+# update the django package to the latest, and requests to v2.0.0
+$ pip-compile --upgrade-package django --upgrade-package requests==2.0.0
+```
 
-You can combine ``--upgrade`` and ``--upgrade-package`` in one command, to
+You can combine `--upgrade` and `--upgrade-package` in one command, to
 provide constraints on the allowed upgrades. For example to upgrade all
 packages whilst constraining requests to the latest version less than 3.0:
 
-.. code-block:: bash
-
-    $ pip-compile --upgrade --upgrade-package 'requests<3.0'
+```console
+$ pip-compile --upgrade --upgrade-package 'requests<3.0'
+```
+
+### Using hashes
+
+If you would like to use _Hash-Checking Mode_ available in `pip` since
+version 8.0, `pip-compile` offers `--generate-hashes` flag:
+
+```console
+$ pip-compile --generate-hashes requirements.in
+#
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
+#
+#    pip-compile --generate-hashes requirements.in
+#
+asgiref==3.6.0 \
+    --hash=sha256:71e68008da809b957b7ee4b43dbccff33d1b23519fb8344e33f049897077afac \
+    --hash=sha256:9567dfe7bd8d3c8c892227827c41cce860b368104c3431da67a0c5a65a949506
+    # via django
+django==4.1.7 \
+    --hash=sha256:44f714b81c5f190d9d2ddad01a532fe502fa01c4cb8faf1d081f4264ed15dcd8 \
+    --hash=sha256:f2f431e75adc40039ace496ad3b9f17227022e8b11566f4b363da44c7e44761e
+    # via -r requirements.in
+sqlparse==0.4.3 \
+    --hash=sha256:0323c0ec29cd52bceabc1b4d9d579e311f3e4961b98d174201d5622a23b85e34 \
+    --hash=sha256:69ca804846bb114d2ec380e4360a8a340db83f0ccf3afceeb1404df028f57268
+    # via django
+```
 
-Using hashes
-------------
-
-If you would like to use *Hash-Checking Mode* available in ``pip`` since
-version 8.0, ``pip-compile`` offers ``--generate-hashes`` flag:
-
-.. code-block:: bash
-
-    $ pip-compile --generate-hashes requirements.in
-    #
-    # This file is autogenerated by pip-compile
-    # To update, run:
-    #
-    #    pip-compile --generate-hashes requirements.in
-    #
-    asgiref==3.2.3 \
-        --hash=sha256:7e06d934a7718bf3975acbf87780ba678957b87c7adc056f13b6215d610695a0 \
-        --hash=sha256:ea448f92fc35a0ef4b1508f53a04c4670255a3f33d22a81c8fc9c872036adbe5 \
-        # via django
-    django==3.0.3 \
-        --hash=sha256:2f1ba1db8648484dd5c238fb62504777b7ad090c81c5f1fd8d5eb5ec21b5f283 \
-        --hash=sha256:c91c91a7ad6ef67a874a4f76f58ba534f9208412692a840e1d125eb5c279cb0a \
-        # via -r requirements.in
-    pytz==2019.3 \
-        --hash=sha256:1c557d7d0e871de1f5ccd5833f60fb2550652da6be2693c1e02300743d21500d \
-        --hash=sha256:b02c06db6cf09c12dd25137e563b31700d3b80fcc4ad23abb7a315f2789819be \
-        # via django
-    sqlparse==0.3.0 \
-        --hash=sha256:40afe6b8d4b1117e7dff5504d7a8ce07d9a1b15aeeade8a2d10f130a834f8177 \
-        --hash=sha256:7c3dca29c022744e95b547e867cee89f4fce4373f3549ccd8797d8eb52cdb873 \
-        # via django
-
-Output File
------------
+### Output File
 
 To output the pinned requirements in a filename other than
-``requirements.txt``, use ``--output-file``. This might be useful for compiling
+`requirements.txt`, use `--output-file`. This might be useful for compiling
 multiple files, for example with different constraints on django to test a
-library with both versions using `tox <https://tox.readthedocs.io/en/latest/>`__:
+library with both versions using [tox](https://tox.readthedocs.io/en/latest/):
+
+```console
+$ pip-compile --upgrade-package 'django<1.0' --output-file requirements-django0x.txt
+$ pip-compile --upgrade-package 'django<2.0' --output-file requirements-django1x.txt
+```
 
-.. code-block:: bash
+Or to output to standard output, use `--output-file=-`:
 
-    $ pip-compile --upgrade-package 'django<1.0' --output-file requirements-django0x.txt
-    $ pip-compile --upgrade-package 'django<2.0' --output-file requirements-django1x.txt
+```console
+$ pip-compile --output-file=- > requirements.txt
+$ pip-compile - --output-file=- < requirements.in > requirements.txt
+```
 
-Or to output to standard output, use ``--output-file=-``:
+### Forwarding options to `pip`
 
-.. code-block:: bash
+Any valid `pip` flags or arguments may be passed on with `pip-compile`'s
+`--pip-args` option, e.g.
 
-    $ pip-compile --output-file=- > requirements.txt
-    $ pip-compile - --output-file=- < requirements.in > requirements.txt
+```console
+$ pip-compile requirements.in --pip-args "--retries 10 --timeout 30"
+```
 
-Forwarding options to ``pip``
------------------------------
+### Configuration
 
-Any valid ``pip`` flags or arguments may be passed on with ``pip-compile``'s
-``--pip-args`` option, e.g.
+You can define project-level defaults for `pip-compile` and `pip-sync` by
+writing them to a configuration file in the same directory as your requirements
+input files (or the current working directory if piping input from stdin).
+By default, both `pip-compile` and `pip-sync` will look first
+for a `.pip-tools.toml` file and then in your `pyproject.toml`. You can
+also specify an alternate TOML configuration file with the `--config` option.
 
-.. code-block:: bash
+For example, to by default generate `pip` hashes in the resulting
+requirements file output, you can specify in a configuration file
 
-    $ pip-compile requirements.in --pip-args "--retries 10 --timeout 30"
+```toml
+[tool.pip-tools]
+generate-hashes = true
 
-Configuration
--------------
+```
 
-You might be wrapping the ``pip-compile`` command in another script. To avoid
+Options to `pip-compile` and `pip-sync` that may be used more than once
+must be defined as lists in a configuration file, even if they only have one
+value.
+
+You might be wrapping the `pip-compile` command in another script. To avoid
 confusing consumers of your custom script you can override the update command
 generated at the top of requirements files by setting the
-``CUSTOM_COMPILE_COMMAND`` environment variable.
-
-.. code-block:: bash
+`CUSTOM_COMPILE_COMMAND` environment variable.
 
-    $ CUSTOM_COMPILE_COMMAND="./pipcompilewrapper" pip-compile requirements.in
-    #
-    # This file is autogenerated by pip-compile
-    # To update, run:
-    #
-    #    ./pipcompilewrapper
-    #
-    asgiref==3.2.3
-        # via django
-    django==3.0.3
-        # via -r requirements.in
-    pytz==2019.3
-        # via django
-    sqlparse==0.3.0
-        # via django
+```console
+$ CUSTOM_COMPILE_COMMAND="./pipcompilewrapper" pip-compile requirements.in
+#
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
+#
+#    ./pipcompilewrapper
+#
+asgiref==3.6.0
+    # via django
+django==4.1.7
+    # via -r requirements.in
+sqlparse==0.4.3
+    # via django
+```
 
-Workflow for layered requirements
----------------------------------
+### Workflow for layered requirements
 
 If you have different environments that you need to install different but
 compatible packages for, then you can create layered requirements files and use
 one layer to constrain the other.
 
-For example, if you have a Django project where you want the newest ``2.1``
+For example, if you have a Django project where you want the newest `2.1`
 release in production and when developing you want to use the Django debug
-toolbar, then you can create two ``*.in`` files, one for each layer:
+toolbar, then you can create two `*.in` files, one for each layer:
 
-.. code-block:: ini
+```
+# requirements.in
+django<2.2
+```
+
+At the top of the development requirements `dev-requirements.in` you use `-c
+requirements.txt` to constrain the dev requirements to packages already
+selected for production in `requirements.txt`.
+
+```
+# dev-requirements.in
+-c requirements.txt
+django-debug-toolbar<2.2
+```
+
+First, compile `requirements.txt` as usual:
+
+```
+$ pip-compile
+#
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
+#
+#    pip-compile
+#
+django==2.1.15
+    # via -r requirements.in
+pytz==2023.3
+    # via django
+```
 
-    # requirements.in
-    django<2.2
-
-At the top of the development requirements ``dev-requirements.in`` you use ``-c
-requirements.txt`` to constrain the dev requirements to packages already
-selected for production in ``requirements.txt``.
-
-.. code-block:: ini
-
-    # dev-requirements.in
-    -c requirements.txt
-    django-debug-toolbar
-
-First, compile ``requirements.txt`` as usual:
-
-.. code-block:: bash
-
-    $ pip-compile
-    #
-    # This file is autogenerated by pip-compile
-    # To update, run:
-    #
-    #    pip-compile
-    #
-    django==2.1.15
-        # via -r requirements.in
-    pytz==2019.3
-        # via django
-
-
-Now compile the dev requirements and the ``requirements.txt`` file is used as
+Now compile the dev requirements and the `requirements.txt` file is used as
 a constraint:
 
-.. code-block:: bash
-
-    $ pip-compile dev-requirements.in
-    #
-    # This file is autogenerated by pip-compile
-    # To update, run:
-    #
-    #    pip-compile dev-requirements.in
-    #
-    django-debug-toolbar==2.2
-        # via -r dev-requirements.in
-    django==2.1.15
-        # via
-        #   -c requirements.txt
-        #   django-debug-toolbar
-    pytz==2019.3
-        # via
-        #   -c requirements.txt
-        #   django
-    sqlparse==0.3.0
-        # via django-debug-toolbar
+```console
+$ pip-compile dev-requirements.in
+#
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
+#
+#    pip-compile dev-requirements.in
+#
+django==2.1.15
+    # via
+    #   -c requirements.txt
+    #   django-debug-toolbar
+django-debug-toolbar==2.1
+    # via -r dev-requirements.in
+pytz==2023.3
+    # via
+    #   -c requirements.txt
+    #   django
+sqlparse==0.4.3
+    # via django-debug-toolbar
+```
 
-As you can see above, even though a ``2.2`` release of Django is available, the
-dev requirements only include a ``2.1`` version of Django because they were
+As you can see above, even though a `2.2` release of Django is available, the
+dev requirements only include a `2.1` version of Django because they were
 constrained. Now both compiled requirements files can be installed safely in
 the dev environment.
 
 To install requirements in production stage use:
 
-.. code-block:: bash
-
-    $ pip-sync
+```console
+$ pip-sync
+```
 
 You can install requirements in development stage by:
 
-.. code-block:: bash
-
-    $ pip-sync requirements.txt dev-requirements.txt
+```console
+$ pip-sync requirements.txt dev-requirements.txt
+```
+
+### Version control integration
+
+You might use `pip-compile` as a hook for the [pre-commit](https://github.com/pre-commit/pre-commit).
+See [pre-commit docs](https://pre-commit.com/) for instructions.
+Sample `.pre-commit-config.yaml`:
+
+```yaml
+repos:
+  - repo: https://github.com/jazzband/pip-tools
+    rev: 7.0.0
+    hooks:
+      - id: pip-compile
+```
+
+You might want to customize `pip-compile` args by configuring `args` and/or `files`, for example:
+
+```yaml
+repos:
+  - repo: https://github.com/jazzband/pip-tools
+    rev: 7.0.0
+    hooks:
+      - id: pip-compile
+        files: ^requirements/production\.(in|txt)$
+        args: [--index-url=https://example.com, requirements/production.in]
+```
+
+If you have multiple requirement files make sure you create a hook for each file.
+
+```yaml
+repos:
+  - repo: https://github.com/jazzband/pip-tools
+    rev: 7.0.0
+    hooks:
+      - id: pip-compile
+        name: pip-compile setup.py
+        files: ^(setup\.py|requirements\.txt)$
+      - id: pip-compile
+        name: pip-compile requirements-dev.in
+        args: [requirements-dev.in]
+        files: ^requirements-dev\.(in|txt)$
+      - id: pip-compile
+        name: pip-compile requirements-lint.in
+        args: [requirements-lint.in]
+        files: ^requirements-lint\.(in|txt)$
+      - id: pip-compile
+        name: pip-compile requirements.in
+        args: [requirements.in]
+        files: ^requirements\.(in|txt)$
+```
 
+### Example usage for `pip-sync`
 
-Version control integration
----------------------------
-
-You might use ``pip-compile`` as a hook for the `pre-commit <https://github.com/pre-commit/pre-commit>`_.
-See `pre-commit docs <https://pre-commit.com/>`_ for instructions.
-Sample ``.pre-commit-config.yaml``:
-
-.. code-block:: yaml
-
-    repos:
-      - repo: https://github.com/jazzband/pip-tools
-        rev: 6.3.0
-        hooks:
-          - id: pip-compile
-
-You might want to customize ``pip-compile`` args by configuring ``args`` and/or ``files``, for example:
-
-.. code-block:: yaml
-
-    repos:
-      - repo: https://github.com/jazzband/pip-tools
-        rev: 6.3.0
-        hooks:
-          - id: pip-compile
-            files: ^requirements/production\.(in|txt)$
-            args: [--index-url=https://example.com, requirements/production.in]
-
-If you have multiple requirement files make sure you create a hook for each file. 
-
-.. code-block:: yaml 
-
-    repos:
-      - repo: https://github.com/jazzband/pip-tools
-        rev: 5.3.1
-        hooks:
-          - id: pip-compile
-            name: pip-compile setup.py
-            files: ^(setup\.py|requirements\.txt)$
-          - id: pip-compile
-            name: pip-compile requirements-dev.in
-            args: [requirements-dev.in]
-            files: ^requirements-dev\.(in|txt)$
-          - id: pip-compile
-            name: pip-compile requirements-lint.in
-            args: [requirements-lint.in]
-            files: ^requirements-lint\.(in|txt)$
-          - id: pip-compile
-            name: pip-compile requirements.txt
-            args: [requirements.txt]
-            files: ^requirements\.(in|txt)$
-
-
-Example usage for ``pip-sync``
-==============================
-
-Now that you have a ``requirements.txt``, you can use ``pip-sync`` to update
+Now that you have a `requirements.txt`, you can use `pip-sync` to update
 your virtual environment to reflect exactly what's in there. This will
 install/upgrade/uninstall everything necessary to match the
-``requirements.txt`` contents.
+`requirements.txt` contents.
 
-Run it with ``pip-sync`` or ``python -m piptools sync``. If you use multiple
-Python versions, you can also run ``py -X.Y -m piptools sync`` on Windows and
-``pythonX.Y -m piptools sync`` on other systems.
+Run it with `pip-sync` or `python -m piptools sync`. If you use multiple
+Python versions, you can also run `py -X.Y -m piptools sync` on Windows and
+`pythonX.Y -m piptools sync` on other systems.
 
-``pip-sync`` must be installed into and run from the same virtual
+`pip-sync` must be installed into and run from the same virtual
 environment as your project to identify which packages to install
 or upgrade.
 
-**Be careful**: ``pip-sync`` is meant to be used only with a
-``requirements.txt`` generated by ``pip-compile``.
-
-.. code-block:: bash
+**Be careful**: `pip-sync` is meant to be used only with a
+`requirements.txt` generated by `pip-compile`.
 
-    $ pip-sync
-    Uninstalling flake8-2.4.1:
-      Successfully uninstalled flake8-2.4.1
-    Collecting click==4.1
-      Downloading click-4.1-py2.py3-none-any.whl (62kB)
-        100% |................................| 65kB 1.8MB/s
-      Found existing installation: click 4.0
-        Uninstalling click-4.0:
-          Successfully uninstalled click-4.0
-    Successfully installed click-4.1
+```console
+$ pip-sync
+Uninstalling flake8-2.4.1:
+    Successfully uninstalled flake8-2.4.1
+Collecting click==4.1
+    Downloading click-4.1-py2.py3-none-any.whl (62kB)
+    100% |................................| 65kB 1.8MB/s
+    Found existing installation: click 4.0
+    Uninstalling click-4.0:
+        Successfully uninstalled click-4.0
+Successfully installed click-4.1
+```
 
-To sync multiple ``*.txt`` dependency lists, just pass them in via command
+To sync multiple `*.txt` dependency lists, just pass them in via command
 line arguments, e.g.
 
-.. code-block:: bash
-
-    $ pip-sync dev-requirements.txt requirements.txt
+```console
+$ pip-sync dev-requirements.txt requirements.txt
+```
 
-Passing in empty arguments would cause it to default to ``requirements.txt``.
+Passing in empty arguments would cause it to default to `requirements.txt`.
 
-Any valid ``pip install`` flags or arguments may be passed with ``pip-sync``'s
-``--pip-args`` option, e.g.
+Any valid `pip install` flags or arguments may be passed with `pip-sync`'s
+`--pip-args` option, e.g.
 
-.. code-block:: bash
+```console
+$ pip-sync requirements.txt --pip-args "--no-cache-dir --no-deps"
+```
 
-    $ pip-sync requirements.txt --pip-args "--no-cache-dir --no-deps"
-
-**Note**: ``pip-sync`` will not upgrade or uninstall packaging tools like
-``setuptools``, ``pip``, or ``pip-tools`` itself. Use ``python -m pip install --upgrade``
+**Note**: `pip-sync` will not upgrade or uninstall packaging tools like
+`setuptools`, `pip`, or `pip-tools` itself. Use `python -m pip install --upgrade`
 to upgrade those packages.
 
-Should I commit ``requirements.in`` and ``requirements.txt`` to source control?
-===============================================================================
+### Should I commit `requirements.in` and `requirements.txt` to source control?
 
 Generally, yes. If you want a reproducible environment installation available from your source control,
-then yes, you should commit both ``requirements.in`` and ``requirements.txt`` to source control.
+then yes, you should commit both `requirements.in` and `requirements.txt` to source control.
 
 Note that if you are deploying on multiple Python environments (read the section below),
 then you must commit a separate output file for each Python environment.
-We suggest to use the ``{env}-requirements.txt`` format
-(ex: ``win32-py3.7-requirements.txt``, ``macos-py3.10-requirements.txt``, etc.).
-
+We suggest to use the `{env}-requirements.txt` format
+(ex: `win32-py3.7-requirements.txt`, `macos-py3.10-requirements.txt`, etc.).
 
-Cross-environment usage of ``requirements.in``/``requirements.txt`` and ``pip-compile``
-=======================================================================================
+### Cross-environment usage of `requirements.in`/`requirements.txt` and `pip-compile`
 
 The dependencies of a package can change depending on the Python environment in which it
-is installed.  Here, we define a Python environment as the combination of Operating
+is installed. Here, we define a Python environment as the combination of Operating
 System, Python version (3.7, 3.8, etc.), and Python implementation (CPython, PyPy,
-etc.). For an exact definition, refer to the possible combinations of `PEP 508
-environment markers`_.
+etc.). For an exact definition, refer to the possible combinations of [PEP 508
+environment markers][environment-markers].
 
-As the resulting ``requirements.txt`` can differ for each environment, users must
-execute ``pip-compile`` **on each Python environment separately** to generate a
-``requirements.txt`` valid for each said environment.  The same ``requirements.in`` can
-be used as the source file for all environments, using `PEP 508 environment markers`_ as
-needed, the same way it would be done for regular ``pip`` cross-environment usage.
+As the resulting `requirements.txt` can differ for each environment, users must
+execute `pip-compile` **on each Python environment separately** to generate a
+`requirements.txt` valid for each said environment. The same `requirements.in` can
+be used as the source file for all environments, using
+[PEP 508 environment markers][environment-markers] as
+needed, the same way it would be done for regular `pip` cross-environment usage.
 
-If the generated ``requirements.txt`` remains exactly the same for all Python
+If the generated `requirements.txt` remains exactly the same for all Python
 environments, then it can be used across Python environments safely. **But** users
-should be careful as any package update can introduce environment-dependant
-dependencies, making any newly generated ``requirements.txt`` environment-dependant too.
-As a general rule, it's advised that users should still always execute ``pip-compile``
+should be careful as any package update can introduce environment-dependent
+dependencies, making any newly generated `requirements.txt` environment-dependent too.
+As a general rule, it's advised that users should still always execute `pip-compile`
 on each targeted Python environment to avoid issues.
 
-.. _PEP 508 environment markers: https://www.python.org/dev/peps/pep-0508/#environment-markers
-
-Other useful tools
-==================
-
-- `pipdeptree`_ to print the dependency tree of the installed packages.
-- ``requirements.in``/``requirements.txt`` syntax highlighting:
-
-  * `requirements.txt.vim`_ for Vim.
-  * `Python extension for VS Code`_ for VS Code.
-  * `pip-requirements.el`_ for Emacs.
+### Other useful tools
 
-.. _pipdeptree: https://github.com/naiquevin/pipdeptree
-.. _requirements.txt.vim: https://github.com/raimon49/requirements.txt.vim
-.. _Python extension for VS Code: https://marketplace.visualstudio.com/items?itemName=ms-python.python
-.. _pip-requirements.el: https://github.com/Wilfred/pip-requirements.el
+- [pipdeptree](https://github.com/tox-dev/pipdeptree) to print the dependency tree of the installed packages.
+- `requirements.in`/`requirements.txt` syntax highlighting:
 
+  - [requirements.txt.vim](https://github.com/raimon49/requirements.txt.vim) for Vim.
+  - [Python extension for VS Code](https://marketplace.visualstudio.com/items?itemName=ms-python.python) for VS Code.
+  - [pip-requirements.el](https://github.com/Wilfred/pip-requirements.el) for Emacs.
 
-Deprecations
-============
+### Deprecations
 
-This section lists ``pip-tools`` features that are currently deprecated.
+This section lists `pip-tools` features that are currently deprecated.
 
-- In future versions, the ``--allow-unsafe`` behavior will be enabled by
-  default. Use ``--no-allow-unsafe`` to keep the old behavior. It is
-  recommended to pass the ``--allow-unsafe`` now to adapt to the upcoming
+- In future versions, the `--allow-unsafe` behavior will be enabled by
+  default. Use `--no-allow-unsafe` to keep the old behavior. It is
+  recommended to pass the `--allow-unsafe` now to adapt to the upcoming
   change.
+- Legacy resolver is deprecated and will be removed in future versions.
+  Use `--resolver=backtracking` instead.
 
-Versions and compatibility
-==========================
+### A Note on Resolvers
 
-The table below summarizes the latest ``pip-tools`` versions with the required
-``pip`` and Python versions. Generally, ``pip-tools`` supports the same Python
-versions as the required ``pip`` versions.
-
-+---------------+----------------+----------------+
-| pip-tools     | pip            | Python         |
-+===============+================+================+
-| 4.5.*         | 8.1.3 - 20.0.2 | 2.7, 3.5 - 3.8 |
-+---------------+----------------+----------------+
-| 5.0.0 - 5.3.0 | 20.0 - 20.1.1  | 2.7, 3.5 - 3.8 |
-+---------------+----------------+----------------+
-| 5.4.0         | 20.1 - 20.3.*  | 2.7, 3.5 - 3.8 |
-+---------------+----------------+----------------+
-| 5.5.0         | 20.1 - 20.3.*  | 2.7, 3.5 - 3.9 |
-+---------------+----------------+----------------+
-| 6.0.0 - 6.3.1 | 20.3 - 21.2.*  | 3.6 - 3.9      |
-+---------------+----------------+----------------+
-| 6.4.0         | 21.2 - 21.3.*  | 3.6 - 3.10     |
-+---------------+----------------+----------------+
-| 6.5.0+        | 21.2+          | 3.7 - 3.10     |
-+---------------+----------------+----------------+
+You can choose from either the legacy or the backtracking resolver.
+The backtracking resolver is recommended, and will become the default
+with the 7.0 release.
+
+Use it now with the `--resolver=backtracking` option to `pip-compile`.
+
+The legacy resolver will occasionally fail to resolve dependencies. The
+backtracking resolver is more robust, but can take longer to run in
+general.
+
+You can continue using the legacy resolver with `--resolver=legacy`.
+
+### Versions and compatibility
+
+The table below summarizes the latest `pip-tools` versions with the required
+`pip` and Python versions. Generally, `pip-tools` supports the same Python
+versions as the required `pip` versions.
+
+| pip-tools      | pip            | Python         |
+| -------------- | -------------- | -------------- |
+| 4.5.\*         | 8.1.3 - 20.0.2 | 2.7, 3.5 - 3.8 |
+| 5.0.0 - 5.3.0  | 20.0 - 20.1.1  | 2.7, 3.5 - 3.8 |
+| 5.4.0          | 20.1 - 20.3.\* | 2.7, 3.5 - 3.8 |
+| 5.5.0          | 20.1 - 20.3.\* | 2.7, 3.5 - 3.9 |
+| 6.0.0 - 6.3.1  | 20.3 - 21.2.\* | 3.6 - 3.9      |
+| 6.4.0          | 21.2 - 21.3.\* | 3.6 - 3.10     |
+| 6.5.0 - 6.10.0 | 21.2 - 22.3.\* | 3.7 - 3.11     |
+| 6.11.0+        | 22.2+          | 3.7 - 3.11     |
+
+[jazzband]: https://jazzband.co/
+[jazzband-image]: https://jazzband.co/static/img/badge.svg
+[pypi]: https://pypi.org/project/pip-tools/
+[pypi-image]: https://img.shields.io/pypi/v/pip-tools.svg
+[pyversions]: https://pypi.org/project/pip-tools/
+[pyversions-image]: https://img.shields.io/pypi/pyversions/pip-tools.svg
+[pre-commit]: https://results.pre-commit.ci/latest/github/jazzband/pip-tools/main
+[pre-commit-image]: https://results.pre-commit.ci/badge/github/jazzband/pip-tools/main.svg
+[buildstatus-gha]: https://github.com/jazzband/pip-tools/actions?query=workflow%3ACI
+[buildstatus-gha-image]: https://github.com/jazzband/pip-tools/workflows/CI/badge.svg
+[codecov]: https://codecov.io/gh/jazzband/pip-tools
+[codecov-image]: https://codecov.io/gh/jazzband/pip-tools/branch/main/graph/badge.svg
+[Matrix Room Badge]: https://img.shields.io/matrix/pip-tools:matrix.org?label=Discuss%20on%20Matrix%20at%20%23pip-tools%3Amatrix.org&logo=matrix&server_fqdn=matrix.org&style=flat
+[Matrix Room]: https://matrix.to/#/%23pip-tools:matrix.org
+[Matrix Space Badge]: https://img.shields.io/matrix/jazzband:matrix.org?label=Discuss%20on%20Matrix%20at%20%23jazzband%3Amatrix.org&logo=matrix&server_fqdn=matrix.org&style=flat
+[Matrix Space]: https://matrix.to/#/%23jazzband:matrix.org
+[pip-tools-overview]: https://github.com/jazzband/pip-tools/raw/main/img/pip-tools-overview.svg
+[environment-markers]: https://peps.python.org/pep-0508/#environment-markers
+[discord-chat]: https://discord.gg/pypa
+[discord-chat-image]: https://img.shields.io/discord/803025117553754132?label=Discord%20chat%20%23pip-tools&style=flat-square
```

### Comparing `pip-tools-6.9.0/README.rst` & `pip-tools-7.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,598 +1,649 @@
-|jazzband| |pypi| |pyversions| |pre-commit| |buildstatus-gha| |codecov|
-
-==================================
-pip-tools = pip-compile + pip-sync
-==================================
-
-A set of command line tools to help you keep your ``pip``-based packages fresh,
-even when you've pinned them.  You do pin them, right? (In building your Python application and its dependencies for production, you want to make sure that your builds are predictable and deterministic.)
-
-.. image:: https://github.com/jazzband/pip-tools/raw/master/img/pip-tools-overview.svg
-   :alt: pip-tools overview for phase II
-
-.. |buildstatus-gha| image:: https://github.com/jazzband/pip-tools/workflows/CI/badge.svg
-   :alt: GitHub Actions build status
-   :target: https://github.com/jazzband/pip-tools/actions?query=workflow%3ACI
-.. |codecov| image:: https://codecov.io/gh/jazzband/pip-tools/branch/master/graph/badge.svg
-   :alt: Coverage
-   :target: https://codecov.io/gh/jazzband/pip-tools
-.. |jazzband| image:: https://jazzband.co/static/img/badge.svg
-   :alt: Jazzband
-   :target: https://jazzband.co/
-.. |pre-commit| image:: https://results.pre-commit.ci/badge/github/jazzband/pip-tools/master.svg
-   :alt: pre-commit.ci status
-   :target: https://results.pre-commit.ci/latest/github/jazzband/pip-tools/master
-.. |pypi| image:: https://img.shields.io/pypi/v/pip-tools.svg
-   :alt: PyPI version
-   :target: https://pypi.org/project/pip-tools/
-.. |pyversions| image:: https://img.shields.io/pypi/pyversions/pip-tools.svg
-   :alt: Supported Python versions
-   :target: https://pypi.org/project/pip-tools/
-.. _You do pin them, right?: http://nvie.com/posts/pin-your-packages/
-
-Installation
-============
-
-Similar to ``pip``, ``pip-tools`` must be installed in each of your project's
-`virtual environments`_:
-
-.. code-block:: bash
-
-    $ source /path/to/venv/bin/activate
-    (venv) $ python -m pip install pip-tools
+Metadata-Version: 2.1
+Name: pip-tools
+Version: 7.0.0
+Summary: pip-tools keeps your pinned dependencies fresh.
+Author-email: Vincent Driessen <me@nvie.com>
+License: BSD
+Project-URL: homepage, https://github.com/jazzband/pip-tools/
+Project-URL: documentation, https://pip-tools.readthedocs.io/en/latest/
+Project-URL: repository, https://github.com/jazzband/pip-tools
+Project-URL: changelog, https://github.com/jazzband/pip-tools/releases
+Keywords: pip,requirements,packaging
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+Provides-Extra: coverage
+License-File: LICENSE
+
+[![jazzband-image]][jazzband]
+[![pypi][pypi-image]][pypi]
+[![pyversions][pyversions-image]][pyversions]
+[![pre-commit][pre-commit-image]][pre-commit]
+[![buildstatus-gha][buildstatus-gha-image]][buildstatus-gha]
+[![codecov][codecov-image]][codecov]
+[![Matrix Room Badge]][Matrix Room]
+[![Matrix Space Badge]][Matrix Space]
+[![discord-chat-image]][discord-chat]
+
+# pip-tools = pip-compile + pip-sync
+
+A set of command line tools to help you keep your `pip`-based packages fresh,
+even when you've pinned them. You do pin them, right? (In building your Python application and its dependencies for production, you want to make sure that your builds are predictable and deterministic.)
+
+[![pip-tools overview for phase II][pip-tools-overview]][pip-tools-overview]
+
+## Installation
+
+Similar to `pip`, `pip-tools` must be installed in each of your project's
+[virtual environments](https://packaging.python.org/tutorials/installing-packages/#creating-virtual-environments):
+
+```console
+$ source /path/to/venv/bin/activate
+(venv) $ python -m pip install pip-tools
+```
 
 **Note**: all of the remaining example commands assume you've activated your
 project's virtual environment.
 
-.. _virtual environments: https://packaging.python.org/tutorials/installing-packages/#creating-virtual-environments
-
-Example usage for ``pip-compile``
-=================================
+## Example usage for `pip-compile`
 
-The ``pip-compile`` command lets you compile a ``requirements.txt`` file from
-your dependencies, specified in either ``pyproject.toml``, ``setup.cfg``,
-``setup.py``, or ``requirements.in``.
+The `pip-compile` command lets you compile a `requirements.txt` file from
+your dependencies, specified in either `pyproject.toml`, `setup.cfg`,
+`setup.py`, or `requirements.in`.
 
-Run it with ``pip-compile`` or ``python -m piptools compile``. If you use
-multiple Python versions, you can also run ``py -X.Y -m piptools compile`` on
-Windows and ``pythonX.Y -m piptools compile`` on other systems.
+Run it with `pip-compile` or `python -m piptools compile`. If you use
+multiple Python versions, you can also run `py -X.Y -m piptools compile` on
+Windows and `pythonX.Y -m piptools compile` on other systems.
 
-``pip-compile`` should be run from the same virtual environment as your
+`pip-compile` should be run from the same virtual environment as your
 project so conditional dependencies that require a specific Python version,
 or other environment markers, resolve relative to your project's
 environment.
 
-**Note**: If ``pip-compile`` finds an existing ``requirements.txt`` file that
+**Note**: If `pip-compile` finds an existing `requirements.txt` file that
 fulfils the dependencies then no changes will be made, even if updates are
 available. To compile from scratch, first delete the existing
-``requirements.txt`` file, or see `Updating requirements`_ for alternative
-approaches.
+`requirements.txt` file, or see
+[Updating requirements](#updating-requirements)
+for alternative approaches.
+
+### Requirements from `pyproject.toml`
+
+The `pyproject.toml` file is the
+[latest standard](https://peps.python.org/pep-0621/) for configuring
+packages and applications, and is recommended for new projects. `pip-compile`
+supports both installing your `project.dependencies` as well as your
+`project.optional-dependencies`. Thanks to the fact that this is an
+official standard, you can use `pip-compile` to pin the dependencies
+in projects that use modern standards-adhering packaging tools like
+[Setuptools](https://setuptools.pypa.io), [Hatch](https://hatch.pypa.io/)
+or [flit](https://flit.pypa.io/).
 
-Requirements from ``pyproject.toml``
-------------------------------------
+Suppose you have a 'foobar' Python application that is packaged using `Setuptools`,
+and you want to pin it for production. You can declare the project metadata as:
 
-The ``pyproject.toml`` file is the
-`latest standard <https://peps.python.org/pep-0621/>`_ for configuring
-packages and applications, and is recommended for new projects. ``pip-compile``
-supports both installing your ``project.dependencies`` as well as your
-``project.optional-dependencies``. Thanks to the fact that this is an
-official standard, you can use ``pip-compile`` to pin the dependencies
-in projects that use modern standards-adhering packaging tools like
-`Hatch <https://hatch.pypa.io/>`_ or `flit <https://flit.pypa.io/>`_.
+```toml
+[build-system]
+requires = ["setuptools", "setuptools-scm"]
+build-backend = "setuptools.build_meta"
+
+[project]
+requires-python = ">=3.9"
+name = "foobar"
+dynamic = ["dependencies", "optional-dependencies"]
+
+[tool.setuptools.dynamic]
+dependencies = { file = ["requirements.in"] }
+optional-dependencies.test = { file = ["requirements-test.txt"] }
 
-Suppose you have a Django application that is packaged using ``Hatch``, and you
+```
+
+If you have a Django application that is packaged using `Hatch`, and you
 want to pin it for production. You also want to pin your development tools
-in a separate pin file. You declare ``django`` as a dependency and create an
-optional dependency ``dev`` that includes ``pytest``:
+in a separate pin file. You declare `django` as a dependency and create an
+optional dependency `dev` that includes `pytest`:
 
-.. code-block:: toml
+```toml
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "my-cool-django-app"
+version = "42"
+dependencies = ["django"]
 
-    [build-system]
-    requires = ["hatchling"]
-    build-backend = "hatchling.build"
-
-    [project]
-    name = "my-cool-django-app"
-    version = "42"
-    dependencies = ["django"]
-    
-    [project.optional-dependencies]
-    dev = ["pytest"]
+[project.optional-dependencies]
+dev = ["pytest"]
 
-You can produce your pin files as easily as:
+```
 
-.. code-block:: console
+You can produce your pin files as easily as:
 
-    $ pip-compile -o requirements.txt pyproject.toml
-    #
-    # This file is autogenerated by pip-compile with python 3.10
-    # To update, run:
-    #
-    #    pip-compile --output-file=requirements.txt pyproject.toml
-    #
-
-    asgiref==3.5.2
-       # via django
-    django==4.1
-        # via my-cool-django-app (pyproject.toml)
-    sqlparse==0.4.2
-        # via django
-
-    $ pip-compile --extra dev -o dev-requirements.txt pyproject.toml
-    #  
-    # This file is autogenerated by pip-compile with python 3.10
-    # To update, run:
-    #
-    #    pip-compile --extra=dev --output-file=dev-requirements.txt pyproject.toml
-    #
-
-    asgiref==3.5.2
-        # via django
-    attrs==22.1.0
-        # via pytest
-    django==4.1
-        # via my-cool-django-app (pyproject.toml)
-    iniconfig==1.1.1
-        # via pytest
-    packaging==21.3
-        # via pytest
-    pluggy==1.0.0
-        # via pytest
-    py==1.11.0
-        # via pytest
-    pyparsing==3.0.9
-        # via packaging
-    pytest==7.1.2
-        # via my-cool-django-app (pyproject.toml)
-    sqlparse==0.4.2
-        # via django
-    tomli==2.0.1
-        # via pytest
+```console
+$ pip-compile -o requirements.txt pyproject.toml
+#
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
+#
+#    pip-compile --output-file=requirements.txt pyproject.toml
+#
+asgiref==3.6.0
+    # via django
+django==4.1.7
+    # via my-cool-django-app (pyproject.toml)
+sqlparse==0.4.3
+    # via django
+
+$ pip-compile --extra dev -o dev-requirements.txt pyproject.toml
+#
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
+#
+#    pip-compile --extra=dev --output-file=dev-requirements.txt pyproject.toml
+#
+asgiref==3.6.0
+    # via django
+attrs==22.2.0
+    # via pytest
+django==4.1.7
+    # via my-cool-django-app (pyproject.toml)
+exceptiongroup==1.1.1
+    # via pytest
+iniconfig==2.0.0
+    # via pytest
+packaging==23.0
+    # via pytest
+pluggy==1.0.0
+    # via pytest
+pytest==7.2.2
+    # via my-cool-django-app (pyproject.toml)
+sqlparse==0.4.3
+    # via django
+tomli==2.0.1
+    # via pytest
+```
 
 This is great for both pinning your applications, but also to keep the CI
 of your open-source Python package stable.
 
-Requirements from ``setup.py`` and ``setup.cfg``
-------------------------------------------------
+### Requirements from `setup.py` and `setup.cfg`
 
-``pip-compile`` has also full support for ``setup.py``- and
-``setup.cfg``-based projects that use ``setuptools``.
+`pip-compile` has also full support for `setup.py`- and
+`setup.cfg`-based projects that use `setuptools`.
 
 Just define your dependencies and extras as usual and run
-``pip-compile`` as above.
+`pip-compile` as above.
 
-Requirements from ``requirements.in``
--------------------------------------
+### Requirements from `requirements.in`
 
 You can also use plain text files for your requirements (e.g. if you don't
-want your application to be a package). To use a ``requirements.in`` file to
+want your application to be a package). To use a `requirements.in` file to
 declare the Django dependency:
 
-.. code-block:: ini
+```
+# requirements.in
+django
+```
+
+Now, run `pip-compile requirements.in`:
+
+```console
+$ pip-compile requirements.in
+#
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
+#
+#    pip-compile requirements.in
+#
+asgiref==3.6.0
+    # via django
+django==4.1.7
+    # via -r requirements.in
+sqlparse==0.4.3
+    # via django
+```
 
-    # requirements.in
-    django
-
-Now, run ``pip-compile requirements.in``:
-
-.. code-block:: bash
-
-    $ pip-compile requirements.in
-    #
-    # This file is autogenerated by pip-compile
-    # To update, run:
-    #
-    #    pip-compile requirements.in
-    #
-    asgiref==3.2.3
-        # via django
-    django==3.0.3
-        # via -r requirements.in
-    pytz==2019.3
-        # via django
-    sqlparse==0.3.0
-        # via django
-
-And it will produce your ``requirements.txt``, with all the Django dependencies
+And it will produce your `requirements.txt`, with all the Django dependencies
 (and all underlying dependencies) pinned.
 
-.. _Updating requirements:
+(updating-requirements)=
 
-Updating requirements
----------------------
+### Updating requirements
 
-``pip-compile`` generates a ``requirements.txt`` file using the latest versions
+`pip-compile` generates a `requirements.txt` file using the latest versions
 that fulfil the dependencies you specify in the supported files.
 
-If ``pip-compile`` finds an existing ``requirements.txt`` file that fulfils the
+If `pip-compile` finds an existing `requirements.txt` file that fulfils the
 dependencies then no changes will be made, even if updates are available.
 
-To force ``pip-compile`` to update all packages in an existing
-``requirements.txt``, run ``pip-compile --upgrade``.
+To force `pip-compile` to update all packages in an existing
+`requirements.txt`, run `pip-compile --upgrade`.
 
 To update a specific package to the latest or a specific version use the
-``--upgrade-package`` or ``-P`` flag:
-
-.. code-block:: bash
+`--upgrade-package` or `-P` flag:
 
-    # only update the django package
-    $ pip-compile --upgrade-package django
+```console
+# only update the django package
+$ pip-compile --upgrade-package django
 
-    # update both the django and requests packages
-    $ pip-compile --upgrade-package django --upgrade-package requests
+# update both the django and requests packages
+$ pip-compile --upgrade-package django --upgrade-package requests
 
-    # update the django package to the latest, and requests to v2.0.0
-    $ pip-compile --upgrade-package django --upgrade-package requests==2.0.0
+# update the django package to the latest, and requests to v2.0.0
+$ pip-compile --upgrade-package django --upgrade-package requests==2.0.0
+```
 
-You can combine ``--upgrade`` and ``--upgrade-package`` in one command, to
+You can combine `--upgrade` and `--upgrade-package` in one command, to
 provide constraints on the allowed upgrades. For example to upgrade all
 packages whilst constraining requests to the latest version less than 3.0:
 
-.. code-block:: bash
-
-    $ pip-compile --upgrade --upgrade-package 'requests<3.0'
+```console
+$ pip-compile --upgrade --upgrade-package 'requests<3.0'
+```
+
+### Using hashes
+
+If you would like to use _Hash-Checking Mode_ available in `pip` since
+version 8.0, `pip-compile` offers `--generate-hashes` flag:
+
+```console
+$ pip-compile --generate-hashes requirements.in
+#
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
+#
+#    pip-compile --generate-hashes requirements.in
+#
+asgiref==3.6.0 \
+    --hash=sha256:71e68008da809b957b7ee4b43dbccff33d1b23519fb8344e33f049897077afac \
+    --hash=sha256:9567dfe7bd8d3c8c892227827c41cce860b368104c3431da67a0c5a65a949506
+    # via django
+django==4.1.7 \
+    --hash=sha256:44f714b81c5f190d9d2ddad01a532fe502fa01c4cb8faf1d081f4264ed15dcd8 \
+    --hash=sha256:f2f431e75adc40039ace496ad3b9f17227022e8b11566f4b363da44c7e44761e
+    # via -r requirements.in
+sqlparse==0.4.3 \
+    --hash=sha256:0323c0ec29cd52bceabc1b4d9d579e311f3e4961b98d174201d5622a23b85e34 \
+    --hash=sha256:69ca804846bb114d2ec380e4360a8a340db83f0ccf3afceeb1404df028f57268
+    # via django
+```
 
-Using hashes
-------------
-
-If you would like to use *Hash-Checking Mode* available in ``pip`` since
-version 8.0, ``pip-compile`` offers ``--generate-hashes`` flag:
-
-.. code-block:: bash
-
-    $ pip-compile --generate-hashes requirements.in
-    #
-    # This file is autogenerated by pip-compile
-    # To update, run:
-    #
-    #    pip-compile --generate-hashes requirements.in
-    #
-    asgiref==3.2.3 \
-        --hash=sha256:7e06d934a7718bf3975acbf87780ba678957b87c7adc056f13b6215d610695a0 \
-        --hash=sha256:ea448f92fc35a0ef4b1508f53a04c4670255a3f33d22a81c8fc9c872036adbe5 \
-        # via django
-    django==3.0.3 \
-        --hash=sha256:2f1ba1db8648484dd5c238fb62504777b7ad090c81c5f1fd8d5eb5ec21b5f283 \
-        --hash=sha256:c91c91a7ad6ef67a874a4f76f58ba534f9208412692a840e1d125eb5c279cb0a \
-        # via -r requirements.in
-    pytz==2019.3 \
-        --hash=sha256:1c557d7d0e871de1f5ccd5833f60fb2550652da6be2693c1e02300743d21500d \
-        --hash=sha256:b02c06db6cf09c12dd25137e563b31700d3b80fcc4ad23abb7a315f2789819be \
-        # via django
-    sqlparse==0.3.0 \
-        --hash=sha256:40afe6b8d4b1117e7dff5504d7a8ce07d9a1b15aeeade8a2d10f130a834f8177 \
-        --hash=sha256:7c3dca29c022744e95b547e867cee89f4fce4373f3549ccd8797d8eb52cdb873 \
-        # via django
-
-Output File
------------
+### Output File
 
 To output the pinned requirements in a filename other than
-``requirements.txt``, use ``--output-file``. This might be useful for compiling
+`requirements.txt`, use `--output-file`. This might be useful for compiling
 multiple files, for example with different constraints on django to test a
-library with both versions using `tox <https://tox.readthedocs.io/en/latest/>`__:
+library with both versions using [tox](https://tox.readthedocs.io/en/latest/):
+
+```console
+$ pip-compile --upgrade-package 'django<1.0' --output-file requirements-django0x.txt
+$ pip-compile --upgrade-package 'django<2.0' --output-file requirements-django1x.txt
+```
 
-.. code-block:: bash
+Or to output to standard output, use `--output-file=-`:
 
-    $ pip-compile --upgrade-package 'django<1.0' --output-file requirements-django0x.txt
-    $ pip-compile --upgrade-package 'django<2.0' --output-file requirements-django1x.txt
+```console
+$ pip-compile --output-file=- > requirements.txt
+$ pip-compile - --output-file=- < requirements.in > requirements.txt
+```
 
-Or to output to standard output, use ``--output-file=-``:
+### Forwarding options to `pip`
 
-.. code-block:: bash
+Any valid `pip` flags or arguments may be passed on with `pip-compile`'s
+`--pip-args` option, e.g.
 
-    $ pip-compile --output-file=- > requirements.txt
-    $ pip-compile - --output-file=- < requirements.in > requirements.txt
+```console
+$ pip-compile requirements.in --pip-args "--retries 10 --timeout 30"
+```
 
-Forwarding options to ``pip``
------------------------------
+### Configuration
 
-Any valid ``pip`` flags or arguments may be passed on with ``pip-compile``'s
-``--pip-args`` option, e.g.
+You can define project-level defaults for `pip-compile` and `pip-sync` by
+writing them to a configuration file in the same directory as your requirements
+input files (or the current working directory if piping input from stdin).
+By default, both `pip-compile` and `pip-sync` will look first
+for a `.pip-tools.toml` file and then in your `pyproject.toml`. You can
+also specify an alternate TOML configuration file with the `--config` option.
 
-.. code-block:: bash
+For example, to by default generate `pip` hashes in the resulting
+requirements file output, you can specify in a configuration file
 
-    $ pip-compile requirements.in --pip-args "--retries 10 --timeout 30"
+```toml
+[tool.pip-tools]
+generate-hashes = true
 
-Configuration
--------------
+```
 
-You might be wrapping the ``pip-compile`` command in another script. To avoid
+Options to `pip-compile` and `pip-sync` that may be used more than once
+must be defined as lists in a configuration file, even if they only have one
+value.
+
+You might be wrapping the `pip-compile` command in another script. To avoid
 confusing consumers of your custom script you can override the update command
 generated at the top of requirements files by setting the
-``CUSTOM_COMPILE_COMMAND`` environment variable.
-
-.. code-block:: bash
+`CUSTOM_COMPILE_COMMAND` environment variable.
 
-    $ CUSTOM_COMPILE_COMMAND="./pipcompilewrapper" pip-compile requirements.in
-    #
-    # This file is autogenerated by pip-compile
-    # To update, run:
-    #
-    #    ./pipcompilewrapper
-    #
-    asgiref==3.2.3
-        # via django
-    django==3.0.3
-        # via -r requirements.in
-    pytz==2019.3
-        # via django
-    sqlparse==0.3.0
-        # via django
+```console
+$ CUSTOM_COMPILE_COMMAND="./pipcompilewrapper" pip-compile requirements.in
+#
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
+#
+#    ./pipcompilewrapper
+#
+asgiref==3.6.0
+    # via django
+django==4.1.7
+    # via -r requirements.in
+sqlparse==0.4.3
+    # via django
+```
 
-Workflow for layered requirements
----------------------------------
+### Workflow for layered requirements
 
 If you have different environments that you need to install different but
 compatible packages for, then you can create layered requirements files and use
 one layer to constrain the other.
 
-For example, if you have a Django project where you want the newest ``2.1``
+For example, if you have a Django project where you want the newest `2.1`
 release in production and when developing you want to use the Django debug
-toolbar, then you can create two ``*.in`` files, one for each layer:
+toolbar, then you can create two `*.in` files, one for each layer:
 
-.. code-block:: ini
+```
+# requirements.in
+django<2.2
+```
+
+At the top of the development requirements `dev-requirements.in` you use `-c
+requirements.txt` to constrain the dev requirements to packages already
+selected for production in `requirements.txt`.
+
+```
+# dev-requirements.in
+-c requirements.txt
+django-debug-toolbar<2.2
+```
+
+First, compile `requirements.txt` as usual:
+
+```
+$ pip-compile
+#
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
+#
+#    pip-compile
+#
+django==2.1.15
+    # via -r requirements.in
+pytz==2023.3
+    # via django
+```
 
-    # requirements.in
-    django<2.2
-
-At the top of the development requirements ``dev-requirements.in`` you use ``-c
-requirements.txt`` to constrain the dev requirements to packages already
-selected for production in ``requirements.txt``.
-
-.. code-block:: ini
-
-    # dev-requirements.in
-    -c requirements.txt
-    django-debug-toolbar
-
-First, compile ``requirements.txt`` as usual:
-
-.. code-block:: bash
-
-    $ pip-compile
-    #
-    # This file is autogenerated by pip-compile
-    # To update, run:
-    #
-    #    pip-compile
-    #
-    django==2.1.15
-        # via -r requirements.in
-    pytz==2019.3
-        # via django
-
-
-Now compile the dev requirements and the ``requirements.txt`` file is used as
+Now compile the dev requirements and the `requirements.txt` file is used as
 a constraint:
 
-.. code-block:: bash
-
-    $ pip-compile dev-requirements.in
-    #
-    # This file is autogenerated by pip-compile
-    # To update, run:
-    #
-    #    pip-compile dev-requirements.in
-    #
-    django-debug-toolbar==2.2
-        # via -r dev-requirements.in
-    django==2.1.15
-        # via
-        #   -c requirements.txt
-        #   django-debug-toolbar
-    pytz==2019.3
-        # via
-        #   -c requirements.txt
-        #   django
-    sqlparse==0.3.0
-        # via django-debug-toolbar
+```console
+$ pip-compile dev-requirements.in
+#
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
+#
+#    pip-compile dev-requirements.in
+#
+django==2.1.15
+    # via
+    #   -c requirements.txt
+    #   django-debug-toolbar
+django-debug-toolbar==2.1
+    # via -r dev-requirements.in
+pytz==2023.3
+    # via
+    #   -c requirements.txt
+    #   django
+sqlparse==0.4.3
+    # via django-debug-toolbar
+```
 
-As you can see above, even though a ``2.2`` release of Django is available, the
-dev requirements only include a ``2.1`` version of Django because they were
+As you can see above, even though a `2.2` release of Django is available, the
+dev requirements only include a `2.1` version of Django because they were
 constrained. Now both compiled requirements files can be installed safely in
 the dev environment.
 
 To install requirements in production stage use:
 
-.. code-block:: bash
-
-    $ pip-sync
+```console
+$ pip-sync
+```
 
 You can install requirements in development stage by:
 
-.. code-block:: bash
-
-    $ pip-sync requirements.txt dev-requirements.txt
+```console
+$ pip-sync requirements.txt dev-requirements.txt
+```
+
+### Version control integration
+
+You might use `pip-compile` as a hook for the [pre-commit](https://github.com/pre-commit/pre-commit).
+See [pre-commit docs](https://pre-commit.com/) for instructions.
+Sample `.pre-commit-config.yaml`:
+
+```yaml
+repos:
+  - repo: https://github.com/jazzband/pip-tools
+    rev: 7.0.0
+    hooks:
+      - id: pip-compile
+```
+
+You might want to customize `pip-compile` args by configuring `args` and/or `files`, for example:
+
+```yaml
+repos:
+  - repo: https://github.com/jazzband/pip-tools
+    rev: 7.0.0
+    hooks:
+      - id: pip-compile
+        files: ^requirements/production\.(in|txt)$
+        args: [--index-url=https://example.com, requirements/production.in]
+```
+
+If you have multiple requirement files make sure you create a hook for each file.
+
+```yaml
+repos:
+  - repo: https://github.com/jazzband/pip-tools
+    rev: 7.0.0
+    hooks:
+      - id: pip-compile
+        name: pip-compile setup.py
+        files: ^(setup\.py|requirements\.txt)$
+      - id: pip-compile
+        name: pip-compile requirements-dev.in
+        args: [requirements-dev.in]
+        files: ^requirements-dev\.(in|txt)$
+      - id: pip-compile
+        name: pip-compile requirements-lint.in
+        args: [requirements-lint.in]
+        files: ^requirements-lint\.(in|txt)$
+      - id: pip-compile
+        name: pip-compile requirements.in
+        args: [requirements.in]
+        files: ^requirements\.(in|txt)$
+```
 
+### Example usage for `pip-sync`
 
-Version control integration
----------------------------
-
-You might use ``pip-compile`` as a hook for the `pre-commit <https://github.com/pre-commit/pre-commit>`_.
-See `pre-commit docs <https://pre-commit.com/>`_ for instructions.
-Sample ``.pre-commit-config.yaml``:
-
-.. code-block:: yaml
-
-    repos:
-      - repo: https://github.com/jazzband/pip-tools
-        rev: 6.3.0
-        hooks:
-          - id: pip-compile
-
-You might want to customize ``pip-compile`` args by configuring ``args`` and/or ``files``, for example:
-
-.. code-block:: yaml
-
-    repos:
-      - repo: https://github.com/jazzband/pip-tools
-        rev: 6.3.0
-        hooks:
-          - id: pip-compile
-            files: ^requirements/production\.(in|txt)$
-            args: [--index-url=https://example.com, requirements/production.in]
-
-If you have multiple requirement files make sure you create a hook for each file. 
-
-.. code-block:: yaml 
-
-    repos:
-      - repo: https://github.com/jazzband/pip-tools
-        rev: 5.3.1
-        hooks:
-          - id: pip-compile
-            name: pip-compile setup.py
-            files: ^(setup\.py|requirements\.txt)$
-          - id: pip-compile
-            name: pip-compile requirements-dev.in
-            args: [requirements-dev.in]
-            files: ^requirements-dev\.(in|txt)$
-          - id: pip-compile
-            name: pip-compile requirements-lint.in
-            args: [requirements-lint.in]
-            files: ^requirements-lint\.(in|txt)$
-          - id: pip-compile
-            name: pip-compile requirements.txt
-            args: [requirements.txt]
-            files: ^requirements\.(in|txt)$
-
-
-Example usage for ``pip-sync``
-==============================
-
-Now that you have a ``requirements.txt``, you can use ``pip-sync`` to update
+Now that you have a `requirements.txt`, you can use `pip-sync` to update
 your virtual environment to reflect exactly what's in there. This will
 install/upgrade/uninstall everything necessary to match the
-``requirements.txt`` contents.
+`requirements.txt` contents.
 
-Run it with ``pip-sync`` or ``python -m piptools sync``. If you use multiple
-Python versions, you can also run ``py -X.Y -m piptools sync`` on Windows and
-``pythonX.Y -m piptools sync`` on other systems.
+Run it with `pip-sync` or `python -m piptools sync`. If you use multiple
+Python versions, you can also run `py -X.Y -m piptools sync` on Windows and
+`pythonX.Y -m piptools sync` on other systems.
 
-``pip-sync`` must be installed into and run from the same virtual
+`pip-sync` must be installed into and run from the same virtual
 environment as your project to identify which packages to install
 or upgrade.
 
-**Be careful**: ``pip-sync`` is meant to be used only with a
-``requirements.txt`` generated by ``pip-compile``.
-
-.. code-block:: bash
+**Be careful**: `pip-sync` is meant to be used only with a
+`requirements.txt` generated by `pip-compile`.
 
-    $ pip-sync
-    Uninstalling flake8-2.4.1:
-      Successfully uninstalled flake8-2.4.1
-    Collecting click==4.1
-      Downloading click-4.1-py2.py3-none-any.whl (62kB)
-        100% |................................| 65kB 1.8MB/s
-      Found existing installation: click 4.0
-        Uninstalling click-4.0:
-          Successfully uninstalled click-4.0
-    Successfully installed click-4.1
+```console
+$ pip-sync
+Uninstalling flake8-2.4.1:
+    Successfully uninstalled flake8-2.4.1
+Collecting click==4.1
+    Downloading click-4.1-py2.py3-none-any.whl (62kB)
+    100% |................................| 65kB 1.8MB/s
+    Found existing installation: click 4.0
+    Uninstalling click-4.0:
+        Successfully uninstalled click-4.0
+Successfully installed click-4.1
+```
 
-To sync multiple ``*.txt`` dependency lists, just pass them in via command
+To sync multiple `*.txt` dependency lists, just pass them in via command
 line arguments, e.g.
 
-.. code-block:: bash
-
-    $ pip-sync dev-requirements.txt requirements.txt
+```console
+$ pip-sync dev-requirements.txt requirements.txt
+```
 
-Passing in empty arguments would cause it to default to ``requirements.txt``.
+Passing in empty arguments would cause it to default to `requirements.txt`.
 
-Any valid ``pip install`` flags or arguments may be passed with ``pip-sync``'s
-``--pip-args`` option, e.g.
+Any valid `pip install` flags or arguments may be passed with `pip-sync`'s
+`--pip-args` option, e.g.
 
-.. code-block:: bash
+```console
+$ pip-sync requirements.txt --pip-args "--no-cache-dir --no-deps"
+```
 
-    $ pip-sync requirements.txt --pip-args "--no-cache-dir --no-deps"
-
-**Note**: ``pip-sync`` will not upgrade or uninstall packaging tools like
-``setuptools``, ``pip``, or ``pip-tools`` itself. Use ``python -m pip install --upgrade``
+**Note**: `pip-sync` will not upgrade or uninstall packaging tools like
+`setuptools`, `pip`, or `pip-tools` itself. Use `python -m pip install --upgrade`
 to upgrade those packages.
 
-Should I commit ``requirements.in`` and ``requirements.txt`` to source control?
-===============================================================================
+### Should I commit `requirements.in` and `requirements.txt` to source control?
 
 Generally, yes. If you want a reproducible environment installation available from your source control,
-then yes, you should commit both ``requirements.in`` and ``requirements.txt`` to source control.
+then yes, you should commit both `requirements.in` and `requirements.txt` to source control.
 
 Note that if you are deploying on multiple Python environments (read the section below),
 then you must commit a separate output file for each Python environment.
-We suggest to use the ``{env}-requirements.txt`` format
-(ex: ``win32-py3.7-requirements.txt``, ``macos-py3.10-requirements.txt``, etc.).
-
+We suggest to use the `{env}-requirements.txt` format
+(ex: `win32-py3.7-requirements.txt`, `macos-py3.10-requirements.txt`, etc.).
 
-Cross-environment usage of ``requirements.in``/``requirements.txt`` and ``pip-compile``
-=======================================================================================
+### Cross-environment usage of `requirements.in`/`requirements.txt` and `pip-compile`
 
 The dependencies of a package can change depending on the Python environment in which it
-is installed.  Here, we define a Python environment as the combination of Operating
+is installed. Here, we define a Python environment as the combination of Operating
 System, Python version (3.7, 3.8, etc.), and Python implementation (CPython, PyPy,
-etc.). For an exact definition, refer to the possible combinations of `PEP 508
-environment markers`_.
+etc.). For an exact definition, refer to the possible combinations of [PEP 508
+environment markers][environment-markers].
 
-As the resulting ``requirements.txt`` can differ for each environment, users must
-execute ``pip-compile`` **on each Python environment separately** to generate a
-``requirements.txt`` valid for each said environment.  The same ``requirements.in`` can
-be used as the source file for all environments, using `PEP 508 environment markers`_ as
-needed, the same way it would be done for regular ``pip`` cross-environment usage.
+As the resulting `requirements.txt` can differ for each environment, users must
+execute `pip-compile` **on each Python environment separately** to generate a
+`requirements.txt` valid for each said environment. The same `requirements.in` can
+be used as the source file for all environments, using
+[PEP 508 environment markers][environment-markers] as
+needed, the same way it would be done for regular `pip` cross-environment usage.
 
-If the generated ``requirements.txt`` remains exactly the same for all Python
+If the generated `requirements.txt` remains exactly the same for all Python
 environments, then it can be used across Python environments safely. **But** users
-should be careful as any package update can introduce environment-dependant
-dependencies, making any newly generated ``requirements.txt`` environment-dependant too.
-As a general rule, it's advised that users should still always execute ``pip-compile``
+should be careful as any package update can introduce environment-dependent
+dependencies, making any newly generated `requirements.txt` environment-dependent too.
+As a general rule, it's advised that users should still always execute `pip-compile`
 on each targeted Python environment to avoid issues.
 
-.. _PEP 508 environment markers: https://www.python.org/dev/peps/pep-0508/#environment-markers
-
-Other useful tools
-==================
-
-- `pipdeptree`_ to print the dependency tree of the installed packages.
-- ``requirements.in``/``requirements.txt`` syntax highlighting:
-
-  * `requirements.txt.vim`_ for Vim.
-  * `Python extension for VS Code`_ for VS Code.
-  * `pip-requirements.el`_ for Emacs.
+### Other useful tools
 
-.. _pipdeptree: https://github.com/naiquevin/pipdeptree
-.. _requirements.txt.vim: https://github.com/raimon49/requirements.txt.vim
-.. _Python extension for VS Code: https://marketplace.visualstudio.com/items?itemName=ms-python.python
-.. _pip-requirements.el: https://github.com/Wilfred/pip-requirements.el
+- [pipdeptree](https://github.com/tox-dev/pipdeptree) to print the dependency tree of the installed packages.
+- `requirements.in`/`requirements.txt` syntax highlighting:
 
+  - [requirements.txt.vim](https://github.com/raimon49/requirements.txt.vim) for Vim.
+  - [Python extension for VS Code](https://marketplace.visualstudio.com/items?itemName=ms-python.python) for VS Code.
+  - [pip-requirements.el](https://github.com/Wilfred/pip-requirements.el) for Emacs.
 
-Deprecations
-============
+### Deprecations
 
-This section lists ``pip-tools`` features that are currently deprecated.
+This section lists `pip-tools` features that are currently deprecated.
 
-- In future versions, the ``--allow-unsafe`` behavior will be enabled by
-  default. Use ``--no-allow-unsafe`` to keep the old behavior. It is
-  recommended to pass the ``--allow-unsafe`` now to adapt to the upcoming
+- In future versions, the `--allow-unsafe` behavior will be enabled by
+  default. Use `--no-allow-unsafe` to keep the old behavior. It is
+  recommended to pass the `--allow-unsafe` now to adapt to the upcoming
   change.
+- Legacy resolver is deprecated and will be removed in future versions.
+  Use `--resolver=backtracking` instead.
 
-Versions and compatibility
-==========================
+### A Note on Resolvers
 
-The table below summarizes the latest ``pip-tools`` versions with the required
-``pip`` and Python versions. Generally, ``pip-tools`` supports the same Python
-versions as the required ``pip`` versions.
-
-+---------------+----------------+----------------+
-| pip-tools     | pip            | Python         |
-+===============+================+================+
-| 4.5.*         | 8.1.3 - 20.0.2 | 2.7, 3.5 - 3.8 |
-+---------------+----------------+----------------+
-| 5.0.0 - 5.3.0 | 20.0 - 20.1.1  | 2.7, 3.5 - 3.8 |
-+---------------+----------------+----------------+
-| 5.4.0         | 20.1 - 20.3.*  | 2.7, 3.5 - 3.8 |
-+---------------+----------------+----------------+
-| 5.5.0         | 20.1 - 20.3.*  | 2.7, 3.5 - 3.9 |
-+---------------+----------------+----------------+
-| 6.0.0 - 6.3.1 | 20.3 - 21.2.*  | 3.6 - 3.9      |
-+---------------+----------------+----------------+
-| 6.4.0         | 21.2 - 21.3.*  | 3.6 - 3.10     |
-+---------------+----------------+----------------+
-| 6.5.0+        | 21.2+          | 3.7 - 3.10     |
-+---------------+----------------+----------------+
+You can choose from either the legacy or the backtracking resolver.
+The backtracking resolver is recommended, and will become the default
+with the 7.0 release.
+
+Use it now with the `--resolver=backtracking` option to `pip-compile`.
+
+The legacy resolver will occasionally fail to resolve dependencies. The
+backtracking resolver is more robust, but can take longer to run in
+general.
+
+You can continue using the legacy resolver with `--resolver=legacy`.
+
+### Versions and compatibility
+
+The table below summarizes the latest `pip-tools` versions with the required
+`pip` and Python versions. Generally, `pip-tools` supports the same Python
+versions as the required `pip` versions.
+
+| pip-tools      | pip            | Python         |
+| -------------- | -------------- | -------------- |
+| 4.5.\*         | 8.1.3 - 20.0.2 | 2.7, 3.5 - 3.8 |
+| 5.0.0 - 5.3.0  | 20.0 - 20.1.1  | 2.7, 3.5 - 3.8 |
+| 5.4.0          | 20.1 - 20.3.\* | 2.7, 3.5 - 3.8 |
+| 5.5.0          | 20.1 - 20.3.\* | 2.7, 3.5 - 3.9 |
+| 6.0.0 - 6.3.1  | 20.3 - 21.2.\* | 3.6 - 3.9      |
+| 6.4.0          | 21.2 - 21.3.\* | 3.6 - 3.10     |
+| 6.5.0 - 6.10.0 | 21.2 - 22.3.\* | 3.7 - 3.11     |
+| 6.11.0+        | 22.2+          | 3.7 - 3.11     |
+
+[jazzband]: https://jazzband.co/
+[jazzband-image]: https://jazzband.co/static/img/badge.svg
+[pypi]: https://pypi.org/project/pip-tools/
+[pypi-image]: https://img.shields.io/pypi/v/pip-tools.svg
+[pyversions]: https://pypi.org/project/pip-tools/
+[pyversions-image]: https://img.shields.io/pypi/pyversions/pip-tools.svg
+[pre-commit]: https://results.pre-commit.ci/latest/github/jazzband/pip-tools/main
+[pre-commit-image]: https://results.pre-commit.ci/badge/github/jazzband/pip-tools/main.svg
+[buildstatus-gha]: https://github.com/jazzband/pip-tools/actions?query=workflow%3ACI
+[buildstatus-gha-image]: https://github.com/jazzband/pip-tools/workflows/CI/badge.svg
+[codecov]: https://codecov.io/gh/jazzband/pip-tools
+[codecov-image]: https://codecov.io/gh/jazzband/pip-tools/branch/main/graph/badge.svg
+[Matrix Room Badge]: https://img.shields.io/matrix/pip-tools:matrix.org?label=Discuss%20on%20Matrix%20at%20%23pip-tools%3Amatrix.org&logo=matrix&server_fqdn=matrix.org&style=flat
+[Matrix Room]: https://matrix.to/#/%23pip-tools:matrix.org
+[Matrix Space Badge]: https://img.shields.io/matrix/jazzband:matrix.org?label=Discuss%20on%20Matrix%20at%20%23jazzband%3Amatrix.org&logo=matrix&server_fqdn=matrix.org&style=flat
+[Matrix Space]: https://matrix.to/#/%23jazzband:matrix.org
+[pip-tools-overview]: https://github.com/jazzband/pip-tools/raw/main/img/pip-tools-overview.svg
+[environment-markers]: https://peps.python.org/pep-0508/#environment-markers
+[discord-chat]: https://discord.gg/pypa
+[discord-chat-image]: https://img.shields.io/discord/803025117553754132?label=Discord%20chat%20%23pip-tools&style=flat-square
```

### Comparing `pip-tools-6.9.0/docs/conf.py` & `pip-tools-7.0.0/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 """Configuration file for the Sphinx documentation builder."""
 
+from __future__ import annotations
+
 from functools import partial
 from pathlib import Path
 
 from setuptools_scm import get_version
 
 # -- Path setup --------------------------------------------------------------
 
@@ -16,15 +18,17 @@
 
 project = "pip-tools"
 author = f"{project} Contributors"
 copyright = f"The {author}"
 
 # The short X.Y version
 version = ".".join(
-    get_scm_version(local_scheme="no-local-version",).split(
+    get_scm_version(
+        local_scheme="no-local-version",
+    ).split(
         "."
     )[:3],
 )
 
 # The full version, including alpha/beta/rc tags
 release = get_scm_version()
 
@@ -44,7 +48,13 @@
 #
 html_theme = "furo"
 
 
 # -------------------------------------------------------------------------
 default_role = "any"
 nitpicky = True
+
+linkcheck_ignore = [
+    r"^https://matrix\.to/#",
+]
+
+suppress_warnings = ["myst.xref_missing"]
```

### Comparing `pip-tools-6.9.0/img/pip-tools-overview.svg` & `pip-tools-7.0.0/img/pip-tools-overview.svg`

 * *Files identical despite different names*

### Comparing `pip-tools-6.9.0/pip_tools.egg-info/SOURCES.txt` & `pip-tools-7.0.0/pip_tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 .bandit
 .coveragerc
+.flake8
 .gitignore
 .pre-commit-config.yaml
 .pre-commit-hooks.yaml
 .prettierrc.yaml
-.readthedocs.yml
+.readthedocs.yaml
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
-README.rst
+README.md
 codecov.yml
-setup.cfg
-setup.py
+pyproject.toml
 tox.ini
 .github/PULL_REQUEST_TEMPLATE.md
 .github/release-drafter.yml
 .github/ISSUE_TEMPLATE/bug-report.md
 .github/ISSUE_TEMPLATE/feature-request.md
 .github/workflows/ci.yml
 .github/workflows/cron.yml
-.github/workflows/qa.yml
 .github/workflows/release-drafter.yml
 .github/workflows/release.yml
+.github/workflows/reusable-qa.yml
 docs/.gitignore
 docs/changelog.md
 docs/conf.py
 docs/contributing.md
-docs/index.rst
+docs/index.md
 docs/requirements.txt
 examples/django.in
 examples/flask.in
 examples/hypothesis.in
 examples/protection.in
 examples/sentry.in
 img/pip-tools-overview.svg
 pip_tools.egg-info/PKG-INFO
 pip_tools.egg-info/SOURCES.txt
 pip_tools.egg-info/dependency_links.txt
 pip_tools.egg-info/entry_points.txt
-pip_tools.egg-info/not-zip-safe
 pip_tools.egg-info/requires.txt
 pip_tools.egg-info/top_level.txt
 piptools/__init__.py
 piptools/__main__.py
 piptools/cache.py
 piptools/exceptions.py
 piptools/locations.py
@@ -51,15 +50,14 @@
 piptools/py.typed
 piptools/resolver.py
 piptools/subprocess_utils.py
 piptools/sync.py
 piptools/utils.py
 piptools/writer.py
 piptools/_compat/__init__.py
-piptools/_compat/click.py
 piptools/_compat/pip_compat.py
 piptools/repositories/__init__.py
 piptools/repositories/base.py
 piptools/repositories/local.py
 piptools/repositories/pypi.py
 piptools/scripts/__init__.py
 piptools/scripts/compile.py
```

### Comparing `pip-tools-6.9.0/piptools/cache.py` & `pip-tools-7.0.0/piptools/cache.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from __future__ import annotations
+
 import json
 import os
 import platform
 import sys
-from typing import Dict, Iterable, List, Optional, Set, Tuple, cast
+from typing import Dict, Iterable, List, Tuple, cast
 
 from pip._internal.req import InstallRequirement
 from pip._vendor.packaging.requirements import Requirement
 
 from .exceptions import PipToolsError
 from .utils import as_tuple, key_from_req, lookup_table_from_tuples
 
@@ -37,18 +39,18 @@
             "Inspect, or delete, the following file:",
             f"  {self.path}",
         ]
         return os.linesep.join(lines)
 
 
 def read_cache_file(cache_file_path: str) -> CacheDict:
-    with open(cache_file_path) as cache_file:
+    with open(cache_file_path, encoding="utf-8") as cache_file:
         try:
             doc = json.load(cache_file)
-        except json.JSONDecodeError:
+        except (json.JSONDecodeError, UnicodeDecodeError):
             raise CorruptCacheError(cache_file_path)
 
         # Check version and load the contents
         if doc["__format__"] != 1:
             raise ValueError("Unknown cache file format")
         return cast(CacheDict, doc["dependencies"])
 
@@ -66,15 +68,15 @@
     """
 
     def __init__(self, cache_dir: str):
         os.makedirs(cache_dir, exist_ok=True)
         cache_filename = f"depcache-{_implementation_name()}.json"
 
         self._cache_file = os.path.join(cache_dir, cache_filename)
-        self._cache: Optional[CacheDict] = None
+        self._cache: CacheDict | None = None
 
     @property
     def cache(self) -> CacheDict:
         """
         The dictionary that is the actual in-memory cache.  This property
         lazily loads the cache from disk.
         """
@@ -104,52 +106,52 @@
         else:
             extras_string = f"[{','.join(extras)}]"
         return name, f"{version}{extras_string}"
 
     def write_cache(self) -> None:
         """Writes the cache to disk as JSON."""
         doc = {"__format__": 1, "dependencies": self._cache}
-        with open(self._cache_file, "w") as f:
+        with open(self._cache_file, "w", encoding="utf-8") as f:
             json.dump(doc, f, sort_keys=True)
 
     def clear(self) -> None:
         self._cache = {}
         self.write_cache()
 
     def __contains__(self, ireq: InstallRequirement) -> bool:
         pkgname, pkgversion_and_extras = self.as_cache_key(ireq)
         return pkgversion_and_extras in self.cache.get(pkgname, {})
 
-    def __getitem__(self, ireq: InstallRequirement) -> List[str]:
+    def __getitem__(self, ireq: InstallRequirement) -> list[str]:
         pkgname, pkgversion_and_extras = self.as_cache_key(ireq)
         return self.cache[pkgname][pkgversion_and_extras]
 
-    def __setitem__(self, ireq: InstallRequirement, values: List[str]) -> None:
+    def __setitem__(self, ireq: InstallRequirement, values: list[str]) -> None:
         pkgname, pkgversion_and_extras = self.as_cache_key(ireq)
         self.cache.setdefault(pkgname, {})
         self.cache[pkgname][pkgversion_and_extras] = values
         self.write_cache()
 
     def reverse_dependencies(
         self, ireqs: Iterable[InstallRequirement]
-    ) -> Dict[str, Set[str]]:
+    ) -> dict[str, set[str]]:
         """
         Returns a lookup table of reverse dependencies for all the given ireqs.
 
         Since this is all static, it only works if the dependency cache
         contains the complete data, otherwise you end up with a partial view.
         This is typically no problem if you use this function after the entire
         dependency tree is resolved.
         """
         ireqs_as_cache_values = [self.as_cache_key(ireq) for ireq in ireqs]
         return self._reverse_dependencies(ireqs_as_cache_values)
 
     def _reverse_dependencies(
-        self, cache_keys: Iterable[Tuple[str, str]]
-    ) -> Dict[str, Set[str]]:
+        self, cache_keys: Iterable[tuple[str, str]]
+    ) -> dict[str, set[str]]:
         """
         Returns a lookup table of reverse dependencies for all the given cache keys.
 
         Example input:
 
             [('pep8', '1.5.7'),
              ('flake8', '2.4.0'),
```

### Comparing `pip-tools-6.9.0/piptools/exceptions.py` & `pip-tools-7.0.0/piptools/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Iterable
 
 from pip._internal.index.package_finder import PackageFinder
 from pip._internal.models.candidate import InstallationCandidate
 from pip._internal.req import InstallRequirement
 from pip._internal.utils.misc import redact_auth_from_url
```

### Comparing `pip-tools-6.9.0/piptools/logging.py` & `pip-tools-7.0.0/piptools/logging.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import contextlib
 import logging
 import sys
 from typing import Any, Iterator
 
 import click
 
@@ -10,17 +12,17 @@
 logging.basicConfig()
 
 
 class LogContext:
     stream = sys.stderr
 
     def __init__(self, verbosity: int = 0, indent_width: int = 2):
-        self.verbosity = verbosity
-        self.current_indent = 0
-        self._indent_width = indent_width
+        self.verbosity = self._initial_verbosity = verbosity
+        self.current_indent = self._initial_indent = 0
+        self._indent_width = self._initial_indent_width = indent_width
 
     def log(self, message: str, *args: Any, **kwargs: Any) -> None:
         kwargs.setdefault("err", True)
         prefix = " " * self.current_indent
         click.secho(prefix + message, *args, **kwargs)
 
     def debug(self, message: str, *args: Any, **kwargs: Any) -> None:
@@ -52,9 +54,15 @@
         """
         self._indent()
         try:
             yield
         finally:
             self._dedent()
 
+    def reset(self) -> None:
+        """Reset logger to initial state."""
+        self.verbosity = self._initial_verbosity
+        self.current_indent = self._initial_indent
+        self._indent_width = self._initial_indent_width
+
 
 log = LogContext()
```

### Comparing `pip-tools-6.9.0/piptools/repositories/base.py` & `pip-tools-7.0.0/piptools/repositories/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from __future__ import annotations
+
 import optparse
 from abc import ABCMeta, abstractmethod
 from contextlib import contextmanager
-from typing import Iterator, Optional, Set
+from typing import Iterator
 
 from pip._internal.commands.install import InstallCommand
 from pip._internal.index.package_finder import PackageFinder
 from pip._internal.models.index import PyPI
 from pip._internal.network.session import PipSession
 from pip._internal.req import InstallRequirement
 
@@ -14,31 +16,31 @@
     DEFAULT_INDEX_URL = PyPI.simple_url
 
     def clear_caches(self) -> None:
         """Should clear any caches used by the implementation."""
 
     @abstractmethod
     def find_best_match(
-        self, ireq: InstallRequirement, prereleases: Optional[bool]
+        self, ireq: InstallRequirement, prereleases: bool | None
     ) -> InstallRequirement:
         """
         Returns a pinned InstallRequirement object that indicates the best match
         for the given InstallRequirement according to the external repository.
         """
 
     @abstractmethod
-    def get_dependencies(self, ireq: InstallRequirement) -> Set[InstallRequirement]:
+    def get_dependencies(self, ireq: InstallRequirement) -> set[InstallRequirement]:
         """
         Given a pinned, URL, or editable InstallRequirement, returns a set of
         dependencies (also InstallRequirements, but not necessarily pinned).
         They indicate the secondary dependencies for the given requirement.
         """
 
     @abstractmethod
-    def get_hashes(self, ireq: InstallRequirement) -> Set[str]:
+    def get_hashes(self, ireq: InstallRequirement) -> set[str]:
         """
         Given a pinned InstallRequirement, returns a set of hashes that represent
         all of the files for a given requirement. It is not acceptable for an
         editable or unpinned requirement to be passed to this function.
         """
 
     @abstractmethod
```

### Comparing `pip-tools-6.9.0/piptools/repositories/local.py` & `pip-tools-7.0.0/piptools/repositories/local.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 import optparse
 from contextlib import contextmanager
-from typing import Iterator, Mapping, Optional, Set, cast
+from typing import Iterator, Mapping, cast
 
 from pip._internal.commands.install import InstallCommand
 from pip._internal.index.package_finder import PackageFinder
 from pip._internal.models.candidate import InstallationCandidate
 from pip._internal.network.session import PipSession
 from pip._internal.req import InstallRequirement
 from pip._internal.utils.hashes import FAVORITE_HASH
@@ -67,28 +69,28 @@
         """Return an install command instance."""
         return self.repository.command
 
     def clear_caches(self) -> None:
         self.repository.clear_caches()
 
     def find_best_match(
-        self, ireq: InstallRequirement, prereleases: Optional[bool] = None
+        self, ireq: InstallRequirement, prereleases: bool | None = None
     ) -> InstallationCandidate:
         key = key_from_ireq(ireq)
         existing_pin = self.existing_pins.get(key)
         if existing_pin and ireq_satisfied_by_existing_pin(ireq, existing_pin):
             project, version, _ = as_tuple(existing_pin)
             return make_install_requirement(project, version, ireq)
         else:
             return self.repository.find_best_match(ireq, prereleases)
 
-    def get_dependencies(self, ireq: InstallRequirement) -> Set[InstallRequirement]:
+    def get_dependencies(self, ireq: InstallRequirement) -> set[InstallRequirement]:
         return self.repository.get_dependencies(ireq)
 
-    def get_hashes(self, ireq: InstallRequirement) -> Set[str]:
+    def get_hashes(self, ireq: InstallRequirement) -> set[str]:
         existing_pin = self._reuse_hashes and self.existing_pins.get(
             key_from_ireq(ireq)
         )
         if existing_pin and ireq_satisfied_by_existing_pin(ireq, existing_pin):
             hashes = existing_pin.hash_options
             hexdigests = hashes.get(FAVORITE_HASH)
             if hexdigests:
```

### Comparing `pip-tools-6.9.0/piptools/repositories/pypi.py` & `pip-tools-7.0.0/piptools/repositories/pypi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,40 @@
+from __future__ import annotations
+
 import contextlib
 import hashlib
 import itertools
-import logging
 import optparse
 import os
 from contextlib import contextmanager
 from shutil import rmtree
-from typing import (
-    Any,
-    BinaryIO,
-    ContextManager,
-    Dict,
-    Iterator,
-    List,
-    NamedTuple,
-    Optional,
-    Set,
-)
+from typing import Any, BinaryIO, ContextManager, Iterator, NamedTuple
 
 from click import progressbar
 from pip._internal.cache import WheelCache
 from pip._internal.commands import create_command
 from pip._internal.commands.install import InstallCommand
 from pip._internal.index.package_finder import PackageFinder
 from pip._internal.models.candidate import InstallationCandidate
 from pip._internal.models.index import PackageIndex
 from pip._internal.models.link import Link
 from pip._internal.models.wheel import Wheel
 from pip._internal.network.session import PipSession
+from pip._internal.operations.build.build_tracker import get_build_tracker
 from pip._internal.req import InstallRequirement, RequirementSet
 from pip._internal.utils.hashes import FAVORITE_HASH
 from pip._internal.utils.logging import indent_log, setup_logging
 from pip._internal.utils.misc import normalize_path
 from pip._internal.utils.temp_dir import TempDirectory, global_tempdir_manager
 from pip._internal.utils.urls import path_to_url, url_to_path
 from pip._vendor.packaging.tags import Tag
 from pip._vendor.packaging.version import _BaseVersion
 from pip._vendor.requests import RequestException, Session
 
-from .._compat import PIP_VERSION
-from .._compat.pip_compat import get_build_tracker
+from .._compat import create_wheel_cache
 from ..exceptions import NoCandidateFound
 from ..logging import log
 from ..utils import (
     as_tuple,
     is_pinned_requirement,
     is_url_requirement,
     lookup_table,
@@ -52,28 +43,28 @@
 from .base import BaseRepository
 
 FILE_CHUNK_SIZE = 4096
 
 
 class FileStream(NamedTuple):
     stream: BinaryIO
-    size: Optional[float]
+    size: float | None
 
 
 class PyPIRepository(BaseRepository):
     HASHABLE_PACKAGE_TYPES = {"bdist_wheel", "sdist"}
 
     """
     The PyPIRepository will use the provided Finder instance to lookup
     packages.  Typically, it looks up packages on PyPI (the default implicit
     config), but any other PyPI mirror can be used if index_urls is
     changed/configured on the Finder.
     """
 
-    def __init__(self, pip_args: List[str], cache_dir: str):
+    def __init__(self, pip_args: list[str], cache_dir: str):
         # Use pip's parser for pip.conf management and defaults.
         # General options (find_links, index_url, extra_index_url, trusted_host,
         # and pre) are deferred to pip.
         self._command: InstallCommand = create_command("install")
 
         options, _ = self.command.parse_args(pip_args)
         if options.cache_dir:
@@ -87,26 +78,31 @@
             options=options, session=self.session
         )
 
         # Caches
         # stores project_name => InstallationCandidate mappings for all
         # versions reported by PyPI, so we only have to ask once for each
         # project
-        self._available_candidates_cache: Dict[str, List[InstallationCandidate]] = {}
+        self._available_candidates_cache: dict[str, list[InstallationCandidate]] = {}
 
         # stores InstallRequirement => list(InstallRequirement) mappings
         # of all secondary dependencies for the given requirement, so we
         # only have to go to disk once for each requirement
-        self._dependencies_cache: Dict[InstallRequirement, Set[InstallRequirement]] = {}
+        self._dependencies_cache: dict[InstallRequirement, set[InstallRequirement]] = {}
 
         # Setup file paths
         self._cache_dir = normalize_path(str(cache_dir))
         self._download_dir = os.path.join(self._cache_dir, "pkgs")
 
-        self._setup_logging()
+        # Default pip's logger is noisy, so decrease it's verbosity
+        setup_logging(
+            verbosity=log.verbosity - 1,
+            no_color=self.options.no_color,
+            user_log_file=self.options.log,
+        )
 
     def clear_caches(self) -> None:
         rmtree(self._download_dir, ignore_errors=True)
 
     @property
     def options(self) -> optparse.Values:
         return self._options
@@ -120,22 +116,22 @@
         return self._finder
 
     @property
     def command(self) -> InstallCommand:
         """Return an install command instance."""
         return self._command
 
-    def find_all_candidates(self, req_name: str) -> List[InstallationCandidate]:
+    def find_all_candidates(self, req_name: str) -> list[InstallationCandidate]:
         if req_name not in self._available_candidates_cache:
             candidates = self.finder.find_all_candidates(req_name)
             self._available_candidates_cache[req_name] = candidates
         return self._available_candidates_cache[req_name]
 
     def find_best_match(
-        self, ireq: InstallRequirement, prereleases: Optional[bool] = None
+        self, ireq: InstallRequirement, prereleases: bool | None = None
     ) -> InstallRequirement:
         """
         Returns a pinned InstallRequirement object that indicates the best match
         for the given InstallRequirement according to the external repository.
         """
         if ireq.editable or is_url_requirement(ireq):
             return ireq  # return itself as the best match
@@ -163,42 +159,35 @@
             best_candidate.name,
             best_candidate.version,
             ireq,
         )
 
     def resolve_reqs(
         self,
-        download_dir: Optional[str],
+        download_dir: str | None,
         ireq: InstallRequirement,
         wheel_cache: WheelCache,
-    ) -> Set[InstallationCandidate]:
+    ) -> set[InstallationCandidate]:
         with get_build_tracker() as build_tracker, TempDirectory(
             kind="resolver"
         ) as temp_dir, indent_log():
             preparer_kwargs = {
                 "temp_build_dir": temp_dir,
                 "options": self.options,
                 "session": self.session,
                 "finder": self.finder,
                 "use_user_site": False,
                 "download_dir": download_dir,
+                "build_tracker": build_tracker,
             }
-
-            if PIP_VERSION[:2] <= (22, 0):
-                preparer_kwargs["req_tracker"] = build_tracker
-            else:
-                preparer_kwargs["build_tracker"] = build_tracker
-
             preparer = self.command.make_requirement_preparer(**preparer_kwargs)
 
             reqset = RequirementSet()
             ireq.user_supplied = True
-            if PIP_VERSION[:3] < (22, 1, 1):
-                reqset.add_requirement(ireq)
-            elif getattr(ireq, "name", None):
+            if getattr(ireq, "name", None):
                 reqset.add_named_requirement(ireq)
             else:
                 reqset.add_unnamed_requirement(ireq)
 
             resolver = self.command.make_resolver(
                 preparer=preparer,
                 finder=self.finder,
@@ -214,15 +203,15 @@
             if not ireq.prepared:
                 # If still not prepared, e.g. a constraint, do enough to assign
                 # the ireq a name:
                 resolver._get_dist_for(ireq)
 
         return set(results)
 
-    def get_dependencies(self, ireq: InstallRequirement) -> Set[InstallRequirement]:
+    def get_dependencies(self, ireq: InstallRequirement) -> set[InstallRequirement]:
         """
         Given a pinned, URL, or editable InstallRequirement, returns a set of
         dependencies (also InstallRequirements, but not necessarily pinned).
         They indicate the secondary dependencies for the given requirement.
         """
         if not (
             ireq.editable or is_url_requirement(ireq) or is_pinned_requirement(ireq)
@@ -242,15 +231,18 @@
                 # using git-checkout-index, which gets rid of the .git dir.
                 download_dir = None
             else:
                 download_dir = self._get_download_path(ireq)
                 os.makedirs(download_dir, exist_ok=True)
 
             with global_tempdir_manager():
-                wheel_cache = WheelCache(self._cache_dir, self.options.format_control)
+                wheel_cache = create_wheel_cache(
+                    cache_dir=self._cache_dir,
+                    format_control=self.options.format_control,
+                )
                 self._dependencies_cache[ireq] = self.resolve_reqs(
                     download_dir, ireq, wheel_cache
                 )
 
         return self._dependencies_cache[ireq]
 
     def _get_project(self, ireq: InstallRequirement) -> Any:
@@ -297,15 +289,15 @@
             # (see pypi _get_cache_path_parts, which inspired this)
             return os.path.join(
                 self._download_dir, salt[:2], salt[2:4], salt[4:6], salt[6:]
             )
         else:
             return self._download_dir
 
-    def get_hashes(self, ireq: InstallRequirement) -> Set[str]:
+    def get_hashes(self, ireq: InstallRequirement) -> set[str]:
         """
         Given an InstallRequirement, return a set of hashes that represent all
         of the files for a given requirement. Unhashable requirements return an
         empty set. Unpinned requirements raise a TypeError.
         """
 
         if ireq.link:
@@ -330,67 +322,79 @@
 
         if not is_pinned_requirement(ireq):
             raise TypeError(f"Expected pinned requirement, got {ireq}")
 
         log.debug(ireq.name)
 
         with log.indentation():
-            hashes = self._get_hashes_from_pypi(ireq)
-            if hashes is None:
-                log.debug("Couldn't get hashes from PyPI, fallback to hashing files")
-                return self._get_hashes_from_files(ireq)
+            return self._get_req_hashes(ireq)
 
-        return hashes
+    def _get_req_hashes(self, ireq: InstallRequirement) -> set[str]:
+        """
+        Collects the hashes for all candidates satisfying the given InstallRequirement. Computes
+        the hashes for the candidates that don't have one reported by their index.
+        """
+        matching_candidates = self._get_matching_candidates(ireq)
+        pypi_hashes_by_link = self._get_hashes_from_pypi(ireq)
+        pypi_hashes = {
+            pypi_hashes_by_link[candidate.link.url]
+            for candidate in matching_candidates
+            if candidate.link.url in pypi_hashes_by_link
+        }
+        local_hashes = {
+            self._get_file_hash(candidate.link)
+            for candidate in matching_candidates
+            if candidate.link.url not in pypi_hashes_by_link
+        }
+        return pypi_hashes | local_hashes
 
-    def _get_hashes_from_pypi(self, ireq: InstallRequirement) -> Optional[Set[str]]:
+    def _get_hashes_from_pypi(self, ireq: InstallRequirement) -> dict[str, str]:
         """
-        Return a set of hashes from PyPI JSON API for a given InstallRequirement.
-        Return None if fetching data is failed or missing digests.
+        Builds a mapping from the release URLs to their hashes as reported by the PyPI JSON API
+        for a given InstallRequirement.
         """
         project = self._get_project(ireq)
         if project is None:
-            return None
+            return {}
 
         _, version, _ = as_tuple(ireq)
 
         try:
             release_files = project["releases"][version]
         except KeyError:
             log.debug("Missing release files on PyPI")
-            return None
+            return {}
 
         try:
             hashes = {
-                f"{FAVORITE_HASH}:{file_['digests'][FAVORITE_HASH]}"
+                file_["url"]: f"{FAVORITE_HASH}:{file_['digests'][FAVORITE_HASH]}"
                 for file_ in release_files
                 if file_["packagetype"] in self.HASHABLE_PACKAGE_TYPES
             }
         except KeyError:
             log.debug("Missing digests of release files on PyPI")
-            return None
+            return {}
 
         return hashes
 
-    def _get_hashes_from_files(self, ireq: InstallRequirement) -> Set[str]:
+    def _get_matching_candidates(
+        self, ireq: InstallRequirement
+    ) -> set[InstallationCandidate]:
         """
-        Return a set of hashes for all release files of a given InstallRequirement.
+        Returns all candidates that satisfy the given InstallRequirement.
         """
         # We need to get all of the candidates that match our current version
         # pin, these will represent all of the files that could possibly
         # satisfy this constraint.
         all_candidates = self.find_all_candidates(ireq.name)
         candidates_by_version = lookup_table(all_candidates, key=candidate_version)
         matching_versions = list(
             ireq.specifier.filter(candidate.version for candidate in all_candidates)
         )
-        matching_candidates = candidates_by_version[matching_versions[0]]
-
-        return {
-            self._get_file_hash(candidate.link) for candidate in matching_candidates
-        }
+        return candidates_by_version[matching_versions[0]]
 
     def _get_file_hash(self, link: Link) -> str:
         log.debug(f"Hashing {link.show_url}")
         h = hashlib.new(FAVORITE_HASH)
         with open_local_or_remote_file(link, self.session) as f:
             # Chunks to iterate
             chunks = iter(lambda: f.stream.read(FILE_CHUNK_SIZE), b"")
@@ -423,19 +427,19 @@
         """
         Monkey patches pip.Wheel to allow wheels from all platforms and Python versions.
 
         This also saves the candidate cache and set a new one, or else the results from
         the previous non-patched calls will interfere.
         """
 
-        def _wheel_supported(self: Wheel, tags: List[Tag]) -> bool:
+        def _wheel_supported(self: Wheel, tags: list[Tag]) -> bool:
             # Ignore current platform. Support everything.
             return True
 
-        def _wheel_support_index_min(self: Wheel, tags: List[Tag]) -> int:
+        def _wheel_support_index_min(self: Wheel, tags: list[Tag]) -> int:
             # All wheels are equal priority for sorting.
             return 0
 
         original_wheel_supported = Wheel.supported
         original_support_index_min = Wheel.support_index_min
         original_cache = self._available_candidates_cache
 
@@ -450,50 +454,14 @@
         try:
             yield
         finally:
             Wheel.supported = original_wheel_supported
             Wheel.support_index_min = original_support_index_min
             self._available_candidates_cache = original_cache
 
-    def _setup_logging(self) -> None:
-        """
-        Setup pip's logger. Ensure pip is verbose same as pip-tools and sync
-        pip's log stream with LogContext.stream. This is only necessary for
-        pip<22.0.
-        """
-        # Default pip's logger is noisy, so decrease it's verbosity
-        setup_logging(
-            verbosity=log.verbosity - 1,
-            no_color=self.options.no_color,
-            user_log_file=self.options.log,
-        )
-
-        if PIP_VERSION[0] >= 22:
-            return
-
-        # Sync pip's console handler stream with LogContext.stream
-        logger = logging.getLogger()
-        for handler in logger.handlers:
-            if handler.name == "console":  # pragma: no branch
-                assert isinstance(handler, logging.StreamHandler)
-                handler.stream = log.stream
-                break
-        else:  # pragma: no cover
-            # There is always a console handler. This warning would be a signal that
-            # this block should be removed/revisited, because of pip possibly
-            # refactored-out logging config.
-            log.warning("Couldn't find a 'console' logging handler")
-
-        # This import will fail with pip 22.1, but here we're pip<22.0
-        from pip._internal.cli.progress_bars import BAR_TYPES
-
-        # Sync pip's progress bars stream with LogContext.stream
-        for bar_cls in itertools.chain(*BAR_TYPES.values()):
-            bar_cls.file = log.stream
-
 
 @contextmanager
 def open_local_or_remote_file(link: Link, session: Session) -> Iterator[FileStream]:
     """
     Open local or remote file for reading.
 
     :type link: pip.index.Link
@@ -514,15 +482,15 @@
                 yield FileStream(stream=local_file, size=st.st_size)
     else:
         # Remote URL
         headers = {"Accept-Encoding": "identity"}
         response = session.get(url, headers=headers, stream=True)
 
         # Content length must be int or None
-        content_length: Optional[int]
+        content_length: int | None
         try:
             content_length = int(response.headers["content-length"])
         except (ValueError, KeyError, TypeError):
             content_length = None
 
         try:
             yield FileStream(stream=response.raw, size=content_length)
```

### Comparing `pip-tools-6.9.0/piptools/resolver.py` & `pip-tools-7.0.0/piptools/resolver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,37 @@
+from __future__ import annotations
+
 import collections
 import copy
 from abc import ABCMeta, abstractmethod
 from functools import partial
 from itertools import chain, count, groupby
-from typing import (
-    Any,
-    Container,
-    DefaultDict,
-    Dict,
-    Iterable,
-    Iterator,
-    List,
-    Optional,
-    Set,
-    Tuple,
-)
+from typing import Any, Container, DefaultDict, Iterable, Iterator
 
 import click
-from pip._internal.cache import WheelCache
 from pip._internal.exceptions import DistributionNotFound
+from pip._internal.operations.build.build_tracker import (
+    get_build_tracker,
+    update_env_context_manager,
+)
 from pip._internal.req import InstallRequirement
 from pip._internal.req.constructors import install_req_from_line
 from pip._internal.resolution.resolvelib.base import Candidate
 from pip._internal.resolution.resolvelib.candidates import ExtrasCandidate
 from pip._internal.resolution.resolvelib.resolver import Resolver
 from pip._internal.utils.logging import indent_log
 from pip._internal.utils.temp_dir import TempDirectory, global_tempdir_manager
 from pip._vendor.packaging.specifiers import SpecifierSet
 from pip._vendor.packaging.utils import canonicalize_name
 from pip._vendor.resolvelib.resolvers import ResolutionImpossible, Result
 
 from piptools.cache import DependencyCache
 from piptools.repositories.base import BaseRepository
 
-from ._compat import PIP_VERSION
-from ._compat.pip_compat import get_build_tracker, update_env_context_manager
+from ._compat import create_wheel_cache
 from .exceptions import PipToolsError
 from .logging import log
 from .utils import (
     UNSAFE_PACKAGES,
     as_tuple,
     copy_install_requirement,
     format_requirement,
@@ -88,15 +81,15 @@
 ) -> InstallRequirement:
     """
     Return a single install requirement that reflects a combination of
     all the inputs.
     """
     # We will store the source ireqs in a _source_ireqs attribute;
     # if any of the inputs have this, then use those sources directly.
-    source_ireqs: List[InstallRequirement] = []
+    source_ireqs: list[InstallRequirement] = []
     for ireq in ireqs:
         source_ireqs.extend(getattr(ireq, "_source_ireqs", [ireq]))
 
     # Optimization. Don't bother with combination logic.
     if len(source_ireqs) == 1:
         return source_ireqs[0]
 
@@ -151,36 +144,36 @@
     combined_ireq._source_ireqs = source_ireqs
 
     return combined_ireq
 
 
 class BaseResolver(metaclass=ABCMeta):
     repository: BaseRepository
-    unsafe_constraints: Set[InstallRequirement]
+    unsafe_constraints: set[InstallRequirement]
 
     @abstractmethod
-    def resolve(self, max_rounds: int) -> Set[InstallRequirement]:
+    def resolve(self, max_rounds: int) -> set[InstallRequirement]:
         """
         Find concrete package versions for all the given InstallRequirements
         and their recursive dependencies and return a set of pinned
         ``InstallRequirement``'s.
         """
 
     def resolve_hashes(
-        self, ireqs: Set[InstallRequirement]
-    ) -> Dict[InstallRequirement, Set[str]]:
+        self, ireqs: set[InstallRequirement]
+    ) -> dict[InstallRequirement, set[str]]:
         """Find acceptable hashes for all of the given ``InstallRequirement``s."""
         log.debug("")
         log.debug("Generating hashes:")
         with self.repository.allow_all_wheels(), log.indentation():
             return {ireq: self.repository.get_hashes(ireq) for ireq in ireqs}
 
     def _filter_out_unsafe_constraints(
         self,
-        ireqs: Set[InstallRequirement],
+        ireqs: set[InstallRequirement],
         unsafe_packages: Container[str],
     ) -> None:
         """
         Remove from a given set of ``InstallRequirement``'s unsafe constraints.
         """
         for req in ireqs.copy():
             if req.name in unsafe_packages:
@@ -188,53 +181,53 @@
                 ireqs.remove(req)
 
 
 class LegacyResolver(BaseResolver):
     def __init__(
         self,
         constraints: Iterable[InstallRequirement],
-        existing_constraints: Dict[str, InstallRequirement],
+        existing_constraints: dict[str, InstallRequirement],
         repository: BaseRepository,
         cache: DependencyCache,
-        prereleases: Optional[bool] = False,
+        prereleases: bool | None = False,
         clear_caches: bool = False,
         allow_unsafe: bool = False,
-        unsafe_packages: Optional[Set[str]] = None,
+        unsafe_packages: set[str] | None = None,
     ) -> None:
         """
         This class resolves a given set of constraints (a collection of
         InstallRequirement objects) by consulting the given Repository and the
         DependencyCache.
         """
         self.our_constraints = set(constraints)
-        self.their_constraints: Set[InstallRequirement] = set()
+        self.their_constraints: set[InstallRequirement] = set()
         self.repository = repository
         self.dependency_cache = cache
         self.prereleases = prereleases
         self.clear_caches = clear_caches
         self.allow_unsafe = allow_unsafe
-        self.unsafe_constraints: Set[InstallRequirement] = set()
+        self.unsafe_constraints: set[InstallRequirement] = set()
         self.unsafe_packages = unsafe_packages or UNSAFE_PACKAGES
 
         options = self.repository.options
         if "legacy-resolver" not in options.deprecated_features_enabled:
             raise PipToolsError("Legacy resolver deprecated feature must be enabled.")
 
         # Make sure there is no enabled 2020-resolver
         options.features_enabled = omit_list_value(
             options.features_enabled, "2020-resolver"
         )
 
     @property
-    def constraints(self) -> Set[InstallRequirement]:
+    def constraints(self) -> set[InstallRequirement]:
         return set(
             self._group_constraints(chain(self.our_constraints, self.their_constraints))
         )
 
-    def resolve(self, max_rounds: int = 10) -> Set[InstallRequirement]:
+    def resolve(self, max_rounds: int = 10) -> set[InstallRequirement]:
         """
         Find concrete package versions for all the given InstallRequirements
         and their recursive dependencies and return a set of pinned
         ``InstallRequirement``'s.
 
         Resolves constraints one round at a time, until they don't change
         anymore.  Protects against infinite loops by breaking out after a max
@@ -312,15 +305,15 @@
         # ireq will be editable, if one exists.
         for _, ireqs in groupby(
             sorted(constraints, key=(lambda x: (key_from_ireq(x), not x.editable))),
             key=key_from_ireq,
         ):
             yield combine_install_requirements(ireqs)
 
-    def _resolve_one_round(self) -> Tuple[bool, Set[InstallRequirement]]:
+    def _resolve_one_round(self) -> tuple[bool, set[InstallRequirement]]:
         """
         Resolves one level of the current constraints, by finding the best
         match for each package in the repository and adding all requirements
         for those best package versions.  Some of these constraints may be new
         or updated.
 
         Returns whether new constraints appeared in this round.  If no
@@ -340,15 +333,15 @@
         with log.indentation():
             best_matches = {self.get_best_match(ireq) for ireq in constraints}
 
         # Find the new set of secondary dependencies
         log.debug("")
         log.debug("Finding secondary dependencies:")
 
-        their_constraints: List[InstallRequirement] = []
+        their_constraints: list[InstallRequirement] = []
         with log.indentation():
             for best_match in best_matches:
                 their_constraints.extend(self._iter_dependencies(best_match))
         # Grouping constraints to make clean diff between rounds
         theirs = set(self._group_constraints(their_constraints))
 
         # NOTE: We need to compare RequirementSummary objects, since
@@ -464,15 +457,15 @@
             self.dependency_cache[ireq] = sorted(str(ireq.req) for ireq in dependencies)
 
         # Example: ['Werkzeug>=0.9', 'Jinja2>=2.4']
         dependency_strings = self.dependency_cache[ireq]
         yield from self._ireqs_of_dependencies(ireq, dependency_strings)
 
     def _ireqs_of_dependencies(
-        self, ireq: InstallRequirement, dependency_strings: List[str]
+        self, ireq: InstallRequirement, dependency_strings: list[str]
     ) -> Iterator[InstallRequirement]:
         log.debug(
             "{:25} requires {}".format(
                 format_requirement(ireq),
                 ", ".join(sorted(dependency_strings, key=lambda s: s.lower())) or "-",
             )
         )
@@ -487,93 +480,102 @@
 
 class BacktrackingResolver(BaseResolver):
     """A wrapper for backtracking resolver."""
 
     def __init__(
         self,
         constraints: Iterable[InstallRequirement],
-        existing_constraints: Dict[str, InstallRequirement],
+        existing_constraints: dict[str, InstallRequirement],
         repository: BaseRepository,
         allow_unsafe: bool = False,
-        unsafe_packages: Optional[Set[str]] = None,
+        unsafe_packages: set[str] | None = None,
         **kwargs: Any,
     ) -> None:
         self.constraints = list(constraints)
         self.repository = repository
         self.allow_unsafe = allow_unsafe
         self.unsafe_packages = unsafe_packages or UNSAFE_PACKAGES
 
         options = self.options = self.repository.options
         self.session = self.repository.session
         self.finder = self.repository.finder
         self.command = self.repository.command
-        self.unsafe_constraints: Set[InstallRequirement] = set()
+        self.unsafe_constraints: set[InstallRequirement] = set()
 
         self.existing_constraints = existing_constraints
-        self._constraints_map = {key_from_ireq(ireq): ireq for ireq in constraints}
+
+        # Categorize InstallRequirements into sets by key
+        constraints_sets: DefaultDict[
+            str, set[InstallRequirement]
+        ] = collections.defaultdict(set)
+        for ireq in constraints:
+            constraints_sets[key_from_ireq(ireq)].add(ireq)
+        # Collapse each set of InstallRequirements using combine_install_requirements
+        self._constraints_map = {
+            ireq_key: combine_install_requirements(ireqs)
+            for ireq_key, ireqs in constraints_sets.items()
+        }
 
         # Make sure there is no enabled legacy resolver
         options.deprecated_features_enabled = omit_list_value(
             options.deprecated_features_enabled, "legacy-resolver"
         )
 
-    def resolve(self, max_rounds: int = 10) -> Set[InstallRequirement]:
+    def resolve(self, max_rounds: int = 10) -> set[InstallRequirement]:
         """
         Find concrete package versions for all the given InstallRequirements
         and their recursive dependencies and return a set of pinned
         ``InstallRequirement``'s.
         """
         with update_env_context_manager(
             PIP_EXISTS_ACTION="i"
         ), get_build_tracker() as build_tracker, global_tempdir_manager(), indent_log():
             # Mark direct/primary/user_supplied packages
             for ireq in self.constraints:
+                if ireq.constraint:
+                    ireq.extras = set()  # pip does not support extras in constraints
                 ireq.user_supplied = True
 
             # Pass compiled requirements from `requirements.txt`
             # as constraints to resolver
-            compatible_existing_constraints: Dict[str, InstallRequirement] = {}
+            compatible_existing_constraints: dict[str, InstallRequirement] = {}
             for ireq in self.existing_constraints.values():
                 # Skip if the compiled install requirement conflicts with
                 # the primary install requirement.
                 primary_ireq = self._constraints_map.get(key_from_ireq(ireq))
                 if primary_ireq is not None:
                     _, version, _ = as_tuple(ireq)
                     prereleases = ireq.specifier.prereleases
                     if not primary_ireq.specifier.contains(version, prereleases):
                         continue
 
-                ireq.extras = set()  # pip does not support extras in constraints
+                ireq.extras = set()
                 ireq.constraint = True
                 ireq.user_supplied = False
                 compatible_existing_constraints[key_from_ireq(ireq)] = ireq
 
-            wheel_cache = WheelCache(
-                self.options.cache_dir, self.options.format_control
+            wheel_cache = create_wheel_cache(
+                cache_dir=self.options.cache_dir,
+                format_control=self.options.format_control,
             )
 
             temp_dir = TempDirectory(
                 delete=not self.options.no_clean,
                 kind="resolve",
                 globally_managed=True,
             )
 
             preparer_kwargs = {
                 "temp_build_dir": temp_dir,
                 "options": self.options,
                 "session": self.session,
                 "finder": self.finder,
                 "use_user_site": False,
+                "build_tracker": build_tracker,
             }
-
-            if PIP_VERSION[:2] <= (22, 0):
-                preparer_kwargs["req_tracker"] = build_tracker
-            else:
-                preparer_kwargs["build_tracker"] = build_tracker
-
             preparer = self.command.make_requirement_preparer(**preparer_kwargs)
 
             resolver = self.command.make_resolver(
                 preparer=preparer,
                 finder=self.finder,
                 options=self.options,
                 wheel_cache=wheel_cache,
@@ -620,15 +622,15 @@
             )
 
         return result_ireqs
 
     def _do_resolve(
         self,
         resolver: Resolver,
-        compatible_existing_constraints: Dict[str, InstallRequirement],
+        compatible_existing_constraints: dict[str, InstallRequirement],
     ) -> bool:
         """
         Return true on successful resolution, otherwise remove problematic
         requirements from existing constraints and return false.
         """
         try:
             resolver.resolve(
@@ -667,17 +669,17 @@
 
             return False
 
         return True
 
     def _get_install_requirements(
         self, resolver_result: Result
-    ) -> Set[InstallRequirement]:
+    ) -> set[InstallRequirement]:
         """Return a set of install requirements from resolver results."""
-        result_ireqs: Dict[str, InstallRequirement] = {}
+        result_ireqs: dict[str, InstallRequirement] = {}
 
         # Get reverse requirements from the resolver result graph.
         reverse_dependencies = self._get_reverse_dependencies(resolver_result)
 
         # Transform candidates to install requirements
         resolved_candidates = tuple(resolver_result.mapping.values())
         for candidate in resolved_candidates:
@@ -704,16 +706,16 @@
             ireq.req.extras |= extras_candidate.extras
 
         return set(result_ireqs.values())
 
     @staticmethod
     def _get_reverse_dependencies(
         resolver_result: Result,
-    ) -> Dict[str, Set[str]]:
-        reverse_dependencies: DefaultDict[str, Set[str]] = collections.defaultdict(set)
+    ) -> dict[str, set[str]]:
+        reverse_dependencies: DefaultDict[str, set[str]] = collections.defaultdict(set)
 
         for candidate in resolver_result.mapping.values():
             stripped_name = strip_extras(canonicalize_name(candidate.name))
 
             for parent_name in resolver_result.graph.iter_parents(candidate.name):
                 # Skip root dependency which is always None
                 if parent_name is None:
@@ -726,16 +728,16 @@
                     continue
 
                 reverse_dependencies[stripped_name].add(stripped_parent_name)
 
         return dict(reverse_dependencies)
 
     def _get_install_requirement_from_candidate(
-        self, candidate: Candidate, reverse_dependencies: Dict[str, Set[str]]
-    ) -> Optional[InstallRequirement]:
+        self, candidate: Candidate, reverse_dependencies: dict[str, set[str]]
+    ) -> InstallRequirement | None:
         ireq = candidate.get_install_requirement()
         if ireq is None:
             return None
 
         # Determine a pin operator
         version_pin_operator = "=="
         version_as_str = str(candidate.version)
@@ -764,13 +766,18 @@
             f"{version_pin_operator}{candidate.version}"
         )
 
         # Save reverse dependencies for annotation
         ireq_key = key_from_ireq(ireq)
         pinned_ireq._required_by = reverse_dependencies.get(ireq_key, set())
 
-        # Save source for annotation
-        source_ireq = self._constraints_map.get(ireq_key)
-        if source_ireq is not None and ireq_key not in self.existing_constraints:
-            pinned_ireq._source_ireqs = [source_ireq]
+        # Save sources for annotation
+        constraint_ireq = self._constraints_map.get(ireq_key)
+        if constraint_ireq is not None:
+            if hasattr(constraint_ireq, "_source_ireqs"):
+                # If the constraint is combined (has _source_ireqs), use those
+                pinned_ireq._source_ireqs = constraint_ireq._source_ireqs
+            else:
+                # Otherwise (the constraint is not combined) it is the source
+                pinned_ireq._source_ireqs = [constraint_ireq]
 
         return pinned_ireq
```

### Comparing `pip-tools-6.9.0/piptools/scripts/compile.py` & `pip-tools-7.0.0/piptools/scripts/compile.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,96 @@
+from __future__ import annotations
+
 import itertools
 import os
 import shlex
 import sys
 import tempfile
-from typing import IO, Any, BinaryIO, List, Optional, Tuple, Union, cast
+from pathlib import Path
+from typing import IO, Any, BinaryIO, cast
 
 import click
 from build import BuildBackendException
 from build.util import project_wheel_metadata
 from click.utils import LazyFile, safecall
 from pip._internal.commands import create_command
 from pip._internal.req import InstallRequirement
 from pip._internal.req.constructors import install_req_from_line
 from pip._internal.utils.misc import redact_auth_from_url
 
-from .._compat import IS_CLICK_VER_8_PLUS, parse_requirements
+from .._compat import parse_requirements
 from ..cache import DependencyCache
-from ..exceptions import PipToolsError
-from ..locations import CACHE_DIR
+from ..exceptions import NoCandidateFound, PipToolsError
+from ..locations import CACHE_DIR, CONFIG_FILE_NAME
 from ..logging import log
 from ..repositories import LocalRequirementsRepository, PyPIRepository
 from ..repositories.base import BaseRepository
 from ..resolver import BacktrackingResolver, LegacyResolver
 from ..utils import (
     UNSAFE_PACKAGES,
     dedup,
     drop_extras,
     is_pinned_requirement,
     key_from_ireq,
+    override_defaults_from_config_file,
+    parse_requirements_from_wheel_metadata,
 )
 from ..writer import OutputWriter
 
-DEFAULT_REQUIREMENTS_FILE = "requirements.in"
+DEFAULT_REQUIREMENTS_FILES = (
+    "requirements.in",
+    "setup.py",
+    "pyproject.toml",
+    "setup.cfg",
+)
 DEFAULT_REQUIREMENTS_OUTPUT_FILE = "requirements.txt"
 METADATA_FILENAMES = frozenset({"setup.py", "setup.cfg", "pyproject.toml"})
 
-# TODO: drop click 7 and remove this block, pass directly to version_option
-version_option_kwargs = {"package_name": "pip-tools"} if IS_CLICK_VER_8_PLUS else {}
-
 
 def _get_default_option(option_name: str) -> Any:
     """
     Get default value of the pip's option (including option from pip.conf)
     by a given option name.
     """
     install_command = create_command("install")
     default_values = install_command.parser.get_default_values()
     return getattr(default_values, option_name)
 
 
+def _determine_linesep(
+    strategy: str = "preserve", filenames: tuple[str, ...] = ()
+) -> str:
+    """
+    Determine and return linesep string for OutputWriter to use.
+    Valid strategies: "LF", "CRLF", "native", "preserve"
+    When preserving, files are checked in order for existing newlines.
+    """
+    if strategy == "preserve":
+        for fname in filenames:
+            try:
+                with open(fname, "rb") as existing_file:
+                    existing_text = existing_file.read()
+            except FileNotFoundError:
+                continue
+            if b"\r\n" in existing_text:
+                strategy = "CRLF"
+                break
+            elif b"\n" in existing_text:
+                strategy = "LF"
+                break
+    return {
+        "native": os.linesep,
+        "LF": "\n",
+        "CRLF": "\r\n",
+        "preserve": "\n",
+    }[strategy]
+
+
 @click.command(context_settings={"help_option_names": ("-h", "--help")})
-@click.version_option(**version_option_kwargs)
+@click.version_option(package_name="pip-tools")
 @click.pass_context
 @click.option("-v", "--verbose", count=True, help="Show more output")
 @click.option("-q", "--quiet", count=True, help="Give less output")
 @click.option(
     "-n",
     "--dry-run",
     is_flag=True,
@@ -95,14 +131,19 @@
     "-i",
     "--index-url",
     help="Change index URL (defaults to {index_url})".format(
         index_url=redact_auth_from_url(_get_default_option("index_url"))
     ),
 )
 @click.option(
+    "--no-index",
+    is_flag=True,
+    help="Ignore package index (only looking at --find-links URLs instead).",
+)
+@click.option(
     "--extra-index-url",
     multiple=True,
     help="Add another index URL to search; may be used more than once",
 )
 @click.option("--cert", help="Path to alternate CA bundle.")
 @click.option(
     "--client-cert",
@@ -162,14 +203,20 @@
     type=click.File("w+b", atomic=True, lazy=True),
     help=(
         "Output file name. Required if more than one input file is given. "
         "Will be derived from input file otherwise."
     ),
 )
 @click.option(
+    "--newline",
+    type=click.Choice(("LF", "CRLF", "native", "preserve"), case_sensitive=False),
+    default="preserve",
+    help="Override the newline control characters used",
+)
+@click.option(
     "--allow-unsafe/--no-allow-unsafe",
     is_flag=True,
     default=False,
     help=(
         "Pin packages considered unsafe: {}.\n\n"
         "WARNING: Future versions of pip-tools will enable this behavior by default. "
         "Use --no-allow-unsafe to keep the old behavior. It is recommended to pass the "
@@ -231,15 +278,15 @@
 @click.option(
     "--pip-args", "pip_args_str", help="Arguments to pass directly to the pip command."
 )
 @click.option(
     "--resolver",
     "resolver_name",
     type=click.Choice(("legacy", "backtracking")),
-    default="legacy",
+    default="backtracking",
     envvar="PIP_TOOLS_RESOLVER",
     help="Choose the dependency resolver.",
 )
 @click.option(
     "--emit-index-url/--no-emit-index-url",
     is_flag=True,
     default=True,
@@ -253,68 +300,93 @@
 )
 @click.option(
     "--unsafe-package",
     multiple=True,
     help="Specify a package to consider unsafe; may be used more than once. "
     f"Replaces default unsafe packages: {', '.join(sorted(UNSAFE_PACKAGES))}",
 )
+@click.option(
+    "--config",
+    type=click.Path(
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        readable=True,
+        allow_dash=False,
+        path_type=str,
+    ),
+    help=f"Read configuration from TOML file. By default, looks for a {CONFIG_FILE_NAME} or "
+    "pyproject.toml.",
+    is_eager=True,
+    callback=override_defaults_from_config_file,
+)
+@click.option(
+    "--no-config",
+    is_flag=True,
+    default=False,
+    help="Do not read any config file.",
+    is_eager=True,
+)
 def cli(
     ctx: click.Context,
     verbose: int,
     quiet: int,
     dry_run: bool,
     pre: bool,
     rebuild: bool,
-    extras: Tuple[str, ...],
+    extras: tuple[str, ...],
     all_extras: bool,
-    find_links: Tuple[str, ...],
+    find_links: tuple[str, ...],
     index_url: str,
-    extra_index_url: Tuple[str, ...],
-    cert: Optional[str],
-    client_cert: Optional[str],
-    trusted_host: Tuple[str, ...],
+    no_index: bool,
+    extra_index_url: tuple[str, ...],
+    cert: str | None,
+    client_cert: str | None,
+    trusted_host: tuple[str, ...],
     header: bool,
     emit_trusted_host: bool,
     annotate: bool,
     annotation_style: str,
     upgrade: bool,
-    upgrade_packages: Tuple[str, ...],
-    output_file: Union[LazyFile, IO[Any], None],
+    upgrade_packages: tuple[str, ...],
+    output_file: LazyFile | IO[Any] | None,
+    newline: str,
     allow_unsafe: bool,
     strip_extras: bool,
     generate_hashes: bool,
     reuse_hashes: bool,
-    src_files: Tuple[str, ...],
+    src_files: tuple[str, ...],
     max_rounds: int,
     build_isolation: bool,
     emit_find_links: bool,
     cache_dir: str,
-    pip_args_str: Optional[str],
+    pip_args_str: str | None,
     resolver_name: str,
     emit_index_url: bool,
     emit_options: bool,
-    unsafe_package: Tuple[str, ...],
+    unsafe_package: tuple[str, ...],
+    config: Path | None,
+    no_config: bool,
 ) -> None:
     """
     Compiles requirements.txt from requirements.in, pyproject.toml, setup.cfg,
     or setup.py specs.
     """
     log.verbosity = verbose - quiet
 
     if len(src_files) == 0:
-        if os.path.exists(DEFAULT_REQUIREMENTS_FILE):
-            src_files = (DEFAULT_REQUIREMENTS_FILE,)
-        elif os.path.exists("setup.py"):
-            src_files = ("setup.py",)
+        for file_path in DEFAULT_REQUIREMENTS_FILES:
+            if os.path.exists(file_path):
+                src_files = (file_path,)
+                break
         else:
             raise click.BadParameter(
                 (
-                    "If you do not specify an input file, "
-                    "the default is {} or setup.py"
-                ).format(DEFAULT_REQUIREMENTS_FILE)
+                    "If you do not specify an input file, the default is one of: {}"
+                ).format(", ".join(DEFAULT_REQUIREMENTS_FILES))
             )
 
     if not output_file:
         # An output file must be provided for stdin
         if src_files == ("-",):
             raise click.BadParameter("--output-file is required if input is from stdin")
         # Use default requirements output file if there is a setup.py the source file
@@ -336,83 +408,107 @@
 
         # Close the file at the end of the context execution
         assert output_file is not None
         # only LazyFile has close_intelligently, newer IO[Any] does not
         if isinstance(output_file, LazyFile):  # pragma: no cover
             ctx.call_on_close(safecall(output_file.close_intelligently))
 
+    if output_file.name != "-" and output_file.name in src_files:
+        raise click.BadArgumentUsage(
+            f"input and output filenames must not be matched: {output_file.name}"
+        )
+
+    if config:
+        log.debug(f"Using pip-tools configuration defaults found in '{config !s}'.")
+
+    if resolver_name == "legacy":
+        log.warning(
+            "WARNING: the legacy dependency resolver is deprecated and will be removed"
+            " in future versions of pip-tools."
+        )
+
     ###
     # Setup
     ###
 
     right_args = shlex.split(pip_args_str or "")
     pip_args = []
     for link in find_links:
         pip_args.extend(["-f", link])
     if index_url:
         pip_args.extend(["-i", index_url])
+    if no_index:
+        pip_args.extend(["--no-index"])
     for extra_index in extra_index_url:
         pip_args.extend(["--extra-index-url", extra_index])
     if cert:
         pip_args.extend(["--cert", cert])
     if client_cert:
         pip_args.extend(["--client-cert", client_cert])
     if pre:
         pip_args.extend(["--pre"])
     for host in trusted_host:
         pip_args.extend(["--trusted-host", host])
     if not build_isolation:
         pip_args.append("--no-build-isolation")
     if resolver_name == "legacy":
         pip_args.extend(["--use-deprecated", "legacy-resolver"])
+    if resolver_name == "backtracking" and cache_dir:
+        pip_args.extend(["--cache-dir", cache_dir])
     pip_args.extend(right_args)
 
     repository: BaseRepository
     repository = PyPIRepository(pip_args, cache_dir=cache_dir)
 
     # Parse all constraints coming from --upgrade-package/-P
     upgrade_reqs_gen = (install_req_from_line(pkg) for pkg in upgrade_packages)
     upgrade_install_reqs = {
         key_from_ireq(install_req): install_req for install_req in upgrade_reqs_gen
     }
 
-    existing_pins_to_upgrade = set()
-
-    # Exclude packages from --upgrade-package/-P from the existing
-    # constraints, and separately gather pins to be upgraded
+    # Exclude packages from --upgrade-package/-P from the existing constraints
     existing_pins = {}
 
     # Proxy with a LocalRequirementsRepository if --upgrade is not specified
     # (= default invocation)
-    if not upgrade and os.path.exists(output_file.name):
+    output_file_exists = os.path.exists(output_file.name)
+    if not upgrade and output_file_exists:
+        output_file_is_empty = os.path.getsize(output_file.name) == 0
+        if upgrade_install_reqs and output_file_is_empty:
+            log.warning(
+                f"WARNING: the output file {output_file.name} exists but is empty. "
+                "Pip-tools cannot upgrade only specific packages (using -P/--upgrade-package) "
+                "without an existing pin file to provide constraints. "
+                "This often occurs if you redirect standard output to your output file, "
+                "as any existing content is truncated."
+            )
+
         # Use a temporary repository to ensure outdated(removed) options from
         # existing requirements.txt wouldn't get into the current repository.
         tmp_repository = PyPIRepository(pip_args, cache_dir=cache_dir)
         ireqs = parse_requirements(
             output_file.name,
             finder=tmp_repository.finder,
             session=tmp_repository.session,
             options=tmp_repository.options,
         )
 
         for ireq in filter(is_pinned_requirement, ireqs):
             key = key_from_ireq(ireq)
-            if key in upgrade_install_reqs:
-                existing_pins_to_upgrade.add(key)
-            else:
+            if key not in upgrade_install_reqs:
                 existing_pins[key] = ireq
         repository = LocalRequirementsRepository(
             existing_pins, repository, reuse_hashes=reuse_hashes
         )
 
     ###
     # Parsing/collecting initial requirements
     ###
 
-    constraints: List[InstallRequirement] = []
+    constraints: list[InstallRequirement] = []
     setup_file_found = False
     for src_file in src_files:
         is_setup_file = os.path.basename(src_file) in METADATA_FILENAMES
         if src_file == "-":
             # pip requires filenames and not files. Since we want to support
             # piping from stdin, we need to briefly save the input from stdin
             # to a temporary file and have pip read that.  also used for
@@ -432,27 +528,28 @@
             for req in reqs:
                 req.comes_from = comes_from
             constraints.extend(reqs)
         elif is_setup_file:
             setup_file_found = True
             try:
                 metadata = project_wheel_metadata(
-                    os.path.dirname(os.path.abspath(src_file))
+                    os.path.dirname(os.path.abspath(src_file)),
+                    isolated=build_isolation,
                 )
             except BuildBackendException as e:
                 log.error(str(e))
                 log.error(f"Failed to parse {os.path.abspath(src_file)}")
                 sys.exit(2)
-            comes_from = f"{metadata.get_all('Name')[0]} ({src_file})"
+
             constraints.extend(
-                [
-                    install_req_from_line(req, comes_from=comes_from)
-                    for req in metadata.get_all("Requires-Dist") or []
-                ]
+                parse_requirements_from_wheel_metadata(
+                    metadata=metadata, src_file=src_file
+                )
             )
+
             if all_extras:
                 if extras:
                     msg = "--extra has no effect when used with --all-extras"
                     raise click.BadParameter(msg)
                 extras = tuple(metadata.get_all("Provides-Extra"))
         else:
             constraints.extend(
@@ -460,37 +557,60 @@
                     src_file,
                     finder=repository.finder,
                     session=repository.session,
                     options=repository.options,
                 )
             )
 
+    if upgrade_packages:
+        constraints_file = tempfile.NamedTemporaryFile(mode="wt", delete=False)
+        constraints_file.write("\n".join(upgrade_packages))
+        constraints_file.flush()
+        try:
+            reqs = list(
+                parse_requirements(
+                    constraints_file.name,
+                    finder=repository.finder,
+                    session=repository.session,
+                    options=repository.options,
+                    constraint=True,
+                )
+            )
+        finally:
+            constraints_file.close()
+            os.unlink(constraints_file.name)
+        for req in reqs:
+            req.comes_from = None
+        constraints.extend(reqs)
+
     extras = tuple(itertools.chain.from_iterable(ex.split(",") for ex in extras))
 
     if extras and not setup_file_found:
         msg = "--extra has effect only with setup.py and PEP-517 input formats"
         raise click.BadParameter(msg)
 
     primary_packages = {
         key_from_ireq(ireq) for ireq in constraints if not ireq.constraint
     }
 
-    allowed_upgrades = primary_packages | existing_pins_to_upgrade
     constraints.extend(
-        ireq for key, ireq in upgrade_install_reqs.items() if key in allowed_upgrades
+        ireq for key, ireq in upgrade_install_reqs.items() if key in primary_packages
     )
 
     constraints = [req for req in constraints if req.match_markers(extras)]
     for req in constraints:
         drop_extras(req)
 
-    log.debug("Using indexes:")
-    with log.indentation():
-        for index_url in dedup(repository.finder.index_urls):
-            log.debug(redact_auth_from_url(index_url))
+    if repository.finder.index_urls:
+        log.debug("Using indexes:")
+        with log.indentation():
+            for index_url in dedup(repository.finder.index_urls):
+                log.debug(redact_auth_from_url(index_url))
+    else:
+        log.debug("Ignoring indexes.")
 
     if repository.finder.find_links:
         log.debug("")
         log.debug("Using links:")
         with log.indentation():
             for find_link in dedup(repository.finder.find_links):
                 log.debug(redact_auth_from_url(find_link))
@@ -505,20 +625,34 @@
             cache=DependencyCache(cache_dir),
             clear_caches=rebuild,
             allow_unsafe=allow_unsafe,
             unsafe_packages=set(unsafe_package),
         )
         results = resolver.resolve(max_rounds=max_rounds)
         hashes = resolver.resolve_hashes(results) if generate_hashes else None
+    except NoCandidateFound as e:
+        if resolver_cls == LegacyResolver:  # pragma: no branch
+            log.error(
+                "Using legacy resolver. "
+                "Consider using backtracking resolver with "
+                "`--resolver=backtracking`."
+            )
+
+        log.error(str(e))
+        sys.exit(2)
     except PipToolsError as e:
         log.error(str(e))
         sys.exit(2)
 
     log.debug("")
 
+    linesep = _determine_linesep(
+        strategy=newline, filenames=(output_file.name, *src_files)
+    )
+
     ##
     # Output
     ##
 
     writer = OutputWriter(
         cast(BinaryIO, output_file),
         click_ctx=ctx,
@@ -530,21 +664,23 @@
         annotation_style=annotation_style,
         strip_extras=strip_extras,
         generate_hashes=generate_hashes,
         default_index_url=repository.DEFAULT_INDEX_URL,
         index_urls=repository.finder.index_urls,
         trusted_hosts=repository.finder.trusted_hosts,
         format_control=repository.finder.format_control,
+        linesep=linesep,
         allow_unsafe=allow_unsafe,
         find_links=repository.finder.find_links,
         emit_find_links=emit_find_links,
         emit_options=emit_options,
     )
     writer.write(
         results=results,
+        unsafe_packages=resolver.unsafe_packages,
         unsafe_requirements=resolver.unsafe_constraints,
         markers={
             key_from_ireq(ireq): ireq.markers for ireq in constraints if ireq.markers
         },
         hashes=hashes,
     )
```

### Comparing `pip-tools-6.9.0/piptools/scripts/sync.py` & `pip-tools-7.0.0/piptools/scripts/sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,42 @@
+from __future__ import annotations
+
 import itertools
 import os
 import shlex
 import shutil
 import sys
-from typing import List, Optional, Tuple, cast
+from pathlib import Path
+from typing import cast
 
 import click
 from pip._internal.commands import create_command
 from pip._internal.commands.install import InstallCommand
 from pip._internal.index.package_finder import PackageFinder
 from pip._internal.metadata import get_environment
 
 from .. import sync
-from .._compat import IS_CLICK_VER_8_PLUS, parse_requirements
-from .._compat.pip_compat import Distribution
+from .._compat import Distribution, parse_requirements
 from ..exceptions import PipToolsError
+from ..locations import CONFIG_FILE_NAME
 from ..logging import log
 from ..repositories import PyPIRepository
 from ..utils import (
     flat_map,
     get_pip_version_for_python_executable,
     get_required_pip_specification,
     get_sys_path_for_python_executable,
+    override_defaults_from_config_file,
 )
 
 DEFAULT_REQUIREMENTS_FILE = "requirements.txt"
 
-# TODO: drop click 7 and remove this block, pass directly to version_option
-version_option_kwargs = {"package_name": "pip-tools"} if IS_CLICK_VER_8_PLUS else {}
-
 
 @click.command(context_settings={"help_option_names": ("-h", "--help")})
-@click.version_option(**version_option_kwargs)
+@click.version_option(package_name="pip-tools")
 @click.option(
     "-a",
     "--ask",
     is_flag=True,
     help="Show what would happen, then ask whether to continue",
 )
 @click.option(
@@ -83,31 +84,55 @@
 @click.option(
     "--client-cert",
     help="Path to SSL client certificate, a single file containing "
     "the private key and the certificate in PEM format.",
 )
 @click.argument("src_files", required=False, type=click.Path(exists=True), nargs=-1)
 @click.option("--pip-args", help="Arguments to pass directly to pip install.")
+@click.option(
+    "--config",
+    type=click.Path(
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        readable=True,
+        allow_dash=False,
+        path_type=str,
+    ),
+    help=f"Read configuration from TOML file. By default, looks for a {CONFIG_FILE_NAME} or "
+    "pyproject.toml.",
+    is_eager=True,
+    callback=override_defaults_from_config_file,
+)
+@click.option(
+    "--no-config",
+    is_flag=True,
+    default=False,
+    help="Do not read any config file.",
+    is_eager=True,
+)
 def cli(
     ask: bool,
     dry_run: bool,
     force: bool,
-    find_links: Tuple[str, ...],
-    index_url: Optional[str],
-    extra_index_url: Tuple[str, ...],
-    trusted_host: Tuple[str, ...],
+    find_links: tuple[str, ...],
+    index_url: str | None,
+    extra_index_url: tuple[str, ...],
+    trusted_host: tuple[str, ...],
     no_index: bool,
-    python_executable: Optional[str],
+    python_executable: str | None,
     verbose: int,
     quiet: int,
     user_only: bool,
-    cert: Optional[str],
-    client_cert: Optional[str],
-    src_files: Tuple[str, ...],
-    pip_args: Optional[str],
+    cert: str | None,
+    client_cert: str | None,
+    src_files: tuple[str, ...],
+    pip_args: str | None,
+    config: Path | None,
+    no_config: bool,
 ) -> None:
     """Synchronize virtual environment with requirements.txt."""
     log.verbosity = verbose - quiet
 
     if not src_files:
         if os.path.exists(DEFAULT_REQUIREMENTS_FILE):
             src_files = (DEFAULT_REQUIREMENTS_FILE,)
@@ -124,14 +149,17 @@
         )
         if force:
             log.warning("WARNING: " + msg)
         else:
             log.error("ERROR: " + msg)
             sys.exit(2)
 
+    if config:
+        log.debug(f"Using pip-tools configuration defaults found in '{config !s}'.")
+
     if python_executable:
         _validate_python_executable(python_executable)
 
     install_command = cast(InstallCommand, create_command("install"))
     options, _ = install_command.parse_args([])
     session = install_command._build_session(options)
     finder = install_command._build_package_finder(options=options, session=session)
@@ -206,22 +234,22 @@
         )
         sys.exit(2)
 
 
 def _compose_install_flags(
     finder: PackageFinder,
     no_index: bool,
-    index_url: Optional[str],
-    extra_index_url: Tuple[str, ...],
-    trusted_host: Tuple[str, ...],
-    find_links: Tuple[str, ...],
+    index_url: str | None,
+    extra_index_url: tuple[str, ...],
+    trusted_host: tuple[str, ...],
+    find_links: tuple[str, ...],
     user_only: bool,
-    cert: Optional[str],
-    client_cert: Optional[str],
-) -> List[str]:
+    cert: str | None,
+    client_cert: str | None,
+) -> list[str]:
     """
     Compose install flags with the given finder and CLI options.
     """
     result = []
 
     # Build --index-url/--extra-index-url/--no-index
     if no_index:
@@ -268,18 +296,18 @@
 
     return result
 
 
 def _get_installed_distributions(
     local_only: bool = True,
     user_only: bool = False,
-    paths: Optional[List[str]] = None,
-) -> List[Distribution]:
+    paths: list[str] | None = None,
+) -> list[Distribution]:
     """Return a list of installed Distribution objects."""
 
     env = get_environment(paths)
     dists = env.iter_installed_distributions(
         local_only=local_only,
         user_only=user_only,
         skip=[],
     )
-    return [cast(Distribution, dist)._dist for dist in dists]
+    return [Distribution.from_pip_distribution(dist) for dist in dists]
```

### Comparing `pip-tools-6.9.0/piptools/subprocess_utils.py` & `pip-tools-7.0.0/piptools/subprocess_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # WARNING! BE CAREFUL UPDATING THIS FILE
 # Consider possible security implications associated with subprocess module.
+from __future__ import annotations
+
 import subprocess  # nosec
 
 
 def run_python_snippet(python_executable: str, code_to_run: str) -> str:
     """
     Executes python code by calling python_executable with '-c' option.
     """
```

### Comparing `pip-tools-6.9.0/piptools/sync.py` & `pip-tools-7.0.0/piptools/sync.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,26 @@
+from __future__ import annotations
+
 import collections
 import os
 import sys
 import tempfile
 from subprocess import run  # nosec
-from typing import (
-    Deque,
-    Dict,
-    Iterable,
-    List,
-    Mapping,
-    Optional,
-    Set,
-    Tuple,
-    ValuesView,
-)
+from typing import Deque, Iterable, Mapping, ValuesView
 
 import click
-from pip._internal.commands.freeze import DEV_PKGS
+from pip._internal.models.direct_url import ArchiveInfo
 from pip._internal.req import InstallRequirement
 from pip._internal.utils.compat import stdlib_pkgs
+from pip._internal.utils.direct_url_helpers import (
+    direct_url_as_pep440_direct_reference,
+    direct_url_from_link,
+)
 
-from ._compat.pip_compat import Distribution, dist_requires
+from ._compat import Distribution, get_dev_pkgs
 from .exceptions import IncompatibleRequirements
 from .logging import log
 from .utils import (
     flat_map,
     format_requirement,
     get_hashes_from_ireq,
     is_url_requirement,
@@ -35,21 +31,21 @@
 PACKAGES_TO_IGNORE = [
     "-markerlib",
     "pip",
     "pip-tools",
     "pip-review",
     "pkg-resources",
     *stdlib_pkgs,
-    *DEV_PKGS,
+    *get_dev_pkgs(),
 ]
 
 
 def dependency_tree(
     installed_keys: Mapping[str, Distribution], root_key: str
-) -> Set[str]:
+) -> set[str]:
     """
     Calculate the dependency tree for the package `root_key` and return
     a collection of all its dependencies.  Uses a DFS traversal algorithm.
 
     `installed_keys` should be a {key: requirement} mapping, e.g.
         {'django': from_line('django==1.8')}
     `root_key` should be the key to return the dependency tree for.
@@ -59,108 +55,126 @@
 
     if root_key in installed_keys:
         dep = installed_keys[root_key]
         queue.append(dep)
 
     while queue:
         v = queue.popleft()
-        key = key_from_req(v)
+        key = v.key
         if key in dependencies:
             continue
 
         dependencies.add(key)
 
-        for dep_specifier in dist_requires(v):
+        for dep_specifier in v.requires:
             dep_name = key_from_req(dep_specifier)
             if dep_name in installed_keys:
                 dep = installed_keys[dep_name]
 
                 if dep_specifier.specifier.contains(dep.version):
                     queue.append(dep)
 
     return dependencies
 
 
-def get_dists_to_ignore(installed: Iterable[Distribution]) -> List[str]:
+def get_dists_to_ignore(installed: Iterable[Distribution]) -> list[str]:
     """
     Returns a collection of package names to ignore when performing pip-sync,
     based on the currently installed environment.  For example, when pip-tools
     is installed in the local environment, it should be ignored, including all
     of its dependencies (e.g. click).  When pip-tools is not installed
     locally, click should also be installed/uninstalled depending on the given
     requirements.
     """
-    installed_keys = {key_from_req(r): r for r in installed}
+    installed_keys = {r.key: r for r in installed}
     return list(
         flat_map(lambda req: dependency_tree(installed_keys, req), PACKAGES_TO_IGNORE)
     )
 
 
 def merge(
     requirements: Iterable[InstallRequirement], ignore_conflicts: bool
 ) -> ValuesView[InstallRequirement]:
-    by_key: Dict[str, InstallRequirement] = {}
+    by_key: dict[str, InstallRequirement] = {}
 
     for ireq in requirements:
         # Limitation: URL requirements are merged by precise string match, so
         # "file:///example.zip#egg=example", "file:///example.zip", and
         # "example==1.0" will not merge with each other
         if ireq.match_markers():
             key = key_from_ireq(ireq)
 
             if not ignore_conflicts:
                 existing_ireq = by_key.get(key)
                 if existing_ireq:
                     # NOTE: We check equality here since we can assume that the
                     # requirements are all pinned
-                    if ireq.specifier != existing_ireq.specifier:
+                    if (
+                        ireq.req
+                        and existing_ireq.req
+                        and ireq.specifier != existing_ireq.specifier
+                    ):
                         raise IncompatibleRequirements(ireq, existing_ireq)
 
             # TODO: Always pick the largest specifier in case of a conflict
             by_key[key] = ireq
     return by_key.values()
 
 
 def diff_key_from_ireq(ireq: InstallRequirement) -> str:
     """
     Calculate a key for comparing a compiled requirement with installed modules.
     For URL requirements, only provide a useful key if the url includes
-    #egg=name==version, which will set ireq.req.name and ireq.specifier.
+    a hash, e.g. #sha1=..., in any of the supported hash algorithms.
     Otherwise return ireq.link so the key will not match and the package will
     reinstall. Reinstall is necessary to ensure that packages will reinstall
-    if the URL is changed but the version is not.
+    if the contents at the URL have changed but the version has not.
     """
     if is_url_requirement(ireq):
-        if (
-            ireq.req
-            and (getattr(ireq.req, "key", None) or getattr(ireq.req, "name", None))
-            and ireq.specifier
-        ):
-            return key_from_ireq(ireq)
+        if getattr(ireq.req, "name", None) and ireq.link.has_hash:
+            return str(
+                direct_url_as_pep440_direct_reference(
+                    direct_url_from_link(ireq.link), ireq.req.name
+                )
+            )
+        # TODO: Also support VCS and editable installs.
         return str(ireq.link)
     return key_from_ireq(ireq)
 
 
+def diff_key_from_req(req: Distribution) -> str:
+    """Get a unique key for the requirement."""
+    key = req.key
+    if (
+        req.direct_url
+        and isinstance(req.direct_url.info, ArchiveInfo)
+        and req.direct_url.info.hash
+    ):
+        key = direct_url_as_pep440_direct_reference(req.direct_url, key)
+    # TODO: Also support VCS and editable installs.
+    return key
+
+
 def diff(
     compiled_requirements: Iterable[InstallRequirement],
     installed_dists: Iterable[Distribution],
-) -> Tuple[Set[InstallRequirement], Set[str]]:
+) -> tuple[set[InstallRequirement], set[str]]:
     """
     Calculate which packages should be installed or uninstalled, given a set
     of compiled requirements and a list of currently installed modules.
     """
     requirements_lut = {diff_key_from_ireq(r): r for r in compiled_requirements}
 
     satisfied = set()  # holds keys
     to_install = set()  # holds InstallRequirement objects
     to_uninstall = set()  # holds keys
 
     pkgs_to_ignore = get_dists_to_ignore(installed_dists)
     for dist in installed_dists:
-        key = key_from_req(dist)
+        key = diff_key_from_req(dist)
         if key not in requirements_lut or not requirements_lut[key].match_markers():
             to_uninstall.add(key)
         elif requirements_lut[key].specifier.contains(dist.version):
             satisfied.add(key)
 
     for key, requirement in requirements_lut.items():
         if key not in satisfied and requirement.match_markers():
@@ -172,17 +186,17 @@
     return (to_install, to_uninstall)
 
 
 def sync(
     to_install: Iterable[InstallRequirement],
     to_uninstall: Iterable[InstallRequirement],
     dry_run: bool = False,
-    install_flags: Optional[List[str]] = None,
+    install_flags: list[str] | None = None,
     ask: bool = False,
-    python_executable: Optional[str] = None,
+    python_executable: str | None = None,
 ) -> int:
     """
     Install and uninstalls the given sets of modules.
     """
     exit_code = 0
 
     python_executable = python_executable or sys.executable
```

### Comparing `pip-tools-6.9.0/piptools/writer.py` & `pip-tools-7.0.0/piptools/writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,25 @@
+from __future__ import annotations
+
+import io
 import os
 import re
 import sys
 from itertools import chain
-from typing import (
-    BinaryIO,
-    Dict,
-    Iterable,
-    Iterator,
-    List,
-    Optional,
-    Set,
-    Tuple,
-    Union,
-    cast,
-)
+from typing import BinaryIO, Iterable, Iterator, cast
 
 from click import unstyle
 from click.core import Context
 from pip._internal.models.format_control import FormatControl
 from pip._internal.req.req_install import InstallRequirement
 from pip._vendor.packaging.markers import Marker
 from pip._vendor.packaging.utils import canonicalize_name
 
 from .logging import log
 from .utils import (
-    UNSAFE_PACKAGES,
     comment,
     dedup,
     format_requirement,
     get_compile_command,
     key_from_ireq,
     strip_extras,
 )
@@ -37,15 +28,16 @@
     "# WARNING: pip install will require the following package to be hashed."
     "\n# Consider using a hashable URL like "
     "https://github.com/jazzband/pip-tools/archive/SOMECOMMIT.zip"
 )
 
 MESSAGE_UNSAFE_PACKAGES_UNPINNED = comment(
     "# WARNING: The following packages were not pinned, but pip requires them to be"
-    "\n# pinned when the requirements file includes hashes. "
+    "\n# pinned when the requirements file includes hashes and the requirement is not"
+    "\n# satisfied by a package already installed. "
     "Consider using the --allow-unsafe flag."
 )
 
 MESSAGE_UNSAFE_PACKAGES = comment(
     "# The following packages are considered to be unsafe in a requirements file:"
 )
 
@@ -54,34 +46,34 @@
     "See # WARNING lines for details."
 )
 
 
 strip_comes_from_line_re = re.compile(r" \(line \d+\)$")
 
 
-def _comes_from_as_string(comes_from: Union[str, InstallRequirement]) -> str:
+def _comes_from_as_string(comes_from: str | InstallRequirement) -> str:
     if isinstance(comes_from, str):
         return strip_comes_from_line_re.sub("", comes_from)
     return cast(str, canonicalize_name(key_from_ireq(comes_from)))
 
 
-def annotation_style_split(required_by: Set[str]) -> str:
+def annotation_style_split(required_by: set[str]) -> str:
     sorted_required_by = sorted(required_by)
     if len(sorted_required_by) == 1:
         source = sorted_required_by[0]
         annotation = "# via " + source
     else:
         annotation_lines = ["# via"]
         for source in sorted_required_by:
             annotation_lines.append("    #   " + source)
         annotation = "\n".join(annotation_lines)
     return annotation
 
 
-def annotation_style_line(required_by: Set[str]) -> str:
+def annotation_style_line(required_by: set[str]) -> str:
     return f"# via {', '.join(sorted(required_by))}"
 
 
 class OutputWriter:
     def __init__(
         self,
         dst_file: BinaryIO,
@@ -94,16 +86,17 @@
         annotation_style: str,
         strip_extras: bool,
         generate_hashes: bool,
         default_index_url: str,
         index_urls: Iterable[str],
         trusted_hosts: Iterable[str],
         format_control: FormatControl,
+        linesep: str,
         allow_unsafe: bool,
-        find_links: List[str],
+        find_links: list[str],
         emit_find_links: bool,
         emit_options: bool,
     ) -> None:
         self.dst_file = dst_file
         self.click_ctx = click_ctx
         self.dry_run = dry_run
         self.emit_header = emit_header
@@ -113,30 +106,31 @@
         self.annotation_style = annotation_style
         self.strip_extras = strip_extras
         self.generate_hashes = generate_hashes
         self.default_index_url = default_index_url
         self.index_urls = index_urls
         self.trusted_hosts = trusted_hosts
         self.format_control = format_control
+        self.linesep = linesep
         self.allow_unsafe = allow_unsafe
         self.find_links = find_links
         self.emit_find_links = emit_find_links
         self.emit_options = emit_options
 
-    def _sort_key(self, ireq: InstallRequirement) -> Tuple[bool, str]:
+    def _sort_key(self, ireq: InstallRequirement) -> tuple[bool, str]:
         return (not ireq.editable, key_from_ireq(ireq))
 
     def write_header(self) -> Iterator[str]:
         if self.emit_header:
             yield comment("#")
             yield comment(
-                "# This file is autogenerated by pip-compile with python "
+                "# This file is autogenerated by pip-compile with Python "
                 f"{sys.version_info.major}.{sys.version_info.minor}"
             )
-            yield comment("# To update, run:")
+            yield comment("# by the following command:")
             yield comment("#")
             compile_command = os.environ.get(
                 "CUSTOM_COMPILE_COMMAND"
             ) or get_compile_command(self.click_ctx)
             yield comment(f"#    {compile_command}")
             yield comment("#")
 
@@ -177,22 +171,22 @@
             emitted = True
             yield line
         if emitted:
             yield ""
 
     def _iter_lines(
         self,
-        results: Set[InstallRequirement],
-        unsafe_requirements: Optional[Set[InstallRequirement]] = None,
-        markers: Optional[Dict[str, Marker]] = None,
-        hashes: Optional[Dict[InstallRequirement, Set[str]]] = None,
+        results: set[InstallRequirement],
+        unsafe_requirements: set[InstallRequirement],
+        unsafe_packages: set[str],
+        markers: dict[str, Marker],
+        hashes: dict[InstallRequirement, set[str]] | None = None,
     ) -> Iterator[str]:
         # default values
-        unsafe_requirements = unsafe_requirements or set()
-        markers = markers or {}
+        unsafe_packages = unsafe_packages if self.allow_unsafe else set()
         hashes = hashes or {}
 
         # Check for unhashed or unpinned packages if at least one package does have
         # hashes, which will trigger pip install's --require-hashes mode.
         warn_uninstallable = False
         has_hashes = hashes and any(hash for hash in hashes.values())
 
@@ -201,20 +195,18 @@
         for line in self.write_header():
             yield line
             yielded = True
         for line in self.write_flags():
             yield line
             yielded = True
 
-        unsafe_requirements = (
-            {r for r in results if r.name in UNSAFE_PACKAGES}
-            if not unsafe_requirements
-            else unsafe_requirements
-        )
-        packages = {r for r in results if r.name not in UNSAFE_PACKAGES}
+        unsafe_requirements = unsafe_requirements or {
+            r for r in results if r.name in unsafe_packages
+        }
+        packages = {r for r in results if r.name not in unsafe_packages}
 
         if packages:
             for ireq in sorted(packages, key=self._sort_key):
                 if has_hashes and not hashes.get(ireq):
                     yield MESSAGE_UNHASHED_PACKAGE
                     warn_uninstallable = True
                 line = self._format_requirement(
@@ -247,34 +239,47 @@
             yield ""
 
         if warn_uninstallable:
             log.warning(MESSAGE_UNINSTALLABLE)
 
     def write(
         self,
-        results: Set[InstallRequirement],
-        unsafe_requirements: Set[InstallRequirement],
-        markers: Dict[str, Marker],
-        hashes: Optional[Dict[InstallRequirement, Set[str]]],
+        results: set[InstallRequirement],
+        unsafe_requirements: set[InstallRequirement],
+        unsafe_packages: set[str],
+        markers: dict[str, Marker],
+        hashes: dict[InstallRequirement, set[str]] | None,
     ) -> None:
-
-        for line in self._iter_lines(results, unsafe_requirements, markers, hashes):
-            if self.dry_run:
-                # Bypass the log level to always print this during a dry run
-                log.log(line)
-            else:
-                log.info(line)
-                self.dst_file.write(unstyle(line).encode())
-                self.dst_file.write(os.linesep.encode())
+        if not self.dry_run:
+            dst_file = io.TextIOWrapper(
+                self.dst_file,
+                encoding="utf8",
+                newline=self.linesep,
+                line_buffering=True,
+            )
+        try:
+            for line in self._iter_lines(
+                results, unsafe_requirements, unsafe_packages, markers, hashes
+            ):
+                if self.dry_run:
+                    # Bypass the log level to always print this during a dry run
+                    log.log(line)
+                else:
+                    log.info(line)
+                    dst_file.write(unstyle(line))
+                    dst_file.write("\n")
+        finally:
+            if not self.dry_run:
+                dst_file.detach()
 
     def _format_requirement(
         self,
         ireq: InstallRequirement,
-        marker: Optional[Marker] = None,
-        hashes: Optional[Dict[InstallRequirement, Set[str]]] = None,
+        marker: Marker | None = None,
+        hashes: dict[InstallRequirement, set[str]] | None = None,
     ) -> str:
         ireq_hashes = (hashes if hashes is not None else {}).get(ireq)
 
         line = format_requirement(ireq, marker=marker, hashes=ireq_hashes)
         if self.strip_extras:
             line = strip_extras(line)
```

### Comparing `pip-tools-6.9.0/tests/conftest.py` & `pip-tools-7.0.0/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,61 @@
+from __future__ import annotations
+
 import json
 import os
+import platform
 import subprocess
 import sys
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 from functools import partial
+from pathlib import Path
 from textwrap import dedent
-from typing import List, Optional
+from typing import Any
 
 import pytest
+import tomli_w
 from click.testing import CliRunner
 from pip._internal.commands.install import InstallCommand
 from pip._internal.index.package_finder import PackageFinder
 from pip._internal.models.candidate import InstallationCandidate
+from pip._internal.models.link import Link
 from pip._internal.network.session import PipSession
 from pip._internal.req.constructors import (
     install_req_from_editable,
     install_req_from_line,
 )
+from pip._internal.utils.direct_url_helpers import direct_url_from_link
 from pip._vendor.packaging.version import Version
 from pip._vendor.pkg_resources import Requirement
 
-from piptools._compat.pip_compat import uses_pkg_resources
+from piptools._compat import PIP_VERSION, Distribution
 from piptools.cache import DependencyCache
 from piptools.exceptions import NoCandidateFound
+from piptools.locations import CONFIG_FILE_NAME
+from piptools.logging import log
 from piptools.repositories import PyPIRepository
 from piptools.repositories.base import BaseRepository
 from piptools.resolver import BacktrackingResolver, LegacyResolver
 from piptools.utils import (
     as_tuple,
     is_url_requirement,
     key_from_ireq,
-    key_from_req,
     make_install_requirement,
 )
 
 from .constants import MINIMAL_WHEELS_PATH, TEST_DATA_PATH
 from .utils import looks_like_ci
 
 
 @dataclass
 class FakeOptions:
-    features_enabled: List[str] = field(default_factory=list)
-    deprecated_features_enabled: List[str] = field(default_factory=list)
-    target_dir: Optional[str] = None
+    features_enabled: list[str] = field(default_factory=list)
+    deprecated_features_enabled: list[str] = field(default_factory=list)
+    target_dir: str | None = None
 
 
 class FakeRepository(BaseRepository):
     def __init__(self, options: FakeOptions):
         self._options = options
 
         with open(os.path.join(TEST_DATA_PATH, "fake-index.json")) as f:
@@ -114,52 +122,39 @@
         """Not used"""
 
     @property
     def command(self) -> InstallCommand:
         """Not used"""
 
 
-class FakeInstalledDistribution:
-    def __init__(self, line, deps=None):
-        if deps is None:
-            deps = []
-        self.dep_strs = deps
-        self.deps = [Requirement.parse(d) for d in deps]
-
-        self.req = Requirement.parse(line)
-
-        self.key = key_from_req(self.req)
-        self.specifier = self.req.specifier
-
-        self.version = line.split("==")[1]
-
-    # The Distribution interface has changed between pkg_resources and
-    # importlib.metadata.
-    if uses_pkg_resources:
-
-        def requires(self):
-            return self.deps
-
-    else:
-
-        @property
-        def requires(self):
-            return self.dep_strs
-
-
 def pytest_collection_modifyitems(config, items):
     for item in items:
         # Mark network tests as flaky
         if item.get_closest_marker("network") and looks_like_ci():
             item.add_marker(pytest.mark.flaky(reruns=3, reruns_delay=2))
 
 
 @pytest.fixture
 def fake_dist():
-    return FakeInstalledDistribution
+    def _fake_dist(line, deps=None):
+        if deps is None:
+            deps = []
+        req = Requirement.parse(line)
+        key = req.key
+        if "==" in line:
+            version = line.split("==")[1]
+        else:
+            version = "0+unknown"
+        requires = [Requirement.parse(d) for d in deps]
+        direct_url = None
+        if req.url:
+            direct_url = direct_url_from_link(Link(req.url))
+        return Distribution(key, version, requires, direct_url)
+
+    return _fake_dist
 
 
 @pytest.fixture
 def repository():
     return FakeRepository(
         options=FakeOptions(deprecated_features_enabled=["legacy-resolver"])
     )
@@ -209,15 +204,23 @@
 @pytest.fixture
 def base_resolver(depcache):
     return partial(LegacyResolver, cache=depcache, existing_constraints={})
 
 
 @pytest.fixture
 def from_line():
-    return install_req_from_line
+    def _from_line(*args, **kwargs):
+        if PIP_VERSION[:2] <= (23, 0):
+            hash_options = kwargs.pop("hash_options", {})
+            options = kwargs.pop("options", {})
+            options["hashes"] = hash_options
+            kwargs["options"] = options
+        return install_req_from_line(*args, **kwargs)
+
+    return _from_line
 
 
 @pytest.fixture
 def from_editable():
     return install_req_from_editable
 
 
@@ -286,15 +289,14 @@
 @pytest.fixture
 def make_package(tmp_path):
     """
     Make a package from a given name, version and list of required packages.
     """
 
     def _make_package(name, version="0.1", install_requires=None, extras_require=None):
-
         if install_requires is None:
             install_requires = []
 
         if extras_require is None:
             extras_require = dict()
 
         install_requires_str = "[{}]".format(
@@ -412,14 +414,53 @@
     Generate distribution packages `small-fake-{a..f}`
     """
     dists_path = os.path.join(tmpdir, "dists")
     pkgs = [
         make_package("small-fake-a", version="0.1"),
         make_package("small-fake-b", version="0.2"),
         make_package("small-fake-c", version="0.3"),
-        make_package("small-fake-d", version="0.4"),
-        make_package("small-fake-e", version="0.5"),
-        make_package("small-fake-f", version="0.6"),
     ]
     for pkg in pkgs:
         make_wheel(pkg, dists_path)
     return dists_path
+
+
+@pytest.fixture
+def venv(tmp_path):
+    """Create a temporary venv and get the path of its directory of executables."""
+    subprocess.run(
+        [sys.executable, "-m", "venv", os.fspath(tmp_path)],
+        check=True,
+    )
+    return tmp_path / ("Scripts" if platform.system() == "Windows" else "bin")
+
+
+@pytest.fixture(autouse=True)
+def _reset_log():
+    """
+    Since piptools.logging.log is a global variable we have to restore its initial
+    state. Some tests can change logger verbosity which might cause a conflict
+    with other tests that depend on it.
+    """
+    log.reset()
+
+
+@pytest.fixture
+def make_config_file(tmpdir_cwd):
+    """
+    Make a config file for pip-tools with a given parameter set to a specific
+    value, returning a ``pathlib.Path`` to the config file.
+    """
+
+    def _maker(
+        pyproject_param: str, new_default: Any, config_file_name: str = CONFIG_FILE_NAME
+    ) -> Path:
+        # Make a config file with this one config default override
+        config_path = Path(tmpdir_cwd) / pyproject_param
+        config_file = config_path / config_file_name
+        config_path.mkdir(exist_ok=True)
+
+        config_to_dump = {"tool": {"pip-tools": {pyproject_param: new_default}}}
+        config_file.write_text(tomli_w.dumps(config_to_dump))
+        return config_file.relative_to(tmpdir_cwd)
+
+    return _maker
```

### Comparing `pip-tools-6.9.0/tests/test_cache.py` & `pip-tools-7.0.0/tests/test_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import sys
 from contextlib import contextmanager
 from shutil import rmtree
 from tempfile import NamedTemporaryFile
 
 import pytest
```

### Comparing `pip-tools-6.9.0/tests/test_cli_compile.py` & `pip-tools-7.0.0/tests/test_cli_compile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,38 @@
+from __future__ import annotations
+
+import hashlib
 import os
 import shutil
 import subprocess
 import sys
 from textwrap import dedent
 from unittest import mock
 
 import pytest
+from pip._internal.utils.hashes import FAVORITE_HASH
 from pip._internal.utils.urls import path_to_url
 
 from piptools.scripts.compile import cli
 from piptools.utils import COMPILE_EXCLUDE_OPTIONS
 
 from .constants import MINIMAL_WHEELS_PATH, PACKAGES_PATH
 
 legacy_resolver_only = pytest.mark.parametrize(
     "current_resolver",
     ("legacy",),
     indirect=("current_resolver",),
 )
 
+backtracking_resolver_only = pytest.mark.parametrize(
+    "current_resolver",
+    ("backtracking",),
+    indirect=("current_resolver",),
+)
+
 
 @pytest.fixture(
     autouse=True,
     params=[
         pytest.param("legacy", id="legacy resolver"),
         pytest.param("backtracking", id="backtracking resolver"),
     ],
@@ -88,30 +98,38 @@
             "89872db07ae70770fba97205b0737c17ef013d0d1c790"
             "899c16bb8bac419/pip_tools-3.6.1-py2.py3-none-any.whl",
             id="wheel URL",
         ),
     ),
 )
 def test_command_line_setuptools_read(
-    runner, make_pip_conf, make_package, install_requires, expected_output
+    runner, make_package, install_requires, expected_output
 ):
     package_dir = make_package(
         name="fake-setuptools-a",
         install_requires=(install_requires,),
     )
 
     out = runner.invoke(
         cli,
-        (str(package_dir / "setup.py"), "--find-links", MINIMAL_WHEELS_PATH),
+        (
+            str(package_dir / "setup.py"),
+            "--find-links",
+            MINIMAL_WHEELS_PATH,
+            "--no-build-isolation",
+        ),
     )
-
-    assert expected_output in out.stderr.splitlines()
+    assert out.exit_code == 0
 
     # check that pip-compile generated a configuration file
-    assert (package_dir / "requirements.txt").exists()
+    output_file = package_dir / "requirements.txt"
+    assert output_file.exists()
+
+    # The package version must NOT be updated in the output file
+    assert expected_output in output_file.read_text().splitlines()
 
 
 @pytest.mark.network
 @pytest.mark.parametrize(
     ("options", "expected_output_file"),
     (
         # For the `pip-compile` output file should be "requirements.txt"
@@ -137,15 +155,15 @@
                 """\
                 from setuptools import setup
                 setup(install_requires=[])
                 """
             )
         )
 
-    out = runner.invoke(cli, options)
+    out = runner.invoke(cli, ["--no-build-isolation"] + options)
     assert out.exit_code == 0
     assert os.path.exists(expected_output_file)
 
 
 @pytest.mark.network
 def test_command_line_setuptools_nested_output_file(tmpdir, runner):
     """
@@ -159,15 +177,15 @@
                 """\
                 from setuptools import setup
                 setup(install_requires=[])
                 """
             )
         )
 
-    out = runner.invoke(cli, [str(proj_dir / "setup.py")])
+    out = runner.invoke(cli, [str(proj_dir / "setup.py"), "--no-build-isolation"])
     assert out.exit_code == 0
     assert (proj_dir / "requirements.txt").exists()
 
 
 @pytest.mark.network
 def test_setuptools_preserves_environment_markers(
     runner, make_package, make_wheel, make_pip_conf, tmpdir
@@ -189,24 +207,37 @@
     bar_dir = make_package(
         name="bar", version="2.0", install_requires=['foo ; python_version >= "1"']
     )
     out = runner.invoke(
         cli,
         [
             str(bar_dir / "setup.py"),
+            "--output-file",
+            "-",
             "--no-header",
             "--no-annotate",
             "--no-emit-find-links",
+            "--no-build-isolation",
             "--find-links",
             str(dists_dir),
         ],
     )
 
     assert out.exit_code == 0, out.stderr
-    assert out.stderr == 'foo==1.0 ; python_version >= "1"\n'
+    assert out.stdout == 'foo==1.0 ; python_version >= "1"\n'
+
+
+def test_no_index_option(runner, tmp_path):
+    req_in = tmp_path / "requirements.in"
+    req_in.touch()
+
+    out = runner.invoke(cli, [req_in.as_posix(), "--no-index", "--verbose"])
+
+    assert out.exit_code == 0
+    assert "Ignoring indexes." in out.stderr
 
 
 def test_find_links_option(runner):
     with open("requirements.in", "w") as req_in:
         req_in.write("-f ./libs3")
 
     out = runner.invoke(cli, ["-v", "-f", "./libs1", "-f", "./libs2"])
@@ -343,16 +374,16 @@
             ["--index-url", "https://index-url", "--no-emit-index-url"], id="index url"
         ),
     ),
 )
 def test_all_no_emit_options(runner, options):
     with open("requirements.in", "w"):
         pass
-    out = runner.invoke(cli, ["--no-header", *options])
-    assert out.stderr.strip().splitlines() == []
+    out = runner.invoke(cli, ["--output-file", "-", "--no-header", *options])
+    assert out.stdout.strip().splitlines() == []
 
 
 @pytest.mark.parametrize(
     ("option", "expected_output"),
     (
         pytest.param(
             "--emit-index-url", ["--index-url https://index-url"], id="index url"
@@ -361,18 +392,27 @@
     ),
 )
 def test_emit_index_url_option(runner, option, expected_output):
     with open("requirements.in", "w"):
         pass
 
     out = runner.invoke(
-        cli, ["--no-header", "--index-url", "https://index-url", option]
+        cli,
+        [
+            "--output-file",
+            "-",
+            "--quiet",
+            "--no-header",
+            "--index-url",
+            "https://index-url",
+            option,
+        ],
     )
 
-    assert out.stderr.strip().splitlines() == expected_output
+    assert out.stdout.strip().splitlines() == expected_output
 
 
 @pytest.mark.network
 def test_realistic_complex_sub_dependencies(runner):
     wheels_dir = "wheels"
 
     # make a temporary wheel of a fake package
@@ -460,20 +500,20 @@
 
     with open("requirements.in", "w") as req_in:
         req_in.write(
             "-c constraints.txt"  # require editable fake package
             "\nsmall_fake_with_unpinned_deps"  # This one also requires small_fake_a
         )
 
-    out = runner.invoke(cli, ["-n"])
+    out = runner.invoke(cli, ["--output-file", "-", "--quiet"])
 
     assert out.exit_code == 0
-    assert fake_package_dir in out.stderr
+    assert fake_package_dir in out.stdout
     # Shouldn't include a non-editable small-fake-a==<version>.
-    assert "small-fake-a==" not in out.stderr
+    assert "small-fake-a==" not in out.stdout
 
 
 @legacy_resolver_only
 @pytest.mark.parametrize("req_editable", ((True,), (False,)))
 def test_editable_package_in_constraints(pip_conf, runner, req_editable):
     """
     piptools can compile an editable that appears in both primary requirements
@@ -507,14 +547,69 @@
         req_in.write("-e " + vcs_package)
     out = runner.invoke(cli, ["-n", "--rebuild"])
     assert out.exit_code == 0
     assert vcs_package in out.stderr
     assert "click" in out.stderr  # dependency of pip-tools
 
 
+@pytest.mark.network
+def test_compile_cached_vcs_package(runner, venv):
+    """
+    Test pip-compile doesn't write local paths for cached wheels of VCS packages.
+
+    Regression test for issue GH-1647.
+    """
+    vcs_package = (
+        "typing-extensions @ git+https://github.com/python/typing_extensions@"
+        "9c0759a260fe126210a1e2026720000a3c40a919"
+    )
+    vcs_wheel_prefix = "typing_extensions-4.3.0-py3"
+
+    # Install and cache VCS package.
+    subprocess.run(
+        [os.fspath(venv / "python"), "-m" "pip", "install", vcs_package],
+        check=True,
+    )
+    assert (
+        vcs_wheel_prefix
+        in subprocess.run(
+            [
+                sys.executable,
+                "-m" "pip",
+                "cache",
+                "list",
+                "--format=abspath",
+                vcs_wheel_prefix,
+            ],
+            check=True,
+            capture_output=True,
+            text=True,
+        ).stdout
+    )
+
+    with open("requirements.in", "w") as req_in:
+        req_in.write(vcs_package)
+
+    out = runner.invoke(
+        cli,
+        [
+            "--output-file",
+            "-",
+            "--quiet",
+            "--no-header",
+            "--no-emit-options",
+            "--no-annotate",
+            "--no-build-isolation",
+        ],
+    )
+
+    assert out.exit_code == 0, out
+    assert vcs_package == out.stdout.strip()
+
+
 @legacy_resolver_only
 def test_locally_available_editable_package_is_not_archived_in_cache_dir(
     pip_conf, tmpdir, runner
 ):
     """
     piptools will not create an archive for a locally available editable requirement
     """
@@ -572,15 +667,17 @@
 )
 @pytest.mark.parametrize("generate_hashes", ((True,), (False,)))
 @pytest.mark.network
 def test_url_package(runner, line, dependency, generate_hashes):
     with open("requirements.in", "w") as req_in:
         req_in.write(line)
     out = runner.invoke(
-        cli, ["-n", "--rebuild"] + (["--generate-hashes"] if generate_hashes else [])
+        cli,
+        ["-n", "--rebuild", "--no-build-isolation"]
+        + (["--generate-hashes"] if generate_hashes else []),
     )
     assert out.exit_code == 0
     assert dependency in out.stderr
 
 
 @pytest.mark.parametrize(
     ("line", "dependency", "rewritten_line"),
@@ -676,15 +773,15 @@
 
 
 def test_direct_reference_with_extras(runner):
     with open("requirements.in", "w") as req_in:
         req_in.write(
             "pip-tools[testing,coverage] @ git+https://github.com/jazzband/pip-tools@6.2.0"
         )
-    out = runner.invoke(cli, ["-n", "--rebuild"])
+    out = runner.invoke(cli, ["-n", "--rebuild", "--no-build-isolation"])
     assert out.exit_code == 0
     assert "pip-tools @ git+https://github.com/jazzband/pip-tools@6.2.0" in out.stderr
     assert "pytest==" in out.stderr
     assert "pytest-cov==" in out.stderr
 
 
 def test_input_file_without_extension(pip_conf, runner):
@@ -757,14 +854,35 @@
         req_in.write("small-fake-a\nsmall-fake-b")
 
     out = runner.invoke(cli, ["--no-annotate", "-P", "small-fake-b"])
 
     assert out.exit_code == 0
     assert "small-fake-a==0.2" in out.stderr.splitlines()
     assert "small-fake-b==0.3" in out.stderr.splitlines()
+    assert (
+        "WARNING: the output file requirements.txt exists but is empty"
+        not in out.stderr
+    )
+
+
+def test_upgrade_packages_empty_target_file_warning(pip_conf, runner):
+    """
+    piptools warns the user if --upgrade-package/-P is specified and the
+    output file exists, but is empty.
+    """
+    with open("requirements.in", "w") as req_in:
+        req_in.write("small-fake-a==0.2")
+    with open("requirements.txt", "w") as req_txt:
+        req_txt.write("")
+
+    out = runner.invoke(cli, ["--no-annotate", "-P", "small-fake-a"])
+
+    assert out.exit_code == 0
+    assert "small-fake-a==0.2" in out.stderr.splitlines()
+    assert "WARNING: the output file requirements.txt exists but is empty" in out.stderr
 
 
 @pytest.mark.parametrize(
     ("current_package", "upgraded_package"),
     (
         pytest.param("small-fake-b==0.1", "small-fake-b==0.3", id="upgrade"),
         pytest.param("small-fake-b==0.3", "small-fake-b==0.1", id="downgrade"),
@@ -799,21 +917,28 @@
     out = runner.invoke(cli, ["-P", "small-fake-b==0.2"])
 
     assert out.exit_code == 0
     assert "small-fake-a==0.2" in out.stderr
     assert "small-fake-b==0.2" in out.stderr
 
 
-def test_upgrade_packages_version_option_and_upgrade(pip_conf, runner):
+@pytest.mark.parametrize(
+    "reqs_in",
+    (
+        pytest.param("small-fake-a\nsmall-fake-b", id="direct reqs"),
+        pytest.param("small-fake-with-unpinned-deps", id="parent req"),
+    ),
+)
+def test_upgrade_packages_version_option_and_upgrade(pip_conf, runner, reqs_in):
     """
     piptools respects --upgrade-package/-P inline list with specified versions
     whilst also doing --upgrade.
     """
     with open("requirements.in", "w") as req_in:
-        req_in.write("small-fake-a\nsmall-fake-b")
+        req_in.write(reqs_in)
     with open("requirements.txt", "w") as req_in:
         req_in.write("small-fake-a==0.1\nsmall-fake-b==0.1")
 
     out = runner.invoke(cli, ["--upgrade", "-P", "small-fake-b==0.1"])
 
     assert out.exit_code == 0
     assert "small-fake-a==0.2" in out.stderr
@@ -831,35 +956,85 @@
     out = runner.invoke(cli, ["--upgrade", "-P", "small-fake-b==0.1"])
 
     assert out.exit_code == 0
     assert "small-fake-a==0.2" in out.stderr
     assert "small-fake-b==0.1" in out.stderr
 
 
-def test_quiet_option(runner):
-    with open("requirements", "w"):
-        pass
-    out = runner.invoke(cli, ["--quiet", "requirements"])
-    # Pinned requirements result has not been written to stdout or stderr:
-    assert not out.stdout_bytes
-    assert not out.stderr_bytes
+def test_upgrade_package_with_extra(runner, make_package, make_sdist, tmpdir):
+    """
+    piptools ignores extras on --upgrade-package/-P items if already constrained.
+    """
+    test_package_1 = make_package(
+        "test_package_1", version="0.1", extras_require={"more": "test_package_2"}
+    )
+    test_package_2 = make_package(
+        "test_package_2",
+        version="0.1",
+    )
+    dists_dir = tmpdir / "dists"
+    for pkg in (test_package_1, test_package_2):
+        make_sdist(pkg, dists_dir)
+
+    # Constrain our requirement with an extra
+    with open("requirements.in", "w") as req_in:
+        req_in.write("test-package-1[more]")
+
+    # Run update on test-package-1[more] -- this should be equivalent
+    # to running an update on test-package-1
+    out = runner.invoke(
+        cli,
+        [
+            "--output-file",
+            "-",
+            "--quiet",
+            "--find-links",
+            str(dists_dir),
+            "--no-annotate",
+            "--no-header",
+            "--no-emit-options",
+            "--no-build-isolation",
+            "--upgrade-package",
+            "test-package-1[more]",
+        ],
+    )
+
+    assert out.exit_code == 0, out
+    assert (
+        dedent(
+            """\
+            test-package-1[more]==0.1
+            test-package-2==0.1
+            """
+        )
+        == out.stdout
+    )
+
+
+def test_quiet_option(pip_conf, runner):
+    with open("requirements.in", "w") as req_in:
+        req_in.write("small-fake-a")
+
+    out = runner.invoke(cli, ["--quiet"])
+    # Pinned requirements result has not been written to stderr:
+    assert b"small-fake-a" not in out.stderr_bytes
 
 
 def test_dry_run_noisy_option(runner):
-    with open("requirements", "w"):
+    with open("requirements.in", "w"):
         pass
-    out = runner.invoke(cli, ["--dry-run", "requirements"])
+    out = runner.invoke(cli, ["--dry-run"])
     # Dry-run message has been written to output
     assert "Dry-run, so nothing updated." in out.stderr.splitlines()
 
 
 def test_dry_run_quiet_option(runner):
-    with open("requirements", "w"):
+    with open("requirements.in", "w"):
         pass
-    out = runner.invoke(cli, ["--dry-run", "--quiet", "requirements"])
+    out = runner.invoke(cli, ["--output-file", "-", "--dry-run", "--quiet"])
     # Neither dry-run message nor pinned requirements written to output:
     assert not out.stdout_bytes
     # Dry-run message has not been written to stderr:
     assert "dry-run" not in out.stderr.lower()
     # Pinned requirements (just the header in this case) *are* written to stderr:
     assert "# " in out.stderr
 
@@ -914,52 +1089,150 @@
 
 
 @pytest.mark.network
 def test_generate_hashes_with_annotations(runner):
     with open("requirements.in", "w") as fp:
         fp.write("six==1.15.0")
 
-    out = runner.invoke(cli, ["--generate-hashes"])
-    assert out.stderr == dedent(
-        f"""\
-        #
-        # This file is autogenerated by pip-compile with python \
-{sys.version_info.major}.{sys.version_info.minor}
-        # To update, run:
-        #
-        #    pip-compile --generate-hashes
-        #
+    out = runner.invoke(
+        cli,
+        [
+            "--output-file",
+            "-",
+            "--quiet",
+            "--no-header",
+            "--generate-hashes",
+        ],
+    )
+    assert out.stdout == dedent(
+        """\
         six==1.15.0 \\
             --hash=sha256:30639c035cdb23534cd4aa2dd52c3bf48f06e5f4a941509c8bafd8ce11080259 \\
             --hash=sha256:8b74bedcbbbaca38ff6d7491d76f2b06b3592611af620f8426e82dddb04a5ced
             # via -r requirements.in
         """
     )
 
 
 @pytest.mark.network
+@pytest.mark.parametrize("gen_hashes", (True, False))
+@pytest.mark.parametrize(
+    "annotate_options",
+    (
+        ("--no-annotate",),
+        ("--annotation-style", "line"),
+        ("--annotation-style", "split"),
+    ),
+)
+@pytest.mark.parametrize(
+    ("nl_options", "must_include", "must_exclude"),
+    (
+        pytest.param(("--newline", "lf"), b"\n", b"\r\n", id="LF"),
+        pytest.param(("--newline", "crlf"), b"\r\n", b"\n", id="CRLF"),
+        pytest.param(
+            ("--newline", "native"),
+            os.linesep.encode(),
+            {"\n": b"\r\n", "\r\n": b"\n"}[os.linesep],
+            id="native",
+        ),
+    ),
+)
+def test_override_newline(
+    pip_conf,
+    runner,
+    gen_hashes,
+    annotate_options,
+    nl_options,
+    must_include,
+    must_exclude,
+    tmp_path,
+):
+    opts = annotate_options + nl_options
+    if gen_hashes:
+        opts += ("--generate-hashes",)
+
+    example_dir = tmp_path / "example_dir"
+    example_dir.mkdir()
+    in_path = example_dir / "requirements.in"
+    out_path = example_dir / "requirements.txt"
+    in_path.write_bytes(b"small-fake-a==0.1\nsmall-fake-b\n")
+
+    runner.invoke(
+        cli, [*opts, f"--output-file={os.fsdecode(out_path)}", os.fsdecode(in_path)]
+    )
+    txt = out_path.read_bytes()
+
+    assert must_include in txt
+
+    if must_exclude in must_include:
+        txt = txt.replace(must_include, b"")
+    assert must_exclude not in txt
+
+    # Do it again, with --newline=preserve:
+
+    opts = annotate_options + ("--newline", "preserve")
+    if gen_hashes:
+        opts += ("--generate-hashes",)
+
+    runner.invoke(
+        cli, [*opts, f"--output-file={os.fsdecode(out_path)}", os.fsdecode(in_path)]
+    )
+    txt = out_path.read_bytes()
+
+    assert must_include in txt
+
+    if must_exclude in must_include:
+        txt = txt.replace(must_include, b"")
+    assert must_exclude not in txt
+
+
+@pytest.mark.network
+@pytest.mark.parametrize(
+    ("linesep", "must_exclude"),
+    (pytest.param("\n", "\r\n", id="LF"), pytest.param("\r\n", "\n", id="CRLF")),
+)
+def test_preserve_newline_from_input(runner, linesep, must_exclude):
+    with open("requirements.in", "wb") as req_in:
+        req_in.write(f"six{linesep}".encode())
+
+    runner.invoke(cli, ["--newline=preserve", "requirements.in"])
+    with open("requirements.txt", "rb") as req_txt:
+        txt = req_txt.read().decode()
+
+    assert linesep in txt
+
+    if must_exclude in linesep:
+        txt = txt.replace(linesep, "")
+    assert must_exclude not in txt
+
+
+@pytest.mark.network
 def test_generate_hashes_with_split_style_annotations(runner):
     with open("requirements.in", "w") as fp:
         fp.write("Django==1.11.29\n")
         fp.write("django-debug-toolbar==1.11\n")
         fp.write("django-storages==1.9.1\n")
         fp.write("django-taggit==0.24.0\n")
         fp.write("pytz==2020.4\n")
         fp.write("sqlparse==0.3.1\n")
 
-    out = runner.invoke(cli, ["--generate-hashes", "--annotation-style", "split"])
-    assert out.stderr == dedent(
-        f"""\
-        #
-        # This file is autogenerated by pip-compile with python \
-{sys.version_info.major}.{sys.version_info.minor}
-        # To update, run:
-        #
-        #    pip-compile --generate-hashes
-        #
+    out = runner.invoke(
+        cli,
+        [
+            "--output-file",
+            "-",
+            "--quiet",
+            "--no-header",
+            "--generate-hashes",
+            "--annotation-style",
+            "split",
+        ],
+    )
+    assert out.stdout == dedent(
+        """\
         django==1.11.29 \\
             --hash=sha256:014e3392058d94f40569206a24523ce254d55ad2f9f46c6550b0fe2e4f94cf3f \\
             --hash=sha256:4200aefb6678019a0acf0005cd14cfce3a5e6b9b90d06145fcdd2e474ad4329c
             # via
             #   -r requirements.in
             #   django-debug-toolbar
             #   django-storages
@@ -998,24 +1271,28 @@
         fp.write("Django==1.11.29\n")
         fp.write("django-debug-toolbar==1.11\n")
         fp.write("django-storages==1.9.1\n")
         fp.write("django-taggit==0.24.0\n")
         fp.write("pytz==2020.4\n")
         fp.write("sqlparse==0.3.1\n")
 
-    out = runner.invoke(cli, ["--generate-hashes", "--annotation-style", "line"])
-    assert out.stderr == dedent(
-        f"""\
-        #
-        # This file is autogenerated by pip-compile with python \
-{sys.version_info.major}.{sys.version_info.minor}
-        # To update, run:
-        #
-        #    pip-compile --annotation-style=line --generate-hashes
-        #
+    out = runner.invoke(
+        cli,
+        [
+            "--output-file",
+            "-",
+            "--quiet",
+            "--no-header",
+            "--generate-hashes",
+            "--annotation-style",
+            "line",
+        ],
+    )
+    assert out.stdout == dedent(
+        """\
         django==1.11.29 \\
             --hash=sha256:014e3392058d94f40569206a24523ce254d55ad2f9f46c6550b0fe2e4f94cf3f \\
             --hash=sha256:4200aefb6678019a0acf0005cd14cfce3a5e6b9b90d06145fcdd2e474ad4329c
             # via -r requirements.in, django-debug-toolbar, django-storages, django-taggit
         django-debug-toolbar==1.11 \\
             --hash=sha256:89d75b60c65db363fb24688d977e5fbf0e73386c67acf562d278402a10fc3736 \\
             --hash=sha256:c2b0134119a624f4ac9398b44f8e28a01c7686ac350a12a74793f3dd57a9eea0
@@ -1036,33 +1313,91 @@
             --hash=sha256:022fb9c87b524d1f7862b3037e541f68597a730a8843245c349fc93e1643dc4e \\
             --hash=sha256:e162203737712307dfe78860cc56c8da8a852ab2ee33750e33aeadf38d12c548
             # via -r requirements.in, django-debug-toolbar
         """
     )
 
 
+@pytest.mark.network
+def test_generate_hashes_with_mixed_sources(
+    runner, make_package, make_wheel, make_sdist, tmp_path
+):
+    """
+    Test that pip-compile generate hashes for every file from all given sources:
+    PyPI and/or --find-links.
+    """
+
+    wheels_dir = tmp_path / "wheels"
+    wheels_dir.mkdir()
+
+    dummy_six_pkg = make_package(name="six", version="1.16.0")
+    make_wheel(dummy_six_pkg, wheels_dir, "--build-number", "123")
+
+    fav_hasher = hashlib.new(FAVORITE_HASH)
+    fav_hasher.update((wheels_dir / "six-1.16.0-123-py3-none-any.whl").read_bytes())
+    dummy_six_wheel_digest = fav_hasher.hexdigest()
+
+    with open("requirements.in", "w") as fp:
+        fp.write("six==1.16.0\n")
+
+    out = runner.invoke(
+        cli,
+        [
+            "--output-file",
+            "-",
+            "--quiet",
+            "--no-header",
+            "--generate-hashes",
+            "--no-emit-options",
+            "--no-annotate",
+            "--find-links",
+            wheels_dir.as_uri(),
+        ],
+    )
+
+    expected_digests = sorted(
+        (
+            # sdist hash for six-1.16.0.tar.gz from PyPI
+            "1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
+            # wheel hash for six-1.16.0-py2.py3-none-any.whl from PyPI
+            "8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254",
+            # wheel hash for local six-1.16.0-123-py3-none-any.whl file
+            dummy_six_wheel_digest,
+        )
+    )
+    expected_output = dedent(
+        f"""\
+        six==1.16.0 \\
+            --hash=sha256:{expected_digests[0]} \\
+            --hash=sha256:{expected_digests[1]} \\
+            --hash=sha256:{expected_digests[2]}
+        """
+    )
+    assert out.stdout == expected_output
+
+
 def test_filter_pip_markers(pip_conf, runner):
     """
     Check that pip-compile works with pip environment markers (PEP496)
     """
-    with open("requirements", "w") as req_in:
+    with open("requirements.in", "w") as req_in:
         req_in.write("small-fake-a==0.1\nunknown_package==0.1; python_version == '1'")
 
-    out = runner.invoke(cli, ["-n", "requirements"])
+    out = runner.invoke(cli, ["--output-file", "-", "--quiet"])
 
     assert out.exit_code == 0
-    assert "small-fake-a==0.1" in out.stderr
-    assert "unknown_package" not in out.stderr
+    assert "small-fake-a==0.1" in out.stdout
+    assert "unknown_package" not in out.stdout
 
 
 def test_bad_setup_file(runner):
     with open("setup.py", "w") as package:
         package.write("BAD SYNTAX")
 
-    out = runner.invoke(cli, [])
+    out = runner.invoke(cli, ["--no-build-isolation"])
 
     assert out.exit_code == 2
     assert f"Failed to parse {os.path.abspath('setup.py')}" in out.stderr
 
 
 @legacy_resolver_only
 def test_no_candidates(pip_conf, runner):
@@ -1125,46 +1460,28 @@
     """
     out = runner.invoke(cli, ["-n", "-"])
 
     assert out.exit_code == 2
     assert "--output-file is required if input is from stdin" in out.stderr
 
 
-def test_not_specified_input_file(runner):
-    """
-    It should raise an error if there are no input files or default input files
-    such as "setup.py" or "requirements.in".
-    """
-    out = runner.invoke(cli)
-    assert "If you do not specify an input file" in out.stderr
-    assert out.exit_code == 2
-
-
 def test_stdin(pip_conf, runner):
     """
     Test compile requirements from STDIN.
     """
     out = runner.invoke(
         cli,
-        ["-", "--output-file", "requirements.txt", "-n", "--no-emit-find-links"],
+        ["-", "--output-file", "-", "--quiet", "--no-emit-options", "--no-header"],
         input="small-fake-a==0.1",
     )
 
-    assert out.stderr == dedent(
-        f"""\
-        #
-        # This file is autogenerated by pip-compile with python \
-{sys.version_info.major}.{sys.version_info.minor}
-        # To update, run:
-        #
-        #    pip-compile --no-emit-find-links --output-file=requirements.txt -
-        #
+    assert out.stdout == dedent(
+        """\
         small-fake-a==0.1
             # via -r -
-        Dry-run, so nothing updated.
         """
     )
 
 
 def test_multiple_input_files_without_output_file(runner):
     """
     The --output-file option is required for multiple requirement input files.
@@ -1184,61 +1501,37 @@
 
 
 @pytest.mark.parametrize(
     ("options", "expected"),
     (
         pytest.param(
             ("--annotate",),
-            f"""\
-            #
-            # This file is autogenerated by pip-compile with python \
-{sys.version_info.major}.{sys.version_info.minor}
-            # To update, run:
-            #
-            #    pip-compile --no-emit-find-links
-            #
+            """\
             small-fake-a==0.1
                 # via
                 #   -c constraints.txt
                 #   small-fake-with-deps
             small-fake-with-deps==0.1
                 # via -r requirements.in
-            Dry-run, so nothing updated.
             """,
             id="annotate",
         ),
         pytest.param(
             ("--annotate", "--annotation-style", "line"),
-            f"""\
-            #
-            # This file is autogenerated by pip-compile with python \
-{sys.version_info.major}.{sys.version_info.minor}
-            # To update, run:
-            #
-            #    pip-compile --annotation-style=line --no-emit-find-links
-            #
+            """\
             small-fake-a==0.1         # via -c constraints.txt, small-fake-with-deps
             small-fake-with-deps==0.1  # via -r requirements.in
-            Dry-run, so nothing updated.
             """,
             id="annotate line style",
         ),
         pytest.param(
             ("--no-annotate",),
-            f"""\
-            #
-            # This file is autogenerated by pip-compile with python \
-{sys.version_info.major}.{sys.version_info.minor}
-            # To update, run:
-            #
-            #    pip-compile --no-annotate --no-emit-find-links
-            #
+            """\
             small-fake-a==0.1
             small-fake-with-deps==0.1
-            Dry-run, so nothing updated.
             """,
             id="no annotate",
         ),
     ),
 )
 def test_annotate_option(pip_conf, runner, options, expected):
     """
@@ -1246,29 +1539,34 @@
     """
     with open("constraints.txt", "w") as constraints_in:
         constraints_in.write("small-fake-a==0.1")
     with open("requirements.in", "w") as req_in:
         req_in.write("-c constraints.txt\n")
         req_in.write("small_fake_with_deps")
 
-    out = runner.invoke(cli, [*options, "-n", "--no-emit-find-links"])
+    out = runner.invoke(
+        cli,
+        [*options, "--output-file", "-", "--quiet", "--no-emit-options", "--no-header"],
+    )
 
     assert out.exit_code == 0, out
-    assert out.stderr == dedent(expected)
+    assert out.stdout == dedent(expected)
 
 
 @pytest.mark.parametrize(
     ("option", "expected"),
     (
         pytest.param(
             "--allow-unsafe",
             dedent(
                 """\
                 small-fake-a==0.1
                 small-fake-b==0.3
+
+                # The following packages are considered to be unsafe in a requirements file:
                 small-fake-with-deps==0.1
                 """
             ),
             id="allow all packages",
         ),
         pytest.param(
             "--no-allow-unsafe",
@@ -1306,23 +1604,79 @@
     with open("requirements.in", "w") as req_in:
         req_in.write("small-fake-b\n")
         req_in.write("small-fake-with-deps")
 
     out = runner.invoke(
         cli,
         [
+            "--output-file",
+            "-",
+            "--quiet",
             "--no-header",
             "--no-emit-options",
             "--no-annotate",
             *([option] if option else []),
         ],
     )
 
     assert out.exit_code == 0, out
-    assert out.stderr == expected
+    assert out.stdout == expected
+
+
+@pytest.mark.parametrize(
+    ("unsafe_package", "expected"),
+    (
+        (
+            "small-fake-with-deps",
+            dedent(
+                """\
+                small-fake-a==0.1
+                small-fake-b==0.3
+
+                # The following packages are considered to be unsafe in a requirements file:
+                # small-fake-with-deps
+                """
+            ),
+        ),
+        (
+            "small-fake-a",
+            dedent(
+                """\
+                small-fake-b==0.3
+                small-fake-with-deps==0.1
+
+                # The following packages are considered to be unsafe in a requirements file:
+                # small-fake-a
+                """
+            ),
+        ),
+    ),
+)
+def test_unsafe_package_option(pip_conf, monkeypatch, runner, unsafe_package, expected):
+    monkeypatch.setattr("piptools.resolver.UNSAFE_PACKAGES", {"small-fake-with-deps"})
+    with open("requirements.in", "w") as req_in:
+        req_in.write("small-fake-b\n")
+        req_in.write("small-fake-with-deps")
+
+    out = runner.invoke(
+        cli,
+        [
+            "--output-file",
+            "-",
+            "--quiet",
+            "--no-header",
+            "--no-emit-options",
+            "--no-annotate",
+            "--unsafe-package",
+            unsafe_package,
+        ],
+    )
+
+    assert out.exit_code == 0, out
+    assert out.stdout == expected
 
 
 @pytest.mark.parametrize(
     ("option", "attr", "expected"),
     (("--cert", "cert", "foo.crt"), ("--client-cert", "client_cert", "bar.pem")),
 )
 @mock.patch("piptools.scripts.compile.parse_requirements")
@@ -1341,29 +1695,61 @@
 
 
 @pytest.mark.parametrize(
     ("option", "expected"),
     (("--build-isolation", True), ("--no-build-isolation", False)),
 )
 @mock.patch("piptools.scripts.compile.parse_requirements")
-def test_build_isolation_option(parse_requirements, runner, option, expected):
+def test_parse_requirements_build_isolation_option(
+    parse_requirements, runner, option, expected
+):
     """
     A value of the --build-isolation/--no-build-isolation flag
     must be passed to parse_requirements().
     """
     with open("requirements.in", "w"):
         pass
 
     runner.invoke(cli, [option])
 
     # Ensure the options in parse_requirements has the expected build_isolation option
     args, kwargs = parse_requirements.call_args
     assert kwargs["options"].build_isolation is expected
 
 
+@pytest.mark.parametrize(
+    ("option", "expected"),
+    (("--build-isolation", True), ("--no-build-isolation", False)),
+)
+@mock.patch("piptools.scripts.compile.project_wheel_metadata")
+def test_project_wheel_metadata_isolation_option(
+    project_wheel_metadata, runner, option, expected
+):
+    """
+    A value of the --build-isolation/--no-build-isolation flag
+    must be passed to project_wheel_metadata().
+    """
+
+    with open("setup.py", "w") as package:
+        package.write(
+            dedent(
+                """\
+                from setuptools import setup
+                setup(install_requires=[])
+                """
+            )
+        )
+
+    runner.invoke(cli, [option])
+
+    # Ensure the options in project_wheel_metadata has the isolated kwarg
+    _, kwargs = project_wheel_metadata.call_args
+    assert kwargs["isolated"] is expected
+
+
 @mock.patch("piptools.scripts.compile.PyPIRepository")
 def test_forwarded_args(PyPIRepository, runner):
     """
     Test the forwarded cli args (--pip-args 'arg...') are passed to the pip command.
     """
     with open("requirements.in", "w"):
         pass
@@ -1507,33 +1893,62 @@
     # Downgrade small-fake-a to 0.1
     with open("requirements.txt", "w") as req_txt:
         req_txt.write(
             "small-fake-with-deps==0.1\n"
             "small-fake-a==0.1         # via small-fake-with-deps\n"
         )
 
-    runner.invoke(cli, ["-P", "small-fake-a", "--no-emit-find-links"])
+    runner.invoke(cli, ["-P", "small-fake-a", "--no-emit-options", "--no-header"])
     with open("requirements.txt") as req_txt:
         assert req_txt.read() == dedent(
-            f"""\
-            #
-            # This file is autogenerated by pip-compile with python \
-{sys.version_info.major}.{sys.version_info.minor}
-            # To update, run:
-            #
-            #    pip-compile --no-emit-find-links
-            #
+            """\
             small-fake-a==0.1
                 # via small-fake-with-deps
             small-fake-with-deps==0.1
                 # via -r requirements.in
             """
         )
 
 
+@pytest.mark.parametrize(("num_inputs"), (2, 3, 10))
+def test_many_inputs_includes_all_annotations(pip_conf, runner, tmp_path, num_inputs):
+    """
+    Tests that an entry required by multiple input files is attributed to all of them in the
+    annotation.
+    See: https://github.com/jazzband/pip-tools/issues/1853
+    """
+    req_ins = [tmp_path / f"requirements{n:02d}.in" for n in range(num_inputs)]
+    for req_in in req_ins:
+        req_in.write_text("small-fake-a==0.1\n")
+
+    out = runner.invoke(
+        cli,
+        [
+            "--output-file",
+            "-",
+            "--quiet",
+            "--no-header",
+            "--no-emit-find-links",
+        ]
+        + [str(r) for r in req_ins],
+    )
+    assert out.exit_code == 0, out.stderr
+    assert (
+        out.stdout
+        == "\n".join(
+            [
+                "small-fake-a==0.1",
+                "    # via",
+            ]
+            + [f"    #   -r {req_in}" for req_in in req_ins]
+        )
+        + "\n"
+    )
+
+
 @pytest.mark.parametrize(
     "options",
     (
         "--index-url https://example.com",
         "--extra-index-url https://example.com",
         "--find-links ./libs1",
         "--trusted-host example.com",
@@ -1588,34 +2003,36 @@
     assert out.exit_code == 2, out
 
     stderr_lines = out.stderr.splitlines()
     assert "No versions found" in stderr_lines
     assert expected_message in stderr_lines
 
 
+@pytest.mark.parametrize("subdep_already_pinned", (True, False))
 @pytest.mark.parametrize(
     ("current_package", "upgraded_package"),
     (
         pytest.param("small-fake-b==0.1", "small-fake-b==0.2", id="upgrade"),
         pytest.param("small-fake-b==0.2", "small-fake-b==0.1", id="downgrade"),
     ),
 )
 def test_upgrade_packages_option_subdependency(
-    pip_conf, runner, current_package, upgraded_package
+    pip_conf, runner, current_package, upgraded_package, subdep_already_pinned
 ):
     """
     Test that pip-compile --upgrade-package/-P upgrades/downgrades subdependencies.
     """
 
     with open("requirements.in", "w") as reqs:
         reqs.write("small-fake-with-unpinned-deps\n")
 
     with open("requirements.txt", "w") as reqs:
         reqs.write("small-fake-a==0.1\n")
-        reqs.write(current_package + "\n")
+        if subdep_already_pinned:
+            reqs.write(current_package + "\n")
         reqs.write("small-fake-with-unpinned-deps==0.1\n")
 
     out = runner.invoke(
         cli, ["--no-annotate", "--dry-run", "--upgrade-package", upgraded_package]
     )
 
     stderr_lines = out.stderr.splitlines()
@@ -1671,18 +2088,18 @@
     after compile if they were removed from requirements.in file.
     """
     with open("requirements.in", "w") as req_in:
         req_in.write(input_opts)
     with open("requirements.txt", "w") as req_txt:
         req_txt.write(output_opts)
 
-    out = runner.invoke(cli, ["--no-header"])
+    out = runner.invoke(cli, ["--output-file", "-", "--quiet", "--no-header"])
 
     assert out.exit_code == 0, out
-    assert out.stderr.strip() == input_opts
+    assert out.stdout.strip() == input_opts
 
 
 def test_sub_dependencies_with_constraints(pip_conf, runner):
     # Write constraints file
     with open("constraints.txt", "w") as constraints_in:
         constraints_in.write("small-fake-a==0.1\n")
         constraints_in.write("small-fake-b==0.2\n")
@@ -1714,14 +2131,35 @@
 
     out = runner.invoke(cli, ["--no-annotate", "--no-header"])
 
     assert out.exit_code == 0, out
     assert "small-fake-a==0.3b1" in out.stderr.splitlines()
 
 
+@backtracking_resolver_only
+def test_ignore_compiled_unavailable_version(pip_conf, runner, current_resolver):
+    with open("requirements.in", "w") as req_in:
+        req_in.write("small-fake-a")
+
+    with open("requirements.txt", "w") as req_txt:
+        req_txt.write("small-fake-a==9999")
+
+    out = runner.invoke(cli, ["--no-annotate", "--no-header"])
+
+    assert out.exit_code == 0, out
+    assert "small-fake-a==" in out.stderr
+    assert "small-fake-a==9999" not in out.stderr.splitlines()
+
+    assert (
+        "Discarding small-fake-a==9999 "
+        "(from -r requirements.txt (line 1)) "
+        "to proceed the resolution"
+    ) in out.stderr
+
+
 def test_prefer_binary_dist(
     pip_conf, make_package, make_sdist, make_wheel, tmpdir, runner
 ):
     """
     Test pip-compile chooses a correct version of a package with
     a binary distribution when PIP_PREFER_BINARY environment variable is on.
     """
@@ -1926,15 +2364,24 @@
             [
                 "fake-ray[default]==0.1\n",
                 "fake-tune-sklearn==0.7\n",
             ]
         )
 
     out = runner.invoke(
-        cli, ["--find-links", str(dists_dir), "--no-header", "--no-emit-options"]
+        cli,
+        [
+            "--output-file",
+            "-",
+            "--quiet",
+            "--find-links",
+            str(dists_dir),
+            "--no-header",
+            "--no-emit-options",
+        ],
     )
     assert out.exit_code == 0
     assert (
         dedent(
             """\
         fake-colorful==0.3
             # via fake-ray
@@ -1944,15 +2391,15 @@
             #   fake-tune-sklearn
         fake-tensorboardx==0.5
             # via fake-ray
         fake-tune-sklearn==0.7
             # via -r requirements.in
         """
         )
-        == out.stderr
+        == out.stdout
     )
 
 
 @pytest.mark.parametrize(
     ("pkg2_install_requires", "req_in_content", "out_expected_content"),
     (
         pytest.param(
@@ -2030,41 +2477,35 @@
             [metadata]
             name = sample_lib
             author = Vincent Driessen
             author_email = me@nvie.com
 
             [options]
             packages = find:
-            install_requires =
-                small-fake-a==0.1
-                small-fake-b==0.2
+            install_requires = small-fake-a==0.1
 
             [options.extras_require]
-            dev =
-                small-fake-c==0.3
-                small-fake-d==0.4
-            test =
-                small-fake-e==0.5
-                small-fake-f==0.6
+            dev = small-fake-b==0.2
+            test = small-fake-c==0.3
         """,
         id="setup.cfg",
     ),
     pytest.param(
         "setup.py",
         """
             from setuptools import setup, find_packages
 
             setup(
                 name="sample_lib",
                 version=0.1,
-                install_requires=["small-fake-a==0.1", "small-fake-b==0.2"],
+                install_requires=["small-fake-a==0.1"],
                 packages=find_packages(),
                 extras_require={
-                    "dev": ["small-fake-c==0.3", "small-fake-d==0.4"],
-                    "test": ["small-fake-e==0.5", "small-fake-f==0.6"],
+                    "dev": ["small-fake-b==0.2"],
+                    "test": ["small-fake-c==0.3"],
                 },
             )
         """,
         id="setup.py",
     ),
     pytest.param(
         "pyproject.toml",
@@ -2074,19 +2515,19 @@
             build-backend = "flit_core.buildapi"
 
             [tool.flit.metadata]
             module = "sample_lib"
             author = "Vincent Driessen"
             author-email = "me@nvie.com"
 
-            requires = ["small-fake-a==0.1", "small-fake-b==0.2"]
+            requires = ["small-fake-a==0.1"]
 
             [tool.flit.metadata.requires-extra]
-            dev  = ["small-fake-c==0.3", "small-fake-d==0.4"]
-            test = ["small-fake-e==0.5", "small-fake-f==0.6"]
+            dev  = ["small-fake-b==0.2"]
+            test = ["small-fake-c==0.3"]
         """,
         id="flit",
     ),
     pytest.param(
         "pyproject.toml",
         """
             [build-system]
@@ -2099,64 +2540,107 @@
             description = ""
             authors = ["Vincent Driessen <me@nvie.com>"]
 
             [tool.poetry.dependencies]
             python = "*"
             small-fake-a = "0.1"
             small-fake-b = "0.2"
-
             small-fake-c = "0.3"
-            small-fake-d = "0.4"
-            small-fake-e = "0.5"
-            small-fake-f = "0.6"
 
             [tool.poetry.extras]
-            dev  = ["small-fake-c", "small-fake-d"]
-            test = ["small-fake-e", "small-fake-f"]
+            dev  = ["small-fake-b"]
+            test = ["small-fake-c"]
         """,
         id="poetry",
     ),
 )
 
 
 @pytest.mark.network
 @pytest.mark.parametrize(("fname", "content"), METADATA_TEST_CASES)
+def test_not_specified_input_file(
+    fake_dists, runner, make_module, fname, content, monkeypatch
+):
+    """
+    Test that a default-named file is parsed if present.
+    """
+    meta_path = make_module(fname=fname, content=content)
+    monkeypatch.chdir(os.path.dirname(meta_path))
+    out = runner.invoke(
+        cli,
+        [
+            "--output-file",
+            "-",
+            "--no-header",
+            "--no-emit-options",
+            "--no-annotate",
+            "--no-build-isolation",
+            "--find-links",
+            fake_dists,
+        ],
+    )
+    monkeypatch.undo()
+
+    assert out.exit_code == 0, out.stderr
+    assert "small-fake-a==0.1\n" == out.stdout
+
+
+def test_not_specified_input_file_without_allowed_files(runner):
+    """
+    It should raise an error if there are no input files or default input files
+    such as "setup.py" or "requirements.in".
+    """
+    out = runner.invoke(cli)
+    assert out.exit_code == 2
+    expected_error = (
+        "Error: Invalid value: If you do not specify an input file, the default "
+        "is one of: requirements.in, setup.py, pyproject.toml, setup.cfg"
+    )
+    assert expected_error in out.stderr.splitlines()
+
+
+@pytest.mark.network
+@pytest.mark.parametrize(("fname", "content"), METADATA_TEST_CASES)
 def test_input_formats(fake_dists, runner, make_module, fname, content):
     """
     Test different dependency formats as input file.
     """
     meta_path = make_module(fname=fname, content=content)
-    out = runner.invoke(cli, ["-n", "--find-links", fake_dists, meta_path])
+    out = runner.invoke(
+        cli, ["-n", "--no-build-isolation", "--find-links", fake_dists, meta_path]
+    )
     assert out.exit_code == 0, out.stderr
     assert "small-fake-a==0.1" in out.stderr
-    assert "small-fake-b==0.2" in out.stderr
+    assert "small-fake-b" not in out.stderr
     assert "small-fake-c" not in out.stderr
-    assert "small-fake-d" not in out.stderr
-    assert "small-fake-e" not in out.stderr
-    assert "small-fake-f" not in out.stderr
     assert "extra ==" not in out.stderr
 
 
 @pytest.mark.network
 @pytest.mark.parametrize(("fname", "content"), METADATA_TEST_CASES)
 def test_one_extra(fake_dists, runner, make_module, fname, content):
     """
     Test one `--extra` (dev) passed, other extras (test) must be ignored.
     """
     meta_path = make_module(fname=fname, content=content)
     out = runner.invoke(
-        cli, ["-n", "--extra", "dev", "--find-links", fake_dists, meta_path]
+        cli,
+        [
+            "-n",
+            "--extra",
+            "dev",
+            "--no-build-isolation",
+            "--find-links",
+            fake_dists,
+            meta_path,
+        ],
     )
     assert out.exit_code == 0, out.stderr
     assert "small-fake-a==0.1" in out.stderr
     assert "small-fake-b==0.2" in out.stderr
-    assert "small-fake-c==0.3" in out.stderr
-    assert "small-fake-d==0.4" in out.stderr
-    assert "small-fake-e" not in out.stderr
-    assert "small-fake-f" not in out.stderr
     assert "extra ==" not in out.stderr
 
 
 @pytest.mark.network
 @pytest.mark.parametrize(
     "extra_opts",
     (
@@ -2171,63 +2655,59 @@
     """
     meta_path = make_module(fname=fname, content=content)
     out = runner.invoke(
         cli,
         [
             "-n",
             *extra_opts,
+            "--no-build-isolation",
             "--find-links",
             fake_dists,
             meta_path,
         ],
     )
     assert out.exit_code == 0, out.stderr
     assert "small-fake-a==0.1" in out.stderr
     assert "small-fake-b==0.2" in out.stderr
-    assert "small-fake-c==0.3" in out.stderr
-    assert "small-fake-d==0.4" in out.stderr
-    assert "small-fake-e==0.5" in out.stderr
-    assert "small-fake-f==0.6" in out.stderr
     assert "extra ==" not in out.stderr
 
 
 @pytest.mark.network
 @pytest.mark.parametrize(("fname", "content"), METADATA_TEST_CASES)
 def test_all_extras(fake_dists, runner, make_module, fname, content):
     """
     Test passing `--all-extras` includes all applicable extras.
     """
     meta_path = make_module(fname=fname, content=content)
     out = runner.invoke(
         cli,
         [
-            "-n",
+            "--output-file",
+            "-",
+            "--quiet",
             "--all-extras",
             "--find-links",
             fake_dists,
             "--no-annotate",
             "--no-emit-options",
             "--no-header",
+            "--no-build-isolation",
             meta_path,
         ],
     )
-    assert out.exit_code == 0, out.stderr
+    assert out.exit_code == 0, out
     assert (
         dedent(
             """\
             small-fake-a==0.1
             small-fake-b==0.2
             small-fake-c==0.3
-            small-fake-d==0.4
-            small-fake-e==0.5
-            small-fake-f==0.6
-            Dry-run, so nothing updated.
             """
         )
-        == out.stderr
+        == out.stdout
     )
 
 
 # This should not depend on the metadata format so testing all cases is wasteful
 @pytest.mark.parametrize(("fname", "content"), METADATA_TEST_CASES[:1])
 def test_all_extras_fail_with_extra(fake_dists, runner, make_module, fname, content):
     """
@@ -2242,14 +2722,15 @@
             "--extra",
             "dev",
             "--find-links",
             fake_dists,
             "--no-annotate",
             "--no-emit-options",
             "--no-header",
+            "--no-build-isolation",
             meta_path,
         ],
     )
     assert out.exit_code == 2
     exp = "--extra has no effect when used with --all-extras"
     assert exp in out.stderr
 
@@ -2307,7 +2788,204 @@
     """Test resolver reched max rounds and raises error."""
     with open("requirements.in", "w") as reqs_out:
         reqs_out.write("six")
 
     out = runner.invoke(cli, ["--max-rounds", 0])
 
     assert out.exit_code != 0, out
+
+
+def test_preserve_via_requirements_constrained_dependencies_when_run_twice(
+    pip_conf, runner
+):
+    """
+    Test that 2 consecutive runs of pip-compile (first with a non-existing requirements.txt file,
+    second with an existing file) produce the same output.
+    """
+    with open("constraints.txt", "w") as constraints_in:
+        constraints_in.write("small-fake-a==0.1")
+
+    with open("requirements.in", "w") as req_in:
+        req_in.write("-c constraints.txt\nsmall_fake_with_deps")
+
+    cli_arguments = ["--no-emit-options", "--no-header"]
+
+    # First run of the command will generate `requirements.txt`, which doesn't yet exist.
+    first_out = runner.invoke(cli, cli_arguments)
+    assert first_out.exit_code == 0, first_out
+
+    with open("requirements.txt") as req_txt:
+        first_output = req_txt.read()
+
+    # Second run of the command will update `requirements.txt`.
+    second_out = runner.invoke(cli, cli_arguments)
+    assert second_out.exit_code == 0, second_out
+
+    with open("requirements.txt") as req_txt:
+        second_output = req_txt.read()
+
+    expected_output = dedent(
+        """\
+        small-fake-a==0.1
+            # via
+            #   -c constraints.txt
+            #   small-fake-with-deps
+        small-fake-with-deps==0.1
+            # via -r requirements.in
+        """
+    )
+    assert first_output == expected_output
+    assert second_output == expected_output
+
+
+def test_failure_of_legacy_resolver_prompts_for_backtracking(
+    pip_conf, runner, tmpdir, make_package, make_wheel, current_resolver
+):
+    """Test that pip-compile prompts to use the backtracking resolver"""
+    pkgs = [
+        make_package("a", version="0.1", install_requires=["b==0.1"]),
+        make_package("a", version="0.2", install_requires=["b==0.2"]),
+        make_package("b", version="0.1"),
+        make_package("b", version="0.2"),
+        make_package("c", version="1", install_requires=["b==0.1", "a"]),
+    ]
+
+    dists_dir = tmpdir / "dists"
+    for pkg in pkgs:
+        make_wheel(pkg, dists_dir)
+
+    with open("requirements.in", "w") as req_in:
+        req_in.writelines(["c"])
+
+    out = runner.invoke(
+        cli,
+        ["--resolver", current_resolver, "--find-links", str(dists_dir)],
+    )
+
+    if current_resolver == "legacy":
+        assert out.exit_code == 2, out
+        assert "Consider using backtracking resolver with" in out.stderr
+    elif current_resolver == "backtracking":
+        assert out.exit_code == 0, out
+    else:
+        raise AssertionError("unreachable")
+
+
+def test_print_deprecation_warning_if_using_legacy_resolver(runner, current_resolver):
+    with open("requirements.in", "w"):
+        pass
+
+    out = runner.invoke(cli)
+    assert out.exit_code == 0, out
+
+    expected_warning = "WARNING: the legacy dependency resolver is deprecated"
+    if current_resolver == "legacy":
+        assert expected_warning in out.stderr
+    else:
+        assert expected_warning not in out.stderr
+
+
+@pytest.mark.parametrize(
+    "input_filenames",
+    (
+        pytest.param(("requirements.txt",), id="one file"),
+        pytest.param(("requirements.txt", "dev-requirements.in"), id="multiple files"),
+    ),
+)
+def test_raise_error_when_input_and_output_filenames_are_matched(
+    runner, tmp_path, input_filenames
+):
+    req_in_paths = []
+    for input_filename in input_filenames:
+        req_in = tmp_path / input_filename
+        req_in.touch()
+        req_in_paths.append(req_in.as_posix())
+
+    req_out = tmp_path / "requirements.txt"
+    req_out_path = req_out.as_posix()
+
+    out = runner.invoke(cli, req_in_paths + ["--output-file", req_out_path])
+    assert out.exit_code == 2
+
+    expected_error = (
+        f"Error: input and output filenames must not be matched: {req_out_path}"
+    )
+    assert expected_error in out.stderr.splitlines()
+
+
+@pytest.mark.network
+@backtracking_resolver_only
+def test_pass_pip_cache_to_pip_args(tmpdir, runner, current_resolver):
+    cache_dir = tmpdir.mkdir("cache_dir")
+
+    with open("requirements.in", "w") as fp:
+        fp.write("six==1.15.0")
+
+    out = runner.invoke(
+        cli, ["--cache-dir", str(cache_dir), "--resolver", current_resolver]
+    )
+    assert out.exit_code == 0
+    assert os.listdir(os.path.join(str(cache_dir), "http"))
+
+
+@backtracking_resolver_only
+def test_compile_recursive_extras(runner, tmp_path, current_resolver):
+    (tmp_path / "pyproject.toml").write_text(
+        dedent(
+            """
+            [project]
+            name = "foo"
+            version = "0.0.1"
+            dependencies = ["small-fake-a"]
+            [project.optional-dependencies]
+            footest = ["small-fake-b"]
+            dev = ["foo[footest]"]
+            """
+        )
+    )
+    out = runner.invoke(
+        cli,
+        [
+            "--no-header",
+            "--no-annotate",
+            "--no-emit-find-links",
+            "--extra",
+            "dev",
+            "--find-links",
+            os.fspath(MINIMAL_WHEELS_PATH),
+            os.fspath(tmp_path / "pyproject.toml"),
+        ],
+    )
+    expected = rf"""foo @ {tmp_path.as_uri()}
+small-fake-a==0.2
+small-fake-b==0.3
+"""
+    assert out.exit_code == 0
+    assert expected == out.stderr
+
+
+def test_config_option(pip_conf, runner, tmp_path, make_config_file):
+    config_file = make_config_file("dry-run", True)
+
+    req_in = tmp_path / "requirements.in"
+    req_in.touch()
+
+    out = runner.invoke(cli, [req_in.as_posix(), "--config", config_file.as_posix()])
+
+    assert out.exit_code == 0
+    assert "Dry-run, so nothing updated" in out.stderr
+
+
+def test_no_config_option_overrides_config_with_defaults(
+    pip_conf, runner, tmp_path, make_config_file
+):
+    config_file = make_config_file("dry-run", True)
+
+    req_in = tmp_path / "requirements.in"
+    req_in.touch()
+
+    out = runner.invoke(
+        cli, [req_in.as_posix(), "--no-config", "--config", config_file.as_posix()]
+    )
+
+    assert out.exit_code == 0
+    assert "Dry-run, so nothing updated" not in out.stderr
```

### Comparing `pip-tools-6.9.0/tests/test_cli_sync.py` & `pip-tools-7.0.0/tests/test_cli_sync.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,47 @@
+from __future__ import annotations
+
 import os
 import subprocess
 import sys
 from unittest import mock
 
 import pytest
 from pip._vendor.packaging.version import Version
 
-from piptools.scripts.sync import DEFAULT_REQUIREMENTS_FILE, cli
+from piptools.scripts import sync
+from piptools.scripts.sync import cli
+
+
+@pytest.fixture(autouse=True)
+def _temp_default_reqs(tmp_path, monkeypatch):
+    monkeypatch.setattr(
+        sync, "DEFAULT_REQUIREMENTS_FILE", str(tmp_path / "requirements.txt")
+    )
 
 
 def test_run_as_module_sync():
     """piptools can be run as ``python -m piptools ...``."""
 
     result = subprocess.run(
         [sys.executable, "-m", "piptools", "sync", "--help"],
         stdout=subprocess.PIPE,
         check=True,
     )
 
-    # Should have run pip-compile successfully.
+    # Should have run pip-sync successfully.
     assert result.stdout.startswith(b"Usage:")
     assert b"Synchronize virtual environment with" in result.stdout
 
 
 @mock.patch("piptools.sync.run")
 def test_quiet_option(run, runner):
     """sync command can be run with `--quiet` or `-q` flag."""
 
-    with open("requirements.txt", "w") as req_in:
+    with open(sync.DEFAULT_REQUIREMENTS_FILE, "w") as req_in:
         req_in.write("six==1.10.0")
 
     out = runner.invoke(cli, ["-q"])
     assert not out.stderr_bytes
     assert out.exit_code == 0
 
     # for every call to pip ensure the `-q` flag is set
@@ -41,60 +51,59 @@
 
 
 @mock.patch("piptools.sync.run")
 def test_quiet_option_when_up_to_date(run, runner):
     """
     Sync should output nothing when everything is up to date and quiet option is set.
     """
-    with open("requirements.txt", "w"):
+    with open(sync.DEFAULT_REQUIREMENTS_FILE, "w"):
         pass
 
     with mock.patch("piptools.sync.diff", return_value=(set(), set())):
         out = runner.invoke(cli, ["-q"])
 
     assert not out.stderr_bytes
     assert out.exit_code == 0
     run.assert_not_called()
 
 
 def test_no_requirements_file(runner):
     """
     It should raise an error if there are no input files
-    or a requirements.txt file does not exist.
+    and a requirements.txt file does not exist.
     """
     out = runner.invoke(cli)
 
     assert "No requirement files given" in out.stderr
     assert out.exit_code == 2
 
 
-def test_input_files_with_dot_in_extension(runner):
+def test_input_files_with_dot_in_extension(runner, tmp_path):
     """
     It should raise an error if some of the input files have .in extension.
     """
-    with open("requirements.in", "w") as req_in:
-        req_in.write("six==1.10.0")
+    req_in = tmp_path / "requirements.in"
+    req_in.write_text("six==1.10.0")
 
-    out = runner.invoke(cli, ["requirements.in"])
+    out = runner.invoke(cli, [str(req_in)])
 
     assert "ERROR: Some input files have the .in extension" in out.stderr
     assert out.exit_code == 2
 
 
-def test_force_files_with_dot_in_extension(runner):
+def test_force_files_with_dot_in_extension(runner, tmp_path):
     """
     It should print a warning and sync anyway if some of the input files
     have .in extension.
     """
-
-    with open("requirements.in", "w") as req_in:
-        req_in.write("six==1.10.0")
+    req_in = tmp_path / "requirements.in"
+    req_in.write_text("six==1.10.0")
 
     with mock.patch("piptools.sync.run"):
-        out = runner.invoke(cli, ["requirements.in", "--force"])
+        out = runner.invoke(cli, [str(req_in), "--force"])
 
     assert "WARNING: Some input files have the .in extension" in out.stderr
     assert out.exit_code == 0
 
 
 @pytest.mark.parametrize(
     ("req_lines", "should_raise"),
@@ -108,29 +117,53 @@
 )
 def test_merge_error(req_lines, should_raise, runner):
     """
     Sync command should raise an error if there are merge errors.
     It should not raise an error if otherwise incompatible requirements
     are isolated by exclusive environment markers.
     """
-    with open("requirements.txt", "w") as req_in:
+    with open(sync.DEFAULT_REQUIREMENTS_FILE, "w") as req_in:
         for line in req_lines:
             req_in.write(line + "\n")
 
     with mock.patch("piptools.sync.run"):
         out = runner.invoke(cli, ["-n"])
 
     if should_raise:
         assert out.exit_code == 2
         assert "Incompatible requirements found" in out.stderr
     else:
         assert out.exit_code == 1
 
 
 @pytest.mark.parametrize(
+    "req_line",
+    (
+        "file:.",
+        "-e file:.",
+    ),
+)
+@mock.patch("piptools.sync.run")
+def test_merge_no_name_urls(run, req_line, runner, tmp_path):
+    """
+    Test sync succeeds when merging requirements that lack names.
+    """
+    reqs_paths = [
+        (tmp_path / name) for name in ("requirements.txt", "dev_requirements.txt")
+    ]
+
+    for reqs_path in reqs_paths:
+        reqs_path.write_text(f"{req_line} \n")
+
+    out = runner.invoke(cli, [str(path) for path in reqs_paths])
+    assert out.exit_code == 0
+    assert run.call_count == 2
+
+
+@pytest.mark.parametrize(
     ("cli_flags", "expected_install_flags"),
     (
         (
             ["--find-links", "./libs1", "--find-links", "./libs2"],
             ["--find-links", "./libs1", "--find-links", "./libs2"],
         ),
         (["--no-index"], ["--no-index"]),
@@ -161,15 +194,15 @@
     ),
 )
 @mock.patch("piptools.sync.run")
 def test_pip_install_flags(run, cli_flags, expected_install_flags, runner):
     """
     Test the cli flags have to be passed to the pip install command.
     """
-    with open("requirements.txt", "w") as req_in:
+    with open(sync.DEFAULT_REQUIREMENTS_FILE, "w") as req_in:
         req_in.write("six==1.10.0")
 
     runner.invoke(cli, cli_flags)
 
     call_args = [call[0][0] for call in run.call_args_list]
     called_install_options = [args[6:] for args in call_args if args[3] == "install"]
     assert called_install_options == [expected_install_flags], "Called args: {}".format(
@@ -190,15 +223,15 @@
     ),
 )
 @mock.patch("piptools.sync.run")
 def test_pip_install_flags_in_requirements_file(run, runner, install_flags):
     """
     Test the options from requirements.txt file pass to the pip install command.
     """
-    with open(DEFAULT_REQUIREMENTS_FILE, "w") as reqs:
+    with open(sync.DEFAULT_REQUIREMENTS_FILE, "w") as reqs:
         reqs.write(" ".join(install_flags) + "\n")
         reqs.write("six==1.10.0")
 
     out = runner.invoke(cli)
     assert out.exit_code == 0, out
 
     # Make sure pip install command has expected options
@@ -208,41 +241,41 @@
 
 
 @mock.patch("piptools.sync.run")
 def test_sync_ask_declined(run, runner):
     """
     Make sure nothing is installed if the confirmation is declined
     """
-    with open("requirements.txt", "w") as req_in:
+    with open(sync.DEFAULT_REQUIREMENTS_FILE, "w") as req_in:
         req_in.write("small-fake-a==1.10.0")
 
     runner.invoke(cli, ["--ask"], input="n\n")
 
     run.assert_not_called()
 
 
 @mock.patch("piptools.sync.run")
 def test_sync_ask_accepted(run, runner):
     """
     Make sure pip is called when the confirmation is accepted (even if
     --dry-run is given)
     """
-    with open("requirements.txt", "w") as req_in:
+    with open(sync.DEFAULT_REQUIREMENTS_FILE, "w") as req_in:
         req_in.write("small-fake-a==1.10.0")
 
     runner.invoke(cli, ["--ask", "--dry-run"], input="y\n")
 
     assert run.call_count == 2
 
 
 def test_sync_dry_run_returns_non_zero_exit_code(runner):
     """
     Make sure non-zero exit code is returned when --dry-run is given.
     """
-    with open("requirements.txt", "w") as req_in:
+    with open(sync.DEFAULT_REQUIREMENTS_FILE, "w") as req_in:
         req_in.write("small-fake-a==1.10.0")
 
     out = runner.invoke(cli, ["--dry-run"])
 
     assert out.exit_code == 1
 
 
@@ -251,15 +284,15 @@
     run,
     runner,
     fake_dist,
 ):
     """
     Make sure sync command can run with `--python-executable` option.
     """
-    with open("requirements.txt", "w") as req_in:
+    with open(sync.DEFAULT_REQUIREMENTS_FILE, "w") as req_in:
         req_in.write("small-fake-a==1.10.0")
 
     custom_executable = os.path.abspath(sys.executable)
 
     runner.invoke(cli, ["--python-executable", custom_executable])
 
     assert run.call_count == 2
@@ -280,53 +313,52 @@
     "python_executable",
     (
         "/tmp/invalid_executable",
         "invalid_python",
     ),
 )
 def test_invalid_python_executable(runner, python_executable):
-    with open("requirements.txt", "w") as req_in:
+    with open(sync.DEFAULT_REQUIREMENTS_FILE, "w") as req_in:
         req_in.write("small-fake-a==1.10.0")
 
     out = runner.invoke(cli, ["--python-executable", python_executable])
     assert out.exit_code == 2, out
     message = "Could not resolve '{}' as valid executable path or alias.\n"
     assert out.stderr == message.format(python_executable)
 
 
 @mock.patch("piptools.scripts.sync.get_pip_version_for_python_executable")
 def test_invalid_pip_version_in_python_executable(
-    get_pip_version_for_python_executable, runner
+    get_pip_version_for_python_executable, runner, tmp_path
 ):
-    with open("requirements.txt", "w") as req_in:
+    with open(sync.DEFAULT_REQUIREMENTS_FILE, "w") as req_in:
         req_in.write("small-fake-a==1.10.0")
 
-    custom_executable = os.path.abspath("custom_executable")
-    with open(custom_executable, "w") as exec_file:
-        exec_file.write("")
+    custom_executable = tmp_path / "custom_executable"
+    custom_executable.write_text("")
 
-    os.chmod(custom_executable, 0o700)
+    custom_executable.chmod(0o700)
 
     get_pip_version_for_python_executable.return_value = Version("19.1")
 
-    out = runner.invoke(cli, ["--python-executable", custom_executable])
+    out = runner.invoke(cli, ["--python-executable", str(custom_executable)])
     assert out.exit_code == 2, out
     message = (
         "Target python executable '{}' has pip version 19.1 installed. "
         "Version"  # ">=20.3 is expected.\n" part is omitted
     )
     assert out.stderr.startswith(message.format(custom_executable))
 
 
 @mock.patch("piptools.sync.run")
 def test_default_python_executable_option(run, runner):
     """
     Make sure sys.executable is used when --python-executable is not provided.
     """
-    with open("requirements.txt", "w") as req_in:
+    with open(sync.DEFAULT_REQUIREMENTS_FILE, "w") as req_in:
         req_in.write("small-fake-a==1.10.0")
 
     runner.invoke(cli)
 
     assert run.call_count == 2
 
     call_args = [call[0][0] for call in run.call_args_list]
@@ -336,7 +368,33 @@
             sys.executable,
             "-m",
             "pip",
             "install",
             "-r",
         ]
     ]
+
+
+@mock.patch("piptools.sync.run")
+def test_config_option(run, runner, make_config_file):
+    config_file = make_config_file("dry-run", True)
+
+    with open(sync.DEFAULT_REQUIREMENTS_FILE, "w") as reqs_txt:
+        reqs_txt.write("six==1.10.0")
+
+    out = runner.invoke(cli, ["--config", config_file.as_posix()])
+
+    assert out.exit_code == 1
+    assert "Would install:" in out.stdout
+
+
+@mock.patch("piptools.sync.run")
+def test_no_config_option_overrides_config_with_defaults(run, runner, make_config_file):
+    config_file = make_config_file("dry-run", True)
+
+    with open(sync.DEFAULT_REQUIREMENTS_FILE, "w") as reqs_txt:
+        reqs_txt.write("six==1.10.0")
+
+    out = runner.invoke(cli, ["--no-config", "--config", config_file.as_posix()])
+
+    assert out.exit_code == 0
+    assert "Would install:" not in out.stdout
```

### Comparing `pip-tools-6.9.0/tests/test_data/fake-index.json` & `pip-tools-7.0.0/tests/test_data/fake-index.json`

 * *Files identical despite different names*

### Comparing `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_a-0.1-py2.py3-none-any.whl` & `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_a-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_a-0.2-py2.py3-none-any.whl` & `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_a-0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_a-0.3b1-py2.py3-none-any.whl` & `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_a-0.3b1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_b-0.1-py2.py3-none-any.whl` & `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_b-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_b-0.2-py2.py3-none-any.whl` & `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_b-0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_b-0.3-py2.py3-none-any.whl` & `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_b-0.3-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_i686.whl` & `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_i686.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_x86_64.whl` & `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-manylinux1_x86_64.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-win32.whl` & `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_multi_arch-0.1-py2.py3-none-win32.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_with_deps-0.1-py2.py3-none-any.whl` & `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_with_deps-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_with_deps_and_sub_deps-0.1-py2.py3-none-any.whl` & `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_with_deps_and_sub_deps-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.9.0/tests/test_data/minimal_wheels/small_fake_with_unpinned_deps-0.1-py2.py3-none-any.whl` & `pip-tools-7.0.0/tests/test_data/minimal_wheels/small_fake_with_unpinned_deps-0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pip-tools-6.9.0/tests/test_data/packages/fake_with_deps/setup.py` & `pip-tools-7.0.0/tests/test_data/packages/fake_with_deps/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from setuptools import setup
 
 setup(
     name="fake_with_deps",
     version=0.1,
     install_requires=[
         "python-dateutil>=2.4.2,<2.5",
```

### Comparing `pip-tools-6.9.0/tests/test_fake_index.py` & `pip-tools-7.0.0/tests/test_fake_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 
 
 def test_find_best_match(from_line, repository):
     ireq = from_line("django>1.5")
     assert str(repository.find_best_match(ireq)) == "django==1.8"
```

### Comparing `pip-tools-6.9.0/tests/test_logging.py` & `pip-tools-7.0.0/tests/test_logging.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from piptools.logging import LogContext
 
 
 def test_indentation(runner):
     """
     Test LogContext.indentation() context manager increases indentation.
     """
```

### Comparing `pip-tools-6.9.0/tests/test_minimal_upgrade.py` & `pip-tools-7.0.0/tests/test_minimal_upgrade.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 
 from piptools.repositories import LocalRequirementsRepository
 from piptools.utils import key_from_ireq
 
 
 @pytest.mark.parametrize(
```

### Comparing `pip-tools-6.9.0/tests/test_repository_local.py` & `pip-tools-7.0.0/tests/test_repository_local.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 
 from piptools.repositories.local import LocalRequirementsRepository
 from piptools.utils import key_from_ireq
 
 EXPECTED = {"sha256:5e6071ee6e4c59e0d0408d366fe9b66781d2cf01be9a6e19a2433bb3c5336330"}
 
@@ -17,16 +19,16 @@
     captured = capsys.readouterr()
     assert captured.out == ""
     assert captured.err == ""
 
 
 def test_get_hashes_local_repository_cache_hit(from_line, repository):
     # Create an install requirement with the hashes included in its options
-    options = {"hashes": {"sha256": [entry.split(":")[1] for entry in EXPECTED]}}
-    req = from_line("small-fake-a==0.1", options=options)
+    hash_options = {"sha256": [entry.split(":")[1] for entry in EXPECTED]}
+    req = from_line("small-fake-a==0.1", hash_options=hash_options)
     existing_pins = {key_from_ireq(req): req}
 
     # Use fake repository so that we know the hashes are coming from cache
     local_repository = LocalRequirementsRepository(existing_pins, repository)
     with local_repository.allow_all_wheels():
         hashes = local_repository.get_hashes(from_line("small-fake-a==0.1"))
         assert hashes == EXPECTED
@@ -38,16 +40,16 @@
 @pytest.mark.parametrize(
     ("reuse_hashes", "expected"), ((True, NONSENSE), (False, EXPECTED))
 )
 def test_toggle_reuse_hashes_local_repository(
     capsys, pip_conf, from_line, pypi_repository, reuse_hashes, expected
 ):
     # Create an install requirement with the hashes included in its options
-    options = {"hashes": {"sha256": [entry.split(":")[1] for entry in NONSENSE]}}
-    req = from_line("small-fake-a==0.1", options=options)
+    hash_options = {"sha256": [entry.split(":")[1] for entry in NONSENSE]}
+    req = from_line("small-fake-a==0.1", hash_options=hash_options)
     existing_pins = {key_from_ireq(req): req}
 
     local_repository = LocalRequirementsRepository(
         existing_pins, pypi_repository, reuse_hashes=reuse_hashes
     )
     with local_repository.allow_all_wheels():
         assert local_repository.get_hashes(from_line("small-fake-a==0.1")) == expected
```

### Comparing `pip-tools-6.9.0/tests/test_repository_pypi.py` & `pip-tools-7.0.0/tests/test_repository_pypi.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+from __future__ import annotations
+
 import os
 from unittest import mock
 
 import pytest
+from pip._internal.models.candidate import InstallationCandidate
 from pip._internal.models.link import Link
 from pip._internal.utils.urls import path_to_url
 from pip._vendor.requests import HTTPError, Session
 
 from piptools.repositories import PyPIRepository
 from piptools.repositories.pypi import open_local_or_remote_file
 
@@ -171,79 +174,101 @@
         pytest.param(
             {
                 "releases": {
                     "0.1": [
                         {
                             "packagetype": "bdist_wheel",
                             "digests": {"sha256": "fake-hash"},
+                            "url": "https://link",
                         }
                     ]
                 }
             },
-            {"sha256:fake-hash"},
+            {"https://link": "sha256:fake-hash"},
             id="return single hash",
         ),
         pytest.param(
             {
                 "releases": {
                     "0.1": [
                         {
                             "packagetype": "bdist_wheel",
                             "digests": {"sha256": "fake-hash-number1"},
+                            "url": "https://link1",
                         },
                         {
                             "packagetype": "sdist",
                             "digests": {"sha256": "fake-hash-number2"},
+                            "url": "https://link2",
                         },
                     ]
                 }
             },
-            {"sha256:fake-hash-number1", "sha256:fake-hash-number2"},
+            {
+                "https://link1": "sha256:fake-hash-number1",
+                "https://link2": "sha256:fake-hash-number2",
+            },
             id="return multiple hashes",
         ),
         pytest.param(
             {
                 "releases": {
                     "0.1": [
                         {
                             "packagetype": "bdist_wheel",
                             "digests": {"sha256": "fake-hash-number1"},
+                            "url": "https://link1",
                         },
                         {
                             "packagetype": "sdist",
                             "digests": {"sha256": "fake-hash-number2"},
+                            "url": "https://link2",
                         },
                         {
                             "packagetype": "bdist_eggs",
                             "digests": {"sha256": "fake-hash-number3"},
+                            "url": "https://link3",
                         },
                     ]
                 }
             },
-            {"sha256:fake-hash-number1", "sha256:fake-hash-number2"},
+            {
+                "https://link1": "sha256:fake-hash-number1",
+                "https://link2": "sha256:fake-hash-number2",
+            },
             id="return only bdist_wheel and sdist hashes",
         ),
-        pytest.param(None, None, id="not found project data"),
-        pytest.param({}, None, id="not found releases key"),
-        pytest.param({"releases": {}}, None, id="not found version"),
-        pytest.param({"releases": {"0.1": [{}]}}, None, id="not found digests"),
+        pytest.param(None, {}, id="not found project data"),
+        pytest.param({}, {}, id="not found releases key"),
+        pytest.param({"releases": {}}, {}, id="not found version"),
+        pytest.param({"releases": {"0.1": [{}]}}, {}, id="not found digests"),
         pytest.param(
-            {"releases": {"0.1": [{"packagetype": "bdist_wheel", "digests": {}}]}},
-            None,
+            {
+                "releases": {
+                    "0.1": [
+                        {"packagetype": "bdist_wheel", "digests": {}, "url": "link"}
+                    ]
+                }
+            },
+            {},
             id="digests are empty",
         ),
         pytest.param(
             {
                 "releases": {
                     "0.1": [
-                        {"packagetype": "bdist_wheel", "digests": {"md5": "fake-hash"}}
+                        {
+                            "packagetype": "bdist_wheel",
+                            "digests": {"md5": "fake-hash"},
+                            "url": "https://link",
+                        }
                     ]
                 }
             },
-            None,
+            {},
             id="not found sha256 algo",
         ),
     ),
 )
 def test_get_hashes_from_pypi(from_line, tmpdir, project_data, expected_hashes):
     """
     Test PyPIRepository._get_hashes_from_pypi() returns expected hashes or None.
@@ -258,14 +283,72 @@
     )
     ireq = from_line("fake-package==0.1")
 
     actual_hashes = pypi_repository._get_hashes_from_pypi(ireq)
     assert actual_hashes == expected_hashes
 
 
+def test_get_hashes_from_mixed(pip_conf, from_line, tmpdir):
+    """
+    Test PyPIRepository.get_hashes() returns hashes from both PyPi and extra indexes/links
+    """
+
+    package_name = "small-fake-multi-arch"
+    package_version = "0.1"
+
+    # One candidate from PyPi and the rest from find-links / extra indexes
+    extra_index_link1 = Link("https://extra-index-link1")
+    extra_index_link2 = Link("https://extra-index-link2")
+    pypi_link = Link("https://pypi-link")
+
+    all_candidates = [
+        InstallationCandidate(package_name, package_version, extra_index_link1),
+        InstallationCandidate(package_name, package_version, extra_index_link2),
+        InstallationCandidate(package_name, package_version, pypi_link),
+    ]
+
+    # Extra indexes hashes so we don't spend time computing them
+    file_hashes = {
+        extra_index_link1: "sha256:hash-link1",
+        extra_index_link2: "sha256:hash-link2",
+    }
+    pypi_hash = "pypi-hash"
+
+    class MockPyPIRepository(PyPIRepository):
+        def _get_project(self, ireq):
+            return {
+                "releases": {
+                    package_version: [
+                        {
+                            "packagetype": "bdist_wheel",
+                            "digests": {"sha256": pypi_hash},
+                            "url": str(pypi_link),
+                        },
+                    ]
+                }
+            }
+
+        def find_all_candidates(self, req_name):
+            return all_candidates
+
+        def _get_file_hash(self, link):
+            return file_hashes[link]
+
+    pypi_repository = MockPyPIRepository(
+        ["--no-cache-dir"], cache_dir=(tmpdir / "pypi-repo-cache")
+    )
+
+    ireq = from_line(f"{package_name}=={package_version}")
+
+    expected_hashes = {"sha256:" + pypi_hash} | set(file_hashes.values())
+
+    actual_hashes = pypi_repository.get_hashes(ireq)
+    assert actual_hashes == expected_hashes
+
+
 def test_get_project__returns_data(from_line, tmpdir, monkeypatch, pypi_repository):
     """
     Test PyPIRepository._get_project() returns expected project data.
     """
     expected_data = {"releases": {"0.1": [{"digests": {"sha256": "fake-hash"}}]}}
 
     class MockResponse:
@@ -345,16 +428,16 @@
     assert actual_data is None
 
 
 def test_name_collision(from_line, pypi_repository, make_package, make_sdist, tmpdir):
     """
     Test to ensure we don't fail if there are multiple URL-based requirements
     ending with the same filename where later ones depend on earlier, e.g.
-    https://git.example.com/requirement1/master.zip#egg=req_package_1
-    https://git.example.com/requirement2/master.zip#egg=req_package_2
+    https://git.example.com/requirement1/main.zip#egg=req_package_1
+    https://git.example.com/requirement2/main.zip#egg=req_package_2
     In this case, if req_package_2 depends on req_package_1 we don't want to
     fail due to issues such as caching the requirement based on filename.
     """
     packages = {
         "test_package_1": make_package("test_package_1", version="0.1"),
         "test_package_2": make_package(
             "test_package_2", version="0.1", install_requires=["test-package-1"]
@@ -364,24 +447,24 @@
     for pkg_name, pkg in packages.items():
         pkg_path = tmpdir / pkg_name
 
         make_sdist(pkg, pkg_path, "--formats=zip")
 
         os.rename(
             os.path.join(pkg_path, f"{pkg_name}-0.1.zip"),
-            os.path.join(pkg_path, "master.zip"),
+            os.path.join(pkg_path, "main.zip"),
         )
 
     name_collision_1 = "file://{dist_path}#egg=test_package_1".format(
-        dist_path=tmpdir / "test_package_1" / "master.zip"
+        dist_path=tmpdir / "test_package_1" / "main.zip"
     )
     ireq = from_line(name_collision_1)
     deps = pypi_repository.get_dependencies(ireq)
     assert len(deps) == 0
 
     name_collision_2 = "file://{dist_path}#egg=test_package_2".format(
-        dist_path=tmpdir / "test_package_2" / "master.zip"
+        dist_path=tmpdir / "test_package_2" / "main.zip"
     )
     ireq = from_line(name_collision_2)
     deps = pypi_repository.get_dependencies(ireq)
     assert len(deps) == 1
     assert deps.pop().name == "test-package-1"
```

### Comparing `pip-tools-6.9.0/tests/test_resolver.py` & `pip-tools-7.0.0/tests/test_resolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 from pip._internal.exceptions import DistributionNotFound
 from pip._internal.utils.urls import path_to_url
 
 from piptools.exceptions import NoCandidateFound
 from piptools.resolver import RequirementSummary, combine_install_requirements
```

### Comparing `pip-tools-6.9.0/tests/test_sync.py` & `pip-tools-7.0.0/tests/test_sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import io
 import os
 import sys
 import tempfile
 from collections import Counter
 from unittest import mock
 
@@ -109,14 +111,34 @@
     ]
 
     assert Counter(requirements[1:]) == Counter(
         merge(requirements, ignore_conflicts=False)
     )
 
 
+@pytest.mark.parametrize(
+    "install_req",
+    (
+        "from_line",
+        "from_editable",
+    ),
+)
+def test_merge_no_name_urls(install_req, request):
+    install_req = request.getfixturevalue(install_req)
+    url = "file:///example.zip"
+    requirements = [
+        install_req(url),
+        install_req(url),
+    ]
+
+    assert Counter(requirements[1:]) == Counter(
+        merge(requirements, ignore_conflicts=False)
+    )
+
+
 def test_diff_should_do_nothing():
     installed = []  # empty env
     reqs = []  # no requirements
 
     to_install, to_uninstall = diff(reqs, installed)
     assert to_install == set()
     assert to_uninstall == set()
@@ -237,35 +259,49 @@
 
     assert len(to_install) == 1
     package = list(to_install)[0]
     assert package.editable
     assert package.link.url == path_to_url(path_to_package)
 
 
-def test_diff_with_matching_url_versions(fake_dist, from_line):
+def test_diff_with_matching_url_hash(fake_dist, from_line):
     # if URL version is explicitly provided, use it to avoid reinstalling
-    installed = [fake_dist("example==1.0")]
-    reqs = [from_line("file:///example.zip#egg=example==1.0")]
+    line = "example@file:///example.zip#sha1=abc"
+    installed = [fake_dist(line)]
+    reqs = [from_line(line)]
 
     to_install, to_uninstall = diff(reqs, installed)
     assert to_install == set()
     assert to_uninstall == set()
 
 
-def test_diff_with_no_url_versions(fake_dist, from_line):
-    # if URL version is not provided, assume the contents have
+def test_diff_with_no_url_hash(fake_dist, from_line):
+    # if URL hash is not provided, assume the contents have
     # changed and reinstall
-    installed = [fake_dist("example==1.0")]
-    reqs = [from_line("file:///example.zip#egg=example")]
+    line = "example@file:///example.zip"
+    installed = [fake_dist(line)]
+    reqs = [from_line(line)]
 
     to_install, to_uninstall = diff(reqs, installed)
     assert to_install == set(reqs)
     assert to_uninstall == {"example"}
 
 
+def test_diff_with_unequal_url_hash(fake_dist, from_line):
+    # if URL hashes mismatch, assume the contents have
+    # changed and reinstall
+    line = "example@file:///example.zip#"
+    installed = [fake_dist(line + "sha1=abc")]
+    reqs = [from_line(line + "sha1=def")]
+
+    to_install, to_uninstall = diff(reqs, installed)
+    assert to_install == set(reqs)
+    assert to_uninstall == {"example @ file:///example.zip#sha1=abc"}
+
+
 def test_sync_install_temporary_requirement_file(
     from_line, from_editable, mocked_tmp_req_file
 ):
     with mock.patch("piptools.sync.run") as run:
         to_install = {from_line("django==1.8")}
         sync(to_install, set())
         run.assert_called_once_with(
@@ -309,45 +345,39 @@
 def test_sync_requirement_file_with_hashes(
     from_line, from_editable, mocked_tmp_req_file
 ):
     with mock.patch("piptools.sync.run"):
         to_install = {
             from_line(
                 "django==1.8",
-                options={
-                    "hashes": {
-                        "sha256": [
-                            "6a03ce2feafdd193a0ba8a26dbd9773e"
-                            "757d2e5d5e7933a62eac129813bd381a"
-                        ]
-                    }
+                hash_options={
+                    "sha256": [
+                        "6a03ce2feafdd193a0ba8a26dbd9773e"
+                        "757d2e5d5e7933a62eac129813bd381a"
+                    ]
                 },
             ),
             from_line(
                 "click==4.0",
-                options={
-                    "hashes": {
-                        "sha256": [
-                            "9ab1d313f99b209f8f71a629f3683303"
-                            "0c8d7c72282cf7756834baf567dca662"
-                        ]
-                    }
+                hash_options={
+                    "sha256": [
+                        "9ab1d313f99b209f8f71a629f3683303"
+                        "0c8d7c72282cf7756834baf567dca662"
+                    ]
                 },
             ),
             from_line(
                 "pytz==2017.2",
-                options={
-                    "hashes": {
-                        "sha256": [
-                            "d1d6729c85acea542367138286862712"
-                            "9432fba9a89ecbb248d8d1c7a9f01c67",
-                            "f5c056e8f62d45ba8215e5cb8f50dfcc"
-                            "b198b4b9fbea8500674f3443e4689589",
-                        ]
-                    }
+                hash_options={
+                    "sha256": [
+                        "d1d6729c85acea542367138286862712"
+                        "9432fba9a89ecbb248d8d1c7a9f01c67",
+                        "f5c056e8f62d45ba8215e5cb8f50dfcc"
+                        "b198b4b9fbea8500674f3443e4689589",
+                    ]
                 },
             ),
         }
 
         sync(to_install, set())
 
         expected = (
```

### Comparing `pip-tools-6.9.0/tests/test_utils.py` & `pip-tools-7.0.0/tests/test_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,40 @@
+from __future__ import annotations
+
 import logging
 import operator
 import os
 import shlex
 import sys
+from pathlib import Path
 
 import pip
 import pytest
+from click import BadOptionUsage, Context, FileError
 from pip._vendor.packaging.version import Version
 
 from piptools.scripts.compile import cli as compile_cli
 from piptools.utils import (
     as_tuple,
     dedup,
     drop_extras,
     flat_map,
     format_requirement,
     format_specifier,
+    get_click_dest_for_option,
     get_compile_command,
     get_hashes_from_ireq,
     get_pip_version_for_python_executable,
     get_sys_path_for_python_executable,
     is_pinned_requirement,
     is_url_requirement,
     key_from_ireq,
     lookup_table,
     lookup_table_from_tuples,
+    override_defaults_from_config_file,
 )
 
 
 def test_format_requirement(from_line):
     ireq = from_line("test==1.2")
     assert format_requirement(ireq) == "test==1.2"
 
@@ -225,21 +231,19 @@
 def test_dedup():
     assert list(dedup([3, 1, 2, 4, 3, 5])) == [3, 1, 2, 4, 5]
 
 
 def test_get_hashes_from_ireq(from_line):
     ireq = from_line(
         "pytz==2017.2",
-        options={
-            "hashes": {
-                "sha256": [
-                    "d1d6729c85acea5423671382868627129432fba9a89ecbb248d8d1c7a9f01c67",
-                    "f5c056e8f62d45ba8215e5cb8f50dfccb198b4b9fbea8500674f3443e4689589",
-                ]
-            }
+        hash_options={
+            "sha256": [
+                "d1d6729c85acea5423671382868627129432fba9a89ecbb248d8d1c7a9f01c67",
+                "f5c056e8f62d45ba8215e5cb8f50dfccb198b4b9fbea8500674f3443e4689589",
+            ]
         },
     )
     expected = {
         "sha256:d1d6729c85acea5423671382868627129432fba9a89ecbb248d8d1c7a9f01c67",
         "sha256:f5c056e8f62d45ba8215e5cb8f50dfccb198b4b9fbea8500674f3443e4689589",
     }
     assert get_hashes_from_ireq(ireq) == expected
@@ -278,15 +282,15 @@
     ("line", "expected"),
     (
         ("django==1.8", False),
         ("django", False),
         ("file:///example.zip", True),
         ("https://example.com/example.zip", True),
         ("https://example.com/example.zip#egg=example", True),
-        ("git+https://github.com/jazzband/pip-tools@master", True),
+        ("git+https://github.com/jazzband/pip-tools@main", True),
     ),
 )
 def test_is_url_requirement(caplog, from_line, line, expected):
     ireq = from_line(line)
     assert is_url_requirement(ireq) is expected
 
 
@@ -378,14 +382,38 @@
     """
     Test general scenarios for the get_compile_command function.
     """
     with compile_cli.make_context("pip-compile", cli_args) as ctx:
         assert get_compile_command(ctx) == expected_command
 
 
+@pytest.mark.parametrize(
+    ("config_file", "expected_command"),
+    (
+        pytest.param(
+            "pyproject.toml", "pip-compile", id="exclude default pyproject.toml"
+        ),
+        pytest.param(
+            ".pip-tools.toml", "pip-compile", id="exclude default .pip-tools.toml"
+        ),
+        pytest.param(
+            "my-config.toml",
+            "pip-compile --config=my-config.toml",
+            id="include non-default my-config.toml",
+        ),
+    ),
+)
+def test_get_compile_command_with_config(tmpdir_cwd, config_file, expected_command):
+    """Test that get_compile_command excludes or includes config file."""
+    with open(config_file, "w"):
+        pass
+    with compile_cli.make_context("pip-compile", ["--config", config_file]) as ctx:
+        assert get_compile_command(ctx) == expected_command
+
+
 def test_get_compile_command_escaped_filenames(tmpdir_cwd):
     """
     Test that get_compile_command output (re-)escapes ' -- '-escaped filenames.
     """
     with open("--requirements.in", "w"):
         pass
     with compile_cli.make_context("pip-compile", ["--", "--requirements.in"]) as ctx:
@@ -536,7 +564,117 @@
 
 def test_get_sys_path_for_python_executable():
     result = get_sys_path_for_python_executable(sys.executable)
     assert result, "get_sys_path_for_python_executable should not return empty result"
     # not testing for equality, because pytest adds extra paths into current sys.path
     for path in result:
         assert path in sys.path
+
+
+@pytest.mark.parametrize(
+    ("pyproject_param", "new_default"),
+    (
+        # From sync
+        ("ask", True),
+        ("dry-run", True),
+        ("find-links", ["changed"]),
+        ("extra-index-url", ["changed"]),
+        ("trusted-host", ["changed"]),
+        ("no-index", True),
+        ("python-executable", "changed"),
+        ("verbose", True),
+        ("quiet", True),
+        ("user", True),
+        ("cert", "changed"),
+        ("client-cert", "changed"),
+        ("pip-args", "changed"),
+        # From compile, unless also in sync
+        ("pre", True),
+        ("rebuild", True),
+        ("extras", ["changed"]),
+        ("all-extras", True),
+        ("index-url", "changed"),
+        ("header", False),
+        ("emit-trusted-host", False),
+        ("annotate", False),
+        ("annotation-style", "line"),
+        ("upgrade", True),
+        ("upgrade-package", ["changed"]),
+        ("output-file", "changed"),
+        ("newline", "native"),
+        ("allow-unsafe", True),
+        ("strip-extras", True),
+        ("generate-hashes", True),
+        ("reuse-hashes", False),
+        ("max-rounds", 100),
+        ("build-isolation", False),
+        ("emit-find-links", False),
+        ("cache-dir", "changed"),
+        ("resolver", "backtracking"),
+        ("emit-index-url", False),
+        ("emit-options", False),
+        ("unsafe-package", ["changed"]),
+    ),
+)
+def test_callback_config_file_defaults(pyproject_param, new_default, make_config_file):
+    config_file = make_config_file(pyproject_param, new_default)
+    # Create a "compile" run example pointing to the config file
+    ctx = Context(compile_cli)
+    ctx.params["src_files"] = (str(config_file),)
+    found_config_file = override_defaults_from_config_file(ctx, "config", None)
+    assert found_config_file == config_file
+    # Make sure the default has been updated
+    lookup_param = get_click_dest_for_option(pyproject_param)
+    assert ctx.default_map[lookup_param] == new_default
+
+
+@pytest.mark.parametrize(
+    "mv_option",
+    (
+        "extra",
+        "upgrade-package",
+        "unsafe-package",
+        "find-links",
+        "extra-index-url",
+        "trusted-host",
+    ),
+)
+def test_callback_config_file_defaults_multi_value_options(mv_option, make_config_file):
+    config_file = make_config_file(mv_option, "not-a-list")
+    ctx = Context(compile_cli)
+    ctx.params["src_files"] = (str(config_file),)
+    with pytest.raises(BadOptionUsage, match="must be a list"):
+        override_defaults_from_config_file(ctx, "config", None)
+
+
+def test_callback_config_file_defaults_bad_toml(make_config_file):
+    config_file = make_config_file("verbose", True)
+    # Simple means of making invalid TOML: have duplicate keys
+    with Path(config_file).open("r+") as fs:
+        config_text_lines = fs.readlines()
+        fs.write(config_text_lines[-1])
+    ctx = Context(compile_cli)
+    ctx.params["src_files"] = (str(config_file),)
+    with pytest.raises(FileError, match="Could not parse "):
+        override_defaults_from_config_file(ctx, "config", None)
+
+
+def test_callback_config_file_defaults_precedence(make_config_file):
+    piptools_config_file = make_config_file("newline", "LF")
+    project_config_file = make_config_file("newline", "CRLF", "pyproject.toml")
+    ctx = Context(compile_cli)
+    ctx.params["src_files"] = (str(project_config_file),)
+    found_config_file = override_defaults_from_config_file(ctx, "config", None)
+    # The pip-tools specific config file should take precedence over pyproject.toml
+    assert found_config_file == piptools_config_file
+    lookup_param = get_click_dest_for_option("newline")
+    assert ctx.default_map[lookup_param] == "LF"
+
+
+def test_callback_config_file_defaults_unreadable_toml(make_config_file):
+    ctx = Context(compile_cli)
+    with pytest.raises(FileError, match="Could not read "):
+        override_defaults_from_config_file(
+            ctx,
+            "config",
+            "/dev/null/path/does/not/exist/my-config.toml",
+        )
```

### Comparing `pip-tools-6.9.0/tests/test_writer.py` & `pip-tools-7.0.0/tests/test_writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import sys
 
 import pytest
 from pip._internal.models.format_control import FormatControl
 
 from piptools.scripts.compile import cli
 from piptools.utils import comment
@@ -38,14 +40,15 @@
             annotate=True,
             annotation_style="split",
             generate_hashes=False,
             default_index_url=None,
             index_urls=[],
             trusted_hosts=[],
             format_control=FormatControl(set(), set()),
+            linesep="\n",
             allow_unsafe=False,
             find_links=[],
             emit_find_links=True,
             strip_extras=False,
             emit_options=True,
         )
         yield writer
@@ -106,15 +109,18 @@
 
 @pytest.mark.parametrize("allow_unsafe", ((True,), (False,)))
 def test_iter_lines__unsafe_dependencies(writer, from_line, allow_unsafe):
     writer.allow_unsafe = allow_unsafe
     writer.emit_header = False
 
     lines = writer._iter_lines(
-        [from_line("test==1.2")], [from_line("setuptools==1.10.0")]
+        {from_line("test==1.2")},
+        {from_line("setuptools==1.10.0")},
+        unsafe_packages=set(),
+        markers={},
     )
 
     expected_lines = (
         "test==1.2",
         "",
         MESSAGE_UNSAFE_PACKAGES,
         "setuptools==1.10.0" if allow_unsafe else comment("# setuptools"),
@@ -125,15 +131,17 @@
 def test_iter_lines__unsafe_with_hashes(capsys, writer, from_line):
     writer.allow_unsafe = False
     writer.emit_header = False
     ireqs = [from_line("test==1.2")]
     unsafe_ireqs = [from_line("setuptools==1.10.0")]
     hashes = {ireqs[0]: {"FAKEHASH"}, unsafe_ireqs[0]: set()}
 
-    lines = writer._iter_lines(ireqs, unsafe_ireqs, hashes=hashes)
+    lines = writer._iter_lines(
+        ireqs, unsafe_ireqs, unsafe_packages=set(), markers={}, hashes=hashes
+    )
 
     expected_lines = (
         "test==1.2 \\\n    --hash=FAKEHASH",
         "",
         MESSAGE_UNSAFE_PACKAGES_UNPINNED,
         comment("# setuptools"),
     )
@@ -145,15 +153,21 @@
 
 def test_iter_lines__hash_missing(capsys, writer, from_line):
     writer.allow_unsafe = False
     writer.emit_header = False
     ireqs = [from_line("test==1.2"), from_line("file:///example/#egg=example")]
     hashes = {ireqs[0]: {"FAKEHASH"}, ireqs[1]: set()}
 
-    lines = writer._iter_lines(ireqs, hashes=hashes)
+    lines = writer._iter_lines(
+        ireqs,
+        hashes=hashes,
+        unsafe_requirements=set(),
+        unsafe_packages=set(),
+        markers={},
+    )
 
     expected_lines = (
         MESSAGE_UNHASHED_PACKAGE,
         "example @ file:///example/",
         "test==1.2 \\\n    --hash=FAKEHASH",
     )
     assert tuple(lines) == expected_lines
@@ -171,31 +185,37 @@
     writer.emit_header = False
     ireqs = [
         from_line("file:///unhashable-pkg1/#egg=unhashable-pkg1"),
         from_line("file:///unhashable-pkg2/#egg=unhashable-pkg2"),
     ]
     hashes = {ireq: set() for ireq in ireqs}
 
-    lines = writer._iter_lines(ireqs, hashes=hashes)
+    lines = writer._iter_lines(
+        ireqs,
+        hashes=hashes,
+        unsafe_requirements=set(),
+        unsafe_packages=set(),
+        markers={},
+    )
 
     expected_lines = (
         "unhashable-pkg1 @ file:///unhashable-pkg1/",
         "unhashable-pkg2 @ file:///unhashable-pkg2/",
     )
     assert tuple(lines) == expected_lines
 
 
 def test_write_header(writer):
     expected = map(
         comment,
         [
             "#",
-            "# This file is autogenerated by pip-compile with python "
+            "# This file is autogenerated by pip-compile with Python "
             f"{sys.version_info.major}.{sys.version_info.minor}",
-            "# To update, run:",
+            "# by the following command:",
             "#",
             "#    pip-compile --output-file={} src_file src_file2".format(
                 writer.click_ctx.params["output_file"].name
             ),
             "#",
         ],
     )
@@ -204,17 +224,17 @@
 
 def test_write_header_custom_compile_command(writer, monkeypatch):
     monkeypatch.setenv("CUSTOM_COMPILE_COMMAND", "./pipcompilewrapper")
     expected = map(
         comment,
         [
             "#",
-            "# This file is autogenerated by pip-compile with python "
+            "# This file is autogenerated by pip-compile with Python "
             f"{sys.version_info.major}.{sys.version_info.minor}",
-            "# To update, run:",
+            "# by the following command:",
             "#",
             "#    ./pipcompilewrapper",
             "#",
         ],
     )
     assert list(writer.write_header()) == list(expected)
 
@@ -382,20 +402,23 @@
 def test_write_order(writer, from_line):
     """
     Order of packages should match that of `pip freeze`, with the exception
     that requirement names should be canonicalized.
     """
     writer.emit_header = False
 
-    packages = [
+    packages = {
         from_line("package_a==0.1"),
         from_line("Package-b==2.3.4"),
         from_line("Package==5.6"),
         from_line("package2==7.8.9"),
-    ]
+    }
     expected_lines = [
         "package==5.6",
         "package-a==0.1",
         "package-b==2.3.4",
         "package2==7.8.9",
     ]
-    assert list(writer._iter_lines(packages)) == expected_lines
+    result = writer._iter_lines(
+        packages, unsafe_requirements=set(), unsafe_packages=set(), markers={}
+    )
+    assert list(result) == expected_lines
```

### Comparing `pip-tools-6.9.0/tox.ini` & `pip-tools-7.0.0/tox.ini`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,65 @@
 [tox]
 envlist =
     # NOTE: keep this in sync with the env list in .github/workflows/ci.yml.
-    py{37,38,39,310,311,py3}-pip{previous,latest,main}-coverage
+    py{37,38,39,310,311,312,py3}-pip{previous,latest,main}-coverage
     checkqa
     readme
 skip_missing_interpreters = True
 
 [testenv]
+description = run the tests with pytest
 extras =
     testing
     coverage: coverage
 deps =
-    pipprevious: pip==21.3.*
+    pipprevious: pip==22.2.*
     piplatest: pip
-    pipmain: -e git+https://github.com/pypa/pip.git@main#egg=pip
+    pipmain: https://github.com/pypa/pip/archive/main.zip
 setenv =
     coverage: PYTEST_ADDOPTS=--strict-markers --doctest-modules --cov --cov-report=term-missing --cov-report=xml {env:PYTEST_ADDOPTS:}
 commands_pre =
     piplatest: python -m pip install -U pip
     pip --version
 commands = pytest {posargs}
-passenv = CI GITHUB_ACTIONS
+passenv =
+    CI
+    FORCE_COLOR
+    GITHUB_ACTIONS
+    MYPY_FORCE_COLOR
+    PRE_COMMIT_COLOR
+    PY_COLORS
 pip_pre=True
 
 [testenv:checkqa]
+description = format the code base and check its quality
 skip_install = True
 deps = pre-commit
 commands_pre =
 commands = pre-commit run --all-files --show-diff-on-failure
 
 [testenv:readme]
-deps = twine
+description = check whether the long description will render correctly on PyPI
+deps =
+    build
+    twine
 commands_pre =
-commands = twine check {distdir}/*
+commands =
+    python -m build --outdir {envtmpdir} --sdist {toxinidir}
+    twine check --strict {envtmpdir}{/}*
+skip_install = true
 
 [testenv:build-docs]
-basepython = python3
+description = build the documentation
 deps =
   -r{toxinidir}/docs/requirements.txt
   # FIXME: re-enable the "-r" + "-c" paradigm once the pip bug is fixed.
   # Ref: https://github.com/pypa/pip/issues/9243
   # -r{toxinidir}/docs/requirements.in
   # -c{toxinidir}/docs/requirements.txt
-description = Build The Docs
 commands_pre =
 commands =
   # Retrieve possibly missing commits:
   -git fetch --unshallow
   -git fetch --tags
 
   # Build the html docs with Sphinx:
@@ -72,26 +85,56 @@
   \N\{QUOTATION MARK\}\{docs_dir\}\N\{QUOTATION MARK\} 0\n\n" +\
   "=" * 120)'
 changedir = {toxinidir}/docs
 isolated_build = true
 passenv =
   SSH_AUTH_SOCK
 skip_install = true
-whitelist_externals =
+allowlist_externals =
   git
 
+
+[testenv:preview-docs]
+description = preview the docs
+deps =
+  sphinx-autobuild
+  {[testenv:build-docs]deps}
+commands_pre =
+commands =
+  # Retrieve possibly missing commits:
+  -git fetch --unshallow
+  -git fetch --tags
+
+  # Build the html docs with sphinx-autobuild:
+  {envpython} -m sphinx_autobuild \
+    -j auto \
+    -b html \
+    -n \
+    -W \
+    -d "{temp_dir}/.doctrees" \
+    . \
+    --watch ../README.rst \
+    --watch ../CHANGELOG.md \
+    "{envdir}/docs_out"
+
+changedir = {[testenv:build-docs]changedir}
+isolated_build = {[testenv:build-docs]isolated_build}
+passenv = {[testenv:build-docs]passenv}
+skip_install = {[testenv:build-docs]skip_install}
+allowlist_externals = {[testenv:build-docs]allowlist_externals}
+
+
 [testenv:linkcheck-docs]
-basepython = python3
+description = check links in the documentation
 deps =
   -r{toxinidir}/docs/requirements.txt
   # FIXME: re-enable the "-r" + "-c" paradigm once the pip bug is fixed.
   # Ref: https://github.com/pypa/pip/issues/9243
   # -r{toxinidir}/docs/requirements.in
   # -c{toxinidir}/docs/requirements.txt
-description = Linkcheck The Docs
 commands_pre =
 commands =
   # Retrieve possibly missing commits:
   -git fetch --unshallow
   -git fetch --tags
 
   # Build the html docs with Sphinx:
@@ -105,9 +148,9 @@
     . \
     "{envdir}/docs_out"
 changedir = {toxinidir}/docs
 isolated_build = true
 passenv =
   SSH_AUTH_SOCK
 skip_install = true
-whitelist_externals =
+allowlist_externals =
   git
```

