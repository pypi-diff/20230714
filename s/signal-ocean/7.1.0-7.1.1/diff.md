# Comparing `tmp/signal-ocean-7.1.0.tar.gz` & `tmp/signal-ocean-7.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signal-ocean-7.1.0.tar", last modified: Tue Jul 11 15:10:05 2023, max compression
+gzip compressed data, was "signal-ocean-7.1.1.tar", last modified: Fri Jul 14 10:44:17 2023, max compression
```

## Comparing `signal-ocean-7.1.0.tar` & `signal-ocean-7.1.1.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2175 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1184 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)       30 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-11 15:10:05.677616 signal-ocean-7.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1524 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.661617 signal-ocean-7.1.0/signal_ocean/
--rw-r--r--   0 root         (0) root         (0)     1151 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/_internals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.665617 signal-ocean-7.1.0/signal_ocean/companies/
--rw-r--r--   0 root         (0) root         (0)      236 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/companies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1768 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/companies/companies_api.py
--rw-r--r--   0 root         (0) root         (0)     3020 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/companies/models.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.665617 signal-ocean-7.1.0/signal_ocean/distances/
--rw-r--r--   0 root         (0) root         (0)     1210 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/distances/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2523 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/distances/_distances_json.py
--rw-r--r--   0 root         (0) root         (0)    11714 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/distances/distances_api.py
--rw-r--r--   0 root         (0) root         (0)      287 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/distances/loading_condition.py
--rw-r--r--   0 root         (0) root         (0)     4589 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/distances/models.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/distances/port.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/distances/port_filter.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/distances/vessel_class.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/distances/vessel_class_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.665617 signal-ocean-7.1.0/signal_ocean/freight_pricing/
--rw-r--r--   0 root         (0) root         (0)     1318 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1113 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/_freight_pricing_json.py
--rw-r--r--   0 root         (0) root         (0)     4766 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/freight_pricing_api.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/models.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/port.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/port_filter.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/vessel_class.py
--rw-r--r--   0 root         (0) root         (0)      897 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/vessel_class_filter.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/vessel_subclass.py
--rw-r--r--   0 root         (0) root         (0)      263 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/vessel_type.py
--rw-r--r--   0 root         (0) root         (0)      877 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_pricing/vessel_type_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.665617 signal-ocean-7.1.0/signal_ocean/freight_rates/
--rw-r--r--   0 root         (0) root         (0)      565 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_rates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2145 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_rates/_freight_rates_json.py
--rw-r--r--   0 root         (0) root         (0)      524 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_rates/enums.py
--rw-r--r--   0 root         (0) root         (0)     3750 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_rates/freight_rates_api.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_rates/models.py
--rw-r--r--   0 root         (0) root         (0)      793 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_rates/port_filter.py
--rw-r--r--   0 root         (0) root         (0)     1278 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/freight_rates/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.665617 signal-ocean-7.1.0/signal_ocean/geos/
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/geos/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4338 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/geos/geos_api.py
--rw-r--r--   0 root         (0) root         (0)     6299 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/geos/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.669617 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/
--rw-r--r--   0 root         (0) root         (0)     2261 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/_historical_tonnage_list_json.py
--rw-r--r--   0 root         (0) root         (0)      331 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/area.py
--rw-r--r--   0 root         (0) root         (0)     2537 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/column.py
--rw-r--r--   0 root         (0) root         (0)      675 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/commercial_status.py
--rw-r--r--   0 root         (0) root         (0)      235 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/fixture_type.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/historical_tonnage_list.py
--rw-r--r--   0 root         (0) root         (0)     4968 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/historical_tonnage_list_api.py
--rw-r--r--   0 root         (0) root         (0)      208 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/index_level.py
--rw-r--r--   0 root         (0) root         (0)      493 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/location_taxonomy.py
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/market_deployment.py
--rw-r--r--   0 root         (0) root         (0)     1292 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/operational_status.py
--rw-r--r--   0 root         (0) root         (0)      510 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/push_type.py
--rw-r--r--   0 root         (0) root         (0)      552 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/tonnage_list.py
--rw-r--r--   0 root         (0) root         (0)     5517 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/vessel.py
--rw-r--r--   0 root         (0) root         (0)     6831 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/vessel_filter.py
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/vessel_subclass.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.669617 signal-ocean-7.1.0/signal_ocean/market_rates/
--rw-r--r--   0 root         (0) root         (0)      536 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/market_rates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1909 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/market_rates/_market_rates_json.py
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/market_rates/enums.py
--rw-r--r--   0 root         (0) root         (0)     4006 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/market_rates/market_rates_api.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/market_rates/models.py
--rw-r--r--   0 root         (0) root         (0)      773 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/market_rates/utils.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/market_rates/vessel_classes.py
--rw-r--r--   0 root         (0) root         (0)     2299 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/plots.py
--rw-r--r--   0 root         (0) root         (0)      578 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/port.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/port_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.669617 signal-ocean-7.1.0/signal_ocean/port_congestion/
--rw-r--r--   0 root         (0) root         (0)      347 2023-07-11 15:09:06.000000 signal-ocean-7.1.0/signal_ocean/port_congestion/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4274 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/port_congestion/models.py
--rw-r--r--   0 root         (0) root         (0)    19251 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/port_congestion/port_congestion.py
--rw-r--r--   0 root         (0) root         (0)     4670 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/port_congestion/port_congestion_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.669617 signal-ocean-7.1.0/signal_ocean/port_expenses/
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/port_expenses/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1433 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/port_expenses/_port_expenses_json.py
--rw-r--r--   0 root         (0) root         (0)      823 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/port_expenses/enums.py
--rw-r--r--   0 root         (0) root         (0)     1867 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/port_expenses/models.py
--rw-r--r--   0 root         (0) root         (0)     8527 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/port_expenses/port_expenses_api.py
--rw-r--r--   0 root         (0) root         (0)      779 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/port_expenses/port_filter.py
--rw-r--r--   0 root         (0) root         (0)     1147 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/port_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.669617 signal-ocean-7.1.0/signal_ocean/scraped_cargoes/
--rw-r--r--   0 root         (0) root         (0)      277 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_cargoes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26586 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_cargoes/models.py
--rw-r--r--   0 root         (0) root         (0)     5363 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_cargoes/scraped_cargoes_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.669617 signal-ocean-7.1.0/signal_ocean/scraped_data/
--rw-r--r--   0 root         (0) root         (0)       41 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4560 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_data/scraped_data_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.669617 signal-ocean-7.1.0/signal_ocean/scraped_fixtures/
--rw-r--r--   0 root         (0) root         (0)      291 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32666 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_fixtures/models.py
--rw-r--r--   0 root         (0) root         (0)     6009 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_fixtures/scraped_fixtures_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/signal_ocean/scraped_lineups/
--rw-r--r--   0 root         (0) root         (0)      281 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_lineups/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21114 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_lineups/models.py
--rw-r--r--   0 root         (0) root         (0)     5968 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_lineups/scraped_lineups_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/signal_ocean/scraped_positions/
--rw-r--r--   0 root         (0) root         (0)      301 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_positions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16973 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_positions/models.py
--rw-r--r--   0 root         (0) root         (0)     6044 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/scraped_positions/scraped_positions_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/signal_ocean/tonnage_list/
--rw-r--r--   0 root         (0) root         (0)      879 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/tonnage_list/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3345 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/tonnage_list/_json.py
--rw-r--r--   0 root         (0) root         (0)     6084 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/tonnage_list/api.py
--rw-r--r--   0 root         (0) root         (0)     7229 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/tonnage_list/data_frame.py
--rw-r--r--   0 root         (0) root         (0)    26447 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/tonnage_list/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/signal_ocean/util/
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6505 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/util/parsing_helpers.py
--rw-r--r--   0 root         (0) root         (0)     6529 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/util/request_helpers.py
--rw-r--r--   0 root         (0) root         (0)      647 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessel_class.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessel_class_api.py
--rw-r--r--   0 root         (0) root         (0)     1296 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessel_class_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/signal_ocean/vessel_emissions/
--rw-r--r--   0 root         (0) root         (0)      761 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessel_emissions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14765 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessel_emissions/models.py
--rw-r--r--   0 root         (0) root         (0)    13047 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessel_emissions/vessel_emissions_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/signal_ocean/vessel_valuations/
--rw-r--r--   0 root         (0) root         (0)      298 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessel_valuations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      595 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessel_valuations/_valuation_json.py
--rw-r--r--   0 root         (0) root         (0)      608 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessel_valuations/models.py
--rw-r--r--   0 root         (0) root         (0)     2679 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessel_valuations/vessel_valuations_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/signal_ocean/vessels/
--rw-r--r--   0 root         (0) root         (0)      378 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessels/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17416 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessels/models.py
--rw-r--r--   0 root         (0) root         (0)     3539 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/vessels/vessels_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/signal_ocean/voyages/
--rw-r--r--   0 root         (0) root         (0)     1298 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/voyages/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46003 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/voyages/models.py
--rw-r--r--   0 root         (0) root         (0)    44702 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/voyages/voyages_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.673617 signal-ocean-7.1.0/signal_ocean/voyages_market_data/
--rw-r--r--   0 root         (0) root         (0)      539 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/voyages_market_data/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15350 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/voyages_market_data/models.py
--rw-r--r--   0 root         (0) root         (0)    15865 2023-07-11 15:09:07.000000 signal-ocean-7.1.0/signal_ocean/voyages_market_data/voyages_market_data_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:10:05.665617 signal-ocean-7.1.0/signal_ocean.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2175 2023-07-11 15:10:05.000000 signal-ocean-7.1.0/signal_ocean.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5081 2023-07-11 15:10:05.000000 signal-ocean-7.1.0/signal_ocean.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 15:10:05.000000 signal-ocean-7.1.0/signal_ocean.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      124 2023-07-11 15:10:05.000000 signal-ocean-7.1.0/signal_ocean.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 15:10:05.000000 signal-ocean-7.1.0/signal_ocean.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.880928 signal-ocean-7.1.1/
+-rw-rw-r--   0 root         (0) root         (0)    11357 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2175 2023-07-14 10:44:17.880928 signal-ocean-7.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1184 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/README.md
+-rw-rw-r--   0 root         (0) root         (0)       30 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       73 2023-07-14 10:44:17.880928 signal-ocean-7.1.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1524 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.868927 signal-ocean-7.1.1/signal_ocean/
+-rw-rw-r--   0 root         (0) root         (0)     1151 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1886 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/_internals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.868927 signal-ocean-7.1.1/signal_ocean/companies/
+-rw-rw-r--   0 root         (0) root         (0)      236 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/companies/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1768 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/companies/companies_api.py
+-rw-rw-r--   0 root         (0) root         (0)     3020 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/companies/models.py
+-rw-rw-r--   0 root         (0) root         (0)     2511 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.868927 signal-ocean-7.1.1/signal_ocean/distances/
+-rw-rw-r--   0 root         (0) root         (0)     1210 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/distances/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2523 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/distances/_distances_json.py
+-rw-rw-r--   0 root         (0) root         (0)    11714 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/distances/distances_api.py
+-rw-rw-r--   0 root         (0) root         (0)      287 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/distances/loading_condition.py
+-rw-rw-r--   0 root         (0) root         (0)     4589 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/distances/models.py
+-rw-rw-r--   0 root         (0) root         (0)      266 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/distances/port.py
+-rw-rw-r--   0 root         (0) root         (0)      777 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/distances/port_filter.py
+-rw-rw-r--   0 root         (0) root         (0)      306 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/distances/vessel_class.py
+-rw-rw-r--   0 root         (0) root         (0)      897 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/distances/vessel_class_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.868927 signal-ocean-7.1.1/signal_ocean/freight_pricing/
+-rw-rw-r--   0 root         (0) root         (0)     1318 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1113 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/_freight_pricing_json.py
+-rw-rw-r--   0 root         (0) root         (0)     4766 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/freight_pricing_api.py
+-rw-rw-r--   0 root         (0) root         (0)     1274 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/models.py
+-rw-rw-r--   0 root         (0) root         (0)      266 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/port.py
+-rw-rw-r--   0 root         (0) root         (0)      777 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/port_filter.py
+-rw-rw-r--   0 root         (0) root         (0)      306 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/vessel_class.py
+-rw-rw-r--   0 root         (0) root         (0)      897 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/vessel_class_filter.py
+-rw-rw-r--   0 root         (0) root         (0)      167 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/vessel_subclass.py
+-rw-rw-r--   0 root         (0) root         (0)      263 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/vessel_type.py
+-rw-rw-r--   0 root         (0) root         (0)      877 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_pricing/vessel_type_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.872928 signal-ocean-7.1.1/signal_ocean/freight_rates/
+-rw-rw-r--   0 root         (0) root         (0)      565 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_rates/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2145 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_rates/_freight_rates_json.py
+-rw-rw-r--   0 root         (0) root         (0)      524 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_rates/enums.py
+-rw-rw-r--   0 root         (0) root         (0)     3750 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_rates/freight_rates_api.py
+-rw-rw-r--   0 root         (0) root         (0)     1820 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_rates/models.py
+-rw-rw-r--   0 root         (0) root         (0)      793 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_rates/port_filter.py
+-rw-rw-r--   0 root         (0) root         (0)     1278 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/freight_rates/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.872928 signal-ocean-7.1.1/signal_ocean/geos/
+-rw-rw-r--   0 root         (0) root         (0)      132 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/geos/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4338 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/geos/geos_api.py
+-rw-rw-r--   0 root         (0) root         (0)     6299 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/geos/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.872928 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/
+-rw-rw-r--   0 root         (0) root         (0)     2261 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2559 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/_historical_tonnage_list_json.py
+-rw-rw-r--   0 root         (0) root         (0)      331 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/area.py
+-rw-rw-r--   0 root         (0) root         (0)     2537 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/column.py
+-rw-rw-r--   0 root         (0) root         (0)      675 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/commercial_status.py
+-rw-rw-r--   0 root         (0) root         (0)      235 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/fixture_type.py
+-rw-rw-r--   0 root         (0) root         (0)     2105 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/historical_tonnage_list.py
+-rw-rw-r--   0 root         (0) root         (0)     4968 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/historical_tonnage_list_api.py
+-rw-rw-r--   0 root         (0) root         (0)      208 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/index_level.py
+-rw-rw-r--   0 root         (0) root         (0)      493 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/location_taxonomy.py
+-rw-rw-r--   0 root         (0) root         (0)     1004 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/market_deployment.py
+-rw-rw-r--   0 root         (0) root         (0)     1292 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/operational_status.py
+-rw-rw-r--   0 root         (0) root         (0)      510 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/push_type.py
+-rw-rw-r--   0 root         (0) root         (0)      552 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/tonnage_list.py
+-rw-rw-r--   0 root         (0) root         (0)     5517 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/vessel.py
+-rw-rw-r--   0 root         (0) root         (0)     6831 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/vessel_filter.py
+-rw-rw-r--   0 root         (0) root         (0)      632 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/vessel_subclass.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.872928 signal-ocean-7.1.1/signal_ocean/market_rates/
+-rw-rw-r--   0 root         (0) root         (0)      536 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/market_rates/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1909 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/market_rates/_market_rates_json.py
+-rw-rw-r--   0 root         (0) root         (0)      178 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/market_rates/enums.py
+-rw-rw-r--   0 root         (0) root         (0)     4006 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/market_rates/market_rates_api.py
+-rw-rw-r--   0 root         (0) root         (0)     2548 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/market_rates/models.py
+-rw-rw-r--   0 root         (0) root         (0)      773 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/market_rates/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     2029 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/market_rates/vessel_classes.py
+-rw-rw-r--   0 root         (0) root         (0)     2299 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/plots.py
+-rw-rw-r--   0 root         (0) root         (0)      578 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port.py
+-rw-rw-r--   0 root         (0) root         (0)     1489 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.876927 signal-ocean-7.1.1/signal_ocean/port_congestion/
+-rw-rw-r--   0 root         (0) root         (0)      347 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_congestion/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4274 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_congestion/models.py
+-rw-rw-r--   0 root         (0) root         (0)    19251 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_congestion/port_congestion.py
+-rw-rw-r--   0 root         (0) root         (0)     4670 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_congestion/port_congestion_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.876927 signal-ocean-7.1.1/signal_ocean/port_expenses/
+-rw-rw-r--   0 root         (0) root         (0)     1026 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_expenses/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1433 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_expenses/_port_expenses_json.py
+-rw-rw-r--   0 root         (0) root         (0)      823 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_expenses/enums.py
+-rw-rw-r--   0 root         (0) root         (0)     1867 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_expenses/models.py
+-rw-rw-r--   0 root         (0) root         (0)     8527 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_expenses/port_expenses_api.py
+-rw-rw-r--   0 root         (0) root         (0)      779 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_expenses/port_filter.py
+-rw-rw-r--   0 root         (0) root         (0)     1147 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/port_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.876927 signal-ocean-7.1.1/signal_ocean/scraped_cargoes/
+-rw-rw-r--   0 root         (0) root         (0)      277 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_cargoes/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    26586 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_cargoes/models.py
+-rw-rw-r--   0 root         (0) root         (0)     5363 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_cargoes/scraped_cargoes_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.876927 signal-ocean-7.1.1/signal_ocean/scraped_data/
+-rw-rw-r--   0 root         (0) root         (0)       41 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_data/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4560 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_data/scraped_data_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.876927 signal-ocean-7.1.1/signal_ocean/scraped_fixtures/
+-rw-rw-r--   0 root         (0) root         (0)      291 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_fixtures/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    32666 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_fixtures/models.py
+-rw-rw-r--   0 root         (0) root         (0)     6009 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_fixtures/scraped_fixtures_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.876927 signal-ocean-7.1.1/signal_ocean/scraped_lineups/
+-rw-rw-r--   0 root         (0) root         (0)      281 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_lineups/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    21114 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_lineups/models.py
+-rw-rw-r--   0 root         (0) root         (0)     5968 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_lineups/scraped_lineups_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.876927 signal-ocean-7.1.1/signal_ocean/scraped_positions/
+-rw-rw-r--   0 root         (0) root         (0)      301 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_positions/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    16973 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_positions/models.py
+-rw-rw-r--   0 root         (0) root         (0)     6044 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/scraped_positions/scraped_positions_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.876927 signal-ocean-7.1.1/signal_ocean/tonnage_list/
+-rw-rw-r--   0 root         (0) root         (0)      879 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/tonnage_list/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3345 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/tonnage_list/_json.py
+-rw-rw-r--   0 root         (0) root         (0)     6084 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/tonnage_list/api.py
+-rw-rw-r--   0 root         (0) root         (0)     7229 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/tonnage_list/data_frame.py
+-rw-rw-r--   0 root         (0) root         (0)    26447 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/tonnage_list/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.876927 signal-ocean-7.1.1/signal_ocean/util/
+-rw-rw-r--   0 root         (0) root         (0)       56 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/util/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6505 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/util/parsing_helpers.py
+-rw-rw-r--   0 root         (0) root         (0)     6529 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/util/request_helpers.py
+-rw-rw-r--   0 root         (0) root         (0)      647 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessel_class.py
+-rw-rw-r--   0 root         (0) root         (0)     1653 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessel_class_api.py
+-rw-rw-r--   0 root         (0) root         (0)     1296 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessel_class_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.876927 signal-ocean-7.1.1/signal_ocean/vessel_emissions/
+-rw-rw-r--   0 root         (0) root         (0)      761 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessel_emissions/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    15668 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessel_emissions/models.py
+-rw-rw-r--   0 root         (0) root         (0)    14610 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessel_emissions/vessel_emissions_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.880928 signal-ocean-7.1.1/signal_ocean/vessel_valuations/
+-rw-rw-r--   0 root         (0) root         (0)      298 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessel_valuations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      595 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessel_valuations/_valuation_json.py
+-rw-rw-r--   0 root         (0) root         (0)      608 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessel_valuations/models.py
+-rw-rw-r--   0 root         (0) root         (0)     2679 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessel_valuations/vessel_valuations_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.880928 signal-ocean-7.1.1/signal_ocean/vessels/
+-rw-rw-r--   0 root         (0) root         (0)      378 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessels/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    17416 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessels/models.py
+-rw-rw-r--   0 root         (0) root         (0)     3539 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/vessels/vessels_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.880928 signal-ocean-7.1.1/signal_ocean/voyages/
+-rw-rw-r--   0 root         (0) root         (0)     1298 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/voyages/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    46003 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/voyages/models.py
+-rw-rw-r--   0 root         (0) root         (0)    44702 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/voyages/voyages_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.880928 signal-ocean-7.1.1/signal_ocean/voyages_market_data/
+-rw-rw-r--   0 root         (0) root         (0)      539 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/voyages_market_data/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    15350 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/voyages_market_data/models.py
+-rw-rw-r--   0 root         (0) root         (0)    15865 2023-07-14 10:43:18.000000 signal-ocean-7.1.1/signal_ocean/voyages_market_data/voyages_market_data_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:44:17.868927 signal-ocean-7.1.1/signal_ocean.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2175 2023-07-14 10:44:17.000000 signal-ocean-7.1.1/signal_ocean.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5081 2023-07-14 10:44:17.000000 signal-ocean-7.1.1/signal_ocean.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 10:44:17.000000 signal-ocean-7.1.1/signal_ocean.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2023-07-14 10:44:17.000000 signal-ocean-7.1.1/signal_ocean.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-14 10:44:17.000000 signal-ocean-7.1.1/signal_ocean.egg-info/top_level.txt
```

### Comparing `signal-ocean-7.1.0/LICENSE` & `signal-ocean-7.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/PKG-INFO` & `signal-ocean-7.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal-ocean
-Version: 7.1.0
+Version: 7.1.1
 Summary: Access Signal Ocean Platform data using Python.
 Home-page: https://apis.signalocean.com/
 Author: Signal Ocean Developers
 Author-email: signaloceandevelopers@thesignalgroup.com
 License: Apache 2.0
 Project-URL: The Signal Group, https://www.thesignalgroup.com/
 Project-URL: Signal Ocean, https://www.signalocean.com/
```

### Comparing `signal-ocean-7.1.0/README.md` & `signal-ocean-7.1.1/README.md`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/setup.py` & `signal-ocean-7.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/__init__.py` & `signal-ocean-7.1.1/signal_ocean/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/_internals.py` & `signal-ocean-7.1.1/signal_ocean/_internals.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/companies/companies_api.py` & `signal-ocean-7.1.1/signal_ocean/companies/companies_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/companies/models.py` & `signal-ocean-7.1.1/signal_ocean/companies/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/connection.py` & `signal-ocean-7.1.1/signal_ocean/connection.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/distances/__init__.py` & `signal-ocean-7.1.1/signal_ocean/distances/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/distances/_distances_json.py` & `signal-ocean-7.1.1/signal_ocean/distances/_distances_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/distances/distances_api.py` & `signal-ocean-7.1.1/signal_ocean/distances/distances_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/distances/models.py` & `signal-ocean-7.1.1/signal_ocean/distances/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/distances/port_filter.py` & `signal-ocean-7.1.1/signal_ocean/distances/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/distances/vessel_class_filter.py` & `signal-ocean-7.1.1/signal_ocean/distances/vessel_class_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/freight_pricing/__init__.py` & `signal-ocean-7.1.1/signal_ocean/freight_pricing/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/freight_pricing/_freight_pricing_json.py` & `signal-ocean-7.1.1/signal_ocean/freight_pricing/_freight_pricing_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/freight_pricing/freight_pricing_api.py` & `signal-ocean-7.1.1/signal_ocean/freight_pricing/freight_pricing_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/freight_pricing/models.py` & `signal-ocean-7.1.1/signal_ocean/freight_pricing/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/freight_pricing/port_filter.py` & `signal-ocean-7.1.1/signal_ocean/freight_pricing/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/freight_pricing/vessel_class_filter.py` & `signal-ocean-7.1.1/signal_ocean/freight_pricing/vessel_class_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/freight_pricing/vessel_type_filter.py` & `signal-ocean-7.1.1/signal_ocean/freight_pricing/vessel_type_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/freight_rates/__init__.py` & `signal-ocean-7.1.1/signal_ocean/freight_rates/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/freight_rates/_freight_rates_json.py` & `signal-ocean-7.1.1/signal_ocean/freight_rates/_freight_rates_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/freight_rates/enums.py` & `signal-ocean-7.1.1/signal_ocean/freight_rates/enums.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/freight_rates/freight_rates_api.py` & `signal-ocean-7.1.1/signal_ocean/freight_rates/freight_rates_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/freight_rates/models.py` & `signal-ocean-7.1.1/signal_ocean/freight_rates/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/freight_rates/port_filter.py` & `signal-ocean-7.1.1/signal_ocean/freight_rates/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/freight_rates/utils.py` & `signal-ocean-7.1.1/signal_ocean/freight_rates/utils.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/geos/geos_api.py` & `signal-ocean-7.1.1/signal_ocean/geos/geos_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/geos/models.py` & `signal-ocean-7.1.1/signal_ocean/geos/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/__init__.py` & `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/_historical_tonnage_list_json.py` & `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/_historical_tonnage_list_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/column.py` & `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/column.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/commercial_status.py` & `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/commercial_status.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/historical_tonnage_list.py` & `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/historical_tonnage_list.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/historical_tonnage_list_api.py` & `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/historical_tonnage_list_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/market_deployment.py` & `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/market_deployment.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/operational_status.py` & `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/operational_status.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/tonnage_list.py` & `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/tonnage_list.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/vessel.py` & `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/vessel.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/vessel_filter.py` & `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/vessel_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/historical_tonnage_list/vessel_subclass.py` & `signal-ocean-7.1.1/signal_ocean/historical_tonnage_list/vessel_subclass.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/market_rates/__init__.py` & `signal-ocean-7.1.1/signal_ocean/market_rates/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/market_rates/_market_rates_json.py` & `signal-ocean-7.1.1/signal_ocean/market_rates/_market_rates_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/market_rates/market_rates_api.py` & `signal-ocean-7.1.1/signal_ocean/market_rates/market_rates_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/market_rates/models.py` & `signal-ocean-7.1.1/signal_ocean/market_rates/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/market_rates/utils.py` & `signal-ocean-7.1.1/signal_ocean/market_rates/utils.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/market_rates/vessel_classes.py` & `signal-ocean-7.1.1/signal_ocean/market_rates/vessel_classes.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/plots.py` & `signal-ocean-7.1.1/signal_ocean/plots.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/port.py` & `signal-ocean-7.1.1/signal_ocean/port.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/port_api.py` & `signal-ocean-7.1.1/signal_ocean/port_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/port_congestion/models.py` & `signal-ocean-7.1.1/signal_ocean/port_congestion/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/port_congestion/port_congestion.py` & `signal-ocean-7.1.1/signal_ocean/port_congestion/port_congestion.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/port_congestion/port_congestion_api.py` & `signal-ocean-7.1.1/signal_ocean/port_congestion/port_congestion_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/port_expenses/__init__.py` & `signal-ocean-7.1.1/signal_ocean/port_expenses/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/port_expenses/_port_expenses_json.py` & `signal-ocean-7.1.1/signal_ocean/port_expenses/_port_expenses_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/port_expenses/enums.py` & `signal-ocean-7.1.1/signal_ocean/port_expenses/enums.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/port_expenses/models.py` & `signal-ocean-7.1.1/signal_ocean/port_expenses/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/port_expenses/port_expenses_api.py` & `signal-ocean-7.1.1/signal_ocean/port_expenses/port_expenses_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/port_expenses/port_filter.py` & `signal-ocean-7.1.1/signal_ocean/port_expenses/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/port_filter.py` & `signal-ocean-7.1.1/signal_ocean/port_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/scraped_cargoes/models.py` & `signal-ocean-7.1.1/signal_ocean/scraped_cargoes/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/scraped_cargoes/scraped_cargoes_api.py` & `signal-ocean-7.1.1/signal_ocean/scraped_cargoes/scraped_cargoes_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/scraped_data/scraped_data_api.py` & `signal-ocean-7.1.1/signal_ocean/scraped_data/scraped_data_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/scraped_fixtures/models.py` & `signal-ocean-7.1.1/signal_ocean/scraped_fixtures/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/scraped_fixtures/scraped_fixtures_api.py` & `signal-ocean-7.1.1/signal_ocean/scraped_fixtures/scraped_fixtures_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/scraped_lineups/models.py` & `signal-ocean-7.1.1/signal_ocean/scraped_lineups/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/scraped_lineups/scraped_lineups_api.py` & `signal-ocean-7.1.1/signal_ocean/scraped_lineups/scraped_lineups_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/scraped_positions/models.py` & `signal-ocean-7.1.1/signal_ocean/scraped_positions/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/scraped_positions/scraped_positions_api.py` & `signal-ocean-7.1.1/signal_ocean/scraped_positions/scraped_positions_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/tonnage_list/__init__.py` & `signal-ocean-7.1.1/signal_ocean/tonnage_list/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/tonnage_list/_json.py` & `signal-ocean-7.1.1/signal_ocean/tonnage_list/_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/tonnage_list/api.py` & `signal-ocean-7.1.1/signal_ocean/tonnage_list/api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/tonnage_list/data_frame.py` & `signal-ocean-7.1.1/signal_ocean/tonnage_list/data_frame.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/tonnage_list/models.py` & `signal-ocean-7.1.1/signal_ocean/tonnage_list/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/util/parsing_helpers.py` & `signal-ocean-7.1.1/signal_ocean/util/parsing_helpers.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/util/request_helpers.py` & `signal-ocean-7.1.1/signal_ocean/util/request_helpers.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/vessel_class.py` & `signal-ocean-7.1.1/signal_ocean/vessel_class.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/vessel_class_api.py` & `signal-ocean-7.1.1/signal_ocean/vessel_class_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/vessel_class_filter.py` & `signal-ocean-7.1.1/signal_ocean/vessel_class_filter.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/vessel_emissions/__init__.py` & `signal-ocean-7.1.1/signal_ocean/vessel_emissions/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/vessel_emissions/models.py` & `signal-ocean-7.1.1/signal_ocean/vessel_emissions/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """The models for vessel emissions api."""
+import dataclasses
 from dataclasses import dataclass
 from typing import Optional, List
+from operator import attrgetter
 
 
 @dataclass(frozen=True)
 class Emissions:
     """Contains the reported emissions per gas type.
 
     Attributes:
@@ -14,22 +16,22 @@
     n2_oin_tons: N20 emissions in tons
     nmvocin_tons: NMVOC emissions in tons
     nox_in_tons: NOX emissions in tons
     sox_in_tons: SOX emissions in tons
     pmin_tons: PM emissions in tons
 
     """
-    co2_in_tons: float
-    coin_tons: float
-    ch4_in_tons: float
-    n2_oin_tons: float
-    nmvocin_tons: float
-    nox_in_tons: float
-    sox_in_tons: float
-    pmin_tons: float
+    co2_in_tons: Optional[float] = None
+    coin_tons: Optional[float] = None
+    ch4_in_tons: Optional[float] = None
+    n2_oin_tons: Optional[float] = None
+    nmvocin_tons: Optional[float] = None
+    nox_in_tons: Optional[float] = None
+    sox_in_tons: Optional[float] = None
+    pmin_tons: Optional[float] = None
 
 
 @dataclass(frozen=True)
 class EmissionsBreakdown:
     """Contains emissions breakdown for different parts of the Voyage.
 
     Attributes:
@@ -56,21 +58,21 @@
     mgo_in_tons: MGO vessel consumption in tons
     lng_in_tons: LNG vessel consumption in tons
     lpg_propane_in_tons: LPG Propane vessel consumption in tons
     lpg_butane_in_tons: LPG Butane vessel consumption in tons
     total_in_tons: Total vessel consumption in tons
 
     """
+    total_in_tons: float
     hfoin_tons: Optional[float] = None
     lfoin_tons: Optional[float] = None
     mgoin_tons: Optional[float] = None
     lngin_tons: Optional[float] = None
     lpgpropane_in_tons: Optional[float] = None
     lpgbutane_in_tons: Optional[float] = None
-    total_in_tons: Optional[float] = None
 
 
 @dataclass(frozen=True)
 class ConsumptionsBreakdown:
     """Contains consumptions breakdown for different parts of the Voyage.
 
     Attributes:
@@ -190,63 +192,66 @@
         EOI and the given alignment target from Sea Cargo Charter.
         Negative is aligned, positive is misaligned.
         kg_co2_per_tonne_cargo: Kg of CO2 per tonne of cargo carried
         kg_co2_per_tonne_dwt: Kg of CO2 per tonne of the vessel's deadweight
 
 
     """
-    voyage_cii: float
-    voyage_cii_unit: str
-    voyage_cii_rating: str
-    voyage_cii_target: float
-    voyage_cii_target_year: int
-    capacity_eeoi: float
-    capacity_eeoi_unit: str
-    capacity_eeoi_sea_cargo_charter_year_target: float
-    capacity_eeoi_sea_cargo_charter_class: str
-    capacity_eeoi_sea_cargo_charter_alignment_in_percentage: float
-    eeoi: Optional[float]
-    eeoi_unit: Optional[str]
-    eeoi_sea_cargo_charter_year_target: Optional[float]
-    eeoi_sea_cargo_charter_class: Optional[str]
-    eeoi_sea_cargo_charter_alignment_in_percentage: Optional[float]
-    kg_co2_per_tonne_cargo: Optional[float]
-    kg_co2_per_tonne_dwt: Optional[float]
+    voyage_cii: Optional[float] = None
+    voyage_cii_unit: Optional[str] = None
+    voyage_cii_rating: Optional[str] = None
+    voyage_cii_target: Optional[float] = None
+    voyage_cii_target_year: Optional[int] = None
+    capacity_eeoi: Optional[float] = None
+    capacity_eeoi_unit: Optional[str] = None
+    capacity_eeoi_sea_cargo_charter_year_target: \
+        Optional[float] = None
+    capacity_eeoi_sea_cargo_charter_class: Optional[str] = None
+    capacity_eeoi_sea_cargo_charter_alignment_in_percentage: \
+        Optional[float] = None
+    eeoi: Optional[float] = None
+    eeoi_unit: Optional[str] = None
+    eeoi_sea_cargo_charter_year_target: Optional[float] = None
+    eeoi_sea_cargo_charter_class: Optional[str] = None
+    eeoi_sea_cargo_charter_alignment_in_percentage: \
+        Optional[float] = None
+    kg_co2_per_tonne_cargo: Optional[float] = None
+    kg_co2_per_tonne_dwt: Optional[float] = None
 
 
 @dataclass(frozen=True)
 class SeagoingSpeedStatistics:
     """Contains speed statistics.
 
     Attributes:
         average_speed_in_knots: Average seagoing speed in knots
         std_speed_in_knots: Standard deviation speed in knots
         min_speed_in_knots: Minimum seagoing speed in knots
         max_speed_in_knots: Maximum seagoing speed in knots
 
     """
-    average_speed_in_knots: Optional[float]
-    std_speed_in_knots: Optional[float]
-    min_speed_in_knots: Optional[float]
-    max_speed_in_knots: Optional[float]
+    average_speed_in_knots: Optional[float] = None
+    std_speed_in_knots: Optional[float] = None
+    min_speed_in_knots: Optional[float] = None
+    max_speed_in_knots: Optional[float] = None
 
 
 @dataclass(frozen=True)
 class SeagoingSpeedStatisticsBreakdown:
     """Contains speed statistics for different parts of the Voyage.
 
     Attributes:
         voyage: Speed statistics for the voyage"
         laden: Speed statistics for the ballast part of the voyage
         ballast: Speed statistics for the laden part of the voyage
 
     """
-    voyage: SeagoingSpeedStatistics
-    laden: SeagoingSpeedStatistics
-    ballast: SeagoingSpeedStatistics
+    voyage: Optional[SeagoingSpeedStatistics] = None
+    laden: Optional[SeagoingSpeedStatistics] = None
+    ballast: Optional[SeagoingSpeedStatistics] = None
 
 
 @dataclass(frozen=True)
 class EmissionsEssentialStatistics:
     """Contains Emissions essential statistics.
 
     Attributes:
@@ -294,38 +299,56 @@
         Speed Statistics breakdown for the voyage
         duration: Duration breakdown for the voyage
         distances: Distance travelled breakdown for the voyage
         efficiency_metrics: Emissions Efficiency metrics for the voyage
         european_union_regulated: European Union Related Emissions
 
     """
-    id: Optional[str] = None
-    imo: Optional[int] = None
-    vessel_name: Optional[str] = None
-    voyage_number: Optional[int] = None
-    vessel_type_id: Optional[int] = None
+    id: str
+    imo: int
+    vessel_name: str
+    voyage_number: int
+    vessel_type_id: int
+    vessel_class_id: int
+    start_date: str
+    end_date: str
+    deadweight: int
+    emissions: EmissionsBreakdown
     vessel_type: Optional[str] = None
-    vessel_class_id: Optional[int] = None
     vessel_class: Optional[str] = None
-    start_date: Optional[str] = None
-    end_date: Optional[str] = None
     quantity: Optional[float] = None
-    deadweight: Optional[int] = None
     transport_work_in_million_tonne_miles: Optional[float] = None
     transport_work_in_million_dwt_miles: Optional[float] = None
     contains_eu_emissions: Optional[bool] = None
-    emissions: Optional[EmissionsBreakdown] = None
     consumptions: Optional[ConsumptionsBreakdown] = None
     seagoing_speed_statistics: \
         Optional[SeagoingSpeedStatisticsBreakdown] = None
     duration: Optional[DurationBreakdown] = None
     distances: Optional[DistancesBreakdown] = None
     efficiency_metrics: Optional[Metrics] = None
     european_union_regulated: Optional[EmissionsEssentialStatistics] = None
 
+    def __repr__(self) -> str:
+        """Override of the default __repr__ function.
+
+        Returns:
+            Object string representation omitting None attributes
+
+        """
+        nodef_f_vals = (
+            (f.name, attrgetter(f.name)(self))
+            for f in dataclasses.fields(self)
+            if attrgetter(f.name)(self) != f.default
+        )
+
+        nodef_f_repr = ", ".join(f"{name}={value}"
+                                 for name, value
+                                 in nodef_f_vals)
+        return f"{self.__class__.__name__}({nodef_f_repr})"
+
 
 @dataclass(frozen=True)
 class Eexi:
     """Contains EEXI info.
 
     Attributes:
         value: Acquired EEXI value
```

### Comparing `signal-ocean-7.1.0/signal_ocean/vessel_emissions/vessel_emissions_api.py` & `signal-ocean-7.1.1/signal_ocean/vessel_emissions/vessel_emissions_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,102 @@
 """The vessel emissions api."""
-from typing import Optional, List, Union
-from urllib.parse import urljoin
+from typing import Optional, List, Union, Dict, Any
+from urllib.parse import urljoin, urlencode
 from datetime import date
 from signal_ocean import Connection
 from signal_ocean.util.request_helpers import get_multiple, get_single
 from signal_ocean.vessel_emissions.models import EmissionsEstimation, \
     VesselMetrics, VesselClassEmissions, VesselClassMetrics
 
 
+def make_url(
+        base_url: str,
+        *res: Union[str, int],
+        **params: str
+) -> str:
+    """Constructs url for the request.
+
+    Args:
+        base_url: the base to build the url.
+        Can be either emissions or emissions/metrics
+
+    """
+    url = base_url
+    for r in res:
+        url = '{}/{}'.format(url, r)
+    if params:
+        url = '{}?{}'.format(url, urlencode(params))
+    return url
+
+
+def custom_headers(connection: Connection) -> Dict[str, Optional[str]]:
+    """Custom function to change the request header.
+
+    Args:
+        connection: Connection object
+
+    Returns:
+        headers dict
+
+    """
+    return {
+        "Ocp-Apim-Subscription-Key":
+            connection._Connection__api_key,  # type: ignore
+        "Content-Type": "application/json",
+        "Source": "SignalSDK",
+    }
+
+
 class VesselEmissionsAPI:
     """Represents Signal's Vessel Emissions API."""
 
     relative_url = "vessel-emissions-api/public/v2/"
     default_pit = str(date.today())
 
     def __init__(self, connection: Optional[Connection] = None):
-        """Initializes VesselsAPI.
+        """Initializes VesselEmissionsAPI.
 
         Args:
             connection: API connection configuration. If not provided, the
                 default connection method is used.
         """
-        self.__connection = connection or Connection()
+        if connection is not None:
+            func_type = type(
+                connection._Connection__get_headers  # type: ignore
+            )
+            connection._Connection__get_headers = func_type(  # type: ignore
+                custom_headers, connection
+            )
+            self.__connection = connection
+        else:
+            connection = Connection()
+            func_type = type(
+                connection._Connection__get_headers  # type: ignore
+            )
+            connection._Connection__get_headers = func_type(  # type: ignore
+                custom_headers, connection
+            )
+            self.__connection = connection
 
-    def construct_emissions_url_parameters(
+    def construct_url_parameters(
             self,
             quantity: Union[int, None] = None,
-            token: Union[str, None] = None,
+            token: Optional[str] = None,
             include_consumptions: bool = False,
             include_efficiency_metrics: bool = False,
             include_distances: bool = False,
             include_durations: bool = False,
             include_speed_statistics: bool = False,
             include_eu_emissions: bool = False,
-            sulphur_content_hfo: Union[float, None] = 0.025,
-            sulphur_content_lfo: Union[float, None] = 0.001,
-            sulphur_content_mgo: Union[float, None] = 0.001,
-            sulphur_content_lng: Union[float, None] = 0.00004
-           ) -> str:
-        """Construct the request URL based on the input parameters.
+            sulphur_content_hfo: Optional[Union[float, None]] = None,
+            sulphur_content_lfo: Optional[Union[float, None]] = None,
+            sulphur_content_mgo: Optional[Union[float, None]] = None,
+            sulphur_content_lng: Optional[Union[float, None]] = None
+    ) -> Dict[Any, str]:
+        """Construct the request parameters based on the user's input.
 
         Args:
         quantity: Cargo quantity of the voyage
         token: Next page token
         include_consumptions: Include consumption data in response
         include_efficiency_metrics: Include efficiency metrics in response
         include_distances: Include distances data in the response
@@ -52,56 +106,53 @@
         emissions in response
         sulphur_content_hfo: Sulphur Content of HFO fuel type
         sulphur_content_lfo: Sulphur Content of LFO fuel type
         sulphur_content_mgo: Sulphur Content of MGO fuel type
         sulphur_content_lng: Sulphur Content of LNG fuel type
 
         Returns:
-            The last part of Request URL
+            The parameters dictionary of Request URL
         """
-        url = "?"
-        if quantity:
-            url = urljoin(url, f"quality={quantity}")
-        if token:
-            url = urljoin(url, f"token={token}")
-        query_url = (
-            f"include_consumptions={include_consumptions}"
-            f"&include_efficiency_metrics={include_efficiency_metrics}"
-            f"&include_distances={include_distances}"
-            f"&include_durations={include_durations}"
-            f"&include_speed_statistics={include_speed_statistics}"
-            f"&include_eu_emissions={include_eu_emissions}"
-        )
-        url = urljoin(url, query_url)
-        if sulphur_content_hfo:
-            url = urljoin(url, f"&sulphur_content_hfo={sulphur_content_hfo}")
-        if sulphur_content_lfo:
-            url = urljoin(url, f"&sulphur_content_lfo={sulphur_content_lfo}")
-        if sulphur_content_mgo:
-            url = urljoin(url, f"&sulphur_content_mgo={sulphur_content_mgo}")
-        if sulphur_content_lng:
-            url = urljoin(url, f"&sulphur_content_lng={sulphur_content_lng}")
-        return url
+        params = {}
+        if quantity is not None:
+            params['quantity'] = str(quantity)
+        if token is not None:
+            params['token'] = token
+        params['include_consumptions'] = str(include_consumptions)
+        params['include_efficiency_metrics'] = str(include_efficiency_metrics)
+        params['include_distances'] = str(include_distances)
+        params['include_durations'] = str(include_durations)
+        params['include_speed_statistics'] = str(include_speed_statistics)
+        params['include_eu_emissions'] = str(include_eu_emissions)
+        if sulphur_content_hfo is not None:
+            params['sulphur_content_hfo'] = str(sulphur_content_hfo)
+        if sulphur_content_lfo is not None:
+            params['sulphur_content_lfo'] = str(sulphur_content_lfo)
+        if sulphur_content_mgo is not None:
+            params['sulphur_content_mgo'] = str(sulphur_content_mgo)
+        if sulphur_content_lng is not None:
+            params['sulphur_content_lng'] = str(sulphur_content_lng)
+        return params
 
     def get_emissions_by_imo_and_voyage_number(
             self,
             imo: int,
             voyage_number: int,
             quantity: Union[int, None] = None,
             include_consumptions: bool = False,
             include_efficiency_metrics: bool = False,
             include_distances: bool = False,
             include_durations: bool = False,
             include_speed_statistics: bool = False,
             include_eu_emissions: bool = False,
-            sulphur_content_hfo: Union[float, None] = 0.025,
-            sulphur_content_lfo: Union[float, None] = 0.001,
-            sulphur_content_mgo: Union[float, None] = 0.001,
-            sulphur_content_lng: Union[float, None] = 0.00004
-            ) -> Optional[EmissionsEstimation]:
+            sulphur_content_hfo: Union[float, None] = None,
+            sulphur_content_lfo: Union[float, None] = None,
+            sulphur_content_mgo: Union[float, None] = None,
+            sulphur_content_lng: Union[float, None] = None
+    ) -> Optional[EmissionsEstimation]:
         """Retrieves voyage emissions for a vessel by its IMO and Voyage Number.
 
         Args:
             imo: Vessel IMO to retrieve.
             voyage_number: Voyage Number to retrieve.
             quantity: User defined transported quantity for voyage.
             include_consumptions: Include consumption data in the response.
@@ -116,46 +167,47 @@
             sulphur_content_mgo: Sulphur Content of MGO fuel type.
             sulphur_content_lng: Sulphur Content of LNG fuel type.
 
         Returns:
             EmissionsEstimation if no vessel with
             the specified IMO or Voyage Number has been found.
         """
-        query_url = self.construct_emissions_url_parameters(
+        params_dict = self.construct_url_parameters(
             quantity=quantity,
             include_consumptions=include_consumptions,
             include_efficiency_metrics=include_efficiency_metrics,
             include_distances=include_distances,
             include_durations=include_durations,
             include_speed_statistics=include_speed_statistics,
             include_eu_emissions=include_eu_emissions,
             sulphur_content_hfo=sulphur_content_hfo,
             sulphur_content_lfo=sulphur_content_lfo,
             sulphur_content_mgo=sulphur_content_mgo,
             sulphur_content_lng=sulphur_content_lng)
-        query_url = urljoin(f"emissions/imo/{imo}"
-                            f"/voyage_number/{voyage_number}",
-                            query_url)
+        query_url = make_url('emissions',
+                             'imo', imo,
+                             'voyage_number', voyage_number,
+                             **params_dict)
         url = urljoin(VesselEmissionsAPI.relative_url, query_url)
         return get_single(self.__connection, url, EmissionsEstimation)
 
     def get_emissions_by_imo(
             self,
             imo: int,
             include_consumptions: bool = False,
             include_efficiency_metrics: bool = False,
             include_distances: bool = False,
             include_durations: bool = False,
             include_speed_statistics: bool = False,
             include_eu_emissions: bool = False,
-            sulphur_content_hfo: Union[float, None] = 0.025,
-            sulphur_content_lfo: Union[float, None] = 0.001,
-            sulphur_content_mgo: Union[float, None] = 0.001,
-            sulphur_content_lng: Union[float, None] = 0.00004
-            ) -> List[EmissionsEstimation]:
+            sulphur_content_hfo: Union[float, None] = None,
+            sulphur_content_lfo: Union[float, None] = None,
+            sulphur_content_mgo: Union[float, None] = None,
+            sulphur_content_lng: Union[float, None] = None
+    ) -> List[EmissionsEstimation]:
         """Retrieves a list of vessel emissions by its IMO.
 
         Args:
             imo: IMO of the vessel to retrieve emissions.
             include_consumptions: Include consumption data in the response.
             include_efficiency_metrics: Include efficiency metrics
              data in the response.
@@ -170,26 +222,29 @@
             sulphur_content_mgo: Sulphur Content of MGO fuel type.
             sulphur_content_lng: Sulphur Content of LNG fuel type.
 
         Returns:
             A list of vessel emissions or None if no vessel
              with the specified IMO has been found.
         """
-        query_url = self.construct_emissions_url_parameters(
+        params_dict = self.construct_url_parameters(
             include_consumptions=include_consumptions,
             include_efficiency_metrics=include_efficiency_metrics,
             include_distances=include_distances,
             include_durations=include_durations,
             include_speed_statistics=include_speed_statistics,
             include_eu_emissions=include_eu_emissions,
             sulphur_content_hfo=sulphur_content_hfo,
             sulphur_content_lfo=sulphur_content_lfo,
             sulphur_content_mgo=sulphur_content_mgo,
-            sulphur_content_lng=sulphur_content_lng)
-        query_url = urljoin(f"emissions/imo/{imo}", query_url)
+            sulphur_content_lng=sulphur_content_lng
+        )
+        query_url = make_url('emissions',
+                             'imo', imo,
+                             **params_dict)
         url = urljoin(VesselEmissionsAPI.relative_url, query_url)
         return [i for i in get_multiple(self.__connection,
                                         url,
                                         EmissionsEstimation)]
 
     def get_metrics_by_imo(
             self,
@@ -241,26 +296,27 @@
              data in the response.
 
         Returns:
             List of emissions estimation for all
              available voyages of a vessel class.
 
         """
-        query_url = self.construct_emissions_url_parameters(
+        params_dict = self.construct_url_parameters(
             token=token,
             include_consumptions=include_consumptions,
             include_efficiency_metrics=include_efficiency_metrics,
             include_distances=include_distances,
             include_durations=include_durations,
             include_speed_statistics=include_speed_statistics,
             include_eu_emissions=include_eu_emissions
         )
-        query_url = urljoin(f"emissions/class/"
-                            f"{vessel_class_id}",
-                            query_url)
+        query_url = make_url('emissions',
+                             'class', vessel_class_id,
+                             **params_dict)
+
         url = urljoin(VesselEmissionsAPI.relative_url, query_url)
         return get_single(self.__connection,
                           url,
                           VesselClassEmissions)
 
     def get_metrics_by_vessel_class_id(self,
                                        vessel_class_id: int,
```

### Comparing `signal-ocean-7.1.0/signal_ocean/vessel_valuations/_valuation_json.py` & `signal-ocean-7.1.1/signal_ocean/vessel_valuations/_valuation_json.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/vessel_valuations/models.py` & `signal-ocean-7.1.1/signal_ocean/vessel_valuations/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/vessel_valuations/vessel_valuations_api.py` & `signal-ocean-7.1.1/signal_ocean/vessel_valuations/vessel_valuations_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/vessels/models.py` & `signal-ocean-7.1.1/signal_ocean/vessels/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/vessels/vessels_api.py` & `signal-ocean-7.1.1/signal_ocean/vessels/vessels_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/voyages/__init__.py` & `signal-ocean-7.1.1/signal_ocean/voyages/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/voyages/models.py` & `signal-ocean-7.1.1/signal_ocean/voyages/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/voyages/voyages_api.py` & `signal-ocean-7.1.1/signal_ocean/voyages/voyages_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/voyages_market_data/__init__.py` & `signal-ocean-7.1.1/signal_ocean/voyages_market_data/__init__.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/voyages_market_data/models.py` & `signal-ocean-7.1.1/signal_ocean/voyages_market_data/models.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean/voyages_market_data/voyages_market_data_api.py` & `signal-ocean-7.1.1/signal_ocean/voyages_market_data/voyages_market_data_api.py`

 * *Files identical despite different names*

### Comparing `signal-ocean-7.1.0/signal_ocean.egg-info/PKG-INFO` & `signal-ocean-7.1.1/signal_ocean.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal-ocean
-Version: 7.1.0
+Version: 7.1.1
 Summary: Access Signal Ocean Platform data using Python.
 Home-page: https://apis.signalocean.com/
 Author: Signal Ocean Developers
 Author-email: signaloceandevelopers@thesignalgroup.com
 License: Apache 2.0
 Project-URL: The Signal Group, https://www.thesignalgroup.com/
 Project-URL: Signal Ocean, https://www.signalocean.com/
```

### Comparing `signal-ocean-7.1.0/signal_ocean.egg-info/SOURCES.txt` & `signal-ocean-7.1.1/signal_ocean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

