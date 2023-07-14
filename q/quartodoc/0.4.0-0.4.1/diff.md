# Comparing `tmp/quartodoc-0.4.0.tar.gz` & `tmp/quartodoc-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quartodoc-0.4.0.tar", last modified: Wed Jul 12 22:53:10 2023, max compression
+gzip compressed data, was "quartodoc-0.4.1.tar", last modified: Fri Jul 14 17:58:19 2023, max compression
```

## Comparing `quartodoc-0.4.0.tar` & `quartodoc-0.4.1.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.818970 quartodoc-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.798969 quartodoc-0.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-12 22:52:56.000000 quartodoc-0.4.0/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.798969 quartodoc-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-12 22:52:56.000000 quartodoc-0.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-12 22:52:56.000000 quartodoc-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-12 22:52:56.000000 quartodoc-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-12 22:52:56.000000 quartodoc-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-12 22:52:56.000000 quartodoc-0.4.0/MAINTAINERS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-12 22:52:56.000000 quartodoc-0.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-12 22:53:10.818970 quartodoc-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-12 22:52:56.000000 quartodoc-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-12 22:52:56.000000 quartodoc-0.4.0/README.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.794968 quartodoc-0.4.0/_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.798969 quartodoc-0.4.0/_extensions/interlinks/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 22:52:56.000000 quartodoc-0.4.0/_extensions/interlinks/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-12 22:52:56.000000 quartodoc-0.4.0/_extensions/interlinks/_extension.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-12 22:52:56.000000 quartodoc-0.4.0/_extensions/interlinks/interlinks.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.802969 quartodoc-0.4.0/case_studies/
--rw-r--r--   0 runner    (1001) docker     (123)    66407 2023-07-12 22:52:56.000000 quartodoc-0.4.0/case_studies/objects_sqla.inv
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-12 22:52:56.000000 quartodoc-0.4.0/case_studies/parsing.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-12 22:52:56.000000 quartodoc-0.4.0/case_studies/some_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-12 22:52:56.000000 quartodoc-0.4.0/case_studies/sphinx-inventory.md
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-12 22:52:56.000000 quartodoc-0.4.0/case_studies/sphinx-inventory.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.802969 quartodoc-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/about.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.802969 quartodoc-0.4.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/examples/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.806970 quartodoc-0.4.0/docs/get-started/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/advanced-layouts.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/architecture.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/basic-building.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/basic-content.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/basic-docs.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/crossrefs.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/dev-big-picture.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/dev-dataclasses.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/dev-docstrings.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/dev-prepare.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/dev-renderers.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/docstring-examples.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/docstring-style.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/extending.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/extra-build-sequence.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/interlinks.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/overview.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/get-started/sidebar.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-12 22:52:56.000000 quartodoc-0.4.0/docs/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.806970 quartodoc-0.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.806970 quartodoc-0.4.0/examples/auto-package/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/auto-package/_quarto.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.806970 quartodoc-0.4.0/examples/dascore/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/dascore/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/dascore/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/dascore/generate_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/dascore/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.806970 quartodoc-0.4.0/examples/pkgdown/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/pkgdown/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/pkgdown/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/pkgdown/objects.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.806970 quartodoc-0.4.0/examples/pkgdown/reference/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/pkgdown/reference/Builder.build.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/pkgdown/reference/Builder.qmd
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/pkgdown/reference/get_object.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/pkgdown/reference/index.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/pkgdown/reference/preview.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.806970 quartodoc-0.4.0/examples/single-page/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/single-page/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/single-page/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/single-page/objects.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.806970 quartodoc-0.4.0/examples/single-page/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/single-page/reference/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.806970 quartodoc-0.4.0/examples/weird-install/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/weird-install/_quarto.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.806970 quartodoc-0.4.0/examples/weird-install/src/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-12 22:52:56.000000 quartodoc-0.4.0/examples/weird-install/src/some_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-12 22:52:56.000000 quartodoc-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.810970 quartodoc-0.4.0/quartodoc/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/autosummary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.810970 quartodoc-0.4.0/quartodoc/builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/builder/_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/builder/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/builder/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/builder/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/builder/write.py
--rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/interlinks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.810970 quartodoc-0.4.0/quartodoc/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/renderers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20767 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/renderers/md_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.814970 quartodoc-0.4.0/quartodoc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.814970 quartodoc-0.4.0/quartodoc/tests/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/__snapshots__/test_renderers.ambr
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_alias_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.814970 quartodoc-0.4.0/quartodoc/tests/example_interlinks/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_interlinks/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_interlinks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.814970 quartodoc-0.4.0/quartodoc/tests/example_interlinks/_inv/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_interlinks/_inv/other_objects.json
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_interlinks/_quarto.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_interlinks/interlinks.lua
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_interlinks/objects.json
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_interlinks/spec.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_interlinks/test.md
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_interlinks/test.qmd
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/example_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/test_builder_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/test_interlinks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/test_renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-12 22:52:56.000000 quartodoc-0.4.0/quartodoc/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.810970 quartodoc-0.4.0/quartodoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-12 22:53:10.000000 quartodoc-0.4.0/quartodoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-12 22:53:10.000000 quartodoc-0.4.0/quartodoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 22:53:10.000000 quartodoc-0.4.0/quartodoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-12 22:53:10.000000 quartodoc-0.4.0/quartodoc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-12 22:53:10.000000 quartodoc-0.4.0/quartodoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 22:53:10.000000 quartodoc-0.4.0/quartodoc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-12 22:52:56.000000 quartodoc-0.4.0/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.798969 quartodoc-0.4.0/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 22:53:10.818970 quartodoc-0.4.0/scripts/filter-spec/
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-12 22:52:56.000000 quartodoc-0.4.0/scripts/filter-spec/generate_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-12 22:52:56.000000 quartodoc-0.4.0/scripts/filter-spec/generate_test_qmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-12 22:53:10.818970 quartodoc-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.858332 quartodoc-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.830331 quartodoc-0.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-14 17:58:06.000000 quartodoc-0.4.1/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.834331 quartodoc-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-14 17:58:06.000000 quartodoc-0.4.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-14 17:58:06.000000 quartodoc-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-14 17:58:06.000000 quartodoc-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-14 17:58:06.000000 quartodoc-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-14 17:58:06.000000 quartodoc-0.4.1/MAINTAINERS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-14 17:58:06.000000 quartodoc-0.4.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-14 17:58:19.858332 quartodoc-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-14 17:58:06.000000 quartodoc-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-14 17:58:06.000000 quartodoc-0.4.1/README.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.818331 quartodoc-0.4.1/_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.834331 quartodoc-0.4.1/_extensions/interlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 17:58:06.000000 quartodoc-0.4.1/_extensions/interlinks/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-14 17:58:06.000000 quartodoc-0.4.1/_extensions/interlinks/_extension.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-14 17:58:06.000000 quartodoc-0.4.1/_extensions/interlinks/interlinks.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.834331 quartodoc-0.4.1/case_studies/
+-rw-r--r--   0 runner    (1001) docker     (123)    66407 2023-07-14 17:58:06.000000 quartodoc-0.4.1/case_studies/objects_sqla.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-14 17:58:06.000000 quartodoc-0.4.1/case_studies/parsing.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-14 17:58:06.000000 quartodoc-0.4.1/case_studies/some_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-14 17:58:06.000000 quartodoc-0.4.1/case_studies/sphinx-inventory.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-14 17:58:06.000000 quartodoc-0.4.1/case_studies/sphinx-inventory.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.838332 quartodoc-0.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/about.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.838332 quartodoc-0.4.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/examples/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.842332 quartodoc-0.4.1/docs/get-started/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/advanced-layouts.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/architecture.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/basic-building.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/basic-content.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/basic-docs.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/crossrefs.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/dev-big-picture.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/dev-dataclasses.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/dev-docstrings.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/dev-prepare.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/dev-renderers.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/docstring-examples.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/docstring-style.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/extending.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/extra-build-sequence.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/interlinks.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/overview.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/get-started/sidebar.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-14 17:58:06.000000 quartodoc-0.4.1/docs/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.842332 quartodoc-0.4.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.842332 quartodoc-0.4.1/examples/auto-package/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/auto-package/_quarto.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.842332 quartodoc-0.4.1/examples/dascore/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/dascore/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/dascore/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/dascore/generate_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/dascore/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.842332 quartodoc-0.4.1/examples/pkgdown/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/pkgdown/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/pkgdown/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/pkgdown/objects.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.842332 quartodoc-0.4.1/examples/pkgdown/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/pkgdown/reference/Builder.build.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/pkgdown/reference/Builder.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/pkgdown/reference/get_object.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/pkgdown/reference/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/pkgdown/reference/preview.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.846331 quartodoc-0.4.1/examples/single-page/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/single-page/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/single-page/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/single-page/objects.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.846331 quartodoc-0.4.1/examples/single-page/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/single-page/reference/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.846331 quartodoc-0.4.1/examples/weird-install/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/weird-install/_quarto.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.846331 quartodoc-0.4.1/examples/weird-install/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-14 17:58:06.000000 quartodoc-0.4.1/examples/weird-install/src/some_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-14 17:58:06.000000 quartodoc-0.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.846331 quartodoc-0.4.1/quartodoc/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/autosummary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.850332 quartodoc-0.4.1/quartodoc/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/builder/_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11241 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/builder/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/builder/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/builder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/builder/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/interlinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.850332 quartodoc-0.4.1/quartodoc/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/renderers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20767 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/renderers/md_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.854332 quartodoc-0.4.1/quartodoc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.854332 quartodoc-0.4.1/quartodoc/tests/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/__snapshots__/test_renderers.ambr
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_alias_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.854332 quartodoc-0.4.1/quartodoc/tests/example_interlinks/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_interlinks/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_interlinks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.854332 quartodoc-0.4.1/quartodoc/tests/example_interlinks/_inv/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_interlinks/_inv/other_objects.json
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_interlinks/_quarto.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_interlinks/interlinks.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_interlinks/objects.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_interlinks/spec.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_interlinks/test.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_interlinks/test.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/example_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/test_builder_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/test_interlinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/test_renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-14 17:58:06.000000 quartodoc-0.4.1/quartodoc/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.850332 quartodoc-0.4.1/quartodoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-14 17:58:19.000000 quartodoc-0.4.1/quartodoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-14 17:58:19.000000 quartodoc-0.4.1/quartodoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:58:19.000000 quartodoc-0.4.1/quartodoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 17:58:19.000000 quartodoc-0.4.1/quartodoc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-14 17:58:19.000000 quartodoc-0.4.1/quartodoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 17:58:19.000000 quartodoc-0.4.1/quartodoc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-14 17:58:06.000000 quartodoc-0.4.1/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.826331 quartodoc-0.4.1/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:58:19.858332 quartodoc-0.4.1/scripts/filter-spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-14 17:58:06.000000 quartodoc-0.4.1/scripts/filter-spec/generate_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-14 17:58:06.000000 quartodoc-0.4.1/scripts/filter-spec/generate_test_qmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-14 17:58:19.858332 quartodoc-0.4.1/setup.cfg
```

### Comparing `quartodoc-0.4.0/.github/CODE_OF_CONDUCT.md` & `quartodoc-0.4.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/.github/workflows/ci.yml` & `quartodoc-0.4.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/.gitignore` & `quartodoc-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/LICENSE` & `quartodoc-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/Makefile` & `quartodoc-0.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/PKG-INFO` & `quartodoc-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quartodoc
-Version: 0.4.0
+Version: 0.4.1
 Summary: Generate API documentation with quarto.
 Home-page: https://github.com/machow/quartodoc
 Author: Michael Chow
 Author-email: michael.chow@posit.co
 License: MIT
 Keywords: documentation,quarto
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quartodoc-0.4.0/README.md` & `quartodoc-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/README.qmd` & `quartodoc-0.4.1/README.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/_extensions/interlinks/interlinks.lua` & `quartodoc-0.4.1/_extensions/interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/case_studies/objects_sqla.inv` & `quartodoc-0.4.1/case_studies/objects_sqla.inv`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/case_studies/parsing.qmd` & `quartodoc-0.4.1/case_studies/parsing.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/case_studies/some_package.py` & `quartodoc-0.4.1/case_studies/some_package.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/case_studies/sphinx-inventory.md` & `quartodoc-0.4.1/case_studies/sphinx-inventory.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/case_studies/sphinx-inventory.qmd` & `quartodoc-0.4.1/case_studies/sphinx-inventory.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/docs/_quarto.yml` & `quartodoc-0.4.1/docs/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/docs/examples/index.qmd` & `quartodoc-0.4.1/docs/examples/index.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/docs/get-started/architecture.qmd` & `quartodoc-0.4.1/docs/get-started/architecture.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/docs/get-started/basic-building.qmd` & `quartodoc-0.4.1/docs/get-started/basic-building.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/docs/get-started/basic-content.qmd` & `quartodoc-0.4.1/docs/get-started/basic-content.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/docs/get-started/basic-docs.qmd` & `quartodoc-0.4.1/docs/get-started/basic-docs.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/docs/get-started/crossrefs.qmd` & `quartodoc-0.4.1/docs/get-started/crossrefs.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/docs/get-started/dev-big-picture.qmd` & `quartodoc-0.4.1/docs/get-started/dev-big-picture.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/docs/get-started/dev-docstrings.qmd` & `quartodoc-0.4.1/docs/get-started/dev-docstrings.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/docs/get-started/dev-prepare.qmd` & `quartodoc-0.4.1/docs/get-started/dev-prepare.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/docs/get-started/dev-renderers.qmd` & `quartodoc-0.4.1/docs/get-started/dev-renderers.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/docs/get-started/docstring-examples.qmd` & `quartodoc-0.4.1/docs/get-started/docstring-examples.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/docs/get-started/extending.qmd` & `quartodoc-0.4.1/docs/get-started/extending.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/docs/get-started/extra-build-sequence.qmd` & `quartodoc-0.4.1/docs/get-started/extra-build-sequence.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/docs/get-started/interlinks.qmd` & `quartodoc-0.4.1/docs/get-started/interlinks.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/docs/get-started/overview.qmd` & `quartodoc-0.4.1/docs/get-started/overview.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/docs/get-started/sidebar.qmd` & `quartodoc-0.4.1/docs/get-started/sidebar.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/docs/styles.css` & `quartodoc-0.4.1/docs/styles.css`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/examples/dascore/_quarto.yml` & `quartodoc-0.4.1/examples/dascore/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/examples/dascore/generate_api.py` & `quartodoc-0.4.1/examples/dascore/generate_api.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/examples/pkgdown/_quarto.yml` & `quartodoc-0.4.1/examples/pkgdown/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/examples/pkgdown/objects.json` & `quartodoc-0.4.1/examples/pkgdown/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/examples/pkgdown/reference/Builder.qmd` & `quartodoc-0.4.1/examples/pkgdown/reference/Builder.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/examples/pkgdown/reference/get_object.qmd` & `quartodoc-0.4.1/examples/pkgdown/reference/get_object.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/examples/single-page/_quarto.yml` & `quartodoc-0.4.1/examples/single-page/_quarto.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/examples/single-page/objects.json` & `quartodoc-0.4.1/examples/single-page/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/examples/single-page/reference/index.qmd` & `quartodoc-0.4.1/examples/single-page/reference/index.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/__init__.py` & `quartodoc-0.4.1/quartodoc/__init__.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/__main__.py` & `quartodoc-0.4.1/quartodoc/__main__.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/ast.py` & `quartodoc-0.4.1/quartodoc/ast.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/autosummary.py` & `quartodoc-0.4.1/quartodoc/autosummary.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/builder/blueprint.py` & `quartodoc-0.4.1/quartodoc/builder/blueprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,14 +288,17 @@
 
         if not el.include_private:
             options = {k: v for k, v in options.items() if not k.startswith("_")}
 
         if not el.include_imports:
             options = {k: v for k, v in options.items() if not v.is_alias}
 
+        if not el.include_empty:
+            options = {k: v for k, v in options.items() if v.docstring is not None}
+
         # for modules, remove any Alias objects, since they were imported from
         # other places. Sphinx has a flag for this behavior, so may be good
         # to do something similar.
         # if obj.is_module:
         #    options = {k: v for k, v in options.items() if not v.is_alias}
 
         return sorted(options)
```

### Comparing `quartodoc-0.4.0/quartodoc/builder/collect.py` & `quartodoc-0.4.1/quartodoc/builder/collect.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/builder/utils.py` & `quartodoc-0.4.1/quartodoc/builder/utils.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/interlinks.py` & `quartodoc-0.4.1/quartodoc/interlinks.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/inventory.py` & `quartodoc-0.4.1/quartodoc/inventory.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/layout.py` & `quartodoc-0.4.1/quartodoc/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,16 @@
         Name of the object. This should be the path needed to import it.
     members:
         A list of members, such as attributes or methods on a class, to document.
     include_private:
         Whether to include members starting with "_"
     include_imports:
         Whether to include members that were imported from somewhere else.
+    include_empty:
+        Whether to include members with no docstring.
     include:
         (Not implemented). A list of members to include.
     exclude:
         (Not implemented). A list of members to exclude.
     dynamic:
         Whether to dynamically load docstring. By default docstrings are loaded
         using static analysis. dynamic may be a string pointing to another object,
@@ -215,14 +217,15 @@
     """
 
     kind: Literal["auto"] = "auto"
     name: str
     members: Optional[list[str]] = None
     include_private: bool = False
     include_imports: bool = False
+    include_empty: bool = False
     include: Optional[str] = None
     exclude: Optional[str] = None
     dynamic: Union[None, bool, str] = None
     children: ChoicesChildren = ChoicesChildren.embedded
     package: Union[str, None, MISSING] = MISSING()
```

### Comparing `quartodoc-0.4.0/quartodoc/renderers/base.py` & `quartodoc-0.4.1/quartodoc/renderers/base.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/renderers/md_renderer.py` & `quartodoc-0.4.1/quartodoc/renderers/md_renderer.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/tests/__snapshots__/test_renderers.ambr` & `quartodoc-0.4.1/quartodoc/tests/__snapshots__/test_renderers.ambr`

 * *Files 8% similar despite different names*

```diff
@@ -19,17 +19,15 @@
   
   ## Attributes
   
   | Name | Description |
   | --- | --- |
   | [SOME_ATTRIBUTE](#quartodoc.tests.example_class.C.SOME_ATTRIBUTE) | An attribute |
   | [some_property](#quartodoc.tests.example_class.C.some_property) | A property |
-  | [x](#quartodoc.tests.example_class.C.x) |  |
-  | [y](#quartodoc.tests.example_class.C.y) |  |
-  | [z](#quartodoc.tests.example_class.C.z) |  |
+  | [z](#quartodoc.tests.example_class.C.z) | A documented init attribute |
   
   ## Methods
   
   | Name | Description |
   | --- | --- |
   | [some_method](#quartodoc.tests.example_class.C.some_method) | A method |
   
@@ -60,17 +58,15 @@
   
   ## Attributes
   
   | Name | Description |
   | --- | --- |
   | [SOME_ATTRIBUTE](#quartodoc.tests.example_class.C.SOME_ATTRIBUTE) | An attribute |
   | [some_property](#quartodoc.tests.example_class.C.some_property) | A property |
-  | [x](#quartodoc.tests.example_class.C.x) |  |
-  | [y](#quartodoc.tests.example_class.C.y) |  |
-  | [z](#quartodoc.tests.example_class.C.z) |  |
+  | [z](#quartodoc.tests.example_class.C.z) | A documented init attribute |
   
   ## Methods
   
   | Name | Description |
   | --- | --- |
   | [some_method](#quartodoc.tests.example_class.C.some_method) | A method |
   
@@ -112,20 +108,22 @@
   | --- | --- |
   | [a_attr](#quartodoc.tests.example.a_attr) | An attribute |
   
   ## Classes
   
   | Name | Description |
   | --- | --- |
-  | [AClass](#quartodoc.tests.example.AClass) |  |
+  | [AClass](#quartodoc.tests.example.AClass) | A class |
   
   ### AClass { #quartodoc.tests.example.AClass }
   
   `tests.example.AClass()`
   
+  A class
+  
   #### Attributes
   
   | Name | Description |
   | --- | --- |
   | [a_attr](#quartodoc.tests.example.AClass.a_attr) | A class attribute |
   
   #### Methods
@@ -167,20 +165,22 @@
   | --- | --- |
   | [a_attr](#quartodoc.tests.example.a_attr) | An attribute |
   
   ## Classes
   
   | Name | Description |
   | --- | --- |
-  | [AClass](#quartodoc.tests.example.AClass) |  |
+  | [AClass](#quartodoc.tests.example.AClass) | A class |
   
   ## AClass { #quartodoc.tests.example.AClass }
   
   `tests.example.AClass()`
   
+  A class
+  
   ### Attributes
   
   | Name | Description |
   | --- | --- |
   | [a_attr](#quartodoc.tests.example.AClass.a_attr) | A class attribute |
   
   ### Methods
```

### Comparing `quartodoc-0.4.0/quartodoc/tests/example_class.py` & `quartodoc-0.4.1/quartodoc/tests/example_class.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     SOME_ATTRIBUTE: float
     """An attribute"""
 
     def __init__(self, x: str, y: int):
         self.x = x
         self.y = y
         self.z: int = 1
+        """A documented init attribute"""
 
     def some_method(self):
         """A method"""
 
     @property
     def some_property(self):
         """A property"""
```

### Comparing `quartodoc-0.4.0/quartodoc/tests/example_dynamic.py` & `quartodoc-0.4.1/quartodoc/tests/example_dynamic.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/tests/example_interlinks/interlinks.lua` & `quartodoc-0.4.1/quartodoc/tests/example_interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/tests/example_interlinks/objects.json` & `quartodoc-0.4.1/quartodoc/tests/example_interlinks/objects.json`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/tests/example_interlinks/spec.yml` & `quartodoc-0.4.1/quartodoc/tests/example_interlinks/spec.yml`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/tests/example_interlinks/test.md` & `quartodoc-0.4.1/quartodoc/tests/example_interlinks/test.md`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/tests/example_interlinks/test.qmd` & `quartodoc-0.4.1/quartodoc/tests/example_interlinks/test.qmd`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/tests/test_ast.py` & `quartodoc-0.4.1/quartodoc/tests/test_ast.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/tests/test_basic.py` & `quartodoc-0.4.1/quartodoc/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/tests/test_builder.py` & `quartodoc-0.4.1/quartodoc/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/tests/test_builder_blueprint.py` & `quartodoc-0.4.1/quartodoc/tests/test_builder_blueprint.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/tests/test_interlinks.py` & `quartodoc-0.4.1/quartodoc/tests/test_interlinks.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/tests/test_layout.py` & `quartodoc-0.4.1/quartodoc/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/tests/test_renderers.py` & `quartodoc-0.4.1/quartodoc/tests/test_renderers.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/tests/test_validation.py` & `quartodoc-0.4.1/quartodoc/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc/validation.py` & `quartodoc-0.4.1/quartodoc/validation.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/quartodoc.egg-info/PKG-INFO` & `quartodoc-0.4.1/quartodoc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quartodoc
-Version: 0.4.0
+Version: 0.4.1
 Summary: Generate API documentation with quarto.
 Home-page: https://github.com/machow/quartodoc
 Author: Michael Chow
 Author-email: michael.chow@posit.co
 License: MIT
 Keywords: documentation,quarto
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quartodoc-0.4.0/quartodoc.egg-info/SOURCES.txt` & `quartodoc-0.4.1/quartodoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/requirements-dev.txt` & `quartodoc-0.4.1/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/scripts/filter-spec/generate_files.py` & `quartodoc-0.4.1/scripts/filter-spec/generate_files.py`

 * *Files identical despite different names*

### Comparing `quartodoc-0.4.0/setup.cfg` & `quartodoc-0.4.1/setup.cfg`

 * *Files identical despite different names*

