# Comparing `tmp/repository_service_tuf-0.3.0a1.tar.gz` & `tmp/repository_service_tuf-0.4.0b1.tar.gz`

## Comparing `repository_service_tuf-0.3.0a1.tar` & `repository_service_tuf-0.4.0b1.tar`

### file list

```diff
@@ -1,80 +1,83 @@
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.gitignore
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.readthedocs.yaml
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/CODE_OF_CONDUCT.rst
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/LICENSE
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/MAINTAINERS.rst
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/Makefile
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/Pipfile
--rw-r--r--   0        0        0    80650 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/Pipfile.lock
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/README.rst
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/pyproject.toml
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/requirements-dev.txt
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/requirements.txt
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tox.ini
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.github/dependabot.yml
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.github/ISSUE_TEMPLATE/other.yml
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.github/ISSUE_TEMPLATE/task.yml
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.github/PULL_REQUEST_TEMPLATE/pr.yml
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.github/workflows/cd.yml
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.github/workflows/update-python-deps.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/make.bat
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/requirements.txt
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/diagrams/repository-service-tuf-cli-C1.puml
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/diagrams/repository-service-tuf-cli-C2.puml
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/diagrams/repository-service-tuf-cli-C3.puml
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/conf.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/index.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/_static/INFO
--rw-r--r--   0        0        0    19648 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/_static/repository-service-tuf-cli-C1.png
--rw-r--r--   0        0        0    41916 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/_static/repository-service-tuf-cli-C2.png
--rw-r--r--   0        0        0    94852 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/_static/repository-service-tuf-cli-C3.png
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/devel/design.rst
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/devel/index.rst
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/devel/modules.rst
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/devel/repository_service_tuf.cli.admin.rst
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/devel/repository_service_tuf.cli.key.rst
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/devel/repository_service_tuf.cli.rst
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/devel/repository_service_tuf.helpers.rst
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/devel/repository_service_tuf.rst
--rw-r--r--   0        0        0    48362 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/guide/index.rst
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/__version__.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/constants.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/cli/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/cli/admin/__init__.py
--rw-r--r--   0        0        0    25461 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/cli/admin/ceremony.py
--rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/cli/admin/import_targets.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/cli/admin/login.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/cli/admin/token.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/cli/key/__init__.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/cli/key/generate_key.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/helpers/__init__.py
--rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/helpers/api_client.py
--rw-r--r--   0        0        0     8014 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/helpers/tuf.py
--rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/conftest.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/test_tuf_repository_service.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/files/README.md
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/files/key_storage/JanisJoplin.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/files/key_storage/JanisJoplin.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/files/key_storage/JimiHendrix.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/files/key_storage/JimiHendrix.pub
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/files/key_storage/online-rsa.key
--rwxr-xr-x   0        0        0      624 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/files/key_storage/online-rsa.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/files/key_storage/online.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/files/key_storage/online.pub
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/unit/cli/test__init__.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/unit/cli/admin/__init__.py
--rw-r--r--   0        0        0    32354 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/unit/cli/admin/test_ceremony.py
--rw-r--r--   0        0        0    15993 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/unit/cli/admin/test_import_targets.py
--rw-r--r--   0        0        0    12272 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/unit/cli/admin/test_login.py
--rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/unit/cli/key/test_generate_key.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/unit/helpers/__init__.py
--rw-r--r--   0        0        0    21413 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/unit/helpers/test_api_client.py
--rw-r--r--   0        0        0    13747 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/unit/helpers/test_tuf.py
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.gitignore
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.readthedocs.yaml
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/LICENSE
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/MAINTAINERS.rst
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/Makefile
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/Pipfile
+-rw-r--r--   0        0        0    82238 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/Pipfile.lock
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/README.rst
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/pyproject.toml
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/requirements-dev.txt
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/requirements.txt
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tox.ini
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.github/ISSUE_TEMPLATE/other.yml
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.github/ISSUE_TEMPLATE/task.yml
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.github/PULL_REQUEST_TEMPLATE/pr.yml
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.github/workflows/cd.yml
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/.github/workflows/update-python-deps.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/make.bat
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/requirements.txt
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/diagrams/repository-service-tuf-cli-C1.puml
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/diagrams/repository-service-tuf-cli-C2.puml
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/diagrams/repository-service-tuf-cli-C3.puml
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/conf.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/_static/INFO
+-rw-r--r--   0        0        0    19648 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/_static/repository-service-tuf-cli-C1.png
+-rw-r--r--   0        0        0    41916 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/_static/repository-service-tuf-cli-C2.png
+-rw-r--r--   0        0        0   108509 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/_static/repository-service-tuf-cli-C3.png
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/devel/design.rst
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/devel/index.rst
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/devel/modules.rst
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/devel/repository_service_tuf.cli.admin.rst
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/devel/repository_service_tuf.cli.key.rst
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/devel/repository_service_tuf.cli.rst
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/devel/repository_service_tuf.helpers.rst
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/devel/repository_service_tuf.rst
+-rw-r--r--   0        0        0    79560 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/docs/source/guide/index.rst
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/__version__.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/constants.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/cli/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/__init__.py
+-rw-r--r--   0        0        0    23494 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/ceremony.py
+-rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/import_targets.py
+-rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/login.py
+-rw-r--r--   0        0        0    17959 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/metadata.py
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/token.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/cli/key/__init__.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/cli/key/generate_key.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/helpers/__init__.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/helpers/api_client.py
+-rw-r--r--   0        0        0    16677 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/repository_service_tuf/helpers/tuf.py
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/conftest.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/test_tuf_repository_service.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/files/README.md
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/files/root.json
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/files/key_storage/JanisJoplin.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/files/key_storage/JanisJoplin.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/files/key_storage/JimiHendrix.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/files/key_storage/JimiHendrix.pub
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/files/key_storage/online-rsa.key
+-rwxr-xr-x   0        0        0      624 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/files/key_storage/online-rsa.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/files/key_storage/online.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/files/key_storage/online.pub
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/unit/cli/test__init__.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/unit/cli/admin/__init__.py
+-rw-r--r--   0        0        0    24147 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/unit/cli/admin/test_ceremony.py
+-rw-r--r--   0        0        0    16749 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/unit/cli/admin/test_import_targets.py
+-rw-r--r--   0        0        0    11163 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/unit/cli/admin/test_login.py
+-rw-r--r--   0        0        0    29849 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/unit/cli/admin/test_metadata_update.py
+-rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/unit/cli/key/test_generate_key.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/unit/helpers/__init__.py
+-rw-r--r--   0        0        0    30868 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/unit/helpers/test_api_client.py
+-rw-r--r--   0        0        0    28947 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/tests/unit/helpers/test_tuf.py
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 repository_service_tuf-0.4.0b1/PKG-INFO
```

### Comparing `repository_service_tuf-0.3.0a1/.gitignore` & `repository_service_tuf-0.4.0b1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -128,10 +128,11 @@
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
 payload.json
+metadata-update-payload.json
 
 # VScode settings folder
 .vscode
```

### Comparing `repository_service_tuf-0.3.0a1/.pre-commit-config.yaml` & `repository_service_tuf-0.4.0b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/.readthedocs.yaml` & `repository_service_tuf-0.4.0b1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/CODE_OF_CONDUCT.rst` & `repository_service_tuf-0.4.0b1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/CONTRIBUTING.rst` & `repository_service_tuf-0.4.0b1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/LICENSE` & `repository_service_tuf-0.4.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/Pipfile` & `repository_service_tuf-0.4.0b1/Pipfile`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/Pipfile.lock` & `repository_service_tuf-0.4.0b1/Pipfile.lock`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9734259259259259%*

 * *Differences: {"'default'": "{'charset-normalizer': {'hashes': "*

 * *              "['sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96', "*

 * *              "'sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c', "*

 * *              "'sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710', "*

 * *              "'sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706', "*

 * *              "'sha256:1249cbbf3d3b04902ff081ffbb33ce3377fa6e4c7356f759f3cd076cc138d020', "*

 * * […]*

```diff
@@ -91,143 +91,147 @@
                 "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
                 "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
             ],
             "version": "==1.15.1"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
-                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
-                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
-                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
-                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
-                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
-                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
-                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
-                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
-                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
-                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
-                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
-                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
-                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
-                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
-                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
-                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
-                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
-                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
-                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
-                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
-                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
-                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
-                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
-                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
-                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
-                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
-                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
-                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
-                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
-                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
-                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
-                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
-                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
-                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
-                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
-                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
-                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
-                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
-                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
-                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
-                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
-                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
-                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
-                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
-                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
-                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
-                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
-                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
-                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
-                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
-                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
-                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
-                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
-                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
-                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
-                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
-                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
-                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
-                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
-                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
-                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
-                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
-                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
-                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
-                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
-                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
-                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
-                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
-                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
-                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
-                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
-                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
-                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
-                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
+                "sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96",
+                "sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c",
+                "sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710",
+                "sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706",
+                "sha256:1249cbbf3d3b04902ff081ffbb33ce3377fa6e4c7356f759f3cd076cc138d020",
+                "sha256:1920d4ff15ce893210c1f0c0e9d19bfbecb7983c76b33f046c13a8ffbd570252",
+                "sha256:193cbc708ea3aca45e7221ae58f0fd63f933753a9bfb498a3b474878f12caaad",
+                "sha256:1a100c6d595a7f316f1b6f01d20815d916e75ff98c27a01ae817439ea7726329",
+                "sha256:1f30b48dd7fa1474554b0b0f3fdfdd4c13b5c737a3c6284d3cdc424ec0ffff3a",
+                "sha256:203f0c8871d5a7987be20c72442488a0b8cfd0f43b7973771640fc593f56321f",
+                "sha256:246de67b99b6851627d945db38147d1b209a899311b1305dd84916f2b88526c6",
+                "sha256:2dee8e57f052ef5353cf608e0b4c871aee320dd1b87d351c28764fc0ca55f9f4",
+                "sha256:2efb1bd13885392adfda4614c33d3b68dee4921fd0ac1d3988f8cbb7d589e72a",
+                "sha256:2f4ac36d8e2b4cc1aa71df3dd84ff8efbe3bfb97ac41242fbcfc053c67434f46",
+                "sha256:3170c9399da12c9dc66366e9d14da8bf7147e1e9d9ea566067bbce7bb74bd9c2",
+                "sha256:3b1613dd5aee995ec6d4c69f00378bbd07614702a315a2cf6c1d21461fe17c23",
+                "sha256:3bb3d25a8e6c0aedd251753a79ae98a093c7e7b471faa3aa9a93a81431987ace",
+                "sha256:3bb7fda7260735efe66d5107fb7e6af6a7c04c7fce9b2514e04b7a74b06bf5dd",
+                "sha256:41b25eaa7d15909cf3ac4c96088c1f266a9a93ec44f87f1d13d4a0e86c81b982",
+                "sha256:45de3f87179c1823e6d9e32156fb14c1927fcc9aba21433f088fdfb555b77c10",
+                "sha256:46fb8c61d794b78ec7134a715a3e564aafc8f6b5e338417cb19fe9f57a5a9bf2",
+                "sha256:48021783bdf96e3d6de03a6e39a1171ed5bd7e8bb93fc84cc649d11490f87cea",
+                "sha256:4957669ef390f0e6719db3613ab3a7631e68424604a7b448f079bee145da6e09",
+                "sha256:5e86d77b090dbddbe78867a0275cb4df08ea195e660f1f7f13435a4649e954e5",
+                "sha256:6339d047dab2780cc6220f46306628e04d9750f02f983ddb37439ca47ced7149",
+                "sha256:681eb3d7e02e3c3655d1b16059fbfb605ac464c834a0c629048a30fad2b27489",
+                "sha256:6c409c0deba34f147f77efaa67b8e4bb83d2f11c8806405f76397ae5b8c0d1c9",
+                "sha256:7095f6fbfaa55defb6b733cfeb14efaae7a29f0b59d8cf213be4e7ca0b857b80",
+                "sha256:70c610f6cbe4b9fce272c407dd9d07e33e6bf7b4aa1b7ffb6f6ded8e634e3592",
+                "sha256:72814c01533f51d68702802d74f77ea026b5ec52793c791e2da806a3844a46c3",
+                "sha256:7a4826ad2bd6b07ca615c74ab91f32f6c96d08f6fcc3902ceeedaec8cdc3bcd6",
+                "sha256:7c70087bfee18a42b4040bb9ec1ca15a08242cf5867c58726530bdf3945672ed",
+                "sha256:855eafa5d5a2034b4621c74925d89c5efef61418570e5ef9b37717d9c796419c",
+                "sha256:8700f06d0ce6f128de3ccdbc1acaea1ee264d2caa9ca05daaf492fde7c2a7200",
+                "sha256:89f1b185a01fe560bc8ae5f619e924407efca2191b56ce749ec84982fc59a32a",
+                "sha256:8b2c760cfc7042b27ebdb4a43a4453bd829a5742503599144d54a032c5dc7e9e",
+                "sha256:8c2f5e83493748286002f9369f3e6607c565a6a90425a3a1fef5ae32a36d749d",
+                "sha256:8e098148dd37b4ce3baca71fb394c81dc5d9c7728c95df695d2dca218edf40e6",
+                "sha256:94aea8eff76ee6d1cdacb07dd2123a68283cb5569e0250feab1240058f53b623",
+                "sha256:95eb302ff792e12aba9a8b8f8474ab229a83c103d74a750ec0bd1c1eea32e669",
+                "sha256:9bd9b3b31adcb054116447ea22caa61a285d92e94d710aa5ec97992ff5eb7cf3",
+                "sha256:9e608aafdb55eb9f255034709e20d5a83b6d60c054df0802fa9c9883d0a937aa",
+                "sha256:a103b3a7069b62f5d4890ae1b8f0597618f628b286b03d4bc9195230b154bfa9",
+                "sha256:a386ebe437176aab38c041de1260cd3ea459c6ce5263594399880bbc398225b2",
+                "sha256:a38856a971c602f98472050165cea2cdc97709240373041b69030be15047691f",
+                "sha256:a401b4598e5d3f4a9a811f3daf42ee2291790c7f9d74b18d75d6e21dda98a1a1",
+                "sha256:a7647ebdfb9682b7bb97e2a5e7cb6ae735b1c25008a70b906aecca294ee96cf4",
+                "sha256:aaf63899c94de41fe3cf934601b0f7ccb6b428c6e4eeb80da72c58eab077b19a",
+                "sha256:b0dac0ff919ba34d4df1b6131f59ce95b08b9065233446be7e459f95554c0dc8",
+                "sha256:baacc6aee0b2ef6f3d308e197b5d7a81c0e70b06beae1f1fcacffdbd124fe0e3",
+                "sha256:bf420121d4c8dce6b889f0e8e4ec0ca34b7f40186203f06a946fa0276ba54029",
+                "sha256:c04a46716adde8d927adb9457bbe39cf473e1e2c2f5d0a16ceb837e5d841ad4f",
+                "sha256:c0b21078a4b56965e2b12f247467b234734491897e99c1d51cee628da9786959",
+                "sha256:c1c76a1743432b4b60ab3358c937a3fe1341c828ae6194108a94c69028247f22",
+                "sha256:c4983bf937209c57240cff65906b18bb35e64ae872da6a0db937d7b4af845dd7",
+                "sha256:c4fb39a81950ec280984b3a44f5bd12819953dc5fa3a7e6fa7a80db5ee853952",
+                "sha256:c57921cda3a80d0f2b8aec7e25c8aa14479ea92b5b51b6876d975d925a2ea346",
+                "sha256:c8063cf17b19661471ecbdb3df1c84f24ad2e389e326ccaf89e3fb2484d8dd7e",
+                "sha256:ccd16eb18a849fd8dcb23e23380e2f0a354e8daa0c984b8a732d9cfaba3a776d",
+                "sha256:cd6dbe0238f7743d0efe563ab46294f54f9bc8f4b9bcf57c3c666cc5bc9d1299",
+                "sha256:d62e51710986674142526ab9f78663ca2b0726066ae26b78b22e0f5e571238dd",
+                "sha256:db901e2ac34c931d73054d9797383d0f8009991e723dab15109740a63e7f902a",
+                "sha256:e03b8895a6990c9ab2cdcd0f2fe44088ca1c65ae592b8f795c3294af00a461c3",
+                "sha256:e1c8a2f4c69e08e89632defbfabec2feb8a8d99edc9f89ce33c4b9e36ab63037",
+                "sha256:e4b749b9cc6ee664a3300bb3a273c1ca8068c46be705b6c31cf5d276f8628a94",
+                "sha256:e6a5bf2cba5ae1bb80b154ed68a3cfa2fa00fde979a7f50d6598d3e17d9ac20c",
+                "sha256:e857a2232ba53ae940d3456f7533ce6ca98b81917d47adc3c7fd55dad8fab858",
+                "sha256:ee4006268ed33370957f55bf2e6f4d263eaf4dc3cfc473d1d90baff6ed36ce4a",
+                "sha256:eef9df1eefada2c09a5e7a40991b9fc6ac6ef20b1372abd48d2794a316dc0449",
+                "sha256:f058f6963fd82eb143c692cecdc89e075fa0828db2e5b291070485390b2f1c9c",
+                "sha256:f25c229a6ba38a35ae6e25ca1264621cc25d4d38dca2942a7fce0b67a4efe918",
+                "sha256:f2a1d0fd4242bd8643ce6f98927cf9c04540af6efa92323e9d3124f57727bfc1",
+                "sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c",
+                "sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac",
+                "sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==3.1.0"
+            "version": "==3.2.0"
         },
         "click": {
             "hashes": [
-                "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
-                "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
+                "sha256:4be4b1af8d665c6d942909916d31a213a106800c47d0eeba73d34da3cbc11367",
+                "sha256:e576aa487d679441d7d30abb87e1b43d24fc53bffb8758443b1a9e1cee504548"
             ],
             "index": "pypi",
-            "version": "==8.1.3"
+            "version": "==8.1.5"
         },
         "configobj": {
             "hashes": [
                 "sha256:6f704434a07dc4f4dc7c9a745172c1cad449feb548febd9f7fe362629c627a97",
                 "sha256:a7a8c6ab7daade85c3f329931a807c8aee750a2494363934f8ea84d8a54c87ea",
                 "sha256:d808d7e04e6f81fbb23d5ac2cd50e69ccbee58eaf9360eb89ede22d93216a314"
             ],
             "version": "==5.0.8"
         },
         "cryptography": {
             "hashes": [
-                "sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440",
-                "sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288",
-                "sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b",
-                "sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958",
-                "sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b",
-                "sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d",
-                "sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a",
-                "sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404",
-                "sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b",
-                "sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e",
-                "sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2",
-                "sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c",
-                "sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b",
-                "sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9",
-                "sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b",
-                "sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636",
-                "sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99",
-                "sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e",
-                "sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9"
+                "sha256:01f1d9e537f9a15b037d5d9ee442b8c22e3ae11ce65ea1f3316a41c78756b711",
+                "sha256:079347de771f9282fbfe0e0236c716686950c19dee1b76240ab09ce1624d76d7",
+                "sha256:182be4171f9332b6741ee818ec27daff9fb00349f706629f5cbf417bd50e66fd",
+                "sha256:192255f539d7a89f2102d07d7375b1e0a81f7478925b3bc2e0549ebf739dae0e",
+                "sha256:2a034bf7d9ca894720f2ec1d8b7b5832d7e363571828037f9e0c4f18c1b58a58",
+                "sha256:342f3767e25876751e14f8459ad85e77e660537ca0a066e10e75df9c9e9099f0",
+                "sha256:439c3cc4c0d42fa999b83ded80a9a1fb54d53c58d6e59234cfe97f241e6c781d",
+                "sha256:49c3222bb8f8e800aead2e376cbef687bc9e3cb9b58b29a261210456a7783d83",
+                "sha256:674b669d5daa64206c38e507808aae49904c988fa0a71c935e7006a3e1e83831",
+                "sha256:7a9a3bced53b7f09da251685224d6a260c3cb291768f54954e28f03ef14e3766",
+                "sha256:7af244b012711a26196450d34f483357e42aeddb04128885d95a69bd8b14b69b",
+                "sha256:7d230bf856164de164ecb615ccc14c7fc6de6906ddd5b491f3af90d3514c925c",
+                "sha256:84609ade00a6ec59a89729e87a503c6e36af98ddcd566d5f3be52e29ba993182",
+                "sha256:9a6673c1828db6270b76b22cc696f40cde9043eb90373da5c2f8f2158957f42f",
+                "sha256:9b6d717393dbae53d4e52684ef4f022444fc1cce3c48c38cb74fca29e1f08eaa",
+                "sha256:9c3fe6534d59d071ee82081ca3d71eed3210f76ebd0361798c74abc2bcf347d4",
+                "sha256:a719399b99377b218dac6cf547b6ec54e6ef20207b6165126a280b0ce97e0d2a",
+                "sha256:b332cba64d99a70c1e0836902720887fb4529ea49ea7f5462cf6640e095e11d2",
+                "sha256:d124682c7a23c9764e54ca9ab5b308b14b18eba02722b8659fb238546de83a76",
+                "sha256:d73f419a56d74fef257955f51b18d046f3506270a5fd2ac5febbfa259d6c0fa5",
+                "sha256:f0dc40e6f7aa37af01aba07277d3d64d5a03dc66d682097541ec4da03cc140ee",
+                "sha256:f14ad275364c8b4e525d018f6716537ae7b6d369c094805cae45300847e0894f",
+                "sha256:f772610fe364372de33d76edcd313636a25684edb94cee53fd790195f5989d14"
             ],
-            "version": "==40.0.2"
+            "version": "==41.0.2"
         },
         "dynaconf": {
             "extras": [
                 "ini"
             ],
             "hashes": [
-                "sha256:11a60bcd735f82b8a47b288f99e4ffbbd08c6c130a7be93c5d03e93fc260a5e1",
-                "sha256:a79d7b3ad4a35af9b576c49f11cd3b23a1b04b87b63a4e9f92cc82f2b0cafeeb"
+                "sha256:791d8029c74548d57b0266aabd6557ebfff6540bffd7f58ba700f577c047c0f5",
+                "sha256:a28442d12860a44fad5fa1d9db918c710cbfc971e8b7694697429fb8f1c3c620"
             ],
             "index": "pypi",
-            "version": "==3.1.12"
+            "version": "==3.2.0"
         },
         "greenlet": {
             "hashes": [
                 "sha256:03a8f4f3430c3b3ff8d10a2a86028c660355ab637cee9333d63d66b56f09d52a",
                 "sha256:0bf60faf0bc2468089bdc5edd10555bab6e85152191df713e2ab1fcc86382b5a",
                 "sha256:18a7f18b82b52ee85322d7a7874e676f34ab319b9f8cce5de06067384aa8ff43",
                 "sha256:18e98fb3de7dba1c0a852731c3070cf022d14f0d68b4c87a19cc1016f3bb8b33",
@@ -305,19 +309,19 @@
                 "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"
             ],
             "index": "pypi",
             "version": "==5.12.0"
         },
         "markdown-it-py": {
             "hashes": [
-                "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30",
-                "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"
+                "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1",
+                "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2.2.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.0.0"
         },
         "mdurl": {
             "hashes": [
                 "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
                 "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
             ],
             "markers": "python_version >= '3.7'",
@@ -371,27 +375,27 @@
                 "sha256:e46dae94e34b085175f8abb3b0aaa7da40767865ac82c928eeb9e57e1ea8a543"
             ],
             "index": "pypi",
             "version": "==1.5.0"
         },
         "requests": {
             "hashes": [
-                "sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294",
-                "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
-            "version": "==2.30.0"
+            "version": "==2.31.0"
         },
         "rich": {
             "hashes": [
-                "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c",
-                "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"
+                "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
+                "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
             "index": "pypi",
-            "version": "==13.3.5"
+            "version": "==13.4.2"
         },
         "rich-click": {
             "hashes": [
                 "sha256:0fcf4d1a09029d79322dd814ab0b2e66ac183633037561881d45abae8a161d95",
                 "sha256:f8ff96693ec6e261d1544e9f7d9a5811c5ef5d74c8adb4978430fc0dac16777e"
             ],
             "index": "pypi",
@@ -414,82 +418,82 @@
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
         },
         "sqlalchemy": {
             "hashes": [
-                "sha256:0aa2cbde85a6eab9263ab480f19e8882d022d30ebcdc14d69e6a8d7c07b0a871",
-                "sha256:0d6979c9707f8b82366ba34b38b5a6fe32f75766b2e901f9820e271e95384070",
-                "sha256:0eb14a386a5b610305bec6639b35540b47f408b0a59f75999199aed5b3d40079",
-                "sha256:2424a84f131901fbb20a99844d47b38b517174c6e964c8efb15ea6bb9ced8c2b",
-                "sha256:2ad9688debf1f0ae9c6e0706a4e2d33b1a01281317cee9bd1d7eef8020c5baac",
-                "sha256:2f0a355264af0952570f18457102984e1f79510f856e5e0ae652e63316d1ca23",
-                "sha256:31f72bb300eed7bfdb373c7c046121d84fa0ae6f383089db9505ff553ac27cef",
-                "sha256:375b7ba88f261dbd79d044f20cbcd919d88befb63f26af9d084614f10cdf97a6",
-                "sha256:37de4010f53f452e94e5ed6684480432cfe6a7a8914307ef819cd028b05b98d5",
-                "sha256:49c138856035cb97f0053e5e57ba90ec936b28a0b8b0020d44965c7b0c0bf03a",
-                "sha256:4f9832815257969b3ca9bf0501351e4c02c8d60cbd3ec9f9070d5b0f8852900e",
-                "sha256:566a0ac347cf4632f551e7b28bbd0d215af82e6ffaa2556f565a3b6b51dc3f81",
-                "sha256:6777673d346071451bf7cccf8d0499024f1bd6a835fc90b4fe7af50373d92ce6",
-                "sha256:72746ec17a7d9c5acf2c57a6e6190ceba3dad7127cd85bb17f24e90acc0e8e3f",
-                "sha256:755f653d693f9b8f4286d987aec0d4279821bf8d179a9de8e8a5c685e77e57d6",
-                "sha256:7612a7366a0855a04430363fb4ab392dc6818aaece0b2e325ff30ee77af9b21f",
-                "sha256:7ad24c85f2a1caf0cd1ae8c2fdb668777a51a02246d9039420f94bd7dbfd37ed",
-                "sha256:881cc388dded44ae6e17a1666364b98bd76bcdc71b869014ae725f06ba298e0e",
-                "sha256:8d97b37b4e60073c38bcf94e289e3be09ef9be870de88d163f16e08f2b9ded1a",
-                "sha256:9119795d2405eb23bf7e6707e228fe38124df029494c1b3576459aa3202ea432",
-                "sha256:9136d596111c742d061c0f99bab95c5370016c4101a32e72c2b634ad5e0757e6",
-                "sha256:9ad883ac4f5225999747f0849643c4d0ec809d9ffe0ddc81a81dd3e68d0af463",
-                "sha256:a25b4c4fdd633501233924f873e6f6cd8970732859ecfe4ecfb60635881f70be",
-                "sha256:a30e4db983faa5145e00ef6eaf894a2d503b3221dbf40a595f3011930d3d0bac",
-                "sha256:a5e9e78332a5d841422b88b8c490dfd7f761e64b3430249b66c05d02f72ceab0",
-                "sha256:b4e08e3831671008888bad5d160d757ef35ce34dbb73b78c3998d16aa1334c97",
-                "sha256:bf1aae95e80acea02a0a622e1c12d3fefc52ffd0fe7bda70a30d070373fbb6c3",
-                "sha256:c61b89803a87a3b2a394089a7dadb79a6c64c89f2e8930cc187fec43b319f8d2",
-                "sha256:cdf80359b641185ae7e580afb9f88cf560298f309a38182972091165bfe1225d",
-                "sha256:d93ebbff3dcf05274843ad8cf650b48ee634626e752c5d73614e5ec9df45f0ce",
-                "sha256:db24d2738add6db19d66ca820479d2f8f96d3f5a13c223f27fa28dd2f268a4bd",
-                "sha256:e0d20f27edfd6f35b388da2bdcd7769e4ffa374fef8994980ced26eb287e033a",
-                "sha256:e2f3b5236079bc3e318a92bab2cc3f669cc32127075ab03ff61cacbae1c392b8",
-                "sha256:e481e54db8cec1457ee7c05f6d2329e3298a304a70d3b5e2e82e77170850b385",
-                "sha256:e5e5dc300a0ca8755ada1569f5caccfcdca28607dfb98b86a54996b288a8ebd3",
-                "sha256:ec2f525273528425ed2f51861b7b88955160cb95dddb17af0914077040aff4a5",
-                "sha256:f234ba3bb339ad17803009c8251f5ee65dcf283a380817fe486823b08b26383d",
-                "sha256:f463598f9e51ccc04f0fe08500f9a0c3251a7086765350be418598b753b5561d",
-                "sha256:f717944aee40e9f48776cf85b523bb376aa2d9255a268d6d643c57ab387e7264",
-                "sha256:fd0febae872a4042da44e972c070f0fd49a85a0a7727ab6b85425f74348be14e",
-                "sha256:fec56c7d1b6a22c8f01557de3975d962ee40270b81b60d1cfdadf2a105d10e84"
+                "sha256:00aa050faf24ce5f2af643e2b86822fa1d7149649995f11bc1e769bbfbf9010b",
+                "sha256:09397a18733fa2a4c7680b746094f980060666ee549deafdb5e102a99ce4619b",
+                "sha256:0f7fdcce52cd882b559a57b484efc92e108efeeee89fab6b623aba1ac68aad2e",
+                "sha256:10514adc41fc8f5922728fbac13d401a1aefcf037f009e64ca3b92464e33bf0e",
+                "sha256:10e001a84f820fea2640e4500e12322b03afc31d8f4f6b813b44813b2a7c7e0d",
+                "sha256:194f2d5a7cb3739875c4d25b3fe288ab0b3dc33f7c857ba2845830c8c51170a0",
+                "sha256:1aac42a21a7fa6c9665392c840b295962992ddf40aecf0a88073bc5c76728117",
+                "sha256:1fb792051db66e09c200e7bc3bda3b1eb18a5b8eb153d2cedb2b14b56a68b8cb",
+                "sha256:2756485f49e7df5c2208bdc64263d19d23eba70666f14ad12d6d8278a2fff65f",
+                "sha256:2b791577c546b6bbd7b43953565fcb0a2fec63643ad605353dd48afbc3c48317",
+                "sha256:420bc6d06d4ae7fb6921524334689eebcbea7bf2005efef070a8562cc9527a37",
+                "sha256:45b07470571bda5ee7f5ec471271bbde97267cc8403fce05e280c36ea73f4754",
+                "sha256:4ebc542d2289c0b016d6945fd07a7e2e23f4abc41e731ac8ad18a9e0c2fd0ec2",
+                "sha256:556dc18e39b6edb76239acfd1c010e37395a54c7fde8c57481c15819a3ffb13e",
+                "sha256:589aba9a35869695b319ed76c6f673d896cd01a7ff78054be1596df7ad9b096f",
+                "sha256:5c95e3e7cc6285bf7ff263eabb0d3bfe3def9a1ff98124083d45e5ece72f4579",
+                "sha256:5dd574a37be388512c72fe0d7318cb8e31743a9b2699847a025e0c08c5bf579d",
+                "sha256:67fbb40db3985c0cfb942fe8853ad94a5e9702d2987dec03abadc2f3b6a24afb",
+                "sha256:6852cd34d96835e4c9091c1e6087325efb5b607b75fd9f7075616197d1c4688a",
+                "sha256:69ae0e9509c43474e33152abe1385b8954922544616426bf793481e1a37e094f",
+                "sha256:6c5bae4c288bda92a7550fe8de9e068c0a7cd56b1c5d888aae5b40f0e13b40bd",
+                "sha256:774bd401e7993452ba0596e741c0c4d6d22f882dd2a798993859181dbffadc62",
+                "sha256:79228a7b90d95957354f37b9d46f2cc8926262ae17b0d3ed8f36c892f2a37e06",
+                "sha256:7b8cba5a25e95041e3413d91f9e50616bcfaec95afa038ce7dc02efefe576745",
+                "sha256:7db97eabd440327c35b751d5ebf78a107f505586485159bcc87660da8bb1fdca",
+                "sha256:7ddd6d35c598af872f9a0a5bce7f7c4a1841684a72dab3302e3df7f17d1b5249",
+                "sha256:82edf3a6090554a83942cec79151d6b5eb96e63d143e80e4cf6671e5d772f6be",
+                "sha256:8b7b3ebfa9416c8eafaffa65216e229480c495e305a06ba176dcac32710744e6",
+                "sha256:8da677135eff43502b7afab5a1e641edfb2dc734ba7fc146e9b1b86817a728e2",
+                "sha256:908c850b98cac1e203ababd4ba76868d19ae0d7172cdc75d3f1b7829b16837d2",
+                "sha256:9da4ee8f711e077633730955c8f3cd2485c9abf5ea0f80aac23221a3224b9a8c",
+                "sha256:a6f1d8256d06f58e6ece150fbe05c63c7f9510df99ee8ac37423f5476a2cebb4",
+                "sha256:afb322ca05e2603deedbcd2e9910f11a3fd2f42bdeafe63018e5641945c7491c",
+                "sha256:b52c6741073de5a744d27329f9803938dcad5c9fee7e61690c705f72973f4175",
+                "sha256:ba633b51835036ff0f402c21f3ff567c565a22ff0a5732b060a68f4660e2a38f",
+                "sha256:bfa1a0f83bdf8061db8d17c2029454722043f1e4dd1b3d3d3120d1b54e75825a",
+                "sha256:bffd6cd47c2e68970039c0d3e355c9ed761d3ca727b204e63cd294cad0e3df90",
+                "sha256:d7a2c1e711ce59ac9d0bba780318bcd102d2958bb423209f24c6354d8c4da930",
+                "sha256:da46beef0ce882546d92b7b2e8deb9e04dbb8fec72945a8eb28b347ca46bc15a",
+                "sha256:ebdd2418ab4e2e26d572d9a1c03877f8514a9b7436729525aa571862507b3fea",
+                "sha256:fc44e50f9d5e96af1a561faa36863f9191f27364a4df3eb70bca66e9370480b6"
             ],
             "index": "pypi",
-            "version": "==2.0.13"
+            "version": "==2.0.18"
         },
         "tuf": {
             "hashes": [
                 "sha256:1524b0fbd8504245f600f121daf86b8fdcb30df74410acc9655944c4868e461c",
                 "sha256:76e7f2a7aced84466865fac2a7127b6085afae51d4328af896fb46f952dd3a53"
             ],
             "index": "pypi",
             "version": "==2.0.0"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
-                "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
+                "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36",
+                "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==4.5.0"
+            "version": "==4.7.1"
         },
         "urllib3": {
             "hashes": [
-                "sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc",
-                "sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e"
+                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
+                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.0.2"
+            "version": "==2.0.3"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
                 "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
                 "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
@@ -511,58 +515,55 @@
                 "sha256:bdfc739baa03b880c2d15d0431b31c658ffc348e907fe197e54e0389dd59e11e"
             ],
             "index": "pypi",
             "version": "==1.7.5"
         },
         "black": {
             "hashes": [
-                "sha256:064101748afa12ad2291c2b91c960be28b817c0c7eaa35bec09cc63aa56493c5",
-                "sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915",
-                "sha256:11c410f71b876f961d1de77b9699ad19f939094c3a677323f43d7a29855fe326",
-                "sha256:1c7b8d606e728a41ea1ccbd7264677e494e87cf630e399262ced92d4a8dac940",
-                "sha256:1d06691f1eb8de91cd1b322f21e3bfc9efe0c7ca1f0e1eb1db44ea367dff656b",
-                "sha256:3238f2aacf827d18d26db07524e44741233ae09a584273aa059066d644ca7b30",
-                "sha256:32daa9783106c28815d05b724238e30718f34155653d4d6e125dc7daec8e260c",
-                "sha256:35d1381d7a22cc5b2be2f72c7dfdae4072a3336060635718cc7e1ede24221d6c",
-                "sha256:3a150542a204124ed00683f0db1f5cf1c2aaaa9cc3495b7a3b5976fb136090ab",
-                "sha256:48f9d345675bb7fbc3dd85821b12487e1b9a75242028adad0333ce36ed2a6d27",
-                "sha256:50cb33cac881766a5cd9913e10ff75b1e8eb71babf4c7104f2e9c52da1fb7de2",
-                "sha256:562bd3a70495facf56814293149e51aa1be9931567474993c7942ff7d3533961",
-                "sha256:67de8d0c209eb5b330cce2469503de11bca4085880d62f1628bd9972cc3366b9",
-                "sha256:6b39abdfb402002b8a7d030ccc85cf5afff64ee90fa4c5aebc531e3ad0175ddb",
-                "sha256:6f3c333ea1dd6771b2d3777482429864f8e258899f6ff05826c3a4fcc5ce3f70",
-                "sha256:714290490c18fb0126baa0fca0a54ee795f7502b44177e1ce7624ba1c00f2331",
-                "sha256:7c3eb7cea23904399866c55826b31c1f55bbcd3890ce22ff70466b907b6775c2",
-                "sha256:92c543f6854c28a3c7f39f4d9b7694f9a6eb9d3c5e2ece488c327b6e7ea9b266",
-                "sha256:a6f6886c9869d4daae2d1715ce34a19bbc4b95006d20ed785ca00fa03cba312d",
-                "sha256:a8a968125d0a6a404842fa1bf0b349a568634f856aa08ffaff40ae0dfa52e7c6",
-                "sha256:c7ab5790333c448903c4b721b59c0d80b11fe5e9803d8703e84dcb8da56fec1b",
-                "sha256:e114420bf26b90d4b9daa597351337762b63039752bdf72bf361364c1aa05925",
-                "sha256:e198cf27888ad6f4ff331ca1c48ffc038848ea9f031a3b40ba36aced7e22f2c8",
-                "sha256:ec751418022185b0c1bb7d7736e6933d40bbb14c14a0abcf9123d1b159f98dd4",
-                "sha256:f0bd2f4a58d6666500542b26354978218a9babcdc972722f4bf90779524515f3"
+                "sha256:01ede61aac8c154b55f35301fac3e730baf0c9cf8120f65a9cd61a81cfb4a0c3",
+                "sha256:022a582720b0d9480ed82576c920a8c1dde97cc38ff11d8d8859b3bd6ca9eedb",
+                "sha256:25cc308838fe71f7065df53aedd20327969d05671bac95b38fdf37ebe70ac087",
+                "sha256:27eb7a0c71604d5de083757fbdb245b1a4fae60e9596514c6ec497eb63f95320",
+                "sha256:327a8c2550ddc573b51e2c352adb88143464bb9d92c10416feb86b0f5aee5ff6",
+                "sha256:47e56d83aad53ca140da0af87678fb38e44fd6bc0af71eebab2d1f59b1acf1d3",
+                "sha256:501387a9edcb75d7ae8a4412bb8749900386eaef258f1aefab18adddea1936bc",
+                "sha256:552513d5cd5694590d7ef6f46e1767a4df9af168d449ff767b13b084c020e63f",
+                "sha256:5c4bc552ab52f6c1c506ccae05681fab58c3f72d59ae6e6639e8885e94fe2587",
+                "sha256:642496b675095d423f9b8448243336f8ec71c9d4d57ec17bf795b67f08132a91",
+                "sha256:6d1c6022b86f83b632d06f2b02774134def5d4d4f1dac8bef16d90cda18ba28a",
+                "sha256:7f3bf2dec7d541b4619b8ce526bda74a6b0bffc480a163fed32eb8b3c9aed8ad",
+                "sha256:831d8f54c3a8c8cf55f64d0422ee875eecac26f5f649fb6c1df65316b67c8926",
+                "sha256:8417dbd2f57b5701492cd46edcecc4f9208dc75529bcf76c514864e48da867d9",
+                "sha256:86cee259349b4448adb4ef9b204bb4467aae74a386bce85d56ba4f5dc0da27be",
+                "sha256:893695a76b140881531062d48476ebe4a48f5d1e9388177e175d76234ca247cd",
+                "sha256:9fd59d418c60c0348505f2ddf9609c1e1de8e7493eab96198fc89d9f865e7a96",
+                "sha256:ad0014efc7acf0bd745792bd0d8857413652979200ab924fbf239062adc12491",
+                "sha256:b5b0ee6d96b345a8b420100b7d71ebfdd19fab5e8301aff48ec270042cd40ac2",
+                "sha256:c333286dc3ddca6fdff74670b911cccedacb4ef0a60b34e491b8a67c833b343a",
+                "sha256:f9062af71c59c004cd519e2fb8f5d25d39e46d3af011b41ab43b9c74e27e236f",
+                "sha256:fb074d8b213749fa1d077d630db0d5f8cc3b2ae63587ad4116e8a436e9bbe995"
             ],
             "index": "pypi",
-            "version": "==23.3.0"
+            "version": "==23.7.0"
         },
         "build": {
             "hashes": [
                 "sha256:af266720050a66c893a6096a2f410989eeac74ff9a68ba194b3f6473e8e26171",
                 "sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269"
             ],
             "index": "pypi",
             "version": "==0.10.0"
         },
         "cachetools": {
             "hashes": [
-                "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14",
-                "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
+                "sha256:95ef631eeaea14ba2e36f06437f36463aac3a096799e876ee55e5cdccb102590",
+                "sha256:dce83f2d9b4e1f732a8cd44af8e8fab2dbe46201467fc98b3ef8f269092bf62b"
             ],
-            "markers": "python_version ~= '3.7'",
-            "version": "==5.3.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==5.3.1"
         },
         "certifi": {
             "hashes": [
                 "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
                 "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
@@ -582,165 +583,174 @@
                 "sha256:362777fb014af596ad31334fde1e8c327dfdb076e1960d1694662d46a6917ab9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==5.1.0"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
-                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
-                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
-                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
-                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
-                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
-                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
-                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
-                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
-                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
-                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
-                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
-                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
-                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
-                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
-                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
-                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
-                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
-                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
-                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
-                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
-                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
-                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
-                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
-                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
-                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
-                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
-                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
-                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
-                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
-                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
-                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
-                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
-                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
-                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
-                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
-                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
-                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
-                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
-                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
-                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
-                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
-                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
-                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
-                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
-                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
-                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
-                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
-                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
-                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
-                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
-                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
-                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
-                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
-                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
-                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
-                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
-                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
-                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
-                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
-                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
-                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
-                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
-                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
-                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
-                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
-                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
-                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
-                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
-                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
-                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
-                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
-                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
-                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
-                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
+                "sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96",
+                "sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c",
+                "sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710",
+                "sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706",
+                "sha256:1249cbbf3d3b04902ff081ffbb33ce3377fa6e4c7356f759f3cd076cc138d020",
+                "sha256:1920d4ff15ce893210c1f0c0e9d19bfbecb7983c76b33f046c13a8ffbd570252",
+                "sha256:193cbc708ea3aca45e7221ae58f0fd63f933753a9bfb498a3b474878f12caaad",
+                "sha256:1a100c6d595a7f316f1b6f01d20815d916e75ff98c27a01ae817439ea7726329",
+                "sha256:1f30b48dd7fa1474554b0b0f3fdfdd4c13b5c737a3c6284d3cdc424ec0ffff3a",
+                "sha256:203f0c8871d5a7987be20c72442488a0b8cfd0f43b7973771640fc593f56321f",
+                "sha256:246de67b99b6851627d945db38147d1b209a899311b1305dd84916f2b88526c6",
+                "sha256:2dee8e57f052ef5353cf608e0b4c871aee320dd1b87d351c28764fc0ca55f9f4",
+                "sha256:2efb1bd13885392adfda4614c33d3b68dee4921fd0ac1d3988f8cbb7d589e72a",
+                "sha256:2f4ac36d8e2b4cc1aa71df3dd84ff8efbe3bfb97ac41242fbcfc053c67434f46",
+                "sha256:3170c9399da12c9dc66366e9d14da8bf7147e1e9d9ea566067bbce7bb74bd9c2",
+                "sha256:3b1613dd5aee995ec6d4c69f00378bbd07614702a315a2cf6c1d21461fe17c23",
+                "sha256:3bb3d25a8e6c0aedd251753a79ae98a093c7e7b471faa3aa9a93a81431987ace",
+                "sha256:3bb7fda7260735efe66d5107fb7e6af6a7c04c7fce9b2514e04b7a74b06bf5dd",
+                "sha256:41b25eaa7d15909cf3ac4c96088c1f266a9a93ec44f87f1d13d4a0e86c81b982",
+                "sha256:45de3f87179c1823e6d9e32156fb14c1927fcc9aba21433f088fdfb555b77c10",
+                "sha256:46fb8c61d794b78ec7134a715a3e564aafc8f6b5e338417cb19fe9f57a5a9bf2",
+                "sha256:48021783bdf96e3d6de03a6e39a1171ed5bd7e8bb93fc84cc649d11490f87cea",
+                "sha256:4957669ef390f0e6719db3613ab3a7631e68424604a7b448f079bee145da6e09",
+                "sha256:5e86d77b090dbddbe78867a0275cb4df08ea195e660f1f7f13435a4649e954e5",
+                "sha256:6339d047dab2780cc6220f46306628e04d9750f02f983ddb37439ca47ced7149",
+                "sha256:681eb3d7e02e3c3655d1b16059fbfb605ac464c834a0c629048a30fad2b27489",
+                "sha256:6c409c0deba34f147f77efaa67b8e4bb83d2f11c8806405f76397ae5b8c0d1c9",
+                "sha256:7095f6fbfaa55defb6b733cfeb14efaae7a29f0b59d8cf213be4e7ca0b857b80",
+                "sha256:70c610f6cbe4b9fce272c407dd9d07e33e6bf7b4aa1b7ffb6f6ded8e634e3592",
+                "sha256:72814c01533f51d68702802d74f77ea026b5ec52793c791e2da806a3844a46c3",
+                "sha256:7a4826ad2bd6b07ca615c74ab91f32f6c96d08f6fcc3902ceeedaec8cdc3bcd6",
+                "sha256:7c70087bfee18a42b4040bb9ec1ca15a08242cf5867c58726530bdf3945672ed",
+                "sha256:855eafa5d5a2034b4621c74925d89c5efef61418570e5ef9b37717d9c796419c",
+                "sha256:8700f06d0ce6f128de3ccdbc1acaea1ee264d2caa9ca05daaf492fde7c2a7200",
+                "sha256:89f1b185a01fe560bc8ae5f619e924407efca2191b56ce749ec84982fc59a32a",
+                "sha256:8b2c760cfc7042b27ebdb4a43a4453bd829a5742503599144d54a032c5dc7e9e",
+                "sha256:8c2f5e83493748286002f9369f3e6607c565a6a90425a3a1fef5ae32a36d749d",
+                "sha256:8e098148dd37b4ce3baca71fb394c81dc5d9c7728c95df695d2dca218edf40e6",
+                "sha256:94aea8eff76ee6d1cdacb07dd2123a68283cb5569e0250feab1240058f53b623",
+                "sha256:95eb302ff792e12aba9a8b8f8474ab229a83c103d74a750ec0bd1c1eea32e669",
+                "sha256:9bd9b3b31adcb054116447ea22caa61a285d92e94d710aa5ec97992ff5eb7cf3",
+                "sha256:9e608aafdb55eb9f255034709e20d5a83b6d60c054df0802fa9c9883d0a937aa",
+                "sha256:a103b3a7069b62f5d4890ae1b8f0597618f628b286b03d4bc9195230b154bfa9",
+                "sha256:a386ebe437176aab38c041de1260cd3ea459c6ce5263594399880bbc398225b2",
+                "sha256:a38856a971c602f98472050165cea2cdc97709240373041b69030be15047691f",
+                "sha256:a401b4598e5d3f4a9a811f3daf42ee2291790c7f9d74b18d75d6e21dda98a1a1",
+                "sha256:a7647ebdfb9682b7bb97e2a5e7cb6ae735b1c25008a70b906aecca294ee96cf4",
+                "sha256:aaf63899c94de41fe3cf934601b0f7ccb6b428c6e4eeb80da72c58eab077b19a",
+                "sha256:b0dac0ff919ba34d4df1b6131f59ce95b08b9065233446be7e459f95554c0dc8",
+                "sha256:baacc6aee0b2ef6f3d308e197b5d7a81c0e70b06beae1f1fcacffdbd124fe0e3",
+                "sha256:bf420121d4c8dce6b889f0e8e4ec0ca34b7f40186203f06a946fa0276ba54029",
+                "sha256:c04a46716adde8d927adb9457bbe39cf473e1e2c2f5d0a16ceb837e5d841ad4f",
+                "sha256:c0b21078a4b56965e2b12f247467b234734491897e99c1d51cee628da9786959",
+                "sha256:c1c76a1743432b4b60ab3358c937a3fe1341c828ae6194108a94c69028247f22",
+                "sha256:c4983bf937209c57240cff65906b18bb35e64ae872da6a0db937d7b4af845dd7",
+                "sha256:c4fb39a81950ec280984b3a44f5bd12819953dc5fa3a7e6fa7a80db5ee853952",
+                "sha256:c57921cda3a80d0f2b8aec7e25c8aa14479ea92b5b51b6876d975d925a2ea346",
+                "sha256:c8063cf17b19661471ecbdb3df1c84f24ad2e389e326ccaf89e3fb2484d8dd7e",
+                "sha256:ccd16eb18a849fd8dcb23e23380e2f0a354e8daa0c984b8a732d9cfaba3a776d",
+                "sha256:cd6dbe0238f7743d0efe563ab46294f54f9bc8f4b9bcf57c3c666cc5bc9d1299",
+                "sha256:d62e51710986674142526ab9f78663ca2b0726066ae26b78b22e0f5e571238dd",
+                "sha256:db901e2ac34c931d73054d9797383d0f8009991e723dab15109740a63e7f902a",
+                "sha256:e03b8895a6990c9ab2cdcd0f2fe44088ca1c65ae592b8f795c3294af00a461c3",
+                "sha256:e1c8a2f4c69e08e89632defbfabec2feb8a8d99edc9f89ce33c4b9e36ab63037",
+                "sha256:e4b749b9cc6ee664a3300bb3a273c1ca8068c46be705b6c31cf5d276f8628a94",
+                "sha256:e6a5bf2cba5ae1bb80b154ed68a3cfa2fa00fde979a7f50d6598d3e17d9ac20c",
+                "sha256:e857a2232ba53ae940d3456f7533ce6ca98b81917d47adc3c7fd55dad8fab858",
+                "sha256:ee4006268ed33370957f55bf2e6f4d263eaf4dc3cfc473d1d90baff6ed36ce4a",
+                "sha256:eef9df1eefada2c09a5e7a40991b9fc6ac6ef20b1372abd48d2794a316dc0449",
+                "sha256:f058f6963fd82eb143c692cecdc89e075fa0828db2e5b291070485390b2f1c9c",
+                "sha256:f25c229a6ba38a35ae6e25ca1264621cc25d4d38dca2942a7fce0b67a4efe918",
+                "sha256:f2a1d0fd4242bd8643ce6f98927cf9c04540af6efa92323e9d3124f57727bfc1",
+                "sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c",
+                "sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac",
+                "sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==3.1.0"
+            "version": "==3.2.0"
         },
         "click": {
             "hashes": [
-                "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
-                "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
+                "sha256:4be4b1af8d665c6d942909916d31a213a106800c47d0eeba73d34da3cbc11367",
+                "sha256:e576aa487d679441d7d30abb87e1b43d24fc53bffb8758443b1a9e1cee504548"
             ],
             "index": "pypi",
-            "version": "==8.1.3"
+            "version": "==8.1.5"
         },
         "colorama": {
             "hashes": [
                 "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44",
                 "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
             "version": "==0.4.6"
         },
         "coverage": {
             "hashes": [
-                "sha256:0342a28617e63ad15d96dca0f7ae9479a37b7d8a295f749c14f3436ea59fdcb3",
-                "sha256:066b44897c493e0dcbc9e6a6d9f8bbb6607ef82367cf6810d387c09f0cd4fe9a",
-                "sha256:10b15394c13544fce02382360cab54e51a9e0fd1bd61ae9ce012c0d1e103c813",
-                "sha256:12580845917b1e59f8a1c2ffa6af6d0908cb39220f3019e36c110c943dc875b0",
-                "sha256:156192e5fd3dbbcb11cd777cc469cf010a294f4c736a2b2c891c77618cb1379a",
-                "sha256:1637253b11a18f453e34013c665d8bf15904c9e3c44fbda34c643fbdc9d452cd",
-                "sha256:292300f76440651529b8ceec283a9370532f4ecba9ad67d120617021bb5ef139",
-                "sha256:30dcaf05adfa69c2a7b9f7dfd9f60bc8e36b282d7ed25c308ef9e114de7fc23b",
-                "sha256:338aa9d9883aaaad53695cb14ccdeb36d4060485bb9388446330bef9c361c252",
-                "sha256:373ea34dca98f2fdb3e5cb33d83b6d801007a8074f992b80311fc589d3e6b790",
-                "sha256:38c0a497a000d50491055805313ed83ddba069353d102ece8aef5d11b5faf045",
-                "sha256:40cc0f91c6cde033da493227797be2826cbf8f388eaa36a0271a97a332bfd7ce",
-                "sha256:4436cc9ba5414c2c998eaedee5343f49c02ca93b21769c5fdfa4f9d799e84200",
-                "sha256:509ecd8334c380000d259dc66feb191dd0a93b21f2453faa75f7f9cdcefc0718",
-                "sha256:5c587f52c81211d4530fa6857884d37f514bcf9453bdeee0ff93eaaf906a5c1b",
-                "sha256:5f3671662dc4b422b15776cdca89c041a6349b4864a43aa2350b6b0b03bbcc7f",
-                "sha256:6599bf92f33ab041e36e06d25890afbdf12078aacfe1f1d08c713906e49a3fe5",
-                "sha256:6e8a95f243d01ba572341c52f89f3acb98a3b6d1d5d830efba86033dd3687ade",
-                "sha256:706ec567267c96717ab9363904d846ec009a48d5f832140b6ad08aad3791b1f5",
-                "sha256:780551e47d62095e088f251f5db428473c26db7829884323e56d9c0c3118791a",
-                "sha256:7ff8f3fb38233035028dbc93715551d81eadc110199e14bbbfa01c5c4a43f8d8",
-                "sha256:828189fcdda99aae0d6bf718ea766b2e715eabc1868670a0a07bf8404bf58c33",
-                "sha256:857abe2fa6a4973f8663e039ead8d22215d31db613ace76e4a98f52ec919068e",
-                "sha256:883123d0bbe1c136f76b56276074b0c79b5817dd4238097ffa64ac67257f4b6c",
-                "sha256:8877d9b437b35a85c18e3c6499b23674684bf690f5d96c1006a1ef61f9fdf0f3",
-                "sha256:8e575a59315a91ccd00c7757127f6b2488c2f914096077c745c2f1ba5b8c0969",
-                "sha256:97072cc90f1009386c8a5b7de9d4fc1a9f91ba5ef2146c55c1f005e7b5c5e068",
-                "sha256:9a22cbb5ede6fade0482111fa7f01115ff04039795d7092ed0db43522431b4f2",
-                "sha256:a063aad9f7b4c9f9da7b2550eae0a582ffc7623dca1c925e50c3fbde7a579771",
-                "sha256:a08c7401d0b24e8c2982f4e307124b671c6736d40d1c39e09d7a8687bddf83ed",
-                "sha256:a0b273fe6dc655b110e8dc89b8ec7f1a778d78c9fd9b4bda7c384c8906072212",
-                "sha256:a2b3b05e22a77bb0ae1a3125126a4e08535961c946b62f30985535ed40e26614",
-                "sha256:a66e055254a26c82aead7ff420d9fa8dc2da10c82679ea850d8feebf11074d88",
-                "sha256:aa387bd7489f3e1787ff82068b295bcaafbf6f79c3dad3cbc82ef88ce3f48ad3",
-                "sha256:ae453f655640157d76209f42c62c64c4d4f2c7f97256d3567e3b439bd5c9b06c",
-                "sha256:b5016e331b75310610c2cf955d9f58a9749943ed5f7b8cfc0bb89c6134ab0a84",
-                "sha256:b9a4ee55174b04f6af539218f9f8083140f61a46eabcaa4234f3c2a452c4ed11",
-                "sha256:bd3b4b8175c1db502adf209d06136c000df4d245105c8839e9d0be71c94aefe1",
-                "sha256:bebea5f5ed41f618797ce3ffb4606c64a5de92e9c3f26d26c2e0aae292f015c1",
-                "sha256:c10fbc8a64aa0f3ed136b0b086b6b577bc64d67d5581acd7cc129af52654384e",
-                "sha256:c2c41c1b1866b670573657d584de413df701f482574bad7e28214a2362cb1fd1",
-                "sha256:cf97ed82ca986e5c637ea286ba2793c85325b30f869bf64d3009ccc1a31ae3fd",
-                "sha256:d1f25ee9de21a39b3a8516f2c5feb8de248f17da7eead089c2e04aa097936b47",
-                "sha256:d2fbc2a127e857d2f8898aaabcc34c37771bf78a4d5e17d3e1f5c30cd0cbc62a",
-                "sha256:dc945064a8783b86fcce9a0a705abd7db2117d95e340df8a4333f00be5efb64c",
-                "sha256:ddc5a54edb653e9e215f75de377354e2455376f416c4378e1d43b08ec50acc31",
-                "sha256:e8834e5f17d89e05697c3c043d3e58a8b19682bf365048837383abfe39adaed5",
-                "sha256:ef9659d1cda9ce9ac9585c045aaa1e59223b143f2407db0eaee0b61a4f266fb6",
-                "sha256:f6f5cab2d7f0c12f8187a376cc6582c477d2df91d63f75341307fcdcb5d60303",
-                "sha256:f81c9b4bd8aa747d417407a7f6f0b1469a43b36a85748145e144ac4e8d303cb5",
-                "sha256:f99ef080288f09ffc687423b8d60978cf3a465d3f404a18d1a05474bd8575a47"
+                "sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f",
+                "sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2",
+                "sha256:0a5f9e1dbd7fbe30196578ca36f3fba75376fb99888c395c5880b355e2875f8a",
+                "sha256:0e1f928eaf5469c11e886fe0885ad2bf1ec606434e79842a879277895a50942a",
+                "sha256:171717c7cb6b453aebac9a2ef603699da237f341b38eebfee9be75d27dc38e01",
+                "sha256:1e9d683426464e4a252bf70c3498756055016f99ddaec3774bf368e76bbe02b6",
+                "sha256:201e7389591af40950a6480bd9edfa8ed04346ff80002cec1a66cac4549c1ad7",
+                "sha256:245167dd26180ab4c91d5e1496a30be4cd721a5cf2abf52974f965f10f11419f",
+                "sha256:2aee274c46590717f38ae5e4650988d1af340fe06167546cc32fe2f58ed05b02",
+                "sha256:2e07b54284e381531c87f785f613b833569c14ecacdcb85d56b25c4622c16c3c",
+                "sha256:31563e97dae5598556600466ad9beea39fb04e0229e61c12eaa206e0aa202063",
+                "sha256:33d6d3ea29d5b3a1a632b3c4e4f4ecae24ef170b0b9ee493883f2df10039959a",
+                "sha256:3d376df58cc111dc8e21e3b6e24606b5bb5dee6024f46a5abca99124b2229ef5",
+                "sha256:419bfd2caae268623dd469eff96d510a920c90928b60f2073d79f8fe2bbc5959",
+                "sha256:48c19d2159d433ccc99e729ceae7d5293fbffa0bdb94952d3579983d1c8c9d97",
+                "sha256:49969a9f7ffa086d973d91cec8d2e31080436ef0fb4a359cae927e742abfaaa6",
+                "sha256:52edc1a60c0d34afa421c9c37078817b2e67a392cab17d97283b64c5833f427f",
+                "sha256:537891ae8ce59ef63d0123f7ac9e2ae0fc8b72c7ccbe5296fec45fd68967b6c9",
+                "sha256:54b896376ab563bd38453cecb813c295cf347cf5906e8b41d340b0321a5433e5",
+                "sha256:58c2ccc2f00ecb51253cbe5d8d7122a34590fac9646a960d1430d5b15321d95f",
+                "sha256:5b7540161790b2f28143191f5f8ec02fb132660ff175b7747b95dcb77ac26562",
+                "sha256:5baa06420f837184130752b7c5ea0808762083bf3487b5038d68b012e5937dbe",
+                "sha256:5e330fc79bd7207e46c7d7fd2bb4af2963f5f635703925543a70b99574b0fea9",
+                "sha256:61b9a528fb348373c433e8966535074b802c7a5d7f23c4f421e6c6e2f1697a6f",
+                "sha256:63426706118b7f5cf6bb6c895dc215d8a418d5952544042c8a2d9fe87fcf09cb",
+                "sha256:6d040ef7c9859bb11dfeb056ff5b3872436e3b5e401817d87a31e1750b9ae2fb",
+                "sha256:6f48351d66575f535669306aa7d6d6f71bc43372473b54a832222803eb956fd1",
+                "sha256:7ee7d9d4822c8acc74a5e26c50604dff824710bc8de424904c0982e25c39c6cb",
+                "sha256:81c13a1fc7468c40f13420732805a4c38a105d89848b7c10af65a90beff25250",
+                "sha256:8d13c64ee2d33eccf7437961b6ea7ad8673e2be040b4f7fd4fd4d4d28d9ccb1e",
+                "sha256:8de8bb0e5ad103888d65abef8bca41ab93721647590a3f740100cd65c3b00511",
+                "sha256:8fa03bce9bfbeeef9f3b160a8bed39a221d82308b4152b27d82d8daa7041fee5",
+                "sha256:924d94291ca674905fe9481f12294eb11f2d3d3fd1adb20314ba89e94f44ed59",
+                "sha256:975d70ab7e3c80a3fe86001d8751f6778905ec723f5b110aed1e450da9d4b7f2",
+                "sha256:976b9c42fb2a43ebf304fa7d4a310e5f16cc99992f33eced91ef6f908bd8f33d",
+                "sha256:9e31cb64d7de6b6f09702bb27c02d1904b3aebfca610c12772452c4e6c21a0d3",
+                "sha256:a342242fe22407f3c17f4b499276a02b01e80f861f1682ad1d95b04018e0c0d4",
+                "sha256:a3d33a6b3eae87ceaefa91ffdc130b5e8536182cd6dfdbfc1aa56b46ff8c86de",
+                "sha256:a895fcc7b15c3fc72beb43cdcbdf0ddb7d2ebc959edac9cef390b0d14f39f8a9",
+                "sha256:afb17f84d56068a7c29f5fa37bfd38d5aba69e3304af08ee94da8ed5b0865833",
+                "sha256:b1c546aca0ca4d028901d825015dc8e4d56aac4b541877690eb76490f1dc8ed0",
+                "sha256:b29019c76039dc3c0fd815c41392a044ce555d9bcdd38b0fb60fb4cd8e475ba9",
+                "sha256:b46517c02ccd08092f4fa99f24c3b83d8f92f739b4657b0f146246a0ca6a831d",
+                "sha256:b7aa5f8a41217360e600da646004f878250a0d6738bcdc11a0a39928d7dc2050",
+                "sha256:b7b4c971f05e6ae490fef852c218b0e79d4e52f79ef0c8475566584a8fb3e01d",
+                "sha256:ba90a9563ba44a72fda2e85302c3abc71c5589cea608ca16c22b9804262aaeb6",
+                "sha256:cb017fd1b2603ef59e374ba2063f593abe0fc45f2ad9abdde5b4d83bd922a353",
+                "sha256:d22656368f0e6189e24722214ed8d66b8022db19d182927b9a248a2a8a2f67eb",
+                "sha256:d2c2db7fd82e9b72937969bceac4d6ca89660db0a0967614ce2481e81a0b771e",
+                "sha256:d39b5b4f2a66ccae8b7263ac3c8170994b65266797fb96cbbfd3fb5b23921db8",
+                "sha256:d62a5c7dad11015c66fbb9d881bc4caa5b12f16292f857842d9d1871595f4495",
+                "sha256:e7d9405291c6928619403db1d10bd07888888ec1abcbd9748fdaa971d7d661b2",
+                "sha256:e84606b74eb7de6ff581a7915e2dab7a28a0517fbe1c9239eb227e1354064dcd",
+                "sha256:eb393e5ebc85245347950143969b241d08b52b88a3dc39479822e073a1a8eb27",
+                "sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1",
+                "sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818",
+                "sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4",
+                "sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e",
+                "sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850",
+                "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"
             ],
             "index": "pypi",
-            "version": "==7.2.5"
+            "version": "==7.2.7"
         },
         "distlib": {
             "hashes": [
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
@@ -751,35 +761,35 @@
                 "sha256:679987caf361a7539d76e584cbeddc311e3aee937877c87346f31debc63e9d06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==0.18.1"
         },
         "editables": {
             "hashes": [
-                "sha256:167524e377358ed1f1374e61c268f0d7a4bf7dbd046c656f7b410cde16161b1a",
-                "sha256:ee686a8db9f5d91da39849f175ffeef094dd0e9c36d6a59a2e8c7f92a3b80020"
+                "sha256:dc322c42e7ccaf19600874035a4573898d88aadd07e177c239298135b75da772",
+                "sha256:dd430dcf41c78d1d68ebbb893e498b0a306b554be9e7cede73b1c876c6ddbc8d"
             ],
             "markers": "python_version >= '3.1'",
-            "version": "==0.3"
+            "version": "==0.4"
         },
         "exceptiongroup": {
             "hashes": [
-                "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
-                "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
+                "sha256:12c3e887d6485d16943a309616de20ae5582633e0a2eda17f4e10fd61c1e8af5",
+                "sha256:e346e69d186172ca7cf029c8c1d16235aa0e04035e5750b4b95039e65204328f"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==1.1.1"
+            "version": "==1.1.2"
         },
         "filelock": {
             "hashes": [
-                "sha256:ad98852315c2ab702aeb628412cbf7e95b7ce8c3bf9565670b4eaecf1db370a9",
-                "sha256:fc03ae43288c013d2ea83c8597001b1129db351aad9c57fe2409327916b8e718"
+                "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81",
+                "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.12.0"
+            "version": "==3.12.2"
         },
         "flake8": {
             "hashes": [
                 "sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7",
                 "sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181"
             ],
             "index": "pypi",
@@ -791,19 +801,19 @@
                 "sha256:c286cf298426064079ed96a9e4a9d39e7f3e9bf15ba60701e95f5492f28415c7"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.0.10"
         },
         "gitpython": {
             "hashes": [
-                "sha256:8ce3bcf69adfdf7c7d503e78fd3b1c492af782d58893b650adb2ac8912ddd573",
-                "sha256:f04893614f6aa713a60cbbe1e6a97403ef633103cdd0ef5eb6efe0deb98dbe8d"
+                "sha256:8d9b8cb1e80b9735e8717c9362079d3ce4c6e5ddeebedd0361b228c3a67a62f6",
+                "sha256:e3d59b1c2c6ebb9dfa7a184daf3b6dd4914237e7488a1730a6d8f6f5d0b4187f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.31"
+            "version": "==3.1.32"
         },
         "hatchling": {
             "hashes": [
                 "sha256:054276e05e2838dffd756a679c334ce6720eba1df2bb096f0e72c0f6e400217a",
                 "sha256:81f2e6063cdbdf17ea11cffe603dfa3fba781da0c127a2814ab1eb5b864de2c0"
             ],
             "index": "pypi",
@@ -829,14 +839,22 @@
             "hashes": [
                 "sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b",
                 "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.4.1"
         },
+        "importlib-metadata": {
+            "hashes": [
+                "sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb",
+                "sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743"
+            ],
+            "markers": "python_version < '3.10'",
+            "version": "==6.8.0"
+        },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
@@ -855,75 +873,75 @@
                 "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.2"
         },
         "markdown-it-py": {
             "hashes": [
-                "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30",
-                "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"
+                "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1",
+                "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2.2.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.0.0"
         },
         "markupsafe": {
             "hashes": [
-                "sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed",
-                "sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc",
-                "sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2",
-                "sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460",
-                "sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7",
-                "sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0",
-                "sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1",
-                "sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa",
-                "sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03",
-                "sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323",
-                "sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65",
-                "sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013",
-                "sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036",
-                "sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f",
-                "sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4",
-                "sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419",
-                "sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2",
-                "sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619",
-                "sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a",
-                "sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a",
-                "sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd",
-                "sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7",
-                "sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666",
-                "sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65",
-                "sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859",
-                "sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625",
-                "sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff",
-                "sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156",
-                "sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd",
-                "sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba",
-                "sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f",
-                "sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1",
-                "sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094",
-                "sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a",
-                "sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513",
-                "sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed",
-                "sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d",
-                "sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3",
-                "sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147",
-                "sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c",
-                "sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603",
-                "sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601",
-                "sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a",
-                "sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1",
-                "sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d",
-                "sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3",
-                "sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54",
-                "sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2",
-                "sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6",
-                "sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58"
+                "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e",
+                "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e",
+                "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431",
+                "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686",
+                "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559",
+                "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc",
+                "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c",
+                "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0",
+                "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4",
+                "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9",
+                "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575",
+                "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba",
+                "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d",
+                "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3",
+                "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00",
+                "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155",
+                "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac",
+                "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52",
+                "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f",
+                "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8",
+                "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b",
+                "sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24",
+                "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea",
+                "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198",
+                "sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0",
+                "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee",
+                "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be",
+                "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2",
+                "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707",
+                "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6",
+                "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58",
+                "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779",
+                "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636",
+                "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c",
+                "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad",
+                "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee",
+                "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc",
+                "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2",
+                "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48",
+                "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7",
+                "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e",
+                "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b",
+                "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa",
+                "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5",
+                "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e",
+                "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb",
+                "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9",
+                "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57",
+                "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc",
+                "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.1.2"
+            "version": "==2.1.3"
         },
         "mccabe": {
             "hashes": [
                 "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "markers": "python_version >= '3.6'",
@@ -935,43 +953,43 @@
                 "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.1.2"
         },
         "mypy": {
             "hashes": [
-                "sha256:1c4c42c60a8103ead4c1c060ac3cdd3ff01e18fddce6f1016e08939647a0e703",
-                "sha256:44797d031a41516fcf5cbfa652265bb994e53e51994c1bd649ffcd0c3a7eccbf",
-                "sha256:473117e310febe632ddf10e745a355714e771ffe534f06db40702775056614c4",
-                "sha256:4c99c3ecf223cf2952638da9cd82793d8f3c0c5fa8b6ae2b2d9ed1e1ff51ba85",
-                "sha256:550a8b3a19bb6589679a7c3c31f64312e7ff482a816c96e0cecec9ad3a7564dd",
-                "sha256:658fe7b674769a0770d4b26cb4d6f005e88a442fe82446f020be8e5f5efb2fae",
-                "sha256:6e33bb8b2613614a33dff70565f4c803f889ebd2f859466e42b46e1df76018dd",
-                "sha256:6e42d29e324cdda61daaec2336c42512e59c7c375340bd202efa1fe0f7b8f8ca",
-                "sha256:74bc9b6e0e79808bf8678d7678b2ae3736ea72d56eede3820bd3849823e7f305",
-                "sha256:76ec771e2342f1b558c36d49900dfe81d140361dd0d2df6cd71b3db1be155409",
-                "sha256:7d23370d2a6b7a71dc65d1266f9a34e4cde9e8e21511322415db4b26f46f6b8c",
-                "sha256:87df44954c31d86df96c8bd6e80dfcd773473e877ac6176a8e29898bfb3501cb",
-                "sha256:8c5979d0deb27e0f4479bee18ea0f83732a893e81b78e62e2dda3e7e518c92ee",
-                "sha256:95d8d31a7713510685b05fbb18d6ac287a56c8f6554d88c19e73f724a445448a",
-                "sha256:a22435632710a4fcf8acf86cbd0d69f68ac389a3892cb23fbad176d1cddaf228",
-                "sha256:a8763e72d5d9574d45ce5881962bc8e9046bf7b375b0abf031f3e6811732a897",
-                "sha256:c1eb485cea53f4f5284e5baf92902cd0088b24984f4209e25981cc359d64448d",
-                "sha256:c5d2cc54175bab47011b09688b418db71403aefad07cbcd62d44010543fc143f",
-                "sha256:cbc07246253b9e3d7d74c9ff948cd0fd7a71afcc2b77c7f0a59c26e9395cb152",
-                "sha256:d0b6c62206e04061e27009481cb0ec966f7d6172b5b936f3ead3d74f29fe3dcf",
-                "sha256:ddae0f39ca146972ff6bb4399f3b2943884a774b8771ea0a8f50e971f5ea5ba8",
-                "sha256:e1f4d16e296f5135624b34e8fb741eb0eadedca90862405b1f1fde2040b9bd11",
-                "sha256:e86c2c6852f62f8f2b24cb7a613ebe8e0c7dc1402c61d36a609174f63e0ff017",
-                "sha256:ebc95f8386314272bbc817026f8ce8f4f0d2ef7ae44f947c4664efac9adec929",
-                "sha256:f9dca1e257d4cc129517779226753dbefb4f2266c4eaad610fc15c6a7e14283e",
-                "sha256:faff86aa10c1aa4a10e1a301de160f3d8fc8703b88c7e98de46b531ff1276a9a"
+                "sha256:01fd2e9f85622d981fd9063bfaef1aed6e336eaacca00892cd2d82801ab7c042",
+                "sha256:0dde1d180cd84f0624c5dcaaa89c89775550a675aff96b5848de78fb11adabcd",
+                "sha256:141dedfdbfe8a04142881ff30ce6e6653c9685b354876b12e4fe6c78598b45e2",
+                "sha256:16f0db5b641ba159eff72cff08edc3875f2b62b2fa2bc24f68c1e7a4e8232d01",
+                "sha256:190b6bab0302cec4e9e6767d3eb66085aef2a1cc98fe04936d8a42ed2ba77bb7",
+                "sha256:2460a58faeea905aeb1b9b36f5065f2dc9a9c6e4c992a6499a2360c6c74ceca3",
+                "sha256:34a9239d5b3502c17f07fd7c0b2ae6b7dd7d7f6af35fbb5072c6208e76295816",
+                "sha256:43b592511672017f5b1a483527fd2684347fdffc041c9ef53428c8dc530f79a3",
+                "sha256:43d24f6437925ce50139a310a64b2ab048cb2d3694c84c71c3f2a1626d8101dc",
+                "sha256:45d32cec14e7b97af848bddd97d85ea4f0db4d5a149ed9676caa4eb2f7402bb4",
+                "sha256:470c969bb3f9a9efcedbadcd19a74ffb34a25f8e6b0e02dae7c0e71f8372f97b",
+                "sha256:566e72b0cd6598503e48ea610e0052d1b8168e60a46e0bfd34b3acf2d57f96a8",
+                "sha256:5703097c4936bbb9e9bce41478c8d08edd2865e177dc4c52be759f81ee4dd26c",
+                "sha256:7549fbf655e5825d787bbc9ecf6028731973f78088fbca3a1f4145c39ef09462",
+                "sha256:8207b7105829eca6f3d774f64a904190bb2231de91b8b186d21ffd98005f14a7",
+                "sha256:8c4d8e89aa7de683e2056a581ce63c46a0c41e31bd2b6d34144e2c80f5ea53dc",
+                "sha256:98324ec3ecf12296e6422939e54763faedbfcc502ea4a4c38502082711867258",
+                "sha256:9bbcd9ab8ea1f2e1c8031c21445b511442cc45c89951e49bbf852cbb70755b1b",
+                "sha256:9d40652cc4fe33871ad3338581dca3297ff5f2213d0df345bcfbde5162abf0c9",
+                "sha256:a2746d69a8196698146a3dbe29104f9eb6a2a4d8a27878d92169a6c0b74435b6",
+                "sha256:ae704dcfaa180ff7c4cfbad23e74321a2b774f92ca77fd94ce1049175a21c97f",
+                "sha256:bfdca17c36ae01a21274a3c387a63aa1aafe72bff976522886869ef131b937f1",
+                "sha256:c482e1246726616088532b5e964e39765b6d1520791348e6c9dc3af25b233828",
+                "sha256:ca637024ca67ab24a7fd6f65d280572c3794665eaf5edcc7e90a866544076878",
+                "sha256:e02d700ec8d9b1859790c0475df4e4092c7bf3272a4fd2c9f33d87fac4427b8f",
+                "sha256:e5952d2d18b79f7dc25e62e014fe5a23eb1a3d2bc66318df8988a01b1a037c5b"
             ],
             "index": "pypi",
-            "version": "==1.3.0"
+            "version": "==1.4.1"
         },
         "mypy-extensions": {
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
@@ -1015,35 +1033,35 @@
                 "sha256:3ef6ac33239e4027d9a5598a381b9d30880a1477e50039db2eac6e8a8f6d1b18"
             ],
             "index": "pypi",
             "version": "==23.1.2"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f",
-                "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"
+                "sha256:cec7b889196b9144d088e4c57d9ceef7374f6c39694ad1577a0aab50d27ea28c",
+                "sha256:f87ca4fcff7d2b0f81c6a748a77973d7af0f4d526f98f308477c3c436c74d528"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.5.1"
+            "version": "==3.8.1"
         },
         "pluggy": {
             "hashes": [
-                "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
-                "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
+                "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
+                "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
             "markers": "python_version >= '3.1'",
-            "version": "==1.0.0"
+            "version": "==1.2.0"
         },
         "pre-commit": {
             "hashes": [
-                "sha256:218e9e3f7f7f3271ebc355a15598a4d3893ad9fc7b57fe446db75644543323b9",
-                "sha256:733f78c9a056cdd169baa6cd4272d51ecfda95346ef8a89bf93712706021b907"
+                "sha256:10badb65d6a38caff29703362271d7dca483d01da88f9d7e05d0b97171c136cb",
+                "sha256:a2256f489cd913d575c145132ae196fe335da32d91a8294b7afe6622335dd023"
             ],
             "index": "pypi",
-            "version": "==3.3.1"
+            "version": "==3.3.3"
         },
         "pretend": {
             "hashes": [
                 "sha256:c90eb810cde8ebb06dafcb8796f9a95228ce796531bc806e794c2f4649aa1b10",
                 "sha256:e389b12b7073604be67845dbe32bf8297360ad9a609b24846fe15d86e0b7dc01"
             ],
             "index": "pypi",
@@ -1071,35 +1089,35 @@
                 "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.15.1"
         },
         "pyproject-api": {
             "hashes": [
-                "sha256:435f46547a9ff22cf4208ee274fca3e2869aeb062a4834adfc99a4dd64af3cf9",
-                "sha256:4698a3777c2e0f6b624f8a4599131e2a25376d90fe8d146d7ac74c67c6f97c43"
+                "sha256:14cf09828670c7b08842249c1f28c8ee6581b872e893f81b62d5465bec41502f",
+                "sha256:ffb5b2d7cad43f5b2688ab490de7c4d3f6f15e0b819cb588c4b771567c9729eb"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.5.1"
+            "version": "==1.5.3"
         },
         "pyproject-hooks": {
             "hashes": [
                 "sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8",
                 "sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.0"
         },
         "pytest": {
             "hashes": [
-                "sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362",
-                "sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3"
+                "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32",
+                "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"
             ],
             "index": "pypi",
-            "version": "==7.3.1"
+            "version": "==7.4.0"
         },
         "pyyaml": {
             "hashes": [
                 "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
@@ -1141,35 +1159,35 @@
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.0"
         },
         "requests": {
             "hashes": [
-                "sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294",
-                "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
-            "version": "==2.30.0"
+            "version": "==2.31.0"
         },
         "rich": {
             "hashes": [
-                "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c",
-                "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"
+                "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
+                "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
             "index": "pypi",
-            "version": "==13.3.5"
+            "version": "==13.4.2"
         },
         "setuptools": {
             "hashes": [
-                "sha256:23aaf86b85ca52ceb801d32703f12d77517b2556af839621c641fca11287952b",
-                "sha256:f104fa03692a2602fa0fec6c6a9e63b6c8a968de13e17c026957dd1f53d80990"
+                "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f",
+                "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==67.7.2"
+            "version": "==68.0.0"
         },
         "smmap": {
             "hashes": [
                 "sha256:2aba19d6a040e78d8b09de5c57e96207b09ed71d8e55ce0959eeee6c8e190d94",
                 "sha256:c840e62059cd3be204b0c9c9f74be2c09d5648eddd4580d9314c3ecde0b30936"
             ],
             "markers": "python_version >= '3.6'",
@@ -1188,19 +1206,19 @@
                 "sha256:97787ff1fa3256a3eef9eda523a63dbf299f7b47e053cfcf684a1c2a8380c912"
             ],
             "index": "pypi",
             "version": "==6.2.1"
         },
         "sphinx-rtd-theme": {
             "hashes": [
-                "sha256:a0d8bd1a2ed52e0b338cbe19c4b2eef3c5e7a048769753dac6a9f059c7b641b8",
-                "sha256:f823f7e71890abe0ac6aaa6013361ea2696fc8d3e1fa798f463e82bdb77eeff2"
+                "sha256:01c5c5a72e2d025bd23d1f06c59a4831b06e6ce6c01fdd5ebfe9986c0a880fc7",
+                "sha256:6a7e7d8af34eb8fc57d52a09c6b6b9c46ff44aea5951bc831eeb9245378f3689"
             ],
             "index": "pypi",
-            "version": "==1.2.0"
+            "version": "==1.2.2"
         },
         "sphinxcontrib-applehelp": {
             "hashes": [
                 "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228",
                 "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"
             ],
             "index": "pypi",
@@ -1223,15 +1241,15 @@
             "version": "==2.0.1"
         },
         "sphinxcontrib-jquery": {
             "hashes": [
                 "sha256:1620739f04e36a2c779f1a131a2dfd49b2fd07351bf1968ced074365933abc7a",
                 "sha256:f936030d7d0147dd026a4f2b5a57343d233f1fc7b363f68b3d4f1cb0993878ae"
             ],
-            "markers": "python_version >= '3.1'",
+            "markers": "python_version >= '2.7'",
             "version": "==4.1"
         },
         "sphinxcontrib-jsmath": {
             "hashes": [
                 "sha256:2ec2eaebfb78f3f2078e73666b1415417a116cc848b72e5172e596c871103178",
                 "sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8"
             ],
@@ -1275,54 +1293,62 @@
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version >= '3.1'",
             "version": "==2.0.1"
         },
         "tox": {
             "hashes": [
-                "sha256:5a2eac5fb816779dfdf5cb00fecbc27eb0524e4626626bb1de84747b24cacc56",
-                "sha256:d25a2e6cb261adc489604fafd76cd689efeadfa79709965e965668d6d3f63046"
+                "sha256:1b8f8ae08d6a5475cad9d508236c51ea060620126fd7c3c513d0f5c7f29cc776",
+                "sha256:5e2ad8845764706170d3dcaac171704513cc8a725655219acb62fe4380bdadda"
             ],
             "index": "pypi",
-            "version": "==4.5.1"
+            "version": "==4.6.4"
         },
         "types-requests": {
             "hashes": [
-                "sha256:c6cf08e120ca9f0dc4fa4e32c3f953c3fba222bcc1db6b97695bce8da1ba9864",
-                "sha256:dec781054324a70ba64430ae9e62e7e9c8e4618c185a5cb3f87a6738251b5a31"
+                "sha256:3de667cffa123ce698591de0ad7db034a5317457a596eb0b4944e5a9d9e8d1ac",
+                "sha256:afb06ef8f25ba83d59a1d424bd7a5a939082f94b94e90ab5e6116bd2559deaa3"
             ],
             "index": "pypi",
-            "version": "==2.30.0.0"
+            "version": "==2.31.0.1"
         },
         "types-urllib3": {
             "hashes": [
                 "sha256:3300538c9dc11dad32eae4827ac313f5d986b8b21494801f1bf97a1ac6c03ae5",
                 "sha256:5dbd1d2bef14efee43f5318b5d36d805a489f6600252bb53626d4bfafd95e27c"
             ],
             "version": "==1.26.25.13"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
-                "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
+                "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36",
+                "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==4.5.0"
+            "version": "==4.7.1"
         },
         "urllib3": {
             "hashes": [
-                "sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc",
-                "sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e"
+                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
+                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.0.2"
+            "version": "==2.0.3"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e",
-                "sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924"
+                "sha256:34da10f14fea9be20e0fd7f04aba9732f84e593dac291b757ce42e3368a39419",
+                "sha256:8ff19a38c1021c742148edc4f81cb43d7f8c6816d2ede2ab72af5b84c749ade1"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.23.0"
+            "version": "==20.23.1"
+        },
+        "zipp": {
+            "hashes": [
+                "sha256:0b37c326d826d5ca35f2b9685cd750292740774ef16190008b00a0227c256fe0",
+                "sha256:857b158da2cbf427b376da1c24fd11faecbac5a4ac7523c3607f8a01f94c2ec0"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==3.16.1"
         }
     }
 }
```

### Comparing `repository_service_tuf-0.3.0a1/README.rst` & `repository_service_tuf-0.4.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/pyproject.toml` & `repository_service_tuf-0.4.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/requirements-dev.txt` & `repository_service_tuf-0.4.0b1/requirements-dev.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,89 @@
 -i https://pypi.org/simple
-alabaster==0.7.13 ; python_version >= '3.6'
-babel==2.12.1 ; python_version >= '3.7'
+alabaster==0.7.13; python_version >= '3.6'
+babel==2.12.1; python_version >= '3.7'
 bandit==1.7.5
-black==23.3.0
+black==23.7.0
 build==0.10.0
-cachetools==5.3.0 ; python_version ~= '3.7'
-certifi==2023.5.7 ; python_version >= '3.6'
-cfgv==3.3.1 ; python_full_version >= '3.6.1'
-chardet==5.1.0 ; python_version >= '3.7'
-charset-normalizer==3.1.0 ; python_full_version >= '3.7.0'
-click==8.1.3
-colorama==0.4.6 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'
-coverage==7.2.5
+cachetools==5.3.1; python_version >= '3.7'
+certifi==2023.5.7; python_version >= '3.6'
+cfgv==3.3.1; python_full_version >= '3.6.1'
+chardet==5.1.0; python_version >= '3.7'
+charset-normalizer==3.2.0; python_full_version >= '3.7.0'
+click==8.1.5
+colorama==0.4.6; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'
+coverage==7.2.7
 distlib==0.3.6
-docutils==0.18.1 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
-editables==0.3 ; python_version >= '3.1'
-exceptiongroup==1.1.1 ; python_version < '3.11'
-filelock==3.12.0 ; python_version >= '3.7'
+docutils==0.18.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
+editables==0.4; python_version >= '3.1'
+exceptiongroup==1.1.2; python_version < '3.11'
+filelock==3.12.2; python_version >= '3.7'
 flake8==6.0.0
-gitdb==4.0.10 ; python_version >= '3.7'
-gitpython==3.1.31 ; python_version >= '3.7'
+gitdb==4.0.10; python_version >= '3.7'
+gitpython==3.1.32; python_version >= '3.7'
 hatchling==0.22.0
-identify==2.5.24 ; python_version >= '3.7'
-idna==3.4 ; python_version >= '3.5'
-imagesize==1.4.1 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
-iniconfig==2.0.0 ; python_version >= '3.7'
+identify==2.5.24; python_version >= '3.7'
+idna==3.4; python_version >= '3.5'
+imagesize==1.4.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
+importlib-metadata==6.8.0; python_version < '3.10'
+iniconfig==2.0.0; python_version >= '3.7'
 isort==5.12.0
-jinja2==3.1.2 ; python_version >= '3.7'
-markdown-it-py==2.2.0 ; python_version >= '3.7'
-markupsafe==2.1.2 ; python_version >= '3.7'
-mccabe==0.7.0 ; python_version >= '3.6'
-mdurl==0.1.2 ; python_version >= '3.7'
-mypy==1.3.0
-mypy-extensions==1.0.0 ; python_version >= '3.5'
-nodeenv==1.8.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'
-packaging==23.1 ; python_version >= '3.1'
-pathspec==0.11.1 ; python_version >= '3.7'
-pbr==5.11.1 ; python_version >= '2.6'
+jinja2==3.1.2; python_version >= '3.7'
+markdown-it-py==3.0.0; python_version >= '3.8'
+markupsafe==2.1.3; python_version >= '3.7'
+mccabe==0.7.0; python_version >= '3.6'
+mdurl==0.1.2; python_version >= '3.7'
+mypy==1.4.1
+mypy-extensions==1.0.0; python_version >= '3.5'
+nodeenv==1.8.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'
+packaging==23.1; python_version >= '3.1'
+pathspec==0.11.1; python_version >= '3.7'
+pbr==5.11.1; python_version >= '2.6'
 pip==23.1.2
-platformdirs==3.5.1 ; python_version >= '3.7'
-pluggy==1.0.0 ; python_version >= '3.1'
-pre-commit==3.3.1
+platformdirs==3.8.1; python_version >= '3.7'
+pluggy==1.2.0; python_version >= '3.1'
+pre-commit==3.3.3
 pretend==1.0.9
-pycodestyle==2.10.0 ; python_version >= '3.6'
-pyflakes==3.0.1 ; python_version >= '3.6'
-pygments==2.15.1 ; python_version >= '3.7'
-pyproject-api==1.5.1 ; python_version >= '3.7'
-pyproject-hooks==1.0.0 ; python_version >= '3.7'
-pytest==7.3.1
-pyyaml==6.0 ; python_version >= '3.6'
-requests==2.30.0
-rich==13.3.5
-setuptools==67.7.2 ; python_version >= '3.7'
-smmap==5.0.0 ; python_version >= '3.6'
+pycodestyle==2.10.0; python_version >= '3.6'
+pyflakes==3.0.1; python_version >= '3.6'
+pygments==2.15.1; python_version >= '3.7'
+pyproject-api==1.5.3; python_version >= '3.7'
+pyproject-hooks==1.0.0; python_version >= '3.7'
+pytest==7.4.0
+pyyaml==6.0; python_version >= '3.6'
+requests==2.31.0
+rich==13.4.2
+setuptools==68.0.0; python_version >= '3.7'
+smmap==5.0.0; python_version >= '3.6'
 snowballstemmer==2.2.0
 sphinx==6.2.1
-sphinx-rtd-theme==1.2.0
+sphinx-rtd-theme==1.2.2
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
-sphinxcontrib-jquery==4.1 ; python_version >= '3.1'
+sphinxcontrib-jquery==4.1; python_version >= '2.7'
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-plantuml==0.25
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-stevedore==5.1.0 ; python_version >= '3.8'
-tomli==2.0.1 ; python_version >= '3.1'
-tox==4.5.1
-types-requests==2.30.0.0
+stevedore==5.1.0; python_version >= '3.8'
+tomli==2.0.1; python_version >= '3.1'
+tox==4.6.4
+types-requests==2.31.0.1
 types-urllib3==1.26.25.13
-typing-extensions==4.5.0 ; python_version >= '3.7'
-urllib3==2.0.2 ; python_version >= '3.7'
-virtualenv==20.23.0 ; python_version >= '3.7'
+typing-extensions==4.7.1; python_version >= '3.7'
+urllib3==2.0.3; python_version >= '3.7'
+virtualenv==20.23.1; python_version >= '3.7'
+zipp==3.16.1; python_version >= '3.8'
 cffi==1.15.1
 configobj==5.0.8
-cryptography==40.0.2
-dynaconf[ini]==3.1.12
-greenlet==2.0.2 ; platform_machine == 'aarch64' or (platform_machine == 'ppc64le' or (platform_machine == 'x86_64' or (platform_machine == 'amd64' or (platform_machine == 'AMD64' or (platform_machine == 'win32' or platform_machine == 'WIN32')))))
+cryptography==41.0.2
+dynaconf[ini]==3.2.0
+greenlet==2.0.2; platform_machine == 'aarch64' or (platform_machine == 'ppc64le' or (platform_machine == 'x86_64' or (platform_machine == 'amd64' or (platform_machine == 'AMD64' or (platform_machine == 'win32' or platform_machine == 'WIN32')))))
 psycopg2==2.9.6
 pycparser==2.21
 pynacl==1.5.0
 rich-click==1.6.1
 securesystemslib[crypto]==0.28.0
-six==1.16.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
-sqlalchemy==2.0.13
+six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
+sqlalchemy==2.0.18
 tuf==2.0.0
```

### Comparing `repository_service_tuf-0.3.0a1/requirements.txt` & `repository_service_tuf-0.4.0b1/requirements.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 -i https://pypi.org/simple
-certifi==2023.5.7 ; python_version >= '3.6'
+certifi==2023.5.7; python_version >= '3.6'
 cffi==1.15.1
-charset-normalizer==3.1.0 ; python_full_version >= '3.7.0'
-click==8.1.3
+charset-normalizer==3.2.0; python_full_version >= '3.7.0'
+click==8.1.5
 configobj==5.0.8
-cryptography==40.0.2
-dynaconf[ini]==3.1.12
-greenlet==2.0.2 ; platform_machine == 'aarch64' or (platform_machine == 'ppc64le' or (platform_machine == 'x86_64' or (platform_machine == 'amd64' or (platform_machine == 'AMD64' or (platform_machine == 'win32' or platform_machine == 'WIN32')))))
-idna==3.4 ; python_version >= '3.5'
+cryptography==41.0.2
+dynaconf[ini]==3.2.0
+greenlet==2.0.2; platform_machine == 'aarch64' or (platform_machine == 'ppc64le' or (platform_machine == 'x86_64' or (platform_machine == 'amd64' or (platform_machine == 'AMD64' or (platform_machine == 'win32' or platform_machine == 'WIN32')))))
+idna==3.4; python_version >= '3.5'
 isort==5.12.0
-markdown-it-py==2.2.0 ; python_version >= '3.7'
-mdurl==0.1.2 ; python_version >= '3.7'
+markdown-it-py==3.0.0; python_version >= '3.8'
+mdurl==0.1.2; python_version >= '3.7'
 psycopg2==2.9.6
 pycparser==2.21
-pygments==2.15.1 ; python_version >= '3.7'
+pygments==2.15.1; python_version >= '3.7'
 pynacl==1.5.0
-requests==2.30.0
-rich==13.3.5
+requests==2.31.0
+rich==13.4.2
 rich-click==1.6.1
 securesystemslib[crypto]==0.28.0
-six==1.16.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
-sqlalchemy==2.0.13
+six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
+sqlalchemy==2.0.18
 tuf==2.0.0
-typing-extensions==4.5.0 ; python_version >= '3.7'
-urllib3==2.0.2 ; python_version >= '3.7'
+typing-extensions==4.7.1; python_version >= '3.7'
+urllib3==2.0.3; python_version >= '3.7'
```

### Comparing `repository_service_tuf-0.3.0a1/tox.ini` & `repository_service_tuf-0.4.0b1/tox.ini`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/.github/ISSUE_TEMPLATE/bug.yml` & `repository_service_tuf-0.4.0b1/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/.github/ISSUE_TEMPLATE/other.yml` & `repository_service_tuf-0.4.0b1/.github/ISSUE_TEMPLATE/other.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/.github/ISSUE_TEMPLATE/task.yml` & `repository_service_tuf-0.4.0b1/.github/ISSUE_TEMPLATE/task.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/.github/PULL_REQUEST_TEMPLATE/pr.yml` & `repository_service_tuf-0.4.0b1/.github/PULL_REQUEST_TEMPLATE/pr.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/.github/workflows/cd.yml` & `repository_service_tuf-0.4.0b1/.github/workflows/cd.yml`

 * *Files 8% similar despite different names*

```diff
@@ -23,20 +23,20 @@
     name: Build
     runs-on: ubuntu-latest
     needs: functional-latest
     outputs:
       release_id: ${{ steps.gh-release.outputs.id }}
     steps:
       - name: Checkout release tag
-        uses: actions/checkout@8e5e7e5ab8b370d6c329ec480221332ada57f0ab
+        uses: actions/checkout@c85c95e3d7251135ab7dc9ce3241c5835cc595a9
         with:
           ref: ${{ github.event.workflow_run.head_branch }}
 
       - name: Set up Python
-        uses: actions/setup-python@57ded4d7d5e986d7296eab16560982c6dd7c923b
+        uses: actions/setup-python@bd6b4b6205c4dbad673328db7b31b7fab9e241c0
         with:
           python-version: '3.x'
 
       - name: Install build dependency
         run: python3 -m pip install --upgrade pip build twine
 
       - name: Build binary wheel and source tarball
@@ -90,18 +90,18 @@
             })
 
       - name: Publish distribution 📦 to Test PyPI
         env:
           name: testpypi
           url: https://pypi.org/p/repository-service-tuf
         if: github.repository == 'repository-service-tuf/repository-service-tuf-cli'
-        uses: pypa/gh-action-pypi-publish@a56da0b891b3dc519c7ee3284aff1fad93cc8598
+        uses: pypa/gh-action-pypi-publish@f5622bde02b04381239da3573277701ceca8f6a0
         with:
           repository-url: https://test.pypi.org/legacy/
 
       - name: Publish binary wheel and source tarball 📦 on PyPI
         env:
           name: pypi
           url: https://pypi.org/p/repository-service-tuf
         # Only attempt PyPI upload in upstream repository
         if: github.repository == 'repository-service-tuf/repository-service-tuf-cli'
-        uses: pypa/gh-action-pypi-publish@a56da0b891b3dc519c7ee3284aff1fad93cc8598
+        uses: pypa/gh-action-pypi-publish@f5622bde02b04381239da3573277701ceca8f6a0
```

### Comparing `repository_service_tuf-0.3.0a1/.github/workflows/ci.yml` & `repository_service_tuf-0.4.0b1/.github/workflows/ci.yml`

 * *Files 19% similar despite different names*

```diff
@@ -11,16 +11,16 @@
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-versions: [ "3.9", "3.10", "3.11" ]
 
     steps:
-    - uses: actions/checkout@8e5e7e5ab8b370d6c329ec480221332ada57f0ab
-    - uses: actions/setup-python@57ded4d7d5e986d7296eab16560982c6dd7c923b
+    - uses: actions/checkout@c85c95e3d7251135ab7dc9ce3241c5835cc595a9
+    - uses: actions/setup-python@bd6b4b6205c4dbad673328db7b31b7fab9e241c0
       with:
         python-version: ${{ matrix.python-versions }}
 
     - name: Install tox and coverage
       run: pip install tox tox-gh-actions build
 
     - name: Install build dependency
```

### Comparing `repository_service_tuf-0.3.0a1/.github/workflows/update-python-deps.yml` & `repository_service_tuf-0.4.0b1/.github/workflows/update-python-deps.yml`

 * *Files 14% similar despite different names*

```diff
@@ -4,32 +4,32 @@
   schedule:
     - cron: "0 8 * * *"
 jobs:
   update-dep:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-versions: [ "3.9", "3.10", "3.11"]
+        python-versions: [ "3.9" ]
     steps:
-      - uses: actions/checkout@8e5e7e5ab8b370d6c329ec480221332ada57f0ab
-      - uses: actions/setup-python@57ded4d7d5e986d7296eab16560982c6dd7c923b
+      - uses: actions/checkout@c85c95e3d7251135ab7dc9ce3241c5835cc595a9
+      - uses: actions/setup-python@bd6b4b6205c4dbad673328db7b31b7fab9e241c0
         with:
           python-version: ${{ matrix.python-versions }}
       - name: Install prerequisites
         run: |
           pip install tox pipenv
       - name: Update dependencies
         run: |
           pipenv update -d
           make requirements
       - name: Run tests
         run: |
           make tests
       - name: Create Pull Request
-        uses: peter-evans/create-pull-request@284f54f989303d2699d373481a0cfa13ad5a6666
+        uses: peter-evans/create-pull-request@153407881ec5c347639a548ade7d8ad1d6740e38
         with:
           token: ${{ secrets.GITHUB_TOKEN }}
           commit-message: "build: Update Python dependencies"
           branch: "rstuf-bot/update-python-dependencies"
           delete-branch: true
           title: "build: Update Python dependencies"
           body: >
```

### Comparing `repository_service_tuf-0.3.0a1/docs/Makefile` & `repository_service_tuf-0.4.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/docs/make.bat` & `repository_service_tuf-0.4.0b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/docs/diagrams/repository-service-tuf-cli-C1.puml` & `repository_service_tuf-0.4.0b1/docs/diagrams/repository-service-tuf-cli-C1.puml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/docs/diagrams/repository-service-tuf-cli-C2.puml` & `repository_service_tuf-0.4.0b1/docs/diagrams/repository-service-tuf-cli-C2.puml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/docs/diagrams/repository-service-tuf-cli-C3.puml` & `repository_service_tuf-0.4.0b1/docs/diagrams/repository-service-tuf-cli-C3.puml`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 
 System_Boundary(trs_cli, "Repository Service for TUF CLI") #APPLICATION {
     Container_Boundary(repository_service_tuf, "repository_service_tuf")  #LightSkyBlue {
         Container_Boundary(cli, "cli") #DeepSkyBlue{
             Container_Ext(click, "click")
             Container_Boundary(admin, "admin") {
                 Container(ceremony, "ceremony")
+                Container_Boundary(metadata, "metadata"){
+                    Container(update, "update")
+                }
                 Container(login, "login")
                 Container_Boundary(token, "token"){
                     Container(generate, "generate")
                 }
             }
         }
         Container_Boundary(users, "helpers",) #LightBlue {
@@ -65,20 +68,23 @@
 }
 Container(tuf_repository_service_api, "REPOSITORY-SERVICE-TUF-API", "HTTP REST API", $tags="queue") #APPLICATION
 
 Rel_R(user, trs_cli, "rstuf-cli", $tags="terminal")
 
 Rel(ceremony, tuf, " ")
 Rel(ceremony, api_client, " ")
+Rel(update, tuf, " ")
+Rel(update, api_client, " ")
 Rel_R(generate, api_client, " ")
 Rel_L(token, click, " ")
 Rel(login, api_client, " ")
 Rel(api_client, requests, " ")
 Rel(dynaconf, user, " ", $tags="os")
 Rel(python_tuf, user, " ", $tags="os")
 Rel_U(ceremony, click, " ")
 Rel_U(login, click, " ")
+Rel_U(update, click, " ")
 
 Rel(requests, tuf_repository_service_api, " ")
 
 HIDE_STEREOTYPE()
 @enduml
```

### Comparing `repository_service_tuf-0.3.0a1/docs/source/conf.py` & `repository_service_tuf-0.4.0b1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/docs/source/_static/repository-service-tuf-cli-C1.png` & `repository_service_tuf-0.4.0b1/docs/source/_static/repository-service-tuf-cli-C1.png`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/docs/source/_static/repository-service-tuf-cli-C2.png` & `repository_service_tuf-0.4.0b1/docs/source/_static/repository-service-tuf-cli-C2.png`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/docs/source/devel/design.rst` & `repository_service_tuf-0.4.0b1/docs/source/devel/design.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/docs/source/devel/repository_service_tuf.cli.admin.rst` & `repository_service_tuf-0.4.0b1/docs/source/devel/repository_service_tuf.cli.admin.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/docs/source/devel/repository_service_tuf.helpers.rst` & `repository_service_tuf-0.4.0b1/docs/source/devel/repository_service_tuf.helpers.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/repository_service_tuf/constants.py` & `repository_service_tuf-0.4.0b1/repository_service_tuf/constants.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/repository_service_tuf/cli/__init__.py` & `repository_service_tuf-0.4.0b1/repository_service_tuf/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,17 @@
                 prog_name = line.split("=")[0].strip()
                 break
 
 except FileNotFoundError:
     pass
 
 
-@click.group(context_settings={"help_option_names": ["-h", "--help"]})
+@click.group(  # type: ignore
+    context_settings={"help_option_names": ["-h", "--help"]}
+)
 @click.option(
     "-c",
     "--config",
     "config",
     default=os.path.join(HOME, ".rstuf.ini"),
     help="Repository Service for TUF config file.",
     required=False,
```

### Comparing `repository_service_tuf-0.3.0a1/repository_service_tuf/cli/admin/ceremony.py` & `repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/ceremony.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,37 @@
 # SPDX-FileCopyrightText: 2022-2023 VMware Inc
 #
 # SPDX-License-Identifier: MIT
 
 #
 # Ceremony
 #
-import json
 import os
 from typing import Any, Dict, Generator, Optional
 
 from rich import box, markdown, prompt, table  # type: ignore
-from securesystemslib.exceptions import (  # type: ignore
-    CryptoError,
-    Error,
-    FormatError,
-    StorageError,
-)
-from securesystemslib.interface import (  # type: ignore
-    import_privatekey_from_file,
-)
 
 from repository_service_tuf.cli import click, console
 from repository_service_tuf.cli.admin import admin
 from repository_service_tuf.constants import KeyType
 from repository_service_tuf.helpers.api_client import (
     URL,
-    LazySettings,
-    Methods,
     bootstrap_status,
-    get_headers,
-    request_server,
+    send_payload,
     task_status,
 )
 from repository_service_tuf.helpers.tuf import (
     BootstrapSetup,
     Roles,
     RSTUFKey,
     ServiceSettings,
     TUFManagement,
+    load_key,
+    load_payload,
+    save_payload,
 )
 
 CEREMONY_INTRO = """
 # Repository Metadata and Settings for the Repository Service for TUF
 
 Repository Service for TUF (RSTUF) is a system for securing content downloads
 from tampering between the repository and the client using The Update Framework
@@ -134,15 +124,15 @@
 **timestamp**
 
 The timestamp role is responsible for providing information about the
 timelines of available updates. Timelines information is made available by
 frequently signing a new timestamp.json file with a short expiration time.
 This file indicates the latest version of `snapshot.json`.
 
-Uses one single online key,
+Uses one single online key.
 """
 
 STEP_1 = """
 # STEP 1: Configure the Roles
 
 The TUF root role supports multiple keys and the threshold (quorum of trust)
 defines the minimal number of keys required to take actions using the root role.
@@ -264,93 +254,14 @@
 
     if setup.root_keys.get(keyid) is not None:
         return True
 
     return False
 
 
-def _load_key(
-    filepath: str, keytype: str, password: Optional[str], name: str
-) -> RSTUFKey:
-    try:
-        key = import_privatekey_from_file(filepath, keytype, password)
-        # Make sure name cannot be an empty string.
-        # If no name is given use first 7 letters of the keyid.
-        name = name if name != "" else key["keyid"][:7]
-        return RSTUFKey(key=key, key_path=filepath, name=name)
-    except CryptoError as err:
-        return RSTUFKey(
-            error=(
-                f":cross_mark: [red]Failed[/]: {str(err)} Check the"
-                " password, type, etc"
-            )
-        )
-
-    except (StorageError, FormatError, Error, OSError) as err:
-        return RSTUFKey(error=f":cross_mark: [red]Failed[/]: {str(err)}")
-
-
-def _send_bootstrap(
-    settings: LazySettings, bootstrap_payload: Dict[str, Any]
-) -> str:
-    headers = get_headers(settings)
-    response = request_server(
-        settings.SERVER,
-        URL.bootstrap.value,
-        Methods.post,
-        bootstrap_payload,
-        headers=headers,
-    )
-
-    if response.status_code != 202:
-        raise click.ClickException(
-            f"Error {response.status_code} {response.text}"
-        )
-
-    response_json = response.json()
-    if (
-        response_json.get("message") is None
-        or response_json.get("message") != "Bootstrap accepted."
-    ):
-        raise click.ClickException(response.text)
-
-    else:
-        if data := response_json.get("data"):
-            task_id = data.get("task_id")
-            if task_id is None:
-                raise click.ClickException(
-                    f"Failed to get `task id` {response.text}"
-                )
-            console.print(f"Bootstrap status: ACCEPTED ({task_id})")
-
-            return task_id
-        else:
-            raise click.ClickException(
-                f"Failed to get task response data {response.text}"
-            )
-
-
-def _load_bootstrap_payload(path: str) -> Dict[str, Any]:
-    try:
-        with open(path) as payload_data:
-            bootstrap_payload = json.load(payload_data)
-    except OSError as err:
-        raise click.ClickException(f"Error to load {path}. {str(err)}")
-
-    return bootstrap_payload
-
-
-def _save_bootstrap_payload(file: str, bootstrap_payload: Dict[str, Any]):
-    try:
-        with open(file, "w") as f:
-            f.write(json.dumps(bootstrap_payload, indent=2))
-    except OSError as err:
-        raise click.ClickException(f"Failed to save {file}. {str(err)}")
-
-
 def _configure_role_target():
     console.print("\n")
     console.print(markdown.Markdown(BINS_DELEGATION_MESSAGE), width=100)
     show_example = prompt.Confirm.ask("Show example?", default="y")
     if show_example:
         with console.pager(links=True):
             console.print(markdown.Markdown(HASH_BINS_EXAMPLE), width=100)
@@ -399,22 +310,30 @@
         )
 
 
 def _configure_role(role: Roles) -> None:
     console.print(
         markdown.Markdown(f"## {role.value} configuration"), width=100
     )
-    setup.expiration[role] = prompt.IntPrompt.ask(
-        (
-            "\nWhat is the [green]metadata expiration[/] for "
-            f"the [cyan]{role.value}[/] role?(Days)"
-        ),
-        default=setup.expiration[role],
-        show_default=True,
-    )
+    role_expiration = 0
+    while True:
+        role_expiration = prompt.IntPrompt.ask(
+            (
+                "\nWhat is the [green]metadata expiration[/] for "
+                f"the [cyan]{role.value}[/] role?(Days)"
+            ),
+            default=setup.expiration[role],
+            show_default=True,
+        )
+        if role_expiration < 1:
+            console.print(f"Expiration of {role.value} must be at least 1 day")
+        else:
+            break
+
+    setup.expiration[role] = role_expiration
 
     if role == Roles.ROOT:
         _configure_role_root()
 
     if role == Roles.TARGETS:
         _configure_role_target()
 
@@ -430,25 +349,27 @@
             default=KeyType.KEY_TYPE_ED25519.value,
         )
         filepath = prompt.Prompt.ask(
             f"Enter {key_count}/{number_of_keys} the "
             f"[cyan]{role}[/]`s private key [green]path[/]"
         )
 
+        colored_role = click.style(role, fg="cyan")
+        colored_pass = click.style("password", fg="green")
         password = click.prompt(
             f"Enter {key_count}/{number_of_keys} the "
-            f"{role}`s private key password",
+            f"{colored_role}`s private key {colored_pass}",
             hide_input=True,
         )
         name = prompt.Prompt.ask(
-            "[Optional] Give a name/tag to the key",
+            "[Optional] Give a [green]name/tag[/] to the key",
             default="",
             show_default=False,
         )
-        role_key: RSTUFKey = _load_key(filepath, key_type, password, name)
+        role_key: RSTUFKey = load_key(filepath, key_type, password, name)
 
         if role_key.error:
             console.print(role_key.error)
             try_again = prompt.Confirm.ask("Try again?", default="y")
             if try_again:
                 continue
             else:
@@ -484,18 +405,18 @@
     def _init_keys_table(path: Optional[bool] = True) -> table.Table:
         """Gets a new keys table"""
         keys_table = table.Table(box=box.MINIMAL)
         if path is True:
             keys_table.add_column(
                 "path", justify="right", style="cyan", no_wrap=True
             )
-        keys_table.add_column("type", justify="center")
-        keys_table.add_column("verified", justify="center")
-        keys_table.add_column("name/tag", justify="center")
-        keys_table.add_column("id", justify="center")
+        keys_table.add_column("Storage", justify="center")
+        keys_table.add_column("Verified", justify="center")
+        keys_table.add_column("Name/Tag", justify="center")
+        keys_table.add_column("Id", justify="center")
 
         return keys_table
 
     # Validations
     #
     # Online key validation
     while True:
@@ -658,15 +579,15 @@
     json_payload["metadata"] = {
         key: data.to_dict() for key, data in metadata.items()
     }
 
     return json_payload
 
 
-@admin.command()
+@admin.command()  # type: ignore
 @click.option(
     "-b",
     "--bootstrap",
     "bootstrap",
     help=(
         "Bootstrap a Repository Service for TUF using the Repository Metadata "
         "after Ceremony"
@@ -687,22 +608,22 @@
     required=False,
 )
 @click.option(
     "-u",
     "--upload",
     help=(
         "Upload existent payload 'file'. Requires '-b/--bootstrap'. "
-        "Optional '-f/--file' to use non default file."
+        "Optional '-f/--file' to use non default file name."
     ),
     required=False,
     is_flag=True,
 )
 @click.option(
     "--upload-server",
-    help="[when using '--no-auth'] Upload RSTUF API Server address. ",
+    help="[when using '--auth'] Upload to RSTUF API Server address. ",
     required=False,
     hidden=True,
 )
 @click.option(
     "-s",
     "--save",
     help=(
@@ -735,39 +656,51 @@
 
     # option upload: it requires -b/--bootstrap
     if upload is True and bootstrap is False:
         raise click.ClickException("Requires '-b/--bootstrap' option.")
 
     # option bootstrap: checks if the server accepts it beforehand
     if bootstrap:
-        if settings.AUTH is True and upload_server is None:
+        if settings.AUTH is False and upload_server is None:
             raise click.ClickException(
-                "Requires '--upload-server' when using '--auth'. "
+                "Requires '--upload-server' "
                 "Example: --upload-server https://rstuf-api.example.com"
             )
         elif upload_server:
             settings.SERVER = upload_server
 
         bs_status = bootstrap_status(settings)
         if bs_status.get("data", {}).get("bootstrap") is True:
             raise click.ClickException(f"{bs_status.get('message')}")
 
     # option bootstrap + upload: bootstrap payload is available, skips ceremony
     if bootstrap is True and upload is True:
-        bootstrap_payload = _load_bootstrap_payload(file)
+        bootstrap_payload = load_payload(file)
         console.print("Starting online bootstrap")
-        task_id = _send_bootstrap(settings, bootstrap_payload)
+        task_id = send_payload(
+            settings=settings,
+            url=URL.bootstrap.value,
+            payload=bootstrap_payload,
+            expected_msg="Bootstrap accepted.",
+            command_name="Bootstrap",
+        )
         task_status(task_id, settings, "Bootstrap status: ")
         console.print(f"Bootstrap completed using `{file}`. 🔐 🎉")
 
     # option ceremony: runs the ceremony, save the payload
     else:
         bootstrap_payload = _run_ceremony_steps(save)
-        _save_bootstrap_payload(file, bootstrap_payload)
+        save_payload(file, bootstrap_payload)
         console.print(
             f"\nCeremony done. 🔐 🎉. Bootstrap payload ({file}) saved."
         )
 
         if bootstrap is True:
-            task_id = _send_bootstrap(settings, bootstrap_payload)
+            task_id = send_payload(
+                settings=settings,
+                url=URL.bootstrap.value,
+                payload=bootstrap_payload,
+                expected_msg="Bootstrap accepted.",
+                command_name="Bootstrap",
+            )
             task_status(task_id, settings, "Bootstrap status: ")
             console.print("\nCeremony done. 🔐 🎉. Bootstrap completed.")
```

### Comparing `repository_service_tuf-0.3.0a1/repository_service_tuf/cli/admin/import_targets.py` & `repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/import_targets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import json
 import os
 from datetime import datetime
+from math import log
 from typing import Any, Dict, List
 
-from tuf.api.metadata import Delegations, SuccinctRoles, Targets
+from tuf.api.metadata import SuccinctRoles
 
 from repository_service_tuf.cli import click, console
 from repository_service_tuf.cli.admin import admin
 from repository_service_tuf.helpers.api_client import (
+    URL,
     Methods,
     bootstrap_status,
     publish_targets,
     request_server,
     task_status,
 )
-from repository_service_tuf.helpers.tuf import Metadata
 
 
 def _check_csv_files(csv_files: List[str]):
     not_found_csv_files: List[str] = []
     for csv_file in csv_files:
         if not os.path.isfile(csv_file):
             not_found_csv_files.append(csv_file)
@@ -26,85 +27,106 @@
     if len(not_found_csv_files) > 0:
         raise click.ClickException(
             f"CSV file(s) not found: {(', ').join(not_found_csv_files)}"
         )
 
 
 def _parse_csv_data(
-    csv_file: str, succinct_roles: SuccinctRoles
+    db: Any,
+    rstuf_target_roles: Any,
+    succinct_roles: SuccinctRoles,
+    csv_file: str,
 ) -> List[Dict[str, Any]]:
     rstuf_db_data: List[Dict[str, Any]] = []
     with open(csv_file, "r") as f:
         for line in f:
+            path = line.split(";")[0]
+            length = int(line.split(";")[1])
+            hash_algorithm = line.split(";")[2]
+            hash_digest = line.split(";")[3]
             rstuf_db_data.append(
                 {
-                    "path": line.split(";")[0],
+                    "path": path,
                     "info": {
-                        "length": int(line.split(";")[1]),
-                        "hashes": {line.split(";")[2]: line.split(";")[3]},
+                        "length": length,
+                        "hashes": {hash_algorithm: hash_digest},
                     },
-                    "rolename": succinct_roles.get_role_for_target(
-                        line.split(";")[0]
-                    ),
                     "published": False,
                     "action": "ADD",
+                    "targets_role": db.execute(
+                        rstuf_target_roles.select().where(
+                            rstuf_target_roles.c.rolename
+                            == succinct_roles.get_role_for_target(path)
+                        )
+                    ).one()[0],
                     "last_update": datetime.now(),
                 }
             )
 
     return rstuf_db_data
 
 
 def _import_csv_to_rstuf(
     db_client: Any,
-    rstuf_table: Any,
+    rstuf_target_files: Any,
+    rstuf_target_roles: Any,
     csv_files: List[str],
     succinct_roles: SuccinctRoles,
 ) -> None:
     # Required to except the appropriate exception.
     from sqlalchemy.exc import IntegrityError
 
     for csv_file in csv_files:
         console.print(f"Import status: Loading data from {csv_file}")
-        rstuf_db_data = _parse_csv_data(csv_file, succinct_roles)
+        rstuf_db_data = _parse_csv_data(
+            db_client, rstuf_target_roles, succinct_roles, csv_file
+        )
         console.print(f"Import status: Importing {csv_file} data")
         try:
-            db_client.execute(rstuf_table.insert(), rstuf_db_data)
+            db_client.execute(rstuf_target_files.insert(), rstuf_db_data)
         except IntegrityError:
             raise click.ClickException(
                 "Import status: ABORTED due duplicated targets. "
                 "CSV files must to have unique targets (path). "
                 "No data added to RSTUF DB."
             )
         console.print(f"Import status: {csv_file} imported")
 
 
-def _get_succinct_roles(metadata_url: str) -> SuccinctRoles:
-    response = request_server(metadata_url, "1.bin.json", Methods.get)
-    if response.status_code == 404:
-        raise click.ClickException("RSTUF Metadata Targets not found.")
+def _get_succinct_roles(api_url: str) -> SuccinctRoles:
+    response = request_server(api_url, URL.config.value, Methods.get)
+    if response.status_code != 200:
+        raise click.ClickException(
+            f"Failed to retrieve RSTUF config {response.text}"
+        )
 
-    json_data = json.loads(response.text)
-    targets: Metadata[Targets] = Metadata.from_dict(json_data)
-    if targets.signed.delegations is None:
-        raise click.ClickException("Failed to get Targets Delegations")
+    try:
+        data = response.json()["data"]
+        num_bins = data["number_of_delegated_bins"]
 
-    targets_delegations: Delegations = targets.signed.delegations
+    except (json.JSONDecodeError, KeyError):
+        raise click.ClickException(
+            "Failed to parse 'data', 'number_of_delegated_bins' from config "
+            f"{response.text}"
+        )
+    bit_length = int(log(num_bins, 2))
 
-    if targets_delegations.succinct_roles is None:
-        raise click.ClickException("Failed to get Targets succinct roles")
+    # the 'keyids' and the 'threshold' are irrelevant once we need the names
+    succinct_roles = SuccinctRoles(
+        keyids=[], threshold=1, bit_length=bit_length, name_prefix="bins"
+    )
 
-    return targets_delegations.succinct_roles
+    return succinct_roles
 
 
-@admin.command()
+@admin.command()  # type: ignore
 @click.option(
-    "--metadata-url",
+    "--api-url",
     required=True,
-    help="RSTUF Metadata URL i.e.: http://127.0.0.1 .",
+    help="RSTUF API URL i.e.: http://127.0.0.1 .",
 )
 @click.option(
     "--db-uri",
     required=True,
     help="RSTUF DB URI. i.e.: postgresql://postgres:secret@127.0.0.1:5433",
 )
 @click.option(
@@ -120,15 +142,15 @@
     "--skip-publish-targets",
     is_flag=True,
     help="Skip publishing targets in TUF Metadata.",
 )
 @click.pass_context
 def import_targets(
     context: Any,
-    metadata_url: str,
+    api_url: str,
     db_uri: str,
     csv: List[str],
     skip_publish_targets: bool,
 ):
     """
     Import targets to RSTUF from exported CSV file.\n
     Note: sqlalchemy needs to be installed in order to use this command.\n
@@ -140,35 +162,42 @@
     try:
         from sqlalchemy import Connection, MetaData, Table, create_engine
     except ModuleNotFoundError:
         raise ModuleNotFoundError(
             "SQLAlchemy is required by import-targets. "
             "pip install repository-service-tuf[sqlalchemy,psycopg2]"
         )
-
     settings = context.obj["settings"]
+    settings.SERVER = api_url
 
     bs_status = bootstrap_status(settings)
     if bs_status.get("data", {}).get("bootstrap") is False:
         raise click.ClickException(
             "`import-targets` requires bootstrap process done. "
             f"{bs_status.get('message')}"
         )
 
     # load all required infrastructure
-    succinct_roles = _get_succinct_roles(metadata_url)
+    succinct_roles = _get_succinct_roles(api_url)
     engine = create_engine(f"{db_uri}")
     db_metadata = MetaData()
     db_client: Connection = engine.connect()
-    rstuf_table = Table("rstuf_targets", db_metadata, autoload_with=engine)
+    rstuf_target_files = Table(
+        "rstuf_target_files", db_metadata, autoload_with=engine
+    )
+    rstuf_target_roles = Table(
+        "rstuf_target_roles", db_metadata, autoload_with=engine
+    )
 
     # validate if the CSV files are accessible
     _check_csv_files(csv_files=csv)
     # import all CSV file(s) data to RSTUF DB without commiting
-    _import_csv_to_rstuf(db_client, rstuf_table, csv, succinct_roles)
+    _import_csv_to_rstuf(
+        db_client, rstuf_target_files, rstuf_target_roles, csv, succinct_roles
+    )
 
     # commit data into RSTUF DB
     console.print("Import status: Commiting all data to the RSTUF database")
     db_client.commit()
     console.print("Import status: All data imported to RSTUF DB")
 
     if skip_publish_targets:
```

### Comparing `repository_service_tuf-0.3.0a1/repository_service_tuf/cli/admin/login.py` & `repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/login.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     )
     if token_response.status_code != 200:
         raise click.ClickException(token_response.json()["detail"])
 
     return token_response.json()
 
 
-def _run_login(context, server_, user_, password_, expires_):
+def _run_login(context, server_, password_, expires_):
     settings = context.obj.get("settings")
     console.print(
         markdown.Markdown(
             f"""# Login to Repository Service for TUF\n
             The server and token will generate a token and it will be
             stored in {context.obj.get('config')}
             """
@@ -51,23 +51,18 @@
             console.print(
                 f"Please use 'http://{server}' or 'https://{server}'"
             )
             server_ = None
         else:
             break
 
-    if user_ is None:
-        username = prompt.Prompt.ask(
-            "Username", default="admin", show_default=True
-        )
-    else:
-        username = user_
+    username = "admin"
 
     if password_ is None:
-        password = click.prompt("Password", hide_input=True)
+        password = click.prompt(f"Password for {username}", hide_input=True)
     else:
         password = password_
 
     if expires_ is None:
         expires = prompt.IntPrompt.ask(
             "Expire (in hours)", default=24, show_default=False
         )
@@ -81,39 +76,39 @@
             "write:targets "
             "write:bootstrap "
             "read:bootstrap "
             "read:settings "
             "read:token "
             "read:tasks "
             "write:token "
+            "write:metadata "
         ),
         "expires": expires,
     }
 
     token = _login(server, data)
     settings.SERVER = server
     settings.TOKEN = token["access_token"]
     loaders.write(context.obj.get("config"), settings.to_dict())
 
     console.print(f"Token stored in {context.obj.get('config')}\n")
     console.print("Login successful.")
 
 
-@admin.command()
+@admin.command()  # type: ignore
 @click.option(
     "-f", "--force", "force", help="Force login/Renew token", is_flag=True
 )
 @click.option("-s", "server_", help="Server", required=False, default=None)
-@click.option("-u", "user_", help="User", required=False, default=None)
 @click.option("-p", "password_", help="Password", required=False, default=None)
 @click.option(
     "-e", "expires_", help="Expires in Hours", required=False, default=None
 )
 @click.pass_context
-def login(context, force, server_, user_, password_, expires_):
+def login(context, force, server_, password_, expires_):
     """
     Login to Repository Service for TUF (API).
     """
     settings = context.obj.get("settings")
 
     if settings.get("AUTH") is False:
         return None
@@ -121,19 +116,19 @@
     elif (
         force is False
         and settings.get("SERVER") is not None
         and settings.get("TOKEN") is not None
     ):
         response = is_logged(settings)
         if response.state is False:
-            _run_login(context, server_, user_, password_, expires_)
+            _run_login(context, server_, password_, expires_)
 
         else:
             data = response.data
             if response.data.get("expired") is False:
                 console.print(
                     f"Already logged to {settings.get('SERVER')}. "
                     f"Valid until '{data['expiration']}'"
                 )
 
     else:
-        _run_login(context, server_, user_, password_, expires_)
+        _run_login(context, server_, password_, expires_)
```

### Comparing `repository_service_tuf-0.3.0a1/repository_service_tuf/cli/admin/token.py` & `repository_service_tuf-0.4.0b1/repository_service_tuf/cli/admin/token.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     """
     settings = context.obj.get("settings")
     if settings.get("AUTH") is False:
         console.print("[INFO] admin token is disabled, use `--auth`")
         raise click.Abort()
 
 
-@token.command()
+@token.command()  # type: ignore
 @click.option(
     "-e",
     "--expires",
     "expires",
     help="Expires in hours. Default: 24",
     default=24,
     required=False,
@@ -50,15 +50,17 @@
     Generate new token.
     """
     settings = context.obj.get("settings")
     server = settings.get("SERVER")
     logged_token = settings.get("TOKEN")
     login = is_logged(settings)
     if login.state is False:
-        raise click.ClickException("Not logged. Use 'rstuf admin login'")
+        raise click.ClickException(
+            "Not logged. Use 'rstuf --auth admin login'"
+        )
 
     headers = {"Authorization": f"Bearer {logged_token}"}
     payload = {"scopes": list(scope), "expires": expires}
     response = request_server(
         server,
         f"{URL.token.value}new/",
         Methods.post,
@@ -73,26 +75,28 @@
         raise click.ClickException(
             f"Error: {response.status_code} {response.json()['detail']}"
         )
 
     console.print_json(response.text)
 
 
-@token.command()
+@token.command()  # type: ignore
 @click.argument("token")
 @click.pass_context
 def inspect(context, token):
     "Show token information details."
 
     settings = context.obj.get("settings")
     server = settings.get("SERVER")
     logged_token = settings.get("TOKEN")
     login = is_logged(settings)
     if login.state is False:
-        raise click.ClickException("Not logged. Use 'rstuf admin login'")
+        raise click.ClickException(
+            "Not logged. Use 'rstuf --auth admin login'"
+        )
 
     headers = {"Authorization": f"Bearer {logged_token}"}
     response = request_server(
         server,
         f"{URL.token.value}?token={token}",
         Methods.get,
         headers=headers,
```

### Comparing `repository_service_tuf-0.3.0a1/repository_service_tuf/cli/key/generate_key.py` & `repository_service_tuf-0.4.0b1/repository_service_tuf/cli/key/generate_key.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/repository_service_tuf/helpers/api_client.py` & `repository_service_tuf-0.4.0b1/repository_service_tuf/helpers/api_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,23 +3,28 @@
 # SPDX-License-Identifier: MIT
 import time
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Dict, Optional
 
 import requests
+import rich_click as click
 from dynaconf import LazySettings
 from requests.exceptions import ConnectionError
+from rich.console import Console
+from tuf.api.metadata import Metadata
 
-from repository_service_tuf.cli import click, console
+console = Console()
 
 
 class URL(Enum):
     token = "api/v1/token/"  # nosec bandit: not hard coded password.
     bootstrap = "api/v1/bootstrap/"
+    config = "api/v1/config/"
+    metadata = "api/v1/metadata/"
     task = "api/v1/task/?task_id="
     publish_targets = "api/v1/targets/publish/"
 
 
 class Methods(Enum):
     get = "get"
     post = "post"
@@ -90,33 +95,35 @@
     server = settings.get("SERVER")
     token = settings.get("TOKEN")
     if server and token:
         token_access_check = is_logged(settings)
         if token_access_check.state is False:
             raise click.ClickException(
                 f"{str(token_access_check.data)}"
-                "\n\nTry re-login: 'rstuf admin login'"
+                "\n\nTry re-login: 'rstuf --auth admin login'"
             )
 
         expired_admin = token_access_check.data.get("expired")
         if expired_admin is True:
             raise click.ClickException(
-                "The token has expired. Run 'rstuf admin login'"
+                "The token has expired. Run 'rstuf --auth admin login'"
             )
         else:
             headers = {"Authorization": f"Bearer {token}"}
             response = request_server(
                 server, URL.bootstrap.value, Methods.get, headers=headers
             )
             if response.status_code != 200:
                 raise click.ClickException(
                     f"Unexpected error: {response.text}"
                 )
     else:
-        raise click.ClickException("Login first. Run 'rstuf admin login'")
+        raise click.ClickException(
+            "Login first. Run 'rstuf --auth admin login'"
+        )
 
     return headers
 
 
 def bootstrap_status(settings: LazySettings) -> Dict[str, Any]:
     headers = get_headers(settings)
     response = request_server(
@@ -197,7 +204,75 @@
         raise click.ClickException(
             f"Failed to publish targets. {publish_targets.status_code} "
             f"{publish_targets.text}"
         )
     task_id = publish_targets.json()["data"]["task_id"]
 
     return task_id
+
+
+def send_payload(
+    settings: LazySettings,
+    url: str,
+    payload: Dict[str, Any],
+    expected_msg: str,
+    command_name: str,
+) -> str:
+    """
+    Send 'payload' to a given 'settings.SERVER'.
+
+    Args:
+        settings: the command context settings object
+        url: one of the URLs to a given endpoint as defined in api_client.py
+        payload: dictionary containing the payload to send
+        expected_msg: expected message to receive as a response to the request
+        command_name: name of the command sending the payload, used for logging
+
+    Returns:
+        Task id of the job sending the payload.
+    """
+    headers = get_headers(settings)
+    response = request_server(
+        settings.SERVER,
+        url,
+        Methods.post,
+        payload,
+        headers=headers,
+    )
+
+    if response.status_code != 202:
+        raise click.ClickException(
+            f"Error {response.status_code} {response.text}"
+        )
+
+    response_json = response.json()
+    if (
+        response_json.get("message") is None
+        or response_json.get("message") != expected_msg
+    ):
+        raise click.ClickException(response.text)
+
+    if data := response_json.get("data"):
+        task_id = data.get("task_id")
+        if task_id is None:
+            raise click.ClickException(
+                f"Failed to get `task id` {response.text}"
+            )
+        console.print(f"{command_name} status: ACCEPTED ({task_id})")
+
+        return task_id
+    else:
+        raise click.ClickException(
+            f"Failed to get task response data {response.text}"
+        )
+
+
+def get_md_file(file_uri: str) -> Metadata:
+    if file_uri.startswith("http"):
+        console.print(f"Fetching file {file_uri}")
+        response = requests.get(file_uri)
+        if response.status_code != 200:
+            raise click.ClickException(f"Cannot fetch {file_uri}")
+
+        return Metadata.from_bytes(response.content)
+    else:
+        return Metadata.from_file(file_uri)
```

### Comparing `repository_service_tuf-0.3.0a1/tests/test_tuf_repository_service.py` & `repository_service_tuf-0.4.0b1/tests/test_tuf_repository_service.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/tests/files/key_storage/JanisJoplin.key` & `repository_service_tuf-0.4.0b1/tests/files/key_storage/JanisJoplin.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/tests/files/key_storage/JimiHendrix.key` & `repository_service_tuf-0.4.0b1/tests/files/key_storage/JimiHendrix.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/tests/files/key_storage/online-rsa.key` & `repository_service_tuf-0.4.0b1/tests/files/key_storage/online-rsa.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/tests/files/key_storage/online-rsa.pub` & `repository_service_tuf-0.4.0b1/tests/files/key_storage/online-rsa.pub`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/tests/files/key_storage/online.key` & `repository_service_tuf-0.4.0b1/tests/files/key_storage/online.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/tests/unit/cli/test__init__.py` & `repository_service_tuf-0.4.0b1/tests/unit/cli/test__init__.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/tests/unit/cli/admin/test_ceremony.py` & `repository_service_tuf-0.4.0b1/tests/unit/cli/admin/test_ceremony.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # SPDX-FileCopyrightText: 2022-2023 VMware Inc
 #
 # SPDX-License-Identifier: MIT
 
 import pretend  # type: ignore
-import pytest
 
 from repository_service_tuf.cli.admin import ceremony
-from repository_service_tuf.constants import KeyType
+from repository_service_tuf.helpers.api_client import URL
 
 
 class TestCeremonyFunctions:
     def test__key_already_in_use(self, test_setup):
         ceremony.setup = test_setup
         result = ceremony._key_already_in_use({"keyid": "ema"})
         assert result is False
@@ -24,310 +23,14 @@
     def test__key_already_in_use_exists_in_online_key(self, test_setup):
         test_setup.online_key = ceremony.RSTUFKey(key={"keyid": "ema"})
 
         ceremony.setup = test_setup
         result = ceremony._key_already_in_use({"keyid": "ema"})
         assert result is True
 
-    def test__load_key(self, monkeypatch):
-        monkeypatch.setattr(
-            ceremony,
-            "import_privatekey_from_file",
-            pretend.call_recorder(lambda *a: {"keyid": "ema"}),
-        )
-
-        result = ceremony._load_key(
-            "/p/key", KeyType.KEY_TYPE_ED25519.value, "pwd", None
-        )
-        assert result == ceremony.RSTUFKey({"keyid": "ema"}, "/p/key", None)
-        assert ceremony.import_privatekey_from_file.calls == [
-            pretend.call("/p/key", KeyType.KEY_TYPE_ED25519.value, "pwd")
-        ]
-
-    def test__load_key_CryptoError(self, monkeypatch):
-        monkeypatch.setattr(
-            ceremony,
-            "import_privatekey_from_file",
-            pretend.raiser(ceremony.CryptoError("wrong password")),
-        )
-
-        result = ceremony._load_key(
-            "/p/key", KeyType.KEY_TYPE_ED25519.value, "pwd", None
-        )
-        assert result == ceremony.RSTUFKey(
-            {},
-            None,
-            error=(
-                ":cross_mark: [red]Failed[/]: wrong password Check the "
-                "password, type, etc"
-            ),
-        )
-
-    def test__load_key_OSError(self, monkeypatch):
-        monkeypatch.setattr(
-            ceremony,
-            "import_privatekey_from_file",
-            pretend.raiser(OSError("permission denied")),
-        )
-        result = ceremony._load_key(
-            "/p/key", KeyType.KEY_TYPE_ED25519.value, "pwd", None
-        )
-        assert result == ceremony.RSTUFKey(
-            {}, None, error=":cross_mark: [red]Failed[/]: permission denied"
-        )
-
-    def test__send_bootstrap(self, test_context):
-        test_context["settings"].SERVER = "http://fake-rstuf"
-        ceremony.get_headers = pretend.call_recorder(
-            lambda *a: {"auth": "token"}
-        )
-        ceremony.request_server = pretend.call_recorder(
-            lambda *a, **kw: pretend.stub(
-                status_code=202,
-                json=pretend.call_recorder(
-                    lambda: {
-                        "data": {"task_id": "task_id_123"},
-                        "message": "Bootstrap accepted.",
-                    }
-                ),
-            )
-        )
-
-        result = ceremony._send_bootstrap(
-            test_context["settings"], {"payload": "data"}
-        )
-        assert result == "task_id_123"
-        assert ceremony.get_headers.calls == [
-            pretend.call(test_context["settings"])
-        ]
-        assert ceremony.request_server.calls == [
-            pretend.call(
-                test_context["settings"].SERVER,
-                ceremony.URL.bootstrap.value,
-                ceremony.Methods.post,
-                {"payload": "data"},
-                headers={"auth": "token"},
-            )
-        ]
-
-    def test__send_bootstrap_not_202(self, test_context):
-        test_context["settings"].SERVER = "http://fake-rstuf"
-        ceremony.get_headers = pretend.call_recorder(
-            lambda *a: {"auth": "token"}
-        )
-        ceremony.request_server = pretend.call_recorder(
-            lambda *a, **kw: pretend.stub(
-                status_code=200,
-                json=pretend.call_recorder(
-                    lambda: {
-                        "data": {"task_id": "task_id_123"},
-                        "message": "Bootstrap accepted.",
-                    }
-                ),
-                text="Unexpected result data",
-            )
-        )
-
-        with pytest.raises(ceremony.click.ClickException) as err:
-            ceremony._send_bootstrap(
-                test_context["settings"], {"payload": "data"}
-            )
-
-        assert "Error 200" in str(err)
-        assert ceremony.get_headers.calls == [
-            pretend.call(test_context["settings"])
-        ]
-        assert ceremony.request_server.calls == [
-            pretend.call(
-                test_context["settings"].SERVER,
-                ceremony.URL.bootstrap.value,
-                ceremony.Methods.post,
-                {"payload": "data"},
-                headers={"auth": "token"},
-            )
-        ]
-
-    def test__send_bootstrap_no_message(self, test_context):
-        test_context["settings"].SERVER = "http://fake-rstuf"
-        ceremony.get_headers = pretend.call_recorder(
-            lambda *a: {"auth": "token"}
-        )
-        ceremony.request_server = pretend.call_recorder(
-            lambda *a, **kw: pretend.stub(
-                status_code=202,
-                json=pretend.call_recorder(
-                    lambda: {
-                        "data": {"task_id": "task_id_123"},
-                    }
-                ),
-                text="No message available.",
-            )
-        )
-
-        with pytest.raises(ceremony.click.ClickException) as err:
-            ceremony._send_bootstrap(
-                test_context["settings"], {"payload": "data"}
-            )
-
-        assert "No message available." in str(err)
-        assert ceremony.get_headers.calls == [
-            pretend.call(test_context["settings"])
-        ]
-        assert ceremony.request_server.calls == [
-            pretend.call(
-                test_context["settings"].SERVER,
-                ceremony.URL.bootstrap.value,
-                ceremony.Methods.post,
-                {"payload": "data"},
-                headers={"auth": "token"},
-            )
-        ]
-
-    def test__send_bootstrap_no_task_id(self, test_context):
-        test_context["settings"].SERVER = "http://fake-rstuf"
-        ceremony.get_headers = pretend.call_recorder(
-            lambda *a: {"auth": "token"}
-        )
-        ceremony.request_server = pretend.call_recorder(
-            lambda *a, **kw: pretend.stub(
-                status_code=202,
-                json=pretend.call_recorder(
-                    lambda: {
-                        "data": {"task_id": None},
-                        "message": "Bootstrap accepted.",
-                    }
-                ),
-                text="No task id",
-            )
-        )
-
-        with pytest.raises(ceremony.click.ClickException) as err:
-            ceremony._send_bootstrap(
-                test_context["settings"], {"payload": "data"}
-            )
-
-        assert "Failed to get `task id`" in str(err)
-        assert ceremony.get_headers.calls == [
-            pretend.call(test_context["settings"])
-        ]
-        assert ceremony.request_server.calls == [
-            pretend.call(
-                test_context["settings"].SERVER,
-                ceremony.URL.bootstrap.value,
-                ceremony.Methods.post,
-                {"payload": "data"},
-                headers={"auth": "token"},
-            )
-        ]
-
-    def test__send_bootstrap_no_data(self, test_context):
-        test_context["settings"].SERVER = "http://fake-rstuf"
-        ceremony.get_headers = pretend.call_recorder(
-            lambda *a: {"auth": "token"}
-        )
-        ceremony.request_server = pretend.call_recorder(
-            lambda *a, **kw: pretend.stub(
-                status_code=202,
-                json=pretend.call_recorder(
-                    lambda: {
-                        "data": {},
-                        "message": "Bootstrap accepted.",
-                    }
-                ),
-                text="No data",
-            )
-        )
-
-        with pytest.raises(ceremony.click.ClickException) as err:
-            ceremony._send_bootstrap(
-                test_context["settings"], {"payload": "data"}
-            )
-
-        assert "Failed to get task response data" in str(err)
-        assert ceremony.get_headers.calls == [
-            pretend.call(test_context["settings"])
-        ]
-        assert ceremony.request_server.calls == [
-            pretend.call(
-                test_context["settings"].SERVER,
-                ceremony.URL.bootstrap.value,
-                ceremony.Methods.post,
-                {"payload": "data"},
-                headers={"auth": "token"},
-            )
-        ]
-
-    def test__load_bootstrap_payload(self, monkeypatch):
-        fake_data = [
-            pretend.stub(read=pretend.call_recorder(lambda: b"{'k': 'v'}"))
-        ]
-        fake_file_obj = pretend.stub(
-            __enter__=pretend.call_recorder(lambda: fake_data),
-            __exit__=pretend.call_recorder(lambda *a: None),
-            close=pretend.call_recorder(lambda: None),
-            read=pretend.call_recorder(lambda: fake_data),
-        )
-        monkeypatch.setitem(
-            ceremony.__builtins__, "open", lambda *a: fake_file_obj
-        )
-        ceremony.json.load = pretend.call_recorder(lambda *a: {"k": "v"})
-
-        result = ceremony._load_bootstrap_payload("new_file")
-        assert result == {"k": "v"}
-        assert ceremony.json.load.calls == [pretend.call(fake_data)]
-
-    def test__load_bootstrap_payload_OSError(self, monkeypatch):
-        monkeypatch.setitem(
-            ceremony.__builtins__,
-            "open",
-            pretend.raiser(FileNotFoundError("payload.json not found")),
-        )
-        with pytest.raises(ceremony.click.ClickException) as err:
-            ceremony._load_bootstrap_payload("payload.json")
-
-        assert "Error to load payload.json" in str(err)
-        assert "payload.json not found" in str(err)
-
-    def test__save_bootstrap_payload(self, monkeypatch):
-        fake_data = pretend.stub(
-            write=pretend.call_recorder(lambda *a: "{'k': 'v'}")
-        )
-        fake_file_obj = pretend.stub(
-            __enter__=pretend.call_recorder(lambda: fake_data),
-            __exit__=pretend.call_recorder(lambda *a: None),
-            close=pretend.call_recorder(lambda: None),
-            write=pretend.call_recorder(lambda: fake_data),
-        )
-        monkeypatch.setitem(
-            ceremony.__builtins__, "open", lambda *a: fake_file_obj
-        )
-        monkeypatch.setattr(
-            ceremony.json,
-            "dumps",
-            pretend.call_recorder(lambda *a, **kw: "{'k': 'v'}"),
-        )
-
-        result = ceremony._save_bootstrap_payload("new_file", {"k": "v"})
-        assert result is None
-        assert ceremony.json.dumps.calls == [
-            pretend.call({"k": "v"}, indent=2)
-        ]
-
-    def test__save_bootstrap_payload_OSError(self, monkeypatch):
-        monkeypatch.setitem(
-            ceremony.__builtins__,
-            "open",
-            pretend.raiser(PermissionError("permission denied")),
-        )
-        with pytest.raises(ceremony.click.ClickException) as err:
-            ceremony._save_bootstrap_payload("payload.json", {"k": "v"})
-
-        assert "Failed to save payload.json" in str(err)
-        assert "permission denied" in str(err)
-
 
 class TestCeremonyInteraction:
     """Test the Ceremony Interaction"""
 
     def test_ceremony(self, client, test_context):
         test_result = client.invoke(ceremony.ceremony, obj=test_context)
         assert test_result.exit_code == 1
@@ -381,14 +84,52 @@
         )
 
         assert test_result.exit_code == 0, test_result.output
         assert "Ceremony done. 🔐 🎉." in test_result.output
         # passwords not shown in output
         assert "strongPass" not in test_result.output
 
+    def test_ceremony_negative_expiry_and_try_again(
+        self, client, test_context, test_inputs, test_setup
+    ):
+        ceremony.setup = test_setup
+        input_step1, input_step2, input_step3, input_step4 = test_inputs
+        # Adding two additional questions for root expiry because the last
+        # given values for the root expiration are below 1.
+        input_step1 = [
+            "y",  # Do you want more information about roles and responsibilities?  # noqa
+            "y",  # Do you want to start the ceremony?
+            "-1",  # What is the metadata expiration for the root role?(Days)
+            "0",  # What is the metadata expiration for the root role?(Days)
+            "",  # What is the metadata expiration for the root role?(Days)
+            "",  # What is the number of keys for the root role? (2)
+            "",  # What is the key threshold for root role signing?
+            "",  # What is the metadata expiration for the targets role?(Days) (365)?  # noqa
+            "y",  # Show example?
+            "16",  # Choose the number of delegated hash bin roles
+            "http://www.example.com/repository",  # What is the targets base URL  # noqa
+            "",  # What is the metadata expiration for the snapshot role?(Days) (365)?  # noqa
+            "",  # What is the metadata expiration for the timestamp role?(Days) (365)?  # noqa
+            "",  # What is the metadata expiration for the bins role?(Days) (365)?  # noqa
+            "Y",  # Ready to start loading the keys? Passwords will be required for keys [y/n]  # noqa
+        ]
+        test_result = client.invoke(
+            ceremony.ceremony,
+            "--save",
+            input="\n".join(
+                input_step1 + input_step2 + input_step3 + input_step4
+            ),
+            obj=test_context,
+        )
+
+        assert test_result.exit_code == 0, test_result.output
+        assert "Ceremony done. 🔐 🎉." in test_result.output
+        # passwords not shown in output
+        assert "strongPass" not in test_result.output
+
     def test_ceremony_key_bad_input_try_again_yes(
         self, client, test_context, test_inputs, test_setup
     ):
         ceremony.setup = test_setup
         input_step1, input_step2, input_step3, input_step4 = test_inputs
 
         # overwrite the input_step2
@@ -610,17 +351,15 @@
         )
 
         # mock ceremony process steps.
         # the process is tested in previous the test
         ceremony._run_ceremony_steps = pretend.call_recorder(
             lambda *a: {"k": "v"}
         )
-        ceremony._save_bootstrap_payload = pretend.call_recorder(
-            lambda *a: None
-        )
+        ceremony.save_payload = pretend.call_recorder(lambda *a: None)
 
         test_result = client.invoke(
             ceremony.ceremony,
             "--save",
             input="\n".join(
                 input_step1 + input_step2 + input_step3 + input_step4
             ),
@@ -630,15 +369,15 @@
         assert test_result.exit_code == 0, test_result.output
         assert "Ceremony done. 🔐 🎉." in test_result.output
         assert "Bootstrap payload (payload.json) saved." in test_result.output
         assert ceremony.os.makedirs.calls == [
             pretend.call("metadata", exist_ok=True)
         ]
         assert ceremony._run_ceremony_steps.calls == [pretend.call(True)]
-        assert ceremony._save_bootstrap_payload.calls == [
+        assert ceremony.save_payload.calls == [
             pretend.call("payload.json", {"k": "v"})
         ]
 
     def test_ceremony_option_save_OSError(
         self, client, test_context, test_inputs, test_setup, monkeypatch
     ):
         ceremony.setup = test_setup
@@ -669,45 +408,49 @@
     ):
         ceremony.setup = test_setup
         input_step1, input_step2, input_step3, input_step4 = test_inputs
 
         ceremony.bootstrap_status = pretend.call_recorder(
             lambda *a: {"data": {"bootstrap": False}}
         )
-        ceremony._send_bootstrap = pretend.call_recorder(
-            lambda *a: "fake_task_id"
+        ceremony.send_payload = pretend.call_recorder(
+            lambda **kw: "fake_task_id"
         )
         ceremony._run_ceremony_steps = pretend.call_recorder(
             lambda *a: {"k": "v"}
         )
-        ceremony._save_bootstrap_payload = pretend.call_recorder(
-            lambda *a: None
-        )
+        ceremony.save_payload = pretend.call_recorder(lambda *a: None)
         ceremony.task_status = pretend.call_recorder(lambda *a: None)
 
         test_result = client.invoke(
             ceremony.ceremony,
-            "--bootstrap",
+            ["--bootstrap", "--upload-server", "http://fake-api"],
             input="\n".join(
                 input_step1 + input_step2 + input_step3 + input_step4
             ),
             obj=test_context,
         )
 
         assert test_result.exit_code == 0, test_result.output
         assert "Ceremony done. 🔐 🎉." in test_result.output
         assert "Bootstrap completed." in test_result.output
         assert ceremony.bootstrap_status.calls == [
             pretend.call(test_context["settings"])
         ]
-        assert ceremony._send_bootstrap.calls == [
-            pretend.call(test_context["settings"], {"k": "v"})
+        assert ceremony.send_payload.calls == [
+            pretend.call(
+                settings=test_context["settings"],
+                url=URL.bootstrap.value,
+                payload={"k": "v"},
+                expected_msg="Bootstrap accepted.",
+                command_name="Bootstrap",
+            )
         ]
         assert ceremony._run_ceremony_steps.calls == [pretend.call(False)]
-        assert ceremony._save_bootstrap_payload.calls == [
+        assert ceremony.save_payload.calls == [
             pretend.call("payload.json", {"k": "v"})
         ]
         assert ceremony.task_status.calls == [
             pretend.call(
                 "fake_task_id", test_context["settings"], "Bootstrap status: "
             )
         ]
@@ -723,15 +466,15 @@
                 "data": {"bootstrap": True},
                 "message": "System LOCKED for bootstrap",
             }
         )
 
         test_result = client.invoke(
             ceremony.ceremony,
-            "--bootstrap",
+            ["--bootstrap", "--upload-server", "http://fake-api"],
             input="\n".join(
                 input_step1 + input_step2 + input_step3 + input_step4
             ),
             obj=test_context,
         )
 
         assert test_result.exit_code == 1, test_result.output
@@ -740,111 +483,110 @@
             pretend.call(test_context["settings"])
         ]
 
     def test_ceremony_option_bootstrap_upload(self, client, test_context):
         ceremony.bootstrap_status = pretend.call_recorder(
             lambda *a: {"data": {"bootstrap": False}}
         )
-        ceremony._load_bootstrap_payload = pretend.call_recorder(
-            lambda *a: {"k": "v"}
-        )
-        ceremony._send_bootstrap = pretend.call_recorder(
-            lambda *a: "fake_task_id"
+        ceremony.load_payload = pretend.call_recorder(lambda *a: {"k": "v"})
+        ceremony.send_payload = pretend.call_recorder(
+            lambda **kw: "fake_task_id"
         )
         ceremony.task_status = pretend.call_recorder(lambda *a: None)
 
-        test_context["settings"].SERVER = "http://server"
         test_result = client.invoke(
             ceremony.ceremony,
-            ["--bootstrap", "--upload"],
+            ["--bootstrap", "--upload", "--upload-server", "http://fake-api"],
             input=None,
             obj=test_context,
         )
 
         assert test_result.exit_code == 0, test_result.output
         assert (
             "Bootstrap completed using `payload.json`. 🔐 🎉"
             in test_result.output
         )
         assert ceremony.bootstrap_status.calls == [
             pretend.call(test_context["settings"])
         ]
-        assert ceremony._load_bootstrap_payload.calls == [
-            pretend.call("payload.json")
-        ]
-        assert ceremony._send_bootstrap.calls == [
-            pretend.call(test_context["settings"], {"k": "v"})
+        assert ceremony.load_payload.calls == [pretend.call("payload.json")]
+        assert ceremony.send_payload.calls == [
+            pretend.call(
+                settings=test_context["settings"],
+                url=URL.bootstrap.value,
+                payload={"k": "v"},
+                expected_msg="Bootstrap accepted.",
+                command_name="Bootstrap",
+            )
         ]
         assert ceremony.task_status.calls == [
             pretend.call(
                 "fake_task_id", test_context["settings"], "Bootstrap status: "
             )
         ]
         # test regression https://github.com/repository-service-tuf/repository-service-tuf-cli/pull/259  # noqa
         assert test_context["settings"].SERVER is not None
 
+    def test_ceremony_option_bootstrap_upload_missing_upload_server(
+        self, client, test_context
+    ):
+        test_result = client.invoke(
+            ceremony.ceremony,
+            ["--bootstrap", "--upload"],
+            input=None,
+            obj=test_context,
+        )
+
+        assert test_result.exit_code == 1, test_result.output
+        assert "Requires '--upload-server'" in test_result.output
+
     def test_ceremony_option_bootstrap_upload_auth(self, client, test_context):
         ceremony.bootstrap_status = pretend.call_recorder(
             lambda *a: {"data": {"bootstrap": False}}
         )
-        ceremony._load_bootstrap_payload = pretend.call_recorder(
-            lambda *a: {"k": "v"}
-        )
-        ceremony._send_bootstrap = pretend.call_recorder(
-            lambda *a: "fake_task_id"
+        ceremony.load_payload = pretend.call_recorder(lambda *a: {"k": "v"})
+        ceremony.send_payload = pretend.call_recorder(
+            lambda **kw: "fake_task_id"
         )
         ceremony.task_status = pretend.call_recorder(lambda *a: None)
 
         test_context["settings"].AUTH = True
+        test_context["settings"].SERVER = "http://fake-api"
 
         test_result = client.invoke(
             ceremony.ceremony,
-            ["--bootstrap", "--upload", "--upload-server", "http://rstuf"],
+            ["--bootstrap", "--upload"],
             input=None,
             obj=test_context,
         )
 
         assert test_result.exit_code == 0, test_result.output
         assert (
             "Bootstrap completed using `payload.json`. 🔐 🎉"
             in test_result.output
         )
         assert ceremony.bootstrap_status.calls == [
             pretend.call(test_context["settings"])
         ]
-        assert ceremony._load_bootstrap_payload.calls == [
-            pretend.call("payload.json")
-        ]
-        assert ceremony._send_bootstrap.calls == [
-            pretend.call(test_context["settings"], {"k": "v"})
+        assert ceremony.load_payload.calls == [pretend.call("payload.json")]
+        assert ceremony.send_payload.calls == [
+            pretend.call(
+                settings=test_context["settings"],
+                url=URL.bootstrap.value,
+                payload={"k": "v"},
+                expected_msg="Bootstrap accepted.",
+                command_name="Bootstrap",
+            )
         ]
         assert ceremony.task_status.calls == [
             pretend.call(
                 "fake_task_id", test_context["settings"], "Bootstrap status: "
             )
         ]
 
-    def test_ceremony_option_bootstrap_upload_auth_missing_upload_server(
-        self, client, test_context
-    ):
-        test_context["settings"].AUTH = True
-
-        test_result = client.invoke(
-            ceremony.ceremony,
-            ["--bootstrap", "--upload"],
-            input=None,
-            obj=test_context,
-        )
-
-        assert test_result.exit_code == 1, test_result.output
-        assert (
-            "Requires '--upload-server' when using '--auth'"
-            in test_result.output
-        )
-
     def test_ceremony_option_upload_missing_bootstrap(
         self, client, test_context, test_inputs, test_setup
     ):
         ceremony.setup = test_setup
         input_step1, input_step2, input_step3, input_step4 = test_inputs
 
         ceremony.bootstrap_status = pretend.call_recorder(
```

### Comparing `repository_service_tuf-0.3.0a1/tests/unit/cli/admin/test_import_targets.py` & `repository_service_tuf-0.4.0b1/tests/unit/cli/admin/test_import_targets.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,32 @@
         ]
 
     def test__parse_csv_data(self, monkeypatch):
         fake_data = [
             "path/file1;123;blake2b-256;hash1",
             "path/file2;456;blake2b-256;hash2",
         ]
+        db = pretend.stub(
+            execute=pretend.call_recorder(
+                lambda *a: pretend.stub(
+                    one=pretend.call_recorder(lambda: [15])
+                )
+            )
+        )
+        succinct_roles = pretend.stub(
+            get_role_for_target=pretend.call_recorder(lambda *a: "bins-e")
+        )
+        rstuf_target_roles = pretend.stub(
+            c=pretend.stub(rolename="bins-e"),
+            select=pretend.call_recorder(
+                lambda: pretend.stub(
+                    where=pretend.call_recorder(lambda *a: True)
+                )
+            ),
+        )
         fake_file_obj = pretend.stub(
             __enter__=pretend.call_recorder(lambda: fake_data),
             __exit__=pretend.call_recorder(lambda *a: None),
             close=pretend.call_recorder(lambda: None),
             read=pretend.call_recorder(lambda: fake_data),
         )
         monkeypatch.setitem(
@@ -60,164 +78,177 @@
             "repository_service_tuf.cli.admin.import_targets.datetime",
             fake_datetime,
         )
         succinct_roles = pretend.stub(
             get_role_for_target=pretend.call_recorder(lambda *a: "bins-a")
         )
 
-        result = import_targets._parse_csv_data("fake_file", succinct_roles)
+        result = import_targets._parse_csv_data(
+            db, rstuf_target_roles, succinct_roles, "fake_file"
+        )
 
         assert result == [
             {
                 "path": "path/file1",
                 "info": {"length": 123, "hashes": {"blake2b-256": "hash1"}},
-                "rolename": "bins-a",
+                "targets_role": 15,
                 "published": False,
                 "action": "ADD",
                 "last_update": datetime.datetime(2019, 6, 16, 9, 5, 1),
             },
             {
                 "path": "path/file2",
                 "info": {"length": 456, "hashes": {"blake2b-256": "hash2"}},
-                "rolename": "bins-a",
+                "targets_role": 15,
                 "published": False,
                 "action": "ADD",
                 "last_update": datetime.datetime(2019, 6, 16, 9, 5, 1),
             },
         ]
+        assert db.execute.calls == [pretend.call(True), pretend.call(True)]
+        assert succinct_roles.get_role_for_target.calls == [
+            pretend.call("path/file1"),
+            pretend.call("path/file2"),
+        ]
 
     def test__import_csv_to_rstuf(self):
-        fake_rstuf_table = pretend.stub(
+        fake_rstuf_files = pretend.stub(
             insert=pretend.call_recorder(lambda: None)
         )
         fake_db_client = pretend.stub(
             execute=pretend.call_recorder(lambda *a: None)
         )
         import_targets._parse_csv_data = pretend.call_recorder(
             lambda *a: [{"k1": "v1", "k2": "v2"}]
         )
 
         result = import_targets._import_csv_to_rstuf(
             fake_db_client,
-            fake_rstuf_table,
+            fake_rstuf_files,
+            "fake_rstuf_roles",
             ["csv1", "csv2"],
             "fake_succinct_roles",
         )
 
         assert result is None
         assert import_targets._parse_csv_data.calls == [
-            pretend.call("csv1", "fake_succinct_roles"),
-            pretend.call("csv2", "fake_succinct_roles"),
-        ]
-        assert fake_db_client.execute.calls == [
             pretend.call(
-                fake_rstuf_table.insert(), [{"k1": "v1", "k2": "v2"}]
+                fake_db_client,
+                "fake_rstuf_roles",
+                "fake_succinct_roles",
+                "csv1",
             ),
             pretend.call(
-                fake_rstuf_table.insert(), [{"k1": "v1", "k2": "v2"}]
+                fake_db_client,
+                "fake_rstuf_roles",
+                "fake_succinct_roles",
+                "csv2",
             ),
         ]
-        assert fake_rstuf_table.insert.calls == [
-            pretend.call(),
-            pretend.call(),
+        assert fake_db_client.execute.calls == [
+            pretend.call(None, [{"k1": "v1", "k2": "v2"}]),
+            pretend.call(None, [{"k1": "v1", "k2": "v2"}]),
+        ]
+        assert fake_rstuf_files.insert.calls == [
             pretend.call(),
             pretend.call(),
         ]
 
     def test__import_csv_to_rstuf_duplicate_targets(self):
         # Required to raise an exception type from import inside a function
         from sqlalchemy.exc import IntegrityError
 
-        fake_rstuf_table = pretend.stub(
+        fake_rstuf_files = pretend.stub(
             insert=pretend.raiser(IntegrityError("Duplicate", "param", "orig"))
         )
         fake_db_client = pretend.stub(
             execute=pretend.call_recorder(lambda *a: None)
         )
         import_targets._parse_csv_data = pretend.call_recorder(
             lambda *a: [{"k1": "v1", "k2": "v2"}]
         )
 
         with pytest.raises(import_targets.click.ClickException) as err:
             import_targets._import_csv_to_rstuf(
                 fake_db_client,
-                fake_rstuf_table,
+                fake_rstuf_files,
+                "fake_rstuf_roles",
                 ["csv1", "csv2"],
                 "fake_succinct_roles",
             )
-
         assert "ABORTED due duplicated targets." in str(err)
         assert import_targets._parse_csv_data.calls == [
-            pretend.call("csv1", "fake_succinct_roles"),
+            pretend.call(
+                fake_db_client,
+                "fake_rstuf_roles",
+                "fake_succinct_roles",
+                "csv1",
+            ),
         ]
 
-    def test__get_succinct_roles(self, monkeypatch):
-        import_targets.request_server = pretend.call_recorder(
-            lambda *a: pretend.stub(status_code=200, text=b"data")
+    def test__get_succinct_roles(self):
+        fake_response = pretend.stub(
+            status_code=200,
+            json=pretend.call_recorder(
+                lambda: {"data": {"number_of_delegated_bins": 16}}
+            ),
         )
-        monkeypatch.setattr(
-            import_targets.json, "loads", lambda *a: "json_data"
+        import_targets.request_server = pretend.call_recorder(
+            lambda *a: fake_response
         )
-        import_targets.Metadata.from_dict = pretend.call_recorder(
-            lambda *a: pretend.stub(
-                signed=pretend.stub(
-                    delegations=pretend.stub(
-                        succinct_roles="fake_succinct_roles"
-                    )
-                )
-            )
+        import_targets.SuccinctRoles = pretend.call_recorder(
+            lambda **kw: "fake_succinct_roles"
         )
 
-        result = import_targets._get_succinct_roles(
-            "http://127.0.0.1/metadata"
-        )
+        result = import_targets._get_succinct_roles("http://127.0.0.1")
         assert result == "fake_succinct_roles"
+        assert import_targets.request_server.calls == [
+            pretend.call(
+                "http://127.0.0.1",
+                import_targets.URL.config.value,
+                import_targets.Methods.get,
+            )
+        ]
+        assert import_targets.SuccinctRoles.calls == [
+            pretend.call(
+                keyids=[], threshold=1, bit_length=4, name_prefix="bins"
+            )
+        ]
+        assert fake_response.json.calls == [pretend.call()]
 
-    def test__get_succinct_roles_not_found_metadata(self, monkeypatch):
+    def test__get_succinct_roles_failed_retrieve_config(self):
         import_targets.request_server = pretend.call_recorder(
-            lambda *a: pretend.stub(status_code=404, text=b"data")
+            lambda *a: pretend.stub(status_code=404, text="Not found")
         )
 
         with pytest.raises(import_targets.click.ClickException) as err:
             import_targets._get_succinct_roles("http://127.0.0.1/metadata")
-        assert "RSTUF Metadata Targets not found." in str(err)
+        assert "Failed to retrieve RSTUF config" in str(err)
 
-    def test__get_succinct_roles_no_delegations(self, monkeypatch):
-        import_targets.request_server = pretend.call_recorder(
-            lambda *a: pretend.stub(status_code=200, text=b"data")
-        )
-        monkeypatch.setattr(
-            import_targets.json, "loads", lambda *a: "json_data"
-        )
-        import_targets.Metadata.from_dict = pretend.call_recorder(
-            lambda *a: pretend.stub(signed=pretend.stub(delegations=None))
+    def test__get_succinct_roles_failed_parsing(self, monkeypatch):
+        fake_response = pretend.stub(
+            status_code=200,
+            json=pretend.call_recorder(lambda: {"data": {}}),
+            text="{'data': {}}",
         )
-
-        with pytest.raises(import_targets.click.ClickException) as err:
-            import_targets._get_succinct_roles("http://127.0.0.1/metadata")
-        assert "Failed to get Targets Delegations" in str(err)
-
-    def test__get_succinct_roles_no_succinct_roles(self, monkeypatch):
         import_targets.request_server = pretend.call_recorder(
-            lambda *a: pretend.stub(status_code=200, text=b"data")
-        )
-        monkeypatch.setattr(
-            import_targets.json, "loads", lambda *a: "json_data"
-        )
-        import_targets.Metadata.from_dict = pretend.call_recorder(
-            lambda *a: pretend.stub(
-                signed=pretend.stub(
-                    delegations=pretend.stub(succinct_roles=None)
-                )
-            )
+            lambda *a: fake_response
         )
 
         with pytest.raises(import_targets.click.ClickException) as err:
-            import_targets._get_succinct_roles("http://127.0.0.1/metadata")
-        assert "Failed to get Targets succinct roles" in str(err)
+            import_targets._get_succinct_roles("http://127.0.0.1")
+        assert "Failed to parse 'data', 'number_of_delegated_bins'" in str(err)
+        assert import_targets.request_server.calls == [
+            pretend.call(
+                "http://127.0.0.1",
+                import_targets.URL.config.value,
+                import_targets.Methods.get,
+            )
+        ]
+        assert fake_response.json.calls == [pretend.call()]
 
 
 class TestImportTargetsGroupCLI:
     def test_import_targets(self, client, test_context):
         # Required to properly mock functions imported inside import_targets
         import sqlalchemy
 
@@ -251,16 +282,16 @@
             lambda *a: "fake_task_id"
         )
         import_targets.task_status = pretend.call_recorder(
             lambda *a: {"status": "SUCCESS"}
         )
 
         options = [
-            "--metadata-url",
-            "http://127.0.0.1/metadata/",
+            "--api-url",
+            "http://127.0.0.1",
             "--db-uri",
             "postgresql://postgres:secret@127.0.0.1:5433",
             "--csv",
             "targets1of2.csv",
             "--csv",
             "targets2of2.csv",
         ]
@@ -269,15 +300,15 @@
         )
         assert result.exit_code == 0, result.output
         assert "Finished." in result.output
         assert import_targets.bootstrap_status.calls == [
             pretend.call(test_context["settings"])
         ]
         assert import_targets._get_succinct_roles.calls == [
-            pretend.call("http://127.0.0.1/metadata/")
+            pretend.call("http://127.0.0.1")
         ]
         assert sqlalchemy.create_engine.calls == [
             pretend.call("postgresql://postgres:secret@127.0.0.1:5433")
         ]
         assert import_targets._check_csv_files.calls == [
             pretend.call(csv_files=("targets1of2.csv", "targets2of2.csv"))
         ]
@@ -326,16 +357,16 @@
             lambda *a: "fake_task_id"
         )
         import_targets.task_status = pretend.call_recorder(
             lambda *a: {"status": "SUCCESS"}
         )
 
         options = [
-            "--metadata-url",
-            "http://127.0.0.1/metadata/",
+            "--api-url",
+            "http://127.0.0.1",
             "--db-uri",
             "postgresql://postgres:secret@127.0.0.1:5433",
             "--csv",
             "targets1of2.csv",
             "--csv",
             "targets2of2.csv",
             "--skip-publish-targets",
@@ -346,15 +377,15 @@
         assert result.exit_code == 0, result.output
         assert "Finished." in result.output
         assert "Not targets published" in result.output
         assert import_targets.bootstrap_status.calls == [
             pretend.call(test_context["settings"])
         ]
         assert import_targets._get_succinct_roles.calls == [
-            pretend.call("http://127.0.0.1/metadata/")
+            pretend.call("http://127.0.0.1")
         ]
         assert sqlalchemy.create_engine.calls == [
             pretend.call("postgresql://postgres:secret@127.0.0.1:5433")
         ]
         assert import_targets._check_csv_files.calls == [
             pretend.call(csv_files=("targets1of2.csv", "targets2of2.csv"))
         ]
@@ -375,15 +406,15 @@
                 raise ModuleNotFoundError()
 
             return real_import(name, *args, **kwargs)
 
         builtins.__import__ = fake_import
 
         test_context["settings"].SERVER = "fake-server"
-        options = ["--metadata-url", "", "--db-uri", "", "--csv", ""]
+        options = ["--api-url", "", "--db-uri", "", "--csv", ""]
         result = client.invoke(
             import_targets.import_targets, options, obj=test_context
         )
 
         # Return the original import to not cause other exceptions.
         builtins.__import__ = real_import
 
@@ -396,16 +427,16 @@
         test_context["settings"].SERVER = "fake-server"
 
         import_targets.bootstrap_status = pretend.raiser(
             import_targets.click.ClickException("Server ERROR")
         )
 
         options = [
-            "--metadata-url",
-            "http://127.0.0.1/metadata/",
+            "--api-url",
+            "http://127.0.0.1",
             "--db-uri",
             "postgresql://postgres:secret@127.0.0.1:5433",
             "--csv",
             "targets1of2.csv",
             "--csv",
             "targets2of2.csv",
         ]
@@ -420,16 +451,16 @@
         test_context["settings"].SERVER = "fake-server"
 
         import_targets.bootstrap_status = pretend.call_recorder(
             lambda *a: {"data": {"bootstrap": False}, "message": "some msg"}
         )
 
         options = [
-            "--metadata-url",
-            "http://127.0.0.1/metadata/",
+            "--api-url",
+            "http://127.0.0.1",
             "--db-uri",
             "postgresql://postgres:secret@127.0.0.1:5433",
             "--csv",
             "targets1of2.csv",
             "--csv",
             "targets2of2.csv",
         ]
```

### Comparing `repository_service_tuf-0.3.0a1/tests/unit/cli/admin/test_login.py` & `repository_service_tuf-0.4.0b1/tests/unit/cli/admin/test_login.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,15 +51,14 @@
                 data=test_data,
             )
         ]
 
     def test_login(self, client, test_context):
         steps = [
             "http://test-rstuf",
-            "admin",
             "pass",
             "1",
         ]
         login._login = pretend.call_recorder(
             lambda *a: {"access_token": "fake-token"}
         )
         login.loaders = pretend.stub(
@@ -78,15 +77,14 @@
                 test_context["config"], test_context["settings"].to_dict()
             )
         ]
 
     def test_login_no_auth(self, client, test_context):
         steps = [
             "http://test-rstuf",
-            "admin",
             "pass",
             "1",
         ]
         login._login = pretend.call_recorder(
             lambda *a: {"access_token": "fake-token"}
         )
         login.loaders = pretend.stub(
@@ -102,15 +100,14 @@
     def test_login_force(self, client, test_context):
         # simulate the settings file
         test_context["settings"].SERVER = "fake-server"
         test_context["settings"].TOKEN = "test-token"
 
         steps = [
             "http://test-rstuf",
-            "admin",
             "pass",
             "1",
         ]
         login._login = pretend.call_recorder(
             lambda *a: {"access_token": "fake-token"}
         )
 
@@ -133,15 +130,14 @@
     def test_login_expired_token(self, client, test_context):
         # simulate the settings file with invalid/expired token
         test_context["settings"].SERVER = "http://test-rstuf"
         test_context["settings"].TOKEN = "fake-token"
 
         steps = [
             "http://test-rstuf",
-            "admin",
             "pass",
             "1",
         ]
 
         login.is_logged = pretend.call_recorder(
             lambda *a: pretend.stub(state=False)
         )
@@ -171,15 +167,14 @@
     def test_login_already_logged(self, client, test_context):
         # simulate the settings file with invalid/expired token
         test_context["settings"].SERVER = "http://test-rstuf"
         test_context["settings"].TOKEN = "fake-token"
 
         steps = [
             "http://test-rstuf",
-            "admin",
             "pass",
             "1",
         ]
 
         login.is_logged = pretend.call_recorder(
             lambda *a: pretend.stub(
                 state=True,
@@ -207,15 +202,14 @@
             pretend.call(test_context["settings"])
         ]
 
     def test_login_missing_http_protocol(self, client, test_context):
         steps = [
             "test-rstuf",
             "http://test-rstuf",
-            "admin",
             "pass",
             "1",
         ]
 
         login._login = pretend.call_recorder(
             lambda *a: {"access_token": "fake-token"}
         )
@@ -228,15 +222,14 @@
             login.login, input="\n".join(steps), obj=test_context
         )
         assert test_result.exit_code == 0
         assert "Login successful." in test_result.output
 
     def test_login_with_server(self, client, test_context):
         steps = [
-            "admin",
             "pass",
             "1",
         ]
         login._login = pretend.call_recorder(
             lambda *a: {"access_token": "fake-token"}
         )
 
@@ -258,15 +251,14 @@
             pretend.call(
                 test_context["config"], test_context["settings"].to_dict()
             )
         ]
 
     def test_login_with_server_bad_address(self, client, test_context):
         steps = [
-            "admin",
             "pass",
             "1",
         ]
         login._login = pretend.call_recorder(
             lambda *a: {"access_token": "fake-token"}
         )
         test_context["settings"].AUTH = True
@@ -285,15 +277,14 @@
         )
 
     def test_login_with_server_bad_address_them_fixed(
         self, client, test_context
     ):
         steps = [
             "http://test-rstuf",
-            "admin",
             "pass",
             "1",
         ]
         login._login = pretend.call_recorder(
             lambda *a: {"access_token": "fake-token"}
         )
 
@@ -313,43 +304,14 @@
         assert "Login successful." in test_result.output
         assert login.loaders.write.calls == [
             pretend.call(
                 test_context["config"], test_context["settings"].to_dict()
             )
         ]
 
-    def test_login_with_server_user(self, client, test_context):
-        steps = [
-            "pass",
-            "1",
-        ]
-        login._login = pretend.call_recorder(
-            lambda *a: {"access_token": "fake-token"}
-        )
-
-        login.loaders = pretend.stub(
-            write=pretend.call_recorder(lambda *a: None)
-        )
-        test_context["settings"].AUTH = True
-
-        test_result = client.invoke(
-            login.login,
-            ["-s", "http://test-rstuf", "-u", "admin"],
-            input="\n".join(steps),
-            obj=test_context,
-        )
-
-        assert test_result.exit_code == 0
-        assert "Login successful." in test_result.output
-        assert login.loaders.write.calls == [
-            pretend.call(
-                test_context["config"], test_context["settings"].to_dict()
-            )
-        ]
-
     def test_login_with_server_user_pass(self, client, test_context):
         steps = [
             "pass",
             "1",
         ]
         login._login = pretend.call_recorder(
             lambda *a: {"access_token": "fake-token"}
@@ -358,15 +320,15 @@
         login.loaders = pretend.stub(
             write=pretend.call_recorder(lambda *a: None)
         )
         test_context["settings"].AUTH = True
 
         test_result = client.invoke(
             login.login,
-            ["-s", "http://test-rstuf", "-u", "admin", "-p", "pass"],
+            ["-s", "http://test-rstuf", "-p", "pass"],
             input="\n".join(steps),
             obj=test_context,
         )
 
         assert test_result.exit_code == 0
         assert "Login successful." in test_result.output
         assert login.loaders.write.calls == [
@@ -386,16 +348,14 @@
         test_context["settings"].AUTH = True
 
         test_result = client.invoke(
             login.login,
             [
                 "-s",
                 "http://test-rstuf",
-                "-u",
-                "admin",
                 "-p",
                 "pass",
                 "-e",
                 "1",
             ],
             obj=test_context,
         )
```

### Comparing `repository_service_tuf-0.3.0a1/tests/unit/cli/key/test_generate_key.py` & `repository_service_tuf-0.4.0b1/tests/unit/cli/key/test_generate_key.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.3.0a1/tests/unit/helpers/test_api_client.py` & `repository_service_tuf-0.4.0b1/tests/unit/helpers/test_api_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 #
 # SPDX-License-Identifier: MIT
 
 from unittest.mock import Mock
 
 import pretend
 import pytest
+import rich_click as click
 
 from repository_service_tuf.helpers import api_client
 
 
 class TestAPIClient:
+    path = "repository_service_tuf.helpers.api_client"
+
     def test_request_server_get(self):
         fake_response = pretend.stub(
             status_code=200,
             json=pretend.call_recorder(lambda: {"key": "value"}),
         )
         api_client.requests = pretend.stub(
             get=pretend.call_recorder(lambda *a, **kw: fake_response)
@@ -183,15 +186,15 @@
 
         assert result == {}
 
     def test_get_headers_never_logged(self):
         with pytest.raises(api_client.click.ClickException) as err:
             api_client.get_headers({})
 
-        assert "Login first. Run 'rstuf admin login'" in str(err)
+        assert "Login first. Run 'rstuf --auth admin login'" in str(err)
 
     def test_get_headers_is_logged_state_false(self, test_context):
         api_client.is_logged = pretend.call_recorder(
             lambda *a: api_client.Login(state=False, data={"expired": False})
         )
 
         test_context["settings"].SERVER = "http://server"
@@ -589,7 +592,263 @@
             pretend.call(
                 test_context["settings"].SERVER,
                 api_client.URL.publish_targets.value,
                 api_client.Methods.post,
                 headers={"Auth": "Token"},
             )
         ]
+
+    def test_send_payload(self, test_context):
+        test_context["settings"].SERVER = "http://fake-rstuf"
+        api_client.get_headers = pretend.call_recorder(
+            lambda *a: {"auth": "token"}
+        )
+        api_client.request_server = pretend.call_recorder(
+            lambda *a, **kw: pretend.stub(
+                status_code=202,
+                json=pretend.call_recorder(
+                    lambda: {
+                        "data": {"task_id": "task_id_123"},
+                        "message": "Bootstrap accepted.",
+                    }
+                ),
+            )
+        )
+        result = api_client.send_payload(
+            settings=test_context["settings"],
+            url=api_client.URL.bootstrap.value,
+            payload={"payload": "data"},
+            expected_msg="Bootstrap accepted.",
+            command_name="Bootstrap",
+        )
+        assert result == "task_id_123"
+        assert api_client.get_headers.calls == [
+            pretend.call(test_context["settings"])
+        ]
+        assert api_client.request_server.calls == [
+            pretend.call(
+                test_context["settings"].SERVER,
+                api_client.URL.bootstrap.value,
+                api_client.Methods.post,
+                {"payload": "data"},
+                headers={"auth": "token"},
+            )
+        ]
+
+    def test_send_payload_not_202(self, test_context):
+        test_context["settings"].SERVER = "http://fake-rstuf"
+        api_client.get_headers = pretend.call_recorder(
+            lambda *a: {"auth": "token"}
+        )
+        api_client.request_server = pretend.call_recorder(
+            lambda *a, **kw: pretend.stub(
+                status_code=200,
+                json=pretend.call_recorder(
+                    lambda: {
+                        "data": {"task_id": "task_id_123"},
+                        "message": "Bootstrap accepted.",
+                    }
+                ),
+                text="Unexpected result data",
+            )
+        )
+
+        with pytest.raises(api_client.click.ClickException) as err:
+            api_client.send_payload(
+                settings=test_context["settings"],
+                url=api_client.URL.bootstrap.value,
+                payload={"payload": "data"},
+                expected_msg="Bootstrap accepted.",
+                command_name="Bootstrap",
+            )
+
+        assert "Error 200" in str(err)
+        assert api_client.get_headers.calls == [
+            pretend.call(test_context["settings"])
+        ]
+        assert api_client.request_server.calls == [
+            pretend.call(
+                test_context["settings"].SERVER,
+                api_client.URL.bootstrap.value,
+                api_client.Methods.post,
+                {"payload": "data"},
+                headers={"auth": "token"},
+            )
+        ]
+
+    def test_send_payload_no_message(self, test_context):
+        test_context["settings"].SERVER = "http://fake-rstuf"
+        api_client.get_headers = pretend.call_recorder(
+            lambda *a: {"auth": "token"}
+        )
+        api_client.request_server = pretend.call_recorder(
+            lambda *a, **kw: pretend.stub(
+                status_code=202,
+                json=pretend.call_recorder(
+                    lambda: {
+                        "data": {"task_id": "task_id_123"},
+                    }
+                ),
+                text="No message available.",
+            )
+        )
+
+        with pytest.raises(api_client.click.ClickException) as err:
+            api_client.send_payload(
+                settings=test_context["settings"],
+                url=api_client.URL.bootstrap.value,
+                payload={"payload": "data"},
+                expected_msg="Bootstrap accepted.",
+                command_name="Bootstrap",
+            )
+
+        assert "No message available." in str(err)
+        assert api_client.get_headers.calls == [
+            pretend.call(test_context["settings"])
+        ]
+        assert api_client.request_server.calls == [
+            pretend.call(
+                test_context["settings"].SERVER,
+                api_client.URL.bootstrap.value,
+                api_client.Methods.post,
+                {"payload": "data"},
+                headers={"auth": "token"},
+            )
+        ]
+
+    def test_send_payload_no_task_id(self, test_context):
+        test_context["settings"].SERVER = "http://fake-rstuf"
+        api_client.get_headers = pretend.call_recorder(
+            lambda *a: {"auth": "token"}
+        )
+        api_client.request_server = pretend.call_recorder(
+            lambda *a, **kw: pretend.stub(
+                status_code=202,
+                json=pretend.call_recorder(
+                    lambda: {
+                        "data": {"task_id": None},
+                        "message": "Bootstrap accepted.",
+                    }
+                ),
+                text="No task id",
+            )
+        )
+
+        with pytest.raises(api_client.click.ClickException) as err:
+            api_client.send_payload(
+                settings=test_context["settings"],
+                url=api_client.URL.bootstrap.value,
+                payload={"payload": "data"},
+                expected_msg="Bootstrap accepted.",
+                command_name="Bootstrap",
+            )
+
+        assert "Failed to get `task id`" in str(err)
+        assert api_client.get_headers.calls == [
+            pretend.call(test_context["settings"])
+        ]
+        assert api_client.request_server.calls == [
+            pretend.call(
+                test_context["settings"].SERVER,
+                api_client.URL.bootstrap.value,
+                api_client.Methods.post,
+                {"payload": "data"},
+                headers={"auth": "token"},
+            )
+        ]
+
+    def test_send_payload_no_data(self, test_context):
+        test_context["settings"].SERVER = "http://fake-rstuf"
+        api_client.get_headers = pretend.call_recorder(
+            lambda *a: {"auth": "token"}
+        )
+        api_client.request_server = pretend.call_recorder(
+            lambda *a, **kw: pretend.stub(
+                status_code=202,
+                json=pretend.call_recorder(
+                    lambda: {
+                        "data": {},
+                        "message": "Bootstrap accepted.",
+                    }
+                ),
+                text="No data",
+            )
+        )
+
+        with pytest.raises(api_client.click.ClickException) as err:
+            api_client.send_payload(
+                settings=test_context["settings"],
+                url=api_client.URL.bootstrap.value,
+                payload={"payload": "data"},
+                expected_msg="Bootstrap accepted.",
+                command_name="Bootstrap",
+            )
+
+        assert "Failed to get task response data" in str(err)
+        assert api_client.get_headers.calls == [
+            pretend.call(test_context["settings"])
+        ]
+        assert api_client.request_server.calls == [
+            pretend.call(
+                test_context["settings"].SERVER,
+                api_client.URL.bootstrap.value,
+                api_client.Methods.post,
+                {"payload": "data"},
+                headers={"auth": "token"},
+            )
+        ]
+
+    def test_get_md_file_local_file(self):
+        api_client.Metadata.from_file = pretend.call_recorder(
+            lambda *a: bytes("abc", "utf-8")
+        )
+        result = api_client.get_md_file("tests/files/root.json")
+        assert result == bytes("abc", "utf-8")
+        assert api_client.Metadata.from_file.calls == [
+            pretend.call("tests/files/root.json")
+        ]
+
+    def test_get_md_file_url(self, monkeypatch):
+        api_client.console.print = pretend.call_recorder(lambda *a: None)
+        api_client.requests.get = pretend.call_recorder(
+            lambda *a: pretend.stub(
+                status_code=200, content='{"metadata": "root"}'
+            )
+        )
+        fake_from_bytes = pretend.call_recorder(
+            lambda *a: bytes("abc", "utf-8")
+        )
+        monkeypatch.setattr(
+            f"{self.path}.Metadata.from_bytes", fake_from_bytes
+        )
+        file = "1.root.json"
+        url = f"http://localhost/{file}"
+        result = api_client.get_md_file(url)
+        assert result == bytes("abc", "utf-8")
+        assert api_client.console.print.calls == [
+            pretend.call(f"Fetching file {url}"),
+        ]
+        assert api_client.requests.get.calls == [
+            pretend.call(url),
+        ]
+        assert fake_from_bytes.calls == [pretend.call('{"metadata": "root"}')]
+
+    def test_get_md_file_url_response_not_200(self):
+        api_client.console.print = pretend.call_recorder(lambda *a: None)
+        api_client.requests.get = pretend.call_recorder(
+            lambda *a: pretend.stub(
+                status_code=404,
+            )
+        )
+        file = "1.root.json"
+        url = f"http://localhost/{file}"
+        with pytest.raises(click.ClickException) as err:
+            result = api_client.get_md_file(url)
+            assert result is None
+
+        assert f"Cannot fetch {url}" in str(err.value)
+        assert api_client.console.print.calls == [
+            pretend.call(f"Fetching file {url}"),
+        ]
+        assert api_client.requests.get.calls == [
+            pretend.call(url),
+        ]
```

### Comparing `repository_service_tuf-0.3.0a1/PKG-INFO` & `repository_service_tuf-0.4.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repository-service-tuf
-Version: 0.3.0a1
+Version: 0.4.0b1
 Summary: Repository Service for TUF Command Line Interface
 Author-email: Kairo de Araujo <kairo@dearaujo.nl>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

