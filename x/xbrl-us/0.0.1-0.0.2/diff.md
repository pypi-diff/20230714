# Comparing `tmp/xbrl-us-0.0.1.tar.gz` & `tmp/xbrl-us-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbrl-us-0.0.1.tar", last modified: Sun Jul  9 17:07:13 2023, max compression
+gzip compressed data, was "xbrl-us-0.0.2.tar", last modified: Fri Jul 14 15:48:31 2023, max compression
```

## Comparing `xbrl-us-0.0.1.tar` & `xbrl-us-0.0.2.tar`

### file list

```diff
@@ -1,202 +1,111 @@
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:13.007988 xbrl-us-0.0.1/
--rw-r--r--   0 hamid      (501) staff       (20)      527 2023-07-09 16:41:01.000000 xbrl-us-0.0.1/.bumpversion.cfg
--rw-r--r--   0 hamid      (501) staff       (20)     2015 2023-07-09 16:41:01.000000 xbrl-us-0.0.1/.cookiecutterrc
--rw-r--r--   0 hamid      (501) staff       (20)      175 2023-06-26 21:38:04.000000 xbrl-us-0.0.1/.coveragerc
--rw-r--r--   0 hamid      (501) staff       (20)      353 2023-06-26 21:38:04.000000 xbrl-us-0.0.1/.editorconfig
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.887680 xbrl-us-0.0.1/.github/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.897964 xbrl-us-0.0.1/.github/workflows/
--rw-r--r--   0 hamid      (501) staff       (20)     5651 2023-07-08 20:14:20.000000 xbrl-us-0.0.1/.github/workflows/github-actions.yml
--rw-r--r--   0 hamid      (501) staff       (20)      688 2023-06-26 21:40:12.000000 xbrl-us-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 hamid      (501) staff       (20)      285 2023-07-08 20:32:20.000000 xbrl-us-0.0.1/.readthedocs.yml
--rw-r--r--   0 hamid      (501) staff       (20)       71 2023-07-06 22:38:13.000000 xbrl-us-0.0.1/AUTHORS.rst
--rw-r--r--   0 hamid      (501) staff       (20)       86 2023-07-09 17:04:06.000000 xbrl-us-0.0.1/CHANGELOG.rst
--rw-r--r--   0 hamid      (501) staff       (20)     2376 2023-06-26 21:38:04.000000 xbrl-us-0.0.1/CONTRIBUTING.rst
--rw-r--r--   0 hamid      (501) staff       (20)     1105 2023-06-26 21:41:13.000000 xbrl-us-0.0.1/LICENSE
--rw-r--r--   0 hamid      (501) staff       (20)      427 2023-06-26 21:38:04.000000 xbrl-us-0.0.1/MANIFEST.in
--rw-r--r--   0 hamid      (501) staff       (20)     8523 2023-07-09 17:07:13.007210 xbrl-us-0.0.1/PKG-INFO
--rw-r--r--   0 hamid      (501) staff       (20)     7172 2023-07-09 16:55:24.000000 xbrl-us-0.0.1/README.rst
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.898598 xbrl-us-0.0.1/ci/
--rwxr-xr-x   0 hamid      (501) staff       (20)     2867 2023-06-26 21:38:04.000000 xbrl-us-0.0.1/ci/bootstrap.py
--rw-r--r--   0 hamid      (501) staff       (20)       72 2023-06-26 21:38:04.000000 xbrl-us-0.0.1/ci/requirements.txt
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.888069 xbrl-us-0.0.1/ci/templates/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.888168 xbrl-us-0.0.1/ci/templates/.github/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.899166 xbrl-us-0.0.1/ci/templates/.github/workflows/
--rw-r--r--   0 hamid      (501) staff       (20)     1963 2023-06-26 21:38:04.000000 xbrl-us-0.0.1/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.905176 xbrl-us-0.0.1/docs/
--rw-r--r--   0 hamid      (501) staff       (20)       28 2023-06-26 21:38:04.000000 xbrl-us-0.0.1/docs/authors.rst
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.913339 xbrl-us-0.0.1/docs/build/
--rw-r--r--   0 hamid      (501) staff       (20)      230 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/.buildinfo
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.922479 xbrl-us-0.0.1/docs/build/.doctrees/
--rw-r--r--   0 hamid      (501) staff       (20)     2997 2023-07-09 14:48:43.000000 xbrl-us-0.0.1/docs/build/.doctrees/authors.doctree
--rw-r--r--   0 hamid      (501) staff       (20)     3032 2023-07-09 14:48:43.000000 xbrl-us-0.0.1/docs/build/.doctrees/changelog.doctree
--rw-r--r--   0 hamid      (501) staff       (20)    15513 2023-07-09 14:48:43.000000 xbrl-us-0.0.1/docs/build/.doctrees/contributing.doctree
--rw-r--r--   0 hamid      (501) staff       (20)  1161456 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/.doctrees/environment.pickle
--rw-r--r--   0 hamid      (501) staff       (20)     4406 2023-07-09 14:48:43.000000 xbrl-us-0.0.1/docs/build/.doctrees/index.doctree
--rw-r--r--   0 hamid      (501) staff       (20)     2716 2023-07-09 14:48:43.000000 xbrl-us-0.0.1/docs/build/.doctrees/modules.doctree
--rw-r--r--   0 hamid      (501) staff       (20)    27034 2023-07-09 14:48:43.000000 xbrl-us-0.0.1/docs/build/.doctrees/readme.doctree
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.924603 xbrl-us-0.0.1/docs/build/.doctrees/reference/
--rw-r--r--   0 hamid      (501) staff       (20)     2753 2023-07-09 15:04:38.000000 xbrl-us-0.0.1/docs/build/.doctrees/reference/index.doctree
--rw-r--r--   0 hamid      (501) staff       (20)    65369 2023-07-09 15:07:14.000000 xbrl-us-0.0.1/docs/build/.doctrees/reference/xbrl_us.doctree
--rw-r--r--   0 hamid      (501) staff       (20)   139110 2023-07-09 15:07:14.000000 xbrl-us-0.0.1/docs/build/.doctrees/xbrl_us.doctree
--rw-r--r--   0 hamid      (501) staff       (20)    54287 2023-07-09 15:07:14.000000 xbrl-us-0.0.1/docs/build/.doctrees/xbrl_us.schemas.doctree
--rw-r--r--   0 hamid      (501) staff       (20)   417391 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/.doctrees/xbrl_us.utils.doctree
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.925593 xbrl-us-0.0.1/docs/build/_modules/
--rw-r--r--   0 hamid      (501) staff       (20)    10821 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/_modules/index.html
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.927327 xbrl-us-0.0.1/docs/build/_modules/xbrl_us/
--rw-r--r--   0 hamid      (501) staff       (20)    12257 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/_modules/xbrl_us/cli.html
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.929647 xbrl-us-0.0.1/docs/build/_modules/xbrl_us/schemas/
--rw-r--r--   0 hamid      (501) staff       (20)    38625 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/_modules/xbrl_us/schemas/concept_details.html
--rw-r--r--   0 hamid      (501) staff       (20)    17749 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/_modules/xbrl_us/schemas/dimension_details.html
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.931489 xbrl-us-0.0.1/docs/build/_modules/xbrl_us/utils/
--rw-r--r--   0 hamid      (501) staff       (20)    11798 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/_modules/xbrl_us/utils/exceptions.html
--rw-r--r--   0 hamid      (501) staff       (20)    12174 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/_modules/xbrl_us/utils/fields.html
--rw-r--r--   0 hamid      (501) staff       (20)   100712 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/_modules/xbrl_us/utils/paramters.html
--rw-r--r--   0 hamid      (501) staff       (20)    77224 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/_modules/xbrl_us/xbrl_us.html
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.938514 xbrl-us-0.0.1/docs/build/_sources/
--rw-r--r--   0 hamid      (501) staff       (20)       28 2023-06-26 21:38:04.000000 xbrl-us-0.0.1/docs/build/_sources/authors.rst.txt
--rw-r--r--   0 hamid      (501) staff       (20)       30 2023-06-26 21:38:04.000000 xbrl-us-0.0.1/docs/build/_sources/changelog.rst.txt
--rw-r--r--   0 hamid      (501) staff       (20)       33 2023-06-26 21:38:04.000000 xbrl-us-0.0.1/docs/build/_sources/contributing.rst.txt
--rw-r--r--   0 hamid      (501) staff       (20)      219 2023-07-09 12:54:31.000000 xbrl-us-0.0.1/docs/build/_sources/index.rst.txt
--rw-r--r--   0 hamid      (501) staff       (20)       58 2023-07-07 21:55:14.000000 xbrl-us-0.0.1/docs/build/_sources/modules.rst.txt
--rw-r--r--   0 hamid      (501) staff       (20)       27 2023-06-26 21:38:04.000000 xbrl-us-0.0.1/docs/build/_sources/readme.rst.txt
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.940350 xbrl-us-0.0.1/docs/build/_sources/reference/
--rw-r--r--   0 hamid      (501) staff       (20)       59 2023-07-09 15:02:31.000000 xbrl-us-0.0.1/docs/build/_sources/reference/index.rst.txt
--rw-r--r--   0 hamid      (501) staff       (20)       98 2023-07-09 15:02:46.000000 xbrl-us-0.0.1/docs/build/_sources/reference/xbrl_us.rst.txt
--rw-r--r--   0 hamid      (501) staff       (20)      523 2023-07-07 21:55:14.000000 xbrl-us-0.0.1/docs/build/_sources/xbrl_us.rst.txt
--rw-r--r--   0 hamid      (501) staff       (20)     2413 2023-07-07 21:55:14.000000 xbrl-us-0.0.1/docs/build/_sources/xbrl_us.schemas.rst.txt
--rw-r--r--   0 hamid      (501) staff       (20)      510 2023-07-07 21:55:14.000000 xbrl-us-0.0.1/docs/build/_sources/xbrl_us.utils.rst.txt
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.953796 xbrl-us-0.0.1/docs/build/_static/
--rw-r--r--   0 hamid      (501) staff       (20)    14813 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/_static/basic.css
--rw-r--r--   0 hamid      (501) staff       (20)      313 2023-07-08 23:07:03.000000 xbrl-us-0.0.1/docs/build/_static/check-solid.svg
--rw-r--r--   0 hamid      (501) staff       (20)     9031 2023-07-08 23:07:03.000000 xbrl-us-0.0.1/docs/build/_static/clipboard.min.js
--rw-r--r--   0 hamid      (501) staff       (20)      411 2023-07-08 23:07:03.000000 xbrl-us-0.0.1/docs/build/_static/copy-button.svg
--rw-r--r--   0 hamid      (501) staff       (20)     2060 2023-07-08 23:07:03.000000 xbrl-us-0.0.1/docs/build/_static/copybutton.css
--rw-r--r--   0 hamid      (501) staff       (20)     8467 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/_static/copybutton.js
--rw-r--r--   0 hamid      (501) staff       (20)     2698 2023-07-08 23:07:03.000000 xbrl-us-0.0.1/docs/build/_static/copybutton_funcs.js
--rw-r--r--   0 hamid      (501) staff       (20)     1266 2023-07-06 21:59:12.000000 xbrl-us-0.0.1/docs/build/_static/debug.css
--rw-r--r--   0 hamid      (501) staff       (20)     4472 2023-07-06 21:59:11.000000 xbrl-us-0.0.1/docs/build/_static/doctools.js
--rw-r--r--   0 hamid      (501) staff       (20)      420 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/_static/documentation_options.js
--rw-r--r--   0 hamid      (501) staff       (20)      286 2023-07-06 21:59:11.000000 xbrl-us-0.0.1/docs/build/_static/file.png
--rw-r--r--   0 hamid      (501) staff       (20)     4758 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/_static/language_data.js
--rw-r--r--   0 hamid      (501) staff       (20)       90 2023-07-06 21:59:11.000000 xbrl-us-0.0.1/docs/build/_static/minus.png
--rw-r--r--   0 hamid      (501) staff       (20)       90 2023-07-06 21:59:11.000000 xbrl-us-0.0.1/docs/build/_static/plus.png
--rw-r--r--   0 hamid      (501) staff       (20)    20380 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/_static/pygments.css
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.956004 xbrl-us-0.0.1/docs/build/_static/scripts/
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-06 21:59:12.000000 xbrl-us-0.0.1/docs/build/_static/scripts/furo-extensions.js
--rw-r--r--   0 hamid      (501) staff       (20)     5275 2023-07-06 21:59:12.000000 xbrl-us-0.0.1/docs/build/_static/scripts/furo.js
--rw-r--r--   0 hamid      (501) staff       (20)      187 2023-07-06 21:59:12.000000 xbrl-us-0.0.1/docs/build/_static/scripts/furo.js.LICENSE.txt
--rw-r--r--   0 hamid      (501) staff       (20)    28547 2023-07-06 21:59:12.000000 xbrl-us-0.0.1/docs/build/_static/scripts/furo.js.map
--rw-r--r--   0 hamid      (501) staff       (20)    18215 2023-07-06 21:59:11.000000 xbrl-us-0.0.1/docs/build/_static/searchtools.js
--rw-r--r--   0 hamid      (501) staff       (20)     6034 2023-07-06 21:59:12.000000 xbrl-us-0.0.1/docs/build/_static/skeleton.css
--rw-r--r--   0 hamid      (501) staff       (20)     4712 2023-07-06 21:59:11.000000 xbrl-us-0.0.1/docs/build/_static/sphinx_highlight.js
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.959181 xbrl-us-0.0.1/docs/build/_static/styles/
--rw-r--r--   0 hamid      (501) staff       (20)     5529 2023-07-06 21:59:12.000000 xbrl-us-0.0.1/docs/build/_static/styles/furo-extensions.css
--rw-r--r--   0 hamid      (501) staff       (20)     7809 2023-07-06 21:59:12.000000 xbrl-us-0.0.1/docs/build/_static/styles/furo-extensions.css.map
--rw-r--r--   0 hamid      (501) staff       (20)    48206 2023-07-06 21:59:12.000000 xbrl-us-0.0.1/docs/build/_static/styles/furo.css
--rw-r--r--   0 hamid      (501) staff       (20)    72813 2023-07-06 21:59:12.000000 xbrl-us-0.0.1/docs/build/_static/styles/furo.css.map
--rw-r--r--   0 hamid      (501) staff       (20)    11440 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/authors.html
--rw-r--r--   0 hamid      (501) staff       (20)    11496 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/changelog.html
--rw-r--r--   0 hamid      (501) staff       (20)    18213 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/contributing.html
--rw-r--r--   0 hamid      (501) staff       (20)    44049 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/genindex.html
--rw-r--r--   0 hamid      (501) staff       (20)    13397 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/index.html
--rw-r--r--   0 hamid      (501) staff       (20)    15952 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/modules.html
--rw-r--r--   0 hamid      (501) staff       (20)     1473 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/objects.inv
--rw-r--r--   0 hamid      (501) staff       (20)    14841 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/py-modindex.html
--rw-r--r--   0 hamid      (501) staff       (20)    29857 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/readme.html
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.961131 xbrl-us-0.0.1/docs/build/reference/
--rw-r--r--   0 hamid      (501) staff       (20)    12275 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/reference/index.html
--rw-r--r--   0 hamid      (501) staff       (20)    33338 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/reference/xbrl_us.html
--rw-r--r--   0 hamid      (501) staff       (20)    10477 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/search.html
--rw-r--r--   0 hamid      (501) staff       (20)    41060 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/searchindex.js
--rw-r--r--   0 hamid      (501) staff       (20)    93386 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/xbrl_us.html
--rw-r--r--   0 hamid      (501) staff       (20)    33921 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/xbrl_us.schemas.html
--rw-r--r--   0 hamid      (501) staff       (20)   158637 2023-07-09 15:07:15.000000 xbrl-us-0.0.1/docs/build/xbrl_us.utils.html
--rw-r--r--   0 hamid      (501) staff       (20)       30 2023-06-26 21:38:04.000000 xbrl-us-0.0.1/docs/changelog.rst
--rw-r--r--   0 hamid      (501) staff       (20)     1155 2023-07-09 16:41:01.000000 xbrl-us-0.0.1/docs/conf.py
--rw-r--r--   0 hamid      (501) staff       (20)       33 2023-06-26 21:38:04.000000 xbrl-us-0.0.1/docs/contributing.rst
--rw-r--r--   0 hamid      (501) staff       (20)      219 2023-07-09 12:54:31.000000 xbrl-us-0.0.1/docs/index.rst
--rw-r--r--   0 hamid      (501) staff       (20)       58 2023-07-07 21:55:14.000000 xbrl-us-0.0.1/docs/modules.rst
--rw-r--r--   0 hamid      (501) staff       (20)       27 2023-06-26 21:38:04.000000 xbrl-us-0.0.1/docs/readme.rst
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.962537 xbrl-us-0.0.1/docs/reference/
--rw-r--r--   0 hamid      (501) staff       (20)       59 2023-07-09 15:02:31.000000 xbrl-us-0.0.1/docs/reference/index.rst
--rw-r--r--   0 hamid      (501) staff       (20)       98 2023-07-09 15:02:46.000000 xbrl-us-0.0.1/docs/reference/xbrl_us.rst
--rw-r--r--   0 hamid      (501) staff       (20)       35 2023-07-09 00:13:53.000000 xbrl-us-0.0.1/docs/requirements.txt
--rw-r--r--   0 hamid      (501) staff       (20)      109 2023-06-26 21:38:04.000000 xbrl-us-0.0.1/docs/spelling_wordlist.txt
--rw-r--r--   0 hamid      (501) staff       (20)      523 2023-07-07 21:55:14.000000 xbrl-us-0.0.1/docs/xbrl_us.rst
--rw-r--r--   0 hamid      (501) staff       (20)     2413 2023-07-07 21:55:14.000000 xbrl-us-0.0.1/docs/xbrl_us.schemas.rst
--rw-r--r--   0 hamid      (501) staff       (20)      510 2023-07-07 21:55:14.000000 xbrl-us-0.0.1/docs/xbrl_us.utils.rst
--rw-r--r--   0 hamid      (501) staff       (20)     1194 2023-06-26 21:38:04.000000 xbrl-us-0.0.1/pyproject.toml
--rw-r--r--   0 hamid      (501) staff       (20)      772 2023-06-26 21:38:04.000000 xbrl-us-0.0.1/pytest.ini
--rw-r--r--   0 hamid      (501) staff       (20)       38 2023-07-09 17:07:13.008161 xbrl-us-0.0.1/setup.cfg
--rwxr-xr-x   0 hamid      (501) staff       (20)     2891 2023-07-09 17:06:57.000000 xbrl-us-0.0.1/setup.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.890542 xbrl-us-0.0.1/src/
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.965582 xbrl-us-0.0.1/src/xbrl_us/
--rw-r--r--   0 hamid      (501) staff       (20)     6148 2023-07-05 15:58:36.000000 xbrl-us-0.0.1/src/xbrl_us/.DS_Store
--rw-r--r--   0 hamid      (501) staff       (20)       69 2023-07-09 16:41:01.000000 xbrl-us-0.0.1/src/xbrl_us/__init__.py
--rw-r--r--   0 hamid      (501) staff       (20)      383 2023-06-26 21:38:04.000000 xbrl-us-0.0.1/src/xbrl_us/__main__.py
--rw-r--r--   0 hamid      (501) staff       (20)      813 2023-06-26 21:38:04.000000 xbrl-us-0.0.1/src/xbrl_us/cli.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.995353 xbrl-us-0.0.1/src/xbrl_us/methods/
--rw-r--r--   0 hamid      (501) staff       (20)      814 2023-07-09 15:35:51.000000 xbrl-us-0.0.1/src/xbrl_us/methods/assertion search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      151 2023-07-09 15:53:07.000000 xbrl-us-0.0.1/src/xbrl_us/methods/assertion validate.yml
--rw-r--r--   0 hamid      (501) staff       (20)      852 2023-07-09 16:30:01.000000 xbrl-us-0.0.1/src/xbrl_us/methods/concept name search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      831 2023-07-09 16:32:18.000000 xbrl-us-0.0.1/src/xbrl_us/methods/concept search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      927 2023-07-09 16:22:11.000000 xbrl-us-0.0.1/src/xbrl_us/methods/cube search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      814 2023-07-09 16:23:23.000000 xbrl-us-0.0.1/src/xbrl_us/methods/dimension search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      522 2023-07-09 16:25:56.000000 xbrl-us-0.0.1/src/xbrl_us/methods/document search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      330 2023-07-09 16:00:53.000000 xbrl-us-0.0.1/src/xbrl_us/methods/dts id concept label.yml
--rw-r--r--   0 hamid      (501) staff       (20)      720 2023-07-09 15:59:38.000000 xbrl-us-0.0.1/src/xbrl_us/methods/dts id concept name.yml
--rw-r--r--   0 hamid      (501) staff       (20)      439 2023-07-09 16:01:40.000000 xbrl-us-0.0.1/src/xbrl_us/methods/dts id concept reference.yml
--rw-r--r--   0 hamid      (501) staff       (20)      803 2023-07-09 15:58:18.000000 xbrl-us-0.0.1/src/xbrl_us/methods/dts id concept search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1120 2023-07-09 16:04:42.000000 xbrl-us-0.0.1/src/xbrl_us/methods/dts id network search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      700 2023-07-09 16:03:43.000000 xbrl-us-0.0.1/src/xbrl_us/methods/dts id network.yml
--rw-r--r--   0 hamid      (501) staff       (20)      375 2023-07-09 15:55:59.000000 xbrl-us-0.0.1/src/xbrl_us/methods/dts search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1079 2023-07-09 15:30:31.000000 xbrl-us-0.0.1/src/xbrl_us/methods/entity id report search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      193 2023-07-09 15:33:34.000000 xbrl-us-0.0.1/src/xbrl_us/methods/entity id.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1123 2023-07-09 15:32:42.000000 xbrl-us-0.0.1/src/xbrl_us/methods/entity report search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      237 2023-07-09 15:35:01.000000 xbrl-us-0.0.1/src/xbrl_us/methods/entity search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1585 2023-07-09 01:30:09.000000 xbrl-us-0.0.1/src/xbrl_us/methods/fact id.yml
--rw-r--r--   0 hamid      (501) staff       (20)      969 2023-07-09 15:12:43.000000 xbrl-us-0.0.1/src/xbrl_us/methods/fact search oim.yml
--rw-r--r--   0 hamid      (501) staff       (20)     2524 2023-07-09 01:30:09.000000 xbrl-us-0.0.1/src/xbrl_us/methods/fact search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      369 2023-07-09 16:09:23.000000 xbrl-us-0.0.1/src/xbrl_us/methods/label dts id search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      360 2023-07-09 16:10:31.000000 xbrl-us-0.0.1/src/xbrl_us/methods/label search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1182 2023-07-09 16:12:21.000000 xbrl-us-0.0.1/src/xbrl_us/methods/network id relationship search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      244 2023-07-09 16:13:45.000000 xbrl-us-0.0.1/src/xbrl_us/methods/network id.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1169 2023-07-09 16:13:19.000000 xbrl-us-0.0.1/src/xbrl_us/methods/network relationship search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1173 2023-07-09 16:20:24.000000 xbrl-us-0.0.1/src/xbrl_us/methods/relationship search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      806 2023-07-09 16:20:24.000000 xbrl-us-0.0.1/src/xbrl_us/methods/relationship tree search.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1183 2023-07-09 15:26:42.000000 xbrl-us-0.0.1/src/xbrl_us/methods/report fact search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      110 2023-07-09 15:28:03.000000 xbrl-us-0.0.1/src/xbrl_us/methods/report id delete.yml
--rw-r--r--   0 hamid      (501) staff       (20)     2741 2023-07-09 15:24:28.000000 xbrl-us-0.0.1/src/xbrl_us/methods/report id fact search.yml
--rw-r--r--   0 hamid      (501) staff       (20)      749 2023-07-09 15:18:44.000000 xbrl-us-0.0.1/src/xbrl_us/methods/report id.yml
--rw-r--r--   0 hamid      (501) staff       (20)     1146 2023-07-09 15:17:55.000000 xbrl-us-0.0.1/src/xbrl_us/methods/report search.yml
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:13.003075 xbrl-us-0.0.1/src/xbrl_us/schemas/
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:52:58.000000 xbrl-us-0.0.1/src/xbrl_us/schemas/__init__.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:14.000000 xbrl-us-0.0.1/src/xbrl_us/schemas/assertion_details.py
--rw-r--r--   0 hamid      (501) staff       (20)     5257 2023-07-07 22:17:57.000000 xbrl-us-0.0.1/src/xbrl_us/schemas/concept_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:14.000000 xbrl-us-0.0.1/src/xbrl_us/schemas/cube_details.py
--rw-r--r--   0 hamid      (501) staff       (20)     1501 2023-07-07 22:17:57.000000 xbrl-us-0.0.1/src/xbrl_us/schemas/dimension_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:36.000000 xbrl-us-0.0.1/src/xbrl_us/schemas/document_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:29.000000 xbrl-us-0.0.1/src/xbrl_us/schemas/dts_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:05.000000 xbrl-us-0.0.1/src/xbrl_us/schemas/entity_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:56:32.000000 xbrl-us-0.0.1/src/xbrl_us/schemas/fact_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:47.000000 xbrl-us-0.0.1/src/xbrl_us/schemas/label_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:54.000000 xbrl-us-0.0.1/src/xbrl_us/schemas/network_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:04.000000 xbrl-us-0.0.1/src/xbrl_us/schemas/relationship_details.py
--rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:41:48.000000 xbrl-us-0.0.1/src/xbrl_us/schemas/report_details.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:13.006004 xbrl-us-0.0.1/src/xbrl_us/utils/
--rw-r--r--   0 hamid      (501) staff       (20)       97 2023-07-08 23:56:21.000000 xbrl-us-0.0.1/src/xbrl_us/utils/__init__.py
--rw-r--r--   0 hamid      (501) staff       (20)      243 2023-07-07 15:30:35.000000 xbrl-us-0.0.1/src/xbrl_us/utils/exceptions.py
--rw-r--r--   0 hamid      (501) staff       (20)      464 2023-07-08 23:56:22.000000 xbrl-us-0.0.1/src/xbrl_us/utils/fields.py
--rw-r--r--   0 hamid      (501) staff       (20)    26377 2023-07-07 22:12:20.000000 xbrl-us-0.0.1/src/xbrl_us/utils/paramters.py
--rw-r--r--   0 hamid      (501) staff       (20)    20916 2023-07-09 15:07:46.000000 xbrl-us-0.0.1/src/xbrl_us/xbrl_us.py
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:12.971383 xbrl-us-0.0.1/src/xbrl_us.egg-info/
--rw-r--r--   0 hamid      (501) staff       (20)     8523 2023-07-09 17:07:12.000000 xbrl-us-0.0.1/src/xbrl_us.egg-info/PKG-INFO
--rw-r--r--   0 hamid      (501) staff       (20)     5672 2023-07-09 17:07:12.000000 xbrl-us-0.0.1/src/xbrl_us.egg-info/SOURCES.txt
--rw-r--r--   0 hamid      (501) staff       (20)        1 2023-07-09 17:07:12.000000 xbrl-us-0.0.1/src/xbrl_us.egg-info/dependency_links.txt
--rw-r--r--   0 hamid      (501) staff       (20)       45 2023-07-09 17:07:12.000000 xbrl-us-0.0.1/src/xbrl_us.egg-info/entry_points.txt
--rw-r--r--   0 hamid      (501) staff       (20)        1 2023-07-08 14:55:19.000000 xbrl-us-0.0.1/src/xbrl_us.egg-info/not-zip-safe
--rw-r--r--   0 hamid      (501) staff       (20)       61 2023-07-09 17:07:12.000000 xbrl-us-0.0.1/src/xbrl_us.egg-info/requires.txt
--rw-r--r--   0 hamid      (501) staff       (20)        8 2023-07-09 17:07:12.000000 xbrl-us-0.0.1/src/xbrl_us.egg-info/top_level.txt
-drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-09 17:07:13.006486 xbrl-us-0.0.1/tests/
--rw-r--r--   0 hamid      (501) staff       (20)       73 2023-06-26 21:41:13.000000 xbrl-us-0.0.1/tests/test_xbrl_us.py
--rw-r--r--   0 hamid      (501) staff       (20)     1656 2023-07-08 20:05:02.000000 xbrl-us-0.0.1/tox.ini
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.470951 xbrl-us-0.0.2/
+-rw-r--r--   0 hamid      (501) staff       (20)      527 2023-07-14 15:47:57.000000 xbrl-us-0.0.2/.bumpversion.cfg
+-rw-r--r--   0 hamid      (501) staff       (20)     2015 2023-07-14 15:47:57.000000 xbrl-us-0.0.2/.cookiecutterrc
+-rw-r--r--   0 hamid      (501) staff       (20)      175 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/.coveragerc
+-rw-r--r--   0 hamid      (501) staff       (20)      353 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/.editorconfig
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.420849 xbrl-us-0.0.2/.github/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.428399 xbrl-us-0.0.2/.github/workflows/
+-rw-r--r--   0 hamid      (501) staff       (20)     4514 2023-07-12 22:29:46.000000 xbrl-us-0.0.2/.github/workflows/github-actions.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      688 2023-06-26 21:40:12.000000 xbrl-us-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 hamid      (501) staff       (20)      285 2023-07-08 20:32:20.000000 xbrl-us-0.0.2/.readthedocs.yml
+-rw-r--r--   0 hamid      (501) staff       (20)       71 2023-07-06 22:38:13.000000 xbrl-us-0.0.2/AUTHORS.rst
+-rw-r--r--   0 hamid      (501) staff       (20)      377 2023-07-12 21:27:40.000000 xbrl-us-0.0.2/CHANGELOG.rst
+-rw-r--r--   0 hamid      (501) staff       (20)     2376 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 hamid      (501) staff       (20)     1105 2023-06-26 21:41:13.000000 xbrl-us-0.0.2/LICENSE
+-rw-r--r--   0 hamid      (501) staff       (20)      458 2023-07-12 23:53:11.000000 xbrl-us-0.0.2/MANIFEST.in
+-rw-r--r--   0 hamid      (501) staff       (20)     9385 2023-07-14 15:48:31.470263 xbrl-us-0.0.2/PKG-INFO
+-rw-r--r--   0 hamid      (501) staff       (20)     7743 2023-07-13 01:01:08.000000 xbrl-us-0.0.2/README.rst
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.428972 xbrl-us-0.0.2/ci/
+-rwxr-xr-x   0 hamid      (501) staff       (20)     2867 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/ci/bootstrap.py
+-rw-r--r--   0 hamid      (501) staff       (20)       72 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/ci/requirements.txt
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.421286 xbrl-us-0.0.2/ci/templates/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.421393 xbrl-us-0.0.2/ci/templates/.github/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.429288 xbrl-us-0.0.2/ci/templates/.github/workflows/
+-rw-r--r--   0 hamid      (501) staff       (20)     1963 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.432919 xbrl-us-0.0.2/docs/
+-rw-r--r--   0 hamid      (501) staff       (20)       28 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/docs/authors.rst
+-rw-r--r--   0 hamid      (501) staff       (20)       30 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/docs/changelog.rst
+-rw-r--r--   0 hamid      (501) staff       (20)     1155 2023-07-14 15:47:57.000000 xbrl-us-0.0.2/docs/conf.py
+-rw-r--r--   0 hamid      (501) staff       (20)       33 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/docs/contributing.rst
+-rw-r--r--   0 hamid      (501) staff       (20)      219 2023-07-09 12:54:31.000000 xbrl-us-0.0.2/docs/index.rst
+-rw-r--r--   0 hamid      (501) staff       (20)       27 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/docs/readme.rst
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.433620 xbrl-us-0.0.2/docs/reference/
+-rw-r--r--   0 hamid      (501) staff       (20)       59 2023-07-09 15:02:31.000000 xbrl-us-0.0.2/docs/reference/index.rst
+-rw-r--r--   0 hamid      (501) staff       (20)       98 2023-07-09 15:02:46.000000 xbrl-us-0.0.2/docs/reference/xbrl_us.rst
+-rw-r--r--   0 hamid      (501) staff       (20)       35 2023-07-09 00:13:53.000000 xbrl-us-0.0.2/docs/requirements.txt
+-rw-r--r--   0 hamid      (501) staff       (20)      109 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/docs/spelling_wordlist.txt
+-rw-r--r--   0 hamid      (501) staff       (20)     1194 2023-07-12 22:49:38.000000 xbrl-us-0.0.2/pyproject.toml
+-rw-r--r--   0 hamid      (501) staff       (20)      772 2023-06-26 21:38:04.000000 xbrl-us-0.0.2/pytest.ini
+-rw-r--r--   0 hamid      (501) staff       (20)       38 2023-07-14 15:48:31.471122 xbrl-us-0.0.2/setup.cfg
+-rwxr-xr-x   0 hamid      (501) staff       (20)     2930 2023-07-14 15:47:57.000000 xbrl-us-0.0.2/setup.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.422065 xbrl-us-0.0.2/src/
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.435628 xbrl-us-0.0.2/src/xbrl_us/
+-rw-r--r--   0 hamid      (501) staff       (20)       69 2023-07-14 15:47:57.000000 xbrl-us-0.0.2/src/xbrl_us/__init__.py
+-rw-r--r--   0 hamid      (501) staff       (20)      372 2023-07-12 22:27:55.000000 xbrl-us-0.0.2/src/xbrl_us/__main__.py
+-rw-r--r--   0 hamid      (501) staff       (20)    15086 2023-07-14 15:26:16.000000 xbrl-us-0.0.2/src/xbrl_us/app.py
+-rw-r--r--   0 hamid      (501) staff       (20)      373 2023-07-12 22:49:38.000000 xbrl-us-0.0.2/src/xbrl_us/cli.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.459478 xbrl-us-0.0.2/src/xbrl_us/methods/
+-rw-r--r--   0 hamid      (501) staff       (20)      964 2023-07-10 12:13:32.000000 xbrl-us-0.0.2/src/xbrl_us/methods/assertion search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      297 2023-07-10 18:27:24.000000 xbrl-us-0.0.2/src/xbrl_us/methods/assertion validate.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1002 2023-07-10 12:13:32.000000 xbrl-us-0.0.2/src/xbrl_us/methods/concept name search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1555 2023-07-10 12:13:32.000000 xbrl-us-0.0.2/src/xbrl_us/methods/concept search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1077 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/cube search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      964 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/dimension search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      672 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/document search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      480 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/dts id concept label.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      870 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/dts id concept name.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      589 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/dts id concept reference.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      953 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/dts id concept search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1270 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/dts id network search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      850 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/dts id network.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      525 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/dts search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1229 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/entity id report search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      343 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/entity id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1273 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/entity report search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      387 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/entity search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1552 2023-07-10 19:53:06.000000 xbrl-us-0.0.2/src/xbrl_us/methods/fact id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      960 2023-07-10 19:53:06.000000 xbrl-us-0.0.2/src/xbrl_us/methods/fact search oim.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     9191 2023-07-13 13:17:04.000000 xbrl-us-0.0.2/src/xbrl_us/methods/fact search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      519 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/label dts id search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      510 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/label search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1332 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/network id relationship search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      394 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/network id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1319 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/network relationship search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1323 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/relationship search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      956 2023-07-10 12:16:52.000000 xbrl-us-0.0.2/src/xbrl_us/methods/relationship tree search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     2923 2023-07-10 21:15:17.000000 xbrl-us-0.0.2/src/xbrl_us/methods/report fact search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)       99 2023-07-10 19:53:06.000000 xbrl-us-0.0.2/src/xbrl_us/methods/report id delete.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     2743 2023-07-10 20:49:26.000000 xbrl-us-0.0.2/src/xbrl_us/methods/report id fact search.yml
+-rw-r--r--   0 hamid      (501) staff       (20)      731 2023-07-10 20:05:31.000000 xbrl-us-0.0.2/src/xbrl_us/methods/report id.yml
+-rw-r--r--   0 hamid      (501) staff       (20)     1150 2023-07-10 19:53:06.000000 xbrl-us-0.0.2/src/xbrl_us/methods/report search.yml
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.466346 xbrl-us-0.0.2/src/xbrl_us/schemas/
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:52:58.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/__init__.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:14.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/assertion_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)     5257 2023-07-07 22:17:57.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/concept_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:14.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/cube_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)     1501 2023-07-07 22:17:57.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/dimension_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:36.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/document_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:29.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/dts_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:05.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/entity_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-07-05 15:56:32.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/fact_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:47.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/label_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:42:54.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/network_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:43:04.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/relationship_details.py
+-rw-r--r--   0 hamid      (501) staff       (20)        0 2023-06-26 23:41:48.000000 xbrl-us-0.0.2/src/xbrl_us/schemas/report_details.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.468644 xbrl-us-0.0.2/src/xbrl_us/utils/
+-rw-r--r--   0 hamid      (501) staff       (20)       97 2023-07-10 21:39:35.000000 xbrl-us-0.0.2/src/xbrl_us/utils/__init__.py
+-rw-r--r--   0 hamid      (501) staff       (20)     1377 2023-07-12 17:14:14.000000 xbrl-us-0.0.2/src/xbrl_us/utils/exceptions.py
+-rw-r--r--   0 hamid      (501) staff       (20)      464 2023-07-08 23:56:22.000000 xbrl-us-0.0.2/src/xbrl_us/utils/fields.py
+-rw-r--r--   0 hamid      (501) staff       (20)    26377 2023-07-07 22:12:20.000000 xbrl-us-0.0.2/src/xbrl_us/utils/paramters.py
+-rw-r--r--   0 hamid      (501) staff       (20)    26440 2023-07-14 15:15:23.000000 xbrl-us-0.0.2/src/xbrl_us/xbrl_us.py
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.439068 xbrl-us-0.0.2/src/xbrl_us.egg-info/
+-rw-r--r--   0 hamid      (501) staff       (20)     9385 2023-07-14 15:48:31.000000 xbrl-us-0.0.2/src/xbrl_us.egg-info/PKG-INFO
+-rw-r--r--   0 hamid      (501) staff       (20)     2915 2023-07-14 15:48:31.000000 xbrl-us-0.0.2/src/xbrl_us.egg-info/SOURCES.txt
+-rw-r--r--   0 hamid      (501) staff       (20)        1 2023-07-14 15:48:31.000000 xbrl-us-0.0.2/src/xbrl_us.egg-info/dependency_links.txt
+-rw-r--r--   0 hamid      (501) staff       (20)       45 2023-07-14 15:48:31.000000 xbrl-us-0.0.2/src/xbrl_us.egg-info/entry_points.txt
+-rw-r--r--   0 hamid      (501) staff       (20)        1 2023-07-12 23:37:24.000000 xbrl-us-0.0.2/src/xbrl_us.egg-info/not-zip-safe
+-rw-r--r--   0 hamid      (501) staff       (20)       88 2023-07-14 15:48:31.000000 xbrl-us-0.0.2/src/xbrl_us.egg-info/requires.txt
+-rw-r--r--   0 hamid      (501) staff       (20)        8 2023-07-14 15:48:31.000000 xbrl-us-0.0.2/src/xbrl_us.egg-info/top_level.txt
+drwxr-xr-x   0 hamid      (501) staff       (20)        0 2023-07-14 15:48:31.469412 xbrl-us-0.0.2/tests/
+-rw-r--r--   0 hamid      (501) staff       (20)      515 2023-07-12 23:36:14.000000 xbrl-us-0.0.2/tests/test_xbrl_us.py
+-rw-r--r--   0 hamid      (501) staff       (20)     1572 2023-07-12 22:40:42.000000 xbrl-us-0.0.2/tox.ini
```

### Comparing `xbrl-us-0.0.1/.bumpversion.cfg` & `xbrl-us-0.0.2/.bumpversion.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.0.1
+current_version = 0.0.2
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `xbrl-us-0.0.1/.cookiecutterrc` & `xbrl-us-0.0.2/.cookiecutterrc`

 * *Files 0% similar despite different names*

```diff
@@ -50,12 +50,12 @@
     scrutinizer: "no"
     setup_py_uses_setuptools_scm: "no"
     sphinx_docs: "yes"
     sphinx_docs_hosting: "https://python-xbrl-us.readthedocs.io/"
     sphinx_doctest: "no"
     sphinx_theme: "furo"
     test_matrix_separate_coverage: "no"
-    version: "0.0.1"
+    version: "0.0.2"
     version_manager: "bump2version"
     website: "https://hamidvakilzadeh.com"
     year_from: "2023"
     year_to: "2023"
```

### Comparing `xbrl-us-0.0.1/.github/workflows/github-actions.yml` & `xbrl-us-0.0.2/.github/workflows/github-actions.yml`

 * *Files 12% similar despite different names*

```diff
@@ -19,32 +19,14 @@
             tox_env: 'check'
             os: 'ubuntu-latest'
           - name: 'docs'
             python: '3.11'
             toxpython: 'python3.11'
             tox_env: 'docs'
             os: 'ubuntu-latest'
-          - name: 'py37 (ubuntu)'
-            python: '3.7'
-            toxpython: 'python3.7'
-            python_arch: 'x64'
-            tox_env: 'py37'
-            os: 'ubuntu-latest'
-          - name: 'py37 (windows)'
-            python: '3.7'
-            toxpython: 'python3.7'
-            python_arch: 'x64'
-            tox_env: 'py37'
-            os: 'windows-latest'
-          - name: 'py37 (macos)'
-            python: '3.7'
-            toxpython: 'python3.7'
-            python_arch: 'x64'
-            tox_env: 'py37'
-            os: 'macos-latest'
           - name: 'py38 (ubuntu)'
             python: '3.8'
             toxpython: 'python3.8'
             python_arch: 'x64'
             tox_env: 'py38'
             os: 'ubuntu-latest'
           - name: 'py38 (windows)'
@@ -109,32 +91,14 @@
             os: 'windows-latest'
           - name: 'py311 (macos)'
             python: '3.11'
             toxpython: 'python3.11'
             python_arch: 'x64'
             tox_env: 'py311'
             os: 'macos-latest'
-          - name: 'pypy37 (ubuntu)'
-            python: 'pypy-3.7'
-            toxpython: 'pypy3.7'
-            python_arch: 'x64'
-            tox_env: 'pypy37'
-            os: 'ubuntu-latest'
-          - name: 'pypy37 (windows)'
-            python: 'pypy-3.7'
-            toxpython: 'pypy3.7'
-            python_arch: 'x64'
-            tox_env: 'pypy37'
-            os: 'windows-latest'
-          - name: 'pypy37 (macos)'
-            python: 'pypy-3.7'
-            toxpython: 'pypy3.7'
-            python_arch: 'x64'
-            tox_env: 'pypy37'
-            os: 'macos-latest'
           - name: 'pypy38 (ubuntu)'
             python: 'pypy-3.8'
             toxpython: 'pypy3.8'
             python_arch: 'x64'
             tox_env: 'pypy38'
             os: 'ubuntu-latest'
           - name: 'pypy38 (windows)'
```

### Comparing `xbrl-us-0.0.1/.pre-commit-config.yaml` & `xbrl-us-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.1/CONTRIBUTING.rst` & `xbrl-us-0.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.1/LICENSE` & `xbrl-us-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.1/PKG-INFO` & `xbrl-us-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbrl-us
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper for xbrl.us API
 Home-page: https://github.com/hamid-vakilzadeh/python-xbrl-us
 Author: hamid-vakilzadeh
 Author-email: vakilzas@uww.edu
 License: MIT
 Project-URL: Documentation, https://python-xbrl-us.readthedocs.io/
 Project-URL: Changelog, https://python-xbrl-us.readthedocs.io/en/latest/changelog.html
@@ -43,51 +43,64 @@
 
 It's important to note that while the XBRL US Python Wrapper is free and distributed under the permissive MIT license,
 the usage of the underlying XBRL US API is subject to the policies and terms defined by XBRL US.
 These policies govern the access, usage, and restrictions imposed on the API data and services.
 Users of the XBRL US Python Wrapper should review and comply with the XBRL US policies to ensure appropriate
 usage of the API and adherence to any applicable licensing terms.
 
-If you are utilizing the XBRL US Python Wrapper for research purposes, we kindly request that you cite the following paper:
+.. important::
 
-[FILL: Insert Paper Title]
+    Any and all use of the XBRL APIs to return
+    data from the XBRL US Database of Public Filings is in explicit consent and
+    agreement with the `XBRL API Terms of Agreement <https://xbrl.us/home/about/legal/xbrl-api-clientid/>`_.
 
-[FILL: Authors]
+.. note::
+    If you are utilizing the XBRL US Python Wrapper for research purposes, we kindly request that you cite the following paper:
 
-[FILL: Publication Details]
+    [FILL: Insert Paper Title]
 
+    [FILL: Authors]
+
+    [FILL: Publication Details]
 
 
 Tutorial ✏️📖📚
 ================
 
 This tutorial will guide you through using the XBRL-US Python library to interact with the XBRL API. The XBRL-US library provides a convenient way to query and retrieve financial data from the XBRL API using Python.
 
 Prerequisites
 ~~~~~~~~~~~~~
 
 Before you begin, ensure you have the following:
 
 * **Python installed on your system**.
   Right now, the XBRL-US library supports Python 3.10 and above.
-  Backwards compatibility with Python 3.7 and above is planned for a future release.
+  Backwards compatibility with Python 3.8 and above is planned for a future release.
 * **XBRL-US library installed**.
 * **XBRL-US API credentials**.
   You can obtain your credentials by registering for a
   free XBRL-US account at https://xbrl.us/home/use/xbrl-api/.
 * **XBRL-US OAuth2 Access**.
   You can obtain your client ID and client secret by registering for a
   free XBRL-US account at https://xbrl.us/home/use/xbrl-api/access-token/.
 
 You can install it using pip:
 
 .. code-block:: bash
 
     pip install xbrl-us
 
+.. caution::
+
+        The XBRL US Python Wrapper is currently in beta and is subject to change.
+        We welcome your feedback and suggestions for improvement.
+        Please submit any issues or feature requests to
+        the `GitHub repository <https://github.com/hamid-vakilzadeh/python-xbrl-us/issues>`_.
+
 
 **Documentation**
 
 For detailed information about the XBRL-US Python
 library, you can refer to the documentation at https://python-xbrl-us.readthedocs.io/en/latest/.
 
 **Official Documentation**
@@ -154,15 +167,15 @@
             'fact.value',
             'fact.id',
             'entity.id',
             'entity.cik',
             'entity.name',
             'report.sic-code',
         ],
-        limit={'fact': 100},
+        limit=100,
         as_dataframe=True
     )
 
 In this example, we are searching for facts related
 to specific concepts, fiscal years, and SIC codes.
 We are also specifying the fields we want to retrieve
 in the response. The ``limit`` parameter restricts the
@@ -198,15 +211,15 @@
             Fields.FACT_VALUE,
             Fields.FACT_ID,
             Fields.ENTITY_ID,
             Fields.ENTITY_CIK,
             Fields.ENTITY_NAME,
             Fields.REPORT_SIC_CODE,
         ],
-        limit={'fact': 100},
+        limit=100,
         as_dataframe=True
     )
 
 
 This alternative approach also allows you to
 take advantage of the autocomplete feature of your IDE to
 easily find the parameters and fields.
@@ -269,11 +282,23 @@
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
 
-0.0.0 (2023-06-26)
+0.0.2 (2023-07-12)
+~~~~~~~~~~~~~~~~~~
+
+
+* Bug fixes
+* Enhanced error handling
+* Improved method attributes
+* Added the ability to print the query string
+* Implemented a feature to handle queries with large limits
+* NEW: Introduced a web interface for the API, making it even easier to use
+
+
+0.0.1 (2023-07-09)
 ~~~~~~~~~~~~~~~~~~
 
 * First release on PyPI.
```

### Comparing `xbrl-us-0.0.1/README.rst` & `xbrl-us-0.0.2/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -13,51 +13,64 @@
 
 It's important to note that while the XBRL US Python Wrapper is free and distributed under the permissive MIT license,
 the usage of the underlying XBRL US API is subject to the policies and terms defined by XBRL US.
 These policies govern the access, usage, and restrictions imposed on the API data and services.
 Users of the XBRL US Python Wrapper should review and comply with the XBRL US policies to ensure appropriate
 usage of the API and adherence to any applicable licensing terms.
 
-If you are utilizing the XBRL US Python Wrapper for research purposes, we kindly request that you cite the following paper:
+.. important::
 
-[FILL: Insert Paper Title]
+    Any and all use of the XBRL APIs to return
+    data from the XBRL US Database of Public Filings is in explicit consent and
+    agreement with the `XBRL API Terms of Agreement <https://xbrl.us/home/about/legal/xbrl-api-clientid/>`_.
 
-[FILL: Authors]
+.. note::
+    If you are utilizing the XBRL US Python Wrapper for research purposes, we kindly request that you cite the following paper:
 
-[FILL: Publication Details]
+    [FILL: Insert Paper Title]
 
+    [FILL: Authors]
+
+    [FILL: Publication Details]
 
 
 Tutorial ✏️📖📚
 ================
 
 This tutorial will guide you through using the XBRL-US Python library to interact with the XBRL API. The XBRL-US library provides a convenient way to query and retrieve financial data from the XBRL API using Python.
 
 Prerequisites
 ~~~~~~~~~~~~~
 
 Before you begin, ensure you have the following:
 
 * **Python installed on your system**.
   Right now, the XBRL-US library supports Python 3.10 and above.
-  Backwards compatibility with Python 3.7 and above is planned for a future release.
+  Backwards compatibility with Python 3.8 and above is planned for a future release.
 * **XBRL-US library installed**.
 * **XBRL-US API credentials**.
   You can obtain your credentials by registering for a
   free XBRL-US account at https://xbrl.us/home/use/xbrl-api/.
 * **XBRL-US OAuth2 Access**.
   You can obtain your client ID and client secret by registering for a
   free XBRL-US account at https://xbrl.us/home/use/xbrl-api/access-token/.
 
 You can install it using pip:
 
 .. code-block:: bash
 
     pip install xbrl-us
 
+.. caution::
+
+        The XBRL US Python Wrapper is currently in beta and is subject to change.
+        We welcome your feedback and suggestions for improvement.
+        Please submit any issues or feature requests to
+        the `GitHub repository <https://github.com/hamid-vakilzadeh/python-xbrl-us/issues>`_.
+
 
 **Documentation**
 
 For detailed information about the XBRL-US Python
 library, you can refer to the documentation at https://python-xbrl-us.readthedocs.io/en/latest/.
 
 **Official Documentation**
@@ -124,15 +137,15 @@
             'fact.value',
             'fact.id',
             'entity.id',
             'entity.cik',
             'entity.name',
             'report.sic-code',
         ],
-        limit={'fact': 100},
+        limit=100,
         as_dataframe=True
     )
 
 In this example, we are searching for facts related
 to specific concepts, fiscal years, and SIC codes.
 We are also specifying the fields we want to retrieve
 in the response. The ``limit`` parameter restricts the
@@ -168,15 +181,15 @@
             Fields.FACT_VALUE,
             Fields.FACT_ID,
             Fields.ENTITY_ID,
             Fields.ENTITY_CIK,
             Fields.ENTITY_NAME,
             Fields.REPORT_SIC_CODE,
         ],
-        limit={'fact': 100},
+        limit=100,
         as_dataframe=True
     )
 
 
 This alternative approach also allows you to
 take advantage of the autocomplete feature of your IDE to
 easily find the parameters and fields.
```

### Comparing `xbrl-us-0.0.1/ci/bootstrap.py` & `xbrl-us-0.0.2/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.1/ci/templates/.github/workflows/github-actions.yml` & `xbrl-us-0.0.2/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.1/docs/conf.py` & `xbrl-us-0.0.2/docs/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "xbrl-us"
 year = "2023"
 author = "hamid-vakilzadeh"
 copyright = f"{year}, {author}"
-version = release = "0.0.1"
+version = release = "0.0.2"
 
 pygments_style = "emacs"
 highlight_language = "python"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/hamid-vakilzadeh/python-xbrl-us/issues/%s", "#"),
     "pr": ("https://github.com/hamid-vakilzadeh/python-xbrl-us/pull/%s", "PR #"),
```

### Comparing `xbrl-us-0.0.1/pyproject.toml` & `xbrl-us-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -33,20 +33,20 @@
     "RSE", # flake8-raise
     "RUF", # ruff-specific rules
     "S", # flake8-bandit
     "UP", # pyupgrade
     "W", # pycodestyle warnings
 ]
 src = ["src", "tests"]
-target-version = "py37"
+target-version = "py38"
 
 [tool.ruff.flake8-pytest-style]
 fixture-parentheses = false
 mark-parentheses = false
 
 [tool.ruff.isort]
 forced-separate = ["conftest"]
 force-single-line = true
 
 [tool.black]
 line-length = 140
-target-version = ["py37"]
+target-version = ["py38"]
```

### Comparing `xbrl-us-0.0.1/pytest.ini` & `xbrl-us-0.0.2/pytest.ini`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.1/setup.py` & `xbrl-us-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(*names, **kwargs):
     with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
     name="xbrl-us",
-    version="0.0.1",
+    version="0.0.2",
     license="MIT",
     description="Python wrapper for xbrl.us API",
     long_description_content_type="text/x-rst",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
@@ -58,15 +58,15 @@
         "Changelog": "https://python-xbrl-us.readthedocs.io/en/latest/changelog.html",
         "Issue Tracker": "https://github.com/hamid-vakilzadeh/python-xbrl-us/issues",
     },
     keywords=[
         # eg: "xbrl-us", "xbrl", "sec",
     ],
     python_requires=">=3.10",
-    install_requires=["requests>=2.25.1", "pandas>=1.2.4", "PyYAML>=5.3", "sphinx-copybutton"],
+    install_requires=["requests>=2.25.1", "pandas>=1.2.4", "PyYAML>=5.3", "sphinx-copybutton", "streamlit", "retry", "tqdm", "stqdm"],
     extras_require={
         # eg:
         #   "rst": ["docutils>=0.11"],
         #   ":python_version=="2.6"": ["argparse"],
     },
     entry_points={
         "console_scripts": [
```

### Comparing `xbrl-us-0.0.1/src/xbrl_us/methods/assertion search.yml` & `xbrl-us-0.0.2/src/xbrl_us/methods/assertion search.yml`

 * *Files 7% similar despite different names*

```diff
@@ -31,13 +31,25 @@
   - report.entry-url
   - report.filing-date
   - report.filing-year
   - report.id
   - report.sec-url
   - report.sic-code
 limit:
-  -
+  - assertion
+  - concept
+  - cube
+  - dimension
+  - document
+  - dts
+  - entity
+  - fact
+  - label
+  - network
+  - reference
+  - relationship
+  - report
 sort:
   -
 offset:
   -
 url: /api/v1/assertion/search
```

### Comparing `xbrl-us-0.0.1/src/xbrl_us/methods/concept name search.yml` & `xbrl-us-0.0.2/src/xbrl_us/methods/dts id concept search.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 parameters:
-  - concept.local-name
+  - dts.id *
   - concept.id
+  - concept.local-name
   - concept.namespace
   - dts.entry-point
   - dts.hash
-  - dts.id
   - dts.target-namespace
 fields:
   - concept.balance-type
   - concept.datatype
   - concept.id
   - concept.is-abstract
   - concept.is-monetary
@@ -18,31 +18,40 @@
   - concept.namespace
   - concept.period-type
   - concept.substitution
   - dts.id
   - dts.entry-point
   - dts.hash
   - dts.target-namespace
-  - concept.*
   - label.id
   - label.text
   - label.lang
   - label.role
   - label.role-short
-  - label.*
-  - reference.id
   - reference.role
   - reference.role-definition
   - reference.role-short
-  - reference.*
   - parts.local-name
   - parts.namespace
   - parts.order
   - parts.part-value
-  - parts.*
+  - reference.id
+  - parts.
 limit:
-  -
+  - assertion
+  - concept
+  - cube
+  - dimension
+  - document
+  - dts
+  - entity
+  - fact
+  - label
+  - network
+  - reference
+  - relationship
+  - report
 sort:
   -
 offset:
   -
-url: /api/v1/concept/{concept.local-name}/search
+url: /api/v1/dts/{dts.id}/concept/search
```

### Comparing `xbrl-us-0.0.1/src/xbrl_us/methods/concept search.yml` & `xbrl-us-0.0.2/src/xbrl_us/methods/concept search.yml`

 * *Files 13% similar despite different names*

```diff
@@ -36,13 +36,52 @@
   - parts.local-name
   - parts.namespace
   - parts.order
   - parts.part-value
   - reference.id
   - parts.*
 limit:
-  -
+  - assertion
+  - concept
+  - cube
+  - dimension
+  - document
+  - dts
+  - entity
+  - fact
+  - label
+  - network
+  - reference
+  - relationship
+  - report
 sort:
-  -
+  - concept.balance-type
+  - concept.datatype
+  - concept.id
+  - concept.is-abstract
+  - concept.is-monetary
+  - concept.is-nillable
+  - concept.is-numeric
+  - concept.local-name
+  - concept.namespace
+  - concept.period-type
+  - concept.substitution
+  - dts.id
+  - dts.entry-point
+  - dts.hash
+  - dts.target-namespace
+  - label.id
+  - label.text
+  - label.lang
+  - label.role
+  - label.role-short
+  - reference.role
+  - reference.role-definition
+  - reference.role-short
+  - parts.local-name
+  - parts.namespace
+  - parts.order
+  - parts.part-value
+  - reference.id
 offset:
-  -
+  - concept.id
 url: /api/v1/concept/search
```

### Comparing `xbrl-us-0.0.1/src/xbrl_us/methods/cube search.yml` & `xbrl-us-0.0.2/src/xbrl_us/methods/cube search.yml`

 * *Files 18% similar despite different names*

```diff
@@ -40,13 +40,25 @@
   - period.fiscal-year
   - period.year
   - report.accession
   - report.id
   - unit
   - cube.*
 limit:
-  -
+  - assertion
+  - concept
+  - cube
+  - dimension
+  - document
+  - dts
+  - entity
+  - fact
+  - label
+  - network
+  - reference
+  - relationship
+  - report
 sort:
   -
 offset:
   -
 url: /api/v1/cube/search
```

### Comparing `xbrl-us-0.0.1/src/xbrl_us/methods/dts id concept name.yml` & `xbrl-us-0.0.2/src/xbrl_us/methods/dts id concept name.yml`

 * *Files 19% similar despite different names*

```diff
@@ -28,13 +28,25 @@
   - parts.local-name
   - parts.namespace
   - parts.order
   - parts.part-value
   - reference.id
   - parts.
 limit:
-  -
+  - assertion
+  - concept
+  - cube
+  - dimension
+  - document
+  - dts
+  - entity
+  - fact
+  - label
+  - network
+  - reference
+  - relationship
+  - report
 sort:
   -
 offset:
   -
 url: /api/v1/dts/{dts.id}/concept/{concept.local-name}
```

### Comparing `xbrl-us-0.0.1/src/xbrl_us/methods/dts id concept search.yml` & `xbrl-us-0.0.2/src/xbrl_us/methods/concept name search.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 parameters:
-  - dts.id *
-  - concept.id
   - concept.local-name
+  - concept.id
   - concept.namespace
   - dts.entry-point
   - dts.hash
+  - dts.id
   - dts.target-namespace
 fields:
   - concept.balance-type
   - concept.datatype
   - concept.id
   - concept.is-abstract
   - concept.is-monetary
@@ -18,28 +18,43 @@
   - concept.namespace
   - concept.period-type
   - concept.substitution
   - dts.id
   - dts.entry-point
   - dts.hash
   - dts.target-namespace
+  - concept.*
   - label.id
   - label.text
   - label.lang
   - label.role
   - label.role-short
+  - label.*
+  - reference.id
   - reference.role
   - reference.role-definition
   - reference.role-short
+  - reference.*
   - parts.local-name
   - parts.namespace
   - parts.order
   - parts.part-value
-  - reference.id
-  - parts.
+  - parts.*
 limit:
-  -
+  - assertion
+  - concept
+  - cube
+  - dimension
+  - document
+  - dts
+  - entity
+  - fact
+  - label
+  - network
+  - reference
+  - relationship
+  - report
 sort:
   -
 offset:
   -
-url: /api/v1/dts/{dts.id}/concept/search
+url: /api/v1/concept/{concept.local-name}/search
```

### Comparing `xbrl-us-0.0.1/src/xbrl_us/methods/dts id network search.yml` & `xbrl-us-0.0.2/src/xbrl_us/methods/network id relationship search.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 parameters:
-  - dts.id
   - network.id
-  - network.role-uri
+  - dts.entry-point
+  - dts.id
   - network.arcrole-uri
   - network.link-name
+  - network.role-description
+  - network.role-uri
   - relationship.id
   - relationship.order
   - relationship.preferred-label
   - relationship.source-concept-id
   - relationship.source-name
   - relationship.source-namespace
   - relationship.target-concept-id
@@ -35,13 +37,25 @@
   - relationship.target-is-abstract
   - relationship.target-name
   - relationship.target-namespace
   - relationship.tree-depth
   - relationship.tree-sequence
   - relationship.weight
 limit:
-  -
+  - assertion
+  - concept
+  - cube
+  - dimension
+  - document
+  - dts
+  - entity
+  - fact
+  - label
+  - network
+  - reference
+  - relationship
+  - report
 sort:
   -
 offset:
   -
-url: /api/v1/dts/{dts.id}/network/search
+url: /api/v1/network/{network.id}/relationship/search
```

### Comparing `xbrl-us-0.0.1/src/xbrl_us/methods/dts id network.yml` & `xbrl-us-0.0.2/src/xbrl_us/methods/dts id network.yml`

 * *Files 4% similar despite different names*

```diff
@@ -20,13 +20,25 @@
   - relationship.target-is-abstract
   - relationship.target-name
   - relationship.target-namespace
   - relationship.tree-depth
   - relationship.tree-sequence
   - relationship.weight
 limit:
-  -
+  - assertion
+  - concept
+  - cube
+  - dimension
+  - document
+  - dts
+  - entity
+  - fact
+  - label
+  - network
+  - reference
+  - relationship
+  - report
 sort:
   -
 offset:
   -
 url: /api/v1/dts/{dts.id}/network
```

### Comparing `xbrl-us-0.0.1/src/xbrl_us/methods/entity id report search.yml` & `xbrl-us-0.0.2/src/xbrl_us/methods/report search.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 parameters:
+  - dts.id
+  - entity.cik
   - entity.id
-  - report.source-id
-  - report.source-name
+  - entity.ticker
   - report.accession
-  - report.id
   - report.document-type
+  - report.document-index
+  - report.entity-name
   - report.entry-type
   - report.entry-url
   - report.filer-category
+  - report.id
   - report.is-most-current
   - report.period-index
   - report.restated
   - report.restated-index
   - report.sec-url
   - report.sic-code
+  - report.source-id
+  - report.source-name
 fields:
   - entity.cik
   - entity.id
-  - entity.name
-  - entity.scheme
   - entity.ticker
   - dts.id
   - report.accepted-timestamp
   - report.accession
   - report.address
   - report.base-taxonomy
   - report.creation-software
   - report.document-type
+  - report.document-index
   - report.entity-name
   - report.entry-type
   - report.entry-url
   - report.filer-category
   - report.filing-date
   - report.id
   - report.is-most-current
@@ -41,15 +45,13 @@
   - report.restated
   - report.restated-index
   - report.sec-url
   - report.sic-code
   - report.source-id
   - report.source-name
   - report.state-of-incorporation
-  - report.
+  - report.*
 limit:
-  -
-sort:
-  -
+  - report
 offset:
-  -
-url: /api/v1/entity/{entity.id}/report/search
+  - report
+url: /api/v1/report/search
```

### Comparing `xbrl-us-0.0.1/src/xbrl_us/methods/fact id.yml` & `xbrl-us-0.0.2/src/xbrl_us/methods/fact id.yml`

 * *Files 8% similar despite different names*

```diff
@@ -71,13 +71,9 @@
   - report.type
   - unit
   - unit.denominator
   - unit.numerator
   - unit.qname
   - fact.*
 limit:
-  - fact
-sort:
-  - fact
 offset:
-  - fact
 url: /api/v1/fact/{fact.id}
```

### Comparing `xbrl-us-0.0.1/src/xbrl_us/methods/fact search oim.yml` & `xbrl-us-0.0.2/src/xbrl_us/methods/fact search oim.yml`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,12 @@
   - report.restated-index
   - report.sec-url
   - report.sic-code
   - report.source-id
   - report.source-name
   - unit
 fields:
-  -
 limit:
-  -
-sort:
-  -
+  - fact
 offset:
   -
 url: /api/v1/fact/oim/search
```

### Comparing `xbrl-us-0.0.1/src/xbrl_us/methods/fact search.yml` & `xbrl-us-0.0.2/src/xbrl_us/methods/report id fact search.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 parameters:
+  - report.id
   - concept.id
   - concept.is-base
   - concept.is-monetary
   - concept.local-name
   - concept.namespace
   - dimension.is-base
   - dimension.local-name
@@ -32,18 +33,15 @@
   - period.fiscal-id
   - period.fiscal-period
   - period.fiscal-year
   - period.id
   - period.year
   - report.accession
   - report.creation-software
-  - report.document-type
-  - report.document-index
   - report.entry-url
-  - report.id
   - report.restated
   - report.restated-index
   - report.sec-url
   - report.sic-code
   - report.source-id
   - report.source-name
   - unit
@@ -96,34 +94,43 @@
   - period.fiscal-id
   - period.fiscal-period
   - period.fiscal-year
   - period.id
   - period.instant
   - period.start
   - period.year
+  - report.accepted-timestamp
   - report.accession
+  - report.address
+  - report.base-taxonomy
   - report.creation-software
   - report.document-type
   - report.document-index
+  - report.entity-name
+  - report.entry-type
   - report.entry-url
+  - report.filer-category
   - report.filing-date
   - report.id
+  - report.is-most-current
   - report.period-end
+  - report.period-index
+  - report.phone
+  - report.properties
   - report.restated
   - report.restated-index
   - report.sec-url
   - report.sic-code
   - report.source-id
   - report.source-name
-  - report.type
+  - report.state-of-incorporation
+  - report.*
   - unit
   - unit.denominator
   - unit.numerator
   - unit.qname
   - fact.*
 limit:
   - fact
-sort:
-  - fact
 offset:
   - fact
-url: /api/v1/fact/search
+url: /api/v1/report/{report.id}/fact/search
```

### Comparing `xbrl-us-0.0.1/src/xbrl_us/methods/network id relationship search.yml` & `xbrl-us-0.0.2/src/xbrl_us/methods/network relationship search.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 parameters:
-  - network.id
   - dts.entry-point
   - dts.id
   - network.arcrole-uri
+  - network.id
   - network.link-name
   - network.role-description
   - network.role-uri
   - relationship.id
   - relationship.order
   - relationship.preferred-label
   - relationship.source-concept-id
@@ -37,13 +37,25 @@
   - relationship.target-is-abstract
   - relationship.target-name
   - relationship.target-namespace
   - relationship.tree-depth
   - relationship.tree-sequence
   - relationship.weight
 limit:
-  -
+  - assertion
+  - concept
+  - cube
+  - dimension
+  - document
+  - dts
+  - entity
+  - fact
+  - label
+  - network
+  - reference
+  - relationship
+  - report
 sort:
   -
 offset:
   -
-url: /api/v1/network/{network.id}/relationship/search
+url: /api/v1/network/relationship/search
```

### Comparing `xbrl-us-0.0.1/src/xbrl_us/methods/network relationship search.yml` & `xbrl-us-0.0.2/src/xbrl_us/methods/relationship search.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 parameters:
-  - dts.entry-point
   - dts.id
   - network.arcrole-uri
   - network.id
   - network.link-name
   - network.role-description
   - network.role-uri
   - relationship.id
   - relationship.order
   - relationship.preferred-label
   - relationship.source-concept-id
   - relationship.source-name
   - relationship.source-namespace
   - relationship.target-concept-id
+  - relationship.target-is-abstract
   - relationship.target-name
   - relationship.target-namespace
   - relationship.tree-depth
   - relationship.tree-sequence
+  - stringmatch
 fields:
-  - dts.entry-point
   - dts.id
   - network.arcrole-uri
   - network.id
   - network.link-name
   - network.role-description
   - network.role-uri
   - relationship.id
@@ -37,13 +37,25 @@
   - relationship.target-is-abstract
   - relationship.target-name
   - relationship.target-namespace
   - relationship.tree-depth
   - relationship.tree-sequence
   - relationship.weight
 limit:
-  -
+  - assertion
+  - concept
+  - cube
+  - dimension
+  - document
+  - dts
+  - entity
+  - fact
+  - label
+  - network
+  - reference
+  - relationship
+  - report
 sort:
   -
 offset:
   -
-url: /api/v1/network/relationship/search
+url: /api/v1/relationship/search
```

### Comparing `xbrl-us-0.0.1/src/xbrl_us/methods/relationship tree search.yml` & `xbrl-us-0.0.2/src/xbrl_us/methods/relationship tree search.yml`

 * *Files 22% similar despite different names*

```diff
@@ -25,13 +25,25 @@
   - relationship.target-is-abstract
   - relationship.target-name
   - relationship.target-namespace
   - relationship.tree-depth
   - relationship.tree-sequence
   - relationship.weight
 limit:
-  -
+  - assertion
+  - concept
+  - cube
+  - dimension
+  - document
+  - dts
+  - entity
+  - fact
+  - label
+  - network
+  - reference
+  - relationship
+  - report
 sort:
   -
 offset:
   -
 url: /api/v1/relationship/tree/search
```

### Comparing `xbrl-us-0.0.1/src/xbrl_us/methods/report fact search.yml` & `xbrl-us-0.0.2/src/xbrl_us/methods/report fact search.yml`

 * *Files 16% similar despite different names*

```diff
@@ -49,15 +49,97 @@
   - report.restated
   - report.sec-url
   - report.sic-code
   - report.source-id
   - report.source-name
   - unit
 fields:
-  -
+  - concept.balance-type
+  - concept.datatype
+  - concept.id
+  - concept.is-base
+  - concept.is-monetary
+  - concept.local-name
+  - concept.namespace
+  - concept.period-type
+  - dimension.is-base
+  - dimension.local-name
+  - dimension.namespace
+  - dimensions
+  - dimensions.count
+  - dimensions.id
+  - dts.entry-point
+  - dts.id
+  - dts.target-namespace
+  - entity.cik
+  - entity.id
+  - entity.name
+  - entity.scheme
+  - fact.decimals
+  - fact.example
+  - fact.has-dimensions
+  - fact.hash
+  - fact.highlighted-value
+  - fact.id
+  - fact.inline-display-value
+  - fact.inline-is-hidden
+  - fact.inline-negated
+  - fact.inline-scale
+  - fact.is-extended
+  - fact.numerical-value
+  - fact.ultimus
+  - fact.ultimus-index
+  - fact.value
+  - fact.value-link
+  - fact.xml-id
+  - member.is-base
+  - member.local-name
+  - member.typed-value
+  - member.member-value
+  - member.namespace
+  - period.calendar-period
+  - period.end
+  - period.fiscal-id
+  - period.fiscal-period
+  - period.fiscal-year
+  - period.id
+  - period.instant
+  - period.start
+  - period.year
+  - report.accepted-timestamp
+  - report.accession
+  - report.address
+  - report.base-taxonomy
+  - report.creation-software
+  - report.document-type
+  - report.document-index
+  - report.entity-name
+  - report.entry-type
+  - report.entry-url
+  - report.filer-category
+  - report.filing-date
+  - report.id
+  - report.is-most-current
+  - report.period-end
+  - report.period-index
+  - report.phone
+  - report.properties
+  - report.restated
+  - report.restated-index
+  - report.sec-url
+  - report.sic-code
+  - report.source-id
+  - report.source-name
+  - report.state-of-incorporation
+  - report.*
+  - unit
+  - unit.denominator
+  - unit.numerator
+  - unit.qname
+  - fact.*
 limit:
-  -
-sort:
-  -
+  - fact
+  - report
 offset:
-  -
+  - fact
+  - report
 url: /api/v1/report/fact/search
```

### Comparing `xbrl-us-0.0.1/src/xbrl_us/methods/report id.yml` & `xbrl-us-0.0.2/src/xbrl_us/methods/report id.yml`

 * *Files 4% similar despite different names*

```diff
@@ -28,13 +28,9 @@
   - report.sec-url
   - report.sic-code
   - report.source-id
   - report.source-name
   - report.state-of-incorporation
   - report.*
 limit:
-  -
-sort:
-  -
 offset:
-  -
 url: /api/v1/report/{report.id}
```

### Comparing `xbrl-us-0.0.1/src/xbrl_us/methods/report search.yml` & `xbrl-us-0.0.2/src/xbrl_us/methods/entity report search.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 parameters:
-  - dts.id
   - entity.cik
   - entity.id
+  - report.entity-name
   - entity.ticker
+  - report.source-id
+  - report.source-name
   - report.accession
+  - report.id
   - report.document-type
-  - report.document-index
-  - report.entity-name
   - report.entry-type
   - report.entry-url
   - report.filer-category
-  - report.id
   - report.is-most-current
   - report.period-index
   - report.restated
   - report.restated-index
   - report.sec-url
   - report.sic-code
-  - report.source-id
-  - report.source-name
 fields:
   - entity.cik
   - entity.id
+  - entity.name
+  - entity.scheme
   - entity.ticker
   - dts.id
   - report.accepted-timestamp
   - report.accession
   - report.address
   - report.base-taxonomy
   - report.creation-software
   - report.document-type
-  - report.document-index
   - report.entity-name
   - report.entry-type
   - report.entry-url
   - report.filer-category
   - report.filing-date
   - report.id
   - report.is-most-current
@@ -45,15 +44,27 @@
   - report.restated
   - report.restated-index
   - report.sec-url
   - report.sic-code
   - report.source-id
   - report.source-name
   - report.state-of-incorporation
-  - report.*
+  - report.
 limit:
-  -
+  - assertion
+  - concept
+  - cube
+  - dimension
+  - document
+  - dts
+  - entity
+  - fact
+  - label
+  - network
+  - reference
+  - relationship
+  - report
 sort:
   -
 offset:
   -
-url: /api/v1/report/search
+url: /api/v1/entity/report/search
```

### Comparing `xbrl-us-0.0.1/src/xbrl_us/schemas/concept_details.py` & `xbrl-us-0.0.2/src/xbrl_us/schemas/concept_details.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.1/src/xbrl_us/schemas/dimension_details.py` & `xbrl-us-0.0.2/src/xbrl_us/schemas/dimension_details.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.1/src/xbrl_us/utils/paramters.py` & `xbrl-us-0.0.2/src/xbrl_us/utils/paramters.py`

 * *Files identical despite different names*

### Comparing `xbrl-us-0.0.1/src/xbrl_us/xbrl_us.py` & `xbrl-us-0.0.2/src/xbrl_us/xbrl_us.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+import logging
 import re
 import time
 import warnings
 from collections.abc import Iterable
 from functools import wraps
 from pathlib import Path
 from typing import Optional
 from typing import Union
 
 import requests
 from pandas import DataFrame
+from retry import retry
+from tqdm import tqdm
 from yaml import safe_load
 
 from .utils import Parameters
+from .utils import exceptions
+
+logging.basicConfig()
 
 _dir = Path(__file__).resolve()
 
 
 class XBRL:
     """
     XBRL US API client. Initializes an instance of XBRL authorized connection.
@@ -28,14 +34,16 @@
         grant_type (str): Used to identify which credentials the authorization server needs to check
 
             * client_credentials - Requires a client_id and client_secret only
             * password - Requires a username and password as well as client_id and client_secret
             * default - "password"
     """
 
+    _query_exceptions = (requests.exceptions.ConnectionError, requests.exceptions.Timeout, requests.exceptions.ReadTimeout)
+
     def __init__(
         self,
         client_id: str,
         client_secret: str,
         username: str,
         password: str,
         grant_type: str = "password",
@@ -44,14 +52,15 @@
         self.client_id = client_id
         self.client_secret = client_secret
         self.username = username
         self.password = password
         self.grant_type = grant_type
         self.access_token = None
         self.refresh_token = None
+        self.account_limit = None
         self._access_token_expires_at = 0
         self._refresh_token_expires_at = 0
 
     @staticmethod
     def acceptable_params(method_name: str):
         """
         Get the names of the attributes that are allowed to be used for
@@ -68,14 +77,16 @@
         with file_path.open("r") as file:
             method_features = safe_load(file)
 
         _attributes = {"method_name": method_name}
         for key, _value in method_features.items():
             _attributes[f"{key}"] = method_features.get(key)
 
+        _attributes["sort"] = [value for value in _attributes["fields"] if "*" not in value]
+
         # Create the dynamic class using type()
         _class = type(method_name, (), _attributes)
         return _class()
 
     @staticmethod
     def methods():
         """
@@ -154,28 +165,31 @@
 
         if response.status_code == 200:
             token_info = response.json()
             self.access_token = token_info["access_token"]
             self.refresh_token = token_info["refresh_token"]
             self._access_token_expires_at = time.time() + token_info["expires_in"]
             self._refresh_token_expires_at = time.time() + token_info["refresh_token_expires_in"]
+        else:
+            raise ValueError(f"Unable to retrieve token: {response.json()}. Please check your credentials.")
 
     def _is_access_token_expired(self):
         return time.time() >= self._access_token_expires_at
 
     def _is_refresh_token_expired(self):
         return time.time() >= self._refresh_token_expires_at
 
     def _ensure_access_token(self):
         if not self.access_token or self._is_access_token_expired():
             if self.refresh_token and not self._is_refresh_token_expired():
                 self._get_token(grant_type="refresh_token", refresh_token=self.refresh_token)
             else:
                 self._get_token()
 
+    @retry(exceptions=_query_exceptions, tries=3, delay=2, backoff=2)
     def _make_request(self, method, url, **kwargs) -> requests.Response:
         """
         Makes an HTTP request with the provided method, URL, and additional arguments.
 
         Args:
             method (str): The HTTP method for the request.
             url (str): The URL to send the request to.
@@ -189,199 +203,237 @@
         headers = kwargs.get("headers", {})
         headers.update({"Authorization": f"Bearer {self.access_token}"})
         kwargs["headers"] = headers
 
         response = requests.request(method, url, timeout=30, **kwargs)
         return response
 
+    def _get_account_limit(
+        self,
+        url: str,
+        params: dict,
+    ):
+        # Query the API with a limit of more than 5000.
+        fields = params["fields"]
+        new_fields = ",".join([fields, "fact.limit(5001)"])
+        params["fields"] = new_fields
+
+        response = self._make_request(
+            method="get",
+            url=url,
+            params=params,
+        )
+
+        # Extract the limit from the response message.
+        match = re.search(r"user limit amount is (\d+)", response.text)
+        if match:
+            self.account_limit = int(match.group(1))
+        else:
+            print(f"Error: {response.status_code}")
+            self.account_limit = None
+
+    @staticmethod
+    def _remove_special_fields(fields):
+        # Define the patterns to be removed
+        patterns = [r"(.+)\.(sort\((.+)\))?$", r"(.+)\.(limit\((\d+)\))?$", r"(.+)\.(offset\((\d+)\))?$"]
+
+        # For each field, check if it matches any of the patterns. If it does, remove it.
+        for field in fields[:]:  # iterate over a slice copy of the list to safely modify it during iteration
+            if any(re.match(pattern, field, re.IGNORECASE) for pattern in patterns):
+                fields.remove(field)
+
+        return fields
+
     @staticmethod
     def _validate_parameters(func):
         @wraps(func)
-        def wrapper(instance, *args, **kwargs):
+        def wrapper(instance, **kwargs):
             """
-            Validate the parameters passed to the query method.
+            Validate the parameters passed to the query method including fields, parameters, sort, limit, and offset.
+            This is a decorator for the query _build_query_params method.
 
             Args:
-                instance: The instance of the XBRL class.
-                *args: Variable length argument list.
+                instance (XBRLAPIClient): The instance of the XBRLAPIClient.
                 **kwargs: Arbitrary keyword arguments.
 
             Returns:
                 The result of the wrapped function.
             """
             method_name = kwargs.get("method")
 
+            if not method_name:
+                raise exceptions.XBRLMissingValueError(param="method", expected_value=instance.methods())
+            elif method_name not in instance.methods():
+                raise exceptions.XBRLInvalidValueError(key=method_name, param="method", expected_value=instance.methods())
+
+            elif not isinstance(method_name, str):
+                raise exceptions.XBRLInvalidTypeError(key=method_name, received_type=type(method_name), expected_type=str)
+
             # load the yaml file that has allowed parameters for the method
             file_path = _dir.parent / "methods" / f"{method_name.lower()}.yml"
 
             with file_path.open("r") as file:
                 allowed_for_query = safe_load(file)
 
             # get the parameters, fields, limit, sort, and offset from kwargs that the user passed in
             parameters = kwargs.get("parameters")
             fields = kwargs.get("fields")
             limit = kwargs.get("limit")
             sort = kwargs.get("sort")
             offset = kwargs.get("offset")
+            kwargs.get("print_query")
 
             # get the allowed parameters, fields, limit, sort, and offset from the yaml file
-            allowed_params = allowed_for_query.get("parameters", set())
+            allowed_params = list(allowed_for_query.get("parameters", set()).keys())
             allowed_fields = allowed_for_query.get("fields", set())
             allowed_limit_fields = allowed_for_query.get("limit", set())
-            allowed_sort_fields = allowed_for_query.get("sort", set())
-            allowed_offset_fields = allowed_for_query.get("offset", set())
+            allowed_sort_fields = [field for field in allowed_fields if "*" not in field]
+            allowed_offset_fields = allowed_limit_fields
 
             # Validate fields
             if not fields:
-                raise ValueError("fields cannot be None.")
+                raise exceptions.XBRLMissingValueError(param="fields", expected_value=allowed_fields)
 
+            # clear the conditions from the previous query
+            # this could happen when the limit is greater than account limit or
+            # when the user passes in a field with a condition
+            fields = instance._remove_special_fields(fields)
             for field in fields:
                 if not isinstance(field, str):
-                    raise ValueError(f"field must be a string. {field} is {type(field)}")
+                    raise exceptions.XBRLInvalidTypeError(key=field, expected_type=str, received_type=type(field))
+
                 if field not in allowed_fields:
-                    raise ValueError(
-                        f"""Field
-                        '{field}' is not allowed as a field for '{method_name}'. Allowed fields are:
-                        '{allowed_fields}'.
-                        """
-                    )
+                    raise exceptions.XBRLInvalidValueError(key=field, param="fields", expected_value=allowed_fields, method=method_name)
 
             # Validate parameters
             if parameters:
                 for param in parameters:
                     if param not in allowed_params:
-                        raise ValueError(
-                            f"""
-                        Parameter '{param}' is not allowed for '{method_name}'. Allowed parameters are:
-                        {allowed_params}.
-                        """
+                        raise exceptions.XBRLInvalidValueError(
+                            key=param, param="parameters", expected_value=allowed_params, method=method_name
                         )
 
             # Validate limit
             if limit:
-                if not isinstance(limit, dict):
-                    raise ValueError(f"""limit must be a dictionary not {type(limit)}. e.g. limit = {{'fact': 100}}.""")
-                for key, value in limit.items():
-                    if key not in allowed_limit_fields:
-                        raise ValueError(f"""Limit key '{key}' is not allowed. Allowed limit keys are: {allowed_limit_fields}""")
-                    if not isinstance(value, int):
-                        raise ValueError(f"Limit value must be an integer. {value} is not an integer")
+                # if not dict or an int, raise an error
+                if not isinstance(limit, int):
+                    raise exceptions.XBRLInvalidTypeError(key=limit, expected_type=int, received_type=type(limit))
+
             else:
                 warnings.warn(
-                    """You have not set a limit. This will return the first 100 results by default.
-                    """,
+                    "You have not set a limit; returning the first page only.",
                     UserWarning,
                     stacklevel=2,
                 )
 
             # Validate sort
             if sort:
                 if not isinstance(sort, dict):
                     raise ValueError("Sort must be a dictionary")
+                sort = {instance._remove_special_fields(key): value for key, value in sort.items()}
                 for key, value in sort.items():
                     if key not in allowed_sort_fields:
-                        raise ValueError(f"""Sort key '{key}' is not allowed. Allowed sort keys are: {allowed_sort_fields}.""")
+                        raise exceptions.XBRLInvalidValueError(
+                            key=key, param="sort", expected_value=allowed_sort_fields, method=method_name
+                        )
                     if value.lower() not in ["asc", "desc"]:
-                        raise ValueError("Sort value should be 'asc' or 'desc' only.")
-
-            elif offset:
+                        raise exceptions.XBRLInvalidValueError(key=value, param="sort", expected_value=["asc", "desc"])
+            else:
                 warnings.warn(
-                    "You have set an offset but not a sort method. "
-                    "When using offset, it is recommended that you set a sort method "
-                    "to get reliable results.",
+                    "You have not passed a sort value; for reliable results, set a field to sort.",
                     UserWarning,
                     stacklevel=2,
                 )
 
             # Validate offset
             if offset:
-                if not isinstance(offset, dict):
-                    raise ValueError("Offset must be a dictionary")
-                for key, value in offset.items():
-                    if key not in allowed_offset_fields:
-                        raise ValueError(f"""Offset key '{key}' is not allowed. Allowed offset keys are: {allowed_offset_fields}.""")
-                    if not isinstance(value, int):
-                        raise ValueError(f"Offset value must be an integer. {value} is not an integer.")
+                if not isinstance(offset, int):
+                    raise exceptions.XBRLInvalidTypeError(key=offset, expected_type=int, received_type=type(offset))
 
-            return func(instance, *args, **kwargs)
+            limit_field = next(iter(allowed_limit_fields))
+            offset_field = next(iter(allowed_offset_fields))
+
+            return func(
+                instance,
+                fields=fields,
+                parameters=parameters,
+                limit=limit,
+                sort=sort,
+                offset=offset,
+                limit_field=limit_field,
+                offset_field=offset_field,
+            )
 
         return wrapper
 
-    @staticmethod
+    @_validate_parameters
     def _build_query_params(
+        self,
         fields: Optional[list] = None,
-        parameters=None,
-        limit: Optional[dict] = None,
+        parameters: Optional[dict] = None,
+        limit: Optional[int] = None,
         sort: Optional[dict] = None,
-        offset: Optional[dict] = None,
+        offset: Optional[int] = 0,
+        limit_field: Optional[str] = None,
+        offset_field: Optional[str] = None,
     ) -> dict:
         """
         Build the query parameters for the API request in the format required by the API.
 
         Args:
             fields (list): The list of fields to include in the query.
             parameters (dict): The parameters for the query.
             limit (dict): The limit parameters for the query.
             sort (dict): The sort parameters for the query.
-            offset (dict): The offset parameters for the query.
+            offset (dict): dynamically set if needed
+            limit_field (str): The limit field accepted for the chosen method.
+            offset_field (str): The offset field accepted for the chosen method (which is usually the same as the
+                ``limit_filed``).
 
         Returns:
-            dict: The query parameters.
+            dict: The query parameters that will be submitted to the API.
         """
         query_params = {}
 
         if parameters:
+            # convert the parameters to a string and add it to the query_params
             query_params.update(
                 {
                     f"{k}": ",".join(map(str, v)) if isinstance(v, Iterable) and not isinstance(v, str) else str(v)
                     for k, v in parameters.items()
                 }
             )
 
         # Handle sort
         if sort:
-            # TODO: verify that sort, limit, and offset work together for the same field
             # check if the sort field is in the fields list
             for field, direction in sort.items():
-                # if the field is not in the fields list add the field name followed by .sort(value)
-                if field not in fields:
-                    fields.append(f"{field}.sort({direction.upper()})")
-                # if the field is in the fields list, remove the field
-                # name and add the field name followed by .sort(value)
-                else:
+                # name the field name followed by .sort(value)
+                sorted_arg = f"{field}.sort({direction.upper()})"
+                if field in fields:
+                    # if the field is in the fields list, remove the field
                     fields.remove(field)
-                    fields.append(f"{field}.sort({direction.upper()})")
+                fields.append(sorted_arg)
 
         # Handle limit
         if limit:
-            # check if the limit field is in the fields list
-            for field, value in limit.items():
-                # if the field is not in the fields list add the field name followed by .limit(value)
-                if field not in fields:
-                    fields.append(f"{field}.limit({value})")
+            # name and add the field name followed by .limit(value)
+            limit_arg = f"{limit_field}.limit({limit})"
+            if limit_field in fields:
                 # if the field is in the fields list, remove the field
-                # name and add the field name followed by .limit(value)
-                else:
-                    fields.remove(field)
-                    fields.append(f"{field}.limit({value})")
-        else:
-            fields.append("fact.limit(100)")
+                fields.remove(limit_field)
+            fields.append(limit_arg)
 
         # Handle offset
         if offset:
-            # check if the offset field is in the fields list
-            for field in offset.items():
-                # if the field is not in the fields list add the field name followed by .offset(value)
-                if field not in fields:
-                    fields.append(f"{field}.offset({offset})")
-                # if the field is in the fields list, remove the field
-                # name and add the field name followed by .offset(value)
-                else:
-                    fields.remove(field)
-                    fields.append(f"{field}.offset({offset})")
+            # name and add the field name followed by .offset(value)
+            offset_arg = f"{offset_field}.offset({offset})"
+            if offset_field in fields:
+                fields.remove(offset_field)
+            fields.append(offset_arg)
 
         query_params["fields"] = ",".join(fields)
 
         return query_params
 
     @staticmethod
     def _convert_params_to_dict_decorator(func):
@@ -424,64 +476,180 @@
         # get the url for this method
         with file_path.open("r") as file:
             url = safe_load(file)["url"]
 
         # check if the link requires parameters
         keys = [key.strip("{}") for key in re.findall(r"{(.*?)}", url)]
         if len(keys) > 0:
+            if not parameters:
+                raise exceptions.XBRLRequiredValueError(key=keys, method=method_name)
+
             values = {key: parameters[key] for key in keys if key in parameters}
 
+            # check if all required parameters are present
+            if len(values) != len(keys):
+                missing_keys = [key for key in keys if key not in values]
+                for key in missing_keys:
+                    raise exceptions.XBRLRequiredValueError(key=key, method=method_name)
+
             # get the required parameters for this method
             for key, value in values.items():
                 placeholder = "{" + key + "}"
                 url = url.replace(placeholder, str(value))
-        return f"https://api.xbrl.us{url}"
+        return f"https://api.xbrl.us{url}?"
 
     @_convert_params_to_dict_decorator
-    @_validate_parameters
     def query(
         self,
         method: str,
         fields: Optional[list] = None,
         parameters: Optional[Union[Parameters, dict]] = None,
-        limit: Optional[dict] = None,
+        limit: Optional[int] = None,
         sort: Optional[dict] = None,
-        offset: Optional[dict] = None,
         as_dataframe: bool = False,
+        print_query: Optional[bool] = False,
+        **kwargs,
     ) -> Union[dict, DataFrame]:
         """
 
         Args:
             method (str): The name of the method to query.
             fields (list): The fields query parameter establishes the details of the data to return for the specific query.
             parameters (dict | Parameters): The parameters for the query.
-            limit (dict): A limit restricts the number of results returned by the query.
+            limit (int): A limit restricts the number of results returned by the query.
                 The limit attribute can only be added to an object type and not a property.
                 For example, to limit the number of facts in a query, {"fact": 10}.
             sort (dict): Any returned value can be sorted in ascending or descending order,
                 using ``ASC`` or ``DESC`` (i.e. {"report.document-type": "DESC"}.
                 Multiple sort criteria can be defined and the sort sequence is determined by
                 the order of the items in the dictionary.
-            offset: This attribute enables targeting a return to a specific starting point in a
-                query return sequence (i.e. {"report": 100}. To work reliably,
-                at least one sorted property should be included in the returned fields.
-            as_dataframe (bool=False): Whether to return the results as a DataFrame or json.
+            as_dataframe (bool): If ``True`` returns the results as a ``DataFrame`` else returns the data
+                as ``json``.
+            print_query (bool=False): Whether to print the query.
 
         Returns:
             dict | DataFrame: The results of the query.
         """
+
+        method_url = self._get_method_url(method, parameters)
+        # if limit is all
+        if limit == "all":
+            # arbitrary large number
+            limit = 999999999
+
+        query_params = self._build_query_params(
+            method=method,
+            fields=fields,
+            parameters=parameters,
+            limit=limit,
+            sort=sort,
+        )
+
+        if print_query:
+            print(query_params)
+
+        # check if the account limit has been set
+        if not self.account_limit:
+            self._get_account_limit(url=method_url, params=query_params)
+
+        # ensure the limit is not greater than the account limit
+        account_limit = min(limit, self.account_limit) if limit is not None else self.account_limit
+
+        streamlit_indicator = kwargs.get("streamlit", False)
+        if streamlit_indicator:
+            from stqdm import stqdm
+
+            pbar = stqdm(total=None, desc="Downloading Data:", ncols=80)
+        else:
+            # create a progress bar
+            pbar = tqdm(total=None, desc="Downloading Data:", ncols=80)
+
+        # update the limit in the query params with the new limit
+        query_params = self._build_query_params(
+            method=method,
+            fields=fields,
+            parameters=parameters,
+            limit=account_limit,
+            sort=sort,
+        )
+
         response = self._make_request(
             method="get",
-            url=self._get_method_url(method, parameters),
-            params=self._build_query_params(
-                fields=fields,
-                parameters=parameters,
-                limit=limit,
-                sort=sort,
-                offset=offset,
-            ),
+            url=method_url,
+            params=query_params,
         )
 
+        response_data = response.json()
+
+        if response.status_code != 200:
+            raise response_data["message"]
+        elif "data" not in response_data:
+            warnings.warn("No data returned from the query.", UserWarning, stacklevel=2)
+            return response_data
+
+        data = response_data["data"]
+
+        # update the progress bar
+        pbar.update(len(data))
+
+        if limit is None:
+            # Return the items from the first response if no user limit is provided
+            if as_dataframe:
+                return DataFrame.from_dict(data)
+            else:
+                return data
+
+        else:
+            remaining_limit = limit - len(data)
+
+        # To store all the items from the API response
+        all_data = data
+
+        offset = len(data)
+
+        while remaining_limit > 0:
+            # Determine the limit for the current request
+            try:
+                current_limit = min(account_limit, remaining_limit)
+                query_params = self._build_query_params(
+                    method=method,
+                    fields=fields,
+                    parameters=parameters,
+                    limit=current_limit,
+                    sort=sort,
+                    offset=offset,
+                )
+
+                response = self._make_request(
+                    method="get",
+                    url=method_url,
+                    params=query_params,
+                )
+
+                response_data = response.json()
+                data = response_data["data"]
+
+                # Add the items to the overall collection
+                all_data.extend(data)
+
+                # Decrease the remaining limit by the number of items received
+                remaining_limit -= len(data)
+
+                # update the progress bar
+                pbar.update(len(data))
+
+                if len(data) < current_limit:
+                    # If the number of items received is less than the current limit,
+                    # it means we have reached the end
+                    # of available items, so we can break out of the loop.
+                    break
+
+                # Update the offset for the next request
+                offset += len(data)
+
+            except Exception as e:
+                raise e
+
         if as_dataframe:
-            return DataFrame.from_dict(response.json()["data"])
+            return DataFrame.from_dict(all_data)
         else:
-            return response.json()["data"]
+            return all_data
```

### Comparing `xbrl-us-0.0.1/src/xbrl_us.egg-info/PKG-INFO` & `xbrl-us-0.0.2/src/xbrl_us.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbrl-us
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper for xbrl.us API
 Home-page: https://github.com/hamid-vakilzadeh/python-xbrl-us
 Author: hamid-vakilzadeh
 Author-email: vakilzas@uww.edu
 License: MIT
 Project-URL: Documentation, https://python-xbrl-us.readthedocs.io/
 Project-URL: Changelog, https://python-xbrl-us.readthedocs.io/en/latest/changelog.html
@@ -43,51 +43,64 @@
 
 It's important to note that while the XBRL US Python Wrapper is free and distributed under the permissive MIT license,
 the usage of the underlying XBRL US API is subject to the policies and terms defined by XBRL US.
 These policies govern the access, usage, and restrictions imposed on the API data and services.
 Users of the XBRL US Python Wrapper should review and comply with the XBRL US policies to ensure appropriate
 usage of the API and adherence to any applicable licensing terms.
 
-If you are utilizing the XBRL US Python Wrapper for research purposes, we kindly request that you cite the following paper:
+.. important::
 
-[FILL: Insert Paper Title]
+    Any and all use of the XBRL APIs to return
+    data from the XBRL US Database of Public Filings is in explicit consent and
+    agreement with the `XBRL API Terms of Agreement <https://xbrl.us/home/about/legal/xbrl-api-clientid/>`_.
 
-[FILL: Authors]
+.. note::
+    If you are utilizing the XBRL US Python Wrapper for research purposes, we kindly request that you cite the following paper:
 
-[FILL: Publication Details]
+    [FILL: Insert Paper Title]
 
+    [FILL: Authors]
+
+    [FILL: Publication Details]
 
 
 Tutorial ✏️📖📚
 ================
 
 This tutorial will guide you through using the XBRL-US Python library to interact with the XBRL API. The XBRL-US library provides a convenient way to query and retrieve financial data from the XBRL API using Python.
 
 Prerequisites
 ~~~~~~~~~~~~~
 
 Before you begin, ensure you have the following:
 
 * **Python installed on your system**.
   Right now, the XBRL-US library supports Python 3.10 and above.
-  Backwards compatibility with Python 3.7 and above is planned for a future release.
+  Backwards compatibility with Python 3.8 and above is planned for a future release.
 * **XBRL-US library installed**.
 * **XBRL-US API credentials**.
   You can obtain your credentials by registering for a
   free XBRL-US account at https://xbrl.us/home/use/xbrl-api/.
 * **XBRL-US OAuth2 Access**.
   You can obtain your client ID and client secret by registering for a
   free XBRL-US account at https://xbrl.us/home/use/xbrl-api/access-token/.
 
 You can install it using pip:
 
 .. code-block:: bash
 
     pip install xbrl-us
 
+.. caution::
+
+        The XBRL US Python Wrapper is currently in beta and is subject to change.
+        We welcome your feedback and suggestions for improvement.
+        Please submit any issues or feature requests to
+        the `GitHub repository <https://github.com/hamid-vakilzadeh/python-xbrl-us/issues>`_.
+
 
 **Documentation**
 
 For detailed information about the XBRL-US Python
 library, you can refer to the documentation at https://python-xbrl-us.readthedocs.io/en/latest/.
 
 **Official Documentation**
@@ -154,15 +167,15 @@
             'fact.value',
             'fact.id',
             'entity.id',
             'entity.cik',
             'entity.name',
             'report.sic-code',
         ],
-        limit={'fact': 100},
+        limit=100,
         as_dataframe=True
     )
 
 In this example, we are searching for facts related
 to specific concepts, fiscal years, and SIC codes.
 We are also specifying the fields we want to retrieve
 in the response. The ``limit`` parameter restricts the
@@ -198,15 +211,15 @@
             Fields.FACT_VALUE,
             Fields.FACT_ID,
             Fields.ENTITY_ID,
             Fields.ENTITY_CIK,
             Fields.ENTITY_NAME,
             Fields.REPORT_SIC_CODE,
         ],
-        limit={'fact': 100},
+        limit=100,
         as_dataframe=True
     )
 
 
 This alternative approach also allows you to
 take advantage of the autocomplete feature of your IDE to
 easily find the parameters and fields.
@@ -269,11 +282,23 @@
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
 
-0.0.0 (2023-06-26)
+0.0.2 (2023-07-12)
+~~~~~~~~~~~~~~~~~~
+
+
+* Bug fixes
+* Enhanced error handling
+* Improved method attributes
+* Added the ability to print the query string
+* Implemented a feature to handle queries with large limits
+* NEW: Introduced a web interface for the API, making it even easier to use
+
+
+0.0.1 (2023-07-09)
 ~~~~~~~~~~~~~~~~~~
 
 * First release on PyPI.
```

### Comparing `xbrl-us-0.0.1/tox.ini` & `xbrl-us-0.0.2/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -10,24 +10,22 @@
 
 ; a generative tox configuration, see: https://tox.wiki/en/latest/user_guide.html#generative-environments
 [tox]
 envlist =
     clean,
     check,
     docs,
-    {py37,py38,py39,py310,py311,pypy37,pypy38,pypy39},
+    {py38,py39,py310,py311,pypy38,pypy39},
     report
 ignore_basepython_conflict = true
 
 [testenv]
 basepython =
-    pypy37: {env:TOXPYTHON:pypy3.7}
     pypy38: {env:TOXPYTHON:pypy3.8}
     pypy39: {env:TOXPYTHON:pypy3.9}
-    py37: {env:TOXPYTHON:python3.7}
     py38: {env:TOXPYTHON:python3.8}
     py39: {env:TOXPYTHON:python3.9}
     py310: {env:TOXPYTHON:python3.10}
     py311: {env:TOXPYTHON:python3.11}
     {bootstrap,clean,check,report,docs}: {env:TOXPYTHON:python3}
 setenv =
     PYTHONPATH={toxinidir}/tests
```

