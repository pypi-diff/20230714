# Comparing `tmp/phanos-0.0.7.tar.gz` & `tmp/phanos-0.0.8.tar.gz`

## Comparing `phanos-0.0.7.tar` & `phanos-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 phanos-0.0.7/CHANGELOG.md
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.0.7/Pipfile
--rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.0.7/Pipfile.lock
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 phanos-0.0.7/requirements.txt
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/Activate.ps1
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/activate
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/activate.csh
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/activate.fish
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/pip
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/pip3
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/pip3.10
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/pip3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/python -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/python3 -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.7/deactivate/bin/python3.11 -> /usr/bin/python3.11
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 phanos-0.0.7/src/phanos/__init__.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 phanos-0.0.7/src/phanos/log.py
--rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 phanos-0.0.7/src/phanos/metrics.py
--rw-r--r--   0        0        0    15975 2020-02-02 00:00:00.000000 phanos-0.0.7/src/phanos/publisher.py
--rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 phanos-0.0.7/src/phanos/tree.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 phanos-0.0.7/test/__init__.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 phanos-0.0.7/test/dummy_api.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 phanos-0.0.7/test/requirements.txt
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 phanos-0.0.7/test/run_tests.py
--rw-r--r--   0        0        0    20465 2020-02-02 00:00:00.000000 phanos-0.0.7/test/test_metric.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 phanos-0.0.7/test/testing_data.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.0.7/.gitignore
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.0.7/LICENSE
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 phanos-0.0.7/README.md
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 phanos-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 phanos-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 phanos-0.0.8/CHANGELOG.md
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.0.8/Pipfile
+-rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.0.8/Pipfile.lock
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 phanos-0.0.8/requirements.txt
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/Activate.ps1
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/activate
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/activate.csh
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/activate.fish
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/pip
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/pip3
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/pip3.10
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/pip3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/python -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/python3 -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.0.8/deactivate/bin/python3.11 -> /usr/bin/python3.11
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 phanos-0.0.8/src/phanos/__init__.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 phanos-0.0.8/src/phanos/log.py
+-rw-r--r--   0        0        0    17210 2020-02-02 00:00:00.000000 phanos-0.0.8/src/phanos/metrics.py
+-rw-r--r--   0        0        0    16975 2020-02-02 00:00:00.000000 phanos-0.0.8/src/phanos/publisher.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 phanos-0.0.8/src/phanos/tree.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 phanos-0.0.8/test/__init__.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 phanos-0.0.8/test/dummy_api.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 phanos-0.0.8/test/requirements.txt
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 phanos-0.0.8/test/run_tests.py
+-rw-r--r--   0        0        0    20704 2020-02-02 00:00:00.000000 phanos-0.0.8/test/test_metric.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 phanos-0.0.8/test/testing_data.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.0.8/LICENSE
+-rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 phanos-0.0.8/README.md
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 phanos-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 phanos-0.0.8/PKG-INFO
```

### Comparing `phanos-0.0.7/Pipfile.lock` & `phanos-0.0.8/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `phanos-0.0.7/deactivate/bin/Activate.ps1` & `phanos-0.0.8/deactivate/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `phanos-0.0.7/deactivate/bin/activate` & `phanos-0.0.8/deactivate/bin/activate`

 * *Files identical despite different names*

### Comparing `phanos-0.0.7/deactivate/bin/activate.csh` & `phanos-0.0.8/deactivate/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `phanos-0.0.7/deactivate/bin/activate.fish` & `phanos-0.0.8/deactivate/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `phanos-0.0.7/src/phanos/log.py` & `phanos-0.0.8/src/phanos/log.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.7/src/phanos/metrics.py` & `phanos-0.0.8/src/phanos/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,21 +45,32 @@
         self._values = []
         self.method = []
         self.job = ""
         self.label_names = list(set(labels)) if labels else []
         self._label_values = []
         self.operations = {}
         self.default_operation = ""
-        super().__init__(logged_name="phanos", logger=logger or logging.getLogger(__name__))
+        super().__init__(
+            logged_name="phanos", logger=logger or logging.getLogger(__name__)
+        )
 
     def to_records(self) -> typing.List[Record]:
         """Convert measured values into Type Record
 
-        :returns: List of records"""
+        :returns: List of records
+        :raises RuntimeError: if one of records would be incomplete
+        """
         records = []
+        if not (len(self.method) == len(self._values) == len(self._label_values)):
+            self.error(
+                f"{self.to_records.__qualname__}: one of records missing method || value || label_values"
+            )
+            raise RuntimeError(
+                f"{len(self.method)}, {len(self._values)}, {len(self._label_values)}"
+            )
         for i in range(len(self._values)):
             label_value = (
                 self._label_values[i] if self._label_values is not None else {}
             )
             record: Record = {
                 "item": self.method[i].split(":")[0],
                 "metric": self.metric,
@@ -118,37 +129,47 @@
         except RuntimeError:
             pass
 
         if label_values is None:
             label_values = {}
         try:
             labels_ok = self._check_labels(list(label_values.keys()))
-            if labels_ok and label_values is not None:
+            if labels_ok:
                 self._label_values.append(label_values)
             else:
+                self.error(
+                    f"{self.store_operation.__qualname__}: expected labels: {self.label_names}, "
+                    f"labels given: {label_values.keys()}"
+                )
                 raise ValueError("Unknown or missing label")
             if operation is None:
                 operation = self.default_operation
             self.method.append(method)
-            self.debug("metric %s stored operation %s, value %s", self.name, operation, value)
+            self.debug(
+                "metric %s stored operation %s, value %s", self.name, operation, value
+            )
             self.operations[operation](value, args, kwargs)
         except KeyError as exc:
+            self.error(
+                f"{self.store_operation.__qualname__}: operation {operation} unknown."
+                f"Known operations: {self.operations.keys()}"
+            )
             raise ValueError("Unknown operation") from exc
 
     def cleanup(self) -> None:
-        """Cleanup after metrics was sent"""
+        """Cleanup after all records was sent"""
         if self._values is not None:
             self._values.clear()
         if self._label_values is not None:
             self._label_values.clear()
         if self.method is not None:
             self.method.clear()
         if self.item is not None:
             self.item.clear()
-        self.debug("metric %s cleared", self.name)
+        self.debug("%s: metric %s cleared", self.cleanup.__qualname__, self.name)
 
 
 class Histogram(MetricWrapper):
     """class representing histogram metric of Prometheus"""
 
     metric: str
 
@@ -172,18 +193,20 @@
         self.default_operation = "observe"
         self.operations = {"observe": self._observe}
 
     def _observe(self, value: float, *args, **kwargs) -> None:
         """Method representing observe action of Histogram
 
         :param value: measured value
+        :raises ValueError: if value is not float
         """
         _ = args
         _ = kwargs
         if not isinstance(value, float):
+            self.error(f"{self._observe.__qualname__}: accepts only float values")
             raise TypeError("Value must be float")
         self._values.append(("observe", value))
 
 
 class Summary(MetricWrapper):
     """class representing summary metric of Prometheus"""
 
@@ -209,18 +232,20 @@
         self.default_operation = "observe"
         self.operations = {"observe": self._observe}
 
     def _observe(self, value: float, *args, **kwargs) -> None:
         """Method representing observe action of Summary
 
         :param value: measured value
+        :raises ValueError: if value is not float
         """
         _ = args
         _ = kwargs
         if not isinstance(value, float):
+            self.error(f"{self._observe.__qualname__}: accepts only float values")
             raise TypeError("Value must be float")
         self._values.append(("observe", value))
 
 
 class Counter(MetricWrapper):
     """class representing counter metric of Prometheus"""
 
@@ -246,19 +271,21 @@
         self.default_operation = "inc"
         self.operations = {"inc": self._inc}
 
     def _inc(self, value: float, *args, **kwargs) -> None:
         """Method representing inc action of counter
 
         :param value: measured value
+        :raises ValueError: if value is not float >= 0
         """
         _ = args
         _ = kwargs
         if not isinstance(value, float) or value < 0:
-            raise TypeError("Value must be float > 0")
+            self.error(f"{self._inc.__qualname__}: accepts only float values >= 0")
+            raise TypeError("Value must be float >= 0")
         self._values.append(("inc", value))
 
 
 class Info(MetricWrapper):
     """class representing info metric of Prometheus"""
 
     metric: str
@@ -287,19 +314,20 @@
 
     def _info(
         self, value: typing.Dict[typing.Any, typing.Any], *args, **kwargs
     ) -> None:
         """Method representing info action of info
 
         :param value: measured value
+        :raises ValueError: if value is not dictionary
         """
         _ = args
         _ = kwargs
         if not isinstance(value, dict):
-            logging.error("Phanos - Metric info value must be dict")
+            self.error(f"{self._info.__qualname__}: accepts only dictionary values")
             raise ValueError("Value must be dictionary")
         self._values.append(("info", value))
 
 
 class Gauge(MetricWrapper):
     """class representing gauge metric of Prometheus"""
 
@@ -329,40 +357,46 @@
             "set": self._set,
         }
 
     def _inc(self, value: float, *args, **kwargs) -> None:
         """Method representing inc action of gauge
 
         :param value: measured value
+        :raises ValueError: if value is not float >= 0
         """
         _ = args
         _ = kwargs
         if not isinstance(value, float) or value < 0:
+            self.error(f"{self._inc.__qualname__}: accepts only float values >= 0")
             raise TypeError("Value must be float >= 0")
         self._values.append(("inc", value))
 
     def _dec(self, value: float, *args, **kwargs) -> None:
         """Method representing dec action of gauge
 
         :param value: measured value
+        :raises ValueError: if value is not float >= 0
         """
         _ = args
         _ = kwargs
         if not isinstance(value, float) or value < 0:
+            self.error(f"{self._dec.__qualname__}: accepts only float values >= 0")
             raise TypeError("Value must be float >= 0")
         self._values.append(("dec", value))
 
     def _set(self, value: float, *args, **kwargs) -> None:
         """Method representing set action of gauge
 
         :param value: measured value
+        :raises ValueError: if value is not float
         """
         _ = args
         _ = kwargs
         if not isinstance(value, float):
+            self.error(f"{self._set.__qualname__}: accepts only float values")
             raise TypeError("Value must be float")
         self._values.append(("set", value))
 
 
 class Enum(MetricWrapper):
     """class representing enum metric of Prometheus"""
 
@@ -399,17 +433,19 @@
 
         :param value: measured value
         :raises ValueError: if value not in states at initialization
         """
         _ = args
         _ = kwargs
         if value not in self.states:
-            raise TypeError(
-                f"State  {value} not allowed for this Enum. Allowed values: {self.states}"
+            self.warning(
+                f"{self._state.__qualname__}: state  {value!r} not allowed for Enum {self.name!r}. "
+                f"Allowed values: {self.states!r}"
             )
+            raise ValueError("Invalid state for Enum metric")
         self._values.append(("state", value))
 
 
 class TimeProfiler(Histogram):
     """class for measuring multiple time records in one endpoint.
      Used for measuring time consuming operations
 
@@ -422,41 +458,50 @@
         self,
         name: str,
         labels: typing.Optional[typing.List[str]] = None,
         logger: typing.Optional[logging.Logger] = None,
     ) -> None:
         """
         :param labels: label_names of metric viz. Type Record
+        :raises RuntimeError: if start timestamps < number of stop measurement operation
         """
         super().__init__(name, "mS", labels, logger)
         self.operations = {"stop": self._stop}
         self.default_operation = "stop"
         self._start_ts = []
+        self.debug("TimeProfiler metric initialized")
 
     # ############################### measurement operations -> checking labels, not sending records
     def _stop(self, *args, **kwargs) -> None:
         """Records time difference between last start_ts and now"""
         _ = args
         _ = kwargs
-        method_time = dt.now() - self._start_ts.pop(-1)
-
-        self._observe(
-            method_time.total_seconds() * 1000.0,
-        )
+        try:
+            method_time = dt.now() - self._start_ts.pop(-1)
+            self._observe(
+                method_time.total_seconds() * 1000.0,
+            )
+        except IndexError:
+            self.error(
+                f"{self._stop.__qualname__}: Cannot record operation. No start ts exists."
+            )
+            raise RuntimeError(
+                "Number of start timestamps < number of stop measurement operations"
+            )
 
     # ############################### helper operations -> not checking labels, not checking records
     def start(self, *args, **kwargs) -> None:
         """Starts time measurement - stores dt.now()"""
         _ = args
         _ = kwargs
         self._start_ts.append(dt.now())
 
     def cleanup(self) -> None:
         """Method responsible for cleanup after publishing records"""
-        self._start_ts = []
+        self._start_ts.clear()
         super().cleanup()
 
 
 class ResponseSize(Histogram):
     """class for measuring response size from API
 
     measured in bytes
@@ -470,13 +515,14 @@
     ) -> None:
         """
         :param labels: label_names of metric viz. Type Record
         """
         super().__init__(name, "B", labels, logger)
         self.operations = {"rec": self._rec}
         self.default_operation = "rec"
+        self.debug("ResponseSize metric initialized")
 
     def _rec(self, value: str, *args, **kwargs) -> None:
         """records size of response"""
         _ = args
         _ = kwargs
         self._observe(float(sys.getsizeof(value)))
```

### Comparing `phanos-0.0.7/src/phanos/publisher.py` & `phanos-0.0.8/src/phanos/publisher.py`

 * *Files 8% similar despite different names*

```diff
@@ -306,21 +306,27 @@
         self.add_metric(self.time_profile)
         self.debug("Phanos - time profiler created")
 
     def create_response_size_profiler(self) -> None:
         """create response size profiling metric"""
         self.resp_size_profile = ResponseSize(RESPONSE_SIZE, logger=self.logger)
         self.add_metric(self.resp_size_profile)
-        self.debug("response size profiler created")
+        self.debug("Phanos - response size profiler created")
 
     def delete_metric(self, item: str) -> None:
         """deletes one metric instance
         :param item: name of the metric instance
+        :raises KeyError: if metric does not exist
         """
-        _ = self._metrics.pop(item, None)
+        try:
+            _ = self._metrics.pop(item)
+        except KeyError:
+            self.error(f"{self.delete_metric.__qualname__}: metric {item} do not exist")
+            raise KeyError(f"metric {item} do not exist")
+
         if item == "time_profiler":
             self.time_profile = None
         if item == "response_size":
             self.resp_size_profile = None
         self.debug(f"metric {item} deleted")
 
     def delete_metrics(
@@ -347,31 +353,46 @@
         self._root.clear_tree()
 
     def add_metric(self, metric: MetricWrapper) -> None:
         """adds new metric to profiling
 
         :param metric: metric instance
         """
+        if self._metrics.get(metric.name, None):
+            self.warning(
+                f"Metric {metric.name} already exist. Overwriting with new metric"
+            )
         self._metrics[metric.name] = metric
-        self.debug(f"metric {metric.name} added")
+        self.debug(f"Metric {metric.name} added to phanos profiler")
 
     def add_handler(self, handler: BaseHandler) -> None:
         """Add handler to profiler
 
         :param handler: handler instance
         """
+        if self._handlers.get(handler.handler_name, None):
+            self.warning(
+                f"Handler {handler.handler_name} already exist. Overwriting with new handler"
+            )
         self._handlers[handler.handler_name] = handler
-        self.debug(f"handler {handler.handler_name} added to phanos profiler")
+        self.debug(f"Handler {handler.handler_name} added to phanos profiler")
 
     def delete_handler(self, handler_name: str) -> None:
         """Delete handler from profiler
 
         :param handler_name: name of handler:
+        :raises KeyError: if handler do not exist
         """
-        _ = self._handlers.pop(handler_name, None)
+        try:
+            _ = self._handlers.pop(handler_name)
+        except KeyError:
+            self.error(
+                f"{self.delete_handler.__qualname__}: handler {handler_name} do not exist"
+            )
+            raise KeyError(f"handler {handler_name} do not exist")
         self.debug(f"handler {handler_name} deleted")
 
     def delete_handlers(self) -> None:
         """delete all handlers"""
         self._handlers.clear()
         self.debug(f"all handlers deleted")
 
@@ -415,53 +436,52 @@
         return inner
 
     def _before_root_func(self, function: typing.Callable, *args, **kwargs) -> None:
         """method executing before root function
 
         :param function: root function
         """
-        # custom
+        # users custom metrics operation recording
         if callable(self.before_root_func):
             self.before_root_func(function=function, *args, **kwargs)
-        # here mine if needed
+        # place for phanos metrics if needed
 
     def _after_root_func(self, fn_result: typing.Any, *args, **kwargs) -> None:
         """method executing after the root function
 
 
         :param fn_result: result of function
         """
-        # mine
+        # phanos metrics
         if self.resp_size_profile:
             self.resp_size_profile.store_operation(
                 operation="rec",
                 method=self.current_node.context,
                 value=fn_result,
                 label_values={},
             )
-        # user custom function
+        # users custom metrics operation recording
         if callable(self.after_root_func):
             self.after_root_func(fn_result=fn_result, *args, **kwargs)
 
     def _before_func(self, func, *args, **kwargs) -> None:
-        # user custom
+        # users custom metrics operation recording
         if callable(self.before_func):
             self.before_func(function=func, *args, **kwargs)
-        # mine
+        # phanos metrics
         if self.time_profile:
             self.time_profile.start()
 
     def _after_func(self, fn_result: typing.Any, *args, **kwargs) -> None:
-        # mine
+        # phanos metrics
         if self.time_profile:
             self.time_profile.store_operation(
                 operation="stop", method=self.current_node.context, label_values={}
             )
-            self.debug(f"{self.time_profile.name} recorded operation ")
-        # custom
+        # users custom metrics operation recording
         if callable(self.after_func):
             self.after_func(fn_result=fn_result, *args, **kwargs)
 
     def handle_records_clear(self) -> None:
         """Pass records to each registered Handler and clear stored records"""
         # send records and log em
         for metric in self._metrics.values():
```

### Comparing `phanos-0.0.7/src/phanos/tree.py` & `phanos-0.0.8/src/phanos/tree.py`

 * *Files 22% similar despite different names*

```diff
@@ -44,66 +44,49 @@
         """
         child.parent = self
         if self.method is None:  # equivalent of 'self.context != ""' -> i am root
             child.context = (
                 self.get_method_class(child.method) + ":" + child.context
             )  # child.method cannot be None
         else:
-            between = self._get_methods_between()
-            if between != "":
-                child.context = self.context + "." + between + "." + child.context
-            else:
-                child.context = self.context + "." + child.context
+            child.context = self.context + "." + child.context
         self.children.append(child)
-        self.debug(f"node {self.context} added child: {child.context}")
+        self.debug(
+            f"{self.add_child.__qualname__}: node {self.context!r} added child: {child.context!r}"
+        )
         return child
 
-    def _get_methods_between(self) -> str:
-        methods_between = []
-        split_context = self.context.split(".")
-        if len(split_context) == 1:
-            starting_method = self.context.split(":")[-1]
-        else:
-            starting_method = split_context[-1]
-        between = ""
-        if inspect.stack():
-            for item in inspect.stack():
-                if item.function == starting_method:
-                    break
-                if item.function not in [
-                    "<module>",
-                    "inner",
-                    "add_child",
-                    "_get_methods_between",
-                ]:
-                    methods_between.append(item.function)
-            methods_between.reverse()
-            between = ".".join(f"{method}" for method in methods_between)
-
-        return between
-
     def delete_child(self) -> None:
         """Delete first child of node"""
-        child = self.children.pop(0)
-        child.parent = None
-        self.debug(f"node {self.context} deleted child: {child.context}")
+        try:
+            child = self.children.pop(0)
+            child.parent = None
+            self.debug(
+                f"{self.delete_child.__qualname__}: node {self.context!r} deleted child: {child.context!r}"
+            )
+        except IndexError:
+            self.debug(
+                f"{self.delete_child.__qualname__}: node {self.context!r} do not have any children"
+            )
 
     def clear_tree(self) -> None:
         """Clears tree of all nodes from self"""
         for child in self.children:
             child.clear_tree()
         self._clear_children()
 
     def _clear_children(self):
         self.parent = None
         children = []
         for child in self.children:
             children.append(child.context)
         self.children.clear()
-        self.debug(f"node {self.context} deleted children: {children}")
+        self.debug(
+            f"{self._clear_children.__qualname__}: node {self.context!r} deleted children: {children}"
+        )
 
     @staticmethod
     def get_method_class(meth: typing.Callable) -> str:
         """
         Gets class/module name where specified method/function was defined.
 
         Cannot do: partial, lambda !!!!!
```

### Comparing `phanos-0.0.7/test/dummy_api.py` & `phanos-0.0.8/test/dummy_api.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.7/test/run_tests.py` & `phanos-0.0.8/test/run_tests.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.7/test/test_metric.py` & `phanos-0.0.8/test/test_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,29 +198,30 @@
             self.assertRaises(
                 TypeError,
                 hist_no_lbl.store_operation,
                 "test:method",
                 "observe",
                 "asd",
             )
+            hist_no_lbl.cleanup()
             # valid operation
             hist_no_lbl.store_operation("test:method", "observe", 2.0),
             self.assertEqual(hist_no_lbl.to_records(), testing_data.hist_no_lbl)
 
             hist_w_lbl = Histogram("hist_w_lbl", "V", labels=["test"])
 
             # missing label
             self.assertRaises(
                 ValueError,
                 hist_w_lbl.store_operation,
                 "test:method",
                 "observe",
                 2.0,
             )
-
+            hist_w_lbl.cleanup()
             # default operation
             hist_w_lbl.store_operation(
                 method="test:method", value=2.0, label_values={"test": "test"}
             )
             self.assertEqual(hist_w_lbl.to_records(), testing_data.hist_w_lbl)
 
     def test_summary(self):
@@ -250,14 +251,15 @@
             self.assertRaises(
                 TypeError,
                 sum_no_lbl.store_operation,
                 "test:method",
                 "observe",
                 "asd",
             )
+            sum_no_lbl.cleanup()
             # valid operation
             sum_no_lbl.store_operation("test:method", "observe", 2.0),
             self.assertEqual(sum_no_lbl.to_records(), testing_data.sum_no_lbl)
 
     def test_counter(self):
         with app.test_request_context():
             cnt_no_lbl = Counter(
@@ -293,14 +295,15 @@
             self.assertRaises(
                 ValueError,
                 cnt_no_lbl.store_operation,
                 "test:method",
                 "nonexistent",
                 2.0,
             )
+            cnt_no_lbl.cleanup()
 
             # valid operation
             cnt_no_lbl.store_operation("test:method", "inc", 2.0),
             self.assertEqual(cnt_no_lbl.to_records(), testing_data.cnt_no_lbl)
 
     def test_info(self):
         with app.test_request_context():
@@ -319,15 +322,15 @@
             self.assertRaises(
                 ValueError,
                 inf_no_lbl.store_operation,
                 "test:method",
                 "nonexistent",
                 2.0,
             )
-
+            inf_no_lbl.cleanup()
             # valid operation
             inf_no_lbl.store_operation("test:method", "info", {"value": "asd"}),
             self.assertEqual(inf_no_lbl.to_records(), testing_data.inf_no_lbl)
 
     def test_gauge(self):
         with app.test_request_context():
             gauge_no_lbl = Gauge(
@@ -379,46 +382,46 @@
             self.assertRaises(
                 ValueError,
                 gauge_no_lbl.store_operation,
                 "test:method",
                 "nonexistent",
                 2.0,
             )
-
+            gauge_no_lbl.cleanup()
             # valid operation
             gauge_no_lbl.store_operation("test:method", "inc", 2.0),
             gauge_no_lbl.store_operation("test:method", "dec", 2.0),
             gauge_no_lbl.store_operation("test:method", "set", 2.0),
             self.assertEqual(gauge_no_lbl.to_records(), testing_data.gauge_no_lbl)
 
     def test_enum(self):
         with app.test_request_context():
             enum_no_lbl = Enum(
                 "enum_no_lbl",
                 ["true", "false"],
             )
             # invalid value
             self.assertRaises(
-                TypeError,
+                ValueError,
                 enum_no_lbl.store_operation,
                 "test:method",
                 "state",
                 "maybe",
             )
             # invalid operation
             self.assertRaises(
                 ValueError,
                 enum_no_lbl.store_operation,
                 "test:method",
                 "nonexistent",
                 "true",
             )
-
+            enum_no_lbl.cleanup()
             # valid operation
-            enum_no_lbl.store_operation("test", "state", "true")
+            enum_no_lbl.store_operation("test:method", "state", "true")
             self.assertEqual(enum_no_lbl.to_records(), testing_data.enum_no_lbl)
 
     def test_builtin_profilers(self):
         time_profiler = TimeProfiler("test_time_prof")
 
         time_profiler.start()
         time_profiler.start()
```

### Comparing `phanos-0.0.7/test/testing_data.py` & `phanos-0.0.8/test/testing_data.py`

 * *Files identical despite different names*

### Comparing `phanos-0.0.7/.gitignore` & `phanos-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `phanos-0.0.7/LICENSE` & `phanos-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `phanos-0.0.7/README.md` & `phanos-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,18 +25,21 @@
 2. Instantiate handlers you need for measured records at app construction.
    ```python      
    from phanos import phanos_profiler
    from phanos.publisher import LoggerHandler, ImpProfHandler
    # some code
    class SomeApp(Flask):
       """some code""" 
+   phanos_profiler.config(logger, should_time_profile, should_resp_size_profile, should_handle_records)
    log_handler = LoggerHandler('logger_name', logger_instance, logging_level)
    phanos_profiler.addHandler(log_handler)    
       # some code
    ```
+In `config` method you can select if you want to turn off  time profiling, response size profiling
+ or records handling. Default is turned on.
 After root method is executed all measured records are handled by all handlers added to
 `phanos_profiler`
 
 ## Handlers
 
 Each handler have handler_name parameter. This string can be used to delete handlers later
 with `phanos_profiler.deleteHandler(handler_name)`.
```

### Comparing `phanos-0.0.7/pyproject.toml` & `phanos-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "phanos"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Miroslav Bulička", email="bulickamiroslav@gmail.com" },
 ]
 description = "Python client to gather data for Prometheus logging in server with multiple instances and workers."
 readme = "README.md"
 requires-python = ">=3.10.6"
 classifiers = [
```

### Comparing `phanos-0.0.7/PKG-INFO` & `phanos-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phanos
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python client to gather data for Prometheus logging in server with multiple instances and workers.
 Project-URL: Homepage, https://github.com/kajotgames/phanos
 Project-URL: Bug Tracker, https://github.com/kajotgames/phanos/issues
 Author-email: Miroslav Bulička <bulickamiroslav@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -44,18 +44,21 @@
 2. Instantiate handlers you need for measured records at app construction.
    ```python      
    from phanos import phanos_profiler
    from phanos.publisher import LoggerHandler, ImpProfHandler
    # some code
    class SomeApp(Flask):
       """some code""" 
+   phanos_profiler.config(logger, should_time_profile, should_resp_size_profile, should_handle_records)
    log_handler = LoggerHandler('logger_name', logger_instance, logging_level)
    phanos_profiler.addHandler(log_handler)    
       # some code
    ```
+In `config` method you can select if you want to turn off  time profiling, response size profiling
+ or records handling. Default is turned on.
 After root method is executed all measured records are handled by all handlers added to
 `phanos_profiler`
 
 ## Handlers
 
 Each handler have handler_name parameter. This string can be used to delete handlers later
 with `phanos_profiler.deleteHandler(handler_name)`.
```

