# Comparing `tmp/sdss_clu-2.1.0.tar.gz` & `tmp/sdss_clu-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_clu-2.1.0.tar", max compression
+gzip compressed data, was "sdss_clu-2.1.1.tar", max compression
```

## Comparing `sdss_clu-2.1.0.tar` & `sdss_clu-2.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1504 2023-06-21 19:00:04.136605 sdss_clu-2.1.0/LICENSE.md
--rw-r--r--   0        0        0     5049 2023-06-21 19:00:04.136911 sdss_clu-2.1.0/README.rst
--rw-r--r--   0        0        0     2774 2023-06-21 19:00:04.150234 sdss_clu-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      889 2023-06-21 19:00:04.150625 sdss_clu-2.1.0/python/clu/__init__.py
--rwxr-xr-x   0        0        0     9074 2023-06-21 19:00:04.150900 sdss_clu-2.1.0/python/clu/__main__.py
--rw-r--r--   0        0        0    13555 2023-06-21 19:00:04.151167 sdss_clu-2.1.0/python/clu/actor.py
--rw-r--r--   0        0        0    19832 2023-06-21 19:00:04.151454 sdss_clu-2.1.0/python/clu/base.py
--rw-r--r--   0        0        0    14705 2023-06-21 19:00:04.151738 sdss_clu-2.1.0/python/clu/client.py
--rw-r--r--   0        0        0    20069 2023-06-21 19:00:04.152048 sdss_clu-2.1.0/python/clu/command.py
--rw-r--r--   0        0        0     4135 2023-06-21 19:00:04.152368 sdss_clu-2.1.0/python/clu/device.py
--rw-r--r--   0        0        0     1347 2023-06-21 19:00:04.152584 sdss_clu-2.1.0/python/clu/exceptions.py
--rw-r--r--   0        0        0       41 2023-06-21 19:00:04.152890 sdss_clu-2.1.0/python/clu/legacy/__init__.py
--rw-r--r--   0        0        0    17892 2023-06-21 19:00:04.153192 sdss_clu-2.1.0/python/clu/legacy/actor.py
--rw-r--r--   0        0        0    13538 2023-06-21 19:00:04.153573 sdss_clu-2.1.0/python/clu/legacy/tron.py
--rw-r--r--   0        0        0        0 2023-06-21 19:00:04.153821 sdss_clu-2.1.0/python/clu/legacy/types/__init__.py
--rw-r--r--   0        0        0    15014 2023-06-21 19:00:04.154044 sdss_clu-2.1.0/python/clu/legacy/types/html.py
--rw-r--r--   0        0        0    17888 2023-06-21 19:00:04.154344 sdss_clu-2.1.0/python/clu/legacy/types/keys.py
--rw-r--r--   0        0        0    17508 2023-06-21 19:00:04.154681 sdss_clu-2.1.0/python/clu/legacy/types/messages.py
--rw-r--r--   0        0        0     9489 2023-06-21 19:00:04.154939 sdss_clu-2.1.0/python/clu/legacy/types/parser.py
--rwxr-xr-x   0        0        0      104 2023-06-21 19:00:04.155211 sdss_clu-2.1.0/python/clu/legacy/types/ply/__init__.py
--rwxr-xr-x   0        0        0    38405 2023-06-21 19:00:04.155653 sdss_clu-2.1.0/python/clu/legacy/types/ply/cpp.py
--rwxr-xr-x   0        0        0     2877 2023-06-21 19:00:04.155941 sdss_clu-2.1.0/python/clu/legacy/types/ply/ctokens.py
--rwxr-xr-x   0        0        0    45219 2023-06-21 19:00:04.156310 sdss_clu-2.1.0/python/clu/legacy/types/ply/lex.py
--rwxr-xr-x   0        0        0   140885 2023-06-21 19:00:04.157049 sdss_clu-2.1.0/python/clu/legacy/types/ply/yacc.py
--rwxr-xr-x   0        0        0     2314 2023-06-21 19:00:04.157341 sdss_clu-2.1.0/python/clu/legacy/types/ply/ygen.py
--rw-r--r--   0        0        0     5487 2023-06-21 19:00:04.157780 sdss_clu-2.1.0/python/clu/legacy/types/pvt.py
--rw-r--r--   0        0        0    19685 2023-06-21 19:00:04.158177 sdss_clu-2.1.0/python/clu/legacy/types/types.py
--rw-r--r--   0        0        0    11758 2023-06-21 19:00:04.158499 sdss_clu-2.1.0/python/clu/model.py
--rw-r--r--   0        0        0      309 2023-06-21 19:00:04.158939 sdss_clu-2.1.0/python/clu/parsers/__init__.py
--rw-r--r--   0        0        0    20428 2023-06-21 19:00:04.159248 sdss_clu-2.1.0/python/clu/parsers/click.py
--rw-r--r--   0        0        0     2685 2023-06-21 19:00:04.159550 sdss_clu-2.1.0/python/clu/parsers/json.py
--rw-r--r--   0        0        0    19724 2023-06-21 19:00:04.159899 sdss_clu-2.1.0/python/clu/protocol.py
--rw-r--r--   0        0        0     2805 2023-06-21 19:00:04.160148 sdss_clu-2.1.0/python/clu/store.py
--rw-r--r--   0        0        0     7820 2023-06-21 19:00:04.160404 sdss_clu-2.1.0/python/clu/testing.py
--rw-r--r--   0        0        0    16901 2023-06-21 19:00:04.160692 sdss_clu-2.1.0/python/clu/tools.py
--rw-r--r--   0        0        0     3648 2023-06-21 19:00:04.160967 sdss_clu-2.1.0/python/clu/websocket.py
--rw-r--r--   0        0        0     6513 1970-01-01 00:00:00.000000 sdss_clu-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-13 23:14:45.798150 sdss_clu-2.1.1/LICENSE.md
+-rw-r--r--   0        0        0     5049 2023-07-13 23:14:45.798512 sdss_clu-2.1.1/README.rst
+-rw-r--r--   0        0        0     2774 2023-07-13 23:14:45.810979 sdss_clu-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      889 2023-07-13 23:14:45.811399 sdss_clu-2.1.1/python/clu/__init__.py
+-rwxr-xr-x   0        0        0     9086 2023-07-13 23:14:45.811650 sdss_clu-2.1.1/python/clu/__main__.py
+-rw-r--r--   0        0        0    13556 2023-07-13 23:14:45.811913 sdss_clu-2.1.1/python/clu/actor.py
+-rw-r--r--   0        0        0    19832 2023-07-13 23:14:45.812217 sdss_clu-2.1.1/python/clu/base.py
+-rw-r--r--   0        0        0    14705 2023-07-13 23:14:45.812519 sdss_clu-2.1.1/python/clu/client.py
+-rw-r--r--   0        0        0    20069 2023-07-13 23:14:45.812815 sdss_clu-2.1.1/python/clu/command.py
+-rw-r--r--   0        0        0     4135 2023-07-13 23:14:45.813191 sdss_clu-2.1.1/python/clu/device.py
+-rw-r--r--   0        0        0     1347 2023-07-13 23:14:45.813419 sdss_clu-2.1.1/python/clu/exceptions.py
+-rw-r--r--   0        0        0       41 2023-07-13 23:14:45.813698 sdss_clu-2.1.1/python/clu/legacy/__init__.py
+-rw-r--r--   0        0        0    17892 2023-07-13 23:14:45.813988 sdss_clu-2.1.1/python/clu/legacy/actor.py
+-rw-r--r--   0        0        0    13538 2023-07-13 23:14:45.814278 sdss_clu-2.1.1/python/clu/legacy/tron.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:14:45.814482 sdss_clu-2.1.1/python/clu/legacy/types/__init__.py
+-rw-r--r--   0        0        0    15014 2023-07-13 23:14:45.814714 sdss_clu-2.1.1/python/clu/legacy/types/html.py
+-rw-r--r--   0        0        0    17888 2023-07-13 23:14:45.815022 sdss_clu-2.1.1/python/clu/legacy/types/keys.py
+-rw-r--r--   0        0        0    17508 2023-07-13 23:14:45.815432 sdss_clu-2.1.1/python/clu/legacy/types/messages.py
+-rw-r--r--   0        0        0     9489 2023-07-13 23:14:45.815729 sdss_clu-2.1.1/python/clu/legacy/types/parser.py
+-rwxr-xr-x   0        0        0      104 2023-07-13 23:14:45.816023 sdss_clu-2.1.1/python/clu/legacy/types/ply/__init__.py
+-rwxr-xr-x   0        0        0    38405 2023-07-13 23:14:45.816385 sdss_clu-2.1.1/python/clu/legacy/types/ply/cpp.py
+-rwxr-xr-x   0        0        0     2877 2023-07-13 23:14:45.817092 sdss_clu-2.1.1/python/clu/legacy/types/ply/ctokens.py
+-rwxr-xr-x   0        0        0    45219 2023-07-13 23:14:45.817627 sdss_clu-2.1.1/python/clu/legacy/types/ply/lex.py
+-rwxr-xr-x   0        0        0   140885 2023-07-13 23:14:45.818414 sdss_clu-2.1.1/python/clu/legacy/types/ply/yacc.py
+-rwxr-xr-x   0        0        0     2314 2023-07-13 23:14:45.818724 sdss_clu-2.1.1/python/clu/legacy/types/ply/ygen.py
+-rw-r--r--   0        0        0     5487 2023-07-13 23:14:45.818955 sdss_clu-2.1.1/python/clu/legacy/types/pvt.py
+-rw-r--r--   0        0        0    19685 2023-07-13 23:14:45.819238 sdss_clu-2.1.1/python/clu/legacy/types/types.py
+-rw-r--r--   0        0        0    11789 2023-07-13 23:14:45.819534 sdss_clu-2.1.1/python/clu/model.py
+-rw-r--r--   0        0        0      309 2023-07-13 23:14:45.819946 sdss_clu-2.1.1/python/clu/parsers/__init__.py
+-rw-r--r--   0        0        0    20428 2023-07-13 23:14:45.824817 sdss_clu-2.1.1/python/clu/parsers/click.py
+-rw-r--r--   0        0        0     2685 2023-07-13 23:14:45.825170 sdss_clu-2.1.1/python/clu/parsers/json.py
+-rw-r--r--   0        0        0    19724 2023-07-13 23:14:45.825509 sdss_clu-2.1.1/python/clu/protocol.py
+-rw-r--r--   0        0        0     2805 2023-07-13 23:14:45.825788 sdss_clu-2.1.1/python/clu/store.py
+-rw-r--r--   0        0        0     7820 2023-07-13 23:14:45.826117 sdss_clu-2.1.1/python/clu/testing.py
+-rw-r--r--   0        0        0    16901 2023-07-13 23:14:45.826432 sdss_clu-2.1.1/python/clu/tools.py
+-rw-r--r--   0        0        0     3648 2023-07-13 23:14:45.826802 sdss_clu-2.1.1/python/clu/websocket.py
+-rw-r--r--   0        0        0     6513 1970-01-01 00:00:00.000000 sdss_clu-2.1.1/PKG-INFO
```

### Comparing `sdss_clu-2.1.0/LICENSE.md` & `sdss_clu-2.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/README.rst` & `sdss_clu-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/pyproject.toml` & `sdss_clu-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-clu"
-version = "2.1.0"
+version = "2.1.1"
 description = "A new protocol for SDSS actors."
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.rst"
 homepage = "https://github.com/sdss/clu"
 repository = "https://github.com/sdss/clu"
 documentation = "https://clu.readthedocs.io/en/latest/"
```

### Comparing `sdss_clu-2.1.0/python/clu/__init__.py` & `sdss_clu-2.1.1/python/clu/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/__main__.py` & `sdss_clu-2.1.1/python/clu/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         style_name = "solarized-dark" if "solarized-dark" in STYLE_MAP else "default"
         style = style_from_pygments_cls(get_style_by_name(style_name))  # type: ignore
 
         if body:
             print_chunks.append(PygmentsTokens(body_tokens))
             print(*print_chunks, style=style, end="")
         else:
-            print(*print_chunks)  # Newline
+            print(*print_chunks, flush=True)  # Newline
 
 
 async def shell_client_prompt(
     actors: tuple[str, ...] = (),
     url: str | None = None,
     user: str = "guest",
     password: str = "guest",
```

### Comparing `sdss_clu-2.1.0/python/clu/actor.py` & `sdss_clu-2.1.1/python/clu/actor.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         # Binds the commands queue.
         self.commands_queue = await self.connection.add_queue(
             f"{self.name}_commands",
             callback=self.new_command,
             bindings=[f"command.{self.name}.#"],
         )
 
-        self.log.info(
+        self.log.debug(
             f"commands queue {self.commands_queue.name!r} "
             f"bound to {self.connection.connection.url!s}"
         )
 
         self.timed_commands.start()
 
         return self
```

### Comparing `sdss_clu-2.1.0/python/clu/base.py` & `sdss_clu-2.1.1/python/clu/base.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/client.py` & `sdss_clu-2.1.1/python/clu/client.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/command.py` & `sdss_clu-2.1.1/python/clu/command.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/device.py` & `sdss_clu-2.1.1/python/clu/device.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/exceptions.py` & `sdss_clu-2.1.1/python/clu/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/legacy/actor.py` & `sdss_clu-2.1.1/python/clu/legacy/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/legacy/tron.py` & `sdss_clu-2.1.1/python/clu/legacy/tron.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/legacy/types/html.py` & `sdss_clu-2.1.1/python/clu/legacy/types/html.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/legacy/types/keys.py` & `sdss_clu-2.1.1/python/clu/legacy/types/keys.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/legacy/types/messages.py` & `sdss_clu-2.1.1/python/clu/legacy/types/messages.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/legacy/types/parser.py` & `sdss_clu-2.1.1/python/clu/legacy/types/parser.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/legacy/types/ply/cpp.py` & `sdss_clu-2.1.1/python/clu/legacy/types/ply/cpp.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/legacy/types/ply/ctokens.py` & `sdss_clu-2.1.1/python/clu/legacy/types/ply/ctokens.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/legacy/types/ply/lex.py` & `sdss_clu-2.1.1/python/clu/legacy/types/ply/lex.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/legacy/types/ply/yacc.py` & `sdss_clu-2.1.1/python/clu/legacy/types/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/legacy/types/ply/ygen.py` & `sdss_clu-2.1.1/python/clu/legacy/types/ply/ygen.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/legacy/types/pvt.py` & `sdss_clu-2.1.1/python/clu/legacy/types/pvt.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/legacy/types/types.py` & `sdss_clu-2.1.1/python/clu/legacy/types/types.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/model.py` & `sdss_clu-2.1.1/python/clu/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -364,39 +364,44 @@
         self.client = client
         self.actors = actors
 
         self.__raise_exception = raise_exception
         self.__get_schema_command = get_schema_command
         self.__kwargs = kwargs
 
+    async def add_actor(self, actor: str):
+        """Adds an actor schema."""
+
+        schema = None
+
+        try:
+            cmd = await self.client.send_command(
+                actor,
+                self.__get_schema_command,
+                internal=True,
+            )
+            await cmd
+
+            if cmd.status.did_fail:
+                raise CluError(f"Failed getting schema for {actor}.")
+            else:
+                for reply in cmd.replies:
+                    if "schema" in reply.message:
+                        schema = json.loads(reply.message["schema"])
+                        break
+                if schema is None:
+                    raise CluError(f"{actor} did not reply with a model.")
+
+            self[actor] = Model(actor, schema, **self.__kwargs)
+
+        except Exception as err:
+            if not self.__raise_exception:
+                warnings.warn(f"Cannot load model {actor!r}. {err}", CluWarning)
+                return
+            raise
+
     async def load_schemas(self, actors: Optional[List[str]] = None):
         """Loads the actor schames."""
 
         actors = actors or self.actors or []
-        schema = None
-
         for actor in actors:
-            try:
-                cmd = await self.client.send_command(
-                    actor,
-                    self.__get_schema_command,
-                    internal=True,
-                )
-                await cmd
-
-                if cmd.status.did_fail:
-                    raise CluError(f"Failed getting schema for {actor}.")
-                else:
-                    for reply in cmd.replies:
-                        if "schema" in reply.message:
-                            schema = json.loads(reply.message["schema"])
-                            break
-                    if schema is None:
-                        raise CluError(f"{actor} did not reply with a model.")
-
-                self[actor] = Model(actor, schema, **self.__kwargs)
-
-            except Exception as err:
-                if not self.__raise_exception:
-                    warnings.warn(f"Cannot load model {actor!r}. {err}", CluWarning)
-                    continue
-                raise
+            await self.add_actor(actor)
```

### Comparing `sdss_clu-2.1.0/python/clu/parsers/click.py` & `sdss_clu-2.1.1/python/clu/parsers/click.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/parsers/json.py` & `sdss_clu-2.1.1/python/clu/parsers/json.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/protocol.py` & `sdss_clu-2.1.1/python/clu/protocol.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/store.py` & `sdss_clu-2.1.1/python/clu/store.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/testing.py` & `sdss_clu-2.1.1/python/clu/testing.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/tools.py` & `sdss_clu-2.1.1/python/clu/tools.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/python/clu/websocket.py` & `sdss_clu-2.1.1/python/clu/websocket.py`

 * *Files identical despite different names*

### Comparing `sdss_clu-2.1.0/PKG-INFO` & `sdss_clu-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-clu
-Version: 2.1.0
+Version: 2.1.1
 Summary: A new protocol for SDSS actors.
 Home-page: https://github.com/sdss/clu
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.8,<4.0
```

