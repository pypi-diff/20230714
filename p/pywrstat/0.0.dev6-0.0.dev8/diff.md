# Comparing `tmp/pywrstat-0.0.dev6.tar.gz` & `tmp/pywrstat-0.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pywrstat-0.0.dev6.tar", last modified: Mon Jul 25 19:29:10 2022, max compression
+gzip compressed data, was "pywrstat-0.0.dev8.tar", last modified: Fri Jul 14 17:36:42 2023, max compression
```

## Comparing `pywrstat-0.0.dev6.tar` & `pywrstat-0.0.dev8.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 19:29:10.000000 pywrstat-0.0.dev6/
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-07-25 19:29:10.000000 pywrstat-0.0.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-07-25 19:28:54.000000 pywrstat-0.0.dev6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 19:29:10.000000 pywrstat-0.0.dev6/pywrstat/
--rw-r--r--   0 runner    (1001) docker     (121)      808 2022-07-25 19:28:54.000000 pywrstat-0.0.dev6/pywrstat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24261 2022-07-25 19:28:54.000000 pywrstat-0.0.dev6/pywrstat/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1987 2022-07-25 19:28:54.000000 pywrstat-0.0.dev6/pywrstat/dto.py
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-07-25 19:28:54.000000 pywrstat-0.0.dev6/pywrstat/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-07-25 19:28:54.000000 pywrstat-0.0.dev6/pywrstat/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-07-25 19:28:54.000000 pywrstat-0.0.dev6/pywrstat/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 19:29:10.000000 pywrstat-0.0.dev6/pywrstat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-07-25 19:29:10.000000 pywrstat-0.0.dev6/pywrstat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-07-25 19:29:10.000000 pywrstat-0.0.dev6/pywrstat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-25 19:29:10.000000 pywrstat-0.0.dev6/pywrstat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-07-25 19:29:10.000000 pywrstat-0.0.dev6/pywrstat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-07-25 19:29:10.000000 pywrstat-0.0.dev6/pywrstat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-25 19:29:10.000000 pywrstat-0.0.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1294 2022-07-25 19:28:54.000000 pywrstat-0.0.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:36:42.416357 pywrstat-0.0.dev8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-14 17:36:13.000000 pywrstat-0.0.dev8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-14 17:36:42.416357 pywrstat-0.0.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-14 17:36:13.000000 pywrstat-0.0.dev8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:36:42.412357 pywrstat-0.0.dev8/pywrstat/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-14 17:36:13.000000 pywrstat-0.0.dev8/pywrstat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-07-14 17:36:13.000000 pywrstat-0.0.dev8/pywrstat/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24669 2023-07-14 17:36:13.000000 pywrstat-0.0.dev8/pywrstat/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-14 17:36:13.000000 pywrstat-0.0.dev8/pywrstat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-14 17:36:13.000000 pywrstat-0.0.dev8/pywrstat/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-14 17:36:13.000000 pywrstat-0.0.dev8/pywrstat/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-14 17:36:13.000000 pywrstat-0.0.dev8/pywrstat/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-14 17:36:13.000000 pywrstat-0.0.dev8/pywrstat/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-14 17:36:13.000000 pywrstat-0.0.dev8/pywrstat/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:36:42.416357 pywrstat-0.0.dev8/pywrstat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-14 17:36:42.000000 pywrstat-0.0.dev8/pywrstat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-14 17:36:42.000000 pywrstat-0.0.dev8/pywrstat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:36:42.000000 pywrstat-0.0.dev8/pywrstat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-14 17:36:42.000000 pywrstat-0.0.dev8/pywrstat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 17:36:42.000000 pywrstat-0.0.dev8/pywrstat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:36:42.416357 pywrstat-0.0.dev8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-14 17:36:13.000000 pywrstat-0.0.dev8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pywrstat-0.0.dev6/PKG-INFO` & `pywrstat-0.0.dev8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: pywrstat
-Version: 0.0.dev6
+Version: 0.0.dev8
 Summary: Pwrstat (CyberPower UPS Linux command line) Python wrapper API
 Home-page: https://github.com/jean-edouard-boulanger/pywrstat
 Author: Jean-Edouard Boulanger
 Author-email: jean.edouard.boulanger@gmail.com
 License: MIT
-Description: # pywrstat
-        
-        Pwrstat (CyberPower UPS Linux command line) Python wrapper API. Pywrstat needs the `pwrstat` command line utility installed
-        on the same machine.
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Power (UPS)
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pywrstat
+
+Pwrstat (CyberPower UPS Linux command line) Python wrapper API. Pywrstat needs the `pwrstat` command line utility installed
+on the same machine.
+
+
```

### Comparing `pywrstat-0.0.dev6/pywrstat/__init__.py` & `pywrstat-0.0.dev8/pywrstat/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from pywrstat.client import Pywrstat
-from pywrstat.dto import (
+from pywrstat.errors import (
+    CommandFailed,
+    Error,
+    NotReady,
+    SetupFailed,
+    Timeout,
+    Unreachable,
+)
+from pywrstat.schema import (
     DaemonConfiguration,
-    Event,
+    Events,
     LowBatteryAction,
     PowerEvent,
     PowerFailureAction,
-    ReachabilityChanged,
+    ReachabilityChangedEvent,
     TestResult,
     TestStatus,
     UPSProperties,
     UPSStatus,
-    ValueChanged,
-)
-from pywrstat.errors import (
-    CommandFailed,
-    Error,
-    NotReady,
-    SetupFailed,
-    Timeout,
-    Unreachable,
+    ValueChangedEvent,
 )
 from pywrstat.version import __version__  # noqa
 
 __all__ = [
     "CommandFailed",
     "DaemonConfiguration",
     "Error",
-    "Event",
+    "Events",
     "LowBatteryAction",
     "NotReady",
     "PowerEvent",
     "PowerFailureAction",
     "Pywrstat",
-    "ReachabilityChanged",
+    "ReachabilityChangedEvent",
     "SetupFailed",
     "TestResult",
     "TestStatus",
     "Timeout",
     "UPSProperties",
     "UPSStatus",
     "Unreachable",
-    "ValueChanged",
+    "ValueChangedEvent",
 ]
```

### Comparing `pywrstat-0.0.dev6/pywrstat/client.py` & `pywrstat-0.0.dev8/pywrstat/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import dataclasses
+import json
 import re
 import time
 from collections import defaultdict
 from datetime import datetime, timedelta
 from pathlib import Path
 from typing import Dict, Generator, Optional, Union
 
 from dateutil.parser import parse as parse_time
 
-from pywrstat.dto import (
+from pywrstat.errors import CommandFailed, NotReady, SetupFailed, Timeout, Unreachable
+from pywrstat.reader import Reader, ReaderBase
+from pywrstat.schema import (
     DaemonConfiguration,
-    Event,
+    Events,
     LowBatteryAction,
     PowerEvent,
     PowerFailureAction,
-    ReachabilityChanged,
+    ReachabilityChangedEvent,
     TestResult,
     TestStatus,
     UPSProperties,
     UPSStatus,
-    ValueChanged,
+    ValueChangedEvent,
 )
-from pywrstat.errors import CommandFailed, NotReady, SetupFailed, Timeout, Unreachable
-from pywrstat.reader import Reader, ReaderBase
 
 _PywrstatSectionType = str
 _PywrstatPropertyType = str
 _PywrstatValueType = str
 _PywrstatParsedOutputType = Dict[
     _PywrstatSectionType, Dict[_PywrstatPropertyType, _PywrstatValueType]
 ]
@@ -76,22 +76,24 @@
             test_time=parse_time(match.group(2)),
         )
     return None
 
 
 def _parse_power_event(raw_power_event: str) -> Optional[PowerEvent]:
     match = re.search(
-        r"^([\w\s]+)\s+at\s+(\d{4}/\d{2}/\d{2}\s+\d{2}:\d{2}:\d{2})\s+for\s+(\d+) sec\.$",
+        r"^([\w\s]+)\s+at\s+(\d{4}/\d{2}/\d{2}\s+\d{2}:\d{2}:\d{2})\s+for\s+(\d+) (sec|min)\.$",
         raw_power_event,
     )
     if match:
+        unit = match.group(4)
+        multiplier = 1 if unit == "sec" else 60
         return PowerEvent(
             event_type=match.group(1),
             event_time=parse_time(match.group(2)),
-            duration=timedelta(seconds=int(match.group(3))),
+            duration=timedelta(seconds=(int(match.group(3)) * multiplier)),
         )
     return None
 
 
 def _is_ups_reachable(raw_ups_status: PropertyBag) -> bool:
     return raw_ups_status["State"] != "Lost Communication"
 
@@ -249,15 +251,15 @@
             line_interaction=data["Line Interaction"],
             test_result=_parse_test_result(data["Test Result"]),
             last_power_event=_parse_power_event(data["Last Power Event"]),
         )
 
     def monitor_ups_status(
         self, poll_every: Optional[timedelta] = None
-    ) -> Generator[Event, None, None]:
+    ) -> Generator[Events, None, None]:
         """Monitor the UPS status, sends events whenever the status changes.
 
         Possible events are:
 
           - ReachabilityChanged: when the UPS becomes unreachable / reachable again).
           - ValueChanged: when one / more UPS status property changes.
 
@@ -268,41 +270,50 @@
         poll_every = poll_every or timedelta(seconds=1)
         previous_state: Optional[UPSStatus] = None
         previously_reachable: Optional[bool] = None
         while True:
             try:
                 current_state = self.get_ups_status()
                 if previously_reachable is False:
-                    yield Event(
-                        event_metadata=ReachabilityChanged(reachable=True),
+                    yield Events(
+                        events=[ReachabilityChangedEvent(reachable=True)],
                         new_state=current_state,
                         previous_state=previous_state,
                     )
                 if previous_state:
-                    previous_state_serialized = dataclasses.asdict(previous_state)
-                    current_state_serialized = dataclasses.asdict(current_state)
+                    previous_state_serialized = json.loads(
+                        previous_state.model_dump_json()
+                    )
+                    current_state_serialized = json.loads(
+                        current_state.model_dump_json()
+                    )
+                    events = []
                     for field in sorted(previous_state_serialized.keys()):
                         previous_value = previous_state_serialized[field]
                         current_value = current_state_serialized[field]
                         if current_value != previous_value:
-                            yield Event(
-                                event_metadata=ValueChanged(
+                            events.append(
+                                ValueChangedEvent(
                                     field_name=field,
                                     new_value=current_value,
                                     previous_value=previous_value,
-                                ),
-                                new_state=current_state,
-                                previous_state=previous_state,
+                                )
                             )
+                    if events:
+                        yield Events(
+                            events=events,
+                            previous_state=previous_state,
+                            new_state=current_state,
+                        )
                 previous_state = current_state
                 previously_reachable = True
             except Unreachable:
                 if previously_reachable is True:
-                    yield Event(
-                        event_metadata=ReachabilityChanged(reachable=False),
+                    yield Events(
+                        events=[ReachabilityChangedEvent(reachable=False)],
                         new_state=None,
                         previous_state=previous_state,
                     )
                 previous_state = None
                 previously_reachable = False
             time.sleep(poll_every.total_seconds())
 
@@ -320,15 +331,15 @@
         """Get the UPS status limited to the "Properties" section.
         :return: The UPS status limited to the "Properties" section. The output is deserialized to a
                  `UPSProperties` object.
         :raises: Unreachable: If the UPS is not reachable.
         """
         data = self.get_raw_ups_properties(check_reachable=True)
         return UPSProperties(
-            model_name=data["Model Name"],
+            ups_model_name=data["Model Name"],
             firmware_number=data["Firmware Number"],
             rating_voltage_volts=float(data["Rating Voltage"].split()[0]),
             rating_power_watts=float(data["Rating Power"].split()[0]),
         )
 
     def test_ups(
         self,
@@ -388,36 +399,36 @@
     def hibernation_enabled(self) -> bool:
         """Check whether system hibernation (vs. system shutdown) is enabled.
         :return: `True` if hibernation is enabled, `False` otherwise.
         """
         return self.get_daemon_configuration().hibernate_enabled
 
     @hibernation_enabled.setter
-    def hibernation_enabled(self, enabled: bool):
+    def hibernation_enabled(self, enabled: bool) -> None:
         """Set up the hibernation (vs. system shutdown) enablement (as run by `pwrstat -hibernate [on/off]`).
         :param enabled: Specify whether to enable or disable hibernation (vs. system shutdown).
         """
         self._check_setup(self._reader.read(["-hibernate", _on_off(enabled)]))
 
     @property
     def alarm_enabled(self) -> bool:
         """Check whether the UPS alarm is enabled.
         :return: `True` if the UPS alarm is enabled, `False` otherwise.
         """
         return self.get_daemon_configuration().alarm_enabled
 
     @alarm_enabled.setter
-    def alarm_enabled(self, enabled: bool):
+    def alarm_enabled(self, enabled: bool) -> None:
         """Set the UPS alarm enablement (as run by `pwrstat -alarm [on/off]`).
         :param enabled: Specify whether to enable or disable the UPS alarm.
         :raises: SetupFailed: If alarm enablement could not be setup.
         """
         self._check_setup(self._reader.read(["-alarm", _on_off(enabled)]))
 
-    def mute(self):
+    def mute(self) -> None:
         """Setup temporally mute alarm when alarm is on enable state (as run by `pwrstat -mute`).
         :raises: Unreachable: If the UPS is not reachable.
         :raises: SetupFailed: If alarm enablement could not be muted.
         """
         self._check_setup(self._reader.read(["-mute"]))
 
     def _configure_action(
@@ -426,15 +437,15 @@
         delay: Optional[timedelta] = None,
         runtime: Optional[timedelta] = None,
         capacity: Optional[float] = None,
         active: Optional[bool] = None,
         cmd: Optional[Union[str, Path]] = None,
         duration: Optional[timedelta] = None,
         shutdown: Optional[bool] = None,
-    ):
+    ) -> None:
         args = [action]
         if delay is not None:
             args += ["-delay", str(int(delay.total_seconds()))]
         if runtime is not None:
             args += ["-runtime", str(int(runtime.total_seconds()))]
         if capacity is not None:
             args += ["-capacity", str(int(_check_percent(capacity) * 100.0))]
```

### Comparing `pywrstat-0.0.dev6/pywrstat.egg-info/PKG-INFO` & `pywrstat-0.0.dev8/pywrstat.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: pywrstat
-Version: 0.0.dev6
+Version: 0.0.dev8
 Summary: Pwrstat (CyberPower UPS Linux command line) Python wrapper API
 Home-page: https://github.com/jean-edouard-boulanger/pywrstat
 Author: Jean-Edouard Boulanger
 Author-email: jean.edouard.boulanger@gmail.com
 License: MIT
-Description: # pywrstat
-        
-        Pwrstat (CyberPower UPS Linux command line) Python wrapper API. Pywrstat needs the `pwrstat` command line utility installed
-        on the same machine.
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Power (UPS)
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pywrstat
+
+Pwrstat (CyberPower UPS Linux command line) Python wrapper API. Pywrstat needs the `pwrstat` command line utility installed
+on the same machine.
+
+
```

### Comparing `pywrstat-0.0.dev6/setup.py` & `pywrstat-0.0.dev8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,25 +17,29 @@
     long_description=README,
     long_description_content_type="text/markdown",
     author="Jean-Edouard Boulanger",
     url="https://github.com/jean-edouard-boulanger/pywrstat",
     author_email="jean.edouard.boulanger@gmail.com",
     license="MIT",
     packages=["pywrstat"],
-    python_requires=">=3.7",
+    python_requires=">=3.9",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: System Administrators",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: System :: Power (UPS)",
     ],
     install_requires=[
         "python-dateutil>=2.8.2,<3",
+        "pydantic>=2.0.2,<3",
+        "Flask>=2.3.2,<3",
+        "gunicorn>=20.1.0,<21",
+        "PyJWT>=2.7.0,<3",
+        "python-dotenv>=1.0.0,<2",
     ],
 )
```

