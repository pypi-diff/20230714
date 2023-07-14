# Comparing `tmp/spacy-llm-0.4.1.tar.gz` & `tmp/spacy-llm-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-llm-0.4.1.tar", last modified: Tue Jul 11 11:30:17 2023, max compression
+gzip compressed data, was "spacy-llm-0.4.2.tar", last modified: Fri Jul 14 09:43:35 2023, max compression
```

## Comparing `spacy-llm-0.4.1.tar` & `spacy-llm-0.4.2.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.310685 spacy-llm-0.4.1/
--rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      147 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)   102951 2023-07-11 11:30:17.314685 spacy-llm-0.4.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)   101733 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      918 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1827 2023-07-11 11:30:17.314685 spacy-llm-0.4.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.294685 spacy-llm-0.4.1/spacy_llm/
--rw-r--r--   0 vsts      (1001) docker     (122)      232 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10379 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)      895 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.294685 spacy-llm-0.4.1/spacy_llm/models/
--rw-r--r--   0 vsts      (1001) docker     (122)      291 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.298685 spacy-llm-0.4.1/spacy_llm/models/hf/
--rw-r--r--   0 vsts      (1001) docker     (122)      264 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/hf/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4886 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/hf/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2439 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/hf/dolly.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2814 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/hf/falcon.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3332 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/hf/openllama.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4816 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/hf/stablelm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.298685 spacy-llm-0.4.1/spacy_llm/models/langchain/
--rw-r--r--   0 vsts      (1001) docker     (122)      227 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/langchain/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4540 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/langchain/model.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.298685 spacy-llm-0.4.1/spacy_llm/models/rest/
--rw-r--r--   0 vsts      (1001) docker     (122)      136 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.298685 spacy-llm-0.4.1/spacy_llm/models/rest/anthropic/
--rw-r--r--   0 vsts      (1001) docker     (122)      476 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/anthropic/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4252 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/anthropic/model.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10902 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/anthropic/registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5971 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/base.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.298685 spacy-llm-0.4.1/spacy_llm/models/rest/cohere/
--rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/cohere/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3369 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/cohere/model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2016 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/cohere/registry.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.298685 spacy-llm-0.4.1/spacy_llm/models/rest/noop/
--rw-r--r--   0 vsts      (1001) docker     (122)      123 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/noop/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      865 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/noop/model.py
--rw-r--r--   0 vsts      (1001) docker     (122)      351 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/noop/registry.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.298685 spacy-llm-0.4.1/spacy_llm/models/rest/openai/
--rw-r--r--   0 vsts      (1001) docker     (122)      538 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5813 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/openai/model.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19421 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/openai/registry.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.298685 spacy-llm-0.4.1/spacy_llm/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11251 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/pipeline/llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.298685 spacy-llm-0.4.1/spacy_llm/registry/
--rw-r--r--   0 vsts      (1001) docker     (122)      262 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/registry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/registry/normalizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2940 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/registry/reader.py
--rw-r--r--   0 vsts      (1001) docker     (122)      450 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/registry/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.302685 spacy-llm-0.4.1/spacy_llm/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)      850 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4725 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/lemma.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8738 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)      645 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/noop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8998 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/rel.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4807 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/sentiment.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6944 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/span.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9497 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/spancat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5720 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/summarization.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.302685 spacy-llm-0.4.1/spacy_llm/tasks/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)      288 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1003 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/lemma.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)      732 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/ner.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/ner.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1571 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/rel.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)      526 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/sentiment.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)      755 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/spancat.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/spancat.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)      661 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/summarization.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1237 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/textcat.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1703 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/textcat.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     2148 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/textcat.v3.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)    16409 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/textcat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.302685 spacy-llm-0.4.1/spacy_llm/tasks/util/
--rw-r--r--   0 vsts      (1001) docker     (122)      132 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1319 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/util/parsing.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4042 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/util/serialization.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.302685 spacy-llm-0.4.1/spacy_llm/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      315 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/compat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1350 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.306685 spacy-llm-0.4.1/spacy_llm/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2323 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/models/test_anthropic.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3068 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/models/test_cohere.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1618 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/models/test_dolly.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1508 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/models/test_falcon.py
--rw-r--r--   0 vsts      (1001) docker     (122)      597 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/models/test_langchain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1865 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/models/test_openllama.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3299 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/models/test_rest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2085 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/models/test_stablelm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.306685 spacy-llm-0.4.1/spacy_llm/tests/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8914 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/pipeline/test_llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.306685 spacy-llm-0.4.1/spacy_llm/tests/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.310685 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/
--rw-r--r--   0 vsts      (1001) docker     (122)     1115 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/lemma.json
--rw-r--r--   0 vsts      (1001) docker     (122)      841 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/lemma.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      930 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/lemma.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/ner.json
--rw-r--r--   0 vsts      (1001) docker     (122)      233 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/ner.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/ner.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      349 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/ner_inconsistent.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      579 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/rel.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/sentiment.json
--rw-r--r--   0 vsts      (1001) docker     (122)      186 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/sentiment.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      174 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/sentiment.yml
--rw-r--r--   0 vsts      (1001) docker     (122)     3126 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/summarization.json
--rw-r--r--   0 vsts      (1001) docker     (122)     3093 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/summarization.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)     3089 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/summarization.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/textcat_binary.json
--rw-r--r--   0 vsts      (1001) docker     (122)      355 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/textcat_binary.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/textcat_binary.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      417 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/textcat_multi_excl.json
--rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/textcat_multi_excl.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      379 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/textcat_multi_excl.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.json
--rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      395 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.yml
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.310685 spacy-llm-0.4.1/spacy_llm/tests/tasks/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/templates/lemma.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/templates/ner.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)       27 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/templates/sentiment.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/templates/summarization.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/templates/textcat.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)     9678 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/test_lemma.py
--rw-r--r--   0 vsts      (1001) docker     (122)    24355 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/test_ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6093 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/test_rel.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6983 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/test_sentiment.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17549 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/test_spancat.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13777 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/test_summarization.py
--rw-r--r--   0 vsts      (1001) docker     (122)    23930 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/test_textcat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9200 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/test_cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1694 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/test_combinations.py
--rw-r--r--   0 vsts      (1001) docker     (122)      325 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/test_registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9252 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/ty.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1764 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.294685 spacy-llm-0.4.1/spacy_llm.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)   102951 2023-07-11 11:30:17.000000 spacy-llm-0.4.1/spacy_llm.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     5129 2023-07-11 11:30:17.000000 spacy-llm-0.4.1/spacy_llm.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-11 11:30:17.000000 spacy-llm-0.4.1/spacy_llm.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-07-11 11:30:17.000000 spacy-llm-0.4.1/spacy_llm.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-11 11:30:17.000000 spacy-llm-0.4.1/spacy_llm.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      137 2023-07-11 11:30:17.000000 spacy-llm-0.4.1/spacy_llm.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-07-11 11:30:17.000000 spacy-llm-0.4.1/spacy_llm.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.310685 spacy-llm-0.4.1/usage_examples/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.310685 spacy-llm-0.4.1/usage_examples/multitask_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/multitask_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1244 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/multitask_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.310685 spacy-llm-0.4.1/usage_examples/ner_dolly/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/ner_dolly/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/ner_dolly/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.310685 spacy-llm-0.4.1/usage_examples/ner_langchain_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/ner_langchain_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/ner_langchain_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.310685 spacy-llm-0.4.1/usage_examples/rel_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/rel_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1337 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/rel_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.310685 spacy-llm-0.4.1/usage_examples/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3361 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/tests/test_readme_examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2608 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/tests/test_usage_examples.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.310685 spacy-llm-0.4.1/usage_examples/textcat_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/textcat_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1173 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/textcat_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.309926 spacy-llm-0.4.2/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      147 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)   102951 2023-07-14 09:43:35.309926 spacy-llm-0.4.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)   101733 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      918 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1827 2023-07-14 09:43:35.309926 spacy-llm-0.4.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.293926 spacy-llm-0.4.2/spacy_llm/
+-rw-r--r--   0 vsts      (1001) docker     (122)      232 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10379 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      895 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.293926 spacy-llm-0.4.2/spacy_llm/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)      291 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.293926 spacy-llm-0.4.2/spacy_llm/models/hf/
+-rw-r--r--   0 vsts      (1001) docker     (122)      264 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/hf/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4886 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/hf/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2439 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/hf/dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2814 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/hf/falcon.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3332 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/hf/openllama.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4816 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/hf/stablelm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.293926 spacy-llm-0.4.2/spacy_llm/models/langchain/
+-rw-r--r--   0 vsts      (1001) docker     (122)      227 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/langchain/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4540 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/langchain/model.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.293926 spacy-llm-0.4.2/spacy_llm/models/rest/
+-rw-r--r--   0 vsts      (1001) docker     (122)      136 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.293926 spacy-llm-0.4.2/spacy_llm/models/rest/anthropic/
+-rw-r--r--   0 vsts      (1001) docker     (122)      476 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/anthropic/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4627 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/anthropic/model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10902 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/anthropic/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5971 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/base.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.293926 spacy-llm-0.4.2/spacy_llm/models/rest/cohere/
+-rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/cohere/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3722 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/cohere/model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2016 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/cohere/registry.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.297926 spacy-llm-0.4.2/spacy_llm/models/rest/noop/
+-rw-r--r--   0 vsts      (1001) docker     (122)      123 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/noop/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      865 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/noop/model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      351 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/noop/registry.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.297926 spacy-llm-0.4.2/spacy_llm/models/rest/openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)      538 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6093 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/openai/model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19421 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/models/rest/openai/registry.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.297926 spacy-llm-0.4.2/spacy_llm/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11251 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/pipeline/llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.297926 spacy-llm-0.4.2/spacy_llm/registry/
+-rw-r--r--   0 vsts      (1001) docker     (122)      262 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/registry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/registry/normalizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2940 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/registry/reader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      450 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/registry/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.297926 spacy-llm-0.4.2/spacy_llm/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)      850 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4725 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/lemma.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8738 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      645 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/noop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9184 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/rel.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4807 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/sentiment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6944 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/span.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9497 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/spancat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5720 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/summarization.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.301926 spacy-llm-0.4.2/spacy_llm/tasks/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)      288 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1003 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/lemma.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      732 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/ner.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/ner.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1571 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/rel.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      526 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/sentiment.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      755 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/spancat.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/spancat.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      661 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/summarization.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1237 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/textcat.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1703 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/textcat.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     2148 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/templates/textcat.v3.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)    16409 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/textcat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.301926 spacy-llm-0.4.2/spacy_llm/tasks/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)      132 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1319 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/util/parsing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4042 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tasks/util/serialization.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.301926 spacy-llm-0.4.2/spacy_llm/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      315 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1350 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/conftest.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.301926 spacy-llm-0.4.2/spacy_llm/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2323 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/models/test_anthropic.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3068 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/models/test_cohere.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1618 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/models/test_dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1508 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/models/test_falcon.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      597 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/models/test_langchain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1865 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/models/test_openllama.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3299 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/models/test_rest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2085 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/models/test_stablelm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.301926 spacy-llm-0.4.2/spacy_llm/tests/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8914 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/pipeline/test_llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.301926 spacy-llm-0.4.2/spacy_llm/tests/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.305926 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1115 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/lemma.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      841 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/lemma.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      930 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/lemma.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/ner.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      233 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/ner.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/ner.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      349 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/ner_inconsistent.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      579 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/rel.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/sentiment.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      186 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/sentiment.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      174 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/sentiment.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)     3126 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/summarization.json
+-rw-r--r--   0 vsts      (1001) docker     (122)     3093 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/summarization.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)     3089 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/summarization.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/textcat_binary.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      355 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/textcat_binary.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/textcat_binary.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      417 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/textcat_multi_excl.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/textcat_multi_excl.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      379 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/textcat_multi_excl.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      395 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.yml
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.305926 spacy-llm-0.4.2/spacy_llm/tests/tasks/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/templates/lemma.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/templates/ner.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)       27 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/templates/sentiment.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/templates/summarization.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/templates/textcat.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)     9678 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/test_lemma.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    24355 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/test_ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6774 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/test_rel.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6983 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/test_sentiment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17549 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/test_spancat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13777 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/test_summarization.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    23930 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/tasks/test_textcat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9200 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/test_cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1694 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/test_combinations.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      325 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/tests/test_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9252 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/ty.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1764 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/spacy_llm/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.293926 spacy-llm-0.4.2/spacy_llm.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)   102951 2023-07-14 09:43:35.000000 spacy-llm-0.4.2/spacy_llm.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     5129 2023-07-14 09:43:35.000000 spacy-llm-0.4.2/spacy_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-14 09:43:35.000000 spacy-llm-0.4.2/spacy_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-07-14 09:43:35.000000 spacy-llm-0.4.2/spacy_llm.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-14 09:43:35.000000 spacy-llm-0.4.2/spacy_llm.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      137 2023-07-14 09:43:35.000000 spacy-llm-0.4.2/spacy_llm.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-07-14 09:43:35.000000 spacy-llm-0.4.2/spacy_llm.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.305926 spacy-llm-0.4.2/usage_examples/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.305926 spacy-llm-0.4.2/usage_examples/multitask_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/multitask_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1244 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/multitask_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.305926 spacy-llm-0.4.2/usage_examples/ner_dolly/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/ner_dolly/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/ner_dolly/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.309926 spacy-llm-0.4.2/usage_examples/ner_langchain_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/ner_langchain_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/ner_langchain_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.309926 spacy-llm-0.4.2/usage_examples/rel_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/rel_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1337 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/rel_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.309926 spacy-llm-0.4.2/usage_examples/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3361 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/tests/test_readme_examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2608 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/tests/test_usage_examples.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-14 09:43:35.309926 spacy-llm-0.4.2/usage_examples/textcat_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/textcat_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1173 2023-07-14 09:43:21.000000 spacy-llm-0.4.2/usage_examples/textcat_openai/run_pipeline.py
```

### Comparing `spacy-llm-0.4.1/LICENSE` & `spacy-llm-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/PKG-INFO` & `spacy-llm-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-llm
-Version: 0.4.1
+Version: 0.4.2
 Summary: Integrating LLMs into structured NLP pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
 Project-URL: Source, https://github.com/explosion/spacy-llm
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-llm Version: 0.4.1 Summary: Integrating LLMs
+Metadata-Version: 2.1 Name: spacy-llm Version: 0.4.2 Summary: Integrating LLMs
 into structured NLP pipelines Author: Explosion Author-email:
 contact@explosion.ai License: MIT Project-URL: Release notes, https://
 github.com/explosion/spacy-llm/releases Project-URL: Source, https://
 github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
```

### Comparing `spacy-llm-0.4.1/README.md` & `spacy-llm-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/pyproject.toml` & `spacy-llm-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/setup.cfg` & `spacy-llm-0.4.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.4.1
+version = 0.4.2
 description = Integrating LLMs into structured NLP pipelines
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `spacy-llm-0.4.1/spacy_llm/cache.py` & `spacy-llm-0.4.2/spacy_llm/cache.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/compat.py` & `spacy-llm-0.4.2/spacy_llm/compat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/models/hf/base.py` & `spacy-llm-0.4.2/spacy_llm/models/hf/base.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/models/hf/dolly.py` & `spacy-llm-0.4.2/spacy_llm/models/hf/dolly.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/models/hf/falcon.py` & `spacy-llm-0.4.2/spacy_llm/models/hf/falcon.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/models/hf/openllama.py` & `spacy-llm-0.4.2/spacy_llm/models/hf/openllama.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/models/hf/stablelm.py` & `spacy-llm-0.4.2/spacy_llm/models/hf/stablelm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/models/langchain/model.py` & `spacy-llm-0.4.2/spacy_llm/models/langchain/model.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/models/rest/anthropic/model.py` & `spacy-llm-0.4.2/spacy_llm/models/rest/anthropic/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import warnings
 from enum import Enum
 from typing import Any, Dict, Iterable, List, Sized, Tuple
 
 import requests  # type: ignore[import]
 import srsly  # type: ignore[import]
 from requests import HTTPError
 
@@ -29,25 +30,34 @@
     }
 
     @property
     def credentials(self) -> Dict[str, str]:
         # Fetch and check the key, set up headers
         api_key = os.getenv("ANTHROPIC_API_KEY")
         if api_key is None:
-            raise ValueError(
+            warnings.warn(
                 "Could not find the API key to access the Anthropic Claude API. Ensure you have an API key "
                 "set up via the Anthropic console (https://console.anthropic.com/), then make it available as "
                 "an environment variable 'ANTHROPIC_API_KEY."
             )
 
-        return {"X-API-Key": api_key}
+        return {"X-API-Key": api_key if api_key else ""}
 
     def _verify_auth(self) -> None:
         # Execute a dummy prompt. If the API setup is incorrect, we should fail at initialization time.
-        self(["test"])
+        try:
+            self(["test"])
+        except ValueError as err:
+            if "authentication_error" in str(err):
+                warnings.warn(
+                    "Authentication with provided API key failed. Please double-check you provided the correct "
+                    "credentials."
+                )
+            else:
+                raise err
 
     def __call__(self, prompts: Iterable[str]) -> Iterable[str]:
         headers = {
             **self._credentials,
             "model": self._name,
             "Content-Type": "application/json",
         }
```

### Comparing `spacy-llm-0.4.1/spacy_llm/models/rest/anthropic/registry.py` & `spacy-llm-0.4.2/spacy_llm/models/rest/anthropic/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/models/rest/base.py` & `spacy-llm-0.4.2/spacy_llm/models/rest/base.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/models/rest/cohere/model.py` & `spacy-llm-0.4.2/spacy_llm/models/rest/cohere/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import warnings
 from enum import Enum
 from typing import Any, Dict, Iterable, List, Sized, Tuple
 
 import requests  # type: ignore[import]
 import srsly  # type: ignore[import]
 from requests import HTTPError
 
@@ -14,24 +15,33 @@
 
 
 class Cohere(REST):
     @property
     def credentials(self) -> Dict[str, str]:
         api_key = os.getenv("CO_API_KEY")
         if api_key is None:
-            raise ValueError(
+            warnings.warn(
                 "Could not find the API key to access the Cohere API. Ensure you have an API key "
                 "set up via https://dashboard.cohere.ai/api-keys, then make it available as "
                 "an environment variable 'CO_API_KEY'."
             )
 
         return {"Authorization": f"Bearer {api_key}"}
 
     def _verify_auth(self) -> None:
-        self(["test"])
+        try:
+            self(["test"])
+        except ValueError as err:
+            if "invalid api token" in str(err):
+                warnings.warn(
+                    "Authentication with provided API key failed. Please double-check you provided the correct "
+                    "credentials."
+                )
+            else:
+                raise err
 
     def __call__(self, prompts: Iterable[str]) -> Iterable[str]:
         headers = {
             **self._credentials,
             "Content-Type": "application/json",
             "Accept": "application/json",
         }
```

### Comparing `spacy-llm-0.4.1/spacy_llm/models/rest/cohere/registry.py` & `spacy-llm-0.4.2/spacy_llm/models/rest/cohere/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/models/rest/noop/model.py` & `spacy-llm-0.4.2/spacy_llm/models/rest/noop/model.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/models/rest/openai/__init__.py` & `spacy-llm-0.4.2/spacy_llm/models/rest/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/models/rest/openai/model.py` & `spacy-llm-0.4.2/spacy_llm/models/rest/openai/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import warnings
 from enum import Enum
 from typing import Any, Dict, Iterable, List, Sized, Tuple
 
 import requests  # type: ignore[import]
 import srsly  # type: ignore[import]
 from requests import HTTPError
 
@@ -17,15 +18,15 @@
 class OpenAI(REST):
     @property
     def credentials(self) -> Dict[str, str]:
         # Fetch and check the key
         api_key = os.getenv("OPENAI_API_KEY")
         api_org = os.getenv("OPENAI_API_ORG")
         if api_key is None:
-            raise ValueError(
+            warnings.warn(
                 "Could not find the API key to access the OpenAI API. Ensure you have an API key "
                 "set up via https://platform.openai.com/account/api-keys, then make it available as "
                 "an environment variable 'OPENAI_API_KEY."
             )
 
         # Check the access and get a list of available models to verify the model argument (if not None)
         # Even if the model is None, this call is used as a healthcheck to verify access.
@@ -47,22 +48,28 @@
         r = self.retry(
             call_method=requests.get,
             url="https://api.openai.com/v1/models",
             headers=self._credentials,
             timeout=self._max_request_time,
         )
         if r.status_code == 422:
-            raise ValueError(
+            warnings.warn(
                 "Could not access api.openai.com -- 422 permission denied."
                 "Visit https://platform.openai.com/account/api-keys to check your API keys."
             )
         elif r.status_code != 200:
-            raise ValueError(
-                f"Error accessing api.openai.com ({r.status_code}): {r.text}"
-            )
+            if "Incorrect API key" in r.text:
+                warnings.warn(
+                    "Authentication with provided API key failed. Please double-check you provided the correct "
+                    "credentials."
+                )
+            else:
+                warnings.warn(
+                    f"Error accessing api.openai.com ({r.status_code}): {r.text}"
+                )
 
         response = r.json()["data"]
         models = [response[i]["id"] for i in range(len(response))]
         if self._name not in models:
             raise ValueError(
                 f"The specified model '{self._name}' is not available. Choices are: {sorted(set(models))}"
             )
```

### Comparing `spacy-llm-0.4.1/spacy_llm/models/rest/openai/registry.py` & `spacy-llm-0.4.2/spacy_llm/models/rest/openai/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/pipeline/llm.py` & `spacy-llm-0.4.2/spacy_llm/pipeline/llm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/registry/normalizer.py` & `spacy-llm-0.4.2/spacy_llm/registry/normalizer.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/registry/reader.py` & `spacy-llm-0.4.2/spacy_llm/registry/reader.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/__init__.py` & `spacy-llm-0.4.2/spacy_llm/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/lemma.py` & `spacy-llm-0.4.2/spacy_llm/tasks/lemma.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/ner.py` & `spacy-llm-0.4.2/spacy_llm/tasks/ner.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/noop.py` & `spacy-llm-0.4.2/spacy_llm/tasks/noop.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/rel.py` & `spacy-llm-0.4.2/spacy_llm/tasks/rel.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,35 +156,39 @@
                 labels=list(self._label_dict.values()),
                 label_definitions=self._label_definitions,
                 examples=self._prompt_examples,
                 preannotate=_preannotate,
             )
             yield prompt
 
-    def _format_response(self, response: str) -> List[RelationItem]:
+    def _format_response(self, response: str, doc: Doc) -> List[RelationItem]:
         """Parse raw string response into a structured format"""
         relations = []
         for line in response.strip().split("\n"):
             try:
-                relations.append(RelationItem.parse_raw(line))
+                rel_item = RelationItem.parse_raw(line)
+                if 0 <= rel_item.dep < len(doc.ents) and 0 <= rel_item.dest < len(
+                    doc.ents
+                ):
+                    relations.append(rel_item)
             except ValidationError:
                 msg.warn(
                     "Validation issue",
                     line,
                     show=self._verbose,
                 )
         return relations
 
     def parse_responses(
         self, docs: Iterable[Doc], responses: Iterable[str]
     ) -> Iterable[Doc]:
         self._check_rel_extension()
 
         for doc, prompt_response in zip(docs, responses):
-            rels = self._format_response(prompt_response)
+            rels = self._format_response(prompt_response, doc)
             doc._.rel = rels
             yield doc
 
     def initialize(
         self,
         get_examples: Callable[[], Iterable["Example"]],
         nlp: Language,
```

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/sentiment.py` & `spacy-llm-0.4.2/spacy_llm/tasks/sentiment.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/span.py` & `spacy-llm-0.4.2/spacy_llm/tasks/span.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/spancat.py` & `spacy-llm-0.4.2/spacy_llm/tasks/spancat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/summarization.py` & `spacy-llm-0.4.2/spacy_llm/tasks/summarization.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/templates/lemma.jinja` & `spacy-llm-0.4.2/spacy_llm/tasks/templates/lemma.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/templates/ner.jinja` & `spacy-llm-0.4.2/spacy_llm/tasks/templates/ner.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/templates/ner.v2.jinja` & `spacy-llm-0.4.2/spacy_llm/tasks/templates/ner.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/templates/rel.jinja` & `spacy-llm-0.4.2/spacy_llm/tasks/templates/rel.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/templates/sentiment.jinja` & `spacy-llm-0.4.2/spacy_llm/tasks/templates/sentiment.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/templates/spancat.jinja` & `spacy-llm-0.4.2/spacy_llm/tasks/templates/spancat.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/templates/spancat.v2.jinja` & `spacy-llm-0.4.2/spacy_llm/tasks/templates/spancat.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/templates/summarization.jinja` & `spacy-llm-0.4.2/spacy_llm/tasks/templates/summarization.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/templates/textcat.jinja` & `spacy-llm-0.4.2/spacy_llm/tasks/templates/textcat.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/templates/textcat.v2.jinja` & `spacy-llm-0.4.2/spacy_llm/tasks/templates/textcat.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/templates/textcat.v3.jinja` & `spacy-llm-0.4.2/spacy_llm/tasks/templates/textcat.v3.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/textcat.py` & `spacy-llm-0.4.2/spacy_llm/tasks/textcat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/util/parsing.py` & `spacy-llm-0.4.2/spacy_llm/tasks/util/parsing.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tasks/util/serialization.py` & `spacy-llm-0.4.2/spacy_llm/tasks/util/serialization.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/conftest.py` & `spacy-llm-0.4.2/spacy_llm/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/models/test_anthropic.py` & `spacy-llm-0.4.2/spacy_llm/tests/models/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/models/test_cohere.py` & `spacy-llm-0.4.2/spacy_llm/tests/models/test_cohere.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/models/test_dolly.py` & `spacy-llm-0.4.2/spacy_llm/tests/models/test_dolly.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/models/test_falcon.py` & `spacy-llm-0.4.2/spacy_llm/tests/models/test_falcon.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/models/test_langchain.py` & `spacy-llm-0.4.2/spacy_llm/tests/models/test_langchain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/models/test_openllama.py` & `spacy-llm-0.4.2/spacy_llm/tests/models/test_openllama.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/models/test_rest.py` & `spacy-llm-0.4.2/spacy_llm/tests/models/test_rest.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/models/test_stablelm.py` & `spacy-llm-0.4.2/spacy_llm/tests/models/test_stablelm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/pipeline/test_llm.py` & `spacy-llm-0.4.2/spacy_llm/tests/pipeline/test_llm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/lemma.json` & `spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/lemma.json`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/lemma.jsonl` & `spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/lemma.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/lemma.yml` & `spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/lemma.yml`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/rel.jsonl` & `spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/rel.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/summarization.json` & `spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/summarization.json`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/summarization.jsonl` & `spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/summarization.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/summarization.yml` & `spacy-llm-0.4.2/spacy_llm/tests/tasks/examples/summarization.yml`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/tasks/test_lemma.py` & `spacy-llm-0.4.2/spacy_llm/tests/tasks/test_lemma.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/tasks/test_ner.py` & `spacy-llm-0.4.2/spacy_llm/tests/tasks/test_ner.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/tasks/test_rel.py` & `spacy-llm-0.4.2/spacy_llm/tests/tasks/test_rel.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import json
 from pathlib import Path
 
 import pytest
 from confection import Config
 from pytest import FixtureRequest
-from spacy.tokens import Span
+from spacy.tokens import Doc, Span
 from spacy.training import Example
+from spacy.util import get_lang_class
 
 from spacy_llm.pipeline import LLMWrapper
-from spacy_llm.tasks.rel import RelationItem, RELTask
+from spacy_llm.tasks.rel import _DEFAULT_REL_TEMPLATE, RelationItem, RELTask
 from spacy_llm.ty import Labeled, LLMTask
 from spacy_llm.util import assemble_from_config, split_labels
 
 from ..compat import has_openai_key
 
 EXAMPLES_DIR = Path(__file__).parent / "examples"
 
@@ -226,7 +227,25 @@
     cfg = json.loads(cfgs[0].read_text())
     assert cfg["_label_dict"] == labels
 
     nlp2.from_disk(path)
     nlp3.from_bytes(nlp1.to_bytes())
 
     assert task1._label_dict == task2._label_dict == task3._label_dict == labels
+
+
+def test_incorrect_indexing():
+    """Tests whether incorrect indexing is handled properly (i. e. when the LLM response indices non-existent
+    entities).
+    """
+    task = RELTask(labels=["LivesIn", "WorksIn"], template=_DEFAULT_REL_TEMPLATE)
+
+    doc = Doc(get_lang_class("en")().vocab, words=["This", "is", "a", "test"])
+    doc.ents = [Span(doc, 0, 1, label="TEST")]
+    assert (
+        len(task._format_response('{"dep": 0, "dest": 1, "relation": "LivesIn"}', doc))
+        == 0
+    )
+    assert (
+        len(task._format_response('{"dep": 0, "dest": 0, "relation": "LivesIn"}', doc))
+        == 1
+    )
```

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/tasks/test_sentiment.py` & `spacy-llm-0.4.2/spacy_llm/tests/tasks/test_sentiment.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/tasks/test_spancat.py` & `spacy-llm-0.4.2/spacy_llm/tests/tasks/test_spancat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/tasks/test_summarization.py` & `spacy-llm-0.4.2/spacy_llm/tests/tasks/test_summarization.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/tasks/test_textcat.py` & `spacy-llm-0.4.2/spacy_llm/tests/tasks/test_textcat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/test_cache.py` & `spacy-llm-0.4.2/spacy_llm/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/tests/test_combinations.py` & `spacy-llm-0.4.2/spacy_llm/tests/test_combinations.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/ty.py` & `spacy-llm-0.4.2/spacy_llm/ty.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm/util.py` & `spacy-llm-0.4.2/spacy_llm/util.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/spacy_llm.egg-info/PKG-INFO` & `spacy-llm-0.4.2/spacy_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-llm
-Version: 0.4.1
+Version: 0.4.2
 Summary: Integrating LLMs into structured NLP pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
 Project-URL: Source, https://github.com/explosion/spacy-llm
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-llm Version: 0.4.1 Summary: Integrating LLMs
+Metadata-Version: 2.1 Name: spacy-llm Version: 0.4.2 Summary: Integrating LLMs
 into structured NLP pipelines Author: Explosion Author-email:
 contact@explosion.ai License: MIT Project-URL: Release notes, https://
 github.com/explosion/spacy-llm/releases Project-URL: Source, https://
 github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
```

### Comparing `spacy-llm-0.4.1/spacy_llm.egg-info/SOURCES.txt` & `spacy-llm-0.4.2/spacy_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/usage_examples/multitask_openai/run_pipeline.py` & `spacy-llm-0.4.2/usage_examples/multitask_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/usage_examples/ner_dolly/run_pipeline.py` & `spacy-llm-0.4.2/usage_examples/ner_dolly/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/usage_examples/ner_langchain_openai/run_pipeline.py` & `spacy-llm-0.4.2/usage_examples/ner_langchain_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/usage_examples/rel_openai/run_pipeline.py` & `spacy-llm-0.4.2/usage_examples/rel_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/usage_examples/tests/test_readme_examples.py` & `spacy-llm-0.4.2/usage_examples/tests/test_readme_examples.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/usage_examples/tests/test_usage_examples.py` & `spacy-llm-0.4.2/usage_examples/tests/test_usage_examples.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.1/usage_examples/textcat_openai/run_pipeline.py` & `spacy-llm-0.4.2/usage_examples/textcat_openai/run_pipeline.py`

 * *Files identical despite different names*

