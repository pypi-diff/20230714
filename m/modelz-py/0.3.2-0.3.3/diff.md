# Comparing `tmp/modelz-py-0.3.2.tar.gz` & `tmp/modelz-py-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelz-py-0.3.2.tar", last modified: Thu Mar 30 01:52:27 2023, max compression
+gzip compressed data, was "modelz-py-0.3.3.tar", last modified: Fri Jul 14 05:42:08 2023, max compression
```

## Comparing `modelz-py-0.3.2.tar` & `modelz-py-0.3.3.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0    11350 2023-03-30 01:52:18.713414 modelz-py-0.3.2/LICENSE
--rw-r--r--   0        0        0      222 2023-03-30 01:52:18.713414 modelz-py-0.3.2/README.md
--rw-r--r--   0        0        0       68 2023-03-30 01:52:18.713414 modelz-py-0.3.2/modelz/__init__.py
--rw-r--r--   0        0        0     1832 2023-03-30 01:52:18.713414 modelz-py-0.3.2/modelz/args.py
--rw-r--r--   0        0        0     4060 2023-03-30 01:52:18.713414 modelz-py-0.3.2/modelz/client.py
--rw-r--r--   0        0        0     2106 2023-03-30 01:52:18.713414 modelz-py-0.3.2/modelz/cmd.py
--rw-r--r--   0        0        0      431 2023-03-30 01:52:18.713414 modelz-py-0.3.2/modelz/env.py
--rw-r--r--   0        0        0     1284 2023-03-30 01:52:18.713414 modelz-py-0.3.2/modelz/serde.py
--rw-r--r--   0        0        0     1151 2023-03-30 01:52:18.713414 modelz-py-0.3.2/pyproject.toml
--rw-r--r--   0        0        0       34 2023-03-30 01:52:18.713414 modelz-py-0.3.2/tests/dummy_test.py
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 modelz-py-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11350 2023-07-14 05:41:58.769980 modelz-py-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1219 2023-07-14 05:41:58.769980 modelz-py-0.3.3/README.md
+-rw-r--r--   0        0        0      128 2023-07-14 05:41:58.769980 modelz-py-0.3.3/modelz/__init__.py
+-rw-r--r--   0        0        0     2074 2023-07-14 05:41:58.769980 modelz-py-0.3.3/modelz/args.py
+-rw-r--r--   0        0        0     4533 2023-07-14 05:41:58.769980 modelz-py-0.3.3/modelz/client.py
+-rw-r--r--   0        0        0     2159 2023-07-14 05:41:58.769980 modelz-py-0.3.3/modelz/cmd.py
+-rw-r--r--   0        0        0      431 2023-07-14 05:41:58.769980 modelz-py-0.3.3/modelz/env.py
+-rw-r--r--   0        0        0      518 2023-07-14 05:41:58.769980 modelz-py-0.3.3/modelz/gradio_client.py
+-rw-r--r--   0        0        0     1285 2023-07-14 05:41:58.769980 modelz-py-0.3.3/modelz/serde.py
+-rw-r--r--   0        0        0     1418 2023-07-14 05:41:58.769980 modelz-py-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1813 2023-07-14 05:41:58.769980 modelz-py-0.3.3/tests/test_cli.py
+-rw-r--r--   0        0        0      518 2023-07-14 05:41:58.769980 modelz-py-0.3.3/tests/test_serde.py
+-rw-r--r--   0        0        0     1635 1970-01-01 00:00:00.000000 modelz-py-0.3.3/PKG-INFO
```

### Comparing `modelz-py-0.3.2/LICENSE` & `modelz-py-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `modelz-py-0.3.2/modelz/args.py` & `modelz-py-0.3.3/modelz/args.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from __future__ import annotations
-from typing import List
+
 import argparse
+from typing import List
 
 
-def parse_arguments():
+def build_argument_parser():
     parser = argparse.ArgumentParser(
         prog="modelz",
         description="modelz CLI",
     )
 
     subparser = parser.add_subparsers(dest="command")
-    inf_parser = subparser.add_parser("inference")
+    inf_parser = subparser.add_parser(
+        "inference",
+        epilog="You can pass the `key=value` format parameters after the command"
+        "like `modelz inference -d foo model=llm prompt='chat like a cat'`",
+    )
     metrics_parser = subparser.add_parser("metrics")
     subparser.add_parser("build")
 
     # inference
     inf_parser.add_argument(
         "--key",
         help="API key for Modelz, will read from env $MODELZ_API_KEY if not provided",
@@ -38,16 +43,18 @@
         "--key",
         help="API key for Modelz, will read from env $MODELZ_API_KEY if not provided",
     )
     metrics_parser.add_argument(
         "-d", "--deployment", help="deployment key", required=True
     )
 
-    # build
+    return parser
+
 
+def parse_arguments(parser: argparse.ArgumentParser):
     known, others = parser.parse_known_args()
     params = parse_unknown_args(others)
     command = known.command
     args = vars(known)
     args.pop("command")
     return command, args, params
```

### Comparing `modelz-py-0.3.2/modelz/client.py` & `modelz-py-0.3.3/modelz/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
-from typing import Any, Generator
+
 from http import HTTPStatus
+from typing import Any, Generator
 from urllib.parse import urljoin
 
 import httpx
 from rich.console import Console
 
-from .env import EnvConfig
-from .serde import Serde, SerdeEnum, TextSerde
-
+from modelz.env import EnvConfig
+from modelz.serde import Serde, SerdeEnum, TextSerde
 
 TIMEOUT = httpx.Timeout(5, read=300, write=300)
 console = Console()
 config = EnvConfig()
 DEFAULT_RESP_SERDE = TextSerde()
+DEFAULT_RETRY = 3
 
 
 class ModelzAuth(httpx.Auth):
     def __init__(self, key: str | None = None) -> None:
         self.key: str = key if key else config.api_key
         if not self.key:
             raise RuntimeError("cannot find the API key")
@@ -26,72 +27,84 @@
         self, request: httpx.Request
     ) -> Generator[httpx.Request, httpx.Response, None]:
         request.headers["X-API-Key"] = self.key
         yield request
 
 
 class ModelzResponse:
+    """Modelz internal response.
+
+    The initialization will raise an error if the response status code is not 200.
+    """
+
     def __init__(self, resp: httpx.Response, serde: Serde = DEFAULT_RESP_SERDE):
-        """Modelz internal response."""
         if resp.status_code != HTTPStatus.OK:
             console.print(f"[bold red]err[{resp.status_code}][/bold red]: {resp.text}")
             raise ValueError(f"inference err with code {resp.status_code}")
         self.resp = resp
         self.serde = serde
         self._data = None
 
     def save_to_file(self, file: str):
+        """Save the response data to a file in binary format."""
         with open(file, "wb") as f:
             f.write(self.data)
 
     @property
     def data(self) -> Any:
+        """Access the response data.
+
+        It will be decoded by the serde method provided.
+        """
         if not self._data:
             self._data = self.serde.decode(self.resp.content)
         return self._data
 
     def show(self):
+        """Display the response data in the console with color."""
         console.print(self.data)
 
 
 class ModelzClient:
+    """Create a Modelz Client.
+
+    Args:
+        deployment: deployment ID
+        key: API key
+        host: Modelz host address
+        timeout: request timeout (second)
+    """
+
     def __init__(
         self,
         deployment: str | None = None,
         key: str | None = None,
         host: str | None = None,
         timeout: float | httpx.Timeout = TIMEOUT,
     ) -> None:
-        """Create a Modelz Client.
-
-        Args:
-            deployment: deployment ID
-            key: API key
-            host: Modelz host address
-            timeout: request timeout (second)
-        """
         self.host = host if host else config.host
-        auth = ModelzAuth(key)
         self.deployment = deployment
-        self.client = httpx.Client(auth=auth)
+        auth = ModelzAuth(key)
+        transport = httpx.HTTPTransport(retries=DEFAULT_RETRY)
+        self.client = httpx.Client(auth=auth, transport=transport)
         self.serde: Serde
         self.timeout = timeout
 
     def inference(
         self,
         params: Any,
         deployment: str | None = None,
         serde: str = "json",
     ) -> ModelzResponse:
         """Get the inference result.
 
         Args:
-            params: request params, will be serialized by `serde`
+            params: request params, will be serialized by ``serde``
             deployment: deployment ID
-            serde: serialize/deserialize method, choose from ("json", "msg", "raw")
+            serde: serialize/deserialize method, choose from ("json", "msgpack", "raw")
         """
         deploy = deployment if deployment else self.deployment
         assert deploy, "deployment is required"
         self.serde = SerdeEnum[serde.lower()].value()
 
         with console.status(f"[bold green]Modelz {deploy} inference..."):
             resp = self.client.post(
@@ -116,15 +129,19 @@
                 urljoin(self.host.format(deploy), "/metrics"),
                 timeout=self.timeout,
             )
 
         return ModelzResponse(resp)
 
     def build(self, repo: str):
-        """Build a Docker image and push it to the registry."""
+        """Build a Docker image and push it to the registry.
+
+        Args:
+            repo: git repo url
+        """
         with console.status(f"[bold green]Modelz build {repo}..."):
             resp = self.client.post(
                 urljoin(self.host.format("api"), "/build"),
                 timeout=self.timeout,
             )
 
         ModelzResponse(resp)
```

### Comparing `modelz-py-0.3.2/modelz/cmd.py` & `modelz-py-0.3.3/modelz/cmd.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from typing import Optional, Dict
 import sys
+from typing import Dict, Optional
 
 from rich.console import Console
 
+from modelz.args import build_argument_parser, parse_arguments
 from modelz.client import ModelzClient
-from modelz.args import parse_arguments
-
 
 console = Console()
 
 
 def inference(
     deployment: str,
     params: Optional[Dict[str, str]] = None,
@@ -17,22 +16,22 @@
     write_file: Optional[str] = None,
     key: Optional[str] = None,
     serde: str = "json",
 ):
     """Model inference.
 
     Example:
-        `modelz inference -d $DEPLOYMENT prompt='cut cat'`
+        ``modelz inference -d $DEPLOYMENT prompt='cut cat'``
 
     Args:
         deployment: deployment id
         params: request params dict
         read_stdin: read stdin as request body
         write_file: write response to the file
-        key: API key, will try to read from env `MODELZ_API_KEY` if not provided
+        key: API key, will try to read from env ``MODELZ_API_KEY`` if not provided
         serde: serilize/deserilize method, choose from [json|msgpack|raw]
         output: output target, choose from [console|file]
     """
     data = params
     if read_stdin:
         # override req data
         data = sys.stdin.buffer.read()
@@ -47,32 +46,32 @@
         console.print(f"result has been written in [bold cyan]{write_file}[/bold cyan]")
 
 
 def metrics(deployment: str, key: Optional[str] = None):
     """Model service metrics.
 
     Usage:
-        `modelz metrics -d $DEPLOYMENT`
+        ``modelz metrics -d $DEPLOYMENT``
 
     Args:
-        key: API key, will try to read from env `MODELZ_API_KEY` if not provided
+        key: API key, will try to read from env ``MODELZ_API_KEY`` if not provided
         deployment: deployment id
     """
     client = ModelzClient(key=key, deployment=deployment)
     client.metrics().show()
 
 
 def build(repo: str, key: Optional[str] = None):
     """Build the docker image from a GitHub repo"""
     pass
 
 
 def main():
     """CLI entrypoint."""
-    command, args, params = parse_arguments()
+    command, args, params = parse_arguments(build_argument_parser())
     if command.startswith("inf"):
         inference(**args, params=params)
     elif command.startswith("metrics"):
         metrics(**args)
     elif command.startswith("build"):
         build(**args)
     else:
```

### Comparing `modelz-py-0.3.2/modelz/serde.py` & `modelz-py-0.3.3/modelz/serde.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
+
+import json
 from abc import ABC, abstractmethod
-from typing import Any
 from enum import Enum
+from typing import Any
 
-import json
 import msgpack  # type: ignore
 
 
 class Serde(ABC):
     """Serilization and deserilization."""
 
     @abstractmethod
```

