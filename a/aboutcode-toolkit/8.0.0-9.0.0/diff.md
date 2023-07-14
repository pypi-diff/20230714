# Comparing `tmp/aboutcode-toolkit-8.0.0.tar.gz` & `tmp/aboutcode-toolkit-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aboutcode-toolkit-8.0.0.tar", last modified: Thu Mar  9 10:10:39 2023, max compression
+gzip compressed data, was "aboutcode-toolkit-9.0.0.tar", last modified: Fri Jul 14 10:34:44 2023, max compression
```

## Comparing `aboutcode-toolkit-8.0.0.tar` & `aboutcode-toolkit-9.0.0.tar`

### file list

```diff
@@ -1,541 +1,542 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:39.018629 aboutcode-toolkit-8.0.0/
--rw-rw-rw-   0        0        0       89 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/.gitattributes
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.011814 aboutcode-toolkit-8.0.0/.github/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.246917 aboutcode-toolkit-8.0.0/.github/workflows/
--rw-rw-rw-   0        0        0      855 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/.github/workflows/docs-ci.yml
--rw-rw-rw-   0        0        0     2023 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/.github/workflows/pypi-release.yml
--rw-rw-rw-   0        0        0      771 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/.gitignore
--rw-rw-rw-   0        0        0      392 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/.readthedocs.yml
--rw-rw-rw-   0        0        0       88 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/AUTHORS.rst
--rw-rw-rw-   0        0        0    10700 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/CHANGELOG.rst
--rw-rw-rw-   0        0        0     3422 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/CODE_OF_CONDUCT.rst
--rw-rw-rw-   0        0        0     1153 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/Dockerfile
--rw-rw-rw-   0        0        0      218 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1596 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/Makefile
--rw-rw-rw-   0        0        0      752 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/NOTICE
--rw-rw-rw-   0        0        0     6853 2023-03-09 10:10:39.018629 aboutcode-toolkit-8.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5309 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/README.rst
--rw-rw-rw-   0        0        0      537 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/about
--rw-rw-rw-   0        0        0      869 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/about.ABOUT
--rwxrwxrwx   0        0        0      879 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/about.bat
--rw-rw-rw-   0        0        0    11558 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/apache-2.0.LICENSE
--rw-rw-rw-   0        0        0      628 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/appveyor.yml
--rw-rw-rw-   0        0        0     2459 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/azure-pipelines.yml
--rw-rw-rw-   0        0        0     6328 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/configure
--rwxrwxrwx   0        0        0     6948 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/configure.bat
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.258444 aboutcode-toolkit-8.0.0/docs/
--rw-rw-rw-   0        0        0      638 2023-03-09 10:09:11.000000 aboutcode-toolkit-8.0.0/docs/Makefile
--rwxrwxrwx   0        0        0      799 2023-03-09 10:09:11.000000 aboutcode-toolkit-8.0.0/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.272491 aboutcode-toolkit-8.0.0/docs/scripts/
--rw-rw-rw-   0        0        0      131 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/docs/scripts/doc8_style_check.sh
--rw-rw-rw-   0        0        0      124 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/docs/scripts/sphinx_build_link_check.sh
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.324457 aboutcode-toolkit-8.0.0/docs/source/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.333455 aboutcode-toolkit-8.0.0/docs/source/_static/
--rw-rw-rw-   0        0        0    10299 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/docs/source/_static/theme_overrides.css
--rw-rw-rw-   0        0        0     2175 2023-03-09 10:09:11.000000 aboutcode-toolkit-8.0.0/docs/source/conf.py
--rw-rw-rw-   0        0        0    21485 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/docs/source/general.rst
--rw-rw-rw-   0        0        0     5296 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/docs/source/home.rst
--rw-rw-rw-   0        0        0      346 2023-03-09 10:09:11.000000 aboutcode-toolkit-8.0.0/docs/source/index.rst
--rw-rw-rw-   0        0        0    28753 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/docs/source/reference.rst
--rw-rw-rw-   0        0        0    16422 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/docs/source/specification.rst
--rw-rw-rw-   0        0        0     1250 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/docs/source/type_of_errors.rst
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.016814 aboutcode-toolkit-8.0.0/etc/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.400787 aboutcode-toolkit-8.0.0/etc/ci/
--rw-rw-rw-   0        0        0     1700 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/ci/azure-container-deb.yml
--rw-rw-rw-   0        0        0     1753 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/ci/azure-container-rpm.yml
--rw-rw-rw-   0        0        0     1240 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/ci/azure-posix.yml
--rw-rw-rw-   0        0        0     1215 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/ci/azure-win.yml
--rw-rw-rw-   0        0        0      257 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/ci/install_sudo.sh
--rw-rw-rw-   0        0        0     8365 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/ci/macports-ci
--rw-rw-rw-   0        0        0      684 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/ci/macports-ci.ABOUT
--rw-rw-rw-   0        0        0     1022 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/ci/mit.LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.525992 aboutcode-toolkit-8.0.0/etc/scripts/
--rw-rw-rw-   0        0        0     3744 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/README.rst
--rw-rw-rw-   0        0        0     1301 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/check_thirdparty.py
--rw-rw-rw-   0        0        0     9486 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/fetch_thirdparty.py
--rw-rw-rw-   0        0        0     9699 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/gen_pypi_simple.py
--rw-rw-rw-   0        0        0      354 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/gen_pypi_simple.py.ABOUT
--rw-rw-rw-   0        0        0     2776 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/gen_pypi_simple.py.NOTICE
--rw-rw-rw-   0        0        0     1715 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/gen_requirements.py
--rw-rw-rw-   0        0        0     2266 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/gen_requirements_dev.py
--rw-rw-rw-   0        0        0      101 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/requirements.txt
--rw-rw-rw-   0        0        0     4497 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/test_utils_pip_compatibility_tags.py
--rw-rw-rw-   0        0        0      504 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
--rw-rw-rw-   0        0        0     2839 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/test_utils_pypi_supported_tags.py
--rw-rw-rw-   0        0        0      773 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
--rw-rw-rw-   0        0        0     6418 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/utils_dejacode.py
--rw-rw-rw-   0        0        0     6704 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/utils_pip_compatibility_tags.py
--rw-rw-rw-   0        0        0      494 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
--rw-rw-rw-   0        0        0     2850 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/utils_pypi_supported_tags.py
--rw-rw-rw-   0        0        0      741 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT
--rw-rw-rw-   0        0        0     6152 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/utils_requirements.py
--rw-rw-rw-   0        0        0    75931 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/utils_thirdparty.py
--rw-rw-rw-   0        0        0      608 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/etc/scripts/utils_thirdparty.py.ABOUT
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.018813 aboutcode-toolkit-8.0.0/example/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.030810 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.019812 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.540995 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/
--rw-rw-rw-   0        0        0      365 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/alocal.m4.ABOUT
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.559003 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/config/
--rw-rw-rw-   0        0        0      556 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/config/config.guess.ABOUT
--rw-rw-rw-   0        0        0      475 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/config/config.rpath.ABOUT
--rw-rw-rw-   0        0        0      552 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/config/config.sub.ABOUT
--rw-rw-rw-   0        0        0      952 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/config/gpl-2.0-autoconf.LICENSE
--rw-rw-rw-   0        0        0      425 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/config/mkinstalldirs.ABOUT
--rw-rw-rw-   0        0        0       62 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/config/public-domain.LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.563530 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/contrib/
--rw-rw-rw-   0        0        0      320 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/contrib/UlrichWindl.LICENSE
--rw-rw-rw-   0        0        0      284 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/contrib/dconf.ABOUT
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.596528 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/
--rw-rw-rw-   0        0        0      709 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/KazKylheku.LICENSE
--rw-rw-rw-   0        0        0      458 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/argv_parse.c.ABOUT
--rw-rw-rw-   0        0        0      458 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/argv_parse.h.ABOUT
--rw-rw-rw-   0        0        0      243 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/dict.c.ABOUT
--rw-rw-rw-   0        0        0      243 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/dict.h.ABOUT
--rw-rw-rw-   0        0        0    18409 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/gpl-2.0.LICENSE
--rw-rw-rw-   0        0        0      497 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/journal.c.ABOUT
--rw-rw-rw-   0        0        0    25751 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/lgpl-2.0.LICENSE
--rw-rw-rw-   0        0        0       48 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/mit-old-style-legal-2.LICENSE
--rw-rw-rw-   0        0        0      546 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/mtrace.c.ABOUT
--rw-rw-rw-   0        0        0      486 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/mtrace.h.ABOUT
--rw-rw-rw-   0        0        0      492 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/profile.c.ABOUT
--rw-rw-rw-   0        0        0      492 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/profile.h.ABOUT
--rw-rw-rw-   0        0        0      500 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsprogs-1.39.ABOUT
--rw-rw-rw-   0        0        0     1438 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsprogs-1.39.NOTICE
--rw-rw-rw-   0        0        0    18409 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/gpl-2.0.LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.023812 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/include/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.600527 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/include/nonunix/
--rw-rw-rw-   0        0        0      560 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/include/nonunix/getopt.h.ABOUT
--rw-rw-rw-   0        0        0    25751 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/include/nonunix/lgpl-2.0.LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.605526 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/install-utils/
--rw-rw-rw-   0        0        0      430 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/install-utils/convfstab.ABOUT
--rw-rw-rw-   0        0        0       62 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/install-utils/public-domain.LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.610530 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/intl/
--rw-rw-rw-   0        0        0      390 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/intl/intl.ABOUT
--rw-rw-rw-   0        0        0    25751 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/intl/lgpl-2.0.LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.615523 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.620531 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/blkid/
--rw-rw-rw-   0        0        0      437 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/blkid/blkid.ABOUT
--rw-rw-rw-   0        0        0    26742 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/blkid/lgpl-2.1.LICENSE
--rw-rw-rw-   0        0        0      824 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/bsla.LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.625526 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/e2p/
--rw-rw-rw-   0        0        0      400 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/e2p/e2p.ABOUT
--rw-rw-rw-   0        0        0    25751 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/e2p/lgpl-2.0.LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.641531 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/
--rw-rw-rw-   0        0        0     1435 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/bsd-new.LICENSE
--rw-rw-rw-   0        0        0      824 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/bsla.LICENSE
--rw-rw-rw-   0        0        0      446 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/com_right.c.ABOUT
--rw-rw-rw-   0        0        0      180 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/et.ABOUT
--rw-rw-rw-   0        0        0    18409 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/gpl-2.0.LICENSE
--rw-rw-rw-   0        0        0     6406 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/kerberos.LICENSE
--rw-rw-rw-   0        0        0      436 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/texinfo.tex.ABOUT
--rw-rw-rw-   0        0        0      417 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/vfprintf.c.ABOUT
--rw-rw-rw-   0        0        0      384 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/fpopen.c.ABOUT
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.645537 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/ss/
--rw-rw-rw-   0        0        0     6406 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/ss/kerberos.LICENSE
--rw-rw-rw-   0        0        0      180 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/ss/ss.ABOUT
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.648536 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/uuid/
--rw-rw-rw-   0        0        0     1435 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/uuid/bsd-new.LICENSE
--rw-rw-rw-   0        0        0      309 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/uuid/uuid.ABOUT
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.652539 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/misc/
--rw-rw-rw-   0        0        0      416 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/misc/blkid.c.ABOUT
--rw-rw-rw-   0        0        0    26742 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/misc/lgpl-2.1.LICENSE
--rw-rw-rw-   0        0        0       62 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/public-domain.LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.660060 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/input/
--rw-rw-rw-   0        0        0     1338 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/input/MAPPING.CONFIG
--rw-rw-rw-   0        0        0     7094 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/input/e2fsprogs-1.39-CreateAboutFile.csv
--rw-rw-rw-   0        0        0    14597 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/input/e2fsprogs-1.39-INV.xlsx
--rw-rw-rw-   0        0        0     3758 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/input/template_sample_attribution_starship.html
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.662058 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/output/
--rw-rw-rw-   0        0        0   118207 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/output/sample_attribution_starship.html
--rw-rw-rw-   0        0        0      867 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      400 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/requirements-dev.txt
--rw-rw-rw-   0        0        0     1602 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/requirements.txt
--rw-rw-rw-   0        0        0     1858 2023-03-09 10:10:39.022629 aboutcode-toolkit-8.0.0/setup.cfg
--rw-rw-rw-   0        0        0       92 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.033813 aboutcode-toolkit-8.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.684061 aboutcode-toolkit-8.0.0/src/aboutcode_toolkit.egg-info/
--rw-rw-rw-   0        0        0     6853 2023-03-09 10:10:36.000000 aboutcode-toolkit-8.0.0/src/aboutcode_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    23831 2023-03-09 10:10:36.000000 aboutcode-toolkit-8.0.0/src/aboutcode_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 10:10:36.000000 aboutcode-toolkit-8.0.0/src/aboutcode_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-03-09 10:10:36.000000 aboutcode-toolkit-8.0.0/src/aboutcode_toolkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-08-23 07:28:54.000000 aboutcode-toolkit-8.0.0/src/aboutcode_toolkit.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      232 2023-03-09 10:10:36.000000 aboutcode-toolkit-8.0.0/src/aboutcode_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-09 10:10:36.000000 aboutcode-toolkit-8.0.0/src/aboutcode_toolkit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.706060 aboutcode-toolkit-8.0.0/src/attributecode/
--rw-rw-rw-   0        0        0     3529 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/src/attributecode/__init__.py
--rw-rw-rw-   0        0        0      921 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/src/attributecode/__main__.py
--rw-rw-rw-   0        0        0     3445 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/src/attributecode/api.py
--rw-rw-rw-   0        0        0    12672 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/src/attributecode/attrib.py
--rw-rw-rw-   0        0        0     4274 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/src/attributecode/attrib_util.py
--rw-rw-rw-   0        0        0    32449 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/src/attributecode/cmd.py
--rw-rw-rw-   0        0        0    16032 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/src/attributecode/gen.py
--rw-rw-rw-   0        0        0     2050 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/src/attributecode/licenses.py
--rw-rw-rw-   0        0        0    71093 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/src/attributecode/model.py
--rw-rw-rw-   0        0        0    14186 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/src/attributecode/transform.py
--rw-rw-rw-   0        0        0    24809 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/src/attributecode/util.py
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.741060 aboutcode-toolkit-8.0.0/templates/
--rw-rw-rw-   0        0        0     3368 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/templates/default_html.template
--rw-rw-rw-   0        0        0      768 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/templates/default_json.template
--rw-rw-rw-   0        0        0     2652 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/templates/license_ref.template
--rw-rw-rw-   0        0        0      165 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/templates/list.csv
--rw-rw-rw-   0        0        0     3001 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/templates/scancode_html.template
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.757074 aboutcode-toolkit-8.0.0/tests/
--rw-rw-rw-   0        0        0     3502 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/test_api.py
--rw-rw-rw-   0        0        0    11418 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/test_attrib.py
--rw-rw-rw-   0        0        0    12179 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/test_cmd.py
--rw-rw-rw-   0        0        0    14845 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/test_gen.py
--rw-rw-rw-   0        0        0    51062 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/test_model.py
--rw-rw-rw-   0        0        0     9989 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/test_transform.py
--rw-rw-rw-   0        0        0    23518 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/test_util.py
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.085333 aboutcode-toolkit-8.0.0/tests/testdata/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.042811 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.773160 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/default_template/
--rw-rw-rw-   0        0        0     1816 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/default_template/expect.html
--rw-rw-rw-   0        0        0      111 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/default_template/simple_sample.csv
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.785158 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/gen_default_template/
--rw-rw-rw-   0        0        0       74 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/gen_default_template/attrib.ABOUT
--rw-rw-rw-   0        0        0      926 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/gen_default_template/expected_default_attrib.html
--rw-rw-rw-   0        0        0       37 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/gen_default_template/httpd-2.4.3.tar.gz
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.789163 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/gen_license_key_name_check/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.793161 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/gen_license_key_name_check/LICENSES/
--rw-rw-rw-   0        0        0       14 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/gen_license_key_name_check/LICENSES/Apache-2.0.txt
--rw-rw-rw-   0        0        0       12 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/gen_license_key_name_check/LICENSES/LGPL-3.0.txt
--rw-rw-rw-   0        0        0      706 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/gen_license_key_name_check/custom.template
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.795158 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/gen_license_key_name_check/expected/
--rw-rw-rw-   0        0        0      537 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/gen_license_key_name_check/expected/expected.html
--rw-rw-rw-   0        0        0      256 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/gen_license_key_name_check/test.ABOUT
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.801164 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/gen_simple/
--rw-rw-rw-   0        0        0       74 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/gen_simple/attrib.ABOUT
--rw-rw-rw-   0        0        0       37 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/gen_simple/httpd-2.4.3.tar.gz
--rw-rw-rw-   0        0        0      169 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/gen_simple/test.template
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.847176 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/scancode_input/
--rw-rw-rw-   0        0        0     4800 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/scancode_input/clean-text-0.3.0-mod-lceupi.json
--rw-rw-rw-   0        0        0     3485 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/scancode_input/expect.html
--rw-rw-rw-   0        0        0     3072 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/scancode_input/scancode.template
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.855188 aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/
--rw-rw-rw-   0        0        0     1026 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/geninventory.csv
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.941703 aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/help/
--rw-rw-rw-   0        0        0     1614 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/help/about_attrib_help.txt
--rw-rw-rw-   0        0        0      595 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/help/about_check_help.txt
--rw-rw-rw-   0        0        0     1305 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/help/about_gen_help.txt
--rw-rw-rw-   0        0        0      676 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/help/about_gen_license_help.txt
--rw-rw-rw-   0        0        0     1117 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/help/about_help.txt
--rw-rw-rw-   0        0        0      575 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/help/about_inventory_help.txt
--rw-rw-rw-   0        0        0     2388 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/help/about_transform_config_help.txt
--rw-rw-rw-   0        0        0      822 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/help/about_transform_help.txt
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.963228 aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/repository-mini/
--rw-rw-rw-   0        0        0      102 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/repository-mini/apache-2.0.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/repository-mini/appdirs-1.4.3-py2.py3-none-any.whl
--rw-rw-rw-   0        0        0      429 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/repository-mini/appdirs.ABOUT
--rw-rw-rw-   0        0        0      137 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/repository-mini/appdirs.LICENSE
--rw-rw-rw-   0        0        0       72 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/repository-mini/mit.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/repository-mini/xtrans-1.3.5.txz
--rw-rw-rw-   0        0        0      374 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/repository-mini/xtrans-1.3.5.txz.ABOUT
--rw-rw-rw-   0        0        0     1280 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/transform.csv
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.993229 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/
--rw-rw-rw-   0        0        0       50 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/about.py.ABOUT
--rw-rw-rw-   0        0        0      102 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/dup_keys.csv
--rw-rw-rw-   0        0        0      102 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/dup_keys_with_diff_case.csv
--rw-rw-rw-   0        0        0      426 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inv.csv
--rw-rw-rw-   0        0        0       53 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inv2.csv
--rw-rw-rw-   0        0        0       63 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inv3.csv
--rw-rw-rw-   0        0        0      164 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inv4.csv
--rw-rw-rw-   0        0        0      426 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inv5.csv
--rw-rw-rw-   0        0        0      422 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inv6.csv
--rw-rw-rw-   0        0        0       62 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inv_no_about_resource.csv
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.048817 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.006250 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.286892 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/Jinja2-2.7.3-py2-none-any.whl
--rw-rw-rw-   0        0        0      433 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/Jinja2.ABOUT
--rw-rw-rw-   0        0        0     1523 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/Jinja2.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/MarkupSafe-0.23-py2-none-any.whl
--rw-rw-rw-   0        0        0      447 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/MarkupSafe.ABOUT
--rw-rw-rw-   0        0        0     1582 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/MarkupSafe.LICENSE
--rw-rw-rw-   0        0        0       79 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/NOTICE
--rw-rw-rw-   0        0        0    33061 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/PSF.LICENSE
--rw-rw-rw-   0        0        0      474 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/about.ABOUT
--rw-rw-rw-   0        0        0    10174 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/apache-2.0.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/certifi-14.05.14-py2.py3-none-any.whl
--rw-rw-rw-   0        0        0      269 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/certifi.ABOUT
--rw-rw-rw-   0        0        0     1048 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/certifi.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/click-3.2-py2.py3-none-any.whl
--rw-rw-rw-   0        0        0      739 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/click.ABOUT
--rw-rw-rw-   0        0        0     1788 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/click.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/colorama-0.3.1-py2-none-any.whl
--rw-rw-rw-   0        0        0      490 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/colorama.ABOUT
--rw-rw-rw-   0        0        0     1492 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/colorama.LICENSE
--rw-rw-rw-   0        0        0    26478 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/lgpl-2.1.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/pip-1.5.6-py2.py3-none-any.whl
--rw-rw-rw-   0        0        0      452 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/pip.ABOUT
--rw-rw-rw-   0        0        0     4939 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/pip.AUTHORS
--rw-rw-rw-   0        0        0     1907 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/pip.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/py-1.4.23-py2-none-any.whl
--rw-rw-rw-   0        0        0      510 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/py.ABOUT
--rw-rw-rw-   0        0        0     1061 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/py.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/pytest-2.6.1-py2.py3-none-any.whl
--rw-rw-rw-   0        0        0      520 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/pytest.ABOUT
--rw-rw-rw-   0        0        0     1061 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/pytest.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/schematics-0.9_5-py2-none-any.whl
--rw-rw-rw-   0        0        0      392 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/schematics.ABOUT
--rw-rw-rw-   0        0        0     1524 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/schematics.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/setuptools-5.6-py2.py3-none-any.whl
--rw-rw-rw-   0        0        0      359 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/setuptools.ABOUT
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/unicodecsv-0.9.4-py2-none-any.whl
--rw-rw-rw-   0        0        0      430 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/unicodecsv.ABOUT
--rw-rw-rw-   0        0        0     1486 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/unicodecsv.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/wheel-0.24.0-py2.py3-none-any.whl
--rw-rw-rw-   0        0        0      472 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/wheel.ABOUT
--rw-rw-rw-   0        0        0     1125 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/wheel.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/wincertstore-0.2-py2.py3-none-any.whl
--rw-rw-rw-   0        0        0      443 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/wincertstore.ABOUT
--rw-rw-rw-   0        0        0     2409 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/wincertstore.LICENSE
--rw-rw-rw-   0        0        0       56 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about_file_path_dir_endswith_space.csv
--rw-rw-rw-   0        0        0     5510 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/expected.csv
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.299886 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/lic_issue_450/
--rw-rw-rw-   0        0        0       26 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/lic_issue_450/custom.txt
--rw-rw-rw-   0        0        0      135 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/lic_issue_450/custom_and_valid_lic_key_with_file.csv
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.324890 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/load/
--rw-rw-rw-   0        0        0    59301 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/load/clean-text-0.3.0-lceupi.json
--rw-rw-rw-   0        0        0    10224 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/load/simple_sample.xlsx
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.327888 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/multi_lic_issue_443/
--rw-rw-rw-   0        0        0      152 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/multi_lic_issue_443/test.csv
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.330889 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/multi_lic_issue_444/
--rw-rw-rw-   0        0        0      108 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/multi_lic_issue_444/test1.csv
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.355897 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/parser_tests/
--rw-rw-rw-   0        0        0       39 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/parser_tests/.ABOUT
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/parser_tests/about_resource.c
--rw-rw-rw-   0        0        0       58 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/parser_tests/about_resource_field.ABOUT
--rw-rw-rw-   0        0        0      290 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/parser_tests/about_resource_field_present.ABOUT
--rw-rw-rw-   0        0        0       76 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/parser_tests/missing_about_ref.ABOUT
--rw-rw-rw-   0        0        0      363 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/parser_tests/upper_field_names.ABOUT
--rw-rw-rw-   0        0        0       71 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_gen/this.ABOUT
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.374422 aboutcode-toolkit-8.0.0/tests/testdata/test_model/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.383422 aboutcode-toolkit-8.0.0/tests/testdata/test_model/android/
--rw-rw-rw-   0        0        0       83 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/android/expected_NOTICE
--rw-rw-rw-   0        0        0      543 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/android/multi_license.c.ABOUT
--rw-rw-rw-   0        0        0       62 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/android/public-domain.LICENSE
--rw-rw-rw-   0        0        0      350 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/android/single_license.c.ABOUT
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.389422 aboutcode-toolkit-8.0.0/tests/testdata/test_model/base_dir/
--rw-rw-rw-   0        0        0       17 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/base_dir/license.LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.395426 aboutcode-toolkit-8.0.0/tests/testdata/test_model/collect_inventory_errors/
--rw-rw-rw-   0        0        0       82 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/collect_inventory_errors/non-supported_date_format.ABOUT
--rw-rw-rw-   0        0        0       75 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/collect_inventory_errors/supported_date_format.ABOUT
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.401418 aboutcode-toolkit-8.0.0/tests/testdata/test_model/crlf/
--rw-rw-rw-   0        0        0      114 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/crlf/about.ABOUT
--rw-rw-rw-   0        0        0      104 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/crlf/expected.csv
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.404425 aboutcode-toolkit-8.0.0/tests/testdata/test_model/custom_fields/
--rw-rw-rw-   0        0        0      121 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/custom_fields/custom_fields.about
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.414420 aboutcode-toolkit-8.0.0/tests/testdata/test_model/dumps/
--rw-rw-rw-   0        0        0       79 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/dumps/NOTICE
--rw-rw-rw-   0        0        0      534 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/dumps/about.ABOUT
--rw-rw-rw-   0        0        0      157 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/dumps/apache-2.0.LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.064332 aboutcode-toolkit-8.0.0/tests/testdata/test_model/equal/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.424419 aboutcode-toolkit-8.0.0/tests/testdata/test_model/equal/complete/
--rw-rw-rw-   0        0        0       83 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/equal/complete/NOTICE
--rw-rw-rw-   0        0        0      518 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/equal/complete/about.ABOUT
--rw-rw-rw-   0        0        0       78 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/equal/complete/apache-2.0.LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.431428 aboutcode-toolkit-8.0.0/tests/testdata/test_model/equal/complete2/
--rw-rw-rw-   0        0        0       86 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/equal/complete2/NOTICE
--rw-rw-rw-   0        0        0      528 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/equal/complete2/about.ABOUT
--rw-rw-rw-   0        0        0       73 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/equal/complete2/apache-2.0.LICENSE
--rw-rw-rw-   0        0        0       60 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/expected.csv
--rw-rw-rw-   0        0        0      106 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/expected.json
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.437418 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.439429 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/basic/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.448436 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/basic/about/
--rw-rw-rw-   0        0        0       79 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/basic/about/NOTICE
--rw-rw-rw-   0        0        0      497 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/basic/about/about.ABOUT
--rw-rw-rw-   0        0        0      157 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/basic/about/apache-2.0.LICENSE
--rw-rw-rw-   0        0        0      483 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/basic/expected.csv
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.452434 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/basic_with_about_resource_path/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.457436 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/basic_with_about_resource_path/about/
--rw-rw-rw-   0        0        0       64 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/basic_with_about_resource_path/about/about_with_about_resource_path.ABOUT
--rw-rw-rw-   0        0        0      157 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/basic_with_about_resource_path/about/apache-2.0.LICENSE
--rw-rw-rw-   0        0        0       67 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/basic_with_about_resource_path/expected.csv
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.470960 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complete/
--rw-rw-rw-   0        0        0       79 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complete/NOTICE
--rw-rw-rw-   0        0        0      509 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complete/about.ABOUT
--rw-rw-rw-   0        0        0      157 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complete/apache-2.0.LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.489961 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.677080 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/Jinja2-2.7.3-py2-none-any.whl
--rw-rw-rw-   0        0        0      433 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/Jinja2.ABOUT
--rw-rw-rw-   0        0        0     1523 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/Jinja2.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/MarkupSafe-0.23-py2-none-any.whl
--rw-rw-rw-   0        0        0      447 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/MarkupSafe.ABOUT
--rw-rw-rw-   0        0        0     1582 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/MarkupSafe.LICENSE
--rw-rw-rw-   0        0        0       79 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/NOTICE
--rw-rw-rw-   0        0        0    33061 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/PSF.LICENSE
--rw-rw-rw-   0        0        0      474 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/about.ABOUT
--rw-rw-rw-   0        0        0    10174 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/apache-2.0.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/certifi-14.05.14-py2.py3-none-any.whl
--rw-rw-rw-   0        0        0      269 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/certifi.ABOUT
--rw-rw-rw-   0        0        0     1048 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/certifi.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/click-3.2-py2.py3-none-any.whl
--rw-rw-rw-   0        0        0      739 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/click.ABOUT
--rw-rw-rw-   0        0        0     1788 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/click.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/colorama-0.3.1-py2-none-any.whl
--rw-rw-rw-   0        0        0      490 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/colorama.ABOUT
--rw-rw-rw-   0        0        0     1492 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/colorama.LICENSE
--rw-rw-rw-   0        0        0    26478 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/lgpl-2.1.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/pip-1.5.6-py2.py3-none-any.whl
--rw-rw-rw-   0        0        0      452 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/pip.ABOUT
--rw-rw-rw-   0        0        0     4939 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/pip.AUTHORS
--rw-rw-rw-   0        0        0     1907 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/pip.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/py-1.4.23-py2-none-any.whl
--rw-rw-rw-   0        0        0      510 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/py.ABOUT
--rw-rw-rw-   0        0        0     1061 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/py.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/pytest-2.6.1-py2.py3-none-any.whl
--rw-rw-rw-   0        0        0      520 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/pytest.ABOUT
--rw-rw-rw-   0        0        0     1061 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/pytest.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/schematics-0.9_5-py2-none-any.whl
--rw-rw-rw-   0        0        0      392 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/schematics.ABOUT
--rw-rw-rw-   0        0        0     1524 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/schematics.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/setuptools-5.6-py2.py3-none-any.whl
--rw-rw-rw-   0        0        0      359 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/setuptools.ABOUT
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/unicodecsv-0.9.4-py2-none-any.whl
--rw-rw-rw-   0        0        0      430 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/unicodecsv.ABOUT
--rw-rw-rw-   0        0        0     1486 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/unicodecsv.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/virtualenv-1.11.6-py2.py3-none-any.whl
--rw-rw-rw-   0        0        0      625 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/virtualenv.ABOUT
--rw-rw-rw-   0        0        0     1180 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/virtualenv.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/virtualenv.py
--rw-rw-rw-   0        0        0      600 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/virtualenv.py.ABOUT
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/wheel-0.24.0-py2.py3-none-any.whl
--rw-rw-rw-   0        0        0      472 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/wheel.ABOUT
--rw-rw-rw-   0        0        0     1125 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/wheel.LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/wincertstore-0.2-py2.py3-none-any.whl
--rw-rw-rw-   0        0        0      443 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/wincertstore.ABOUT
--rw-rw-rw-   0        0        0     2409 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/wincertstore.LICENSE
--rw-rw-rw-   0        0        0     5993 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/expected.csv
--rw-rw-rw-   0        0        0       64 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/custom_fields.ABOUT
--rw-rw-rw-   0        0        0       64 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/custom_fields2.ABOUT
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.071331 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/no_about_resource_key/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.680080 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/no_about_resource_key/about/
--rw-rw-rw-   0        0        0       15 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/no_about_resource_key/about/about.ABOUT
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.686082 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/relative/
--rw-rw-rw-   0        0        0       79 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/relative/NOTICE
--rw-rw-rw-   0        0        0      509 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/relative/about.ABOUT
--rw-rw-rw-   0        0        0      157 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/relative/apache-2.0.LICENSE
--rw-rw-rw-   0        0        0    12428 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/longpath.zip
--rw-rw-rw-   0        0        0      168 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/multiple_files.ABOUT
--rw-rw-rw-   0        0        0      175 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/multiple_files_expected.csv
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.748087 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/
--rw-rw-rw-   0        0        0       41 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/basic.about
--rw-rw-rw-   0        0        0      129 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/boolean_data.about
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.759605 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/complete2/
--rw-rw-rw-   0        0        0       79 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/complete2/NOTICE
--rw-rw-rw-   0        0        0       91 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/complete2/about.ABOUT
--rw-rw-rw-   0        0        0      117 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/complete2/about2.ABOUT
--rw-rw-rw-   0        0        0      157 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/complete2/apache-2.0.LICENSE
--rw-rw-rw-   0        0        0      115 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/complex.about
--rw-rw-rw-   0        0        0       89 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/continuation.about
--rw-rw-rw-   0        0        0      116 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/continuation_verbatim.about
--rw-rw-rw-   0        0        0       96 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/continuation_verbatim_with_tab.about
--rw-rw-rw-   0        0        0       63 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/dupe_field_name.ABOUT
--rw-rw-rw-   0        0        0       55 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/dupe_field_name_no_new_value.ABOUT
--rw-rw-rw-   0        0        0       70 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/empty_notice_field.about
--rw-rw-rw-   0        0        0       23 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/empty_required.ABOUT
--rw-rw-rw-   0        0        0       56 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/illegal_custom_field.about
--rw-rw-rw-   0        0        0       55 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/invalid_boolean.about
--rw-rw-rw-   0        0        0      102 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/invalid_continuation.about
--rw-rw-rw-   0        0        0      148 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/invalid_names.about
--rw-rw-rw-   0        0        0      122 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/license_file_notice_file.ABOUT
--rw-rw-rw-   0        0        0      181 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/license_text.LICENSE
--rw-rw-rw-   0        0        0       55 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/missing_notice_file.ABOUT
--rw-rw-rw-   0        0        0       89 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/missing_notice_license_files.ABOUT
--rw-rw-rw-   0        0        0       70 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/missing_required.ABOUT
--rw-rw-rw-   0        0        0      280 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/multi_line_license_expresion.ABOUT
--rw-rw-rw-   0        0        0       64 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/name_mapping_test.ABOUT
--rw-rw-rw-   0        0        0       29 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/no_file_fields.ABOUT
--rw-rw-rw-   0        0        0       80 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/non_ascii_field_name_value.about
--rw-rw-rw-   0        0        0       44 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/notice_text.NOTICE
--rw-rw-rw-   0        0        0       75 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/parse/ordered_fields.ABOUT
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.767616 aboutcode-toolkit-8.0.0/tests/testdata/test_model/redistribution/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.075333 aboutcode-toolkit-8.0.0/tests/testdata/test_model/redistribution/test/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.773621 aboutcode-toolkit-8.0.0/tests/testdata/test_model/redistribution/test/subdir/
--rw-rw-rw-   0        0        0       44 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/redistribution/test/subdir/test.ABOUT
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/redistribution/test/subdir/test.c
--rw-rw-rw-   0        0        0       67 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/redistribution/this.ABOUT
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/redistribution/this.c
--rw-rw-rw-   0        0        0       69 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/redistribution/this2.ABOUT
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/redistribution/this2.c
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.080330 aboutcode-toolkit-8.0.0/tests/testdata/test_model/rel/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.078337 aboutcode-toolkit-8.0.0/tests/testdata/test_model/rel/allAboutInOneDir/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.809617 aboutcode-toolkit-8.0.0/tests/testdata/test_model/rel/allAboutInOneDir/about_ref/
--rw-rw-rw-   0        0        0      314 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/rel/allAboutInOneDir/about_ref/csv_serialize.py.ABOUT
--rw-rw-rw-   0        0        0      472 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/rel/allAboutInOneDir/about_ref/django_snippets_2413.ABOUT
--rw-rw-rw-   0        0        0      720 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/rel/allAboutInOneDir/about_ref/elasticsearch.ABOUT
--rw-rw-rw-   0        0        0      322 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/rel/allAboutInOneDir/about_ref/ez_setup.py.ABOUT
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:37.079332 aboutcode-toolkit-8.0.0/tests/testdata/test_model/rel/allAboutInOneDir/about_ref/t1/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.811616 aboutcode-toolkit-8.0.0/tests/testdata/test_model/rel/allAboutInOneDir/about_ref/t1/t2/
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/rel/allAboutInOneDir/about_ref/t1/t2/ez_setup.py
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.818618 aboutcode-toolkit-8.0.0/tests/testdata/test_model/rel/thirdparty/
--rw-rw-rw-   0        0        0        0 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/rel/thirdparty/django_snippets.LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/rel/thirdparty/elasticsearch.LICENSE
--rw-rw-rw-   0        0        0      165 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/rel/thirdparty/elasticsearch.NOTICE
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.827629 aboutcode-toolkit-8.0.0/tests/testdata/test_model/serialize/
--rw-rw-rw-   0        0        0       79 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/serialize/NOTICE
--rw-rw-rw-   0        0        0      509 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/serialize/about.ABOUT
--rw-rw-rw-   0        0        0      157 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/serialize/apache-2.0.LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.846620 aboutcode-toolkit-8.0.0/tests/testdata/test_model/single_file/
--rw-rw-rw-   0        0        0     1159 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/single_file/django_snippets.LICENSE
--rw-rw-rw-   0        0        0      438 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/single_file/django_snippets_2413.ABOUT
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/single_file/django_snippets_2413.py
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.854643 aboutcode-toolkit-8.0.0/tests/testdata/test_model/special/
--rw-rw-rw-   0        0        0       79 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/special/NOTICE
--rw-rw-rw-   0        0        0      509 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/special/about.ABOUT
--rw-rw-rw-   0        0        0      157 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/special/apache-2.0.LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.857628 aboutcode-toolkit-8.0.0/tests/testdata/test_model/special_char/
--rw-rw-rw-   0        0        0       77 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/special_char/about.ABOUT
--rw-rw-rw-   0        0        0       50 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/this.ABOUT
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.863091 aboutcode-toolkit-8.0.0/tests/testdata/test_model/unicode/
--rw-rw-rw-   0        0        0      518 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/unicode/nose-selecttests.ABOUT
--rw-rw-rw-   0        0        0       31 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_model/unicode/not-unicode.ABOUT
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.945105 aboutcode-toolkit-8.0.0/tests/testdata/test_transform/
--rw-rw-rw-   0        0        0      215 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_transform/configuration
--rw-rw-rw-   0        0        0      113 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_transform/configuration2
--rw-rw-rw-   0        0        0      108 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_transform/configuration_new_cols
--rw-rw-rw-   0        0        0       98 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_transform/input.csv
--rw-rw-rw-   0        0        0      163 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_transform/input.json
--rw-rw-rw-   0        0        0     9995 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_transform/input.xlsx
--rw-rw-rw-   0        0        0     1761 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_transform/input_scancode.json
--rw-rw-rw-   0        0        0       97 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_transform/simple.csv
--rw-rw-rw-   0        0        0    10056 2023-03-09 10:07:06.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_transform/simple.xlsx
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.948097 aboutcode-toolkit-8.0.0/tests/testdata/test_util/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.957100 aboutcode-toolkit-8.0.0/tests/testdata/test_util/about_locations/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.962628 aboutcode-toolkit-8.0.0/tests/testdata/test_util/about_locations/dir1/
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.964626 aboutcode-toolkit-8.0.0/tests/testdata/test_util/about_locations/dir1/dir2/
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/about_locations/dir1/dir2/file1.about
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/about_locations/dir1/file2
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/about_locations/dir1/file2.aBout
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.966626 aboutcode-toolkit-8.0.0/tests/testdata/test_util/about_locations/dir2/
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/about_locations/dir2/file1
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/about_locations/file with_spaces.ABOUT
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/about_locations/file1
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/about_locations/file2
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.979626 aboutcode-toolkit-8.0.0/tests/testdata/test_util/csv/
--rw-rw-rw-   0        0        0       72 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/csv/about.csv
--rw-rw-rw-   0        0        0       70 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/csv/about_key_with_upper_case.csv
--rw-rw-rw-   0        0        0       40 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/csv/test_ms_utf8.csv
--rw-rw-rw-   0        0        0       34 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/csv/test_utf8.csv
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:38.989632 aboutcode-toolkit-8.0.0/tests/testdata/test_util/get_about_locations/
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/get_about_locations/NOTICE
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/get_about_locations/about.ABOUT
--rw-rw-rw-   0        0        0        0 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/get_about_locations/apache-2.0.LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:39.008625 aboutcode-toolkit-8.0.0/tests/testdata/test_util/json/
--rw-rw-rw-   0        0        0     1078 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/json/aboutcode_manager_exported.json
--rw-rw-rw-   0        0        0      140 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/json/expected.json
--rw-rw-rw-   0        0        0      135 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/json/expected_need_mapping.json
--rw-rw-rw-   0        0        0      130 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/json/not_a_list.json
--rw-rw-rw-   0        0        0      119 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/json/not_a_list_need_mapping.json
--rw-rw-rw-   0        0        0     1361 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/json/scancode_info.json
-drwxrwxrwx   0        0        0        0 2023-03-09 10:10:39.015634 aboutcode-toolkit-8.0.0/tests/testdata/test_util/licenses/
--rw-rw-rw-   0        0        0     1084 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/licenses/mit.LICENSE
--rw-rw-rw-   0        0        0     1084 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/licenses/mit2.LICENSE
--rw-rw-rw-   0        0        0       62 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/licenses/public-domain.LICENSE
--rw-rw-rw-   0        0        0    12428 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testdata/test_util/longpath.zip
--rw-rw-rw-   0        0        0     6512 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tests/testing_utils.py
--rw-rw-rw-   0        0        0      130 2022-04-11 01:40:16.000000 aboutcode-toolkit-8.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.325777 aboutcode-toolkit-9.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.253776 aboutcode-toolkit-9.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.265776 aboutcode-toolkit-9.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/.github/workflows/docs-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      525 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10940 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3422 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)      218 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)     6660 2023-07-14 10:34:44.325777 aboutcode-toolkit-9.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5309 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (122)      537 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/about
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/about.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      879 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/about.bat
+-rw-r--r--   0 runner    (1001) docker     (122)    11558 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      628 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/azure-pipelines.yml
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6328 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/configure
+-rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/configure.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.269776 aboutcode-toolkit-9.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.269776 aboutcode-toolkit-9.0.0/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/docs/scripts/doc8_style_check.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/docs/scripts/sphinx_build_link_check.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.269776 aboutcode-toolkit-9.0.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.269776 aboutcode-toolkit-9.0.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)    10299 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/docs/source/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3368 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21604 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/docs/source/general.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5296 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/docs/source/home.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    28753 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/docs/source/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    17066 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/docs/source/specification.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/docs/source/type_of_errors.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.253776 aboutcode-toolkit-9.0.0/etc/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.269776 aboutcode-toolkit-9.0.0/etc/ci/
+-rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/ci/azure-container-deb.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/ci/azure-container-rpm.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/ci/azure-posix.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/ci/azure-win.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/ci/install_sudo.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     8365 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/ci/macports-ci
+-rw-r--r--   0 runner    (1001) docker     (122)      684 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/ci/macports-ci.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/ci/mit.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.273776 aboutcode-toolkit-9.0.0/etc/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)     3744 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/check_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9486 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/fetch_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9699 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/gen_pypi_simple.py
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/gen_pypi_simple.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     2776 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/gen_pypi_simple.py.NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/gen_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2266 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/gen_requirements_dev.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4497 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/test_utils_pip_compatibility_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     2839 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/test_utils_pypi_supported_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     6418 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/utils_dejacode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6704 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/utils_pip_compatibility_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      494 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/utils_pypi_supported_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     6152 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/utils_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)    75931 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/utils_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (122)      608 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/etc/scripts/utils_thirdparty.py.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.253776 aboutcode-toolkit-9.0.0/example/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.257776 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.253776 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.273776 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/alocal.m4.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.273776 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/config/config.guess.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/config/config.rpath.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/config/config.sub.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/config/gpl-2.0-autoconf.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/config/mkinstalldirs.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/config/public-domain.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.273776 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/contrib/
+-rw-r--r--   0 runner    (1001) docker     (122)      320 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/contrib/UlrichWindl.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      284 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/contrib/dconf.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.277776 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/KazKylheku.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/argv_parse.c.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/argv_parse.h.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/dict.c.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/dict.h.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)    18409 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/gpl-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/journal.c.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)    25751 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/lgpl-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/mit-old-style-legal-2.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/mtrace.c.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/mtrace.h.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/profile.c.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/profile.h.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      500 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsprogs-1.39.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1438 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsprogs-1.39.NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)    18409 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/gpl-2.0.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.253776 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/include/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.277776 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/include/nonunix/
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/include/nonunix/getopt.h.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)    25751 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/include/nonunix/lgpl-2.0.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.277776 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/install-utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      430 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/install-utils/convfstab.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/install-utils/public-domain.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.277776 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/intl/
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/intl/intl.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)    25751 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/intl/lgpl-2.0.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.277776 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.277776 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/blkid/
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/blkid/blkid.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)    26742 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/blkid/lgpl-2.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/bsla.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.277776 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/e2p/
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/e2p/e2p.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)    25751 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/e2p/lgpl-2.0.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.277776 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/bsd-new.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/bsla.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      446 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/com_right.c.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/et.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)    18409 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/gpl-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     6406 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/kerberos.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      436 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/texinfo.tex.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/vfprintf.c.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      384 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/fpopen.c.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.277776 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/ss/
+-rw-r--r--   0 runner    (1001) docker     (122)     6406 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/ss/kerberos.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/ss/ss.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.277776 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/uuid/
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/uuid/bsd-new.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/uuid/uuid.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.281776 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/misc/
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/misc/blkid.c.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)    26742 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/misc/lgpl-2.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/public-domain.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.281776 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/input/
+-rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/input/MAPPING.CONFIG
+-rw-r--r--   0 runner    (1001) docker     (122)     7094 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/input/e2fsprogs-1.39-CreateAboutFile.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    14597 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/input/e2fsprogs-1.39-INV.xlsx
+-rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/input/template_sample_attribution_starship.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.281776 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/output/
+-rw-r--r--   0 runner    (1001) docker     (122)   118207 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/output/sample_attribution_starship.html
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1602 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1798 2023-07-14 10:34:44.325777 aboutcode-toolkit-9.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.257776 aboutcode-toolkit-9.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.281776 aboutcode-toolkit-9.0.0/src/aboutcode_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6660 2023-07-14 10:34:44.000000 aboutcode-toolkit-9.0.0/src/aboutcode_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    23982 2023-07-14 10:34:44.000000 aboutcode-toolkit-9.0.0/src/aboutcode_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 10:34:44.000000 aboutcode-toolkit-9.0.0/src/aboutcode_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-14 10:34:44.000000 aboutcode-toolkit-9.0.0/src/aboutcode_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 10:34:44.000000 aboutcode-toolkit-9.0.0/src/aboutcode_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-07-14 10:34:44.000000 aboutcode-toolkit-9.0.0/src/aboutcode_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-07-14 10:34:44.000000 aboutcode-toolkit-9.0.0/src/aboutcode_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.281776 aboutcode-toolkit-9.0.0/src/attributecode/
+-rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/src/attributecode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/src/attributecode/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3445 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/src/attributecode/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12660 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/src/attributecode/attrib.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4274 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/src/attributecode/attrib_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32449 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/src/attributecode/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16032 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/src/attributecode/gen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/src/attributecode/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (122)    71679 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/src/attributecode/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.285776 aboutcode-toolkit-9.0.0/src/attributecode/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     3368 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/src/attributecode/templates/default_html.template
+-rw-r--r--   0 runner    (1001) docker     (122)      768 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/src/attributecode/templates/default_json.template
+-rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/src/attributecode/templates/license_ref.template
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/src/attributecode/templates/list.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/src/attributecode/templates/scancode_html.template
+-rw-r--r--   0 runner    (1001) docker     (122)    14186 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/src/attributecode/transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25088 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/src/attributecode/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.285776 aboutcode-toolkit-9.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3502 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11418 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/test_attrib.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12179 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/test_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14845 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/test_gen.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51493 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9989 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23518 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.261776 aboutcode-toolkit-9.0.0/tests/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.257776 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.285776 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/default_template/
+-rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/default_template/expect.html
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/default_template/simple_sample.csv
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.285776 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/gen_default_template/
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/gen_default_template/attrib.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      926 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/gen_default_template/expected_default_attrib.html
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/gen_default_template/httpd-2.4.3.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.285776 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/gen_license_key_name_check/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.285776 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/gen_license_key_name_check/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/gen_license_key_name_check/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/gen_license_key_name_check/LICENSES/LGPL-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/gen_license_key_name_check/custom.template
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.285776 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/gen_license_key_name_check/expected/
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/gen_license_key_name_check/expected/expected.html
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/gen_license_key_name_check/test.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.285776 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/gen_simple/
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/gen_simple/attrib.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/gen_simple/httpd-2.4.3.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/gen_simple/test.template
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.285776 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/scancode_input/
+-rw-r--r--   0 runner    (1001) docker     (122)     4800 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/scancode_input/clean-text-0.3.0-mod-lceupi.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3485 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/scancode_input/expect.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3072 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/scancode_input/scancode.template
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.285776 aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/
+-rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/geninventory.csv
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.289776 aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/help/
+-rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/help/about_attrib_help.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/help/about_check_help.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/help/about_gen_help.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/help/about_gen_license_help.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/help/about_help.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/help/about_inventory_help.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/help/about_transform_config_help.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      822 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/help/about_transform_help.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.289776 aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/repository-mini/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/repository-mini/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/repository-mini/appdirs-1.4.3-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/repository-mini/appdirs.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/repository-mini/appdirs.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/repository-mini/mit.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/repository-mini/xtrans-1.3.5.txz
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/repository-mini/xtrans-1.3.5.txz.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1280 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/transform.csv
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.289776 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/about.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/dup_keys.csv
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/dup_keys_with_diff_case.csv
+-rw-r--r--   0 runner    (1001) docker     (122)      426 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inv.csv
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inv2.csv
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inv3.csv
+-rw-r--r--   0 runner    (1001) docker     (122)      164 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inv4.csv
+-rw-r--r--   0 runner    (1001) docker     (122)      426 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inv5.csv
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inv6.csv
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inv_no_about_resource.csv
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.257776 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.289776 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.297777 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/Jinja2-2.7.3-py2-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      433 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/Jinja2.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/Jinja2.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/MarkupSafe-0.23-py2-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      447 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/MarkupSafe.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/MarkupSafe.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)    33061 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/PSF.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      474 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/about.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/certifi-14.05.14-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/certifi.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/certifi.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/click-3.2-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      739 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/click.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1788 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/click.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/colorama-0.3.1-py2-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      490 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/colorama.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/colorama.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    26478 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/lgpl-2.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/pip-1.5.6-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      452 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/pip.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     4939 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/pip.AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/pip.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/py-1.4.23-py2-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/py.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/pytest-2.6.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/pytest.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/pytest.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/schematics-0.9_5-py2-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/schematics.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/schematics.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/setuptools-5.6-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/setuptools.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/unicodecsv-0.9.4-py2-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      430 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/unicodecsv.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/unicodecsv.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/wheel-0.24.0-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/wheel.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/wheel.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/wincertstore-0.2-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      443 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/wincertstore.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/wincertstore.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about_file_path_dir_endswith_space.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     5510 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/expected.csv
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.297777 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/lic_issue_450/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/lic_issue_450/custom.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/lic_issue_450/custom_and_valid_lic_key_with_file.csv
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.297777 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/load/
+-rw-r--r--   0 runner    (1001) docker     (122)    59301 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/load/clean-text-0.3.0-lceupi.json
+-rw-r--r--   0 runner    (1001) docker     (122)    10224 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/load/simple_sample.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.297777 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/multi_lic_issue_443/
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/multi_lic_issue_443/test.csv
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.297777 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/multi_lic_issue_444/
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/multi_lic_issue_444/test1.csv
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.297777 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/parser_tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/parser_tests/.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/parser_tests/about_resource.c
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/parser_tests/about_resource_field.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      290 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/parser_tests/about_resource_field_present.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/parser_tests/missing_about_ref.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/parser_tests/upper_field_names.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_gen/this.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.301777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.301777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/android/
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/android/expected_NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)      543 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/android/multi_license.c.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/android/public-domain.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/android/single_license.c.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.301777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/base_dir/
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/base_dir/license.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.301777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/collect_inventory_errors/
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/collect_inventory_errors/non-supported_date_format.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/collect_inventory_errors/supported_date_format.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.301777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/crlf/
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/crlf/about.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/crlf/expected.csv
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.301777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/custom_fields/custom_fields.about
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.301777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/dumps/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/dumps/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)      534 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/dumps/about.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/dumps/apache-2.0.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.261776 aboutcode-toolkit-9.0.0/tests/testdata/test_model/equal/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.301777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/equal/complete/
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/equal/complete/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/equal/complete/about.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/equal/complete/apache-2.0.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.301777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/equal/complete2/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/equal/complete2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)      528 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/equal/complete2/about.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/equal/complete2/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/expected.csv
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/expected.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.301777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.301777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/basic/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.305776 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/basic/about/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/basic/about/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/basic/about/about.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/basic/about/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      483 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/basic/expected.csv
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.305776 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/basic_with_about_resource_path/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.305776 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/basic_with_about_resource_path/about/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/basic_with_about_resource_path/about/about_with_about_resource_path.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/basic_with_about_resource_path/about/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/basic_with_about_resource_path/expected.csv
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.305776 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complete/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complete/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complete/about.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complete/apache-2.0.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.305776 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.313777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/Jinja2-2.7.3-py2-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      433 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/Jinja2.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/Jinja2.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/MarkupSafe-0.23-py2-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      447 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/MarkupSafe.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/MarkupSafe.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)    33061 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/PSF.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      474 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/about.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/certifi-14.05.14-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/certifi.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/certifi.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/click-3.2-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      739 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/click.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1788 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/click.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/colorama-0.3.1-py2-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      490 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/colorama.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/colorama.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    26478 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/lgpl-2.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/pip-1.5.6-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      452 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/pip.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     4939 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/pip.AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/pip.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/py-1.4.23-py2-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/py.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/pytest-2.6.1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/pytest.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/pytest.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/schematics-0.9_5-py2-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/schematics.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/schematics.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/setuptools-5.6-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/setuptools.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/unicodecsv-0.9.4-py2-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      430 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/unicodecsv.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/unicodecsv.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/virtualenv-1.11.6-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/virtualenv.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1180 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/virtualenv.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/virtualenv.py
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/virtualenv.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/wheel-0.24.0-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/wheel.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/wheel.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/wincertstore-0.2-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)      443 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/wincertstore.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/wincertstore.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     5993 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/expected.csv
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/custom_fields.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/custom_fields2.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.261776 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/no_about_resource_key/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.313777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/no_about_resource_key/about/
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/no_about_resource_key/about/about.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.313777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/relative/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/relative/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/relative/about.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/relative/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    12428 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/longpath.zip
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/multiple_files.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/multiple_files_expected.csv
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.317777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/basic.about
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/boolean_data.about
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.317777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/complete2/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/complete2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/complete2/about.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/complete2/about2.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/complete2/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/complex.about
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/continuation.about
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/continuation_verbatim.about
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/continuation_verbatim_with_tab.about
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/dupe_field_name.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/dupe_field_name_no_new_value.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/empty_notice_field.about
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/empty_required.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/illegal_custom_field.about
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/invalid_boolean.about
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/invalid_continuation.about
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/invalid_names.about
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/license_file_notice_file.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/license_text.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/missing_notice_file.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/missing_notice_license_files.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/missing_required.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/multi_line_license_expresion.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/name_mapping_test.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/no_file_fields.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/non_ascii_field_name_value.about
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/notice_text.NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/ordered_fields.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/parse/with_ignored_resources.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.317777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/redistribution/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.261776 aboutcode-toolkit-9.0.0/tests/testdata/test_model/redistribution/test/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.317777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/redistribution/test/subdir/
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/redistribution/test/subdir/test.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/redistribution/test/subdir/test.c
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/redistribution/this.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/redistribution/this.c
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/redistribution/this2.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/redistribution/this2.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.261776 aboutcode-toolkit-9.0.0/tests/testdata/test_model/rel/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.261776 aboutcode-toolkit-9.0.0/tests/testdata/test_model/rel/allAboutInOneDir/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.317777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/rel/allAboutInOneDir/about_ref/
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/rel/allAboutInOneDir/about_ref/csv_serialize.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/rel/allAboutInOneDir/about_ref/django_snippets_2413.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/rel/allAboutInOneDir/about_ref/elasticsearch.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/rel/allAboutInOneDir/about_ref/ez_setup.py.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.261776 aboutcode-toolkit-9.0.0/tests/testdata/test_model/rel/allAboutInOneDir/about_ref/t1/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.317777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/rel/allAboutInOneDir/about_ref/t1/t2/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/rel/allAboutInOneDir/about_ref/t1/t2/ez_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.317777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/rel/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/rel/thirdparty/django_snippets.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/rel/thirdparty/elasticsearch.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/rel/thirdparty/elasticsearch.NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.317777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/serialize/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/serialize/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/serialize/about.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/serialize/apache-2.0.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.317777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/single_file/
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/single_file/django_snippets.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/single_file/django_snippets_2413.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/single_file/django_snippets_2413.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.317777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/special/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/special/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/special/about.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/special/apache-2.0.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.317777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/special_char/
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/special_char/about.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/this.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.321777 aboutcode-toolkit-9.0.0/tests/testdata/test_model/unicode/
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/unicode/nose-selecttests.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_model/unicode/not-unicode.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.321777 aboutcode-toolkit-9.0.0/tests/testdata/test_transform/
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_transform/configuration
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_transform/configuration2
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_transform/configuration_new_cols
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_transform/input.csv
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_transform/input.json
+-rw-r--r--   0 runner    (1001) docker     (122)     9995 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_transform/input.xlsx
+-rw-r--r--   0 runner    (1001) docker     (122)     1761 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_transform/input_scancode.json
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_transform/simple.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    10056 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_transform/simple.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.321777 aboutcode-toolkit-9.0.0/tests/testdata/test_util/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.321777 aboutcode-toolkit-9.0.0/tests/testdata/test_util/about_locations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.321777 aboutcode-toolkit-9.0.0/tests/testdata/test_util/about_locations/dir1/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.321777 aboutcode-toolkit-9.0.0/tests/testdata/test_util/about_locations/dir1/dir2/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/about_locations/dir1/dir2/file1.about
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/about_locations/dir1/file2
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/about_locations/dir1/file2.aBout
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.321777 aboutcode-toolkit-9.0.0/tests/testdata/test_util/about_locations/dir2/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/about_locations/dir2/file1
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/about_locations/file with_spaces.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/about_locations/file1
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/about_locations/file2
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.321777 aboutcode-toolkit-9.0.0/tests/testdata/test_util/csv/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/csv/about.csv
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/csv/about_key_with_upper_case.csv
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/csv/test_ms_utf8.csv
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/csv/test_utf8.csv
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.321777 aboutcode-toolkit-9.0.0/tests/testdata/test_util/get_about_locations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/get_about_locations/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/get_about_locations/about.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/get_about_locations/apache-2.0.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.325777 aboutcode-toolkit-9.0.0/tests/testdata/test_util/json/
+-rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/json/aboutcode_manager_exported.json
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/json/expected.json
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/json/expected_need_mapping.json
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/json/not_a_list.json
+-rw-r--r--   0 runner    (1001) docker     (122)      119 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/json/not_a_list_need_mapping.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/json/scancode_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 10:34:44.325777 aboutcode-toolkit-9.0.0/tests/testdata/test_util/licenses/
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/licenses/mit.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/licenses/mit2.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/licenses/public-domain.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    12428 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testdata/test_util/longpath.zip
+-rw-r--r--   0 runner    (1001) docker     (122)     6512 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tests/testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-07-14 10:34:34.000000 aboutcode-toolkit-9.0.0/tox.ini
```

### Comparing `aboutcode-toolkit-8.0.0/.github/workflows/docs-ci.yml` & `aboutcode-toolkit-9.0.0/.github/workflows/docs-ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     strategy:
       max-parallel: 4
       matrix:
         python-version: [3.9]
 
     steps:
       - name: Checkout code
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Give permission to run scripts
         run: chmod +x ./docs/scripts/doc8_style_check.sh
 
       - name: Install Dependencies
```

### Comparing `aboutcode-toolkit-8.0.0/.github/workflows/pypi-release.yml` & `aboutcode-toolkit-9.0.0/.github/workflows/pypi-release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 jobs:
   build-pypi-distribs:
     name: Build and publish library to PyPI
     runs-on: ubuntu-20.04
 
     steps:
-      - uses: actions/checkout@master
+      - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v1
+        uses: actions/setup-python@v4
         with:
           python-version: 3.9
 
       - name: Install pypa/build
         run: python -m pip install build --user
 
       - name: Build a binary wheel and a source tarball
@@ -74,10 +74,10 @@
         uses: actions/download-artifact@v3
         with:
           name: pypi_archives
           path: dist
 
       - name: Publish to PyPI
         if: startsWith(github.ref, 'refs/tags')
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `aboutcode-toolkit-8.0.0/.gitignore` & `aboutcode-toolkit-9.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/CHANGELOG.rst` & `aboutcode-toolkit-9.0.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 ==============================
 Changelog
+
+2023-07-14
+    Release 9.0.0
+
+    * The tool will now show which worksheet (if .xlsx input) is the tool working on
+    * Error handling if defined worksheet does not exist
+    * Adopt 3.3.1 specification: introduce ``ignored_resources``
+
+
 2023-03-09
     Release 8.0.0
 
     * Fixed the transform code for xlsx and json
     * Remove irrelevant error for attrib
     * Add support to identify worksheet name for XLSX input
     * The severity error level for "contains illegal name characters (or empty spaces) and is ignored" is changed from ERROR to WARNING
```

### Comparing `aboutcode-toolkit-8.0.0/CODE_OF_CONDUCT.rst` & `aboutcode-toolkit-9.0.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/Dockerfile` & `aboutcode-toolkit-9.0.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/Makefile` & `aboutcode-toolkit-9.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/NOTICE` & `aboutcode-toolkit-9.0.0/NOTICE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/PKG-INFO` & `aboutcode-toolkit-9.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,193 +1,193 @@
-Metadata-Version: 2.1
-Name: aboutcode-toolkit
-Version: 8.0.0
-Summary: AboutCode-toolkit is a tool to document the provenance (origin and license) of third-party software using small text files. Collect inventories and generate attribution documentation.
-Home-page: https://github.com/nexB/aboutcode-toolkit
-Author: nexB. Inc. and others
-Author-email: info@aboutcode.org
-License: Apache-2.0
-Keywords: license,about,metadata,package,copyright,attribution,software,inventory,open source,sca,SBOM,spdx
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Documentation
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: Topic :: System :: Software Distribution
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: testing
-Provides-Extra: docs
-License-File: apache-2.0.LICENSE
-License-File: NOTICE
-License-File: AUTHORS.rst
-License-File: CHANGELOG.rst
-License-File: CODE_OF_CONDUCT.rst
-
-=================
-AboutCode Toolkit
-=================
-
-Introduction
-------------
-The AboutCode Toolkit and ABOUT files provide a simple way to document the
-origin, license, usage and other important or interesting information about
-third-party software components that you use in your project.
-
-You start by storing ABOUT files (a small YAML formatted text file with field/value pairs)
-side-by-side with each of the third-party software components you use.
-Each ABOUT file documents origin and license for one software.
-There are many examples of ABOUT files (valid or invalid) in the testdata/
-directory of the whole repository.
-
-The current version of the AboutCode Toolkit can read these ABOUT files so that you
-can collect and validate the inventory of third-party components that you use.
-
-In addition, this tool is able to generate attribution notices and
-identify redistributable source code used in your project to help you comply
-with open source licenses conditions.
-
-This version of the AboutCode Toolkit follows the ABOUT specification version 3.3.0 at:
-https://aboutcode-toolkit.readthedocs.io/en/latest/specification.html
-
-
-Build and tests status
-----------------------
-
-+-------+-----------------+--------------+
-|Branch | **Linux/macOS** | **Windows**  |
-+=======+=================+==============+
-|Master | |master-posix|  | |master-win| |
-+-------+-----------------+--------------+
-|Develop| |devel-posix|   | |devel-win|  |
-+-------+-----------------+--------------+
-
-
-REQUIREMENTS
-------------
-The AboutCode Toolkit is tested with Python 3.7 or above only on Linux, Mac and Windows.
-You will need to install a Python interpreter if you do not have one already
-installed.
-
-On Linux and Mac, Python is typically pre-installed. To verify which
-version may be pre-installed, open a terminal and type:
-
-    python --version
-
-Note
-~~~~
-    Debian has decided that distutils is not a core python package, so it is not included in the last versions of debian and debian-based OSes.
-    A solution is to run: `sudo apt install python3-distutils`
-
-On Windows or Mac, you can download the latest Python here:
-    https://www.python.org/downloads/
-
-Download the .msi installer for Windows or the .dmg archive for Mac.
-Open and run the installer using all the default options.
-
-INSTALLATION
-------------
-Checkout or download and extract the AboutCode Toolkit from:
-    https://github.com/nexB/aboutcode-toolkit/
-
-To install all the needed dependencies in a virtualenv, run (on posix):
-    ./configure
-or on windows:
-    configure
-
-ACTIVATE the VIRTUALENV
------------------------
-To activate the virtualenv, run (on posix):
-    source venv/bin/activate
-or on windows:
-    venv\\bin\\activate
-
-
-DEACTIVATE the VIRTUALENV
--------------------------
-To deactivate the virtualenv, run (on both posix and windows):
-    deactivate
-
-
-VERSIONING SCHEMA
------------------
-Starting at AboutCode version 4.0.0, the AboutCode Toolkit will follow SemVer for the versioning schema.
-
-i.e. MAJOR.MINOR.PATCH format
-    1. MAJOR version when making incompatible API changes,
-    2. MINOR version when making functionality in a backwards compatible manner, and
-    3. PATCH version when making backwards compatible bug fixes.
-
-
-REFERENCE
----------
-See https://aboutcode-toolkit.readthedocs.io/en/latest/ for documentation.
-
-See https://aboutcode-toolkit.readthedocs.io/en/latest/reference.html for reference.
-
-TESTS and DEVELOPMENT
----------------------
-To install all the needed development dependencies, run (on posix):
-    ./configure --dev
-or on windows:
-    configure --dev
-
-To verify that everything works fine you can run the test suite with:
-    pytest
-
-
-CLEAN BUILD AND INSTALLED FILES
--------------------------------
-To clean the built and installed files, run (on posix):
-    ./configure --clean
-or on windows:
-    configure --clean
-
-
-HELP and SUPPORT
-----------------
-If you have a question or find a bug, enter a ticket at:
-
-    https://github.com/nexB/aboutcode-toolkit
-
-For issues, you can use:
-
-    https://github.com/nexB/aboutcode-toolkit/issues
-
-
-SOURCE CODE
------------
-The AboutCode Toolkit is available through GitHub. For the latest version visit:
-    https://github.com/nexB/aboutcode-toolkit
-
-
-HACKING
--------
-We accept pull requests provided under the same license as this tool.
-You agree to the http://developercertificate.org/
-
-
-LICENSE
--------
-The AboutCode Toolkit is released under the Apache 2.0 license.
-See (of course) the about.ABOUT file for details.
-
-
-.. |master-posix| image:: https://api.travis-ci.org/nexB/aboutcode-toolkit.png?branch=master
-    :target: https://travis-ci.org/nexB/aboutcode-toolkit
-    :alt: Linux Master branch tests status
-.. |devel-posix| image:: https://api.travis-ci.org/nexB/aboutcode-toolkit.png?branch=develop
-    :target: https://travis-ci.org/nexB/aboutcode-toolkit
-    :alt: Linux Develop branch tests status
-
-.. |master-win| image:: https://ci.appveyor.com/api/projects/status/uwj2gh8i9ga1mqwn/branch/master?png=true
-    :target: https://ci.appveyor.com/project/nexB/aboutcode-toolkit
-    :alt: Windows Master branch tests status
-.. |devel-win| image:: https://ci.appveyor.com/api/projects/status/uwj2gh8i9ga1mqwn/branch/develop?png=true
-    :target: https://ci.appveyor.com/project/nexB/aboutcode-toolkit
-    :alt: Windows Develop branch tests status
+Metadata-Version: 2.1
+Name: aboutcode-toolkit
+Version: 9.0.0
+Summary: AboutCode-toolkit is a tool to document the provenance (origin and license) of third-party software using small text files. Collect inventories and generate attribution documentation.
+Home-page: https://github.com/nexB/aboutcode-toolkit
+Author: nexB. Inc. and others
+Author-email: info@aboutcode.org
+License: Apache-2.0
+Keywords: license,about,metadata,package,copyright,attribution,software,inventory,open source,sca,SBOM,spdx
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: System :: Software Distribution
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: testing
+Provides-Extra: docs
+License-File: apache-2.0.LICENSE
+License-File: NOTICE
+License-File: AUTHORS.rst
+License-File: CHANGELOG.rst
+License-File: CODE_OF_CONDUCT.rst
+
+=================
+AboutCode Toolkit
+=================
+
+Introduction
+------------
+The AboutCode Toolkit and ABOUT files provide a simple way to document the
+origin, license, usage and other important or interesting information about
+third-party software components that you use in your project.
+
+You start by storing ABOUT files (a small YAML formatted text file with field/value pairs)
+side-by-side with each of the third-party software components you use.
+Each ABOUT file documents origin and license for one software.
+There are many examples of ABOUT files (valid or invalid) in the testdata/
+directory of the whole repository.
+
+The current version of the AboutCode Toolkit can read these ABOUT files so that you
+can collect and validate the inventory of third-party components that you use.
+
+In addition, this tool is able to generate attribution notices and
+identify redistributable source code used in your project to help you comply
+with open source licenses conditions.
+
+This version of the AboutCode Toolkit follows the ABOUT specification version 3.3.1 at:
+https://aboutcode-toolkit.readthedocs.io/en/latest/specification.html
+
+
+Build and tests status
+----------------------
+
++-------+-----------------+--------------+
+|Branch | **Linux/macOS** | **Windows**  |
++=======+=================+==============+
+|Master | |master-posix|  | |master-win| |
++-------+-----------------+--------------+
+|Develop| |devel-posix|   | |devel-win|  |
++-------+-----------------+--------------+
+
+
+REQUIREMENTS
+------------
+The AboutCode Toolkit is tested with Python 3.7 or above only on Linux, Mac and Windows.
+You will need to install a Python interpreter if you do not have one already
+installed.
+
+On Linux and Mac, Python is typically pre-installed. To verify which
+version may be pre-installed, open a terminal and type:
+
+    python --version
+
+Note
+~~~~
+    Debian has decided that distutils is not a core python package, so it is not included in the last versions of debian and debian-based OSes.
+    A solution is to run: `sudo apt install python3-distutils`
+
+On Windows or Mac, you can download the latest Python here:
+    https://www.python.org/downloads/
+
+Download the .msi installer for Windows or the .dmg archive for Mac.
+Open and run the installer using all the default options.
+
+INSTALLATION
+------------
+Checkout or download and extract the AboutCode Toolkit from:
+    https://github.com/nexB/aboutcode-toolkit/
+
+To install all the needed dependencies in a virtualenv, run (on posix):
+    ./configure
+or on windows:
+    configure
+
+ACTIVATE the VIRTUALENV
+-----------------------
+To activate the virtualenv, run (on posix):
+    source venv/bin/activate
+or on windows:
+    venv\\bin\\activate
+
+
+DEACTIVATE the VIRTUALENV
+-------------------------
+To deactivate the virtualenv, run (on both posix and windows):
+    deactivate
+
+
+VERSIONING SCHEMA
+-----------------
+Starting at AboutCode version 4.0.0, the AboutCode Toolkit will follow SemVer for the versioning schema.
+
+i.e. MAJOR.MINOR.PATCH format
+    1. MAJOR version when making incompatible API changes,
+    2. MINOR version when making functionality in a backwards compatible manner, and
+    3. PATCH version when making backwards compatible bug fixes.
+
+
+REFERENCE
+---------
+See https://aboutcode-toolkit.readthedocs.io/en/latest/ for documentation.
+
+See https://aboutcode-toolkit.readthedocs.io/en/latest/reference.html for reference.
+
+TESTS and DEVELOPMENT
+---------------------
+To install all the needed development dependencies, run (on posix):
+    ./configure --dev
+or on windows:
+    configure --dev
+
+To verify that everything works fine you can run the test suite with:
+    pytest
+
+
+CLEAN BUILD AND INSTALLED FILES
+-------------------------------
+To clean the built and installed files, run (on posix):
+    ./configure --clean
+or on windows:
+    configure --clean
+
+
+HELP and SUPPORT
+----------------
+If you have a question or find a bug, enter a ticket at:
+
+    https://github.com/nexB/aboutcode-toolkit
+
+For issues, you can use:
+
+    https://github.com/nexB/aboutcode-toolkit/issues
+
+
+SOURCE CODE
+-----------
+The AboutCode Toolkit is available through GitHub. For the latest version visit:
+    https://github.com/nexB/aboutcode-toolkit
+
+
+HACKING
+-------
+We accept pull requests provided under the same license as this tool.
+You agree to the http://developercertificate.org/
+
+
+LICENSE
+-------
+The AboutCode Toolkit is released under the Apache 2.0 license.
+See (of course) the about.ABOUT file for details.
+
+
+.. |master-posix| image:: https://api.travis-ci.org/nexB/aboutcode-toolkit.png?branch=master
+    :target: https://travis-ci.org/nexB/aboutcode-toolkit
+    :alt: Linux Master branch tests status
+.. |devel-posix| image:: https://api.travis-ci.org/nexB/aboutcode-toolkit.png?branch=develop
+    :target: https://travis-ci.org/nexB/aboutcode-toolkit
+    :alt: Linux Develop branch tests status
+
+.. |master-win| image:: https://ci.appveyor.com/api/projects/status/uwj2gh8i9ga1mqwn/branch/master?png=true
+    :target: https://ci.appveyor.com/project/nexB/aboutcode-toolkit
+    :alt: Windows Master branch tests status
+.. |devel-win| image:: https://ci.appveyor.com/api/projects/status/uwj2gh8i9ga1mqwn/branch/develop?png=true
+    :target: https://ci.appveyor.com/project/nexB/aboutcode-toolkit
+    :alt: Windows Develop branch tests status
```

### Comparing `aboutcode-toolkit-8.0.0/README.rst` & `aboutcode-toolkit-9.0.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 The current version of the AboutCode Toolkit can read these ABOUT files so that you
 can collect and validate the inventory of third-party components that you use.
 
 In addition, this tool is able to generate attribution notices and
 identify redistributable source code used in your project to help you comply
 with open source licenses conditions.
 
-This version of the AboutCode Toolkit follows the ABOUT specification version 3.3.0 at:
+This version of the AboutCode Toolkit follows the ABOUT specification version 3.3.1 at:
 https://aboutcode-toolkit.readthedocs.io/en/latest/specification.html
 
 
 Build and tests status
 ----------------------
 
 +-------+-----------------+--------------+
```

### Comparing `aboutcode-toolkit-8.0.0/about` & `aboutcode-toolkit-9.0.0/about`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/about.ABOUT` & `aboutcode-toolkit-9.0.0/about.ABOUT`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 about_resource: .
 name: AboutCode-toolkit
-version: 8.0.0
+version: 9.0.0
 author: Jillian Daguil, Chin Yeung Li, Philippe Ombredanne, Thomas Druez
 copyright: Copyright (c) nexB Inc.
 description: |
     AboutCode Toolkit is a tool to process ABOUT files. An ABOUT file
     provides a simple way to document the provenance (origin and license)
     'about' a software component. This is a small text file stored in the
     codebase side-by-side with the documented software component.
```

### Comparing `aboutcode-toolkit-8.0.0/about.bat` & `aboutcode-toolkit-9.0.0/about.bat`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/apache-2.0.LICENSE` & `aboutcode-toolkit-9.0.0/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/appveyor.yml` & `aboutcode-toolkit-9.0.0/appveyor.yml`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/azure-pipelines.yml` & `aboutcode-toolkit-9.0.0/azure-pipelines.yml`

 * *Files 9% similar despite different names*

```diff
@@ -5,22 +5,14 @@
 # These jobs are using VMs with Azure-provided Python builds
 ################################################################################
 
 jobs:
 
     - template: etc/ci/azure-posix.yml
       parameters:
-          job_name: ubuntu18_cpython
-          image_name: ubuntu-18.04
-          python_versions: ['3.7', '3.8', '3.9', '3.10', '3.11']
-          test_suites:
-              all: venv/bin/pytest -n 2 -vvs
-
-    - template: etc/ci/azure-posix.yml
-      parameters:
           job_name: ubuntu20_cpython
           image_name: ubuntu-20.04
           python_versions: ['3.7', '3.8', '3.9', '3.10', '3.11']
           test_suites:
               all: venv/bin/pytest -n 2 -vvs
 
     - template: etc/ci/azure-posix.yml
@@ -29,22 +21,14 @@
           image_name: ubuntu-22.04
           python_versions: ['3.7', '3.8', '3.9', '3.10', '3.11']
           test_suites:
               all: venv/bin/pytest -n 2 -vvs
 
     - template: etc/ci/azure-posix.yml
       parameters:
-          job_name: macos1015_cpython_2
-          image_name: macos-10.15
-          python_versions: ['3.7', '3.8', '3.9', '3.10', '3.11']
-          test_suites:
-              all: venv/bin/pytest -n 2 -vvs
-
-    - template: etc/ci/azure-posix.yml
-      parameters:
           job_name: macos11_cpython
           image_name: macos-11
           python_versions: ['3.7', '3.8', '3.9', '3.10', '3.11']
           test_suites:
               all: venv/bin/pytest -n 2 -vvs
 
     - template: etc/ci/azure-posix.yml
```

### Comparing `aboutcode-toolkit-8.0.0/configure` & `aboutcode-toolkit-9.0.0/configure`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/configure.bat` & `aboutcode-toolkit-9.0.0/configure.bat`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/docs/Makefile` & `aboutcode-toolkit-9.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/docs/make.bat` & `aboutcode-toolkit-9.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/docs/source/_static/theme_overrides.css` & `aboutcode-toolkit-9.0.0/docs/source/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/docs/source/general.rst` & `aboutcode-toolkit-9.0.0/docs/source/general.rst`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,17 @@
       - Notes
     * - about_resource
       - Name/path of the component resource
       - Mandatory
     * - name
       - Component name
       - Mandatory
+    * - ignored_resources
+      - List of paths ignored from the ``about_resource``
+      - Optional
     * - version
       - Component version
       - Optional
     * - download_url
       - Direct URL to download the original file or archive documented by this ABOUT file
       - Optional
     * - description
@@ -315,15 +318,15 @@
 
 Prepare an Attribution Template to Use
 --------------------------------------
 
 You can run attrib using the default_html.template (or default_json.template)
 provided with the AboutCode Toolkit tools:
 
-https://github.com/nexB/aboutcode-toolkit/blob/develop/templates/default_html.template
+https://github.com/nexB/aboutcode-toolkit/blob/develop/src/attributecode/templates/default_html.template
 
 If you choose to do that, you will most likely want to edit the generated .html
 file to provide header information about your own organization and product.
 
 Running attrib with the default_html.template file is probably your best choice when
 you are still testing your AboutCode Toolkit process. Once you have a good understanding
 of the generated output, you can customize the template to provide the standard text that
```

### Comparing `aboutcode-toolkit-8.0.0/docs/source/home.rst` & `aboutcode-toolkit-9.0.0/docs/source/home.rst`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 The current version of the AboutCode Toolkit can read these ABOUT files so that you
 can collect and validate the inventory of third-party components that you use.
 
 In addition, this tool is able to generate attribution notices and
 identify redistributable source code used in your project to help you comply
 with open source licenses conditions.
 
-This version of the AboutCode Toolkit follows the ABOUT specification version 3.3.0 at:
+This version of the AboutCode Toolkit follows the ABOUT specification version 3.3.1 at:
 https://aboutcode-toolkit.readthedocs.io/en/latest/specification.html
 
 
 Build and tests status
 ----------------------
 
 +-------+-----------------+--------------+
```

### Comparing `aboutcode-toolkit-8.0.0/docs/source/reference.rst` & `aboutcode-toolkit-9.0.0/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/docs/source/specification.rst` & `aboutcode-toolkit-9.0.0/docs/source/specification.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .. _specification:
 
 ===============================
-ABOUT File Specification v3.3.0
+ABOUT File Specification v3.3.1
 ===============================
 
 Purpose
 =======
 
 An ABOUT file provides a simple way to document the provenance (origin and license)
 and other important or interesting information about a software component.
@@ -214,19 +214,22 @@
 ``Y`` or ``x`` must be interpreted as "true" in any case combination.
 ``False``, ``F``, ``No`` or ``N`` must be interpreted as "false"
 in any case combination.
 
 Referencing the file or directory documented by an ABOUT file
 -------------------------------------------------------------
 
-An ABOUT file documents one file or directory. The mandatory "about_resource"
-field reference the documented file or directory. The value of the "about_resource"
-field is the name or path of the referenced file or directory.
+An ABOUT file documents one file or directory. The mandatory ``about_resource``
+field reference the documented file or directory. The value of the ``about_resource``
+field is the name or path of the referenced file or directory. There is also a
+``ignored_resources`` field which can be used to ignore a set of subpaths inside the
+directory which is being documented in the ABOUT file.
 
-A tool processing an ABOUT file must report an error if this field is missing.
+A tool processing an ABOUT file must report an error if the ``about_resource``
+field is missing.
 
 By convention, an ABOUT file is often stored in the same directory side-by-side
 to the file or directory that it documents, but this is not mandatory.
 
 For example, a file named django.ABOUT contains the following field to document
 the django-1.2.3.tar.gz archive stored in the same directory:
 
@@ -236,14 +239,22 @@
 
 In this example, the ABOUT file documents a whole sub-directory:
 
         ..  code-block:: none
 
                 about_resource: linux-kernel-2.6.23
 
+In this example, the ABOUT file documents a whole sub-directory, with some
+sub-paths under the directory ignored:
+
+        ..  code-block:: none
+
+                about_resource: linux-kernel-2.6.23
+                ignored_resources: linux-kernel-2.6.23/Documentation
+
 In this example, the ABOUT file documents the current directory, using a "." period to reference it:
 
         ..  code-block:: none
 
                 about_resource: .
 
 Other Mandatory fields
@@ -254,14 +265,17 @@
 
 -   about_resource: The resource this file referencing to.
 -   name: Component name.
 
 Optional Information fields
 ---------------------------
 
+-   ignored_resources: A list of paths under the ``about_resource`` path, which are
+    not documented in the ABOUT file, and the information in the ABOUT file does not
+    apply to these subpaths.
 -   version: Component or package version. A component or package usually has a version,
     such as a revision number or hash from a version control system (for a snapshot checked
     out from VCS such as Subversion or Git). If not available, the version should be the date
     the component was provisioned, in an ISO date format such as 'YYYY-MM-DD'.
 -   spec_version: The version of the ABOUT file format specification used for this file.
     This is provided as a hint to readers and tools in order to support future versions
     of this specification.
```

### Comparing `aboutcode-toolkit-8.0.0/docs/source/type_of_errors.rst` & `aboutcode-toolkit-9.0.0/docs/source/type_of_errors.rst`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/ci/azure-container-deb.yml` & `aboutcode-toolkit-9.0.0/etc/ci/azure-container-deb.yml`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/ci/azure-container-rpm.yml` & `aboutcode-toolkit-9.0.0/etc/ci/azure-container-rpm.yml`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/ci/azure-posix.yml` & `aboutcode-toolkit-9.0.0/etc/ci/azure-posix.yml`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/ci/azure-win.yml` & `aboutcode-toolkit-9.0.0/etc/ci/azure-win.yml`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/ci/macports-ci` & `aboutcode-toolkit-9.0.0/etc/ci/macports-ci`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/ci/macports-ci.ABOUT` & `aboutcode-toolkit-9.0.0/etc/ci/macports-ci.ABOUT`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/ci/mit.LICENSE` & `aboutcode-toolkit-9.0.0/etc/ci/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/scripts/README.rst` & `aboutcode-toolkit-9.0.0/etc/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/scripts/check_thirdparty.py` & `aboutcode-toolkit-9.0.0/etc/scripts/check_thirdparty.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/scripts/fetch_thirdparty.py` & `aboutcode-toolkit-9.0.0/etc/scripts/fetch_thirdparty.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/scripts/gen_pypi_simple.py` & `aboutcode-toolkit-9.0.0/etc/scripts/gen_pypi_simple.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/scripts/gen_pypi_simple.py.NOTICE` & `aboutcode-toolkit-9.0.0/etc/scripts/gen_pypi_simple.py.NOTICE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/scripts/gen_requirements.py` & `aboutcode-toolkit-9.0.0/etc/scripts/gen_requirements.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/scripts/gen_requirements_dev.py` & `aboutcode-toolkit-9.0.0/etc/scripts/gen_requirements_dev.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/scripts/test_utils_pip_compatibility_tags.py` & `aboutcode-toolkit-9.0.0/etc/scripts/test_utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/scripts/test_utils_pypi_supported_tags.py` & `aboutcode-toolkit-9.0.0/etc/scripts/test_utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT` & `aboutcode-toolkit-9.0.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/scripts/utils_dejacode.py` & `aboutcode-toolkit-9.0.0/etc/scripts/utils_dejacode.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/scripts/utils_pip_compatibility_tags.py` & `aboutcode-toolkit-9.0.0/etc/scripts/utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/scripts/utils_pypi_supported_tags.py` & `aboutcode-toolkit-9.0.0/etc/scripts/utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT` & `aboutcode-toolkit-9.0.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/scripts/utils_requirements.py` & `aboutcode-toolkit-9.0.0/etc/scripts/utils_requirements.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/scripts/utils_thirdparty.py` & `aboutcode-toolkit-9.0.0/etc/scripts/utils_thirdparty.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/etc/scripts/utils_thirdparty.py.ABOUT` & `aboutcode-toolkit-9.0.0/etc/scripts/utils_thirdparty.py.ABOUT`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/config/config.guess.ABOUT` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/config/config.guess.ABOUT`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/config/config.sub.ABOUT` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/config/config.sub.ABOUT`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/config/gpl-2.0-autoconf.LICENSE` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/config/gpl-2.0-autoconf.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/KazKylheku.LICENSE` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/KazKylheku.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/gpl-2.0.LICENSE` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/gpl-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/lgpl-2.0.LICENSE` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/lgpl-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/mtrace.c.ABOUT` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsck/mtrace.c.ABOUT`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsprogs-1.39.NOTICE` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/e2fsprogs-1.39.NOTICE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/gpl-2.0.LICENSE` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/gpl-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/include/nonunix/getopt.h.ABOUT` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/include/nonunix/getopt.h.ABOUT`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/include/nonunix/lgpl-2.0.LICENSE` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/include/nonunix/lgpl-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/intl/lgpl-2.0.LICENSE` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/intl/lgpl-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/blkid/lgpl-2.1.LICENSE` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/blkid/lgpl-2.1.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/bsla.LICENSE` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/bsla.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/e2p/lgpl-2.0.LICENSE` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/e2p/lgpl-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/bsd-new.LICENSE` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/bsd-new.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/bsla.LICENSE` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/bsla.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/gpl-2.0.LICENSE` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/gpl-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/kerberos.LICENSE` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/et/kerberos.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/ss/kerberos.LICENSE` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/ss/kerberos.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/uuid/bsd-new.LICENSE` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/lib/uuid/bsd-new.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/misc/lgpl-2.1.LICENSE` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/e2fsprogs-about/e2fsprogs-1.39/misc/lgpl-2.1.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/input/MAPPING.CONFIG` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/input/MAPPING.CONFIG`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/input/e2fsprogs-1.39-CreateAboutFile.csv` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/input/e2fsprogs-1.39-CreateAboutFile.csv`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/input/e2fsprogs-1.39-INV.xlsx` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/input/e2fsprogs-1.39-INV.xlsx`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/input/template_sample_attribution_starship.html` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/input/template_sample_attribution_starship.html`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/example/e2fsprogs-1.39/output/sample_attribution_starship.html` & `aboutcode-toolkit-9.0.0/example/e2fsprogs-1.39/output/sample_attribution_starship.html`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/pyproject.toml` & `aboutcode-toolkit-9.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/requirements.txt` & `aboutcode-toolkit-9.0.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/setup.cfg` & `aboutcode-toolkit-9.0.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,117 +1,113 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2061 626f 7574 636f 6465 2d74 6f6f   = aboutcode-too
-00000020: 6c6b 6974 0d0a 6c69 6365 6e73 6520 3d20  lkit..license = 
-00000030: 4170 6163 6865 2d32 2e30 0d0a 6465 7363  Apache-2.0..desc
-00000040: 7269 7074 696f 6e20 3d20 4162 6f75 7443  ription = AboutC
-00000050: 6f64 652d 746f 6f6c 6b69 7420 6973 2061  ode-toolkit is a
-00000060: 2074 6f6f 6c20 746f 2064 6f63 756d 656e   tool to documen
-00000070: 7420 7468 6520 7072 6f76 656e 616e 6365  t the provenance
-00000080: 2028 6f72 6967 696e 2061 6e64 206c 6963   (origin and lic
-00000090: 656e 7365 2920 6f66 2074 6869 7264 2d70  ense) of third-p
-000000a0: 6172 7479 2073 6f66 7477 6172 6520 7573  arty software us
-000000b0: 696e 6720 736d 616c 6c20 7465 7874 2066  ing small text f
-000000c0: 696c 6573 2e20 436f 6c6c 6563 7420 696e  iles. Collect in
-000000d0: 7665 6e74 6f72 6965 7320 616e 6420 6765  ventories and ge
-000000e0: 6e65 7261 7465 2061 7474 7269 6275 7469  nerate attributi
-000000f0: 6f6e 2064 6f63 756d 656e 7461 7469 6f6e  on documentation
-00000100: 2e0d 0a6c 6f6e 675f 6465 7363 7269 7074  ...long_descript
-00000110: 696f 6e20 3d20 6669 6c65 3a52 4541 444d  ion = file:READM
-00000120: 452e 7273 740d 0a6c 6f6e 675f 6465 7363  E.rst..long_desc
-00000130: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
-00000140: 7479 7065 203d 2074 6578 742f 782d 7273  type = text/x-rs
-00000150: 740d 0a75 726c 203d 2068 7474 7073 3a2f  t..url = https:/
-00000160: 2f67 6974 6875 622e 636f 6d2f 6e65 7842  /github.com/nexB
-00000170: 2f61 626f 7574 636f 6465 2d74 6f6f 6c6b  /aboutcode-toolk
-00000180: 6974 0d0a 6175 7468 6f72 203d 206e 6578  it..author = nex
-00000190: 422e 2049 6e63 2e20 616e 6420 6f74 6865  B. Inc. and othe
-000001a0: 7273 0d0a 6175 7468 6f72 5f65 6d61 696c  rs..author_email
-000001b0: 203d 2069 6e66 6f40 6162 6f75 7463 6f64   = info@aboutcod
-000001c0: 652e 6f72 670d 0a63 6c61 7373 6966 6965  e.org..classifie
-000001d0: 7273 203d 200d 0a09 4465 7665 6c6f 706d  rs = ...Developm
-000001e0: 656e 7420 5374 6174 7573 203a 3a20 3520  ent Status :: 5 
-000001f0: 2d20 5072 6f64 7563 7469 6f6e 2f53 7461  - Production/Sta
-00000200: 626c 650d 0a09 496e 7465 6e64 6564 2041  ble...Intended A
-00000210: 7564 6965 6e63 6520 3a3a 2044 6576 656c  udience :: Devel
-00000220: 6f70 6572 730d 0a09 5072 6f67 7261 6d6d  opers...Programm
-00000230: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000240: 5079 7468 6f6e 203a 3a20 3320 3a3a 204f  Python :: 3 :: O
-00000250: 6e6c 790d 0a09 5072 6f67 7261 6d6d 696e  nly...Programmin
-00000260: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000270: 7468 6f6e 203a 3a20 332e 370d 0a09 5072  thon :: 3.7...Pr
-00000280: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000290: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000002a0: 332e 380d 0a09 5072 6f67 7261 6d6d 696e  3.8...Programmin
-000002b0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000002c0: 7468 6f6e 203a 3a20 332e 390d 0a09 5072  thon :: 3.9...Pr
-000002d0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000002e0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000002f0: 332e 3130 0d0a 0954 6f70 6963 203a 3a20  3.10...Topic :: 
-00000300: 536f 6674 7761 7265 2044 6576 656c 6f70  Software Develop
-00000310: 6d65 6e74 0d0a 0954 6f70 6963 203a 3a20  ment...Topic :: 
-00000320: 536f 6674 7761 7265 2044 6576 656c 6f70  Software Develop
-00000330: 6d65 6e74 203a 3a20 446f 6375 6d65 6e74  ment :: Document
-00000340: 6174 696f 6e0d 0a09 546f 7069 6320 3a3a  ation...Topic ::
-00000350: 2053 6f66 7477 6172 6520 4465 7665 6c6f   Software Develo
-00000360: 706d 656e 7420 3a3a 2051 7561 6c69 7479  pment :: Quality
-00000370: 2041 7373 7572 616e 6365 0d0a 0954 6f70   Assurance...Top
-00000380: 6963 203a 3a20 5379 7374 656d 203a 3a20  ic :: System :: 
-00000390: 536f 6674 7761 7265 2044 6973 7472 6962  Software Distrib
-000003a0: 7574 696f 6e0d 0a09 546f 7069 6320 3a3a  ution...Topic ::
-000003b0: 2055 7469 6c69 7469 6573 0d0a 6b65 7977   Utilities..keyw
-000003c0: 6f72 6473 203d 200d 0a09 6c69 6365 6e73  ords = ...licens
-000003d0: 650d 0a09 6162 6f75 740d 0a09 6d65 7461  e...about...meta
-000003e0: 6461 7461 0d0a 0970 6163 6b61 6765 0d0a  data...package..
-000003f0: 0963 6f70 7972 6967 6874 0d0a 0961 7474  .copyright...att
-00000400: 7269 6275 7469 6f6e 0d0a 0973 6f66 7477  ribution...softw
-00000410: 6172 650d 0a09 696e 7665 6e74 6f72 790d  are...inventory.
-00000420: 0a09 6f70 656e 2073 6f75 7263 650d 0a09  ..open source...
-00000430: 7363 610d 0a09 5342 4f4d 0d0a 0973 7064  sca...SBOM...spd
-00000440: 780d 0a6c 6963 656e 7365 5f66 696c 6573  x..license_files
-00000450: 203d 200d 0a09 6170 6163 6865 2d32 2e30   = ...apache-2.0
-00000460: 2e4c 4943 454e 5345 0d0a 094e 4f54 4943  .LICENSE...NOTIC
-00000470: 450d 0a09 4155 5448 4f52 532e 7273 740d  E...AUTHORS.rst.
-00000480: 0a09 4348 414e 4745 4c4f 472e 7273 740d  ..CHANGELOG.rst.
-00000490: 0a09 434f 4445 5f4f 465f 434f 4e44 5543  ..CODE_OF_CONDUC
-000004a0: 542e 7273 740d 0a0d 0a5b 6f70 7469 6f6e  T.rst....[option
-000004b0: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
-000004c0: 3d20 0d0a 093d 7372 630d 0a70 6163 6b61  = ...=src..packa
-000004d0: 6765 7320 3d20 6669 6e64 3a0d 0a69 6e63  ges = find:..inc
-000004e0: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
-000004f0: 6120 3d20 7472 7565 0d0a 7a69 705f 7361  a = true..zip_sa
-00000500: 6665 203d 2066 616c 7365 0d0a 7365 7475  fe = false..setu
-00000510: 705f 7265 7175 6972 6573 203d 2073 6574  p_requires = set
-00000520: 7570 746f 6f6c 735f 7363 6d5b 746f 6d6c  uptools_scm[toml
-00000530: 5d20 3e3d 2034 0d0a 7079 7468 6f6e 5f72  ] >= 4..python_r
-00000540: 6571 7569 7265 7320 3d20 3e3d 332e 370d  equires = >=3.7.
-00000550: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-00000560: 7320 3d20 0d0a 0961 7474 7273 0d0a 0962  s = ...attrs...b
-00000570: 6f6f 6c65 616e 2e70 7920 3e3d 2033 2e35  oolean.py >= 3.5
-00000580: 0d0a 0963 6572 7469 6669 0d0a 0963 6c69  ...certifi...cli
-00000590: 636b 0d0a 096a 696e 6a61 320d 0a09 6c69  ck...jinja2...li
-000005a0: 6365 6e73 655f 6578 7072 6573 7369 6f6e  cense_expression
-000005b0: 203e 3d20 302e 3934 0d0a 096f 7065 6e70   >= 0.94...openp
-000005c0: 7978 6c0d 0a09 7061 636b 6167 6575 726c  yxl...packageurl
-000005d0: 5f70 7974 686f 6e20 3e3d 2030 2e39 2e30  _python >= 0.9.0
-000005e0: 0d0a 0973 616e 6579 616d 6c0d 0a0d 0a5b  ...saneyaml....[
-000005f0: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
-00000600: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
-00000610: 7372 630d 0a0d 0a5b 6f70 7469 6f6e 732e  src....[options.
-00000620: 6578 7472 6173 5f72 6571 7569 7265 5d0d  extras_require].
-00000630: 0a74 6573 7469 6e67 203d 200d 0a09 7079  .testing = ...py
-00000640: 7465 7374 203e 3d20 362c 2021 3d20 372e  test >= 6, != 7.
-00000650: 302e 300d 0a09 7079 7465 7374 2d78 6469  0.0...pytest-xdi
-00000660: 7374 203e 3d20 320d 0a09 7477 696e 650d  st >= 2...twine.
-00000670: 0a09 626c 6163 6b0d 0a09 6973 6f72 740d  ..black...isort.
-00000680: 0a64 6f63 7320 3d20 0d0a 0953 7068 696e  .docs = ...Sphin
-00000690: 7820 3e3d 2033 2e33 2e31 0d0a 0973 7068  x >= 3.3.1...sph
-000006a0: 696e 782d 7274 642d 7468 656d 6520 3e3d  inx-rtd-theme >=
-000006b0: 2030 2e35 2e30 0d0a 0964 6f63 3820 3e3d   0.5.0...doc8 >=
-000006c0: 2030 2e38 2e31 0d0a 0d0a 5b6f 7074 696f   0.8.1....[optio
-000006d0: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
-000006e0: 0d0a 636f 6e73 6f6c 655f 7363 7269 7074  ..console_script
-000006f0: 7320 3d20 0d0a 0961 626f 7574 3d61 7474  s = ...about=att
-00000700: 7269 6275 7465 636f 6465 2e63 6d64 3a61  ributecode.cmd:a
-00000710: 626f 7574 0d0a 0d0a 5b65 6767 5f69 6e66  bout....[egg_inf
-00000720: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000730: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-00000740: 0d0a                                     ..
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6162 6f75 7463 6f64 652d 746f 6f6c  = aboutcode-tool
+00000020: 6b69 740a 6c69 6365 6e73 6520 3d20 4170  kit.license = Ap
+00000030: 6163 6865 2d32 2e30 0a64 6573 6372 6970  ache-2.0.descrip
+00000040: 7469 6f6e 203d 2041 626f 7574 436f 6465  tion = AboutCode
+00000050: 2d74 6f6f 6c6b 6974 2069 7320 6120 746f  -toolkit is a to
+00000060: 6f6c 2074 6f20 646f 6375 6d65 6e74 2074  ol to document t
+00000070: 6865 2070 726f 7665 6e61 6e63 6520 286f  he provenance (o
+00000080: 7269 6769 6e20 616e 6420 6c69 6365 6e73  rigin and licens
+00000090: 6529 206f 6620 7468 6972 642d 7061 7274  e) of third-part
+000000a0: 7920 736f 6674 7761 7265 2075 7369 6e67  y software using
+000000b0: 2073 6d61 6c6c 2074 6578 7420 6669 6c65   small text file
+000000c0: 732e 2043 6f6c 6c65 6374 2069 6e76 656e  s. Collect inven
+000000d0: 746f 7269 6573 2061 6e64 2067 656e 6572  tories and gener
+000000e0: 6174 6520 6174 7472 6962 7574 696f 6e20  ate attribution 
+000000f0: 646f 6375 6d65 6e74 6174 696f 6e2e 0a6c  documentation..l
+00000100: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
+00000110: 3d20 6669 6c65 3a52 4541 444d 452e 7273  = file:README.rs
+00000120: 740a 6c6f 6e67 5f64 6573 6372 6970 7469  t.long_descripti
+00000130: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
+00000140: 3d20 7465 7874 2f78 2d72 7374 0a75 726c  = text/x-rst.url
+00000150: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
+00000160: 622e 636f 6d2f 6e65 7842 2f61 626f 7574  b.com/nexB/about
+00000170: 636f 6465 2d74 6f6f 6c6b 6974 0a61 7574  code-toolkit.aut
+00000180: 686f 7220 3d20 6e65 7842 2e20 496e 632e  hor = nexB. Inc.
+00000190: 2061 6e64 206f 7468 6572 730a 6175 7468   and others.auth
+000001a0: 6f72 5f65 6d61 696c 203d 2069 6e66 6f40  or_email = info@
+000001b0: 6162 6f75 7463 6f64 652e 6f72 670a 636c  aboutcode.org.cl
+000001c0: 6173 7369 6669 6572 7320 3d20 0a09 4465  assifiers = ..De
+000001d0: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
+000001e0: 203a 3a20 3520 2d20 5072 6f64 7563 7469   :: 5 - Producti
+000001f0: 6f6e 2f53 7461 626c 650a 0949 6e74 656e  on/Stable..Inten
+00000200: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
+00000210: 4465 7665 6c6f 7065 7273 0a09 5072 6f67  Developers..Prog
+00000220: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000230: 203a 3a20 5079 7468 6f6e 203a 3a20 3320   :: Python :: 3 
+00000240: 3a3a 204f 6e6c 790a 0950 726f 6772 616d  :: Only..Program
+00000250: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000260: 2050 7974 686f 6e20 3a3a 2033 2e37 0a09   Python :: 3.7..
+00000270: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000280: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000290: 3a20 332e 380a 0950 726f 6772 616d 6d69  : 3.8..Programmi
+000002a0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000002b0: 7974 686f 6e20 3a3a 2033 2e39 0a09 5072  ython :: 3.9..Pr
+000002c0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000002d0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000002e0: 332e 3130 0a09 546f 7069 6320 3a3a 2053  3.10..Topic :: S
+000002f0: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
+00000300: 656e 740a 0954 6f70 6963 203a 3a20 536f  ent..Topic :: So
+00000310: 6674 7761 7265 2044 6576 656c 6f70 6d65  ftware Developme
+00000320: 6e74 203a 3a20 446f 6375 6d65 6e74 6174  nt :: Documentat
+00000330: 696f 6e0a 0954 6f70 6963 203a 3a20 536f  ion..Topic :: So
+00000340: 6674 7761 7265 2044 6576 656c 6f70 6d65  ftware Developme
+00000350: 6e74 203a 3a20 5175 616c 6974 7920 4173  nt :: Quality As
+00000360: 7375 7261 6e63 650a 0954 6f70 6963 203a  surance..Topic :
+00000370: 3a20 5379 7374 656d 203a 3a20 536f 6674  : System :: Soft
+00000380: 7761 7265 2044 6973 7472 6962 7574 696f  ware Distributio
+00000390: 6e0a 0954 6f70 6963 203a 3a20 5574 696c  n..Topic :: Util
+000003a0: 6974 6965 730a 6b65 7977 6f72 6473 203d  ities.keywords =
+000003b0: 200a 096c 6963 656e 7365 0a09 6162 6f75   ..license..abou
+000003c0: 740a 096d 6574 6164 6174 610a 0970 6163  t..metadata..pac
+000003d0: 6b61 6765 0a09 636f 7079 7269 6768 740a  kage..copyright.
+000003e0: 0961 7474 7269 6275 7469 6f6e 0a09 736f  .attribution..so
+000003f0: 6674 7761 7265 0a09 696e 7665 6e74 6f72  ftware..inventor
+00000400: 790a 096f 7065 6e20 736f 7572 6365 0a09  y..open source..
+00000410: 7363 610a 0953 424f 4d0a 0973 7064 780a  sca..SBOM..spdx.
+00000420: 6c69 6365 6e73 655f 6669 6c65 7320 3d20  license_files = 
+00000430: 0a09 6170 6163 6865 2d32 2e30 2e4c 4943  ..apache-2.0.LIC
+00000440: 454e 5345 0a09 4e4f 5449 4345 0a09 4155  ENSE..NOTICE..AU
+00000450: 5448 4f52 532e 7273 740a 0943 4841 4e47  THORS.rst..CHANG
+00000460: 454c 4f47 2e72 7374 0a09 434f 4445 5f4f  ELOG.rst..CODE_O
+00000470: 465f 434f 4e44 5543 542e 7273 740a 0a5b  F_CONDUCT.rst..[
+00000480: 6f70 7469 6f6e 735d 0a70 6163 6b61 6765  options].package
+00000490: 5f64 6972 203d 200a 093d 7372 630a 7061  _dir = ..=src.pa
+000004a0: 636b 6167 6573 203d 2066 696e 643a 0a69  ckages = find:.i
+000004b0: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
+000004c0: 6174 6120 3d20 7472 7565 0a7a 6970 5f73  ata = true.zip_s
+000004d0: 6166 6520 3d20 6661 6c73 650a 7365 7475  afe = false.setu
+000004e0: 705f 7265 7175 6972 6573 203d 2073 6574  p_requires = set
+000004f0: 7570 746f 6f6c 735f 7363 6d5b 746f 6d6c  uptools_scm[toml
+00000500: 5d20 3e3d 2034 0a70 7974 686f 6e5f 7265  ] >= 4.python_re
+00000510: 7175 6972 6573 203d 203e 3d33 2e37 0a69  quires = >=3.7.i
+00000520: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
+00000530: 3d20 0a09 6174 7472 730a 0962 6f6f 6c65  = ..attrs..boole
+00000540: 616e 2e70 7920 3e3d 2033 2e35 0a09 6365  an.py >= 3.5..ce
+00000550: 7274 6966 690a 0963 6c69 636b 0a09 6a69  rtifi..click..ji
+00000560: 6e6a 6132 0a09 6c69 6365 6e73 655f 6578  nja2..license_ex
+00000570: 7072 6573 7369 6f6e 203e 3d20 302e 3934  pression >= 0.94
+00000580: 0a09 6f70 656e 7079 786c 0a09 7061 636b  ..openpyxl..pack
+00000590: 6167 6575 726c 5f70 7974 686f 6e20 3e3d  ageurl_python >=
+000005a0: 2030 2e39 2e30 0a09 7361 6e65 7961 6d6c   0.9.0..saneyaml
+000005b0: 0a0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+000005c0: 6765 732e 6669 6e64 5d0a 7768 6572 6520  ges.find].where 
+000005d0: 3d20 7372 630a 0a5b 6f70 7469 6f6e 732e  = src..[options.
+000005e0: 6578 7472 6173 5f72 6571 7569 7265 5d0a  extras_require].
+000005f0: 7465 7374 696e 6720 3d20 0a09 7079 7465  testing = ..pyte
+00000600: 7374 203e 3d20 362c 2021 3d20 372e 302e  st >= 6, != 7.0.
+00000610: 300a 0970 7974 6573 742d 7864 6973 7420  0..pytest-xdist 
+00000620: 3e3d 2032 0a09 7477 696e 650a 0962 6c61  >= 2..twine..bla
+00000630: 636b 0a09 6973 6f72 740a 646f 6373 203d  ck..isort.docs =
+00000640: 200a 0953 7068 696e 783e 3d35 2e30 2e32   ..Sphinx>=5.0.2
+00000650: 0a09 7370 6869 6e78 2d72 7464 2d74 6865  ..sphinx-rtd-the
+00000660: 6d65 3e3d 312e 302e 300a 0973 7068 696e  me>=1.0.0..sphin
+00000670: 782d 7265 7265 6469 7265 6374 7320 3e3d  x-reredirects >=
+00000680: 2030 2e31 2e32 0a09 646f 6338 3e3d 302e   0.1.2..doc8>=0.
+00000690: 3131 2e32 0a0a 5b6f 7074 696f 6e73 2e65  11.2..[options.e
+000006a0: 6e74 7279 5f70 6f69 6e74 735d 0a63 6f6e  ntry_points].con
+000006b0: 736f 6c65 5f73 6372 6970 7473 203d 200a  sole_scripts = .
+000006c0: 0961 626f 7574 3d61 7474 7269 6275 7465  .about=attribute
+000006d0: 636f 6465 2e63 6d64 3a61 626f 7574 0a0a  code.cmd:about..
+000006e0: 5b65 6767 5f69 6e66 6f5d 0a74 6167 5f62  [egg_info].tag_b
+000006f0: 7569 6c64 203d 200a 7461 675f 6461 7465  uild = .tag_date
+00000700: 203d 2030 0a0a                            = 0..
```

### Comparing `aboutcode-toolkit-8.0.0/src/aboutcode_toolkit.egg-info/PKG-INFO` & `aboutcode-toolkit-9.0.0/src/aboutcode_toolkit.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,193 +1,193 @@
-Metadata-Version: 2.1
-Name: aboutcode-toolkit
-Version: 8.0.0
-Summary: AboutCode-toolkit is a tool to document the provenance (origin and license) of third-party software using small text files. Collect inventories and generate attribution documentation.
-Home-page: https://github.com/nexB/aboutcode-toolkit
-Author: nexB. Inc. and others
-Author-email: info@aboutcode.org
-License: Apache-2.0
-Keywords: license,about,metadata,package,copyright,attribution,software,inventory,open source,sca,SBOM,spdx
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Documentation
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: Topic :: System :: Software Distribution
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: testing
-Provides-Extra: docs
-License-File: apache-2.0.LICENSE
-License-File: NOTICE
-License-File: AUTHORS.rst
-License-File: CHANGELOG.rst
-License-File: CODE_OF_CONDUCT.rst
-
-=================
-AboutCode Toolkit
-=================
-
-Introduction
-------------
-The AboutCode Toolkit and ABOUT files provide a simple way to document the
-origin, license, usage and other important or interesting information about
-third-party software components that you use in your project.
-
-You start by storing ABOUT files (a small YAML formatted text file with field/value pairs)
-side-by-side with each of the third-party software components you use.
-Each ABOUT file documents origin and license for one software.
-There are many examples of ABOUT files (valid or invalid) in the testdata/
-directory of the whole repository.
-
-The current version of the AboutCode Toolkit can read these ABOUT files so that you
-can collect and validate the inventory of third-party components that you use.
-
-In addition, this tool is able to generate attribution notices and
-identify redistributable source code used in your project to help you comply
-with open source licenses conditions.
-
-This version of the AboutCode Toolkit follows the ABOUT specification version 3.3.0 at:
-https://aboutcode-toolkit.readthedocs.io/en/latest/specification.html
-
-
-Build and tests status
-----------------------
-
-+-------+-----------------+--------------+
-|Branch | **Linux/macOS** | **Windows**  |
-+=======+=================+==============+
-|Master | |master-posix|  | |master-win| |
-+-------+-----------------+--------------+
-|Develop| |devel-posix|   | |devel-win|  |
-+-------+-----------------+--------------+
-
-
-REQUIREMENTS
-------------
-The AboutCode Toolkit is tested with Python 3.7 or above only on Linux, Mac and Windows.
-You will need to install a Python interpreter if you do not have one already
-installed.
-
-On Linux and Mac, Python is typically pre-installed. To verify which
-version may be pre-installed, open a terminal and type:
-
-    python --version
-
-Note
-~~~~
-    Debian has decided that distutils is not a core python package, so it is not included in the last versions of debian and debian-based OSes.
-    A solution is to run: `sudo apt install python3-distutils`
-
-On Windows or Mac, you can download the latest Python here:
-    https://www.python.org/downloads/
-
-Download the .msi installer for Windows or the .dmg archive for Mac.
-Open and run the installer using all the default options.
-
-INSTALLATION
-------------
-Checkout or download and extract the AboutCode Toolkit from:
-    https://github.com/nexB/aboutcode-toolkit/
-
-To install all the needed dependencies in a virtualenv, run (on posix):
-    ./configure
-or on windows:
-    configure
-
-ACTIVATE the VIRTUALENV
------------------------
-To activate the virtualenv, run (on posix):
-    source venv/bin/activate
-or on windows:
-    venv\\bin\\activate
-
-
-DEACTIVATE the VIRTUALENV
--------------------------
-To deactivate the virtualenv, run (on both posix and windows):
-    deactivate
-
-
-VERSIONING SCHEMA
------------------
-Starting at AboutCode version 4.0.0, the AboutCode Toolkit will follow SemVer for the versioning schema.
-
-i.e. MAJOR.MINOR.PATCH format
-    1. MAJOR version when making incompatible API changes,
-    2. MINOR version when making functionality in a backwards compatible manner, and
-    3. PATCH version when making backwards compatible bug fixes.
-
-
-REFERENCE
----------
-See https://aboutcode-toolkit.readthedocs.io/en/latest/ for documentation.
-
-See https://aboutcode-toolkit.readthedocs.io/en/latest/reference.html for reference.
-
-TESTS and DEVELOPMENT
----------------------
-To install all the needed development dependencies, run (on posix):
-    ./configure --dev
-or on windows:
-    configure --dev
-
-To verify that everything works fine you can run the test suite with:
-    pytest
-
-
-CLEAN BUILD AND INSTALLED FILES
--------------------------------
-To clean the built and installed files, run (on posix):
-    ./configure --clean
-or on windows:
-    configure --clean
-
-
-HELP and SUPPORT
-----------------
-If you have a question or find a bug, enter a ticket at:
-
-    https://github.com/nexB/aboutcode-toolkit
-
-For issues, you can use:
-
-    https://github.com/nexB/aboutcode-toolkit/issues
-
-
-SOURCE CODE
------------
-The AboutCode Toolkit is available through GitHub. For the latest version visit:
-    https://github.com/nexB/aboutcode-toolkit
-
-
-HACKING
--------
-We accept pull requests provided under the same license as this tool.
-You agree to the http://developercertificate.org/
-
-
-LICENSE
--------
-The AboutCode Toolkit is released under the Apache 2.0 license.
-See (of course) the about.ABOUT file for details.
-
-
-.. |master-posix| image:: https://api.travis-ci.org/nexB/aboutcode-toolkit.png?branch=master
-    :target: https://travis-ci.org/nexB/aboutcode-toolkit
-    :alt: Linux Master branch tests status
-.. |devel-posix| image:: https://api.travis-ci.org/nexB/aboutcode-toolkit.png?branch=develop
-    :target: https://travis-ci.org/nexB/aboutcode-toolkit
-    :alt: Linux Develop branch tests status
-
-.. |master-win| image:: https://ci.appveyor.com/api/projects/status/uwj2gh8i9ga1mqwn/branch/master?png=true
-    :target: https://ci.appveyor.com/project/nexB/aboutcode-toolkit
-    :alt: Windows Master branch tests status
-.. |devel-win| image:: https://ci.appveyor.com/api/projects/status/uwj2gh8i9ga1mqwn/branch/develop?png=true
-    :target: https://ci.appveyor.com/project/nexB/aboutcode-toolkit
-    :alt: Windows Develop branch tests status
+Metadata-Version: 2.1
+Name: aboutcode-toolkit
+Version: 9.0.0
+Summary: AboutCode-toolkit is a tool to document the provenance (origin and license) of third-party software using small text files. Collect inventories and generate attribution documentation.
+Home-page: https://github.com/nexB/aboutcode-toolkit
+Author: nexB. Inc. and others
+Author-email: info@aboutcode.org
+License: Apache-2.0
+Keywords: license,about,metadata,package,copyright,attribution,software,inventory,open source,sca,SBOM,spdx
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: System :: Software Distribution
+Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: testing
+Provides-Extra: docs
+License-File: apache-2.0.LICENSE
+License-File: NOTICE
+License-File: AUTHORS.rst
+License-File: CHANGELOG.rst
+License-File: CODE_OF_CONDUCT.rst
+
+=================
+AboutCode Toolkit
+=================
+
+Introduction
+------------
+The AboutCode Toolkit and ABOUT files provide a simple way to document the
+origin, license, usage and other important or interesting information about
+third-party software components that you use in your project.
+
+You start by storing ABOUT files (a small YAML formatted text file with field/value pairs)
+side-by-side with each of the third-party software components you use.
+Each ABOUT file documents origin and license for one software.
+There are many examples of ABOUT files (valid or invalid) in the testdata/
+directory of the whole repository.
+
+The current version of the AboutCode Toolkit can read these ABOUT files so that you
+can collect and validate the inventory of third-party components that you use.
+
+In addition, this tool is able to generate attribution notices and
+identify redistributable source code used in your project to help you comply
+with open source licenses conditions.
+
+This version of the AboutCode Toolkit follows the ABOUT specification version 3.3.1 at:
+https://aboutcode-toolkit.readthedocs.io/en/latest/specification.html
+
+
+Build and tests status
+----------------------
+
++-------+-----------------+--------------+
+|Branch | **Linux/macOS** | **Windows**  |
++=======+=================+==============+
+|Master | |master-posix|  | |master-win| |
++-------+-----------------+--------------+
+|Develop| |devel-posix|   | |devel-win|  |
++-------+-----------------+--------------+
+
+
+REQUIREMENTS
+------------
+The AboutCode Toolkit is tested with Python 3.7 or above only on Linux, Mac and Windows.
+You will need to install a Python interpreter if you do not have one already
+installed.
+
+On Linux and Mac, Python is typically pre-installed. To verify which
+version may be pre-installed, open a terminal and type:
+
+    python --version
+
+Note
+~~~~
+    Debian has decided that distutils is not a core python package, so it is not included in the last versions of debian and debian-based OSes.
+    A solution is to run: `sudo apt install python3-distutils`
+
+On Windows or Mac, you can download the latest Python here:
+    https://www.python.org/downloads/
+
+Download the .msi installer for Windows or the .dmg archive for Mac.
+Open and run the installer using all the default options.
+
+INSTALLATION
+------------
+Checkout or download and extract the AboutCode Toolkit from:
+    https://github.com/nexB/aboutcode-toolkit/
+
+To install all the needed dependencies in a virtualenv, run (on posix):
+    ./configure
+or on windows:
+    configure
+
+ACTIVATE the VIRTUALENV
+-----------------------
+To activate the virtualenv, run (on posix):
+    source venv/bin/activate
+or on windows:
+    venv\\bin\\activate
+
+
+DEACTIVATE the VIRTUALENV
+-------------------------
+To deactivate the virtualenv, run (on both posix and windows):
+    deactivate
+
+
+VERSIONING SCHEMA
+-----------------
+Starting at AboutCode version 4.0.0, the AboutCode Toolkit will follow SemVer for the versioning schema.
+
+i.e. MAJOR.MINOR.PATCH format
+    1. MAJOR version when making incompatible API changes,
+    2. MINOR version when making functionality in a backwards compatible manner, and
+    3. PATCH version when making backwards compatible bug fixes.
+
+
+REFERENCE
+---------
+See https://aboutcode-toolkit.readthedocs.io/en/latest/ for documentation.
+
+See https://aboutcode-toolkit.readthedocs.io/en/latest/reference.html for reference.
+
+TESTS and DEVELOPMENT
+---------------------
+To install all the needed development dependencies, run (on posix):
+    ./configure --dev
+or on windows:
+    configure --dev
+
+To verify that everything works fine you can run the test suite with:
+    pytest
+
+
+CLEAN BUILD AND INSTALLED FILES
+-------------------------------
+To clean the built and installed files, run (on posix):
+    ./configure --clean
+or on windows:
+    configure --clean
+
+
+HELP and SUPPORT
+----------------
+If you have a question or find a bug, enter a ticket at:
+
+    https://github.com/nexB/aboutcode-toolkit
+
+For issues, you can use:
+
+    https://github.com/nexB/aboutcode-toolkit/issues
+
+
+SOURCE CODE
+-----------
+The AboutCode Toolkit is available through GitHub. For the latest version visit:
+    https://github.com/nexB/aboutcode-toolkit
+
+
+HACKING
+-------
+We accept pull requests provided under the same license as this tool.
+You agree to the http://developercertificate.org/
+
+
+LICENSE
+-------
+The AboutCode Toolkit is released under the Apache 2.0 license.
+See (of course) the about.ABOUT file for details.
+
+
+.. |master-posix| image:: https://api.travis-ci.org/nexB/aboutcode-toolkit.png?branch=master
+    :target: https://travis-ci.org/nexB/aboutcode-toolkit
+    :alt: Linux Master branch tests status
+.. |devel-posix| image:: https://api.travis-ci.org/nexB/aboutcode-toolkit.png?branch=develop
+    :target: https://travis-ci.org/nexB/aboutcode-toolkit
+    :alt: Linux Develop branch tests status
+
+.. |master-win| image:: https://ci.appveyor.com/api/projects/status/uwj2gh8i9ga1mqwn/branch/master?png=true
+    :target: https://ci.appveyor.com/project/nexB/aboutcode-toolkit
+    :alt: Windows Master branch tests status
+.. |devel-win| image:: https://ci.appveyor.com/api/projects/status/uwj2gh8i9ga1mqwn/branch/develop?png=true
+    :target: https://ci.appveyor.com/project/nexB/aboutcode-toolkit
+    :alt: Windows Develop branch tests status
```

### Comparing `aboutcode-toolkit-8.0.0/src/aboutcode_toolkit.egg-info/SOURCES.txt` & `aboutcode-toolkit-9.0.0/src/aboutcode_toolkit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -137,19 +137,19 @@
 src/attributecode/attrib_util.py
 src/attributecode/cmd.py
 src/attributecode/gen.py
 src/attributecode/licenses.py
 src/attributecode/model.py
 src/attributecode/transform.py
 src/attributecode/util.py
-templates/default_html.template
-templates/default_json.template
-templates/license_ref.template
-templates/list.csv
-templates/scancode_html.template
+src/attributecode/templates/default_html.template
+src/attributecode/templates/default_json.template
+src/attributecode/templates/license_ref.template
+src/attributecode/templates/list.csv
+src/attributecode/templates/scancode_html.template
 tests/test_api.py
 tests/test_attrib.py
 tests/test_cmd.py
 tests/test_gen.py
 tests/test_model.py
 tests/test_transform.py
 tests/test_util.py
@@ -368,14 +368,15 @@
 tests/testdata/test_model/parse/missing_required.ABOUT
 tests/testdata/test_model/parse/multi_line_license_expresion.ABOUT
 tests/testdata/test_model/parse/name_mapping_test.ABOUT
 tests/testdata/test_model/parse/no_file_fields.ABOUT
 tests/testdata/test_model/parse/non_ascii_field_name_value.about
 tests/testdata/test_model/parse/notice_text.NOTICE
 tests/testdata/test_model/parse/ordered_fields.ABOUT
+tests/testdata/test_model/parse/with_ignored_resources.ABOUT
 tests/testdata/test_model/parse/complete2/NOTICE
 tests/testdata/test_model/parse/complete2/about.ABOUT
 tests/testdata/test_model/parse/complete2/about2.ABOUT
 tests/testdata/test_model/parse/complete2/apache-2.0.LICENSE
 tests/testdata/test_model/redistribution/this.ABOUT
 tests/testdata/test_model/redistribution/this.c
 tests/testdata/test_model/redistribution/this2.ABOUT
```

### Comparing `aboutcode-toolkit-8.0.0/src/attributecode/__init__.py` & `aboutcode-toolkit-9.0.0/src/attributecode/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 
 from collections import namedtuple
 import logging
 import os
 
 import saneyaml
 
-__version__ = '8.0.0'
+__version__ = '9.0.0'
 
-__about_spec_version__ = '3.3.0'
+__about_spec_version__ = '3.3.1'
 
 __copyright__ = """
 Copyright (c) nexB Inc. All rights reserved. http://dejacode.org
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `aboutcode-toolkit-8.0.0/src/attributecode/__main__.py` & `aboutcode-toolkit-9.0.0/src/attributecode/__main__.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/src/attributecode/api.py` & `aboutcode-toolkit-9.0.0/src/attributecode/api.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/src/attributecode/attrib.py` & `aboutcode-toolkit-9.0.0/src/attributecode/attrib.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 from attributecode.licenses import COMMON_LICENSES
 from attributecode.model import parse_license_expression
 from attributecode.model import License, StringField
 from attributecode.util import add_unc
 from attributecode.attrib_util import multi_sort
 
 DEFAULT_TEMPLATE_FILE = os.path.join(
-    os.path.dirname(os.path.realpath(__file__)), '../../templates', 'default_html.template')
+    os.path.dirname(os.path.realpath(__file__)), 'templates', 'default_html.template')
 
 DEFAULT_TEMPLATE_SCANCODE_FILE = os.path.join(
-    os.path.dirname(os.path.realpath(__file__)), '../../templates', 'scancode_html.template')
+    os.path.dirname(os.path.realpath(__file__)), 'templates', 'scancode_html.template')
 
 DEFAULT_LICENSE_SCORE = 100
 
 def generate(abouts, is_about_input, license_dict, scancode, min_license_score, template=None, vartext=None):
     """
     Generate an attribution text from an `abouts` list of About objects, a
     `template` template text and a `vartext` optional dict of extra
```

### Comparing `aboutcode-toolkit-8.0.0/src/attributecode/attrib_util.py` & `aboutcode-toolkit-9.0.0/src/attributecode/attrib_util.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/src/attributecode/cmd.py` & `aboutcode-toolkit-9.0.0/src/attributecode/cmd.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/src/attributecode/gen.py` & `aboutcode-toolkit-9.0.0/src/attributecode/gen.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/src/attributecode/licenses.py` & `aboutcode-toolkit-9.0.0/src/attributecode/licenses.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/src/attributecode/model.py` & `aboutcode-toolkit-9.0.0/src/attributecode/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -554,14 +554,30 @@
         self.resolved_paths = []
 
     def _validate(self, *args, **kwargs):
         errors = super(AboutResourceField, self)._validate(*args, ** kwargs)
         return errors
 
 
+class IgnoredResourcesField(PathField):
+    """
+    Special field for ignored_resources. self.ignored_paths contains a list of
+    path patterns (glob patterns) which are not part of the summarization provided
+    by the ABOUT file. 
+    """
+
+    def __init__(self, *args, ** kwargs):
+        super(AboutResourceField, self).__init__(*args, ** kwargs)
+        self.resolved_paths = []
+
+    def _validate(self, *args, **kwargs):
+        errors = super(AboutResourceField, self)._validate(*args, ** kwargs)
+        return errors
+
+
 class FileTextField(PathField):
     """
     A path field pointing to one or more text files such as license files.
     The validated value is an ordered dict of path->Text or None if no
     location or text could not be loaded.
     """
 
@@ -760,14 +776,15 @@
         """
         Create fields in an ordered dict to keep a standard ordering. We
         could use a metaclass to track ordering django-like but this approach
         is simpler.
         """
         self.fields = dict([
             ('about_resource', AboutResourceField(required=True)),
+            ('ignored_resources', AboutResourceField()),
             ('name', SingleLineField(required=True)),
             ('version', SingleLineField()),
 
             ('download_url', UrlField()),
             ('description', StringField()),
             ('homepage_url', UrlField()),
             ('package_url', PackageUrlField()),
```

### Comparing `aboutcode-toolkit-8.0.0/src/attributecode/transform.py` & `aboutcode-toolkit-9.0.0/src/attributecode/transform.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/src/attributecode/util.py` & `aboutcode-toolkit-9.0.0/src/attributecode/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -676,18 +676,24 @@
     results = []
     errors = []
     import warnings
 
     # This is to prevent showing the: warn("Workbook contains no default style, apply openpyxl's default")
     with warnings.catch_warnings(record=True):
         input_bom = openpyxl.load_workbook(location)
+        sheetnames = input_bom.sheetnames
         if worksheet:
+            if worksheet not in sheetnames:
+                import sys
+                print("The input worksheet name does not exist. Exiting.")
+                sys.exit(1)
             sheet_obj = input_bom[worksheet]
         else:
             sheet_obj = input_bom.active
+    print("Working on the " + sheet_obj.title + " worksheet.")
     max_col = sheet_obj.max_column
 
     index = 1
     col_keys = []
     mapping_dict = {}
 
     while index <= max_col:
```

### Comparing `aboutcode-toolkit-8.0.0/templates/default_html.template` & `aboutcode-toolkit-9.0.0/src/attributecode/templates/default_html.template`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/templates/default_json.template` & `aboutcode-toolkit-9.0.0/src/attributecode/templates/default_json.template`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/templates/license_ref.template` & `aboutcode-toolkit-9.0.0/src/attributecode/templates/license_ref.template`

 * *Files 4% similar despite different names*

```diff
@@ -30,24 +30,24 @@
     </div>
     <hr>
 
     {% for license in licenses_list %}
         <div id="group_{{ loop.index0 }}">
             <h3>{{ license.name }}</h3>
             <p>This product contains the following open source software packages licensed under the terms of the license: {{license.name}}</p>
-            
+
             <div class="oss-component" id="component_{{ loop.index0 }}">
-            {%for about_object in abouts %} 
+            {%for about_object in abouts %}
                 {% if loop.first %}
                     {% if license.url %}
                         <p>License Gallery URL: <a href="{{ license.url }}">{{license.url}}</a> </p>
                     {% endif %}
                 {% endif %}
                 {% if license.key in about_object.license_key.value %}
-                    <li>{{ about_object.name.value }}{% if about_object.version.value %}  - Version  {{ about_object.version.value }}{% endif %}</li>       
+                    <li>{{ about_object.name.value }}{% if about_object.version.value %}  - Version  {{ about_object.version.value }}{% endif %}</li>
                     {% if about_object.copyright.value %}
                         <pre>Copyright: {{about_object.copyright.value}}</pre>
                     {% endif %}
                     {% if about_object.notice_file.value %}
                         {% for notice in about_object.notice_file.value %}
                             <pre class="component-notice">
                                 {{ about_object.notice_file.value[notice] }}
@@ -59,11 +59,11 @@
                     <pre>{{license.text}}</pre>
                 {% endif %}
             {% endfor %}
             </div>
         </div>
     {% endfor %}
     <hr>
-<hr> 
+<hr>
 <h3><a id="End">End</a></h3>
 </body>
 </html>
```

### Comparing `aboutcode-toolkit-8.0.0/templates/scancode_html.template` & `aboutcode-toolkit-9.0.0/src/attributecode/templates/scancode_html.template`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/test_api.py` & `aboutcode-toolkit-9.0.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/test_attrib.py` & `aboutcode-toolkit-9.0.0/tests/test_attrib.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/test_cmd.py` & `aboutcode-toolkit-9.0.0/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/test_gen.py` & `aboutcode-toolkit-9.0.0/tests/test_gen.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/test_model.py` & `aboutcode-toolkit-9.0.0/tests/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,14 +452,25 @@
         test_file = get_test_loc('test_gen/parser_tests/about_resource_field.ABOUT')
         a = model.About(test_file)
         assert [] == a.errors
         result = a.about_resource.value['about_resource.c']
         # this means we have a location
         self.assertNotEqual([], result)
 
+    def test_About_loads_ignored_resources_field(self):
+        # fields in this file are not in the standard order
+        test_file = get_test_loc('test_model/parse/with_ignored_resources.ABOUT')
+        a = model.About(test_file)
+        #assert [] == a.errors
+
+        expected = ['about_resource', 'ignored_resources', 'name']
+        result = [f.name for f in a.all_fields() if f.present]
+        assert expected == result
+
+
     def test_About_has_errors_when_about_resource_is_missing(self):
         test_file = get_test_loc('test_gen/parser_tests/.ABOUT')
         a = model.About(test_file)
         expected = [Error(CRITICAL, 'Field about_resource is required')]
         result = a.errors
         assert expected == result
```

### Comparing `aboutcode-toolkit-8.0.0/tests/test_transform.py` & `aboutcode-toolkit-9.0.0/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/test_util.py` & `aboutcode-toolkit-9.0.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/default_template/expect.html` & `aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/default_template/expect.html`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/gen_default_template/expected_default_attrib.html` & `aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/gen_default_template/expected_default_attrib.html`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/gen_license_key_name_check/custom.template` & `aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/gen_license_key_name_check/custom.template`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/gen_license_key_name_check/expected/expected.html` & `aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/gen_license_key_name_check/expected/expected.html`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/scancode_input/clean-text-0.3.0-mod-lceupi.json` & `aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/scancode_input/clean-text-0.3.0-mod-lceupi.json`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/scancode_input/expect.html` & `aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/scancode_input/expect.html`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_attrib/scancode_input/scancode.template` & `aboutcode-toolkit-9.0.0/tests/testdata/test_attrib/scancode_input/scancode.template`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/geninventory.csv` & `aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/geninventory.csv`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/help/about_attrib_help.txt` & `aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/help/about_attrib_help.txt`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/help/about_check_help.txt` & `aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/help/about_check_help.txt`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/help/about_gen_help.txt` & `aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/help/about_gen_help.txt`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/help/about_gen_license_help.txt` & `aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/help/about_gen_license_help.txt`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/help/about_help.txt` & `aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/help/about_help.txt`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/help/about_inventory_help.txt` & `aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/help/about_inventory_help.txt`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/help/about_transform_config_help.txt` & `aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/help/about_transform_config_help.txt`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/help/about_transform_help.txt` & `aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/help/about_transform_help.txt`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_cmd/transform.csv` & `aboutcode-toolkit-9.0.0/tests/testdata/test_cmd/transform.csv`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/Jinja2.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/Jinja2.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/MarkupSafe.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/MarkupSafe.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/PSF.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/PSF.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/apache-2.0.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/certifi.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/certifi.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/click.ABOUT` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/click.ABOUT`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/click.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/click.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/colorama.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/colorama.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/lgpl-2.1.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/lgpl-2.1.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/pip.AUTHORS` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/pip.AUTHORS`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/pip.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/pip.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/py.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/py.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/pytest.ABOUT` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/pytest.ABOUT`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/pytest.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/pytest.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/schematics.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/schematics.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/unicodecsv.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/unicodecsv.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/wheel.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/wheel.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/about/wincertstore.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/about/wincertstore.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/inventory/complex/expected.csv` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/inventory/complex/expected.csv`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/load/clean-text-0.3.0-lceupi.json` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/load/clean-text-0.3.0-lceupi.json`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_gen/load/simple_sample.xlsx` & `aboutcode-toolkit-9.0.0/tests/testdata/test_gen/load/simple_sample.xlsx`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/android/multi_license.c.ABOUT` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/android/multi_license.c.ABOUT`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/dumps/about.ABOUT` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/dumps/about.ABOUT`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/equal/complete/about.ABOUT` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/equal/complete/about.ABOUT`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/equal/complete2/about.ABOUT` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/equal/complete2/about.ABOUT`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/Jinja2.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/Jinja2.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/MarkupSafe.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/MarkupSafe.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/PSF.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/PSF.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/apache-2.0.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/certifi.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/certifi.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/click.ABOUT` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/click.ABOUT`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/click.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/click.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/colorama.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/colorama.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/lgpl-2.1.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/lgpl-2.1.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/pip.AUTHORS` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/pip.AUTHORS`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/pip.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/pip.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/py.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/py.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/pytest.ABOUT` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/pytest.ABOUT`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/pytest.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/pytest.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/schematics.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/schematics.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/unicodecsv.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/unicodecsv.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/virtualenv.ABOUT` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/virtualenv.ABOUT`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/virtualenv.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/virtualenv.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/virtualenv.py.ABOUT` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/virtualenv.py.ABOUT`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/wheel.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/wheel.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/about/wincertstore.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/about/wincertstore.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/inventory/complex/expected.csv` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/inventory/complex/expected.csv`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/longpath.zip` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/longpath.zip`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/rel/allAboutInOneDir/about_ref/elasticsearch.ABOUT` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/rel/allAboutInOneDir/about_ref/elasticsearch.ABOUT`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/single_file/django_snippets.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/single_file/django_snippets.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_model/unicode/nose-selecttests.ABOUT` & `aboutcode-toolkit-9.0.0/tests/testdata/test_model/unicode/nose-selecttests.ABOUT`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_transform/input.xlsx` & `aboutcode-toolkit-9.0.0/tests/testdata/test_transform/input.xlsx`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_transform/input_scancode.json` & `aboutcode-toolkit-9.0.0/tests/testdata/test_transform/input_scancode.json`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_transform/simple.xlsx` & `aboutcode-toolkit-9.0.0/tests/testdata/test_transform/simple.xlsx`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_util/json/aboutcode_manager_exported.json` & `aboutcode-toolkit-9.0.0/tests/testdata/test_util/json/aboutcode_manager_exported.json`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_util/json/scancode_info.json` & `aboutcode-toolkit-9.0.0/tests/testdata/test_util/json/scancode_info.json`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_util/licenses/mit.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_util/licenses/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_util/licenses/mit2.LICENSE` & `aboutcode-toolkit-9.0.0/tests/testdata/test_util/licenses/mit2.LICENSE`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testdata/test_util/longpath.zip` & `aboutcode-toolkit-9.0.0/tests/testdata/test_util/longpath.zip`

 * *Files identical despite different names*

### Comparing `aboutcode-toolkit-8.0.0/tests/testing_utils.py` & `aboutcode-toolkit-9.0.0/tests/testing_utils.py`

 * *Files identical despite different names*

