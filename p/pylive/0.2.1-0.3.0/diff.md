# Comparing `tmp/pylive-0.2.1.tar.gz` & `tmp/pylive-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pylive-0.2.1.tar", last modified: Mon Sep 30 14:24:52 2019, max compression
+gzip compressed data, was "pylive-0.3.0.tar", last modified: Fri Jul 14 21:13:20 2023, max compression
```

## Comparing `pylive-0.2.1.tar` & `pylive-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,33 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-09-30 14:24:52.000000 pylive-0.2.1/
--rw-r--r--   0 daniel     (501) staff       (20)     6558 2019-09-30 14:24:52.000000 pylive-0.2.1/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)     5122 2019-05-29 14:49:28.000000 pylive-0.2.1/README.md
--rwxr-xr-x   0 daniel     (501) staff       (20)      845 2019-09-30 14:21:00.000000 pylive-0.2.1/setup.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-09-30 14:24:52.000000 pylive-0.2.1/live/
--rw-r--r--   0 daniel     (501) staff       (20)     7923 2019-07-07 16:03:27.000000 pylive-0.2.1/live/query.py
--rw-r--r--   0 daniel     (501) staff       (20)     2071 2019-05-29 14:49:28.000000 pylive-0.2.1/live/object.py
--rw-r--r--   0 daniel     (501) staff       (20)     1287 2019-05-29 14:49:28.000000 pylive-0.2.1/live/device.py
--rw-r--r--   0 daniel     (501) staff       (20)     7729 2019-06-16 14:17:57.000000 pylive-0.2.1/live/track.py
--rw-r--r--   0 daniel     (501) staff       (20)       95 2019-05-27 21:42:45.000000 pylive-0.2.1/live/constants.py
--rw-r--r--   0 daniel     (501) staff       (20)      808 2019-05-29 14:49:28.000000 pylive-0.2.1/live/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)      758 2019-05-29 14:49:28.000000 pylive-0.2.1/live/scene.py
--rw-r--r--   0 daniel     (501) staff       (20)     2055 2019-06-16 11:44:23.000000 pylive-0.2.1/live/group.py
--rw-r--r--   0 daniel     (501) staff       (20)      389 2019-06-02 11:49:47.000000 pylive-0.2.1/live/exceptions.py
--rw-r--r--   0 daniel     (501) staff       (20)     6379 2019-05-29 14:49:28.000000 pylive-0.2.1/live/clip.py
--rw-r--r--   0 daniel     (501) staff       (20)    39705 2019-09-30 13:03:59.000000 pylive-0.2.1/live/set.py
--rw-r--r--   0 daniel     (501) staff       (20)     2047 2019-05-29 14:49:28.000000 pylive-0.2.1/live/parameter.py
--rw-r--r--   0 daniel     (501) staff       (20)       98 2019-09-30 14:24:52.000000 pylive-0.2.1/setup.cfg
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2019-09-30 14:24:52.000000 pylive-0.2.1/pylive.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)     6558 2019-09-30 14:24:52.000000 pylive-0.2.1/pylive.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      360 2019-09-30 14:24:52.000000 pylive-0.2.1/pylive.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)       22 2019-09-30 14:24:52.000000 pylive-0.2.1/pylive.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)        5 2019-09-30 14:24:52.000000 pylive-0.2.1/pylive.egg-info/top_level.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2019-09-30 14:24:52.000000 pylive-0.2.1/pylive.egg-info/dependency_links.txt
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-14 21:13:20.419553 pylive-0.3.0/
+-rw-r--r--   0 daniel     (501) staff       (20)     5875 2023-07-14 21:13:20.419631 pylive-0.3.0/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)     5354 2023-07-14 21:09:11.000000 pylive-0.3.0/README.md
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-14 21:13:20.416123 pylive-0.3.0/live/
+-rw-r--r--   0 daniel     (501) staff       (20)      644 2023-07-14 21:09:11.000000 pylive-0.3.0/live/__init__.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-14 21:13:20.417698 pylive-0.3.0/live/classes/
+-rw-r--r--   0 daniel     (501) staff       (20)      148 2023-07-14 21:09:11.000000 pylive-0.3.0/live/classes/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)     3774 2023-07-14 21:09:11.000000 pylive-0.3.0/live/classes/clip.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1650 2023-07-14 21:09:11.000000 pylive-0.3.0/live/classes/device.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1926 2023-07-14 21:09:11.000000 pylive-0.3.0/live/classes/group.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2236 2023-07-14 21:09:11.000000 pylive-0.3.0/live/classes/parameter.py
+-rw-r--r--   0 daniel     (501) staff       (20)      936 2023-07-14 21:09:11.000000 pylive-0.3.0/live/classes/scene.py
+-rw-r--r--   0 daniel     (501) staff       (20)    30329 2023-07-14 21:09:11.000000 pylive-0.3.0/live/classes/set.py
+-rw-r--r--   0 daniel     (501) staff       (20)     5911 2023-07-14 21:09:11.000000 pylive-0.3.0/live/classes/track.py
+-rw-r--r--   0 daniel     (501) staff       (20)       95 2013-08-08 16:14:39.000000 pylive-0.3.0/live/constants.py
+-rw-r--r--   0 daniel     (501) staff       (20)      422 2023-07-14 21:09:11.000000 pylive-0.3.0/live/exceptions.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1294 2023-07-14 21:09:11.000000 pylive-0.3.0/live/object.py
+-rw-r--r--   0 daniel     (501) staff       (20)     7467 2023-07-14 21:09:11.000000 pylive-0.3.0/live/query.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-14 21:13:20.418411 pylive-0.3.0/pylive.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)     5875 2023-07-14 21:13:20.000000 pylive-0.3.0/pylive.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      552 2023-07-14 21:13:20.000000 pylive-0.3.0/pylive.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-07-14 21:13:20.000000 pylive-0.3.0/pylive.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       11 2023-07-14 21:13:20.000000 pylive-0.3.0/pylive.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       11 2023-07-14 21:13:20.000000 pylive-0.3.0/pylive.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       98 2023-07-14 21:13:20.419875 pylive-0.3.0/setup.cfg
+-rwxr-xr-x   0 daniel     (501) staff       (20)      852 2023-07-14 21:10:27.000000 pylive-0.3.0/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-14 21:13:20.419426 pylive-0.3.0/tests/
+-rw-r--r--   0 daniel     (501) staff       (20)      435 2023-07-14 21:09:11.000000 pylive-0.3.0/tests/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)      181 2019-10-05 22:51:35.000000 pylive-0.3.0/tests/shared.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1235 2023-07-14 21:09:11.000000 pylive-0.3.0/tests/test_clip.py
+-rw-r--r--   0 daniel     (501) staff       (20)      862 2023-07-14 21:09:11.000000 pylive-0.3.0/tests/test_group.py
+-rw-r--r--   0 daniel     (501) staff       (20)     5049 2023-07-14 21:09:11.000000 pylive-0.3.0/tests/test_set.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2782 2023-07-14 21:09:11.000000 pylive-0.3.0/tests/test_track.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pylive-0.2.1/README.md` & `pylive-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 # PyLive
 
+**NOTE: pylive has now been updated to to interface exclusively with [AbletonOSC](https://github.com/ideoforms/AbletonOSC) for Live 11 support. Legacy LiveOSC is no longer supported beyond [v0.2.2](https://github.com/ideoforms/pylive/releases/tag/v0.2.2).**
+
 PyLive is a framework for querying and controlling Ableton Live from a standalone Python script, mediated via Open Sound Control. It is effectively an interface to the Live Control Surfaces paradigm, which means it can do anything that a hardware control surface can do, including:
 
  - query and modify global parameters such as tempo, volume, pan, quantize, arrangement time
  - query and modify properties of tracks, clips, scenes and devices
  - trigger and stop clips and scenes
 
 It can perform most of the operations described in the [LiveOSC OSC API](https://github.com/hanshuebner/LiveOSC/blob/master/OSCAPI.txt).
 
+If you are looking simply to send MIDI messages to Live, this module is not what you want. Instead, try setting up a [virtual MIDI bus](https://help.ableton.com/hc/en-us/articles/209774225-How-to-setup-a-virtual-MIDI-bus) and using [isobar](https://ideoforms.github.io/isobar/) to generate MIDI sequences.
+
 ## Requirements
 
-* [Ableton Live 9+](http://www.ableton.com/live)
-* [Python 2.6+](http://www.python.org)
-* [LiveOSC (fork)](https://github.com/ideoforms/LiveOSC): A maintained fork of the [LiveOSC](http://livecontrol.q3f.org/ableton-liveapi/liveosc/) MIDI control script, updated to work with Live 9.6 and 10. Must be installed in Live's `MIDI Remote Scripts` (see [README](https://github.com/ideoforms/LiveOSC))
-* [liblo](http://liblo.sourceforge.net/): Install via Homebrew with `brew install liblo`
+* [Ableton Live 11+](http://www.ableton.com/live)
+* [Python 3.7+](http://www.python.org)
+* [AbletonOSC](https://github.com/ideoforms/AbletonOSC)
 
 ## Installation
 
 From PyPi:
 
 ```
-pip install pylive
+pip3 install pylive
 ```
 
-Via git:
+Or via git:
 ```
 git clone https://github.com/ideoforms/pylive.git
 cd pylive
-python setup.py install
+python3 setup.py install
 ```
 
 To check that pylive is communicating successfully with Ableton Live, try running one of the [examples](examples), or run the test suite with:
 ```
-python setup.py test
+python3 setup.py test
 ```
 
 ## Usage
 
 ```python
 #------------------------------------------------------------------------
 # Basic example of pylive usage: scan a Live set, trigger a clip,
```

### Comparing `pylive-0.2.1/setup.py` & `pylive-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup(
     name = 'pylive',
-    version = '0.2.1',
+    version = '0.3.0',
     description = 'Python remote control of Ableton Live',
     long_description = open("README.md", "r").read(),
     long_description_content_type = "text/markdown",
     author = 'Daniel Jones',
     author_email = 'dan-pylive@erase.net',
     url = 'https://github.com/ideoforms/pylive',
-    packages = ['live'],
-    install_requires = ['cython', 'pyliblo >= 0.9.1'],
+    packages = find_packages(),
+    install_requires = ['python-osc'],
     keywords = ('sound', 'music', 'ableton', 'osc'),
     classifiers = [
         'Topic :: Multimedia :: Sound/Audio',
         'Topic :: Artistic Software',
         'Topic :: Communications',
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers'
```

### Comparing `pylive-0.2.1/live/query.py` & `pylive-0.3.0/live/query.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,160 +1,150 @@
-import time
-import signal
 import inspect
+import logging
+import argparse
 import threading
 
-import liblo
+from live.exceptions import LiveConnectionError
 
-from .object import LoggingObject
-from .exceptions import LiveConnectionError
+from pythonosc.dispatcher import Dispatcher
+from pythonosc.osc_server import ThreadingOSCUDPServer
+from pythonosc.udp_client import SimpleUDPClient
 
 def singleton(cls):
     instances = {}
+
     def getinstance(*args):
         if cls not in instances:
             instances[cls] = cls(*args)
         return instances[cls]
+
     return getinstance
 
 #------------------------------------------------------------------------
 # Helper methods to save instantiating an object when making calls.
 #------------------------------------------------------------------------
 
 def query(*args, **kwargs):
     return Query().query(*args, **kwargs)
 
-def cmd (*args, **kwargs):
+def cmd(*args, **kwargs):
     Query().cmd(*args, **kwargs)
 
 @singleton
-class Query(LoggingObject):
-    """ Object responsible for passing OSC queries to the LiveOSC server,
+class Query:
+    """
+    Object responsible for passing OSC queries to the LiveOSC server,
     parsing and proxying responses.
 
     This object is a singleton, under the assumption that only one Live instance
     can be running, so only one global Live Query object should be needed.
 
     Following this assumption, static helper functions also exist:
 
         live.query(path, *args)
         live.cmd(path, *args)
     """
 
-    def __init__(self, address=("localhost", 9000), listen_port=9001):
+    def __init__(self, address=("127.0.0.1", 11000), listen_port=11001):
         self.beat_callback = None
         self.startup_callback = None
         self.listen_port = listen_port
+        self.logger = logging.getLogger(__name__)
 
         #------------------------------------------------------------------------
         # Handler callbacks for particular messages from Live.
         # Used so that other processes can register callbacks when states change.
         #------------------------------------------------------------------------
         self.handlers = {}
 
         self.osc_address = address
-        self.osc_target = liblo.Address(address[0], address[1])
-        self.osc_server = liblo.Server(listen_port)
-        self.osc_server.add_method(None, None, self.handler)
-        self.osc_server_thread = None
-        self.osc_server.add_bundle_handlers(self.start_bundle_handler, self.end_bundle_handler)
+        self.osc_client = SimpleUDPClient(*address)
+
+        self.dispatcher = Dispatcher()
+        self.dispatcher.set_default_handler(self.osc_handler)
+        self.osc_server = ThreadingOSCUDPServer((address[0], listen_port),
+                                                self.dispatcher)
 
+        self.osc_server_thread = None
         self.osc_read_event = None
         self.osc_timeout = 3.0
-
         self.osc_server_events = {}
 
         self.query_address = None
         self.query_rv = []
 
         self.listen()
 
-    def osc_server_read(self):
-        while True:
-            self.osc_server.recv(10)
-
     def listen(self):
-        self.osc_server_thread = threading.Thread(target=self.osc_server_read)
+        target = self.osc_server.serve_forever
+
+        self.osc_server_thread = threading.Thread(target=target)
         self.osc_server_thread.setDaemon(True)
         self.osc_server_thread.start()
 
     def stop(self):
         """ Terminate this query object and unbind from OSC listening. """
         pass
 
-    def cmd(self, msg, *args):
+    def cmd(self, msg: str, args: tuple = ()):
         """ Send a Live command without expecting a response back:
 
             live.cmd("/live/tempo", 110.0) """
-        
-        self.log_debug("OSC output: %s %s", msg, args)
+
+        self.logger.debug("OSC output: %s %s", msg, args)
+        with open("/tmp/liveosc.log", "a") as fd:
+            import datetime
+            fd.write("%s %s %s\n" % (datetime.datetime.now(), msg, args))
         try:
-            liblo.send(self.osc_target, msg, *args)
-        except Exception as e:
-            raise LiveConnectionError("Couldn't send message to Live (is LiveOSC present and activated?)")
+            self.osc_client.send_message(msg, args)
 
-    def query(self, msg, *args, **kwargs):
-        """ Send a Live command and synchronously wait for its response:
+        except Exception as e:
+            raise LiveConnectionError("Couldn't send message to Live (is AbletonOSC present and activated?): %s" % e)
 
-            return live.query("/live/tempo")
+    def query(self, msg: str, args: tuple = (), timeout: float = None):
+        """
+        Send a Live command and synchronously wait for its response:
 
-        Returns a list of values. """
+        return live.query("/live/tempo")
 
-        #------------------------------------------------------------------------
-        # Use **kwargs because we want to be able to specify an optional kw
-        # arg after variable-length args -- 
-        # eg live.query("/set/freq", 440, 1.0, response_address = "/verify/freq")
-        #
-        # http://stackoverflow.com/questions/5940180/python-default-keyword-arguments-after-variable-length-positional-arguments
-        #------------------------------------------------------------------------
-
-        #------------------------------------------------------------------------
-        # Some calls produce responses at different addresses
-        # (eg /live/device -> /live/deviceall). Specify a response_address to
-        # take account of this.
-        #------------------------------------------------------------------------
-        response_address = kwargs.get("response_address", None)
-        if response_address:
-            response_address = response_address
-        else:
-            response_address = msg
+        Returns a list of values.
+        """
 
         #------------------------------------------------------------------------
         # Create an Event to block the thread until this response has been
         # triggered.
         #------------------------------------------------------------------------
-        self.osc_server_events[response_address] = threading.Event()
+        self.osc_server_events[msg] = threading.Event()
 
         #------------------------------------------------------------------------
         # query_rv will be populated by the callback, storing the return value
         # of the OSC query.
         #------------------------------------------------------------------------
-        self.query_address = response_address
+        self.query_address = msg
         self.query_rv = []
-        self.cmd(msg, *args)
+        self.cmd(msg, args)
 
         #------------------------------------------------------------------------
         # Wait for a response. 
         #------------------------------------------------------------------------
-        timeout = kwargs.get("timeout", self.osc_timeout)
-        rv = self.osc_server_events[response_address].wait(timeout)
+        if timeout is None:
+            timeout = self.osc_timeout
+        rv = self.osc_server_events[msg].wait(timeout)
 
         if not rv:
-            raise LiveConnectionError("Timed out waiting for response from LiveOSC. Is Live running and LiveOSC installed?")
+            self.logger.debug("Timeout during query ({msg}, {args}, {kwargs})")
+            raise LiveConnectionError("Timed out waiting for response to query: %s %s. Is Live running and LiveOSC installed?" % (self.query_address, args))
 
         return self.query_rv
 
-    def start_bundle_handler(self, *args):
-        self.log_debug("OSC: start bundle")
-
-    def end_bundle_handler(self, *args):
-        self.log_debug("OSC: end bundle")
+    def osc_handler(self, address, *args):
+        self.handler(address, args)
 
-    def handler(self, address, data, types):
-        self.log_debug("OSC input: %s %s" % (address, data))
+    def handler(self, address, data):
+        self.logger.debug("OSC input: %s %s" % (address, data))
 
         #------------------------------------------------------------------------
         # Execute any callbacks that have been registered for this message
         #------------------------------------------------------------------------
         if address in self.handlers:
             for handler in self.handlers[address]:
                 handler(*data)
@@ -164,39 +154,47 @@
         # thread event and update our return value. 
         #------------------------------------------------------------------------
         if address == self.query_address:
             self.query_rv += data
             self.osc_server_events[address].set()
             return
 
-        if address == "/live/beat":
+        if address == "/live/song/beat":
             if self.beat_callback is not None:
                 #------------------------------------------------------------------------
                 # Beat callbacks are used if we want to trigger an event on each beat,
                 # to synchronise with the timing of the Live set.
                 #
                 # Callbacks may take one argument: the current beat count.
                 # If not specified, call with 0 arguments.
                 #------------------------------------------------------------------------
-                has_arg = False
-                try:
-                    signature = inspect.signature(self.beat_callback)
-                    has_arg = len(signature.parameters) > 0
-                except:
-                    # Python 2
-                    argspec = inspect.getargspec(self.beat_callback)
-                    has_arg = len(argspec.args) > 0 and argspec.args[-1] != "self"
+                signature = inspect.signature(self.beat_callback)
+                has_arg = len(signature.parameters) > 0
 
                 if has_arg:
                     self.beat_callback(data[0])
                 else:
                     self.beat_callback()
 
-        elif address == "/remix/oscserver/startup":
+        elif address == "/live/startup":
             if self.startup_callback is not None:
                 self.startup_callback()
 
     def add_handler(self, address, handler):
         if not address in self.handlers:
             self.handlers[address] = []
         self.handlers[address].append(handler)
 
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser()
+    parser.add_argument("-v", "--verbose", action="store_true", help="Verbose output")
+    parser.add_argument("--reload", action="store_true", help="Prompt AbletonOSC to reload code")
+    args = parser.parse_args()
+    logging.basicConfig(level=logging.DEBUG if args.verbose else logging.INFO)
+
+    query = Query()
+    if args.reload:
+        query.cmd("/live/reload")
+    print("Awaiting Live events...")
+    while True:
+        cmd = input()
+        query.cmd(cmd)
```

### Comparing `pylive-0.2.1/live/device.py` & `pylive-0.3.0/live/classes/device.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-import live.query
-import live.object
+import logging
 
-import random
-
-class Device(live.LoggingObject):
+class Device:
     """ Represents an instrument or audio effect residing within a Track.
     Contains one one or more Parameters.
 
     Properties:
     track -- Track object that this Device resides within
     index -- Numeric index of this device
     name -- Human-readable name
@@ -15,18 +12,33 @@
     """
 
     def __init__(self, track, index, name):
         self.track = track
         self.index = index
         self.name = name
         self.parameters = []
+        self.logger = logging.getLogger(__name__)
 
     def __str__(self):
         return "Device (%d,%d): %s" % (self.track.index, self.index, self.name)
 
+    def __getstate__(self):
+        return {
+            "track": self.track,
+            "index": self.index,
+            "name": self.name,
+            "parameters": self.parameters,
+        }
+
+    def __setstate__(self, d: dict):
+        self.track = d["track"]
+        self.index = d["index"]
+        self.name = d["name"]
+        self.parameters = d["parameters"]
+
     @property
     def set(self):
         """ Helper function to return the Set that this Device resides within. """
         return self.track.set
 
     def set_parameter(self, index, value):
         if type(index) == int:
```

### Comparing `pylive-0.2.1/live/__init__.py` & `pylive-0.3.0/live/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,24 +20,16 @@
 
 clip = track.clips[0]
 print("clip name %s, length %d beats" % (clip.name, clip.length))
 clip.play()
 
 """
 
-__version__ = "0.2.0"
 __author__ = "Daniel Jones <http://www.erase.net/>"
-__all__ = [ "Query", "Set", "Track", "Group", "Clip", "Device", "Parameter", "Scene" ]
-
-debug = False
+__all__ = ["Query", "Set", "Track", "Group", "Clip", "Device", "Parameter", "Scene"]
 
 from .object import *
 from .constants import *
-from .set import *
+from .classes import *
 from .query import *
-from .track import *
-from .group import *
-from .clip import *
-from .scene import *
-from .device import *
-from .parameter import *
+
 from .exceptions import *
```

### Comparing `pylive-0.2.1/live/scene.py` & `pylive-0.3.0/live/classes/scene.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,10 @@
-from live.constants import *
+import logging
 
-import live.query
-import live.object
-
-import random
-
-class Scene(live.LoggingObject):
+class Scene:
     """ An object representing a single scene in a Live set.
 
     Properties:
     index -- index of this scene
     name -- human-readable name
     """
 
@@ -18,17 +13,28 @@
         
         Arguments:
         index -- index of this scene
         """
         self.set = set
         self.index = index
         self.name = None
+        self.logger = logging.getLogger(__name__)
 
     def __str__(self):
         name = ": %s" % self.name if self.name else ""
-        
+
         return "Scene (%d)%s" % (self.index, name)
 
+    def __getstate__(self):
+        return {
+            "index": self.index,
+            "name": self.name,
+        }
+
+    def __setstate__(self, d: dict):
+        self.index = d["index"]
+        self.name = d["name"]
+
     def play(self):
         """ Start playing scene. """
-        self.log_info("playing")
+        self.logger.info("playing")
         self.set.play_scene(self.index)
```

### Comparing `pylive-0.2.1/live/group.py` & `pylive-0.3.0/live/classes/group.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,63 @@
-from live.object import *
-from live.track import *
+from __future__ import annotations
 
-class Group (Track):
-    """ Represents a grouped set of Track objects.
+import logging
 
-    Properties:
-    track_index -- The numerical track index of this group
-    group_index -- Groups are auto-numbered from 0
-    name -- Human-readable name
-    tracks -- List of Track objects contained within this group
+from .track import Track
+
+class Group(Track):
+    """
+    Represents a grouped set of Track objects.
     """
 
-    def __init__(self, set, track_index, group_index, name):
-        Track.__init__(self, set, track_index, name)
+    def __init__(self, set, track_index: int, group_index: int, name: str, group: Group):
+        Track.__init__(self, set, track_index, name, group)
 
         self.track_index = track_index
         self.group_index = group_index
 
         # needed so that Clip objects can call the 'index' method on Group and Track accordingly
         # TODO: rename 'index' to 'track_index' on Track objects too
         self.index = track_index
         self.is_group = True
-        self.group = None
+        self.group: Group = None
 
-        self.tracks = []
+        self.tracks: list[Track] = []
+        self.logger = logging.getLogger(__name__)
 
     def __str__(self):
         string = "Group (%d): %s" % (self.group_index, self.name)
         if len(self.tracks):
             string = string + " [tracks %d-%d]" % (self.tracks[0].index, self.tracks[len(self.tracks) - 1].index)
         return string
 
     def __iter__(self):
         return iter(self.tracks)
 
-    @property
-    def scene_indexes(self):
-        indexes = {}
-        for track in self.tracks:
-            for index in track.scene_indexes:
-                indexes[index] = 1
-        indexes = list(indexes.keys())
-        indexes = sorted(indexes)
-        return indexes
+    def __getstate__(self):
+        return {
+            **super().__getstate__(),
+            "track_index": self.track_index,
+            "group_index": self.group_index,
+            "tracks": self.tracks,
+        }
+
+    def __setstate__(self, d: dict):
+        super().__setstate__(d)
+        self.track_index = d["track_index"]
+        self.group_index = d["group_index"]
+        self.tracks = d["tracks"]
 
     def dump(self):
-        self.log_info("%d tracks" % len(self.tracks))
+        self.logger.info("%d tracks" % len(self.tracks))
         for track in self.tracks:
             track.dump()
-    
-    @property
-    def is_playing(self):
-        for track in self.tracks:
-            if track.is_playing:
-                return True
-        return False
-
-    def stop(self):
-        """ Immediately stop group from playing. """
-        self.set.stop_track(self.track_index)
 
     @property
     def active_clips(self):
         """ Return a dictionary of all non-empty clipslots: { index : Clip, ... } """
         active_clips = [n for n in self.clips if n is not None]
         return active_clips
+
+    @property
+    def is_playing(self):
+        return any(track.is_playing for track in self.tracks)
```

### Comparing `pylive-0.2.1/live/parameter.py` & `pylive-0.3.0/live/classes/parameter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-import live.query
-import live.object
-
+import logging
 import random
+from ..query import Query
 
-class Parameter(live.LoggingObject):
-    """ Represents a parameter of a Live device (either an instrument or
-    effects unit.
-
-    Properties:
-    device -- the Device object that this Parameter belongs to
-    index -- numerical index
-    name -- name, as specified by the device 
-    value -- current value, within a parameter-specific range
-
-    minimum -- minimum value (float or int)
-    maximum -- maximum value (float or int)
+class Parameter:
+    """
+    Represents a parameter of a Live device (either an instrument or
+    effects unit.)
     """
 
     def __init__(self, device, index, name, value):
+        """
+        Args:
+            device: the Device object that this Parameter belongs to
+            index: numerical index
+            name: name, as specified by the device
+            value: current value, within a parameter-specific range
+        """
         self.device = device
         self.index = index
         self.name = name
-        self.value = value
-        self.minimum = 0.0
-        self.maximum = 1.0
+        self._value = value
+        self.min = 0.0
+        self.max = 1.0
+        self.is_quantized = False
         self.indent = 3
+        self.logger = logging.getLogger(__name__)
+
+    @property
+    def live(self):
+        return Query()
 
     def __str__(self):
-        return "Parameter (%d,%d,%d): %s (range %.3f-%.3f)" % (self.device.track.index, self.device.index, self.index, self.name, self.minimum, self.maximum)
+        return "Parameter (%d,%d,%d): %s (range %.3f-%.3f)" % (self.device.track.index, self.device.index, self.index, self.name, self.min, self.max)
 
     def is_integer(self):
         # TODO: fix for enums (such as Quality in Reverb unit). how?
         return self.name.endswith("On")
 
     @property
     def set(self):
@@ -40,24 +44,31 @@
 
     @property
     def track(self):
         """ Helper function to return the Track that this parameter resides within. """
         return self.device.track
 
     def dump(self):
-        self.log_info()
+        self.logger.info()
 
     def set_value(self, value):
-        self.set.set_device_param(self.device.track.index, self.device.index, self.index, value)
+        self._value = value
+        self.live.cmd("/live/device/set/parameter/value",
+                      (self.device.track.index, self.device.index, self.index, value))
+
     def get_value(self):
-        return self.device.track.set.get_device_param(self.device.track.index, self.device.index, self.index)
+        return self.live.query("/live/device/get/parameter/value",
+                               (self.device.track.index, self.device.index, self.index))
+
     value = property(get_value, set_value)
 
     def randomise(self):
-        """ Set the parameter's value to a uniformly random value within
-        [minimum, maximum] """
+        """
+        Set the parameter's value to a uniformly random value within
+        [min, max]
+        """
 
         if self.is_integer():
-            value = random.randint(self.minimum, self.maximum)
+            value = random.randint(self.min, self.max)
         else:
-            value = random.uniform(self.minimum, self.maximum)
+            value = random.uniform(self.min, self.max)
         self.value = value
```

