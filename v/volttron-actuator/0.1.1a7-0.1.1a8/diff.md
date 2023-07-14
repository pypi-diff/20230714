# Comparing `tmp/volttron_actuator-0.1.1a7.tar.gz` & `tmp/volttron_actuator-0.1.1a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_actuator-0.1.1a7.tar", max compression
+gzip compressed data, was "volttron_actuator-0.1.1a8.tar", max compression
```

## Comparing `volttron_actuator-0.1.1a7.tar` & `volttron_actuator-0.1.1a8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11927 2023-07-10 16:39:51.230102 volttron_actuator-0.1.1a7/LICENSE
--rw-r--r--   0        0        0     1830 2023-07-10 16:39:51.230102 volttron_actuator-0.1.1a7/README.md
--rw-r--r--   0        0        0     1911 2023-07-10 16:42:51.533458 volttron_actuator-0.1.1a7/pyproject.toml
--rw-r--r--   0        0        0     1570 2023-07-10 16:39:51.230102 volttron_actuator-0.1.1a7/src/actuator/__init__.py
--rw-r--r--   0        0        0    52552 2023-07-10 16:39:51.234102 volttron_actuator-0.1.1a7/src/actuator/agent.py
--rw-r--r--   0        0        0    16122 2023-07-10 16:39:51.234102 volttron_actuator-0.1.1a7/src/actuator/scheduler.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 volttron_actuator-0.1.1a7/setup.py
--rw-r--r--   0        0        0     2929 1970-01-01 00:00:00.000000 volttron_actuator-0.1.1a7/PKG-INFO
+-rw-r--r--   0        0        0    11927 2023-07-14 01:06:54.517948 volttron_actuator-0.1.1a8/LICENSE
+-rw-r--r--   0        0        0     1830 2023-07-14 01:06:54.517948 volttron_actuator-0.1.1a8/README.md
+-rw-r--r--   0        0        0     1911 2023-07-14 01:08:35.551147 volttron_actuator-0.1.1a8/pyproject.toml
+-rw-r--r--   0        0        0     1570 2023-07-14 01:06:54.517948 volttron_actuator-0.1.1a8/src/actuator/__init__.py
+-rw-r--r--   0        0        0    54904 2023-07-14 01:06:54.517948 volttron_actuator-0.1.1a8/src/actuator/agent.py
+-rw-r--r--   0        0        0    16122 2023-07-14 01:06:54.521948 volttron_actuator-0.1.1a8/src/actuator/scheduler.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 volttron_actuator-0.1.1a8/setup.py
+-rw-r--r--   0        0        0     2929 1970-01-01 00:00:00.000000 volttron_actuator-0.1.1a8/PKG-INFO
```

### Comparing `volttron_actuator-0.1.1a7/LICENSE` & `volttron_actuator-0.1.1a8/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_actuator-0.1.1a7/README.md` & `volttron_actuator-0.1.1a8/README.md`

 * *Files identical despite different names*

### Comparing `volttron_actuator-0.1.1a7/pyproject.toml` & `volttron_actuator-0.1.1a8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 warn_return_any = true
 warn_unused_configs = true
 show_error_codes = true
 exclude = ['docs/']
 
 [tool.poetry]
 name = "volttron-actuator"
-version = "0.1.1a7"
+version = "0.1.1a8"
 description = "The Actuator Agent is used to manage write access to devices. Other agents may request scheduled times, called Tasks, to interact with one or more devices."
 authors = ["Mark Bonicillo <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/VOLTTRON/volttron-actuator"
 homepage = "https://github.com/VOLTTRON/volttron-actuator"
 keywords = []
@@ -39,15 +39,15 @@
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 tzlocal = "^4.2"
 volttron = ">=10.0.4rc1,<11.0"
 types-tzlocal = "^4.2.2.2"
 
 [tool.poetry.group.dev.dependencies]
-volttron-testing = "^0.4.0rc0"
+volttron-testing = "^0.4.1rc4"
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 mock = "^4.0.3"
 pre-commit = "^2.17.0"
 yapf = "^0.32.0"
 toml = "^0.10.2"
 mypy = "^0.942"
```

### Comparing `volttron_actuator-0.1.1a7/src/actuator/__init__.py` & `volttron_actuator-0.1.1a8/src/actuator/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron_actuator-0.1.1a7/src/actuator/agent.py` & `volttron_actuator-0.1.1a8/src/actuator/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -445,14 +445,15 @@
     get_aware_utc_now,
     load_config,
     setup_logging,
     vip_main,
 )
 from volttron.utils.jsonrpc import RemoteError
 from volttron.utils.time import parse_timestamp_string
+from volttron.client.messaging.health import STATUS_BAD
 
 from actuator import unpack_legacy_message
 from actuator.scheduler import ScheduleManager
 
 VALUE_RESPONSE_PREFIX = topics.ACTUATOR_VALUE()
 REVERT_POINT_RESPONSE_PREFIX = topics.ACTUATOR_REVERTED_POINT()
 REVERT_DEVICE_RESPONSE_PREFIX = topics.ACTUATOR_REVERTED_DEVICE()
@@ -554,15 +555,15 @@
         self.heartbeat_interval = heartbeat_interval
         self._schedule_manager = None
         self.schedule_publish_interval = schedule_publish_interval
         self.subscriptions_setup = False
         #Only turn this on once we have confirmation from the config store.
         self.allow_no_lock_write = False
         self._update_event_time = None
-
+        self.driver_vip_identity = None
         self.default_config = {
             "heartbeat_interval": heartbeat_interval,
             "schedule_publish_interval": schedule_publish_interval,
             "preempt_grace_time": preempt_grace_time,
             "driver_vip_identity": driver_vip_identity,
             "allow_no_lock_write": allow_no_lock_write
         }
@@ -581,25 +582,44 @@
             schedule_publish_interval = float(config["schedule_publish_interval"])
 
             heartbeat_interval = float(config["heartbeat_interval"])
             preempt_grace_time = float(config["preempt_grace_time"])
             allow_no_lock_write = bool(config["allow_no_lock_write"])
         except ValueError as e:
             _log.error("ERROR PROCESSING CONFIGURATION: {}".format(e))
-            #TODO: set a health status for the agent
+            self.vip.health.set_status(STATUS_BAD, "Error processing configuration: {e}")
             return
 
+        _log.debug(f"Configuring Actuator Agent. driver vip id is: {driver_vip_identity}")
+        if action == "NEW":
+            count = 0
+            # may be both driver and actuator was auto started with the same priority.
+            # retry for a minute
+            while not self._is_driver_running(driver_vip_identity) and count < 12:
+                count = count + 1
+                gevent.sleep(5)
+            if not self._is_driver_running(driver_vip_identity):
+                _log.error("Configuration of actuator agent failed. Start driver agent and restart actuator")
+                return
+        else:
+            if not self._is_driver_running(driver_vip_identity):
+                # if this is not the first time. i.e. this is a config store update, don't retry simply abort
+                # config change and return
+                _log.error(f"Configuration update of actuator agent failed. Configured driver agent with vip "
+                           f"identity, {driver_vip_identity}, is NOT running")
+                return
+
         self.driver_vip_identity = driver_vip_identity
         self.schedule_publish_interval = schedule_publish_interval
         self.allow_no_lock_write = allow_no_lock_write
 
         _log.debug("PlatformDriver VIP IDENTITY: {}".format(self.driver_vip_identity))
         _log.debug("Schedule publish interval: {}".format(self.schedule_publish_interval))
 
-        #Only restart the heartbeat if it changes.
+        # Only restart the heartbeat if it changes.
         if (self.heartbeat_interval != heartbeat_interval or action == "NEW"
                 or self.heartbeat_greenlet is None):
             if self.heartbeat_greenlet is not None:
                 self.heartbeat_greenlet.kill()
 
             self.heartbeat_interval = heartbeat_interval
 
@@ -614,15 +634,15 @@
             except KeyError:
                 state_string = None
             self._setup_schedule(preempt_grace_time, state_string)
         else:
             self._schedule_manager.set_grace_period(preempt_grace_time)
 
         if not self.subscriptions_setup and self._schedule_manager is not None:
-            #Do this after the scheduler is setup.
+            # Do this after the scheduler is setup.
             self.vip.pubsub.subscribe(peer='pubsub',
                                       prefix=topics.ACTUATOR_GET(),
                                       callback=self.handle_get)
 
             self.vip.pubsub.subscribe(peer='pubsub',
                                       prefix=topics.ACTUATOR_SET(),
                                       callback=self.handle_set)
@@ -637,16 +657,35 @@
 
             self.vip.pubsub.subscribe(peer='pubsub',
                                       prefix=topics.ACTUATOR_REVERT_DEVICE(),
                                       callback=self.handle_revert_device)
 
             self.subscriptions_setup = True
 
+    def _is_driver_running(self, driver_vip_id):
+        # validate driver vip identity. driver agent should be running
+        peers = self.vip.peerlist().get(timeout=5)
+
+        if driver_vip_id in peers:
+            return True
+        else:
+            self.vip.health.set_status(STATUS_BAD, f"Platform driver agent with vip identity, {driver_vip_id}, "
+                                                   f"is NOT running")
+            _log.error(f"Platform driver agent with vip identity, {driver_vip_id}, is NOT running. "
+                       f"Please make sure a volttron platform driver agent is installed and running "
+                       f"(vctl install volttron-driver). Actuator by default looks for driver agent with vip id "
+                       f"'platform.driver. To point to a different vip id, configure it using driver_vip_identity "
+                       f"parameter in this agent's configuration")
+            # return as nothing much can be done till driver is up
+            return False
+
     def _heart_beat(self):
-        _log.debug("sending heartbeat")
+        if self.driver_vip_identity is None or not self._is_driver_running(self.driver_vip_identity):
+            _log.warning("Platform driver is not running")
+            return
         try:
             self.vip.rpc.call(self.driver_vip_identity, 'heart_beat').get(timeout=20.0)
         except Unreachable:
             _log.warning("Platform driver is not running")
         except (Exception, gevent.Timeout) as e:
             _log.warning(''.join([e.__class__.__name__, '(', str(e), ')']))
 
@@ -675,17 +714,17 @@
         test_now = get_aware_utc_now()
         if test_now - now > datetime.timedelta(minutes=3):
             now = test_now
         _log.debug("In _update_device_state_and_schedule: now is {}".format(now))
         self._device_states = self._schedule_manager.get_schedule_state(now)
         _log.debug("device states is {}".format(self._device_states))
 
-        #device_only and publish tells us if we were called by a reservation change.
-        #If we are being called as part of a regularly scheduled publish
-        #we ignore our previous publish schedule time.
+        # device_only and publish tells us if we were called by a reservation change.
+        # If we are being called as part of a regularly scheduled publish
+        # we ignore our previous publish schedule time.
         if device_only is None and publish:
             self._update_event_time = None
 
         schedule_next_event_time = self._schedule_manager.get_next_event_time(now)
         _log.debug("schedule_next_event_time is {}".format(schedule_next_event_time))
         new_update_event_time = self._get_adjusted_next_event_time(now, schedule_next_event_time,
                                                                    self._update_event_time)
```

### Comparing `volttron_actuator-0.1.1a7/src/actuator/scheduler.py` & `volttron_actuator-0.1.1a8/src/actuator/scheduler.py`

 * *Files identical despite different names*

### Comparing `volttron_actuator-0.1.1a7/setup.py` & `volttron_actuator-0.1.1a8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'volttron>=10.0.4rc1,<11.0']
 
 entry_points = \
 {'console_scripts': ['volttron-actuator = actuator.agent:main']}
 
 setup_kwargs = {
     'name': 'volttron-actuator',
-    'version': '0.1.1a7',
+    'version': '0.1.1a8',
     'description': 'The Actuator Agent is used to manage write access to devices. Other agents may request scheduled times, called Tasks, to interact with one or more devices.',
     'long_description': '# volttron-actuator\n\n![Eclipse VOLTTRON 10.0.4rc](https://img.shields.io/badge/Eclipse%20VOLTTRON-10.0.4rc-red.svg)\n![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)\n![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)\n[![Passing?](https://github.com/eclipse-volttron/volttron-actuator/actions/workflows/run-tests.yml/badge.svg)](https://github.com/VOLTTRON/volttron-actuator/actions/workflows/run-tests.yml)\n[![pypi version](https://img.shields.io/pypi/v/volttron-actuator.svg)](https://pypi.org/project/volttron-actuator/)\n\n\nThe Actuator Agent is used to manage write access to devices. Other agents may request scheduled times, called Tasks, to interact with one or more devices.\n\n## Requirements\n\n* python >= 3.10\n* volttron >= 10.0\n* tzlocal >= 4.2\n* types-tzlocal >= 4.2.2.2\n\n## Documentation\n\nMore detailed documentation can be found on [ReadTheDocs](https://volttron.readthedocs.io/en/modular/). The RST source\nof the documentation for this component is located in the "docs" directory of this repository.\n\n## Installation\n\nBefore installing, VOLTTRON should be installed and running.  Its virtual environment should be active.\nInformation on how to install of the VOLTTRON platform can be found\n[here](https://github.com/eclipse-volttron/volttron-core).\n\nInstall and start the volttron-actuator.\n\n```shell\nvctl install volttron-actuator --agent-config <path to agent config> --start\n```\n\nView the status of the installed agent\n\n```shell\nvctl status\n```\n\n## Development\n\nPlease see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).\n\nPlease see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)\n\n',
     'author': 'Mark Bonicillo',
     'author_email': 'volttron@pnnl.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/VOLTTRON/volttron-actuator',
```

### Comparing `volttron_actuator-0.1.1a7/PKG-INFO` & `volttron_actuator-0.1.1a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-actuator
-Version: 0.1.1a7
+Version: 0.1.1a8
 Summary: The Actuator Agent is used to manage write access to devices. Other agents may request scheduled times, called Tasks, to interact with one or more devices.
 Home-page: https://github.com/VOLTTRON/volttron-actuator
 License: Apache-2.0
 Author: Mark Bonicillo
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
```

