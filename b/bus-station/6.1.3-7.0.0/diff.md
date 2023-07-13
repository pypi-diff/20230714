# Comparing `tmp/bus_station-6.1.3.tar.gz` & `tmp/bus_station-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bus_station-6.1.3.tar", max compression
+gzip compressed data, was "bus_station-7.0.0.tar", max compression
```

## Comparing `bus_station-6.1.3.tar` & `bus_station-7.0.0.tar`

### file list

```diff
@@ -1,162 +1,150 @@
--rw-r--r--   0        0        0       48 2023-07-10 22:28:28.364446 bus_station-6.1.3/README.md
--rw-r--r--   0        0        0      985 2023-07-10 22:30:19.186889 bus_station-6.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/__init__.py
--rw-r--r--   0        0        0      143 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/bus_stop.py
--rw-r--r--   0        0        0      185 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/bus_stop_not_found.py
--rw-r--r--   0        0        0      690 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/environment.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/registration/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/registration/address/__init__.py
--rw-r--r--   0        0        0      199 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/registration/address/address_not_found_for_bus_stop.py
--rw-r--r--   0        0        0      407 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/registration/address/bus_stop_address_registry.py
--rw-r--r--   0        0        0      673 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/registration/address/redis_bus_stop_address_registry.py
--rw-r--r--   0        0        0     3774 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/registration/bus_stop_registry.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/registration/supervisor/__init__.py
--rw-r--r--   0        0        0     1180 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/registration/supervisor/bus_stop_address_registration_supervisor.py
--rw-r--r--   0        0        0      255 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/registration/supervisor/bus_stop_registration_supervisor.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/resolvers/__init__.py
--rw-r--r--   0        0        0      250 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/resolvers/bus_stop_resolver.py
--rw-r--r--   0        0        0      587 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/resolvers/in_memory_bus_stop_resolver.py
--rw-r--r--   0        0        0      772 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/resolvers/pypendency_bus_stop_resolver.py
--rw-r--r--   0        0        0     1107 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/resolvers/yandil_bus_stop_resolver.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/asynchronous/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/asynchronous/distributed/__init__.py
--rw-r--r--   0        0        0     1352 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/asynchronous/distributed/kombu_command_bus.py
--rw-r--r--   0        0        0      889 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/asynchronous/memory_queue_command_bus.py
--rw-r--r--   0        0        0     1237 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/asynchronous/threaded_command_bus.py
--rw-r--r--   0        0        0      258 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/command_bus.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/synchronous/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/synchronous/distributed/__init__.py
--rw-r--r--   0        0        0     2315 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/synchronous/distributed/json_rpc_command_bus.py
--rw-r--r--   0        0        0     2188 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/synchronous/distributed/rpyc_command_bus.py
--rw-r--r--   0        0        0     1128 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/synchronous/sync_command_bus.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus_engine/__init__.py
--rw-r--r--   0        0        0     1326 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus_engine/json_rpc_command_bus_engine.py
--rw-r--r--   0        0        0     2747 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus_engine/kombu_command_bus_engine.py
--rw-r--r--   0        0        0     1856 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus_engine/memory_queue_command_bus_engine.py
--rw-r--r--   0        0        0     1266 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus_engine/rpyc_command_bus_engine.py
--rw-r--r--   0        0        0      253 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/command.py
--rw-r--r--   0        0        0      292 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/command_execution_failed.py
--rw-r--r--   0        0        0      457 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/command_handler.py
--rw-r--r--   0        0        0      227 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/command_handler_not_found.py
--rw-r--r--   0        0        0     1795 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/command_handler_registry.py
--rw-r--r--   0        0        0      233 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/handler_not_found_for_command.py
--rw-r--r--   0        0        0      725 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/json_rpc_command_server.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/middleware/__init__.py
--rw-r--r--   0        0        0      607 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/middleware/command_middleware.py
--rw-r--r--   0        0        0     1078 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/middleware/command_middleware_receiver.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/middleware/implementations/__init__.py
--rw-r--r--   0        0        0     1070 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/middleware/implementations/logging_command_middleware.py
--rw-r--r--   0        0        0     1039 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/middleware/implementations/timing_command_middleware.py
--rw-r--r--   0        0        0      890 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/middleware/implementations/tracking_command_middleware.py
--rw-r--r--   0        0        0      712 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/rpyc_command_server.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus/asynchronous/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus/asynchronous/distributed/__init__.py
--rw-r--r--   0        0        0     1247 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus/asynchronous/distributed/kombu_event_bus.py
--rw-r--r--   0        0        0     1212 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus/asynchronous/memory_queue_event_bus.py
--rw-r--r--   0        0        0      984 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus/asynchronous/threaded_event_bus.py
--rw-r--r--   0        0        0      246 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus/event_bus.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus/synchronous/__init__.py
--rw-r--r--   0        0        0      872 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus/synchronous/sync_event_bus.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus_engine/__init__.py
--rw-r--r--   0        0        0     3196 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus_engine/kombu_event_bus_engine.py
--rw-r--r--   0        0        0     1625 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus_engine/memory_queue_event_bus_engine.py
--rw-r--r--   0        0        0      249 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/event.py
--rw-r--r--   0        0        0      446 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/event_consumer.py
--rw-r--r--   0        0        0      221 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/event_consumer_not_found.py
--rw-r--r--   0        0        0     1439 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/event_consumer_registry.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/middleware/__init__.py
--rw-r--r--   0        0        0      590 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/middleware/event_middleware.py
--rw-r--r--   0        0        0     1049 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/middleware/event_middleware_receiver.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/middleware/implementations/__init__.py
--rw-r--r--   0        0        0     1038 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/middleware/implementations/logging_event_middleware.py
--rw-r--r--   0        0        0     1012 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/middleware/implementations/timing_event_middleware.py
--rw-r--r--   0        0        0      864 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/middleware/implementations/tracking_event_middleware.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/__init__.py
--rw-r--r--   0        0        0     1440 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/memory_queue_passenger_worker.py
--rw-r--r--   0        0        0     2319 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/passenger.py
--rw-r--r--   0        0        0     2042 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/passenger_kombu_consumer.py
--rw-r--r--   0        0        0     2294 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/passenger_mapper.py
--rw-r--r--   0        0        0       76 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/passenger_middleware.py
--rw-r--r--   0        0        0      637 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/passenger_registry.py
--rw-r--r--   0        0        0      641 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/passenger_resolvers.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/reception/__init__.py
--rw-r--r--   0        0        0     1386 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/reception/passenger_middleware_receiver.py
--rw-r--r--   0        0        0      792 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/reception/passenger_receiver.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/serialization/__init__.py
--rw-r--r--   0        0        0      347 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/serialization/passenger_deserialization_error.py
--rw-r--r--   0        0        0      321 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/serialization/passenger_deserializer.py
--rw-r--r--   0        0        0     1016 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/serialization/passenger_json_deserializer.py
--rw-r--r--   0        0        0      822 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/serialization/passenger_json_serializer.py
--rw-r--r--   0        0        0      241 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/serialization/passenger_serializer.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/query_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/query_terminal/bus/__init__.py
--rw-r--r--   0        0        0      323 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/query_terminal/bus/query_bus.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/query_terminal/bus/synchronous/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/query_terminal/bus/synchronous/distributed/__init__.py
--rw-r--r--   0        0        0     2671 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/bus/synchronous/distributed/json_rpc_query_bus.py
--rw-r--r--   0        0        0     2580 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/bus/synchronous/distributed/rpyc_query_bus.py
--rw-r--r--   0        0        0     1127 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/bus/synchronous/sync_query_bus.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/bus_engine/__init__.py
--rw-r--r--   0        0        0     1242 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/bus_engine/json_rpc_query_bus_engine.py
--rw-r--r--   0        0        0     1218 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/bus_engine/rpyc_query_bus_engine.py
--rw-r--r--   0        0        0      219 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/handler_not_found_for_query.py
--rw-r--r--   0        0        0     1483 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/json_rpc_query_server.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/middleware/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/middleware/implementations/__init__.py
--rw-r--r--   0        0        0     1261 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/middleware/implementations/logging_query_middleware.py
--rw-r--r--   0        0        0     1178 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/middleware/implementations/timing_query_middleware.py
--rw-r--r--   0        0        0     1227 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/middleware/implementations/tracking_query_middleware.py
--rw-r--r--   0        0        0      726 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/middleware/query_middleware.py
--rw-r--r--   0        0        0     1286 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/middleware/query_middleware_receiver.py
--rw-r--r--   0        0        0      249 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/query.py
--rw-r--r--   0        0        0      273 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/query_execution_failed.py
--rw-r--r--   0        0        0      520 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/query_handler.py
--rw-r--r--   0        0        0      215 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/query_handler_not_found.py
--rw-r--r--   0        0        0     1747 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/query_handler_registry.py
--rw-r--r--   0        0        0      138 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/query_response.py
--rw-r--r--   0        0        0     1442 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/rpyc_query_server.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/serialization/__init__.py
--rw-r--r--   0        0        0      282 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/serialization/query_response_deserializer.py
--rw-r--r--   0        0        0      465 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/serialization/query_response_json_deserializer.py
--rw-r--r--   0        0        0      390 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/serialization/query_response_json_serializer.py
--rw-r--r--   0        0        0      267 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/serialization/query_response_serializer.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/broker_connection/__init__.py
--rw-r--r--   0        0        0      352 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/broker_connection/broker_connection_type.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/broker_connection/connection_parameters/__init__.py
--rw-r--r--   0        0        0      176 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/broker_connection/connection_parameters/connection_parameters.py
--rw-r--r--   0        0        0     1249 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/broker_connection/connection_parameters/rabbitmq_connection_parameters.py
--rw-r--r--   0        0        0      695 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/bus.py
--rw-r--r--   0        0        0      438 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/context.py
--rw-r--r--   0        0        0      118 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/dataclass_type.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/engine/__init__.py
--rw-r--r--   0        0        0      181 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/engine/engine.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/engine/runner/__init__.py
--rw-r--r--   0        0        0      436 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/engine/runner/engine_runner.py
--rw-r--r--   0        0        0      805 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/engine/runner/process_engine_runner.py
--rw-r--r--   0        0        0      241 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/engine/runner/self_process_engine_runner.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/factories/__init__.py
--rw-r--r--   0        0        0      381 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/factories/kombu_connection_factory.py
--rw-r--r--   0        0        0      545 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/factories/memory_queue_factory.py
--rw-r--r--   0        0        0      305 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/fqn.py
--rw-r--r--   0        0        0     2493 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/json_rpc_server.py
--rw-r--r--   0        0        0      956 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/kafka_topic_creator.py
--rw-r--r--   0        0        0     2037 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/rpyc_server.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/models/__init__.py
--rw-r--r--   0        0        0      185 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/models/command_tracking.py
--rw-r--r--   0        0        0      183 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/models/event_tracking.py
--rw-r--r--   0        0        0      950 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/models/passenger_model_tracking_map.py
--rw-r--r--   0        0        0      347 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/models/passenger_tracking.py
--rw-r--r--   0        0        0      744 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/models/passenger_tracking_json_serializer.py
--rw-r--r--   0        0        0      297 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/models/passenger_tracking_serializer.py
--rw-r--r--   0        0        0      281 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/models/query_tracking.py
--rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/trackers/__init__.py
--rw-r--r--   0        0        0     1400 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/trackers/kafka_passenger_tracker.py
--rw-r--r--   0        0        0     2483 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/trackers/passenger_tracker.py
--rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 bus_station-6.1.3/PKG-INFO
+-rw-r--r--   0        0        0       48 2023-07-13 23:33:57.396474 bus_station-7.0.0/README.md
+-rw-r--r--   0        0        0      954 2023-07-13 23:35:30.112864 bus_station-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/bus_stop/__init__.py
+-rw-r--r--   0        0        0      937 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/bus_stop/bus_stop.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/bus_stop/registration/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/bus_stop/registration/address/__init__.py
+-rw-r--r--   0        0        0      214 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/bus_stop/registration/address/address_not_found_for_passenger.py
+-rw-r--r--   0        0        0      653 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/bus_stop/registration/address/bus_stop_address_registry.py
+-rw-r--r--   0        0        0     1299 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/bus_stop/registration/address/redis_bus_stop_address_registry.py
+-rw-r--r--   0        0        0     1597 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/bus_stop/registration/bus_stop_registry.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/bus/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/bus/asynchronous/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/bus/asynchronous/distributed/__init__.py
+-rw-r--r--   0        0        0     1352 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/bus/asynchronous/distributed/kombu_command_bus.py
+-rw-r--r--   0        0        0      889 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/bus/asynchronous/memory_queue_command_bus.py
+-rw-r--r--   0        0        0     1237 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/bus/asynchronous/threaded_command_bus.py
+-rw-r--r--   0        0        0      258 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/bus/command_bus.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/bus/synchronous/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/bus/synchronous/distributed/__init__.py
+-rw-r--r--   0        0        0     1880 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/bus/synchronous/distributed/json_rpc_command_bus.py
+-rw-r--r--   0        0        0     1753 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/bus/synchronous/distributed/rpyc_command_bus.py
+-rw-r--r--   0        0        0     1128 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/bus/synchronous/sync_command_bus.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/bus_engine/__init__.py
+-rw-r--r--   0        0        0     1185 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/bus_engine/json_rpc_command_bus_engine.py
+-rw-r--r--   0        0        0     2606 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/bus_engine/kombu_command_bus_engine.py
+-rw-r--r--   0        0        0     1715 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/bus_engine/memory_queue_command_bus_engine.py
+-rw-r--r--   0        0        0     1125 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/bus_engine/rpyc_command_bus_engine.py
+-rw-r--r--   0        0        0      253 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/command.py
+-rw-r--r--   0        0        0      292 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/command_execution_failed.py
+-rw-r--r--   0        0        0      648 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/command_handler.py
+-rw-r--r--   0        0        0      227 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/command_handler_not_found.py
+-rw-r--r--   0        0        0      973 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/command_handler_registry.py
+-rw-r--r--   0        0        0      233 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/handler_not_found_for_command.py
+-rw-r--r--   0        0        0      725 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/json_rpc_command_server.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/middleware/__init__.py
+-rw-r--r--   0        0        0      607 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/middleware/command_middleware.py
+-rw-r--r--   0        0        0     1078 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/middleware/command_middleware_receiver.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/middleware/implementations/__init__.py
+-rw-r--r--   0        0        0     1070 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/middleware/implementations/logging_command_middleware.py
+-rw-r--r--   0        0        0     1039 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/middleware/implementations/timing_command_middleware.py
+-rw-r--r--   0        0        0      890 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/middleware/implementations/tracking_command_middleware.py
+-rw-r--r--   0        0        0      712 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/command_terminal/rpyc_command_server.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/event_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/event_terminal/bus/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/event_terminal/bus/asynchronous/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/event_terminal/bus/asynchronous/distributed/__init__.py
+-rw-r--r--   0        0        0     1247 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/event_terminal/bus/asynchronous/distributed/kombu_event_bus.py
+-rw-r--r--   0        0        0     1212 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/event_terminal/bus/asynchronous/memory_queue_event_bus.py
+-rw-r--r--   0        0        0      984 2023-07-13 23:33:57.396474 bus_station-7.0.0/src/bus_station/event_terminal/bus/asynchronous/threaded_event_bus.py
+-rw-r--r--   0        0        0      246 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/event_terminal/bus/event_bus.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/event_terminal/bus/synchronous/__init__.py
+-rw-r--r--   0        0        0      872 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/event_terminal/bus/synchronous/sync_event_bus.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/event_terminal/bus_engine/__init__.py
+-rw-r--r--   0        0        0     3056 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/event_terminal/bus_engine/kombu_event_bus_engine.py
+-rw-r--r--   0        0        0     1625 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/event_terminal/bus_engine/memory_queue_event_bus_engine.py
+-rw-r--r--   0        0        0      249 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/event_terminal/event.py
+-rw-r--r--   0        0        0      634 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/event_terminal/event_consumer.py
+-rw-r--r--   0        0        0      221 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/event_terminal/event_consumer_not_found.py
+-rw-r--r--   0        0        0      742 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/event_terminal/event_consumer_registry.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/event_terminal/middleware/__init__.py
+-rw-r--r--   0        0        0      590 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/event_terminal/middleware/event_middleware.py
+-rw-r--r--   0        0        0     1049 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/event_terminal/middleware/event_middleware_receiver.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/event_terminal/middleware/implementations/__init__.py
+-rw-r--r--   0        0        0     1038 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/event_terminal/middleware/implementations/logging_event_middleware.py
+-rw-r--r--   0        0        0     1012 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/event_terminal/middleware/implementations/timing_event_middleware.py
+-rw-r--r--   0        0        0      864 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/event_terminal/middleware/implementations/tracking_event_middleware.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/passengers/__init__.py
+-rw-r--r--   0        0        0     1440 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/passengers/memory_queue_passenger_worker.py
+-rw-r--r--   0        0        0     2319 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/passengers/passenger.py
+-rw-r--r--   0        0        0     2042 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/passengers/passenger_kombu_consumer.py
+-rw-r--r--   0        0        0     2294 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/passengers/passenger_mapper.py
+-rw-r--r--   0        0        0       76 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/passengers/passenger_middleware.py
+-rw-r--r--   0        0        0      645 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/passengers/passenger_registry.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/passengers/reception/__init__.py
+-rw-r--r--   0        0        0     1386 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/passengers/reception/passenger_middleware_receiver.py
+-rw-r--r--   0        0        0      792 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/passengers/reception/passenger_receiver.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/passengers/serialization/__init__.py
+-rw-r--r--   0        0        0      347 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/passengers/serialization/passenger_deserialization_error.py
+-rw-r--r--   0        0        0      321 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/passengers/serialization/passenger_deserializer.py
+-rw-r--r--   0        0        0     1016 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/passengers/serialization/passenger_json_deserializer.py
+-rw-r--r--   0        0        0      822 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/passengers/serialization/passenger_json_serializer.py
+-rw-r--r--   0        0        0      241 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/passengers/serialization/passenger_serializer.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/bus/__init__.py
+-rw-r--r--   0        0        0      323 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/bus/query_bus.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/bus/synchronous/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/bus/synchronous/distributed/__init__.py
+-rw-r--r--   0        0        0     2256 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/bus/synchronous/distributed/json_rpc_query_bus.py
+-rw-r--r--   0        0        0     2165 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/bus/synchronous/distributed/rpyc_query_bus.py
+-rw-r--r--   0        0        0     1127 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/bus/synchronous/sync_query_bus.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/bus_engine/__init__.py
+-rw-r--r--   0        0        0     1103 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/bus_engine/json_rpc_query_bus_engine.py
+-rw-r--r--   0        0        0     1079 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/bus_engine/rpyc_query_bus_engine.py
+-rw-r--r--   0        0        0      219 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/handler_not_found_for_query.py
+-rw-r--r--   0        0        0     1483 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/json_rpc_query_server.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/middleware/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/middleware/implementations/__init__.py
+-rw-r--r--   0        0        0     1261 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/middleware/implementations/logging_query_middleware.py
+-rw-r--r--   0        0        0     1178 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/middleware/implementations/timing_query_middleware.py
+-rw-r--r--   0        0        0     1227 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/middleware/implementations/tracking_query_middleware.py
+-rw-r--r--   0        0        0      726 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/middleware/query_middleware.py
+-rw-r--r--   0        0        0     1286 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/middleware/query_middleware_receiver.py
+-rw-r--r--   0        0        0      249 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/query.py
+-rw-r--r--   0        0        0      273 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/query_execution_failed.py
+-rw-r--r--   0        0        0      707 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/query_handler.py
+-rw-r--r--   0        0        0      215 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/query_handler_not_found.py
+-rw-r--r--   0        0        0      926 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/query_handler_registry.py
+-rw-r--r--   0        0        0      138 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/query_response.py
+-rw-r--r--   0        0        0     1442 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/rpyc_query_server.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/serialization/__init__.py
+-rw-r--r--   0        0        0      282 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/serialization/query_response_deserializer.py
+-rw-r--r--   0        0        0      465 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/serialization/query_response_json_deserializer.py
+-rw-r--r--   0        0        0      390 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/serialization/query_response_json_serializer.py
+-rw-r--r--   0        0        0      267 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/query_terminal/serialization/query_response_serializer.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/broker_connection/__init__.py
+-rw-r--r--   0        0        0      352 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/broker_connection/broker_connection_type.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/broker_connection/connection_parameters/__init__.py
+-rw-r--r--   0        0        0      176 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/broker_connection/connection_parameters/connection_parameters.py
+-rw-r--r--   0        0        0     1249 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/broker_connection/connection_parameters/rabbitmq_connection_parameters.py
+-rw-r--r--   0        0        0      695 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/bus.py
+-rw-r--r--   0        0        0      438 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/context.py
+-rw-r--r--   0        0        0      118 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/dataclass_type.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/engine/__init__.py
+-rw-r--r--   0        0        0      181 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/engine/engine.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/engine/runner/__init__.py
+-rw-r--r--   0        0        0      436 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/engine/runner/engine_runner.py
+-rw-r--r--   0        0        0      805 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/engine/runner/process_engine_runner.py
+-rw-r--r--   0        0        0      241 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/engine/runner/self_process_engine_runner.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/factories/__init__.py
+-rw-r--r--   0        0        0      381 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/factories/kombu_connection_factory.py
+-rw-r--r--   0        0        0      545 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/factories/memory_queue_factory.py
+-rw-r--r--   0        0        0     2493 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/json_rpc_server.py
+-rw-r--r--   0        0        0      956 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/kafka_topic_creator.py
+-rw-r--r--   0        0        0     2037 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/shared_terminal/rpyc_server.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/tracking_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/tracking_terminal/models/__init__.py
+-rw-r--r--   0        0        0      185 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/tracking_terminal/models/command_tracking.py
+-rw-r--r--   0        0        0      183 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/tracking_terminal/models/event_tracking.py
+-rw-r--r--   0        0        0      950 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/tracking_terminal/models/passenger_model_tracking_map.py
+-rw-r--r--   0        0        0      347 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/tracking_terminal/models/passenger_tracking.py
+-rw-r--r--   0        0        0      744 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/tracking_terminal/models/passenger_tracking_json_serializer.py
+-rw-r--r--   0        0        0      297 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/tracking_terminal/models/passenger_tracking_serializer.py
+-rw-r--r--   0        0        0      281 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/tracking_terminal/models/query_tracking.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/tracking_terminal/trackers/__init__.py
+-rw-r--r--   0        0        0     1400 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/tracking_terminal/trackers/kafka_passenger_tracker.py
+-rw-r--r--   0        0        0     2483 2023-07-13 23:33:57.400474 bus_station-7.0.0/src/bus_station/tracking_terminal/trackers/passenger_tracker.py
+-rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 bus_station-7.0.0/PKG-INFO
```

### Comparing `bus_station-6.1.3/pyproject.toml` & `bus_station-7.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 [tool.poetry]
 name = "bus-station"
-version = "6.1.3"
+version = "7.0.0"
 description = "A python bus station"
 readme = "README.md"
 authors = ["DeejayRevok <seryi_one@hotmail.com>"]
 
 [tool.poetry.dependencies]
 python = "~=3.10.0"
 kombu = "5.2.2"
 redis = "4.4.4"
-rpyc = "5.0.1"
-jsonrpcserver = "^5.0.6"
-jsonrpcclient = "^4.0.2"
+rpyc = "^5.3.1"
+jsonrpcserver = "^5.0.9"
+jsonrpcclient = "^4.0.3"
 requests = "^2.27.1"
-pypendency = "~0"
 confluent-kafka = "^2.1.1"
 freezegun = "^1.2.2"
-yandil = "~0"
 
 [tool.poetry.dev-dependencies]
 black = "22.1.0"
 coverage = "5.3"
 flake8 = "3.8.4"
 pyre-check = "0.9.18"
 tox = "3.20.1"
@@ -41,15 +39,15 @@
 [tool.isort]
 profile = "black"
 py_version=310
 line_length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "6.1.3"
+version = "7.0.0"
 tag_format = "$version"
 version_files = [
   "pyproject.toml:version"
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `bus_station-6.1.3/src/bus_station/bus_stop/registration/address/redis_bus_stop_address_registry.py` & `bus_station-7.0.0/src/bus_station/bus_stop/registration/address/redis_bus_stop_address_registry.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,29 @@
-from typing import Optional
+from typing import Optional, Type, TypeVar
 
 from redis.client import Redis
 
+from bus_station.bus_stop.bus_stop import BusStop
 from bus_station.bus_stop.registration.address.bus_stop_address_registry import BusStopAddressRegistry
+from bus_station.passengers.passenger import Passenger
+
+BT = TypeVar("BT", bound=BusStop)
+PT = TypeVar("PT", bound=Passenger)
 
 
 class RedisBusStopAddressRegistry(BusStopAddressRegistry):
     def __init__(self, redis_client: Redis):
         self.__redis_client = redis_client
 
-    def register(self, bus_stop_id: str, address: str) -> None:
-        self.__redis_client.set(bus_stop_id, address)
-
-    def get_bus_stop_address(self, bus_stop_id: str) -> Optional[str]:
-        return self.__redis_client.get(bus_stop_id).decode("UTF-8")
-
-    def unregister(self, bus_stop_id: str) -> None:
-        self.__redis_client.delete(bus_stop_id)
+    def register(self, bus_stop_class: Type[BT], address: str) -> None:
+        bus_stop_name = bus_stop_class.bus_stop_name()
+        passenger_name = bus_stop_class.passenger().passenger_name()
+        self.__redis_client.set(passenger_name, bus_stop_name)
+        self.__redis_client.set(bus_stop_name, address)
+
+    def get_address_for_bus_stop_passenger_class(self, bus_stop_passenger_class: Type[PT]) -> Optional[str]:
+        bus_stop_name = self.__redis_client.get(bus_stop_passenger_class.passenger_name())
+        return self.__redis_client.get(bus_stop_name).decode("UTF-8")
+
+    def unregister(self, bus_stop_class: Type[BT]) -> None:
+        self.__redis_client.delete(bus_stop_class.passenger().passenger_name())
+        self.__redis_client.delete(bus_stop_class.bus_stop_name())
```

### Comparing `bus_station-6.1.3/src/bus_station/command_terminal/bus/asynchronous/distributed/kombu_command_bus.py` & `bus_station-7.0.0/src/bus_station/command_terminal/bus/asynchronous/distributed/kombu_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/command_terminal/bus/asynchronous/memory_queue_command_bus.py` & `bus_station-7.0.0/src/bus_station/command_terminal/bus/asynchronous/memory_queue_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/command_terminal/bus/asynchronous/threaded_command_bus.py` & `bus_station-7.0.0/src/bus_station/command_terminal/bus/asynchronous/threaded_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/command_terminal/bus/synchronous/distributed/json_rpc_command_bus.py` & `bus_station-7.0.0/src/bus_station/command_terminal/bus/synchronous/distributed/json_rpc_command_bus.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import requests
 from jsonrpcclient import Error, parse, request
 
-from bus_station.bus_stop.registration.address.address_not_found_for_bus_stop import AddressNotFoundForBusStop
+from bus_station.bus_stop.registration.address.address_not_found_for_passenger import AddressNotFoundForPassenger
 from bus_station.bus_stop.registration.address.bus_stop_address_registry import BusStopAddressRegistry
 from bus_station.command_terminal.bus.command_bus import CommandBus
 from bus_station.command_terminal.command import Command
 from bus_station.command_terminal.command_execution_failed import CommandExecutionFailed
-from bus_station.command_terminal.handler_not_found_for_command import HandlerNotFoundForCommand
-from bus_station.passengers.passenger_registry import passenger_bus_stop_registry
 from bus_station.passengers.serialization.passenger_serializer import PassengerSerializer
 
 
 class JsonRPCCommandBus(CommandBus):
     def __init__(
         self,
         command_serializer: PassengerSerializer,
@@ -22,22 +20,17 @@
 
     def _transport(self, passenger: Command) -> None:
         handler_address = self.__get_handler_address(passenger)
 
         self.__execute_command(passenger, handler_address)
 
     def __get_handler_address(self, passenger: Command) -> str:
-        command_handler_ids = passenger_bus_stop_registry.get_bus_stops_for_passenger(passenger.passenger_name())
-        if len(command_handler_ids) == 0:
-            raise HandlerNotFoundForCommand(passenger.passenger_name())
-
-        command_handler_id = next(iter(command_handler_ids))
-        handler_address = self.__address_registry.get_bus_stop_address(command_handler_id)
+        handler_address = self.__address_registry.get_address_for_bus_stop_passenger_class(passenger.__class__)
         if handler_address is None:
-            raise AddressNotFoundForBusStop(command_handler_id)
+            raise AddressNotFoundForPassenger(passenger.passenger_name())
 
         return handler_address
 
     def __execute_command(self, command: Command, command_handler_addr: str) -> None:
         serialized_command = self.__command_serializer.serialize(command)
 
         request_response = requests.post(
```

### Comparing `bus_station-6.1.3/src/bus_station/command_terminal/bus/synchronous/distributed/rpyc_command_bus.py` & `bus_station-7.0.0/src/bus_station/command_terminal/bus/synchronous/distributed/rpyc_command_bus.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from rpyc import Connection, connect
 
-from bus_station.bus_stop.registration.address.address_not_found_for_bus_stop import AddressNotFoundForBusStop
+from bus_station.bus_stop.registration.address.address_not_found_for_passenger import AddressNotFoundForPassenger
 from bus_station.bus_stop.registration.address.bus_stop_address_registry import BusStopAddressRegistry
 from bus_station.command_terminal.bus.command_bus import CommandBus
 from bus_station.command_terminal.command import Command
-from bus_station.command_terminal.handler_not_found_for_command import HandlerNotFoundForCommand
-from bus_station.passengers.passenger_registry import passenger_bus_stop_registry
 from bus_station.passengers.serialization.passenger_serializer import PassengerSerializer
 
 
 class RPyCCommandBus(CommandBus):
     def __init__(
         self,
         command_serializer: PassengerSerializer,
@@ -23,22 +21,17 @@
 
         rpyc_client = self.__get_rpyc_client(handler_address)
         self.__execute_command(rpyc_client, passenger)
 
         rpyc_client.close()
 
     def __get_handler_address(self, passenger: Command) -> str:
-        command_handler_ids = passenger_bus_stop_registry.get_bus_stops_for_passenger(passenger.passenger_name())
-        if len(command_handler_ids) == 0:
-            raise HandlerNotFoundForCommand(passenger.passenger_name())
-
-        command_handler_id = next(iter(command_handler_ids))
-        handler_address = self.__address_registry.get_bus_stop_address(command_handler_id)
+        handler_address = self.__address_registry.get_address_for_bus_stop_passenger_class(passenger.__class__)
         if handler_address is None:
-            raise AddressNotFoundForBusStop(command_handler_id)
+            raise AddressNotFoundForPassenger(passenger.passenger_name())
 
         return handler_address
 
     def __get_rpyc_client(self, handler_addr: str) -> Connection:
         host, port = handler_addr.split(":")
         return connect(host, port=port, config={"allow_public_attrs": True})
```

### Comparing `bus_station-6.1.3/src/bus_station/command_terminal/bus/synchronous/sync_command_bus.py` & `bus_station-7.0.0/src/bus_station/command_terminal/bus/synchronous/sync_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/command_terminal/bus_engine/json_rpc_command_bus_engine.py` & `bus_station-7.0.0/src/bus_station/command_terminal/bus_engine/json_rpc_command_bus_engine.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from bus_station.command_terminal.command_handler_not_found import CommandHandlerNotFound
 from bus_station.command_terminal.command_handler_registry import CommandHandlerRegistry
 from bus_station.command_terminal.json_rpc_command_server import JsonRPCCommandServer
-from bus_station.passengers.passenger_resolvers import resolve_passenger_class_from_bus_stop
 from bus_station.shared_terminal.engine.engine import Engine
 
 
 class JsonRPCCommandBusEngine(Engine):
     def __init__(
         self,
         server: JsonRPCCommandServer,
@@ -18,15 +17,15 @@
     def __register_command_handler_in_server(
         self, command_handler_registry: CommandHandlerRegistry, command_handler_name: str
     ) -> None:
         handler = command_handler_registry.get_bus_stop_by_name(command_handler_name)
         if handler is None:
             raise CommandHandlerNotFound(command_handler_name)
 
-        command_type = resolve_passenger_class_from_bus_stop(handler, "handle", "command")
+        command_type = handler.passenger()
         self.__server.register(command_type, handler)
 
     def start(self) -> None:
         self.__server.run()
 
     def stop(self):
         pass
```

### Comparing `bus_station-6.1.3/src/bus_station/command_terminal/bus_engine/kombu_command_bus_engine.py` & `bus_station-7.0.0/src/bus_station/command_terminal/bus_engine/kombu_command_bus_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from kombu.transport.base import StdChannel
 
 from bus_station.command_terminal.command import Command
 from bus_station.command_terminal.command_handler import CommandHandler
 from bus_station.command_terminal.command_handler_not_found import CommandHandlerNotFound
 from bus_station.command_terminal.command_handler_registry import CommandHandlerRegistry
 from bus_station.passengers.passenger_kombu_consumer import PassengerKombuConsumer
-from bus_station.passengers.passenger_resolvers import resolve_passenger_class_from_bus_stop
 from bus_station.passengers.reception.passenger_receiver import PassengerReceiver
 from bus_station.passengers.serialization.passenger_deserializer import PassengerDeserializer
 from bus_station.shared_terminal.engine.engine import Engine
 
 
 class KombuCommandBusEngine(Engine):
     __DEAD_LETTER_EXCHANGE_NAME: ClassVar = "failed_commands"
@@ -25,15 +24,15 @@
         command_deserializer: PassengerDeserializer,
         command_handler_name: str,
     ):
         command_handler = command_handler_registry.get_bus_stop_by_name(command_handler_name)
         if command_handler is None:
             raise CommandHandlerNotFound(command_handler_name)
 
-        command_type = resolve_passenger_class_from_bus_stop(command_handler, "handle", "command")
+        command_type = command_handler.passenger()
         channel = broker_connection.channel()
         self.__create_dead_letter_exchange(channel)
 
         command_queue = self.__create_command_handler_queue(command_type.passenger_name(), channel)
 
         self.__command_consumer = PassengerKombuConsumer(
             broker_connection,
```

### Comparing `bus_station-6.1.3/src/bus_station/command_terminal/bus_engine/memory_queue_command_bus_engine.py` & `bus_station-7.0.0/src/bus_station/command_terminal/bus_engine/memory_queue_command_bus_engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from bus_station.command_terminal.command import Command
 from bus_station.command_terminal.command_handler import CommandHandler
 from bus_station.command_terminal.command_handler_not_found import CommandHandlerNotFound
 from bus_station.command_terminal.command_handler_registry import CommandHandlerRegistry
 from bus_station.passengers.memory_queue_passenger_worker import MemoryQueuePassengerWorker
-from bus_station.passengers.passenger_resolvers import resolve_passenger_class_from_bus_stop
 from bus_station.passengers.reception.passenger_receiver import PassengerReceiver
 from bus_station.passengers.serialization.passenger_deserializer import PassengerDeserializer
 from bus_station.shared_terminal.engine.engine import Engine
 from bus_station.shared_terminal.factories.memory_queue_factory import memory_queue_factory
 
 
 class MemoryQueueCommandBusEngine(Engine):
@@ -18,15 +17,15 @@
         command_deserializer: PassengerDeserializer,
         command_handler_name: str,
     ):
         command_handler = command_handler_registry.get_bus_stop_by_name(command_handler_name)
         if command_handler is None:
             raise CommandHandlerNotFound(command_handler_name)
 
-        command = resolve_passenger_class_from_bus_stop(command_handler, "handle", "command")
+        command = command_handler.passenger()
         command_queue = memory_queue_factory.queue_with_id(command.passenger_name())
         self.__command_worker = MemoryQueuePassengerWorker(
             command_queue, command_handler, command_receiver, command_deserializer
         )
 
     def start(self) -> None:
         try:
```

### Comparing `bus_station-6.1.3/src/bus_station/command_terminal/bus_engine/rpyc_command_bus_engine.py` & `bus_station-7.0.0/src/bus_station/command_terminal/bus_engine/rpyc_command_bus_engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bus_station.command_terminal.command_handler_not_found import CommandHandlerNotFound
 from bus_station.command_terminal.command_handler_registry import CommandHandlerRegistry
-from bus_station.passengers.passenger_resolvers import resolve_passenger_class_from_bus_stop
 from bus_station.shared_terminal.engine.engine import Engine
 from bus_station.shared_terminal.rpyc_server import RPyCServer
 
 
 class RPyCCommandBusEngine(Engine):
     def __init__(
         self, rpyc_server: RPyCServer, command_handler_registry: CommandHandlerRegistry, command_handler_name: str
@@ -14,15 +13,15 @@
 
     def __register_command_in_server(
         self, command_handler_registry: CommandHandlerRegistry, command_handler_name: str
     ) -> None:
         handler = command_handler_registry.get_bus_stop_by_name(command_handler_name)
         if handler is None:
             raise CommandHandlerNotFound(command_handler_name)
-        command_type = resolve_passenger_class_from_bus_stop(handler, "handle", "command")
+        command_type = handler.passenger()
         self.__server.register(command_type, handler)
 
     def start(self) -> None:
         self.__server.run()
 
     def stop(self) -> None:
         pass
```

### Comparing `bus_station-6.1.3/src/bus_station/command_terminal/json_rpc_command_server.py` & `bus_station-7.0.0/src/bus_station/command_terminal/json_rpc_command_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/command_terminal/middleware/command_middleware.py` & `bus_station-7.0.0/src/bus_station/command_terminal/middleware/command_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/command_terminal/middleware/command_middleware_receiver.py` & `bus_station-7.0.0/src/bus_station/command_terminal/middleware/command_middleware_receiver.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/command_terminal/middleware/implementations/logging_command_middleware.py` & `bus_station-7.0.0/src/bus_station/command_terminal/middleware/implementations/logging_command_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/command_terminal/middleware/implementations/timing_command_middleware.py` & `bus_station-7.0.0/src/bus_station/command_terminal/middleware/implementations/timing_command_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/command_terminal/middleware/implementations/tracking_command_middleware.py` & `bus_station-7.0.0/src/bus_station/command_terminal/middleware/implementations/tracking_command_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/command_terminal/rpyc_command_server.py` & `bus_station-7.0.0/src/bus_station/command_terminal/rpyc_command_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/event_terminal/bus/asynchronous/distributed/kombu_event_bus.py` & `bus_station-7.0.0/src/bus_station/event_terminal/bus/asynchronous/distributed/kombu_event_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/event_terminal/bus/asynchronous/memory_queue_event_bus.py` & `bus_station-7.0.0/src/bus_station/event_terminal/bus/asynchronous/memory_queue_event_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/event_terminal/bus/asynchronous/threaded_event_bus.py` & `bus_station-7.0.0/src/bus_station/event_terminal/bus/asynchronous/threaded_event_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/event_terminal/bus/synchronous/sync_event_bus.py` & `bus_station-7.0.0/src/bus_station/event_terminal/bus/synchronous/sync_event_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/event_terminal/bus_engine/kombu_event_bus_engine.py` & `bus_station-7.0.0/src/bus_station/event_terminal/bus_engine/kombu_event_bus_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from kombu.transport.base import StdChannel
 
 from bus_station.event_terminal.event import Event
 from bus_station.event_terminal.event_consumer import EventConsumer
 from bus_station.event_terminal.event_consumer_not_found import EventConsumerNotFound
 from bus_station.event_terminal.event_consumer_registry import EventConsumerRegistry
 from bus_station.passengers.passenger_kombu_consumer import PassengerKombuConsumer
-from bus_station.passengers.passenger_resolvers import resolve_passenger_class_from_bus_stop
 from bus_station.passengers.reception.passenger_receiver import PassengerReceiver
 from bus_station.passengers.serialization.passenger_deserializer import PassengerDeserializer
 from bus_station.shared_terminal.engine.engine import Engine
 
 
 class KombuEventBusEngine(Engine):
     __DEAD_LETTER_EXCHANGE_NAME: ClassVar = "failed_events"
@@ -25,15 +24,15 @@
         event_deserializer: PassengerDeserializer,
         event_consumer_name: str,
     ):
         event_consumer = event_consumer_registry.get_bus_stop_by_name(event_consumer_name)
         if event_consumer is None:
             raise EventConsumerNotFound(event_consumer_name)
 
-        event = resolve_passenger_class_from_bus_stop(event_consumer, "consume", "event")
+        event = event_consumer.passenger()
 
         channel = broker_connection.channel()
         self.__create_dead_letter_exchange(channel)
 
         event_exchange = self.__create_event_consumer_exchange(event.passenger_name(), channel)
         event_consumer_queue = self.__create_event_consumer_queue(event_consumer, event_exchange, channel)
```

### Comparing `bus_station-6.1.3/src/bus_station/event_terminal/bus_engine/memory_queue_event_bus_engine.py` & `bus_station-7.0.0/src/bus_station/event_terminal/bus_engine/memory_queue_event_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/event_terminal/middleware/event_middleware.py` & `bus_station-7.0.0/src/bus_station/event_terminal/middleware/event_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/event_terminal/middleware/event_middleware_receiver.py` & `bus_station-7.0.0/src/bus_station/event_terminal/middleware/event_middleware_receiver.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/event_terminal/middleware/implementations/logging_event_middleware.py` & `bus_station-7.0.0/src/bus_station/event_terminal/middleware/implementations/logging_event_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/event_terminal/middleware/implementations/timing_event_middleware.py` & `bus_station-7.0.0/src/bus_station/event_terminal/middleware/implementations/timing_event_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/event_terminal/middleware/implementations/tracking_event_middleware.py` & `bus_station-7.0.0/src/bus_station/event_terminal/middleware/implementations/tracking_event_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/passengers/memory_queue_passenger_worker.py` & `bus_station-7.0.0/src/bus_station/passengers/memory_queue_passenger_worker.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/passengers/passenger.py` & `bus_station-7.0.0/src/bus_station/passengers/passenger.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/passengers/passenger_kombu_consumer.py` & `bus_station-7.0.0/src/bus_station/passengers/passenger_kombu_consumer.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/passengers/passenger_mapper.py` & `bus_station-7.0.0/src/bus_station/passengers/passenger_mapper.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/passengers/passenger_registry.py` & `bus_station-7.0.0/src/bus_station/passengers/passenger_registry.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from typing import Dict, Set
 
 
 class __PassengerBusStopRegistry:
     def __init__(self):
         self.__registry: Dict[str, Set[str]] = defaultdict(set)
 
-    def register(self, passenger_name: str, bus_stop_id: str) -> None:
-        self.__registry[passenger_name].add(bus_stop_id)
+    def register(self, passenger_name: str, bus_stop_name: str) -> None:
+        self.__registry[passenger_name].add(bus_stop_name)
 
     def get_bus_stops_for_passenger(self, passenger_name: str) -> Set[str]:
         return self.__registry[passenger_name]
 
-    def unregister(self, passenger_name: str, bus_stop_id: str) -> None:
-        self.__registry[passenger_name].remove(bus_stop_id)
+    def unregister(self, passenger_name: str, bus_stop_name: str) -> None:
+        self.__registry[passenger_name].remove(bus_stop_name)
 
 
 passenger_bus_stop_registry = __PassengerBusStopRegistry()
```

### Comparing `bus_station-6.1.3/src/bus_station/passengers/reception/passenger_middleware_receiver.py` & `bus_station-7.0.0/src/bus_station/passengers/reception/passenger_middleware_receiver.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/passengers/reception/passenger_receiver.py` & `bus_station-7.0.0/src/bus_station/passengers/reception/passenger_receiver.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/passengers/serialization/passenger_json_deserializer.py` & `bus_station-7.0.0/src/bus_station/passengers/serialization/passenger_json_deserializer.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/passengers/serialization/passenger_json_serializer.py` & `bus_station-7.0.0/src/bus_station/passengers/serialization/passenger_json_serializer.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/query_terminal/bus/synchronous/distributed/json_rpc_query_bus.py` & `bus_station-7.0.0/src/bus_station/query_terminal/bus/synchronous/distributed/json_rpc_query_bus.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import requests
 from jsonrpcclient import Error, parse, request
 
-from bus_station.bus_stop.registration.address.address_not_found_for_bus_stop import AddressNotFoundForBusStop
+from bus_station.bus_stop.registration.address.address_not_found_for_passenger import AddressNotFoundForPassenger
 from bus_station.bus_stop.registration.address.bus_stop_address_registry import BusStopAddressRegistry
-from bus_station.passengers.passenger_registry import passenger_bus_stop_registry
 from bus_station.passengers.serialization.passenger_serializer import PassengerSerializer
 from bus_station.query_terminal.bus.query_bus import QueryBus
-from bus_station.query_terminal.handler_not_found_for_query import HandlerNotFoundForQuery
 from bus_station.query_terminal.query import Query
 from bus_station.query_terminal.query_execution_failed import QueryExecutionFailed
 from bus_station.query_terminal.query_response import QueryResponse
 from bus_station.query_terminal.serialization.query_response_deserializer import QueryResponseDeserializer
 
 
 class JsonRPCQueryBus(QueryBus):
@@ -25,22 +23,17 @@
         self.__query_response_deserializer = query_response_deserializer
 
     def _transport(self, passenger: Query) -> QueryResponse:
         handler_address = self.__get_handler_address(passenger)
         return self.__execute_query(passenger, handler_address)
 
     def __get_handler_address(self, passenger: Query) -> str:
-        query_handler_ids = passenger_bus_stop_registry.get_bus_stops_for_passenger(passenger.passenger_name())
-        if len(query_handler_ids) == 0:
-            raise HandlerNotFoundForQuery(passenger.passenger_name())
-
-        query_handler_id = next(iter(query_handler_ids))
-        handler_address = self.__address_registry.get_bus_stop_address(query_handler_id)
+        handler_address = self.__address_registry.get_address_for_bus_stop_passenger_class(passenger.__class__)
         if handler_address is None:
-            raise AddressNotFoundForBusStop(query_handler_id)
+            raise AddressNotFoundForPassenger(passenger.passenger_name())
 
         return handler_address
 
     def __execute_query(self, query: Query, query_handler_addr: str) -> QueryResponse:
         serialized_query = self.__query_serializer.serialize(query)
 
         request_response = requests.post(
```

### Comparing `bus_station-6.1.3/src/bus_station/query_terminal/bus/synchronous/distributed/rpyc_query_bus.py` & `bus_station-7.0.0/src/bus_station/query_terminal/bus/synchronous/distributed/rpyc_query_bus.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from rpyc import Connection, connect
 
-from bus_station.bus_stop.registration.address.address_not_found_for_bus_stop import AddressNotFoundForBusStop
+from bus_station.bus_stop.registration.address.address_not_found_for_passenger import AddressNotFoundForPassenger
 from bus_station.bus_stop.registration.address.bus_stop_address_registry import BusStopAddressRegistry
-from bus_station.passengers.passenger_registry import passenger_bus_stop_registry
 from bus_station.passengers.serialization.passenger_serializer import PassengerSerializer
 from bus_station.query_terminal.bus.query_bus import QueryBus
-from bus_station.query_terminal.handler_not_found_for_query import HandlerNotFoundForQuery
 from bus_station.query_terminal.query import Query
 from bus_station.query_terminal.query_response import QueryResponse
 from bus_station.query_terminal.serialization.query_response_deserializer import QueryResponseDeserializer
 
 
 class RPyCQueryBus(QueryBus):
     def __init__(
@@ -27,22 +25,17 @@
 
         rpyc_client = self.__get_rpyc_client(handler_address)
         query_response = self.__execute_query(rpyc_client, passenger)
         rpyc_client.close()
         return query_response
 
     def __get_handler_address(self, passenger: Query) -> str:
-        query_handler_ids = passenger_bus_stop_registry.get_bus_stops_for_passenger(passenger.passenger_name())
-        if len(query_handler_ids) == 0:
-            raise HandlerNotFoundForQuery(passenger.passenger_name())
-
-        query_handler_id = next(iter(query_handler_ids))
-        handler_address = self.__address_registry.get_bus_stop_address(query_handler_id)
+        handler_address = self.__address_registry.get_address_for_bus_stop_passenger_class(passenger.__class__)
         if handler_address is None:
-            raise AddressNotFoundForBusStop(query_handler_id)
+            raise AddressNotFoundForPassenger(passenger.passenger_name())
 
         return handler_address
 
     def __get_rpyc_client(self, handler_addr: str) -> Connection:
         host, port = handler_addr.split(":")
         return connect(host, port=port)
```

### Comparing `bus_station-6.1.3/src/bus_station/query_terminal/bus/synchronous/sync_query_bus.py` & `bus_station-7.0.0/src/bus_station/query_terminal/bus/synchronous/sync_query_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/query_terminal/bus_engine/json_rpc_query_bus_engine.py` & `bus_station-7.0.0/src/bus_station/query_terminal/bus_engine/rpyc_query_bus_engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-from bus_station.passengers.passenger_resolvers import resolve_passenger_class_from_bus_stop
-from bus_station.query_terminal.json_rpc_query_server import JsonRPCQueryServer
 from bus_station.query_terminal.query_handler_not_found import QueryHandlerNotFound
 from bus_station.query_terminal.query_handler_registry import QueryHandlerRegistry
 from bus_station.shared_terminal.engine.engine import Engine
+from bus_station.shared_terminal.rpyc_server import RPyCServer
 
 
-class JsonRPCQueryBusEngine(Engine):
-    def __init__(
-        self, server: JsonRPCQueryServer, query_handler_registry: QueryHandlerRegistry, query_handler_name: str
-    ):
+class RPyCQueryBusEngine(Engine):
+    def __init__(self, rpyc_server: RPyCServer, query_handler_registry: QueryHandlerRegistry, query_handler_name: str):
         super().__init__()
-        self.__server = server
+        self.__server = rpyc_server
         self.__register_query_in_server(query_handler_registry, query_handler_name)
 
     def __register_query_in_server(self, query_handler_registry: QueryHandlerRegistry, query_handler_name: str) -> None:
         handler = query_handler_registry.get_bus_stop_by_name(query_handler_name)
         if handler is None:
             raise QueryHandlerNotFound(query_handler_name)
 
-        query_type = resolve_passenger_class_from_bus_stop(handler, "handle", "query")
+        query_type = handler.passenger()
         self.__server.register(query_type, handler)
 
     def start(self) -> None:
         self.__server.run()
 
-    def stop(self):
+    def stop(self) -> None:
         pass
```

### Comparing `bus_station-6.1.3/src/bus_station/query_terminal/bus_engine/rpyc_query_bus_engine.py` & `bus_station-7.0.0/src/bus_station/query_terminal/bus_engine/json_rpc_query_bus_engine.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from bus_station.passengers.passenger_resolvers import resolve_passenger_class_from_bus_stop
+from bus_station.query_terminal.json_rpc_query_server import JsonRPCQueryServer
 from bus_station.query_terminal.query_handler_not_found import QueryHandlerNotFound
 from bus_station.query_terminal.query_handler_registry import QueryHandlerRegistry
 from bus_station.shared_terminal.engine.engine import Engine
-from bus_station.shared_terminal.rpyc_server import RPyCServer
 
 
-class RPyCQueryBusEngine(Engine):
-    def __init__(self, rpyc_server: RPyCServer, query_handler_registry: QueryHandlerRegistry, query_handler_name: str):
+class JsonRPCQueryBusEngine(Engine):
+    def __init__(
+        self, server: JsonRPCQueryServer, query_handler_registry: QueryHandlerRegistry, query_handler_name: str
+    ):
         super().__init__()
-        self.__server = rpyc_server
+        self.__server = server
         self.__register_query_in_server(query_handler_registry, query_handler_name)
 
     def __register_query_in_server(self, query_handler_registry: QueryHandlerRegistry, query_handler_name: str) -> None:
         handler = query_handler_registry.get_bus_stop_by_name(query_handler_name)
         if handler is None:
             raise QueryHandlerNotFound(query_handler_name)
 
-        query_type = resolve_passenger_class_from_bus_stop(handler, "handle", "query")
+        query_type = handler.passenger()
         self.__server.register(query_type, handler)
 
     def start(self) -> None:
         self.__server.run()
 
-    def stop(self) -> None:
+    def stop(self):
         pass
```

### Comparing `bus_station-6.1.3/src/bus_station/query_terminal/json_rpc_query_server.py` & `bus_station-7.0.0/src/bus_station/query_terminal/json_rpc_query_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/query_terminal/middleware/implementations/logging_query_middleware.py` & `bus_station-7.0.0/src/bus_station/query_terminal/middleware/implementations/logging_query_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/query_terminal/middleware/implementations/timing_query_middleware.py` & `bus_station-7.0.0/src/bus_station/query_terminal/middleware/implementations/timing_query_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/query_terminal/middleware/implementations/tracking_query_middleware.py` & `bus_station-7.0.0/src/bus_station/query_terminal/middleware/implementations/tracking_query_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/query_terminal/middleware/query_middleware.py` & `bus_station-7.0.0/src/bus_station/query_terminal/middleware/query_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/query_terminal/middleware/query_middleware_receiver.py` & `bus_station-7.0.0/src/bus_station/query_terminal/middleware/query_middleware_receiver.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/query_terminal/query_handler_registry.py` & `bus_station-7.0.0/src/bus_station/query_terminal/query_handler_registry.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,20 @@
-from functools import partial
-from typing import List, Optional
+from typing import Optional
 
 from bus_station.bus_stop.registration.bus_stop_registry import BusStopRegistry
-from bus_station.bus_stop.registration.supervisor.bus_stop_registration_supervisor import BusStopRegistrationSupervisor
-from bus_station.bus_stop.resolvers.bus_stop_resolver import BusStopResolver
 from bus_station.passengers.passenger_registry import passenger_bus_stop_registry
-from bus_station.passengers.passenger_resolvers import resolve_passenger_class_from_bus_stop
 from bus_station.query_terminal.handler_not_found_for_query import HandlerNotFoundForQuery
 from bus_station.query_terminal.query_handler import QueryHandler
 
 
 class QueryHandlerRegistry(BusStopRegistry[QueryHandler]):
-    def __init__(
-        self,
-        bus_stop_resolver: BusStopResolver,
-        registration_supervisors: Optional[List[BusStopRegistrationSupervisor]] = None,
-    ):
-        bus_stop_passenger_resolver = partial(
-            resolve_passenger_class_from_bus_stop,
-            bus_stop_handle_function_name="handle",
-            passenger_type_name="query",
-        )
-        super().__init__(bus_stop_resolver, bus_stop_passenger_resolver, registration_supervisors)
-
     def get_handler_from_query(self, query_name: str) -> Optional[QueryHandler]:
-        query_handler_ids = passenger_bus_stop_registry.get_bus_stops_for_passenger(query_name)
-        if len(query_handler_ids) == 0:
+        query_handler_names = passenger_bus_stop_registry.get_bus_stops_for_passenger(query_name)
+        if len(query_handler_names) == 0:
             return None
 
-        query_handler_id = next(iter(query_handler_ids))
-        resolved_query_handler = self._bus_stop_resolver.resolve(query_handler_id)
+        query_handler_name = next(iter(query_handler_names))
+        query_handler = self.get_bus_stop_by_name(query_handler_name)
 
-        if not isinstance(resolved_query_handler, QueryHandler):
+        if not isinstance(query_handler, QueryHandler):
             raise HandlerNotFoundForQuery(query_name)
-        return resolved_query_handler
+        return query_handler
```

### Comparing `bus_station-6.1.3/src/bus_station/query_terminal/rpyc_query_server.py` & `bus_station-7.0.0/src/bus_station/query_terminal/rpyc_query_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/shared_terminal/broker_connection/connection_parameters/rabbitmq_connection_parameters.py` & `bus_station-7.0.0/src/bus_station/shared_terminal/broker_connection/connection_parameters/rabbitmq_connection_parameters.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/shared_terminal/bus.py` & `bus_station-7.0.0/src/bus_station/shared_terminal/bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/shared_terminal/engine/runner/process_engine_runner.py` & `bus_station-7.0.0/src/bus_station/shared_terminal/engine/runner/process_engine_runner.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/shared_terminal/factories/memory_queue_factory.py` & `bus_station-7.0.0/src/bus_station/shared_terminal/factories/memory_queue_factory.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/shared_terminal/json_rpc_server.py` & `bus_station-7.0.0/src/bus_station/shared_terminal/json_rpc_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/shared_terminal/kafka_topic_creator.py` & `bus_station-7.0.0/src/bus_station/shared_terminal/kafka_topic_creator.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/shared_terminal/rpyc_server.py` & `bus_station-7.0.0/src/bus_station/shared_terminal/rpyc_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/tracking_terminal/models/passenger_model_tracking_map.py` & `bus_station-7.0.0/src/bus_station/tracking_terminal/models/passenger_model_tracking_map.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/tracking_terminal/models/passenger_tracking_json_serializer.py` & `bus_station-7.0.0/src/bus_station/tracking_terminal/models/passenger_tracking_json_serializer.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/tracking_terminal/trackers/kafka_passenger_tracker.py` & `bus_station-7.0.0/src/bus_station/tracking_terminal/trackers/kafka_passenger_tracker.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/src/bus_station/tracking_terminal/trackers/passenger_tracker.py` & `bus_station-7.0.0/src/bus_station/tracking_terminal/trackers/passenger_tracker.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.3/PKG-INFO` & `bus_station-7.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: bus-station
-Version: 6.1.3
+Version: 7.0.0
 Summary: A python bus station
 Author: DeejayRevok
 Author-email: seryi_one@hotmail.com
 Requires-Python: >=3.10.0,<3.11.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: confluent-kafka (>=2.1.1,<3.0.0)
 Requires-Dist: freezegun (>=1.2.2,<2.0.0)
-Requires-Dist: jsonrpcclient (>=4.0.2,<5.0.0)
-Requires-Dist: jsonrpcserver (>=5.0.6,<6.0.0)
+Requires-Dist: jsonrpcclient (>=4.0.3,<5.0.0)
+Requires-Dist: jsonrpcserver (>=5.0.9,<6.0.0)
 Requires-Dist: kombu (==5.2.2)
-Requires-Dist: pypendency (>=0,<1)
 Requires-Dist: redis (==4.4.4)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
-Requires-Dist: rpyc (==5.0.1)
-Requires-Dist: yandil (>=0,<1)
+Requires-Dist: rpyc (>=5.3.1,<6.0.0)
 Description-Content-Type: text/markdown
 
 # Bus station
 Python bus pattern implementation
```

