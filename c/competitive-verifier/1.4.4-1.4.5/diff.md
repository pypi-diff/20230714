# Comparing `tmp/competitive_verifier-1.4.4.tar.gz` & `tmp/competitive_verifier-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "competitive_verifier-1.4.4.tar", max compression
+gzip compressed data, was "competitive_verifier-1.4.5.tar", max compression
```

## Comparing `competitive_verifier-1.4.4.tar` & `competitive_verifier-1.4.5.tar`

### file list

```diff
@@ -1,118 +1,117 @@
--rw-r--r--   0        0        0     1062 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/LICENSE
--rw-r--r--   0        0        0     1305 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/README.md
--rw-r--r--   0        0        0     2246 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/src/competitive_verifier/__init__.py
--rw-r--r--   0        0        0     1340 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/src/competitive_verifier/arg.py
--rw-r--r--   0        0        0        0 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/src/competitive_verifier/check/__init__.py
--rw-r--r--   0        0        0     1553 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/src/competitive_verifier/check/main.py
--rw-r--r--   0        0        0      100 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/src/competitive_verifier/config.py
--rw-r--r--   0        0        0        0 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/src/competitive_verifier/console/__init__.py
--rw-r--r--   0        0        0     4143 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/src/competitive_verifier/console/app.py
--rw-r--r--   0        0        0        0 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/src/competitive_verifier/documents/__init__.py
--rw-r--r--   0        0        0    14022 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/src/competitive_verifier/documents/builder.py
--rw-r--r--   0        0        0     1117 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/src/competitive_verifier/documents/front_matter.py
--rw-r--r--   0        0        0     4236 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/src/competitive_verifier/documents/job.py
--rw-r--r--   0        0        0     2469 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/src/competitive_verifier/documents/main.py
--rw-r--r--   0        0        0     3240 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/src/competitive_verifier/documents/render.py
--rw-r--r--   0        0        0     1770 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/src/competitive_verifier/documents/type.py
--rw-r--r--   0        0        0        0 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/src/competitive_verifier/download/__init__.py
--rw-r--r--   0        0        0     2823 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/src/competitive_verifier/download/main.py
--rw-r--r--   0        0        0      247 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/src/competitive_verifier/error.py
--rw-r--r--   0        0        0     1546 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/src/competitive_verifier/exec.py
--rw-r--r--   0        0        0     1012 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/src/competitive_verifier/git.py
--rw-r--r--   0        0        0     5200 2023-02-06 02:05:50.010992 competitive_verifier-1.4.4/src/competitive_verifier/github.py
--rw-r--r--   0        0        0     3392 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/log.py
--rw-r--r--   0        0        0        0 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/merge_input/__init__.py
--rw-r--r--   0        0        0     1321 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/merge_input/main.py
--rw-r--r--   0        0        0        0 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/merge_result/__init__.py
--rw-r--r--   0        0        0     1823 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/merge_result/main.py
--rw-r--r--   0        0        0        0 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/migrate/__init__.py
--rw-r--r--   0        0        0     1057 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/migrate/main.py
--rw-r--r--   0        0        0     7868 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/migrate/migration.py
--rw-r--r--   0        0        0      903 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/models/__init__.py
--rw-r--r--   0        0        0     2754 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/models/_scc.py
--rw-r--r--   0        0        0     6283 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/models/dependency.py
--rw-r--r--   0        0        0     7696 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/models/file.py
--rw-r--r--   0        0        0     3059 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/models/result.py
--rw-r--r--   0        0        0      127 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/models/result_status.py
--rw-r--r--   0        0        0     2948 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/models/verification.py
--rw-r--r--   0        0        0     4498 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/oj.py
--rw-r--r--   0        0        0        0 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/oj_resolve/__init__.py
--rw-r--r--   0        0        0     1709 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/oj_resolve/main.py
--rw-r--r--   0        0        0     6268 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/oj_resolve/resolver.py
--rw-r--r--   0        0        0      252 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/resource.py
--rw-r--r--   0        0        0     4228 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/summary.py
--rw-r--r--   0        0        0      388 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/util.py
--rw-r--r--   0        0        0        0 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/verify/__init__.py
--rw-r--r--   0        0        0     5419 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/verify/main.py
--rw-r--r--   0        0        0     1253 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/verify/split_state.py
--rw-r--r--   0        0        0    11907 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier/verify/verifier.py
--rw-r--r--   0        0        0       25 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/__init__.py
--rw-r--r--   0        0        0     1086 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/config.py
--rw-r--r--   0        0        0        0 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/__init__.py
--rw-r--r--   0        0        0     9474 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/cplusplus.py
--rw-r--r--   0        0        0    17572 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/cplusplus_bundle.py
--rw-r--r--   0        0        0      578 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/go.py
--rw-r--r--   0        0        0      568 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/haskell.py
--rw-r--r--   0        0        0     1671 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/java.py
--rw-r--r--   0        0        0     1715 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/models.py
--rw-r--r--   0        0        0     4092 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/nim.py
--rw-r--r--   0        0        0     3091 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/python.py
--rw-r--r--   0        0        0      560 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/ruby.py
--rw-r--r--   0        0        0    21249 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/rust.py
--rw-r--r--   0        0        0     1880 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/special_comments.py
--rw-r--r--   0        0        0     3531 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/user_defined.py
--rw-r--r--   0        0        0     2446 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/list.py
--rw-r--r--   0        0        0     2308 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/shlex2.py
--rw-r--r--   0        0        0     1089 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/subprocess2.py
--rw-r--r--   0        0        0      611 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/utils.py
--rw-r--r--   0        0        0       73 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/Gemfile
--rw-r--r--   0        0        0        0 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/__init__.py
--rw-r--r--   0        0        0      330 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/_config.yml
--rw-r--r--   0        0        0      560 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/doc_usage.txt
--rw-r--r--   0        0        0       73 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/Gemfile
--rw-r--r--   0        0        0     1014 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_includes/code.html
--rw-r--r--   0        0        0     1215 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_includes/document_body.html
--rw-r--r--   0        0        0       56 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_includes/document_footer.html
--rw-r--r--   0        0        0     2025 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_includes/document_header.html
--rw-r--r--   0        0        0      217 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_includes/head-custom.html
--rw-r--r--   0        0        0       99 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_includes/head-custom2.html
--rw-r--r--   0        0        0      533 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_includes/highlight/highlight_header.html
--rw-r--r--   0        0        0      107 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_includes/highlight_additional.html
--rw-r--r--   0        0        0      131 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_includes/mathjax/mathjax.html
--rw-r--r--   0        0        0      423 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_includes/mathjax/mathjax2.html
--rw-r--r--   0        0        0      644 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_includes/mathjax/mathjax3.html
--rw-r--r--   0        0        0      455 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_includes/theme_fix.html
--rw-r--r--   0        0        0      797 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_includes/toppage_body.html
--rw-r--r--   0        0        0      357 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_includes/toppage_header.html
--rw-r--r--   0        0        0      150 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_layouts/document.html
--rw-r--r--   0        0        0       41 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_layouts/page.html
--rw-r--r--   0        0        0      468 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_layouts/toppage.html
--rw-r--r--   0        0        0      983 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/assets/css/code.scss
--rw-r--r--   0        0        0     1581 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/assets/js/code.js
--rw-r--r--   0        0        0        0 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/__init__.py
--rw-r--r--   0        0        0     2369 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/console/test_app.py
--rw-r--r--   0        0        0        0 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/documents/__init__.py
--rw-r--r--   0        0        0      807 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/documents/test_builder.py
--rw-r--r--   0        0        0        0 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/download/__init__.py
--rw-r--r--   0        0        0     3325 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/download/test_main.py
--rw-r--r--   0        0        0        0 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/merge_input/__init__.py
--rw-r--r--   0        0        0     4669 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/merge_input/test_main.py
--rw-r--r--   0        0        0        0 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/merge_result/__init__.py
--rw-r--r--   0        0        0     4384 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/merge_result/test_main.py
--rw-r--r--   0        0        0     2400 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/migrate/test_subn.py
--rw-r--r--   0        0        0        0 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/models/__init__.py
--rw-r--r--   0        0        0    21012 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/models/test_dependency.py
--rw-r--r--   0        0        0     4735 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/models/test_file.py
--rw-r--r--   0        0        0    23991 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/models/test_result.py
--rw-r--r--   0        0        0     8757 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/models/test_verification.py
--rw-r--r--   0        0        0     7221 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/models/test_verification_input.py
--rw-r--r--   0        0        0     3071 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/test_oj.py
--rw-r--r--   0        0        0      828 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/test_summary.py
--rw-r--r--   0        0        0        0 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/verify/__init__.py
--rw-r--r--   0        0        0     2204 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/verify/test_main.py
--rw-r--r--   0        0        0      765 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/verify/test_split_state.py
--rw-r--r--   0        0        0    16126 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/verify/test_verifier.py
--rw-r--r--   0        0        0    16226 2023-02-06 02:05:50.014992 competitive_verifier-1.4.4/tests/verify/test_verifier_verify.py
--rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 competitive_verifier-1.4.4/setup.py
--rw-r--r--   0        0        0     2208 1970-01-01 00:00:00.000000 competitive_verifier-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-14 10:31:05.265014 competitive_verifier-1.4.5/LICENSE
+-rw-r--r--   0        0        0     1305 2023-07-14 10:31:05.265014 competitive_verifier-1.4.5/README.md
+-rw-r--r--   0        0        0     2246 2023-07-14 10:31:05.265014 competitive_verifier-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 10:31:05.265014 competitive_verifier-1.4.5/src/competitive_verifier/__init__.py
+-rw-r--r--   0        0        0     1340 2023-07-14 10:31:05.265014 competitive_verifier-1.4.5/src/competitive_verifier/arg.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:31:05.265014 competitive_verifier-1.4.5/src/competitive_verifier/check/__init__.py
+-rw-r--r--   0        0        0     1553 2023-07-14 10:31:05.265014 competitive_verifier-1.4.5/src/competitive_verifier/check/main.py
+-rw-r--r--   0        0        0      100 2023-07-14 10:31:05.265014 competitive_verifier-1.4.5/src/competitive_verifier/config.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:31:05.265014 competitive_verifier-1.4.5/src/competitive_verifier/console/__init__.py
+-rw-r--r--   0        0        0     4143 2023-07-14 10:31:05.265014 competitive_verifier-1.4.5/src/competitive_verifier/console/app.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:31:05.265014 competitive_verifier-1.4.5/src/competitive_verifier/documents/__init__.py
+-rw-r--r--   0        0        0    14022 2023-07-14 10:31:05.265014 competitive_verifier-1.4.5/src/competitive_verifier/documents/builder.py
+-rw-r--r--   0        0        0     1117 2023-07-14 10:31:05.265014 competitive_verifier-1.4.5/src/competitive_verifier/documents/front_matter.py
+-rw-r--r--   0        0        0     4236 2023-07-14 10:31:05.265014 competitive_verifier-1.4.5/src/competitive_verifier/documents/job.py
+-rw-r--r--   0        0        0     2469 2023-07-14 10:31:05.265014 competitive_verifier-1.4.5/src/competitive_verifier/documents/main.py
+-rw-r--r--   0        0        0     3240 2023-07-14 10:31:05.265014 competitive_verifier-1.4.5/src/competitive_verifier/documents/render.py
+-rw-r--r--   0        0        0     1770 2023-07-14 10:31:05.265014 competitive_verifier-1.4.5/src/competitive_verifier/documents/type.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:31:05.265014 competitive_verifier-1.4.5/src/competitive_verifier/download/__init__.py
+-rw-r--r--   0        0        0     2823 2023-07-14 10:31:05.265014 competitive_verifier-1.4.5/src/competitive_verifier/download/main.py
+-rw-r--r--   0        0        0      247 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/error.py
+-rw-r--r--   0        0        0     1546 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/exec.py
+-rw-r--r--   0        0        0     1012 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/git.py
+-rw-r--r--   0        0        0     5200 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/github.py
+-rw-r--r--   0        0        0     3392 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/log.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/merge_input/__init__.py
+-rw-r--r--   0        0        0     1321 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/merge_input/main.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/merge_result/__init__.py
+-rw-r--r--   0        0        0     1823 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/merge_result/main.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/migrate/__init__.py
+-rw-r--r--   0        0        0     1057 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/migrate/main.py
+-rw-r--r--   0        0        0     7868 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/migrate/migration.py
+-rw-r--r--   0        0        0      903 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/models/__init__.py
+-rw-r--r--   0        0        0     2754 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/models/_scc.py
+-rw-r--r--   0        0        0     6283 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/models/dependency.py
+-rw-r--r--   0        0        0     7696 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/models/file.py
+-rw-r--r--   0        0        0     3059 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/models/result.py
+-rw-r--r--   0        0        0      127 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/models/result_status.py
+-rw-r--r--   0        0        0     2948 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/models/verification.py
+-rw-r--r--   0        0        0     4498 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/oj.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/oj_resolve/__init__.py
+-rw-r--r--   0        0        0     1709 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/oj_resolve/main.py
+-rw-r--r--   0        0        0     6268 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/oj_resolve/resolver.py
+-rw-r--r--   0        0        0      252 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/resource.py
+-rw-r--r--   0        0        0     4228 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/summary.py
+-rw-r--r--   0        0        0      388 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/util.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/verify/__init__.py
+-rw-r--r--   0        0        0     5419 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/verify/main.py
+-rw-r--r--   0        0        0     1253 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/verify/split_state.py
+-rw-r--r--   0        0        0    11907 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier/verify/verifier.py
+-rw-r--r--   0        0        0       25 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/__init__.py
+-rw-r--r--   0        0        0     1086 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/config.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/__init__.py
+-rw-r--r--   0        0        0     9474 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/cplusplus.py
+-rw-r--r--   0        0        0    17572 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/cplusplus_bundle.py
+-rw-r--r--   0        0        0      578 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/go.py
+-rw-r--r--   0        0        0      568 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/haskell.py
+-rw-r--r--   0        0        0     1671 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/java.py
+-rw-r--r--   0        0        0     1715 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/models.py
+-rw-r--r--   0        0        0     4092 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/nim.py
+-rw-r--r--   0        0        0     3091 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/python.py
+-rw-r--r--   0        0        0      560 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/ruby.py
+-rw-r--r--   0        0        0    21249 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/rust.py
+-rw-r--r--   0        0        0     1880 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/special_comments.py
+-rw-r--r--   0        0        0     3531 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/user_defined.py
+-rw-r--r--   0        0        0     2446 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/list.py
+-rw-r--r--   0        0        0     2308 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/shlex2.py
+-rw-r--r--   0        0        0     1089 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/subprocess2.py
+-rw-r--r--   0        0        0      611 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/utils.py
+-rw-r--r--   0        0        0       73 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/Gemfile
+-rw-r--r--   0        0        0        0 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/__init__.py
+-rw-r--r--   0        0        0      330 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/_config.yml
+-rw-r--r--   0        0        0      560 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/doc_usage.txt
+-rw-r--r--   0        0        0       73 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/Gemfile
+-rw-r--r--   0        0        0     1014 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_includes/code.html
+-rw-r--r--   0        0        0     1215 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_includes/document_body.html
+-rw-r--r--   0        0        0       56 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_includes/document_footer.html
+-rw-r--r--   0        0        0     2025 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_includes/document_header.html
+-rw-r--r--   0        0        0      217 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_includes/head-custom.html
+-rw-r--r--   0        0        0       99 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_includes/head-custom2.html
+-rw-r--r--   0        0        0      533 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_includes/highlight/highlight_header.html
+-rw-r--r--   0        0        0      107 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_includes/highlight_additional.html
+-rw-r--r--   0        0        0      131 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_includes/mathjax/mathjax.html
+-rw-r--r--   0        0        0      423 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_includes/mathjax/mathjax2.html
+-rw-r--r--   0        0        0      644 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_includes/mathjax/mathjax3.html
+-rw-r--r--   0        0        0      455 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_includes/theme_fix.html
+-rw-r--r--   0        0        0      797 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_includes/toppage_body.html
+-rw-r--r--   0        0        0      357 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_includes/toppage_header.html
+-rw-r--r--   0        0        0      150 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_layouts/document.html
+-rw-r--r--   0        0        0       41 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_layouts/page.html
+-rw-r--r--   0        0        0      468 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_layouts/toppage.html
+-rw-r--r--   0        0        0      983 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/assets/css/code.scss
+-rw-r--r--   0        0        0     1581 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/assets/js/code.js
+-rw-r--r--   0        0        0        0 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/__init__.py
+-rw-r--r--   0        0        0     2369 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/console/test_app.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/documents/__init__.py
+-rw-r--r--   0        0        0      807 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/documents/test_builder.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/download/__init__.py
+-rw-r--r--   0        0        0     3325 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/download/test_main.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/merge_input/__init__.py
+-rw-r--r--   0        0        0     4669 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/merge_input/test_main.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/merge_result/__init__.py
+-rw-r--r--   0        0        0     4384 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/merge_result/test_main.py
+-rw-r--r--   0        0        0     2400 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/migrate/test_subn.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/models/__init__.py
+-rw-r--r--   0        0        0    21012 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/models/test_dependency.py
+-rw-r--r--   0        0        0     4735 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/models/test_file.py
+-rw-r--r--   0        0        0    23991 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/models/test_result.py
+-rw-r--r--   0        0        0     8757 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/models/test_verification.py
+-rw-r--r--   0        0        0     7221 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/models/test_verification_input.py
+-rw-r--r--   0        0        0     3071 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/test_oj.py
+-rw-r--r--   0        0        0      828 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/test_summary.py
+-rw-r--r--   0        0        0        0 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/verify/__init__.py
+-rw-r--r--   0        0        0     2204 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/verify/test_main.py
+-rw-r--r--   0        0        0      765 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/verify/test_split_state.py
+-rw-r--r--   0        0        0    16126 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/verify/test_verifier.py
+-rw-r--r--   0        0        0    16226 2023-07-14 10:31:05.269014 competitive_verifier-1.4.5/tests/verify/test_verifier_verify.py
+-rw-r--r--   0        0        0     2208 1970-01-01 00:00:00.000000 competitive_verifier-1.4.5/PKG-INFO
```

### Comparing `competitive_verifier-1.4.4/LICENSE` & `competitive_verifier-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/README.md` & `competitive_verifier-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/pyproject.toml` & `competitive_verifier-1.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "competitive-verifier"
-version = "1.4.4"
+version = "1.4.5"
 description = "Verifier for libraries of competitive programming"
 
 license = "MIT"
 authors = ["kzrnm <gengesa@gmail.com>"]
 
 repository = "https://github.com/competitive-verifier/competitive-verifier"
 homepage = "https://github.com/competitive-verifier/competitive-verifier"
```

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/arg.py` & `competitive_verifier-1.4.5/src/competitive_verifier/arg.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/check/main.py` & `competitive_verifier-1.4.5/src/competitive_verifier/check/main.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/console/app.py` & `competitive_verifier-1.4.5/src/competitive_verifier/console/app.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/documents/builder.py` & `competitive_verifier-1.4.5/src/competitive_verifier/documents/builder.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import importlib.resources
 import pathlib
-from logging import getLogger
 from functools import cache
+from logging import getLogger
 from typing import Any, Iterable, Optional, Union
 
 import yaml
 
 from competitive_verifier import git, github, log
 from competitive_verifier.models import (
     ProblemVerification,
```

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/documents/front_matter.py` & `competitive_verifier-1.4.5/src/competitive_verifier/documents/front_matter.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/documents/job.py` & `competitive_verifier-1.4.5/src/competitive_verifier/documents/job.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/documents/main.py` & `competitive_verifier-1.4.5/src/competitive_verifier/documents/main.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/documents/render.py` & `competitive_verifier-1.4.5/src/competitive_verifier/documents/render.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/documents/type.py` & `competitive_verifier-1.4.5/src/competitive_verifier/documents/type.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/download/main.py` & `competitive_verifier-1.4.5/src/competitive_verifier/download/main.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/exec.py` & `competitive_verifier-1.4.5/src/competitive_verifier/exec.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/git.py` & `competitive_verifier-1.4.5/src/competitive_verifier/git.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/github.py` & `competitive_verifier-1.4.5/src/competitive_verifier/github.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/log.py` & `competitive_verifier-1.4.5/src/competitive_verifier/log.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/merge_input/main.py` & `competitive_verifier-1.4.5/src/competitive_verifier/merge_input/main.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/merge_result/main.py` & `competitive_verifier-1.4.5/src/competitive_verifier/merge_result/main.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/migrate/main.py` & `competitive_verifier-1.4.5/src/competitive_verifier/migrate/main.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/migrate/migration.py` & `competitive_verifier-1.4.5/src/competitive_verifier/migrate/migration.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/models/__init__.py` & `competitive_verifier-1.4.5/src/competitive_verifier/models/__init__.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/models/_scc.py` & `competitive_verifier-1.4.5/src/competitive_verifier/models/_scc.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/models/dependency.py` & `competitive_verifier-1.4.5/src/competitive_verifier/models/dependency.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/models/file.py` & `competitive_verifier-1.4.5/src/competitive_verifier/models/file.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/models/result.py` & `competitive_verifier-1.4.5/src/competitive_verifier/models/result.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/models/verification.py` & `competitive_verifier-1.4.5/src/competitive_verifier/models/verification.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/oj.py` & `competitive_verifier-1.4.5/src/competitive_verifier/oj.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/oj_resolve/main.py` & `competitive_verifier-1.4.5/src/competitive_verifier/oj_resolve/main.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/oj_resolve/resolver.py` & `competitive_verifier-1.4.5/src/competitive_verifier/oj_resolve/resolver.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/summary.py` & `competitive_verifier-1.4.5/src/competitive_verifier/summary.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/verify/main.py` & `competitive_verifier-1.4.5/src/competitive_verifier/verify/main.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/verify/split_state.py` & `competitive_verifier-1.4.5/src/competitive_verifier/verify/split_state.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier/verify/verifier.py` & `competitive_verifier-1.4.5/src/competitive_verifier/verify/verifier.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/config.py` & `competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/config.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/cplusplus.py` & `competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/cplusplus.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/cplusplus_bundle.py` & `competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/cplusplus_bundle.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/go.py` & `competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/go.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/haskell.py` & `competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/haskell.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/java.py` & `competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/java.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/models.py` & `competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/models.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/nim.py` & `competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/nim.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/python.py` & `competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/python.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/ruby.py` & `competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/ruby.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/rust.py` & `competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/rust.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/special_comments.py` & `competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/special_comments.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/languages/user_defined.py` & `competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/languages/user_defined.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/list.py` & `competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/list.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/shlex2.py` & `competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/shlex2.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/subprocess2.py` & `competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/subprocess2.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_oj_clone/utils.py` & `competitive_verifier-1.4.5/src/competitive_verifier_oj_clone/utils.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_resources/doc_usage.txt` & `competitive_verifier-1.4.5/src/competitive_verifier_resources/doc_usage.txt`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_includes/code.html` & `competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_includes/code.html`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_includes/document_body.html` & `competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_includes/document_body.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 {%- if page.data.dependsOn.size != 0 -%}
     <h2>Depends on</h2>
     <ul>
     {%- for item in page.data._extendedDependsOn -%}
-        <li><a href="{{ item.path | absolute_url }}">{{ item.icon }} {{ item.title }}
+        <li><a href="{{ item.path | relative_url }}">{{ item.icon }} {{ item.title }}
             {%- if item.title != item.path %}<small>({{ item.path }})</small>{%- endif -%}
         </a></li>
     {%- endfor -%}
     </ul>
 {%- endif -%}
 
 
 {%- if page.data.requiredBy.size != 0 -%}
     <h2>Required by</h2>
     <ul>
     {%- for item in page.data._extendedRequiredBy -%}
-        <li><a href="{{ item.path | absolute_url }}">{{ item.icon }} {{ item.title }}
+        <li><a href="{{ item.path | relative_url }}">{{ item.icon }} {{ item.title }}
             {%- if item.title != item.path %}<small>({{ item.path }})</small>{%- endif -%}
         </a></li>
     {%- endfor -%}
     </ul>
 {%- endif -%}
 
 
 {%- if page.data.verifiedWith.size != 0 -%}
     <h2>Verified with</h2>
     <ul>
     {%- for item in page.data._extendedVerifiedWith -%}
-        <li><a href="{{ item.path | absolute_url }}">{{ item.icon }} {{ item.title }}
+        <li><a href="{{ item.path | relative_url }}">{{ item.icon }} {{ item.title }}
             {%- if item.title != item.path %}<small>({{ item.path }})</small>{%- endif -%}
         </a></li>
     {%- endfor -%}
     </ul>
 {%- endif -%}
 
 <h2>Code</h2>
```

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_includes/document_header.html` & `competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_includes/document_header.html`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_includes/mathjax/mathjax3.html` & `competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_includes/mathjax/mathjax3.html`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/_includes/toppage_body.html` & `competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/_includes/toppage_body.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 <h2>Library Files</h2>
 
 {% for category in page.data.libraryCategories %}
     <h3>{{ category.name }}</h3>
     <ul>
         {% for item in category.pages %}
-        <li><a href="{{ item.path | absolute_url }}">{{ item.icon }} {{ item.title }}
+        <li><a href="{{ item.path | relative_url }}">{{ item.icon }} {{ item.title }}
             {% if item.title != item.path %}<small>({{ item.path }})</small>{% endif %}
         </a></li>
         {% endfor %}
     </ul>
 {% endfor %}
 
 <h2>Verification Files</h2>
 
 {% for category in page.data.verificationCategories %}
     <h3>{{ category.name }}</h3>
     <ul>
         {% for item in category.pages %}
-        <li><a href="{{ item.path | absolute_url }}">{{ item.icon }} {{ item.title }}
+        <li><a href="{{ item.path | relative_url }}">{{ item.icon }} {{ item.title }}
             {% if item.title != item.path %}<small>({{ item.path }})</small>{% endif %}
         </a></li>
         {% endfor %}
     </ul>
 {% endfor %}
```

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/assets/css/code.scss` & `competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/assets/css/code.scss`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/src/competitive_verifier_resources/jekyll/assets/js/code.js` & `competitive_verifier-1.4.5/src/competitive_verifier_resources/jekyll/assets/js/code.js`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/tests/console/test_app.py` & `competitive_verifier-1.4.5/tests/console/test_app.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/tests/documents/test_builder.py` & `competitive_verifier-1.4.5/tests/documents/test_builder.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/tests/download/test_main.py` & `competitive_verifier-1.4.5/tests/download/test_main.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/tests/merge_input/test_main.py` & `competitive_verifier-1.4.5/tests/merge_input/test_main.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/tests/merge_result/test_main.py` & `competitive_verifier-1.4.5/tests/merge_result/test_main.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/tests/migrate/test_subn.py` & `competitive_verifier-1.4.5/tests/migrate/test_subn.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/tests/models/test_dependency.py` & `competitive_verifier-1.4.5/tests/models/test_dependency.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/tests/models/test_file.py` & `competitive_verifier-1.4.5/tests/models/test_file.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/tests/models/test_result.py` & `competitive_verifier-1.4.5/tests/models/test_result.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/tests/models/test_verification.py` & `competitive_verifier-1.4.5/tests/models/test_verification.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/tests/models/test_verification_input.py` & `competitive_verifier-1.4.5/tests/models/test_verification_input.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/tests/test_oj.py` & `competitive_verifier-1.4.5/tests/test_oj.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/tests/test_summary.py` & `competitive_verifier-1.4.5/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/tests/verify/test_main.py` & `competitive_verifier-1.4.5/tests/verify/test_main.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/tests/verify/test_split_state.py` & `competitive_verifier-1.4.5/tests/verify/test_split_state.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/tests/verify/test_verifier.py` & `competitive_verifier-1.4.5/tests/verify/test_verifier.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/tests/verify/test_verifier_verify.py` & `competitive_verifier-1.4.5/tests/verify/test_verifier_verify.py`

 * *Files identical despite different names*

### Comparing `competitive_verifier-1.4.4/PKG-INFO` & `competitive_verifier-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: competitive-verifier
-Version: 1.4.4
+Version: 1.4.5
 Summary: Verifier for libraries of competitive programming
 Home-page: https://github.com/competitive-verifier/competitive-verifier
 License: MIT
 Author: kzrnm
 Author-email: gengesa@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

