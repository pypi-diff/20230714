# Comparing `tmp/markdown-to-confluence-0.1.6.tar.gz` & `tmp/markdown-to-confluence-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown-to-confluence-0.1.6.tar", last modified: Wed Jun 28 12:35:13 2023, max compression
+gzip compressed data, was "markdown-to-confluence-0.1.7.tar", last modified: Fri Jul 14 12:11:38 2023, max compression
```

## Comparing `markdown-to-confluence-0.1.6.tar` & `markdown-to-confluence-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-28 12:35:13.070721 markdown-to-confluence-0.1.6/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1077 2023-04-21 19:22:25.000000 markdown-to-confluence-0.1.6/LICENSE
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3743 2023-06-28 12:35:13.071026 markdown-to-confluence-0.1.6/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2907 2022-12-09 13:01:59.000000 markdown-to-confluence-0.1.6/README.md
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-28 12:35:13.065700 markdown-to-confluence-0.1.6/markdown_to_confluence.egg-info/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3743 2023-06-28 12:35:13.000000 markdown-to-confluence-0.1.6/markdown_to_confluence.egg-info/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      455 2023-06-28 12:35:13.000000 markdown-to-confluence-0.1.6/markdown_to_confluence.egg-info/SOURCES.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-06-28 12:35:13.000000 markdown-to-confluence-0.1.6/markdown_to_confluence.egg-info/dependency_links.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      105 2023-06-28 12:35:13.000000 markdown-to-confluence-0.1.6/markdown_to_confluence.egg-info/requires.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        8 2023-06-28 12:35:13.000000 markdown-to-confluence-0.1.6/markdown_to_confluence.egg-info/top_level.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-06-28 12:35:12.000000 markdown-to-confluence-0.1.6/markdown_to_confluence.egg-info/zip-safe
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-28 12:35:13.069494 markdown-to-confluence-0.1.6/md2conf/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      402 2023-06-28 12:33:21.000000 markdown-to-confluence-0.1.6/md2conf/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2354 2023-06-28 12:33:51.000000 markdown-to-confluence-0.1.6/md2conf/__main__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    11273 2023-05-31 12:50:28.000000 markdown-to-confluence-0.1.6/md2conf/api.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      864 2023-06-28 12:33:51.000000 markdown-to-confluence-0.1.6/md2conf/application.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     9018 2023-06-28 12:33:51.000000 markdown-to-confluence-0.1.6/md2conf/converter.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-04-21 19:11:21.000000 markdown-to-confluence-0.1.6/md2conf/py.typed
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2022-06-17 11:04:46.000000 markdown-to-confluence-0.1.6/pyproject.toml
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1106 2023-06-28 12:35:13.072240 markdown-to-confluence-0.1.6/setup.cfg
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       69 2022-06-17 11:09:13.000000 markdown-to-confluence-0.1.6/setup.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-28 12:35:13.070021 markdown-to-confluence-0.1.6/tests/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2460 2023-06-28 12:33:51.000000 markdown-to-confluence-0.1.6/tests/test_api.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:11:38.711354 markdown-to-confluence-0.1.7/
+-rw-rw-rw-   0        0        0     1098 2023-07-14 10:47:17.000000 markdown-to-confluence-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     6346 2023-07-14 12:11:38.711354 markdown-to-confluence-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5487 2023-07-14 12:04:51.000000 markdown-to-confluence-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 12:11:38.686558 markdown-to-confluence-0.1.7/markdown_to_confluence.egg-info/
+-rw-rw-rw-   0        0        0     6346 2023-07-14 12:11:38.000000 markdown-to-confluence-0.1.7/markdown_to_confluence.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      476 2023-07-14 12:11:38.000000 markdown-to-confluence-0.1.7/markdown_to_confluence.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 12:11:38.000000 markdown-to-confluence-0.1.7/markdown_to_confluence.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2023-07-14 12:11:38.000000 markdown-to-confluence-0.1.7/markdown_to_confluence.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-14 12:11:38.000000 markdown-to-confluence-0.1.7/markdown_to_confluence.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-14 10:47:45.000000 markdown-to-confluence-0.1.7/markdown_to_confluence.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-07-14 12:11:38.707083 markdown-to-confluence-0.1.7/md2conf/
+-rw-rw-rw-   0        0        0      415 2023-07-14 12:05:03.000000 markdown-to-confluence-0.1.7/md2conf/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-07-14 10:47:17.000000 markdown-to-confluence-0.1.7/md2conf/__main__.py
+-rw-rw-rw-   0        0        0    11622 2023-07-14 10:47:17.000000 markdown-to-confluence-0.1.7/md2conf/api.py
+-rw-rw-rw-   0        0        0      894 2023-07-14 10:47:17.000000 markdown-to-confluence-0.1.7/md2conf/application.py
+-rw-rw-rw-   0        0        0    11336 2023-07-14 10:47:17.000000 markdown-to-confluence-0.1.7/md2conf/converter.py
+-rw-rw-rw-   0        0        0    30752 2023-07-14 10:47:17.000000 markdown-to-confluence-0.1.7/md2conf/entities.dtd
+-rw-rw-rw-   0        0        0        0 2023-07-14 10:47:17.000000 markdown-to-confluence-0.1.7/md2conf/py.typed
+-rw-rw-rw-   0        0        0       97 2023-07-14 10:47:17.000000 markdown-to-confluence-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1169 2023-07-14 12:11:38.713351 markdown-to-confluence-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-07-14 10:47:17.000000 markdown-to-confluence-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:11:38.710396 markdown-to-confluence-0.1.7/tests/
+-rw-rw-rw-   0        0        0     2533 2023-07-14 10:47:17.000000 markdown-to-confluence-0.1.7/tests/test_api.py
```

### Comparing `markdown-to-confluence-0.1.6/md2conf/api.py` & `markdown-to-confluence-0.1.7/md2conf/api.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,349 +1,349 @@
-import json
-import logging
-import mimetypes
-import os
-import os.path
-import sys
-import typing
-from contextlib import contextmanager
-from dataclasses import dataclass
-from types import TracebackType
-from typing import Dict, Generator, List, Optional, Type, Union
-from urllib.parse import urlencode, urlparse, urlunparse
-
-import requests
-
-from .converter import ParseError, sanitize_confluence
-
-# a JSON type with possible `null` values
-JsonType = Union[
-    None,
-    bool,
-    int,
-    float,
-    str,
-    Dict[str, "JsonType"],
-    List["JsonType"],
-]
-
-
-def build_url(base_url: str, query: Optional[Dict[str, str]] = None) -> str:
-    "Builds a URL with scheme, host, port, path and query string parameters."
-
-    scheme, netloc, path, params, query_str, fragment = urlparse(base_url)
-
-    if params:
-        raise ValueError("expected: url with no parameters")
-    if query_str:
-        raise ValueError("expected: url with no query string")
-    if fragment:
-        raise ValueError("expected: url with no fragment")
-
-    url_parts = (scheme, netloc, path, None, urlencode(query) if query else None, None)
-    return urlunparse(url_parts)
-
-
-if sys.version_info >= (3, 9):
-
-    def removeprefix(string: str, prefix: str) -> str:
-        "If the string starts with the prefix, return the string without the prefix; otherwise, return the original string."
-
-        return string.removeprefix(prefix)
-
-else:
-
-    def removeprefix(string: str, prefix: str) -> str:
-        "If the string starts with the prefix, return the string without the prefix; otherwise, return the original string."
-
-        if string.startswith(prefix):
-            return string[len(prefix) :]
-        else:
-            return string
-
-
-LOGGER = logging.getLogger(__name__)
-
-
-class ConfluenceError(RuntimeError):
-    pass
-
-
-@dataclass
-class ConfluenceAttachment:
-    id: str
-    media_type: str
-    file_size: int
-    comment: str
-
-
-@dataclass
-class ConfluencePage:
-    id: str
-    title: str
-    version: int
-    content: str
-
-
-class ConfluenceAPI:
-    domain: str
-    space_key: str
-    user_name: str
-    api_key: str
-
-    session: Optional["ConfluenceSession"] = None
-
-    def __init__(
-        self,
-        domain: Optional[str] = None,
-        user_name: Optional[str] = None,
-        api_key: Optional[str] = None,
-        space_key: Optional[str] = None,
-    ) -> None:
-        opt_domain = domain or os.getenv("CONFLUENCE_DOMAIN")
-        opt_user_name = user_name or os.getenv("CONFLUENCE_USER_NAME")
-        opt_api_key = api_key or os.getenv("CONFLUENCE_API_KEY")
-        opt_space_key = space_key or os.getenv("CONFLUENCE_SPACE_KEY")
-
-        if not opt_domain:
-            raise ConfluenceError("Confluence domain not specified")
-        if not opt_user_name:
-            raise ConfluenceError("Confluence user name not specified")
-        if not opt_api_key:
-            raise ConfluenceError("Confluence API key not specified")
-        if not opt_space_key:
-            raise ConfluenceError("Confluence space key not specified")
-
-        if opt_domain.startswith(("http://", "https://")):
-            raise ConfluenceError(
-                "Confluence domain looks like a URL; only host name required"
-            )
-
-        self.domain = opt_domain
-        self.user_name = opt_user_name
-        self.api_key = opt_api_key
-        self.space_key = opt_space_key
-
-    def __enter__(self) -> "ConfluenceSession":
-        session = requests.Session()
-        session.auth = (self.user_name, self.api_key)
-        self.session = ConfluenceSession(session, self.domain, self.space_key)
-        return self.session
-
-    def __exit__(
-        self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> None:
-        if self.session is not None:
-            self.session.close()
-            self.session = None
-
-
-class ConfluenceSession:
-    session: requests.Session
-    domain: str
-    space_key: str
-
-    def __init__(self, session: requests.Session, domain: str, space_key: str) -> None:
-        self.session = session
-        self.domain = domain
-        self.space_key = space_key
-
-    def close(self) -> None:
-        self.session.close()
-
-    @contextmanager
-    def switch_space(self, new_space_key: str) -> Generator[None, None, None]:
-        old_space_key = self.space_key
-        self.space_key = new_space_key
-        try:
-            yield
-        finally:
-            self.space_key = old_space_key
-
-    def _build_url(self, path: str, query: Optional[Dict[str, str]] = None) -> str:
-        base_url = f"https://{self.domain}/wiki/rest/api{path}"
-        return build_url(base_url, query)
-
-    def _invoke(self, path: str, query: Dict[str, str]) -> JsonType:
-        url = self._build_url(path, query)
-        response = self.session.get(url)
-        response.raise_for_status()
-        return response.json()
-
-    def _save(self, path: str, data: dict) -> None:
-        url = self._build_url(path)
-        response = self.session.put(
-            url,
-            data=json.dumps(data),
-            headers={"Content-Type": "application/json"},
-        )
-        response.raise_for_status()
-
-    def get_attachment_by_name(
-        self, page_id: str, filename: str
-    ) -> ConfluenceAttachment:
-        path = f"/content/{page_id}/child/attachment"
-        query = {"spaceKey": self.space_key, "filename": filename}
-        data = typing.cast(Dict[str, JsonType], self._invoke(path, query))
-
-        results = typing.cast(List[JsonType], data["results"])
-        if len(results) != 1:
-            raise ConfluenceError(f"no such attachment on page {page_id}: {filename}")
-        result = typing.cast(Dict[str, JsonType], results[0])
-
-        id = typing.cast(str, result["id"])
-        extensions = typing.cast(Dict[str, JsonType], result["extensions"])
-        media_type = typing.cast(str, extensions["mediaType"])
-        file_size = typing.cast(int, extensions["fileSize"])
-        comment = typing.cast(str, extensions["comment"])
-        return ConfluenceAttachment(id, media_type, file_size, comment)
-
-    def upload_attachment(
-        self,
-        page_id: str,
-        attachment_path: str,
-        attachment_name: str,
-        comment: Optional[str] = None,
-    ) -> None:
-        content_type = mimetypes.guess_type(attachment_path, strict=True)[0]
-
-        if not os.path.isfile(attachment_path):
-            raise ConfluenceError(f"file not found: {attachment_path}")
-
-        try:
-            attachment = self.get_attachment_by_name(page_id, attachment_name)
-
-            if attachment.file_size == os.path.getsize(attachment_path):
-                LOGGER.info("Up-to-date attachment: %s", attachment_name)
-                return
-
-            id = removeprefix(attachment.id, "att")
-            path = f"/content/{page_id}/child/attachment/{id}/data"
-
-        except ConfluenceError:
-            path = f"/content/{page_id}/child/attachment"
-
-        url = self._build_url(path)
-
-        with open(attachment_path, "rb") as attachment_file:
-            file_to_upload = {
-                "comment": comment,
-                "file": (
-                    attachment_name,  # will truncate path component
-                    attachment_file,
-                    content_type,
-                    {"Expires": "0"},
-                ),
-            }
-            LOGGER.info("Uploading attachment: %s", attachment_name)
-            response = self.session.post(
-                url,
-                files=file_to_upload,  # type: ignore
-                headers={"X-Atlassian-Token": "no-check"},
-            )
-
-        response.raise_for_status()
-        data = response.json()
-
-        if "results" in data:
-            result = data["results"][0]
-        else:
-            result = data
-
-        attachment_id = result["id"]
-        version = result["version"]["number"] + 1
-
-        # ensure path component is retained in attachment name
-        self._update_attachment(page_id, attachment_id, version, attachment_name)
-
-    def _update_attachment(
-        self, page_id: str, attachment_id: str, version: int, attachment_title: str
-    ) -> None:
-        id = removeprefix(attachment_id, "att")
-        path = f"/content/{page_id}/child/attachment/{id}"
-        data = {
-            "id": attachment_id,
-            "type": "attachment",
-            "status": "current",
-            "title": attachment_title,
-            "space": {"key": self.space_key},
-            "version": {"minorEdit": True, "number": version},
-        }
-
-        LOGGER.info("Updating attachment: %s", attachment_id)
-        self._save(path, data)
-
-    def get_page_id_by_title(self, title: str) -> str:
-        """
-        Retrieve a Confluence wiki page details by title.
-
-        :param title: The page title.
-        :returns: Confluence page info.
-        """
-
-        LOGGER.info("Looking up page with title: %s", title)
-        path = "/content"
-        query = {"title": title, "spaceKey": self.space_key}
-        data = typing.cast(Dict[str, JsonType], self._invoke(path, query))
-
-        results = typing.cast(List[JsonType], data["results"])
-        if len(results) != 1:
-            raise ConfluenceError(f"page not found with title: {title}")
-
-        result = typing.cast(Dict[str, JsonType], results[0])
-        id = typing.cast(str, result["id"])
-        return id
-
-    def get_page(self, page_id: str) -> ConfluencePage:
-        path = f"/content/{page_id}"
-        query = {
-            "spaceKey": self.space_key,
-            "expand": "body.storage,version",
-        }
-        data = typing.cast(Dict[str, JsonType], self._invoke(path, query))
-        version = typing.cast(Dict[str, JsonType], data["version"])
-        body = typing.cast(Dict[str, JsonType], data["body"])
-        storage = typing.cast(Dict[str, JsonType], body["storage"])
-
-        return ConfluencePage(
-            id=page_id,
-            title=typing.cast(str, data["title"]),
-            version=typing.cast(int, version["number"]),
-            content=typing.cast(str, storage["value"]),
-        )
-
-    def get_page_version(self, page_id: str) -> int:
-        path = f"/content/{page_id}"
-        query = {
-            "spaceKey": self.space_key,
-            "expand": "version",
-        }
-        data = typing.cast(Dict[str, JsonType], self._invoke(path, query))
-        version = typing.cast(Dict[str, JsonType], data["version"])
-        return typing.cast(int, version["number"])
-
-    def update_page(self, page_id: str, new_content: str) -> None:
-        page = self.get_page(page_id)
-
-        try:
-            old_content = sanitize_confluence(page.content)
-            if old_content == new_content:
-                LOGGER.info("Up-to-date page: %s", page_id)
-                return
-        except ParseError as exc:
-            LOGGER.warning(exc)
-
-        path = f"/content/{page_id}"
-        data = {
-            "id": page_id,
-            "type": "page",
-            "title": page.title,
-            "space": {"key": self.space_key},
-            "body": {"storage": {"value": new_content, "representation": "storage"}},
-            "version": {"minorEdit": True, "number": page.version + 1},
-        }
-
-        LOGGER.info("Updating page: %s", page_id)
-        self._save(path, data)
+import json
+import logging
+import mimetypes
+import os
+import os.path
+import sys
+import typing
+from contextlib import contextmanager
+from dataclasses import dataclass
+from types import TracebackType
+from typing import Dict, Generator, List, Optional, Type, Union
+from urllib.parse import urlencode, urlparse, urlunparse
+
+import requests
+
+from .converter import ParseError, sanitize_confluence
+
+# a JSON type with possible `null` values
+JsonType = Union[
+    None,
+    bool,
+    int,
+    float,
+    str,
+    Dict[str, "JsonType"],
+    List["JsonType"],
+]
+
+
+def build_url(base_url: str, query: Optional[Dict[str, str]] = None) -> str:
+    "Builds a URL with scheme, host, port, path and query string parameters."
+
+    scheme, netloc, path, params, query_str, fragment = urlparse(base_url)
+
+    if params:
+        raise ValueError("expected: url with no parameters")
+    if query_str:
+        raise ValueError("expected: url with no query string")
+    if fragment:
+        raise ValueError("expected: url with no fragment")
+
+    url_parts = (scheme, netloc, path, None, urlencode(query) if query else None, None)
+    return urlunparse(url_parts)
+
+
+if sys.version_info >= (3, 9):
+
+    def removeprefix(string: str, prefix: str) -> str:
+        "If the string starts with the prefix, return the string without the prefix; otherwise, return the original string."
+
+        return string.removeprefix(prefix)
+
+else:
+
+    def removeprefix(string: str, prefix: str) -> str:
+        "If the string starts with the prefix, return the string without the prefix; otherwise, return the original string."
+
+        if string.startswith(prefix):
+            return string[len(prefix) :]
+        else:
+            return string
+
+
+LOGGER = logging.getLogger(__name__)
+
+
+class ConfluenceError(RuntimeError):
+    pass
+
+
+@dataclass
+class ConfluenceAttachment:
+    id: str
+    media_type: str
+    file_size: int
+    comment: str
+
+
+@dataclass
+class ConfluencePage:
+    id: str
+    title: str
+    version: int
+    content: str
+
+
+class ConfluenceAPI:
+    domain: str
+    space_key: str
+    user_name: str
+    api_key: str
+
+    session: Optional["ConfluenceSession"] = None
+
+    def __init__(
+        self,
+        domain: Optional[str] = None,
+        user_name: Optional[str] = None,
+        api_key: Optional[str] = None,
+        space_key: Optional[str] = None,
+    ) -> None:
+        opt_domain = domain or os.getenv("CONFLUENCE_DOMAIN")
+        opt_user_name = user_name or os.getenv("CONFLUENCE_USER_NAME")
+        opt_api_key = api_key or os.getenv("CONFLUENCE_API_KEY")
+        opt_space_key = space_key or os.getenv("CONFLUENCE_SPACE_KEY")
+
+        if not opt_domain:
+            raise ConfluenceError("Confluence domain not specified")
+        if not opt_user_name:
+            raise ConfluenceError("Confluence user name not specified")
+        if not opt_api_key:
+            raise ConfluenceError("Confluence API key not specified")
+        if not opt_space_key:
+            raise ConfluenceError("Confluence space key not specified")
+
+        if opt_domain.startswith(("http://", "https://")):
+            raise ConfluenceError(
+                "Confluence domain looks like a URL; only host name required"
+            )
+
+        self.domain = opt_domain
+        self.user_name = opt_user_name
+        self.api_key = opt_api_key
+        self.space_key = opt_space_key
+
+    def __enter__(self) -> "ConfluenceSession":
+        session = requests.Session()
+        session.auth = (self.user_name, self.api_key)
+        self.session = ConfluenceSession(session, self.domain, self.space_key)
+        return self.session
+
+    def __exit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc_val: Optional[BaseException],
+        exc_tb: Optional[TracebackType],
+    ) -> None:
+        if self.session is not None:
+            self.session.close()
+            self.session = None
+
+
+class ConfluenceSession:
+    session: requests.Session
+    domain: str
+    space_key: str
+
+    def __init__(self, session: requests.Session, domain: str, space_key: str) -> None:
+        self.session = session
+        self.domain = domain
+        self.space_key = space_key
+
+    def close(self) -> None:
+        self.session.close()
+
+    @contextmanager
+    def switch_space(self, new_space_key: str) -> Generator[None, None, None]:
+        old_space_key = self.space_key
+        self.space_key = new_space_key
+        try:
+            yield
+        finally:
+            self.space_key = old_space_key
+
+    def _build_url(self, path: str, query: Optional[Dict[str, str]] = None) -> str:
+        base_url = f"https://{self.domain}/wiki/rest/api{path}"
+        return build_url(base_url, query)
+
+    def _invoke(self, path: str, query: Dict[str, str]) -> JsonType:
+        url = self._build_url(path, query)
+        response = self.session.get(url)
+        response.raise_for_status()
+        return response.json()
+
+    def _save(self, path: str, data: dict) -> None:
+        url = self._build_url(path)
+        response = self.session.put(
+            url,
+            data=json.dumps(data),
+            headers={"Content-Type": "application/json"},
+        )
+        response.raise_for_status()
+
+    def get_attachment_by_name(
+        self, page_id: str, filename: str
+    ) -> ConfluenceAttachment:
+        path = f"/content/{page_id}/child/attachment"
+        query = {"spaceKey": self.space_key, "filename": filename}
+        data = typing.cast(Dict[str, JsonType], self._invoke(path, query))
+
+        results = typing.cast(List[JsonType], data["results"])
+        if len(results) != 1:
+            raise ConfluenceError(f"no such attachment on page {page_id}: {filename}")
+        result = typing.cast(Dict[str, JsonType], results[0])
+
+        id = typing.cast(str, result["id"])
+        extensions = typing.cast(Dict[str, JsonType], result["extensions"])
+        media_type = typing.cast(str, extensions["mediaType"])
+        file_size = typing.cast(int, extensions["fileSize"])
+        comment = typing.cast(str, extensions["comment"])
+        return ConfluenceAttachment(id, media_type, file_size, comment)
+
+    def upload_attachment(
+        self,
+        page_id: str,
+        attachment_path: str,
+        attachment_name: str,
+        comment: Optional[str] = None,
+    ) -> None:
+        content_type = mimetypes.guess_type(attachment_path, strict=True)[0]
+
+        if not os.path.isfile(attachment_path):
+            raise ConfluenceError(f"file not found: {attachment_path}")
+
+        try:
+            attachment = self.get_attachment_by_name(page_id, attachment_name)
+
+            if attachment.file_size == os.path.getsize(attachment_path):
+                LOGGER.info("Up-to-date attachment: %s", attachment_name)
+                return
+
+            id = removeprefix(attachment.id, "att")
+            path = f"/content/{page_id}/child/attachment/{id}/data"
+
+        except ConfluenceError:
+            path = f"/content/{page_id}/child/attachment"
+
+        url = self._build_url(path)
+
+        with open(attachment_path, "rb") as attachment_file:
+            file_to_upload = {
+                "comment": comment,
+                "file": (
+                    attachment_name,  # will truncate path component
+                    attachment_file,
+                    content_type,
+                    {"Expires": "0"},
+                ),
+            }
+            LOGGER.info("Uploading attachment: %s", attachment_name)
+            response = self.session.post(
+                url,
+                files=file_to_upload,  # type: ignore
+                headers={"X-Atlassian-Token": "no-check"},
+            )
+
+        response.raise_for_status()
+        data = response.json()
+
+        if "results" in data:
+            result = data["results"][0]
+        else:
+            result = data
+
+        attachment_id = result["id"]
+        version = result["version"]["number"] + 1
+
+        # ensure path component is retained in attachment name
+        self._update_attachment(page_id, attachment_id, version, attachment_name)
+
+    def _update_attachment(
+        self, page_id: str, attachment_id: str, version: int, attachment_title: str
+    ) -> None:
+        id = removeprefix(attachment_id, "att")
+        path = f"/content/{page_id}/child/attachment/{id}"
+        data = {
+            "id": attachment_id,
+            "type": "attachment",
+            "status": "current",
+            "title": attachment_title,
+            "space": {"key": self.space_key},
+            "version": {"minorEdit": True, "number": version},
+        }
+
+        LOGGER.info("Updating attachment: %s", attachment_id)
+        self._save(path, data)
+
+    def get_page_id_by_title(self, title: str) -> str:
+        """
+        Retrieve a Confluence wiki page details by title.
+
+        :param title: The page title.
+        :returns: Confluence page info.
+        """
+
+        LOGGER.info("Looking up page with title: %s", title)
+        path = "/content"
+        query = {"title": title, "spaceKey": self.space_key}
+        data = typing.cast(Dict[str, JsonType], self._invoke(path, query))
+
+        results = typing.cast(List[JsonType], data["results"])
+        if len(results) != 1:
+            raise ConfluenceError(f"page not found with title: {title}")
+
+        result = typing.cast(Dict[str, JsonType], results[0])
+        id = typing.cast(str, result["id"])
+        return id
+
+    def get_page(self, page_id: str) -> ConfluencePage:
+        path = f"/content/{page_id}"
+        query = {
+            "spaceKey": self.space_key,
+            "expand": "body.storage,version",
+        }
+        data = typing.cast(Dict[str, JsonType], self._invoke(path, query))
+        version = typing.cast(Dict[str, JsonType], data["version"])
+        body = typing.cast(Dict[str, JsonType], data["body"])
+        storage = typing.cast(Dict[str, JsonType], body["storage"])
+
+        return ConfluencePage(
+            id=page_id,
+            title=typing.cast(str, data["title"]),
+            version=typing.cast(int, version["number"]),
+            content=typing.cast(str, storage["value"]),
+        )
+
+    def get_page_version(self, page_id: str) -> int:
+        path = f"/content/{page_id}"
+        query = {
+            "spaceKey": self.space_key,
+            "expand": "version",
+        }
+        data = typing.cast(Dict[str, JsonType], self._invoke(path, query))
+        version = typing.cast(Dict[str, JsonType], data["version"])
+        return typing.cast(int, version["number"])
+
+    def update_page(self, page_id: str, new_content: str) -> None:
+        page = self.get_page(page_id)
+
+        try:
+            old_content = sanitize_confluence(page.content)
+            if old_content == new_content:
+                LOGGER.info("Up-to-date page: %s", page_id)
+                return
+        except ParseError as exc:
+            LOGGER.warning(exc)
+
+        path = f"/content/{page_id}"
+        data = {
+            "id": page_id,
+            "type": "page",
+            "title": page.title,
+            "space": {"key": self.space_key},
+            "body": {"storage": {"value": new_content, "representation": "storage"}},
+            "version": {"minorEdit": True, "number": page.version + 1},
+        }
+
+        LOGGER.info("Updating page: %s", page_id)
+        self._save(path, data)
```

### Comparing `markdown-to-confluence-0.1.6/setup.cfg` & `markdown-to-confluence-0.1.7/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,74 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 6d61 726b 646f 776e 2d74 6f2d 636f  = markdown-to-co
-00000020: 6e66 6c75 656e 6365 0a76 6572 7369 6f6e  nfluence.version
-00000030: 203d 2061 7474 723a 206d 6432 636f 6e66   = attr: md2conf
-00000040: 2e5f 5f76 6572 7369 6f6e 5f5f 0a64 6573  .__version__.des
-00000050: 6372 6970 7469 6f6e 203d 2050 7562 6c69  cription = Publi
-00000060: 7368 204d 6172 6b64 6f77 6e20 6669 6c65  sh Markdown file
-00000070: 7320 746f 2043 6f6e 666c 7565 6e63 6520  s to Confluence 
-00000080: 7769 6b69 0a61 7574 686f 7220 3d20 4c65  wiki.author = Le
-00000090: 7665 6e74 6520 4875 6e79 6164 690a 6175  vente Hunyadi.au
-000000a0: 7468 6f72 5f65 6d61 696c 203d 2068 756e  thor_email = hun
-000000b0: 7961 6469 4067 6d61 696c 2e63 6f6d 0a75  yadi@gmail.com.u
-000000c0: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
-000000d0: 6875 622e 636f 6d2f 6875 6e79 6164 692f  hub.com/hunyadi/
-000000e0: 6d64 3263 6f6e 660a 6c6f 6e67 5f64 6573  md2conf.long_des
-000000f0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
-00000100: 2052 4541 444d 452e 6d64 0a6c 6f6e 675f   README.md.long_
-00000110: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
-00000120: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
-00000130: 6d61 726b 646f 776e 0a6c 6963 656e 7365  markdown.license
-00000140: 203d 204d 4954 0a63 6c61 7373 6966 6965   = MIT.classifie
-00000150: 7273 203d 200a 0944 6576 656c 6f70 6d65  rs = ..Developme
-00000160: 6e74 2053 7461 7475 7320 3a3a 2035 202d  nt Status :: 5 -
-00000170: 2050 726f 6475 6374 696f 6e2f 5374 6162   Production/Stab
-00000180: 6c65 0a09 456e 7669 726f 6e6d 656e 7420  le..Environment 
-00000190: 3a3a 2043 6f6e 736f 6c65 0a09 496e 7465  :: Console..Inte
-000001a0: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-000001b0: 2045 6e64 2055 7365 7273 2f44 6573 6b74   End Users/Deskt
-000001c0: 6f70 0a09 4c69 6365 6e73 6520 3a3a 204f  op..License :: O
-000001d0: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
-000001e0: 4954 204c 6963 656e 7365 0a09 4f70 6572  IT License..Oper
-000001f0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000200: 4f53 2049 6e64 6570 656e 6465 6e74 0a09  OS Independent..
-00000210: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000220: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000230: 3a20 330a 0950 726f 6772 616d 6d69 6e67  : 3..Programming
-00000240: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000250: 686f 6e20 3a3a 2033 2e38 0a09 5072 6f67  hon :: 3.8..Prog
-00000260: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000270: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000280: 390a 0950 726f 6772 616d 6d69 6e67 204c  9..Programming L
-00000290: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000002a0: 6e20 3a3a 2033 2e31 300a 0950 726f 6772  n :: 3.10..Progr
-000002b0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000002c0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-000002d0: 310a 0954 7970 696e 6720 3a3a 2054 7970  1..Typing :: Typ
-000002e0: 6564 0a0a 5b6f 7074 696f 6e73 5d0a 7a69  ed..[options].zi
-000002f0: 705f 7361 6665 203d 2054 7275 650a 696e  p_safe = True.in
-00000300: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
-00000310: 7461 203d 2054 7275 650a 7061 636b 6167  ta = True.packag
-00000320: 6573 203d 2066 696e 643a 0a70 7974 686f  es = find:.pytho
-00000330: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000340: 2e38 0a69 6e73 7461 6c6c 5f72 6571 7569  .8.install_requi
-00000350: 7265 7320 3d20 0a09 6c78 6d6c 203e 3d20  res = ..lxml >= 
-00000360: 342e 390a 096d 6172 6b64 6f77 6e20 3e3d  4.9..markdown >=
-00000370: 2033 2e34 0a09 7079 6d64 6f77 6e2d 6578   3.4..pymdown-ex
-00000380: 7465 6e73 696f 6e73 203e 3d20 392e 3131  tensions >= 9.11
-00000390: 0a09 7265 7175 6573 7473 203e 3d20 322e  ..requests >= 2.
-000003a0: 3238 0a09 7479 7065 732d 6d61 726b 646f  28..types-markdo
-000003b0: 776e 203e 3d20 332e 340a 0974 7970 6573  wn >= 3.4..types
-000003c0: 2d72 6571 7565 7374 7320 3e3d 2032 2e32  -requests >= 2.2
-000003d0: 380a 0a5b 6f70 7469 6f6e 732e 7061 636b  8..[options.pack
-000003e0: 6167 6573 2e66 696e 645d 0a65 7863 6c75  ages.find].exclu
-000003f0: 6465 203d 200a 0974 6573 7473 2a0a 0a5b  de = ..tests*..[
-00000400: 6f70 7469 6f6e 732e 7061 636b 6167 655f  options.package_
-00000410: 6461 7461 5d0a 6d64 3263 6f6e 6620 3d20  data].md2conf = 
-00000420: 0a09 7079 2e74 7970 6564 0a0a 5b65 6767  ..py.typed..[egg
-00000430: 5f69 6e66 6f5d 0a74 6167 5f62 7569 6c64  _info].tag_build
-00000440: 203d 200a 7461 675f 6461 7465 203d 2030   = .tag_date = 0
-00000450: 0a0a                                     ..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 206d 6172 6b64 6f77 6e2d 746f 2d63   = markdown-to-c
+00000020: 6f6e 666c 7565 6e63 650d 0a76 6572 7369  onfluence..versi
+00000030: 6f6e 203d 2061 7474 723a 206d 6432 636f  on = attr: md2co
+00000040: 6e66 2e5f 5f76 6572 7369 6f6e 5f5f 0d0a  nf.__version__..
+00000050: 6465 7363 7269 7074 696f 6e20 3d20 5075  description = Pu
+00000060: 626c 6973 6820 4d61 726b 646f 776e 2066  blish Markdown f
+00000070: 696c 6573 2074 6f20 436f 6e66 6c75 656e  iles to Confluen
+00000080: 6365 2077 696b 690d 0a61 7574 686f 7220  ce wiki..author 
+00000090: 3d20 4c65 7665 6e74 6520 4875 6e79 6164  = Levente Hunyad
+000000a0: 690d 0a61 7574 686f 725f 656d 6169 6c20  i..author_email 
+000000b0: 3d20 6875 6e79 6164 6940 676d 6169 6c2e  = hunyadi@gmail.
+000000c0: 636f 6d0d 0a75 726c 203d 2068 7474 7073  com..url = https
+000000d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6875  ://github.com/hu
+000000e0: 6e79 6164 692f 6d64 3263 6f6e 660d 0a6c  nyadi/md2conf..l
+000000f0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
+00000100: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
+00000110: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
+00000120: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
+00000130: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
+00000140: 0d0a 6c69 6365 6e73 6520 3d20 4d49 540d  ..license = MIT.
+00000150: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
+00000160: 0a09 4465 7665 6c6f 706d 656e 7420 5374  ..Development St
+00000170: 6174 7573 203a 3a20 3520 2d20 5072 6f64  atus :: 5 - Prod
+00000180: 7563 7469 6f6e 2f53 7461 626c 650d 0a09  uction/Stable...
+00000190: 456e 7669 726f 6e6d 656e 7420 3a3a 2043  Environment :: C
+000001a0: 6f6e 736f 6c65 0d0a 0949 6e74 656e 6465  onsole...Intende
+000001b0: 6420 4175 6469 656e 6365 203a 3a20 456e  d Audience :: En
+000001c0: 6420 5573 6572 732f 4465 736b 746f 700d  d Users/Desktop.
+000001d0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
+000001e0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
+000001f0: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
+00000200: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
+00000210: 5320 496e 6465 7065 6e64 656e 740d 0a09  S Independent...
+00000220: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000230: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000240: 3a20 330d 0a09 5072 6f67 7261 6d6d 696e  : 3...Programmin
+00000250: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000260: 7468 6f6e 203a 3a20 332e 380d 0a09 5072  thon :: 3.8...Pr
+00000270: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000280: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000290: 332e 390d 0a09 5072 6f67 7261 6d6d 696e  3.9...Programmin
+000002a0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000002b0: 7468 6f6e 203a 3a20 332e 3130 0d0a 0950  thon :: 3.10...P
+000002c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000002d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000002e0: 2033 2e31 310d 0a09 5479 7069 6e67 203a   3.11...Typing :
+000002f0: 3a20 5479 7065 640d 0a0d 0a5b 6f70 7469  : Typed....[opti
+00000300: 6f6e 735d 0d0a 7a69 705f 7361 6665 203d  ons]..zip_safe =
+00000310: 2054 7275 650d 0a69 6e63 6c75 6465 5f70   True..include_p
+00000320: 6163 6b61 6765 5f64 6174 6120 3d20 5472  ackage_data = Tr
+00000330: 7565 0d0a 7061 636b 6167 6573 203d 2066  ue..packages = f
+00000340: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
+00000350: 7569 7265 7320 3d20 3e3d 332e 380d 0a69  uires = >=3.8..i
+00000360: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
+00000370: 3d20 0d0a 096c 786d 6c20 3e3d 2034 2e39  = ...lxml >= 4.9
+00000380: 0d0a 096d 6172 6b64 6f77 6e20 3e3d 2033  ...markdown >= 3
+00000390: 2e34 0d0a 0970 796d 646f 776e 2d65 7874  .4...pymdown-ext
+000003a0: 656e 7369 6f6e 7320 3e3d 2039 2e31 310d  ensions >= 9.11.
+000003b0: 0a09 7265 7175 6573 7473 203e 3d20 322e  ..requests >= 2.
+000003c0: 3238 0d0a 0974 7970 6573 2d6d 6172 6b64  28...types-markd
+000003d0: 6f77 6e20 3e3d 2033 2e34 0d0a 0974 7970  own >= 3.4...typ
+000003e0: 6573 2d72 6571 7565 7374 7320 3e3d 2032  es-requests >= 2
+000003f0: 2e32 380d 0a0d 0a5b 6f70 7469 6f6e 732e  .28....[options.
+00000400: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+00000410: 6578 636c 7564 6520 3d20 0d0a 0974 6573  exclude = ...tes
+00000420: 7473 2a0d 0a0d 0a5b 6f70 7469 6f6e 732e  ts*....[options.
+00000430: 7061 636b 6167 655f 6461 7461 5d0d 0a6d  package_data]..m
+00000440: 6432 636f 6e66 203d 200d 0a09 656e 7469  d2conf = ...enti
+00000450: 7469 6573 2e64 7464 0d0a 0970 792e 7479  ties.dtd...py.ty
+00000460: 7065 640d 0a0d 0a5b 6567 675f 696e 666f  ped....[egg_info
+00000470: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000480: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000490: 0a                                       .
```

### Comparing `markdown-to-confluence-0.1.6/tests/test_api.py` & `markdown-to-confluence-0.1.7/tests/test_api.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-import logging
-import os
-import os.path
-import unittest
-
-from md2conf.api import ConfluenceAPI, ConfluenceAttachment, ConfluencePage
-from md2conf.application import synchronize_page
-from md2conf.converter import (
-    ConfluenceDocument,
-    ConfluenceDocumentOptions,
-    sanitize_confluence,
-)
-
-logging.basicConfig(
-    level=logging.INFO,
-    format="%(asctime)s - %(levelname)s - %(funcName)s [%(lineno)d] - %(message)s",
-)
-
-
-class TestAPI(unittest.TestCase):
-    def test_markdown(self) -> None:
-        document = ConfluenceDocument("example.md", ConfluenceDocumentOptions())
-        self.assertListEqual(document.links, [])
-        self.assertListEqual(
-            document.images,
-            ["figure/interoperability.png", "figure/interoperability.png"],
-        )
-
-        with open(os.path.join("tests", "output", "document.html"), "w") as f:
-            f.write(document.xhtml())
-
-    def test_find_page_by_title(self) -> None:
-        with ConfluenceAPI() as api:
-            id = api.get_page_id_by_title("Publish to Confluence")
-            self.assertEqual(id, "85668266616")
-
-    def test_switch_space(self) -> None:
-        with ConfluenceAPI(space_key="PLAT") as api:
-            with api.switch_space("DAP"):
-                id = api.get_page_id_by_title("Publish to Confluence")
-                self.assertEqual(id, "85668266616")
-
-    def test_get_page(self) -> None:
-        with ConfluenceAPI() as api:
-            page = api.get_page("85668266616")
-            self.assertIsInstance(page, ConfluencePage)
-
-        with open(os.path.join("tests", "output", "page.html"), "w") as f:
-            f.write(sanitize_confluence(page.content))
-
-    def test_get_attachment(self) -> None:
-        with ConfluenceAPI() as api:
-            data = api.get_attachment_by_name(
-                "85668266616", "figure/interoperability.png"
-            )
-            self.assertIsInstance(data, ConfluenceAttachment)
-
-    def test_upload_attachment(self) -> None:
-        with ConfluenceAPI() as api:
-            api.upload_attachment(
-                "85668266616",
-                os.path.join(os.getcwd(), "figure", "interoperability.png"),
-                "figure/interoperability.png",
-                "A sample figure",
-            )
-
-    def test_synchronize_page(self) -> None:
-        with ConfluenceAPI() as api:
-            synchronize_page(api, "example.md", ConfluenceDocumentOptions())
-
-
-if __name__ == "__main__":
-    unittest.main()
+import logging
+import os
+import os.path
+import unittest
+
+from md2conf.api import ConfluenceAPI, ConfluenceAttachment, ConfluencePage
+from md2conf.application import synchronize_page
+from md2conf.converter import (
+    ConfluenceDocument,
+    ConfluenceDocumentOptions,
+    sanitize_confluence,
+)
+
+logging.basicConfig(
+    level=logging.INFO,
+    format="%(asctime)s - %(levelname)s - %(funcName)s [%(lineno)d] - %(message)s",
+)
+
+
+class TestAPI(unittest.TestCase):
+    def test_markdown(self) -> None:
+        document = ConfluenceDocument("example.md", ConfluenceDocumentOptions())
+        self.assertListEqual(document.links, [])
+        self.assertListEqual(
+            document.images,
+            ["figure/interoperability.png", "figure/interoperability.png"],
+        )
+
+        with open(os.path.join("tests", "output", "document.html"), "w") as f:
+            f.write(document.xhtml())
+
+    def test_find_page_by_title(self) -> None:
+        with ConfluenceAPI() as api:
+            id = api.get_page_id_by_title("Publish to Confluence")
+            self.assertEqual(id, "85668266616")
+
+    def test_switch_space(self) -> None:
+        with ConfluenceAPI(space_key="PLAT") as api:
+            with api.switch_space("DAP"):
+                id = api.get_page_id_by_title("Publish to Confluence")
+                self.assertEqual(id, "85668266616")
+
+    def test_get_page(self) -> None:
+        with ConfluenceAPI() as api:
+            page = api.get_page("85668266616")
+            self.assertIsInstance(page, ConfluencePage)
+
+        with open(os.path.join("tests", "output", "page.html"), "w") as f:
+            f.write(sanitize_confluence(page.content))
+
+    def test_get_attachment(self) -> None:
+        with ConfluenceAPI() as api:
+            data = api.get_attachment_by_name(
+                "85668266616", "figure/interoperability.png"
+            )
+            self.assertIsInstance(data, ConfluenceAttachment)
+
+    def test_upload_attachment(self) -> None:
+        with ConfluenceAPI() as api:
+            api.upload_attachment(
+                "85668266616",
+                os.path.join(os.getcwd(), "figure", "interoperability.png"),
+                "figure/interoperability.png",
+                "A sample figure",
+            )
+
+    def test_synchronize_page(self) -> None:
+        with ConfluenceAPI() as api:
+            synchronize_page(api, "example.md", ConfluenceDocumentOptions())
+
+
+if __name__ == "__main__":
+    unittest.main()
```

