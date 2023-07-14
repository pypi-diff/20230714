# Comparing `tmp/lmql-0.0.6.4.tar.gz` & `tmp/lmql-0.0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmql-0.0.6.4.tar", last modified: Thu Jun  8 15:29:16 2023, max compression
+gzip compressed data, was "lmql-0.0.6.5.tar", last modified: Fri Jul 14 15:57:02 2023, max compression
```

## Comparing `lmql-0.0.6.4.tar` & `lmql-0.0.6.5.tar`

### file list

```diff
@@ -1,292 +1,315 @@
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.487840 lmql-0.0.6.4/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.459840 lmql-0.0.6.4/.github/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.463840 lmql-0.0.6.4/.github/workflows/
--rw-rw-r--   0 luca      (1000) luca      (1000)     2285 2023-06-02 17:03:48.000000 lmql-0.0.6.4/.github/workflows/lmql-web.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)     2743 2023-05-11 15:13:38.000000 lmql-0.0.6.4/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.6.4/LICENSE
--rw-rw-r--   0 luca      (1000) luca      (1000)      140 2023-04-17 14:44:31.000000 lmql-0.0.6.4/MANIFEST.in
--rw-rw-r--   0 luca      (1000) luca      (1000)     4991 2023-06-08 15:29:16.487840 lmql-0.0.6.4/PKG-INFO
--rw-rw-r--   0 luca      (1000) luca      (1000)     4541 2023-06-07 20:54:49.000000 lmql-0.0.6.4/README.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.463840 lmql-0.0.6.4/docs/
--rw-rw-r--   0 luca      (1000) luca      (1000)      638 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/Makefile
--rw-rw-r--   0 luca      (1000) luca      (1000)      444 2023-03-14 15:27:49.000000 lmql-0.0.6.4/docs/RELEASE.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      799 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/make.bat
--rw-rw-r--   0 luca      (1000) luca      (1000)       81 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/requirements.txt
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.463840 lmql-0.0.6.4/docs/source/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.463840 lmql-0.0.6.4/docs/source/_ext/
--rw-rw-r--   0 luca      (1000) luca      (1000)     5543 2023-05-11 20:52:54.000000 lmql-0.0.6.4/docs/source/_ext/lmql_snippets.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.459840 lmql-0.0.6.4/docs/source/_static/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.463840 lmql-0.0.6.4/docs/source/_static/css/
--rw-rw-r--   0 luca      (1000) luca      (1000)     5883 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/_static/css/lmql-docs.css
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/docs/source/_static/images/
--rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/source/_static/images/lmql.svg
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/docs/source/_static/js/
--rw-rw-r--   0 luca      (1000) luca      (1000)     2252 2023-05-11 20:52:54.000000 lmql-0.0.6.4/docs/source/_static/js/lmql-playground.js
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/docs/source/_templates/
--rw-rw-r--   0 luca      (1000) luca      (1000)      292 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/source/_templates/layout.html
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/docs/source/blog/
--rw-rw-r--   0 luca      (1000) luca      (1000)     4591 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/blog/release-0.0.5.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     1444 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/blog/release-0.0.6.1.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     2068 2023-05-11 20:52:54.000000 lmql-0.0.6.4/docs/source/blog/release-0.0.6.3.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     8976 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/blog/release-0.0.6.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     1167 2023-04-17 14:48:56.000000 lmql-0.0.6.4/docs/source/conf.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1293 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/source/dev-setup.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     2333 2023-05-22 15:02:40.000000 lmql-0.0.6.4/docs/source/docker-setup.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/docs/source/images/
--rw-rw-r--   0 luca      (1000) luca      (1000)   125712 2023-06-07 20:54:49.000000 lmql-0.0.6.4/docs/source/images/inference.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     2798 2023-05-22 15:02:40.000000 lmql-0.0.6.4/docs/source/index.rst
--rw-rw-r--   0 luca      (1000) luca      (1000)     2563 2023-05-22 15:02:40.000000 lmql-0.0.6.4/docs/source/installation.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/docs/source/language/
--rw-rw-r--   0 luca      (1000) luca      (1000)     1382 2023-06-07 20:54:49.000000 lmql-0.0.6.4/docs/source/language/azure.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     7435 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/source/language/constraints.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     4067 2023-04-17 14:48:56.000000 lmql-0.0.6.4/docs/source/language/decoders.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     7850 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/source/language/functions.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     3967 2023-06-07 20:54:49.000000 lmql-0.0.6.4/docs/source/language/hf.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      753 2023-06-07 20:54:49.000000 lmql-0.0.6.4/docs/source/language/models.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     5710 2023-06-07 20:54:49.000000 lmql-0.0.6.4/docs/source/language/openai.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     8507 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/language/overview.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     3676 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/language/scripted_prompts.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     3675 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/source/lmql.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)    28444 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/source/logo.png
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/docs/source/pending/
--rw-rw-r--   0 luca      (1000) luca      (1000)     3550 2023-05-11 20:52:54.000000 lmql-0.0.6.4/docs/source/pending/release-next.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/docs/source/python/
--rw-rw-r--   0 luca      (1000) luca      (1000)       11 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/source/python/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    11193 2023-06-08 13:00:38.000000 lmql-0.0.6.4/docs/source/python/langchain.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     1157 2023-06-08 13:00:38.000000 lmql-0.0.6.4/docs/source/python/lc.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     6681 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/python/llama_index.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)    75148 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/source/python/lmql.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)     7458 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/python/output.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     9592 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/python/pandas.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     8847 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/python/python.ipynb
--rw-rw-r--   0 luca      (1000) luca      (1000)     3135 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/source/quickstart.md
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/docs/source/releases/
--rw-rw-r--   0 luca      (1000) luca      (1000)     2263 2023-05-11 15:13:38.000000 lmql-0.0.6.4/docs/source/releases/misc-snippets.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      321 2023-04-17 14:48:56.000000 lmql-0.0.6.4/docs/source/releases/release-0.0.5.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      257 2023-04-17 14:44:31.000000 lmql-0.0.6.4/docs/todo.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      137 2023-03-14 15:27:49.000000 lmql-0.0.6.4/pyproject.toml
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/scripts/
--rw-rw-r--   0 luca      (1000) luca      (1000)      577 2023-05-22 15:02:40.000000 lmql-0.0.6.4/scripts/Dockerfile
--rw-rw-r--   0 luca      (1000) luca      (1000)      295 2023-04-17 14:44:31.000000 lmql-0.0.6.4/scripts/activate-dev.sh
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/scripts/conda/
--rw-rw-r--   0 luca      (1000) luca      (1000)      198 2023-05-11 15:26:02.000000 lmql-0.0.6.4/scripts/conda/requirements-no-gpu.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)      332 2023-05-11 15:26:02.000000 lmql-0.0.6.4/scripts/conda/requirements.yml
--rw-rw-r--   0 luca      (1000) luca      (1000)      486 2023-03-14 15:27:49.000000 lmql-0.0.6.4/scripts/pypi-release.sh
--rw-rw-r--   0 luca      (1000) luca      (1000)     3897 2023-06-07 20:54:49.000000 lmql-0.0.6.4/scripts/serve-all.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      817 2023-03-14 15:27:49.000000 lmql-0.0.6.4/scripts/wheel.sh
--rw-rw-r--   0 luca      (1000) luca      (1000)      868 2023-06-08 15:29:16.487840 lmql-0.0.6.4/setup.cfg
--rw-rw-r--   0 luca      (1000) luca      (1000)       37 2023-05-10 14:35:25.000000 lmql-0.0.6.4/setup.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/src/
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.467840 lmql-0.0.6.4/src/lmql/
--rw-rw-r--   0 luca      (1000) luca      (1000)     6821 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/__init__.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.471840 lmql-0.0.6.4/src/lmql/algorithms/
--rw-rw-r--   0 luca      (1000) luca      (1000)       45 2023-05-18 06:05:21.000000 lmql-0.0.6.4/src/lmql/algorithms/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2556 2023-06-02 17:03:48.000000 lmql-0.0.6.4/src/lmql/algorithms/cache.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      916 2023-06-02 17:03:48.000000 lmql-0.0.6.4/src/lmql/algorithms/functools.py
--rwxrwxr-x   0 luca      (1000) luca      (1000)     8222 2023-06-08 13:11:14.000000 lmql-0.0.6.4/src/lmql/cli.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1577 2023-06-02 17:03:48.000000 lmql-0.0.6.4/src/lmql/demo.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1531 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql/http.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.471840 lmql-0.0.6.4/src/lmql/language/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/language/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    24626 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/language/compiler.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    10194 2023-06-08 14:18:51.000000 lmql-0.0.6.4/src/lmql/language/fragment_parser.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1374 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/language/qstrings.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1804 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/language/validator.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.471840 lmql-0.0.6.4/src/lmql/models/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/models/__init__.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.471840 lmql-0.0.6.4/src/lmql/models/lmtp/
--rw-rw-r--   0 luca      (1000) luca      (1000)     6156 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/models/lmtp/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     5726 2023-06-07 20:54:59.000000 lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_client.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    19104 2023-06-07 20:54:59.000000 lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_dcmodel.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    18111 2023-06-07 20:59:25.000000 lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_inference_server.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     5514 2023-06-07 20:54:59.000000 lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_multiprocessing.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      298 2023-06-07 20:54:59.000000 lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_programmatic_serve_example.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4445 2023-06-07 20:54:59.000000 lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_serve.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3562 2023-06-07 20:54:59.000000 lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_threading.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      465 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/models/lmtp/utils.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3230 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/models/model.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.471840 lmql-0.0.6.4/src/lmql/ops/
--rw-rw-r--   0 luca      (1000) luca      (1000)       93 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ops/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     7542 2023-06-02 17:03:48.000000 lmql-0.0.6.4/src/lmql/ops/follow_map.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    41664 2023-06-02 17:03:48.000000 lmql-0.0.6.4/src/lmql/ops/ops.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    21151 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/ops/token_set.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.471840 lmql-0.0.6.4/src/lmql/output/
--rw-rw-r--   0 luca      (1000) luca      (1000)       57 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/output/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2334 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/output/http.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1889 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/output/sse.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2282 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/output/ws.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.471840 lmql-0.0.6.4/src/lmql/runtime/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/runtime/__init__.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.471840 lmql-0.0.6.4/src/lmql/runtime/bopenai/
--rw-rw-r--   0 luca      (1000) luca      (1000)     2236 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/runtime/bopenai/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    29480 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/bopenai/batched_openai.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    21244 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/bopenai/openai_api.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2096 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/caching.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.475840 lmql-0.0.6.4/src/lmql/runtime/dclib/
--rw-rw-r--   0 luca      (1000) luca      (1000)      494 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/runtime/dclib/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    18839 2023-05-18 06:05:21.000000 lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_array.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    26228 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_cache.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      592 2023-06-08 13:11:09.000000 lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_global.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4971 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_model.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     8589 2023-06-02 17:03:48.000000 lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_rewrite.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    32272 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_seq.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    21200 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/dclib/decoders.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    36788 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/runtime/interpreter.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      250 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/runtime/interrupt.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1231 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/runtime/langchain.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     8241 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/runtime/lmql_runtime.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1840 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/runtime/loop.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1245 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/maiohttp.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1726 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/runtime/masks.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2783 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/runtime/model_registry.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     5943 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/runtime/multi_head_interpretation.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    44712 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/openai_integration.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1971 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql/runtime/openai_secret.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4042 2023-06-02 17:03:48.000000 lmql-0.0.6.4/src/lmql/runtime/output_writer.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.475840 lmql-0.0.6.4/src/lmql/runtime/postprocessing/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/runtime/postprocessing/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3543 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/postprocessing/conditional_prob.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      152 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql/runtime/postprocessing/group_by.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2067 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/program_state.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1317 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql/runtime/stats.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2116 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/token_distribution.py
--rw-rw-r--   0 luca      (1000) luca      (1000)    10709 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/runtime/tokenizer.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.475840 lmql-0.0.6.4/src/lmql/runtime/tokenizers/
--rw-rw-r--   0 luca      (1000) luca      (1000)     3027 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/tokenizers/hf_tokenizer.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3415 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/tokenizers/pure_python_tokenizer.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3207 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/runtime/tokenizers/tiktoken_tokenizer.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.475840 lmql-0.0.6.4/src/lmql/tests/
--rw-rw-r--   0 luca      (1000) luca      (1000)      319 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql/tests/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     5899 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/tests/expr_test_utils.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1314 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/fin_and.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      879 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/tests/local_model_python.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.475840 lmql-0.0.6.4/src/lmql/tests/outdated/
--rw-rw-r--   0 luca      (1000) luca      (1000)     1611 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/outdated/mask_product_test.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2789 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/outdated/monotonicity.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      546 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/outdated/one_of_tests.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      758 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/outdated/sentences_op.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      984 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/outdated/starts_with_op_test.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1236 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/outdated/stops_at.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      537 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/outdated/str_in_str_tests.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4738 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/outdated/test_multi_head.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3036 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/outdated/token_set_test.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.475840 lmql-0.0.6.4/src/lmql/tests/queryargs/
--rw-rw-r--   0 luca      (1000) luca      (1000)     4489 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/tests/queryargs/test_args.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2072 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/tests/queryargs/test_args_query_str.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1095 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/tests/queryargs/test_args_run.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1066 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/tests/queryargs/test_sync.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1092 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/tests/queryargs/test_var_errors.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.475840 lmql-0.0.6.4/src/lmql/tests/system/
--rw-rw-r--   0 luca      (1000) luca      (1000)     3402 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/tests/system/basic_use_cases.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      842 2023-05-18 06:05:21.000000 lmql-0.0.6.4/src/lmql/tests/tail_token_set.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      788 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/test_back2back_caching.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2382 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/test_eq.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1139 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/tests/test_multibyte_characters.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1140 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/tests/test_multibyte_local_models.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      457 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/test_orop.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      448 2023-06-08 13:00:38.000000 lmql-0.0.6.4/src/lmql/tests/test_query_args.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2639 2023-05-18 06:05:21.000000 lmql-0.0.6.4/src/lmql/tests/test_sample_queries.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     1720 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/test_scoping.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3572 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/tests/test_stopping.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      707 2023-05-18 06:05:21.000000 lmql-0.0.6.4/src/lmql/tests/tiktoken_tsets.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.475840 lmql-0.0.6.4/src/lmql/ui/
--rw-rw-r--   0 luca      (1000) luca      (1000)       27 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/__init__.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.479840 lmql-0.0.6.4/src/lmql/ui/live/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/live/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     6747 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/live/live.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     3313 2023-06-06 10:45:15.000000 lmql-0.0.6.4/src/lmql/ui/live/live.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     3885 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/live/livelib.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      349 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/live/package.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    33701 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/live/yarn.lock
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.479840 lmql-0.0.6.4/src/lmql/ui/playground/
--rw-rw-r--   0 luca      (1000) luca      (1000)       31 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/.dockerignore
--rw-rw-r--   0 luca      (1000) luca      (1000)       34 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/.env
--rw-rw-r--   0 luca      (1000) luca      (1000)      310 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/.gitignore
--rw-rw-r--   0 luca      (1000) luca      (1000)      354 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/Dockerfile
--rw-rw-r--   0 luca      (1000) luca      (1000)     3359 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)     1327 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/package.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.479840 lmql-0.0.6.4/src/lmql/ui/playground/public/
--rw-rw-r--   0 luca      (1000) luca      (1000)       90 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/_headers
--rw-rw-r--   0 luca      (1000) luca      (1000)     3870 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/favicon.ico
--rw-rw-r--   0 luca      (1000) luca      (1000)     1678 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/index.html
--rw-rw-r--   0 luca      (1000) luca      (1000)     2817 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/lmql.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)      306 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/manifest.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.483840 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/
--rw-rw-r--   0 luca      (1000) luca      (1000)  1227728 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/calc.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   295285 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/chat.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   160153 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/cot.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    81768 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/distribution.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    22895 2023-06-08 13:49:28.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/hello.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    89531 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/joke.json
--rw-rw-r--   0 luca      (1000) luca      (1000)  1710847 2023-05-23 11:41:29.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/kv.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    52748 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/list.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   628184 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/meta.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   264768 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/translation.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   215050 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/wiki.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       67 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/robots.txt
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.483840 lmql-0.0.6.4/src/lmql/ui/playground/public/snippets/
--rw-rw-r--   0 luca      (1000) luca      (1000)   381736 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
--rw-rw-r--   0 luca      (1000) luca      (1000)   184008 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/ui/playground/public/snippets/json-parsing.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       62 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/ref.py
--rw-rw-r--   0 luca      (1000) luca      (1000)       80 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/run-in-docker.sh
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.487840 lmql-0.0.6.4/src/lmql/ui/playground/src/
--rw-rw-r--   0 luca      (1000) luca      (1000)    69705 2023-06-08 15:24:40.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/App.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      246 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/App.test.js
--rw-rw-r--   0 luca      (1000) luca      (1000)    29983 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/CodeScreenshot.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      807 2023-06-02 17:03:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/Configuration.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     1174 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/DataListView.js
--rw-rw-r--   0 luca      (1000) luca      (1000)    21617 2023-06-08 15:27:15.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/DecoderGraph.js
--rw-rw-r--   0 luca      (1000) luca      (1000)      329 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/DecodingTree.js
--rw-rw-r--   0 luca      (1000) luca      (1000)       89 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/Embed.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)     9601 2023-06-02 17:03:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/Explore.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)      675 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/SharedState.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     4819 2023-06-08 15:09:20.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/State.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     5871 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/ValidationGraph.jsx
--rw-rw-r--   0 luca      (1000) luca      (1000)     9360 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/browser_process.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     1163 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/build_info.js
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.487840 lmql-0.0.6.4/src/lmql/ui/playground/src/editor/
--rw-rw-r--   0 luca      (1000) luca      (1000)     8696 2023-06-02 17:03:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     4758 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/editor/theme.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      889 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/explore.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     1345 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/graph-layout.css
--rw-rw-r--   0 luca      (1000) luca      (1000)     1698 2023-05-25 08:49:26.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/index.css
--rw-rw-r--   0 luca      (1000) luca      (1000)      489 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/index.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     2632 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/logo.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     8152 2023-06-08 13:54:23.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/queries.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     5990 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/remote_process.js
--rw-rw-r--   0 luca      (1000) luca      (1000)      362 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/reportWebVitals.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     9520 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/screenshot.css
--rw-rw-r--   0 luca      (1000) luca      (1000)      241 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/setupTests.js
--rw-rw-r--   0 luca      (1000) luca      (1000)     3466 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/spinner.svg
--rw-rw-r--   0 luca      (1000) luca      (1000)     3181 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/ui/playground/src/tagged-model-result.js
--rw-rw-r--   0 luca      (1000) luca      (1000)   449905 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/playground/yarn.lock
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.487840 lmql-0.0.6.4/src/lmql/ui/vscode/
--rw-rw-r--   0 luca      (1000) luca      (1000)       76 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/vscode/.gitattributes
--rw-rw-r--   0 luca      (1000) luca      (1000)       19 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/vscode/.gitignore
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.487840 lmql-0.0.6.4/src/lmql/ui/vscode/.vscode/
--rw-rw-r--   0 luca      (1000) luca      (1000)      540 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/vscode/.vscode/launch.json
--rw-rw-r--   0 luca      (1000) luca      (1000)       66 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/vscode/.vscodeignore
--rw-rw-r--   0 luca      (1000) luca      (1000)    23151 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql/ui/vscode/LICENSE
--rw-rw-r--   0 luca      (1000) luca      (1000)      357 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql/ui/vscode/README.md
--rw-rw-r--   0 luca      (1000) luca      (1000)      959 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/vscode/language-configuration.json
--rw-rw-r--   0 luca      (1000) luca      (1000)    11532 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql/ui/vscode/lmql-vscode.png
--rw-rw-r--   0 luca      (1000) luca      (1000)     1214 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql/ui/vscode/package.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.487840 lmql-0.0.6.4/src/lmql/ui/vscode/syntaxes/
--rw-rw-r--   0 luca      (1000) luca      (1000)      518 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      642 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
--rw-rw-r--   0 luca      (1000) luca      (1000)      853 2023-04-17 14:44:31.000000 lmql-0.0.6.4/src/lmql/ui/vscode/syntaxes/pylmql.json
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.487840 lmql-0.0.6.4/src/lmql/utils/
--rw-rw-r--   0 luca      (1000) luca      (1000)        0 2023-03-14 15:27:49.000000 lmql-0.0.6.4/src/lmql/utils/__init__.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2402 2023-05-11 15:13:38.000000 lmql-0.0.6.4/src/lmql/utils/docstring_parser.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     4933 2023-05-11 15:26:02.000000 lmql-0.0.6.4/src/lmql/utils/graph.py
--rw-rw-r--   0 luca      (1000) luca      (1000)     2592 2023-06-07 20:54:49.000000 lmql-0.0.6.4/src/lmql/utils/nputil.py
--rw-rw-r--   0 luca      (1000) luca      (1000)      115 2023-06-08 15:29:11.000000 lmql-0.0.6.4/src/lmql/version.py
-drwxrwxr-x   0 luca      (1000) luca      (1000)        0 2023-06-08 15:29:16.471840 lmql-0.0.6.4/src/lmql.egg-info/
--rw-rw-r--   0 luca      (1000) luca      (1000)     4991 2023-06-08 15:29:16.000000 lmql-0.0.6.4/src/lmql.egg-info/PKG-INFO
--rw-rw-r--   0 luca      (1000) luca      (1000)     8328 2023-06-08 15:29:16.000000 lmql-0.0.6.4/src/lmql.egg-info/SOURCES.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)        1 2023-06-08 15:29:16.000000 lmql-0.0.6.4/src/lmql.egg-info/dependency_links.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)       39 2023-06-08 15:29:16.000000 lmql-0.0.6.4/src/lmql.egg-info/entry_points.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)       95 2023-06-08 15:29:16.000000 lmql-0.0.6.4/src/lmql.egg-info/requires.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)        5 2023-06-08 15:29:16.000000 lmql-0.0.6.4/src/lmql.egg-info/top_level.txt
--rw-rw-r--   0 luca      (1000) luca      (1000)   115785 2023-04-17 14:48:56.000000 lmql-0.0.6.4/src/lmql.svg
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.120350 lmql-0.0.6.5/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.080351 lmql-0.0.6.5/.github/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.088351 lmql-0.0.6.5/.github/workflows/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2590 2023-07-14 15:52:52.000000 lmql-0.0.6.5/.github/workflows/lmql-ci.yml
+-rw-r--r--   0 docker    (1000) docker    (1000)     1543 2023-07-14 11:33:53.000000 lmql-0.0.6.5/.github/workflows/lmql-tests.yml
+-rw-r--r--   0 docker    (1000) docker    (1000)     2285 2023-07-14 11:31:18.000000 lmql-0.0.6.5/.github/workflows/lmql-web.yml
+-rw-r--r--   0 docker    (1000) docker    (1000)     2743 2023-07-14 11:31:18.000000 lmql-0.0.6.5/.gitignore
+-rw-r--r--   0 docker    (1000) docker    (1000)    23151 2023-07-14 11:31:18.000000 lmql-0.0.6.5/LICENSE
+-rw-r--r--   0 docker    (1000) docker    (1000)      140 2023-07-14 11:31:18.000000 lmql-0.0.6.5/MANIFEST.in
+-rw-r--r--   0 docker    (1000) docker    (1000)     9898 2023-07-14 15:57:02.120350 lmql-0.0.6.5/PKG-INFO
+-rw-r--r--   0 docker    (1000) docker    (1000)     9448 2023-07-14 15:36:31.000000 lmql-0.0.6.5/README.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.088351 lmql-0.0.6.5/docs/
+-rw-r--r--   0 docker    (1000) docker    (1000)      638 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/Makefile
+-rw-r--r--   0 docker    (1000) docker    (1000)      444 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/RELEASE.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      799 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/make.bat
+-rw-r--r--   0 docker    (1000) docker    (1000)       81 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/requirements.txt
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.088351 lmql-0.0.6.5/docs/source/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.088351 lmql-0.0.6.5/docs/source/_ext/
+-rw-r--r--   0 docker    (1000) docker    (1000)     5728 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/_ext/lmql_snippets.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.080351 lmql-0.0.6.5/docs/source/_static/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.088351 lmql-0.0.6.5/docs/source/_static/css/
+-rw-r--r--   0 docker    (1000) docker    (1000)     6010 2023-07-14 15:36:31.000000 lmql-0.0.6.5/docs/source/_static/css/lmql-docs.css
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.088351 lmql-0.0.6.5/docs/source/_static/images/
+-rw-r--r--   0 docker    (1000) docker    (1000)     3675 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/_static/images/lmql.svg
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.088351 lmql-0.0.6.5/docs/source/_static/js/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2087 2023-07-14 15:36:31.000000 lmql-0.0.6.5/docs/source/_static/js/lmql-playground.js
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.088351 lmql-0.0.6.5/docs/source/_templates/
+-rw-r--r--   0 docker    (1000) docker    (1000)      292 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/_templates/layout.html
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.088351 lmql-0.0.6.5/docs/source/blog/
+-rw-r--r--   0 docker    (1000) docker    (1000)     4591 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/blog/release-0.0.5.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     1444 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/blog/release-0.0.6.1.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     2068 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/blog/release-0.0.6.3.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     3221 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/blog/release-0.0.6.4.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     5349 2023-07-14 15:36:31.000000 lmql-0.0.6.5/docs/source/blog/release-0.0.6.5.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     8976 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/blog/release-0.0.6.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     1167 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/conf.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1293 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/dev-setup.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     2333 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/docker-setup.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.088351 lmql-0.0.6.5/docs/source/images/
+-rw-r--r--   0 docker    (1000) docker    (1000)   125712 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/images/inference.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)     2823 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/index.rst
+-rw-r--r--   0 docker    (1000) docker    (1000)     2563 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/installation.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.092351 lmql-0.0.6.5/docs/source/language/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2313 2023-07-14 15:36:31.000000 lmql-0.0.6.5/docs/source/language/azure.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     7435 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/language/constraints.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     5365 2023-07-14 15:36:31.000000 lmql-0.0.6.5/docs/source/language/decoders.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     7850 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/language/functions.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     3967 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/language/hf.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     2027 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/language/llama.cpp.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     2896 2023-07-14 15:36:31.000000 lmql-0.0.6.5/docs/source/language/models.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     5710 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/language/openai.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     8292 2023-07-14 15:36:31.000000 lmql-0.0.6.5/docs/source/language/overview.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     6032 2023-07-14 15:36:31.000000 lmql-0.0.6.5/docs/source/language/scripted_prompts.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     3675 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/lmql.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)    28444 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/logo.png
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.092351 lmql-0.0.6.5/docs/source/pending/
+-rw-r--r--   0 docker    (1000) docker    (1000)     3550 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/pending/release-next.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.092351 lmql-0.0.6.5/docs/source/python/
+-rw-r--r--   0 docker    (1000) docker    (1000)       11 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/python/.gitignore
+-rw-r--r--   0 docker    (1000) docker    (1000)     4924 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/python/comparison.md
+-rw-r--r--   0 docker    (1000) docker    (1000)    11193 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/python/langchain.ipynb
+-rw-r--r--   0 docker    (1000) docker    (1000)     1157 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/python/lc.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     6681 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/python/llama_index.ipynb
+-rw-r--r--   0 docker    (1000) docker    (1000)    75148 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/python/lmql.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)     7458 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/python/output.ipynb
+-rw-r--r--   0 docker    (1000) docker    (1000)     9592 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/python/pandas.ipynb
+-rw-r--r--   0 docker    (1000) docker    (1000)    13317 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/python/python.ipynb
+-rw-r--r--   0 docker    (1000) docker    (1000)     4806 2023-07-14 15:36:31.000000 lmql-0.0.6.5/docs/source/quickstart.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.092351 lmql-0.0.6.5/docs/source/releases/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2263 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/releases/misc-snippets.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      321 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/source/releases/release-0.0.5.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      257 2023-07-14 11:31:18.000000 lmql-0.0.6.5/docs/todo.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      137 2023-07-14 11:31:18.000000 lmql-0.0.6.5/pyproject.toml
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.092351 lmql-0.0.6.5/scripts/
+-rw-r--r--   0 docker    (1000) docker    (1000)      577 2023-07-14 11:31:18.000000 lmql-0.0.6.5/scripts/Dockerfile
+-rw-r--r--   0 docker    (1000) docker    (1000)      295 2023-07-14 11:31:18.000000 lmql-0.0.6.5/scripts/activate-dev.sh
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.092351 lmql-0.0.6.5/scripts/conda/
+-rw-r--r--   0 docker    (1000) docker    (1000)      198 2023-07-14 11:31:18.000000 lmql-0.0.6.5/scripts/conda/requirements-no-gpu.yml
+-rw-r--r--   0 docker    (1000) docker    (1000)      332 2023-07-14 11:31:18.000000 lmql-0.0.6.5/scripts/conda/requirements.yml
+-rw-r--r--   0 docker    (1000) docker    (1000)      638 2023-07-14 11:31:18.000000 lmql-0.0.6.5/scripts/pypi-release.sh
+-rw-r--r--   0 docker    (1000) docker    (1000)     3897 2023-07-14 11:31:18.000000 lmql-0.0.6.5/scripts/serve-all.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      854 2023-07-14 11:31:18.000000 lmql-0.0.6.5/scripts/wheel.sh
+-rw-r--r--   0 docker    (1000) docker    (1000)      868 2023-07-14 15:57:02.120350 lmql-0.0.6.5/setup.cfg
+-rw-r--r--   0 docker    (1000) docker    (1000)       37 2023-07-14 11:31:18.000000 lmql-0.0.6.5/setup.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.092351 lmql-0.0.6.5/src/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.092351 lmql-0.0.6.5/src/lmql/
+-rw-r--r--   0 docker    (1000) docker    (1000)     7767 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/__init__.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.096351 lmql-0.0.6.5/src/lmql/algorithms/
+-rw-r--r--   0 docker    (1000) docker    (1000)       45 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/algorithms/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2556 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/algorithms/cache.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      916 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/algorithms/functools.py
+-rwxr-xr-x   0 docker    (1000) docker    (1000)     8313 2023-07-14 11:38:09.000000 lmql-0.0.6.5/src/lmql/cli.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1578 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/demo.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1531 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/http.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.096351 lmql-0.0.6.5/src/lmql/language/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/language/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    27521 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/language/compiler.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    11042 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/language/fragment_parser.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4545 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/language/qstrings.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1804 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/language/validator.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.096351 lmql-0.0.6.5/src/lmql/models/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/__init__.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.096351 lmql-0.0.6.5/src/lmql/models/lmtp/
+-rw-r--r--   0 docker    (1000) docker    (1000)     6156 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/README.md
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.096351 lmql-0.0.6.5/src/lmql/models/lmtp/backends/
+-rw-r--r--   0 docker    (1000) docker    (1000)      493 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/backends/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      694 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/backends/__main__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4159 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/backends/llama_cpp_model.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4689 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/backends/lmtp_model.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2002 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/backends/random_model.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3906 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/backends/transformers_model.py
+-rw-r--r--   0 docker    (1000) docker    (1000)       42 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/errors.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4669 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_async.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5645 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_client.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    20101 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_dcmodel.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2283 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_inference_server.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5606 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_multiprocessing.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      298 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_programmatic_serve_example.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    15157 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_scheduler.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5685 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_serve.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3562 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_threading.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      634 2023-07-14 15:36:31.000000 lmql-0.0.6.5/src/lmql/models/lmtp/utils.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3396 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/models/model.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.096351 lmql-0.0.6.5/src/lmql/ops/
+-rw-r--r--   0 docker    (1000) docker    (1000)       93 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ops/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     7542 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ops/follow_map.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    41979 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ops/ops.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    21170 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ops/token_set.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.096351 lmql-0.0.6.5/src/lmql/output/
+-rw-r--r--   0 docker    (1000) docker    (1000)       57 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/output/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2334 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/output/http.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1889 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/output/sse.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2282 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/output/ws.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.100351 lmql-0.0.6.5/src/lmql/runtime/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/__init__.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.100351 lmql-0.0.6.5/src/lmql/runtime/bopenai/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2236 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/bopenai/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    29480 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/bopenai/batched_openai.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    21828 2023-07-14 15:36:31.000000 lmql-0.0.6.5/src/lmql/runtime/bopenai/openai_api.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2096 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/caching.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.100351 lmql-0.0.6.5/src/lmql/runtime/dclib/
+-rw-r--r--   0 docker    (1000) docker    (1000)      494 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/dclib/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    18839 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_array.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    26354 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_cache.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      592 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_global.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4970 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_model.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     8589 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_rewrite.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    32348 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_seq.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    22035 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/dclib/decoders.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    39770 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/interpreter.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      250 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/interrupt.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1231 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/langchain.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     8977 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/lmql_runtime.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1940 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/loop.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1245 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/maiohttp.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1726 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/masks.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3139 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/model_registry.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5943 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/multi_head_interpretation.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    44972 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/openai_integration.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1971 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/openai_secret.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4042 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/output_writer.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.100351 lmql-0.0.6.5/src/lmql/runtime/postprocessing/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/postprocessing/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3543 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/postprocessing/conditional_prob.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      152 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/postprocessing/group_by.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2209 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/program_state.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1317 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/stats.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2220 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/token_distribution.py
+-rw-r--r--   0 docker    (1000) docker    (1000)    11565 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/tokenizer.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.100351 lmql-0.0.6.5/src/lmql/runtime/tokenizers/
+-rw-r--r--   0 docker    (1000) docker    (1000)     4509 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/tokenizers/hf_tokenizer.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3427 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/tokenizers/pure_python_tokenizer.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3207 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/runtime/tokenizers/tiktoken_tokenizer.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.104351 lmql-0.0.6.5/src/lmql/tests/
+-rw-r--r--   0 docker    (1000) docker    (1000)      319 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/README.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      907 2023-07-14 11:44:57.000000 lmql-0.0.6.5/src/lmql/tests/all.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5914 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/expr_test_utils.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1314 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/fin_and.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.104351 lmql-0.0.6.5/src/lmql/tests/outdated/
+-rw-r--r--   0 docker    (1000) docker    (1000)     1611 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/outdated/mask_product_test.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2789 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/outdated/monotonicity.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      546 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/outdated/one_of_tests.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      758 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/outdated/sentences_op.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      984 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/outdated/starts_with_op_test.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1236 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/outdated/stops_at.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      537 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/outdated/str_in_str_tests.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4738 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/outdated/test_multi_head.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3036 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/outdated/token_set_test.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.104351 lmql-0.0.6.5/src/lmql/tests/queryargs/
+-rw-r--r--   0 docker    (1000) docker    (1000)     4489 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/queryargs/test_args.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2072 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/queryargs/test_args_query_str.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1095 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/queryargs/test_args_run.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1066 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/queryargs/test_sync.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1092 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/queryargs/test_var_errors.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.104351 lmql-0.0.6.5/src/lmql/tests/system/
+-rw-r--r--   0 docker    (1000) docker    (1000)     3402 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/system/basic_use_cases.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      842 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/tail_token_set.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      788 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_back2back_caching.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      335 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_beam_in.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2775 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_eq.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1756 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_escaping.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      877 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_local_model_python.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1444 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_minimal_syntax.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1139 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_multibyte_characters.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1171 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_multibyte_local_models.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      457 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_orop.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2931 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_qstrings.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      479 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_query_args.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2639 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_sample_queries.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1703 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_scoping.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3647 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/test_stopping.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      707 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/tests/tiktoken_tsets.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.104351 lmql-0.0.6.5/src/lmql/ui/
+-rw-r--r--   0 docker    (1000) docker    (1000)       27 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/.gitignore
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/__init__.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.108351 lmql-0.0.6.5/src/lmql/ui/live/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/live/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     6747 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/live/live.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     3475 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/live/live.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     3885 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/live/livelib.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      349 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/live/package.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    33701 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/live/yarn.lock
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.108351 lmql-0.0.6.5/src/lmql/ui/playground/
+-rw-r--r--   0 docker    (1000) docker    (1000)       31 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/.dockerignore
+-rw-r--r--   0 docker    (1000) docker    (1000)       34 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/.env
+-rw-r--r--   0 docker    (1000) docker    (1000)      310 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/.gitignore
+-rw-r--r--   0 docker    (1000) docker    (1000)      354 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/Dockerfile
+-rw-r--r--   0 docker    (1000) docker    (1000)     3359 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/README.md
+-rw-r--r--   0 docker    (1000) docker    (1000)     1327 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/package.json
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.108351 lmql-0.0.6.5/src/lmql/ui/playground/public/
+-rw-r--r--   0 docker    (1000) docker    (1000)       90 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/_headers
+-rw-r--r--   0 docker    (1000) docker    (1000)     3870 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/favicon.ico
+-rw-r--r--   0 docker    (1000) docker    (1000)     1678 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/index.html
+-rw-r--r--   0 docker    (1000) docker    (1000)     2817 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/lmql.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)      306 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/manifest.json
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.112351 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/
+-rw-r--r--   0 docker    (1000) docker    (1000)  1227728 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/calc.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   295285 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/chat.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   160131 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/cot.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    81768 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/distribution.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    22895 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/hello.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    89531 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/joke.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   265372 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/json-template.json
+-rw-r--r--   0 docker    (1000) docker    (1000)  1710847 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/kv.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    52748 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/list.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   628184 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/meta.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   264768 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/translation.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   215050 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/wiki.json
+-rw-r--r--   0 docker    (1000) docker    (1000)       67 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/robots.txt
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.116351 lmql-0.0.6.5/src/lmql/ui/playground/public/snippets/
+-rw-r--r--   0 docker    (1000) docker    (1000)   381736 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/snippets/dynamic-cfg.json
+-rw-r--r--   0 docker    (1000) docker    (1000)   184008 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/public/snippets/json-parsing.json
+-rw-r--r--   0 docker    (1000) docker    (1000)       62 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/ref.py
+-rw-r--r--   0 docker    (1000) docker    (1000)       80 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/run-in-docker.sh
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.116351 lmql-0.0.6.5/src/lmql/ui/playground/src/
+-rw-r--r--   0 docker    (1000) docker    (1000)    75521 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/App.jsx
+-rw-r--r--   0 docker    (1000) docker    (1000)      246 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/App.test.js
+-rw-r--r--   0 docker    (1000) docker    (1000)    29983 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/CodeScreenshot.jsx
+-rw-r--r--   0 docker    (1000) docker    (1000)      807 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/Configuration.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     1174 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/DataListView.js
+-rw-r--r--   0 docker    (1000) docker    (1000)    21617 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/DecoderGraph.js
+-rw-r--r--   0 docker    (1000) docker    (1000)      329 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/DecodingTree.js
+-rw-r--r--   0 docker    (1000) docker    (1000)       89 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/Embed.jsx
+-rw-r--r--   0 docker    (1000) docker    (1000)     9601 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/Explore.jsx
+-rw-r--r--   0 docker    (1000) docker    (1000)      675 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/SharedState.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     4819 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/State.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     5871 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/ValidationGraph.jsx
+-rw-r--r--   0 docker    (1000) docker    (1000)     9360 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/browser_process.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     1163 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/build_info.js
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.120350 lmql-0.0.6.5/src/lmql/ui/playground/src/editor/
+-rw-r--r--   0 docker    (1000) docker    (1000)     8696 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/editor/lmql-monaco-language.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     4758 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/editor/theme.json
+-rw-r--r--   0 docker    (1000) docker    (1000)      889 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/explore.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)     1345 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/graph-layout.css
+-rw-r--r--   0 docker    (1000) docker    (1000)     1698 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/index.css
+-rw-r--r--   0 docker    (1000) docker    (1000)      489 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/index.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     2632 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/logo.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)     8766 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/queries.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     5990 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/remote_process.js
+-rw-r--r--   0 docker    (1000) docker    (1000)      362 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/reportWebVitals.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     9520 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/screenshot.css
+-rw-r--r--   0 docker    (1000) docker    (1000)      241 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/setupTests.js
+-rw-r--r--   0 docker    (1000) docker    (1000)     3466 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/spinner.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)     3200 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/src/tagged-model-result.js
+-rw-r--r--   0 docker    (1000) docker    (1000)   449905 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/playground/yarn.lock
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.120350 lmql-0.0.6.5/src/lmql/ui/vscode/
+-rw-r--r--   0 docker    (1000) docker    (1000)       76 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/.gitattributes
+-rw-r--r--   0 docker    (1000) docker    (1000)       19 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/.gitignore
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.120350 lmql-0.0.6.5/src/lmql/ui/vscode/.vscode/
+-rw-r--r--   0 docker    (1000) docker    (1000)      540 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/.vscode/launch.json
+-rw-r--r--   0 docker    (1000) docker    (1000)       66 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/.vscodeignore
+-rw-r--r--   0 docker    (1000) docker    (1000)    23151 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/LICENSE
+-rw-r--r--   0 docker    (1000) docker    (1000)      357 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/README.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      959 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/language-configuration.json
+-rw-r--r--   0 docker    (1000) docker    (1000)    11532 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/lmql-vscode.png
+-rw-r--r--   0 docker    (1000) docker    (1000)     1214 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/package.json
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.120350 lmql-0.0.6.5/src/lmql/ui/vscode/syntaxes/
+-rw-r--r--   0 docker    (1000) docker    (1000)      518 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/syntaxes/lmql.qstring.json
+-rw-r--r--   0 docker    (1000) docker    (1000)      642 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json
+-rw-r--r--   0 docker    (1000) docker    (1000)      853 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/ui/vscode/syntaxes/pylmql.json
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.120350 lmql-0.0.6.5/src/lmql/utils/
+-rw-r--r--   0 docker    (1000) docker    (1000)        0 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/utils/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2402 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/utils/docstring_parser.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     4933 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/utils/graph.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     2715 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql/utils/nputil.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      114 2023-07-14 15:56:54.000000 lmql-0.0.6.5/src/lmql/version.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2023-07-14 15:57:02.092351 lmql-0.0.6.5/src/lmql.egg-info/
+-rw-r--r--   0 docker    (1000) docker    (1000)     9898 2023-07-14 15:57:01.000000 lmql-0.0.6.5/src/lmql.egg-info/PKG-INFO
+-rw-r--r--   0 docker    (1000) docker    (1000)     9141 2023-07-14 15:57:02.000000 lmql-0.0.6.5/src/lmql.egg-info/SOURCES.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)        1 2023-07-14 15:57:01.000000 lmql-0.0.6.5/src/lmql.egg-info/dependency_links.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)       39 2023-07-14 15:57:01.000000 lmql-0.0.6.5/src/lmql.egg-info/entry_points.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)       95 2023-07-14 15:57:01.000000 lmql-0.0.6.5/src/lmql.egg-info/requires.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)        5 2023-07-14 15:57:01.000000 lmql-0.0.6.5/src/lmql.egg-info/top_level.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)   115785 2023-07-14 11:31:18.000000 lmql-0.0.6.5/src/lmql.svg
+-rw-r--r--   0 docker    (1000) docker    (1000)       86 2023-07-14 11:31:18.000000 lmql-0.0.6.5/yarn.lock
```

### Comparing `lmql-0.0.6.4/.github/workflows/lmql-web.yml` & `lmql-0.0.6.5/.github/workflows/lmql-web.yml`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/.gitignore` & `lmql-0.0.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/LICENSE` & `lmql-0.0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/Makefile` & `lmql-0.0.6.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/make.bat` & `lmql-0.0.6.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/_ext/lmql_snippets.py` & `lmql-0.0.6.5/docs/source/_ext/lmql_snippets.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,18 +92,21 @@
     has_content = True
 
     def run(self):
         code = []
         output = []
         is_output = False
         name = None
+        noplayground = False
 
         for l in self.content:
             if l.startswith("name::"):
                 name = l[6:]
+            elif l.startswith("noplayground::"):
+                noplayground = True
             elif l.startswith("model-output::"):
                 is_output = True
             else:
                 if is_output: output += [l]
                 else: code += [l]
         
         code = "\n".join(code)
@@ -119,15 +122,18 @@
         snippet_id = os.path.relpath(self.state.document.current_source, self.state.document.settings.env.srcdir)
         # replace all but A-z0-9 with -
         snippet_id = "".join([c if c.isalnum() else "-" for c in snippet_id])
         snippet_id += "-" + name
 
         # create output
         paragraph_node = nodes.paragraph()
-        prefix = """<button href onclick="openPlaygroundSnippet(this, 'doc-snippets/{}')">Open In Playground</button>""".format(snippet_id)
+        if not noplayground:
+            prefix = """<button href onclick="openPlaygroundSnippet(this, 'doc-snippets/{}')">Open In Playground</button>""".format(snippet_id)
+        else:
+            prefix = ""
 
         code = highlight(code, LmqlLexer(), HtmlFormatter(cssclass="highlight lmql"))
         code = code.replace("""<div class="highlight lmql">""", """<div class="highlight lmql">""" + prefix)
         
         # model output highlight
         if len(output) > 0:
             print(output_format(output), flush=True)
```

### Comparing `lmql-0.0.6.4/docs/source/_static/css/lmql-docs.css` & `lmql-0.0.6.5/docs/source/_static/css/lmql-docs.css`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,30 @@
     border: 1pt solid rgb(110, 109, 109);
 }
 
 .highlight.lmql iframe {
     background-color: var(--pst-color-background);
 }
 
+.highlight.lmql pre {
+    line-height: 1.55em !important;
+}
+
 .highlight.lmql.playground {
     border: none;
 }
 
 .highlight.lmql pre {
     border: none;
 }
 
+.highlight.lmql pre span.c1 {
+    opacity: 0.5 !important;
+}
+
 .highlight pre {
     padding-top: 20pt !important;
     padding-bottom: 20pt !important;
 }
 
 .highlight.lmql button {
     background: transparent;
@@ -164,15 +172,15 @@
 
 .nboutput .highlight pre {
     /* break lines */
     white-space: break-spaces !important;
 }
 
 .highlight-model-output::before {
-    content: "Model Output";
+    content: "Model Transcript";
     font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
     position: absolute;
     top: 4pt;
     font-size: 9pt;
     text-transform: uppercase;
     left: 0pt;
     z-index: 2;
```

### Comparing `lmql-0.0.6.4/docs/source/_static/images/lmql.svg` & `lmql-0.0.6.5/docs/source/_static/images/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/_static/js/lmql-playground.js` & `lmql-0.0.6.5/docs/source/_static/js/lmql-playground.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -5,18 +5,16 @@
 
     if (next) {
         return "https://next.lmql.ai/playground";
     }
 
     if (host === "docs.lmql.ai") {
         return "https://lmql.ai/playground";
-    } else if (host.startsWith("localhost") || host.startsWith("127.0.0.1")) {
-        return "http://localhost:3000/playground";
     } else {
-        return "https://lbeurerkellner.github.io/green-gold-dachshund-web/playground";
+        return "http://localhost:8081/playground/";
     }
 }
 
 function closePlaygroundSnippet() {
     if (openPlaygroundElement) {
         openPlaygroundElement.innerHTML = openPlaygroundElement.originalHTML;
         openPlaygroundElement.classList.remove('playground');
```

### Comparing `lmql-0.0.6.4/docs/source/blog/release-0.0.5.md` & `lmql-0.0.6.5/docs/source/blog/release-0.0.5.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/blog/release-0.0.6.1.md` & `lmql-0.0.6.5/docs/source/blog/release-0.0.6.1.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/blog/release-0.0.6.3.md` & `lmql-0.0.6.5/docs/source/blog/release-0.0.6.3.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/blog/release-0.0.6.md` & `lmql-0.0.6.5/docs/source/blog/release-0.0.6.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/conf.py` & `lmql-0.0.6.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/dev-setup.md` & `lmql-0.0.6.5/docs/source/dev-setup.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/docker-setup.md` & `lmql-0.0.6.5/docs/source/docker-setup.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/images/inference.svg` & `lmql-0.0.6.5/docs/source/images/inference.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/index.rst` & `lmql-0.0.6.5/docs/source/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,15 @@
     :caption: 🔗 Python Integration
     
     python/python.ipynb
     python/langchain.ipynb
     python/llama_index.ipynb
     python/pandas.ipynb
     python/output.md
+    python/comparison.md
    
 .. toctree::
     :maxdepth: 1
     :caption: 💬 Contribute
     
     dev-setup
     docker-setup
```

#### html2text {}

```diff
@@ -21,12 +21,12 @@
 Contents -------- .. toctree:: :maxdepth: 1 quickstart installation â¡ï¸
 Playground IDE
 lmql.ai/playground> .. toctree:: :maxdepth: 1 :caption: ð LMQL Language
 language/overview.md language/scripted_prompts.md language/constraints.md
 language/decoders.md language/models.md language/functions.md .. toctree:: :
 maxdepth: 1 :caption: ð Python Integration python/python.ipynb python/
 langchain.ipynb python/llama_index.ipynb python/pandas.ipynb python/output.md
-.. toctree:: :maxdepth: 1 :caption: ð¬ Contribute dev-setup docker-setup
-Discord
+python/comparison.md .. toctree:: :maxdepth: 1 :caption: ð¬ Contribute dev-
+setup docker-setup Discord
 discord.gg/7eJP4fcyNT> GitHub Issues
 github.com/eth-sri/lmql/issues> E-Mail
 lmql.ai>
```

### Comparing `lmql-0.0.6.4/docs/source/installation.md` & `lmql-0.0.6.5/docs/source/installation.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/language/constraints.md` & `lmql-0.0.6.5/docs/source/language/constraints.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/language/decoders.md` & `lmql-0.0.6.5/docs/source/language/decoders.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,47 @@
 
 LMQL support various decoding algorithms, which are used to generate text from the token distribution of a language model. The decoding algorithm in use, is specified right at the beginning of a query, e.g. `argmax`. Here, we provide a brief overview of the currently supported decoders.
 
 LMQL also includes a library for array-based decoding `dclib`, which can be used to implement custom decoders. More information on this, will be provided in the future. The implementation of the available decoding procedures is located in `src/lmql/runtime/dclib/decoders.py` of the LMQL repository.
 
 In general, all LMQL decoding algorithms are model-agnostic and can be used with any LMQL-supported inference backend. For more information on the supported inference backends, see the [Models](./models.md) chapter.
 
+## Specifying The Decoding Algorithm
+
+Depending on the context, LMQL offers two ways to specify the decoding algorithm to use. 
+
+**Queries with Decoding Clause**: The first option is to simply specify the decoding algorithm and its parameters as part of the query itself. This can be particularly useful, if your choice of decoder is relevant and should be part of your program.
+
+```{lmql}
+
+name::specify-decoder
+beam(n=2)
+    "This is a query with a specified decoder: [RESPONSE]
+from
+    "openai/text-ada-001"
+```
+
+**Specifying the Decoding Algorithm Externally**: The second option is to specify the decoding algorithm and parameters externally, i.e. separatly from the actual program code:
+
+```python
+import lmql
+
+@lmql.query(model="openai/text-davinci-003", decoder="sample", temperature=1.8)
+def tell_a_joke():
+    '''lmql
+    """A list good dad joke. A indicates the punchline:
+    Q:[JOKE]
+    A:[PUNCHLINE]""" where STOPS_AT(JOKE, "?") and  STOPS_AT(PUNCHLINE, "\n")
+    '''
+
+tell_a_joke() # uses the decoder specified in @lmql.query(...)
+tell_a_joke(decoder="beam", n=2) # uses a beam search decoder with n=2
+```
+
+This is only possible when using LMQL from a Python program. For more information on this, also see the chapter on how to specify the [model to use for decoding](models.md).
 ## Supported Decoding Algorithms
 
 In general, the very first keyword of an LMQL query, specifies the decoding algorithm to use. For this, the following decoder keywords are available:
 
 ### `argmax`
 
 The `argmax` decoder is the simplest decoder available in LMQL. It greedily selects the most likely token at each step of the decoding process. It has no additional parameters. Since `argmax` decoding is deterministic, one can only generate a single sequence at a time.
```

### Comparing `lmql-0.0.6.4/docs/source/language/functions.md` & `lmql-0.0.6.5/docs/source/language/functions.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/language/hf.md` & `lmql-0.0.6.5/docs/source/language/hf.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/language/openai.md` & `lmql-0.0.6.5/docs/source/language/openai.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/language/overview.md` & `lmql-0.0.6.5/docs/source/language/overview.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,140 +1,127 @@
 # Overview
 
-LMQL is a declarative, SQL-like programming language for language model interaction. As an example consider the following query, demonstrating the basic syntax of LMQL:
+LMQL is a Python-based programming language for LLM programming with declarative elements. As a simple example consider the following program, demonstrating the basic syntax of LMQL:
 
 ```{lmql}
 
 name::overview-query
-argmax
-   """Review: We had a great stay. Hiking in the mountains was fabulous and the food is really good.
-   Q: What is the underlying sentiment of this review and why?
-   A:[ANALYSIS]
-   Based on this, the overall sentiment of the message can be considered to be[CLASSIFICATION]"""
-from
-   "openai/text-davinci-003"
-where
-   not "\n" in ANALYSIS and CLASSIFICATION in [" positive", " neutral", " negative"]
+
+# review to be analyzed
+review = """We had a great stay. Hiking in the mountains 
+            was fabulous and the food is really good."""
+
+# use prompt statements to pass information to the model
+"Review: {review}"
+"Q: What is the underlying sentiment of this review and why?"
+# template variables like [ANALYSIS] are used to generate text
+"A:[ANALYSIS]" where not "\n" in ANALYSIS
+
+# use constrained variable to produce a classification
+"Based on this, the overall sentiment of the message\
+ can be considered to be[CLS]" where CLS in [" positive", " neutral", " negative"]
+
+CLS # positive
 
 model-output::
 Review: We had a great stay. Hiking in the mountains was fabulous and the food is really good.⏎
 Q: What is the underlying sentiment of this review and why?⏎
 A: [ANALYSIS The underlying sentiment of this review is positive because the reviewer had a great stay, enjoyed the hiking and found the food to be good.]⏎
-Based on this, the overall sentiment of the message can be considered to be [CLASSIFICATION positive]
+Based on this, the overall sentiment of the message can be considered to be [CLS positive]
 ```
 
-In this program, we use the language model `openai/text-davinci-003` (GPT-3.5) to perform a sentiment analysis on a provided user review. We first ask the model to provide some basic analysis of the review, and then we ask the model to classify the overall sentiment as one of `positive`, `neutral`, or `negative`. The model is able to correctly identify the sentiment of the review as `positive`.
-
-Overall, the query consists of four main clauses:
-
-1. **Decoder Clause** First, we specify the decoding algorithm to use for text generation. In this case we use `argmax` decoding, however, LMQL also support branching decoding algorithms like beam search. See [Decoders](./decoders.md) to learn more about this.
-
-2. **Prompt Clause**
-
-   ```python
-   """Review: We had a great stay. Hiking in the mountains was fabulous and the food is really good.
-   Q: What is the underlying sentiment of this review and why?
-   A:[ANALYSIS]
-   Based on this, the overall sentiment of the message can be considered to be[CLASSIFICATION]"""
-   ```
-
-   In this part of the program, you specify your prompt. Here, we include the user review, as well as the two questions we want to ask the model. Template variables like `[ANALYSIS]` are automatically completed by the model. Apart from simple textual prompts, LMQL also support multi-part and scripted prompts. To learn more, see [Scripted Prompting](./scripted_prompts.md).
+In this program, we program an LLM to perform sentiment analysis on a provided user review. We first ask the model to provide some basic analysis, and then we ask it to classify the overall sentiment as one of `positive`, `neutral`, or `negative`. The model is able to correctly identify the sentiment of the review as `positive`.
 
-3. **Model Clause**
+To implement this workflow, we use two template variables `[ANALYSIS]` and `[CLS]`, both of which are constrained using designated `where` expressions. 
 
-    ```python
-    from "openai/text-davinci-003"
-    ```
+For `ANALYSIS` we constrain the model to not output any newlines, which prevents it from outputting multiple lines that could potentially break the program. For `CLS` we constrain the model to output one of the three possible values. Using these constraints allows us to decode a fitting answer from the model, where both the analysis and the classification are well-formed and in an expected format.
 
-    Next, we specify what model we want to use for text generation. In this case, we use the language model `openai/text-davinci-003`. To learn more about the different models available in LMQL, see [Models](./models.md).
-
-4. **Constraint Clause**
-
-    ```python
-    not "\n" in ANALYSIS and CLASSIFICATION in [" positive", " neutral", " negative"]
-    ```
-
-    In this part of the query, users can specify logical, high-level constraints on the generated text.<br>
-    
-    Here, we specify two constraints: For `ANALYSIS` we constrain the model to not output any newlines, which prevents the model from outputting multiple lines, which could potentially breaking the prompt. For `CLASSIFICATION` we constrain the model to output one of the three possible values. Using these constraints allows us to decode a fitting answer from the model, where both the analysis and the classification are well-formed and in an expected format.
-
-   Without constraints, the prompt above could produce different final classifications, such as `good`, `bad`, or `neutral`. To handle this in an automated way, one would again have to employ some model of language understanding to parse the model's CLASSIFICATION result.
-
-   To learn more about the different types of constraints available in LMQL, see [Constraints](./constraints.md).
+Without constraints, the prompt above could produce different final classifications, such as `good` or `bad`. To handle this in an automated way, one would have to employ ad-hoc parsing to CLS result to obtain a clear result. Using LMQL's constraints, however, we can simply restrict the model to only output one of the desired values, thereby enabling robust and reliable integration. To learn more about the different types of constraints available in LMQL, see [Constraints](./constraints.md).
 
 ### Extracting More Information With Distributions
 
 While the query above allows us to extract the sentiment of a review, we do not get any certainty information on the model's confidence in its classification. To obtain this information, we can additionally employ LMQL's `distribution` clause, to obtain the full distribution over the possible values for `CLASSIFICATION`:
 
 ```{lmql}
 
 name::sentiment-distribution
 argmax
-   """Review: We had a great stay. Hiking in the mountains was fabulous and the food is really good.
-   Q: What is the underlying sentiment of this review and why?
-   A:[ANALYSIS]
-   Based on this, the overall sentiment of the message can be considered to be[CLASSIFICATION]"""
-from
-   "openai/text-davinci-003"
-where
-   not "\n" in ANALYSIS
+    # review to be analyzed
+    review = """We had a great stay. Hiking in the mountains was fabulous and the food is really good."""
+
+    # use prompt statements to pass information to the model
+    "Review: {review}"
+    "Q: What is the underlying sentiment of this review and why?"
+    # template variables like [ANALYSIS] are used to generate text
+    "A:[ANALYSIS]" where not "\n" in ANALYSIS
+
+    # use constrained variable to produce a classification
+    "Based on this, the overall sentiment of the message can be considered to be[CLS]"
 distribution
-   CLASSIFICATION in [" positive", " neutral", " negative"]
+   CLS in [" positive", " neutral", " negative"]
 
 model-output::
 Review: We had a great stay. Hiking in the mountains was fabulous and the food is really good.⏎
 Q: What is the underlying sentiment of this review and why?⏎
 A: [ANALYSIS The underlying sentiment of this review is positive because the reviewer had a great stay, enjoyed the hiking and found the food to be good.]⏎
-Based on this, the overall sentiment of the message can be considered to be [CLASSIFICATION]
+Based on this, the overall sentiment of the message can be considered to be [CLS]
 
-P(CLASSIFICATION)
+P(CLS)
  -  positive (*) 0.9999244826658527
  -  neutral      7.513155848720942e-05
  -  negative     3.8577566019560874e-07
 ```
 
 **Distribution Clause**
 
-Instead of constraining `CLASSIFICATION` as part of the `where` clause, we now constrain in the `distribution` clause. In LMQL, the `distribution` clause is used to specify whether we want to additionally obtain the distribution over the possible values for a given variable. In this case, we want to obtain the distribution over the possible values for `CLASSIFICATION`.
+Instead of constraining `CLS` with a `where` expression, we now constrain it in the separate `distribution` clause. In LMQL, the `distribution` clause can be used to specify whether we want to additionally obtain the distribution over the possible values for a given variable. In this case, we want to obtain the distribution over the possible values for `CLS`. 
 
-In addition to using the model to perform the `ANALYSIS`, LMQL now also scores each of the individually provided values for `CLASSIFICATION` and normalizes the resulting sequence scores into a probability distribution `P(CLASSIFICATION)` (printed to the Terminal Output of the Playground or Standard Output of the CLI).
+> **Extended Syntax**: Note, that to use the `distribution` clause, we have to make our choice of decoding algorithm explicit, by specifying `argmax` at the beginning of our code (see [Decoding Algorithms](./decoding.md) for more information). ¸
+>
+> In general, this extended form of LMQL syntax, i.e. indenting your program and explicitly specifying e.g. `argmax` at the beginning of your code, is optional, but recommended if you want to use the `distribution` clause. Throughout the documentation we will make use of both syntax variants.
+
+In addition to using the model to perform the `ANALYSIS`, LMQL now also scores each of the individually provided values for `CLS` and normalizes the resulting sequence scores into a probability distribution `P(CLS)` (printed to the Terminal Output of the Playground or Standard Output of the CLI).
 
 Here, we can see that the model is indeed quite confident in its classification of the review as `positive`, with an overwhelming probability of `99.9%`.
 
-> Note that currently distribution variables like `CLASSIFICATION` can only occur at the end of a prompt.
+> Note that currently distribution variables like `CLS` can only occur at the end of your program.
 
 ### Dynamically Reacting To Model Output
 
 Another way to improve on our initial query, is to implement a more dynamic prompt, where we can react to the model's output. For example, we could ask the model to provide a more detailed analysis of the review, depending on the model's classification:
 
 ```{lmql}
 
 name::dynamic-analysis
 argmax
-   """Review: We had a great stay. Hiking in the mountains was fabulous and the food is really good.
+   review = """We had a great stay. Hiking in the mountains 
+               was fabulous and the food is really good."""
+   """Review: {review}
    Q: What is the underlying sentiment of this review and why?
-   A:[ANALYSIS]
-   Based on this, the overall sentiment of the message can be considered to be[CLASSIFICATION]"""
-   if CLASSIFICATION == " positive":
+   A:[ANALYSIS]""" where not "\n" in ANALYSIS
+   
+   "Based on this, the overall sentiment of the message can be considered to be[CLS]" where CLS in [" positive", " neutral", " negative"]
+   
+   if CLS == " positive":
       "What is it that they liked about their stay? [FURTHER_ANALYSIS]"
-   elif CLASSIFICATION == " neutral":
+   elif CLS == " neutral":
       "What is it that could have been improved? [FURTHER_ANALYSIS]"
-   elif CLASSIFICATION == " negative":
+   elif CLS == " negative":
       "What is it that they did not like about their stay? [FURTHER_ANALYSIS]"
-from
-    "openai/text-davinci-003"
 where
-    not "\n" in ANALYSIS and CLASSIFICATION in [" positive", " neutral", " negative"] and STOPS_AT(FURTHER_ANALYSIS, ".")
+   STOPS_AT(FURTHER_ANALYSIS, ".")
 
 model-output::
 Review: We had a great stay. Hiking in the mountains was fabulous and the food is really good.⏎
 Q: What is the underlying sentiment of this review and why?⏎
 A: [ANALYSIS The underlying sentiment of this review is positive because the reviewer had a great stay, enjoyed the hiking and found the food to be good.]⏎
 Based on this, the overall sentiment of the message can be considered to be [CLASSIFICATION positive]⏎
 What is it that they liked about their stay?⏎
 ⏎
 [FURTHER_ANALYSIS The reviewer liked the hiking in the mountains and the food.]
 ```
 
 As shown here, we can use the `if` statement to dynamically react to the model's output. In this case, we ask the model to provide a more detailed analysis of the review, depending on the overall positive, neutral, or negative sentiment of the review. All intermediate variables like `ANALYSIS`, `CLASSIFICATION` or `FURTHER_ANALYSIS` can be considered the output of query, and may be processed by an surrounding automated system.
 
 To learn more about the capabilities of such control-flow-guided prompts, see [Scripted Prompting](./scripted_prompts.md).
+
+As shown here, in addition to inline `where` expressions as seen earlier, you can also provide a global `where` expression at the end of your program, e.g. to specify constraints that should apply for all variables. Depending on your use case, this can be a convenient way to avoid having to repeat the same constraints multiple times, like for `FURTHER_ANALYSIS` in this example.
```

### Comparing `lmql-0.0.6.4/docs/source/lmql.svg` & `lmql-0.0.6.5/docs/source/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/logo.png` & `lmql-0.0.6.5/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/pending/release-next.md` & `lmql-0.0.6.5/docs/source/pending/release-next.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/python/langchain.ipynb` & `lmql-0.0.6.5/docs/source/python/langchain.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/python/lc.py` & `lmql-0.0.6.5/docs/source/python/lc.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/python/llama_index.ipynb` & `lmql-0.0.6.5/docs/source/python/llama_index.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/python/lmql.txt` & `lmql-0.0.6.5/docs/source/python/lmql.txt`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/python/output.ipynb` & `lmql-0.0.6.5/docs/source/python/output.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/python/pandas.ipynb` & `lmql-0.0.6.5/docs/source/python/pandas.ipynb`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/docs/source/releases/misc-snippets.md` & `lmql-0.0.6.5/docs/source/releases/misc-snippets.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/scripts/Dockerfile` & `lmql-0.0.6.5/scripts/Dockerfile`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/scripts/serve-all.py` & `lmql-0.0.6.5/scripts/serve-all.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/scripts/wheel.sh` & `lmql-0.0.6.5/scripts/wheel.sh`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# fail if any commands fails
+set -e
+
 COMMIT=$(git rev-parse HEAD)
 HAS_UNSTAGED=$(git diff-index --quiet HEAD -- src; echo $?)
 
 if [ $HAS_UNSTAGED -eq 1 ]; then
     echo "Unstaged changes detected. Please commit or stash them before packaging for PyPI."
     echo $(git diff-index HEAD -- src)
     exit 1
```

### Comparing `lmql-0.0.6.4/setup.cfg` & `lmql-0.0.6.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lmql
-version = 0.0.6.4
+version = 0.0.6.5
 author = Luca Beurer-Kellner, Marc Fischer, Martin Vechev
 author_email = hello@lmql.ai
 description = A query language for language models.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://lmql.ai
 project_urls =
```

### Comparing `lmql-0.0.6.4/src/lmql/__init__.py` & `lmql-0.0.6.5/src/lmql/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,16 @@
                                        EmptyVariableScope)
 from lmql.runtime.model_registry import LMQLModelRegistry
 from lmql.runtime.output_writer import headless, printing, silent, stream
 from lmql.runtime.interpreter import LMQLResult
 from lmql.models.model import model
 from lmql.runtime.loop import main
 
+from typing import Optional
+
 model_registry = LMQLModelRegistry
 
 def connect(server="http://localhost:8080", model_name="EleutherAI/gpt-j-6B"):
     print("warning: connect() is deprecated. Use set_backend() instead.")
 
 def autoconnect():
     model_registry.autoconnect = True
@@ -53,75 +55,79 @@
 
     module = module.load()
     module.query.force_model(force_model)
     return module
 
 async def run_file(filepath, *args, output_writer=None, force_model=None, **kwargs):
     import inspect
-    module = load(filepath, autoconnect=True, output_writer=output_writer, force_model=force_model)
+    with open(filepath, "r") as f:
+        code = f.read()
     
-    if module is None: 
-        print("Failed to compile query.")
-        return
-
-    if output_writer is not None:
-        module.query.output_writer = output_writer
-
-    compiled_fct_args = module.query.args
-    query_args = []
-
-    calling_frame = inspect.stack()[1]
-    scope = LMQLInputVariableScope(module.query.fct, calling_frame)
-    for arg in compiled_fct_args:
-        if scope.resolve(arg) == None:
-            query_args.append(arg)
-
-    output_variables = module.query.output_variables
-    query_args = list(set(query_args) - set(output_variables))
-
-    return await module.query(*args, **kwargs)
+    q = _query_from_string(code, output_writer=printing)
+    return await q(*args, **kwargs)
 
 async def run(code, *args, **kwargs):
     """
     Compiles and runs the given query string asynchronously.
 
     For synchronous execution (w/o await), use `lmql.run_sync` instead.
     """
-    q = _query_from_string(code)
+    q = _query_from_string(code, output_writer=kwargs.get("output_writer", None))
     return await q(*args, **kwargs)
         
 def run_sync(code, *args, **kwargs):
     """
     Compiles and runs the given query string synchronously.
 
     For async execution, use `lmql.run` instead.
     """
     q = _query_from_string(code, is_async=False)
     return q(*args, **kwargs)
 
-def _query_from_string(s, input_variables=None, is_async=True):
+def _query_from_string(s, input_variables=None, is_async=True, output_writer=None, **extra_args):
     if input_variables is None: input_variables = []
 
     import inspect
     temp_lmql_file = tempfile.mktemp(suffix=".lmql")
     with open(temp_lmql_file, "w") as f:
         f.write(s)
-    module = load(temp_lmql_file, autoconnect=True, output_writer=silent)
+    module = load(temp_lmql_file, autoconnect=True, output_writer=output_writer or silent)
     
     # lmql.query(str) does not capture function context
     scope = EmptyVariableScope()
     compiled_query_fct_args = inspect.getfullargspec(module.query.fct).args
     fct_signature = inspect.Signature(parameters=[inspect.Parameter(name, inspect.Parameter.POSITIONAL_OR_KEYWORD) for name in input_variables])
 
     module.query.function_context = FunctionContext(fct_signature, compiled_query_fct_args, scope)
     module.query.is_async = is_async
+    module.query.output_writer = output_writer
+    module.query.extra_args = extra_args
     
     return module.query
 
-def query(fct, input_variables=None, is_async=True):
+def F(s: str, constraints: Optional[str] = None, **kwargs):
+    """
+    Constructs a LMQL query function from the given string.
+
+    Example:
+
+    ```python
+    lmql.F("Say 'this is a test': [RESPONSE]", "len(TOKENS(RESPONSE)) < 10")
+    ```
+
+    The second argument contains an optional `where` clause expression and can be omitted.
+
+    The resulting callable acts like a `lmql.query` function and can be called with the same arguments.
+    """
+    # escape all double quotes
+    s = s.replace('"', '\\"')
+    is_async = kwargs.pop("is_async", False)
+    return query(f'"{s}"' + (f' where {constraints}' if constraints is not None else ''), is_async=is_async, is_f_function=True, **kwargs)
+
+def query(__fct__=None, input_variables=None, is_async=True, calling_frame=None, **extra_args):
     """
     Constructs a new LMQL query function from the given function and or string of code.
 
     You can use `lmql.query` as a function decorator or to compile a string of LMQL code.
 
     * As a decorator, it can be used as follows:
 
@@ -141,25 +147,36 @@
         my_query_function = lmql.query('''
             <LMQL code>
         ''')
 
         By default the returned query function is asynchronous (has to be called as `await my_query_function(...)`).
         To construct a synchronous query function, use lmql.query(<query string>, is_async=False).
     """
+    fct = __fct__
+
+    # check for @lmql.query(<args>) def f(): ... use with additional arguments
+    if fct is None:
+        def wrapper(fct):
+            import inspect
+            calling_frame = inspect.stack()[1]
+            return query(fct, input_variables=input_variables, is_async=is_async, calling_frame=calling_frame, **extra_args)
+        return wrapper
+
+    # otherwise assume @lmql.query def f(): ...
     import inspect
 
     if type(fct) is LMQLQueryFunction: return fct
 
     # support for lmql.query(<query string>)
     if type(fct) is str: 
-        return _query_from_string(fct, input_variables)
+        return _query_from_string(fct, input_variables, is_async=is_async, **extra_args)
     else:
         assert input_variables is None, "input_variables must be None when using @lmql.query as a decorator."
     
-    calling_frame = inspect.stack()[1]
+    calling_frame = calling_frame or inspect.stack()[1]
     scope = LMQLInputVariableScope(fct, calling_frame)
     code = get_decorated_function_code(fct)
 
     temp_lmql_file = tempfile.mktemp(suffix=".lmql")
     with open(temp_lmql_file, "w") as f:
         f.write(code)
     module = load(temp_lmql_file, autoconnect=True, output_writer=silent)
@@ -168,20 +185,21 @@
     
     decorate_fct_signature = inspect.signature(fct)
     compiled_query_fct_args = inspect.getfullargspec(module.query.fct).args
     
     # set the function context of the query based on the function context of the decorated function
     module.query.function_context = FunctionContext(decorate_fct_signature, compiled_query_fct_args, scope)
     module.query.is_async = is_async
+    module.query.extra_args = extra_args
 
     def lmql_query_wrapper(*args, **kwargs):
         return module.query(*args, **kwargs)
 
-    # copy all attributes of model.query to the wrapper function
-    for attr in ["aschain"]:
+    # copy some attributes of model.query to the wrapper function
+    for attr in ["aschain", "lmql_code", "is_async", "output_variables"]:
         setattr(lmql_query_wrapper, attr, getattr(module.query, attr))
 
     return lmql_query_wrapper
 
 async def static_prompt(query_fct, *args, **kwargs):
     """
     Returns the static prompt prefix that is generated by the given query function up until the first variable.
```

### Comparing `lmql-0.0.6.4/src/lmql/algorithms/cache.py` & `lmql-0.0.6.5/src/lmql/algorithms/cache.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/algorithms/functools.py` & `lmql-0.0.6.5/src/lmql/algorithms/functools.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/cli.py` & `lmql-0.0.6.5/src/lmql/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,16 +89,17 @@
     parser.add_argument("--ui-port", type=int, default=3000, help="port to use to host the LMQL debugger UI")
     
     args = parser.parse_args(sys.argv[2:])
 
     project_root = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
     print(f"[lmql playground {project_root}, liveserver=localhost:{args.live_port}, ui=localhost:{args.ui_port}]")
 
-    # make sure yarn is installed
-    os.system("npm install -g yarn")
+    # # make sure yarn is installed
+    if os.system("yarn --version") != 0:
+        os.system("npm install -g yarn")
 
     # repo commit
     if os.path.exists(os.path.join(project_root, "../.git")):
         commit = subprocess.check_output("git rev-parse HEAD", shell=True, cwd=project_root).decode("utf-8").strip()
         commit = commit[:7]
         has_uncomitted_files = len(subprocess.check_output("git status --porcelain", shell=True, cwd=project_root).decode("utf-8").strip()) > 0
         if has_uncomitted_files:
@@ -168,27 +169,25 @@
         backend = sys.argv[2]
         if backend not in ["hf", "openai"]:
             print("Invalid backend, please specify one of {}".format(", ".join(["hf", "openai"])))
             sys.exit(1)
     
     if backend is None or backend == "hf":
         code_local = """
-    argmax "Hello[WHO]" from "local:gpt2-medium" where len(WHO) < 10    
+    argmax "Hello[WHO]" from "local:gpt2-medium" where len(TOKENS(WHO)) < 10
     """
         print("[Greeting 🤗 Transformers]")
         asyncio.run(lmql.run(code_local, output_writer=lmql.printing))
     
     if backend is None or backend == "openai":
         import lmql.runtime.dclib as dc
         dc.clear_tokenizer()
         print("[Greeting OpenAI]")
-        code_openai = """
-    argmax "Hello[WHO]" from "openai/text-ada-001" where len(WHO) < 10    
-    """
-        asyncio.run(lmql.run(code_openai, output_writer=lmql.printing))
+        code_openai = 'argmax "Hello[WHO]" from "openai/text-ada-001" where len(TOKENS(WHO)) < 10 and not "\\n" in WHO'
+        asyncio.run(lmql.run(code_openai, output_writer=lmql.printing, model="openai/text-ada-001"))
 
 def basic_samples():
     from lmql.tests.test_sample_queries import main
     import asyncio
     asyncio.run(main())
 
 hidden_commands = {
```

### Comparing `lmql-0.0.6.4/src/lmql/demo.py` & `lmql-0.0.6.5/src/lmql/demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-def gsm8k_samples(): return """Q: Every hour Joanne has to collect the coins out of the fountain inside the mall. During the first hour, she collected 15 coins. For the next two hours, she collected 35 coins from the fountain. In the fourth hour, she collected 50 coins from the fountain but she gave 15 of them to her coworker so she could buy a soda. How many coins did she have after the fourth hour?
+def gsm8k_samples(): return """
+Q: Every hour Joanne has to collect the coins out of the fountain inside the mall. During the first hour, she collected 15 coins. For the next two hours, she collected 35 coins from the fountain. In the fourth hour, she collected 50 coins from the fountain but she gave 15 of them to her coworker so she could buy a soda. How many coins did she have after the fourth hour?
 A: Let's think step by step.
 15 coins collected in hour one
 35 coins collected in hour two
 35 coins collected in hour three
 50 coins collected in hour four
 Before giving her coworker some coins there were 15+35+35+50=<< 15+35+35+50 = 135 >>135 coins
 The number of coins after given 15 to her coworker is 135-15=<< 135-15 = 120 >>120
```

### Comparing `lmql-0.0.6.4/src/lmql/http.py` & `lmql-0.0.6.5/src/lmql/http.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/language/compiler.py` & `lmql-0.0.6.5/src/lmql/language/compiler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from _ast import AsyncFunctionDef, ClassDef, FunctionDef, Import, ImportFrom
+from _ast import And, AsyncFunctionDef, BinOp, ClassDef, Compare, FunctionDef, Import, ImportFrom, Return
 import ast
 import sys
 from typing import Any
 import astunparse
 import os
 import importlib
 import re
 
 from io import StringIO
 from lmql.ops.ops import lmql_operation_registry
 
-from lmql.language.qstrings import qstring_to_stmts, TemplateVariable
+from lmql.language.qstrings import qstring_to_stmts, TemplateVariable, FExpression, DistributionVariable, TagExpression, stmts_to_qstring
 from lmql.language.validator import LMQLValidator, LMQLValidationError
 from lmql.language.fragment_parser import LMQLDecoderConfiguration, LMQLQuery, LanguageFragmentParser, FragmentParserError
 from lmql.runtime.model_registry import model_name_aliases
 import lmql.runtime.lmql_runtime as lmql_runtime
 from lmql.runtime.dclib import get_all_decoders
 
 OPS_NAMESPACE = "lmql.ops"
@@ -47,15 +47,15 @@
 
     def visit_Name(self, node):
         if type(node.ctx) is ast.Store:
             self.defined_vars.add(node.id)
 
     def visit_FunctionDef(self, node: FunctionDef) -> Any:
         self.defined_vars.add(node.name)
-    
+
     def visit_ClassDef(self, node: ClassDef) -> Any:
         self.defined_vars.add(node.name)
 
     def visit_Import(self, node: Import) -> Any:
         for alias in node.names:
             self.defined_vars.add(alias.asname or alias.name)
 
@@ -105,63 +105,66 @@
             FreeVarCollector(self.free_vars, exclude_criteria=[self.exclude_identifier]).visit(query.distribution.values)
 
         # remove all defined and prologue vars from free vars
         self.free_vars = self.free_vars - self.defined_vars - self.prologue_vars
 
         query.scope = self
 
-    def visit_Constant(self, node):
+    def visit_Expr(self, expr):
+        if type(expr.value) is ast.Constant:
+            self.scope_Constant(expr.value)
+        else:
+            super().generic_visit(expr)
+
+    def visit_BoolOp(self, node: ast.BoolOp) -> Any:
+        if is_query_string_with_constraints(node):
+            self.scope_Constant(node.values[0])
+
+    def scope_Constant(self, node):
         if type(node.value) is not str: return super().visit_Constant(node)
         qstring = node.value
 
+        stmts = qstring_to_stmts(qstring, mode="all")
+
         # capture set of defined vars
-        declared_template_vars = [v.name for v in qstring_to_stmts(qstring) if type(v) is TemplateVariable]
+        declared_template_vars = [v.name for v in stmts if type(v) is TemplateVariable]
         for v in declared_template_vars: 
             self.defined_vars.add(v)
             self.written_vars.add(v)
             if v in self.free_vars: self.free_vars.remove(v)
 
-        # capture set of format vars (exclude {{ and }})
-        # replace {{ and }} with escape sequence \u007b and \u007d 
-        qstring = qstring.replace("{{", "__curly_open__").replace("}}", "__curly_close__")
-        # same for [[ and ]]
-        qstring = qstring.replace("[[", "__square_open__").replace("]]", "__square_close__")
-
-        used_fstring_expr = [v[1:-1] for v in re.findall("\{[^\}\{]+\}", qstring)]
+        used_fstring_expr = [s.expr for s in stmts if type(s) is FExpression]
         for v in used_fstring_expr:
-            if v.startswith(":"):
-                continue
             try:
-                parsed = ast.parse(v).body[0].value
+                parsed = ast.parse(v, mode="eval")
                 self.visit(parsed)
-            except:
-                print("info: failed to parse fstring expression: ", v)
+            except Exception as e:
+                print("info: failed to parse fstring expression: ", [v])
+                raise e
                 # raise RuntimeError("Failed to parse fstring expression: ", v)
                 return super().visit_Constant(node)
 
-        # put double curly braces back in
-        qstring = qstring.replace("__curly_open__", "{{").replace("__curly_close__", "}}")
-        qstring = qstring.replace("__square_open__", "[[").replace("__square_close__", "]]")
-        
-        template_tags = [v[1:-1] for v in re.findall("\{:[A-z0-9]+\}", qstring)]
-        for tt in template_tags:
-            qstring = qstring.replace(f"{{{tt}}}", f"{{lmql.tag('{tt[1:]}')}}")
-        
-        # replace other {} with lmql.escape
-        qstring = re.sub("\{[^\}]+\}", lambda m: f"{{lmql.lmql_runtime.f_escape({m.group(0)[1:-1]})}}", qstring)
+        def transform_qexpr(qexpr):
+            if type(qexpr) is TemplateVariable and qexpr.name in self.distribution_vars:
+                return DistributionVariable(qexpr.name)
+            if type(qexpr) is FExpression:
+                return FExpression(f"lmql.lmql_runtime.f_escape({qexpr.expr})")
+            elif type(qexpr) is TagExpression:
+                return TagExpression(f"lmql.lmql_runtime.tag(\"{qexpr.tag[1:]}\")")
+            return str(qexpr)
 
-        node.value = qstring
+        node.value = stmts_to_qstring([transform_qexpr(s) for s in stmts])
 
         return super().visit_Constant(node)
 
     def exclude_identifier(self, name):
         # make sure "input" can be intercepted
         if name in ["input"]:
             return False
-        if name in ["lmql"]:
+        if name in ["lmql", "context", "__dynamic__"]:
             return True
         if name in self.free_vars:
             return True
         if name in self.written_vars:
             return True
         # exclude LMQL built-ins
         if get_builtin_name(name) is not None:
@@ -183,14 +186,33 @@
             
         if type(node.ctx) is ast.Load:
             if self.exclude_identifier(name):
                 return
             self.free_vars.add(name)
         
         return True
+    
+    def visit_FunctionDef(self, node: FunctionDef) -> Any:
+        self.defined_vars.add(node.name)
+    
+    def visit_AsyncFunctionDef(self, node: AsyncFunctionDef) -> Any:
+        self.defined_vars.add(node.name)
+
+    def visit_ClassDef(self, node: ClassDef) -> Any:
+        self.defined_vars.add(node.name)
+
+    def visit_ImportFrom(self, node: ImportFrom) -> Any:
+        for alias in node.names:
+            self.defined_vars.add(alias.asname or alias.name)
+
+def is_query_string_with_constraints(node: ast.BoolOp):
+    if len(node.values) < 1:
+        return False
+    left_most_operand = node.values[0]
+    return type(left_most_operand) is ast.Constant and type(left_most_operand.value) is str and isinstance(node.op, ast.And)
 
 class QueryStringTransformation(ast.NodeTransformer):
     """
     Transformes string expressions on statement level to model queries.
     """
     
     def __init__(self, query):
@@ -211,43 +233,65 @@
         name = str(node.id)
         
         if type(node.ctx) is ast.Load:
             if name == "context":
                 return ast.parse("(" + yield_call("get_context", ()) + ")").body[0].value
         return node
 
+    def visit_BoolOp(self, node: ast.BoolOp) -> Any:
+        if is_query_string_with_constraints(node):
+            left_most_operand = node.values[0]
+            if len(node.values[1:]) > 1:
+                constraints_expression = ast.BoolOp(op=node.op, values=node.values[1:])
+            if len(node.values[1:]) == 1:
+                constraints_expression = node.values[1]
+            elif len(node.values[1:]) == 0:
+                constraints_expression = None
+            return self.transform_Constant(left_most_operand, constraints = constraints_expression)
+        return node
 
-    def transform_Constant(self, constant):
+    def transform_Constant(self, constant, constraints=None):
         if type(constant.value) is not str: return constant
+        
         qstring = constant.value
-        # TODO: handle escaping more completely and gracefully
-        qstring = qstring.replace("\n", "\\\\n")
+        qstring = qstring.encode("unicode_escape").decode("utf-8").encode('unicode_escape').decode('utf-8')
+        
         compiled_qstring = ""
 
         declared_template_vars = set()
 
-        for i, stmt in enumerate(qstring_to_stmts(qstring)):
+        for stmt in qstring_to_stmts(qstring, mode="square-only"):
             if type(stmt) is str:
                 compiled_qstring += stmt
+            elif type(stmt) is DistributionVariable:
+                compiled_qstring += str(stmt)
             elif type(stmt) is TemplateVariable:
-                if stmt.name in self.query.scope.distribution_vars:
-                    compiled_qstring += f"[distribution:{stmt.name}]"
-                else:
-                    declared_template_vars.add(stmt.name)
-                    compiled_qstring += "[" + stmt.name + "]"
+                declared_template_vars.add(stmt.name)
+                compiled_qstring += str(stmt)
+
+        # keep track of last stmt in this qstring
+        last_stmt = stmt
 
         if len(compiled_qstring) == 0:
             return constant
 
-        # result_code = f'yield context.query(f"""{compiled_qstring}""")'
-        result_code = interrupt_call('query', f'f"""{compiled_qstring}"""')
+        if constraints is not None:
+            constraint_transformation = InlineConstraintsTransformation(constraints, scope=self.query.scope)
+            code_str, result_reference = constraint_transformation.transform()
+            result_code = code_str + "\n"
+
+            # result_code = f'yield context.query(f"""{compiled_qstring}""")'
+            result_code += interrupt_call('query', f'f"""{compiled_qstring}"""', "{**globals(), **locals()}", "constraints=" + result_reference)
+        else:
+            result_code = interrupt_call('query', f'f"""{compiled_qstring}"""', "{**globals(), **locals()}")
 
         for v in declared_template_vars:
             get_var_call = yield_call('get_var', f'"{v}"')
             result_code += f"\n{v} = " + get_var_call
+
         return ast.parse(result_code)
 
     # def transform_prompt_stmt(self, stmt):
     #     if type(stmt) is ast.Expr:
     #         if type(stmt.value) is ast.Constant and type(stmt.value.value) is str:
     #             # print(stmt.value.value)
     #             stmt.value = self.transform_query_string(stmt.value.value)
@@ -295,47 +339,42 @@
 class ReturnStatementTransformer(ast.NodeTransformer):
     def __init__(self, query):
         self.query = query
     
     def transform(self):
         self.query.prompt = [self.visit(p) for p in self.query.prompt]
 
-    def visit_Return(self, node):
-        return ast.parse("yield ('result', " + astunparse.unparse(node.value).strip() + ")")
-
-class WhereClauseTransformation():
-    def __init__(self, query: LMQLQuery):
-        self.query = query
-        self.scope: PromptScope = query.scope
-
-        assert self.scope is not None, "WhereClauseTransformation requires a scoped query for transformation"
+    def visit_FunctionDef(self, node: FunctionDef) -> Any:
+        # do not recurse into nested functions
+        return node
     
-    def transform(self):
-        snf = SNFList()
-        
-        if self.query.where is None:  return None
-        if type(self.query.where) is ast.Expr: 
-            self.query.where = self.query.where.value
+    def visit_AsyncFunctionDef(self, node: AsyncFunctionDef) -> Any:
+        # do not recurse into nested functions
+        return node
 
-        result = self.transform_node(self.query.where, snf=snf)
+    def visit_Return(self, node):
+        return ast.parse("yield ('result', " + astunparse.unparse(node.value).strip() + ")")
 
-        self.query.where = snf.str()
-        self.query.where_expr = result
+class LMQLConstraintTransformation:
+    def __init__(self, scope) -> None:
+        self.scope = scope
 
     def transform_name(self, node, keep_variables=False, plain_python=False):
         # check for built-ins
         bn = get_builtin_name(node, plain_python)
         if bn is not None: return bn
         # check if variable is distribution variable
         if node.id in self.scope.distribution_vars:
             raise LMQLValidationError("Distribution variable {} cannot be used in where clause.".format(node.id))
 
         # check for template variables
         if node.id in self.scope.defined_vars and not keep_variables:
             return f"lmql.runtime_support.Var('{node.id}')"
+        else:
+            return f"lmql.runtime_support.Var('{node.id}', python_variable=True)"
 
         return bn or node.id
 
     def transform_node(self, expr, snf):
         if type(expr) is ast.BoolOp:
             if type(expr.op) is ast.And or type(expr.op) is ast.Or:
                 ops = expr.values
@@ -425,14 +464,50 @@
 
         args = (" " + ", ".join(names)) if len(names) > 0 else ""
         var_ops = (", ".join([f"{OPS_NAMESPACE}.Var('{n}')" for n in names])).strip() if len(names) > 0 else ""
         fct_code = astunparse.unparse(node).strip()
         
         return f"{OPS_NAMESPACE}.OpaqueLambdaOp([lambda{args}: {fct_code}, {var_ops}])"
 
+class WhereClauseTransformation(LMQLConstraintTransformation):
+    def __init__(self, query: LMQLQuery):
+        super().__init__(scope=query.scope)
+        self.query = query
+        
+        assert self.scope is not None, "WhereClauseTransformation requires a scoped query for transformation"
+    
+    def transform(self):
+        snf = SNFList()
+        
+        if self.query.where is None:  return None
+        if type(self.query.where) is ast.Expr: 
+            self.query.where = self.query.where.value
+
+        result = self.transform_node(self.query.where, snf=snf)
+
+        self.query.where = snf.str()
+        self.query.where_expr = result
+
+class InlineConstraintsTransformation(LMQLConstraintTransformation):
+    def __init__(self, expression: ast.BoolOp, scope):
+        super().__init__(scope=scope)
+        self.expression = expression
+    
+    def transform(self):
+        snf = SNFList()
+        
+        if self.expression is None:  return None
+        if type(self.expression) is ast.Expr: 
+            self.expression = self.expression.value
+
+        result = self.transform_node(self.expression, snf=snf)
+
+        return snf.str(), result
+
+
 def is_allowed_builtin_python_call(node):
     if type(node) is not ast.Name:
         return False
     allowed_builtin_functions = set(["set", "all"])
     return node.id in allowed_builtin_functions
 
 def get_builtin_name(node, plain_python=False):
@@ -654,8 +729,9 @@
                     writer.add(yield_call("set_distribution", "\"" + q.distribution.variable_name + "\"", astunparse.unparse(q.distribution.values).strip()))
                 
                 writer.add(f"yield ('result', (" + yield_call("get_return_value", ()) + "))")
 
             return LMQLModule(output_file, lmql_code=lmql_code, output_variables=[v for v in scope.defined_vars])
         except FragmentParserError as e:
             sys.stderr.write("error: " + str(e) + "\n")
+            sys.exit(1)
```

### Comparing `lmql-0.0.6.4/src/lmql/language/fragment_parser.py` & `lmql-0.0.6.5/src/lmql/language/fragment_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,19 +86,14 @@
 
 def remove_comments(s):
     if type(s) is str: return s
     assert type(s) is list
     return tokenize.untokenize([transform_token(t) for t in s if t.type != tokenize.COMMENT])
 
 def transform_token(t):
-    if is_keyword(t, "as"):
-        # return tokenize.Token
-        # print(t)
-        return tokenize.TokenInfo(tokenize.OP, "=", start = t.start, end = t.end, line = t.line)
-
     return t
 
 def ast_parse(s, unindent=False, oneline=False, loc=None):
     try:
         s = remove_comments(s)
         if unindent: s = remove_indentation(s, oneline=oneline)
         return ast.parse(s)
@@ -136,62 +131,81 @@
         self.state = "start" # "decode" | "prompt" | "where" | "scoring" | "import"
         self.query = LMQLQuery()
         self.paren_count = 0
 
     def parse(self, readline):
         for i, tok in enumerate(tokenize.generate_tokens(readline)):
             self.digest(tok)
+        
+        if self.state == "start":
+            self.query.prompt_str = self.query.prologue
+            self.query.prologue = []
+            self.state = "prompt"
 
         # print("decode_str", remove_comments(self.query.decode_str))
         # print("prompt_str", remove_comments(self.query.prompt_str))
         # print("from_str", remove_comments(self.query.from_str))
 
         self.prologue_transform()
+        self.inline_where_transform()
         self.ast_parse()
         self.syntax_validation()
         self.ast_transform()
 
         return self.query
 
+    def inline_where_transform(self):
+        prompt_tokens = self.query.prompt_str
+        for i in range(len(prompt_tokens) - 1):
+            tok = prompt_tokens[i]
+            lookahead = prompt_tokens[i+1]
+            if tok.type == tokenize.STRING and lookahead.type == tokenize.NAME and lookahead.string == "where":
+                # print(prompt_tokens[i+1])
+                prompt_tokens[i+1] = tokenize.TokenInfo(type=tokenize.OP, string="and", start=lookahead.start, end=lookahead.end, line=lookahead.line)
+        
+
     def prologue_transform(self):
         # translate prologue tokens into str
         self.query.prologue = tokenize.untokenize(self.query.prologue)
 
     def ast_transform(self):
         if self.query.distribution is not None:
             # this structure is already validated (see self.syntax_validation)
             variable_name = self.query.distribution.left.id
             self.query.distribution = LMQLDistributionClause(variable_name, self.query.distribution.comparators[0])
 
     def syntax_validation(self):
-        # validate decode clause
-        if len(self.query.decode_str) == 0:
-            raise FragmentParserError("A query must start with a decode clause (e.g. ARGMAX).")
-        
-        # validate from clause
-        if len(self.query.from_str) == 0:
-            raise FragmentParserError("The query is missing a FROM clause (e.g. FROM 'gpt-2').")
-
         # validation distribution clause
         if self.query.distribution is not None:
             error_msg = "The distribution clause must be formed like 'VAR in [list of values]'."
             if type(self.query.distribution) is not ast.Compare:
                 raise FragmentParserError(error_msg)
             if type(self.query.distribution.ops[0]) is not ast.In:
                 raise FragmentParserError(error_msg)
             variable_node = self.query.distribution.left
             if type(variable_node) is not ast.Name:
                 raise FragmentParserError(error_msg)
             values_list = self.query.distribution.comparators[0]
 
     def ast_parse(self):
         # parse decode, prompt and from
-        self.query.decode = ast_parse(self.query.decode_str, loc="decode").body[0].value
+        decode_body = ast_parse(self.query.decode_str, loc="decode").body
+        if len(decode_body) > 0:
+            self.query.decode = decode_body[0].value
+        else:
+            # default decoder
+            self.query.decode = ast.parse("__dynamic__").body[0].value
+        
         self.query.prompt = ast_parse(self.query.prompt_str, unindent=True, loc="prompt").body
-        self.query.from_ast = ast_parse(self.query.from_str, unindent=True, loc="from").body[0]
+        
+        from_body = ast_parse(self.query.from_str, unindent=True, loc="from").body
+        if len(from_body) > 0:
+            self.query.from_ast = from_body[0]
+        else:
+            self.query.from_ast = ast.Str(s="<dynamic>")
 
         where_body = ast_parse(self.query.where_str, unindent=True, oneline=True, loc="where").body
         if len(where_body) > 0:
             self.query.where = where_body[0]
         else:
             self.query.where = None
         
@@ -213,14 +227,20 @@
             if tok.type == tokenize.NAME:
                 # when we encounter the first decoder keyword, we switch to the query parsing state
                 if tok.string.lower() in get_all_decoders():
                     self.query.decode_str += [tok]
                     self.state = "decode"
                     return
             
+            if is_keyword(tok, "where"):
+                self.query.prompt_str = self.query.prologue + [tok]
+                self.query.prologue = []
+                self.state = "prompt"
+                return
+
             # otherwise add token to prologue tokens (e.g. imports, comments, function definitions)
             self.query.prologue.append(tok)
             return
         elif self.state == "decode":
             if tok.type == tokenize.STRING and self.paren_count == 0:
                 self.state = "prompt"
                 self.query.prompt_str += [tok]
@@ -231,20 +251,22 @@
             if tok.type == tokenize.OP and tok_str(tok) == "(":
                 self.paren_count += 1
             elif tok.type == tokenize.OP and tok_str(tok) == ")":
                 self.paren_count -= 1
             if self.paren_count == 0:
                 self.state = "prompt"
         elif self.state == "prompt":
+            if is_keyword(tok, "where"):
+                if self.query.prompt_str[-1].type != tokenize.STRING:
+                    self.state = "where"
+                    return
+            
             if is_keyword(tok, "FROM"):
                 self.state = "from"
                 return
-            if is_keyword(tok, "WHERE"):
-                self.state = "where"
-                return
             if is_keyword(tok, "SCORING"):
                 self.state = "scoring"
                 return
             if is_keyword(tok, "DISTRIBUTION"):
                 self.state = "distribution"
                 return
```

### Comparing `lmql-0.0.6.4/src/lmql/language/validator.py` & `lmql-0.0.6.5/src/lmql/language/validator.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/models/lmtp/README.md` & `lmql-0.0.6.5/src/lmql/models/lmtp/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_client.py` & `lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,15 @@
 For debugging purposes, run this file directly for an interactive client CLI.
 """
 
 import aiohttp
 import asyncio
 import json
 import sys
-import multiprocessing
-from multiprocessing.connection import Connection
-
-class LMTPStreamError(Exception):
-    pass
+from .errors import LMTPStreamError
 
 class LMTPWebSocketClient:
     """
     Simple 'websockets' based client for LMTP.
     """
     def __init__(self, model_identifier, ws: aiohttp.ClientWebSocketResponse):
         self.ws = ws
```

### Comparing `lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_dcmodel.py` & `lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_dcmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 """
 LMQL model implementation that uses the LMTP protocol to communicate with a
 hosted model server, or a model running in a separate process.
 """
 
 from lmql.runtime.dclib.dclib_model import DcModel
 from lmql.runtime.tokenizer import load_tokenizer
-from .lmtp_client import LMTPWebSocketClient
-from .lmtp_multiprocessing import LMTPMultiProcessingClient
-from .lmtp_threading import LMTPThreadedClient
-from .lmtp_inference_server import Scheduler
+from .lmtp_async import LMTPAsyncClient
 import lmql.runtime.dclib as dc
 import asyncio
 import numpy as np
-import aiohttp
 import lmql.utils.nputil as nputil
 import lmql.runtime.masks as masks
 from lmql.runtime.token_distribution import TokenDistribution
 
 from typing import Any, List, Union
 
 class LMTPModel(DcModel):
@@ -31,73 +27,82 @@
         self._client_loop = None
         # set once self.client is set up
         self.connected_signal = asyncio.Event()
         # set to termiante self._client_loop
         self.close_signal = asyncio.Event()
         # error signal
         self.error_signal = asyncio.Event()
+        self.error = None
         
         # endpoint in case of remote model
         self.endpoint = endpoint
         if endpoint is not None and not self.endpoint.startswith("http"):
             self.endpoint = "http://" + self.endpoint
 
         self.inprocess = inprocess
         self.lmtp_server_kwargs = lmtp_server_kwargs
         assert self.inprocess or  lmtp_server_kwargs is None, "LMTP server kwargs can only be set when using lmql.inprocess mode"
         if inprocess:
-            self.inprocess_client_constructor = inprocess_client_constructor or LMTPMultiProcessingClient
+            self.inprocess_client_constructor = inprocess_client_constructor
 
         # model statistics
         self.requests = 0
         self.tokens = 0
 
     async def inprocess_client_loop(self):
         self.client = self.inprocess_client_constructor(self.model.model_identifier, **self.lmtp_server_kwargs)
 
         self.connected_signal.set()
         await self.close_signal.wait()
         await self.client.close()
         self.client = None
 
     async def ws_client_loop(self):
+        import aiohttp
+        from .lmtp_client import LMTPWebSocketClient
+        
         try:
             async with aiohttp.ClientSession() as session:
                 async with session.ws_connect(self.endpoint) as ws:
                     self.client = LMTPWebSocketClient(self.model.model_identifier, ws)
                     self.client.connect()
                     
                     self.connected_signal.set()
                     await self.close_signal.wait()
         except Exception as e:
-            print("Failed to communicate with lmtp endpoint: {}".format(self.endpoint), flush=True)
             self.error_signal.set()
+            self.error = "Failed to communicate with lmtp endpoint: {}. Please check that the endpoint is correct and the server is running.".format(self.endpoint)
             self.connected_signal.set()
 
     def make_cache_entry(self, s, payload, sampling_mode):
         scores = {}
         for t, score in payload["top_logprobs"].items():
             scores[int(t)] = score
         
         if sampling_mode == "top-1":
             scores[int(payload["token"])] = payload["logprob"]
 
         top_entries = list(sorted(scores.items(), key=lambda x: x[1], reverse=True))
         tokens = [t for t, _ in top_entries]
         scores = [s for _, s in top_entries]
         edge_type = ["top-{}".format(i+1) for i in range(len(top_entries))]
-        
+
         # for non argmax sampling modes, add the sampled token
         if sampling_mode != "top-1":
             tokens = [payload["token"]] + tokens
             scores = [payload["logprob"]] + scores
             edge_type = [sampling_mode] + edge_type
 
         tokens = self.tokenizer.decode_bytes(tokens)
 
+        # replace top-1 with payload["token"] if sampling mode is top-1
+        if sampling_mode == "top-1":
+            edge_type[0] = "top-1"
+            tokens[0] = self.tokenizer.decode_bytes([payload["token"]])
+
         return (s, tokens, scores, edge_type, {})
 
     async def stream_and_return_first(self, s, iterator, sampling_mode):
         buffer = []
         for i in range(4):
             try:
                 buffer += [await anext(iterator)]
@@ -126,27 +131,27 @@
             self.register_token_stream(token_stream)
         asyncio.ensure_future(do_register())
         
         return buffer[0]
 
     async def ensure_connected(self):
         if self.error_signal.is_set():
-            raise RuntimeError("LMTP client encountered an error")
+            raise RuntimeError("LMTP client encountered an error: {}".format(self.error))
 
         if self.client is None:
             if not self.inprocess:
                 self._client_loop = asyncio.create_task(self.ws_client_loop())
             else:
                 self._client_loop = asyncio.create_task(self.inprocess_client_loop())
         
         await self.connected_signal.wait()
         
         # double check for errors
         if self.error_signal.is_set():
-            raise RuntimeError("LMTP client encountered an error")
+            raise RuntimeError("LMTP client encountered an error: {}".format(self.error))
 
     # on deinit
     def close(self):
         self.close_signal.set()
 
     def __del__(self):
         self.close_signal.set()
@@ -154,15 +159,15 @@
     def make_logits(self, payload):
         scores = {}
         for t, score in payload["top_logprobs"].items():
             scores[int(t)] = score
         scores[int(payload["token"])] = payload["logprob"]
         scores = scores.items()
 
-        logits = np.ones(self.tokenizer.vocab_size) * self.truncation_threshold
+        logits = np.ones(self.tokenizer.vocab_range) * self.truncation_threshold
         logits[[t for t, _ in scores]] = [s for _, s in scores]
 
         return logits
 
     async def singleton_result(self, token, score):
         yield {"token": token, "logprob": score, "top_logprobs": {token: score}}
 
@@ -187,14 +192,17 @@
 
             if invert: masked = (mask >= 0)
             else: masked = (mask < 0)
             mask_value = 100 if invert else -100
             mask = {int(idx): mask_value for idx in np.nonzero(masked)[0]}
 
         ids = self.tokenizer.convert_bytes_to_ids(s.input_ids)
+        
+        if self.tokenizer.bos_token_id is not None and ids[0] != self.tokenizer.bos_token_id:
+            ids = [self.tokenizer.bos_token_id] + ids
 
         return self.client.generate(ids, max_tokens=chunk_size, temperature=temperature, logit_bias=mask, top_logprobs=top_logprobs)
 
     async def argmax(self, sequences: dc.DataArray, **kwargs):
         return await self.sample(sequences, temperature=0.0, **kwargs)
 
     async def sample(self, sequences: dc.DataArray, temperature, **kwargs):
@@ -298,14 +306,17 @@
         
         scores = []
         i = 0
         
         ids = self.tokenizer.convert_bytes_to_ids(s.input_ids)
         next_tokens = self.tokenizer.convert_bytes_to_ids(next_tokens)
 
+        if self.tokenizer.bos_token_id is not None and ids[0] != self.tokenizer.bos_token_id:
+            ids = [self.tokenizer.bos_token_id] + ids
+
         async for token in self.client.score(ids, next_tokens):
             t = next_tokens[i]
             assert token["token"] == t, "Expected token {}, got {}".format(t, token["token"])
             scores.append(token["logprob"])
             i += 1
         assert len(scores) == len(next_tokens), "Expected {} scores, got {}".format(len(next_tokens), len(scores))
         
@@ -356,43 +367,54 @@
     """
     Factory class for LMTPModelCls client instances.
 
     In case of inprocess=True, lmtp_model keeps a reference to the internally instantiated 
     LMTPMultiProcessingClient to share it between all uses of the resulting LMTPModelCls 
     across several queries.
     """
-    def __init__(self, model_identifier, inprocess=False, endpoint=None, **kwargs):
+    def __init__(self, model_identifier, inprocess=False, endpoint=None, async_transport=False, **kwargs):
         self.model_identifier = model_identifier
         self.tokenizer_identifier = kwargs.pop("tokenizer", self.model_identifier)
 
         self.inprocess = inprocess
+        self.async_transport = async_transport
         self.endpoint = endpoint
         self.kwargs = kwargs
 
         self.lmtp_inprocess_client = None
     
     # ensures that all inprocess lmtp models instantiated via this class 
     # share the same underlying LMTPMultiProcessingClient instance
     # (uses reference counting to ensure that the client is only shut down 
     # once all LMTPModel instances have closed)
     def inprocess_client_constructor_factory(self, identifier, **kwargs):
         assert identifier == self.model_identifier, "Model identifier mismatch: {} vs {}".format(self.model_identifier, identifier)
         
+        # use in-process, async client
+        if self.async_transport:
+            return LMTPAsyncClient(identifier, **kwargs)
+
+        # otherwise, use multiprocessing
+        from .lmtp_multiprocessing import LMTPMultiProcessingClient
+
         if self.lmtp_inprocess_client is None:
             # ref owned by self
             self.lmtp_inprocess_client = LMTPMultiProcessingClient(identifier, **kwargs).ref()
             # ref owned by caller
             return self.lmtp_inprocess_client.ref()
         
         # ref owned by caller
         return self.lmtp_inprocess_client.ref()
 
     def __del__(self):
         if self.lmtp_inprocess_client is not None:
-            asyncio.ensure_future(self.lmtp_inprocess_client.close())
+            if asyncio.get_event_loop() == asyncio.get_event_loop_policy().get_event_loop():
+                pass
+            else:
+                asyncio.ensure_future(self.lmtp_inprocess_client.close())
             # print("closing shared LMTPMultiProcessingClient instance for model {}".format(self.model_identifier), self.lmtp_inprocess_client.refs, flush=True)
 
     def __call__(self):
         # reference to factory instance
         this = self
 
         class LMTPModelCls:
@@ -403,15 +425,15 @@
 
                 self.decoder_args = {}
 
                 self.num_queries = 0
 
             def get_tokenizer(self):
                 if self._tokenizer is None:
-                    self._tokenizer = load_tokenizer(this.tokenizer_identifier)
+                    self._tokenizer = load_tokenizer(this.tokenizer_identifier, **this.kwargs)
                 self.served_model = self
                 return self._tokenizer
 
             def get_dclib_model(self):
                 bos_token_id = self.get_tokenizer().bos_token_id
                 eos_token_id = self.get_tokenizer().eos_token_id
```

### Comparing `lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_inference_server.py` & `lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_scheduler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,22 @@
-"""
-HuggingFace Transformers LMTP inference server implementation.
-
-To run an instance of this LMTP server, run e.g. the following command:
-
-lmql serve-model --cuda gpt2-medium
-
-See lmtp_client for an example how to connect to this server via 'websocket'.
-"""
-
-import sys
-import aiohttp
-from aiohttp import web
 import asyncio
 import json
 import pickle
-from dataclasses import dataclass
-from queue import Queue, Empty as QueueEmpty
+import sys
 import threading
 import time
-import torch
-import atexit
-from typing import Optional, Tuple
+from dataclasses import dataclass
+from queue import Empty as QueueEmpty
+from queue import Queue
 
-from transformers import AutoModelForCausalLM
+import numpy as np
+
+import lmql.models.lmtp.backends as backends
+import lmql.utils.nputil as nputil
+from lmql.models.lmtp.backends.lmtp_model import LMTPModel
 
 class LMTPCannotLoadModelByPolicy(Exception):
     pass
 
 @dataclass
 class GenerateCall:
     prompt: str
@@ -84,54 +74,25 @@
                 padding = max_len - len(c.prompt)
                 scoring_offsets.append(c.kwargs.get("scoring_offset", 0) + padding)
         else:
             scoring_offsets = None
 
         return cls(input_ids, attention_mask, temperature, max_tokens, logit_biases, calls, is_score, scoring_offsets)
 
-    def logits_processors(self):
-        bias_tensors = None
-        logit_biases = self.logit_biases
-        
-        if len(logit_biases) == 0:
-            return []
-
-        class BatchLogitsProcessor:
-            def __call__(self, input_ids: torch.LongTensor, scores: torch.FloatTensor) -> torch.FloatTensor:
-                nonlocal bias_tensors
-
-                vocab_size = scores.shape[-1]
-                if bias_tensors is None:
-                    bias_tensors = [torch.zeros(vocab_size) for _ in logit_biases]
-                    for i, bias in enumerate(logit_biases):
-                        if len(bias) > 0:
-                            indices = torch.tensor(list(bias.keys()), dtype=torch.long)
-                            values = torch.tensor(list(bias.values()), dtype=torch.float32)
-                            bias_tensors[i][indices] = values
-                    bias_tensors = torch.stack(bias_tensors).to(scores.device)
-
-                return scores + bias_tensors
-
-        return [BatchLogitsProcessor()]
-
     def generate_args(self):
         return {
-            "input_ids": torch.tensor(self.input_ids),
-            "do_sample": self.temperature > 0.0,
-            "attention_mask": torch.tensor(self.attention_mask),
+            "input_ids": self.input_ids,
+            "attention_mask": self.attention_mask,
             "temperature": self.temperature,
             "max_new_tokens": self.max_tokens,
-            "logits_processor": self.logits_processors(),
-            "output_scores": True,
-            "return_dict_in_generate": True,
-            **({"scoring_offsets": self.scoring_offsets} if self.is_score else {})
+            "bias_tensor": self.logit_biases if len(self.logit_biases) > 0 else None
         }
 
 class ScoreStreamer:
-    def log_token(self, batch: GenerateBatch, all_scores: torch.FloatTensor, **kwargs):
+    def log_token(self, batch: GenerateBatch, all_scores, **kwargs):
         batch_size = all_scores.shape[0]
         
         for i in range(batch_size):
             offset = batch.scoring_offsets[i]
             scores = all_scores[i][offset:]
             scored_ids = batch.input_ids[i][offset:]
             call = batch.calls[i]
@@ -146,160 +107,187 @@
                 call.put(token_payload)
 
 class TokenStreamer:
     def __init__(self, batch: GenerateBatch, eos_token_id):
         self.batch = batch
         self.eos_token_id = eos_token_id
 
-    def __call__(self, input_ids: torch.LongTensor, scores: torch.FloatTensor, **kwargs) -> bool:
+    def __call__(self, input_ids, scores, **kwargs) -> bool:
         self.log_token(input_ids, scores, **kwargs)
         return False
 
-    def log_token(self, input_ids: torch.LongTensor, scores: torch.FloatTensor, last=False, **kwargs):
+    def log_token(self, input_ids, scores, last=False, **kwargs):
         batch_size = input_ids.shape[0]
         
         last_tokens = input_ids[:, -1]
         last_scores = scores[-1]
-        
+
         max_num_top_logprobs = max([c.kwargs.get("top_logprobs", 1) for c in self.batch.calls])
 
+        if not nputil.is_array(last_tokens):
+            last_tokens = last_tokens.cpu().numpy()
+        if not nputil.is_array(last_scores):
+            last_scores = last_scores.cpu().numpy()
+
         # for each sample get top logprobs
-        top_logprobs = torch.topk(last_scores, max_num_top_logprobs, dim=-1, largest=True, sorted=True)
+        all_logprobs, all_indices  = nputil.topk(last_scores, max_num_top_logprobs, sorted=True, axis=-1)
+
         for i in range(batch_size):
-            logprobs = top_logprobs.values[i]
-            tokens = top_logprobs.indices[i]
+            logprobs = all_logprobs[i]
+            tokens = all_indices[i]
             token_score = last_scores[i][last_tokens[i]]
 
+            top_logprobs = {
+                int(last_tokens[i]): float(token_score.item()),
+                **{int(token.item()): float(logprob.item()) for logprob, token in zip(logprobs, tokens)}
+            }
+
             num_top_logprobs = self.batch.calls[i].kwargs.get("top_logprobs", 1)
             logprobs = logprobs[:num_top_logprobs]
             tokens = tokens[:num_top_logprobs]
 
             token_payload = {
                 "token": int(last_tokens[i].item()),
                 "stream_id": self.batch.calls[i].stream_id,
                 "logprob": float(token_score.item()),
                 "finish_reason": ("stop" if last_tokens[i].item() == self.eos_token_id else "length" if last else None),
-                "top_logprobs": {
-                    int(token.item()): float(logprob.item()) for logprob, token in zip(logprobs, tokens)
-                }
+                "top_logprobs": top_logprobs
             }
-
+            
             self.batch.calls[i].put(token_payload)
 
 class Scheduler:
     """
     A scheduler that takes calls to generate and batches them together. 
 
-    Can be shared between multiple clients, make sure to call unregister(<user>) when done,
-    to allow the scheduler to shut down when no longer needed by anyone.
+    Can be shared among multiple clients, make sure to call unregister(<user>) when done,
+    to allow the scheduler to shut down when no longer needed.
     """
-    def __init__(self, model_identifier, model_args = None):
+    def __init__(self, model_identifier, model_args = None, sync=False):
         self.model_identifier = model_identifier
         if model_args is None: self.model_args = {}
         else: self.model_args = model_args
         
         self.queue = Queue()
         self.kill_event = threading.Event()
         
-        self.worker_thread = threading.Thread(target=self.worker, daemon=True)
-        self.worker_thread.start()
+        self.sync = sync
+
+        if not self.sync:
+            self.worker_thread = threading.Thread(target=self.worker, daemon=True, name="scheduler-worker")
+            self.worker_thread.start()
+        else:
+            pass
 
         self.users = set()
         self.last_use = time.time()
 
     def put(self, call: GenerateCall):
         self.queue.put(call)
 
-    def batches(self):
+    def batches(self, max_batch_size=8):
         start = time.time()
         calls = []
         # get as many calls from the queue as possible within 0.1 seconds
         while time.time() - start < 0.1:
             try:
                 calls.append(self.queue.get_nowait())
             except QueueEmpty:
                 break
         # group calls into batches
         batches_by_mode = {}
         for c in calls:
             mode = c.generation_mode()
             batches_by_mode.setdefault(mode, []).append(c)
-        return batches_by_mode.values()
+        
+        # split batches that are too large
+        fitting_batches = []
+        for mode, batches in batches_by_mode.items():
+            if len(batches) > max_batch_size:
+                for i in range(0, len(batches), max_batch_size):
+                    fitting_batches.append(batches[i:i+max_batch_size])
+            else:
+                fitting_batches.append(batches)
 
-    def score(
-        self,
-        model,
-        input_ids: torch.LongTensor,
-        attention_mask: torch.LongTensor,
-        eos_token_id: Optional[int] = None,
-        **model_kwargs,
-    ) -> Tuple[torch.FloatTensor, torch.FloatTensor]:
-        # prepare model inputs
-        model_inputs = model.prepare_inputs_for_generation(input_ids, **model_kwargs, eos_token_id=eos_token_id)
-        model_inputs["attention_mask"] = attention_mask
-
-        token_scores = []
-        
-        outputs = model(
-            **model_inputs,
-            return_dict=True,
-            output_attentions=False,
-            output_hidden_states=False,
-        )
-
-        next_token_logits = outputs.logits[:, -len(input_ids), :]
-        next_token_logits = torch.log_softmax(next_token_logits, dim=-1)
-        token_scores = next_token_logits.gather(-1, input_ids)
+        return fitting_batches
 
-        return token_scores
+    async def async_worker(self):
+        """
+        Can be used when self.sync, in place of worker_thread.
 
-    def worker(self):
-        print("[Loading", self.model_identifier, "with", f"AutoModelForCausalLM.from_pretrained({self.model_identifier}, {str(self.model_args)[1:-1]})]", flush=True)
-        model = AutoModelForCausalLM.from_pretrained(self.model_identifier, **self.model_args)
+        Runs the model asynchronously on the main thread. Blocks remaining application
+        during model calls. As a consequence, tokens are only streamed when the model
+        has finished generating the current batch.
+        """
 
-        print("[", self.model_identifier, " ready on device ", model.device, flush=True, sep="", end="]\n")
+        model = LMTPModel.load(self.model_identifier, **self.model_args)
 
         while True:
             if self.kill_event.is_set():
                 break
 
-            for batch in self.batches():
-                eos_token = model.config.eos_token_id
+            if self.queue.empty():
+                await asyncio.sleep(0.01)
+                continue
 
-                try:
-                    b = GenerateBatch.from_calls(batch)
+            self.process_batch(model)
+    
+    def worker(self):
+        """
+        Can be used when not self.sync, in place of async_worker.
+
+        Runs the model on a separate thread. Does not block the application during model
+        calls. As a consequence, tokens are streamed as soon as they are generated.
+
+        This is the default mode and the thread is started automatically when instantiating
+        the scheduler with sync=False.
+        """
+
+        model = LMTPModel.load(self.model_identifier, **self.model_args)
+
+        while True:
+            if self.kill_event.is_set():
+                break
+            self.process_batch(model)
+
+    def process_batch(self, model):
+        for batch in self.batches(model.max_batch_size):
+            try:
+                b = GenerateBatch.from_calls(batch)
+                
+                if b.is_score:
+                    kwargs = b.generate_args()
+                    input_ids = kwargs["input_ids"]
+                    attention_mask = kwargs["attention_mask"]
+                    
+                    scores = model.score(input_ids, attention_mask)
+                    ScoreStreamer().log_token(b, scores)
+                else:
+                    streamer = TokenStreamer(b, model.eos_token_id)
+                    kwargs = b.generate_args()
                     
-                    if b.is_score:
-                        kwargs = b.generate_args()
-                        input_ids = kwargs["input_ids"].to(model.device)
-                        attention_mask = kwargs["attention_mask"].to(model.device)
-                        
-                        scores = self.score(model, input_ids, attention_mask, eos_token_id=eos_token)
-                        ScoreStreamer().log_token(b, scores)
-                    else:
-                        streamer = TokenStreamer(b, model.config.eos_token_id)
-                        kwargs = b.generate_args()
-                        kwargs["input_ids"] = kwargs["input_ids"].to(model.device)
-                        kwargs["attention_mask"] = kwargs["attention_mask"].to(model.device)
-                        result = model.generate(**kwargs, stopping_criteria=[streamer], eos_token_id=eos_token, pad_token_id=eos_token)
-                        streamer.log_token(result.sequences, result.scores, last=True)
-                except Exception as e:
-                    print("[Error during generate()]", e, flush=True)
-                    for c in batch:
-                        c.error("failed to generate tokens '" + str(e) + "'")
-                    raise e
+                    kwargs["input_ids"] = np.array(kwargs["input_ids"], dtype=np.int64)
+                    kwargs["attention_mask"] = np.array(kwargs["attention_mask"], dtype=np.int32)
+
+                    result = model.generate(**kwargs, streamer=streamer)
+                    streamer.log_token(result.sequences, result.scores, last=True)
+            except Exception as e:
+                print("[Error during generate()]", e, flush=True)
+                for c in batch:
+                    c.error("failed to generate tokens '" + str(e) + "'")
+                raise e
 
     @staticmethod
-    def instance(model_identifier, model_args, user, only_existing=False):
+    def instance(model_identifier, model_args, user, only_existing=False, sync=False):
         identifier = (model_identifier, pickle.dumps(model_args).hex())
 
         if identifier not in Scheduler._instances:
             if only_existing:
                 raise LMTPCannotLoadModelByPolicy("Model '" + model_identifier + "' is not loaded and server is not configured to load it on demand.")
-            Scheduler._instances[identifier] = Scheduler(model_identifier, model_args)
+            Scheduler._instances[identifier] = Scheduler(model_identifier, model_args, sync=sync)
 
         s = Scheduler._instances[identifier]
         s.last_use = time.time()
         
         if user is not None:
             s.users.add(user)
 
@@ -422,62 +410,8 @@
                 scheduler.unregister(self)
                 
                 if self.longrunning:
                     scheduler.gc()
                 else:
                     Scheduler.gc(0)
             except LMTPCannotLoadModelByPolicy:
-                pass
-
-class LMTPWebSocketTransport:
-    """
-    Exposes a LMTP TokenSession over a websocket.
-    """
-    def __init__(self, ws):
-        self.ws = ws
-        self.queue = asyncio.Queue()
-        self._dumper = asyncio.create_task(self.dumper())
-
-    async def dumper(self):
-        while True:
-            try:
-                batch = [await self.queue.get()]
-                # while len(batch) < 1:
-                #     try:
-                #         batch.append(await asyncio.wait_for(self.queue.get(), timeout=0.1))
-                #     except asyncio.TimeoutError:
-                #         break
-                if len(batch) > 0:
-                    await self.ws.send_str("TOKEN" + " " + json.dumps(batch))
-            except asyncio.CancelledError:
-                break
-            except Exception as e:
-                print("LMTPWebSocketTransport.dumper error", e, flush=True)
-
-    async def send(self, type, payload):
-        await self.queue.put(payload)
-
-    @staticmethod
-    async def listen(ws, model_args, static):
-        transport = LMTPWebSocketTransport(ws)
-        session = TokenSession(transport, model_args, static=static, longrunning=True)
-
-        try:
-            async for msg in ws:
-                if msg.type == aiohttp.WSMsgType.TEXT:
-                    cmd, kwargs = msg.data.split(" ", 1)
-                    
-                    kwargs = json.loads(kwargs)
-                    logit_bias = kwargs.pop("logit_bias", {})
-                    logit_bias = {int(k): float(v) for k, v in logit_bias.items()}
-                    kwargs["logit_bias"] = logit_bias
-                    
-                    await session.handle(cmd, kwargs)
-                elif msg.type == aiohttp.WSMsgType.ERROR:
-                    break
-        finally:
-            transport._dumper.cancel()
-            session.close()
-            await ws.close()
-
-    async def close(self):
-        await self.ws.close()
+                pass
```

### Comparing `lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_multiprocessing.py` & `lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_multiprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 A client/server implementation for LMTP that runs the model in a subprocess
 and communicates with it via multiprocessing pipes (IPC).
 """
 
 import multiprocessing
+from multiprocessing.connection import Connection
 import pickle
 import sys
 from .lmtp_client import *
 from .lmtp_inference_server import TokenSession
 
 async def multiprocessing_main_async(pipe: Connection, kwargs):
-    transport = LMTPMulitprocessingTransport(pipe)
+    transport = LMTPMultiprocessingTransport(pipe)
     session = TokenSession(transport, kwargs)
 
     try:
         while True:
             if not multiprocessing.parent_process().is_alive():
                 print("[Parent process died, exiting]", flush=True)
                 break
@@ -30,15 +31,15 @@
     finally:
         sys.exit(0)
 
 
 def multiprocessing_main(pipe: Connection, kwargs):
     asyncio.run(multiprocessing_main_async(pipe, kwargs))
 
-class LMTPMulitprocessingTransport:
+class LMTPMultiprocessingTransport:
     def __init__(self, pipe):
         self.connection: Connection = pipe
 
     async def send(self, type, payload):
         self.connection.send((type, payload))
 
 def ensure_picklable(kwargs, msg=""):
@@ -73,19 +74,19 @@
 class LMTPMultiProcessingClient:
     """
     Allows use of a LMTP TokenSession from within the same process (model runs in the same process too).
     """
 
     def __init__(self, model_identifier, **kwargs):
         ensure_picklable(kwargs, "lmtp.inprocess kwargs must be pickleable as it has to be sent to a subprocess")
-        
         self.model_identifier = model_identifier
 
         (c2, c1) = multiprocessing.Pipe(duplex=True)
-        self.subprocess = multiprocessing.Process(target=multiprocessing_main, args=(c1,kwargs), name="lmtp-model-server", daemon=True)
+        self.subprocess = multiprocessing.Process(target=multiprocessing_main, args=(c1,kwargs), 
+                                                  name="lmtp-model-server", daemon=True)
         self.subprocess.start()
         
         self.connection = c2
         
         self.stream_id = 0
         self.iterators = {}
```

### Comparing `lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_serve.py` & `lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_serve.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     """
     Serves the provided model as an LMTP/LMQL inference endpoint.
 
     Args:
         model_name (str): The model to load or 'auto' if any model should automatically be loaded on client request.
         host (str, optional): The host to serve the model on. Defaults to "localhost".
         port (int, optional): The port to serve the model on. Defaults to 8080.
+        single_thread (bool, optional): If set, the model and the inference server will run in the same thread. Defaults to False. This can lead to increased latency when processing multiple requests, but may be required depending on model implementation.
         cuda (bool, optional): If set, the model will be loaded on the GPU. Defaults to False.
         dtype (str, optional): What format to load the model weights. Options: 'float16' (not available on all models), '8bit' (requires bitsandbytes). Defaults to None.
         static (bool, optional): If set, the model cannot be switched on client request but remains fixed to the model specified in the model argument. Defaults to False.
         **kwargs: Any other argument will be passed as a keyword argument to the AutoModelForCausalLM.from_pretrained function.
 
     """
     return lmtp_serve_main({
@@ -34,41 +35,55 @@
     CLI for starting an LMTP server with a given HuggingFace 'transformers' model.
     """
 
     # extract explicit arguments
     host = model_args.pop("host", "localhost")
     port = model_args.pop("port", 8080)
     model = model_args.pop("model", None)
-    static = model_args.pop("static", False)
+    single_thread = model_args.pop("single_thread", False)
+    static = model_args.pop("static", False) or single_thread
     
+    assert not single_thread or model != "auto", "Cannot use --single_thread mode with model 'auto'. Please specify a specific model to load."
+
     # check 'auto' vs static
     assert not static or model != "auto", "Cannot use --static mode with model 'auto'. Please specify a specific model."
 
     # all other arguments are model arguments
     model_args = rename_model_args(model_args)    
 
     # stream endpoint
     async def stream(request):
         # bidirectional websocket 
         ws = web.WebSocketResponse()
         await ws.prepare(request)
         await LMTPWebSocketTransport.listen(ws, model_args, static=static)
 
-    if model != "auto":
+    if model != "auto" and not single_thread:
         Scheduler.instance(model, model_args, user=None)
 
     app = web.Application()
     app.add_routes([web.get('/', stream)])
-    web.run_app(app, host=host, port=port)
+    
+    def web_print(*args):
+        if len(args) == 1 and args[0].startswith("======== Running on"):
+            print(f"[Serving LMTP endpoint on ws://{host}:{port}/]")
+        else:
+            print(*args)
+    
+    # r executor
+    tasks = [web._run_app(app, host=host, port=port, print=web_print)]
+    if static and single_thread:
+        tasks += [Scheduler.instance(model, model_args, user=None, sync=True).async_worker()]
+    asyncio.get_event_loop().run_until_complete(asyncio.gather(*tasks))
 
 def argparser(args):
     next_argument_name = None
     
     kwargs = {}
-    flag_args = ["cuda", "static"]
+    flag_args = ["cuda", "static", "single_thread"]
 
     help_text = """
 usage: serve-model [-h] [--port PORT] [--host HOST] [--cuda] [--dtype DTYPE] [--[*] VALUE] model
 
 positional arguments:
   model          The model to load or 'auto' if the model should be automatically loaded on client request.
 
@@ -97,14 +112,23 @@
             if next_argument_name is None:
                 assert not "model" in kwargs, "Positional argument 'model' already specified"
                 kwargs["model"] = arg
             else:
                 assert next_argument_name is not None
                 if arg == "True": arg = True
                 elif arg == "False": arg = False
+                else:
+                    try:
+                        arg = int(arg)
+                    except:
+                        try:
+                            arg = float(arg)
+                        except:
+                            arg = str(arg)
+
 
                 kwargs[next_argument_name] = arg
                 next_argument_name = None
 
     if not "model" in kwargs:
         kwargs["model"] = "auto"
```

### Comparing `lmql-0.0.6.4/src/lmql/models/lmtp/lmtp_threading.py` & `lmql-0.0.6.5/src/lmql/models/lmtp/lmtp_threading.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/models/model.py` & `lmql-0.0.6.5/src/lmql/models/model.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,16 +4,21 @@
     def __init__(self, model_identifier, model=None, **kwargs):
         self.model_identifier = model_identifier
         self.kwargs = kwargs
 
         # if this is a fixed reference to an existing model
         self.model = model
 
-global inprocess_models
-inprocess_models = {}
+    def __repr__(self) -> str:
+        return str(self)
+    
+    def __str__(self):
+        return "<LMQLModel: {}>".format(self.model_identifier)
+
+LMQLModel.inprocess_instances = {}
 
 def inprocess(model_name, use_existing_configuration=False, **kwargs):
     """
     Loads a 'transformers' model in-process.
 
     This is useful when you don't want to spawn a separate 'lmql serve-model' process.
 
@@ -26,48 +31,49 @@
         
         kwargs: Additional arguments to pass to the serve-model command line. (see lmql serve-model --help)
                 For this, use keys as they occur in the command line, e.g. 'port' for '--port' and for
                 boolean flags, use True/False as values, e.g. 'cuda=True' for '--cuda'.
     Return:
         InProcessServer: An object representing the loaded model, can be passed in the 'from' clause of a query.
     """
-    try:
-        import transformers
-        from .lmtp.lmtp_dcmodel import lmtp_model
-    except ImportError:
-        raise NotImplementedError("Your installation of LMQL does not support local models via inprocess(). Please make sure you have 'transformers' installed.")
-
+    from .lmtp.lmtp_dcmodel import lmtp_model
     assert not model_name.startswith("openai/"), "openai/ models cannot be loaded with inprocess=True, they always use the remote API."
 
     # extract/reassign renamed like 'cuda'
     kwargs = rename_model_args(kwargs)
 
+    # special case for 'llama.cpp'
+    if model_name.startswith("llama.cpp:"):
+        # kwargs["async_transport"] = True
+        kwargs["tokenizer"] = "huggyllama/llama-7b"
+
     if "endpoint" in kwargs:
         print("info: 'endpoint' argument is ignored for inprocess=True/local: models.")
 
     cmdline_args = f"{model_name} "
     for k,v in kwargs.items():
         if type(v) is bool:
             cmdline_args += f"--{k} "
         else:
             cmdline_args += f"--{k} {v} "
 
-    if cmdline_args in inprocess_models:
-        print("info: reusing existing in-process model.")
-        model = inprocess_models[cmdline_args]
+    if cmdline_args in LMQLModel.inprocess_instances.keys():
+        print("info: reusing existing in-process model.", flush=True)
+        model = LMQLModel.inprocess_instances[cmdline_args]
         return LMQLModel(model_name, model=model)
-    
+
     if use_existing_configuration:
         # find existing match for model_name only
-        for cmdargs, p in inprocess_models.items():
+        for cmdargs, p in LMQLModel.inprocess_instances.items():
             if cmdargs.split(" ")[0] == model_name:
                 return LMQLModel(model_name, model=p)
     
-    model = lmtp_model(model_name, inprocess=True, **kwargs)
-    inprocess_models[cmdline_args] = model
+    kwargs["inprocess"] = True
+    model = lmtp_model(model_name, **kwargs)
+    LMQLModel.inprocess_instances[cmdline_args] = model
     return LMQLModel(model_name, model=model)
 
 def model(model_identifier, **kwargs):
     # handle inprocess models
     is_inprocess = kwargs.pop("inprocess", False) or model_identifier.startswith("local:")
     if is_inprocess and model_identifier.startswith("local:"):
         model_identifier = model_identifier[6:]
```

### Comparing `lmql-0.0.6.4/src/lmql/ops/follow_map.py` & `lmql-0.0.6.5/src/lmql/ops/follow_map.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ops/ops.py` & `lmql-0.0.6.5/src/lmql/ops/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,15 +447,15 @@
             if is_next_token(op1): 
                 return fmap(
                     ("*", True)
                 )
             else:
                 return InOpStrInSet([]).follow(op2, [op1])
 
-        if type(op1) is str or type(op1) is str:
+        if type(op1) is str or type(op2) is str:
             op_shorter = op1 if len(strip_next_token(op1)) < len(strip_next_token(op2)) else op2
             op_longer = op1 if len(strip_next_token(op1)) > len(strip_next_token(op2)) else op2
 
             if strip_next_token(op_longer) == op_longer and strip_next_token(op_shorter) != op_shorter:
                 return InOpStrInSet([]).follow(op_shorter, [op_longer])
 
         return all([a == args[0] for a in args])
@@ -569,32 +569,40 @@
         if l == "fin": 
             return "fin"
         if result is not None and (l == "fin" or l == "inc"):
             return "fin"
         else: return "var"
 
 class Var(Node):
-    def __init__(self, name):
+    def __init__(self, name, python_variable=False):
         super().__init__([])
         self.name = name
+        self.python_variable = python_variable
 
         self.depends_on_context = True
         
         # indicates whether the downstream node requires text diff information
         self.diff_aware_read = False
 
     async def json(self):
         return self.name
 
     def forward(self, context, **kwargs):
+        if self.python_variable:
+            return context.python_scope.get(self.name)
+
         if self.diff_aware_read:
             return (context.get(self.name, None), context.get_diff(self.name, None))
+        
         return context.get(self.name, None)
     
     def follow(self, context, **kwargs):
+        if self.python_variable:
+            return context.python_scope.get(self.name)
+
         value = context.get(self.name, None)
         if value is None: return None
         
         # also return the text diff if required
         if self.diff_aware_read:
             value = (value, context.get_diff(self.name, None))
 
@@ -605,14 +613,16 @@
 
         return fmap(
             ("eos", PredeterminedFinal(strip_nt(value), "fin")),
             ("*", value),
         )
 
     def final(self, x, context, operands=None, result=None, **kwargs):
+        if self.python_variable:
+            return "fin"
         return context.final(self.name)
 
     def __repr__(self) -> str:
         return f"<Var {self.name}>"
 
 class RawValueOp(Node):
     def __init__(self, args):
```

### Comparing `lmql-0.0.6.4/src/lmql/ops/token_set.py` & `lmql-0.0.6.5/src/lmql/ops/token_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     def init(tokenizer):
         if VocabularyMatcher._instance is not None:
             return
 
         # first try to load pickled matcher from cache (faster)
         import pickle
 
-        cache_identifier = tokenizer.model_identifier.replace("/", "-")
+        cache_identifier = tokenizer.model_identifier.replace("/", "-").replace(":", "__")
         cache_identifier += "-" + type(tokenizer.tokenizer_impl).__name__.replace("[^a-z0-9]", "")
         cache_path = f"token-mask-cache-{cache_identifier}.pkl"
         matcher_path = f"matcher-{cache_identifier}.pkl"
 
         try:
             with cachefile(matcher_path, "rb") as f:
                 VocabularyMatcher._instance = pickle.load(f)
```

### Comparing `lmql-0.0.6.4/src/lmql/output/http.py` & `lmql-0.0.6.5/src/lmql/output/http.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/output/sse.py` & `lmql-0.0.6.5/src/lmql/output/sse.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/output/ws.py` & `lmql-0.0.6.5/src/lmql/output/ws.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/runtime/bopenai/__init__.py` & `lmql-0.0.6.5/src/lmql/runtime/bopenai/__init__.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/runtime/bopenai/batched_openai.py` & `lmql-0.0.6.5/src/lmql/runtime/bopenai/batched_openai.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/runtime/bopenai/openai_api.py` & `lmql-0.0.6.5/src/lmql/runtime/bopenai/openai_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,16 +49,23 @@
     def __enter__(self):
         self.task = asyncio.create_task(self.task)
         return self
     
     def __exit__(self, *args):
         self.task.cancel()
 
+def is_azure_chat(kwargs):
+    if not "api_config" in kwargs: return False
+    api_config = kwargs["api_config"]
+    if not "api_type" in api_config: 
+        return os.environ.get("OPENAI_API_TYPE", "azure") == "azure-chat"
+    return ("api_type" in api_config and "azure-chat" in api_config.get("api_type", ""))
+
 async def complete(**kwargs):
-    if kwargs["model"].startswith("gpt-3.5-turbo") or "gpt-4" in kwargs["model"]:
+    if kwargs["model"].startswith("gpt-3.5-turbo") or "gpt-4" in kwargs["model"] or is_azure_chat(kwargs):
         async for r in chat_api(**kwargs): yield r
     else:
         async for r in completion_api(**kwargs): yield r
 
 global tokenizer
 tokenizer = None
 
@@ -93,59 +100,63 @@
         offset = m.end()
     segments.append({"tag": current_tag, "text": s[offset:]})
     return segments
 
 
 def get_azure_config(model, api_config):
     endpoint = api_config.get("endpoint", None)
+    api_type = api_config.get("api_type", os.environ.get("OPENAI_API_TYPE", ""))
 
-    # first check endpoint configuration
-    if endpoint is not None and endpoint.startswith("azure:"):
-        endpoint = "https:" + endpoint[6:]
-        env_name = model.upper().replace(".", "_")
+    if (api_type == "azure" or api_type == "azure-chat"):
+        api_base = api_config.get("api_base", None) or os.environ.get("OPENAI_API_BASE", None)
+        assert api_base is not None, "Please specify the Azure API base URL as 'api_base' or environment variable OPENAI_API_BASE"
+        api_version = api_config.get("api_version", None) or os.environ.get("OPENAI_API_VERSION", "2023-05-15")
+        deployment = api_config.get("api_deployment", None) or os.environ.get("OPENAI_DEPLOYMENT", model)
         
-        azure_key = api_config.get("azure_api_key", None)
-        if azure_key is None:
-            assert "AZURE_OPENAI_" + env_name + "_KEY" in os.environ, f"Please set the environment variable AZURE_OPENAI_{env_name}_KEY to your Azure API key, or specify it in code as 'lmql.model(..., azure_api_key=...')"
-            azure_key = os.environ["AZURE_OPENAI_" + env_name + "_KEY"]
+        deployment_specific_api_key = f"OPENAI_API_KEY_{deployment.upper()}"
+        api_key = api_config.get("api_key", None) or os.environ.get(deployment_specific_api_key, None) or os.environ.get("OPENAI_API_KEY", None)
+        assert api_key is not None, "Please specify the Azure API key as 'api_key' or environment variable OPENAI_API_KEY or OPENAI_API_KEY_<DEPLOYMENT>"
         
-        headers = {
-            "Content-Type": "application/json",
-            "api-key": azure_key,
-        }
+        is_chat = api_type == "azure-chat"
 
-        return endpoint, headers
+        if is_chat:
+            endpoint = f"{api_base}/openai/deployments/{deployment}/chat/completions"
+        else:
+            endpoint = f"{api_base}/openai/deployments/{deployment}/completions"
+        
+        if api_version is not None:
+            endpoint += f"?api-version={api_version}"
 
-    # then check env
-    if os.environ.get("OPENAI_API_TYPE", 'openai') == 'azure':
-        model_env_name = model.upper().replace(".", "_")
-        endpoint = os.environ[f"AZURE_OPENAI_{model_env_name}_ENDPOINT"]
-        assert "AZURE_OPENAI_" + model_env_name + "_KEY" in os.environ, f"Please set the environment variable AZURE_OPENAI_{model_env_name}_KEY to your Azure API key, or specify it in code as 'lmql.model(..., azure_api_key=...')"
-        key = os.environ[f"AZURE_OPENAI_{model_env_name}_KEY"]
         headers = {
             "Content-Type": "application/json",
-            "api-key": key,
+            "api-key": api_key,
         }
+
+        if "verbose" in api_config and api_config["verbose"] or os.environ.get("OPENAI_VERBOSE", "0") == "1":
+            print(f"Using Azure API endpoint: {endpoint}", is_chat)
+
         return endpoint, headers
 
+    return None
+
 def get_endpoint_and_headers(kwargs):
     model = kwargs["model"]
     api_config = kwargs.pop("api_config", {})
     endpoint = api_config.get("endpoint", None)
 
     # try to get azure config from endpoint or env
     azure_config = get_azure_config(model, api_config)
     if azure_config is not None:
         return azure_config
     
     # otherwise use custom endpoint as plain URL without authorization
     if endpoint is not None:
-        if not endpoint.endswith("http"):
+        if not endpoint.startswith("http"):
             endpoint = f"http://{endpoint}"
-        return endpoint + "/completions", {
+        return endpoint, {
             "Content-Type": "application/json"
         }
     
     # use standard public API config
     from lmql.runtime.openai_secret import openai_secret, openai_org
     if kwargs["model"].startswith("gpt-3.5-turbo") or "gpt-4" in kwargs["model"]:
         endpoint = "https://api.openai.com/v1/chat/completions"
@@ -207,25 +218,25 @@
         else:
             print(f"warning: {tag} is not a valid tag for the OpenAI chat API. Please use one of :system, :user or :assistant.")
         
         messages.append({
             "role": role, 
             "content": s["text"]
         })
-    
+
     del kwargs["prompt"]
     kwargs["messages"] = messages
     
     del kwargs["logprobs"]
 
     async with CapacitySemaphore(num_prompts * max_tokens):
         
         current_chunk = ""
         stream_start = time.time()
-        
+
         async with aiohttp.ClientSession() as session:
             endpoint, headers = get_endpoint_and_headers(kwargs)
             async with session.post(
                     endpoint,
                     headers=headers,
                     json={**kwargs},
             ) as resp:
```

### Comparing `lmql-0.0.6.4/src/lmql/runtime/caching.py` & `lmql-0.0.6.5/src/lmql/runtime/caching.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_array.py` & `lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_array.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_cache.py` & `lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
         if hasattr(self.delegate, "close"):
             self.delegate.close()
     
     def base_key(self, ids, *args):
         if isinstance(ids, DecoderSequence):
             return self.base_key(ids.input_ids)
-        return str(ids)
+        return "[" + ",".join([str(i) for i in ids]) + "]"
 
     async def get_mask(self, s: DecoderSequence, **kwargs):
         if s.id in self.mask_cache:
             return self.mask_cache[s.id]
         if hasattr(s, "logits_mask"):
             return s.logits_mask
 
@@ -219,17 +219,18 @@
             # check cache for all
             cache_entries = [await self.get_cache(s, 'top-1', user_data=True, **kwargs) for s in seqs]
             cached_tokens = [e[1] for e in cache_entries]
             cache_keys = [e[0] for e in cache_entries]
 
             # apply operation for non-cached
             non_cached = [s for s, c in zip(seqs, cached_tokens) if c is None]
+            # if len(non_cached) == 0:
+            #     print("cache hit for", len(cache_keys[0][0][0]), cache_keys[0][0][0][-50:], "with", cached_tokens[0][0])
             # generator over new results
-            non_cached_argmax = iter((await self.delegate.argmax(DataArray(non_cached), **kwargs)).items())
-            
+            non_cached_argmax = iter((await self.delegate.argmax(DataArray(non_cached), **kwargs)).items())                
             results = []
             # put new results in cache
             for i, (s, key, c) in enumerate(zip(seqs, cache_keys, cached_tokens)):
                 if c is None: 
                     r = next(non_cached_argmax)
                     results.append(r)
                     self.set_cache(key, r)
@@ -316,16 +317,17 @@
                 if any(ct is None for ct in c):
                     r = next(non_cached_sample)
                     if any(ct is not None for ct in c):
                         mask = (await self.get_mask(s, **kwargs)).logits_mask[0]
                         # print("WARNING: some cache entries are None, but some are not", len([e for e in c if e is not None]), len(r.token))
                         # print([await s.text()])
                     results.append(r)
-                    next_token_ids = ensure_iterable(r.token)
-                    next_token_scores = ensure_iterable(r.logprob)
+                    next_token_ids = ensure_iterable(r.token)[:len(key)]
+                    next_token_scores = ensure_iterable(r.logprob)[:len(key)]
+
                     # cache each continuation separately
                     assert len(next_token_ids) <= len(key)
                     for i,ck in zip(range(len(next_token_ids)), key):
                         self.set_cache(ck, (next_token_ids[i], next_token_scores[i]))
                     
                     # fill remaining top-k slots with empty result
                     for i in range(len(next_token_ids) + 1, k + 1):
@@ -446,16 +448,15 @@
                 token_scores = np.array(result.logprobs[len(sq.input_ids):].tolist() + result.next_logprobs.tolist())
                 completion = np.array(unexpanded_tok)
                 assert len(token_scores) == len(completion), f"Expected {len(completion)} scores, but got {len(token_scores)}"
 
                 # store in cache
                 ids = continued_seq.input_ids
                 for i, (score, token) in enumerate(zip(token_scores[-len(tok):], tok)):
-                    # TODO: is this the correct user_data?
-                    self.set_cache([(self.base_key(ids, user_data if i > 0 else sq.user_data), str(token))], (np.array(token), np.array(score)))
+                    self.set_cache([(self.base_key(ids), str(token))], (np.array(token), np.array(score)))
                     ids = np.append(ids, token)
                 
             # determine detseq deterministic flags
             if type(deterministic) is bool:
                 deterministic_flags = np.concatenate([sq.deterministic, np.array([deterministic])])
                 next_deterministic = np.array([deterministic] * len(completion[1:]))
             else:
```

### Comparing `lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_global.py` & `lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_global.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_model.py` & `lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,14 @@
 
     async def argmax(self, sequences, **kwargs):
         """
         Returns a pool with `n` sampled successor nodes per node in the pool.
         """
         raise NotImplementedError()
 
-
     async def score(self, sqs: List[DecoderSequence], tokens: List[List[int]], max_batch_size=None, deterministic: Union[bool, List[bool]]=False, stop_phrase=False, needs_rewrite=True, user_data=None, noscore=False, internal=False):
         raise NotImplementedError()
         
     async def score_tokens(self, sqs: List[DecoderSequence], tokens: List[List[int]], max_batch_size=None, noscore=False):
         """
         Iterates the scores for 'tokens' when appended to the sequences in 'sqs', element-wise.
```

### Comparing `lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_rewrite.py` & `lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_rewrite.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/runtime/dclib/dclib_seq.py` & `lmql-0.0.6.5/src/lmql/runtime/dclib/dclib_seq.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 
     @property
     def num_tokens(self):
         return len(self.input_ids) - self.prompt_len
 
     async def detokenized(self, name):
         async def seqtext_provider():
-            t = str([get_tokenizer().decode(self.input_ids)][0])
+            t = str(get_tokenizer().decode(self.input_ids))
             t = str(t.encode("utf-8"))[2:-1]
             return t
         async def text_provider():
             t = str([get_tokenizer().decode(self.input_ids[-1:])])[2:-2]
             INVALID_CHARACTER = "\uFFFD"
             if INVALID_CHARACTER in t:
                 # use token id
@@ -351,15 +351,15 @@
 
         if stop_phrases is None:
             return new_stop_phrase
 
         ids = np.concatenate([self.input_ids, continuation.token.reshape(1)])
         for stop in stop_phrases:
             len_stop = len(stop)
-            if ids[-len_stop:] == stop:
+            if all(ids[-len_stop:] == stop):
                 new_stop_phrase[-len_stop:] = True
                 break
 
         return new_stop_phrase
 
     def __len__(self):
         return len(self.input_ids)
@@ -388,15 +388,17 @@
             return f"<seq token_len={len(self.input_ids)} ids=[... {ids}]>"
 
     def __str__(self):
         ids = ", ".join([str(i) for i in self.input_ids[-10:]])
         return f"<seq token_len={len(self.input_ids)} ids=[... {ids}]>"
 
     def is_done(self):
-        return self.input_ids[-1] == get_tokenizer().eos_token_id or self.input_ids[-1] == str(get_tokenizer().eos_token_id).encode() or self.input_ids[-1] == b"<|endoftext|>"
+        return self.input_ids[-1] == get_tokenizer().eos_token_id or \
+            self.input_ids[-1] == str(get_tokenizer().eos_token_id).encode() or \
+            self.input_ids[-1] == b"<|endoftext|>"
 
     def make_successors(self, next_tokens, next_token_scores, logits, user_data=None):
         # remove very low scoring tokens (likely they were masked and therefore score low)
         next_tokens = nputil.ensure_iterable(next_tokens)
         next_token_scores = nputil.ensure_iterable(next_token_scores)
         
         tokens = [t for t, s in zip(next_tokens, next_token_scores) if s > DecoderSequence.truncation_threshold]
@@ -478,14 +480,15 @@
         self.align_user_data()
 
     # async def text(self, offset: int = None, limit: int = None, pretty=True) -> str:
     #     return "<detseq> " + await super().text(offset, limit, pretty)
 
     def align_user_data(self):
         if self.user_data is None: return
+        if not "head" in self.user_data: return
 
         # lmql-specific user data should be different for deterministic sequences
         head_variable = resolve_path(self.user_data, "head.variable")
 
         if head_variable is not None:
             # if "before(" in head_variable:
             #     head_variable = head_variable.split(":before(", 1)[0]
```

### Comparing `lmql-0.0.6.4/src/lmql/runtime/dclib/decoders.py` & `lmql-0.0.6.5/src/lmql/runtime/dclib/decoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,44 @@
         
         step += 1
 
         yield (h, done)
 
     dc.finish(done)
 
+
+@dc.decoder
+async def my_argmax(prompt_ids: np.ndarray, n=1, max_len=2048, **kwargs):
+    model = dc.model(**kwargs)
+    h = dc.seqs([dc.seq(prompt_ids)] * 1)
+    done = dc.seqs()
+    step = 0
+    
+    # provide early first result to user
+    yield h
+
+    while len(h) > 0:
+        # extend current hypothesis with top-k continuations
+        h = h.extend(await model.topk_continuations(h, k=4, **kwargs))
+        # check logprob of each continuation
+        for s in h.items():
+            print(s.logprobs[-1], flush=True)
+        # select top-1 continuation only
+        h = dc.topk(h, 1)
+        
+        print(h, flush=True)
+        h = await model.rewrite(h, noscore=True)
+        h, done = (h + done).separate_by(dc.logical_not(dc.eos), dc.lt(max_len))
+        
+        step += 1
+
+        yield (h, done)
+
+    dc.finish(done)
+
 @dc.decoder
 async def sample(prompt_ids: np.ndarray, temperature=1, n=1, max_len=2048, **kwargs):
     model = dc.model(**kwargs)
     h = dc.seqs([dc.seq(prompt_ids)] * n)
     done = dc.seqs()
 
     while len(h) > 0:
```

### Comparing `lmql-0.0.6.4/src/lmql/runtime/interpreter.py` & `lmql-0.0.6.5/src/lmql/runtime/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from lmql.runtime.tokenizer import LMQLTokenizer
 from lmql.runtime.interrupt import interrupt
 from lmql.language.qstrings import qstring_to_stmts, TemplateVariable, DistributionVariable, unescape_qstring
 from lmql.utils.nputil import replace_inf_nan_with_str
 
 from lmql.ops.token_set import VocabularyMatcher, has_tail
 from lmql.runtime.model_registry import LMQLModelRegistry
-from lmql.models.model import LMQLModel
+from lmql.models.model import model, LMQLModel
 
 from lmql.ops.token_set import tset
 import lmql.ops.ops as ops
 
 class _DCLibDebugPrinter: pass
 _DCLibDebugPrinter.printer = None
 
@@ -37,34 +37,47 @@
     rewritten_seq_user_data: Optional[Union[List[Dict[str, Any]], Dict[str, Any]]] = None
 
 class advance: pass # used as symbol
 
 class PromptState(NamedTuple):
     variable : str
     prompt : str
+    
     stmt_buffer : List[Any]
     query_head : Any
     program_state : Any
+    
     recurring_variable_counter : Dict[str, int]
     variable_offset : int
 
+    # optional extra constraint only applicable to current context (inline where)
+    constraints: Optional[ops.Node]
+
     # only set after processing where clause
     valid: Optional[bool]
     final: Optional[str] 
     mask : Optional[Any]
     stopping_phrases: Optional[Any]
     where: Optional[Any]
 
     def __str__(self):
         return f"<PromptState '{self.prompt}'>"
 
     def updated(self, **updated):
         data_dict = self._asdict()
         data_dict.update(updated)
         return PromptState(**data_dict)
+    
+    def full_where_condition(self, interpreter):
+        if interpreter.where is None:
+            return self.constraints
+        elif self.constraints is None:
+            return interpreter.where
+        else:
+            return ops.AndOp([interpreter.where, self.constraints])
 
 class LMQLContext:
     def __init__(self, interpreter, state):
         self.interpreter = interpreter
         
         if state:
             self.program_state: ProgramState = state.program_state
@@ -89,16 +102,16 @@
             return dcmodel.calls - dcmodel.hits
         else:
             return 0
 
     async def get_var(self, name):
         return self.program_state.get_program_value(name)
 
-    async def query(self, qstring):
-        return InterpreterCall(qstring, loc=None)
+    async def query(self, qstring, __locals, constraints=None):
+        return InterpreterCall(qstring, __locals, constraints, loc=None)
 
     async def set_model(self, model_name):
         self.interpreter.set_model(model_name)
 
     async def set_decoder(self, method, **kwargs):
         self.interpreter.set_decoder(method, **kwargs)
 
@@ -113,14 +126,22 @@
         return self.program_state.variable_program_values.copy()
 
     async def set_distribution(self, distribution_variable, values):
         self.interpreter.distribution_variable = distribution_variable
         self.interpreter.distribution_values = values
 
     async def get_return_value(self, *args):
+        # for lmql.F functions, do not use LMQLResult and unpack single results
+        if "is_f_function" in self.interpreter.extra_kwargs:
+            result_values = await self.get_all_vars()
+            if len(result_values) == 1:
+                return list(result_values.values())[0]
+            else:
+                return result_values
+
         return LMQLResult(self.state.prompt, await self.get_all_vars(),self.interpreter.distribution_variable, self.interpreter.distribution_values)
 
 
 @dataclass
 class LMQLResult:
     prompt: str
     variables: Dict[str, str]
@@ -191,76 +212,88 @@
 
         if "backend" in kwargs:
             LMQLModelRegistry.backend_configuration = kwargs["backend"]
 
     def set_model(self, model_name):
         model_args = {}
 
-        if type(model_name) is not str:
-            assert isinstance(model_name, LMQLModel), "Not a supported LMQL model '{}' of type '{}'".format(model_name, type(model_name))
-            model_object = model_name
-
-            if model_name.model is not None:
-                model_object = model_name.model
-                # if model_object is a type reference, we can use the model_identifier
-                if callable(model_object):
-                    model_object = model_object()
+        if type(model_name) is str:
+            model_name = model(model_name)
 
-                self.model_identifier = model_object.model_identifier
-                self.model = model_object
+        assert isinstance(model_name, LMQLModel), "Not a supported LMQL model '{}' of type '{}'".format(model_name, type(model_name))
+        model_object = model_name
 
-                # setup the VocabularyMatcher to use the concrete vocabulary of the model
-                VocabularyMatcher.init(self.model.get_tokenizer())
+        if model_name.model is not None:
+            model_object = model_name.model
+            # if model_object is a type reference, instantiate it
+            if callable(model_object):
+                model_object = model_object()
 
-                return
-            else:
-                model_name = model_object.model_identifier
-                model_args = model_object.kwargs
+            self.model_identifier = model_object.model_identifier
+            self.model = model_object
+
+            # setup the VocabularyMatcher to use the concrete vocabulary of the model
+            VocabularyMatcher.init(self.model.get_tokenizer())
+
+            return
+        else:
+            model_name = model_object.model_identifier
+            model_args = model_object.kwargs
 
         if self.model is None:
             self.model = model_name
             self.model_identifier = model_name
+        elif type(self.model_identifier) is not str:
+            self.model_identifier = self.model.model_identifier
 
         client = LMQLModelRegistry.get(self.model, **model_args)
 
         # setup the VocabularyMatcher to use the concrete vocabulary of the model
         VocabularyMatcher.init(client.get_tokenizer())
         
         # for OpenAI models we optimize for compact logit masks
-        if self.model.startswith("openai/"):
+        if self.model_identifier.startswith("openai/"):
             self.prefers_compact_mask = True
 
         self.model = client
 
     async def advance(self, state: PromptState):
         if state.variable is not None:
             return state
         
         variable = state.variable
+        constraints = state.constraints
+        
         stmt_buffer = state.stmt_buffer
+        constraints_after_last_continue = constraints
+        program_variables_after_last_continue = None
         prompt = state.prompt
 
         distribution_variable = None
         distribution_values = None
 
         query_head = state.query_head
 
         async def continue_for_more_prompt_stmts():
-            nonlocal stmt_buffer
-            nonlocal query_head
+            nonlocal stmt_buffer, query_head, constraints_after_last_continue, program_variables_after_last_continue
 
             if len(stmt_buffer) != 0: return
             
             if query_head.current_args is None:
                 query_head = query_head.copy()
                 assert query_head.fresh_copy, "query head must be fresh copy to avoid state sharing side effects"
                 query_head.context = LMQLContext(self, state)
                 await query_head.continue_()
 
             qstring = query_head.current_args[0]
+            constraints_after_last_continue = query_head.current_args[2] if len(query_head.current_args) > 2 else None
+            
+            if len(query_head.current_args) > 2:
+                program_variables_after_last_continue = query_head.current_args[1]
+            
             stmt_buffer = qstring_to_stmts(qstring) + [advance]
 
             # return context used for last continue_
             return query_head.context
         
         try:
             while variable is None and query_head.result is None:
@@ -268,18 +301,21 @@
                     await continue_for_more_prompt_stmts()
 
                 s = stmt_buffer[0]
 
                 if type(s) is str:
                     prompt += unescape_qstring(s)
                     stmt_buffer = stmt_buffer[1:]
+                    constraints = None
+                    
                     # keep latest prompt in transient state
                     state = state.updated(prompt=prompt)
                 elif type(s) is TemplateVariable:
                     variable = s.name
+                    constraints = constraints_after_last_continue
                     # keep track of number of times a variable with this name has been decoded
                     if variable not in state.recurring_variable_counter.keys():
                         state.recurring_variable_counter[s.name] = -1
                     state.recurring_variable_counter[s.name] += 1
                     
                     stmt_buffer = stmt_buffer[1:]
                     break
@@ -296,21 +332,25 @@
                     await query_head.advance(None)
                     stmt_buffer = stmt_buffer[1:]
                 else:
                     assert False, "prompt interpreter encountered unsupported prompt stmt of type {}: {}".format(type(s), s)
         except InterpretationHeadDone:
             pass
 
-        # merge named tuple with new stmt_buffer
+        program_state = state.program_state.copy()
+        program_state.python_scope = program_variables_after_last_continue or program_state.python_scope
 
+        # merge named tuple with new stmt_buffer
         return state.updated(
             variable=variable,
             prompt=prompt,
+            constraints=constraints,
             stmt_buffer=stmt_buffer,
-            query_head=query_head
+            query_head=query_head,
+            program_state=program_state
         )
 
     def interpreter_state_user_data(self, state: PromptState):
         return {"head": state}
 
     def interpreter_state_from_user_data(self, seq, noroot=False):
         if noroot:
@@ -394,14 +434,15 @@
         trace = None
         logit_mask = None
         
         variable = state.variable
         variable_offset = state.variable_offset
 
         text = ""
+        where = self.where
 
         if is_done:
             mask = tset("eos")
             logit_mask = mask.mask
             stopping_phrases = {"text": [], "tokenized": []}
             follow_trace = None
         elif variable is not None:
@@ -415,74 +456,77 @@
             program_state: ProgramState = state.program_state.copy()
             program_state.set(variable, text, scores=(), diff=diff_text, montonicity="inc")
 
             # follow context
             follow_program_state: ProgramState = state.program_state.copy()
             follow_program_state.set(variable, text + str(ops.NextToken), scores=(), diff=diff_text, montonicity="inc")
 
+            # determine full where condition
+            where = state.full_where_condition(self)
+
             # digest token with where expr
-            valid, is_final, trace, follow_trace = ops.digest(self.where,
+            valid, is_final, trace, follow_trace = ops.digest(where,
                 context=program_state,
                 follow_context=follow_program_state
             )
 
             # obtain where follow map
-            follow_map = follow_trace[self.where] if self.where is not None else None
+            follow_map = follow_trace[where] if where is not None else None
             # print(id(self), self.variable, [text], "mask", follow_map)
             mask = ops.create_mask(follow_map, valid, is_final)
 
             if mask == "*": 
                 logit_mask = None
             else:
                 logit_mask = mask.mask
 
             # check stopping conditions
-            stopping_conditions: List[ops.StopAtOp] = ops.execute_op_stops_at_only(state.variable, self.where, trace)
+            stopping_conditions: List[ops.StopAtOp] = ops.execute_op_stops_at_only(state.variable, where, trace)
             for sc in stopping_conditions:
                 stop_trace = trace.copy()
                 del stop_trace[sc]
                 # check if stopping phrase applies in this step
                 if ops.execute_op(sc, stop_trace, context=program_state, semantics="stop"):
                     # print("apply stop", sc, [text], [diff_text])
                     mask = tset("eos")
                     logit_mask = mask.mask
                     trace[sc] = (sc.stopping_phrase(trace), "stopped")
             stopping_phrases = {
                 "text": [sc.stopping_phrase(trace) for sc in stopping_conditions if type(sc) is ops.StopBeforeOp],
-                "tokenized": [self.tokenizer(sc.stopping_phrase(trace))["input_ids"] for sc in stopping_conditions if type(sc) is ops.StopBeforeOp]
+                "tokenized": [self.tokenizer.tokenize(sc.stopping_phrase(trace), asbytes=True) for sc in stopping_conditions if type(sc) is ops.StopBeforeOp]
             }
 
         else:
             assert False, f"error: where() is called but current variable and current prompt are None and query head has result {state.query_head.result}"
 
-        await self.debugger_output(state, s, valid, is_final, mask, stopping_phrases, program_state, trace, text)
+        await self.debugger_output(state, s, valid, is_final, mask, stopping_phrases, program_state, trace, text, where)
 
         state = state.updated(
                         variable=variable,
                         valid=valid,
                         final=is_final,
                         mask=mask,
                         program_state=program_state,
                         stopping_phrases=stopping_phrases,
-                        where=await self.where_graph_with_trace(trace, follow_trace)
+                        where=await self.where_graph_with_trace(where, trace, follow_trace)
         )
 
         # no mask, no logits processing
         if logit_mask is None:
             return None, None, self.interpreter_state_user_data(state)
         
         # translate boolean mask to logit bias mask
         if len(mask) == 1:
             logit_mask = mask.mask.argmax()
         else:
             logit_mask = np.logical_not(logit_mask) * np.finfo(np.float32).min
         
         return mask, logit_mask, self.interpreter_state_user_data(state)
 
-    async def where_graph_with_trace(self, trace, follow_trace):
+    async def where_graph_with_trace(self, where, trace, follow_trace):
         from lmql.utils.graph import CytoscapeGraphWriter
 
         def node_data(op):
             result = "-"
             follow_map = "-"
             if trace is not None and op in trace:
                 result = trace[op]
@@ -492,21 +536,21 @@
             return {
                 "result": result,
                 "follow_map": follow_map,
                 "repr": repr(op)
             }
 
         writer = CytoscapeGraphWriter(extra_data_provider=node_data)
-        writer.write(self.where)
+        writer.write(where)
 
         return writer.graph.to_json(return_dict=True)
 
-    async def debugger_output(self, state: PromptState, s: dc.DecoderSequence, valid, is_final, mask, stopping_phrases, program_variables, trace, text):
+    async def debugger_output(self, state: PromptState, s: dc.DecoderSequence, valid, is_final, mask, stopping_phrases, program_variables, trace, text, where):
         if self.output_writer is not None:
-           await self.output_writer.add_interpreter_head_state(state.variable, 0, state.prompt + text, self.where, trace, valid, is_final, mask, len(s.input_ids), program_variables)
+           await self.output_writer.add_interpreter_head_state(state.variable, 0, state.prompt + text, where, trace, valid, is_final, mask, len(s.input_ids), program_variables)
 
     async def where_processor(self, seqs, additional_logits_processor_mask, **kwargs):
         zipped_task_inputs = zip(seqs, additional_logits_processor_mask, range(len(seqs)))
         token_mask_tasks = [self.where_for_sequence(s, needs_masking, seqidx, **kwargs) for s,needs_masking, seqidx in zipped_task_inputs]
         results = [(mask, user_data) for mask, user_data in await asyncio.gather(*token_mask_tasks)]
         
         return TokenMask([r[0] for r in results], [r[1] for r in results])
@@ -526,19 +570,22 @@
             
             text = (await seq.text(offset=state.variable_offset, limit=-1, pretty=False))
             text_diff = text[len(await seq.text(state.variable_offset, limit=-2, pretty=False)):]
             
             variable_value = text
             # set raw variable value
             program_state.set(variable, variable_value, scores=(), diff=text_diff, montonicity="fin")
-            
+
+            # get full where condition
+            where = state.full_where_condition(self)
+
             # apply postprocessing, if constraints specify it
             # - variable_value is the postprocessed, converted value (does not have to be a string)
             # - postprocessed_prompt is the string in the prompt that corresponds to the variable value
-            variable_value, postprocessed_prompt = ops.execute_postprocess(self.where, variable, variable_value, context=program_state)
+            variable_value, postprocessed_prompt = ops.execute_postprocess(where, variable, variable_value, context=program_state)
             
             # set postprocessed variable value and program value
             program_state.set(variable, postprocessed_prompt, program_value=variable_value, scores=(), diff="", montonicity="fin")
 
             # current variable is done
             variable = None
             prompt = state.prompt
@@ -575,34 +622,33 @@
                 
                 # value_offset indicates to the decoder, that the first `value_offset` appended tokens are still the value 
                 # of the variable, not deterministic tokens introduced by the prompt program
                 appended_ids = value_ids + program_ids
                 value_offset = state.variable_offset + len(value_ids)
                 
                 combined_new_ids = seq.input_ids[:-n_tokens_to_strip].tolist() + appended_ids
-                variable_offset = len(combined_new_ids)
-
-                rewritten_state = state.updated(variable_offset=variable_offset, variable="__done__" if state.variable is None else state.variable + ":before")
 
+                res = []
+                i = 0
+                while i < len(combined_new_ids):
+                    if type(combined_new_ids[i]) is bytes:
+                        res += [combined_new_ids[i]]
+                        i += 1
+                    else:
+                        j = i+1
+                        while j < len(combined_new_ids) and type(combined_new_ids[j]) is not bytes:
+                            j += 1
+                        r = self.tokenizer.decode_bytes(combined_new_ids[i:j])
+                        res += r
+                        i = j
+                combined_new_ids = np.array(res, dtype=np.bytes_)
 
-                if type(combined_new_ids[0]) is bytes:
-                    res = []
-                    i = 0
-                    while i < len(combined_new_ids):
-                        if type(combined_new_ids[i]) is bytes:
-                            res += [combined_new_ids[i]]
-                            i += 1
-                        else:
-                            j = i+1
-                            while j < len(combined_new_ids) and type(combined_new_ids[j]) is not bytes:
-                                j += 1
-                            r = self.tokenizer.decode_bytes(combined_new_ids[i:j])
-                            res += r
-                            i = j
-                    combined_new_ids = np.array(res, dtype=np.bytes_)
+                variable_offset = len(combined_new_ids)
+                rewritten_state = state.updated(variable_offset=variable_offset, variable="__done__" if state.variable is None else state.variable + ":before")
+                # state = state.updated(variable_offset=variable_offset)
 
                 # appended input ids are now a full replacement for input ids
                 return RewrittenInputIds(
                     appended_input_ids=combined_new_ids, 
                     strip_eos=-n_tokens_to_strip,
                     value_offset=value_offset,
                     user_data=self.interpreter_state_user_data(state),
@@ -654,14 +700,15 @@
             kwargs["input"] = self.input
 
         # prepare initial program state
         context = LMQLContext(self, None)
         query_head = InterpretationHead(fct, context, args, kwargs)
         self.root_state = PromptState(variable=None, prompt="", stmt_buffer=[],
             query_head=query_head, program_state=context.program_state,
+            constraints=None,
             recurring_variable_counter={}, variable_offset=0,
             valid=None, final=None, mask=None, 
             stopping_phrases=None, where=None)
         self.root_state = await self.advance(self.root_state)
 
         # prepare dcmodel
         decoder_args = self.decoder_kwargs
@@ -713,15 +760,20 @@
             set_dclib_debug_printer(self.output_writer)
 
         if _DCLibDebugPrinter.printer is not None:
             if hasattr(_DCLibDebugPrinter.printer, "records_graph"):
                 if _DCLibDebugPrinter.printer.records_graph:
                     dc.set_record_graph()
 
+        # get decoder function
         mode = decoder_args["decoder"].lower()
+        # handle dynamically-set decoding (e.g. set via @lmql.query(decoder="beam", n=2))
+        if mode == "__dynamic__":
+            mode, extra_decoder_args = self.derive_decoder_args(self.extra_kwargs)
+            decoder_args = {**decoder_args, **extra_decoder_args}
         decoder_fct = dc.get_decoder(mode)
         self.validate_args(decoder_args, decoder_fct)
 
         # alias max_length -> max_len
         if "max_length" in decoder_args:
             decoder_args["max_len"] = decoder_args["max_length"]
         if not "max_len" in decoder_args.keys():
@@ -824,18 +876,38 @@
                     results.append(state.query_head.result)
             
             # set decoder step +1, for all stats logging that happens in postprocessing
             self.decoder_step += 1
 
             return results
 
+    def derive_decoder_args(self, extra_kwargs):
+        # default is argmax
+        decoder = extra_kwargs.get("decoder", "argmax")
+        # if temperature is != 0, use 'sample'
+        if extra_kwargs.get("temperature", 0.0) != 0.0:
+            decoder = "sample"
+
+        decoder_fct = dc.get_decoder(decoder)
+        
+        decoder_arg_names = inspect.getfullargspec(decoder_fct).args
+        decoder_kwarg_names = inspect.getfullargspec(decoder_fct).kwonlyargs
+        decoder_args = {}
+
+        for a in decoder_arg_names + decoder_kwarg_names:
+            if a in extra_kwargs.keys():
+                decoder_args[a] = extra_kwargs[a]
+        
+        return decoder, decoder_args
+    
     def validate_args(self, decoder_args, decoder_fct):
-        INTERNAL_ARGS = ["decoder", "dcmodel", "modern_rewriter", "modern_logits_processor", "dclib_additional_logits_processor", "input_id_rewriter", "output_writer", 
-                         "chunk_timeout", "chatty_openai", "distribution_batch_size", "openai_chunksize", "step_budget", "stats", "performance_stats", "cache", 
-                         "show_speculative", "openai_nonstop", "chunksize"]
+        INTERNAL_ARGS = ["decoder", "dcmodel", "modern_rewriter", "modern_logits_processor", "dclib_additional_logits_processor", 
+                         "input_id_rewriter", "output_writer", "chunk_timeout", "chatty_openai", "distribution_batch_size", 
+                         "openai_chunksize", "step_budget", "stats", "performance_stats", "cache", "show_speculative", 
+                         "openai_nonstop", "chunksize"]
 
         # get all arg names and kwarg names of decoder function
         decoder_arg_names = inspect.getfullargspec(decoder_fct).args
         decoder_kwarg_names = inspect.getfullargspec(decoder_fct).kwonlyargs
         for k in decoder_args.keys():
             if k not in decoder_arg_names and k not in decoder_kwarg_names and k not in INTERNAL_ARGS:
                 raise ValueError("Unknown decoder argument: {}".format(k))
```

### Comparing `lmql-0.0.6.4/src/lmql/runtime/langchain.py` & `lmql-0.0.6.5/src/lmql/runtime/langchain.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/runtime/lmql_runtime.py` & `lmql-0.0.6.5/src/lmql/runtime/lmql_runtime.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,16 +32,22 @@
         else:
             if errors == "ignore":
                 return None
             else:
                 raise TypeError("Failed to resolve value of variable '" + name + "' in @lmql.query " + str(self.fct), name)
 
 class EmptyVariableScope:
-    def resolve(self, name):
-        return None
+    def resolve(self, name, errors=None):
+        if name in __builtins__.keys():
+            return __builtins__[name]
+        else:
+            if errors == "ignore":
+                return None
+            else:
+                raise TypeError("Failed to resolve value of variable '" + name + "' in LMQL query")
 
 @dataclass
 class FunctionContext:
     argnames: inspect.Signature
     args_of_query: List[str]
     scope: LMQLInputVariableScope
 
@@ -52,14 +58,17 @@
     postprocessors: List[Any]
     scope: Any
 
     output_writer: Optional[Any] = None
     args: Optional[List[str]] = None
     model: Optional[Any] = None
     function_context: Optional[FunctionContext] = None
+    
+    # extra arguments to consider as query context (e.g. passed to the @lmql.query(<args>) decorator)
+    extra_args: Dict = None
 
     lmql_code: str = None
 
     is_async: bool = True
     
     def __init__(self, fct, output_variables, postprocessors, scope, *args, **kwargs):
         self.fct = fct
@@ -134,14 +143,15 @@
         for name, value in signature.arguments.items():
             if name in args_of_query:
                 compiled_query_args[name] = value
                 captured_variables.remove(name)
 
         failed_to_resolve = []
 
+
         # resolve remaining unset args from scope
         for v in captured_variables:
             if not v in compiled_query_args:
                 try:
                     compiled_query_args[v] = scope.resolve(v, errors="raise")
                 except TypeError:
                     failed_to_resolve.append(v)
@@ -157,18 +167,21 @@
         if not self.is_async:
             return call_sync(self, *args, **kwargs)
 
         return self.__acall__(*args, **kwargs)
 
     async def __acall__(self, *args, **kwargs):
         query_kwargs, runtime_args = self.make_kwargs(*args, **kwargs)
-        interpreter = PromptInterpreter(force_model=self.model)
+        
+        forced_model = self.model or runtime_args.get("model") or (self.extra_args or {}).get("model")
+        interpreter = PromptInterpreter(force_model=forced_model)
 
         if self.output_writer is not None:
             runtime_args["output_writer"] = self.output_writer
+        runtime_args  = {**(self.extra_args or {}), **runtime_args}
         interpreter.set_extra_args(**runtime_args)
 
         # rename 'self'
         if "self" in query_kwargs:
             query_kwargs["__self__"] = query_kwargs.pop("self")
 
         # execute main prompt
@@ -181,14 +194,18 @@
         if self.postprocessors is not None:
             for postprocessor in self.postprocessors:
                 results = await postprocessor.process(results, self.output_writer)
         
         interpreter.print_stats()
         interpreter.dcmodel.close()
 
+        # for lmql.F we assume 'argmax' and unpack the result
+        if "is_f_function" in interpreter.extra_kwargs:
+            results = results[0]
+
         return results
 
     def aschain(self, output_keys=None):
         """
         Returns a LangChain 'Chain' object that can be used to chain multiple queries together.
 
         Args:
```

### Comparing `lmql-0.0.6.4/src/lmql/runtime/loop.py` & `lmql-0.0.6.5/src/lmql/runtime/loop.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 lmql_loop = None
 
 def call_sync(lmql_query_function, *args, **kwargs):
     import asyncio
     global lmql_loop
 
     if lmql_loop is None:
-        lmql_loop = asyncio.new_event_loop()
+        try:
+            lmql_loop = asyncio.get_event_loop()
+        except RuntimeError as e:
+            lmql_loop = asyncio.new_event_loop()
     loop = lmql_loop
     
     asyncio.set_event_loop(loop)
 
     task = lmql_query_function.__acall__(*args, **kwargs)
     error = None
```

### Comparing `lmql-0.0.6.4/src/lmql/runtime/maiohttp.py` & `lmql-0.0.6.5/src/lmql/runtime/maiohttp.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/runtime/masks.py` & `lmql-0.0.6.5/src/lmql/runtime/masks.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/runtime/model_registry.py` & `lmql-0.0.6.5/src/lmql/runtime/model_registry.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,35 @@
-from lmql.models.model import model, LMQLModel
+from lmql.models.model import LMQLModel, inprocess
 import os
 
 model_name_aliases = {
     "chatgpt": "openai/gpt-3.5-turbo",
     "gpt-4": "openai/gpt-4",
 }
 class LMQLModelRegistry: 
     """
     Central registry of models and backends that can be used in LMQL.
     """
     backend_configuration = None
 
     @staticmethod
     def get(model, **kwargs):
+        if model == "<dynamic>":
+            model = LMQLModelRegistry.default_model
+
         if model in model_name_aliases:
             model = model_name_aliases[model]
 
+        if type(model) is LMQLModel:
+            if model.model is not None:
+                return model
+            else:
+                kwargs = {**model.kwargs, **kwargs}
+                model = model.model_identifier
+
         client = LMQLModelRegistry.clients.get(model, None)
 
         if client is None:
             # use resolve to obtain model connection from model identifier
             if model not in LMQLModelRegistry.registry:
                 resolve(model, **kwargs)
 
@@ -41,41 +51,46 @@
         from lmql.runtime.openai_integration import openai_model
 
         # hard-code openai/ namespace to be openai-API-based
         Model = openai_model(model_name[7:], endpoint=endpoint, **kwargs)
         register_model(model_name, Model)
         register_model("*", Model)
     else:
-        try:
-            import transformers
-        except:
-            if "LMQL_BROWSER" in os.environ:
-                assert False, "The browser distribution of LMQL does not support HuggingFace Transformers models.\
-                    Please use openai/ models or install lmql with 'transformers' support (pip install lmql[hf])."
-            else:
-                assert False, "Your distribution of LMQL does not support HuggingFace Transformers models.\
-                    Please use openai/ models or install lmql with 'transformers' support (pip install lmql[hf])."
-
         from lmql.models.lmtp.lmtp_dcmodel import lmtp_model
 
+        # special case for 'random' model (see random_model.py)
+        if model_name == "random":
+            kwargs["tokenizer"] = "gpt2"
+            kwargs["inprocess"] = True
+            kwargs["async_transport"] = True
+
+        # special case for 'llama.cpp'
+        if model_name.startswith("llama.cpp:"):
+            # kwargs["async_transport"] = True
+            kwargs["tokenizer"] = "huggyllama/llama-7b"
+
         # determine endpoint URL
         if endpoint is None:
             endpoint = "localhost:8080"
 
         # determine model name and if we run in-process
         if model_name.startswith("local:"):
             model_name = model_name[6:]
             kwargs["inprocess"] = True
-        
-        Model = lmtp_model(model_name, endpoint=endpoint, **kwargs)
+
+        if kwargs.get("inprocess", False):
+            Model = inprocess(model_name, use_existing_configuration=True, **kwargs).model
+        else:
+            Model = lmtp_model(model_name, endpoint=endpoint, **kwargs)
         
         register_model(model_name, Model)
         return
 
 def register_model(identifier, ModelClass):
     LMQLModelRegistry.registry[identifier] = ModelClass
 
 LMQLModelRegistry.autoconnect = None
 
 LMQLModelRegistry.registry = {}
 # instance of model clients in this process
-LMQLModelRegistry.clients = {}
+LMQLModelRegistry.clients = {}
+LMQLModelRegistry.default_model = "openai/text-davinci-003"
```

### Comparing `lmql-0.0.6.4/src/lmql/runtime/multi_head_interpretation.py` & `lmql-0.0.6.5/src/lmql/runtime/multi_head_interpretation.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/runtime/openai_integration.py` & `lmql-0.0.6.5/src/lmql/runtime/openai_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,19 @@
             print("warning: The OpenAI API has merged {} token(s) server-side, which will reflect in inaccurate 0.0 scores in the decoding tree".format(server_side_swallowed_tokens))
 
         return res
     
     async def score(self, sqs: List[DecoderSequence], tokens: List[List[bytes]], max_batch_size=4, deterministic: Union[bool, List[bool]]=False, stop_phrase=False, needs_rewrite=True, user_data=None, noscore=False, internal=False):
         assert len(sqs) == len(tokens), "Number of sequences and number of tokens to be scored must match, but got {} and {}".format(len(sqs), len(tokens))
 
+        # make sure score erases any openai-continuations
+        if user_data is None:
+            user_data = {}
+        user_data["openai-continuations"] = None
+        
         def make_detseq(s, token_score, completion):
             # compose deterministic flags
             if type(deterministic) is bool:
                 deterministic_flags = np.concatenate([s.deterministic, np.array([deterministic])])
                 next_deterministic = np.array([deterministic] * len(completion[1:]))
             else:
                 assert type(deterministic) is list and len(deterministic) == len(completion), "If deterministic is a list, it must have the same length as the number of tokens to be scored, but is {} and {}".format(deterministic, completion)
@@ -303,15 +308,15 @@
         elif mode == "fixed": # complete with fixed token
             fixed_next_token = completion_call.logit_mask_or_fixed_id # special return value case for prepare function
 
             if fixed_next_token == self.eos:
                 return CompletionResult(openai.response_buffer.singleton(token=fixed_next_token, token_logprob=0), completion_call.continuation_type, completion_call.logit_mask_or_fixed_id)
             else:
                 if noscore: logprob = 0.0
-                else: logprob = (await self.api_score(np.append(input_ids, fixed_next_token, axis=0), len(tokenized_input_ids)))
+                else: logprob = (await self.api_score(np.append(input_ids, nputil.ensure_array(fixed_next_token).reshape(-1), axis=0), -1))
                 return CompletionResult(openai.response_buffer.singleton(token=fixed_next_token, token_logprob=logprob), 
                                         completion_call.continuation_type, completion_call.logit_mask_or_fixed_id)
         else:
             assert False, f"Internal openai API dispatcher returned an unknown completion mode {mode}"
 
         if len(completion_call.stopping_phrases) > 0:
             if len(completion_call.stopping_phrases) > 4:
@@ -324,16 +329,28 @@
         # TODO: we are now overestimate the number of tokens billed to the user since we are not account for stopping phrases for the sake of streaming
         self.count_billed_tokens(len(tokenized_input_ids) + kwargs.get("max_tokens") * batch_size, self.model_identifier)
         
         if self.model_args.get("chatty_openai", False):
             args = kwargs.copy()
             # args["prompt"] = str([await self.detokenize(kwargs["prompt"])])[2:-2]
             print(f"openai complete: {args}", flush=True)
-        
-        return CompletionResult((await openai.async_buffer(await openai.Completion.create(**kwargs), tokenizer=self.tokenize_list))[len(tokenized_input_ids):], completion_call.continuation_type, completion_call.logit_mask_or_fixed_id)
+
+        buffer = (await openai.async_buffer(await openai.Completion.create(**kwargs), tokenizer=self.tokenize_list))
+        t = b""
+        to_skip = b"".join(input_ids)
+
+        # skip echoed prompt prefix (cannot just offset by tokenized_input_ids since server-side the prompt may be tokenized differently)
+        while len(t) < len(to_skip):
+            skipped = await buffer.get(0)
+            skipped = skipped["logprobs"]["tokens"]
+            skipped = b"".join(self.convert([skipped]))
+            t += skipped
+            buffer = buffer[1:]
+
+        return CompletionResult(buffer, completion_call.continuation_type, completion_call.logit_mask_or_fixed_id)
     
     async def tokenize_list(self, tokens: List[str]):
         if len(tokens) > 0 and type(tokens[0]) is str:
             return [[t[0]] for t in await self.model.tokenize(tokens)]
         return tokens
     
     async def openai_cache_delegate(self, kwargs, tokens, scores):
@@ -589,15 +606,15 @@
                 r += [ord(s[i])]
                 i += 1
         return bytes(r)
 
     def convert(self, token):
         result = []
         for t in token:
-            if type(t) is int or (type(t) is np.ndarray and t.dtype != np.str_):
+            if type(t) is int or type(t) is np.int64 or (type(t) is np.ndarray and t.dtype != np.str_):
                 result.append(t)
             elif type(t) is bytes:
                 result.append(t)
             elif t.startswith("bytes:"):
                 result.append(self.frombytes(t[6:]))
             else:
                 result.append(t.encode("utf-8"))
@@ -655,18 +672,15 @@
                 # retroactively apply logits mask to logits
                 mask = completion.logit_mask_or_fixed_id
                 if mask is None: pass
                 elif type(mask) is int: distribution[mask] = np.finfo(np.float32).min
                 else: distribution[mask < 0] = np.finfo(np.float32).min
                 
                 # make sure all token_ids are unique
-                tokens = np.array(list(set(tokens)))
-
-                # re-determine logprobs with logits mask applied
-                logprobs = distribution.score(tokens)
+                tokens, logprobs = distribution.topk(k=k)
 
                 next_token_ids.append(tokens)
                 next_token_scores.append(logprobs)
                 logits.append(distribution)
 
             next_token_ids = [self.convert(t) for t in next_token_ids]
 
@@ -753,18 +767,14 @@
             return all(len(t) >= skip[i] for i,t in enumerate(self.tokens))
 
         # skip as many items as needed to reach the previous token count per sequence
         while not minimum_token_count_reached():
             self.process_next_result(next(self.res))
 
     def process_next_result(self, c):
-        # print("data is", data)
-        # choices = data.choices
-        # assert len(choices) == self.n, f"OpenAI model returned different number of choices than expected: {len(choices)} != {self.n}\n\n {json.dumps(data)}"
-        # index = int(c["index"])
         index = 0
         assert self.n == 1, "ModelOutputBuffer only supports n=1"
         self.tokens[index] += self.text_to_tokens(c.logprobs.tokens)
         self.logprobs[index] += c.logprobs.token_logprobs
         self.response_data[index] += [c] * len(c.logprobs.token_logprobs)
 
     async def advance_stream_iter(self, skip=None):
```

### Comparing `lmql-0.0.6.4/src/lmql/runtime/openai_secret.py` & `lmql-0.0.6.5/src/lmql/runtime/openai_secret.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/runtime/output_writer.py` & `lmql-0.0.6.5/src/lmql/runtime/output_writer.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/runtime/postprocessing/conditional_prob.py` & `lmql-0.0.6.5/src/lmql/runtime/postprocessing/conditional_prob.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/runtime/program_state.py` & `lmql-0.0.6.5/src/lmql/runtime/program_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,17 @@
         self.variable_values = {}
         # postprocessed, converted variable values if not just str (e.g. objects, int)
         self.variable_program_values = {}
         self.variable_diffs = {}
         self.variable_scores = {}
         self.variable_monotonicity = {}
 
+        # python scope of local variables (also user-defined ones)
+        self.python_scope = {}
+
         self.runtime = runtime
 
     async def json(self):
         def json_value(k):
             fin = self.variable_monotonicity.get(k, "var")
             # do not include diff and score for now
             return fin + "(\"" + str(self.variable_values[k]) + "\")"
@@ -48,8 +51,9 @@
         s = ProgramState()
         s.variable_values = self.variable_values.copy()
         s.variable_program_values = self.variable_program_values.copy()
         s.variable_monotonicity = self.variable_monotonicity.copy()
         s.variable_diffs = self.variable_diffs.copy()
         s.variable_scores = self.variable_scores.copy()
         s.runtime = self.runtime
+        s.python_scope = self.python_scope
         return s
```

### Comparing `lmql-0.0.6.4/src/lmql/runtime/stats.py` & `lmql-0.0.6.5/src/lmql/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/runtime/token_distribution.py` & `lmql-0.0.6.5/src/lmql/runtime/token_distribution.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,17 @@
     def __setitem__(self, key, value):
         if type(key) is int:
             key = [key]
             value = [value]
         elif type(key) is str:
             key = [key]
             value = [value]
-        
+        elif type(key) is np.ndarray and key.dtype == np.bool_:
+            key = np.where(key)[0]
+
         key = nputil.ensure_iterable(key)
         value = nputil.ensure_iterable(value)
 
         key, value = self.broadcast(key, value)
 
         for k,v in zip(key, value):
             self.probs[k] = v
@@ -64,10 +66,10 @@
         """
         items = list(self.probs.items())
         keys = [k for k, v in items]
         logprobs = np.array([v for k, v in items])
         
         k = min(k, len(logprobs))
         
-        scores, key_ids = nputil.topk(logprobs, k=k)
+        scores, key_ids = nputil.topk(logprobs, k=k, sorted=True)
 
         return [keys[i] for i in key_ids], scores
```

### Comparing `lmql-0.0.6.4/src/lmql/runtime/tokenizer.py` & `lmql-0.0.6.5/src/lmql/runtime/tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 See .tokenizers for concrete implementations.
 """
 
 import os
 import pickle
 import numpy as np
+from typing import Optional
+
 from lmql.runtime.caching import cache_file_exists, cachefile
 
 from lmql.runtime.tokenizers.pure_python_tokenizer import PythonBackedTokenizer
 from lmql.runtime.tokenizers.tiktoken_tokenizer import TiktokenTokenizer
 from threading import Thread
 
 global special_token_mappings
@@ -57,15 +59,15 @@
     @property
     def vocab_size(self):
         # in LMQL vocab_size is the vocab_range (the highest vocabulary ID + 1)
         # this allows us to use a dense one hot array where no IDs are skipped
         return self.vocab_range
 
     @property
-    def bos_token_id(self):
+    def bos_token_id(self) -> Optional[int]:
         return self.tokenizer_impl.bos_token_id
     
     @property
     def eos_token_id(self):
         return self.tokenizer_impl.eos_token_id
 
     @property
@@ -96,15 +98,15 @@
         result = []
         global reverse_special_token_mappings
         
         for i in input_ids:
             if i in reverse_special_token_mappings.keys():
                 chunk_result = self.tokenizer_impl.decode_tokens_bytes(chunk)
                 result += chunk_result
-                result.append(reverse_special_token_mappings[i].encode("utf-8"))
+                result.append(("<" + reverse_special_token_mappings[i] + "/>").encode("utf-8"))
                 chunk = []
             else:
                 chunk.append(i)
 
         if len(chunk) > 0:
             result += self.tokenizer_impl.decode_tokens_bytes(chunk)
 
@@ -117,16 +119,21 @@
         # TODO: handle special IDs, i.e. tags (only relevant for tag use with LMTP backend)
         return self.tokenizer_impl.convert_token_bytes_to_ids(token_bytes)
 
     def convert_bytes_to_string(self, token_bytes):
         """
         Transforms token bytes into a text.
         """
-        # TODO: handle special IDs, i.e. tags (only relevant for tag use with LMTP backend)
-        return self.tokenizer_impl.convert_bytes_to_string(token_bytes)
+        result = ""
+        for chunk in self.chunk_out_by_special_ids_bytes(token_bytes):
+            if type(chunk) is str:
+                result += chunk
+            else:
+                result += self.tokenizer_impl.convert_bytes_to_string(chunk)
+        return result
 
     def decode(self, input_ids):
         if len(input_ids) > 0 and type(input_ids[0]) is np.bytes_:
             return self.convert_bytes_to_string(input_ids)
 
         s = ""
         for chunk in self.chunk_out_by_special_ids(input_ids):
@@ -184,14 +191,33 @@
                     yield c
                 c = []
                 yield "<" + reverse_special_token_mappings[i] + "/>"
             else:
                 c.append(i)
         yield c
     
+    def chunk_out_by_special_ids_bytes(self, token_bytes, tokenize=True):
+        global reverse_special_token_mappings
+        global special_token_mappings
+        c = []
+        for i in token_bytes:
+            try:
+                decoded = i.decode("utf-8")
+                
+                if decoded.startswith("<") and decoded.endswith("/>") and decoded[1:-2] in special_token_mappings.keys():
+                    if len(c) > 0:
+                        yield c
+                    c = []
+                    yield decoded
+                else:
+                    c.append(i)
+            except:
+                c.append(i)
+        yield c
+    
     def chunk_out_by_tags(self, s, tokenize=True):
         # filter out all special tokens <lmql:.../>
         import re
         segments = []
         offset = 0
         for m in re.finditer(r"<lmql:(.*?)\/>", s):
             segments.append(s[offset:m.start()])
@@ -207,16 +233,16 @@
 def load_tokenizer_notransformers(model_identifier):
     if not "SLOW_TOKENIZER_OK" in os.environ.keys():
         print("warning: using slow python-backed tokenizer as no other tokenizer is available for {} (transformers or tiktoken)".format(model_identifier))
     assert PythonBackedTokenizer.is_available(), "PythonBackedTokenizer not available. Please make sure the 'gpt3_tokenizer' package is installed."
     
     return PythonBackedTokenizer(model_identifier)
 
-def load_tokenizer(model_identifier, type="auto"):
-    cache_identifier = model_identifier.replace("/", "-")
+def load_tokenizer(model_identifier, type="auto", **kwargs):
+    cache_identifier = model_identifier.replace("/", "-").replace(":", "__")
     cache_path = f"tokenizer-{cache_identifier}.pkl"
 
     if type in ["auto", "tiktoken"]:
         tiktoken_available = False
         # for GPT models we force non-HF tokenizers (tiktoken or python-backed)
         try:
             if TiktokenTokenizer.is_available(model_identifier):
@@ -241,24 +267,23 @@
     try:
         assert type in ["auto", "hf"]
 
         def loader():
             import os
             os.environ["TOKENIZERS_PARALLELISM"] = "true"
 
-            import torch
             from lmql.runtime.tokenizers.hf_tokenizer import TransformersTokenizer
 
             assert TransformersTokenizer.is_available(model_identifier), "TransformersTokenizer not available. Please make sure the 'transformers' package is installed."
 
             if cache_file_exists(cache_path):
                 with cachefile(cache_path, "rb") as f:
                     return LMQLTokenizer(pickle.load(f), model_identifier)
             else:
-                t = TransformersTokenizer(model_identifier)
+                t = TransformersTokenizer.from_pretrained(model_identifier, **kwargs)
 
                 with cachefile(cache_path, "wb") as f:
                     pickle.dump(t, f)
             return t
         return LMQLTokenizer(model_identifier, loader=loader)
     except Exception as e:
         # fallback to non-transformers tokenizer
```

### Comparing `lmql-0.0.6.4/src/lmql/runtime/tokenizers/hf_tokenizer.py` & `lmql-0.0.6.5/src/lmql/runtime/tokenizers/tiktoken_tokenizer.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,97 +2,108 @@
 from lmql.runtime.stats import Stats
 
 def unicode(v):
     r = v.decode("utf-8", "ignore")
     assert type(r) is str
     return r
 
-class TransformersTokenizer:
+class TiktokenTokenizer:
     def __init__(self, model_identifier):
-        from transformers import AutoTokenizer
-        
+        import tiktoken
+
         self.model_identifier = model_identifier
-        self.tokenizer = AutoTokenizer.from_pretrained(model_identifier)
+        self.enc = tiktoken.encoding_for_model(model_identifier)
+
+        self.bytes_can_concat = True
+
+        self.vocab = {self.enc.decode([i]): i for i in range(self.enc.max_token_value)}
+        self.stats = Stats("tiktoken")
+
+        for i in range(self.enc.n_vocab, self.enc.max_token_value):
+            token_name = f"<|special_{i}|>"
+            assert token_name not in self.vocab, f"token {token_name} already in vocab"
+            self.vocab[token_name] = i
 
     @staticmethod
     def is_available(model_identifier):
-        """
-        Returns True if this tokenizer implementation is available for the given model identifier.
-        """
         try:
-            from transformers import AutoTokenizer
+            import tiktoken
+            tiktoken.encoding_for_model(model_identifier)
         except ImportError:
             return False
+        except KeyError:
+            return False
         return True
 
     # do not picke self.enc
     def __getstate__(self):
         return {
             "model_identifier": self.model_identifier,
-            "tokenizer": self.tokenizer
+            "vocab": self.vocab
         }
     
     def __setstate__(self, state):
-        from transformers import AutoTokenizer
+        import tiktoken
         
         self.model_identifier = state["model_identifier"]
-        self.tokenizer = state["tokenizer"]
+        self.vocab = state["vocab"]
+        self.enc = tiktoken.encoding_for_model(self.model_identifier)
+        self.stats = Stats("tiktoken")
+
+    def encode(self, text):
+        return self.enc.encode(text, allowed_special={"<|endoftext|>"})
 
     def tokenize(self, text, asbytes=False):
-        """
-        Translates a string into a list of tokens (sub-strings)
-        """
+        ids = self.encode(text)
+        tokens = self.enc.decode_tokens_bytes(ids)
+        
         if asbytes:
-            return self.decode_tokens_bytes(self.tokenizer(text)["input_ids"])
-        return self.tokenizer.tokenize(text)
+            return tokens
+        return [t.decode("raw-unicode-escape", "backslashreplace") for t in tokens]
 
     def decode_tokens_bytes(self, ids):
-        """
-        Converts a list of token ids into a list of token bytes.
-        """
-        # translate 'ids' into a bytes representation
-        return [f"{i}".encode("utf-8") for i in ids]
+        return self.enc.decode_tokens_bytes(ids)
 
     def decode(self, ids, clean_up_tokenization_spaces=True):
-        """
-        Converts a list of token ids into a string.
-        """
-        return self.tokenizer.decode(ids, clean_up_tokenization_spaces=clean_up_tokenization_spaces)
+        return self.enc.decode(ids)
     
     def convert_bytes_to_string(self, token_bytes):
-        """
-        Converts a list of token bytes into a string.
-
-        It must hold that self.convert_bytes_to_string(self.decode_tokens_bytes(ids)) == self.decode(ids).
-        """
-        ids = self.convert_token_bytes_to_ids(token_bytes)
-        return self.tokenizer.decode(ids)
+        return b"".join(token_bytes).decode("utf-8", "replace")
     
     def convert_token_bytes_to_ids(self, tokens):
-        """
-        Converts a list of token bytes into a list of token ids.
-
-        Inverse of self.decode_tokens_bytes.
-        """
-        return [int(t.decode("utf-8")) for t in tokens]
+        text = self.convert_bytes_to_string(tokens)
+        return self.encode(text)
 
     def __call__(self, text_or_list, add_special_tokens=False):
-        return self.tokenizer(text_or_list, add_special_tokens=add_special_tokens)
+        if isinstance(text_or_list, str):
+            input_ids = self.encode(text_or_list)
+        else:
+            input_ids = [self.encode(text) for text in text_or_list]
+
+        return {"input_ids": input_ids}
 
     @property
     def vocab_size(self):
-        return self.tokenizer.vocab_size
+        return self.enc.max_token_value + 1
     
     @property
     def eos_token_id(self):
-        return self.tokenizer.eos_token_id
+        return self.enc.eot_token
 
     @property
     def bos_token_id(self):
-        return self.tokenizer.bos_token_id
+        return self.enc.eot_token
 
     def convert_tokens_to_string(self, tokens):
-        return self.tokenizer.convert_tokens_to_string(tokens)
+        return "".join(tokens)
 
     @property
     def name(self):
-        return "hf-" + self.model_identifier
+        return "tiktoken-" + self.model_identifier
+
+def get_tokenizer(model_identifier):
+    import tiktoken
+
+    if model_identifier.startswith("openai/"):
+        model_identifier = model_identifier[len("openai/"):]
+    
+    return TiktokenTokenizer(model_identifier)
```

### Comparing `lmql-0.0.6.4/src/lmql/runtime/tokenizers/pure_python_tokenizer.py` & `lmql-0.0.6.5/src/lmql/runtime/tokenizers/pure_python_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,18 +38,18 @@
         if asbytes:
             ids = self(s)["input_ids"]
             return self.decode_tokens_bytes(ids)
         else:
             return self._tokenize(s)
 
     def convert_bytes_to_string(self, token_bytes):
-        ids = self.convert_bytes_to_ids(token_bytes)
+        ids = self.convert_token_bytes_to_ids(token_bytes)
         return self.decode(ids)
 
-    def convert_bytes_to_ids(self, token_bytes):
+    def convert_token_bytes_to_ids(self, token_bytes):
         import gpt3_tokenizer
         result = []
         for b in token_bytes:
             if len(b) == 0:
                 continue
             if b == b"<|endoftext|>":
                 result.append(50256)
```

### Comparing `lmql-0.0.6.4/src/lmql/tests/expr_test_utils.py` & `lmql-0.0.6.5/src/lmql/tests/expr_test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,25 +148,25 @@
     loop = asyncio.get_event_loop()
 
     for k in list(g.keys()):
         try:
             if k.startswith("test"): 
                 print("Running", k, "." * (40 - len(k)), end=" ")
                 
-                if type(g[k]) is LMQLQueryFunction:
+                if (type(g[k]) is LMQLQueryFunction or hasattr(g[k], "lmql_code")) and g[k].is_async:
                     loop.run_until_complete(g[k]())
                 elif inspect.iscoroutinefunction(g[k]):
                     loop.run_until_complete(g[k]())
                 else:
                     g[k]()
                 termcolor.cprint("OK", "green")
         except AssertionError as e:
-            print(e)
             num_errors += 1
             termcolor.cprint("FAILED", "red")
+            print(e)
 
     # wait for all tasks to finish
     try:
         for t in asyncio.all_tasks(loop=loop):
             if t.done(): continue
             try:
                 t.cancel()
@@ -177,13 +177,12 @@
     except RuntimeError:
         pass
 
     if num_errors != 0: 
         print(num_errors, "test(s) failed.")
         sys.exit(1)
     else: 
-        print("All tests passed.")
         sys.exit(0)
 
 def enable_show_transformed():
     global show_transformed
     show_transformed =True
```

### Comparing `lmql-0.0.6.4/src/lmql/tests/fin_and.py` & `lmql-0.0.6.5/src/lmql/tests/fin_and.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/tests/local_model_python.py` & `lmql-0.0.6.5/src/lmql/tests/test_local_model_python.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 import lmql
 from lmql.tests.expr_test_utils import run_all_tests
 
-m = lmql.model("facebook/opt-350m", inprocess=True)
+m = lmql.model("gpt2", inprocess=True)
 
 @lmql.query
-async def test_model_reference():
+def test_model_reference():
     '''lmql
     import lmql
 
     argmax(chunk_timeout=10.0)
         """Hello[WHO]"""
     from
         m
     where
         STOPS_AT(WHO, "\n") and len(TOKENS(WHO)) < 10
     '''
 
 @lmql.query
-async def test_local_string():
+def test_local_string():
     '''lmql
     import lmql
 
     argmax(chunk_timeout=10.0)
         """Hello[WHO]"""
     from
-        m
+        "local:gpt2"
     where
         STOPS_AT(WHO, "\n") and len(TOKENS(WHO)) < 10
     '''
 
-m2 = lmql.model("facebook/opt-350m", cuda=True, inprocess=True)
+m2 = lmql.model("gpt2", cuda=True, inprocess=True)
 
 @lmql.query
-async def test_model_reference_cuda():
+def test_model_reference_cuda():
     '''lmql
     import lmql
 
     argmax(chunk_timeout=10.0)
         """Hello[WHO]"""
     from
         m2
     where
         STOPS_AT(WHO, "\n") and len(TOKENS(WHO)) < 10
     '''
 
-run_all_tests(locals())
+if __name__ == "__main__":
+    run_all_tests(locals())
```

### Comparing `lmql-0.0.6.4/src/lmql/tests/outdated/mask_product_test.py` & `lmql-0.0.6.5/src/lmql/tests/outdated/mask_product_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/tests/outdated/monotonicity.py` & `lmql-0.0.6.5/src/lmql/tests/outdated/monotonicity.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/tests/outdated/one_of_tests.py` & `lmql-0.0.6.5/src/lmql/tests/outdated/one_of_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/tests/outdated/sentences_op.py` & `lmql-0.0.6.5/src/lmql/tests/outdated/sentences_op.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/tests/outdated/starts_with_op_test.py` & `lmql-0.0.6.5/src/lmql/tests/outdated/starts_with_op_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/tests/outdated/stops_at.py` & `lmql-0.0.6.5/src/lmql/tests/outdated/stops_at.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/tests/outdated/str_in_str_tests.py` & `lmql-0.0.6.5/src/lmql/tests/outdated/str_in_str_tests.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/tests/outdated/test_multi_head.py` & `lmql-0.0.6.5/src/lmql/tests/outdated/test_multi_head.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/tests/outdated/token_set_test.py` & `lmql-0.0.6.5/src/lmql/tests/outdated/token_set_test.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/tests/queryargs/test_args.py` & `lmql-0.0.6.5/src/lmql/tests/queryargs/test_args.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/tests/queryargs/test_args_query_str.py` & `lmql-0.0.6.5/src/lmql/tests/queryargs/test_args_query_str.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/tests/queryargs/test_args_run.py` & `lmql-0.0.6.5/src/lmql/tests/queryargs/test_args_run.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/tests/queryargs/test_sync.py` & `lmql-0.0.6.5/src/lmql/tests/queryargs/test_sync.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/tests/queryargs/test_var_errors.py` & `lmql-0.0.6.5/src/lmql/tests/queryargs/test_var_errors.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/tests/system/basic_use_cases.py` & `lmql-0.0.6.5/src/lmql/tests/system/basic_use_cases.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/tests/tail_token_set.py` & `lmql-0.0.6.5/src/lmql/tests/tail_token_set.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/tests/test_back2back_caching.py` & `lmql-0.0.6.5/src/lmql/tests/test_back2back_caching.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/tests/test_eq.py` & `lmql-0.0.6.5/src/lmql/tests/test_eq.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,99 +1,112 @@
 import lmql
 from lmql.tests.expr_test_utils import run_all_tests
+from lmql.runtime.tokenizer import load_tokenizer
+
+t = load_tokenizer("gpt2")
+
+def token_diff(s1, s2):
+    ids1 = t(s1)["input_ids"]
+    ids2 = t(s2)["input_ids"]
+    return ids2[len(ids1):]
+
+def tlen(s):
+    return len(t(s)["input_ids"])
 
 async def test_eq_str():
     @lmql.query
     async def q():
         '''lmql
         argmax
             "Q: Hi. A:[OUTPUT]"
         FROM
-            "openai/text-davinci-003"
+            lmql.model("random", seed=123)
         WHERE
             OUTPUT == "Hello you"
         '''
     result = await q()
     assert result[0].variables["OUTPUT"] == "Hello you"
 
 
 async def test_double_eq_str():
     @lmql.query
     async def q():
         '''lmql
         argmax
             "Q: Hi. A:[OUTPUT]"
         FROM
-            "openai/text-davinci-003"
+            lmql.model("random", seed=123)
         WHERE
             OUTPUT == "Hello you" or OUTPUT == "Hello There"
         '''
     result = await q()
     assert result[0].variables["OUTPUT"] in ["Hello you", "Hello There"]
 
 
 async def test_double_eq_int():
     @lmql.query
     async def q():
         '''lmql
         argmax
             "Q: Hi. A:[OUTPUT]"
         FROM
-            "openai/text-davinci-003"
+            lmql.model("random", seed=123)
         WHERE
             len(TOKENS(OUTPUT)) == 2
         '''
     result = await q()
-    assert result[0].prompt == "Q: Hi. A: Hi."
+    ids = token_diff("Q: Hi. A:", result[0].prompt)
+    assert len(ids) == 2
 
 async def test_double_eq_charlen():
     @lmql.query
     async def q():
         '''lmql
         argmax
             "Q: Hi. A:[OUTPUT]"
-        FROM
-            "openai/text-davinci-003"
-        WHERE
+        from
+            lmql.model("random", seed=123)
+        where
             len(OUTPUT) == 2
         '''
     result = await q()
-    assert result[0].prompt == "Q: Hi. A:\n\n"
+    assert len(result[0].variables["OUTPUT"]) == 2
 
 @lmql.query
 async def test_later_var_token_constrained():
     '''lmql
     argmax(max_len=256)
         "A rhyme:\n"
         "Verse: [RHYME_START]\n"
         for i in range(5):
             "Verse: [RHYME]\n"
-            assert RHYME == "\n\nI'm not"
+            assert len(t(RHYME)["input_ids"]) == 5, "RHYME has " + str(len(t(RHYME)["input_ids"])) + " tokens"
     from
-        'openai/text-ada-001'
+        lmql.model("random", seed=123)
     where
         len(TOKENS(RHYME)) == 5 and len(TOKENS(RHYME_START)) == 5
     '''
 
 @lmql.query
 async def test_stops_before_exact_token_len():
     '''lmql
     argmax(max_len=256, openai_chunksize=4)
         "A rhyme named '[NAME]':\n"
         assert not "'" in NAME
         "Verse: [RHYME]\n"
-        assert RHYME == "\n\nAin"
+        assert tlen(RHYME) == 4
         "Verse: [RHYME]\n"
-        assert RHYME == "\n\nAll\n"
+        assert tlen(RHYME) == 4
         "Verse: [RHYME]\n"
-        assert RHYME == "\n\nAll\n"
+        assert tlen(RHYME) == 4
         "Verse: [RHYME]\n"
-        assert RHYME == "\n\nAll\n"
+        assert tlen(RHYME) == 4
         "Verse: [RHYME]\n"
-        assert RHYME == "\n\nAll\n"
+        assert tlen(RHYME) == 4
     from
-        'openai/text-ada-001'
+        lmql.model("random", seed=123)
     where
         len(TOKENS(RHYME)) == 4 and STOPS_BEFORE(NAME, "'")
     '''
 
-run_all_tests(globals())
+if __name__ == "__main__":
+    run_all_tests(globals())
```

### Comparing `lmql-0.0.6.4/src/lmql/tests/test_multibyte_characters.py` & `lmql-0.0.6.5/src/lmql/tests/test_multibyte_characters.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/tests/test_multibyte_local_models.py` & `lmql-0.0.6.5/src/lmql/tests/test_multibyte_local_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,8 +28,9 @@
         assert "π" in formula, "π must occur in the formula"
     from
         m
     where
         len(TOKENS(formula)) < 20
     '''
 
-run_all_tests(globals())
+if __name__ == "__main__":
+    run_all_tests(globals())
```

### Comparing `lmql-0.0.6.4/src/lmql/tests/test_sample_queries.py` & `lmql-0.0.6.5/src/lmql/tests/test_sample_queries.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/tests/test_scoping.py` & `lmql-0.0.6.5/src/lmql/tests/test_scoping.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 import lmql
 from lmql.tests.expr_test_utils import run_all_tests
 
 
 @lmql.query
-async def test_q():
+async def test_q(actual_input: str = None):
     '''lmql
     a = 12
 
     def f(): return 12
 
     class A: pass
 
     argmax
         "Q: Hi {actual_input} {a}{f}{A}"
         for id in ['A', 'a', 'f']:
             assert locals().get(id) is None and globals().get(id) is not None, f"Global identifier {id} in local scope, or not in global scope. locals: {locals()}"
         assert "actual_input" in locals().keys(), f"Input variable actual_input not in local scope. locals: {locals()}"
         assert "actual_input" not in globals().keys(), f"Input variable actual_input not in global scope. locals: {locals()}"
     from 
-        "openai/text-ada-001" 
-    where
-        len(TOKENS(WHO)) < 10
+        "openai/text-ada-001"
     '''
 
 async def test_decode_clause_scoping():
     await lmql.run('''lmql
     argmax(n=n)
         "Q: Hi {n}. A: [WHO]"
         assert "n" in locals().keys(), f"Input variable n not captured by scope"
```

### Comparing `lmql-0.0.6.4/src/lmql/tests/test_stopping.py` & `lmql-0.0.6.5/src/lmql/tests/test_stopping.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,27 +107,28 @@
     '''
 
 @lmql.query
 async def test_stop_should_not_postprocess_if_sc_not_satisfied():
     '''lmql
     argmax 
         "A good movie review:[REVIEW] "
-        assert REVIEW.endswith("sad"), "Expected REVIEW to end with sad, but was " + str([REVIEW])
+        assert REVIEW.endswith("smiles"), "Expected REVIEW to end with 'smiles', but was " + str([REVIEW])
     from 
-        "openai/text-ada-001" 
+        lmql.model("random", seed=123)
     where
-        len(TOKENS(REVIEW)) > 10 and STOPS_AT(REVIEW, "sad") and STOPS_AT(REVIEW, "Fault")
+        len(TOKENS(REVIEW)) > 10 and STOPS_AT(REVIEW, "exempted") and STOPS_AT(REVIEW, "smiles")
     '''
 
 @lmql.query
 async def test_stop_before_should_not_postprocess_if_sc_not_satisfied():
     '''lmql
     argmax 
         "A good movie review:[REVIEW] "
-        assert REVIEW.endswith("sad"), "Expected REVIEW to end with sad, but was " + str([REVIEW])
+        assert REVIEW.endswith("smiles"), "Expected REVIEW to end with 'smiles', but was " + str([REVIEW])
     from 
-        "openai/text-ada-001" 
+        lmql.model("random", seed=123)
     where
-        len(TOKENS(REVIEW)) > 10 and STOPS_AT(REVIEW, "sad") and STOPS_BEFORE(REVIEW, "Fault")
+        len(TOKENS(REVIEW)) > 10 and STOPS_BEFORE(REVIEW, "exempted") and STOPS_AT(REVIEW, "smiles")
     '''
 
-run_all_tests(globals())
+if __name__ == "__main__":
+    run_all_tests(globals())
```

### Comparing `lmql-0.0.6.4/src/lmql/tests/tiktoken_tsets.py` & `lmql-0.0.6.5/src/lmql/tests/tiktoken_tsets.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/live/live.js` & `lmql-0.0.6.5/src/lmql/ui/live/live.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/live/live.py` & `lmql-0.0.6.5/src/lmql/ui/live/live.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,21 +61,26 @@
             "code": code
         })
 
 @live()
 async def lmql(code, *args, web=False):
     import lmql
     
+    model = None
+    if len(args) > 0 and type(args[0]) is dict:
+        model = args[0].get("model")
+        if model == "automatic": model = None
+
     if code.startswith("./"):
         with open(code) as f:
             code = f.read()
 
     output_writer = LiveDebuggerOutputWriter(web=web)
 
-    result = await lmql.run(code, output_writer=output_writer)
+    result = await lmql.run(code, output_writer=output_writer, model=model)
 
     for r in (result if type(result) is list else [result]):
         if r is None:
             continue
 
         if type(r) is not lmql.LMQLResult:
             continue
```

### Comparing `lmql-0.0.6.4/src/lmql/ui/live/livelib.py` & `lmql-0.0.6.5/src/lmql/ui/live/livelib.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/live/yarn.lock` & `lmql-0.0.6.5/src/lmql/ui/live/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/README.md` & `lmql-0.0.6.5/src/lmql/ui/playground/README.md`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/package.json` & `lmql-0.0.6.5/src/lmql/ui/playground/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/public/favicon.ico` & `lmql-0.0.6.5/src/lmql/ui/playground/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/public/index.html` & `lmql-0.0.6.5/src/lmql/ui/playground/public/index.html`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/public/lmql.svg` & `lmql-0.0.6.5/src/lmql/ui/playground/public/lmql.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/calc.json` & `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/calc.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/chat.json` & `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/chat.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/cot.json` & `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/cot.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'lmql-editor-contents'": "'# zero-shot cot according to "*

 * *                           'https://arxiv.org/pdf/2205.11916.pdf\\nargmax\\n   """Q: It was Sept. '*

 * *                           '1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\n   '*

 * *                           'Answer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) '*

 * *                           "08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\n   A: Let\\'s think step by "*

 * *                           'step."""\\n   "[REASONING]\ […]*

```diff
@@ -1,4 +1,4 @@
 {
     "decoder-graph": "{\"nodes\":[{\"id\":\"n0\",\"seq_id\":\"s_0\",\"text\":[\"<|endoftext|>Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\\\nA: Let's think step by step.\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\"],\"root\":true,\"logprob\":\"0\",\"logprobs\":[0,0,0,0,0],\"logprobs_det\":[0,0,0,0,0],\"logprobs_norm\":[],\"seqlogprob\":\"0\",\"score_det\":\"0.0\",\"score_nor\":\"0.0\",\"score_tot\":0,\"pool\":null,\"user_data\":{\"head\":{\"head_index\":0,\"variable\":\"REASONING[0]\",\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"13\",\"deterministic_5\":[true,true,true,true,true],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n1\",\"seq_id\":\"s_1\",\"text\":[\"\\\\n\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\"],\"root\":false,\"logprob\":-1.486771,\"logprobs\":[0,0,0,0,-1.486771],\"logprobs_det\":[0,0,0,0],\"logprobs_norm\":[-1.486771],\"seqlogprob\":-1.486771,\"score_det\":\"0.0\",\"score_nor\":-1.486771,\"score_tot\":-1.486771,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=100 tokens_left\u226531 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"198\",\"deterministic_5\":[true,true,true,true,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n2\",\"seq_id\":\"s_2\",\"text\":[\"\\\\n\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\n\"],\"root\":false,\"logprob\":-0.546809,\"logprobs\":[0,0,0,-1.486771,-0.546809],\"logprobs_det\":[0,0,0],\"logprobs_norm\":[-1.486771,-0.546809],\"seqlogprob\":-2.03358,\"score_det\":\"0.0\",\"score_nor\":-1.2518153280449775,\"score_tot\":-1.2518153280449775,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=101 tokens_left\u226530 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\n\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\n\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"198\",\"deterministic_5\":[true,true,true,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n3\",\"seq_id\":\"s_3\",\"text\":[\"Sept\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept\"],\"root\":false,\"logprob\":-1.0818186,\"logprobs\":[0,0,-1.486771,-0.546809,-1.0818186],\"logprobs_det\":[0,0],\"logprobs_norm\":[-1.486771,-0.546809,-1.0818186],\"seqlogprob\":-3.1153986000000002,\"score_det\":\"0.0\",\"score_nor\":-1.4438721582191152,\"score_tot\":-1.4438721582191152,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=102 tokens_left\u226529 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"14635\",\"deterministic_5\":[true,true,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n4\",\"seq_id\":\"s_4\",\"text\":[\".\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept.\"],\"root\":false,\"logprob\":-0.12604097,\"logprobs\":[0,-1.486771,-0.546809,-1.0818186,-0.12604097],\"logprobs_det\":[0],\"logprobs_norm\":[-1.486771,-0.546809,-1.0818186,-0.12604097],\"seqlogprob\":-3.2414395700000003,\"score_det\":\"0.0\",\"score_nor\":-1.2282759138978354,\"score_tot\":-1.2282759138978354,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=103 tokens_left\u226528 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept.\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept.\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"13\",\"deterministic_5\":[true,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n5\",\"seq_id\":\"s_5\",\"text\":[\" 1\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1\"],\"root\":false,\"logprob\":-0.0014816872,\"logprobs\":[-1.486771,-0.546809,-1.0818186,-0.12604097,-0.0014816872],\"logprobs_det\":[],\"logprobs_norm\":[-1.486771,-0.546809,-1.0818186,-0.12604097,-0.0014816872],\"seqlogprob\":-3.2429212572000004,\"score_det\":\"0.0\",\"score_nor\":-1.0511323456072736,\"score_tot\":-1.0511323456072736,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=104 tokens_left\u226527 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"352\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n6\",\"seq_id\":\"s_6\",\"text\":[\"st\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st\"],\"root\":false,\"logprob\":-0.030104088,\"logprobs\":[-0.546809,-1.0818186,-0.12604097,-0.0014816872,-0.030104088],\"logprobs_det\":[],\"logprobs_norm\":[-0.546809,-1.0818186,-0.12604097,-0.0014816872,-0.030104088],\"seqlogprob\":-3.2730253452,\"score_det\":\"0.0\",\"score_nor\":-0.9337776891662345,\"score_tot\":-0.9337776891662345,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=105 tokens_left\u226526 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"301\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n7\",\"seq_id\":\"s_7\",\"text\":[\",\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st,\"],\"root\":false,\"logprob\":-0.37463278,\"logprobs\":[-1.0818186,-0.12604097,-0.0014816872,-0.030104088,-0.37463278],\"logprobs_det\":[],\"logprobs_norm\":[-1.0818186,-0.12604097,-0.0014816872,-0.030104088,-0.37463278],\"seqlogprob\":-3.6476581252000004,\"score_det\":\"0.0\",\"score_nor\":-0.9342121247952457,\"score_tot\":-0.9342121247952457,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=106 tokens_left\u226525 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st,\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st,\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"11\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n8\",\"seq_id\":\"s_8\",\"text\":[\" 2021\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021\"],\"root\":false,\"logprob\":-0.00019750134,\"logprobs\":[-0.12604097,-0.0014816872,-0.030104088,-0.37463278,-0.00019750134],\"logprobs_det\":[],\"logprobs_norm\":[-0.12604097,-0.0014816872,-0.030104088,-0.37463278,-0.00019750134],\"seqlogprob\":-3.6478556265400006,\"score_det\":\"0.0\",\"score_nor\":-0.8508924119812478,\"score_tot\":-0.8508924119812478,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=107 tokens_left\u226524 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"33448\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n9\",\"seq_id\":\"s_9\",\"text\":[\" was\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was\"],\"root\":false,\"logprob\":-0.19758251,\"logprobs\":[-0.0014816872,-0.030104088,-0.37463278,-0.00019750134,-0.19758251],\"logprobs_det\":[],\"logprobs_norm\":[-0.0014816872,-0.030104088,-0.37463278,-0.00019750134,-0.19758251],\"seqlogprob\":-3.8454381365400008,\"score_det\":\"0.0\",\"score_nor\":-0.8259924400505539,\"score_tot\":-0.8259924400505539,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=108 tokens_left\u226523 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"373\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n10\",\"seq_id\":\"s_10\",\"text\":[\" a\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a\"],\"root\":false,\"logprob\":-0.15417615,\"logprobs\":[-0.030104088,-0.37463278,-0.00019750134,-0.19758251,-0.15417615],\"logprobs_det\":[],\"logprobs_norm\":[-0.030104088,-0.37463278,-0.00019750134,-0.19758251,-0.15417615],\"seqlogprob\":-3.999614286540001,\"score_det\":\"0.0\",\"score_nor\":-0.7980279660344407,\"score_tot\":-0.7980279660344407,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=109 tokens_left\u226522 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"257\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n11\",\"seq_id\":\"s_11\",\"text\":[\" week\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week\"],\"root\":false,\"logprob\":-0.00020072184,\"logprobs\":[-0.37463278,-0.00019750134,-0.19758251,-0.15417615,-0.00020072184],\"logprobs_det\":[],\"logprobs_norm\":[-0.37463278,-0.00019750134,-0.19758251,-0.15417615,-0.00020072184],\"seqlogprob\":-3.999815008380001,\"score_det\":\"0.0\",\"score_nor\":-0.7465605310549213,\"score_tot\":-0.7465605310549213,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=110 tokens_left\u226521 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"1285\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n12\",\"seq_id\":\"s_12\",\"text\":[\" ago\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago\"],\"root\":false,\"logprob\":-0.0003033258,\"logprobs\":[-0.00019750134,-0.19758251,-0.15417615,-0.00020072184,-0.0003033258],\"logprobs_det\":[],\"logprobs_norm\":[-0.00019750134,-0.19758251,-0.15417615,-0.00020072184,-0.0003033258],\"seqlogprob\":-4.000118334180001,\"score_det\":\"0.0\",\"score_nor\":-0.7024994149230782,\"score_tot\":-0.7024994149230782,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=111 tokens_left\u226520 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"2084\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n13\",\"seq_id\":\"s_13\",\"text\":[\",\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago,\"],\"root\":false,\"logprob\":-0.43836734,\"logprobs\":[-0.19758251,-0.15417615,-0.00020072184,-0.0003033258,-0.43836734],\"logprobs_det\":[],\"logprobs_norm\":[-0.19758251,-0.15417615,-0.00020072184,-0.0003033258,-0.43836734],\"seqlogprob\":-4.438485674180001,\"score_det\":\"0.0\",\"score_nor\":-0.7370118587675974,\"score_tot\":-0.7370118587675974,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=112 tokens_left\u226519 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago,\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago,\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"11\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n14\",\"seq_id\":\"s_14\",\"text\":[\" so\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so\"],\"root\":false,\"logprob\":-0.4010986,\"logprobs\":[-0.15417615,-0.00020072184,-0.0003033258,-0.43836734,-0.4010986],\"logprobs_det\":[],\"logprobs_norm\":[-0.15417615,-0.00020072184,-0.0003033258,-0.43836734,-0.4010986],\"seqlogprob\":-4.839584274180001,\"score_det\":\"0.0\",\"score_nor\":-0.7629892724800564,\"score_tot\":-0.7629892724800564,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=113 tokens_left\u226518 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"523\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n15\",\"seq_id\":\"s_15\",\"text\":[\" 10\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10\"],\"root\":false,\"logprob\":-0.2789501,\"logprobs\":[-0.00020072184,-0.0003033258,-0.43836734,-0.4010986,-0.2789501],\"logprobs_det\":[],\"logprobs_norm\":[-0.00020072184,-0.0003033258,-0.43836734,-0.4010986,-0.2789501],\"seqlogprob\":-5.118534374180001,\"score_det\":\"0.0\",\"score_nor\":-0.768921036778274,\"score_tot\":-0.768921036778274,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=114 tokens_left\u226517 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"838\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n16\",\"seq_id\":\"s_16\",\"text\":[\" days\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days\"],\"root\":false,\"logprob\":-0.00007231626,\"logprobs\":[-0.0003033258,-0.43836734,-0.4010986,-0.2789501,-0.00007231626],\"logprobs_det\":[],\"logprobs_norm\":[-0.0003033258,-0.43836734,-0.4010986,-0.2789501,-0.00007231626],\"seqlogprob\":-5.118606690440001,\"score_det\":\"0.0\",\"score_nor\":-0.7349668856481557,\"score_tot\":-0.7349668856481557,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=115 tokens_left\u226516 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"1528\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n17\",\"seq_id\":\"s_17\",\"text\":[\" ago\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago\"],\"root\":false,\"logprob\":-0.030898329,\"logprobs\":[-0.43836734,-0.4010986,-0.2789501,-0.00007231626,-0.030898329],\"logprobs_det\":[],\"logprobs_norm\":[-0.43836734,-0.4010986,-0.2789501,-0.00007231626,-0.030898329],\"seqlogprob\":-5.149505019440001,\"score_det\":\"0.0\",\"score_nor\":-0.708681736790406,\"score_tot\":-0.708681736790406,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=116 tokens_left\u226515 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"2084\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n18\",\"seq_id\":\"s_18\",\"text\":[\" would\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would\"],\"root\":false,\"logprob\":-0.30163112,\"logprobs\":[-0.4010986,-0.2789501,-0.00007231626,-0.030898329,-0.30163112],\"logprobs_det\":[],\"logprobs_norm\":[-0.4010986,-0.2789501,-0.00007231626,-0.030898329,-0.30163112],\"seqlogprob\":-5.451136139440001,\"score_det\":\"0.0\",\"score_nor\":-0.7207692910149671,\"score_tot\":-0.7207692910149671,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=117 tokens_left\u226514 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"561\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n19\",\"seq_id\":\"s_19\",\"text\":[\" be\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be\"],\"root\":false,\"logprob\":-0.110199064,\"logprobs\":[-0.2789501,-0.00007231626,-0.030898329,-0.30163112,-0.110199064],\"logprobs_det\":[],\"logprobs_norm\":[-0.2789501,-0.00007231626,-0.030898329,-0.30163112,-0.110199064],\"seqlogprob\":-5.5613352034400005,\"score_det\":\"0.0\",\"score_nor\":-0.7080298242841601,\"score_tot\":-0.7080298242841601,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=118 tokens_left\u226513 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"307\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n20\",\"seq_id\":\"s_20\",\"text\":[\" 8\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8\"],\"root\":false,\"logprob\":-0.58483523,\"logprobs\":[-0.00007231626,-0.030898329,-0.30163112,-0.110199064,-0.58483523],\"logprobs_det\":[],\"logprobs_norm\":[-0.00007231626,-0.030898329,-0.30163112,-0.110199064,-0.58483523],\"seqlogprob\":-6.146170433440001,\"score_det\":\"0.0\",\"score_nor\":-0.7548898779635244,\"score_tot\":-0.7548898779635244,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=119 tokens_left\u226512 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"807\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n21\",\"seq_id\":\"s_21\",\"text\":[\" days\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days\"],\"root\":false,\"logprob\":-0.005031326,\"logprobs\":[-0.030898329,-0.30163112,-0.110199064,-0.58483523,-0.005031326],\"logprobs_det\":[],\"logprobs_norm\":[-0.030898329,-0.30163112,-0.110199064,-0.58483523,-0.005031326],\"seqlogprob\":-6.15120175944,\"score_det\":\"0.0\",\"score_nor\":-0.7301405452444888,\"score_tot\":-0.7301405452444888,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=120 tokens_left\u226511 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"1528\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n22\",\"seq_id\":\"s_22\",\"text\":[\" before\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before\"],\"root\":false,\"logprob\":-0.2860951,\"logprobs\":[-0.30163112,-0.110199064,-0.58483523,-0.005031326,-0.2860951],\"logprobs_det\":[],\"logprobs_norm\":[-0.30163112,-0.110199064,-0.58483523,-0.005031326,-0.2860951],\"seqlogprob\":-6.43729685944,\"score_det\":\"0.0\",\"score_nor\":-0.739618321446627,\"score_tot\":-0.739618321446627,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=121 tokens_left\u226510 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"878\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n23\",\"seq_id\":\"s_23\",\"text\":[\" that\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that\"],\"root\":false,\"logprob\":-0.16659938,\"logprobs\":[-0.110199064,-0.58483523,-0.005031326,-0.2860951,-0.16659938],\"logprobs_det\":[],\"logprobs_norm\":[-0.110199064,-0.58483523,-0.005031326,-0.2860951,-0.16659938],\"seqlogprob\":-6.60389623944,\"score_det\":\"0.0\",\"score_nor\":-0.7355136818614856,\"score_tot\":-0.7355136818614856,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=122 tokens_left\u22659 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"326\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n24\",\"seq_id\":\"s_24\",\"text\":[\",\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that,\"],\"root\":false,\"logprob\":-0.61369115,\"logprobs\":[-0.58483523,-0.005031326,-0.2860951,-0.16659938,-0.61369115],\"logprobs_det\":[],\"logprobs_norm\":[-0.58483523,-0.005031326,-0.2860951,-0.16659938,-0.61369115],\"seqlogprob\":-7.21758738944,\"score_det\":\"0.0\",\"score_nor\":-0.7802686927218565,\"score_tot\":-0.7802686927218565,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=123 tokens_left\u22658 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that,\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that,\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"11\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n25\",\"seq_id\":\"s_25\",\"text\":[\" which\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which\"],\"root\":false,\"logprob\":-0.6257873,\"logprobs\":[-0.005031326,-0.2860951,-0.16659938,-0.61369115,-0.6257873],\"logprobs_det\":[],\"logprobs_norm\":[-0.005031326,-0.2860951,-0.16659938,-0.61369115,-0.6257873],\"seqlogprob\":-7.84337468944,\"score_det\":\"0.0\",\"score_nor\":-0.824033668086837,\"score_tot\":-0.824033668086837,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=124 tokens_left\u22657 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"543\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n26\",\"seq_id\":\"s_26\",\"text\":[\" is\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is\"],\"root\":false,\"logprob\":-0.89486104,\"logprobs\":[-0.2860951,-0.16659938,-0.61369115,-0.6257873,-0.89486104],\"logprobs_det\":[],\"logprobs_norm\":[-0.2860951,-0.16659938,-0.61369115,-0.6257873,-0.89486104],\"seqlogprob\":-8.73823572944,\"score_det\":\"0.0\",\"score_nor\":-0.893187039825983,\"score_tot\":-0.893187039825983,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=125 tokens_left\u22656 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"318\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n27\",\"seq_id\":\"s_27\",\"text\":[\" August\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August\"],\"root\":false,\"logprob\":-0.32124403,\"logprobs\":[-0.16659938,-0.61369115,-0.6257873,-0.89486104,-0.32124403],\"logprobs_det\":[],\"logprobs_norm\":[-0.16659938,-0.61369115,-0.6257873,-0.89486104,-0.32124403],\"seqlogprob\":-9.05947975944,\"score_det\":\"0.0\",\"score_nor\":-0.9018797258029358,\"score_tot\":-0.9018797258029358,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=126 tokens_left\u22655 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"2932\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n28\",\"seq_id\":\"s_28\",\"text\":[\" 23\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23\"],\"root\":false,\"logprob\":-0.091041826,\"logprobs\":[-0.61369115,-0.6257873,-0.89486104,-0.32124403,-0.091041826],\"logprobs_det\":[],\"logprobs_norm\":[-0.61369115,-0.6257873,-0.89486104,-0.32124403,-0.091041826],\"seqlogprob\":-9.15052158544,\"score_det\":\"0.0\",\"score_nor\":-0.8880455204048348,\"score_tot\":-0.8880455204048348,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=127 tokens_left\u22654 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"2242\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n29\",\"seq_id\":\"s_29\",\"text\":[\"rd\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd\"],\"root\":false,\"logprob\":-0.029552825,\"logprobs\":[-0.6257873,-0.89486104,-0.32124403,-0.091041826,-0.029552825],\"logprobs_det\":[],\"logprobs_norm\":[-0.6257873,-0.89486104,-0.32124403,-0.091041826,-0.029552825],\"seqlogprob\":-9.18007441044,\"score_det\":\"0.0\",\"score_nor\":-0.8692958432073266,\"score_tot\":-0.8692958432073266,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=128 tokens_left\u22653 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"4372\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n30\",\"seq_id\":\"s_30\",\"text\":[\",\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd,\"],\"root\":false,\"logprob\":-0.12553144,\"logprobs\":[-0.89486104,-0.32124403,-0.091041826,-0.029552825,-0.12553144],\"logprobs_det\":[],\"logprobs_norm\":[-0.89486104,-0.32124403,-0.091041826,-0.029552825,-0.12553144],\"seqlogprob\":-9.30560585044,\"score_det\":\"0.0\",\"score_nor\":-0.8605176355644039,\"score_tot\":-0.8605176355644039,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=129 tokens_left\u22652 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd,\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd,\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"11\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n31\",\"seq_id\":\"s_31\",\"text\":[\" 2021\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021\"],\"root\":false,\"logprob\":-0.00021348093,\"logprobs\":[-0.32124403,-0.091041826,-0.029552825,-0.12553144,-0.00021348093],\"logprobs_det\":[],\"logprobs_norm\":[-0.32124403,-0.091041826,-0.029552825,-0.12553144,-0.00021348093],\"seqlogprob\":-9.30581933137,\"score_det\":\"0.0\",\"score_nor\":-0.8410105250921117,\"score_tot\":-0.8410105250921117,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=130 tokens_left\u22651 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"33448\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n32\",\"seq_id\":\"s_32\",\"text\":[\".\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\"],\"root\":false,\"logprob\":-0.016921155,\"logprobs\":[-0.091041826,-0.029552825,-0.12553144,-0.00021348093,-0.016921155],\"logprobs_det\":[],\"logprobs_norm\":[-0.091041826,-0.029552825,-0.12553144,-0.00021348093,-0.016921155],\"seqlogprob\":-9.32274048637,\"score_det\":\"0.0\",\"score_nor\":-0.8240216271443249,\"score_tot\":-0.8240216271443249,\"pool\":null,\"user_data\":{\"openai-continuations\":{},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"13\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n33\",\"seq_id\":\"s_33\",\"text\":[\"\\\\n\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\"],\"root\":false,\"logprob\":-0.9252133,\"logprobs\":[-0.029552825,-0.12553144,-0.00021348093,-0.016921155,-0.9252133],\"logprobs_det\":[],\"logprobs_norm\":[-0.029552825,-0.12553144,-0.00021348093,-0.016921155,-0.9252133],\"seqlogprob\":-10.24795378637,\"score_det\":\"0.0\",\"score_nor\":-0.8864972655939624,\"score_tot\":-0.8864972655939624,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=132 tokens_left\u226517 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"198\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n34\",\"seq_id\":\"s_34\",\"text\":[\"\\\\n\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\n\"],\"root\":false,\"logprob\":-0.046842318,\"logprobs\":[-0.12553144,-0.00021348093,-0.016921155,-0.9252133,-0.046842318],\"logprobs_det\":[],\"logprobs_norm\":[-0.12553144,-0.00021348093,-0.016921155,-0.9252133,-0.046842318],\"seqlogprob\":-10.294796104369999,\"score_det\":\"0.0\",\"score_nor\":-0.8721325739750563,\"score_tot\":-0.8721325739750563,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=133 tokens_left\u226516 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\n\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\n\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"198\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n35\",\"seq_id\":\"s_35\",\"text\":[\"Therefore\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore\"],\"root\":false,\"logprob\":-0.43705934,\"logprobs\":[-0.00021348093,-0.016921155,-0.9252133,-0.046842318,-0.43705934],\"logprobs_det\":[],\"logprobs_norm\":[-0.00021348093,-0.016921155,-0.9252133,-0.046842318,-0.43705934],\"seqlogprob\":-10.731855444369998,\"score_det\":\"0.0\",\"score_nor\":-0.8908963572033478,\"score_tot\":-0.8908963572033478,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=134 tokens_left\u226515 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"26583\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n36\",\"seq_id\":\"s_36\",\"text\":[\",\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore,\"],\"root\":false,\"logprob\":-0.023194522,\"logprobs\":[-0.016921155,-0.9252133,-0.046842318,-0.43705934,-0.023194522],\"logprobs_det\":[],\"logprobs_norm\":[-0.016921155,-0.9252133,-0.046842318,-0.43705934,-0.023194522],\"seqlogprob\":-10.755049966369999,\"score_det\":\"0.0\",\"score_nor\":-0.8753881873345057,\"score_tot\":-0.8753881873345057,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=135 tokens_left\u226514 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore,\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore,\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"11\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n37\",\"seq_id\":\"s_37\",\"text\":[\" the\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the\"],\"root\":false,\"logprob\":-0.0028921051,\"logprobs\":[-0.9252133,-0.046842318,-0.43705934,-0.023194522,-0.0028921051],\"logprobs_det\":[],\"logprobs_norm\":[-0.9252133,-0.046842318,-0.43705934,-0.023194522,-0.0028921051],\"seqlogprob\":-10.75794207147,\"score_det\":\"0.0\",\"score_nor\":-0.8589897756331534,\"score_tot\":-0.8589897756331534,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=136 tokens_left\u226513 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"262\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n38\",\"seq_id\":\"s_38\",\"text\":[\" answer\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer\"],\"root\":false,\"logprob\":-0.5872189,\"logprobs\":[-0.046842318,-0.43705934,-0.023194522,-0.0028921051,-0.5872189],\"logprobs_det\":[],\"logprobs_norm\":[-0.046842318,-0.43705934,-0.023194522,-0.0028921051,-0.5872189],\"seqlogprob\":-11.34516097147,\"score_det\":\"0.0\",\"score_nor\":-0.8891236138641484,\"score_tot\":-0.8891236138641484,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=137 tokens_left\u226512 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"3280\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n39\",\"seq_id\":\"s_39\",\"text\":[\" is\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is\"],\"root\":false,\"logprob\":-0.02803042,\"logprobs\":[-0.43705934,-0.023194522,-0.0028921051,-0.5872189,-0.02803042],\"logprobs_det\":[],\"logprobs_norm\":[-0.43705934,-0.023194522,-0.0028921051,-0.5872189,-0.02803042],\"seqlogprob\":-11.37319139147,\"score_det\":\"0.0\",\"score_nor\":-0.875260083375643,\"score_tot\":-0.875260083375643,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=138 tokens_left\u226511 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"318\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n40\",\"seq_id\":\"s_40\",\"text\":[\" (\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (\"],\"root\":false,\"logprob\":-0.19375733,\"logprobs\":[-0.023194522,-0.0028921051,-0.5872189,-0.02803042,-0.19375733],\"logprobs_det\":[],\"logprobs_norm\":[-0.023194522,-0.0028921051,-0.5872189,-0.02803042,-0.19375733],\"seqlogprob\":-11.56694872147,\"score_det\":\"0.0\",\"score_nor\":-0.8745342371463354,\"score_tot\":-0.8745342371463354,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=139 tokens_left\u226510 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"357\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n41\",\"seq_id\":\"s_41\",\"text\":[\"A\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A\"],\"root\":false,\"logprob\":-0.3978184,\"logprobs\":[-0.0028921051,-0.5872189,-0.02803042,-0.19375733,-0.3978184],\"logprobs_det\":[],\"logprobs_norm\":[-0.0028921051,-0.5872189,-0.02803042,-0.19375733,-0.3978184],\"seqlogprob\":-11.96476712147,\"score_det\":\"0.0\",\"score_nor\":-0.8891101135885072,\"score_tot\":-0.8891101135885072,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=140 tokens_left\u22659 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"32\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n42\",\"seq_id\":\"s_42\",\"text\":[\")\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A)\"],\"root\":false,\"logprob\":-0.038968075,\"logprobs\":[-0.5872189,-0.02803042,-0.19375733,-0.3978184,-0.038968075],\"logprobs_det\":[],\"logprobs_norm\":[-0.5872189,-0.02803042,-0.19375733,-0.3978184,-0.038968075],\"seqlogprob\":-12.00373519647,\"score_det\":\"0.0\",\"score_nor\":-0.8770854428514203,\"score_tot\":-0.8770854428514203,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=141 tokens_left\u22658 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A)\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A)\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"8\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n43\",\"seq_id\":\"s_43\",\"text\":[\" 08\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08\"],\"root\":false,\"logprob\":-0.0010216809,\"logprobs\":[-0.02803042,-0.19375733,-0.3978184,-0.038968075,-0.0010216809],\"logprobs_det\":[],\"logprobs_norm\":[-0.02803042,-0.19375733,-0.3978184,-0.038968075,-0.0010216809],\"seqlogprob\":-12.00475687737,\"score_det\":\"0.0\",\"score_nor\":-0.8628304238728832,\"score_tot\":-0.8628304238728832,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=142 tokens_left\u22657 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"8487\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n44\",\"seq_id\":\"s_44\",\"text\":[\"/\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/\"],\"root\":false,\"logprob\":-0.000001022884,\"logprobs\":[-0.19375733,-0.3978184,-0.038968075,-0.0010216809,-0.000001022884],\"logprobs_det\":[],\"logprobs_norm\":[-0.19375733,-0.3978184,-0.038968075,-0.0010216809,-0.000001022884],\"seqlogprob\":-12.004757900253999,\"score_det\":\"0.0\",\"score_nor\":-0.8490563855090045,\"score_tot\":-0.8490563855090045,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=143 tokens_left\u22656 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"14\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n45\",\"seq_id\":\"s_45\",\"text\":[\"23\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23\"],\"root\":false,\"logprob\":-0.0067903185,\"logprobs\":[-0.3978184,-0.038968075,-0.0010216809,-0.000001022884,-0.0067903185],\"logprobs_det\":[],\"logprobs_norm\":[-0.3978184,-0.038968075,-0.0010216809,-0.000001022884,-0.0067903185],\"seqlogprob\":-12.011548218754001,\"score_det\":\"0.0\",\"score_nor\":-0.83627714786517,\"score_tot\":-0.83627714786517,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=144 tokens_left\u22655 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"1954\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n46\",\"seq_id\":\"s_46\",\"text\":[\"/\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/\"],\"root\":false,\"logprob\":-0.0000013823812,\"logprobs\":[-0.038968075,-0.0010216809,-0.000001022884,-0.0067903185,-0.0000013823812],\"logprobs_det\":[],\"logprobs_norm\":[-0.038968075,-0.0010216809,-0.000001022884,-0.0067903185,-0.0000013823812],\"seqlogprob\":-12.0115496011352,\"score_det\":\"0.0\",\"score_nor\":-0.8235093924804957,\"score_tot\":-0.8235093924804957,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=145 tokens_left\u22654 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"14\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n47\",\"seq_id\":\"s_47\",\"text\":[\"20\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/20\"],\"root\":false,\"logprob\":-0.000004721163,\"logprobs\":[-0.0010216809,-0.000001022884,-0.0067903185,-0.0000013823812,-0.000004721163],\"logprobs_det\":[],\"logprobs_norm\":[-0.0010216809,-0.000001022884,-0.0067903185,-0.0000013823812,-0.000004721163],\"seqlogprob\":-12.0115543222982,\"score_det\":\"0.0\",\"score_nor\":-0.8112051687193574,\"score_tot\":-0.8112051687193574,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=146 tokens_left\u22653 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/20\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/20\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"1238\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n48\",\"seq_id\":\"s_48\",\"text\":[\"21\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021\"],\"root\":false,\"logprob\":-0.0000018601542,\"logprobs\":[-0.000001022884,-0.0067903185,-0.0000013823812,-0.000004721163,-0.0000018601542],\"logprobs_det\":[],\"logprobs_norm\":[-0.000001022884,-0.0067903185,-0.0000013823812,-0.000004721163,-0.0000018601542],\"seqlogprob\":-12.0115561824524,\"score_det\":\"0.0\",\"score_nor\":-0.799337910343471,\"score_tot\":-0.799337910343471,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=147 tokens_left\u22652 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"2481\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n49\",\"seq_id\":\"s_49\",\"text\":[\".\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\"],\"root\":false,\"logprob\":-0.13062377,\"logprobs\":[-0.0067903185,-0.0000013823812,-0.000004721163,-0.0000018601542,-0.13062377],\"logprobs_det\":[],\"logprobs_norm\":[-0.0067903185,-0.0000013823812,-0.000004721163,-0.0000018601542,-0.13062377],\"seqlogprob\":-12.1421799524524,\"score_det\":\"0.0\",\"score_nor\":-0.7964516365649502,\"score_tot\":-0.7964516365649502,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=148 tokens_left\u22651 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"REASONING[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\",\"num_variables_decoded\":0,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"13\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n50\",\"seq_id\":\"s_50\",\"text\":[\"<|endoftext|>\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.<|endoftext|>\"],\"root\":false,\"logprob\":-0.00015779921,\"logprobs\":[-0.0000013823812,-0.000004721163,-0.0000018601542,-0.13062377,-0.00015779921],\"logprobs_det\":[],\"logprobs_norm\":[-0.0000013823812,-0.000004721163,-0.0000018601542,-0.13062377,-0.00015779921],\"seqlogprob\":-12.1423377516624,\"score_det\":\"0.0\",\"score_nor\":-0.7852777746983867,\"score_tot\":-0.7852777746983867,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-*\":\"CompletionResult(buffer=<response_buffer_slice lower=149 tokens_left\u22650 >, continuation_type='temp-0-logprobs-5-*', logit_mask_or_fixed_id=None)\"},\"head\":{\"variable\":\"RESULT[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\",\"num_variables_decoded\":1,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"rewrite\"},\"token_id\":\"50256\",\"deterministic_5\":[false,false,false,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n51\",\"seq_id\":\"s_51\",\"text\":[\"\\\\n\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\n\"],\"root\":false,\"logprob\":-12.089864730834961,\"seqlogprob\":-24.232044683287363,\"pool\":null,\"deterministic\":true,\"next_ids\":[26583,11,1871,317,832,376,11,262,3280,318],\"next_logprobs\":[-13.974494934082031,-0.08850023150444031,-12.91045093536377,-8.747084617614746,-7.016685485839844,-0.002760721603408456,-0.08455567061901093,-0.1204521507024765,-1.2680811882019043,-0.07165201008319855],\"user_data\":{\"openai-continuations\":{},\"head\":{\"variable\":\"RESULT[0]\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\"},\"mask\":\"*\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\",\"num_variables_decoded\":1,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"198\",\"deterministic_5\":[false,false,false,false,true],\"stop_phrase_5\":[false,false,false,false,false],\"score_det\":-12.089864730834961,\"score_nor\":-0.7964516365649502,\"score_tot\":-12.88631636739991,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n52\",\"seq_id\":\"s_52\",\"text\":[\"Therefore\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\nTherefore\"],\"root\":false,\"logprob\":-13.974494934082031,\"seqlogprob\":-38.206539617369394,\"pool\":null,\"deterministic\":true,\"next_ids\":[11,1871,317,832,376,11,262,3280,318],\"next_logprobs\":[-0.08850023150444031,-12.91045093536377,-8.747084617614746,-7.016685485839844,-0.002760721603408456,-0.08455567061901093,-0.1204521507024765,-1.2680811882019043,-0.07165201008319855],\"user_data\":{\"openai-continuations\":{},\"head\":{\"variable\":\"RESULT[0]:before(9)\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\"},\"mask\":\"{token_id=11}\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\",\"num_variables_decoded\":1,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"26583\",\"deterministic_5\":[false,false,false,true,true],\"stop_phrase_5\":[false,false,false,false,false],\"score_det\":-16.044495394437565,\"score_nor\":-0.7964516365649502,\"score_tot\":-16.840947031002514,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n53\",\"seq_id\":\"s_53\",\"text\":[\",\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\nTherefore,\"],\"root\":false,\"logprob\":-0.08850023150444031,\"seqlogprob\":-38.295039848873834,\"pool\":null,\"deterministic\":true,\"next_ids\":[1871,317,832,376,11,262,3280,318],\"next_logprobs\":[-12.91045093536377,-8.747084617614746,-7.016685485839844,-0.002760721603408456,-0.08455567061901093,-0.1204521507024765,-1.2680811882019043,-0.07165201008319855],\"user_data\":{\"openai-continuations\":{},\"head\":{\"variable\":\"RESULT[0]:before(8)\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\"},\"mask\":\"{token_id=1871}\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\",\"num_variables_decoded\":1,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"11\",\"deterministic_5\":[false,false,true,true,true],\"stop_phrase_5\":[false,false,false,false,false],\"score_det\":-12.120884390924537,\"score_nor\":-0.7964516365649502,\"score_tot\":-12.917336027489487,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n54\",\"seq_id\":\"s_54\",\"text\":[\" among\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\nTherefore, among\"],\"root\":false,\"logprob\":-12.91045093536377,\"seqlogprob\":-51.205490784237604,\"pool\":null,\"deterministic\":true,\"next_ids\":[317,832,376,11,262,3280,318],\"next_logprobs\":[-8.747084617614746,-7.016685485839844,-0.002760721603408456,-0.08455567061901093,-0.1204521507024765,-1.2680811882019043,-0.07165201008319855],\"user_data\":{\"openai-continuations\":{},\"head\":{\"variable\":\"RESULT[0]:before(7)\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\"},\"mask\":\"{token_id=317}\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\",\"num_variables_decoded\":1,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"1871\",\"deterministic_5\":[false,true,true,true,true],\"stop_phrase_5\":[false,false,false,false,false],\"score_det\":-14.80222684262048,\"score_nor\":-0.7964516365649502,\"score_tot\":-15.598678479185429,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n55\",\"seq_id\":\"s_55\",\"text\":[\" A\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\nTherefore, among A\"],\"root\":false,\"logprob\":-8.747084617614746,\"seqlogprob\":-59.95257540185235,\"pool\":null,\"deterministic\":true,\"next_ids\":[832,376,11,262,3280,318],\"next_logprobs\":[-7.016685485839844,-0.002760721603408456,-0.08455567061901093,-0.1204521507024765,-1.2680811882019043,-0.07165201008319855],\"user_data\":{\"openai-continuations\":{},\"head\":{\"variable\":\"RESULT[0]:before(6)\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\"},\"mask\":\"{token_id=832}\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\",\"num_variables_decoded\":1,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"317\",\"deterministic_5\":[true,true,true,true,true],\"stop_phrase_5\":[false,false,false,false,false],\"score_det\":-15.496846555111935,\"score_nor\":-0.7964516365649502,\"score_tot\":-16.293298191676886,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n56\",\"seq_id\":\"s_56\",\"text\":[\" through\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\nTherefore, among A through\"],\"root\":false,\"logprob\":-7.016685485839844,\"seqlogprob\":-66.9692608876922,\"pool\":null,\"deterministic\":true,\"next_ids\":[376,11,262,3280,318],\"next_logprobs\":[-0.002760721603408456,-0.08455567061901093,-0.1204521507024765,-1.2680811882019043,-0.07165201008319855],\"user_data\":{\"openai-continuations\":{},\"head\":{\"variable\":\"RESULT[0]:before(5)\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\"},\"mask\":\"{token_id=376}\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\",\"num_variables_decoded\":1,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"832\",\"deterministic_5\":[true,true,true,true,true],\"stop_phrase_5\":[false,false,false,false,false],\"score_det\":-15.64189077072666,\"score_nor\":-0.7964516365649502,\"score_tot\":-16.43834240729161,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n57\",\"seq_id\":\"s_57\",\"text\":[\" F\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\nTherefore, among A through F\"],\"root\":false,\"logprob\":-0.002760721603408456,\"seqlogprob\":-66.97202160929561,\"pool\":null,\"deterministic\":true,\"next_ids\":[11,262,3280,318],\"next_logprobs\":[-0.08455567061901093,-0.1204521507024765,-1.2680811882019043,-0.07165201008319855],\"user_data\":{\"openai-continuations\":{},\"head\":{\"variable\":\"RESULT[0]:before(4)\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\"},\"mask\":\"{token_id=11}\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\",\"num_variables_decoded\":1,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"376\",\"deterministic_5\":[true,true,true,true,true],\"stop_phrase_5\":[false,false,false,false,false],\"score_det\":-14.042627109857735,\"score_nor\":-0.7964516365649502,\"score_tot\":-14.839078746422684,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n58\",\"seq_id\":\"s_58\",\"text\":[\",\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\nTherefore, among A through F,\"],\"root\":false,\"logprob\":-0.08455567061901093,\"seqlogprob\":-67.05657727991462,\"pool\":null,\"deterministic\":true,\"next_ids\":[262,3280,318],\"next_logprobs\":[-0.1204521507024765,-1.2680811882019043,-0.07165201008319855],\"user_data\":{\"openai-continuations\":{},\"head\":{\"variable\":\"RESULT[0]:before(3)\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\"},\"mask\":\"{token_id=262}\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\",\"num_variables_decoded\":1,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"11\",\"deterministic_5\":[true,true,true,true,true],\"stop_phrase_5\":[false,false,false,false,false],\"score_det\":-12.809236104220732,\"score_nor\":-0.7964516365649502,\"score_tot\":-13.605687740785681,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n59\",\"seq_id\":\"s_59\",\"text\":[\" the\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\nTherefore, among A through F, the\"],\"root\":false,\"logprob\":-0.1204521507024765,\"seqlogprob\":-67.1770294306171,\"pool\":null,\"deterministic\":true,\"next_ids\":[3280,318],\"next_logprobs\":[-1.2680811882019043,-0.07165201008319855],\"user_data\":{\"openai-continuations\":{},\"head\":{\"variable\":\"RESULT[0]:before(2)\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\"},\"mask\":\"{token_id=3280}\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\",\"num_variables_decoded\":1,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"262\",\"deterministic_5\":[true,true,true,true,true],\"stop_phrase_5\":[false,false,false,false,false],\"score_det\":-11.821375872967797,\"score_nor\":-0.7964516365649502,\"score_tot\":-12.617827509532747,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n60\",\"seq_id\":\"s_60\",\"text\":[\" answer\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\nTherefore, among A through F, the answer\"],\"root\":false,\"logprob\":-1.2680811882019043,\"seqlogprob\":-68.445110618819,\"pool\":null,\"deterministic\":true,\"next_ids\":[318],\"next_logprobs\":[-0.07165201008319855],\"user_data\":{\"openai-continuations\":{},\"head\":{\"variable\":\"RESULT[0]:before(1)\",\"head_index\":0,\"valid\":\"None\",\"final\":\"var\",\"program_state\":{\"REASONING\":\"inc(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\"},\"mask\":\"{token_id=318}\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\",\"num_variables_decoded\":1,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"None\",\"var\"],\"follow_map\":\"* -> var(None)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"3280\",\"deterministic_5\":[true,true,true,true,true],\"stop_phrase_5\":[false,false,false,false,false],\"score_det\":-11.233911578090694,\"score_nor\":-0.7964516365649502,\"score_tot\":-12.030363214655644,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n61\",\"seq_id\":\"s_61\",\"text\":[\" is\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\nTherefore, among A through F, the answer is\"],\"root\":false,\"logprob\":-0.07165201008319855,\"seqlogprob\":-68.5167626289022,\"pool\":null,\"deterministic\":true,\"next_ids\":[],\"next_logprobs\":[],\"user_data\":{\"openai-continuations\":{},\"head\":{\"variable\":\"RESULT[0]\",\"head_index\":0,\"valid\":true,\"final\":\"var\",\"program_state\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"inc(\\\"\\\")\"},\"mask\":\"{, , , , , }\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\nTherefore, among A through F, the answer is\",\"num_variables_decoded\":1,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[true,\"var\"],\"follow_map\":\"* \\\\ {, , , , , } -> fin(False) and {, , , , , } -> var(True)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"\",\"inc\"],\"follow_map\":\"{eos} -> fin() and * \\\\ {eos} -> inc(<lmql.next>)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"318\",\"deterministic_5\":[true,true,true,true,true],\"stop_phrase_5\":[false,false,false,false,false],\"score_det\":-10.522246227076375,\"score_nor\":-0.7964516365649502,\"score_tot\":-11.318697863641324,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n62\",\"seq_id\":\"s_62\",\"text\":[\"A\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\nTherefore, among A through F, the answer isA\"],\"root\":false,\"logprob\":-0.00116059,\"logprobs\":[-0.08455567061901093,-0.1204521507024765,-1.2680811882019043,-0.07165201008319855,-0.00116059],\"logprobs_det\":[-0.08455567061901093,-0.1204521507024765,-1.2680811882019043,-0.07165201008319855],\"logprobs_norm\":[-0.00116059],\"seqlogprob\":-68.51792321890218,\"score_det\":-10.522246227076375,\"score_nor\":-0.7853426278869706,\"score_tot\":-11.307588854963345,\"pool\":null,\"user_data\":{\"openai-continuations\":{\"temp-0-logprobs-5-32=100-33=100-34=100-35=100-36=100-37=100\":\"CompletionResult(buffer=<response_buffer_slice lower=160 tokens_left\u22650 >, continuation_type='temp-0-logprobs-5-32=100-33=100-34=100-35=100-36=100-37=100', logit_mask_or_fixed_id=array([-3.4028235e+38, -3.4028235e+38, -3.4028235e+38, ...,\\n       -3.4028235e+38, -3.4028235e+38, -3.4028235e+38], dtype=float32))\"},\"head\":{\"variable\":\"RESULT[0]\",\"head_index\":0,\"valid\":true,\"final\":\"var\",\"program_state\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"inc(\\\"A\\\")\"},\"mask\":\"{eos}\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\nTherefore, among A through F, the answer isA\",\"num_variables_decoded\":1,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[true,\"var\"],\"follow_map\":\"{eos} -> fin(True) and * \\\\ {eos} -> fin(False)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"A\",\"inc\"],\"follow_map\":\"{eos} -> fin(A) and * \\\\ {eos} -> inc(A<lmql.next>)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"where\"},\"token_id\":\"32\",\"deterministic_5\":[true,true,true,true,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]},{\"id\":\"n63\",\"seq_id\":\"s_63\",\"text\":[\"<|endoftext|>\"],\"seqtext\":[\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\nTherefore, among A through F, the answer isA<|endoftext|>\"],\"root\":false,\"logprob\":0,\"logprobs\":[-0.1204521507024765,-1.2680811882019043,-0.07165201008319855,-0.00116059,0],\"logprobs_det\":[-0.1204521507024765,-1.2680811882019043,-0.07165201008319855],\"logprobs_norm\":[-0.00116059,0],\"seqlogprob\":-68.51792321890218,\"score_det\":-10.522246227076375,\"score_nor\":-0.7745314393273911,\"score_tot\":-11.296777666403766,\"pool\":null,\"user_data\":{\"head\":{\"variable\":\"__done__\",\"head_index\":0,\"valid\":true,\"final\":\"var\",\"program_state\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"inc(\\\"A\\\")\"},\"mask\":\"{eos}\",\"stopping_phrases\":{\"tokenized\":[],\"text\":[]},\"full_text\":\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\\nAnswer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\\nA: Let's think step by step.\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\nTherefore, among A through F, the answer isA\",\"num_variables_decoded\":2,\"where\":{\"nodes\":[{\"data\":{\"id\":\"n0\",\"label\":\"InOp\",\"is_token\":0,\"result\":[true,\"var\"],\"follow_map\":\"{eos} -> fin(True) and * \\\\ {eos} -> fin(False)\",\"repr\":\"<InOp>\"}},{\"data\":{\"id\":\"n1\",\"label\":\"<class 'lmql.ops.ops.Var'>\",\"is_token\":0,\"result\":[\"A\",\"inc\"],\"follow_map\":\"{eos} -> fin(A) and * \\\\ {eos} -> inc(A<lmql.next>)\",\"repr\":\"<Var RESULT>\"}}],\"edges\":[{\"data\":{\"source\":\"n1\",\"target\":\"n0\"}}]},\"program_variables\":{\"REASONING\":\"fin(\\\"\\n\\nSept. 1st, 2021 was a week ago, so 10 days ago would be 8 days before that, which is August 23rd, 2021.\\n\\nTherefore, the answer is (A) 08/23/2021.\\\")\",\"RESULT\":\"fin(\\\"A\\\")\"}},\"set_by\":\"rewrite\"},\"token_id\":\"50256\",\"deterministic_5\":[true,true,true,false,false],\"stop_phrase_5\":[false,false,false,false,false],\"prompt_len\":99,\"sticky_user_data_keys\":[\"head.variable\"]}],\"edges\":[[\"n0\",\"n1\"],[\"n1\",\"n2\"],[\"n2\",\"n3\"],[\"n3\",\"n4\"],[\"n4\",\"n5\"],[\"n5\",\"n6\"],[\"n6\",\"n7\"],[\"n7\",\"n8\"],[\"n8\",\"n9\"],[\"n9\",\"n10\"],[\"n10\",\"n11\"],[\"n11\",\"n12\"],[\"n12\",\"n13\"],[\"n13\",\"n14\"],[\"n14\",\"n15\"],[\"n15\",\"n16\"],[\"n16\",\"n17\"],[\"n17\",\"n18\"],[\"n18\",\"n19\"],[\"n19\",\"n20\"],[\"n20\",\"n21\"],[\"n21\",\"n22\"],[\"n22\",\"n23\"],[\"n23\",\"n24\"],[\"n24\",\"n25\"],[\"n25\",\"n26\"],[\"n26\",\"n27\"],[\"n27\",\"n28\"],[\"n28\",\"n29\"],[\"n29\",\"n30\"],[\"n30\",\"n31\"],[\"n31\",\"n32\"],[\"n32\",\"n33\"],[\"n33\",\"n34\"],[\"n34\",\"n35\"],[\"n35\",\"n36\"],[\"n36\",\"n37\"],[\"n37\",\"n38\"],[\"n38\",\"n39\"],[\"n39\",\"n40\"],[\"n40\",\"n41\"],[\"n41\",\"n42\"],[\"n42\",\"n43\"],[\"n43\",\"n44\"],[\"n44\",\"n45\"],[\"n45\",\"n46\"],[\"n46\",\"n47\"],[\"n47\",\"n48\"],[\"n48\",\"n49\"],[\"n49\",\"n50\"],[\"n49\",\"n51\"],[\"n51\",\"n52\"],[\"n52\",\"n53\"],[\"n53\",\"n54\"],[\"n54\",\"n55\"],[\"n55\",\"n56\"],[\"n56\",\"n57\"],[\"n57\",\"n58\"],[\"n58\",\"n59\"],[\"n59\",\"n60\"],[\"n60\",\"n61\"],[\"n61\",\"n62\"],[\"n62\",\"n63\"]]}",
-    "lmql-editor-contents": "# zero-shot cot according to https://arxiv.org/pdf/2205.11916.pdf\nargmax\n   \"\"\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\n   Answer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\n   A: Let's think step by step.\"\"\"\n   \"[REASONING]\\n\"\n   \"Therefore, among A through F, the answer is[RESULT]\"\n   assert RESULT == \"A\"\nfrom\n   \"openai/text-davinci-003\"\nwhere\n   RESULT in [\"A\", \"B\", \"C\", \"D\", \"E\", \"F\"]"
+    "lmql-editor-contents": "# zero-shot cot according to https://arxiv.org/pdf/2205.11916.pdf\nargmax\n   \"\"\"Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?\n   Answer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021\n   A: Let's think step by step.\"\"\"\n   \"[REASONING]\\n\"\n   \"Therefore, among A through F, the answer is[RESULT]\"\n   \nfrom\n   \"openai/text-davinci-003\"\nwhere\n   RESULT in [\"A\", \"B\", \"C\", \"D\", \"E\", \"F\"]"
 }
```

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/distribution.json` & `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/distribution.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/hello.json` & `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/hello.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/joke.json` & `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/joke.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/kv.json` & `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/kv.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/list.json` & `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/list.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/meta.json` & `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/meta.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/translation.json` & `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/translation.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/public/precomputed/wiki.json` & `lmql-0.0.6.5/src/lmql/ui/playground/public/precomputed/wiki.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/public/snippets/dynamic-cfg.json` & `lmql-0.0.6.5/src/lmql/ui/playground/public/snippets/dynamic-cfg.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/public/snippets/json-parsing.json` & `lmql-0.0.6.5/src/lmql/ui/playground/public/snippets/json-parsing.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/App.jsx` & `lmql-0.0.6.5/src/lmql/ui/playground/src/App.jsx`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import './graph-layout.css';
 
 import styled from 'styled-components';
 import Editor from "@monaco-editor/react";
 import React, { useEffect, useRef, useState } from "react";
 import { registerLmqlLanguage } from "./editor/lmql-monaco-language";
-import { BsSquare, BsFillExclamationSquareFill, BsBoxArrowUpRight, BsArrowRightCircle, BsFillCameraFill, BsCheckSquare, BsSendFill, BsFileArrowDownFill, BsKeyFill, BsTerminal, BsFileCode, BsGithub, BsCardList, BsFullscreen, BsXCircle, BsFillChatLeftTextFill, BsGear, BsGridFill } from 'react-icons/bs';
+import { BsSquare, BsFillExclamationSquareFill, BsBoxArrowUpRight, BsArrowRightCircle, BsFillCameraFill, BsCheckSquare, BsSendFill, 
+  BsFileArrowDownFill, BsKeyFill, BsTerminal, BsFileCode, BsGithub, BsCardList, BsFullscreen, BsXCircle, BsFillChatLeftTextFill, 
+  BsGear, BsGridFill, BsPlus } from 'react-icons/bs';
 import { DecoderGraph } from './DecoderGraph';
 import { BUILD_INFO } from './build_info';
 import exploreIcon from "./explore.svg"
 import { ExploreState, Explore, PromptPopup, Dialog } from './Explore'
 import { CodeScreenshot } from "./CodeScreenshot";
 import { errorState, persistedState, trackingState, displayState} from "./State"
 import { configuration, LMQLProcess, isLocalMode} from './Configuration';
@@ -28,15 +30,15 @@
 const ResizeObservers = {
   addResizeListener: l => ResizeObservers.listeners.push(l),
   removeResizeListener: l => ResizeObservers.listeners = ResizeObservers.listeners.filter(x => x !== l),
   listeners: [],
   notify: () => ResizeObservers.listeners.forEach(l => l()),
 }
 
-const bg = '#1e1e1e';
+const bg = '#252526';
 
 const ContentContainer = styled.div`
   /* width: 900pt; */
   display: flex;
   flex-direction: column;
   justify-content: flex-start;
   
@@ -387,14 +389,235 @@
 //     />
 //     </PlotContainer>
 //   } else {
 //     return <CenterBox style={props.style}><h2>No Statistics Available</h2></CenterBox>
 //   }
 // }
 
+const ModelSelectionDiv = styled.div`
+  flex: 1;
+  position: absolute;
+  background-color: transparent;
+  margin: 2pt;
+  text-align: right;
+  top: 0pt;
+  right: 0pt;
+  height: 18pt;
+  width: 40%;
+
+  &:hover {
+    border-bottom: 1pt solid grey;
+  }
+
+  &:active {
+    text-decoration: underline;
+  }
+
+  &.auto {
+    opacity: 0.2
+  }
+
+  &.auto:hover, &.auto:active {
+    opacity: 1.0
+  }
+
+  >input {
+    position: absolute;
+    top: 0;
+    left: 0;
+    right: 0;
+    bottom: 0;
+    border: none;
+    outline: none;
+    background-color: #ffffff19;
+    background: none;
+    text-align: right;
+    z-index: 990;
+    display: block;
+  }
+
+  .select {
+    position: absolute;
+    flex-direction: column;
+    top: calc(100% + 5pt);
+    bottom: auto;
+    width: 100%;
+    color: black;
+    background-color: white;
+    border-radius: 4pt;
+    text-align: left;
+    max-height: 300pt;
+    max-height: calc(100vh - 100pt);
+    overflow-y: scroll;
+    display: none;
+    z-index: 999;
+    padding-bottom: 10pt;
+  }
+
+  .select.open {
+    display: flex;
+  }
+
+  .select .option:hover {
+    background-color: #f0f0f0aa;
+    cursor: pointer;
+  }
+
+  .select .option:first-child {
+    border-top: none;
+  }
+
+  .select .option {
+    text-align: left;
+    padding: 4pt;
+    font-family: monospace;
+    margin: 0pt 0pt;
+    border-radius: 2pt;
+    border-top: 0.5pt solid #d6d6d6;
+    font-size: 8pt;
+    display: flex;
+    flex-direction: row;
+  }
+
+  .option .note {
+    text-align: right;
+    display: block;
+    flex: 1;
+    font-size: 6pt;
+    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
+    line-height: 10pt;
+  }
+
+  .select h2 {
+    font-size: 8pt;
+    margin: 8pt 4pt;
+    font-weight: normal;
+    padding: 0;
+  }
+
+  .select .instructions {
+    display: block;
+    font-size: 8pt;
+    padding: 5pt;
+    color: #3c3c3c;
+  }
+
+  .option:hover.selected, .option.selected {
+    background-color: #c4c4c4;
+  }
+  
+  >input {
+    z-index: 3;
+    right: 20pt;
+    font-size: 8pt;
+    color: #ffffffae;
+    padding-left: 5pt;
+    font-family: monospace;
+    z-index: 999;
+    border-radius: 2pt;
+  }
+
+  &.active input, input:focus {
+    background-color: #ffffff3c !important;
+  }
+
+  .select h2:first-of-type {
+    font-weight: bold !important;
+  }
+
+  svg {
+    position: absolute;
+    top: 3.5pt;
+    height: 10pt;
+    width: 10pt;
+    right: 7pt;
+    z-index: 1;
+    opacity: 0.4;
+  }
+
+  .overlay {
+    background-color: black;
+    width: 100vw;
+    height: 100vh;
+    position: fixed;
+    top: 0;
+    left: 0;
+    opacity: 0.3;
+    z-index: 20;
+  }
+`
+
+function ModelSelection() {
+  const [model, setModel] = useState(persistedState.getItem("playground-model"))
+  const [selectOpen, setSelectOpen] = useState(false)
+
+  const onChange = (value) => {
+    persistedState.setItem("playground-model", value)
+    setModel(value)
+  }
+
+  const PREDEFINED = {
+    "": [
+      {"name": "automatic", note: "Use model as specified by the query.", inprocess: false},
+      {"name": "random", note: "Random (uniform) token sampling.", inprocess: false}
+    ],
+    "Other Suggestions": [
+      {"name": "openai/text-ada-001", "note": "OpenAI", inprocess: false},
+      {"name": "openai/text-curie-001", "note": "OpenAI", inprocess: false},
+      {"name": "openai/text-babbage-001", "note": "OpenAI", inprocess: false},
+      {"name": "openai/text-davinci-001", "note": "OpenAI", inprocess: false},
+      {"name": "openai/text-davinci-003", "note": "OpenAI", inprocess: false},
+      {"name": "chatgpt", "note": "OpenAI", inprocess: false},
+      {"name": "gpt-4", "note": "OpenAI", inprocess: false}
+    ]
+  }
+
+  if (!configuration.BROWSER_MODE) {
+    PREDEFINED["Other Suggestions"] = Array.from([
+      {"name": "gpt2", "note": "🤗 Tranformers", inprocess: true},
+      {"name": "gpt2-medium", "note": "🤗 Tranformers", inprocess: true},
+      {"name": "facebook/opt-350m", "note": "🤗 Tranformers", inprocess: true},
+      {"name": "llama.cpp:<PATH>/llama-7b.bin", "note": "🦙 llama.cpp", inprocess: true},
+    ]).concat(PREDEFINED["Other Suggestions"])
+  }
+
+  const onInputEnter = (e) => {
+    if (e.key == "Enter") {
+      setSelectOpen(false)
+      e.target.blur()
+    }
+  }
+
+  return <ModelSelectionDiv className={(model == "automatic" ? "auto" : "") + (selectOpen ? " active" : "") }>
+    <input spellCheck={false} placeholder="automatic" value={model} onChange={e => onChange(e.target.value)} autoCorrect={false} onKeyDown={onInputEnter}/>
+    <div className={'select ' + (selectOpen ? "open" : "")}>
+      <span class="instructions">
+        <b>Custom Model</b><br/>
+        Specify the model to execute your query with. You can also type in the text field above.
+        {configuration.BROWSER_MODE ? <><br/><a href={"https://docs.lmql.ai/en/latest/quickstart.html"} target="_blank" rel="noreferrer" className="hidden-on-small">
+          Install LMQL locally </a> to use other models, e.g. from 🤗 Tranformers</>
+        : null}
+      </span>
+      {Object.keys(PREDEFINED).map(k => <>
+        {k != "" ? <h2 key={"key-"+k}>{k}</h2> : null}
+        {PREDEFINED[k].map(o => <div className={'option' + (o.name == model ? " selected" : "")} 
+          onClick={() => {onChange(o.name); setSelectOpen(false);}} key={k+o}>
+          {o.name}
+          <span class="note">
+            {o.note}
+          </span>
+        </div>)}
+        </>)
+      }
+    </div>
+    <div class="overlay" style={{display: selectOpen ? "block" : "none"}} onClick={() => setSelectOpen(false)}></div>
+    <BsPlus onClick={() => setSelectOpen(!selectOpen)}/>
+  </ModelSelectionDiv>
+}
+
 const EditorContainer = styled.div`
   flex: 1;
   overflow: hidden;
   height: auto;
 `
 
 function EditorPanel(props) {
@@ -438,15 +661,15 @@
   let fontSize = window.innerWidth < 700 ? 10 : 16
   if (displayState.mode == "embed") fontSize = 10
 
   return (
     <Panel className='stretch max-width-50' id='editor-panel' style={{
       display: "flex",
     }}>
-      <h2>Query</h2>
+      <h2>Program</h2>
       <EditorContainer ref={editorContainer}>
       <Editor
         defaultValue={persistedState.getItem("lmql-editor-contents") || ""}
         theme="vs-dark"
         // no minimap
         options={{
           // no minimap
@@ -454,43 +677,44 @@
           // no line numbers
           lineNumbers: "off",
           // font size 14pt
           fontSize: fontSize,
           // line wrap
           wordWrap: "on",
           // tabs are spaces
-          // tabSize: 6,
+          tabSize: 4,
           // show whitespace
           renderWhitespace: "all",
           // set font family
           fontFamily: "Fira Code, monospace",
           automaticLayout: true
         }}
         // custom language
         defaultLanguage="lmql"
         style={{ maxHeight: "80%" }}
         onMount={handleEditorDidMount}
       />
       </EditorContainer>
       <ButtonGroup>
-        <FancyButton className='green' onClick={props.onRun} disabled={props.processState != "idle" && props.processState != "secret-missing"}>
+        <FancyButton className='green' onClick={() => props.onRun()} disabled={props.processState != "idle" && props.processState != "secret-missing"}>
           {props.processState == "running" ? <>Running...</> : <>&#x25B6; Run</>}
         </FancyButton>
         {/* status light for connection status */}
         <StatusLight connectionState={props.status} />
         <StopButton onClick={() => {
           LMQLProcess.kill()
         }} disabled={props.processState != "running"}>
           {/* utf8 stop square */}
           <i>&#x25A0;</i> Stop
         </StopButton>
         <ErrorIndicator/>
         {/* <Spacer></Spacer> */}
         <TokenCountIndicator />
       </ButtonGroup>
+      <ModelSelection/>
     </Panel>
   );
 }
 
 const ButtonErrorIndicator = styled.button`
   background: none;
   border: none;
@@ -762,40 +986,40 @@
     opacity: 0.5;
   }
 
   div .tag-system {
     display: block;
     text-align: center;
     background-color: #ffffff13;
-    border-radius: 8pt;
+    border-radius: 2pt;
     font-size: 90%;
     margin-top: 10pt;
     margin-bottom: 10pt;
     color: #c0c0c0;
   }
 
   div .tag-assistant {
-    display: inline-block;
-    border: 1pt solid #5c5c5c;
-    margin-top: 5pt;
-    margin-right: 4%;
+    /* display: inline-block; */
+    /* border: 1pt solid #5c5c5c; */
+    /* margin-top: 5pt;
+    margin-right: 4%; */
 
-    border-radius: 8pt;
+    /* border-radius: 8pt; */
     overflow: hidden;
-    padding: 4pt;
+    /* padding: 4pt; */
   }
 
   div .tag-user {
     display: block;
-    margin-left: 4%;
+    margin-left: 10%;
     position: relative;
     border: 1pt solid #5c5c5c;
     border-radius: 8pt;
     padding: 4pt;
-    margin-bottom: 2pt;
+    margin-bottom: 10pt;
     margin-top: 5pt;
   }
   
   &>div>span:first-child {
     margin-left: 0pt;
     padding-left: 0pt;
   }
@@ -1912,15 +2136,15 @@
 
 const FancyButton = styled.button`
   /* blue purpleish button gardient */
   background-color: #6b77ff;
   border: 0pt solid #6b77ff;
   padding: 8pt 10pt;
   font-size: 10pt;
-  border-radius: 3pt;
+  border-radius: 2pt;
   font-weight: bold;
   color: white;
 
   :hover {
     /* border: 1pt solid #8e98ea; */
     background-color: #a5acfa;
     cursor: pointer;
@@ -2507,19 +2731,22 @@
     a.setAttribute("href", dataUrl);
     a.setAttribute("download", "lmql-state.json");
     a.click();
   }
 
   onRun() {
     const code = persistedState.getItem("lmql-editor-contents");
+    const model = persistedState.getItem("playground-model");
     const appData = {
       "name": "lmql",
       // monaco get editor content
       "app_input": code,
-      "app_arguments": {}
+      "app_arguments": [{
+        "model": model
+      }]
     };
 
     LMQLProcess.run(appData);
   }
 
   onSelectNode(node, additive = false) {
     trackingState.setTrackMostLikely(false)
```

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/CodeScreenshot.jsx` & `lmql-0.0.6.5/src/lmql/ui/playground/src/CodeScreenshot.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/Configuration.js` & `lmql-0.0.6.5/src/lmql/ui/playground/src/Configuration.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/DataListView.js` & `lmql-0.0.6.5/src/lmql/ui/playground/src/DataListView.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/DecoderGraph.js` & `lmql-0.0.6.5/src/lmql/ui/playground/src/DecoderGraph.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/Explore.jsx` & `lmql-0.0.6.5/src/lmql/ui/playground/src/Explore.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/SharedState.js` & `lmql-0.0.6.5/src/lmql/ui/playground/src/SharedState.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/State.js` & `lmql-0.0.6.5/src/lmql/ui/playground/src/State.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/ValidationGraph.jsx` & `lmql-0.0.6.5/src/lmql/ui/playground/src/ValidationGraph.jsx`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/browser_process.js` & `lmql-0.0.6.5/src/lmql/ui/playground/src/browser_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/build_info.js` & `lmql-0.0.6.5/src/lmql/ui/playground/src/build_info.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/editor/lmql-monaco-language.js` & `lmql-0.0.6.5/src/lmql/ui/playground/src/editor/lmql-monaco-language.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/editor/theme.json` & `lmql-0.0.6.5/src/lmql/ui/playground/src/editor/theme.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910552536231885%*

 * *Differences: {"'colors'": "{'editor.background': '#252526'}",*

 * * "'rules'": "{2: {'foreground': 'B8E38D'}, 12: {'foreground': 'C678DD'}}"}*

```diff
@@ -1,11 +1,11 @@
 {
     "base": "vs-dark",
     "colors": {
-        "editor.background": "#1e1e1e",
+        "editor.background": "#252526",
         "editor.foreground": "#f8f8f2",
         "editor.lineHighlightBackground": "#3b3e4d",
         "editor.selectionBackground": "#44475a",
         "editor.selectionHighlightBorder": "#222218",
         "editorCursor.foreground": "#f8f8f0",
         "editorIndentGuide.activeBackground": "#9D550FB0",
         "editorWhitespace.foreground": "#3B3A32"
@@ -17,15 +17,15 @@
             "token": ""
         },
         {
             "foreground": "6272a4",
             "token": "comment"
         },
         {
-            "foreground": "98c379",
+            "foreground": "B8E38D",
             "token": "string"
         },
         {
             "foreground": "bd93f9",
             "token": "constant.numeric"
         },
         {
@@ -58,15 +58,15 @@
         },
         {
             "foreground": "ff79c6",
             "token": "string source.ruby"
         },
         {
             "fontStyle": "bold",
-            "foreground": "ff79c6",
+            "foreground": "C678DD",
             "token": "keyword"
         },
         {
             "foreground": "ff79c6",
             "token": "storage"
         },
         {
```

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/explore.svg` & `lmql-0.0.6.5/src/lmql/ui/playground/src/explore.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/graph-layout.css` & `lmql-0.0.6.5/src/lmql/ui/playground/src/graph-layout.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/index.css` & `lmql-0.0.6.5/src/lmql/ui/playground/src/index.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/logo.svg` & `lmql-0.0.6.5/src/lmql/ui/playground/src/logo.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/queries.js` & `lmql-0.0.6.5/src/lmql/ui/playground/src/queries.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -4,221 +4,242 @@
         {
             category: "Introductory Examples",
             queries: [{
                 // hello world
                 name: "👋 Hello World",
                 description: "Who This?",
                 code: `argmax 
-   "Say 'this is a test':[RESPONSE]" 
+    "Say 'this is a test':[RESPONSE]" 
 from 
-   "openai/text-ada-001" 
+    "openai/text-ada-001" 
 where 
-   len(TOKENS(RESPONSE)) < 10`,
+    len(TOKENS(RESPONSE)) < 10`,
                 state: 'precomputed/hello.json'
             }, {
                 name: "👴 Tell A Joke",
                 description: "Few-Shot Samples & Constraints",
                 code: `argmax
-   """A list of good dad jokes. A indicates the punchline
-   Q: How does a penguin build its house?
-   A: Igloos it together.
-   Q: Which knight invented King Arthur's Round Table?
-   A: Sir Cumference.
-   Q:[JOKE]
-   A:[PUNCHLINE]"""
+    """A list of good dad jokes. A indicates the punchline
+    Q: How does a penguin build its house?
+    A: Igloos it together.
+    Q: Which knight invented King Arthur's Round Table?
+    A: Sir Cumference.
+    Q:[JOKE]
+    A:[PUNCHLINE]"""
 from
-   "openai/text-davinci-003"
+    "openai/text-davinci-003"
 where
-   len(JOKE) < 120 and 
-   STOPS_AT(JOKE, "?") and 
-   STOPS_AT(PUNCHLINE, "\\n") and 
-   len(PUNCHLINE) > 1`,
+    len(JOKE) < 120 and 
+    STOPS_AT(JOKE, "?") and 
+    STOPS_AT(PUNCHLINE, "\\n") and 
+    len(PUNCHLINE) > 1`,
                 state: 'precomputed/joke.json'
             }, {
                 name: "🌴 Packing List",
                 description: "Control-Flow Guided Generation",
                 code: `sample(temperature=0.8)
-   "A list of things not to forget when going to the sea (not travelling): \\n"
-   "- Sunglasses \\n"
-   for i in range(4):
-      "- [THING] \\n"
+    "A list of things not to forget when going to the sea (not travelling): \\n"
+    "- Sunglasses \\n"
+    for i in range(4):
+        "- [THING] \\n"
 from
-   'openai/text-ada-001'
+    'openai/text-ada-001'
 where
-   THING in set(["Volleyball", "Sunscreen", "Bathing Suite"])`,
+    THING in set(["Volleyball", "Sunscreen", "Bathing Suite"])`,
                 state: 'precomputed/list.json'
-            }, ]
+            }, {
+                name: "📝 Generate JSON",
+                description: "Template-Based Generation",
+                code: `argmax 
+    """
+    Write a summary of Bruno Mars, the singer:
+    {{
+      "name": "[STRING_VALUE]",
+      "age": [INT_VALUE],
+      "top_songs": [[
+         "[STRING_VALUE]",
+         "[STRING_VALUE]"
+      ]]
+    }}
+    """
+from
+    "openai/text-davinci-003" 
+where
+    STOPS_BEFORE(STRING_VALUE, '"') and INT(INT_VALUE) and len(TOKENS(INT_VALUE)) < 2
+         
+         `,
+                state: 'precomputed/json-template.json'
+            }]
         }, {
             category: "LLM Reasoning",
             queries: [{
                 name: "🧠 Chain-Of-Thought",
                 description: "CoT with robust result extraction.",
                 code: `# zero-shot cot based on https://arxiv.org/pdf/2205.11916.pdf
 argmax
-   """Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?
-   Answer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021
-   A: Let's think step by step."""
-   "[REASONING]\\n"
-   "Therefore, among A through F, the answer is[RESULT]"
-   assert RESULT == "A"
+    """Q: It was Sept. 1st, 2021 a week ago. What is the date 10 days ago in MM/DD/YYYY?
+    Answer Choices: (A) 08/29/2021 (B) 08/28/2021 (C) 08/29/1925 (D) 08/30/2021 (E) 05/25/2021 (F) 09/19/2021
+    A: Let's think step by step."""
+    "[REASONING]\\n"
+    "Therefore, among A through F, the answer is[RESULT]"
 from
-   "openai/text-davinci-003"
+    "openai/text-davinci-003"
 where
-   RESULT in ["A", "B", "C", "D", "E", "F"]`,
+    RESULT in ["A", "B", "C", "D", "E", "F"]`,
                 state: 'precomputed/cot.json'
             }, {
                 name: "👩‍🔬 Meta Prompting",
                 description: "Asking an expert to answer.",
                 code: `# metaprompting based on https://arxiv.org/pdf/2102.07350.pdf
 beam(n=2)
-   "Q: What are Large Language Models?\\n\\n"
-   "A good person to answer this question would be[EXPERT]\\n\\n"
-   expert_name = EXPERT.rstrip(".\\n")
-   "For instance,{expert_name} would answer[ANSWER]"
+    "Q: What are Large Language Models?\\n\\n"
+    "A good person to answer this question would be[EXPERT]\\n\\n"
+    expert_name = EXPERT.rstrip(".\\n")
+    "For instance,{expert_name} would answer[ANSWER]"
 from 
-   "openai/text-davinci-001"
+    "openai/text-davinci-001"
 where
-   STOPS_AT(EXPERT, ".") and STOPS_AT(EXPERT, "\\n") and STOPS_AT(ANSWER, ".")`,
+    STOPS_AT(EXPERT, ".") and STOPS_AT(EXPERT, "\\n") and STOPS_AT(ANSWER, ".")`,
                 state: 'precomputed/meta.json'
             }]
         }, {
             category: "Tool-Augmented Queries",
             queries: [{
                 name: "🧮 Calculator",
                 description: "On-the-fly arithmetic evaluation using Python.",
                 code: `import re
 from lmql.demo import gsm8k_samples
 
 def calc(expr):
-      expr = re.sub(r"[^0-9\+\\-*/\(\)\.]", "", expr)
-      return eval(expr)
+    expr = re.sub(r"[^0-9\+\\-*/\(\)\.]", "", expr)
+    return eval(expr)
 
 argmax(openai_chunksize=64, max_len=2048)
-      QUESTION = "Josh decides to try flipping a house.  He buys a house for $80,000 and then puts in $50,000 in repairs.  This increased the value of the house by 150%.  How much profit did he make?"
-      # few shot samples
-      "{gsm8k_samples()}"
-      # prompt template
-      "Q: {QUESTION}\\n"
-      "Let's think step by step.\\n"
-      for i in range(4):
-         "[REASON_OR_CALC]"
-         if REASON_OR_CALC.endswith("<<"):
+    QUESTION = "Josh decides to try flipping a house.  He buys a house for $80,000 and then puts in $50,000 in repairs.  This increased the value of the house by 150%.  How much profit did he make?"
+    # few shot samples
+    "{gsm8k_samples()}"
+    # prompt template
+    "Q: {QUESTION}\\n"
+    "Let's think step by step.\\n"
+    for i in range(4):
+        "[REASON_OR_CALC]"
+        if REASON_OR_CALC.endswith("<<"):
             " [EXPR]"
             " {calc(EXPR)}>>"
-         elif REASON_OR_CALC.endswith("So the answer"):
+        elif REASON_OR_CALC.endswith("So the answer"):
             break
-      "is[RESULT]"
+    "is[RESULT]"
 from 
-      'openai/text-davinci-003'
+    'openai/text-davinci-003'
 where
-      STOPS_AT(REASON_OR_CALC, "<<") and
-      STOPS_AT(EXPR, "=") and
-      STOPS_AT(REASON_OR_CALC, "So the answer")`,
+    STOPS_AT(REASON_OR_CALC, "<<") and
+    STOPS_AT(EXPR, "=") and
+    STOPS_AT(REASON_OR_CALC, "So the answer")`,
                 state: 'precomputed/calc.json'
             }, {
                 name: "🌎 Wikipedia Search",
                 description: "Interactive LM-driven Wikipedia search.",
                 code: `async def wikipedia(q):
-   from lmql.http import fetch
-   try:
-      q = q.strip("\\n '.")
-      pages = await fetch(f"https://en.wikipedia.org/w/api.php?format=json&action=query&prop=extracts&exintro&explaintext&redirects=1&titles={q}&origin=*", "query.pages")
-      return list(pages.values())[0]["extract"][:280]
-   except:
-      return "No results"
+    from lmql.http import fetch
+    try:
+        q = q.strip("\\n '.")
+        pages = await fetch(f"https://en.wikipedia.org/w/api.php?format=json&action=query&prop=extracts&exintro&explaintext&redirects=1&titles={q}&origin=*", "query.pages")
+        return list(pages.values())[0]["extract"][:280]
+    except:
+        return "No results"
 
 argmax
-   "Q: From which countries did the Norse originate?\\n"
-   "Action: Let's search Wikipedia for the term '[TERM]\\n"
-   result = await wikipedia(TERM)
-   "Result: {result}\\n"
-   "Final Answer:[ANSWER]"
+    "Q: From which countries did the Norse originate?\\n"
+    "Action: Let's search Wikipedia for the term '[TERM]\\n"
+    result = await wikipedia(TERM)
+    "Result: {result}\\n"
+    "Final Answer:[ANSWER]"
 from 
-   "openai/text-davinci-003"
+    "openai/text-davinci-003"
 where
-   STOPS_AT(TERM, "'")`,
+    STOPS_AT(TERM, "'")`,
                 state: 'precomputed/wiki.json'
             }, {
                 name: "📖 Key-Value Memory",
                 description: "Augment the LM with a key-value storage.",
                 code: `# simple kv storage
 storage = {}
 def assign(key, value): storage[key] = value; return f'{{{key}: "{value}"}}'
 def get(key): return storage.get(key)
 
 argmax(n=1, openai_chunksize=128, max_len=2048, step_budget=4*2048)
-   """In your reasoning you can use actions. You do this as follows:
-   \`action_name(<args>) # result: <inserted result>\`
-   To remember things, you can use 'assign'/'get':
-   - To remember something:
-   \`assign("Alice", "banana") # result: "banana"\`
-   - To retrieve a stored value:
-   \`get("Alice") # result: "banana"\`
-   Always tail calls with " # result". Using these actions, let's solve the following question.
+    """In your reasoning you can use actions. You do this as follows:
+    \`action_name(<args>) # result: <inserted result>\`
+    To remember things, you can use 'assign'/'get':
+    - To remember something:
+    \`assign("Alice", "banana") # result: "banana"\`
+    - To retrieve a stored value:
+    \`get("Alice") # result: "banana"\`
+    Always tail calls with " # result". Using these actions, let's solve the following question.
    
-   Q: Alice, Bob, and Claire are playing a game. At the start of the game, they are each holding a ball: Alice has a black ball, Bob has a brown ball, and Claire has a blue ball. \\n\\nAs the game progresses, pairs of players trade balls. First, Bob and Claire swap balls. Then, Alice and Bob swap balls. Finally, Claire and Bob swap balls. At the end of the game, what ball does Alice have?
-   A: Let's think step by step.\\n"""
-   for i in range(32):
-      "[REASONING]"
-      if REASONING.endswith("# result"):
-         cmd = REASONING.rsplit("\`",1)[-1]
-         cmd = cmd[:-len("# result")]
-         "{eval(cmd)}\`\\n"
-      else:
-         break
-   """Therefore at the end of the game, Alice has the[OBJECT]"""
-   assert "blue ball." in OBJECT
+    Q: Alice, Bob, and Claire are playing a game. At the start of the game, they are each holding a ball: Alice has a black ball, Bob has a brown ball, and Claire has a blue ball. \\n\\nAs the game progresses, pairs of players trade balls. First, Bob and Claire swap balls. Then, Alice and Bob swap balls. Finally, Claire and Bob swap balls. At the end of the game, what ball does Alice have?
+    A: Let's think step by step.\\n"""
+    for i in range(32):
+        "[REASONING]"
+        if REASONING.endswith("# result"):
+            cmd = REASONING.rsplit("\`",1)[-1]
+            cmd = cmd[:-len("# result")]
+            "{eval(cmd)}\`\\n"
+        else:
+            break
+    """Therefore at the end of the game, Alice has the[OBJECT]"""
+    assert "blue ball." in OBJECT
 from 
-   "openai/text-davinci-003"
+    "openai/text-davinci-003"
 where
-   STOPS_AT(REASONING, "# result") and STOPS_AT(REASONING, "Therefore, ") and
-   STOPS_AT(OBJECT, ".") and STOPS_AT(OBJECT, ",")            
+    STOPS_AT(REASONING, "# result") and STOPS_BEFORE(REASONING, "Therefore") and
+    STOPS_AT(OBJECT, ".") and STOPS_AT(OBJECT, ",")            
 `,
                 state: 'precomputed/kv.json'
             }]
         }, {
             category: "Decoding",
             queries: [{
                 name: "🔍 Visualize Decoding",
                 description: "Inspect the decoding tree of beam search.",
                 code: `beam(n=4)
-   """English to French Translation:
-   English: I am going to the store
-   French: [TRANSLATION]
-   """
+    """English to French Translation:
+    English: I am going to the store
+    French: [TRANSLATION]
+    """
 from 
-   "openai/text-davinci-001"
+    "openai/text-davinci-001"
 where
-   STOPS_AT(TRANSLATION, "\\n")`,
+    STOPS_AT(TRANSLATION, "\\n")`,
                 state: 'precomputed/translation.json'
             }, {
                 name: "📊 Distributions",
                 description: "Classification via LM-based conditional distributions.",
                 code: `argmax
-   """Review: We had a great stay. Hiking in the mountains was fabulous and the food is really good.\\n
-   Q: What is the underlying sentiment of this review and why?\\n
-   A:[ANALYSIS]\\n
-   Based on this, the overall sentiment of the message can be considered to be[CLASSIFICATION]"""
+    """Review: We had a great stay. Hiking in the mountains was fabulous and the food is really good.\\n
+    Q: What is the underlying sentiment of this review and why?\\n
+    A:[ANALYSIS]\\n
+    Based on this, the overall sentiment of the message can be considered to be[CLASSIFICATION]"""
 from 
-   "openai/text-davinci-003"
+    "openai/text-davinci-003"
 distribution
-   CLASSIFICATION in [" positive", " neutral", " negative"]`,
+    CLASSIFICATION in [" positive", " neutral", " negative"]`,
                 state: 'precomputed/distribution.json'
             }]
         }, {
             category: "Chatbots",
             requires_input: true,
             queries: [{
                 name: "🗣️ Chatbot",
                 description: "Build a chatbot using interactive querying.",
                 code: `argmax 
-   "{:system} You are a marketing chatbot for the language model query language (LMQL)."
-   for i in range(10):
-      "{:user} {await input()}"
-      "{:assistant} [ANSWER]"
+    "{:system} You are a marketing chatbot for the language model query language (LMQL)."
+    for i in range(10):
+        "{:user} {await input()}"
+        "{:assistant} [ANSWER]"
 from
    "chatgpt"`,
                 state: 'precomputed/chat.json'
             }, ]
         },
     ]
 };
```

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/remote_process.js` & `lmql-0.0.6.5/src/lmql/ui/playground/src/remote_process.js`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/screenshot.css` & `lmql-0.0.6.5/src/lmql/ui/playground/src/screenshot.css`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/spinner.svg` & `lmql-0.0.6.5/src/lmql/ui/playground/src/spinner.svg`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/src/tagged-model-result.js` & `lmql-0.0.6.5/src/lmql/ui/playground/src/tagged-model-result.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2,15 +2,15 @@
     if (nodes == null) {
         return []
     }
 
     function unescapeBytes(s) {
         if (s.length == 1) {
             // unpack array
-            if (s[0].startsWith("bytes:")) {
+            if (s[0].startsWith && s[0].startsWith("bytes:")) {
                 return [s[0].substring(6)]
             } else {
                 return [s]
             }
         }
         return s
     }
```

### Comparing `lmql-0.0.6.4/src/lmql/ui/playground/yarn.lock` & `lmql-0.0.6.5/src/lmql/ui/playground/yarn.lock`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/vscode/.vscode/launch.json` & `lmql-0.0.6.5/src/lmql/ui/vscode/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/vscode/LICENSE` & `lmql-0.0.6.5/src/lmql/ui/vscode/LICENSE`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/vscode/language-configuration.json` & `lmql-0.0.6.5/src/lmql/ui/vscode/language-configuration.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/vscode/lmql-vscode.png` & `lmql-0.0.6.5/src/lmql/ui/vscode/lmql-vscode.png`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/vscode/package.json` & `lmql-0.0.6.5/src/lmql/ui/vscode/package.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/vscode/syntaxes/lmql.qstring.json` & `lmql-0.0.6.5/src/lmql/ui/vscode/syntaxes/lmql.qstring.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json` & `lmql-0.0.6.5/src/lmql/ui/vscode/syntaxes/lmql.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/ui/vscode/syntaxes/pylmql.json` & `lmql-0.0.6.5/src/lmql/ui/vscode/syntaxes/pylmql.json`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/utils/docstring_parser.py` & `lmql-0.0.6.5/src/lmql/utils/docstring_parser.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/utils/graph.py` & `lmql-0.0.6.5/src/lmql/utils/graph.py`

 * *Files identical despite different names*

### Comparing `lmql-0.0.6.4/src/lmql/utils/nputil.py` & `lmql-0.0.6.5/src/lmql/utils/nputil.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,20 +26,23 @@
         return v
     elif hasattr(v, "numpy"):
         return ensure_iterable(v.numpy())
     else:
         assert False, f"ensure_iterable(): type {type(v)} cannot be converted to iterable"
 
 
-def log_softmax(a):
+def log_softmax(a, axis=-1):
+    a = ensure_array(a)
     # check for log div by zero
-    normalizer = np.sum(np.exp(a))
-    if normalizer == 0:
+    normalizer = np.sum(np.exp(a), axis=axis)
+    if (normalizer == 0).any():
         # assign 1.0 to max value
         return np.where(a == np.max(a), 0.0, -np.inf)
+    if len(a.shape) > 1:
+        normalizer = normalizer.reshape(-1,1)
     return a - np.log(normalizer)
 
 def topk(a, k:int, sorted: bool = False, axis=-1):
     assert k > 0, "topk(): k must be > 0"
     idx = np.argpartition(a, -k, axis=axis)[..., -k:]
     if sorted: 
         index_values = np.take_along_axis(a, idx, axis=axis)
```

### Comparing `lmql-0.0.6.4/src/lmql.egg-info/SOURCES.txt` & `lmql-0.0.6.5/src/lmql.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 .gitignore
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+yarn.lock
+.github/workflows/lmql-ci.yml
+.github/workflows/lmql-tests.yml
 .github/workflows/lmql-web.yml
 docs/Makefile
 docs/RELEASE.md
 docs/make.bat
 docs/requirements.txt
 docs/todo.md
 docs/source/conf.py
@@ -23,27 +26,31 @@
 docs/source/_static/css/lmql-docs.css
 docs/source/_static/images/lmql.svg
 docs/source/_static/js/lmql-playground.js
 docs/source/_templates/layout.html
 docs/source/blog/release-0.0.5.md
 docs/source/blog/release-0.0.6.1.md
 docs/source/blog/release-0.0.6.3.md
+docs/source/blog/release-0.0.6.4.md
+docs/source/blog/release-0.0.6.5.md
 docs/source/blog/release-0.0.6.md
 docs/source/images/inference.svg
 docs/source/language/azure.md
 docs/source/language/constraints.md
 docs/source/language/decoders.md
 docs/source/language/functions.md
 docs/source/language/hf.md
+docs/source/language/llama.cpp.md
 docs/source/language/models.md
 docs/source/language/openai.md
 docs/source/language/overview.md
 docs/source/language/scripted_prompts.md
 docs/source/pending/release-next.md
 docs/source/python/.gitignore
+docs/source/python/comparison.md
 docs/source/python/langchain.ipynb
 docs/source/python/lc.py
 docs/source/python/llama_index.ipynb
 docs/source/python/lmql.txt
 docs/source/python/output.ipynb
 docs/source/python/pandas.ipynb
 docs/source/python/python.ipynb
@@ -75,22 +82,31 @@
 src/lmql/language/compiler.py
 src/lmql/language/fragment_parser.py
 src/lmql/language/qstrings.py
 src/lmql/language/validator.py
 src/lmql/models/__init__.py
 src/lmql/models/model.py
 src/lmql/models/lmtp/README.md
+src/lmql/models/lmtp/errors.py
+src/lmql/models/lmtp/lmtp_async.py
 src/lmql/models/lmtp/lmtp_client.py
 src/lmql/models/lmtp/lmtp_dcmodel.py
 src/lmql/models/lmtp/lmtp_inference_server.py
 src/lmql/models/lmtp/lmtp_multiprocessing.py
 src/lmql/models/lmtp/lmtp_programmatic_serve_example.py
+src/lmql/models/lmtp/lmtp_scheduler.py
 src/lmql/models/lmtp/lmtp_serve.py
 src/lmql/models/lmtp/lmtp_threading.py
 src/lmql/models/lmtp/utils.py
+src/lmql/models/lmtp/backends/__init__.py
+src/lmql/models/lmtp/backends/__main__.py
+src/lmql/models/lmtp/backends/llama_cpp_model.py
+src/lmql/models/lmtp/backends/lmtp_model.py
+src/lmql/models/lmtp/backends/random_model.py
+src/lmql/models/lmtp/backends/transformers_model.py
 src/lmql/ops/__init__.py
 src/lmql/ops/follow_map.py
 src/lmql/ops/ops.py
 src/lmql/ops/token_set.py
 src/lmql/output/__init__.py
 src/lmql/output/http.py
 src/lmql/output/sse.py
@@ -127,23 +143,28 @@
 src/lmql/runtime/postprocessing/__init__.py
 src/lmql/runtime/postprocessing/conditional_prob.py
 src/lmql/runtime/postprocessing/group_by.py
 src/lmql/runtime/tokenizers/hf_tokenizer.py
 src/lmql/runtime/tokenizers/pure_python_tokenizer.py
 src/lmql/runtime/tokenizers/tiktoken_tokenizer.py
 src/lmql/tests/README.md
+src/lmql/tests/all.py
 src/lmql/tests/expr_test_utils.py
 src/lmql/tests/fin_and.py
-src/lmql/tests/local_model_python.py
 src/lmql/tests/tail_token_set.py
 src/lmql/tests/test_back2back_caching.py
+src/lmql/tests/test_beam_in.py
 src/lmql/tests/test_eq.py
+src/lmql/tests/test_escaping.py
+src/lmql/tests/test_local_model_python.py
+src/lmql/tests/test_minimal_syntax.py
 src/lmql/tests/test_multibyte_characters.py
 src/lmql/tests/test_multibyte_local_models.py
 src/lmql/tests/test_orop.py
+src/lmql/tests/test_qstrings.py
 src/lmql/tests/test_query_args.py
 src/lmql/tests/test_sample_queries.py
 src/lmql/tests/test_scoping.py
 src/lmql/tests/test_stopping.py
 src/lmql/tests/tiktoken_tsets.py
 src/lmql/tests/outdated/mask_product_test.py
 src/lmql/tests/outdated/monotonicity.py
@@ -185,14 +206,15 @@
 src/lmql/ui/playground/public/robots.txt
 src/lmql/ui/playground/public/precomputed/calc.json
 src/lmql/ui/playground/public/precomputed/chat.json
 src/lmql/ui/playground/public/precomputed/cot.json
 src/lmql/ui/playground/public/precomputed/distribution.json
 src/lmql/ui/playground/public/precomputed/hello.json
 src/lmql/ui/playground/public/precomputed/joke.json
+src/lmql/ui/playground/public/precomputed/json-template.json
 src/lmql/ui/playground/public/precomputed/kv.json
 src/lmql/ui/playground/public/precomputed/list.json
 src/lmql/ui/playground/public/precomputed/meta.json
 src/lmql/ui/playground/public/precomputed/translation.json
 src/lmql/ui/playground/public/precomputed/wiki.json
 src/lmql/ui/playground/public/snippets/dynamic-cfg.json
 src/lmql/ui/playground/public/snippets/json-parsing.json
```

### Comparing `lmql-0.0.6.4/src/lmql.svg` & `lmql-0.0.6.5/src/lmql.svg`

 * *Files identical despite different names*

