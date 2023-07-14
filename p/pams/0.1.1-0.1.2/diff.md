# Comparing `tmp/pams-0.1.1.tar.gz` & `tmp/pams-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pams-0.1.1.tar", max compression
+gzip compressed data, was "pams-0.1.2.tar", max compression
```

## Comparing `pams-0.1.1.tar` & `pams-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1072 2023-06-30 18:54:16.371418 pams-0.1.1/LICENSE
--rw-r--r--   0        0        0     1903 2023-06-30 18:54:16.371418 pams-0.1.1/README.md
--rw-r--r--   0        0        0      594 2023-06-30 18:54:16.371418 pams-0.1.1/pams/__init__.py
--rw-r--r--   0        0        0      187 2023-06-30 18:54:16.371418 pams-0.1.1/pams/agents/__init__.py
--rw-r--r--   0        0        0     6689 2023-06-30 18:54:16.375418 pams-0.1.1/pams/agents/arbitrage_agent.py
--rw-r--r--   0        0        0     8620 2023-06-30 18:54:16.375418 pams-0.1.1/pams/agents/base.py
--rw-r--r--   0        0        0     9663 2023-06-30 18:54:16.375418 pams-0.1.1/pams/agents/fcn_agent.py
--rw-r--r--   0        0        0      363 2023-06-30 18:54:16.375418 pams-0.1.1/pams/agents/high_frequency_agent.py
--rw-r--r--   0        0        0     2323 2023-06-30 18:54:16.375418 pams-0.1.1/pams/agents/test_agent.py
--rw-r--r--   0        0        0      206 2023-06-30 18:54:16.375418 pams-0.1.1/pams/events/__init__.py
--rw-r--r--   0        0        0     9916 2023-06-30 18:54:16.375418 pams-0.1.1/pams/events/base.py
--rw-r--r--   0        0        0     3832 2023-06-30 18:54:16.375418 pams-0.1.1/pams/events/fundamental_price_shock.py
--rw-r--r--   0        0        0     4833 2023-06-30 18:54:16.375418 pams-0.1.1/pams/events/price_limit_rule.py
--rw-r--r--   0        0        0     6163 2023-06-30 18:54:16.375418 pams-0.1.1/pams/events/trading_halt_rule.py
--rw-r--r--   0        0        0    10298 2023-06-30 18:54:16.375418 pams-0.1.1/pams/fundamentals.py
--rw-r--r--   0        0        0     6379 2023-06-30 18:54:16.375418 pams-0.1.1/pams/index_market.py
--rw-r--r--   0        0        0      447 2023-06-30 18:54:16.375418 pams-0.1.1/pams/logs/__init__.py
--rw-r--r--   0        0        0    13673 2023-06-30 18:54:16.375418 pams-0.1.1/pams/logs/base.py
--rw-r--r--   0        0        0     1465 2023-06-30 18:54:16.375418 pams-0.1.1/pams/logs/market_step_loggers.py
--rw-r--r--   0        0        0    33146 2023-06-30 18:54:16.375418 pams-0.1.1/pams/market.py
--rw-r--r--   0        0        0    10140 2023-06-30 18:54:16.375418 pams-0.1.1/pams/order.py
--rw-r--r--   0        0        0     6151 2023-06-30 18:54:16.375418 pams-0.1.1/pams/order_book.py
--rw-r--r--   0        0        0       66 2023-06-30 18:54:16.375418 pams-0.1.1/pams/runners/__init__.py
--rw-r--r--   0        0        0     3848 2023-06-30 18:54:16.375418 pams-0.1.1/pams/runners/base.py
--rw-r--r--   0        0        0    27383 2023-06-30 18:54:16.375418 pams-0.1.1/pams/runners/sequential.py
--rw-r--r--   0        0        0     6187 2023-06-30 18:54:16.375418 pams-0.1.1/pams/session.py
--rw-r--r--   0        0        0    18332 2023-06-30 18:54:16.375418 pams-0.1.1/pams/simulator.py
--rw-r--r--   0        0        0      147 2023-06-30 18:54:16.375418 pams-0.1.1/pams/utils/__init__.py
--rw-r--r--   0        0        0     1353 2023-06-30 18:54:16.375418 pams-0.1.1/pams/utils/class_finder.py
--rw-r--r--   0        0        0     2312 2023-06-30 18:54:16.375418 pams-0.1.1/pams/utils/json_extends.py
--rw-r--r--   0        0        0     7435 2023-06-30 18:54:16.375418 pams-0.1.1/pams/utils/json_random.py
--rw-r--r--   0        0        0       22 2023-06-30 18:54:16.375418 pams-0.1.1/pams/version.py
--rw-r--r--   0        0        0     1271 2023-06-30 18:54:16.375418 pams-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2527 1970-01-01 00:00:00.000000 pams-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-14 15:21:55.444094 pams-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1903 2023-07-14 15:21:55.444094 pams-0.1.2/README.md
+-rw-r--r--   0        0        0      594 2023-07-14 15:21:55.444094 pams-0.1.2/pams/__init__.py
+-rw-r--r--   0        0        0      187 2023-07-14 15:21:55.444094 pams-0.1.2/pams/agents/__init__.py
+-rw-r--r--   0        0        0     6689 2023-07-14 15:21:55.444094 pams-0.1.2/pams/agents/arbitrage_agent.py
+-rw-r--r--   0        0        0     8620 2023-07-14 15:21:55.444094 pams-0.1.2/pams/agents/base.py
+-rw-r--r--   0        0        0     9663 2023-07-14 15:21:55.444094 pams-0.1.2/pams/agents/fcn_agent.py
+-rw-r--r--   0        0        0      363 2023-07-14 15:21:55.444094 pams-0.1.2/pams/agents/high_frequency_agent.py
+-rw-r--r--   0        0        0     2323 2023-07-14 15:21:55.444094 pams-0.1.2/pams/agents/test_agent.py
+-rw-r--r--   0        0        0      206 2023-07-14 15:21:55.444094 pams-0.1.2/pams/events/__init__.py
+-rw-r--r--   0        0        0     9916 2023-07-14 15:21:55.444094 pams-0.1.2/pams/events/base.py
+-rw-r--r--   0        0        0     3832 2023-07-14 15:21:55.444094 pams-0.1.2/pams/events/fundamental_price_shock.py
+-rw-r--r--   0        0        0     4833 2023-07-14 15:21:55.444094 pams-0.1.2/pams/events/price_limit_rule.py
+-rw-r--r--   0        0        0     6163 2023-07-14 15:21:55.444094 pams-0.1.2/pams/events/trading_halt_rule.py
+-rw-r--r--   0        0        0    10298 2023-07-14 15:21:55.444094 pams-0.1.2/pams/fundamentals.py
+-rw-r--r--   0        0        0     6379 2023-07-14 15:21:55.444094 pams-0.1.2/pams/index_market.py
+-rw-r--r--   0        0        0      447 2023-07-14 15:21:55.444094 pams-0.1.2/pams/logs/__init__.py
+-rw-r--r--   0        0        0    13673 2023-07-14 15:21:55.444094 pams-0.1.2/pams/logs/base.py
+-rw-r--r--   0        0        0     1465 2023-07-14 15:21:55.444094 pams-0.1.2/pams/logs/market_step_loggers.py
+-rw-r--r--   0        0        0    33146 2023-07-14 15:21:55.448094 pams-0.1.2/pams/market.py
+-rw-r--r--   0        0        0    10140 2023-07-14 15:21:55.448094 pams-0.1.2/pams/order.py
+-rw-r--r--   0        0        0     6151 2023-07-14 15:21:55.448094 pams-0.1.2/pams/order_book.py
+-rw-r--r--   0        0        0       66 2023-07-14 15:21:55.448094 pams-0.1.2/pams/runners/__init__.py
+-rw-r--r--   0        0        0     3848 2023-07-14 15:21:55.448094 pams-0.1.2/pams/runners/base.py
+-rw-r--r--   0        0        0    27935 2023-07-14 15:21:55.448094 pams-0.1.2/pams/runners/sequential.py
+-rw-r--r--   0        0        0     6187 2023-07-14 15:21:55.448094 pams-0.1.2/pams/session.py
+-rw-r--r--   0        0        0    18332 2023-07-14 15:21:55.448094 pams-0.1.2/pams/simulator.py
+-rw-r--r--   0        0        0      147 2023-07-14 15:21:55.448094 pams-0.1.2/pams/utils/__init__.py
+-rw-r--r--   0        0        0     1353 2023-07-14 15:21:55.448094 pams-0.1.2/pams/utils/class_finder.py
+-rw-r--r--   0        0        0     2312 2023-07-14 15:21:55.448094 pams-0.1.2/pams/utils/json_extends.py
+-rw-r--r--   0        0        0     7435 2023-07-14 15:21:55.448094 pams-0.1.2/pams/utils/json_random.py
+-rw-r--r--   0        0        0       22 2023-07-14 15:21:55.448094 pams-0.1.2/pams/version.py
+-rw-r--r--   0        0        0     1271 2023-07-14 15:21:55.448094 pams-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2527 1970-01-01 00:00:00.000000 pams-0.1.2/PKG-INFO
```

### Comparing `pams-0.1.1/LICENSE` & `pams-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/README.md` & `pams-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/__init__.py` & `pams-0.1.2/pams/__init__.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/agents/arbitrage_agent.py` & `pams-0.1.2/pams/agents/arbitrage_agent.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/agents/base.py` & `pams-0.1.2/pams/agents/base.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/agents/fcn_agent.py` & `pams-0.1.2/pams/agents/fcn_agent.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/agents/test_agent.py` & `pams-0.1.2/pams/agents/test_agent.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/events/base.py` & `pams-0.1.2/pams/events/base.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/events/fundamental_price_shock.py` & `pams-0.1.2/pams/events/fundamental_price_shock.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/events/price_limit_rule.py` & `pams-0.1.2/pams/events/price_limit_rule.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/events/trading_halt_rule.py` & `pams-0.1.2/pams/events/trading_halt_rule.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/fundamentals.py` & `pams-0.1.2/pams/fundamentals.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/index_market.py` & `pams-0.1.2/pams/index_market.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/logs/base.py` & `pams-0.1.2/pams/logs/base.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/logs/market_step_loggers.py` & `pams-0.1.2/pams/logs/market_step_loggers.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/market.py` & `pams-0.1.2/pams/market.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/order.py` & `pams-0.1.2/pams/order.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/order_book.py` & `pams-0.1.2/pams/order_book.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/runners/base.py` & `pams-0.1.2/pams/runners/base.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/runners/sequential.py` & `pams-0.1.2/pams/runners/sequential.py`

 * *Files 2% similar despite different names*

```diff
@@ -516,15 +516,25 @@
                             agent = self.simulator.id2agent[order.order.agent_id]
                             agent.canceled_order(log=log_)
                             self.simulator._trigger_event_after_cancel(cancel_log=log_)
                         else:
                             raise NotImplementedError
                         if session.with_order_execution:
                             logs = market._execution()
+                            self.simulator._update_agents_for_execution(
+                                execution_logs=logs
+                            )
                             for execution_log in logs:
+                                agent = self.simulator.id2agent[
+                                    execution_log.buy_agent_id
+                                ]
+                                agent.executed_order(log=execution_log)
+                                agent = self.simulator.id2agent[
+                                    execution_log.sell_agent_id
+                                ]
                                 agent.executed_order(log=execution_log)
                                 self.simulator._trigger_event_after_execution(
                                     execution_log=execution_log
                                 )
         return all_orders
 
     def _update_markets(self, session: Session) -> None:
```

### Comparing `pams-0.1.1/pams/session.py` & `pams-0.1.2/pams/session.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/simulator.py` & `pams-0.1.2/pams/simulator.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/utils/class_finder.py` & `pams-0.1.2/pams/utils/class_finder.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/utils/json_extends.py` & `pams-0.1.2/pams/utils/json_extends.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pams/utils/json_random.py` & `pams-0.1.2/pams/utils/json_random.py`

 * *Files identical despite different names*

### Comparing `pams-0.1.1/pyproject.toml` & `pams-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pams"
-version = "0.1.1"
+version = "0.1.2"
 description = "PAMS: Platform for Artificial Market Simulations"
 authors = ["Masanori HIRANO <masa.hirano.1996@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `pams-0.1.1/PKG-INFO` & `pams-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pams
-Version: 0.1.1
+Version: 0.1.2
 Summary: PAMS: Platform for Artificial Market Simulations
 License: MIT
 Author: Masanori HIRANO
 Author-email: masa.hirano.1996@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

