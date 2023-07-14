# Comparing `tmp/council_ai-0.0.4.tar.gz` & `tmp/council_ai-0.0.5.tar.gz`

## Comparing `council_ai-0.0.4.tar` & `council_ai-0.0.5.tar`

### file list

```diff
@@ -1,126 +1,157 @@
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.4/Makefile
--rw-r--r--   0        0        0    34335 2020-02-02 00:00:00.000000 council_ai-0.0.4/engine_flow.png
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 council_ai-0.0.4/requirements.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/__init__.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/agent_tests/__init__.py
--rw-r--r--   0        0        0     6570 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/agent_tests/agent_tests.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/agents/__init__.py
--rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/agents/agent.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/agents/agent_chain.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/agents/agent_result.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/controllers/__init__.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/controllers/basic_controller.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/controllers/controller_base.py
--rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/controllers/llm_controller.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/core/__init__.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/core/budget.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/core/cancellation_token.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/core/chain.py
--rw-r--r--   0        0        0    14710 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/core/execution_context.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/core/execution_unit.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/core/result.py
--rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/core/runners.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/core/scorer_base.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/core/skill_base.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/evaluators/__init__.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/evaluators/basic_evaluator.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/evaluators/evaluator_base.py
--rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/evaluators/llm_evaluator.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/llm/__init__.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/llm/azure_configuration.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/llm/azure_llm.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/llm/llm_base.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/llm/llm_exception.py
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/llm/llm_message.py
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/llm/openai_configuration.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/llm/openai_llm.py
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/mocks/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/prompt/__init__.py
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/prompt/prompt_builder.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/scorer/__init__.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/scorer/llm_similarity_scorer.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/skill/__init__.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/skill/llm_skill.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/skill/google/__init__.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/skill/google/google_news_skill.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/skill/google/google_search_skill.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/skill/google/google_context/__init__.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/skill/google/google_context/context_provider.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/skill/google/google_context/google_news.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/skill/google/google_context/google_search.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/skill/google/google_context/schemas.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/utils/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/utils/env.py
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 council_ai-0.0.4/council/utils/option.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/.gitignore
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/Makefile
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/README.md
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/docker-compose.yaml
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/dockerfile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/make.bat
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/requirements.txt
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/conf.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/index.rst
--rw-r--r--   0        0        0    17142 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/_static/00_chainml_logo.png
--rw-r--r--   0        0        0    18827 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/_static/02_chainml_logo_black.png
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/concepts/key_concepts.md
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/contributing/contributing.rst
--rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/examples/langchain_llm_integration.ipynb
--rw-r--r--   0        0        0     9452 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/examples/my_first_agent.ipynb
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/getting_started/usage.rst
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/introduction/introduction.rst
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/agents.rst
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/controllers.rst
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/core.rst
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/evaluators.rst
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/llm.rst
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/runners.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/scorer.rst
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/skill.rst
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/utils.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/agents/agent.rst
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/agents/agent_result.rst
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/agent_context.rst
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/agent_message.rst
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/chain_context.rst
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/chain_history.rst
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/chat_history.rst
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/chat_message_base.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/iteration_context.rst
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/scored_agent_message.rst
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/skill_context.rst
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/skill_error_message.rst
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/skill_message.rst
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/skill_success_message.rst
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/context/user_message.rst
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/controllers/basic_controller.rst
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/controllers/controller_base.rst
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/controllers/llm_controller.rst
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/core/budget.rst
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/core/chain.rst
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/core/scorer_base.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/core/similarity_scorer_exception.rst
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/core/skill_base.rst
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/evaluators/basic_evaluator.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/evaluators/evaluator_base.rst
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/evaluators/llm_evaluator.rst
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/llm/azure_configuration.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/llm/azure_llm.rst
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/llm/llm_base.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/llm/llm_message.rst
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/llm/openai_configuration.rst
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/llm/openai_llm.rst
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/runners/parallel_for.rst
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/scorer/llm_similarity_scorer.rst
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/skill/llm_skill.rst
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/skill/google/google_news_skill.rst
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/skill/google/google_search_skill.rst
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/utils/option.rst
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 council_ai-0.0.4/docs/source/reference/utils/option_exception.rst
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 council_ai-0.0.4/stubs/GoogleNews.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 council_ai-0.0.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 council_ai-0.0.4/LICENSE
--rw-r--r--   0        0        0     9285 2020-02-02 00:00:00.000000 council_ai-0.0.4/README.md
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 council_ai-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 council_ai-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.5/Makefile
+-rw-r--r--   0        0        0    34335 2020-02-02 00:00:00.000000 council_ai-0.0.5/engine_flow.png
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 council_ai-0.0.5/requirements.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/__init__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/agent_tests/__init__.py
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/agent_tests/agent_tests.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/agents/__init__.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/agents/agent.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/agents/agent_chain.py
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/agents/agent_result.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/chains/__init__.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/chains/chain.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/contexts/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/contexts/cancellation_token.py
+-rw-r--r--   0        0        0     9517 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/contexts/execution_context.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/contexts/messages.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/controllers/__init__.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/controllers/basic_controller.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/controllers/controller_base.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/controllers/execution_unit.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/controllers/llm_controller.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/evaluators/__init__.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/evaluators/basic_evaluator.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/evaluators/evaluator_base.py
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/evaluators/llm_evaluator.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/llm/__init__.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/llm/azure_llm.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/llm/azure_llm_configuration.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/llm/llm_base.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/llm/llm_configuration_base.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/llm/llm_exception.py
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/llm/llm_message.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/llm/openai_chat_completions_llm.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/llm/openai_llm.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/llm/openai_llm_configuration.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/mocks/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/prompt/__init__.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/prompt/prompt_builder.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/__init__.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/budget.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/errrors.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/if_runner.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/loop_runner_base.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/parallel.py
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/parallel_for.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/runner_base.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/runner_executor.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/sequential.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/skill_runner_base.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/types.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/scorers/__init__.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/scorers/llm_similarity_scorer.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/scorers/scorer_base.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/scorers/scorer_exception.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/__init__.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/llm_skill.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/skill_base.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/google/__init__.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/google/google_news_skill.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/google/google_search_skill.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/google/google_context/__init__.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/google/google_context/context_provider.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/google/google_context/google_news.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/google/google_context/google_search.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/google/google_context/schemas.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/utils/__init__.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/utils/env.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/utils/option.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/utils/result.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/.gitignore
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/.readthedocs.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/Makefile
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/README.md
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/docker-compose.yaml
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/dockerfile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/make.bat
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/requirements.txt
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/conf.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/index.rst
+-rw-r--r--   0        0        0    17142 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/_static/00_chainml_logo.png
+-rw-r--r--   0        0        0    18827 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/_static/02_chainml_logo_black.png
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/contributing/contributing.md
+-rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/getting_started/first_example.ipynb
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/getting_started/installation.md
+-rw-r--r--   0        0        0    34335 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/introduction/engine_flow.png
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/introduction/key_concepts.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/introduction/key_features.md
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/introduction/welcome.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/agents.rst
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/chains.rst
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/controllers.rst
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/evaluators.rst
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/llm.rst
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/scorers.rst
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/skills.rst
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/utils.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/agents/agent.rst
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/agents/agent_result.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/chains/chain.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/agent_context.rst
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/agent_message.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/chain_context.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/chain_history.rst
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/chat_history.rst
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/chat_message_base.rst
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/chat_message_kind.rst
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/iteration_context.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/scored_agent_message.rst
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/skill_context.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/skill_error_message.rst
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/skill_message.rst
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/skill_success_message.rst
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/user_message.rst
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/controllers/basic_controller.rst
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/controllers/controller_base.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/controllers/llm_controller.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/evaluators/basic_evaluator.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/evaluators/evaluator_base.rst
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/evaluators/llm_evaluator.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/llm/azure_llm.rst
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/llm/azure_llm_configuration.rst
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/llm/llm_base.rst
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/llm/llm_configuration_base.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/llm/llm_message.rst
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/llm/llm_message_role.rst
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/llm/openai_llm.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/llm/openai_llm_configuration.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners/budget.rst
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners/errors.rst
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners/if.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners/loop_runner_base.rst
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners/parallel.rst
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners/parallel_for.rst
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners/runner_base.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners/runner_executor.rst
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners/sequential.rst
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners/skill_runner_base.rst
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/scorers/llm_similarity_scorer.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/scorers/scorer_base.rst
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/scorers/scorer_exception.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/skills/google.rst
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/skills/llm_skill.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/skills/skill_base.rst
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/skills/google/google_news_skill.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/skills/google/google_search_skill.rst
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/utils/option.rst
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/utils/option_exception.rst
+-rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/use_cases/langchain_llm_integration.ipynb
+-rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/use_cases/multi_chain_agent.ipynb
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 council_ai-0.0.5/stubs/GoogleNews.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 council_ai-0.0.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 council_ai-0.0.5/LICENSE
+-rw-r--r--   0        0        0     9277 2020-02-02 00:00:00.000000 council_ai-0.0.5/README.md
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 council_ai-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    10009 2020-02-02 00:00:00.000000 council_ai-0.0.5/PKG-INFO
```

### Comparing `council_ai-0.0.4/engine_flow.png` & `council_ai-0.0.5/engine_flow.png`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.4/council/agent_tests/agent_tests.py` & `council_ai-0.0.5/council/agent_tests/agent_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import time
 from enum import Enum
 from typing import List, Dict, Any, Sequence, Optional
 import progressbar  # type: ignore
-from council.agents import Agent
 
-from council.core import (
-    ScorerBase,
+from council.agents import Agent
+from council.runners import Budget
+from council.scorers import ScorerBase, ScorerException
+from council.contexts import (
     AgentContext,
     ChatHistory,
-    Budget,
-    ScorerException,
 )
 
 
 class AgentTestCaseOutcome(str, Enum):
     Success = "Success"
     Error = "Error"
     Unknown = "Unknown"
```

### Comparing `council_ai-0.0.4/council/agents/agent.py` & `council_ai-0.0.5/council/agents/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import logging
 from typing import List
 
-from council.core.budget import Budget
-from council.core.chain import Chain
+from council.chains import Chain
+from council.contexts import AgentContext, ChatHistory
 from council.controllers import ControllerBase, BasicController
-from council.evaluators.evaluator_base import EvaluatorBase
-from council.core.execution_context import AgentContext, ChatHistory
-from council.core.runners import new_runner_executor
+from council.evaluators import BasicEvaluator, EvaluatorBase
+from council.runners import Budget, new_runner_executor
+from council.skills import SkillBase
 from .agent_result import AgentResult
-from ..core import SkillBase
-from ..evaluators import BasicEvaluator
 
 logger = logging.getLogger(__name__)
 
 
 class Agent:
     """
     Represents an agent that executes a set of chains to interact with the environment.
@@ -86,15 +84,15 @@
             logger.info('message="agent execution ended"')
             executor.shutdown(wait=False, cancel_futures=True)
 
     @staticmethod
     def from_skill(skill: SkillBase) -> "Agent":
         """
         Helper function to create a new agent with a  :class:`.BasicController`, a
-            :class:`.BasicEvaluator` and a single :class:`.SkillBase` wrapped into a `class:.Chain`
+            :class:`.BasicEvaluator` and a single :class:`.SkillBase` wrapped into a :class:`.Chain`
 
         Parameters:
              skill(SkillBase): a skill
         Returns:
             Agent: a new instance
         """
         chain = Chain(name="BasicChain", description="basic chain", runners=[skill])
```

### Comparing `council_ai-0.0.4/council/agents/agent_chain.py` & `council_ai-0.0.5/council/agents/agent_chain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional, Any
 
 from .agent import Agent
-from council.core import Chain, AgentContext, ChainContext, Budget
-from council.core.execution_context import SkillSuccessMessage
-from council.core.runners import RunnerExecutor
+from council.chains import Chain
+from council.contexts import AgentContext, ChainContext, SkillSuccessMessage
+from council.runners import Budget, RunnerExecutor
 
 
 class AgentChain(Chain):
     def __init__(self, name: str, description: str, agent: Agent):
         super().__init__(name, description, [])
         self.agent = agent
```

### Comparing `council_ai-0.0.4/council/agents/agent_result.py` & `council_ai-0.0.5/council/agents/agent_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections.abc import Sequence
 from typing import List, Optional
 
-from council.core.execution_context import ScoredAgentMessage, AgentMessage
+from council.contexts import ScoredAgentMessage, AgentMessage
 from council.utils import Option
 
 
 class AgentResult:
     """
     Represent the execution result of an :class:`Agent`
     """
```

### Comparing `council_ai-0.0.4/council/controllers/basic_controller.py` & `council_ai-0.0.5/council/controllers/basic_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import List
 
+from council.chains import Chain
+from council.contexts import AgentContext, ScoredAgentMessage
+from council.runners import Budget
+
 from .controller_base import ControllerBase
-from council.core import AgentContext, Chain, Budget
-from council.core.execution_context import ScoredAgentMessage
-from council.core.execution_unit import ExecutionUnit
+from .execution_unit import ExecutionUnit
 
 
 class BasicController(ControllerBase):
     """a basic controller that requests all chains to be executed and returns all results"""
 
     def get_plan(self, context: AgentContext, chains: List[Chain], budget: Budget) -> List[ExecutionUnit]:
         return [ExecutionUnit(chain, budget) for chain in chains]
```

### Comparing `council_ai-0.0.4/council/controllers/controller_base.py` & `council_ai-0.0.5/council/controllers/controller_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import List
 
-from council.core.budget import Budget
-from council.core.chain import Chain
-from council.core.execution_context import AgentContext, ScoredAgentMessage
-from council.core.execution_unit import ExecutionUnit
+from council.chains import Chain
+from council.contexts import AgentContext, ScoredAgentMessage
+from council.runners import Budget
+from .execution_unit import ExecutionUnit
 
 
 class ControllerBase(ABC):
     """
     Abstract base class for an agent controller.
 
     """
```

### Comparing `council_ai-0.0.4/council/controllers/llm_controller.py` & `council_ai-0.0.5/council/controllers/llm_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
 from typing import List, Tuple
 
-from .controller_base import ControllerBase
-from council.core import AgentContext, Budget
-from council.core.chain import Chain
-from council.core.execution_context import ScoredAgentMessage
-from council.core.execution_unit import ExecutionUnit
+from council.contexts import AgentContext, ScoredAgentMessage
+from council.chains import Chain
 from council.llm import LLMMessage, LLMBase
 from council.utils import Option
+from council.runners import Budget
+
+from .controller_base import ControllerBase
+from .execution_unit import ExecutionUnit
 
 logger = logging.getLogger(__name__)
 
 
 class LLMController(ControllerBase):
     """
     A controller that uses an LLM to decide the execution plan
```

### Comparing `council_ai-0.0.4/council/core/budget.py` & `council_ai-0.0.5/council/runners/budget.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.4/council/core/chain.py` & `council_ai-0.0.5/council/chains/chain.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,11 @@
 from typing import List, Any, Optional
 
-from council.core.budget import Budget
-from council.core.execution_context import (
-    ChainContext,
-)
-
-from council.core.runners import (
-    Sequential,
-    RunnerBase,
-    RunnerExecutor,
-)
+from council.contexts import ChainContext
+from council.runners import Budget, RunnerBase, Sequential, RunnerExecutor
 
 
 class Chain:
     """
     Represents a chain of skills that can be executed in a specific order.
 
     Attributes:
@@ -62,15 +54,15 @@
     ) -> Any:
         """
         Executes the chain of skills based on the provided context, budget, and optional executor.
 
         Args:
             context (ChainContext): The context for executing the chain.
             budget (Budget): The budget for chain execution.
-            executor (Optional[SkillExecutor]): The skill executor to use for executing the chain.
+            executor (Optional[RunnerExecutor]): The skill executor to use for executing the chain.
 
         Returns:
             Any: The result of executing the chain.
 
         Raises:
             None
         """
```

### Comparing `council_ai-0.0.4/council/core/execution_context.py` & `council_ai-0.0.5/council/contexts/execution_context.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,234 +1,17 @@
-from abc import ABC, abstractmethod
-from enum import Enum
 from typing import Any, Dict, List, Optional
 
-from council.core.cancellation_token import CancellationToken
+from .messages import ChatMessageBase, UserMessage, AgentMessage, SkillMessage, ScoredAgentMessage
+from .cancellation_token import CancellationToken
 from council.utils import Option
 
 
-class ChatMessageKind(str, Enum):
-    """
-    Enum representing the kinds or categories of chat messages within a chat system or application.
-    """
-
-    User = "USER"
-    """
-    Represents a chat message from the user.
-    """
-
-    Agent = "AGENT"
-    """
-    Represents a chat message from the agent or customer support representative.
-    """
-
-    System = "SYSTEM"
-    """
-    Represents a system-generated chat message.
-    """
-
-    Skill = "SKILL"
-    """
-    Represents a chat message generated by a specific skill or functionality within the chat system.
-    """
-
-
-class ChatMessageBase(ABC):
-    """
-    base class for chat messages.
-
-    Attributes:
-        message: a text message
-        kind:the kind of message
-    """
-
-    message: str
-    kind: ChatMessageKind
-
-    def __init__(self, message: str, kind: ChatMessageKind):
-        self.message = message
-        self.kind = kind
-
-    def is_of_kind(self, kind: ChatMessageKind) -> bool:
-        return self.kind == kind
-
-    def __str__(self):
-        max_length = 50
-        message = self.message[:max_length] + "..." if len(self.message) > max_length else self.message
-        return f"Message of kind {self.kind}: {message}"
-
-
-class UserMessage(ChatMessageBase):
-    """
-    a message from the user.
-
-    Attributes:
-        message: a text message
-    """
-
-    def __init__(self, message: str):
-        super().__init__(message, ChatMessageKind.User)
-
-
-class AgentMessage(ChatMessageBase):
-    """
-    a message generated from an :class:`~council.core.Agent`.
-
-    Attributes:
-        message: a text message
-    """
-
-    data: Any
-
-    def __init__(self, message: str, data: Any):
-        super().__init__(message, ChatMessageKind.Agent)
-        self.data = data
-
-
-class ScoredAgentMessage:
-    """
-    an :class:`AgentMessage` with a scored, as returned by an :class:`~.EvaluatorBase`
-
-    Attributes:
-        message (AgentMessage): an agent message
-        score: a score reflecting the quality of the message
-    """
-
-    message: AgentMessage
-    score: float
-
-    def __init__(self, message: AgentMessage, score: float):
-        self.message = message
-        self.score = score
-
-
-class SkillMessage(ChatMessageBase):
-    """
-    Base class for a message generated by a :class:`~.SkillBase`
-    """
-
-    _skill_name: str
-    _data: Any
-
-    def __init__(self, skill_name: str, message: str, data: Any = None):
-        """
-        Initialise a new instance.
-
-        Arguments:
-            skill_name (str): name of the skill
-            message (str): a text message
-            data (Any): optional data to enrich the message
-        """
-
-        super().__init__(message, ChatMessageKind.Skill)
-        self._skill_name = skill_name
-        self._data = data
-
-    @abstractmethod
-    def is_error(self) -> bool:
-        """
-        `True` if this is a :class:`~SkillErrorMessage`, otherwise `False`
-
-        Returns:
-            bool
-        """
-        pass
-
-    @abstractmethod
-    def is_ok(self) -> bool:
-        """
-        `True` if this is a :class:`SkillSuccessMessage`, otherwise `False`
-
-        Returns:
-            bool
-        """
-        pass
-
-    @property
-    def data(self) -> Any:
-        """
-        data related to the message
-
-        Returns:
-            Any
-        """
-        return self._data
-
-    @property
-    def from_skill(self) -> str:
-        """
-        the name of the :class:`.SkillBase` that has generated the message
-
-        Returns:
-            str
-        """
-        return self._skill_name
-
-    def is_from_skill(self, skill_name: str) -> bool:
-        """
-        `True` is the message has been generated by the given :class:`.SkillBase`
-
-        Arguments:
-            skill_name (str): the skill name to check against
-
-        Returns:
-            bool
-        """
-        return self._skill_name == skill_name
-
-
-class SkillSuccessMessage(SkillMessage):
-    """
-    a message generated by a :class:`.SkillBase` when executed successfully
-    """
-
-    def __init__(self, skill_name: str, message: str, data: Any = None):
-        """
-        initialize a new instance
-
-        Parameters:
-            skill_name (str): name of the :class:`.SkillBase` that generated the message.
-            message (str): a text message.
-            data (Any): optional data related to the message
-        """
-        super().__init__(skill_name=skill_name, message=message, data=data)
-
-    def is_error(self) -> bool:
-        return False
-
-    def is_ok(self) -> bool:
-        return True
-
-
-class SkillErrorMessage(SkillMessage):
-    """
-    a message generated by a :class:`.SkillBase` when an error occurred
-    """
-
-    def __init__(self, skill_name: str, message: str, data: Any = None):
-        """
-        initialize a new instance
-
-        Parameters:
-            skill_name (str): name of the :class:`.SkillBase` that generated the message.
-            message (str): a text message.
-            data (Any): optional data related to the message
-        """
-        super().__init__(skill_name=skill_name, message=message, data=data)
-
-    def is_ok(self) -> bool:
-        return False
-
-    def is_error(self) -> bool:
-        return True
-
-
 class ChatHistory:
     """
-    represents the history of messages exchanged between the user and the :class:`~.Agent`
+    represents the history of messages exchanged between the user and the :class:`.Agent`
 
     Attributes:
         messages(list[ChatMessageBase]): list of messages
     """
 
     messages: List[ChatMessageBase] = []
 
@@ -250,15 +33,15 @@
         self.messages.append(UserMessage(message))
 
     def last_user_message(self) -> Option[UserMessage]:
         """
         get the most recent user message in the history, if any.
 
         Returns:
-            Option[UserMessage]: an :class:`council.utils.Option` with a user message, if any
+            Option[UserMessage]: an :class:`.Option` with a user message, if any
         """
         for message in reversed(self.messages):
             if isinstance(message, UserMessage):
                 return Option(message)
         return Option.none()
 
     def add_agent_message(self, message: str, data: Any = None):
@@ -273,28 +56,28 @@
         self.messages.append(AgentMessage(message, data))
 
     def last_agent_message(self) -> Option[AgentMessage]:
         """
         get the most recent agent message in the history, if any.
 
         Returns:
-            Option[AgentMessage]: an :class:`council.utils.Option` with an agent message, if any
+            Option[AgentMessage]: an :class:`.Option` with an agent message, if any
         """
 
         for message in reversed(self.messages):
             if isinstance(message, AgentMessage):
                 return Option(message)
         return Option.none()
 
     def last_message(self) -> Option[ChatMessageBase]:
         """
         get the most recent message in the history, if any.
 
         Returns:
-            Option[ChatMessageBase]: an :class:`council.utils.Option` with an agent message, if any
+            Option[ChatMessageBase]: an :class:`.Option` with an agent message, if any
         """
 
         return Option.none() if len(self.messages) == 0 else Option.some(self.messages[-1])
 
     @staticmethod
     def from_user_message(message: str) -> "ChatHistory":
         history = ChatHistory()
@@ -317,28 +100,28 @@
         self.messages = []
 
     def last_message(self) -> Option[SkillMessage]:
         """
         Get the last (most recent) message, if any, added by a :class:`.SkillBase`
 
         Returns:
-            Option[SkillMessage]: an :class:`council.utils.Option` wrapping a :class:`.SkillMessage` if any.
+            Option[SkillMessage]: an :class:`~.Option` wrapping a :class:`.SkillMessage` if any.
         """
         if len(self.messages) > 0:
             return Option(self.messages[-1])
         return Option.none()
 
     def last_message_from(self, skill: str) -> Option[SkillMessage]:
         """
         Get the last (most recent) message, if any, added by specific :class:`.SkillBase` identified by its name.
 
         Parameters:
             skill (str): the name of the skill
         Returns:
-            Option[SkillMessage]: an :class:`council.utils.Option` wrapping a :class:`.SkillMessage` if any.
+            Option[SkillMessage]: an :class:`~.Option` wrapping a :class:`.SkillMessage` if any.
         """
         for message in self.messages[::-1]:
             if message.is_from_skill(skill):
                 return Option(message)
         return Option.none()
```

### Comparing `council_ai-0.0.4/council/core/result.py` & `council_ai-0.0.5/council/utils/result.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.4/council/core/scorer_base.py` & `council_ai-0.0.5/council/scorers/scorer_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 import abc
 import logging
 from typing import Any, Dict
 
-from council.core.execution_context import AgentMessage
+from council.contexts import AgentMessage
+from .scorer_exception import ScorerException
 
-logger = logging.getLogger(__name__)
-
-
-class ScorerException(Exception):
-    """
-    Exception raised by :class:`ScorerBase`
-    """
 
-    pass
+logger = logging.getLogger(__name__)
 
 
 class ScorerBase(abc.ABC):
     """
     Base class for implementing a Scorer
     """
```

### Comparing `council_ai-0.0.4/council/core/skill_base.py` & `council_ai-0.0.5/council/skills/skill_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 from __future__ import annotations
 
 import logging
 from typing import Any
 from abc import abstractmethod
 
-from council.core.budget import Budget
-from council.core.execution_context import (
-    SkillMessage,
-    SkillErrorMessage,
-    SkillSuccessMessage,
-    SkillContext,
-)
-from council.core.runners import SkillRunnerBase, RunnerSkillError
+from council.contexts import SkillMessage, SkillErrorMessage, SkillSuccessMessage, SkillContext
+from council.runners import RunnerSkillError, SkillRunnerBase, Budget
 
 logger = logging.getLogger(__name__)
 
 
 class SkillBase(SkillRunnerBase):
     """
     Abstract base class for a skill.
```

### Comparing `council_ai-0.0.4/council/evaluators/basic_evaluator.py` & `council_ai-0.0.5/council/evaluators/basic_evaluator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from typing import List
 
-from council.core import AgentContext, Budget
-from council.evaluators.evaluator_base import EvaluatorBase
-from council.core.execution_context import (
-    ScoredAgentMessage,
-    SkillSuccessMessage,
-    AgentMessage,
-)
+from council.contexts import AgentContext, ScoredAgentMessage, SkillSuccessMessage, AgentMessage
+from council.runners.budget import Budget
+from .evaluator_base import EvaluatorBase
 
 
 class BasicEvaluator(EvaluatorBase):
     def execute(self, context: AgentContext, budget: Budget) -> List[ScoredAgentMessage]:
         result = []
         for chain_history in context.chainHistory.values():
             chain_result = chain_history[-1].messages[-1]
```

### Comparing `council_ai-0.0.4/council/evaluators/evaluator_base.py` & `council_ai-0.0.5/council/evaluators/evaluator_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from abc import ABC, abstractmethod
 from typing import List
 
-from council.core.execution_context import (
-    AgentContext,
-    ScoredAgentMessage,
-)
-from council.core.budget import Budget
+from council.contexts import AgentContext, ScoredAgentMessage
+from council.runners import Budget
 
 
 class EvaluatorBase(ABC):
     """
     Abstract base class for an agent evaluator.
 
     """
```

### Comparing `council_ai-0.0.4/council/evaluators/llm_evaluator.py` & `council_ai-0.0.5/council/evaluators/llm_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 LLMEvaluator implementation.
 
 This evaluator uses the given `LLM` to evaluate the chain's responses.
 """
 import logging
 from typing import List
 
-from council.core import AgentContext, Budget
-from council.core.execution_context import ScoredAgentMessage, AgentMessage, SkillMessage, UserMessage, Option
+from council.contexts import AgentContext, ScoredAgentMessage, AgentMessage, SkillMessage, UserMessage
 from council.evaluators import EvaluatorBase
 from council.llm import LLMBase, LLMMessage
+from council.runners import Budget
+from council.utils import Option
 
 
 class LLMEvaluator(EvaluatorBase):
     """Evaluator using an `LLM` to evaluate chain responses."""
 
     def __init__(self, llm: LLMBase):
         """
```

### Comparing `council_ai-0.0.4/council/llm/azure_llm.py` & `council_ai-0.0.5/council/llm/openai_chat_completions_llm.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 import logging
+
 import httpx
 
-from typing import List, Any
+from typing import List, Any, Protocol
 
-from .azure_configuration import AzureConfiguration
+from . import LLMConfigurationBase
 from .llm_message import LLMMessage
 from .llm_exception import LLMException
 from .llm_base import LLMBase
 
+logger = logging.getLogger(__name__)
+
+
+class Provider(Protocol):
+    def __call__(self, payload: dict[str, Any]) -> httpx.Response:
+        ...
+
 
-class AzureLLM(LLMBase):
+class OpenAIChatCompletionsModel(LLMBase):
     """
     Represents an OpenAI language model hosted on Azure.
     """
 
-    config: AzureConfiguration
+    config: LLMConfigurationBase
 
-    def __init__(self, config: AzureConfiguration):
+    def __init__(self, config: LLMConfigurationBase, provider: Provider):
         self.config = config
+        self._provider = provider
 
     def _post_chat_request(self, messages: List[LLMMessage], **kwargs: Any) -> str:
-        payload = {
-            "messages": [message.dict() for message in messages],
-            "temperature": self.config.temperature,
-        }
+        payload = self.config.build_default_payload()
+        payload["messages"] = [message.dict() for message in messages]
         for key, value in kwargs.items():
             payload[key] = value
 
-        return self.post_request(payload, **kwargs)
+        logger.debug(f'message="Sending chat GPT completions request" payload="{payload}"')
+        response = self._provider.__call__(payload)
+        return self.validate_and_parse_response(response)
 
-    def post_request(self, payload, **kwargs: Any):
-        uri = f"{self.config.api_base}/openai/deployments/{self.config.deployment_name}/chat/completions"
-        headers = {"api-key": self.config.api_key, "Content-Type": "application/json"}
-        params = {"api-version": self.config.api_version}
-        logging.debug(f'message="Sending request" payload="{payload}"')
-        with httpx.Client() as client:
-            client.timeout.read = self.config.timeout
-            response = client.post(url=uri, headers=headers, params=params, json=payload)
-            return AzureLLM.validate_and_parse_response(response)
-
-    @staticmethod
-    def validate_and_parse_response(response: httpx.Response) -> str:
+    def validate_and_parse_response(self, response: httpx.Response) -> str:
         if response.status_code != httpx.codes.OK:
             raise LLMException(f"Wrong status code: {response.status_code}. Reason: {response.text}")
-        return response.json()["choices"][0]["message"]["content"]
+        choices = response.json()["choices"]
+
+        n = self.config.n.unwrap_or(1)
+        if n <= 1:
+            return choices[0]["message"]["content"]
+
+        return "\n".join(choice["message"]["content"] for choice in choices)
```

### Comparing `council_ai-0.0.4/council/llm/llm_base.py` & `council_ai-0.0.5/council/llm/llm_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.4/council/llm/llm_message.py` & `council_ai-0.0.5/council/llm/llm_message.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 from typing import Optional, List
 
-from council.core.execution_context import ChatMessageBase, ChatMessageKind
+from council.contexts import ChatMessageBase, ChatMessageKind
 
 
 class LLMMessageRole(str, Enum):
     """
     Enum representing the roles of messages in a conversation or dialogue.
     """
 
@@ -73,29 +73,29 @@
         return LLMMessage(role=LLMMessageRole.Assistant, content=content)
 
     def dict(self) -> dict[str, str]:
         return {"role": self._role, "content": self._content}
 
     @property
     def content(self) -> str:
-        """Retrieve the content of the `LLMMessage`"""
+        """Retrieve the content of this instance"""
         return self._content
 
     @property
     def role(self) -> LLMMessageRole:
-        """Retrieve the role of the `LLMMessage`"""
+        """Retrieve the role of this instance"""
         return self._role
 
     def is_of_role(self, role: LLMMessageRole) -> bool:
-        """Check the role of the `LLMMessage`"""
+        """Check the role of this instance"""
         return self._role == role
 
     @staticmethod
     def from_chat_message(chat_message: ChatMessageBase) -> Optional["LLMMessage"]:
-        """Convert :class:`~council.core.execution_context.ChatMessageBase` into :class:`LLMMessage`"""
+        """Convert :class:`~.ChatMessageBase` into :class:`.LLMMessage`"""
         if chat_message.kind == ChatMessageKind.User:
             return LLMMessage.user_message(chat_message.message)
         elif chat_message.kind == ChatMessageKind.Agent:
             return LLMMessage.assistant_message(chat_message.message)
         return None
 
     @staticmethod
```

### Comparing `council_ai-0.0.4/council/mocks/__init__.py` & `council_ai-0.0.5/council/mocks/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import time
 import random
 from typing import List, Any, Callable, Optional, Protocol
 
 from council.agents import Agent, AgentResult
-from council.core import AgentContext, Budget, ScorerBase, SkillBase
-from council.core.execution_context import (
-    ScoredAgentMessage,
-    AgentMessage,
-    SkillContext,
-    SkillMessage,
-    SkillSuccessMessage,
-)
+from council.contexts import AgentContext, ScoredAgentMessage, AgentMessage, SkillContext, SkillMessage
 from council.llm import LLMBase, LLMMessage
+from council.runners import Budget
+from council.scorers import ScorerBase
+from council.skills import SkillBase
 
 
 class LLMMessagesToStr(Protocol):
     def __call__(self, messages: List[LLMMessage]) -> str:
         ...
```

### Comparing `council_ai-0.0.4/council/prompt/prompt_builder.py` & `council_ai-0.0.5/council/prompt/prompt_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import Any, List, Optional
 
 from jinja2 import Template
 
-from council.core import ChainContext, ChatMessageKind
+from council.contexts import ChainContext, ChatMessageKind
 
 logger = logging.getLogger(__name__)
 
 
 class PromptBuilder:
     """
     A class for building prompts using a Jinja2 template and optional instructions.
```

### Comparing `council_ai-0.0.4/council/scorer/llm_similarity_scorer.py` & `council_ai-0.0.5/council/scorers/llm_similarity_scorer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Dict, Any
 
-from council.core import ScorerBase
-from council.core.execution_context import AgentMessage
+from .scorer_base import ScorerBase
+from council.contexts import AgentMessage
 from council.llm import LLMBase, LLMMessage
 
 
 class LLMSimilarityScorer(ScorerBase):
     """
     Using an LLM to compute a similarity score between two messages.
     """
```

### Comparing `council_ai-0.0.4/council/skill/llm_skill.py` & `council_ai-0.0.5/council/skills/llm_skill.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from typing import List, Protocol
 
-from council.core import SkillBase, Budget, ChainContext
-from council.core.execution_context import SkillMessage, SkillSuccessMessage, SkillContext
+from council.contexts import ChainContext, SkillMessage, SkillSuccessMessage, SkillContext
 from council.llm import LLMBase, LLMMessage
 from council.prompt import PromptBuilder
+from council.runners import Budget
+from council.skills import SkillBase
 
 
 class ReturnMessages(Protocol):
     def __call__(self, context: SkillContext) -> List[LLMMessage]:
         ...
```

### Comparing `council_ai-0.0.4/council/skill/google/google_news_skill.py` & `council_ai-0.0.5/council/skills/google/google_news_skill.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 
-from council.core import SkillBase, Budget
-from council.core import ChainContext
-from council.core.execution_context import SkillMessage
+from council.contexts import ChainContext, SkillMessage
+from council.runners import Budget
 from .google_context import GoogleNewsSearchEngine
+from .. import SkillBase
 
 
 class GoogleNewsSkill(SkillBase):
     """
-    A skill that performs a Google news search.
+    A skill that performs a Google News search.
 
     """
 
     def __init__(self, suffix: str = ""):
         super().__init__("gnews")
         self.gn = GoogleNewsSearchEngine(period="90d", suffix=suffix)
```

### Comparing `council_ai-0.0.4/council/skill/google/google_search_skill.py` & `council_ai-0.0.5/council/skills/google/google_search_skill.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from council.core import Budget, SkillBase
-from council.core.execution_context import ChainContext, SkillMessage
-from .google_context import GoogleSearchEngine
-
 import json
 
+from council.contexts import ChainContext, SkillMessage
+from council.runners import Budget
+from .google_context import GoogleSearchEngine
+from .. import SkillBase
+
 
 class GoogleSearchSkill(SkillBase):
     """
     A skill that performs a Google search.
 
     Notes:
         * GOOGLE_API_KEY environment variable needs to be set
```

### Comparing `council_ai-0.0.4/council/skill/google/google_context/context_provider.py` & `council_ai-0.0.5/council/skills/google/google_context/context_provider.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.4/council/skill/google/google_context/google_news.py` & `council_ai-0.0.5/council/skills/google/google_context/google_news.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.4/council/skill/google/google_context/google_search.py` & `council_ai-0.0.5/council/skills/google/google_context/google_search.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC
 from typing import Optional, Any
 
-from council.utils import OptionException, read_env
+from council.utils import OptionException, read_env_str, MissingEnvVariableException
 
 from .context_provider import ContextProvider
 from .schemas import ResponseReference
 
 from googleapiclient.discovery import build
 
 
@@ -49,12 +49,12 @@
             return ResponseReference(title=title, url=url, snippet=snippet, date=None)
 
         return None
 
     @classmethod
     def from_env(cls) -> Optional["GoogleSearchEngine"]:
         try:
-            api_key = read_env("GOOGLE_API_KEY")
-            engine_id = read_env("GOOGLE_SEARCH_ENGINE_ID")
-        except OptionException:
+            api_key: str = read_env_str("GOOGLE_API_KEY").unwrap()
+            engine_id: str = read_env_str("GOOGLE_SEARCH_ENGINE_ID").unwrap()
+        except (MissingEnvVariableException, OptionException):
             return None
         return GoogleSearchEngine(api_key=api_key, engine_id=engine_id)
```

### Comparing `council_ai-0.0.4/council/skill/google/google_context/schemas.py` & `council_ai-0.0.5/council/skills/google/google_context/schemas.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.4/council/utils/option.py` & `council_ai-0.0.5/council/utils/option.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self._some = some
 
     def unwrap(self, message: Optional[str] = None) -> T:
         """
         unwrap the value in the instance.
 
         Parameters:
-            message (Optional(str)): error message to be set on the :class:`council.utils.OptionException`
+            message (Optional(str)): error message to be set on the :class:`~.OptionException`
             if there is no value to unwrap
         returns:
             T: the value
 
         raises:
             OptionException: there is no value wrapped by this instance
         """
```

### Comparing `council_ai-0.0.4/docs/Makefile` & `council_ai-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.4/docs/make.bat` & `council_ai-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.4/docs/source/conf.py` & `council_ai-0.0.5/docs/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,9 +60,10 @@
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_title = f"{project} {release}"
 html_theme = "furo"
 html_show_copyright = False
+html_show_sphinx = False
 html_static_path = ["_static"]
-html_theme_options = {"dark_logo": "00_chainml_logo.png", "light_logo": "02_chainml_logo_black.png"}
+# html_theme_options = {"dark_logo": "00_chainml_logo.png", "light_logo": "02_chainml_logo_black.png"}
```

### Comparing `council_ai-0.0.4/docs/source/index.rst` & `council_ai-0.0.5/docs/source/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,34 @@
-Welcome to Conversational AI Engine
-===================================
-
-**Council** is a Python library for developers that facilitates the creation of of advanced Chat Bot.
-
-
-.. warning::
-    This project is under active development
-
+.. include:: introduction/welcome.md
+    :parser: myst_parser.sphinx_
 
 .. toctree::
+    :caption: Introduction
     :maxdepth: 2
     :hidden:
 
-    introduction/introduction.rst
+    introduction/welcome
+    introduction/key_features
+    introduction/key_concepts
 
 .. toctree::
     :caption: Getting Started
     :maxdepth: 2
     :hidden:
 
-    getting_started/usage
-
-.. toctree::
-    :maxdepth: 2
-    :caption: Concepts
-    :hidden:
-
-    concepts/key_concepts
+    getting_started/installation
+    getting_started/first_example
 
 .. toctree::
     :maxdepth: 2
-    :caption: Examples
+    :caption: Use Cases
     :hidden:
 
-    examples/my_first_agent.ipynb
-    examples/langchain_llm_integration.ipynb
+    use_cases/multi_chain_agent.ipynb
+    use_cases/langchain_llm_integration.ipynb
 
 .. toctree::
     :maxdepth: 2
     :caption: Reference
     :name: reference
     :hidden:
     :glob:
```

### Comparing `council_ai-0.0.4/docs/source/_static/00_chainml_logo.png` & `council_ai-0.0.5/docs/source/_static/00_chainml_logo.png`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.4/docs/source/_static/02_chainml_logo_black.png` & `council_ai-0.0.5/docs/source/_static/02_chainml_logo_black.png`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.4/docs/source/examples/langchain_llm_integration.ipynb` & `council_ai-0.0.5/docs/source/use_cases/langchain_llm_integration.ipynb`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.4/docs/source/examples/my_first_agent.ipynb` & `council_ai-0.0.5/docs/source/use_cases/multi_chain_agent.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992229524911816%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Multi Chain Agent\\n')], delete: [0]}}, 2: {'source': "*

 * *            "{insert: [(0, 'from council.chains import Chain\\n'), (1, 'from council.skills import "*

 * *            "LLMSkill\\n')], delete: [1, 0]}}, 16: {'source': {insert: [(1, 'from council.runners "*

 * *            "import Budget\\n')], delete: [1]}}, 18: {'source': {insert: [(0, 'from "*

 * *            "council.contexts import AgentContext, ChatHistory\\n')], delete: [0]}}, 20: "*

 * *            "{'source': {insert:  […]*

```diff
@@ -2,15 +2,15 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "# My First Agent\n",
+                "# Multi Chain Agent\n",
                 "\n",
                 "### Introduction\n",
                 "In this notebook, we will build and test an agent capable of answering questions on different topics.\n",
                 "The agent will be composed of:\n",
                 "\n",
                 "### Agent Overview\n",
                 "- a **LLM Controller** The LLM (Language Model) Controller is responsible for selecting the relevant chains. It utilizes a specific mechanism or logic to identify the most appropriate chain based on the given question.\n",
@@ -45,16 +45,16 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
-                "from council.core import Chain\n",
-                "from council.skill import LLMSkill\n",
+                "from council.chains import Chain\n",
+                "from council.skills import LLMSkill\n",
                 "from council.llm import AzureLLM, AzureConfiguration\n",
                 "import dotenv"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -200,15 +200,15 @@
             "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "from council.agents import Agent\n",
-                "from council.core import Budget\n",
+                "from council.runners import Budget\n",
                 "\n",
                 "agent = Agent(controller=controller, chains=[finance_chain, game_chain, fake_chain], evaluator=evaluator)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -222,15 +222,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
-                "from council.core.execution_context import AgentContext, ChatHistory\n",
+                "from council.contexts import AgentContext, ChatHistory\n",
                 "\n",
                 "chat_history = ChatHistory()\n",
                 "chat_history.add_user_message(message=\"what is inflation?\")\n",
                 "# chat_history.add_user_message(\"what are the most popular video games?\")\n",
                 "# chat_history.add_user_message(\"what is the age of the captain?\")\n",
                 "context = AgentContext(chat_history=chat_history)\n",
                 "result = agent.execute(context=context, budget=Budget(20))\n",
@@ -257,15 +257,15 @@
             "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
                 "from council.agent_tests import AgentTestSuite, AgentTestCase\n",
-                "from council.scorer import LLMSimilarityScorer\n",
+                "from council.scorers import LLMSimilarityScorer\n",
                 "import json\n",
                 "\n",
                 "tests = [\n",
                 "    AgentTestCase(\n",
                 "        prompt=\"What is inflation\",\n",
                 "        scorers=[\n",
                 "            LLMSimilarityScorer(\n",
```

### Comparing `council_ai-0.0.4/stubs/GoogleNews.pyi` & `council_ai-0.0.5/stubs/GoogleNews.pyi`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.4/LICENSE` & `council_ai-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.4/README.md` & `council_ai-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 Note: Some of the features listed above are work-in-progress and due in a future release (refer to Roadmap section below).
 
 # Key Concepts
 
 Key components of the framework are shown in below image and further introduced in this section.
 
-<img src="engine_flow.png" width="800px">
+![engine flow](engine_flow.png "engine")
 
 ## Agent
 Agents encapsulate the end-to-end application logic from prompt input to final response across Controller, Evaluation and registered Chains of Skills. Agents itself can be recursively nested within other Agents in the form of AgentChains.
 
 ## Controller
 Controllers determine user intent given a prompt and prompt history and route the prompt to one or multiple of registered Chains before leveraging one or multiple Evaluators to score returned results and determine further course of action (including the ability to determine whether a revision is needed in which case Chains might be prompted again). Controllers will control whether one or multiple Chains are called, whether calls happen in series or in parallel. They will also be responsible for the distribution of compute budget to Chains and handling Chains that are not able to return results within the allocated compute budget. A State Management component will allow Controllers to save and retrieve state across user sessions. Controllers can be implemented in Python or (soon) Rust (to meet the needs of performance-critical applications).
 
@@ -64,20 +64,20 @@
 Set up your required API keys in a `.env`  (e.g. OpenAI). Refer to `.env.example` as an example. 
 
 ## Usage
 
 Import Council.
 
 ```python
-from council.core import Chain
-from council.skill import LLMSkill
+from council.chains import Chain
+from council.skills import LLMSkill
 from council.llm import OpenAILLM, OpenAIConfiguration
 ```
 
-Setup API keys in .env file (example in repository) and use it to setup the LLM (here: AzureLLM).
+Setup API keys in .env file (example in repository) and use it to setup the LLM (here: OpenAILLM).
 
 ```python
 import dotenv
 
 dotenv.load_dotenv()
 openai_llm = OpenAILLM(config=OpenAIConfiguration.from_env())
 ```
@@ -86,15 +86,15 @@
 
 ```python
 prompt = "You are responding to every prompt with a short poem titled hello world"
 hw_skill = LLMSkill(llm=openai_llm, system_prompt=prompt)
 hw_chain = Chain(name="Hello World", description="Answers with a poem about titled Hello World", runners=[hw_skill])
 ```
 
-Create a second Skill (that responds with generated Ascii art).
+Create a second Skill (that responds only with Emojis).
 
 ```python
 prompt = "You are responding to every prompt with an emoji that best addresses the question asked or statement made"
 em_skill = LLMSkill(llm=openai_llm, system_prompt=prompt)
 em_chain = Chain(name="Emoji Agent", description="Responds to every prompt with an emoji that best fits the prompt",
                  runners=[em_skill])
 ```
@@ -116,23 +116,23 @@
 ```
 
 Finalize setup of the Hello World first Agent by combining all components created.
 
 
 ```python
 from council.agents import Agent
-from council.core import Budget
 
 agent = Agent(controller=controller, chains=[hw_chain, em_chain], evaluator=evaluator)
 ```
 
 Now, we are ready to invoke the agent. The ChatHistory object is used to track message history between User and Agents.
 
 ```python
-from council.core.execution_context import AgentContext, ChatHistory
+from council.contexts import AgentContext, ChatHistory
+from council.runners import Budget
 
 chat_history = ChatHistory()
 chat_history.add_user_message(message="hello world?!")
 context = AgentContext(chat_history=chat_history)
 result = agent.execute(context=context, budget=Budget(20))
 print(result.best_message.message)
 ```
@@ -143,15 +143,15 @@
 
 ## Black
 
 Use `black .` to automatically reformat files.
 
 # Documentation
 
-A detailed documentation of Council can be found at <a href="council.dev">council.dev</a>.
+A detailed documentation of Council can be found at <a href="https://council.dev">council.dev</a>.
 
 # Roadmap
 
 We have big plans and an ambitious roadmap for the framework with incremental releases scheduled every two weeks. 
 
 Major milestones the core team is working towards are shown in below table. The roadmap is subject to frequent changes as community needs emerge. Breaking changes to our APIs are still to be expected.
```

### Comparing `council_ai-0.0.4/pyproject.toml` & `council_ai-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "council-ai"
-version = "0.0.4"
+version = "0.0.5"
 description = "Council is an open-source framework for the rapid development and robust deployment of customized generative AI applications"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = []
 license = "Apache-2.0"
 
 dynamic = ["dependencies"]
 
 [project.urls]
 Source = "https://github.com/chain-ml/council"
+Documentation = "https://council.dev"
 
 [tool.hatch.build]
 exclude = [
     ".github",
     "*-requirements.txt",
     "tests",
     "venv",
```

### Comparing `council_ai-0.0.4/PKG-INFO` & `council_ai-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: council-ai
-Version: 0.0.4
+Version: 0.0.5
 Summary: Council is an open-source framework for the rapid development and robust deployment of customized generative AI applications
 Project-URL: Source, https://github.com/chain-ml/council
+Project-URL: Documentation, https://council.dev
 License-Expression: Apache-2.0
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: google-api-python-client-stubs
 Requires-Dist: google-api-python-client==2.93.0
 Requires-Dist: googlenews==1.6.8
 Requires-Dist: httpx==0.24.1
@@ -39,15 +40,15 @@
 
 Note: Some of the features listed above are work-in-progress and due in a future release (refer to Roadmap section below).
 
 # Key Concepts
 
 Key components of the framework are shown in below image and further introduced in this section.
 
-<img src="engine_flow.png" width="800px">
+![engine flow](engine_flow.png "engine")
 
 ## Agent
 Agents encapsulate the end-to-end application logic from prompt input to final response across Controller, Evaluation and registered Chains of Skills. Agents itself can be recursively nested within other Agents in the form of AgentChains.
 
 ## Controller
 Controllers determine user intent given a prompt and prompt history and route the prompt to one or multiple of registered Chains before leveraging one or multiple Evaluators to score returned results and determine further course of action (including the ability to determine whether a revision is needed in which case Chains might be prompted again). Controllers will control whether one or multiple Chains are called, whether calls happen in series or in parallel. They will also be responsible for the distribution of compute budget to Chains and handling Chains that are not able to return results within the allocated compute budget. A State Management component will allow Controllers to save and retrieve state across user sessions. Controllers can be implemented in Python or (soon) Rust (to meet the needs of performance-critical applications).
 
@@ -83,20 +84,20 @@
 Set up your required API keys in a `.env`  (e.g. OpenAI). Refer to `.env.example` as an example. 
 
 ## Usage
 
 Import Council.
 
 ```python
-from council.core import Chain
-from council.skill import LLMSkill
+from council.chains import Chain
+from council.skills import LLMSkill
 from council.llm import OpenAILLM, OpenAIConfiguration
 ```
 
-Setup API keys in .env file (example in repository) and use it to setup the LLM (here: AzureLLM).
+Setup API keys in .env file (example in repository) and use it to setup the LLM (here: OpenAILLM).
 
 ```python
 import dotenv
 
 dotenv.load_dotenv()
 openai_llm = OpenAILLM(config=OpenAIConfiguration.from_env())
 ```
@@ -105,15 +106,15 @@
 
 ```python
 prompt = "You are responding to every prompt with a short poem titled hello world"
 hw_skill = LLMSkill(llm=openai_llm, system_prompt=prompt)
 hw_chain = Chain(name="Hello World", description="Answers with a poem about titled Hello World", runners=[hw_skill])
 ```
 
-Create a second Skill (that responds with generated Ascii art).
+Create a second Skill (that responds only with Emojis).
 
 ```python
 prompt = "You are responding to every prompt with an emoji that best addresses the question asked or statement made"
 em_skill = LLMSkill(llm=openai_llm, system_prompt=prompt)
 em_chain = Chain(name="Emoji Agent", description="Responds to every prompt with an emoji that best fits the prompt",
                  runners=[em_skill])
 ```
@@ -135,23 +136,23 @@
 ```
 
 Finalize setup of the Hello World first Agent by combining all components created.
 
 
 ```python
 from council.agents import Agent
-from council.core import Budget
 
 agent = Agent(controller=controller, chains=[hw_chain, em_chain], evaluator=evaluator)
 ```
 
 Now, we are ready to invoke the agent. The ChatHistory object is used to track message history between User and Agents.
 
 ```python
-from council.core.execution_context import AgentContext, ChatHistory
+from council.contexts import AgentContext, ChatHistory
+from council.runners import Budget
 
 chat_history = ChatHistory()
 chat_history.add_user_message(message="hello world?!")
 context = AgentContext(chat_history=chat_history)
 result = agent.execute(context=context, budget=Budget(20))
 print(result.best_message.message)
 ```
@@ -162,15 +163,15 @@
 
 ## Black
 
 Use `black .` to automatically reformat files.
 
 # Documentation
 
-A detailed documentation of Council can be found at <a href="council.dev">council.dev</a>.
+A detailed documentation of Council can be found at <a href="https://council.dev">council.dev</a>.
 
 # Roadmap
 
 We have big plans and an ambitious roadmap for the framework with incremental releases scheduled every two weeks. 
 
 Major milestones the core team is working towards are shown in below table. The roadmap is subject to frequent changes as community needs emerge. Breaking changes to our APIs are still to be expected.
```

