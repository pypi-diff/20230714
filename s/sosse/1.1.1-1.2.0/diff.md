# Comparing `tmp/sosse-1.1.1.tar.gz` & `tmp/sosse-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosse-1.1.1.tar", last modified: Thu Jun 29 14:30:06 2023, max compression
+gzip compressed data, was "sosse-1.2.0.tar", last modified: Fri Jul 14 10:55:52 2023, max compression
```

## Comparing `sosse-1.1.1.tar` & `sosse-1.2.0.tar`

### file list

```diff
@@ -1,229 +1,230 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.108817 sosse-1.1.1/
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-06-29 14:29:39.000000 sosse-1.1.1/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      351 2023-06-29 14:29:39.000000 sosse-1.1.1/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.036820 sosse-1.1.1/.gitlab/
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-29 14:29:39.000000 sosse-1.1.1/.gitlab/changelog_config.yml
--rw-rw-rw-   0 root         (0) root         (0)     6963 2023-06-29 14:29:39.000000 sosse-1.1.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      491 2023-06-29 14:29:39.000000 sosse-1.1.1/.readthedocs.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-06-29 14:29:39.000000 sosse-1.1.1/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1659 2023-06-29 14:29:39.000000 sosse-1.1.1/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)    34523 2023-06-29 14:29:39.000000 sosse-1.1.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-29 14:29:39.000000 sosse-1.1.1/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     7600 2023-06-29 14:29:39.000000 sosse-1.1.1/Makefile
--rw-r--r--   0 root         (0) root         (0)     3198 2023-06-29 14:30:06.108817 sosse-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2806 2023-06-29 14:29:39.000000 sosse-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.040820 sosse-1.1.1/debian/
--rw-rw-rw-   0 root         (0) root         (0)      570 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/changelog
--rw-rw-rw-   0 root         (0) root         (0)        3 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/compat
--rw-rw-rw-   0 root         (0) root         (0)      697 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/control
--rwxrwxrwx   0 root         (0) root         (0)      182 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/rules
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/sosse-crawler.service
--rw-rw-rw-   0 root         (0) root         (0)      803 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/sosse-uwsgi.service
--rw-rw-rw-   0 root         (0) root         (0)     2176 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/sosse.conf
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/sosse.install
--rw-rw-rw-   0 root         (0) root         (0)     2733 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/sosse.postinst
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/uwsgi.ini
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-06-29 14:29:39.000000 sosse-1.1.1/debian/uwsgi.params
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.040820 sosse-1.1.1/doc/
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/Makefile
--rwxrwxrwx   0 root         (0) root         (0)      314 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/build_changelog.sh
--rw-rw-rw-   0 root         (0) root         (0)     1897 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/get_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.048819 sosse-1.1.1/doc/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.048819 sosse-1.1.1/doc/source/_extensions/
--rw-rw-rw-   0 root         (0) root         (0)     1124 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/_extensions/code_blocks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.048819 sosse-1.1.1/doc/source/_static/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/_static/style.css
--rw-rw-rw-   0 root         (0) root         (0)      723 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/admin_ui.rst
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/administration.rst
--rw-rw-rw-   0 root         (0) root         (0)      502 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/archive.rst
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/authentication.rst
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/cli.rst
--rw-rw-rw-   0 root         (0) root         (0)     1951 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/config_file.rst
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/cookies.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.052819 sosse-1.1.1/doc/source/crawl/
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/crawl/add_to_queue.rst
--rw-rw-rw-   0 root         (0) root         (0)     1452 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/crawl/crawl_depth.rst
--rw-rw-rw-   0 root         (0) root         (0)     5773 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/crawl/policies.rst
--rw-rw-rw-   0 root         (0) root         (0)      316 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/crawl/status.rst
--rw-rw-rw-   0 root         (0) root         (0)     1452 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/documents.rst
--rw-rw-rw-   0 root         (0) root         (0)     1408 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/domain_settings.rst
--rw-rw-rw-   0 root         (0) root         (0)      315 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/excluded_urls.rst
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.052819 sosse-1.1.1/doc/source/install/
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/install/database.rst.template
--rw-rw-rw-   0 root         (0) root         (0)     1463 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/install/debian.rst
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/install/debian_upgrades.rst
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/install/docker.rst
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/install/docker_upgrades.rst
--rw-rw-rw-   0 root         (0) root         (0)     3444 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/install/pip.rst
--rw-rw-rw-   0 root         (0) root         (0)      450 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/install/pip_upgrades.rst
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/install.rst
--rw-rw-rw-   0 root         (0) root         (0)      988 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/permissions.rst
--rw-rw-rw-   0 root         (0) root         (0)     1141 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/screenshots.rst
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/search_engines.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.056819 sosse-1.1.1/doc/source/user/
--rw-rw-rw-   0 root         (0) root         (0)      823 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/user/cached.rst
--rw-rw-rw-   0 root         (0) root         (0)      593 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/user/history.rst
--rw-rw-rw-   0 root         (0) root         (0)     1407 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/user/preferences.rst
--rw-rw-rw-   0 root         (0) root         (0)     4293 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/user/search.rst
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/user/shortcut_list.rst
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/user/shortcuts.rst
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/user/statistics.rst
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-06-29 14:29:39.000000 sosse-1.1.1/doc/source/user_doc.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.056819 sosse-1.1.1/docker/
--rw-rw-rw-   0 root         (0) root         (0)      882 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/Makefile.common
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.056819 sosse-1.1.1/docker/debian/
--rw-rw-rw-   0 root         (0) root         (0)     2006 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/debian/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/debian/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.056819 sosse-1.1.1/docker/debian-pkg/
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/debian-pkg/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/debian-pkg/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.060819 sosse-1.1.1/docker/debian-test/
--rw-rw-rw-   0 root         (0) root         (0)     1166 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/debian-test/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/debian-test/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.060819 sosse-1.1.1/docker/doc/
--rw-rw-rw-   0 root         (0) root         (0)      435 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/doc/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/doc/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.060819 sosse-1.1.1/docker/pip-base/
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/pip-base/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/pip-base/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.060819 sosse-1.1.1/docker/pip-release/
--rw-rw-rw-   0 root         (0) root         (0)     1489 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/pip-release/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/pip-release/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.060819 sosse-1.1.1/docker/pip-test/
--rw-rw-rw-   0 root         (0) root         (0)      617 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/pip-test/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-29 14:29:39.000000 sosse-1.1.1/docker/pip-test/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      892 2023-06-29 14:29:39.000000 sosse-1.1.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-29 14:29:39.000000 sosse-1.1.1/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.072818 sosse-1.1.1/se/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:29:39.000000 sosse-1.1.1/se/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20834 2023-06-29 14:29:39.000000 sosse-1.1.1/se/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      996 2023-06-29 14:29:39.000000 sosse-1.1.1/se/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     4121 2023-06-29 14:29:39.000000 sosse-1.1.1/se/atom.py
--rw-rw-rw-   0 root         (0) root         (0)    24429 2023-06-29 14:29:39.000000 sosse-1.1.1/se/browser.py
--rw-rw-rw-   0 root         (0) root         (0)     3135 2023-06-29 14:29:39.000000 sosse-1.1.1/se/cached.py
--rw-rw-rw-   0 root         (0) root         (0)     4314 2023-06-29 14:29:39.000000 sosse-1.1.1/se/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-06-29 14:29:39.000000 sosse-1.1.1/se/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.072818 sosse-1.1.1/se/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:29:39.000000 sosse-1.1.1/se/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.076818 sosse-1.1.1/se/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:29:39.000000 sosse-1.1.1/se/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4311 2023-06-29 14:29:39.000000 sosse-1.1.1/se/management/commands/crawl.py
--rw-rw-rw-   0 root         (0) root         (0)     1427 2023-06-29 14:29:39.000000 sosse-1.1.1/se/management/commands/default_admin.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-06-29 14:29:39.000000 sosse-1.1.1/se/management/commands/default_conf.py
--rw-rw-rw-   0 root         (0) root         (0)     6143 2023-06-29 14:29:39.000000 sosse-1.1.1/se/management/commands/extract_doc.py
--rw-rw-rw-   0 root         (0) root         (0)     1275 2023-06-29 14:29:39.000000 sosse-1.1.1/se/management/commands/generate_secret.py
--rw-rw-rw-   0 root         (0) root         (0)     1746 2023-06-29 14:29:39.000000 sosse-1.1.1/se/management/commands/load_se.py
--rw-rw-rw-   0 root         (0) root         (0)     2150 2023-06-29 14:29:39.000000 sosse-1.1.1/se/management/commands/update_se.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.076818 sosse-1.1.1/se/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    13998 2023-06-29 14:18:44.000000 sosse-1.1.1/se/migrations/0001_initial.py
--rwxrwxrwx   0 root         (0) root         (0)     2976 2023-06-29 14:18:44.000000 sosse-1.1.1/se/migrations/0002_search_vector.py
--rw-rw-rw-   0 root         (0) root         (0)     1143 2023-06-29 14:18:44.000000 sosse-1.1.1/se/migrations/0003_sosse_1_1_0.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:18:44.000000 sosse-1.1.1/se/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    56021 2023-06-29 14:29:39.000000 sosse-1.1.1/se/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1974 2023-06-29 14:29:39.000000 sosse-1.1.1/se/screenshot.py
--rw-rw-rw-   0 root         (0) root         (0)     6607 2023-06-29 14:29:39.000000 sosse-1.1.1/se/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.028820 sosse-1.1.1/se/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.084818 sosse-1.1.1/se/static/se/
--rw-rw-rw-   0 root         (0) root         (0)    19511 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/admin-base.css
--rw-rw-rw-   0 root         (0) root         (0)     8810 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/admin-forms.css
--rw-rw-rw-   0 root         (0) root         (0)     2005 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/base.js
--rw-rw-rw-   0 root         (0) root         (0)     2435 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/icon-atom.svg
--rw-rw-rw-   0 root         (0) root         (0)     2196 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/icon-clear.svg
--rw-rw-rw-   0 root         (0) root         (0)     3722 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/icon-cog.svg
--rw-rw-rw-   0 root         (0) root         (0)     6887 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/icon-search.svg
--rw-rw-rw-   0 root         (0) root         (0)     2488 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/icon-stats.svg
--rw-rw-rw-   0 root         (0) root         (0)     3644 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/icon-trash.svg
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/icon-user.svg
--rw-rw-rw-   0 root         (0) root         (0)     9798 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/index.js
--rw-rw-rw-   0 root         (0) root         (0)     4462 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/logo.png
--rw-rw-rw-   0 root         (0) root         (0)     9908 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/logo.svg
--rw-rw-rw-   0 root         (0) root         (0)     5967 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/pygal-tooltips.min.js
--rw-rw-rw-   0 root         (0) root         (0)      982 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/screenshot.js
--rw-rw-rw-   0 root         (0) root         (0)     2522 2023-06-29 14:29:39.000000 sosse-1.1.1/se/static/se/style.css
--rw-rw-rw-   0 root         (0) root         (0)     8567 2023-06-29 14:29:39.000000 sosse-1.1.1/se/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.028820 sosse-1.1.1/se/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.084818 sosse-1.1.1/se/templates/admin/
--rw-rw-rw-   0 root         (0) root         (0)     3427 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/admin/add_to_queue.html
--rw-rw-rw-   0 root         (0) root         (0)     2518 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/admin/app_list.html
--rw-rw-rw-   0 root         (0) root         (0)     2270 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/admin/base.html
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/admin/base_site.html
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/admin/change_form.html
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/admin/crawl_status.html
--rw-rw-rw-   0 root         (0) root         (0)     2706 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/admin/crawl_status_content.html
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/admin/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.092817 sosse-1.1.1/se/templates/se/
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/about.html
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/base.html
--rw-rw-rw-   0 root         (0) root         (0)     2285 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/cached.html
--rw-rw-rw-   0 root         (0) root         (0)     1870 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/history.html
--rw-rw-rw-   0 root         (0) root         (0)      671 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/home_browse.html
--rw-rw-rw-   0 root         (0) root         (0)     9293 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/index.html
--rw-rw-rw-   0 root         (0) root         (0)     1320 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/main_menu.html
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/opensearch.xml
--rw-rw-rw-   0 root         (0) root         (0)      761 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/pagination.html
--rw-rw-rw-   0 root         (0) root         (0)     2242 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/prefs.html
--rw-rw-rw-   0 root         (0) root         (0)     1706 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/screenshot.html
--rw-rw-rw-   0 root         (0) root         (0)     1523 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/search_redirect.html
--rw-rw-rw-   0 root         (0) root         (0)     1547 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/stats.html
--rw-rw-rw-   0 root         (0) root         (0)      741 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/unknown_url.html
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/words.html
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-29 14:29:39.000000 sosse-1.1.1/se/templates/se/www.html
--rw-rw-rw-   0 root         (0) root         (0)     5979 2023-06-29 14:29:39.000000 sosse-1.1.1/se/test_cookie.py
--rw-rw-rw-   0 root         (0) root         (0)    14987 2023-06-29 14:29:39.000000 sosse-1.1.1/se/test_crawl.py
--rw-rw-rw-   0 root         (0) root         (0)     9790 2023-06-29 14:29:39.000000 sosse-1.1.1/se/test_functionals.py
--rw-rw-rw-   0 root         (0) root         (0)     1459 2023-06-29 14:29:39.000000 sosse-1.1.1/se/test_misc.py
--rw-rw-rw-   0 root         (0) root         (0)     4659 2023-06-29 14:29:39.000000 sosse-1.1.1/se/test_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2133 2023-06-29 14:29:39.000000 sosse-1.1.1/se/test_redirect.py
--rw-rw-rw-   0 root         (0) root         (0)     1600 2023-06-29 14:29:39.000000 sosse-1.1.1/se/test_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     9547 2023-06-29 14:29:39.000000 sosse-1.1.1/se/test_search.py
--rw-rw-rw-   0 root         (0) root         (0)     2612 2023-06-29 14:29:39.000000 sosse-1.1.1/se/test_url.py
--rw-rw-rw-   0 root         (0) root         (0)     6326 2023-06-29 14:29:39.000000 sosse-1.1.1/se/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)     3101 2023-06-29 14:29:39.000000 sosse-1.1.1/se/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     8615 2023-06-29 14:29:39.000000 sosse-1.1.1/se/views.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-06-29 14:29:39.000000 sosse-1.1.1/se/words.py
--rw-rw-rw-   0 root         (0) root         (0)     2831 2023-06-29 14:29:39.000000 sosse-1.1.1/se/www.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 14:30:06.108817 sosse-1.1.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.096817 sosse-1.1.1/sosse/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 14:29:39.000000 sosse-1.1.1/sosse/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16990 2023-06-29 14:29:39.000000 sosse-1.1.1/sosse/conf.py
--rw-rw-rw-   0 root         (0) root         (0)    18193 2023-06-29 14:29:39.000000 sosse-1.1.1/sosse/search_engines.json
--rw-rw-rw-   0 root         (0) root         (0)     7433 2023-06-29 14:29:49.000000 sosse-1.1.1/sosse/settings.py
--rwxrwxrwx   0 root         (0) root         (0)     1328 2023-06-29 14:29:39.000000 sosse-1.1.1/sosse/sosse_admin.py
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-06-29 14:29:39.000000 sosse-1.1.1/sosse/test_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     2548 2023-06-29 14:29:39.000000 sosse-1.1.1/sosse/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2023-06-29 14:29:39.000000 sosse-1.1.1/sosse/wsgi.py
--rwxrwxrwx   0 root         (0) root         (0)       70 2023-06-29 14:29:39.000000 sosse-1.1.1/sosse-admin
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.100817 sosse-1.1.1/sosse.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3198 2023-06-29 14:30:05.000000 sosse-1.1.1/sosse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4845 2023-06-29 14:30:06.000000 sosse-1.1.1/sosse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 14:30:05.000000 sosse-1.1.1/sosse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-06-29 14:30:05.000000 sosse-1.1.1/sosse.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      129 2023-06-29 14:30:05.000000 sosse-1.1.1/sosse.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-29 14:30:05.000000 sosse-1.1.1/sosse.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.104817 sosse-1.1.1/tests/
--rwxrwxrwx   0 root         (0) root         (0)      281 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/build_doc.sh
--rw-rw-rw-   0 root         (0) root         (0)      809 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/cookies.json
--rwxrwxrwx   0 root         (0) root         (0)     1629 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/doc_test.sh
--rwxrwxrwx   0 root         (0) root         (0)      477 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/docker_run.sh
--rw-rw-rw-   0 root         (0) root         (0)     1015 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/document-ja.json
--rw-rw-rw-   0 root         (0) root         (0)      496 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/opensearch.xml
--rw-rw-rw-   0 root         (0) root         (0)      898 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/release.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.108817 sosse-1.1.1/tests/robotframework/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/robotframework/config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     7309 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/robotframework/home_docs.json
--rw-rw-rw-   0 root         (0) root         (0)    64349 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/robotframework/home_favicon.json
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/robotframework/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)      605 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/robotframework/start.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:30:06.108817 sosse-1.1.1/tests/robotframework/tests/
--rw-rw-rw-   0 root         (0) root         (0)     5212 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/robotframework/tests/01_crawl.robot
--rw-rw-rw-   0 root         (0) root         (0)     3334 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/robotframework/tests/02_user.robot
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/robotframework/tests/__init__.robot
--rw-rw-rw-   0 root         (0) root         (0)     1583 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/robotframework/tests/common.robot
--rw-rw-rw-   0 root         (0) root         (0)      467 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/searchhistory.json
--rwxrwxrwx   0 root         (0) root         (0)      938 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/test_app.sh
--rwxrwxrwx   0 root         (0) root         (0)      101 2023-06-29 14:29:39.000000 sosse-1.1.1/tests/wait_for_pg.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.913452 sosse-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-07-14 10:55:29.000000 sosse-1.2.0/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      371 2023-07-14 10:55:29.000000 sosse-1.2.0/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.801455 sosse-1.2.0/.gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-07-14 10:55:29.000000 sosse-1.2.0/.gitlab/changelog_config.yml
+-rw-rw-rw-   0 root         (0) root         (0)     7252 2023-07-14 10:55:29.000000 sosse-1.2.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-07-14 10:55:29.000000 sosse-1.2.0/.readthedocs.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1783 2023-07-14 10:55:29.000000 sosse-1.2.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2023-07-14 10:55:29.000000 sosse-1.2.0/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)    34523 2023-07-14 10:55:29.000000 sosse-1.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-14 10:55:29.000000 sosse-1.2.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     7687 2023-07-14 10:55:29.000000 sosse-1.2.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-07-14 10:55:52.909452 sosse-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2806 2023-07-14 10:55:29.000000 sosse-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.809454 sosse-1.2.0/debian/
+-rw-rw-rw-   0 root         (0) root         (0)      856 2023-07-14 10:55:29.000000 sosse-1.2.0/debian/changelog
+-rw-rw-rw-   0 root         (0) root         (0)        3 2023-07-14 10:55:29.000000 sosse-1.2.0/debian/compat
+-rw-rw-rw-   0 root         (0) root         (0)      697 2023-07-14 10:55:29.000000 sosse-1.2.0/debian/control
+-rwxrwxrwx   0 root         (0) root         (0)      182 2023-07-14 10:55:29.000000 sosse-1.2.0/debian/rules
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-07-14 10:55:29.000000 sosse-1.2.0/debian/sosse-crawler.service
+-rw-rw-rw-   0 root         (0) root         (0)      803 2023-07-14 10:55:29.000000 sosse-1.2.0/debian/sosse-uwsgi.service
+-rw-rw-rw-   0 root         (0) root         (0)     2176 2023-07-14 10:55:29.000000 sosse-1.2.0/debian/sosse.conf
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-07-14 10:55:29.000000 sosse-1.2.0/debian/sosse.install
+-rw-rw-rw-   0 root         (0) root         (0)     2733 2023-07-14 10:55:29.000000 sosse-1.2.0/debian/sosse.postinst
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-07-14 10:55:29.000000 sosse-1.2.0/debian/uwsgi.ini
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-14 10:55:29.000000 sosse-1.2.0/debian/uwsgi.params
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.809454 sosse-1.2.0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/Makefile
+-rwxrwxrwx   0 root         (0) root         (0)      314 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/build_changelog.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1897 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/get_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.821454 sosse-1.2.0/doc/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.821454 sosse-1.2.0/doc/source/_extensions/
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/_extensions/code_blocks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.821454 sosse-1.2.0/doc/source/_static/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/_static/style.css
+-rw-rw-rw-   0 root         (0) root         (0)      723 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/admin_ui.rst
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/administration.rst
+-rw-rw-rw-   0 root         (0) root         (0)      502 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/archive.rst
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/authentication.rst
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/cli.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1951 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/config_file.rst
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/cookies.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.825454 sosse-1.2.0/doc/source/crawl/
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/crawl/add_to_queue.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1452 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/crawl/crawl_depth.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5942 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/crawl/policies.rst
+-rw-rw-rw-   0 root         (0) root         (0)      316 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/crawl/status.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1452 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/documents.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1408 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/domain_settings.rst
+-rw-rw-rw-   0 root         (0) root         (0)      315 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/excluded_urls.rst
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.829454 sosse-1.2.0/doc/source/install/
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/install/database.rst.template
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/install/debian.rst
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/install/debian_upgrades.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/install/docker.rst
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/install/docker_upgrades.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3454 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/install/pip.rst
+-rw-rw-rw-   0 root         (0) root         (0)      450 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/install/pip_upgrades.rst
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/install.rst
+-rw-rw-rw-   0 root         (0) root         (0)      988 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/permissions.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/screenshots.rst
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/search_engines.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.833454 sosse-1.2.0/doc/source/user/
+-rw-rw-rw-   0 root         (0) root         (0)      823 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/user/cached.rst
+-rw-rw-rw-   0 root         (0) root         (0)      593 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/user/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/user/preferences.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/user/search.rst
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/user/shortcut_list.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/user/shortcuts.rst
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/user/statistics.rst
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-07-14 10:55:29.000000 sosse-1.2.0/doc/source/user_doc.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.833454 sosse-1.2.0/docker/
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-07-14 10:55:29.000000 sosse-1.2.0/docker/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-07-14 10:55:29.000000 sosse-1.2.0/docker/Makefile.common
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.837454 sosse-1.2.0/docker/debian/
+-rw-rw-rw-   0 root         (0) root         (0)     2006 2023-07-14 10:55:29.000000 sosse-1.2.0/docker/debian/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-14 10:55:29.000000 sosse-1.2.0/docker/debian/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.837454 sosse-1.2.0/docker/debian-pkg/
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-07-14 10:55:29.000000 sosse-1.2.0/docker/debian-pkg/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-14 10:55:29.000000 sosse-1.2.0/docker/debian-pkg/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.837454 sosse-1.2.0/docker/debian-test/
+-rw-rw-rw-   0 root         (0) root         (0)     1166 2023-07-14 10:55:29.000000 sosse-1.2.0/docker/debian-test/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-07-14 10:55:29.000000 sosse-1.2.0/docker/debian-test/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.837454 sosse-1.2.0/docker/doc/
+-rw-rw-rw-   0 root         (0) root         (0)      435 2023-07-14 10:55:29.000000 sosse-1.2.0/docker/doc/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-07-14 10:55:29.000000 sosse-1.2.0/docker/doc/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.841454 sosse-1.2.0/docker/pip-base/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-07-14 10:55:29.000000 sosse-1.2.0/docker/pip-base/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-14 10:55:29.000000 sosse-1.2.0/docker/pip-base/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.841454 sosse-1.2.0/docker/pip-release/
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2023-07-14 10:55:29.000000 sosse-1.2.0/docker/pip-release/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-07-14 10:55:29.000000 sosse-1.2.0/docker/pip-release/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.841454 sosse-1.2.0/docker/pip-test/
+-rw-rw-rw-   0 root         (0) root         (0)      617 2023-07-14 10:55:29.000000 sosse-1.2.0/docker/pip-test/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-14 10:55:29.000000 sosse-1.2.0/docker/pip-test/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      892 2023-07-14 10:55:29.000000 sosse-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-07-14 10:55:29.000000 sosse-1.2.0/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.857453 sosse-1.2.0/se/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 10:55:29.000000 sosse-1.2.0/se/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20857 2023-07-14 10:55:29.000000 sosse-1.2.0/se/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      996 2023-07-14 10:55:29.000000 sosse-1.2.0/se/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     4121 2023-07-14 10:55:29.000000 sosse-1.2.0/se/atom.py
+-rw-rw-rw-   0 root         (0) root         (0)    24917 2023-07-14 10:55:29.000000 sosse-1.2.0/se/browser.py
+-rw-rw-rw-   0 root         (0) root         (0)     3135 2023-07-14 10:55:29.000000 sosse-1.2.0/se/cached.py
+-rw-rw-rw-   0 root         (0) root         (0)     4314 2023-07-14 10:55:29.000000 sosse-1.2.0/se/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-07-14 10:55:29.000000 sosse-1.2.0/se/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.861453 sosse-1.2.0/se/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 10:55:29.000000 sosse-1.2.0/se/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.865453 sosse-1.2.0/se/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 10:55:29.000000 sosse-1.2.0/se/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4311 2023-07-14 10:55:29.000000 sosse-1.2.0/se/management/commands/crawl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2023-07-14 10:55:29.000000 sosse-1.2.0/se/management/commands/default_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-07-14 10:55:29.000000 sosse-1.2.0/se/management/commands/default_conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6143 2023-07-14 10:55:29.000000 sosse-1.2.0/se/management/commands/extract_doc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2023-07-14 10:55:29.000000 sosse-1.2.0/se/management/commands/generate_secret.py
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2023-07-14 10:55:29.000000 sosse-1.2.0/se/management/commands/load_se.py
+-rw-rw-rw-   0 root         (0) root         (0)     2150 2023-07-14 10:55:29.000000 sosse-1.2.0/se/management/commands/update_se.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.865453 sosse-1.2.0/se/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    13998 2023-07-14 10:52:54.000000 sosse-1.2.0/se/migrations/0001_initial.py
+-rwxrwxrwx   0 root         (0) root         (0)     2976 2023-07-14 10:52:54.000000 sosse-1.2.0/se/migrations/0002_search_vector.py
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2023-07-14 10:52:54.000000 sosse-1.2.0/se/migrations/0003_sosse_1_1_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1195 2023-07-14 10:52:54.000000 sosse-1.2.0/se/migrations/0004_sosse_1_2_0.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 10:52:54.000000 sosse-1.2.0/se/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    56451 2023-07-14 10:55:29.000000 sosse-1.2.0/se/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2023-07-14 10:55:29.000000 sosse-1.2.0/se/screenshot.py
+-rw-rw-rw-   0 root         (0) root         (0)     6607 2023-07-14 10:55:29.000000 sosse-1.2.0/se/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.789455 sosse-1.2.0/se/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.877453 sosse-1.2.0/se/static/se/
+-rw-rw-rw-   0 root         (0) root         (0)    19511 2023-07-14 10:55:29.000000 sosse-1.2.0/se/static/se/admin-base.css
+-rw-rw-rw-   0 root         (0) root         (0)     8810 2023-07-14 10:55:29.000000 sosse-1.2.0/se/static/se/admin-forms.css
+-rw-rw-rw-   0 root         (0) root         (0)     2005 2023-07-14 10:55:29.000000 sosse-1.2.0/se/static/se/base.js
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2023-07-14 10:55:29.000000 sosse-1.2.0/se/static/se/icon-atom.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2196 2023-07-14 10:55:29.000000 sosse-1.2.0/se/static/se/icon-clear.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3722 2023-07-14 10:55:29.000000 sosse-1.2.0/se/static/se/icon-cog.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2023-07-14 10:55:29.000000 sosse-1.2.0/se/static/se/icon-search.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2488 2023-07-14 10:55:29.000000 sosse-1.2.0/se/static/se/icon-stats.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3644 2023-07-14 10:55:29.000000 sosse-1.2.0/se/static/se/icon-trash.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-07-14 10:55:29.000000 sosse-1.2.0/se/static/se/icon-user.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9798 2023-07-14 10:55:29.000000 sosse-1.2.0/se/static/se/index.js
+-rw-rw-rw-   0 root         (0) root         (0)     4462 2023-07-14 10:55:29.000000 sosse-1.2.0/se/static/se/logo.png
+-rw-rw-rw-   0 root         (0) root         (0)     9908 2023-07-14 10:55:29.000000 sosse-1.2.0/se/static/se/logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     5967 2023-07-14 10:55:29.000000 sosse-1.2.0/se/static/se/pygal-tooltips.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-07-14 10:55:29.000000 sosse-1.2.0/se/static/se/screenshot.js
+-rw-rw-rw-   0 root         (0) root         (0)     2522 2023-07-14 10:55:29.000000 sosse-1.2.0/se/static/se/style.css
+-rw-rw-rw-   0 root         (0) root         (0)     8567 2023-07-14 10:55:29.000000 sosse-1.2.0/se/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.789455 sosse-1.2.0/se/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.881453 sosse-1.2.0/se/templates/admin/
+-rw-rw-rw-   0 root         (0) root         (0)     3427 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/admin/add_to_queue.html
+-rw-rw-rw-   0 root         (0) root         (0)     2518 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/admin/app_list.html
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/admin/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/admin/base_site.html
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/admin/change_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/admin/crawl_status.html
+-rw-rw-rw-   0 root         (0) root         (0)     3261 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/admin/crawl_status_content.html
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/admin/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.889453 sosse-1.2.0/se/templates/se/
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/se/about.html
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/se/base.html
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/se/cached.html
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/se/history.html
+-rw-rw-rw-   0 root         (0) root         (0)      671 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/se/home_browse.html
+-rw-rw-rw-   0 root         (0) root         (0)     9293 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/se/index.html
+-rw-rw-rw-   0 root         (0) root         (0)     1421 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/se/main_menu.html
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/se/opensearch.xml
+-rw-rw-rw-   0 root         (0) root         (0)      761 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/se/pagination.html
+-rw-rw-rw-   0 root         (0) root         (0)     2242 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/se/prefs.html
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/se/screenshot.html
+-rw-rw-rw-   0 root         (0) root         (0)     1523 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/se/search_redirect.html
+-rw-rw-rw-   0 root         (0) root         (0)     1547 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/se/stats.html
+-rw-rw-rw-   0 root         (0) root         (0)      741 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/se/unknown_url.html
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/se/words.html
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-07-14 10:55:29.000000 sosse-1.2.0/se/templates/se/www.html
+-rw-rw-rw-   0 root         (0) root         (0)     5979 2023-07-14 10:55:29.000000 sosse-1.2.0/se/test_cookie.py
+-rw-rw-rw-   0 root         (0) root         (0)    14987 2023-07-14 10:55:29.000000 sosse-1.2.0/se/test_crawl.py
+-rw-rw-rw-   0 root         (0) root         (0)     9790 2023-07-14 10:55:29.000000 sosse-1.2.0/se/test_functionals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1459 2023-07-14 10:55:29.000000 sosse-1.2.0/se/test_misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5282 2023-07-14 10:55:29.000000 sosse-1.2.0/se/test_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2133 2023-07-14 10:55:29.000000 sosse-1.2.0/se/test_redirect.py
+-rw-rw-rw-   0 root         (0) root         (0)     1600 2023-07-14 10:55:29.000000 sosse-1.2.0/se/test_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     9547 2023-07-14 10:55:29.000000 sosse-1.2.0/se/test_search.py
+-rw-rw-rw-   0 root         (0) root         (0)     2612 2023-07-14 10:55:29.000000 sosse-1.2.0/se/test_url.py
+-rw-rw-rw-   0 root         (0) root         (0)     6326 2023-07-14 10:55:29.000000 sosse-1.2.0/se/test_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     3101 2023-07-14 10:55:29.000000 sosse-1.2.0/se/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     8615 2023-07-14 10:55:29.000000 sosse-1.2.0/se/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-07-14 10:55:29.000000 sosse-1.2.0/se/words.py
+-rw-rw-rw-   0 root         (0) root         (0)     2831 2023-07-14 10:55:29.000000 sosse-1.2.0/se/www.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 10:55:52.913452 sosse-1.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.897452 sosse-1.2.0/sosse/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 10:55:29.000000 sosse-1.2.0/sosse/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16990 2023-07-14 10:55:29.000000 sosse-1.2.0/sosse/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)    18193 2023-07-14 10:55:29.000000 sosse-1.2.0/sosse/search_engines.json
+-rw-rw-rw-   0 root         (0) root         (0)     7433 2023-07-14 10:55:35.000000 sosse-1.2.0/sosse/settings.py
+-rwxrwxrwx   0 root         (0) root         (0)     1328 2023-07-14 10:55:29.000000 sosse-1.2.0/sosse/sosse_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-07-14 10:55:29.000000 sosse-1.2.0/sosse/test_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2548 2023-07-14 10:55:29.000000 sosse-1.2.0/sosse/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-07-14 10:55:29.000000 sosse-1.2.0/sosse/wsgi.py
+-rwxrwxrwx   0 root         (0) root         (0)       70 2023-07-14 10:55:29.000000 sosse-1.2.0/sosse-admin
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.901452 sosse-1.2.0/sosse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-07-14 10:55:52.000000 sosse-1.2.0/sosse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4879 2023-07-14 10:55:52.000000 sosse-1.2.0/sosse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 10:55:52.000000 sosse-1.2.0/sosse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-14 10:55:52.000000 sosse-1.2.0/sosse.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      129 2023-07-14 10:55:52.000000 sosse-1.2.0/sosse.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-14 10:55:52.000000 sosse-1.2.0/sosse.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.905452 sosse-1.2.0/tests/
+-rwxrwxrwx   0 root         (0) root         (0)      281 2023-07-14 10:55:29.000000 sosse-1.2.0/tests/build_doc.sh
+-rw-rw-rw-   0 root         (0) root         (0)      809 2023-07-14 10:55:29.000000 sosse-1.2.0/tests/cookies.json
+-rwxrwxrwx   0 root         (0) root         (0)     1629 2023-07-14 10:55:29.000000 sosse-1.2.0/tests/doc_test.sh
+-rwxrwxrwx   0 root         (0) root         (0)      477 2023-07-14 10:55:29.000000 sosse-1.2.0/tests/docker_run.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1015 2023-07-14 10:55:29.000000 sosse-1.2.0/tests/document-ja.json
+-rw-rw-rw-   0 root         (0) root         (0)      496 2023-07-14 10:55:29.000000 sosse-1.2.0/tests/opensearch.xml
+-rw-rw-rw-   0 root         (0) root         (0)      898 2023-07-14 10:55:29.000000 sosse-1.2.0/tests/release.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.909452 sosse-1.2.0/tests/robotframework/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-14 10:55:29.000000 sosse-1.2.0/tests/robotframework/config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     7309 2023-07-14 10:55:29.000000 sosse-1.2.0/tests/robotframework/home_docs.json
+-rw-rw-rw-   0 root         (0) root         (0)    64349 2023-07-14 10:55:29.000000 sosse-1.2.0/tests/robotframework/home_favicon.json
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-14 10:55:29.000000 sosse-1.2.0/tests/robotframework/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)      605 2023-07-14 10:55:29.000000 sosse-1.2.0/tests/robotframework/start.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:55:52.909452 sosse-1.2.0/tests/robotframework/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5212 2023-07-14 10:55:29.000000 sosse-1.2.0/tests/robotframework/tests/01_crawl.robot
+-rw-rw-rw-   0 root         (0) root         (0)     3334 2023-07-14 10:55:29.000000 sosse-1.2.0/tests/robotframework/tests/02_user.robot
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-07-14 10:55:29.000000 sosse-1.2.0/tests/robotframework/tests/__init__.robot
+-rw-rw-rw-   0 root         (0) root         (0)     1637 2023-07-14 10:55:29.000000 sosse-1.2.0/tests/robotframework/tests/common.robot
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-07-14 10:55:29.000000 sosse-1.2.0/tests/searchhistory.json
+-rwxrwxrwx   0 root         (0) root         (0)      938 2023-07-14 10:55:29.000000 sosse-1.2.0/tests/test_app.sh
+-rwxrwxrwx   0 root         (0) root         (0)      101 2023-07-14 10:55:29.000000 sosse-1.2.0/tests/wait_for_pg.sh
```

### Comparing `sosse-1.1.1/.gitlab-ci.yml` & `sosse-1.2.0/.gitlab-ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -87,14 +87,16 @@
       - doc/source/*/*_generated.rst
       - doc/source/CHANGELOG.md
   script:
     - ./sosse-admin extract_doc conf > doc/source/config_file_generated.rst
     - ./sosse-admin extract_doc cli > doc/source/cli_generated.rst
     - ./sosse-admin extract_doc se > doc/source/user/shortcut_list_generated.rst
     - ./doc/build_changelog.sh > doc/source/CHANGELOG.md
+    - sed -e 's#|sosse-admin|#sosse-admin#' doc/source/install/database.rst.template > doc/source/install/database_debian_generated.rst
+    - sed -e 's#|sosse-admin|#/opt/sosse-venv/bin/sosse-admin#' doc/source/install/database.rst.template > doc/source/install/database_pip_generated.rst
 
 doc_code_extract:
   image: biolds/sosse:doc
   stage: test
   needs:
     - doc_gen
   artifacts:
```

### Comparing `sosse-1.1.1/CHANGELOG.md` & `sosse-1.2.0/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+## 1.2.0 (2023-07-14)
+### Features (2 changes)
+- [crawling status improvements](biolds1/sosse@848fba81977bf56780430592261bd0847ee52110) ([merge request](biolds1/sosse!18))
+- [navigation elements removal](biolds1/sosse@0d9d3582486ed45202359fa5174aadc5bb945d3d) ([merge request](biolds1/sosse!16))
+### Bug fixes (1 change)
+- [fix screenshots resize](biolds1/sosse@5f6ca3441cd402b5d71ad77598b0e8a17c80dbd6) ([merge request](biolds1/sosse!17))
+
+## 1.1.2 (2023-06-30)
+### Bug fixes (1 change)
+- [fix database configuration documentation](biolds1/sosse@d10379ffbdfe19bbaef302822110641e9495f75a)
+
 ## 1.1.1 (2023-06-29)
 ### Bug fixes (1 change)
 - [misc Bookworm, Docker and Selenium fixes](biolds1/sosse@54fcc7043bfc34a6125fa301d58c08ea02e0b292) ([merge request](biolds1/sosse!12))
 
 ## 1.1.0 (2023-06-18)
 ### Features (3 changes)
 - [Debian Bookworm support](biolds1/sosse@b2112e5a0a526e777600499d726002ad62612aac) ([merge request](biolds1/sosse!10))
```

### Comparing `sosse-1.1.1/Dockerfile` & `sosse-1.2.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/LICENSE` & `sosse-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/Makefile` & `sosse-1.2.0/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,18 @@
 
 deb:
 	mkdir $(current_dir)/deb/ &>/dev/null ||:
 	docker run --rm -v $(current_dir):/sosse:ro -v $(current_dir)/deb:/deb biolds/sosse:debian-pkg bash -c 'cp -x -r /sosse /sosse-deb && make -C /sosse-deb _deb'
 
 _build_doc:
 	./doc/build_changelog.sh > doc/source/CHANGELOG.md
-	sed -e 's#|sosse-admin|#sosse-admin#' doc/source/install/database.rst.template > doc/source/install/database_debian.rst
-	sed -e 's#|sosse-admin|#/opt/sosse-venv/bin/sosse-admin#' doc/source/install/database.rst.template > doc/source/install/database_pip.rst
-	. /opt/sosse-doc/bin/activate ; make -C doc linkcheck html SPHINXOPTS="-W"
+	sed -e 's#|sosse-admin|#sosse-admin#' doc/source/install/database.rst.template > doc/source/install/database_debian_generated.rst
+	sed -e 's#|sosse-admin|#/opt/sosse-venv/bin/sosse-admin#' doc/source/install/database.rst.template > doc/source/install/database_pip_generated.rst
+	#. /opt/sosse-doc/bin/activate ; make -C doc linkcheck html SPHINXOPTS="-W"
+	. /opt/sosse-doc/bin/activate ; make -C doc html SPHINXOPTS="-W"
 	jq . < doc/code_blocks.json > /tmp/code_blocks.json
 	mv /tmp/code_blocks.json doc/code_blocks.json
 
 build_doc:
 	mkdir -p doc/build/
 	docker run --rm -v $(current_dir):/sosse:ro -v $(current_dir)/doc:/sosse/doc biolds/sosse:doc bash -c 'cd /sosse && make _build_doc'
```

### Comparing `sosse-1.1.1/PKG-INFO` & `sosse-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosse
-Version: 1.1.1
+Version: 1.2.0
 Summary: Selenium Open Source Search Engine
 Author-email: Laurent Defert <laurent_defert@yahoo.fr>
 License: GNU Affero General Public License v3
 Keywords: search engine,crawler
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sosse Version: 1.1.1 Summary: Selenium Open Source
+Metadata-Version: 2.1 Name: sosse Version: 1.2.0 Summary: Selenium Open Source
 Search Engine Author-email: Laurent Defert
 yahoo.fr> License: GNU Affero General Public License v3 Keywords: search
 engine,crawler Classifier: Framework :: Django Classifier: Programming Language
 :: Python :: 3 Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE
 [https://raw.githubusercontent.com/biolds/sosse/main/se/static/se/logo.svg]
 [https://img.shields.io/gitlab/pipeline-coverage/biolds1/
```

### Comparing `sosse-1.1.1/README.md` & `sosse-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/debian/changelog` & `sosse-1.2.0/debian/changelog`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+sosse (1.2.0-1) bookworm; urgency=medium
+
+  * Upstream release
+
+ -- Laurent Defert <laurent_defert@yahoo.fr>  Fri, 14 Jul 2023 11:21:11 +0200
+
+sosse (1.1.2-1) bookworm; urgency=medium
+
+  * Upstream release
+
+ -- Laurent Defert <laurent_defert@yahoo.fr>  Fri, 30 Jun 2023 20:52:18 +0200
+
 sosse (1.1.1-1) bookworm; urgency=medium
 
   * Upstream release
 
  -- Laurent Defert <laurent_defert@yahoo.fr>  Thu, 29 Jun 2023 16:03:50 +0200
 
 sosse (1.1.0-1) bookworm; urgency=medium
```

### Comparing `sosse-1.1.1/debian/control` & `sosse-1.2.0/debian/control`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/debian/sosse-crawler.service` & `sosse-1.2.0/debian/sosse-crawler.service`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/debian/sosse-uwsgi.service` & `sosse-1.2.0/debian/sosse-uwsgi.service`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/debian/sosse.conf` & `sosse-1.2.0/debian/sosse.conf`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/debian/sosse.postinst` & `sosse-1.2.0/debian/sosse.postinst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/debian/uwsgi.params` & `sosse-1.2.0/debian/uwsgi.params`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/Makefile` & `sosse-1.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/get_artifacts.py` & `sosse-1.2.0/doc/get_artifacts.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/make.bat` & `sosse-1.2.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/source/_extensions/code_blocks.py` & `sosse-1.2.0/doc/source/_extensions/code_blocks.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/source/admin_ui.rst` & `sosse-1.2.0/doc/source/admin_ui.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/source/authentication.rst` & `sosse-1.2.0/doc/source/authentication.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/source/conf.py` & `sosse-1.2.0/doc/source/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 import os
 import sys
 
 project = 'SOSSE'
 copyright = '2023, Laurent Defert'
 author = 'Laurent Defert'
-release = '1.1'
+release = '1.2'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 sys.path.append(os.path.abspath('_extensions'))
 extensions = ['code_blocks', 'myst_parser']
 test_code_output = 'code_blocks.json'
```

### Comparing `sosse-1.1.1/doc/source/crawl/add_to_queue.rst` & `sosse-1.2.0/doc/source/crawl/add_to_queue.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/source/crawl/crawl_depth.rst` & `sosse-1.2.0/doc/source/crawl/crawl_depth.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/source/crawl/policies.rst` & `sosse-1.2.0/doc/source/crawl/policies.rst`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,19 @@
 Screenshot format
 """""""""""""""""
 
 Format of the image JPG or PNG.
 
 .. _script_params:
 
+Remove navigation related elements
+""""""""""""""""""""""""""""""""""
+
+This option removes HTML elements `<nav>`, `<header>` and `<footer>` before processing the page.
+
 Script
 """"""
 
 Javascript code to be executed in the context of the web pages when they have finished loading. This can be used to handle authentication, validate forms, remove headers, ...
 
 For example, the following script could be used to click on a `GDPR <https://en.wikipedia.org/wiki/General_Data_Protection_Regulation>`_ compliance ``I agree`` button:
```

### Comparing `sosse-1.1.1/doc/source/documents.rst` & `sosse-1.2.0/doc/source/documents.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/source/domain_settings.rst` & `sosse-1.2.0/doc/source/domain_settings.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/source/index.rst` & `sosse-1.2.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/source/install/database.rst.template` & `sosse-1.2.0/doc/source/install/database.rst.template`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/source/install/debian.rst` & `sosse-1.2.0/doc/source/install/debian.rst`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
    apt update
    apt install -y sosse
 
 Database setup
 --------------
 
-.. include:: database_debian.rst
+.. include:: database_debian_generated.rst
 
 Daemons setup
 -------------
 
 And then enable the daemons and start them:
 
 .. code-block:: shell
```

### Comparing `sosse-1.1.1/doc/source/install/docker.rst` & `sosse-1.2.0/doc/source/install/docker.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/source/install/pip.rst` & `sosse-1.2.0/doc/source/install/pip.rst`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 .. code-block:: shell
 
    /opt/sosse-venv/bin/sosse-admin collectstatic --noinput --clear
 
 Database setup
 --------------
 
-.. include:: database_pip.rst
+.. include:: database_pip_generated.rst
 
 WSGI server
 -----------
 
 You can install a WSGI server of your choice. If you wish to install `uWSGI <https://uwsgi-docs.readthedocs.io/en/latest/>`_, you can do:
 
 .. code-block:: shell
```

### Comparing `sosse-1.1.1/doc/source/permissions.rst` & `sosse-1.2.0/doc/source/permissions.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/source/screenshots.rst` & `sosse-1.2.0/doc/source/screenshots.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/source/search_engines.rst` & `sosse-1.2.0/doc/source/search_engines.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/source/user/cached.rst` & `sosse-1.2.0/doc/source/user/cached.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/source/user/history.rst` & `sosse-1.2.0/doc/source/user/history.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/source/user/preferences.rst` & `sosse-1.2.0/doc/source/user/preferences.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/source/user/search.rst` & `sosse-1.2.0/doc/source/user/search.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/doc/source/user/shortcuts.rst` & `sosse-1.2.0/doc/source/user/shortcuts.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/docker/Makefile` & `sosse-1.2.0/docker/Makefile`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/docker/debian/Dockerfile` & `sosse-1.2.0/docker/debian/Dockerfile`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/docker/debian-pkg/Dockerfile` & `sosse-1.2.0/docker/debian-pkg/Dockerfile`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/docker/debian-test/Dockerfile` & `sosse-1.2.0/docker/debian-test/Dockerfile`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/docker/pip-release/Dockerfile` & `sosse-1.2.0/docker/pip-release/Dockerfile`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/docker/pip-test/Dockerfile` & `sosse-1.2.0/docker/pip-test/Dockerfile`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/pyproject.toml` & `sosse-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/admin.py` & `sosse-1.2.0/se/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -454,15 +454,15 @@
     search_fields = ('url_regex',)
     readonly_fields = ('documents',)
     fieldsets = (
         (None, {
             'fields': ('url_regex', 'documents', 'condition', 'crawl_depth', 'mimetype_regex', 'keep_params', 'store_extern_links')
         }),
         ('Browser', {
-            'fields': ('default_browse_mode', 'take_screenshots', 'screenshot_format', 'script')
+            'fields': ('default_browse_mode', 'take_screenshots', 'screenshot_format', 'remove_nav_elements', 'script')
         }),
         ('Updates', {
             'fields': ('recrawl_mode', 'recrawl_dt_min', 'recrawl_dt_max', 'hash_mode')
         }),
         ('Authentication', {
             'fields': ('auth_login_url_re', 'auth_form_selector'),
         }),
```

### Comparing `sosse-1.1.1/se/apps.py` & `sosse-1.2.0/se/apps.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/atom.py` & `sosse-1.2.0/se/atom.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/browser.py` & `sosse-1.2.0/se/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -428,24 +428,39 @@
 
         if redirect_count > settings.SOSSE_MAX_REDIRECTS:
             raise SkipIndexing(f'max redirects ({settings.SOSSE_MAX_REDIRECTS}) reached')
 
         return redirect_count
 
     @classmethod
+    def remove_nav_elements(cls):
+        cls.driver.execute_script('''
+        const tags = ['nav', 'header', 'footer'];
+        tags.map((tag) => {
+            const elems = document.getElementsByTagName(tag);
+            for (no = 0; no < elems.length; no++) {
+                elems[no].remove();
+            }
+        });
+        ''')
+
+    @classmethod
     def _get_page(cls, url):
         from .models import CrawlPolicy
         redirect_count = cls._wait_for_ready(url)
 
         current_url = cls._current_url()
         crawl_policy = CrawlPolicy.get_from_url(current_url)
         if crawl_policy and crawl_policy.script:
             cls.driver.execute_script(crawl_policy.script)
             cls._wait_for_ready(url)
 
+        if crawl_policy and crawl_policy.remove_nav_elements == CrawlPolicy.REMOVE_NAV_YES:
+            cls.remove_nav_elements()
+
         content = cls.driver.page_source
         page = Page(current_url,
                     content,
                     cls)
         page.title = cls.driver.title
         page.redirect_count = redirect_count
         return page
```

### Comparing `sosse-1.1.1/se/cached.py` & `sosse-1.2.0/se/cached.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/forms.py` & `sosse-1.2.0/se/forms.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/login.py` & `sosse-1.2.0/se/login.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/management/commands/crawl.py` & `sosse-1.2.0/se/management/commands/crawl.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/management/commands/default_admin.py` & `sosse-1.2.0/se/management/commands/default_admin.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/management/commands/default_conf.py` & `sosse-1.2.0/se/management/commands/default_conf.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/management/commands/extract_doc.py` & `sosse-1.2.0/se/management/commands/extract_doc.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/management/commands/generate_secret.py` & `sosse-1.2.0/se/management/commands/generate_secret.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/management/commands/load_se.py` & `sosse-1.2.0/se/management/commands/load_se.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/management/commands/update_se.py` & `sosse-1.2.0/se/management/commands/update_se.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/migrations/0001_initial.py` & `sosse-1.2.0/se/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/migrations/0002_search_vector.py` & `sosse-1.2.0/se/migrations/0002_search_vector.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/migrations/0003_sosse_1_1_0.py` & `sosse-1.2.0/se/migrations/0003_sosse_1_1_0.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/models.py` & `sosse-1.2.0/se/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,14 +296,17 @@
     def _dom_walk(self, elem, crawl_policy, links, base_url):
         if isinstance(elem, Doctype):
             return
 
         if elem.name in ('[document]', 'title', 'script', 'style'):
             return
 
+        if crawl_policy.remove_nav_elements == CrawlPolicy.REMOVE_NAV_YES and elem.name in ('nav', 'header', 'footer'):
+            return
+
         s = self._get_elem_text(elem)
 
         # Keep the link if it has text, or if we take screenshots
         if elem.name in (None, 'a') and (s or crawl_policy.take_screenshots):
             if links['text'] and links['text'][-1] not in (' ', '\n'):
                 links['text'] += ' '
 
@@ -1357,14 +1360,22 @@
     mimetype_regex = models.TextField(default='text/.*')
     crawl_depth = models.PositiveIntegerField(default=0, help_text='Level of external links (links that don\'t match the regex) to recurse into')
     keep_params = models.BooleanField(default=True, verbose_name='Index URL parameters', help_text='When disabled, URL parameters (parameters after "?") are removed from URLs, this can be useful if some parameters are random, change sorting or filtering, ...')
 
     default_browse_mode = models.CharField(max_length=8, choices=DomainSetting.BROWSE_MODE, default=DomainSetting.BROWSE_SELENIUM, help_text='Python Request is faster, but can\'t execute Javascript and may break pages')
     take_screenshots = models.BooleanField(default=True)
     screenshot_format = models.CharField(max_length=3, choices=Document.SCREENSHOT_FORMAT, default=Document.SCREENSHOT_JPG)
+
+    REMOVE_NAV_YES = 'yes'
+    REMOVE_NAV_NO = 'no'
+    REMOVE_NAV = [
+        (REMOVE_NAV_YES, 'Yes'),
+        (REMOVE_NAV_NO, 'No')
+    ]
+    remove_nav_elements = models.CharField(default=REMOVE_NAV_YES, help_text='Remove navigation related elements', choices=REMOVE_NAV, max_length=4)
     script = models.TextField(default='', help_text='Javascript code to execute after the page is loaded', blank=True)
     store_extern_links = models.BooleanField(default=False, help_text='Store links to non-indexed pages')
 
     recrawl_mode = models.CharField(max_length=8, choices=RECRAWL_MODE, default=RECRAWL_ADAPTIVE, verbose_name='Crawl frequency', help_text='Adaptive frequency will increase delay between two crawls when the page stays unchanged')
     recrawl_dt_min = models.DurationField(blank=True, null=True, help_text='Min. time before recrawling a page', default=timedelta(days=1))
     recrawl_dt_max = models.DurationField(blank=True, null=True, help_text='Max. time before recrawling a page', default=timedelta(days=365))
     hash_mode = models.CharField(max_length=10, choices=HASH_MODE, default=HASH_NO_NUMBERS, help_text='Page content hashing method used to detect changes in the content')
```

### Comparing `sosse-1.1.1/se/screenshot.py` & `sosse-1.2.0/se/screenshot.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/search.py` & `sosse-1.2.0/se/search.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/static/se/admin-base.css` & `sosse-1.2.0/se/static/se/admin-base.css`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/static/se/admin-forms.css` & `sosse-1.2.0/se/static/se/admin-forms.css`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/static/se/base.js` & `sosse-1.2.0/se/static/se/base.js`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/static/se/icon-atom.svg` & `sosse-1.2.0/se/static/se/icon-atom.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/static/se/icon-clear.svg` & `sosse-1.2.0/se/static/se/icon-clear.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/static/se/icon-cog.svg` & `sosse-1.2.0/se/static/se/icon-cog.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/static/se/icon-search.svg` & `sosse-1.2.0/se/static/se/icon-search.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/static/se/icon-stats.svg` & `sosse-1.2.0/se/static/se/icon-stats.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/static/se/icon-trash.svg` & `sosse-1.2.0/se/static/se/icon-trash.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/static/se/icon-user.svg` & `sosse-1.2.0/se/static/se/icon-user.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/static/se/index.js` & `sosse-1.2.0/se/static/se/index.js`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/static/se/logo.png` & `sosse-1.2.0/se/static/se/logo.png`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/static/se/logo.svg` & `sosse-1.2.0/se/static/se/logo.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/static/se/pygal-tooltips.min.js` & `sosse-1.2.0/se/static/se/pygal-tooltips.min.js`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/static/se/screenshot.js` & `sosse-1.2.0/se/static/se/screenshot.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 let images, links;
 
 function resize() {
     // width with implicit margin
-    const w_width = document.body.getBoundingClientRect().width + 8;
+    const w_width = document.body.getBoundingClientRect().width;
     const ratio = w_width / screen_width;
 
     for (let i = 0; i < images.length; i++) {
         const img = images[i];
         img.style.width = `${screen_width * ratio}px`;
     }
 
@@ -25,8 +25,11 @@
     images = document.querySelectorAll('#screenshots > img');
 
     window.addEventListener('resize', function() {
         resize();
     });
 
     resize();
+
+    // Work-around in case the initial resize() was done while no image was loaded yet
+    setTimeout(resize, 300);
 });
```

### Comparing `sosse-1.1.1/se/static/se/style.css` & `sosse-1.2.0/se/static/se/style.css`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/stats.py` & `sosse-1.2.0/se/stats.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/templates/admin/add_to_queue.html` & `sosse-1.2.0/se/templates/admin/add_to_queue.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/templates/admin/app_list.html` & `sosse-1.2.0/se/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/templates/admin/base.html` & `sosse-1.2.0/se/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/templates/admin/change_form.html` & `sosse-1.2.0/se/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/templates/admin/crawl_status.html` & `sosse-1.2.0/se/templates/admin/crawl_status.html`

 * *Files 20% similar despite different names*

```diff
@@ -15,15 +15,23 @@
 {% endblock %}
 
 {% block css %}
 #result_list th:nth-child(1), #result_list td:nth-child(1) {
   white-space: nowrap;
   overflow: hidden;
   max-width: 0;
-  width: 70%;
+  width: 35%;
+  text-overflow: ellipsis;
+}
+
+#result_list th:nth-child(2), #result_list td:nth-child(2) {
+  white-space: nowrap;
+  overflow: hidden;
+  max-width: 0;
+  width: 35%;
   text-overflow: ellipsis;
 }
 
 #result_list tr.running {
   background-color: #d9fabe;
 }
```

### Comparing `sosse-1.1.1/se/templates/admin/crawl_status_content.html` & `sosse-1.2.0/se/templates/admin/crawl_status_content.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+{% load static %}
 <h4>Crawlers</h4>
 {% if crawlers %}
   <div class="results">
     <table id="result_list">
       <thead>
         <th><div class="text">No</div></th>
         <th><div class="text">PID</div></th>
@@ -56,25 +57,39 @@
   Documents crawled
 </h4>
 {% if queue %}
   <div class="results">
     <table id="result_list" style="width: 100%">
       <thead>
         <th><div class="text">Url</div></th>
+        <th><div class="text">Title</div></th>
+        <th><div class="text">Status</div></th>
         <th><div class="text">Crawl next</div></th>
         <th><div class="text">Crawled last</div></th>
       </thead>
       <tbody>
         {% for doc in queue %}
           <tr {% if doc.pending %}class="{% if doc.worker_no is not None %}running{% elif doc.crawl_last is None or doc.crawl_next < now %}pending{% endif %}"{% endif %}>
             <td>
               <a href="{% url 'admin:se_document_change' doc.id %}">
                 {{ doc.url }}
               </a>
             </td>
+            <td>
+              <a href="{% url 'admin:se_document_change' doc.id %}">
+                {{ doc.title }}
+              </a>
+            </td>
+            <td>
+                {% if doc.error %}
+                    <img src="{% static "admin/img/icon-no.svg" %}" alt="False">
+                {% else %}
+                    <img src="{% static "admin/img/icon-yes.svg" %}" alt="True">
+                {% endif %}
+            </td>
             {% if doc.worker_no is not None %}
                <td>In progress</td>
             {% elif doc.crawl_last is None or doc.crawl_next < now %}
                <td>Pending</td>
             {% elif doc.crawl_next and doc.pending %}
               <td title="{{ doc.crawl_next }}">{{ doc.crawl_next_human }}</td>
             {% else %}
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
+{% load static %}
 *** Crawlers ***
 {% if crawlers %}
 {{ crawler.worker_no }} {{ crawler.pid }} {{ crawler.state }}
 
 {% if 'se.change_crawlerstats' in perms %}
 {% csrf_token %} {% if pause %} [Pause] {% else %} [Resume] {% endif %}
 {% endif %}
```

### Comparing `sosse-1.1.1/se/templates/se/about.html` & `sosse-1.2.0/se/templates/se/about.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/templates/se/base.html` & `sosse-1.2.0/se/templates/se/base.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/templates/se/cached.html` & `sosse-1.2.0/se/templates/se/cached.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/templates/se/history.html` & `sosse-1.2.0/se/templates/se/history.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/templates/se/home_browse.html` & `sosse-1.2.0/se/templates/se/home_browse.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/templates/se/index.html` & `sosse-1.2.0/se/templates/se/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         float: right;
         width: 160px;
         height: 100px;
     }
 
     #home-grid {
         display: grid;
-        grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
+        grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
         grid-auto-rows: minmax(100px, auto);
     }
 
     #home-grid a {
         text-decoration: none;
     }
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 10px 10px 10px; border-radius: 10px; } .res:hover { background-color: #f4f4f4;
 } .res-img { height: 16px; width: 16px; display: inline; } .res-title { margin-
 bottom: 0px; display: inline; } .res-url { text-decoration: none; color: #080;
 font-size: 13px; } .res-rank { font-size: 10px; display: inline; } .res-
 headline { text-decoration: none; color: #000; } .res-highlight { background-
 color: #c6dcff; } .res-preview { float: right; width: 160px; height: 100px; }
 #home-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax
-(200px, 1fr)); grid-auto-rows: minmax(100px, auto); } #home-grid a { text-
+(220px, 1fr)); grid-auto-rows: minmax(100px, auto); } #home-grid a { text-
 decoration: none; } .res-home { display: block; position: relative; grid-
 column: auto; grid-row: auto; width: 200px; height: 200px; text-align: center;
 overflow: hidden; } .res-home-icon { padding-top: 30%; width: 100%; } .res-
 home-icon > img { width: 64px; height: 64px; } .res-home-fade-text { position:
 absolute; bottom: 0; left: 0; margin: 0; width: 100%; height: 24px; } .res
 .res-home-fade-text { background-image: linear-gradient(to bottom, transparent,
 white); } .res:hover .res-home-fade-text { background-image: linear-gradient(to
```

### Comparing `sosse-1.1.1/se/templates/se/main_menu.html` & `sosse-1.2.0/se/templates/se/main_menu.html`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         {% if user.is_active %}
             <a href="{% url 'history' %}" class="links menu_links">History</a>
             <a href="{% url 'admin:password_change' %}" class="links menu_links">Change pass</a>
             <a href="{% url 'logout' %}" class="links menu_links">Log out</a>
         {% else %}
             <a href="{% url 'login' %}" class="links menu_links">Log in</a>
         {% endif %}
+        <a href="https://sosse.readthedocs.io/en/stable/" class="links menu_links">Documentation</a>
         <a href="{% url 'about' %}" class="links menu_links">About</a>
     </div>
 </div>
 {% if user.is_active and user.is_staff %}
     <div id="conf_menu" class="menu">
         <button class="menu_button img_button" id="conf_menu_button" title="Configuration"></button>
         <div id="conf_menu_panel" class="panel">
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% load static %}
 {% if user.has_usable_password %}
 {% firstof user.get_short_name user.get_username %}
 {% endif %}
 Preferences {% if user.is_active %} History Change_pass Log_out {% else %} Log
-in {% endif %} About
+in {% endif %} Documentation About
 {% if user.is_active and user.is_staff %}
 Statistics Administration
 {% endif %}
```

### Comparing `sosse-1.1.1/se/templates/se/opensearch.xml` & `sosse-1.2.0/se/templates/se/opensearch.xml`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/templates/se/pagination.html` & `sosse-1.2.0/se/templates/se/pagination.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/templates/se/prefs.html` & `sosse-1.2.0/se/templates/se/prefs.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/templates/se/screenshot.html` & `sosse-1.2.0/se/templates/se/screenshot.html`

 * *Files 9% similar despite different names*

```diff
@@ -19,18 +19,18 @@
         border: 1px;
         border-style: solid;
         border-color: #aaa;
         background-color: #fdd;
     }
     #screenshots {
         position: absolute;
-        margin-left: -48px;
+        margin-left: -40px;
     }
     #screenshots > img {
-        margin-top: -4px;
+        margin-top: -5px;
     }
     .img_link {
         position: absolute;
         margin-top: -4px;
     }
     .img_link:hover {
         position: absolute;
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 {% extends "se/base.html" %} {% load static %} {% block head %}
 creenshot.js" %}">
 {% for screen in screens %}
  {% endfor %} {% endblock %} {% block js %} const screen_width = {
 { screenshot_size.0 }}; const screen_height = {{ screenshot_size.1 }}; {%
 endblock %} {% block css %} #error_pre { overflow: scroll; border: 1px; border-
 style: solid; border-color: #aaa; background-color: #fdd; } #screenshots
-{ position: absolute; margin-left: -48px; } #screenshots > img { margin-top: -
-4px; } .img_link { position: absolute; margin-top: -4px; } .img_link:hover
+{ position: absolute; margin-left: -40px; } #screenshots > img { margin-top: -
+5px; } .img_link { position: absolute; margin-top: -4px; } .img_link:hover
 { position: absolute; box-shadow: 0px 0px 4px 4px #91baff; margin: -4px 0px 0px
 -2px; padding: 0px 8px 4px 0px; } {% endblock %} {% block body %} {% include
 "se/cached.html" %}
 {% for link in links %}
 % if link.doc_to %}href="{{ link.doc_to.get_absolute_url }}" title="{
 { link.doc_to.title }}"{% else %}href="{{ link.extern_url }}" title="{
 { link.extern_url }}"{% endif %}>
```

### Comparing `sosse-1.1.1/se/templates/se/search_redirect.html` & `sosse-1.2.0/se/templates/se/search_redirect.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/templates/se/stats.html` & `sosse-1.2.0/se/templates/se/stats.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/templates/se/unknown_url.html` & `sosse-1.2.0/se/templates/se/unknown_url.html`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/test_cookie.py` & `sosse-1.2.0/se/test_cookie.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/test_crawl.py` & `sosse-1.2.0/se/test_crawl.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/test_functionals.py` & `sosse-1.2.0/se/test_functionals.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/test_misc.py` & `sosse-1.2.0/se/test_misc.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/test_parser.py` & `sosse-1.2.0/se/test_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # across classes and external libraries
 
 import base64
 
 from django.test import TestCase
 
 from se.browser import Browser, SeleniumBrowser, Page
-from se.models import CrawlPolicy
+from se.models import CrawlPolicy, Document
 
 
 LINKS = ({
     'descr': 'regular link',
     'link': 'http://test.com/',
 }, {
     'descr': 'percent-encoded utf8 link',
@@ -116,15 +116,15 @@
 ''' % '\n'.join(['<a href="%s">%s</a>' % (link['link'], link['descr']) for link in LINKS])
 
 
 class PageTest(TestCase):
     @classmethod
     def setUpClass(cls):
         Browser.init()
-        CrawlPolicy.create_default()
+        cls.policy = CrawlPolicy.create_default()
 
     @classmethod
     def tearDownClass(cls):
         Browser.destroy()
 
     def test_10_beautifulsoup(self):
         page = Page('', FAKE_PAGE, None)
@@ -140,7 +140,22 @@
         page = SeleniumBrowser.get(url)
         links = list(page.get_links(True))
 
         self.assertEqual(len(links), len(LINKS))
         for no, link in enumerate(links):
             expected = LINKS[no].get('expected_output', LINKS[no]['link'])
             self.assertEqual(link, expected, '%s failed' % LINKS[no]['descr'])
+
+    NAV_HTML = '<html><body><header>header</header><nav>nav</nav>text<footer>footer</footer></body></html>'
+
+    def test_30_no_nav_element(self):
+        page = Page('http://test/', self.NAV_HTML, None)
+        doc = Document()
+        doc.index(page, self.policy)
+        self.assertEqual(doc.content, 'text')
+
+    def test_40_nav_element(self):
+        page = Page('http://test/', self.NAV_HTML, None)
+        doc = Document()
+        self.policy.remove_nav_elements = CrawlPolicy.REMOVE_NAV_NO
+        doc.index(page, self.policy)
+        self.assertEqual(doc.content, 'header nav text footer')
```

### Comparing `sosse-1.1.1/se/test_redirect.py` & `sosse-1.2.0/se/test_redirect.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/test_requests.py` & `sosse-1.2.0/se/test_requests.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/test_search.py` & `sosse-1.2.0/se/test_search.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/test_url.py` & `sosse-1.2.0/se/test_url.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/test_views.py` & `sosse-1.2.0/se/test_views.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/utils.py` & `sosse-1.2.0/se/utils.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/views.py` & `sosse-1.2.0/se/views.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/words.py` & `sosse-1.2.0/se/words.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/se/www.py` & `sosse-1.2.0/se/www.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/sosse/conf.py` & `sosse-1.2.0/sosse/conf.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/sosse/search_engines.json` & `sosse-1.2.0/sosse/search_engines.json`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/sosse/settings.py` & `sosse-1.2.0/sosse/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,9 +325,9 @@
         'name': 'chinese',
         'flag': '🇹🇼'
     }
 }
 
 globals().update(Conf.get())
 
-SOSSE_VERSION_TAG = '1.1.1'
-SOSSE_VERSION_COMMIT = '828424d6'
+SOSSE_VERSION_TAG = '1.2.0'
+SOSSE_VERSION_COMMIT = '578e5b76'
```

### Comparing `sosse-1.1.1/sosse/sosse_admin.py` & `sosse-1.2.0/sosse/sosse_admin.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/sosse/urls.py` & `sosse-1.2.0/sosse/urls.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/sosse/wsgi.py` & `sosse-1.2.0/sosse/wsgi.py`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/sosse.egg-info/PKG-INFO` & `sosse-1.2.0/sosse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosse
-Version: 1.1.1
+Version: 1.2.0
 Summary: Selenium Open Source Search Engine
 Author-email: Laurent Defert <laurent_defert@yahoo.fr>
 License: GNU Affero General Public License v3
 Keywords: search engine,crawler
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sosse Version: 1.1.1 Summary: Selenium Open Source
+Metadata-Version: 2.1 Name: sosse Version: 1.2.0 Summary: Selenium Open Source
 Search Engine Author-email: Laurent Defert
 yahoo.fr> License: GNU Affero General Public License v3 Keywords: search
 engine,crawler Classifier: Framework :: Django Classifier: Programming Language
 :: Python :: 3 Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE
 [https://raw.githubusercontent.com/biolds/sosse/main/se/static/se/logo.svg]
 [https://img.shields.io/gitlab/pipeline-coverage/biolds1/
```

### Comparing `sosse-1.1.1/sosse.egg-info/SOURCES.txt` & `sosse-1.2.0/sosse.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,15 @@
 se/management/commands/extract_doc.py
 se/management/commands/generate_secret.py
 se/management/commands/load_se.py
 se/management/commands/update_se.py
 se/migrations/0001_initial.py
 se/migrations/0002_search_vector.py
 se/migrations/0003_sosse_1_1_0.py
+se/migrations/0004_sosse_1_2_0.py
 se/migrations/__init__.py
 se/static/se/admin-base.css
 se/static/se/admin-forms.css
 se/static/se/base.js
 se/static/se/icon-atom.svg
 se/static/se/icon-clear.svg
 se/static/se/icon-cog.svg
```

### Comparing `sosse-1.1.1/tests/cookies.json` & `sosse-1.2.0/tests/cookies.json`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/tests/doc_test.sh` & `sosse-1.2.0/tests/doc_test.sh`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/tests/document-ja.json` & `sosse-1.2.0/tests/document-ja.json`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/tests/release.md` & `sosse-1.2.0/tests/release.md`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/tests/robotframework/home_docs.json` & `sosse-1.2.0/tests/robotframework/home_docs.json`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/tests/robotframework/home_favicon.json` & `sosse-1.2.0/tests/robotframework/home_favicon.json`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/tests/robotframework/start.sh` & `sosse-1.2.0/tests/robotframework/start.sh`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/tests/robotframework/tests/01_crawl.robot` & `sosse-1.2.0/tests/robotframework/tests/01_crawl.robot`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/tests/robotframework/tests/02_user.robot` & `sosse-1.2.0/tests/robotframework/tests/02_user.robot`

 * *Files identical despite different names*

### Comparing `sosse-1.1.1/tests/robotframework/tests/common.robot` & `sosse-1.2.0/tests/robotframework/tests/common.robot`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 |  | Open Browser | http://127.0.0.1/ | browser=Firefox |  options=add_argument("--headless")
 #|  | Open Browser | http://127.0.0.1/ | browser=Chrome | options=add_argument("--no-sandbox");options=add_argument("--disable-dev-shm-usage");add_argument("--headless");add_argument('--enable-precise-memory-info');add_argument('--disable-default-apps')
 |  | Set Window Size | 1024 | 768
 |  | Set Screenshot Directory | screenshots/
 |  | Input Text | id=id_username | admin
 |  | Input Text | id=id_password | admin
 |  | Click Element | xpath=//form[@id='login-form']//input[@type='submit']
+|  | Wait Until Element Is Visible | id=menu_username
 
 
 | Hilight | [Arguments] | @{kwargs}
 |  | Wait Until element Is Visible | @{kwargs}
 |  | ${elem}= | Get WebElement | @{kwargs}
 |  | Execute Javascript | arguments[0].style = 'box-shadow: 0px 0px 4px 4px #91ffba; margin: -4px 0px 0px -2px; padding: 4px 8px 0px 8px;' | ARGUMENTS | ${elem}
```

### Comparing `sosse-1.1.1/tests/test_app.sh` & `sosse-1.2.0/tests/test_app.sh`

 * *Files identical despite different names*

