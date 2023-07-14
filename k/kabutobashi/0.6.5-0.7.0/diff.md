# Comparing `tmp/kabutobashi-0.6.5.tar.gz` & `tmp/kabutobashi-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kabutobashi-0.6.5.tar", last modified: Thu Mar  9 14:07:01 2023, max compression
+gzip compressed data, was "kabutobashi-0.7.0.tar", last modified: Fri Jul 14 03:44:21 2023, max compression
```

## Comparing `kabutobashi-0.6.5.tar` & `kabutobashi-0.7.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:07:01.053883 kabutobashi-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-03-09 14:07:01.053883 kabutobashi-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:07:01.049883 kabutobashi-0.6.5/kabutobashi/
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:07:01.049883 kabutobashi-0.6.5/kabutobashi/application/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/application/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/application/crawl_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/application/di_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:07:01.049883 kabutobashi-0.6.5/kabutobashi/domain/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:07:01.049883 kabutobashi-0.6.5/kabutobashi/domain/aggregates/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/aggregates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/aggregates/single_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:07:01.049883 kabutobashi-0.6.5/kabutobashi/domain/entity/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14360 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/entity/stock.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:07:01.049883 kabutobashi-0.6.5/kabutobashi/domain/services/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/analyze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:07:01.049883 kabutobashi-0.6.5/kabutobashi/domain/services/converter/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/converter/to_entity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:07:01.049883 kabutobashi-0.6.5/kabutobashi/domain/services/decode_html/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/decode_html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/decode_html/html_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/decode_html/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:07:01.053883 kabutobashi-0.6.5/kabutobashi/domain/services/method/
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/method/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/method/adx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/method/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/method/bollinger_bands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/method/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/method/ichimoku.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/method/industry_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/method/macd.py
--rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/method/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/method/momentum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/method/pct_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/method/psycho_logical.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/method/sma.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/method/stochastics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/services/method/volatility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:07:01.053883 kabutobashi-0.6.5/kabutobashi/domain/values/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/values/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/values/decoded_html_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/values/raw_html_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/values/stock_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/domain/values/user_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/example_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:07:01.053883 kabutobashi-0.6.5/kabutobashi/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:07:01.053883 kabutobashi-0.6.5/kabutobashi/infrastructure/repository/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/infrastructure/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/infrastructure/repository/html_page_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/kabutobashi/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:07:01.049883 kabutobashi-0.6.5/kabutobashi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-03-09 14:07:00.000000 kabutobashi-0.6.5/kabutobashi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-03-09 14:07:01.000000 kabutobashi-0.6.5/kabutobashi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 14:07:00.000000 kabutobashi-0.6.5/kabutobashi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-09 14:07:00.000000 kabutobashi-0.6.5/kabutobashi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-09 14:07:00.000000 kabutobashi-0.6.5/kabutobashi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-09 14:07:01.053883 kabutobashi-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:07:01.053883 kabutobashi-0.6.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:07:01.053883 kabutobashi-0.6.5/test/test_application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/test/test_application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/test/test_application/test_crawl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 14:07:01.053883 kabutobashi-0.6.5/test/test_domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/test/test_domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/test/test_domain/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/test/test_domain/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/test/test_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-03-09 14:06:48.000000 kabutobashi-0.6.5/test/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.728854 kabutobashi-0.7.0/kabutobashi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/kabutobashi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.728854 kabutobashi-0.7.0/kabutobashi/application/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/kabutobashi/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/kabutobashi/application/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/kabutobashi/application/crawl_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/kabutobashi/application/di_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/kabutobashi/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/kabutobashi/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/kabutobashi/domain/aggregates/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/kabutobashi/domain/aggregates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/kabutobashi/domain/aggregates/single_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/kabutobashi/domain/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/kabutobashi/domain/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14511 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/entity/stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/kabutobashi/domain/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/kabutobashi/domain/services/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/converter/to_entity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/kabutobashi/domain/services/decode_html/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/decode_html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/decode_html/html_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/decode_html/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/kabutobashi/domain/services/method/
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/adx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/bollinger_bands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/ichimoku.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/industry_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/macd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/momentum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/pct_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/psycho_logical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/sma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/stochastics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/volatility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/kabutobashi/domain/values/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/values/decoded_html_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/values/raw_html_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/values/stock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/values/user_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/example_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/kabutobashi/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/kabutobashi/infrastructure/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/infrastructure/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/infrastructure/repository/html_page_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.728854 kabutobashi-0.7.0/kabutobashi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-14 03:44:21.000000 kabutobashi-0.7.0/kabutobashi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-14 03:44:21.000000 kabutobashi-0.7.0/kabutobashi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 03:44:21.000000 kabutobashi-0.7.0/kabutobashi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 03:44:21.000000 kabutobashi-0.7.0/kabutobashi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 03:44:21.000000 kabutobashi-0.7.0/kabutobashi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-14 03:44:21.736854 kabutobashi-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/test/test_application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/test/test_application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/test/test_application/test_crawl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/test/test_domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/test/test_domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/test/test_domain/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/test/test_domain/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/test/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/test/test_utilities.py
```

### Comparing `kabutobashi-0.6.5/LICENSE` & `kabutobashi-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/PKG-INFO` & `kabutobashi-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kabutobashi
-Version: 0.6.5
+Version: 0.7.0
 Summary: Analyze stock
 Home-page: https://github.com/gsy0911/kabutobashi
 Author: gsy0911
 Author-email: yoshiki0911@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `kabutobashi-0.6.5/README.md` & `kabutobashi-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/__init__.py` & `kabutobashi-0.7.0/kabutobashi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 # estimate filters
 sa_fundamental = SaFundamental()
 sa_volume = SaVolume()
 
 stock_analysis = [sa_fundamental, sa_volume]
 
 # comparable tuple
-VERSION = (0, 6, 5)
+VERSION = (0, 7, 0)
 # generate __version__ via VERSION tuple
 __version__ = ".".join(map(str, VERSION))
 
 # module level doc-string
 __doc__ = """
 kabutobashi
 ===========
```

### Comparing `kabutobashi-0.6.5/kabutobashi/application/applications.py` & `kabutobashi-0.7.0/kabutobashi/application/applications.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/application/crawl_application.py` & `kabutobashi-0.7.0/kabutobashi/application/crawl_application.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/application/di_container.py` & `kabutobashi-0.7.0/kabutobashi/application/di_container.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/aggregates/single_code.py` & `kabutobashi-0.7.0/kabutobashi/domain/aggregates/single_code.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/entity/stock.py` & `kabutobashi-0.7.0/kabutobashi/domain/entity/stock.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             industry_type=data.get("industry_type"),
             market_capitalization=data.get("market_capitalization"),
             issued_shares=data.get("issued_shares"),
             is_delisting=data.get("is_delisting", False),
         )
 
     def to_dict(self) -> dict:
-        return self.dict()
+        return self.model_dump()
 
     def __eq__(self, other):
         if not isinstance(other, StockBrand):
             return False
         return self.code == other.code
 
     def __hash__(self):
@@ -120,16 +120,17 @@
             if self.market_capitalization is not None
             else other.market_capitalization,
             name=self.name if self.name is not None else other.name,
             issued_shares=self.issued_shares if self.issued_shares is not None else other.issued_shares,
             is_delisting=self.is_delisting or other.is_delisting,
         )
 
-    class Config:
-        orm_mode = True
+    # TODO modify
+    # class Config:
+    #     orm_mode = True
 
 
 class StockPriceRecord(BaseModel, IDictSerialize, IDfSerialize):
     """
     Model: Entity
     JP: 日次株価
     """
@@ -166,16 +167,15 @@
             dt=dt,
         )
 
     def is_outlier(self) -> bool:
         return self.open == 0 or self.high == 0 or self.low == 0 or self.close == 0
 
     def to_dict(self) -> dict:
-        data = self.dict()
-        del data["id"]
+        data = self.model_dump(exclude={"id"})
         return data
 
     @staticmethod
     def from_dict(data: dict) -> "StockPriceRecord":
         # code may "100.0"
         code = str(data["code"]).split(".")[0]
         return StockPriceRecord(
@@ -214,47 +214,48 @@
         if not isinstance(other, StockPriceRecord):
             return False
         return self.code == other.code and self.dt == other.dt
 
     def __hash__(self):
         return hash(self.code)
 
-    class Config:
-        orm_mode = True
+    # TODO update
+    # class Config:
+    #     orm_mode = True
 
 
 class StockReferenceIndicator(BaseModel, IDictSerialize):
     """
     Model: Entity
     JP: 参考指標
     """
 
     id: Optional[int]
     code: str = Field(description="銘柄コード")
     dt: str = Field(description="日付")
-    psr: Optional[float] = Field(description="株価売上高倍率:Price to Sales Ratio")
-    per: Optional[float] = Field(description="株価収益率:Price Earnings Ratio")
-    pbr: Optional[float] = Field(description="株価純資産倍率:Price Book-value Ratio")
-    ipo_manager: Optional[str] = Field(description="IPO_主幹")
-    ipo_evaluation: Optional[str] = Field(description="IPO_評価")
-    stock_listing_at: Optional[str] = Field(description="上場日")
-    initial_price: Optional[float] = Field(description="初値")
+    psr: Optional[float] = Field(description="株価売上高倍率:Price to Sales Ratio", default=None)
+    per: Optional[float] = Field(description="株価収益率:Price Earnings Ratio", default=None)
+    pbr: Optional[float] = Field(description="株価純資産倍率:Price Book-value Ratio", default=None)
+    ipo_manager: Optional[str] = Field(description="IPO_主幹", default=None)
+    ipo_evaluation: Optional[str] = Field(description="IPO_評価", default=None)
+    stock_listing_at: Optional[str] = Field(description="上場日", default=None)
+    initial_price: Optional[float] = Field(description="初値", default=None)
 
     def __init__(self, id: int, code: str, dt: str, psr: Optional[float], per: Optional[float], pbr: Optional[float]):
         super().__init__(
             id=id,
             code=code,
             dt=dt,
             psr=psr,
             per=per,
             pbr=pbr,
         )
 
     def to_dict(self) -> dict:
-        return self.dict()
+        return self.model_dump()
 
     @staticmethod
     def from_dict(data: dict) -> "StockReferenceIndicator":
         return StockReferenceIndicator(
             id=0,
             code=data["code"],
             dt=data["dt"],
```

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/errors.py` & `kabutobashi-0.7.0/kabutobashi/domain/errors.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/serialize.py` & `kabutobashi-0.7.0/kabutobashi/domain/serialize.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/services/analyze.py` & `kabutobashi-0.7.0/kabutobashi/domain/services/analyze.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/services/converter/to_entity.py` & `kabutobashi-0.7.0/kabutobashi/domain/services/converter/to_entity.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/services/decode_html/html_info.py` & `kabutobashi-0.7.0/kabutobashi/domain/services/decode_html/html_info.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/services/decode_html/utils.py` & `kabutobashi-0.7.0/kabutobashi/domain/services/decode_html/utils.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/services/method/__init__.py` & `kabutobashi-0.7.0/kabutobashi/domain/services/method/__init__.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/services/method/adx.py` & `kabutobashi-0.7.0/kabutobashi/domain/services/method/adx.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/services/method/basic.py` & `kabutobashi-0.7.0/kabutobashi/domain/services/method/basic.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/services/method/bollinger_bands.py` & `kabutobashi-0.7.0/kabutobashi/domain/services/method/bollinger_bands.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/services/method/fitting.py` & `kabutobashi-0.7.0/kabutobashi/domain/services/method/fitting.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/services/method/ichimoku.py` & `kabutobashi-0.7.0/kabutobashi/domain/services/method/ichimoku.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/services/method/industry_cat.py` & `kabutobashi-0.7.0/kabutobashi/domain/services/method/industry_cat.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/services/method/macd.py` & `kabutobashi-0.7.0/kabutobashi/domain/services/method/macd.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/services/method/method.py` & `kabutobashi-0.7.0/kabutobashi/domain/services/method/method.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/services/method/momentum.py` & `kabutobashi-0.7.0/kabutobashi/domain/services/method/momentum.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/services/method/pct_change.py` & `kabutobashi-0.7.0/kabutobashi/domain/services/method/pct_change.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/services/method/psycho_logical.py` & `kabutobashi-0.7.0/kabutobashi/domain/services/method/psycho_logical.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/services/method/sma.py` & `kabutobashi-0.7.0/kabutobashi/domain/services/method/sma.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/services/method/stochastics.py` & `kabutobashi-0.7.0/kabutobashi/domain/services/method/stochastics.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/services/method/volatility.py` & `kabutobashi-0.7.0/kabutobashi/domain/services/method/volatility.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/values/decoded_html_pages.py` & `kabutobashi-0.7.0/kabutobashi/domain/values/decoded_html_pages.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-from abc import ABC, abstractmethod
-from dataclasses import asdict, dataclass, field
+from abc import ABC
+
+from pydantic import BaseModel, Field, computed_field
 
-from kabutobashi.domain.serialize import IDictSerialize
 from kabutobashi.utilities import convert_float
 
+__all__ = [
+    "DecodedHtmlPage",
+    "DecodeHtmlPageStockIpo",
+    "DecodeHtmlPageStockInfoMultipleDays",
+    "DecodeHtmlPageStockInfoMinkabuTop",
+]
+
 
-@dataclass(frozen=True)
 class DecodedHtmlPage(ABC):
     """
     Model: ValueObject
     JP: 変換済みHTML
     id: code & dt
     """
 
-    def __post_init__(self):
-        self._validate()
-
-    @abstractmethod
-    def _validate(self):
-        raise NotImplementedError()  # pragma: no cover
-
 
-@dataclass(frozen=True)
-class DecodeHtmlPageStockInfoMinkabuTop(DecodedHtmlPage, IDictSerialize):
+class DecodeHtmlPageStockInfoMinkabuTop(BaseModel, DecodedHtmlPage):
     code: str
     dt: str
     name: str
     industry_type: str
     market: str
     open: str
     high: str
@@ -35,29 +33,25 @@
     unit: str
     per: str
     psr: str
     pbr: str
     volume: str
     market_capitalization: str
     issued_shares: str
-    html: str = field(repr=False)
+    html: str = Field(repr=False)
 
-    def _validate(self):
-        pass
-
-    def is_delisting(self) -> bool:
-        # 上場廃止の確認
+    @computed_field
+    @property
+    def is_delisting(self) -> int:
         if self.open == "---" and self.high == "---" and self.low == "---":
             return True
         return False
 
     def to_dict(self) -> dict:
-        data = asdict(self)
-        del data["html"]
-        return data
+        return self.model_dump(exclude={"html"})
 
     @staticmethod
     def from_dict(data: dict) -> "DecodeHtmlPageStockInfoMinkabuTop":
         return DecodeHtmlPageStockInfoMinkabuTop(
             code=data["code"],
             dt=data["dt"],
             name=data["name"],
@@ -74,35 +68,29 @@
             market_capitalization=data["market_capitalization"],
             industry_type=data["industry_type"],
             issued_shares=data["issued_shares"],
             html=data["html"],
         )
 
 
-@dataclass(frozen=True)
-class DecodeHtmlPageStockInfoMultipleDays(DecodedHtmlPage, IDictSerialize):
+class DecodeHtmlPageStockInfoMultipleDays(BaseModel, DecodedHtmlPage):
     code: str
     dt: str
     open: str
     high: str
     low: str
     close: str
     per: str
     psr: str
     pbr: str
     volume: str
-    html: str = field(repr=False)
-
-    def _validate(self):
-        pass
+    html: str = Field(repr=False)
 
     def to_dict(self) -> dict:
-        data = asdict(self)
-        del data["html"]
-        return data
+        return self.model_dump(exclude={"html"})
 
     @staticmethod
     def from_dict(data: dict) -> "DecodeHtmlPageStockInfoMultipleDays":
         return DecodeHtmlPageStockInfoMultipleDays(
             code=data["code"],
             dt=data["dt"],
             open=data["open"],
@@ -113,25 +101,21 @@
             per=data["per"],
             psr=data["psr"],
             volume=data["volume"],
             html="",
         )
 
 
-@dataclass(frozen=True)
-class DecodeHtmlPageStockIpo(DecodedHtmlPage, IDictSerialize):
-    code: str = field(metadata={"jp": "銘柄コード"})
-    manager: str = field(metadata={"jp": "主幹"})
-    stock_listing_at: str = field(metadata={"jp": "上場日"})
-    public_offering: float = field(metadata={"jp": "公募"})
-    evaluation: str = field(metadata={"jp": "評価"})
-    initial_price: float = field(metadata={"jp": "初値"})
-
-    def _validate(self):
-        pass
+class DecodeHtmlPageStockIpo(BaseModel, DecodedHtmlPage):
+    code: str = Field(description="銘柄コード")
+    manager: str = Field(description="主幹")
+    stock_listing_at: str = Field(description="上場日")
+    public_offering: float = Field(description="公募")
+    evaluation: str = Field(description="評価")
+    initial_price: float = Field(description="初値")
 
     @staticmethod
     def from_dict(data: dict) -> "DecodeHtmlPageStockIpo":
         manager = ""
         stock_listing_at = ""
         public_offering = 0
         evaluation = ""
@@ -167,8 +151,8 @@
             stock_listing_at=stock_listing_at,
             public_offering=convert_float(public_offering),
             evaluation=evaluation,
             initial_price=convert_float(initial_price),
         )
 
     def to_dict(self) -> dict:
-        return asdict(self)
+        return self.model_dump()
```

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/values/raw_html_pages.py` & `kabutobashi-0.7.0/kabutobashi/domain/values/raw_html_pages.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from abc import ABC, abstractmethod
-from dataclasses import dataclass, field
 from typing import List, NoReturn, Union
 
 from bs4 import BeautifulSoup
+from pydantic import BaseModel, Field, field_validator
 
 
-@dataclass(frozen=True)
-class RawHtmlPage:
+class RawHtmlPage(BaseModel):
     """
     Model: ValueObject
     JP: 変換対象HTML
     """
 
-    html: str = field(repr=False)
+    html: str = Field(repr=False)
     page_type: str
     url: str
 
-    def __post_init__(self):
-        assert self.page_type in ["info", "info_multiple", "ipo"]
+    @classmethod
+    @field_validator("page_type")
+    def _validate_page_type(cls, v):
+        assert v in ["info", "info_multiple", "ipo"]
 
     def get_as_soup(self) -> BeautifulSoup:
         return BeautifulSoup(self.html, features="lxml")
 
 
 class IHtmlPageRepository(ABC):
     """
@@ -43,25 +44,21 @@
         self._html_page_write(data=data)
 
     @abstractmethod
     def _html_page_write(self, data: RawHtmlPage) -> NoReturn:
         raise NotImplementedError()  # pragma: no cover
 
 
-@dataclass(frozen=True)
 class RawHtmlPageStockInfo(RawHtmlPage):
     code: Union[int, str]
 
 
-@dataclass(frozen=True)
 class RawHtmlPageStockIpo(RawHtmlPage):
     year: str
 
 
-@dataclass(frozen=True)
 class RawHtmlPageStockInfoMultipleDaysMain(RawHtmlPage):
     code: Union[int, str]
 
 
-@dataclass(frozen=True)
 class RawHtmlPageStockInfoMultipleDaysSub(RawHtmlPage):
     code: Union[int, str]
```

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/values/stock_data.py` & `kabutobashi-0.7.0/kabutobashi/domain/values/stock_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,59 @@
-from dataclasses import dataclass, field
 from typing import Any, Dict, List
 
 import matplotlib.pyplot as plt
 import pandas as pd
+from pydantic import BaseModel, ConfigDict, Field, field_validator
+from pydantic_core.core_schema import FieldValidationInfo
 
 from kabutobashi.domain.errors import KabutobashiEntityError
 
 
-@dataclass(frozen=True)
-class StockDataProcessed:
+class StockDataProcessed(BaseModel):
     """
     StockDataProcessed: ValueObject
     Holds data processed by singular-Method.
     """
 
     code: str
     start_at: str
     end_at: str
     applied_method_name: str
-    df: pd.DataFrame = field(repr=False)
-    df_required_columns: List[str] = field(repr=False)
+    df: pd.DataFrame = Field(repr=False)
+    df_required_columns: List[str] = Field(repr=False)
     parameters: Dict[str, Any]
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
-    def __post_init__(self):
-        df_columns = self.df.columns
-        if not all([c in df_columns for c in self.df_required_columns]):
+    @classmethod
+    @field_validator("df")
+    def _validate_df(cls, v, info: FieldValidationInfo):
+        df_required_columns = info.data["df_required_columns"]
+        df_columns = v.columns
+        if not all([c in df_columns for c in df_required_columns]):
             raise KabutobashiEntityError()
 
 
-@dataclass(frozen=True)
-class StockDataVisualized:
+class StockDataVisualized(BaseModel):
     """
     StockDataVisualized: ValueObject
     Used to visualize.
     """
 
     fig: plt.Figure
     size_ratio: int
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
-    def __post_init__(self):
-        if type(self.fig) is not plt.Figure:
+    @classmethod
+    @field_validator("fig")
+    def _validate_fig(cls, v):
+        if type(v) is not plt.Figure:
             raise KabutobashiEntityError()
 
 
-@dataclass(frozen=True)
-class StockDataEstimated:
+class StockDataEstimated(BaseModel):
     """
     StockDataEstimated: ValueObject
     """
 
     code: str
     estimated_value: float
     estimate_filter_name: str
```

### Comparing `kabutobashi-0.6.5/kabutobashi/domain/values/user_agent.py` & `kabutobashi-0.7.0/kabutobashi/domain/values/user_agent.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/example_data.py` & `kabutobashi-0.7.0/kabutobashi/example_data.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/infrastructure/repository/html_page_repository.py` & `kabutobashi-0.7.0/kabutobashi/infrastructure/repository/html_page_repository.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi/utilities.py` & `kabutobashi-0.7.0/kabutobashi/utilities.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/kabutobashi.egg-info/PKG-INFO` & `kabutobashi-0.7.0/kabutobashi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kabutobashi
-Version: 0.6.5
+Version: 0.7.0
 Summary: Analyze stock
 Home-page: https://github.com/gsy0911/kabutobashi
 Author: gsy0911
 Author-email: yoshiki0911@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `kabutobashi-0.6.5/kabutobashi.egg-info/SOURCES.txt` & `kabutobashi-0.7.0/kabutobashi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/pyproject.toml` & `kabutobashi-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "kabutobashi"
-version = "0.6.5"
+version = "0.7.0"
 description = ""
 authors = ["yoshiki <yoshiki0911@gmail.com>"]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
-pandas = "^1.5.0"
-requests = "^2.28.0"
-beautifulsoup4 = "^4.9.0"
-lxml = "^4.9.1"
+python = ">=3.9,<3.13"
+pandas = "^2.0.3"
+requests = "^2.31.0"
+beautifulsoup4 = "^4.12.2"
+lxml = "^4.9.3"
 jpholiday = "^0.1.8"
-matplotlib = "^3.6.3"
+matplotlib = "^3.7.2"
 mplfinance = "^0.12.7-alpha.7"
 Cerberus = "^1.3.4"
-scipy = "^1.8.0"
-pydantic = "^1.10.4"
+scipy = "^1.11.1"
+pydantic = "^2.0.2"
 injector = "^0.20.1"
 xlrd = "^2.0.1"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
```

### Comparing `kabutobashi-0.6.5/setup.py` & `kabutobashi-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/test/conftest.py` & `kabutobashi-0.7.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/test/test_application/test_crawl.py` & `kabutobashi-0.7.0/test/test_application/test_crawl.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/test/test_domain/test_entities.py` & `kabutobashi-0.7.0/test/test_domain/test_entities.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/test/test_domain/test_methods.py` & `kabutobashi-0.7.0/test/test_domain/test_methods.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/test/test_page.py` & `kabutobashi-0.7.0/test/test_page.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.6.5/test/test_utilities.py` & `kabutobashi-0.7.0/test/test_utilities.py`

 * *Files identical despite different names*

